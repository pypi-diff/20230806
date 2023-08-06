# Comparing `tmp/funda-scraper-1.0.4.tar.gz` & `tmp/funda-scraper-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funda-scraper-1.0.4.tar", last modified: Sun Aug  6 12:39:08 2023, max compression
+gzip compressed data, was "funda-scraper-1.0.5.tar", last modified: Sun Aug  6 12:49:27 2023, max compression
```

## Comparing `funda-scraper-1.0.4.tar` & `funda-scraper-1.0.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 willchien   (501) staff       (20)        0 2023-08-06 12:39:08.675545 funda-scraper-1.0.4/
--rw-r--r--   0 willchien   (501) staff       (20)      358 2022-09-17 10:26:03.000000 funda-scraper-1.0.4/MANIFEST.in
--rw-r--r--   0 willchien   (501) staff       (20)     3825 2023-08-06 12:39:08.675412 funda-scraper-1.0.4/PKG-INFO
--rw-r--r--   0 willchien   (501) staff       (20)     3007 2023-08-05 15:18:43.000000 funda-scraper-1.0.4/README.md
-drwxr-xr-x   0 willchien   (501) staff       (20)        0 2023-08-06 12:39:08.672566 funda-scraper-1.0.4/funda_scraper/
--rw-r--r--   0 willchien   (501) staff       (20)        5 2023-08-06 12:38:31.000000 funda-scraper-1.0.4/funda_scraper/VERSION
--rw-r--r--   0 willchien   (501) staff       (20)       83 2023-06-05 14:47:30.000000 funda-scraper-1.0.4/funda_scraper/__init__.py
-drwxr-xr-x   0 willchien   (501) staff       (20)        0 2023-08-06 12:39:08.673703 funda-scraper-1.0.4/funda_scraper/config/
--rw-r--r--   0 willchien   (501) staff       (20)        0 2022-09-13 14:21:55.000000 funda-scraper-1.0.4/funda_scraper/config/__init__.py
--rw-r--r--   0 willchien   (501) staff       (20)     2198 2023-08-05 14:17:10.000000 funda-scraper-1.0.4/funda_scraper/config/config.yaml
--rw-r--r--   0 willchien   (501) staff       (20)      363 2023-08-05 14:17:10.000000 funda-scraper-1.0.4/funda_scraper/config/core.py
--rw-r--r--   0 willchien   (501) staff       (20)     7165 2023-08-06 10:40:10.000000 funda-scraper-1.0.4/funda_scraper/preprocess.py
--rw-r--r--   0 willchien   (501) staff       (20)     9691 2023-08-06 12:38:43.000000 funda-scraper-1.0.4/funda_scraper/scrape.py
--rw-r--r--   0 willchien   (501) staff       (20)      970 2022-09-17 07:54:57.000000 funda-scraper-1.0.4/funda_scraper/utils.py
-drwxr-xr-x   0 willchien   (501) staff       (20)        0 2023-08-06 12:39:08.673259 funda-scraper-1.0.4/funda_scraper.egg-info/
--rw-r--r--   0 willchien   (501) staff       (20)     3825 2023-08-06 12:39:08.000000 funda-scraper-1.0.4/funda_scraper.egg-info/PKG-INFO
--rw-r--r--   0 willchien   (501) staff       (20)      547 2023-08-06 12:39:08.000000 funda-scraper-1.0.4/funda_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 willchien   (501) staff       (20)        1 2023-08-06 12:39:08.000000 funda-scraper-1.0.4/funda_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 willchien   (501) staff       (20)      103 2023-08-06 12:39:08.000000 funda-scraper-1.0.4/funda_scraper.egg-info/requires.txt
--rw-r--r--   0 willchien   (501) staff       (20)       14 2023-08-06 12:39:08.000000 funda-scraper-1.0.4/funda_scraper.egg-info/top_level.txt
--rw-r--r--   0 willchien   (501) staff       (20)      120 2022-09-13 18:41:58.000000 funda-scraper-1.0.4/pyproject.toml
-drwxr-xr-x   0 willchien   (501) staff       (20)        0 2023-08-06 12:39:08.671588 funda-scraper-1.0.4/requirements/
--rw-r--r--   0 willchien   (501) staff       (20)      102 2023-06-05 15:09:36.000000 funda-scraper-1.0.4/requirements/requirements.txt
--rw-r--r--   0 willchien   (501) staff       (20)       38 2023-08-06 12:39:08.675582 funda-scraper-1.0.4/setup.cfg
--rw-r--r--   0 willchien   (501) staff       (20)     1753 2023-08-05 14:51:56.000000 funda-scraper-1.0.4/setup.py
-drwxr-xr-x   0 willchien   (501) staff       (20)        0 2023-08-06 12:39:08.673888 funda-scraper-1.0.4/static/
--rw-r--r--   0 willchien   (501) staff       (20)    84501 2022-09-17 09:27:50.000000 funda-scraper-1.0.4/static/example_df.png
-drwxr-xr-x   0 willchien   (501) staff       (20)        0 2023-08-06 12:39:08.675137 funda-scraper-1.0.4/tests/
--rw-r--r--   0 willchien   (501) staff       (20)     1760 2023-08-05 14:17:10.000000 funda-scraper-1.0.4/tests/test_preprocess.py
--rw-r--r--   0 willchien   (501) staff       (20)     1382 2023-08-05 14:51:56.000000 funda-scraper-1.0.4/tests/test_scrape.py
+drwxr-xr-x   0 willchien   (501) staff       (20)        0 2023-08-06 12:49:27.546584 funda-scraper-1.0.5/
+-rw-r--r--   0 willchien   (501) staff       (20)      358 2022-09-17 10:26:03.000000 funda-scraper-1.0.5/MANIFEST.in
+-rw-r--r--   0 willchien   (501) staff       (20)     3825 2023-08-06 12:49:27.546424 funda-scraper-1.0.5/PKG-INFO
+-rw-r--r--   0 willchien   (501) staff       (20)     3007 2023-08-05 15:18:43.000000 funda-scraper-1.0.5/README.md
+drwxr-xr-x   0 willchien   (501) staff       (20)        0 2023-08-06 12:49:27.543837 funda-scraper-1.0.5/funda_scraper/
+-rw-r--r--   0 willchien   (501) staff       (20)        5 2023-08-06 12:49:03.000000 funda-scraper-1.0.5/funda_scraper/VERSION
+-rw-r--r--   0 willchien   (501) staff       (20)       83 2023-06-05 14:47:30.000000 funda-scraper-1.0.5/funda_scraper/__init__.py
+drwxr-xr-x   0 willchien   (501) staff       (20)        0 2023-08-06 12:49:27.545001 funda-scraper-1.0.5/funda_scraper/config/
+-rw-r--r--   0 willchien   (501) staff       (20)        0 2022-09-13 14:21:55.000000 funda-scraper-1.0.5/funda_scraper/config/__init__.py
+-rw-r--r--   0 willchien   (501) staff       (20)     2198 2023-08-05 14:17:10.000000 funda-scraper-1.0.5/funda_scraper/config/config.yaml
+-rw-r--r--   0 willchien   (501) staff       (20)      363 2023-08-05 14:17:10.000000 funda-scraper-1.0.5/funda_scraper/config/core.py
+-rw-r--r--   0 willchien   (501) staff       (20)     7165 2023-08-06 12:46:07.000000 funda-scraper-1.0.5/funda_scraper/preprocess.py
+-rw-r--r--   0 willchien   (501) staff       (20)     9994 2023-08-06 12:48:16.000000 funda-scraper-1.0.5/funda_scraper/scrape.py
+-rw-r--r--   0 willchien   (501) staff       (20)      970 2022-09-17 07:54:57.000000 funda-scraper-1.0.5/funda_scraper/utils.py
+drwxr-xr-x   0 willchien   (501) staff       (20)        0 2023-08-06 12:49:27.544547 funda-scraper-1.0.5/funda_scraper.egg-info/
+-rw-r--r--   0 willchien   (501) staff       (20)     3825 2023-08-06 12:49:27.000000 funda-scraper-1.0.5/funda_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 willchien   (501) staff       (20)      547 2023-08-06 12:49:27.000000 funda-scraper-1.0.5/funda_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 willchien   (501) staff       (20)        1 2023-08-06 12:49:27.000000 funda-scraper-1.0.5/funda_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 willchien   (501) staff       (20)      103 2023-08-06 12:49:27.000000 funda-scraper-1.0.5/funda_scraper.egg-info/requires.txt
+-rw-r--r--   0 willchien   (501) staff       (20)       14 2023-08-06 12:49:27.000000 funda-scraper-1.0.5/funda_scraper.egg-info/top_level.txt
+-rw-r--r--   0 willchien   (501) staff       (20)      120 2022-09-13 18:41:58.000000 funda-scraper-1.0.5/pyproject.toml
+drwxr-xr-x   0 willchien   (501) staff       (20)        0 2023-08-06 12:49:27.542697 funda-scraper-1.0.5/requirements/
+-rw-r--r--   0 willchien   (501) staff       (20)      102 2023-06-05 15:09:36.000000 funda-scraper-1.0.5/requirements/requirements.txt
+-rw-r--r--   0 willchien   (501) staff       (20)       38 2023-08-06 12:49:27.546626 funda-scraper-1.0.5/setup.cfg
+-rw-r--r--   0 willchien   (501) staff       (20)     1753 2023-08-05 14:51:56.000000 funda-scraper-1.0.5/setup.py
+drwxr-xr-x   0 willchien   (501) staff       (20)        0 2023-08-06 12:49:27.545191 funda-scraper-1.0.5/static/
+-rw-r--r--   0 willchien   (501) staff       (20)    84501 2022-09-17 09:27:50.000000 funda-scraper-1.0.5/static/example_df.png
+drwxr-xr-x   0 willchien   (501) staff       (20)        0 2023-08-06 12:49:27.546054 funda-scraper-1.0.5/tests/
+-rw-r--r--   0 willchien   (501) staff       (20)     1760 2023-08-05 14:17:10.000000 funda-scraper-1.0.5/tests/test_preprocess.py
+-rw-r--r--   0 willchien   (501) staff       (20)     1382 2023-08-05 14:51:56.000000 funda-scraper-1.0.5/tests/test_scrape.py
```

### Comparing `funda-scraper-1.0.4/PKG-INFO` & `funda-scraper-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funda-scraper
-Version: 1.0.4
+Version: 1.0.5
 Summary: FundaScaper provides you the easiest way to perform web scraping from Funda, the Dutch housing website.
 Home-page: https://github.com/whchien/funda-scraper
 Author: Will Chien
 Author-email: locriginal@gmail.com
 License: gpl-3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
```

### Comparing `funda-scraper-1.0.4/README.md` & `funda-scraper-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `funda-scraper-1.0.4/funda_scraper/config/config.yaml` & `funda-scraper-1.0.5/funda_scraper/config/config.yaml`

 * *Files identical despite different names*

### Comparing `funda-scraper-1.0.4/funda_scraper/preprocess.py` & `funda-scraper-1.0.5/funda_scraper/preprocess.py`

 * *Files identical despite different names*

### Comparing `funda-scraper-1.0.4/funda_scraper/scrape.py` & `funda-scraper-1.0.5/funda_scraper/scrape.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,21 +47,21 @@
         )
 
     @property
     def site_url(self) -> Dict[str, str]:
         """Return the corresponding urls."""
         if self.to_buy:
             return {
-                "close": f'{self.base_url}/zoeken/koop?selected_area="{self.area}"&availability="unavailable"',
-                "open": f'{self.base_url}/zoeken/koop?selected_area="{self.area}"/',
+                "close": f"{self.base_url}/zoeken/koop?selected_area=\"{self.area}\"&availability=\"unavailable\"",
+                "open": f"{self.base_url}/zoeken/koop?selected_area=\"{self.area}\"/",
             }
         else:
             return {
-                "close": f'{self.base_url}/zoeken/huur?selected_area="{self.area}"&availability="unavailable"',
-                "open": f'{self.base_url}/zoeken/huur?selected_area="{self.area}"/',
+                "close": f"{self.base_url}/zoeken/huur?selected_area=\"{self.area}\"&availability=\"unavailable\"",
+                "open": f"{self.base_url}/zoeken/huur?selected_area=\"{self.area}\"/",
             }
 
     @property
     def to_buy(self) -> bool:
         """Whether to buy or not"""
         if self.want_to.lower() in ["buy", "koop", "b"]:
             return True
@@ -115,15 +115,17 @@
         for i in tqdm(range(0, self.n_pages + 1)):
             item_list = self._get_links_from_one_parent(f"{main_url}&search_result={i}")
             if len(item_list) == 0:
                 self.n_pages = i
                 break
             urls += item_list
         urls = list(set(urls))
-        logger.info(f"*** Got all the urls. {len(urls)} houses found in {self.n_pages} pages. ***")
+        logger.info(
+            f"*** Got all the urls. {len(urls)} houses found in {self.n_pages} pages. ***"
+        )
         self.links = urls
 
     @staticmethod
     def get_value_from_css(soup: BeautifulSoup, selector: str) -> str:
         """Use CSS selector to find certain features."""
         result = soup.select(selector)
         if len(result) > 0:
@@ -136,43 +138,59 @@
         """Scrape all the features from one house item given a link."""
 
         # Initialize for each page
         response = requests.get(link, headers=config.header)
         soup = BeautifulSoup(response.text, "lxml")
 
         # Get the value according to respective CSS selectors
-        list_since_selector = self.selectors.listed_since if self.to_buy else ".fd-align-items-center:nth-child(7) span"
+        list_since_selector = (
+            self.selectors.listed_since
+            if self.to_buy
+            else ".fd-align-items-center:nth-child(7) span"
+        )
         result = [
             link,
             self.get_value_from_css(soup, self.selectors.price),
             self.get_value_from_css(soup, self.selectors.address),
             self.get_value_from_css(soup, self.selectors.descrip),
             self.get_value_from_css(soup, list_since_selector).replace("\n", ""),
-            self.get_value_from_css(soup, self.selectors.zip_code).replace("\n", "").replace("\r        ", ""),
+            self.get_value_from_css(soup, self.selectors.zip_code)
+            .replace("\n", "")
+            .replace("\r        ", ""),
             self.get_value_from_css(soup, self.selectors.size),
             self.get_value_from_css(soup, self.selectors.year),
             self.get_value_from_css(soup, self.selectors.living_area),
             self.get_value_from_css(soup, self.selectors.kind_of_house),
             self.get_value_from_css(soup, self.selectors.building_type),
-            self.get_value_from_css(soup, self.selectors.num_of_rooms).replace("\n", ""),
-            self.get_value_from_css(soup, self.selectors.num_of_bathrooms).replace("\n", ""),
+            self.get_value_from_css(soup, self.selectors.num_of_rooms).replace(
+                "\n", ""
+            ),
+            self.get_value_from_css(soup, self.selectors.num_of_bathrooms).replace(
+                "\n", ""
+            ),
             self.get_value_from_css(soup, self.selectors.layout),
-            self.get_value_from_css(soup, self.selectors.energy_label).replace("\r\n        ", ""),
+            self.get_value_from_css(soup, self.selectors.energy_label).replace(
+                "\r\n        ", ""
+            ),
             self.get_value_from_css(soup, self.selectors.insulation).replace("\n", ""),
             self.get_value_from_css(soup, self.selectors.heating).replace("\n", ""),
             self.get_value_from_css(soup, self.selectors.ownership).replace("\n", ""),
             self.get_value_from_css(soup, self.selectors.exteriors),
             self.get_value_from_css(soup, self.selectors.parking),
             self.get_value_from_css(soup, self.selectors.neighborhood_name),
             self.get_value_from_css(soup, self.selectors.date_list),
             self.get_value_from_css(soup, self.selectors.date_sold),
             self.get_value_from_css(soup, self.selectors.term),
             self.get_value_from_css(soup, self.selectors.price_sold),
-            self.get_value_from_css(soup, self.selectors.last_ask_price).replace("\n", ""),
-            self.get_value_from_css(soup, self.selectors.last_ask_price_m2).split("\r")[0],
+            self.get_value_from_css(soup, self.selectors.last_ask_price).replace(
+                "\n", ""
+            ),
+            self.get_value_from_css(soup, self.selectors.last_ask_price_m2).split("\r")[
+                0
+            ],
         ]
 
         return result
 
     def scrape_pages(self) -> None:
         """Scrape all the content acoss multiple pages."""
 
@@ -204,19 +222,23 @@
                 else:
                     status = "rented"
             else:
                 if self.to_buy:
                     status = "selling"
                 else:
                     status = "renting"
-            filepath = f"./data/houseprice_{date}_{self.area}_{status}_{len(self.links)}.csv"
+            filepath = (
+                f"./data/houseprice_{date}_{self.area}_{status}_{len(self.links)}.csv"
+            )
         df.to_csv(filepath, index=False)
         logger.info(f"*** File saved: {filepath}. ***")
 
-    def run(self, raw_data: bool = False, save: bool = False, filepath: str = None) -> pd.DataFrame:
+    def run(
+        self, raw_data: bool = False, save: bool = False, filepath: str = None
+    ) -> pd.DataFrame:
         """
         Scrape all links and all content.
 
         :param raw_data: if true, the data won't be pre-processed
         :param save: if true, the data will be saved as a csv file
         :param filepath: the name for the file
         :return: the (pre-processed) dataframe from scraping
@@ -235,12 +257,12 @@
             self.save_csv(df, filepath)
 
         logger.info("*** Done! ***")
         return df
 
 
 if __name__ == "__main__":
-    scraper = FundaScraper(area="rotterdam", want_to="rent", find_past=True, n_pages=1)
-    scraper.fetch_all_links()
-    print(scraper.links)
-    # df = scraper.run(raw_data=False)
-    # print(df.head())
+    scraper = FundaScraper(area="amsterdam", want_to="buy", find_past=True, n_pages=1)
+    # scraper.fetch_all_links()
+    # print(scraper.links)
+    df = scraper.run(raw_data=False)
+    print(df.head())
```

### Comparing `funda-scraper-1.0.4/funda_scraper/utils.py` & `funda-scraper-1.0.5/funda_scraper/utils.py`

 * *Files identical despite different names*

### Comparing `funda-scraper-1.0.4/funda_scraper.egg-info/PKG-INFO` & `funda-scraper-1.0.5/funda_scraper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funda-scraper
-Version: 1.0.4
+Version: 1.0.5
 Summary: FundaScaper provides you the easiest way to perform web scraping from Funda, the Dutch housing website.
 Home-page: https://github.com/whchien/funda-scraper
 Author: Will Chien
 Author-email: locriginal@gmail.com
 License: gpl-3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
```

### Comparing `funda-scraper-1.0.4/funda_scraper.egg-info/SOURCES.txt` & `funda-scraper-1.0.5/funda_scraper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `funda-scraper-1.0.4/setup.py` & `funda-scraper-1.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `funda-scraper-1.0.4/static/example_df.png` & `funda-scraper-1.0.5/static/example_df.png`

 * *Files identical despite different names*

### Comparing `funda-scraper-1.0.4/tests/test_preprocess.py` & `funda-scraper-1.0.5/tests/test_preprocess.py`

 * *Files identical despite different names*

### Comparing `funda-scraper-1.0.4/tests/test_scrape.py` & `funda-scraper-1.0.5/tests/test_scrape.py`

 * *Files identical despite different names*

