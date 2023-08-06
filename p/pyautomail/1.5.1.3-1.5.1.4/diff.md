# Comparing `tmp/pyautomail-1.5.1.3.tar.gz` & `tmp/pyautomail-1.5.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyautomail-1.5.1.3.tar", last modified: Thu Aug  3 00:58:02 2023, max compression
+gzip compressed data, was "pyautomail-1.5.1.4.tar", last modified: Sun Aug  6 01:53:20 2023, max compression
```

## Comparing `pyautomail-1.5.1.3.tar` & `pyautomail-1.5.1.4.tar`

### file list

```diff
@@ -1,72 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:58:02.954076 pyautomail-1.5.1.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:58:02.946076 pyautomail-1.5.1.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:58:02.950076 pyautomail-1.5.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5210 2023-08-03 00:58:02.954076 pyautomail-1.5.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:58:02.950076 pyautomail-1.5.1.3/automail/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/automail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/automail/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/automail/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:58:02.950076 pyautomail-1.5.1.3/automail/config/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/automail/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/automail/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8864 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/automail/emailsender.py
--rw-r--r--   0 runner    (1001) docker     (123)    10398 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/automail/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:58:02.950076 pyautomail-1.5.1.3/automail/storage/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/automail/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/automail/storage/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/automail/storage/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/automail/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/config.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/contact.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:58:02.954076 pyautomail-1.5.1.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:58:02.954076 pyautomail-1.5.1.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)   191926 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/docs/_static/automail-logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:58:02.946076 pyautomail-1.5.1.3/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:58:02.954076 pyautomail-1.5.1.3/docs/_templates/apidoc/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/docs/_templates/apidoc/module.rst_t
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/docs/_templates/apidoc/package.rst_t
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/docs/_templates/apidoc/toc.rst_t
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:58:02.954076 pyautomail-1.5.1.3/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/docs/api/automail.config.rst
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/docs/api/automail.rst
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/docs/api/automail.storage.rst
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/docs/getting-started.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/docs/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:58:02.954076 pyautomail-1.5.1.3/docs/tutorial/
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/docs/tutorial/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    36379 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/document.pdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:58:02.954076 pyautomail-1.5.1.3/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/examples/base-usage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:58:02.954076 pyautomail-1.5.1.3/pyautomail.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5210 2023-08-03 00:58:02.000000 pyautomail-1.5.1.3/pyautomail.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-08-03 00:58:02.000000 pyautomail-1.5.1.3/pyautomail.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 00:58:02.000000 pyautomail-1.5.1.3/pyautomail.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-03 00:58:02.000000 pyautomail-1.5.1.3/pyautomail.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-03 00:58:02.000000 pyautomail-1.5.1.3/pyautomail.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-03 00:58:02.000000 pyautomail-1.5.1.3/pyautomail.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/sending_gmail.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-08-03 00:58:02.958077 pyautomail-1.5.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/sub.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:58:02.954076 pyautomail-1.5.1.3/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/templates/body.txt
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/templates/html.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:58:02.954076 pyautomail-1.5.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:58:02.954076 pyautomail-1.5.1.3/tests/test_cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/tests/test_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/tests/test_cli/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/tests/test_cli/test_cli_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/tests/test_cli/test_cli_register.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/tests/test_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 01:53:20.611472 pyautomail-1.5.1.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 01:53:20.603471 pyautomail-1.5.1.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 01:53:20.607472 pyautomail-1.5.1.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5210 2023-08-06 01:53:20.611472 pyautomail-1.5.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 01:53:20.607472 pyautomail-1.5.1.4/automail/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/automail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/automail/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15395 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/automail/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 01:53:20.607472 pyautomail-1.5.1.4/automail/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/automail/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/automail/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9011 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/automail/emailsender.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10398 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/automail/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 01:53:20.607472 pyautomail-1.5.1.4/automail/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/automail/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/automail/storage/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/automail/storage/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/automail/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/config.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/contact.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 01:53:20.607472 pyautomail-1.5.1.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 01:53:20.611472 pyautomail-1.5.1.4/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)   191926 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/docs/_static/automail-logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 01:53:20.607472 pyautomail-1.5.1.4/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 01:53:20.611472 pyautomail-1.5.1.4/docs/_templates/apidoc/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/docs/_templates/apidoc/module.rst_t
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/docs/_templates/apidoc/package.rst_t
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/docs/_templates/apidoc/toc.rst_t
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 01:53:20.611472 pyautomail-1.5.1.4/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/docs/api/automail.config.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/docs/api/automail.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/docs/api/automail.storage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/docs/getting-started.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/docs/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 01:53:20.611472 pyautomail-1.5.1.4/docs/tutorial/
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/docs/tutorial/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    36379 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/document.pdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 01:53:20.611472 pyautomail-1.5.1.4/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/examples/base-usage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 01:53:20.611472 pyautomail-1.5.1.4/pyautomail.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5210 2023-08-06 01:53:20.000000 pyautomail-1.5.1.4/pyautomail.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-08-06 01:53:20.000000 pyautomail-1.5.1.4/pyautomail.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 01:53:20.000000 pyautomail-1.5.1.4/pyautomail.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-06 01:53:20.000000 pyautomail-1.5.1.4/pyautomail.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-06 01:53:20.000000 pyautomail-1.5.1.4/pyautomail.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-06 01:53:20.000000 pyautomail-1.5.1.4/pyautomail.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/sending_gmail.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-08-06 01:53:20.611472 pyautomail-1.5.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/sub.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 01:53:20.611472 pyautomail-1.5.1.4/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/templates/body.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/templates/html.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 01:53:20.611472 pyautomail-1.5.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 01:53:20.611472 pyautomail-1.5.1.4/tests/test_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/tests/test_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/tests/test_cli/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/tests/test_cli/test_cli_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/tests/test_cli/test_cli_other.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/tests/test_cli/test_cli_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/tests/test_manager.py
```

### Comparing `pyautomail-1.5.1.3/.readthedocs.yaml` & `pyautomail-1.5.1.4/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `pyautomail-1.5.1.3/PKG-INFO` & `pyautomail-1.5.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyautomail
-Version: 1.5.1.3
+Version: 1.5.1.4
 Summary: Automated Email Sending for Large Scale Email and Gmail Automation
 Home-page: https://github.com/msinamsina/pyautomail
 Author: Mohammad sina Allahkaram
 Author-email: msinamsina@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/msinamsina/pyautomail/issues
 Project-URL: Changelog, https://github.com/msinamsina/pyautomail/releases
```

### Comparing `pyautomail-1.5.1.3/README.md` & `pyautomail-1.5.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pyautomail-1.5.1.3/automail/config/config.py` & `pyautomail-1.5.1.4/automail/config/config.py`

 * *Files identical despite different names*

### Comparing `pyautomail-1.5.1.3/automail/emailsender.py` & `pyautomail-1.5.1.4/automail/emailsender.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import smtplib
 import os
 import sys
 import jinja2
 import logging
+import json
 from email import encoders
 from email.mime.base import MIMEBase
 from email.mime.multipart import MIMEMultipart
 from email.mime.text import MIMEText
 from configparser import ConfigParser
 from automail.config import configurable
 
@@ -174,20 +175,23 @@
 
     def render_template(self, data):
         """This method is used by send method.
 
         :param data: dictionary of data to be replaced in the template.
         :return: body: the string of the rendered template.
         """
+        if isinstance(data, str):
+            data = json.loads(data)
         if self.template_type == 'html':
             self.__logger.debug("Rendering HTML template...")
             return jinja2.Template(self.template).render(data)
         elif self.template_type == 'txt':
             self.__logger.debug("Rendering TXT template...")
-            return self.template.format(**data)
+            # return self.template.format(**data)
+            return jinja2.Template(self.template).render(data)
         else:
             self.__logger.error("Template type not supported! Exiting! (please use HTML or TXT templates.)")
             raise (NotImplemented, "Template type not supported! Exiting! (please use HTML or TXT templates.)")
 
     def send(self, receiver_email_address: str, subject: str, data: dict, attachment_path=None) -> dict:
         """
```

### Comparing `pyautomail-1.5.1.3/automail/manager.py` & `pyautomail-1.5.1.4/automail/manager.py`

 * *Files identical despite different names*

### Comparing `pyautomail-1.5.1.3/automail/storage/model.py` & `pyautomail-1.5.1.4/automail/storage/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,17 +26,17 @@
     data = Column(String)
     """str : the custom data of the email a string of json"""
     attachment_path = Column(String)
     """str : the path to the attachment file"""
     status = Column(ChoiceType(STATUSES), default='unsent')
     """str : the status of the record it can be choose from STATUSES"""
 
-    process_id = Column(Integer, ForeignKey("process.id"), nullable=False)
+    process_id = Column(Integer, ForeignKey("process.id", ondelete="CASCADE"), nullable=False)
     """int : the id of the process which this record belongs to"""
-    process = relationship("Process", backref=backref("records", order_by=id))
+    process = relationship("Process", backref=backref("records", order_by=id, cascade="all, delete"))
     """automail.storage.database.Process : the process of the record"""
 
 
 class Process(Base):
     """This class is used to store the processes of the emails in the database the table name is `process`
 
     - Every time you register a contact list to send emails to it, a process will be created and stored in the database
```

### Comparing `pyautomail-1.5.1.3/automail/storage/util.py` & `pyautomail-1.5.1.4/automail/storage/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from sqlalchemy.orm import sessionmaker, declarative_base
 from sqlalchemy import create_engine
 import os
 import datetime
 import pandas as pd
+from automail.utils import init_logger
 
 Base = declarative_base()
 
 
 def create_tables(engine):
     """create tables in database
```

### Comparing `pyautomail-1.5.1.3/automail/utils.py` & `pyautomail-1.5.1.4/automail/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 import sys
 import configparser
-
+import multiprocessing
 
 def init_logger(name=''):
     """This function will initialize a logger object
 
     Parameters
     ----------
     name : str
@@ -39,22 +39,23 @@
     [2019-08-20 15:30:00,000 - ERROR (EmailSender) ] : error message
     >>> logger_obj.critical('critical message')
     [2019-08-20 15:30:00,000 - CRITICAL (EmailSender) ] : critical message
 
 
     """
     logger_obj = logging.getLogger(name)
+    # logger_obj = multiprocessing.get_logger(name)
     logger_obj.setLevel(logging.DEBUG)
     formatter = logging.Formatter('[%(asctime)s - %(levelname)s (%(name)s) ] : %(message)s')
     handler1 = logging.StreamHandler(sys.stdout)
     handler1.setFormatter(formatter)
-    handler2 = logging.FileHandler('../emailsender.log')
-    handler2.setFormatter(formatter)
+    # handler2 = logging.FileHandler('../emailsender.log')
+    # handler2.setFormatter(formatter)
     logger_obj.addHandler(handler1)
-    logger_obj.addHandler(handler2)
+    # logger_obj.addHandler(handler2)
     return logger_obj
 
 
 def create_config_file(smtp_server, smtp_port, sender_email='', password='', is_test=False):
     """This function will create a config file for the email sender.
 
     Parameters
@@ -79,15 +80,15 @@
         [SENDER]
         email = example@gmail.com
         password = password
 
     """
     with open('./config.cfg', 'w') as f:
         f.write('[smtp]\n')
-        f.write(f'server = {smtp_server}\n')
+        f.write(f'host = {smtp_server}\n')
         f.write(f'port = {smtp_port}\n')
         f.write(f'is_test = {is_test}\n')
         f.write('\n')
         f.write('[account]\n')
         f.write(f'user = {sender_email}\n')
         f.write(f'password = {password}\n')
```

### Comparing `pyautomail-1.5.1.3/docs/Makefile` & `pyautomail-1.5.1.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyautomail-1.5.1.3/docs/_static/automail-logo.png` & `pyautomail-1.5.1.4/docs/_static/automail-logo.png`

 * *Files identical despite different names*

### Comparing `pyautomail-1.5.1.3/docs/_templates/apidoc/package.rst_t` & `pyautomail-1.5.1.4/docs/_templates/apidoc/package.rst_t`

 * *Files identical despite different names*

### Comparing `pyautomail-1.5.1.3/docs/api/automail.rst` & `pyautomail-1.5.1.4/docs/api/automail.rst`

 * *Files identical despite different names*

### Comparing `pyautomail-1.5.1.3/docs/conf.py` & `pyautomail-1.5.1.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyautomail-1.5.1.3/docs/getting-started.rst` & `pyautomail-1.5.1.4/docs/getting-started.rst`

 * *Files identical despite different names*

### Comparing `pyautomail-1.5.1.3/docs/index.rst` & `pyautomail-1.5.1.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pyautomail-1.5.1.3/docs/introduction.rst` & `pyautomail-1.5.1.4/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `pyautomail-1.5.1.3/docs/make.bat` & `pyautomail-1.5.1.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyautomail-1.5.1.3/docs/tutorial/index.rst` & `pyautomail-1.5.1.4/docs/tutorial/index.rst`

 * *Files identical despite different names*

### Comparing `pyautomail-1.5.1.3/document.pdf` & `pyautomail-1.5.1.4/document.pdf`

 * *Files identical despite different names*

### Comparing `pyautomail-1.5.1.3/pyautomail.egg-info/PKG-INFO` & `pyautomail-1.5.1.4/pyautomail.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyautomail
-Version: 1.5.1.3
+Version: 1.5.1.4
 Summary: Automated Email Sending for Large Scale Email and Gmail Automation
 Home-page: https://github.com/msinamsina/pyautomail
 Author: Mohammad sina Allahkaram
 Author-email: msinamsina@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/msinamsina/pyautomail/issues
 Project-URL: Changelog, https://github.com/msinamsina/pyautomail/releases
```

### Comparing `pyautomail-1.5.1.3/pyautomail.egg-info/SOURCES.txt` & `pyautomail-1.5.1.4/pyautomail.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -47,8 +47,9 @@
 templates/body.txt
 templates/html.html
 tests/__init__.py
 tests/test_manager.py
 tests/test_cli/__init__.py
 tests/test_cli/test_cli.py
 tests/test_cli/test_cli_init.py
+tests/test_cli/test_cli_other.py
 tests/test_cli/test_cli_register.py
```

### Comparing `pyautomail-1.5.1.3/sending_gmail.py` & `pyautomail-1.5.1.4/sending_gmail.py`

 * *Files identical despite different names*

### Comparing `pyautomail-1.5.1.3/setup.cfg` & `pyautomail-1.5.1.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyautomail-1.5.1.3/setup.py` & `pyautomail-1.5.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `pyautomail-1.5.1.3/tests/test_cli/test_cli_init.py` & `pyautomail-1.5.1.4/tests/test_cli/test_cli_init.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,32 @@
 from typer.testing import CliRunner
 import shutil
 import os
 from automail import cli
+import pytest
+import tempfile
 
 
 runner = CliRunner()
 
 
+@pytest.fixture(scope='module', autouse=True)
+def setup():
+
+    print("setup module fixture is called ... sinasina")
+    test_dir = tempfile.mkdtemp()
+    print('-'*50)
+    print(test_dir)
+    os.chdir(test_dir)
+    print(os.getcwd())
+    yield
+    os.chdir('..')
+    shutil.rmtree(test_dir)
+
+
 def usual_output(result):
     assert result.exit_code == 0
     assert "Where do you want to initialize the automail project? [./automail-workspace]: " in result.stdout
     assert "What is your smtp server? [smtp.gmail.com]: " in result.stdout
     assert "What is your smtp port? [465]: " in result.stdout
 
 
@@ -28,15 +44,15 @@
     usual_output(result)
     assert "Initializing automail database..." in result.stdout
     assert "Done!" in result.stdout
     assert os.path.exists("test") is True
     assert os.path.exists("test/mail.db") is True
     with open("test/config.cfg") as f:
         config = f.read()
-    assert "[smtp]\nserver = smtp.gmail.com\nport = 465\nis_test = False\n\n[account]\nuser = \npassword = \n" == config
+    assert "[smtp]\nhost = smtp.gmail.com\nport = 465\nis_test = False\n\n[account]\nuser = \npassword = \n" == config
 
 
 def test_init_3():
     # enter a path that already exists and choose not to delete it
     result = runner.invoke(cli.app, ["init"], input="test")
     usual_output(result)
     assert "Directory test already exists." in result.stdout
@@ -82,24 +98,24 @@
 
 def test_init_7():
     result = runner.invoke(cli.app, ["init", "-db", "test", "-ss", "smtp.server.com"], input="\ny\n")
     _helper_init(result)
     assert "What is your smtp port? [465]: " in result.stdout
     with open("test/config.cfg") as f:
         config = f.read()
-    assert "[smtp]\nserver = smtp.server.com\nport = 465\nis_test = False\n\n[account]\nuser = \npassword = \n" == config
+    assert "[smtp]\nhost = smtp.server.com\nport = 465\nis_test = False\n\n[account]\nuser = \npassword = \n" == config
 
 
 def test_init_8():
     result = runner.invoke(cli.app, ["init", "-db", "test", "-ss", "smtp.gmail.com", "-sp", "111"], input="y\n")
     _helper_init(result)
     with open("test/config.cfg") as f:
         config = f.read()
-    assert "[smtp]\nserver = smtp.gmail.com\nport = 111\nis_test = False\n\n[account]\nuser = \npassword = \n" == config
+    assert "[smtp]\nhost = smtp.gmail.com\nport = 111\nis_test = False\n\n[account]\nuser = \npassword = \n" == config
 
 
 def test_init_9():
     result = runner.invoke(cli.app, ["init", "-db", "test", "-ss", "smtp.gmail.com", "-sp", "111", "-t"], input="y\n")
     _helper_init(result)
     with open("test/config.cfg") as f:
         config = f.read()
-    assert "[smtp]\nserver = smtp.gmail.com\nport = 111\nis_test = True\n\n[account]\nuser = \npassword = \n" == config
+    assert "[smtp]\nhost = smtp.gmail.com\nport = 111\nis_test = True\n\n[account]\nuser = \npassword = \n" == config
```

### Comparing `pyautomail-1.5.1.3/tests/test_manager.py` & `pyautomail-1.5.1.4/tests/test_manager.py`

 * *Files identical despite different names*

