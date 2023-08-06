# Comparing `tmp/tensorshare-0.0.1.tar.gz` & `tmp/tensorshare-0.0.2.tar.gz`

## Comparing `tensorshare-0.0.1.tar` & `tensorshare-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,14 @@
--rw-r--r--   0        0        0     5507 2020-02-02 00:00:00.000000 tensorshare-0.0.1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     2758 2020-02-02 00:00:00.000000 tensorshare-0.0.1/CONTRIBUTING.md
--rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 tensorshare-0.0.1/mkdocs.yml
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 tensorshare-0.0.1/src/tensorshare/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tensorshare-0.0.1/src/tensorshare/py.typed
--rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 tensorshare-0.0.1/.gitignore
--rw-r--r--   0        0        0    10758 2020-02-02 00:00:00.000000 tensorshare-0.0.1/LICENSE
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 tensorshare-0.0.1/README.md
--rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 tensorshare-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 tensorshare-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     5507 2020-02-02 00:00:00.000000 tensorshare-0.0.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     2758 2020-02-02 00:00:00.000000 tensorshare-0.0.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 tensorshare-0.0.2/mkdocs.yml
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 tensorshare-0.0.2/src/tensorshare/__init__.py
+-rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 tensorshare-0.0.2/src/tensorshare/import_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tensorshare-0.0.2/src/tensorshare/py.typed
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 tensorshare-0.0.2/src/tensorshare/schema.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 tensorshare-0.0.2/src/tensorshare/converter/__init__.py
+-rw-r--r--   0        0        0     4269 2020-02-02 00:00:00.000000 tensorshare-0.0.2/src/tensorshare/converter/utils.py
+-rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 tensorshare-0.0.2/.gitignore
+-rw-r--r--   0        0        0    10758 2020-02-02 00:00:00.000000 tensorshare-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 tensorshare-0.0.2/README.md
+-rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 tensorshare-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4982 2020-02-02 00:00:00.000000 tensorshare-0.0.2/PKG-INFO
```

### Comparing `tensorshare-0.0.1/CODE_OF_CONDUCT.md` & `tensorshare-0.0.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `tensorshare-0.0.1/CONTRIBUTING.md` & `tensorshare-0.0.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `tensorshare-0.0.1/mkdocs.yml` & `tensorshare-0.0.2/mkdocs.yml`

 * *Files 13% similar despite different names*

```diff
@@ -18,19 +18,23 @@
     - scheme: slate
       toggle:
         icon: material/brightness-4
         name: Switch to light mode
   font:
     text: Roboto
     code: Roboto Mono
+  icon:
+    logo: material/handshake
 
 markdown_extensions:
   - pymdownx.highlight:
       anchor_linenums: true
   - pymdownx.superfences
+  - pymdownx.tasklist:
+      custom_checkbox: true
 
 plugins:
   - search:
   - git-revision-date-localized:
       type: timeago
       enable_creation_date: true
   - mkdocstrings:
```

### Comparing `tensorshare-0.0.1/src/tensorshare/__init__.py` & `tensorshare-0.0.2/src/tensorshare/converter/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,11 +7,8 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""`tensorshare `: 🤝 Trade any tensors over the network"""
-
-__author__ = "Thomas Chaigneau <t.chaigneau.tc@gmail.com>"
-__version__ = "0.0.1"
+"""Converter is used to convert any tensors format to safetensors format"""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `tensorshare-0.0.1/.gitignore` & `tensorshare-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `tensorshare-0.0.1/LICENSE` & `tensorshare-0.0.2/LICENSE`

 * *Files identical despite different names*

