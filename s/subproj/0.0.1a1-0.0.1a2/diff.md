# Comparing `tmp/subproj-0.0.1a1-py3-none-any.whl.zip` & `tmp/subproj-0.0.1a2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,32 @@
-Zip file size: 4811 bytes, number of entries: 11
--rw-r--r--  2.0 unx      100 b- defN 23-Jul-21 09:25 subproj/__init__.py
--rw-r--r--  2.0 unx     1155 b- defN 23-Jul-21 09:25 subproj/__main__.py
--rw-r--r--  2.0 unx      542 b- defN 23-Jul-21 09:25 subproj/logging.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 09:25 subproj/setup/__init__.py
--rw-r--r--  2.0 unx      606 b- defN 23-Jul-21 09:25 subproj/setup/update.py
--rw-r--r--  2.0 unx     1515 b- defN 23-Jul-21 10:42 subproj-0.0.1a1.dist-info/LICENSE.rst
--rw-r--r--  2.0 unx     1563 b- defN 23-Jul-21 10:42 subproj-0.0.1a1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-21 10:42 subproj-0.0.1a1.dist-info/WHEEL
--rw-r--r--  2.0 unx       50 b- defN 23-Jul-21 10:42 subproj-0.0.1a1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 23-Jul-21 10:42 subproj-0.0.1a1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      879 b- defN 23-Jul-21 10:42 subproj-0.0.1a1.dist-info/RECORD
-11 files, 6510 bytes uncompressed, 3315 bytes compressed:  49.1%
+Zip file size: 18008 bytes, number of entries: 30
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Aug-06 07:54 subproj/__init__.py
+-rw-rw-rw-  2.0 fat     1155 b- defN 23-Jul-20 06:16 subproj/__main__.py
+-rw-rw-rw-  2.0 fat      542 b- defN 22-Sep-19 19:24 subproj/logging.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-20 06:07 subproj/setup/__init__.py
+-rw-rw-rw-  2.0 fat      606 b- defN 23-Jul-20 06:18 subproj/setup/update.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Aug-06 07:54 subproj/widget/__init__.py
+-rw-rw-rw-  2.0 fat     4571 b- defN 23-Jul-19 05:37 subproj/widget/tk_base.py
+-rw-rw-rw-  2.0 fat     2052 b- defN 23-Jul-17 08:24 subproj/widget/tk_commit.py
+-rw-rw-rw-  2.0 fat    15646 b- defN 23-Aug-06 07:50 subproj/widget/tk_subproj.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-14 05:21 subproj/widget/actions/__init__.py
+-rw-rw-rw-  2.0 fat     2037 b- defN 23-Jul-20 06:20 subproj/widget/actions/package_install.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-14 05:12 subproj/widget/startup/__init__.py
+-rw-rw-rw-  2.0 fat     1867 b- defN 23-Jul-14 05:10 subproj/widget/startup/app_checks.py
+-rw-rw-rw-  2.0 fat      614 b- defN 23-Aug-06 07:55 subproj/widget/widgets/__init__.py
+-rw-rw-rw-  2.0 fat      386 b- defN 23-Jul-14 13:59 subproj/widget/widgets/button_quit.py
+-rw-rw-rw-  2.0 fat      360 b- defN 23-Jul-17 09:11 subproj/widget/widgets/label.py
+-rw-rw-rw-  2.0 fat     1177 b- defN 23-Jul-17 09:27 subproj/widget/widgets/local_subproj_tree.py
+-rw-rw-rw-  2.0 fat      449 b- defN 23-Jul-17 09:27 subproj/widget/widgets/log.py
+-rw-rw-rw-  2.0 fat     1052 b- defN 23-Jul-17 09:27 subproj/widget/widgets/remote_package_tree.py
+-rw-rw-rw-  2.0 fat      569 b- defN 23-Jul-14 11:40 subproj/widget/widgets/select_proj.py
+-rw-rw-rw-  2.0 fat      449 b- defN 23-Jul-14 11:56 subproj/widget/widgets/select_remote.py
+-rw-rw-rw-  2.0 fat      465 b- defN 23-Jul-14 11:40 subproj/widget/widgets/select_subproj.py
+-rw-rw-rw-  2.0 fat      439 b- defN 23-Jul-14 13:21 subproj/widget/widgets/startup_state.py
+-rw-rw-rw-  2.0 fat      580 b- defN 23-Jul-14 12:51 subproj/widget/widgets/worker_progress.py
+-rw-rw-rw-  2.0 fat     1515 b- defN 23-Aug-06 08:01 subproj-0.0.1a2.dist-info/LICENSE.rst
+-rw-rw-rw-  2.0 fat     1633 b- defN 23-Aug-06 08:01 subproj-0.0.1a2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-06 08:01 subproj-0.0.1a2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       50 b- defN 23-Aug-06 08:01 subproj-0.0.1a2.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Aug-06 08:01 subproj-0.0.1a2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     2612 b- defN 23-Aug-06 08:01 subproj-0.0.1a2.dist-info/RECORD
+30 files, 41026 bytes uncompressed, 13734 bytes compressed:  66.5%
```

## zipnote {}

```diff
@@ -9,26 +9,83 @@
 
 Filename: subproj/setup/__init__.py
 Comment: 
 
 Filename: subproj/setup/update.py
 Comment: 
 
-Filename: subproj-0.0.1a1.dist-info/LICENSE.rst
+Filename: subproj/widget/__init__.py
 Comment: 
 
-Filename: subproj-0.0.1a1.dist-info/METADATA
+Filename: subproj/widget/tk_base.py
 Comment: 
 
-Filename: subproj-0.0.1a1.dist-info/WHEEL
+Filename: subproj/widget/tk_commit.py
 Comment: 
 
-Filename: subproj-0.0.1a1.dist-info/entry_points.txt
+Filename: subproj/widget/tk_subproj.py
 Comment: 
 
-Filename: subproj-0.0.1a1.dist-info/top_level.txt
+Filename: subproj/widget/actions/__init__.py
 Comment: 
 
-Filename: subproj-0.0.1a1.dist-info/RECORD
+Filename: subproj/widget/actions/package_install.py
+Comment: 
+
+Filename: subproj/widget/startup/__init__.py
+Comment: 
+
+Filename: subproj/widget/startup/app_checks.py
+Comment: 
+
+Filename: subproj/widget/widgets/__init__.py
+Comment: 
+
+Filename: subproj/widget/widgets/button_quit.py
+Comment: 
+
+Filename: subproj/widget/widgets/label.py
+Comment: 
+
+Filename: subproj/widget/widgets/local_subproj_tree.py
+Comment: 
+
+Filename: subproj/widget/widgets/log.py
+Comment: 
+
+Filename: subproj/widget/widgets/remote_package_tree.py
+Comment: 
+
+Filename: subproj/widget/widgets/select_proj.py
+Comment: 
+
+Filename: subproj/widget/widgets/select_remote.py
+Comment: 
+
+Filename: subproj/widget/widgets/select_subproj.py
+Comment: 
+
+Filename: subproj/widget/widgets/startup_state.py
+Comment: 
+
+Filename: subproj/widget/widgets/worker_progress.py
+Comment: 
+
+Filename: subproj-0.0.1a2.dist-info/LICENSE.rst
+Comment: 
+
+Filename: subproj-0.0.1a2.dist-info/METADATA
+Comment: 
+
+Filename: subproj-0.0.1a2.dist-info/WHEEL
+Comment: 
+
+Filename: subproj-0.0.1a2.dist-info/entry_points.txt
+Comment: 
+
+Filename: subproj-0.0.1a2.dist-info/top_level.txt
+Comment: 
+
+Filename: subproj-0.0.1a2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## subproj/__init__.py

```diff
@@ -1,6 +1,6 @@
 """
 Runtime metadata for the ``subproj`` module.
 """
 
-__version__ = "0.0.1a1"
+__version__ = "0.0.1a2"
 "Full version string"
```

## Comparing `subproj-0.0.1a1.dist-info/LICENSE.rst` & `subproj-0.0.1a2.dist-info/LICENSE.rst`

 * *Files identical despite different names*

## Comparing `subproj-0.0.1a1.dist-info/METADATA` & `subproj-0.0.1a2.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-Metadata-Version: 2.1
-Name: subproj
-Version: 0.0.1a1
-Summary: Handle PVSS subprojects
-Home-page: https://gitlab.com/fholmer/subproj
-Author: Frode Holmer
-Author-email: fholmer+subproj@gmail.com
-License: BSD-3-Clause
-Project-URL: Documentation, https://fholmer.gitlab.io/subproj
-Project-URL: Source Code, https://gitlab.com/fholmer/subproj
-Keywords: subproj,subprojects,deploy,install,on-prem,pvss
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-License-File: LICENSE.rst
-Requires-Dist: adop
-Requires-Dist: keyring
-
-=======
-subproj
-=======
-
-* PyPI: https://pypi.org/project/subproj/
-* Downloads: https://gitlab.com/fholmer/subproj/-/packages
-* Documentation: https://fholmer.gitlab.io/subproj
-* Source Code: https://gitlab.com/fholmer/subproj
-* License: BSD License
-
-Summary
-=======
-
-Handle subprojects on-prem.
-
-Warning
-=======
-
-* This is a beta version. Not ready for production.
-
-
-Installation
-============
-
-Open command line and and install using pip:
-
-.. code-block:: console
-
-    $ pip install subproj
-
-
-Usage
-=====
-
-subproj is available as console script and library module
-
-.. code-block:: console
-
-    $ subproj -h
-    $ python -m subproj -h
-
-Update a project
-
-.. code-block:: console
-
-  $ cd proj
-  $ subproj update .
+Metadata-Version: 2.1
+Name: subproj
+Version: 0.0.1a2
+Summary: Handle PVSS subprojects
+Home-page: https://gitlab.com/fholmer/subproj
+Author: Frode Holmer
+Author-email: fholmer+subproj@gmail.com
+License: BSD-3-Clause
+Project-URL: Documentation, https://fholmer.gitlab.io/subproj
+Project-URL: Source Code, https://gitlab.com/fholmer/subproj
+Keywords: subproj,subprojects,deploy,install,on-prem,pvss
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+License-File: LICENSE.rst
+Requires-Dist: adop
+Requires-Dist: keyring
+
+=======
+subproj
+=======
+
+* PyPI: https://pypi.org/project/subproj/
+* Downloads: https://gitlab.com/fholmer/subproj/-/packages
+* Documentation: https://fholmer.gitlab.io/subproj
+* Source Code: https://gitlab.com/fholmer/subproj
+* License: BSD License
+
+Summary
+=======
+
+Handle subprojects on-prem.
+
+Warning
+=======
+
+* This is a beta version. Not ready for production.
+
+
+Installation
+============
+
+Open command line and and install using pip:
+
+.. code-block:: console
+
+    $ pip install subproj
+
+
+Usage
+=====
+
+subproj is available as console script and library module
+
+.. code-block:: console
+
+    $ subproj -h
+    $ python -m subproj -h
+
+Update a project
+
+.. code-block:: console
+
+  $ cd proj
+  $ subproj update .
```

