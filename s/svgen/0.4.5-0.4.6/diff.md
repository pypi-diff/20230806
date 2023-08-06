# Comparing `tmp/svgen-0.4.5.tar.gz` & `tmp/svgen-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "svgen-0.4.5.tar", last modified: Sun Mar 19 15:10:40 2023, max compression
+gzip compressed data, was "svgen-0.4.6.tar", last modified: Sun Aug  6 07:16:44 2023, max compression
```

## Comparing `svgen-0.4.5.tar` & `svgen-0.4.6.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 15:10:40.112856 svgen-0.4.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-03-19 15:09:38.000000 svgen-0.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-03-19 15:10:40.108856 svgen-0.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-03-19 15:09:38.000000 svgen-0.4.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-03-19 15:09:38.000000 svgen-0.4.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-19 15:10:40.112856 svgen-0.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-03-19 15:09:38.000000 svgen-0.4.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 15:10:40.100856 svgen-0.4.5/svgen/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-03-19 15:09:38.000000 svgen-0.4.5/svgen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-03-19 15:09:38.000000 svgen-0.4.5/svgen/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-03-19 15:09:38.000000 svgen-0.4.5/svgen/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 15:10:40.100856 svgen-0.4.5/svgen/attribute/
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-03-19 15:09:38.000000 svgen-0.4.5/svgen/attribute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-03-19 15:09:38.000000 svgen-0.4.5/svgen/attribute/style.py
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-03-19 15:09:38.000000 svgen-0.4.5/svgen/attribute/viewbox.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 15:10:40.104856 svgen-0.4.5/svgen/cartesian/
--rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-03-19 15:09:38.000000 svgen-0.4.5/svgen/cartesian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-03-19 15:09:38.000000 svgen-0.4.5/svgen/cartesian/circle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-03-19 15:09:38.000000 svgen-0.4.5/svgen/cartesian/mutate.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-03-19 15:09:38.000000 svgen-0.4.5/svgen/cartesian/plane.py
--rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-03-19 15:09:38.000000 svgen-0.4.5/svgen/cartesian/point.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 15:10:40.104856 svgen-0.4.5/svgen/cartesian/rectangle/
--rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-03-19 15:09:38.000000 svgen-0.4.5/svgen/cartesian/rectangle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-03-19 15:09:38.000000 svgen-0.4.5/svgen/cartesian/rectangle/corner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-03-19 15:09:38.000000 svgen-0.4.5/svgen/cartesian/rectangle/grid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 15:10:40.104856 svgen-0.4.5/svgen/color/
--rw-r--r--   0 runner    (1001) docker     (123)     6525 2023-03-19 15:09:38.000000 svgen-0.4.5/svgen/color/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-03-19 15:09:38.000000 svgen-0.4.5/svgen/color/alpha.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-03-19 15:09:38.000000 svgen-0.4.5/svgen/color/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-03-19 15:09:38.000000 svgen-0.4.5/svgen/color/hsl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-03-19 15:09:38.000000 svgen-0.4.5/svgen/color/numbers.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-03-19 15:09:38.000000 svgen-0.4.5/svgen/color/resolve.py
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-03-19 15:09:38.000000 svgen-0.4.5/svgen/color/rgb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 15:10:40.104856 svgen-0.4.5/svgen/color/theme/
--rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-03-19 15:09:38.000000 svgen-0.4.5/svgen/color/theme/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-03-19 15:09:38.000000 svgen-0.4.5/svgen/color/theme/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-03-19 15:09:38.000000 svgen-0.4.5/svgen/color/theme/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 15:10:40.092856 svgen-0.4.5/svgen/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 15:10:40.108856 svgen-0.4.5/svgen/data/themes/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-03-19 15:09:38.000000 svgen-0.4.5/svgen/data/themes/blue_gray.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-03-19 15:09:38.000000 svgen-0.4.5/svgen/data/themes/gray.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-19 15:09:38.000000 svgen-0.4.5/svgen/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-03-19 15:09:38.000000 svgen-0.4.5/svgen/display.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 15:10:40.108856 svgen-0.4.5/svgen/element/
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-03-19 15:09:38.000000 svgen-0.4.5/svgen/element/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-03-19 15:09:38.000000 svgen-0.4.5/svgen/element/circle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-03-19 15:09:38.000000 svgen-0.4.5/svgen/element/line.py
--rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-03-19 15:09:38.000000 svgen-0.4.5/svgen/element/rect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-03-19 15:09:38.000000 svgen-0.4.5/svgen/element/svg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-03-19 15:09:38.000000 svgen-0.4.5/svgen/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 15:10:40.108856 svgen-0.4.5/svgen/generation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-19 15:09:38.000000 svgen-0.4.5/svgen/generation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-03-19 15:09:38.000000 svgen-0.4.5/svgen/generation/images.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-03-19 15:09:38.000000 svgen-0.4.5/svgen/inkscape.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-19 15:09:38.000000 svgen-0.4.5/svgen/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-19 15:09:38.000000 svgen-0.4.5/svgen/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-03-19 15:09:38.000000 svgen-0.4.5/svgen/script.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 15:10:40.108856 svgen-0.4.5/svgen/shapes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-19 15:09:38.000000 svgen-0.4.5/svgen/shapes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-03-19 15:09:38.000000 svgen-0.4.5/svgen/shapes/chip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-03-19 15:09:38.000000 svgen-0.4.5/svgen/shapes/pins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 15:10:40.100856 svgen-0.4.5/svgen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-03-19 15:10:40.000000 svgen-0.4.5/svgen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-03-19 15:10:40.000000 svgen-0.4.5/svgen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-19 15:10:40.000000 svgen-0.4.5/svgen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-19 15:10:40.000000 svgen-0.4.5/svgen.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-03-19 15:10:40.000000 svgen-0.4.5/svgen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-19 15:10:40.000000 svgen-0.4.5/svgen.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 15:10:40.108856 svgen-0.4.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-03-19 15:09:38.000000 svgen-0.4.5/tests/test_display.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-03-19 15:09:38.000000 svgen-0.4.5/tests/test_entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:16:44.175109 svgen-0.4.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-06 07:15:14.000000 svgen-0.4.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-08-06 07:16:44.175109 svgen-0.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-08-06 07:15:14.000000 svgen-0.4.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-08-06 07:15:14.000000 svgen-0.4.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 07:16:44.175109 svgen-0.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-08-06 07:15:14.000000 svgen-0.4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:16:44.167110 svgen-0.4.6/svgen/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-08-06 07:15:14.000000 svgen-0.4.6/svgen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-08-06 07:15:14.000000 svgen-0.4.6/svgen/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-08-06 07:15:14.000000 svgen-0.4.6/svgen/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:16:44.171110 svgen-0.4.6/svgen/attribute/
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-08-06 07:15:14.000000 svgen-0.4.6/svgen/attribute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-08-06 07:15:14.000000 svgen-0.4.6/svgen/attribute/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-08-06 07:15:14.000000 svgen-0.4.6/svgen/attribute/viewbox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:16:44.171110 svgen-0.4.6/svgen/cartesian/
+-rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-08-06 07:15:14.000000 svgen-0.4.6/svgen/cartesian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-08-06 07:15:14.000000 svgen-0.4.6/svgen/cartesian/circle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-08-06 07:15:14.000000 svgen-0.4.6/svgen/cartesian/mutate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-08-06 07:15:14.000000 svgen-0.4.6/svgen/cartesian/plane.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-08-06 07:15:14.000000 svgen-0.4.6/svgen/cartesian/point.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:16:44.171110 svgen-0.4.6/svgen/cartesian/rectangle/
+-rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-08-06 07:15:14.000000 svgen-0.4.6/svgen/cartesian/rectangle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-08-06 07:15:14.000000 svgen-0.4.6/svgen/cartesian/rectangle/corner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-08-06 07:15:14.000000 svgen-0.4.6/svgen/cartesian/rectangle/grid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:16:44.171110 svgen-0.4.6/svgen/color/
+-rw-r--r--   0 runner    (1001) docker     (123)     6525 2023-08-06 07:15:14.000000 svgen-0.4.6/svgen/color/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-08-06 07:15:14.000000 svgen-0.4.6/svgen/color/alpha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-08-06 07:15:14.000000 svgen-0.4.6/svgen/color/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-08-06 07:15:14.000000 svgen-0.4.6/svgen/color/hsl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-08-06 07:15:14.000000 svgen-0.4.6/svgen/color/numbers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-08-06 07:15:14.000000 svgen-0.4.6/svgen/color/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-08-06 07:15:14.000000 svgen-0.4.6/svgen/color/rgb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:16:44.171110 svgen-0.4.6/svgen/color/theme/
+-rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-08-06 07:15:14.000000 svgen-0.4.6/svgen/color/theme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-08-06 07:15:14.000000 svgen-0.4.6/svgen/color/theme/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-08-06 07:15:14.000000 svgen-0.4.6/svgen/color/theme/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:16:44.167110 svgen-0.4.6/svgen/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:16:44.171110 svgen-0.4.6/svgen/data/themes/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-08-06 07:15:14.000000 svgen-0.4.6/svgen/data/themes/blue_gray.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-08-06 07:15:14.000000 svgen-0.4.6/svgen/data/themes/gray.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-06 07:15:14.000000 svgen-0.4.6/svgen/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-08-06 07:15:14.000000 svgen-0.4.6/svgen/display.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:16:44.171110 svgen-0.4.6/svgen/element/
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-08-06 07:15:14.000000 svgen-0.4.6/svgen/element/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-08-06 07:15:14.000000 svgen-0.4.6/svgen/element/circle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-08-06 07:15:14.000000 svgen-0.4.6/svgen/element/line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-08-06 07:15:14.000000 svgen-0.4.6/svgen/element/rect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-08-06 07:15:14.000000 svgen-0.4.6/svgen/element/svg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-08-06 07:15:14.000000 svgen-0.4.6/svgen/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:16:44.171110 svgen-0.4.6/svgen/generation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 07:15:14.000000 svgen-0.4.6/svgen/generation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-08-06 07:15:14.000000 svgen-0.4.6/svgen/generation/images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-08-06 07:15:14.000000 svgen-0.4.6/svgen/inkscape.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 07:15:14.000000 svgen-0.4.6/svgen/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-06 07:15:14.000000 svgen-0.4.6/svgen/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-08-06 07:15:14.000000 svgen-0.4.6/svgen/script.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:16:44.175109 svgen-0.4.6/svgen/shapes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 07:15:14.000000 svgen-0.4.6/svgen/shapes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-08-06 07:15:14.000000 svgen-0.4.6/svgen/shapes/chip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-08-06 07:15:14.000000 svgen-0.4.6/svgen/shapes/pins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:16:44.171110 svgen-0.4.6/svgen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-08-06 07:16:44.000000 svgen-0.4.6/svgen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-08-06 07:16:44.000000 svgen-0.4.6/svgen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 07:16:44.000000 svgen-0.4.6/svgen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-06 07:16:44.000000 svgen-0.4.6/svgen.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-06 07:16:44.000000 svgen-0.4.6/svgen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-06 07:16:44.000000 svgen-0.4.6/svgen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:16:44.175109 svgen-0.4.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-08-06 07:15:14.000000 svgen-0.4.6/tests/test_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-08-06 07:15:14.000000 svgen-0.4.6/tests/test_entry.py
```

### Comparing `svgen-0.4.5/LICENSE` & `svgen-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `svgen-0.4.5/PKG-INFO` & `svgen-0.4.6/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,59 +1,42 @@
-Metadata-Version: 2.1
-Name: svgen
-Version: 0.4.5
-Summary: A tool for working with scalable vector graphics.
-Home-page: https://github.com/vkottler/svgen
-Author: Vaughn Kottler
-Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
-Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: Unix
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE
-
 <!--
     =====================================
     generator=datazen
-    version=3.1.0
-    hash=bde00c56e321c249355c2d1fc449e235
+    version=3.1.2
+    hash=848c4ceae1ab8dff160beff92e43bef4
     =====================================
 -->
 
-# svgen ([0.4.5](https://pypi.org/project/svgen/))
+# svgen ([0.4.6](https://pypi.org/project/svgen/))
 
 [![python](https://img.shields.io/pypi/pyversions/svgen.svg)](https://pypi.org/project/svgen/)
 ![Build Status](https://github.com/vkottler/svgen/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/svgen/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/svgen)
 ![PyPI - Status](https://img.shields.io/pypi/status/svgen)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/svgen)
 
 *A tool for working with scalable vector graphics.*
 
-See also: [generated documentation](https://vkottler.github.io/python/pydoc/svgen.html)
-(created with [`pydoc`](https://docs.python.org/3/library/pydoc.html)).
+## Documentation
+
+### Generated
+
+* By [sphinx-apidoc](https://vkottler.github.io/python/sphinx/svgen)
+(What's [`sphinx-apidoc`](https://www.sphinx-doc.org/en/master/man/sphinx-apidoc.html)?)
+* By [pydoc](https://vkottler.github.io/python/pydoc/svgen.html)
+(What's [`pydoc`](https://docs.python.org/3/library/pydoc.html)?)
 
 ## Python Version Support
 
 This package is tested with the following Python minor versions:
 
-* [`python3.7`](https://docs.python.org/3.7/)
 * [`python3.8`](https://docs.python.org/3.8/)
 * [`python3.9`](https://docs.python.org/3.9/)
 * [`python3.10`](https://docs.python.org/3.10/)
+* [`python3.11`](https://docs.python.org/3.11/)
 
 ## Platform Support
 
 This package is tested on the following platforms:
 
 * `ubuntu-latest`
 * `macos-latest`
@@ -62,27 +45,27 @@
 # Introduction
 
 This utility provides a means to work on graphics with a programmatic workflow.
 
 # Command-line Options
 
 ```
-$ ./venv3.8/bin/svgen -h
+$ ./venv3.11/bin/svgen -h
 
 usage: svgen [-h] [--version] [-v] [-C DIR] [-c CONFIG] [--height HEIGHT]
              [--width WIDTH] [--images] [-o OUTPUT]
-             [scripts [scripts ...]]
+             [scripts ...]
 
 A tool for working with scalable vector graphics.
 
 positional arguments:
   scripts               scripts to run for composing the SVG document (in
                         order)
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
   --version             show program's version number and exit
   -v, --verbose         set to increase logging verbosity
   -C DIR, --dir DIR     execute from a specific directory
   -c CONFIG, --config CONFIG
                         top-level configuration to load (default:
                         'svgen.json')
```

### Comparing `svgen-0.4.5/pyproject.toml` & `svgen-0.4.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,47 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "svgen"
-version = "0.4.5"
+version = "0.4.6"
 description = "A tool for working with scalable vector graphics."
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 classifiers = [
-  "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
   "Operating System :: Microsoft :: Windows",
   "Operating System :: MacOS",
   "Operating System :: POSIX :: Linux",
   "Operating System :: Unix",
   "Development Status :: 5 - Production/Stable",
   "License :: OSI Approved :: MIT License"
 ]
 dynamic = ["dependencies"]
 
 [project.optional-dependencies]
 test = [
   "pylint",
   "flake8",
-  "pytest",
-  "pytest-cov",
-  "mypy",
   "black",
+  "ruff",
+  "mypy",
   "isort",
-  "setuptools-wrapper"
+  "yamllint",
+  "yambs",
+  "vmklib",
+  "setuptools-wrapper",
+  "pytest"
 ]
 
 [project.scripts]
 svgen = "svgen.entry:main"
```

### Comparing `svgen-0.4.5/setup.py` & `svgen-0.4.6/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # =====================================
 # generator=datazen
-# version=3.1.0
-# hash=a8a0d03626a8371219b90fe5e4a7a49a
+# version=3.1.2
+# hash=224dbecf0fd19b1222e824b1fbe652a8
 # =====================================
 
 """
 svgen - Package definition for distribution.
 """
 
 # third-party
@@ -24,17 +24,17 @@
 }
 pkg_info = {
     "name": PKG_NAME,
     "slug": PKG_NAME.replace("-", "_"),
     "version": VERSION,
     "description": DESCRIPTION,
     "versions": [
-        "3.7",
         "3.8",
         "3.9",
         "3.10",
+        "3.11",
     ],
 }
 setup(
     pkg_info,
     author_info,
 )
```

### Comparing `svgen-0.4.5/svgen/app.py` & `svgen-0.4.6/svgen/app.py`

 * *Files identical despite different names*

### Comparing `svgen-0.4.5/svgen/attribute/__init__.py` & `svgen-0.4.6/svgen/attribute/__init__.py`

 * *Files identical despite different names*

### Comparing `svgen-0.4.5/svgen/attribute/style.py` & `svgen-0.4.6/svgen/attribute/style.py`

 * *Files identical despite different names*

### Comparing `svgen-0.4.5/svgen/attribute/viewbox.py` & `svgen-0.4.6/svgen/attribute/viewbox.py`

 * *Files identical despite different names*

### Comparing `svgen-0.4.5/svgen/cartesian/__init__.py` & `svgen-0.4.6/svgen/cartesian/__init__.py`

 * *Files identical despite different names*

### Comparing `svgen-0.4.5/svgen/cartesian/circle.py` & `svgen-0.4.6/svgen/cartesian/circle.py`

 * *Files identical despite different names*

### Comparing `svgen-0.4.5/svgen/cartesian/mutate.py` & `svgen-0.4.6/svgen/cartesian/mutate.py`

 * *Files identical despite different names*

### Comparing `svgen-0.4.5/svgen/cartesian/plane.py` & `svgen-0.4.6/svgen/cartesian/plane.py`

 * *Files identical despite different names*

### Comparing `svgen-0.4.5/svgen/cartesian/point.py` & `svgen-0.4.6/svgen/cartesian/point.py`

 * *Files identical despite different names*

### Comparing `svgen-0.4.5/svgen/cartesian/rectangle/__init__.py` & `svgen-0.4.6/svgen/cartesian/rectangle/__init__.py`

 * *Files identical despite different names*

### Comparing `svgen-0.4.5/svgen/cartesian/rectangle/corner.py` & `svgen-0.4.6/svgen/cartesian/rectangle/corner.py`

 * *Files identical despite different names*

### Comparing `svgen-0.4.5/svgen/cartesian/rectangle/grid.py` & `svgen-0.4.6/svgen/cartesian/rectangle/grid.py`

 * *Files identical despite different names*

### Comparing `svgen-0.4.5/svgen/color/__init__.py` & `svgen-0.4.6/svgen/color/__init__.py`

 * *Files identical despite different names*

### Comparing `svgen-0.4.5/svgen/color/alpha.py` & `svgen-0.4.6/svgen/color/alpha.py`

 * *Files identical despite different names*

### Comparing `svgen-0.4.5/svgen/color/conversion.py` & `svgen-0.4.6/svgen/color/conversion.py`

 * *Files identical despite different names*

### Comparing `svgen-0.4.5/svgen/color/hsl.py` & `svgen-0.4.6/svgen/color/hsl.py`

 * *Files identical despite different names*

### Comparing `svgen-0.4.5/svgen/color/numbers.py` & `svgen-0.4.6/svgen/color/numbers.py`

 * *Files identical despite different names*

### Comparing `svgen-0.4.5/svgen/color/rgb.py` & `svgen-0.4.6/svgen/color/rgb.py`

 * *Files identical despite different names*

### Comparing `svgen-0.4.5/svgen/color/theme/__init__.py` & `svgen-0.4.6/svgen/color/theme/__init__.py`

 * *Files identical despite different names*

### Comparing `svgen-0.4.5/svgen/color/theme/manager.py` & `svgen-0.4.6/svgen/color/theme/manager.py`

 * *Files identical despite different names*

### Comparing `svgen-0.4.5/svgen/color/theme/visualize.py` & `svgen-0.4.6/svgen/color/theme/visualize.py`

 * *Files identical despite different names*

### Comparing `svgen-0.4.5/svgen/display.py` & `svgen-0.4.6/svgen/display.py`

 * *Files identical despite different names*

### Comparing `svgen-0.4.5/svgen/element/__init__.py` & `svgen-0.4.6/svgen/element/__init__.py`

 * *Files identical despite different names*

### Comparing `svgen-0.4.5/svgen/element/circle.py` & `svgen-0.4.6/svgen/element/circle.py`

 * *Files identical despite different names*

### Comparing `svgen-0.4.5/svgen/element/line.py` & `svgen-0.4.6/svgen/element/line.py`

 * *Files identical despite different names*

### Comparing `svgen-0.4.5/svgen/element/rect.py` & `svgen-0.4.6/svgen/element/rect.py`

 * *Files identical despite different names*

### Comparing `svgen-0.4.5/svgen/element/svg.py` & `svgen-0.4.6/svgen/element/svg.py`

 * *Files identical despite different names*

### Comparing `svgen-0.4.5/svgen/entry.py` & `svgen-0.4.6/svgen/entry.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # =====================================
 # generator=datazen
-# version=3.1.0
+# version=3.1.2
 # hash=f5f67a32a57018457ae0ec8578a0eda8
 # =====================================
 
 """
 This package's command-line entry-point (boilerplate).
 """
```

### Comparing `svgen-0.4.5/svgen/generation/images.py` & `svgen-0.4.6/svgen/generation/images.py`

 * *Files identical despite different names*

### Comparing `svgen-0.4.5/svgen/inkscape.py` & `svgen-0.4.6/svgen/inkscape.py`

 * *Files identical despite different names*

### Comparing `svgen-0.4.5/svgen/shapes/chip.py` & `svgen-0.4.6/svgen/shapes/chip.py`

 * *Files identical despite different names*

### Comparing `svgen-0.4.5/svgen/shapes/pins.py` & `svgen-0.4.6/svgen/shapes/pins.py`

 * *Files identical despite different names*

### Comparing `svgen-0.4.5/svgen.egg-info/PKG-INFO` & `svgen-0.4.6/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,59 +1,65 @@
 Metadata-Version: 2.1
 Name: svgen
-Version: 0.4.5
+Version: 0.4.6
 Summary: A tool for working with scalable vector graphics.
 Home-page: https://github.com/vkottler/svgen
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
-    version=3.1.0
-    hash=bde00c56e321c249355c2d1fc449e235
+    version=3.1.2
+    hash=848c4ceae1ab8dff160beff92e43bef4
     =====================================
 -->
 
-# svgen ([0.4.5](https://pypi.org/project/svgen/))
+# svgen ([0.4.6](https://pypi.org/project/svgen/))
 
 [![python](https://img.shields.io/pypi/pyversions/svgen.svg)](https://pypi.org/project/svgen/)
 ![Build Status](https://github.com/vkottler/svgen/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/svgen/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/svgen)
 ![PyPI - Status](https://img.shields.io/pypi/status/svgen)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/svgen)
 
 *A tool for working with scalable vector graphics.*
 
-See also: [generated documentation](https://vkottler.github.io/python/pydoc/svgen.html)
-(created with [`pydoc`](https://docs.python.org/3/library/pydoc.html)).
+## Documentation
+
+### Generated
+
+* By [sphinx-apidoc](https://vkottler.github.io/python/sphinx/svgen)
+(What's [`sphinx-apidoc`](https://www.sphinx-doc.org/en/master/man/sphinx-apidoc.html)?)
+* By [pydoc](https://vkottler.github.io/python/pydoc/svgen.html)
+(What's [`pydoc`](https://docs.python.org/3/library/pydoc.html)?)
 
 ## Python Version Support
 
 This package is tested with the following Python minor versions:
 
-* [`python3.7`](https://docs.python.org/3.7/)
 * [`python3.8`](https://docs.python.org/3.8/)
 * [`python3.9`](https://docs.python.org/3.9/)
 * [`python3.10`](https://docs.python.org/3.10/)
+* [`python3.11`](https://docs.python.org/3.11/)
 
 ## Platform Support
 
 This package is tested on the following platforms:
 
 * `ubuntu-latest`
 * `macos-latest`
@@ -62,27 +68,27 @@
 # Introduction
 
 This utility provides a means to work on graphics with a programmatic workflow.
 
 # Command-line Options
 
 ```
-$ ./venv3.8/bin/svgen -h
+$ ./venv3.11/bin/svgen -h
 
 usage: svgen [-h] [--version] [-v] [-C DIR] [-c CONFIG] [--height HEIGHT]
              [--width WIDTH] [--images] [-o OUTPUT]
-             [scripts [scripts ...]]
+             [scripts ...]
 
 A tool for working with scalable vector graphics.
 
 positional arguments:
   scripts               scripts to run for composing the SVG document (in
                         order)
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
   --version             show program's version number and exit
   -v, --verbose         set to increase logging verbosity
   -C DIR, --dir DIR     execute from a specific directory
   -c CONFIG, --config CONFIG
                         top-level configuration to load (default:
                         'svgen.json')
```

### Comparing `svgen-0.4.5/svgen.egg-info/SOURCES.txt` & `svgen-0.4.6/svgen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `svgen-0.4.5/tests/test_display.py` & `svgen-0.4.6/tests/test_display.py`

 * *Files identical despite different names*

### Comparing `svgen-0.4.5/tests/test_entry.py` & `svgen-0.4.6/tests/test_entry.py`

 * *Files identical despite different names*

