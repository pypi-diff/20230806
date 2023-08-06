# Comparing `tmp/pydt3-0.0.5.tar.gz` & `tmp/pydt3-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydt3-0.0.5.tar", last modified: Thu May  4 08:33:44 2023, max compression
+gzip compressed data, was "pydt3-0.0.6.tar", last modified: Thu May  4 17:48:04 2023, max compression
```

## Comparing `pydt3-0.0.5.tar` & `pydt3-0.0.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 koc        (501) staff       (20)        0 2023-05-04 08:33:44.526252 pydt3-0.0.5/
--rw-r--r--   0 koc        (501) staff       (20)     1057 2023-05-01 21:26:29.000000 pydt3-0.0.5/LICENSE.txt
--rw-r--r--   0 koc        (501) staff       (20)     4986 2023-05-04 08:33:44.525636 pydt3-0.0.5/PKG-INFO
--rw-r--r--   0 koc        (501) staff       (20)     4576 2023-05-02 14:57:11.000000 pydt3-0.0.5/README.md
-drwxr-xr-x   0 koc        (501) staff       (20)        0 2023-05-04 08:33:44.505668 pydt3-0.0.5/pydt3/
--rw-r--r--   0 koc        (501) staff       (20)       75 2023-05-01 16:57:05.000000 pydt3-0.0.5/pydt3/__init__.py
--rw-r--r--   0 koc        (501) staff       (20)    13774 2023-05-04 05:35:22.000000 pydt3-0.0.5/pydt3/devonthink.py
--rw-r--r--   0 koc        (501) staff       (20)     5746 2023-05-04 08:16:13.000000 pydt3-0.0.5/pydt3/jxa_helper.scpt
-drwxr-xr-x   0 koc        (501) staff       (20)        0 2023-05-04 08:33:44.521422 pydt3-0.0.5/pydt3/models/
--rw-r--r--   0 koc        (501) staff       (20)        0 2023-05-01 19:54:18.000000 pydt3-0.0.5/pydt3/models/__init__.py
--rw-r--r--   0 koc        (501) staff       (20)     3713 2023-05-04 05:33:12.000000 pydt3-0.0.5/pydt3/models/database.py
--rw-r--r--   0 koc        (501) staff       (20)      254 2023-05-01 13:05:27.000000 pydt3-0.0.5/pydt3/models/item.py
--rw-r--r--   0 koc        (501) staff       (20)    21341 2023-05-04 07:57:38.000000 pydt3-0.0.5/pydt3/models/record.py
--rw-r--r--   0 koc        (501) staff       (20)     2272 2023-04-29 13:54:14.000000 pydt3-0.0.5/pydt3/models/reminder.py
--rw-r--r--   0 koc        (501) staff       (20)     1535 2023-05-04 05:24:23.000000 pydt3-0.0.5/pydt3/models/smartgroup.py
--rw-r--r--   0 koc        (501) staff       (20)        0 2023-04-29 15:08:38.000000 pydt3-0.0.5/pydt3/models/tab.py
--rw-r--r--   0 koc        (501) staff       (20)     1916 2023-05-01 20:20:12.000000 pydt3-0.0.5/pydt3/models/text.py
--rw-r--r--   0 koc        (501) staff       (20)     6078 2023-05-04 05:02:03.000000 pydt3-0.0.5/pydt3/models/windows.py
--rw-r--r--   0 koc        (501) staff       (20)     7751 2023-05-04 08:30:48.000000 pydt3-0.0.5/pydt3/osascript.py
--rw-r--r--   0 koc        (501) staff       (20)        0 2023-04-29 05:42:20.000000 pydt3-0.0.5/pydt3/utils.py
-drwxr-xr-x   0 koc        (501) staff       (20)        0 2023-05-04 08:33:44.509233 pydt3-0.0.5/pydt3.egg-info/
--rw-r--r--   0 koc        (501) staff       (20)     4986 2023-05-04 08:33:44.000000 pydt3-0.0.5/pydt3.egg-info/PKG-INFO
--rw-r--r--   0 koc        (501) staff       (20)      555 2023-05-04 08:33:44.000000 pydt3-0.0.5/pydt3.egg-info/SOURCES.txt
--rw-r--r--   0 koc        (501) staff       (20)        1 2023-05-04 08:33:44.000000 pydt3-0.0.5/pydt3.egg-info/dependency_links.txt
--rw-r--r--   0 koc        (501) staff       (20)       77 2023-05-04 08:33:44.000000 pydt3-0.0.5/pydt3.egg-info/requires.txt
--rw-r--r--   0 koc        (501) staff       (20)        6 2023-05-04 08:33:44.000000 pydt3-0.0.5/pydt3.egg-info/top_level.txt
--rw-r--r--   0 koc        (501) staff       (20)      714 2023-05-04 08:33:04.000000 pydt3-0.0.5/pyproject.toml
--rw-r--r--   0 koc        (501) staff       (20)       38 2023-05-04 08:33:44.526464 pydt3-0.0.5/setup.cfg
-drwxr-xr-x   0 koc        (501) staff       (20)        0 2023-05-04 08:33:44.524541 pydt3-0.0.5/tests/
--rw-r--r--   0 koc        (501) staff       (20)     1652 2023-05-04 05:36:41.000000 pydt3-0.0.5/tests/test_application.py
--rw-r--r--   0 koc        (501) staff       (20)     1713 2023-05-04 06:38:47.000000 pydt3-0.0.5/tests/test_database.py
--rw-r--r--   0 koc        (501) staff       (20)      862 2023-05-04 07:58:05.000000 pydt3-0.0.5/tests/test_record.py
+drwxr-xr-x   0 koc        (501) staff       (20)        0 2023-05-04 17:48:04.946778 pydt3-0.0.6/
+-rw-r--r--   0 koc        (501) staff       (20)     1057 2023-05-01 21:26:29.000000 pydt3-0.0.6/LICENSE.txt
+-rw-r--r--   0 koc        (501) staff       (20)     4986 2023-05-04 17:48:04.946213 pydt3-0.0.6/PKG-INFO
+-rw-r--r--   0 koc        (501) staff       (20)     4576 2023-05-02 14:57:11.000000 pydt3-0.0.6/README.md
+drwxr-xr-x   0 koc        (501) staff       (20)        0 2023-05-04 17:48:04.927029 pydt3-0.0.6/pydt3/
+-rw-r--r--   0 koc        (501) staff       (20)       75 2023-05-01 16:57:05.000000 pydt3-0.0.6/pydt3/__init__.py
+-rw-r--r--   0 koc        (501) staff       (20)    15172 2023-05-04 17:30:30.000000 pydt3-0.0.6/pydt3/devonthink.py
+-rw-r--r--   0 koc        (501) staff       (20)     5746 2023-05-04 08:16:13.000000 pydt3-0.0.6/pydt3/jxa_helper.scpt
+drwxr-xr-x   0 koc        (501) staff       (20)        0 2023-05-04 17:48:04.942047 pydt3-0.0.6/pydt3/models/
+-rw-r--r--   0 koc        (501) staff       (20)        0 2023-05-01 19:54:18.000000 pydt3-0.0.6/pydt3/models/__init__.py
+-rw-r--r--   0 koc        (501) staff       (20)     3713 2023-05-04 05:33:12.000000 pydt3-0.0.6/pydt3/models/database.py
+-rw-r--r--   0 koc        (501) staff       (20)      254 2023-05-01 13:05:27.000000 pydt3-0.0.6/pydt3/models/item.py
+-rw-r--r--   0 koc        (501) staff       (20)    21387 2023-05-04 09:03:08.000000 pydt3-0.0.6/pydt3/models/record.py
+-rw-r--r--   0 koc        (501) staff       (20)     2272 2023-04-29 13:54:14.000000 pydt3-0.0.6/pydt3/models/reminder.py
+-rw-r--r--   0 koc        (501) staff       (20)     1535 2023-05-04 05:24:23.000000 pydt3-0.0.6/pydt3/models/smartgroup.py
+-rw-r--r--   0 koc        (501) staff       (20)        0 2023-04-29 15:08:38.000000 pydt3-0.0.6/pydt3/models/tab.py
+-rw-r--r--   0 koc        (501) staff       (20)     1916 2023-05-01 20:20:12.000000 pydt3-0.0.6/pydt3/models/text.py
+-rw-r--r--   0 koc        (501) staff       (20)     6078 2023-05-04 05:02:03.000000 pydt3-0.0.6/pydt3/models/windows.py
+-rw-r--r--   0 koc        (501) staff       (20)     7751 2023-05-04 08:30:48.000000 pydt3-0.0.6/pydt3/osascript.py
+-rw-r--r--   0 koc        (501) staff       (20)        0 2023-04-29 05:42:20.000000 pydt3-0.0.6/pydt3/utils.py
+drwxr-xr-x   0 koc        (501) staff       (20)        0 2023-05-04 17:48:04.931403 pydt3-0.0.6/pydt3.egg-info/
+-rw-r--r--   0 koc        (501) staff       (20)     4986 2023-05-04 17:48:04.000000 pydt3-0.0.6/pydt3.egg-info/PKG-INFO
+-rw-r--r--   0 koc        (501) staff       (20)      555 2023-05-04 17:48:04.000000 pydt3-0.0.6/pydt3.egg-info/SOURCES.txt
+-rw-r--r--   0 koc        (501) staff       (20)        1 2023-05-04 17:48:04.000000 pydt3-0.0.6/pydt3.egg-info/dependency_links.txt
+-rw-r--r--   0 koc        (501) staff       (20)       77 2023-05-04 17:48:04.000000 pydt3-0.0.6/pydt3.egg-info/requires.txt
+-rw-r--r--   0 koc        (501) staff       (20)        6 2023-05-04 17:48:04.000000 pydt3-0.0.6/pydt3.egg-info/top_level.txt
+-rw-r--r--   0 koc        (501) staff       (20)      714 2023-05-04 17:47:31.000000 pydt3-0.0.6/pyproject.toml
+-rw-r--r--   0 koc        (501) staff       (20)       38 2023-05-04 17:48:04.946975 pydt3-0.0.6/setup.cfg
+drwxr-xr-x   0 koc        (501) staff       (20)        0 2023-05-04 17:48:04.944939 pydt3-0.0.6/tests/
+-rw-r--r--   0 koc        (501) staff       (20)     1652 2023-05-04 05:36:41.000000 pydt3-0.0.6/tests/test_application.py
+-rw-r--r--   0 koc        (501) staff       (20)     1713 2023-05-04 06:38:47.000000 pydt3-0.0.6/tests/test_database.py
+-rw-r--r--   0 koc        (501) staff       (20)      862 2023-05-04 07:58:05.000000 pydt3-0.0.6/tests/test_record.py
```

### Comparing `pydt3-0.0.5/LICENSE.txt` & `pydt3-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pydt3-0.0.5/PKG-INFO` & `pydt3-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydt3
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python API for Devonthink 3 utilizes AppleScript (JXA) and PyObjC.
 Author-email: astrosheep <astrosheepthesheep@outlook.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `pydt3-0.0.5/README.md` & `pydt3-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pydt3-0.0.5/pydt3/devonthink.py` & `pydt3-0.0.6/pydt3/devonthink.py`

 * *Files 9% similar despite different names*

```diff
@@ -151,14 +151,46 @@
             'defaultButton': default_button,
             'withIcon': with_icon,
         }
 
         kwargs = {k: v for k, v in kwargs.items() if v is not None}
         return self.call_method('displayDialog', [text], kwargs)
     
+    
+    def display_notification(self, text: str, with_title: str = None, subtitle: str = None, sound_name: str = None) -> None:
+        return self.call_method('displayNotification', [text], {
+            'withTitle': with_title,
+            'subtitle': subtitle,
+            'soundName': sound_name,
+        })
+    
+    
+    # DEVONthink suit
+
+    def show_progress_indicator(self, title: str, cancel_button: bool, steps: int) -> bool:
+        """Show a progress indicator or update an already visible indicator. You have to ensure that the indicator is hidden again via 'hide progress indicator' when the script ends or if an error occurs.
+        
+        Args:
+            title (str): The title of the progress.
+            cancel_button (bool):  Display a button to cancel the process.
+            steps (int):  The number of steps of the progress or a negative value for an indeterminate number.
+        """
+        return self.call_method('showProgressIndicator', [title], {
+            'cancelButton': cancel_button,
+            'steps': steps,
+        })
+    
+    def hide_progress_indicator(self) -> bool:
+        """Hide a visible progress indicator."""
+        return self.call_method('hideProgressIndicator')
+        
+    def step_progress_indicator(self, title) -> bool:
+        """Go to next step of a progress."""
+        return self.call_method('stepProgressIndicator', [title])
+
     def search(self, text: str, comparision: str = 'no case', excludeSubgroups: bool = False) -> List[Record]:
         """Search for records in specified group or all databases.
 
         Args:
             text (str): The search string.
             comparision (str, optional):  The comparison to use (default `'no case'`). One of fuzzy/‌no case/‌no umlauts.
             excludeSubgroups (bool, optional): Don't search in subgroups of the specified group. (default `false`).
@@ -247,15 +279,15 @@
             'database': database,
         })
 
     def create_record_with(self, properties: dict, in_: Optional['Record'] = None) -> Record:
         """Create a new record.
 
         Args:
-            record (Record): The properties of the record. Possible keys for record are 'name', 'type', 'comment', 'path', 'URL', 'creation date', 'modification date', 'date', 'plain text', 'rich text', 'source', 'data', 'content', 'columns', 'cells', 'thumbnail' and 'tags'.
+            record (dict): The properties of the record. Possible keys for record are 'name', 'type', 'comment', 'path', 'URL', 'creation date', 'modification date', 'date', 'plain text', 'rich text', 'source', 'data', 'content', 'columns', 'cells', 'thumbnail' and 'tags'.
             in_ (Record, optional): The destination group for the new record. Uses incoming group or group selector if not specified.
         Returns:
             Record: The newly created record.
         """
         return self.call_method('createRecordWith', [properties], {'in': in_})
 
     def delete(self, record: 'Record', in_: Optional['Record'] = None) -> bool:
```

### Comparing `pydt3-0.0.5/pydt3/jxa_helper.scpt` & `pydt3-0.0.6/pydt3/jxa_helper.scpt`

 * *Files identical despite different names*

### Comparing `pydt3-0.0.5/pydt3/models/database.py` & `pydt3-0.0.6/pydt3/models/database.py`

 * *Files identical despite different names*

### Comparing `pydt3-0.0.5/pydt3/models/record.py` & `pydt3-0.0.6/pydt3/models/record.py`

 * *Files 0% similar despite different names*

```diff
@@ -611,8 +611,9 @@
     
     def __repr__(self):
         return f'<Record: {self.name}>'
 
 OSAObjProxy._NAME_CLASS_MAP['record'] = Record
 OSAObjProxy._NAME_CLASS_MAP['content'] = Record
 OSAObjProxy._NAME_CLASS_MAP['parent'] = Record
+OSAObjProxy._NAME_CLASS_MAP['child'] = Record
 OSAObjProxy._NAME_CLASS_MAP['selectedRecord'] = Record
```

### Comparing `pydt3-0.0.5/pydt3/models/reminder.py` & `pydt3-0.0.6/pydt3/models/reminder.py`

 * *Files identical despite different names*

### Comparing `pydt3-0.0.5/pydt3/models/smartgroup.py` & `pydt3-0.0.6/pydt3/models/smartgroup.py`

 * *Files identical despite different names*

### Comparing `pydt3-0.0.5/pydt3/models/text.py` & `pydt3-0.0.6/pydt3/models/text.py`

 * *Files identical despite different names*

### Comparing `pydt3-0.0.5/pydt3/models/windows.py` & `pydt3-0.0.6/pydt3/models/windows.py`

 * *Files identical despite different names*

### Comparing `pydt3-0.0.5/pydt3/osascript.py` & `pydt3-0.0.6/pydt3/osascript.py`

 * *Files identical despite different names*

### Comparing `pydt3-0.0.5/pydt3.egg-info/PKG-INFO` & `pydt3-0.0.6/pydt3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydt3
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python API for Devonthink 3 utilizes AppleScript (JXA) and PyObjC.
 Author-email: astrosheep <astrosheepthesheep@outlook.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `pydt3-0.0.5/pydt3.egg-info/SOURCES.txt` & `pydt3-0.0.6/pydt3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydt3-0.0.5/pyproject.toml` & `pydt3-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "pydt3"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="astrosheep", email="astrosheepthesheep@outlook.com" },
 ]
 description = "Python API for Devonthink 3 utilizes AppleScript (JXA) and PyObjC."
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = ["pyobjc-core", "pyobjc-framework-AppleScriptKit", "pyobjc-framework-AppleScriptObjC"]
```

### Comparing `pydt3-0.0.5/tests/test_application.py` & `pydt3-0.0.6/tests/test_application.py`

 * *Files identical despite different names*

### Comparing `pydt3-0.0.5/tests/test_database.py` & `pydt3-0.0.6/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `pydt3-0.0.5/tests/test_record.py` & `pydt3-0.0.6/tests/test_record.py`

 * *Files identical despite different names*

