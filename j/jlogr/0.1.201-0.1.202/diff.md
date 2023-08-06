# Comparing `tmp/jlogr-0.1.201.tar.gz` & `tmp/jlogr-0.1.202.tar.gz`

## Comparing `jlogr-0.1.201.tar` & `jlogr-0.1.202.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      419 1970-01-01 00:00:00.000000 jlogr-0.1.201/Cargo.toml
--rw-r--r--   0     1001      123      583 2023-08-06 13:05:35.000000 jlogr-0.1.201/.github/workflows/publish.yml
--rw-r--r--   0     1001      123       42 2023-08-06 13:05:35.000000 jlogr-0.1.201/.gitignore
--rw-r--r--   0     1001      123     1062 2023-08-06 13:05:35.000000 jlogr-0.1.201/LICENSE
--rw-r--r--   0     1001      123      123 2023-08-06 13:05:35.000000 jlogr-0.1.201/README.md
--rw-r--r--   0     1001      123      199 2023-08-06 13:05:35.000000 jlogr-0.1.201/pyproject.toml
--rw-r--r--   0     1001      123      137 2023-08-06 13:05:35.000000 jlogr-0.1.201/python/jlogr/__init__.py
--rw-r--r--   0     1001      123     4477 2023-08-06 13:05:35.000000 jlogr-0.1.201/src/lib.rs
--rw-r--r--   0     1001      123     2244 2023-08-06 13:05:35.000000 jlogr-0.1.201/src/structures/logger.rs
--rw-r--r--   0     1001      123     4763 2023-08-06 13:05:35.000000 jlogr-0.1.201/src/structures/logging.rs
--rw-r--r--   0     1001      123       33 2023-08-06 13:05:35.000000 jlogr-0.1.201/src/structures/mod.rs
--rw-r--r--   0     1001      123    13668 2023-08-06 13:05:45.000000 jlogr-0.1.201/Cargo.lock
--rw-r--r--   0        0        0      267 1970-01-01 00:00:00.000000 jlogr-0.1.201/PKG-INFO
+-rw-r--r--   0        0        0      484 1970-01-01 00:00:00.000000 jlogr-0.1.202/Cargo.toml
+-rw-r--r--   0     1001      123      583 2023-08-06 13:44:25.000000 jlogr-0.1.202/.github/workflows/publish.yml
+-rw-r--r--   0     1001      123       42 2023-08-06 13:44:25.000000 jlogr-0.1.202/.gitignore
+-rw-r--r--   0     1001      123     1062 2023-08-06 13:44:25.000000 jlogr-0.1.202/LICENSE
+-rw-r--r--   0     1001      123      123 2023-08-06 13:44:25.000000 jlogr-0.1.202/README.md
+-rw-r--r--   0     1001      123       92 2023-08-06 13:44:25.000000 jlogr-0.1.202/package/jlogr/__init__.py
+-rw-r--r--   0     1001      123      230 2023-08-06 13:44:25.000000 jlogr-0.1.202/pyproject.toml
+-rw-r--r--   0     1001      123     4532 2023-08-06 13:44:25.000000 jlogr-0.1.202/src/lib.rs
+-rw-r--r--   0     1001      123     2244 2023-08-06 13:44:25.000000 jlogr-0.1.202/src/structures/logger.rs
+-rw-r--r--   0     1001      123     4763 2023-08-06 13:44:25.000000 jlogr-0.1.202/src/structures/logging.rs
+-rw-r--r--   0     1001      123       33 2023-08-06 13:44:25.000000 jlogr-0.1.202/src/structures/mod.rs
+-rw-r--r--   0     1001      123    13668 2023-08-06 13:44:29.000000 jlogr-0.1.202/Cargo.lock
+-rw-r--r--   0        0        0      267 1970-01-01 00:00:00.000000 jlogr-0.1.202/PKG-INFO
```

### Comparing `jlogr-0.1.201/.github/workflows/publish.yml` & `jlogr-0.1.202/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `jlogr-0.1.201/LICENSE` & `jlogr-0.1.202/LICENSE`

 * *Files identical despite different names*

### Comparing `jlogr-0.1.201/src/lib.rs` & `jlogr-0.1.202/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 #[pymodule]
 #[pyo3(name = "jlogr")]
 #[doc = "
 Module for clean and colourful logging in python
 This is just how i like my logs, so there aren't formatting options or anything like that.
 If you want to change the format, feel free to make a fork.
 "]
-pub fn jlogr(py: Python<'_>, m: &PyModule) -> PyResult<()> {
+pub fn jlogr(_py: Python<'_>, m: &PyModule) -> PyResult<()> {
+    m.add("__version__", env!("CARGO_PKG_VERSION"))?;
     m.add_function(wrap_pyfunction!(info, m)?)?;
     m.add_function(wrap_pyfunction!(debug, m)?)?;
     m.add_function(wrap_pyfunction!(warning, m)?)?;
     m.add_function(wrap_pyfunction!(error, m)?)?;
     m.add_function(wrap_pyfunction!(parse_list_of_logs, m)?)?;
     Ok(())
 }
```

### Comparing `jlogr-0.1.201/src/structures/logger.rs` & `jlogr-0.1.202/src/structures/logger.rs`

 * *Files identical despite different names*

### Comparing `jlogr-0.1.201/src/structures/logging.rs` & `jlogr-0.1.202/src/structures/logging.rs`

 * *Files identical despite different names*

### Comparing `jlogr-0.1.201/Cargo.lock` & `jlogr-0.1.202/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "jlogr"
-version = "0.1.201"
+version = "0.1.202"
 dependencies = [
  "anyhow",
  "chrono",
  "pyo3",
  "termcolor",
 ]
```

