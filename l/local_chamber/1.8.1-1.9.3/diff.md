# Comparing `tmp/local_chamber-1.8.1.tar.gz` & `tmp/local_chamber-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "local_chamber-1.8.1.tar", last modified: Sun Oct 30 18:41:08 2022, max compression
+gzip compressed data, was "local_chamber-1.9.3.tar", last modified: Sun Mar 26 10:20:06 2023, max compression
```

## Comparing `local_chamber-1.8.1.tar` & `local_chamber-1.9.3.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0      589 2022-03-28 22:04:20.160000 local_chamber-1.8.1/.circleci/config.yml
--rw-r--r--   0        0        0     1250 2022-06-18 09:40:21.060000 local_chamber-1.8.1/.gitignore
--rw-r--r--   0        0        0     1071 2022-03-16 08:26:57.202608 local_chamber-1.8.1/LICENSE
--rw-r--r--   0        0        0      478 2022-06-03 17:23:06.010000 local_chamber-1.8.1/Makefile
--rw-r--r--   0        0        0      990 2022-06-03 17:29:42.740000 local_chamber-1.8.1/README.md
--rwxr-xr-x   0        0        0     1869 2022-10-18 11:15:02.570000 local_chamber-1.8.1/configure
--rw-r--r--   0        0        0      614 2022-03-16 08:26:57.252608 local_chamber-1.8.1/docs/Makefile
--rw-r--r--   0        0        0       91 2022-03-16 08:26:57.242608 local_chamber-1.8.1/docs/cli.rst
--rwxr-xr-x   0        0        0     4941 2022-03-23 18:10:05.530000 local_chamber-1.8.1/docs/conf.py
--rw-r--r--   0        0        0       33 2022-03-16 08:26:57.252608 local_chamber-1.8.1/docs/contributing.rst
--rw-r--r--   0        0        0       28 2022-03-16 08:26:57.252608 local_chamber-1.8.1/docs/history.rst
--rw-r--r--   0        0        0      297 2022-03-16 08:26:57.242608 local_chamber-1.8.1/docs/index.rst
--rw-r--r--   0        0        0     1150 2022-03-16 08:26:57.242608 local_chamber-1.8.1/docs/installation.rst
--rw-r--r--   0        0        0      657 2022-06-03 17:13:49.450000 local_chamber-1.8.1/docs/local_chamber.rst
--rw-r--r--   0        0        0      775 2022-03-16 08:26:57.242608 local_chamber-1.8.1/docs/make.bat
--rw-r--r--   0        0        0       76 2022-06-03 17:25:29.660000 local_chamber-1.8.1/docs/modules.rst
--rw-r--r--   0        0        0       27 2022-03-16 08:26:57.252608 local_chamber-1.8.1/docs/readme.rst
--rw-r--r--   0        0        0       71 2022-03-17 08:36:16.062608 local_chamber-1.8.1/docs/requirements.txt
--rw-r--r--   0        0        0      318 2022-10-28 22:30:14.190000 local_chamber-1.8.1/local_chamber/__init__.py
--rw-r--r--   0        0        0      193 2022-06-03 17:06:34.560000 local_chamber-1.8.1/local_chamber/__main__.py
--rwxr-xr-x   0        0        0     2690 2022-10-29 14:56:56.040000 local_chamber-1.8.1/local_chamber/archive.py
--rw-r--r--   0        0        0    17708 2022-10-29 20:46:17.590000 local_chamber-1.8.1/local_chamber/chamber.py
--rw-r--r--   0        0        0    11626 2022-10-30 18:34:03.880000 local_chamber-1.8.1/local_chamber/cli.py
--rw-r--r--   0        0        0       40 2022-10-18 12:51:58.110000 local_chamber-1.8.1/local_chamber/exception.py
--rw-r--r--   0        0        0      960 2022-10-18 11:15:02.580000 local_chamber-1.8.1/local_chamber/shell.py
--rwxr-xr-x   0        0        0     3847 2022-10-29 14:57:09.360000 local_chamber-1.8.1/local_chamber/vault.py
--rw-r--r--   0        0        0      127 2022-10-30 18:37:30.000000 local_chamber-1.8.1/local_chamber/version.py
--rw-r--r--   0        0        0      289 2022-03-16 08:26:57.262608 local_chamber-1.8.1/make.include/browser.mk
--rw-r--r--   0        0        0      608 2022-03-16 08:26:57.252608 local_chamber-1.8.1/make.include/clean.mk
--rw-r--r--   0        0        0     1860 2022-06-03 17:18:18.100000 local_chamber-1.8.1/make.include/common.mk
--rw-r--r--   0        0        0      508 2022-06-03 17:25:22.790000 local_chamber-1.8.1/make.include/docs.mk
--rw-r--r--   0        0        0      249 2022-06-03 17:19:52.310000 local_chamber-1.8.1/make.include/lint.mk
--rw-r--r--   0        0        0     1688 2022-06-03 17:16:55.220000 local_chamber-1.8.1/make.include/publish.mk
--rw-r--r--   0        0        0     1118 2022-10-28 21:18:03.080000 local_chamber-1.8.1/make.include/test.mk
--rw-r--r--   0        0        0      977 2022-06-03 17:18:40.090000 local_chamber-1.8.1/make.include/version.mk
--rw-r--r--   0        0        0     1357 2022-10-27 20:41:20.600000 local_chamber-1.8.1/pyproject.toml
--rw-r--r--   0        0        0      231 2022-03-16 08:26:57.212608 local_chamber-1.8.1/pytest.ini
--rwxr-xr-x   0        0        0     1845 2022-10-18 11:15:02.580000 local_chamber-1.8.1/scripts/testinit
--rw-r--r--   0        0        0       43 2022-03-16 08:26:57.242608 local_chamber-1.8.1/tests/__init__.py
--rw-r--r--   0        0        0     1578 2022-10-29 20:31:02.260000 local_chamber-1.8.1/tests/conftest.py
--rw-r--r--   0        0        0       15 2022-03-16 15:28:35.212608 local_chamber-1.8.1/tests/data/secrets-test/-/commastr
--rw-r--r--   0        0        0        3 2022-03-16 15:28:35.212608 local_chamber-1.8.1/tests/data/secrets-test/-/foo
--rw-r--r--   0        0        0        5 2022-03-16 15:28:35.212608 local_chamber-1.8.1/tests/data/secrets-test/-/key
--rw-r--r--   0        0        0        5 2022-03-16 15:28:35.212608 local_chamber-1.8.1/tests/data/secrets-test/-/version
--rw-r--r--   0        0        0       13 2022-03-16 15:28:35.212608 local_chamber-1.8.1/tests/data/secrets-test/-/words
--rw-r--r--   0        0        0      293 2022-10-18 11:27:25.510000 local_chamber-1.8.1/tests/data/secrets.json
--rw-r--r--   0        0        0        3 2022-03-17 06:59:33.922608 local_chamber-1.8.1/tests/data/secrets/testservice/dynakey
--rw-r--r--   0        0        0        3 2022-03-17 06:59:33.922608 local_chamber-1.8.1/tests/data/secrets/testservice/fookey
--rw-r--r--   0        0        0        6 2022-04-02 21:31:22.470000 local_chamber-1.8.1/tests/data/secrets/testservice/key1
--rw-r--r--   0        0        0       13 2022-03-17 06:59:33.922608 local_chamber-1.8.1/tests/data/secrets/testservice/key_multiword
--rw-r--r--   0        0        0        7 2022-03-16 20:05:47.392608 local_chamber-1.8.1/tests/data/secrets/testservice/sub1/key1
--rw-r--r--   0        0        0        7 2022-03-16 20:05:55.812608 local_chamber-1.8.1/tests/data/secrets/testservice/sub1/key2
--rw-r--r--   0        0        0        7 2022-03-16 20:05:41.042608 local_chamber-1.8.1/tests/data/secrets/testservice/sub2/key1
--rw-r--r--   0        0        0        6 2022-03-16 15:17:17.432608 local_chamber-1.8.1/tests/data/secrets/testservice/sub2/key2
--rw-r--r--   0        0        0        5 2022-03-17 06:59:33.922608 local_chamber-1.8.1/tests/data/secrets/testservice/testkey
--rw-r--r--   0        0        0       77 2022-03-16 20:26:00.452608 local_chamber-1.8.1/tests/data/test.csv
--rw-r--r--   0        0        0       87 2022-03-16 20:26:00.792608 local_chamber-1.8.1/tests/data/test.dotenv
--rw-r--r--   0        0        0       99 2022-03-16 20:26:01.112608 local_chamber-1.8.1/tests/data/test.json
--rw-r--r--   0        0        0       97 2022-03-16 20:26:01.432608 local_chamber-1.8.1/tests/data/test.tfvars
--rw-r--r--   0        0        0       77 2022-03-16 20:26:01.792608 local_chamber-1.8.1/tests/data/test.tsv
--rw-r--r--   0        0        0       82 2022-03-16 20:26:02.122608 local_chamber-1.8.1/tests/data/test.yaml
--rw-r--r--   0        0        0       99 2022-03-16 20:27:42.662608 local_chamber-1.8.1/tests/data/testservice.json
--rw-r--r--   0        0        0     2163 2022-10-29 20:31:02.290000 local_chamber-1.8.1/tests/test_archive.py
--rw-r--r--   0        0        0     8981 2022-10-29 20:31:02.390000 local_chamber-1.8.1/tests/test_cli.py
--rw-r--r--   0        0        0    16742 2022-10-29 20:50:12.550000 local_chamber-1.8.1/tests/test_local_chamber.py
--rw-r--r--   0        0        0      391 2022-10-18 11:15:02.580000 local_chamber-1.8.1/tox.ini
--rw-r--r--   0        0        0     2344 1970-01-01 00:00:00.000000 local_chamber-1.8.1/PKG-INFO
+-rw-r--r--   0        0        0      589 2022-08-22 20:15:20.596645 local_chamber-1.9.3/.circleci/config.yml
+-rw-r--r--   0        0        0     1256 2023-03-12 21:03:05.950632 local_chamber-1.9.3/.gitignore
+-rw-r--r--   0        0        0     1071 2022-08-22 20:15:20.596645 local_chamber-1.9.3/LICENSE
+-rw-r--r--   0        0        0      478 2022-08-22 20:15:20.596645 local_chamber-1.9.3/Makefile
+-rw-r--r--   0        0        0      990 2022-08-22 20:15:20.596645 local_chamber-1.9.3/README.md
+-rwxr-xr-x   0        0        0     1869 2022-08-25 13:55:35.066098 local_chamber-1.9.3/configure
+-rw-r--r--   0        0        0      614 2022-08-22 20:15:20.596645 local_chamber-1.9.3/docs/Makefile
+-rw-r--r--   0        0        0       91 2022-08-22 20:15:20.596645 local_chamber-1.9.3/docs/cli.rst
+-rwxr-xr-x   0        0        0     4941 2022-08-22 20:15:20.596645 local_chamber-1.9.3/docs/conf.py
+-rw-r--r--   0        0        0       33 2022-08-22 20:15:20.596645 local_chamber-1.9.3/docs/contributing.rst
+-rw-r--r--   0        0        0       28 2022-08-22 20:15:20.596645 local_chamber-1.9.3/docs/history.rst
+-rw-r--r--   0        0        0      297 2022-08-22 20:15:20.596645 local_chamber-1.9.3/docs/index.rst
+-rw-r--r--   0        0        0     1150 2022-08-22 20:15:20.596645 local_chamber-1.9.3/docs/installation.rst
+-rw-r--r--   0        0        0      657 2022-08-22 20:15:20.596645 local_chamber-1.9.3/docs/local_chamber.rst
+-rw-r--r--   0        0        0      775 2022-08-22 20:15:20.596645 local_chamber-1.9.3/docs/make.bat
+-rw-r--r--   0        0        0       76 2022-08-22 20:15:20.596645 local_chamber-1.9.3/docs/modules.rst
+-rw-r--r--   0        0        0       27 2022-08-22 20:15:20.596645 local_chamber-1.9.3/docs/readme.rst
+-rw-r--r--   0        0        0       71 2022-08-22 20:15:20.596645 local_chamber-1.9.3/docs/requirements.txt
+-rw-r--r--   0        0        0      318 2022-08-26 05:45:30.662697 local_chamber-1.9.3/local_chamber/__init__.py
+-rw-r--r--   0        0        0      193 2022-08-22 20:15:20.596645 local_chamber-1.9.3/local_chamber/__main__.py
+-rwxr-xr-x   0        0        0     2690 2023-03-12 20:38:13.825216 local_chamber-1.9.3/local_chamber/archive.py
+-rw-r--r--   0        0        0    17708 2023-03-12 20:59:11.445629 local_chamber-1.9.3/local_chamber/chamber.py
+-rw-r--r--   0        0        0    11648 2023-03-12 21:41:14.048844 local_chamber-1.9.3/local_chamber/cli.py
+-rw-r--r--   0        0        0       40 2023-03-12 20:38:13.825216 local_chamber-1.9.3/local_chamber/exception.py
+-rw-r--r--   0        0        0      960 2022-08-26 10:28:26.017874 local_chamber-1.9.3/local_chamber/shell.py
+-rwxr-xr-x   0        0        0     3847 2023-03-12 20:38:13.825216 local_chamber-1.9.3/local_chamber/vault.py
+-rw-r--r--   0        0        0      127 2023-03-26 10:16:14.496564 local_chamber-1.9.3/local_chamber/version.py
+-rw-r--r--   0        0        0      289 2022-08-22 20:15:20.596645 local_chamber-1.9.3/make.include/browser.mk
+-rw-r--r--   0        0        0      608 2022-08-22 20:15:20.596645 local_chamber-1.9.3/make.include/clean.mk
+-rw-r--r--   0        0        0     1860 2022-08-22 20:15:20.596645 local_chamber-1.9.3/make.include/common.mk
+-rw-r--r--   0        0        0      508 2022-08-22 20:15:20.596645 local_chamber-1.9.3/make.include/docs.mk
+-rw-r--r--   0        0        0      284 2023-03-12 21:02:40.458958 local_chamber-1.9.3/make.include/lint.mk
+-rw-r--r--   0        0        0     1688 2022-08-25 14:11:44.882827 local_chamber-1.9.3/make.include/publish.mk
+-rw-r--r--   0        0        0     1118 2023-03-12 20:38:13.825216 local_chamber-1.9.3/make.include/test.mk
+-rw-r--r--   0        0        0      977 2022-08-26 06:17:13.623016 local_chamber-1.9.3/make.include/version.mk
+-rw-r--r--   0        0        0     1310 2023-03-26 10:09:03.353675 local_chamber-1.9.3/pyproject.toml
+-rw-r--r--   0        0        0      231 2022-08-22 20:15:20.596645 local_chamber-1.9.3/pytest.ini
+-rwxr-xr-x   0        0        0     1845 2022-08-26 05:35:37.924458 local_chamber-1.9.3/scripts/testinit
+-rw-r--r--   0        0        0       43 2022-08-22 20:15:20.596645 local_chamber-1.9.3/tests/__init__.py
+-rw-r--r--   0        0        0     1578 2023-03-12 20:38:13.825216 local_chamber-1.9.3/tests/conftest.py
+-rw-r--r--   0        0        0       15 2022-08-22 20:15:20.596645 local_chamber-1.9.3/tests/data/secrets-test/-/commastr
+-rw-r--r--   0        0        0        3 2022-08-22 20:15:20.596645 local_chamber-1.9.3/tests/data/secrets-test/-/foo
+-rw-r--r--   0        0        0        5 2022-08-22 20:15:20.596645 local_chamber-1.9.3/tests/data/secrets-test/-/key
+-rw-r--r--   0        0        0        5 2022-08-22 20:15:20.596645 local_chamber-1.9.3/tests/data/secrets-test/-/version
+-rw-r--r--   0        0        0       13 2022-08-22 20:15:20.596645 local_chamber-1.9.3/tests/data/secrets-test/-/words
+-rw-r--r--   0        0        0      293 2022-08-26 02:17:36.403644 local_chamber-1.9.3/tests/data/secrets.json
+-rw-r--r--   0        0        0        3 2022-08-22 20:15:20.596645 local_chamber-1.9.3/tests/data/secrets/testservice/dynakey
+-rw-r--r--   0        0        0        3 2022-08-22 20:15:20.596645 local_chamber-1.9.3/tests/data/secrets/testservice/fookey
+-rw-r--r--   0        0        0        6 2022-08-22 20:15:20.596645 local_chamber-1.9.3/tests/data/secrets/testservice/key1
+-rw-r--r--   0        0        0       13 2022-08-22 20:15:20.596645 local_chamber-1.9.3/tests/data/secrets/testservice/key_multiword
+-rw-r--r--   0        0        0        7 2022-08-22 20:15:20.596645 local_chamber-1.9.3/tests/data/secrets/testservice/sub1/key1
+-rw-r--r--   0        0        0        7 2022-08-22 20:15:20.596645 local_chamber-1.9.3/tests/data/secrets/testservice/sub1/key2
+-rw-r--r--   0        0        0        7 2022-08-22 20:15:20.596645 local_chamber-1.9.3/tests/data/secrets/testservice/sub2/key1
+-rw-r--r--   0        0        0        6 2022-08-22 20:15:20.596645 local_chamber-1.9.3/tests/data/secrets/testservice/sub2/key2
+-rw-r--r--   0        0        0        5 2022-08-22 20:15:20.596645 local_chamber-1.9.3/tests/data/secrets/testservice/testkey
+-rw-r--r--   0        0        0       77 2022-08-22 20:15:20.596645 local_chamber-1.9.3/tests/data/test.csv
+-rw-r--r--   0        0        0       87 2022-08-22 20:15:20.596645 local_chamber-1.9.3/tests/data/test.dotenv
+-rw-r--r--   0        0        0       99 2022-08-22 22:24:14.477611 local_chamber-1.9.3/tests/data/test.json
+-rw-r--r--   0        0        0       97 2022-08-22 20:15:20.596645 local_chamber-1.9.3/tests/data/test.tfvars
+-rw-r--r--   0        0        0       77 2022-08-22 20:15:20.596645 local_chamber-1.9.3/tests/data/test.tsv
+-rw-r--r--   0        0        0       82 2022-08-22 20:15:20.596645 local_chamber-1.9.3/tests/data/test.yaml
+-rw-r--r--   0        0        0       99 2022-08-22 20:15:20.596645 local_chamber-1.9.3/tests/data/testservice.json
+-rw-r--r--   0        0        0     2163 2023-03-12 20:38:13.825216 local_chamber-1.9.3/tests/test_archive.py
+-rw-r--r--   0        0        0     9929 2023-03-26 10:15:36.245023 local_chamber-1.9.3/tests/test_cli.py
+-rw-r--r--   0        0        0    16672 2023-03-12 20:59:11.421630 local_chamber-1.9.3/tests/test_local_chamber.py
+-rw-r--r--   0        0        0      391 2022-08-25 13:58:53.460755 local_chamber-1.9.3/tox.ini
+-rw-r--r--   0        0        0     2324 1970-01-01 00:00:00.000000 local_chamber-1.9.3/PKG-INFO
```

### Comparing `local_chamber-1.8.1/.circleci/config.yml` & `local_chamber-1.9.3/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `local_chamber-1.8.1/.gitignore` & `local_chamber-1.9.3/.gitignore`

 * *Files 8% similar despite different names*

```diff
@@ -106,7 +106,8 @@
 .idea/
 
 # locals
 .dist
 .timestamp
 notes
 postactivate
+.lint
```

### Comparing `local_chamber-1.8.1/LICENSE` & `local_chamber-1.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `local_chamber-1.8.1/README.md` & `local_chamber-1.9.3/README.md`

 * *Files identical despite different names*

### Comparing `local_chamber-1.8.1/configure` & `local_chamber-1.9.3/configure`

 * *Files identical despite different names*

### Comparing `local_chamber-1.8.1/docs/Makefile` & `local_chamber-1.9.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `local_chamber-1.8.1/docs/conf.py` & `local_chamber-1.9.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `local_chamber-1.8.1/docs/installation.rst` & `local_chamber-1.9.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `local_chamber-1.8.1/docs/local_chamber.rst` & `local_chamber-1.9.3/docs/local_chamber.rst`

 * *Files identical despite different names*

### Comparing `local_chamber-1.8.1/docs/make.bat` & `local_chamber-1.9.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `local_chamber-1.8.1/local_chamber/archive.py` & `local_chamber-1.9.3/local_chamber/archive.py`

 * *Files identical despite different names*

### Comparing `local_chamber-1.8.1/local_chamber/chamber.py` & `local_chamber-1.9.3/local_chamber/chamber.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,15 @@
         """Print the secrets from the secrets directory in a format to export as environment variables"""  # noqa
         service = self._verify_service(service)
         if service:
             secrets = self._secrets(service)
             self.echo("\n".join(sorted([self._export(k, v) for k, v in secrets.items()])))
         return 0
 
-    def _exec(self, *, services, cmd, pristine=False, strict_value='chamberme', child=True, buffer_output=True):
+    def _exec(self, *, services, cmd, pristine=False, strict_value="chamberme", child=True, buffer_output=True):
         """Executes a command with secrets loaded into the environment"""
         if not cmd:
             raise ChamberError("Error: must specify command to run. See usage: requires at least 1 arg(s), only received 0")  # noqa
         env = dict(environ).copy()
         if strict_value:
             # strict_vars must be filled from services or raise error
             strict_vars = [k for k, v in env.items() if v == strict_value]
```

### Comparing `local_chamber-1.8.1/local_chamber/cli.py` & `local_chamber-1.9.3/local_chamber/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,14 +65,15 @@
     is_flag=True,
     help="debug mode, output detailed error diagnostics",
 )
 @click.option(
     "-b",
     "--backend",
     envvar="SECRETS_BACKEND",
+    show_envvar=True,
     default="vault",
     type=click.Choice(list(BACKENDS.keys())),
     help="selected backend system",
 )
 @click.option(
     "-e/-E",
     "--exists/--if-exists",
```

### Comparing `local_chamber-1.8.1/local_chamber/shell.py` & `local_chamber-1.9.3/local_chamber/shell.py`

 * *Files identical despite different names*

### Comparing `local_chamber-1.8.1/local_chamber/vault.py` & `local_chamber-1.9.3/local_chamber/vault.py`

 * *Files identical despite different names*

### Comparing `local_chamber-1.8.1/make.include/clean.mk` & `local_chamber-1.9.3/make.include/clean.mk`

 * *Files identical despite different names*

### Comparing `local_chamber-1.8.1/make.include/common.mk` & `local_chamber-1.9.3/make.include/common.mk`

 * *Files identical despite different names*

### Comparing `local_chamber-1.8.1/make.include/publish.mk` & `local_chamber-1.9.3/make.include/publish.mk`

 * *Files identical despite different names*

### Comparing `local_chamber-1.8.1/make.include/test.mk` & `local_chamber-1.9.3/make.include/test.mk`

 * *Files identical despite different names*

### Comparing `local_chamber-1.8.1/make.include/version.mk` & `local_chamber-1.9.3/make.include/version.mk`

 * *Files identical despite different names*

### Comparing `local_chamber-1.8.1/pyproject.toml` & `local_chamber-1.9.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -19,31 +19,32 @@
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10"
 ]
 dynamic = ["version", "description"] 
 
 dependencies = [
-  "click==8.1.3",
-  "hvac==0.11.2",
-  "pyyaml==5.4.1"
+  "click>=8.1.3",
+  "hvac>=0.11.2",
+  "pyyaml>=5.4.1"
 ]
 
 [project.optional-dependencies]
 dev = [
-  "black==22.3.0",
-  "bump2version==1.0.1",
-  "coverage==6.4.1",
-  "flake8==4.0.1",
-  "flit==3.7.1",
+  "black",
+  "bump2version",
+  "coverage",
+  "flake8",
+  "flit",
+  "isort",
   "pdbpp",
-  "pytest==7.1.2",
+  "pytest",
   "pytest-click",
-  "pytest-datadir==1.3.1",
-  "tox==3.25.0"
+  "pytest-datadir",
+  "tox"
 ]
 docs = [
   "sphinx==5.0.1",
   "sphinx-click==4.1.0",
   "sphinx-rtd-theme==1.0.0"
 ]
```

### Comparing `local_chamber-1.8.1/scripts/testinit` & `local_chamber-1.9.3/scripts/testinit`

 * *Files identical despite different names*

### Comparing `local_chamber-1.8.1/tests/conftest.py` & `local_chamber-1.9.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `local_chamber-1.8.1/tests/test_archive.py` & `local_chamber-1.9.3/tests/test_archive.py`

 * *Files identical despite different names*

### Comparing `local_chamber-1.8.1/tests/test_cli.py` & `local_chamber-1.9.3/tests/test_cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 import json
 import os
 import pdb
 import sys
 from logging import getLogger
 from subprocess import check_output
+from uuid import uuid4
 
 import click
 import pytest
 from click.testing import Result
 
 from local_chamber import ChamberError, __version__, cli
 from local_chamber.cli import SysArgs
@@ -281,7 +282,31 @@
 
     test3 = check_output(f"ls {str(shared_datadir)}/tardis", shell=True, text=True)
     assert "daleks.tgz" in test3
 
     checkdir = shared_datadir / "tardis"
     tbs = [i for i in checkdir.iterdir() if i.is_file() and i.suffix == ".tgz"]
     assert len(tbs) == 2
+
+
+def test_cli_backend_env(runner, shared_datadir):
+    secrets_file = shared_datadir / "cli_backend_env.json"
+    secrets = {
+        "service1": {"key1": str(uuid4()), "key2": str(uuid4()), "key3": str(uuid4())},
+        "service2": {"key1": str(uuid4()), "key2": str(uuid4()), "key3": str(uuid4())},
+    }
+    secrets_file.write_text(json.dumps(secrets))
+    env = {k: v for k, v in os.environ.items()}
+    env["SECRETS_BACKEND"] = "file"
+    env["SECRETS_FILE"] = str(secrets_file)
+
+    result = runner(["list-services"], env=env)
+    services = result.output.split()
+    assert services[0] == "Service"
+    services.pop(0)
+    assert set(services) == set(["service1", "service2"])
+
+    result = runner(["-b", "file", "-f", str(secrets_file), "list-services"], env=env)
+    services = result.output.split()
+    assert services[0] == "Service"
+    services.pop(0)
+    assert set(services) == set(["service1", "service2"])
```

### Comparing `local_chamber-1.8.1/tests/test_local_chamber.py` & `local_chamber-1.9.3/tests/test_local_chamber.py`

 * *Files 0% similar despite different names*

```diff
@@ -406,21 +406,15 @@
     assert proc.returncode == 0
     before = lines(capfd)
     # before = proc.stdout.strip().split()
 
     after_cmd = ["env"]
     capfd.readouterr()
     with chamber_class(config=config, debug=True, echo=_echo, require_exists=True) as chamber:
-        ret = chamber._exec(
-            pristine=True,
-            strict_value=None,
-            services=["testservice"],
-            cmd=after_cmd,
-            buffer_output=False
-        )
+        ret = chamber._exec(pristine=True, strict_value=None, services=["testservice"], cmd=after_cmd, buffer_output=False)
     assert ret == 0
     after = lines(capfd)
 
     diff = set(after).difference(set(before))
     pprint(diff)
 
     verify_testservice = json.loads(testservice_json.read_text())
```

### Comparing `local_chamber-1.8.1/PKG-INFO` & `local_chamber-1.9.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 Metadata-Version: 2.1
 Name: local_chamber
-Version: 1.8.1
+Version: 1.9.3
 Summary: Top-level package for local-chamber.
 Keywords: local-chamber
 Author-email: Matt Krueger <mkrueger@rstms.net>
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: click==8.1.3
-Requires-Dist: hvac==0.11.2
-Requires-Dist: pyyaml==5.4.1
-Requires-Dist: black==22.3.0 ; extra == "dev"
-Requires-Dist: bump2version==1.0.1 ; extra == "dev"
-Requires-Dist: coverage==6.4.1 ; extra == "dev"
-Requires-Dist: flake8==4.0.1 ; extra == "dev"
-Requires-Dist: flit==3.7.1 ; extra == "dev"
+Requires-Dist: click>=8.1.3
+Requires-Dist: hvac>=0.11.2
+Requires-Dist: pyyaml>=5.4.1
+Requires-Dist: black ; extra == "dev"
+Requires-Dist: bump2version ; extra == "dev"
+Requires-Dist: coverage ; extra == "dev"
+Requires-Dist: flake8 ; extra == "dev"
+Requires-Dist: flit ; extra == "dev"
+Requires-Dist: isort ; extra == "dev"
 Requires-Dist: pdbpp ; extra == "dev"
-Requires-Dist: pytest==7.1.2 ; extra == "dev"
+Requires-Dist: pytest ; extra == "dev"
 Requires-Dist: pytest-click ; extra == "dev"
-Requires-Dist: pytest-datadir==1.3.1 ; extra == "dev"
-Requires-Dist: tox==3.25.0 ; extra == "dev"
+Requires-Dist: pytest-datadir ; extra == "dev"
+Requires-Dist: tox ; extra == "dev"
 Requires-Dist: sphinx==5.0.1 ; extra == "docs"
 Requires-Dist: sphinx-click==4.1.0 ; extra == "docs"
 Requires-Dist: sphinx-rtd-theme==1.0.0 ; extra == "docs"
 Project-URL: Home, https://github.com/rstms/local-chamber
 Provides-Extra: dev
 Provides-Extra: docs
```

