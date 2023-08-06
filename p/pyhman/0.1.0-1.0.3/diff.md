# Comparing `tmp/pyhman-0.1.0.tar.gz` & `tmp/pyhman-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhman-0.1.0.tar", last modified: Tue Jul  4 21:59:30 2023, max compression
+gzip compressed data, was "pyhman-1.0.3.tar", last modified: Sun Aug  6 16:54:29 2023, max compression
```

## Comparing `pyhman-0.1.0.tar` & `pyhman-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxrwxr-x   0 aightech  (1000) aightech  (1000)        0 2023-07-04 21:59:30.942882 pyhman-0.1.0/
--rw-rw-r--   0 aightech  (1000) aightech  (1000)    35149 2023-06-17 13:55:10.000000 pyhman-0.1.0/LICENSE
--rw-rw-r--   0 aightech  (1000) aightech  (1000)     2835 2023-07-04 21:59:30.942882 pyhman-0.1.0/PKG-INFO
--rw-rw-r--   0 aightech  (1000) aightech  (1000)     2551 2023-06-24 12:02:23.000000 pyhman-0.1.0/README.md
-drwxrwxr-x   0 aightech  (1000) aightech  (1000)        0 2023-07-04 21:59:30.938882 pyhman-0.1.0/pyhman/
--rw-rw-r--   0 aightech  (1000) aightech  (1000)       23 2023-07-04 21:49:05.000000 pyhman-0.1.0/pyhman/__init__.py
--rw-rw-r--   0 aightech  (1000) aightech  (1000)     7388 2023-07-04 21:51:02.000000 pyhman-0.1.0/pyhman/hman.py
--rw-rw-r--   0 aightech  (1000) aightech  (1000)     2817 2023-07-04 21:42:07.000000 pyhman-0.1.0/pyhman/hmanserver.py
-drwxrwxr-x   0 aightech  (1000) aightech  (1000)        0 2023-07-04 21:59:30.942882 pyhman-0.1.0/pyhman.egg-info/
--rw-rw-r--   0 aightech  (1000) aightech  (1000)     2835 2023-07-04 21:59:30.000000 pyhman-0.1.0/pyhman.egg-info/PKG-INFO
--rw-rw-r--   0 aightech  (1000) aightech  (1000)      230 2023-07-04 21:59:30.000000 pyhman-0.1.0/pyhman.egg-info/SOURCES.txt
--rw-rw-r--   0 aightech  (1000) aightech  (1000)        1 2023-07-04 21:59:30.000000 pyhman-0.1.0/pyhman.egg-info/dependency_links.txt
--rw-rw-r--   0 aightech  (1000) aightech  (1000)       20 2023-07-04 21:59:30.000000 pyhman-0.1.0/pyhman.egg-info/requires.txt
--rw-rw-r--   0 aightech  (1000) aightech  (1000)        7 2023-07-04 21:59:30.000000 pyhman-0.1.0/pyhman.egg-info/top_level.txt
--rw-rw-r--   0 aightech  (1000) aightech  (1000)       38 2023-07-04 21:59:30.942882 pyhman-0.1.0/setup.cfg
--rw-rw-r--   0 aightech  (1000) aightech  (1000)      561 2023-07-04 21:59:26.000000 pyhman-0.1.0/setup.py
+drwxrwxr-x   0 aightech  (1000) aightech  (1000)        0 2023-08-06 16:54:29.264194 pyhman-1.0.3/
+-rw-rw-r--   0 aightech  (1000) aightech  (1000)    35149 2023-06-17 13:27:16.000000 pyhman-1.0.3/LICENSE
+-rw-rw-r--   0 aightech  (1000) aightech  (1000)     2791 2023-08-06 16:54:29.264194 pyhman-1.0.3/PKG-INFO
+-rw-rw-r--   0 aightech  (1000) aightech  (1000)     2551 2023-06-17 13:55:43.000000 pyhman-1.0.3/README.md
+drwxrwxr-x   0 aightech  (1000) aightech  (1000)        0 2023-08-06 16:54:29.264194 pyhman-1.0.3/pyhman/
+-rw-rw-r--   0 aightech  (1000) aightech  (1000)       57 2023-08-06 16:48:19.000000 pyhman-1.0.3/pyhman/__init__.py
+-rw-rw-r--   0 aightech  (1000) aightech  (1000)     8415 2023-08-06 15:57:26.000000 pyhman-1.0.3/pyhman/hman.py
+-rw-rw-r--   0 aightech  (1000) aightech  (1000)     2799 2023-06-17 11:43:16.000000 pyhman-1.0.3/pyhman/hmanserver.py
+drwxrwxr-x   0 aightech  (1000) aightech  (1000)        0 2023-08-06 16:54:29.264194 pyhman-1.0.3/pyhman.egg-info/
+-rw-rw-r--   0 aightech  (1000) aightech  (1000)     2791 2023-08-06 16:54:29.000000 pyhman-1.0.3/pyhman.egg-info/PKG-INFO
+-rw-rw-r--   0 aightech  (1000) aightech  (1000)      201 2023-08-06 16:54:29.000000 pyhman-1.0.3/pyhman.egg-info/SOURCES.txt
+-rw-rw-r--   0 aightech  (1000) aightech  (1000)        1 2023-08-06 16:54:29.000000 pyhman-1.0.3/pyhman.egg-info/dependency_links.txt
+-rw-rw-r--   0 aightech  (1000) aightech  (1000)        7 2023-08-06 16:54:29.000000 pyhman-1.0.3/pyhman.egg-info/top_level.txt
+-rw-rw-r--   0 aightech  (1000) aightech  (1000)       38 2023-08-06 16:54:29.264194 pyhman-1.0.3/setup.cfg
+-rw-rw-r--   0 aightech  (1000) aightech  (1000)      472 2023-08-06 16:54:21.000000 pyhman-1.0.3/setup.py
```

### Comparing `pyhman-0.1.0/LICENSE` & `pyhman-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhman-0.1.0/PKG-INFO` & `pyhman-1.0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: pyhman
-Version: 0.1.0
-Summary: Python library for the Hman robot
-Home-page: https://github.com/Aightech/pyHman
-Author: Alexis Devillard
-License: GPL-3.0
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # pyHman
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 This is a Python library for controlling and communicating with the Hman device. This library provides high-level interfaces to set and get various parameters of hman, such as motor positions, modes, currents, and so on.
 
 ## Installation
 
@@ -77,9 +65,8 @@
 
 ## Support
 
 If you have any questions or run into any problems, please open an issue in the GitHub repository.
 7
 ## Disclaimer
 
-Use this software at your own risk. The authors are not responsible for any damage that may be caused directly or indirectly through the use of this software.
-
+Use this software at your own risk. The authors are not responsible for any damage that may be caused directly or indirectly through the use of this software.
```

### Comparing `pyhman-0.1.0/README.md` & `pyhman-1.0.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: pyhman
+Version: 1.0.3
+Summary: Python library to control the HMan robot
+Home-page: UNKNOWN
+Author: Alexis Devillard
+License: MIT
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # pyHman
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 This is a Python library for controlling and communicating with the Hman device. This library provides high-level interfaces to set and get various parameters of hman, such as motor positions, modes, currents, and so on.
 
 ## Installation
 
@@ -65,8 +76,9 @@
 
 ## Support
 
 If you have any questions or run into any problems, please open an issue in the GitHub repository.
 7
 ## Disclaimer
 
-Use this software at your own risk. The authors are not responsible for any damage that may be caused directly or indirectly through the use of this software.
+Use this software at your own risk. The authors are not responsible for any damage that may be caused directly or indirectly through the use of this software.
+
```

### Comparing `pyhman-0.1.0/pyhman/hman.py` & `pyhman-1.0.3/pyhman/hman.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         modes (dict): Dictionary of possible modes.
         positions (list): List of encoder positions.
         target_positions (list): List of target positions.
         target_currents (list): List of target currents.
         port (int): Port of the hman.
         address (str): IP address of the hman.
     """
-    def __init__(self, nb_mot=3, verbose=False):
+    def __init__(self, nb_mot, verbose):
         self.nb_mot = nb_mot
         self.verbose = verbose
         self._pkgSize = 2 + 3 * 8
         self.mode = None
         self._cmd = bytearray(self._pkgSize)
         self._client = None
         self.positions = [0, 0, 0]#encoder positions
@@ -61,15 +61,14 @@
         """
         self.address = address
         self.port = port
         logging.info('Connecting to %s:%d...', self.address, self.port)
         self._client = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         try:
             self._client.connect((address, self.port))
-            logging.info('Connected.')
         except socket.error as exc:
             logging.error(f'Caught exception socket.error : {exc}')
 
     def set_mode(self, mode):
         """Set the mode of the hman.
         Args:
             mode (str): Mode to set.
@@ -102,21 +101,38 @@
         if not data:
             logging.error('No data received.')
             return
         self.positions = [struct.unpack('<i', data[i*4 : (i+1)*4])[0] for i in range(self.nb_mot)]#encoder positions
         return self.positions
     
     def setPID(self, PID):
+        """Set the PID of the hman.
+        Args:
+            PID (list): List of PID values. [P, I, D] 
+        """
         self._cmd[0] = ord('K')
         self._cmd[1] = 0xff
         logging.debug('Setting values to %s', PID)
         for i in range(3):
             v = int(PID[i]*1000000)
             self._cmd[2 + i * 4 : 2 + (i + 1) * 4] = struct.pack('<i', v)
         self._client.sendall(self._cmd)
+
+    def set_max_speed(self, speed):
+        """Set the max speed of the hman. Above this speed, the hman will stop.
+        Args:
+            speed (list): List of max speed values. [M1, M2, M3], in turn/1024/5ms
+        """
+        self._cmd[0] = ord('S')
+        self._cmd[1] = 0xff
+        logging.debug('Setting values to %s', speed)
+        for i in range(3):
+            v = int(speed[i])
+            self._cmd[2 + i * 4 : 2 + (i + 1) * 4] = struct.pack('<i', v)
+        self._client.sendall(self._cmd)
         
 
     def set_cartesian_pos(self, posx, posy, posz):
         """Set the cartesian position of the hman.
         Args:
             posx (float): X position.
             posy (float): Y position.
@@ -132,16 +148,16 @@
         self.__set_values(pos, 3)
         #transform the cartesian articular position to cartesian position
         return [(self.positions[0] + self.positions[1]) / 2, (-self.positions[0] + self.positions[1]) / 2]
 
     def set_articular_pos(self, pos1, pos2, pos3):
         """Set the articular position of the hman.
         Args:
-            pos1 (float): Position of the first motor.
-            pos2 (float): Position of the second motor.
+            pos1 (float): Position of the first motor, in increment (A full revolution is 1024).
+            pos2 (float): Position of the second motor, in increment (A full revolution is 1024).
             pos3 (float): Position of the third motor.
         Returns:
             list: List of encoder positions.
         """ 
         if self.mode != 'position':
             self.set_mode('position')
 
@@ -149,16 +165,16 @@
         self.target_positions = pos
         self.__set_values(pos, 3)
         return self.positions
 
     def set_motors_current(self, cur1, cur2, cur3):
         """Set the current of the motors.
         Args:
-            cur1 (float): Current of the first motor.
-            cur2 (float): Current of the second motor.
+            cur1 (float): Current of the first motor, in pwm (410-3686)
+            cur2 (float): Current of the second motor, in pwm (410-3686)
             cur3 (float): Current of the third motor.
         Returns:
             list: List of encoder positions.
         """
         if self.mode != 'current':
             self.set_mode('current')
 
@@ -201,34 +217,39 @@
 if __name__ == '__main__':
     #create a hman object
     hman = Hman(2, True)
     #connect to the hman
     hman.connect('192.168.127.250')
     #set the motors in articular position
 
+    hman.setPID([0.007,0.000001,0])#set the PID at Kp=0.005, Ki=0.0000, Kd=0.005
+    hman.home()
 
-
-    hman.setPID([0.001,0.0000,0])#set the PID at Kp=0.005, Ki=0.0000, Kd=0.005
-
+    hman.set_max_speed([100,100,100])
+    hman.setPID([0.0035,0.0,0.00001])#set the PID at Kp=0.005, Ki=0.0000, Kd=0.005
     sp = [4000,4000,180]
     T = 5
-    nb_step=1
+    nb_step=100
     dt=T/nb_step
 
-    hman.home()
+    print('homed')
 
-    for i in range(1,nb_step,1):
+    for i in range(1,nb_step+1,1):
         pos = hman.set_cartesian_pos(int(sp[0]*i/nb_step),int(sp[1]*i/nb_step),int(sp[2]*i/nb_step))
         print(pos)
+        print([int(sp[0]*i/nb_step),int(sp[1]*i/nb_step),int(sp[2]*i/nb_step)])
         time.sleep(dt)
+    
+    time.sleep(1)
 
     for i in range(nb_step,-1,-1):
         pos = hman.set_cartesian_pos(int(sp[0]*i/nb_step),int(sp[1]*i/nb_step),int(sp[2]*i/nb_step))
         print(pos)
+        print([int(sp[0]*i/nb_step),int(sp[1]*i/nb_step),int(sp[2]*i/nb_step)])
         time.sleep(dt)
     
     #pos = hman.set_motors_current(1000,1000,1000)
     # print(pos)
 
-    time.sleep(3)
+    time.sleep(1)
 
     hman.disconnect()
```

### Comparing `pyhman-0.1.0/pyhman/hmanserver.py` & `pyhman-1.0.3/pyhman/hmanserver.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         self.target_currents = [0, 0, 0]#
         self.modes = 0
         self.data = bytearray(3*4)
         self.server = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         self.server.bind((self.host, self.port))
         self.server.listen(1)
         logging.basicConfig(level=logging.DEBUG if verbose else logging.INFO)
-        logging.info('Server started at {self.host}:{self.port}'.format(self=self))
+        logging.info('Server started at {self.host}:{self.port}')
 
     def start(self):
         while True:
             logging.info('Waiting for a connection on port {host}:{port}...'.format(host=self.host, port=self.port))
             client, addr = self.server.accept()
 
             logging.info('Connected by {addr}'.format(addr=addr))
```

### Comparing `pyhman-0.1.0/pyhman.egg-info/PKG-INFO` & `pyhman-1.0.3/pyhman.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: pyhman
-Version: 0.1.0
-Summary: Python library for the Hman robot
-Home-page: https://github.com/Aightech/pyHman
+Version: 1.0.3
+Summary: Python library to control the HMan robot
+Home-page: UNKNOWN
 Author: Alexis Devillard
-License: GPL-3.0
+License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE
 
 # pyHman
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 This is a Python library for controlling and communicating with the Hman device. This library provides high-level interfaces to set and get various parameters of hman, such as motor positions, modes, currents, and so on.
```

