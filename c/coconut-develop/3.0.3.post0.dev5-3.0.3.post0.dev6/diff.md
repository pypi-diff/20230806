# Comparing `tmp/coconut-develop-3.0.3.post0.dev5.tar.gz` & `tmp/coconut-develop-3.0.3.post0.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/coconut-develop-3.0.3.post0.dev5.tar", last modified: Thu Aug  3 10:08:05 2023, max compression
+gzip compressed data, was "dist/coconut-develop-3.0.3.post0.dev6.tar", last modified: Sun Aug  6 20:39:28 2023, max compression
```

## Comparing `coconut-develop-3.0.3.post0.dev5.tar` & `coconut-develop-3.0.3.post0.dev6.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:08:05.000000 coconut-develop-3.0.3.post0.dev5/
--rw-r--r--   0 runner    (1001) docker     (123)   202781 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/DOCS.md
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-08-03 10:08:05.000000 coconut-develop-3.0.3.post0.dev5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:08:05.000000 coconut-develop-3.0.3.post0.dev5/coconut/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:08:05.000000 coconut-develop-3.0.3.post0.dev5/coconut/icoconut/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:08:05.000000 coconut-develop-3.0.3.post0.dev5/coconut/icoconut/coconut/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-08-03 10:08:03.000000 coconut-develop-3.0.3.post0.dev5/coconut/icoconut/coconut/kernel.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:08:05.000000 coconut-develop-3.0.3.post0.dev5/coconut/icoconut/coconut_py3/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/icoconut/coconut_py3/kernel.json
--rw-r--r--   0 runner    (1001) docker     (123)    10776 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/icoconut/root.py
--rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/icoconut/embed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:08:05.000000 coconut-develop-3.0.3.post0.dev5/coconut/icoconut/coconut_py/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/icoconut/coconut_py/kernel.json
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/icoconut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/icoconut/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:08:05.000000 coconut-develop-3.0.3.post0.dev5/coconut/icoconut/coconut_py2/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/icoconut/coconut_py2/kernel.json
--rw-r--r--   0 runner    (1001) docker     (123)    11906 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11623 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/requirements.py
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/__coconut__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/__coconut__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15522 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/root.py
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/highlighter.py
--rw-r--r--   0 runner    (1001) docker     (123)    21746 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/terminal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:08:05.000000 coconut-develop-3.0.3.post0.dev5/coconut/command/
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/command/mypy.py
--rw-r--r--   0 runner    (1001) docker     (123)    47581 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/command/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:08:05.000000 coconut-develop-3.0.3.post0.dev5/coconut/command/resources/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/command/resources/zcoconut.pth
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/command/watch.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/command/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    24763 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/command/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/command/command.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8467 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/command/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:08:05.000000 coconut-develop-3.0.3.post0.dev5/coconut/compiler/
--rw-r--r--   0 runner    (1001) docker     (123)    93531 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/compiler/grammar.py
--rw-r--r--   0 runner    (1001) docker     (123)   206822 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/compiler/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)    57558 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/compiler/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    58872 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/compiler/matching.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:08:05.000000 coconut-develop-3.0.3.post0.dev5/coconut/compiler/templates/
--rw-r--r--   0 runner    (1001) docker     (123)   102541 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/compiler/templates/header.py_template
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/compiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36566 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/compiler/header.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11790 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/convenience.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/api.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:08:05.000000 coconut-develop-3.0.3.post0.dev5/coconut/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    32695 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/tests/main_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/tests/constants_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:08:05.000000 coconut-develop-3.0.3.post0.dev5/coconut/tests/src/
--rw-r--r--   0 runner    (1001) docker     (123)    24083 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/tests/src/extras.coco
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/tests/src/importable.coco
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/tests/src/runnable.coco
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/tests/src/runner.coco
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:08:05.000000 coconut-develop-3.0.3.post0.dev5/coconut/tests/src/cocotest/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:08:05.000000 coconut-develop-3.0.3.post0.dev5/coconut/tests/src/cocotest/agnostic/
--rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/tests/src/cocotest/agnostic/main.coco
--rw-r--r--   0 runner    (1001) docker     (123)    42170 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/tests/src/cocotest/agnostic/suite.coco
--rw-r--r--   0 runner    (1001) docker     (123)    46342 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/tests/src/cocotest/agnostic/util.coco
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/tests/src/cocotest/agnostic/__init__.coco
--rw-r--r--   0 runner    (1001) docker     (123)    15411 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/tests/src/cocotest/agnostic/tutorial.coco
--rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/tests/src/cocotest/agnostic/specific.coco
--rw-r--r--   0 runner    (1001) docker     (123)    64209 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/tests/src/cocotest/agnostic/primary.coco
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:08:05.000000 coconut-develop-3.0.3.post0.dev5/coconut/tests/src/cocotest/target_3/
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/tests/src/cocotest/target_3/py3_test.coco
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:08:05.000000 coconut-develop-3.0.3.post0.dev5/coconut/tests/src/cocotest/target_sys/
--rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/tests/src/cocotest/target_sys/target_sys_test.coco
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:08:05.000000 coconut-develop-3.0.3.post0.dev5/coconut/tests/src/cocotest/non_strict/
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/tests/src/cocotest/non_strict/non_strict_test.coco
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:08:05.000000 coconut-develop-3.0.3.post0.dev5/coconut/tests/src/cocotest/target_38/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/tests/src/cocotest/target_38/py38_test.coco
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:08:05.000000 coconut-develop-3.0.3.post0.dev5/coconut/tests/src/cocotest/target_35/
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/tests/src/cocotest/target_35/py35_test.coco
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:08:05.000000 coconut-develop-3.0.3.post0.dev5/coconut/tests/src/cocotest/target_2/
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/tests/src/cocotest/target_2/py2_test.coco
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:08:05.000000 coconut-develop-3.0.3.post0.dev5/coconut/tests/src/cocotest/target_36/
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/tests/src/cocotest/target_36/py36_test.coco
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/tests/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9534 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/integrations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10580 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    15825 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/_pyparsing.py
--rw-r--r--   0 runner    (1001) docker     (123)    38295 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/convenience.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:08:05.000000 coconut-develop-3.0.3.post0.dev5/coconut_develop.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-08-03 10:08:05.000000 coconut-develop-3.0.3.post0.dev5/coconut_develop.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:08:05.000000 coconut-develop-3.0.3.post0.dev5/__coconut__/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/__coconut__/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    60331 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/__coconut__/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/__coconut__/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7601 2023-08-03 10:08:05.000000 coconut-develop-3.0.3.post0.dev5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:08:05.000000 coconut-develop-3.0.3.post0.dev5/xontrib/
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/xontrib/coconut.py
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11350 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/FAQ.md
--rw-r--r--   0 runner    (1001) docker     (123)    65131 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/HELP.md
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)    13807 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:08:05.000000 coconut-develop-3.0.3.post0.dev5/_coconut/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/_coconut/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/_coconut/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/_coconut/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:39:28.000000 coconut-develop-3.0.3.post0.dev6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-08-06 20:39:28.000000 coconut-develop-3.0.3.post0.dev6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:39:28.000000 coconut-develop-3.0.3.post0.dev6/xontrib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/xontrib/coconut.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:39:28.000000 coconut-develop-3.0.3.post0.dev6/coconut/
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/coconut/highlighter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/coconut/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9534 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/coconut/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10580 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/coconut/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11790 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/coconut/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11623 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/coconut/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/coconut/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/coconut/__coconut__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:39:28.000000 coconut-develop-3.0.3.post0.dev6/coconut/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:39:28.000000 coconut-develop-3.0.3.post0.dev6/coconut/tests/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/coconut/tests/src/runner.coco
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/coconut/tests/src/importable.coco
+-rw-r--r--   0 runner    (1001) docker     (123)    24337 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/coconut/tests/src/extras.coco
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/coconut/tests/src/runnable.coco
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:39:28.000000 coconut-develop-3.0.3.post0.dev6/coconut/tests/src/cocotest/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:39:28.000000 coconut-develop-3.0.3.post0.dev6/coconut/tests/src/cocotest/target_3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/coconut/tests/src/cocotest/target_3/py3_test.coco
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:39:28.000000 coconut-develop-3.0.3.post0.dev6/coconut/tests/src/cocotest/target_sys/
+-rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/coconut/tests/src/cocotest/target_sys/target_sys_test.coco
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:39:28.000000 coconut-develop-3.0.3.post0.dev6/coconut/tests/src/cocotest/target_38/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/coconut/tests/src/cocotest/target_38/py38_test.coco
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:39:28.000000 coconut-develop-3.0.3.post0.dev6/coconut/tests/src/cocotest/agnostic/
+-rw-r--r--   0 runner    (1001) docker     (123)    15411 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/coconut/tests/src/cocotest/agnostic/tutorial.coco
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/coconut/tests/src/cocotest/agnostic/__init__.coco
+-rw-r--r--   0 runner    (1001) docker     (123)    46342 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/coconut/tests/src/cocotest/agnostic/util.coco
+-rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/coconut/tests/src/cocotest/agnostic/specific.coco
+-rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/coconut/tests/src/cocotest/agnostic/main.coco
+-rw-r--r--   0 runner    (1001) docker     (123)    42170 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/coconut/tests/src/cocotest/agnostic/suite.coco
+-rw-r--r--   0 runner    (1001) docker     (123)    64209 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/coconut/tests/src/cocotest/agnostic/primary.coco
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:39:28.000000 coconut-develop-3.0.3.post0.dev6/coconut/tests/src/cocotest/target_36/
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/coconut/tests/src/cocotest/target_36/py36_test.coco
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:39:28.000000 coconut-develop-3.0.3.post0.dev6/coconut/tests/src/cocotest/target_35/
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/coconut/tests/src/cocotest/target_35/py35_test.coco
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:39:28.000000 coconut-develop-3.0.3.post0.dev6/coconut/tests/src/cocotest/non_strict/
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/coconut/tests/src/cocotest/non_strict/non_strict_test.coco
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:39:28.000000 coconut-develop-3.0.3.post0.dev6/coconut/tests/src/cocotest/target_2/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/coconut/tests/src/cocotest/target_2/py2_test.coco
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/coconut/tests/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32688 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/coconut/tests/main_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/coconut/tests/constants_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/coconut/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15522 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/coconut/root.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/coconut/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/coconut/api.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/coconut/convenience.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:39:28.000000 coconut-develop-3.0.3.post0.dev6/coconut/compiler/
+-rw-r--r--   0 runner    (1001) docker     (123)    93531 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/coconut/compiler/grammar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36566 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/coconut/compiler/header.py
+-rw-r--r--   0 runner    (1001) docker     (123)   206866 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/coconut/compiler/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57558 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/coconut/compiler/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:39:28.000000 coconut-develop-3.0.3.post0.dev6/coconut/compiler/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)   102541 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/coconut/compiler/templates/header.py_template
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/coconut/compiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58872 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/coconut/compiler/matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15825 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/coconut/_pyparsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/coconut/convenience.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38295 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/coconut/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:39:28.000000 coconut-develop-3.0.3.post0.dev6/coconut/icoconut/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:39:28.000000 coconut-develop-3.0.3.post0.dev6/coconut/icoconut/coconut_py3/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/coconut/icoconut/coconut_py3/kernel.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:39:28.000000 coconut-develop-3.0.3.post0.dev6/coconut/icoconut/coconut_py2/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/coconut/icoconut/coconut_py2/kernel.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:39:28.000000 coconut-develop-3.0.3.post0.dev6/coconut/icoconut/coconut/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-08-06 20:39:27.000000 coconut-develop-3.0.3.post0.dev6/coconut/icoconut/coconut/kernel.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10776 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/coconut/icoconut/root.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/coconut/icoconut/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/coconut/icoconut/embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/coconut/icoconut/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:39:28.000000 coconut-develop-3.0.3.post0.dev6/coconut/icoconut/coconut_py/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/coconut/icoconut/coconut_py/kernel.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/coconut/__coconut__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:39:28.000000 coconut-develop-3.0.3.post0.dev6/coconut/command/
+-rw-r--r--   0 runner    (1001) docker     (123)    24763 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/coconut/command/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/coconut/command/watch.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/coconut/command/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    47607 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/coconut/command/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/coconut/command/mypy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:39:28.000000 coconut-develop-3.0.3.post0.dev6/coconut/command/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/coconut/command/resources/zcoconut.pth
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/coconut/command/command.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/coconut/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8467 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/coconut/command/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11906 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/coconut/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/coconut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/coconut/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    21746 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/coconut/terminal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    65131 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/HELP.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13807 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:39:28.000000 coconut-develop-3.0.3.post0.dev6/__coconut__/
+-rw-r--r--   0 runner    (1001) docker     (123)    60331 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/__coconut__/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/__coconut__/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/__coconut__/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11350 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/FAQ.md
+-rw-r--r--   0 runner    (1001) docker     (123)   202781 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/DOCS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7601 2023-08-06 20:39:28.000000 coconut-develop-3.0.3.post0.dev6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:39:28.000000 coconut-develop-3.0.3.post0.dev6/_coconut/
+-rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/_coconut/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/_coconut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 19:36:22.000000 coconut-develop-3.0.3.post0.dev6/_coconut/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:39:28.000000 coconut-develop-3.0.3.post0.dev6/coconut_develop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-08-06 20:39:28.000000 coconut-develop-3.0.3.post0.dev6/coconut_develop.egg-info/SOURCES.txt
```

### Comparing `coconut-develop-3.0.3.post0.dev5/DOCS.md` & `coconut-develop-3.0.3.post0.dev6/DOCS.md`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev5/coconut/icoconut/root.py` & `coconut-develop-3.0.3.post0.dev6/coconut/icoconut/root.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev5/coconut/icoconut/embed.py` & `coconut-develop-3.0.3.post0.dev6/coconut/icoconut/embed.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev5/coconut/icoconut/__init__.py` & `coconut-develop-3.0.3.post0.dev6/coconut/icoconut/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev5/coconut/icoconut/__main__.py` & `coconut-develop-3.0.3.post0.dev6/coconut/icoconut/__main__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev5/coconut/api.py` & `coconut-develop-3.0.3.post0.dev6/coconut/api.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev5/coconut/requirements.py` & `coconut-develop-3.0.3.post0.dev6/coconut/requirements.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev5/coconut/__coconut__.pyi` & `coconut-develop-3.0.3.post0.dev6/coconut/__coconut__.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev5/coconut/__coconut__.py` & `coconut-develop-3.0.3.post0.dev6/coconut/__coconut__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev5/coconut/root.py` & `coconut-develop-3.0.3.post0.dev6/coconut/root.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # -----------------------------------------------------------------------------------------------------------------------
 # VERSION:
 # -----------------------------------------------------------------------------------------------------------------------
 
 VERSION = "3.0.3"
 VERSION_NAME = None
 # False for release, int >= 1 for develop
-DEVELOP = 5
+DEVELOP = 6
 ALPHA = False  # for pre releases rather than post releases
 
 assert DEVELOP is False or DEVELOP >= 1, "DEVELOP must be False or an int >= 1"
 assert DEVELOP or not ALPHA, "alpha releases are only for develop"
 
 # -----------------------------------------------------------------------------------------------------------------------
 # UTILITIES:
```

### Comparing `coconut-develop-3.0.3.post0.dev5/coconut/highlighter.py` & `coconut-develop-3.0.3.post0.dev6/coconut/highlighter.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev5/coconut/terminal.py` & `coconut-develop-3.0.3.post0.dev6/coconut/terminal.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev5/coconut/command/mypy.py` & `coconut-develop-3.0.3.post0.dev6/coconut/command/mypy.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev5/coconut/command/command.py` & `coconut-develop-3.0.3.post0.dev6/coconut/command/command.py`

 * *Files 0% similar despite different names*

```diff
@@ -604,15 +604,15 @@
                         self.execute_file(destpath, argv_source_path=codepath)
 
             parse_kwargs = dict(
                 filename=os.path.basename(codepath),
             )
             if self.incremental:
                 if disable_incremental_for_len is not None and len(code) > disable_incremental_for_len:
-                    logger.warn("--incremental mode is not currently supported for files as large as {codepath!r}")
+                    logger.warn("--incremental mode is not currently supported for files as large as {codepath!r}".format(codepath=codepath))
                 else:
                     code_dir, code_fname = os.path.split(codepath)
 
                     cache_dir = os.path.join(code_dir, coconut_cache_dir)
                     ensure_dir(cache_dir)
 
                     pickle_fname = code_fname + ".pickle"
```

### Comparing `coconut-develop-3.0.3.post0.dev5/coconut/command/watch.py` & `coconut-develop-3.0.3.post0.dev6/coconut/command/watch.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev5/coconut/command/util.py` & `coconut-develop-3.0.3.post0.dev6/coconut/command/util.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev5/coconut/command/command.pyi` & `coconut-develop-3.0.3.post0.dev6/coconut/command/command.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev5/coconut/command/__init__.py` & `coconut-develop-3.0.3.post0.dev6/coconut/command/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev5/coconut/command/cli.py` & `coconut-develop-3.0.3.post0.dev6/coconut/command/cli.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev5/coconut/compiler/grammar.py` & `coconut-develop-3.0.3.post0.dev6/coconut/compiler/grammar.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev5/coconut/compiler/compiler.py` & `coconut-develop-3.0.3.post0.dev6/coconut/compiler/compiler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1237,14 +1237,15 @@
                     ln = self.adjust(lineno(loc, original))
                     comment = self.reformat(" ".join(self.comments[ln]), ignore_errors=True)
                     if not self.noqa_regex.search(comment):
                         self.strict_err_or_warn(
                             "found unused import " + repr(self.reformat(name, ignore_errors=True)) + " (add '# NOQA' to suppress)",
                             original,
                             loc,
+                            endpoint=False,
                         )
 
     def parse(
         self,
         inputstring,
         parser,
         preargs,
```

### Comparing `coconut-develop-3.0.3.post0.dev5/coconut/compiler/util.py` & `coconut-develop-3.0.3.post0.dev6/coconut/compiler/util.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev5/coconut/compiler/matching.py` & `coconut-develop-3.0.3.post0.dev6/coconut/compiler/matching.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev5/coconut/compiler/templates/header.py_template` & `coconut-develop-3.0.3.post0.dev6/coconut/compiler/templates/header.py_template`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev5/coconut/compiler/__init__.py` & `coconut-develop-3.0.3.post0.dev6/coconut/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev5/coconut/compiler/header.py` & `coconut-develop-3.0.3.post0.dev6/coconut/compiler/header.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev5/coconut/__init__.pyi` & `coconut-develop-3.0.3.post0.dev6/coconut/__init__.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev5/coconut/util.py` & `coconut-develop-3.0.3.post0.dev6/coconut/util.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev5/coconut/main.py` & `coconut-develop-3.0.3.post0.dev6/coconut/main.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev5/coconut/convenience.pyi` & `coconut-develop-3.0.3.post0.dev6/coconut/convenience.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev5/coconut/api.pyi` & `coconut-develop-3.0.3.post0.dev6/coconut/api.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev5/coconut/tests/main_test.py` & `coconut-develop-3.0.3.post0.dev6/coconut/tests/main_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -808,15 +808,15 @@
             p.sendline("'1; 2' |> print")
             p.expect("1; 2")
             p.sendline('$ENV_VAR = "ABC"')
             p.expect("$")
             p.sendline('echo f"{$ENV_VAR}"; echo f"{$ENV_VAR}"')
             p.expect("ABC")
             p.expect("ABC")
-            p.sendline('len("""1\n3\n5""") |> print')
+            p.sendline('len("""1\n3\n5""")\n')
             p.expect("5")
             if not PYPY or PY39:
                 if PY36:
                     p.sendline("echo 123;; 123")
                     p.expect("123;; 123")
                     p.sendline("echo abc; echo abc")
                     p.expect("abc")
```

### Comparing `coconut-develop-3.0.3.post0.dev5/coconut/tests/constants_test.py` & `coconut-develop-3.0.3.post0.dev6/coconut/tests/constants_test.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev5/coconut/tests/src/extras.coco` & `coconut-develop-3.0.3.post0.dev6/coconut/tests/src/extras.coco`

 * *Files 0% similar despite different names*

```diff
@@ -344,14 +344,24 @@
     assert_raises(-> parse("""case x:
     match x:
         pass"""), CoconutStyleError, err_has="case x:")
     assert_raises(-> parse("obj."), CoconutStyleError, err_has="getattr")
     assert_raises(-> parse("def x -> pass, 1"), CoconutStyleError, err_has="statement lambda")
     assert_raises(-> parse("abc = f'abc'"), CoconutStyleError, err_has="\n        ^")
     assert_raises(-> parse('f"{f"{f"infinite"}"}"'), CoconutStyleError, err_has=" ^~~~~~~~~~~|")
+    try:
+        parse("""
+import abc
+1
+2
+3
+        """.strip())
+    except CoconutStyleError as err:
+        assert str(err) == """found unused import 'abc' (add '# NOQA' to suppress) (remove --strict to downgrade to a warning) (line 1)
+  import abc"""
 
     setup(line_numbers=False, strict=True, target="sys")
     assert_raises(-> parse("await f x"), CoconutParseError, err_has='invalid use of the keyword "await"')
 
     setup(line_numbers=False, target="2.7")
     assert parse("from io import BytesIO", mode="lenient") == "from io import BytesIO"
     assert_raises(-> parse("def f(*, x=None) = x"), CoconutTargetError, err_has="\n        ^")
```

### Comparing `coconut-develop-3.0.3.post0.dev5/coconut/tests/src/cocotest/agnostic/main.coco` & `coconut-develop-3.0.3.post0.dev6/coconut/tests/src/cocotest/agnostic/main.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev5/coconut/tests/src/cocotest/agnostic/suite.coco` & `coconut-develop-3.0.3.post0.dev6/coconut/tests/src/cocotest/agnostic/suite.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev5/coconut/tests/src/cocotest/agnostic/util.coco` & `coconut-develop-3.0.3.post0.dev6/coconut/tests/src/cocotest/agnostic/util.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev5/coconut/tests/src/cocotest/agnostic/tutorial.coco` & `coconut-develop-3.0.3.post0.dev6/coconut/tests/src/cocotest/agnostic/tutorial.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev5/coconut/tests/src/cocotest/agnostic/specific.coco` & `coconut-develop-3.0.3.post0.dev6/coconut/tests/src/cocotest/agnostic/specific.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev5/coconut/tests/src/cocotest/agnostic/primary.coco` & `coconut-develop-3.0.3.post0.dev6/coconut/tests/src/cocotest/agnostic/primary.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev5/coconut/tests/src/cocotest/target_3/py3_test.coco` & `coconut-develop-3.0.3.post0.dev6/coconut/tests/src/cocotest/target_3/py3_test.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev5/coconut/tests/src/cocotest/target_sys/target_sys_test.coco` & `coconut-develop-3.0.3.post0.dev6/coconut/tests/src/cocotest/target_sys/target_sys_test.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev5/coconut/tests/src/cocotest/non_strict/non_strict_test.coco` & `coconut-develop-3.0.3.post0.dev6/coconut/tests/src/cocotest/non_strict/non_strict_test.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev5/coconut/tests/src/cocotest/target_35/py35_test.coco` & `coconut-develop-3.0.3.post0.dev6/coconut/tests/src/cocotest/target_35/py35_test.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev5/coconut/tests/src/cocotest/target_36/py36_test.coco` & `coconut-develop-3.0.3.post0.dev6/coconut/tests/src/cocotest/target_36/py36_test.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev5/coconut/tests/__init__.py` & `coconut-develop-3.0.3.post0.dev6/coconut/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev5/coconut/tests/__main__.py` & `coconut-develop-3.0.3.post0.dev6/coconut/tests/__main__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev5/coconut/integrations.py` & `coconut-develop-3.0.3.post0.dev6/coconut/integrations.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev5/coconut/__init__.py` & `coconut-develop-3.0.3.post0.dev6/coconut/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev5/coconut/__main__.py` & `coconut-develop-3.0.3.post0.dev6/coconut/__main__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev5/coconut/exceptions.py` & `coconut-develop-3.0.3.post0.dev6/coconut/exceptions.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev5/coconut/_pyparsing.py` & `coconut-develop-3.0.3.post0.dev6/coconut/_pyparsing.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev5/coconut/constants.py` & `coconut-develop-3.0.3.post0.dev6/coconut/constants.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev5/coconut/convenience.py` & `coconut-develop-3.0.3.post0.dev6/coconut/convenience.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev5/coconut_develop.egg-info/SOURCES.txt` & `coconut-develop-3.0.3.post0.dev6/coconut_develop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev5/README.rst` & `coconut-develop-3.0.3.post0.dev6/README.rst`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev5/__coconut__/__init__.pyi` & `coconut-develop-3.0.3.post0.dev6/__coconut__/__init__.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev5/__coconut__/__init__.py` & `coconut-develop-3.0.3.post0.dev6/__coconut__/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev5/PKG-INFO` & `coconut-develop-3.0.3.post0.dev6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coconut-develop
-Version: 3.0.3.post0.dev5
+Version: 3.0.3.post0.dev6
 Summary: Simple, elegant, Pythonic functional programming.
 Home-page: http://coconut-lang.org
 Author: Evan Hubinger
 Author-email: evanjhub@gmail.com
 License: Apache 2.0
 Description: |logo| Coconut
         ==============
```

### Comparing `coconut-develop-3.0.3.post0.dev5/xontrib/coconut.py` & `coconut-develop-3.0.3.post0.dev6/xontrib/coconut.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev5/LICENSE.txt` & `coconut-develop-3.0.3.post0.dev6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev5/FAQ.md` & `coconut-develop-3.0.3.post0.dev6/FAQ.md`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev5/HELP.md` & `coconut-develop-3.0.3.post0.dev6/HELP.md`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev5/setup.py` & `coconut-develop-3.0.3.post0.dev6/setup.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev5/CONTRIBUTING.md` & `coconut-develop-3.0.3.post0.dev6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev5/conf.py` & `coconut-develop-3.0.3.post0.dev6/conf.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev5/_coconut/__init__.pyi` & `coconut-develop-3.0.3.post0.dev6/_coconut/__init__.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev5/_coconut/__init__.py` & `coconut-develop-3.0.3.post0.dev6/_coconut/__init__.py`

 * *Files identical despite different names*

