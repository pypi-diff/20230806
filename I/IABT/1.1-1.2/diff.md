# Comparing `tmp/IABT-1.1.tar.gz` & `tmp/IABT-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\IABT-1.1.tar", last modified: Sun Aug  6 02:38:23 2023, max compression
+gzip compressed data, was "dist\IABT-1.2.tar", last modified: Sun Aug  6 02:47:11 2023, max compression
```

## Comparing `IABT-1.1.tar` & `IABT-1.2.tar`

### file list

```diff
@@ -1,111 +1,105 @@
-drwxrwxrwx   0        0        0        0 2023-08-06 02:38:23.000000 IABT-1.1/
-drwxrwxrwx   0        0        0        0 2023-08-06 02:38:23.000000 IABT-1.1/IABT/
--rw-rw-rw-   0        0        0      127 2023-08-05 03:44:22.000000 IABT-1.1/IABT/InxioManifest.vsp
--rw-rw-rw-   0        0        0        0 2023-08-05 05:18:55.000000 IABT-1.1/IABT/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-06 02:38:23.000000 IABT-1.1/IABT/__pycache__/
--rw-rw-rw-   0        0        0     9229 2023-08-06 02:11:47.000000 IABT-1.1/IABT/__pycache__/build.cpython-38.pyc
--rw-rw-rw-   0        0        0     3980 2023-08-06 02:11:47.000000 IABT-1.1/IABT/__pycache__/file_control.cpython-38.pyc
--rw-rw-rw-   0        0        0     1042 2023-08-06 02:11:47.000000 IABT-1.1/IABT/__pycache__/generate_path.cpython-38.pyc
--rw-rw-rw-   0        0        0     1396 2023-08-06 02:11:47.000000 IABT-1.1/IABT/__pycache__/json_control.cpython-38.pyc
--rw-rw-rw-   0        0        0    11709 2023-08-05 03:44:22.000000 IABT-1.1/IABT/build.py
-drwxrwxrwx   0        0        0        0 2023-08-06 02:38:23.000000 IABT-1.1/IABT/data/
--rw-rw-rw-   0        0        0     7825 2023-07-30 10:25:48.000000 IABT-1.1/IABT/data/EventActivity.java
--rw-rw-rw-   0        0        0     6236 2023-07-23 07:40:17.000000 IABT-1.1/IABT/data/FormalActivity.java
--rw-rw-rw-   0        0        0     8430 2023-07-30 10:25:48.000000 IABT-1.1/IABT/data/PermissionActivity.java
--rw-rw-rw-   0        0        0      126 2023-07-30 10:25:48.000000 IABT-1.1/IABT/data/VDialogInterface.java
--rw-rw-rw-   0        0        0      134 2023-07-30 10:25:48.000000 IABT-1.1/IABT/data/VLocationListener.java
--rw-rw-rw-   0        0        0      134 2023-07-30 10:25:48.000000 IABT-1.1/IABT/data/VOnClickListener.java
--rw-rw-rw-   0        0        0      147 2023-07-30 10:25:48.000000 IABT-1.1/IABT/data/VSensorEventListener.java
--rw-rw-rw-   0        0        0     2078 2023-08-05 04:02:38.000000 IABT-1.1/IABT/data/app_build.gradle
--rw-rw-rw-   0        0        0      290 2023-07-30 15:14:52.000000 IABT-1.1/IABT/data/project_build.gradle
--rw-rw-rw-   0        0        0     4848 2023-08-05 03:47:28.000000 IABT-1.1/IABT/file_control.py
--rw-rw-rw-   0        0        0      773 2023-07-31 01:59:57.000000 IABT-1.1/IABT/generate_path.py
--rw-rw-rw-   0        0        0    15919 2023-08-06 02:38:09.000000 IABT-1.1/IABT/iabt.py
-drwxrwxrwx   0        0        0        0 2023-08-06 02:38:23.000000 IABT-1.1/IABT/inxio_core/
-drwxrwxrwx   0        0        0        0 2023-08-06 02:38:23.000000 IABT-1.1/IABT/inxio_core/Inxio/
--rw-rw-rw-   0        0        0        0 2023-06-06 07:24:07.000000 IABT-1.1/IABT/inxio_core/Inxio/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-06 02:38:23.000000 IABT-1.1/IABT/inxio_core/Inxio/android/
-drwxrwxrwx   0        0        0        0 2023-08-06 02:38:23.000000 IABT-1.1/IABT/inxio_core/Inxio/android/APP/
--rw-rw-rw-   0        0        0        0 2023-05-21 04:19:19.000000 IABT-1.1/IABT/inxio_core/Inxio/android/APP/__init__.py
--rw-rw-rw-   0        0        0     6720 2023-08-05 04:50:57.000000 IABT-1.1/IABT/inxio_core/Inxio/android/APP/app.py
--rw-rw-rw-   0        0        0    15752 2023-06-08 07:42:03.000000 IABT-1.1/IABT/inxio_core/Inxio/android/APP/permission.py
--rw-rw-rw-   0        0        0        0 2023-05-05 11:40:31.000000 IABT-1.1/IABT/inxio_core/Inxio/android/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-06 02:38:23.000000 IABT-1.1/IABT/inxio_core/Inxio/android/core_components/
--rw-rw-rw-   0        0        0    15598 2023-08-05 03:47:28.000000 IABT-1.1/IABT/inxio_core/Inxio/android/core_components/Activity.py
--rw-rw-rw-   0        0        0     2992 2023-06-06 11:34:29.000000 IABT-1.1/IABT/inxio_core/Inxio/android/core_components/Bundle.py
--rw-rw-rw-   0        0        0     8728 2023-06-08 09:30:34.000000 IABT-1.1/IABT/inxio_core/Inxio/android/core_components/EventProcess.py
--rw-rw-rw-   0        0        0      229 2023-08-05 03:47:28.000000 IABT-1.1/IABT/inxio_core/Inxio/android/core_components/Fragment.py
--rw-rw-rw-   0        0        0      726 2023-08-05 03:47:28.000000 IABT-1.1/IABT/inxio_core/Inxio/android/core_components/Intent.py
--rw-rw-rw-   0        0        0     5451 2023-08-05 03:47:28.000000 IABT-1.1/IABT/inxio_core/Inxio/android/core_components/LocationManager.py
--rw-rw-rw-   0        0        0    12985 2023-08-05 03:47:28.000000 IABT-1.1/IABT/inxio_core/Inxio/android/core_components/NotificationManager.py
--rw-rw-rw-   0        0        0     2368 2023-06-12 08:23:38.000000 IABT-1.1/IABT/inxio_core/Inxio/android/core_components/PendingIntent.py
--rw-rw-rw-   0        0        0     6025 2023-08-05 03:47:28.000000 IABT-1.1/IABT/inxio_core/Inxio/android/core_components/SensorManager.py
--rw-rw-rw-   0        0        0        0 2023-07-01 04:16:08.000000 IABT-1.1/IABT/inxio_core/Inxio/android/core_components/Service.py
--rw-rw-rw-   0        0        0     2064 2023-08-05 03:47:28.000000 IABT-1.1/IABT/inxio_core/Inxio/android/core_components/View.py
--rw-rw-rw-   0        0        0     1994 2023-08-05 03:44:22.000000 IABT-1.1/IABT/inxio_core/Inxio/android/core_components/View_Listeners.py
--rw-rw-rw-   0        0        0     6855 2023-05-06 04:49:08.000000 IABT-1.1/IABT/inxio_core/Inxio/android/core_components/XMLGenerator.py
--rw-rw-rw-   0        0        0        0 2023-05-05 13:58:33.000000 IABT-1.1/IABT/inxio_core/Inxio/android/core_components/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-06 02:38:23.000000 IABT-1.1/IABT/inxio_core/Inxio/android/executable/
--rw-rw-rw-   0        0        0     4716 2023-08-05 03:47:28.000000 IABT-1.1/IABT/inxio_core/Inxio/android/executable/ExecutionBlock.py
--rw-rw-rw-   0        0        0        0 2023-05-21 03:35:13.000000 IABT-1.1/IABT/inxio_core/Inxio/android/executable/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-06 02:38:23.000000 IABT-1.1/IABT/inxio_core/Inxio/android/ui/
-drwxrwxrwx   0        0        0        0 2023-08-06 02:38:23.000000 IABT-1.1/IABT/inxio_core/Inxio/android/ui/Element/
--rw-rw-rw-   0        0        0     1205 2023-08-05 03:47:28.000000 IABT-1.1/IABT/inxio_core/Inxio/android/ui/Element/AlertDialog.py
--rw-rw-rw-   0        0        0     1169 2023-08-05 03:47:28.000000 IABT-1.1/IABT/inxio_core/Inxio/android/ui/Element/Text.py
--rw-rw-rw-   0        0        0      478 2023-05-21 05:27:23.000000 IABT-1.1/IABT/inxio_core/Inxio/android/ui/Element/Toast.py
--rw-rw-rw-   0        0        0        0 2023-05-05 13:59:30.000000 IABT-1.1/IABT/inxio_core/Inxio/android/ui/Element/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-06 02:38:23.000000 IABT-1.1/IABT/inxio_core/Inxio/android/ui/Layout/
--rw-rw-rw-   0        0        0      742 2023-08-05 03:46:48.000000 IABT-1.1/IABT/inxio_core/Inxio/android/ui/Layout/FrameLayout.py
--rw-rw-rw-   0        0        0     1090 2023-08-05 03:47:28.000000 IABT-1.1/IABT/inxio_core/Inxio/android/ui/Layout/GridLayout.py
--rw-rw-rw-   0        0        0     1763 2023-05-06 04:40:15.000000 IABT-1.1/IABT/inxio_core/Inxio/android/ui/Layout/LayoutParams.py
--rw-rw-rw-   0        0        0      926 2023-08-05 03:47:28.000000 IABT-1.1/IABT/inxio_core/Inxio/android/ui/Layout/LinearLayout.py
--rw-rw-rw-   0        0        0      855 2023-08-05 03:47:28.000000 IABT-1.1/IABT/inxio_core/Inxio/android/ui/Layout/RelativeLayout.py
--rw-rw-rw-   0        0        0      707 2023-08-05 03:47:28.000000 IABT-1.1/IABT/inxio_core/Inxio/android/ui/Layout/TableLayout.py
--rw-rw-rw-   0        0        0        0 2023-05-05 13:59:09.000000 IABT-1.1/IABT/inxio_core/Inxio/android/ui/Layout/__init__.py
--rw-rw-rw-   0        0        0        0 2023-05-05 13:58:55.000000 IABT-1.1/IABT/inxio_core/Inxio/android/ui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-06 02:38:23.000000 IABT-1.1/IABT/inxio_core/Inxio/android/vsp/
--rw-rw-rw-   0        0        0    39731 2023-08-05 03:47:28.000000 IABT-1.1/IABT/inxio_core/Inxio/android/vsp/VSPparser.py
--rw-rw-rw-   0        0        0        0 2023-06-04 23:25:11.000000 IABT-1.1/IABT/inxio_core/Inxio/android/vsp/__init__.py
--rw-rw-rw-   0        0        0      327 2023-06-04 23:25:29.000000 IABT-1.1/IABT/inxio_core/Inxio/android/vsp/try.py
--rw-rw-rw-   0        0        0       33 2023-05-28 14:02:07.000000 IABT-1.1/IABT/inxio_core/Inxio/android/vsp/ty.py
--rw-rw-rw-   0        0        0      425 2023-06-04 23:15:22.000000 IABT-1.1/IABT/inxio_core/Inxio/android/vsp/vsp2xml.py
-drwxrwxrwx   0        0        0        0 2023-08-06 02:38:23.000000 IABT-1.1/IABT/inxio_core/Inxio/extends/
--rw-rw-rw-   0        0        0        0 2023-06-10 10:06:44.000000 IABT-1.1/IABT/inxio_core/Inxio/extends/__init__.py
--rw-rw-rw-   0        0        0       67 2023-08-04 05:32:04.000000 IABT-1.1/IABT/inxio_core/Inxio/file_type.py
--rw-rw-rw-   0        0        0       31 2023-08-05 04:00:36.000000 IABT-1.1/IABT/inxio_core/Inxio/global_var.py
-drwxrwxrwx   0        0        0        0 2023-08-06 02:38:23.000000 IABT-1.1/IABT/inxio_core/Inxio/ui_shell/
--rw-rw-rw-   0        0        0      511 2023-08-05 03:47:28.000000 IABT-1.1/IABT/inxio_core/Inxio/ui_shell/Button.py
--rw-rw-rw-   0        0        0        0 2023-08-05 01:52:53.000000 IABT-1.1/IABT/inxio_core/Inxio/ui_shell/__init__.py
--rw-rw-rw-   0        0        0     1285 2023-07-26 06:18:16.000000 IABT-1.1/IABT/json_control.py
-drwxrwxrwx   0        0        0        0 2023-08-06 02:38:23.000000 IABT-1.1/IABT/pretreatment_files/
--rw-rw-rw-   0        0        0    35662 2023-08-04 14:17:54.000000 IABT-1.1/IABT/pretreatment_files/python.jpg
-drwxrwxrwx   0        0        0        0 2023-08-06 02:38:23.000000 IABT-1.1/IABT/translate/
--rw-rw-rw-   0        0        0        0 2023-06-21 14:26:57.000000 IABT-1.1/IABT/translate/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-06 02:38:23.000000 IABT-1.1/IABT/translate/__pycache__/
--rw-rw-rw-   0        0        0      168 2023-08-06 02:11:47.000000 IABT-1.1/IABT/translate/__pycache__/__init__.cpython-38.pyc
--rw-rw-rw-   0        0        0     2674 2023-08-06 02:11:47.000000 IABT-1.1/IABT/translate/__pycache__/translator.cpython-38.pyc
--rw-rw-rw-   0        0        0     4787 2023-08-06 02:11:47.000000 IABT-1.1/IABT/translate/__pycache__/vsp2xml.cpython-38.pyc
--rw-rw-rw-   0        0        0     4911 2023-08-06 02:11:47.000000 IABT-1.1/IABT/translate/__pycache__/xml_generate.cpython-38.pyc
--rw-rw-rw-   0        0        0     2563 2023-08-04 03:39:51.000000 IABT-1.1/IABT/translate/translator.py
--rw-rw-rw-   0        0        0     5303 2023-08-05 03:44:22.000000 IABT-1.1/IABT/translate/vsp2xml.py
--rw-rw-rw-   0        0        0     4463 2023-08-04 09:48:36.000000 IABT-1.1/IABT/translate/xml_generate.py
-drwxrwxrwx   0        0        0        0 2023-08-06 02:38:23.000000 IABT-1.1/IABT/vsp/
--rw-rw-rw-   0        0        0    40003 2023-08-05 03:47:28.000000 IABT-1.1/IABT/vsp/VSPparser.py
--rw-rw-rw-   0        0        0        0 2023-06-04 23:25:11.000000 IABT-1.1/IABT/vsp/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-06 02:38:23.000000 IABT-1.1/IABT/vsp/__pycache__/
--rw-rw-rw-   0        0        0    34678 2023-08-06 02:11:48.000000 IABT-1.1/IABT/vsp/__pycache__/VSPparser.cpython-38.pyc
--rw-rw-rw-   0        0        0      162 2023-08-06 02:11:47.000000 IABT-1.1/IABT/vsp/__pycache__/__init__.cpython-38.pyc
--rw-rw-rw-   0        0        0      327 2023-06-04 23:25:29.000000 IABT-1.1/IABT/vsp/try.py
--rw-rw-rw-   0        0        0       33 2023-05-28 14:02:07.000000 IABT-1.1/IABT/vsp/ty.py
--rw-rw-rw-   0        0        0      425 2023-06-04 23:15:22.000000 IABT-1.1/IABT/vsp/vsp2xml.py
-drwxrwxrwx   0        0        0        0 2023-08-06 02:38:23.000000 IABT-1.1/IABT.egg-info/
--rw-rw-rw-   0        0        0      602 2023-08-06 02:38:23.000000 IABT-1.1/IABT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3523 2023-08-06 02:38:23.000000 IABT-1.1/IABT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-06 02:38:23.000000 IABT-1.1/IABT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-08-06 02:38:23.000000 IABT-1.1/IABT.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-08-06 02:38:23.000000 IABT-1.1/IABT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       26 2023-08-06 01:52:22.000000 IABT-1.1/MANIFEST.in
--rw-rw-rw-   0        0        0      602 2023-08-06 02:38:23.000000 IABT-1.1/PKG-INFO
--rw-rw-rw-   0        0        0      194 2023-08-05 05:21:21.000000 IABT-1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-08-06 02:38:23.000000 IABT-1.1/setup.cfg
--rw-rw-rw-   0        0        0     1440 2023-08-06 02:37:15.000000 IABT-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-06 02:47:11.000000 IABT-1.2/
+drwxrwxrwx   0        0        0        0 2023-08-06 02:47:10.000000 IABT-1.2/IABT/
+-rw-rw-rw-   0        0        0      127 2023-08-05 03:44:22.000000 IABT-1.2/IABT/InxioManifest.vsp
+-rw-rw-rw-   0        0        0        0 2023-08-06 02:43:33.000000 IABT-1.2/IABT/__init__.py
+-rw-rw-rw-   0        0        0    11739 2023-08-06 02:44:24.000000 IABT-1.2/IABT/build.py
+drwxrwxrwx   0        0        0        0 2023-08-06 02:47:10.000000 IABT-1.2/IABT/data/
+-rw-rw-rw-   0        0        0     7825 2023-07-30 10:25:48.000000 IABT-1.2/IABT/data/EventActivity.java
+-rw-rw-rw-   0        0        0     6236 2023-07-23 07:40:17.000000 IABT-1.2/IABT/data/FormalActivity.java
+-rw-rw-rw-   0        0        0     8430 2023-07-30 10:25:48.000000 IABT-1.2/IABT/data/PermissionActivity.java
+-rw-rw-rw-   0        0        0      126 2023-07-30 10:25:48.000000 IABT-1.2/IABT/data/VDialogInterface.java
+-rw-rw-rw-   0        0        0      134 2023-07-30 10:25:48.000000 IABT-1.2/IABT/data/VLocationListener.java
+-rw-rw-rw-   0        0        0      134 2023-07-30 10:25:48.000000 IABT-1.2/IABT/data/VOnClickListener.java
+-rw-rw-rw-   0        0        0      147 2023-07-30 10:25:48.000000 IABT-1.2/IABT/data/VSensorEventListener.java
+-rw-rw-rw-   0        0        0     2078 2023-08-05 04:02:38.000000 IABT-1.2/IABT/data/app_build.gradle
+-rw-rw-rw-   0        0        0      290 2023-07-30 15:14:52.000000 IABT-1.2/IABT/data/project_build.gradle
+-rw-rw-rw-   0        0        0     5054 2023-08-05 12:35:27.000000 IABT-1.2/IABT/file_control.py
+-rw-rw-rw-   0        0        0      773 2023-07-31 01:59:57.000000 IABT-1.2/IABT/generate_path.py
+-rw-rw-rw-   0        0        0    15929 2023-08-06 02:46:43.000000 IABT-1.2/IABT/iabt.py
+drwxrwxrwx   0        0        0        0 2023-08-06 02:47:10.000000 IABT-1.2/IABT/inxio_core/
+drwxrwxrwx   0        0        0        0 2023-08-06 02:47:10.000000 IABT-1.2/IABT/inxio_core/Inxio/
+-rw-rw-rw-   0        0        0        0 2023-06-06 07:24:07.000000 IABT-1.2/IABT/inxio_core/Inxio/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-06 02:47:10.000000 IABT-1.2/IABT/inxio_core/Inxio/android/
+drwxrwxrwx   0        0        0        0 2023-08-06 02:47:10.000000 IABT-1.2/IABT/inxio_core/Inxio/android/APP/
+-rw-rw-rw-   0        0        0        0 2023-05-21 04:19:19.000000 IABT-1.2/IABT/inxio_core/Inxio/android/APP/__init__.py
+-rw-rw-rw-   0        0        0     6720 2023-08-05 04:50:57.000000 IABT-1.2/IABT/inxio_core/Inxio/android/APP/app.py
+-rw-rw-rw-   0        0        0    15752 2023-06-08 07:42:03.000000 IABT-1.2/IABT/inxio_core/Inxio/android/APP/permission.py
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:40:31.000000 IABT-1.2/IABT/inxio_core/Inxio/android/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-06 02:47:10.000000 IABT-1.2/IABT/inxio_core/Inxio/android/core_components/
+-rw-rw-rw-   0        0        0    15598 2023-08-05 03:47:28.000000 IABT-1.2/IABT/inxio_core/Inxio/android/core_components/Activity.py
+-rw-rw-rw-   0        0        0     2992 2023-06-06 11:34:29.000000 IABT-1.2/IABT/inxio_core/Inxio/android/core_components/Bundle.py
+-rw-rw-rw-   0        0        0     8728 2023-06-08 09:30:34.000000 IABT-1.2/IABT/inxio_core/Inxio/android/core_components/EventProcess.py
+-rw-rw-rw-   0        0        0      229 2023-08-05 03:47:28.000000 IABT-1.2/IABT/inxio_core/Inxio/android/core_components/Fragment.py
+-rw-rw-rw-   0        0        0      726 2023-08-05 03:47:28.000000 IABT-1.2/IABT/inxio_core/Inxio/android/core_components/Intent.py
+-rw-rw-rw-   0        0        0     5451 2023-08-05 03:47:28.000000 IABT-1.2/IABT/inxio_core/Inxio/android/core_components/LocationManager.py
+-rw-rw-rw-   0        0        0    12985 2023-08-05 03:47:28.000000 IABT-1.2/IABT/inxio_core/Inxio/android/core_components/NotificationManager.py
+-rw-rw-rw-   0        0        0     2368 2023-06-12 08:23:38.000000 IABT-1.2/IABT/inxio_core/Inxio/android/core_components/PendingIntent.py
+-rw-rw-rw-   0        0        0     6025 2023-08-05 03:47:28.000000 IABT-1.2/IABT/inxio_core/Inxio/android/core_components/SensorManager.py
+-rw-rw-rw-   0        0        0        0 2023-07-01 04:16:08.000000 IABT-1.2/IABT/inxio_core/Inxio/android/core_components/Service.py
+-rw-rw-rw-   0        0        0     2064 2023-08-05 03:47:28.000000 IABT-1.2/IABT/inxio_core/Inxio/android/core_components/View.py
+-rw-rw-rw-   0        0        0     1994 2023-08-05 03:44:22.000000 IABT-1.2/IABT/inxio_core/Inxio/android/core_components/View_Listeners.py
+-rw-rw-rw-   0        0        0     6855 2023-05-06 04:49:08.000000 IABT-1.2/IABT/inxio_core/Inxio/android/core_components/XMLGenerator.py
+-rw-rw-rw-   0        0        0        0 2023-05-05 13:58:33.000000 IABT-1.2/IABT/inxio_core/Inxio/android/core_components/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-06 02:47:10.000000 IABT-1.2/IABT/inxio_core/Inxio/android/executable/
+-rw-rw-rw-   0        0        0     4716 2023-08-05 03:47:28.000000 IABT-1.2/IABT/inxio_core/Inxio/android/executable/ExecutionBlock.py
+-rw-rw-rw-   0        0        0        0 2023-05-21 03:35:13.000000 IABT-1.2/IABT/inxio_core/Inxio/android/executable/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-06 02:47:10.000000 IABT-1.2/IABT/inxio_core/Inxio/android/ui/
+drwxrwxrwx   0        0        0        0 2023-08-06 02:47:10.000000 IABT-1.2/IABT/inxio_core/Inxio/android/ui/Element/
+-rw-rw-rw-   0        0        0     1205 2023-08-05 03:47:28.000000 IABT-1.2/IABT/inxio_core/Inxio/android/ui/Element/AlertDialog.py
+-rw-rw-rw-   0        0        0     1169 2023-08-05 03:47:28.000000 IABT-1.2/IABT/inxio_core/Inxio/android/ui/Element/Text.py
+-rw-rw-rw-   0        0        0      478 2023-05-21 05:27:23.000000 IABT-1.2/IABT/inxio_core/Inxio/android/ui/Element/Toast.py
+-rw-rw-rw-   0        0        0        0 2023-05-05 13:59:30.000000 IABT-1.2/IABT/inxio_core/Inxio/android/ui/Element/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-06 02:47:10.000000 IABT-1.2/IABT/inxio_core/Inxio/android/ui/Layout/
+-rw-rw-rw-   0        0        0      742 2023-08-05 03:46:48.000000 IABT-1.2/IABT/inxio_core/Inxio/android/ui/Layout/FrameLayout.py
+-rw-rw-rw-   0        0        0     1090 2023-08-05 03:47:28.000000 IABT-1.2/IABT/inxio_core/Inxio/android/ui/Layout/GridLayout.py
+-rw-rw-rw-   0        0        0     1763 2023-05-06 04:40:15.000000 IABT-1.2/IABT/inxio_core/Inxio/android/ui/Layout/LayoutParams.py
+-rw-rw-rw-   0        0        0      926 2023-08-05 03:47:28.000000 IABT-1.2/IABT/inxio_core/Inxio/android/ui/Layout/LinearLayout.py
+-rw-rw-rw-   0        0        0      855 2023-08-05 03:47:28.000000 IABT-1.2/IABT/inxio_core/Inxio/android/ui/Layout/RelativeLayout.py
+-rw-rw-rw-   0        0        0      707 2023-08-05 03:47:28.000000 IABT-1.2/IABT/inxio_core/Inxio/android/ui/Layout/TableLayout.py
+-rw-rw-rw-   0        0        0        0 2023-05-05 13:59:09.000000 IABT-1.2/IABT/inxio_core/Inxio/android/ui/Layout/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-05-05 13:58:55.000000 IABT-1.2/IABT/inxio_core/Inxio/android/ui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-06 02:47:10.000000 IABT-1.2/IABT/inxio_core/Inxio/android/vsp/
+-rw-rw-rw-   0        0        0    39731 2023-08-05 03:47:28.000000 IABT-1.2/IABT/inxio_core/Inxio/android/vsp/VSPparser.py
+-rw-rw-rw-   0        0        0        0 2023-06-04 23:25:11.000000 IABT-1.2/IABT/inxio_core/Inxio/android/vsp/__init__.py
+-rw-rw-rw-   0        0        0      327 2023-06-04 23:25:29.000000 IABT-1.2/IABT/inxio_core/Inxio/android/vsp/try.py
+-rw-rw-rw-   0        0        0      255 2023-05-24 12:38:20.000000 IABT-1.2/IABT/inxio_core/Inxio/android/vsp/try.vsp
+-rw-rw-rw-   0        0        0       33 2023-05-28 14:02:07.000000 IABT-1.2/IABT/inxio_core/Inxio/android/vsp/ty.py
+-rw-rw-rw-   0        0        0      425 2023-06-04 23:15:22.000000 IABT-1.2/IABT/inxio_core/Inxio/android/vsp/vsp2xml.py
+-rw-rw-rw-   0        0        0      951 2023-08-05 03:47:28.000000 IABT-1.2/IABT/inxio_core/Inxio/android/vsp/语法.txt
+drwxrwxrwx   0        0        0        0 2023-08-06 02:47:10.000000 IABT-1.2/IABT/inxio_core/Inxio/extends/
+-rw-rw-rw-   0        0        0        0 2023-06-10 10:06:44.000000 IABT-1.2/IABT/inxio_core/Inxio/extends/__init__.py
+-rw-rw-rw-   0        0        0       67 2023-08-04 05:32:04.000000 IABT-1.2/IABT/inxio_core/Inxio/file_type.py
+-rw-rw-rw-   0        0        0       31 2023-08-05 04:00:36.000000 IABT-1.2/IABT/inxio_core/Inxio/global_var.py
+drwxrwxrwx   0        0        0        0 2023-08-06 02:47:10.000000 IABT-1.2/IABT/inxio_core/Inxio/ui_shell/
+-rw-rw-rw-   0        0        0      511 2023-08-05 03:47:28.000000 IABT-1.2/IABT/inxio_core/Inxio/ui_shell/Button.py
+-rw-rw-rw-   0        0        0        0 2023-08-05 01:52:53.000000 IABT-1.2/IABT/inxio_core/Inxio/ui_shell/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-08-06 02:43:46.000000 IABT-1.2/IABT/inxio_core/__init__.py
+-rw-rw-rw-   0        0        0     1285 2023-07-26 06:18:16.000000 IABT-1.2/IABT/json_control.py
+drwxrwxrwx   0        0        0        0 2023-08-06 02:47:10.000000 IABT-1.2/IABT/pretreatment_files/
+-rw-rw-rw-   0        0        0    35662 2023-08-04 14:17:54.000000 IABT-1.2/IABT/pretreatment_files/python.jpg
+drwxrwxrwx   0        0        0        0 2023-08-06 02:47:11.000000 IABT-1.2/IABT/translate/
+-rw-rw-rw-   0        0        0        0 2023-06-21 14:26:57.000000 IABT-1.2/IABT/translate/__init__.py
+-rw-rw-rw-   0        0        0     2572 2023-08-06 02:44:24.000000 IABT-1.2/IABT/translate/translator.py
+-rw-rw-rw-   0        0        0     5313 2023-08-06 02:44:24.000000 IABT-1.2/IABT/translate/vsp2xml.py
+-rw-rw-rw-   0        0        0     4463 2023-08-04 09:48:36.000000 IABT-1.2/IABT/translate/xml_generate.py
+-rw-rw-rw-   0        0        0     2443 2023-08-06 02:44:39.000000 IABT-1.2/IABT/try.py
+drwxrwxrwx   0        0        0        0 2023-08-06 02:47:11.000000 IABT-1.2/IABT/vsp/
+-rw-rw-rw-   0        0        0    40003 2023-08-05 03:47:28.000000 IABT-1.2/IABT/vsp/VSPparser.py
+-rw-rw-rw-   0        0        0        0 2023-06-04 23:25:11.000000 IABT-1.2/IABT/vsp/__init__.py
+-rw-rw-rw-   0        0        0      858 2023-07-01 04:39:51.000000 IABT-1.2/IABT/vsp/hellolay.vsp
+-rw-rw-rw-   0        0        0      327 2023-06-04 23:25:29.000000 IABT-1.2/IABT/vsp/try.py
+-rw-rw-rw-   0        0        0      243 2023-06-21 13:55:10.000000 IABT-1.2/IABT/vsp/try.vsp
+-rw-rw-rw-   0        0        0       33 2023-05-28 14:02:07.000000 IABT-1.2/IABT/vsp/ty.py
+-rw-rw-rw-   0        0        0      425 2023-06-04 23:15:22.000000 IABT-1.2/IABT/vsp/vsp2xml.py
+-rw-rw-rw-   0        0        0      951 2023-08-05 03:47:28.000000 IABT-1.2/IABT/vsp/语法.txt
+drwxrwxrwx   0        0        0        0 2023-08-06 02:47:10.000000 IABT-1.2/IABT.egg-info/
+-rw-rw-rw-   0        0        0      602 2023-08-06 02:47:10.000000 IABT-1.2/IABT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3235 2023-08-06 02:47:10.000000 IABT-1.2/IABT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-06 02:47:10.000000 IABT-1.2/IABT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-08-06 02:47:10.000000 IABT-1.2/IABT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-08-06 02:47:10.000000 IABT-1.2/IABT.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       26 2023-08-06 01:52:22.000000 IABT-1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      602 2023-08-06 02:47:11.000000 IABT-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      194 2023-08-05 05:21:21.000000 IABT-1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-06 02:47:11.000000 IABT-1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1440 2023-08-06 02:45:20.000000 IABT-1.2/setup.py
```

### Comparing `IABT-1.1/IABT/build.py` & `IABT-1.2/IABT/build.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from file_control import *
-from json_control import *
-from translate.translator import generate_xml
-from file_control import get_file_paths
-from vsp.VSPparser import VSP
-from translate.vsp2xml import generate_vm
+from IABT.file_control import *
+from IABT.json_control import *
+from IABT.translate.translator import generate_xml
+from IABT.file_control import get_file_paths
+from IABT.vsp.VSPparser import VSP
+from IABT.translate.vsp2xml import generate_vm
 
 
 def copy_data_to(project_path, asp_path, site):
     """
     将类似assets、resources文件夹中的东西拷贝到目标项目文件夹
     :param site: 域名
     :param project_path:此项目路径
```

### Comparing `IABT-1.1/IABT/data/EventActivity.java` & `IABT-1.2/IABT/data/EventActivity.java`

 * *Files identical despite different names*

### Comparing `IABT-1.1/IABT/data/FormalActivity.java` & `IABT-1.2/IABT/data/FormalActivity.java`

 * *Files identical despite different names*

### Comparing `IABT-1.1/IABT/data/PermissionActivity.java` & `IABT-1.2/IABT/data/PermissionActivity.java`

 * *Files identical despite different names*

### Comparing `IABT-1.1/IABT/data/app_build.gradle` & `IABT-1.2/IABT/data/app_build.gradle`

 * *Files identical despite different names*

### Comparing `IABT-1.1/IABT/file_control.py` & `IABT-1.2/IABT/file_control.py`

 * *Files 6% similar despite different names*

```diff
@@ -98,26 +98,27 @@
         shutil.copytree(old_path, new_path)
 
 
 def walkFile(file):
     root_path = file
     file_list = []
     for root, dirs, files in os.walk(file):
-
         # root 表示当前正在访问的文件夹路径
         # dirs 表示该文件夹下的子目录名list
         # files 表示该文件夹下的文件list
         # 遍历文件
         for f in files:
             file_list.append([root.split(root_path)[-1], f])
     return file_list
 
 
 def only_copy(old_path, new_path, update=False):
-    """new_path必须存在！不支持复制空文件夹"""
+    """
+    new_path必须存在！不支持复制空文件夹
+    """
     if update:
         shutil.rmtree(new_path)
     p = ["\\", "/"][int("/" in old_path)]
     p2 = ["\\", "/"][int("/" in new_path)]
     if old_path[-1] != p:
         old_path += p
     if new_path[-1] != p2:
@@ -144,7 +145,18 @@
     # shutil.copytree(r"C:\Users\Administrator\AndroidStudioProjects\PythonAPP\app\src\main\java\com\cemeye",
     #                 r"C:\Users\Administrator\Desktop\CV\PythonAPP\AndroidRequire\try")
     # only_copy(
     #     r"C:\Users\Administrator\Desktop\copy_test\a",
     #     r"C:\Users\Administrator\Desktop\copy_test\b"
     # )
     print(get_file_paths(r"C:\Users\Administrator\Desktop\CV\PythonAPP"))
+
+
+    class A:
+        def __init__(self):
+            ...
+
+        def __enter__(self):
+            return self
+
+        def __exit__(self, exc_type, exc_val, exc_tb):
+            ...
```

### Comparing `IABT-1.1/IABT/generate_path.py` & `IABT-1.2/IABT/generate_path.py`

 * *Files identical despite different names*

### Comparing `IABT-1.1/IABT/iabt.py` & `IABT-1.2/IABT/iabt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 
 import sys
-from generate_path import create_paths, create_path, create_files, create_file
-from build import *
+from IABT.generate_path import create_paths, create_path, create_files, create_file
+from IABT.build import *
 
 not_color = False
 
 all_right = True
 
 try:
     from colorama import Fore, Back, init
@@ -43,15 +43,15 @@
 ██║    ███████║    ██████╔╝       ██║          
 ██║    ██╔══██║    ██╔══██╗       ██║          
 ██║    ██║  ██║    ██████╔╝       ██║       ██╗
 ╚═╝    ╚═╝  ╚═╝    ╚═════╝        ╚═╝       ╚═╝
                                                """)
     print(Fore.LIGHTRED_EX + "        （Inxio Android Build Tools）")
     print(Fore.LIGHTGREEN_EX + """
-v.1.1
+v.1.2
 author:cemeye
 
 本代码用于创建、构建你的Inxio项目,以下是代码帮助.""")
     print(Fore.LIGHTWHITE_EX +
           f"""                            
   [*]参数列表:
   -l|--link     :     链接到目标AndroidStudio项目，后面请接参数[AndroidStudio项目路径]
@@ -83,15 +83,15 @@
 ██║    ██╔══██╗    ██╔══██╗    ╚══██╔══╝       
 ██║    ███████║    ██████╔╝       ██║          
 ██║    ██╔══██║    ██╔══██╗       ██║          
 ██║    ██║  ██║    ██████╔╝       ██║       ██╗
 ╚═╝    ╚═╝  ╚═╝    ╚═════╝        ╚═╝       ╚═╝
                                                
         （Inxio Android Build Tools）
-v.1.1
+v.1.2
 author:cemeye
 
 本代码用于创建、构建你的Inxio项目,以下是代码帮助.
   [*]参数列表:
   -l|--link     :     链接到目标AndroidStudio项目，后面请接参数[AndroidStudio项目路径]
   -n|--name     :     输入项目名称
   -c|--create   :     输入创建的Inxio项目路径
```

### Comparing `IABT-1.1/IABT/inxio_core/Inxio/android/APP/app.py` & `IABT-1.2/IABT/inxio_core/Inxio/android/APP/app.py`

 * *Files identical despite different names*

### Comparing `IABT-1.1/IABT/inxio_core/Inxio/android/APP/permission.py` & `IABT-1.2/IABT/inxio_core/Inxio/android/APP/permission.py`

 * *Files identical despite different names*

### Comparing `IABT-1.1/IABT/inxio_core/Inxio/android/core_components/Activity.py` & `IABT-1.2/IABT/inxio_core/Inxio/android/core_components/Activity.py`

 * *Files identical despite different names*

### Comparing `IABT-1.1/IABT/inxio_core/Inxio/android/core_components/Bundle.py` & `IABT-1.2/IABT/inxio_core/Inxio/android/core_components/Bundle.py`

 * *Files identical despite different names*

### Comparing `IABT-1.1/IABT/inxio_core/Inxio/android/core_components/EventProcess.py` & `IABT-1.2/IABT/inxio_core/Inxio/android/core_components/EventProcess.py`

 * *Files identical despite different names*

### Comparing `IABT-1.1/IABT/inxio_core/Inxio/android/core_components/Intent.py` & `IABT-1.2/IABT/inxio_core/Inxio/android/core_components/Intent.py`

 * *Files identical despite different names*

### Comparing `IABT-1.1/IABT/inxio_core/Inxio/android/core_components/LocationManager.py` & `IABT-1.2/IABT/inxio_core/Inxio/android/core_components/LocationManager.py`

 * *Files identical despite different names*

### Comparing `IABT-1.1/IABT/inxio_core/Inxio/android/core_components/NotificationManager.py` & `IABT-1.2/IABT/inxio_core/Inxio/android/core_components/NotificationManager.py`

 * *Files identical despite different names*

### Comparing `IABT-1.1/IABT/inxio_core/Inxio/android/core_components/PendingIntent.py` & `IABT-1.2/IABT/inxio_core/Inxio/android/core_components/PendingIntent.py`

 * *Files identical despite different names*

### Comparing `IABT-1.1/IABT/inxio_core/Inxio/android/core_components/SensorManager.py` & `IABT-1.2/IABT/inxio_core/Inxio/android/core_components/SensorManager.py`

 * *Files identical despite different names*

### Comparing `IABT-1.1/IABT/inxio_core/Inxio/android/core_components/View.py` & `IABT-1.2/IABT/inxio_core/Inxio/android/core_components/View.py`

 * *Files identical despite different names*

### Comparing `IABT-1.1/IABT/inxio_core/Inxio/android/core_components/View_Listeners.py` & `IABT-1.2/IABT/inxio_core/Inxio/android/core_components/View_Listeners.py`

 * *Files identical despite different names*

### Comparing `IABT-1.1/IABT/inxio_core/Inxio/android/core_components/XMLGenerator.py` & `IABT-1.2/IABT/inxio_core/Inxio/android/core_components/XMLGenerator.py`

 * *Files identical despite different names*

### Comparing `IABT-1.1/IABT/inxio_core/Inxio/android/executable/ExecutionBlock.py` & `IABT-1.2/IABT/inxio_core/Inxio/android/executable/ExecutionBlock.py`

 * *Files identical despite different names*

### Comparing `IABT-1.1/IABT/inxio_core/Inxio/android/ui/Element/AlertDialog.py` & `IABT-1.2/IABT/inxio_core/Inxio/android/ui/Element/AlertDialog.py`

 * *Files identical despite different names*

### Comparing `IABT-1.1/IABT/inxio_core/Inxio/android/ui/Element/Text.py` & `IABT-1.2/IABT/inxio_core/Inxio/android/ui/Element/Text.py`

 * *Files identical despite different names*

### Comparing `IABT-1.1/IABT/inxio_core/Inxio/android/ui/Layout/FrameLayout.py` & `IABT-1.2/IABT/inxio_core/Inxio/android/ui/Layout/FrameLayout.py`

 * *Files identical despite different names*

### Comparing `IABT-1.1/IABT/inxio_core/Inxio/android/ui/Layout/GridLayout.py` & `IABT-1.2/IABT/inxio_core/Inxio/android/ui/Layout/GridLayout.py`

 * *Files identical despite different names*

### Comparing `IABT-1.1/IABT/inxio_core/Inxio/android/ui/Layout/LayoutParams.py` & `IABT-1.2/IABT/inxio_core/Inxio/android/ui/Layout/LayoutParams.py`

 * *Files identical despite different names*

### Comparing `IABT-1.1/IABT/inxio_core/Inxio/android/ui/Layout/LinearLayout.py` & `IABT-1.2/IABT/inxio_core/Inxio/android/ui/Layout/LinearLayout.py`

 * *Files identical despite different names*

### Comparing `IABT-1.1/IABT/inxio_core/Inxio/android/ui/Layout/RelativeLayout.py` & `IABT-1.2/IABT/inxio_core/Inxio/android/ui/Layout/RelativeLayout.py`

 * *Files identical despite different names*

### Comparing `IABT-1.1/IABT/inxio_core/Inxio/android/ui/Layout/TableLayout.py` & `IABT-1.2/IABT/inxio_core/Inxio/android/ui/Layout/TableLayout.py`

 * *Files identical despite different names*

### Comparing `IABT-1.1/IABT/inxio_core/Inxio/android/vsp/VSPparser.py` & `IABT-1.2/IABT/inxio_core/Inxio/android/vsp/VSPparser.py`

 * *Files identical despite different names*

### Comparing `IABT-1.1/IABT/json_control.py` & `IABT-1.2/IABT/json_control.py`

 * *Files identical despite different names*

### Comparing `IABT-1.1/IABT/pretreatment_files/python.jpg` & `IABT-1.2/IABT/pretreatment_files/python.jpg`

 * *Files identical despite different names*

### Comparing `IABT-1.1/IABT/translate/translator.py` & `IABT-1.2/IABT/translate/translator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from translate.vsp2xml import LayoutTranslator
-from vsp.VSPparser import VSP
+from IABT.translate.vsp2xml import LayoutTranslator
+from IABT.vsp.VSPparser import VSP
 import os
 import random
 
 
 def random_name(length=8) -> str:
     result = ""
     for i in range(length):
@@ -34,15 +34,15 @@
 
 
 def load_string(vsp_str, name=None, encoding="utf-8"):
     if not name:
         file_name = random_name(length=10) + ".vsp"
     else:
         file_name = name + ".vsp"
-    write_file(file_name, "./", vsp_str, encoding=encoding)
+    write_file(file_name, "/", vsp_str, encoding=encoding)
     vsp_class = VSP(path=f"./{file_name}").get_tab().son[0]
     os.remove("./" + file_name)
     return vsp_class
 
 
 def generate_xml_by_string(vsp_str, xml_name, path, encoding="utf-8"):
     """
```

### Comparing `IABT-1.1/IABT/translate/vsp2xml.py` & `IABT-1.2/IABT/translate/vsp2xml.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 将VSP源代码转化为XML代码，即第一次编译
 """
-from translate.xml_generate import XMLTag, DataTag
-from vsp.VSPparser import VSPTab
+from IABT.translate.xml_generate import XMLTag, DataTag
+from IABT.vsp.VSPparser import VSPTab
 
 
 def _(x):
     return x[1:]
 
 
 class LayoutTranslator:
```

### Comparing `IABT-1.1/IABT/translate/xml_generate.py` & `IABT-1.2/IABT/translate/xml_generate.py`

 * *Files identical despite different names*

### Comparing `IABT-1.1/IABT/vsp/VSPparser.py` & `IABT-1.2/IABT/vsp/VSPparser.py`

 * *Files identical despite different names*

### Comparing `IABT-1.1/IABT.egg-info/PKG-INFO` & `IABT-1.2/IABT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IABT
-Version: 1.1
+Version: 1.2
 Summary: IABT is a tool to build your Inxio project.It can create a project and build a project.
 Home-page: UNKNOWN
 Author: cemeye
 Author-email: caomingyang2022@163.com
 License: MIT
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `IABT-1.1/PKG-INFO` & `IABT-1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IABT
-Version: 1.1
+Version: 1.2
 Summary: IABT is a tool to build your Inxio project.It can create a project and build a project.
 Home-page: UNKNOWN
 Author: cemeye
 Author-email: caomingyang2022@163.com
 License: MIT
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `IABT-1.1/setup.py` & `IABT-1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # these things are needed for the README.md show on pypi (if you dont need delete it)
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 # you need to change all these
-VERSION = '1.1'
+VERSION = '1.2'
 DESCRIPTION = 'IABT is a tool to build your Inxio project.It can create a project and build a project.'
 
 setup(
     name="IABT",
     version=VERSION,
     author="cemeye",
     author_email="caomingyang2022@163.com",
```

