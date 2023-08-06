# Comparing `tmp/edc-pdf-reports-0.3.16.tar.gz` & `tmp/edc-pdf-reports-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-pdf-reports-0.3.16.tar", last modified: Sun Aug  6 19:01:27 2023, max compression
+gzip compressed data, was "edc-pdf-reports-0.3.9.tar", last modified: Tue Jun 21 03:01:12 2022, max compression
```

## Comparing `edc-pdf-reports-0.3.16.tar` & `edc-pdf-reports-0.3.9.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-06 19:01:27.503777 edc-pdf-reports-0.3.16/
--rw-r--r--   0 erikvw     (501) staff       (20)      105 2022-06-21 03:01:03.000000 edc-pdf-reports-0.3.16/.coveragerc
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2021-02-07 13:48:34.000000 edc-pdf-reports-0.3.16/.editorconfig
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-06 19:01:27.495879 edc-pdf-reports-0.3.16/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-06 19:01:27.499283 edc-pdf-reports-0.3.16/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     1927 2023-08-06 19:01:19.000000 edc-pdf-reports-0.3.16/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)     1236 2022-06-21 03:01:03.000000 edc-pdf-reports-0.3.16/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)     1077 2023-05-16 03:07:59.000000 edc-pdf-reports-0.3.16/.pre-commit-config.yaml
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2023-05-02 01:46:53.000000 edc-pdf-reports-0.3.16/.yamllint
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-21 03:01:03.000000 edc-pdf-reports-0.3.16/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-21 03:01:03.000000 edc-pdf-reports-0.3.16/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35147 2020-03-04 23:38:36.000000 edc-pdf-reports-0.3.16/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)      117 2022-06-21 03:01:03.000000 edc-pdf-reports-0.3.16/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     1551 2023-08-06 19:01:27.503869 edc-pdf-reports-0.3.16/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)      722 2022-06-21 03:01:03.000000 edc-pdf-reports-0.3.16/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      166 2023-05-02 01:46:53.000000 edc-pdf-reports-0.3.16/codecov.yml
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-06 19:01:27.500779 edc-pdf-reports-0.3.16/edc_pdf_reports/
--rw-r--r--   0 erikvw     (501) staff       (20)      112 2022-06-21 03:01:03.000000 edc-pdf-reports-0.3.16/edc_pdf_reports/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      118 2022-06-21 03:01:03.000000 edc-pdf-reports-0.3.16/edc_pdf_reports/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)     8275 2022-06-21 03:01:03.000000 edc-pdf-reports-0.3.16/edc_pdf_reports/crf_pdf_report.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2428 2022-06-21 03:01:03.000000 edc-pdf-reports-0.3.16/edc_pdf_reports/crfs_to_pdf.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1145 2023-05-16 03:07:59.000000 edc-pdf-reports-0.3.16/edc_pdf_reports/numbered_canvas.py
--rw-r--r--   0 erikvw     (501) staff       (20)     7489 2023-07-18 02:09:50.000000 edc-pdf-reports-0.3.16/edc_pdf_reports/report.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-06 19:01:27.496129 edc-pdf-reports-0.3.16/edc_pdf_reports/static/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-06 19:01:27.501814 edc-pdf-reports-0.3.16/edc_pdf_reports/static/edc_pdf_reports/
--rw-r--r--   0 erikvw     (501) staff       (20)     6725 2022-06-21 03:01:03.000000 edc-pdf-reports-0.3.16/edc_pdf_reports/static/edc_pdf_reports/clinicedc_logo.jpg
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-06 19:01:27.502355 edc-pdf-reports-0.3.16/edc_pdf_reports/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-21 03:01:03.000000 edc-pdf-reports-0.3.16/edc_pdf_reports/tests/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-06 19:01:27.503626 edc-pdf-reports-0.3.16/edc_pdf_reports/tests/etc/
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-06-21 03:01:03.000000 edc-pdf-reports-0.3.16/edc_pdf_reports/tests/etc/user-aes-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-06-21 03:01:03.000000 edc-pdf-reports-0.3.16/edc_pdf_reports/tests/etc/user-aes-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-06-21 03:01:03.000000 edc-pdf-reports-0.3.16/edc_pdf_reports/tests/etc/user-rsa-local-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-06-21 03:01:03.000000 edc-pdf-reports-0.3.16/edc_pdf_reports/tests/etc/user-rsa-local-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-06-21 03:01:03.000000 edc-pdf-reports-0.3.16/edc_pdf_reports/tests/etc/user-rsa-restricted-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-06-21 03:01:03.000000 edc-pdf-reports-0.3.16/edc_pdf_reports/tests/etc/user-rsa-restricted-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-06-21 03:01:03.000000 edc-pdf-reports-0.3.16/edc_pdf_reports/tests/etc/user-salt-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-06-21 03:01:03.000000 edc-pdf-reports-0.3.16/edc_pdf_reports/tests/etc/user-salt-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1610 2022-06-21 03:01:03.000000 edc-pdf-reports-0.3.16/edc_pdf_reports/tests/my_report.py
--rw-r--r--   0 erikvw     (501) staff       (20)      380 2023-08-06 19:01:19.000000 edc-pdf-reports-0.3.16/edc_pdf_reports/tests/test_report.py
--rw-r--r--   0 erikvw     (501) staff       (20)      111 2022-06-21 03:01:03.000000 edc-pdf-reports-0.3.16/edc_pdf_reports/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-06 19:01:27.501685 edc-pdf-reports-0.3.16/edc_pdf_reports.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     1551 2023-08-06 19:01:27.000000 edc-pdf-reports-0.3.16/edc_pdf_reports.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1204 2023-08-06 19:01:27.000000 edc-pdf-reports-0.3.16/edc_pdf_reports.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-08-06 19:01:27.000000 edc-pdf-reports-0.3.16/edc_pdf_reports.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-06-15 23:37:29.000000 edc-pdf-reports-0.3.16/edc_pdf_reports.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)       18 2023-08-06 19:01:27.000000 edc-pdf-reports-0.3.16/edc_pdf_reports.egg-info/requires.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       16 2023-08-06 19:01:27.000000 edc-pdf-reports-0.3.16/edc_pdf_reports.egg-info/top_level.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1737 2023-08-06 19:01:19.000000 edc-pdf-reports-0.3.16/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)     1056 2023-08-01 05:13:24.000000 edc-pdf-reports-0.3.16/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1177 2023-08-06 19:01:27.504167 edc-pdf-reports-0.3.16/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-21 03:01:12.705163 edc-pdf-reports-0.3.9/
+-rw-r--r--   0 erikvw     (501) staff       (20)      105 2022-06-21 03:01:03.000000 edc-pdf-reports-0.3.9/.coveragerc
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2021-02-07 13:48:34.000000 edc-pdf-reports-0.3.9/.editorconfig
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-21 03:01:12.699154 edc-pdf-reports-0.3.9/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-21 03:01:12.702082 edc-pdf-reports-0.3.9/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1745 2022-05-19 02:12:43.000000 edc-pdf-reports-0.3.9/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1236 2022-06-21 03:01:03.000000 edc-pdf-reports-0.3.9/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-21 03:01:03.000000 edc-pdf-reports-0.3.9/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-21 03:01:03.000000 edc-pdf-reports-0.3.9/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35147 2020-03-04 23:38:36.000000 edc-pdf-reports-0.3.9/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)      117 2022-06-21 03:01:03.000000 edc-pdf-reports-0.3.9/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     1598 2022-06-21 03:01:12.705271 edc-pdf-reports-0.3.9/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)      722 2022-06-21 03:01:03.000000 edc-pdf-reports-0.3.9/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-06-21 03:01:03.000000 edc-pdf-reports-0.3.9/VERSION
+-rw-r--r--   0 erikvw     (501) staff       (20)      162 2021-02-07 13:48:34.000000 edc-pdf-reports-0.3.9/codecov.yml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-21 03:01:12.702954 edc-pdf-reports-0.3.9/edc_pdf_reports/
+-rw-r--r--   0 erikvw     (501) staff       (20)      112 2022-06-21 03:01:03.000000 edc-pdf-reports-0.3.9/edc_pdf_reports/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      118 2022-06-21 03:01:03.000000 edc-pdf-reports-0.3.9/edc_pdf_reports/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     8275 2022-06-21 03:01:03.000000 edc-pdf-reports-0.3.9/edc_pdf_reports/crf_pdf_report.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2428 2022-06-21 03:01:03.000000 edc-pdf-reports-0.3.9/edc_pdf_reports/crfs_to_pdf.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1146 2022-06-21 03:01:03.000000 edc-pdf-reports-0.3.9/edc_pdf_reports/numbered_canvas.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     6050 2022-06-21 03:01:03.000000 edc-pdf-reports-0.3.9/edc_pdf_reports/report.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-21 03:01:12.699370 edc-pdf-reports-0.3.9/edc_pdf_reports/static/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-21 03:01:12.703920 edc-pdf-reports-0.3.9/edc_pdf_reports/static/edc_pdf_reports/
+-rw-r--r--   0 erikvw     (501) staff       (20)     6725 2022-06-21 03:01:03.000000 edc-pdf-reports-0.3.9/edc_pdf_reports/static/edc_pdf_reports/clinicedc_logo.jpg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-21 03:01:12.704222 edc-pdf-reports-0.3.9/edc_pdf_reports/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-21 03:01:03.000000 edc-pdf-reports-0.3.9/edc_pdf_reports/tests/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-21 03:01:12.705064 edc-pdf-reports-0.3.9/edc_pdf_reports/tests/etc/
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-06-21 03:01:03.000000 edc-pdf-reports-0.3.9/edc_pdf_reports/tests/etc/user-aes-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-06-21 03:01:03.000000 edc-pdf-reports-0.3.9/edc_pdf_reports/tests/etc/user-aes-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-06-21 03:01:03.000000 edc-pdf-reports-0.3.9/edc_pdf_reports/tests/etc/user-rsa-local-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-06-21 03:01:03.000000 edc-pdf-reports-0.3.9/edc_pdf_reports/tests/etc/user-rsa-local-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-06-21 03:01:03.000000 edc-pdf-reports-0.3.9/edc_pdf_reports/tests/etc/user-rsa-restricted-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-06-21 03:01:03.000000 edc-pdf-reports-0.3.9/edc_pdf_reports/tests/etc/user-rsa-restricted-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-06-21 03:01:03.000000 edc-pdf-reports-0.3.9/edc_pdf_reports/tests/etc/user-salt-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-06-21 03:01:03.000000 edc-pdf-reports-0.3.9/edc_pdf_reports/tests/etc/user-salt-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1610 2022-06-21 03:01:03.000000 edc-pdf-reports-0.3.9/edc_pdf_reports/tests/my_report.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      368 2022-06-21 03:01:03.000000 edc-pdf-reports-0.3.9/edc_pdf_reports/tests/test_report.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      111 2022-06-21 03:01:03.000000 edc-pdf-reports-0.3.9/edc_pdf_reports/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-21 03:01:12.703811 edc-pdf-reports-0.3.9/edc_pdf_reports.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1598 2022-06-21 03:01:12.000000 edc-pdf-reports-0.3.9/edc_pdf_reports.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     1195 2022-06-21 03:01:12.000000 edc-pdf-reports-0.3.9/edc_pdf_reports.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-06-21 03:01:12.000000 edc-pdf-reports-0.3.9/edc_pdf_reports.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-06-15 23:37:29.000000 edc-pdf-reports-0.3.9/edc_pdf_reports.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)       18 2022-06-21 03:01:12.000000 edc-pdf-reports-0.3.9/edc_pdf_reports.egg-info/requires.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       16 2022-06-21 03:01:12.000000 edc-pdf-reports-0.3.9/edc_pdf_reports.egg-info/top_level.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1591 2022-06-21 03:01:03.000000 edc-pdf-reports-0.3.9/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)       18 2021-02-07 13:48:34.000000 edc-pdf-reports-0.3.9/requirements.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)      997 2022-06-21 03:01:03.000000 edc-pdf-reports-0.3.9/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1214 2022-06-21 03:01:12.705576 edc-pdf-reports-0.3.9/setup.cfg
```

### Comparing `edc-pdf-reports-0.3.16/.github/workflows/build.yml` & `edc-pdf-reports-0.3.9/.github/workflows/build.yml`

 * *Files 15% similar despite different names*

```diff
@@ -1,68 +1,68 @@
----
 name: build
 
 on: [push, pull_request]
 
 jobs:
   build:
     name: build (Python ${{ matrix.python-version }}, Django ${{ matrix.django-version }})
     runs-on: ubuntu-latest
 
     strategy:
       fail-fast: false
       matrix:
-        python-version: ['3.11']
-        django-version: ['4.1', '4.2', 'dev']
+        python-version: ['3.9']
+        django-version: ['3.2']
+
     services:
+
       mysql:
         image: mysql:latest
         env:
           MYSQL_DATABASE: mysql
           MYSQL_ROOT_PASSWORD: mysql
         ports:
           - 3306:3306
         options: --health-cmd="mysqladmin ping" --health-interval=10s --health-timeout=5s --health-retries=3
 
     steps:
-      - name: Install pycups and words dependency
-        run: |
-          sudo sed -i 's/azure\.//' /etc/apt/sources.list
-          sudo apt-get -y update
-          sudo apt-get install libcups2-dev wamerican
-
-      - uses: actions/checkout@v3
-      - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v4
-        with:
-          python-version: ${{ matrix.python-version }}
-
-      - name: Get pip cache dir
-        id: pip-cache
-        run: |
-          echo "dir=$(pip cache dir)" >>$GITHUB_OUTPUT
-
-      - name: Cache
-        uses: actions/cache@v3
-        with:
-          path: ${{ steps.pip-cache.outputs.dir }}
-          key:
-            ${{ matrix.python-version }}-v1-${{ hashFiles('**/setup.py') }}-${{ hashFiles('**/tox.ini') }}
-          restore-keys: |
-            ${{ matrix.python-version }}-v1-
-
-      - name: Install dependencies
-        run: |
-          python -m pip install --upgrade pip
-          python -m pip install -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/tox.txt
-
-
-      - name: Tox tests
-        run: |
-          tox -v
-        env:
-          DJANGO: ${{ matrix.django-version }}
-
-      - name: Upload coverage to Codecov
-        uses: codecov/codecov-action@v3
-        with:
-          name: Python ${{ matrix.python-version }}
+    - name: Install pycups and words dependency
+      run: |
+        sudo apt-get install libcups2-dev wamerican
+
+    - uses: actions/checkout@v2
+
+    - name: Set up Python ${{ matrix.python-version }}
+      uses: actions/setup-python@v2
+      with:
+        python-version: ${{ matrix.python-version }}
+
+    - name: Get pip cache dir
+      id: pip-cache
+      run: |
+        echo "::set-output name=dir::$(pip cache dir)"
+
+    - name: Cache
+      uses: actions/cache@v2
+      with:
+        path: ${{ steps.pip-cache.outputs.dir }}
+        key:
+          ${{ matrix.python-version }}-v1-${{ hashFiles('**/setup.py') }}-${{ hashFiles('**/tox.ini') }}
+        restore-keys: |
+          ${{ matrix.python-version }}-v1-
+
+    - name: Install dependencies
+      run: |
+        python -m pip install --upgrade pip
+        python -m pip install -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/tox.txt
+
+
+    - name: Tox tests
+      run: |
+        tox -v
+      env:
+        DJANGO: ${{ matrix.django-version }}
+
+    - name: Upload coverage
+      uses: codecov/codecov-action@v1
+      with:
+        name: Python ${{ matrix.python-version }}
```

### Comparing `edc-pdf-reports-0.3.16/.gitignore` & `edc-pdf-reports-0.3.9/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-pdf-reports-0.3.16/LICENSE` & `edc-pdf-reports-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-pdf-reports-0.3.16/PKG-INFO` & `edc-pdf-reports-0.3.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: edc-pdf-reports
-Version: 0.3.16
+Version: 0.3.9
 Summary: Report classes using reportlab/pdf for clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-pdf-reports
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django edc pdf reportlab,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 3.2
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Requires-Python: >=3.11
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
 
 |pypi| |actions| |codecov| |downloads|
```

### Comparing `edc-pdf-reports-0.3.16/README.rst` & `edc-pdf-reports-0.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `edc-pdf-reports-0.3.16/edc_pdf_reports/crf_pdf_report.py` & `edc-pdf-reports-0.3.9/edc_pdf_reports/crf_pdf_report.py`

 * *Files identical despite different names*

### Comparing `edc-pdf-reports-0.3.16/edc_pdf_reports/crfs_to_pdf.py` & `edc-pdf-reports-0.3.9/edc_pdf_reports/crfs_to_pdf.py`

 * *Files identical despite different names*

### Comparing `edc-pdf-reports-0.3.16/edc_pdf_reports/numbered_canvas.py` & `edc-pdf-reports-0.3.9/edc_pdf_reports/numbered_canvas.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from reportlab.lib.enums import TA_CENTER
 from reportlab.lib.pagesizes import A4
 from reportlab.lib.styles import ParagraphStyle, getSampleStyleSheet
 from reportlab.pdfgen import canvas
 
 
 class NumberedCanvas(canvas.Canvas):
+
     static_footer_text = None
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._saved_page_states = []
 
     def showPage(self):
```

### Comparing `edc-pdf-reports-0.3.16/edc_pdf_reports/report.py` & `edc-pdf-reports-0.3.9/edc_pdf_reports/report.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,25 @@
-from __future__ import annotations
-
-import os.path
-import sys
-import warnings
 from abc import ABC
 from io import BytesIO
 from uuid import uuid4
 
 from django.contrib import messages
 from django.http import HttpResponse
 from django.utils import timezone
 from django_revision.revision import Revision
 from edc_protocol import Protocol
 from reportlab.lib.enums import TA_CENTER, TA_LEFT, TA_RIGHT
 from reportlab.lib.pagesizes import A4
-from reportlab.lib.styles import (
-    ParagraphStyle,
-    StyleSheet1,
-    _baseFontNameB,
-    getSampleStyleSheet,
-)
+from reportlab.lib.styles import ParagraphStyle, _baseFontNameB, getSampleStyleSheet
 from reportlab.lib.units import cm
 from reportlab.platypus import Paragraph, SimpleDocTemplate
 
 from .numbered_canvas import NumberedCanvas
 
 
-class ReportError(Exception):
-    def __init__(self, message, code=None):
-        super().__init__(message)
-        self.code = code
-
-
 class Report(ABC):
     document_template = SimpleDocTemplate
 
     default_page = dict(
         rightMargin=0.5 * cm,
         leftMargin=0.5 * cm,
         topMargin=1.5 * cm,
@@ -70,60 +54,40 @@
         """Callback for `onFirstPage`"""
         self.draw_footer(canvas, doc)
 
     def on_later_pages(self, canvas, doc):
         """Callback for onLaterPages"""
         self.draw_footer(canvas, doc)
 
-    def render_to_buffer(self, **kwargs):
+    def render(self, message_user=None, **kwargs):
+
+        message_user = True if message_user is None else message_user
+        response = HttpResponse(content_type="application/pdf")
+        response["Content-Disposition"] = f'attachment; filename="{self.report_filename}"'
+
         buffer = BytesIO()
+
         document_template = self.document_template(buffer, **self.page)
+
         story = self.get_report_story(**kwargs)
+
         document_template.build(
             story,
             onFirstPage=self.on_first_page,
             onLaterPages=self.on_later_pages,
             canvasmaker=NumberedCanvas,
         )
-        buffer_value = buffer.getvalue()
-        buffer.close()
-        return buffer_value
 
-    def render(self, message_user: bool | None = None, **kwargs):
-        """Deprecated wrapper for render_to_response"""
-        warnings.warn(
-            "Method `render` has been deprecated. Use `render_to_response` instead.",
-            DeprecationWarning,
-        )
-        return self.render_to_response(message_user=message_user, **kwargs)
-
-    def render_to_response(self, message_user: bool | None = None, **kwargs):
-        """Render buffer to HTTP response"""
-        message_user = True if message_user is None else message_user
-        response = HttpResponse(content_type="application/pdf")
-        response["Content-Disposition"] = f'attachment; filename="{self.report_filename}"'
-        buffer_value = self.render_to_buffer()
-        response.write(buffer_value)
+        pdf = buffer.getvalue()
+        buffer.close()
+        response.write(pdf)
         if message_user and self.request:
             self.message_user(**kwargs)
         return response
 
-    def render_to_file(self, path: str, verbose: bool | None = None):
-        """Render buffer to file"""
-        buffer_value = self.render_to_buffer()
-        if not os.path.exists(path):
-            raise ReportError(f"Path does not exist. Got {path}")
-        else:
-            filename = os.path.join(path, self.report_filename)
-            with open(filename, "wb") as f:
-                f.write(buffer_value)
-                if verbose:
-                    sys.stdout.write(f"Created file {filename}\n")
-        return None
-
     def message_user(self, **kwargs):
         messages.success(
             self.request,
             f"The report has been exported as a PDF. See downloads in your browser. "
             f"The filename is '{self.report_filename}'.",
             fail_silently=True,
         )
@@ -145,15 +109,15 @@
     def styles(self):
         if not self._styles:
             styles = getSampleStyleSheet()
             styles.add(ParagraphStyle(name="titleR", fontSize=8, alignment=TA_RIGHT))
             styles.add(ParagraphStyle(name="header", fontSize=6, alignment=TA_CENTER))
             styles.add(ParagraphStyle(name="footer", fontSize=6, alignment=TA_RIGHT))
             styles.add(ParagraphStyle(name="center", alignment=TA_CENTER))
-            styles.add(ParagraphStyle(name="right", alignment=TA_RIGHT))
+            styles.add(ParagraphStyle(name="Right", alignment=TA_RIGHT))
             styles.add(ParagraphStyle(name="left", alignment=TA_LEFT))
             styles.add(
                 ParagraphStyle(name="line_data", alignment=TA_LEFT, fontSize=8, leading=10)
             )
             styles.add(
                 ParagraphStyle(
                     name="line_data_small", alignment=TA_LEFT, fontSize=7, leading=9
@@ -199,12 +163,9 @@
             )
             styles.add(
                 ParagraphStyle(name="row_header", fontSize=8, leading=8, alignment=TA_CENTER)
             )
             styles.add(
                 ParagraphStyle(name="row_data", fontSize=7, leading=7, alignment=TA_CENTER)
             )
-            self._styles = self.add_to_styles(styles)
+            self._styles = styles
         return self._styles
-
-    def add_to_styles(self, styles: StyleSheet1) -> StyleSheet1:
-        return styles
```

### Comparing `edc-pdf-reports-0.3.16/edc_pdf_reports/static/edc_pdf_reports/clinicedc_logo.jpg` & `edc-pdf-reports-0.3.9/edc_pdf_reports/static/edc_pdf_reports/clinicedc_logo.jpg`

 * *Files identical despite different names*

### Comparing `edc-pdf-reports-0.3.16/edc_pdf_reports/tests/etc/user-rsa-local-private.pem` & `edc-pdf-reports-0.3.9/edc_pdf_reports/tests/etc/user-rsa-local-private.pem`

 * *Files identical despite different names*

### Comparing `edc-pdf-reports-0.3.16/edc_pdf_reports/tests/etc/user-rsa-restricted-private.pem` & `edc-pdf-reports-0.3.9/edc_pdf_reports/tests/etc/user-rsa-restricted-private.pem`

 * *Files identical despite different names*

### Comparing `edc-pdf-reports-0.3.16/edc_pdf_reports/tests/my_report.py` & `edc-pdf-reports-0.3.9/edc_pdf_reports/tests/my_report.py`

 * *Files identical despite different names*

### Comparing `edc-pdf-reports-0.3.16/edc_pdf_reports.egg-info/PKG-INFO` & `edc-pdf-reports-0.3.9/edc_pdf_reports.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: edc-pdf-reports
-Version: 0.3.16
+Version: 0.3.9
 Summary: Report classes using reportlab/pdf for clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-pdf-reports
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django edc pdf reportlab,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 3.2
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Requires-Python: >=3.11
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
 
 |pypi| |actions| |codecov| |downloads|
```

### Comparing `edc-pdf-reports-0.3.16/edc_pdf_reports.egg-info/SOURCES.txt` & `edc-pdf-reports-0.3.9/edc_pdf_reports.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 .coveragerc
 .editorconfig
 .gitignore
-.pre-commit-config.yaml
-.yamllint
 AUTHORS
 CHANGES
 LICENSE
 MANIFEST.in
 README.rst
+VERSION
 codecov.yml
 pyproject.toml
+requirements.txt
 runtests.py
 setup.cfg
 .github/workflows/build.yml
 edc_pdf_reports/__init__.py
 edc_pdf_reports/apps.py
 edc_pdf_reports/crf_pdf_report.py
 edc_pdf_reports/crfs_to_pdf.py
```

### Comparing `edc-pdf-reports-0.3.16/pyproject.toml` & `edc-pdf-reports-0.3.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -3,72 +3,64 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools_scm]
 write_to = "_version.py"
 
 [tool.black]
 line-length = 95
-target-version = ["py310"]
+target-version = ["py39"]
 extend-exclude = '''^(.*\/)*\b(migrations)\b($|\/.*$)'''
 
 [tool.isort]
 profile = "black"
-py_version = "310"
+py_version = "39"
 skip = [".tox", ".eggs", "migrations"]
 
 [tool.coverage.run]
-parallel = false
+parallel = true
 branch = true
 source = ["edc_pdf_reports"]
 
 [tool.coverage.paths]
 source = ["edc_pdf_reports"]
 
 [tool.coverage.report]
 show_missing = true
 skip_covered = true
 omit = ["requirements.txt"]
-exclude_lines = [
-  "pragma: no cover",
-  "if TYPE_CHECKING:",
-]
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 envlist =
-    py{311}-dj{41,42,dev},
+    py{39}-dj{32,dev},
     lint
-
 isolated_build = true
 
 [gh-actions]
 python =
-    3.11: py311, lint
+    3.9: py39, lint
 
 [gh-actions:env]
 DJANGO =
-    4.1: dj41
-    4.2: dj42, lint
+    3.2: dj32, lint
     dev: djdev
 
 [testenv]
 deps =
     -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/tox.txt
     -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/test_utils.txt
     -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/edc.txt
     -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/third_party_dev.txt
-    dj41: Django>=4.1,<4.2
-    dj42: Django>=4.2,<5.0
+    dj32: Django>=3.2,<3.3
     djdev: https://github.com/django/django/tarball/main
 
 commands =
-    pip install -U pip coverage[toml]
+    pip install -U pip
     pip --version
-    pip freeze
     coverage run -a runtests.py
     coverage report
 
 [testenv:lint]
 deps = -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/lint.txt
 commands =
     isort --profile=black --check --diff .
```

### Comparing `edc-pdf-reports-0.3.16/runtests.py` & `edc-pdf-reports-0.3.9/runtests.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 app_name = "edc_pdf_reports"
 base_dir = dirname(abspath(__file__))
 
 DEFAULT_SETTINGS = DefaultTestSettings(
     calling_file=__file__,
     BASE_DIR=base_dir,
     APP_NAME=app_name,
-    SUBJECT_VISIT_MODEL="edc_visit_tracking.subjectvisit",
     EDC_AUTH_SKIP_SITE_AUTHS=True,
     EDC_AUTH_SKIP_AUTH_UPDATER=True,
     EDC_NAVBAR_VERIFY_ON_LOAD=IGNORE,
     ETC_DIR=os.path.join(base_dir, app_name, "tests", "etc"),
     add_dashboard_middleware=True,
     add_lab_dashboard_middleware=True,
 ).settings
```

### Comparing `edc-pdf-reports-0.3.16/setup.cfg` & `edc-pdf-reports-0.3.9/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -8,23 +8,24 @@
 description = Report classes using reportlab/pdf for clinicedc/edc projects
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 keywords = django edc pdf reportlab, clinicedc, clinical trials
 classifiers = 
 	Environment :: Web Environment
 	Framework :: Django
-	Framework :: Django :: 4.1
+	Framework :: Django :: 3.2
 	Intended Audience :: Developers
 	Intended Audience :: Science/Research
 	Operating System :: OS Independent
-	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.8
+	Programming Language :: Python :: 3.9
 	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 
 [options]
-python_requires = >=3.11
+python_requires = >=3.9
 zip_safe = False
 include_package_data = True
 packages = find:
 install_requires = 
 	reportlab
 	inflect
```

