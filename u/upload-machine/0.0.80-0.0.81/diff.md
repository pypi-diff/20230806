# Comparing `tmp/upload_machine-0.0.80.tar.gz` & `tmp/upload_machine-0.0.81.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upload_machine-0.0.80.tar", last modified: Sun Aug  6 09:32:49 2023, max compression
+gzip compressed data, was "upload_machine-0.0.81.tar", last modified: Sun Aug  6 09:48:53 2023, max compression
```

## Comparing `upload_machine-0.0.80.tar` & `upload_machine-0.0.81.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 moyu       (501) staff       (20)        0 2023-08-06 09:32:49.446617 upload_machine-0.0.80/
--rwx------   0 moyu       (501) staff       (20)     1063 2022-10-06 05:53:46.000000 upload_machine-0.0.80/LICENSE
--rwx------   0 moyu       (501) staff       (20)       37 2022-10-06 08:50:43.000000 upload_machine-0.0.80/MANIFEST.in
--rw-r--r--   0 moyu       (501) staff       (20)    14608 2023-08-06 09:32:49.442100 upload_machine-0.0.80/PKG-INFO
--rwxr-xr-x   0 moyu       (501) staff       (20)    14206 2023-08-06 07:01:29.000000 upload_machine-0.0.80/README.md
--rw-r--r--   0 moyu       (501) staff       (20)       38 2023-08-06 09:32:49.446842 upload_machine-0.0.80/setup.cfg
--rwx------   0 moyu       (501) staff       (20)     1110 2023-08-06 09:32:42.000000 upload_machine-0.0.80/setup.py
-drwxr-xr-x   0 moyu       (501) staff       (20)        0 2023-08-06 09:32:49.325187 upload_machine-0.0.80/upload_machine/
--rwx------   0 moyu       (501) staff       (20)        0 2022-10-06 05:53:46.000000 upload_machine-0.0.80/upload_machine/__init__.py
--rwx------   0 moyu       (501) staff       (20)      241 2022-10-06 08:12:01.000000 upload_machine-0.0.80/upload_machine/basicinfo.yaml
--rwx------   0 moyu       (501) staff       (20)     2622 2023-01-02 14:54:11.000000 upload_machine-0.0.80/upload_machine/main.py
-drwxr-xr-x   0 moyu       (501) staff       (20)        0 2023-08-06 09:32:49.330597 upload_machine-0.0.80/upload_machine/utils/
--rwx------   0 moyu       (501) staff       (20)        0 2022-10-06 05:53:46.000000 upload_machine-0.0.80/upload_machine/utils/__init__.py
-drwxr-xr-x   0 moyu       (501) staff       (20)        0 2023-08-06 09:32:49.331379 upload_machine-0.0.80/upload_machine/utils/edittorrent/
--rwx------   0 moyu       (501) staff       (20)        0 2022-10-06 05:53:46.000000 upload_machine-0.0.80/upload_machine/utils/edittorrent/__init__.py
--rwx------   0 moyu       (501) staff       (20)     3966 2022-10-06 05:53:46.000000 upload_machine-0.0.80/upload_machine/utils/edittorrent/edittorrent.py
-drwxr-xr-x   0 moyu       (501) staff       (20)        0 2023-08-06 09:32:49.341434 upload_machine-0.0.80/upload_machine/utils/img_upload/
--rwx------   0 moyu       (501) staff       (20)        0 2022-10-06 05:53:46.000000 upload_machine-0.0.80/upload_machine/utils/img_upload/__init__.py
--rwx------   0 moyu       (501) staff       (20)     7231 2022-10-06 05:53:46.000000 upload_machine-0.0.80/upload_machine/utils/img_upload/chevereto.py
--rwx------   0 moyu       (501) staff       (20)     2674 2022-10-06 05:53:46.000000 upload_machine-0.0.80/upload_machine/utils/img_upload/fapping_emp.py
--rwx------   0 moyu       (501) staff       (20)     4521 2022-10-06 05:53:46.000000 upload_machine-0.0.80/upload_machine/utils/img_upload/imgbox.py
--rwxr-xr-x   0 moyu       (501) staff       (20)     9014 2023-01-20 04:03:37.000000 upload_machine-0.0.80/upload_machine/utils/img_upload/imgupload.py
--rwx------   0 moyu       (501) staff       (20)     2510 2022-10-06 05:53:46.000000 upload_machine-0.0.80/upload_machine/utils/img_upload/ptpimg.py
--rwx------   0 moyu       (501) staff       (20)     1904 2022-11-06 06:50:27.000000 upload_machine-0.0.80/upload_machine/utils/img_upload/redleaves.py
--rw-r--r--   0 moyu       (501) staff       (20)     2426 2023-01-20 04:03:37.000000 upload_machine-0.0.80/upload_machine/utils/img_upload/sharkimg.py
--rwx------   0 moyu       (501) staff       (20)     2875 2022-10-06 05:53:46.000000 upload_machine-0.0.80/upload_machine/utils/img_upload/smms.py
-drwxr-xr-x   0 moyu       (501) staff       (20)        0 2023-08-06 09:32:49.348378 upload_machine-0.0.80/upload_machine/utils/mediafile/
--rwx------   0 moyu       (501) staff       (20)        0 2022-10-06 05:53:46.000000 upload_machine-0.0.80/upload_machine/utils/mediafile/__init__.py
--rwx------   0 moyu       (501) staff       (20)    17212 2022-10-06 05:53:46.000000 upload_machine-0.0.80/upload_machine/utils/mediafile/douban_book.py
--rwx------   0 moyu       (501) staff       (20)    24814 2022-10-06 05:53:46.000000 upload_machine-0.0.80/upload_machine/utils/mediafile/douban_movie.py
--rwx------   0 moyu       (501) staff       (20)     6861 2022-10-06 08:34:29.000000 upload_machine-0.0.80/upload_machine/utils/mediafile/doubaninfo.py
--rw-r--r--   0 moyu       (501) staff       (20)     2418 2023-01-03 18:41:08.000000 upload_machine-0.0.80/upload_machine/utils/mediafile/maketorrent.py
--rwx------   0 moyu       (501) staff       (20)    64920 2023-08-06 09:31:08.000000 upload_machine-0.0.80/upload_machine/utils/mediafile/mediafile.py
-drwxr-xr-x   0 moyu       (501) staff       (20)        0 2023-08-06 09:32:49.354495 upload_machine-0.0.80/upload_machine/utils/para_ctrl/
--rwx------   0 moyu       (501) staff       (20)      218 2022-10-06 08:34:43.000000 upload_machine-0.0.80/upload_machine/utils/para_ctrl/__init__.py
--rwx------   0 moyu       (501) staff       (20)     6779 2022-10-09 10:10:39.000000 upload_machine-0.0.80/upload_machine/utils/para_ctrl/para_ctrl.py
--rwxr-xr-x   0 moyu       (501) staff       (20)     2154 2023-01-20 04:03:37.000000 upload_machine-0.0.80/upload_machine/utils/para_ctrl/readargs.py
--rwx------   0 moyu       (501) staff       (20)     1901 2023-01-06 10:01:44.000000 upload_machine-0.0.80/upload_machine/utils/para_ctrl/readyaml.py
-drwxr-xr-x   0 moyu       (501) staff       (20)        0 2023-08-06 09:32:49.356342 upload_machine-0.0.80/upload_machine/utils/pathinfo/
--rwx------   0 moyu       (501) staff       (20)        0 2022-10-06 05:53:46.000000 upload_machine-0.0.80/upload_machine/utils/pathinfo/__init__.py
--rwx------   0 moyu       (501) staff       (20)    26791 2023-08-06 07:37:26.000000 upload_machine-0.0.80/upload_machine/utils/pathinfo/pathinfo.py
-drwxr-xr-x   0 moyu       (501) staff       (20)        0 2023-08-06 09:32:49.358236 upload_machine-0.0.80/upload_machine/utils/rss_ctrl/
--rwx------   0 moyu       (501) staff       (20)        0 2022-10-06 05:53:46.000000 upload_machine-0.0.80/upload_machine/utils/rss_ctrl/__init__.py
-drwxr-xr-x   0 moyu       (501) staff       (20)        0 2023-08-06 09:32:49.360288 upload_machine-0.0.80/upload_machine/utils/seed_machine/
--rwx------   0 moyu       (501) staff       (20)        0 2022-10-06 05:53:46.000000 upload_machine-0.0.80/upload_machine/utils/seed_machine/__init__.py
--rwx------   0 moyu       (501) staff       (20)    21911 2023-08-06 08:04:07.000000 upload_machine-0.0.80/upload_machine/utils/seed_machine/seed_machine.py
-drwxr-xr-x   0 moyu       (501) staff       (20)        0 2023-08-06 09:32:49.361836 upload_machine-0.0.80/upload_machine/utils/signer/
--rwx------   0 moyu       (501) staff       (20)        0 2022-10-06 05:53:46.000000 upload_machine-0.0.80/upload_machine/utils/signer/__init__.py
-drwxr-xr-x   0 moyu       (501) staff       (20)        0 2023-08-06 09:32:49.362722 upload_machine-0.0.80/upload_machine/utils/site/
--rwx------   0 moyu       (501) staff       (20)        0 2022-10-06 05:53:46.000000 upload_machine-0.0.80/upload_machine/utils/site/__init__.py
--rwx------   0 moyu       (501) staff       (20)     4302 2023-01-02 15:05:32.000000 upload_machine-0.0.80/upload_machine/utils/site/site.py
-drwxr-xr-x   0 moyu       (501) staff       (20)        0 2023-08-06 09:32:49.428348 upload_machine-0.0.80/upload_machine/utils/uploader/
--rwx------   0 moyu       (501) staff       (20)        0 2022-10-06 05:53:46.000000 upload_machine-0.0.80/upload_machine/utils/uploader/__init__.py
--rwx------   0 moyu       (501) staff       (20)     5800 2023-01-08 11:40:16.000000 upload_machine-0.0.80/upload_machine/utils/uploader/audience_upload.py
--rwx------   0 moyu       (501) staff       (20)     1706 2023-08-06 06:58:29.000000 upload_machine-0.0.80/upload_machine/utils/uploader/auto_upload.py
--rwx------   0 moyu       (501) staff       (20)     7397 2023-01-05 04:08:25.000000 upload_machine-0.0.80/upload_machine/utils/uploader/carpt_upload.py
--rw-r--r--   0 moyu       (501) staff       (20)     8198 2023-08-05 18:44:07.000000 upload_machine-0.0.80/upload_machine/utils/uploader/dajiao_upload.py
--rwx------   0 moyu       (501) staff       (20)    10309 2023-01-06 12:18:37.000000 upload_machine-0.0.80/upload_machine/utils/uploader/hares_upload.py
--rwx------   0 moyu       (501) staff       (20)     8922 2023-01-08 11:39:46.000000 upload_machine-0.0.80/upload_machine/utils/uploader/hdfans_upload.py
--rwx------   0 moyu       (501) staff       (20)     6032 2023-01-05 04:08:36.000000 upload_machine-0.0.80/upload_machine/utils/uploader/hdpt_upload.py
--rwx------   0 moyu       (501) staff       (20)     7263 2023-01-06 12:18:50.000000 upload_machine-0.0.80/upload_machine/utils/uploader/hdsky_upload.py
--rwx------   0 moyu       (501) staff       (20)     8357 2023-08-06 09:24:01.000000 upload_machine-0.0.80/upload_machine/utils/uploader/hdvideo_upload.py
--rwx------   0 moyu       (501) staff       (20)     9220 2023-01-06 12:18:58.000000 upload_machine-0.0.80/upload_machine/utils/uploader/hhclub_upload.py
--rwx------   0 moyu       (501) staff       (20)     8642 2023-01-06 12:19:01.000000 upload_machine-0.0.80/upload_machine/utils/uploader/ihdbits_upload.py
--rwx------   0 moyu       (501) staff       (20)    19758 2023-01-11 18:07:47.000000 upload_machine-0.0.80/upload_machine/utils/uploader/lemonhd_upload.py
--rwx------   0 moyu       (501) staff       (20)     7123 2023-01-06 12:19:07.000000 upload_machine-0.0.80/upload_machine/utils/uploader/mteam_upload.py
--rw-r--r--   0 moyu       (501) staff       (20)     8728 2023-08-05 18:44:22.000000 upload_machine-0.0.80/upload_machine/utils/uploader/pandapt_upload.py
--rwx------   0 moyu       (501) staff       (20)     7926 2023-02-12 10:09:06.000000 upload_machine-0.0.80/upload_machine/utils/uploader/piggo_upload.py
--rwx------   0 moyu       (501) staff       (20)     4804 2023-01-05 04:09:08.000000 upload_machine-0.0.80/upload_machine/utils/uploader/pter_upload.py
--rwx------   0 moyu       (501) staff       (20)     8888 2023-05-14 16:45:46.000000 upload_machine-0.0.80/upload_machine/utils/uploader/redleaves_upload.py
--rw-r--r--   0 moyu       (501) staff       (20)     8379 2023-08-06 09:32:35.000000 upload_machine-0.0.80/upload_machine/utils/uploader/rousi_upload.py
--rwxr-xr-x   0 moyu       (501) staff       (20)     8322 2023-02-28 11:45:25.000000 upload_machine-0.0.80/upload_machine/utils/uploader/sharkpt_upload.py
--rwx------   0 moyu       (501) staff       (20)     7308 2023-01-11 18:11:31.000000 upload_machine-0.0.80/upload_machine/utils/uploader/ssd_upload.py
--rwx------   0 moyu       (501) staff       (20)    10649 2023-01-06 04:48:18.000000 upload_machine-0.0.80/upload_machine/utils/uploader/upload_tools.py
--rwx------   0 moyu       (501) staff       (20)     7707 2023-01-06 12:19:20.000000 upload_machine-0.0.80/upload_machine/utils/uploader/wintersakura_upload.py
--rwx------   0 moyu       (501) staff       (20)    10462 2023-01-06 17:28:21.000000 upload_machine-0.0.80/upload_machine/utils/uploader/zhuque_upload.py
--rwx------   0 moyu       (501) staff       (20)     7858 2023-01-08 11:39:12.000000 upload_machine-0.0.80/upload_machine/utils/uploader/zmpt_upload.py
-drwxr-xr-x   0 moyu       (501) staff       (20)        0 2023-08-06 09:32:49.330123 upload_machine-0.0.80/upload_machine.egg-info/
--rwx------   0 moyu       (501) staff       (20)    14608 2023-08-06 09:32:47.000000 upload_machine-0.0.80/upload_machine.egg-info/PKG-INFO
--rwx------   0 moyu       (501) staff       (20)     2814 2023-08-06 09:32:49.000000 upload_machine-0.0.80/upload_machine.egg-info/SOURCES.txt
--rwx------   0 moyu       (501) staff       (20)        1 2023-08-06 09:32:48.000000 upload_machine-0.0.80/upload_machine.egg-info/dependency_links.txt
--rwx------   0 moyu       (501) staff       (20)       90 2023-08-06 09:32:48.000000 upload_machine-0.0.80/upload_machine.egg-info/entry_points.txt
--rwx------   0 moyu       (501) staff       (20)      137 2023-08-06 09:32:48.000000 upload_machine-0.0.80/upload_machine.egg-info/requires.txt
--rwx------   0 moyu       (501) staff       (20)       15 2023-08-06 09:32:48.000000 upload_machine-0.0.80/upload_machine.egg-info/top_level.txt
+drwxr-xr-x   0 moyu       (501) staff       (20)        0 2023-08-06 09:48:53.642978 upload_machine-0.0.81/
+-rwx------   0 moyu       (501) staff       (20)     1063 2022-10-06 05:53:46.000000 upload_machine-0.0.81/LICENSE
+-rwx------   0 moyu       (501) staff       (20)       37 2022-10-06 08:50:43.000000 upload_machine-0.0.81/MANIFEST.in
+-rw-r--r--   0 moyu       (501) staff       (20)    14608 2023-08-06 09:48:53.640661 upload_machine-0.0.81/PKG-INFO
+-rwxr-xr-x   0 moyu       (501) staff       (20)    14206 2023-08-06 07:01:29.000000 upload_machine-0.0.81/README.md
+-rw-r--r--   0 moyu       (501) staff       (20)       38 2023-08-06 09:48:53.643117 upload_machine-0.0.81/setup.cfg
+-rwx------   0 moyu       (501) staff       (20)     1110 2023-08-06 09:48:42.000000 upload_machine-0.0.81/setup.py
+drwxr-xr-x   0 moyu       (501) staff       (20)        0 2023-08-06 09:48:53.574595 upload_machine-0.0.81/upload_machine/
+-rwx------   0 moyu       (501) staff       (20)        0 2022-10-06 05:53:46.000000 upload_machine-0.0.81/upload_machine/__init__.py
+-rwx------   0 moyu       (501) staff       (20)      241 2022-10-06 08:12:01.000000 upload_machine-0.0.81/upload_machine/basicinfo.yaml
+-rwx------   0 moyu       (501) staff       (20)     2622 2023-01-02 14:54:11.000000 upload_machine-0.0.81/upload_machine/main.py
+drwxr-xr-x   0 moyu       (501) staff       (20)        0 2023-08-06 09:48:53.579726 upload_machine-0.0.81/upload_machine/utils/
+-rwx------   0 moyu       (501) staff       (20)        0 2022-10-06 05:53:46.000000 upload_machine-0.0.81/upload_machine/utils/__init__.py
+drwxr-xr-x   0 moyu       (501) staff       (20)        0 2023-08-06 09:48:53.580718 upload_machine-0.0.81/upload_machine/utils/edittorrent/
+-rwx------   0 moyu       (501) staff       (20)        0 2022-10-06 05:53:46.000000 upload_machine-0.0.81/upload_machine/utils/edittorrent/__init__.py
+-rwx------   0 moyu       (501) staff       (20)     3966 2022-10-06 05:53:46.000000 upload_machine-0.0.81/upload_machine/utils/edittorrent/edittorrent.py
+drwxr-xr-x   0 moyu       (501) staff       (20)        0 2023-08-06 09:48:53.591312 upload_machine-0.0.81/upload_machine/utils/img_upload/
+-rwx------   0 moyu       (501) staff       (20)        0 2022-10-06 05:53:46.000000 upload_machine-0.0.81/upload_machine/utils/img_upload/__init__.py
+-rwx------   0 moyu       (501) staff       (20)     7231 2022-10-06 05:53:46.000000 upload_machine-0.0.81/upload_machine/utils/img_upload/chevereto.py
+-rwx------   0 moyu       (501) staff       (20)     2674 2022-10-06 05:53:46.000000 upload_machine-0.0.81/upload_machine/utils/img_upload/fapping_emp.py
+-rwx------   0 moyu       (501) staff       (20)     4521 2022-10-06 05:53:46.000000 upload_machine-0.0.81/upload_machine/utils/img_upload/imgbox.py
+-rwxr-xr-x   0 moyu       (501) staff       (20)     9014 2023-01-20 04:03:37.000000 upload_machine-0.0.81/upload_machine/utils/img_upload/imgupload.py
+-rwx------   0 moyu       (501) staff       (20)     2510 2022-10-06 05:53:46.000000 upload_machine-0.0.81/upload_machine/utils/img_upload/ptpimg.py
+-rwx------   0 moyu       (501) staff       (20)     1904 2022-11-06 06:50:27.000000 upload_machine-0.0.81/upload_machine/utils/img_upload/redleaves.py
+-rw-r--r--   0 moyu       (501) staff       (20)     2426 2023-01-20 04:03:37.000000 upload_machine-0.0.81/upload_machine/utils/img_upload/sharkimg.py
+-rwx------   0 moyu       (501) staff       (20)     2875 2022-10-06 05:53:46.000000 upload_machine-0.0.81/upload_machine/utils/img_upload/smms.py
+drwxr-xr-x   0 moyu       (501) staff       (20)        0 2023-08-06 09:48:53.597681 upload_machine-0.0.81/upload_machine/utils/mediafile/
+-rwx------   0 moyu       (501) staff       (20)        0 2022-10-06 05:53:46.000000 upload_machine-0.0.81/upload_machine/utils/mediafile/__init__.py
+-rwx------   0 moyu       (501) staff       (20)    17212 2022-10-06 05:53:46.000000 upload_machine-0.0.81/upload_machine/utils/mediafile/douban_book.py
+-rwx------   0 moyu       (501) staff       (20)    24814 2022-10-06 05:53:46.000000 upload_machine-0.0.81/upload_machine/utils/mediafile/douban_movie.py
+-rwx------   0 moyu       (501) staff       (20)     6861 2022-10-06 08:34:29.000000 upload_machine-0.0.81/upload_machine/utils/mediafile/doubaninfo.py
+-rw-r--r--   0 moyu       (501) staff       (20)     2418 2023-01-03 18:41:08.000000 upload_machine-0.0.81/upload_machine/utils/mediafile/maketorrent.py
+-rwx------   0 moyu       (501) staff       (20)    64920 2023-08-06 09:31:08.000000 upload_machine-0.0.81/upload_machine/utils/mediafile/mediafile.py
+drwxr-xr-x   0 moyu       (501) staff       (20)        0 2023-08-06 09:48:53.602498 upload_machine-0.0.81/upload_machine/utils/para_ctrl/
+-rwx------   0 moyu       (501) staff       (20)      218 2022-10-06 08:34:43.000000 upload_machine-0.0.81/upload_machine/utils/para_ctrl/__init__.py
+-rwx------   0 moyu       (501) staff       (20)     6779 2022-10-09 10:10:39.000000 upload_machine-0.0.81/upload_machine/utils/para_ctrl/para_ctrl.py
+-rwxr-xr-x   0 moyu       (501) staff       (20)     2154 2023-01-20 04:03:37.000000 upload_machine-0.0.81/upload_machine/utils/para_ctrl/readargs.py
+-rwx------   0 moyu       (501) staff       (20)     1901 2023-01-06 10:01:44.000000 upload_machine-0.0.81/upload_machine/utils/para_ctrl/readyaml.py
+drwxr-xr-x   0 moyu       (501) staff       (20)        0 2023-08-06 09:48:53.603636 upload_machine-0.0.81/upload_machine/utils/pathinfo/
+-rwx------   0 moyu       (501) staff       (20)        0 2022-10-06 05:53:46.000000 upload_machine-0.0.81/upload_machine/utils/pathinfo/__init__.py
+-rwx------   0 moyu       (501) staff       (20)    26791 2023-08-06 07:37:26.000000 upload_machine-0.0.81/upload_machine/utils/pathinfo/pathinfo.py
+drwxr-xr-x   0 moyu       (501) staff       (20)        0 2023-08-06 09:48:53.604832 upload_machine-0.0.81/upload_machine/utils/rss_ctrl/
+-rwx------   0 moyu       (501) staff       (20)        0 2022-10-06 05:53:46.000000 upload_machine-0.0.81/upload_machine/utils/rss_ctrl/__init__.py
+drwxr-xr-x   0 moyu       (501) staff       (20)        0 2023-08-06 09:48:53.605513 upload_machine-0.0.81/upload_machine/utils/seed_machine/
+-rwx------   0 moyu       (501) staff       (20)        0 2022-10-06 05:53:46.000000 upload_machine-0.0.81/upload_machine/utils/seed_machine/__init__.py
+-rwx------   0 moyu       (501) staff       (20)    21911 2023-08-06 08:04:07.000000 upload_machine-0.0.81/upload_machine/utils/seed_machine/seed_machine.py
+drwxr-xr-x   0 moyu       (501) staff       (20)        0 2023-08-06 09:48:53.607103 upload_machine-0.0.81/upload_machine/utils/signer/
+-rwx------   0 moyu       (501) staff       (20)        0 2022-10-06 05:53:46.000000 upload_machine-0.0.81/upload_machine/utils/signer/__init__.py
+drwxr-xr-x   0 moyu       (501) staff       (20)        0 2023-08-06 09:48:53.608390 upload_machine-0.0.81/upload_machine/utils/site/
+-rwx------   0 moyu       (501) staff       (20)        0 2022-10-06 05:53:46.000000 upload_machine-0.0.81/upload_machine/utils/site/__init__.py
+-rwx------   0 moyu       (501) staff       (20)     4302 2023-01-02 15:05:32.000000 upload_machine-0.0.81/upload_machine/utils/site/site.py
+drwxr-xr-x   0 moyu       (501) staff       (20)        0 2023-08-06 09:48:53.639604 upload_machine-0.0.81/upload_machine/utils/uploader/
+-rwx------   0 moyu       (501) staff       (20)        0 2022-10-06 05:53:46.000000 upload_machine-0.0.81/upload_machine/utils/uploader/__init__.py
+-rwx------   0 moyu       (501) staff       (20)     5800 2023-01-08 11:40:16.000000 upload_machine-0.0.81/upload_machine/utils/uploader/audience_upload.py
+-rwx------   0 moyu       (501) staff       (20)     1706 2023-08-06 06:58:29.000000 upload_machine-0.0.81/upload_machine/utils/uploader/auto_upload.py
+-rwx------   0 moyu       (501) staff       (20)     7397 2023-01-05 04:08:25.000000 upload_machine-0.0.81/upload_machine/utils/uploader/carpt_upload.py
+-rw-r--r--   0 moyu       (501) staff       (20)     8198 2023-08-05 18:44:07.000000 upload_machine-0.0.81/upload_machine/utils/uploader/dajiao_upload.py
+-rwx------   0 moyu       (501) staff       (20)    10309 2023-01-06 12:18:37.000000 upload_machine-0.0.81/upload_machine/utils/uploader/hares_upload.py
+-rwx------   0 moyu       (501) staff       (20)     8922 2023-01-08 11:39:46.000000 upload_machine-0.0.81/upload_machine/utils/uploader/hdfans_upload.py
+-rwx------   0 moyu       (501) staff       (20)     6032 2023-01-05 04:08:36.000000 upload_machine-0.0.81/upload_machine/utils/uploader/hdpt_upload.py
+-rwx------   0 moyu       (501) staff       (20)     7263 2023-01-06 12:18:50.000000 upload_machine-0.0.81/upload_machine/utils/uploader/hdsky_upload.py
+-rwx------   0 moyu       (501) staff       (20)     8361 2023-08-06 09:48:36.000000 upload_machine-0.0.81/upload_machine/utils/uploader/hdvideo_upload.py
+-rwx------   0 moyu       (501) staff       (20)     9220 2023-01-06 12:18:58.000000 upload_machine-0.0.81/upload_machine/utils/uploader/hhclub_upload.py
+-rwx------   0 moyu       (501) staff       (20)     8642 2023-01-06 12:19:01.000000 upload_machine-0.0.81/upload_machine/utils/uploader/ihdbits_upload.py
+-rwx------   0 moyu       (501) staff       (20)    19758 2023-01-11 18:07:47.000000 upload_machine-0.0.81/upload_machine/utils/uploader/lemonhd_upload.py
+-rwx------   0 moyu       (501) staff       (20)     7123 2023-01-06 12:19:07.000000 upload_machine-0.0.81/upload_machine/utils/uploader/mteam_upload.py
+-rw-r--r--   0 moyu       (501) staff       (20)     8728 2023-08-05 18:44:22.000000 upload_machine-0.0.81/upload_machine/utils/uploader/pandapt_upload.py
+-rwx------   0 moyu       (501) staff       (20)     7926 2023-02-12 10:09:06.000000 upload_machine-0.0.81/upload_machine/utils/uploader/piggo_upload.py
+-rwx------   0 moyu       (501) staff       (20)     4804 2023-01-05 04:09:08.000000 upload_machine-0.0.81/upload_machine/utils/uploader/pter_upload.py
+-rwx------   0 moyu       (501) staff       (20)     8888 2023-05-14 16:45:46.000000 upload_machine-0.0.81/upload_machine/utils/uploader/redleaves_upload.py
+-rw-r--r--   0 moyu       (501) staff       (20)     8379 2023-08-06 09:32:35.000000 upload_machine-0.0.81/upload_machine/utils/uploader/rousi_upload.py
+-rwxr-xr-x   0 moyu       (501) staff       (20)     8322 2023-02-28 11:45:25.000000 upload_machine-0.0.81/upload_machine/utils/uploader/sharkpt_upload.py
+-rwx------   0 moyu       (501) staff       (20)     7308 2023-01-11 18:11:31.000000 upload_machine-0.0.81/upload_machine/utils/uploader/ssd_upload.py
+-rwx------   0 moyu       (501) staff       (20)    10649 2023-01-06 04:48:18.000000 upload_machine-0.0.81/upload_machine/utils/uploader/upload_tools.py
+-rwx------   0 moyu       (501) staff       (20)     7707 2023-01-06 12:19:20.000000 upload_machine-0.0.81/upload_machine/utils/uploader/wintersakura_upload.py
+-rwx------   0 moyu       (501) staff       (20)    10462 2023-01-06 17:28:21.000000 upload_machine-0.0.81/upload_machine/utils/uploader/zhuque_upload.py
+-rwx------   0 moyu       (501) staff       (20)     7858 2023-01-08 11:39:12.000000 upload_machine-0.0.81/upload_machine/utils/uploader/zmpt_upload.py
+drwxr-xr-x   0 moyu       (501) staff       (20)        0 2023-08-06 09:48:53.578739 upload_machine-0.0.81/upload_machine.egg-info/
+-rwx------   0 moyu       (501) staff       (20)    14608 2023-08-06 09:48:52.000000 upload_machine-0.0.81/upload_machine.egg-info/PKG-INFO
+-rwx------   0 moyu       (501) staff       (20)     2814 2023-08-06 09:48:53.000000 upload_machine-0.0.81/upload_machine.egg-info/SOURCES.txt
+-rwx------   0 moyu       (501) staff       (20)        1 2023-08-06 09:48:52.000000 upload_machine-0.0.81/upload_machine.egg-info/dependency_links.txt
+-rwx------   0 moyu       (501) staff       (20)       90 2023-08-06 09:48:52.000000 upload_machine-0.0.81/upload_machine.egg-info/entry_points.txt
+-rwx------   0 moyu       (501) staff       (20)      137 2023-08-06 09:48:52.000000 upload_machine-0.0.81/upload_machine.egg-info/requires.txt
+-rwx------   0 moyu       (501) staff       (20)       15 2023-08-06 09:48:53.000000 upload_machine-0.0.81/upload_machine.egg-info/top_level.txt
```

### Comparing `upload_machine-0.0.80/LICENSE` & `upload_machine-0.0.81/LICENSE`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.80/PKG-INFO` & `upload_machine-0.0.81/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upload_machine
-Version: 0.0.80
+Version: 0.0.81
 Summary: Upload local resources to PT trackers automatically.
 Home-page: https://github.com/dongshuyan/Upload_Machine
 Author: sauterne
 Author-email: ssauterne@qq.com
 License: MIT Licence
 Keywords: pip,autoupload,auto,upload,PT,private tracker
 Platform: any
```

### Comparing `upload_machine-0.0.80/README.md` & `upload_machine-0.0.81/README.md`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.80/setup.py` & `upload_machine-0.0.81/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import io
 
 setup(
     name = "upload_machine",     
-    version = "0.0.80", 
+    version = "0.0.81", 
     keywords = ["pip", "autoupload","auto","upload","PT","private tracker"],            
     description = "Upload local resources to PT trackers automatically.",    
     long_description=io.open("README.md", "r", encoding='utf-8').read(),
     long_description_content_type="text/markdown",
     license = "MIT Licence",    
 
     entry_points = {
```

### Comparing `upload_machine-0.0.80/upload_machine/main.py` & `upload_machine-0.0.81/upload_machine/main.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.80/upload_machine/utils/edittorrent/edittorrent.py` & `upload_machine-0.0.81/upload_machine/utils/edittorrent/edittorrent.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.80/upload_machine/utils/img_upload/chevereto.py` & `upload_machine-0.0.81/upload_machine/utils/img_upload/chevereto.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.80/upload_machine/utils/img_upload/fapping_emp.py` & `upload_machine-0.0.81/upload_machine/utils/img_upload/fapping_emp.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.80/upload_machine/utils/img_upload/imgbox.py` & `upload_machine-0.0.81/upload_machine/utils/img_upload/imgbox.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.80/upload_machine/utils/img_upload/imgupload.py` & `upload_machine-0.0.81/upload_machine/utils/img_upload/imgupload.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.80/upload_machine/utils/img_upload/ptpimg.py` & `upload_machine-0.0.81/upload_machine/utils/img_upload/ptpimg.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.80/upload_machine/utils/img_upload/redleaves.py` & `upload_machine-0.0.81/upload_machine/utils/img_upload/redleaves.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.80/upload_machine/utils/img_upload/sharkimg.py` & `upload_machine-0.0.81/upload_machine/utils/img_upload/sharkimg.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.80/upload_machine/utils/img_upload/smms.py` & `upload_machine-0.0.81/upload_machine/utils/img_upload/smms.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.80/upload_machine/utils/mediafile/douban_book.py` & `upload_machine-0.0.81/upload_machine/utils/mediafile/douban_book.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.80/upload_machine/utils/mediafile/douban_movie.py` & `upload_machine-0.0.81/upload_machine/utils/mediafile/douban_movie.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.80/upload_machine/utils/mediafile/doubaninfo.py` & `upload_machine-0.0.81/upload_machine/utils/mediafile/doubaninfo.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.80/upload_machine/utils/mediafile/maketorrent.py` & `upload_machine-0.0.81/upload_machine/utils/mediafile/maketorrent.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.80/upload_machine/utils/mediafile/mediafile.py` & `upload_machine-0.0.81/upload_machine/utils/mediafile/mediafile.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.80/upload_machine/utils/para_ctrl/para_ctrl.py` & `upload_machine-0.0.81/upload_machine/utils/para_ctrl/para_ctrl.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.80/upload_machine/utils/para_ctrl/readargs.py` & `upload_machine-0.0.81/upload_machine/utils/para_ctrl/readargs.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.80/upload_machine/utils/para_ctrl/readyaml.py` & `upload_machine-0.0.81/upload_machine/utils/para_ctrl/readyaml.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.80/upload_machine/utils/pathinfo/pathinfo.py` & `upload_machine-0.0.81/upload_machine/utils/pathinfo/pathinfo.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.80/upload_machine/utils/seed_machine/seed_machine.py` & `upload_machine-0.0.81/upload_machine/utils/seed_machine/seed_machine.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.80/upload_machine/utils/site/site.py` & `upload_machine-0.0.81/upload_machine/utils/site/site.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.80/upload_machine/utils/uploader/audience_upload.py` & `upload_machine-0.0.81/upload_machine/utils/uploader/audience_upload.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.80/upload_machine/utils/uploader/auto_upload.py` & `upload_machine-0.0.81/upload_machine/utils/uploader/auto_upload.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.80/upload_machine/utils/uploader/carpt_upload.py` & `upload_machine-0.0.81/upload_machine/utils/uploader/carpt_upload.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.80/upload_machine/utils/uploader/dajiao_upload.py` & `upload_machine-0.0.81/upload_machine/utils/uploader/dajiao_upload.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.80/upload_machine/utils/uploader/hares_upload.py` & `upload_machine-0.0.81/upload_machine/utils/uploader/hares_upload.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.80/upload_machine/utils/uploader/hdfans_upload.py` & `upload_machine-0.0.81/upload_machine/utils/uploader/hdfans_upload.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.80/upload_machine/utils/uploader/hdpt_upload.py` & `upload_machine-0.0.81/upload_machine/utils/uploader/hdpt_upload.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.80/upload_machine/utils/uploader/hdsky_upload.py` & `upload_machine-0.0.81/upload_machine/utils/uploader/hdsky_upload.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.80/upload_machine/utils/uploader/hdvideo_upload.py` & `upload_machine-0.0.81/upload_machine/utils/uploader/hdvideo_upload.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,37 +110,37 @@
         codec_sel='6'
     else:
         codec_sel='6'
     logger.info('已成功选择编码为'+file1.Video_Format)
 
     #选择音频编码
     if file1.Audio_Format.upper()=='AAC':
-        audiocodec_sel='6'
+        audiocodec_sel='21'
     elif 'DTS-HDMA' in file1.Audio_Format.upper() or 'DTS-HD MA' in file1.Audio_Format.upper():
         audiocodec_sel='3'
     elif 'TRUEHD ATMOS' in file1.Audio_Format.upper():
-        audiocodec_sel='11'
+        audiocodec_sel='14'
     elif 'PCM' in file1.Audio_Format.upper():
         audiocodec_sel='8'
     elif 'TRUEHD' in file1.Audio_Format.upper():
         audiocodec_sel='11'
     elif 'FLAC' in file1.Audio_Format.upper():
         audiocodec_sel='1'
     elif 'APE' in file1.Audio_Format.upper():
         audiocodec_sel='2'
     elif 'MP3' in file1.Audio_Format.upper():
-        audiocodec_sel='7'
+        audiocodec_sel='18'
     elif 'AC3' in file1.Audio_Format.upper() or 'AC-3' in file1.Audio_Format.upper() or 'DD' in file1.Audio_Format.upper():
         audiocodec_sel='9'
     elif 'EAC3' in file1.Audio_Format.upper() or 'EAC-3' in file1.Audio_Format.upper() or 'DDP' in file1.Audio_Format.upper():
         audiocodec_sel='10'
     elif 'DTS:X' in file1.Audio_Format.upper() or 'DTS-X' in file1.Audio_Format.upper():
-        audiocodec_sel='3'
+        audiocodec_sel='16'
     elif 'DTS' in file1.Audio_Format.upper():
-        audiocodec_sel='3'
+        audiocodec_sel='17'
     elif 'WAV' in file1.Audio_Format.upper():
         audiocodec_sel='12'
     elif 'M4A' in file1.Audio_Format.upper():
         audiocodec_sel='7'
     elif 'OPUS' in file1.Audio_Format.upper():
         audiocodec_sel='5'
     else:
```

### Comparing `upload_machine-0.0.80/upload_machine/utils/uploader/hhclub_upload.py` & `upload_machine-0.0.81/upload_machine/utils/uploader/hhclub_upload.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.80/upload_machine/utils/uploader/ihdbits_upload.py` & `upload_machine-0.0.81/upload_machine/utils/uploader/ihdbits_upload.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.80/upload_machine/utils/uploader/lemonhd_upload.py` & `upload_machine-0.0.81/upload_machine/utils/uploader/lemonhd_upload.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.80/upload_machine/utils/uploader/mteam_upload.py` & `upload_machine-0.0.81/upload_machine/utils/uploader/mteam_upload.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.80/upload_machine/utils/uploader/pandapt_upload.py` & `upload_machine-0.0.81/upload_machine/utils/uploader/pandapt_upload.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.80/upload_machine/utils/uploader/piggo_upload.py` & `upload_machine-0.0.81/upload_machine/utils/uploader/piggo_upload.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.80/upload_machine/utils/uploader/pter_upload.py` & `upload_machine-0.0.81/upload_machine/utils/uploader/pter_upload.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.80/upload_machine/utils/uploader/redleaves_upload.py` & `upload_machine-0.0.81/upload_machine/utils/uploader/redleaves_upload.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.80/upload_machine/utils/uploader/rousi_upload.py` & `upload_machine-0.0.81/upload_machine/utils/uploader/rousi_upload.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.80/upload_machine/utils/uploader/sharkpt_upload.py` & `upload_machine-0.0.81/upload_machine/utils/uploader/sharkpt_upload.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.80/upload_machine/utils/uploader/ssd_upload.py` & `upload_machine-0.0.81/upload_machine/utils/uploader/ssd_upload.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.80/upload_machine/utils/uploader/upload_tools.py` & `upload_machine-0.0.81/upload_machine/utils/uploader/upload_tools.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.80/upload_machine/utils/uploader/wintersakura_upload.py` & `upload_machine-0.0.81/upload_machine/utils/uploader/wintersakura_upload.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.80/upload_machine/utils/uploader/zhuque_upload.py` & `upload_machine-0.0.81/upload_machine/utils/uploader/zhuque_upload.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.80/upload_machine/utils/uploader/zmpt_upload.py` & `upload_machine-0.0.81/upload_machine/utils/uploader/zmpt_upload.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.80/upload_machine.egg-info/PKG-INFO` & `upload_machine-0.0.81/upload_machine.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upload-machine
-Version: 0.0.80
+Version: 0.0.81
 Summary: Upload local resources to PT trackers automatically.
 Home-page: https://github.com/dongshuyan/Upload_Machine
 Author: sauterne
 Author-email: ssauterne@qq.com
 License: MIT Licence
 Keywords: pip,autoupload,auto,upload,PT,private tracker
 Platform: any
```

### Comparing `upload_machine-0.0.80/upload_machine.egg-info/SOURCES.txt` & `upload_machine-0.0.81/upload_machine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

