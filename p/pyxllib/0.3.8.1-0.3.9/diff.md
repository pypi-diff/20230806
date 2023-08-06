# Comparing `tmp/pyxllib-0.3.8.1.tar.gz` & `tmp/pyxllib-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxllib-0.3.8.1.tar", last modified: Thu Oct 13 10:38:47 2022, max compression
+gzip compressed data, was "pyxllib-0.3.9.tar", last modified: Tue Oct 18 02:03:36 2022, max compression
```

## Comparing `pyxllib-0.3.8.1.tar` & `pyxllib-0.3.9.tar`

### file list

```diff
@@ -1,385 +1,385 @@
-drwxrwxrwx   0        0        0        0 2022-10-13 10:38:47.317240 pyxllib-0.3.8.1/
--rw-rw-rw-   0        0        0    10443 2020-05-30 01:21:59.000000 pyxllib-0.3.8.1/LICENSE
--rw-rw-rw-   0        0        0       80 2022-04-14 09:35:06.000000 pyxllib-0.3.8.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1091 2022-10-13 10:38:47.317240 pyxllib-0.3.8.1/PKG-INFO
--rw-rw-rw-   0        0        0      441 2022-02-25 06:57:44.000000 pyxllib-0.3.8.1/README.md
-drwxrwxrwx   0        0        0        0 2022-10-13 10:38:45.276387 pyxllib-0.3.8.1/pyxllib/
--rw-rw-rw-   0        0        0      529 2022-06-24 02:18:32.000000 pyxllib-0.3.8.1/pyxllib/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-13 10:38:45.351187 pyxllib-0.3.8.1/pyxllib/algo/
--rw-rw-rw-   0        0        0      161 2021-06-03 14:47:35.000000 pyxllib-0.3.8.1/pyxllib/algo/__init__.py
--rw-rw-rw-   0        0        0     1282 2021-10-09 09:44:24.000000 pyxllib-0.3.8.1/pyxllib/algo/disjoint.py
--rw-rw-rw-   0        0        0    18190 2022-09-12 12:59:06.000000 pyxllib-0.3.8.1/pyxllib/algo/geo.py
--rw-rw-rw-   0        0        0    36718 2022-10-06 01:42:08.000000 pyxllib-0.3.8.1/pyxllib/algo/intervals.py
--rw-rw-rw-   0        0        0     4168 2022-02-26 07:37:55.000000 pyxllib-0.3.8.1/pyxllib/algo/newbie.py
--rw-rw-rw-   0        0        0    15611 2022-08-13 13:39:38.000000 pyxllib-0.3.8.1/pyxllib/algo/pupil.py
--rw-rw-rw-   0        0        0     2393 2021-06-23 06:19:33.000000 pyxllib-0.3.8.1/pyxllib/algo/shapelylib.py
--rw-rw-rw-   0        0        0     8584 2021-08-03 09:17:26.000000 pyxllib-0.3.8.1/pyxllib/algo/specialist.py
--rw-rw-rw-   0        0        0    12884 2022-09-13 08:15:15.000000 pyxllib-0.3.8.1/pyxllib/algo/stat.py
--rw-rw-rw-   0        0        0     5094 2022-07-04 01:30:35.000000 pyxllib-0.3.8.1/pyxllib/algo/treelib.py
--rw-rw-rw-   0        0        0     1953 2022-03-16 03:08:01.000000 pyxllib-0.3.8.1/pyxllib/algo/unitlib.py
-drwxrwxrwx   0        0        0        0 2022-10-13 10:38:45.410030 pyxllib-0.3.8.1/pyxllib/cv/
--rw-rw-rw-   0        0        0      132 2021-06-03 15:42:25.000000 pyxllib-0.3.8.1/pyxllib/cv/__init__.py
--rw-rw-rw-   0        0        0     5054 2022-09-13 08:21:17.000000 pyxllib-0.3.8.1/pyxllib/cv/expert.py
--rw-rw-rw-   0        0        0     6757 2021-06-25 09:32:56.000000 pyxllib-0.3.8.1/pyxllib/cv/imfile.py
--rw-rw-rw-   0        0        0      907 2022-09-01 08:06:20.000000 pyxllib-0.3.8.1/pyxllib/cv/imhash.py
--rw-rw-rw-   0        0        0      339 2022-05-05 11:22:25.000000 pyxllib-0.3.8.1/pyxllib/cv/pupil.py
--rw-rw-rw-   0        0        0    38224 2022-06-12 09:01:30.000000 pyxllib-0.3.8.1/pyxllib/cv/rgbfmt.py
--rw-rw-rw-   0        0        0     9259 2022-09-13 06:56:02.000000 pyxllib-0.3.8.1/pyxllib/cv/trackbartools.py
--rw-rw-rw-   0        0        0    38288 2022-09-27 02:50:20.000000 pyxllib-0.3.8.1/pyxllib/cv/xlcvlib.py
--rw-rw-rw-   0        0        0    14998 2022-10-09 07:09:36.000000 pyxllib-0.3.8.1/pyxllib/cv/xlpillib.py
-drwxrwxrwx   0        0        0        0 2022-10-13 10:38:45.439950 pyxllib-0.3.8.1/pyxllib/data/
--rw-rw-rw-   0        0        0        0 2021-06-10 06:26:12.000000 pyxllib-0.3.8.1/pyxllib/data/__init__.py
--rw-rw-rw-   0        0        0     3659 2022-09-13 06:56:02.000000 pyxllib-0.3.8.1/pyxllib/data/echarts.py
--rw-rw-rw-   0        0        0     2477 2021-10-09 09:43:21.000000 pyxllib-0.3.8.1/pyxllib/data/oss.py
--rw-rw-rw-   0        0        0    24425 2022-09-28 06:11:36.000000 pyxllib-0.3.8.1/pyxllib/data/pglib.py
--rw-rw-rw-   0        0        0     6709 2022-10-04 08:12:19.000000 pyxllib-0.3.8.1/pyxllib/data/sqlite.py
--rw-rw-rw-   0        0        0    11955 2021-10-09 09:40:53.000000 pyxllib-0.3.8.1/pyxllib/data/sqllib.py
-drwxrwxrwx   0        0        0        0 2022-10-13 10:38:45.515749 pyxllib-0.3.8.1/pyxllib/extend/
--rw-rw-rw-   0        0        0      134 2022-09-13 07:42:34.000000 pyxllib-0.3.8.1/pyxllib/extend/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-13 10:38:45.537688 pyxllib-0.3.8.1/pyxllib/extend/autogui/
--rw-rw-rw-   0        0        0      229 2022-09-13 08:23:33.000000 pyxllib-0.3.8.1/pyxllib/extend/autogui/__init__.py
--rw-rw-rw-   0        0        0    25358 2022-09-27 06:29:43.000000 pyxllib-0.3.8.1/pyxllib/extend/autogui/autogui.py
--rw-rw-rw-   0        0        0     3654 2021-08-03 11:27:22.000000 pyxllib-0.3.8.1/pyxllib/extend/autogui/virtualkey.py
--rw-rw-rw-   0        0        0     8552 2022-06-30 06:11:06.000000 pyxllib-0.3.8.1/pyxllib/extend/demolib.py
--rw-rw-rw-   0        0        0    27407 2022-09-13 08:24:35.000000 pyxllib-0.3.8.1/pyxllib/extend/old.py
--rw-rw-rw-   0        0        0     9966 2022-07-12 08:13:02.000000 pyxllib-0.3.8.1/pyxllib/extend/qt.py
--rw-rw-rw-   0        0        0     5004 2021-06-06 12:23:02.000000 pyxllib-0.3.8.1/pyxllib/extend/tk.py
--rw-rw-rw-   0        0        0    34930 2022-09-14 03:21:11.000000 pyxllib-0.3.8.1/pyxllib/extend/unixlib.py
--rw-rw-rw-   0        0        0    13016 2022-09-13 08:26:05.000000 pyxllib-0.3.8.1/pyxllib/extend/utools.py
--rw-rw-rw-   0        0        0     2922 2021-06-06 12:45:02.000000 pyxllib-0.3.8.1/pyxllib/extend/webhook.py
--rw-rw-rw-   0        0        0     1237 2021-12-19 10:33:17.000000 pyxllib-0.3.8.1/pyxllib/extend/win32lib.py
-drwxrwxrwx   0        0        0        0 2022-10-13 10:38:45.593538 pyxllib-0.3.8.1/pyxllib/file/
--rw-rw-rw-   0        0        0      452 2021-06-03 15:43:58.000000 pyxllib-0.3.8.1/pyxllib/file/__init__.py
--rw-rw-rw-   0        0        0    29443 2022-09-23 06:45:05.000000 pyxllib-0.3.8.1/pyxllib/file/docxlib.py
--rw-rw-rw-   0        0        0    11620 2022-09-13 08:19:54.000000 pyxllib-0.3.8.1/pyxllib/file/gitlib.py
--rw-rw-rw-   0        0        0     5880 2022-07-05 06:50:20.000000 pyxllib-0.3.8.1/pyxllib/file/movielib.py
--rw-rw-rw-   0        0        0      218 2021-06-06 09:44:33.000000 pyxllib-0.3.8.1/pyxllib/file/newbie.py
--rw-rw-rw-   0        0        0    54951 2022-09-14 02:44:42.000000 pyxllib-0.3.8.1/pyxllib/file/onenotelib.py
-drwxrwxrwx   0        0        0        0 2022-10-13 10:38:45.607501 pyxllib-0.3.8.1/pyxllib/file/packlib/
--rw-rw-rw-   0        0        0     7085 2022-07-05 07:09:24.000000 pyxllib-0.3.8.1/pyxllib/file/packlib/__init__.py
--rw-rw-rw-   0        0        0    90165 2022-02-15 02:13:17.000000 pyxllib-0.3.8.1/pyxllib/file/packlib/zipfile.py
--rw-rw-rw-   0        0        0    16927 2022-09-13 08:20:38.000000 pyxllib-0.3.8.1/pyxllib/file/pdflib.py
--rw-rw-rw-   0        0        0     5997 2021-10-17 07:30:24.000000 pyxllib-0.3.8.1/pyxllib/file/pupil.py
-drwxrwxrwx   0        0        0        0 2022-10-13 10:38:45.624456 pyxllib-0.3.8.1/pyxllib/file/specialist/
--rw-rw-rw-   0        0        0      277 2021-06-30 06:21:43.000000 pyxllib-0.3.8.1/pyxllib/file/specialist/__init__.py
--rw-rw-rw-   0        0        0    32216 2022-09-13 08:19:04.000000 pyxllib-0.3.8.1/pyxllib/file/specialist/dirlib.py
--rw-rw-rw-   0        0        0     6534 2022-09-09 07:59:04.000000 pyxllib-0.3.8.1/pyxllib/file/specialist/download.py
--rw-rw-rw-   0        0        0    65428 2022-09-13 08:19:21.000000 pyxllib-0.3.8.1/pyxllib/file/specialist/filelib.py
--rw-rw-rw-   0        0        0    36528 2022-09-13 08:20:58.000000 pyxllib-0.3.8.1/pyxllib/file/xlsxlib.py
-drwxrwxrwx   0        0        0        0 2022-10-13 10:38:45.646397 pyxllib-0.3.8.1/pyxllib/prog/
--rw-rw-rw-   0        0        0      132 2021-06-03 15:22:15.000000 pyxllib-0.3.8.1/pyxllib/prog/__init__.py
--rw-rw-rw-   0        0        0     8499 2021-06-05 17:05:47.000000 pyxllib-0.3.8.1/pyxllib/prog/deprecatedlib.py
--rw-rw-rw-   0        0        0    11982 2022-09-13 06:49:51.000000 pyxllib-0.3.8.1/pyxllib/prog/newbie.py
--rw-rw-rw-   0        0        0    33283 2022-09-27 06:09:15.000000 pyxllib-0.3.8.1/pyxllib/prog/pupil.py
--rw-rw-rw-   0        0        0      996 2021-06-06 08:23:35.000000 pyxllib-0.3.8.1/pyxllib/prog/sitepackages.py
-drwxrwxrwx   0        0        0        0 2022-10-13 10:38:45.727182 pyxllib-0.3.8.1/pyxllib/prog/specialist/
--rw-rw-rw-   0        0        0     8230 2022-09-13 06:56:02.000000 pyxllib-0.3.8.1/pyxllib/prog/specialist/__init__.py
--rw-rw-rw-   0        0        0     9644 2022-09-29 06:23:13.000000 pyxllib-0.3.8.1/pyxllib/prog/specialist/bc.py
--rw-rw-rw-   0        0        0    19775 2022-09-13 08:33:02.000000 pyxllib-0.3.8.1/pyxllib/prog/specialist/browser.py
--rw-rw-rw-   0        0        0    13309 2022-04-09 12:50:47.000000 pyxllib-0.3.8.1/pyxllib/prog/specialist/common.py
--rw-rw-rw-   0        0        0     4527 2022-03-16 02:37:13.000000 pyxllib-0.3.8.1/pyxllib/prog/specialist/datetime.py
--rw-rw-rw-   0        0        0     8206 2022-09-13 08:14:07.000000 pyxllib-0.3.8.1/pyxllib/prog/specialist/tictoc.py
--rw-rw-rw-   0        0        0     8289 2022-09-13 08:14:20.000000 pyxllib-0.3.8.1/pyxllib/prog/specialist/xllog.py
-drwxrwxrwx   0        0        0        0 2022-10-13 10:38:45.733165 pyxllib-0.3.8.1/pyxllib/stdlib/
--rw-rw-rw-   0        0        0      581 2022-02-15 02:25:06.000000 pyxllib-0.3.8.1/pyxllib/stdlib/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-13 10:38:45.754110 pyxllib-0.3.8.1/pyxllib/stdlib/tablepyxl/
--rw-rw-rw-   0        0        0      193 2021-06-03 09:24:15.000000 pyxllib-0.3.8.1/pyxllib/stdlib/tablepyxl/__init__.py
--rw-rw-rw-   0        0        0    10924 2022-04-22 12:23:11.000000 pyxllib-0.3.8.1/pyxllib/stdlib/tablepyxl/style.py
--rw-rw-rw-   0        0        0     4531 2022-04-22 12:23:21.000000 pyxllib-0.3.8.1/pyxllib/stdlib/tablepyxl/tablepyxl.py
-drwxrwxrwx   0        0        0        0 2022-10-13 10:38:45.794002 pyxllib-0.3.8.1/pyxllib/text/
--rw-rw-rw-   0        0        0      170 2021-06-03 14:58:07.000000 pyxllib-0.3.8.1/pyxllib/text/__init__.py
--rw-rw-rw-   0        0        0     1259 2021-10-09 09:37:54.000000 pyxllib-0.3.8.1/pyxllib/text/ahocorasick.py
-drwxrwxrwx   0        0        0        0 2022-10-13 10:38:45.799987 pyxllib-0.3.8.1/pyxllib/text/latex/
--rw-rw-rw-   0        0        0     6416 2022-09-13 08:15:50.000000 pyxllib-0.3.8.1/pyxllib/text/latex/__init__.py
--rw-rw-rw-   0        0        0     4310 2022-09-13 08:17:11.000000 pyxllib-0.3.8.1/pyxllib/text/levenshtein.py
--rw-rw-rw-   0        0        0    49235 2022-10-13 08:50:28.000000 pyxllib-0.3.8.1/pyxllib/text/nestenv.py
--rw-rw-rw-   0        0        0     7941 2022-05-19 02:34:37.000000 pyxllib-0.3.8.1/pyxllib/text/newbie.py
-drwxrwxrwx   0        0        0        0 2022-10-13 10:38:45.814947 pyxllib-0.3.8.1/pyxllib/text/pupil/
--rw-rw-rw-   0        0        0      217 2021-06-06 09:36:42.000000 pyxllib-0.3.8.1/pyxllib/text/pupil/__init__.py
--rw-rw-rw-   0        0        0    31077 2022-09-13 08:16:22.000000 pyxllib-0.3.8.1/pyxllib/text/pupil/common.py
--rw-rw-rw-   0        0        0    10985 2021-07-17 02:50:04.000000 pyxllib-0.3.8.1/pyxllib/text/pupil/xlalign.py
--rw-rw-rw-   0        0        0     1585 2022-09-13 08:06:32.000000 pyxllib-0.3.8.1/pyxllib/text/pycode.py
-drwxrwxrwx   0        0        0        0 2022-10-13 10:38:45.829908 pyxllib-0.3.8.1/pyxllib/text/specialist/
--rw-rw-rw-   0        0        0      224 2021-09-23 01:54:34.000000 pyxllib-0.3.8.1/pyxllib/text/specialist/__init__.py
--rw-rw-rw-   0        0        0     3935 2022-09-13 08:16:41.000000 pyxllib-0.3.8.1/pyxllib/text/specialist/common.py
--rw-rw-rw-   0        0        0     6686 2022-09-13 08:16:52.000000 pyxllib-0.3.8.1/pyxllib/text/specialist/ptag.py
--rw-rw-rw-   0        0        0     7706 2022-09-13 08:17:44.000000 pyxllib-0.3.8.1/pyxllib/text/spellchecker.py
--rw-rw-rw-   0        0        0    26666 2022-09-29 09:25:22.000000 pyxllib-0.3.8.1/pyxllib/text/xmllib.py
--rw-rw-rw-   0        0        0      698 2022-09-13 08:11:02.000000 pyxllib-0.3.8.1/pyxllib/xl.py
--rw-rw-rw-   0        0        0      652 2022-07-05 09:15:11.000000 pyxllib-0.3.8.1/pyxllib/xlcv.py
-drwxrwxrwx   0        0        0        0 2022-10-13 10:38:45.293341 pyxllib-0.3.8.1/pyxllib.egg-info/
--rw-rw-rw-   0        0        0     1091 2022-10-13 10:38:44.000000 pyxllib-0.3.8.1/pyxllib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    11453 2022-10-13 10:38:45.000000 pyxllib-0.3.8.1/pyxllib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-13 10:38:44.000000 pyxllib-0.3.8.1/pyxllib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      323 2022-10-13 10:38:44.000000 pyxllib-0.3.8.1/pyxllib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2022-10-13 10:38:44.000000 pyxllib-0.3.8.1/pyxllib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-10-13 10:38:45.844867 pyxllib-0.3.8.1/pyxlpr/
--rw-rw-rw-   0        0        0      126 2022-04-14 01:52:38.000000 pyxllib-0.3.8.1/pyxlpr/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-13 10:38:45.882766 pyxllib-0.3.8.1/pyxlpr/ai/
--rw-rw-rw-   0        0        0      132 2021-06-03 14:16:46.000000 pyxllib-0.3.8.1/pyxlpr/ai/__init__.py
--rw-rw-rw-   0        0        0    49872 2022-09-28 08:53:04.000000 pyxllib-0.3.8.1/pyxlpr/ai/clientlib.py
--rw-rw-rw-   0        0        0     9682 2022-06-30 06:26:38.000000 pyxllib-0.3.8.1/pyxlpr/ai/specialist.py
--rw-rw-rw-   0        0        0     6591 2022-09-14 02:36:54.000000 pyxllib-0.3.8.1/pyxlpr/ai/torch_app.py
--rw-rw-rw-   0        0        0    24956 2022-08-16 07:21:21.000000 pyxllib-0.3.8.1/pyxlpr/ai/xlpaddle.py
--rw-rw-rw-   0        0        0    29450 2022-07-19 09:30:02.000000 pyxllib-0.3.8.1/pyxlpr/ai/xltorch.py
-drwxrwxrwx   0        0        0        0 2022-10-13 10:38:45.939253 pyxllib-0.3.8.1/pyxlpr/data/
--rw-rw-rw-   0        0        0      281 2021-07-29 01:04:03.000000 pyxllib-0.3.8.1/pyxlpr/data/__init__.py
--rw-rw-rw-   0        0        0    57147 2022-09-19 08:15:27.000000 pyxllib-0.3.8.1/pyxlpr/data/coco.py
--rw-rw-rw-   0        0        0    14619 2022-04-14 02:38:30.000000 pyxllib-0.3.8.1/pyxlpr/data/datacls.py
--rw-rw-rw-   0        0        0     8252 2021-10-21 08:58:12.000000 pyxllib-0.3.8.1/pyxlpr/data/datasets.py
-drwxrwxrwx   0        0        0        0 2022-10-13 10:38:45.971168 pyxllib-0.3.8.1/pyxlpr/data/icdar/
--rw-rw-rw-   0        0        0     4603 2022-08-30 02:50:10.000000 pyxllib-0.3.8.1/pyxlpr/data/icdar/__init__.py
--rw-rw-rw-   0        0        0    18077 2022-08-30 02:33:05.000000 pyxllib-0.3.8.1/pyxlpr/data/icdar/deteval.py
--rw-rw-rw-   0        0        0    16306 2022-08-30 02:31:32.000000 pyxllib-0.3.8.1/pyxlpr/data/icdar/icdar2013.py
--rw-rw-rw-   0        0        0    13859 2022-08-30 08:50:22.000000 pyxllib-0.3.8.1/pyxlpr/data/icdar/iou.py
--rw-rw-rw-   0        0        0    19740 2021-03-11 12:41:54.000000 pyxllib-0.3.8.1/pyxlpr/data/icdar/rrc_evaluation_funcs_1_1.py
--rw-rw-rw-   0        0        0    19054 2022-09-14 02:43:04.000000 pyxllib-0.3.8.1/pyxlpr/data/imtextline.py
--rw-rw-rw-   0        0        0    33925 2022-09-13 06:56:02.000000 pyxllib-0.3.8.1/pyxlpr/data/labelme.py
--rw-rw-rw-   0        0        0     6499 2021-09-08 06:16:36.000000 pyxllib-0.3.8.1/pyxlpr/data/removeline.py
--rw-rw-rw-   0        0        0     2066 2021-06-25 09:03:58.000000 pyxllib-0.3.8.1/pyxlpr/data/specialist.py
-drwxrwxrwx   0        0        0        0 2022-10-13 10:38:45.976155 pyxllib-0.3.8.1/pyxlpr/eval/
--rw-rw-rw-   0        0        0     2980 2022-04-24 02:55:19.000000 pyxllib-0.3.8.1/pyxlpr/eval/__init__.py
--rw-rw-rw-   0        0        0    32303 2022-09-13 06:56:02.000000 pyxllib-0.3.8.1/pyxlpr/paddleocr.py
-drwxrwxrwx   0        0        0        0 2022-10-13 10:38:45.981141 pyxllib-0.3.8.1/pyxlpr/ppocr/
--rw-rw-rw-   0        0        0      651 2022-04-14 01:50:28.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-13 10:38:45.249459 pyxllib-0.3.8.1/pyxlpr/ppocr/configs/
-drwxrwxrwx   0        0        0        0 2022-10-13 10:38:45.249459 pyxllib-0.3.8.1/pyxlpr/ppocr/configs/rec/
-drwxrwxrwx   0        0        0        0 2022-10-13 10:38:45.987124 pyxllib-0.3.8.1/pyxlpr/ppocr/configs/rec/multi_language/
--rw-rw-rw-   0        0        0     8633 2021-12-14 06:42:12.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/configs/rec/multi_language/generate_multi_language_configs.py
-drwxrwxrwx   0        0        0        0 2022-10-13 10:38:46.029013 pyxllib-0.3.8.1/pyxlpr/ppocr/data/
--rw-rw-rw-   0        0        0     5565 2022-04-14 09:57:11.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/data/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-13 10:38:46.150687 pyxllib-0.3.8.1/pyxlpr/ppocr/data/imaug/
--rw-rw-rw-   0        0        0     1053 2022-01-14 02:17:07.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/data/imaug/ColorJitter.py
--rw-rw-rw-   0        0        0     2395 2022-01-14 02:36:55.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/data/imaug/__init__.py
--rw-rw-rw-   0        0        0     6655 2022-04-14 09:57:17.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/data/imaug/copy_paste.py
--rw-rw-rw-   0        0        0    17757 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/data/imaug/east_process.py
--rw-rw-rw-   0        0        0     9565 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/data/imaug/gen_table_mask.py
--rw-rw-rw-   0        0        0     3791 2021-12-14 08:52:21.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/data/imaug/iaa_augment.py
--rw-rw-rw-   0        0        0    28912 2022-04-14 09:57:22.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/data/imaug/label_ops.py
--rw-rw-rw-   0        0        0     7144 2021-12-31 07:49:15.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/data/imaug/make_border_map.py
--rw-rw-rw-   0        0        0     4008 2022-01-14 02:17:07.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/data/imaug/make_pse_gt.py
--rw-rw-rw-   0        0        0     4898 2022-01-01 02:45:22.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/data/imaug/make_shrink_map.py
--rw-rw-rw-   0        0        0    15625 2022-04-10 05:57:02.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/data/imaug/operators.py
--rw-rw-rw-   0        0        0    36408 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/data/imaug/pg_process.py
--rw-rw-rw-   0        0        0     5591 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/data/imaug/randaugment.py
--rw-rw-rw-   0        0        0     8442 2022-01-14 02:43:40.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/data/imaug/random_crop_data.py
--rw-rw-rw-   0        0        0    17398 2022-01-14 02:44:43.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/data/imaug/rec_img_aug.py
--rw-rw-rw-   0        0        0    30175 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/data/imaug/sast_process.py
-drwxrwxrwx   0        0        0        0 2022-10-13 10:38:46.169637 pyxllib-0.3.8.1/pyxlpr/ppocr/data/imaug/text_image_aug/
--rw-rw-rw-   0        0        0      750 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/data/imaug/text_image_aug/__init__.py
--rw-rw-rw-   0        0        0     3557 2022-01-14 02:37:02.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/data/imaug/text_image_aug/augment.py
--rw-rw-rw-   0        0        0     6619 2022-01-14 02:37:07.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/data/imaug/text_image_aug/warp_mls.py
--rw-rw-rw-   0        0        0     4485 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/data/lmdb_dataset.py
--rw-rw-rw-   0        0        0     4235 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/data/pgnet_dataset.py
--rw-rw-rw-   0        0        0     4410 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/data/pubtab_dataset.py
--rw-rw-rw-   0        0        0    15429 2022-07-17 08:19:44.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/data/simple_dataset.py
-drwxrwxrwx   0        0        0        0 2022-10-13 10:38:46.297299 pyxllib-0.3.8.1/pyxlpr/ppocr/losses/
--rw-rw-rw-   0        0        0     1925 2022-01-14 02:46:47.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/losses/__init__.py
--rw-rw-rw-   0        0        0     1811 2022-01-14 02:17:07.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/losses/ace_loss.py
--rw-rw-rw-   0        0        0     4431 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/losses/basic_loss.py
--rw-rw-rw-   0        0        0     3581 2022-01-14 02:17:07.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/losses/center_loss.py
--rw-rw-rw-   0        0        0     1106 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/losses/cls_loss.py
--rw-rw-rw-   0        0        0     2497 2022-01-14 02:47:04.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/losses/combined_loss.py
--rw-rw-rw-   0        0        0     7682 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/losses/det_basic_loss.py
--rw-rw-rw-   0        0        0     3245 2022-01-01 03:12:22.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/losses/det_db_loss.py
--rw-rw-rw-   0        0        0     2338 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/losses/det_east_loss.py
--rw-rw-rw-   0        0        0     5872 2022-04-14 09:57:27.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/losses/det_pse_loss.py
--rw-rw-rw-   0        0        0     5197 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/losses/det_sast_loss.py
--rw-rw-rw-   0        0        0     9741 2022-01-14 02:48:26.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/losses/distillation_loss.py
--rw-rw-rw-   0        0        0     6716 2022-04-14 09:57:33.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/losses/e2e_pg_loss.py
--rw-rw-rw-   0        0        0     4779 2022-01-14 02:17:07.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/losses/kie_sdmgr_loss.py
--rw-rw-rw-   0        0        0     3860 2022-01-14 02:17:07.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/losses/rec_aster_loss.py
--rw-rw-rw-   0        0        0     1568 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/losses/rec_att_loss.py
--rw-rw-rw-   0        0        0     1761 2022-01-14 02:48:09.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/losses/rec_ctc_loss.py
--rw-rw-rw-   0        0        0     2570 2022-01-14 02:17:07.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/losses/rec_enhanced_ctc_loss.py
--rw-rw-rw-   0        0        0     1120 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/losses/rec_nrtr_loss.py
--rw-rw-rw-   0        0        0     1110 2022-01-14 02:17:07.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/losses/rec_sar_loss.py
--rw-rw-rw-   0        0        0     1864 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/losses/rec_srn_loss.py
--rw-rw-rw-   0        0        0     4735 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/losses/table_att_loss.py
-drwxrwxrwx   0        0        0        0 2022-10-13 10:38:46.374089 pyxllib-0.3.8.1/pyxlpr/ppocr/metrics/
--rw-rw-rw-   0        0        0     1526 2022-01-14 02:48:48.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/metrics/__init__.py
--rw-rw-rw-   0        0        0     1497 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/metrics/cls_metric.py
--rw-rw-rw-   0        0        0     3256 2021-12-17 11:27:16.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/metrics/det_metric.py
--rw-rw-rw-   0        0        0     2460 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/metrics/distillation_metric.py
--rw-rw-rw-   0        0        0     3278 2022-04-14 09:57:38.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/metrics/e2e_metric.py
--rw-rw-rw-   0        0        0    10453 2022-01-12 09:51:33.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/metrics/eval_det_iou.py
--rw-rw-rw-   0        0        0     2445 2022-01-14 02:17:07.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/metrics/kie_metric.py
--rw-rw-rw-   0        0        0     2637 2022-01-20 09:03:43.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/metrics/rec_metric.py
--rw-rw-rw-   0        0        0     1784 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/metrics/table_metric.py
-drwxrwxrwx   0        0        0        0 2022-10-13 10:38:45.252452 pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/
-drwxrwxrwx   0        0        0        0 2022-10-13 10:38:46.391045 pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/architectures/
--rw-rw-rw-   0        0        0     1058 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/architectures/__init__.py
--rw-rw-rw-   0        0        0     3373 2022-04-14 09:57:43.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/architectures/base_model.py
--rw-rw-rw-   0        0        0     2406 2022-04-14 09:57:49.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/architectures/distillation_model.py
-drwxrwxrwx   0        0        0        0 2022-10-13 10:38:46.460858 pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/backbones/
--rw-rw-rw-   0        0        0     2296 2022-01-14 02:51:49.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/backbones/__init__.py
--rw-rw-rw-   0        0        0     9218 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/backbones/det_mobilenet_v3.py
--rw-rw-rw-   0        0        0     8164 2022-01-14 02:52:14.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/backbones/det_resnet_vd.py
--rw-rw-rw-   0        0        0     9816 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/backbones/det_resnet_vd_sast.py
--rw-rw-rw-   0        0        0     9163 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/backbones/e2e_resnet_vd_pg.py
--rw-rw-rw-   0        0        0     6270 2022-01-14 02:17:07.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/backbones/kie_unet_sdmgr.py
--rw-rw-rw-   0        0        0     5677 2022-04-14 09:57:53.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/backbones/rec_mobilenet_v3.py
--rw-rw-rw-   0        0        0     8192 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/backbones/rec_mv1_enhance.py
--rw-rw-rw-   0        0        0     1883 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/backbones/rec_nrtr_mtb.py
--rw-rw-rw-   0        0        0     7365 2022-01-14 02:17:07.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/backbones/rec_resnet_31.py
--rw-rw-rw-   0        0        0     4714 2022-01-14 02:17:07.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/backbones/rec_resnet_aster.py
--rw-rw-rw-   0        0        0    11084 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/backbones/rec_resnet_fpn.py
--rw-rw-rw-   0        0        0     9715 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/backbones/rec_resnet_vd.py
-drwxrwxrwx   0        0        0        0 2022-10-13 10:38:46.587519 pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/heads/
--rw-rw-rw-   0        0        0     1799 2022-01-14 02:54:10.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/heads/__init__.py
--rw-rw-rw-   0        0        0     1694 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/heads/cls_head.py
--rw-rw-rw-   0        0        0     4333 2021-12-30 06:31:07.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/heads/det_db_head.py
--rw-rw-rw-   0        0        0     3836 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/heads/det_east_head.py
--rw-rw-rw-   0        0        0     1374 2022-01-14 02:17:07.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/heads/det_pse_head.py
--rw-rw-rw-   0        0        0     4880 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/heads/det_sast_head.py
--rw-rw-rw-   0        0        0     8013 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/heads/e2e_pg_head.py
--rw-rw-rw-   0        0        0     8314 2022-01-14 02:17:07.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/heads/kie_sdmgr_head.py
--rw-rw-rw-   0        0        0     6646 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/heads/multiheadAttention.py
--rw-rw-rw-   0        0        0    16232 2022-01-14 02:17:07.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/heads/rec_aster_head.py
--rw-rw-rw-   0        0        0     8171 2022-01-14 02:53:49.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/heads/rec_att_head.py
--rw-rw-rw-   0        0        0     3014 2022-01-14 02:53:42.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/heads/rec_ctc_head.py
--rw-rw-rw-   0        0        0    33928 2022-04-14 09:58:00.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/heads/rec_nrtr_head.py
--rw-rw-rw-   0        0        0    14454 2022-01-14 02:17:07.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/heads/rec_sar_head.py
--rw-rw-rw-   0        0        0    11171 2022-04-14 09:58:04.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/heads/rec_srn_head.py
--rw-rw-rw-   0        0        0    15211 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/heads/self_attention.py
--rw-rw-rw-   0        0        0    10680 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/heads/table_att_head.py
-drwxrwxrwx   0        0        0        0 2022-10-13 10:38:46.630404 pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/necks/
--rw-rw-rw-   0        0        0     1230 2022-01-14 02:53:27.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/necks/__init__.py
--rw-rw-rw-   0        0        0     4130 2021-12-30 06:26:52.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/necks/db_fpn.py
--rw-rw-rw-   0        0        0     6050 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/necks/east_fpn.py
--rw-rw-rw-   0        0        0     5113 2022-01-14 02:17:07.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/necks/fpn.py
--rw-rw-rw-   0        0        0    10185 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/necks/pg_fpn.py
--rw-rw-rw-   0        0        0     3149 2022-04-14 09:58:09.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/necks/rnn.py
--rw-rw-rw-   0        0        0    11150 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/necks/sast_fpn.py
--rw-rw-rw-   0        0        0     4306 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/necks/table_fpn.py
-drwxrwxrwx   0        0        0        0 2022-10-13 10:38:46.653343 pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/transforms/
--rw-rw-rw-   0        0        0     1009 2022-01-14 02:53:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/transforms/__init__.py
--rw-rw-rw-   0        0        0     5251 2022-01-14 02:17:07.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/transforms/stn.py
--rw-rw-rw-   0        0        0    11696 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/transforms/tps.py
--rw-rw-rw-   0        0        0     6923 2022-01-14 02:17:07.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/transforms/tps_spatial_transformer.py
-drwxrwxrwx   0        0        0        0 2022-10-13 10:38:46.681269 pyxllib-0.3.8.1/pyxlpr/ppocr/optimizer/
--rw-rw-rw-   0        0        0     2280 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/optimizer/__init__.py
--rw-rw-rw-   0        0        0     8587 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/optimizer/learning_rate.py
--rw-rw-rw-   0        0        0     2036 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/optimizer/lr_scheduler.py
--rw-rw-rw-   0        0        0     5476 2022-01-14 02:56:11.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/optimizer/optimizer.py
--rw-rw-rw-   0        0        0     1665 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/optimizer/regularizer.py
-drwxrwxrwx   0        0        0        0 2022-10-13 10:38:46.736122 pyxllib-0.3.8.1/pyxlpr/ppocr/postprocess/
--rw-rw-rw-   0        0        0     2201 2022-01-14 02:57:04.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/postprocess/__init__.py
--rw-rw-rw-   0        0        0     1323 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/postprocess/cls_postprocess.py
--rw-rw-rw-   0        0        0     8752 2022-01-01 03:08:09.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/postprocess/db_postprocess.py
--rw-rw-rw-   0        0        0     5238 2022-01-14 02:57:52.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/postprocess/east_postprocess.py
--rw-rw-rw-   0        0        0     5233 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/postprocess/locality_aware_nms.py
--rw-rw-rw-   0        0        0     1872 2022-04-14 09:58:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/postprocess/pg_postprocess.py
-drwxrwxrwx   0        0        0        0 2022-10-13 10:38:46.749087 pyxllib-0.3.8.1/pyxlpr/ppocr/postprocess/pse_postprocess/
--rw-rw-rw-   0        0        0      668 2022-01-14 02:17:07.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/postprocess/pse_postprocess/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-13 10:38:46.763059 pyxllib-0.3.8.1/pyxlpr/ppocr/postprocess/pse_postprocess/pse/
--rw-rw-rw-   0        0        0     1174 2022-01-14 02:17:07.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/postprocess/pse_postprocess/pse/__init__.py
--rw-rw-rw-   0        0        0      340 2022-01-14 02:17:07.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/postprocess/pse_postprocess/pse/setup.py
--rw-rw-rw-   0        0        0     4172 2022-04-14 09:58:17.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/postprocess/pse_postprocess/pse_postprocess.py
--rw-rw-rw-   0        0        0    25827 2022-01-24 07:22:21.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/postprocess/rec_postprocess.py
--rw-rw-rw-   0        0        0    14016 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/postprocess/sast_postprocess.py
-drwxrwxrwx   0        0        0        0 2022-10-13 10:38:46.847827 pyxllib-0.3.8.1/pyxlpr/ppocr/tools/
--rw-rw-rw-   0        0        0      708 2022-01-14 02:59:47.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/tools/__init__.py
--rw-rw-rw-   0        0        0     3132 2022-04-14 09:58:24.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/tools/eval.py
--rw-rw-rw-   0        0        0     2777 2022-04-27 02:43:32.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/tools/export_center.py
--rw-rw-rw-   0        0        0     5319 2022-04-14 09:58:35.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/tools/export_model.py
-drwxrwxrwx   0        0        0        0 2022-10-13 10:38:46.886723 pyxllib-0.3.8.1/pyxlpr/ppocr/tools/infer/
--rw-rw-rw-   0        0        0     5927 2022-04-27 02:43:57.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/tools/infer/predict_cls.py
--rw-rw-rw-   0        0        0    11911 2022-04-27 02:35:39.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/tools/infer/predict_det.py
--rw-rw-rw-   0        0        0     6501 2022-04-27 02:44:01.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/tools/infer/predict_e2e.py
--rw-rw-rw-   0        0        0    17592 2022-04-14 06:12:47.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/tools/infer/predict_rec.py
--rw-rw-rw-   0        0        0     7531 2022-04-14 06:12:33.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/tools/infer/predict_system.py
--rw-rw-rw-   0        0        0    25355 2022-04-14 10:43:39.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/tools/infer/utility.py
--rw-rw-rw-   0        0        0     2747 2022-04-27 02:43:41.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/tools/infer_cls.py
--rw-rw-rw-   0        0        0     5009 2022-04-14 09:58:45.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/tools/infer_det.py
--rw-rw-rw-   0        0        0     4472 2022-04-27 02:43:44.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/tools/infer_e2e.py
--rw-rw-rw-   0        0        0     5558 2022-04-27 02:43:47.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/tools/infer_kie.py
--rw-rw-rw-   0        0        0     5865 2022-04-27 02:43:50.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/tools/infer_rec.py
--rw-rw-rw-   0        0        0     3842 2022-04-27 02:43:54.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/tools/infer_table.py
--rw-rw-rw-   0        0        0    24550 2022-07-16 08:06:04.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/tools/program.py
--rw-rw-rw-   0        0        0     4200 2022-04-27 02:47:07.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/tools/test_hubserving.py
--rw-rw-rw-   0        0        0     6109 2022-04-14 09:59:15.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/tools/train.py
--rw-rw-rw-   0        0        0    33700 2022-09-02 09:04:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/tools/xlprog.py
-drwxrwxrwx   0        0        0        0 2022-10-13 10:38:46.976110 pyxllib-0.3.8.1/pyxlpr/ppocr/utils/
--rw-rw-rw-   0        0        0      280 2022-01-14 02:17:07.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/utils/EN_symbol_dict.txt
--rw-rw-rw-   0        0        0      881 2022-04-29 07:46:48.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-13 10:38:47.165604 pyxllib-0.3.8.1/pyxlpr/ppocr/utils/dict/
--rw-rw-rw-   0        0        0      390 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/utils/dict/ar_dict.txt
--rw-rw-rw-   0        0        0      569 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/utils/dict/arabic_dict.txt
--rw-rw-rw-   0        0        0      502 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/utils/dict/be_dict.txt
--rw-rw-rw-   0        0        0      481 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/utils/dict/bg_dict.txt
--rw-rw-rw-   0        0        0    41864 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/utils/dict/chinese_cht_dict.txt
--rw-rw-rw-   0        0        0      573 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/utils/dict/cyrillic_dict.txt
--rw-rw-rw-   0        0        0      675 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/utils/dict/devanagari_dict.txt
--rw-rw-rw-   0        0        0      189 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/utils/dict/en_dict.txt
--rw-rw-rw-   0        0        0      466 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/utils/dict/fa_dict.txt
--rw-rw-rw-   0        0        0      460 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/utils/dict/french_dict.txt
--rw-rw-rw-   0        0        0      489 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/utils/dict/german_dict.txt
--rw-rw-rw-   0        0        0      650 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/utils/dict/hi_dict.txt
--rw-rw-rw-   0        0        0      384 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/utils/dict/it_dict.txt
--rw-rw-rw-   0        0        0    21731 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/utils/dict/japan_dict.txt
--rw-rw-rw-   0        0        0      606 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/utils/dict/ka_dict.txt
--rw-rw-rw-   0        0        0    18168 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/utils/dict/korean_dict.txt
--rw-rw-rw-   0        0        0      653 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/utils/dict/latin_dict.txt
--rw-rw-rw-   0        0        0      605 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/utils/dict/mr_dict.txt
--rw-rw-rw-   0        0        0      605 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/utils/dict/ne_dict.txt
--rw-rw-rw-   0        0        0      306 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/utils/dict/oc_dict.txt
--rw-rw-rw-   0        0        0      435 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/utils/dict/pu_dict.txt
--rw-rw-rw-   0        0        0      285 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/utils/dict/rs_dict.txt
--rw-rw-rw-   0        0        0      458 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/utils/dict/rsc_dict.txt
--rw-rw-rw-   0        0        0      438 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/utils/dict/ru_dict.txt
--rw-rw-rw-   0        0        0      481 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/utils/dict/ta_dict.txt
--rw-rw-rw-   0        0        0     1171 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/utils/dict/table_dict.txt
--rw-rw-rw-   0        0        0    21350 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/utils/dict/table_structure_dict.txt
--rw-rw-rw-   0        0        0      580 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/utils/dict/te_dict.txt
--rw-rw-rw-   0        0        0      377 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/utils/dict/ug_dict.txt
--rw-rw-rw-   0        0        0      490 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/utils/dict/uk_dict.txt
--rw-rw-rw-   0        0        0      469 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/utils/dict/ur_dict.txt
--rw-rw-rw-   0        0        0      360 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/utils/dict/xi_dict.txt
--rw-rw-rw-   0        0        0      268 2022-01-14 02:17:07.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/utils/dict90.txt
-drwxrwxrwx   0        0        0        0 2022-10-13 10:38:47.193529 pyxllib-0.3.8.1/pyxlpr/ppocr/utils/e2e_metric/
--rw-rw-rw-   0        0        0    26617 2022-04-14 10:43:48.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/utils/e2e_metric/Deteval.py
--rw-rw-rw-   0        0        0     2925 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/utils/e2e_metric/polygon_fast.py
-drwxrwxrwx   0        0        0        0 2022-10-13 10:38:47.226441 pyxllib-0.3.8.1/pyxlpr/ppocr/utils/e2e_utils/
--rw-rw-rw-   0        0        0     3373 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/utils/e2e_utils/extract_batchsize.py
--rw-rw-rw-   0        0        0    17760 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/utils/e2e_utils/extract_textpoint_fast.py
--rw-rw-rw-   0        0        0    22815 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/utils/e2e_utils/extract_textpoint_slow.py
--rw-rw-rw-   0        0        0     6513 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/utils/e2e_utils/pgnet_pp_utils.py
--rw-rw-rw-   0        0        0     5420 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/utils/e2e_utils/visual.py
--rw-rw-rw-   0        0        0      285 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/utils/en_dict.txt
--rw-rw-rw-   0        0        0     3054 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/utils/gen_label.py
--rw-rw-rw-   0        0        0      106 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/utils/ic15_dict.txt
--rw-rw-rw-   0        0        0     1754 2022-01-14 02:17:07.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/utils/iou.py
--rw-rw-rw-   0        0        0     2724 2022-01-13 02:16:10.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/utils/logging.py
--rw-rw-rw-   0        0        0     3253 2022-04-14 10:43:43.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/utils/network.py
--rw-rw-rw-   0        0        0    32871 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/utils/ppocr_keys_v1.txt
--rw-rw-rw-   0        0        0     4503 2022-01-14 02:17:07.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/utils/profiler.py
--rw-rw-rw-   0        0        0     5637 2022-04-14 02:31:32.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/utils/save_load.py
--rw-rw-rw-   0        0        0     2304 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/utils/stats.py
--rw-rw-rw-   0        0        0     3160 2022-01-14 06:09:57.000000 pyxllib-0.3.8.1/pyxlpr/ppocr/utils/utility.py
-drwxrwxrwx   0        0        0        0 2022-10-13 10:38:47.242398 pyxllib-0.3.8.1/pyxlpr/ppstructure/
--rw-rw-rw-   0        0        0      621 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppstructure/__init__.py
--rw-rw-rw-   0        0        0     7797 2022-04-27 02:47:14.000000 pyxllib-0.3.8.1/pyxlpr/ppstructure/predict_system.py
-drwxrwxrwx   0        0        0        0 2022-10-13 10:38:47.266336 pyxllib-0.3.8.1/pyxlpr/ppstructure/table/
--rw-rw-rw-   0        0        0      621 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppstructure/table/__init__.py
--rw-rw-rw-   0        0        0     2377 2022-04-14 10:44:53.000000 pyxllib-0.3.8.1/pyxlpr/ppstructure/table/eval_table.py
--rw-rw-rw-   0        0        0     7168 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppstructure/table/matcher.py
--rw-rw-rw-   0        0        0     4663 2022-04-27 02:44:04.000000 pyxllib-0.3.8.1/pyxlpr/ppstructure/table/predict_structure.py
--rw-rw-rw-   0        0        0     8851 2022-04-27 02:44:08.000000 pyxllib-0.3.8.1/pyxlpr/ppstructure/table/predict_table.py
-drwxrwxrwx   0        0        0        0 2022-10-13 10:38:47.282292 pyxllib-0.3.8.1/pyxlpr/ppstructure/table/table_metric/
--rw-rw-rw-   0        0        0      673 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppstructure/table/table_metric/__init__.py
--rw-rw-rw-   0        0        0     2198 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppstructure/table/table_metric/parallel.py
--rw-rw-rw-   0        0        0     9532 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppstructure/table/table_metric/table_metric.py
-drwxrwxrwx   0        0        0        0 2022-10-13 10:38:47.299248 pyxllib-0.3.8.1/pyxlpr/ppstructure/table/tablepyxl/
--rw-rw-rw-   0        0        0      619 2021-12-14 06:42:13.000000 pyxllib-0.3.8.1/pyxlpr/ppstructure/table/tablepyxl/__init__.py
--rw-rw-rw-   0        0        0    10415 2022-04-22 12:24:19.000000 pyxllib-0.3.8.1/pyxlpr/ppstructure/table/tablepyxl/style.py
--rw-rw-rw-   0        0        0     4217 2022-04-22 12:24:30.000000 pyxllib-0.3.8.1/pyxlpr/ppstructure/table/tablepyxl/tablepyxl.py
--rw-rw-rw-   0        0        0     2538 2022-04-14 06:13:21.000000 pyxllib-0.3.8.1/pyxlpr/ppstructure/utility.py
--rw-rw-rw-   0        0        0      260 2022-08-10 07:36:15.000000 pyxllib-0.3.8.1/pyxlpr/xlai.py
--rw-rw-rw-   0        0        0      212 2022-07-12 12:58:43.000000 pyxllib-0.3.8.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2022-10-13 10:38:47.318197 pyxllib-0.3.8.1/setup.cfg
--rw-rw-rw-   0        0        0     2416 2022-10-13 10:38:43.000000 pyxllib-0.3.8.1/setup.py
-drwxrwxrwx   0        0        0        0 2022-10-13 10:38:47.316202 pyxllib-0.3.8.1/xlproject/
--rw-rw-rw-   0        0        0        0 2022-04-14 01:52:34.000000 pyxllib-0.3.8.1/xlproject/__init__.py
--rw-rw-rw-   0        0        0    46439 2022-10-05 01:24:13.000000 pyxllib-0.3.8.1/xlproject/kq5034lib.py
--rw-rw-rw-   0        0        0    27561 2022-09-13 07:50:23.000000 pyxllib-0.3.8.1/xlproject/核酸统计工具_在线版.py
+drwxrwxrwx   0        0        0        0 2022-10-18 02:03:36.257886 pyxllib-0.3.9/
+-rw-rw-rw-   0        0        0    10443 2020-05-30 01:21:59.000000 pyxllib-0.3.9/LICENSE
+-rw-rw-rw-   0        0        0       80 2022-04-14 09:35:06.000000 pyxllib-0.3.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     1089 2022-10-18 02:03:36.256889 pyxllib-0.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0      441 2022-02-25 06:57:44.000000 pyxllib-0.3.9/README.md
+drwxrwxrwx   0        0        0        0 2022-10-18 02:03:35.532177 pyxllib-0.3.9/pyxllib/
+-rw-rw-rw-   0        0        0      529 2022-06-24 02:18:32.000000 pyxllib-0.3.9/pyxllib/__init__.py
+drwxrwxrwx   0        0        0        0 2022-10-18 02:03:35.577057 pyxllib-0.3.9/pyxllib/algo/
+-rw-rw-rw-   0        0        0      161 2021-06-03 14:47:35.000000 pyxllib-0.3.9/pyxllib/algo/__init__.py
+-rw-rw-rw-   0        0        0     1282 2021-10-09 09:44:24.000000 pyxllib-0.3.9/pyxllib/algo/disjoint.py
+-rw-rw-rw-   0        0        0    18190 2022-09-12 12:59:06.000000 pyxllib-0.3.9/pyxllib/algo/geo.py
+-rw-rw-rw-   0        0        0    36718 2022-10-06 01:42:08.000000 pyxllib-0.3.9/pyxllib/algo/intervals.py
+-rw-rw-rw-   0        0        0     4168 2022-02-26 07:37:55.000000 pyxllib-0.3.9/pyxllib/algo/newbie.py
+-rw-rw-rw-   0        0        0    15611 2022-08-13 13:39:38.000000 pyxllib-0.3.9/pyxllib/algo/pupil.py
+-rw-rw-rw-   0        0        0     2393 2021-06-23 06:19:33.000000 pyxllib-0.3.9/pyxllib/algo/shapelylib.py
+-rw-rw-rw-   0        0        0     8584 2021-08-03 09:17:26.000000 pyxllib-0.3.9/pyxllib/algo/specialist.py
+-rw-rw-rw-   0        0        0    12884 2022-09-13 08:15:15.000000 pyxllib-0.3.9/pyxllib/algo/stat.py
+-rw-rw-rw-   0        0        0     5094 2022-07-04 01:30:35.000000 pyxllib-0.3.9/pyxllib/algo/treelib.py
+-rw-rw-rw-   0        0        0     1953 2022-03-16 03:08:01.000000 pyxllib-0.3.9/pyxllib/algo/unitlib.py
+drwxrwxrwx   0        0        0        0 2022-10-18 02:03:35.593014 pyxllib-0.3.9/pyxllib/cv/
+-rw-rw-rw-   0        0        0      132 2021-06-03 15:42:25.000000 pyxllib-0.3.9/pyxllib/cv/__init__.py
+-rw-rw-rw-   0        0        0     5054 2022-09-13 08:21:17.000000 pyxllib-0.3.9/pyxllib/cv/expert.py
+-rw-rw-rw-   0        0        0     6757 2021-06-25 09:32:56.000000 pyxllib-0.3.9/pyxllib/cv/imfile.py
+-rw-rw-rw-   0        0        0      907 2022-09-01 08:06:20.000000 pyxllib-0.3.9/pyxllib/cv/imhash.py
+-rw-rw-rw-   0        0        0      339 2022-05-05 11:22:25.000000 pyxllib-0.3.9/pyxllib/cv/pupil.py
+-rw-rw-rw-   0        0        0    38224 2022-06-12 09:01:30.000000 pyxllib-0.3.9/pyxllib/cv/rgbfmt.py
+-rw-rw-rw-   0        0        0     9259 2022-09-13 06:56:02.000000 pyxllib-0.3.9/pyxllib/cv/trackbartools.py
+-rw-rw-rw-   0        0        0    38288 2022-09-27 02:50:20.000000 pyxllib-0.3.9/pyxllib/cv/xlcvlib.py
+-rw-rw-rw-   0        0        0    14998 2022-10-09 07:09:36.000000 pyxllib-0.3.9/pyxllib/cv/xlpillib.py
+drwxrwxrwx   0        0        0        0 2022-10-18 02:03:35.602988 pyxllib-0.3.9/pyxllib/data/
+-rw-rw-rw-   0        0        0        0 2021-06-10 06:26:12.000000 pyxllib-0.3.9/pyxllib/data/__init__.py
+-rw-rw-rw-   0        0        0     3659 2022-09-13 06:56:02.000000 pyxllib-0.3.9/pyxllib/data/echarts.py
+-rw-rw-rw-   0        0        0     2477 2021-10-09 09:43:21.000000 pyxllib-0.3.9/pyxllib/data/oss.py
+-rw-rw-rw-   0        0        0    28262 2022-10-17 12:13:14.000000 pyxllib-0.3.9/pyxllib/data/pglib.py
+-rw-rw-rw-   0        0        0     7791 2022-10-14 02:35:47.000000 pyxllib-0.3.9/pyxllib/data/sqlite.py
+-rw-rw-rw-   0        0        0    11955 2021-10-09 09:40:53.000000 pyxllib-0.3.9/pyxllib/data/sqllib.py
+drwxrwxrwx   0        0        0        0 2022-10-18 02:03:35.618945 pyxllib-0.3.9/pyxllib/extend/
+-rw-rw-rw-   0        0        0      134 2022-09-13 07:42:34.000000 pyxllib-0.3.9/pyxllib/extend/__init__.py
+drwxrwxrwx   0        0        0        0 2022-10-18 02:03:35.624929 pyxllib-0.3.9/pyxllib/extend/autogui/
+-rw-rw-rw-   0        0        0      229 2022-09-13 08:23:33.000000 pyxllib-0.3.9/pyxllib/extend/autogui/__init__.py
+-rw-rw-rw-   0        0        0    25358 2022-09-27 06:29:43.000000 pyxllib-0.3.9/pyxllib/extend/autogui/autogui.py
+-rw-rw-rw-   0        0        0     3654 2021-08-03 11:27:22.000000 pyxllib-0.3.9/pyxllib/extend/autogui/virtualkey.py
+-rw-rw-rw-   0        0        0     8552 2022-06-30 06:11:06.000000 pyxllib-0.3.9/pyxllib/extend/demolib.py
+-rw-rw-rw-   0        0        0    27407 2022-09-13 08:24:35.000000 pyxllib-0.3.9/pyxllib/extend/old.py
+-rw-rw-rw-   0        0        0     9966 2022-07-12 08:13:02.000000 pyxllib-0.3.9/pyxllib/extend/qt.py
+-rw-rw-rw-   0        0        0     5004 2021-06-06 12:23:02.000000 pyxllib-0.3.9/pyxllib/extend/tk.py
+-rw-rw-rw-   0        0        0    33702 2022-10-17 12:41:00.000000 pyxllib-0.3.9/pyxllib/extend/unixlib.py
+-rw-rw-rw-   0        0        0    13016 2022-09-13 08:26:05.000000 pyxllib-0.3.9/pyxllib/extend/utools.py
+-rw-rw-rw-   0        0        0     2922 2021-06-06 12:45:02.000000 pyxllib-0.3.9/pyxllib/extend/webhook.py
+-rw-rw-rw-   0        0        0     1237 2021-12-19 10:33:17.000000 pyxllib-0.3.9/pyxllib/extend/win32lib.py
+drwxrwxrwx   0        0        0        0 2022-10-18 02:03:35.643879 pyxllib-0.3.9/pyxllib/file/
+-rw-rw-rw-   0        0        0      452 2021-06-03 15:43:58.000000 pyxllib-0.3.9/pyxllib/file/__init__.py
+-rw-rw-rw-   0        0        0    29443 2022-09-23 06:45:05.000000 pyxllib-0.3.9/pyxllib/file/docxlib.py
+-rw-rw-rw-   0        0        0    11620 2022-09-13 08:19:54.000000 pyxllib-0.3.9/pyxllib/file/gitlib.py
+-rw-rw-rw-   0        0        0     5880 2022-07-05 06:50:20.000000 pyxllib-0.3.9/pyxllib/file/movielib.py
+-rw-rw-rw-   0        0        0      218 2021-06-06 09:44:33.000000 pyxllib-0.3.9/pyxllib/file/newbie.py
+-rw-rw-rw-   0        0        0    54951 2022-09-14 02:44:42.000000 pyxllib-0.3.9/pyxllib/file/onenotelib.py
+drwxrwxrwx   0        0        0        0 2022-10-18 02:03:35.647868 pyxllib-0.3.9/pyxllib/file/packlib/
+-rw-rw-rw-   0        0        0     7085 2022-07-05 07:09:24.000000 pyxllib-0.3.9/pyxllib/file/packlib/__init__.py
+-rw-rw-rw-   0        0        0    90165 2022-02-15 02:13:17.000000 pyxllib-0.3.9/pyxllib/file/packlib/zipfile.py
+-rw-rw-rw-   0        0        0    16927 2022-09-13 08:20:38.000000 pyxllib-0.3.9/pyxllib/file/pdflib.py
+-rw-rw-rw-   0        0        0     5997 2021-10-17 07:30:24.000000 pyxllib-0.3.9/pyxllib/file/pupil.py
+drwxrwxrwx   0        0        0        0 2022-10-18 02:03:35.655846 pyxllib-0.3.9/pyxllib/file/specialist/
+-rw-rw-rw-   0        0        0      277 2021-06-30 06:21:43.000000 pyxllib-0.3.9/pyxllib/file/specialist/__init__.py
+-rw-rw-rw-   0        0        0    32216 2022-09-13 08:19:04.000000 pyxllib-0.3.9/pyxllib/file/specialist/dirlib.py
+-rw-rw-rw-   0        0        0     6534 2022-09-09 07:59:04.000000 pyxllib-0.3.9/pyxllib/file/specialist/download.py
+-rw-rw-rw-   0        0        0    65428 2022-09-13 08:19:21.000000 pyxllib-0.3.9/pyxllib/file/specialist/filelib.py
+-rw-rw-rw-   0        0        0    36528 2022-09-13 08:20:58.000000 pyxllib-0.3.9/pyxllib/file/xlsxlib.py
+drwxrwxrwx   0        0        0        0 2022-10-18 02:03:35.665820 pyxllib-0.3.9/pyxllib/prog/
+-rw-rw-rw-   0        0        0      132 2021-06-03 15:22:15.000000 pyxllib-0.3.9/pyxllib/prog/__init__.py
+-rw-rw-rw-   0        0        0     8499 2021-06-05 17:05:47.000000 pyxllib-0.3.9/pyxllib/prog/deprecatedlib.py
+-rw-rw-rw-   0        0        0    11982 2022-09-13 06:49:51.000000 pyxllib-0.3.9/pyxllib/prog/newbie.py
+-rw-rw-rw-   0        0        0    33283 2022-09-27 06:09:15.000000 pyxllib-0.3.9/pyxllib/prog/pupil.py
+-rw-rw-rw-   0        0        0      996 2021-06-06 08:23:35.000000 pyxllib-0.3.9/pyxllib/prog/sitepackages.py
+drwxrwxrwx   0        0        0        0 2022-10-18 02:03:35.679782 pyxllib-0.3.9/pyxllib/prog/specialist/
+-rw-rw-rw-   0        0        0     8230 2022-09-13 06:56:02.000000 pyxllib-0.3.9/pyxllib/prog/specialist/__init__.py
+-rw-rw-rw-   0        0        0     9644 2022-09-29 06:23:13.000000 pyxllib-0.3.9/pyxllib/prog/specialist/bc.py
+-rw-rw-rw-   0        0        0    19775 2022-09-13 08:33:02.000000 pyxllib-0.3.9/pyxllib/prog/specialist/browser.py
+-rw-rw-rw-   0        0        0    13309 2022-04-09 12:50:47.000000 pyxllib-0.3.9/pyxllib/prog/specialist/common.py
+-rw-rw-rw-   0        0        0     4527 2022-03-16 02:37:13.000000 pyxllib-0.3.9/pyxllib/prog/specialist/datetime.py
+-rw-rw-rw-   0        0        0     8206 2022-09-13 08:14:07.000000 pyxllib-0.3.9/pyxllib/prog/specialist/tictoc.py
+-rw-rw-rw-   0        0        0     8289 2022-09-13 08:14:20.000000 pyxllib-0.3.9/pyxllib/prog/specialist/xllog.py
+drwxrwxrwx   0        0        0        0 2022-10-18 02:03:35.680780 pyxllib-0.3.9/pyxllib/stdlib/
+-rw-rw-rw-   0        0        0      581 2022-02-15 02:25:06.000000 pyxllib-0.3.9/pyxllib/stdlib/__init__.py
+drwxrwxrwx   0        0        0        0 2022-10-18 02:03:35.686764 pyxllib-0.3.9/pyxllib/stdlib/tablepyxl/
+-rw-rw-rw-   0        0        0      193 2021-06-03 09:24:15.000000 pyxllib-0.3.9/pyxllib/stdlib/tablepyxl/__init__.py
+-rw-rw-rw-   0        0        0    10924 2022-04-22 12:23:11.000000 pyxllib-0.3.9/pyxllib/stdlib/tablepyxl/style.py
+-rw-rw-rw-   0        0        0     4531 2022-04-22 12:23:21.000000 pyxllib-0.3.9/pyxllib/stdlib/tablepyxl/tablepyxl.py
+drwxrwxrwx   0        0        0        0 2022-10-18 02:03:35.704716 pyxllib-0.3.9/pyxllib/text/
+-rw-rw-rw-   0        0        0      170 2021-06-03 14:58:07.000000 pyxllib-0.3.9/pyxllib/text/__init__.py
+-rw-rw-rw-   0        0        0     1259 2021-10-09 09:37:54.000000 pyxllib-0.3.9/pyxllib/text/ahocorasick.py
+drwxrwxrwx   0        0        0        0 2022-10-18 02:03:35.706710 pyxllib-0.3.9/pyxllib/text/latex/
+-rw-rw-rw-   0        0        0     6416 2022-09-13 08:15:50.000000 pyxllib-0.3.9/pyxllib/text/latex/__init__.py
+-rw-rw-rw-   0        0        0     4310 2022-09-13 08:17:11.000000 pyxllib-0.3.9/pyxllib/text/levenshtein.py
+-rw-rw-rw-   0        0        0    49235 2022-10-13 08:50:28.000000 pyxllib-0.3.9/pyxllib/text/nestenv.py
+-rw-rw-rw-   0        0        0     7941 2022-05-19 02:34:37.000000 pyxllib-0.3.9/pyxllib/text/newbie.py
+drwxrwxrwx   0        0        0        0 2022-10-18 02:03:35.712695 pyxllib-0.3.9/pyxllib/text/pupil/
+-rw-rw-rw-   0        0        0      217 2021-06-06 09:36:42.000000 pyxllib-0.3.9/pyxllib/text/pupil/__init__.py
+-rw-rw-rw-   0        0        0    31077 2022-09-13 08:16:22.000000 pyxllib-0.3.9/pyxllib/text/pupil/common.py
+-rw-rw-rw-   0        0        0    10985 2021-07-17 02:50:04.000000 pyxllib-0.3.9/pyxllib/text/pupil/xlalign.py
+-rw-rw-rw-   0        0        0     1585 2022-09-13 08:06:32.000000 pyxllib-0.3.9/pyxllib/text/pycode.py
+drwxrwxrwx   0        0        0        0 2022-10-18 02:03:35.718679 pyxllib-0.3.9/pyxllib/text/specialist/
+-rw-rw-rw-   0        0        0      224 2021-09-23 01:54:34.000000 pyxllib-0.3.9/pyxllib/text/specialist/__init__.py
+-rw-rw-rw-   0        0        0     3935 2022-09-13 08:16:41.000000 pyxllib-0.3.9/pyxllib/text/specialist/common.py
+-rw-rw-rw-   0        0        0     6686 2022-09-13 08:16:52.000000 pyxllib-0.3.9/pyxllib/text/specialist/ptag.py
+-rw-rw-rw-   0        0        0     7706 2022-09-13 08:17:44.000000 pyxllib-0.3.9/pyxllib/text/spellchecker.py
+-rw-rw-rw-   0        0        0    26666 2022-09-29 09:25:22.000000 pyxllib-0.3.9/pyxllib/text/xmllib.py
+-rw-rw-rw-   0        0        0      698 2022-09-13 08:11:02.000000 pyxllib-0.3.9/pyxllib/xl.py
+-rw-rw-rw-   0        0        0      652 2022-07-05 09:15:11.000000 pyxllib-0.3.9/pyxllib/xlcv.py
+drwxrwxrwx   0        0        0        0 2022-10-18 02:03:35.557111 pyxllib-0.3.9/pyxllib.egg-info/
+-rw-rw-rw-   0        0        0     1089 2022-10-18 02:03:34.000000 pyxllib-0.3.9/pyxllib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    11453 2022-10-18 02:03:35.000000 pyxllib-0.3.9/pyxllib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-10-18 02:03:34.000000 pyxllib-0.3.9/pyxllib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      323 2022-10-18 02:03:34.000000 pyxllib-0.3.9/pyxllib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2022-10-18 02:03:34.000000 pyxllib-0.3.9/pyxllib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-10-18 02:03:35.724662 pyxllib-0.3.9/pyxlpr/
+-rw-rw-rw-   0        0        0      126 2022-04-14 01:52:38.000000 pyxllib-0.3.9/pyxlpr/__init__.py
+drwxrwxrwx   0        0        0        0 2022-10-18 02:03:35.737628 pyxllib-0.3.9/pyxlpr/ai/
+-rw-rw-rw-   0        0        0      132 2021-06-03 14:16:46.000000 pyxllib-0.3.9/pyxlpr/ai/__init__.py
+-rw-rw-rw-   0        0        0    49872 2022-09-28 08:53:04.000000 pyxllib-0.3.9/pyxlpr/ai/clientlib.py
+-rw-rw-rw-   0        0        0     9682 2022-06-30 06:26:38.000000 pyxllib-0.3.9/pyxlpr/ai/specialist.py
+-rw-rw-rw-   0        0        0     6591 2022-09-14 02:36:54.000000 pyxllib-0.3.9/pyxlpr/ai/torch_app.py
+-rw-rw-rw-   0        0        0    24956 2022-08-16 07:21:21.000000 pyxllib-0.3.9/pyxlpr/ai/xlpaddle.py
+-rw-rw-rw-   0        0        0    29450 2022-07-19 09:30:02.000000 pyxllib-0.3.9/pyxlpr/ai/xltorch.py
+drwxrwxrwx   0        0        0        0 2022-10-18 02:03:35.753585 pyxllib-0.3.9/pyxlpr/data/
+-rw-rw-rw-   0        0        0      281 2021-07-29 01:04:03.000000 pyxllib-0.3.9/pyxlpr/data/__init__.py
+-rw-rw-rw-   0        0        0    57147 2022-09-19 08:15:27.000000 pyxllib-0.3.9/pyxlpr/data/coco.py
+-rw-rw-rw-   0        0        0    14619 2022-04-14 02:38:30.000000 pyxllib-0.3.9/pyxlpr/data/datacls.py
+-rw-rw-rw-   0        0        0     8252 2021-10-21 08:58:12.000000 pyxllib-0.3.9/pyxlpr/data/datasets.py
+drwxrwxrwx   0        0        0        0 2022-10-18 02:03:35.765553 pyxllib-0.3.9/pyxlpr/data/icdar/
+-rw-rw-rw-   0        0        0     4603 2022-08-30 02:50:10.000000 pyxllib-0.3.9/pyxlpr/data/icdar/__init__.py
+-rw-rw-rw-   0        0        0    18077 2022-08-30 02:33:05.000000 pyxllib-0.3.9/pyxlpr/data/icdar/deteval.py
+-rw-rw-rw-   0        0        0    16306 2022-08-30 02:31:32.000000 pyxllib-0.3.9/pyxlpr/data/icdar/icdar2013.py
+-rw-rw-rw-   0        0        0    13859 2022-08-30 08:50:22.000000 pyxllib-0.3.9/pyxlpr/data/icdar/iou.py
+-rw-rw-rw-   0        0        0    19740 2021-03-11 12:41:54.000000 pyxllib-0.3.9/pyxlpr/data/icdar/rrc_evaluation_funcs_1_1.py
+-rw-rw-rw-   0        0        0    19054 2022-09-14 02:43:04.000000 pyxllib-0.3.9/pyxlpr/data/imtextline.py
+-rw-rw-rw-   0        0        0    33925 2022-09-13 06:56:02.000000 pyxllib-0.3.9/pyxlpr/data/labelme.py
+-rw-rw-rw-   0        0        0     6499 2021-09-08 06:16:36.000000 pyxllib-0.3.9/pyxlpr/data/removeline.py
+-rw-rw-rw-   0        0        0     2066 2021-06-25 09:03:58.000000 pyxllib-0.3.9/pyxlpr/data/specialist.py
+drwxrwxrwx   0        0        0        0 2022-10-18 02:03:35.767552 pyxllib-0.3.9/pyxlpr/eval/
+-rw-rw-rw-   0        0        0     2980 2022-04-24 02:55:19.000000 pyxllib-0.3.9/pyxlpr/eval/__init__.py
+-rw-rw-rw-   0        0        0    32303 2022-09-13 06:56:02.000000 pyxllib-0.3.9/pyxlpr/paddleocr.py
+drwxrwxrwx   0        0        0        0 2022-10-18 02:03:35.770540 pyxllib-0.3.9/pyxlpr/ppocr/
+-rw-rw-rw-   0        0        0      651 2022-04-14 01:50:28.000000 pyxllib-0.3.9/pyxlpr/ppocr/__init__.py
+drwxrwxrwx   0        0        0        0 2022-10-18 02:03:35.503254 pyxllib-0.3.9/pyxlpr/ppocr/configs/
+drwxrwxrwx   0        0        0        0 2022-10-18 02:03:35.503254 pyxllib-0.3.9/pyxlpr/ppocr/configs/rec/
+drwxrwxrwx   0        0        0        0 2022-10-18 02:03:35.772537 pyxllib-0.3.9/pyxlpr/ppocr/configs/rec/multi_language/
+-rw-rw-rw-   0        0        0     8633 2021-12-14 06:42:12.000000 pyxllib-0.3.9/pyxlpr/ppocr/configs/rec/multi_language/generate_multi_language_configs.py
+drwxrwxrwx   0        0        0        0 2022-10-18 02:03:35.784506 pyxllib-0.3.9/pyxlpr/ppocr/data/
+-rw-rw-rw-   0        0        0     5565 2022-04-14 09:57:11.000000 pyxllib-0.3.9/pyxlpr/ppocr/data/__init__.py
+drwxrwxrwx   0        0        0        0 2022-10-18 02:03:35.831378 pyxllib-0.3.9/pyxlpr/ppocr/data/imaug/
+-rw-rw-rw-   0        0        0     1053 2022-01-14 02:17:07.000000 pyxllib-0.3.9/pyxlpr/ppocr/data/imaug/ColorJitter.py
+-rw-rw-rw-   0        0        0     2395 2022-01-14 02:36:55.000000 pyxllib-0.3.9/pyxlpr/ppocr/data/imaug/__init__.py
+-rw-rw-rw-   0        0        0     6655 2022-04-14 09:57:17.000000 pyxllib-0.3.9/pyxlpr/ppocr/data/imaug/copy_paste.py
+-rw-rw-rw-   0        0        0    17757 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/data/imaug/east_process.py
+-rw-rw-rw-   0        0        0     9565 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/data/imaug/gen_table_mask.py
+-rw-rw-rw-   0        0        0     3791 2021-12-14 08:52:21.000000 pyxllib-0.3.9/pyxlpr/ppocr/data/imaug/iaa_augment.py
+-rw-rw-rw-   0        0        0    28912 2022-04-14 09:57:22.000000 pyxllib-0.3.9/pyxlpr/ppocr/data/imaug/label_ops.py
+-rw-rw-rw-   0        0        0     7144 2021-12-31 07:49:15.000000 pyxllib-0.3.9/pyxlpr/ppocr/data/imaug/make_border_map.py
+-rw-rw-rw-   0        0        0     4008 2022-01-14 02:17:07.000000 pyxllib-0.3.9/pyxlpr/ppocr/data/imaug/make_pse_gt.py
+-rw-rw-rw-   0        0        0     4898 2022-01-01 02:45:22.000000 pyxllib-0.3.9/pyxlpr/ppocr/data/imaug/make_shrink_map.py
+-rw-rw-rw-   0        0        0    15625 2022-04-10 05:57:02.000000 pyxllib-0.3.9/pyxlpr/ppocr/data/imaug/operators.py
+-rw-rw-rw-   0        0        0    36408 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/data/imaug/pg_process.py
+-rw-rw-rw-   0        0        0     5591 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/data/imaug/randaugment.py
+-rw-rw-rw-   0        0        0     8442 2022-01-14 02:43:40.000000 pyxllib-0.3.9/pyxlpr/ppocr/data/imaug/random_crop_data.py
+-rw-rw-rw-   0        0        0    17398 2022-01-14 02:44:43.000000 pyxllib-0.3.9/pyxlpr/ppocr/data/imaug/rec_img_aug.py
+-rw-rw-rw-   0        0        0    30175 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/data/imaug/sast_process.py
+drwxrwxrwx   0        0        0        0 2022-10-18 02:03:35.839355 pyxllib-0.3.9/pyxlpr/ppocr/data/imaug/text_image_aug/
+-rw-rw-rw-   0        0        0      750 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/data/imaug/text_image_aug/__init__.py
+-rw-rw-rw-   0        0        0     3557 2022-01-14 02:37:02.000000 pyxllib-0.3.9/pyxlpr/ppocr/data/imaug/text_image_aug/augment.py
+-rw-rw-rw-   0        0        0     6619 2022-01-14 02:37:07.000000 pyxllib-0.3.9/pyxlpr/ppocr/data/imaug/text_image_aug/warp_mls.py
+-rw-rw-rw-   0        0        0     4485 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/data/lmdb_dataset.py
+-rw-rw-rw-   0        0        0     4235 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/data/pgnet_dataset.py
+-rw-rw-rw-   0        0        0     4410 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/data/pubtab_dataset.py
+-rw-rw-rw-   0        0        0    15429 2022-07-17 08:19:44.000000 pyxllib-0.3.9/pyxlpr/ppocr/data/simple_dataset.py
+drwxrwxrwx   0        0        0        0 2022-10-18 02:03:35.878482 pyxllib-0.3.9/pyxlpr/ppocr/losses/
+-rw-rw-rw-   0        0        0     1925 2022-01-14 02:46:47.000000 pyxllib-0.3.9/pyxlpr/ppocr/losses/__init__.py
+-rw-rw-rw-   0        0        0     1811 2022-01-14 02:17:07.000000 pyxllib-0.3.9/pyxlpr/ppocr/losses/ace_loss.py
+-rw-rw-rw-   0        0        0     4431 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/losses/basic_loss.py
+-rw-rw-rw-   0        0        0     3581 2022-01-14 02:17:07.000000 pyxllib-0.3.9/pyxlpr/ppocr/losses/center_loss.py
+-rw-rw-rw-   0        0        0     1106 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/losses/cls_loss.py
+-rw-rw-rw-   0        0        0     2497 2022-01-14 02:47:04.000000 pyxllib-0.3.9/pyxlpr/ppocr/losses/combined_loss.py
+-rw-rw-rw-   0        0        0     7682 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/losses/det_basic_loss.py
+-rw-rw-rw-   0        0        0     3245 2022-01-01 03:12:22.000000 pyxllib-0.3.9/pyxlpr/ppocr/losses/det_db_loss.py
+-rw-rw-rw-   0        0        0     2338 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/losses/det_east_loss.py
+-rw-rw-rw-   0        0        0     5872 2022-04-14 09:57:27.000000 pyxllib-0.3.9/pyxlpr/ppocr/losses/det_pse_loss.py
+-rw-rw-rw-   0        0        0     5197 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/losses/det_sast_loss.py
+-rw-rw-rw-   0        0        0     9741 2022-01-14 02:48:26.000000 pyxllib-0.3.9/pyxlpr/ppocr/losses/distillation_loss.py
+-rw-rw-rw-   0        0        0     6716 2022-04-14 09:57:33.000000 pyxllib-0.3.9/pyxlpr/ppocr/losses/e2e_pg_loss.py
+-rw-rw-rw-   0        0        0     4779 2022-01-14 02:17:07.000000 pyxllib-0.3.9/pyxlpr/ppocr/losses/kie_sdmgr_loss.py
+-rw-rw-rw-   0        0        0     3860 2022-01-14 02:17:07.000000 pyxllib-0.3.9/pyxlpr/ppocr/losses/rec_aster_loss.py
+-rw-rw-rw-   0        0        0     1568 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/losses/rec_att_loss.py
+-rw-rw-rw-   0        0        0     1761 2022-01-14 02:48:09.000000 pyxllib-0.3.9/pyxlpr/ppocr/losses/rec_ctc_loss.py
+-rw-rw-rw-   0        0        0     2570 2022-01-14 02:17:07.000000 pyxllib-0.3.9/pyxlpr/ppocr/losses/rec_enhanced_ctc_loss.py
+-rw-rw-rw-   0        0        0     1120 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/losses/rec_nrtr_loss.py
+-rw-rw-rw-   0        0        0     1110 2022-01-14 02:17:07.000000 pyxllib-0.3.9/pyxlpr/ppocr/losses/rec_sar_loss.py
+-rw-rw-rw-   0        0        0     1864 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/losses/rec_srn_loss.py
+-rw-rw-rw-   0        0        0     4735 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/losses/table_att_loss.py
+drwxrwxrwx   0        0        0        0 2022-10-18 02:03:35.896432 pyxllib-0.3.9/pyxlpr/ppocr/metrics/
+-rw-rw-rw-   0        0        0     1526 2022-01-14 02:48:48.000000 pyxllib-0.3.9/pyxlpr/ppocr/metrics/__init__.py
+-rw-rw-rw-   0        0        0     1497 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/metrics/cls_metric.py
+-rw-rw-rw-   0        0        0     3256 2021-12-17 11:27:16.000000 pyxllib-0.3.9/pyxlpr/ppocr/metrics/det_metric.py
+-rw-rw-rw-   0        0        0     2460 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/metrics/distillation_metric.py
+-rw-rw-rw-   0        0        0     3278 2022-04-14 09:57:38.000000 pyxllib-0.3.9/pyxlpr/ppocr/metrics/e2e_metric.py
+-rw-rw-rw-   0        0        0    10453 2022-01-12 09:51:33.000000 pyxllib-0.3.9/pyxlpr/ppocr/metrics/eval_det_iou.py
+-rw-rw-rw-   0        0        0     2445 2022-01-14 02:17:07.000000 pyxllib-0.3.9/pyxlpr/ppocr/metrics/kie_metric.py
+-rw-rw-rw-   0        0        0     2637 2022-01-20 09:03:43.000000 pyxllib-0.3.9/pyxlpr/ppocr/metrics/rec_metric.py
+-rw-rw-rw-   0        0        0     1784 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/metrics/table_metric.py
+drwxrwxrwx   0        0        0        0 2022-10-18 02:03:35.508241 pyxllib-0.3.9/pyxlpr/ppocr/modeling/
+drwxrwxrwx   0        0        0        0 2022-10-18 02:03:35.902416 pyxllib-0.3.9/pyxlpr/ppocr/modeling/architectures/
+-rw-rw-rw-   0        0        0     1058 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/modeling/architectures/__init__.py
+-rw-rw-rw-   0        0        0     3373 2022-04-14 09:57:43.000000 pyxllib-0.3.9/pyxlpr/ppocr/modeling/architectures/base_model.py
+-rw-rw-rw-   0        0        0     2406 2022-04-14 09:57:49.000000 pyxllib-0.3.9/pyxlpr/ppocr/modeling/architectures/distillation_model.py
+drwxrwxrwx   0        0        0        0 2022-10-18 02:03:35.932337 pyxllib-0.3.9/pyxlpr/ppocr/modeling/backbones/
+-rw-rw-rw-   0        0        0     2296 2022-01-14 02:51:49.000000 pyxllib-0.3.9/pyxlpr/ppocr/modeling/backbones/__init__.py
+-rw-rw-rw-   0        0        0     9218 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/modeling/backbones/det_mobilenet_v3.py
+-rw-rw-rw-   0        0        0     8164 2022-01-14 02:52:14.000000 pyxllib-0.3.9/pyxlpr/ppocr/modeling/backbones/det_resnet_vd.py
+-rw-rw-rw-   0        0        0     9816 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/modeling/backbones/det_resnet_vd_sast.py
+-rw-rw-rw-   0        0        0     9163 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/modeling/backbones/e2e_resnet_vd_pg.py
+-rw-rw-rw-   0        0        0     6270 2022-01-14 02:17:07.000000 pyxllib-0.3.9/pyxlpr/ppocr/modeling/backbones/kie_unet_sdmgr.py
+-rw-rw-rw-   0        0        0     5677 2022-04-14 09:57:53.000000 pyxllib-0.3.9/pyxlpr/ppocr/modeling/backbones/rec_mobilenet_v3.py
+-rw-rw-rw-   0        0        0     8192 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/modeling/backbones/rec_mv1_enhance.py
+-rw-rw-rw-   0        0        0     1883 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/modeling/backbones/rec_nrtr_mtb.py
+-rw-rw-rw-   0        0        0     7365 2022-01-14 02:17:07.000000 pyxllib-0.3.9/pyxlpr/ppocr/modeling/backbones/rec_resnet_31.py
+-rw-rw-rw-   0        0        0     4714 2022-01-14 02:17:07.000000 pyxllib-0.3.9/pyxlpr/ppocr/modeling/backbones/rec_resnet_aster.py
+-rw-rw-rw-   0        0        0    11084 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/modeling/backbones/rec_resnet_fpn.py
+-rw-rw-rw-   0        0        0     9715 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/modeling/backbones/rec_resnet_vd.py
+drwxrwxrwx   0        0        0        0 2022-10-18 02:03:35.970235 pyxllib-0.3.9/pyxlpr/ppocr/modeling/heads/
+-rw-rw-rw-   0        0        0     1799 2022-01-14 02:54:10.000000 pyxllib-0.3.9/pyxlpr/ppocr/modeling/heads/__init__.py
+-rw-rw-rw-   0        0        0     1694 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/modeling/heads/cls_head.py
+-rw-rw-rw-   0        0        0     4333 2021-12-30 06:31:07.000000 pyxllib-0.3.9/pyxlpr/ppocr/modeling/heads/det_db_head.py
+-rw-rw-rw-   0        0        0     3836 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/modeling/heads/det_east_head.py
+-rw-rw-rw-   0        0        0     1374 2022-01-14 02:17:07.000000 pyxllib-0.3.9/pyxlpr/ppocr/modeling/heads/det_pse_head.py
+-rw-rw-rw-   0        0        0     4880 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/modeling/heads/det_sast_head.py
+-rw-rw-rw-   0        0        0     8013 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/modeling/heads/e2e_pg_head.py
+-rw-rw-rw-   0        0        0     8314 2022-01-14 02:17:07.000000 pyxllib-0.3.9/pyxlpr/ppocr/modeling/heads/kie_sdmgr_head.py
+-rw-rw-rw-   0        0        0     6646 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/modeling/heads/multiheadAttention.py
+-rw-rw-rw-   0        0        0    16232 2022-01-14 02:17:07.000000 pyxllib-0.3.9/pyxlpr/ppocr/modeling/heads/rec_aster_head.py
+-rw-rw-rw-   0        0        0     8171 2022-01-14 02:53:49.000000 pyxllib-0.3.9/pyxlpr/ppocr/modeling/heads/rec_att_head.py
+-rw-rw-rw-   0        0        0     3014 2022-01-14 02:53:42.000000 pyxllib-0.3.9/pyxlpr/ppocr/modeling/heads/rec_ctc_head.py
+-rw-rw-rw-   0        0        0    33928 2022-04-14 09:58:00.000000 pyxllib-0.3.9/pyxlpr/ppocr/modeling/heads/rec_nrtr_head.py
+-rw-rw-rw-   0        0        0    14454 2022-01-14 02:17:07.000000 pyxllib-0.3.9/pyxlpr/ppocr/modeling/heads/rec_sar_head.py
+-rw-rw-rw-   0        0        0    11171 2022-04-14 09:58:04.000000 pyxllib-0.3.9/pyxlpr/ppocr/modeling/heads/rec_srn_head.py
+-rw-rw-rw-   0        0        0    15211 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/modeling/heads/self_attention.py
+-rw-rw-rw-   0        0        0    10680 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/modeling/heads/table_att_head.py
+drwxrwxrwx   0        0        0        0 2022-10-18 02:03:35.991179 pyxllib-0.3.9/pyxlpr/ppocr/modeling/necks/
+-rw-rw-rw-   0        0        0     1230 2022-01-14 02:53:27.000000 pyxllib-0.3.9/pyxlpr/ppocr/modeling/necks/__init__.py
+-rw-rw-rw-   0        0        0     4130 2021-12-30 06:26:52.000000 pyxllib-0.3.9/pyxlpr/ppocr/modeling/necks/db_fpn.py
+-rw-rw-rw-   0        0        0     6050 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/modeling/necks/east_fpn.py
+-rw-rw-rw-   0        0        0     5113 2022-01-14 02:17:07.000000 pyxllib-0.3.9/pyxlpr/ppocr/modeling/necks/fpn.py
+-rw-rw-rw-   0        0        0    10185 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/modeling/necks/pg_fpn.py
+-rw-rw-rw-   0        0        0     3149 2022-04-14 09:58:09.000000 pyxllib-0.3.9/pyxlpr/ppocr/modeling/necks/rnn.py
+-rw-rw-rw-   0        0        0    11150 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/modeling/necks/sast_fpn.py
+-rw-rw-rw-   0        0        0     4306 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/modeling/necks/table_fpn.py
+drwxrwxrwx   0        0        0        0 2022-10-18 02:03:35.998160 pyxllib-0.3.9/pyxlpr/ppocr/modeling/transforms/
+-rw-rw-rw-   0        0        0     1009 2022-01-14 02:53:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/modeling/transforms/__init__.py
+-rw-rw-rw-   0        0        0     5251 2022-01-14 02:17:07.000000 pyxllib-0.3.9/pyxlpr/ppocr/modeling/transforms/stn.py
+-rw-rw-rw-   0        0        0    11696 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/modeling/transforms/tps.py
+-rw-rw-rw-   0        0        0     6923 2022-01-14 02:17:07.000000 pyxllib-0.3.9/pyxlpr/ppocr/modeling/transforms/tps_spatial_transformer.py
+drwxrwxrwx   0        0        0        0 2022-10-18 02:03:36.010129 pyxllib-0.3.9/pyxlpr/ppocr/optimizer/
+-rw-rw-rw-   0        0        0     2280 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/optimizer/__init__.py
+-rw-rw-rw-   0        0        0     8587 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/optimizer/learning_rate.py
+-rw-rw-rw-   0        0        0     2036 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/optimizer/lr_scheduler.py
+-rw-rw-rw-   0        0        0     5476 2022-01-14 02:56:11.000000 pyxllib-0.3.9/pyxlpr/ppocr/optimizer/optimizer.py
+-rw-rw-rw-   0        0        0     1665 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/optimizer/regularizer.py
+drwxrwxrwx   0        0        0        0 2022-10-18 02:03:36.027083 pyxllib-0.3.9/pyxlpr/ppocr/postprocess/
+-rw-rw-rw-   0        0        0     2201 2022-01-14 02:57:04.000000 pyxllib-0.3.9/pyxlpr/ppocr/postprocess/__init__.py
+-rw-rw-rw-   0        0        0     1323 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/postprocess/cls_postprocess.py
+-rw-rw-rw-   0        0        0     8752 2022-01-01 03:08:09.000000 pyxllib-0.3.9/pyxlpr/ppocr/postprocess/db_postprocess.py
+-rw-rw-rw-   0        0        0     5238 2022-01-14 02:57:52.000000 pyxllib-0.3.9/pyxlpr/ppocr/postprocess/east_postprocess.py
+-rw-rw-rw-   0        0        0     5233 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/postprocess/locality_aware_nms.py
+-rw-rw-rw-   0        0        0     1872 2022-04-14 09:58:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/postprocess/pg_postprocess.py
+drwxrwxrwx   0        0        0        0 2022-10-18 02:03:36.030075 pyxllib-0.3.9/pyxlpr/ppocr/postprocess/pse_postprocess/
+-rw-rw-rw-   0        0        0      668 2022-01-14 02:17:07.000000 pyxllib-0.3.9/pyxlpr/ppocr/postprocess/pse_postprocess/__init__.py
+drwxrwxrwx   0        0        0        0 2022-10-18 02:03:36.037056 pyxllib-0.3.9/pyxlpr/ppocr/postprocess/pse_postprocess/pse/
+-rw-rw-rw-   0        0        0     1174 2022-01-14 02:17:07.000000 pyxllib-0.3.9/pyxlpr/ppocr/postprocess/pse_postprocess/pse/__init__.py
+-rw-rw-rw-   0        0        0      340 2022-01-14 02:17:07.000000 pyxllib-0.3.9/pyxlpr/ppocr/postprocess/pse_postprocess/pse/setup.py
+-rw-rw-rw-   0        0        0     4172 2022-04-14 09:58:17.000000 pyxllib-0.3.9/pyxlpr/ppocr/postprocess/pse_postprocess/pse_postprocess.py
+-rw-rw-rw-   0        0        0    25827 2022-01-24 07:22:21.000000 pyxllib-0.3.9/pyxlpr/ppocr/postprocess/rec_postprocess.py
+-rw-rw-rw-   0        0        0    14016 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/postprocess/sast_postprocess.py
+drwxrwxrwx   0        0        0        0 2022-10-18 02:03:36.062989 pyxllib-0.3.9/pyxlpr/ppocr/tools/
+-rw-rw-rw-   0        0        0      708 2022-01-14 02:59:47.000000 pyxllib-0.3.9/pyxlpr/ppocr/tools/__init__.py
+-rw-rw-rw-   0        0        0     3132 2022-04-14 09:58:24.000000 pyxllib-0.3.9/pyxlpr/ppocr/tools/eval.py
+-rw-rw-rw-   0        0        0     2777 2022-04-27 02:43:32.000000 pyxllib-0.3.9/pyxlpr/ppocr/tools/export_center.py
+-rw-rw-rw-   0        0        0     5319 2022-04-14 09:58:35.000000 pyxllib-0.3.9/pyxlpr/ppocr/tools/export_model.py
+drwxrwxrwx   0        0        0        0 2022-10-18 02:03:36.073958 pyxllib-0.3.9/pyxlpr/ppocr/tools/infer/
+-rw-rw-rw-   0        0        0     5927 2022-04-27 02:43:57.000000 pyxllib-0.3.9/pyxlpr/ppocr/tools/infer/predict_cls.py
+-rw-rw-rw-   0        0        0    11911 2022-04-27 02:35:39.000000 pyxllib-0.3.9/pyxlpr/ppocr/tools/infer/predict_det.py
+-rw-rw-rw-   0        0        0     6501 2022-04-27 02:44:01.000000 pyxllib-0.3.9/pyxlpr/ppocr/tools/infer/predict_e2e.py
+-rw-rw-rw-   0        0        0    17592 2022-04-14 06:12:47.000000 pyxllib-0.3.9/pyxlpr/ppocr/tools/infer/predict_rec.py
+-rw-rw-rw-   0        0        0     7531 2022-04-14 06:12:33.000000 pyxllib-0.3.9/pyxlpr/ppocr/tools/infer/predict_system.py
+-rw-rw-rw-   0        0        0    25355 2022-04-14 10:43:39.000000 pyxllib-0.3.9/pyxlpr/ppocr/tools/infer/utility.py
+-rw-rw-rw-   0        0        0     2747 2022-04-27 02:43:41.000000 pyxllib-0.3.9/pyxlpr/ppocr/tools/infer_cls.py
+-rw-rw-rw-   0        0        0     5009 2022-04-14 09:58:45.000000 pyxllib-0.3.9/pyxlpr/ppocr/tools/infer_det.py
+-rw-rw-rw-   0        0        0     4472 2022-04-27 02:43:44.000000 pyxllib-0.3.9/pyxlpr/ppocr/tools/infer_e2e.py
+-rw-rw-rw-   0        0        0     5558 2022-04-27 02:43:47.000000 pyxllib-0.3.9/pyxlpr/ppocr/tools/infer_kie.py
+-rw-rw-rw-   0        0        0     5865 2022-04-27 02:43:50.000000 pyxllib-0.3.9/pyxlpr/ppocr/tools/infer_rec.py
+-rw-rw-rw-   0        0        0     3842 2022-04-27 02:43:54.000000 pyxllib-0.3.9/pyxlpr/ppocr/tools/infer_table.py
+-rw-rw-rw-   0        0        0    24550 2022-07-16 08:06:04.000000 pyxllib-0.3.9/pyxlpr/ppocr/tools/program.py
+-rw-rw-rw-   0        0        0     4200 2022-04-27 02:47:07.000000 pyxllib-0.3.9/pyxlpr/ppocr/tools/test_hubserving.py
+-rw-rw-rw-   0        0        0     6109 2022-04-14 09:59:15.000000 pyxllib-0.3.9/pyxlpr/ppocr/tools/train.py
+-rw-rw-rw-   0        0        0    33700 2022-09-02 09:04:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/tools/xlprog.py
+drwxrwxrwx   0        0        0        0 2022-10-18 02:03:36.104722 pyxllib-0.3.9/pyxlpr/ppocr/utils/
+-rw-rw-rw-   0        0        0      280 2022-01-14 02:17:07.000000 pyxllib-0.3.9/pyxlpr/ppocr/utils/EN_symbol_dict.txt
+-rw-rw-rw-   0        0        0      881 2022-04-29 07:46:48.000000 pyxllib-0.3.9/pyxlpr/ppocr/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2022-10-18 02:03:36.180095 pyxllib-0.3.9/pyxlpr/ppocr/utils/dict/
+-rw-rw-rw-   0        0        0      390 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/utils/dict/ar_dict.txt
+-rw-rw-rw-   0        0        0      569 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/utils/dict/arabic_dict.txt
+-rw-rw-rw-   0        0        0      502 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/utils/dict/be_dict.txt
+-rw-rw-rw-   0        0        0      481 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/utils/dict/bg_dict.txt
+-rw-rw-rw-   0        0        0    41864 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/utils/dict/chinese_cht_dict.txt
+-rw-rw-rw-   0        0        0      573 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/utils/dict/cyrillic_dict.txt
+-rw-rw-rw-   0        0        0      675 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/utils/dict/devanagari_dict.txt
+-rw-rw-rw-   0        0        0      189 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/utils/dict/en_dict.txt
+-rw-rw-rw-   0        0        0      466 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/utils/dict/fa_dict.txt
+-rw-rw-rw-   0        0        0      460 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/utils/dict/french_dict.txt
+-rw-rw-rw-   0        0        0      489 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/utils/dict/german_dict.txt
+-rw-rw-rw-   0        0        0      650 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/utils/dict/hi_dict.txt
+-rw-rw-rw-   0        0        0      384 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/utils/dict/it_dict.txt
+-rw-rw-rw-   0        0        0    21731 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/utils/dict/japan_dict.txt
+-rw-rw-rw-   0        0        0      606 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/utils/dict/ka_dict.txt
+-rw-rw-rw-   0        0        0    18168 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/utils/dict/korean_dict.txt
+-rw-rw-rw-   0        0        0      653 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/utils/dict/latin_dict.txt
+-rw-rw-rw-   0        0        0      605 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/utils/dict/mr_dict.txt
+-rw-rw-rw-   0        0        0      605 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/utils/dict/ne_dict.txt
+-rw-rw-rw-   0        0        0      306 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/utils/dict/oc_dict.txt
+-rw-rw-rw-   0        0        0      435 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/utils/dict/pu_dict.txt
+-rw-rw-rw-   0        0        0      285 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/utils/dict/rs_dict.txt
+-rw-rw-rw-   0        0        0      458 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/utils/dict/rsc_dict.txt
+-rw-rw-rw-   0        0        0      438 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/utils/dict/ru_dict.txt
+-rw-rw-rw-   0        0        0      481 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/utils/dict/ta_dict.txt
+-rw-rw-rw-   0        0        0     1171 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/utils/dict/table_dict.txt
+-rw-rw-rw-   0        0        0    21350 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/utils/dict/table_structure_dict.txt
+-rw-rw-rw-   0        0        0      580 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/utils/dict/te_dict.txt
+-rw-rw-rw-   0        0        0      377 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/utils/dict/ug_dict.txt
+-rw-rw-rw-   0        0        0      490 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/utils/dict/uk_dict.txt
+-rw-rw-rw-   0        0        0      469 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/utils/dict/ur_dict.txt
+-rw-rw-rw-   0        0        0      360 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/utils/dict/xi_dict.txt
+-rw-rw-rw-   0        0        0      268 2022-01-14 02:17:07.000000 pyxllib-0.3.9/pyxlpr/ppocr/utils/dict90.txt
+drwxrwxrwx   0        0        0        0 2022-10-18 02:03:36.186080 pyxllib-0.3.9/pyxlpr/ppocr/utils/e2e_metric/
+-rw-rw-rw-   0        0        0    26617 2022-04-14 10:43:48.000000 pyxllib-0.3.9/pyxlpr/ppocr/utils/e2e_metric/Deteval.py
+-rw-rw-rw-   0        0        0     2925 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/utils/e2e_metric/polygon_fast.py
+drwxrwxrwx   0        0        0        0 2022-10-18 02:03:36.198046 pyxllib-0.3.9/pyxlpr/ppocr/utils/e2e_utils/
+-rw-rw-rw-   0        0        0     3373 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/utils/e2e_utils/extract_batchsize.py
+-rw-rw-rw-   0        0        0    17760 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/utils/e2e_utils/extract_textpoint_fast.py
+-rw-rw-rw-   0        0        0    22815 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/utils/e2e_utils/extract_textpoint_slow.py
+-rw-rw-rw-   0        0        0     6513 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/utils/e2e_utils/pgnet_pp_utils.py
+-rw-rw-rw-   0        0        0     5420 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/utils/e2e_utils/visual.py
+-rw-rw-rw-   0        0        0      285 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/utils/en_dict.txt
+-rw-rw-rw-   0        0        0     3054 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/utils/gen_label.py
+-rw-rw-rw-   0        0        0      106 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/utils/ic15_dict.txt
+-rw-rw-rw-   0        0        0     1754 2022-01-14 02:17:07.000000 pyxllib-0.3.9/pyxlpr/ppocr/utils/iou.py
+-rw-rw-rw-   0        0        0     2724 2022-01-13 02:16:10.000000 pyxllib-0.3.9/pyxlpr/ppocr/utils/logging.py
+-rw-rw-rw-   0        0        0     3253 2022-04-14 10:43:43.000000 pyxllib-0.3.9/pyxlpr/ppocr/utils/network.py
+-rw-rw-rw-   0        0        0    32871 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/utils/ppocr_keys_v1.txt
+-rw-rw-rw-   0        0        0     4503 2022-01-14 02:17:07.000000 pyxllib-0.3.9/pyxlpr/ppocr/utils/profiler.py
+-rw-rw-rw-   0        0        0     5637 2022-04-14 02:31:32.000000 pyxllib-0.3.9/pyxlpr/ppocr/utils/save_load.py
+-rw-rw-rw-   0        0        0     2304 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppocr/utils/stats.py
+-rw-rw-rw-   0        0        0     3160 2022-01-14 06:09:57.000000 pyxllib-0.3.9/pyxlpr/ppocr/utils/utility.py
+drwxrwxrwx   0        0        0        0 2022-10-18 02:03:36.207022 pyxllib-0.3.9/pyxlpr/ppstructure/
+-rw-rw-rw-   0        0        0      621 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppstructure/__init__.py
+-rw-rw-rw-   0        0        0     7797 2022-04-27 02:47:14.000000 pyxllib-0.3.9/pyxlpr/ppstructure/predict_system.py
+drwxrwxrwx   0        0        0        0 2022-10-18 02:03:36.221983 pyxllib-0.3.9/pyxlpr/ppstructure/table/
+-rw-rw-rw-   0        0        0      621 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppstructure/table/__init__.py
+-rw-rw-rw-   0        0        0     2377 2022-04-14 10:44:53.000000 pyxllib-0.3.9/pyxlpr/ppstructure/table/eval_table.py
+-rw-rw-rw-   0        0        0     7168 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppstructure/table/matcher.py
+-rw-rw-rw-   0        0        0     4663 2022-04-27 02:44:04.000000 pyxllib-0.3.9/pyxlpr/ppstructure/table/predict_structure.py
+-rw-rw-rw-   0        0        0     8851 2022-04-27 02:44:08.000000 pyxllib-0.3.9/pyxlpr/ppstructure/table/predict_table.py
+drwxrwxrwx   0        0        0        0 2022-10-18 02:03:36.228963 pyxllib-0.3.9/pyxlpr/ppstructure/table/table_metric/
+-rw-rw-rw-   0        0        0      673 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppstructure/table/table_metric/__init__.py
+-rw-rw-rw-   0        0        0     2198 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppstructure/table/table_metric/parallel.py
+-rw-rw-rw-   0        0        0     9532 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppstructure/table/table_metric/table_metric.py
+drwxrwxrwx   0        0        0        0 2022-10-18 02:03:36.243924 pyxllib-0.3.9/pyxlpr/ppstructure/table/tablepyxl/
+-rw-rw-rw-   0        0        0      619 2021-12-14 06:42:13.000000 pyxllib-0.3.9/pyxlpr/ppstructure/table/tablepyxl/__init__.py
+-rw-rw-rw-   0        0        0    10415 2022-04-22 12:24:19.000000 pyxllib-0.3.9/pyxlpr/ppstructure/table/tablepyxl/style.py
+-rw-rw-rw-   0        0        0     4217 2022-04-22 12:24:30.000000 pyxllib-0.3.9/pyxlpr/ppstructure/table/tablepyxl/tablepyxl.py
+-rw-rw-rw-   0        0        0     2538 2022-04-14 06:13:21.000000 pyxllib-0.3.9/pyxlpr/ppstructure/utility.py
+-rw-rw-rw-   0        0        0      260 2022-08-10 07:36:15.000000 pyxllib-0.3.9/pyxlpr/xlai.py
+-rw-rw-rw-   0        0        0      212 2022-07-12 12:58:43.000000 pyxllib-0.3.9/requirements.txt
+-rw-rw-rw-   0        0        0       42 2022-10-18 02:03:36.258883 pyxllib-0.3.9/setup.cfg
+-rw-rw-rw-   0        0        0     2414 2022-10-18 02:03:31.000000 pyxllib-0.3.9/setup.py
+drwxrwxrwx   0        0        0        0 2022-10-18 02:03:36.253898 pyxllib-0.3.9/xlproject/
+-rw-rw-rw-   0        0        0        0 2022-04-14 01:52:34.000000 pyxllib-0.3.9/xlproject/__init__.py
+-rw-rw-rw-   0        0        0    46439 2022-10-05 01:24:13.000000 pyxllib-0.3.9/xlproject/kq5034lib.py
+-rw-rw-rw-   0        0        0    27561 2022-09-13 07:50:23.000000 pyxllib-0.3.9/xlproject/核酸统计工具_在线版.py
```

### Comparing `pyxllib-0.3.8.1/LICENSE` & `pyxllib-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/PKG-INFO` & `pyxllib-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxllib
-Version: 0.3.8.1
+Version: 0.3.9
 Summary: 厦门理工模式识别团队通用python代码工具库
 Home-page: https://github.com/XLPRUtils/pyxllib
 Author: code4101
 Author-email: 877362867@qq.com
 License: Apache License 2.0
 Keywords: pyxllib,pyxlpr,xlproject
 Platform: UNKNOWN
```

### Comparing `pyxllib-0.3.8.1/pyxllib/__init__.py` & `pyxllib-0.3.9/pyxllib/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxllib/algo/disjoint.py` & `pyxllib-0.3.9/pyxllib/algo/disjoint.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxllib/algo/geo.py` & `pyxllib-0.3.9/pyxllib/algo/geo.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxllib/algo/intervals.py` & `pyxllib-0.3.9/pyxllib/algo/intervals.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxllib/algo/newbie.py` & `pyxllib-0.3.9/pyxllib/algo/newbie.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxllib/algo/pupil.py` & `pyxllib-0.3.9/pyxllib/algo/pupil.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxllib/algo/shapelylib.py` & `pyxllib-0.3.9/pyxllib/algo/shapelylib.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxllib/algo/specialist.py` & `pyxllib-0.3.9/pyxllib/algo/specialist.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxllib/algo/stat.py` & `pyxllib-0.3.9/pyxllib/algo/stat.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxllib/algo/treelib.py` & `pyxllib-0.3.9/pyxllib/algo/treelib.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxllib/algo/unitlib.py` & `pyxllib-0.3.9/pyxllib/algo/unitlib.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxllib/cv/expert.py` & `pyxllib-0.3.9/pyxllib/cv/expert.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxllib/cv/imfile.py` & `pyxllib-0.3.9/pyxllib/cv/imfile.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxllib/cv/imhash.py` & `pyxllib-0.3.9/pyxllib/cv/imhash.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxllib/cv/rgbfmt.py` & `pyxllib-0.3.9/pyxllib/cv/rgbfmt.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxllib/cv/trackbartools.py` & `pyxllib-0.3.9/pyxllib/cv/trackbartools.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxllib/cv/xlcvlib.py` & `pyxllib-0.3.9/pyxllib/cv/xlcvlib.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxllib/cv/xlpillib.py` & `pyxllib-0.3.9/pyxllib/cv/xlpillib.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxllib/data/echarts.py` & `pyxllib-0.3.9/pyxllib/data/echarts.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxllib/data/oss.py` & `pyxllib-0.3.9/pyxllib/data/oss.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxllib/data/pglib.py` & `pyxllib-0.3.9/pyxllib/data/pglib.py`

 * *Files 7% similar despite different names*

```diff
@@ -201,14 +201,34 @@
         使用后，需要重启IDE重新加载环境变量
         并且本句明文代码需要删除
         """
         # TODO 目前只设一个账号，后续可以扩展支持多个账号指定配置
         # conninfo = 'postgresql://postgres:yourpassword@172.16.170.110/xlpr'
         return XlOsEnv.persist_set('XlprDbAccount', {'conninfo': conninfo, 'seckey': seckey}, encoding=True)
 
+    @classmethod
+    def connect(cls, conninfo='', seckey='', *,
+                autocommit=False, row_factory=None, context=None, **kwargs) -> 'XlprDb':
+        """ 因为要标记 -> XlprDb，IDE才会识别出类别，有自动补全功能
+        但在类中写@classmethod，无法标记 -> XlprDb，所以就放外面单独写一个方法了
+        """
+        d = XlOsEnv.get('XlprDbAccount', decoding=True)
+        if conninfo == '':
+            conninfo = d['conninfo']
+        if seckey == '':
+            seckey = d['seckey']
+        # 注意这里获取的是XlprDb类型
+        con = super(XlprDb, cls).connect(conninfo, autocommit=autocommit, row_factory=row_factory, context=context,
+                                         **kwargs)
+        con.seckey = seckey
+        return con
+
+    def __1_hosts相关数据表操作(self):
+        pass
+
     def update_host(self, host_name, accounts=None, **kwargs):
         """ 更新一台服务器的信息
 
         :param dict accounts: 账号信息，记得要列全，比如
             {'root': '123456', 'chenkunze': '654321'}
         """
         if not self.execute('SELECT EXISTS (SELECT FROM hosts WHERE host_name=%s)', (host_name,)).fetchone()[0]:
@@ -216,32 +236,54 @@
         if kwargs:
             self.update('hosts', kwargs, {'host_name': host_name})
         if accounts:
             self.execute('UPDATE hosts SET accounts=pgp_sym_encrypt(%s, %s) WHERE host_name=%s',
                          (json.dumps(accounts, ensure_ascii=False), self.seckey, host_name))
         self.commit()
 
-    @classmethod
-    def connect(cls, conninfo='', seckey='', *,
-                autocommit=False, row_factory=None, context=None, **kwargs) -> 'XlprDb':
-        """ 因为要标记 -> XlprDb，IDE才会识别出类别，有自动补全功能
-        但在类中写@classmethod，无法标记 -> XlprDb，所以就放外面单独写一个方法了
+    def set_host_account(self, host_name, user_name, passwd):
+        """ 设置某台服务器的一个账号密码
+
+        >> xldb.set_host_account('titan2', 'chenkunze', '123456')
+
         """
-        d = XlOsEnv.get('XlprDbAccount', decoding=True)
-        if conninfo == '':
-            conninfo = d['conninfo']
-        if seckey == '':
-            seckey = d['seckey']
-        con = super(XlprDb, cls).connect(conninfo,
-                                         autocommit=autocommit, row_factory=row_factory,
-                                         context=context, **kwargs)
-        con.seckey = seckey
-        return con
+        # 读取旧的账号密码字典数据
+        d = self.execute("SELECT pgp_sym_decrypt(accounts, %s)::jsonb FROM hosts WHERE host_name=%s",
+                         (self.seckey, host_name)).fetchone()[0]
+        # 修改字典数据
+        d[user_name] = str(passwd)
+        # 将新的字典数据写回数据库
+        self.execute('UPDATE hosts SET accounts=pgp_sym_encrypt(%s, %s) WHERE host_name=%s',
+                     (json.dumps(d, ensure_ascii=False), self.seckey, host_name))
+        self.commit()
+
+    def login_ssh(self, host_name, user_name, map_path=None, **kwargs):
+        """ 通过数据库里的服务器数据记录，直接登录服务器 """
+        from pyxllib.extend.unixlib import XlSSHClient
+
+        if host_name.startswith('g_'):
+            host_ip = self.execute("SELECT host_ip FROM hosts WHERE host_name='xlpr0'").fetchone()[0]
+            pw, port = self.execute('SELECT (pgp_sym_decrypt(accounts, %s)::jsonb)[%s]::text, frpc_port'
+                                    ' FROM hosts WHERE host_name=%s',
+                                    (self.seckey, user_name, host_name[2:])).fetchone()
+        else:
+            port = 22
+            host_ip, pw = self.execute('SELECT host_ip, (pgp_sym_decrypt(accounts, %s)::jsonb)[%s]::text'
+                                       ' FROM hosts WHERE host_name=%s',
+                                       (self.seckey, user_name, host_name)).fetchone()
+
+        if map_path is None:
+            if sys.platform == 'win32':
+                map_path = {'C:/': '/'}
+            else:
+                map_path = {'/': '/'}
 
-    def __1_xlapi相关数据表操作(self):
+        return XlSSHClient(host_ip, user_name, pw[1:-1], port=port, map_path=map_path, **kwargs)
+
+    def __2_xlapi相关数据表操作(self):
         """
         files，存储二进制文件的表
             etag，文件、二进制对应的etag值
             meta，可以存储不同数据类型一些特殊的属性，比如图片可以存储高、宽
                 但因为用户使用中，为了提高速度，以及减少PIL等依赖，执行中不做计算
                 可以其他途径使用定期脚本自动处理
         xlapi，底层api调用的记录统计
@@ -365,21 +407,55 @@
             if 'log_id' in res:  # 有xlapi_id的标记，就不用百度原本的log_id了
                 del res['log_id']
         else:
             res = func(buffer, **options)
 
         return res
 
-    def __2_host_trace相关可视化(self):
+    def __3_host_trace相关可视化(self):
         """ TODO dbview 改名 host_trace """
         pass
 
     def __dbtool(self):
         pass
 
+    def record_host_usage(self, cpu=True, gpu=True, disk=False):
+        """ 记录服务器各种状况，存储到PG数据库
+
+        TODO 并行处理
+        TODO 功能还可以增加：gpu显卡温度、硬盘读写速率检查、网络上传下载带宽
+        """
+        # 1 服务器列表
+        host_names = list(self.exec_col('SELECT host_name FROM hosts WHERE id > 1 ORDER BY id'))
+        host_cpu_gb = {h: v for h, v in self.execute('SELECT host_name, cpu_gb FROM hosts')}
+
+        # 2 去所有服务器取使用情况
+        for i, host_name in enumerate(host_names, start=1):
+            print('-' * 20, i, host_name, '-' * 20)
+            try:
+                ssh = self.login_ssh(host_name, 'root', relogin=5, relogin_interval=0.2)
+                status = {}
+                if cpu:
+                    data = ssh.check_cpu_usage(print_mode=True)
+                    status['cpu'] = {k: v[0] for k, v in data.items()}
+                    status['cpu_memory'] = {k: round(v[1] * host_cpu_gb[host_name] / 100, 2) for k, v in data.items()}
+                if gpu:
+                    status['gpu_memory'] = ssh.check_gpu_usage(print_mode=True)
+                if disk and host_name not in {'xlpr4'}:  # 四卡服务器明确有问题，不检查磁盘空间大小
+                    # 检查磁盘空间会很慢，如果超时可以跳过。
+                    status['disk_memory'] = ssh.check_disk_usage(print_mode=True, timeout=7200)
+            except Exception as e:
+                status = {'error': f'{str(type(e))[8:-2]}: {e}'}
+                print(status)
+
+            if status:
+                self.insert_row('host_trace',
+                                {'host_name': host_name, 'status': status, 'update_time': utc_timestamp(8)})
+            print()
+
     def _get_host_trace_total(self, mode, title, yaxis_name, date_trunc, recent, host_attr):
         # CREATE INDEX ON gpu_trace (update_time);  -- update_time最好建个索引
         ls = self.execute(textwrap.dedent(f"""\
         WITH cte1 AS (  -- 筛选近期内的数据，并且时间做trunc处理
             SELECT host_name, (status)['{mode}'], date_trunc('{date_trunc}', update_time) ttime
             FROM host_trace WHERE update_time > %s AND (status ? '{mode}')
         ), cte2 AS (  -- 每个时间里每个服务器的多条记录取平均
```

### Comparing `pyxllib-0.3.8.1/pyxllib/data/sqlite.py` & `pyxllib-0.3.9/pyxllib/data/sqlite.py`

 * *Files 10% similar despite different names*

```diff
@@ -63,14 +63,28 @@
         SELECT	从一个或多个表中检索某些记录。
     """
 
     def has_table(self, table_name):
         res = self.execute(f"SELECT name FROM sqlite_master WHERE type='table' AND name='{table_name}'").fetchone()
         return bool(res)
 
+    def get_table_names(self):
+        """ 获得所有表格名 """
+        return [x[0] for x in self.execute("SELECT name FROM sqlite_master WHERE type='table'")]
+
+    def count_all_talbe_rows(self):
+        """ 统计所有表格的数据行数 """
+        names = self.get_table_names()
+        ls = []
+        for name in names:
+            n = self.execute(f'SELECT count(*) FROM {name}').fetchone()[0]
+            ls.append([name, n])
+        ls.sort(key=lambda x: -x[1])
+        return ls
+
     @classmethod
     def autotype(cls, val):
         if isinstance(val, str):
             return 'text'
         elif isinstance(val, (int, bool)):
             return 'integer'
         elif isinstance(val, float):
@@ -179,7 +193,20 @@
             for idx, col in enumerate(cursor.description):
                 d[col[0]] = row[idx]
             return d
 
         cur = self.cursor()
         cur.row_factory = dict_factory
         return cur.execute(*args, **kwargs)
+
+    def vacuum(self):
+        """ 删除数据后，文件不会直接减小，需要使用vacuum来实际压缩文件占用空间 """
+        self.execute('vacuum')  # 不用 commit
+
+    def keep_top_n_rows(self, table_name, num, col_name='id'):
+        """ 只保留一小部分数据，常用来做lite、demo数据示例文件
+
+        :param col_name: 参照的列名
+        """
+        self.execute(f'DELETE FROM {table_name} WHERE {col_name} NOT IN'
+                     f'(SELECT {col_name} FROM {table_name} LIMIT {num})')
+        self.commit()
```

### Comparing `pyxllib-0.3.8.1/pyxllib/data/sqllib.py` & `pyxllib-0.3.9/pyxllib/data/sqllib.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxllib/extend/autogui/autogui.py` & `pyxllib-0.3.9/pyxllib/extend/autogui/autogui.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxllib/extend/autogui/virtualkey.py` & `pyxllib-0.3.9/pyxllib/extend/autogui/virtualkey.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxllib/extend/demolib.py` & `pyxllib-0.3.9/pyxllib/extend/demolib.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxllib/extend/old.py` & `pyxllib-0.3.9/pyxllib/extend/old.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxllib/extend/qt.py` & `pyxllib-0.3.9/pyxllib/extend/qt.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxllib/extend/tk.py` & `pyxllib-0.3.9/pyxllib/extend/tk.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxllib/extend/unixlib.py` & `pyxllib-0.3.9/pyxllib/extend/unixlib.py`

 * *Files 2% similar despite different names*

```diff
@@ -207,53 +207,29 @@
                 if human_readable:
                     return humanfriendly.format_size(self.size, binary=True)
                 else:
                     return sz
 
         self.Path = Path
 
-    @classmethod
-    def login(cls, host_name, user_name, map_path=None, **kwargs):
-        r""" 使用XlprDb里存储的服务器、账号信息，进行登录
-        """
-        from pyxllib.data.pglib import XlprDb
-
-        with XlprDb.connect() as con:
-            if host_name.startswith('g_'):
-                host_ip = con.execute("SELECT host_ip FROM hosts WHERE host_name='xlpr0'").fetchone()[0]
-                pw, port = con.execute('SELECT (pgp_sym_decrypt(accounts, %s)::jsonb)[%s]::text, frpc_port'
-                                       ' FROM hosts WHERE host_name=%s',
-                                       (con.seckey, user_name, host_name[2:])).fetchone()
-            else:
-                port = 22
-                host_ip, pw = con.execute('SELECT host_ip, (pgp_sym_decrypt(accounts, %s)::jsonb)[%s]::text'
-                                          ' FROM hosts WHERE host_name=%s',
-                                          (con.seckey, user_name, host_name)).fetchone()
-
-        if map_path is None:
-            if sys.platform == 'win32':
-                map_path = {'C:/': '/'}
-            else:
-                map_path = {'/': '/'}
-        return cls(host_ip, user_name, pw[1:-1], port=port, map_path=map_path, **kwargs)
-
     def exec(self, command, *args, ignore_errors=False, pipe_in=None, **kwargs):
         """ exec_command的简化版
 
         :param ignore_errors:
             如果stderr出错，则抛出异常，否则返回运行结果的文本数据
             注意有些功能比较特别，是会往stderr写一些内容，但不一定是报错的，如果需要精细控制，建议直接使用exec_command接口
 
             【备忘】
             nginx -t的两句返回，虽然是正确状态，默认是放在stderr的
             安装anaconda也是会有一些输出到stderr的内容
         :param pipe_in: 通过管道输入课交互式操作的内容
         """
         # 这个命令有些交互性的操作，需要通过管道输入文本的机制来代替手动交互的过程
         if pipe_in:
+            self.exec('mkdir -p /tmp/pipeins')
             host_file = '/tmp/pipeins/' + XlPath.tempfile().name
             # os.makedirs(XlPath(host_file).parent, exist_ok=True)
             self.write_file(host_file, pipe_in, newline='\n')
             command = f'{command} < {host_file}'
 
         # 执行命令
         stdin, stdout, stderr = self.exec_command(command, *args, **kwargs)
```

### Comparing `pyxllib-0.3.8.1/pyxllib/extend/utools.py` & `pyxllib-0.3.9/pyxllib/extend/utools.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxllib/extend/webhook.py` & `pyxllib-0.3.9/pyxllib/extend/webhook.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxllib/extend/win32lib.py` & `pyxllib-0.3.9/pyxllib/extend/win32lib.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxllib/file/docxlib.py` & `pyxllib-0.3.9/pyxllib/file/docxlib.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxllib/file/gitlib.py` & `pyxllib-0.3.9/pyxllib/file/gitlib.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxllib/file/movielib.py` & `pyxllib-0.3.9/pyxllib/file/movielib.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxllib/file/onenotelib.py` & `pyxllib-0.3.9/pyxllib/file/onenotelib.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxllib/file/packlib/__init__.py` & `pyxllib-0.3.9/pyxllib/file/packlib/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxllib/file/packlib/zipfile.py` & `pyxllib-0.3.9/pyxllib/file/packlib/zipfile.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxllib/file/pdflib.py` & `pyxllib-0.3.9/pyxllib/file/pdflib.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxllib/file/pupil.py` & `pyxllib-0.3.9/pyxllib/file/pupil.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxllib/file/specialist/dirlib.py` & `pyxllib-0.3.9/pyxllib/file/specialist/dirlib.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxllib/file/specialist/download.py` & `pyxllib-0.3.9/pyxllib/file/specialist/download.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxllib/file/specialist/filelib.py` & `pyxllib-0.3.9/pyxllib/file/specialist/filelib.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxllib/file/xlsxlib.py` & `pyxllib-0.3.9/pyxllib/file/xlsxlib.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxllib/prog/deprecatedlib.py` & `pyxllib-0.3.9/pyxllib/prog/deprecatedlib.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxllib/prog/newbie.py` & `pyxllib-0.3.9/pyxllib/prog/newbie.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxllib/prog/pupil.py` & `pyxllib-0.3.9/pyxllib/prog/pupil.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxllib/prog/sitepackages.py` & `pyxllib-0.3.9/pyxllib/prog/sitepackages.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxllib/prog/specialist/__init__.py` & `pyxllib-0.3.9/pyxllib/prog/specialist/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxllib/prog/specialist/bc.py` & `pyxllib-0.3.9/pyxllib/prog/specialist/bc.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxllib/prog/specialist/browser.py` & `pyxllib-0.3.9/pyxllib/prog/specialist/browser.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxllib/prog/specialist/common.py` & `pyxllib-0.3.9/pyxllib/prog/specialist/common.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxllib/prog/specialist/datetime.py` & `pyxllib-0.3.9/pyxllib/prog/specialist/datetime.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxllib/prog/specialist/tictoc.py` & `pyxllib-0.3.9/pyxllib/prog/specialist/tictoc.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxllib/prog/specialist/xllog.py` & `pyxllib-0.3.9/pyxllib/prog/specialist/xllog.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxllib/stdlib/__init__.py` & `pyxllib-0.3.9/pyxllib/stdlib/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxllib/stdlib/tablepyxl/style.py` & `pyxllib-0.3.9/pyxllib/stdlib/tablepyxl/style.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxllib/stdlib/tablepyxl/tablepyxl.py` & `pyxllib-0.3.9/pyxllib/stdlib/tablepyxl/tablepyxl.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxllib/text/ahocorasick.py` & `pyxllib-0.3.9/pyxllib/text/ahocorasick.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxllib/text/latex/__init__.py` & `pyxllib-0.3.9/pyxllib/text/latex/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxllib/text/levenshtein.py` & `pyxllib-0.3.9/pyxllib/text/levenshtein.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxllib/text/nestenv.py` & `pyxllib-0.3.9/pyxllib/text/nestenv.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxllib/text/newbie.py` & `pyxllib-0.3.9/pyxllib/text/newbie.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxllib/text/pupil/common.py` & `pyxllib-0.3.9/pyxllib/text/pupil/common.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxllib/text/pupil/xlalign.py` & `pyxllib-0.3.9/pyxllib/text/pupil/xlalign.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxllib/text/pycode.py` & `pyxllib-0.3.9/pyxllib/text/pycode.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxllib/text/specialist/common.py` & `pyxllib-0.3.9/pyxllib/text/specialist/common.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxllib/text/specialist/ptag.py` & `pyxllib-0.3.9/pyxllib/text/specialist/ptag.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxllib/text/spellchecker.py` & `pyxllib-0.3.9/pyxllib/text/spellchecker.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxllib/text/xmllib.py` & `pyxllib-0.3.9/pyxllib/text/xmllib.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxllib/xl.py` & `pyxllib-0.3.9/pyxllib/xl.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxllib/xlcv.py` & `pyxllib-0.3.9/pyxllib/xlcv.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxllib.egg-info/PKG-INFO` & `pyxllib-0.3.9/pyxllib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxllib
-Version: 0.3.8.1
+Version: 0.3.9
 Summary: 厦门理工模式识别团队通用python代码工具库
 Home-page: https://github.com/XLPRUtils/pyxllib
 Author: code4101
 Author-email: 877362867@qq.com
 License: Apache License 2.0
 Keywords: pyxllib,pyxlpr,xlproject
 Platform: UNKNOWN
```

### Comparing `pyxllib-0.3.8.1/pyxllib.egg-info/SOURCES.txt` & `pyxllib-0.3.9/pyxllib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ai/clientlib.py` & `pyxllib-0.3.9/pyxlpr/ai/clientlib.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ai/specialist.py` & `pyxllib-0.3.9/pyxlpr/ai/specialist.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ai/torch_app.py` & `pyxllib-0.3.9/pyxlpr/ai/torch_app.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ai/xlpaddle.py` & `pyxllib-0.3.9/pyxlpr/ai/xlpaddle.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ai/xltorch.py` & `pyxllib-0.3.9/pyxlpr/ai/xltorch.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/data/coco.py` & `pyxllib-0.3.9/pyxlpr/data/coco.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/data/datacls.py` & `pyxllib-0.3.9/pyxlpr/data/datacls.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/data/datasets.py` & `pyxllib-0.3.9/pyxlpr/data/datasets.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/data/icdar/__init__.py` & `pyxllib-0.3.9/pyxlpr/data/icdar/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/data/icdar/deteval.py` & `pyxllib-0.3.9/pyxlpr/data/icdar/deteval.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/data/icdar/icdar2013.py` & `pyxllib-0.3.9/pyxlpr/data/icdar/icdar2013.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/data/icdar/iou.py` & `pyxllib-0.3.9/pyxlpr/data/icdar/iou.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/data/icdar/rrc_evaluation_funcs_1_1.py` & `pyxllib-0.3.9/pyxlpr/data/icdar/rrc_evaluation_funcs_1_1.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/data/imtextline.py` & `pyxllib-0.3.9/pyxlpr/data/imtextline.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/data/labelme.py` & `pyxllib-0.3.9/pyxlpr/data/labelme.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/data/removeline.py` & `pyxllib-0.3.9/pyxlpr/data/removeline.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/data/specialist.py` & `pyxllib-0.3.9/pyxlpr/data/specialist.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/eval/__init__.py` & `pyxllib-0.3.9/pyxlpr/eval/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/paddleocr.py` & `pyxllib-0.3.9/pyxlpr/paddleocr.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/__init__.py` & `pyxllib-0.3.9/pyxlpr/ppocr/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/configs/rec/multi_language/generate_multi_language_configs.py` & `pyxllib-0.3.9/pyxlpr/ppocr/configs/rec/multi_language/generate_multi_language_configs.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/data/__init__.py` & `pyxllib-0.3.9/pyxlpr/ppocr/data/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/data/imaug/ColorJitter.py` & `pyxllib-0.3.9/pyxlpr/ppocr/data/imaug/ColorJitter.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/data/imaug/__init__.py` & `pyxllib-0.3.9/pyxlpr/ppocr/data/imaug/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/data/imaug/copy_paste.py` & `pyxllib-0.3.9/pyxlpr/ppocr/data/imaug/copy_paste.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/data/imaug/east_process.py` & `pyxllib-0.3.9/pyxlpr/ppocr/data/imaug/east_process.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/data/imaug/gen_table_mask.py` & `pyxllib-0.3.9/pyxlpr/ppocr/data/imaug/gen_table_mask.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/data/imaug/iaa_augment.py` & `pyxllib-0.3.9/pyxlpr/ppocr/data/imaug/iaa_augment.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/data/imaug/label_ops.py` & `pyxllib-0.3.9/pyxlpr/ppocr/data/imaug/label_ops.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/data/imaug/make_border_map.py` & `pyxllib-0.3.9/pyxlpr/ppocr/data/imaug/make_border_map.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/data/imaug/make_pse_gt.py` & `pyxllib-0.3.9/pyxlpr/ppocr/data/imaug/make_pse_gt.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/data/imaug/make_shrink_map.py` & `pyxllib-0.3.9/pyxlpr/ppocr/data/imaug/make_shrink_map.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/data/imaug/operators.py` & `pyxllib-0.3.9/pyxlpr/ppocr/data/imaug/operators.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/data/imaug/pg_process.py` & `pyxllib-0.3.9/pyxlpr/ppocr/data/imaug/pg_process.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/data/imaug/randaugment.py` & `pyxllib-0.3.9/pyxlpr/ppocr/data/imaug/randaugment.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/data/imaug/random_crop_data.py` & `pyxllib-0.3.9/pyxlpr/ppocr/data/imaug/random_crop_data.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/data/imaug/rec_img_aug.py` & `pyxllib-0.3.9/pyxlpr/ppocr/data/imaug/rec_img_aug.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/data/imaug/sast_process.py` & `pyxllib-0.3.9/pyxlpr/ppocr/data/imaug/sast_process.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/data/imaug/text_image_aug/__init__.py` & `pyxllib-0.3.9/pyxlpr/ppocr/data/imaug/text_image_aug/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/data/imaug/text_image_aug/augment.py` & `pyxllib-0.3.9/pyxlpr/ppocr/data/imaug/text_image_aug/augment.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/data/imaug/text_image_aug/warp_mls.py` & `pyxllib-0.3.9/pyxlpr/ppocr/data/imaug/text_image_aug/warp_mls.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/data/lmdb_dataset.py` & `pyxllib-0.3.9/pyxlpr/ppocr/data/lmdb_dataset.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/data/pgnet_dataset.py` & `pyxllib-0.3.9/pyxlpr/ppocr/data/pgnet_dataset.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/data/pubtab_dataset.py` & `pyxllib-0.3.9/pyxlpr/ppocr/data/pubtab_dataset.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/data/simple_dataset.py` & `pyxllib-0.3.9/pyxlpr/ppocr/data/simple_dataset.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/losses/__init__.py` & `pyxllib-0.3.9/pyxlpr/ppocr/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/losses/ace_loss.py` & `pyxllib-0.3.9/pyxlpr/ppocr/losses/ace_loss.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/losses/basic_loss.py` & `pyxllib-0.3.9/pyxlpr/ppocr/losses/basic_loss.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/losses/center_loss.py` & `pyxllib-0.3.9/pyxlpr/ppocr/losses/center_loss.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/losses/cls_loss.py` & `pyxllib-0.3.9/pyxlpr/ppocr/losses/cls_loss.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/losses/combined_loss.py` & `pyxllib-0.3.9/pyxlpr/ppocr/losses/combined_loss.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/losses/det_basic_loss.py` & `pyxllib-0.3.9/pyxlpr/ppocr/losses/det_basic_loss.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/losses/det_db_loss.py` & `pyxllib-0.3.9/pyxlpr/ppocr/losses/det_db_loss.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/losses/det_east_loss.py` & `pyxllib-0.3.9/pyxlpr/ppocr/losses/det_east_loss.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/losses/det_pse_loss.py` & `pyxllib-0.3.9/pyxlpr/ppocr/losses/det_pse_loss.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/losses/det_sast_loss.py` & `pyxllib-0.3.9/pyxlpr/ppocr/losses/det_sast_loss.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/losses/distillation_loss.py` & `pyxllib-0.3.9/pyxlpr/ppocr/losses/distillation_loss.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/losses/e2e_pg_loss.py` & `pyxllib-0.3.9/pyxlpr/ppocr/losses/e2e_pg_loss.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/losses/kie_sdmgr_loss.py` & `pyxllib-0.3.9/pyxlpr/ppocr/losses/kie_sdmgr_loss.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/losses/rec_aster_loss.py` & `pyxllib-0.3.9/pyxlpr/ppocr/losses/rec_aster_loss.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/losses/rec_att_loss.py` & `pyxllib-0.3.9/pyxlpr/ppocr/losses/rec_att_loss.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/losses/rec_ctc_loss.py` & `pyxllib-0.3.9/pyxlpr/ppocr/losses/rec_ctc_loss.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/losses/rec_enhanced_ctc_loss.py` & `pyxllib-0.3.9/pyxlpr/ppocr/losses/rec_enhanced_ctc_loss.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/losses/rec_nrtr_loss.py` & `pyxllib-0.3.9/pyxlpr/ppocr/losses/rec_nrtr_loss.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/losses/rec_sar_loss.py` & `pyxllib-0.3.9/pyxlpr/ppocr/losses/rec_sar_loss.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/losses/rec_srn_loss.py` & `pyxllib-0.3.9/pyxlpr/ppocr/losses/rec_srn_loss.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/losses/table_att_loss.py` & `pyxllib-0.3.9/pyxlpr/ppocr/losses/table_att_loss.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/metrics/__init__.py` & `pyxllib-0.3.9/pyxlpr/ppocr/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/metrics/cls_metric.py` & `pyxllib-0.3.9/pyxlpr/ppocr/metrics/cls_metric.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/metrics/det_metric.py` & `pyxllib-0.3.9/pyxlpr/ppocr/metrics/det_metric.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/metrics/distillation_metric.py` & `pyxllib-0.3.9/pyxlpr/ppocr/metrics/distillation_metric.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/metrics/e2e_metric.py` & `pyxllib-0.3.9/pyxlpr/ppocr/metrics/e2e_metric.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/metrics/eval_det_iou.py` & `pyxllib-0.3.9/pyxlpr/ppocr/metrics/eval_det_iou.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/metrics/kie_metric.py` & `pyxllib-0.3.9/pyxlpr/ppocr/metrics/kie_metric.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/metrics/rec_metric.py` & `pyxllib-0.3.9/pyxlpr/ppocr/metrics/rec_metric.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/metrics/table_metric.py` & `pyxllib-0.3.9/pyxlpr/ppocr/metrics/table_metric.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/architectures/__init__.py` & `pyxllib-0.3.9/pyxlpr/ppocr/modeling/architectures/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/architectures/base_model.py` & `pyxllib-0.3.9/pyxlpr/ppocr/modeling/architectures/base_model.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/architectures/distillation_model.py` & `pyxllib-0.3.9/pyxlpr/ppocr/modeling/architectures/distillation_model.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/backbones/__init__.py` & `pyxllib-0.3.9/pyxlpr/ppocr/modeling/backbones/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/backbones/det_mobilenet_v3.py` & `pyxllib-0.3.9/pyxlpr/ppocr/modeling/backbones/det_mobilenet_v3.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/backbones/det_resnet_vd.py` & `pyxllib-0.3.9/pyxlpr/ppocr/modeling/backbones/det_resnet_vd.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/backbones/det_resnet_vd_sast.py` & `pyxllib-0.3.9/pyxlpr/ppocr/modeling/backbones/det_resnet_vd_sast.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/backbones/e2e_resnet_vd_pg.py` & `pyxllib-0.3.9/pyxlpr/ppocr/modeling/backbones/e2e_resnet_vd_pg.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/backbones/kie_unet_sdmgr.py` & `pyxllib-0.3.9/pyxlpr/ppocr/modeling/backbones/kie_unet_sdmgr.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/backbones/rec_mobilenet_v3.py` & `pyxllib-0.3.9/pyxlpr/ppocr/modeling/backbones/rec_mobilenet_v3.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/backbones/rec_mv1_enhance.py` & `pyxllib-0.3.9/pyxlpr/ppocr/modeling/backbones/rec_mv1_enhance.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/backbones/rec_nrtr_mtb.py` & `pyxllib-0.3.9/pyxlpr/ppocr/modeling/backbones/rec_nrtr_mtb.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/backbones/rec_resnet_31.py` & `pyxllib-0.3.9/pyxlpr/ppocr/modeling/backbones/rec_resnet_31.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/backbones/rec_resnet_aster.py` & `pyxllib-0.3.9/pyxlpr/ppocr/modeling/backbones/rec_resnet_aster.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/backbones/rec_resnet_fpn.py` & `pyxllib-0.3.9/pyxlpr/ppocr/modeling/backbones/rec_resnet_fpn.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/backbones/rec_resnet_vd.py` & `pyxllib-0.3.9/pyxlpr/ppocr/modeling/backbones/rec_resnet_vd.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/heads/__init__.py` & `pyxllib-0.3.9/pyxlpr/ppocr/modeling/heads/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/heads/cls_head.py` & `pyxllib-0.3.9/pyxlpr/ppocr/modeling/heads/cls_head.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/heads/det_db_head.py` & `pyxllib-0.3.9/pyxlpr/ppocr/modeling/heads/det_db_head.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/heads/det_east_head.py` & `pyxllib-0.3.9/pyxlpr/ppocr/modeling/heads/det_east_head.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/heads/det_pse_head.py` & `pyxllib-0.3.9/pyxlpr/ppocr/modeling/heads/det_pse_head.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/heads/det_sast_head.py` & `pyxllib-0.3.9/pyxlpr/ppocr/modeling/heads/det_sast_head.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/heads/e2e_pg_head.py` & `pyxllib-0.3.9/pyxlpr/ppocr/modeling/heads/e2e_pg_head.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/heads/kie_sdmgr_head.py` & `pyxllib-0.3.9/pyxlpr/ppocr/modeling/heads/kie_sdmgr_head.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/heads/multiheadAttention.py` & `pyxllib-0.3.9/pyxlpr/ppocr/modeling/heads/multiheadAttention.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/heads/rec_aster_head.py` & `pyxllib-0.3.9/pyxlpr/ppocr/modeling/heads/rec_aster_head.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/heads/rec_att_head.py` & `pyxllib-0.3.9/pyxlpr/ppocr/modeling/heads/rec_att_head.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/heads/rec_ctc_head.py` & `pyxllib-0.3.9/pyxlpr/ppocr/modeling/heads/rec_ctc_head.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/heads/rec_nrtr_head.py` & `pyxllib-0.3.9/pyxlpr/ppocr/modeling/heads/rec_nrtr_head.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/heads/rec_sar_head.py` & `pyxllib-0.3.9/pyxlpr/ppocr/modeling/heads/rec_sar_head.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/heads/rec_srn_head.py` & `pyxllib-0.3.9/pyxlpr/ppocr/modeling/heads/rec_srn_head.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/heads/self_attention.py` & `pyxllib-0.3.9/pyxlpr/ppocr/modeling/heads/self_attention.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/heads/table_att_head.py` & `pyxllib-0.3.9/pyxlpr/ppocr/modeling/heads/table_att_head.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/necks/__init__.py` & `pyxllib-0.3.9/pyxlpr/ppocr/modeling/necks/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/necks/db_fpn.py` & `pyxllib-0.3.9/pyxlpr/ppocr/modeling/necks/db_fpn.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/necks/east_fpn.py` & `pyxllib-0.3.9/pyxlpr/ppocr/modeling/necks/east_fpn.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/necks/fpn.py` & `pyxllib-0.3.9/pyxlpr/ppocr/modeling/necks/fpn.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/necks/pg_fpn.py` & `pyxllib-0.3.9/pyxlpr/ppocr/modeling/necks/pg_fpn.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/necks/rnn.py` & `pyxllib-0.3.9/pyxlpr/ppocr/modeling/necks/rnn.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/necks/sast_fpn.py` & `pyxllib-0.3.9/pyxlpr/ppocr/modeling/necks/sast_fpn.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/necks/table_fpn.py` & `pyxllib-0.3.9/pyxlpr/ppocr/modeling/necks/table_fpn.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/transforms/__init__.py` & `pyxllib-0.3.9/pyxlpr/ppocr/modeling/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/transforms/stn.py` & `pyxllib-0.3.9/pyxlpr/ppocr/modeling/transforms/stn.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/transforms/tps.py` & `pyxllib-0.3.9/pyxlpr/ppocr/modeling/transforms/tps.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/modeling/transforms/tps_spatial_transformer.py` & `pyxllib-0.3.9/pyxlpr/ppocr/modeling/transforms/tps_spatial_transformer.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/optimizer/__init__.py` & `pyxllib-0.3.9/pyxlpr/ppocr/optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/optimizer/learning_rate.py` & `pyxllib-0.3.9/pyxlpr/ppocr/optimizer/learning_rate.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/optimizer/lr_scheduler.py` & `pyxllib-0.3.9/pyxlpr/ppocr/optimizer/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/optimizer/optimizer.py` & `pyxllib-0.3.9/pyxlpr/ppocr/optimizer/optimizer.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/optimizer/regularizer.py` & `pyxllib-0.3.9/pyxlpr/ppocr/optimizer/regularizer.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/postprocess/__init__.py` & `pyxllib-0.3.9/pyxlpr/ppocr/postprocess/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/postprocess/cls_postprocess.py` & `pyxllib-0.3.9/pyxlpr/ppocr/postprocess/cls_postprocess.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/postprocess/db_postprocess.py` & `pyxllib-0.3.9/pyxlpr/ppocr/postprocess/db_postprocess.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/postprocess/east_postprocess.py` & `pyxllib-0.3.9/pyxlpr/ppocr/postprocess/east_postprocess.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/postprocess/locality_aware_nms.py` & `pyxllib-0.3.9/pyxlpr/ppocr/postprocess/locality_aware_nms.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/postprocess/pg_postprocess.py` & `pyxllib-0.3.9/pyxlpr/ppocr/postprocess/pg_postprocess.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/postprocess/pse_postprocess/__init__.py` & `pyxllib-0.3.9/pyxlpr/ppocr/postprocess/pse_postprocess/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/postprocess/pse_postprocess/pse/__init__.py` & `pyxllib-0.3.9/pyxlpr/ppocr/postprocess/pse_postprocess/pse/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/postprocess/pse_postprocess/pse_postprocess.py` & `pyxllib-0.3.9/pyxlpr/ppocr/postprocess/pse_postprocess/pse_postprocess.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/postprocess/rec_postprocess.py` & `pyxllib-0.3.9/pyxlpr/ppocr/postprocess/rec_postprocess.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/postprocess/sast_postprocess.py` & `pyxllib-0.3.9/pyxlpr/ppocr/postprocess/sast_postprocess.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/tools/__init__.py` & `pyxllib-0.3.9/pyxlpr/ppocr/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/tools/eval.py` & `pyxllib-0.3.9/pyxlpr/ppocr/tools/eval.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/tools/export_center.py` & `pyxllib-0.3.9/pyxlpr/ppocr/tools/export_center.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/tools/export_model.py` & `pyxllib-0.3.9/pyxlpr/ppocr/tools/export_model.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/tools/infer/predict_cls.py` & `pyxllib-0.3.9/pyxlpr/ppocr/tools/infer/predict_cls.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/tools/infer/predict_det.py` & `pyxllib-0.3.9/pyxlpr/ppocr/tools/infer/predict_det.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/tools/infer/predict_e2e.py` & `pyxllib-0.3.9/pyxlpr/ppocr/tools/infer/predict_e2e.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/tools/infer/predict_rec.py` & `pyxllib-0.3.9/pyxlpr/ppocr/tools/infer/predict_rec.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/tools/infer/predict_system.py` & `pyxllib-0.3.9/pyxlpr/ppocr/tools/infer/predict_system.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/tools/infer/utility.py` & `pyxllib-0.3.9/pyxlpr/ppocr/tools/infer/utility.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/tools/infer_cls.py` & `pyxllib-0.3.9/pyxlpr/ppocr/tools/infer_cls.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/tools/infer_det.py` & `pyxllib-0.3.9/pyxlpr/ppocr/tools/infer_det.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/tools/infer_e2e.py` & `pyxllib-0.3.9/pyxlpr/ppocr/tools/infer_e2e.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/tools/infer_kie.py` & `pyxllib-0.3.9/pyxlpr/ppocr/tools/infer_kie.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/tools/infer_rec.py` & `pyxllib-0.3.9/pyxlpr/ppocr/tools/infer_rec.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/tools/infer_table.py` & `pyxllib-0.3.9/pyxlpr/ppocr/tools/infer_table.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/tools/program.py` & `pyxllib-0.3.9/pyxlpr/ppocr/tools/program.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/tools/test_hubserving.py` & `pyxllib-0.3.9/pyxlpr/ppocr/tools/test_hubserving.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/tools/train.py` & `pyxllib-0.3.9/pyxlpr/ppocr/tools/train.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/tools/xlprog.py` & `pyxllib-0.3.9/pyxlpr/ppocr/tools/xlprog.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/utils/__init__.py` & `pyxllib-0.3.9/pyxlpr/ppocr/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/utils/dict/arabic_dict.txt` & `pyxllib-0.3.9/pyxlpr/ppocr/utils/dict/arabic_dict.txt`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/utils/dict/chinese_cht_dict.txt` & `pyxllib-0.3.9/pyxlpr/ppocr/utils/dict/chinese_cht_dict.txt`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/utils/dict/cyrillic_dict.txt` & `pyxllib-0.3.9/pyxlpr/ppocr/utils/dict/cyrillic_dict.txt`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/utils/dict/devanagari_dict.txt` & `pyxllib-0.3.9/pyxlpr/ppocr/utils/dict/devanagari_dict.txt`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/utils/dict/hi_dict.txt` & `pyxllib-0.3.9/pyxlpr/ppocr/utils/dict/hi_dict.txt`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/utils/dict/japan_dict.txt` & `pyxllib-0.3.9/pyxlpr/ppocr/utils/dict/japan_dict.txt`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/utils/dict/ka_dict.txt` & `pyxllib-0.3.9/pyxlpr/ppocr/utils/dict/ka_dict.txt`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/utils/dict/korean_dict.txt` & `pyxllib-0.3.9/pyxlpr/ppocr/utils/dict/korean_dict.txt`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/utils/dict/latin_dict.txt` & `pyxllib-0.3.9/pyxlpr/ppocr/utils/dict/latin_dict.txt`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/utils/dict/mr_dict.txt` & `pyxllib-0.3.9/pyxlpr/ppocr/utils/dict/mr_dict.txt`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/utils/dict/ne_dict.txt` & `pyxllib-0.3.9/pyxlpr/ppocr/utils/dict/ne_dict.txt`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/utils/dict/table_dict.txt` & `pyxllib-0.3.9/pyxlpr/ppocr/utils/dict/table_dict.txt`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/utils/dict/table_structure_dict.txt` & `pyxllib-0.3.9/pyxlpr/ppocr/utils/dict/table_structure_dict.txt`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/utils/dict/te_dict.txt` & `pyxllib-0.3.9/pyxlpr/ppocr/utils/dict/te_dict.txt`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/utils/e2e_metric/Deteval.py` & `pyxllib-0.3.9/pyxlpr/ppocr/utils/e2e_metric/Deteval.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/utils/e2e_metric/polygon_fast.py` & `pyxllib-0.3.9/pyxlpr/ppocr/utils/e2e_metric/polygon_fast.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/utils/e2e_utils/extract_batchsize.py` & `pyxllib-0.3.9/pyxlpr/ppocr/utils/e2e_utils/extract_batchsize.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/utils/e2e_utils/extract_textpoint_fast.py` & `pyxllib-0.3.9/pyxlpr/ppocr/utils/e2e_utils/extract_textpoint_fast.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/utils/e2e_utils/extract_textpoint_slow.py` & `pyxllib-0.3.9/pyxlpr/ppocr/utils/e2e_utils/extract_textpoint_slow.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/utils/e2e_utils/pgnet_pp_utils.py` & `pyxllib-0.3.9/pyxlpr/ppocr/utils/e2e_utils/pgnet_pp_utils.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/utils/e2e_utils/visual.py` & `pyxllib-0.3.9/pyxlpr/ppocr/utils/e2e_utils/visual.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/utils/gen_label.py` & `pyxllib-0.3.9/pyxlpr/ppocr/utils/gen_label.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/utils/iou.py` & `pyxllib-0.3.9/pyxlpr/ppocr/utils/iou.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/utils/logging.py` & `pyxllib-0.3.9/pyxlpr/ppocr/utils/logging.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/utils/network.py` & `pyxllib-0.3.9/pyxlpr/ppocr/utils/network.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/utils/ppocr_keys_v1.txt` & `pyxllib-0.3.9/pyxlpr/ppocr/utils/ppocr_keys_v1.txt`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/utils/profiler.py` & `pyxllib-0.3.9/pyxlpr/ppocr/utils/profiler.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/utils/save_load.py` & `pyxllib-0.3.9/pyxlpr/ppocr/utils/save_load.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/utils/stats.py` & `pyxllib-0.3.9/pyxlpr/ppocr/utils/stats.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppocr/utils/utility.py` & `pyxllib-0.3.9/pyxlpr/ppocr/utils/utility.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppstructure/__init__.py` & `pyxllib-0.3.9/pyxlpr/ppstructure/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppstructure/predict_system.py` & `pyxllib-0.3.9/pyxlpr/ppstructure/predict_system.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppstructure/table/__init__.py` & `pyxllib-0.3.9/pyxlpr/ppstructure/table/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppstructure/table/eval_table.py` & `pyxllib-0.3.9/pyxlpr/ppstructure/table/eval_table.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppstructure/table/matcher.py` & `pyxllib-0.3.9/pyxlpr/ppstructure/table/matcher.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppstructure/table/predict_structure.py` & `pyxllib-0.3.9/pyxlpr/ppstructure/table/predict_structure.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppstructure/table/predict_table.py` & `pyxllib-0.3.9/pyxlpr/ppstructure/table/predict_table.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppstructure/table/table_metric/__init__.py` & `pyxllib-0.3.9/pyxlpr/ppstructure/table/table_metric/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppstructure/table/table_metric/parallel.py` & `pyxllib-0.3.9/pyxlpr/ppstructure/table/table_metric/parallel.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppstructure/table/table_metric/table_metric.py` & `pyxllib-0.3.9/pyxlpr/ppstructure/table/table_metric/table_metric.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppstructure/table/tablepyxl/__init__.py` & `pyxllib-0.3.9/pyxlpr/ppstructure/table/tablepyxl/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppstructure/table/tablepyxl/style.py` & `pyxllib-0.3.9/pyxlpr/ppstructure/table/tablepyxl/style.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppstructure/table/tablepyxl/tablepyxl.py` & `pyxllib-0.3.9/pyxlpr/ppstructure/table/tablepyxl/tablepyxl.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/pyxlpr/ppstructure/utility.py` & `pyxllib-0.3.9/pyxlpr/ppstructure/utility.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/setup.py` & `pyxllib-0.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 """
 # fvcore
 
 _dir = Path(__file__).parent
 
 setup(
     name='pyxllib',  # pip 安装时用的名字
-    version='0.3.8.1',  # 当前版本，每次更新上传到pypi都需要修改; 第4位版本号一般是修紧急bug
+    version='0.3.9',  # 当前版本，每次更新上传到pypi都需要修改; 第4位版本号一般是修紧急bug
     author='code4101',
     author_email='877362867@qq.com',
     url='https://github.com/XLPRUtils/pyxllib',
     keywords=['pyxllib', 'pyxlpr', 'xlproject'],
     description='厦门理工模式识别团队通用python代码工具库',
     long_description=(_dir / 'README.md').read_text(),  # 偷懒，就不创建f然后close了~~
     long_description_content_type='text/markdown',
```

### Comparing `pyxllib-0.3.8.1/xlproject/kq5034lib.py` & `pyxllib-0.3.9/xlproject/kq5034lib.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.8.1/xlproject/核酸统计工具_在线版.py` & `pyxllib-0.3.9/xlproject/核酸统计工具_在线版.py`

 * *Files identical despite different names*

