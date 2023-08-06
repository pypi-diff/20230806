# Comparing `tmp/maryam-2.5.2.tar.gz` & `tmp/maryam-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maryam-2.5.2.tar", last modified: Thu Jun 22 09:46:46 2023, max compression
+gzip compressed data, was "maryam-2.5.2.post1.tar", last modified: Sun Aug  6 09:39:58 2023, max compression
```

## Comparing `maryam-2.5.2.tar` & `maryam-2.5.2.post1.tar`

### file list

```diff
@@ -1,114 +1,188 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 09:46:46.646822 maryam-2.5.2/
--rw-r--r--   0 root         (0) root         (0)    35147 2023-06-22 07:37:52.000000 maryam-2.5.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-22 07:37:52.000000 maryam-2.5.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3373 2023-06-22 09:46:46.646822 maryam-2.5.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2671 2023-06-22 09:37:46.000000 maryam-2.5.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 09:46:46.630821 maryam-2.5.2/bin/
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-22 07:37:52.000000 maryam-2.5.2/bin/maryam
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 09:46:46.630821 maryam-2.5.2/maryam/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     1781 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 09:46:46.634821 maryam-2.5.2/maryam/core/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      103 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/basedir.py
--rwxr-xr-x   0 root         (0) root         (0)    25144 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/core.py
--rwxr-xr-x   0 root         (0) root         (0)    14486 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/initial.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 09:46:46.634821 maryam-2.5.2/maryam/core/util/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 09:46:46.634821 maryam-2.5.2/maryam/core/util/engines/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/engines/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1893 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/engines/baidu.py
--rw-r--r--   0 root         (0) root         (0)     5041 2023-06-22 08:17:28.000000 maryam-2.5.2/maryam/core/util/engines/bing.py
--rw-r--r--   0 root         (0) root         (0)     2506 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/engines/bing_images.py
--rw-r--r--   0 root         (0) root         (0)     3030 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/engines/carrot2.py
--rw-r--r--   0 root         (0) root         (0)     3198 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/engines/dogpile.py
--rw-r--r--   0 root         (0) root         (0)     4150 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/engines/duckduckgo.py
--rw-r--r--   0 root         (0) root         (0)     6609 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/engines/google.py
--rw-r--r--   0 root         (0) root         (0)     3386 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/engines/google_images.py
--rw-r--r--   0 root         (0) root         (0)     3603 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/engines/metacrawler.py
--rw-r--r--   0 root         (0) root         (0)     3427 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/engines/qwant.py
--rw-r--r--   0 root         (0) root         (0)     3177 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/engines/qwant_images.py
--rw-r--r--   0 root         (0) root         (0)     2955 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/engines/searx.py
--rw-r--r--   0 root         (0) root         (0)     3191 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/engines/startpage.py
--rw-r--r--   0 root         (0) root         (0)     3722 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/engines/yahoo.py
--rw-r--r--   0 root         (0) root         (0)     2143 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/engines/yandex.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 09:46:46.638821 maryam-2.5.2/maryam/core/util/footprint/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/footprint/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7471 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/footprint/cms_identify.py
--rw-r--r--   0 root         (0) root         (0)     2180 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/footprint/lang_identify.py
--rw-r--r--   0 root         (0) root         (0)     2380 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/footprint/os_identify.py
--rw-r--r--   0 root         (0) root         (0)    45321 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/footprint/waf_identify.py
--rw-r--r--   0 root         (0) root         (0)     5455 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/footprint/wapps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 09:46:46.638821 maryam-2.5.2/maryam/core/util/helpers/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/helpers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2831 2023-06-22 08:56:59.000000 maryam-2.5.2/maryam/core/util/helpers/keywords.py
--rw-r--r--   0 root         (0) root         (0)     9945 2023-06-22 08:42:20.000000 maryam-2.5.2/maryam/core/util/helpers/page_parse.py
--rw-r--r--   0 root         (0) root         (0)     4983 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/helpers/rand_uagent.py
--rw-r--r--   0 root         (0) root         (0)     3031 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/helpers/reglib.py
--rw-r--r--   0 root         (0) root         (0)     3410 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/helpers/urlib.py
--rw-r--r--   0 root         (0) root         (0)     9042 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/helpers/web_scrap.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 09:46:46.638821 maryam-2.5.2/maryam/core/util/iris/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/iris/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1269 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/iris/chart.py
--rw-r--r--   0 root         (0) root         (0)     3909 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/iris/cluster.py
--rw-r--r--   0 root         (0) root         (0)     2123 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/iris/meta_search_util.py
--rw-r--r--   0 root         (0) root         (0)     8046 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/iris/retriever.py
--rw-r--r--   0 root         (0) root         (0)     2329 2023-06-22 09:33:59.000000 maryam-2.5.2/maryam/core/util/iris/safe_searcher.py
--rw-r--r--   0 root         (0) root         (0)     2244 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/iris/tf_histogram.py
--rw-r--r--   0 root         (0) root         (0)     7419 2023-06-22 07:42:30.000000 maryam-2.5.2/maryam/core/util/iris/topic.py
--rw-r--r--   0 root         (0) root         (0)     1739 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/iris/word_cloud.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 09:46:46.642822 maryam-2.5.2/maryam/core/util/osint/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/osint/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1302 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/osint/ahmia.py
--rw-r--r--   0 root         (0) root         (0)     1849 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/osint/bing_mobile_view.py
--rw-r--r--   0 root         (0) root         (0)     2522 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/osint/darksearch.py
--rw-r--r--   0 root         (0) root         (0)     1896 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/osint/exalead.py
--rw-r--r--   0 root         (0) root         (0)     2544 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/osint/hunter.py
--rw-r--r--   0 root         (0) root         (0)     1740 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/osint/keyserver.py
--rw-r--r--   0 root         (0) root         (0)     2599 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/osint/netcraft.py
--rw-r--r--   0 root         (0) root         (0)     2390 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/osint/numverify.py
--rw-r--r--   0 root         (0) root         (0)     2019 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/osint/onionland.py
--rw-r--r--   0 root         (0) root         (0)     2798 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/osint/reddit.py
--rw-r--r--   0 root         (0) root         (0)     4758 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/osint/tweet_search.py
--rw-r--r--   0 root         (0) root         (0)     2151 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/osint/urlscan.py
--rw-r--r--   0 root         (0) root         (0)     1991 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/osint/virustotal.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 09:46:46.646822 maryam-2.5.2/maryam/core/util/search/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/search/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2670 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/search/arxiv.py
--rw-r--r--   0 root         (0) root         (0)     1850 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/search/ask.py
--rw-r--r--   0 root         (0) root         (0)     2335 2023-06-22 09:24:52.000000 maryam-2.5.2/maryam/core/util/search/core_ac.py
--rw-r--r--   0 root         (0) root         (0)     1570 2023-06-22 09:43:19.000000 maryam-2.5.2/maryam/core/util/search/crt.py
--rw-r--r--   0 root         (0) root         (0)     2015 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/search/dictionary.py
--rw-r--r--   0 root         (0) root         (0)     1875 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/search/discord.py
--rw-r--r--   0 root         (0) root         (0)     8393 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/search/instagram.py
--rw-r--r--   0 root         (0) root         (0)     2566 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/search/openstreetmap.py
--rw-r--r--   0 root         (0) root         (0)     3155 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/search/pastebin.py
--rw-r--r--   0 root         (0) root         (0)     1901 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/search/photon.py
--rw-r--r--   0 root         (0) root         (0)     2678 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/search/piratebay.py
--rw-r--r--   0 root         (0) root         (0)     2370 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/search/pubmed.py
--rw-r--r--   0 root         (0) root         (0)     3028 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/search/reddit_pushshift.py
--rw-r--r--   0 root         (0) root         (0)     5218 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/search/sanctionsearch.py
--rw-r--r--   0 root         (0) root         (0)     2132 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/search/scholar.py
--rw-r--r--   0 root         (0) root         (0)     2527 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/search/sepiasearch.py
--rw-r--r--   0 root         (0) root         (0)     2645 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/search/wikileaks.py
--rw-r--r--   0 root         (0) root         (0)     2569 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/search/wikipedia.py
--rw-r--r--   0 root         (0) root         (0)     3978 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/search/zlibrary.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 09:46:46.646822 maryam-2.5.2/maryam/core/web/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/web/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5330 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/web/api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 09:46:46.646822 maryam-2.5.2/maryam/data/
--rw-r--r--   0 root         (0) root         (0)     4782 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/data/dnsnames.txt
--rw-r--r--   0 root         (0) root         (0)      936 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/data/stopwords.csv
--rw-r--r--   0 root         (0) root         (0)    10201 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/data/tlds.txt
--rw-r--r--   0 root         (0) root         (0)    58532 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/data/username_checker.json
--rw-r--r--   0 root         (0) root         (0)   406174 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/data/wapps.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 09:46:46.646822 maryam-2.5.2/maryam/modules/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/modules/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 09:46:46.634821 maryam-2.5.2/maryam.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3373 2023-06-22 09:46:46.000000 maryam-2.5.2/maryam.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3204 2023-06-22 09:46:46.000000 maryam-2.5.2/maryam.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 09:46:46.000000 maryam-2.5.2/maryam.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      168 2023-06-22 09:46:46.000000 maryam-2.5.2/maryam.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-22 09:46:46.000000 maryam-2.5.2/maryam.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 09:46:46.646822 maryam-2.5.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1938 2023-06-22 09:38:14.000000 maryam-2.5.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 09:39:58.069723 maryam-2.5.2.post1/
+-rw-r--r--   0 root         (0) root         (0)    35147 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       22 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3379 2023-08-06 09:39:58.069723 maryam-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2671 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 09:39:58.041723 maryam-2.5.2.post1/bin/
+-rw-r--r--   0 root         (0) root         (0)      119 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/bin/maryam
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 09:39:58.041723 maryam-2.5.2.post1/maryam/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     1781 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 09:39:58.045723 maryam-2.5.2.post1/maryam/core/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      103 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/basedir.py
+-rwxr-xr-x   0 root         (0) root         (0)    25144 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/core.py
+-rwxr-xr-x   0 root         (0) root         (0)    14657 2023-08-06 09:36:49.000000 maryam-2.5.2.post1/maryam/core/initial.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 09:39:58.045723 maryam-2.5.2.post1/maryam/core/util/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/util/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 09:39:58.045723 maryam-2.5.2.post1/maryam/core/util/engines/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/util/engines/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1893 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/util/engines/baidu.py
+-rw-r--r--   0 root         (0) root         (0)     5041 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/util/engines/bing.py
+-rw-r--r--   0 root         (0) root         (0)     2506 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/util/engines/bing_images.py
+-rw-r--r--   0 root         (0) root         (0)     3030 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/util/engines/carrot2.py
+-rw-r--r--   0 root         (0) root         (0)     3198 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/util/engines/dogpile.py
+-rw-r--r--   0 root         (0) root         (0)     4150 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/util/engines/duckduckgo.py
+-rw-r--r--   0 root         (0) root         (0)     6609 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/util/engines/google.py
+-rw-r--r--   0 root         (0) root         (0)     3386 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/util/engines/google_images.py
+-rw-r--r--   0 root         (0) root         (0)     3603 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/util/engines/metacrawler.py
+-rw-r--r--   0 root         (0) root         (0)     3427 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/util/engines/qwant.py
+-rw-r--r--   0 root         (0) root         (0)     3177 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/util/engines/qwant_images.py
+-rw-r--r--   0 root         (0) root         (0)     2955 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/util/engines/searx.py
+-rw-r--r--   0 root         (0) root         (0)     3191 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/util/engines/startpage.py
+-rw-r--r--   0 root         (0) root         (0)     3722 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/util/engines/yahoo.py
+-rw-r--r--   0 root         (0) root         (0)     2143 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/util/engines/yandex.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 09:39:58.049723 maryam-2.5.2.post1/maryam/core/util/footprint/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/util/footprint/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7471 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/util/footprint/cms_identify.py
+-rw-r--r--   0 root         (0) root         (0)     2180 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/util/footprint/lang_identify.py
+-rw-r--r--   0 root         (0) root         (0)     2380 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/util/footprint/os_identify.py
+-rw-r--r--   0 root         (0) root         (0)    45321 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/util/footprint/waf_identify.py
+-rw-r--r--   0 root         (0) root         (0)     5455 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/util/footprint/wapps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 09:39:58.049723 maryam-2.5.2.post1/maryam/core/util/helpers/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/util/helpers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2831 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/util/helpers/keywords.py
+-rw-r--r--   0 root         (0) root         (0)     9945 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/util/helpers/page_parse.py
+-rw-r--r--   0 root         (0) root         (0)     4983 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/util/helpers/rand_uagent.py
+-rw-r--r--   0 root         (0) root         (0)     3031 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/util/helpers/reglib.py
+-rw-r--r--   0 root         (0) root         (0)     3410 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/util/helpers/urlib.py
+-rw-r--r--   0 root         (0) root         (0)     9042 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/util/helpers/web_scrap.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 09:39:58.049723 maryam-2.5.2.post1/maryam/core/util/iris/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/util/iris/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1269 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/util/iris/chart.py
+-rw-r--r--   0 root         (0) root         (0)     3909 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/util/iris/cluster.py
+-rw-r--r--   0 root         (0) root         (0)     2123 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/util/iris/meta_search_util.py
+-rw-r--r--   0 root         (0) root         (0)     8046 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/util/iris/retriever.py
+-rw-r--r--   0 root         (0) root         (0)     2329 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/util/iris/safe_searcher.py
+-rw-r--r--   0 root         (0) root         (0)     2244 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/util/iris/tf_histogram.py
+-rw-r--r--   0 root         (0) root         (0)     7419 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/util/iris/topic.py
+-rw-r--r--   0 root         (0) root         (0)     1739 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/util/iris/word_cloud.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 09:39:58.053723 maryam-2.5.2.post1/maryam/core/util/osint/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/util/osint/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1302 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/util/osint/ahmia.py
+-rw-r--r--   0 root         (0) root         (0)     1849 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/util/osint/bing_mobile_view.py
+-rw-r--r--   0 root         (0) root         (0)     2522 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/util/osint/darksearch.py
+-rw-r--r--   0 root         (0) root         (0)     1896 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/util/osint/exalead.py
+-rw-r--r--   0 root         (0) root         (0)     2544 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/util/osint/hunter.py
+-rw-r--r--   0 root         (0) root         (0)     1740 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/util/osint/keyserver.py
+-rw-r--r--   0 root         (0) root         (0)     2599 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/util/osint/netcraft.py
+-rw-r--r--   0 root         (0) root         (0)     2390 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/util/osint/numverify.py
+-rw-r--r--   0 root         (0) root         (0)     2019 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/util/osint/onionland.py
+-rw-r--r--   0 root         (0) root         (0)     2798 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/util/osint/reddit.py
+-rw-r--r--   0 root         (0) root         (0)     4758 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/util/osint/tweet_search.py
+-rw-r--r--   0 root         (0) root         (0)     2151 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/util/osint/urlscan.py
+-rw-r--r--   0 root         (0) root         (0)     1991 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/util/osint/virustotal.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 09:39:58.057723 maryam-2.5.2.post1/maryam/core/util/search/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/util/search/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2670 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/util/search/arxiv.py
+-rw-r--r--   0 root         (0) root         (0)     1850 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/util/search/ask.py
+-rw-r--r--   0 root         (0) root         (0)     2335 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/util/search/core_ac.py
+-rw-r--r--   0 root         (0) root         (0)     1570 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/util/search/crt.py
+-rw-r--r--   0 root         (0) root         (0)     2015 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/util/search/dictionary.py
+-rw-r--r--   0 root         (0) root         (0)     1875 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/util/search/discord.py
+-rw-r--r--   0 root         (0) root         (0)     8393 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/util/search/instagram.py
+-rw-r--r--   0 root         (0) root         (0)     2566 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/util/search/openstreetmap.py
+-rw-r--r--   0 root         (0) root         (0)     3155 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/util/search/pastebin.py
+-rw-r--r--   0 root         (0) root         (0)     1901 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/util/search/photon.py
+-rw-r--r--   0 root         (0) root         (0)     2678 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/util/search/piratebay.py
+-rw-r--r--   0 root         (0) root         (0)     2370 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/util/search/pubmed.py
+-rw-r--r--   0 root         (0) root         (0)     3028 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/util/search/reddit_pushshift.py
+-rw-r--r--   0 root         (0) root         (0)     5218 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/util/search/sanctionsearch.py
+-rw-r--r--   0 root         (0) root         (0)     2132 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/util/search/scholar.py
+-rw-r--r--   0 root         (0) root         (0)     2527 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/util/search/sepiasearch.py
+-rw-r--r--   0 root         (0) root         (0)     2645 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/util/search/wikileaks.py
+-rw-r--r--   0 root         (0) root         (0)     2569 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/util/search/wikipedia.py
+-rw-r--r--   0 root         (0) root         (0)     3978 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/util/search/zlibrary.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 09:39:58.057723 maryam-2.5.2.post1/maryam/core/web/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/web/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5330 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/core/web/api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 09:39:58.057723 maryam-2.5.2.post1/maryam/data/
+-rw-r--r--   0 root         (0) root         (0)     4782 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/data/dnsnames.txt
+-rw-r--r--   0 root         (0) root         (0)      936 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/data/stopwords.csv
+-rw-r--r--   0 root         (0) root         (0)    10201 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/data/tlds.txt
+-rw-r--r--   0 root         (0) root         (0)    58532 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/data/username_checker.json
+-rw-r--r--   0 root         (0) root         (0)   406174 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/data/wapps.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 09:39:58.057723 maryam-2.5.2.post1/maryam/modules/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/modules/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 09:39:58.057723 maryam-2.5.2.post1/maryam/modules/footprint/
+-rw-r--r--   0 root         (0) root         (0)     3723 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/modules/footprint/crawl_pages.py
+-rw-r--r--   0 root         (0) root         (0)     4954 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/modules/footprint/dnsbrute.py
+-rw-r--r--   0 root         (0) root         (0)     1895 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/modules/footprint/entry_points.py
+-rw-r--r--   0 root         (0) root         (0)     6351 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/modules/footprint/filebrute.py
+-rw-r--r--   0 root         (0) root         (0)    16954 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/modules/footprint/interest_files.py
+-rw-r--r--   0 root         (0) root         (0)     3266 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/modules/footprint/tldbrute.py
+-rw-r--r--   0 root         (0) root         (0)     1833 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/modules/footprint/wapps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 09:39:58.061723 maryam-2.5.2.post1/maryam/modules/iris/
+-rwxr-xr-x   0 root         (0) root         (0)     1502 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/modules/iris/cluster.py
+-rwxr-xr-x   0 root         (0) root         (0)     2551 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/modules/iris/iris.py
+-rwxr-xr-x   0 root         (0) root         (0)     1871 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/modules/iris/iris_cluster.py
+-rwxr-xr-x   0 root         (0) root         (0)     3088 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/modules/iris/sentiment.py
+-rwxr-xr-x   0 root         (0) root         (0)     2844 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/modules/iris/topicmodeling.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 09:39:58.061723 maryam-2.5.2.post1/maryam/modules/osint/
+-rw-r--r--   0 root         (0) root         (0)     1940 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/modules/osint/article_search.py
+-rw-r--r--   0 root         (0) root         (0)     2844 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/modules/osint/cloud_storage.py
+-rw-r--r--   0 root         (0) root         (0)     2575 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/modules/osint/crawler.py
+-rw-r--r--   0 root         (0) root         (0)     4112 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/modules/osint/cve_search.py
+-rw-r--r--   0 root         (0) root         (0)     9928 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/modules/osint/dark_web_crawler.py
+-rw-r--r--   0 root         (0) root         (0)    12297 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/modules/osint/dns_search.py
+-rw-r--r--   0 root         (0) root         (0)     2873 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/modules/osint/docs_search.py
+-rw-r--r--   0 root         (0) root         (0)     6388 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/modules/osint/domain_reputation.py
+-rw-r--r--   0 root         (0) root         (0)     2073 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/modules/osint/email_pwned.py
+-rw-r--r--   0 root         (0) root         (0)     3134 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/modules/osint/email_search.py
+-rw-r--r--   0 root         (0) root         (0)     6371 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/modules/osint/famous_person.py
+-rw-r--r--   0 root         (0) root         (0)     5437 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/modules/osint/github_leaks.py
+-rw-r--r--   0 root         (0) root         (0)     2087 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/modules/osint/image_search.py
+-rw-r--r--   0 root         (0) root         (0)     1503 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/modules/osint/onion_search.py
+-rw-r--r--   0 root         (0) root         (0)     1461 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/modules/osint/phone_number_search.py
+-rw-r--r--   0 root         (0) root         (0)     1635 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/modules/osint/reddit_search.py
+-rw-r--r--   0 root         (0) root         (0)     3376 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/modules/osint/social_nets.py
+-rw-r--r--   0 root         (0) root         (0)     1412 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/modules/osint/suggest.py
+-rw-r--r--   0 root         (0) root         (0)     4526 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/modules/osint/tweet_search.py
+-rw-r--r--   0 root         (0) root         (0)     3947 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/modules/osint/username_search.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 09:39:58.069723 maryam-2.5.2.post1/maryam/modules/search/
+-rw-r--r--   0 root         (0) root         (0)     1366 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/modules/search/arxiv.py
+-rw-r--r--   0 root         (0) root         (0)     1503 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/modules/search/bing.py
+-rw-r--r--   0 root         (0) root         (0)     1234 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/modules/search/carrot2.py
+-rw-r--r--   0 root         (0) root         (0)     1357 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/modules/search/core_ac.py
+-rw-r--r--   0 root         (0) root         (0)     1874 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/modules/search/crt.py
+-rw-r--r--   0 root         (0) root         (0)     1512 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/modules/search/dictionary.py
+-rw-r--r--   0 root         (0) root         (0)     2739 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/modules/search/discord.py
+-rw-r--r--   0 root         (0) root         (0)     1371 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/modules/search/dogpile.py
+-rw-r--r--   0 root         (0) root         (0)     1410 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/modules/search/duckduckgo.py
+-rw-r--r--   0 root         (0) root         (0)     3363 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/modules/search/facebook.py
+-rw-r--r--   0 root         (0) root         (0)     3671 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/modules/search/github.py
+-rw-r--r--   0 root         (0) root         (0)     1515 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/modules/search/google.py
+-rw-r--r--   0 root         (0) root         (0)     4596 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/modules/search/instagram.py
+-rw-r--r--   0 root         (0) root         (0)     2962 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/modules/search/linkedin.py
+-rw-r--r--   0 root         (0) root         (0)     1398 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/modules/search/metacrawler.py
+-rw-r--r--   0 root         (0) root         (0)     1479 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/modules/search/openstreetmap.py
+-rw-r--r--   0 root         (0) root         (0)     1759 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/modules/search/pastebin.py
+-rw-r--r--   0 root         (0) root         (0)     2562 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/modules/search/photon.py
+-rw-r--r--   0 root         (0) root         (0)     1454 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/modules/search/piratebay.py
+-rw-r--r--   0 root         (0) root         (0)     1407 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/modules/search/pubmed.py
+-rw-r--r--   0 root         (0) root         (0)     3256 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/modules/search/quora.py
+-rw-r--r--   0 root         (0) root         (0)     1359 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/modules/search/qwant.py
+-rw-r--r--   0 root         (0) root         (0)     4951 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/modules/search/reddit.py
+-rw-r--r--   0 root         (0) root         (0)     2212 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/modules/search/sanctionsearch.py
+-rw-r--r--   0 root         (0) root         (0)     1435 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/modules/search/scholar.py
+-rw-r--r--   0 root         (0) root         (0)     1359 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/modules/search/searx.py
+-rw-r--r--   0 root         (0) root         (0)     1581 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/modules/search/sepiasearch.py
+-rw-r--r--   0 root         (0) root         (0)     3294 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/modules/search/spotify.py
+-rw-r--r--   0 root         (0) root         (0)     3499 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/modules/search/stackoverflow.py
+-rw-r--r--   0 root         (0) root         (0)     1397 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/modules/search/startpage.py
+-rw-r--r--   0 root         (0) root         (0)     4650 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/modules/search/telegram.py
+-rw-r--r--   0 root         (0) root         (0)     3273 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/modules/search/tiktok.py
+-rw-r--r--   0 root         (0) root         (0)     3085 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/modules/search/trello.py
+-rw-r--r--   0 root         (0) root         (0)     3042 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/modules/search/twitter.py
+-rw-r--r--   0 root         (0) root         (0)     1607 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/modules/search/wikileaks.py
+-rw-r--r--   0 root         (0) root         (0)     2187 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/modules/search/wikipedia.py
+-rw-r--r--   0 root         (0) root         (0)     1516 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/modules/search/yahoo.py
+-rw-r--r--   0 root         (0) root         (0)     2887 2023-08-06 08:08:07.000000 maryam-2.5.2.post1/maryam/modules/search/youtube.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 09:39:58.045723 maryam-2.5.2.post1/maryam.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3379 2023-08-06 09:39:58.000000 maryam-2.5.2.post1/maryam.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5663 2023-08-06 09:39:58.000000 maryam-2.5.2.post1/maryam.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-06 09:39:58.000000 maryam-2.5.2.post1/maryam.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      168 2023-08-06 09:39:58.000000 maryam-2.5.2.post1/maryam.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-08-06 09:39:58.000000 maryam-2.5.2.post1/maryam.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-06 09:39:58.069723 maryam-2.5.2.post1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1903 2023-08-06 09:38:15.000000 maryam-2.5.2.post1/setup.py
```

### Comparing `maryam-2.5.2/LICENSE` & `maryam-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/PKG-INFO` & `maryam-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maryam
-Version: 2.5.2
+Version: 2.5.2.post1
 Summary: OWASP Maryam is a modular/optional open-source framework based on OSINT and data gathering.
 Home-page: https://github.com/saeeddhqan/Maryam
 Author: Saeed Dehqan
 Author-email: saeed.dehghan@owasp.org
 License: GPL-V3
 Keywords: OWASP,OSINT,search-engine,social-networks,Maryam
 Classifier: Programming Language :: Python :: 3.10
@@ -13,15 +13,15 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Environment :: Console
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Build Status](https://app.travis-ci.com/saeeddhqan/Maryam.svg?branch=master)](https://app.travis-ci.com/github/saeeddhqan/Maryam)
-![Version 2.5.2](https://img.shields.io/badge/Version-2.5.1-green.svg)
+![Version 2.5.2](https://img.shields.io/badge/Version-2.5.2-green.svg)
 ![GPLv3 License](https://img.shields.io/badge/License-GPLv3-green.svg)
 ![Python 3.10.x](https://img.shields.io/badge/Python-3.10.x-green.svg)
 [![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/4577/badge)](https://bestpractices.coreinfrastructure.org/projects/4577)
 
 # OWASP Maryam
 
 OWASP Maryam is a modular open-source framework based on OSINT and data gathering. It is designed to provide a robust environment to harvest data from open sources and search engines quickly and thoroughly.
```

### Comparing `maryam-2.5.2/README.md` & `maryam-2.5.2.post1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [![Build Status](https://app.travis-ci.com/saeeddhqan/Maryam.svg?branch=master)](https://app.travis-ci.com/github/saeeddhqan/Maryam)
-![Version 2.5.2](https://img.shields.io/badge/Version-2.5.1-green.svg)
+![Version 2.5.2](https://img.shields.io/badge/Version-2.5.2-green.svg)
 ![GPLv3 License](https://img.shields.io/badge/License-GPLv3-green.svg)
 ![Python 3.10.x](https://img.shields.io/badge/Python-3.10.x-green.svg)
 [![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/4577/badge)](https://bestpractices.coreinfrastructure.org/projects/4577)
 
 # OWASP Maryam
 
 OWASP Maryam is a modular open-source framework based on OSINT and data gathering. It is designed to provide a robust environment to harvest data from open sources and search engines quickly and thoroughly.
```

### Comparing `maryam-2.5.2/maryam/__main__.py` & `maryam-2.5.2.post1/maryam/__main__.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam/core/core.py` & `maryam-2.5.2.post1/maryam/core/core.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam/core/initial.py` & `maryam-2.5.2.post1/maryam/core/initial.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
-__version__ = 'v2.5.1'
+__version__ = 'v2.5.2'
 
 import argparse
-import imp
+import importlib
 import os
 import shutil
 import sys
 import shlex
 import json
 import concurrent.futures
 
@@ -97,54 +97,60 @@
 
 	def _init_home(self):
 		self._home = os.path.expanduser('~')
 		# initialize home folder
 		if not os.path.exists(self._home):
 			os.makedirs(self._home)
 
+	def _load_a_module(self, mod_name, mod_path):
+		spec = importlib.util.spec_from_file_location(mod_name, mod_path)
+		module = importlib.util.module_from_spec(spec)
+		spec.loader.exec_module(module)
+		return module
+
 	def _init_util_classes(self, require='*'):
 		util_path = os.path.join(self.core_path, 'util')
 		for dirpath, _, files in os.walk(util_path, followlinks=True):
 			if not dirpath.endswith(require) and require != '*' and util_path != dirpath: continue
 			for file in filter(lambda f: f.endswith('.py')\
 						and not f.startswith('__'), files):
 				mod_name = file.split('.')[0]
 				mod_path = os.path.join(dirpath, file)
 				try:
-					imp.load_source(mod_name, mod_path, open(mod_path)).main
+					module = self._load_a_module(mod_name, mod_path)
 				except Exception as e:
 					self.error(f"Util class '{mod_name}' has been disabled due to this error: {e}", 'initial', '_init_util_classes')
 				else:
-					exec(f"self.{mod_name} = sys.modules['{mod_name}'].main")
+					exec(f"self.{mod_name} = module.main")
 					exec(f"self.{mod_name}.framework = self")
 
 	def _load_modules(self, require='*'):
 		self.loaded_category = {}
 		self._loaded_modules = core._loaded_modules
 		self._init_util_classes(require)
 		for dirpath, dirnames, _ in os.walk(self.module_path, followlinks=True):
-			# Each Section
+			# Each section
 			for section in filter(lambda d: not d.startswith('__'), dirnames):
 				category = section
 				if require != category and require != '*': continue
 				self._cat_module_names[category] = []
 				section = os.path.join(dirpath, section)
 				for _, _, files in os.walk(section):
-					# Each File
+					# Each file
 					for file in filter(lambda f: f.endswith(self.module_ext) and not f.startswith('__'), files):
 						mod_path = os.path.join(section, file)
 						mod_load_name = f"__{file.split('.')[0]}"
 						mod_disp_name = file.split('.')[0]
 						try:
-							imp.load_source(mod_load_name, mod_path, open(mod_path))
+							module = self._load_a_module(mod_load_name, mod_path)
 						except Exception as e:
 							if not self._global_options['api_mode']:
 								self.error(f"Module name '{mod_disp_name}' has been disabled due to this error: {e}", 'initial', '_load_modules')
 						else:
-							self._loaded_modules[mod_disp_name] = sys.modules[mod_load_name]
+							self._loaded_modules[mod_disp_name] = module
 							self._cat_module_names[category].append(mod_disp_name)
 							self._module_names.append(mod_disp_name)
 
 	# ////////////////////////
 	#          API 		    //
 	# ////////////////////////
```

### Comparing `maryam-2.5.2/maryam/core/util/engines/baidu.py` & `maryam-2.5.2.post1/maryam/core/util/engines/baidu.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam/core/util/engines/bing.py` & `maryam-2.5.2.post1/maryam/core/util/engines/bing.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam/core/util/engines/bing_images.py` & `maryam-2.5.2.post1/maryam/core/util/engines/bing_images.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam/core/util/engines/carrot2.py` & `maryam-2.5.2.post1/maryam/core/util/engines/carrot2.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam/core/util/engines/dogpile.py` & `maryam-2.5.2.post1/maryam/core/util/engines/dogpile.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam/core/util/engines/duckduckgo.py` & `maryam-2.5.2.post1/maryam/core/util/engines/duckduckgo.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam/core/util/engines/google.py` & `maryam-2.5.2.post1/maryam/core/util/engines/google.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam/core/util/engines/google_images.py` & `maryam-2.5.2.post1/maryam/core/util/engines/google_images.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam/core/util/engines/metacrawler.py` & `maryam-2.5.2.post1/maryam/core/util/engines/metacrawler.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam/core/util/engines/qwant.py` & `maryam-2.5.2.post1/maryam/core/util/engines/qwant.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam/core/util/engines/qwant_images.py` & `maryam-2.5.2.post1/maryam/core/util/engines/qwant_images.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam/core/util/engines/searx.py` & `maryam-2.5.2.post1/maryam/core/util/engines/searx.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam/core/util/engines/startpage.py` & `maryam-2.5.2.post1/maryam/core/util/engines/startpage.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam/core/util/engines/yahoo.py` & `maryam-2.5.2.post1/maryam/core/util/engines/yahoo.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam/core/util/engines/yandex.py` & `maryam-2.5.2.post1/maryam/core/util/engines/yandex.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam/core/util/footprint/cms_identify.py` & `maryam-2.5.2.post1/maryam/core/util/footprint/cms_identify.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam/core/util/footprint/lang_identify.py` & `maryam-2.5.2.post1/maryam/core/util/footprint/lang_identify.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam/core/util/footprint/os_identify.py` & `maryam-2.5.2.post1/maryam/core/util/footprint/os_identify.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam/core/util/footprint/waf_identify.py` & `maryam-2.5.2.post1/maryam/core/util/footprint/waf_identify.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam/core/util/footprint/wapps.py` & `maryam-2.5.2.post1/maryam/core/util/footprint/wapps.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam/core/util/helpers/keywords.py` & `maryam-2.5.2.post1/maryam/core/util/helpers/keywords.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam/core/util/helpers/page_parse.py` & `maryam-2.5.2.post1/maryam/core/util/helpers/page_parse.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam/core/util/helpers/rand_uagent.py` & `maryam-2.5.2.post1/maryam/core/util/helpers/rand_uagent.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam/core/util/helpers/reglib.py` & `maryam-2.5.2.post1/maryam/core/util/helpers/reglib.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam/core/util/helpers/urlib.py` & `maryam-2.5.2.post1/maryam/core/util/helpers/urlib.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam/core/util/helpers/web_scrap.py` & `maryam-2.5.2.post1/maryam/core/util/helpers/web_scrap.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam/core/util/iris/chart.py` & `maryam-2.5.2.post1/maryam/core/util/iris/chart.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam/core/util/iris/cluster.py` & `maryam-2.5.2.post1/maryam/core/util/iris/cluster.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam/core/util/iris/meta_search_util.py` & `maryam-2.5.2.post1/maryam/core/util/iris/meta_search_util.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam/core/util/iris/retriever.py` & `maryam-2.5.2.post1/maryam/core/util/iris/retriever.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam/core/util/iris/safe_searcher.py` & `maryam-2.5.2.post1/maryam/core/util/iris/safe_searcher.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam/core/util/iris/tf_histogram.py` & `maryam-2.5.2.post1/maryam/core/util/iris/tf_histogram.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam/core/util/iris/topic.py` & `maryam-2.5.2.post1/maryam/core/util/iris/topic.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam/core/util/iris/word_cloud.py` & `maryam-2.5.2.post1/maryam/core/util/iris/word_cloud.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam/core/util/osint/ahmia.py` & `maryam-2.5.2.post1/maryam/core/util/osint/ahmia.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam/core/util/osint/bing_mobile_view.py` & `maryam-2.5.2.post1/maryam/core/util/osint/bing_mobile_view.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam/core/util/osint/darksearch.py` & `maryam-2.5.2.post1/maryam/core/util/osint/darksearch.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam/core/util/osint/exalead.py` & `maryam-2.5.2.post1/maryam/core/util/osint/exalead.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam/core/util/osint/hunter.py` & `maryam-2.5.2.post1/maryam/core/util/osint/hunter.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam/core/util/osint/keyserver.py` & `maryam-2.5.2.post1/maryam/core/util/osint/keyserver.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam/core/util/osint/netcraft.py` & `maryam-2.5.2.post1/maryam/core/util/osint/netcraft.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam/core/util/osint/numverify.py` & `maryam-2.5.2.post1/maryam/core/util/osint/numverify.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam/core/util/osint/onionland.py` & `maryam-2.5.2.post1/maryam/core/util/osint/onionland.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam/core/util/osint/reddit.py` & `maryam-2.5.2.post1/maryam/core/util/osint/reddit.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam/core/util/osint/tweet_search.py` & `maryam-2.5.2.post1/maryam/core/util/osint/tweet_search.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam/core/util/osint/urlscan.py` & `maryam-2.5.2.post1/maryam/core/util/osint/urlscan.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam/core/util/osint/virustotal.py` & `maryam-2.5.2.post1/maryam/core/util/osint/virustotal.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam/core/util/search/arxiv.py` & `maryam-2.5.2.post1/maryam/core/util/search/arxiv.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam/core/util/search/ask.py` & `maryam-2.5.2.post1/maryam/core/util/search/ask.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam/core/util/search/core_ac.py` & `maryam-2.5.2.post1/maryam/core/util/search/core_ac.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam/core/util/search/crt.py` & `maryam-2.5.2.post1/maryam/core/util/search/crt.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam/core/util/search/dictionary.py` & `maryam-2.5.2.post1/maryam/core/util/search/dictionary.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam/core/util/search/discord.py` & `maryam-2.5.2.post1/maryam/core/util/search/discord.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam/core/util/search/instagram.py` & `maryam-2.5.2.post1/maryam/core/util/search/instagram.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam/core/util/search/openstreetmap.py` & `maryam-2.5.2.post1/maryam/core/util/search/openstreetmap.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam/core/util/search/pastebin.py` & `maryam-2.5.2.post1/maryam/core/util/search/pastebin.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam/core/util/search/photon.py` & `maryam-2.5.2.post1/maryam/core/util/search/photon.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam/core/util/search/piratebay.py` & `maryam-2.5.2.post1/maryam/core/util/search/piratebay.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam/core/util/search/pubmed.py` & `maryam-2.5.2.post1/maryam/core/util/search/pubmed.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam/core/util/search/reddit_pushshift.py` & `maryam-2.5.2.post1/maryam/core/util/search/reddit_pushshift.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam/core/util/search/sanctionsearch.py` & `maryam-2.5.2.post1/maryam/core/util/search/sanctionsearch.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam/core/util/search/scholar.py` & `maryam-2.5.2.post1/maryam/core/util/search/scholar.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam/core/util/search/sepiasearch.py` & `maryam-2.5.2.post1/maryam/core/util/search/sepiasearch.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam/core/util/search/wikileaks.py` & `maryam-2.5.2.post1/maryam/core/util/search/wikileaks.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam/core/util/search/wikipedia.py` & `maryam-2.5.2.post1/maryam/core/util/search/wikipedia.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam/core/util/search/zlibrary.py` & `maryam-2.5.2.post1/maryam/core/util/search/zlibrary.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam/core/web/api.py` & `maryam-2.5.2.post1/maryam/core/web/api.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam/data/dnsnames.txt` & `maryam-2.5.2.post1/maryam/data/dnsnames.txt`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam/data/stopwords.csv` & `maryam-2.5.2.post1/maryam/data/stopwords.csv`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam/data/tlds.txt` & `maryam-2.5.2.post1/maryam/data/tlds.txt`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam/data/username_checker.json` & `maryam-2.5.2.post1/maryam/data/username_checker.json`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam/data/wapps.json` & `maryam-2.5.2.post1/maryam/data/wapps.json`

 * *Files identical despite different names*

### Comparing `maryam-2.5.2/maryam.egg-info/PKG-INFO` & `maryam-2.5.2.post1/maryam.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maryam
-Version: 2.5.2
+Version: 2.5.2.post1
 Summary: OWASP Maryam is a modular/optional open-source framework based on OSINT and data gathering.
 Home-page: https://github.com/saeeddhqan/Maryam
 Author: Saeed Dehqan
 Author-email: saeed.dehghan@owasp.org
 License: GPL-V3
 Keywords: OWASP,OSINT,search-engine,social-networks,Maryam
 Classifier: Programming Language :: Python :: 3.10
@@ -13,15 +13,15 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Environment :: Console
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Build Status](https://app.travis-ci.com/saeeddhqan/Maryam.svg?branch=master)](https://app.travis-ci.com/github/saeeddhqan/Maryam)
-![Version 2.5.2](https://img.shields.io/badge/Version-2.5.1-green.svg)
+![Version 2.5.2](https://img.shields.io/badge/Version-2.5.2-green.svg)
 ![GPLv3 License](https://img.shields.io/badge/License-GPLv3-green.svg)
 ![Python 3.10.x](https://img.shields.io/badge/Python-3.10.x-green.svg)
 [![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/4577/badge)](https://bestpractices.coreinfrastructure.org/projects/4577)
 
 # OWASP Maryam
 
 OWASP Maryam is a modular open-source framework based on OSINT and data gathering. It is designed to provide a robust environment to harvest data from open sources and search engines quickly and thoroughly.
```

### Comparing `maryam-2.5.2/setup.py` & `maryam-2.5.2.post1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,48 +16,48 @@
 along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 from setuptools import setup, find_packages
 
 setup(
 	name='maryam',
-	version='2.5.2',
+	version='2.5.2-1',
 	url='https://github.com/saeeddhqan/Maryam',
 	author='Saeed Dehqan',
 	author_email='saeed.dehghan@owasp.org',
 	packages=find_packages(),
 	include_package_data=True,
-	package_data={"maryam": ['data/*']},
+	package_data={"maryam": ['data/*', 'modules/osint/*', 'modules/search/*', 'modules/iris/*', 'modules/footprint/*']},
 	license='GPL-V3',
 	description='OWASP Maryam is a modular/optional open-source framework based on OSINT and data gathering.',
 	long_description=open('README.md').read(),
 	long_description_content_type='text/markdown',
 	keywords=['OWASP', 'OSINT', 'search-engine', 'social-networks', 'Maryam'],
 	scripts=['bin/maryam'],
 	install_requires=[
-        'requests',
-        'cloudscraper',
-        'bs4',
-        'lxml',
-        'flask',
-        'vaderSentiment',
-        'plotly',
-        'matplotlib',
-        'pandas',
-        'wordcloud',
-        'numpy',
-        'dask',
-        'scikit-learn',
-        'scipy',
-        'umap',
-        'bertopic',
-        'sentence_transformers',
-        'gensim',
-        'top2vec'
-    ],
+		'requests',
+		'cloudscraper',
+		'bs4',
+		'lxml',
+		'flask',
+		'vaderSentiment',
+		'plotly',
+		'matplotlib',
+		'pandas',
+		'wordcloud',
+		'numpy',
+		'dask',
+		'scikit-learn',
+		'scipy',
+		'umap',
+		'bertopic',
+		'sentence_transformers',
+		'gensim',
+		'top2vec'
+	],
 	classifiers=[
 		'Programming Language :: Python :: 3.10',
 		'Development Status :: 5 - Production/Stable',
 		'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
 		'Natural Language :: English',
 		'Operating System :: POSIX :: Linux',
 		'Environment :: Console',
```

