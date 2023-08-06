# Comparing `tmp/yeref-0.2.8.tar.gz` & `tmp/yeref-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeref-0.2.8.tar", last modified: Sun Jun 25 10:12:02 2023, max compression
+gzip compressed data, was "yeref-0.2.9.tar", last modified: Sun Jun 25 10:28:31 2023, max compression
```

## Comparing `yeref-0.2.8.tar` & `yeref-0.2.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-25 10:12:02.778665 yeref-0.2.8/
--rw-r--r--   0 mark       (501) staff       (20)       84 2023-06-25 10:12:02.778916 yeref-0.2.8/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-06-25 10:12:02.779823 yeref-0.2.8/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1390 2023-06-25 10:11:22.000000 yeref-0.2.8/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-25 10:12:02.765372 yeref-0.2.8/yeref/
--rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.2.8/yeref/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)   558219 2023-06-25 10:11:22.000000 yeref-0.2.8/yeref/l_.py
--rw-r--r--   0 mark       (501) staff       (20)   211219 2023-06-23 18:30:42.000000 yeref-0.2.8/yeref/yeref.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-25 10:12:02.777309 yeref-0.2.8/yeref.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)       84 2023-06-25 10:12:02.000000 yeref-0.2.8/yeref.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      179 2023-06-25 10:12:02.000000 yeref-0.2.8/yeref.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-06-25 10:12:02.000000 yeref-0.2.8/yeref.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        6 2023-06-25 10:12:02.000000 yeref-0.2.8/yeref.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-25 10:28:31.658668 yeref-0.2.9/
+-rw-r--r--   0 mark       (501) staff       (20)       84 2023-06-25 10:28:31.658912 yeref-0.2.9/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-06-25 10:28:31.659829 yeref-0.2.9/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     1390 2023-06-25 10:28:13.000000 yeref-0.2.9/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-25 10:28:31.652441 yeref-0.2.9/yeref/
+-rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.2.9/yeref/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)   558205 2023-06-25 10:27:43.000000 yeref-0.2.9/yeref/l_.py
+-rw-r--r--   0 mark       (501) staff       (20)   211219 2023-06-23 18:30:42.000000 yeref-0.2.9/yeref/yeref.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-25 10:28:31.657998 yeref-0.2.9/yeref.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)       84 2023-06-25 10:28:31.000000 yeref-0.2.9/yeref.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      179 2023-06-25 10:28:31.000000 yeref-0.2.9/yeref.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-06-25 10:28:31.000000 yeref-0.2.9/yeref.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        6 2023-06-25 10:28:31.000000 yeref-0.2.9/yeref.egg-info/top_level.txt
```

### Comparing `yeref-0.2.8/setup.py` & `yeref-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
       name='yeref',
-      version='0.2.08',
+      version='0.2.09',
       description='desc-f',
       author='john smith',
       packages=['yeref'],
       # install_requires=[
       #       "httplib2>=0.20.4",
       #       "moviepy>=1.0.3",
       #       "Pillow>=9.2.0",
```

### Comparing `yeref-0.2.8/yeref/l_.py` & `yeref-0.2.9/yeref/l_.py`

 * *Files 0% similar despite different names*

```diff
@@ -453,15 +453,15 @@
     'en': "✅ User <b>{0}</b> (username={1}, id= {2} ) <i>clicked</i> on [<b>{3}</b>] in post # <u>{4}</u>",
     'es': "✅ El usuario <b>{0}</b> (username={1}, id= {2} ) <i>hizo clic</i> en [<b>{3}</b>] en la publicación n.º <u>{4}</u>",
     'fr': "✅ L'utilisateur <b>{0}</b> (username={1}, id= {2} ) <i>a cliqué</i> sur [<b>{3}</b>] dans le post # <u>{4}</u>",
     'zh': "✅ 用户<b>{0}</b> （用户名 = {1}，id = {2} ）在帖子 # <u>{4}</u>中<i>点击了</i>[<b>{3}</b>]",
     'ar': "✅ المستخدم <b>{0}</b> (اسم المستخدم = {1} ، المعرف = {2} ) <i>نقر</i> على [<b>{3}</b>] في المشاركة رقم <u>{4}</u>",
 }
 l_post_datetime = {
-    'ru': "<b>Дата публикации</b>",
+    'ru': "<b>Дата</b>",
     'en': "<b>Publication date</b>",
     'es': "<b>Fecha de publicación</b>",
     'fr': "<b>Date de publication</b>",
     'zh': "<b>发布日期</b>",
     'ar': "<b>تاريخ النشر</b>",
 }
 l_post_preview = {
@@ -607,15 +607,15 @@
     'en': "📍 Location <b>time zone</b> set\n\n🕐 <b>Current</b> time: <u>{0}</u> ({1}{2} GMT)",
     'es': "📍 Configuración <b>de la zona horaria</b> de la ubicación\n\n🕐 Hora <b>actual</b> : <u>{0}</u> ({1}{2} GMT)",
     'fr': "📍 <b>Fuseau horaire</b> de l&#x27;emplacement défini\n\n🕐 Heure <b>actuelle</b> : <u>{0}</u> ({1}{2} GMT)",
     'zh': "📍 位置<b>时区</b>设置\n\n🕐<b>当前</b>时间： <u>{0}</u> （{1}{2} GMT）",
     'ar': "📍 تعيين <b>المنطقة الزمنية</b> للموقع\n\n🕐 الوقت <b>الحالي</b> : <u>{0}</u> ({1} {2} GMT)",
 }
 l_post_time_future = {
-    'ru': "🕒 Укажи время в будущем",
+    'ru': "🕒 <b>Укажи</b> время в будущем",
     'en': "🕒 Set time in the future",
     'es': "🕒 Establecer tiempo en el futuro",
     'fr': "🕒 Réglez l'heure dans le futur",
     'zh': "🕒 设定未来的时间",
     'ar': "🕒 حدد الوقت في المستقبل",
 }
 l_me = {
```

### Comparing `yeref-0.2.8/yeref/yeref.py` & `yeref-0.2.9/yeref/yeref.py`

 * *Files identical despite different names*

