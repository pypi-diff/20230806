# Comparing `tmp/robothub_oak-1.4.0.tar.gz` & `tmp/robothub_oak-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robothub_oak-1.4.0.tar", last modified: Tue Jun 27 23:12:29 2023, max compression
+gzip compressed data, was "robothub_oak-2.0.0.tar", last modified: Sun Aug  6 12:00:19 2023, max compression
```

## Comparing `robothub_oak-1.4.0.tar` & `robothub_oak-2.0.0.tar`

### file list

```diff
@@ -1,39 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:12:29.337386 robothub_oak-1.4.0/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1064 2023-06-27 23:11:54.000000 robothub_oak-1.4.0/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (123)       39 2023-06-27 23:11:54.000000 robothub_oak-1.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-27 23:12:29.337386 robothub_oak-1.4.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)      585 2023-06-27 23:11:54.000000 robothub_oak-1.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 23:12:29.337386 robothub_oak-1.4.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1291 2023-06-27 23:11:54.000000 robothub_oak-1.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:12:29.321386 robothub_oak-1.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:12:29.329386 robothub_oak-1.4.0/src/robothub_oak/
--rwxr-xr-x   0 runner    (1001) docker     (123)      256 2023-06-27 23:11:54.000000 robothub_oak-1.4.0/src/robothub_oak/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1972 2023-06-27 23:11:54.000000 robothub_oak-1.4.0/src/robothub_oak/callbacks.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13996 2023-06-27 23:11:54.000000 robothub_oak-1.4.0/src/robothub_oak/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:12:29.333386 robothub_oak-1.4.0/src/robothub_oak/components/
--rwxr-xr-x   0 runner    (1001) docker     (123)       74 2023-06-27 23:11:54.000000 robothub_oak-1.4.0/src/robothub_oak/components/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1367 2023-06-27 23:11:54.000000 robothub_oak-1.4.0/src/robothub_oak/components/_component.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      410 2023-06-27 23:11:54.000000 robothub_oak-1.4.0/src/robothub_oak/components/_streamable.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5101 2023-06-27 23:11:54.000000 robothub_oak-1.4.0/src/robothub_oak/components/camera.py
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:11:54.000000 robothub_oak-1.4.0/src/robothub_oak/components/imu.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3173 2023-06-27 23:11:54.000000 robothub_oak-1.4.0/src/robothub_oak/components/neural_network.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4460 2023-06-27 23:11:54.000000 robothub_oak-1.4.0/src/robothub_oak/components/stereo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8486 2023-06-27 23:11:54.000000 robothub_oak-1.4.0/src/robothub_oak/device.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13748 2023-06-27 23:11:54.000000 robothub_oak-1.4.0/src/robothub_oak/hub_camera.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8656 2023-06-27 23:11:54.000000 robothub_oak-1.4.0/src/robothub_oak/manager.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2465 2023-06-27 23:11:54.000000 robothub_oak-1.4.0/src/robothub_oak/packets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:12:29.333386 robothub_oak-1.4.0/src/robothub_oak/trigger_action/
--rwxr-xr-x   0 runner    (1001) docker     (123)       47 2023-06-27 23:11:54.000000 robothub_oak-1.4.0/src/robothub_oak/trigger_action/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      924 2023-06-27 23:11:54.000000 robothub_oak-1.4.0/src/robothub_oak/trigger_action/actions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      952 2023-06-27 23:11:54.000000 robothub_oak-1.4.0/src/robothub_oak/trigger_action/triggers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      142 2023-06-27 23:11:54.000000 robothub_oak-1.4.0/src/robothub_oak/types.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1232 2023-06-27 23:11:54.000000 robothub_oak-1.4.0/src/robothub_oak/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:12:29.329386 robothub_oak-1.4.0/src/robothub_oak.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-27 23:12:29.000000 robothub_oak-1.4.0/src/robothub_oak.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-27 23:12:29.000000 robothub_oak-1.4.0/src/robothub_oak.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 23:12:29.000000 robothub_oak-1.4.0/src/robothub_oak.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-27 23:12:29.000000 robothub_oak-1.4.0/src/robothub_oak.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:12:29.337386 robothub_oak-1.4.0/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:11:54.000000 robothub_oak-1.4.0/tests/test_callback.py
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:11:54.000000 robothub_oak-1.4.0/tests/test_hub_camera.py
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:11:54.000000 robothub_oak-1.4.0/tests/test_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:00:19.558300 robothub_oak-2.0.0/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1065 2023-08-06 11:59:49.000000 robothub_oak-2.0.0/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-08-06 11:59:49.000000 robothub_oak-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-08-06 12:00:19.558300 robothub_oak-2.0.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)      629 2023-08-06 11:59:49.000000 robothub_oak-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 12:00:19.558300 robothub_oak-2.0.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1286 2023-08-06 11:59:49.000000 robothub_oak-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:00:19.554300 robothub_oak-2.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:00:19.554300 robothub_oak-2.0.0/src/robothub_oak/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      379 2023-08-06 11:59:49.000000 robothub_oak-2.0.0/src/robothub_oak/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-08-06 11:59:49.000000 robothub_oak-2.0.0/src/robothub_oak/application.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:00:19.558300 robothub_oak-2.0.0/src/robothub_oak/data_processors/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-06 11:59:49.000000 robothub_oak-2.0.0/src/robothub_oak/data_processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-06 11:59:49.000000 robothub_oak-2.0.0/src/robothub_oak/data_processors/base_processor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3568 2023-08-06 11:59:49.000000 robothub_oak-2.0.0/src/robothub_oak/events.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10322 2023-08-06 11:59:49.000000 robothub_oak-2.0.0/src/robothub_oak/live_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-08-06 11:59:49.000000 robothub_oak-2.0.0/src/robothub_oak/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-08-06 11:59:49.000000 robothub_oak-2.0.0/src/robothub_oak/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:00:19.558300 robothub_oak-2.0.0/src/robothub_oak.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-08-06 12:00:19.000000 robothub_oak-2.0.0/src/robothub_oak.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-08-06 12:00:19.000000 robothub_oak-2.0.0/src/robothub_oak.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 12:00:19.000000 robothub_oak-2.0.0/src/robothub_oak.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-06 12:00:19.000000 robothub_oak-2.0.0/src/robothub_oak.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:00:19.558300 robothub_oak-2.0.0/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:59:49.000000 robothub_oak-2.0.0/tests/test_callback.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:59:49.000000 robothub_oak-2.0.0/tests/test_hub_camera.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:59:49.000000 robothub_oak-2.0.0/tests/test_manager.py
```

### Comparing `robothub_oak-1.4.0/LICENSE` & `robothub_oak-2.0.0/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -10,12 +10,12 @@
 furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all
 copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+FITNESS FOR A PARTICULAR PURPOSE AND NON-INFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `robothub_oak-1.4.0/PKG-INFO` & `robothub_oak-2.0.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: robothub_oak
-Version: 1.4.0
-Summary: RobotHub-OAK integration library
+Version: 2.0.0
+Summary: RobotHub integration library
 Home-page: https://www.luxonis.com/
 Author: Luxonis
 Author-email: support@luxonis.com
 License: MIT
-Project-URL: Homepage, https://github.com/luxonis/robothub-oak/
+Project-URL: Homepage, https://github.com/luxonis/robothub/
 Project-URL: Documentation, https://hub-docs.luxonis.com/
-Keywords: robothub robot hub connect agent depthai oak sdk
+Keywords: robothub camera robot hub connect agent depthai sdk
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
@@ -40,12 +40,12 @@
 
 ```
 $ python3 -m pip install robothub-oak
 ```
 
 ## Examples
 
-There are several examples in the [examples](examples) folder.
+You can find examples in the [robothub-examples](https://github.com/luxonis/robothub-examples) repository.
 
 ## License
 
 This project is licensed under the terms of the MIT license.
```

### Comparing `robothub_oak-1.4.0/setup.py` & `robothub_oak-2.0.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 
 from setuptools import setup
 
 long_description = io.open('README.md', encoding='utf-8').read()
 
 setup(
     name='robothub_oak',
-    version='1.4.0',
-    description='RobotHub-OAK integration library',
+    version='2.0.0',
+    description='RobotHub integration library',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://www.luxonis.com/',
     license='MIT',
-    keywords='robothub robot hub connect agent depthai oak sdk',
+    keywords='robothub camera robot hub connect agent depthai sdk',
     author='Luxonis',
     author_email='support@luxonis.com',
     packages=['robothub_oak'],
     package_dir={'': 'src'},  # https://stackoverflow.com/a/67238346/5494277
     include_package_data=True,
     project_urls={
-        'Homepage': 'https://github.com/luxonis/robothub-oak/',
+        'Homepage': 'https://github.com/luxonis/robothub/',
         'Documentation': 'https://hub-docs.luxonis.com/',
     },
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'Intended Audience :: Education',
         'Intended Audience :: Information Technology',
```

### Comparing `robothub_oak-1.4.0/src/robothub_oak.egg-info/PKG-INFO` & `robothub_oak-2.0.0/src/robothub_oak.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: robothub-oak
-Version: 1.4.0
-Summary: RobotHub-OAK integration library
+Version: 2.0.0
+Summary: RobotHub integration library
 Home-page: https://www.luxonis.com/
 Author: Luxonis
 Author-email: support@luxonis.com
 License: MIT
-Project-URL: Homepage, https://github.com/luxonis/robothub-oak/
+Project-URL: Homepage, https://github.com/luxonis/robothub/
 Project-URL: Documentation, https://hub-docs.luxonis.com/
-Keywords: robothub robot hub connect agent depthai oak sdk
+Keywords: robothub camera robot hub connect agent depthai sdk
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
@@ -40,12 +40,12 @@
 
 ```
 $ python3 -m pip install robothub-oak
 ```
 
 ## Examples
 
-There are several examples in the [examples](examples) folder.
+You can find examples in the [robothub-examples](https://github.com/luxonis/robothub-examples) repository.
 
 ## License
 
 This project is licensed under the terms of the MIT license.
```

