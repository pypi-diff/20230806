# Comparing `tmp/CaptchaGenerator-1.1.4.tar.gz` & `tmp/CaptchaGenerator-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CaptchaGenerator-1.1.4.tar", last modified: Fri Aug  4 15:59:18 2023, max compression
+gzip compressed data, was "CaptchaGenerator-1.1.5.tar", last modified: Sat Aug  5 22:04:13 2023, max compression
```

## Comparing `CaptchaGenerator-1.1.4.tar` & `CaptchaGenerator-1.1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 rar4      (1000) rar4      (1000)        0 2023-08-04 15:59:18.511183 CaptchaGenerator-1.1.4/
-drwxr-xr-x   0 rar4      (1000) rar4      (1000)        0 2023-08-04 15:59:18.503033 CaptchaGenerator-1.1.4/CaptchaGenerator/
--rw-r--r--   0 rar4      (1000) rar4      (1000)     6927 2023-08-04 13:38:22.000000 CaptchaGenerator-1.1.4/CaptchaGenerator/CaptchaGenerator.py
--rw-r--r--   0 rar4      (1000) rar4      (1000)     2046 2023-08-04 15:29:26.000000 CaptchaGenerator-1.1.4/CaptchaGenerator/__main__.py
-drwxr-xr-x   0 rar4      (1000) rar4      (1000)        0 2023-08-04 15:59:18.511183 CaptchaGenerator-1.1.4/CaptchaGenerator.egg-info/
--rw-r--r--   0 rar4      (1000) rar4      (1000)      375 2023-08-04 15:59:18.000000 CaptchaGenerator-1.1.4/CaptchaGenerator.egg-info/PKG-INFO
--rw-r--r--   0 rar4      (1000) rar4      (1000)      293 2023-08-04 15:59:18.000000 CaptchaGenerator-1.1.4/CaptchaGenerator.egg-info/SOURCES.txt
--rw-r--r--   0 rar4      (1000) rar4      (1000)        1 2023-08-04 15:59:18.000000 CaptchaGenerator-1.1.4/CaptchaGenerator.egg-info/dependency_links.txt
--rw-r--r--   0 rar4      (1000) rar4      (1000)       16 2023-08-04 15:59:18.000000 CaptchaGenerator-1.1.4/CaptchaGenerator.egg-info/requires.txt
--rw-r--r--   0 rar4      (1000) rar4      (1000)       17 2023-08-04 15:59:18.000000 CaptchaGenerator-1.1.4/CaptchaGenerator.egg-info/top_level.txt
--rw-r--r--   0 rar4      (1000) rar4      (1000)      375 2023-08-04 15:59:18.512175 CaptchaGenerator-1.1.4/PKG-INFO
--rw-r--r--   0 rar4      (1000) rar4      (1000)      101 2023-08-04 15:56:54.000000 CaptchaGenerator-1.1.4/README.md
--rw-r--r--   0 rar4      (1000) rar4      (1000)       79 2023-08-04 15:59:18.512175 CaptchaGenerator-1.1.4/setup.cfg
--rw-r--r--   0 rar4      (1000) rar4      (1000)      556 2023-08-04 15:57:42.000000 CaptchaGenerator-1.1.4/setup.py
+drwxr-xr-x   0 rar4      (1000) rar4      (1000)        0 2023-08-05 22:04:13.439669 CaptchaGenerator-1.1.5/
+drwxr-xr-x   0 rar4      (1000) rar4      (1000)        0 2023-08-05 22:04:13.432692 CaptchaGenerator-1.1.5/CaptchaGenerator/
+-rw-r--r--   0 rar4      (1000) rar4      (1000)    12660 2023-08-05 18:20:55.000000 CaptchaGenerator-1.1.5/CaptchaGenerator/CaptchaGenerator.py
+-rw-r--r--   0 rar4      (1000) rar4      (1000)     2592 2023-08-05 21:46:23.000000 CaptchaGenerator-1.1.5/CaptchaGenerator/TelegramBotVersion.py
+drwxr-xr-x   0 rar4      (1000) rar4      (1000)        0 2023-08-05 22:04:13.439669 CaptchaGenerator-1.1.5/CaptchaGenerator.egg-info/
+-rw-r--r--   0 rar4      (1000) rar4      (1000)      377 2023-08-05 22:04:13.000000 CaptchaGenerator-1.1.5/CaptchaGenerator.egg-info/PKG-INFO
+-rw-r--r--   0 rar4      (1000) rar4      (1000)      303 2023-08-05 22:04:13.000000 CaptchaGenerator-1.1.5/CaptchaGenerator.egg-info/SOURCES.txt
+-rw-r--r--   0 rar4      (1000) rar4      (1000)        1 2023-08-05 22:04:13.000000 CaptchaGenerator-1.1.5/CaptchaGenerator.egg-info/dependency_links.txt
+-rw-r--r--   0 rar4      (1000) rar4      (1000)       16 2023-08-05 22:04:13.000000 CaptchaGenerator-1.1.5/CaptchaGenerator.egg-info/requires.txt
+-rw-r--r--   0 rar4      (1000) rar4      (1000)       17 2023-08-05 22:04:13.000000 CaptchaGenerator-1.1.5/CaptchaGenerator.egg-info/top_level.txt
+-rw-r--r--   0 rar4      (1000) rar4      (1000)      377 2023-08-05 22:04:13.440661 CaptchaGenerator-1.1.5/PKG-INFO
+-rw-r--r--   0 rar4      (1000) rar4      (1000)      101 2023-08-05 22:03:57.000000 CaptchaGenerator-1.1.5/README.md
+-rw-r--r--   0 rar4      (1000) rar4      (1000)       79 2023-08-05 22:04:13.440661 CaptchaGenerator-1.1.5/setup.cfg
+-rw-r--r--   0 rar4      (1000) rar4      (1000)      558 2023-08-05 22:03:53.000000 CaptchaGenerator-1.1.5/setup.py
```

### Comparing `CaptchaGenerator-1.1.4/setup.py` & `CaptchaGenerator-1.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup
 
 setup(
     long_description = """
-    <a href="https://github.com/Sepehr0Day/CaptchaGenerator/">You can see library info in my github</a>'
+    # <a href="https://github.com/Sepehr0Day/CaptchaGenerator/">You can see library info in my github</a>'
     """,
     long_description_content_type = "text/markdown",
     name='CaptchaGenerator',
-    version='1.1.4',
+    version='1.1.5',
     license='MIT',
     description='A library for captcha generator for Telegram bots',
     author='Sepehr0Day',
     author_email='sphrz2324@gmail.com',
     packages=['CaptchaGenerator'],
     install_requires=[
         'Pillow',
```

#### html2text {}

```diff
@@ -1,6 +1,6 @@
-from setuptools import setup setup( long_description = """ You_can_see_library
-info_in_my_github' """, long_description_content_type = "text/markdown",
-name='CaptchaGenerator', version='1.1.4', license='MIT', description='A library
-for captcha generator for Telegram bots', author='Sepehr0Day',
-author_email='sphrz2324@gmail.com', packages=['CaptchaGenerator'],
-install_requires=[ 'Pillow', 'colorama', ], )
+from setuptools import setup setup( long_description = """ # You_can_see
+library_info_in_my_github' """, long_description_content_type = "text/
+markdown", name='CaptchaGenerator', version='1.1.5', license='MIT',
+description='A library for captcha generator for Telegram bots',
+author='Sepehr0Day', author_email='sphrz2324@gmail.com', packages=
+['CaptchaGenerator'], install_requires=[ 'Pillow', 'colorama', ], )
```

