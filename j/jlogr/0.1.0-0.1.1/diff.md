# Comparing `tmp/jlogr-0.1.0.tar.gz` & `tmp/jlogr-0.1.1.tar.gz`

## Comparing `jlogr-0.1.0.tar` & `jlogr-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0      364 1970-01-01 00:00:00.000000 jlogr-0.1.0/Cargo.toml
--rw-r--r--   0      501       20       33 2023-08-06 06:32:45.000000 jlogr-0.1.0/.gitignore
--rw-r--r--   0      501       20      375 2023-08-06 07:43:36.000000 jlogr-0.1.0/logs.log
--rw-r--r--   0      501       20      127 2023-08-06 04:07:10.000000 jlogr-0.1.0/pyproject.toml
--rw-r--r--   0      501       20     4201 2023-08-06 07:31:08.000000 jlogr-0.1.0/src/lib.rs
--rw-r--r--   0      501       20     2244 2023-08-06 07:40:40.000000 jlogr-0.1.0/src/structures/logger.rs
--rw-r--r--   0      501       20     4763 2023-08-06 07:33:51.000000 jlogr-0.1.0/src/structures/logging.rs
--rw-r--r--   0      501       20       33 2023-08-06 05:33:34.000000 jlogr-0.1.0/src/structures/mod.rs
--rw-r--r--   0      501       20    13666 2023-08-06 05:17:46.000000 jlogr-0.1.0/Cargo.lock
--rw-r--r--   0        0        0       49 1970-01-01 00:00:00.000000 jlogr-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      364 1970-01-01 00:00:00.000000 jlogr-0.1.1/Cargo.toml
+-rw-r--r--   0     1001      123      513 2023-08-06 09:38:13.000000 jlogr-0.1.1/.github/workflows/publish.yml
+-rw-r--r--   0     1001      123       42 2023-08-06 09:38:13.000000 jlogr-0.1.1/.gitignore
+-rw-r--r--   0     1001      123     1062 2023-08-06 09:38:13.000000 jlogr-0.1.1/LICENSE
+-rw-r--r--   0     1001      123      127 2023-08-06 09:38:13.000000 jlogr-0.1.1/pyproject.toml
+-rw-r--r--   0     1001      123     3945 2023-08-06 09:38:13.000000 jlogr-0.1.1/src/lib.rs
+-rw-r--r--   0     1001      123     2244 2023-08-06 09:38:13.000000 jlogr-0.1.1/src/structures/logger.rs
+-rw-r--r--   0     1001      123     4763 2023-08-06 09:38:13.000000 jlogr-0.1.1/src/structures/logging.rs
+-rw-r--r--   0     1001      123       33 2023-08-06 09:38:13.000000 jlogr-0.1.1/src/structures/mod.rs
+-rw-r--r--   0     1001      123    13666 2023-08-06 09:38:16.000000 jlogr-0.1.1/Cargo.lock
+-rw-r--r--   0        0        0       49 1970-01-01 00:00:00.000000 jlogr-0.1.1/PKG-INFO
```

### Comparing `jlogr-0.1.0/src/lib.rs` & `jlogr-0.1.1/src/lib.rs`

 * *Files 26% similar despite different names*

```diff
@@ -1,135 +1,148 @@
 pub mod structures;
 use pyo3::prelude::*;
 use structures::logging::Log;
 
-/// Module for clean and colourful logging in python
-/// This is just how i like my logs, so there aren't formatting options or anything like that.
-/// If you want to change the format, feel free to make a fork.
 #[pymodule]
+#[doc = "
+Module for clean and colourful logging in python
+This is just how i like my logs, so there aren't formatting options or anything like that.
+If you want to change the format, feel free to make a fork.
+"]
 fn jlogr(_py: Python, m: &PyModule) -> PyResult<()> {
     m.add_function(wrap_pyfunction!(info, m)?)?;
     m.add_function(wrap_pyfunction!(debug, m)?)?;
     m.add_function(wrap_pyfunction!(warning, m)?)?;
     m.add_function(wrap_pyfunction!(error, m)?)?;
     m.add_function(wrap_pyfunction!(parse_list_of_logs, m)?)?;
     Ok(())
 }
 
-/// Log a info message
-///
-/// # Example
-/// ```python
-/// import jlogr
-/// jlogr.info("Hello, world!")
-/// ```
-///
-/// # Output
-/// ```bash
-/// 2021-08-15T21:04:05.000000000+00:00 :: [INFO] :: Hello, world!
-/// ```
-///
-/// # Parameters
-/// - message: The message to log
-/// - module: The module that the message is coming from
-/// - function: The function that the message is coming from
-/// - class: The class that the message is coming from
 #[pyfunction]
+#[doc = "
+Log a info message
+
+# Example
+```python
+import jlogr
+jlogr.info(\"Hello, world!\")
+```
+
+# Output
+```bash
+2021-08-15T21:04:05.000000000+00:00 :: [INFO] :: Hello, world!
+```
+
+# Parameters
+- message: The message to log
+- module: The module that the message is coming from
+- function: The function that the message is coming from
+- class: The class that the message is coming from
+"]
 fn info(message: &str, module: Option<&str>, function: Option<&str>, class: Option<&str>) {
     Log::new(message, "info", module, function, class).pretty_print();
 }
 
-/// Log a debug message
-///
-/// # Example
-/// ```python
-/// import jlogr
-/// jlogr.debug("Hello, world!")
-/// ```
-/// # Output
-/// ```bash
-/// 2021-08-15T21:04:05.000000000+00:00 :: [DEBUG] :: Hello, world!
-/// ```
-///
-/// # Parameters
-/// - message: The message to log
-/// - module: The module that the message is coming from
-/// - function: The function that the message is coming from
-/// - class: The class that the message is coming from
 #[pyfunction]
+#[doc = "
+Log a debug message
+# Example
+```python
+import jlogr
+jlogr.debug(\"Hello, world!\")
+```
+
+# Output
+```bash
+2021-08-15T21:04:05.000000000+00:00 :: [DEBUG] :: Hello, world!
+```
+
+# Parameters
+- message: The message to log
+- module: The module that the message is coming from
+- function: The function that the message is coming from
+- class: The class that the message is coming from
+"]
 fn debug(message: &str) {
     Log::new(message, "debug", None, None, None).pretty_print();
 }
 
-/// Log a message as a warning
-///
-/// # Example
-/// ```python
-/// import jlogr
-/// jlogr.warning("Hello, world!")
-/// ```
-/// # Output
-/// ```bash
-/// 2021-08-15T21:04:05.000000000+00:00 :: [WARNING] :: Hello, world!
-/// ```
-///
-/// # Parameters
-/// - message: The message to log
-/// - module: The module that the message is coming from
-/// - function: The function that the message is coming from
-/// - class: The class that the message is coming from
 #[pyfunction]
+#[doc = "
+Log a message as a warning
+
+# Example
+```python
+import jlogr
+jlogr.warning(\"Hello, world!\")
+```
+
+# Output
+```bash
+2021-08-15T21:04:05.000000000+00:00 :: [WARNING] :: Hello, world!
+```
+
+# Parameters
+- message: The message to log
+- module: The module that the message is coming from
+- function: The function that the message is coming from
+- class: The class that the message is coming from
+"]
 fn warning(message: &str) {
     Log::new(message, "warning", None, None, None).pretty_print();
 }
 
-/// Log a message as an error
-///
-/// # Example
-/// ```python
-/// import jlogr
-/// jlogr.error("Hello, world!")
-/// ```
-///
-/// # Output
-/// ```bash
-/// 2021-08-15T21:04:05.000000000+00:00 :: [ERROR] :: Hello, world!
-/// ```
-///
-/// # Parameters
-/// - message: The message to log
-/// - module: The module that the message is coming from
-/// - function: The function that the message is coming from
-/// - class: The class that the message is coming from
 #[pyfunction]
+#[doc = "
+Log a message as an error
+
+# Example
+```python
+import jlogr
+jlogr.error(\"Hello, world!\")
+```
+
+# Output
+```bash
+2021-08-15T21:04:05.000000000+00:00 :: [ERROR] :: Hello, world!
+```
+
+# Parameters
+- message: The message to log
+- module: The module that the message is coming from
+- function: The function that the message is coming from
+- class: The class that the message is coming from
+"]
 fn error(message: &str) {
     Log::new(message, "error", None, None, None).pretty_print();
 }
 
-/// Logs should be a list of tuples of strings, where the first string is the message and the second
-/// string is the log level.
-///
-/// # Example
-/// ```python
-/// import jlogr
-/// logs = [("Hello, world!", "info"), ("Hello, world!", "debug"), ("Hello, world!", "warning"), ("Hello, world!", "error")]
-/// jlogr.parse_list_of_logs(logs)
-/// ```
-///
-/// # Output
-/// ```bash
-/// 2021-08-15T21:04:05.000000000+00:00 :: [INFO] :: Hello, world!
-/// 2021-08-15T21:04:05.000000000+00:00 :: [DEBUG] :: Hello, world!
-/// 2021-08-15T21:04:05.000000000+00:00 :: [WARNING] :: Hello, world!
-/// 2021-08-15T21:04:05.000000000+00:00 :: [ERROR] :: Hello, world!
-/// ```
-///
-/// # Parameters
-/// - logs: A list of tuples of strings, where the tuple is structured (message, level, module, function, class)
 #[pyfunction]
+#[doc = "
+Logs should be a list of tuples of strings, where the first string is the message and the second
+string is the log level.
+
+# Example
+```python
+import jlogr
+logs = [(\"Hello, world!\", \"info\"), (\"Hello, world!\", \"debug\"), (\"Hello, world!\", \"warning\"), (\"Hello, world!\", \"error\")]
+jlogr.parse_list_of_logs(logs)
+```
+
+# Output
+```bash
+2021-08-15T21:04:05.000000000+00:00 :: [INFO] :: Hello, world!
+2021-08-15T21:04:05.000000000+00:00 :: [DEBUG] :: Hello, world!
+2021-08-15T21:04:05.000000000+00:00 :: [WARNING] :: Hello, world!
+2021-08-15T21:04:05.000000000+00:00 :: [ERROR] :: Hello, world!
+```
+
+# Parameters
+- logs: A list of tuples of strings, where the tuple is structured (message, level, module, function, class)
+"]
 fn parse_list_of_logs(
     logs: Vec<(
         String,
         String,
         Option<String>,
         Option<String>,
         Option<String>,
```

### Comparing `jlogr-0.1.0/src/structures/logger.rs` & `jlogr-0.1.1/src/structures/logger.rs`

 * *Files identical despite different names*

### Comparing `jlogr-0.1.0/src/structures/logging.rs` & `jlogr-0.1.1/src/structures/logging.rs`

 * *Files identical despite different names*

### Comparing `jlogr-0.1.0/Cargo.lock` & `jlogr-0.1.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "jlogr"
-version = "0.1.0"
+version = "0.1.1"
 dependencies = [
  "anyhow",
  "chrono",
  "pyo3",
  "termcolor",
 ]
```

