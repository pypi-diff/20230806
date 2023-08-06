# Comparing `tmp/OpenVulnQuery-1.31.tar.gz` & `tmp/OpenVulnQuery-1.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/OpenVulnQuery-1.31.tar", last modified: Mon Nov 16 05:12:12 2020, max compression
+gzip compressed data, was "dist/OpenVulnQuery-1.34.tar", last modified: Sun Aug  6 03:17:08 2023, max compression
```

## Comparing `OpenVulnQuery-1.31.tar` & `OpenVulnQuery-1.34.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-11-16 05:12:12.076610 OpenVulnQuery-1.31/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-11-16 05:12:12.076610 OpenVulnQuery-1.31/OpenVulnQuery.egg-info/
--rw-r--r--   0 root         (0) root         (0)    20923 2020-11-16 05:12:12.000000 OpenVulnQuery-1.31/OpenVulnQuery.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      717 2020-11-16 05:12:12.000000 OpenVulnQuery-1.31/OpenVulnQuery.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2020-11-16 05:12:12.000000 OpenVulnQuery-1.31/OpenVulnQuery.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       59 2020-11-16 05:12:12.000000 OpenVulnQuery-1.31/OpenVulnQuery.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2020-11-16 04:57:14.000000 OpenVulnQuery-1.31/OpenVulnQuery.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       33 2020-11-16 05:12:12.000000 OpenVulnQuery-1.31/OpenVulnQuery.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2020-11-16 05:12:12.000000 OpenVulnQuery-1.31/OpenVulnQuery.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)    20923 2020-11-16 05:12:12.076610 OpenVulnQuery-1.31/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    16684 2020-11-16 04:48:56.000000 OpenVulnQuery-1.31/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-11-16 05:12:12.076610 OpenVulnQuery-1.31/openVulnQuery/
--rw-r--r--   0 root         (0) root         (0)      279 2020-11-16 04:48:56.000000 OpenVulnQuery-1.31/openVulnQuery/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-11-16 05:12:12.076610 OpenVulnQuery-1.31/openVulnQuery/_library/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-16 04:48:56.000000 OpenVulnQuery-1.31/openVulnQuery/_library/__init__.py
--rw-r--r--   0 root         (0) root         (0)      187 2020-11-16 04:48:56.000000 OpenVulnQuery-1.31/openVulnQuery/_library/_compatibility.py
--rw-r--r--   0 root         (0) root         (0)     4310 2020-11-16 04:48:56.000000 OpenVulnQuery-1.31/openVulnQuery/_library/advisory.py
--rw-r--r--   0 root         (0) root         (0)      792 2020-11-16 04:48:56.000000 OpenVulnQuery-1.31/openVulnQuery/_library/authorization.py
--rw-r--r--   0 root         (0) root         (0)    11146 2020-11-16 04:48:56.000000 OpenVulnQuery-1.31/openVulnQuery/_library/cli_api.py
--rw-r--r--   0 root         (0) root         (0)      878 2020-11-16 04:48:56.000000 OpenVulnQuery-1.31/openVulnQuery/_library/config.py
--rw-r--r--   0 root         (0) root         (0)      772 2020-11-16 04:48:56.000000 OpenVulnQuery-1.31/openVulnQuery/_library/constants.py
--rw-r--r--   0 root         (0) root         (0)     2234 2020-11-16 04:48:56.000000 OpenVulnQuery-1.31/openVulnQuery/_library/main.py
--rw-r--r--   0 root         (0) root         (0)    12900 2020-11-16 04:48:56.000000 OpenVulnQuery-1.31/openVulnQuery/_library/query_client.py
--rw-r--r--   0 root         (0) root         (0)     4130 2020-11-16 04:48:56.000000 OpenVulnQuery-1.31/openVulnQuery/_library/rest_api.py
--rw-r--r--   0 root         (0) root         (0)     4169 2020-11-16 04:48:56.000000 OpenVulnQuery-1.31/openVulnQuery/_library/utils.py
--rwxr-xr-x   0 root         (0) root         (0)       71 2020-11-16 04:48:56.000000 OpenVulnQuery-1.31/openVulnQuery/main.py
--rw-r--r--   0 root         (0) root         (0)       38 2020-11-16 05:12:12.076610 OpenVulnQuery-1.31/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      810 2020-11-16 04:48:56.000000 OpenVulnQuery-1.31/setup.py
+drwxr-xr-x   0 omar       (501) staff       (20)        0 2023-08-06 03:17:08.000000 OpenVulnQuery-1.34/
+drwxr-xr-x   0 omar       (501) staff       (20)        0 2023-08-06 03:17:08.000000 OpenVulnQuery-1.34/OpenVulnQuery.egg-info/
+-rw-r--r--   0 omar       (501) staff       (20)    22857 2023-08-06 03:17:08.000000 OpenVulnQuery-1.34/OpenVulnQuery.egg-info/PKG-INFO
+-rw-r--r--   0 omar       (501) staff       (20)      717 2023-08-06 03:17:08.000000 OpenVulnQuery-1.34/OpenVulnQuery.egg-info/SOURCES.txt
+-rw-r--r--   0 omar       (501) staff       (20)        1 2023-08-06 03:17:08.000000 OpenVulnQuery-1.34/OpenVulnQuery.egg-info/dependency_links.txt
+-rw-r--r--   0 omar       (501) staff       (20)       59 2023-08-06 03:17:08.000000 OpenVulnQuery-1.34/OpenVulnQuery.egg-info/entry_points.txt
+-rw-r--r--   0 omar       (501) staff       (20)        1 2023-08-06 03:17:08.000000 OpenVulnQuery-1.34/OpenVulnQuery.egg-info/not-zip-safe
+-rw-r--r--   0 omar       (501) staff       (20)       33 2023-08-06 03:17:08.000000 OpenVulnQuery-1.34/OpenVulnQuery.egg-info/requires.txt
+-rw-r--r--   0 omar       (501) staff       (20)       14 2023-08-06 03:17:08.000000 OpenVulnQuery-1.34/OpenVulnQuery.egg-info/top_level.txt
+-rw-r--r--   0 omar       (501) staff       (20)    22857 2023-08-06 03:17:08.000000 OpenVulnQuery-1.34/PKG-INFO
+-rw-r--r--   0 omar       (501) staff       (20)    18330 2023-08-06 03:07:01.000000 OpenVulnQuery-1.34/README.md
+drwxr-xr-x   0 omar       (501) staff       (20)        0 2023-08-06 03:17:08.000000 OpenVulnQuery-1.34/openVulnQuery/
+-rw-r--r--   0 omar       (501) staff       (20)      279 2023-08-06 03:07:01.000000 OpenVulnQuery-1.34/openVulnQuery/__init__.py
+drwxr-xr-x   0 omar       (501) staff       (20)        0 2023-08-06 03:17:08.000000 OpenVulnQuery-1.34/openVulnQuery/_library/
+-rw-r--r--   0 omar       (501) staff       (20)        0 2023-08-06 03:07:01.000000 OpenVulnQuery-1.34/openVulnQuery/_library/__init__.py
+-rw-r--r--   0 omar       (501) staff       (20)      187 2023-08-06 03:07:01.000000 OpenVulnQuery-1.34/openVulnQuery/_library/_compatibility.py
+-rw-r--r--   0 omar       (501) staff       (20)     5176 2023-08-06 03:07:01.000000 OpenVulnQuery-1.34/openVulnQuery/_library/advisory.py
+-rw-r--r--   0 omar       (501) staff       (20)     1032 2023-08-06 03:07:01.000000 OpenVulnQuery-1.34/openVulnQuery/_library/authorization.py
+-rw-r--r--   0 omar       (501) staff       (20)    14780 2023-08-06 03:07:01.000000 OpenVulnQuery-1.34/openVulnQuery/_library/cli_api.py
+-rw-r--r--   0 omar       (501) staff       (20)     1131 2023-08-06 03:07:01.000000 OpenVulnQuery-1.34/openVulnQuery/_library/config.py
+-rw-r--r--   0 omar       (501) staff       (20)     1830 2023-08-06 03:07:01.000000 OpenVulnQuery-1.34/openVulnQuery/_library/constants.py
+-rw-r--r--   0 omar       (501) staff       (20)     3513 2023-08-06 03:07:01.000000 OpenVulnQuery-1.34/openVulnQuery/_library/main.py
+-rw-r--r--   0 omar       (501) staff       (20)    17830 2023-08-06 03:07:01.000000 OpenVulnQuery-1.34/openVulnQuery/_library/query_client.py
+-rw-r--r--   0 omar       (501) staff       (20)      568 2023-08-06 03:07:01.000000 OpenVulnQuery-1.34/openVulnQuery/_library/rest_api.py
+-rw-r--r--   0 omar       (501) staff       (20)     4470 2023-08-06 03:07:01.000000 OpenVulnQuery-1.34/openVulnQuery/_library/utils.py
+-rwxr-xr-x   0 omar       (501) staff       (20)       71 2023-08-06 03:07:01.000000 OpenVulnQuery-1.34/openVulnQuery/main.py
+-rw-r--r--   0 omar       (501) staff       (20)       38 2023-08-06 03:17:08.000000 OpenVulnQuery-1.34/setup.cfg
+-rw-r--r--   0 omar       (501) staff       (20)      786 2023-08-06 03:16:34.000000 OpenVulnQuery-1.34/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `OpenVulnQuery-1.31/OpenVulnQuery.egg-info/PKG-INFO` & `OpenVulnQuery-1.34/OpenVulnQuery.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,104 +1,99 @@
 Metadata-Version: 2.1
 Name: OpenVulnQuery
-Version: 1.31
+Version: 1.34
 Summary: A python-based module(s) to query the Cisco PSIRT openVuln API.
-Home-page: https://github.com/CiscoPSIRT/openVulnAPI/tree/master/openVulnQuery
+Home-page: https://github.com/CiscoPSIRT/openVulnQuery
 Author:  Omar Santos
 Author-email: os@cisco.com
 License: The MIT License (MIT)
 Description: # openVulnQuery
         
-        A python-based module(s) to query the Cisco PSIRT openVuln API.
+        A python-based module(s) to query the Cisco PSIRT openVuln API. openVulnQuery is supported in Python version 3.x.
         
         The Cisco Product Security Incident Response Team (PSIRT) openVuln API is a RESTful API that allows customers to obtain Cisco Security Vulnerability information in different machine-consumable formats. APIs are important for customers because they allow their technical staff and programmers to build tools that help them do their job more effectively (in this case, to keep up with security vulnerability information). More information about the API can be found at: <https://developer.cisco.com/psirt>
         
         ## PIP Installation
         
-        You can easily do:
+        You can easily install openVulnQuery using [pip](https://pypi.org/project/pip/):
         
         ```
-        pip install openVulnQuery
+        pip3 install openVulnQuery
         ```
         
-        Depending on your environment, you may need to specify the latest version (1.29), as demonstrated below:
+        Alternatively, depending on your environment, you may need to specify the latest version (1.31), as demonstrated below:
         
         ```
-        python3 -m pip install openVulnQuery==1.30
+        python3 -m pip install openVulnQuery==1.31
         ```
         
-        If you are experiencing any difficulty installing openVulnQuery. Here is the link to [common installation issues solutions] (<https://github.com/iamparas/openVulnAPI/blob/master/openVulnQuery/InstallationIssueSolutions.md>).
+        If you are experiencing any difficulty installing openVulnQuery. Here is the link to [common installation issues solutions](<https://github.com/iamparas/openVulnAPI/blob/master/openVulnQuery/InstallationIssueSolutions.md>).
         
         Requirements
         
-        - Tested on Python Version 2.7 and 3.7
+        - Tested on Python 3.7 and 3.9.2
         - `argparse >= 1.4.0`
-        - requests >= 2.10.0`
+        - `requests >= 2.10.0`
         
         ## Config File
         
         Obtain client ID and Secret:
         
         1. Visit <https://apiconsole.cisco.com/>
         2. Sign In
         3. Select My Applications Tab
         4. Register a New Application by:
         
-          - Entering Application Name
-          - Under OAuth2.0 Credentials check Client Credentials
+          - Enter an application name
+          - Enter a description of your application.
+          - Application Type field is Service.
+          - Grant Type is Client Credentials.
           - Under Select APIs choose Cisco PSIRT openVuln API
           - Agree to the terms and service and click Register
         
-        5. Take note of the "rate contract" presented like e.g.:
-        
-          ```
-           Rate Limits
-           10    Calls per second
-           5,000    Calls per day
-          ```
-        
+        5. The openVuln API rate limits are shown in the https://apiconsole.cisco.com/apps/mykeys
         6. Note the value of "Client ID" (a string like e.g. 'abc12abcd13abcdefabcde1a')
         7. Note the value of "Client Secret" (a string like e.g. '1a2abcDEfaBcDefAbcDeFA3b')
         8. Provide the credentials to the application at runtime via two preferred alternativev ways:
         
           - Either export two matching environment variables (below the syntax for bash and assuming the values are as in steps 6\. and 7.):
         
-            ```
-               >> export CLIENT_ID="abc12abcd13abcdefabcde1a"
-               >> export CLIENT_SECRET="1a2abcDEfaBcDefAbcDeFA3b"
-            ```
+        ```
+        >> export CLIENT_ID="abc12abcd13abcdefabcde1a"
+        >> export CLIENT_SECRET="1a2abcDEfaBcDefAbcDeFA3b"
+        ```
         
           - Or create a valid JSON file (e.g. `credentials.json`) with these personal credentials similar to the below given (assuming the values are as in steps 6\. and 7.):
         
-            ```
-               {
-                   "CLIENT_ID": "abc12abcd13abcdefabcde1a",
-                   "CLIENT_SECRET": "1a2abcDEfaBcDefAbcDeFA3b"
-               }
-            ```
+        ```
+        {
+            "CLIENT_ID": "abc12abcd13abcdefabcde1a",
+            "CLIENT_SECRET": "1a2abcDEfaBcDefAbcDeFA3b"
+        }
+        ```
         
         9. Do not distribute the credentials file resulting from previous step
         
         **Notes**:
         
         - The resulting OAuth2 Token will be automatically generated on every call to the API.
         
         ## Run OpenVulnQuery in the Terminal
         
         - If installed with pip run the program by typing
         
-          ```
-          >>openVulnQuery --config PathToCredentialsFile --Advisory Type --API Filters --Parsing Fields --Output Format -Count
-          ```
+        ```
+        >> openVulnQuery --config PathToCredentialsFile --Advisory Type --API Filters --Parsing Fields --Output Format -Count
+        ```
         
         - Or cd into the directory with the main.py file and run using
         
-          ```
-          >>python main.py --config PathToCredentialsFile --Advisory Type --API Filters --Parsing Fields --Output Format -Count
-          ```
+        ```
+        >> python main.py --config PathToCredentialsFile --Advisory Type --API Filters --Parsing Fields --Output Format -Count
+        ```
         
           Notes:
         
         -- Used for whole word commands, - Used for single character commands
         
         ## Configuration (Optional)
         
@@ -113,51 +108,56 @@
         ```
         
         ## API Filters (Required)
         
         ```
         --all
                 Returns all advisories
-                Examples:
+                Example:
                 >> openVulnQuery --all
         
         
         --advisory
                 Search by specific advisory id
-                Examples:
+                Example:
                 >> openVulnQuery --advisory cisco-sa-20110201-webex
+                
+        --bugid
+                Search by specific Cisco Bug id
+                Example:
+                >> openVulnQuery --bugid CSCwb92675
         
         --cve
                 Search by specific cve id
-                Examples:
+                Example:
                 >> openVulnQuery --cve CVE-2010-3043
         
         --latest
                 Search by the last number of advisories published
-                Examples:
+                Example:
                 >> openVulnQuery  --latest 10
         
                 Note: the latest option is limited to 100 maximum queries
         
         --severity
                 Search by severity (low, medium, high, critical)
                 Examples:
                 >> openVulnQuery  --severity critical
                 >> openVulnQuery  --severity high
                 >> openVulnQuery  --severity medium
                 >> openVulnQuery  --severity low
         
         --year
                 Search by the year (1995 to present)
-                Examples:
+                Example:
                 >> openVulnQuery  --year 2016
         
         --product
                  Search by the product name
-                 Examples:
+                 Example:
                  >> openVulnQuery  --product Cisco
         
         --ios
                 Cisco Software Checker has been integrated with openVulnAPI.
                 Search by IOS version
                 Examples:
                 >> openVulnQuery --ios 15.6\(2\)SP  (*use \ to escape bracket in ios version)
@@ -177,14 +177,50 @@
                 >> openVulnQuery --nxos 8.3(1)
         
         --aci
                 Cisco Software Checker has been integrated with openVulnAPI.
                 Search by Cisco NX-OS (ACI mode) Software version.
                 Example:
                 >> openVulnQuery --aci 11.0(2j)
+                
+        --asa
+                Cisco Software Checker has been integrated with openVulnAPI.
+                Search by Cisco ASA Software version.
+                Example:
+                >> openVulnQuery --asa 9.18.1
+                
+        --fmc
+                Cisco Software Checker has been integrated with openVulnAPI.
+                Search by Cisco FMC Software version.
+                Example:
+                >> openVulnQuery --fmc 7.0.1
+                
+        --ftd
+                Cisco Software Checker has been integrated with openVulnAPI.
+                Search by Cisco FTD Software version.
+                Example:
+                >> openVulnQuery --ftd 7.0.1
+                
+        --fxos
+                Cisco Software Checker has been integrated with openVulnAPI.
+                Search by Cisco FXOS Software version.
+                Example:
+                >> openVulnQuery --fxos 2.6.1.131
+                
+        --OS
+                To obtain version information regarding the different Network Operating Systems.
+                Examples:
+                >> openVulnQuery --OS asa
+                >> openVulnQuery --OS ios
+                
+        --platform
+                To obtain platform alias information regarding the different Network Operating Systems.
+                Examples:
+                >> openVulnQuery --platform asa
+                >> openVulnQuery --platform nxos  
         ```
         
         **NOTE**: Cisco reserves the right to remove End-of-Support releases from the Cisco Software Checker (subsequently reflected in this API).
         
         
         ## Client Application (Optional)
         
@@ -214,14 +250,17 @@
         - advisory_title
         - publication_url
         - cwe
         - product_names
         - summary
         - vuln_title
         - cvrf_url
+        - csafUrl
+        
+        **NOTE**: [CSAF](https://csaf.io) is a specification for structured machine-readable vulnerability-related advisories and further refine those standards over time. CSAF is the new name and replacement for the Common Vulnerability Reporting Framework (CVRF). Cisco will support CVRF until December 31, 2023. More information at: https://csaf.io 
         
         ```
         -f or --fields
         
                 API Fields
                       Examples:
                       openVulnQuery --config PathToCredentialsFile --any API filter -f  or --fields list of fields separated by space
@@ -296,16 +335,16 @@
         
         No support for filtering based on --API fields, you can't use --year 2016 and --severity high
         
         Filtering with Grep:
         
         ```
         Finding the Number of CVRF Advisories with a "Critical" sir in 2013
-                >> openVulnQuery --config PathToCredentialsFile  --year 2013 -f sir | grep -c "Critical"
-                >> openVulnQuery --config PathToCredentialsFile  --severity critical -f first_published | grep -c "2013"
+        >> openVulnQuery --config PathToCredentialsFile  --year 2013 -f sir | grep -c "Critical"
+        >> openVulnQuery --config PathToCredentialsFile  --severity critical -f first_published | grep -c "2013"
         ```
         
         If more than one API filter is entered, the last filter will be used for the API call.
         
         You can alternatively use the date range functionality, as shown below:
         
         ```
@@ -417,27 +456,27 @@
         ```
         
         ### Running the tests
         
         To run the tests in the tests folder, the additional required `mock` module should be installed inside the `venv`with the usual:
         
         ```
-        pip install mock pytest
+        pip3 install mock pytest
         ```
         
         There are unit tests in `tests/` and some sample like system level test (`tests/test_query_client_cvrf.py`) skipped in below sample runs, as it contacting the real API.
         
-        Sample run (expecting `pytest` has been installed e.g. via `pip install pytest`):
+        Sample run (expecting `pytest` has been installed e.g. via `pip3 install pytest`):
         
         ```
         $ cd /www/github.com/CiscoPSIRT/openVulnAPI/openVulnQuery
         
         $ pytest
         =========================================================================================================== test session starts ============================================================================================================
-        platform darwin -- Python 2.7.13, pytest-3.1.2, py-1.4.34, pluggy-0.4.0
+        platform darwin -- pytest-3.1.2, py-1.4.34, pluggy-0.4.0
         rootdir: /www/github.com/CiscoPSIRT/openVulnAPI/openVulnQuery, inifile:
         plugins: cov-2.5.1
         collected 159 items
         
         tests/test_advisory.py ......................
         tests/test_authorization.py ...
         tests/test_cli_api.py ..............................................
@@ -452,15 +491,15 @@
         ```
         
         Including coverage info (requires `pip install pytest-cov` which includes `pip install coverage` ):
         
         ```
         $ pytest --cov=openVulnQuery --cov-report=term-missing --cov-report=html
         =========================================================================================================== test session starts ============================================================================================================
-        platform darwin -- Python 2.7.13, pytest-3.1.2, py-1.4.34, pluggy-0.4.0
+        platform darwin -- pytest-3.1.2, py-1.4.34, pluggy-0.4.0
         rootdir: /www/github.com/CiscoPSIRT/openVulnAPI/openVulnQuery, inifile:
         plugins: cov-2.5.1
         collected 159 items
         
         tests/test_advisory.py ......................
         tests/test_authorization.py ...
         tests/test_cli_api.py ..............................................
```

### Comparing `OpenVulnQuery-1.31/OpenVulnQuery.egg-info/SOURCES.txt` & `OpenVulnQuery-1.34/OpenVulnQuery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OpenVulnQuery-1.31/PKG-INFO` & `OpenVulnQuery-1.34/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,104 +1,99 @@
 Metadata-Version: 2.1
 Name: OpenVulnQuery
-Version: 1.31
+Version: 1.34
 Summary: A python-based module(s) to query the Cisco PSIRT openVuln API.
-Home-page: https://github.com/CiscoPSIRT/openVulnAPI/tree/master/openVulnQuery
+Home-page: https://github.com/CiscoPSIRT/openVulnQuery
 Author:  Omar Santos
 Author-email: os@cisco.com
 License: The MIT License (MIT)
 Description: # openVulnQuery
         
-        A python-based module(s) to query the Cisco PSIRT openVuln API.
+        A python-based module(s) to query the Cisco PSIRT openVuln API. openVulnQuery is supported in Python version 3.x.
         
         The Cisco Product Security Incident Response Team (PSIRT) openVuln API is a RESTful API that allows customers to obtain Cisco Security Vulnerability information in different machine-consumable formats. APIs are important for customers because they allow their technical staff and programmers to build tools that help them do their job more effectively (in this case, to keep up with security vulnerability information). More information about the API can be found at: <https://developer.cisco.com/psirt>
         
         ## PIP Installation
         
-        You can easily do:
+        You can easily install openVulnQuery using [pip](https://pypi.org/project/pip/):
         
         ```
-        pip install openVulnQuery
+        pip3 install openVulnQuery
         ```
         
-        Depending on your environment, you may need to specify the latest version (1.29), as demonstrated below:
+        Alternatively, depending on your environment, you may need to specify the latest version (1.31), as demonstrated below:
         
         ```
-        python3 -m pip install openVulnQuery==1.30
+        python3 -m pip install openVulnQuery==1.31
         ```
         
-        If you are experiencing any difficulty installing openVulnQuery. Here is the link to [common installation issues solutions] (<https://github.com/iamparas/openVulnAPI/blob/master/openVulnQuery/InstallationIssueSolutions.md>).
+        If you are experiencing any difficulty installing openVulnQuery. Here is the link to [common installation issues solutions](<https://github.com/iamparas/openVulnAPI/blob/master/openVulnQuery/InstallationIssueSolutions.md>).
         
         Requirements
         
-        - Tested on Python Version 2.7 and 3.7
+        - Tested on Python 3.7 and 3.9.2
         - `argparse >= 1.4.0`
-        - requests >= 2.10.0`
+        - `requests >= 2.10.0`
         
         ## Config File
         
         Obtain client ID and Secret:
         
         1. Visit <https://apiconsole.cisco.com/>
         2. Sign In
         3. Select My Applications Tab
         4. Register a New Application by:
         
-          - Entering Application Name
-          - Under OAuth2.0 Credentials check Client Credentials
+          - Enter an application name
+          - Enter a description of your application.
+          - Application Type field is Service.
+          - Grant Type is Client Credentials.
           - Under Select APIs choose Cisco PSIRT openVuln API
           - Agree to the terms and service and click Register
         
-        5. Take note of the "rate contract" presented like e.g.:
-        
-          ```
-           Rate Limits
-           10    Calls per second
-           5,000    Calls per day
-          ```
-        
+        5. The openVuln API rate limits are shown in the https://apiconsole.cisco.com/apps/mykeys
         6. Note the value of "Client ID" (a string like e.g. 'abc12abcd13abcdefabcde1a')
         7. Note the value of "Client Secret" (a string like e.g. '1a2abcDEfaBcDefAbcDeFA3b')
         8. Provide the credentials to the application at runtime via two preferred alternativev ways:
         
           - Either export two matching environment variables (below the syntax for bash and assuming the values are as in steps 6\. and 7.):
         
-            ```
-               >> export CLIENT_ID="abc12abcd13abcdefabcde1a"
-               >> export CLIENT_SECRET="1a2abcDEfaBcDefAbcDeFA3b"
-            ```
+        ```
+        >> export CLIENT_ID="abc12abcd13abcdefabcde1a"
+        >> export CLIENT_SECRET="1a2abcDEfaBcDefAbcDeFA3b"
+        ```
         
           - Or create a valid JSON file (e.g. `credentials.json`) with these personal credentials similar to the below given (assuming the values are as in steps 6\. and 7.):
         
-            ```
-               {
-                   "CLIENT_ID": "abc12abcd13abcdefabcde1a",
-                   "CLIENT_SECRET": "1a2abcDEfaBcDefAbcDeFA3b"
-               }
-            ```
+        ```
+        {
+            "CLIENT_ID": "abc12abcd13abcdefabcde1a",
+            "CLIENT_SECRET": "1a2abcDEfaBcDefAbcDeFA3b"
+        }
+        ```
         
         9. Do not distribute the credentials file resulting from previous step
         
         **Notes**:
         
         - The resulting OAuth2 Token will be automatically generated on every call to the API.
         
         ## Run OpenVulnQuery in the Terminal
         
         - If installed with pip run the program by typing
         
-          ```
-          >>openVulnQuery --config PathToCredentialsFile --Advisory Type --API Filters --Parsing Fields --Output Format -Count
-          ```
+        ```
+        >> openVulnQuery --config PathToCredentialsFile --Advisory Type --API Filters --Parsing Fields --Output Format -Count
+        ```
         
         - Or cd into the directory with the main.py file and run using
         
-          ```
-          >>python main.py --config PathToCredentialsFile --Advisory Type --API Filters --Parsing Fields --Output Format -Count
-          ```
+        ```
+        >> python main.py --config PathToCredentialsFile --Advisory Type --API Filters --Parsing Fields --Output Format -Count
+        ```
         
           Notes:
         
         -- Used for whole word commands, - Used for single character commands
         
         ## Configuration (Optional)
         
@@ -113,51 +108,56 @@
         ```
         
         ## API Filters (Required)
         
         ```
         --all
                 Returns all advisories
-                Examples:
+                Example:
                 >> openVulnQuery --all
         
         
         --advisory
                 Search by specific advisory id
-                Examples:
+                Example:
                 >> openVulnQuery --advisory cisco-sa-20110201-webex
+                
+        --bugid
+                Search by specific Cisco Bug id
+                Example:
+                >> openVulnQuery --bugid CSCwb92675
         
         --cve
                 Search by specific cve id
-                Examples:
+                Example:
                 >> openVulnQuery --cve CVE-2010-3043
         
         --latest
                 Search by the last number of advisories published
-                Examples:
+                Example:
                 >> openVulnQuery  --latest 10
         
                 Note: the latest option is limited to 100 maximum queries
         
         --severity
                 Search by severity (low, medium, high, critical)
                 Examples:
                 >> openVulnQuery  --severity critical
                 >> openVulnQuery  --severity high
                 >> openVulnQuery  --severity medium
                 >> openVulnQuery  --severity low
         
         --year
                 Search by the year (1995 to present)
-                Examples:
+                Example:
                 >> openVulnQuery  --year 2016
         
         --product
                  Search by the product name
-                 Examples:
+                 Example:
                  >> openVulnQuery  --product Cisco
         
         --ios
                 Cisco Software Checker has been integrated with openVulnAPI.
                 Search by IOS version
                 Examples:
                 >> openVulnQuery --ios 15.6\(2\)SP  (*use \ to escape bracket in ios version)
@@ -177,14 +177,50 @@
                 >> openVulnQuery --nxos 8.3(1)
         
         --aci
                 Cisco Software Checker has been integrated with openVulnAPI.
                 Search by Cisco NX-OS (ACI mode) Software version.
                 Example:
                 >> openVulnQuery --aci 11.0(2j)
+                
+        --asa
+                Cisco Software Checker has been integrated with openVulnAPI.
+                Search by Cisco ASA Software version.
+                Example:
+                >> openVulnQuery --asa 9.18.1
+                
+        --fmc
+                Cisco Software Checker has been integrated with openVulnAPI.
+                Search by Cisco FMC Software version.
+                Example:
+                >> openVulnQuery --fmc 7.0.1
+                
+        --ftd
+                Cisco Software Checker has been integrated with openVulnAPI.
+                Search by Cisco FTD Software version.
+                Example:
+                >> openVulnQuery --ftd 7.0.1
+                
+        --fxos
+                Cisco Software Checker has been integrated with openVulnAPI.
+                Search by Cisco FXOS Software version.
+                Example:
+                >> openVulnQuery --fxos 2.6.1.131
+                
+        --OS
+                To obtain version information regarding the different Network Operating Systems.
+                Examples:
+                >> openVulnQuery --OS asa
+                >> openVulnQuery --OS ios
+                
+        --platform
+                To obtain platform alias information regarding the different Network Operating Systems.
+                Examples:
+                >> openVulnQuery --platform asa
+                >> openVulnQuery --platform nxos  
         ```
         
         **NOTE**: Cisco reserves the right to remove End-of-Support releases from the Cisco Software Checker (subsequently reflected in this API).
         
         
         ## Client Application (Optional)
         
@@ -214,14 +250,17 @@
         - advisory_title
         - publication_url
         - cwe
         - product_names
         - summary
         - vuln_title
         - cvrf_url
+        - csafUrl
+        
+        **NOTE**: [CSAF](https://csaf.io) is a specification for structured machine-readable vulnerability-related advisories and further refine those standards over time. CSAF is the new name and replacement for the Common Vulnerability Reporting Framework (CVRF). Cisco will support CVRF until December 31, 2023. More information at: https://csaf.io 
         
         ```
         -f or --fields
         
                 API Fields
                       Examples:
                       openVulnQuery --config PathToCredentialsFile --any API filter -f  or --fields list of fields separated by space
@@ -296,16 +335,16 @@
         
         No support for filtering based on --API fields, you can't use --year 2016 and --severity high
         
         Filtering with Grep:
         
         ```
         Finding the Number of CVRF Advisories with a "Critical" sir in 2013
-                >> openVulnQuery --config PathToCredentialsFile  --year 2013 -f sir | grep -c "Critical"
-                >> openVulnQuery --config PathToCredentialsFile  --severity critical -f first_published | grep -c "2013"
+        >> openVulnQuery --config PathToCredentialsFile  --year 2013 -f sir | grep -c "Critical"
+        >> openVulnQuery --config PathToCredentialsFile  --severity critical -f first_published | grep -c "2013"
         ```
         
         If more than one API filter is entered, the last filter will be used for the API call.
         
         You can alternatively use the date range functionality, as shown below:
         
         ```
@@ -417,27 +456,27 @@
         ```
         
         ### Running the tests
         
         To run the tests in the tests folder, the additional required `mock` module should be installed inside the `venv`with the usual:
         
         ```
-        pip install mock pytest
+        pip3 install mock pytest
         ```
         
         There are unit tests in `tests/` and some sample like system level test (`tests/test_query_client_cvrf.py`) skipped in below sample runs, as it contacting the real API.
         
-        Sample run (expecting `pytest` has been installed e.g. via `pip install pytest`):
+        Sample run (expecting `pytest` has been installed e.g. via `pip3 install pytest`):
         
         ```
         $ cd /www/github.com/CiscoPSIRT/openVulnAPI/openVulnQuery
         
         $ pytest
         =========================================================================================================== test session starts ============================================================================================================
-        platform darwin -- Python 2.7.13, pytest-3.1.2, py-1.4.34, pluggy-0.4.0
+        platform darwin -- pytest-3.1.2, py-1.4.34, pluggy-0.4.0
         rootdir: /www/github.com/CiscoPSIRT/openVulnAPI/openVulnQuery, inifile:
         plugins: cov-2.5.1
         collected 159 items
         
         tests/test_advisory.py ......................
         tests/test_authorization.py ...
         tests/test_cli_api.py ..............................................
@@ -452,15 +491,15 @@
         ```
         
         Including coverage info (requires `pip install pytest-cov` which includes `pip install coverage` ):
         
         ```
         $ pytest --cov=openVulnQuery --cov-report=term-missing --cov-report=html
         =========================================================================================================== test session starts ============================================================================================================
-        platform darwin -- Python 2.7.13, pytest-3.1.2, py-1.4.34, pluggy-0.4.0
+        platform darwin -- pytest-3.1.2, py-1.4.34, pluggy-0.4.0
         rootdir: /www/github.com/CiscoPSIRT/openVulnAPI/openVulnQuery, inifile:
         plugins: cov-2.5.1
         collected 159 items
         
         tests/test_advisory.py ......................
         tests/test_authorization.py ...
         tests/test_cli_api.py ..............................................
```

### Comparing `OpenVulnQuery-1.31/README.md` & `OpenVulnQuery-1.34/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,96 +1,91 @@
 # openVulnQuery
 
-A python-based module(s) to query the Cisco PSIRT openVuln API.
+A python-based module(s) to query the Cisco PSIRT openVuln API. openVulnQuery is supported in Python version 3.x.
 
 The Cisco Product Security Incident Response Team (PSIRT) openVuln API is a RESTful API that allows customers to obtain Cisco Security Vulnerability information in different machine-consumable formats. APIs are important for customers because they allow their technical staff and programmers to build tools that help them do their job more effectively (in this case, to keep up with security vulnerability information). More information about the API can be found at: <https://developer.cisco.com/psirt>
 
 ## PIP Installation
 
-You can easily do:
+You can easily install openVulnQuery using [pip](https://pypi.org/project/pip/):
 
 ```
-pip install openVulnQuery
+pip3 install openVulnQuery
 ```
 
-Depending on your environment, you may need to specify the latest version (1.29), as demonstrated below:
+Alternatively, depending on your environment, you may need to specify the latest version (1.31), as demonstrated below:
 
 ```
-python3 -m pip install openVulnQuery==1.30
+python3 -m pip install openVulnQuery==1.31
 ```
 
-If you are experiencing any difficulty installing openVulnQuery. Here is the link to [common installation issues solutions] (<https://github.com/iamparas/openVulnAPI/blob/master/openVulnQuery/InstallationIssueSolutions.md>).
+If you are experiencing any difficulty installing openVulnQuery. Here is the link to [common installation issues solutions](<https://github.com/iamparas/openVulnAPI/blob/master/openVulnQuery/InstallationIssueSolutions.md>).
 
 Requirements
 
-- Tested on Python Version 2.7 and 3.7
+- Tested on Python 3.7 and 3.9.2
 - `argparse >= 1.4.0`
-- requests >= 2.10.0`
+- `requests >= 2.10.0`
 
 ## Config File
 
 Obtain client ID and Secret:
 
 1. Visit <https://apiconsole.cisco.com/>
 2. Sign In
 3. Select My Applications Tab
 4. Register a New Application by:
 
-  - Entering Application Name
-  - Under OAuth2.0 Credentials check Client Credentials
+  - Enter an application name
+  - Enter a description of your application.
+  - Application Type field is Service.
+  - Grant Type is Client Credentials.
   - Under Select APIs choose Cisco PSIRT openVuln API
   - Agree to the terms and service and click Register
 
-5. Take note of the "rate contract" presented like e.g.:
-
-  ```
-   Rate Limits
-   10    Calls per second
-   5,000    Calls per day
-  ```
-
+5. The openVuln API rate limits are shown in the https://apiconsole.cisco.com/apps/mykeys
 6. Note the value of "Client ID" (a string like e.g. 'abc12abcd13abcdefabcde1a')
 7. Note the value of "Client Secret" (a string like e.g. '1a2abcDEfaBcDefAbcDeFA3b')
 8. Provide the credentials to the application at runtime via two preferred alternativev ways:
 
   - Either export two matching environment variables (below the syntax for bash and assuming the values are as in steps 6\. and 7.):
 
-    ```
-       >> export CLIENT_ID="abc12abcd13abcdefabcde1a"
-       >> export CLIENT_SECRET="1a2abcDEfaBcDefAbcDeFA3b"
-    ```
+```
+>> export CLIENT_ID="abc12abcd13abcdefabcde1a"
+>> export CLIENT_SECRET="1a2abcDEfaBcDefAbcDeFA3b"
+```
 
   - Or create a valid JSON file (e.g. `credentials.json`) with these personal credentials similar to the below given (assuming the values are as in steps 6\. and 7.):
 
-    ```
-       {
-           "CLIENT_ID": "abc12abcd13abcdefabcde1a",
-           "CLIENT_SECRET": "1a2abcDEfaBcDefAbcDeFA3b"
-       }
-    ```
+```
+{
+    "CLIENT_ID": "abc12abcd13abcdefabcde1a",
+    "CLIENT_SECRET": "1a2abcDEfaBcDefAbcDeFA3b"
+}
+```
 
 9. Do not distribute the credentials file resulting from previous step
 
 **Notes**:
 
 - The resulting OAuth2 Token will be automatically generated on every call to the API.
 
 ## Run OpenVulnQuery in the Terminal
 
 - If installed with pip run the program by typing
 
-  ```
-  >>openVulnQuery --config PathToCredentialsFile --Advisory Type --API Filters --Parsing Fields --Output Format -Count
-  ```
+```
+>> openVulnQuery --config PathToCredentialsFile --Advisory Type --API Filters --Parsing Fields --Output Format -Count
+```
 
 - Or cd into the directory with the main.py file and run using
 
-  ```
-  >>python main.py --config PathToCredentialsFile --Advisory Type --API Filters --Parsing Fields --Output Format -Count
-  ```
+```
+>> python main.py --config PathToCredentialsFile --Advisory Type --API Filters --Parsing Fields --Output Format -Count
+```
 
   Notes:
 
 -- Used for whole word commands, - Used for single character commands
 
 ## Configuration (Optional)
 
@@ -105,51 +100,56 @@
 ```
 
 ## API Filters (Required)
 
 ```
 --all
         Returns all advisories
-        Examples:
+        Example:
         >> openVulnQuery --all
 
 
 --advisory
         Search by specific advisory id
-        Examples:
+        Example:
         >> openVulnQuery --advisory cisco-sa-20110201-webex
+        
+--bugid
+        Search by specific Cisco Bug id
+        Example:
+        >> openVulnQuery --bugid CSCwb92675
 
 --cve
         Search by specific cve id
-        Examples:
+        Example:
         >> openVulnQuery --cve CVE-2010-3043
 
 --latest
         Search by the last number of advisories published
-        Examples:
+        Example:
         >> openVulnQuery  --latest 10
 
         Note: the latest option is limited to 100 maximum queries
 
 --severity
         Search by severity (low, medium, high, critical)
         Examples:
         >> openVulnQuery  --severity critical
         >> openVulnQuery  --severity high
         >> openVulnQuery  --severity medium
         >> openVulnQuery  --severity low
 
 --year
         Search by the year (1995 to present)
-        Examples:
+        Example:
         >> openVulnQuery  --year 2016
 
 --product
          Search by the product name
-         Examples:
+         Example:
          >> openVulnQuery  --product Cisco
 
 --ios
         Cisco Software Checker has been integrated with openVulnAPI.
         Search by IOS version
         Examples:
         >> openVulnQuery --ios 15.6\(2\)SP  (*use \ to escape bracket in ios version)
@@ -169,14 +169,50 @@
         >> openVulnQuery --nxos 8.3(1)
 
 --aci
         Cisco Software Checker has been integrated with openVulnAPI.
         Search by Cisco NX-OS (ACI mode) Software version.
         Example:
         >> openVulnQuery --aci 11.0(2j)
+        
+--asa
+        Cisco Software Checker has been integrated with openVulnAPI.
+        Search by Cisco ASA Software version.
+        Example:
+        >> openVulnQuery --asa 9.18.1
+        
+--fmc
+        Cisco Software Checker has been integrated with openVulnAPI.
+        Search by Cisco FMC Software version.
+        Example:
+        >> openVulnQuery --fmc 7.0.1
+        
+--ftd
+        Cisco Software Checker has been integrated with openVulnAPI.
+        Search by Cisco FTD Software version.
+        Example:
+        >> openVulnQuery --ftd 7.0.1
+        
+--fxos
+        Cisco Software Checker has been integrated with openVulnAPI.
+        Search by Cisco FXOS Software version.
+        Example:
+        >> openVulnQuery --fxos 2.6.1.131
+        
+--OS
+        To obtain version information regarding the different Network Operating Systems.
+        Examples:
+        >> openVulnQuery --OS asa
+        >> openVulnQuery --OS ios
+        
+--platform
+        To obtain platform alias information regarding the different Network Operating Systems.
+        Examples:
+        >> openVulnQuery --platform asa
+        >> openVulnQuery --platform nxos  
 ```
 
 **NOTE**: Cisco reserves the right to remove End-of-Support releases from the Cisco Software Checker (subsequently reflected in this API).
 
 
 ## Client Application (Optional)
 
@@ -206,14 +242,17 @@
 - advisory_title
 - publication_url
 - cwe
 - product_names
 - summary
 - vuln_title
 - cvrf_url
+- csafUrl
+
+**NOTE**: [CSAF](https://csaf.io) is a specification for structured machine-readable vulnerability-related advisories and further refine those standards over time. CSAF is the new name and replacement for the Common Vulnerability Reporting Framework (CVRF). Cisco will support CVRF until December 31, 2023. More information at: https://csaf.io 
 
 ```
 -f or --fields
 
         API Fields
               Examples:
               openVulnQuery --config PathToCredentialsFile --any API filter -f  or --fields list of fields separated by space
@@ -288,16 +327,16 @@
 
 No support for filtering based on --API fields, you can't use --year 2016 and --severity high
 
 Filtering with Grep:
 
 ```
 Finding the Number of CVRF Advisories with a "Critical" sir in 2013
-        >> openVulnQuery --config PathToCredentialsFile  --year 2013 -f sir | grep -c "Critical"
-        >> openVulnQuery --config PathToCredentialsFile  --severity critical -f first_published | grep -c "2013"
+>> openVulnQuery --config PathToCredentialsFile  --year 2013 -f sir | grep -c "Critical"
+>> openVulnQuery --config PathToCredentialsFile  --severity critical -f first_published | grep -c "2013"
 ```
 
 If more than one API filter is entered, the last filter will be used for the API call.
 
 You can alternatively use the date range functionality, as shown below:
 
 ```
@@ -409,27 +448,27 @@
 ```
 
 ### Running the tests
 
 To run the tests in the tests folder, the additional required `mock` module should be installed inside the `venv`with the usual:
 
 ```
-pip install mock pytest
+pip3 install mock pytest
 ```
 
 There are unit tests in `tests/` and some sample like system level test (`tests/test_query_client_cvrf.py`) skipped in below sample runs, as it contacting the real API.
 
-Sample run (expecting `pytest` has been installed e.g. via `pip install pytest`):
+Sample run (expecting `pytest` has been installed e.g. via `pip3 install pytest`):
 
 ```
 $ cd /www/github.com/CiscoPSIRT/openVulnAPI/openVulnQuery
 
 $ pytest
 =========================================================================================================== test session starts ============================================================================================================
-platform darwin -- Python 2.7.13, pytest-3.1.2, py-1.4.34, pluggy-0.4.0
+platform darwin -- pytest-3.1.2, py-1.4.34, pluggy-0.4.0
 rootdir: /www/github.com/CiscoPSIRT/openVulnAPI/openVulnQuery, inifile:
 plugins: cov-2.5.1
 collected 159 items
 
 tests/test_advisory.py ......................
 tests/test_authorization.py ...
 tests/test_cli_api.py ..............................................
@@ -444,15 +483,15 @@
 ```
 
 Including coverage info (requires `pip install pytest-cov` which includes `pip install coverage` ):
 
 ```
 $ pytest --cov=openVulnQuery --cov-report=term-missing --cov-report=html
 =========================================================================================================== test session starts ============================================================================================================
-platform darwin -- Python 2.7.13, pytest-3.1.2, py-1.4.34, pluggy-0.4.0
+platform darwin -- pytest-3.1.2, py-1.4.34, pluggy-0.4.0
 rootdir: /www/github.com/CiscoPSIRT/openVulnAPI/openVulnQuery, inifile:
 plugins: cov-2.5.1
 collected 159 items
 
 tests/test_advisory.py ......................
 tests/test_authorization.py ...
 tests/test_cli_api.py ..............................................
```

### Comparing `OpenVulnQuery-1.31/openVulnQuery/_library/advisory.py` & `OpenVulnQuery-1.34/openVulnQuery/_library/advisory.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,45 @@
 from abc import ABCMeta
 
 from . import constants
 from ._compatibility import is_unicode_or_bytes
 
 NA = constants.NA_INDICATOR
 IPS_SIG = constants.IPS_SIGNATURE_LABEL
+PLATFORMS_TAG = constants.PLATFORMS_LABEL
 
 ADVISORIES_COMMONS_MAP = {
     'advisory_id': "advisoryId",
     'advisory_title': "advisoryTitle",
     'bug_ids': "bugIDs",
     'cves': "cves",
     'cvss_base_score': "cvssBaseScore",
     'cwe': "cwe",
     'first_published': "firstPublished",
     'last_updated': "lastUpdated",
     'product_names': "productNames",
     'publication_url': "publicationUrl",
     'cvrfUrl': "cvrfUrl",
+    'csafUrl': "csafUrl",
     'sir': "sir",
     'summary': "summary",
 }
 
 IPS_SIG_MAP = {
     IPS_SIG: 'ipsSignatures',
 }
 
-
 IOS_ADD_ONS_MAP = {
     'first_fixed': 'firstFixed',
     'ios_release': 'iosRelease',
 }
 
+PLATFORMS_MAP = {
+    PLATFORMS_TAG: 'platforms',
+}
 
 class Filterable(object):
     """Filterable mixin class"""
 
     def filter(self, *args):
         filtered_dict = {}
         for arg in args:
@@ -55,81 +59,102 @@
     This class abstracts advisory object
     """
 
     __metaclass__ = ABCMeta
 
     def __init__(self, advisory_id, sir, first_published, last_updated, cves,
                  bug_ids, cvss_base_score, advisory_title, publication_url,
-                 cwe, cvrfUrl,
-                 product_names, summary):
+                 cwe, cvrfUrl, csafUrl, product_names, summary):
         self.advisory_id = advisory_id
         self.sir = sir
         self.first_published = first_published
         self.last_updated = last_updated
         self.cves = cves
         self.bug_ids = bug_ids
         self.cvss_base_score = cvss_base_score
         self.advisory_title = advisory_title
         self.publication_url = publication_url
         self.cwe = cwe
         self.cvrfUrl = cvrfUrl
+        self.csafUrl = csafUrl
         self.product_names = product_names
         self.summary = summary
 
-
 class AdvisoryDefault(Advisory):
     """Default object inherits from Advisory"""
 
     def __init__(self, *args, **kwargs):
         self.ips_signatures = []
         if IPS_SIG in kwargs:
             self.ips_signatures = [
                 IPSSignature(**kw) if not is_unicode_or_bytes(kw) else NA
                 for kw in kwargs.pop(IPS_SIG)]
+
+        self.platforms = []
+        if 'platforms' in kwargs:
+            self.platforms = [
+                platformsList(**kw) if not is_unicode_or_bytes(kw) else NA
+                for kw in kwargs.pop('platforms')]
+
         super(AdvisoryDefault, self).__init__(*args, **kwargs)
 
 class AdvisoryIOS(Advisory):
     """Advisory Object with additional information on IOS/IOSXE version """
 
     def __init__(self, *args, **kwargs):
+        self.ips_signatures = []
+        if IPS_SIG in kwargs:
+            self.ips_signatures = [
+                IPSSignature(**kw) if not is_unicode_or_bytes(kw) else NA
+                for kw in kwargs.pop(IPS_SIG)]
+
         self.first_fixed = kwargs.pop('first_fixed', None)
         self.ios_release = kwargs.pop('ios_release', None)
         super(AdvisoryIOS, self).__init__(*args, **kwargs)
 
-
 class IPSSignature(Filterable):
     def __init__(self, legacyIpsId, releaseVersion, softwareVersion,
                  legacyIpsUrl):
         self.legacy_ips_id = legacyIpsId
         self.release_version = releaseVersion
         self.software_version = softwareVersion
         self.legacy_ips_url = legacyIpsUrl
 
+class platformsList(Filterable):
+    def __init__(self, id, name, firstFixes, vulnerabilityState):
+        self.id = id
+        self.name = name
+        self.firstFixes = firstFixes
+        self.vulnerabilityState = vulnerabilityState
 
 def advisory_format_factory_map():
     """Map the advisory format tokens to callable instantiators."""
     return dict(zip(
         constants.ADVISORY_FORMAT_TOKENS, (AdvisoryDefault, AdvisoryIOS)))
 
 def advisory_factory(adv_data, adv_format, logger):
     """Converts json into a list of advisory objects.
     :param adv_data: A dictionary describing an advisory.
     :param adv_format: The target format in ('default', 'ios')
     :param logger: A logger (for now expecting to be ready to log)
     :returns advisory instance according to adv_format
     """
+
     adv_map = {}  # Initial fill from shared common model key map:
     for k, v in ADVISORIES_COMMONS_MAP.items():
         adv_map[k] = adv_data[v]
 
+    for k, v in IPS_SIG_MAP.items():
+        adv_map[k] = adv_data[v]
 
-    if adv_format == constants.DEFAULT_ADVISORY_FORMAT_TOKEN:
-        for k, v in IPS_SIG_MAP.items():
+    for k, v in PLATFORMS_MAP.items():
+        if v in adv_data:
             adv_map[k] = adv_data[v]
-    else:  # IOS advisory format targeted:
+
+    if adv_format == constants.IOS_ADVISORY_FORMAT_TOKEN:
         for k, v in IOS_ADD_ONS_MAP.items():
             if v in adv_data:
                 adv_map[k] = adv_data[v]
 
     an_adv = advisory_format_factory_map()[adv_format](**adv_map)
     logger.debug(
         "{} Advisory {} Created".format(adv_format, an_adv.advisory_id))
```

### Comparing `OpenVulnQuery-1.31/openVulnQuery/_library/authorization.py` & `OpenVulnQuery-1.34/openVulnQuery/_library/authorization.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,9 +15,13 @@
 
     """
     r = requests.post(
         request_token_url if request_token_url else config.REQUEST_TOKEN_URL,
         params={'client_id': client_id, 'client_secret': client_secret},
         data={'grant_type': 'client_credentials'}
     )
+    # Added check to see if migrated to new API structure.
+    if r.status_code == 400:
+        print("Ensure you have updated your code as per https://raw.githubusercontent.com/api-at-cisco/Images/master/Whats_New_Doc.pdf")
+        exit()
     r.raise_for_status()
     return r.json()['access_token']
```

### Comparing `OpenVulnQuery-1.31/openVulnQuery/_library/cli_api.py` & `OpenVulnQuery-1.34/openVulnQuery/_library/cli_api.py`

 * *Files 18% similar despite different names*

```diff
@@ -66,18 +66,15 @@
 '''
 
 CLI_API_API_RESOURCE = (
     {
         'action': 'store_const',
         'const': ('all', 'all'),
         'dest': 'api_resource',
-
-        'help': 'Retrieves all advisiories',
-
-      
+        'help': 'Retrieves all advisories',
         'tokens': ('--all',),
     },
     {
         'dest': 'api_resource',
         'help': 'Retrieve advisories by advisory id',
         'metavar': '<advisory-id>',
         'tokens': ('--advisory',),
@@ -88,15 +85,21 @@
         'help': 'Retrieve advisories by cve id',
         'metavar': '<CVE-id>',
         'tokens': ('--cve',),
         'type': (lambda x: ('cve', x)),
     },
     {
         'dest': 'api_resource',
-
+        'help': 'Retrieve advisories by Cisco Bug id',
+        'metavar': '<BUG-id>',
+        'tokens': ('--bugid',),
+        'type': (lambda x: ('bugid', x)),
+    },
+    {
+        'dest': 'api_resource',
         'help': 'Retrieves latest (number) advisories',
         'metavar': 'number',
         'tokens': ('--latest',),
         'type': (lambda x: ('latest', x)),
     },
     {
         'dest': 'api_resource',
@@ -119,47 +122,101 @@
         'metavar': 'product_name',
         'tokens': ('--product',),
         'type': (lambda x: ('product', x)),
     },
     {
         'dest': 'api_resource',
         'help': (
-            'Retrieve advisories affecting user inputted ios_xe version.'
+            'Retrieve advisories affecting user inputted ios_xe version. '
             'Only one version at a time is allowed.'),
         'metavar': 'iosxe_version',
         'tokens': ('--ios_xe',),
         'type': (lambda x: ('ios_xe', x)),
     },
     {
         'dest': 'api_resource',
         'help': (
-            'Retrieve advisories affecting user inputted ios version.'
+            'Retrieve advisories affecting user inputted ios version. '
             'Only one version at a time is allowed.'),
         'metavar': 'ios_version',
         'tokens': ('--ios',),
         'type': (lambda x: ('ios', x)),
     },
     {
         'dest': 'api_resource',
         'help': (
-            'Retrieve advisories affecting user inputted NX-OS (in standalone mode) version.'
+            'Retrieve advisories affecting user inputted NX-OS (in standalone mode) version. '
             'Only one version at a time is allowed.'),
         'metavar': 'nxos_version',
         'tokens': ('--nxos',),
         'type': (lambda x: ('nxos', x)),
     },
     {
         'dest': 'api_resource',
         'help': (
-            'Retrieve advisories affecting user inputted NX-OS (in ACI mode) version.'
+            'Retrieve advisories affecting user inputted NX-OS (in ACI mode) version. '
             'Only one version at a time is allowed.'),
         'metavar': 'aci_version',
         'tokens': ('--aci',),
         'type': (lambda x: ('aci', x)),
     },
+    {
+        'dest': 'api_resource',
+        'help': (
+            'Retrieve advisories affecting user inputted ASA version. '
+            'Only one version at a time is allowed.'),
+        'metavar': 'asa_version',
+        'tokens': ('--asa',),
+        'type': (lambda x: ('asa', x)),
+    },
+    {
+        'dest': 'api_resource',
+        'help': (
+            'Retrieve advisories affecting user inputted FMC version. '
+            'Only one version at a time is allowed.'),
+        'metavar': 'fmc_version',
+        'tokens': ('--fmc',),
+        'type': (lambda x: ('fmc', x)),
+    },
+    {
+        'dest': 'api_resource',
+        'help': (
+            'Retrieve advisories affecting user inputted FTD version. '
+            'Only one version at a time is allowed.'),
+        'metavar': 'ftd_version',
+        'tokens': ('--ftd',),
+        'type': (lambda x: ('ftd', x)),
+    },
+    {
+        'dest': 'api_resource',
+        'help': (
+            'Retrieve advisories affecting user inputted FXOS version. '
+            'Only one version at a time is allowed.'),
+        'metavar': 'fxos_version',
+        'tokens': ('--fxos',),
+        'type': (lambda x: ('fxos', x)),
+    },
+    {
+        'dest': 'api_resource',
+        'help': (
+            'Retrieve version information regarding the different Network Operating Systems. '
+            'Only one Network Operating System at a time is allowed.'),
+        'metavar': 'OS_version',
+        'tokens': ('--OS',),
+        'type': (lambda x: ('OS', x)),
+    },
+    {
+        'dest': 'api_resource',
+        'help': (
+            'Retrieve platform alias information regarding the different Network Operating Systems. '
+            'Only one Network Operating System at a time is allowed.'),
+        'metavar': 'platform',
+        'tokens': ('--platform',),
+        'type': (lambda x: ('platform', x)),
+    },
 )
 
 CLI_API_OUTPUT_FORMAT = (
     {
         'dest': 'output_format',
         'help': 'Output to CSV with file path',
         'metavar': 'filepath',
@@ -210,18 +267,28 @@
                  ' Allowed values are: %s' % ', '.join(constants.API_LABELS)),
         'metavar': '',
         'nargs': '+',
         'tokens': ('-f', '--fields'),  # TODO reversed order, verify that OK
     },
     {
         'dest': 'user_agent',
-        'help': 'Announced User-Agent hedar value (towards service)',
+        'help': 'Announced User-Agent headar value (towards service)',
         'metavar': 'string',
         'tokens': ('--user-agent',),
     },
+    {
+        'choices': constants.SUPPORTED_PLATFORMS_ALIAS_NAME_ASA + constants.SUPPORTED_PLATFORMS_ALIAS_NAME_FTD +
+                   constants.SUPPORTED_PLATFORMS_ALIAS_NAME_FXOS + constants.SUPPORTED_PLATFORMS_ALIAS_NAME_NXOS,
+        'dest': 'platformAlias',
+        'help': ('Single platform alias.  '
+                 ' Supported only for: %s' % ', '.join(constants.SUPPORTED_PLATFORMS_ALIAS)),
+        'metavar': '',
+        'nargs': '+',
+        'tokens': ('-pa', '--platformAlias'),
+    },
 )
 
 CLI_API_CONFIG = (
     {
         'dest': 'json_config_path',
         'help': ('Path to JSON file with config (otherwise fallback to'
                  ' environment variables CLIENT_ID and CLIENT_SECRET, or'
@@ -289,21 +356,40 @@
 def process_command_line(string_list=None):
     """Interpret parameters given in command line."""
 
     parser = parser_factory()
 
     args = parser.parse_args(args=string_list)
 
-
     if args.api_resource[0] not in constants.ALLOWS_FILTER:
         if args.first_published or args.last_published:
             parser.error(
                 'Only {} based filter can have additional first_published or'
                 ' last_published filter'.format(constants.ALLOWS_FILTER))
 
+    if args.api_resource[0] not in constants.SUPPORTED_PLATFORMS_ALIAS:
+        if args.platformAlias:
+            parser.error(
+                'Only {} based filter can have additional platformAlias filter'
+                .format(constants.SUPPORTED_PLATFORMS_ALIAS))
+
+    if args.api_resource[0] in constants.NON_ADVISORY_QUERY:
+        if args.count or args.fields:
+            parser.error(
+                '{} do not support fields or count options'.format(constants.NON_ADVISORY_QUERY))
+
+        if args.api_resource[0] == "OS":
+            if args.api_resource[1] not in constants.SUPPORTED_PLATFORMS_VERSION:
+                parser.error(
+                    'Only network operating system types for OS type query are: {}'.format(constants.SUPPORTED_PLATFORMS_VERSION))
+        elif args.api_resource[0] == "platform":
+            if args.api_resource[1] not in constants.SUPPORTED_PLATFORMS_ALIAS:
+                parser.error(
+                    'Only network operating system types for platform type query are: {}'.format(constants.SUPPORTED_PLATFORMS_ALIAS))
+
     if not args.json_config_path:
         # Try next environment variables are set, then config.py, or fail:
         keys_required = ('CLIENT_ID', 'CLIENT_SECRET')
         env_config = {k: os.getenv(k, None) for k in keys_required}
 
         if all([v for v in env_config.values()]):  # OK, take env values:
             for key in keys_required:
```

### Comparing `OpenVulnQuery-1.31/openVulnQuery/_library/config.py` & `OpenVulnQuery-1.34/openVulnQuery/_library/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,9 +5,13 @@
 #  - Make API Calls
 
 # Enter your client ID and client secret below.  
 
 CLIENT_ID = ""
 CLIENT_SECRET = ""
 
-REQUEST_TOKEN_URL = "https://cloudsso.cisco.com/as/token.oauth2"
-API_URL = "https://api.cisco.com/security/advisories"
+#The following two URLs have changed.  See https://raw.githubusercontent.com/api-at-cisco/Images/master/Whats_New_Doc.pdf
+#REQUEST_TOKEN_URL = "https://cloudsso.cisco.com/as/token.oauth2"
+#API_URL = "https://api.cisco.com/security/advisories/v2"
+
+REQUEST_TOKEN_URL = "https://id.cisco.com/oauth2/default/v1/token"
+API_URL = "https://apix.cisco.com/security/advisories/v2"
```

### Comparing `OpenVulnQuery-1.31/openVulnQuery/_library/query_client.py` & `OpenVulnQuery-1.34/openVulnQuery/_library/query_client.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,45 +13,57 @@
 from . import rest_api
 
 ADV_TOKENS = constants.ADVISORY_FORMAT_TOKENS
 
 TEMPORAL_FILTER_KEYS = ('startDate', 'endDate')
 PUBLISHED_FIRST = 'firstpublished'
 PUBLISHED_LAST = 'lastpublished'
+PLATFORMALIAS = 'platformAlias'
+
 TEMPORAL_PUBLICATION_ASPECTS = (PUBLISHED_FIRST, PUBLISHED_LAST)
 
 DEBUG_API_USAGE = os.getenv('CISCO_OPEN_VULN_API_DEBUG', None)
 DEBUG_API_PATH = os.getenv('CISCO_OPEN_VULN_API_PATH', None)
 DEBUG_TIME_STAMP_FORMAT = "%Y%m%dT%H%M%S.%f"
 
 def ensure_adv_format_token(adv_format):
     return adv_format if adv_format in ADV_TOKENS else ADV_TOKENS[-1]
 
+
 class Filter(object):
     def __init__(self, path='', params=None):
         self.path = path
         self.params = params
 
 
 class TemporalFilter(object):
     def __init__(self, path, *args):
         self.path = path  # Better be in TEMPORAL_PUBLICATION_ASPECTS ...
         self.params = dict(zip(TEMPORAL_FILTER_KEYS, args))
 
+class OptionalParameters(object):
+    def __init__(self, parameter_name='', *args):
+        self.parameter_name = parameter_name
+        self.parameter_value = args
+
 
 class FirstPublished(TemporalFilter):
     def __init__(self, *args):
         super(FirstPublished, self).__init__(PUBLISHED_FIRST, *args)
 
 
 class LastUpdated(TemporalFilter):
     def __init__(self, *args):
         super(LastUpdated, self).__init__(PUBLISHED_LAST, *args)
 
 
+class PlatformAlias(OptionalParameters):
+    def __init__(self, *args):
+        super(PlatformAlias, self).__init__(PLATFORMALIAS, *args)
+
 class OpenVulnQueryClient(object):
     """Client sends get request for advisory information from OpenVuln API.
 
     :var auth_token: OAuth2 Token for API authorization.
     :var headers: Headers containing OAuth2 Token and data type for
      request.
     """
@@ -70,15 +82,15 @@
         self.logger = logging.getLogger(__name__)
         self.auth_url = auth_url if auth_url else config.REQUEST_TOKEN_URL
         self.auth_token = authorization.get_oauth_token(
             client_id, client_secret, request_token_url=self.auth_url)
         self.headers = rest_api.rest_with_auth_headers(
             self.auth_token, user_agent)
 
-    def get_by_all(self, adv_format, all_adv, a_filter):
+    def get_by_all(self, adv_format, all_adv, a_filter=None):
         """Return all the advisories using requested advisory format"""
         req_cfg = {
             'filter': a_filter.path,
         }
         req_path = "all/{filter}".format(**req_cfg)
         advisories = self.get_request(req_path, a_filter.params)
         return self.advisory_list(advisories['advisories'], adv_format)
@@ -88,14 +100,23 @@
         req_cfg = {
             'cve_id': cve_id,
         }
         req_path = "cve/{cve_id}".format(**req_cfg)
         advisories = self.get_request(req_path)
         return self.advisory_list(advisories['advisories'], adv_format)
 
+    def get_by_bugid(self, adv_format, bug_id, a_filter=None):
+        """Return the advisory using requested cve id"""
+        req_cfg = {
+            'bug_id': bug_id,
+        }
+        req_path = "bugid/{bug_id}".format(**req_cfg)
+        advisories = self.get_request(req_path)
+        return self.advisory_list(advisories['advisories'], adv_format)
+
     def get_by_advisory(self, adv_format, an_advisory, a_filter=None):
         """Return the advisory using requested advisory id"""
         req_cfg = {
             'advisory': an_advisory,
         }
         req_path = "advisory/{advisory}".format(**req_cfg)
         advisories = self.get_request(req_path)
@@ -142,75 +163,164 @@
         req_path = "product"
         advisories = self.get_request(
             req_path, params={'product': product_name})
         return self.advisory_list(advisories['advisories'], adv_format)
 
     def get_by_ios_xe(self, adv_format, ios_version, a_filter=None):
         """Return advisories by Cisco IOS advisories version"""
-        req_path = "iosxe"
+        req_path = "OSType/iosxe"
         try:
             advisories = self.get_request(
                 req_path,
                 params={'version': ios_version})
-            return self.advisory_list(advisories['advisories'], None)
+            return self.advisory_list(advisories['advisories'], adv_format)
         except requests.exceptions.HTTPError as e:
             raise requests.exceptions.HTTPError(
                 e.response.status_code, e.response.text)
 
     def get_by_ios(self, adv_format, ios_version, a_filter=None):
         """Return advisories by Cisco IOS advisories version"""
-        req_path = "ios"
+        req_path = "OSType/ios"
         try:
             advisories = self.get_request(
                 req_path,
                 params={'version': ios_version})
-            return self.advisory_list(advisories['advisories'], None)
+            return self.advisory_list(advisories['advisories'], adv_format)
         except requests.exceptions.HTTPError as e:
             raise requests.exceptions.HTTPError(
                 e.response.status_code, e.response.text)
 
     def get_by_nxos(self, adv_format, nxos_version, a_filter=None):
         """Return advisories by Cisco NX-OS (standalone mode) advisories version"""
-        req_path = "nxos"
+        req_path = "OSType/nxos"
         try:
-            advisories = self.get_request(
-                req_path,
-                params={'version': nxos_version})
-            return self.advisory_list(advisories['advisories'], None)
+            req_cfg = {
+                'version': nxos_version,
+                'platformAlias': '' if a_filter is None else a_filter.parameter_value,
+            }
+            advisories = self.get_request(req_path, req_cfg)
+            return self.advisory_list(advisories['advisories'], adv_format)
         except requests.exceptions.HTTPError as e:
             raise requests.exceptions.HTTPError(
                 e.response.status_code, e.response.text)
 
     def get_by_aci(self, adv_format, aci_version, a_filter=None):
         """Return advisories by Cisco NX-OS (in ACI mode) advisories version"""
-        req_path = "aci"
+        req_path = "OSType/aci"
         try:
             advisories = self.get_request(
                 req_path,
                 params={'version': aci_version})
-            return self.advisory_list(advisories['advisories'], None)
+            return self.advisory_list(advisories['advisories'], adv_format)
+        except requests.exceptions.HTTPError as e:
+            raise requests.exceptions.HTTPError(
+                e.response.status_code, e.response.text)
+            
+
+    def get_by_asa(self, adv_format, asa_version, a_filter=None):
+        """Return advisories by Cisco ASA advisories version"""
+        req_path = "OSType/asa"
+        try:
+            req_cfg = {
+                'version': asa_version,
+                'platformAlias': '' if a_filter is None else a_filter.parameter_value,
+            }
+            advisories = self.get_request(req_path, req_cfg)
+            return self.advisory_list(advisories['advisories'], adv_format)
+        except requests.exceptions.HTTPError as e:
+            raise requests.exceptions.HTTPError(
+                e.response.status_code, e.response.text)
+
+    def get_by_fmc(self, adv_format, fmc_version, a_filter=None):
+        """Return advisories by Cisco FMC advisories version"""
+        req_path = "OSType/fmc"
+        try:
+            advisories = self.get_request(
+                req_path,
+                params={'version': fmc_version})
+            return self.advisory_list(advisories['advisories'], adv_format)
+        except requests.exceptions.HTTPError as e:
+            raise requests.exceptions.HTTPError(
+                e.response.status_code, e.response.text)
+
+    def get_by_ftd(self, adv_format, ftd_version, a_filter=None):
+        """Return advisories by Cisco FTD advisories version"""
+        req_path = "OSType/ftd"
+        try:
+            req_cfg = {
+                'version': ftd_version,
+                'platformAlias': '' if a_filter is None else a_filter.parameter_value,
+            }
+            advisories = self.get_request(req_path, req_cfg)
+            return self.advisory_list(advisories['advisories'], adv_format)
+        except requests.exceptions.HTTPError as e:
+            raise requests.exceptions.HTTPError(
+                e.response.status_code, e.response.text)
+
+    def get_by_fxos(self, adv_format, fxos_version, a_filter=None):
+        """Return advisories by Cisco FXOS advisories version"""
+        req_path = "OSType/fxos"
+        try:
+            req_cfg = {
+                'version': fxos_version,
+                'platformAlias': '' if a_filter is None else a_filter.parameter_value,
+            }
+            advisories = self.get_request(req_path, req_cfg)
+            return self.advisory_list(advisories['advisories'], adv_format)
+        except requests.exceptions.HTTPError as e:
+            raise requests.exceptions.HTTPError(
+                e.response.status_code, e.response.text)            
+
+    def get_by_os(self, adv_format, os_type, a_filter=None):
+        """Return version information regarding the different Network Operating Systems."""
+        req_path = "OS_version/OS_data"
+        try:
+            NOS_Data = self.get_request(
+                req_path,
+                params={'OSType': os_type})
+            #Data is already a list of nost_type objects
+            return NOS_Data
+        except requests.exceptions.HTTPError as e:
+            raise requests.exceptions.HTTPError(
+                e.response.status_code, e.response.text)
+
+    def get_by_platform(self, adv_format, os_type, a_filter=None):
+        """Return platform information regarding the different Network Operating Systems."""
+        req_path = "platforms"
+        try:
+            platforms = self.get_request(
+                req_path,
+                params={'OSType': os_type})
+            #Data is already a list of platformAlias objects
+            return platforms
         except requests.exceptions.HTTPError as e:
             raise requests.exceptions.HTTPError(
                 e.response.status_code, e.response.text)
 
     def get_by(self, topic, format, aspect, **kwargs):
         """Cartesian product ternary paths biased REST dispatcher."""
         trampoline = {  # key: function; required and [optional] parameters
             'all': self.get_by_all,  # format, all_adv, a_filter
             'cve': self.get_by_cve,  # format, cve, [a_filter]
+            'bugid': self.get_by_bugid,  # format, bugid, [a_filter]
             'advisory': self.get_by_advisory,  # format, an_advisory,[a_filter]
             'severity': self.get_by_severity,  # format, severity, [a_filter]
             'year': self.get_by_year,  # format, year, [a_filter]
             'latest': self.get_by_latest,  # format, latest, [a_filter]
             'product': self.get_by_product,  # format, product_name, [a_filter]
             'ios_xe': self.get_by_ios_xe,  # 'ios', ios_version, [a_filter]
             'ios': self.get_by_ios,  # 'ios', ios_version, [a_filter]
             'nxos': self.get_by_nxos,  # 'ios', nxos_version, [a_filter]
             'aci': self.get_by_aci,  # 'ios', aci_version, [a_filter]
-
+            'asa': self.get_by_asa,  # 'ios', asa_version, [a_filter]
+            'fmc': self.get_by_fmc,  # 'ios', fmc_version, [a_filter]
+            'ftd': self.get_by_ftd,  # 'ios', ftd_version, [a_filter]
+            'fxos': self.get_by_fxos,  # 'ios', fxos_version, [a_filter]
+            'OS': self.get_by_os,  # format, OS_Type, 'none'
+            'platform': self.get_by_platform,  # format, OS_Type, 'none'
         }
         if topic not in trampoline:
             raise KeyError(
                 "REST API 'topic' ({}) not (yet) supported.".format(topic))
 
         return trampoline[topic](format, aspect, **kwargs)
```

### Comparing `OpenVulnQuery-1.31/openVulnQuery/_library/utils.py` & `OpenVulnQuery-1.34/openVulnQuery/_library/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,32 +3,41 @@
 import sys
 
 from . import constants
 from ._compatibility import is_unicode_or_bytes
 
 TAB = u'\t'
 IPS_SIG = constants.IPS_SIGNATURE_LABEL
-
+PLATFORMS_TAG = constants.PLATFORMS_LABEL
 
 def filter_advisories(advisories, fields):
     """Filter the advisories per some criteria ...
 
     :param advisories: An iterable with advisory entries
     :param fields: The requested fields (TODO reverse documentation?)
     :return list of advisories passing filter criteria
     """
     is_nested_ips_signature_field = any(
         field in constants.IPS_SIGNATURES for field in fields)
 
+    is_nested_platforms_field = any(
+        field in constants.PLATFORMS for field in fields)
+
     filter_fields = list(fields)
+
     if is_nested_ips_signature_field:
         filter_fields.append(IPS_SIG)
     elif IPS_SIG in fields:  # and not is_nested_ips_signature_field:
         filter_fields.extend(constants.IPS_SIGNATURES)
 
+    if is_nested_platforms_field:
+        filter_fields.append(PLATFORMS_TAG)
+    elif PLATFORMS_TAG in fields:
+        filter_fields.extend(constants.PLATFORMS)
+
     return [adv.filter(*filter_fields) for adv in advisories]
 
 
 def count_fields(advisories, fields):
     """Counter dict from fields over all advisories. """
     counts = dict.fromkeys(fields, 0)
     for adv in advisories:
```

### Comparing `OpenVulnQuery-1.31/setup.py` & `OpenVulnQuery-1.34/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name='OpenVulnQuery',
-      version='1.31',
+      version='1.34',
       description='A python-based module(s) to query the Cisco PSIRT openVuln API.',
       long_description=long_description,
       long_description_content_type="text/markdown",
-      url='https://github.com/CiscoPSIRT/openVulnAPI/tree/master/openVulnQuery',
+      url='https://github.com/CiscoPSIRT/openVulnQuery',
       author=' Omar Santos',
       author_email='os@cisco.com',
       license='The MIT License (MIT)',
       packages=find_packages(exclude=["tests"]),
       entry_points={
           'console_scripts':
               ['openVulnQuery=openVulnQuery.main:main']
```

