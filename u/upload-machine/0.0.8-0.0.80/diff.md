# Comparing `tmp/upload_machine-0.0.8.tar.gz` & `tmp/upload_machine-0.0.80.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/upload_machine-0.0.8.tar", last modified: Sun Oct  9 10:11:37 2022, max compression
+gzip compressed data, was "upload_machine-0.0.80.tar", last modified: Sun Aug  6 09:32:49 2023, max compression
```

## Comparing `upload_machine-0.0.8.tar` & `upload_machine-0.0.80.tar`

### file list

```diff
@@ -1,70 +1,84 @@
-drwxr-xr-x   0 moyu       (501) staff       (20)        0 2022-10-09 10:11:37.525736 upload_machine-0.0.8/
--rw-------   0 moyu       (501) staff       (20)       37 2022-10-06 08:50:43.000000 upload_machine-0.0.8/MANIFEST.in
--rw-r--r--   0 moyu       (501) staff       (20)    16463 2022-10-09 10:11:37.525339 upload_machine-0.0.8/PKG-INFO
--rw-------   0 moyu       (501) staff       (20)    12909 2022-10-09 09:42:11.000000 upload_machine-0.0.8/README.md
--rw-r--r--   0 moyu       (501) staff       (20)       38 2022-10-09 10:11:37.525834 upload_machine-0.0.8/setup.cfg
--rw-------   0 moyu       (501) staff       (20)     1085 2022-10-09 10:11:31.000000 upload_machine-0.0.8/setup.py
-drwxr-xr-x   0 moyu       (501) staff       (20)        0 2022-10-09 10:11:37.485881 upload_machine-0.0.8/upload_machine/
--rwxr-xr-x   0 moyu       (501) staff       (20)        0 2022-10-06 05:53:46.000000 upload_machine-0.0.8/upload_machine/__init__.py
--rw-------   0 moyu       (501) staff       (20)      241 2022-10-06 08:12:01.000000 upload_machine-0.0.8/upload_machine/basicinfo.yaml
--rw-------   0 moyu       (501) staff       (20)     2563 2022-10-08 03:16:09.000000 upload_machine-0.0.8/upload_machine/main.py
-drwxr-xr-x   0 moyu       (501) staff       (20)        0 2022-10-09 10:11:37.490089 upload_machine-0.0.8/upload_machine/utils/
--rw-------   0 moyu       (501) staff       (20)        0 2022-10-06 05:53:46.000000 upload_machine-0.0.8/upload_machine/utils/__init__.py
-drwxr-xr-x   0 moyu       (501) staff       (20)        0 2022-10-09 10:11:37.490565 upload_machine-0.0.8/upload_machine/utils/edittorrent/
--rw-------   0 moyu       (501) staff       (20)        0 2022-10-06 05:53:46.000000 upload_machine-0.0.8/upload_machine/utils/edittorrent/__init__.py
--rw-------   0 moyu       (501) staff       (20)     3966 2022-10-06 05:53:46.000000 upload_machine-0.0.8/upload_machine/utils/edittorrent/edittorrent.py
-drwxr-xr-x   0 moyu       (501) staff       (20)        0 2022-10-09 10:11:37.496482 upload_machine-0.0.8/upload_machine/utils/img_upload/
--rw-------   0 moyu       (501) staff       (20)        0 2022-10-06 05:53:46.000000 upload_machine-0.0.8/upload_machine/utils/img_upload/__init__.py
--rw-------   0 moyu       (501) staff       (20)     7231 2022-10-06 05:53:46.000000 upload_machine-0.0.8/upload_machine/utils/img_upload/chevereto.py
--rw-------   0 moyu       (501) staff       (20)     2674 2022-10-06 05:53:46.000000 upload_machine-0.0.8/upload_machine/utils/img_upload/fapping_emp.py
--rw-------   0 moyu       (501) staff       (20)     4521 2022-10-06 05:53:46.000000 upload_machine-0.0.8/upload_machine/utils/img_upload/imgbox.py
--rw-------   0 moyu       (501) staff       (20)     7893 2022-10-06 08:33:48.000000 upload_machine-0.0.8/upload_machine/utils/img_upload/imgupload.py
--rw-------   0 moyu       (501) staff       (20)     2510 2022-10-06 05:53:46.000000 upload_machine-0.0.8/upload_machine/utils/img_upload/ptpimg.py
--rw-------   0 moyu       (501) staff       (20)     2875 2022-10-06 05:53:46.000000 upload_machine-0.0.8/upload_machine/utils/img_upload/smms.py
-drwxr-xr-x   0 moyu       (501) staff       (20)        0 2022-10-09 10:11:37.502247 upload_machine-0.0.8/upload_machine/utils/mediafile/
--rw-------   0 moyu       (501) staff       (20)        0 2022-10-06 05:53:46.000000 upload_machine-0.0.8/upload_machine/utils/mediafile/__init__.py
--rw-------   0 moyu       (501) staff       (20)    17212 2022-10-06 05:53:46.000000 upload_machine-0.0.8/upload_machine/utils/mediafile/douban_book.py
--rw-------   0 moyu       (501) staff       (20)    24814 2022-10-06 05:53:46.000000 upload_machine-0.0.8/upload_machine/utils/mediafile/douban_movie.py
--rw-------   0 moyu       (501) staff       (20)     6861 2022-10-06 08:34:29.000000 upload_machine-0.0.8/upload_machine/utils/mediafile/doubaninfo.py
--rw-------   0 moyu       (501) staff       (20)    50539 2022-10-08 12:40:30.000000 upload_machine-0.0.8/upload_machine/utils/mediafile/mediafile.py
-drwxr-xr-x   0 moyu       (501) staff       (20)        0 2022-10-09 10:11:37.505879 upload_machine-0.0.8/upload_machine/utils/para_ctrl/
--rw-------   0 moyu       (501) staff       (20)      218 2022-10-06 08:34:43.000000 upload_machine-0.0.8/upload_machine/utils/para_ctrl/__init__.py
--rw-------   0 moyu       (501) staff       (20)     6779 2022-10-09 10:10:39.000000 upload_machine-0.0.8/upload_machine/utils/para_ctrl/para_ctrl.py
--rw-------   0 moyu       (501) staff       (20)     2112 2022-10-06 08:36:10.000000 upload_machine-0.0.8/upload_machine/utils/para_ctrl/readargs.py
--rw-------   0 moyu       (501) staff       (20)     1156 2022-10-06 05:53:46.000000 upload_machine-0.0.8/upload_machine/utils/para_ctrl/readyaml.py
-drwxr-xr-x   0 moyu       (501) staff       (20)        0 2022-10-09 10:11:37.506721 upload_machine-0.0.8/upload_machine/utils/pathinfo/
--rw-------   0 moyu       (501) staff       (20)        0 2022-10-06 05:53:46.000000 upload_machine-0.0.8/upload_machine/utils/pathinfo/__init__.py
--rw-------   0 moyu       (501) staff       (20)    23713 2022-10-09 10:03:48.000000 upload_machine-0.0.8/upload_machine/utils/pathinfo/pathinfo.py
-drwxr-xr-x   0 moyu       (501) staff       (20)        0 2022-10-09 10:11:37.508038 upload_machine-0.0.8/upload_machine/utils/rss_ctrl/
--rw-------   0 moyu       (501) staff       (20)        0 2022-10-06 05:53:46.000000 upload_machine-0.0.8/upload_machine/utils/rss_ctrl/__init__.py
-drwxr-xr-x   0 moyu       (501) staff       (20)        0 2022-10-09 10:11:37.509213 upload_machine-0.0.8/upload_machine/utils/seed_machine/
--rw-------   0 moyu       (501) staff       (20)        0 2022-10-06 05:53:46.000000 upload_machine-0.0.8/upload_machine/utils/seed_machine/__init__.py
--rw-------   0 moyu       (501) staff       (20)    13441 2022-10-06 08:33:04.000000 upload_machine-0.0.8/upload_machine/utils/seed_machine/seed_machine.py
-drwxr-xr-x   0 moyu       (501) staff       (20)        0 2022-10-09 10:11:37.510372 upload_machine-0.0.8/upload_machine/utils/signer/
--rw-------   0 moyu       (501) staff       (20)        0 2022-10-06 05:53:46.000000 upload_machine-0.0.8/upload_machine/utils/signer/__init__.py
-drwxr-xr-x   0 moyu       (501) staff       (20)        0 2022-10-09 10:11:37.511035 upload_machine-0.0.8/upload_machine/utils/site/
--rw-------   0 moyu       (501) staff       (20)        0 2022-10-06 05:53:46.000000 upload_machine-0.0.8/upload_machine/utils/site/__init__.py
--rw-------   0 moyu       (501) staff       (20)     3273 2022-10-06 08:13:52.000000 upload_machine-0.0.8/upload_machine/utils/site/site.py
-drwxr-xr-x   0 moyu       (501) staff       (20)        0 2022-10-09 10:11:37.524015 upload_machine-0.0.8/upload_machine/utils/uploader/
--rwxr-xr-x   0 moyu       (501) staff       (20)        0 2022-10-06 05:53:46.000000 upload_machine-0.0.8/upload_machine/utils/uploader/__init__.py
--rw-------   0 moyu       (501) staff       (20)     5368 2022-10-08 14:34:31.000000 upload_machine-0.0.8/upload_machine/utils/uploader/audience_upload.py
--rw-------   0 moyu       (501) staff       (20)      998 2022-10-07 18:35:39.000000 upload_machine-0.0.8/upload_machine/utils/uploader/auto_upload.py
--rw-------   0 moyu       (501) staff       (20)     5900 2022-10-08 14:26:24.000000 upload_machine-0.0.8/upload_machine/utils/uploader/carpt_upload.py
--rw-------   0 moyu       (501) staff       (20)     9128 2022-10-08 14:31:44.000000 upload_machine-0.0.8/upload_machine/utils/uploader/hare_upload.py
--rw-------   0 moyu       (501) staff       (20)     8426 2022-10-08 14:26:33.000000 upload_machine-0.0.8/upload_machine/utils/uploader/hdfans_upload.py
--rw-------   0 moyu       (501) staff       (20)     5600 2022-10-08 14:26:36.000000 upload_machine-0.0.8/upload_machine/utils/uploader/hdpt_upload.py
--rw-------   0 moyu       (501) staff       (20)     6831 2022-10-08 14:26:39.000000 upload_machine-0.0.8/upload_machine/utils/uploader/hdsky_upload.py
--rw-------   0 moyu       (501) staff       (20)     8160 2022-10-08 14:26:43.000000 upload_machine-0.0.8/upload_machine/utils/uploader/hhclub_upload.py
--rw-------   0 moyu       (501) staff       (20)    18810 2022-10-08 14:26:59.000000 upload_machine-0.0.8/upload_machine/utils/uploader/lemonhd_upload.py
--rw-------   0 moyu       (501) staff       (20)     6812 2022-10-08 14:27:06.000000 upload_machine-0.0.8/upload_machine/utils/uploader/piggo_upload.py
--rw-------   0 moyu       (501) staff       (20)     4372 2022-10-08 14:27:10.000000 upload_machine-0.0.8/upload_machine/utils/uploader/pter_upload.py
--rw-------   0 moyu       (501) staff       (20)     6847 2022-10-08 14:27:15.000000 upload_machine-0.0.8/upload_machine/utils/uploader/ssd_upload.py
--rw-------   0 moyu       (501) staff       (20)     8673 2022-10-07 18:29:44.000000 upload_machine-0.0.8/upload_machine/utils/uploader/upload_tools.py
--rw-------   0 moyu       (501) staff       (20)     7275 2022-10-08 14:27:19.000000 upload_machine-0.0.8/upload_machine/utils/uploader/wintersakura_upload.py
-drwxr-xr-x   0 moyu       (501) staff       (20)        0 2022-10-09 10:11:37.489609 upload_machine-0.0.8/upload_machine.egg-info/
--rw-------   0 moyu       (501) staff       (20)    16463 2022-10-09 10:11:37.000000 upload_machine-0.0.8/upload_machine.egg-info/PKG-INFO
--rw-------   0 moyu       (501) staff       (20)     2197 2022-10-09 10:11:37.000000 upload_machine-0.0.8/upload_machine.egg-info/SOURCES.txt
--rw-------   0 moyu       (501) staff       (20)        1 2022-10-09 10:11:37.000000 upload_machine-0.0.8/upload_machine.egg-info/dependency_links.txt
--rw-------   0 moyu       (501) staff       (20)       91 2022-10-09 10:11:37.000000 upload_machine-0.0.8/upload_machine.egg-info/entry_points.txt
--rw-------   0 moyu       (501) staff       (20)      115 2022-10-09 10:11:37.000000 upload_machine-0.0.8/upload_machine.egg-info/requires.txt
--rw-------   0 moyu       (501) staff       (20)       15 2022-10-09 10:11:37.000000 upload_machine-0.0.8/upload_machine.egg-info/top_level.txt
+drwxr-xr-x   0 moyu       (501) staff       (20)        0 2023-08-06 09:32:49.446617 upload_machine-0.0.80/
+-rwx------   0 moyu       (501) staff       (20)     1063 2022-10-06 05:53:46.000000 upload_machine-0.0.80/LICENSE
+-rwx------   0 moyu       (501) staff       (20)       37 2022-10-06 08:50:43.000000 upload_machine-0.0.80/MANIFEST.in
+-rw-r--r--   0 moyu       (501) staff       (20)    14608 2023-08-06 09:32:49.442100 upload_machine-0.0.80/PKG-INFO
+-rwxr-xr-x   0 moyu       (501) staff       (20)    14206 2023-08-06 07:01:29.000000 upload_machine-0.0.80/README.md
+-rw-r--r--   0 moyu       (501) staff       (20)       38 2023-08-06 09:32:49.446842 upload_machine-0.0.80/setup.cfg
+-rwx------   0 moyu       (501) staff       (20)     1110 2023-08-06 09:32:42.000000 upload_machine-0.0.80/setup.py
+drwxr-xr-x   0 moyu       (501) staff       (20)        0 2023-08-06 09:32:49.325187 upload_machine-0.0.80/upload_machine/
+-rwx------   0 moyu       (501) staff       (20)        0 2022-10-06 05:53:46.000000 upload_machine-0.0.80/upload_machine/__init__.py
+-rwx------   0 moyu       (501) staff       (20)      241 2022-10-06 08:12:01.000000 upload_machine-0.0.80/upload_machine/basicinfo.yaml
+-rwx------   0 moyu       (501) staff       (20)     2622 2023-01-02 14:54:11.000000 upload_machine-0.0.80/upload_machine/main.py
+drwxr-xr-x   0 moyu       (501) staff       (20)        0 2023-08-06 09:32:49.330597 upload_machine-0.0.80/upload_machine/utils/
+-rwx------   0 moyu       (501) staff       (20)        0 2022-10-06 05:53:46.000000 upload_machine-0.0.80/upload_machine/utils/__init__.py
+drwxr-xr-x   0 moyu       (501) staff       (20)        0 2023-08-06 09:32:49.331379 upload_machine-0.0.80/upload_machine/utils/edittorrent/
+-rwx------   0 moyu       (501) staff       (20)        0 2022-10-06 05:53:46.000000 upload_machine-0.0.80/upload_machine/utils/edittorrent/__init__.py
+-rwx------   0 moyu       (501) staff       (20)     3966 2022-10-06 05:53:46.000000 upload_machine-0.0.80/upload_machine/utils/edittorrent/edittorrent.py
+drwxr-xr-x   0 moyu       (501) staff       (20)        0 2023-08-06 09:32:49.341434 upload_machine-0.0.80/upload_machine/utils/img_upload/
+-rwx------   0 moyu       (501) staff       (20)        0 2022-10-06 05:53:46.000000 upload_machine-0.0.80/upload_machine/utils/img_upload/__init__.py
+-rwx------   0 moyu       (501) staff       (20)     7231 2022-10-06 05:53:46.000000 upload_machine-0.0.80/upload_machine/utils/img_upload/chevereto.py
+-rwx------   0 moyu       (501) staff       (20)     2674 2022-10-06 05:53:46.000000 upload_machine-0.0.80/upload_machine/utils/img_upload/fapping_emp.py
+-rwx------   0 moyu       (501) staff       (20)     4521 2022-10-06 05:53:46.000000 upload_machine-0.0.80/upload_machine/utils/img_upload/imgbox.py
+-rwxr-xr-x   0 moyu       (501) staff       (20)     9014 2023-01-20 04:03:37.000000 upload_machine-0.0.80/upload_machine/utils/img_upload/imgupload.py
+-rwx------   0 moyu       (501) staff       (20)     2510 2022-10-06 05:53:46.000000 upload_machine-0.0.80/upload_machine/utils/img_upload/ptpimg.py
+-rwx------   0 moyu       (501) staff       (20)     1904 2022-11-06 06:50:27.000000 upload_machine-0.0.80/upload_machine/utils/img_upload/redleaves.py
+-rw-r--r--   0 moyu       (501) staff       (20)     2426 2023-01-20 04:03:37.000000 upload_machine-0.0.80/upload_machine/utils/img_upload/sharkimg.py
+-rwx------   0 moyu       (501) staff       (20)     2875 2022-10-06 05:53:46.000000 upload_machine-0.0.80/upload_machine/utils/img_upload/smms.py
+drwxr-xr-x   0 moyu       (501) staff       (20)        0 2023-08-06 09:32:49.348378 upload_machine-0.0.80/upload_machine/utils/mediafile/
+-rwx------   0 moyu       (501) staff       (20)        0 2022-10-06 05:53:46.000000 upload_machine-0.0.80/upload_machine/utils/mediafile/__init__.py
+-rwx------   0 moyu       (501) staff       (20)    17212 2022-10-06 05:53:46.000000 upload_machine-0.0.80/upload_machine/utils/mediafile/douban_book.py
+-rwx------   0 moyu       (501) staff       (20)    24814 2022-10-06 05:53:46.000000 upload_machine-0.0.80/upload_machine/utils/mediafile/douban_movie.py
+-rwx------   0 moyu       (501) staff       (20)     6861 2022-10-06 08:34:29.000000 upload_machine-0.0.80/upload_machine/utils/mediafile/doubaninfo.py
+-rw-r--r--   0 moyu       (501) staff       (20)     2418 2023-01-03 18:41:08.000000 upload_machine-0.0.80/upload_machine/utils/mediafile/maketorrent.py
+-rwx------   0 moyu       (501) staff       (20)    64920 2023-08-06 09:31:08.000000 upload_machine-0.0.80/upload_machine/utils/mediafile/mediafile.py
+drwxr-xr-x   0 moyu       (501) staff       (20)        0 2023-08-06 09:32:49.354495 upload_machine-0.0.80/upload_machine/utils/para_ctrl/
+-rwx------   0 moyu       (501) staff       (20)      218 2022-10-06 08:34:43.000000 upload_machine-0.0.80/upload_machine/utils/para_ctrl/__init__.py
+-rwx------   0 moyu       (501) staff       (20)     6779 2022-10-09 10:10:39.000000 upload_machine-0.0.80/upload_machine/utils/para_ctrl/para_ctrl.py
+-rwxr-xr-x   0 moyu       (501) staff       (20)     2154 2023-01-20 04:03:37.000000 upload_machine-0.0.80/upload_machine/utils/para_ctrl/readargs.py
+-rwx------   0 moyu       (501) staff       (20)     1901 2023-01-06 10:01:44.000000 upload_machine-0.0.80/upload_machine/utils/para_ctrl/readyaml.py
+drwxr-xr-x   0 moyu       (501) staff       (20)        0 2023-08-06 09:32:49.356342 upload_machine-0.0.80/upload_machine/utils/pathinfo/
+-rwx------   0 moyu       (501) staff       (20)        0 2022-10-06 05:53:46.000000 upload_machine-0.0.80/upload_machine/utils/pathinfo/__init__.py
+-rwx------   0 moyu       (501) staff       (20)    26791 2023-08-06 07:37:26.000000 upload_machine-0.0.80/upload_machine/utils/pathinfo/pathinfo.py
+drwxr-xr-x   0 moyu       (501) staff       (20)        0 2023-08-06 09:32:49.358236 upload_machine-0.0.80/upload_machine/utils/rss_ctrl/
+-rwx------   0 moyu       (501) staff       (20)        0 2022-10-06 05:53:46.000000 upload_machine-0.0.80/upload_machine/utils/rss_ctrl/__init__.py
+drwxr-xr-x   0 moyu       (501) staff       (20)        0 2023-08-06 09:32:49.360288 upload_machine-0.0.80/upload_machine/utils/seed_machine/
+-rwx------   0 moyu       (501) staff       (20)        0 2022-10-06 05:53:46.000000 upload_machine-0.0.80/upload_machine/utils/seed_machine/__init__.py
+-rwx------   0 moyu       (501) staff       (20)    21911 2023-08-06 08:04:07.000000 upload_machine-0.0.80/upload_machine/utils/seed_machine/seed_machine.py
+drwxr-xr-x   0 moyu       (501) staff       (20)        0 2023-08-06 09:32:49.361836 upload_machine-0.0.80/upload_machine/utils/signer/
+-rwx------   0 moyu       (501) staff       (20)        0 2022-10-06 05:53:46.000000 upload_machine-0.0.80/upload_machine/utils/signer/__init__.py
+drwxr-xr-x   0 moyu       (501) staff       (20)        0 2023-08-06 09:32:49.362722 upload_machine-0.0.80/upload_machine/utils/site/
+-rwx------   0 moyu       (501) staff       (20)        0 2022-10-06 05:53:46.000000 upload_machine-0.0.80/upload_machine/utils/site/__init__.py
+-rwx------   0 moyu       (501) staff       (20)     4302 2023-01-02 15:05:32.000000 upload_machine-0.0.80/upload_machine/utils/site/site.py
+drwxr-xr-x   0 moyu       (501) staff       (20)        0 2023-08-06 09:32:49.428348 upload_machine-0.0.80/upload_machine/utils/uploader/
+-rwx------   0 moyu       (501) staff       (20)        0 2022-10-06 05:53:46.000000 upload_machine-0.0.80/upload_machine/utils/uploader/__init__.py
+-rwx------   0 moyu       (501) staff       (20)     5800 2023-01-08 11:40:16.000000 upload_machine-0.0.80/upload_machine/utils/uploader/audience_upload.py
+-rwx------   0 moyu       (501) staff       (20)     1706 2023-08-06 06:58:29.000000 upload_machine-0.0.80/upload_machine/utils/uploader/auto_upload.py
+-rwx------   0 moyu       (501) staff       (20)     7397 2023-01-05 04:08:25.000000 upload_machine-0.0.80/upload_machine/utils/uploader/carpt_upload.py
+-rw-r--r--   0 moyu       (501) staff       (20)     8198 2023-08-05 18:44:07.000000 upload_machine-0.0.80/upload_machine/utils/uploader/dajiao_upload.py
+-rwx------   0 moyu       (501) staff       (20)    10309 2023-01-06 12:18:37.000000 upload_machine-0.0.80/upload_machine/utils/uploader/hares_upload.py
+-rwx------   0 moyu       (501) staff       (20)     8922 2023-01-08 11:39:46.000000 upload_machine-0.0.80/upload_machine/utils/uploader/hdfans_upload.py
+-rwx------   0 moyu       (501) staff       (20)     6032 2023-01-05 04:08:36.000000 upload_machine-0.0.80/upload_machine/utils/uploader/hdpt_upload.py
+-rwx------   0 moyu       (501) staff       (20)     7263 2023-01-06 12:18:50.000000 upload_machine-0.0.80/upload_machine/utils/uploader/hdsky_upload.py
+-rwx------   0 moyu       (501) staff       (20)     8357 2023-08-06 09:24:01.000000 upload_machine-0.0.80/upload_machine/utils/uploader/hdvideo_upload.py
+-rwx------   0 moyu       (501) staff       (20)     9220 2023-01-06 12:18:58.000000 upload_machine-0.0.80/upload_machine/utils/uploader/hhclub_upload.py
+-rwx------   0 moyu       (501) staff       (20)     8642 2023-01-06 12:19:01.000000 upload_machine-0.0.80/upload_machine/utils/uploader/ihdbits_upload.py
+-rwx------   0 moyu       (501) staff       (20)    19758 2023-01-11 18:07:47.000000 upload_machine-0.0.80/upload_machine/utils/uploader/lemonhd_upload.py
+-rwx------   0 moyu       (501) staff       (20)     7123 2023-01-06 12:19:07.000000 upload_machine-0.0.80/upload_machine/utils/uploader/mteam_upload.py
+-rw-r--r--   0 moyu       (501) staff       (20)     8728 2023-08-05 18:44:22.000000 upload_machine-0.0.80/upload_machine/utils/uploader/pandapt_upload.py
+-rwx------   0 moyu       (501) staff       (20)     7926 2023-02-12 10:09:06.000000 upload_machine-0.0.80/upload_machine/utils/uploader/piggo_upload.py
+-rwx------   0 moyu       (501) staff       (20)     4804 2023-01-05 04:09:08.000000 upload_machine-0.0.80/upload_machine/utils/uploader/pter_upload.py
+-rwx------   0 moyu       (501) staff       (20)     8888 2023-05-14 16:45:46.000000 upload_machine-0.0.80/upload_machine/utils/uploader/redleaves_upload.py
+-rw-r--r--   0 moyu       (501) staff       (20)     8379 2023-08-06 09:32:35.000000 upload_machine-0.0.80/upload_machine/utils/uploader/rousi_upload.py
+-rwxr-xr-x   0 moyu       (501) staff       (20)     8322 2023-02-28 11:45:25.000000 upload_machine-0.0.80/upload_machine/utils/uploader/sharkpt_upload.py
+-rwx------   0 moyu       (501) staff       (20)     7308 2023-01-11 18:11:31.000000 upload_machine-0.0.80/upload_machine/utils/uploader/ssd_upload.py
+-rwx------   0 moyu       (501) staff       (20)    10649 2023-01-06 04:48:18.000000 upload_machine-0.0.80/upload_machine/utils/uploader/upload_tools.py
+-rwx------   0 moyu       (501) staff       (20)     7707 2023-01-06 12:19:20.000000 upload_machine-0.0.80/upload_machine/utils/uploader/wintersakura_upload.py
+-rwx------   0 moyu       (501) staff       (20)    10462 2023-01-06 17:28:21.000000 upload_machine-0.0.80/upload_machine/utils/uploader/zhuque_upload.py
+-rwx------   0 moyu       (501) staff       (20)     7858 2023-01-08 11:39:12.000000 upload_machine-0.0.80/upload_machine/utils/uploader/zmpt_upload.py
+drwxr-xr-x   0 moyu       (501) staff       (20)        0 2023-08-06 09:32:49.330123 upload_machine-0.0.80/upload_machine.egg-info/
+-rwx------   0 moyu       (501) staff       (20)    14608 2023-08-06 09:32:47.000000 upload_machine-0.0.80/upload_machine.egg-info/PKG-INFO
+-rwx------   0 moyu       (501) staff       (20)     2814 2023-08-06 09:32:49.000000 upload_machine-0.0.80/upload_machine.egg-info/SOURCES.txt
+-rwx------   0 moyu       (501) staff       (20)        1 2023-08-06 09:32:48.000000 upload_machine-0.0.80/upload_machine.egg-info/dependency_links.txt
+-rwx------   0 moyu       (501) staff       (20)       90 2023-08-06 09:32:48.000000 upload_machine-0.0.80/upload_machine.egg-info/entry_points.txt
+-rwx------   0 moyu       (501) staff       (20)      137 2023-08-06 09:32:48.000000 upload_machine-0.0.80/upload_machine.egg-info/requires.txt
+-rwx------   0 moyu       (501) staff       (20)       15 2023-08-06 09:32:48.000000 upload_machine-0.0.80/upload_machine.egg-info/top_level.txt
```

### Comparing `upload_machine-0.0.8/README.md` & `upload_machine-0.0.80/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -21,15 +21,39 @@
 - 无需安装Chrome浏览器以及相关插件
 - 无需原来的Json格式的cookie文件改为在配置文件 `au.yaml`中填写F12获取的cookie
 - 更轻量，更快速，更少出错的可能
 - 但是无法浏览模拟发种过程
 - 无法在发种前暂停自行修改信息
 
 ## 更新说明
-
+- 20230806 增加对站点Rousi的支持
+- 20230806 增加对pandapt和dajiao站点的支持，并更新了hdvideo站点发布
+- 20230112 piggo发布更新，sharkpt merge了官组相关设置
+- 20230108 修复了无数个由于上一次更新带来的bug
+- 20221205 新增将未发布资源打包发布的功能，设置方法是将配置文件`au.yaml`中`path`中的`collection`参数设置为2
+- 20221205 对于zhuque站点发种失败，新增返回错误信息
+- 20221205 针对sharkpt的种子标题以及mediainfo的更新做了适配
+- 20221204 更改了制作种子的底层逻辑算法以改善对于Windows下制作种子的问题，同时增加制种进度条
+- 20221202 增加对于Zhuque的支持,发布合集后会把合集内的集数都算做已发布
+- 20221202 增加对于SharkPT的支持
+- 20221219 更正“内嵌字幕”为“内封字幕”
+- 20221202 增加对于MTeam的支持
+- 20221202 随着carpt升级更改carpt发种部分代码以顺利发种，ihdbits添加音频编码。
+- 20221029 增加对红叶(redleaves)站点以及图床的支持
+- 20221029 副标题第EXX集取消字符“E”
+- 20221029 如果配置文件为空时自动使用备份配置文件文件，修复DoubanInfo了抓取imdb分数超时的bug
+- 20221028 增加对ihdbits的支持
+- 20221028 增加对zmpt，hdvideo的支持,增加对于粤语的判断.修改了配置文件部分描述，使得配置变得更加简单。详细参数说明参考[au_example.yaml](https://github.com/dongshuyan/Upload_Machine/blob/master/au_example.yaml)
+- 20221012 增加了自动生成0day文件带有中文标题的功能,详细参数说明参考[au_example.yaml](https://github.com/dongshuyan/Upload_Machine/blob/master/au_example.yaml)中`basic` 中 `new_folder`参数说明
+- 20221012 修改了`zeroday_name`可能引起的bug
+- 20221011 支持了mediainfo模板文件，详细参数说明参考[au_example.yaml](https://github.com/dongshuyan/Upload_Machine/blob/master/au_example.yaml)中`site info` 中 `站点` 中 `mediainfo_template_file`参数说明
+- 20221010 更改副标题样式为标准样式，对于多语言音轨在主标题添加类似 2Audio的内容
+- 20221010 hare改为hares
+- 20221010 新增自定义配置“副标题”，“自定义截图”，“简介头信息”，“简介尾信息”等配置参数
+- 20221010 修复imdb链接只记录了id的bug
 - 20221008 豆瓣简介的获取改使用doubaninfo的接口
 - 20221008 增加对hdpt,carpt,hdfans,hares和wintersakura的支持
 - 20221007 增加对pter，hhclub和LemonHD的支持
 - 20221006 增加对audience和ssd的支持
 - 20221006 增加对hdsky的支持
 
 ## 功能说明
@@ -44,27 +68,26 @@
 
 全平台支持了以下功能:
 
 - 根据配置文件分析待发布资源的中英文名
 - 根据配置文件分析已经发布的资源并自动找到未发布的资源
 - 可选是否在资源外层套一个0day名字的文件夹
 - 大量参数可以自动抓取也可以自己配置，包括且不限于 视频格式，音频格式，字幕信息，音轨信息等
-- 将未发布的资源有序发布
+- 将未发布的资源有序 单集/按照合集 发布
 - 自动获取待发布资源的豆瓣链接/动漫资源的bgm链接
 - 自动获取待发布资源的豆瓣简介
 - 自动获取待发布资源的截图并上传到图床获取bbcode
 - 自动获取待发布资源的mediainfo信息
 - 自动制作种子
-- 根据上述信息自动发布到各个站点（分集发布/打包发布）
+- 根据上述信息自动发布到各个站点（分集发布/整体打包发布/未发布过的分集打包发布）
 - 自动获取下载链接并传递给Qbittorrent自动做种
 - 自动记录发布资源信息生成excel表格(csv文件)
 - 自动统计目前已发布的总量(可以用来统计每月发种数量)
 
-目前支持的平台:
-
+目前支持所有运行python环境的平台，包括但不限于:
 - MacOS
 - Windows
 - Linux
 
 目前支持的资源类型:
 
 - 动漫
@@ -80,22 +103,34 @@
 - pter (猫站)
 - hhclub (憨憨)
 - lemonhd (柠檬)
 - hdpt (明教)
 - wintersakura (冬樱)
 - carpt (车站)
 - hdfans (红豆饭)
-- hare (白兔)
+- hares (白兔)
+- zmpt (织梦)
+- hdvideo(高清视频)
+- iHDBits(爱好多)
+- redleaves(红叶)
+- mteam(馒头)
+- sharkpt(鲨鱼)
+- zhuque(朱雀)
+- dajiao(打胶)
+- pandapt(熊猫)
+
 
 正在适配的站点(排名不分先后):
 
-- MT
+- HDTime
+- Rousi
 
 Todolist:
-
+- 自动文件改名
+- 配置文件详细教程
 - GUI（有考虑，需要学）
 - 自定义站点（需要考虑做不做和怎么做）
 
 如果有新的站点/资源类型等需求,可以加入QQ群交流(735803201)
 
 ## 安装Upload_Machine自动发种机
 
@@ -117,57 +152,49 @@
 以下几个插件的安装包可以去通过下面官方途径下载，也可以前往[Install文件夹](https://github.com/dongshuyan/Auto_Upload/blob/master/install)获取 或者 前往交流群的群文件获取。3.安装 `ffmpeg`，并确认安装正确:
 
 - 下载安装 `ffmpeg` & `ffprobe`：https://github.com/BtbN/FFmpeg-Builds/releases
 - 将解压后的 `ffmpeg`文件夹移动到一个相对稳定的文件夹,比如 `D:\Program Files\`
 - 将上一步 `ffmpeg\bin`文件夹路径添加到系统PATH我的电脑【右击】 -> 选择 属性 -> 高级系统设置 -> 高级 -> 环境变量  -> 系统变量里面找到'Path',点击编辑 -> 新建 -> 将上一步 `ffmpeg\bin`文件夹路径路径粘贴进去 -> 确定 --> 确定 … 保存即可。一般也是 不需要重启
 - 在PowerShell确认ffmpeg和ffprobe安装成功
 
-4.安装 `mktorrent`，并确认安装正确:
-
-- 根据自己电脑下载[64位安装包](https://github.com/q3aql/mktorrent-win/releases/download/v1.1-2/mktorrent-1.1-win-64bit-build2.7z)或者[32位安装包](https://github.com/q3aql/mktorrent-win/releases/download/v1.1-2/mktorrent-1.1-win-32bit-build2.7z)
-- 使用[7-zip](http://www.7-zip.org/) or [Winrar](http://www.rarlab.com/)解压文件.
-- 将 `mktorrent`文件夹移动到一个相对稳定的文件夹,比如 `D:\Program Files\`
-- 将上一步 `mktorrent\bin`文件夹路径添加到系统PATH
-  我的电脑【右击】 -> 选择 属性 -> 高级系统设置 -> 高级 -> 环境变量  -> 系统变量里面找到'Path',点击编辑 -> 新建 -> 将上一步 `mktorrent\bin`文件夹路径路径粘贴进去 -> 确定 --> 确定 … 保存即可。一般也是 不需要重启
-
-5.安装 `mediainfo`，并确认安装正确
+4.安装 `mediainfo`，并确认安装正确
 
 - 下载[mediainfo-cli](https://mediaarea.net/download/binary/mediainfo/22.06/MediaInfo_CLI_22.06_Windows_x64.zip)：https://mediaarea.net/en/MediaInfo/Download/Windows
 - 解压zip文件并解压后的 `Mediainfo_CLIxxx`文件夹移动到一个相对稳定的位置
 - 将上一步 `Mediainfo_CLIxxx`文件夹路径添加到系统PATH我的电脑【右击】 -> 选择 属性 -> 高级系统设置 -> 高级 -> 环境变量  -> 系统变量里面找到'Path',点击编辑 -> 新建 -> 将上一步 `Mediainfo_CLIxxx`文件夹路径粘贴进去 -> 确定 --> 确定 … 保存即可。一般也是 不需要重启。
 - 在PowerShell确认 `mediainfo`安装成功
 
 ```bash
 mediainfo -h
 ```
 
-6.安装 `Upload_Machine`，在以管理员身份打开 `Windows PowerShell`中输入:
+5.安装 `Upload_Machine`，在以管理员身份打开 `Windows PowerShell`中输入:
 
 ```bash
-python3 -m pip install upload_machine  -i https://pypi.tuna.tsinghua.edu.cn/simple/
+pip install upload_machine
 upload_machine -h
 ```
 
 如果上述命令没反应或者报错可以尝试下面这个：
 
 ```bash
-pip install upload_machine  -i https://pypi.tuna.tsinghua.edu.cn/simple/
+pip3 install upload_machine
 upload_machine -h
 ```
 
 7.更新 `Upload_Machine`，在 `Windows PowerShell`中输入:
 
 ```bash
-python3 -m pip install --upgrade upload_machine  -i https://pypi.tuna.tsinghua.edu.cn/simple/
+pip install --upgrade upload_machine
 ```
 
 如果上述命令没反应或者报错可以尝试下面这个：
 
 ```bash
-pip install --upgrade upload_machine  -i https://pypi.tuna.tsinghua.edu.cn/simple/
+pip3 install --upgrade upload_machine 
 ```
 
 ### Linux
 
 0.升级 `python`至 `3.7.0`版本以上，建议 `3.9.0`
 如果有 `_ssl`或者 `_ctypes`找不到，也可以试试按照下面步骤重新安装python3
 
@@ -204,35 +231,35 @@
 sudo python3 -m pip install --upgrade pip
 sudo apt-get install python3-pip ffmpeg mediainfo mktorrent
 ```
 
 3.安装 `Upload_Machine`
 
 ```bash
-python3 -m pip install upload_machine -i https://pypi.tuna.tsinghua.edu.cn/simple/
+pip install upload_machine
 upload_machine -h
 ```
 
 如果上述命令没反应或者报错可以尝试下面这个：
 
 ```bash
-pip install upload_machine -i https://pypi.tuna.tsinghua.edu.cn/simple/
+pip3 install upload_machine
 upload_machine -h
 ```
 
 4.更新 `Upload_Machine`，，在 `Terminal.app`中输入:
 
 ```bash
-python3 -m pip install --upgrade upload_machine -i https://pypi.tuna.tsinghua.edu.cn/simple/
+pip install --upgrade upload_machine
 ```
 
 如果上述命令没反应或者报错可以尝试下面这个：
 
 ```bash
-pip install --upgrade upload_machine -i https://pypi.tuna.tsinghua.edu.cn/simple/
+pip3 install --upgrade upload_machine
 ```
 
 ### MacOS(已测试成功)
 
 1.安装 `Homebrew`，在Termial.app中输入:
 
 ```bash
@@ -246,35 +273,35 @@
 ffmpeg -version
 mediainfo --version
 ```
 
 3.安装 `Upload_Machine`，在 `Terminal.app`中输入:
 
 ```bash
-python3 -m pip install upload_machine -i https://pypi.tuna.tsinghua.edu.cn/simple/
+pip install upload_machine
 upload_machine -h
 ```
 
 如果上述命令没反应或者报错可以尝试下面这个：
 
 ```bash
-pip install upload_machine -i https://pypi.tuna.tsinghua.edu.cn/simple/
+pip3 install upload_machine
 upload_machine -h
 ```
 
 5.更新 `Upload_Machine`，，在 `Terminal.app`中输入:
 
 ```bash
-python3 -m pip install --upgrade upload_machine -i https://pypi.tuna.tsinghua.edu.cn/simple/
+pip install --upgrade upload_machine
 ```
 
 如果上述命令没反应或者报错可以尝试下面这个：
 
 ```bash
-pip install --upgrade upload_machine -i https://pypi.tuna.tsinghua.edu.cn/simple/
+pip3 install --upgrade upload_machine
 ```
 
 ## 配置环境&文件
 
 ### 1.本地新建一个工作目录
 
 例如路径为:/Users/Desktop/upload_machine
@@ -328,14 +355,15 @@
 
 - ptpimg
 - picgo
 - chd
 - imgbox
 - pter
 - smms
+- sharkimg
 
 ### 3.获取豆瓣信息
 
 ```bash
 upload_machine -yp '工作目录/au.yaml' -di -du '豆瓣链接'
 ```
 
@@ -355,14 +383,15 @@
 
 - ptpimg
 - picgo
 - chd
 - imgbox
 - pter
 - smms
+- sharkimg
 
 图片格式(可以不填，默认'img'):
 
 - img 图片原始链接
 - bbcode BBcode格式链接
 
 截图数量(可以不填，默认3张)
@@ -381,15 +410,15 @@
 
 ## 交流群
 
 群号:735803201
 
 ## Reference
 
-[Differential 差速器](https://github.com/LeiShi1313/Differential)  (复制了上传图床部分代码)
-[Differential差速器使用教程](https://leishi.io/blog/posts/2021-12/Differential/)  (Upload_Machine安装教程主要参考本文)
-[mktorrent-win-builds](https://github.com/q3aql/mktorrent-win-builds)
-[MKTORRENT WIN下命令行制作种子](https://blog.acesheep.com/index.php/archives/551/)
-[linux 安装 Chrome](https://www.cnblogs.com/ivantang/p/6290729.html)
-[windows10 环境变量设置](https://blog.csdn.net/palmer_kai/article/details/80588594)
-[Linux Ubuntu系统升级Python3版本至Python3.9版本步骤](https://blog.csdn.net/u012080686/article/details/112600252)
-[PYTorrent](https://github.com/ndroi/pytorrent)
+[Differential 差速器](https://github.com/LeiShi1313/Differential)  (复制了上传图床部分代码)  
+[Differential差速器使用教程](https://leishi.io/blog/posts/2021-12/Differential/)  (Upload_Machine安装教程主要参考本文)  
+[mktorrent-win-builds](https://github.com/q3aql/mktorrent-win-builds)  
+[MKTORRENT WIN下命令行制作种子](https://blog.acesheep.com/index.php/archives/551/)  
+[linux 安装 Chrome](https://www.cnblogs.com/ivantang/p/6290729.html)  
+[windows10 环境变量设置](https://blog.csdn.net/palmer_kai/article/details/80588594)  
+[Linux Ubuntu系统升级Python3版本至Python3.9版本步骤](https://blog.csdn.net/u012080686/article/details/112600252)  
+[PYTorrent](https://github.com/ndroi/pytorrent)
```

### Comparing `upload_machine-0.0.8/setup.py` & `upload_machine-0.0.80/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import io
 
 setup(
     name = "upload_machine",     
-    version = "0.0.8", 
+    version = "0.0.80", 
     keywords = ["pip", "autoupload","auto","upload","PT","private tracker"],            
     description = "Upload local resources to PT trackers automatically.",    
     long_description=io.open("README.md", "r", encoding='utf-8').read(),
     long_description_content_type="text/markdown",
     license = "MIT Licence",    
 
     entry_points = {
@@ -22,10 +22,10 @@
     author_email = "ssauterne@qq.com",
 
     packages = find_packages(),
     include_package_data = True,
     exclude_package_data = {'': ['__pycache__']},
 
     platforms = "any",
-    python_requires = '>=3.9.0',
-    install_requires = ["loguru","pathlib","typing","lxml","pyyaml","requests","bs4","datetime","qbittorrent-api","function_controler","doubaninfo","cloudscraper"]
+    python_requires = '>=3',
+    install_requires = ["loguru","pathlib","typing","lxml","pyyaml","requests","bs4","datetime","qbittorrent-api","function_controler","doubaninfo >= 0.0.13","cloudscraper","progress","torf"]
 )
```

### Comparing `upload_machine-0.0.8/upload_machine/main.py` & `upload_machine-0.0.80/upload_machine/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,16 @@
     logger.info("欢迎使用sauterne开发的Upload_Machine\n")
     yamlinfo=read_para()
     #设置路径，如果有下载文件都下载到screenshot_path
     os.chdir(yamlinfo['basic']['screenshot_path'])
 
     if 'basic' in yamlinfo and 'log' in yamlinfo['basic'] and yamlinfo['basic']['log']!=None:
         log = yamlinfo['basic']['log']
+        if os.path.exists(log):
+            os.remove(log)
         logger.add(log, level="TRACE", backtrace=True, diagnose=True)
 
     if yamlinfo['mod']=='img_upload':
         logger.info('正在使用上传图床模式')
         res=img_upload(imgdata=yamlinfo['image hosting'],imglist=yamlinfo['imgfilelist'],host=yamlinfo['img_host'],form=yamlinfo['img_form'])
         logger.info('成功上传图床')
         print(res)
```

### Comparing `upload_machine-0.0.8/upload_machine/utils/edittorrent/edittorrent.py` & `upload_machine-0.0.80/upload_machine/utils/edittorrent/edittorrent.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.8/upload_machine/utils/img_upload/chevereto.py` & `upload_machine-0.0.80/upload_machine/utils/img_upload/chevereto.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.8/upload_machine/utils/img_upload/fapping_emp.py` & `upload_machine-0.0.80/upload_machine/utils/img_upload/fapping_emp.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.8/upload_machine/utils/img_upload/imgbox.py` & `upload_machine-0.0.80/upload_machine/utils/img_upload/imgbox.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.8/upload_machine/utils/img_upload/imgupload.py` & `upload_machine-0.0.80/upload_machine/utils/img_upload/imgupload.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import os
 from loguru import logger
 from upload_machine.utils.img_upload.chevereto import chevereto_api_upload_files,chevereto_cookie_upload_files
 from upload_machine.utils.img_upload.ptpimg import ptpimg_upload_files
 from upload_machine.utils.img_upload.smms import smms_upload_files
 from upload_machine.utils.img_upload.fapping_emp import femp_upload_files
 from upload_machine.utils.img_upload.imgbox import imgbox_upload_files
+from upload_machine.utils.img_upload.redleaves import redleaves_upload_files
+from upload_machine.utils.img_upload.sharkimg import sharkimg_upload_files
 
 
 def existitem(imgdata,item):
     if item in imgdata and not(imgdata[item]=='') and not imgdata[item]==None:
         return True
     return False
 
 def createimgdict(imgdata):
     imgdict=dict()
-    imghostlist=['ptpimg','picgo','smms','pter','emp','femp','imgbox','chd','freeimage']
+    imghostlist=['ptpimg','picgo','smms','pter','emp','femp','imgbox','chd','freeimage','redleaves','sharkimg']
     for item in imghostlist:
         imgdict[item]=False
     if existitem(imgdata,'ptpimg') and existitem(imgdata['ptpimg'],'apikey'):
         imgdict['ptpimg']=True
     if existitem(imgdata,'picgo') and existitem(imgdata['picgo'],'apikey') and existitem(imgdata['picgo'],'url') :
         imgdict['picgo']=True
     if existitem(imgdata,'smms') and existitem(imgdata['smms'],'apikey'):
@@ -27,15 +29,18 @@
         imgdict['pter']=True
     if existitem(imgdata,'emp')  and existitem(imgdata['emp'],'url') and existitem(imgdata['emp'],'cookie') :
         imgdict['emp']=True
     if existitem(imgdata,'chd')  and existitem(imgdata['chd'],'url') and existitem(imgdata['chd'],'cookie') :
         imgdict['chd']=True
     if existitem(imgdata,'freeimage')  and existitem(imgdata['freeimage'],'url') and existitem(imgdata['freeimage'],'cookie') :
         imgdict['freeimage']=True
+    if existitem(imgdata, 'sharkimg') and existitem(imgdata['sharkimg'], 'token'):
+        imgdict['sharkimg'] = True
     imgdict['femp']=True
+    imgdict['redleaves']=True
     imgdict['imgbox']=True
     listnum=1
     seq=[]
     while (existitem(imgdata['seq'],(listnum))):
         seq.append(imgdata['seq'][(listnum)])
         listnum=listnum+1
     return imgdata,imgdict,seq
@@ -138,14 +143,24 @@
         if imgdict[host]==True:
             res=chevereto_cookie_upload_files(imgpaths=imglist,url=imgdata[host]['url'].strip('/'), cookie=imgdata[host]['cookie'], form=form)
         else:
             success=False
             logger.warning('图床'+host+'配置信息缺失')
         if res=='':
             success=False
+    elif 'redleaves' in host.lower():
+        host='redleaves'
+        logger.info('正在尝试使用'+host+'上传图片,请稍等...')
+        if imgdict[host]==True:
+            res=redleaves_upload_files(imgpaths=imglist, form=form)
+        else:
+            success=False
+            logger.warning('图床'+host+'配置信息缺失')
+        if res=='':
+            success=False
     elif 'chevereto_api' in host.lower():
         host='chevereto_api'
         logger.info('正在尝试使用'+host+'上传图片,请稍等...')
         if not (chevereto_url=='' or chevereto_apikey==''):
             res=chevereto_api_upload_files(imgpaths=imglist,url=chevereto_url,api_key=chevereto_apikey,form=form)
         else:
             success=False
@@ -158,14 +173,24 @@
         if not (chevereto_url=='' or chevereto_cookie==''):
             res=chevereto_cookie_upload_files(imgpaths=imglist,url=chevereto_url, cookie=chevereto_cookie, form=form)
         else:
             success=False
             logger.warning('图床'+host+'配置信息缺失')
         if res=='':
             success=False
+    elif 'sharkimg'in host.lower():
+        host='sharkimg'
+        logger.info('正在尝试使用'+host+'上传图片,请稍等...')
+        if imgdict[host]==True:
+            res=sharkimg_upload_files(imgpaths=imglist,token=imgdata[host]['token'],form=form)
+        else:
+            success=False
+            logger.warning('图床'+host+'配置信息缺失')
+        if res=='':
+            success=False
     else:
         host='ptpimg'
         logger.info('未找到该图床，正在尝试使用'+host+'上传图片,请稍等...')
         if imgdict[host]==True:
             res=ptpimg_upload_files(imgpaths=imglist,api_key=imgdata[host]['apikey'],form=form)
         else:
             success=False
```

### Comparing `upload_machine-0.0.8/upload_machine/utils/img_upload/ptpimg.py` & `upload_machine-0.0.80/upload_machine/utils/img_upload/ptpimg.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.8/upload_machine/utils/img_upload/smms.py` & `upload_machine-0.0.80/upload_machine/utils/img_upload/smms.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.8/upload_machine/utils/mediafile/douban_book.py` & `upload_machine-0.0.80/upload_machine/utils/mediafile/douban_book.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.8/upload_machine/utils/mediafile/douban_movie.py` & `upload_machine-0.0.80/upload_machine/utils/mediafile/douban_movie.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.8/upload_machine/utils/mediafile/doubaninfo.py` & `upload_machine-0.0.80/upload_machine/utils/mediafile/doubaninfo.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.8/upload_machine/utils/mediafile/mediafile.py` & `upload_machine-0.0.80/upload_machine/utils/mediafile/mediafile.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 from upload_machine.utils.pathinfo.pathinfo import findnum
+from upload_machine.utils.pathinfo.pathinfo import findeps
 import os
 from loguru import logger
 import time
 import requests
 import re
 import json
 import sys
 from upload_machine.utils.img_upload.imgupload import img_upload
 from upload_machine.utils.edittorrent.edittorrent import *
 from shutil import move
 from doubaninfo.doubaninfo import getdoubaninfo
+from progress.bar import IncrementalBar
+from torf import Torrent
+from pathlib import Path
 
 def deletetorrent(delpath=''):
     if delpath=='':
         delpath = os.path.dirname(os.path.abspath(__file__))
     logger.info('正在清除此文件夹下所有种子文件:'+delpath)
     ls = os.listdir(delpath)
     for i in ls:
@@ -88,15 +92,18 @@
             if os.path.exists(torrentname):
                 logger.info('已存在种子文件，正在删除'+torrentname)
                 try:
                     os.remove(torrentname)
                 except Exception as r:
                     logger.error('删除种子发生错误: %s' %(r))
             res=os.popen(order)
+            temp=res
             res=res.buffer.read().decode('utf-8')
+            temp.close()
+            del(temp)
             if os.path.exists(torrentname):
                 filesize=os.path.getsize(torrentname)
             else:
                 filesize=0
 
         os.rename(new_filepath,filepath)
         t=Torrent()
@@ -128,32 +135,45 @@
                     except Exception as r:
                         logger.error('删除种子发生错误: %s' %(r))
                 logger.info(order)
             logger.info('第'+str(trytime)+'次制作种子:')
 
             #os.system(order)
             res=os.popen(order)
+            temp=res
             res=res.buffer.read().decode('utf-8')
-            if os.path.exists(torrentname):
-                filesize=os.path.getsize(torrentname)
-            else:
-                filesize=0
+            temp.close()
+            del(temp)
+            filesizetime=0
+            while filesize==0:
+                filesizetime=filesizetime+1
+                if filesizetime>5:
+                    break
+                if os.path.exists(torrentname):
+                    filesize=os.path.getsize(torrentname)
+                else:
+                    filesize=0
+                if filesize==0:
+                    time.sleep(1)
+            
 
         os.rename(new_filepath,filepath)
         t=Torrent()
         t.load(torrentname)
         t.data[b"info"][b"name"]=str2bytes(os.path.basename(filepath))
         t.dump(torrentname)
 
 
 
     logger.info('已完成制作种子'+torrentname)
     os.chdir(cwd)
 
-def mktorrent(filepath,torrentname,tracker="https://announce.leaguehd.com/announce.php"):
+
+
+def mktorrent_old(filepath,torrentname,tracker="https://announce.leaguehd.com/announce.php"):
     if 'win32' in sys.platform:
         mktorrent_win(filepath,torrentname,tracker)
         return 
     if os.path.isdir(filepath):
         logger.info('检测到路径制种，将先删除掉路径里面所有种子文件(torrent后缀)以及隐藏文件（.开头的文件）...')
         deletetorrent(filepath) 
     deletetorrent(os.path.dirname(torrentname))
@@ -169,16 +189,15 @@
             os.rename(torrentname,torrentname+'temp')
             os.remove(torrentname+'temp')
         except Exception as r:
             logger.warning('删除种子发生错误: %s' %(r))
 
     logger.info('正在对下面路径制作种子:'+filepath)
     #order='mktorrent -v -p -f -l 24 -c "Made by Auto_Upload" -a '+tracker+' -o \"'+torrentname+ '\" \"'+filepath+'\"'+' > /dev/null'
-    order='mktorrent -v -p -l 24 -c "Made by Auto_Upload" -a '+tracker+' -o \"'+torrentname+ '\" \"'+filepath+'\"'
-        
+    order='mktorrent -v -p -l 24 -c "Made by Upload_Machine" -a '+tracker+' -o \"'+torrentname+ '\" \"'+filepath+'\"'
     #logger.info(order)
     trytime=0
     filesize=0
     while filesize==0:
         trytime=trytime+1
         if trytime>10:
             logger.error('制作种子失败')
@@ -191,30 +210,99 @@
         if os.path.exists(torrentname):
             logger.info('已存在种子文件，正在删除'+torrentname)
             try:
                 os.remove(torrentname)
             except Exception as r:
                 logger.error('删除种子发生错误: %s' %(r))
         res=os.popen(order)
+        temp=res
         res=res.buffer.read().decode('utf-8')
-        if os.path.exists(torrentname):
-            filesize=os.path.getsize(torrentname)
-        else:
-            filesize=0
+        temp.close()
+        del(temp)
+        filesizetime=0
+        while filesize==0:
+            filesizetime=filesizetime+1
+            if filesizetime>5:
+                break
+            if os.path.exists(torrentname):
+                filesize=os.path.getsize(torrentname)
+            else:
+                filesize=0
+            if filesize==0:
+                time.sleep(1)
+        
 
     logger.info('已完成制作种子'+torrentname)
 
 
+def mktorrent(filepath: str, torrentname:str, tracker="https://announce.leaguehd.com/announce.php"):
+
+    if os.path.isdir(filepath):
+        logger.info('检测到路径制种，将先删除掉路径里面所有种子文件(torrent后缀)以及隐藏文件（.开头的文件）...')
+        deletetorrent(filepath) 
+    deletetorrent(os.path.dirname(torrentname))
+    logger.info('即将开始制作种子...')
+    torrent_path = Path(torrentname)
+    path = Path(filepath)
+    piece_size = 4 * 1024 * 1024
+    private = True
+    created_by = "Upload Machine"
+    source = "Upload Machine"
+    trytime=0
+    filesize=0
+
+    while filesize==0:
+        trytime=trytime+1
+        if trytime>10:
+            logger.error('制作种子失败')
+            return
+        if trytime>1:
+            logger.warning('第'+str(trytime-1)+'次制作种子失败')
+        logger.info('正在第'+str(trytime)+'次制作种子:') 
+        if torrent_path.exists():
+            logger.info('已存在种子文件，正在删除'+torrentname)
+            try:
+                os.remove(torrent_path)
+            except Exception as r:
+                logger.error('删除种子发生错误: %s' %(r))
+            
+        if tracker:
+            torrent = Torrent(path=str(path.absolute()), trackers=[tracker], piece_size=piece_size, private=private, created_by=created_by, source=source)
+        else:
+            torrent = Torrent(path=str(path.absolute()), piece_size=piece_size, private=private,  created_by=created_by)
+        bar = IncrementalBar(message="制种中:", max=torrent.pieces,suffix="%(index)d/%(max)d [%(eta_td)s]")
+
+        def cb(__torrent: Torrent, path: str, hashed_pieces: int, total_pieces: int):
+            bar.next()
+
+        torrent.generate(callback=cb, interval=0)
+        torrent.write(str(torrent_path))
+        bar.finish()
+        filesizetime=0
+        while filesize==0:
+            filesizetime=filesizetime+1
+            if filesizetime>5:
+                break
+            if os.path.exists(torrentname):
+                filesize=os.path.getsize(torrentname)
+            else:
+                filesize=0
+            if filesize==0:
+                time.sleep(1)
+    logger.info('已完成制作种子'+torrentname)
+    return 
+
 def get_video_duration(video_path: str):
     ext = os.path.splitext(video_path)[-1]
     if ext != '.mp4' and ext != '.avi' and ext != '.flv'and ext != '.ts'and ext != '.mkv':
         raise Exception('format not support')
     ffprobe_cmd = 'ffprobe -i "'+video_path+'" -show_entries format=duration -v quiet -of csv="p=0"'
     a=os.popen(ffprobe_cmd)
     duration_info = float(a.read())
+    a.close()
     #duration_info = float(a.buffer.read().decode('utf-8'))
     return duration_info
 
 def takescreenshot(file,screenshotaddress,screenshotnum):
     '''
     para:
         file:视频文件
@@ -269,31 +357,30 @@
                 if (os.path.isdir(c_path)) or (i.startswith('.')) or (not(  os.path.splitext(i)[1].lower()== ('.mp4') or os.path.splitext(i)[1].lower()== ('.mkv')  or os.path.splitext(i)[1].lower()== ('.avi') or os.path.splitext(i)[1].lower()== ('.ts')    )):
                     continue
                 filesize=os.path.getsize(c_path)
                 if filesize>maxsize:
                     self.address=c_path
                     maxsize=filesize
 
-               
-            if 'zeroday_path' in self.pathinfo.infodict and self.pathinfo.infodict['zeroday_path']!=None:
-                ls = os.listdir(self.pathinfo.infodict['zeroday_path'])
-                for i in ls:
-                    c_path=os.path.join(self.pathinfo.infodict['zeroday_path'], i)
-                    if (os.path.isdir(c_path)) or (i.startswith('.')) or (not(  os.path.splitext(i)[1].lower()== ('.mp4') or os.path.splitext(i)[1].lower()== ('.mkv')  or os.path.splitext(i)[1].lower()== ('.avi') or os.path.splitext(i)[1].lower()== ('.ts')    )):
-                        continue
-                    filesize=os.path.getsize(c_path)
-                    if filesize>maxsize:
-                        self.address=c_path
-                        maxsize=filesize
+            if self.pathinfo.collection>=1 and 'zeroday_name' in self.pathinfo.infodict and self.pathinfo.infodict['zeroday_name']!=None and self.pathinfo.infodict['zeroday_name']!='':
+                zeroday_path=os.path.join(self.pathinfo.path,self.pathinfo.infodict['zeroday_name'])
+                if os.path.exists(zeroday_path):
+                    ls = os.listdir(zeroday_path)
+                    for i in ls:
+                        c_path=os.path.join(zeroday_path, i)
+                        if (os.path.isdir(c_path)) or (i.startswith('.')) or (not(  os.path.splitext(i)[1].lower()== ('.mp4') or os.path.splitext(i)[1].lower()== ('.mkv')  or os.path.splitext(i)[1].lower()== ('.avi') or os.path.splitext(i)[1].lower()== ('.ts')    )):
+                            continue
+                        filesize=os.path.getsize(c_path)
+                        if filesize>maxsize:
+                            self.address=c_path
+                            maxsize=filesize
         
         else:
             self.address           = mediapath
             self.isdir=False
-            
- 
         
         #种子目录
         self.topath            = ''
         self.screenshotaddress = basic['screenshot_path']
         self.screenshotnum     = int(basic['picture_num'])
         self.imgdata           = imgdata
         
@@ -302,37 +389,41 @@
         self.mediatype         = pathinfo.type
         self.doubanurl         = pathinfo.doubanurl
         self.imdburl           = pathinfo.imdb_url
         self.bgmurl            = pathinfo.bgm_url
         self.anidburl          = pathinfo.anidb_url
         self.from_url          = pathinfo.from_url
         self.transfer          = pathinfo.transfer
+        self.complete          = pathinfo.complete
         self.filename          = os.path.basename(self.address)
         self.episodename       = findnum(self.filename)[0]
         self.episode           = int(self.episodename)
 
         self.sub               = self.pathinfo.sub
         self.englishname       = self.pathinfo.englishname
         self.chinesename       = self.pathinfo.chinesename
 
         self.audio_ch=0
         self.audio_jp=0
         self.audio_en=0
+        self.audio_yue=0
+        self.audio_num=0
+
         self.text_jp=0
         self.text_sc=0
         self.text_tc=0
         self.text_en=0
  
         if ('anime' in self.mediatype.lower() or 'tv' in self.mediatype.lower() ):
             self.season            = self.pathinfo.season
             self.seasonnum         = self.pathinfo.seasonnum
             self.season_ch         = self.pathinfo.season_ch
             self.complete          = self.pathinfo.complete
 
-        dlgroup           =['NaN-Raws','NaN Raws','NC-Raws','NC Raws','Lilith-Raws','Lilith Raws','ANi','Skymoon-Raws','Skymoon Raws']
+        dlgroup           =['NaN-Raws','NaN Raws','NC-Raws','NC Raws','Lilith-Raws','Lilith Raws','ANi','Skymoon-Raws','Skymoon Raws','GMTeam','GM-Team']
         self.type              ='WEBRip'
         self.Video_Format      ='H264'
         
         if 'hdtvrip' in self.filename.lower() or 'hdtv-rip' in self.filename.lower() or 'tv-rip' in self.filename.lower() or 'tvrip' in self.filename.lower():
             self.type='HDTVRip'
         elif 'hdtv' in self.filename.lower():
             self.type='HDTV'
@@ -359,26 +450,28 @@
         self.getptgen_done=0
         self.mktorrent_done=0
         self.getinfo_done=0
 
 
         self.language=''
         self.country=''
-        self.year=2022
+        self.year=2023
+
         #根据文件名判断内嵌字幕信息
         self.sublan=''
         jp=0
         sc=0
         tc=0
         if 'SC' in self.filename.upper() or 'CHS' in self.filename.upper() or 'GB' in self.filename.upper() or '简' in self.filename.upper() or '簡' in self.filename.upper():
             sc=1
         if 'TC' in self.filename.upper() or 'CHT' in self.filename.upper() or 'BIG5' in self.filename.upper() or '繁' in self.filename.upper():
             tc=1
         if 'JP' in self.filename.upper() or 'JAPANESE' in self.filename.upper() or '日' in self.filename.upper():
             jp=1
+        
         if jp==0 and sc==0 and tc==1:
             self.sublan='[内嵌繁中]'
         elif jp==0 and sc==1 and tc==0:
             self.sublan='[内嵌简中]'
         elif jp==0 and sc==1 and tc==1:
             self.sublan='[内嵌简繁中字]'
         elif jp==1 and sc==0 and tc==0:
@@ -387,14 +480,15 @@
             self.sublan='[内嵌繁日双语]'
         elif jp==1 and sc==1 and tc==0:
             self.sublan='[内嵌简日双语]'
         elif jp==1 and sc==1 and tc==1:
             self.sublan='[内嵌简繁日双语]'
         else:
             self.sublan=''
+        
         if jp+sc+tc>0:
             logger.info('根据文件名分析，字幕语言为'+self.sublan)
         else:
             logger.warning('无法根据文件名分析出字幕语言信息')
 
 
 
@@ -444,46 +538,46 @@
                     if subitem.lower().startswith('language') or subitem.lower().startswith('title'):
                         if 'SC' in subitem.upper() or 'CHS' in subitem.upper() or 'GB' in subitem.upper() or '简' in subitem.upper() or '簡' in subitem.upper():
                             sc=1
                         if 'TC' in subitem.upper() or 'CHT' in subitem.upper() or 'BIG5' in subitem.upper() or '繁' in subitem.upper():
                             tc=1
                         if 'JP' in subitem.upper() or 'JA' in subitem.upper() or'JAPANESE' in subitem.upper() or '日' in subitem.upper():
                             jp=1
-                        elif 'EN' in subitem.upper() or 'ENGLISH' in subitem.upper() or '英' in subitem.upper():
+                        if 'EN' in subitem.upper() or 'ENGLISH' in subitem.upper() or '英' in subitem.upper():
                             en=1
         if en==0 and jp==0 and sc==0 and tc==1:
-            self.sublan='[繁体中字]'
+            self.sublan='[内封繁体中字]'
         elif en==0 and jp==0 and sc==1 and tc==0:
-            self.sublan='[简体中字]'
+            self.sublan='[内封简体中字]'
         elif en==0 and jp==0 and sc==1 and tc==1:
-            self.sublan='[简繁中字]'
+            self.sublan='[内封简繁中字]'
         elif en==0 and jp==1 and sc==0 and tc==0:
-            self.sublan='[日文字幕]'
+            self.sublan='[内封日文字幕]'
         elif en==0 and jp==1 and sc==0 and tc==1:
-            self.sublan='[繁日双语]'
+            self.sublan='[内封繁日双语]'
         elif en==0 and jp==1 and sc==1 and tc==0:
-            self.sublan='[简日双语]'
+            self.sublan='[内封简日双语]'
         elif en==0 and jp==1 and sc==1 and tc==1:
-            self.sublan='[简繁日双语]'
+            self.sublan='[内封简繁日双语]'
         elif en==1 and jp==0 and sc==0 and tc==0:
-            self.sublan='[英文字幕]'
+            self.sublan='[内封英文字幕]'
         elif en==1 and jp==0 and sc==0 and tc==1:
-            self.sublan='[繁英双语]'
+            self.sublan='[内封繁英双语]'
         elif en==1 and jp==0 and sc==1 and tc==0:
-            self.sublan='[简英双语]'
+            self.sublan='[内封简英双语]'
         elif en==1 and jp==0 and sc==1 and tc==1:
-            self.sublan='[简繁英双语]'
+            self.sublan='[内封简繁英双语]'
         elif en==1 and jp==1 and sc==0 and tc==0:
-            self.sublan='[日英双语]'
+            self.sublan='[内封日英双语]'
         elif en==1 and jp==1 and sc==0 and tc==1:
-            self.sublan='[繁日英三语]'
+            self.sublan='[内封繁日英三语]'
         elif en==1 and jp==1 and sc==1 and tc==0:
-            self.sublan='[简日英三语]'
+            self.sublan='[内封简日英三语]'
         elif en==0 and jp==1 and sc==1 and tc==1:
-            self.sublan='[简繁日英三语]'
+            self.sublan='[内封简繁日英三语]'
 
         self.text_jp=jp
         self.text_sc=sc
         self.text_tc=tc
         self.text_en=en
 
         if jp+sc+tc+en>0:
@@ -491,14 +585,15 @@
         else:
             logger.warning('无法根据mediainfo分析出字幕语言信息')
 
     def dealaudio(self,res):
         ch=0
         jp=0
         en=0
+        yue=0
         a=res.split('\n\n')
         for item in a:
             if item.startswith('Audio'):
                 b=item.split('\n')
                 for subitem in b:
                     if subitem.lower().startswith('language') or subitem.lower().startswith('title'):
 
@@ -507,16 +602,18 @@
                             #logger.info('根据mediainfo音轨分析，语言为'+self.language)
                         if  'JAPANESE' in subitem.upper() or '日' in subitem.upper():
                             jp=1
                             #logger.info('根据mediainfo音轨分析，语言为'+self.language)
                         if 'ENGLISH' in subitem.upper() or '英' in subitem.upper():
                             en=1
                             #logger.info('根据mediainfo音轨分析，语言为'+self.language)
+                        if 'CANTON' in subitem.upper() or '粤' in subitem.upper():
+                            yue=1
 
-
+        '''
         if jp==0 and ch==0 and en==1:
             self.language='英语'
         elif jp==0 and ch==1 and en==0:
             self.language='国语'
         elif jp==0 and ch==1 and en==1:
             self.language='中英双语'
         elif jp==1 and ch==0 and en==0:
@@ -524,49 +621,75 @@
         elif jp==1 and ch==0 and en==1:
             self.language='日英双语'
         elif jp==1 and ch==1 and en==0:
             self.language='中日双语'
         elif jp==1 and ch==1 and en==1:
             self.language='中英日三语'
         else:
+            self.language=self.language
+        '''
+        if jp+ch+en+yue>0:
             self.language=''
-
+            if ch==1:
+                self.language=self.language+'国'
+            if yue==1:
+                self.language=self.language+'粤'
+            if jp==1:
+                self.language=self.language+'日'
+            if en==1:
+                self.language=self.language+'英'
+        self.audio_num=jp+ch+en+yue
         self.audio_ch=ch
         self.audio_jp=jp
         self.audio_en=en
+        self.audio_yue=yue
 
-        if jp+ch+en>0:
+        if self.audio_num=='1':
+            self.language=self.language+'语'
+        elif self.audio_num=='2':
+            self.language=self.language+'双语'
+        elif self.audio_num=='3':
+            self.language=self.language+'三语'
+        elif self.audio_num=='4':
+            self.language=self.language+'四语'
+
+        if self.audio_num>0:
             logger.info('根据mediainfo音轨分析，语言为'+self.language)
         else:
             logger.warning('无法根据mediainfo分析出音轨语言信息')
 
     def getaudio(self):
         ch=0
         jp=0
         en=0
+        yue=0
         infolist=self.mediainfo_json['media']['track']
         for item in infolist:
             if not '@type' in item:
                 continue
             if item['@type'].lower()=='audio':
                 if 'Title' in item :
                     if 'CHINESE' in item['Title'].upper() or '中' in item['Title'].upper() or 'CH' in item['Title'].upper() or 'ZH' in item['Title'].upper() or '国' in item['Title'].upper():
                         ch=1
                     if  'JA' in item['Title'].upper() or 'JP' in item['Title'].upper() or '日' in item['Title'].upper():
                         jp=1
                     if 'EN' in item['Title'].upper() or '英' in item['Title'].upper():
                         en=1
+                    if 'CANTON' in item['Title'].upper() or '粤' in item['Title'].upper():
+                        yue=1
                 elif 'Language' in item :
                     if 'CHINESE' in item['Language'].upper() or '中' in item['Language'].upper() or 'CH' in item['Language'].upper() or 'ZH' in item['Language'].upper() or '国' in item['Language'].upper():
                         ch=1
                     if  'JA' in item['Language'].upper() or 'JP' in item['Language'].upper() or '日' in item['Language'].upper():
                         jp=1
                     if 'EN' in item['Language'].upper() or '英' in item['Language'].upper():
                         en=1
-
+                    if 'CANTON' in item['Language'].upper() or '粤' in item['Language'].upper():
+                        yue=1
+        '''
         if jp==0 and ch==0 and en==1:
             self.language='英语'
         elif jp==0 and ch==1 and en==0:
             self.language='国语'
         elif jp==0 and ch==1 and en==1:
             self.language='中英双语'
         elif jp==1 and ch==0 and en==0:
@@ -574,25 +697,54 @@
         elif jp==1 and ch==0 and en==1:
             self.language='日英双语'
         elif jp==1 and ch==1 and en==0:
             self.language='中日双语'
         elif jp==1 and ch==1 and en==1:
             self.language='中英日三语'
         else:
-            self.language=''
+            self.language=self.language
 
         self.audio_ch=ch
         self.audio_jp=jp
         self.audio_en=en
 
         if jp+ch+en>0:
             logger.info('根据mediainfo音轨分析，语言为'+self.language)
         else:
             logger.warning('无法根据mediainfo分析出音轨语言信息')
+        '''
+        if jp+ch+en+yue>0:
+            self.language=''
+            if ch==1:
+                self.language=self.language+'国'
+            if yue==1:
+                self.language=self.language+'粤'
+            if jp==1:
+                self.language=self.language+'日'
+            if en==1:
+                self.language=self.language+'英'
+        self.audio_num=jp+ch+en+yue
+        self.audio_ch=ch
+        self.audio_jp=jp
+        self.audio_en=en
+        self.audio_yue=yue
 
+        if self.audio_num=='1':
+            self.language=self.language+'语'
+        elif self.audio_num=='2':
+            self.language=self.language+'双语'
+        elif self.audio_num=='3':
+            self.language=self.language+'三语'
+        elif self.audio_num=='4':
+            self.language=self.language+'四语'
+
+        if self.audio_num>0:
+            logger.info('根据mediainfo音轨分析，语言为'+self.language)
+        else:
+            logger.warning('无法根据mediainfo分析出音轨语言信息')
 
     def getsubtext(self):
         jp=0
         sc=0
         tc=0
         en=0
         infolist=self.mediainfo_json['media']['track']
@@ -655,33 +807,70 @@
         self.text_en=en
 
         if jp+sc+tc+en>0:
             logger.info('根据mediainfo分析，字幕语言为'+self.sublan)
         else:
             logger.warning('无法根据mediainfo分析出字幕语言信息')
 
+    def updatemediainfo(self,filepath=''):
+        if os.path.isdir(self.topath):
+            self.address=os.path.join(self.topath,os.path.basename(self.address))
+        if not (filepath=='' or filepath==None):
+            logger.info('检测到mediainfo模板文件正在应用...')
+            a=os.popen('mediainfo --Inform=file://"'+filepath+'" "'+self.address+'"')
+            res=a.buffer.read().decode('utf-8')
+            self.mediainfo=res
+            a.close()
+            self.content=self.douban_info+"\n[quote=Mediainfo]\n"+self.mediainfo+"[/quote]\n"+self.screenshoturl
+            #logger.info('使用模板后，mediainfo变更为:\n'+self.mediainfo)
+        else:
+            #logger.info('未检测到mediainfo模板文件,正在使用原版mediainfo...')
+            a=os.popen('mediainfo "'+self.address+'"')
+            res=a.buffer.read().decode('utf-8')
+            a.close()
+            ss=res.split('\n')
+            for i in range(len(ss)):
+                if ss[i].startswith('Complete name'):
+                    ss[i]=':'.join([ss[i].split(':')[0],' '+self.filename])
+            i=0
+            while (i<len(ss)):
+                if (ss[i].upper()).startswith('Unique'.upper()):
+                    del(ss[i])
+                    i=i-1
+                i+=1
+            res='\n'.join(ss)
+            self.mediainfo=res
+            self.content=self.douban_info+"\n[quote=Mediainfo]\n"+self.mediainfo+"[/quote]\n"+self.screenshoturl
 
     def getmediainfo(self):
         if self.getmediainfo_done==1:
             return self.mediainfo
-        a=os.popen("mediainfo \""+self.address+'"')
+        a=os.popen('mediainfo "'+self.address+'"')
         #res=a.read()
         res=a.buffer.read().decode('utf-8')
+        a.close()
         #self.dealsubtext(res)
         #self.dealaudio(res)
         ss=res.split('\n')
         #ss[1]=':'.join([ss[1].split(':')[0],' '+self.filename])
         for i in range(len(ss)):
             if ss[i].startswith('Complete name'):
                 ss[i]=':'.join([ss[i].split(':')[0],' '+self.filename])
+        i=0
+        while (i<len(ss)):
+            if (ss[i].upper()).startswith('Unique'.upper()):
+                del(ss[i])
+                i=i-1
+            i+=1
 
         self.mediainfo='\n'.join(ss)
         a=os.popen("mediainfo --Output=JSON \""+self.address+'"')
         #res_json=a.read()
         res_json=a.buffer.read().decode('utf-8')
+        a.close()
         media_json=json.loads(res_json)
 
         self.mediainfo_json=media_json
 
         self.getsubtext()
         self.getaudio()
 
@@ -764,59 +953,105 @@
                 self.release=item[5:].strip()
                 logger.info('根据豆瓣信息分析，上映日期为'+self.release)
             if '首\u3000\u3000播'in item:
                 self.firstRelease=item[5:].strip()
                 logger.info('根据豆瓣信息分析，首播为'+self.firstRelease)
             if '集\u3000\u3000数'in item:
                 self.num=int(item[5:].strip())
-                if self.pathinfo.max>=self.num:
-                    self.complete=1
+                if not (self.complete==1 or self.complete==0):
+                    if self.pathinfo.max>=self.num:
+                        self.complete=1
+                    else:
+                        self.complete=0
                 logger.info('根据豆瓣信息分析，总集数为'+str(self.num))
             if self.imdburl=='' and 'imdb'in item and '链接'in item and not((item[7:].strip()).endswith('//')):
                 self.imdburl=item[7:].strip()
             if '片\u3000\u3000长'in item:
                 self.runtime=item[5:].strip()
-    
+            if not (self.complete==1 or self.complete==0):
+                self.complete=0
     def get_douban(self):
         if 'doubancookie' in self.basic and self.basic['doubancookie']!=None:
-            res_douban=getdoubaninfo(url=self.doubanurl,cookie=self.basic['doubancookie'],ret_val=True)
+            get_success=0
+            get_time=0
+            while get_success==0:
+                get_time+=1
+                if get_time>5:
+                    raise Exception('获取豆瓣info出错，请尝试能否正常打开豆瓣')
+                try:
+                    res_douban=getdoubaninfo(url=self.doubanurl,cookie=self.basic['doubancookie'],ret_val=True)
+                    douban_dict=res_douban.parse()
+                    get_success=1
+                except Exception as r:
+                    get_success=0
+                    logger.warning('抓取豆瓣info错误，一秒后重试，原因: %s' %(r))
+                    time.sleep(1)
+
         else:
-            res_douban=getdoubaninfo(url=self.doubanurl,ret_val=True)
-        douban_dict=res_douban.parse()
+            get_success=0
+            get_time=0
+            while get_success==0:
+                get_time+=1
+                if get_time>5:
+                    raise Exception('获取豆瓣info出错，请尝试能否正常打开豆瓣')
+                try:
+                    res_douban=getdoubaninfo(url=self.doubanurl,ret_val=True)
+                    douban_dict=res_douban.parse()
+                    get_success=1
+                except Exception as r:
+                    get_success=0
+                    logger.warning('抓取豆瓣info错误，一秒后重试，原因: %s' %(r))
+                    time.sleep(1)
+        
+
+        self.douban_dict=douban_dict
         self.douban_info=res_douban.info()
 
         #if (douban_dict['names']['chinesename']):
         #    self.chinesename=douban_dict['names']['chinesename']
         if (douban_dict['names']['akaTitles']):
             self.allName='/'.join(douban_dict['names']['akaTitles'])
         if (douban_dict['year']):
             try:
                 self.year=int(douban_dict['year'])
             except:
                 logger.warning("douban_dict['year']转换数字出错,其内容为: "+str(douban_dict['year']))
-                self.year=2022
+                self.year=2023
         if (douban_dict['countries'] and len(douban_dict['countries']) > 0) :
             self.country=" / ".join(douban_dict['countries'])
         if (douban_dict['genres'] and len(douban_dict['genres']) > 0):
             self.genre=" / ".join(douban_dict['genres'])
         if (douban_dict['languages'] and len(douban_dict['languages']) > 0) :
-            self.language=" / ".join(douban_dict['languages'])
+            if self.language.strip()=='':
+                self.language=" / ".join(douban_dict['languages'])
+                logger.info('根据豆瓣信息分析，语言为'+self.language)
         if (douban_dict['pubdates'] and len(douban_dict['pubdates']) > 0) :
             self.release=" / ".join(douban_dict['pubdates'])
         if (douban_dict['imdb'].strip()!='') :
             self.imdburl=douban_dict['imdb']
-            self.pathinfo.imdb_url=douban_dict['imdb']
-            logger.info('根据豆瓣信息分析，imdb链接为'+douban_dict['imdb'])
-        if (douban_dict['episodes']) :
+            self.imdburl='https://www.imdb.com/title/'+self.imdburl+'/'
+            self.pathinfo.imdb_url=self.imdburl
+            logger.info('根据豆瓣信息分析，imdb链接为'+self.imdburl)
+        if (douban_dict['episodes']) and  (not('movie' in self.mediatype.lower())):
             self.media_type='TV_series'
-            self.num=int(douban_dict['episodes'])
-            if self.pathinfo.max>=self.num:
-                self.complete=1
-            logger.info('根据豆瓣信息分析，总集数为'+str(self.num))
-        
+            try:
+                self.num=int(douban_dict['episodes'])
+                logger.info('根据豆瓣信息分析，总集数为'+str(self.num))
+            except:
+                self.num=1000000
+                logger.info('豆瓣页面暂无集数数据')
+            if not (self.complete==1 or self.complete==0):
+                if self.pathinfo.max>=self.num:
+                    self.complete=1
+                else:
+                    self.complete=0
+            
+        #没有获取到集数信息则默认为“未完结”
+        if not (self.complete==1 or self.complete==0):
+                self.complete=0
         self.getptgen_done=1
 
     def getptgen_douban_info(self):
         if self.getptgen_done==1:
             return
         url='https://api.iyuu.cn/App.Movie.Ptgen?url='+self.doubanurl
         user_agent = 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/98.0.4758.102 Safari/537.36'
@@ -919,23 +1154,26 @@
             douban_info += "\n◎首\u3000\u3000播　" + " / ".join(data['firstRelease'])
             self.firstRelease=" / ".join(data['firstRelease'])
             logger.info('根据豆瓣信息分析，首播为'+self.firstRelease)
         if (data['num']) :
             douban_info += "\n◎集\u3000\u3000数　" + data['num']
             self.media_type='TV_series'
             self.num=int(data['num'])
-            if self.pathinfo.max>=self.num:
-                self.complete=1
+            if not (self.complete==1 or self.complete==0):
+                if self.pathinfo.max>=self.num:
+                    self.complete=1
+                else:
+                    self.complete=0
             logger.info('根据豆瓣信息分析，总集数为'+str(self.num))
         if (data['imdbRating']) :
             douban_info += "\n◎IMDb评分  " + data['imdbRating'] + "/10 from " + data['imdbVotes'] + " users"
         if (data['imdbUrl']) :
             douban_info += "\n◎IMDb链接  " + data['imdbUrl']
             self.imdburl=data['imdbUrl']
-            pathinfo.imdb_url=data['imdbUrl']
+            self.pathinfo.imdb_url=data['imdbUrl']
             logger.info('根据豆瓣信息分析，imdb链接为'+data['imdbUrl'])
         if (data['rating']) :
             douban_info += "\n◎豆瓣评分　" + data['rating'] + "/10 from " + data['votes'] + " users";
         if (data['url']) :
             douban_info += "\n◎豆瓣链接　" + data['url']
         if (data['runtime'] and len(data['runtime']) > 0) :
             douban_info += "\n◎片　　长　" + " / ".join(data['runtime'])
@@ -974,54 +1212,71 @@
             for item in data['awards']:
                 awardstr=awardstr+"\n\n　　" + item['title'];
                 for itemc in item['content']:
                     awardstr=awardstr+"\n　　" + itemc
             douban_info += "\n\n◎获奖情况　" + awardstr
 
         douban_info =douban_info+ "\n\n"
-
+        if not (self.complete==1 or self.complete==0):
+            self.complete=0
         self.douban_info=douban_info
         self.getptgen_done=1
 
     def mktorrent(self,tracker='https://announce.leaguehd.com/announce.php'):
         #if self.mktorrent_done==1:
         #    return
         torrentpath=os.path.join(self.screenshotaddress,str(self.episode)+'.torrent')
         self.torrentpath=torrentpath
         mktorrent(self.topath,torrentpath,tracker=tracker)
         self.mktorrent_done=1
 
     def gettorrent(self,tracker='https://announce.leaguehd.com/announce.php'):
+        if not('new_folder' in self.basic and self.basic['new_folder']>=1):
+            self.mktorrent(tracker)
+            return
         dirpath=os.path.dirname(self.topath)
         filelist=[]
         if not os.path.exists(self.topath):
             os.makedirs(self.topath)
         else:
             ls = os.listdir(self.topath)
             for i in ls:
                 c_path=os.path.join(self.topath, i)
+                if i.startswith('.') and os.path.exists(c_path):
+                    try:
+                        os.remove(c_path)
+                    except Exception as r:
+                        logger.error('删除.开头文件"'+c_path+'"发生错误: %s' %(r))
+                    continue
                 if (os.path.isdir(c_path)):
                     if not os.path.exists(   os.path.join(dirpath,i)    ):
                         newpath=move(c_path,dirpath)
                         filelist.append(newpath)
                     else:
                         logger.warning('由于文件'+c_path+'在里外文件夹均已存在,已改名为_temp')
-                        os.rename(c_path,c_path+'_temp')
+                        try:
+                            os.rename(c_path,c_path+'_temp')
+                        except Exception as r:
+                            logger.error('rename文件夹"'+c_path+'"发生错误: %s' %(r))
                         newpath=move(c_path+'_temp',dirpath)
                         filelist.append(newpath)
                 else:
                     if not os.path.exists(   os.path.join(dirpath,i)    ):
                         newpath=move(c_path,dirpath)
                         filelist.append(newpath)
                     else:
                         logger.warning('由于文件'+c_path+'在里外文件夹均已存在,已改名为_temp')
                         stem, suffix = os.path.splitext(c_path)
-                        os.rename(c_path,stem+'_temp'+suffix)
-                        newpath=move(stem+'_temp'+suffix,dirpath)
-                        filelist.append(newpath)
+                        try:
+                            os.rename(c_path,stem+'_temp'+suffix)
+                            newpath=move(stem+'_temp'+suffix,dirpath)
+                            filelist.append(newpath)
+                        except Exception as r:
+                            logger.error('rename temp文件"'+c_path+'"发生错误: %s' %(r))
+                        
 
         logger.info('检测到路径制种，将先删除掉路径里面所有种子文件(torrent后缀)以及隐藏文件（.开头的文件）...')
         deletetorrent(self.topath) 
         if os.path.isdir(self.mediapath):
             ls = os.listdir(self.mediapath)
             for i in ls:
                 c_path=os.path.join(self.mediapath, i)
@@ -1033,28 +1288,38 @@
 
         self.mktorrent(tracker)
 
         for item in filelist:
             if os.path.exists(item):
                 newpath=move(item,self.topath)
                 if '_temp' in newpath and os.path.exists(newpath):
-                    rename(newpath,newpath.replace('_temp',''))
+                    os.rename(newpath,newpath.replace('_temp',''))
+            else:
+                logger.warning('文件 '+item+' 丢失')
 
 
 
     def getfullinfo(self,tracker='https://announce.leaguehd.com/announce.php'):
         if self.getinfo_done==1:
             return
-
+        
+        trytime=0
         while not self.getptgen_done==1:
+            logger.info('正在获取豆瓣信息...')
+            trytime += 1
+            if trytime>10:
+                logger.error('获取豆瓣信息失败')
+                raise Exception('获取豆瓣信息失败')
             self.get_douban()
+            '''
             if self.getptgen_done<1:
                 self.getptgen_douban_info()
             if self.getptgen_done<1:
                 self.getdoubaninfo()
+            '''
             if self.getptgen_done<1:
                 time.sleep(3)
         
 
 
         self.getmediainfo()
 
@@ -1069,74 +1334,133 @@
         if self.pathinfo.txt_info!='':
             self.sublan='['+self.pathinfo.txt_info+']'
         if self.pathinfo.audio_info!='':
             self.language=self.pathinfo.audio_info
 
 
         self.uploadname=self.englishname+' '+str(self.year)
-        self.small_descr=self.chinesename
-
+        self.uploadname_sharkpt = self.englishname
+        self.small_descr=self.chinesename.strip()
+        
+        
         
         medianame=self.uploadname
         if self.pathinfo.type=='anime' or self.pathinfo.type=='tv':
             self.uploadname=self.uploadname+' '+self.season
-            self.small_descr=self.small_descr+' ('+self.season_ch+') '
+            self.uploadname_sharkpt=self.uploadname_sharkpt+' '+self.season
+            #if int(self.seasonnum)>1:
+            #self.small_descr=self.small_descr+' | '+self.season_ch.strip()
             medianame=self.uploadname
             if not self.isdir:
                 self.uploadname=self.uploadname+'E'+self.episodename
-                self.small_descr=self.small_descr+'(第'+self.episodename+'集) '
+                self.uploadname_sharkpt=self.uploadname_sharkpt+'E'+self.episodename
+                self.small_descr=self.small_descr+' | 第'+self.episodename+'集'
+            elif self.pathinfo.collection==2:
+                eps_temp=findeps([self.mediapath])
+                eps_temp.sort()
+                if len(eps_temp)>1:
+                    self.uploadname=self.uploadname+'E'+str(eps_temp[0]).zfill(2)+'-E'+str(eps_temp[-1]).zfill(2)
+                    self.uploadname_sharkpt=self.uploadname_sharkpt+'E'+str(eps_temp[0]).zfill(2)+'-E'+str(eps_temp[-1]).zfill(2)
+                    self.small_descr=self.small_descr+' | 第'+str(eps_temp[0]).zfill(2)+'-'+str(eps_temp[-1]).zfill(2)+'集'
+                else:
+                    self.uploadname=self.uploadname+'E'+self.episodename
+                    self.uploadname_sharkpt=self.uploadname_sharkpt+'E'+self.episodename
+                    self.small_descr=self.small_descr+' | 第'+self.episodename+'集'
             elif self.complete==1:
                 self.uploadname=self.uploadname
-                self.small_descr=self.small_descr+'(全'+str(self.pathinfo.max)+'集)'
+                self.small_descr=self.small_descr+' | 全 '+str(self.pathinfo.max)+' 集'
             else:
                 self.uploadname=self.uploadname+'E'+str(self.pathinfo.min).zfill(2)+'-E'+str(self.pathinfo.max).zfill(2)
-                self.small_descr=self.small_descr+'(第'+str(self.pathinfo.min).zfill(2)+'-'+str(self.pathinfo.max).zfill(2)+'集)'
+                self.uploadname_sharkpt=self.uploadname_sharkpt+'E'+str(self.pathinfo.min).zfill(2)+'-E'+str(self.pathinfo.max).zfill(2)
+                self.small_descr=self.small_descr+' | 第'+str(self.pathinfo.min).zfill(2)+'-'+str(self.pathinfo.max).zfill(2)+'集'
+
+
+        if self.douban_dict['directors']:
+            self.small_descr=self.small_descr+' | 导演: '+self.douban_dict['directors'][0]['name'].strip()
+            for i in range(min(len(self.douban_dict['directors'])-1,1)):
+                self.small_descr=self.small_descr+' / '+self.douban_dict['directors'][i+1]['name'].strip()
+
+        if self.douban_dict['actors']:
+            self.small_descr=self.small_descr+' | 主演: '+self.douban_dict['actors'][0]['name'].strip()
+            for i in range(min(len(self.douban_dict['actors'])-1,4)):
+                self.small_descr=self.small_descr+' / '+self.douban_dict['actors'][i+1]['name'].strip()
 
         medianame = medianame+' '+self.standard_sel+' '+self.type+' '+self.Video_Format+' '+self.Audio_Format+'-'+self.sub
         while '  'in medianame:
             medianame=medianame.replace('  ',' ')
         medianame=medianame.replace(' ','.')
-        #self.topath=os.path.join(os.path.dirname(self.address),medianame)
-        self.topath=os.path.join(self.pathinfo.path,medianame)
-
-        if self.pathinfo.zeroday_name!='':
-            #self.topath=os.path.join(os.path.dirname(self.address),self.pathinfo.zeroday_name)
-            self.topath=os.path.join(self.pathinfo.path,self.pathinfo.zeroday_name)
+        
 
         
 
         if 'new_folder' in self.basic and self.basic['new_folder']==1:
-            self.pathinfo.infodict['zeroday_path']=self.topath
+            if self.pathinfo.zeroday_name!='':
+                self.topath=os.path.join(self.pathinfo.path,self.pathinfo.zeroday_name)
+            else:
+                self.topath=os.path.join(self.pathinfo.path,medianame)
+                self.pathinfo.zeroday_name=medianame
+                self.pathinfo.infodict['zeroday_name']=medianame
+        elif 'new_folder' in self.basic and self.basic['new_folder']==2:
+            if self.pathinfo.zeroday_name!='':
+                self.topath=os.path.join(self.pathinfo.path,self.pathinfo.zeroday_name)
+            else:
+                tempchinesename=self.chinesename.strip()
+                while '  'in tempchinesename:
+                    tempchinesename=tempchinesename.replace('  ',' ')
+                tempchinesename=tempchinesename.replace(' ','.')
+                self.topath=os.path.join(self.pathinfo.path,tempchinesename+'.'+medianame)
+                self.pathinfo.infodict['zeroday_name']=tempchinesename+'.'+medianame
+                self.pathinfo.zeroday_name=tempchinesename+'.'+medianame
+                del(tempchinesename)
         else:
             self.topath=self.mediapath
+            
 
             
 
-        self.uploadname_ssd=self.uploadname+' '+self.type+' '+self.standard_sel+' '+self.Video_Format+' '+self.Audio_Format+'-'+self.sub
-        self.uploadname    =self.uploadname+' '+self.standard_sel+' '+self.type+' '+self.Video_Format+' '+self.Audio_Format+'-'+self.sub
+        self.uploadname_ssd     =self.uploadname+' '+self.type+' '+self.standard_sel+' '+self.Video_Format+' '+self.Audio_Format+(self.audio_num>1)*('.'+str(self.audio_num)+'Audio') +'-'+self.sub
+        self.uploadname_sharkpt =self.uploadname_sharkpt+' '+str(self.year)+' '+self.standard_sel+' '+self.type+' '+self.Video_Format+' '+self.Audio_Format+(self.audio_num>1)*(' '+str(self.audio_num)+'Audio') +'-'+self.sub
+        self.uploadname         =self.uploadname+' '+self.standard_sel+' '+self.type+' '+self.Video_Format+' '+self.Audio_Format+(self.audio_num>1)*(' '+str(self.audio_num)+'Audio') +'-'+self.sub
         
         try:
-            if not self.language=='':
-                self.small_descr=self.small_descr+'['+self.language+'] '
+            if self.language!='':
+                self.small_descr=self.small_descr+' ['+self.language+']'
         except:
             logger.warning('未找到资源语言信息，默认为日语')
-            self.small_descr=self.small_descr+'[日语] '
+            self.small_descr=self.small_descr+' [日语]'
 
         if not self.sublan=='':
-            self.small_descr=self.small_descr+self.sublan
+            self.small_descr=self.small_descr+' '+self.sublan
+        else:
+            self.small_descr=self.small_descr+' [无字幕]'
         self.small_descr=self.small_descr.replace('（','(').replace('）',')')
 
-
+        if self.pathinfo.small_descr!='':
+            self.small_descr=self.pathinfo.small_descr
+        #logger.debug('副标题为'+self.small_descr)
         self.getimgurl()
+        if self.pathinfo.screenshot!='':
+            self.screenshoturl=self.pathinfo.screenshot+'\n'+self.screenshoturl
         self.content=self.douban_info+"\n[quote=Mediainfo]\n"+self.mediainfo+"[/quote]\n"+self.screenshoturl
+
+        if self.pathinfo.contenthead!='':
+            self.content= self.pathinfo.contenthead+self.content
         
-        if 'new_folder' in self.basic and self.basic['new_folder']==1:
+        if self.pathinfo.contenttail!='':
+            self.content= self.content+self.pathinfo.contenttail
+
+        '''
+        if 'new_folder' in self.basic and self.basic['new_folder']>=1:
             self.gettorrent(tracker)
         else:
             self.mktorrent(tracker)
+        '''
+        self.gettorrent(tracker)
+        if not (self.complete==1 or self.complete==0):
+            self.complete=0
         self.getinfo_done=1
 
     def print(self):
         self.getfullinfo()
         attr=['uploadname','small_descr','content']
         for item in attr:
             exec('print("'+item+':"  ,self.'+item+'  )')
```

### Comparing `upload_machine-0.0.8/upload_machine/utils/para_ctrl/para_ctrl.py` & `upload_machine-0.0.80/upload_machine/utils/para_ctrl/para_ctrl.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.8/upload_machine/utils/para_ctrl/readargs.py` & `upload_machine-0.0.80/upload_machine/utils/para_ctrl/readargs.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     parser = argparse.ArgumentParser(description='Weclome Upload_Machine By Sauterne')
     parser.add_argument('-u','--upload', action='store_true', default=False, help='Upload local resources automatically')
     parser.add_argument('-s','--sign', action='store_true', default=False, help='SignUp automatically')
     parser.add_argument('-iu','--img-upload', action='store_true', default=False, help='Upload picture as url')
     parser.add_argument('-di','--douban-info', action='store_true', default=False, help='Get douban info')
     parser.add_argument('-mi','--media-img', action='store_true', default=False, help='Get screenshots of the video and upload the image')
 
-    parser.add_argument('-ih','--img-host', type=str, help='Choose your img host from the following list. [ptpimg,picgo,chd,smms,pter,emp,femp,imgbox,freeimage]',choices=['ptpimg','picgo','chd','smms','pter','emp','femp','imgbox','freeimage'],required=False,default='')
+    parser.add_argument('-ih','--img-host', type=str, help='Choose your img host from the following list. [ptpimg,picgo,chd,smms,pter,emp,femp,imgbox,freeimage,redleaves,sharkimg]',choices=['ptpimg','picgo','chd','smms','pter','emp','femp','imgbox','freeimage','redleaves','sharkimg'],required=False,default='')
     parser.add_argument('-if','--img-file', nargs='+',help='Choose your img file',action='append',required=False)
     parser.add_argument('-iform','--img-form', help='Choose your img form the following list. [bbcode,img]',choices=['bbcode','img'],required=False,default='img')
 
     parser.add_argument('-du','--douban-url', type=str, help='Input your douban-url',required=False,default='')
 
     parser.add_argument('-mf','--media-file', type=str, help='Choose your mediafile',required=False,default='')
     parser.add_argument('-in','--img-num', type=int, help='Choose the number of screenshots,default=3',required=False,default=3)
```

### Comparing `upload_machine-0.0.8/upload_machine/utils/pathinfo/pathinfo.py` & `upload_machine-0.0.80/upload_machine/utils/pathinfo/pathinfo.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,75 +4,75 @@
 from urllib.parse import unquote
 import re
 import requests
 from upload_machine.utils.para_ctrl.readyaml import write_yaml
 from shutil import move
 
 def findnum(name):
-    num=re.findall(r" ([0-9]{1,2}) ",name)
-    if len(num)!=0:
-        sty=" "+num[0]+" "
-        stz=" XX "
-        stx=" "+num[0]+" "
-        return num[0],sty,stz,stx
-    num=re.findall(r"第([0-9]{1,2})話",name)
-    if len(num)!=0:
-        sty='第'+num[0]+'話'
-        stz="第XX話"
-        stx='第'+num[0]+'話'
-        return num[0],sty,stz,stx
-    num=re.findall(r"第([0-9]{1,2})话",name)
-    if len(num)!=0:
-        sty='第'+num[0]+'话'
-        stz="第XX话"
-        stx='第'+num[0]+'话'
-        return num[0],sty,stz,stx
-    num=re.findall(r"E([0-9]{1,2})",name)
-    if len(num)!=0:
-        sty='第'+num[0]+'话'
-        stz="第XX话"
-        stx='第'+num[0]+'话'
-        return num[0],sty,stz,stx
-    num=re.findall(r"_([0-9]{1,2})_",name)
-    if len(num)!=0:
-        sty='_'+num[0]+'_'
-        stz="_XX_"
-        stx='_'+num[0]+'_'
-        return num[0],sty,stz,stx
-    num=re.findall(r"\[([0-9]{1,2})\D",name)
-    if len(num)!=0:
-        sty="\["+num[0]+"\]"
-        stz="[XX]"
-        stx="["+num[0]+"]"
-        return num[0],sty,stz,stx
-    num=re.findall(r"\D([0-9]{1,2})\]",name)
-    if len(num)!=0:
-        sty="\["+num[0]+"\]"
-        stz="[XX]"
-        stx="["+num[0]+"]"
-        return num[0],sty,stz,stx
-    num=re.findall(r"-([0-9]{1,2})\D",name)
-    if len(num)!=0:
-        sty='-'+num[0]
-        stz="-XX"
-        stx="-"+num[0]
-        return num[0],sty,stz,stx
-    num=re.findall(r"\D([0-9]{1,2})\D",name)
-    if len(num)!=0:
-        sty=num[0]
-        stz="XX"
-        stx=num[0]
-        return num[0],sty,stz,stx  
-    
-    num=re.findall(r"([0-9]{1,2})",name)
-    if len(num)!=0:
-        sty=num[0]
-        stz="XX"
-        stx=num[0]
-        return num[0],sty,stz,stx     
+    for i in range(2,0,-1):
+        num=re.findall(r" ([0-9]{"+str(i)+"}) ",name)
+        if len(num)!=0:
+            sty=" "+num[0]+" "
+            stz=" XX "
+            stx=" "+num[0]+" "
+            return num[0],sty,stz,stx
+        num=re.findall(r"第([0-9]{"+str(i)+"})話",name)
+        if len(num)!=0:
+            sty='第'+num[0]+'話'
+            stz="第XX話"
+            stx='第'+num[0]+'話'
+            return num[0],sty,stz,stx
+        num=re.findall(r"第([0-9]{"+str(i)+"})话",name)
+        if len(num)!=0:
+            sty='第'+num[0]+'话'
+            stz="第XX话"
+            stx='第'+num[0]+'话'
+            return num[0],sty,stz,stx
+        num=re.findall(r"E([0-9]{"+str(i)+"})",name)
+        if len(num)!=0:
+            sty='第'+num[0]+'话'
+            stz="第XX话"
+            stx='第'+num[0]+'话'
+            return num[0],sty,stz,stx
+        num=re.findall(r"_([0-9]{"+str(i)+"})_",name)
+        if len(num)!=0:
+            sty='_'+num[0]+'_'
+            stz="_XX_"
+            stx='_'+num[0]+'_'
+            return num[0],sty,stz,stx
+        num=re.findall(r"\[([0-9]{"+str(i)+"})\D",name)
+        if len(num)!=0:
+            sty="\["+num[0]+"\]"
+            stz="[XX]"
+            stx="["+num[0]+"]"
+            return num[0],sty,stz,stx
+        num=re.findall(r"\D([0-9]{"+str(i)+"})\]",name)
+        if len(num)!=0:
+            sty="\["+num[0]+"\]"
+            stz="[XX]"
+            stx="["+num[0]+"]"
+            return num[0],sty,stz,stx
+        num=re.findall(r"-([0-9]{"+str(i)+"})\D",name)
+        if len(num)!=0:
+            sty='-'+num[0]
+            stz="-XX"
+            stx="-"+num[0]
+            return num[0],sty,stz,stx
+        num=re.findall(r"\D([0-9]{"+str(i)+"})\D",name)
+        if len(num)!=0:
+            sty=num[0]
+            stz="XX"
+            stx=num[0]
+            return num[0],sty,stz,stx  
+        num=re.findall(r"([0-9]{"+str(i)+"})",name)
+        if len(num)!=0:
+            sty=num[0]
+            stz="XX"
+            stx=num[0]
+            return num[0],sty,stz,stx     
     return '-1','-1','XX','-1'
 
 def finddoubanurl(name):
     logger.info('正在寻找 '+name+' 的豆瓣链接，请稍等...')
     url_encode_name = quote(name.replace(' ',''))
     url='https://www.douban.com/search?q='+url_encode_name
     user_agent = 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/98.0.4758.102 Safari/537.36'
@@ -120,14 +120,16 @@
             logger.info('已确认 '+name+' 的Bangumi链接为:'+res+'\n')
             return res
     return ''
 
 def findeps(pathlist):
     eps=[]
     for path in pathlist:
+        if not os.path.exists(path):
+            continue
         ls = os.listdir(path)
         ls.sort()
         for i in ls:
             c_path = os.path.join(path, i)
             if (os.path.isdir(c_path)) or (i.startswith('.')) or (not(  os.path.splitext(i)[1].lower()== ('.mp4') or os.path.splitext(i)[1].lower()== ('.mkv')  or os.path.splitext(i)[1].lower()== ('.avi') or os.path.splitext(i)[1].lower()== ('.ts')    )):
                 continue
             epnum=int(findnum(i)[0])
@@ -140,14 +142,57 @@
     return eps
 
 
 
 
 
 class pathinfo(object):
+    def updatepath(self,newpath):
+        self.path=newpath
+        if self.path[-1]=='\\' or self.path[-1]=='/':
+            self.path=self.path[:-1]
+        if ('anime' in self.type.lower() or 'tv' in self.type.lower()):
+            if self.zeroday_name=='':
+                self.eps=findeps([self.path])
+            else:
+                self.eps=findeps([self.path,os.path.join(self.path,self.zeroday_name)])
+            if (len(self.eps)<1):
+                #raise Exception('路径'+pathid+' : '+self.infodict['path']+'中没找到视频文件')
+                logger.warning('路径'+self.pathid+' : '+self.infodict['path']+'中没找到任何视频文件,请检查或者联系开发者')
+            if len(self.eps)>0:
+                self.min=self.eps[0]
+                self.max=self.eps[-1]
+            else:
+                self.min=10000
+                self.max=-1000
+        if ('anime' in self.type or 'tv' in self.type):
+            if len(self.eps) == self.max-self.min+1:
+                self.lack=False
+            else:
+                self.lack=True
+            if self.lack:
+                self.lackeps=[]
+                for i in range(self.min,self.max+1):
+                    if not i in self.eps:
+                        self.lackeps.append(i)
+                logger.warning('识别到路径'+self.pathid+' 中资源存在部分集数缺失,缺失集数:'+str(self.lackeps))
+                res=100
+                while not(res==0 or res==1):
+                    res=input('识别到路径'+self.pathid+' 中资源存在部分集数缺失,缺失集数为:'+str(self.lackeps)+'。是否仍然继续发布？请回复选项对应的数字\n0:先不发布，退出程序 1:无视警告,仍然发布\n')
+                    try:
+                        res=int(res)
+                    except:
+                        res=100
+                    if not(res==0 or res==1):
+                        logger.warning('输入有误，请重新输入')
+                if res==0:
+                    logger.error('识别到路径'+self.pathid+' 中资源存在部分集数缺失,用户退出程序')
+                    raise ValueError ('识别到路径'+self.pathid+' 中资源存在部分集数缺失,用户退出程序')
+        #self.print()
+
     def __init__(self,pathid,infodict,sites,basic):
         self.pathid=pathid
         self.sites=[]
         self.exclusive=[]
         self.infodict=infodict
         self.max=1
         self.min=1
@@ -156,46 +201,40 @@
         for item in attr_must:
             if not item in infodict or infodict[item]==None:
                 logger.error('未识别'+pathid+' 中的'+item+'信息')
                 raise ValueError ('未识别'+pathid+' 中的'+item+'信息')
             else:
                 exec('self.'+item+'=infodict[item]')
                 exec('self.exist_'+item+'=True')
-
+        if self.path[-1]=='\\' or self.path[-1]=='/':
+            self.path=self.path[:-1]
         
 
         #可有可无的属性,后面写入配置文件
-        attr_disp=['type','collection','complete','enable','doubanurl','imdb_url','bgm_url','anidb_url','from_url','transfer']
+        attr_disp=['type','collection','enable','doubanurl','complete']
         for item in attr_disp:
             if not item in infodict or infodict[item]==None:
                 exec('self.'+item+'=""')
                 exec('infodict[item]=None')
                 exec('self.exist_'+item+'=False')
             else:
                 exec('self.'+item+'=infodict[item]')
                 exec('self.exist_'+item+'=True')
 
         #可有可无的属性,后面不写入配置文件
-        attr_disp=['video_type','video_format','audio_format','year','zeroday_name','exinfo','seasonnum','txt_info','audio_info','zeroday_path']
+        attr_disp=['video_type','video_format','audio_format','year','zeroday_name','exinfo','seasonnum','imdb_url','bgm_url','anidb_url','transfer','txt_info','audio_info','from_url','contenttail','contenthead','screenshot','small_descr']
         for item in attr_disp:
             if not item in infodict or infodict[item]==None:
                 exec('self.'+item+'=""')
                 exec('self.exist_'+item+'=False')
             else:
                 exec('self.'+item+'=infodict[item]')
                 exec('self.exist_'+item+'=True')
-        '''
-        if self.zeroday_path!='':
-            ls = os.listdir(self.zeroday_path)
-            for i in ls:
-                c_path=os.path.join(self.zeroday_path, i)
-                if (os.path.isdir(c_path)) or (i.startswith('.')) or (not(  os.path.splitext(i)[1].lower()== ('.mp4') or os.path.splitext(i)[1].lower()== ('.mkv')  or os.path.splitext(i)[1].lower()== ('.avi') or os.path.splitext(i)[1].lower()== ('.ts')    )):
-                    continue
-                filepath=move(c_path,self.path)
-        '''
+        
+        
         pathstr=os.path.basename(self.path)
         if (self.exist_chinesename and self.exist_englishname and self.exist_sub):
             if self.exinfo!='':
                 self.exinfo='['+self.exinfo+']'
             if self.seasonnum=='':
                 self.seasonnum=1
                 self.season='S01'
@@ -280,50 +319,49 @@
                 infodict['type']='movie'
             else:
                 logger.error(pathid+' 中type(资源类型)输入错误')
                 raise ValueError (pathid+' 中type(资源类型)输入错误')
 
 
         self.downloadpath=''
-        if not 'downloadpath' in infodict or infodict['downloadpath']==None:
-            if (self.collection or 'movie' in self.type) == 1 and ('new_folder' in basic and basic['new_folder']==0):
+        if not 'downloadpath' in infodict or infodict['downloadpath']==None or infodict['downloadpath']=='':
+            if (self.collection>0 or 'movie' in self.type.lower()) and ( (not 'new_folder' in basic) or str(basic['new_folder'])=='0' or basic['new_folder']==None or basic['new_folder']==''):
                 self.downloadpath=os.path.dirname( self.path)
             else:
                 self.downloadpath=self.path
         else:
             self.downloadpath=infodict['downloadpath']
 
         self.category=None
         if not 'category' in infodict or infodict['category']==None:
             self.category=None
         else:
             self.category=infodict['category']
 
-        if self.complete=='':
-            self.complete=0
-        else:
-            self.complete=int(self.complete)
 
         
         if ('anime' in self.type or 'tv' in self.type) and not self.exist_collection:
             res=100
             while not(res==0 or res==1):
-                res=input('未识别路径'+pathid+'的collection（资源是否按合集发布）信息,请重新输入选项对应的数字:\n0:发布单集,1:发布合集\n')
+                res=input('未识别路径'+pathid+'的collection（资源是否按合集发布）信息,请重新输入选项对应的数字:\n0:发布单集,1:发布合集,2:将未发布的资源按合集发布\n')
                 try:
                     res=int(res)
                 except:
                     res=100
-                if not(res==0 or res==1):
+                if not(res==0 or res==1 or res==2):
                     logger.warning('输入有误，请重新输入')
             if res==0:
                 self.collection =0
                 infodict['collection']=0
             elif res==1:
                 self.collection =1
                 infodict['collection']=1
+            elif res==2:
+                self.collection =2
+                infodict['collection']=2
             else:
                 logger.error('未识别路径'+pathid+'的collection（资源是否按合集发布）信息')
                 raise ValueError ('未识别路径'+pathid+'的collection（资源是否按合集发布）信息')
 
 
         if self.exist_enable:
             try:
@@ -344,15 +382,15 @@
         if self.exist_collection:
             try:
                 self.collection =int(self.collection)
             except:
                 logger.warning('未识别路径'+pathid+'的collection（资源是否以合集发布）信息,已设置为0（单集发布）')
                 self.collection =0
                 infodict['collection']=0
-            if not (self.collection==0 or self.collection==1):
+            if not (self.collection==0 or self.collection==1 or self.collection==2):
                 logger.warning('未识别路径'+pathid+'的collection（资源是否以合集发布）信息,已设置为0（单集发布）')
                 self.collection =0
                 infodict['collection']=0
         else:
             logger.warning('未识别路径'+pathid+'的collection（资源是否以合集发布）信息,已设置为0（单集发布）')
             self.collection =0
             infodict['collection']=0
@@ -378,35 +416,32 @@
             self.from_url = 'https://mikanani.me/'
             infodict['from_url']='https://mikanani.me/'
 
         if self.exist_complete:
             try:
                 self.complete =int(self.complete)
             except:
-                logger.warning('未识别路径'+pathid+'的complete(资源是否为完结)信息,已设置为0（未完结）')
-                self.complete =0
-                infodict['complete']=0
-            if not (self.complete==0 or self.complete==1):
-                logger.warning('未识别路径'+pathid+'的complete(资源是否为完结)信息,已设置为0（未完结）')
-                self.complete =0
-                infodict['complete']=0
+                logger.warning('未识别路径'+pathid+'的complete(资源是否为完结)信息,默认设置为0（未完结）')
+                self.complete =-1
+            if not (self.complete==0 or self.complete==1 or self.complete==-1):
+                logger.warning('未识别路径'+pathid+'的complete(资源是否为完结)信息,默认设置为0（未完结）')
+                self.complete =-1
         else:
-            logger.warning('未识别路径'+pathid+'的complete(资源是否为完结)信息,已设置为0（未完结）')
-            self.complete =0
-            infodict['complete']=0
+            logger.warning('未识别路径'+pathid+'的complete(资源是否为完结)信息,默认设置为0（未完结）')
+            self.complete =-1
             
 
 
         
         for siteitem in sites:
             if sites[siteitem].enable==0:
                 continue
             self.sites.append(siteitem)
             if (not siteitem in infodict) or (infodict[siteitem]==None):
-                logger.warning('未找到路径'+pathitem+'在'+siteitem+'的站点信息,已设置为10000（不发)')
+                logger.warning('未找到路径'+pathitem+'在'+siteitem+'的站点信息,已设置为不发')
                 exec('self.'+siteitem+'_done=[]')
                 exec('self.'+siteitem+'_max_done=10000')
                 exec('self.'+siteitem+'_min_done=-1')
                 infodict[siteitem]=None
             else:
                 exec('self.'+siteitem+'_done='+'str(infodict[siteitem]).split(",")')
                 exec('self.'+siteitem+'_max_done=-1')
@@ -420,52 +455,68 @@
                         exec('self.'+siteitem+'_min_done=self.'+siteitem+'_done[i]')
                 exec('self.'+siteitem+'_done.sort()')
         
         if 'exclusive' in infodict and infodict['exclusive']!=None:
             self.exclusive=infodict['exclusive'].split(",")
             self.exclusive=[i.strip().lower() for i in self.exclusive]
 
-
-        if ('anime' in self.type or 'tv' in self.type):
+        season_ch=''
+        season_ch=season_ch+'第'
+        if self.seasonnum==1:
+            season_ch=season_ch+'一'
+        elif self.seasonnum==2:
+            season_ch=season_ch+'二'
+        elif self.seasonnum==3:
+            season_ch=season_ch+'三'
+        elif self.seasonnum==4:
+            season_ch=season_ch+'四'
+        elif self.seasonnum==5:
+            season_ch=season_ch+'五'
+        elif self.seasonnum==6:
+            season_ch=season_ch+'六'
+        elif self.seasonnum==7:
+            season_ch=season_ch+'七'
+        elif self.seasonnum==8:
+            season_ch=season_ch+'八'
+        elif self.seasonnum==9:
+            season_ch=season_ch+'九'
+        elif self.seasonnum==10:
+            season_ch=season_ch+'十'
+        elif self.seasonnum==11:
+            season_ch=season_ch+'十一'
+        elif self.seasonnum==12:
+            season_ch=season_ch+'十二'
+        elif self.seasonnum==13:
+            season_ch=season_ch+'十三'
+        elif self.seasonnum==14:
+            season_ch=season_ch+'十四'
+        elif self.seasonnum==15:
+            season_ch=season_ch+'十五'
+        else:
+            season_ch=season_ch+str(self.seasonnum)
+        season_ch=season_ch+'季'
+        self.season_ch=season_ch
+        
+        if ('anime' in self.type.lower() or 'tv' in self.type.lower()):
+            
             
-            season_ch=''
-            season_ch=season_ch+'第'
-            if self.seasonnum==1:
-                season_ch=season_ch+'一'
-            elif self.seasonnum==2:
-                season_ch=season_ch+'二'
-            elif self.seasonnum==3:
-                season_ch=season_ch+'三'
-            elif self.seasonnum==4:
-                season_ch=season_ch+'四'
-            elif self.seasonnum==5:
-                season_ch=season_ch+'五'
-            elif self.seasonnum==6:
-                season_ch=season_ch+'六'
-            elif self.seasonnum==7:
-                season_ch=season_ch+'七'
-            elif self.seasonnum==8:
-                season_ch=season_ch+'八'
-            elif self.seasonnum==9:
-                season_ch=season_ch+'九'
-            elif self.seasonnum==10:
-                season_ch=season_ch+'十'
-            else:
-                season_ch=season_ch+str(self.seasonnum)
-            season_ch=season_ch+'季'
-            self.season_ch=season_ch
 
-            if self.zeroday_path=='':
+            if self.zeroday_name=='':
                 self.eps=findeps([self.path])
             else:
-                self.eps=findeps([self.path,self.zeroday_path])
-
-
-            self.min=self.eps[0]
-            self.max=self.eps[-1]
+                self.eps=findeps([self.path,os.path.join(self.path,self.zeroday_name)])
+            if (len(self.eps)<1):
+                #raise Exception('路径'+pathid+' : '+self.infodict['path']+'中没找到视频文件')
+                logger.warning('路径'+pathid+' : '+self.infodict['path']+'中没找到任何视频文件,请检查或者联系开发者')
+            if len(self.eps)>0:
+                self.min=self.eps[0]
+                self.max=self.eps[-1]
+            else:
+                self.min=10000
+                self.max=-10000
             '''
             if (not self.exist_bgm_url) and 'anime' in self.type:
                 if self.seasonnum>1:
                     self.bgm_url=findbgmurl(self.chinesename.strip()+' '+self.season_ch.strip())
                 else:
                     self.bgm_url=findbgmurl(self.chinesename.strip())
                 if self.bgm_url=='':
```

### Comparing `upload_machine-0.0.8/upload_machine/utils/seed_machine/seed_machine.py` & `upload_machine-0.0.80/upload_machine/utils/seed_machine/seed_machine.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from upload_machine.utils.pathinfo.pathinfo import findnum
 from upload_machine.utils.mediafile.mediafile import mediafile
 from upload_machine.utils.uploader.auto_upload import auto_upload
 from shutil import move
 from qbittorrentapi import Client
 import time
 import datetime
+import shutil
 
 
 def get_newhash(qbinfo):
     logger.info('正在查找最新发布的种子的hash...')
     logger.info('正在登录Qbittorrent WEBUI页面...')
     try:
         client = Client(host=qbinfo['qburl'],username=qbinfo['qbwebuiusername'],password=qbinfo['qbwebuipassword'])
@@ -86,73 +87,82 @@
             #发布过此集的站点略过
             if sites[siteitem].enable==1 and not( eval('pathinfo.'+siteitem+'_max_done==10000')) and not eval('pathep in pathinfo.'+siteitem+'_done'):
                 site_upload.append(sites[siteitem])
 
         #如果没有站点要发布就略过本集
         if len(site_upload)==0:
             continue
+        
 
         ls = os.listdir(pathinfo.path)
         filepath=''
         for i in ls:
             c_path=os.path.join(pathinfo.path, i)
             if (os.path.isdir(c_path)) or (i.startswith('.')) or (not(  os.path.splitext(i)[1].lower()== ('.mp4') or os.path.splitext(i)[1].lower()== ('.mkv')  or os.path.splitext(i)[1].lower()== ('.avi') or os.path.splitext(i)[1].lower()== ('.ts')    )):
                 continue
             if int(findnum(i)[0])==pathep:
                 filepath=c_path
                 break
         move_suc=0
         move_newpath=''
         move_oldpath=''
-        if filepath=='' and pathinfo.zeroday_path!='':
-            ls = os.listdir(pathinfo.zeroday_path)
+        filelist=[]
+        if filepath=='' and pathinfo.zeroday_name!='':
+            zeroday_path=os.path.join(pathinfo.path,pathinfo.zeroday_name)
+            ls = os.listdir(zeroday_path)
             filepath=''
             for i in ls:
-                c_path=os.path.join(pathinfo.zeroday_path, i)
+                c_path=os.path.join(zeroday_path, i)
                 if (os.path.isdir(c_path)) or (i.startswith('.')) or (not(  os.path.splitext(i)[1].lower()== ('.mp4') or os.path.splitext(i)[1].lower()== ('.mkv')  or os.path.splitext(i)[1].lower()== ('.avi') or os.path.splitext(i)[1].lower()== ('.ts')    )):
                     continue
                 if int(findnum(i)[0])==pathep:
                     move_oldpath=os.path.dirname(c_path)
                     filepath=move(c_path,pathinfo.path)
                     move_newpath=filepath
                     move_suc=1
                     break
-        
+    
         if filepath=='':
             logger.error('未找到文件夹'+pathinfo.path+'下第'+str(pathep)+'集资源')
             raise ValueError ('未找到文件夹'+pathinfo.path+'下第'+str(pathep)+'集资源')
 
         #获取file全部信息
         file1=mediafile(filepath,pathinfo,basic,imgdata)
-        if not pathinfo.imdb_url=='' and pathyaml['imdb_url']==None:
+        if not pathinfo.imdb_url=='' and ((not 'imdb_url' in pathyaml) or pathyaml['imdb_url']==None):
             pathyaml['imdb_url']=pathinfo.imdb_url
+        if file1.complete==1 and (not 'complete' in pathyaml or pathyaml['complete']==None or pathyaml['complete']==''):
+            pathyaml['complete']=1
+        
         
-        file1.getfullinfo()
         logger.info('正在发布路径'+pathinfo.path+'下第'+str(pathep)+'集资源:'+filepath)
+        logger.info('正在抓取资源信息,请稍后...')
+        file1.getfullinfo()
         for siteitem in site_upload:
             if siteitem.enable==0:
                 continue
             logger.info('正在'+siteitem.sitename+'站点发布路径'+pathinfo.chinesename+'第'+str(pathep)+'集资源')
-            
             upload_success=False
             uploadtime=0
+            #用模板获取mediainfo
+            file1.updatemediainfo(siteitem.mediainfo_template_file)
             while upload_success==False and uploadtime<3:
                 uploadtime=uploadtime+1
                 logger.info('第'+str(uploadtime)+'次尝试发布')
 
                 try:
                     upload_success,logstr=auto_upload(siteitem,file1,basic['record_path'],qbinfo,basic,hashlist)
                 except Exception as r:
                     logger.warning('发布资源发生错误，错误信息: %s' %(r))
                     upload_success=False
 
                 if not upload_success:
                     logger.warning(siteitem.sitename+'第'+str(uploadtime)+'次发布任务失败')
                     logger.warning(logstr)
-                    file1.mktorrent()
+                    #file1.mktorrent()
+                    file1.gettorrent()
 
             if not upload_success:
                 logger.warning(siteitem.sitename+'发布任务失败，本站暂停发种')
                 siteitem.enable=0
                 errornum=errornum+1
                 log_error=log_error+str(errornum)+':\t'+siteitem.sitename+'   \t'+logstr+'\n'
                 logger.warning(logstr)
@@ -172,22 +182,157 @@
                 exec('pathinfo.'+siteitem.sitename+'_done.append(pathep)')
                 exec('pathinfo.'+siteitem.sitename+'_done.sort()')
                 exec('pathyaml["'+siteitem.sitename+'"]=",".join([str(i) for i in pathinfo.'+siteitem.sitename+'_done])')
                 #deletetorrent(basic['screenshot_path'])
             #a=input('check')
             
         del(file1)
-        if move_suc==1 and 'new_folder' in basic and basic['new_folder']==0 and os.path.exists(move_newpath) and os.path.exists(move_oldpath):
+        if move_suc==1 and os.path.exists(move_newpath) and os.path.exists(move_oldpath):
+            logger.info('正在尝试将文件：'+move_newpath+'移动回原位：'+move_oldpath)
             try:
                 move_newpath=move(move_newpath,move_oldpath)
+                move_suc=0
             except Exception as r:
                 logger.warning('移动文件'+move_newpath+'到'+move_oldpath+'链接失败，原因: %s' %(r))
+            
     logger.info('路径'+pathinfo.path+'下资源已全部发布完毕')
     return log_error,log_succ
 
+
+#发布剩余合集
+def seedmachine_rest(pathinfo,sites,pathyaml,basic,qbinfo,imgdata,hashlist):
+    
+    #把没发布的集数转移到新建文件夹内
+    log_error=''
+    log_succ=''
+    logstr=''
+    #1.将没有发布过的资源移到新路径path_new
+    path_old=pathinfo.path
+    path_new=os.path.join(pathinfo.path,os.path.basename(pathinfo.path))
+    for siteitem in sites:
+        #发布过此集的站点略过
+        if sites[siteitem].enable!=1 or ( eval('pathinfo.'+siteitem+'_max_done==10000')):
+            continue
+        #收集需要发布的合集
+        eps=[]
+        for pathep in pathinfo.eps:
+            if  not eval('pathep in pathinfo.'+siteitem+'_done'):
+                eps.append(int (pathep))
+        if len(eps)<=0:
+            logger.info('正在'+siteitem+'站点发布路径'+path_old+'下无未发布分集,已跳过')
+            continue
+        
+        #新建文件夹
+        try:
+            os.mkdir(path_new)
+        except Exception as r:
+            logger.warning('新建文件夹发生错误,错误信息: %s' %(r))  
+            log_error=log_error+'路径'+path_old+'新建子文件夹'+path_new+'发生错误\n'
+            if os.path.exists(path_new):
+                logger.warning('路径 '+path_old+' 内已存在文件夹 '+path_new+'请更改此文件夹命名\n')
+            continue
+
+        ls = os.listdir(path_old)
+        for i in ls:
+            c_path=os.path.join(path_old, i)
+            if (os.path.isdir(c_path)) or (i.startswith('.')) or (not(  os.path.splitext(i)[1].lower()== ('.mp4') or os.path.splitext(i)[1].lower()== ('.mkv')  or os.path.splitext(i)[1].lower()== ('.avi') or os.path.splitext(i)[1].lower()== ('.ts')    )):
+                continue
+            if int(findnum(i)[0]) in eps:
+                shutil.move(c_path, path_new) 
+        if pathinfo.zeroday_name!='' and pathinfo.zeroday_name!=None and os.path.exists(os.path.join(path_old,pathinfo.zeroday_name)):
+            path_file=os.path.join(path_old,pathinfo.zeroday_name)
+            ls = os.listdir(path_file)
+            for i in ls:
+                c_path=os.path.join(path_file, i)
+                if (os.path.isdir(c_path)) or (i.startswith('.')) or (not(  os.path.splitext(i)[1].lower()== ('.mp4') or os.path.splitext(i)[1].lower()== ('.mkv')  or os.path.splitext(i)[1].lower()== ('.avi') or os.path.splitext(i)[1].lower()== ('.ts')    )):
+                    continue
+                if int(findnum(i)[0]) in eps:
+                    shutil.move(c_path, path_new)
+        #2.将path_new按照合集发布
+        if pathinfo.path!=path_new:
+            pathinfo.updatepath(path_new)
+        logger.info('正在'+siteitem+'站点发布路径'+path_old+'下没发布过的资源合集，分别为：'+str(eps))
+        
+        errornum=0
+        succnum=0
+        siteitem=sites[siteitem]
+        #获取file全部信息
+        file1=mediafile(path_new,pathinfo,basic,imgdata)
+        logger.info('正在抓取资源信息,请稍后...')
+        file1.getfullinfo()
+        if not pathinfo.imdb_url=='' and ((not 'imdb_url' in pathyaml) or pathyaml['imdb_url']==None):
+            pathyaml['imdb_url']=pathinfo.imdb_url
+        if file1.complete==1 and (not 'complete' in pathyaml or pathyaml['complete']==None or pathyaml['complete']==''):
+            pathyaml['complete']=1
+        #用模板获取mediainfo
+        file1.updatemediainfo(siteitem.mediainfo_template_file)
+
+        #3.把文件返回原位
+        
+        dst_path=path_old
+        if ('new_folder' in basic) and (str(basic['new_folder'])=='1' or str(basic['new_folder'])=='2') :
+            dst_path=os.path.join(path_old,os.path.basename(file1.topath))
+        if not os.path.exists(dst_path):
+            os.mkdir(dst_path)
+        ls = os.listdir(file1.topath)
+        for i in ls:
+            c_path=os.path.join(file1.topath, i)
+            if (os.path.isdir(c_path)) or (i.startswith('.')) or (not(  os.path.splitext(i)[1].lower()== ('.mp4') or os.path.splitext(i)[1].lower()== ('.mkv')  or os.path.splitext(i)[1].lower()== ('.avi') or os.path.splitext(i)[1].lower()== ('.ts')    )):
+                continue
+            shutil.move(c_path, dst_path) 
+        #4.删除path_new文件夹
+        shutil.rmtree(path_new)
+
+        upload_success=False
+        uploadtime=0
+        
+        while upload_success==False and uploadtime<3:
+            uploadtime=uploadtime+1
+            logger.info('第'+str(uploadtime)+'次尝试发布')
+            upload_success,logstr=auto_upload(siteitem,file1,basic['record_path'],qbinfo,basic,hashlist)
+            if not upload_success:
+                logger.warning(siteitem.sitename+'第'+str(uploadtime)+'次发布任务失败')
+                logger.warning(logstr)
+                #file1.mktorrent()
+                file1.gettorrent()
+        if not upload_success:
+            logger.warning(siteitem.sitename+'发布任务失败，本站暂停发种')
+            siteitem.enable=0
+            errornum=errornum+1
+            log_error=log_error+str(errornum)+':\t'+siteitem.sitename+'  \t'+logstr+'\n'
+            logger.warning(logstr)
+        elif '已存在' in  logstr:
+            errornum=errornum+1
+            log_error=log_error+str(errornum)+':\t'+siteitem.sitename+'   \t'+logstr+'\n'
+            logger.warning(logstr)
+            #记录已发布的种子
+            for epitem in eps:
+                exec('pathinfo.'+siteitem.sitename+'_done.append('+str(epitem)+')')
+            exec('pathinfo.'+siteitem.sitename+'_done=list(set('+'pathinfo.'+siteitem.sitename+'_done'+'))')
+            exec('pathinfo.'+siteitem.sitename+'_done.sort()')
+            exec('pathyaml["'+siteitem.sitename+'"]=",".join([str(i) for i in pathinfo.'+siteitem.sitename+'_done])')
+        else:
+            succnum=succnum+1
+            log_succ=log_succ+str(succnum)+':\t'+siteitem.sitename+'   \t'+logstr+'\n'
+            logger.info(logstr)
+            #记录已发布的种子
+            for epitem in eps:
+                exec('pathinfo.'+siteitem.sitename+'_done.append('+str(epitem)+')')
+            exec('pathinfo.'+siteitem.sitename+'_done=list(set('+'pathinfo.'+siteitem.sitename+'_done'+'))')
+            exec('pathinfo.'+siteitem.sitename+'_done.sort()')
+            exec('pathyaml["'+siteitem.sitename+'"]=",".join([str(i) for i in pathinfo.'+siteitem.sitename+'_done])')
+            #deletetorrent(basic['screenshot_path'])
+        #a=input('check')
+            
+        del(file1)  
+        logger.info(siteitem.sitename+'站点,路径'+path_old+'下资源合集发布完毕，分别为：'+str(eps))
+        
+    return log_error,log_succ
+    
+#发布合集
 def seedmachine(pathinfo,sites,pathyaml,basic,qbinfo,imgdata,hashlist):
     '''
     para:
         pathinfo
         sites 
         pathyaml 用于更新yaml中发布信息
         basic
@@ -209,59 +354,76 @@
     if len(site_upload)==0:
         logger.info('路径'+pathinfo.path+'下资源已全部发布完毕')
         return log_error,log_succ
 
 
     #获取file全部信息
     file1=mediafile(pathinfo.path,pathinfo,basic,imgdata)
-    if not pathinfo.imdb_url=='' and pathyaml['imdb_url']==None:
+    logger.info('正在抓取资源信息,请稍后...')
+    file1.getfullinfo()
+    if not pathinfo.imdb_url=='' and ((not 'imdb_url' in pathyaml) or pathyaml['imdb_url']==None):
         pathyaml['imdb_url']=pathinfo.imdb_url
+    if file1.complete==1 and (not 'complete' in pathyaml or pathyaml['complete']==None or pathyaml['complete']==''):
+        pathyaml['complete']=1
+        
 
-    logger.info('正在'+siteitem+'站点发布路径'+pathinfo.path+'下资源')
-    file1.getfullinfo()
+    logger.info('正在发布路径'+pathinfo.path+'下资源')
+    
 
     for siteitem in site_upload:
         if siteitem.enable==0:
             continue
         logger.info('正在'+siteitem.sitename+'站点发布'+pathinfo.chinesename+'资源')
         upload_success=False
         uploadtime=0
+        #用模板获取mediainfo
+        file1.updatemediainfo(siteitem.mediainfo_template_file)
         while upload_success==False and uploadtime<3:
             uploadtime=uploadtime+1
             logger.info('第'+str(uploadtime)+'次尝试发布')
-            print("正在准备登录"+siteitem.sitename)
 
 
             upload_success,logstr=auto_upload(siteitem,file1,basic['record_path'],qbinfo,basic,hashlist)
             if not upload_success:
                 logger.warning(siteitem.sitename+'第'+str(uploadtime)+'次发布任务失败')
                 logger.warning(logstr)
                 #file1.mktorrent()
+                file1.gettorrent()
 
         if not upload_success:
             logger.warning(siteitem.sitename+'发布任务失败，本站暂停发种')
             siteitem.enable=0
             errornum=errornum+1
             log_error=log_error+str(errornum)+':\t'+siteitem.sitename+'  \t'+logstr+'\n'
             logger.warning(logstr)
         elif '已存在' in  logstr:
             errornum=errornum+1
             log_error=log_error+str(errornum)+':\t'+siteitem.sitename+'   \t'+logstr+'\n'
             logger.warning(logstr)
             #记录已发布的种子
-            exec('pathinfo.'+siteitem.sitename+'_done.append(-1)')
-            exec('pathinfo.'+siteitem.sitename+'_done.sort()')
+            if not 'movie' in pathinfo.type.lower():
+                for epitem in pathinfo.eps:
+                    exec('pathinfo.'+siteitem.sitename+'_done.append('+str(epitem)+')')
+                exec('pathinfo.'+siteitem.sitename+'_done=list(set('+'pathinfo.'+siteitem.sitename+'_done'+'))')
+                exec('pathinfo.'+siteitem.sitename+'_done.sort()')
+            if pathinfo.complete==1:
+                exec('pathinfo.'+siteitem.sitename+'_done.append(-1)')
             exec('pathyaml["'+siteitem.sitename+'"]=",".join([str(i) for i in pathinfo.'+siteitem.sitename+'_done])')
         else:
             succnum=succnum+1
             log_succ=log_succ+str(succnum)+':\t'+siteitem.sitename+'   \t'+logstr+'\n'
             logger.info(logstr)
             #记录已发布的种子
-            exec('pathinfo.'+siteitem.sitename+'_done.append(-1)')
-            exec('pathinfo.'+siteitem.sitename+'_done.sort()')
+            if not 'movie' in pathinfo.type.lower():
+                for epitem in pathinfo.eps:
+                    exec('pathinfo.'+siteitem.sitename+'_done.append('+str(epitem)+')')
+                exec('pathinfo.'+siteitem.sitename+'_done=list(set('+'pathinfo.'+siteitem.sitename+'_done'+'))')
+                exec('pathinfo.'+siteitem.sitename+'_done.sort()')
+            if pathinfo.complete==1:
+                exec('pathinfo.'+siteitem.sitename+'_done.append(-1)')
             exec('pathyaml["'+siteitem.sitename+'"]=",".join([str(i) for i in pathinfo.'+siteitem.sitename+'_done])')
             #deletetorrent(basic['screenshot_path'])
         #a=input('check')
             
     del(file1)  
     logger.info('路径'+pathinfo.path+'下资源已全部发布完毕')
     return log_error,log_succ
@@ -274,14 +436,16 @@
     hashlist=[]
     for path in pathlist:
         if path.enable==0:
             logger.info('路径'+path.path+'的enable被设置为0，已忽略')
             continue
         if (path.type=='anime' or path.type=='tv') and path.collection==0:
             log_error,log_succ=seedmachine_single(path,sites,yamlinfo['path info'][path.pathid],yamlinfo['basic'],yamlinfo['qbinfo'],yamlinfo['image hosting'],hashlist)
+        elif (path.type=='anime' or path.type=='tv') and path.collection==2:
+            log_error,log_succ=seedmachine_rest(path,sites,yamlinfo['path info'][path.pathid],yamlinfo['basic'],yamlinfo['qbinfo'],yamlinfo['image hosting'],hashlist)
         else:
             log_error,log_succ=seedmachine(path,sites,yamlinfo['path info'][path.pathid],yamlinfo['basic'],yamlinfo['qbinfo'],yamlinfo['image hosting'],hashlist)
         write_yaml(yamlinfo)
         if not log_succ=='':
             log_allsucc=log_allsucc+log_succ+'\n'
             logger.info(log_succ)
         print('\n')
```

### Comparing `upload_machine-0.0.8/upload_machine/utils/site/site.py` & `upload_machine-0.0.80/upload_machine/utils/site/site.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,28 +6,39 @@
     def __init__(self,sitename,sitedict):
         self.sitename   = sitename
         self.exist_cookie=False
         self.exist_password=False
         self.uplver =1
         self.enable =0
         self.check = False
+        self.mediainfo_template_file=''
+        self.token='' #zhuque站点token
+        self.torrentkey='' #zhuque站点torrentkey
 
 
         try:
             self.uplver =int(sitedict['uplver'])
         except:
             logger.warning(sitename+'站点匿名发布uplver信息填错错误，已设置为1:默认匿名发布')
             self.uplver =1
             sitedict['uplver']=1
 
         if not (self.uplver==0 or self.uplver==1):
             logger.warning(sitename+'站点匿名发布uplver信息填错错误，已设置为1:默认匿名发布')
             self.uplver =1
             sitedict['uplver']=1
 
+        if 'mediainfo_template_file' in sitedict and sitedict['mediainfo_template_file']!= None and sitedict['mediainfo_template_file'].strip()!='':
+            if os.path.exists(sitedict['mediainfo_template_file']):
+                self.mediainfo_template_file=sitedict['mediainfo_template_file']
+            else:
+                raise Exception(sitename+'站点的mediainfo模板文件不存在')
+        else:
+            self.mediainfo_template_file=''
+
 
         try:
             self.enable =int(sitedict['enable'])
         except:
             logger.warning(sitename+'站点enable信息填错错误，已设置为0:关闭')
             self.enable =0
             sitedict['enable']=0
@@ -50,14 +61,28 @@
             self.exist_cookie=False
 
         if 'check' in sitedict :
             if str(sitedict['check']=='1'):
                 self.check=True
             else:
                 self.check=False
+        
+        if sitename=='zhuque':
+            if 'token' in sitedict :
+                self.token=sitedict['token']
+            else:
+                logger.warning('zhuque站点缺少x-csrf-token')
+            
+            if 'torrentkey' in sitedict :
+                self.torrentkey=sitedict['torrentkey']
+            else:
+                logger.warning('zhuque站点缺少torrentkey，将会导致无法做种')
+            
+
+
         if 'username' in sitedict and not sitedict['username']==None and 'password' in sitedict and not sitedict['password']==None:
             self.username   = sitedict['username']
             self.password   = sitedict['password']
             self.exist_password=True
 
         if self.enable==1 and (not self.exist_cookie and not self.exist_password):
             logger.error('未找到'+sitename+' 站点的cookie信息以及用户名密码信息，请至少填写一个')
```

### Comparing `upload_machine-0.0.8/upload_machine/utils/uploader/audience_upload.py` & `upload_machine-0.0.80/upload_machine/utils/uploader/audience_upload.py`

 * *Files 12% similar despite different names*

```diff
@@ -57,19 +57,19 @@
     logger.info('已成功选择编码为'+file1.Video_Format)
 
     #选择音频编码
     if file1.Audio_Format.upper()=='AAC':
         audiocodec_sel='6'
     elif 'DTS-HDMA' in file1.Audio_Format.upper() or 'DTS-HD MA' in file1.Audio_Format.upper():
         audiocodec_sel='19'
-    elif 'TrueHD Atmos' in file1.Audio_Format.upper():
+    elif 'TRUEHD ATMOS' in file1.Audio_Format.upper():
         audiocodec_sel='26'
     elif 'LPCM' in file1.Audio_Format.upper():
         audiocodec_sel='21'
-    elif 'TrueHD' in file1.Audio_Format.upper():
+    elif 'TRUEHD' in file1.Audio_Format.upper():
         audiocodec_sel='20'
     elif 'FLAC' in file1.Audio_Format.upper():
         audiocodec_sel='1'
     elif 'APE' in file1.Audio_Format.upper():
         audiocodec_sel='2'
     elif 'MP3' in file1.Audio_Format.upper():
         audiocodec_sel='23'
@@ -159,10 +159,22 @@
             "standard_sel": standard_sel,
             "team_sel": team_sel,
             "uplver": uplver,
             "tags[]": tags,
             }
 
     scraper=cloudscraper.create_scraper()
-    r = scraper.post(post_url, cookies=cookies_raw2jar(siteinfo.cookie),data=other_data, files=file_tup,timeout=time_out)
+    success_upload=0
+    try_upload=0
+    while success_upload==0:
+        try_upload+=1
+        if try_upload>5:
+            return False,fileinfo+' 发布种子发生请求错误,请确认站点是否正常运行'
+        logger.info('正在发布种子')
+        try:
+            r = scraper.post(post_url, cookies=cookies_raw2jar(siteinfo.cookie),data=other_data, files=file_tup,timeout=time_out)
+            success_upload=1
+        except Exception as r:
+            logger.warning('发布种子发生错误: %s' %(r))
+            success_upload=0
     
     return afterupload(r,fileinfo,record_path,siteinfo,file1,qbinfo,hashlist)
```

### Comparing `upload_machine-0.0.8/upload_machine/utils/uploader/auto_upload.py` & `upload_machine-0.0.80/upload_machine/utils/uploader/auto_upload.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,15 +5,25 @@
 from upload_machine.utils.uploader.pter_upload import pter_upload
 from upload_machine.utils.uploader.hhclub_upload import hhclub_upload
 from upload_machine.utils.uploader.lemonhd_upload import lemonhd_upload
 from upload_machine.utils.uploader.hdpt_upload import hdpt_upload
 from upload_machine.utils.uploader.wintersakura_upload import wintersakura_upload
 from upload_machine.utils.uploader.carpt_upload import carpt_upload
 from upload_machine.utils.uploader.hdfans_upload import hdfans_upload
-from upload_machine.utils.uploader.hare_upload import hare_upload
+from upload_machine.utils.uploader.hares_upload import hares_upload
+from upload_machine.utils.uploader.zmpt_upload import zmpt_upload
+from upload_machine.utils.uploader.hdvideo_upload import hdvideo_upload
+from upload_machine.utils.uploader.ihdbits_upload import ihdbits_upload
+from upload_machine.utils.uploader.redleaves_upload import redleaves_upload
+from upload_machine.utils.uploader.mteam_upload import mteam_upload
+from upload_machine.utils.uploader.sharkpt_upload import sharkpt_upload
+from upload_machine.utils.uploader.zhuque_upload import zhuque_upload
+from upload_machine.utils.uploader.dajiao_upload import dajiao_upload
+from upload_machine.utils.uploader.pandapt_upload import pandapt_upload
+from upload_machine.utils.uploader.rousi_upload import rousi_upload
 
 
 
 
 
 def auto_upload(siteitem,file,record_path,qbinfo,basic,hashlist):
     return eval(siteitem.sitename+'_upload(siteitem,file,record_path,qbinfo,basic,hashlist)')
```

### Comparing `upload_machine-0.0.8/upload_machine/utils/uploader/carpt_upload.py` & `upload_machine-0.0.80/upload_machine/utils/uploader/hdsky_upload.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,182 +1,223 @@
 from loguru import logger
 import time
 import os
 from upload_machine.utils.uploader.upload_tools import *
 import re
 import cloudscraper
 
-def carpt_upload(siteinfo,file1,record_path,qbinfo,basic,hashlist):
-    post_url = "https://carpt.net/takeupload.php"
+def hdsky_upload(siteinfo,file1,record_path,qbinfo,basic,hashlist):
+    post_url = "https://hdsky.me/takeupload.php"
     tags=[]
     time_out=40
     if (file1.pathinfo.type=='anime' or file1.pathinfo.type=='tv') and file1.pathinfo.collection==0:
         fileinfo=file1.chinesename+'在'+siteinfo.sitename+'第'+file1.episodename+'集'
     else:
         fileinfo=file1.chinesename+'在'+siteinfo.sitename
 
 
     #选择类型
     if 'anime' in file1.pathinfo.type.lower():
-        select_type='403'
-    elif 'tv' in file1.pathinfo.type.lower():
-        select_type='402'
+        select_type='405'
+    elif 'tv' in file1.pathinfo.type.lower() and file1.pathinfo.collection>=1:
+        if '大陆' in file1.country or '香港' in file1.country or '台湾' in file1.country:
+            select_type='411'
+        else:
+            select_type='413'
+    elif 'tv' in file1.pathinfo.type.lower() and file1.pathinfo.collection==0:
+        if '大陆' in file1.country or '香港' in file1.country or '台湾' in file1.country:
+            select_type='402'
+        else:
+            select_type='412'
     elif 'movie' in file1.pathinfo.type.lower():
         select_type='401'
-    elif 'show' in file1.pathinfo.type.lower():
-        select_type='405'
-    elif 'doc' in file1.pathinfo.type.lower():
-        select_type='404'
-    elif 'sport' in file1.pathinfo.type.lower():
-        select_type='407'
-    elif 'mv' in file1.pathinfo.type.lower():
-        select_type='407'
-    elif 'music' in file1.pathinfo.type.lower():
-        select_type='406'
-    elif 'cartoon' in file1.pathinfo.type.lower():
-        select_type='403'
     else:
-        select_type='407'
+        select_type='409'
     logger.info('已成功填写类型为'+file1.pathinfo.type)
 
-    #选择媒介
+
+    #选择来源 
     if file1.type=='WEB-DL':
-        medium_sel='2'
-    elif 'webrip' in file1.type.lower():
-        medium_sel='1'
-    elif 'dvdrip' in file1.type.lower():
-        medium_sel='4'
-    elif 'rip' in file1.type.lower():
-        medium_sel='1'
-    elif 'hdtv'in file1.type.lower():
+        medium_sel='11'
+    elif 'rip' in file1.type.lower() or file1.type=='bluray'  :
+        medium_sel='7'
+    elif file1.type=='HDTV':
+        medium_sel='5'
+    elif file1.type=='remux':
         medium_sel='3'
-    elif 'remux' in file1.type.lower():
-        medium_sel='6'
     else:
-        medium_sel='6'
+        medium_sel='7'
     logger.info('已成功选择质量为'+file1.type)
    
 
 
     #选择编码
     if file1.Video_Format=='H264':
         codec_sel='1'
     elif file1.Video_Format=='x264':
-        codec_sel='1'
+        codec_sel='10'
     elif file1.Video_Format=='H265':
-        codec_sel='2'
+        codec_sel='12'
     elif file1.Video_Format=='x265':
-        codec_sel='2'
+        codec_sel='13'
     else:
         codec_sel='1'
     logger.info('已成功选择编码为'+file1.Video_Format)
 
     #选择音频编码
     if file1.Audio_Format.upper()=='AAC':
-        audiocodec_sel='7'
-    elif 'DTS-HDMA' in file1.Audio_Format.upper() or 'DTS-HD MA' in file1.Audio_Format.upper():
-        audiocodec_sel='2'
-    elif 'TrueHD Atmos' in file1.Audio_Format.upper():
-        audiocodec_sel='1'
+        audiocodec_sel='6'
+    elif 'DTS-HDMA:X 7.1' in file1.Audio_Format.upper():
+        audiocodec_sel='16'
+    elif 'DTS-HDMA' in file1.Audio_Format.upper():
+        audiocodec_sel='10'
+    elif 'TRUEHD ATMOS' in file1.Audio_Format.upper():
+        audiocodec_sel='17'
     elif 'LPCM' in file1.Audio_Format.upper():
-        audiocodec_sel='4'
-    elif 'TrueHD' in file1.Audio_Format.upper():
-        audiocodec_sel='1'
+        audiocodec_sel='13'
+    elif 'TRUEHD' in file1.Audio_Format.upper():
+        audiocodec_sel='11'
+    elif 'DTS-HD HR' in file1.Audio_Format.upper():
+        audiocodec_sel='14'
+    elif 'PCM' in file1.Audio_Format.upper():
+        audiocodec_sel='19'
     elif 'FLAC' in file1.Audio_Format.upper():
-        audiocodec_sel='5'
+        audiocodec_sel='1'
     elif 'APE' in file1.Audio_Format.upper():
-        audiocodec_sel='8'
+        audiocodec_sel='2'
     elif 'MP3' in file1.Audio_Format.upper():
-        audiocodec_sel='6'
+        audiocodec_sel='4'
+    elif 'OGG' in file1.Audio_Format.upper():
+        audiocodec_sel='5'
     elif 'AC3' in file1.Audio_Format.upper() or 'DD' in file1.Audio_Format.upper():
-        audiocodec_sel='3'
-    elif 'DTS:X' in file1.Audio_Format.upper() or 'DTS-X' in file1.Audio_Format.upper():
-        audiocodec_sel='2'
+        audiocodec_sel='12'
     elif 'DTS' in file1.Audio_Format.upper():
-        audiocodec_sel='2'
+        audiocodec_sel='3'
     elif 'WAV' in file1.Audio_Format.upper():
-        audiocodec_sel='9'
-    elif 'M4A' in file1.Audio_Format.upper():
-        audiocodec_sel='9'
+        audiocodec_sel='15'
+    elif 'DSD' in file1.Audio_Format.upper():
+        audiocodec_sel='18'
+    elif 'Dolby Digital Plus Dolby Atmos' in file1.Audio_Format.upper():
+        audiocodec_sel='21'
+    elif 'Dolby Digital Plus' in file1.Audio_Format.upper():
+        audiocodec_sel='20'
     else:
-        audiocodec_sel='9'
+        audiocodec_sel='7'
     logger.info('已成功选择音频编码为'+file1.Audio_Format.upper())
 
     #选择分辨率
-    if '8K' in file1.standard_sel:
-        standard_sel='1'
-    elif '2160' in file1.standard_sel:
-        standard_sel='1'
+    if '2160' in file1.standard_sel:
+        standard_sel='5'
     elif '1080p' in file1.standard_sel.lower():
-        standard_sel='2'
+        standard_sel='1'
     elif '1080i' in file1.standard_sel.lower():
         standard_sel='2'
     elif '720' in file1.standard_sel:
         standard_sel='3'
     elif '480' in file1.standard_sel:
         standard_sel='4'
     else:
-        standard_sel='5'
+        standard_sel='1'
     logger.info('已成功选择分辨率为'+file1.standard_sel)
     
 
     #选择制作组
-    if 'CARPT' in file1.sub.upper():
+    if 'HDSKY' in file1.sub.upper():
+        team_sel='6'
+        tags.append(12)
+    elif 'HDS3D' in file1.sub.upper():
+        team_sel='28'
+        tags.append(12)
+    elif 'HDSTV' in file1.sub.upper():
+        team_sel='9'
+        tags.append(12)
+    elif 'HDSWEB' in file1.sub.upper() and file1.pathinfo.collection>=1:
+        team_sel='35'
+        tags.append(12)
+    elif 'HDSWEB' in file1.sub.upper():
+        team_sel='31'
+        tags.append(12)
+    elif 'HDSPAD' in file1.sub.upper():
+        team_sel='18'
+        tags.append(12)
+    elif 'HDSCD' in file1.sub.upper():
+        team_sel='22'
+        tags.append(12)
+    elif 'hdspecial' in file1.sub.lower():
+        team_sel='34'
+        tags.append(12)
+    elif 'BMDRU' in file1.sub.upper():
+        team_sel='30'
+        tags.append(12)
+    elif 'AREA11' in file1.sub.upper():
+        team_sel='25'
+        tags.append(12)
+    elif 'HDSAB' in file1.sub.upper():
+        team_sel='36'
+        tags.append(12)
+    elif 'HDS' in file1.sub.upper():
         team_sel='1'
-    elif 'WIKI' in file1.sub.upper():
-        team_sel='2'
-    elif 'CMCT' in file1.sub.upper():
-        team_sel='3'
-    elif 'M-TEAM' in file1.sub.upper() or 'MTEAM' in file1.sub.upper():
-        team_sel='4'
+        tags.append(12)
+    elif file1.transfer==0:
+        team_sel='24'
+    elif file1.transfer==1:
+        team_sel='27'
     else:
-        team_sel='5'
+        team_sel='27'
     logger.info('制作组已成功选择为'+file1.sub)
     
-    if 'carpt' in file1.sub.lower():
-        tags.append(3)
-        logger.info('已选择官方')
-    if 'carpt' in file1.pathinfo.exclusive :
-        tags.append(1)
-        logger.info('已选择禁转')
+    if 'hdsky' in file1.pathinfo.exclusive :
+        tags.append(2)
     if '国' in file1.language or '中' in file1.language:
         tags.append(5)
-        logger.info('已选择国语')
     if not file1.sublan=='' and ('简' in file1.sublan or '繁' in file1.sublan or '中' in file1.sublan):
         tags.append(6)
-        logger.info('已选择中字')
-
-    
+    if file1.transfer==0:
+        tags.append(14)
     tags=list(set(tags))
     tags.sort()
-    
     if siteinfo.uplver==1:
         uplver='yes'
     else:
         uplver='no'
 
     torrent_file = file1.torrentpath
     file_tup = ("file", (os.path.basename(torrent_file), open(torrent_file, 'rb'), 'application/x-bittorrent')),
             
 
     other_data = {
             "name": file1.uploadname,
             "small_descr": file1.small_descr+file1.pathinfo.exinfo,
-            "url" : file1.imdburl,
+            "url": file1.imdburl,
+            "url_douban": file1.doubanurl,
+            "nfo": "",
             "color": "0",
             "font": "0",
             "size": "0",
             "descr": file1.content,
             "type": select_type,
             "medium_sel": medium_sel,
             "codec_sel": codec_sel,
             "audiocodec_sel": audiocodec_sel,
             "standard_sel": standard_sel,
             "team_sel": team_sel,
             "uplver": uplver,
-            "tags[]": tags,
+            "option_sel[]": tags,
             }
 
     scraper=cloudscraper.create_scraper()
-    r = scraper.post(post_url, cookies=cookies_raw2jar(siteinfo.cookie),data=other_data, files=file_tup,timeout=time_out)
+    success_upload=0
+    try_upload=0
+    while success_upload==0:
+        try_upload+=1
+        if try_upload>5:
+            return False,fileinfo+' 发布种子发生请求错误,请确认站点是否正常运行'
+        logger.info('正在发布种子')
+        try:
+            r = scraper.post(post_url, cookies=cookies_raw2jar(siteinfo.cookie),data=other_data, files=file_tup,timeout=time_out)
+            success_upload=1
+        except Exception as r:
+            logger.warning('发布种子发生错误: %s' %(r))
+            success_upload=0
     
+
     return afterupload(r,fileinfo,record_path,siteinfo,file1,qbinfo,hashlist)
```

### Comparing `upload_machine-0.0.8/upload_machine/utils/uploader/hare_upload.py` & `upload_machine-0.0.80/upload_machine/utils/uploader/dajiao_upload.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from loguru import logger
 import time
 import os
 from upload_machine.utils.uploader.upload_tools import *
 import re
 import cloudscraper
 
-def hare_upload(siteinfo,file1,record_path,qbinfo,basic,hashlist):
-    post_url = "https://club.hares.top/takeupload.php"
+def dajiao_upload(siteinfo,file1,record_path,qbinfo,basic,hashlist):
+    post_url = "https://dajiao.cyou/takeupload.php"
     tags=[]
     time_out=40
     if (file1.pathinfo.type=='anime' or file1.pathinfo.type=='tv') and file1.pathinfo.collection==0:
         fileinfo=file1.chinesename+'在'+siteinfo.sitename+'第'+file1.episodename+'集'
     else:
         fileinfo=file1.chinesename+'在'+siteinfo.sitename
 
 
     #选择类型
     if 'anime' in file1.pathinfo.type.lower():
         select_type='405'
-    elif 'tv' in file1.pathinfo.type.lower() and file1.pathinfo.collection==1:
+    elif 'tv' in file1.pathinfo.type.lower() and file1.pathinfo.collection>=1:
         if '大陆' in file1.country or '香港' in file1.country or '台湾' in file1.country:
             select_type='402'
         else:
             select_type='402'
     elif 'tv' in file1.pathinfo.type.lower() and file1.pathinfo.collection==0:
         if '大陆' in file1.country or '香港' in file1.country or '台湾' in file1.country:
             select_type='402'
@@ -31,193 +31,164 @@
     elif 'movie' in file1.pathinfo.type.lower():
         select_type='401'
     elif 'show' in file1.pathinfo.type.lower():
         select_type='403'
     elif 'doc' in file1.pathinfo.type.lower():
         select_type='404'
     elif 'mv' in file1.pathinfo.type.lower():
-        select_type='406'
+        select_type='415'
     elif 'sport' in file1.pathinfo.type.lower():
-        select_type='407'
+        select_type='417'
     elif 'music' in file1.pathinfo.type.lower():
-        select_type='415'
+        select_type='409'
     else:
-        select_type='415'
+        select_type='405'
     logger.info('已成功填写类型为'+file1.pathinfo.type)
 
 
+    source_sel='24'
+    #选择来源
+    if 'web' in file1.type.lower() and 'dl' in file1.type.lower():
+        source_sel='24'
+    elif (file1.type=='bluray') and '2160' in file1.standard_sel:
+        source_sel='23'
+    elif file1.type=='bluray':
+        source_sel='22'
+    elif 'rip' in file1.type.lower() and  'web' in file1.type.lower():
+        source_sel='24'
+    elif 'dvd' in file1.type.lower():
+        source_sel='25'
+    elif 'rip' in file1.type.lower()  :
+        source_sel='22'
+    elif 'HDTV' in file1.type.upper() and '2160' in file1.standard_sel:
+        source_sel='26'
+    elif 'HDTV' in file1.type.upper():
+        source_sel='26'
+    elif 'remux' in file1.type.lower():
+        source_sel='22'
+    else:
+        source_sel='28'
+    logger.info('已成功填写来源为'+file1.type)
+
+
     #选择媒介
-    if 'web' in file1.type.lower():
-        medium_sel='5'
+    if 'web' in file1.type.lower() and 'dl' in file1.type.lower():
+        medium_sel='10'
     elif (file1.type=='bluray') and '2160' in file1.standard_sel:
         medium_sel='1'
     elif file1.type=='bluray':
-        medium_sel='2'
-    elif 'rip' in file1.type.lower()  :
-        medium_sel='4'
-    elif file1.type=='HDTV' and '2160' in file1.standard_sel:
+        medium_sel='1'
+    elif 'rip' in file1.type.lower() and  'dvd' in file1.type.lower():
         medium_sel='6'
-    elif file1.type=='HDTV':
-        medium_sel='8'
-    elif file1.type=='remux':
+    elif 'rip' in file1.type.lower()  :
+        medium_sel='7'
+    elif 'HDTV' in file1.type.upper() and '2160' in file1.standard_sel:
+        medium_sel='5'
+    elif 'HDTV' in file1.type.upper():
+        medium_sel='5'
+    elif 'remux' in file1.type.lower():
         medium_sel='3'
+    elif 'dvd' in file1.type.lower():
+        medium_sel='2'
     else:
-        medium_sel='5'
+        medium_sel='10'
     logger.info('已成功填写来源为'+file1.type)
-   
+
 
 
     #选择编码
     if file1.Video_Format=='H264':
         codec_sel='1'
     elif file1.Video_Format=='x264':
-        codec_sel='8'
+        codec_sel='1'
     elif file1.Video_Format=='H265':
         codec_sel='6'
     elif file1.Video_Format=='x265':
-        codec_sel='7'
+        codec_sel='6'
     else:
         codec_sel='1'
     logger.info('已成功选择编码为'+file1.Video_Format)
 
     #选择音频编码
     if file1.Audio_Format.upper()=='AAC':
         audiocodec_sel='6'
     elif 'DTS-HDMA' in file1.Audio_Format.upper() or 'DTS-HD MA' in file1.Audio_Format.upper():
         audiocodec_sel='11'
-    elif 'TrueHD Atmos' in file1.Audio_Format.upper():
+    elif 'TRUEHD ATMOS' in file1.Audio_Format.upper():
         audiocodec_sel='8'
-    elif 'LPCM' in file1.Audio_Format.upper():
+    elif 'PCM' in file1.Audio_Format.upper():
         audiocodec_sel='14'
-    elif 'TrueHD' in file1.Audio_Format.upper():
+    elif 'TRUEHD' in file1.Audio_Format.upper():
         audiocodec_sel='9'
     elif 'FLAC' in file1.Audio_Format.upper():
         audiocodec_sel='1'
     elif 'APE' in file1.Audio_Format.upper():
         audiocodec_sel='2'
     elif 'MP3' in file1.Audio_Format.upper():
         audiocodec_sel='4'
     elif 'AC3' in file1.Audio_Format.upper() or 'AC-3' in file1.Audio_Format.upper() or 'DD' in file1.Audio_Format.upper():
-        audiocodec_sel='8'
+        audiocodec_sel='13'
+    elif 'EAC3' in file1.Audio_Format.upper() or 'EAC-3' in file1.Audio_Format.upper() or 'DDP' in file1.Audio_Format.upper():
+        audiocodec_sel='13'
     elif 'DTS:X' in file1.Audio_Format.upper() or 'DTS-X' in file1.Audio_Format.upper():
-        audiocodec_sel='3'
+        audiocodec_sel='10'
     elif 'DTS' in file1.Audio_Format.upper():
         audiocodec_sel='3'
-    elif 'MP3' in file1.Audio_Format.upper():
-        audiocodec_sel='4'
     elif 'WAV' in file1.Audio_Format.upper():
-        audiocodec_sel='15'
+        audiocodec_sel='7'
+    elif 'M4A' in file1.Audio_Format.upper():
+        audiocodec_sel='7'
     elif 'OGG' in file1.Audio_Format.upper():
         audiocodec_sel='5'
     else:
         audiocodec_sel='7'
     logger.info('已成功选择音频编码为'+file1.Audio_Format.upper())
 
     #选择分辨率
     if '8K' in file1.standard_sel:
-        standard_sel='5'
+        standard_sel='6'
     elif '2160' in file1.standard_sel:
         standard_sel='6'
     elif '1080p' in file1.standard_sel.lower():
         standard_sel='1'
     elif '1080i' in file1.standard_sel.lower():
         standard_sel='2'
     elif '720' in file1.standard_sel:
         standard_sel='3'
-    elif '1440' in file1.standard_sel:
+    elif '480' in file1.standard_sel:
         standard_sel='7'
     else:
-        standard_sel='1'
+        standard_sel='8'
     logger.info('已成功选择分辨率为'+file1.standard_sel)
     
-    #选择地区
-    if not file1.country=='':
-        if '大陆' in file1.country:
-            processing_sel='1'
-            logger.info('国家信息已选择'+file1.country)
-        elif '香港' in file1.country:
-            processing_sel='2'
-            logger.info('国家信息已选择'+file1.country)
-        elif '台湾' in file1.country:
-            processing_sel='3'
-            logger.info('国家信息已选择'+file1.country)
-        elif '美国' in file1.country:
-            processing_sel='4'
-            logger.info('国家信息已选择'+file1.country)
-        elif '英国' in file1.country:
-            processing_sel='4'
-            logger.info('国家信息已选择'+file1.country)
-        elif '法国' in file1.country:
-            processing_sel='4'
-            logger.info('国家信息已选择'+file1.country)
-        elif '韩国' in file1.country:
-            processing_sel='7'
-            logger.info('国家信息已选择'+file1.country)
-        elif '日本' in file1.country:
-            processing_sel='7'
-            logger.info('国家信息已选择'+file1.country)
-        elif '印度' in file1.country:
-            processing_sel='9'
-            logger.info('国家信息已选择'+file1.country)
-        else:
-            processing_sel='10'
-            logger.info('未找到资源国家信息，已选择其他')
-    else:
-        processing_sel='10'
-        logger.info('未找到资源国家信息，已默认其他')
-
     #选择制作组
-    if 'HARESWEB' in file1.sub.upper():
+    if 'DJWEB' in file1.sub.upper():
+        team_sel='1'
+    elif 'DJTV' in file1.sub.upper():
         team_sel='2'
-    elif 'HARESTV' in file1.sub.upper():
+    elif 'DJZB' in file1.sub.upper():
         team_sel='3'
-    elif 'HARES' in file1.sub.upper():
-        team_sel='1'
-    elif 'CHD' in file1.sub.upper():
-        team_sel='4'
-    elif 'HDS' in file1.sub.upper():
-        team_sel='5'
-    elif 'WIKI' in file1.sub.upper():
+    elif 'CatEDU' in file1.sub.upper():
         team_sel='6'
-    elif 'CMCT' in file1.sub.upper():
+    elif 'Zaxyzit' in file1.sub.upper():
         team_sel='8'
-    elif 'BEAST' in file1.sub.upper():
-        team_sel='9'
-    elif 'HDC' in file1.sub.upper():
-        team_sel='10'
-    elif 'FRDS' in file1.sub.upper():
-        team_sel='11'
-    elif 'PTER' in file1.sub.upper():
-        team_sel='12'
-    elif 'BHD' in file1.sub.upper():
-        team_sel='13'
-    elif 'PTH' in file1.sub.upper():
-        team_sel='14'
     else:
-        team_sel='15'
+        team_sel='7'
     logger.info('制作组已成功选择为'+file1.sub)
     
-    if 'hare' in file1.pathinfo.exclusive :
+
+    if 'dajiao' in file1.pathinfo.exclusive :
         tags.append(1)
         logger.info('已选择禁转')
-    if 'HARES' in file1.sub.upper():
-        tags.append(3)
-        logger.info('已选择官方')
-    if file1.pathinfo.transfer==0:
-        tags.append(4)
-        logger.info('已选择原创')
     if '国' in file1.language or '中' in file1.language:
-        tags.append(6)
+        tags.append(5)
         logger.info('已选择国语')
     if not file1.sublan=='' and ('简' in file1.sublan or '繁' in file1.sublan or '中' in file1.sublan):
-        tags.append(9)
+        tags.append(6)
         logger.info('已选择中字')
-    if (file1.pathinfo.type=='anime' or file1.pathinfo.type=='tv') and file1.pathinfo.complete==0:
-        tags.append(16)
-        logger.info('已选择追更')
 
     
     tags=list(set(tags))
     tags.sort()
     
     if siteinfo.uplver==1:
         uplver='yes'
@@ -225,34 +196,42 @@
         uplver='no'
 
     torrent_file = file1.torrentpath
     file_tup = ("file", (os.path.basename(torrent_file), open(torrent_file, 'rb'), 'application/x-bittorrent')),
             
 
     other_data = {
-            "name": file1.uploadname.replace('  ',' ').replace(' ','.'),
+            "name": file1.uploadname,
             "small_descr": file1.small_descr+file1.pathinfo.exinfo,
-            "pt_gen[douban][link]": file1.doubanurl,
-            "pt_gen[imdb][link]" : file1.imdburl,
-            "pt_gen[bangumi][link]" : file1.bgmurl,
-            "url_poster" : re.findall(r'\[img\](.*)\[/img\]',file1.douban_info),
-            "screenshots" : file1.screenshoturl.replace('[img]','').replace('[/img]',''),
+            "url": file1.imdburl,
+            "pt_gen": file1.doubanurl,
             "color": "0",
             "font": "0",
             "size": "0",
-            "descr": file1.douban_info,
-            "technical_info" : file1.mediainfo,
+            "descr": file1.pathinfo.contenthead+'\n'+file1.douban_info+'\n'+file1.screenshoturl+'\n'+file1.pathinfo.contenttail,
+            "technical_info": file1.mediainfo,
             "type": select_type,
-            "medium_sel": medium_sel,
-            "codec_sel": codec_sel,
-            "audiocodec_sel": audiocodec_sel,
-            "standard_sel": standard_sel,
-            "processing_sel" : processing_sel,
-            "team_sel": team_sel,
+            "medium_sel[4]": medium_sel,
+            "codec_sel[4]": codec_sel,
+            "standard_sel[4]": standard_sel,
+            "team_sel[4]": team_sel,
+            "audiocodec_sel[4]": audiocodec_sel,
             "uplver": uplver,
-            "tags[]": tags,
+            "tags[4][]": tags,
             }
 
     scraper=cloudscraper.create_scraper()
-    r = scraper.post(post_url, cookies=cookies_raw2jar(siteinfo.cookie),data=other_data, files=file_tup,timeout=time_out)
+    success_upload=0
+    try_upload=0
+    while success_upload==0:
+        try_upload+=1
+        if try_upload>5:
+            return False,fileinfo+' 发布种子发生请求错误,请确认站点是否正常运行'
+        logger.info('正在发布种子')
+        try:
+            r = scraper.post(post_url, cookies=cookies_raw2jar(siteinfo.cookie),data=other_data, files=file_tup,timeout=time_out)
+            success_upload=1
+        except Exception as r:
+            logger.warning('发布种子发生错误: %s' %(r))
+            success_upload=0
     
     return afterupload(r,fileinfo,record_path,siteinfo,file1,qbinfo,hashlist)
```

### Comparing `upload_machine-0.0.8/upload_machine/utils/uploader/hdfans_upload.py` & `upload_machine-0.0.80/upload_machine/utils/uploader/hdfans_upload.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,19 +65,19 @@
     logger.info('已成功选择编码为'+file1.Video_Format)
 
     #选择音频编码
     if file1.Audio_Format.upper()=='AAC':
         audiocodec_sel='11'
     elif 'DTS-HDMA' in file1.Audio_Format.upper() or 'DTS-HD MA' in file1.Audio_Format.upper():
         audiocodec_sel='4'
-    elif 'TrueHD Atmos' in file1.Audio_Format.upper():
+    elif 'TRUEHD ATMOS' in file1.Audio_Format.upper():
         audiocodec_sel='1'
     elif 'LPCM' in file1.Audio_Format.upper():
         audiocodec_sel='7'
-    elif 'TrueHD' in file1.Audio_Format.upper():
+    elif 'TRUEHD' in file1.Audio_Format.upper():
         audiocodec_sel='6'
     elif 'FLAC' in file1.Audio_Format.upper():
         audiocodec_sel='12'
     elif 'APE' in file1.Audio_Format.upper():
         audiocodec_sel='13'
     elif 'MP3' in file1.Audio_Format.upper():
         audiocodec_sel='17'
@@ -222,24 +222,36 @@
     other_data = {
             "name": file1.uploadname,
             "small_descr": file1.small_descr+file1.pathinfo.exinfo,
             "url" : file1.imdburl,
             "color": "0",
             "font": "0",
             "size": "0",
-            "descr": file1.douban_info+'\n'+file1.screenshoturl,
+            "descr": file1.pathinfo.contenthead+'\n'+file1.douban_info+'\n'+file1.screenshoturl+'\n'+file1.pathinfo.contenttail,
             "technical_info" : file1.mediainfo,
             "type": select_type,
             "medium_sel": medium_sel,
             "codec_sel": codec_sel,
             "audiocodec_sel": audiocodec_sel,
             "standard_sel": standard_sel,
             "processing_sel" : processing_sel,
             "team_sel": team_sel,
             "uplver": uplver,
             "tags[]": tags,
             }
 
     scraper=cloudscraper.create_scraper()
-    r = scraper.post(post_url, cookies=cookies_raw2jar(siteinfo.cookie),data=other_data, files=file_tup,timeout=time_out)
+    success_upload=0
+    try_upload=0
+    while success_upload==0:
+        try_upload+=1
+        if try_upload>5:
+            return False,fileinfo+' 发布种子发生请求错误,请确认站点是否正常运行'
+        logger.info('正在发布种子')
+        try:
+            r = scraper.post(post_url, cookies=cookies_raw2jar(siteinfo.cookie),data=other_data, files=file_tup,timeout=time_out)
+            success_upload=1
+        except Exception as r:
+            logger.warning('发布种子发生错误: %s' %(r))
+            success_upload=0
     
     return afterupload(r,fileinfo,record_path,siteinfo,file1,qbinfo,hashlist)
```

### Comparing `upload_machine-0.0.8/upload_machine/utils/uploader/hdpt_upload.py` & `upload_machine-0.0.80/upload_machine/utils/uploader/hdpt_upload.py`

 * *Files 2% similar despite different names*

```diff
@@ -174,10 +174,22 @@
             "processing_sel" : processing_sel,
             "team_sel": team_sel,
             "uplver": uplver,
             "tags[]": tags,
             }
 
     scraper=cloudscraper.create_scraper()
-    r = scraper.post(post_url, cookies=cookies_raw2jar(siteinfo.cookie),data=other_data, files=file_tup,timeout=time_out)
+    success_upload=0
+    try_upload=0
+    while success_upload==0:
+        try_upload+=1
+        if try_upload>5:
+            return False,fileinfo+' 发布种子发生请求错误,请确认站点是否正常运行'
+        logger.info('正在发布种子')
+        try:
+            r = scraper.post(post_url, cookies=cookies_raw2jar(siteinfo.cookie),data=other_data, files=file_tup,timeout=time_out)
+            success_upload=1
+        except Exception as r:
+            logger.warning('发布种子发生错误: %s' %(r))
+            success_upload=0
     
     return afterupload(r,fileinfo,record_path,siteinfo,file1,qbinfo,hashlist)
```

### Comparing `upload_machine-0.0.8/upload_machine/utils/uploader/hdsky_upload.py` & `upload_machine-0.0.80/upload_machine/utils/uploader/piggo_upload.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,211 +1,231 @@
 from loguru import logger
 import time
 import os
 from upload_machine.utils.uploader.upload_tools import *
 import re
 import cloudscraper
 
-def hdsky_upload(siteinfo,file1,record_path,qbinfo,basic,hashlist):
-    post_url = "https://hdsky.me/takeupload.php"
+def piggo_upload(siteinfo,file1,record_path,qbinfo,basic,hashlist):
+    post_url = "https://piggo.me/takeupload.php"
     tags=[]
     time_out=40
     if (file1.pathinfo.type=='anime' or file1.pathinfo.type=='tv') and file1.pathinfo.collection==0:
         fileinfo=file1.chinesename+'在'+siteinfo.sitename+'第'+file1.episodename+'集'
     else:
         fileinfo=file1.chinesename+'在'+siteinfo.sitename
 
 
     #选择类型
     if 'anime' in file1.pathinfo.type.lower():
         select_type='405'
-    elif 'tv' in file1.pathinfo.type.lower() and file1.pathinfo.collection==1:
-        if '大陆' in file1.country or '香港' in file1.country or '台湾' in file1.country:
-            select_type='411'
-        else:
-            select_type='413'
-    elif 'tv' in file1.pathinfo.type.lower() and file1.pathinfo.collection==0:
-        if '大陆' in file1.country or '香港' in file1.country or '台湾' in file1.country:
-            select_type='402'
-        else:
-            select_type='412'
+    elif 'tv' in file1.pathinfo.type.lower():
+        select_type='402'
     elif 'movie' in file1.pathinfo.type.lower():
         select_type='401'
+    elif 'doc' in file1.pathinfo.type.lower():
+        select_type='404'
+    elif 'show' in file1.pathinfo.type.lower():
+        select_type='403'
+    elif 'mv' in file1.pathinfo.type.lower():
+        select_type='406'
+    elif 'sport' in file1.pathinfo.type.lower():
+        select_type='407'
+    elif 'music' in file1.pathinfo.type.lower():
+        select_type='408'
     else:
         select_type='409'
     logger.info('已成功填写类型为'+file1.pathinfo.type)
 
 
     #选择来源 
+    if 'web' in file1.type.lower() and 'rip' in file1.type.lower():
+        source_sel='10'
+    elif 'web' in file1.type.lower():
+        source_sel='7'
+    elif (file1.type=='bluray' or 'bd' in file1.type.lower()) and '2160' in file1.standard_sel:
+        source_sel='8'
+    elif file1.type=='bluray' or 'bd' in file1.type.lower():
+        source_sel='1'
+    elif 'dvd' in file1.type.lower()  :
+        source_sel='3'
+    elif file1.type=='HDTV':
+        source_sel='4'
+    elif file1.type=='remux':
+        source_sel='1'
+    else:
+        source_sel='6'
+    logger.info('已成功选择质量为'+file1.type)
+   
+
+
+    #选择媒介
     if file1.type=='WEB-DL':
         medium_sel='11'
     elif 'rip' in file1.type.lower() or file1.type=='bluray'  :
         medium_sel='7'
     elif file1.type=='HDTV':
         medium_sel='5'
-    elif file1.type=='remux':
+    elif file1.type=='Remux':
         medium_sel='3'
+    elif (file1.type=='bluray' or 'bd' in file1.type.lower()) and '2160' in file1.standard_sel:
+        medium_sel='10'
+    elif file1.type=='bluray' or 'bd' in file1.type.lower():
+        medium_sel='1'
+    elif 'dvd' in file1.type.lower()  :
+        medium_sel='6'
+    elif 'rip' in file1.type.lower():
+        medium_sel='7'
     else:
         medium_sel='7'
-    logger.info('已成功选择质量为'+file1.type)
-   
+    logger.info('已成功填写媒介为'+file1.type)
 
 
     #选择编码
     if file1.Video_Format=='H264':
         codec_sel='1'
     elif file1.Video_Format=='x264':
-        codec_sel='10'
+        codec_sel='1'
     elif file1.Video_Format=='H265':
-        codec_sel='12'
+        codec_sel='6'
     elif file1.Video_Format=='x265':
-        codec_sel='13'
+        codec_sel='6'
     else:
         codec_sel='1'
     logger.info('已成功选择编码为'+file1.Video_Format)
-
     #选择音频编码
     if file1.Audio_Format.upper()=='AAC':
         audiocodec_sel='6'
-    elif 'DTS-HDMA:X 7.1' in file1.Audio_Format.upper():
-        audiocodec_sel='16'
-    elif 'DTS-HDMA' in file1.Audio_Format.upper():
+    elif 'DTS-HDMA' in file1.Audio_Format.upper() or 'DTS-HD MA' in file1.Audio_Format.upper():
+        audiocodec_sel='3'
+    elif 'TRUEHD ATMOS' in file1.Audio_Format.upper():
         audiocodec_sel='10'
-    elif 'TrueHD Atmos' in file1.Audio_Format.upper():
-        audiocodec_sel='17'
     elif 'LPCM' in file1.Audio_Format.upper():
-        audiocodec_sel='13'
-    elif 'TrueHD' in file1.Audio_Format.upper():
         audiocodec_sel='11'
-    elif 'DTS-HD HR' in file1.Audio_Format.upper():
-        audiocodec_sel='14'
-    elif 'PCM' in file1.Audio_Format.upper():
-        audiocodec_sel='19'
+    elif 'TRUEHD' in file1.Audio_Format.upper():
+        audiocodec_sel='10'
     elif 'FLAC' in file1.Audio_Format.upper():
         audiocodec_sel='1'
     elif 'APE' in file1.Audio_Format.upper():
         audiocodec_sel='2'
     elif 'MP3' in file1.Audio_Format.upper():
         audiocodec_sel='4'
     elif 'OGG' in file1.Audio_Format.upper():
         audiocodec_sel='5'
     elif 'AC3' in file1.Audio_Format.upper() or 'DD' in file1.Audio_Format.upper():
-        audiocodec_sel='12'
+        audiocodec_sel='8'
+    elif 'DTS:X' in file1.Audio_Format.upper() or 'DTS-X' in file1.Audio_Format.upper():
+        audiocodec_sel='3'
     elif 'DTS' in file1.Audio_Format.upper():
         audiocodec_sel='3'
     elif 'WAV' in file1.Audio_Format.upper():
-        audiocodec_sel='15'
-    elif 'DSD' in file1.Audio_Format.upper():
-        audiocodec_sel='18'
-    elif 'Dolby Digital Plus Dolby Atmos' in file1.Audio_Format.upper():
-        audiocodec_sel='21'
-    elif 'Dolby Digital Plus' in file1.Audio_Format.upper():
-        audiocodec_sel='20'
-    else:
         audiocodec_sel='7'
+    elif 'M4A' in file1.Audio_Format.upper():
+        audiocodec_sel='7'
+    else:
+        audiocodec_sel='6'
     logger.info('已成功选择音频编码为'+file1.Audio_Format.upper())
 
     #选择分辨率
-    if '2160' in file1.standard_sel:
+    if '8K' in file1.standard_sel:
+        standard_sel='6'
+    elif '2160' in file1.standard_sel:
         standard_sel='5'
     elif '1080p' in file1.standard_sel.lower():
         standard_sel='1'
     elif '1080i' in file1.standard_sel.lower():
         standard_sel='2'
     elif '720' in file1.standard_sel:
         standard_sel='3'
     elif '480' in file1.standard_sel:
-        standard_sel='4'
+        logger.warning('站点不允许发布'+file1.standard_sel+'资源')
+        return False,fileinfo+'站点不允许发布'+file1.standard_sel+'资源'
     else:
         standard_sel='1'
     logger.info('已成功选择分辨率为'+file1.standard_sel)
     
 
     #选择制作组
-    if 'HDSKY' in file1.sub.upper():
+    if 'HDS' in file1.sub.upper():
+        team_sel='1'
+    elif 'CHD' in file1.sub.upper():
+        team_sel='2'
+    elif 'MYSILU' in file1.sub.upper():
+        team_sel='3'
+    elif 'WIKI' in file1.sub.upper():
+        team_sel='4'
+    elif 'CMCT' in file1.sub.upper():
         team_sel='6'
-        tags.append(12)
-    elif 'HDS3D' in file1.sub.upper():
-        team_sel='28'
-        tags.append(12)
-    elif 'HDSTV' in file1.sub.upper():
+    elif 'PIGGOHD' in file1.sub.upper():
+        team_sel='7'
+    elif 'PIGGOWEB'.upper() in file1.sub.upper():
+        team_sel='8'
+    elif 'PiGoNF'.upper() in file1.sub.upper():
         team_sel='9'
-        tags.append(12)
-    elif 'HDSWEB' in file1.sub.upper() and file1.pathinfo.collection==1:
-        team_sel='35'
-        tags.append(12)
-    elif 'HDSWEB' in file1.sub.upper():
-        team_sel='31'
-        tags.append(12)
-    elif 'HDSPAD' in file1.sub.upper():
-        team_sel='18'
-        tags.append(12)
-    elif 'HDSCD' in file1.sub.upper():
-        team_sel='22'
-        tags.append(12)
-    elif 'hdspecial' in file1.sub.lower():
-        team_sel='34'
-        tags.append(12)
-    elif 'BMDRU' in file1.sub.upper():
-        team_sel='30'
-        tags.append(12)
-    elif 'AREA11' in file1.sub.upper():
-        team_sel='25'
-        tags.append(12)
-    elif 'HDSAB' in file1.sub.upper():
-        team_sel='36'
-        tags.append(12)
-    elif 'HDS' in file1.sub.upper():
-        team_sel='1'
-        tags.append(12)
-    elif file1.transfer==0:
-        team_sel='24'
-    elif file1.transfer==1:
-        team_sel='27'
+    elif 'PigoAD'.upper() in file1.sub.upper():
+        team_sel='10'
     else:
-        team_sel='27'
+        team_sel='5'
     logger.info('制作组已成功选择为'+file1.sub)
-    
-    if 'hdsky' in file1.pathinfo.exclusive :
-        tags.append(2)
+
+
+    if 'piggo' in file1.pathinfo.exclusive :
+        tags.append(1)
+    if 'PIGO' in file1.sub.upper():
+        tags.append(3)
     if '国' in file1.language or '中' in file1.language:
         tags.append(5)
     if not file1.sublan=='' and ('简' in file1.sublan or '繁' in file1.sublan or '中' in file1.sublan):
         tags.append(6)
-    if file1.transfer==0:
+    if file1.pathinfo.collection==1:
+        tags.append(11)
+    if file1.pathinfo.complete==1:
+        tags.append(13)
+    if (file1.pathinfo.type=='anime' or file1.pathinfo.type=='tv') and file1.pathinfo.complete==0:
         tags.append(14)
-    tags=list(set(tags))
-    tags.sort()
+    
     if siteinfo.uplver==1:
         uplver='yes'
     else:
         uplver='no'
 
     torrent_file = file1.torrentpath
+
     file_tup = ("file", (os.path.basename(torrent_file), open(torrent_file, 'rb'), 'application/x-bittorrent')),
             
-
     other_data = {
             "name": file1.uploadname,
             "small_descr": file1.small_descr+file1.pathinfo.exinfo,
             "url": file1.imdburl,
-            "url_douban": file1.doubanurl,
+            "pt_gen": file1.doubanurl,
             "nfo": "",
             "color": "0",
             "font": "0",
             "size": "0",
-            "descr": file1.content,
+            "descr": file1.pathinfo.contenthead+'\n'+file1.douban_info+'\n'+file1.screenshoturl+'\n'+file1.pathinfo.contenttail,
+            "technical_info": file1.mediainfo,
             "type": select_type,
-            "medium_sel": medium_sel,
-            "codec_sel": codec_sel,
-            "audiocodec_sel": audiocodec_sel,
-            "standard_sel": standard_sel,
-            "team_sel": team_sel,
+            "source_sel[4]": source_sel,
+            "medium_sel[4]": medium_sel,
+            "codec_sel[4]": codec_sel,
+            "audiocodec_sel[4]": audiocodec_sel,
+            "standard_sel[4]": standard_sel,
+            "team_sel[4]": team_sel,
+            "processing_sel[4]": 1,
             "uplver": uplver,
-            "option_sel[]": tags,
+            "tags[4][]": tags,
             }
-
     scraper=cloudscraper.create_scraper()
-    r = scraper.post(post_url, cookies=cookies_raw2jar(siteinfo.cookie),data=other_data, files=file_tup,timeout=time_out)
-    
-
+    success_upload=0
+    try_upload=0
+    while success_upload==0:
+        try_upload+=1
+        if try_upload>5:
+            return False,fileinfo+' 发布种子发生请求错误,请确认站点是否正常运行'
+        logger.info('正在发布种子')
+        try:
+            r = scraper.post(post_url, cookies=cookies_raw2jar(siteinfo.cookie),data=other_data, files=file_tup,timeout=time_out)
+            success_upload=1
+        except Exception as r:
+            logger.warning('发布种子发生错误: %s' %(r))
+            success_upload=0
     return afterupload(r,fileinfo,record_path,siteinfo,file1,qbinfo,hashlist)
```

### Comparing `upload_machine-0.0.8/upload_machine/utils/uploader/hhclub_upload.py` & `upload_machine-0.0.80/upload_machine/utils/uploader/hdvideo_upload.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from loguru import logger
 import time
 import os
 from upload_machine.utils.uploader.upload_tools import *
 import re
 import cloudscraper
 
-def hhclub_upload(siteinfo,file1,record_path,qbinfo,basic,hashlist):
-    post_url = "https://hhanclub.top/takeupload.php"
+def hdvideo_upload(siteinfo,file1,record_path,qbinfo,basic,hashlist):
+    post_url = "https://hdvideo.one/takeupload.php"
     tags=[]
     time_out=40
     if (file1.pathinfo.type=='anime' or file1.pathinfo.type=='tv') and file1.pathinfo.collection==0:
         fileinfo=file1.chinesename+'在'+siteinfo.sitename+'第'+file1.episodename+'集'
     else:
         fileinfo=file1.chinesename+'在'+siteinfo.sitename
 
 
     #选择类型
     if 'anime' in file1.pathinfo.type.lower():
         select_type='405'
-    elif 'tv' in file1.pathinfo.type.lower() and file1.pathinfo.collection==1:
+    elif 'tv' in file1.pathinfo.type.lower() and file1.pathinfo.collection>=1:
         if '大陆' in file1.country or '香港' in file1.country or '台湾' in file1.country:
             select_type='402'
         else:
             select_type='402'
     elif 'tv' in file1.pathinfo.type.lower() and file1.pathinfo.collection==0:
         if '大陆' in file1.country or '香港' in file1.country or '台湾' in file1.country:
             select_type='402'
@@ -35,171 +35,166 @@
     elif 'doc' in file1.pathinfo.type.lower():
         select_type='404'
     elif 'mv' in file1.pathinfo.type.lower():
         select_type='406'
     elif 'sport' in file1.pathinfo.type.lower():
         select_type='407'
     elif 'music' in file1.pathinfo.type.lower():
-        select_type='409'
+        select_type='408'
     else:
         select_type='405'
     logger.info('已成功填写类型为'+file1.pathinfo.type)
 
+
+    source_sel='24'
     #选择来源
-    if 'web' in file1.type.lower():
-        source_sel='6'
-    elif (file1.type=='bluray' or 'bd' in file1.type.lower()) and '2160' in file1.standard_sel:
-        source_sel='1'
-    elif file1.type=='bluray' or 'bd' in file1.type.lower():
-        source_sel='1'
-    elif 'dvd' in file1.type.lower()  :
-        source_sel='3'
-    elif file1.type=='HDTV':
-        source_sel='4'
-    elif file1.type=='remux':
-        source_sel='1'
+    if 'web' in file1.type.lower() and 'dl' in file1.type.lower():
+        source_sel='24'
+    elif (file1.type=='bluray') and '2160' in file1.standard_sel:
+        source_sel='23'
+    elif file1.type=='bluray':
+        source_sel='22'
+    elif 'rip' in file1.type.lower() and  'web' in file1.type.lower():
+        source_sel='24'
+    elif 'dvd' in file1.type.lower():
+        source_sel='25'
+    elif 'rip' in file1.type.lower()  :
+        source_sel='22'
+    elif 'HDTV' in file1.type.upper() and '2160' in file1.standard_sel:
+        source_sel='26'
+    elif 'HDTV' in file1.type.upper():
+        source_sel='26'
+    elif 'remux' in file1.type.lower():
+        source_sel='22'
     else:
-        source_sel='6'
+        source_sel='28'
     logger.info('已成功填写来源为'+file1.type)
 
+
     #选择媒介
-    if file1.type=='WEB-DL':
+    if 'web' in file1.type.lower() and 'dl' in file1.type.lower():
+        medium_sel='14'
+    elif (file1.type=='bluray') and '2160' in file1.standard_sel:
         medium_sel='10'
-    elif 'rip' in file1.type.lower() or file1.type=='bluray'  :
-        medium_sel='7'
-    elif file1.type=='HDTV':
-        medium_sel='5'
-    elif file1.type=='Remux':
-        medium_sel='3'
-    else:
-        medium_sel='1'
-    logger.info('已成功选择质量为'+file1.type)
-   
+    elif file1.type=='bluray':
+        medium_sel='11'
+    elif 'rip' in file1.type.lower() and  'web' in file1.type.lower():
+        medium_sel='15'
+    elif 'rip' in file1.type.lower()  :
+        medium_sel='13'
+    elif 'HDTV' in file1.type.upper() and '2160' in file1.standard_sel:
+        medium_sel='16'
+    elif 'HDTV' in file1.type.upper():
+        medium_sel='16'
+    elif 'remux' in file1.type.lower():
+        medium_sel='12'
+    elif 'dvd' in file1.type.lower():
+        medium_sel='18'
+    else:
+        medium_sel='19'
+    logger.info('已成功填写来源为'+file1.type)
+
 
 
     #选择编码
     if file1.Video_Format=='H264':
-        codec_sel='1'
+        codec_sel='7'
     elif file1.Video_Format=='x264':
-        codec_sel='1'
+        codec_sel='7'
+    elif 'AVC' in file1.Video_Format.upper():
+        codec_sel='7'
     elif file1.Video_Format=='H265':
         codec_sel='6'
     elif file1.Video_Format=='x265':
         codec_sel='6'
+    elif 'HEVC' in file1.Video_Format.upper():
+        codec_sel='6'
     else:
         codec_sel='6'
     logger.info('已成功选择编码为'+file1.Video_Format)
 
     #选择音频编码
     if file1.Audio_Format.upper()=='AAC':
         audiocodec_sel='6'
     elif 'DTS-HDMA' in file1.Audio_Format.upper() or 'DTS-HD MA' in file1.Audio_Format.upper():
         audiocodec_sel='3'
-    elif 'TrueHD Atmos' in file1.Audio_Format.upper():
-        audiocodec_sel='7'
-    elif 'LPCM' in file1.Audio_Format.upper():
-        audiocodec_sel='7'
-    elif 'TrueHD' in file1.Audio_Format.upper():
-        audiocodec_sel='7'
+    elif 'TRUEHD ATMOS' in file1.Audio_Format.upper():
+        audiocodec_sel='11'
+    elif 'PCM' in file1.Audio_Format.upper():
+        audiocodec_sel='8'
+    elif 'TRUEHD' in file1.Audio_Format.upper():
+        audiocodec_sel='11'
     elif 'FLAC' in file1.Audio_Format.upper():
         audiocodec_sel='1'
     elif 'APE' in file1.Audio_Format.upper():
         audiocodec_sel='2'
     elif 'MP3' in file1.Audio_Format.upper():
-        audiocodec_sel='4'
+        audiocodec_sel='7'
     elif 'AC3' in file1.Audio_Format.upper() or 'AC-3' in file1.Audio_Format.upper() or 'DD' in file1.Audio_Format.upper():
-        audiocodec_sel='8'
+        audiocodec_sel='9'
+    elif 'EAC3' in file1.Audio_Format.upper() or 'EAC-3' in file1.Audio_Format.upper() or 'DDP' in file1.Audio_Format.upper():
+        audiocodec_sel='10'
     elif 'DTS:X' in file1.Audio_Format.upper() or 'DTS-X' in file1.Audio_Format.upper():
         audiocodec_sel='3'
     elif 'DTS' in file1.Audio_Format.upper():
         audiocodec_sel='3'
     elif 'WAV' in file1.Audio_Format.upper():
-        audiocodec_sel='7'
+        audiocodec_sel='12'
     elif 'M4A' in file1.Audio_Format.upper():
         audiocodec_sel='7'
+    elif 'OPUS' in file1.Audio_Format.upper():
+        audiocodec_sel='5'
     else:
         audiocodec_sel='7'
     logger.info('已成功选择音频编码为'+file1.Audio_Format.upper())
 
     #选择分辨率
     if '8K' in file1.standard_sel:
-        standard_sel='1'
+        standard_sel='5'
     elif '2160' in file1.standard_sel:
-        standard_sel='1'
+        standard_sel='6'
     elif '1080p' in file1.standard_sel.lower():
-        standard_sel='2'
+        standard_sel='8'
     elif '1080i' in file1.standard_sel.lower():
-        standard_sel='2'
+        standard_sel='9'
     elif '720' in file1.standard_sel:
-        standard_sel='3'
+        standard_sel='10'
     elif '480' in file1.standard_sel:
-        standard_sel='4'
+        standard_sel='11'
     else:
-        standard_sel='2'
+        standard_sel='8'
     logger.info('已成功选择分辨率为'+file1.standard_sel)
     
-    #选择地区
-    if not file1.country=='':
-        if '大陆' in file1.country:
-            processing_sel='8'
-            logger.info('国家信息已选择'+file1.country)
-        elif '香港' in file1.country:
-            processing_sel='6'
-            logger.info('国家信息已选择'+file1.country)
-        elif '台湾' in file1.country:
-            processing_sel='7'
-            logger.info('国家信息已选择'+file1.country)
-        elif '美国' in file1.country:
-            processing_sel='3'
-            logger.info('国家信息已选择'+file1.country)
-        elif '英国' in file1.country:
-            processing_sel='9'
-            logger.info('国家信息已选择'+file1.country)
-        elif '法国' in file1.country:
-            processing_sel='9'
-            logger.info('国家信息已选择'+file1.country)
-        elif '韩国' in file1.country:
-            processing_sel='5'
-            logger.info('国家信息已选择'+file1.country)
-        elif '日本' in file1.country:
-            processing_sel='4'
-            logger.info('国家信息已选择'+file1.country)
-        elif '印度' in file1.country:
-            processing_sel='9'
-            logger.info('国家信息已选择'+file1.country)
-        else:
-            processing_sel='9'
-            logger.info('未找到资源国家信息，已选择其他')
-    else:
-        processing_sel='4'
-        logger.info('未找到资源国家信息，已默认日本')
-
     #选择制作组
-    if 'HHWEB' in file1.sub.upper():
+    if 'HDVWEB' in file1.sub.upper():
         team_sel='1'
+    elif 'HDVMV' in file1.sub.upper():
+        team_sel='2'
     else:
-        team_sel='5'
+        team_sel='4'
     logger.info('制作组已成功选择为'+file1.sub)
     
-    if 'HHWEB' in file1.sub.upper():
-        tags.append(2)
+    if 'HDV' in file1.sub.upper():
         tags.append(3)
-        tags.append(4)
-    if 'WEB' in file1.type:
-        tags.append(4)
-        logger.info('已选择WEB')
-    if 'hhclub' in file1.pathinfo.exclusive :
+        logger.info('已选择官方')
+    if 'hdvideo' in file1.pathinfo.exclusive :
         tags.append(1)
         logger.info('已选择禁转')
     if '国' in file1.language or '中' in file1.language:
         tags.append(5)
         logger.info('已选择国语')
+    if '粤' in file1.language:
+        tags.append(10)
+        logger.info('已选择粤语')
     if not file1.sublan=='' and ('简' in file1.sublan or '繁' in file1.sublan or '中' in file1.sublan):
         tags.append(6)
         logger.info('已选择中字')
+    if file1.pathinfo.complete==1:
+        tags.append(17)
+        logger.info('已选择完结')
 
     
     tags=list(set(tags))
     tags.sort()
     
     if siteinfo.uplver==1:
         uplver='yes'
@@ -209,28 +204,40 @@
     torrent_file = file1.torrentpath
     file_tup = ("file", (os.path.basename(torrent_file), open(torrent_file, 'rb'), 'application/x-bittorrent')),
             
 
     other_data = {
             "name": file1.uploadname,
             "small_descr": file1.small_descr+file1.pathinfo.exinfo,
+            "url": file1.imdburl,
             "pt_gen": file1.doubanurl,
             "color": "0",
             "font": "0",
             "size": "0",
             "descr": file1.content,
             "type": select_type,
-            "source_sel" : source_sel,
-            "medium_sel": medium_sel,
-            "codec_sel": codec_sel,
-            "audiocodec_sel": audiocodec_sel,
-            "standard_sel": standard_sel,
-            "processing_sel" : processing_sel,
-            "team_sel": team_sel,
+            "source_sel[4]": source_sel,
+            "medium_sel[4]": medium_sel,
+            "codec_sel[4]": codec_sel,
+            "audiocodec_sel[4]": audiocodec_sel,
+            "standard_sel[4]": standard_sel,
+            "team_sel[4]": team_sel,
             "uplver": uplver,
-            "tags[]": tags,
+            "tags[4][]": tags,
             }
 
     scraper=cloudscraper.create_scraper()
-    r = scraper.post(post_url, cookies=cookies_raw2jar(siteinfo.cookie),data=other_data, files=file_tup,timeout=time_out)
+    success_upload=0
+    try_upload=0
+    while success_upload==0:
+        try_upload+=1
+        if try_upload>5:
+            return False,fileinfo+' 发布种子发生请求错误,请确认站点是否正常运行'
+        logger.info('正在发布种子')
+        try:
+            r = scraper.post(post_url, cookies=cookies_raw2jar(siteinfo.cookie),data=other_data, files=file_tup,timeout=time_out)
+            success_upload=1
+        except Exception as r:
+            logger.warning('发布种子发生错误: %s' %(r))
+            success_upload=0
     
     return afterupload(r,fileinfo,record_path,siteinfo,file1,qbinfo,hashlist)
```

### Comparing `upload_machine-0.0.8/upload_machine/utils/uploader/lemonhd_upload.py` & `upload_machine-0.0.80/upload_machine/utils/uploader/lemonhd_upload.py`

 * *Files 9% similar despite different names*

```diff
@@ -61,19 +61,19 @@
     #选择音频编码
     if file1.Audio_Format.upper()=='AAC':
         audiocodec_sel='8'
     elif 'DTS-HD HR' in file1.Audio_Format.upper() or 'DTS-HDHR' in file1.Audio_Format.upper():
         audiocodec_sel='104'
     elif 'DTS-HDMA' in file1.Audio_Format.upper() or 'DTS-HD MA' in file1.Audio_Format.upper():
         audiocodec_sel='5'
-    elif 'TrueHD Atmos' in file1.Audio_Format.upper():
+    elif 'TRUEHD ATMOS' in file1.Audio_Format.upper():
         audiocodec_sel='1'
     elif 'LPCM' in file1.Audio_Format.upper():
         audiocodec_sel='15'
-    elif 'TrueHD' in file1.Audio_Format.upper():
+    elif 'TRUEHD' in file1.Audio_Format.upper():
         audiocodec_sel='2'
     elif 'FLAC' in file1.Audio_Format.upper():
         audiocodec_sel='7'
     elif 'APE' in file1.Audio_Format.upper():
         audiocodec_sel='11'
     elif 'MP3' in file1.Audio_Format.upper():
         audiocodec_sel='9'
@@ -201,20 +201,18 @@
     else:
         if file1.pathinfo.collection==0:
             other_data['animate_type']='3'
             logger.info('已成功选择类型为TV')  
         else:
             other_data['animate_type']='6'
             logger.info('已成功选择类型为collection')
-
-    if file1.pathinfo.complete==0:
+    if file1.pathinfo.collection==0 or (file1.pathinfo.max-file1.pathinfo.min==0):
         other_data['is_complete']='yes'
         logger.info('已成功选择未完结')
         other_data['series']='第'+file1.episodename+'话'
-        
     elif file1.pathinfo.complete==1:
         other_data['series']='TV '+str(file1.pathinfo.min).zfill(2)+'-'+str(file1.pathinfo.max).zfill(2)+' Fin'
     else:
         other_data['series']='TV '+str(file1.pathinfo.min).zfill(2)+'-'+str(file1.pathinfo.max).zfill(2)
     logger.info('已成功填写集数')
 
     if 'i18n' in file1.sub.lower():
@@ -249,15 +247,27 @@
     else:
         other_data['original']='1'
         logger.info('已默认来源为转载')
         other_data['from_url']=file1.from_url
         logger.info('已成功填写转载地址')
 
     scraper=cloudscraper.create_scraper()
-    r = scraper.post(post_url, cookies=cookies_raw2jar(siteinfo.cookie),data=other_data, files=file_tup,timeout=time_out)
+    success_upload=0
+    try_upload=0
+    while success_upload==0:
+        try_upload+=1
+        if try_upload>5:
+            return False,fileinfo+' 发布种子发生请求错误,请确认站点是否正常运行'
+        logger.info('正在发布种子')
+        try:
+            r = scraper.post(post_url, cookies=cookies_raw2jar(siteinfo.cookie),data=other_data, files=file_tup,timeout=time_out)
+            success_upload=1
+        except Exception as r:
+            logger.warning('发布种子发生错误: %s' %(r))
+            success_upload=0
     
     return afterupload(r,fileinfo,record_path,siteinfo,file1,qbinfo,hashlist)
 
 
 
 
 
@@ -314,19 +324,19 @@
     #选择音频编码
     if file1.Audio_Format.upper()=='AAC':
         audiocodec_sel='8'
     elif 'DTS-HD HR' in file1.Audio_Format.upper() or 'DTS-HDHR' in file1.Audio_Format.upper():
         audiocodec_sel='104'
     elif 'DTS-HDMA' in file1.Audio_Format.upper() or 'DTS-HD MA' in file1.Audio_Format.upper():
         audiocodec_sel='5'
-    elif 'TrueHD Atmos' in file1.Audio_Format.upper():
+    elif 'TRUEHD ATMOS' in file1.Audio_Format.upper():
         audiocodec_sel='1'
     elif 'LPCM' in file1.Audio_Format.upper():
         audiocodec_sel='15'
-    elif 'TrueHD' in file1.Audio_Format.upper():
+    elif 'TRUEHD' in file1.Audio_Format.upper():
         audiocodec_sel='2'
     elif 'FLAC' in file1.Audio_Format.upper():
         audiocodec_sel='7'
     elif 'APE' in file1.Audio_Format.upper():
         audiocodec_sel='11'
     elif 'MP3' in file1.Audio_Format.upper():
         audiocodec_sel='9'
@@ -452,15 +462,15 @@
             other_data['type']='402'
             logger.info('已成功选择类型为TV Series(电视剧)')
         if file1.pathinfo.complete==1:
             other_data['is_complete']='yes'
 
         other_data['t_season']=file1.season
         
-        if file1.pathinfo.collection==0:
+        if file1.pathinfo.collection==0 or (file1.pathinfo.max-file1.pathinfo.min==0):
             other_data['series']='E'+file1.episodename
         elif file1.pathinfo.complete==1:
             other_data['series']='E'+str(file1.pathinfo.min).zfill(2)+'-E'+str(file1.pathinfo.max).zfill(2)+' Fin'
         else:
             other_data['series']='E'+str(file1.pathinfo.min).zfill(2)+'-E'+str(file1.pathinfo.max).zfill(2)
         logger.info('已成功填写集数')
     
@@ -497,10 +507,22 @@
     
     if file1.pathinfo.transfer==1:
         other_data['from_url']=file1.from_url
         logger.info('已成功填写转载地址')
 
 
     scraper=cloudscraper.create_scraper()
-    r = scraper.post(post_url, cookies=cookies_raw2jar(siteinfo.cookie),data=other_data, files=file_tup,timeout=time_out)
+    success_upload=0
+    try_upload=0
+    while success_upload==0:
+        try_upload+=1
+        if try_upload>5:
+            return False,fileinfo+' 发布种子发生请求错误,请确认站点是否正常运行'
+        logger.info('正在发布种子')
+        try:
+            r = scraper.post(post_url, cookies=cookies_raw2jar(siteinfo.cookie),data=other_data, files=file_tup,timeout=time_out)
+            success_upload=1
+        except Exception as r:
+            logger.warning('发布种子发生错误: %s' %(r))
+            success_upload=0
     
     return afterupload(r,fileinfo,record_path,siteinfo,file1,qbinfo,hashlist)
```

### Comparing `upload_machine-0.0.8/upload_machine/utils/uploader/piggo_upload.py` & `upload_machine-0.0.80/upload_machine/utils/uploader/wintersakura_upload.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,207 +1,229 @@
 from loguru import logger
 import time
 import os
 from upload_machine.utils.uploader.upload_tools import *
 import re
 import cloudscraper
 
-def piggo_upload(siteinfo,file1,record_path,qbinfo,basic,hashlist):
-    post_url = "https://piggo.me/takeupload.php"
+def wintersakura_upload(siteinfo,file1,record_path,qbinfo,basic,hashlist):
+    post_url = "https://wintersakura.net/takeupload.php"
     tags=[]
     time_out=40
     if (file1.pathinfo.type=='anime' or file1.pathinfo.type=='tv') and file1.pathinfo.collection==0:
         fileinfo=file1.chinesename+'在'+siteinfo.sitename+'第'+file1.episodename+'集'
     else:
         fileinfo=file1.chinesename+'在'+siteinfo.sitename
 
 
     #选择类型
     if 'anime' in file1.pathinfo.type.lower():
-        select_type='405'
-    elif 'tv' in file1.pathinfo.type.lower():
-        select_type='402'
+        select_type='413'
+    elif 'tv' in file1.pathinfo.type.lower() and file1.pathinfo.collection>=1:
+        if '大陆' in file1.country or '香港' in file1.country or '台湾' in file1.country:
+            select_type='417'
+        else:
+            select_type='402'
+    elif 'tv' in file1.pathinfo.type.lower() and file1.pathinfo.collection==0:
+        if '大陆' in file1.country or '香港' in file1.country or '台湾' in file1.country:
+            select_type='402'
+        else:
+            select_type='416'
     elif 'movie' in file1.pathinfo.type.lower():
         select_type='401'
-    elif 'doc' in file1.pathinfo.type.lower():
-        select_type='404'
     elif 'show' in file1.pathinfo.type.lower():
         select_type='403'
+    elif 'doc' in file1.pathinfo.type.lower():
+        select_type='410'
     elif 'mv' in file1.pathinfo.type.lower():
         select_type='406'
     elif 'sport' in file1.pathinfo.type.lower():
         select_type='407'
-    elif 'music' in file1.pathinfo.type.lower():
-        select_type='408'
     else:
         select_type='409'
     logger.info('已成功填写类型为'+file1.pathinfo.type)
 
-
-    #选择来源 
-    if 'web' in file1.type.lower():
-        source_sel='7'
-    elif (file1.type=='bluray' or 'bd' in file1.type.lower()) and '2160' in file1.standard_sel:
-        source_sel='8'
-    elif file1.type=='bluray' or 'bd' in file1.type.lower():
-        source_sel='1'
-    elif 'dvd' in file1.type.lower()  :
-        source_sel='3'
-    elif file1.type=='HDTV':
-        source_sel='4'
-    elif file1.type=='remux':
-        source_sel='1'
-    else:
-        source_sel='6'
-    logger.info('已成功选择质量为'+file1.type)
-   
-
-
-    #选择媒介
+    #选择质量
     if file1.type=='WEB-DL':
-        medium_sel='11'
+        medium_sel='21'
     elif 'rip' in file1.type.lower() or file1.type=='bluray'  :
-        medium_sel='7'
+        medium_sel='15'
     elif file1.type=='HDTV':
-        medium_sel='5'
+        medium_sel='16'
     elif file1.type=='Remux':
-        medium_sel='3'
+        medium_sel='14'
     else:
-        medium_sel='7'
-    logger.info('已成功填写媒介为'+file1.type)
+        medium_sel='15'
+    logger.info('已成功选择质量为'+file1.type)
+   
 
 
     #选择编码
     if file1.Video_Format=='H264':
-        codec_sel='1'
+        codec_sel='6'
     elif file1.Video_Format=='x264':
-        codec_sel='1'
+        codec_sel='8'
     elif file1.Video_Format=='H265':
-        codec_sel='6'
+        codec_sel='9'
     elif file1.Video_Format=='x265':
-        codec_sel='6'
+        codec_sel='7'
     else:
-        codec_sel='1'
+        codec_sel='6'
     logger.info('已成功选择编码为'+file1.Video_Format)
 
     #选择音频编码
     if file1.Audio_Format.upper()=='AAC':
-        audiocodec_sel='6'
+        audiocodec_sel='19'
     elif 'DTS-HDMA' in file1.Audio_Format.upper() or 'DTS-HD MA' in file1.Audio_Format.upper():
-        audiocodec_sel='3'
-    elif 'TrueHD Atmos' in file1.Audio_Format.upper():
+        audiocodec_sel='8'
+    elif 'TRUEHD ATMOS' in file1.Audio_Format.upper():
         audiocodec_sel='10'
     elif 'LPCM' in file1.Audio_Format.upper():
-        audiocodec_sel='11'
-    elif 'TrueHD' in file1.Audio_Format.upper():
-        audiocodec_sel='10'
+        audiocodec_sel='14'
+    elif 'TRUEHD' in file1.Audio_Format.upper():
+        audiocodec_sel='12'
     elif 'FLAC' in file1.Audio_Format.upper():
-        audiocodec_sel='1'
+        audiocodec_sel='15'
     elif 'APE' in file1.Audio_Format.upper():
-        audiocodec_sel='2'
+        audiocodec_sel='16'
     elif 'MP3' in file1.Audio_Format.upper():
-        audiocodec_sel='4'
-    elif 'OGG' in file1.Audio_Format.upper():
-        audiocodec_sel='5'
-    elif 'AC3' in file1.Audio_Format.upper() or 'DD' in file1.Audio_Format.upper():
-        audiocodec_sel='8'
+        audiocodec_sel='17'
+    elif 'AC3' in file1.Audio_Format.upper() or 'AC-3' in file1.Audio_Format.upper() or 'DD' in file1.Audio_Format.upper():
+        audiocodec_sel='20'
     elif 'DTS:X' in file1.Audio_Format.upper() or 'DTS-X' in file1.Audio_Format.upper():
-        audiocodec_sel='3'
+        audiocodec_sel='13'
     elif 'DTS' in file1.Audio_Format.upper():
-        audiocodec_sel='3'
+        audiocodec_sel='13'
     elif 'WAV' in file1.Audio_Format.upper():
-        audiocodec_sel='7'
+        audiocodec_sel='23'
     elif 'M4A' in file1.Audio_Format.upper():
-        audiocodec_sel='7'
+        audiocodec_sel='21'
     else:
-        audiocodec_sel='6'
+        audiocodec_sel='19'
     logger.info('已成功选择音频编码为'+file1.Audio_Format.upper())
 
     #选择分辨率
     if '8K' in file1.standard_sel:
-        standard_sel='6'
+        standard_sel='5'
     elif '2160' in file1.standard_sel:
         standard_sel='5'
     elif '1080p' in file1.standard_sel.lower():
         standard_sel='1'
     elif '1080i' in file1.standard_sel.lower():
         standard_sel='2'
     elif '720' in file1.standard_sel:
         standard_sel='3'
     elif '480' in file1.standard_sel:
-        logger.warning('站点不允许发布'+file1.standard_sel+'资源')
-        return False,fileinfo+'站点不允许发布'+file1.standard_sel+'资源'
+        standard_sel='4'
     else:
         standard_sel='1'
     logger.info('已成功选择分辨率为'+file1.standard_sel)
     
 
     #选择制作组
-    if 'HDS' in file1.sub.upper():
-        team_sel='1'
-    elif 'CHD' in file1.sub.upper():
+    if 'wsub' in file1.sub.lower():
+        team_sel='12'
+    elif 'sakura academic' in file1.sub.lower():
+        team_sel='19'
+    elif 'wsdiy' in file1.sub.lower():
+        team_sel='11'
+    elif 'wscode' in file1.sub.lower():
+        team_sel='16'
+    elif 'sakuraweb' in file1.sub.lower():
+        team_sel='18'
+    elif 'bhd' in file1.sub.lower():
+        team_sel='9'
+    elif 'chd' in file1.sub.lower():
         team_sel='2'
-    elif 'MYSILU' in file1.sub.upper():
-        team_sel='3'
-    elif 'WIKI' in file1.sub.upper():
-        team_sel='4'
-    elif 'CMCT' in file1.sub.upper():
+    elif 'hds' in file1.sub.lower():
+        team_sel='1'
+    elif 'hdc' in file1.sub.lower():
+        team_sel='14'
+    elif 'mteam' in file1.sub.lower():
+        team_sel='13'
+    elif 'ttg' in file1.sub.lower():
+        team_sel='15'
+    elif 'cmct' in file1.sub.lower():
         team_sel='6'
-    elif 'PIGGOHD' in file1.sub.upper():
+    elif 'frds' in file1.sub.lower():
         team_sel='7'
-    elif 'PIGGOWEB' in file1.sub.upper():
+    elif 'pter' in file1.sub.lower():
         team_sel='8'
+    elif 'tjupt' in file1.sub.lower():
+        team_sel='17'
     else:
         team_sel='5'
     logger.info('制作组已成功选择为'+file1.sub)
-    if 'piggo' in file1.pathinfo.exclusive :
-        tags.append(1)
-    if 'PIGGO' in file1.sub.upper():
+    
+    if 'sakura academic' in file1.sub.lower():
+        tags.append(15)
+        logger.info('已选择Sakura Academic')
+    if 'sakuraweb' in file1.sub.lower():
+        tags.append(14)
+        logger.info('已选择Sakura WEB')
+    if 'wsub' in file1.sub.lower():
+        tags.append(13)
+        logger.info('已选择Sakura SUB')
+    if 'sakura' in file1.sub.lower() or 'wsub' in file1.sub.lower():
         tags.append(3)
+        logger.info('已选择官方标签')
+    if 'wintersakura' in file1.pathinfo.exclusive :
+        tags.append(1)
+        logger.info('已选择禁转')
     if '国' in file1.language or '中' in file1.language:
         tags.append(5)
+        logger.info('已选择国语')
     if not file1.sublan=='' and ('简' in file1.sublan or '繁' in file1.sublan or '中' in file1.sublan):
         tags.append(6)
-    if file1.pathinfo.collection==1:
-        tags.append(11)
-    if file1.pathinfo.complete==1:
-        tags.append(13)
-    if (file1.pathinfo.type=='anime' or file1.pathinfo.type=='tv') and file1.pathinfo.complete==0:
-        tags.append(14)
+        logger.info('已选择中字')
+    if file1.pathinfo.transfer==0:
+        tags.append(8)
+        logger.info('已选择原创')
+
     
+    tags=list(set(tags))
+    tags.sort()
     
     if siteinfo.uplver==1:
         uplver='yes'
     else:
         uplver='no'
 
     torrent_file = file1.torrentpath
-
     file_tup = ("file", (os.path.basename(torrent_file), open(torrent_file, 'rb'), 'application/x-bittorrent')),
             
 
     other_data = {
             "name": file1.uploadname,
             "small_descr": file1.small_descr+file1.pathinfo.exinfo,
-            "url": file1.imdburl,
             "pt_gen": file1.doubanurl,
-            "nfo": "",
+            "url" : file1.imdburl,
             "color": "0",
             "font": "0",
             "size": "0",
-            "descr": file1.douban_info+'\n'+file1.screenshoturl,
-            "technical_info": file1.mediainfo,
+            "descr": file1.content,
             "type": select_type,
-            "source_sel": source_sel,
             "medium_sel": medium_sel,
             "codec_sel": codec_sel,
             "audiocodec_sel": audiocodec_sel,
             "standard_sel": standard_sel,
             "team_sel": team_sel,
             "uplver": uplver,
             "tags[]": tags,
             }
 
     scraper=cloudscraper.create_scraper()
-    r = scraper.post(post_url, cookies=cookies_raw2jar(siteinfo.cookie),data=other_data, files=file_tup,timeout=time_out)
-
+    success_upload=0
+    try_upload=0
+    while success_upload==0:
+        try_upload+=1
+        if try_upload>5:
+            return False,fileinfo+' 发布种子发生请求错误,请确认站点是否正常运行'
+        logger.info('正在发布种子')
+        try:
+            r = scraper.post(post_url, cookies=cookies_raw2jar(siteinfo.cookie),data=other_data, files=file_tup,timeout=time_out)
+            success_upload=1
+        except Exception as r:
+            logger.warning('发布种子发生错误: %s' %(r))
+            success_upload=0
+    
     return afterupload(r,fileinfo,record_path,siteinfo,file1,qbinfo,hashlist)
```

### Comparing `upload_machine-0.0.8/upload_machine/utils/uploader/pter_upload.py` & `upload_machine-0.0.80/upload_machine/utils/uploader/pter_upload.py`

 * *Files 18% similar despite different names*

```diff
@@ -122,10 +122,22 @@
     buttomlist=["uplver","jinzhuan","guoyu","zhongzi","pr","guanfang"]
     for item in buttomlist:
         if eval(item+"=='yes'"):
             exec('other_data["'+item+'"]="yes"')
             
 
     scraper=cloudscraper.create_scraper()
-    r = scraper.post(post_url, cookies=cookies_raw2jar(siteinfo.cookie),data=other_data, files=file_tup,timeout=time_out)
+    success_upload=0
+    try_upload=0
+    while success_upload==0:
+        try_upload+=1
+        if try_upload>5:
+            return False,fileinfo+' 发布种子发生请求错误,请确认站点是否正常运行'
+        logger.info('正在发布种子')
+        try:
+            r = scraper.post(post_url, cookies=cookies_raw2jar(siteinfo.cookie),data=other_data, files=file_tup,timeout=time_out)
+            success_upload=1
+        except Exception as r:
+            logger.warning('发布种子发生错误: %s' %(r))
+            success_upload=0
     
     return afterupload(r,fileinfo,record_path,siteinfo,file1,qbinfo,hashlist)
```

### Comparing `upload_machine-0.0.8/upload_machine/utils/uploader/ssd_upload.py` & `upload_machine-0.0.80/upload_machine/utils/uploader/zmpt_upload.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,202 +1,226 @@
 from loguru import logger
 import time
 import os
 from upload_machine.utils.uploader.upload_tools import *
 import re
 import cloudscraper
 
-def ssd_upload(siteinfo,file1,record_path,qbinfo,basic,hashlist):
-    post_url = "https://springsunday.net/takeupload.php"
+def zmpt_upload(siteinfo,file1,record_path,qbinfo,basic,hashlist):
+    post_url = "https://zmpt.cc/takeupload.php"
     tags=[]
     time_out=40
     if (file1.pathinfo.type=='anime' or file1.pathinfo.type=='tv') and file1.pathinfo.collection==0:
         fileinfo=file1.chinesename+'在'+siteinfo.sitename+'第'+file1.episodename+'集'
     else:
         fileinfo=file1.chinesename+'在'+siteinfo.sitename
 
 
     #选择类型
+    select_type='418'
+    processing_sel='0'
     if 'anime' in file1.pathinfo.type.lower():
-        select_type='504'
+        if not file1.country=='':
+            if '大陆' in file1.country:
+                select_type='417'
+                logger.info('国家信息已选择'+file1.country)
+            elif '香港' in file1.country:
+                select_type='417'
+                logger.info('国家信息已选择'+file1.country)
+            elif '台湾' in file1.country:
+                select_type='417'
+                logger.info('国家信息已选择'+file1.country)
+            elif '美国' in file1.country:
+                select_type='420'
+                logger.info('国家信息已选择'+file1.country)
+            elif '英国' in file1.country:
+                select_type='420'
+                logger.info('国家信息已选择'+file1.country)
+            elif '法国' in file1.country:
+                select_type='420'
+                logger.info('国家信息已选择'+file1.country)
+            elif '韩国' in file1.country:
+                select_type='419'
+                logger.info('国家信息已选择'+file1.country)
+            elif '日本' in file1.country:
+                select_type='418'
+                logger.info('国家信息已选择'+file1.country)
+            elif '印度' in file1.country:
+                select_type='421'
+                logger.info('国家信息已选择'+file1.country)
+            else:
+                select_type='421'
+                logger.info('未找到资源国家信息，已选择其他')
+        else:
+            select_type='418'
+        processing_sel='4'
+        if 'movie' in file1.pathinfo.type.lower():
+            processing_sel='3'
     elif 'tv' in file1.pathinfo.type.lower():
-        select_type='502'
+        select_type='411'
     elif 'movie' in file1.pathinfo.type.lower():
-        select_type='501'
-    elif 'show' in file1.pathinfo.type.lower():
-        select_type='505'
+        select_type='410'
     elif 'doc' in file1.pathinfo.type.lower():
-        select_type='503'
-    elif 'sport' in file1.pathinfo.type.lower():
-        select_type='506'
+        select_type='416'
+    elif 'show' in file1.pathinfo.type.lower():
+        select_type='412'
     elif 'mv' in file1.pathinfo.type.lower():
-        select_type='507'
+        select_type='414'
+    elif 'sport' in file1.pathinfo.type.lower():
+        select_type='416'
     elif 'music' in file1.pathinfo.type.lower():
-        select_type='508'
+        select_type='415'
     else:
-        select_type='509'
+        select_type='416'
     logger.info('已成功填写类型为'+file1.pathinfo.type)
 
 
-    #选择来源 
-    if 'remux' in file1.type.lower():
-        medium_sel='4'
-    elif 'bdrip' in file1.type.lower():
+
+    #选择媒介
+    if file1.type=='WEB-DL':
+        medium_sel='10'
+    elif 'rip' in file1.type.lower() and 'dvd' in file1.type.lower():
         medium_sel='6'
-    elif file1.type=='WEB-DL':
+    elif 'rip' in file1.type.lower():
         medium_sel='7'
-    elif 'webrip' in file1.type.lower():
-        medium_sel='8'
     elif file1.type=='HDTV':
         medium_sel='5'
-    elif 'tvrip' in file1.type.lower():
-        medium_sel='9'
-    elif 'dvdrip' in file1.type.lower():
-        medium_sel='10'
-    elif 'dvd' in file1.type.lower():
+    elif file1.type=='Remux':
         medium_sel='3'
+    elif file1.type=='bluray':
+        medium_sel='1'
     else:
-        medium_sel='12'
-    logger.info('已成功选择质量为'+file1.type)
-
+        medium_sel='10'
+    logger.info('已成功填写媒介为'+file1.type)
 
 
     #选择编码
     if file1.Video_Format=='H264':
-        codec_sel='2'
+        codec_sel='1'
     elif file1.Video_Format=='x264':
-        codec_sel='2'
-    elif file1.Video_Format=='H265':
         codec_sel='1'
+    elif file1.Video_Format=='H265':
+        codec_sel='6'
     elif file1.Video_Format=='x265':
-        codec_sel='1'
+        codec_sel='6'
     else:
-        codec_sel='2'
+        codec_sel='1'
     logger.info('已成功选择编码为'+file1.Video_Format)
 
     #选择音频编码
     if file1.Audio_Format.upper()=='AAC':
-        audiocodec_sel='5'
+        audiocodec_sel='6'
     elif 'DTS-HDMA' in file1.Audio_Format.upper() or 'DTS-HD MA' in file1.Audio_Format.upper():
-        audiocodec_sel='1'
-    elif 'TrueHD Atmos' in file1.Audio_Format.upper():
-        audiocodec_sel='2'
+        audiocodec_sel='3'
+    elif 'TRUEHD ATMOS' in file1.Audio_Format.upper():
+        audiocodec_sel='7'
     elif 'LPCM' in file1.Audio_Format.upper():
-        audiocodec_sel='6'
-    elif 'TrueHD' in file1.Audio_Format.upper():
-        audiocodec_sel='2'
-    elif 'FLAC' in file1.Audio_Format.upper():
         audiocodec_sel='7'
+    elif 'TRUEHD' in file1.Audio_Format.upper():
+        audiocodec_sel='7'
+    elif 'FLAC' in file1.Audio_Format.upper():
+        audiocodec_sel='1'
     elif 'APE' in file1.Audio_Format.upper():
-        audiocodec_sel='8'
+        audiocodec_sel='2'
     elif 'MP3' in file1.Audio_Format.upper():
-        audiocodec_sel='10'
-    elif 'AC3' in file1.Audio_Format.upper() or 'AC-3' in file1.Audio_Format.upper() or 'DD' in file1.Audio_Format.upper():
         audiocodec_sel='4'
+    elif 'OGG' in file1.Audio_Format.upper():
+        audiocodec_sel='5'
+    elif 'AC3' in file1.Audio_Format.upper() or 'DD' in file1.Audio_Format.upper():
+        audiocodec_sel='8'
     elif 'DTS:X' in file1.Audio_Format.upper() or 'DTS-X' in file1.Audio_Format.upper():
         audiocodec_sel='3'
     elif 'DTS' in file1.Audio_Format.upper():
         audiocodec_sel='3'
     elif 'WAV' in file1.Audio_Format.upper():
-        audiocodec_sel='9'
+        audiocodec_sel='7'
     elif 'M4A' in file1.Audio_Format.upper():
-        audiocodec_sel='10'
+        audiocodec_sel='7'
     else:
-        audiocodec_sel='10'
+        audiocodec_sel='6'
     logger.info('已成功选择音频编码为'+file1.Audio_Format.upper())
 
     #选择分辨率
     if '8K' in file1.standard_sel:
-        standard_sel='1'
+        standard_sel='5'
     elif '2160' in file1.standard_sel:
-        standard_sel='1'
+        standard_sel='5'
     elif '1080p' in file1.standard_sel.lower():
-        standard_sel='2'
+        standard_sel='1'
     elif '1080i' in file1.standard_sel.lower():
-        standard_sel='3'
+        standard_sel='2'
     elif '720' in file1.standard_sel:
-        standard_sel='4'
+        standard_sel='3'
     elif '480' in file1.standard_sel:
-        standard_sel='5'
+        standard_sel='4'
     else:
-        standard_sel='2'
+        standard_sel='1'
     logger.info('已成功选择分辨率为'+file1.standard_sel)
     
-    #选择地区
-    if file1.country!='' :
-        if '大陆' in file1.country:
-            source_sel='1'
-            logger.info('国家信息已选择'+file1.country)
-        elif '香港' in file1.country:
-            source_sel='2'
-            logger.info('国家信息已选择'+file1.country)
-        elif '台湾' in file1.country:
-            source_sel='2'
-            logger.info('国家信息已选择'+file1.country)
-        elif '美国' in file1.country:
-            source_sel='9'
-            logger.info('国家信息已选择'+file1.country)
-        elif '英国' in file1.country:
-            source_sel='9'
-            logger.info('国家信息已选择'+file1.country)
-        elif '法国' in file1.country:
-            source_sel='9'
-            logger.info('国家信息已选择'+file1.country)
-        elif '韩国' in file1.country:
-            source_sel='10'
-            logger.info('国家信息已选择'+file1.country)
-        elif '日本' in file1.country:
-            source_sel='10'
-            logger.info('国家信息已选择'+file1.country)
-        elif '印度' in file1.country:
-            source_sel='3'
-            logger.info('国家信息已选择'+file1.country)
-        else:
-            source_sel='3'
-            logger.info('未找到资源国家信息，已选择Other')
-    else:
-        source_sel='10'
-    logger.info('未找到资源国家信息，已默认日本')
 
-    if file1.pathinfo.collection==1:
-        pack='yes'
-    else:
-        pack='no'
+    #选择制作组
+    if 'ZmPT' in file1.sub.upper():
+        team_sel='6'
+    elif 'ZmWeb' in file1.sub.upper():
+        team_sel='7'
+    else:
+        team_sel='5'
+    logger.info('制作组已成功选择为'+file1.sub)
+
+    if 'zmpt' in file1.pathinfo.exclusive :
+        tags.append(1)
+    if 'ZMPT' in file1.sub.upper() or 'ZMWEB' in file1.sub.upper():
+        tags.append(3)
+    if '国' in file1.language or '中' in file1.language:
+        tags.append(5)
+    if not file1.sublan=='' and ('简' in file1.sublan or '繁' in file1.sublan or '中' in file1.sublan):
+        tags.append(6)
+    
     
-    if 'ssd' in file1.pathinfo.exclusive:
-        exclusive='yes'
-    else:
-        exclusive='no'
-
     if siteinfo.uplver==1:
         uplver='yes'
     else:
         uplver='no'
 
     torrent_file = file1.torrentpath
+
     file_tup = ("file", (os.path.basename(torrent_file), open(torrent_file, 'rb'), 'application/x-bittorrent')),
             
 
     other_data = {
-            "name": file1.uploadname.replace('  ',' ').replace(' ','.'),
+            "name": file1.uploadname,
             "small_descr": file1.small_descr+file1.pathinfo.exinfo,
-            "url": file1.doubanurl,
-            "url_vimages": file1.screenshoturl.replace('[img]','').replace('[/img]',''),
-            "Media_BDInfo": file1.mediainfo,
+            "pt_gen": file1.doubanurl,
+            "nfo": "",
             "color": "0",
             "font": "0",
             "size": "0",
+            "descr": file1.pathinfo.contenthead+'\n'+file1.douban_info+'\n'+file1.screenshoturl+'\n'+file1.pathinfo.contenttail,
+            "technical_info": file1.mediainfo,
             "type": select_type,
+            "processing_sel": processing_sel,
             "medium_sel": medium_sel,
             "codec_sel": codec_sel,
             "audiocodec_sel": audiocodec_sel,
             "standard_sel": standard_sel,
-            "source_sel" : source_sel,
+            "team_sel": team_sel,
             "uplver": uplver,
-            "exclusive": exclusive,
-            "pack": pack,
+            "tags[]": tags,
             }
 
     scraper=cloudscraper.create_scraper()
-    r = scraper.post(post_url, cookies=cookies_raw2jar(siteinfo.cookie),data=other_data, files=file_tup,timeout=time_out)
-    
+    success_upload=0
+    try_upload=0
+    while success_upload==0:
+        try_upload+=1
+        if try_upload>5:
+            return False,fileinfo+' 发布种子发生请求错误,请确认站点是否正常运行'
+        logger.info('正在发布种子')
+        try:
+            r = scraper.post(post_url, cookies=cookies_raw2jar(siteinfo.cookie),data=other_data, files=file_tup,timeout=time_out)
+            success_upload=1
+        except Exception as r:
+            logger.warning('发布种子发生错误: %s' %(r))
+            success_upload=0
+        
+
     return afterupload(r,fileinfo,record_path,siteinfo,file1,qbinfo,hashlist)
```

### Comparing `upload_machine-0.0.8/upload_machine/utils/uploader/upload_tools.py` & `upload_machine-0.0.80/upload_machine/utils/uploader/upload_tools.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,61 @@
 from loguru import logger
 from qbittorrentapi import Client
 import time
 import datetime
 import os
 from urllib.parse import urlparse
 from bs4 import BeautifulSoup
+import cloudscraper
 import sys
 import re
 import qbittorrentapi
 from http.cookies import SimpleCookie
-
+from bs4 import BeautifulSoup
 
 def afterupload(r,fileinfo,record_path,siteinfo,file1,qbinfo,hashlist):
     if r.status_code==200:
         logger.info('已发布成功')
+    elif r.status_code==400 and siteinfo.sitename=='zhuque' and 'code' in r.json() and 'TORRENT_ALREADY_UPLOAD' in r.json()['code']:
+        return True,fileinfo+'种子发布失败,失败原因:种子已存在'
+    elif siteinfo.sitename=='zhuque' and r.status_code==400 and 'code' in r.json():
+        logger.warning('发布种子发生错误，错误代码:'+str(r.status_code)+' ,错误信息:'+str(r.reason)+'站点返回信息:'+r.json()['code'])
+        return True,fileinfo+' 站点发布种子发生错误，错误代码:'+str(r.status_code)+' ,错误信息:'+str(r.reason)
+    elif siteinfo.sitename=='zhuque' and 'code' in r.json():
+        logger.warning('发布种子发生错误，错误代码:'+str(r.status_code)+' ,错误信息:'+str(r.reason)+'站点返回信息:'+r.json()['code'])
+        return False,fileinfo+' 发布种子发生错误，错误代码:'+str(r.status_code)+' ,错误信息:'+str(r.reason)
     else:
         logger.warning('发布种子发生错误，错误代码:'+str(r.status_code)+' ,错误信息:'+str(r.reason))
         return False,fileinfo+' 发布种子发生错误，错误代码:'+str(r.status_code)+' ,错误信息:'+str(r.reason)
-    String_url =finduploadurl(r)
-    downloadurl=finddownloadurl(r)
+    if siteinfo.sitename=='zhuque':
+        String_url='https://zhuque.in/torrent/info/'+str(r.json()['data']['id'])
+    else:
+        String_url =finduploadurl(r)
+    if siteinfo.sitename=='zhuque':
+        if siteinfo.torrentkey=='':
+            return True,fileinfo+'种子发布成功,但是做种失败，失败原因:未设置zhuque站点torrentkey.'+',当前网址:'+String_url
+        downloadurl='https://zhuque.in/api/torrent/download/'+str(r.json()['data']['id'])+'/'+siteinfo.torrentkey
+    else:
+        downloadurl=finddownloadurl(r)
     if downloadurl=='已存在':
         return True,fileinfo+'种子发布失败,失败原因:种子'+downloadurl+',当前网址:'+String_url
     recordupload(os.path.join(record_path,siteinfo.sitename+'_torrent.csv'),file1,String_url,downloadurl)
-    if not downloadurl =='':
+    if downloadurl !='':
         res=qbseed(url=downloadurl,filepath=file1.downloadpath,qbinfo=qbinfo,category=file1.pathinfo.category,hashlist=hashlist)
         if res:
             return True,fileinfo+'种子发布成功,种子链接:'+downloadurl+',当前网址:'+String_url
         else:
             return True,fileinfo+'种子发布成功,但是添加种子失败,请手动添加种子，种子链接:'+downloadurl+',当前网址:'+String_url
     else:
-        return False,fileinfo+'未找到下载链接,当前网址:'+String_url
+        logger.warning('正在记录错误的请求返回值')
+        errorfile=os.path.join(record_path,'errorhtml.html')
+        f=open(errorfile,'w', encoding='utf-8')
+        f.write(r.text)
+        f.close()
+        return False,fileinfo+'未找到下载链接,当前网址:'+String_url+' ,请求的返回值已保存至:'+errorfile
 
 def cookies_raw2jar(raw: str) -> dict:
     """
     Arrange Cookies from raw using SimpleCookies
     """
     if not raw:
         raise ValueError("The Cookies is not allowed to be empty.")
@@ -101,39 +123,44 @@
     if not('&uploaded' in String_url):
         logger.warning(String_url+'未找到发布页面网址')
         return '未找到发布页面网址'
     String_url =String_url.split('&uploaded')[0]
     return String_url
 
 
+
 def finddownloadurl(res):
     logger.info('正在寻找页面下载链接')
     o = urlparse(res.url)
     o = o.scheme+'://'+o.hostname+'/download.php?'
     #白兔特判
     if 'hare' in o:
         link = re.findall('(https://club\.hares\.top/download\.php\?downhash=.*)\</p',res.text)
         if len(link)>0:
             return link[0]
         else:
+            if '已存在' in res.text:
+                logger.warning('该种子已存在')
+                return '已存在'
             logger.warning('未找到下载链接')
             return ''
     #白兔特判结束
     soup = BeautifulSoup(res.text,'lxml')
-    for a in soup.find_all('a'):
+    for a in soup.find_all('a', href=True):
         link=''
         try:
             link = a['href']
         except:
-            logger.warning('该a标签未找到href属性')
+            #logger.warning('该a标签未找到href属性')
+            logger.trace('该a标签未找到href属性')
         if o in link:
             logger.info('成功获得下载链接'+link)
             return link
 
-    for a in soup.find_all('a'):
+    for a in soup.find_all('a', href=True):
         link=''
         try:
             link = a['href']
         except:
             logger.warning('该a标签未找到href属性')
         if len(re.findall(r'download.php\?id=[0-9]+&',link))>0:
             o = urlparse(res.url)
@@ -178,43 +205,43 @@
         if trynum>12:
             logger.warning('添加种子失败,种子下载链接为:'+url+'   请自行手动添加')
             return True
         logger.info('正在第'+str(trynum)+'次添加种子')
         try:
             res=client.torrents_add(urls=url,save_path=filepath,is_skip_checking=is_skip_checking,is_paused=is_paused,use_auto_torrent_management=None,category=category)
         except Exception as r:
-            logger.warning('添加种子进入qb出错，错误信息: %s' %(r))
+            logger.warning('添加种子进入qb出错，错误信息: %s' %(str(r)[:50]))
             continue
             #raise ValueError ('添加种子进入qbittorrent出错，程序结束')
         if 'Ok' in res:
             logger.info('返回值显示成功添加种子')
         else:
-            logger.warning('添加种子失败，返回值为:'+str(res))
+            logger.warning('添加种子失败，返回值为:'+str(res)[:50])
         time.sleep(1)
         try:
             tor_num_new=len(client.torrents_info())
         except Exception as r:
             tor_num_new=tor_num
-            logger.warning('计算种子数量出错，错误信息: %s' %(r))
+            logger.warning('计算种子数量出错，错误信息: %s' %(str(r)[:50]))
         if tor_num_new==tor_num:
             time.sleep(5)
             try:
                 tor_num_new=len(client.torrents_info())
             except Exception as r:
                 tor_num_new=tor_num
-                logger.warning('计算种子数量出错，错误信息: %s' %(r))
+                logger.warning('计算种子数量出错，错误信息: %s' %(str(r)[:50]))
 
     logger.info('已经成功添加种子')
     addtime=0
     to=None
     try:
         torrentlist=client.torrents.info()
     except Exception as r:
         torrentlist=[]
-        logger.warning('获取种子信息出错，错误信息: %s' %(r))
+        logger.warning('获取种子信息出错，错误信息: %s' %(str(r)[:50]))
     for item in torrentlist:
         if item.added_on>addtime:
             addtime=item.added_on
             to=item
     if type(to)!=qbittorrentapi.torrents.TorrentDictionary:
         logger.warning('未找到最新的种子')
         return True
@@ -226,10 +253,10 @@
         for item in to.trackers:
             if 'url' in item and 'leaguehd' in item['url']:
                 tracker=item['url']
                 if 'http:' in tracker:
                     try:
                         to.edit_tracker(orig_url=tracker,new_url=tracker.replace('http:','https:'))
                     except Exception as r:
-                        logger.error('更改tracker失败，原因: %s' %(r))
+                        logger.error('更改tracker失败，原因: %s' %(str(r)[:50]))
 
     return True
```

### Comparing `upload_machine-0.0.8/upload_machine/utils/uploader/wintersakura_upload.py` & `upload_machine-0.0.80/upload_machine/utils/uploader/rousi_upload.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,187 +1,207 @@
 from loguru import logger
 import time
 import os
 from upload_machine.utils.uploader.upload_tools import *
 import re
 import cloudscraper
 
-def wintersakura_upload(siteinfo,file1,record_path,qbinfo,basic,hashlist):
-    post_url = "https://wintersakura.net/takeupload.php"
+def rousi_upload(siteinfo,file1,record_path,qbinfo,basic,hashlist):
+    post_url = "https://rousi.zip/takeupload.php"
     tags=[]
     time_out=40
     if (file1.pathinfo.type=='anime' or file1.pathinfo.type=='tv') and file1.pathinfo.collection==0:
         fileinfo=file1.chinesename+'在'+siteinfo.sitename+'第'+file1.episodename+'集'
     else:
         fileinfo=file1.chinesename+'在'+siteinfo.sitename
 
 
     #选择类型
     if 'anime' in file1.pathinfo.type.lower():
-        select_type='413'
-    elif 'tv' in file1.pathinfo.type.lower() and file1.pathinfo.collection==1:
+        select_type='415'
+    elif 'tv' in file1.pathinfo.type.lower() and file1.pathinfo.collection>=1:
         if '大陆' in file1.country or '香港' in file1.country or '台湾' in file1.country:
-            select_type='417'
+            select_type='402'
         else:
             select_type='402'
     elif 'tv' in file1.pathinfo.type.lower() and file1.pathinfo.collection==0:
         if '大陆' in file1.country or '香港' in file1.country or '台湾' in file1.country:
             select_type='402'
         else:
-            select_type='416'
+            select_type='402'
     elif 'movie' in file1.pathinfo.type.lower():
         select_type='401'
     elif 'show' in file1.pathinfo.type.lower():
         select_type='403'
     elif 'doc' in file1.pathinfo.type.lower():
-        select_type='410'
+        select_type='404'
     elif 'mv' in file1.pathinfo.type.lower():
         select_type='406'
     elif 'sport' in file1.pathinfo.type.lower():
         select_type='407'
+    elif 'music' in file1.pathinfo.type.lower():
+        select_type='406'
     else:
-        select_type='409'
+        select_type='405'
     logger.info('已成功填写类型为'+file1.pathinfo.type)
 
-    #选择质量
-    if file1.type=='WEB-DL':
-        medium_sel='21'
-    elif 'rip' in file1.type.lower() or file1.type=='bluray'  :
-        medium_sel='15'
-    elif file1.type=='HDTV':
-        medium_sel='16'
-    elif file1.type=='Remux':
-        medium_sel='14'
-    else:
-        medium_sel='15'
-    logger.info('已成功选择质量为'+file1.type)
-   
+
+    source_sel='24'
+    #选择来源
+    if 'web' in file1.type.lower() and 'dl' in file1.type.lower():
+        source_sel='24'
+    elif (file1.type=='bluray') and '2160' in file1.standard_sel:
+        source_sel='23'
+    elif file1.type=='bluray':
+        source_sel='22'
+    elif 'rip' in file1.type.lower() and  'web' in file1.type.lower():
+        source_sel='24'
+    elif 'dvd' in file1.type.lower():
+        source_sel='25'
+    elif 'rip' in file1.type.lower()  :
+        source_sel='22'
+    elif 'HDTV' in file1.type.upper() and '2160' in file1.standard_sel:
+        source_sel='26'
+    elif 'HDTV' in file1.type.upper():
+        source_sel='26'
+    elif 'remux' in file1.type.lower():
+        source_sel='22'
+    else:
+        source_sel='28'
+    logger.info('已成功填写来源为'+file1.type)
+
+
+    #选择媒介
+    if 'web' in file1.type.lower() and 'dl' in file1.type.lower():
+        medium_sel='10'
+    elif (file1.type=='bluray') and '2160' in file1.standard_sel:
+        medium_sel='1'
+    elif file1.type=='bluray':
+        medium_sel='1'
+    elif 'rip' in file1.type.lower() and  'dvd' in file1.type.lower():
+        medium_sel='6'
+    elif 'rip' in file1.type.lower()  :
+        medium_sel='7'
+    elif 'HDTV' in file1.type.upper() and '2160' in file1.standard_sel:
+        medium_sel='5'
+    elif 'HDTV' in file1.type.upper():
+        medium_sel='5'
+    elif 'remux' in file1.type.lower():
+        medium_sel='3'
+    elif 'dvd' in file1.type.lower():
+        medium_sel='2'
+    else:
+        medium_sel='10'
+    logger.info('已成功填写来源为'+file1.type)
+
 
 
     #选择编码
     if file1.Video_Format=='H264':
-        codec_sel='6'
+        codec_sel='1'
     elif file1.Video_Format=='x264':
-        codec_sel='8'
+        codec_sel='1'
     elif file1.Video_Format=='H265':
-        codec_sel='9'
+        codec_sel='6'
     elif file1.Video_Format=='x265':
-        codec_sel='7'
-    else:
         codec_sel='6'
+    else:
+        codec_sel='1'
     logger.info('已成功选择编码为'+file1.Video_Format)
 
     #选择音频编码
     if file1.Audio_Format.upper()=='AAC':
-        audiocodec_sel='19'
+        audiocodec_sel='6'
     elif 'DTS-HDMA' in file1.Audio_Format.upper() or 'DTS-HD MA' in file1.Audio_Format.upper():
+        audiocodec_sel='11'
+    elif 'TRUEHD ATMOS' in file1.Audio_Format.upper():
         audiocodec_sel='8'
-    elif 'TrueHD Atmos' in file1.Audio_Format.upper():
-        audiocodec_sel='10'
-    elif 'LPCM' in file1.Audio_Format.upper():
+    elif 'PCM' in file1.Audio_Format.upper():
         audiocodec_sel='14'
-    elif 'TrueHD' in file1.Audio_Format.upper():
-        audiocodec_sel='12'
+    elif 'TRUEHD' in file1.Audio_Format.upper():
+        audiocodec_sel='9'
     elif 'FLAC' in file1.Audio_Format.upper():
-        audiocodec_sel='15'
+        audiocodec_sel='1'
     elif 'APE' in file1.Audio_Format.upper():
-        audiocodec_sel='16'
+        audiocodec_sel='2'
     elif 'MP3' in file1.Audio_Format.upper():
-        audiocodec_sel='17'
+        audiocodec_sel='4'
     elif 'AC3' in file1.Audio_Format.upper() or 'AC-3' in file1.Audio_Format.upper() or 'DD' in file1.Audio_Format.upper():
-        audiocodec_sel='20'
-    elif 'DTS:X' in file1.Audio_Format.upper() or 'DTS-X' in file1.Audio_Format.upper():
         audiocodec_sel='13'
-    elif 'DTS' in file1.Audio_Format.upper():
+    elif 'EAC3' in file1.Audio_Format.upper() or 'EAC-3' in file1.Audio_Format.upper() or 'DDP' in file1.Audio_Format.upper():
         audiocodec_sel='13'
+    elif 'DTS:X' in file1.Audio_Format.upper() or 'DTS-X' in file1.Audio_Format.upper():
+        audiocodec_sel='10'
+    elif 'DTS' in file1.Audio_Format.upper():
+        audiocodec_sel='3'
     elif 'WAV' in file1.Audio_Format.upper():
-        audiocodec_sel='23'
+        audiocodec_sel='7'
     elif 'M4A' in file1.Audio_Format.upper():
-        audiocodec_sel='21'
+        audiocodec_sel='7'
+    elif 'OGG' in file1.Audio_Format.upper():
+        audiocodec_sel='5'
     else:
-        audiocodec_sel='19'
+        audiocodec_sel='7'
     logger.info('已成功选择音频编码为'+file1.Audio_Format.upper())
 
     #选择分辨率
     if '8K' in file1.standard_sel:
-        standard_sel='5'
+        standard_sel='6'
     elif '2160' in file1.standard_sel:
-        standard_sel='5'
+        standard_sel='6'
     elif '1080p' in file1.standard_sel.lower():
         standard_sel='1'
     elif '1080i' in file1.standard_sel.lower():
         standard_sel='2'
     elif '720' in file1.standard_sel:
         standard_sel='3'
     elif '480' in file1.standard_sel:
-        standard_sel='4'
+        standard_sel='7'
     else:
-        standard_sel='1'
+        standard_sel='8'
     logger.info('已成功选择分辨率为'+file1.standard_sel)
     
-
     #选择制作组
-    if 'wsub' in file1.sub.lower():
-        team_sel='12'
-    elif 'sakura academic' in file1.sub.lower():
-        team_sel='19'
-    elif 'wsdiy' in file1.sub.lower():
-        team_sel='11'
-    elif 'wscode' in file1.sub.lower():
-        team_sel='16'
-    elif 'sakuraweb' in file1.sub.lower():
-        team_sel='18'
-    elif 'bhd' in file1.sub.lower():
-        team_sel='9'
-    elif 'chd' in file1.sub.lower():
-        team_sel='2'
-    elif 'hds' in file1.sub.lower():
+    if 'DJWEB' in file1.sub.upper():
         team_sel='1'
-    elif 'hdc' in file1.sub.lower():
-        team_sel='14'
-    elif 'mteam' in file1.sub.lower():
-        team_sel='13'
-    elif 'ttg' in file1.sub.lower():
-        team_sel='15'
-    elif 'cmct' in file1.sub.lower():
+    elif 'DJTV' in file1.sub.upper():
+        team_sel='2'
+    elif 'DJZB' in file1.sub.upper():
+        team_sel='3'
+    elif 'CatEDU' in file1.sub.upper():
         team_sel='6'
-    elif 'frds' in file1.sub.lower():
-        team_sel='7'
-    elif 'pter' in file1.sub.lower():
+    elif 'Zaxyzit' in file1.sub.upper():
         team_sel='8'
-    elif 'tjupt' in file1.sub.lower():
-        team_sel='17'
     else:
-        team_sel='5'
+        team_sel='7'
     logger.info('制作组已成功选择为'+file1.sub)
     
-    if 'sakura academic' in file1.sub.lower():
-        tags.append(15)
-        logger.info('已选择Sakura Academic')
-    if 'sakuraweb' in file1.sub.lower():
-        tags.append(14)
-        logger.info('已选择Sakura WEB')
-    if 'wsub' in file1.sub.lower():
-        tags.append(13)
-        logger.info('已选择Sakura SUB')
-    if 'sakura' in file1.sub.lower() or 'wsub' in file1.sub.lower():
-        tags.append(3)
-        logger.info('已选择官方标签')
-    if 'wintersakura' in file1.pathinfo.exclusive :
+
+    if 'rousi' in file1.pathinfo.exclusive :
         tags.append(1)
         logger.info('已选择禁转')
+    if 'ROUSI' in file1.sub.upper():
+        tags.append(3)
+        logger.info('已选择官方')
     if '国' in file1.language or '中' in file1.language:
         tags.append(5)
         logger.info('已选择国语')
     if not file1.sublan=='' and ('简' in file1.sublan or '繁' in file1.sublan or '中' in file1.sublan):
         tags.append(6)
         logger.info('已选择中字')
-    if file1.pathinfo.transfer==0:
-        tags.append(8)
-        logger.info('已选择原创')
+    if '粤' in file1.language:
+        tags.append(15)
+        logger.info('已选择粤语')
+    if '2160' in file1.standard_sel:
+        tags.append(18)
+        logger.info('已选择4K')
+    if 'ROUSIWEB' in file1.sub.upper():
+        tags.append(13)
+        logger.info('已选择RousiWeb')
+
 
     
     tags=list(set(tags))
     tags.sort()
     
     if siteinfo.uplver==1:
         uplver='yes'
@@ -191,27 +211,35 @@
     torrent_file = file1.torrentpath
     file_tup = ("file", (os.path.basename(torrent_file), open(torrent_file, 'rb'), 'application/x-bittorrent')),
             
 
     other_data = {
             "name": file1.uploadname,
             "small_descr": file1.small_descr+file1.pathinfo.exinfo,
+            "url": file1.imdburl,
             "pt_gen": file1.doubanurl,
-            "url" : file1.imdburl,
             "color": "0",
             "font": "0",
             "size": "0",
-            "descr": file1.content,
+            "descr": file1.pathinfo.contenthead+'\n'+file1.douban_info+'\n'+file1.screenshoturl+'\n'+file1.pathinfo.contenttail,
+            "technical_info": file1.mediainfo,
             "type": select_type,
-            "medium_sel": medium_sel,
-            "codec_sel": codec_sel,
-            "audiocodec_sel": audiocodec_sel,
-            "standard_sel": standard_sel,
-            "team_sel": team_sel,
             "uplver": uplver,
-            "tags[]": tags,
+            "tags[4][]": tags,
             }
 
     scraper=cloudscraper.create_scraper()
-    r = scraper.post(post_url, cookies=cookies_raw2jar(siteinfo.cookie),data=other_data, files=file_tup,timeout=time_out)
+    success_upload=0
+    try_upload=0
+    while success_upload==0:
+        try_upload+=1
+        if try_upload>5:
+            return False,fileinfo+' 发布种子发生请求错误,请确认站点是否正常运行'
+        logger.info('正在发布种子')
+        try:
+            r = scraper.post(post_url, cookies=cookies_raw2jar(siteinfo.cookie),data=other_data, files=file_tup,timeout=time_out)
+            success_upload=1
+        except Exception as r:
+            logger.warning('发布种子发生错误: %s' %(r))
+            success_upload=0
     
     return afterupload(r,fileinfo,record_path,siteinfo,file1,qbinfo,hashlist)
```

### Comparing `upload_machine-0.0.8/upload_machine.egg-info/SOURCES.txt` & `upload_machine-0.0.80/upload_machine.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 MANIFEST.in
 README.md
 setup.py
 upload_machine/__init__.py
 upload_machine/basicinfo.yaml
 upload_machine/main.py
 upload_machine.egg-info/PKG-INFO
@@ -15,19 +16,22 @@
 upload_machine/utils/edittorrent/edittorrent.py
 upload_machine/utils/img_upload/__init__.py
 upload_machine/utils/img_upload/chevereto.py
 upload_machine/utils/img_upload/fapping_emp.py
 upload_machine/utils/img_upload/imgbox.py
 upload_machine/utils/img_upload/imgupload.py
 upload_machine/utils/img_upload/ptpimg.py
+upload_machine/utils/img_upload/redleaves.py
+upload_machine/utils/img_upload/sharkimg.py
 upload_machine/utils/img_upload/smms.py
 upload_machine/utils/mediafile/__init__.py
 upload_machine/utils/mediafile/douban_book.py
 upload_machine/utils/mediafile/douban_movie.py
 upload_machine/utils/mediafile/doubaninfo.py
+upload_machine/utils/mediafile/maketorrent.py
 upload_machine/utils/mediafile/mediafile.py
 upload_machine/utils/para_ctrl/__init__.py
 upload_machine/utils/para_ctrl/para_ctrl.py
 upload_machine/utils/para_ctrl/readargs.py
 upload_machine/utils/para_ctrl/readyaml.py
 upload_machine/utils/pathinfo/__init__.py
 upload_machine/utils/pathinfo/pathinfo.py
@@ -37,18 +41,28 @@
 upload_machine/utils/signer/__init__.py
 upload_machine/utils/site/__init__.py
 upload_machine/utils/site/site.py
 upload_machine/utils/uploader/__init__.py
 upload_machine/utils/uploader/audience_upload.py
 upload_machine/utils/uploader/auto_upload.py
 upload_machine/utils/uploader/carpt_upload.py
-upload_machine/utils/uploader/hare_upload.py
+upload_machine/utils/uploader/dajiao_upload.py
+upload_machine/utils/uploader/hares_upload.py
 upload_machine/utils/uploader/hdfans_upload.py
 upload_machine/utils/uploader/hdpt_upload.py
 upload_machine/utils/uploader/hdsky_upload.py
+upload_machine/utils/uploader/hdvideo_upload.py
 upload_machine/utils/uploader/hhclub_upload.py
+upload_machine/utils/uploader/ihdbits_upload.py
 upload_machine/utils/uploader/lemonhd_upload.py
+upload_machine/utils/uploader/mteam_upload.py
+upload_machine/utils/uploader/pandapt_upload.py
 upload_machine/utils/uploader/piggo_upload.py
 upload_machine/utils/uploader/pter_upload.py
+upload_machine/utils/uploader/redleaves_upload.py
+upload_machine/utils/uploader/rousi_upload.py
+upload_machine/utils/uploader/sharkpt_upload.py
 upload_machine/utils/uploader/ssd_upload.py
 upload_machine/utils/uploader/upload_tools.py
-upload_machine/utils/uploader/wintersakura_upload.py
+upload_machine/utils/uploader/wintersakura_upload.py
+upload_machine/utils/uploader/zhuque_upload.py
+upload_machine/utils/uploader/zmpt_upload.py
```

