# Comparing `tmp/funda-scraper-1.0.0.tar.gz` & `tmp/funda-scraper-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funda-scraper-1.0.0.tar", last modified: Sat Aug  5 14:23:04 2023, max compression
+gzip compressed data, was "funda-scraper-1.0.1.tar", last modified: Sat Aug  5 15:19:17 2023, max compression
```

## Comparing `funda-scraper-1.0.0.tar` & `funda-scraper-1.0.1.tar`

### file list

```diff
@@ -1,31 +1,30 @@
-drwxr-xr-x   0 willchien   (501) staff       (20)        0 2023-08-05 14:23:04.374858 funda-scraper-1.0.0/
--rw-r--r--   0 willchien   (501) staff       (20)      358 2022-09-17 10:26:03.000000 funda-scraper-1.0.0/MANIFEST.in
--rw-r--r--   0 willchien   (501) staff       (20)     3076 2023-08-05 14:23:04.374716 funda-scraper-1.0.0/PKG-INFO
--rw-r--r--   0 willchien   (501) staff       (20)     2258 2023-06-05 15:46:08.000000 funda-scraper-1.0.0/README.md
-drwxr-xr-x   0 willchien   (501) staff       (20)        0 2023-08-05 14:23:04.372319 funda-scraper-1.0.0/funda_scraper/
--rw-r--r--   0 willchien   (501) staff       (20)        5 2023-08-05 14:17:10.000000 funda-scraper-1.0.0/funda_scraper/VERSION
--rw-r--r--   0 willchien   (501) staff       (20)       83 2023-06-05 14:47:30.000000 funda-scraper-1.0.0/funda_scraper/__init__.py
-drwxr-xr-x   0 willchien   (501) staff       (20)        0 2023-08-05 14:23:04.373499 funda-scraper-1.0.0/funda_scraper/config/
--rw-r--r--   0 willchien   (501) staff       (20)        0 2022-09-13 14:21:55.000000 funda-scraper-1.0.0/funda_scraper/config/__init__.py
--rw-r--r--   0 willchien   (501) staff       (20)     2198 2023-08-05 14:17:10.000000 funda-scraper-1.0.0/funda_scraper/config/config.yaml
--rw-r--r--   0 willchien   (501) staff       (20)      363 2023-08-05 14:17:10.000000 funda-scraper-1.0.0/funda_scraper/config/core.py
--rw-r--r--   0 willchien   (501) staff       (20)     7193 2023-08-05 14:17:10.000000 funda-scraper-1.0.0/funda_scraper/preprocess.py
--rw-r--r--   0 willchien   (501) staff       (20)    10067 2023-08-05 14:17:10.000000 funda-scraper-1.0.0/funda_scraper/scrape.py
--rw-r--r--   0 willchien   (501) staff       (20)      970 2022-09-17 07:54:57.000000 funda-scraper-1.0.0/funda_scraper/utils.py
-drwxr-xr-x   0 willchien   (501) staff       (20)        0 2023-08-05 14:23:04.373050 funda-scraper-1.0.0/funda_scraper.egg-info/
--rw-r--r--   0 willchien   (501) staff       (20)     3076 2023-08-05 14:23:04.000000 funda-scraper-1.0.0/funda_scraper.egg-info/PKG-INFO
--rw-r--r--   0 willchien   (501) staff       (20)      564 2023-08-05 14:23:04.000000 funda-scraper-1.0.0/funda_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 willchien   (501) staff       (20)        1 2023-08-05 14:23:04.000000 funda-scraper-1.0.0/funda_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 willchien   (501) staff       (20)      103 2023-08-05 14:23:04.000000 funda-scraper-1.0.0/funda_scraper.egg-info/requires.txt
--rw-r--r--   0 willchien   (501) staff       (20)       14 2023-08-05 14:23:04.000000 funda-scraper-1.0.0/funda_scraper.egg-info/top_level.txt
--rw-r--r--   0 willchien   (501) staff       (20)      120 2022-09-13 18:41:58.000000 funda-scraper-1.0.0/pyproject.toml
-drwxr-xr-x   0 willchien   (501) staff       (20)        0 2023-08-05 14:23:04.371280 funda-scraper-1.0.0/requirements/
--rw-r--r--   0 willchien   (501) staff       (20)      102 2023-06-05 15:09:36.000000 funda-scraper-1.0.0/requirements/requirements.txt
--rw-r--r--   0 willchien   (501) staff       (20)      856 2023-08-05 14:18:52.000000 funda-scraper-1.0.0/requirements.txt
--rw-r--r--   0 willchien   (501) staff       (20)       38 2023-08-05 14:23:04.374903 funda-scraper-1.0.0/setup.cfg
--rw-r--r--   0 willchien   (501) staff       (20)     1753 2023-08-05 14:21:54.000000 funda-scraper-1.0.0/setup.py
-drwxr-xr-x   0 willchien   (501) staff       (20)        0 2023-08-05 14:23:04.373651 funda-scraper-1.0.0/static/
--rw-r--r--   0 willchien   (501) staff       (20)    84501 2022-09-17 09:27:50.000000 funda-scraper-1.0.0/static/example_df.png
-drwxr-xr-x   0 willchien   (501) staff       (20)        0 2023-08-05 14:23:04.374506 funda-scraper-1.0.0/tests/
--rw-r--r--   0 willchien   (501) staff       (20)     1760 2023-08-05 14:17:10.000000 funda-scraper-1.0.0/tests/test_preprocess.py
--rw-r--r--   0 willchien   (501) staff       (20)     1470 2023-08-05 14:17:10.000000 funda-scraper-1.0.0/tests/test_scrape.py
+drwxr-xr-x   0 willchien   (501) staff       (20)        0 2023-08-05 15:19:17.281267 funda-scraper-1.0.1/
+-rw-r--r--   0 willchien   (501) staff       (20)      358 2022-09-17 10:26:03.000000 funda-scraper-1.0.1/MANIFEST.in
+-rw-r--r--   0 willchien   (501) staff       (20)     3825 2023-08-05 15:19:17.281120 funda-scraper-1.0.1/PKG-INFO
+-rw-r--r--   0 willchien   (501) staff       (20)     3007 2023-08-05 15:18:43.000000 funda-scraper-1.0.1/README.md
+drwxr-xr-x   0 willchien   (501) staff       (20)        0 2023-08-05 15:19:17.278114 funda-scraper-1.0.1/funda_scraper/
+-rw-r--r--   0 willchien   (501) staff       (20)        5 2023-08-05 15:18:28.000000 funda-scraper-1.0.1/funda_scraper/VERSION
+-rw-r--r--   0 willchien   (501) staff       (20)       83 2023-06-05 14:47:30.000000 funda-scraper-1.0.1/funda_scraper/__init__.py
+drwxr-xr-x   0 willchien   (501) staff       (20)        0 2023-08-05 15:19:17.279498 funda-scraper-1.0.1/funda_scraper/config/
+-rw-r--r--   0 willchien   (501) staff       (20)        0 2022-09-13 14:21:55.000000 funda-scraper-1.0.1/funda_scraper/config/__init__.py
+-rw-r--r--   0 willchien   (501) staff       (20)     2198 2023-08-05 14:17:10.000000 funda-scraper-1.0.1/funda_scraper/config/config.yaml
+-rw-r--r--   0 willchien   (501) staff       (20)      363 2023-08-05 14:17:10.000000 funda-scraper-1.0.1/funda_scraper/config/core.py
+-rw-r--r--   0 willchien   (501) staff       (20)     7165 2023-08-05 14:51:56.000000 funda-scraper-1.0.1/funda_scraper/preprocess.py
+-rw-r--r--   0 willchien   (501) staff       (20)     9632 2023-08-05 15:18:43.000000 funda-scraper-1.0.1/funda_scraper/scrape.py
+-rw-r--r--   0 willchien   (501) staff       (20)      970 2022-09-17 07:54:57.000000 funda-scraper-1.0.1/funda_scraper/utils.py
+drwxr-xr-x   0 willchien   (501) staff       (20)        0 2023-08-05 15:19:17.279000 funda-scraper-1.0.1/funda_scraper.egg-info/
+-rw-r--r--   0 willchien   (501) staff       (20)     3825 2023-08-05 15:19:17.000000 funda-scraper-1.0.1/funda_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 willchien   (501) staff       (20)      547 2023-08-05 15:19:17.000000 funda-scraper-1.0.1/funda_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 willchien   (501) staff       (20)        1 2023-08-05 15:19:17.000000 funda-scraper-1.0.1/funda_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 willchien   (501) staff       (20)      103 2023-08-05 15:19:17.000000 funda-scraper-1.0.1/funda_scraper.egg-info/requires.txt
+-rw-r--r--   0 willchien   (501) staff       (20)       14 2023-08-05 15:19:17.000000 funda-scraper-1.0.1/funda_scraper.egg-info/top_level.txt
+-rw-r--r--   0 willchien   (501) staff       (20)      120 2022-09-13 18:41:58.000000 funda-scraper-1.0.1/pyproject.toml
+drwxr-xr-x   0 willchien   (501) staff       (20)        0 2023-08-05 15:19:17.276950 funda-scraper-1.0.1/requirements/
+-rw-r--r--   0 willchien   (501) staff       (20)      102 2023-06-05 15:09:36.000000 funda-scraper-1.0.1/requirements/requirements.txt
+-rw-r--r--   0 willchien   (501) staff       (20)       38 2023-08-05 15:19:17.281360 funda-scraper-1.0.1/setup.cfg
+-rw-r--r--   0 willchien   (501) staff       (20)     1753 2023-08-05 14:51:56.000000 funda-scraper-1.0.1/setup.py
+drwxr-xr-x   0 willchien   (501) staff       (20)        0 2023-08-05 15:19:17.279758 funda-scraper-1.0.1/static/
+-rw-r--r--   0 willchien   (501) staff       (20)    84501 2022-09-17 09:27:50.000000 funda-scraper-1.0.1/static/example_df.png
+drwxr-xr-x   0 willchien   (501) staff       (20)        0 2023-08-05 15:19:17.280828 funda-scraper-1.0.1/tests/
+-rw-r--r--   0 willchien   (501) staff       (20)     1760 2023-08-05 14:17:10.000000 funda-scraper-1.0.1/tests/test_preprocess.py
+-rw-r--r--   0 willchien   (501) staff       (20)     1382 2023-08-05 14:51:56.000000 funda-scraper-1.0.1/tests/test_scrape.py
```

### Comparing `funda-scraper-1.0.0/PKG-INFO` & `funda-scraper-1.0.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funda-scraper
-Version: 1.0.0
+Version: 1.0.1
 Summary: FundaScaper provides you the easiest way to perform web scraping from Funda, the Dutch housing website.
 Home-page: https://github.com/whchien/funda-scraper
 Author: Will Chien
 Author-email: locriginal@gmail.com
 License: gpl-3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
@@ -23,42 +23,82 @@
 [![Build Status](https://app.travis-ci.com/whchien/funda-scraper.svg?branch=main)](https://app.travis-ci.com/whchien/funda-scraper)
 [![codecov](https://codecov.io/gh/whchien/funda-scraper/branch/main/graph/badge.svg?token=QUKTDyeUqp)](https://codecov.io/gh/whchien/funda-scraper)
 [![Downloads](https://static.pepy.tech/badge/funda-scraper)](https://pepy.tech/project/funda-scraper)
 [![PyPI version](https://img.shields.io/pypi/v/funda-scraper)](https://pypi.org/project/funda-scraper/)
 [![PEP8](https://img.shields.io/badge/code%20style-pep8-orange.svg)](https://www.python.org/dev/peps/pep-0008/)
 
 `FundaScaper` provides you the easiest way to perform web scraping from Funda, the Dutch housing website. 
-You can find listings from either house-buyer or rental market, and you can find historical data from the past few year.
+You can find houses either for sale or for rent, and the historical data from the past few year are also attainable.
 
 Please note:
 1. Scraping this website is only allowed for personal use (as per Funda's Terms and Conditions).
 2. Any commercial use of this Python package is prohibited. The author holds no liability for any misuse of the package.
 
 
 ## Install
+1. The easiest way is to install with pip:
 ```
 pip install funda-scraper
 ```
+2. You can also clone the repository to your local machine with:
+```
+git clone https://github.com/whchien/funda-scraper.git
+cd funda-scraper
+export PYTHONPATH=${PWD}
+python funda_scraper/scrape.py
+```
 
 ## Quickstart 
 ```
 from funda_scraper import FundaScraper
 
 scraper = FundaScraper(area="amsterdam", want_to="rent", find_past=False)
-df = scraper.run()
+df = scraper.run(raw_data=False)
 df.head()
 ```
 ![image](https://i.imgur.com/mmN9mjQ.png)
 
+
 You can pass several arguments to `FundaScraper()` for customized scraping:
 - `area`: Specify the city or specific area you want to look for, eg. Amsterdam, Utrecht, Rotterdam, etc
 - `want_to`: You can choose either `buy` or `rent`, which finds houses either for sale or for rent. 
 - `find_past`: Specify whether you want to check the historical data. The default is `False`.
 - `n_pages`: Indicate how many pages you want to look up. The default is `1`. 
 
+The scraped raw result contains following information:
+- url
+- price
+- address
+- description
+- listed_since
+- zip_code 
+- size
+- year_built
+- living_area
+- kind_of_house
+- building_type
+- num_of_rooms
+- num_of_bathrooms
+- layout
+- energy_label
+- insulation
+- heating
+- ownership
+- exteriors
+- parking
+- neighborhood_name
+- date_list
+- date_sold
+- term
+- price_sold
+- last_ask_price
+- last_ask_price_m2
+- city
+
+You can use `scraper.run(raw_data=True)` to fetch the data without preprocessing.
 
-## Advanced usage
+## More information
 
 You can check the [example notebook](https://colab.research.google.com/drive/1hNzJJRWxD59lrbeDpfY1OUpBz0NktmfW?usp=sharing) for further details. 
 Please give me a [star](https://github.com/whchien/funda-scraper) if you find this project helpful.
```

### Comparing `funda-scraper-1.0.0/README.md` & `funda-scraper-1.0.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -4,42 +4,82 @@
 [![Build Status](https://app.travis-ci.com/whchien/funda-scraper.svg?branch=main)](https://app.travis-ci.com/whchien/funda-scraper)
 [![codecov](https://codecov.io/gh/whchien/funda-scraper/branch/main/graph/badge.svg?token=QUKTDyeUqp)](https://codecov.io/gh/whchien/funda-scraper)
 [![Downloads](https://static.pepy.tech/badge/funda-scraper)](https://pepy.tech/project/funda-scraper)
 [![PyPI version](https://img.shields.io/pypi/v/funda-scraper)](https://pypi.org/project/funda-scraper/)
 [![PEP8](https://img.shields.io/badge/code%20style-pep8-orange.svg)](https://www.python.org/dev/peps/pep-0008/)
 
 `FundaScaper` provides you the easiest way to perform web scraping from Funda, the Dutch housing website. 
-You can find listings from either house-buyer or rental market, and you can find historical data from the past few year.
+You can find houses either for sale or for rent, and the historical data from the past few year are also attainable.
 
 Please note:
 1. Scraping this website is only allowed for personal use (as per Funda's Terms and Conditions).
 2. Any commercial use of this Python package is prohibited. The author holds no liability for any misuse of the package.
 
 
 ## Install
+1. The easiest way is to install with pip:
 ```
 pip install funda-scraper
 ```
+2. You can also clone the repository to your local machine with:
+```
+git clone https://github.com/whchien/funda-scraper.git
+cd funda-scraper
+export PYTHONPATH=${PWD}
+python funda_scraper/scrape.py
+```
 
 ## Quickstart 
 ```
 from funda_scraper import FundaScraper
 
 scraper = FundaScraper(area="amsterdam", want_to="rent", find_past=False)
-df = scraper.run()
+df = scraper.run(raw_data=False)
 df.head()
 ```
 ![image](https://i.imgur.com/mmN9mjQ.png)
 
+
 You can pass several arguments to `FundaScraper()` for customized scraping:
 - `area`: Specify the city or specific area you want to look for, eg. Amsterdam, Utrecht, Rotterdam, etc
 - `want_to`: You can choose either `buy` or `rent`, which finds houses either for sale or for rent. 
 - `find_past`: Specify whether you want to check the historical data. The default is `False`.
 - `n_pages`: Indicate how many pages you want to look up. The default is `1`. 
 
+The scraped raw result contains following information:
+- url
+- price
+- address
+- description
+- listed_since
+- zip_code 
+- size
+- year_built
+- living_area
+- kind_of_house
+- building_type
+- num_of_rooms
+- num_of_bathrooms
+- layout
+- energy_label
+- insulation
+- heating
+- ownership
+- exteriors
+- parking
+- neighborhood_name
+- date_list
+- date_sold
+- term
+- price_sold
+- last_ask_price
+- last_ask_price_m2
+- city
+
+You can use `scraper.run(raw_data=True)` to fetch the data without preprocessing.
 
-## Advanced usage
+## More information
 
 You can check the [example notebook](https://colab.research.google.com/drive/1hNzJJRWxD59lrbeDpfY1OUpBz0NktmfW?usp=sharing) for further details. 
 Please give me a [star](https://github.com/whchien/funda-scraper) if you find this project helpful.
```

### Comparing `funda-scraper-1.0.0/funda_scraper/config/config.yaml` & `funda-scraper-1.0.1/funda_scraper/config/config.yaml`

 * *Files identical despite different names*

### Comparing `funda-scraper-1.0.0/funda_scraper/preprocess.py` & `funda-scraper-1.0.1/funda_scraper/preprocess.py`

 * *Files 4% similar despite different names*

```diff
@@ -177,20 +177,16 @@
     df["zip"] = df["zip_code"].apply(lambda x: x[:4])
 
     # House layout
     df["room"] = df["num_of_rooms"].apply(find_n_room)
     df["bedroom"] = df["num_of_rooms"].apply(find_n_bedroom)
     df["bathroom"] = df["num_of_bathrooms"].apply(find_n_bathroom)
     df["energy_label"] = df["energy_label"].apply(clean_energy_label)
-    df["has_balcony"] = df["exteriors"].apply(
-        lambda x: 1 if str(x).find("Balcony present") != -1 else 0
-    )
-    df["has_garden"] = df["exteriors"].apply(
-        lambda x: 1 if str(x).find("garden") != -1 else 0
-    )
+    df["has_balcony"] = df["exteriors"].apply(lambda x: 1 if str(x).find("Balcony present") != -1 else 0)
+    df["has_garden"] = df["exteriors"].apply(lambda x: 1 if str(x).find("garden") != -1 else 0)
 
     # Time
     df["year_built"] = df["year"].apply(clean_year).astype(int)
     df["house_age"] = datetime.now().year - df["year_built"]
 
     if is_past:
         # Only check past data
```

### Comparing `funda-scraper-1.0.0/funda_scraper/scrape.py` & `funda-scraper-1.0.1/funda_scraper/scrape.py`

 * *Files 3% similar despite different names*

```diff
@@ -115,17 +115,15 @@
         for i in tqdm(range(0, self.n_pages + 1)):
             item_list = self._get_links_from_one_parent(f"{main_url}&search_result={i}")
             if len(item_list) == 0:
                 self.n_pages = i
                 break
             urls += item_list
         urls = list(set(urls))
-        logger.info(
-            f"*** Got all the urls. {len(urls)} houses found in {self.n_pages} pages. ***"
-        )
+        logger.info(f"*** Got all the urls. {len(urls)} houses found in {self.n_pages} pages. ***")
         self.links = urls
 
     @staticmethod
     def get_value_from_css(soup: BeautifulSoup, selector: str) -> str:
         """Use CSS selector to find certain features."""
         result = soup.select(selector)
         if len(result) > 0:
@@ -138,59 +136,43 @@
         """Scrape all the features from one house item given a link."""
 
         # Initialize for each page
         response = requests.get(link, headers=config.header)
         soup = BeautifulSoup(response.text, "lxml")
 
         # Get the value according to respective CSS selectors
-        list_since_selector = (
-            self.selectors.listed_since
-            if self.to_buy
-            else ".fd-align-items-center:nth-child(7) span"
-        )
+        list_since_selector = self.selectors.listed_since if self.to_buy else ".fd-align-items-center:nth-child(7) span"
         result = [
             link,
             self.get_value_from_css(soup, self.selectors.price),
             self.get_value_from_css(soup, self.selectors.address),
             self.get_value_from_css(soup, self.selectors.descrip),
             self.get_value_from_css(soup, list_since_selector).replace("\n", ""),
-            self.get_value_from_css(soup, self.selectors.zip_code)
-            .replace("\n", "")
-            .replace("\r        ", ""),
+            self.get_value_from_css(soup, self.selectors.zip_code).replace("\n", "").replace("\r        ", ""),
             self.get_value_from_css(soup, self.selectors.size),
             self.get_value_from_css(soup, self.selectors.year),
             self.get_value_from_css(soup, self.selectors.living_area),
             self.get_value_from_css(soup, self.selectors.kind_of_house),
             self.get_value_from_css(soup, self.selectors.building_type),
-            self.get_value_from_css(soup, self.selectors.num_of_rooms).replace(
-                "\n", ""
-            ),
-            self.get_value_from_css(soup, self.selectors.num_of_bathrooms).replace(
-                "\n", ""
-            ),
+            self.get_value_from_css(soup, self.selectors.num_of_rooms).replace("\n", ""),
+            self.get_value_from_css(soup, self.selectors.num_of_bathrooms).replace("\n", ""),
             self.get_value_from_css(soup, self.selectors.layout),
-            self.get_value_from_css(soup, self.selectors.energy_label).replace(
-                "\r\n        ", ""
-            ),
+            self.get_value_from_css(soup, self.selectors.energy_label).replace("\r\n        ", ""),
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
-            self.get_value_from_css(soup, self.selectors.last_ask_price).replace(
-                "\n", ""
-            ),
-            self.get_value_from_css(soup, self.selectors.last_ask_price_m2).split("\r")[
-                0
-            ],
+            self.get_value_from_css(soup, self.selectors.last_ask_price).replace("\n", ""),
+            self.get_value_from_css(soup, self.selectors.last_ask_price_m2).split("\r")[0],
         ]
 
         return result
 
     def scrape_pages(self) -> None:
         """Scrape all the content acoss multiple pages."""
 
@@ -222,30 +204,26 @@
                 else:
                     status = "rented"
             else:
                 if self.to_buy:
                     status = "selling"
                 else:
                     status = "renting"
-            filepath = (
-                f"./data/houseprice_{date}_{self.area}_{status}_{len(self.links)}.csv"
-            )
+            filepath = f"./data/houseprice_{date}_{self.area}_{status}_{len(self.links)}.csv"
         df.to_csv(filepath, index=False)
         logger.info(f"*** File saved: {filepath}. ***")
 
-    def run(
-        self, raw_data: bool = False, save: bool = False, filepath: str = None
-    ) -> pd.DataFrame:
+    def run(self, raw_data: bool = False, save: bool = False, filepath: str = None) -> pd.DataFrame:
         """
         Scrape all links and all content.
 
-        :param raw_data: if true, the data won't be post-processed
+        :param raw_data: if true, the data won't be pre-processed
         :param save: if true, the data will be saved as a csv file
         :param filepath: the name for the file
-        :return: the (post-processed) dataframe from scraping
+        :return: the (pre-processed) dataframe from scraping
         """
         self.fetch_all_links()
         self.scrape_pages()
 
         if raw_data:
             df = self.raw_df
         else:
@@ -258,11 +236,9 @@
 
         logger.info("*** Done! ***")
         return df
 
 
 if __name__ == "__main__":
     scraper = FundaScraper(area="amsterdam", want_to="buy", find_past=True, n_pages=1)
-    # scraper.fetch_links()
-    # result = scraper.scrape_one_link("https://www.funda.nl/koop/haarlem/huis-42282691-meeuwenstraat-85-garage/")
     df = scraper.run(raw_data=False)
-    print(len(df))
+    print(df.head())
```

### Comparing `funda-scraper-1.0.0/funda_scraper/utils.py` & `funda-scraper-1.0.1/funda_scraper/utils.py`

 * *Files identical despite different names*

### Comparing `funda-scraper-1.0.0/funda_scraper.egg-info/PKG-INFO` & `funda-scraper-1.0.1/funda_scraper.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funda-scraper
-Version: 1.0.0
+Version: 1.0.1
 Summary: FundaScaper provides you the easiest way to perform web scraping from Funda, the Dutch housing website.
 Home-page: https://github.com/whchien/funda-scraper
 Author: Will Chien
 Author-email: locriginal@gmail.com
 License: gpl-3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
@@ -23,42 +23,82 @@
 [![Build Status](https://app.travis-ci.com/whchien/funda-scraper.svg?branch=main)](https://app.travis-ci.com/whchien/funda-scraper)
 [![codecov](https://codecov.io/gh/whchien/funda-scraper/branch/main/graph/badge.svg?token=QUKTDyeUqp)](https://codecov.io/gh/whchien/funda-scraper)
 [![Downloads](https://static.pepy.tech/badge/funda-scraper)](https://pepy.tech/project/funda-scraper)
 [![PyPI version](https://img.shields.io/pypi/v/funda-scraper)](https://pypi.org/project/funda-scraper/)
 [![PEP8](https://img.shields.io/badge/code%20style-pep8-orange.svg)](https://www.python.org/dev/peps/pep-0008/)
 
 `FundaScaper` provides you the easiest way to perform web scraping from Funda, the Dutch housing website. 
-You can find listings from either house-buyer or rental market, and you can find historical data from the past few year.
+You can find houses either for sale or for rent, and the historical data from the past few year are also attainable.
 
 Please note:
 1. Scraping this website is only allowed for personal use (as per Funda's Terms and Conditions).
 2. Any commercial use of this Python package is prohibited. The author holds no liability for any misuse of the package.
 
 
 ## Install
+1. The easiest way is to install with pip:
 ```
 pip install funda-scraper
 ```
+2. You can also clone the repository to your local machine with:
+```
+git clone https://github.com/whchien/funda-scraper.git
+cd funda-scraper
+export PYTHONPATH=${PWD}
+python funda_scraper/scrape.py
+```
 
 ## Quickstart 
 ```
 from funda_scraper import FundaScraper
 
 scraper = FundaScraper(area="amsterdam", want_to="rent", find_past=False)
-df = scraper.run()
+df = scraper.run(raw_data=False)
 df.head()
 ```
 ![image](https://i.imgur.com/mmN9mjQ.png)
 
+
 You can pass several arguments to `FundaScraper()` for customized scraping:
 - `area`: Specify the city or specific area you want to look for, eg. Amsterdam, Utrecht, Rotterdam, etc
 - `want_to`: You can choose either `buy` or `rent`, which finds houses either for sale or for rent. 
 - `find_past`: Specify whether you want to check the historical data. The default is `False`.
 - `n_pages`: Indicate how many pages you want to look up. The default is `1`. 
 
+The scraped raw result contains following information:
+- url
+- price
+- address
+- description
+- listed_since
+- zip_code 
+- size
+- year_built
+- living_area
+- kind_of_house
+- building_type
+- num_of_rooms
+- num_of_bathrooms
+- layout
+- energy_label
+- insulation
+- heating
+- ownership
+- exteriors
+- parking
+- neighborhood_name
+- date_list
+- date_sold
+- term
+- price_sold
+- last_ask_price
+- last_ask_price_m2
+- city
+
+You can use `scraper.run(raw_data=True)` to fetch the data without preprocessing.
 
-## Advanced usage
+## More information
 
 You can check the [example notebook](https://colab.research.google.com/drive/1hNzJJRWxD59lrbeDpfY1OUpBz0NktmfW?usp=sharing) for further details. 
 Please give me a [star](https://github.com/whchien/funda-scraper) if you find this project helpful.
```

### Comparing `funda-scraper-1.0.0/funda_scraper.egg-info/SOURCES.txt` & `funda-scraper-1.0.1/funda_scraper.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 MANIFEST.in
 README.md
 pyproject.toml
-requirements.txt
 setup.py
 ./requirements/requirements.txt
 funda_scraper/VERSION
 funda_scraper/__init__.py
 funda_scraper/preprocess.py
 funda_scraper/scrape.py
 funda_scraper/utils.py
```

### Comparing `funda-scraper-1.0.0/setup.py` & `funda-scraper-1.0.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 # -*- coding: utf-8 -*-
 
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 # Package meta-data.
-NAME = 'funda-scraper'
+NAME = "funda-scraper"
 URL = "https://github.com/whchien/funda-scraper"
 DESCRIPTION = "FundaScaper provides you the easiest way to perform web scraping from Funda, the Dutch housing website."
 EMAIL = "locriginal@gmail.com"
 AUTHOR = "Will Chien"
 REQUIRES_PYTHON = ">=3.7.0"
 
 about = {}
 ROOT_DIR = Path(__file__).resolve().parent
-REQUIREMENTS_DIR = ROOT_DIR / 'requirements'
-PACKAGE_DIR = ROOT_DIR / 'funda_scraper'
+REQUIREMENTS_DIR = ROOT_DIR / "requirements"
+PACKAGE_DIR = ROOT_DIR / "funda_scraper"
 long_description = (ROOT_DIR / "README.md").read_text()
 with open(PACKAGE_DIR / "VERSION") as f:
     _version = f.read().strip()
     about["__version__"] = _version
 
 
 def list_reqs(fname="requirements.txt"):
```

### Comparing `funda-scraper-1.0.0/static/example_df.png` & `funda-scraper-1.0.1/static/example_df.png`

 * *Files identical despite different names*

### Comparing `funda-scraper-1.0.0/tests/test_preprocess.py` & `funda-scraper-1.0.1/tests/test_preprocess.py`

 * *Files identical despite different names*

### Comparing `funda-scraper-1.0.0/tests/test_scrape.py` & `funda-scraper-1.0.1/tests/test_scrape.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,48 +1,40 @@
 from funda_scraper.preprocess import preprocess_data
 from funda_scraper.scrape import FundaScraper
 
 
 class TestFundaScraper(object):
     def test_rent(self):
-        scraper = FundaScraper(
-            area="amsterdam", want_to="rent", find_past=False, n_pages=1
-        )
+        scraper = FundaScraper(area="amsterdam", want_to="rent", find_past=False, n_pages=1)
         df = scraper.run(raw_data=True)
         assert len(scraper.links) > 1
         assert df.shape[1] == 26
 
         df = preprocess_data(df, is_past=False)
         assert df.shape[1] == 21
 
     def test_rent_past(self):
-        scraper = FundaScraper(
-            area="amsterdam", want_to="rent", find_past=True, n_pages=1
-        )
+        scraper = FundaScraper(area="amsterdam", want_to="rent", find_past=True, n_pages=1)
         df = scraper.run(raw_data=True)
         assert len(scraper.links) > 1
         assert df.shape[1] == 29
 
         df = preprocess_data(df, is_past=True)
         assert df.shape[1] == 25
 
     def test_buy(self):
-        scraper = FundaScraper(
-            area="amsterdam", want_to="buy", find_past=False, n_pages=1
-        )
+        scraper = FundaScraper(area="amsterdam", want_to="buy", find_past=False, n_pages=1)
         df = scraper.run(raw_data=True)
         assert len(scraper.links) > 1
         assert df.shape[1] == 26
 
         df = preprocess_data(df, is_past=False)
         assert df.shape[1] == 21
 
     def test_buy_past(self):
-        scraper = FundaScraper(
-            area="amsterdam", want_to="buy", find_past=True, n_pages=1
-        )
+        scraper = FundaScraper(area="amsterdam", want_to="buy", find_past=True, n_pages=1)
         df = scraper.run(raw_data=True)
         assert len(scraper.links) > 1
         assert df.shape[1] == 29
 
         df = preprocess_data(df, is_past=True)
         assert df.shape[1] == 25
```

