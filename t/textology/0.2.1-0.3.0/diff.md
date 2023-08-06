# Comparing `tmp/textology-0.2.1.tar.gz` & `tmp/textology-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textology-0.2.1.tar", last modified: Sun Jul 30 17:55:13 2023, max compression
+gzip compressed data, was "textology-0.3.0.tar", last modified: Sun Aug  6 20:25:34 2023, max compression
```

## Comparing `textology-0.2.1.tar` & `textology-0.3.0.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2023-07-30 17:55:13.555223 textology-0.2.1/
--rw-r--r--   0 dfritz     (502) staff       (20)     1068 2023-07-01 18:44:36.000000 textology-0.2.1/LICENSE
--rw-r--r--   0 dfritz     (502) staff       (20)       97 2023-07-08 19:46:35.000000 textology-0.2.1/MANIFEST.in
--rw-r--r--   0 dfritz     (502) staff       (20)    15574 2023-07-30 17:55:13.555421 textology-0.2.1/PKG-INFO
--rw-r--r--   0 dfritz     (502) staff       (20)    14212 2023-07-30 17:52:28.000000 textology-0.2.1/README.md
--rw-r--r--   0 dfritz     (502) staff       (20)       34 2023-07-30 17:52:28.000000 textology-0.2.1/requirements-dev.txt
--rw-r--r--   0 dfritz     (502) staff       (20)      168 2023-07-08 19:46:35.000000 textology-0.2.1/requirements-full-dev.txt
--rw-r--r--   0 dfritz     (502) staff       (20)       16 2023-07-30 17:52:28.000000 textology-0.2.1/requirements.txt
--rw-r--r--   0 dfritz     (502) staff       (20)     1667 2023-07-30 17:55:13.556658 textology-0.2.1/setup.cfg
--rw-r--r--   0 dfritz     (502) staff       (20)     3225 2023-07-08 19:46:35.000000 textology-0.2.1/setup.py
-drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2023-07-30 17:55:13.514102 textology-0.2.1/textology/
--rw-r--r--   0 dfritz     (502) staff       (20)       69 2023-07-30 17:52:28.000000 textology-0.2.1/textology/__init__.py
--rw-r--r--   0 dfritz     (502) staff       (20)    16797 2023-07-24 01:09:35.000000 textology-0.2.1/textology/apps.py
--rw-r--r--   0 dfritz     (502) staff       (20)     6108 2023-07-24 01:09:35.000000 textology-0.2.1/textology/dash_compat.py
--rw-r--r--   0 dfritz     (502) staff       (20)     2772 2023-07-04 21:19:10.000000 textology-0.2.1/textology/history.py
--rw-r--r--   0 dfritz     (502) staff       (20)      492 2023-07-04 21:19:10.000000 textology-0.2.1/textology/logging.py
-drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2023-07-30 17:55:13.524380 textology-0.2.1/textology/observers/
--rw-r--r--   0 dfritz     (502) staff       (20)      885 2023-07-24 01:09:35.000000 textology-0.2.1/textology/observers/__init__.py
--rw-r--r--   0 dfritz     (502) staff       (20)     6230 2023-07-24 01:09:35.000000 textology-0.2.1/textology/observers/_dependencies.py
--rw-r--r--   0 dfritz     (502) staff       (20)      458 2023-07-22 18:13:02.000000 textology-0.2.1/textology/observers/_exceptions.py
--rw-r--r--   0 dfritz     (502) staff       (20)    31200 2023-07-24 01:09:35.000000 textology-0.2.1/textology/observers/_managers.py
--rw-r--r--   0 dfritz     (502) staff       (20)     5473 2023-07-24 01:09:35.000000 textology-0.2.1/textology/pages.py
--rw-r--r--   0 dfritz     (502) staff       (20)    16541 2023-07-16 17:16:06.000000 textology-0.2.1/textology/pytest_utils.py
--rw-r--r--   0 dfritz     (502) staff       (20)    17773 2023-07-16 17:16:06.000000 textology-0.2.1/textology/router.py
--rw-r--r--   0 dfritz     (502) staff       (20)    45559 2023-07-24 01:09:35.000000 textology-0.2.1/textology/test-template.html
-drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2023-07-30 17:55:13.536001 textology-0.2.1/textology/widgets/
--rw-r--r--   0 dfritz     (502) staff       (20)     2701 2023-07-30 17:52:28.000000 textology-0.2.1/textology/widgets/__init__.py
--rw-r--r--   0 dfritz     (502) staff       (20)     1712 2023-07-04 21:18:52.000000 textology-0.2.1/textology/widgets/_button.py
--rw-r--r--   0 dfritz     (502) staff       (20)    12809 2023-07-30 17:52:28.000000 textology-0.2.1/textology/widgets/_extensions.py
--rw-r--r--   0 dfritz     (502) staff       (20)    11892 2023-07-16 17:16:06.000000 textology-0.2.1/textology/widgets/_horizontal_menus.py
--rw-r--r--   0 dfritz     (502) staff       (20)     2274 2023-07-30 17:52:28.000000 textology-0.2.1/textology/widgets/_list_item.py
--rw-r--r--   0 dfritz     (502) staff       (20)     1992 2023-07-08 19:46:35.000000 textology-0.2.1/textology/widgets/_list_item_header.py
--rw-r--r--   0 dfritz     (502) staff       (20)     1993 2023-07-16 17:16:06.000000 textology-0.2.1/textology/widgets/_list_item_meta.py
--rw-r--r--   0 dfritz     (502) staff       (20)     4919 2023-07-04 21:18:52.000000 textology-0.2.1/textology/widgets/_list_view.py
--rw-r--r--   0 dfritz     (502) staff       (20)     8735 2023-07-30 17:52:28.000000 textology-0.2.1/textology/widgets/_location.py
--rw-r--r--   0 dfritz     (502) staff       (20)     1955 2023-07-04 21:18:52.000000 textology-0.2.1/textology/widgets/_modal_dialog.py
--rw-r--r--   0 dfritz     (502) staff       (20)     2014 2023-07-30 17:52:28.000000 textology-0.2.1/textology/widgets/_store.py
-drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2023-07-30 17:55:13.554785 textology-0.2.1/textology/widgets/_textual/
--rw-r--r--   0 dfritz     (502) staff       (20)      104 2023-07-30 17:52:28.000000 textology-0.2.1/textology/widgets/_textual/__init__.py
--rw-r--r--   0 dfritz     (502) staff       (20)      294 2023-07-30 17:52:28.000000 textology-0.2.1/textology/widgets/_textual/_checkbox.py
--rw-r--r--   0 dfritz     (502) staff       (20)     1651 2023-07-30 17:52:28.000000 textology-0.2.1/textology/widgets/_textual/_containers.py
--rw-r--r--   0 dfritz     (502) staff       (20)     1600 2023-07-30 17:52:28.000000 textology-0.2.1/textology/widgets/_textual/_content_switcher.py
--rw-r--r--   0 dfritz     (502) staff       (20)     2691 2023-07-30 17:52:28.000000 textology-0.2.1/textology/widgets/_textual/_data_table.py
--rw-r--r--   0 dfritz     (502) staff       (20)     1306 2023-07-30 17:52:28.000000 textology-0.2.1/textology/widgets/_textual/_directory_tree.py
--rw-r--r--   0 dfritz     (502) staff       (20)      630 2023-07-30 17:52:28.000000 textology-0.2.1/textology/widgets/_textual/_footer.py
--rw-r--r--   0 dfritz     (502) staff       (20)      979 2023-07-30 17:52:28.000000 textology-0.2.1/textology/widgets/_textual/_header.py
--rw-r--r--   0 dfritz     (502) staff       (20)      291 2023-07-30 17:52:28.000000 textology-0.2.1/textology/widgets/_textual/_label.py
--rw-r--r--   0 dfritz     (502) staff       (20)      263 2023-07-30 17:52:28.000000 textology-0.2.1/textology/widgets/_textual/_loading_indicator.py
--rw-r--r--   0 dfritz     (502) staff       (20)     2778 2023-07-30 17:52:28.000000 textology-0.2.1/textology/widgets/_textual/_markdown.py
--rw-r--r--   0 dfritz     (502) staff       (20)     1259 2023-07-30 17:52:28.000000 textology-0.2.1/textology/widgets/_textual/_option_list.py
--rw-r--r--   0 dfritz     (502) staff       (20)     1076 2023-07-30 17:52:28.000000 textology-0.2.1/textology/widgets/_textual/_pretty.py
--rw-r--r--   0 dfritz     (502) staff       (20)     1621 2023-07-30 17:52:28.000000 textology-0.2.1/textology/widgets/_textual/_progress_bar.py
--rw-r--r--   0 dfritz     (502) staff       (20)      308 2023-07-30 17:52:28.000000 textology-0.2.1/textology/widgets/_textual/_radio_button.py
--rw-r--r--   0 dfritz     (502) staff       (20)     1213 2023-07-30 17:52:28.000000 textology-0.2.1/textology/widgets/_textual/_radio_set.py
--rw-r--r--   0 dfritz     (502) staff       (20)     1673 2023-07-30 17:52:28.000000 textology-0.2.1/textology/widgets/_textual/_select.py
--rw-r--r--   0 dfritz     (502) staff       (20)     1488 2023-07-30 17:52:28.000000 textology-0.2.1/textology/widgets/_textual/_selection_list.py
--rw-r--r--   0 dfritz     (502) staff       (20)     1490 2023-07-30 17:52:28.000000 textology-0.2.1/textology/widgets/_textual/_sparkline.py
--rw-r--r--   0 dfritz     (502) staff       (20)      354 2023-07-30 17:52:28.000000 textology-0.2.1/textology/widgets/_textual/_static.py
--rw-r--r--   0 dfritz     (502) staff       (20)     1278 2023-07-30 17:52:28.000000 textology-0.2.1/textology/widgets/_textual/_switch.py
--rw-r--r--   0 dfritz     (502) staff       (20)     2564 2023-07-30 17:52:28.000000 textology-0.2.1/textology/widgets/_textual/_tabbed_content.py
--rw-r--r--   0 dfritz     (502) staff       (20)     2098 2023-07-30 17:52:28.000000 textology-0.2.1/textology/widgets/_textual/_tabs.py
--rw-r--r--   0 dfritz     (502) staff       (20)     2169 2023-07-30 17:52:28.000000 textology-0.2.1/textology/widgets/_textual/_text_input.py
--rw-r--r--   0 dfritz     (502) staff       (20)     1780 2023-07-30 17:52:28.000000 textology-0.2.1/textology/widgets/_textual/_text_log.py
--rw-r--r--   0 dfritz     (502) staff       (20)      234 2023-07-30 17:52:28.000000 textology-0.2.1/textology/widgets/_textual/_tooltip.py
--rw-r--r--   0 dfritz     (502) staff       (20)     1409 2023-07-30 17:52:28.000000 textology-0.2.1/textology/widgets/_textual/_tree.py
-drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2023-07-30 17:55:13.520042 textology-0.2.1/textology.egg-info/
--rw-r--r--   0 dfritz     (502) staff       (20)    15574 2023-07-30 17:55:13.000000 textology-0.2.1/textology.egg-info/PKG-INFO
--rw-r--r--   0 dfritz     (502) staff       (20)     2088 2023-07-30 17:55:13.000000 textology-0.2.1/textology.egg-info/SOURCES.txt
--rw-r--r--   0 dfritz     (502) staff       (20)        1 2023-07-30 17:55:13.000000 textology-0.2.1/textology.egg-info/dependency_links.txt
--rw-r--r--   0 dfritz     (502) staff       (20)      303 2023-07-30 17:55:13.000000 textology-0.2.1/textology.egg-info/requires.txt
--rw-r--r--   0 dfritz     (502) staff       (20)       10 2023-07-30 17:55:13.000000 textology-0.2.1/textology.egg-info/top_level.txt
+drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2023-08-06 20:25:34.525037 textology-0.3.0/
+-rw-r--r--   0 dfritz     (502) staff       (20)     1068 2023-07-01 18:44:36.000000 textology-0.3.0/LICENSE
+-rw-r--r--   0 dfritz     (502) staff       (20)       97 2023-07-08 19:46:35.000000 textology-0.3.0/MANIFEST.in
+-rw-r--r--   0 dfritz     (502) staff       (20)    15590 2023-08-06 20:25:34.525231 textology-0.3.0/PKG-INFO
+-rw-r--r--   0 dfritz     (502) staff       (20)    14228 2023-08-06 20:14:59.000000 textology-0.3.0/README.md
+-rw-r--r--   0 dfritz     (502) staff       (20)       34 2023-07-30 17:52:28.000000 textology-0.3.0/requirements-dev.txt
+-rw-r--r--   0 dfritz     (502) staff       (20)      182 2023-08-06 20:14:59.000000 textology-0.3.0/requirements-full-dev.txt
+-rw-r--r--   0 dfritz     (502) staff       (20)       16 2023-07-30 17:52:28.000000 textology-0.3.0/requirements.txt
+-rw-r--r--   0 dfritz     (502) staff       (20)     1667 2023-08-06 20:25:34.526508 textology-0.3.0/setup.cfg
+-rw-r--r--   0 dfritz     (502) staff       (20)     3225 2023-07-08 19:46:35.000000 textology-0.3.0/setup.py
+drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2023-08-06 20:25:34.492687 textology-0.3.0/textology/
+-rw-r--r--   0 dfritz     (502) staff       (20)       69 2023-08-06 20:22:10.000000 textology-0.3.0/textology/__init__.py
+-rw-r--r--   0 dfritz     (502) staff       (20)    17290 2023-08-06 20:14:59.000000 textology-0.3.0/textology/apps.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     6551 2023-08-06 20:14:59.000000 textology-0.3.0/textology/dash_compat.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     2772 2023-07-04 21:19:10.000000 textology-0.3.0/textology/history.py
+-rw-r--r--   0 dfritz     (502) staff       (20)      492 2023-07-04 21:19:10.000000 textology-0.3.0/textology/logging.py
+drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2023-08-06 20:25:34.501345 textology-0.3.0/textology/observers/
+-rw-r--r--   0 dfritz     (502) staff       (20)      885 2023-07-24 01:09:35.000000 textology-0.3.0/textology/observers/__init__.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     6230 2023-07-24 01:09:35.000000 textology-0.3.0/textology/observers/_dependencies.py
+-rw-r--r--   0 dfritz     (502) staff       (20)      458 2023-07-22 18:13:02.000000 textology-0.3.0/textology/observers/_exceptions.py
+-rw-r--r--   0 dfritz     (502) staff       (20)    31303 2023-08-06 20:14:59.000000 textology-0.3.0/textology/observers/_managers.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     6499 2023-08-06 20:14:59.000000 textology-0.3.0/textology/pages.py
+-rw-r--r--   0 dfritz     (502) staff       (20)    16541 2023-07-16 17:16:06.000000 textology-0.3.0/textology/pytest_utils.py
+-rw-r--r--   0 dfritz     (502) staff       (20)    17773 2023-07-16 17:16:06.000000 textology-0.3.0/textology/router.py
+-rw-r--r--   0 dfritz     (502) staff       (20)    45559 2023-07-24 01:09:35.000000 textology-0.3.0/textology/test-template.html
+drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2023-08-06 20:25:34.509510 textology-0.3.0/textology/widgets/
+-rw-r--r--   0 dfritz     (502) staff       (20)     2653 2023-08-06 20:14:59.000000 textology-0.3.0/textology/widgets/__init__.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     2176 2023-08-06 20:14:59.000000 textology-0.3.0/textology/widgets/_button.py
+-rw-r--r--   0 dfritz     (502) staff       (20)    13679 2023-08-06 20:14:59.000000 textology-0.3.0/textology/widgets/_extensions.py
+-rw-r--r--   0 dfritz     (502) staff       (20)    12301 2023-08-06 20:14:59.000000 textology-0.3.0/textology/widgets/_horizontal_menus.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     2625 2023-08-06 20:14:59.000000 textology-0.3.0/textology/widgets/_list_item.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     2407 2023-08-06 20:14:59.000000 textology-0.3.0/textology/widgets/_list_item_header.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     2611 2023-08-06 20:14:59.000000 textology-0.3.0/textology/widgets/_list_item_meta.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     5350 2023-08-06 20:14:59.000000 textology-0.3.0/textology/widgets/_list_view.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     8995 2023-08-06 20:14:59.000000 textology-0.3.0/textology/widgets/_location.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     1955 2023-07-04 21:18:52.000000 textology-0.3.0/textology/widgets/_modal_dialog.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     2263 2023-08-06 20:14:59.000000 textology-0.3.0/textology/widgets/_store.py
+drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2023-08-06 20:25:34.524591 textology-0.3.0/textology/widgets/_textual/
+-rw-r--r--   0 dfritz     (502) staff       (20)      104 2023-07-30 17:52:28.000000 textology-0.3.0/textology/widgets/_textual/__init__.py
+-rw-r--r--   0 dfritz     (502) staff       (20)      294 2023-07-30 17:52:28.000000 textology-0.3.0/textology/widgets/_textual/_checkbox.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     1651 2023-07-30 17:52:28.000000 textology-0.3.0/textology/widgets/_textual/_containers.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     2064 2023-08-06 20:14:59.000000 textology-0.3.0/textology/widgets/_textual/_content_switcher.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     3190 2023-08-06 20:14:59.000000 textology-0.3.0/textology/widgets/_textual/_data_table.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     1770 2023-08-06 20:14:59.000000 textology-0.3.0/textology/widgets/_textual/_directory_tree.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     1095 2023-08-06 20:14:59.000000 textology-0.3.0/textology/widgets/_textual/_footer.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     1561 2023-08-06 20:14:59.000000 textology-0.3.0/textology/widgets/_textual/_header.py
+-rw-r--r--   0 dfritz     (502) staff       (20)      291 2023-07-30 17:52:28.000000 textology-0.3.0/textology/widgets/_textual/_label.py
+-rw-r--r--   0 dfritz     (502) staff       (20)      263 2023-07-30 17:52:28.000000 textology-0.3.0/textology/widgets/_textual/_loading_indicator.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     3623 2023-08-06 20:14:59.000000 textology-0.3.0/textology/widgets/_textual/_markdown.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     1723 2023-08-06 20:14:59.000000 textology-0.3.0/textology/widgets/_textual/_option_list.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     1540 2023-08-06 20:14:59.000000 textology-0.3.0/textology/widgets/_textual/_pretty.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     2085 2023-08-06 20:14:59.000000 textology-0.3.0/textology/widgets/_textual/_progress_bar.py
+-rw-r--r--   0 dfritz     (502) staff       (20)      308 2023-07-30 17:52:28.000000 textology-0.3.0/textology/widgets/_textual/_radio_button.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     1677 2023-08-06 20:14:59.000000 textology-0.3.0/textology/widgets/_textual/_radio_set.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     2137 2023-08-06 20:14:59.000000 textology-0.3.0/textology/widgets/_textual/_select.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     1952 2023-08-06 20:14:59.000000 textology-0.3.0/textology/widgets/_textual/_selection_list.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     1926 2023-08-06 20:14:59.000000 textology-0.3.0/textology/widgets/_textual/_sparkline.py
+-rw-r--r--   0 dfritz     (502) staff       (20)      354 2023-07-30 17:52:28.000000 textology-0.3.0/textology/widgets/_textual/_static.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     1742 2023-08-06 20:14:59.000000 textology-0.3.0/textology/widgets/_textual/_switch.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     3437 2023-08-06 20:14:59.000000 textology-0.3.0/textology/widgets/_textual/_tabbed_content.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     2971 2023-08-06 20:14:59.000000 textology-0.3.0/textology/widgets/_textual/_tabs.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     2633 2023-08-06 20:14:59.000000 textology-0.3.0/textology/widgets/_textual/_text_input.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     2244 2023-08-06 20:14:59.000000 textology-0.3.0/textology/widgets/_textual/_text_log.py
+-rw-r--r--   0 dfritz     (502) staff       (20)      234 2023-07-30 17:52:28.000000 textology-0.3.0/textology/widgets/_textual/_tooltip.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     1873 2023-08-06 20:14:59.000000 textology-0.3.0/textology/widgets/_textual/_tree.py
+drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2023-08-06 20:25:34.497838 textology-0.3.0/textology.egg-info/
+-rw-r--r--   0 dfritz     (502) staff       (20)    15590 2023-08-06 20:25:34.000000 textology-0.3.0/textology.egg-info/PKG-INFO
+-rw-r--r--   0 dfritz     (502) staff       (20)     2088 2023-08-06 20:25:34.000000 textology-0.3.0/textology.egg-info/SOURCES.txt
+-rw-r--r--   0 dfritz     (502) staff       (20)        1 2023-08-06 20:25:34.000000 textology-0.3.0/textology.egg-info/dependency_links.txt
+-rw-r--r--   0 dfritz     (502) staff       (20)      317 2023-08-06 20:25:34.000000 textology-0.3.0/textology.egg-info/requires.txt
+-rw-r--r--   0 dfritz     (502) staff       (20)       10 2023-08-06 20:25:34.000000 textology-0.3.0/textology.egg-info/top_level.txt
```

### Comparing `textology-0.2.1/LICENSE` & `textology-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `textology-0.2.1/PKG-INFO` & `textology-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textology
-Version: 0.2.1
+Version: 0.3.0
 Summary: Textual extensions for creating Terminal User Interfaces
 Home-page: https://github.com/dfrtz/textology
 Author: David Fritz
 License: MIT
 Project-URL: Issue Tracker, https://github.com/dfrtz/textology/issues
 Project-URL: Source Code, https://github.com/dfrtz/textology
 Platform: MacOS
@@ -377,15 +377,15 @@
 ```python
 from textology.widgets import Button
 
 def on_click(event):
     print("Don't press my buttons...")
 
 button = Button(
-    on_button_pressed=on_click,
+    callbacks={"on_button_pressed": on_click},
 )
 ```
 
 - Instance style extension (set styles directly at instantiation based on logic):
 ```python
 from textology.widgets import Button
 
@@ -400,15 +400,15 @@
 
 - Instance message disable extension (avoid unused event chains, such as in large ListViews):
 ```python
 from textual import events
 from textology.widgets import ListItem
 
 item = ListItem(
-    disable_messages=[events.Mount, events.Show],
+    disabled_messages=[events.Mount, events.Show],
 )
 ```
 
 ### Extended Testing
 
 Don't want to serialize your pytests? Looking for the ability to quickly visualize differences when UIs change?
 You came to the right place. Textology extends Textual SVG snapshot capabilities to add support for parallel processing
```

### Comparing `textology-0.2.1/README.md` & `textology-0.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -342,15 +342,15 @@
 ```python
 from textology.widgets import Button
 
 def on_click(event):
     print("Don't press my buttons...")
 
 button = Button(
-    on_button_pressed=on_click,
+    callbacks={"on_button_pressed": on_click},
 )
 ```
 
 - Instance style extension (set styles directly at instantiation based on logic):
 ```python
 from textology.widgets import Button
 
@@ -365,15 +365,15 @@
 
 - Instance message disable extension (avoid unused event chains, such as in large ListViews):
 ```python
 from textual import events
 from textology.widgets import ListItem
 
 item = ListItem(
-    disable_messages=[events.Mount, events.Show],
+    disabled_messages=[events.Mount, events.Show],
 )
 ```
 
 ### Extended Testing
 
 Don't want to serialize your pytests? Looking for the ability to quickly visualize differences when UIs change?
 You came to the right place. Textology extends Textual SVG snapshot capabilities to add support for parallel processing
```

### Comparing `textology-0.2.1/setup.cfg` & `textology-0.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `textology-0.2.1/setup.py` & `textology-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `textology-0.2.1/textology/apps.py` & `textology-0.3.0/textology/apps.py`

 * *Files 3% similar despite different names*

```diff
@@ -270,17 +270,18 @@
         self,
         request: Request,
     ) -> Label:
         """Default handler for when a request is made to a page that is not available."""
         self.logger.warning(f"Page not found {request.url.path}")
         return Label("Page not found")
 
-    def page_registry(self) -> dict:
+    @property
+    def page_registry(self) -> dict[str, Page]:
         """Provide the combined page registry in use by this multi-page application."""
-        return self._page_registry
+        return self._page_registry.copy()
 
     def _page_router(self, pathname: str, search: str) -> list[Widget]:
         """Load the appropriate page based on the URL path and search options."""
         self.logger.debug(f"Routing page content for: {pathname}")
 
         # Simulate router "serve()" to allow error handling at the callback level instead of router/widget level.
         request = Request(pathname if not search else f"{pathname}?{search}")
@@ -314,40 +315,48 @@
                 property_name not in self._observer_map[widget_id]
                 and property_name not in self._observer_map_global[widget_id]
             ):
                 continue
             for callback in self.generate_callbacks(widget_id, property_name):
                 self.watch(widget, property_name, callback, init=False)
 
-    def register_page(
+    def register_page(  # pylint: disable=too-many-arguments
         self,
         page: Page | ModuleType | str | Callable | None = None,
         path: str | None = None,
+        name: str | None = None,
+        order: int = 0,
         redirect_from: str | list[str] | None = None,
         layout: Callable | None = None,
     ) -> None:
         """Register a URL path to a layout in this multi-page application.
 
         Args:
             page: A module, or module path, where the remaining page's variables are defined.
                 e.g. If calling from within the module itself: "__name__"
                 e.g. If calling from another module: "mylib.home"
             path: URL Path, with or without variables. e.g. "/", "/home", "/documents/{document_name}"
                 Inferred from the "module" or "layout" if not provided.
                     e.g. "mylib.home" -> "/home"
                     e.g. "layout_home_page" -> "/home_page"
                 Variables marked as {variable_name} in paths will be passed to "layout" as keyword arguments.
+            name: The name of the page link, such as what might be shown in navigation menus.
+                Inferred from the "path" if not provided.
+                    e.g. "home_page" -> "Home Page"
+            order: The relative order to sort pages in the "page_registry", such as ordering in navigation menus.
             redirect_from: Paths that should redirect to this page's path. e.g. "/v1/home"
             layout: Function to call to generate the widget(s) used in the page's layout.
         """
         if not self._use_pages:
             raise ValueError("Pages are not enabled on this application")
         page = register_page(
             page=page,
             path=path,
+            name=name,
+            order=order,
             redirect_from=redirect_from,
             layout=layout,
             page_map=self._page_registry,
         )
         if page.path in ("/404", "/not_found", "/not_found_404"):
             # This is a special page that is not directly routed; it is used on every invalid path request.
             self.location.endpoint_not_found = Endpoint([], "", page.layout)
```

### Comparing `textology-0.2.1/textology/dash_compat.py` & `textology-0.3.0/textology/dash_compat.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,19 +67,21 @@
         Returns:
             Decorator to register a function as an input/output reaction to one or more property changes.
         """
         return super().when(
             *dependencies,
         )
 
-    def register_page(  # Intentional renames for Dash compatibility. pylint: disable=arguments-renamed
+    def register_page(  # Intentional renames for Dash compatibility. pylint: disable=arguments-renamed, too-many-arguments
         self,
         module: Page | ModuleType | str | Callable | None = None,
         path: str | None = None,
         path_template: str | None = None,
+        name: str | None = None,
+        order: int = 0,
         redirect_from: str | list[str] | None = None,
         layout: Callable | None = None,
     ) -> None:
         """Set up a URL path to provide a layout in a multi-page application.
 
         The "page_registry" global or app attribute can also be used to create page navigation links
         by application template/layout authors.
@@ -92,20 +94,26 @@
                 e.g. If calling from another module: "mylib.home"
             path: URL Path, with or without variables. e.g. "/", "/home", "/documents/{document_name}"
                 Inferred from the "module" or "layout" if not provided.
                     e.g. "mylib.home" -> "/home"
                     e.g. "home_page" -> "/home_page"
                 Variables marked as {variable_name} in paths will be passed to "layout" as keyword arguments.
             path_template: Compatibility alias for "path", no functional difference.
+            name: The name of the page link, such as what might be shown in navigation menus.
+                Inferred from the "path" if not provided.
+                    e.g. "home_page" -> "Home Page"
+            order: The relative order to sort pages in the "page_registry", such as ordering in navigation menus.
             redirect_from: Paths that should redirect to this page's path. e.g. "/v1/home"
             layout: Function to call to generate the widget(s) used in the page's layout.
         """
         super().register_page(
             page=module,
             path=path_template or path,
+            name=name,
+            order=order,
             redirect_from=redirect_from,
             layout=layout,
         )
 
 
 def Input(  # Treat this function as a class factory. pylint: disable=invalid-name
     id_or_exception: str | SupportsID | type[BaseException],
```

### Comparing `textology-0.2.1/textology/history.py` & `textology-0.3.0/textology/history.py`

 * *Files identical despite different names*

### Comparing `textology-0.2.1/textology/observers/__init__.py` & `textology-0.3.0/textology/observers/__init__.py`

 * *Files identical despite different names*

### Comparing `textology-0.2.1/textology/observers/_dependencies.py` & `textology-0.3.0/textology/observers/_dependencies.py`

 * *Files identical despite different names*

### Comparing `textology-0.2.1/textology/observers/_managers.py` & `textology-0.3.0/textology/observers/_managers.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import abc
 import asyncio
 import itertools
 import logging
 import traceback
 import weakref
 from collections import defaultdict
+from functools import lru_cache
 from inspect import isawaitable
 from typing import Any
 from typing import Callable
 from typing import Coroutine
 from typing import Generator
 
 from textology.logging import NullLogger
@@ -36,14 +37,15 @@
 # Type alias to represent function receiving 2 arguments (old value and new value) and returning nothing.
 ValueUpdateHandler = Callable[[Any, Any], Coroutine]
 
 _GLOBAL_OBSERVER_EXC_MAP: dict[type[Exception], list[Observer]] = defaultdict(list)
 _GLOBAL_OBSERVER_ID_MAP: dict[str, Observer] = {}
 _GLOBAL_OBSERVER_MAP: dict[str, dict[str, list[Observer]]] = defaultdict(lambda: defaultdict(list))
 
+CALLBACK_CACHE_SIZE = 1024
 WHEN_DECORATOR = "_textology_when"
 
 
 class Observer:
     """Specification details for an input/output observer.
 
     External callbacks should be considered stateless: they should not store or request any
@@ -279,14 +281,15 @@
                     self.apply_update(observer.id, update_components[comp_id], comp_id, comp_property, value)
             except BaseException as error:  # pylint: disable=broad-exception-caught
                 # Catch all errors to prevent fatal crashes in application callback loops.
                 self.on_callback_error(observer.id, error)
 
         return _on_update
 
+    @lru_cache(maxsize=CALLBACK_CACHE_SIZE)
     def generate_callbacks(self, component_id: str, component_property: str) -> list[ValueUpdateHandler]:
         """Create callbacks that will manage input/output operations for all functions registered to id/property combo.
 
         Args:
             component_id: ID of a component with a property that will trigger callbacks.
             component_property: Property name on the component that will trigger callbacks.
```

### Comparing `textology-0.2.1/textology/pages.py` & `textology-0.3.0/textology/pages.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,44 +12,52 @@
 class Page:
     """Configuration for a page in a multi-page application routed via URL path."""
 
     def __init__(
         self,
         layout: Callable,
         path: str | None = None,
+        name: str | None = None,
+        order: int = 0,
         redirect_from: str | list[str] | None = None,
     ) -> None:
         """Initialize the page configuration.
 
         Args:
             layout: Function to call to generate the widget(s) used in the page's layout.
             path: URL Path, with or without variables. e.g. "/", "/home", "/documents/{document_name}"
                 Inferred from the "layout" if not provided.
                     e.g. "home_page" -> "/home_page"
                 Variables marked as {variable_name} in paths will be passed to "layout" as keyword arguments.
+            name: The name of the page link, such as what might be shown in navigation menus.
+                Inferred from the "path" if not provided.
+                    e.g. "home_page" -> "Home Page"
+            order: The relative order to sort pages in the "page_registry", such as ordering in navigation menus.
             redirect_from: Paths that should redirect to this page's path. e.g. "/v1/home"
         """
         if not path:
             path = layout.__name__.removeprefix("layout_")
         self.layout = layout
         self.path = path if path.startswith("/") else f"/{path}"
+        self.name = name or self.path.strip("/").replace("_", " ").title()
+        self.order = order
         self.redirect_from = [redirect_from] if isinstance(redirect_from, str) else redirect_from
 
     @staticmethod
     def from_module(module: ModuleType | str) -> Page:
         """Convert a module into an application page.
 
         Args:
             module: Loaded module, or path to a module, with page attributes such as "layout".
 
         Returns:
             Newly created page with attributes, such as path, populated by the module's attributes and variables.
         """
         kwargs = {}
-        vars_to_save = ("layout", "path", "redirect_from")
+        vars_to_save = ("layout", "path", "name", "order", "redirect_from")
         if isinstance(module, str):
             module = importlib.import_module(module)
         for var_name in dir(module):
             if var_name not in vars_to_save:
                 continue
             var = getattr(module, var_name)
             kwargs[var_name] = var
@@ -75,17 +83,19 @@
         if isinstance(page, (ModuleType, str)):
             page = Page.from_module(page)
         elif isinstance(page, Callable):
             page = Page(page)
         return page
 
 
-def register_page(
+def register_page(  # pylint: disable=too-many-arguments
     page: Page | ModuleType | str | Callable | None = None,
     path: str | None = None,
+    name: str | None = None,
+    order: int = 0,
     redirect_from: str | list[str] | None = None,
     layout: Callable | None = None,
     page_map: dict[str, Page] | None = None,
 ) -> Page:
     """Register a URL path to a layout shared across all multi-page applications.
 
     Args:
@@ -93,14 +103,18 @@
             e.g. If calling from within the module itself: "__name__"
             e.g. If calling from another module: "mylib.home"
         path: URL Path, with or without variables. e.g. "/", "/home", "/documents/{document_name}"
             Inferred from the "module" or "layout" if not provided.
                 e.g. "mylib.home" -> "/home"
                 e.g. "layout_home_page" -> "/home_page"
             Variables marked as {variable_name} in paths will be passed to "layout" as keyword arguments.
+        name: The name of the page link, such as what might be shown in navigation menus.
+            Inferred from the "path" if not provided.
+                e.g. "home_page" -> "Home Page"
+        order: The relative order to sort pages in the "page_registry", such as ordering in navigation menus.
         redirect_from: Paths that should redirect to this page's path. e.g. "/v1/home"
         layout: Function to call to generate the widget(s) used in the page's layout.
         page_map: All currently registered pages for a multi-page app.
             Modified in place when page is registered. Defaults to global pages shared across apps.
 
     Returns:
         Final page registered to the path, and created from arguments if needed.
@@ -113,18 +127,24 @@
         page = Page.to_page(page)
         if path:
             page.path = path
         if redirect_from:
             page.redirect_from = redirect_from
         if layout:
             page.layout = layout
+        if name:
+            page.name = name
+        if order:
+            page.order = order
     else:
         page = Page(
             layout=layout,
             path=path,
+            name=name,
+            order=order,
             redirect_from=redirect_from,
         )
     paths = [page.path]
     if page.redirect_from:
         paths.extend(page.redirect_from)
     page_map = page_map if page_map is not None else _GLOBAL_PAGE_MAP
     for page_path in paths:
```

### Comparing `textology-0.2.1/textology/pytest_utils.py` & `textology-0.3.0/textology/pytest_utils.py`

 * *Files identical despite different names*

### Comparing `textology-0.2.1/textology/router.py` & `textology-0.3.0/textology/router.py`

 * *Files identical despite different names*

### Comparing `textology-0.2.1/textology/test-template.html` & `textology-0.3.0/textology/test-template.html`

 * *Files identical despite different names*

### Comparing `textology-0.2.1/textology/widgets/__init__.py` & `textology-0.3.0/textology/widgets/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 """
 
 from ._button import Button
 from ._extensions import Clickable
 from ._extensions import WidgetExtension
 from ._extensions import WidgetInitExtension
 from ._horizontal_menus import HorizontalMenus
-from ._list_item import LIST_ITEM_EVENT_IGNORES
 from ._list_item import ListItem
 from ._list_item_header import ListItemHeader
 from ._list_item_meta import ListItemMeta
 from ._list_view import ListView
 from ._location import Location
 from ._modal_dialog import ModalDialog
 from ._store import Store
```

### Comparing `textology-0.2.1/textology/widgets/_button.py` & `textology-0.3.0/textology/widgets/_button.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """Extended Textual, simple, clickable, button."""
 
 from typing import Any
+from typing import Callable
 
 from rich.text import TextType
+from textual import events
 from textual import widgets
 from textual.message import Message
 from textual.widgets.button import ButtonVariant
 
 from ._extensions import Clickable
 from ._extensions import WidgetExtension
 
@@ -19,35 +21,43 @@
         label: TextType | None = None,
         variant: ButtonVariant = "default",
         *,
         name: str | None = None,
         id: str | None = None,
         classes: str | None = None,
         disabled: bool = False,
-        **extension_configs: Any,
+        styles: dict[str, Any] | None = None,
+        disabled_messages: list[type[events.Message]] | None = None,
+        callbacks: dict[str, Callable] | None = None,
     ) -> None:
         """Initialize a Button widget with extension arguments.
 
         Args:
             label: The text that appears within the button.
             variant: The variant of the button.
             name: The name of the button.
             id: The ID of the button in the DOM.
             classes: The CSS classes of the button.
             disabled: Whether the button is disabled or not.
-            extension_configs: Widget extension configurations, such as dynamically provided local callbacks by name.
+            styles: Local inline styles to apply on top of the class' styles for only this instance.
+            disabled_messages: List of messages to disable on this widget instance only.
+            callbacks: Mapping of callbacks to send messages to instead of sending to default handler.
         """
         super().__init__(
             label=label,
             variant=variant,
             name=name,
             id=id,
             classes=classes,
             disabled=disabled,
         )
-        self.__extend_widget__(**extension_configs)
+        self.__extend_widget__(
+            styles=styles,
+            disabled_messages=disabled_messages,
+            callbacks=callbacks,
+        )
 
     async def intercept_message(self, message: Message) -> Message | None:
         """Update reactive attributes on press."""
         if isinstance(message, Button.Pressed):
             self.update_n_clicks()
         return message
```

### Comparing `textology-0.2.1/textology/widgets/_horizontal_menus.py` & `textology-0.3.0/textology/widgets/_horizontal_menus.py`

 * *Files 3% similar despite different names*

```diff
@@ -84,30 +84,34 @@
         *children: Widget | ListItem | ListItemMeta,
         name: str | None = None,
         id: str | None = None,
         classes: str | None = None,
         disabled: bool = False,
         can_focus: bool = False,
         menu_creator: Callable[[int, list[ListItem]], Widget] | None = None,
-        **extension_configs: Any,
+        styles: dict[str, Any] | None = None,
+        disabled_messages: list[type[events.Message]] | None = None,
+        callbacks: dict[str, Callable] | None = None,
     ) -> None:
         """Initialize horizontal menus.
 
         Args:
             *children: Initial menus, or menu items, to display.
                 Each "menu" widget must contain a ListView, but does not have to be a ListView itself.
                 If children are ListItem or ListItemMeta objects, an initial ListView will be made with menu_creator.
             name: The name of the widget.
             id: The ID of the widget in the DOM.
             classes: The CSS classes for the widget.
             disabled: Whether the widget is disabled or not.
             can_focus: Whether the parent widget can be focused, or only the children widgets.
                 If enabled, it will take focus after all the nested ListViews, but before the next sibling.
             menu_creator: Called to create new sub-menus when an item with children is highlighted.
-            extension_configs: Widget extension configurations, such as dynamically provided local callbacks by name.
+            styles: Local inline styles to apply on top of the class' styles for only this instance.
+            disabled_messages: List of messages to disable on this widget instance only.
+            callbacks: Mapping of callbacks to send messages to instead of sending to default handler.
         """
         self.menu_creator = menu_creator or self._default_menu_creator
         if any(isinstance(child, (ListItem, ListItemMeta)) for child in children):
             if not all(isinstance(child, (ListItem, ListItemMeta)) for child in children):
                 raise ValueError("All initial children must be of same type: ListItem, ListItemMeta, or ListView")
             self._update_menu_index(children, 0)
             children = [
@@ -119,15 +123,19 @@
         super().__init__(
             *children,
             name=name,
             id=id,
             classes=classes,
             disabled=disabled,
         )
-        self.__extend_widget__(**extension_configs)
+        self.__extend_widget__(
+            styles=styles,
+            disabled_messages=disabled_messages,
+            callbacks=callbacks,
+        )
         self.can_focus = can_focus
         self.menus = []
         for child in children or []:
             menu = None
             if isinstance(child, ListView):
                 menu = child
             else:
```

### Comparing `textology-0.2.1/textology/widgets/_list_item.py` & `textology-0.3.0/textology/widgets/_list_item.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,60 +1,67 @@
 """Extended Textual widget that is an item within a ListView, and contains metadata about the selection."""
 
 from typing import Any
+from typing import Callable
 
 from textual import events
 from textual import widgets
 from textual.widget import Widget
 
 from ._extensions import WidgetExtension
 from ._textual._label import Label
 
-# Recommended events to ignore when widgets are used in ListViews to prevent large unneeded event batches.
-LIST_ITEM_EVENT_IGNORES = (
-    events.Mount,
-    events.Unmount,
-    events.Show,
-    events.Hide,
-    events.Resize,
-)
-
 
 class ListItem(WidgetExtension, widgets.ListItem):
     """An extended widget that is an item within a ListView, and contains metadata about the selection."""
 
+    # Recommended events to ignore when widgets are used in ListViews to prevent large unneeded event batches.
+    default_disabled_messages = (
+        events.Mount,
+        events.Unmount,
+        events.Show,
+        events.Hide,
+        events.Resize,
+    )
+
     def __init__(
         self,
         *children: Widget,
         name: str | None = None,
         id: str | None = None,
         classes: str | None = None,
         disabled: bool = False,
         data: Any = None,
-        **extension_configs: Any,
+        styles: dict[str, Any] | None = None,
+        disabled_messages: list[type[events.Message]] | None = None,
+        callbacks: dict[str, Callable] | None = None,
     ) -> None:
         """Initialize a ListItem with extension arguments.
 
         Args:
             *children: Child widgets.
             name: The name of the widget.
                 If no child is provided for display, and no "data" with "label" key, name will be used in a Label.
             id: The ID of the widget in the DOM.
             classes: The CSS classes for the widget.
             disabled: Whether the widget is disabled or not.
             data: Optional data associated with the list item.
                 If no child is provided for display, the data will be searched for a "label" key to use in a Label.
-            extension_configs: Widget extension configurations, such as dynamically provided local callbacks by name.
+            styles: Local inline styles to apply on top of the class' styles for only this instance.
+            disabled_messages: List of messages to disable on this widget instance only.
+            callbacks: Mapping of callbacks to send messages to instead of sending to default handler.
         """
         if not children:
             label = name
             if data and "label" in data:
                 label = data["label"]
             if label:
-                children = [Label(label, disable_messages=LIST_ITEM_EVENT_IGNORES)]
+                children = [Label(label, disabled_messages=ListItem.default_disabled_messages)]
 
         super().__init__(*children, name=name, id=id, classes=classes, disabled=disabled)
-        if "disable_messages" not in extension_configs:
-            extension_configs["disable_messages"] = LIST_ITEM_EVENT_IGNORES
-        self.__extend_widget__(**extension_configs)
+        self.__extend_widget__(
+            styles=styles,
+            disabled_messages=disabled_messages,
+            callbacks=callbacks,
+        )
         self.data = data
         self.menu_index: int | None = None
```

### Comparing `textology-0.2.1/textology/widgets/_list_item_header.py` & `textology-0.3.0/textology/widgets/_textual/_tabs.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,64 +1,88 @@
-"""List item that acts as an unselectable header between groups."""
+"""Extended Textual Tab widgets."""
 
 from typing import Any
+from typing import Callable
 
-from textual.events import Click
-from textual.widget import Widget
+from rich.text import TextType
+from textual import events
+from textual import widgets
 
-from ._list_item import ListItem
+from .._extensions import WidgetExtension
 
 
-class ListItemHeader(ListItem):
-    """A widget that is an item within a ListView that acts as an unselectable header between list items."""
+class Tab(WidgetExtension, widgets.Tab):
+    """An extended widget to manage a single tab within a Tabs widget."""
 
-    DEFAULT_CSS = """
-    ListItemHeader>Widget {
-        color: $text;
-        text-style: bold;
-    }
-    ListItemHeader:hover>Widget {
-        color: $text;
-        text-style: bold;
-    }
-    """
+    def __init__(
+        self,
+        label: TextType,
+        *,
+        id: str | None = None,
+        classes: str | None = None,
+        styles: dict[str, Any] | None = None,
+        disabled_messages: list[type[events.Message]] | None = None,
+        callbacks: dict[str, Callable] | None = None,
+    ) -> None:
+        """Initialize a Tab.
+
+        Args:
+            label: The label to use in the tab.
+            id: Optional ID for the widget.
+            classes: Space separated list of class names.
+            styles: Local inline styles to apply on top of the class' styles for only this instance.
+            disabled_messages: List of messages to disable on this widget instance only.
+            callbacks: Mapping of callbacks to send messages to instead of sending to default handler.
+        """
+        super().__init__(
+            label,
+            id=id,
+            classes=classes,
+        )
+        self.__extend_widget__(
+            styles=styles,
+            disabled_messages=disabled_messages,
+            callbacks=callbacks,
+        )
+
+
+class Tabs(WidgetExtension, widgets.Tabs):
+    """An extended row of tabs."""
 
     def __init__(
         self,
-        *children: Widget,
+        *tabs: Tab | TextType,
+        active: str | None = None,
         name: str | None = None,
         id: str | None = None,
         classes: str | None = None,
         disabled: bool = False,
-        disable_click: bool = True,
-        data: Any = None,
-        **extension_configs: Any,
+        styles: dict[str, Any] | None = None,
+        disabled_messages: list[type[events.Message]] | None = None,
+        callbacks: dict[str, Callable] | None = None,
     ) -> None:
-        """Initialize a ListItemHeader with extension arguments.
+        """Initialize a Tabs widget.
 
         Args:
-            *children: Child widgets.
-            name: The name of the widget.
-            id: The ID of the widget in the DOM.
-            classes: The CSS classes for the widget.
-            disabled: Whether the widget is disabled or not.
-            disable_click: Whether clicking the widget it disabled.
-            data: Optional data associated with the list item.
-                If no child is provided for display, the data will be searched for a "label" key to use in a Label.
-            extension_configs: Widget extension configurations, such as dynamically provided local callbacks by name.
+            *tabs: Positional argument should be explicit Tab objects, or a str or Text.
+            active: ID of the tab which should be active on start.
+            name: Optional name for the input widget.
+            id: Optional ID for the widget.
+            classes: Optional initial classes for the widget.
+            disabled: Whether the input is disabled or not.
+            styles: Local inline styles to apply on top of the class' styles for only this instance.
+            disabled_messages: List of messages to disable on this widget instance only.
+            callbacks: Mapping of callbacks to send messages to instead of sending to default handler.
         """
         super().__init__(
-            *children,
+            *tabs,
+            active=active,
             name=name,
             id=id,
             classes=classes,
             disabled=disabled,
-            data=data,
-            **extension_configs,
         )
-        self.disable_click = disable_click
-
-    async def _on_click(self, event: Click) -> None:
-        """Disable clicking header items."""
-        if self.disable_click:
-            event.stop()
-            event.prevent_default()
+        self.__extend_widget__(
+            styles=styles,
+            disabled_messages=disabled_messages,
+            callbacks=callbacks,
+        )
```

### Comparing `textology-0.2.1/textology/widgets/_list_item_meta.py` & `textology-0.3.0/textology/widgets/_list_item_meta.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,56 +1,70 @@
 """Widget metadata that is used to create an item within a ListView on demand."""
 
 from typing import Any
+from typing import Callable
+
+from textual import events
 
 from ._list_item import ListItem
 
 
 class ListItemMeta:
     """A metadata class used to create, and recreate, list items that will be used in list views."""
 
-    def __init__(
+    def __init__(  # pylint: disable=too-many-arguments
         self,
         item_type: type[ListItem] = ListItem,
         name: str | None = None,
         id: str | None = None,
         classes: str | None = None,
+        disabled: bool = False,
         data: Any = None,
-        **extension_configs: Any,
+        styles: dict[str, Any] | None = None,
+        disabled_messages: list[type[events.Message]] | None = None,
+        callbacks: dict[str, Callable] | None = None,
     ) -> None:
         """Initialize metadata object to allow creating list items on demand.
 
         Args:
             item_type: Type of list item to instantiate with the metadata values.
             name: The name of the widget.
             id: The ID of the widget in the DOM.
             classes: The CSS classes for the widget.
             disabled: Whether the widget is disabled or not.
             data: Optional data associated with the list item.
-                If no child is provided for display, the data will be searched for a "name" key to use in a Label.
-            extension_configs: Widget extension configurations, such as dynamically provided local callbacks by name.
+                If no child is provided for display, the data will be searched for a "label" key to use in a Label.
+            styles: Local inline styles to apply on top of the class' styles for only this instance.
+            disabled_messages: List of messages to disable on this widget instance only.
+            callbacks: Mapping of callbacks to send messages to instead of sending to default handler.
         """
         if not issubclass(item_type, ListItem):
             raise ValueError("Item type must be a subclass of ListItem")
         self.item_type = item_type
         self.name = name
         self.id = id
         self.classes = classes
+        self.disabled = disabled
         self.data = data
-        self.extension_configs = extension_configs
         self.menu_index: int | None = None
+        self.extension_configs = {
+            "styles": styles,
+            "disabled_messages": disabled_messages,
+            "callbacks": callbacks,
+        }
 
     def to_item(self) -> ListItem:
         """Create the underlying list item widget.
 
         Returns:
             Newly created item that can be used in a list view.
         """
         item = self.item_type(
             name=self.name,
             id=self.id,
             classes=self.classes,
+            disabled=self.disabled,
             data=self.data,
             **self.extension_configs,
         )
         item.menu_index = self.menu_index
         return item
```

### Comparing `textology-0.2.1/textology/widgets/_list_view.py` & `textology-0.3.0/textology/widgets/_list_view.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Extended Textual vertical list view widget."""
 
 from typing import Any
+from typing import Callable
 
 from textual import events
 from textual import widgets
 from textual.reactive import reactive
 from textual.widget import AwaitMount
 from textual.widget import Widget
 from textual.widgets import ListItem
@@ -29,37 +30,45 @@
         *children: ListItem,
         initial_index: int | None = 0,
         name: str | None = None,
         id: str | None = None,
         classes: str | None = None,
         disabled: bool = False,
         auto_highlight: bool = True,
-        **extension_configs: Any,
+        styles: dict[str, Any] | None = None,
+        disabled_messages: list[events.Message] | None = None,
+        callbacks: dict[str, Callable] | None = None,
     ) -> None:
         """Initialize a ListView with extension arguments.
 
         Args:
             *children: The ListItems to display in the list.
             initial_index: The index that should be highlighted when the list is first mounted.
             name: The name of the widget.
             id: The unique ID of the widget used in CSS/query selection.
             classes: The CSS classes of the widget.
             disabled: Whether the ListView is disabled or not.
             auto_highlight: Whether the ListView automatically highlights the first item on focus.
-            extension_configs: Widget extension configurations, such as dynamically provided local callbacks by name.
+            styles: Local inline styles to apply on top of the class' styles for only this instance.
+            disabled_messages: List of messages to disable on this widget instance only.
+            callbacks: Mapping of callbacks to send messages to instead of sending to default handler.
         """
         super().__init__(
             *children,
             initial_index=initial_index,
             name=name,
             id=id,
             classes=classes,
             disabled=disabled,
         )
-        self.__extend_widget__(**extension_configs)
+        self.__extend_widget__(
+            styles=styles,
+            disabled_messages=disabled_messages,
+            callbacks=callbacks,
+        )
         self.auto_highlight = auto_highlight
 
     def on_focus(self, event: events.Focus) -> None:
         """Automatically highlight the first item in the list when the list is focused."""
         super()._on_focus(event)
         if self.auto_highlight and self.has_focus and self.index is None and self._nodes:
             self.index = 0
```

### Comparing `textology-0.2.1/textology/widgets/_location.py` & `textology-0.3.0/textology/widgets/_location.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Widget representation of the current location of loaded resources."""
 
 from __future__ import annotations
 
 import logging
 from typing import Any
+from typing import Callable
 from urllib.parse import urlparse
 
 from textual import events
 from textual.message import Message
 from textual.reactive import reactive
 from textual.widget import Widget
 
@@ -76,34 +77,36 @@
     # The search (or query) in URL. e.g. "?resource_type=1".
     search: str = reactive("", repaint=False, init=False)
     # The hash (or fragment) in a URL. e.g. "#resource-1".
     hash: str = reactive("", repaint=False, init=False)
     # Sentinel value used to trigger reloads from callbacks. Set to True to manually trigger a reload.
     refresh_url: bool = reactive(False, repaint=False, init=False, always_update=True)
 
-    def __init__(
+    def __init__(  # pylint: disable=too-many-arguments
         self,
         path: str | None = "/",
         id: str | None = None,
         logger: logging.Logger | None = None,
         enable_url_events: bool = False,
         enable_history_events: bool = False,
-        **extension_configs: Any,
+        disabled_messages: list[events.Message] | None = None,
+        callbacks: dict[str, Callable] | None = None,
     ) -> None:
         """Initialize the location, routing, and history.
 
         Args:
             path: The initial path to load after set up.
             id: The ID of the widget in the DOM.
             logger: Custom logger to send routing messages to.
             enable_url_events: Whether URL update events should be sent.
             enable_history_events: Whether history update events should be sent.
-            extension_configs: Widget extension configurations, such as dynamically provided local callbacks by name.
+            disabled_messages: List of messages to disable on this widget instance only.
+            callbacks: Mapping of callbacks to send messages to instead of sending to default handler.
         """
-        super().__init__(id=id, **extension_configs)
+        super().__init__(id=id, disabled_messages=disabled_messages, callbacks=callbacks)
         self._initial_path = path
         # Manually set up router mixin since Widget inheritance does not automatically trigger.
         Router.__init__(self, logger=logger or logging.root)
         self._history = History()
         self.url_events_enabled = enable_url_events
         self.history_events_enabled = enable_history_events
```

### Comparing `textology-0.2.1/textology/widgets/_modal_dialog.py` & `textology-0.3.0/textology/widgets/_modal_dialog.py`

 * *Files identical despite different names*

### Comparing `textology-0.2.1/textology/widgets/_store.py` & `textology-0.3.0/textology/widgets/_store.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """Widget container for basic data storage and sharing between callbacks."""
 
 import time
 from typing import Any
+from typing import Callable
 from typing import TypeVar
 
+from textual import events
 from textual.reactive import reactive
 from textual.widget import Widget
 
 from ._extensions import WidgetInitExtension
 
 JsonType = TypeVar("JsonType", dict, list, bool, float, int, str, None)  # Custom type. pylint: disable=invalid-name
 
@@ -33,24 +35,26 @@
     # Sentinel value used to trigger clears from callbacks. Set to True to manually trigger a clear.
     clear_data: bool = reactive(False, always_update=True, repaint=False, init=False)
 
     def __init__(
         self,
         data: Any,
         id: str | None = None,
-        **extension_configs: Any,
+        disabled_messages: list[events.Message] | None = None,
+        callbacks: dict[str, Callable] | None = None,
     ) -> None:
         """Initialize the data store.
 
         Args:
             data: Initial data to store.
             id: The ID of the widget in the DOM.
-            extension_configs: Widget extension configurations, such as dynamically provided local callbacks by name.
+            disabled_messages: List of messages to disable on this widget instance only.
+            callbacks: Mapping of callbacks to send messages to instead of sending to default handler.
         """
-        super().__init__(id=id, **extension_configs)
+        super().__init__(id=id, disabled_messages=disabled_messages, callbacks=callbacks)
         self.data = data
 
     def watch_clear_data(self, new_value: bool) -> None:
         """Monitor the sentinel attribute for clear data requests from callbacks.
 
         Args:
             new_value: New clear data value set on the reactive attribute.
```

### Comparing `textology-0.2.1/textology/widgets/_textual/_containers.py` & `textology-0.3.0/textology/widgets/_textual/_containers.py`

 * *Files identical despite different names*

### Comparing `textology-0.2.1/textology/widgets/_textual/_content_switcher.py` & `textology-0.3.0/textology/widgets/_textual/_content_switcher.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """Extended Textual ContentSwitcher widget."""
 
 from typing import Any
+from typing import Callable
 
+from textual import events
 from textual import widgets
 from textual.widget import Widget
 
 from .._extensions import WidgetExtension
 
 
 class ContentSwitcher(WidgetExtension, widgets.ContentSwitcher):
@@ -20,25 +22,33 @@
         self,
         *children: Widget,
         name: str | None = None,
         id: str | None = None,
         classes: str | None = None,
         disabled: bool = False,
         initial: str | None = None,
-        **extension_configs: Any,
+        styles: dict[str, Any] | None = None,
+        disabled_messages: list[type[events.Message]] | None = None,
+        callbacks: dict[str, Callable] | None = None,
     ) -> None:
         """Initialize the content switching widget.
 
         Args:
             *children: The widgets to switch between.
             name: The name of the content switcher.
             id: The ID of the content switcher in the DOM.
             classes: The CSS classes of the content switcher.
             disabled: Whether the content switcher is disabled or not.
             initial: The ID of the initial widget to show, ``None`` or empty string for the first tab.
-            extension_configs: Widget extension configurations, such as dynamically provided local callbacks by name.
+            styles: Local inline styles to apply on top of the class' styles for only this instance.
+            disabled_messages: List of messages to disable on this widget instance only.
+            callbacks: Mapping of callbacks to send messages to instead of sending to default handler.
 
         Note:
             If `initial` is not supplied, no children will be shown to start with.
         """
         super().__init__(*children, name=name, id=id, classes=classes, disabled=disabled, initial=initial)
-        self.__extend_widget__(**extension_configs)
+        self.__extend_widget__(
+            styles=styles,
+            disabled_messages=disabled_messages,
+            callbacks=callbacks,
+        )
```

### Comparing `textology-0.2.1/textology/widgets/_textual/_data_table.py` & `textology-0.3.0/textology/widgets/_textual/_progress_bar.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,65 +1,59 @@
-"""Extended Textual DataTable widget."""
+"""Extended Textual ProgressBar widget."""
 
 from typing import Any
+from typing import Callable
 
+from textual import events
 from textual import widgets
-from typing_extensions import Literal
 
 from .._extensions import WidgetExtension
 
 
-class DataTable(WidgetExtension, widgets.DataTable):  # pylint: disable=too-many-ancestors
-    """An extended tabular widget that contains data."""
+class ProgressBar(WidgetExtension, widgets.ProgressBar):
+    """An extended progress bar widget."""
 
     def __init__(
         self,
+        total: float | None = None,
         *,
-        show_header: bool = True,
-        show_row_labels: bool = True,
-        fixed_rows: int = 0,
-        fixed_columns: int = 0,
-        zebra_stripes: bool = False,
-        header_height: int = 1,
-        show_cursor: bool = True,
-        cursor_foreground_priority: Literal["renderable", "css"] = "css",
-        cursor_background_priority: Literal["renderable", "css"] = "renderable",
+        show_bar: bool = True,
+        show_percentage: bool = True,
+        show_eta: bool = True,
         name: str | None = None,
         id: str | None = None,
         classes: str | None = None,
         disabled: bool = False,
-        **extension_configs: Any,
+        styles: dict[str, Any] | None = None,
+        disabled_messages: list[type[events.Message]] | None = None,
+        callbacks: dict[str, Callable] | None = None,
     ) -> None:
-        """Initialize the data table widget.
+        """Initialize a Progress Bar widget.
 
         Args:
-            show_header: Whether to show the table header.
-            show_row_labels: Whether to show labels on every row.
-            fixed_rows: Fixed number of rows to display.
-            fixed_columns: Fixed number of columns to display
-            zebra_stripes: Whether to display the rows with alternating background highlight style.
-            show_cursor: Whether to highlight the currently active cursor highlight.
-            header_height: Height the header row.
-            cursor_foreground_priority: Whether to prioritize the cursor CSS foreground or the renderable foreground.
-            cursor_background_priority: Whether to prioritize the cursor CSS background or the renderable background.
-            name: The name of the content switcher.
-            id: The ID of the content switcher in the DOM.
-            classes: The CSS classes of the content switcher.
-            disabled: Whether the content switcher is disabled or not.
-            extension_configs: Widget extension configurations, such as dynamically provided local callbacks by name.
+            total: The total number of steps in the progress if known.
+            show_bar: Whether to show the bar portion of the progress bar.
+            show_percentage: Whether to show the percentage status of the bar.
+            show_eta: Whether to show the ETA countdown of the progress bar.
+            name: The name of the widget.
+            id: The ID of the widget in the DOM.
+            classes: The CSS classes for the widget.
+            disabled: Whether the widget is disabled or not.
+            styles: Local inline styles to apply on top of the class' styles for only this instance.
+            disabled_messages: List of messages to disable on this widget instance only.
+            callbacks: Mapping of callbacks to send messages to instead of sending to default handler.
         """
         super().__init__(
-            show_header=show_header,
-            show_row_labels=show_row_labels,
-            fixed_rows=fixed_rows,
-            fixed_columns=fixed_columns,
-            zebra_stripes=zebra_stripes,
-            header_height=header_height,
-            show_cursor=show_cursor,
-            cursor_foreground_priority=cursor_foreground_priority,
-            cursor_background_priority=cursor_background_priority,
+            total=total,
+            show_bar=show_bar,
+            show_percentage=show_percentage,
+            show_eta=show_eta,
             name=name,
             id=id,
             classes=classes,
             disabled=disabled,
         )
-        self.__extend_widget__(**extension_configs)
+        self.__extend_widget__(
+            styles=styles,
+            disabled_messages=disabled_messages,
+            callbacks=callbacks,
+        )
```

### Comparing `textology-0.2.1/textology/widgets/_textual/_directory_tree.py` & `textology-0.3.0/textology/widgets/_textual/_footer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,33 @@
-"""Extended Textual DirectoryTree widget."""
+"""Extended Textual Footer widget."""
 
-from pathlib import Path
 from typing import Any
+from typing import Callable
 
+from textual import events
 from textual import widgets
 
 from .._extensions import WidgetExtension
 
 
-class DirectoryTree(WidgetExtension, widgets.DirectoryTree):  # pylint: disable=too-many-ancestors
-    """An extended Tree widget that presents files and directories."""
+class Footer(WidgetExtension, widgets.Footer):
+    """An extended simple footer widget which docks itself to the bottom of the parent container."""
 
     def __init__(
         self,
-        path: str | Path,
-        *,
-        name: str | None = None,
-        id: str | None = None,
-        classes: str | None = None,
-        disabled: bool = False,
-        **extension_configs: Any,
+        styles: dict[str, Any] | None = None,
+        disabled_messages: list[type[events.Message]] | None = None,
+        callbacks: dict[str, Callable] | None = None,
     ) -> None:
-        """Initialize the directory tree.
+        """Initialize the footer widget.
 
         Args:
-            path: Path to directory.
-            name: The name of the widget, or None for no name.
-            id: The ID of the widget in the DOM, or None for no ID.
-            classes: A space-separated list of classes, or None for no classes.
-            disabled: Whether the directory tree is disabled or not.
-            extension_configs: Widget extension configurations, such as dynamically provided local callbacks by name.
+            styles: Local inline styles to apply on top of the class' styles for only this instance.
+            disabled_messages: List of messages to disable on this widget instance only.
+            callbacks: Mapping of callbacks to send messages to instead of sending to default handler.
         """
-        super().__init__(
-            path=path,
-            name=name,
-            id=id,
-            classes=classes,
-            disabled=disabled,
+        super().__init__()
+        self.__extend_widget__(
+            styles=styles,
+            disabled_messages=disabled_messages,
+            callbacks=callbacks,
         )
-        self.__extend_widget__(**extension_configs)
```

### Comparing `textology-0.2.1/textology/widgets/_textual/_markdown.py` & `textology-0.3.0/textology/widgets/_textual/_markdown.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Extended Textual Markdown widgets."""
 
 from typing import Any
 from typing import Callable
 
+from textual import events
 from textual import widgets
 from textual.widgets._markdown import MarkdownIt
 
 from .._extensions import WidgetExtension
 
 
 class Markdown(WidgetExtension, widgets.Markdown):
@@ -16,65 +17,81 @@
         self,
         markdown: str | None = None,
         *,
         name: str | None = None,
         id: str | None = None,
         classes: str | None = None,
         parser_factory: Callable[[], MarkdownIt] | None = None,
-        **extension_configs: Any,
+        styles: dict[str, Any] | None = None,
+        disabled_messages: list[type[events.Message]] | None = None,
+        callbacks: dict[str, Callable] | None = None,
     ) -> None:
         """Initialize a Markdown widget.
 
         Args:
             markdown: String containing Markdown or None to leave blank for now.
             name: The name of the widget.
             id: The ID of the widget in the DOM.
             classes: The CSS classes of the widget.
             parser_factory: A factory function to return a configured MarkdownIt instance.
                 If "None`, a "gfm-like" parser is used.
-            extension_configs: Widget extension configurations, such as dynamically provided local callbacks by name.
+            styles: Local inline styles to apply on top of the class' styles for only this instance.
+            disabled_messages: List of messages to disable on this widget instance only.
+            callbacks: Mapping of callbacks to send messages to instead of sending to default handler.
         """
         super().__init__(
             markdown=markdown,
             name=name,
             id=id,
             classes=classes,
             parser_factory=parser_factory,
         )
-        self.__extend_widget__(**extension_configs)
+        self.__extend_widget__(
+            styles=styles,
+            disabled_messages=disabled_messages,
+            callbacks=callbacks,
+        )
 
 
 class MarkdownViewer(WidgetExtension, widgets.MarkdownViewer):
     """An extended Markdown viewer widget."""
 
     def __init__(
         self,
         markdown: str | None = None,
         *,
         show_table_of_contents: bool = True,
         name: str | None = None,
         id: str | None = None,
         classes: str | None = None,
         parser_factory: Callable[[], MarkdownIt] | None = None,
-        **extension_configs: Any,
+        styles: dict[str, Any] | None = None,
+        disabled_messages: list[type[events.Message]] | None = None,
+        callbacks: dict[str, Callable] | None = None,
     ) -> None:
         """Initialize a Markdown Viewer widget.
 
         Args:
             markdown: String containing Markdown, or None to leave blank.
             show_table_of_contents: Show a table of contents in a sidebar.
             name: The name of the widget.
             id: The ID of the widget in the DOM.
             classes: The CSS classes of the widget.
             parser_factory: A factory function to return a configured MarkdownIt instance.
                 If "None", a "gfm-like" parser is used.
-            extension_configs: Widget extension configurations, such as dynamically provided local callbacks by name.
+            styles: Local inline styles to apply on top of the class' styles for only this instance.
+            disabled_messages: List of messages to disable on this widget instance only.
+            callbacks: Mapping of callbacks to send messages to instead of sending to default handler.
         """
         super().__init__(
             markdown=markdown,
             show_table_of_contents=show_table_of_contents,
             name=name,
             id=id,
             classes=classes,
             parser_factory=parser_factory,
         )
-        self.__extend_widget__(**extension_configs)
+        self.__extend_widget__(
+            styles=styles,
+            disabled_messages=disabled_messages,
+            callbacks=callbacks,
+        )
```

### Comparing `textology-0.2.1/textology/widgets/_textual/_option_list.py` & `textology-0.3.0/textology/widgets/_textual/_option_list.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """Extended Textual OptionList widget."""
 
 from typing import Any
+from typing import Callable
 
+from textual import events
 from textual import widgets
 from textual.widgets._option_list import NewOptionListContent
 
 from .._extensions import WidgetExtension
 
 
 class OptionList(WidgetExtension, widgets.OptionList):
@@ -14,27 +16,35 @@
     def __init__(
         self,
         *content: NewOptionListContent,
         name: str | None = None,
         id: str | None = None,
         classes: str | None = None,
         disabled: bool = False,
-        **extension_configs: Any,
+        styles: dict[str, Any] | None = None,
+        disabled_messages: list[type[events.Message]] | None = None,
+        callbacks: dict[str, Callable] | None = None,
     ) -> None:
         """Initialize the option list.
 
         Args:
             *content: The content for the option list.
             name: The name of the option list.
             id: The ID of the option list in the DOM.
             classes: The CSS classes of the option list.
             disabled: Whether the option list is disabled or not.
-            extension_configs: Widget extension configurations, such as dynamically provided local callbacks by name.
+            styles: Local inline styles to apply on top of the class' styles for only this instance.
+            disabled_messages: List of messages to disable on this widget instance only.
+            callbacks: Mapping of callbacks to send messages to instead of sending to default handler.
         """
         super().__init__(
             *content,
             name=name,
             id=id,
             classes=classes,
             disabled=disabled,
         )
-        self.__extend_widget__(**extension_configs)
+        self.__extend_widget__(
+            styles=styles,
+            disabled_messages=disabled_messages,
+            callbacks=callbacks,
+        )
```

### Comparing `textology-0.2.1/textology/widgets/_textual/_radio_set.py` & `textology-0.3.0/textology/widgets/_textual/_pretty.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,53 @@
-"""Extended Textual RadioSet widget."""
+"""Extended Textual Pretty widget."""
 
 from typing import Any
+from typing import Callable
 
+from textual import events
 from textual import widgets
 
 from .._extensions import WidgetExtension
 
 
-class RadioSet(WidgetExtension, widgets.RadioSet):
-    """Widget for grouping a collection of radio buttons into a set."""
+class Pretty(WidgetExtension, widgets.Pretty):
+    """An extended pretty-printing widget."""
+
+    DEFAULT_CSS = """
+    Pretty {
+        height: auto;
+    }
+    """
 
     def __init__(
         self,
-        *buttons: str | widgets.RadioButton,
+        obj: Any,
+        *,
         name: str | None = None,
         id: str | None = None,
         classes: str | None = None,
-        disabled: bool = False,
-        **extension_configs: Any,
+        styles: dict[str, Any] | None = None,
+        disabled_messages: list[type[events.Message]] | None = None,
+        callbacks: dict[str, Callable] | None = None,
     ) -> None:
-        """Initialize the radio set.
+        """Initialize the Pretty widget.
 
         Args:
-            buttons: A collection of labels or "RadioButton"(s) to group together.
-            name: The name of the radio set.
-            id: The ID of the radio set in the DOM.
-            classes: The CSS classes of the radio set.
-            disabled: Whether the radio set is disabled or not.
-            extension_configs: Widget extension configurations, such as dynamically provided local callbacks by name.
+            obj: The object to pretty-print.
+            name: The name of the pretty widget.
+            id: The ID of the pretty in the DOM.
+            classes: The CSS classes of the pretty.
+            styles: Local inline styles to apply on top of the class' styles for only this instance.
+            disabled_messages: List of messages to disable on this widget instance only.
+            callbacks: Mapping of callbacks to send messages to instead of sending to default handler.
         """
         super().__init__(
-            *buttons,
+            object=obj,
             name=name,
             id=id,
             classes=classes,
-            disabled=disabled,
         )
-        self.__extend_widget__(**extension_configs)
+        self.__extend_widget__(
+            styles=styles,
+            disabled_messages=disabled_messages,
+            callbacks=callbacks,
+        )
```

### Comparing `textology-0.2.1/textology/widgets/_textual/_switch.py` & `textology-0.3.0/textology/widgets/_textual/_switch.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """Extended Textual Switch widget."""
 
 from typing import Any
+from typing import Callable
 
+from textual import events
 from textual import widgets
 
 from .._extensions import WidgetExtension
 
 
 class Switch(WidgetExtension, widgets.Switch):
     """An extended switch widget that represents a boolean value."""
@@ -15,29 +17,37 @@
         value: bool = False,
         *,
         animate: bool = True,
         name: str | None = None,
         id: str | None = None,
         classes: str | None = None,
         disabled: bool = False,
-        **extension_configs: Any,
+        styles: dict[str, Any] | None = None,
+        disabled_messages: list[type[events.Message]] | None = None,
+        callbacks: dict[str, Callable] | None = None,
     ) -> None:
         """Initialize the switch.
 
         Args:
             value: The initial value of the switch.
             animate: True if the switch should animate when toggled.
             name: The name of the switch.
             id: The ID of the switch in the DOM.
             classes: The CSS classes of the switch.
             disabled: Whether the switch is disabled or not.
-            extension_configs: Widget extension configurations, such as dynamically provided local callbacks by name.
+            styles: Local inline styles to apply on top of the class' styles for only this instance.
+            disabled_messages: List of messages to disable on this widget instance only.
+            callbacks: Mapping of callbacks to send messages to instead of sending to default handler.
         """
         super().__init__(
             value,
             animate=animate,
             name=name,
             id=id,
             classes=classes,
             disabled=disabled,
         )
-        self.__extend_widget__(**extension_configs)
+        self.__extend_widget__(
+            styles=styles,
+            disabled_messages=disabled_messages,
+            callbacks=callbacks,
+        )
```

### Comparing `textology-0.2.1/textology/widgets/_textual/_text_input.py` & `textology-0.3.0/textology/widgets/_textual/_text_input.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """Extended Textual Input widget."""
 
 from typing import Any
+from typing import Callable
 from typing import Iterable
 
 from rich.highlighter import Highlighter
+from textual import events
 from textual import widgets
 from textual.suggester import Suggester
 from textual.validation import Validator
 
 from .._extensions import WidgetExtension
 
 
@@ -26,37 +28,45 @@
         *,
         suggester: Suggester | None = None,
         validators: Validator | Iterable[Validator] | None = None,
         name: str | None = None,
         id: str | None = None,
         classes: str | None = None,
         disabled: bool = False,
-        **extension_configs: Any,
+        styles: dict[str, Any] | None = None,
+        disabled_messages: list[type[events.Message]] | None = None,
+        callbacks: dict[str, Callable] | None = None,
     ) -> None:
         """Initialize the text input widget.
 
         Args:
             value: An optional default value for the input.
             placeholder: Optional placeholder text for the input.
             highlighter: An optional highlighter for the input.
             password: Flag to say if the field should obfuscate its content.
             suggester: Suggester associated with this input instance.
             validators: An iterable of validators that the Input value will be checked against.
             name: Optional name for the input widget.
             id: Optional ID for the widget.
             classes: Optional initial classes for the widget.
             disabled: Whether the input is disabled or not.
-            extension_configs: Widget extension configurations, such as dynamically provided local callbacks by name.
+            styles: Local inline styles to apply on top of the class' styles for only this instance.
+            disabled_messages: List of messages to disable on this widget instance only.
+            callbacks: Mapping of callbacks to send messages to instead of sending to default handler.
         """
         super().__init__(
             value=value,
             placeholder=placeholder,
             highlighter=highlighter,
             password=password,
             suggester=suggester,
             validators=validators,
             name=name,
             id=id,
             classes=classes,
             disabled=disabled,
         )
-        self.__extend_widget__(**extension_configs)
+        self.__extend_widget__(
+            styles=styles,
+            disabled_messages=disabled_messages,
+            callbacks=callbacks,
+        )
```

### Comparing `textology-0.2.1/textology/widgets/_textual/_text_log.py` & `textology-0.3.0/textology/widgets/_textual/_text_log.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """Extended Textual TextLog widget."""
 
 from typing import Any
+from typing import Callable
 
+from textual import events
 from textual import widgets
 
 from .._extensions import WidgetExtension
 
 
 class TextLog(WidgetExtension, widgets.TextLog):
     """An extended widget for logging text."""
@@ -19,37 +21,45 @@
         highlight: bool = False,
         markup: bool = False,
         auto_scroll: bool = True,
         name: str | None = None,
         id: str | None = None,
         classes: str | None = None,
         disabled: bool = False,
-        **extension_configs: Any,
+        styles: dict[str, Any] | None = None,
+        disabled_messages: list[type[events.Message]] | None = None,
+        callbacks: dict[str, Callable] | None = None,
     ) -> None:
         """Initialize a TextLog widget.
 
         Args:
             max_lines: Maximum number of lines in the log or `None` for no maximum.
             min_width: Minimum width of renderables.
             wrap: Enable word wrapping (default is off).
             highlight: Automatically highlight content.
             markup: Apply Rich console markup.
             auto_scroll: Enable automatic scrolling to end.
             name: The name of the text log.
             id: The ID of the text log in the DOM.
             classes: The CSS classes of the text log.
             disabled: Whether the text log is disabled or not.
-            extension_configs: Widget extension configurations, such as dynamically provided local callbacks by name.
+            styles: Local inline styles to apply on top of the class' styles for only this instance.
+            disabled_messages: List of messages to disable on this widget instance only.
+            callbacks: Mapping of callbacks to send messages to instead of sending to default handler.
         """
         super().__init__(
             max_lines=max_lines,
             min_width=min_width,
             wrap=wrap,
             highlight=highlight,
             markup=markup,
             auto_scroll=auto_scroll,
             name=name,
             id=id,
             classes=classes,
             disabled=disabled,
         )
-        self.__extend_widget__(**extension_configs)
+        self.__extend_widget__(
+            styles=styles,
+            disabled_messages=disabled_messages,
+            callbacks=callbacks,
+        )
```

### Comparing `textology-0.2.1/textology.egg-info/PKG-INFO` & `textology-0.3.0/textology.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textology
-Version: 0.2.1
+Version: 0.3.0
 Summary: Textual extensions for creating Terminal User Interfaces
 Home-page: https://github.com/dfrtz/textology
 Author: David Fritz
 License: MIT
 Project-URL: Issue Tracker, https://github.com/dfrtz/textology/issues
 Project-URL: Source Code, https://github.com/dfrtz/textology
 Platform: MacOS
@@ -377,15 +377,15 @@
 ```python
 from textology.widgets import Button
 
 def on_click(event):
     print("Don't press my buttons...")
 
 button = Button(
-    on_button_pressed=on_click,
+    callbacks={"on_button_pressed": on_click},
 )
 ```
 
 - Instance style extension (set styles directly at instantiation based on logic):
 ```python
 from textology.widgets import Button
 
@@ -400,15 +400,15 @@
 
 - Instance message disable extension (avoid unused event chains, such as in large ListViews):
 ```python
 from textual import events
 from textology.widgets import ListItem
 
 item = ListItem(
-    disable_messages=[events.Mount, events.Show],
+    disabled_messages=[events.Mount, events.Show],
 )
 ```
 
 ### Extended Testing
 
 Don't want to serialize your pytests? Looking for the ability to quickly visualize differences when UIs change?
 You came to the right place. Textology extends Textual SVG snapshot capabilities to add support for parallel processing
```

### Comparing `textology-0.2.1/textology.egg-info/SOURCES.txt` & `textology-0.3.0/textology.egg-info/SOURCES.txt`

 * *Files identical despite different names*

