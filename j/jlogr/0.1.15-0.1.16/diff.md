# Comparing `tmp/jlogr-0.1.15.tar.gz` & `tmp/jlogr-0.1.16.tar.gz`

## Comparing `jlogr-0.1.15.tar` & `jlogr-0.1.16.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      394 1970-01-01 00:00:00.000000 jlogr-0.1.15/Cargo.toml
--rw-r--r--   0     1001      123      583 2023-08-06 11:40:34.000000 jlogr-0.1.15/.github/workflows/publish.yml
--rw-r--r--   0     1001      123       42 2023-08-06 11:40:34.000000 jlogr-0.1.15/.gitignore
--rw-r--r--   0     1001      123     1062 2023-08-06 11:40:34.000000 jlogr-0.1.15/LICENSE
--rw-r--r--   0     1001      123      123 2023-08-06 11:40:34.000000 jlogr-0.1.15/README.md
--rw-r--r--   0     1001      123      127 2023-08-06 11:40:34.000000 jlogr-0.1.15/pyproject.toml
--rw-r--r--   0     1001      123      104 2023-08-06 11:40:34.000000 jlogr-0.1.15/python/jlogr/__init__.py
--rw-r--r--   0     1001      123     4505 2023-08-06 11:40:34.000000 jlogr-0.1.15/src/lib.rs
--rw-r--r--   0     1001      123     2244 2023-08-06 11:40:34.000000 jlogr-0.1.15/src/structures/logger.rs
--rw-r--r--   0     1001      123     4763 2023-08-06 11:40:34.000000 jlogr-0.1.15/src/structures/logging.rs
--rw-r--r--   0     1001      123       33 2023-08-06 11:40:34.000000 jlogr-0.1.15/src/structures/mod.rs
--rw-r--r--   0     1001      123    13667 2023-08-06 11:40:38.000000 jlogr-0.1.15/Cargo.lock
--rw-r--r--   0        0        0      266 1970-01-01 00:00:00.000000 jlogr-0.1.15/PKG-INFO
+-rw-r--r--   0        0        0      394 1970-01-01 00:00:00.000000 jlogr-0.1.16/Cargo.toml
+-rw-r--r--   0     1001      123      583 2023-08-06 11:49:14.000000 jlogr-0.1.16/.github/workflows/publish.yml
+-rw-r--r--   0     1001      123       42 2023-08-06 11:49:14.000000 jlogr-0.1.16/.gitignore
+-rw-r--r--   0     1001      123     1062 2023-08-06 11:49:14.000000 jlogr-0.1.16/LICENSE
+-rw-r--r--   0     1001      123      123 2023-08-06 11:49:14.000000 jlogr-0.1.16/README.md
+-rw-r--r--   0     1001      123      180 2023-08-06 11:49:14.000000 jlogr-0.1.16/pyproject.toml
+-rw-r--r--   0     1001      123      136 2023-08-06 11:49:14.000000 jlogr-0.1.16/python/jlogr/__init__.py
+-rw-r--r--   0     1001      123     4505 2023-08-06 11:49:14.000000 jlogr-0.1.16/src/lib.rs
+-rw-r--r--   0     1001      123     2244 2023-08-06 11:49:14.000000 jlogr-0.1.16/src/structures/logger.rs
+-rw-r--r--   0     1001      123     4763 2023-08-06 11:49:14.000000 jlogr-0.1.16/src/structures/logging.rs
+-rw-r--r--   0     1001      123       33 2023-08-06 11:49:14.000000 jlogr-0.1.16/src/structures/mod.rs
+-rw-r--r--   0     1001      123    13667 2023-08-06 11:49:18.000000 jlogr-0.1.16/Cargo.lock
+-rw-r--r--   0        0        0      266 1970-01-01 00:00:00.000000 jlogr-0.1.16/PKG-INFO
```

### Comparing `jlogr-0.1.15/.github/workflows/publish.yml` & `jlogr-0.1.16/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `jlogr-0.1.15/LICENSE` & `jlogr-0.1.16/LICENSE`

 * *Files identical despite different names*

### Comparing `jlogr-0.1.15/src/lib.rs` & `jlogr-0.1.16/src/lib.rs`

 * *Files identical despite different names*

### Comparing `jlogr-0.1.15/src/structures/logger.rs` & `jlogr-0.1.16/src/structures/logger.rs`

 * *Files identical despite different names*

### Comparing `jlogr-0.1.15/src/structures/logging.rs` & `jlogr-0.1.16/src/structures/logging.rs`

 * *Files identical despite different names*

### Comparing `jlogr-0.1.15/Cargo.lock` & `jlogr-0.1.16/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "jlogr"
-version = "0.1.15"
+version = "0.1.16"
 dependencies = [
  "anyhow",
  "chrono",
  "pyo3",
  "termcolor",
 ]
```

