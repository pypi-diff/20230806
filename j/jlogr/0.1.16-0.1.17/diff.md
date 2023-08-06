# Comparing `tmp/jlogr-0.1.16.tar.gz` & `tmp/jlogr-0.1.17.tar.gz`

## Comparing `jlogr-0.1.16.tar` & `jlogr-0.1.17.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      394 1970-01-01 00:00:00.000000 jlogr-0.1.16/Cargo.toml
--rw-r--r--   0     1001      123      583 2023-08-06 11:49:14.000000 jlogr-0.1.16/.github/workflows/publish.yml
--rw-r--r--   0     1001      123       42 2023-08-06 11:49:14.000000 jlogr-0.1.16/.gitignore
--rw-r--r--   0     1001      123     1062 2023-08-06 11:49:14.000000 jlogr-0.1.16/LICENSE
--rw-r--r--   0     1001      123      123 2023-08-06 11:49:14.000000 jlogr-0.1.16/README.md
--rw-r--r--   0     1001      123      180 2023-08-06 11:49:14.000000 jlogr-0.1.16/pyproject.toml
--rw-r--r--   0     1001      123      136 2023-08-06 11:49:14.000000 jlogr-0.1.16/python/jlogr/__init__.py
--rw-r--r--   0     1001      123     4505 2023-08-06 11:49:14.000000 jlogr-0.1.16/src/lib.rs
--rw-r--r--   0     1001      123     2244 2023-08-06 11:49:14.000000 jlogr-0.1.16/src/structures/logger.rs
--rw-r--r--   0     1001      123     4763 2023-08-06 11:49:14.000000 jlogr-0.1.16/src/structures/logging.rs
--rw-r--r--   0     1001      123       33 2023-08-06 11:49:14.000000 jlogr-0.1.16/src/structures/mod.rs
--rw-r--r--   0     1001      123    13667 2023-08-06 11:49:18.000000 jlogr-0.1.16/Cargo.lock
--rw-r--r--   0        0        0      266 1970-01-01 00:00:00.000000 jlogr-0.1.16/PKG-INFO
+-rw-r--r--   0        0        0      394 1970-01-01 00:00:00.000000 jlogr-0.1.17/Cargo.toml
+-rw-r--r--   0     1001      123      583 2023-08-06 12:00:36.000000 jlogr-0.1.17/.github/workflows/publish.yml
+-rw-r--r--   0     1001      123       42 2023-08-06 12:00:36.000000 jlogr-0.1.17/.gitignore
+-rw-r--r--   0     1001      123     1062 2023-08-06 12:00:36.000000 jlogr-0.1.17/LICENSE
+-rw-r--r--   0     1001      123      123 2023-08-06 12:00:36.000000 jlogr-0.1.17/README.md
+-rw-r--r--   0     1001      123      180 2023-08-06 12:00:36.000000 jlogr-0.1.17/pyproject.toml
+-rw-r--r--   0     1001      123        0 2023-08-06 12:00:36.000000 jlogr-0.1.17/python/jlogr/__init__.py
+-rw-r--r--   0     1001      123     4566 2023-08-06 12:00:36.000000 jlogr-0.1.17/src/lib.rs
+-rw-r--r--   0     1001      123     2244 2023-08-06 12:00:36.000000 jlogr-0.1.17/src/structures/logger.rs
+-rw-r--r--   0     1001      123     4763 2023-08-06 12:00:36.000000 jlogr-0.1.17/src/structures/logging.rs
+-rw-r--r--   0     1001      123       33 2023-08-06 12:00:36.000000 jlogr-0.1.17/src/structures/mod.rs
+-rw-r--r--   0     1001      123    13667 2023-08-06 12:00:39.000000 jlogr-0.1.17/Cargo.lock
+-rw-r--r--   0        0        0      266 1970-01-01 00:00:00.000000 jlogr-0.1.17/PKG-INFO
```

### Comparing `jlogr-0.1.16/.github/workflows/publish.yml` & `jlogr-0.1.17/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `jlogr-0.1.16/LICENSE` & `jlogr-0.1.17/LICENSE`

 * *Files identical despite different names*

### Comparing `jlogr-0.1.16/src/lib.rs` & `jlogr-0.1.17/src/lib.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 pub mod structures;
 use pyo3::prelude::*;
 use structures::logging::Log;
 
 #[pymodule]
+#[pyo3(name = "jlogr")]
 #[doc = "
 Module for clean and colourful logging in python
 This is just how i like my logs, so there aren't formatting options or anything like that.
 If you want to change the format, feel free to make a fork.
 "]
-fn jlogr(_py: Python, m: &PyModule) -> PyResult<()> {
+pub fn jlogr(_py: Python, m: &PyModule) -> PyResult<()> {
     m.add_function(wrap_pyfunction!(info, m)?)?;
     m.add_function(wrap_pyfunction!(debug, m)?)?;
     m.add_function(wrap_pyfunction!(warning, m)?)?;
     m.add_function(wrap_pyfunction!(error, m)?)?;
     m.add_function(wrap_pyfunction!(parse_list_of_logs, m)?)?;
     Ok(())
 }
@@ -34,17 +35,17 @@
 
 # Parameters
 - message: The message to log
 - module: The module that the message is coming from
 - function: The function that the message is coming from
 - class: The class that the message is coming from
 "]
-#[pyo3(text_signature = "(message, module=None, function=None, class=None)")]
 #[pyo3(name = "info")]
-fn info(
+#[pyo3(text_signature = "(message, module=None, function=None, class=None)")]
+pub fn info(
     _py: Python,
     message: &str,
     module: Option<&str>,
     function: Option<&str>,
     class: Option<&str>,
 ) {
     Log::new(message, "info", module, function, class).pretty_print();
@@ -68,15 +69,15 @@
 - message: The message to log
 - module: The module that the message is coming from
 - function: The function that the message is coming from
 - class: The class that the message is coming from
 "]
 #[pyo3(text_signature = "(message, module=None, function=None, class=None)")]
 #[pyo3(name = "debug")]
-fn debug(_py: Python, message: &str) {
+pub fn debug(_py: Python, message: &str) {
     Log::new(message, "debug", None, None, None).pretty_print();
 }
 
 #[pyfunction]
 #[doc = "
 Log a message as a warning
 
@@ -95,15 +96,15 @@
 - message: The message to log
 - module: The module that the message is coming from
 - function: The function that the message is coming from
 - class: The class that the message is coming from
 "]
 #[pyo3(text_signature = "(message, module=None, function=None, class=None)")]
 #[pyo3(name = "warning")]
-fn warning(_py: Python, message: &str) {
+pub fn warning(_py: Python, message: &str) {
     Log::new(message, "warning", None, None, None).pretty_print();
 }
 
 #[pyfunction]
 #[doc = "
 Log a message as an error
 
@@ -122,15 +123,15 @@
 - message: The message to log
 - module: The module that the message is coming from
 - function: The function that the message is coming from
 - class: The class that the message is coming from
 "]
 #[pyo3(text_signature = "(message, module=None, function=None, class=None)")]
 #[pyo3(name = "error")]
-fn error(_py: Python, message: &str) {
+pub fn error(_py: Python, message: &str) {
     Log::new(message, "error", None, None, None).pretty_print();
 }
 
 #[pyfunction]
 #[doc = "
 Logs should be a list of tuples of strings, where the first string is the message and the second
 string is the log level.
@@ -150,16 +151,16 @@
 2021-08-15T21:04:05.000000000+00:00 :: [ERROR] :: Hello, world!
 ```
 
 # Parameters
 - logs: A list of tuples of strings, where the tuple is structured (message, level, module, function, class)
 "]
 #[pyo3(text_signature = "(logs)")]
-#[pyo3(name = "error")]
-fn parse_list_of_logs(
+#[pyo3(name = "parse_list_of_logs")]
+pub fn parse_list_of_logs(
     _py: Python,
     logs: Vec<(
         String,
         String,
         Option<String>,
         Option<String>,
         Option<String>,
```

### Comparing `jlogr-0.1.16/src/structures/logger.rs` & `jlogr-0.1.17/src/structures/logger.rs`

 * *Files identical despite different names*

### Comparing `jlogr-0.1.16/src/structures/logging.rs` & `jlogr-0.1.17/src/structures/logging.rs`

 * *Files identical despite different names*

### Comparing `jlogr-0.1.16/Cargo.lock` & `jlogr-0.1.17/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "jlogr"
-version = "0.1.16"
+version = "0.1.17"
 dependencies = [
  "anyhow",
  "chrono",
  "pyo3",
  "termcolor",
 ]
```

