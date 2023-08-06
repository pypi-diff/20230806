# Comparing `tmp/gmn-python-api-0.0.8.tar.gz` & `tmp/gmn-python-api-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmn-python-api-0.0.8.tar", max compression
+gzip compressed data, was "gmn-python-api-0.0.9.tar", max compression
```

## Comparing `gmn-python-api-0.0.8.tar` & `gmn-python-api-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1072 2022-12-30 18:13:19.153935 gmn-python-api-0.0.8/LICENSE
--rw-r--r--   0        0        0     4584 2022-12-30 18:13:19.153935 gmn-python-api-0.0.8/README.md
--rw-r--r--   0        0        0     1888 2022-12-30 18:13:30.125985 gmn-python-api-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      469 2022-12-30 18:13:19.153935 gmn-python-api-0.0.8/src/gmn_python_api/__init__.py
--rw-r--r--   0        0        0      218 2022-12-30 18:13:19.153935 gmn-python-api-0.0.8/src/gmn_python_api/__main__.py
--rw-r--r--   0        0        0     7230 2022-12-30 18:13:19.153935 gmn-python-api-0.0.8/src/gmn_python_api/data_directory.py
--rw-r--r--   0        0        0   496793 2022-12-30 18:13:19.157935 gmn-python-api-0.0.8/src/gmn_python_api/data_models/traj_summary_20220304_solrange_344.0-345.0.txt
--rw-r--r--   0        0        0     3758 2022-12-30 18:13:19.157935 gmn-python-api-0.0.8/src/gmn_python_api/data_models/traj_summary_20220304_solrange_344.0-345.0_one_row.txt
--rw-r--r--   0        0        0     6227 2022-12-30 18:13:19.157935 gmn-python-api-0.0.8/src/gmn_python_api/gmn_rest_api.py
--rw-r--r--   0        0        0     1260 2022-12-30 18:13:19.157935 gmn-python-api-0.0.8/src/gmn_python_api/iau_showers.py
--rw-r--r--   0        0        0     9445 2022-12-30 18:13:19.157935 gmn-python-api-0.0.8/src/gmn_python_api/meteor_summary_reader.py
--rw-r--r--   0        0        0     1688 2022-12-30 18:13:19.157935 gmn-python-api-0.0.8/src/gmn_python_api/meteor_summary_schema.py
--rw-r--r--   0        0        0        0 2022-12-30 18:13:19.157935 gmn-python-api-0.0.8/src/gmn_python_api/py.typed
--rw-r--r--   0        0        0     5716 2022-12-30 18:13:33.220521 gmn-python-api-0.0.8/setup.py
--rw-r--r--   0        0        0     5619 2022-12-30 18:13:33.221064 gmn-python-api-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-04-21 22:14:17.675487 gmn-python-api-0.0.9/LICENSE
+-rw-r--r--   0        0        0     4226 2023-04-21 22:14:17.675487 gmn-python-api-0.0.9/README.md
+-rw-r--r--   0        0        0     1929 2023-04-21 22:14:27.499712 gmn-python-api-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      481 2023-04-21 22:14:17.679487 gmn-python-api-0.0.9/src/gmn_python_api/__init__.py
+-rw-r--r--   0        0        0      218 2023-04-21 22:14:17.679487 gmn-python-api-0.0.9/src/gmn_python_api/__main__.py
+-rw-r--r--   0        0        0     7269 2023-04-21 22:14:17.679487 gmn-python-api-0.0.9/src/gmn_python_api/data_directory.py
+-rw-r--r--   0        0        0   496793 2023-04-21 22:14:17.683487 gmn-python-api-0.0.9/src/gmn_python_api/data_models/traj_summary_20220304_solrange_344.0-345.0.txt
+-rw-r--r--   0        0        0     3758 2023-04-21 22:14:17.683487 gmn-python-api-0.0.9/src/gmn_python_api/data_models/traj_summary_20220304_solrange_344.0-345.0_one_row.txt
+-rw-r--r--   0        0        0     6275 2023-04-21 22:14:17.683487 gmn-python-api-0.0.9/src/gmn_python_api/gmn_rest_api.py
+-rw-r--r--   0        0        0     1273 2023-04-21 22:14:17.683487 gmn-python-api-0.0.9/src/gmn_python_api/iau_showers.py
+-rw-r--r--   0        0        0     4603 2023-04-21 22:14:17.683487 gmn-python-api-0.0.9/src/gmn_python_api/meteor_trajectory_reader.py
+-rw-r--r--   0        0        0     2880 2023-04-21 22:14:17.683487 gmn-python-api-0.0.9/src/gmn_python_api/meteor_trajectory_schema.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:14:17.683487 gmn-python-api-0.0.9/src/gmn_python_api/py.typed
+-rw-r--r--   0        0        0     5392 2023-04-21 22:14:29.899477 gmn-python-api-0.0.9/setup.py
+-rw-r--r--   0        0        0     5328 2023-04-21 22:14:29.900018 gmn-python-api-0.0.9/PKG-INFO
```

### Comparing `gmn-python-api-0.0.8/LICENSE` & `gmn-python-api-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gmn-python-api-0.0.8/README.md` & `gmn-python-api-0.0.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -20,32 +20,26 @@
 
 ![Screenshot of GMN data](docs/screenshot.png)
 
 [Demo on Google Colab](https://colab.research.google.com/gist/rickybassom/74d2c99ebbd612b88861038a5b33e021/gmn_data_analysis_template.ipynb)
 
 ## Features
 
-- Listing available daily and monthly csv trajectory summary files from the 
-  [GMN data directory](https://globalmeteornetwork.org/data/traj_summary_data/).
+- Listing available daily and monthly meteor trajectory files from the 
+  [GMN Data Directory](https://globalmeteornetwork.org/data/traj_summary_data/).
 
-- Downloading specific daily and monthly csv trajectory summary files from the data
-  directory.
+- Downloading specific CSV meteor trajectory data from the GMN Data Directory or GMN 
+  REST API.
 
-- Functions for loading the data directory trajectory summary data into 
-  [Pandas](https://pandas.pydata.org/) DataFrames or [Numpy](https://numpy.org/) arrays.
-
-- Functions for retrieving meteor summary data from the future GMN Data Store using the
-  GMN REST API.
-
-- Functions for loading REST API meteor summary data
-  into [Pandas](https://pandas.pydata.org/) DataFrames or [Numpy](https://numpy.org/)
-  arrays.
+- Functions for loading meteor trajectory data into [Pandas](https://pandas.pydata.org/)
+  DataFrames.
 
 - Functions for retrieving available 
-  [IAU](https://www.ta3.sk/IAUC22DB/MDC2007/Roje/roje_lista.php) registered meteor showers.
+  [IAU](https://www.ta3.sk/IAUC22DB/MDC2007/Roje/roje_lista.php) registered meteor
+  showers.
 
 ## Requirements
 
 - Python 3.7.1+, 3.8, 3.9 or 3.10
 
 ## Installation
 
@@ -75,29 +69,30 @@
 
 ## Usage
 
 Simple meteor analysis example:
 
 ```python
 from gmn_python_api import data_directory as dd
-from gmn_python_api import meteor_summary_reader as reader
+from gmn_python_api import meteor_trajectory_reader
 
 # Analyse recorded meteor data for the 24th of July 2019
-traj_sum_file_content = dd.get_daily_file_content_by_date("2019-07-24")
+traj_file_content = dd.get_daily_file_content_by_date("2019-07-24")
 
 # Read data as a Pandas DataFrame
-traj_sum_df = reader.read_meteor_summary_csv_as_dataframe(traj_sum_file_content)
+traj_df = meteor_trajectory_reader.read_csv(traj_file_content)
 
-print(f"{traj_sum_df['Vgeo (km/s)'].max()} km/s was the fastest geostationary velocity")
+print(f"{traj_df['Vgeo (km/s)'].max()} km/s was the fastest geostationary velocity")
 # Output: 65.38499 km/s was the fastest geostationary velocity
 
-print(f"{traj_sum_df.loc[traj_sum_df['IAU (code)'] == 'PER'].shape[0]} Perseid meteors")
+print(f"{traj_df.loc[traj_df['IAU (code)'] == 'PER'].shape[0]} Perseid meteors")
 # Output: 8 Perseid meteors
 
-print(f"Station #{traj_sum_df['Num (stat)'].mode().values[0]} recorded the most meteors")
+print(
+  f"Station #{traj_df['Num (stat)'].mode().values[0]} recorded the most meteors")
 # Output: Station #2 recorded the most meteors
 ```
 
 Please see the [Usage](https://gmn-python-api.readthedocs.io/en/latest/usage.html) and 
 [API Reference](https://gmn-python-api.readthedocs.io/en/latest/autoapi/gmn_python_api/index.html)
 sections for more details.
```

### Comparing `gmn-python-api-0.0.8/pyproject.toml` & `gmn-python-api-0.0.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gmn-python-api"
-version = "0.0.8"
+version = "0.0.9"
 description = "GMN Python API"
 authors = ["Ricky Bassom <rickybas12@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/rickybassom/gmn-python-api"
 repository = "https://github.com/rickybassom/gmn-python-api"
 documentation = "https://gmn-python-api.readthedocs.io"
@@ -19,14 +19,16 @@
 python = "^3.7.1"
 click = "8.0.4"
 pandas = ">=1.1.0, <=1.3.5"
 numpy = ">1.20.3"
 beautifulsoup4 = "^4.10.0"
 requests = "^2.21.0"
 types-requests = "^2.27.8"
+future = ">=0.18.3"
+werkzeug = ">=2.2.3"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.0.1"
 coverage = {extras = ["toml"], version = "^6.1"}
 safety = "^2.2.0"
 mypy = "^0.931"
 sphinx = "^4.3.0"
```

### Comparing `gmn-python-api-0.0.8/src/gmn_python_api/data_directory.py` & `gmn-python-api-0.0.9/src/gmn_python_api/data_directory.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,86 +1,88 @@
 """
-This module contains functions to read trajectory summary files from the GMN data
-directory.
+This module contains functions to read meteor trajectory files from the GMN Data
+ Directory.
 """
 from datetime import date, datetime
 from datetime import timedelta
 from typing import List
 from typing import Optional
 
 import requests
 from bs4 import BeautifulSoup  # type: ignore
 
 BASE_URL: str = "https://globalmeteornetwork.org/data/traj_summary_data/"
-"""The base URL for trajectory summary files in the GMN data directory."""
+"""The base URL for meteor trajectory files in the GMN Data Directory."""
 
 DATA_START_DATE: date = date(2018, 12, 9)
-"""The date of the earliest trajectory summary file in the GMN data directory."""
+"""The date of the earliest meteor trajectory file in the GMN Data Directory."""
 
 DAILY_DIRECTORY: str = "daily/"
-"""The name of the directory containing daily trajectory summary files in the
-base URL."""
+"""The name of the directory containing daily meteor trajectory files in the base
+ URL."""
 
 MONTHLY_DIRECTORY: str = "monthly/"
-"""The name of the directory containing monthly trajectory summary files in
-# the base URL."""
+"""The name of the directory containing monthly meteor trajectory files in the base
+ URL."""
 
 SUMMARY_FILE_EXTENSION: str = "txt"
-"""The extension of the trajectory summary files in the GMN data directory"""
+"""The extension of the meteor trajectory files in the GMN Data Directory"""
 
 SUMMARY_TODAY_FILENAME: str = "traj_summary_latest_daily.txt"
-"""The filename of the most recent trajectory summary file."""
+"""The filename of the most recent meteor trajectory file."""
 
 SUMMARY_YESTERDAY_FILENAME: str = "traj_summary_yesterday.txt"
-"""The filename of the trajectory summary file from yesterday."""
+"""The filename of the meteo trajectory file from yesterday."""
 
 SUMMARY_ALL_FILENAME: str = "traj_summary_all.txt"
-"""The filename of the trajectory summary file containing all data."""
+"""The filename of the meteor trajectory file containing all data."""
 
 DAILY_DATE_INPUT_FORMAT: str = "%Y-%m-%d"
-"""The daily string date format that should be passed into the functions in this."""
+"""The daily string date format that should be passed in as a parameter to the
+ functions in this module."""
 
 MONTHLY_DATE_INPUT_FORMAT: str = "%Y-%m"
-"""The monthly string date format that should be passed into the functions in this."""
+"""The monthly string date format that should be passed in as a parameter to the
+ functions in this module."""
 
 
 def get_all_daily_file_urls() -> List[str]:
     """
-    Get all daily trajectory summary file urls from the GMN data directory.
+    Get all daily meteor trajectory file urls from the GMN Data Directory.
 
     :return: A list of all daily file urls.
     :raises: requests.HTTPError if the data directory url doesn't return a 200 response.
     """
     return _get_url_paths(BASE_URL + DAILY_DIRECTORY, SUMMARY_FILE_EXTENSION)
 
 
 def get_all_monthly_file_urls() -> List[str]:
     """
-    Get all monthly trajectory summary file urls from the GMN data directory.
+    Get all monthly meteor trajectory file urls from the GMN Data Directory.
 
     :return: A list of all monthly file urls.
     :raises: requests.HTTPError if the data directory url doesn't return a 200 response.
     """
     return _get_url_paths(BASE_URL + MONTHLY_DIRECTORY, SUMMARY_FILE_EXTENSION)
 
 
 def get_all_file_url() -> str:
     """
-    Get the URL of the trajectory summary file containing all data.
+    Get the URL of the meteor trajectory file containing all data.
 
     :return: The URL of the file containing all data.
     """
     return BASE_URL + SUMMARY_ALL_FILENAME
 
 
 def get_daily_file_url_by_date(
         date_str: str, current_date: Optional[date] = None
 ) -> str:
     """
-    Get the URL of the daily trajectory summary file for a given date.
+    Get the URL of the daily meteor trajectory file for a given date.
 
     :param date_str: The date of the daily file to get in the format YYYY-MM-DD.
     :param current_date: The current date. Defaults to datetime.now().
 
     :return: The URL of the daily file.
     :raises: FileNotFoundError if the daily file cannot be found. Or
      requests.HTTPError is raised if the file url doesn't return a 200 response.
@@ -100,23 +102,23 @@
 
     all_daily_filenames = get_all_daily_file_urls()
     files_containing_date = [
         f for f in all_daily_filenames if date.strftime("%Y%m%d") in f
     ]
 
     if len(files_containing_date) == 0:
-        raise FileNotFoundError(f"Trajectory summary file not found for date "
+        raise FileNotFoundError(f"Meteor trajectory file not found for date "
                                 f"{date.strftime(DAILY_DATE_INPUT_FORMAT)}")
 
     return files_containing_date[0]
 
 
 def get_monthly_file_url_by_month(date_str: str) -> str:
     """
-    Get the URL of the monthly trajectory summary file for a given month.
+    Get the URL of the monthly meteor trajectory file for a given month.
 
     :param date_str: The date of the monthly file to get in the format YYYY-MM.
 
     :return: The URL of the monthly file.
     :raises: FileNotFoundError if the monthly file cannot be found. Or
      requests.HTTPError is raised if the file url doesn't return a 200 response.
     """
@@ -124,70 +126,70 @@
     all_monthly_filenames = get_all_monthly_file_urls()
     files_containing_date = [
         f for f in all_monthly_filenames if date.strftime("%Y%m") in f
     ]
 
     if len(files_containing_date) == 0:
         raise FileNotFoundError(
-            f"Trajectory summary file not found for month in date "
+            f"Meteor trajectory file not found for month in date "
             f"{date.strftime(MONTHLY_DATE_INPUT_FORMAT)}"
         )
 
     return files_containing_date[0]
 
 
 def get_file_content_from_url(file_url: str) -> str:
     """
-    Get the content of a trajectory summary file from a given URL.
+    Get the content of a meteor trajectory file from a given URL.
 
-    :param url: The URL of the trajectory summary file.
+    :param url: The URL of the meteor trajectory file.
 
     :return: The content of the file.
     :raises: requests.HTTPError If the file url doesn't return a 200 response.
     """
-    response = requests.get(file_url)
+    response = requests.get(file_url, timeout=200)
     if response.ok:
         return str(response.text)
     else:
         response.raise_for_status()
         return ""  # pragma: no cover
 
 
 def get_daily_file_content_by_date(
         date_str: str, current_date: Optional[date] = None
 ) -> str:
     """
-    Get the content of the daily trajectory summary file for a given date.
+    Get the content of the daily meteo trajectory file for a given date.
 
     :param date_str: The date of the daily file to get in the format YYYY-MM-DD.
     :param current_date: The current date. Defaults to datetime.now().
 
     :return: The content of the daily file.
     :raises: requests.HTTPError if the data directory url doesn't return a 200 response.
     """
     file_url = get_daily_file_url_by_date(date_str, current_date)
     return get_file_content_from_url(file_url)
 
 
 def get_monthly_file_content_by_date(date_str: str) -> str:
     """
-    Get the content of the monthly trajectory summary file for a given date.
+    Get the content of the monthly meteor trajectory file for a given date.
 
     :param date_str: The date to get the monthly file for in the format YYYY-MM.
 
     :return: The content of the monthly file.
     :raises: requests.HTTPError if the data directory url doesn't return a 200 response.
     """
     file_url = get_monthly_file_url_by_month(date_str)
     return get_file_content_from_url(file_url)
 
 
 def get_all_file_content() -> str:
     """
-    Get the content of the trajectory summary file containing all data.
+    Get the content of the meteor trajectory file containing all data.
 
     :return: The content of the file containing all data.
     :raises: requests.HTTPError if the data directory url doesn't return a 200 response.
     """
     file_url = get_all_file_url()
     return get_file_content_from_url(file_url)
```

### Comparing `gmn-python-api-0.0.8/src/gmn_python_api/data_models/traj_summary_20220304_solrange_344.0-345.0.txt` & `gmn-python-api-0.0.9/src/gmn_python_api/data_models/traj_summary_20220304_solrange_344.0-345.0.txt`

 * *Files identical despite different names*

### Comparing `gmn-python-api-0.0.8/src/gmn_python_api/data_models/traj_summary_20220304_solrange_344.0-345.0_one_row.txt` & `gmn-python-api-0.0.9/src/gmn_python_api/data_models/traj_summary_20220304_solrange_344.0-345.0_one_row.txt`

 * *Files identical despite different names*

### Comparing `gmn-python-api-0.0.8/src/gmn_python_api/gmn_rest_api.py` & `gmn-python-api-0.0.9/src/gmn_python_api/gmn_rest_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-This module contains functions to read meteor summary data from the GMN REST API.
+This module contains functions to read meteor trajectory data from the GMN REST API.
  The REST API uses the Datasette API endpoint. More info:
  https://docs.datasette.io/en/stable/json_api.html
 """
 from enum import Enum
 from typing import Dict
 from typing import Optional
 from typing import Tuple
@@ -40,15 +40,15 @@
 
 
 def get_meteor_summary_data_reader_compatible(
     where_sql: Optional[str] = None,
     next_page: Optional[str] = None,
 ) -> Tuple[str, Optional[str]]:
     """
-    Get meteor summary data from the GMN REST API in a format that is compatible with
+    Get meteor trajectory data from the GMN REST API in a format that is compatible with
      the meteor_summary_reader functions.
 
     :param where_sql: An optional SQL WHERE clause to filter the data (e.g. iau_no='4').
     :param next_page: An optional URL to access more paginated data provided by the api.
 
     :return: The data returned from the GMN REST API in CSV format.
     :raises: requests.HTTPError If GMN REST API doesn't return a 200 response.
@@ -64,15 +64,15 @@
 def get_meteor_summary_data(
     table_arguments: Optional[Dict[str, str]] = None,
     data_format: DataFormat = DataFormat.JSON,
     data_shape: DataShape = DataShape.ARRAY,
     next_page: Optional[str] = None,
 ) -> Tuple[str, Optional[str]]:
     """
-    Get meteor summary data from the GMN REST API.
+    Get meteor trajectory data from the GMN REST API.
 
     :param table_arguments: An optional dictionary of arguments to filter the data.
      A full list of arguments can be found here:
      https://docs.datasette.io/en/stable/json_api.html#table-arguments
     :param data_format: The data format of the meteor summary data using DataFormat
      enum.
     :param data_shape: The data shape of the meteor summary data using the DataShape
@@ -158,23 +158,23 @@
     Get resultant data from a given GMN REST API URL.
 
     :param url: A query URL of the GMN REST API.
 
     :return: Data, and a URL to access more paginated data if required.
     :raises: requests.HTTPError If URL doesn't return a 200 response.
     """
-    response = requests.get(url)
+    response = requests.get(url, timeout=200)
     if response.ok:
         try:
             next_url = response.links.get("next").get("url")  # type: ignore
         except AttributeError:
             # next_url somtimes is not given even when paginated (for example with CSVs)
             if str(response.text).count("\n") == 101 and (
-                requests.head(url + "&_next=100").ok
-                or requests.head(url + "?_next=100").ok
+                requests.head(url + "&_next=100", timeout=200).ok
+                or requests.head(url + "?_next=100", timeout=200).ok
             ):  # pragma: no cover
                 next_url = url + "&_next=100" if "?" in url else url + "?_next=100"
             else:
                 next_url = None
         return str(response.text), next_url
     else:
         response.raise_for_status()
```

### Comparing `gmn-python-api-0.0.8/src/gmn_python_api/iau_showers.py` & `gmn-python-api-0.0.9/src/gmn_python_api/iau_showers.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     """
     Gets the official list of IAU shower numbers, codes and names.
 
     :return: A dictionary, where the key is the shower number, of dictionaries
      containing the IAU shower information.
     :raises: requests.HTTPError if the source server doesn't return a 200 response.
     """
-    response = requests.get(IAU_SHOWERS_LIST_URL)
+    response = requests.get(IAU_SHOWERS_LIST_URL, timeout=200)
     if not response.ok:
         response.raise_for_status()
         return {}  # pragma: no cover
 
     showers = {}
     for row in response.text.splitlines():
         if not row or row.startswith(":") or row.startswith("+"):
```

### Comparing `gmn-python-api-0.0.8/setup.py` & `gmn-python-api-0.0.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,27 +9,29 @@
 
 package_data = \
 {'': ['*'], 'gmn_python_api': ['data_models/*']}
 
 install_requires = \
 ['beautifulsoup4>=4.10.0,<5.0.0',
  'click==8.0.4',
+ 'future>=0.18.3',
  'numpy>1.20.3',
  'pandas>=1.1.0,<=1.3.5',
  'requests>=2.21.0,<3.0.0',
- 'types-requests>=2.27.8,<3.0.0']
+ 'types-requests>=2.27.8,<3.0.0',
+ 'werkzeug>=2.2.3']
 
 entry_points = \
 {'console_scripts': ['gmn-python-api = gmn_python_api.__main__:main']}
 
 setup_kwargs = {
     'name': 'gmn-python-api',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': 'GMN Python API',
-    'long_description': '[![PyPI](https://img.shields.io/pypi/v/gmn-python-api)](https://pypi.org/project/gmn-python-api/)\n[![Status](https://img.shields.io/pypi/status/gmn-python-api)](https://pypi.org/project/gmn-python-api/)\n[![Python versions](https://img.shields.io/pypi/pyversions/gmn-python-api)](https://pypi.org/project/gmn-python-api/)\n[![License](https://img.shields.io/pypi/l/gmn-python-api)](https://pypi.org/project/gmn-python-api/)\n\n[![Read the Docs](https://img.shields.io/readthedocs/gmn-python-api)](https://gmn-python-api.readthedocs.io/en/latest/)\n[![Tests](https://github.com/rickybassom/gmn-python-api/workflows/Tests/badge.svg)](https://github.com/rickybassom/gmn-python-api/actions?query=workflow%3ATests+branch%3Amain)\n[![Codecov](https://codecov.io/gh/rickybassom/gmn-python-api/branch/main/graph/badge.svg)](https://codecov.io/gh/rickybassom/gmn-python-api)\n\n[![Demo on Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/rickybassom/74d2c99ebbd612b88861038a5b33e021/gmn_data_analysis_template.ipynb)\n\n# gmn-python-api\n\nThis library provides a Python API for accessing open \n[Global Meteor Network](https://globalmeteornetwork.org/) (GMN) meteor trajectory \n[data](https://globalmeteornetwork.org/data/). Global meteor data is generated using a \nnetwork of low-light cameras pointed towards the night sky. Meteor properties (radiants,\norbits, magnitudes and masses) are produced by the GMN and are available through this\nlibrary.\n\n![Screenshot of GMN data](docs/screenshot.png)\n\n[Demo on Google Colab](https://colab.research.google.com/gist/rickybassom/74d2c99ebbd612b88861038a5b33e021/gmn_data_analysis_template.ipynb)\n\n## Features\n\n- Listing available daily and monthly csv trajectory summary files from the \n  [GMN data directory](https://globalmeteornetwork.org/data/traj_summary_data/).\n\n- Downloading specific daily and monthly csv trajectory summary files from the data\n  directory.\n\n- Functions for loading the data directory trajectory summary data into \n  [Pandas](https://pandas.pydata.org/) DataFrames or [Numpy](https://numpy.org/) arrays.\n\n- Functions for retrieving meteor summary data from the future GMN Data Store using the\n  GMN REST API.\n\n- Functions for loading REST API meteor summary data\n  into [Pandas](https://pandas.pydata.org/) DataFrames or [Numpy](https://numpy.org/)\n  arrays.\n\n- Functions for retrieving available \n  [IAU](https://www.ta3.sk/IAUC22DB/MDC2007/Roje/roje_lista.php) registered meteor showers.\n\n## Requirements\n\n- Python 3.7.1+, 3.8, 3.9 or 3.10\n\n## Installation\n\nYou can install `gmn-python-api` via [pip](https://pip.pypa.io/) from \n[PyPI](https://pypi.org/project/gmn-python-api/):\n\n```sh\npip install gmn-python-api\n```\n\nOr install the latest development code, through \n[TestPyPI](https://test.pypi.org/project/gmn-python-api/) or directly from \n[GitHub](https://github.com/rickybassom/gmn-python-api) via \n[pip](https://pip.pypa.io/):\n\n```sh\npip install -i https://test.pypi.org/simple/ --extra-index-url https://pypi.org/simple gmn-python-api==<version>\n```\n\nOr\n\n```sh\npip install git+https://github.com/rickybassom/gmn-python-api\n```\n\nRefer to the [Troubleshooting] guide if you encounter any issues.\n\n## Usage\n\nSimple meteor analysis example:\n\n```python\nfrom gmn_python_api import data_directory as dd\nfrom gmn_python_api import meteor_summary_reader as reader\n\n# Analyse recorded meteor data for the 24th of July 2019\ntraj_sum_file_content = dd.get_daily_file_content_by_date("2019-07-24")\n\n# Read data as a Pandas DataFrame\ntraj_sum_df = reader.read_meteor_summary_csv_as_dataframe(traj_sum_file_content)\n\nprint(f"{traj_sum_df[\'Vgeo (km/s)\'].max()} km/s was the fastest geostationary velocity")\n# Output: 65.38499 km/s was the fastest geostationary velocity\n\nprint(f"{traj_sum_df.loc[traj_sum_df[\'IAU (code)\'] == \'PER\'].shape[0]} Perseid meteors")\n# Output: 8 Perseid meteors\n\nprint(f"Station #{traj_sum_df[\'Num (stat)\'].mode().values[0]} recorded the most meteors")\n# Output: Station #2 recorded the most meteors\n```\n\nPlease see the [Usage](https://gmn-python-api.readthedocs.io/en/latest/usage.html) and \n[API Reference](https://gmn-python-api.readthedocs.io/en/latest/autoapi/gmn_python_api/index.html)\nsections for more details.\n\n## Contributing\nContributions are very welcome. To learn more, see the \n[Contributing guide].\n\n## License\n\nDistributed under the terms of the [MIT](https://opensource.org/licenses/MIT) license,\n`gmn-python-api` is free and open source software.\n\n<!-- Links -->\n[Troubleshooting]: ./TROUBLESHOOTING.md\n[Contributing guide]: ./CONTRIBUTING.md\n',
+    'long_description': '[![PyPI](https://img.shields.io/pypi/v/gmn-python-api)](https://pypi.org/project/gmn-python-api/)\n[![Status](https://img.shields.io/pypi/status/gmn-python-api)](https://pypi.org/project/gmn-python-api/)\n[![Python versions](https://img.shields.io/pypi/pyversions/gmn-python-api)](https://pypi.org/project/gmn-python-api/)\n[![License](https://img.shields.io/pypi/l/gmn-python-api)](https://pypi.org/project/gmn-python-api/)\n\n[![Read the Docs](https://img.shields.io/readthedocs/gmn-python-api)](https://gmn-python-api.readthedocs.io/en/latest/)\n[![Tests](https://github.com/rickybassom/gmn-python-api/workflows/Tests/badge.svg)](https://github.com/rickybassom/gmn-python-api/actions?query=workflow%3ATests+branch%3Amain)\n[![Codecov](https://codecov.io/gh/rickybassom/gmn-python-api/branch/main/graph/badge.svg)](https://codecov.io/gh/rickybassom/gmn-python-api)\n\n[![Demo on Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/rickybassom/74d2c99ebbd612b88861038a5b33e021/gmn_data_analysis_template.ipynb)\n\n# gmn-python-api\n\nThis library provides a Python API for accessing open \n[Global Meteor Network](https://globalmeteornetwork.org/) (GMN) meteor trajectory \n[data](https://globalmeteornetwork.org/data/). Global meteor data is generated using a \nnetwork of low-light cameras pointed towards the night sky. Meteor properties (radiants,\norbits, magnitudes and masses) are produced by the GMN and are available through this\nlibrary.\n\n![Screenshot of GMN data](docs/screenshot.png)\n\n[Demo on Google Colab](https://colab.research.google.com/gist/rickybassom/74d2c99ebbd612b88861038a5b33e021/gmn_data_analysis_template.ipynb)\n\n## Features\n\n- Listing available daily and monthly meteor trajectory files from the \n  [GMN Data Directory](https://globalmeteornetwork.org/data/traj_summary_data/).\n\n- Downloading specific CSV meteor trajectory data from the GMN Data Directory or GMN \n  REST API.\n\n- Functions for loading meteor trajectory data into [Pandas](https://pandas.pydata.org/)\n  DataFrames.\n\n- Functions for retrieving available \n  [IAU](https://www.ta3.sk/IAUC22DB/MDC2007/Roje/roje_lista.php) registered meteor\n  showers.\n\n## Requirements\n\n- Python 3.7.1+, 3.8, 3.9 or 3.10\n\n## Installation\n\nYou can install `gmn-python-api` via [pip](https://pip.pypa.io/) from \n[PyPI](https://pypi.org/project/gmn-python-api/):\n\n```sh\npip install gmn-python-api\n```\n\nOr install the latest development code, through \n[TestPyPI](https://test.pypi.org/project/gmn-python-api/) or directly from \n[GitHub](https://github.com/rickybassom/gmn-python-api) via \n[pip](https://pip.pypa.io/):\n\n```sh\npip install -i https://test.pypi.org/simple/ --extra-index-url https://pypi.org/simple gmn-python-api==<version>\n```\n\nOr\n\n```sh\npip install git+https://github.com/rickybassom/gmn-python-api\n```\n\nRefer to the [Troubleshooting] guide if you encounter any issues.\n\n## Usage\n\nSimple meteor analysis example:\n\n```python\nfrom gmn_python_api import data_directory as dd\nfrom gmn_python_api import meteor_trajectory_reader\n\n# Analyse recorded meteor data for the 24th of July 2019\ntraj_file_content = dd.get_daily_file_content_by_date("2019-07-24")\n\n# Read data as a Pandas DataFrame\ntraj_df = meteor_trajectory_reader.read_csv(traj_file_content)\n\nprint(f"{traj_df[\'Vgeo (km/s)\'].max()} km/s was the fastest geostationary velocity")\n# Output: 65.38499 km/s was the fastest geostationary velocity\n\nprint(f"{traj_df.loc[traj_df[\'IAU (code)\'] == \'PER\'].shape[0]} Perseid meteors")\n# Output: 8 Perseid meteors\n\nprint(\n  f"Station #{traj_df[\'Num (stat)\'].mode().values[0]} recorded the most meteors")\n# Output: Station #2 recorded the most meteors\n```\n\nPlease see the [Usage](https://gmn-python-api.readthedocs.io/en/latest/usage.html) and \n[API Reference](https://gmn-python-api.readthedocs.io/en/latest/autoapi/gmn_python_api/index.html)\nsections for more details.\n\n## Contributing\nContributions are very welcome. To learn more, see the \n[Contributing guide].\n\n## License\n\nDistributed under the terms of the [MIT](https://opensource.org/licenses/MIT) license,\n`gmn-python-api` is free and open source software.\n\n<!-- Links -->\n[Troubleshooting]: ./TROUBLESHOOTING.md\n[Contributing guide]: ./CONTRIBUTING.md\n',
     'author': 'Ricky Bassom',
     'author_email': 'rickybas12@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/rickybassom/gmn-python-api',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `gmn-python-api-0.0.8/PKG-INFO` & `gmn-python-api-0.0.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 Metadata-Version: 2.1
 Name: gmn-python-api
-Version: 0.0.8
+Version: 0.0.9
 Summary: GMN Python API
 Home-page: https://github.com/rickybassom/gmn-python-api
 License: MIT
 Author: Ricky Bassom
 Author-email: rickybas12@gmail.com
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: beautifulsoup4 (>=4.10.0,<5.0.0)
 Requires-Dist: click (==8.0.4)
+Requires-Dist: future (>=0.18.3)
 Requires-Dist: numpy (>1.20.3)
 Requires-Dist: pandas (>=1.1.0,<=1.3.5)
 Requires-Dist: requests (>=2.21.0,<3.0.0)
 Requires-Dist: types-requests (>=2.27.8,<3.0.0)
+Requires-Dist: werkzeug (>=2.2.3)
 Project-URL: Changelog, https://github.com/rickybassom/gmn-python-api/releases
 Project-URL: Documentation, https://gmn-python-api.readthedocs.io
 Project-URL: Repository, https://github.com/rickybassom/gmn-python-api
 Description-Content-Type: text/markdown
 
 [![PyPI](https://img.shields.io/pypi/v/gmn-python-api)](https://pypi.org/project/gmn-python-api/)
 [![Status](https://img.shields.io/pypi/status/gmn-python-api)](https://pypi.org/project/gmn-python-api/)
@@ -46,32 +48,26 @@
 
 ![Screenshot of GMN data](docs/screenshot.png)
 
 [Demo on Google Colab](https://colab.research.google.com/gist/rickybassom/74d2c99ebbd612b88861038a5b33e021/gmn_data_analysis_template.ipynb)
 
 ## Features
 
-- Listing available daily and monthly csv trajectory summary files from the 
-  [GMN data directory](https://globalmeteornetwork.org/data/traj_summary_data/).
+- Listing available daily and monthly meteor trajectory files from the 
+  [GMN Data Directory](https://globalmeteornetwork.org/data/traj_summary_data/).
 
-- Downloading specific daily and monthly csv trajectory summary files from the data
-  directory.
+- Downloading specific CSV meteor trajectory data from the GMN Data Directory or GMN 
+  REST API.
 
-- Functions for loading the data directory trajectory summary data into 
-  [Pandas](https://pandas.pydata.org/) DataFrames or [Numpy](https://numpy.org/) arrays.
-
-- Functions for retrieving meteor summary data from the future GMN Data Store using the
-  GMN REST API.
-
-- Functions for loading REST API meteor summary data
-  into [Pandas](https://pandas.pydata.org/) DataFrames or [Numpy](https://numpy.org/)
-  arrays.
+- Functions for loading meteor trajectory data into [Pandas](https://pandas.pydata.org/)
+  DataFrames.
 
 - Functions for retrieving available 
-  [IAU](https://www.ta3.sk/IAUC22DB/MDC2007/Roje/roje_lista.php) registered meteor showers.
+  [IAU](https://www.ta3.sk/IAUC22DB/MDC2007/Roje/roje_lista.php) registered meteor
+  showers.
 
 ## Requirements
 
 - Python 3.7.1+, 3.8, 3.9 or 3.10
 
 ## Installation
 
@@ -101,29 +97,30 @@
 
 ## Usage
 
 Simple meteor analysis example:
 
 ```python
 from gmn_python_api import data_directory as dd
-from gmn_python_api import meteor_summary_reader as reader
+from gmn_python_api import meteor_trajectory_reader
 
 # Analyse recorded meteor data for the 24th of July 2019
-traj_sum_file_content = dd.get_daily_file_content_by_date("2019-07-24")
+traj_file_content = dd.get_daily_file_content_by_date("2019-07-24")
 
 # Read data as a Pandas DataFrame
-traj_sum_df = reader.read_meteor_summary_csv_as_dataframe(traj_sum_file_content)
+traj_df = meteor_trajectory_reader.read_csv(traj_file_content)
 
-print(f"{traj_sum_df['Vgeo (km/s)'].max()} km/s was the fastest geostationary velocity")
+print(f"{traj_df['Vgeo (km/s)'].max()} km/s was the fastest geostationary velocity")
 # Output: 65.38499 km/s was the fastest geostationary velocity
 
-print(f"{traj_sum_df.loc[traj_sum_df['IAU (code)'] == 'PER'].shape[0]} Perseid meteors")
+print(f"{traj_df.loc[traj_df['IAU (code)'] == 'PER'].shape[0]} Perseid meteors")
 # Output: 8 Perseid meteors
 
-print(f"Station #{traj_sum_df['Num (stat)'].mode().values[0]} recorded the most meteors")
+print(
+  f"Station #{traj_df['Num (stat)'].mode().values[0]} recorded the most meteors")
 # Output: Station #2 recorded the most meteors
 ```
 
 Please see the [Usage](https://gmn-python-api.readthedocs.io/en/latest/usage.html) and 
 [API Reference](https://gmn-python-api.readthedocs.io/en/latest/autoapi/gmn_python_api/index.html)
 sections for more details.
```

