# Comparing `tmp/mkdocstrings_python-1.2.0.tar.gz` & `tmp/mkdocstrings_python-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocstrings_python-1.2.0.tar", last modified: Fri Jul 14 17:33:42 2023, max compression
+gzip compressed data, was "mkdocstrings_python-1.2.1.tar", last modified: Thu Jul 20 13:08:00 2023, max compression
```

## Comparing `mkdocstrings_python-1.2.0.tar` & `mkdocstrings_python-1.2.1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
--rw-r--r--   0        0        0      754 2023-07-13 17:32:07.041776 mkdocstrings_python-1.2.0/LICENSE
--rw-r--r--   0        0        0     4243 2023-07-13 17:32:09.575077 mkdocstrings_python-1.2.0/README.md
--rw-r--r--   0        0        0     2559 2023-07-14 17:33:42.779897 mkdocstrings_python-1.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-13 17:32:06.915111 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/py.typed
--rw-r--r--   0        0        0      326 2023-05-01 15:54:09.233042 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/__init__.py
--rw-r--r--   0        0        0    19005 2023-07-13 18:33:11.207661 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/handler.py
--rw-r--r--   0        0        0     8853 2023-07-13 18:49:48.868895 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/rendering.py
--rw-r--r--   0        0        0     2896 2023-07-14 15:56:20.488607 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/attribute.html
--rw-r--r--   0        0        0     5757 2023-07-13 17:31:51.141977 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/children.html
--rw-r--r--   0        0        0     4765 2023-07-14 15:49:17.999012 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/class.html
--rw-r--r--   0        0        0     1740 2023-03-03 13:20:57.896481 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring.html
--rw-r--r--   0        0        0      274 2023-05-01 15:54:09.233042 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/admonition.html
--rw-r--r--   0        0        0     2827 2023-07-13 18:33:11.207661 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/attributes.html
--rw-r--r--   0        0        0      460 2023-07-13 18:33:11.207661 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/examples.html
--rw-r--r--   0        0        0     2853 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/other_parameters.html
--rw-r--r--   0        0        0     3561 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/parameters.html
--rw-r--r--   0        0        0     2478 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/raises.html
--rw-r--r--   0        0        0     3490 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/receives.html
--rw-r--r--   0        0        0     3465 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/returns.html
--rw-r--r--   0        0        0     2453 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/warns.html
--rw-r--r--   0        0        0     3430 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/yields.html
--rw-r--r--   0        0        0      674 2023-06-27 20:55:41.620344 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/expression.html
--rw-r--r--   0        0        0     2941 2023-07-14 15:55:09.818844 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/function.html
--rw-r--r--   0        0        0      250 2023-06-23 09:39:19.320748 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/labels.html
--rw-r--r--   0        0        0      794 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/languages/en.html
--rw-r--r--   0        0        0      809 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/languages/ja.html
--rw-r--r--   0        0        0      788 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/languages/zh.html
--rw-r--r--   0        0        0     2216 2023-07-14 16:29:48.867591 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/module.html
--rw-r--r--   0        0        0     2790 2023-07-13 18:42:48.068344 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/signature.html
--rw-r--r--   0        0        0       37 2021-11-03 19:53:40.146116 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/attribute.html
--rw-r--r--   0        0        0       36 2021-11-03 19:53:40.146116 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/children.html
--rw-r--r--   0        0        0       33 2021-11-03 19:53:40.146116 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/class.html
--rw-r--r--   0        0        0       37 2021-11-03 19:53:40.146116 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/docstring.html
--rw-r--r--   0        0        0       48 2022-02-01 20:48:46.512716 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/docstring/admonition.html
--rw-r--r--   0        0        0       48 2021-11-03 19:54:24.832142 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/docstring/attributes.html
--rw-r--r--   0        0        0       46 2021-11-03 19:54:24.832142 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/docstring/examples.html
--rw-r--r--   0        0        0       54 2021-11-03 19:54:24.832142 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/docstring/other_parameters.html
--rw-r--r--   0        0        0       48 2021-11-03 19:54:24.832142 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/docstring/parameters.html
--rw-r--r--   0        0        0       44 2021-11-22 18:41:47.281610 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/docstring/raises.html
--rw-r--r--   0        0        0       46 2021-11-22 18:41:51.551545 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/docstring/receives.html
--rw-r--r--   0        0        0       45 2021-11-03 19:54:24.832142 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/docstring/returns.html
--rw-r--r--   0        0        0       43 2021-11-22 18:41:56.598136 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/docstring/warns.html
--rw-r--r--   0        0        0       44 2021-11-03 19:54:24.832142 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/docstring/yields.html
--rw-r--r--   0        0        0       38 2021-11-08 00:26:56.388000 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/expression.html
--rw-r--r--   0        0        0       36 2021-11-03 19:53:40.146116 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/function.html
--rw-r--r--   0        0        0       34 2021-11-03 19:53:40.146116 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/labels.html
--rw-r--r--   0        0        0      431 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/language.html
--rw-r--r--   0        0        0       39 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/languages/en.html
--rw-r--r--   0        0        0       39 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/languages/ja.html
--rw-r--r--   0        0        0       39 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/languages/zh.html
--rw-r--r--   0        0        0       34 2021-11-03 19:53:40.146116 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/module.html
--rw-r--r--   0        0        0       37 2021-11-03 19:53:40.146116 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/signature.html
--rw-r--r--   0        0        0      999 2023-06-04 16:06:08.029138 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/style.css
--rw-r--r--   0        0        0      988 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/attributes.html
--rw-r--r--   0        0        0      994 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/other_parameters.html
--rw-r--r--   0        0        0      988 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/parameters.html
--rw-r--r--   0        0        0      928 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/raises.html
--rw-r--r--   0        0        0     1118 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/receives.html
--rw-r--r--   0        0        0     1067 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/returns.html
--rw-r--r--   0        0        0      923 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/warns.html
--rw-r--r--   0        0        0     1100 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/yields.html
--rw-r--r--   0        0        0      431 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/readthedocs/language.html
--rw-r--r--   0        0        0      328 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/readthedocs/languages/en.html
--rw-r--r--   0        0        0      334 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/readthedocs/languages/ja.html
--rw-r--r--   0        0        0      330 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/readthedocs/languages/zh.html
--rw-r--r--   0        0        0      971 2023-06-03 23:04:52.858439 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/readthedocs/style.css
--rw-r--r--   0        0        0      174 2023-07-13 17:32:06.908444 mkdocstrings_python-1.2.0/tests/__init__.py
--rw-r--r--   0        0        0     3052 2023-07-13 17:32:09.575077 mkdocstrings_python-1.2.0/tests/conftest.py
--rw-r--r--   0        0        0     3295 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.0/tests/test_handler.py
--rw-r--r--   0        0        0     3994 2023-07-13 17:31:51.141977 mkdocstrings_python-1.2.0/tests/test_rendering.py
--rw-r--r--   0        0        0     1332 2023-05-01 15:54:09.233042 mkdocstrings_python-1.2.0/tests/test_themes.py
--rw-r--r--   0        0        0     5697 1970-01-01 00:00:00.000000 mkdocstrings_python-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      754 2023-07-13 17:32:07.041776 mkdocstrings_python-1.2.1/LICENSE
+-rw-r--r--   0        0        0     4243 2023-07-13 17:32:09.575077 mkdocstrings_python-1.2.1/README.md
+-rw-r--r--   0        0        0     2559 2023-07-20 13:08:00.486770 mkdocstrings_python-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-13 17:32:06.915111 mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/py.typed
+-rw-r--r--   0        0        0      326 2023-05-01 15:54:09.233042 mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/__init__.py
+-rw-r--r--   0        0        0    19005 2023-07-13 18:33:11.207661 mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/handler.py
+-rw-r--r--   0        0        0     8895 2023-07-20 13:00:15.028684 mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/rendering.py
+-rw-r--r--   0        0        0     2896 2023-07-14 15:56:20.488607 mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/material/_base/attribute.html
+-rw-r--r--   0        0        0     5757 2023-07-13 17:31:51.141977 mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/material/_base/children.html
+-rw-r--r--   0        0        0     4765 2023-07-14 15:49:17.999012 mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/material/_base/class.html
+-rw-r--r--   0        0        0     1740 2023-03-03 13:20:57.896481 mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring.html
+-rw-r--r--   0        0        0      274 2023-05-01 15:54:09.233042 mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/admonition.html
+-rw-r--r--   0        0        0     2827 2023-07-13 18:33:11.207661 mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/attributes.html
+-rw-r--r--   0        0        0      460 2023-07-13 18:33:11.207661 mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/examples.html
+-rw-r--r--   0        0        0     2853 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/other_parameters.html
+-rw-r--r--   0        0        0     3561 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/parameters.html
+-rw-r--r--   0        0        0     2478 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/raises.html
+-rw-r--r--   0        0        0     3490 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/receives.html
+-rw-r--r--   0        0        0     3465 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/returns.html
+-rw-r--r--   0        0        0     2453 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/warns.html
+-rw-r--r--   0        0        0     3430 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/yields.html
+-rw-r--r--   0        0        0      674 2023-07-20 13:05:33.348084 mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/material/_base/expression.html
+-rw-r--r--   0        0        0     2941 2023-07-14 15:55:09.818844 mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/material/_base/function.html
+-rw-r--r--   0        0        0      250 2023-06-23 09:39:19.320748 mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/material/_base/labels.html
+-rw-r--r--   0        0        0      794 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/material/_base/languages/en.html
+-rw-r--r--   0        0        0      809 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/material/_base/languages/ja.html
+-rw-r--r--   0        0        0      788 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/material/_base/languages/zh.html
+-rw-r--r--   0        0        0     2216 2023-07-14 16:29:48.867591 mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/material/_base/module.html
+-rw-r--r--   0        0        0     2790 2023-07-13 18:42:48.068344 mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/material/_base/signature.html
+-rw-r--r--   0        0        0       37 2021-11-03 19:53:40.146116 mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/material/attribute.html
+-rw-r--r--   0        0        0       36 2021-11-03 19:53:40.146116 mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/material/children.html
+-rw-r--r--   0        0        0       33 2021-11-03 19:53:40.146116 mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/material/class.html
+-rw-r--r--   0        0        0       37 2021-11-03 19:53:40.146116 mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/material/docstring.html
+-rw-r--r--   0        0        0       48 2022-02-01 20:48:46.512716 mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/material/docstring/admonition.html
+-rw-r--r--   0        0        0       48 2021-11-03 19:54:24.832142 mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/material/docstring/attributes.html
+-rw-r--r--   0        0        0       46 2021-11-03 19:54:24.832142 mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/material/docstring/examples.html
+-rw-r--r--   0        0        0       54 2021-11-03 19:54:24.832142 mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/material/docstring/other_parameters.html
+-rw-r--r--   0        0        0       48 2021-11-03 19:54:24.832142 mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/material/docstring/parameters.html
+-rw-r--r--   0        0        0       44 2021-11-22 18:41:47.281610 mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/material/docstring/raises.html
+-rw-r--r--   0        0        0       46 2021-11-22 18:41:51.551545 mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/material/docstring/receives.html
+-rw-r--r--   0        0        0       45 2021-11-03 19:54:24.832142 mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/material/docstring/returns.html
+-rw-r--r--   0        0        0       43 2021-11-22 18:41:56.598136 mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/material/docstring/warns.html
+-rw-r--r--   0        0        0       44 2021-11-03 19:54:24.832142 mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/material/docstring/yields.html
+-rw-r--r--   0        0        0       38 2021-11-08 00:26:56.388000 mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/material/expression.html
+-rw-r--r--   0        0        0       36 2021-11-03 19:53:40.146116 mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/material/function.html
+-rw-r--r--   0        0        0       34 2021-11-03 19:53:40.146116 mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/material/labels.html
+-rw-r--r--   0        0        0      431 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/material/language.html
+-rw-r--r--   0        0        0       39 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/material/languages/en.html
+-rw-r--r--   0        0        0       39 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/material/languages/ja.html
+-rw-r--r--   0        0        0       39 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/material/languages/zh.html
+-rw-r--r--   0        0        0       34 2021-11-03 19:53:40.146116 mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/material/module.html
+-rw-r--r--   0        0        0       37 2021-11-03 19:53:40.146116 mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/material/signature.html
+-rw-r--r--   0        0        0      999 2023-06-04 16:06:08.029138 mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/material/style.css
+-rw-r--r--   0        0        0      988 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/attributes.html
+-rw-r--r--   0        0        0      994 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/other_parameters.html
+-rw-r--r--   0        0        0      988 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/parameters.html
+-rw-r--r--   0        0        0      928 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/raises.html
+-rw-r--r--   0        0        0     1118 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/receives.html
+-rw-r--r--   0        0        0     1067 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/returns.html
+-rw-r--r--   0        0        0      923 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/warns.html
+-rw-r--r--   0        0        0     1100 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/yields.html
+-rw-r--r--   0        0        0      431 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/readthedocs/language.html
+-rw-r--r--   0        0        0      328 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/readthedocs/languages/en.html
+-rw-r--r--   0        0        0      334 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/readthedocs/languages/ja.html
+-rw-r--r--   0        0        0      330 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/readthedocs/languages/zh.html
+-rw-r--r--   0        0        0      971 2023-06-03 23:04:52.858439 mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/readthedocs/style.css
+-rw-r--r--   0        0        0      174 2023-07-13 17:32:06.908444 mkdocstrings_python-1.2.1/tests/__init__.py
+-rw-r--r--   0        0        0     3052 2023-07-13 17:32:09.575077 mkdocstrings_python-1.2.1/tests/conftest.py
+-rw-r--r--   0        0        0     3295 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.1/tests/test_handler.py
+-rw-r--r--   0        0        0     5301 2023-07-20 13:02:26.681181 mkdocstrings_python-1.2.1/tests/test_rendering.py
+-rw-r--r--   0        0        0     1332 2023-05-01 15:54:09.233042 mkdocstrings_python-1.2.1/tests/test_themes.py
+-rw-r--r--   0        0        0     5697 1970-01-01 00:00:00.000000 mkdocstrings_python-1.2.1/PKG-INFO
```

### Comparing `mkdocstrings_python-1.2.0/LICENSE` & `mkdocstrings_python-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.2.0/README.md` & `mkdocstrings_python-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.2.0/pyproject.toml` & `mkdocstrings_python-1.2.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     "Topic :: Utilities",
     "Typing :: Typed",
 ]
 dependencies = [
     "mkdocstrings>=0.20",
     "griffe>=0.30",
 ]
-version = "1.2.0"
+version = "1.2.1"
 
 [project.license]
 text = "ISC"
 
 [project.urls]
 Homepage = "https://mkdocstrings.github.io/python"
 Documentation = "https://mkdocstrings.github.io/python"
```

### Comparing `mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/handler.py` & `mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/handler.py`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/rendering.py` & `mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/rendering.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,27 +105,27 @@
     signature = _format_signature(callable_path, signature, line_length)
     return str(env.filters["highlight"](signature, language="python", inline=False))
 
 
 def do_order_members(
     members: Sequence[Object | Alias],
     order: Order,
-    members_list: list[str] | None,
+    members_list: bool | list[str] | None,
 ) -> Sequence[Object | Alias]:
     """Order members given an ordering method.
 
     Parameters:
         members: The members to order.
         order: The ordering method.
         members_list: An optional member list (manual ordering).
 
     Returns:
         The same members, ordered.
     """
-    if members_list:
+    if isinstance(members_list, list) and members_list:
         sorted_members = []
         members_dict = {member.name: member for member in members}
         for name in members_list:
             if name in members_dict:
                 sorted_members.append(members_dict[name])
         return sorted_members
     return sorted(members, key=order_map[order])
```

### Comparing `mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/attribute.html` & `mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/material/_base/attribute.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/children.html` & `mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/material/_base/children.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/class.html` & `mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/material/_base/class.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring.html` & `mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/attributes.html` & `mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/attributes.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/other_parameters.html` & `mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/other_parameters.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/parameters.html` & `mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/parameters.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/raises.html` & `mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/raises.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/receives.html` & `mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/receives.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/returns.html` & `mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/returns.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/warns.html` & `mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/warns.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/yields.html` & `mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/yields.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/expression.html` & `mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/material/_base/expression.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/function.html` & `mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/material/_base/function.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/languages/en.html` & `mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/material/_base/languages/en.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/languages/ja.html` & `mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/material/_base/languages/ja.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/languages/zh.html` & `mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/material/_base/languages/zh.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/module.html` & `mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/material/_base/module.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/signature.html` & `mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/material/_base/signature.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/style.css` & `mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/material/style.css`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/attributes.html` & `mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/attributes.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/other_parameters.html` & `mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/other_parameters.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/parameters.html` & `mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/parameters.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/raises.html` & `mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/raises.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/receives.html` & `mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/receives.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/returns.html` & `mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/returns.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/warns.html` & `mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/warns.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/yields.html` & `mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/yields.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/readthedocs/style.css` & `mkdocstrings_python-1.2.1/src/mkdocstrings_handlers/python/templates/readthedocs/style.css`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.2.0/tests/conftest.py` & `mkdocstrings_python-1.2.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.2.0/tests/test_handler.py` & `mkdocstrings_python-1.2.1/tests/test_handler.py`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.2.0/tests/test_themes.py` & `mkdocstrings_python-1.2.1/tests/test_themes.py`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.2.0/PKG-INFO` & `mkdocstrings_python-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocstrings-python
-Version: 1.2.0
+Version: 1.2.1
 Summary: A Python handler for mkdocstrings.
 Author-Email: Timothée Mazzucotelli <pawamoy@pm.me>
 License: ISC
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mkdocstrings-python Version: 1.2.0 Summary: A
+Metadata-Version: 2.1 Name: mkdocstrings-python Version: 1.2.1 Summary: A
 Python handler for mkdocstrings. Author-Email: TimothÃ©e Mazzucotelli
 pm.me> License: ISC Classifier: Development Status :: 4 - Beta Classifier:
 Intended Audience :: Developers Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
```

