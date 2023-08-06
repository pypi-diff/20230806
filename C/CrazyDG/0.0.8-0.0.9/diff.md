# Comparing `tmp/CrazyDG-0.0.8.tar.gz` & `tmp/CrazyDG-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CrazyDG-0.0.8.tar", last modified: Thu Aug  3 14:24:42 2023, max compression
+gzip compressed data, was "CrazyDG-0.0.9.tar", last modified: Sun Aug  6 06:48:35 2023, max compression
```

## Comparing `CrazyDG-0.0.8.tar` & `CrazyDG-0.0.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 14:24:42.335681 CrazyDG-0.0.8/
-drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 14:24:42.325900 CrazyDG-0.0.8/CrazyDG/
--rw-r--r--   0 daegeun    (501) staff       (20)      215 2023-08-03 14:24:27.000000 CrazyDG-0.0.8/CrazyDG/__init__.py
-drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 14:24:42.329045 CrazyDG-0.0.8/CrazyDG/control/
--rw-r--r--   0 daegeun    (501) staff       (20)     2159 2023-08-03 10:11:52.000000 CrazyDG-0.0.8/CrazyDG/control/__init__.py
--rw-r--r--   0 daegeun    (501) staff       (20)       69 2023-08-03 01:51:19.000000 CrazyDG-0.0.8/CrazyDG/control/constants.py
--rw-r--r--   0 daegeun    (501) staff       (20)      459 2023-08-03 01:51:19.000000 CrazyDG-0.0.8/CrazyDG/control/integral_loop.py
--rw-r--r--   0 daegeun    (501) staff       (20)     1548 2023-08-03 01:51:19.000000 CrazyDG-0.0.8/CrazyDG/control/optimus_prime.py
-drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 14:24:42.329720 CrazyDG-0.0.8/CrazyDG/crazy/
--rw-r--r--   0 daegeun    (501) staff       (20)       30 2023-08-03 01:51:19.000000 CrazyDG-0.0.8/CrazyDG/crazy/__init__.py
--rw-r--r--   0 daegeun    (501) staff       (20)      428 2023-08-03 01:51:19.000000 CrazyDG-0.0.8/CrazyDG/crazy/crazy.py
-drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 14:24:42.330015 CrazyDG-0.0.8/CrazyDG/guidance/
--rw-r--r--   0 daegeun    (501) staff       (20)      185 2023-08-03 02:04:21.000000 CrazyDG-0.0.8/CrazyDG/guidance/__init__.py
-drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 14:24:42.332590 CrazyDG-0.0.8/CrazyDG/guidance/utils/
--rw-r--r--   0 daegeun    (501) staff       (20)      165 2023-08-03 10:28:33.000000 CrazyDG-0.0.8/CrazyDG/guidance/utils/__init__.py
--rw-r--r--   0 daegeun    (501) staff       (20)      953 2023-08-03 14:12:26.000000 CrazyDG-0.0.8/CrazyDG/guidance/utils/_goto.py
--rw-r--r--   0 daegeun    (501) staff       (20)      807 2023-08-03 10:28:10.000000 CrazyDG-0.0.8/CrazyDG/guidance/utils/_hover.py
--rw-r--r--   0 daegeun    (501) staff       (20)     1172 2023-08-03 11:08:07.000000 CrazyDG-0.0.8/CrazyDG/guidance/utils/_landing.py
--rw-r--r--   0 daegeun    (501) staff       (20)      874 2023-08-03 14:24:11.000000 CrazyDG-0.0.8/CrazyDG/guidance/utils/_landing_supporter.py
--rw-r--r--   0 daegeun    (501) staff       (20)      967 2023-08-03 10:28:22.000000 CrazyDG-0.0.8/CrazyDG/guidance/utils/_takeoff.py
--rw-r--r--   0 daegeun    (501) staff       (20)      157 2023-08-03 14:18:14.000000 CrazyDG-0.0.8/CrazyDG/guidance/utils/constants.py
--rw-r--r--   0 daegeun    (501) staff       (20)      349 2023-08-03 01:51:19.000000 CrazyDG-0.0.8/CrazyDG/guidance/utils/smoother.py
--rw-r--r--   0 daegeun    (501) staff       (20)     1018 2023-08-03 10:19:59.000000 CrazyDG-0.0.8/CrazyDG/main_example.py
-drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 14:24:42.334051 CrazyDG-0.0.8/CrazyDG/navigation/
--rw-r--r--   0 daegeun    (501) staff       (20)      968 2023-08-03 10:28:03.000000 CrazyDG-0.0.8/CrazyDG/navigation/__init__.py
--rw-r--r--   0 daegeun    (501) staff       (20)     1660 2023-08-03 10:27:51.000000 CrazyDG-0.0.8/CrazyDG/navigation/imu.py
--rw-r--r--   0 daegeun    (501) staff       (20)     2098 2023-08-03 10:27:54.000000 CrazyDG-0.0.8/CrazyDG/navigation/imu_setup.py
--rw-r--r--   0 daegeun    (501) staff       (20)     2394 2023-08-03 01:51:19.000000 CrazyDG-0.0.8/CrazyDG/navigation/qualisys.py
-drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 14:24:42.334960 CrazyDG-0.0.8/CrazyDG/recorder/
--rw-r--r--   0 daegeun    (501) staff       (20)       63 2023-08-03 02:12:37.000000 CrazyDG-0.0.8/CrazyDG/recorder/__init__.py
--rw-r--r--   0 daegeun    (501) staff       (20)     3209 2023-08-03 10:30:11.000000 CrazyDG-0.0.8/CrazyDG/recorder/recorder.py
--rw-r--r--   0 daegeun    (501) staff       (20)     2451 2023-08-03 02:12:37.000000 CrazyDG-0.0.8/CrazyDG/recorder/visualizer.py
-drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 14:24:42.327614 CrazyDG-0.0.8/CrazyDG.egg-info/
--rw-r--r--   0 daegeun    (501) staff       (20)      462 2023-08-03 14:24:42.000000 CrazyDG-0.0.8/CrazyDG.egg-info/PKG-INFO
--rw-r--r--   0 daegeun    (501) staff       (20)      912 2023-08-03 14:24:42.000000 CrazyDG-0.0.8/CrazyDG.egg-info/SOURCES.txt
--rw-r--r--   0 daegeun    (501) staff       (20)        1 2023-08-03 14:24:42.000000 CrazyDG-0.0.8/CrazyDG.egg-info/dependency_links.txt
--rw-r--r--   0 daegeun    (501) staff       (20)        1 2023-08-03 14:24:42.000000 CrazyDG-0.0.8/CrazyDG.egg-info/not-zip-safe
--rw-r--r--   0 daegeun    (501) staff       (20)        8 2023-08-03 14:24:42.000000 CrazyDG-0.0.8/CrazyDG.egg-info/top_level.txt
--rw-r--r--   0 daegeun    (501) staff       (20)      462 2023-08-03 14:24:42.335352 CrazyDG-0.0.8/PKG-INFO
--rw-r--r--   0 daegeun    (501) staff       (20)       44 2023-08-03 01:51:19.000000 CrazyDG-0.0.8/README.md
--rw-r--r--   0 daegeun    (501) staff       (20)       38 2023-08-03 14:24:42.335760 CrazyDG-0.0.8/setup.cfg
--rw-r--r--   0 daegeun    (501) staff       (20)      678 2023-08-03 14:24:25.000000 CrazyDG-0.0.8/setup.py
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-06 06:48:35.068680 CrazyDG-0.0.9/
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-06 06:48:35.061826 CrazyDG-0.0.9/CrazyDG/
+-rw-r--r--   0 daegeun    (501) staff       (20)      215 2023-08-06 06:48:09.000000 CrazyDG-0.0.9/CrazyDG/__init__.py
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-06 06:48:35.064001 CrazyDG-0.0.9/CrazyDG/control/
+-rw-r--r--   0 daegeun    (501) staff       (20)     2351 2023-08-06 06:12:17.000000 CrazyDG-0.0.9/CrazyDG/control/__init__.py
+-rw-r--r--   0 daegeun    (501) staff       (20)       69 2023-08-06 06:12:30.000000 CrazyDG-0.0.9/CrazyDG/control/constants.py
+-rw-r--r--   0 daegeun    (501) staff       (20)      459 2023-08-03 01:51:19.000000 CrazyDG-0.0.9/CrazyDG/control/integral_loop.py
+-rw-r--r--   0 daegeun    (501) staff       (20)     1548 2023-08-03 01:51:19.000000 CrazyDG-0.0.9/CrazyDG/control/optimus_prime.py
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-06 06:48:35.064483 CrazyDG-0.0.9/CrazyDG/crazy/
+-rw-r--r--   0 daegeun    (501) staff       (20)       30 2023-08-03 01:51:19.000000 CrazyDG-0.0.9/CrazyDG/crazy/__init__.py
+-rw-r--r--   0 daegeun    (501) staff       (20)      428 2023-08-03 01:51:19.000000 CrazyDG-0.0.9/CrazyDG/crazy/crazy.py
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-06 06:48:35.064709 CrazyDG-0.0.9/CrazyDG/guidance/
+-rw-r--r--   0 daegeun    (501) staff       (20)      185 2023-08-03 02:04:21.000000 CrazyDG-0.0.9/CrazyDG/guidance/__init__.py
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-06 06:48:35.066490 CrazyDG-0.0.9/CrazyDG/guidance/utils/
+-rw-r--r--   0 daegeun    (501) staff       (20)      165 2023-08-03 10:28:33.000000 CrazyDG-0.0.9/CrazyDG/guidance/utils/__init__.py
+-rw-r--r--   0 daegeun    (501) staff       (20)      801 2023-08-06 06:14:56.000000 CrazyDG-0.0.9/CrazyDG/guidance/utils/_goto.py
+-rw-r--r--   0 daegeun    (501) staff       (20)      769 2023-08-06 06:15:06.000000 CrazyDG-0.0.9/CrazyDG/guidance/utils/_hover.py
+-rw-r--r--   0 daegeun    (501) staff       (20)     1172 2023-08-03 11:08:07.000000 CrazyDG-0.0.9/CrazyDG/guidance/utils/_landing.py
+-rw-r--r--   0 daegeun    (501) staff       (20)     1148 2023-08-06 06:20:00.000000 CrazyDG-0.0.9/CrazyDG/guidance/utils/_landing_supporter.py
+-rw-r--r--   0 daegeun    (501) staff       (20)      824 2023-08-06 06:20:32.000000 CrazyDG-0.0.9/CrazyDG/guidance/utils/_takeoff.py
+-rw-r--r--   0 daegeun    (501) staff       (20)      157 2023-08-06 06:20:55.000000 CrazyDG-0.0.9/CrazyDG/guidance/utils/constants.py
+-rw-r--r--   0 daegeun    (501) staff       (20)      349 2023-08-03 01:51:19.000000 CrazyDG-0.0.9/CrazyDG/guidance/utils/smoother.py
+-rw-r--r--   0 daegeun    (501) staff       (20)     1227 2023-08-06 06:47:27.000000 CrazyDG-0.0.9/CrazyDG/main_example.py
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-06 06:48:35.067360 CrazyDG-0.0.9/CrazyDG/navigation/
+-rw-r--r--   0 daegeun    (501) staff       (20)      968 2023-08-03 10:28:03.000000 CrazyDG-0.0.9/CrazyDG/navigation/__init__.py
+-rw-r--r--   0 daegeun    (501) staff       (20)     1660 2023-08-03 10:27:51.000000 CrazyDG-0.0.9/CrazyDG/navigation/imu.py
+-rw-r--r--   0 daegeun    (501) staff       (20)     2098 2023-08-03 10:27:54.000000 CrazyDG-0.0.9/CrazyDG/navigation/imu_setup.py
+-rw-r--r--   0 daegeun    (501) staff       (20)     2394 2023-08-03 01:51:19.000000 CrazyDG-0.0.9/CrazyDG/navigation/qualisys.py
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-06 06:48:35.068107 CrazyDG-0.0.9/CrazyDG/recorder/
+-rw-r--r--   0 daegeun    (501) staff       (20)       63 2023-08-03 02:12:37.000000 CrazyDG-0.0.9/CrazyDG/recorder/__init__.py
+-rw-r--r--   0 daegeun    (501) staff       (20)     3703 2023-08-06 06:28:24.000000 CrazyDG-0.0.9/CrazyDG/recorder/recorder.py
+-rw-r--r--   0 daegeun    (501) staff       (20)     3987 2023-08-06 06:44:25.000000 CrazyDG-0.0.9/CrazyDG/recorder/visualizer.py
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-06 06:48:35.063023 CrazyDG-0.0.9/CrazyDG.egg-info/
+-rw-r--r--   0 daegeun    (501) staff       (20)      507 2023-08-06 06:48:34.000000 CrazyDG-0.0.9/CrazyDG.egg-info/PKG-INFO
+-rw-r--r--   0 daegeun    (501) staff       (20)      912 2023-08-06 06:48:35.000000 CrazyDG-0.0.9/CrazyDG.egg-info/SOURCES.txt
+-rw-r--r--   0 daegeun    (501) staff       (20)        1 2023-08-06 06:48:34.000000 CrazyDG-0.0.9/CrazyDG.egg-info/dependency_links.txt
+-rw-r--r--   0 daegeun    (501) staff       (20)        1 2023-08-06 06:48:34.000000 CrazyDG-0.0.9/CrazyDG.egg-info/not-zip-safe
+-rw-r--r--   0 daegeun    (501) staff       (20)        8 2023-08-06 06:48:34.000000 CrazyDG-0.0.9/CrazyDG.egg-info/top_level.txt
+-rw-r--r--   0 daegeun    (501) staff       (20)      507 2023-08-06 06:48:35.068452 CrazyDG-0.0.9/PKG-INFO
+-rw-r--r--   0 daegeun    (501) staff       (20)       44 2023-08-03 01:51:19.000000 CrazyDG-0.0.9/README.md
+-rw-r--r--   0 daegeun    (501) staff       (20)       38 2023-08-06 06:48:35.068756 CrazyDG-0.0.9/setup.cfg
+-rw-r--r--   0 daegeun    (501) staff       (20)      678 2023-08-06 06:48:14.000000 CrazyDG-0.0.9/setup.py
```

### Comparing `CrazyDG-0.0.8/CrazyDG/control/__init__.py` & `CrazyDG-0.0.9/CrazyDG/control/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -46,14 +46,19 @@
     def stop_send_setpoint( self ):
         ## commander
         commander = self.cf.commander
         ## stop command
         self.cf.command[:] = zeros(3)
         ## stop signal
         self.ready_for_command = False
+
+        for _ in range( 50 ):
+            commander.send_setpoint( 0, 0, 0, 10001 )
+            sleep( 0.2 )
+
         commander.send_stop_setpoint()
 
 
     def run( self ):
 
         cf        = self.cf
         commander = cf.commander
@@ -67,14 +72,16 @@
         acc_cmd = self.acc_cmd
         command = self.command
         thrust  = self.thrust
 
         while not self.ready_for_command:
             sleep( 0.1 )
 
+        print( 'controller starts working' )
+
         while self.ready_for_command:
 
             acc_cmd[:] = cf.command
 
             _command_is_not_in_there( acc_cmd, att_cur )
 
             _command_as_RPY( acc_cmd, command )
@@ -92,8 +99,10 @@
                 commander.send_setpoint(
                     command[0],
                     command[1],
                     command[2],
                     thrust[0]
                 )
 
-                sleep( dt )
+                sleep( dt )
+
+        print( 'controller end' )
```

### Comparing `CrazyDG-0.0.8/CrazyDG/control/optimus_prime.py` & `CrazyDG-0.0.9/CrazyDG/control/optimus_prime.py`

 * *Files identical despite different names*

### Comparing `CrazyDG-0.0.8/CrazyDG/guidance/utils/_goto.py` & `CrazyDG-0.0.9/CrazyDG/guidance/utils/_hover.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,51 +1,44 @@
 from ...crazy import CrazyDragon
 
-from .smoother import smooth_command
-
 from .constants import Kp, Kd, g
 
 from numpy import array, zeros
 
 from time import sleep
 
 
 
-def goto( cf: CrazyDragon, destination, T, dt=0.1 ):
+def hover( cf: CrazyDragon, T, dt=0.1 ):
 
     cur     = zeros(3)
     des     = zeros(3)
-    des_cmd = zeros(3)
     acc_cmd = zeros(3)
     P_pos   = zeros(3)
     D_pos   = zeros(3)
     care_g  = array([0,0,g])
 
-    print( 'goto =>', destination )
+    print( 'hover' )
 
     n = int( T / dt )
     t = 0
 
     command = cf.command
 
     cur[:] = cf.pos
     pos    = cf.pos
     vel    = cf.vel
 
-    des[:] = destination
+    des[:] = cur[:]
 
     cf.destination[:] = des
 
     for _ in range( n ):
 
-        des_cmd[:] = smooth_command( 
-            des, cur, t, int( T / 2 )
-        )
-
-        P_pos[:] = des_cmd - pos
+        P_pos[:] = des - pos
         D_pos[:] = vel
 
         acc_cmd[:] = 0
         acc_cmd[:] += P_pos * Kp
         acc_cmd[:] -= D_pos * Kd
         acc_cmd[:] += care_g
```

### Comparing `CrazyDG-0.0.8/CrazyDG/guidance/utils/_hover.py` & `CrazyDG-0.0.9/CrazyDG/guidance/utils/_landing.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,64 @@
 from ...crazy import CrazyDragon
 
 from .smoother import smooth_command
 
 from .constants import Kp, Kd, g
 
-from numpy import array, zeros
+from numpy        import array, zeros
+from numpy.linalg import norm
 
 from time import sleep
 
 
 
-def hover( cf: CrazyDragon, T, dt=0.1 ):
+def landing( cf: CrazyDragon, option=1, h=0.2, T=5, dt=0.1, step=0.075 ):
 
     cur     = zeros(3)
     des     = zeros(3)
+    des_cmd = zeros(3)
     acc_cmd = zeros(3)
     P_pos   = zeros(3)
     D_pos   = zeros(3)
     care_g  = array([0,0,g])
 
-    print( 'hover' )
+    print( 'landing' )
 
     n = int( T / dt )
     t = 0
 
     command = cf.command
 
     cur[:] = cf.pos
     pos    = cf.pos
     vel    = cf.vel
 
-    des[:] = cur[:]
+    if option:
+        des[0] = cur[0]
+        des[1] = cur[1]
+        des[2] = h
+    else:
+        des[0] = 0
+        des[1] = 0
+        des[2] = h
 
     cf.destination[:] = des
 
     for _ in range( n ):
 
-        P_pos[:] = des - pos
+        des_cmd[:] = smooth_command( 
+            des, cur, t, 5.0
+        )
+
+        P_pos[:] = des_cmd - pos
         D_pos[:] = vel
 
+        if ( norm( pos - des ) ) < 0.2:
+            break
+
         acc_cmd[:] = 0
         acc_cmd[:] += P_pos * Kp
         acc_cmd[:] -= D_pos * Kd
         acc_cmd[:] += care_g
 
         command[:] = acc_cmd
```

### Comparing `CrazyDG-0.0.8/CrazyDG/guidance/utils/_landing.py` & `CrazyDG-0.0.9/CrazyDG/guidance/utils/_landing_supporter.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,67 +1,66 @@
 from ...crazy import CrazyDragon
 
-from .smoother import smooth_command
+from ...recorder import Recorder
 
-from .constants import Kp, Kd, g
+# from .constants import Kp, Kd, g
 
 from numpy        import array, zeros
 from numpy.linalg import norm
 
 from time import sleep
 
 
 
-def landing( cf: CrazyDragon, option=1, h=0.2, T=5, dt=0.1, step=0.075 ):
+w = array([0.700,0.700,0.700])
+j = array([1.600,1.600,0.700])
+
+Kp = w * w
+Kd = 2 * j * w
+
+
+def landing_supporter( cf: CrazyDragon, recorder:Recorder, option=1, dt=0.1, step=0.03 ):
 
-    cur     = zeros(3)
     des     = zeros(3)
-    des_cmd = zeros(3)
     acc_cmd = zeros(3)
     P_pos   = zeros(3)
     D_pos   = zeros(3)
-    care_g  = array([0,0,g])
+    care_g  = array([0,0,9.81])
 
-    print( 'landing' )
+    print( 'landing supporter', recorder.record_length )
 
-    n = int( T / dt )
-    t = 0
+    pos = cf.pos
+    vel = cf.vel
 
-    command = cf.command
+    des[:] = pos
 
-    cur[:] = cf.pos
-    pos    = cf.pos
-    vel    = cf.vel
+    for _ in range( 30 ):
 
-    if option:
-        des[0] = cur[0]
-        des[1] = cur[1]
-        des[2] = h
-    else:
-        des[0] = 0
-        des[1] = 0
-        des[2] = h
+        if ( des[2] > 0 ):
+            des[:] -= step
+        else:
+            des[:] = 0
 
-    cf.destination[:] = des
-
-    for _ in range( n ):
-
-        des_cmd[:] = smooth_command( 
-            des, cur, t, 5.0
-        )
+        if ( norm( pos ) < 0.02 ):
+            break
 
-        P_pos[:] = des_cmd - pos
+        P_pos[:] = des - pos
         D_pos[:] = vel
 
-        if ( norm( pos - des ) ) < 0.2:
-            break
-
         acc_cmd[:] = 0
         acc_cmd[:] += P_pos * Kp
         acc_cmd[:] -= D_pos * Kd
         acc_cmd[:] += care_g
 
-        command[:] = acc_cmd
+        cf.command[:] = acc_cmd
+
+        sleep( dt )
+
+    acc_cmd[:] = care_g
+
+    for _ in range( 10 ):
+
+        acc_cmd[2] -= step
 
-        t += dt
+        cf.command[:] = acc_cmd
 
-        sleep( dt )
+    print( 'land' )
```

### Comparing `CrazyDG-0.0.8/CrazyDG/guidance/utils/_landing_supporter.py` & `CrazyDG-0.0.9/CrazyDG/guidance/utils/_goto.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,48 +1,49 @@
 from ...crazy import CrazyDragon
 
-from ...recorder import Recorder
-
 from .constants import Kp, Kd, g
 
-from numpy        import array, zeros
-from numpy.linalg import norm
+from numpy import array, zeros
 
 from time import sleep
 
 
 
-def landing_supporter( cf: CrazyDragon, recorder:Recorder, option=1, dt=0.1, step=0.03 ):
+def goto( cf: CrazyDragon, destination, T, dt=0.1 ):
 
+    cur     = zeros(3)
     des     = zeros(3)
     acc_cmd = zeros(3)
     P_pos   = zeros(3)
     D_pos   = zeros(3)
-    care_g  = array([0,0,9.81])
+    care_g  = array([0,0,g])
+
+    print( 'goto =>', destination )
 
-    print( 'landing supporter', recorder.record_length )
+    n = int( T / dt )
+    t = 0
 
-    pos = cf.pos
-    vel = cf.vel
+    command = cf.command
 
-    des[:] = 0
+    cur[:] = cf.pos
+    pos    = cf.pos
+    vel    = cf.vel
 
-    for _ in range( 30 ):
+    des[:] = destination
 
-        if ( norm( pos ) < 0.05 ):
-            break
+    cf.destination[:] = des
+
+    for _ in range( n ):
 
         P_pos[:] = des - pos
         D_pos[:] = vel
 
         acc_cmd[:] = 0
         acc_cmd[:] += P_pos * Kp
         acc_cmd[:] -= D_pos * Kd
         acc_cmd[:] += care_g
 
-        cf.command[:] = acc_cmd
-
-        print( acc_cmd )
+        command[:] = acc_cmd
 
-        sleep( dt )
+        t += dt
 
-    print( 'land' )
+        sleep( dt )
```

### Comparing `CrazyDG-0.0.8/CrazyDG/guidance/utils/_takeoff.py` & `CrazyDG-0.0.9/CrazyDG/guidance/utils/_takeoff.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 from ...crazy import CrazyDragon
 
-from .smoother import smooth_command
-
 from .constants import Kp, Kd, g
 
 from numpy import array, zeros
 
 from time import sleep
 
 
 
 def takeoff( cf: CrazyDragon, h=1.5, T=3, dt=0.1 ):
 
     cur     = zeros(3)
     des     = zeros(3)
-    des_cmd = zeros(3)
     acc_cmd = zeros(3)
     P_pos   = zeros(3)
     D_pos   = zeros(3)
     care_g  = array([0,0,g])
 
     print( 'take-off' )
 
@@ -35,19 +32,15 @@
     des[ 1 ] = cur[1]
     des[ 2 ] = h
 
     cf.destination[:] = des
 
     for _ in range( n ):
 
-        des_cmd[:] = smooth_command( 
-            des, cur, t, 1.5
-        )
-
-        P_pos[:] = des_cmd - pos
+        P_pos[:] = des - pos
         D_pos[:] = vel
 
         acc_cmd[:] = 0
         acc_cmd[:] += P_pos * Kp
         acc_cmd[:] -= D_pos * Kd
         acc_cmd[:] += care_g
```

### Comparing `CrazyDG-0.0.8/CrazyDG/main_example.py` & `CrazyDG-0.0.9/CrazyDG/main_example.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-from navigation import Navigation
-
-from control import Controller
-
-from recorder import Recorder
-
-from crazy import CrazyDragon
+from CrazyDG import CrazyDragon
+from CrazyDG import Navigation
+from CrazyDG import Controller
+from CrazyDG import Recorder
+from CrazyDG import utils
 
 from cflib                         import crtp
 from cflib.crazyflie.syncCrazyflie import SyncCrazyflie
 from cflib.utils                   import uri_helper
 
 nav_config = {
     'body_name': 'cf1'
@@ -40,14 +38,24 @@
         CTR.start()
         RCD.start()
 
         ## your guidance function ##
         CTR.init_send_setpoint()
         ##       from here        ##
 
+        utils.takeoff( _cf )
+
+        utils.hover( _cf, T=2 )
+
+        utils.goto( _cf, [2.0,2.0,2.0], T=5 )
+
+        utils.hover( _cf, T=2 )
+
+        utils.landing_supporter( _cf, RCD )
+
         ############################
 
         CTR.stop_send_setpoint()
 
         NAV.join()
         CTR.join()
         RCD.join()
```

### Comparing `CrazyDG-0.0.8/CrazyDG/navigation/__init__.py` & `CrazyDG-0.0.9/CrazyDG/navigation/__init__.py`

 * *Files identical despite different names*

### Comparing `CrazyDG-0.0.8/CrazyDG/navigation/imu.py` & `CrazyDG-0.0.9/CrazyDG/navigation/imu.py`

 * *Files identical despite different names*

### Comparing `CrazyDG-0.0.8/CrazyDG/navigation/imu_setup.py` & `CrazyDG-0.0.9/CrazyDG/navigation/imu_setup.py`

 * *Files identical despite different names*

### Comparing `CrazyDG-0.0.8/CrazyDG/navigation/qualisys.py` & `CrazyDG-0.0.9/CrazyDG/navigation/qualisys.py`

 * *Files identical despite different names*

### Comparing `CrazyDG-0.0.8/CrazyDG/recorder/recorder.py` & `CrazyDG-0.0.9/CrazyDG/recorder/recorder.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 from ..crazy import CrazyDragon
 
 from threading import Thread
 
+from os import system
+
+from datetime import datetime
+
 from numpy import zeros, array
 
 from time  import sleep
 
 from ..control import alpha
 
 from .visualizer import *
@@ -96,36 +100,48 @@
     def guidance_end(self):
 
         self.guidance_end_idx = self.record_length
 
     
     def join(self):
 
+        self.recording = False
+
         super().join()
 
         _len = self.record_length
+        _stt = self.guidance_start_idx
+        _end = self.guidance_end_idx
 
         acc    = self.record_datastrg['acc']
         acccmd = self.record_datastrg['acccmd']
 
         vel    = self.record_datastrg['vel']
 
         pos    = self.record_datastrg['pos']
         posref = self.record_datastrg['posref']
 
         att    = self.record_datastrg['att']
         cmd    = self.record_datastrg['cmd']
         thrust = self.record_datastrg['thrust']
 
-        plot_acc_pos_cmd(acc, acccmd, vel, pos, posref, _len)
-        plot_thrust(thrust[0,:], cmd[3,:]*alpha, _len)
-        plot_att(att, cmd[:3,:], _len)
+        d = datetime.now()
+        date      = f'{d.year}-{d.month}-{d.day:02}-{d.hour:02}-{d.minute:02}-{d.second:02}'
+        self.date = date
+
+        system( f'cd ./flight_data && mkdir {date}' )
+
+        plot_acc_pos_cmd( acc, acccmd, vel, pos, posref, _len, _stt, _end, date )
+        plot_thrust( thrust[0,:], cmd[3,:]*alpha, _len, _stt, _end, date )
+        plot_att( att, cmd[:3,:], _len, _stt, _end, date )
+
+        plot_trj( pos, _len, _stt, _end, date )
 
 
-def array_type_data_callback(datastrg, data, i):
+def array_type_data_callback( datastrg, data, i ):
 
-    datastrg[:,i] = array(data)
+    datastrg[:,i] = array( data )
 
 
-def float_type_data_callback(datastrg, data, i):
+def float_type_data_callback( datastrg, data, i ):
 
     datastrg[0,i] = data
```

### Comparing `CrazyDG-0.0.8/CrazyDG.egg-info/SOURCES.txt` & `CrazyDG-0.0.9/CrazyDG.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CrazyDG-0.0.8/setup.py` & `CrazyDG-0.0.9/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 
 
 setup(
     name='CrazyDG',
-    version='0.0.8',
+    version='0.0.9',
     description='CrazyDG is for convenience',
     author='Daegeun02',
     author_email='redhawkdg02@gmail.com',
     url='https://github.com/Daegeun02/CrazyDG.git',
     install_requires=[],
     packages=find_packages( exclude=[] ),
     keywords=['CrazyDG', 'by daegeun', 'for convenience'],
```

