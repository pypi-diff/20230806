# Comparing `tmp/pretext-1.7.5.dev20230804.tar.gz` & `tmp/pretext-1.7.5.dev20230805.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretext-1.7.5.dev20230804.tar", max compression
+gzip compressed data, was "pretext-1.7.5.dev20230805.tar", max compression
```

## Comparing `pretext-1.7.5.dev20230804.tar` & `pretext-1.7.5.dev20230805.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0    35148 2023-08-04 06:16:20.068428 pretext-1.7.5.dev20230804/LICENSE
--rw-r--r--   0        0        0     9757 2023-08-04 06:16:20.068428 pretext-1.7.5.dev20230804/README.md
--rw-r--r--   0        0        0     1500 2023-08-04 06:16:51.588597 pretext-1.7.5.dev20230804/pretext/__init__.py
--rw-r--r--   0        0        0       61 2023-08-04 06:16:20.072428 pretext-1.7.5.dev20230804/pretext/__main__.py
--rw-r--r--   0        0        0    11608 2023-08-04 06:16:20.072428 pretext-1.7.5.dev20230804/pretext/build.py
--rw-r--r--   0        0        0    27783 2023-08-04 06:16:20.072428 pretext-1.7.5.dev20230804/pretext/cli.py
--rw-r--r--   0        0        0     6149 2023-08-04 06:16:20.072428 pretext-1.7.5.dev20230804/pretext/codechat.py
--rw-r--r--   0        0        0     5943 2023-08-04 06:16:20.072428 pretext-1.7.5.dev20230804/pretext/config/xml_overlay.py
--rw-r--r--   0        0        0      675 2023-08-04 06:16:20.072428 pretext-1.7.5.dev20230804/pretext/constants.py
--rw-r--r--   0        0        0      350 2023-08-04 06:16:20.072428 pretext-1.7.5.dev20230804/pretext/core/__init__.py
--rw-r--r--   0        0        0   172548 2023-08-04 06:16:56.492621 pretext-1.7.5.dev20230804/pretext/core/pretext.py
--rw-r--r--   0        0        0     1484 2023-08-04 06:16:20.072428 pretext-1.7.5.dev20230804/pretext/core/resources.py
--rw-r--r--   0        0        0  1045313 2023-08-04 06:16:56.492621 pretext-1.7.5.dev20230804/pretext/core/resources.zip
--rw-r--r--   0        0        0    16741 2023-08-04 06:16:20.072428 pretext-1.7.5.dev20230804/pretext/generate.py
--rw-r--r--   0        0        0    29656 2023-08-04 06:16:20.072428 pretext-1.7.5.dev20230804/pretext/project/__init__.py
--rw-r--r--   0        0        0    30392 2023-08-04 06:16:20.072428 pretext-1.7.5.dev20230804/pretext/project/refactor.py
--rw-r--r--   0        0        0     2620 2023-08-04 06:16:20.072428 pretext-1.7.5.dev20230804/pretext/project/xml.py
--rw-r--r--   0        0        0      739 2023-08-04 06:16:20.072428 pretext-1.7.5.dev20230804/pretext/templates/__init__.py
--rw-r--r--   0        0        0     2480 2023-08-04 06:16:56.560621 pretext-1.7.5.dev20230804/pretext/templates/resources/.devcontainer.json
--rw-r--r--   0        0        0     1676 2023-08-04 06:16:56.560621 pretext-1.7.5.dev20230804/pretext/templates/resources/.gitignore
--rw-r--r--   0        0        0        0 2023-08-04 06:16:56.560621 pretext-1.7.5.dev20230804/pretext/templates/resources/__init__.py
--rw-r--r--   0        0        0   158949 2023-08-04 06:16:56.560621 pretext-1.7.5.dev20230804/pretext/templates/resources/article.zip
--rw-r--r--   0        0        0     6455 2023-08-04 06:16:56.532621 pretext-1.7.5.dev20230804/pretext/templates/resources/book.zip
--rw-r--r--   0        0        0   172278 2023-08-04 06:16:56.548621 pretext-1.7.5.dev20230804/pretext/templates/resources/demo.zip
--rw-r--r--   0        0        0     3496 2023-08-04 06:16:56.536621 pretext-1.7.5.dev20230804/pretext/templates/resources/hello.zip
--rw-r--r--   0        0        0     1710 2023-08-04 06:16:56.560621 pretext-1.7.5.dev20230804/pretext/templates/resources/project.ptx
--rw-r--r--   0        0        0      242 2023-08-04 06:16:56.560621 pretext-1.7.5.dev20230804/pretext/templates/resources/publication.ptx
--rw-r--r--   0        0        0     7231 2023-08-04 06:16:56.532621 pretext-1.7.5.dev20230804/pretext/templates/resources/slideshow.zip
--rw-r--r--   0        0        0      109 2023-08-04 06:16:20.072428 pretext-1.7.5.dev20230804/pretext/types.py
--rw-r--r--   0        0        0    25401 2023-08-04 06:16:20.072428 pretext-1.7.5.dev20230804/pretext/utils.py
--rw-r--r--   0        0        0     3353 2023-08-04 06:16:51.588597 pretext-1.7.5.dev20230804/pyproject.toml
--rw-r--r--   0        0        0    10891 1970-01-01 00:00:00.000000 pretext-1.7.5.dev20230804/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-08-05 06:13:44.324306 pretext-1.7.5.dev20230805/LICENSE
+-rw-r--r--   0        0        0     9757 2023-08-05 06:13:44.324306 pretext-1.7.5.dev20230805/README.md
+-rw-r--r--   0        0        0     1500 2023-08-05 06:14:28.872484 pretext-1.7.5.dev20230805/pretext/__init__.py
+-rw-r--r--   0        0        0       61 2023-08-05 06:13:44.324306 pretext-1.7.5.dev20230805/pretext/__main__.py
+-rw-r--r--   0        0        0    11608 2023-08-05 06:13:44.324306 pretext-1.7.5.dev20230805/pretext/build.py
+-rw-r--r--   0        0        0    27783 2023-08-05 06:13:44.324306 pretext-1.7.5.dev20230805/pretext/cli.py
+-rw-r--r--   0        0        0     6149 2023-08-05 06:13:44.324306 pretext-1.7.5.dev20230805/pretext/codechat.py
+-rw-r--r--   0        0        0     5943 2023-08-05 06:13:44.324306 pretext-1.7.5.dev20230805/pretext/config/xml_overlay.py
+-rw-r--r--   0        0        0      675 2023-08-05 06:13:44.324306 pretext-1.7.5.dev20230805/pretext/constants.py
+-rw-r--r--   0        0        0      350 2023-08-05 06:13:44.324306 pretext-1.7.5.dev20230805/pretext/core/__init__.py
+-rw-r--r--   0        0        0   172548 2023-08-05 06:14:34.208541 pretext-1.7.5.dev20230805/pretext/core/pretext.py
+-rw-r--r--   0        0        0     1484 2023-08-05 06:13:44.324306 pretext-1.7.5.dev20230805/pretext/core/resources.py
+-rw-r--r--   0        0        0  1045313 2023-08-05 06:14:34.208541 pretext-1.7.5.dev20230805/pretext/core/resources.zip
+-rw-r--r--   0        0        0    16741 2023-08-05 06:13:44.324306 pretext-1.7.5.dev20230805/pretext/generate.py
+-rw-r--r--   0        0        0    29656 2023-08-05 06:13:44.324306 pretext-1.7.5.dev20230805/pretext/project/__init__.py
+-rw-r--r--   0        0        0    30392 2023-08-05 06:13:44.324306 pretext-1.7.5.dev20230805/pretext/project/refactor.py
+-rw-r--r--   0        0        0     2620 2023-08-05 06:13:44.324306 pretext-1.7.5.dev20230805/pretext/project/xml.py
+-rw-r--r--   0        0        0      739 2023-08-05 06:13:44.324306 pretext-1.7.5.dev20230805/pretext/templates/__init__.py
+-rw-r--r--   0        0        0     2480 2023-08-05 06:14:34.304542 pretext-1.7.5.dev20230805/pretext/templates/resources/.devcontainer.json
+-rw-r--r--   0        0        0     1676 2023-08-05 06:14:34.304542 pretext-1.7.5.dev20230805/pretext/templates/resources/.gitignore
+-rw-r--r--   0        0        0        0 2023-08-05 06:14:34.304542 pretext-1.7.5.dev20230805/pretext/templates/resources/__init__.py
+-rw-r--r--   0        0        0   158949 2023-08-05 06:14:34.300542 pretext-1.7.5.dev20230805/pretext/templates/resources/article.zip
+-rw-r--r--   0        0        0     6455 2023-08-05 06:14:34.260542 pretext-1.7.5.dev20230805/pretext/templates/resources/book.zip
+-rw-r--r--   0        0        0   172278 2023-08-05 06:14:34.288542 pretext-1.7.5.dev20230805/pretext/templates/resources/demo.zip
+-rw-r--r--   0        0        0     3496 2023-08-05 06:14:34.268542 pretext-1.7.5.dev20230805/pretext/templates/resources/hello.zip
+-rw-r--r--   0        0        0     1710 2023-08-05 06:14:34.304542 pretext-1.7.5.dev20230805/pretext/templates/resources/project.ptx
+-rw-r--r--   0        0        0      242 2023-08-05 06:14:34.304542 pretext-1.7.5.dev20230805/pretext/templates/resources/publication.ptx
+-rw-r--r--   0        0        0     7231 2023-08-05 06:14:34.264542 pretext-1.7.5.dev20230805/pretext/templates/resources/slideshow.zip
+-rw-r--r--   0        0        0      109 2023-08-05 06:13:44.324306 pretext-1.7.5.dev20230805/pretext/types.py
+-rw-r--r--   0        0        0    25401 2023-08-05 06:13:44.324306 pretext-1.7.5.dev20230805/pretext/utils.py
+-rw-r--r--   0        0        0     3353 2023-08-05 06:14:28.872484 pretext-1.7.5.dev20230805/pyproject.toml
+-rw-r--r--   0        0        0    10891 1970-01-01 00:00:00.000000 pretext-1.7.5.dev20230805/PKG-INFO
```

### Comparing `pretext-1.7.5.dev20230804/LICENSE` & `pretext-1.7.5.dev20230805/LICENSE`

 * *Files identical despite different names*

### Comparing `pretext-1.7.5.dev20230804/README.md` & `pretext-1.7.5.dev20230805/README.md`

 * *Files identical despite different names*

### Comparing `pretext-1.7.5.dev20230804/pretext/__init__.py` & `pretext-1.7.5.dev20230805/pretext/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from pathlib import Path
 from single_version import get_version
 
 log = logging.getLogger("ptxlogger")
 
 VERSION = get_version("pretext", Path(__file__).parent.parent)
 
-CORE_COMMIT = 'e44345df4ee4a0e382c5f5a77f1bb4ac414a931f'
+CORE_COMMIT = '0e1d2ae93af3a2b0a7bca038422a34d192445035'
 
 
 def activate() -> None:
     """
     This function was provided by the original `pretext` package
     deployed to PyPI by Alex Willmer. Thanks to their generosity,
     we were allowed to adopt this namespace as of 1.0, so we raise an error here
```

### Comparing `pretext-1.7.5.dev20230804/pretext/build.py` & `pretext-1.7.5.dev20230805/pretext/build.py`

 * *Files identical despite different names*

### Comparing `pretext-1.7.5.dev20230804/pretext/cli.py` & `pretext-1.7.5.dev20230805/pretext/cli.py`

 * *Files identical despite different names*

### Comparing `pretext-1.7.5.dev20230804/pretext/codechat.py` & `pretext-1.7.5.dev20230805/pretext/codechat.py`

 * *Files identical despite different names*

### Comparing `pretext-1.7.5.dev20230804/pretext/config/xml_overlay.py` & `pretext-1.7.5.dev20230805/pretext/config/xml_overlay.py`

 * *Files identical despite different names*

### Comparing `pretext-1.7.5.dev20230804/pretext/constants.py` & `pretext-1.7.5.dev20230805/pretext/constants.py`

 * *Files identical despite different names*

### Comparing `pretext-1.7.5.dev20230804/pretext/core/pretext.py` & `pretext-1.7.5.dev20230805/pretext/core/pretext.py`

 * *Files identical despite different names*

### Comparing `pretext-1.7.5.dev20230804/pretext/core/resources.py` & `pretext-1.7.5.dev20230805/pretext/core/resources.py`

 * *Files identical despite different names*

### Comparing `pretext-1.7.5.dev20230804/pretext/core/resources.zip` & `pretext-1.7.5.dev20230805/pretext/core/resources.zip`

 * *Files 10% similar despite different names*

#### zipinfo {}

```diff
@@ -1,144 +1,144 @@
 Zip file size: 1045313 bytes, number of entries: 142
-drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-04 06:16 css/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-04 06:16 pretext/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-04 06:16 schema/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-04 06:16 script/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-04 06:16 xsl/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-04 06:16 script/mjsre/
--rw-r--r--  2.0 unx      258 b- defN 23-Aug-04 06:16 script/README.md
--rw-r--r--  2.0 unx     2666 b- defN 23-Aug-04 06:16 script/mbx
--rw-r--r--  2.0 unx      116 b- defN 23-Aug-04 06:16 script/mjsre/package.json
--rw-r--r--  2.0 unx       92 b- defN 23-Aug-04 06:16 script/mjsre/update-sre
--rw-r--r--  2.0 unx     9251 b- defN 23-Aug-04 06:16 script/mjsre/mj-sre-page.js
--rw-r--r--  2.0 unx      481 b- defN 23-Aug-04 06:16 script/mjsre/README.md
--rw-r--r--  2.0 unx   134086 b- defN 23-Aug-04 06:16 schema/pretext.xml
--rw-r--r--  2.0 unx   125241 b- defN 23-Aug-04 06:16 schema/pretext.xsd
--rw-r--r--  2.0 unx    18421 b- defN 23-Aug-04 06:16 schema/pretext-schematron.xsl
--rw-r--r--  2.0 unx    25870 b- defN 23-Aug-04 06:16 schema/pretext-validation-plus.xsl
--rw-r--r--  2.0 unx    58129 b- defN 23-Aug-04 06:16 schema/pretext.rnc
--rw-r--r--  2.0 unx      326 b- defN 23-Aug-04 06:16 schema/xml.xsd
--rw-r--r--  2.0 unx   101895 b- defN 23-Aug-04 06:16 schema/pretext.rng
--rw-r--r--  2.0 unx    17587 b- defN 23-Aug-04 06:16 schema/pretext-dev.rnc
--rw-r--r--  2.0 unx     1180 b- defN 23-Aug-04 06:16 schema/README.md
--rw-r--r--  2.0 unx    34210 b- defN 23-Aug-04 06:16 schema/pretext-dev.rng
--rw-r--r--  2.0 unx     3135 b- defN 23-Aug-04 06:16 schema/build.sh
--rw-r--r--  2.0 unx     2566 b- defN 23-Aug-04 06:16 pretext/pretext.cfg
--rw-r--r--  2.0 unx     1955 b- defN 23-Aug-04 06:16 pretext/module-test.py
--rw-r--r--  2.0 unx    30908 b- defN 23-Aug-04 06:16 pretext/pretext
--rw-r--r--  2.0 unx   172548 b- defN 23-Aug-04 06:16 pretext/pretext.py
--rw-r--r--  2.0 unx    36045 b- defN 23-Aug-04 06:16 pretext/braille_format.py
--rw-r--r--  2.0 unx     1367 b- defN 23-Aug-04 06:16 pretext/README.md
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-04 06:16 pretext/__init__.py
--rw-r--r--  2.0 unx     2446 b- defN 23-Aug-04 06:16 css/colors_martiansands.css
--rw-r--r--  2.0 unx     4021 b- defN 23-Aug-04 06:16 css/update_css
--rw-r--r--  2.0 unx    71198 b- defN 23-Aug-04 06:16 css/pretext_add_on.css
--rw-r--r--  2.0 unx    12567 b- defN 23-Aug-04 06:16 css/style_oscarlevin.css
--rw-r--r--  2.0 unx     1276 b- defN 23-Aug-04 06:16 css/colors_maroon_grey.css
--rw-r--r--  2.0 unx    63664 b- defN 23-Aug-04 06:16 css/mathbook-add-on.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Aug-04 06:16 css/colors_green_blue.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Aug-04 06:16 css/colors_ruby_emerald.css
--rw-r--r--  2.0 unx     2441 b- defN 23-Aug-04 06:16 css/kindle.css
--rw-r--r--  2.0 unx    22438 b- defN 23-Aug-04 06:16 css/pretext.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Aug-04 06:16 css/colors_blue_red.css
--rw-r--r--  2.0 unx     2446 b- defN 23-Aug-04 06:16 css/colors_darkmartiansands.css
--rw-r--r--  2.0 unx     1362 b- defN 23-Aug-04 06:16 css/epub.css
--rw-r--r--  2.0 unx     3473 b- defN 23-Aug-04 06:16 css/style_soundwriting.css
--rw-r--r--  2.0 unx      691 b- defN 23-Aug-04 06:16 css/colors_pastel_blue_orange.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Aug-04 06:16 css/colors_ruby_turquoise.css
--rw-r--r--  2.0 unx     2608 b- defN 23-Aug-04 06:16 css/colors_default.css
--rw-r--r--  2.0 unx     2438 b- defN 23-Aug-04 06:16 css/colors_blue_grey.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Aug-04 06:16 css/colors_orange_navy.css
--rw-r--r--  2.0 unx   435680 b- defN 23-Aug-04 06:16 css/mathbook-3.css
--rw-r--r--  2.0 unx     7761 b- defN 23-Aug-04 06:16 css/style_default.css
--rw-r--r--  2.0 unx     1338 b- defN 23-Aug-04 06:16 css/colors_red_blue.css
--rw-r--r--  2.0 unx   146685 b- defN 23-Aug-04 06:16 css/mathbook-content.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Aug-04 06:16 css/colors_ruby_amethyst.css
--rw-r--r--  2.0 unx     1865 b- defN 23-Aug-04 06:16 css/README.md
--rw-r--r--  2.0 unx     2397 b- defN 23-Aug-04 06:16 css/colors_green_plum.css
--rw-r--r--  2.0 unx     4308 b- defN 23-Aug-04 06:16 css/colors_blue_green.css
--rw-r--r--  2.0 unx     1280 b- defN 23-Aug-04 06:16 css/colors_brown_gold.css
--rw-r--r--  2.0 unx    14069 b- defN 23-Aug-04 06:16 css/setcolors.css
-drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-04 06:16 xsl/latex/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-04 06:16 xsl/localizations/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-04 06:16 xsl/support/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-04 06:16 xsl/utilities/
--rw-r--r--  2.0 unx     2725 b- defN 23-Aug-04 06:16 xsl/extract-asymptote.xsl
--rw-r--r--  2.0 unx    10708 b- defN 23-Aug-04 06:16 xsl/pretext-units.xsl
--rw-r--r--  2.0 unx    17293 b- defN 23-Aug-04 06:16 xsl/pretext-ww-problem-sets.xsl
--rw-r--r--  2.0 unx     4571 b- defN 23-Aug-04 06:16 xsl/pretext-litprog.xsl
--rw-r--r--  2.0 unx     8125 b- defN 23-Aug-04 06:16 xsl/extract-sageplot.xsl
--rw-r--r--  2.0 unx   548615 b- defN 23-Aug-04 06:16 xsl/pretext-common.xsl
--rw-r--r--  2.0 unx     3560 b- defN 23-Aug-04 06:16 xsl/pretext-basic-html.xsl
--rw-r--r--  2.0 unx    21086 b- defN 23-Aug-04 06:16 xsl/pretext-smc.xsl
--rw-r--r--  2.0 unx     2597 b- defN 23-Aug-04 06:16 xsl/extract-trace.xsl
--rw-r--r--  2.0 unx    19072 b- defN 23-Aug-04 06:16 xsl/extract-latex-image.xsl
--rw-r--r--  2.0 unx     2248 b- defN 23-Aug-04 06:16 xsl/extract-mom.xsl
--rw-r--r--  2.0 unx    67275 b- defN 23-Aug-04 06:16 xsl/pretext-epub.xsl
--rw-r--r--  2.0 unx    11766 b- defN 23-Aug-04 06:16 xsl/pretext-sage-doctest.xsl
--rw-r--r--  2.0 unx     6066 b- defN 23-Aug-04 06:16 xsl/pretext-json-manifest.xsl
--rw-r--r--  2.0 unx    22121 b- defN 23-Aug-04 06:16 xsl/pretext-revealjs.xsl
--rw-r--r--  2.0 unx     2740 b- defN 23-Aug-04 06:16 xsl/extract-youtube.xsl
--rw-r--r--  2.0 unx    40230 b- defN 23-Aug-04 06:16 xsl/pretext-jupyter.xsl
--rw-r--r--  2.0 unx   611284 b- defN 23-Aug-04 06:16 xsl/pretext-html.xsl
--rw-r--r--  2.0 unx    39918 b- defN 23-Aug-04 06:16 xsl/pretext-runestone-static.xsl
--rw-r--r--  2.0 unx     9787 b- defN 23-Aug-04 06:16 xsl/entities.ent
--rw-r--r--  2.0 unx     3239 b- defN 23-Aug-04 06:16 xsl/extract-interactive.xsl
--rw-r--r--  2.0 unx   231265 b- defN 23-Aug-04 06:16 xsl/publisher-variables.xsl
--rw-r--r--  2.0 unx     2709 b- defN 23-Aug-04 06:16 xsl/extract-qrcode.xsl
--rw-r--r--  2.0 unx    13037 b- defN 23-Aug-04 06:16 xsl/pretext-text.xsl
--rw-r--r--  2.0 unx    41730 b- defN 23-Aug-04 06:16 xsl/pretext-beamer.xsl
--rw-r--r--  2.0 unx    43020 b- defN 23-Aug-04 06:16 xsl/pretext-text-utilities.xsl
--rw-r--r--  2.0 unx     2601 b- defN 23-Aug-04 06:16 xsl/pretext-merge.xsl
--rw-r--r--  2.0 unx   139486 b- defN 23-Aug-04 06:16 xsl/extract-pg.xsl
--rw-r--r--  2.0 unx   116581 b- defN 23-Aug-04 06:16 xsl/pretext-assembly.xsl
--rw-r--r--  2.0 unx     2846 b- defN 23-Aug-04 06:16 xsl/extract-datafile.xsl
--rw-r--r--  2.0 unx     1768 b- defN 23-Aug-04 06:16 xsl/README.md
--rw-r--r--  2.0 unx    13186 b- defN 23-Aug-04 06:16 xsl/pretext-solution-manual-latex.xsl
--rw-r--r--  2.0 unx     6281 b- defN 23-Aug-04 06:16 xsl/pretext-numbers.xsl
--rw-r--r--  2.0 unx     8535 b- defN 23-Aug-04 06:16 xsl/pretext-view-source.xsl
--rw-r--r--  2.0 unx    12084 b- defN 23-Aug-04 06:16 xsl/xml-to-json.xsl
--rw-r--r--  2.0 unx     8130 b- defN 23-Aug-04 06:16 xsl/extract-identity.xsl
--rw-r--r--  2.0 unx    94587 b- defN 23-Aug-04 06:16 xsl/pretext-braille-preprint.xsl
--rw-r--r--  2.0 unx   111515 b- defN 23-Aug-04 06:16 xsl/pretext-runestone.xsl
--rw-r--r--  2.0 unx   544154 b- defN 23-Aug-04 06:16 xsl/pretext-latex.xsl
--rw-r--r--  2.0 unx      787 b- defN 23-Aug-04 06:16 xsl/utilities/deprecate-index.sed
--rw-r--r--  2.0 unx      513 b- defN 23-Aug-04 06:16 xsl/utilities/deprecate-autoname.sed
--rw-r--r--  2.0 unx     4926 b- defN 23-Aug-04 06:16 xsl/utilities/pretext-enhanced-source.xsl
--rw-r--r--  2.0 unx    30257 b- defN 23-Aug-04 06:16 xsl/utilities/fix-deprecations.xsl
--rw-r--r--  2.0 unx     1810 b- defN 23-Aug-04 06:16 xsl/utilities/README.md
--rw-r--r--  2.0 unx     4299 b- defN 23-Aug-04 06:16 xsl/utilities/author-report.xsl
-drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-04 06:16 xsl/support/play-button/
--rw-r--r--  2.0 unx     5879 b- defN 23-Aug-04 06:16 xsl/support/package-math.xsl
--rw-r--r--  2.0 unx     5241 b- defN 23-Aug-04 06:16 xsl/support/pretext-pg-macros.xsl
--rw-r--r--  2.0 unx      486 b- defN 23-Aug-04 06:16 xsl/support/runestone-services.xml
--rw-r--r--  2.0 unx    10306 b- defN 23-Aug-04 06:16 xsl/support/extract-math.xsl
--rw-r--r--  2.0 unx     5065 b- defN 23-Aug-04 06:16 xsl/support/extract-latex-image-labels.xsl
--rw-r--r--  2.0 unx      504 b- defN 23-Aug-04 06:16 xsl/support/README.md
--rw-r--r--  2.0 unx     5800 b- defN 23-Aug-04 06:16 xsl/support/tactile-svg.xsl
--rw-r--r--  2.0 unx      722 b- defN 23-Aug-04 06:16 xsl/support/play-button/play-button.svg
--rw-r--r--  2.0 unx     2657 b- defN 23-Aug-04 06:16 xsl/support/play-button/README.md
--rw-r--r--  2.0 unx     6621 b- defN 23-Aug-04 06:16 xsl/support/play-button/play-button.png
--rw-r--r--  2.0 unx    17231 b- defN 23-Aug-04 06:16 xsl/localizations/de-DE.xml
--rw-r--r--  2.0 unx    16312 b- defN 23-Aug-04 06:16 xsl/localizations/pt-BR.xml
--rw-r--r--  2.0 unx     2286 b- defN 23-Aug-04 06:16 xsl/localizations/localizations.xml
--rw-r--r--  2.0 unx    17301 b- defN 23-Aug-04 06:16 xsl/localizations/fi-FI.xml
--rw-r--r--  2.0 unx    16349 b- defN 23-Aug-04 06:16 xsl/localizations/fr-FR.xml
--rw-r--r--  2.0 unx    16534 b- defN 23-Aug-04 06:16 xsl/localizations/es-ES.xml
--rw-r--r--  2.0 unx    16837 b- defN 23-Aug-04 06:16 xsl/localizations/af-ZA.xml
--rw-r--r--  2.0 unx    19185 b- defN 23-Aug-04 06:16 xsl/localizations/nl-NL.xml
--rw-r--r--  2.0 unx    16252 b- defN 23-Aug-04 06:16 xsl/localizations/ca-ES.xml
--rw-r--r--  2.0 unx    17056 b- defN 23-Aug-04 06:16 xsl/localizations/bg-BG.xml
--rw-r--r--  2.0 unx    17081 b- defN 23-Aug-04 06:16 xsl/localizations/pt-PT.xml
--rw-r--r--  2.0 unx    15582 b- defN 23-Aug-04 06:16 xsl/localizations/cs-CZ.xml
--rw-r--r--  2.0 unx    20481 b- defN 23-Aug-04 06:16 xsl/localizations/ku-CKB.xml
--rw-r--r--  2.0 unx    19326 b- defN 23-Aug-04 06:16 xsl/localizations/en-US.xml
--rw-r--r--  2.0 unx     4760 b- defN 23-Aug-04 06:16 xsl/localizations/README.md
--rw-r--r--  2.0 unx    15866 b- defN 23-Aug-04 06:16 xsl/localizations/it-IT.xml
--rw-r--r--  2.0 unx    16085 b- defN 23-Aug-04 06:16 xsl/localizations/hu-HU.xml
--rw-r--r--  2.0 unx    16500 b- defN 23-Aug-04 06:16 xsl/localizations/fr-CA.xml
--rw-r--r--  2.0 unx     5135 b- defN 23-Aug-04 06:16 xsl/latex/pretext-latex-guide.xsl
--rw-r--r--  2.0 unx     2261 b- defN 23-Aug-04 06:16 xsl/latex/pretext-latex-AIM.xsl
--rw-r--r--  2.0 unx    14482 b- defN 23-Aug-04 06:16 xsl/latex/pretext-latex-chaos.xsl
--rw-r--r--  2.0 unx     7526 b- defN 23-Aug-04 06:16 xsl/latex/pretext-latex-CLP.xsl
--rw-r--r--  2.0 unx     3024 b- defN 23-Aug-04 06:16 xsl/latex/pretext-latex-dyslexic-font.xsl
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-05 06:14 css/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-05 06:14 pretext/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-05 06:14 schema/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-05 06:14 script/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-05 06:14 xsl/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-05 06:14 script/mjsre/
+-rw-r--r--  2.0 unx      258 b- defN 23-Aug-05 06:14 script/README.md
+-rw-r--r--  2.0 unx     2666 b- defN 23-Aug-05 06:14 script/mbx
+-rw-r--r--  2.0 unx      116 b- defN 23-Aug-05 06:14 script/mjsre/package.json
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-05 06:14 script/mjsre/update-sre
+-rw-r--r--  2.0 unx     9251 b- defN 23-Aug-05 06:14 script/mjsre/mj-sre-page.js
+-rw-r--r--  2.0 unx      481 b- defN 23-Aug-05 06:14 script/mjsre/README.md
+-rw-r--r--  2.0 unx   134086 b- defN 23-Aug-05 06:14 schema/pretext.xml
+-rw-r--r--  2.0 unx   125241 b- defN 23-Aug-05 06:14 schema/pretext.xsd
+-rw-r--r--  2.0 unx    18421 b- defN 23-Aug-05 06:14 schema/pretext-schematron.xsl
+-rw-r--r--  2.0 unx    25870 b- defN 23-Aug-05 06:14 schema/pretext-validation-plus.xsl
+-rw-r--r--  2.0 unx    58129 b- defN 23-Aug-05 06:14 schema/pretext.rnc
+-rw-r--r--  2.0 unx      326 b- defN 23-Aug-05 06:14 schema/xml.xsd
+-rw-r--r--  2.0 unx   101895 b- defN 23-Aug-05 06:14 schema/pretext.rng
+-rw-r--r--  2.0 unx    17587 b- defN 23-Aug-05 06:14 schema/pretext-dev.rnc
+-rw-r--r--  2.0 unx     1180 b- defN 23-Aug-05 06:14 schema/README.md
+-rw-r--r--  2.0 unx    34210 b- defN 23-Aug-05 06:14 schema/pretext-dev.rng
+-rw-r--r--  2.0 unx     3135 b- defN 23-Aug-05 06:14 schema/build.sh
+-rw-r--r--  2.0 unx     2566 b- defN 23-Aug-05 06:14 pretext/pretext.cfg
+-rw-r--r--  2.0 unx     1955 b- defN 23-Aug-05 06:14 pretext/module-test.py
+-rw-r--r--  2.0 unx    30908 b- defN 23-Aug-05 06:14 pretext/pretext
+-rw-r--r--  2.0 unx   172548 b- defN 23-Aug-05 06:14 pretext/pretext.py
+-rw-r--r--  2.0 unx    36045 b- defN 23-Aug-05 06:14 pretext/braille_format.py
+-rw-r--r--  2.0 unx     1367 b- defN 23-Aug-05 06:14 pretext/README.md
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-05 06:14 pretext/__init__.py
+-rw-r--r--  2.0 unx     2446 b- defN 23-Aug-05 06:14 css/colors_martiansands.css
+-rw-r--r--  2.0 unx     4021 b- defN 23-Aug-05 06:14 css/update_css
+-rw-r--r--  2.0 unx    71198 b- defN 23-Aug-05 06:14 css/pretext_add_on.css
+-rw-r--r--  2.0 unx    12567 b- defN 23-Aug-05 06:14 css/style_oscarlevin.css
+-rw-r--r--  2.0 unx     1276 b- defN 23-Aug-05 06:14 css/colors_maroon_grey.css
+-rw-r--r--  2.0 unx    63664 b- defN 23-Aug-05 06:14 css/mathbook-add-on.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Aug-05 06:14 css/colors_green_blue.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Aug-05 06:14 css/colors_ruby_emerald.css
+-rw-r--r--  2.0 unx     2441 b- defN 23-Aug-05 06:14 css/kindle.css
+-rw-r--r--  2.0 unx    22438 b- defN 23-Aug-05 06:14 css/pretext.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Aug-05 06:14 css/colors_blue_red.css
+-rw-r--r--  2.0 unx     2446 b- defN 23-Aug-05 06:14 css/colors_darkmartiansands.css
+-rw-r--r--  2.0 unx     1362 b- defN 23-Aug-05 06:14 css/epub.css
+-rw-r--r--  2.0 unx     3473 b- defN 23-Aug-05 06:14 css/style_soundwriting.css
+-rw-r--r--  2.0 unx      691 b- defN 23-Aug-05 06:14 css/colors_pastel_blue_orange.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Aug-05 06:14 css/colors_ruby_turquoise.css
+-rw-r--r--  2.0 unx     2608 b- defN 23-Aug-05 06:14 css/colors_default.css
+-rw-r--r--  2.0 unx     2438 b- defN 23-Aug-05 06:14 css/colors_blue_grey.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Aug-05 06:14 css/colors_orange_navy.css
+-rw-r--r--  2.0 unx   435680 b- defN 23-Aug-05 06:14 css/mathbook-3.css
+-rw-r--r--  2.0 unx     7761 b- defN 23-Aug-05 06:14 css/style_default.css
+-rw-r--r--  2.0 unx     1338 b- defN 23-Aug-05 06:14 css/colors_red_blue.css
+-rw-r--r--  2.0 unx   146685 b- defN 23-Aug-05 06:14 css/mathbook-content.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Aug-05 06:14 css/colors_ruby_amethyst.css
+-rw-r--r--  2.0 unx     1865 b- defN 23-Aug-05 06:14 css/README.md
+-rw-r--r--  2.0 unx     2397 b- defN 23-Aug-05 06:14 css/colors_green_plum.css
+-rw-r--r--  2.0 unx     4308 b- defN 23-Aug-05 06:14 css/colors_blue_green.css
+-rw-r--r--  2.0 unx     1280 b- defN 23-Aug-05 06:14 css/colors_brown_gold.css
+-rw-r--r--  2.0 unx    14069 b- defN 23-Aug-05 06:14 css/setcolors.css
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-05 06:14 xsl/latex/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-05 06:14 xsl/localizations/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-05 06:14 xsl/support/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-05 06:14 xsl/utilities/
+-rw-r--r--  2.0 unx     2725 b- defN 23-Aug-05 06:14 xsl/extract-asymptote.xsl
+-rw-r--r--  2.0 unx    10708 b- defN 23-Aug-05 06:14 xsl/pretext-units.xsl
+-rw-r--r--  2.0 unx    17293 b- defN 23-Aug-05 06:14 xsl/pretext-ww-problem-sets.xsl
+-rw-r--r--  2.0 unx     4571 b- defN 23-Aug-05 06:14 xsl/pretext-litprog.xsl
+-rw-r--r--  2.0 unx     8125 b- defN 23-Aug-05 06:14 xsl/extract-sageplot.xsl
+-rw-r--r--  2.0 unx   548615 b- defN 23-Aug-05 06:14 xsl/pretext-common.xsl
+-rw-r--r--  2.0 unx     3560 b- defN 23-Aug-05 06:14 xsl/pretext-basic-html.xsl
+-rw-r--r--  2.0 unx    21086 b- defN 23-Aug-05 06:14 xsl/pretext-smc.xsl
+-rw-r--r--  2.0 unx     2597 b- defN 23-Aug-05 06:14 xsl/extract-trace.xsl
+-rw-r--r--  2.0 unx    19072 b- defN 23-Aug-05 06:14 xsl/extract-latex-image.xsl
+-rw-r--r--  2.0 unx     2248 b- defN 23-Aug-05 06:14 xsl/extract-mom.xsl
+-rw-r--r--  2.0 unx    67275 b- defN 23-Aug-05 06:14 xsl/pretext-epub.xsl
+-rw-r--r--  2.0 unx    11766 b- defN 23-Aug-05 06:14 xsl/pretext-sage-doctest.xsl
+-rw-r--r--  2.0 unx     6066 b- defN 23-Aug-05 06:14 xsl/pretext-json-manifest.xsl
+-rw-r--r--  2.0 unx    22121 b- defN 23-Aug-05 06:14 xsl/pretext-revealjs.xsl
+-rw-r--r--  2.0 unx     2740 b- defN 23-Aug-05 06:14 xsl/extract-youtube.xsl
+-rw-r--r--  2.0 unx    40230 b- defN 23-Aug-05 06:14 xsl/pretext-jupyter.xsl
+-rw-r--r--  2.0 unx   611284 b- defN 23-Aug-05 06:14 xsl/pretext-html.xsl
+-rw-r--r--  2.0 unx    39918 b- defN 23-Aug-05 06:14 xsl/pretext-runestone-static.xsl
+-rw-r--r--  2.0 unx     9787 b- defN 23-Aug-05 06:14 xsl/entities.ent
+-rw-r--r--  2.0 unx     3239 b- defN 23-Aug-05 06:14 xsl/extract-interactive.xsl
+-rw-r--r--  2.0 unx   231265 b- defN 23-Aug-05 06:14 xsl/publisher-variables.xsl
+-rw-r--r--  2.0 unx     2709 b- defN 23-Aug-05 06:14 xsl/extract-qrcode.xsl
+-rw-r--r--  2.0 unx    13037 b- defN 23-Aug-05 06:14 xsl/pretext-text.xsl
+-rw-r--r--  2.0 unx    41730 b- defN 23-Aug-05 06:14 xsl/pretext-beamer.xsl
+-rw-r--r--  2.0 unx    43020 b- defN 23-Aug-05 06:14 xsl/pretext-text-utilities.xsl
+-rw-r--r--  2.0 unx     2601 b- defN 23-Aug-05 06:14 xsl/pretext-merge.xsl
+-rw-r--r--  2.0 unx   139486 b- defN 23-Aug-05 06:14 xsl/extract-pg.xsl
+-rw-r--r--  2.0 unx   116581 b- defN 23-Aug-05 06:14 xsl/pretext-assembly.xsl
+-rw-r--r--  2.0 unx     2846 b- defN 23-Aug-05 06:14 xsl/extract-datafile.xsl
+-rw-r--r--  2.0 unx     1768 b- defN 23-Aug-05 06:14 xsl/README.md
+-rw-r--r--  2.0 unx    13186 b- defN 23-Aug-05 06:14 xsl/pretext-solution-manual-latex.xsl
+-rw-r--r--  2.0 unx     6281 b- defN 23-Aug-05 06:14 xsl/pretext-numbers.xsl
+-rw-r--r--  2.0 unx     8535 b- defN 23-Aug-05 06:14 xsl/pretext-view-source.xsl
+-rw-r--r--  2.0 unx    12084 b- defN 23-Aug-05 06:14 xsl/xml-to-json.xsl
+-rw-r--r--  2.0 unx     8130 b- defN 23-Aug-05 06:14 xsl/extract-identity.xsl
+-rw-r--r--  2.0 unx    94587 b- defN 23-Aug-05 06:14 xsl/pretext-braille-preprint.xsl
+-rw-r--r--  2.0 unx   111515 b- defN 23-Aug-05 06:14 xsl/pretext-runestone.xsl
+-rw-r--r--  2.0 unx   544154 b- defN 23-Aug-05 06:14 xsl/pretext-latex.xsl
+-rw-r--r--  2.0 unx      787 b- defN 23-Aug-05 06:14 xsl/utilities/deprecate-index.sed
+-rw-r--r--  2.0 unx      513 b- defN 23-Aug-05 06:14 xsl/utilities/deprecate-autoname.sed
+-rw-r--r--  2.0 unx     4926 b- defN 23-Aug-05 06:14 xsl/utilities/pretext-enhanced-source.xsl
+-rw-r--r--  2.0 unx    30257 b- defN 23-Aug-05 06:14 xsl/utilities/fix-deprecations.xsl
+-rw-r--r--  2.0 unx     1810 b- defN 23-Aug-05 06:14 xsl/utilities/README.md
+-rw-r--r--  2.0 unx     4299 b- defN 23-Aug-05 06:14 xsl/utilities/author-report.xsl
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-05 06:14 xsl/support/play-button/
+-rw-r--r--  2.0 unx     5879 b- defN 23-Aug-05 06:14 xsl/support/package-math.xsl
+-rw-r--r--  2.0 unx     5241 b- defN 23-Aug-05 06:14 xsl/support/pretext-pg-macros.xsl
+-rw-r--r--  2.0 unx      486 b- defN 23-Aug-05 06:14 xsl/support/runestone-services.xml
+-rw-r--r--  2.0 unx    10306 b- defN 23-Aug-05 06:14 xsl/support/extract-math.xsl
+-rw-r--r--  2.0 unx     5065 b- defN 23-Aug-05 06:14 xsl/support/extract-latex-image-labels.xsl
+-rw-r--r--  2.0 unx      504 b- defN 23-Aug-05 06:14 xsl/support/README.md
+-rw-r--r--  2.0 unx     5800 b- defN 23-Aug-05 06:14 xsl/support/tactile-svg.xsl
+-rw-r--r--  2.0 unx      722 b- defN 23-Aug-05 06:14 xsl/support/play-button/play-button.svg
+-rw-r--r--  2.0 unx     2657 b- defN 23-Aug-05 06:14 xsl/support/play-button/README.md
+-rw-r--r--  2.0 unx     6621 b- defN 23-Aug-05 06:14 xsl/support/play-button/play-button.png
+-rw-r--r--  2.0 unx    17231 b- defN 23-Aug-05 06:14 xsl/localizations/de-DE.xml
+-rw-r--r--  2.0 unx    16312 b- defN 23-Aug-05 06:14 xsl/localizations/pt-BR.xml
+-rw-r--r--  2.0 unx     2286 b- defN 23-Aug-05 06:14 xsl/localizations/localizations.xml
+-rw-r--r--  2.0 unx    17301 b- defN 23-Aug-05 06:14 xsl/localizations/fi-FI.xml
+-rw-r--r--  2.0 unx    16349 b- defN 23-Aug-05 06:14 xsl/localizations/fr-FR.xml
+-rw-r--r--  2.0 unx    16534 b- defN 23-Aug-05 06:14 xsl/localizations/es-ES.xml
+-rw-r--r--  2.0 unx    16837 b- defN 23-Aug-05 06:14 xsl/localizations/af-ZA.xml
+-rw-r--r--  2.0 unx    19185 b- defN 23-Aug-05 06:14 xsl/localizations/nl-NL.xml
+-rw-r--r--  2.0 unx    16252 b- defN 23-Aug-05 06:14 xsl/localizations/ca-ES.xml
+-rw-r--r--  2.0 unx    17056 b- defN 23-Aug-05 06:14 xsl/localizations/bg-BG.xml
+-rw-r--r--  2.0 unx    17081 b- defN 23-Aug-05 06:14 xsl/localizations/pt-PT.xml
+-rw-r--r--  2.0 unx    15582 b- defN 23-Aug-05 06:14 xsl/localizations/cs-CZ.xml
+-rw-r--r--  2.0 unx    20481 b- defN 23-Aug-05 06:14 xsl/localizations/ku-CKB.xml
+-rw-r--r--  2.0 unx    19326 b- defN 23-Aug-05 06:14 xsl/localizations/en-US.xml
+-rw-r--r--  2.0 unx     4760 b- defN 23-Aug-05 06:14 xsl/localizations/README.md
+-rw-r--r--  2.0 unx    15866 b- defN 23-Aug-05 06:14 xsl/localizations/it-IT.xml
+-rw-r--r--  2.0 unx    16085 b- defN 23-Aug-05 06:14 xsl/localizations/hu-HU.xml
+-rw-r--r--  2.0 unx    16500 b- defN 23-Aug-05 06:14 xsl/localizations/fr-CA.xml
+-rw-r--r--  2.0 unx     5135 b- defN 23-Aug-05 06:14 xsl/latex/pretext-latex-guide.xsl
+-rw-r--r--  2.0 unx     2261 b- defN 23-Aug-05 06:14 xsl/latex/pretext-latex-AIM.xsl
+-rw-r--r--  2.0 unx    14482 b- defN 23-Aug-05 06:14 xsl/latex/pretext-latex-chaos.xsl
+-rw-r--r--  2.0 unx     7526 b- defN 23-Aug-05 06:14 xsl/latex/pretext-latex-CLP.xsl
+-rw-r--r--  2.0 unx     3024 b- defN 23-Aug-05 06:14 xsl/latex/pretext-latex-dyslexic-font.xsl
 142 files, 4849033 bytes uncompressed, 1027739 bytes compressed:  78.8%
```

### Comparing `pretext-1.7.5.dev20230804/pretext/generate.py` & `pretext-1.7.5.dev20230805/pretext/generate.py`

 * *Files identical despite different names*

### Comparing `pretext-1.7.5.dev20230804/pretext/project/__init__.py` & `pretext-1.7.5.dev20230805/pretext/project/__init__.py`

 * *Files identical despite different names*

### Comparing `pretext-1.7.5.dev20230804/pretext/project/refactor.py` & `pretext-1.7.5.dev20230805/pretext/project/refactor.py`

 * *Files identical despite different names*

### Comparing `pretext-1.7.5.dev20230804/pretext/project/xml.py` & `pretext-1.7.5.dev20230805/pretext/project/xml.py`

 * *Files identical despite different names*

### Comparing `pretext-1.7.5.dev20230804/pretext/templates/__init__.py` & `pretext-1.7.5.dev20230805/pretext/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `pretext-1.7.5.dev20230804/pretext/templates/resources/.devcontainer.json` & `pretext-1.7.5.dev20230805/pretext/templates/resources/.devcontainer.json`

 * *Files identical despite different names*

### Comparing `pretext-1.7.5.dev20230804/pretext/templates/resources/.gitignore` & `pretext-1.7.5.dev20230805/pretext/templates/resources/.gitignore`

 * *Files identical despite different names*

### Comparing `pretext-1.7.5.dev20230804/pretext/templates/resources/article.zip` & `pretext-1.7.5.dev20230805/pretext/templates/resources/article.zip`

 * *Files 4% similar despite different names*

#### zipinfo {}

```diff
@@ -1,14 +1,14 @@
 Zip file size: 158949 bytes, number of entries: 12
-drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-04 06:16 assets/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-04 06:16 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-04 06:16 source/
--rw-r--r--  2.0 unx     1676 b- defN 23-Aug-04 06:16 .gitignore
--rw-r--r--  2.0 unx     1710 b- defN 23-Aug-04 06:16 project.ptx
--rw-r--r--  2.0 unx     2538 b- defN 23-Aug-04 06:16 codechat_config.yaml
--rw-r--r--  2.0 unx       86 b- defN 23-Aug-04 06:16 README.md
--rw-r--r--  2.0 unx      449 b- defN 23-Aug-04 06:16 source/section-1.ptx
--rw-r--r--  2.0 unx      982 b- defN 23-Aug-04 06:16 source/section-2.ptx
--rw-r--r--  2.0 unx      430 b- defN 23-Aug-04 06:16 source/main.ptx
--rw-r--r--  2.0 unx   154806 b- defN 23-Aug-04 06:16 assets/frog.jpg
--rw-r--r--  2.0 unx      242 b- defN 23-Aug-04 06:16 publication/publication.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-05 06:13 assets/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-05 06:13 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-05 06:13 source/
+-rw-r--r--  2.0 unx     1676 b- defN 23-Aug-05 06:14 .gitignore
+-rw-r--r--  2.0 unx     1710 b- defN 23-Aug-05 06:14 project.ptx
+-rw-r--r--  2.0 unx     2538 b- defN 23-Aug-05 06:14 codechat_config.yaml
+-rw-r--r--  2.0 unx       86 b- defN 23-Aug-05 06:13 README.md
+-rw-r--r--  2.0 unx      449 b- defN 23-Aug-05 06:13 source/section-1.ptx
+-rw-r--r--  2.0 unx      982 b- defN 23-Aug-05 06:13 source/section-2.ptx
+-rw-r--r--  2.0 unx      430 b- defN 23-Aug-05 06:13 source/main.ptx
+-rw-r--r--  2.0 unx   154806 b- defN 23-Aug-05 06:13 assets/frog.jpg
+-rw-r--r--  2.0 unx      242 b- defN 23-Aug-05 06:13 publication/publication.ptx
 12 files, 162919 bytes uncompressed, 157669 bytes compressed:  3.2%
```

### Comparing `pretext-1.7.5.dev20230804/pretext/templates/resources/book.zip` & `pretext-1.7.5.dev20230805/pretext/templates/resources/book.zip`

 * *Files 8% similar despite different names*

#### zipinfo {}

```diff
@@ -1,10 +1,10 @@
 Zip file size: 6455 bytes, number of entries: 8
-drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-04 06:16 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-04 06:16 source/
--rw-r--r--  2.0 unx     1676 b- defN 23-Aug-04 06:16 .gitignore
--rw-r--r--  2.0 unx     1710 b- defN 23-Aug-04 06:16 project.ptx
--rw-r--r--  2.0 unx     2538 b- defN 23-Aug-04 06:16 codechat_config.yaml
--rw-r--r--  2.0 unx       82 b- defN 23-Aug-04 06:16 README.md
--rw-r--r--  2.0 unx     1767 b- defN 23-Aug-04 06:16 source/main.ptx
--rw-r--r--  2.0 unx     6114 b- defN 23-Aug-04 06:16 publication/publication.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-05 06:13 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-05 06:13 source/
+-rw-r--r--  2.0 unx     1676 b- defN 23-Aug-05 06:14 .gitignore
+-rw-r--r--  2.0 unx     1710 b- defN 23-Aug-05 06:14 project.ptx
+-rw-r--r--  2.0 unx     2538 b- defN 23-Aug-05 06:14 codechat_config.yaml
+-rw-r--r--  2.0 unx       82 b- defN 23-Aug-05 06:13 README.md
+-rw-r--r--  2.0 unx     1767 b- defN 23-Aug-05 06:13 source/main.ptx
+-rw-r--r--  2.0 unx     6114 b- defN 23-Aug-05 06:13 publication/publication.ptx
 8 files, 13887 bytes uncompressed, 5603 bytes compressed:  59.7%
```

### Comparing `pretext-1.7.5.dev20230804/pretext/templates/resources/demo.zip` & `pretext-1.7.5.dev20230805/pretext/templates/resources/demo.zip`

 * *Files 10% similar despite different names*

#### zipinfo {}

```diff
@@ -1,35 +1,35 @@
 Zip file size: 172278 bytes, number of entries: 33
-drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-04 06:16 assets/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-04 06:16 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-04 06:16 source/
--rw-r--r--  2.0 unx     1676 b- defN 23-Aug-04 06:16 .gitignore
--rw-r--r--  2.0 unx     1710 b- defN 23-Aug-04 06:16 project.ptx
--rw-r--r--  2.0 unx     2538 b- defN 23-Aug-04 06:16 codechat_config.yaml
--rw-r--r--  2.0 unx       82 b- defN 23-Aug-04 06:16 README.md
-drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-04 06:16 source/images/
--rw-r--r--  2.0 unx      339 b- defN 23-Aug-04 06:16 source/ch-features.ptx
--rw-r--r--  2.0 unx     1697 b- defN 23-Aug-04 06:16 source/sec-first-examples.ptx
--rw-r--r--  2.0 unx      375 b- defN 23-Aug-04 06:16 source/fig-sage2d.ptx
--rw-r--r--  2.0 unx      885 b- defN 23-Aug-04 06:16 source/backmatter.ptx
--rw-r--r--  2.0 unx      867 b- defN 23-Aug-04 06:16 source/sec-features.ptx
--rw-r--r--  2.0 unx     2295 b- defN 23-Aug-04 06:16 source/ch-generate.ptx
--rw-r--r--  2.0 unx      335 b- defN 23-Aug-04 06:16 source/fig-asymptote.ptx
--rw-r--r--  2.0 unx     2080 b- defN 23-Aug-04 06:16 source/frontmatter.ptx
--rw-r--r--  2.0 unx      381 b- defN 23-Aug-04 06:16 source/fig-tikz.ptx
--rw-r--r--  2.0 unx      230 b- defN 23-Aug-04 06:16 source/ch-empty.ptx
--rw-r--r--  2.0 unx      847 b- defN 23-Aug-04 06:16 source/sec-first-intro.ptx
--rw-r--r--  2.0 unx     1515 b- defN 23-Aug-04 06:16 source/ex-first.ptx
--rw-r--r--  2.0 unx      777 b- defN 23-Aug-04 06:16 source/ww.ptx
--rw-r--r--  2.0 unx      411 b- defN 23-Aug-04 06:16 source/fig-sage3d.ptx
--rw-r--r--  2.0 unx     1115 b- defN 23-Aug-04 06:16 source/ch-first with spaces.ptx
--rw-r--r--  2.0 unx     1616 b- defN 23-Aug-04 06:16 source/docinfo.ptx
--rw-r--r--  2.0 unx     2428 b- defN 23-Aug-04 06:16 source/main.ptx
--rw-r--r--  2.0 unx      835 b- defN 23-Aug-04 06:16 source/images/cflag.asy
--rw-r--r--  2.0 unx       93 b- defN 23-Aug-04 06:16 source/images/sageplot3d.sage
--rw-r--r--  2.0 unx      357 b- defN 23-Aug-04 06:16 source/images/tikz.tex
--rw-r--r--  2.0 unx       10 b- defN 23-Aug-04 06:16 source/images/sageplot2d.sage
-drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-04 06:16 assets/jsxgraph/
--rw-r--r--  2.0 unx   154806 b- defN 23-Aug-04 06:16 assets/frog.jpg
--rw-r--r--  2.0 unx     1737 b- defN 23-Aug-04 06:16 assets/jsxgraph/infinity.js
--rw-r--r--  2.0 unx     6092 b- defN 23-Aug-04 06:16 publication/publication.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-05 06:13 assets/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-05 06:13 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-05 06:13 source/
+-rw-r--r--  2.0 unx     1676 b- defN 23-Aug-05 06:14 .gitignore
+-rw-r--r--  2.0 unx     1710 b- defN 23-Aug-05 06:14 project.ptx
+-rw-r--r--  2.0 unx     2538 b- defN 23-Aug-05 06:14 codechat_config.yaml
+-rw-r--r--  2.0 unx       82 b- defN 23-Aug-05 06:13 README.md
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-05 06:13 source/images/
+-rw-r--r--  2.0 unx      339 b- defN 23-Aug-05 06:13 source/ch-features.ptx
+-rw-r--r--  2.0 unx     1697 b- defN 23-Aug-05 06:13 source/sec-first-examples.ptx
+-rw-r--r--  2.0 unx      375 b- defN 23-Aug-05 06:13 source/fig-sage2d.ptx
+-rw-r--r--  2.0 unx      885 b- defN 23-Aug-05 06:13 source/backmatter.ptx
+-rw-r--r--  2.0 unx      867 b- defN 23-Aug-05 06:13 source/sec-features.ptx
+-rw-r--r--  2.0 unx     2295 b- defN 23-Aug-05 06:13 source/ch-generate.ptx
+-rw-r--r--  2.0 unx      335 b- defN 23-Aug-05 06:13 source/fig-asymptote.ptx
+-rw-r--r--  2.0 unx     2080 b- defN 23-Aug-05 06:13 source/frontmatter.ptx
+-rw-r--r--  2.0 unx      381 b- defN 23-Aug-05 06:13 source/fig-tikz.ptx
+-rw-r--r--  2.0 unx      230 b- defN 23-Aug-05 06:13 source/ch-empty.ptx
+-rw-r--r--  2.0 unx      847 b- defN 23-Aug-05 06:13 source/sec-first-intro.ptx
+-rw-r--r--  2.0 unx     1515 b- defN 23-Aug-05 06:13 source/ex-first.ptx
+-rw-r--r--  2.0 unx      777 b- defN 23-Aug-05 06:13 source/ww.ptx
+-rw-r--r--  2.0 unx      411 b- defN 23-Aug-05 06:13 source/fig-sage3d.ptx
+-rw-r--r--  2.0 unx     1115 b- defN 23-Aug-05 06:13 source/ch-first with spaces.ptx
+-rw-r--r--  2.0 unx     1616 b- defN 23-Aug-05 06:13 source/docinfo.ptx
+-rw-r--r--  2.0 unx     2428 b- defN 23-Aug-05 06:13 source/main.ptx
+-rw-r--r--  2.0 unx      835 b- defN 23-Aug-05 06:13 source/images/cflag.asy
+-rw-r--r--  2.0 unx       93 b- defN 23-Aug-05 06:13 source/images/sageplot3d.sage
+-rw-r--r--  2.0 unx      357 b- defN 23-Aug-05 06:13 source/images/tikz.tex
+-rw-r--r--  2.0 unx       10 b- defN 23-Aug-05 06:13 source/images/sageplot2d.sage
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-05 06:13 assets/jsxgraph/
+-rw-r--r--  2.0 unx   154806 b- defN 23-Aug-05 06:13 assets/frog.jpg
+-rw-r--r--  2.0 unx     1737 b- defN 23-Aug-05 06:13 assets/jsxgraph/infinity.js
+-rw-r--r--  2.0 unx     6092 b- defN 23-Aug-05 06:13 publication/publication.ptx
 33 files, 188129 bytes uncompressed, 168462 bytes compressed:  10.5%
```

### Comparing `pretext-1.7.5.dev20230804/pretext/templates/resources/hello.zip` & `pretext-1.7.5.dev20230805/pretext/templates/resources/hello.zip`

 * *Files 18% similar despite different names*

#### zipinfo {}

```diff
@@ -1,10 +1,10 @@
 Zip file size: 3496 bytes, number of entries: 8
-drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-04 06:16 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-04 06:16 source/
--rw-r--r--  2.0 unx     1676 b- defN 23-Aug-04 06:16 .gitignore
--rw-r--r--  2.0 unx     1217 b- defN 23-Aug-04 06:16 project.ptx
--rw-r--r--  2.0 unx     2538 b- defN 23-Aug-04 06:16 codechat_config.yaml
--rw-r--r--  2.0 unx       69 b- defN 23-Aug-04 06:16 README.md
--rw-r--r--  2.0 unx      156 b- defN 23-Aug-04 06:16 source/main.ptx
--rw-r--r--  2.0 unx      242 b- defN 23-Aug-04 06:16 publication/publication.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-05 06:13 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-05 06:13 source/
+-rw-r--r--  2.0 unx     1676 b- defN 23-Aug-05 06:14 .gitignore
+-rw-r--r--  2.0 unx     1217 b- defN 23-Aug-05 06:13 project.ptx
+-rw-r--r--  2.0 unx     2538 b- defN 23-Aug-05 06:14 codechat_config.yaml
+-rw-r--r--  2.0 unx       69 b- defN 23-Aug-05 06:13 README.md
+-rw-r--r--  2.0 unx      156 b- defN 23-Aug-05 06:13 source/main.ptx
+-rw-r--r--  2.0 unx      242 b- defN 23-Aug-05 06:13 publication/publication.ptx
 8 files, 5898 bytes uncompressed, 2644 bytes compressed:  55.2%
```

### Comparing `pretext-1.7.5.dev20230804/pretext/templates/resources/project.ptx` & `pretext-1.7.5.dev20230805/pretext/templates/resources/project.ptx`

 * *Files identical despite different names*

### Comparing `pretext-1.7.5.dev20230804/pretext/templates/resources/slideshow.zip` & `pretext-1.7.5.dev20230805/pretext/templates/resources/slideshow.zip`

 * *Files 10% similar despite different names*

#### zipinfo {}

```diff
@@ -1,11 +1,11 @@
 Zip file size: 7231 bytes, number of entries: 9
-drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-04 06:16 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-04 06:16 source/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-04 06:16 xsl/
--rw-r--r--  2.0 unx     1676 b- defN 23-Aug-04 06:16 .gitignore
--rw-r--r--  2.0 unx      784 b- defN 23-Aug-04 06:16 project.ptx
--rw-r--r--  2.0 unx     2538 b- defN 23-Aug-04 06:16 codechat_config.yaml
--rw-r--r--  2.0 unx    11200 b- defN 23-Aug-04 06:16 source/main.ptx
--rw-r--r--  2.0 unx     2097 b- defN 23-Aug-04 06:16 publication/publication.ptx
--rw-r--r--  2.0 unx      190 b- defN 23-Aug-04 06:16 xsl/slides.xsl
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-05 06:13 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-05 06:13 source/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-05 06:13 xsl/
+-rw-r--r--  2.0 unx     1676 b- defN 23-Aug-05 06:14 .gitignore
+-rw-r--r--  2.0 unx      784 b- defN 23-Aug-05 06:13 project.ptx
+-rw-r--r--  2.0 unx     2538 b- defN 23-Aug-05 06:14 codechat_config.yaml
+-rw-r--r--  2.0 unx    11200 b- defN 23-Aug-05 06:13 source/main.ptx
+-rw-r--r--  2.0 unx     2097 b- defN 23-Aug-05 06:13 publication/publication.ptx
+-rw-r--r--  2.0 unx      190 b- defN 23-Aug-05 06:13 xsl/slides.xsl
 9 files, 18485 bytes uncompressed, 6285 bytes compressed:  66.0%
```

### Comparing `pretext-1.7.5.dev20230804/pretext/utils.py` & `pretext-1.7.5.dev20230805/pretext/utils.py`

 * *Files identical despite different names*

### Comparing `pretext-1.7.5.dev20230804/pyproject.toml` & `pretext-1.7.5.dev20230805/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # See https://python-poetry.org/docs/dependency-specification/ to get an understanding of
 # how poetry specifies dependencies.
 #
 # Project metadata
 # ----------------
 [tool.poetry]
 name = "pretext"
-version = "1.7.5.dev20230804"
+version = "1.7.5.dev20230805"
 description = "A package to author, build, and deploy PreTeXt projects."
 readme = "README.md"
 homepage = "https://pretextbook.org"
 repository = "https://github.com/PreTeXtBook/pretext-cli"
 authors = ["Oscar Levin <oscar.levin@unco.edu>", "Steven Clontz <steven.clontz@gmail.com>",]
 license = "GPL-3.0-or-later"
 include = [
```

### Comparing `pretext-1.7.5.dev20230804/PKG-INFO` & `pretext-1.7.5.dev20230805/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretext
-Version: 1.7.5.dev20230804
+Version: 1.7.5.dev20230805
 Summary: A package to author, build, and deploy PreTeXt projects.
 Home-page: https://pretextbook.org
 License: GPL-3.0-or-later
 Author: Oscar Levin
 Author-email: oscar.levin@unco.edu
 Requires-Python: >=3.8.5,<4.0.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

