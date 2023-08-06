# Comparing `tmp/Furious-GUI-0.1.8.tar.gz` & `tmp/Furious-GUI-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Furious-GUI-0.1.8.tar", last modified: Sat Aug  5 03:48:21 2023, max compression
+gzip compressed data, was "Furious-GUI-0.1.9.tar", last modified: Sun Aug  6 09:19:37 2023, max compression
```

## Comparing `Furious-GUI-0.1.8.tar` & `Furious-GUI-0.1.9.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxrwx   0        0        0        0 2023-08-05 03:48:21.872787 Furious-GUI-0.1.8/
-drwxrwxrwx   0        0        0        0 2023-08-05 03:48:21.481694 Furious-GUI-0.1.8/Furious/
-drwxrwxrwx   0        0        0        0 2023-08-05 03:48:21.560144 Furious-GUI-0.1.8/Furious/Action/
--rw-rw-rw-   0        0        0    25095 2023-08-05 03:44:20.000000 Furious-GUI-0.1.8/Furious/Action/Connect.py
--rw-rw-rw-   0        0        0      487 2023-07-24 11:35:24.000000 Furious-GUI-0.1.8/Furious/Action/EditConfiguration.py
--rw-rw-rw-   0        0        0      450 2023-07-24 11:35:24.000000 Furious-GUI-0.1.8/Furious/Action/Exit.py
--rw-rw-rw-   0        0        0     7140 2023-07-24 11:35:24.000000 Furious-GUI-0.1.8/Furious/Action/Export.py
--rw-rw-rw-   0        0        0    15675 2023-08-05 03:44:20.000000 Furious-GUI-0.1.8/Furious/Action/Import.py
--rw-rw-rw-   0        0        0     1514 2023-07-24 11:35:24.000000 Furious-GUI-0.1.8/Furious/Action/Language.py
--rw-rw-rw-   0        0        0     1724 2023-07-24 11:35:24.000000 Furious-GUI-0.1.8/Furious/Action/Routing.py
--rw-rw-rw-   0        0        0     2417 2023-07-24 11:35:24.000000 Furious-GUI-0.1.8/Furious/Action/Settings.py
--rw-rw-rw-   0        0        0      268 2023-07-24 11:35:24.000000 Furious-GUI-0.1.8/Furious/Action/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-05 03:48:21.575730 Furious-GUI-0.1.8/Furious/Core/
--rw-rw-rw-   0        0        0    21870 2023-08-05 03:44:20.000000 Furious-GUI-0.1.8/Furious/Core/Configuration.py
--rw-rw-rw-   0        0        0     4755 2023-07-24 11:35:24.000000 Furious-GUI-0.1.8/Furious/Core/Core.py
--rw-rw-rw-   0        0        0     4575 2023-08-05 03:44:20.000000 Furious-GUI-0.1.8/Furious/Core/Intellisense.py
--rw-rw-rw-   0        0        0        0 2023-07-24 11:35:24.000000 Furious-GUI-0.1.8/Furious/Core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-05 03:48:21.450784 Furious-GUI-0.1.8/Furious/Data/
-drwxrwxrwx   0        0        0        0 2023-08-05 03:48:21.591197 Furious-GUI-0.1.8/Furious/Data/font/
--rw-rw-rw-   0        0        0   624892 2023-07-25 08:47:27.000000 Furious-GUI-0.1.8/Furious/Data/font/CascadiaMono
-drwxrwxrwx   0        0        0        0 2023-08-05 03:48:21.606672 Furious-GUI-0.1.8/Furious/Data/hysteria/
--rw-rw-rw-   0        0        0  1427940 2023-07-25 08:47:27.000000 Furious-GUI-0.1.8/Furious/Data/hysteria/bypass-mainland-China.acl
--rw-rw-rw-   0        0        0  5872899 2023-07-25 08:47:27.000000 Furious-GUI-0.1.8/Furious/Data/hysteria/country.mmdb
-drwxrwxrwx   0        0        0        0 2023-08-05 03:48:21.653938 Furious-GUI-0.1.8/Furious/Data/xray/
--rw-rw-rw-   0        0        0 10006207 2023-07-25 08:47:27.000000 Furious-GUI-0.1.8/Furious/Data/xray/geoip.dat
--rw-rw-rw-   0        0        0  1512983 2023-07-25 08:47:27.000000 Furious-GUI-0.1.8/Furious/Data/xray/geosite.dat
-drwxrwxrwx   0        0        0        0 2023-08-05 03:48:21.669633 Furious-GUI-0.1.8/Furious/Gui/
--rw-rw-rw-   0        0        0     4736 2023-07-24 11:35:24.000000 Furious-GUI-0.1.8/Furious/Gui/Action.py
--rw-rw-rw-   0        0        0      180 2023-07-24 11:35:24.000000 Furious-GUI-0.1.8/Furious/Gui/Icon.py
--rw-rw-rw-   0        0        0        0 2023-07-24 11:35:24.000000 Furious-GUI-0.1.8/Furious/Gui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-05 03:48:21.763183 Furious-GUI-0.1.8/Furious/Utility/
--rw-rw-rw-   0        0        0     1007 2023-07-25 08:47:36.000000 Furious-GUI-0.1.8/Furious/Utility/Constants.py
--rw-rw-rw-   0        0        0     2535 2023-07-24 11:35:24.000000 Furious-GUI-0.1.8/Furious/Utility/Process.py
--rw-rw-rw-   0        0        0     7375 2023-07-24 11:35:24.000000 Furious-GUI-0.1.8/Furious/Utility/Proxy.py
--rw-rw-rw-   0        0        0    42815 2023-07-26 11:22:03.000000 Furious-GUI-0.1.8/Furious/Utility/Resources.py
--rw-rw-rw-   0        0        0     2494 2023-07-24 11:35:24.000000 Furious-GUI-0.1.8/Furious/Utility/Settings.py
--rw-rw-rw-   0        0        0     5829 2023-07-24 11:35:24.000000 Furious-GUI-0.1.8/Furious/Utility/StartupOnBoot.py
--rw-rw-rw-   0        0        0     2364 2023-07-24 11:35:24.000000 Furious-GUI-0.1.8/Furious/Utility/Theme.py
--rw-rw-rw-   0        0        0    24098 2023-07-24 11:35:24.000000 Furious-GUI-0.1.8/Furious/Utility/Translator.py
--rw-rw-rw-   0        0        0     5231 2023-08-05 03:44:20.000000 Furious-GUI-0.1.8/Furious/Utility/Utility.py
--rw-rw-rw-   0        0        0        0 2023-07-24 11:35:24.000000 Furious-GUI-0.1.8/Furious/Utility/__init__.py
--rw-rw-rw-   0        0        0       23 2023-08-05 03:44:20.000000 Furious-GUI-0.1.8/Furious/Version.py
-drwxrwxrwx   0        0        0        0 2023-08-05 03:48:21.841090 Furious-GUI-0.1.8/Furious/Widget/
--rw-rw-rw-   0        0        0     8709 2023-07-26 11:36:26.000000 Furious-GUI-0.1.8/Furious/Widget/Application.py
--rw-rw-rw-   0        0        0     1975 2023-07-24 11:35:24.000000 Furious-GUI-0.1.8/Furious/Widget/ConnectingProgressBar.py
--rw-rw-rw-   0        0        0    66998 2023-07-24 11:35:24.000000 Furious-GUI-0.1.8/Furious/Widget/EditConfiguration.py
--rw-rw-rw-   0        0        0     1733 2023-07-24 11:35:24.000000 Furious-GUI-0.1.8/Furious/Widget/ExportQRCode.py
--rw-rw-rw-   0        0        0     1946 2023-07-24 11:35:24.000000 Furious-GUI-0.1.8/Furious/Widget/IndentSpinBox.py
--rw-rw-rw-   0        0        0     6618 2023-07-24 11:35:24.000000 Furious-GUI-0.1.8/Furious/Widget/LogViewer.py
--rw-rw-rw-   0        0        0     2811 2023-07-24 11:35:24.000000 Furious-GUI-0.1.8/Furious/Widget/SystemTrayIcon.py
--rw-rw-rw-   0        0        0     3808 2023-07-24 11:35:24.000000 Furious-GUI-0.1.8/Furious/Widget/Widget.py
--rw-rw-rw-   0        0        0        0 2023-07-24 11:35:24.000000 Furious-GUI-0.1.8/Furious/Widget/__init__.py
--rw-rw-rw-   0        0        0       32 2023-07-24 11:35:24.000000 Furious-GUI-0.1.8/Furious/__init__.py
--rw-rw-rw-   0        0        0     4260 2023-07-24 11:35:24.000000 Furious-GUI-0.1.8/Furious/__main__.py
-drwxrwxrwx   0        0        0        0 2023-08-05 03:48:21.872787 Furious-GUI-0.1.8/Furious_GUI.egg-info/
--rw-rw-rw-   0        0        0    10866 2023-08-05 03:48:21.000000 Furious-GUI-0.1.8/Furious_GUI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1445 2023-08-05 03:48:21.000000 Furious-GUI-0.1.8/Furious_GUI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-05 03:48:21.000000 Furious-GUI-0.1.8/Furious_GUI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-08-05 03:48:21.000000 Furious-GUI-0.1.8/Furious_GUI.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      195 2023-08-05 03:48:21.000000 Furious-GUI-0.1.8/Furious_GUI.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-08-05 03:48:21.000000 Furious-GUI-0.1.8/Furious_GUI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35823 2023-07-25 08:47:27.000000 Furious-GUI-0.1.8/LICENSE
--rw-rw-rw-   0        0        0    10866 2023-08-05 03:48:21.872787 Furious-GUI-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     9850 2023-08-05 03:44:20.000000 Furious-GUI-0.1.8/README.md
--rw-rw-rw-   0        0        0       42 2023-08-05 03:48:21.872787 Furious-GUI-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1820 2023-08-05 03:44:20.000000 Furious-GUI-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-06 09:19:36.987103 Furious-GUI-0.1.9/
+drwxrwxrwx   0        0        0        0 2023-08-06 09:19:36.627583 Furious-GUI-0.1.9/Furious/
+drwxrwxrwx   0        0        0        0 2023-08-06 09:19:36.658737 Furious-GUI-0.1.9/Furious/Action/
+-rw-rw-rw-   0        0        0    25095 2023-08-05 03:44:20.000000 Furious-GUI-0.1.9/Furious/Action/Connect.py
+-rw-rw-rw-   0        0        0      487 2023-07-24 11:35:24.000000 Furious-GUI-0.1.9/Furious/Action/EditConfiguration.py
+-rw-rw-rw-   0        0        0      450 2023-07-24 11:35:24.000000 Furious-GUI-0.1.9/Furious/Action/Exit.py
+-rw-rw-rw-   0        0        0     7140 2023-07-24 11:35:24.000000 Furious-GUI-0.1.9/Furious/Action/Export.py
+-rw-rw-rw-   0        0        0    15675 2023-08-05 03:44:20.000000 Furious-GUI-0.1.9/Furious/Action/Import.py
+-rw-rw-rw-   0        0        0     1514 2023-07-24 11:35:24.000000 Furious-GUI-0.1.9/Furious/Action/Language.py
+-rw-rw-rw-   0        0        0     1724 2023-07-24 11:35:24.000000 Furious-GUI-0.1.9/Furious/Action/Routing.py
+-rw-rw-rw-   0        0        0     2417 2023-07-24 11:35:24.000000 Furious-GUI-0.1.9/Furious/Action/Settings.py
+-rw-rw-rw-   0        0        0      268 2023-07-24 11:35:24.000000 Furious-GUI-0.1.9/Furious/Action/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-06 09:19:36.674432 Furious-GUI-0.1.9/Furious/Core/
+-rw-rw-rw-   0        0        0    21870 2023-08-05 03:44:20.000000 Furious-GUI-0.1.9/Furious/Core/Configuration.py
+-rw-rw-rw-   0        0        0     4755 2023-07-24 11:35:24.000000 Furious-GUI-0.1.9/Furious/Core/Core.py
+-rw-rw-rw-   0        0        0     4575 2023-08-05 03:44:20.000000 Furious-GUI-0.1.9/Furious/Core/Intellisense.py
+-rw-rw-rw-   0        0        0        0 2023-07-24 11:35:24.000000 Furious-GUI-0.1.9/Furious/Core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-06 09:19:36.596685 Furious-GUI-0.1.9/Furious/Data/
+drwxrwxrwx   0        0        0        0 2023-08-06 09:19:36.689973 Furious-GUI-0.1.9/Furious/Data/font/
+-rw-rw-rw-   0        0        0   624892 2023-07-25 08:47:27.000000 Furious-GUI-0.1.9/Furious/Data/font/CascadiaMono
+drwxrwxrwx   0        0        0        0 2023-08-06 09:19:36.706070 Furious-GUI-0.1.9/Furious/Data/hysteria/
+-rw-rw-rw-   0        0        0  1427940 2023-07-25 08:47:27.000000 Furious-GUI-0.1.9/Furious/Data/hysteria/bypass-mainland-China.acl
+-rw-rw-rw-   0        0        0  5872899 2023-07-25 08:47:27.000000 Furious-GUI-0.1.9/Furious/Data/hysteria/country.mmdb
+drwxrwxrwx   0        0        0        0 2023-08-06 09:19:36.752627 Furious-GUI-0.1.9/Furious/Data/xray/
+-rw-rw-rw-   0        0        0 10006207 2023-07-25 08:47:27.000000 Furious-GUI-0.1.9/Furious/Data/xray/geoip.dat
+-rw-rw-rw-   0        0        0  1512983 2023-07-25 08:47:27.000000 Furious-GUI-0.1.9/Furious/Data/xray/geosite.dat
+drwxrwxrwx   0        0        0        0 2023-08-06 09:19:36.752627 Furious-GUI-0.1.9/Furious/Gui/
+-rw-rw-rw-   0        0        0     4736 2023-07-24 11:35:24.000000 Furious-GUI-0.1.9/Furious/Gui/Action.py
+-rw-rw-rw-   0        0        0      180 2023-07-24 11:35:24.000000 Furious-GUI-0.1.9/Furious/Gui/Icon.py
+-rw-rw-rw-   0        0        0        0 2023-07-24 11:35:24.000000 Furious-GUI-0.1.9/Furious/Gui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-06 09:19:36.799538 Furious-GUI-0.1.9/Furious/Utility/
+-rw-rw-rw-   0        0        0     1007 2023-07-25 08:47:36.000000 Furious-GUI-0.1.9/Furious/Utility/Constants.py
+-rw-rw-rw-   0        0        0     2535 2023-07-24 11:35:24.000000 Furious-GUI-0.1.9/Furious/Utility/Process.py
+-rw-rw-rw-   0        0        0     7375 2023-07-24 11:35:24.000000 Furious-GUI-0.1.9/Furious/Utility/Proxy.py
+-rw-rw-rw-   0        0        0    42815 2023-07-26 11:22:03.000000 Furious-GUI-0.1.9/Furious/Utility/Resources.py
+-rw-rw-rw-   0        0        0     2494 2023-07-24 11:35:24.000000 Furious-GUI-0.1.9/Furious/Utility/Settings.py
+-rw-rw-rw-   0        0        0     5829 2023-07-24 11:35:24.000000 Furious-GUI-0.1.9/Furious/Utility/StartupOnBoot.py
+-rw-rw-rw-   0        0        0     2364 2023-07-24 11:35:24.000000 Furious-GUI-0.1.9/Furious/Utility/Theme.py
+-rw-rw-rw-   0        0        0    24098 2023-07-24 11:35:24.000000 Furious-GUI-0.1.9/Furious/Utility/Translator.py
+-rw-rw-rw-   0        0        0     5231 2023-08-05 03:44:20.000000 Furious-GUI-0.1.9/Furious/Utility/Utility.py
+-rw-rw-rw-   0        0        0        0 2023-07-24 11:35:24.000000 Furious-GUI-0.1.9/Furious/Utility/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-08-06 09:18:41.000000 Furious-GUI-0.1.9/Furious/Version.py
+drwxrwxrwx   0        0        0        0 2023-08-06 09:19:36.955910 Furious-GUI-0.1.9/Furious/Widget/
+-rw-rw-rw-   0        0        0     8709 2023-07-26 11:36:26.000000 Furious-GUI-0.1.9/Furious/Widget/Application.py
+-rw-rw-rw-   0        0        0     1975 2023-07-24 11:35:24.000000 Furious-GUI-0.1.9/Furious/Widget/ConnectingProgressBar.py
+-rw-rw-rw-   0        0        0    66998 2023-07-24 11:35:24.000000 Furious-GUI-0.1.9/Furious/Widget/EditConfiguration.py
+-rw-rw-rw-   0        0        0     1733 2023-07-24 11:35:24.000000 Furious-GUI-0.1.9/Furious/Widget/ExportQRCode.py
+-rw-rw-rw-   0        0        0     1946 2023-07-24 11:35:24.000000 Furious-GUI-0.1.9/Furious/Widget/IndentSpinBox.py
+-rw-rw-rw-   0        0        0     6618 2023-07-24 11:35:24.000000 Furious-GUI-0.1.9/Furious/Widget/LogViewer.py
+-rw-rw-rw-   0        0        0     2811 2023-07-24 11:35:24.000000 Furious-GUI-0.1.9/Furious/Widget/SystemTrayIcon.py
+-rw-rw-rw-   0        0        0     3808 2023-07-24 11:35:24.000000 Furious-GUI-0.1.9/Furious/Widget/Widget.py
+-rw-rw-rw-   0        0        0        0 2023-07-24 11:35:24.000000 Furious-GUI-0.1.9/Furious/Widget/__init__.py
+-rw-rw-rw-   0        0        0       32 2023-07-24 11:35:24.000000 Furious-GUI-0.1.9/Furious/__init__.py
+-rw-rw-rw-   0        0        0     4260 2023-07-24 11:35:24.000000 Furious-GUI-0.1.9/Furious/__main__.py
+drwxrwxrwx   0        0        0        0 2023-08-06 09:19:36.987103 Furious-GUI-0.1.9/Furious_GUI.egg-info/
+-rw-rw-rw-   0        0        0    10866 2023-08-06 09:19:36.000000 Furious-GUI-0.1.9/Furious_GUI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1445 2023-08-06 09:19:36.000000 Furious-GUI-0.1.9/Furious_GUI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-06 09:19:36.000000 Furious-GUI-0.1.9/Furious_GUI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-08-06 09:19:36.000000 Furious-GUI-0.1.9/Furious_GUI.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      201 2023-08-06 09:19:36.000000 Furious-GUI-0.1.9/Furious_GUI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-08-06 09:19:36.000000 Furious-GUI-0.1.9/Furious_GUI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35823 2023-07-25 08:47:27.000000 Furious-GUI-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0    10866 2023-08-06 09:19:36.987103 Furious-GUI-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     9850 2023-08-05 03:44:20.000000 Furious-GUI-0.1.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-06 09:19:36.987103 Furious-GUI-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1838 2023-08-06 09:18:41.000000 Furious-GUI-0.1.9/setup.py
```

### Comparing `Furious-GUI-0.1.8/Furious/Action/Connect.py` & `Furious-GUI-0.1.9/Furious/Action/Connect.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.8/Furious/Action/Export.py` & `Furious-GUI-0.1.9/Furious/Action/Export.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.8/Furious/Action/Import.py` & `Furious-GUI-0.1.9/Furious/Action/Import.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.8/Furious/Action/Language.py` & `Furious-GUI-0.1.9/Furious/Action/Language.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.8/Furious/Action/Routing.py` & `Furious-GUI-0.1.9/Furious/Action/Routing.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.8/Furious/Action/Settings.py` & `Furious-GUI-0.1.9/Furious/Action/Settings.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.8/Furious/Core/Configuration.py` & `Furious-GUI-0.1.9/Furious/Core/Configuration.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.8/Furious/Core/Core.py` & `Furious-GUI-0.1.9/Furious/Core/Core.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.8/Furious/Core/Intellisense.py` & `Furious-GUI-0.1.9/Furious/Core/Intellisense.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.8/Furious/Data/font/CascadiaMono` & `Furious-GUI-0.1.9/Furious/Data/font/CascadiaMono`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.8/Furious/Data/hysteria/bypass-mainland-China.acl` & `Furious-GUI-0.1.9/Furious/Data/hysteria/bypass-mainland-China.acl`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.8/Furious/Data/hysteria/country.mmdb` & `Furious-GUI-0.1.9/Furious/Data/hysteria/country.mmdb`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.8/Furious/Data/xray/geoip.dat` & `Furious-GUI-0.1.9/Furious/Data/xray/geoip.dat`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.8/Furious/Data/xray/geosite.dat` & `Furious-GUI-0.1.9/Furious/Data/xray/geosite.dat`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.8/Furious/Gui/Action.py` & `Furious-GUI-0.1.9/Furious/Gui/Action.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.8/Furious/Utility/Constants.py` & `Furious-GUI-0.1.9/Furious/Utility/Constants.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.8/Furious/Utility/Process.py` & `Furious-GUI-0.1.9/Furious/Utility/Process.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.8/Furious/Utility/Proxy.py` & `Furious-GUI-0.1.9/Furious/Utility/Proxy.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.8/Furious/Utility/Resources.py` & `Furious-GUI-0.1.9/Furious/Utility/Resources.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.8/Furious/Utility/Settings.py` & `Furious-GUI-0.1.9/Furious/Utility/Settings.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.8/Furious/Utility/StartupOnBoot.py` & `Furious-GUI-0.1.9/Furious/Utility/StartupOnBoot.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.8/Furious/Utility/Theme.py` & `Furious-GUI-0.1.9/Furious/Utility/Theme.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.8/Furious/Utility/Translator.py` & `Furious-GUI-0.1.9/Furious/Utility/Translator.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.8/Furious/Utility/Utility.py` & `Furious-GUI-0.1.9/Furious/Utility/Utility.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.8/Furious/Widget/Application.py` & `Furious-GUI-0.1.9/Furious/Widget/Application.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.8/Furious/Widget/ConnectingProgressBar.py` & `Furious-GUI-0.1.9/Furious/Widget/ConnectingProgressBar.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.8/Furious/Widget/EditConfiguration.py` & `Furious-GUI-0.1.9/Furious/Widget/EditConfiguration.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.8/Furious/Widget/ExportQRCode.py` & `Furious-GUI-0.1.9/Furious/Widget/ExportQRCode.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.8/Furious/Widget/IndentSpinBox.py` & `Furious-GUI-0.1.9/Furious/Widget/IndentSpinBox.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.8/Furious/Widget/LogViewer.py` & `Furious-GUI-0.1.9/Furious/Widget/LogViewer.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.8/Furious/Widget/SystemTrayIcon.py` & `Furious-GUI-0.1.9/Furious/Widget/SystemTrayIcon.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.8/Furious/Widget/Widget.py` & `Furious-GUI-0.1.9/Furious/Widget/Widget.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.8/Furious/__main__.py` & `Furious-GUI-0.1.9/Furious/__main__.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.8/Furious_GUI.egg-info/PKG-INFO` & `Furious-GUI-0.1.9/Furious_GUI.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Furious-GUI
-Version: 0.1.8
+Version: 0.1.9
 Summary: A PySide6-based cross platform GUI client that launches your beloved GFW to outer space.
 Home-page: https://github.com/LorenEteval/Furious
 Author: Loren Eteval
 Author-email: loren.eteval@proton.me
 License: GPL v3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `Furious-GUI-0.1.8/Furious_GUI.egg-info/SOURCES.txt` & `Furious-GUI-0.1.9/Furious_GUI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.8/LICENSE` & `Furious-GUI-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.8/PKG-INFO` & `Furious-GUI-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Furious-GUI
-Version: 0.1.8
+Version: 0.1.9
 Summary: A PySide6-based cross platform GUI client that launches your beloved GFW to outer space.
 Home-page: https://github.com/LorenEteval/Furious
 Author: Loren Eteval
 Author-email: loren.eteval@proton.me
 License: GPL v3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `Furious-GUI-0.1.8/README.md` & `Furious-GUI-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.8/setup.py` & `Furious-GUI-0.1.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     install_requires=[
         'PySide6-Essentials',
         'Xray-core',
         'hysteria',
         'ujson',
         'pybase64',
         'pyqrcode',
+        'pypng',
         'sysproxy; sys_platform == "win32"',
         'darkdetect; sys_platform != "darwin"',
         'darkdetect[macos-listener]; sys_platform == "darwin"',
     ],
     entry_points={
         'gui_scripts': [
             'Furious = Furious.__main__:main',
```

