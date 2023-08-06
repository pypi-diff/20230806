# Comparing `tmp/funda-scraper-1.0.1.tar.gz` & `tmp/funda-scraper-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funda-scraper-1.0.1.tar", last modified: Sat Aug  5 15:19:17 2023, max compression
+gzip compressed data, was "funda-scraper-1.0.2.tar", last modified: Sun Aug  6 10:29:57 2023, max compression
```

## Comparing `funda-scraper-1.0.1.tar` & `funda-scraper-1.0.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 willchien   (501) staff       (20)        0 2023-08-05 15:19:17.281267 funda-scraper-1.0.1/
--rw-r--r--   0 willchien   (501) staff       (20)      358 2022-09-17 10:26:03.000000 funda-scraper-1.0.1/MANIFEST.in
--rw-r--r--   0 willchien   (501) staff       (20)     3825 2023-08-05 15:19:17.281120 funda-scraper-1.0.1/PKG-INFO
--rw-r--r--   0 willchien   (501) staff       (20)     3007 2023-08-05 15:18:43.000000 funda-scraper-1.0.1/README.md
-drwxr-xr-x   0 willchien   (501) staff       (20)        0 2023-08-05 15:19:17.278114 funda-scraper-1.0.1/funda_scraper/
--rw-r--r--   0 willchien   (501) staff       (20)        5 2023-08-05 15:18:28.000000 funda-scraper-1.0.1/funda_scraper/VERSION
--rw-r--r--   0 willchien   (501) staff       (20)       83 2023-06-05 14:47:30.000000 funda-scraper-1.0.1/funda_scraper/__init__.py
-drwxr-xr-x   0 willchien   (501) staff       (20)        0 2023-08-05 15:19:17.279498 funda-scraper-1.0.1/funda_scraper/config/
--rw-r--r--   0 willchien   (501) staff       (20)        0 2022-09-13 14:21:55.000000 funda-scraper-1.0.1/funda_scraper/config/__init__.py
--rw-r--r--   0 willchien   (501) staff       (20)     2198 2023-08-05 14:17:10.000000 funda-scraper-1.0.1/funda_scraper/config/config.yaml
--rw-r--r--   0 willchien   (501) staff       (20)      363 2023-08-05 14:17:10.000000 funda-scraper-1.0.1/funda_scraper/config/core.py
--rw-r--r--   0 willchien   (501) staff       (20)     7165 2023-08-05 14:51:56.000000 funda-scraper-1.0.1/funda_scraper/preprocess.py
--rw-r--r--   0 willchien   (501) staff       (20)     9632 2023-08-05 15:18:43.000000 funda-scraper-1.0.1/funda_scraper/scrape.py
--rw-r--r--   0 willchien   (501) staff       (20)      970 2022-09-17 07:54:57.000000 funda-scraper-1.0.1/funda_scraper/utils.py
-drwxr-xr-x   0 willchien   (501) staff       (20)        0 2023-08-05 15:19:17.279000 funda-scraper-1.0.1/funda_scraper.egg-info/
--rw-r--r--   0 willchien   (501) staff       (20)     3825 2023-08-05 15:19:17.000000 funda-scraper-1.0.1/funda_scraper.egg-info/PKG-INFO
--rw-r--r--   0 willchien   (501) staff       (20)      547 2023-08-05 15:19:17.000000 funda-scraper-1.0.1/funda_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 willchien   (501) staff       (20)        1 2023-08-05 15:19:17.000000 funda-scraper-1.0.1/funda_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 willchien   (501) staff       (20)      103 2023-08-05 15:19:17.000000 funda-scraper-1.0.1/funda_scraper.egg-info/requires.txt
--rw-r--r--   0 willchien   (501) staff       (20)       14 2023-08-05 15:19:17.000000 funda-scraper-1.0.1/funda_scraper.egg-info/top_level.txt
--rw-r--r--   0 willchien   (501) staff       (20)      120 2022-09-13 18:41:58.000000 funda-scraper-1.0.1/pyproject.toml
-drwxr-xr-x   0 willchien   (501) staff       (20)        0 2023-08-05 15:19:17.276950 funda-scraper-1.0.1/requirements/
--rw-r--r--   0 willchien   (501) staff       (20)      102 2023-06-05 15:09:36.000000 funda-scraper-1.0.1/requirements/requirements.txt
--rw-r--r--   0 willchien   (501) staff       (20)       38 2023-08-05 15:19:17.281360 funda-scraper-1.0.1/setup.cfg
--rw-r--r--   0 willchien   (501) staff       (20)     1753 2023-08-05 14:51:56.000000 funda-scraper-1.0.1/setup.py
-drwxr-xr-x   0 willchien   (501) staff       (20)        0 2023-08-05 15:19:17.279758 funda-scraper-1.0.1/static/
--rw-r--r--   0 willchien   (501) staff       (20)    84501 2022-09-17 09:27:50.000000 funda-scraper-1.0.1/static/example_df.png
-drwxr-xr-x   0 willchien   (501) staff       (20)        0 2023-08-05 15:19:17.280828 funda-scraper-1.0.1/tests/
--rw-r--r--   0 willchien   (501) staff       (20)     1760 2023-08-05 14:17:10.000000 funda-scraper-1.0.1/tests/test_preprocess.py
--rw-r--r--   0 willchien   (501) staff       (20)     1382 2023-08-05 14:51:56.000000 funda-scraper-1.0.1/tests/test_scrape.py
+drwxr-xr-x   0 willchien   (501) staff       (20)        0 2023-08-06 10:29:57.380618 funda-scraper-1.0.2/
+-rw-r--r--   0 willchien   (501) staff       (20)      358 2022-09-17 10:26:03.000000 funda-scraper-1.0.2/MANIFEST.in
+-rw-r--r--   0 willchien   (501) staff       (20)     3825 2023-08-06 10:29:57.380457 funda-scraper-1.0.2/PKG-INFO
+-rw-r--r--   0 willchien   (501) staff       (20)     3007 2023-08-05 15:18:43.000000 funda-scraper-1.0.2/README.md
+drwxr-xr-x   0 willchien   (501) staff       (20)        0 2023-08-06 10:29:57.377708 funda-scraper-1.0.2/funda_scraper/
+-rw-r--r--   0 willchien   (501) staff       (20)        5 2023-08-06 10:29:26.000000 funda-scraper-1.0.2/funda_scraper/VERSION
+-rw-r--r--   0 willchien   (501) staff       (20)       83 2023-06-05 14:47:30.000000 funda-scraper-1.0.2/funda_scraper/__init__.py
+drwxr-xr-x   0 willchien   (501) staff       (20)        0 2023-08-06 10:29:57.379028 funda-scraper-1.0.2/funda_scraper/config/
+-rw-r--r--   0 willchien   (501) staff       (20)        0 2022-09-13 14:21:55.000000 funda-scraper-1.0.2/funda_scraper/config/__init__.py
+-rw-r--r--   0 willchien   (501) staff       (20)     2198 2023-08-05 14:17:10.000000 funda-scraper-1.0.2/funda_scraper/config/config.yaml
+-rw-r--r--   0 willchien   (501) staff       (20)      363 2023-08-05 14:17:10.000000 funda-scraper-1.0.2/funda_scraper/config/core.py
+-rw-r--r--   0 willchien   (501) staff       (20)     7165 2023-08-05 14:51:56.000000 funda-scraper-1.0.2/funda_scraper/preprocess.py
+-rw-r--r--   0 willchien   (501) staff       (20)     9644 2023-08-06 09:23:26.000000 funda-scraper-1.0.2/funda_scraper/scrape.py
+-rw-r--r--   0 willchien   (501) staff       (20)      970 2022-09-17 07:54:57.000000 funda-scraper-1.0.2/funda_scraper/utils.py
+drwxr-xr-x   0 willchien   (501) staff       (20)        0 2023-08-06 10:29:57.378546 funda-scraper-1.0.2/funda_scraper.egg-info/
+-rw-r--r--   0 willchien   (501) staff       (20)     3825 2023-08-06 10:29:57.000000 funda-scraper-1.0.2/funda_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 willchien   (501) staff       (20)      547 2023-08-06 10:29:57.000000 funda-scraper-1.0.2/funda_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 willchien   (501) staff       (20)        1 2023-08-06 10:29:57.000000 funda-scraper-1.0.2/funda_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 willchien   (501) staff       (20)      103 2023-08-06 10:29:57.000000 funda-scraper-1.0.2/funda_scraper.egg-info/requires.txt
+-rw-r--r--   0 willchien   (501) staff       (20)       14 2023-08-06 10:29:57.000000 funda-scraper-1.0.2/funda_scraper.egg-info/top_level.txt
+-rw-r--r--   0 willchien   (501) staff       (20)      120 2022-09-13 18:41:58.000000 funda-scraper-1.0.2/pyproject.toml
+drwxr-xr-x   0 willchien   (501) staff       (20)        0 2023-08-06 10:29:57.376463 funda-scraper-1.0.2/requirements/
+-rw-r--r--   0 willchien   (501) staff       (20)      102 2023-06-05 15:09:36.000000 funda-scraper-1.0.2/requirements/requirements.txt
+-rw-r--r--   0 willchien   (501) staff       (20)       38 2023-08-06 10:29:57.380667 funda-scraper-1.0.2/setup.cfg
+-rw-r--r--   0 willchien   (501) staff       (20)     1753 2023-08-05 14:51:56.000000 funda-scraper-1.0.2/setup.py
+drwxr-xr-x   0 willchien   (501) staff       (20)        0 2023-08-06 10:29:57.379238 funda-scraper-1.0.2/static/
+-rw-r--r--   0 willchien   (501) staff       (20)    84501 2022-09-17 09:27:50.000000 funda-scraper-1.0.2/static/example_df.png
+drwxr-xr-x   0 willchien   (501) staff       (20)        0 2023-08-06 10:29:57.380143 funda-scraper-1.0.2/tests/
+-rw-r--r--   0 willchien   (501) staff       (20)     1760 2023-08-05 14:17:10.000000 funda-scraper-1.0.2/tests/test_preprocess.py
+-rw-r--r--   0 willchien   (501) staff       (20)     1382 2023-08-05 14:51:56.000000 funda-scraper-1.0.2/tests/test_scrape.py
```

### Comparing `funda-scraper-1.0.1/PKG-INFO` & `funda-scraper-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funda-scraper
-Version: 1.0.1
+Version: 1.0.2
 Summary: FundaScaper provides you the easiest way to perform web scraping from Funda, the Dutch housing website.
 Home-page: https://github.com/whchien/funda-scraper
 Author: Will Chien
 Author-email: locriginal@gmail.com
 License: gpl-3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
```

### Comparing `funda-scraper-1.0.1/README.md` & `funda-scraper-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `funda-scraper-1.0.1/funda_scraper/config/config.yaml` & `funda-scraper-1.0.2/funda_scraper/config/config.yaml`

 * *Files identical despite different names*

### Comparing `funda-scraper-1.0.1/funda_scraper/preprocess.py` & `funda-scraper-1.0.2/funda_scraper/preprocess.py`

 * *Files identical despite different names*

### Comparing `funda-scraper-1.0.1/funda_scraper/scrape.py` & `funda-scraper-1.0.2/funda_scraper/scrape.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,20 +48,20 @@
 
     @property
     def site_url(self) -> Dict[str, str]:
         """Return the corresponding urls."""
         if self.to_buy:
             return {
                 "close": f'{self.base_url}/zoeken/koop/?selected_area="{self.area}"&availability="unavailable"',
-                "open": f'{self.base_url}/zoeken/koop?selected_area="{self.area}"/',
+                "open": f'{self.base_url}/zoeken/koop?selected_area=%5B"{self.area}"%5D/',
             }
         else:
             return {
                 "close": f'{self.base_url}/zoeken/huur?selected_area="{self.area}"&availability="unavailable"',
-                "open": f'{self.base_url}/zoeken/huur?selected_area="{self.area}"/',
+                "open": f'{self.base_url}/zoeken/huur?selected_area=%5B"{self.area}"%5D/',
             }
 
     @property
     def to_buy(self) -> bool:
         """Whether to buy or not"""
         if self.want_to.lower() in ["buy", "koop", "b"]:
             return True
```

### Comparing `funda-scraper-1.0.1/funda_scraper/utils.py` & `funda-scraper-1.0.2/funda_scraper/utils.py`

 * *Files identical despite different names*

### Comparing `funda-scraper-1.0.1/funda_scraper.egg-info/PKG-INFO` & `funda-scraper-1.0.2/funda_scraper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funda-scraper
-Version: 1.0.1
+Version: 1.0.2
 Summary: FundaScaper provides you the easiest way to perform web scraping from Funda, the Dutch housing website.
 Home-page: https://github.com/whchien/funda-scraper
 Author: Will Chien
 Author-email: locriginal@gmail.com
 License: gpl-3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
```

### Comparing `funda-scraper-1.0.1/funda_scraper.egg-info/SOURCES.txt` & `funda-scraper-1.0.2/funda_scraper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `funda-scraper-1.0.1/setup.py` & `funda-scraper-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `funda-scraper-1.0.1/static/example_df.png` & `funda-scraper-1.0.2/static/example_df.png`

 * *Files identical despite different names*

### Comparing `funda-scraper-1.0.1/tests/test_preprocess.py` & `funda-scraper-1.0.2/tests/test_preprocess.py`

 * *Files identical despite different names*

### Comparing `funda-scraper-1.0.1/tests/test_scrape.py` & `funda-scraper-1.0.2/tests/test_scrape.py`

 * *Files identical despite different names*

