# Comparing `tmp/slack-serverless-2023.1003a0.tar.gz` & `tmp/slack-serverless-2023.1004a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slack-serverless-2023.1003a0.tar", last modified: Sat Aug  5 18:03:59 2023, max compression
+gzip compressed data, was "slack-serverless-2023.1004a0.tar", last modified: Sat Aug  5 21:31:06 2023, max compression
```

## Comparing `slack-serverless-2023.1003a0.tar` & `slack-serverless-2023.1004a0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 rosco      (501) staff       (20)        0 2023-08-05 18:03:59.084028 slack-serverless-2023.1003a0/
--rw-r--r--   0 rosco      (501) staff       (20)     1074 2023-08-05 16:16:02.000000 slack-serverless-2023.1003a0/LICENSE.md
--rw-r--r--   0 rosco      (501) staff       (20)     3473 2023-08-05 18:03:59.083666 slack-serverless-2023.1003a0/PKG-INFO
--rw-r--r--   0 rosco      (501) staff       (20)     1810 2023-08-05 16:28:50.000000 slack-serverless-2023.1003a0/README.md
--rw-r--r--   0 rosco      (501) staff       (20)     1310 2023-08-05 18:03:43.000000 slack-serverless-2023.1003a0/pyproject.toml
--rw-r--r--   0 rosco      (501) staff       (20)       38 2023-08-05 18:03:59.084161 slack-serverless-2023.1003a0/setup.cfg
-drwxr-xr-x   0 rosco      (501) staff       (20)        0 2023-08-05 18:03:59.081264 slack-serverless-2023.1003a0/src/
--rw-r--r--   0 rosco      (501) staff       (20)     3217 2023-08-05 18:02:47.000000 slack-serverless-2023.1003a0/src/slack_deferred_gcp.py
--rw-r--r--   0 rosco      (501) staff       (20)     2330 2023-08-05 16:31:23.000000 slack-serverless-2023.1003a0/src/slack_messaging.py
-drwxr-xr-x   0 rosco      (501) staff       (20)        0 2023-08-05 18:03:59.083232 slack-serverless-2023.1003a0/src/slack_serverless.egg-info/
--rw-r--r--   0 rosco      (501) staff       (20)     3473 2023-08-05 18:03:59.000000 slack-serverless-2023.1003a0/src/slack_serverless.egg-info/PKG-INFO
--rw-r--r--   0 rosco      (501) staff       (20)      327 2023-08-05 18:03:59.000000 slack-serverless-2023.1003a0/src/slack_serverless.egg-info/SOURCES.txt
--rw-r--r--   0 rosco      (501) staff       (20)        1 2023-08-05 18:03:59.000000 slack-serverless-2023.1003a0/src/slack_serverless.egg-info/dependency_links.txt
--rw-r--r--   0 rosco      (501) staff       (20)      100 2023-08-05 18:03:59.000000 slack-serverless-2023.1003a0/src/slack_serverless.egg-info/requires.txt
--rw-r--r--   0 rosco      (501) staff       (20)       52 2023-08-05 18:03:59.000000 slack-serverless-2023.1003a0/src/slack_serverless.egg-info/top_level.txt
--rw-r--r--   0 rosco      (501) staff       (20)     3794 2023-08-05 16:31:23.000000 slack-serverless-2023.1003a0/src/slack_serverless.py
+drwxr-xr-x   0 rosco      (501) staff       (20)        0 2023-08-05 21:31:06.409761 slack-serverless-2023.1004a0/
+-rw-r--r--   0 rosco      (501) staff       (20)     1074 2023-08-05 16:16:02.000000 slack-serverless-2023.1004a0/LICENSE.md
+-rw-r--r--   0 rosco      (501) staff       (20)     3473 2023-08-05 21:31:06.409494 slack-serverless-2023.1004a0/PKG-INFO
+-rw-r--r--   0 rosco      (501) staff       (20)     1810 2023-08-05 16:28:50.000000 slack-serverless-2023.1004a0/README.md
+-rw-r--r--   0 rosco      (501) staff       (20)     1310 2023-08-05 21:30:54.000000 slack-serverless-2023.1004a0/pyproject.toml
+-rw-r--r--   0 rosco      (501) staff       (20)       38 2023-08-05 21:31:06.409844 slack-serverless-2023.1004a0/setup.cfg
+drwxr-xr-x   0 rosco      (501) staff       (20)        0 2023-08-05 21:31:06.403375 slack-serverless-2023.1004a0/src/
+-rw-r--r--   0 rosco      (501) staff       (20)     3217 2023-08-05 18:02:47.000000 slack-serverless-2023.1004a0/src/slack_deferred_gcp.py
+-rw-r--r--   0 rosco      (501) staff       (20)     2330 2023-08-05 16:31:23.000000 slack-serverless-2023.1004a0/src/slack_messaging.py
+drwxr-xr-x   0 rosco      (501) staff       (20)        0 2023-08-05 21:31:06.408880 slack-serverless-2023.1004a0/src/slack_serverless.egg-info/
+-rw-r--r--   0 rosco      (501) staff       (20)     3473 2023-08-05 21:31:06.000000 slack-serverless-2023.1004a0/src/slack_serverless.egg-info/PKG-INFO
+-rw-r--r--   0 rosco      (501) staff       (20)      327 2023-08-05 21:31:06.000000 slack-serverless-2023.1004a0/src/slack_serverless.egg-info/SOURCES.txt
+-rw-r--r--   0 rosco      (501) staff       (20)        1 2023-08-05 21:31:06.000000 slack-serverless-2023.1004a0/src/slack_serverless.egg-info/dependency_links.txt
+-rw-r--r--   0 rosco      (501) staff       (20)      100 2023-08-05 21:31:06.000000 slack-serverless-2023.1004a0/src/slack_serverless.egg-info/requires.txt
+-rw-r--r--   0 rosco      (501) staff       (20)       52 2023-08-05 21:31:06.000000 slack-serverless-2023.1004a0/src/slack_serverless.egg-info/top_level.txt
+-rw-r--r--   0 rosco      (501) staff       (20)     7947 2023-08-05 21:30:25.000000 slack-serverless-2023.1004a0/src/slack_serverless.py
```

### Comparing `slack-serverless-2023.1003a0/LICENSE.md` & `slack-serverless-2023.1004a0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `slack-serverless-2023.1003a0/PKG-INFO` & `slack-serverless-2023.1004a0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slack-serverless
-Version: 2023.1003a0
+Version: 2023.1004a0
 Summary: Simplified serverless Slack bot interactions
 Author-email: Ross Bamford <roscopeco@gmail.com>
 License: Copyright 2023 Ross Bamford & Contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `slack-serverless-2023.1003a0/README.md` & `slack-serverless-2023.1004a0/README.md`

 * *Files identical despite different names*

### Comparing `slack-serverless-2023.1003a0/pyproject.toml` & `slack-serverless-2023.1004a0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "slack-serverless"
-version = "2023.1003-alpha"
+version = "2023.1004-alpha"
 description = "Simplified serverless Slack bot interactions"
 readme = "README.md"
 authors = [{ name = "Ross Bamford", email = "roscopeco@gmail.com" }]
 license = { file = "LICENSE.md" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -24,15 +24,15 @@
 [project.optional-dependencies]
 dev = ["black", "bumpver", "pre-commit", "isort", "pip-tools", "pytest"]
 
 [project.urls]
 Homepage = "https://github.com/roscopeco/slack-serverless"
 
 [tool.bumpver]
-current_version = "2023.1003-alpha"
+current_version = "2023.1004-alpha"
 version_pattern = "YYYY.BUILD[-TAG]"
 commit_message = "bump version {old_version} -> {new_version}"
 tag_message = "{new_version}"
 tag_scope = "default"
 commit = true
 tag = true
 push = true
```

### Comparing `slack-serverless-2023.1003a0/src/slack_deferred_gcp.py` & `slack-serverless-2023.1004a0/src/slack_deferred_gcp.py`

 * *Files identical despite different names*

### Comparing `slack-serverless-2023.1003a0/src/slack_messaging.py` & `slack-serverless-2023.1004a0/src/slack_messaging.py`

 * *Files identical despite different names*

### Comparing `slack-serverless-2023.1003a0/src/slack_serverless.egg-info/PKG-INFO` & `slack-serverless-2023.1004a0/src/slack_serverless.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slack-serverless
-Version: 2023.1003a0
+Version: 2023.1004a0
 Summary: Simplified serverless Slack bot interactions
 Author-email: Ross Bamford <roscopeco@gmail.com>
 License: Copyright 2023 Ross Bamford & Contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

