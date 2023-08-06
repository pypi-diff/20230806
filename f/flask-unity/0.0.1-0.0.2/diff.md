# Comparing `tmp/flask_unity-0.0.1.tar.gz` & `tmp/flask_unity-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_unity-0.0.1.tar", last modified: Sat Aug  5 18:39:27 2023, max compression
+gzip compressed data, was "flask_unity-0.0.2.tar", last modified: Sun Aug  6 07:34:08 2023, max compression
```

## Comparing `flask_unity-0.0.1.tar` & `flask_unity-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,55 @@
-drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-08-05 18:39:27.488060 flask_unity-0.0.1/
--rw-rw-r--   0 usman     (1000) usman     (1000)       81 2023-08-05 06:53:11.000000 flask_unity-0.0.1/CHANGELOG
--rw-rw-r--   0 usman     (1000) usman     (1000)     1077 2023-08-05 06:53:20.000000 flask_unity-0.0.1/LICENSE
--rw-rw-r--   0 usman     (1000) usman     (1000)       54 2023-08-04 10:00:06.000000 flask_unity-0.0.1/MANIFEST.in
--rw-rw-r--   0 usman     (1000) usman     (1000)     3366 2023-08-05 18:39:27.468060 flask_unity-0.0.1/PKG-INFO
--rw-rw-r--   0 usman     (1000) usman     (1000)     2543 2023-08-05 07:15:59.000000 flask_unity-0.0.1/README.md
-drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-08-05 18:39:27.444060 flask_unity-0.0.1/flask_unity/
--rw-rw-r--   0 usman     (1000) usman     (1000)     1101 2023-08-05 18:36:58.000000 flask_unity-0.0.1/flask_unity/__init__.py
--rw-rw-r--   0 usman     (1000) usman     (1000)      157 2023-08-04 10:00:06.000000 flask_unity-0.0.1/flask_unity/api.py
--rw-rw-r--   0 usman     (1000) usman     (1000)    12807 2023-08-04 10:00:06.000000 flask_unity-0.0.1/flask_unity/base.py
--rw-rw-r--   0 usman     (1000) usman     (1000)     3278 2023-08-05 07:14:26.000000 flask_unity-0.0.1/flask_unity/dummy.py
--rw-rw-r--   0 usman     (1000) usman     (1000)      203 2023-08-04 10:00:06.000000 flask_unity-0.0.1/flask_unity/utils.py
-drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-08-05 18:39:27.468060 flask_unity-0.0.1/flask_unity.egg-info/
--rw-rw-r--   0 usman     (1000) usman     (1000)     3366 2023-08-05 18:39:25.000000 flask_unity-0.0.1/flask_unity.egg-info/PKG-INFO
--rw-rw-r--   0 usman     (1000) usman     (1000)      335 2023-08-05 18:39:26.000000 flask_unity-0.0.1/flask_unity.egg-info/SOURCES.txt
--rw-rw-r--   0 usman     (1000) usman     (1000)        1 2023-08-05 18:39:25.000000 flask_unity-0.0.1/flask_unity.egg-info/dependency_links.txt
--rw-rw-r--   0 usman     (1000) usman     (1000)        6 2023-08-05 18:39:25.000000 flask_unity-0.0.1/flask_unity.egg-info/requires.txt
--rw-rw-r--   0 usman     (1000) usman     (1000)       12 2023-08-05 18:39:25.000000 flask_unity-0.0.1/flask_unity.egg-info/top_level.txt
--rw-rw-r--   0 usman     (1000) usman     (1000)       38 2023-08-05 18:39:27.492060 flask_unity-0.0.1/setup.cfg
--rw-rw-r--   0 usman     (1000) usman     (1000)     1682 2023-08-05 07:17:43.000000 flask_unity-0.0.1/setup.py
--rw-rw-r--   0 usman     (1000) usman     (1000)       94 2023-08-04 11:27:57.000000 flask_unity-0.0.1/test.py
+drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-08-06 07:34:08.685383 flask_unity-0.0.2/
+-rw-rw-r--   0 usman     (1000) usman     (1000)      659 2023-08-06 06:45:35.000000 flask_unity-0.0.2/CHANGELOG
+-rw-rw-r--   0 usman     (1000) usman     (1000)     1077 2023-08-05 06:53:20.000000 flask_unity-0.0.2/LICENSE
+-rw-rw-r--   0 usman     (1000) usman     (1000)       82 2023-08-06 06:39:07.000000 flask_unity-0.0.2/MANIFEST.in
+-rw-rw-r--   0 usman     (1000) usman     (1000)     6487 2023-08-06 07:34:08.669406 flask_unity-0.0.2/PKG-INFO
+-rw-rw-r--   0 usman     (1000) usman     (1000)     4907 2023-08-06 06:47:11.000000 flask_unity-0.0.2/README.md
+drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-08-06 07:34:08.589523 flask_unity-0.0.2/flask_unity/
+-rw-rw-r--   0 usman     (1000) usman     (1000)      894 2023-08-06 06:48:02.000000 flask_unity-0.0.2/flask_unity/__init__.py
+-rw-rw-r--   0 usman     (1000) usman     (1000)      489 2023-08-06 06:39:07.000000 flask_unity-0.0.2/flask_unity/api.py
+-rw-rw-r--   0 usman     (1000) usman     (1000)    18599 2023-08-06 06:49:41.000000 flask_unity-0.0.2/flask_unity/base.py
+-rw-rw-r--   0 usman     (1000) usman     (1000)     2937 2023-08-06 06:49:28.000000 flask_unity-0.0.2/flask_unity/blueprint.py
+drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-08-06 07:34:08.605500 flask_unity-0.0.2/flask_unity/mute/
+-rw-rw-r--   0 usman     (1000) usman     (1000)      595 2023-08-06 06:52:28.000000 flask_unity-0.0.2/flask_unity/mute/__init__.py
+-rw-rw-r--   0 usman     (1000) usman     (1000)     6815 2023-08-06 06:52:53.000000 flask_unity-0.0.2/flask_unity/mute/app.py
+-rw-rw-r--   0 usman     (1000) usman     (1000)     5991 2023-08-06 06:53:35.000000 flask_unity-0.0.2/flask_unity/mute/auth.py
+-rw-rw-r--   0 usman     (1000) usman     (1000)     2862 2023-08-06 06:54:14.000000 flask_unity-0.0.2/flask_unity/mute/page.py
+-rw-rw-r--   0 usman     (1000) usman     (1000)     4293 2023-08-06 06:54:29.000000 flask_unity-0.0.2/flask_unity/mute/project.py
+drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-08-06 07:34:08.549582 flask_unity-0.0.2/flask_unity/static/
+drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-08-06 07:34:08.553576 flask_unity-0.0.2/flask_unity/static/default_style/
+drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-08-06 07:34:08.605500 flask_unity-0.0.2/flask_unity/static/default_style/css/
+-rw-rw-r--   0 usman     (1000) usman     (1000)     5806 2023-08-06 06:39:07.000000 flask_unity-0.0.2/flask_unity/static/default_style/css/style.css
+drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-08-06 07:34:08.609494 flask_unity-0.0.2/flask_unity/static/default_style/js/
+-rw-rw-r--   0 usman     (1000) usman     (1000)      131 2023-08-06 06:52:10.000000 flask_unity-0.0.2/flask_unity/static/default_style/js/index.js
+drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-08-06 07:34:08.609494 flask_unity-0.0.2/flask_unity/static/default_style/media/
+-rw-rw-r--   0 usman     (1000) usman     (1000)     3767 2023-08-06 06:39:07.000000 flask_unity-0.0.2/flask_unity/static/default_style/media/alert.png
+-rw-rw-r--   0 usman     (1000) usman     (1000)     3767 2023-08-06 06:39:07.000000 flask_unity-0.0.2/flask_unity/static/default_style/media/favicon.ico
+drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-08-06 07:34:08.557570 flask_unity-0.0.2/flask_unity/templates/
+drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-08-06 07:34:08.645441 flask_unity-0.0.2/flask_unity/templates/default_errors/
+-rw-rw-r--   0 usman     (1000) usman     (1000)      152 2023-08-06 06:39:07.000000 flask_unity-0.0.2/flask_unity/templates/default_errors/400.html
+-rw-rw-r--   0 usman     (1000) usman     (1000)      142 2023-08-06 06:39:07.000000 flask_unity-0.0.2/flask_unity/templates/default_errors/401.html
+-rw-rw-r--   0 usman     (1000) usman     (1000)      139 2023-08-06 06:39:07.000000 flask_unity-0.0.2/flask_unity/templates/default_errors/403.html
+-rw-rw-r--   0 usman     (1000) usman     (1000)      139 2023-08-06 06:39:07.000000 flask_unity-0.0.2/flask_unity/templates/default_errors/404.html
+-rw-rw-r--   0 usman     (1000) usman     (1000)      149 2023-08-06 06:39:07.000000 flask_unity-0.0.2/flask_unity/templates/default_errors/406.html
+-rw-rw-r--   0 usman     (1000) usman     (1000)      191 2023-08-06 06:39:07.000000 flask_unity-0.0.2/flask_unity/templates/default_errors/415.html
+-rw-rw-r--   0 usman     (1000) usman     (1000)      163 2023-08-06 06:39:07.000000 flask_unity-0.0.2/flask_unity/templates/default_errors/429.html
+-rw-rw-r--   0 usman     (1000) usman     (1000)      151 2023-08-06 06:39:07.000000 flask_unity-0.0.2/flask_unity/templates/default_errors/500.html
+-rw-rw-r--   0 usman     (1000) usman     (1000)      151 2023-08-06 06:39:07.000000 flask_unity-0.0.2/flask_unity/templates/default_errors/501.html
+-rw-rw-r--   0 usman     (1000) usman     (1000)      147 2023-08-06 06:39:07.000000 flask_unity-0.0.2/flask_unity/templates/default_errors/502.html
+-rw-rw-r--   0 usman     (1000) usman     (1000)      169 2023-08-06 06:39:07.000000 flask_unity-0.0.2/flask_unity/templates/default_errors/503.html
+-rw-rw-r--   0 usman     (1000) usman     (1000)      151 2023-08-06 06:39:07.000000 flask_unity-0.0.2/flask_unity/templates/default_errors/504.html
+drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-08-06 07:34:08.649436 flask_unity-0.0.2/flask_unity/templates/default_page/
+-rw-rw-r--   0 usman     (1000) usman     (1000)      426 2023-08-06 06:39:07.000000 flask_unity-0.0.2/flask_unity/templates/default_page/admin_login.html
+-rw-rw-r--   0 usman     (1000) usman     (1000)      512 2023-08-06 06:39:07.000000 flask_unity-0.0.2/flask_unity/templates/default_page/admin_register.html
+-rw-rw-r--   0 usman     (1000) usman     (1000)     1082 2023-08-06 06:39:07.000000 flask_unity-0.0.2/flask_unity/templates/default_page/default_base.html
+-rw-rw-r--   0 usman     (1000) usman     (1000)     3157 2023-08-06 07:13:47.000000 flask_unity-0.0.2/flask_unity/templates/default_page/default_index.html
+-rw-rw-r--   0 usman     (1000) usman     (1000)    11433 2023-08-06 06:49:07.000000 flask_unity-0.0.2/flask_unity/utils.py
+drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-08-06 07:34:08.597512 flask_unity-0.0.2/flask_unity.egg-info/
+-rw-rw-r--   0 usman     (1000) usman     (1000)     6487 2023-08-06 07:34:07.000000 flask_unity-0.0.2/flask_unity.egg-info/PKG-INFO
+-rw-rw-r--   0 usman     (1000) usman     (1000)     1437 2023-08-06 07:34:08.000000 flask_unity-0.0.2/flask_unity.egg-info/SOURCES.txt
+-rw-rw-r--   0 usman     (1000) usman     (1000)        1 2023-08-06 07:34:07.000000 flask_unity-0.0.2/flask_unity.egg-info/dependency_links.txt
+-rw-rw-r--   0 usman     (1000) usman     (1000)      287 2023-08-06 07:34:07.000000 flask_unity-0.0.2/flask_unity.egg-info/requires.txt
+-rw-rw-r--   0 usman     (1000) usman     (1000)       12 2023-08-06 07:34:07.000000 flask_unity-0.0.2/flask_unity.egg-info/top_level.txt
+-rw-rw-r--   0 usman     (1000) usman     (1000)      287 2023-08-06 06:39:07.000000 flask_unity-0.0.2/requirements.txt
+-rw-rw-r--   0 usman     (1000) usman     (1000)       38 2023-08-06 07:34:08.685383 flask_unity-0.0.2/setup.cfg
+-rw-rw-r--   0 usman     (1000) usman     (1000)     2267 2023-08-06 07:33:29.000000 flask_unity-0.0.2/setup.py
```

### Comparing `flask_unity-0.0.1/LICENSE` & `flask_unity-0.0.2/LICENSE`

 * *Files identical despite different names*

