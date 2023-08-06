# Comparing `tmp/jag-panzer-0.1.24.tar.gz` & `tmp/jag-panzer-0.1.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jag-panzer-0.1.24.tar", last modified: Fri Jul 21 23:55:25 2023, max compression
+gzip compressed data, was "jag-panzer-0.1.31.tar", last modified: Sun Aug  6 06:56:56 2023, max compression
```

## Comparing `jag-panzer-0.1.24.tar` & `jag-panzer-0.1.31.tar`

### file list

```diff
@@ -1,104 +1,106 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 23:55:25.558403 jag-panzer-0.1.24/
--rw-rw-rw-   0        0        0      161 2023-06-09 00:40:57.000000 jag-panzer-0.1.24/LICENSE
--rw-rw-rw-   0        0        0       46 2023-06-09 02:05:06.000000 jag-panzer-0.1.24/MANIFEST.in
--rw-rw-rw-   0        0        0      561 2023-07-21 23:55:25.558403 jag-panzer-0.1.24/PKG-INFO
--rw-rw-rw-   0        0        0       26 2023-06-09 00:32:58.000000 jag-panzer-0.1.24/README.md
--rw-rw-rw-   0        0        0      108 2023-06-09 00:12:29.000000 jag-panzer-0.1.24/pyproject.toml
--rw-rw-rw-   0        0        0      672 2023-07-21 23:55:25.565400 jag-panzer-0.1.24/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-21 23:55:24.754725 jag-panzer-0.1.24/src/
-drwxrwxrwx   0        0        0        0 2023-07-21 23:55:24.846672 jag-panzer-0.1.24/src/jag_panzer/
--rw-rw-rw-   0        0        0        0 2023-06-11 10:49:01.000000 jag-panzer-0.1.24/src/jag_panzer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 23:55:24.887649 jag-panzer-0.1.24/src/jag_panzer/assets/
-drwxrwxrwx   0        0        0        0 2023-07-21 23:55:24.919631 jag-panzer-0.1.24/src/jag_panzer/assets/dir_listing/
--rw-rw-rw-   0        0        0      356 2023-06-08 21:39:34.000000 jag-panzer-0.1.24/src/jag_panzer/assets/dir_listing/base.html
--rw-rw-rw-   0        0        0      446 2023-06-06 00:39:53.000000 jag-panzer-0.1.24/src/jag_panzer/assets/dir_listing/dir_icon.svg
--rw-rw-rw-   0        0        0      682 2023-06-07 06:27:42.000000 jag-panzer-0.1.24/src/jag_panzer/assets/dir_listing/download_icon.svg
--rw-rw-rw-   0        0        0      704 2023-06-06 00:40:06.000000 jag-panzer-0.1.24/src/jag_panzer/assets/dir_listing/file_icon.svg
--rw-rw-rw-   0        0        0       21 2023-06-06 01:12:59.000000 jag-panzer-0.1.24/src/jag_panzer/assets/dir_listing/script.js
--rw-rw-rw-   0        0        0     1355 2023-06-07 07:34:01.000000 jag-panzer-0.1.24/src/jag_panzer/assets/dir_listing/style.css
--rw-rw-rw-   0        0        0      260 2023-06-07 02:18:15.000000 jag-panzer-0.1.24/src/jag_panzer/assets/reject.html
--rw-rw-rw-   0        0        0    21862 2023-07-21 23:54:46.000000 jag-panzer-0.1.24/src/jag_panzer/base_room.py
-drwxrwxrwx   0        0        0        0 2023-07-21 23:55:24.950614 jag-panzer-0.1.24/src/jag_panzer/cgi/
--rw-rw-rw-   0        0        0        0 2023-06-09 00:00:24.000000 jag-panzer-0.1.24/src/jag_panzer/cgi/__init__.py
--rw-rw-rw-   0        0        0     5087 2023-06-03 17:16:43.000000 jag-panzer-0.1.24/src/jag_panzer/cgi/burn_power.py
--rw-rw-rw-   0        0        0      451 2023-06-03 17:16:43.000000 jag-panzer-0.1.24/src/jag_panzer/cgi/hitman.py
--rw-rw-rw-   0        0        0     6691 2023-06-03 17:16:43.000000 jag-panzer-0.1.24/src/jag_panzer/cgi/jag.py
-drwxrwxrwx   0        0        0        0 2023-07-21 23:55:24.955609 jag-panzer-0.1.24/src/jag_panzer/cgi/templates/
-drwxrwxrwx   0        0        0        0 2023-07-21 23:55:24.957608 jag-panzer-0.1.24/src/jag_panzer/cgi/templates/light_httpd/
-drwxrwxrwx   0        0        0        0 2023-07-21 23:55:24.981596 jag-panzer-0.1.24/src/jag_panzer/cgi/templates/light_httpd/conf-enabled/
--rw-rw-rw-   0        0        0       91 2023-06-03 17:16:43.000000 jag-panzer-0.1.24/src/jag_panzer/cgi/templates/light_httpd/conf-enabled/10-accesslog.conf
--rw-rw-rw-   0        0        0      306 2023-06-03 17:16:43.000000 jag-panzer-0.1.24/src/jag_panzer/cgi/templates/light_httpd/conf-enabled/10-cgi.conf
--rw-rw-rw-   0        0        0      454 2023-06-03 17:16:43.000000 jag-panzer-0.1.24/src/jag_panzer/cgi/templates/light_httpd/conf-enabled/10-status.conf
--rw-rw-rw-   0        0        0     2245 2023-06-03 17:16:43.000000 jag-panzer-0.1.24/src/jag_panzer/cgi/templates/light_httpd/server_prms.conf
--rw-rw-rw-   0        0        0      403 2023-06-03 17:16:43.000000 jag-panzer-0.1.24/src/jag_panzer/cgi/templates/unit.service
--rw-rw-rw-   0        0        0     2539 2023-06-08 21:42:17.000000 jag-panzer-0.1.24/src/jag_panzer/dir_list.py
--rw-rw-rw-   0        0        0     2610 2023-07-12 20:58:31.000000 jag-panzer-0.1.24/src/jag_panzer/eztag.py
--rw-rw-rw-   0        0        0      456 2023-07-12 02:05:06.000000 jag-panzer-0.1.24/src/jag_panzer/jag_util.py
-drwxrwxrwx   0        0        0        0 2023-07-21 23:55:24.764719 jag-panzer-0.1.24/src/jag_panzer/libs/
-drwxrwxrwx   0        0        0        0 2023-07-21 23:55:25.059732 jag-panzer-0.1.24/src/jag_panzer/libs/bs4/
--rw-rw-rw-   0        0        0    33822 2023-06-06 00:22:44.000000 jag-panzer-0.1.24/src/jag_panzer/libs/bs4/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 23:55:25.100709 jag-panzer-0.1.24/src/jag_panzer/libs/bs4/builder/
--rw-rw-rw-   0        0        0    24393 2023-06-06 00:22:44.000000 jag-panzer-0.1.24/src/jag_panzer/libs/bs4/builder/__init__.py
--rw-rw-rw-   0        0        0    19078 2023-06-06 00:22:44.000000 jag-panzer-0.1.24/src/jag_panzer/libs/bs4/builder/_html5lib.py
--rw-rw-rw-   0        0        0    14919 2023-06-06 00:22:44.000000 jag-panzer-0.1.24/src/jag_panzer/libs/bs4/builder/_htmlparser.py
--rw-rw-rw-   0        0        0    14904 2023-06-06 00:22:44.000000 jag-panzer-0.1.24/src/jag_panzer/libs/bs4/builder/_lxml.py
--rw-rw-rw-   0        0        0    10077 2023-06-06 00:22:44.000000 jag-panzer-0.1.24/src/jag_panzer/libs/bs4/css.py
--rw-rw-rw-   0        0        0    41158 2023-06-06 00:22:44.000000 jag-panzer-0.1.24/src/jag_panzer/libs/bs4/dammit.py
--rw-rw-rw-   0        0        0     7195 2023-06-06 00:22:44.000000 jag-panzer-0.1.24/src/jag_panzer/libs/bs4/diagnose.py
--rw-rw-rw-   0        0        0    92716 2023-06-06 00:22:44.000000 jag-panzer-0.1.24/src/jag_panzer/libs/bs4/element.py
--rw-rw-rw-   0        0        0     7184 2023-06-06 00:22:44.000000 jag-panzer-0.1.24/src/jag_panzer/libs/bs4/formatter.py
-drwxrwxrwx   0        0        0        0 2023-07-21 23:55:25.315094 jag-panzer-0.1.24/src/jag_panzer/libs/bs4/tests/
--rw-rw-rw-   0        0        0    48391 2023-06-06 00:22:44.000000 jag-panzer-0.1.24/src/jag_panzer/libs/bs4/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 23:55:25.395986 jag-panzer-0.1.24/src/jag_panzer/libs/bs4/tests/fuzz/
--rw-rw-rw-   0        0        0       23 2023-06-06 00:22:44.000000 jag-panzer-0.1.24/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-4818336571064320.testcase
--rw-rw-rw-   0        0        0       30 2023-06-06 00:22:44.000000 jag-panzer-0.1.24/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-4999465949331456.testcase
--rw-rw-rw-   0        0        0    19469 2023-06-06 00:22:44.000000 jag-panzer-0.1.24/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-5167584867909632.testcase
--rw-rw-rw-   0        0        0        5 2023-06-06 00:22:44.000000 jag-panzer-0.1.24/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-5703933063462912.testcase
--rw-rw-rw-   0        0        0       35 2023-06-06 00:22:44.000000 jag-panzer-0.1.24/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-5843991618256896.testcase
--rw-rw-rw-   0        0        0    51495 2023-06-06 00:22:44.000000 jag-panzer-0.1.24/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-5984173902397440.testcase
--rw-rw-rw-   0        0        0    10380 2023-06-06 00:22:44.000000 jag-panzer-0.1.24/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-6124268085182464.testcase
--rw-rw-rw-   0        0        0       19 2023-06-06 00:22:44.000000 jag-panzer-0.1.24/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-6241471367348224.testcase
--rw-rw-rw-   0        0        0     3546 2023-06-06 00:22:44.000000 jag-panzer-0.1.24/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-6450958476902400.testcase
--rw-rw-rw-   0        0        0      124 2023-06-06 00:22:44.000000 jag-panzer-0.1.24/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-6600557255327744.testcase
--rw-rw-rw-   0        0        0     2607 2023-06-06 00:22:44.000000 jag-panzer-0.1.24/src/jag_panzer/libs/bs4/tests/fuzz/crash-0d306a50c8ed8bcd0785b67000fcd5dea1d33f08.testcase
--rw-rw-rw-   0        0        0     1115 2023-06-06 00:22:44.000000 jag-panzer-0.1.24/src/jag_panzer/libs/bs4/tests/test_builder.py
--rw-rw-rw-   0        0        0     5114 2023-06-06 00:22:44.000000 jag-panzer-0.1.24/src/jag_panzer/libs/bs4/tests/test_builder_registry.py
--rw-rw-rw-   0        0        0    17279 2023-06-06 00:22:44.000000 jag-panzer-0.1.24/src/jag_panzer/libs/bs4/tests/test_css.py
--rw-rw-rw-   0        0        0    15451 2023-06-06 00:22:44.000000 jag-panzer-0.1.24/src/jag_panzer/libs/bs4/tests/test_dammit.py
--rw-rw-rw-   0        0        0     1127 2023-06-06 00:22:44.000000 jag-panzer-0.1.24/src/jag_panzer/libs/bs4/tests/test_docs.py
--rw-rw-rw-   0        0        0     2377 2023-06-06 00:22:44.000000 jag-panzer-0.1.24/src/jag_panzer/libs/bs4/tests/test_element.py
--rw-rw-rw-   0        0        0     4148 2023-06-06 00:22:44.000000 jag-panzer-0.1.24/src/jag_panzer/libs/bs4/tests/test_formatter.py
--rw-rw-rw-   0        0        0     3637 2023-06-06 00:22:44.000000 jag-panzer-0.1.24/src/jag_panzer/libs/bs4/tests/test_fuzz.py
--rw-rw-rw-   0        0        0     8322 2023-06-06 00:22:44.000000 jag-panzer-0.1.24/src/jag_panzer/libs/bs4/tests/test_html5lib.py
--rw-rw-rw-   0        0        0     6256 2023-06-06 00:22:44.000000 jag-panzer-0.1.24/src/jag_panzer/libs/bs4/tests/test_htmlparser.py
--rw-rw-rw-   0        0        0     7635 2023-06-06 00:22:44.000000 jag-panzer-0.1.24/src/jag_panzer/libs/bs4/tests/test_lxml.py
--rw-rw-rw-   0        0        0     5081 2023-06-06 00:22:44.000000 jag-panzer-0.1.24/src/jag_panzer/libs/bs4/tests/test_navigablestring.py
--rw-rw-rw-   0        0        0    14274 2023-06-06 00:22:44.000000 jag-panzer-0.1.24/src/jag_panzer/libs/bs4/tests/test_pageelement.py
--rw-rw-rw-   0        0        0    19877 2023-06-06 00:22:44.000000 jag-panzer-0.1.24/src/jag_panzer/libs/bs4/tests/test_soup.py
--rw-rw-rw-   0        0        0     9016 2023-06-06 00:22:44.000000 jag-panzer-0.1.24/src/jag_panzer/libs/bs4/tests/test_tag.py
--rw-rw-rw-   0        0        0    48129 2023-06-06 00:22:44.000000 jag-panzer-0.1.24/src/jag_panzer/libs/bs4/tests/test_tree.py
-drwxrwxrwx   0        0        0        0 2023-07-21 23:55:25.468456 jag-panzer-0.1.24/src/jag_panzer/libs/soupsieve/
--rw-rw-rw-   0        0        0     4630 2023-06-06 00:22:44.000000 jag-panzer-0.1.24/src/jag_panzer/libs/soupsieve/__init__.py
--rw-rw-rw-   0        0        0     6842 2023-06-06 00:22:44.000000 jag-panzer-0.1.24/src/jag_panzer/libs/soupsieve/__meta__.py
--rw-rw-rw-   0        0        0    58152 2023-06-06 00:22:44.000000 jag-panzer-0.1.24/src/jag_panzer/libs/soupsieve/css_match.py
--rw-rw-rw-   0        0        0    47063 2023-06-06 00:22:44.000000 jag-panzer-0.1.24/src/jag_panzer/libs/soupsieve/css_parser.py
--rw-rw-rw-   0        0        0    10337 2023-06-06 00:22:44.000000 jag-panzer-0.1.24/src/jag_panzer/libs/soupsieve/css_types.py
--rw-rw-rw-   0        0        0     4053 2023-06-06 00:22:44.000000 jag-panzer-0.1.24/src/jag_panzer/libs/soupsieve/pretty.py
--rw-rw-rw-   0        0        0        0 2023-06-06 00:22:44.000000 jag-panzer-0.1.24/src/jag_panzer/libs/soupsieve/py.typed
--rw-rw-rw-   0        0        0     3374 2023-06-06 00:22:44.000000 jag-panzer-0.1.24/src/jag_panzer/libs/soupsieve/util.py
-drwxrwxrwx   0        0        0        0 2023-07-21 23:55:25.540413 jag-panzer-0.1.24/src/jag_panzer/libs/yattag/
--rw-rw-rw-   0        0        0     1743 2023-03-03 09:07:48.000000 jag-panzer-0.1.24/src/jag_panzer/libs/yattag/__init__.py
--rw-rw-rw-   0        0        0    18197 2020-08-06 21:26:32.000000 jag-panzer-0.1.24/src/jag_panzer/libs/yattag/doc.py
--rw-rw-rw-   0        0        0    12029 2023-01-02 11:12:52.000000 jag-panzer-0.1.24/src/jag_panzer/libs/yattag/indentation.py
--rw-rw-rw-   0        0        0        0 2019-12-25 20:07:02.000000 jag-panzer-0.1.24/src/jag_panzer/libs/yattag/py.typed
--rw-rw-rw-   0        0        0    18081 2019-12-24 00:01:02.000000 jag-panzer-0.1.24/src/jag_panzer/libs/yattag/simpledoc.py
-drwxrwxrwx   0        0        0        0 2023-07-21 23:55:25.542413 jag-panzer-0.1.24/src/jag_panzer/mimes/
--rw-rw-rw-   0        0        0     2762 2023-06-03 17:16:43.000000 jag-panzer-0.1.24/src/jag_panzer/mimes/mime_types_base.py
--rw-rw-rw-   0        0        0     1938 2023-06-03 17:16:43.000000 jag-panzer-0.1.24/src/jag_panzer/response_codes.py
--rw-rw-rw-   0        0        0     7874 2023-07-21 23:21:40.000000 jag-panzer-0.1.24/src/jag_panzer/server.py
--rwxrwxrwx   0        0        0       12 2023-06-07 01:47:22.000000 jag-panzer-0.1.24/src/jag_panzer/test.cmd
-drwxrwxrwx   0        0        0        0 2023-07-21 23:55:24.885650 jag-panzer-0.1.24/src/jag_panzer.egg-info/
--rw-rw-rw-   0        0        0      561 2023-07-21 23:55:24.000000 jag-panzer-0.1.24/src/jag_panzer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4010 2023-07-21 23:55:24.000000 jag-panzer-0.1.24/src/jag_panzer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 23:55:24.000000 jag-panzer-0.1.24/src/jag_panzer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-07-21 23:55:24.000000 jag-panzer-0.1.24/src/jag_panzer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-06 06:56:56.148529 jag-panzer-0.1.31/
+-rw-rw-rw-   0        0        0      161 2023-06-09 00:40:57.000000 jag-panzer-0.1.31/LICENSE
+-rw-rw-rw-   0        0        0       46 2023-06-09 02:05:06.000000 jag-panzer-0.1.31/MANIFEST.in
+-rw-rw-rw-   0        0        0      561 2023-08-06 06:56:56.149531 jag-panzer-0.1.31/PKG-INFO
+-rw-rw-rw-   0        0        0       26 2023-06-09 00:32:58.000000 jag-panzer-0.1.31/README.md
+-rw-rw-rw-   0        0        0      108 2023-06-09 00:12:29.000000 jag-panzer-0.1.31/pyproject.toml
+-rw-rw-rw-   0        0        0      672 2023-08-06 06:56:56.163520 jag-panzer-0.1.31/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-06 06:56:55.353984 jag-panzer-0.1.31/src/
+drwxrwxrwx   0        0        0        0 2023-08-06 06:56:55.571859 jag-panzer-0.1.31/src/jag_panzer/
+-rw-rw-rw-   0        0        0        0 2023-06-11 10:49:01.000000 jag-panzer-0.1.31/src/jag_panzer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-06 06:56:55.640819 jag-panzer-0.1.31/src/jag_panzer/assets/
+drwxrwxrwx   0        0        0        0 2023-08-06 06:56:55.690792 jag-panzer-0.1.31/src/jag_panzer/assets/dir_listing/
+-rw-rw-rw-   0        0        0      356 2023-06-08 21:39:34.000000 jag-panzer-0.1.31/src/jag_panzer/assets/dir_listing/base.html
+-rw-rw-rw-   0        0        0      446 2023-06-06 00:39:53.000000 jag-panzer-0.1.31/src/jag_panzer/assets/dir_listing/dir_icon.svg
+-rw-rw-rw-   0        0        0      682 2023-06-07 06:27:42.000000 jag-panzer-0.1.31/src/jag_panzer/assets/dir_listing/download_icon.svg
+-rw-rw-rw-   0        0        0      704 2023-06-06 00:40:06.000000 jag-panzer-0.1.31/src/jag_panzer/assets/dir_listing/file_icon.svg
+-rw-rw-rw-   0        0        0       21 2023-06-06 01:12:59.000000 jag-panzer-0.1.31/src/jag_panzer/assets/dir_listing/script.js
+-rw-rw-rw-   0        0        0     1355 2023-06-07 07:34:01.000000 jag-panzer-0.1.31/src/jag_panzer/assets/dir_listing/style.css
+-rw-rw-rw-   0        0        0      260 2023-06-07 02:18:15.000000 jag-panzer-0.1.31/src/jag_panzer/assets/reject.html
+-rw-rw-rw-   0        0        0    29090 2023-08-06 06:55:43.000000 jag-panzer-0.1.31/src/jag_panzer/base_room.py
+drwxrwxrwx   0        0        0        0 2023-08-06 06:56:55.747758 jag-panzer-0.1.31/src/jag_panzer/cgi/
+-rw-rw-rw-   0        0        0        0 2023-06-09 00:00:24.000000 jag-panzer-0.1.31/src/jag_panzer/cgi/__init__.py
+-rw-rw-rw-   0        0        0     5087 2023-06-03 17:16:43.000000 jag-panzer-0.1.31/src/jag_panzer/cgi/burn_power.py
+-rw-rw-rw-   0        0        0      451 2023-06-03 17:16:43.000000 jag-panzer-0.1.31/src/jag_panzer/cgi/hitman.py
+-rw-rw-rw-   0        0        0     6691 2023-06-03 17:16:43.000000 jag-panzer-0.1.31/src/jag_panzer/cgi/jag.py
+drwxrwxrwx   0        0        0        0 2023-08-06 06:56:55.753755 jag-panzer-0.1.31/src/jag_panzer/cgi/templates/
+drwxrwxrwx   0        0        0        0 2023-08-06 06:56:55.772745 jag-panzer-0.1.31/src/jag_panzer/cgi/templates/light_httpd/
+drwxrwxrwx   0        0        0        0 2023-08-06 06:56:55.809724 jag-panzer-0.1.31/src/jag_panzer/cgi/templates/light_httpd/conf-enabled/
+-rw-rw-rw-   0        0        0       91 2023-06-03 17:16:43.000000 jag-panzer-0.1.31/src/jag_panzer/cgi/templates/light_httpd/conf-enabled/10-accesslog.conf
+-rw-rw-rw-   0        0        0      306 2023-06-03 17:16:43.000000 jag-panzer-0.1.31/src/jag_panzer/cgi/templates/light_httpd/conf-enabled/10-cgi.conf
+-rw-rw-rw-   0        0        0      454 2023-06-03 17:16:43.000000 jag-panzer-0.1.31/src/jag_panzer/cgi/templates/light_httpd/conf-enabled/10-status.conf
+-rw-rw-rw-   0        0        0     2245 2023-06-03 17:16:43.000000 jag-panzer-0.1.31/src/jag_panzer/cgi/templates/light_httpd/server_prms.conf
+-rw-rw-rw-   0        0        0      403 2023-06-03 17:16:43.000000 jag-panzer-0.1.31/src/jag_panzer/cgi/templates/unit.service
+-rw-rw-rw-   0        0        0     2539 2023-06-08 21:42:17.000000 jag-panzer-0.1.31/src/jag_panzer/dir_list.py
+drwxrwxrwx   0        0        0        0 2023-08-06 06:56:55.813728 jag-panzer-0.1.31/src/jag_panzer/easy_timings/
+-rw-rw-rw-   0        0        0      537 2023-07-12 21:15:11.000000 jag-panzer-0.1.31/src/jag_panzer/easy_timings/mstime.py
+-rw-rw-rw-   0        0        0     2610 2023-07-12 20:58:31.000000 jag-panzer-0.1.31/src/jag_panzer/eztag.py
+-rw-rw-rw-   0        0        0      456 2023-07-12 02:05:06.000000 jag-panzer-0.1.31/src/jag_panzer/jag_util.py
+drwxrwxrwx   0        0        0        0 2023-08-06 06:56:55.410953 jag-panzer-0.1.31/src/jag_panzer/libs/
+drwxrwxrwx   0        0        0        0 2023-08-06 06:56:55.847701 jag-panzer-0.1.31/src/jag_panzer/libs/bs4/
+-rw-rw-rw-   0        0        0    33822 2023-06-06 00:22:44.000000 jag-panzer-0.1.31/src/jag_panzer/libs/bs4/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-06 06:56:55.893674 jag-panzer-0.1.31/src/jag_panzer/libs/bs4/builder/
+-rw-rw-rw-   0        0        0    24393 2023-06-06 00:22:44.000000 jag-panzer-0.1.31/src/jag_panzer/libs/bs4/builder/__init__.py
+-rw-rw-rw-   0        0        0    19078 2023-06-06 00:22:44.000000 jag-panzer-0.1.31/src/jag_panzer/libs/bs4/builder/_html5lib.py
+-rw-rw-rw-   0        0        0    14919 2023-06-06 00:22:44.000000 jag-panzer-0.1.31/src/jag_panzer/libs/bs4/builder/_htmlparser.py
+-rw-rw-rw-   0        0        0    14904 2023-06-06 00:22:44.000000 jag-panzer-0.1.31/src/jag_panzer/libs/bs4/builder/_lxml.py
+-rw-rw-rw-   0        0        0    10077 2023-06-06 00:22:44.000000 jag-panzer-0.1.31/src/jag_panzer/libs/bs4/css.py
+-rw-rw-rw-   0        0        0    41158 2023-06-06 00:22:44.000000 jag-panzer-0.1.31/src/jag_panzer/libs/bs4/dammit.py
+-rw-rw-rw-   0        0        0     7195 2023-06-06 00:22:44.000000 jag-panzer-0.1.31/src/jag_panzer/libs/bs4/diagnose.py
+-rw-rw-rw-   0        0        0    92716 2023-06-06 00:22:44.000000 jag-panzer-0.1.31/src/jag_panzer/libs/bs4/element.py
+-rw-rw-rw-   0        0        0     7184 2023-06-06 00:22:44.000000 jag-panzer-0.1.31/src/jag_panzer/libs/bs4/formatter.py
+drwxrwxrwx   0        0        0        0 2023-08-06 06:56:56.010609 jag-panzer-0.1.31/src/jag_panzer/libs/bs4/tests/
+-rw-rw-rw-   0        0        0    48391 2023-06-06 00:22:44.000000 jag-panzer-0.1.31/src/jag_panzer/libs/bs4/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-06 06:56:56.071573 jag-panzer-0.1.31/src/jag_panzer/libs/bs4/tests/fuzz/
+-rw-rw-rw-   0        0        0       23 2023-06-06 00:22:44.000000 jag-panzer-0.1.31/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-4818336571064320.testcase
+-rw-rw-rw-   0        0        0       30 2023-06-06 00:22:44.000000 jag-panzer-0.1.31/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-4999465949331456.testcase
+-rw-rw-rw-   0        0        0    19469 2023-06-06 00:22:44.000000 jag-panzer-0.1.31/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-5167584867909632.testcase
+-rw-rw-rw-   0        0        0        5 2023-06-06 00:22:44.000000 jag-panzer-0.1.31/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-5703933063462912.testcase
+-rw-rw-rw-   0        0        0       35 2023-06-06 00:22:44.000000 jag-panzer-0.1.31/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-5843991618256896.testcase
+-rw-rw-rw-   0        0        0    51495 2023-06-06 00:22:44.000000 jag-panzer-0.1.31/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-5984173902397440.testcase
+-rw-rw-rw-   0        0        0    10380 2023-06-06 00:22:44.000000 jag-panzer-0.1.31/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-6124268085182464.testcase
+-rw-rw-rw-   0        0        0       19 2023-06-06 00:22:44.000000 jag-panzer-0.1.31/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-6241471367348224.testcase
+-rw-rw-rw-   0        0        0     3546 2023-06-06 00:22:44.000000 jag-panzer-0.1.31/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-6450958476902400.testcase
+-rw-rw-rw-   0        0        0      124 2023-06-06 00:22:44.000000 jag-panzer-0.1.31/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-6600557255327744.testcase
+-rw-rw-rw-   0        0        0     2607 2023-06-06 00:22:44.000000 jag-panzer-0.1.31/src/jag_panzer/libs/bs4/tests/fuzz/crash-0d306a50c8ed8bcd0785b67000fcd5dea1d33f08.testcase
+-rw-rw-rw-   0        0        0     1115 2023-06-06 00:22:44.000000 jag-panzer-0.1.31/src/jag_panzer/libs/bs4/tests/test_builder.py
+-rw-rw-rw-   0        0        0     5114 2023-06-06 00:22:44.000000 jag-panzer-0.1.31/src/jag_panzer/libs/bs4/tests/test_builder_registry.py
+-rw-rw-rw-   0        0        0    17279 2023-06-06 00:22:44.000000 jag-panzer-0.1.31/src/jag_panzer/libs/bs4/tests/test_css.py
+-rw-rw-rw-   0        0        0    15451 2023-06-06 00:22:44.000000 jag-panzer-0.1.31/src/jag_panzer/libs/bs4/tests/test_dammit.py
+-rw-rw-rw-   0        0        0     1127 2023-06-06 00:22:44.000000 jag-panzer-0.1.31/src/jag_panzer/libs/bs4/tests/test_docs.py
+-rw-rw-rw-   0        0        0     2377 2023-06-06 00:22:44.000000 jag-panzer-0.1.31/src/jag_panzer/libs/bs4/tests/test_element.py
+-rw-rw-rw-   0        0        0     4148 2023-06-06 00:22:44.000000 jag-panzer-0.1.31/src/jag_panzer/libs/bs4/tests/test_formatter.py
+-rw-rw-rw-   0        0        0     3637 2023-06-06 00:22:44.000000 jag-panzer-0.1.31/src/jag_panzer/libs/bs4/tests/test_fuzz.py
+-rw-rw-rw-   0        0        0     8322 2023-06-06 00:22:44.000000 jag-panzer-0.1.31/src/jag_panzer/libs/bs4/tests/test_html5lib.py
+-rw-rw-rw-   0        0        0     6256 2023-06-06 00:22:44.000000 jag-panzer-0.1.31/src/jag_panzer/libs/bs4/tests/test_htmlparser.py
+-rw-rw-rw-   0        0        0     7635 2023-06-06 00:22:44.000000 jag-panzer-0.1.31/src/jag_panzer/libs/bs4/tests/test_lxml.py
+-rw-rw-rw-   0        0        0     5081 2023-06-06 00:22:44.000000 jag-panzer-0.1.31/src/jag_panzer/libs/bs4/tests/test_navigablestring.py
+-rw-rw-rw-   0        0        0    14274 2023-06-06 00:22:44.000000 jag-panzer-0.1.31/src/jag_panzer/libs/bs4/tests/test_pageelement.py
+-rw-rw-rw-   0        0        0    19877 2023-06-06 00:22:44.000000 jag-panzer-0.1.31/src/jag_panzer/libs/bs4/tests/test_soup.py
+-rw-rw-rw-   0        0        0     9016 2023-06-06 00:22:44.000000 jag-panzer-0.1.31/src/jag_panzer/libs/bs4/tests/test_tag.py
+-rw-rw-rw-   0        0        0    48129 2023-06-06 00:22:44.000000 jag-panzer-0.1.31/src/jag_panzer/libs/bs4/tests/test_tree.py
+drwxrwxrwx   0        0        0        0 2023-08-06 06:56:56.117547 jag-panzer-0.1.31/src/jag_panzer/libs/soupsieve/
+-rw-rw-rw-   0        0        0     4630 2023-06-06 00:22:44.000000 jag-panzer-0.1.31/src/jag_panzer/libs/soupsieve/__init__.py
+-rw-rw-rw-   0        0        0     6842 2023-06-06 00:22:44.000000 jag-panzer-0.1.31/src/jag_panzer/libs/soupsieve/__meta__.py
+-rw-rw-rw-   0        0        0    58152 2023-06-06 00:22:44.000000 jag-panzer-0.1.31/src/jag_panzer/libs/soupsieve/css_match.py
+-rw-rw-rw-   0        0        0    47063 2023-06-06 00:22:44.000000 jag-panzer-0.1.31/src/jag_panzer/libs/soupsieve/css_parser.py
+-rw-rw-rw-   0        0        0    10337 2023-06-06 00:22:44.000000 jag-panzer-0.1.31/src/jag_panzer/libs/soupsieve/css_types.py
+-rw-rw-rw-   0        0        0     4053 2023-06-06 00:22:44.000000 jag-panzer-0.1.31/src/jag_panzer/libs/soupsieve/pretty.py
+-rw-rw-rw-   0        0        0        0 2023-06-06 00:22:44.000000 jag-panzer-0.1.31/src/jag_panzer/libs/soupsieve/py.typed
+-rw-rw-rw-   0        0        0     3374 2023-06-06 00:22:44.000000 jag-panzer-0.1.31/src/jag_panzer/libs/soupsieve/util.py
+drwxrwxrwx   0        0        0        0 2023-08-06 06:56:56.141534 jag-panzer-0.1.31/src/jag_panzer/libs/yattag/
+-rw-rw-rw-   0        0        0     1743 2023-03-03 09:07:48.000000 jag-panzer-0.1.31/src/jag_panzer/libs/yattag/__init__.py
+-rw-rw-rw-   0        0        0    18197 2020-08-06 21:26:32.000000 jag-panzer-0.1.31/src/jag_panzer/libs/yattag/doc.py
+-rw-rw-rw-   0        0        0    12029 2023-01-02 11:12:52.000000 jag-panzer-0.1.31/src/jag_panzer/libs/yattag/indentation.py
+-rw-rw-rw-   0        0        0        0 2019-12-25 20:07:02.000000 jag-panzer-0.1.31/src/jag_panzer/libs/yattag/py.typed
+-rw-rw-rw-   0        0        0    18081 2019-12-24 00:01:02.000000 jag-panzer-0.1.31/src/jag_panzer/libs/yattag/simpledoc.py
+drwxrwxrwx   0        0        0        0 2023-08-06 06:56:56.145531 jag-panzer-0.1.31/src/jag_panzer/mimes/
+-rw-rw-rw-   0        0        0     2761 2023-08-01 12:22:23.000000 jag-panzer-0.1.31/src/jag_panzer/mimes/mime_types_base.py
+-rw-rw-rw-   0        0        0     1936 2023-08-01 12:24:05.000000 jag-panzer-0.1.31/src/jag_panzer/response_codes.py
+-rw-rw-rw-   0        0        0     8553 2023-08-06 06:46:46.000000 jag-panzer-0.1.31/src/jag_panzer/server.py
+-rwxrwxrwx   0        0        0       12 2023-06-07 01:47:22.000000 jag-panzer-0.1.31/src/jag_panzer/test.cmd
+drwxrwxrwx   0        0        0        0 2023-08-06 06:56:55.636822 jag-panzer-0.1.31/src/jag_panzer.egg-info/
+-rw-rw-rw-   0        0        0      561 2023-08-06 06:56:55.000000 jag-panzer-0.1.31/src/jag_panzer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4048 2023-08-06 06:56:55.000000 jag-panzer-0.1.31/src/jag_panzer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-06 06:56:55.000000 jag-panzer-0.1.31/src/jag_panzer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-08-06 06:56:55.000000 jag-panzer-0.1.31/src/jag_panzer.egg-info/top_level.txt
```

### Comparing `jag-panzer-0.1.24/PKG-INFO` & `jag-panzer-0.1.31/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jag-panzer
-Version: 0.1.24
+Version: 0.1.31
 Summary: Simple HTTP server allowing pure python workflow
 Home-page: https://github.com/MrKleiner/jag
 Author: Mr.Kleiner
 Author-email: megaadrenaline1055@gmail.com
 Project-URL: Bug Tracker, https://github.com/MrKleiner/jag/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jag-panzer-0.1.24/src/jag_panzer/assets/dir_listing/download_icon.svg` & `jag-panzer-0.1.31/src/jag_panzer/assets/dir_listing/download_icon.svg`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.24/src/jag_panzer/assets/dir_listing/file_icon.svg` & `jag-panzer-0.1.31/src/jag_panzer/assets/dir_listing/file_icon.svg`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.24/src/jag_panzer/assets/dir_listing/style.css` & `jag-panzer-0.1.31/src/jag_panzer/assets/dir_listing/style.css`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.24/src/jag_panzer/base_room.py` & `jag-panzer-0.1.31/src/jag_panzer/base_room.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 from pathlib import Path
 import sys
-# from mstime import perftest
+sys.path.append(str(Path(__file__).parent))
 
 
-sys.path.append(str(Path(__file__).parent))
 
 from jag_util import dict_pretty_print
 
 
 _room_echo = '[Request Evaluator]'
 _rebind = print
 
 
 def conlog(*args):
 	return
 	print(_room_echo, *args)
 
 
-
 def _default_room(request, response, services):
 	conlog('Executing default action', request.abspath)
 
 	# for this to work it has to be a GET request
 	if request.method == 'get':
 
 		# anything that is not inside the server shall get rejected
@@ -46,67 +44,179 @@
 
 
 	# otherwise - reject
 	request.reject()
 
 
 
+class perfrec:
+	def __init__(self, sv_timings, msg='perftest', _internal=False, noreport=False):
+		"""
+		- msg:str='perftest'   -> The name of the timing record
+		- ms:bool=True         -> Use milliseconds instead of seconds to record timing
+		- _internal:bool=False -> Wether the record is coming from jag itself or user
+		- noreport:bool=False  -> Don't write down the record
+		"""
+		self._internal = _internal
+		self.noreport = noreport
+		self.sv_timings = sv_timings
+
+		# time module
+		self.time = sv_timings.time
+		# timestamp of the beginning of the record
+		self.start = self.time.time()
+		# The name of the timing record
+		self.msg = msg
+		# Resulting timings
+		self.result = ('', 0)
+
+	def __enter__(self):
+		return self
+
+	def __exit__(self, type, value, traceback):
+		mtime = (self.time.time() - self.start) * 1000
+		self.result = (self.msg, mtime)
+
+		if not self.noreport:
+			if self._internal:
+				self.sv_timings.jag_time.append(self.result)
+			else:
+				self.sv_timings.timings.append(self.result)
+
+
+
+
+class server_timings:
+	"""
+	Various tools for measuring server performance.
+	
+	Timings are recorded at all times, but Server-Timing API
+	has to be explicitly enabled.
+
+	Ideally, the server should respond within ~100ms,
+	so try to measure performance in groups and not individual function calls.
+	"""
+	def __init__(self):
+		# time module
+		import time
+		self.time = time
+
+		# internal timings
+		self.jag_time = []
+		# custom timings
+		self.timings = []
+
+		# Inclusion of the Server-Timing response header
+		self.enable_header = False
+		# Whether to include internal Jag timings or not
+		self.header_incl_jag = False
+
+
+	def enable_in_response(self, include_jag_timings=False):
+		"""
+		Enable 'Server-Timing' header in response.
+		The system follows Server-Timing specs.
+		- include_jag_timings:bool=False -> whether to include internal Jag timings or not
+
+		It's ok to call this function myltiple times.
+		"""
+		self.enable_header = True
+		self.header_incl_jag = include_jag_timings
+
+
+	def record(self, msg='perftest', noreport=False, _internal=False):
+		"""
+		- msg:str='perftest'   -> The name of the timing record
+		- noreport:bool=False  -> Don't write down the record
+		"""
+		return perfrec(self, msg, _internal, noreport)
+
+
+	def push_record(self, record, _internal=False):
+		"""
+		Manually add an abstract record.
+		Format: tuple(message:str, timing:int|float|str)
+		"""
+		if _internal:
+			self.jag_time.append(record)
+		else:
+			self.timings.append(record)
+
+
+	def as_header(self, only_value=True):
+		records = []
+		for rec in self.jag_time:
+			records.append(f'''{rec[0]};dur={rec[1]}''')
+		for rec in self.timings:
+			records.append(f'''{rec[0]};dur={rec[1]}''')
+
+		if only_value:
+			return ', '.join(records)
+		else:
+			return f"""Server-Timings: {', '.join(records)}"""
+
+
 class sv_services:
 	"""
 	A bunch of default services the server can provide.
 	Most notable one: Serving GET requests
 	"""
 	def __init__(self, request, response):
 		self.request = request
 		self.response = response
+		self.srv_res = request.srv_res
 
 	# Serve a file to the client in a CDN manner
 	# If no file is provided - serve path from the request
 	def serve_file(self, tgt_file=None, respect_range=True, _force_oneflush=False):
 		"""
 		Serve a file to the client.
 		It's possible to specify a target file.
 		If no target file is specified, then reuqest path is used.
 		- tgt_file: Path to the file to serve, defaults to request path.
 		- respect_range: Take the "Range" header into account.
 		"""
 		request = self.request
 		response = self.response
 
-		if not request.abspath.is_file():
+		Path = self.srv_res.pylib.Path
+
+		if not tgt_file and not request.abspath.is_file():
 			self.request.reject()
 			return
+		tgt_file = Path(tgt_file or request.abspath)
 
 		# all good - set content type and send the shit
 		response.content_type = (
-			request.srv_res.mimes['signed'].get(request.abspath.suffix)
+			request.srv_res.mimes['signed'].get(tgt_file.suffix)
 			or
 			'application/octet-stream'
 		)
 
 		# Basically, debugging
 		if _force_oneflush:
-			response.flush_buffer(request.abspath.read_bytes())
+			response.flush_buffer(tgt_file.read_bytes())
 			self.request.terminate()
 			return
 
 		# if the size is too big for a single flush - stream in chunks
 		# This is very important, because serving a 2kb svg in chunks slows the response time
 		# and serving an 18gb .mkv Blu-Ray remux in a single flush is impossible
-		if request.abspath.stat().st_size > request.srv_res.cfg['buffers']['max_file_len']:
-			with open(str(request.abspath), 'r+b') as f:
+		if tgt_file.stat().st_size > request.srv_res.cfg['buffers']['max_file_len']:
+			with open(str(tgt_file), 'r+b') as f:
 				# if request comes with a Range header - try serving the requested byterange
 				# '0-' VERY funny, fuck right off
 				if request.byterange and (request.headers.get('range', 'bytes=0-').strip() != 'bytes=0-') and respect_range:
 					conlog('The client has fucked us over:', request.headers.get('range', '0-').strip())
 					response.serve_range(f)
 				else:
-					response.stream_buffer(f, (1024*1024)*5)
+					# response.stream_buffer(f, (1024*1024)*5)
+					response.stream_buffer(f, self.srv_res.cfg['buffers']['bufstream_chunk_len'])
 		else:
-			response.flush_buffer(request.abspath.read_bytes())
+			response.flush_buffer(tgt_file.read_bytes())
 
 		self.request.terminate()
 
 	# List directory as an html page
 	def list_dir(self):
 		"""
 		- Set content type to text/html
@@ -192,15 +302,15 @@
 
 # src  -----------------------
 # rng        ^         ^      
 # prog       -----            
 # want            ---------   
 # let             ------      
 
-# RANGES ARE INCLUSIVE IN HTTP !
+# RANGES ARE INCLUSIVE FROM BOTH SIDES IN HTTP !
 class aligned_buf_read:
 	def __init__(self, buf, start, end):
 		# START is inclusive
 		# END is NOT inclusive
 		self.buf = buf
 		self.start = start
 		self.end = end
@@ -222,43 +332,59 @@
 
 
 class sv_response:
 	def __init__(self, request, cl_con, srv_res):
 		self.request = request
 		self.cl_con = cl_con
 		self.srv_res = srv_res
+		self.timings = self.request.timings
 		self.headers = {
 			'Server': 'Jag',
+			# 'Server-Timings': '',
 		}
+		self.add_cookies = []
 
 		self.content_type = 'application/octet-stream'
 		self.code = 200
 
 		self.offered_services = sv_services(self.request, self)
 
-	# dump headers and response code to the client
+	# Dump headers and response code to the client
 	def send_preflight(self):
 		"""
 		Dump headers and response code to the client
 		"""
 
 		# send response code
 		self.cl_con.sendall(
-			f"""HTTP/1.1 {self.srv_res.response_codes[self.code]}\r\n""".encode()
+			f"""HTTP/1.1 {self.srv_res.response_codes.get(self.code, self.code)}\r\n""".encode()
 		)
 
 		# important todo: better way of achieving this
 		self.headers['Content-Type'] = self.content_type
 
+		if self.timings.enable_header:
+			self.headers['Server-Timing'] = self.timings.as_header()
+
 		# send headers
 		for header_name, header_value in self.headers.items():
 			self.cl_con.sendall(
 				f"""{header_name}: {header_value}\r\n""".encode()
 			)
 
+		# send cookies, if any
+		# important todo: this is very slow
+		if self.add_cookies:
+			cbuf = self.srv_res.pylib.io.BytesIO()
+			for cookie in self.add_cookies:
+				cbuf.write(b'Set-Cookie: ')
+				cbuf.write(cookie)
+				cbuf.write(b'\r\n')
+			self.cl_con.sendall(cbuf.getvalue())
+
 		# Send an extra \r\n to indicate the end of headers
 		self.cl_con.sendall('\r\n'.encode())
 
 		# important todo: There's a built-in way to make functions only fire once
 		# Yes, BUT, it costs A LOT of time and effort for the machine
 		# Such a simple buttplug is WAY more efficient
 		self.send_preflight = lambda: None
@@ -269,14 +395,20 @@
 		This is needed if you want the response body to be treated
 		as a file download by the client.
 		Useful when a media file, like .mp4 video should be downloaded
 		by the client instead of playing back.
 		"""
 		self.headers['Content-Disposition'] = f'attachment; filename="{str(filename)}"'
 
+	def set_filename(self, filename):
+		"""
+		Give content a name, but not mark it for download.
+		"""
+		self.headers['Content-Disposition'] = f'filename="{str(filename)}"'
+
 	# - Send headers to the client
 	# - Send the entirety of the provided buffer/bytes in one go
 	# - Collapse connection
 	def flush_buffer(self, data):
 		if not isinstance(data, bytes):
 			data = data.getvalue()
 
@@ -288,14 +420,41 @@
 
 		# send the body
 		self.cl_con.sendall(data)
 
 		# terminate
 		self.request.terminate()
 
+
+	def flush_json(self, jdata, bytes_to_array=False):
+		"""
+		Same as flush_buffer, except this function takes dictionaries as an input.
+		Sets Content-Type header to 'application/json'
+		This function also automatically encodes some commonly used types, such as:
+		pathlib > str
+		complex > tuple(c.real, c.imag)
+		"""
+		libs = self.srv_res.pylib
+		json = libs.json
+
+		# todo: use dicts to determine types
+		def complex_encoder(obj):
+			if isinstance(obj, libs.Path):
+				return str(obj)
+			elif isinstance(obj, complex):
+				return (obj.real, obj.imag)
+			else:
+				raise TypeError(f"""Object of type {obj.__class__.__name__} is not serializable""")
+
+		self.content_type = 'application/json'
+		self.flush_buffer(
+			json.dumps(jdata, default=complex_encoder).encode()
+		)
+
+
 	def stream_bytechunks(self, self_terminate=True):
 		"""
 		Stream data to the client in HTTP chunks:
 		- set 'Transfer-Encoding' header to 'chunked'
 		- Dump headers
 		- Start streaming chunks:
 			- This returns an object for use with "with" keyword.
@@ -378,30 +537,78 @@
 				while True:
 					data = aligned_reader.read(self.srv_res.cfg['buffers']['bufstream_chunk_len'])
 					if not data:
 						break
 					stream.send(data)
 
 
+	def set_cookie(self, cname, cval, domain=None, expires=None, secure=False, path=None, httponly=False, max_age=None, samesite=None):
+		"""
+		Adds one Set-Cookie header per call.
+		"expires" parameter accepts datetime objects.
+		"""
+		datetime = self.srv_res.pylib.datetime
+		wday_picker = ['Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat', 'Sun']
+		month_picker = [
+			'_',
+			'Jan',
+			'Feb',
+			'Mar',
+			'Apr',
+			'May',
+			'Jun',
+			'Jul',
+			'Aug',
+			'Sep',
+			'Oct',
+			'Nov',
+			'Dec',
+		]
+
+		cookie_buf = self.srv_res.pylib.io.BytesIO()
+		cookie_buf.write(f'{cname}={cval}'.encode())
+
+		if domain:
+			cookie_buf.write(f'; Domain={domain}'.encode())
+		if expires:
+			formatted_expires = expires
+			if isinstance(expires, datetime.datetime):
+				asutc = expires.astimezone(datetime.timezone.utc)
+				formatted_expires = f"""{wday_picker[asutc.weekday()]}, {asutc.day} {month_picker[asutc.month]} {asutc.year} {asutc.strftime('%H:%M:%S')} GMT"""
+			cookie_buf.write(f'; Expires={formatted_expires}'.encode())
+		if secure == True:
+			cookie_buf.write(b'; Secure')
+		if path:
+			cookie_buf.write(f'; Path={path}'.encode())
+		if httponly:
+			cookie_buf.write(b'; HttpOnly')
+		if max_age:
+			cookie_buf.write(f'; Max-Age={max_age}'.encode())
+		if samesite:
+			cookie_buf.write(f'; SameSite={samesite.capitalize()}'.encode())
+
+		self.add_cookies.append(cookie_buf.getvalue())
 
 
 
 
 class cl_request:
-	def __init__(self, cl_con, cl_addr, srv_res):
+	def __init__(self, cl_con, cl_addr, srv_res, timing_api):
 		self.cl_con = cl_con
 		self.cl_addr = cl_addr
 		self.srv_res = srv_res
+		self.timings = timing_api
 
 		self.headers = {}
 
 		# Initialize the response class
 		# Early init of this class is needed
 		# for rejecting certain requests
-		self.response = sv_response(self, cl_con, srv_res)
+		with self.timings.record('rsp_class_init', _internal=True):
+			self.response = sv_response(self, cl_con, srv_res)
 
 		# Some widely-used headers are lazily processed
 		# for easier use
 		self._cookie = None
 		self._cache_control = None
 		self._accept = None
 		self._byterange = None
@@ -482,59 +689,62 @@
 	def _eval_request(self):
 		# io = self.srv_res.pylib.io
 		# sys = self.srv_res.pylib.sys
 		urllib = self.srv_res.pylib.urllib
 		Path = self.srv_res.pylib.Path
 
 		# Fully custom method of receiving the Request Header
-		# gives a lot of benefits
-		self.collect_head_buf()
-
-		# raw bytes of the header
-		header_data = self.head_buf.getvalue()
-		conlog(header_data.decode())
-
-		# split header into lines
-		header_data = header_data.decode().split('\r\n')
-		conlog('\n'.join(header_data))
-
-		# First line of the header is always the request method, path and http version
-		# It's up to the client to send valid data
-		self.method, self.path, self.protocol = header_data[0].split(' ')
-		conlog(self.method, self.path, self.protocol)
-		self.method = self.method.lower()
-
-		# deconstruct the url into components
-		parsed_url = urllib.parse.urlparse(self.path)
-
-		# important todo: lazy processing
-		# first - evaluate query params
-		self.query_params = {k:(''.join(v)) for (k,v) in urllib.parse.parse_qs(parsed_url.query, True).items()}
-
-		# then, evaluate path
-		decoded_url_path = urllib.parse.unquote(parsed_url.path)
-		self.abspath = self.srv_res.doc_root / Path(decoded_url_path.lstrip('/'))
-		self.relpath = Path(decoded_url_path.lstrip('/'))
-		self.trimpath = self.relpath
-
-		# Delete the first line as it's no longer needed
-		del header_data[0]
-
-		# parse the remaining headers into a dict
-		request_dict = {}
-		for line in header_data:
-			# skip empty stuff
-			if line.strip() == '':
-				continue
-			line_split = line.split(': ')
-			request_dict[line_split[0].lower()] = ': '.join(line_split[1:])
+		# gives a lot of benefits (as well as causing mental retardation)
+		with self.timings.record('collect_hbuf', _internal=True):
+			self.collect_head_buf()
+
+
+		with self.timings.record('eval_hbuf', _internal=True):
+			# raw bytes of the header
+			header_data = self.head_buf.getvalue()
+			conlog(header_data.decode())
+
+			# split header into lines
+			header_data = header_data.decode().split('\r\n')
+			conlog('\n'.join(header_data))
+
+			# First line of the header is always the request method, path and http version
+			# It's up to the client to send valid data
+			self.method, self.path, self.protocol = header_data[0].split(' ')
+			conlog(self.method, self.path, self.protocol)
+			self.method = self.method.lower()
+
+			# deconstruct the url into components
+			parsed_url = urllib.parse.urlparse(self.path)
+
+			# important todo: lazy processing
+			# first - evaluate query params
+			self.query_params = {k:(''.join(v)) for (k,v) in urllib.parse.parse_qs(parsed_url.query, True).items()}
+
+			# then, evaluate path
+			decoded_url_path = urllib.parse.unquote(parsed_url.path)
+			self.abspath = self.srv_res.doc_root / Path(decoded_url_path.lstrip('/'))
+			self.relpath = Path(decoded_url_path.lstrip('/'))
+			self.trimpath = self.relpath
+
+			# Delete the first line as it's no longer needed
+			del header_data[0]
+
+			# parse the remaining headers into a dict
+			request_dict = {}
+			for line in header_data:
+				# skip empty stuff
+				if line.strip() == '':
+					continue
+				line_split = line.split(': ')
+				request_dict[line_split[0].lower()] = ': '.join(line_split[1:])
 
-		dict_pretty_print(request_dict)
+			dict_pretty_print(request_dict)
 
-		self.headers = request_dict
+			self.headers = request_dict
 
 
 	# Actions
 	# =================
 
 	# Properly collapse the tunnel between server and client
 	def terminate(self):
@@ -548,18 +758,33 @@
 	# Send a very simple html document
 	# with a short description of the provided Status Code
 	def reject(self, code=401, hint=''):
 		self.response.code = code
 		self.response.content_type = 'text/html'
 		self.response.flush_buffer(
 			self.srv_res.reject_precache
-			.replace(b'$$reason', self.srv_res.response_codes[code].encode())
+			.replace(b'$$reason', self.srv_res.response_codes.get(code, f'{code} ERROR').encode())
 			.replace(b'$$hint', str(hint).encode())
 		)
 
+	def redirect(self, target, reason=7, softlink=False):
+		"""
+		Redirect the request to the target destination.
+		- target: target URL to redirect to
+		- reason: 0-8 (300, 301, 302...), default to 7 (307)
+		- softlink: False = Location. True = Content-Location
+		"""
+		# self.srv_res.response_codes.get
+		reason_picker = {code:(300+code) for code in range(7)}
+		self.response.code = reason_picker.get(reason, 307)
+		self.response.headers['Content-Location' if hardlink else 'Location'] = str(target)
+
+		self.response.send_preflight()
+		self.terminate()
+
 	# I cannot be bothered. Here, have *args and fuckoff
 	def match_path(self, action_dict, *args, trim_path=True):
 		"""
 		Sample set/list:
 		{
 			('/pootis/sandwich/dispenser', func_name1),
 			('/pootis',                    func_name2),
@@ -571,14 +796,16 @@
 			# print(rpath, 'startswith', )
 			if comparator.startswith(rpath):
 				if trim_path:
 					self.trimpath = self.srv_res.pylib.Path(comparator.lstrip(rpath))
 				return func(self, self.response, self.response.offered_services, *args)
 
 		# if no match was found - return false
+		# todo: return some sort of a variable/class,
+		# so that it's more specific
 		return False
 
 
 	def read_body_stream(self):
 		"""
 		(Generator)
 		Progressively read body of the incoming request
@@ -599,14 +826,15 @@
 	def read_body(self, as_buf=False):
 		import io
 		buf = io.BytesIO()
 		for chunk in self.read_body_stream():
 			buf.write(chunk)
 
 		if as_buf:
+			buf.seek(0, 0)
 			return buf
 		else:
 			return buf.getvalue()
 
 
 	# Utility
 	# =================
@@ -712,61 +940,72 @@
 # The Base Room does some setup, like evaluating the request.
 # Further actions depend on the server setup:
 # If callback function is specified, then it's triggered
 # without any automatic actions
 # If callback function is NOT specified, then server provides
 # Some of its default services
 def base_room(cl_con, cl_addr, srv_res):
-	import sys, traceback
+	import sys, traceback, time
 	import importlib.util
 
 	try:
+		# Init timings
+		timing_api = server_timings()
+
+		timing_api.push_record(
+			('devtime', (time.time() - srv_res.devtime)*1000),
+			_internal=True
+		)
+
+		timing_api.enable_in_response(True)
+
 		# precache some commonly-used python libraries
 		# important todo: is this even needed?
-		srv_res.reload_libs()
+		with timing_api.record('lib_cache', _internal=True):
+			srv_res.reload_libs()
 
 		# Evaluate the request
-		evaluated_request = cl_request(cl_con, cl_addr, srv_res)
-
+		with timing_api.record('rq_eval', _internal=True):
+			evaluated_request = cl_request(cl_con, cl_addr, srv_res, timing_api)
 
 		conlog('Initialized basic room, evaluated request')
 
-		# Create service object
-		# offered_services = sv_services(evaluated_request, evaluated_request.response)
-
 		# Now either pass the control to the room specified in the config
 		# or the default room
 		if srv_res.cfg['room_file']:
-			spec = importlib.util.spec_from_file_location('main', str(srv_res.cfg['room_file']))
-			custom_func = importlib.util.module_from_spec(spec)
-			spec.loader.exec_module(custom_func)
+			with timing_api.record('spec', _internal=True):
+				spec = importlib.util.spec_from_file_location('main', str(srv_res.cfg['room_file']))
+				custom_func = importlib.util.module_from_spec(spec)
+				spec.loader.exec_module(custom_func)
 
 			custom_func.main(
 				evaluated_request,
 				evaluated_request.response,
 				evaluated_request.response.offered_services
 			)
 		else:
 			_default_room(
 				evaluated_request,
 				evaluated_request.response,
 				evaluated_request.response.offered_services
 			)
 
 	except Exception as err:
+
 		conlog(
 			''.join(
 				traceback.format_exception(
 					type(err),
 					err,
 					err.__traceback__
 				)
 			)
 		)
 
+
 		_trback = ''.join(
 			traceback.format_exception(
 				type(err),
 				err,
 				err.__traceback__
 			)
 		)
```

### Comparing `jag-panzer-0.1.24/src/jag_panzer/cgi/burn_power.py` & `jag-panzer-0.1.31/src/jag_panzer/cgi/burn_power.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.24/src/jag_panzer/cgi/jag.py` & `jag-panzer-0.1.31/src/jag_panzer/cgi/jag.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.24/src/jag_panzer/cgi/templates/light_httpd/server_prms.conf` & `jag-panzer-0.1.31/src/jag_panzer/cgi/templates/light_httpd/server_prms.conf`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.24/src/jag_panzer/dir_list.py` & `jag-panzer-0.1.31/src/jag_panzer/dir_list.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.24/src/jag_panzer/eztag.py` & `jag-panzer-0.1.31/src/jag_panzer/eztag.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.24/src/jag_panzer/libs/bs4/__init__.py` & `jag-panzer-0.1.31/src/jag_panzer/libs/bs4/__init__.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.24/src/jag_panzer/libs/bs4/builder/__init__.py` & `jag-panzer-0.1.31/src/jag_panzer/libs/bs4/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.24/src/jag_panzer/libs/bs4/builder/_html5lib.py` & `jag-panzer-0.1.31/src/jag_panzer/libs/bs4/builder/_html5lib.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.24/src/jag_panzer/libs/bs4/builder/_htmlparser.py` & `jag-panzer-0.1.31/src/jag_panzer/libs/bs4/builder/_htmlparser.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.24/src/jag_panzer/libs/bs4/builder/_lxml.py` & `jag-panzer-0.1.31/src/jag_panzer/libs/bs4/builder/_lxml.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.24/src/jag_panzer/libs/bs4/css.py` & `jag-panzer-0.1.31/src/jag_panzer/libs/bs4/css.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.24/src/jag_panzer/libs/bs4/dammit.py` & `jag-panzer-0.1.31/src/jag_panzer/libs/bs4/dammit.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.24/src/jag_panzer/libs/bs4/diagnose.py` & `jag-panzer-0.1.31/src/jag_panzer/libs/bs4/diagnose.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.24/src/jag_panzer/libs/bs4/element.py` & `jag-panzer-0.1.31/src/jag_panzer/libs/bs4/element.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.24/src/jag_panzer/libs/bs4/formatter.py` & `jag-panzer-0.1.31/src/jag_panzer/libs/bs4/formatter.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.24/src/jag_panzer/libs/bs4/tests/__init__.py` & `jag-panzer-0.1.31/src/jag_panzer/libs/bs4/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.24/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-5167584867909632.testcase` & `jag-panzer-0.1.31/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-5167584867909632.testcase`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.24/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-5984173902397440.testcase` & `jag-panzer-0.1.31/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-5984173902397440.testcase`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.24/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-6124268085182464.testcase` & `jag-panzer-0.1.31/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-6124268085182464.testcase`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.24/src/jag_panzer/libs/bs4/tests/fuzz/crash-0d306a50c8ed8bcd0785b67000fcd5dea1d33f08.testcase` & `jag-panzer-0.1.31/src/jag_panzer/libs/bs4/tests/fuzz/crash-0d306a50c8ed8bcd0785b67000fcd5dea1d33f08.testcase`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.24/src/jag_panzer/libs/bs4/tests/test_builder.py` & `jag-panzer-0.1.31/src/jag_panzer/libs/bs4/tests/test_builder.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.24/src/jag_panzer/libs/bs4/tests/test_builder_registry.py` & `jag-panzer-0.1.31/src/jag_panzer/libs/bs4/tests/test_builder_registry.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.24/src/jag_panzer/libs/bs4/tests/test_css.py` & `jag-panzer-0.1.31/src/jag_panzer/libs/bs4/tests/test_css.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.24/src/jag_panzer/libs/bs4/tests/test_dammit.py` & `jag-panzer-0.1.31/src/jag_panzer/libs/bs4/tests/test_dammit.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.24/src/jag_panzer/libs/bs4/tests/test_docs.py` & `jag-panzer-0.1.31/src/jag_panzer/libs/bs4/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.24/src/jag_panzer/libs/bs4/tests/test_element.py` & `jag-panzer-0.1.31/src/jag_panzer/libs/bs4/tests/test_element.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.24/src/jag_panzer/libs/bs4/tests/test_formatter.py` & `jag-panzer-0.1.31/src/jag_panzer/libs/bs4/tests/test_formatter.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.24/src/jag_panzer/libs/bs4/tests/test_fuzz.py` & `jag-panzer-0.1.31/src/jag_panzer/libs/bs4/tests/test_fuzz.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.24/src/jag_panzer/libs/bs4/tests/test_html5lib.py` & `jag-panzer-0.1.31/src/jag_panzer/libs/bs4/tests/test_html5lib.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.24/src/jag_panzer/libs/bs4/tests/test_htmlparser.py` & `jag-panzer-0.1.31/src/jag_panzer/libs/bs4/tests/test_htmlparser.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.24/src/jag_panzer/libs/bs4/tests/test_lxml.py` & `jag-panzer-0.1.31/src/jag_panzer/libs/bs4/tests/test_lxml.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.24/src/jag_panzer/libs/bs4/tests/test_navigablestring.py` & `jag-panzer-0.1.31/src/jag_panzer/libs/bs4/tests/test_navigablestring.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.24/src/jag_panzer/libs/bs4/tests/test_pageelement.py` & `jag-panzer-0.1.31/src/jag_panzer/libs/bs4/tests/test_pageelement.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.24/src/jag_panzer/libs/bs4/tests/test_soup.py` & `jag-panzer-0.1.31/src/jag_panzer/libs/bs4/tests/test_soup.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.24/src/jag_panzer/libs/bs4/tests/test_tag.py` & `jag-panzer-0.1.31/src/jag_panzer/libs/bs4/tests/test_tag.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.24/src/jag_panzer/libs/bs4/tests/test_tree.py` & `jag-panzer-0.1.31/src/jag_panzer/libs/bs4/tests/test_tree.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.24/src/jag_panzer/libs/soupsieve/__init__.py` & `jag-panzer-0.1.31/src/jag_panzer/libs/soupsieve/__init__.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.24/src/jag_panzer/libs/soupsieve/__meta__.py` & `jag-panzer-0.1.31/src/jag_panzer/libs/soupsieve/__meta__.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.24/src/jag_panzer/libs/soupsieve/css_match.py` & `jag-panzer-0.1.31/src/jag_panzer/libs/soupsieve/css_match.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.24/src/jag_panzer/libs/soupsieve/css_parser.py` & `jag-panzer-0.1.31/src/jag_panzer/libs/soupsieve/css_parser.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.24/src/jag_panzer/libs/soupsieve/css_types.py` & `jag-panzer-0.1.31/src/jag_panzer/libs/soupsieve/css_types.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.24/src/jag_panzer/libs/soupsieve/pretty.py` & `jag-panzer-0.1.31/src/jag_panzer/libs/soupsieve/pretty.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.24/src/jag_panzer/libs/soupsieve/util.py` & `jag-panzer-0.1.31/src/jag_panzer/libs/soupsieve/util.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.24/src/jag_panzer/libs/yattag/__init__.py` & `jag-panzer-0.1.31/src/jag_panzer/libs/yattag/__init__.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.24/src/jag_panzer/libs/yattag/doc.py` & `jag-panzer-0.1.31/src/jag_panzer/libs/yattag/doc.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.24/src/jag_panzer/libs/yattag/indentation.py` & `jag-panzer-0.1.31/src/jag_panzer/libs/yattag/indentation.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.24/src/jag_panzer/libs/yattag/simpledoc.py` & `jag-panzer-0.1.31/src/jag_panzer/libs/yattag/simpledoc.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.24/src/jag_panzer/mimes/mime_types_base.py` & `jag-panzer-0.1.31/src/jag_panzer/mimes/mime_types_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,8 +80,7 @@
 	'3g2':    'video/3gpp2; audio/3gpp2',
 	'7z':     'application/x-7z-compressed',
 }
 
 
 base_mimes_signed = {('.'+key):value for (key,value) in base_mimes.items()}
 
-
```

### Comparing `jag-panzer-0.1.24/src/jag_panzer/response_codes.py` & `jag-panzer-0.1.31/src/jag_panzer/response_codes.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,9 +68,7 @@
 	506: '506 Variant Also Negotiates',
 	507: '507 Insufficient Storage',
 	508: '508 Loop Detected',
 	510: '510 Not Extended',
 	511: '511 Network Authentication Required',
 }
 
-
-
```

### Comparing `jag-panzer-0.1.24/src/jag_panzer/server.py` & `jag-panzer-0.1.31/src/jag_panzer/server.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 # important todo: wat ?
 # (this library simply has to be a proper package)
 sys.path.append(str(Path(__file__).parent))
 
 from base_room import base_room
 import jag_util
 
+from easy_timings.mstime import perftest
 
 _main_init = '[root]'
 _server_proc = '[Server Process]'
 
 
 
 # Path
@@ -39,14 +40,15 @@
 		import base64
 		import struct
 		import io
 		import multiprocessing
 		import traceback
 		import urllib
 		import math
+		import datetime
 
 		from pathlib import Path
 
 		import jag_util
 
 		self.jag_util =  jag_util
 
@@ -59,14 +61,15 @@
 		self.json =      json
 		self.base64 =    base64
 		self.struct =    struct
 		self.io =        io
 		self.traceback = traceback
 		self.urllib =    urllib
 		self.math =      math
+		self.datetime =  datetime
 
 
 
 
 # sysroot         = Path-like pointing to the root of the jag package
 # pylib           = A bunch of precached python packages
 # mimes           = A dictionary of mime types; {file_ext:mime}
@@ -89,14 +92,16 @@
 		from mimes.mime_types_base import base_mimes_signed
 		from response_codes import codes as _rcodes
 
 		from pathlib import Path
 		import io
 		import jag_util
 
+		self.devtime = 0
+
 		config = init_config or {}
 
 		# root of the python package
 		self.sysroot = Path(__file__).parent
 
 		# extend python paths with included libs
 		sys.path.append(str(self.sysroot / 'libs'))
@@ -241,29 +246,36 @@
 
 	# Multiprocess pool automatically takes care of a bunch of stuff
 	# But most importantly, it takes care of shadow processess left after collapsed rooms
 	# (linux moment)
 
 	# EXCEPT, process pool is garbage: It's a pool with a fixed amount of workers,
 	# where tasks are distributed between them. Shit
-
-	# with multiprocessing.Pool() as pool:
-	print(_server_proc, 'Accepting connections... (7/7)')
-	while True:
-		# conlog('Entering the main listen cycle which would spawn rooms upon incoming connection requests...', echo=_server_proc)
-		# Try establishing connection, nothing below this line gets executed
-		# until server receives a new connection
-		conn, address = s.accept()
-		# conlog('Got connection, spawning a room. Client info:', address, echo=_server_proc)
-		# Create a basic room
-		# pool.apply_async(base_room, (conn, address, server_resources))
-
-		# conlog('Spawned a room, continue accepting new connections', echo=_server_proc)
-		# poot = multiprocessing.Process(target=base_room, args=(conn, address, server_resources,), daemon=True).start()
-		multiprocessing.Process(target=base_room, args=(conn, address, server_resources,), daemon=True).start()
+	# EXCEPT, the amount of workes can be specified manually
+	with multiprocessing.Pool(processes=32) as pool:
+		print(_server_proc, 'Accepting connections... (7/7)')
+		while True:
+			print('Waiting for requests...')
+			# conlog('Entering the main listen cycle which would spawn rooms upon incoming connection requests...', echo=_server_proc)
+			# Try establishing connection, nothing below this line gets executed
+			# until server receives a new connection
+			conn, address = s.accept()
+			# conlog('Got connection, spawning a room. Client info:', address, echo=_server_proc)
+			# Create a basic room
+			server_resources.devtime = time.time()
+			pool.apply_async(base_room, (conn, address, server_resources))
+			print('    Got request, forwarding...')
+			# conlog('Spawned a room, continue accepting new connections', echo=_server_proc)
+			# poot = multiprocessing.Process(target=base_room, args=(conn, address, server_resources,), daemon=True).start()
+			# with perftest('      Forking...'):
+			# 	multiprocessing.Process(target=base_room, args=(conn, address, server_resources,), daemon=True).start()
+			# 	multiprocessing.Process(target=base_room, args=(conn, address, server_resources), daemon=True).start()
+			# 	multiprocessing.Process(target=base_room, args=(conn, address, 'sex')).start()
+			# 	pool.apply_async(base_room, (conn, address, server_resources))
+			# 	pool.apply_async(base_room, (conn, address, server_resources))
 
 
 
 
 def server_process(srv_params, stfu=False):
 	print(_main_init, 'Creating and starting the server process... (1/7)')
 	# Create a new process containing the main incoming connections listener
```

### Comparing `jag-panzer-0.1.24/src/jag_panzer.egg-info/PKG-INFO` & `jag-panzer-0.1.31/src/jag_panzer.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jag-panzer
-Version: 0.1.24
+Version: 0.1.31
 Summary: Simple HTTP server allowing pure python workflow
 Home-page: https://github.com/MrKleiner/jag
 Author: Mr.Kleiner
 Author-email: megaadrenaline1055@gmail.com
 Project-URL: Bug Tracker, https://github.com/MrKleiner/jag/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jag-panzer-0.1.24/src/jag_panzer.egg-info/SOURCES.txt` & `jag-panzer-0.1.31/src/jag_panzer.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 src/jag_panzer/cgi/hitman.py
 src/jag_panzer/cgi/jag.py
 src/jag_panzer/cgi/templates/unit.service
 src/jag_panzer/cgi/templates/light_httpd/server_prms.conf
 src/jag_panzer/cgi/templates/light_httpd/conf-enabled/10-accesslog.conf
 src/jag_panzer/cgi/templates/light_httpd/conf-enabled/10-cgi.conf
 src/jag_panzer/cgi/templates/light_httpd/conf-enabled/10-status.conf
+src/jag_panzer/easy_timings/mstime.py
 src/jag_panzer/libs/bs4/__init__.py
 src/jag_panzer/libs/bs4/css.py
 src/jag_panzer/libs/bs4/dammit.py
 src/jag_panzer/libs/bs4/diagnose.py
 src/jag_panzer/libs/bs4/element.py
 src/jag_panzer/libs/bs4/formatter.py
 src/jag_panzer/libs/bs4/builder/__init__.py
```

