# Comparing `tmp/pandasai-0.8.2.tar.gz` & `tmp/pandasai-1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasai-0.8.2.tar", max compression
+gzip compressed data, was "pandasai-1.0a1.tar", max compression
```

## Comparing `pandasai-0.8.2.tar` & `pandasai-1.0a1.tar`

### file list

```diff
@@ -1,40 +1,47 @@
--rw-r--r--   0        0        0     1055 2023-08-05 00:39:25.135716 pandasai-0.8.2/LICENSE
--rw-r--r--   0        0        0     7986 2023-08-05 00:39:25.135716 pandasai-0.8.2/README.md
--rw-r--r--   0        0        0    28832 2023-08-05 00:39:25.143716 pandasai-0.8.2/pandasai/__init__.py
--rw-r--r--   0        0        0      155 2023-08-05 00:39:25.143716 pandasai-0.8.2/pandasai/callbacks/__init__.py
--rw-r--r--   0        0        0      519 2023-08-05 00:39:25.143716 pandasai-0.8.2/pandasai/callbacks/base.py
--rw-r--r--   0        0        0      583 2023-08-05 00:39:25.143716 pandasai-0.8.2/pandasai/callbacks/file.py
--rw-r--r--   0        0        0     1438 2023-08-05 00:39:25.143716 pandasai-0.8.2/pandasai/constants.py
--rw-r--r--   0        0        0     1509 2023-08-05 00:39:25.143716 pandasai-0.8.2/pandasai/exceptions.py
--rw-r--r--   0        0        0      316 2023-08-05 00:39:25.143716 pandasai-0.8.2/pandasai/helpers/__init__.py
--rw-r--r--   0        0        0     3814 2023-08-05 00:39:25.143716 pandasai-0.8.2/pandasai/helpers/_optional.py
--rw-r--r--   0        0        0     6404 2023-08-05 00:39:25.143716 pandasai-0.8.2/pandasai/helpers/anonymizer.py
--rw-r--r--   0        0        0     1742 2023-08-05 00:39:25.143716 pandasai-0.8.2/pandasai/helpers/cache.py
--rw-r--r--   0        0        0      566 2023-08-05 00:39:25.143716 pandasai-0.8.2/pandasai/helpers/from_excel.py
--rw-r--r--   0        0        0     3631 2023-08-05 00:39:25.143716 pandasai-0.8.2/pandasai/helpers/from_google_sheets.py
--rw-r--r--   0        0        0     1493 2023-08-05 00:39:25.143716 pandasai-0.8.2/pandasai/helpers/notebook.py
--rw-r--r--   0        0        0     3070 2023-08-05 00:39:25.143716 pandasai-0.8.2/pandasai/helpers/openai_info.py
--rw-r--r--   0        0        0     2454 2023-08-05 00:39:25.143716 pandasai-0.8.2/pandasai/helpers/save_chart.py
--rw-r--r--   0        0        0     9911 2023-08-05 00:39:25.143716 pandasai-0.8.2/pandasai/helpers/shortcuts.py
--rw-r--r--   0        0        0      423 2023-08-05 00:39:25.143716 pandasai-0.8.2/pandasai/llm/__init__.py
--rw-r--r--   0        0        0     4289 2023-08-05 00:39:25.143716 pandasai-0.8.2/pandasai/llm/azure_openai.py
--rw-r--r--   0        0        0    13023 2023-08-05 00:39:25.143716 pandasai-0.8.2/pandasai/llm/base.py
--rw-r--r--   0        0        0      542 2023-08-05 00:39:25.143716 pandasai-0.8.2/pandasai/llm/fake.py
--rw-r--r--   0        0        0      735 2023-08-05 00:39:25.143716 pandasai-0.8.2/pandasai/llm/falcon.py
--rw-r--r--   0        0        0     4440 2023-08-05 00:39:25.143716 pandasai-0.8.2/pandasai/llm/google_palm.py
--rw-r--r--   0        0        0      585 2023-08-05 00:39:25.143716 pandasai-0.8.2/pandasai/llm/langchain.py
--rw-r--r--   0        0        0     3130 2023-08-05 00:39:25.143716 pandasai-0.8.2/pandasai/llm/openai.py
--rw-r--r--   0        0        0      739 2023-08-05 00:39:25.143716 pandasai-0.8.2/pandasai/llm/starcoder.py
--rw-r--r--   0        0        0      192 2023-08-05 00:39:25.143716 pandasai-0.8.2/pandasai/middlewares/__init__.py
--rw-r--r--   0        0        0      663 2023-08-05 00:39:25.143716 pandasai-0.8.2/pandasai/middlewares/base.py
--rw-r--r--   0        0        0      948 2023-08-05 00:39:25.143716 pandasai-0.8.2/pandasai/middlewares/charts.py
--rw-r--r--   0        0        0      653 2023-08-05 00:39:25.143716 pandasai-0.8.2/pandasai/middlewares/streamlit.py
--rw-r--r--   0        0        0      517 2023-08-05 00:39:25.143716 pandasai-0.8.2/pandasai/prompts/__init__.py
--rw-r--r--   0        0        0     1230 2023-08-05 00:39:25.143716 pandasai-0.8.2/pandasai/prompts/base.py
--rw-r--r--   0        0        0     1578 2023-08-05 00:39:25.143716 pandasai-0.8.2/pandasai/prompts/correct_error_prompt.py
--rw-r--r--   0        0        0     1261 2023-08-05 00:39:25.143716 pandasai-0.8.2/pandasai/prompts/correct_multiples_prompt.py
--rw-r--r--   0        0        0     1380 2023-08-05 00:39:25.143716 pandasai-0.8.2/pandasai/prompts/generate_python_code.py
--rw-r--r--   0        0        0      460 2023-08-05 00:39:25.143716 pandasai-0.8.2/pandasai/prompts/generate_response.py
--rw-r--r--   0        0        0     1204 2023-08-05 00:39:25.143716 pandasai-0.8.2/pandasai/prompts/multiple_dataframes.py
--rw-r--r--   0        0        0     2003 2023-08-05 00:39:25.143716 pandasai-0.8.2/pyproject.toml
--rw-r--r--   0        0        0     9285 1970-01-01 00:00:00.000000 pandasai-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0     1055 2023-04-24 05:55:05.323190 pandasai-1.0a1/LICENSE
+-rw-r--r--   0        0        0     7979 2023-08-06 20:52:26.594387 pandasai-1.0a1/README.md
+-rw-r--r--   0        0        0     9277 2023-08-06 21:01:48.067789 pandasai-1.0a1/pandasai/__init__.py
+-rw-r--r--   0        0        0      155 2023-07-27 13:45:00.314291 pandasai-1.0a1/pandasai/callbacks/__init__.py
+-rw-r--r--   0        0        0      519 2023-07-27 13:51:53.758197 pandasai-1.0a1/pandasai/callbacks/base.py
+-rw-r--r--   0        0        0      583 2023-07-27 13:45:00.314481 pandasai-1.0a1/pandasai/callbacks/file.py
+-rw-r--r--   0        0        0     1427 2023-08-06 20:52:26.598302 pandasai-1.0a1/pandasai/constants.py
+-rw-r--r--   0        0        0     1509 2023-06-13 12:20:24.466401 pandasai-1.0a1/pandasai/exceptions.py
+-rw-r--r--   0        0        0      452 2023-08-06 20:56:45.739540 pandasai-1.0a1/pandasai/helpers/__init__.py
+-rw-r--r--   0        0        0     4743 2023-08-06 20:52:26.599196 pandasai-1.0a1/pandasai/helpers/anonymizer.py
+-rw-r--r--   0        0        0     1868 2023-08-06 20:56:45.722791 pandasai-1.0a1/pandasai/helpers/cache.py
+-rw-r--r--   0        0        0     7343 2023-08-06 20:52:26.599852 pandasai-1.0a1/pandasai/helpers/code_manager.py
+-rw-r--r--   0        0        0     2422 2023-08-06 20:52:26.599927 pandasai-1.0a1/pandasai/helpers/data_sampler.py
+-rw-r--r--   0        0        0     2060 2023-08-06 21:04:57.269102 pandasai-1.0a1/pandasai/helpers/df_config.py
+-rw-r--r--   0        0        0      636 2023-08-06 20:52:26.600060 pandasai-1.0a1/pandasai/helpers/df_info.py
+-rw-r--r--   0        0        0      308 2023-08-06 20:56:45.723349 pandasai-1.0a1/pandasai/helpers/env.py
+-rw-r--r--   0        0        0     3631 2023-07-27 13:45:00.314711 pandasai-1.0a1/pandasai/helpers/from_google_sheets.py
+-rw-r--r--   0        0        0     1949 2023-08-06 21:01:33.014035 pandasai-1.0a1/pandasai/helpers/logger.py
+-rw-r--r--   0        0        0      802 2023-08-06 20:52:26.600208 pandasai-1.0a1/pandasai/helpers/memory.py
+-rw-r--r--   0        0        0     1493 2023-06-12 22:05:45.631276 pandasai-1.0a1/pandasai/helpers/notebook.py
+-rw-r--r--   0        0        0     3070 2023-07-25 21:03:21.621048 pandasai-1.0a1/pandasai/helpers/openai_info.py
+-rw-r--r--   0        0        0     3814 2023-08-06 20:52:26.600288 pandasai-1.0a1/pandasai/helpers/optional.py
+-rw-r--r--   0        0        0     1258 2023-08-06 20:56:45.723829 pandasai-1.0a1/pandasai/helpers/path.py
+-rw-r--r--   0        0        0     2399 2023-08-06 20:52:26.600421 pandasai-1.0a1/pandasai/helpers/save_chart.py
+-rw-r--r--   0        0        0     8239 2023-08-06 20:52:26.600581 pandasai-1.0a1/pandasai/helpers/shortcuts.py
+-rw-r--r--   0        0        0      423 2023-08-06 20:52:26.600808 pandasai-1.0a1/pandasai/llm/__init__.py
+-rw-r--r--   0        0        0     4239 2023-08-06 20:56:45.738510 pandasai-1.0a1/pandasai/llm/azure_openai.py
+-rw-r--r--   0        0        0    12958 2023-08-06 20:52:26.601172 pandasai-1.0a1/pandasai/llm/base.py
+-rw-r--r--   0        0        0      584 2023-08-06 20:52:26.601580 pandasai-1.0a1/pandasai/llm/fake.py
+-rw-r--r--   0        0        0      738 2023-08-06 20:56:45.725151 pandasai-1.0a1/pandasai/llm/falcon.py
+-rw-r--r--   0        0        0     4440 2023-07-25 21:03:21.623986 pandasai-1.0a1/pandasai/llm/google_palm.py
+-rw-r--r--   0        0        0      572 2023-08-06 20:52:26.601941 pandasai-1.0a1/pandasai/llm/langchain.py
+-rw-r--r--   0        0        0     3080 2023-08-06 20:56:45.737336 pandasai-1.0a1/pandasai/llm/openai.py
+-rw-r--r--   0        0        0      742 2023-08-06 20:56:45.725842 pandasai-1.0a1/pandasai/llm/starcoder.py
+-rw-r--r--   0        0        0      178 2023-08-06 20:52:26.602522 pandasai-1.0a1/pandasai/middlewares/__init__.py
+-rw-r--r--   0        0        0      663 2023-06-12 22:05:45.635675 pandasai-1.0a1/pandasai/middlewares/base.py
+-rw-r--r--   0        0        0     1306 2023-08-06 20:52:26.602628 pandasai-1.0a1/pandasai/middlewares/charts.py
+-rw-r--r--   0        0        0      653 2023-06-16 21:58:49.858228 pandasai-1.0a1/pandasai/middlewares/streamlit.py
+-rw-r--r--   0        0        0      224 2023-08-06 20:52:26.602743 pandasai-1.0a1/pandasai/prompts/__init__.py
+-rw-r--r--   0        0        0     1288 2023-08-06 20:52:26.602847 pandasai-1.0a1/pandasai/prompts/base.py
+-rw-r--r--   0        0        0     1582 2023-08-06 20:52:26.602971 pandasai-1.0a1/pandasai/prompts/correct_error_prompt.py
+-rw-r--r--   0        0        0     2675 2023-08-06 20:52:26.603103 pandasai-1.0a1/pandasai/prompts/generate_python_code.py
+-rw-r--r--   0        0        0     8095 2023-08-06 20:52:26.603339 pandasai-1.0a1/pandasai/smart_dataframe/__init__.py
+-rw-r--r--   0        0        0     3382 2023-08-06 20:52:26.603414 pandasai-1.0a1/pandasai/smart_dataframe/abstract_df.py
+-rw-r--r--   0        0        0    14157 2023-08-06 20:52:26.604601 pandasai-1.0a1/pandasai/smart_datalake/__init__.py
+-rw-r--r--   0        0        0     2301 2023-08-06 21:20:49.291578 pandasai-1.0a1/pyproject.toml
+-rw-r--r--   0        0        0    10161 1970-01-01 00:00:00.000000 pandasai-1.0a1/PKG-INFO
```

### Comparing `pandasai-0.8.2/LICENSE` & `pandasai-1.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `pandasai-0.8.2/README.md` & `pandasai-1.0a1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -39,29 +39,29 @@
 
 ### Queries
 
 For example, you can ask PandasAI to find all the rows in a DataFrame where the value of a column is greater than 5, and it will return a DataFrame containing only those rows:
 
 ```python
 import pandas as pd
-from pandasai import PandasAI
+from pandasai import SmartDataframe
 
 # Sample DataFrame
 df = pd.DataFrame({
     "country": ["United States", "United Kingdom", "France", "Germany", "Italy", "Spain", "Canada", "Australia", "Japan", "China"],
     "gdp": [19294482071552, 2891615567872, 2411255037952, 3435817336832, 1745433788416, 1181205135360, 1607402389504, 1490967855104, 4380756541440, 14631844184064],
     "happiness_index": [6.94, 7.16, 6.66, 7.07, 6.38, 6.4, 7.23, 7.22, 5.87, 5.12]
 })
 
 # Instantiate a LLM
-from pandasai.llm.openai import OpenAI
+from pandasai.llm import OpenAI
 llm = OpenAI(api_token="YOUR_API_TOKEN")
 
-pandas_ai = PandasAI(llm)
-pandas_ai(df, prompt='Which are the 5 happiest countries?')
+df = SmartDataframe(df, config={"llm": llm})
+df.chat('Which are the 5 happiest countries?')
 ```
 
 The above code will return the following:
 
 ```
 6            Canada
 7         Australia
@@ -70,45 +70,45 @@
 0     United States
 Name: country, dtype: object
 ```
 
 Of course, you can also ask PandasAI to perform more complex queries. For example, you can ask PandasAI to find the sum of the GDPs of the 2 unhappiest countries:
 
 ```python
-pandas_ai(df, prompt='What is the sum of the GDPs of the 2 unhappiest countries?')
+df.chat('What is the sum of the GDPs of the 2 unhappiest countries?')
 ```
 
 The above code will return the following:
 
 ```
 19012600725504
 ```
 
 ### Charts
 
 You can also ask PandasAI to draw a graph:
 
 ```python
-pandas_ai(
-    df,
+df.chat(
     "Plot the histogram of countries showing for each the gdp, using different colors for each bar",
 )
 ```
 
 ![Chart](images/histogram-chart.png?raw=true)
 
 You can save any charts generated by PandasAI by setting the `save_charts` parameter to `True` in the `PandasAI` constructor. For example, `PandasAI(llm, save_charts=True)`. Charts are saved in `./pandasai/exports/charts` .
 
 ### Multiple DataFrames
 
 Additionally, you can also pass in multiple dataframes to PandasAI and ask questions relating them.
 
 ```python
 import pandas as pd
-from pandasai import PandasAI
+from pandasai import SmartDatalake
+from pandasai.llm import OpenAI
 
 employees_data = {
     'EmployeeID': [1, 2, 3, 4, 5],
     'Name': ['John', 'Emma', 'Liam', 'Olivia', 'William'],
     'Department': ['HR', 'Sales', 'IT', 'Marketing', 'Finance']
 }
 
@@ -118,16 +118,16 @@
 }
 
 employees_df = pd.DataFrame(employees_data)
 salaries_df = pd.DataFrame(salaries_data)
 
 
 llm = OpenAI()
-pandas_ai = PandasAI(llm)
-pandas_ai([employees_df, salaries_df], "Who gets paid the most?")
+dl = SmartDatalake([employees_df, salaries_df], config={"llm": llm})
+dl.chat("Who gets paid the most?")
 ```
 
 The above code will return the following:
 
 ```
 Oh, Olivia gets paid the most.
 ```
@@ -136,24 +136,24 @@
 
 ### ⚡️ Shortcuts
 
 PandasAI also provides a number of shortcuts (beta) to make it easier to ask questions to your data. For example, you can ask PandasAI to `clean_data`, `impute_missing_values`, `generate_features`, `plot_histogram`, and many many more.
 
 ```python
 # Clean data
-pandas_ai.clean_data(df)
+df.clean_data()
 
 # Impute missing values
-pandas_ai.impute_missing_values(df)
+df.impute_missing_values()
 
 # Generate features
-pandas_ai.generate_features(df)
+df.generate_features()
 
 # Plot histogram
-pandas_ai.plot_histogram(df, column="gdp")
+df.plot_histogram(column="gdp")
 ```
 
 Learn more about the shortcuts [here](https://pandas-ai.readthedocs.io/en/latest/shortcuts/).
 
 ## 🔒 Privacy & Security
 
 In order to generate the Python code to run, we take the dataframe head, we randomize it (using random generation for sensitive data and shuffling for non-sensitive data) and send just the head.
```

### Comparing `pandasai-0.8.2/pandasai/callbacks/base.py` & `pandasai-1.0a1/pandasai/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.8.2/pandasai/callbacks/file.py` & `pandasai-1.0a1/pandasai/callbacks/file.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.8.2/pandasai/constants.py` & `pandasai-1.0a1/pandasai/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Constants used in the pandasai package.
+
 It includes Start & End Code tags, Whitelisted Python Packages and
 While List Builtin Methods.
-"""
 
+"""
 START_CODE_TAG = "<startCode>"
 END_CODE_TAG = "<endCode>"
 
 # List of Python builtin libraries that are added to the environment by default.
 WHITELISTED_BUILTINS = [
     "abs",
     "all",
@@ -47,15 +48,14 @@
     "map",
     "max",
     "memoryview",
     "min",
     "next",
     "object",
     "oct",
-    "open",
     "ord",
     "pow",
     "print",
     "property",
     "range",
     "repr",
     "reversed",
```

### Comparing `pandasai-0.8.2/pandasai/exceptions.py` & `pandasai-1.0a1/pandasai/exceptions.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.8.2/pandasai/helpers/_optional.py` & `pandasai-1.0a1/pandasai/helpers/optional.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.8.2/pandasai/helpers/cache.py` & `pandasai-1.0a1/pandasai/helpers/cache.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 """Cache module for caching queries."""
 import glob
 import os
 import shelve
-from pathlib import Path
+from .path import find_project_root
 
 
 class Cache:
     """Cache class for caching queries. It is used to cache queries
     to save time and money.
 
     Args:
         filename (str): filename to store the cache.
     """
 
     def __init__(self, filename="cache"):
         # define cache directory and create directory if it does not exist
-        cache_dir = os.path.join(Path.cwd(), "cache")
+        try:
+            cache_dir = os.path.join((find_project_root()), "cache")
+        except ValueError:
+            cache_dir = os.path.join(os.getcwd(), "cache")
+
         os.makedirs(cache_dir, mode=0o777, exist_ok=True)
 
         self.filepath = os.path.join(cache_dir, filename)
         self.cache = shelve.open(self.filepath)
 
     def set(self, key: str, value: str) -> None:
         """Set a key value pair in the cache.
```

### Comparing `pandasai-0.8.2/pandasai/helpers/from_google_sheets.py` & `pandasai-1.0a1/pandasai/helpers/from_google_sheets.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.8.2/pandasai/helpers/notebook.py` & `pandasai-1.0a1/pandasai/helpers/notebook.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.8.2/pandasai/helpers/openai_info.py` & `pandasai-1.0a1/pandasai/helpers/openai_info.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.8.2/pandasai/helpers/save_chart.py` & `pandasai-1.0a1/pandasai/helpers/save_chart.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,27 +21,26 @@
             and value.func.value.id == "plt"
         )
     )
 
 
 def add_save_chart(
     code: str,
+    logger: logging.Logger,
     folder_name: str,
     save_charts_path: str = None,
-    print_save_dir: bool = True,
 ) -> str:
     """
     Add line to code that save charts to a file, if plt.show() is called.
 
     Args:
         code (str): Code to add line to.
+        logger (logging.Logger): Logger to use.
         folder_name (str): Name of folder to save charts to.
         save_charts_path (str): User Defined Path to save Charts
-        print_save_dir (bool): Print the save directory to the console.
-            Defaults to True.
 
     Returns:
         str: Code with line added.
 
     """
 
     if save_charts_path is not None:
@@ -75,13 +74,13 @@
                 counter += 1
 
             chart_save_path = os.path.join(chart_save_dir, f"{filename}.png")
             new_body.append(ast.parse(f"plt.savefig(r'{chart_save_path}')"))
         new_body.append(node)
 
     chart_save_msg = f"Charts saving to: {chart_save_dir}"
-    if print_save_dir:
+    if not logger.verbose:
         print(chart_save_msg)
     logging.info(chart_save_msg)
 
     new_tree = ast.Module(body=new_body)
     return astor.to_source(new_tree, pretty_source=lambda x: "".join(x)).strip()
```

### Comparing `pandasai-0.8.2/pandasai/llm/azure_openai.py` & `pandasai-1.0a1/pandasai/llm/azure_openai.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 """
 
 import os
 from typing import Any, Dict, Optional
 
 import openai
-from dotenv import load_dotenv
+from ..helpers import load_dotenv
 
 from ..exceptions import APIKeyNotFoundError, UnsupportedOpenAIModelError
 from .base import BaseOpenAI
 
 load_dotenv()
 
 
@@ -98,31 +98,31 @@
         """Get the default parameters for calling OpenAI API
 
         Returns: A dict of Default Params
 
         """
         return {**super()._default_params, "engine": self.engine}
 
-    def call(self, instruction: str, value: str, suffix: str = "") -> str:
+    def call(self, instruction: str, suffix: str = "") -> str:
         """
         Call the Azure OpenAI LLM.
 
         Args:
             instruction (str): Instruction to pass
             value (str): Value to pass
             suffix(str): Suffix to pass
 
         Returns:
             str: Response
         """
-        self.last_prompt = str(instruction) + str(value)
+        self.last_prompt = instruction.to_string() + suffix
 
         if self.is_chat_model:
-            response = self.chat_completion(str(instruction) + str(value) + suffix)
+            response = self.chat_completion(self.last_prompt)
         else:
-            response = self.completion(str(instruction) + str(value) + suffix)
+            response = self.completion(self.last_prompt)
 
         return response
 
     @property
     def type(self) -> str:
         return "azure-openai"
```

### Comparing `pandasai-0.8.2/pandasai/llm/base.py` & `pandasai-1.0a1/pandasai/llm/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 from ..constants import END_CODE_TAG, START_CODE_TAG
 from ..exceptions import (
     APIKeyNotFoundError,
     MethodNotImplementedError,
     NoCodeFoundError,
 )
-from ..helpers._optional import import_dependency
+from ..helpers.optional import import_dependency
 from ..helpers.openai_info import openai_callback_var
 from ..prompts.base import Prompt
 
 
 class LLM:
     """Base class to implement a new LLM."""
 
@@ -108,14 +108,15 @@
         Returns:
             str: Extracted code from the response
         """
         code = response
         match = re.search(
             rf"{START_CODE_TAG}(.*)({END_CODE_TAG}"
             rf"|{END_CODE_TAG.replace('<', '</')}"
+            # fix to make it work with ERNIE bot (#389)
             rf"|{START_CODE_TAG.replace('<', '</')})",
             code,
             re.DOTALL,
         )
         if match:
             code = match.group(1).strip()
         if len(code.split(separator)) > 1:
@@ -123,47 +124,47 @@
         code = self._polish_code(code)
         if not self._is_python_code(code):
             raise NoCodeFoundError("No code found in the response")
 
         return code
 
     @abstractmethod
-    def call(self, instruction: Prompt, value: str, suffix: str = "") -> str:
+    def call(self, instruction: Prompt, suffix: str = "") -> str:
         """
         Execute the LLM with given prompt.
 
         Args:
             instruction (Prompt): Prompt
-            value (str): Value
             suffix (str, optional): Suffix. Defaults to "".
 
         Raises:
             MethodNotImplementedError: Call method has not been implemented
         """
         raise MethodNotImplementedError("Call method has not been implemented")
 
-    def generate_code(self, instruction: Prompt, prompt: str) -> str:
+    def generate_code(self, instruction: Prompt) -> str:
         """
         Generate the code based on the instruction and the given prompt.
 
         Returns:
             str: Code
         """
-        return self._extract_code(self.call(instruction, prompt, suffix="\n\nCode:\n"))
+        code = self.call(instruction, suffix="")
+        return self._extract_code(code)
 
 
 class BaseOpenAI(LLM, ABC):
     """Base class to implement a new OpenAI LLM
     LLM base class, this class is extended to be used with OpenAI API.
 
     """
 
     api_token: str
     temperature: float = 0
-    max_tokens: int = 512
+    max_tokens: int = 1000
     top_p: float = 1
     frequency_penalty: float = 0
     presence_penalty: float = 0.6
     stop: Optional[str] = None
     # support explicit proxy for OpenAI
     openai_proxy: Optional[str] = None
 
@@ -321,39 +322,39 @@
 
         response = requests.post(
             self._api_url, headers=headers, json=payload, timeout=60
         )
 
         return response.json()[0]["generated_text"]
 
-    def call(self, instruction: Prompt, value: str, suffix: str = "") -> str:
+    def call(self, instruction: Prompt, suffix: str = "") -> str:
         """
         A call method of HuggingFaceLLM class.
         Args:
             instruction (object): A prompt object
             value (str):
             suffix (str):
 
         Returns (str): A string response
 
         """
 
-        prompt = str(instruction)
-        payload = prompt + value + suffix
+        prompt = instruction.to_string()
+        payload = prompt + suffix
 
         # sometimes the API doesn't return a valid response, so we retry passing the
         # output generated from the previous call as the input
         for _i in range(self._max_retries):
             response = self.query({"inputs": payload})
             payload = response
             if response.count("<endCode>") >= 2:
                 break
 
         # replace instruction + value from the inputs to avoid showing it in the output
-        output = response.replace(prompt + value + suffix, "")
+        output = response.replace(prompt + suffix, "")
         ans = ""
         for line in output.split("\n"):
             if line.find("utput:") != -1:
                 break
             if ans == "":
                 ans = ans + line
             else:
@@ -453,22 +454,21 @@
             prompt (str): Prompt
 
         Returns:
             str: LLM response
         """
         raise MethodNotImplementedError("method has not been implemented")
 
-    def call(self, instruction: Prompt, value: str, suffix: str = "") -> str:
+    def call(self, instruction: Prompt, suffix: str = "") -> str:
         """
         Call the Google LLM.
 
         Args:
             instruction (object): Instruction to pass
             value (str): Value to pass
             suffix (str): Suffix to pass
 
         Returns:
             str: Response
         """
-        self.last_prompt = str(instruction) + value
-        prompt = str(instruction) + value + suffix
-        return self._generate_text(prompt)
+        self.last_prompt = instruction.to_string() + suffix
+        return self._generate_text(self.last_prompt)
```

### Comparing `pandasai-0.8.2/pandasai/llm/fake.py` & `pandasai-1.0a1/pandasai/llm/fake.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,20 +5,21 @@
 from ..prompts.base import Prompt
 from .base import LLM
 
 
 class FakeLLM(LLM):
     """Fake LLM"""
 
-    _output: str = 'print("Hello world")'
+    _output: str = """def analyze_data(dfs):
+    return { 'type': 'text', 'value': "Hello World" }"""
 
     def __init__(self, output: Optional[str] = None):
         if output is not None:
             self._output = output
 
-    def call(self, instruction: Prompt, value: str, suffix: str = "") -> str:
-        self.last_prompt = str(instruction) + str(value) + suffix
+    def call(self, instruction: Prompt, suffix: str = "") -> str:
+        self.last_prompt = instruction.to_string() + suffix
         return self._output
 
     @property
     def type(self) -> str:
         return "fake"
```

### Comparing `pandasai-0.8.2/pandasai/llm/falcon.py` & `pandasai-1.0a1/pandasai/llm/falcon.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Example:
     Use below example to call Falcon Model
 
     >>> from pandasai.llm.falcon import Falcon
 """
 
 
-from dotenv import load_dotenv
+from ..helpers import load_dotenv
 from .base import HuggingFaceLLM
 
 load_dotenv()
 
 
 class Falcon(HuggingFaceLLM):
```

### Comparing `pandasai-0.8.2/pandasai/llm/google_palm.py` & `pandasai-1.0a1/pandasai/llm/google_palm.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.8.2/pandasai/llm/langchain.py` & `pandasai-1.0a1/pandasai/llm/langchain.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,14 @@
     """
 
     _langchain_llm = None
 
     def __init__(self, langchain_llm):
         self._langchain_llm = langchain_llm
 
-    def call(self, instruction: Prompt, value: str, suffix: str = "") -> str:
-        prompt = str(instruction) + value + suffix
+    def call(self, instruction: Prompt, suffix: str = "") -> str:
+        prompt = instruction.to_string() + suffix
         return self._langchain_llm.predict(prompt)
 
     @property
     def type(self) -> str:
         return "langchain_" + self._langchain_llm._llm_type
```

### Comparing `pandasai-0.8.2/pandasai/llm/openai.py` & `pandasai-1.0a1/pandasai/llm/openai.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     >>> from pandasai.llm.openai import OpenAI
 """
 
 import os
 from typing import Any, Dict, Optional
 
 import openai
-from dotenv import load_dotenv
+from ..helpers import load_dotenv
 
 from ..exceptions import APIKeyNotFoundError, UnsupportedOpenAIModelError
 from ..prompts.base import Prompt
 from .base import BaseOpenAI
 
 load_dotenv()
 
@@ -75,35 +75,35 @@
     def _default_params(self) -> Dict[str, Any]:
         """Get the default parameters for calling OpenAI API"""
         return {
             **super()._default_params,
             "model": self.model,
         }
 
-    def call(self, instruction: Prompt, value: str, suffix: str = "") -> str:
+    def call(self, instruction: Prompt, suffix: str = "") -> str:
         """
         Call the OpenAI LLM.
 
         Args:
             instruction (Prompt): Instruction to pass
             value (str): Value to pass
             suffix (str): Suffix to pass
 
         Raises:
             UnsupportedOpenAIModelError: Unsupported model
 
         Returns:
             str: Response
         """
-        self.last_prompt = str(instruction) + str(value)
+        self.last_prompt = instruction.to_string() + suffix
 
         if self.model in self._supported_completion_models:
-            response = self.completion(str(instruction) + str(value) + suffix)
+            response = self.completion(self.last_prompt)
         elif self.model in self._supported_chat_models:
-            response = self.chat_completion(str(instruction) + str(value) + suffix)
+            response = self.chat_completion(self.last_prompt)
         else:
             raise UnsupportedOpenAIModelError("Unsupported model")
 
         return response
 
     @property
     def type(self) -> str:
```

### Comparing `pandasai-0.8.2/pandasai/llm/starcoder.py` & `pandasai-1.0a1/pandasai/llm/starcoder.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Example:
     Use below example to call Starcoder Model
 
     >>> from pandasai.llm.starcoder import Starcoder
 """
 
 
-from dotenv import load_dotenv
+from ..helpers import load_dotenv
 from .base import HuggingFaceLLM
 
 load_dotenv()
 
 
 class Starcoder(HuggingFaceLLM):
```

### Comparing `pandasai-0.8.2/pandasai/middlewares/base.py` & `pandasai-1.0a1/pandasai/middlewares/base.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.8.2/pandasai/middlewares/charts.py` & `pandasai-1.0a1/pandasai/middlewares/charts.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 Charts Middleware class
 
 Middleware to handle the charts in PandasAI.
 """
 
 from pandasai.middlewares.base import Middleware
 import sys
+import ast
 
 
 class ChartsMiddleware(Middleware):
     """Charts Middleware class"""
 
     def _is_running_in_console(self) -> bool:
         """
@@ -25,14 +26,22 @@
         """
         Run the middleware to remove issues with displaying charts in PandasAI.
 
         Returns:
             str: Modified code
         """
 
-        if "plt.show()" in code:
-            if "plt.close('all')" not in code:
-                code = code.replace("plt.show()", "plt.show()\nplt.close('all')")
+        tree = ast.parse(code)
 
-            if not self._is_running_in_console():
-                code = code.replace("plt.show()", "plt.show(block=False)")
+        for node in ast.walk(tree):
+            if isinstance(node, ast.Expr) and isinstance(node.value, ast.Call):
+                call = node.value
+                if isinstance(call.func, ast.Attribute) and call.func.attr == "show":
+                    if "plt.close('all')" not in code:
+                        code = code.replace(
+                            "plt.show()", "plt.show()\nplt.close('all')"
+                        )
+
+                    if not self._is_running_in_console():
+                        code = code.replace("plt.show()", "plt.show(block=False)")
+                    break
         return code
```

### Comparing `pandasai-0.8.2/pandasai/middlewares/streamlit.py` & `pandasai-1.0a1/pandasai/middlewares/streamlit.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.8.2/pandasai/prompts/base.py` & `pandasai-1.0a1/pandasai/prompts/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,12 +31,15 @@
             for var in vars:
                 if var[0] == "_" and var not in self._args:
                     self._args[var] = var
 
     def override_var(self, var, value):
         self._args[var] = value
 
-    def __str__(self):
+    def to_string(self):
         if self.text is None:
             raise MethodNotImplementedError
 
         return self.text.format(**self._args)
+
+    def __str__(self):
+        return self.to_string()
```

### Comparing `pandasai-0.8.2/pandasai/prompts/correct_error_prompt.py` & `pandasai-1.0a1/pandasai/prompts/correct_error_prompt.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
     text: str = """
 You are provided with a pandas dataframe (df) with {num_rows} rows and {num_columns} columns.
 This is the metadata of the dataframe:
 {df_head}.
 
 The user asked the following question:
-{question}
+{conversation}
 
 You generated this python code:
 {code}
 
 It fails with the following error:
 {error_returned}
```

### Comparing `pandasai-0.8.2/pyproject.toml` & `pandasai-1.0a1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,59 +1,67 @@
 [tool.poetry]
 name = "pandasai"
-version = "0.8.2"
+version = "1.0a1"
 description = "Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational."
 authors = ["Gabriele Venturi"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pandasai"}]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.9.7 || >3.9.7,<4.0"
 python-dotenv = "^1.0.0"
 pandas = "1.5.3"
 astor = "^0.8.1"
 openai = "^0.27.5"
 ipython = "^8.13.1"
 matplotlib = "^3.7.1"
-google-generativeai = { version = "^0.1.0rc2", optional = true }
-google-cloud-aiplatform = { version = "^1.26.1", optional = true }
-langchain = { version = "^0.0.199", optional = true}
+pydantic = "^1"
+google-generativeai = {version = "^0.1.0rc2", optional = true}
+google-cloud-aiplatform = {version = "^1.26.1", optional = true}
+langchain = {version = "^0.0.199", optional = true}
+polars = {version = "^0.10.0", optional = true}
+statsmodels = {version = "^0.14.0", optional = true}
+scikit-learn = {version = "^1.2.2", optional = true}
+seaborn = {version = "^0.12.2", optional = true}
+plotly = {version = "^5.15.0", optional = true}
+kaleido = {version = "0.2.0", optional = true}
+ggplot = {version = "^0.11.5", optional = true}
+numpy = {version = "^1.17", optional = true}
+scipy = {version = "^1.9.0", optional = true}
+streamlit = {version = "^1.23.1", optional = true}
 beautifulsoup4 = { version = "^4.12.2", optional = true }
+openpyxl = { version = "^3.0.7", optional = true }
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 pre-commit = "^3.2.2"
 ruff = "^0.0.220"
 pytest = "^7.3.1"
 pytest-mock = "^3.10.0"
 pytest-env = "^0.8.1"
 click = "^8.1.3"
 coverage = "^7.2.7"
 
-
 [tool.poetry.group.extras.dependencies]
 google-cloud-aiplatform = "^1.26.1"
 
 [tool.poetry.extras]
-google = ["google-generativeai"]
-tests = ["numpy", "seaborn"]
+google-ai = ["google-generativeai", "google-cloud-aiplatform"]
+google-sheets = ["beautifulsoup4"]
+excel = ["openpyxl"]
+polars = ["polars"]
 langchain = ["langchain"]
-bs4 = ["beautifulsoup4"]
-google-cloud = ["google-cloud-aiplatform"]
-
-[tool.poetry.group.whitelist.dependencies]
-statsmodels = {version = "^0.14.0", optional = true}
-scikit-learn = {version = "^1.2.2", optional = true}
-seaborn = {version = "^0.12.2", optional = true}
-plotly = {version = "^5.14.1", optional = true}
-ggplot = {version = "^0.11.5", optional = true}
-numpy = {version = "^1.17", optional = true}
-scipy = {version = "^1.9.0", optional = true}
-streamlit = { version = "^1.23.1", optional = true }
+numpy = ["numpy"]
+ggplot = ["ggplot"]
+seaborn = ["seaborn"]
+plotly = ["plotly", "kaleido"]
+statsmodels = ["statsmodels"]
+scikit-learn = ["scikit-learn"]
+streamlit = ["streamlit"]
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "1.4.0"
 mkdocstrings-python = "0.7.1"
 markdown-include = "^0.6.0"
 
 [tool.poetry.scripts]
```

### Comparing `pandasai-0.8.2/PKG-INFO` & `pandasai-1.0a1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,53 @@
 Metadata-Version: 2.1
 Name: pandasai
-Version: 0.8.2
+Version: 1.0a1
 Summary: Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational.
 License: MIT
 Author: Gabriele Venturi
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Provides-Extra: bs4
-Provides-Extra: google
-Provides-Extra: google-cloud
+Provides-Extra: excel
+Provides-Extra: ggplot
+Provides-Extra: google-ai
+Provides-Extra: google-sheets
 Provides-Extra: langchain
-Provides-Extra: tests
+Provides-Extra: numpy
+Provides-Extra: plotly
+Provides-Extra: polars
+Provides-Extra: scikit-learn
+Provides-Extra: seaborn
+Provides-Extra: statsmodels
+Provides-Extra: streamlit
 Requires-Dist: astor (>=0.8.1,<0.9.0)
-Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0) ; extra == "bs4"
-Requires-Dist: google-cloud-aiplatform (>=1.26.1,<2.0.0) ; extra == "google-cloud"
-Requires-Dist: google-generativeai (>=0.1.0rc2,<0.2.0) ; extra == "google"
+Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0) ; extra == "google-sheets"
+Requires-Dist: ggplot (>=0.11.5,<0.12.0) ; extra == "ggplot"
+Requires-Dist: google-cloud-aiplatform (>=1.26.1,<2.0.0) ; extra == "google-ai"
+Requires-Dist: google-generativeai (>=0.1.0rc2,<0.2.0) ; extra == "google-ai"
 Requires-Dist: ipython (>=8.13.1,<9.0.0)
+Requires-Dist: kaleido (==0.2.0) ; extra == "plotly"
 Requires-Dist: langchain (>=0.0.199,<0.0.200) ; extra == "langchain"
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
+Requires-Dist: numpy (>=1.17,<2.0) ; extra == "numpy"
 Requires-Dist: openai (>=0.27.5,<0.28.0)
+Requires-Dist: openpyxl (>=3.0.7,<4.0.0) ; extra == "excel"
 Requires-Dist: pandas (==1.5.3)
+Requires-Dist: plotly (>=5.15.0,<6.0.0) ; extra == "plotly"
+Requires-Dist: polars (>=0.10.0,<0.11.0) ; extra == "polars"
+Requires-Dist: pydantic (>=1,<2)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
+Requires-Dist: scikit-learn (>=1.2.2,<2.0.0) ; extra == "scikit-learn"
+Requires-Dist: scipy (>=1.9.0,<2.0.0)
+Requires-Dist: seaborn (>=0.12.2,<0.13.0) ; extra == "seaborn"
+Requires-Dist: statsmodels (>=0.14.0,<0.15.0) ; extra == "statsmodels"
+Requires-Dist: streamlit (>=1.23.1,<2.0.0) ; extra == "streamlit"
 Description-Content-Type: text/markdown
 
 # PandasAI 🐼
 
 [![Release](https://img.shields.io/pypi/v/pandasai?label=Release&style=flat-square)](https://pypi.org/project/pandasai/)
 [![CI](https://github.com/gventuri/pandas-ai/actions/workflows/ci.yml/badge.svg)](https://github.com/gventuri/pandas-ai/actions/workflows/ci.yml/badge.svg)
 [![CD](https://github.com/gventuri/pandas-ai/actions/workflows/cd.yml/badge.svg)](https://github.com/gventuri/pandas-ai/actions/workflows/cd.yml/badge.svg)
@@ -68,29 +87,29 @@
 
 ### Queries
 
 For example, you can ask PandasAI to find all the rows in a DataFrame where the value of a column is greater than 5, and it will return a DataFrame containing only those rows:
 
 ```python
 import pandas as pd
-from pandasai import PandasAI
+from pandasai import SmartDataframe
 
 # Sample DataFrame
 df = pd.DataFrame({
     "country": ["United States", "United Kingdom", "France", "Germany", "Italy", "Spain", "Canada", "Australia", "Japan", "China"],
     "gdp": [19294482071552, 2891615567872, 2411255037952, 3435817336832, 1745433788416, 1181205135360, 1607402389504, 1490967855104, 4380756541440, 14631844184064],
     "happiness_index": [6.94, 7.16, 6.66, 7.07, 6.38, 6.4, 7.23, 7.22, 5.87, 5.12]
 })
 
 # Instantiate a LLM
-from pandasai.llm.openai import OpenAI
+from pandasai.llm import OpenAI
 llm = OpenAI(api_token="YOUR_API_TOKEN")
 
-pandas_ai = PandasAI(llm)
-pandas_ai(df, prompt='Which are the 5 happiest countries?')
+df = SmartDataframe(df, config={"llm": llm})
+df.chat('Which are the 5 happiest countries?')
 ```
 
 The above code will return the following:
 
 ```
 6            Canada
 7         Australia
@@ -99,45 +118,45 @@
 0     United States
 Name: country, dtype: object
 ```
 
 Of course, you can also ask PandasAI to perform more complex queries. For example, you can ask PandasAI to find the sum of the GDPs of the 2 unhappiest countries:
 
 ```python
-pandas_ai(df, prompt='What is the sum of the GDPs of the 2 unhappiest countries?')
+df.chat('What is the sum of the GDPs of the 2 unhappiest countries?')
 ```
 
 The above code will return the following:
 
 ```
 19012600725504
 ```
 
 ### Charts
 
 You can also ask PandasAI to draw a graph:
 
 ```python
-pandas_ai(
-    df,
+df.chat(
     "Plot the histogram of countries showing for each the gdp, using different colors for each bar",
 )
 ```
 
 ![Chart](images/histogram-chart.png?raw=true)
 
 You can save any charts generated by PandasAI by setting the `save_charts` parameter to `True` in the `PandasAI` constructor. For example, `PandasAI(llm, save_charts=True)`. Charts are saved in `./pandasai/exports/charts` .
 
 ### Multiple DataFrames
 
 Additionally, you can also pass in multiple dataframes to PandasAI and ask questions relating them.
 
 ```python
 import pandas as pd
-from pandasai import PandasAI
+from pandasai import SmartDatalake
+from pandasai.llm import OpenAI
 
 employees_data = {
     'EmployeeID': [1, 2, 3, 4, 5],
     'Name': ['John', 'Emma', 'Liam', 'Olivia', 'William'],
     'Department': ['HR', 'Sales', 'IT', 'Marketing', 'Finance']
 }
 
@@ -147,16 +166,16 @@
 }
 
 employees_df = pd.DataFrame(employees_data)
 salaries_df = pd.DataFrame(salaries_data)
 
 
 llm = OpenAI()
-pandas_ai = PandasAI(llm)
-pandas_ai([employees_df, salaries_df], "Who gets paid the most?")
+dl = SmartDatalake([employees_df, salaries_df], config={"llm": llm})
+dl.chat("Who gets paid the most?")
 ```
 
 The above code will return the following:
 
 ```
 Oh, Olivia gets paid the most.
 ```
@@ -165,24 +184,24 @@
 
 ### ⚡️ Shortcuts
 
 PandasAI also provides a number of shortcuts (beta) to make it easier to ask questions to your data. For example, you can ask PandasAI to `clean_data`, `impute_missing_values`, `generate_features`, `plot_histogram`, and many many more.
 
 ```python
 # Clean data
-pandas_ai.clean_data(df)
+df.clean_data()
 
 # Impute missing values
-pandas_ai.impute_missing_values(df)
+df.impute_missing_values()
 
 # Generate features
-pandas_ai.generate_features(df)
+df.generate_features()
 
 # Plot histogram
-pandas_ai.plot_histogram(df, column="gdp")
+df.plot_histogram(column="gdp")
 ```
 
 Learn more about the shortcuts [here](https://pandas-ai.readthedocs.io/en/latest/shortcuts/).
 
 ## 🔒 Privacy & Security
 
 In order to generate the Python code to run, we take the dataframe head, we randomize it (using random generation for sensitive data and shuffling for non-sensitive data) and send just the head.
```

