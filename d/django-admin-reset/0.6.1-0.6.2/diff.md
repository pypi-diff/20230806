# Comparing `tmp/django_admin_reset-0.6.1-py2.py3-none-any.whl.zip` & `tmp/django_admin_reset-0.6.2-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 9153 bytes, number of entries: 12
--rw-r--r--  2.0 unx       22 b- defN 23-Apr-02 17:10 django_admin_reset/__init__.py
--rw-r--r--  2.0 unx     5998 b- defN 23-Apr-02 17:10 django_admin_reset/admin.py
--rw-r--r--  2.0 unx     1803 b- defN 23-Apr-02 17:11 django_admin_reset/locale/hu/LC_MESSAGES/django.mo
--rw-r--r--  2.0 unx     2040 b- defN 23-Apr-02 17:10 django_admin_reset/locale/hu/LC_MESSAGES/django.po
--rw-r--r--  2.0 unx      317 b- defN 23-Apr-02 17:10 django_admin_reset/templates/admin/add_user_form.html
--rw-r--r--  2.0 unx      264 b- defN 23-Apr-02 17:10 django_admin_reset/templates/admin/change_user.html
--rw-r--r--  2.0 unx      539 b- defN 23-Apr-02 17:10 django_admin_reset/templates/admin/password_reset_url.html
--rw-r--r--  2.0 unx     1476 b- defN 23-Apr-02 17:11 django_admin_reset-0.6.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     2527 b- defN 23-Apr-02 17:11 django_admin_reset-0.6.1.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Apr-02 17:11 django_admin_reset-0.6.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       19 b- defN 23-Apr-02 17:11 django_admin_reset-0.6.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1155 b- defN 23-Apr-02 17:11 django_admin_reset-0.6.1.dist-info/RECORD
-12 files, 16270 bytes uncompressed, 7153 bytes compressed:  56.0%
+Zip file size: 9158 bytes, number of entries: 12
+-rw-r--r--  2.0 unx       22 b- defN 23-Jun-04 20:17 django_admin_reset/__init__.py
+-rw-r--r--  2.0 unx     5998 b- defN 23-Jun-04 20:17 django_admin_reset/admin.py
+-rw-r--r--  2.0 unx     1803 b- defN 23-Jun-04 20:19 django_admin_reset/locale/hu/LC_MESSAGES/django.mo
+-rw-r--r--  2.0 unx     2040 b- defN 23-Jun-04 20:17 django_admin_reset/locale/hu/LC_MESSAGES/django.po
+-rw-r--r--  2.0 unx      317 b- defN 23-Jun-04 20:17 django_admin_reset/templates/admin/add_user_form.html
+-rw-r--r--  2.0 unx      264 b- defN 23-Jun-04 20:17 django_admin_reset/templates/admin/change_user.html
+-rw-r--r--  2.0 unx      539 b- defN 23-Jun-04 20:17 django_admin_reset/templates/admin/password_reset_url.html
+-rw-r--r--  2.0 unx     1476 b- defN 23-Jun-04 20:19 django_admin_reset-0.6.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2564 b- defN 23-Jun-04 20:19 django_admin_reset-0.6.2.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jun-04 20:19 django_admin_reset-0.6.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       19 b- defN 23-Jun-04 20:19 django_admin_reset-0.6.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1155 b- defN 23-Jun-04 20:19 django_admin_reset-0.6.2.dist-info/RECORD
+12 files, 16307 bytes uncompressed, 7158 bytes compressed:  56.1%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: django_admin_reset/templates/admin/change_user.html
 Comment: 
 
 Filename: django_admin_reset/templates/admin/password_reset_url.html
 Comment: 
 
-Filename: django_admin_reset-0.6.1.dist-info/LICENSE
+Filename: django_admin_reset-0.6.2.dist-info/LICENSE
 Comment: 
 
-Filename: django_admin_reset-0.6.1.dist-info/METADATA
+Filename: django_admin_reset-0.6.2.dist-info/METADATA
 Comment: 
 
-Filename: django_admin_reset-0.6.1.dist-info/WHEEL
+Filename: django_admin_reset-0.6.2.dist-info/WHEEL
 Comment: 
 
-Filename: django_admin_reset-0.6.1.dist-info/top_level.txt
+Filename: django_admin_reset-0.6.2.dist-info/top_level.txt
 Comment: 
 
-Filename: django_admin_reset-0.6.1.dist-info/RECORD
+Filename: django_admin_reset-0.6.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## django_admin_reset/__init__.py

```diff
@@ -1 +1 @@
-__version__ = '0.6.1'
+__version__ = '0.6.2'
```

## Comparing `django_admin_reset-0.6.1.dist-info/LICENSE` & `django_admin_reset-0.6.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `django_admin_reset-0.6.1.dist-info/METADATA` & `django_admin_reset-0.6.2.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: django-admin-reset
-Version: 0.6.1
+Version: 0.6.2
 Summary: Django admin password reset
 Home-page: https://github.com/tiborhari/django-admin-reset/
 Author: Tibor Hári
 Author-email: hartib@gmail.com
 Requires-Python: >=3.6, <4
 License-File: LICENSE
-Requires-Dist: django (<4.2,>=3.2)
+Requires-Dist: django (<4.3,>=3.2)
 Provides-Extra: babel
 Requires-Dist: babel (~=2.10.1) ; extra == 'babel'
 Provides-Extra: docs
 Requires-Dist: sphinx (~=4.5.0) ; extra == 'docs'
 Requires-Dist: sphinx-rtd-theme (~=1.0.0) ; extra == 'docs'
 Provides-Extra: testing
 Requires-Dist: flake8 (~=5.0.4) ; extra == 'testing'
@@ -77,8 +77,9 @@
 
 ==============  ========================
 Django version  Python versions
 ==============  ========================
 3.2 LTS         3.6, 3.7, 3.8, 3.9, 3.10
 4.0             3.8, 3.9, 3.10
 4.1             3.8, 3.9, 3.10, 3.11
+4.2             3.8, 3.9, 3.10, 3.11
 ==============  ========================
```

## Comparing `django_admin_reset-0.6.1.dist-info/RECORD` & `django_admin_reset-0.6.2.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-django_admin_reset/__init__.py,sha256=gd3s3RotD0_KL90Tua-YkOr60Jm2C2_wvlEhAT08068,22
+django_admin_reset/__init__.py,sha256=gMDttCkJF3h8Jr3eq_8NuJj26-9xyjg-YjR2bSNcGxM,22
 django_admin_reset/admin.py,sha256=jrCZc8bDYbhK0e15PLRWJZ_YGzrPlIWVxobBD7cNMNw,5998
 django_admin_reset/locale/hu/LC_MESSAGES/django.mo,sha256=FRzr8VtdKacHFyzQ-FaZwdXXglWv4F0p1_M0UFkl_YQ,1803
 django_admin_reset/locale/hu/LC_MESSAGES/django.po,sha256=JItR1wH5wZQqqKRmmJt_VFnsbBzgKbMzUXknHqYxMHI,2040
 django_admin_reset/templates/admin/add_user_form.html,sha256=tgdIIpA2zvlxs38lMvEZBCm4hsMiHPPpwMWQ73KMcjo,317
 django_admin_reset/templates/admin/change_user.html,sha256=9HqSy-1Elm2j2P6VWCJzuiPokrKNIyTmNdOVjSKXQHU,264
 django_admin_reset/templates/admin/password_reset_url.html,sha256=74CkgdwDuZHxNJpXPJyzBErlRqgkNIrKkBvdSU6i81Q,539
-django_admin_reset-0.6.1.dist-info/LICENSE,sha256=HUeCDOHFhxmzf_23dAKJJ5KOcMMLnnod30PvvTG9R_A,1476
-django_admin_reset-0.6.1.dist-info/METADATA,sha256=MbY-mMLU8a3XfGPNhESklDsfM1s0R9YdXzlbDFUCj9E,2527
-django_admin_reset-0.6.1.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-django_admin_reset-0.6.1.dist-info/top_level.txt,sha256=Ccyn6m1bbjFU-uqeAgvw8FwXpKY1q0pj1MB-LTXAPKU,19
-django_admin_reset-0.6.1.dist-info/RECORD,,
+django_admin_reset-0.6.2.dist-info/LICENSE,sha256=HUeCDOHFhxmzf_23dAKJJ5KOcMMLnnod30PvvTG9R_A,1476
+django_admin_reset-0.6.2.dist-info/METADATA,sha256=5bZbQOs9EsdiLtcaryYcEYEHwFrtfH_Vqa3vZazvrNM,2564
+django_admin_reset-0.6.2.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+django_admin_reset-0.6.2.dist-info/top_level.txt,sha256=Ccyn6m1bbjFU-uqeAgvw8FwXpKY1q0pj1MB-LTXAPKU,19
+django_admin_reset-0.6.2.dist-info/RECORD,,
```

