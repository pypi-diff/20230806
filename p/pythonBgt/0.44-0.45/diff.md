# Comparing `tmp/pythonBgt-0.44-py3-none-any.whl.zip` & `tmp/pythonBgt-0.45-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 6685 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat    18072 b- defN 23-Apr-14 21:49 pythonBgt/pythonBgt.py
+Zip file size: 6996 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat    18965 b- defN 23-Aug-06 12:16 pythonBgt/pythonBgt.py
 -rw-rw-rw-  2.0 fat       26 b- defN 22-Mar-07 18:01 pythonBgt/__init__.py
--rw-rw-rw-  2.0 fat      632 b- defN 23-Apr-14 22:04 pythonBgt-0.44.dist-info/metadata.json
--rw-rw-rw-  2.0 fat       10 b- defN 23-Apr-14 22:04 pythonBgt-0.44.dist-info/top_level.txt
--rw-rw-rw-  2.0 fat       97 b- defN 23-Apr-14 22:04 pythonBgt-0.44.dist-info/WHEEL
--rw-rw-rw-  2.0 fat      517 b- defN 23-Apr-14 22:04 pythonBgt-0.44.dist-info/METADATA
--rw-rw-rw-  2.0 fat      558 b- defN 23-Apr-14 22:04 pythonBgt-0.44.dist-info/RECORD
-7 files, 19912 bytes uncompressed, 5705 bytes compressed:  71.3%
+-rw-rw-rw-  2.0 fat      632 b- defN 23-Aug-06 12:16 pythonBgt-0.45.dist-info/metadata.json
+-rw-rw-rw-  2.0 fat       10 b- defN 23-Aug-06 12:16 pythonBgt-0.45.dist-info/top_level.txt
+-rw-rw-rw-  2.0 fat       97 b- defN 23-Aug-06 12:16 pythonBgt-0.45.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat      517 b- defN 23-Aug-06 12:16 pythonBgt-0.45.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      558 b- defN 23-Aug-06 12:16 pythonBgt-0.45.dist-info/RECORD
+7 files, 20805 bytes uncompressed, 6016 bytes compressed:  71.1%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: pythonBgt/pythonBgt.py
 Comment: 
 
 Filename: pythonBgt/__init__.py
 Comment: 
 
-Filename: pythonBgt-0.44.dist-info/metadata.json
+Filename: pythonBgt-0.45.dist-info/metadata.json
 Comment: 
 
-Filename: pythonBgt-0.44.dist-info/top_level.txt
+Filename: pythonBgt-0.45.dist-info/top_level.txt
 Comment: 
 
-Filename: pythonBgt-0.44.dist-info/WHEEL
+Filename: pythonBgt-0.45.dist-info/WHEEL
 Comment: 
 
-Filename: pythonBgt-0.44.dist-info/METADATA
+Filename: pythonBgt-0.45.dist-info/METADATA
 Comment: 
 
-Filename: pythonBgt-0.44.dist-info/RECORD
+Filename: pythonBgt-0.45.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pythonBgt/pythonBgt.py

```diff
@@ -10,14 +10,15 @@
 evtNone=0
 evtConnect=1
 evtRecv=2
 evtDisconnect=3
 import pickle
 import pyperclip
 import wx
+from traceback import format_exception
 import sound_lib
 from sound_lib import stream, output
 from threading import Thread
 from accessible_output2 import outputs
 from copy import copy
 screenReader=outputs.auto.Auto()
 import pygame
@@ -46,14 +47,30 @@
 	return os.path.isfile(fileName)
 def dirCreate(dirName):
 	os.mkdir(dirName)
 def dirExists(dirName):
 	return os.path.isdir(dirName)
 def showWindow(windowName):
 	pygame.display.set_caption(windowName)
+def message(text, continueText="", discardKey=K_RETURN):
+	speak(text)
+	if continueText:
+		speak(continueText)
+	while not keyPressed(discardKey):
+		if keyPressed(K_LEFT) or keyPressed(K_RIGHT) or keyPressed(K_DOWN) or keyPressed(K_UP):
+			speak(text)
+		wait(5)
+def audioMessage(filePath, discardKey=K_RETURN):
+	audioFile=loadSound(filePath)
+	audioFile.play()
+	while not keyPressed(discardKey):
+		wait(5)
+	audioFile.stop()
+	audioFile.close()
+	wait(5)
 def question(title, message):
 	dial=wx.MessageDialog(None, message, title, wx.YES_NO|wx.CANCEL|wx.ICON_QUESTION)
 	answer=dial.ShowModal()
 	dial.Destroy()
 	if answer==wx.ID_YES: return 1
 	elif answer==wx.ID_NO: return 2
 	elif answer==wx.ID_CANCEL: return 3
@@ -87,14 +104,18 @@
 		self.paused=paused
 		self.pausedTime=0
 		if self.paused==False: self.start()
 	def start(self):
 		self.paused=False
 		self.pausedTime=0
 		self.initialTime=pygame.time.get_ticks()
+	def restart(self):
+		self.paused=False
+		self.pausedTime=0
+		self.initialTime=pygame.time.get_ticks()
 	@property
 	def time(self):
 		if self.paused: return self.pausedTime
 		return self.pausedTime+pygame.time.get_ticks()-self.initialTime
 	elapsed=time
 	def pause(self):
 		self.pausedTime=self.time
@@ -298,52 +319,50 @@
 		if self.handle and self.handle.is_playing:
 			self.handle.stop()
 			self.handle.set_position(0)
 
 	def stopAndPlay(self):
 		self.stop()
 		self.play()
-
-	def fadeOut(self, fadeTime):
-		if self.handle and self.handle.is_playing:
-			self.handle.slide_attribute("volume", 0, fadeTime//1000)
-
+	def fadeOut(self, fadeTime, finalVolume):
+		wait(5)
+		fadeTimer=Timer(paused=False)
+		while self.volume>finalVolume:
+			if fadeTimer.elapsed>=fadeTime:
+				self.volume-=1
+				fadeTimer.restart()
+			if keyPressed(K_RETURN):
+				break
+			wait(5)
+		self.stop()
 	def speakerTest(self, time=3000):
 		if self.handle:
 			self.playLooped()
 			self.pan=-100
 			self.handle.slide_attribute("pan", 1, time//1000)
 			while self.pan<100: wait(5)
 
 	@property
 	def active(self):
 		return self.handle.is_active()
 
 	@property
 	def volume(self):
-		if not self.handle:
-			return False
 		return round(math.log10(self.handle.volume)*20)
 	@volume.setter
 	def volume(self,value):
-		if not self.handle:
-			return False
 		self.handle.set_volume(10**(float(value)/20))
 
 	@property
 	def pitch(self):
-		if not self.handle:
-			return False
 		return (self.handle.get_frequency()/self.freq)*100
 
 	@pitch.setter
 	def pitch(self, value):
 		if value>400: value=400
-		if not self.handle:
-			return False
 		self.handle.set_frequency((float(value)/100)*self.freq)
 
 	@property
 	def position(self):
 		return round(self.handle.bytes_to_seconds()*1000)
 
 	@position.setter
@@ -366,22 +385,18 @@
 
 	@property
 	def timeLeft(self):
 		return self.length-self.position
 
 	@property
 	def pan(self):
-		if not self.handle:
-			return False
 		return self.handle.get_pan()*100
 
 	@pan.setter
 	def pan(self, value):
-		if not self.handle:
-			return False
 		self.handle.set_pan(float(value)/100)
 
 	@property
 	def playing(self):
 		if self.handle is None:
 			return False
 		try:
@@ -400,24 +415,27 @@
 	s.load(fileName)
 	return s
 def streamSound(fileName):
 	s=Sound()
 	s.stream(fileName)
 	return s
 class GameMenu:
-	def __init__(self, intro=None, introSound=None, wrap=False, escape=True, enterSound=None, clickSound=None, wrapSound=None, edgeSound=None, items=[]):
+	def __init__(self, intro=None, introSound=None, wrap=False, escape=True, enterSound=None, clickSound=None, wrapSound=None, edgeSound=None, items=None):
 		self.intro=intro
 		self.introSound=introSound
 		self.wrap=wrap
 		self.escape=escape
 		self.enterSound=enterSound
 		self.clickSound=clickSound
 		self.wrapSound=wrapSound
 		self.edgeSound=edgeSound
-		self.items=items
+		if items is None:
+			self.items=[]
+		else:
+			self.items=items
 	def show(self):
 		self.selection=None
 		self.currentSelection=1
 		if self.enterSound:
 			self.__enterObj=loadSound(self.enterSound)
 		if self.clickSound:
 			self.__clickObj=loadSound(self.clickSound)
@@ -590,21 +608,29 @@
 	if not sound.pitch==finalPitch:
 		sound.pitch=finalPitch
 def readEnvironmentVariable(name):
 	return os.environ.get(name, "")
 def waitKey(keyCode=K_RETURN):
 	wait(5)
 	while not keyPressed(keyCode): wait(5)
-def exHandler(type, ex, tb):
-	line=str(tb.tb_lineno)
-	exType=type.__name__
-	exDescript=str(ex)
-	alert("python BGT runtime error", "an error occurred on line "+line+". \n"+exType+": "+exDescript)
+def excHandler(type, exception, tb):
+	errorName=type.__name__
+	errorDescription=str(exception)
+	errorDetails=format_exception(type, exception, tb)
+	showError(errorDetails)
+def showError(errorDetails):
+	errorDial=wx.Dialog(None, title="Python BGT Runtime Error")
+	errorBox=wx.TextCtrl(errorDial, style=wx.TE_MULTILINE|wx.TE_READONLY|wx.TE_DONTWRAP, value="")
+	for detail in errorDetails:
+		errorBox.AppendText(detail)
+	errorBox.SetInsertionPoint(0)
+	closeError=wx.Button(errorDial, wx.ID_CANCEL, "&Close")
+	errorDial.ShowModal()
 	exit()
-sys.excepthook=exHandler
+sys.excepthook=excHandler
 
 def wait(time=5):
 	global keysDown
 	global oldKeys
 	global isWindowActive
 	waitTimer=Timer(paused=False)
 	while waitTimer.elapsed<time:
```

## Comparing `pythonBgt-0.44.dist-info/metadata.json` & `pythonBgt-0.45.dist-info/metadata.json`

 * *Files 1% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9444444444444444%*

 * *Differences: {"'version'": "'0.45'"}*

```diff
@@ -31,9 +31,9 @@
                 "accessible-output2",
                 "pyperclip",
                 "pyenet310"
             ]
         }
     ],
     "summary": "PythonBgt is a library for Python that allows the easy and practical creation of audiogames, combining the flexibility and modernity of Python with the simplicity and practicality of BGT.",
-    "version": "0.44"
+    "version": "0.45"
 }
```

## Comparing `pythonBgt-0.44.dist-info/METADATA` & `pythonBgt-0.45.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.0
 Name: pythonBgt
-Version: 0.44
+Version: 0.45
 Summary: PythonBgt is a library for Python that allows the easy and practical creation of audiogames, combining the flexibility and modernity of Python with the simplicity and practicality of BGT.
 Author: Gabriel Haberkamp
 Keywords: Python,BGT,Python_Bgt,audiogame,audiogames,games
 Requires-Dist: pygame
 Requires-Dist: sound-lib
 Requires-Dist: wxpython310
 Requires-Dist: requests
```

