# Comparing `tmp/funda-scraper-1.0.5.tar.gz` & `tmp/funda-scraper-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funda-scraper-1.0.5.tar", last modified: Sun Aug  6 12:49:27 2023, max compression
+gzip compressed data, was "funda-scraper-1.0.6.tar", last modified: Sun Aug  6 13:21:13 2023, max compression
```

## Comparing `funda-scraper-1.0.5.tar` & `funda-scraper-1.0.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 willchien   (501) staff       (20)        0 2023-08-06 12:49:27.546584 funda-scraper-1.0.5/
--rw-r--r--   0 willchien   (501) staff       (20)      358 2022-09-17 10:26:03.000000 funda-scraper-1.0.5/MANIFEST.in
--rw-r--r--   0 willchien   (501) staff       (20)     3825 2023-08-06 12:49:27.546424 funda-scraper-1.0.5/PKG-INFO
--rw-r--r--   0 willchien   (501) staff       (20)     3007 2023-08-05 15:18:43.000000 funda-scraper-1.0.5/README.md
-drwxr-xr-x   0 willchien   (501) staff       (20)        0 2023-08-06 12:49:27.543837 funda-scraper-1.0.5/funda_scraper/
--rw-r--r--   0 willchien   (501) staff       (20)        5 2023-08-06 12:49:03.000000 funda-scraper-1.0.5/funda_scraper/VERSION
--rw-r--r--   0 willchien   (501) staff       (20)       83 2023-06-05 14:47:30.000000 funda-scraper-1.0.5/funda_scraper/__init__.py
-drwxr-xr-x   0 willchien   (501) staff       (20)        0 2023-08-06 12:49:27.545001 funda-scraper-1.0.5/funda_scraper/config/
--rw-r--r--   0 willchien   (501) staff       (20)        0 2022-09-13 14:21:55.000000 funda-scraper-1.0.5/funda_scraper/config/__init__.py
--rw-r--r--   0 willchien   (501) staff       (20)     2198 2023-08-05 14:17:10.000000 funda-scraper-1.0.5/funda_scraper/config/config.yaml
--rw-r--r--   0 willchien   (501) staff       (20)      363 2023-08-05 14:17:10.000000 funda-scraper-1.0.5/funda_scraper/config/core.py
--rw-r--r--   0 willchien   (501) staff       (20)     7165 2023-08-06 12:46:07.000000 funda-scraper-1.0.5/funda_scraper/preprocess.py
--rw-r--r--   0 willchien   (501) staff       (20)     9994 2023-08-06 12:48:16.000000 funda-scraper-1.0.5/funda_scraper/scrape.py
--rw-r--r--   0 willchien   (501) staff       (20)      970 2022-09-17 07:54:57.000000 funda-scraper-1.0.5/funda_scraper/utils.py
-drwxr-xr-x   0 willchien   (501) staff       (20)        0 2023-08-06 12:49:27.544547 funda-scraper-1.0.5/funda_scraper.egg-info/
--rw-r--r--   0 willchien   (501) staff       (20)     3825 2023-08-06 12:49:27.000000 funda-scraper-1.0.5/funda_scraper.egg-info/PKG-INFO
--rw-r--r--   0 willchien   (501) staff       (20)      547 2023-08-06 12:49:27.000000 funda-scraper-1.0.5/funda_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 willchien   (501) staff       (20)        1 2023-08-06 12:49:27.000000 funda-scraper-1.0.5/funda_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 willchien   (501) staff       (20)      103 2023-08-06 12:49:27.000000 funda-scraper-1.0.5/funda_scraper.egg-info/requires.txt
--rw-r--r--   0 willchien   (501) staff       (20)       14 2023-08-06 12:49:27.000000 funda-scraper-1.0.5/funda_scraper.egg-info/top_level.txt
--rw-r--r--   0 willchien   (501) staff       (20)      120 2022-09-13 18:41:58.000000 funda-scraper-1.0.5/pyproject.toml
-drwxr-xr-x   0 willchien   (501) staff       (20)        0 2023-08-06 12:49:27.542697 funda-scraper-1.0.5/requirements/
--rw-r--r--   0 willchien   (501) staff       (20)      102 2023-06-05 15:09:36.000000 funda-scraper-1.0.5/requirements/requirements.txt
--rw-r--r--   0 willchien   (501) staff       (20)       38 2023-08-06 12:49:27.546626 funda-scraper-1.0.5/setup.cfg
--rw-r--r--   0 willchien   (501) staff       (20)     1753 2023-08-05 14:51:56.000000 funda-scraper-1.0.5/setup.py
-drwxr-xr-x   0 willchien   (501) staff       (20)        0 2023-08-06 12:49:27.545191 funda-scraper-1.0.5/static/
--rw-r--r--   0 willchien   (501) staff       (20)    84501 2022-09-17 09:27:50.000000 funda-scraper-1.0.5/static/example_df.png
-drwxr-xr-x   0 willchien   (501) staff       (20)        0 2023-08-06 12:49:27.546054 funda-scraper-1.0.5/tests/
--rw-r--r--   0 willchien   (501) staff       (20)     1760 2023-08-05 14:17:10.000000 funda-scraper-1.0.5/tests/test_preprocess.py
--rw-r--r--   0 willchien   (501) staff       (20)     1382 2023-08-05 14:51:56.000000 funda-scraper-1.0.5/tests/test_scrape.py
+drwxr-xr-x   0 willchien   (501) staff       (20)        0 2023-08-06 13:21:13.660082 funda-scraper-1.0.6/
+-rw-r--r--   0 willchien   (501) staff       (20)      358 2022-09-17 10:26:03.000000 funda-scraper-1.0.6/MANIFEST.in
+-rw-r--r--   0 willchien   (501) staff       (20)     3825 2023-08-06 13:21:13.659957 funda-scraper-1.0.6/PKG-INFO
+-rw-r--r--   0 willchien   (501) staff       (20)     3007 2023-08-05 15:18:43.000000 funda-scraper-1.0.6/README.md
+drwxr-xr-x   0 willchien   (501) staff       (20)        0 2023-08-06 13:21:13.657471 funda-scraper-1.0.6/funda_scraper/
+-rw-r--r--   0 willchien   (501) staff       (20)        5 2023-08-06 13:20:46.000000 funda-scraper-1.0.6/funda_scraper/VERSION
+-rw-r--r--   0 willchien   (501) staff       (20)       83 2023-06-05 14:47:30.000000 funda-scraper-1.0.6/funda_scraper/__init__.py
+drwxr-xr-x   0 willchien   (501) staff       (20)        0 2023-08-06 13:21:13.658707 funda-scraper-1.0.6/funda_scraper/config/
+-rw-r--r--   0 willchien   (501) staff       (20)        0 2022-09-13 14:21:55.000000 funda-scraper-1.0.6/funda_scraper/config/__init__.py
+-rw-r--r--   0 willchien   (501) staff       (20)     2198 2023-08-05 14:17:10.000000 funda-scraper-1.0.6/funda_scraper/config/config.yaml
+-rw-r--r--   0 willchien   (501) staff       (20)      363 2023-08-05 14:17:10.000000 funda-scraper-1.0.6/funda_scraper/config/core.py
+-rw-r--r--   0 willchien   (501) staff       (20)     7165 2023-08-06 12:46:07.000000 funda-scraper-1.0.6/funda_scraper/preprocess.py
+-rw-r--r--   0 willchien   (501) staff       (20)    10200 2023-08-06 13:20:38.000000 funda-scraper-1.0.6/funda_scraper/scrape.py
+-rw-r--r--   0 willchien   (501) staff       (20)      970 2022-09-17 07:54:57.000000 funda-scraper-1.0.6/funda_scraper/utils.py
+drwxr-xr-x   0 willchien   (501) staff       (20)        0 2023-08-06 13:21:13.658233 funda-scraper-1.0.6/funda_scraper.egg-info/
+-rw-r--r--   0 willchien   (501) staff       (20)     3825 2023-08-06 13:21:13.000000 funda-scraper-1.0.6/funda_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 willchien   (501) staff       (20)      547 2023-08-06 13:21:13.000000 funda-scraper-1.0.6/funda_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 willchien   (501) staff       (20)        1 2023-08-06 13:21:13.000000 funda-scraper-1.0.6/funda_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 willchien   (501) staff       (20)      103 2023-08-06 13:21:13.000000 funda-scraper-1.0.6/funda_scraper.egg-info/requires.txt
+-rw-r--r--   0 willchien   (501) staff       (20)       14 2023-08-06 13:21:13.000000 funda-scraper-1.0.6/funda_scraper.egg-info/top_level.txt
+-rw-r--r--   0 willchien   (501) staff       (20)      120 2022-09-13 18:41:58.000000 funda-scraper-1.0.6/pyproject.toml
+drwxr-xr-x   0 willchien   (501) staff       (20)        0 2023-08-06 13:21:13.656416 funda-scraper-1.0.6/requirements/
+-rw-r--r--   0 willchien   (501) staff       (20)      102 2023-06-05 15:09:36.000000 funda-scraper-1.0.6/requirements/requirements.txt
+-rw-r--r--   0 willchien   (501) staff       (20)       38 2023-08-06 13:21:13.660121 funda-scraper-1.0.6/setup.cfg
+-rw-r--r--   0 willchien   (501) staff       (20)     1753 2023-08-05 14:51:56.000000 funda-scraper-1.0.6/setup.py
+drwxr-xr-x   0 willchien   (501) staff       (20)        0 2023-08-06 13:21:13.658916 funda-scraper-1.0.6/static/
+-rw-r--r--   0 willchien   (501) staff       (20)    84501 2022-09-17 09:27:50.000000 funda-scraper-1.0.6/static/example_df.png
+drwxr-xr-x   0 willchien   (501) staff       (20)        0 2023-08-06 13:21:13.659673 funda-scraper-1.0.6/tests/
+-rw-r--r--   0 willchien   (501) staff       (20)     1760 2023-08-05 14:17:10.000000 funda-scraper-1.0.6/tests/test_preprocess.py
+-rw-r--r--   0 willchien   (501) staff       (20)     1382 2023-08-05 14:51:56.000000 funda-scraper-1.0.6/tests/test_scrape.py
```

### Comparing `funda-scraper-1.0.5/PKG-INFO` & `funda-scraper-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funda-scraper
-Version: 1.0.5
+Version: 1.0.6
 Summary: FundaScaper provides you the easiest way to perform web scraping from Funda, the Dutch housing website.
 Home-page: https://github.com/whchien/funda-scraper
 Author: Will Chien
 Author-email: locriginal@gmail.com
 License: gpl-3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
```

### Comparing `funda-scraper-1.0.5/README.md` & `funda-scraper-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `funda-scraper-1.0.5/funda_scraper/config/config.yaml` & `funda-scraper-1.0.6/funda_scraper/config/config.yaml`

 * *Files identical despite different names*

### Comparing `funda-scraper-1.0.5/funda_scraper/preprocess.py` & `funda-scraper-1.0.6/funda_scraper/preprocess.py`

 * *Files identical despite different names*

### Comparing `funda-scraper-1.0.5/funda_scraper/scrape.py` & `funda-scraper-1.0.6/funda_scraper/scrape.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     def __init__(
         self,
         area: str = None,
         want_to: str = "buy",
         n_pages: int = 1,
         find_past: bool = False,
     ):
+        self.main_url = None
         self.area = area.lower().replace(" ", "-") if isinstance(area, str) else area
         self.want_to = want_to
         self.find_past = find_past
         self.n_pages = min(max(n_pages, 1), 999)
         self.links: List[str] = []
         self.raw_df = pd.DataFrame()
         self.clean_df = pd.DataFrame()
@@ -107,15 +108,20 @@
     def fetch_all_links(self) -> None:
         """Find all the available links across multiple pages."""
         if self.area is None or self.want_to is None:
             raise ValueError("You haven't set the area and what you're looking for.")
 
         logger.info("*** Phase 1: Fetch all the available links from all pages *** ")
         urls = []
-        main_url = self.site_url["close"] if self.find_past else self.site_url["open"]
+        query = "koop" if self.to_buy else "huur"
+        main_url = f"{self.base_url}/zoeken/{query}?selected_area=%22{self.area}%22"
+        if self.find_past:
+            main_url = f"{main_url}&availability=%22unavailable%22"
+        self.main_url = main_url
+
         for i in tqdm(range(0, self.n_pages + 1)):
             item_list = self._get_links_from_one_parent(f"{main_url}&search_result={i}")
             if len(item_list) == 0:
                 self.n_pages = i
                 break
             urls += item_list
         urls = list(set(urls))
@@ -257,12 +263,12 @@
             self.save_csv(df, filepath)
 
         logger.info("*** Done! ***")
         return df
 
 
 if __name__ == "__main__":
-    scraper = FundaScraper(area="amsterdam", want_to="buy", find_past=True, n_pages=1)
-    # scraper.fetch_all_links()
-    # print(scraper.links)
-    df = scraper.run(raw_data=False)
-    print(df.head())
+    scraper = FundaScraper(area="utrecht", want_to="rent", find_past=False, n_pages=1)
+    scraper.fetch_all_links()
+    print(scraper.links)
+    # df = scraper.run(raw_data=False)
+    # print(df.head())
```

### Comparing `funda-scraper-1.0.5/funda_scraper/utils.py` & `funda-scraper-1.0.6/funda_scraper/utils.py`

 * *Files identical despite different names*

### Comparing `funda-scraper-1.0.5/funda_scraper.egg-info/PKG-INFO` & `funda-scraper-1.0.6/funda_scraper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funda-scraper
-Version: 1.0.5
+Version: 1.0.6
 Summary: FundaScaper provides you the easiest way to perform web scraping from Funda, the Dutch housing website.
 Home-page: https://github.com/whchien/funda-scraper
 Author: Will Chien
 Author-email: locriginal@gmail.com
 License: gpl-3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
```

### Comparing `funda-scraper-1.0.5/funda_scraper.egg-info/SOURCES.txt` & `funda-scraper-1.0.6/funda_scraper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `funda-scraper-1.0.5/setup.py` & `funda-scraper-1.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `funda-scraper-1.0.5/static/example_df.png` & `funda-scraper-1.0.6/static/example_df.png`

 * *Files identical despite different names*

### Comparing `funda-scraper-1.0.5/tests/test_preprocess.py` & `funda-scraper-1.0.6/tests/test_preprocess.py`

 * *Files identical despite different names*

### Comparing `funda-scraper-1.0.5/tests/test_scrape.py` & `funda-scraper-1.0.6/tests/test_scrape.py`

 * *Files identical despite different names*

