# Comparing `tmp/accentnotifications-0.0.3.tar.gz` & `tmp/accentnotifications-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accentnotifications-0.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "accentnotifications-0.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `accentnotifications-0.0.3.tar` & `accentnotifications-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       99 2022-10-05 10:37:49.000000 accentnotifications-0.0.3/.flake8
--rw-r--r--   0        0        0      929 2023-07-17 11:26:35.290624 accentnotifications-0.0.3/.github/workflows/test.yml
--rw-r--r--   0        0        0      109 2023-07-17 09:30:14.313081 accentnotifications-0.0.3/.gitignore
--rw-r--r--   0        0        0     1089 2022-10-07 18:12:15.000000 accentnotifications-0.0.3/LICENSE
--rw-r--r--   0        0        0      490 2023-07-17 09:30:14.314070 accentnotifications-0.0.3/README.md
--rw-r--r--   0        0        0       81 2023-07-17 11:28:59.265857 accentnotifications-0.0.3/accentnotifications/__init__.py
--rw-r--r--   0        0        0      246 2022-10-12 08:48:23.000000 accentnotifications-0.0.3/accentnotifications/manager.py
--rw-r--r--   0        0        0      112 2023-07-17 09:30:14.314592 accentnotifications-0.0.3/accentnotifications/notifications/__init__.py
--rw-r--r--   0        0        0      897 2023-07-17 11:16:34.607700 accentnotifications-0.0.3/accentnotifications/notifications/base.py
--rw-r--r--   0        0        0     2845 2023-07-17 11:16:33.855651 accentnotifications-0.0.3/accentnotifications/notifications/smtp.py
--rw-r--r--   0        0        0     3038 2023-07-17 11:16:34.605170 accentnotifications-0.0.3/accentnotifications/notifications/twilio_sms.py
--rw-r--r--   0        0        0     1670 2023-07-17 11:16:15.640920 accentnotifications-0.0.3/accentnotifications/types.py
--rw-r--r--   0        0        0     1363 2023-07-17 09:34:24.491649 accentnotifications-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1640 1970-01-01 00:00:00.000000 accentnotifications-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       99 2022-10-05 10:37:49.000000 accentnotifications-0.0.4/.flake8
+-rw-r--r--   0        0        0      929 2023-07-17 11:26:35.290624 accentnotifications-0.0.4/.github/workflows/test.yml
+-rw-r--r--   0        0        0      109 2023-07-17 09:30:14.313081 accentnotifications-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1089 2022-10-07 18:12:15.000000 accentnotifications-0.0.4/LICENSE
+-rw-r--r--   0        0        0      490 2023-07-17 09:30:14.314070 accentnotifications-0.0.4/README.md
+-rw-r--r--   0        0        0       81 2023-08-06 00:34:18.492627 accentnotifications-0.0.4/accentnotifications/__init__.py
+-rw-r--r--   0        0        0      246 2022-10-12 08:48:23.000000 accentnotifications-0.0.4/accentnotifications/manager.py
+-rw-r--r--   0        0        0      112 2023-07-17 09:30:14.314592 accentnotifications-0.0.4/accentnotifications/notifications/__init__.py
+-rw-r--r--   0        0        0      897 2023-07-17 11:16:34.607700 accentnotifications-0.0.4/accentnotifications/notifications/base.py
+-rw-r--r--   0        0        0     2845 2023-07-17 11:16:33.855651 accentnotifications-0.0.4/accentnotifications/notifications/smtp.py
+-rw-r--r--   0        0        0     3038 2023-07-17 11:16:34.605170 accentnotifications-0.0.4/accentnotifications/notifications/twilio_sms.py
+-rw-r--r--   0        0        0     1670 2023-07-17 11:16:15.640920 accentnotifications-0.0.4/accentnotifications/types.py
+-rw-r--r--   0        0        0     1363 2023-08-06 00:33:57.301595 accentnotifications-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1640 1970-01-01 00:00:00.000000 accentnotifications-0.0.4/PKG-INFO
```

### Comparing `accentnotifications-0.0.3/.github/workflows/test.yml` & `accentnotifications-0.0.4/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `accentnotifications-0.0.3/LICENSE` & `accentnotifications-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `accentnotifications-0.0.3/accentnotifications/notifications/base.py` & `accentnotifications-0.0.4/accentnotifications/notifications/base.py`

 * *Files identical despite different names*

### Comparing `accentnotifications-0.0.3/accentnotifications/notifications/smtp.py` & `accentnotifications-0.0.4/accentnotifications/notifications/smtp.py`

 * *Files identical despite different names*

### Comparing `accentnotifications-0.0.3/accentnotifications/notifications/twilio_sms.py` & `accentnotifications-0.0.4/accentnotifications/notifications/twilio_sms.py`

 * *Files identical despite different names*

### Comparing `accentnotifications-0.0.3/accentnotifications/types.py` & `accentnotifications-0.0.4/accentnotifications/types.py`

 * *Files identical despite different names*

### Comparing `accentnotifications-0.0.3/pyproject.toml` & `accentnotifications-0.0.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python",
 ]
 dependencies = [
-    "pydantic>=2.0.1,<2.1.0",
+    "pydantic>=2.0.1,<2.2.0",
     "pydantic-settings>=2.0.1,<2.1.0",
 ]
 dynamic = ["version", "description"]
 
 [project.urls]
 Homepage = "https://github.com/accentdesign/accentnotifications"
```

### Comparing `accentnotifications-0.0.3/PKG-INFO` & `accentnotifications-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: accentnotifications
-Version: 0.0.3
+Version: 0.0.4
 Summary: Sending various forms of notifications such as smtp
 Author-email: Accent Design Group Ltd <support@accentdesign.co.uk>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python
-Requires-Dist: pydantic>=2.0.1,<2.1.0
+Requires-Dist: pydantic>=2.0.1,<2.2.0
 Requires-Dist: pydantic-settings>=2.0.1,<2.1.0
 Requires-Dist: autoflake ; extra == "dev"
 Requires-Dist: flake8 ; extra == "dev"
 Requires-Dist: aiosmtplib ; extra == "smtp"
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: pytest-asyncio ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: accentnotifications Version: 0.0.3 Summary: Sending
+Metadata-Version: 2.1 Name: accentnotifications Version: 0.0.4 Summary: Sending
 various forms of notifications such as smtp Author-email: Accent Design Group
 Ltd
 accentdesign.co.uk> Requires-Python: >=3.9 Description-Content-Type: text/
 markdown Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-Requires-Dist: pydantic>=2.0.1,<2.1.0 Requires-Dist: pydantic-
+Requires-Dist: pydantic>=2.0.1,<2.2.0 Requires-Dist: pydantic-
 settings>=2.0.1,<2.1.0 Requires-Dist: autoflake ; extra == "dev" Requires-Dist:
 flake8 ; extra == "dev" Requires-Dist: aiosmtplib ; extra == "smtp" Requires-
 Dist: pytest ; extra == "test" Requires-Dist: pytest-asyncio ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test" Requires-Dist: pytest-mock ; extra
 == "test" Requires-Dist: mypy ; extra == "test" Requires-Dist: flake8 ; extra
 == "test" Requires-Dist: black ; extra == "test" Requires-Dist: isort ; extra
 == "test" Requires-Dist: aiohttp ; extra == "twiliosms" Project-URL: Homepage,
```

