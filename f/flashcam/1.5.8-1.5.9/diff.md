# Comparing `tmp/flashcam-1.5.8.tar.gz` & `tmp/flashcam-1.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flashcam-1.5.8.tar", last modified: Fri Jul 14 19:59:28 2023, max compression
+gzip compressed data, was "flashcam-1.5.9.tar", last modified: Sat Jul 15 09:51:01 2023, max compression
```

## Comparing `flashcam-1.5.8.tar` & `flashcam-1.5.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-14 19:59:28.885467 flashcam-1.5.8/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      850 2023-07-14 19:59:28.885467 flashcam-1.5.8/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      569 2023-07-14 19:59:26.000000 flashcam-1.5.8/README.md
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-14 19:59:28.881467 flashcam-1.5.8/bin/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    24892 2023-07-14 19:16:43.000000 flashcam-1.5.8/bin/flashcam
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      150 2023-04-17 20:01:01.000000 flashcam-1.5.8/bin/flashcam_join
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      311 2023-04-17 20:01:01.000000 flashcam-1.5.8/bin/flashcam_rep
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      551 2023-04-17 20:01:01.000000 flashcam-1.5.8/bin/flashcamg
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-14 19:59:28.881467 flashcam-1.5.8/flashcam/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      249 2023-04-17 20:01:01.000000 flashcam-1.5.8/flashcam/__init__.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     5255 2023-04-17 20:01:01.000000 flashcam-1.5.8/flashcam/base_camera2.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     8106 2023-07-13 20:56:38.000000 flashcam-1.5.8/flashcam/config.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-14 19:59:28.881467 flashcam-1.5.8/flashcam/data/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    24159 2023-04-17 20:01:01.000000 flashcam-1.5.8/flashcam/data/BEAM_OFF.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    27944 2023-04-17 20:01:01.000000 flashcam-1.5.8/flashcam/data/BEAM_ON_.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    27715 2023-04-17 20:01:01.000000 flashcam-1.5.8/flashcam/data/DET_NRDY.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    27483 2023-04-17 20:01:01.000000 flashcam-1.5.8/flashcam/data/DET_RDY_.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    34404 2023-04-17 20:01:01.000000 flashcam-1.5.8/flashcam/data/digital-7.mono.ttf
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    19991 2023-04-17 20:01:01.000000 flashcam-1.5.8/flashcam/data/monoskop.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    59930 2023-04-28 18:56:55.000000 flashcam-1.5.8/flashcam/data/win_rain.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    91079 2023-04-28 18:56:55.000000 flashcam-1.5.8/flashcam/data/win_skull.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    76270 2023-04-28 18:56:55.000000 flashcam-1.5.8/flashcam/data/win_storm.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    61604 2023-04-28 18:56:55.000000 flashcam-1.5.8/flashcam/data/win_winter.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    72731 2023-04-17 20:01:01.000000 flashcam-1.5.8/flashcam/data/windows.jpg
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4173 2023-04-17 20:01:01.000000 flashcam-1.5.8/flashcam/direct.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4572 2023-04-17 20:01:01.000000 flashcam-1.5.8/flashcam/izmq_receiver.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4178 2023-04-17 20:01:01.000000 flashcam-1.5.8/flashcam/mmapwr.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    45656 2023-07-14 19:50:06.000000 flashcam-1.5.8/flashcam/real_camera.py
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    35953 2023-04-28 18:56:55.000000 flashcam-1.5.8/flashcam/stream_enhancer.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)   106457 2023-07-14 19:58:39.000000 flashcam-1.5.8/flashcam/uniwrec.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    11302 2023-04-17 20:01:01.000000 flashcam-1.5.8/flashcam/usbcheck.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    34595 2023-07-14 19:49:12.000000 flashcam-1.5.8/flashcam/v4lc.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2023-07-14 19:59:28.000000 flashcam-1.5.8/flashcam/version.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    30433 2023-07-13 20:52:49.000000 flashcam-1.5.8/flashcam/web.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-14 19:59:28.881467 flashcam-1.5.8/flashcam.egg-info/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      850 2023-07-14 19:59:28.000000 flashcam-1.5.8/flashcam.egg-info/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      820 2023-07-14 19:59:28.000000 flashcam-1.5.8/flashcam.egg-info/SOURCES.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2023-07-14 19:59:28.000000 flashcam-1.5.8/flashcam.egg-info/dependency_links.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      157 2023-07-14 19:59:28.000000 flashcam-1.5.8/flashcam.egg-info/requires.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        9 2023-07-14 19:59:28.000000 flashcam-1.5.8/flashcam.egg-info/top_level.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2023-07-14 19:59:28.885467 flashcam-1.5.8/setup.cfg
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2008 2023-04-17 20:44:28.000000 flashcam-1.5.8/setup.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-15 09:51:01.053461 flashcam-1.5.9/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      850 2023-07-15 09:51:01.053461 flashcam-1.5.9/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      569 2023-07-15 09:50:59.000000 flashcam-1.5.9/README.md
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-15 09:51:01.053461 flashcam-1.5.9/bin/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    24892 2023-07-14 19:16:43.000000 flashcam-1.5.9/bin/flashcam
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      150 2023-04-17 20:01:01.000000 flashcam-1.5.9/bin/flashcam_join
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      311 2023-04-17 20:01:01.000000 flashcam-1.5.9/bin/flashcam_rep
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      551 2023-04-17 20:01:01.000000 flashcam-1.5.9/bin/flashcamg
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-15 09:51:01.053461 flashcam-1.5.9/flashcam/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      249 2023-04-17 20:01:01.000000 flashcam-1.5.9/flashcam/__init__.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     5255 2023-04-17 20:01:01.000000 flashcam-1.5.9/flashcam/base_camera2.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     8106 2023-07-13 20:56:38.000000 flashcam-1.5.9/flashcam/config.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-15 09:51:01.053461 flashcam-1.5.9/flashcam/data/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    24159 2023-04-17 20:01:01.000000 flashcam-1.5.9/flashcam/data/BEAM_OFF.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    27944 2023-04-17 20:01:01.000000 flashcam-1.5.9/flashcam/data/BEAM_ON_.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    27715 2023-04-17 20:01:01.000000 flashcam-1.5.9/flashcam/data/DET_NRDY.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    27483 2023-04-17 20:01:01.000000 flashcam-1.5.9/flashcam/data/DET_RDY_.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    34404 2023-04-17 20:01:01.000000 flashcam-1.5.9/flashcam/data/digital-7.mono.ttf
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    19991 2023-04-17 20:01:01.000000 flashcam-1.5.9/flashcam/data/monoskop.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    59930 2023-04-28 18:56:55.000000 flashcam-1.5.9/flashcam/data/win_rain.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    91079 2023-04-28 18:56:55.000000 flashcam-1.5.9/flashcam/data/win_skull.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    76270 2023-04-28 18:56:55.000000 flashcam-1.5.9/flashcam/data/win_storm.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    61604 2023-04-28 18:56:55.000000 flashcam-1.5.9/flashcam/data/win_winter.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    72731 2023-04-17 20:01:01.000000 flashcam-1.5.9/flashcam/data/windows.jpg
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4173 2023-04-17 20:01:01.000000 flashcam-1.5.9/flashcam/direct.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4572 2023-04-17 20:01:01.000000 flashcam-1.5.9/flashcam/izmq_receiver.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4178 2023-04-17 20:01:01.000000 flashcam-1.5.9/flashcam/mmapwr.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    46322 2023-07-15 09:50:25.000000 flashcam-1.5.9/flashcam/real_camera.py
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    37745 2023-07-15 09:45:13.000000 flashcam-1.5.9/flashcam/stream_enhancer.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)   106457 2023-07-14 19:58:39.000000 flashcam-1.5.9/flashcam/uniwrec.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    11302 2023-04-17 20:01:01.000000 flashcam-1.5.9/flashcam/usbcheck.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    34595 2023-07-14 19:49:12.000000 flashcam-1.5.9/flashcam/v4lc.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2023-07-15 09:51:00.000000 flashcam-1.5.9/flashcam/version.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    30433 2023-07-13 20:52:49.000000 flashcam-1.5.9/flashcam/web.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-15 09:51:01.053461 flashcam-1.5.9/flashcam.egg-info/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      850 2023-07-15 09:51:01.000000 flashcam-1.5.9/flashcam.egg-info/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      820 2023-07-15 09:51:01.000000 flashcam-1.5.9/flashcam.egg-info/SOURCES.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2023-07-15 09:51:01.000000 flashcam-1.5.9/flashcam.egg-info/dependency_links.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      157 2023-07-15 09:51:01.000000 flashcam-1.5.9/flashcam.egg-info/requires.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        9 2023-07-15 09:51:01.000000 flashcam-1.5.9/flashcam.egg-info/top_level.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2023-07-15 09:51:01.053461 flashcam-1.5.9/setup.cfg
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2008 2023-04-17 20:44:28.000000 flashcam-1.5.9/setup.py
```

### Comparing `flashcam-1.5.8/PKG-INFO` & `flashcam-1.5.9/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flashcam
-Version: 1.5.8
+Version: 1.5.9
 Summary: Composition of scripts to control a web camera
 Home-page: https://gitlab.com/jaromrax/flashcam
 Author: jaromrax
 Author-email: jaromrax@gmail.com
 License: GPL2
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `flashcam-1.5.8/README.md` & `flashcam-1.5.9/README.md`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.8/bin/flashcam` & `flashcam-1.5.9/bin/flashcam`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.8/bin/flashcamg` & `flashcam-1.5.9/bin/flashcamg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.8/flashcam/base_camera2.py` & `flashcam-1.5.9/flashcam/base_camera2.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.8/flashcam/config.py` & `flashcam-1.5.9/flashcam/config.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.8/flashcam/data/BEAM_OFF.jpg` & `flashcam-1.5.9/flashcam/data/BEAM_OFF.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.8/flashcam/data/BEAM_ON_.jpg` & `flashcam-1.5.9/flashcam/data/BEAM_ON_.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.8/flashcam/data/DET_NRDY.jpg` & `flashcam-1.5.9/flashcam/data/DET_NRDY.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.8/flashcam/data/DET_RDY_.jpg` & `flashcam-1.5.9/flashcam/data/DET_RDY_.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.8/flashcam/data/digital-7.mono.ttf` & `flashcam-1.5.9/flashcam/data/digital-7.mono.ttf`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.8/flashcam/data/monoskop.jpg` & `flashcam-1.5.9/flashcam/data/monoskop.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.8/flashcam/data/win_rain.jpg` & `flashcam-1.5.9/flashcam/data/win_rain.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.8/flashcam/data/win_skull.jpg` & `flashcam-1.5.9/flashcam/data/win_skull.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.8/flashcam/data/win_storm.jpg` & `flashcam-1.5.9/flashcam/data/win_storm.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.8/flashcam/data/win_winter.jpg` & `flashcam-1.5.9/flashcam/data/win_winter.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.8/flashcam/data/windows.jpg` & `flashcam-1.5.9/flashcam/data/windows.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.8/flashcam/direct.py` & `flashcam-1.5.9/flashcam/direct.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.8/flashcam/izmq_receiver.py` & `flashcam-1.5.9/flashcam/izmq_receiver.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.8/flashcam/mmapwr.py` & `flashcam-1.5.9/flashcam/mmapwr.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.8/flashcam/real_camera.py` & `flashcam-1.5.9/flashcam/real_camera.py`

 * *Files 1% similar despite different names*

```diff
@@ -513,17 +513,18 @@
                                     #senh.zoom( zoom ,0,0 )
                                     senh.zoom( zoom ,cross_dx, cross_dy )
                         except Exception as e:
                             print("!... Problem ar cross.txt file:",e)
 
                     # ----------  I need to calculate histogram before labels...
                     if histogram: # just calculate a number on plain frame
-                        hmean = senh.histo_mean( ) # hmean STRING NOW
+                        #hmean = senh.histo_mean( ) # hmean STRING NOW
+                        hmean = senh.histo_medi( ) # hmean STRING NOW
                         # notwrk #self.histomean = hmean # when called from direct...
-                        ##print("i... histo value:", hmean)
+                        # print("i... histo value:", hmean)
                         ##tune_histo(cc, hmean )
 
                     # ---------- before anything - we decode the web command EXECUTE EXECUTION
 
                     # - compensate for speed of the sky
                     if ((speedx!=0) or (speedy!=0)) \
                     and ((abs(speedx)>1) or (abs(speedy)>1)):
@@ -789,15 +790,24 @@
                         #         exposure = newexposure # SENH
                         #         expovalue = -999
 
                         #     if  'exposure' in locals() and exposure != exposuredef:
                         #         senh.setbox(f"expo {(exposure-mine)/(maxe-mine):.4f}",  senh.expo)
 
                         if "exposure_time_absolute" in capa or "exposure_absolute" in capa:
-
+                            if histogram:
+                                if hmean<25:
+                                    cc.autoexpo_off( "autoexpo")
+                                    cc.expo( 1 ,'expo')     # 0-1 log
+
+                                    print("****** -H param => autoex  ************************ OFF")
+                                if hmean>200:
+                                    cc.autoexpo_on( "autoexpo")
+                                    #exposure = -0.1 + exposure
+                                    print("****** -H param => autoex  ********************** ON")
 
                             if expo_divide:
                                 expo_divide = False
                                 v4lc.mk_table(cc)
                                 exposuredef = False
 
                                 cc.autoexpo_off( "autoexpo")
```

### Comparing `flashcam-1.5.8/flashcam/stream_enhancer.py` & `flashcam-1.5.9/flashcam/stream_enhancer.py`

 * *Files 6% similar despite different names*

```diff
@@ -682,14 +682,71 @@
             else:
                 print("i... None frame2")
                 self.delta_frame = self.frame
 
 
 
 # ------------------------------------------------------- HISTO ---------------------------
+    def histo_medi(self):
+        def find_med( arr ):
+            # not transposed!
+            bina = 0
+            suma = 0
+            for i in arr:
+                #print(i)
+                bina+=1
+                suma+=i
+                #print(suma)
+                if suma>0.5:
+                    return bina
+            return len(arr)
+
+        BINS = 256 # 128
+        #bins = np.arange(BINS)
+        bins = np.arange(BINS).reshape(1,BINS)
+        framegray = cv2.cvtColor(self.frame, cv2.COLOR_BGR2GRAY)
+        # images; channels; mask none; histSize [BINS]
+        hist_gray = cv2.calcHist([framegray], [0], None, [BINS], [0, 256])
+
+        #hist_gray = np.transpose( hist_gray) # array
+        sumhist = hist_gray.sum()
+        hist_gray = hist_gray/sumhist
+        sumhist = hist_gray.sum()
+
+        #print(hist_gray)
+        #print(sumhist)
+        med = np.median( hist_gray )
+        med2= find_med( hist_gray)
+        #print( f" sum = {sumhist:6.1f}    med={med:.5f}  bin={med2}" )
+        return med2
+
+        # cv2.normalize(hist_gray,hist_gray,0,255,cv2.NORM_MINMAX)
+        #med =
+        black = (hist_gray[0] + hist_gray[1] )/2 #1st two bins
+        white = (hist_gray[-1]+hist_gray[-2] )/2 #last 2 bins
+
+        mean = np.dot( bins, hist_gray )
+        #print("MEAN",mean)
+        mean = round(100*mean[0][0]/sumhist/BINS) # min is bin 1, max is bin BINS.
+
+        # print(f"   {len(hist_gray)}  {hist_gray[0]}..{hist_gray[-1]}  sum={sumhist}  med={med},  mean={mean}  ")
+
+        #print("MEAN",mean)
+        #print( "LEN TYPE", len(mean),type(mean) )
+        BW = ""
+        if white>100: BW=BW+"W"
+        elif white>0: BW=BW+"w"
+
+        if black>100: BW=BW+"B"
+        elif black>0: BW=BW+"b"
+
+        #return mean
+        return f"*{mean:.0f}{BW}"  #/255*100
+
+
     def histo_mean(self):
 
         BINS = 128
         #bins = np.arange(BINS)
         bins = np.arange(BINS).reshape(1,BINS)
 
         framegray = cv2.cvtColor(self.frame, cv2.COLOR_BGR2GRAY)
```

### Comparing `flashcam-1.5.8/flashcam/uniwrec.py` & `flashcam-1.5.9/flashcam/uniwrec.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.8/flashcam/usbcheck.py` & `flashcam-1.5.9/flashcam/usbcheck.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.8/flashcam/v4lc.py` & `flashcam-1.5.9/flashcam/v4lc.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.8/flashcam/web.py` & `flashcam-1.5.9/flashcam/web.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.8/flashcam.egg-info/PKG-INFO` & `flashcam-1.5.9/flashcam.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flashcam
-Version: 1.5.8
+Version: 1.5.9
 Summary: Composition of scripts to control a web camera
 Home-page: https://gitlab.com/jaromrax/flashcam
 Author: jaromrax
 Author-email: jaromrax@gmail.com
 License: GPL2
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `flashcam-1.5.8/flashcam.egg-info/SOURCES.txt` & `flashcam-1.5.9/flashcam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.8/setup.py` & `flashcam-1.5.9/setup.py`

 * *Files identical despite different names*

