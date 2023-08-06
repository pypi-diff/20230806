# Comparing `tmp/pyautomail-1.5.1.4.tar.gz` & `tmp/pyautomail-1.6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyautomail-1.5.1.4.tar", last modified: Sun Aug  6 01:53:20 2023, max compression
+gzip compressed data, was "pyautomail-1.6.0.0.tar", last modified: Sun Aug  6 16:44:08 2023, max compression
```

## Comparing `pyautomail-1.5.1.4.tar` & `pyautomail-1.6.0.0.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 01:53:20.611472 pyautomail-1.5.1.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 01:53:20.603471 pyautomail-1.5.1.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 01:53:20.607472 pyautomail-1.5.1.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5210 2023-08-06 01:53:20.611472 pyautomail-1.5.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 01:53:20.607472 pyautomail-1.5.1.4/automail/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/automail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/automail/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15395 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/automail/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 01:53:20.607472 pyautomail-1.5.1.4/automail/config/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/automail/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/automail/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9011 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/automail/emailsender.py
--rw-r--r--   0 runner    (1001) docker     (123)    10398 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/automail/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 01:53:20.607472 pyautomail-1.5.1.4/automail/storage/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/automail/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/automail/storage/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/automail/storage/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/automail/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/config.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/contact.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 01:53:20.607472 pyautomail-1.5.1.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 01:53:20.611472 pyautomail-1.5.1.4/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)   191926 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/docs/_static/automail-logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 01:53:20.607472 pyautomail-1.5.1.4/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 01:53:20.611472 pyautomail-1.5.1.4/docs/_templates/apidoc/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/docs/_templates/apidoc/module.rst_t
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/docs/_templates/apidoc/package.rst_t
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/docs/_templates/apidoc/toc.rst_t
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 01:53:20.611472 pyautomail-1.5.1.4/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/docs/api/automail.config.rst
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/docs/api/automail.rst
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/docs/api/automail.storage.rst
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/docs/getting-started.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/docs/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 01:53:20.611472 pyautomail-1.5.1.4/docs/tutorial/
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/docs/tutorial/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    36379 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/document.pdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 01:53:20.611472 pyautomail-1.5.1.4/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/examples/base-usage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 01:53:20.611472 pyautomail-1.5.1.4/pyautomail.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5210 2023-08-06 01:53:20.000000 pyautomail-1.5.1.4/pyautomail.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-08-06 01:53:20.000000 pyautomail-1.5.1.4/pyautomail.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 01:53:20.000000 pyautomail-1.5.1.4/pyautomail.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-06 01:53:20.000000 pyautomail-1.5.1.4/pyautomail.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-06 01:53:20.000000 pyautomail-1.5.1.4/pyautomail.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-06 01:53:20.000000 pyautomail-1.5.1.4/pyautomail.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/sending_gmail.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-08-06 01:53:20.611472 pyautomail-1.5.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/sub.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 01:53:20.611472 pyautomail-1.5.1.4/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/templates/body.txt
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/templates/html.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 01:53:20.611472 pyautomail-1.5.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 01:53:20.611472 pyautomail-1.5.1.4/tests/test_cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/tests/test_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/tests/test_cli/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/tests/test_cli/test_cli_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/tests/test_cli/test_cli_other.py
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/tests/test_cli/test_cli_register.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-06 01:53:11.000000 pyautomail-1.5.1.4/tests/test_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:44:08.019810 pyautomail-1.6.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:44:08.007809 pyautomail-1.6.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:44:08.011810 pyautomail-1.6.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-08-06 16:44:00.000000 pyautomail-1.6.0.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-06 16:44:00.000000 pyautomail-1.6.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-08-06 16:44:00.000000 pyautomail-1.6.0.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-08-06 16:44:08.019810 pyautomail-1.6.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-08-06 16:44:00.000000 pyautomail-1.6.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:44:08.015810 pyautomail-1.6.0.0/automail/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-08-06 16:44:00.000000 pyautomail-1.6.0.0/automail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-08-06 16:44:00.000000 pyautomail-1.6.0.0/automail/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16995 2023-08-06 16:44:00.000000 pyautomail-1.6.0.0/automail/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:44:08.015810 pyautomail-1.6.0.0/automail/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-06 16:44:00.000000 pyautomail-1.6.0.0/automail/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-08-06 16:44:00.000000 pyautomail-1.6.0.0/automail/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9058 2023-08-06 16:44:00.000000 pyautomail-1.6.0.0/automail/emailsender.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10398 2023-08-06 16:44:00.000000 pyautomail-1.6.0.0/automail/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:44:08.015810 pyautomail-1.6.0.0/automail/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-08-06 16:44:00.000000 pyautomail-1.6.0.0/automail/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-08-06 16:44:00.000000 pyautomail-1.6.0.0/automail/storage/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-08-06 16:44:00.000000 pyautomail-1.6.0.0/automail/storage/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-08-06 16:44:00.000000 pyautomail-1.6.0.0/automail/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-06 16:44:00.000000 pyautomail-1.6.0.0/config.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-08-06 16:44:00.000000 pyautomail-1.6.0.0/contact.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:44:08.015810 pyautomail-1.6.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-08-06 16:44:00.000000 pyautomail-1.6.0.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:44:08.015810 pyautomail-1.6.0.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)   191926 2023-08-06 16:44:00.000000 pyautomail-1.6.0.0/docs/_static/automail-logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:44:08.007809 pyautomail-1.6.0.0/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:44:08.015810 pyautomail-1.6.0.0/docs/_templates/apidoc/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-08-06 16:44:00.000000 pyautomail-1.6.0.0/docs/_templates/apidoc/module.rst_t
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-06 16:44:00.000000 pyautomail-1.6.0.0/docs/_templates/apidoc/package.rst_t
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-08-06 16:44:00.000000 pyautomail-1.6.0.0/docs/_templates/apidoc/toc.rst_t
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:44:08.015810 pyautomail-1.6.0.0/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-08-06 16:44:00.000000 pyautomail-1.6.0.0/docs/api/automail.config.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-08-06 16:44:00.000000 pyautomail-1.6.0.0/docs/api/automail.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-08-06 16:44:00.000000 pyautomail-1.6.0.0/docs/api/automail.storage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-06 16:44:00.000000 pyautomail-1.6.0.0/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-08-06 16:44:00.000000 pyautomail-1.6.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-08-06 16:44:00.000000 pyautomail-1.6.0.0/docs/getting-started.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-08-06 16:44:00.000000 pyautomail-1.6.0.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-08-06 16:44:00.000000 pyautomail-1.6.0.0/docs/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-08-06 16:44:00.000000 pyautomail-1.6.0.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:44:08.015810 pyautomail-1.6.0.0/docs/tutorial/
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-08-06 16:44:00.000000 pyautomail-1.6.0.0/docs/tutorial/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    36379 2023-08-06 16:44:00.000000 pyautomail-1.6.0.0/document.pdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:44:08.015810 pyautomail-1.6.0.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-08-06 16:44:00.000000 pyautomail-1.6.0.0/examples/base-usage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:44:08.019810 pyautomail-1.6.0.0/pyautomail.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-08-06 16:44:07.000000 pyautomail-1.6.0.0/pyautomail.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-08-06 16:44:08.000000 pyautomail-1.6.0.0/pyautomail.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 16:44:07.000000 pyautomail-1.6.0.0/pyautomail.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-06 16:44:07.000000 pyautomail-1.6.0.0/pyautomail.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-06 16:44:07.000000 pyautomail-1.6.0.0/pyautomail.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-06 16:44:07.000000 pyautomail-1.6.0.0/pyautomail.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-06 16:44:00.000000 pyautomail-1.6.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-08-06 16:44:00.000000 pyautomail-1.6.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-08-06 16:44:00.000000 pyautomail-1.6.0.0/sending_gmail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-08-06 16:44:08.019810 pyautomail-1.6.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-08-06 16:44:00.000000 pyautomail-1.6.0.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-06 16:44:00.000000 pyautomail-1.6.0.0/sub.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:44:08.019810 pyautomail-1.6.0.0/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-08-06 16:44:00.000000 pyautomail-1.6.0.0/templates/body.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-08-06 16:44:00.000000 pyautomail-1.6.0.0/templates/html.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:44:08.019810 pyautomail-1.6.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 16:44:00.000000 pyautomail-1.6.0.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:44:08.019810 pyautomail-1.6.0.0/tests/test_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 16:44:00.000000 pyautomail-1.6.0.0/tests/test_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-08-06 16:44:00.000000 pyautomail-1.6.0.0/tests/test_cli/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-08-06 16:44:00.000000 pyautomail-1.6.0.0/tests/test_cli/test_cli_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-08-06 16:44:00.000000 pyautomail-1.6.0.0/tests/test_cli/test_cli_other.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-08-06 16:44:00.000000 pyautomail-1.6.0.0/tests/test_cli/test_cli_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-06 16:44:00.000000 pyautomail-1.6.0.0/tests/test_manager.py
```

### Comparing `pyautomail-1.5.1.4/.readthedocs.yaml` & `pyautomail-1.6.0.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `pyautomail-1.5.1.4/PKG-INFO` & `pyautomail-1.6.0.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,11 @@
-Metadata-Version: 2.1
-Name: pyautomail
-Version: 1.5.1.4
-Summary: Automated Email Sending for Large Scale Email and Gmail Automation
-Home-page: https://github.com/msinamsina/pyautomail
-Author: Mohammad sina Allahkaram
-Author-email: msinamsina@gmail.com
-License: MIT
-Project-URL: Bug Tracker, https://github.com/msinamsina/pyautomail/issues
-Project-URL: Changelog, https://github.com/msinamsina/pyautomail/releases
-Project-URL: Documentation, https://pyautomail.readthedocs.io/en/latest/
-Project-URL: Source Code, https://github.com/msinamsina/pyautomail
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-
 # PyAutoMail: A Python package and command-line interface for automation sending email to your contact list
 
 
-<p align="center" width="100%">
-    <img  width="80%" src="https://github.com/msinamsina/automail/blob/main/docs/_static/automail-logo.png?raw=true" >
-</p>
+![pyautomail-image](./docs/_static/automail-logo.png)
 
 
 Pyautomail, an incredibly powerful Python package meticulously crafted for the purpose of automated email delivery, catering especially to large-scale Email or Gmail automation. In today's fast-paced digital era, effective communication stands as a crucial cornerstone for numerous businesses and projects that heavily rely on email as their primary medium of interaction. Nonetheless, the manual handling of individual emails or the management of bulk email campaigns can prove to be both time-consuming and prone to errors.
 
 Fear not, for pyautomail swoops in as the ultimate savior, offering a seamless and highly efficient solution for automating email communication. Be it the need to dispatch personalized emails to a vast audience, the execution of targeted email marketing campaigns, or the automation of repetitive email chores, this package serves as your ultimate go-to tool. With its user-friendly interface and an array of versatile features, pyautomail proves itself as a fitting choice for a wide range of applications, catering to startups, enterprises, professionals, and developers alike.
 
 Revolutionize your email operations, whether it involves mass email distribution, streamlined Gmail tasks, or the quest for enhanced email communication proficiency - pyautomail is here to streamline your workflow, elevate your efficiency, and elevate productivity to soaring heights.
@@ -34,49 +14,100 @@
 ## Installation
 
 ### [PyPi](https://pypi.org/project/pyautomail/)
 ```bash
 pip install pyautomail
 ```
 
-### Github
+### [Github](https://github.com/msinamsina/pyautomail.git)
 ```bash
-pip install git+https://github.com/msinamsina/automail.git
+pip install git+https://github.com/msinamsina/pyautomail.git
 ```
 
 ## How to use in command-line interface
-At first, you should register your email address and contact list
-```bash
-automail register <your-email-address> <Path-to-your-contact-list> [options]
-```
-Then you can send email to your contact list
-```bash
-automail start <process-id>
-```
+
+1. At first, you should initialize project
+    ```bash
+    pyhhon -m automail init
+    ```
+    
+   After running this command, you will see a some questions. You should answer them.
+    
+   ```bash
+   Where do you want to initialize the automail project? [./automail-workspace]
+   What is your smtp server? [smtp.gmail.com]:
+   What is your smtp port? [465]:
+   ```
+   
+    **📘 Note:**   
+    1. This command will create a folder with the project name in the path you specified. 
+    If you don't specify the path, it will create ```automail-workspace```.  
+    2. You can change the default smtp server by default it has been set on **Gmail Smtp Server**. 
+    3. You also can set the port of **Smtm Server** (by default 465).
+    4. Additionally, if you want to save you password in config file, you can use the ```-p``` or 
+   ```--pasword``` switch.
+    5. Moreover, if you want to initialize a test project, you can use ```-t``` or ```--test```. 
+       ```bash
+       $ pyhhon -m automail init -t -p <your-password>
+       ```
+
+   > **[📙 Important]()**  
+   > If directory already exists, it will be overwritten.
+   
+1. Then you should go to the project directory and register your contact list
+    ```bash
+    cd <your-project-name>
+    pyhhon -m automail register <Path-to-your-contact-list> [options]
+   ```
+   **📘 Note:**   
+   For using a template, use ```--template``` switch. The template can be ```.txt``` or ```.html```
+   Format.
+   ```bash
+   pyhhon -m automail register contact-list.csv --template ./body.html
+   ```
+   **body.html:**
+   ```html
+   <h1> Hi {{ name }}, </h1>
+   ```
+   **contact-list.csv:**
+   ```csv
+   email,name,data1,cpdf
+   contact1@gmail.com,contact1,ali,/path/to/pdf1
+   contact2@gmail.com,contact2,mohammad,/path/to/pdf2
+   contact3@gmail.com,contact3,soheila,/path/to/pdf3
+   ```
+   
+1. Now you can start sending emails by running the following command
+   ```bash
+   pyhhon -m automail start <process-id>
+   ```
+   
 ## How to use in python
 ```python
     from automail import EmailSender
     email_sender = EmailSender()
     email_sender.set_template('body.txt')
     data = {'name': 'Jon', 'age': 30}
     email_sender.send('msinamsina@gmail.com', 'sub1', data)
 ```
 
-### Documentation and Resources
+## Documentation and Resources
 
-For more comprehensive information about **PyAutoMail** and its capabilities, please explore our detailed [documentation](https://automail.readthedocs.io/en/latest/).
+For more comprehensive information about **PyAutoMail** and its capabilities, please explore our detailed [documentation](https://pyautomail.readthedocs.io/en/latest/).
 
-- Get a brief overview and explore the features of PyAutoMail in the [Introduction](https://automail.readthedocs.io/en/latest/introduction.html) section.
-- If you're new to PyAutoMail, follow our [Getting Started](https://automail.readthedocs.io/en/latest/getting-started.html) guide to kickstart your email automation journey.
-- For a quick reference, you can check out the [API Reference](https://automail.readthedocs.io/en/latest/api/index.html) section.
-- To gain deeper insights into PyAutoMail and learn best practices, dive into our informative [Tutorial](https://automail.readthedocs.io/en/latest/tutorial/index.html) section.
+- Get a brief overview and explore the features of PyAutoMail in the [Introduction](https://pyautomail.readthedocs.io/en/latest/introduction.html) section.
+- If you're new to PyAutoMail, follow our [Getting Started](https://pyautomail.readthedocs.io/en/latest/getting-started.html) guide to kickstart your email automation journey.
+- For a quick reference, you can check out the [API Reference](https://pyautomail.readthedocs.io/en/latest/api/index.html) section.
+- To gain deeper insights into PyAutoMail and learn best practices, dive into our informative [Tutorial](https://pyautomail.readthedocs.io/en/latest/tutorial/index.html) section.
 
 By exploring these resources, you'll harness the full potential of PyAutoMail and make the most out of its powerful email automation capabilities.
 
-### Contribution and Support
+---
+
+## Contribution and Support
 
 We welcome contributions from the community to enhance **PyAutoMail** and make it even more robust. If you're interested in contributing, here's how you can get involved:
 
 1. **Bug Reports and Feature Requests**: If you come across any issues or have ideas for new features, please [open an issue](https://github.com/msinamsina/automail/issues) on our GitHub repository. We appreciate detailed bug reports with steps to reproduce the problem and clear feature requests with use cases.
 
 2. **Pull Requests**: If you want to contribute code to PyAutoMail, you can do so by submitting a pull request. Please ensure that your code adheres to the existing code style, and include relevant tests to maintain code quality.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyautomail-1.5.1.4/automail/cli.py` & `pyautomail-1.6.0.0/automail/cli.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,519 +1,519 @@
 import os
 import shutil
 import time
 import typer
 from typing import Optional
 from pathlib import Path
 from automail import __app_name__, __version__, EmailSender
-from automail.utils import get_config_dict, read_config_file, init_logger
+from automail import utils
+from automail.utils import get_config_dict, init_logger
 from automail.storage import get_session, create_tables
-from automail.storage.model import Record, Process
-
+from automail.storage import util, Process, Record
 
 app = typer.Typer()
 
 
-def run_process(pid, resume=True):
+def run_process(pid, is_resume=True, wait_time=.05):
     """
     This function will run a process with a specific id
 
     Parameters
     ----------
     pid : int
         the process id
-    resume : bool
+    is_resume : bool
         if True, the program will resume the process if it is paused, otherwise it prints a warning message and \
         return without doing anything
+    wait_time : int
+        the time to wait between sending emails
     """
+    # initialize the logger
+    logger = init_logger('cli')
+    logger.info("Reading arguments...")
 
+    # get the database session
     session, engin = get_session()
     create_tables(engin)
 
-    logger = init_logger('manager')
-    logger.info("Reading arguments...")
+    # get the process and check if it exists
     process = session.query(Process).filter(Process.id == pid).first()
     if not process:
-        logger.error(f"ID:{pid} => Process not found. You can see all processes with 'mailmanager list' command")
+        logger.error(f"ID:{pid} => Process not found. You can see all processes with 'automail list' command")
         return
+
     sender_email = process.sender
     subject = process.subject
     temp_file = process.temp_file
-    if resume:
+
+    if is_resume:
         if process.status != "paused":
-            print(f"ID:{pid} => Program is already {process.status}")
+            logger.error(f"ID:{pid} => Program is already {process.status}. "
+                         f"For resuming the program, it should be paused")
             return
         contacts = session.query(Record).filter(Record.process_id == pid, Record.status == "unsent").all()
     else:
         if process.status in ["paused", "in progress", 'finished']:
             logger.warning(f"ID:{pid} => Program is already {process.status}")
-            print(f"ID:{pid} => Program is already {process.status}")
-            print(f"You can resume the program with 'mailmanager resume {pid}' command")
-            print(f"You can see all processes with 'mailmanager list' command")
-            while True:
-                check = input(f"Are you sure you want to sent all email again? (y/n)")
-                if check == "n":
-                    return
-                elif check == "y":
-                    break
-                else:
-                    print("Please enter y or n!")
+            logger.warning(f"the `automail start {id}` command will strart the program from the beginning")
+
+            check = typer.confirm(f"Are you sure you want to start the program from the beginning?", default=False)
+            if not check:
+                logger.info(f"ID:{pid} => Program not started")
+                return
+
         contacts = session.query(Record).filter(Record.process_id == pid).all()
 
-    password = typer.prompt(f"Enter password for {sender_email}", hide_input=True)
+    # get the password
+    logger.info("Creating EmailSender obj...")
+    if typer.confirm(f"Do you want to use the initial password for {sender_email}?", default=True):
+        sender = EmailSender(cfg="config.cfg", user=sender_email)
+    else:
+        password = typer.prompt(f"Enter password for {sender_email}", hide_input=True)
+        sender = EmailSender(cfg="config.cfg", user=sender_email, password=password)
 
     # Create a secure SSL context
-    logger.info("Creating EmailSender obj...")
-    sender = EmailSender(cfg="config.cfg", user=sender_email, password=password)
     if temp_file:
         sender.set_template(temp_file)
 
     process.status = "in progress"
     session.commit()
 
     pause = False
     for contact in contacts:
         process = session.query(Process).filter(Process.id == pid).first()
         if process.status == "paused":
-            logger.info(f"ID:{pid} => Pausing the program")
-            pause = True
-            break
+            logger.info(f"ID:{pid} => is paused by other process")
+            session.close()
+            engin.dispose()
+            return
         logger.info(f"Sending email to: {contact.receiver}")
         sender.send(contact.receiver, subject, contact.data)
         contact.status = "sent"
         session.commit()
         logger.info(f"ID:{contact.id} => Email sent to {contact.receiver}")
-        time.sleep(10)
-
-    if not pause:
-        process.status = "finished"
-        session.commit()
-        logger.info(f"ID:{pid} => Program finished successfully")
+        time.sleep(wait_time)
 
-
-    session.close()
-    engin.dispose()
+    process.status = "finished"
+    session.commit()
+    logger.info(f"ID:{pid} => Program finished successfully")
 
 
 def _version_callback(value: bool) -> None:
+    """Show the application's version and exit."""
     if value:
         typer.echo(f"{__app_name__} v{__version__}")
         raise typer.Exit()
 
 
 @app.callback()
 def main(
-    version: Optional[bool] = typer.Option(
-        None,
-        "--version",
-        "-v",
-        help="Show the application's version and exit.",
-        callback=_version_callback,
-        is_eager=True,
-    )
-
+        version: Optional[bool] = typer.Option(
+            None,
+            "--version",
+            "-v",
+            help="Show the application's version and exit.",
+            callback=_version_callback,
+            is_eager=True,
+        )
 ) -> None:
     return
 
 
 @app.command()
 def init(
-    db_path: str = typer.Option(
-        './automail-workspace',
-        "--db-path",
-        "-db",
-        prompt="Where do you want to initialize the automail project?",
-    ),
-    smtp_server: str = typer.Option(
-        'smtp.gmail.com',
-        "--smtp-server",
-        "-ss",
-        prompt="What is your smtp server?",
-        help="Your smtp server.",
-    ),
-    smtp_port: int = typer.Option(
-        465,
-        "--smtp-port",
-        "-sp",
-        prompt="What is your smtp port?",
-        help="Your smtp port.",
-    ),
-    email: str = typer.Option(
-        '',
-        "--email",
-        "-e",
-        help="Your email address.",
-    ),
-    password: str = typer.Option(
-        '',
-        "--password",
-        "-p",
-        help="Your email password.",
-        hide_input=True,
-    ),
-    is_test: bool = typer.Option(
-        False,
-        "--test",
-        "-t",
-        help="Test output.",
-    ),
+        db_path: str = typer.Option(
+            './automail-workspace',
+            "--db-path",
+            "-db",
+            prompt="Where do you want to initialize the automail project?",
+        ),
+        smtp_server: str = typer.Option(
+            'smtp.gmail.com',
+            "--smtp-server",
+            "-ss",
+            prompt="What is your smtp server?",
+            help="Your smtp server.",
+        ),
+        smtp_port: int = typer.Option(
+            465,
+            "--smtp-port",
+            "-sp",
+            prompt="What is your smtp port?",
+            help="Your smtp port.",
+        ),
+        email: str = typer.Option(
+            '',
+            "--email",
+            "-e",
+            help="Your email address.",
+        ),
+        password: str = typer.Option(
+            '',
+            "--password",
+            "-p",
+            help="Your email password.",
+            hide_input=True,
+        ),
+        is_test: bool = typer.Option(
+            False,
+            "--test",
+            "-t",
+            help="Test output.",
+        ),
 ) -> None:
     """Initialize the mail database."""
-    from automail import utils
-    from automail import __app_name__
-
+    logger = init_logger('cli')
     if not shutil.os.path.exists(db_path):
         shutil.os.mkdir(db_path)
     else:
-        typer.secho(f"Directory {db_path} already exists.", fg=typer.colors.RED)
+        logger.error(f"Directory {db_path} already exists.")
         # delete the folder if it exists
-        if typer.confirm("Do you want to delete it?", default=False):
+        if typer.confirm(f"Do you want to delete {db_path} directory?", default=False):
             shutil.rmtree(db_path)
-            print("Deleting...")
+            logger.info(f"Deleting {db_path} directory...")
             time.sleep(0.5)
             shutil.os.mkdir(db_path)
-
         else:
-            typer.echo("Aborted!")
+            logger.info(f"Aborted!")
             raise typer.Exit(code=0)
 
-    typer.echo(f"Initializing {__app_name__} database...")
+    # create the database
+    logger.info(f"Initializing {__app_name__} database...")
     os.chdir(db_path)
     session, engin = get_session()
     create_tables(engin)
-    typer.echo("Done!")
+    logger.info(f"Creating tables...")
+    logger.info(f"Done!")
+
     # create the config file
-    typer.echo("Creating config file...")
+    logger.info(f"Creating config file...")
     utils.create_config_file(
         smtp_server=smtp_server, smtp_port=smtp_port, password=password, sender_email=email, is_test=is_test
     )
-    os.chdir("../")
+    logger.info(f"Done!")
 
+    os.chdir("../")
     session.close()
     engin.dispose()
     return
 
 
 @app.command()
 def register(
-    email: str = typer.Option(
-        get_config_dict().get("user", None),
-        "--email",
-        "-e",
-        prompt="What is your email address?",
-        help="Your email address.",
-    ),
-    contact_list: Path = typer.Argument(
+        email: str = typer.Option(
+            "default",
+            "--email",
+            "-e",
+            prompt="What is your email address?",
+            help="Your email address.",
+        ),
+        contact_list: Path = typer.Argument(
             ...,
             exists=True,
             help="The path to your contact list.",
         ),
-    title: str = typer.Option(
-        "Contact List",
-        "--title",
-        "-T",
-        prompt="What is the title of your contact list?",
-        help="The title of your contact list.",
-    ),
-    custom_pdf: bool = typer.Option(
-        False,
-        "--custom-pdf",
-        "-CA",
-        help="Convert your contact list to pdf.",
-    ),
-    attachment: Path = typer.Option(
-        None,
-        "--attachment",
-        "-a",
-        help="The path to the attachment file.",
-    ),
-    custom_pdf_dir: Path = typer.Option(
-        None,
-        "--custom-pdf-dir",
-        "-cpd",
-        help="The path to the custom pdf directory.",
-    ),
-    subject: str = typer.Option(
-        'None',
-        "--subject",
-        "-s",
-        prompt="What is the subject of your email?",
-        help="The subject of your email.",
-    ),
-    template: Optional[Path] = typer.Option(
-        None,
-        "--template",
-        "-t",
-        # exists=True,
-        # file_okay= True,
-        help="The body of your email.",
-    ),
+        title: str = typer.Option(
+            "Contact List",
+            "--title",
+            "-T",
+            prompt="What is the title of your contact list?",
+            help="The title of your contact list.",
+        ),
+        custom_pdf: bool = typer.Option(
+            False,
+            "--custom-pdf",
+            "-CA",
+            help="Convert your contact list to pdf.",
+        ),
+        attachment: Path = typer.Option(
+            None,
+            "--attachment",
+            "-a",
+            help="The path to the attachment file.",
+        ),
+        custom_pdf_dir: Path = typer.Option(
+            None,
+            "--custom-pdf-dir",
+            "-cpd",
+            help="The path to the custom pdf directory.",
+        ),
+        subject: str = typer.Option(
+            'None',
+            "--subject",
+            "-s",
+            prompt="What is the subject of your email?",
+            help="The subject of your email.",
+        ),
+        template: Optional[Path] = typer.Option(
+            None,
+            "--template",
+            "-t",
+            help="The body of your email.",
+        ),
 
 ) -> None:
     """Register your email account."""
+    logger = init_logger('cli')
     if os.path.exists('./mail.db') and os.path.exists('./config.cfg'):
-        from automail.storage import util
-        from automail import utils
-
         if template is None:
             tmp = typer.confirm("Do you want to use template?", default=False)
             if tmp:
                 while True:
                     template = typer.prompt("Please enter the path to your template file.", type=Path)
                     if os.path.isfile(template) and (template.suffix == '.txt' or template.suffix == '.html'):
                         template = str(template)
                         break
                     else:
                         typer.secho(f"File {template} does not exist. or the file type is not supported. "
                                     f"the file type should be .txt or .html", fg=typer.colors.RED)
                         continue
-        print(title)
         if not os.path.exists(title):
             shutil.os.mkdir(title)
         else:
-            typer.secho(f"Directory {title} already exists. Please choose another title.", fg=typer.colors.RED)
+            logger.error(f"Directory {title} already exists. Please choose another title.")
             raise typer.Exit(code=0)
 
         shutil.copy(contact_list, title)
         contact_list = os.path.join(title, os.path.basename(contact_list))
 
         if attachment:
             shutil.copy(attachment, title)
             attachment = os.path.join(title, os.path.basename(attachment))
         if template:
             shutil.copy(template, title)
             template = os.path.join(title, os.path.basename(template))
 
-        typer.echo("Registering your email account...")
+        logger.info(f"Registering your email account...")
+        if email == "default":
+            email = get_config_dict()["user"]
         util.register_new_process(
             email=email,
             contact_list=contact_list,
             title=title,
             custom_pdf=custom_pdf,
             attachment=attachment,
-            custom_pdf_dir=custom_pdf_dir,
+            custom_pdf_dir=str(custom_pdf_dir),
             subject=subject,
             template=template,
         )
 
     else:
-        typer.secho("Please initialize the automail project first.", fg=typer.colors.RED)
+        logger.error("Please initialize the automail project first.")
         raise typer.Exit(code=0)
 
 
 @app.command()
 def start(
-    id: Optional[int] = typer.Argument(
-        None,
-        help="The id of the process.",
-    ),
-    is_test: bool = typer.Option(
-        False,
-        "--test",
-        "-t",
-        help="Test output.",
-    ),
+        pid: Optional[int] = typer.Argument(
+            None,
+            help="The id of the process.",
+        ),
 ) -> None:
     """Start sending emails."""
+    logger = init_logger('cli')
     if os.path.exists('./mail.db') and os.path.exists('./config.cfg'):
-        from automail.storage import util, Process, Record
-
-        print("Starting...")
-    if id is None:
-        typer.secho("Please enter the id of the process.", fg=typer.colors.RED)
-        raise typer.Exit(code=0)
+        logger.info("Starting...")
+        if pid is None:
+            logger.error("Please enter the id of the process.")
+            raise typer.Exit(code=0)
+        else:
+            run_process(pid=pid, is_resume=False)
     else:
-        run_process(pid=id, resume=False)
+        logger.error("Please initialize the automail project first.")
+        raise typer.Exit(code=0)
 
 
 @app.command()
 def resume(
-    id: Optional[int] = typer.Argument(
-        None,
-        help="The id of the process.",
-    ),
-    is_test: bool = typer.Option(
-        False,
-        "--test",
-        "-t",
-        help="Test output.",
-    ),
+        pid: Optional[int] = typer.Argument(
+            None,
+            help="The id of the process.",
+        ),
+
 ) -> None:
     """Resume sending emails."""
+    logger = init_logger('cli')
     if os.path.exists('./mail.db') and os.path.exists('./config.cfg'):
-        from automail.storage import util, Process, Record
-
-        print("Resuming...")
-    if id is None:
-        typer.secho("Please enter the id of the process.", fg=typer.colors.RED)
-        raise typer.Exit(code=0)
+        logger.info("Resuming...")
+        if pid is None:
+            typer.secho("Please enter the id of the process.", fg=typer.colors.RED)
+            raise typer.Exit(code=0)
+        else:
+            run_process(pid=pid, is_resume=True)
     else:
-        run_process(pid=id, resume=True)
+        logger.error("Please initialize the automail project first.")
+        raise typer.Exit(code=0)
 
 
 @app.command()
 def stop(
-    id: Optional[int] = typer.Argument(
-        None,
-        help="The id of the process.",
-    ),
-    is_test: bool = typer.Option(
-        False,
-        "--test",
-        "-t",
-        help="Test output.",
-    ),
+        pid: Optional[int] = typer.Argument(
+            None,
+            help="The id of the process.",
+        ),
 ) -> None:
-    """Stop sending emails."""
+    """Stop a process."""
+    logger = init_logger('cli')
     if os.path.exists('./mail.db') and os.path.exists('./config.cfg'):
-        from automail.storage import util, Process, Record
-
-        print("Stopping...")
-    if id is None:
-        """This function will stop a process with a specific id"""
-        session, engin = get_session()
-        create_tables(engin)
-
-        session.close()
-        engin.dispose()
-        process = session.query(Process).filter(Process.id == pid).first()
-        if process.status == "in progress":
-            process.status = "paused"
-            session.commit()
-            print(f"ID: {pid} => Pausing the program")
+        logger.info("Stopping...")
+        if pid is None:
+            logger.error("Please enter the id of the process.")
+            raise typer.Exit(code=0)
         else:
-            print(f"ID: {pid} => Program is not running")
+            session, engin = get_session()
+            process = session.query(Process).filter(Process.id == pid).first()
+            if process is None:
+                logger.error(f"Process with id {pid} does not exist.")
+                session.close()
+                engin.dispose()
+                raise typer.Exit(code=0)
+            if process.status == "in progress":
+                process.status = "paused"
+                session.commit()
+                logger.info(f"ID: {pid} => Pausing the program.")
+            else:
+                logger.warning(f"ID: {pid} => Program is not in progress.")
+            session.close()
+            engin.dispose()
+    else:
+        logger.error("Please initialize the automail project first.")
+        raise typer.Exit(code=0)
 
 
 @app.command()
 def delete_process(
-    id: Optional[int] = typer.Argument(
-        None,
-        help="The id of the process.",
-    ),
-    dry_run: bool = typer.Option(
-        False,
-        "--dry-run",
-        "-d",
-        help="Test output.",
-    ),
+        pid: Optional[int] = typer.Argument(
+            None,
+            help="The id of the process.",
+        ),
+        dry_run: bool = typer.Option(
+            False,
+            "--dry-run",
+            "-d",
+            help="Test output.",
+        ),
 ) -> None:
     """Delete a process."""
+    logger = init_logger('cli')
     if os.path.exists('./mail.db') and os.path.exists('./config.cfg'):
         from automail.storage import util, Process, Record
-
-        print("Deleting...")
-    if id is None:
-        typer.secho("Please enter the id of the process.", fg=typer.colors.RED)
-        raise typer.Exit(code=0)
-    else:
-        session, engin = get_session()
-
-        process = session.query(Process).filter(Process.id == id).first()
-        if process is None:
-            typer.secho(f"Process with id {id} does not exist.", fg=typer.colors.RED)
+        logger.info("Deleting...")
+        if pid is None:
+            typer.secho("Please enter the id of the process.", fg=typer.colors.RED)
             raise typer.Exit(code=0)
         else:
-            if dry_run:
-                typer.echo(f"Process with id {id} will be deleted.")
+            session, engin = get_session()
+
+            process = session.query(Process).filter(Process.id == pid).first()
+            if process is None:
+                logger.error(f"Process with id {pid} does not exist.")
+                raise typer.Exit(code=0)
             else:
-                session.delete(process)
-                session.commit()
-                typer.echo(f"Process with id {id} has been deleted.")
-                shutil.rmtree(process.title)
-        session.close()
-        engin.dispose()
+                if dry_run:
+                    logger.info(f"Process with id {pid} will be deleted.")
+                else:
+                    session.delete(process)
+                    session.commit()
+                    logger.info(f"Process with id {pid} has been deleted.")
+                    shutil.rmtree(process.title)
+            session.close()
+            engin.dispose()
+    else:
+        logger.error("Please initialize the automail project first.")
+        raise typer.Exit(code=0)
 
 
 @app.command()
 def delete_record(
-    id: Optional[int] = typer.Argument(
-        None,
-        help="The id of the record.",
-    ),
-    dry_run: bool = typer.Option(
-        False,
-        "--dry-run",
-        "-d",
-        help="Test output.",
-    ),
+        rid: Optional[int] = typer.Argument(
+            None,
+            help="The id of the record.",
+        ),
+        dry_run: bool = typer.Option(
+            False,
+            "--dry-run",
+            "-d",
+            help="Test output.",
+        ),
 ) -> None:
-    """Delete a record."""
+    """Delete a record by ID."""
+    logger = init_logger('cli')
     if os.path.exists('./mail.db') and os.path.exists('./config.cfg'):
-        from automail.storage import util, Process, Record
-
-        print("Deleting...")
-    if id is None:
-        typer.secho("Please enter the id of the record.", fg=typer.colors.RED)
-        raise typer.Exit(code=0)
-    else:
-        session, engin = get_session()
-
-        record = session.query(Record).filter(Record.id == id).first()
-        if record is None:
-            typer.secho(f"Record with id {id} does not exist.", fg=typer.colors.RED)
+        logger.info("Deleting...")
+        if rid is None:
+            logger.error("Please enter the id of the record.")
             raise typer.Exit(code=0)
         else:
-            if dry_run:
-                typer.echo(f"Record with id {id} will be deleted.")
+            session, engin = get_session()
+            record = session.query(Record).filter(Record.id == rid).first()
+            if record is None:
+                logger.error(f"Record with id {rid} does not exist.")
+                raise typer.Exit(code=0)
             else:
-                session.delete(record)
-                session.commit()
-                typer.echo(f"Record with id {id} has been deleted.")
-        session.close()
-        engin.dispose()
+                if dry_run:
+                    logger.info(f"Record with id {rid} will be deleted.")
+                else:
+                    session.delete(record)
+                    session.commit()
+                    logger.info(f"Record with id {rid} has been deleted.")
+            session.close()
+            engin.dispose()
+    else:
+        logger.error("Please initialize the automail project first.")
+        raise typer.Exit(code=0)
 
 
-@app.command()
-def list() -> None:
+@app.command("list")
+def list_processes() -> None:
     """List all processes."""
+    logger = init_logger('cli')
     if os.path.exists('./mail.db') and os.path.exists('./config.cfg'):
-        from automail.storage import util, Process, Record
-
-        print("Listing...")
-    session, engin = get_session()
-    create_tables(engin)
+        logger.info("Listing...")
+        session, engin = get_session()
+        create_tables(engin)
 
-    processes = session.query(Process).all()
-    if len(processes) == 0:
-        typer.echo("There is no process.")
-    else:
-        for process in processes:
-            typer.echo(
-                f"ID: {process.id} | Title: {process.title} | Status: {process.status}"
-            )
-    session.close()
-    engin.dispose()
+        processes = session.query(Process).all()
+        if len(processes) == 0:
+            logger.warning("There is no process.")
+        else:
+            for process in processes:
+                logger.info(f"ID: {process.id} | Title: {process.title} | Status: {process.status}")
+        session.close()
+        engin.dispose()
 
 
 @app.command()
 def list_records(
         process_id: Optional[int] = typer.Argument(
             None,
             help="The id of the process.",
         )) -> None:
-    """List all records."""
+    """List all records of one process."""
+    logger = init_logger('cli')
     if os.path.exists('./mail.db') and os.path.exists('./config.cfg'):
-        from automail.storage import util, Process, Record
-
-        print("Listing...")
-    session, engin = get_session()
-    create_tables(engin)
+        logger.info("Listing...")
+        session, engin = get_session()
+        create_tables(engin)
 
-    if process_id is None:
-        records = session.query(Record).all()
-    else:
-        records = (
-            session.query(Record).filter(Record.process_id == process_id).all()
-        )
-    if len(records) == 0:
-        typer.echo("There is no record.")
-    else:
-        for record in records:
-            typer.echo(
-                f"ID: {record.id} | Process ID: {record.process_id} | Email: {record.receiver} | Status: {record.status}"
+        if process_id is None:
+            records = session.query(Record).all()
+        else:
+            records = (
+                session.query(Record).filter(Record.process_id == process_id).all()
             )
-    session.close()
-    engin.dispose()
+        if len(records) == 0:
+            logger.warning("There is no record.")
+        else:
+            for record in records:
+                logger.info(f"ID: {record.id} | Process ID: {record.process_id} | Email: {record.receiver} |"
+                            f" Status: {record.status}"
+                            )
+        session.close()
+        engin.dispose()
+    else:
+        logger.error("Please initialize the automail project first.")
+        raise typer.Exit(code=0)
+
 
 if __name__ == "__main__":
     app(prog_name=__app_name__)
```

### Comparing `pyautomail-1.5.1.4/automail/config/config.py` & `pyautomail-1.6.0.0/automail/config/config.py`

 * *Files identical despite different names*

### Comparing `pyautomail-1.5.1.4/automail/emailsender.py` & `pyautomail-1.6.0.0/automail/emailsender.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,19 +87,20 @@
         self.template = None
         self.__test_flg = is_test
         self.user = user
         self.host = host
         self.port = port
         self.password = None
 
+        print(password)
+        print("-" * 100)
         if not self.__test_flg:
             self.__logger.info("Connecting to SMTP server...")
 
             self.password = password
-
             self.server = smtplib.SMTP_SSL(self.host, self.port)
             self.__logger.info("Connected to SMTP server.")
             self.__logger.info(f"Logging in to user account: {self.user}...")
             self.server.login(self.user, self.password)
             self.__logger.info("Logged in.")
         else:
             self.__logger.warning("Test Mode is enabled. In this mode no email will be sent.")
@@ -237,8 +238,8 @@
             else:
                 output = self.server.sendmail(self.user, receiver_email_address, message.as_string())
                 output['test'] = False
                 output['err'] = 'none'
         except Exception as e:
             self.__logger.error("Error sending email to: " + receiver_email_address + " error: " + str(e))
             return {'test': self.__test_flg, 'err': str(e)}
-        return output
+        return output
```

### Comparing `pyautomail-1.5.1.4/automail/manager.py` & `pyautomail-1.6.0.0/automail/manager.py`

 * *Files identical despite different names*

### Comparing `pyautomail-1.5.1.4/automail/storage/model.py` & `pyautomail-1.6.0.0/automail/storage/model.py`

 * *Files identical despite different names*

### Comparing `pyautomail-1.5.1.4/automail/storage/util.py` & `pyautomail-1.6.0.0/automail/storage/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,15 @@
 
     process = Process(title=title, subject=subject, sender=email,
                       temp_file=template, release_date=datetime.datetime.date(datetime.datetime.now()))
 
     session.add(process)
     session.commit()
 
-    print(f"ID:{process.id} => Registering user {email} with contacts {contact_list}")
+    print(f"ID: {process.id} => Registering Process {email} with contacts {contact_list}")
     contact_df = pd.read_csv(contact_list)
     for index, row in contact_df.iterrows():
         filename = None
         if attachment:
             filename = attachment.strip()
 
         if custom_pdf:
```

### Comparing `pyautomail-1.5.1.4/automail/utils.py` & `pyautomail-1.6.0.0/automail/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 import sys
 import configparser
-import multiprocessing
+import coloredlogs
+
 
 def init_logger(name=''):
     """This function will initialize a logger object
 
     Parameters
     ----------
     name : str
@@ -39,39 +40,41 @@
     [2019-08-20 15:30:00,000 - ERROR (EmailSender) ] : error message
     >>> logger_obj.critical('critical message')
     [2019-08-20 15:30:00,000 - CRITICAL (EmailSender) ] : critical message
 
 
     """
     logger_obj = logging.getLogger(name)
-    # logger_obj = multiprocessing.get_logger(name)
+    coloredlogs.install(level='DEBUG', logger=logger_obj, fmt='[%(asctime)s - %(levelname)s (%(name)s) ] : %(message)s')
     logger_obj.setLevel(logging.DEBUG)
     formatter = logging.Formatter('[%(asctime)s - %(levelname)s (%(name)s) ] : %(message)s')
-    handler1 = logging.StreamHandler(sys.stdout)
-    handler1.setFormatter(formatter)
-    # handler2 = logging.FileHandler('../emailsender.log')
-    # handler2.setFormatter(formatter)
-    logger_obj.addHandler(handler1)
-    # logger_obj.addHandler(handler2)
+    # handler1 = logging.StreamHandler(sys.stdout)
+    # handler1.setFormatter(formatter)
+    handler2 = logging.FileHandler('../emailsender.log')
+    handler2.setFormatter(formatter)
+    # logger_obj.addHandler(handler1)
+    logger_obj.addHandler(handler2)
     return logger_obj
 
 
 def create_config_file(smtp_server, smtp_port, sender_email='', password='', is_test=False):
     """This function will create a config file for the email sender.
 
     Parameters
     ----------
     smtp_server : str
         The SMTP server address.
     smtp_port : int
         The SMTP server port.
     sender_email : str
         The email address of the sender.
-    sender_password : str
+    password : str
         The password of the sender.
+    is_test : bool
+        If True, the email will not be sent.
 
     Notes
     -----
     This function will create a config file with the following format::
 
         [SMTP]
         server = smtp.gmail.com
@@ -144,8 +147,8 @@
     config_dict = {
         'smtp_server': config.get('smtp', 'server', fallback=''),
         'smtp_port': config.getint('smtp', 'port', fallback=0),
         'is_test': config.getboolean('smtp', 'is_test', fallback=False),
         'user': config.get('account', 'user', fallback=''),
         'password': config.get('account', 'password', fallback='')
     }
-    return config_dict
+    return config_dict
```

### Comparing `pyautomail-1.5.1.4/docs/Makefile` & `pyautomail-1.6.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyautomail-1.5.1.4/docs/_static/automail-logo.png` & `pyautomail-1.6.0.0/docs/_static/automail-logo.png`

 * *Files identical despite different names*

### Comparing `pyautomail-1.5.1.4/docs/_templates/apidoc/package.rst_t` & `pyautomail-1.6.0.0/docs/_templates/apidoc/package.rst_t`

 * *Files identical despite different names*

### Comparing `pyautomail-1.5.1.4/docs/api/automail.rst` & `pyautomail-1.6.0.0/docs/api/automail.rst`

 * *Files identical despite different names*

### Comparing `pyautomail-1.5.1.4/docs/conf.py` & `pyautomail-1.6.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyautomail-1.5.1.4/docs/getting-started.rst` & `pyautomail-1.6.0.0/docs/getting-started.rst`

 * *Files identical despite different names*

### Comparing `pyautomail-1.5.1.4/docs/index.rst` & `pyautomail-1.6.0.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pyautomail-1.5.1.4/docs/introduction.rst` & `pyautomail-1.6.0.0/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `pyautomail-1.5.1.4/docs/make.bat` & `pyautomail-1.6.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyautomail-1.5.1.4/docs/tutorial/index.rst` & `pyautomail-1.6.0.0/docs/tutorial/index.rst`

 * *Files identical despite different names*

### Comparing `pyautomail-1.5.1.4/document.pdf` & `pyautomail-1.6.0.0/document.pdf`

 * *Files identical despite different names*

### Comparing `pyautomail-1.5.1.4/pyautomail.egg-info/PKG-INFO` & `pyautomail-1.6.0.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyautomail
-Version: 1.5.1.4
+Version: 1.6.0.0
 Summary: Automated Email Sending for Large Scale Email and Gmail Automation
 Home-page: https://github.com/msinamsina/pyautomail
 Author: Mohammad sina Allahkaram
 Author-email: msinamsina@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/msinamsina/pyautomail/issues
 Project-URL: Changelog, https://github.com/msinamsina/pyautomail/releases
@@ -15,17 +15,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # PyAutoMail: A Python package and command-line interface for automation sending email to your contact list
 
 
-<p align="center" width="100%">
-    <img  width="80%" src="https://github.com/msinamsina/automail/blob/main/docs/_static/automail-logo.png?raw=true" >
-</p>
+![pyautomail-image](./docs/_static/automail-logo.png)
 
 
 Pyautomail, an incredibly powerful Python package meticulously crafted for the purpose of automated email delivery, catering especially to large-scale Email or Gmail automation. In today's fast-paced digital era, effective communication stands as a crucial cornerstone for numerous businesses and projects that heavily rely on email as their primary medium of interaction. Nonetheless, the manual handling of individual emails or the management of bulk email campaigns can prove to be both time-consuming and prone to errors.
 
 Fear not, for pyautomail swoops in as the ultimate savior, offering a seamless and highly efficient solution for automating email communication. Be it the need to dispatch personalized emails to a vast audience, the execution of targeted email marketing campaigns, or the automation of repetitive email chores, this package serves as your ultimate go-to tool. With its user-friendly interface and an array of versatile features, pyautomail proves itself as a fitting choice for a wide range of applications, catering to startups, enterprises, professionals, and developers alike.
 
 Revolutionize your email operations, whether it involves mass email distribution, streamlined Gmail tasks, or the quest for enhanced email communication proficiency - pyautomail is here to streamline your workflow, elevate your efficiency, and elevate productivity to soaring heights.
@@ -34,49 +32,100 @@
 ## Installation
 
 ### [PyPi](https://pypi.org/project/pyautomail/)
 ```bash
 pip install pyautomail
 ```
 
-### Github
+### [Github](https://github.com/msinamsina/pyautomail.git)
 ```bash
-pip install git+https://github.com/msinamsina/automail.git
+pip install git+https://github.com/msinamsina/pyautomail.git
 ```
 
 ## How to use in command-line interface
-At first, you should register your email address and contact list
-```bash
-automail register <your-email-address> <Path-to-your-contact-list> [options]
-```
-Then you can send email to your contact list
-```bash
-automail start <process-id>
-```
+
+1. At first, you should initialize project
+    ```bash
+    pyhhon -m automail init
+    ```
+    
+   After running this command, you will see a some questions. You should answer them.
+    
+   ```bash
+   Where do you want to initialize the automail project? [./automail-workspace]
+   What is your smtp server? [smtp.gmail.com]:
+   What is your smtp port? [465]:
+   ```
+   
+    **📘 Note:**   
+    1. This command will create a folder with the project name in the path you specified. 
+    If you don't specify the path, it will create ```automail-workspace```.  
+    2. You can change the default smtp server by default it has been set on **Gmail Smtp Server**. 
+    3. You also can set the port of **Smtm Server** (by default 465).
+    4. Additionally, if you want to save you password in config file, you can use the ```-p``` or 
+   ```--pasword``` switch.
+    5. Moreover, if you want to initialize a test project, you can use ```-t``` or ```--test```. 
+       ```bash
+       $ pyhhon -m automail init -t -p <your-password>
+       ```
+
+   > **[📙 Important]()**  
+   > If directory already exists, it will be overwritten.
+   
+1. Then you should go to the project directory and register your contact list
+    ```bash
+    cd <your-project-name>
+    pyhhon -m automail register <Path-to-your-contact-list> [options]
+   ```
+   **📘 Note:**   
+   For using a template, use ```--template``` switch. The template can be ```.txt``` or ```.html```
+   Format.
+   ```bash
+   pyhhon -m automail register contact-list.csv --template ./body.html
+   ```
+   **body.html:**
+   ```html
+   <h1> Hi {{ name }}, </h1>
+   ```
+   **contact-list.csv:**
+   ```csv
+   email,name,data1,cpdf
+   contact1@gmail.com,contact1,ali,/path/to/pdf1
+   contact2@gmail.com,contact2,mohammad,/path/to/pdf2
+   contact3@gmail.com,contact3,soheila,/path/to/pdf3
+   ```
+   
+1. Now you can start sending emails by running the following command
+   ```bash
+   pyhhon -m automail start <process-id>
+   ```
+   
 ## How to use in python
 ```python
     from automail import EmailSender
     email_sender = EmailSender()
     email_sender.set_template('body.txt')
     data = {'name': 'Jon', 'age': 30}
     email_sender.send('msinamsina@gmail.com', 'sub1', data)
 ```
 
-### Documentation and Resources
+## Documentation and Resources
 
-For more comprehensive information about **PyAutoMail** and its capabilities, please explore our detailed [documentation](https://automail.readthedocs.io/en/latest/).
+For more comprehensive information about **PyAutoMail** and its capabilities, please explore our detailed [documentation](https://pyautomail.readthedocs.io/en/latest/).
 
-- Get a brief overview and explore the features of PyAutoMail in the [Introduction](https://automail.readthedocs.io/en/latest/introduction.html) section.
-- If you're new to PyAutoMail, follow our [Getting Started](https://automail.readthedocs.io/en/latest/getting-started.html) guide to kickstart your email automation journey.
-- For a quick reference, you can check out the [API Reference](https://automail.readthedocs.io/en/latest/api/index.html) section.
-- To gain deeper insights into PyAutoMail and learn best practices, dive into our informative [Tutorial](https://automail.readthedocs.io/en/latest/tutorial/index.html) section.
+- Get a brief overview and explore the features of PyAutoMail in the [Introduction](https://pyautomail.readthedocs.io/en/latest/introduction.html) section.
+- If you're new to PyAutoMail, follow our [Getting Started](https://pyautomail.readthedocs.io/en/latest/getting-started.html) guide to kickstart your email automation journey.
+- For a quick reference, you can check out the [API Reference](https://pyautomail.readthedocs.io/en/latest/api/index.html) section.
+- To gain deeper insights into PyAutoMail and learn best practices, dive into our informative [Tutorial](https://pyautomail.readthedocs.io/en/latest/tutorial/index.html) section.
 
 By exploring these resources, you'll harness the full potential of PyAutoMail and make the most out of its powerful email automation capabilities.
 
-### Contribution and Support
+---
+
+## Contribution and Support
 
 We welcome contributions from the community to enhance **PyAutoMail** and make it even more robust. If you're interested in contributing, here's how you can get involved:
 
 1. **Bug Reports and Feature Requests**: If you come across any issues or have ideas for new features, please [open an issue](https://github.com/msinamsina/automail/issues) on our GitHub repository. We appreciate detailed bug reports with steps to reproduce the problem and clear feature requests with use cases.
 
 2. **Pull Requests**: If you want to contribute code to PyAutoMail, you can do so by submitting a pull request. Please ensure that your code adheres to the existing code style, and include relevant tests to maintain code quality.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyautomail-1.5.1.4/pyautomail.egg-info/SOURCES.txt` & `pyautomail-1.6.0.0/pyautomail.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyautomail-1.5.1.4/sending_gmail.py` & `pyautomail-1.6.0.0/sending_gmail.py`

 * *Files identical despite different names*

### Comparing `pyautomail-1.5.1.4/setup.cfg` & `pyautomail-1.6.0.0/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -21,14 +21,17 @@
 packages = find:
 python_requires = >=3.9
 install_requires = 
 	sqlalchemy
 	sqlalchemy_utils
 	jinja2
 	pandas
+	coloredlogs
+	pytest
+	typer
 
 [options.packages.find]
 where = ./
 
 [options.entry_points]
 console_scripts = 
 	automail = automail.manager:main
```

### Comparing `pyautomail-1.5.1.4/setup.py` & `pyautomail-1.6.0.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,18 @@
     author='Mohammad sina Allahkaram',
     author_email="msinamsina@gmail.com",
     description='Automated Email Sending for Large Scale Email and Gmail Automation',
     install_requires=[
         'sqlalchemy',
         'sqlalchemy_utils',
         'jinja2',
-        'pandas'
+        'pandas',
+        'coloredlogs',
+        'pytest',
+        'typer'
     ],
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     python_requires='>=3.9',
     entry_points={
         'console_scripts': [
             'automail = automail.manager:main',
```

### Comparing `pyautomail-1.5.1.4/tests/test_cli/test_cli_init.py` & `pyautomail-1.6.0.0/tests/test_cli/test_cli_init.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,24 +52,24 @@
 
 
 def test_init_3():
     # enter a path that already exists and choose not to delete it
     result = runner.invoke(cli.app, ["init"], input="test")
     usual_output(result)
     assert "Directory test already exists." in result.stdout
-    assert "Do you want to delete it? [y/N]: " in result.stdout
+    assert "Do you want to delete test directory? [y/N]: " in result.stdout
     assert "Initializing automail database..." not in result.stdout
     assert "Aborted!" in result.stdout
 
 
 def _helper_init(result):
     assert result.exit_code == 0
     assert "Directory test already exists." in result.stdout
-    assert "Do you want to delete it? [y/N]: " in result.stdout
-    assert "Deleting..." in result.stdout
+    assert "Do you want to delete test directory? [y/N]: " in result.stdout
+    assert "Deleting test directory" in result.stdout
     assert "Initializing automail database..." in result.stdout
     assert "Done!" in result.stdout
 
     assert os.path.exists("test") is True
     assert os.path.exists("test/mail.db") is True
```

### Comparing `pyautomail-1.5.1.4/tests/test_cli/test_cli_other.py` & `pyautomail-1.6.0.0/tests/test_cli/test_cli_register.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,61 +1,81 @@
 from typer.testing import CliRunner
 import typer
 import shutil
 import os
 from automail import cli
 from automail.storage import get_session, Process, Record
+from automail.utils import get_config_dict
 import pytest
 import tempfile
-import time
 
 runner = CliRunner()
 
 
 @pytest.fixture(scope="module", autouse=True)
 def setup():
     # create a temporary directory
     test_dir = tempfile.mkdtemp()
     os.chdir(test_dir)
     # initialize the automail project
-    runner.invoke(cli.app, ["init", "-db", "test-reg", "-ss", "smtp.gmail.com", "-sp", "111", "-t"], input="y\n")
+    runner.invoke(cli.app, ["init", "-db", "test-reg", "-ss", "smtp.gmail.com", "-sp", "111", "-t", '-e', 'example@gmail.com'], input="y\n")
 
     # create a contact list
     with open("contact.csv", "w") as f:
         f.write("name,email\n")
         f.write("John Doe,john@gmail.com\n")
         f.write("Jane Doe,jane@gmail.com\n")
     # create a template
     with open("template.html", "w") as f:
         f.write("<h1>Hello {{ name }}!</h1>")
 
     # go to the project directory
     os.chdir("test-reg")
 
-    # register the contact list
-    runner.invoke(cli.app, ["register", "../contact.csv", "-t", '../template.html'])
+    assert get_config_dict()["user"] == "example@gmail.com"
 
     yield
     # remove the directory after the test
     os.chdir("../..")
-    # shutil.rmtree(test_dir)
+    shutil.rmtree(test_dir, ignore_errors=True)
 
 
-def test_start_1():
-    """Test if the process is started"""
-    result = runner.invoke(cli.app, ["start"])
-    assert result.exit_code == 0
-    assert "Please enter the id of the process." in result.output
+def test_register_1():
+    """Test if there is no contactlist the error is raised"""
+    result = runner.invoke(cli.app, ["register"])
+    assert result.exit_code == 2
+    assert "Error: Missing argument 'CONTACT_LIST'." in result.output
+
+
+def test_register_2():
+    """Test is the contactlist is not existed the error is rased"""
+    try:
+        os.remove("contact.csv")
+    except FileNotFoundError:
+        pass
+    result = runner.invoke(cli.app, ["register", "contact.csv"])
+    assert result.exit_code == 2
+    assert "Error: Invalid value for 'CONTACT_LIST': Path 'contact.csv' does not exist." in result.output
+
 
+def test_register_3():
+    """Test a registration process"""
 
-def test_start_2():
-    """Test if the process is started"""
-    result = runner.invoke(cli.app, ["start", "1"], input="y\n")
+    shutil.rmtree("Contact List", ignore_errors=True)
+
+    result = runner.invoke(cli.app, ["register", "../contact.csv"])
     assert result.exit_code == 0
-    assert "Starting..." in result.output
-    # assert "Process 1 is finished." in result.output
-    assert "Sending email to: john@gmail.com" in result.output
-    assert "<h1>Hello John Doe!</h1>" in result.output
-    assert "Sending email to: jane@gmail.com" in result.output
-    assert "<h1>Hello Jane Doe!</h1>" in result.output
-    assert "Program finished successfully" in result.output
+    print(result.output)
+
+    assert " => Registering Process example@gmail.com with contacts Contact List\\contact.csv" in result.output
+    assert " => Registering record for john@gmail.com" in result.output
+    assert " => Registering record for jane@gmail.com" in result.output
+    assert os.path.exists("Contact List/contact.csv")
+
+    # check the database
+    # go to the Contact List folder
+    session, engine = get_session()
+    assert session.query(Process).filter(Process.title == "Contact List").count() == 1
+
+    session.close()
+    engine.dispose()
```

### Comparing `pyautomail-1.5.1.4/tests/test_manager.py` & `pyautomail-1.6.0.0/tests/test_manager.py`

 * *Files identical despite different names*

