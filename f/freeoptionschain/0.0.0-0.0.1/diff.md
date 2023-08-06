# Comparing `tmp/freeoptionschain-0.0.0.tar.gz` & `tmp/freeoptionschain-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freeoptionschain-0.0.0.tar", last modified: Fri Aug  4 16:37:02 2023, max compression
+gzip compressed data, was "freeoptionschain-0.0.1.tar", last modified: Sun Aug  6 07:19:59 2023, max compression
```

## Comparing `freeoptionschain-0.0.0.tar` & `freeoptionschain-0.0.1.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-08-04 16:37:02.301076 freeoptionschain-0.0.0/
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-08-04 16:37:02.301076 freeoptionschain-0.0.0/FOC/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      239 2023-08-04 16:14:25.000000 freeoptionschain-0.0.0/FOC/__init__.py
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)   880472 2023-08-04 02:17:15.000000 freeoptionschain-0.0.0/FOC/db.cpython-38-x86_64-linux-gnu.so
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1268 2023-08-03 02:46:03.000000 freeoptionschain-0.0.0/FOC/defined.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    12423 2023-08-04 16:08:05.000000 freeoptionschain-0.0.0/FOC/main.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1037 2023-08-04 04:40:58.000000 freeoptionschain-0.0.0/LICENSE
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     5032 2023-08-04 16:37:02.301076 freeoptionschain-0.0.0/PKG-INFO
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     4158 2023-08-04 09:03:59.000000 freeoptionschain-0.0.0/README.md
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-08-04 16:37:02.301076 freeoptionschain-0.0.0/freeoptionschain.egg-info/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     5032 2023-08-04 16:37:02.000000 freeoptionschain-0.0.0/freeoptionschain.egg-info/PKG-INFO
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      331 2023-08-04 16:37:02.000000 freeoptionschain-0.0.0/freeoptionschain.egg-info/SOURCES.txt
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        1 2023-08-04 16:37:02.000000 freeoptionschain-0.0.0/freeoptionschain.egg-info/dependency_links.txt
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)       61 2023-08-04 16:37:02.000000 freeoptionschain-0.0.0/freeoptionschain.egg-info/requires.txt
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        4 2023-08-04 16:37:02.000000 freeoptionschain-0.0.0/freeoptionschain.egg-info/top_level.txt
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      136 2023-08-04 14:43:00.000000 freeoptionschain-0.0.0/pyproject.toml
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      449 2023-08-04 16:37:02.301076 freeoptionschain-0.0.0/setup.cfg
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1274 2023-08-04 16:36:24.000000 freeoptionschain-0.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:19:59.170403 freeoptionschain-0.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:19:59.170403 freeoptionschain-0.0.1/FOC/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-08-06 07:19:50.000000 freeoptionschain-0.0.1/FOC/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   880472 2023-08-06 07:19:50.000000 freeoptionschain-0.0.1/FOC/db.cpython-38-x86_64-linux-gnu.so
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-08-06 07:19:50.000000 freeoptionschain-0.0.1/FOC/defined.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11616 2023-08-06 07:19:50.000000 freeoptionschain-0.0.1/FOC/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-08-06 07:19:50.000000 freeoptionschain-0.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-08-06 07:19:59.170403 freeoptionschain-0.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-08-06 07:19:50.000000 freeoptionschain-0.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:19:59.170403 freeoptionschain-0.0.1/freeoptionschain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-08-06 07:19:59.000000 freeoptionschain-0.0.1/freeoptionschain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-08-06 07:19:59.000000 freeoptionschain-0.0.1/freeoptionschain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 07:19:59.000000 freeoptionschain-0.0.1/freeoptionschain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-06 07:19:59.000000 freeoptionschain-0.0.1/freeoptionschain.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-08-06 07:19:59.000000 freeoptionschain-0.0.1/freeoptionschain.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-08-06 07:19:59.170403 freeoptionschain-0.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-08-06 07:19:52.000000 freeoptionschain-0.0.1/setup.py
```

### Comparing `freeoptionschain-0.0.0/FOC/db.cpython-38-x86_64-linux-gnu.so` & `freeoptionschain-0.0.1/FOC/db.cpython-38-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `freeoptionschain-0.0.0/FOC/defined.py` & `freeoptionschain-0.0.1/FOC/defined.py`

 * *Files identical despite different names*

### Comparing `freeoptionschain-0.0.0/FOC/main.py` & `freeoptionschain-0.0.1/FOC/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -246,23 +246,7 @@
             options_price_data['contract_symbol'] = contract_symbol
             
             if self.dbconn:
                 df_to_save = options_price_data.copy()
                 self.dbconn.insert_data("options_price_data", df_to_save)
             
         return options_price_data
-        
-
-if __name__ == "__main__":
-
-    ref_FOC = FOC()
-    
-    # results = ref_FOC.get_options_chain("AMC","2023-08-11",OptionType.CALLPUT)
-    # results = ref_FOC.get_options_chain("AMC","2023-08-18",OptionType.PUT)
-    # results = ref_FOC.get_options_chain("AMC","2023-08-25",OptionType.CALL)
-    # results = ref_FOC.get_options_chain_greeks("AMC","2023-08-11",OptionType.CALLPUT)
-    # results = ref_FOC.get_options_greeks("AMC---230811C00004000")
-    # results = ref_FOC.get_expiration_dates("AMC")
-    # results = ref_FOC.get_contract_symbol("AMC",'2023-08-11','CALL',4.0)
-    # results = ref_FOC.get_options_data(ref_FOC.get_contract_symbol("AMC",'2023-08-11','CALL',4.0))
-    results = ref_FOC.get_options_price_data(ref_FOC.get_contract_symbol("AMC",'2023-08-11','CALL',4.0))
-    print(results)
```

### Comparing `freeoptionschain-0.0.0/LICENSE` & `freeoptionschain-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `freeoptionschain-0.0.0/PKG-INFO` & `freeoptionschain-0.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: freeoptionschain
-Version: 0.0.0
-Summary: This downloads stock option data and calculates its greeks.
+Version: 0.0.1
+Summary: This library module retrieves stock options data from NASDAQ.
 Home-page: https://github.com/benjamincham/free_options_chain
 Author: Benjamin Cham
 Author-email: benjaminchamwb@gmail.com
 Project-URL: Bug Tracker, https://github.com/benjamincham/free_options_chain/issues
 Project-URL: Changelog, https://github.com/benjamincham/free_options_chain/releases
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Classifier: License :: OSI Approved :: MIT License
@@ -58,26 +58,26 @@
 ``` {.sourceCode .bash}
 pip install freeoptionschain
 ```
 Import
 ------
 
 ``` {.sourceCode .python}
-from FOC import *
+from FOC import FOC
 ```
 Fetch all options expiration dates for a stock
 ---------------------------------
 To fetch the options expiration date for a specific stock for a given  expiration date, you can
 simply use:
 
 ``` {.sourceCode .python}
 #create instance
 ref_FOC = FOC()
 
-# Options Chain of AAPL CALL options for 6 October 2023
+# Fetch options expiration dates for 'AAPL'
 options_chain = ref_FOC.get_expiration_dates("AAPL")
 ```
 Fetch options chain with price
 ---------------------------------
 To fetch the options chain for a specific stock for a given  expiration date, you can
 simply use:
 
@@ -105,16 +105,18 @@
 To fetch single options contract for a specific symbol, you can
 simply use:
 
 ``` {.sourceCode .python}
 #create instance
 ref_FOC = FOC()
 
-# AAPL CALL options with strike $200 for 6 October 2023, with greeks
-options_contract = ref_FOC.get_options_price_data(ref_FOC.get_contract_symbol("AAPL",'2023-10-06','CALL',200.0))
+# get options contract symbol for AAPL CALL options with strike $200 for 6 October 2023
+contract_symbol = ref_FOC.get_contract_symbol("AAPL",'2023-10-06','CALL',200.0)
+#fetch options contract with greeks
+options_contract = ref_FOC.get_options_price_data(contract_symbol)
 ```
 What else?
 ----------
 
 Let me know what other features would be useful to implement, create an issue on the repo or  [email me](mailto:benjaminchamwb@gmail.com).
 
 If you like my work, do consider supporting me so that i can dedicate more time and attention.
```

### Comparing `freeoptionschain-0.0.0/README.md` & `freeoptionschain-0.0.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -38,26 +38,26 @@
 ``` {.sourceCode .bash}
 pip install freeoptionschain
 ```
 Import
 ------
 
 ``` {.sourceCode .python}
-from FOC import *
+from FOC import FOC
 ```
 Fetch all options expiration dates for a stock
 ---------------------------------
 To fetch the options expiration date for a specific stock for a given  expiration date, you can
 simply use:
 
 ``` {.sourceCode .python}
 #create instance
 ref_FOC = FOC()
 
-# Options Chain of AAPL CALL options for 6 October 2023
+# Fetch options expiration dates for 'AAPL'
 options_chain = ref_FOC.get_expiration_dates("AAPL")
 ```
 Fetch options chain with price
 ---------------------------------
 To fetch the options chain for a specific stock for a given  expiration date, you can
 simply use:
 
@@ -85,16 +85,18 @@
 To fetch single options contract for a specific symbol, you can
 simply use:
 
 ``` {.sourceCode .python}
 #create instance
 ref_FOC = FOC()
 
-# AAPL CALL options with strike $200 for 6 October 2023, with greeks
-options_contract = ref_FOC.get_options_price_data(ref_FOC.get_contract_symbol("AAPL",'2023-10-06','CALL',200.0))
+# get options contract symbol for AAPL CALL options with strike $200 for 6 October 2023
+contract_symbol = ref_FOC.get_contract_symbol("AAPL",'2023-10-06','CALL',200.0)
+#fetch options contract with greeks
+options_contract = ref_FOC.get_options_price_data(contract_symbol)
 ```
 What else?
 ----------
 
 Let me know what other features would be useful to implement, create an issue on the repo or  [email me](mailto:benjaminchamwb@gmail.com).
 
 If you like my work, do consider supporting me so that i can dedicate more time and attention.
```

### Comparing `freeoptionschain-0.0.0/freeoptionschain.egg-info/PKG-INFO` & `freeoptionschain-0.0.1/freeoptionschain.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: freeoptionschain
-Version: 0.0.0
-Summary: This downloads stock option data and calculates its greeks.
+Version: 0.0.1
+Summary: This library module retrieves stock options data from NASDAQ.
 Home-page: https://github.com/benjamincham/free_options_chain
 Author: Benjamin Cham
 Author-email: benjaminchamwb@gmail.com
 Project-URL: Bug Tracker, https://github.com/benjamincham/free_options_chain/issues
 Project-URL: Changelog, https://github.com/benjamincham/free_options_chain/releases
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Classifier: License :: OSI Approved :: MIT License
@@ -58,26 +58,26 @@
 ``` {.sourceCode .bash}
 pip install freeoptionschain
 ```
 Import
 ------
 
 ``` {.sourceCode .python}
-from FOC import *
+from FOC import FOC
 ```
 Fetch all options expiration dates for a stock
 ---------------------------------
 To fetch the options expiration date for a specific stock for a given  expiration date, you can
 simply use:
 
 ``` {.sourceCode .python}
 #create instance
 ref_FOC = FOC()
 
-# Options Chain of AAPL CALL options for 6 October 2023
+# Fetch options expiration dates for 'AAPL'
 options_chain = ref_FOC.get_expiration_dates("AAPL")
 ```
 Fetch options chain with price
 ---------------------------------
 To fetch the options chain for a specific stock for a given  expiration date, you can
 simply use:
 
@@ -105,16 +105,18 @@
 To fetch single options contract for a specific symbol, you can
 simply use:
 
 ``` {.sourceCode .python}
 #create instance
 ref_FOC = FOC()
 
-# AAPL CALL options with strike $200 for 6 October 2023, with greeks
-options_contract = ref_FOC.get_options_price_data(ref_FOC.get_contract_symbol("AAPL",'2023-10-06','CALL',200.0))
+# get options contract symbol for AAPL CALL options with strike $200 for 6 October 2023
+contract_symbol = ref_FOC.get_contract_symbol("AAPL",'2023-10-06','CALL',200.0)
+#fetch options contract with greeks
+options_contract = ref_FOC.get_options_price_data(contract_symbol)
 ```
 What else?
 ----------
 
 Let me know what other features would be useful to implement, create an issue on the repo or  [email me](mailto:benjaminchamwb@gmail.com).
 
 If you like my work, do consider supporting me so that i can dedicate more time and attention.
```

### Comparing `freeoptionschain-0.0.0/setup.py` & `freeoptionschain-0.0.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,16 +3,18 @@
 
 here = pathlib.Path(__file__).parent.resolve()
 
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(
     name='freeoptionschain',
+    
+    version='0.0.1',
 
-    description='This downloads stock option data and calculates its greeks.',
+    description='This library module retrieves stock options data from NASDAQ.',
 
     long_description=long_description,
 
     long_description_content_type='text/markdown',
 
     url='https://github.com/benjamincham/free_options_chain',
```

