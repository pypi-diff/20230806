# Comparing `tmp/jlogr-0.1.12.tar.gz` & `tmp/jlogr-0.1.13.tar.gz`

## Comparing `jlogr-0.1.12.tar` & `jlogr-0.1.13.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      394 1970-01-01 00:00:00.000000 jlogr-0.1.12/Cargo.toml
--rw-r--r--   0     1001      123      513 2023-08-06 10:35:22.000000 jlogr-0.1.12/.github/workflows/publish.yml
--rw-r--r--   0     1001      123       42 2023-08-06 10:35:22.000000 jlogr-0.1.12/.gitignore
--rw-r--r--   0     1001      123     1062 2023-08-06 10:35:22.000000 jlogr-0.1.12/LICENSE
--rw-r--r--   0     1001      123      123 2023-08-06 10:35:22.000000 jlogr-0.1.12/README.md
--rw-r--r--   0     1001      123      127 2023-08-06 10:35:22.000000 jlogr-0.1.12/pyproject.toml
--rw-r--r--   0     1001      123     4625 2023-08-06 10:35:22.000000 jlogr-0.1.12/src/lib.rs
--rw-r--r--   0     1001      123     2244 2023-08-06 10:35:22.000000 jlogr-0.1.12/src/structures/logger.rs
--rw-r--r--   0     1001      123     4763 2023-08-06 10:35:22.000000 jlogr-0.1.12/src/structures/logging.rs
--rw-r--r--   0     1001      123       33 2023-08-06 10:35:22.000000 jlogr-0.1.12/src/structures/mod.rs
--rw-r--r--   0     1001      123    13667 2023-08-06 10:35:31.000000 jlogr-0.1.12/Cargo.lock
--rw-r--r--   0        0        0      266 1970-01-01 00:00:00.000000 jlogr-0.1.12/PKG-INFO
+-rw-r--r--   0        0        0      394 1970-01-01 00:00:00.000000 jlogr-0.1.13/Cargo.toml
+-rw-r--r--   0     1001      123      583 2023-08-06 11:12:27.000000 jlogr-0.1.13/.github/workflows/publish.yml
+-rw-r--r--   0     1001      123       42 2023-08-06 11:12:27.000000 jlogr-0.1.13/.gitignore
+-rw-r--r--   0     1001      123     1062 2023-08-06 11:12:27.000000 jlogr-0.1.13/LICENSE
+-rw-r--r--   0     1001      123      123 2023-08-06 11:12:27.000000 jlogr-0.1.13/README.md
+-rw-r--r--   0     1001      123      127 2023-08-06 11:12:27.000000 jlogr-0.1.13/pyproject.toml
+-rw-r--r--   0     1001      123     4505 2023-08-06 11:12:27.000000 jlogr-0.1.13/src/lib.rs
+-rw-r--r--   0     1001      123     2244 2023-08-06 11:12:27.000000 jlogr-0.1.13/src/structures/logger.rs
+-rw-r--r--   0     1001      123     4763 2023-08-06 11:12:27.000000 jlogr-0.1.13/src/structures/logging.rs
+-rw-r--r--   0     1001      123       33 2023-08-06 11:12:27.000000 jlogr-0.1.13/src/structures/mod.rs
+-rw-r--r--   0     1001      123    13667 2023-08-06 11:12:32.000000 jlogr-0.1.13/Cargo.lock
+-rw-r--r--   0        0        0      266 1970-01-01 00:00:00.000000 jlogr-0.1.13/PKG-INFO
```

### Comparing `jlogr-0.1.12/LICENSE` & `jlogr-0.1.13/LICENSE`

 * *Files identical despite different names*

### Comparing `jlogr-0.1.12/src/lib.rs` & `jlogr-0.1.13/src/lib.rs`

 * *Files 10% similar despite different names*

```diff
@@ -36,17 +36,16 @@
 - message: The message to log
 - module: The module that the message is coming from
 - function: The function that the message is coming from
 - class: The class that the message is coming from
 "]
 #[pyo3(text_signature = "(message, module=None, function=None, class=None)")]
 #[pyo3(name = "info")]
-#[pyo3(pass_module)]
 fn info(
-    _py: &PyModule,
+    _py: Python,
     message: &str,
     module: Option<&str>,
     function: Option<&str>,
     class: Option<&str>,
 ) {
     Log::new(message, "info", module, function, class).pretty_print();
 }
@@ -69,16 +68,15 @@
 - message: The message to log
 - module: The module that the message is coming from
 - function: The function that the message is coming from
 - class: The class that the message is coming from
 "]
 #[pyo3(text_signature = "(message, module=None, function=None, class=None)")]
 #[pyo3(name = "debug")]
-#[pyo3(pass_module)]
-fn debug(_py: &PyModule, message: &str) {
+fn debug(_py: Python, message: &str) {
     Log::new(message, "debug", None, None, None).pretty_print();
 }
 
 #[pyfunction]
 #[doc = "
 Log a message as a warning
 
@@ -97,16 +95,15 @@
 - message: The message to log
 - module: The module that the message is coming from
 - function: The function that the message is coming from
 - class: The class that the message is coming from
 "]
 #[pyo3(text_signature = "(message, module=None, function=None, class=None)")]
 #[pyo3(name = "warning")]
-#[pyo3(pass_module)]
-fn warning(_py: &PyModule, message: &str) {
+fn warning(_py: Python, message: &str) {
     Log::new(message, "warning", None, None, None).pretty_print();
 }
 
 #[pyfunction]
 #[doc = "
 Log a message as an error
 
@@ -125,16 +122,15 @@
 - message: The message to log
 - module: The module that the message is coming from
 - function: The function that the message is coming from
 - class: The class that the message is coming from
 "]
 #[pyo3(text_signature = "(message, module=None, function=None, class=None)")]
 #[pyo3(name = "error")]
-#[pyo3(pass_module)]
-fn error(_py: &PyModule, message: &str) {
+fn error(_py: Python, message: &str) {
     Log::new(message, "error", None, None, None).pretty_print();
 }
 
 #[pyfunction]
 #[doc = "
 Logs should be a list of tuples of strings, where the first string is the message and the second
 string is the log level.
@@ -155,17 +151,16 @@
 ```
 
 # Parameters
 - logs: A list of tuples of strings, where the tuple is structured (message, level, module, function, class)
 "]
 #[pyo3(text_signature = "(logs)")]
 #[pyo3(name = "error")]
-#[pyo3(pass_module)]
 fn parse_list_of_logs(
-    _py: &PyModule,
+    _py: Python,
     logs: Vec<(
         String,
         String,
         Option<String>,
         Option<String>,
         Option<String>,
     )>,
```

### Comparing `jlogr-0.1.12/src/structures/logger.rs` & `jlogr-0.1.13/src/structures/logger.rs`

 * *Files identical despite different names*

### Comparing `jlogr-0.1.12/src/structures/logging.rs` & `jlogr-0.1.13/src/structures/logging.rs`

 * *Files identical despite different names*

### Comparing `jlogr-0.1.12/Cargo.lock` & `jlogr-0.1.13/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "jlogr"
-version = "0.1.12"
+version = "0.1.13"
 dependencies = [
  "anyhow",
  "chrono",
  "pyo3",
  "termcolor",
 ]
```

