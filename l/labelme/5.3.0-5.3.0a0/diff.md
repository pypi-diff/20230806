# Comparing `tmp/labelme-5.3.0.tar.gz` & `tmp/labelme-5.3.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labelme-5.3.0.tar", last modified: Sun Aug  6 07:10:09 2023, max compression
+gzip compressed data, was "labelme-5.3.0a0.tar", last modified: Tue May 16 15:09:12 2023, max compression
```

## Comparing `labelme-5.3.0.tar` & `labelme-5.3.0a0.tar`

### file list

```diff
@@ -1,94 +1,93 @@
-drwxr-xr-x   0 wkentaro   (501) staff       (20)        0 2023-08-06 07:10:09.105866 labelme-5.3.0/
--rw-r--r--   0 wkentaro   (501) staff       (20)      692 2023-04-16 12:20:20.000000 labelme-5.3.0/LICENSE
--rw-r--r--   0 wkentaro   (501) staff       (20)       18 2023-04-16 12:20:20.000000 labelme-5.3.0/MANIFEST.in
--rw-r--r--   0 wkentaro   (501) staff       (20)    10956 2023-08-06 07:10:09.105648 labelme-5.3.0/PKG-INFO
--rw-r--r--   0 wkentaro   (501) staff       (20)     8746 2023-07-21 10:20:59.000000 labelme-5.3.0/README.md
-drwxr-xr-x   0 wkentaro   (501) staff       (20)        0 2023-08-06 07:10:09.094573 labelme-5.3.0/labelme/
--rw-r--r--   0 wkentaro   (501) staff       (20)      668 2023-08-06 07:09:48.000000 labelme-5.3.0/labelme/__init__.py
--rw-r--r--   0 wkentaro   (501) staff       (20)     5792 2023-04-16 13:33:53.000000 labelme-5.3.0/labelme/__main__.py
-drwxr-xr-x   0 wkentaro   (501) staff       (20)        0 2023-08-06 07:10:09.097124 labelme-5.3.0/labelme/ai/
--rw-r--r--   0 wkentaro   (501) staff       (20)     1804 2023-05-16 15:08:51.000000 labelme-5.3.0/labelme/ai/__init__.py
-drwxr-xr-x   0 wkentaro   (501) staff       (20)        0 2023-08-06 07:10:09.097388 labelme-5.3.0/labelme/ai/models/
--rw-r--r--   0 wkentaro   (501) staff       (20)        0 2023-05-16 15:08:51.000000 labelme-5.3.0/labelme/ai/models/__init__.py
--rw-r--r--   0 wkentaro   (501) staff       (20)     6007 2023-05-16 15:08:51.000000 labelme-5.3.0/labelme/ai/models/segment_anything.py
--rw-r--r--   0 wkentaro   (501) staff       (20)    77318 2023-05-16 15:08:51.000000 labelme-5.3.0/labelme/app.py
-drwxr-xr-x   0 wkentaro   (501) staff       (20)        0 2023-08-06 07:10:09.098121 labelme-5.3.0/labelme/cli/
--rw-r--r--   0 wkentaro   (501) staff       (20)      119 2023-08-06 07:08:10.000000 labelme-5.3.0/labelme/cli/__init__.py
--rw-r--r--   0 wkentaro   (501) staff       (20)     1345 2023-04-16 12:20:20.000000 labelme-5.3.0/labelme/cli/draw_json.py
--rw-r--r--   0 wkentaro   (501) staff       (20)      636 2023-04-16 12:20:20.000000 labelme-5.3.0/labelme/cli/draw_label_png.py
--rw-r--r--   0 wkentaro   (501) staff       (20)     2133 2023-08-06 07:08:10.000000 labelme-5.3.0/labelme/cli/export_json.py
--rw-r--r--   0 wkentaro   (501) staff       (20)     2508 2023-08-06 07:08:10.000000 labelme-5.3.0/labelme/cli/json_to_dataset.py
--rw-r--r--   0 wkentaro   (501) staff       (20)     2749 2023-04-16 12:20:20.000000 labelme-5.3.0/labelme/cli/on_docker.py
-drwxr-xr-x   0 wkentaro   (501) staff       (20)        0 2023-08-06 07:10:09.098354 labelme-5.3.0/labelme/config/
--rw-r--r--   0 wkentaro   (501) staff       (20)     2698 2023-04-16 12:20:20.000000 labelme-5.3.0/labelme/config/__init__.py
--rw-r--r--   0 wkentaro   (501) staff       (20)     2230 2023-05-16 15:08:51.000000 labelme-5.3.0/labelme/config/default_config.yaml
-drwxr-xr-x   0 wkentaro   (501) staff       (20)        0 2023-08-06 07:10:09.103523 labelme-5.3.0/labelme/icons/
--rw-r--r--   0 wkentaro   (501) staff       (20)     2136 2023-04-16 12:20:20.000000 labelme-5.3.0/labelme/icons/cancel.png
--rw-r--r--   0 wkentaro   (501) staff       (20)     3111 2023-04-16 12:20:20.000000 labelme-5.3.0/labelme/icons/close.png
--rw-r--r--   0 wkentaro   (501) staff       (20)     2368 2023-04-16 12:20:20.000000 labelme-5.3.0/labelme/icons/color-line.png
--rw-r--r--   0 wkentaro   (501) staff       (20)     1461 2023-04-16 12:20:20.000000 labelme-5.3.0/labelme/icons/color.png
--rw-r--r--   0 wkentaro   (501) staff       (20)      646 2023-04-16 12:20:20.000000 labelme-5.3.0/labelme/icons/copy.png
--rw-r--r--   0 wkentaro   (501) staff       (20)     1486 2023-04-16 12:20:20.000000 labelme-5.3.0/labelme/icons/delete.png
--rw-r--r--   0 wkentaro   (501) staff       (20)     2198 2023-04-16 12:20:20.000000 labelme-5.3.0/labelme/icons/done.png
--rw-r--r--   0 wkentaro   (501) staff       (20)    22232 2023-04-16 12:20:20.000000 labelme-5.3.0/labelme/icons/done.svg
--rw-r--r--   0 wkentaro   (501) staff       (20)     1092 2023-04-16 12:20:20.000000 labelme-5.3.0/labelme/icons/edit.png
--rw-r--r--   0 wkentaro   (501) staff       (20)     7718 2023-04-16 12:20:20.000000 labelme-5.3.0/labelme/icons/expert.png
--rw-r--r--   0 wkentaro   (501) staff       (20)     1264 2023-04-16 12:20:20.000000 labelme-5.3.0/labelme/icons/eye.png
--rw-r--r--   0 wkentaro   (501) staff       (20)     8059 2023-04-16 12:20:20.000000 labelme-5.3.0/labelme/icons/feBlend-icon.png
--rw-r--r--   0 wkentaro   (501) staff       (20)      765 2023-04-16 12:20:20.000000 labelme-5.3.0/labelme/icons/file.png
--rw-r--r--   0 wkentaro   (501) staff       (20)     1365 2023-04-16 12:20:20.000000 labelme-5.3.0/labelme/icons/fit-width.png
--rw-r--r--   0 wkentaro   (501) staff       (20)     1102 2023-04-16 12:20:20.000000 labelme-5.3.0/labelme/icons/fit-window.png
--rw-r--r--   0 wkentaro   (501) staff       (20)     2262 2023-04-16 12:20:20.000000 labelme-5.3.0/labelme/icons/fit.png
--rw-r--r--   0 wkentaro   (501) staff       (20)     1587 2023-04-16 12:20:20.000000 labelme-5.3.0/labelme/icons/help.png
--rw-r--r--   0 wkentaro   (501) staff       (20)  1128131 2023-04-16 12:20:20.000000 labelme-5.3.0/labelme/icons/icon.icns
--rw-r--r--   0 wkentaro   (501) staff       (20)   183198 2023-04-16 12:20:20.000000 labelme-5.3.0/labelme/icons/icon.ico
--rw-r--r--   0 wkentaro   (501) staff       (20)    44771 2023-08-04 11:38:25.000000 labelme-5.3.0/labelme/icons/icon.png
--rw-r--r--   0 wkentaro   (501) staff       (20)     2381 2023-04-16 12:20:20.000000 labelme-5.3.0/labelme/icons/labels.png
--rw-r--r--   0 wkentaro   (501) staff       (20)    36694 2023-04-16 12:20:20.000000 labelme-5.3.0/labelme/icons/labels.svg
--rw-r--r--   0 wkentaro   (501) staff       (20)      977 2023-04-16 12:20:20.000000 labelme-5.3.0/labelme/icons/new.png
--rw-r--r--   0 wkentaro   (501) staff       (20)    30288 2023-04-16 12:20:20.000000 labelme-5.3.0/labelme/icons/next.png
--rw-r--r--   0 wkentaro   (501) staff       (20)     1103 2023-04-16 12:20:20.000000 labelme-5.3.0/labelme/icons/objects.png
--rw-r--r--   0 wkentaro   (501) staff       (20)     2073 2023-04-16 12:20:20.000000 labelme-5.3.0/labelme/icons/open.png
--rw-r--r--   0 wkentaro   (501) staff       (20)    18197 2023-04-16 12:20:20.000000 labelme-5.3.0/labelme/icons/open.svg
--rw-r--r--   0 wkentaro   (501) staff       (20)    30665 2023-04-16 12:20:20.000000 labelme-5.3.0/labelme/icons/prev.png
--rw-r--r--   0 wkentaro   (501) staff       (20)     1915 2023-04-16 12:20:20.000000 labelme-5.3.0/labelme/icons/quit.png
--rw-r--r--   0 wkentaro   (501) staff       (20)     2811 2023-04-16 12:20:20.000000 labelme-5.3.0/labelme/icons/save-as.png
--rw-r--r--   0 wkentaro   (501) staff       (20)    64005 2023-04-16 12:20:20.000000 labelme-5.3.0/labelme/icons/save-as.svg
--rw-r--r--   0 wkentaro   (501) staff       (20)     1187 2023-04-16 12:20:20.000000 labelme-5.3.0/labelme/icons/save.png
--rw-r--r--   0 wkentaro   (501) staff       (20)    30613 2023-04-16 12:20:20.000000 labelme-5.3.0/labelme/icons/save.svg
--rw-r--r--   0 wkentaro   (501) staff       (20)     2004 2023-04-16 12:20:20.000000 labelme-5.3.0/labelme/icons/undo-cross.png
--rw-r--r--   0 wkentaro   (501) staff       (20)     2018 2023-04-16 12:20:20.000000 labelme-5.3.0/labelme/icons/undo.png
--rw-r--r--   0 wkentaro   (501) staff       (20)     1099 2023-04-16 12:20:20.000000 labelme-5.3.0/labelme/icons/zoom-in.png
--rw-r--r--   0 wkentaro   (501) staff       (20)     1074 2023-04-16 12:20:20.000000 labelme-5.3.0/labelme/icons/zoom-out.png
--rw-r--r--   0 wkentaro   (501) staff       (20)     1139 2023-04-16 12:20:20.000000 labelme-5.3.0/labelme/icons/zoom.png
--rw-r--r--   0 wkentaro   (501) staff       (20)     5809 2023-05-16 15:08:51.000000 labelme-5.3.0/labelme/label_file.py
--rw-r--r--   0 wkentaro   (501) staff       (20)     1633 2023-05-16 15:08:51.000000 labelme-5.3.0/labelme/logger.py
--rw-r--r--   0 wkentaro   (501) staff       (20)    11626 2023-05-16 15:08:51.000000 labelme-5.3.0/labelme/shape.py
--rw-r--r--   0 wkentaro   (501) staff       (20)      849 2023-04-16 12:20:20.000000 labelme-5.3.0/labelme/testing.py
-drwxr-xr-x   0 wkentaro   (501) staff       (20)        0 2023-08-06 07:10:09.104087 labelme-5.3.0/labelme/utils/
--rw-r--r--   0 wkentaro   (501) staff       (20)      755 2023-05-16 15:08:51.000000 labelme-5.3.0/labelme/utils/__init__.py
--rw-r--r--   0 wkentaro   (501) staff       (20)      675 2023-04-16 12:20:20.000000 labelme-5.3.0/labelme/utils/_io.py
--rw-r--r--   0 wkentaro   (501) staff       (20)     2619 2023-05-16 15:08:51.000000 labelme-5.3.0/labelme/utils/image.py
--rw-r--r--   0 wkentaro   (501) staff       (20)     2414 2023-05-16 15:08:51.000000 labelme-5.3.0/labelme/utils/qt.py
--rw-r--r--   0 wkentaro   (501) staff       (20)     3650 2023-04-16 12:20:20.000000 labelme-5.3.0/labelme/utils/shape.py
-drwxr-xr-x   0 wkentaro   (501) staff       (20)        0 2023-08-06 07:10:09.105462 labelme-5.3.0/labelme/widgets/
--rw-r--r--   0 wkentaro   (501) staff       (20)      510 2023-04-16 12:20:20.000000 labelme-5.3.0/labelme/widgets/__init__.py
--rw-r--r--   0 wkentaro   (501) staff       (20)     1468 2023-04-16 12:20:20.000000 labelme-5.3.0/labelme/widgets/brightness_contrast_dialog.py
--rw-r--r--   0 wkentaro   (501) staff       (20)    38987 2023-05-16 15:08:51.000000 labelme-5.3.0/labelme/widgets/canvas.py
--rw-r--r--   0 wkentaro   (501) staff       (20)     1200 2023-04-16 12:20:20.000000 labelme-5.3.0/labelme/widgets/color_dialog.py
--rw-r--r--   0 wkentaro   (501) staff       (20)      281 2023-04-16 12:20:20.000000 labelme-5.3.0/labelme/widgets/escapable_qlist_widget.py
--rw-r--r--   0 wkentaro   (501) staff       (20)     2434 2023-04-16 12:20:20.000000 labelme-5.3.0/labelme/widgets/file_dialog_preview.py
--rw-r--r--   0 wkentaro   (501) staff       (20)     8780 2023-04-16 12:20:20.000000 labelme-5.3.0/labelme/widgets/label_dialog.py
--rw-r--r--   0 wkentaro   (501) staff       (20)     5792 2023-04-16 12:20:20.000000 labelme-5.3.0/labelme/widgets/label_list_widget.py
--rw-r--r--   0 wkentaro   (501) staff       (20)      970 2023-04-16 12:20:20.000000 labelme-5.3.0/labelme/widgets/tool_bar.py
--rw-r--r--   0 wkentaro   (501) staff       (20)     1374 2023-04-16 12:20:20.000000 labelme-5.3.0/labelme/widgets/unique_label_qlist_widget.py
--rw-r--r--   0 wkentaro   (501) staff       (20)      712 2023-05-10 12:16:05.000000 labelme-5.3.0/labelme/widgets/zoom_widget.py
-drwxr-xr-x   0 wkentaro   (501) staff       (20)        0 2023-08-06 07:10:09.096984 labelme-5.3.0/labelme.egg-info/
--rw-r--r--   0 wkentaro   (501) staff       (20)    10956 2023-08-06 07:10:09.000000 labelme-5.3.0/labelme.egg-info/PKG-INFO
--rw-r--r--   0 wkentaro   (501) staff       (20)     2102 2023-08-06 07:10:09.000000 labelme-5.3.0/labelme.egg-info/SOURCES.txt
--rw-r--r--   0 wkentaro   (501) staff       (20)        1 2023-08-06 07:10:09.000000 labelme-5.3.0/labelme.egg-info/dependency_links.txt
--rw-r--r--   0 wkentaro   (501) staff       (20)      311 2023-08-06 07:10:09.000000 labelme-5.3.0/labelme.egg-info/entry_points.txt
--rw-r--r--   0 wkentaro   (501) staff       (20)      126 2023-08-06 07:10:09.000000 labelme-5.3.0/labelme.egg-info/requires.txt
--rw-r--r--   0 wkentaro   (501) staff       (20)        8 2023-08-06 07:10:09.000000 labelme-5.3.0/labelme.egg-info/top_level.txt
--rw-r--r--   0 wkentaro   (501) staff       (20)       38 2023-08-06 07:10:09.105907 labelme-5.3.0/setup.cfg
--rw-r--r--   0 wkentaro   (501) staff       (20)     4673 2023-08-06 07:08:10.000000 labelme-5.3.0/setup.py
+drwxr-xr-x   0 wkentaro   (501) staff       (20)        0 2023-05-16 15:09:12.209357 labelme-5.3.0a0/
+-rw-r--r--   0 wkentaro   (501) staff       (20)      692 2023-04-16 12:20:20.000000 labelme-5.3.0a0/LICENSE
+-rw-r--r--   0 wkentaro   (501) staff       (20)       18 2023-04-16 12:20:20.000000 labelme-5.3.0a0/MANIFEST.in
+-rw-r--r--   0 wkentaro   (501) staff       (20)    10958 2023-05-16 15:09:12.209162 labelme-5.3.0a0/PKG-INFO
+-rw-r--r--   0 wkentaro   (501) staff       (20)     8746 2023-04-16 12:20:20.000000 labelme-5.3.0a0/README.md
+drwxr-xr-x   0 wkentaro   (501) staff       (20)        0 2023-05-16 15:09:12.200081 labelme-5.3.0a0/labelme/
+-rw-r--r--   0 wkentaro   (501) staff       (20)      670 2023-05-16 15:08:59.000000 labelme-5.3.0a0/labelme/__init__.py
+-rw-r--r--   0 wkentaro   (501) staff       (20)     5792 2023-04-16 13:33:53.000000 labelme-5.3.0a0/labelme/__main__.py
+drwxr-xr-x   0 wkentaro   (501) staff       (20)        0 2023-05-16 15:09:12.200959 labelme-5.3.0a0/labelme/ai/
+-rw-r--r--   0 wkentaro   (501) staff       (20)     1804 2023-05-16 15:08:51.000000 labelme-5.3.0a0/labelme/ai/__init__.py
+drwxr-xr-x   0 wkentaro   (501) staff       (20)        0 2023-05-16 15:09:12.201178 labelme-5.3.0a0/labelme/ai/models/
+-rw-r--r--   0 wkentaro   (501) staff       (20)        0 2023-05-16 15:08:51.000000 labelme-5.3.0a0/labelme/ai/models/__init__.py
+-rw-r--r--   0 wkentaro   (501) staff       (20)     6007 2023-05-16 15:08:51.000000 labelme-5.3.0a0/labelme/ai/models/segment_anything.py
+-rw-r--r--   0 wkentaro   (501) staff       (20)    77318 2023-05-16 15:08:51.000000 labelme-5.3.0a0/labelme/app.py
+drwxr-xr-x   0 wkentaro   (501) staff       (20)        0 2023-05-16 15:09:12.201743 labelme-5.3.0a0/labelme/cli/
+-rw-r--r--   0 wkentaro   (501) staff       (20)      123 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/cli/__init__.py
+-rw-r--r--   0 wkentaro   (501) staff       (20)     1345 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/cli/draw_json.py
+-rw-r--r--   0 wkentaro   (501) staff       (20)      636 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/cli/draw_label_png.py
+-rw-r--r--   0 wkentaro   (501) staff       (20)     2388 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/cli/json_to_dataset.py
+-rw-r--r--   0 wkentaro   (501) staff       (20)     2749 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/cli/on_docker.py
+drwxr-xr-x   0 wkentaro   (501) staff       (20)        0 2023-05-16 15:09:12.202037 labelme-5.3.0a0/labelme/config/
+-rw-r--r--   0 wkentaro   (501) staff       (20)     2698 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/config/__init__.py
+-rw-r--r--   0 wkentaro   (501) staff       (20)     2230 2023-05-16 15:08:51.000000 labelme-5.3.0a0/labelme/config/default_config.yaml
+drwxr-xr-x   0 wkentaro   (501) staff       (20)        0 2023-05-16 15:09:12.207135 labelme-5.3.0a0/labelme/icons/
+-rw-r--r--   0 wkentaro   (501) staff       (20)     2136 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/cancel.png
+-rw-r--r--   0 wkentaro   (501) staff       (20)     3111 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/close.png
+-rw-r--r--   0 wkentaro   (501) staff       (20)     2368 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/color-line.png
+-rw-r--r--   0 wkentaro   (501) staff       (20)     1461 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/color.png
+-rw-r--r--   0 wkentaro   (501) staff       (20)      646 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/copy.png
+-rw-r--r--   0 wkentaro   (501) staff       (20)     1486 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/delete.png
+-rw-r--r--   0 wkentaro   (501) staff       (20)     2198 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/done.png
+-rw-r--r--   0 wkentaro   (501) staff       (20)    22232 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/done.svg
+-rw-r--r--   0 wkentaro   (501) staff       (20)     1092 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/edit.png
+-rw-r--r--   0 wkentaro   (501) staff       (20)     7718 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/expert.png
+-rw-r--r--   0 wkentaro   (501) staff       (20)     1264 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/eye.png
+-rw-r--r--   0 wkentaro   (501) staff       (20)     8059 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/feBlend-icon.png
+-rw-r--r--   0 wkentaro   (501) staff       (20)      765 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/file.png
+-rw-r--r--   0 wkentaro   (501) staff       (20)     1365 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/fit-width.png
+-rw-r--r--   0 wkentaro   (501) staff       (20)     1102 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/fit-window.png
+-rw-r--r--   0 wkentaro   (501) staff       (20)     2262 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/fit.png
+-rw-r--r--   0 wkentaro   (501) staff       (20)     1587 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/help.png
+-rw-r--r--   0 wkentaro   (501) staff       (20)  1128131 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/icon.icns
+-rw-r--r--   0 wkentaro   (501) staff       (20)   183198 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/icon.ico
+-rw-r--r--   0 wkentaro   (501) staff       (20)    44771 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/icon.png
+-rw-r--r--   0 wkentaro   (501) staff       (20)     2381 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/labels.png
+-rw-r--r--   0 wkentaro   (501) staff       (20)    36694 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/labels.svg
+-rw-r--r--   0 wkentaro   (501) staff       (20)      977 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/new.png
+-rw-r--r--   0 wkentaro   (501) staff       (20)    30288 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/next.png
+-rw-r--r--   0 wkentaro   (501) staff       (20)     1103 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/objects.png
+-rw-r--r--   0 wkentaro   (501) staff       (20)     2073 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/open.png
+-rw-r--r--   0 wkentaro   (501) staff       (20)    18197 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/open.svg
+-rw-r--r--   0 wkentaro   (501) staff       (20)    30665 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/prev.png
+-rw-r--r--   0 wkentaro   (501) staff       (20)     1915 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/quit.png
+-rw-r--r--   0 wkentaro   (501) staff       (20)     2811 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/save-as.png
+-rw-r--r--   0 wkentaro   (501) staff       (20)    64005 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/save-as.svg
+-rw-r--r--   0 wkentaro   (501) staff       (20)     1187 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/save.png
+-rw-r--r--   0 wkentaro   (501) staff       (20)    30613 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/save.svg
+-rw-r--r--   0 wkentaro   (501) staff       (20)     2004 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/undo-cross.png
+-rw-r--r--   0 wkentaro   (501) staff       (20)     2018 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/undo.png
+-rw-r--r--   0 wkentaro   (501) staff       (20)     1099 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/zoom-in.png
+-rw-r--r--   0 wkentaro   (501) staff       (20)     1074 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/zoom-out.png
+-rw-r--r--   0 wkentaro   (501) staff       (20)     1139 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/icons/zoom.png
+-rw-r--r--   0 wkentaro   (501) staff       (20)     5809 2023-05-16 15:08:51.000000 labelme-5.3.0a0/labelme/label_file.py
+-rw-r--r--   0 wkentaro   (501) staff       (20)     1633 2023-05-16 15:08:51.000000 labelme-5.3.0a0/labelme/logger.py
+-rw-r--r--   0 wkentaro   (501) staff       (20)    11626 2023-05-16 15:08:51.000000 labelme-5.3.0a0/labelme/shape.py
+-rw-r--r--   0 wkentaro   (501) staff       (20)      849 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/testing.py
+drwxr-xr-x   0 wkentaro   (501) staff       (20)        0 2023-05-16 15:09:12.207700 labelme-5.3.0a0/labelme/utils/
+-rw-r--r--   0 wkentaro   (501) staff       (20)      755 2023-05-16 15:08:51.000000 labelme-5.3.0a0/labelme/utils/__init__.py
+-rw-r--r--   0 wkentaro   (501) staff       (20)      675 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/utils/_io.py
+-rw-r--r--   0 wkentaro   (501) staff       (20)     2619 2023-05-16 15:08:51.000000 labelme-5.3.0a0/labelme/utils/image.py
+-rw-r--r--   0 wkentaro   (501) staff       (20)     2414 2023-05-16 15:08:51.000000 labelme-5.3.0a0/labelme/utils/qt.py
+-rw-r--r--   0 wkentaro   (501) staff       (20)     3650 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/utils/shape.py
+drwxr-xr-x   0 wkentaro   (501) staff       (20)        0 2023-05-16 15:09:12.208980 labelme-5.3.0a0/labelme/widgets/
+-rw-r--r--   0 wkentaro   (501) staff       (20)      510 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/widgets/__init__.py
+-rw-r--r--   0 wkentaro   (501) staff       (20)     1468 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/widgets/brightness_contrast_dialog.py
+-rw-r--r--   0 wkentaro   (501) staff       (20)    38987 2023-05-16 15:08:51.000000 labelme-5.3.0a0/labelme/widgets/canvas.py
+-rw-r--r--   0 wkentaro   (501) staff       (20)     1200 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/widgets/color_dialog.py
+-rw-r--r--   0 wkentaro   (501) staff       (20)      281 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/widgets/escapable_qlist_widget.py
+-rw-r--r--   0 wkentaro   (501) staff       (20)     2434 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/widgets/file_dialog_preview.py
+-rw-r--r--   0 wkentaro   (501) staff       (20)     8780 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/widgets/label_dialog.py
+-rw-r--r--   0 wkentaro   (501) staff       (20)     5792 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/widgets/label_list_widget.py
+-rw-r--r--   0 wkentaro   (501) staff       (20)      970 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/widgets/tool_bar.py
+-rw-r--r--   0 wkentaro   (501) staff       (20)     1374 2023-04-16 12:20:20.000000 labelme-5.3.0a0/labelme/widgets/unique_label_qlist_widget.py
+-rw-r--r--   0 wkentaro   (501) staff       (20)      712 2023-05-10 12:16:05.000000 labelme-5.3.0a0/labelme/widgets/zoom_widget.py
+drwxr-xr-x   0 wkentaro   (501) staff       (20)        0 2023-05-16 15:09:12.200841 labelme-5.3.0a0/labelme.egg-info/
+-rw-r--r--   0 wkentaro   (501) staff       (20)    10958 2023-05-16 15:09:12.000000 labelme-5.3.0a0/labelme.egg-info/PKG-INFO
+-rw-r--r--   0 wkentaro   (501) staff       (20)     2075 2023-05-16 15:09:12.000000 labelme-5.3.0a0/labelme.egg-info/SOURCES.txt
+-rw-r--r--   0 wkentaro   (501) staff       (20)        1 2023-05-16 15:09:12.000000 labelme-5.3.0a0/labelme.egg-info/dependency_links.txt
+-rw-r--r--   0 wkentaro   (501) staff       (20)      260 2023-05-16 15:09:12.000000 labelme-5.3.0a0/labelme.egg-info/entry_points.txt
+-rw-r--r--   0 wkentaro   (501) staff       (20)      126 2023-05-16 15:09:12.000000 labelme-5.3.0a0/labelme.egg-info/requires.txt
+-rw-r--r--   0 wkentaro   (501) staff       (20)        8 2023-05-16 15:09:12.000000 labelme-5.3.0a0/labelme.egg-info/top_level.txt
+-rw-r--r--   0 wkentaro   (501) staff       (20)       38 2023-05-16 15:09:12.209433 labelme-5.3.0a0/setup.cfg
+-rw-r--r--   0 wkentaro   (501) staff       (20)     4605 2023-05-16 15:08:51.000000 labelme-5.3.0a0/setup.py
```

### Comparing `labelme-5.3.0/LICENSE` & `labelme-5.3.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `labelme-5.3.0/PKG-INFO` & `labelme-5.3.0a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labelme
-Version: 5.3.0
+Version: 5.3.0a0
 Summary: Image Polygonal Annotation with Python
 Home-page: https://github.com/wkentaro/labelme
 Author: Kentaro Wada
 Author-email: www.kentaro.wada@gmail.com
 License: GPLv3
 Keywords: Image Annotation,Machine Learning
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: labelme Version: 5.3.0 Summary: Image Polygonal
+Metadata-Version: 2.1 Name: labelme Version: 5.3.0a0 Summary: Image Polygonal
 Annotation with Python Home-page: https://github.com/wkentaro/labelme Author:
 Kentaro Wada Author-email: www.kentaro.wada@gmail.com License: GPLv3 Keywords:
 Image Annotation,Machine Learning Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Science/Research Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python Classifier: Programming Language :: Python :: 3.5 Classifier:
```

### Comparing `labelme-5.3.0/README.md` & `labelme-5.3.0a0/README.md`

 * *Files identical despite different names*

### Comparing `labelme-5.3.0/labelme/__init__.py` & `labelme-5.3.0a0/labelme/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 __appname__ = "labelme"
 
 # Semantic Versioning 2.0.0: https://semver.org/
 # 1. MAJOR version when you make incompatible API changes;
 # 2. MINOR version when you add functionality in a backwards-compatible manner;
 # 3. PATCH version when you make backwards-compatible bug fixes.
 # e.g., 1.0.0a0, 1.0.0a1, 1.0.0b0, 1.0.0rc0, 1.0.0, 1.0.0.post0
-__version__ = "5.3.0"
+__version__ = "5.3.0a0"
 
 QT4 = QT_VERSION[0] == "4"
 QT5 = QT_VERSION[0] == "5"
 del QT_VERSION
 
 PY2 = sys.version[0] == "2"
 PY3 = sys.version[0] == "3"
```

### Comparing `labelme-5.3.0/labelme/__main__.py` & `labelme-5.3.0a0/labelme/__main__.py`

 * *Files identical despite different names*

### Comparing `labelme-5.3.0/labelme/ai/__init__.py` & `labelme-5.3.0a0/labelme/ai/__init__.py`

 * *Files identical despite different names*

### Comparing `labelme-5.3.0/labelme/ai/models/segment_anything.py` & `labelme-5.3.0a0/labelme/ai/models/segment_anything.py`

 * *Files identical despite different names*

### Comparing `labelme-5.3.0/labelme/app.py` & `labelme-5.3.0a0/labelme/app.py`

 * *Files identical despite different names*

### Comparing `labelme-5.3.0/labelme/cli/draw_json.py` & `labelme-5.3.0a0/labelme/cli/draw_json.py`

 * *Files identical despite different names*

### Comparing `labelme-5.3.0/labelme/cli/draw_label_png.py` & `labelme-5.3.0a0/labelme/cli/draw_label_png.py`

 * *Files identical despite different names*

### Comparing `labelme-5.3.0/labelme/cli/export_json.py` & `labelme-5.3.0a0/labelme/cli/json_to_dataset.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,14 +8,23 @@
 import PIL.Image
 
 from labelme.logger import logger
 from labelme import utils
 
 
 def main():
+    logger.warning(
+        "This script is aimed to demonstrate how to convert the "
+        "JSON file to a single image dataset."
+    )
+    logger.warning(
+        "It won't handle multiple JSON files to generate a "
+        "real-use dataset."
+    )
+
     parser = argparse.ArgumentParser()
     parser.add_argument("json_file")
     parser.add_argument("-o", "--out", default=None)
     args = parser.parse_args()
 
     json_file = args.json_file
```

### Comparing `labelme-5.3.0/labelme/cli/on_docker.py` & `labelme-5.3.0a0/labelme/cli/on_docker.py`

 * *Files identical despite different names*

### Comparing `labelme-5.3.0/labelme/config/__init__.py` & `labelme-5.3.0a0/labelme/config/__init__.py`

 * *Files identical despite different names*

### Comparing `labelme-5.3.0/labelme/config/default_config.yaml` & `labelme-5.3.0a0/labelme/config/default_config.yaml`

 * *Files identical despite different names*

### Comparing `labelme-5.3.0/labelme/icons/cancel.png` & `labelme-5.3.0a0/labelme/icons/cancel.png`

 * *Files identical despite different names*

### Comparing `labelme-5.3.0/labelme/icons/close.png` & `labelme-5.3.0a0/labelme/icons/close.png`

 * *Files identical despite different names*

### Comparing `labelme-5.3.0/labelme/icons/color-line.png` & `labelme-5.3.0a0/labelme/icons/color-line.png`

 * *Files identical despite different names*

### Comparing `labelme-5.3.0/labelme/icons/color.png` & `labelme-5.3.0a0/labelme/icons/color.png`

 * *Files identical despite different names*

### Comparing `labelme-5.3.0/labelme/icons/copy.png` & `labelme-5.3.0a0/labelme/icons/copy.png`

 * *Files identical despite different names*

### Comparing `labelme-5.3.0/labelme/icons/delete.png` & `labelme-5.3.0a0/labelme/icons/delete.png`

 * *Files identical despite different names*

### Comparing `labelme-5.3.0/labelme/icons/done.png` & `labelme-5.3.0a0/labelme/icons/done.png`

 * *Files identical despite different names*

### Comparing `labelme-5.3.0/labelme/icons/done.svg` & `labelme-5.3.0a0/labelme/icons/done.svg`

 * *Files identical despite different names*

### Comparing `labelme-5.3.0/labelme/icons/edit.png` & `labelme-5.3.0a0/labelme/icons/edit.png`

 * *Files identical despite different names*

### Comparing `labelme-5.3.0/labelme/icons/expert.png` & `labelme-5.3.0a0/labelme/icons/expert.png`

 * *Files identical despite different names*

### Comparing `labelme-5.3.0/labelme/icons/eye.png` & `labelme-5.3.0a0/labelme/icons/eye.png`

 * *Files identical despite different names*

### Comparing `labelme-5.3.0/labelme/icons/feBlend-icon.png` & `labelme-5.3.0a0/labelme/icons/feBlend-icon.png`

 * *Files identical despite different names*

### Comparing `labelme-5.3.0/labelme/icons/file.png` & `labelme-5.3.0a0/labelme/icons/file.png`

 * *Files identical despite different names*

### Comparing `labelme-5.3.0/labelme/icons/fit-width.png` & `labelme-5.3.0a0/labelme/icons/fit-width.png`

 * *Files identical despite different names*

### Comparing `labelme-5.3.0/labelme/icons/fit-window.png` & `labelme-5.3.0a0/labelme/icons/fit-window.png`

 * *Files identical despite different names*

### Comparing `labelme-5.3.0/labelme/icons/fit.png` & `labelme-5.3.0a0/labelme/icons/fit.png`

 * *Files identical despite different names*

### Comparing `labelme-5.3.0/labelme/icons/help.png` & `labelme-5.3.0a0/labelme/icons/help.png`

 * *Files identical despite different names*

### Comparing `labelme-5.3.0/labelme/icons/icon.icns` & `labelme-5.3.0a0/labelme/icons/icon.icns`

 * *Files identical despite different names*

### Comparing `labelme-5.3.0/labelme/icons/icon.ico` & `labelme-5.3.0a0/labelme/icons/icon.ico`

 * *Files identical despite different names*

### Comparing `labelme-5.3.0/labelme/icons/icon.png` & `labelme-5.3.0a0/labelme/icons/icon.png`

 * *Files identical despite different names*

### Comparing `labelme-5.3.0/labelme/icons/labels.png` & `labelme-5.3.0a0/labelme/icons/labels.png`

 * *Files identical despite different names*

### Comparing `labelme-5.3.0/labelme/icons/labels.svg` & `labelme-5.3.0a0/labelme/icons/labels.svg`

 * *Files identical despite different names*

### Comparing `labelme-5.3.0/labelme/icons/new.png` & `labelme-5.3.0a0/labelme/icons/new.png`

 * *Files identical despite different names*

### Comparing `labelme-5.3.0/labelme/icons/next.png` & `labelme-5.3.0a0/labelme/icons/next.png`

 * *Files identical despite different names*

### Comparing `labelme-5.3.0/labelme/icons/objects.png` & `labelme-5.3.0a0/labelme/icons/objects.png`

 * *Files identical despite different names*

### Comparing `labelme-5.3.0/labelme/icons/open.png` & `labelme-5.3.0a0/labelme/icons/open.png`

 * *Files identical despite different names*

### Comparing `labelme-5.3.0/labelme/icons/open.svg` & `labelme-5.3.0a0/labelme/icons/open.svg`

 * *Files identical despite different names*

### Comparing `labelme-5.3.0/labelme/icons/prev.png` & `labelme-5.3.0a0/labelme/icons/prev.png`

 * *Files identical despite different names*

### Comparing `labelme-5.3.0/labelme/icons/quit.png` & `labelme-5.3.0a0/labelme/icons/quit.png`

 * *Files identical despite different names*

### Comparing `labelme-5.3.0/labelme/icons/save-as.png` & `labelme-5.3.0a0/labelme/icons/save-as.png`

 * *Files identical despite different names*

### Comparing `labelme-5.3.0/labelme/icons/save-as.svg` & `labelme-5.3.0a0/labelme/icons/save-as.svg`

 * *Files identical despite different names*

### Comparing `labelme-5.3.0/labelme/icons/save.png` & `labelme-5.3.0a0/labelme/icons/save.png`

 * *Files identical despite different names*

### Comparing `labelme-5.3.0/labelme/icons/save.svg` & `labelme-5.3.0a0/labelme/icons/save.svg`

 * *Files identical despite different names*

### Comparing `labelme-5.3.0/labelme/icons/undo-cross.png` & `labelme-5.3.0a0/labelme/icons/undo-cross.png`

 * *Files identical despite different names*

### Comparing `labelme-5.3.0/labelme/icons/undo.png` & `labelme-5.3.0a0/labelme/icons/undo.png`

 * *Files identical despite different names*

### Comparing `labelme-5.3.0/labelme/icons/zoom-in.png` & `labelme-5.3.0a0/labelme/icons/zoom-in.png`

 * *Files identical despite different names*

### Comparing `labelme-5.3.0/labelme/icons/zoom-out.png` & `labelme-5.3.0a0/labelme/icons/zoom-out.png`

 * *Files identical despite different names*

### Comparing `labelme-5.3.0/labelme/icons/zoom.png` & `labelme-5.3.0a0/labelme/icons/zoom.png`

 * *Files identical despite different names*

### Comparing `labelme-5.3.0/labelme/label_file.py` & `labelme-5.3.0a0/labelme/label_file.py`

 * *Files identical despite different names*

### Comparing `labelme-5.3.0/labelme/logger.py` & `labelme-5.3.0a0/labelme/logger.py`

 * *Files identical despite different names*

### Comparing `labelme-5.3.0/labelme/shape.py` & `labelme-5.3.0a0/labelme/shape.py`

 * *Files identical despite different names*

### Comparing `labelme-5.3.0/labelme/testing.py` & `labelme-5.3.0a0/labelme/testing.py`

 * *Files identical despite different names*

### Comparing `labelme-5.3.0/labelme/utils/__init__.py` & `labelme-5.3.0a0/labelme/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `labelme-5.3.0/labelme/utils/_io.py` & `labelme-5.3.0a0/labelme/utils/_io.py`

 * *Files identical despite different names*

### Comparing `labelme-5.3.0/labelme/utils/image.py` & `labelme-5.3.0a0/labelme/utils/image.py`

 * *Files identical despite different names*

### Comparing `labelme-5.3.0/labelme/utils/qt.py` & `labelme-5.3.0a0/labelme/utils/qt.py`

 * *Files identical despite different names*

### Comparing `labelme-5.3.0/labelme/utils/shape.py` & `labelme-5.3.0a0/labelme/utils/shape.py`

 * *Files identical despite different names*

### Comparing `labelme-5.3.0/labelme/widgets/brightness_contrast_dialog.py` & `labelme-5.3.0a0/labelme/widgets/brightness_contrast_dialog.py`

 * *Files identical despite different names*

### Comparing `labelme-5.3.0/labelme/widgets/canvas.py` & `labelme-5.3.0a0/labelme/widgets/canvas.py`

 * *Files identical despite different names*

### Comparing `labelme-5.3.0/labelme/widgets/color_dialog.py` & `labelme-5.3.0a0/labelme/widgets/color_dialog.py`

 * *Files identical despite different names*

### Comparing `labelme-5.3.0/labelme/widgets/file_dialog_preview.py` & `labelme-5.3.0a0/labelme/widgets/file_dialog_preview.py`

 * *Files identical despite different names*

### Comparing `labelme-5.3.0/labelme/widgets/label_dialog.py` & `labelme-5.3.0a0/labelme/widgets/label_dialog.py`

 * *Files identical despite different names*

### Comparing `labelme-5.3.0/labelme/widgets/label_list_widget.py` & `labelme-5.3.0a0/labelme/widgets/label_list_widget.py`

 * *Files identical despite different names*

### Comparing `labelme-5.3.0/labelme/widgets/tool_bar.py` & `labelme-5.3.0a0/labelme/widgets/tool_bar.py`

 * *Files identical despite different names*

### Comparing `labelme-5.3.0/labelme/widgets/unique_label_qlist_widget.py` & `labelme-5.3.0a0/labelme/widgets/unique_label_qlist_widget.py`

 * *Files identical despite different names*

### Comparing `labelme-5.3.0/labelme/widgets/zoom_widget.py` & `labelme-5.3.0a0/labelme/widgets/zoom_widget.py`

 * *Files identical despite different names*

### Comparing `labelme-5.3.0/labelme.egg-info/PKG-INFO` & `labelme-5.3.0a0/labelme.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labelme
-Version: 5.3.0
+Version: 5.3.0a0
 Summary: Image Polygonal Annotation with Python
 Home-page: https://github.com/wkentaro/labelme
 Author: Kentaro Wada
 Author-email: www.kentaro.wada@gmail.com
 License: GPLv3
 Keywords: Image Annotation,Machine Learning
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: labelme Version: 5.3.0 Summary: Image Polygonal
+Metadata-Version: 2.1 Name: labelme Version: 5.3.0a0 Summary: Image Polygonal
 Annotation with Python Home-page: https://github.com/wkentaro/labelme Author:
 Kentaro Wada Author-email: www.kentaro.wada@gmail.com License: GPLv3 Keywords:
 Image Annotation,Machine Learning Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Science/Research Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python Classifier: Programming Language :: Python :: 3.5 Classifier:
```

### Comparing `labelme-5.3.0/labelme.egg-info/SOURCES.txt` & `labelme-5.3.0a0/labelme.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 labelme.egg-info/top_level.txt
 labelme/ai/__init__.py
 labelme/ai/models/__init__.py
 labelme/ai/models/segment_anything.py
 labelme/cli/__init__.py
 labelme/cli/draw_json.py
 labelme/cli/draw_label_png.py
-labelme/cli/export_json.py
 labelme/cli/json_to_dataset.py
 labelme/cli/on_docker.py
 labelme/config/__init__.py
 labelme/config/default_config.yaml
 labelme/icons/cancel.png
 labelme/icons/close.png
 labelme/icons/color-line.png
```

### Comparing `labelme-5.3.0/setup.py` & `labelme-5.3.0a0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -147,15 +147,14 @@
         package_data={"labelme": ["icons/*", "config/*.yaml"]},
         entry_points={
             "console_scripts": [
                 "labelme=labelme.__main__:main",
                 "labelme_draw_json=labelme.cli.draw_json:main",
                 "labelme_draw_label_png=labelme.cli.draw_label_png:main",
                 "labelme_json_to_dataset=labelme.cli.json_to_dataset:main",
-                "labelme_export_json=labelme.cli.export_json:main",
                 "labelme_on_docker=labelme.cli.on_docker:main",
             ],
         },
     )
 
 
 if __name__ == "__main__":
```

