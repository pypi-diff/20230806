# Comparing `tmp/autorunpy-5.0.0.tar.gz` & `tmp/autorunpy-6.0.0.tar.gz`

## Comparing `autorunpy-5.0.0.tar` & `autorunpy-6.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 autorunpy-5.0.0/.gitattributes
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 autorunpy-5.0.0/src/autorunpy/__init__.py
--rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 autorunpy-5.0.0/src/autorunpy/auto.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 autorunpy-5.0.0/src/autorunpy/dl_and_ret_dirpath.py
--rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 autorunpy-5.0.0/src/autorunpy/github_release.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 autorunpy-5.0.0/src/autorunpy/make_venv.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 autorunpy-5.0.0/src/autorunpy/ret_module_2_run_name.py
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 autorunpy-5.0.0/src/autorunpy/rm_venv.py
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 autorunpy-5.0.0/src/autorunpy/util.py
--rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 autorunpy-5.0.0/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 autorunpy-5.0.0/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autorunpy-5.0.0/README.md
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 autorunpy-5.0.0/pyproject.toml
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 autorunpy-5.0.0/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 autorunpy-6.0.0/.gitattributes
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 autorunpy-6.0.0/.github/workflows/publish-on-pip-on-release.yml
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 autorunpy-6.0.0/src/autorunpy/__init__.py
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 autorunpy-6.0.0/src/autorunpy/auto.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 autorunpy-6.0.0/src/autorunpy/dl_and_ret_dirpath.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 autorunpy-6.0.0/src/autorunpy/github_release.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 autorunpy-6.0.0/src/autorunpy/make_venv.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 autorunpy-6.0.0/src/autorunpy/ret_module_2_run_name.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 autorunpy-6.0.0/src/autorunpy/util.py
+-rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 autorunpy-6.0.0/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 autorunpy-6.0.0/LICENSE
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 autorunpy-6.0.0/README.md
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 autorunpy-6.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 autorunpy-6.0.0/PKG-INFO
```

### Comparing `autorunpy-5.0.0/.gitignore` & `autorunpy-6.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `autorunpy-5.0.0/LICENSE` & `autorunpy-6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `autorunpy-5.0.0/PKG-INFO` & `autorunpy-6.0.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autorunpy
-Version: 5.0.0
+Version: 6.0.0
 Summary: Tools for auto running python scripts
 Project-URL: Homepage, https://github.com/imahdimir/pyautorun
 Project-URL: Bug Tracker, https://github.com/imahdimir/pyautorun/issues
 Author-email: Mahdi Mir <imahdimir@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Mahdi
@@ -24,7 +24,10 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 License-File: LICENSE
 Requires-Dist: requests
+Description-Content-Type: text/markdown
+
+Tools for auto running Python scripts.
```

