# Comparing `tmp/pythonBgt-0.45-py3-none-any.whl.zip` & `tmp/pythonBgt-0.46-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 6996 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat    18965 b- defN 23-Aug-06 12:16 pythonBgt/pythonBgt.py
+Zip file size: 7019 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat    19155 b- defN 23-Aug-06 15:58 pythonBgt/pythonBgt.py
 -rw-rw-rw-  2.0 fat       26 b- defN 22-Mar-07 18:01 pythonBgt/__init__.py
--rw-rw-rw-  2.0 fat      632 b- defN 23-Aug-06 12:16 pythonBgt-0.45.dist-info/metadata.json
--rw-rw-rw-  2.0 fat       10 b- defN 23-Aug-06 12:16 pythonBgt-0.45.dist-info/top_level.txt
--rw-rw-rw-  2.0 fat       97 b- defN 23-Aug-06 12:16 pythonBgt-0.45.dist-info/WHEEL
--rw-rw-rw-  2.0 fat      517 b- defN 23-Aug-06 12:16 pythonBgt-0.45.dist-info/METADATA
--rw-rw-rw-  2.0 fat      558 b- defN 23-Aug-06 12:16 pythonBgt-0.45.dist-info/RECORD
-7 files, 20805 bytes uncompressed, 6016 bytes compressed:  71.1%
+-rw-rw-rw-  2.0 fat      632 b- defN 23-Aug-06 16:03 pythonBgt-0.46.dist-info/metadata.json
+-rw-rw-rw-  2.0 fat       10 b- defN 23-Aug-06 16:03 pythonBgt-0.46.dist-info/top_level.txt
+-rw-rw-rw-  2.0 fat       97 b- defN 23-Aug-06 16:03 pythonBgt-0.46.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat      517 b- defN 23-Aug-06 16:03 pythonBgt-0.46.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      558 b- defN 23-Aug-06 16:03 pythonBgt-0.46.dist-info/RECORD
+7 files, 20995 bytes uncompressed, 6039 bytes compressed:  71.2%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: pythonBgt/pythonBgt.py
 Comment: 
 
 Filename: pythonBgt/__init__.py
 Comment: 
 
-Filename: pythonBgt-0.45.dist-info/metadata.json
+Filename: pythonBgt-0.46.dist-info/metadata.json
 Comment: 
 
-Filename: pythonBgt-0.45.dist-info/top_level.txt
+Filename: pythonBgt-0.46.dist-info/top_level.txt
 Comment: 
 
-Filename: pythonBgt-0.45.dist-info/WHEEL
+Filename: pythonBgt-0.46.dist-info/WHEEL
 Comment: 
 
-Filename: pythonBgt-0.45.dist-info/METADATA
+Filename: pythonBgt-0.46.dist-info/METADATA
 Comment: 
 
-Filename: pythonBgt-0.45.dist-info/RECORD
+Filename: pythonBgt-0.46.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pythonBgt/pythonBgt.py

```diff
@@ -264,15 +264,19 @@
 			self.close()
 		if not fileName in cachedFiles:
 			file=open(fileName, "rb")
 			fileContent=file.read()
 			cachedFiles[fileName]=fileContent
 		self.handle=stream.FileStream(mem=True, file=cachedFiles[fileName], length=len(cachedFiles[fileName]))
 		self.freq=self.handle.get_frequency()
-
+	def loadFromMemory(self, content):
+		if self.handle:
+			self.close()
+		self.handle=stream.FileStream(mem=True, file=content, length=len(content))
+		self.freq=self.handle.get_frequency()
 	def stream(self, path):
 		path=path.lower()
 		if self.handle:
 			self.close()
 		if path.startswith("http://") or path.startswith("https://"):
 			self.handle=stream.URLStream(path)
 		else:
```

## Comparing `pythonBgt-0.45.dist-info/metadata.json` & `pythonBgt-0.46.dist-info/metadata.json`

 * *Files 1% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9444444444444444%*

 * *Differences: {"'version'": "'0.46'"}*

```diff
@@ -31,9 +31,9 @@
                 "accessible-output2",
                 "pyperclip",
                 "pyenet310"
             ]
         }
     ],
     "summary": "PythonBgt is a library for Python that allows the easy and practical creation of audiogames, combining the flexibility and modernity of Python with the simplicity and practicality of BGT.",
-    "version": "0.45"
+    "version": "0.46"
 }
```

## Comparing `pythonBgt-0.45.dist-info/METADATA` & `pythonBgt-0.46.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.0
 Name: pythonBgt
-Version: 0.45
+Version: 0.46
 Summary: PythonBgt is a library for Python that allows the easy and practical creation of audiogames, combining the flexibility and modernity of Python with the simplicity and practicality of BGT.
 Author: Gabriel Haberkamp
 Keywords: Python,BGT,Python_Bgt,audiogame,audiogames,games
 Requires-Dist: pygame
 Requires-Dist: sound-lib
 Requires-Dist: wxpython310
 Requires-Dist: requests
```

## Comparing `pythonBgt-0.45.dist-info/RECORD` & `pythonBgt-0.46.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-pythonBgt/pythonBgt.py,sha256=twLrVH-M3NUZLmOhFE3eMJ8usGQsXBSl7KavD_J4Sg0,18965
+pythonBgt/pythonBgt.py,sha256=jdYlCgcheKbLtwKo4U8rZVVw7tulHIlogaEnsRSGdc4,19155
 pythonBgt/__init__.py,sha256=1UW_6XpPMbqVOuR-pLvL8H-i20US_b-p5FGx5tdvFTU,26
-pythonBgt-0.45.dist-info/METADATA,sha256=uSVHYpl3obiqAJUYJJJgMaVWdQWC29lFx6h-y54QRfQ,517
-pythonBgt-0.45.dist-info/metadata.json,sha256=rnTUVJG5seDTkIwf-aLubTmOWCsCdNZKPNzujJDXaWc,632
-pythonBgt-0.45.dist-info/RECORD,,
-pythonBgt-0.45.dist-info/top_level.txt,sha256=CM25HsZGfuVFKS7CsCpbSFVgiN_owg2HOjOvJ5v6toA,10
-pythonBgt-0.45.dist-info/WHEEL,sha256=R7GZBaynU7P7eIwbsGv7F-X8eM9JWO6nKzGDfrA5_lo,97
+pythonBgt-0.46.dist-info/METADATA,sha256=RI0fBjcTvihPHgF_sqhDk5jZSUpJfB6fveBfNpV_czs,517
+pythonBgt-0.46.dist-info/metadata.json,sha256=XVxfj9F40ntxnNra6UkmD4PwLLH4H8XAr40MYY8Vc-g,632
+pythonBgt-0.46.dist-info/RECORD,,
+pythonBgt-0.46.dist-info/top_level.txt,sha256=CM25HsZGfuVFKS7CsCpbSFVgiN_owg2HOjOvJ5v6toA,10
+pythonBgt-0.46.dist-info/WHEEL,sha256=R7GZBaynU7P7eIwbsGv7F-X8eM9JWO6nKzGDfrA5_lo,97
```

