# Comparing `tmp/hatch_ci-0.0.4.tar.gz` & `tmp/hatch_ci-0.0.4b25.tar.gz`

## Comparing `hatch_ci-0.0.4.tar` & `hatch_ci-0.0.4b25.tar`

### file list

```diff
@@ -1,43 +1,52 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 hatch_ci-0.0.4/.gitattributes
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 hatch_ci-0.0.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 hatch_ci-0.0.4/Makefile
--rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 hatch_ci-0.0.4/.github/workflows/beta.yml
--rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 hatch_ci-0.0.4/.github/workflows/master.yml
--rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 hatch_ci-0.0.4/.github/workflows/tags.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_ci-0.0.4/build/.keepme
--rw-r--r--   0        0        0    26658 2020-02-02 00:00:00.000000 hatch_ci-0.0.4/build/qa-3.8-ubuntu-latest/coverage.xml
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 hatch_ci-0.0.4/build/qa-3.8-ubuntu-latest/coverage/.gitignore
--rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 hatch_ci-0.0.4/build/qa-3.8-ubuntu-latest/coverage/coverage_html.js
--rw-r--r--   0        0        0     5106 2020-02-02 00:00:00.000000 hatch_ci-0.0.4/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943___init___py.html
--rw-r--r--   0        0        0    44736 2020-02-02 00:00:00.000000 hatch_ci-0.0.4/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_cli_py.html
--rw-r--r--   0        0        0     4935 2020-02-02 00:00:00.000000 hatch_ci-0.0.4/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_common_py.html
--rw-r--r--   0        0        0     6437 2020-02-02 00:00:00.000000 hatch_ci-0.0.4/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_hooks_py.html
--rw-r--r--   0        0        0    85102 2020-02-02 00:00:00.000000 hatch_ci-0.0.4/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_scm_py.html
--rw-r--r--   0        0        0    49436 2020-02-02 00:00:00.000000 hatch_ci-0.0.4/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_script_py.html
--rw-r--r--   0        0        0   115699 2020-02-02 00:00:00.000000 hatch_ci-0.0.4/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_tools_py.html
--rw-r--r--   0        0        0    22221 2020-02-02 00:00:00.000000 hatch_ci-0.0.4/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_version_hook_py.html
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 hatch_ci-0.0.4/build/qa-3.8-ubuntu-latest/coverage/favicon_32.png
--rw-r--r--   0        0        0     6823 2020-02-02 00:00:00.000000 hatch_ci-0.0.4/build/qa-3.8-ubuntu-latest/coverage/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 hatch_ci-0.0.4/build/qa-3.8-ubuntu-latest/coverage/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 hatch_ci-0.0.4/build/qa-3.8-ubuntu-latest/coverage/keybd_open.png
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 hatch_ci-0.0.4/build/qa-3.8-ubuntu-latest/coverage/status.json
--rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 hatch_ci-0.0.4/build/qa-3.8-ubuntu-latest/coverage/style.css
--rw-r--r--   0        0        0    20682 2020-02-02 00:00:00.000000 hatch_ci-0.0.4/build/qa-3.8-ubuntu-latest/junit/junit.html
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 hatch_ci-0.0.4/build/qa-3.8-ubuntu-latest/junit/junit.xml
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 hatch_ci-0.0.4/src/hatch_ci/__init__.py
--rw-r--r--   0        0        0     4098 2020-02-02 00:00:00.000000 hatch_ci-0.0.4/src/hatch_ci/cli.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 hatch_ci-0.0.4/src/hatch_ci/common.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 hatch_ci-0.0.4/src/hatch_ci/hooks.py
--rw-r--r--   0        0        0     7610 2020-02-02 00:00:00.000000 hatch_ci-0.0.4/src/hatch_ci/scm.py
--rw-r--r--   0        0        0     5412 2020-02-02 00:00:00.000000 hatch_ci-0.0.4/src/hatch_ci/script.py
--rw-r--r--   0        0        0    11708 2020-02-02 00:00:00.000000 hatch_ci-0.0.4/src/hatch_ci/tools.py
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 hatch_ci-0.0.4/src/hatch_ci/version_hook.py
--rw-r--r--   0        0        0     6761 2020-02-02 00:00:00.000000 hatch_ci-0.0.4/tests/conftest.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 hatch_ci-0.0.4/tests/requirements.txt
--rw-r--r--   0        0        0     3624 2020-02-02 00:00:00.000000 hatch_ci-0.0.4/tests/test_scm.py
--rw-r--r--   0        0        0    11077 2020-02-02 00:00:00.000000 hatch_ci-0.0.4/tests/test_tools.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 hatch_ci-0.0.4/.gitignore
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 hatch_ci-0.0.4/LICENSE.txt
--rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 hatch_ci-0.0.4/README.md
--rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 hatch_ci-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     3788 2020-02-02 00:00:00.000000 hatch_ci-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 hatch_ci-0.0.4b25/.gitattributes
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 hatch_ci-0.0.4b25/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 hatch_ci-0.0.4b25/Makefile
+-rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 hatch_ci-0.0.4b25/.github/workflows/beta.yml
+-rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 hatch_ci-0.0.4b25/.github/workflows/master.yml
+-rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 hatch_ci-0.0.4b25/.github/workflows/tags.yml
+-rw-r--r--   0        0        0    26658 2020-02-02 00:00:00.000000 hatch_ci-0.0.4b25/build/qa-3.9-ubuntu-latest/coverage.xml
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 hatch_ci-0.0.4b25/build/qa-3.9-ubuntu-latest/coverage/.gitignore
+-rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 hatch_ci-0.0.4b25/build/qa-3.9-ubuntu-latest/coverage/coverage_html.js
+-rw-r--r--   0        0        0     5106 2020-02-02 00:00:00.000000 hatch_ci-0.0.4b25/build/qa-3.9-ubuntu-latest/coverage/d_7005a4ce5d73f943___init___py.html
+-rw-r--r--   0        0        0    44736 2020-02-02 00:00:00.000000 hatch_ci-0.0.4b25/build/qa-3.9-ubuntu-latest/coverage/d_7005a4ce5d73f943_cli_py.html
+-rw-r--r--   0        0        0     4935 2020-02-02 00:00:00.000000 hatch_ci-0.0.4b25/build/qa-3.9-ubuntu-latest/coverage/d_7005a4ce5d73f943_common_py.html
+-rw-r--r--   0        0        0     6437 2020-02-02 00:00:00.000000 hatch_ci-0.0.4b25/build/qa-3.9-ubuntu-latest/coverage/d_7005a4ce5d73f943_hooks_py.html
+-rw-r--r--   0        0        0    85102 2020-02-02 00:00:00.000000 hatch_ci-0.0.4b25/build/qa-3.9-ubuntu-latest/coverage/d_7005a4ce5d73f943_scm_py.html
+-rw-r--r--   0        0        0    49436 2020-02-02 00:00:00.000000 hatch_ci-0.0.4b25/build/qa-3.9-ubuntu-latest/coverage/d_7005a4ce5d73f943_script_py.html
+-rw-r--r--   0        0        0   115699 2020-02-02 00:00:00.000000 hatch_ci-0.0.4b25/build/qa-3.9-ubuntu-latest/coverage/d_7005a4ce5d73f943_tools_py.html
+-rw-r--r--   0        0        0    22221 2020-02-02 00:00:00.000000 hatch_ci-0.0.4b25/build/qa-3.9-ubuntu-latest/coverage/d_7005a4ce5d73f943_version_hook_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 hatch_ci-0.0.4b25/build/qa-3.9-ubuntu-latest/coverage/favicon_32.png
+-rw-r--r--   0        0        0     6823 2020-02-02 00:00:00.000000 hatch_ci-0.0.4b25/build/qa-3.9-ubuntu-latest/coverage/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 hatch_ci-0.0.4b25/build/qa-3.9-ubuntu-latest/coverage/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 hatch_ci-0.0.4b25/build/qa-3.9-ubuntu-latest/coverage/keybd_open.png
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 hatch_ci-0.0.4b25/build/qa-3.9-ubuntu-latest/coverage/status.json
+-rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 hatch_ci-0.0.4b25/build/qa-3.9-ubuntu-latest/coverage/style.css
+-rw-r--r--   0        0        0    20682 2020-02-02 00:00:00.000000 hatch_ci-0.0.4b25/build/qa-3.9-ubuntu-latest/junit/junit.html
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 hatch_ci-0.0.4b25/build/qa-3.9-ubuntu-latest/junit/junit.xml
+-rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 hatch_ci-0.0.4b25/build/qa-3.9-ubuntu-latest/mypy/index.html
+-rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 hatch_ci-0.0.4b25/build/qa-3.9-ubuntu-latest/mypy/mypy-html.css
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 hatch_ci-0.0.4b25/build/qa-3.9-ubuntu-latest/mypy/html/src/hatch_ci/__init__.py.html
+-rw-r--r--   0        0        0    23800 2020-02-02 00:00:00.000000 hatch_ci-0.0.4b25/build/qa-3.9-ubuntu-latest/mypy/html/src/hatch_ci/cli.py.html
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 hatch_ci-0.0.4b25/build/qa-3.9-ubuntu-latest/mypy/html/src/hatch_ci/common.py.html
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 hatch_ci-0.0.4b25/build/qa-3.9-ubuntu-latest/mypy/html/src/hatch_ci/hooks.py.html
+-rw-r--r--   0        0        0    45457 2020-02-02 00:00:00.000000 hatch_ci-0.0.4b25/build/qa-3.9-ubuntu-latest/mypy/html/src/hatch_ci/scm.py.html
+-rw-r--r--   0        0        0    30321 2020-02-02 00:00:00.000000 hatch_ci-0.0.4b25/build/qa-3.9-ubuntu-latest/mypy/html/src/hatch_ci/script.py.html
+-rw-r--r--   0        0        0    68104 2020-02-02 00:00:00.000000 hatch_ci-0.0.4b25/build/qa-3.9-ubuntu-latest/mypy/html/src/hatch_ci/tools.py.html
+-rw-r--r--   0        0        0    10884 2020-02-02 00:00:00.000000 hatch_ci-0.0.4b25/build/qa-3.9-ubuntu-latest/mypy/html/src/hatch_ci/version_hook.py.html
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 hatch_ci-0.0.4b25/src/hatch_ci/__init__.py
+-rw-r--r--   0        0        0     4098 2020-02-02 00:00:00.000000 hatch_ci-0.0.4b25/src/hatch_ci/cli.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 hatch_ci-0.0.4b25/src/hatch_ci/common.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 hatch_ci-0.0.4b25/src/hatch_ci/hooks.py
+-rw-r--r--   0        0        0     7610 2020-02-02 00:00:00.000000 hatch_ci-0.0.4b25/src/hatch_ci/scm.py
+-rw-r--r--   0        0        0     5412 2020-02-02 00:00:00.000000 hatch_ci-0.0.4b25/src/hatch_ci/script.py
+-rw-r--r--   0        0        0    11708 2020-02-02 00:00:00.000000 hatch_ci-0.0.4b25/src/hatch_ci/tools.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 hatch_ci-0.0.4b25/src/hatch_ci/version_hook.py
+-rw-r--r--   0        0        0     6761 2020-02-02 00:00:00.000000 hatch_ci-0.0.4b25/tests/conftest.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 hatch_ci-0.0.4b25/tests/requirements.txt
+-rw-r--r--   0        0        0     3624 2020-02-02 00:00:00.000000 hatch_ci-0.0.4b25/tests/test_scm.py
+-rw-r--r--   0        0        0    11077 2020-02-02 00:00:00.000000 hatch_ci-0.0.4b25/tests/test_tools.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 hatch_ci-0.0.4b25/.gitignore
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 hatch_ci-0.0.4b25/LICENSE.txt
+-rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 hatch_ci-0.0.4b25/README.md
+-rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 hatch_ci-0.0.4b25/pyproject.toml
+-rw-r--r--   0        0        0     3791 2020-02-02 00:00:00.000000 hatch_ci-0.0.4b25/PKG-INFO
```

### Comparing `hatch_ci-0.0.4/.github/workflows/beta.yml` & `hatch_ci-0.0.4b25/.github/workflows/beta.yml`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.4/.github/workflows/master.yml` & `hatch_ci-0.0.4b25/.github/workflows/master.yml`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.4/.github/workflows/tags.yml` & `hatch_ci-0.0.4b25/.github/workflows/tags.yml`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.4/build/qa-3.8-ubuntu-latest/coverage.xml` & `hatch_ci-0.0.4b25/build/qa-3.9-ubuntu-latest/coverage.xml`

 * *Files 0% similar despite different names*

#### Comparing `hatch_ci-0.0.4/build/qa-3.8-ubuntu-latest/coverage.xml` & `hatch_ci-0.0.4b25/build/qa-3.9-ubuntu-latest/coverage.xml`

```diff
@@ -1,9 +1,9 @@
 <?xml version="1.0" encoding="utf-8"?>
-<coverage version="7.2.7" timestamp="1691349792531" lines-valid="548" lines-covered="328" line-rate="0.5985" branches-valid="186" branches-covered="112" branch-rate="0.6022" complexity="0">
+<coverage version="7.2.7" timestamp="1691349508863" lines-valid="548" lines-covered="328" line-rate="0.5985" branches-valid="186" branches-covered="112" branch-rate="0.6022" complexity="0">
   <!-- Generated by coverage.py: https://coverage.readthedocs.io/en/7.2.7 -->
   <!-- Based on https://raw.githubusercontent.com/cobertura/web/master/htdocs/xml/coverage-04.dtd -->
   <sources>
     <source>/home/runner/work/hatch-ci/hatch-ci</source>
   </sources>
   <packages>
     <package name="src.hatch_ci" line-rate="0.5985" branch-rate="0.6022" complexity="0">
```

### Comparing `hatch_ci-0.0.4/build/qa-3.8-ubuntu-latest/coverage/coverage_html.js` & `hatch_ci-0.0.4b25/build/qa-3.9-ubuntu-latest/coverage/coverage_html.js`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.4/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943___init___py.html` & `hatch_ci-0.0.4b25/build/qa-3.9-ubuntu-latest/coverage/d_7005a4ce5d73f943___init___py.html`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_cli_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-06 19:23 +0000
+            created at 2023-08-06 19:18 +0000
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -89,13 +89,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_cli_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-06 19:23 +0000
+            created at 2023-08-06 19:18 +0000
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ***** 2 statements   2 run 0 missing 0 excluded 0 partial *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-06 19:23 +0000
+at 2023-08-06 19:18 +0000
 
 
 1__version__ = "0.0.4" 
 2__hash__ = "" 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-06 19:23 +0000
+at 2023-08-06 19:18 +0000
```

### Comparing `hatch_ci-0.0.4/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_cli_py.html` & `hatch_ci-0.0.4b25/build/qa-3.9-ubuntu-latest/coverage/d_7005a4ce5d73f943_cli_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_common_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-06 19:23 +0000
+            created at 2023-08-06 19:18 +0000
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -223,13 +223,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_common_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-06 19:23 +0000
+            created at 2023-08-06 19:18 +0000
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ***** 72 statements   0 run 72 missing 0 excluded 0 partial *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-06 19:23 +0000
+at 2023-08-06 19:18 +0000
 
 
 1from __future__ import annotations 
 2 
 3import argparse 
 4import functools 
 5import logging 
@@ -151,8 +151,8 @@
 132 raise 
 133 
 134 return _fn1 
 135 
 136 return _fn 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-06 19:23 +0000
+at 2023-08-06 19:18 +0000
```

### Comparing `hatch_ci-0.0.4/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_common_py.html` & `hatch_ci-0.0.4b25/build/qa-3.9-ubuntu-latest/coverage/d_7005a4ce5d73f943_common_py.html`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_cli_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_hooks_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-06 19:23 +0000
+            created at 2023-08-06 19:18 +0000
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -88,13 +88,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_cli_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_hooks_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-06 19:23 +0000
+            created at 2023-08-06 19:18 +0000
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,14 +7,14 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ***** 1 statements   0 run 1 missing 0 excluded 0 partial *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-06 19:23 +0000
+at 2023-08-06 19:18 +0000
 
 
 1PLUGIN_NAME = "ci" 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-06 19:23 +0000
+at 2023-08-06 19:18 +0000
```

### Comparing `hatch_ci-0.0.4/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_hooks_py.html` & `hatch_ci-0.0.4b25/build/qa-3.9-ubuntu-latest/coverage/d_7005a4ce5d73f943_hooks_py.html`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_common_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_scm_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-06 19:23 +0000
+            created at 2023-08-06 19:18 +0000
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -95,13 +95,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_common_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_scm_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-06 19:23 +0000
+            created at 2023-08-06 19:18 +0000
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,21 +7,21 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ***** 5 statements   0 run 5 missing 0 excluded 0 partial *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-06 19:23 +0000
+at 2023-08-06 19:18 +0000
 
 
 1from hatchling.plugin import hookimpl 
 2 
 3from hatch_ci.version_hook import CIVersionSource 
 4 
 5 
 6@hookimpl 
 7def hatch_register_version_source(): 
 8 return CIVersionSource 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-06 19:23 +0000
+at 2023-08-06 19:18 +0000
```

### Comparing `hatch_ci-0.0.4/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_scm_py.html` & `hatch_ci-0.0.4b25/build/qa-3.9-ubuntu-latest/coverage/d_7005a4ce5d73f943_scm_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_hooks_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_script_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-06 19:23 +0000
+            created at 2023-08-06 19:18 +0000
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -353,13 +353,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_hooks_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_script_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-06 19:23 +0000
+            created at 2023-08-06 19:18 +0000
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ***** 162 statements   135 run 27 missing 0 excluded 8 partial *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-06 19:23 +0000
+at 2023-08-06 19:18 +0000
 
 
 1# see https://pypi.org/project/setuptools-github 
 2# copy of setuptools_github.scm 
 3from __future__ import annotations 
 4 
 5import dataclasses as dc 
@@ -287,8 +287,8 @@
 263 if str(cur) == cur.root: 263&#x202F;&#x219B;&#x202F;264line 263 didn't jump
 to line 264, because the condition on line 263 was never true
 264 break 
 265 cur = cur.parent 
 266 return None 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-06 19:23 +0000
+at 2023-08-06 19:18 +0000
```

### Comparing `hatch_ci-0.0.4/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_script_py.html` & `hatch_ci-0.0.4b25/build/qa-3.9-ubuntu-latest/coverage/d_7005a4ce5d73f943_script_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_scm_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_tools_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-06 19:23 +0000
+            created at 2023-08-06 19:18 +0000
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -258,13 +258,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_scm_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_tools_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-06 19:23 +0000
+            created at 2023-08-06 19:18 +0000
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ***** 67 statements   0 run 67 missing 2 excluded 0 partial *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-06 19:23 +0000
+at 2023-08-06 19:18 +0000
 
 
 1"""create a beta branch or release a beta branch 
 2 
 3This script will either create a new beta branch: 
 4 
 5 hatch-ci make-beta ./src/package_name/__init__.py 
@@ -188,8 +188,8 @@
 167 raise RuntimeError(f"unsupported mode {options.mode=}") 
 168 
 169 
 170if __name__ == "__main__": 
 171 main() 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-06 19:23 +0000
+at 2023-08-06 19:18 +0000
```

### Comparing `hatch_ci-0.0.4/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_tools_py.html` & `hatch_ci-0.0.4b25/build/qa-3.9-ubuntu-latest/coverage/d_7005a4ce5d73f943_tools_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_script_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_version_hook_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-06 19:23 +0000
+            created at 2023-08-06 19:18 +0000
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -478,13 +478,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_script_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_version_hook_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-06 19:23 +0000
+            created at 2023-08-06 19:18 +0000
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ***** 201 statements   191 run 10 missing 0 excluded 8 partial *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-06 19:23 +0000
+at 2023-08-06 19:18 +0000
 
 
 1# see https://pypi.org/project/setuptools-github 
 2# copy of setuptools_github.tools 
 3from __future__ import annotations 
 4 
 5import ast 
@@ -418,8 +418,8 @@
 387 for path in list_of_paths(paths): 
 388 txt = apply_fixers(path.read_text(), fixers) 
 389 tmpl = env.from_string(txt) 
 390 path.write_text(tmpl.render(ctx=Context(**data))) 
 391 return data 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-06 19:23 +0000
+at 2023-08-06 19:18 +0000
```

### Comparing `hatch_ci-0.0.4/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_version_hook_py.html` & `hatch_ci-0.0.4b25/build/qa-3.9-ubuntu-latest/coverage/d_7005a4ce5d73f943_version_hook_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_tools_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="index.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-06 19:23 +0000
+            created at 2023-08-06 19:18 +0000
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -148,13 +148,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_tools_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="index.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-06 19:23 +0000
+            created at 2023-08-06 19:18 +0000
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ***** 38 statements   0 run 38 missing 0 excluded 0 partial *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-06 19:23 +0000
+at 2023-08-06 19:18 +0000
 
 
 1from __future__ import annotations 
 2 
 3from typing import Any 
 4 
 5from hatchling.version.source.plugin.interface import VersionSourceInterface 
@@ -73,8 +73,8 @@
 57 ) 
 58 gdata = tools.process( 
 59 version_file, getenv("GITHUB_DUMP"), paths=paths, fixers=fixers 
 60 ) 
 61 return {"version": gdata["version"]} 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-06 19:23 +0000
+at 2023-08-06 19:18 +0000
```

### Comparing `hatch_ci-0.0.4/build/qa-3.8-ubuntu-latest/coverage/favicon_32.png` & `hatch_ci-0.0.4b25/build/qa-3.9-ubuntu-latest/coverage/favicon_32.png`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.4/build/qa-3.8-ubuntu-latest/coverage/index.html` & `hatch_ci-0.0.4b25/build/qa-3.9-ubuntu-latest/coverage/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
             </div>
         </aside>
         <form id="filter_container">
             <input id="filter" type="text" value="" placeholder="filter..." />
         </form>
         <p class="text">
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-06 19:23 +0000
+            created at 2023-08-06 19:18 +0000
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
@@ -154,15 +154,15 @@
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-06 19:23 +0000
+            created at 2023-08-06 19:18 +0000
         </p>
     </div>
     <aside class="hidden">
         <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_version_hook_py.html"/>
         <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943___init___py.html"/>
         <button type="button" class="button_prev_file" data-shortcut="["/>
         <button type="button" class="button_next_file" data-shortcut="]"/>
```

#### html2text {}

```diff
@@ -2,24 +2,24 @@
 ****** Coverage report: 60% ******
  ⁰  [Show/hide keyboard shortcuts]
 Shortcuts on this page
 n s m x b p c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
-coverage.py_v7.2.7, created at 2023-08-06 19:23 +0000
+coverage.py_v7.2.7, created at 2023-08-06 19:18 +0000
 
 Module                   statements missing excluded branches partial coverage
 src/hatch_ci/__init__.py 2          0       0        0        0       100%
 src/hatch_ci/cli.py      72         72      0        18       0       0%
 src/hatch_ci/common.py   1          1       0        0        0       0%
 src/hatch_ci/hooks.py    5          5       0        0        0       0%
 src/hatch_ci/scm.py      162        27      0        52       8       82%
 src/hatch_ci/script.py   67         67      2        20       0       0%
 src/hatch_ci/tools.py    201        10      0        84       8       92%
 src/hatch_ci/            38         38      0        12       0       0%
 version_hook.py
 Total                    548        220     2        186      16      60%
 No items found using the specified filter.
 
-coverage.py_v7.2.7, created at 2023-08-06 19:23 +0000
+coverage.py_v7.2.7, created at 2023-08-06 19:18 +0000
  ____
```

### Comparing `hatch_ci-0.0.4/build/qa-3.8-ubuntu-latest/coverage/keybd_closed.png` & `hatch_ci-0.0.4b25/build/qa-3.9-ubuntu-latest/coverage/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.4/build/qa-3.8-ubuntu-latest/coverage/keybd_open.png` & `hatch_ci-0.0.4b25/build/qa-3.9-ubuntu-latest/coverage/keybd_open.png`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.4/build/qa-3.8-ubuntu-latest/coverage/status.json` & `hatch_ci-0.0.4b25/build/qa-3.9-ubuntu-latest/coverage/status.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.87109375%*

 * *Differences: {"'files'": "{'d_7005a4ce5d73f943_scm_py': {'hash': '09485baef443027d4b5d7014a9e7d1aa'}, "*

 * *            "'d_7005a4ce5d73f943_tools_py': {'hash': '920e588d8d5656224648cba4f71d8359'}}",*

 * * "'globals'": "'6b5e9aeba37f83ffd189f0b2f78f14b1'"}*

```diff
@@ -65,15 +65,15 @@
                     0,
                     0
                 ],
                 "relative_filename": "src/hatch_ci/hooks.py"
             }
         },
         "d_7005a4ce5d73f943_scm_py": {
-            "hash": "b208d1663706f031c634592ef10b4313",
+            "hash": "09485baef443027d4b5d7014a9e7d1aa",
             "index": {
                 "html_filename": "d_7005a4ce5d73f943_scm_py.html",
                 "nums": [
                     0,
                     1,
                     162,
                     0,
@@ -99,15 +99,15 @@
                     0,
                     20
                 ],
                 "relative_filename": "src/hatch_ci/script.py"
             }
         },
         "d_7005a4ce5d73f943_tools_py": {
-            "hash": "18b797e8b6cd409754c438caa4341729",
+            "hash": "920e588d8d5656224648cba4f71d8359",
             "index": {
                 "html_filename": "d_7005a4ce5d73f943_tools_py.html",
                 "nums": [
                     0,
                     1,
                     201,
                     0,
@@ -134,10 +134,10 @@
                     12
                 ],
                 "relative_filename": "src/hatch_ci/version_hook.py"
             }
         }
     },
     "format": 2,
-    "globals": "ee3590caf8daf83034a51a2d83560a03",
+    "globals": "6b5e9aeba37f83ffd189f0b2f78f14b1",
     "version": "7.2.7"
 }
```

### Comparing `hatch_ci-0.0.4/build/qa-3.8-ubuntu-latest/coverage/style.css` & `hatch_ci-0.0.4b25/build/qa-3.9-ubuntu-latest/coverage/style.css`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.4/build/qa-3.8-ubuntu-latest/junit/junit.html` & `hatch_ci-0.0.4b25/build/qa-3.9-ubuntu-latest/junit/junit.html`

 * *Files 1% similar despite different names*

```diff
@@ -435,17 +435,17 @@
     const rows = findAll('.results-table-row').filter(isAllRowsHidden);
     const allRowsHidden = rows.length == 0 ? true : false;
     const notFoundMessage = document.getElementById('not-found-message');
     notFoundMessage.hidden = !allRowsHidden;
 }
 </script>
     <h1>junit.html</h1>
-    <p>Report generated on 06-Aug-2023 at 19:23:12 by <a href="https://pypi.python.org/pypi/pytest-html">pytest-html</a> v3.2.0</p>
+    <p>Report generated on 06-Aug-2023 at 19:18:28 by <a href="https://pypi.python.org/pypi/pytest-html">pytest-html</a> v3.2.0</p>
     <h2>Summary</h2>
-    <p>16 tests ran in 1.21 seconds. </p>
+    <p>16 tests ran in 1.11 seconds. </p>
     <p class="filter" hidden="true">(Un)check the boxes to filter the results.</p><input checked="true" class="filter" data-test-result="passed" hidden="true" name="filter_checkbox" onChange="filterTable(this)" type="checkbox"/><span class="passed">16 passed</span>, <input checked="true" class="filter" data-test-result="skipped" disabled="true" hidden="true" name="filter_checkbox" onChange="filterTable(this)" type="checkbox"/><span class="skipped">0 skipped</span>, <input checked="true" class="filter" data-test-result="failed" disabled="true" hidden="true" name="filter_checkbox" onChange="filterTable(this)" type="checkbox"/><span class="failed">0 failed</span>, <input checked="true" class="filter" data-test-result="error" disabled="true" hidden="true" name="filter_checkbox" onChange="filterTable(this)" type="checkbox"/><span class="error">0 errors</span>, <input checked="true" class="filter" data-test-result="xfailed" disabled="true" hidden="true" name="filter_checkbox" onChange="filterTable(this)" type="checkbox"/><span class="xfailed">0 expected failures</span>, <input checked="true" class="filter" data-test-result="xpassed" disabled="true" hidden="true" name="filter_checkbox" onChange="filterTable(this)" type="checkbox"/><span class="xpassed">0 unexpected passes</span>
     <h2>Results</h2>
     <table id="results-table">
       <thead id="results-table-head">
         <tr>
           <th class="sortable result initial-sort" col="result">Result</th>
           <th class="sortable" col="name">Test</th>
@@ -472,15 +472,15 @@
           <td class="extra" colspan="4">
             <div class="log"> ------------------------------Captured stderr call------------------------------ <br/>Switched to a new branch &#x27;beta/0.0.3&#x27;
 Switched to a new branch &#x27;beta/0.0.4&#x27;
 Switched to branch &#x27;master&#x27;
 Cloning into &#x27;/tmp/pytest-of-runner/pytest-0/test_handle_remote_and_local_r0/test_check_version-repo1&#x27;...
 done.
 Switched to a new branch &#x27;beta/0.0.2&#x27;
-Cloning into &#x27;/tmp/pytest-of-runner/pytest-0/test_handle_remote_and_local_r0/7IHSP7&#x27;...
+Cloning into &#x27;/tmp/pytest-of-runner/pytest-0/test_handle_remote_and_local_r0/R1ERD8&#x27;...
 done.
 Switched to a new branch &#x27;beta/0.0.1&#x27;
 fatal: a branch named &#x27;master&#x27; already exists
 From /tmp/pytest-of-runner/pytest-0/test_handle_remote_and_local_r0/test_check_version-repo1
  * [new branch]      beta/0.0.2 -&gt; repo1/beta/0.0.2
  * [new branch]      master     -&gt; repo1/master
 <br/></div></td></tr></tbody>
@@ -574,15 +574,15 @@
         <tr>
           <td class="extra" colspan="4">
             <div class="empty log">No log output captured.</div></td></tr></tbody>
       <tbody class="passed results-table-row">
         <tr>
           <td class="col-result">Passed</td>
           <td class="col-name">tests/test_tools.py::test_update_version_master</td>
-          <td class="col-duration">0.05</td>
+          <td class="col-duration">0.04</td>
           <td class="col-links"></td></tr>
         <tr>
           <td class="extra" colspan="4">
             <div class="empty log">No log output captured.</div></td></tr></tbody>
       <tbody class="passed results-table-row">
         <tr>
           <td class="col-result">Passed</td>
@@ -607,14 +607,14 @@
             <div class="log"> ------------------------------Captured stderr call------------------------------ <br/>Switched to a new branch &#x27;beta/0.0.3&#x27;
 Updated 1 path from the index
 <br/></div></td></tr></tbody>
       <tbody class="passed results-table-row">
         <tr>
           <td class="col-result">Passed</td>
           <td class="col-name">tests/test_tools.py::test_process</td>
-          <td class="col-duration">0.14</td>
+          <td class="col-duration">0.12</td>
           <td class="col-links"></td></tr>
         <tr>
           <td class="extra" colspan="4">
             <div class="log"> ------------------------------Captured stderr call------------------------------ <br/>Updated 1 path from the index
 Switched to a new branch &#x27;beta/1.2.3&#x27;
 <br/></div></td></tr></tbody></table></body></html>
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 ****** junit.html ******
-Report generated on 06-Aug-2023 at 19:23:12 by pytest-html v3.2.0
+Report generated on 06-Aug-2023 at 19:18:28 by pytest-html v3.2.0
 ***** Summary *****
-16 tests ran in 1.21 seconds.
+16 tests ran in 1.11 seconds.
 (Un)check the boxes to filter the results.
 *16 passed, *0 skipped, *0 failed, *0 errors, *0 expected failures, *0
 unexpected passes
 ***** Results *****
 Result Test                                                  Duration Links
 No results found. Try to check the filters
 Passed tests/test_scm.py::test_lookup                        0.03
@@ -14,15 +14,15 @@
 ------------------------------Captured stderr call--------------------------
 ----
 Switched to a new branch &#x27;beta/0.0.3&#x27; Switched to a new branch
 &#x27;beta/0.0.4&#x27; Switched to branch &#x27;master&#x27; Cloning into
 &#x27;/tmp/pytest-of-runner/pytest-0/test_handle_remote_and_local_r0/
 test_check_version-repo1&#x27;... done. Switched to a new branch &#x27;beta/
 0.0.2&#x27; Cloning into &#x27;/tmp/pytest-of-runner/pytest-0/
-test_handle_remote_and_local_r0/7IHSP7&#x27;... done. Switched to a new
+test_handle_remote_and_local_r0/R1ERD8&#x27;... done. Switched to a new
 branch &#x27;beta/0.0.1&#x27; fatal: a branch named &#x27;master&#x27;
 already exists From /tmp/pytest-of-runner/pytest-0/
 test_handle_remote_and_local_r0/test_check_version-repo1 * [new branch]
 beta/0.0.2 -> repo1/beta/0.0.2 * [new branch] master -> repo1/master
 Passed tests/test_tools.py::test_abort_exception             0.00
 No log output captured.
 Passed tests/test_tools.py::test_urmtree                     0.00
@@ -39,25 +39,25 @@
 No log output captured.
 Passed tests/test_tools.py::test_set_module_var              0.00
 No log output captured.
 Passed tests/test_tools.py::test_set_module_var_empty_file   0.00
 No log output captured.
 Passed tests/test_tools.py::test_bump_version                0.00
 No log output captured.
-Passed tests/test_tools.py::test_update_version_master       0.05
+Passed tests/test_tools.py::test_update_version_master       0.04
 No log output captured.
 Passed tests/test_tools.py::test_update_version_beta         0.11
 ------------------------------Captured stderr call--------------------------
 ----
 Switched to a new branch &#x27;beta/0.0.4&#x27; Updated 1 path from the
 index Updated 1 path from the index Switched to a new branch &#x27;beta/
 0.0.2&#x27;
 Passed tests/test_tools.py::test_update_version_release      0.06
 ------------------------------Captured stderr call--------------------------
 ----
 Switched to a new branch &#x27;beta/0.0.3&#x27; Updated 1 path from the
 index
-Passed tests/test_tools.py::test_process                     0.14
+Passed tests/test_tools.py::test_process                     0.12
 ------------------------------Captured stderr call--------------------------
 ----
 Updated 1 path from the index Switched to a new branch &#x27;beta/
 1.2.3&#x27;
```

### Comparing `hatch_ci-0.0.4/build/qa-3.8-ubuntu-latest/junit/junit.xml` & `hatch_ci-0.0.4b25/build/qa-3.9-ubuntu-latest/junit/junit.xml`

 * *Files 10% similar despite different names*

#### Comparing `hatch_ci-0.0.4/build/qa-3.8-ubuntu-latest/junit/junit.xml` & `hatch_ci-0.0.4b25/build/qa-3.9-ubuntu-latest/junit/junit.xml`

```diff
@@ -1,21 +1,21 @@
 <?xml version="1.0" encoding="utf-8"?>
 <testsuites>
-  <testsuite name="pytest" errors="0" failures="0" skipped="0" tests="16" time="1.193" timestamp="2023-08-06T19:23:11.430916" hostname="fv-az351-917">
-    <testcase classname="tests.test_scm" name="test_lookup" time="0.034"/>
-    <testcase classname="tests.test_scm" name="test_handle_remote_and_local_repos" time="0.268"/>
-    <testcase classname="tests.test_tools" name="test_abort_exception" time="0.001"/>
-    <testcase classname="tests.test_tools" name="test_urmtree" time="0.002"/>
+  <testsuite name="pytest" errors="0" failures="0" skipped="0" tests="16" time="1.106" timestamp="2023-08-06T19:18:27.843262" hostname="fv-az792-750">
+    <testcase classname="tests.test_scm" name="test_lookup" time="0.032"/>
+    <testcase classname="tests.test_scm" name="test_handle_remote_and_local_repos" time="0.262"/>
+    <testcase classname="tests.test_tools" name="test_abort_exception" time="0.002"/>
+    <testcase classname="tests.test_tools" name="test_urmtree" time="0.001"/>
     <testcase classname="tests.test_tools" name="test_indent" time="0.001"/>
     <testcase classname="tests.test_tools" name="test_list_of_paths" time="0.001"/>
     <testcase classname="tests.test_tools" name="test_lstrip" time="0.001"/>
-    <testcase classname="tests.test_tools" name="test_apply_fixers" time="0.004"/>
+    <testcase classname="tests.test_tools" name="test_apply_fixers" time="0.003"/>
     <testcase classname="tests.test_tools" name="test_get_module_var" time="0.003"/>
-    <testcase classname="tests.test_tools" name="test_set_module_var" time="0.004"/>
+    <testcase classname="tests.test_tools" name="test_set_module_var" time="0.003"/>
     <testcase classname="tests.test_tools" name="test_set_module_var_empty_file" time="0.002"/>
     <testcase classname="tests.test_tools" name="test_bump_version" time="0.001"/>
-    <testcase classname="tests.test_tools" name="test_update_version_master" time="0.053"/>
-    <testcase classname="tests.test_tools" name="test_update_version_beta" time="0.115"/>
-    <testcase classname="tests.test_tools" name="test_update_version_release" time="0.067"/>
-    <testcase classname="tests.test_tools" name="test_process" time="0.143"/>
+    <testcase classname="tests.test_tools" name="test_update_version_master" time="0.050"/>
+    <testcase classname="tests.test_tools" name="test_update_version_beta" time="0.111"/>
+    <testcase classname="tests.test_tools" name="test_update_version_release" time="0.065"/>
+    <testcase classname="tests.test_tools" name="test_process" time="0.122"/>
   </testsuite>
 </testsuites>
```

### Comparing `hatch_ci-0.0.4/src/hatch_ci/cli.py` & `hatch_ci-0.0.4b25/src/hatch_ci/cli.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.4/src/hatch_ci/scm.py` & `hatch_ci-0.0.4b25/src/hatch_ci/scm.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.4/src/hatch_ci/script.py` & `hatch_ci-0.0.4b25/src/hatch_ci/script.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.4/src/hatch_ci/tools.py` & `hatch_ci-0.0.4b25/src/hatch_ci/tools.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.4/src/hatch_ci/version_hook.py` & `hatch_ci-0.0.4b25/src/hatch_ci/version_hook.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.4/tests/conftest.py` & `hatch_ci-0.0.4b25/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.4/tests/test_scm.py` & `hatch_ci-0.0.4b25/tests/test_scm.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.4/tests/test_tools.py` & `hatch_ci-0.0.4b25/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.4/LICENSE.txt` & `hatch_ci-0.0.4b25/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.4/README.md` & `hatch_ci-0.0.4b25/README.md`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.4/pyproject.toml` & `hatch_ci-0.0.4b25/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.4/PKG-INFO` & `hatch_ci-0.0.4b25/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hatch-ci
-Version: 0.0.4
+Version: 0.0.4b25
 Summary: Hatch plugin for ci system versioning
 Project-URL: Issues, https://github.com/cav71/hatch-ci/issues
 Project-URL: Source, https://github.com/cav71/hatch-ci
 Author-email: Antonio Cavallo <a.cavallo@cavallinux.eu>
 License: MIT
 License-File: LICENSE.txt
 Keywords: git,hatch,plugin,scm,version
```

