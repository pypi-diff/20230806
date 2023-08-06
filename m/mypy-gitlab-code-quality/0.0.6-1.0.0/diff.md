# Comparing `tmp/mypy-gitlab-code-quality-0.0.6.tar.gz` & `tmp/mypy-gitlab-code-quality-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-gitlab-code-quality-0.0.6.tar", last modified: Fri Dec 24 07:07:27 2021, max compression
+gzip compressed data, was "mypy-gitlab-code-quality-1.0.0.tar", last modified: Sun Aug  6 12:43:08 2023, max compression
```

## Comparing `mypy-gitlab-code-quality-0.0.6.tar` & `mypy-gitlab-code-quality-1.0.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 soul-catcher  (1000) soul-catcher  (1000)        0 2021-12-24 07:07:27.611897 mypy-gitlab-code-quality-0.0.6/
--rw-r--r--   0 soul-catcher  (1000) soul-catcher  (1000)     1072 2021-12-23 07:25:30.000000 mypy-gitlab-code-quality-0.0.6/LICENSE
--rw-r--r--   0 soul-catcher  (1000) soul-catcher  (1000)      548 2021-12-24 07:07:27.611897 mypy-gitlab-code-quality-0.0.6/PKG-INFO
-drwxr-xr-x   0 soul-catcher  (1000) soul-catcher  (1000)        0 2021-12-24 07:07:27.610897 mypy-gitlab-code-quality-0.0.6/mypy_gitlab_code_quality/
--rw-r--r--   0 soul-catcher  (1000) soul-catcher  (1000)     1050 2021-12-24 06:03:25.000000 mypy-gitlab-code-quality-0.0.6/mypy_gitlab_code_quality/__init__.py
-drwxr-xr-x   0 soul-catcher  (1000) soul-catcher  (1000)        0 2021-12-24 07:07:27.611897 mypy-gitlab-code-quality-0.0.6/mypy_gitlab_code_quality.egg-info/
--rw-r--r--   0 soul-catcher  (1000) soul-catcher  (1000)      548 2021-12-24 07:07:27.000000 mypy-gitlab-code-quality-0.0.6/mypy_gitlab_code_quality.egg-info/PKG-INFO
--rw-r--r--   0 soul-catcher  (1000) soul-catcher  (1000)      312 2021-12-24 07:07:27.000000 mypy-gitlab-code-quality-0.0.6/mypy_gitlab_code_quality.egg-info/SOURCES.txt
--rw-r--r--   0 soul-catcher  (1000) soul-catcher  (1000)        1 2021-12-24 07:07:27.000000 mypy-gitlab-code-quality-0.0.6/mypy_gitlab_code_quality.egg-info/dependency_links.txt
--rw-r--r--   0 soul-catcher  (1000) soul-catcher  (1000)       76 2021-12-24 07:07:27.000000 mypy-gitlab-code-quality-0.0.6/mypy_gitlab_code_quality.egg-info/entry_points.txt
--rw-r--r--   0 soul-catcher  (1000) soul-catcher  (1000)       25 2021-12-24 07:07:27.000000 mypy-gitlab-code-quality-0.0.6/mypy_gitlab_code_quality.egg-info/top_level.txt
--rw-r--r--   0 soul-catcher  (1000) soul-catcher  (1000)       90 2021-12-23 15:15:57.000000 mypy-gitlab-code-quality-0.0.6/pyproject.toml
--rw-r--r--   0 soul-catcher  (1000) soul-catcher  (1000)      618 2021-12-24 07:07:27.611897 mypy-gitlab-code-quality-0.0.6/setup.cfg
+drwxr-xr-x   0 soul-catcher  (1000) soul-catcher  (1000)        0 2023-08-06 12:43:08.675523 mypy-gitlab-code-quality-1.0.0/
+-rw-r--r--   0 soul-catcher  (1000) soul-catcher  (1000)     1072 2023-07-12 11:24:35.000000 mypy-gitlab-code-quality-1.0.0/LICENSE
+-rw-r--r--   0 soul-catcher  (1000) soul-catcher  (1000)     4626 2023-08-06 12:43:08.674523 mypy-gitlab-code-quality-1.0.0/PKG-INFO
+-rw-r--r--   0 soul-catcher  (1000) soul-catcher  (1000)     2437 2023-08-06 12:40:35.000000 mypy-gitlab-code-quality-1.0.0/README.md
+drwxr-xr-x   0 soul-catcher  (1000) soul-catcher  (1000)        0 2023-08-06 12:43:08.674523 mypy-gitlab-code-quality-1.0.0/mypy_gitlab_code_quality/
+-rw-r--r--   0 soul-catcher  (1000) soul-catcher  (1000)     2332 2023-08-06 12:40:35.000000 mypy-gitlab-code-quality-1.0.0/mypy_gitlab_code_quality/__init__.py
+drwxr-xr-x   0 soul-catcher  (1000) soul-catcher  (1000)        0 2023-08-06 12:43:08.674523 mypy-gitlab-code-quality-1.0.0/mypy_gitlab_code_quality.egg-info/
+-rw-r--r--   0 soul-catcher  (1000) soul-catcher  (1000)     4626 2023-08-06 12:43:08.000000 mypy-gitlab-code-quality-1.0.0/mypy_gitlab_code_quality.egg-info/PKG-INFO
+-rw-r--r--   0 soul-catcher  (1000) soul-catcher  (1000)      312 2023-08-06 12:43:08.000000 mypy-gitlab-code-quality-1.0.0/mypy_gitlab_code_quality.egg-info/SOURCES.txt
+-rw-r--r--   0 soul-catcher  (1000) soul-catcher  (1000)        1 2023-08-06 12:43:08.000000 mypy-gitlab-code-quality-1.0.0/mypy_gitlab_code_quality.egg-info/dependency_links.txt
+-rw-r--r--   0 soul-catcher  (1000) soul-catcher  (1000)       75 2023-08-06 12:43:08.000000 mypy-gitlab-code-quality-1.0.0/mypy_gitlab_code_quality.egg-info/entry_points.txt
+-rw-r--r--   0 soul-catcher  (1000) soul-catcher  (1000)       25 2023-08-06 12:43:08.000000 mypy-gitlab-code-quality-1.0.0/mypy_gitlab_code_quality.egg-info/top_level.txt
+-rw-r--r--   0 soul-catcher  (1000) soul-catcher  (1000)     1500 2023-08-06 12:40:35.000000 mypy-gitlab-code-quality-1.0.0/pyproject.toml
+-rw-r--r--   0 soul-catcher  (1000) soul-catcher  (1000)       38 2023-08-06 12:43:08.675523 mypy-gitlab-code-quality-1.0.0/setup.cfg
```

### Comparing `mypy-gitlab-code-quality-0.0.6/LICENSE` & `mypy-gitlab-code-quality-1.0.0/LICENSE`

 * *Files identical despite different names*

