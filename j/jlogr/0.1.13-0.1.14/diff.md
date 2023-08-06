# Comparing `tmp/jlogr-0.1.13.tar.gz` & `tmp/jlogr-0.1.14.tar.gz`

## Comparing `jlogr-0.1.13.tar` & `jlogr-0.1.14.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0      394 1970-01-01 00:00:00.000000 jlogr-0.1.13/Cargo.toml
--rw-r--r--   0     1001      123      583 2023-08-06 11:12:27.000000 jlogr-0.1.13/.github/workflows/publish.yml
--rw-r--r--   0     1001      123       42 2023-08-06 11:12:27.000000 jlogr-0.1.13/.gitignore
--rw-r--r--   0     1001      123     1062 2023-08-06 11:12:27.000000 jlogr-0.1.13/LICENSE
--rw-r--r--   0     1001      123      123 2023-08-06 11:12:27.000000 jlogr-0.1.13/README.md
--rw-r--r--   0     1001      123      127 2023-08-06 11:12:27.000000 jlogr-0.1.13/pyproject.toml
--rw-r--r--   0     1001      123     4505 2023-08-06 11:12:27.000000 jlogr-0.1.13/src/lib.rs
--rw-r--r--   0     1001      123     2244 2023-08-06 11:12:27.000000 jlogr-0.1.13/src/structures/logger.rs
--rw-r--r--   0     1001      123     4763 2023-08-06 11:12:27.000000 jlogr-0.1.13/src/structures/logging.rs
--rw-r--r--   0     1001      123       33 2023-08-06 11:12:27.000000 jlogr-0.1.13/src/structures/mod.rs
--rw-r--r--   0     1001      123    13667 2023-08-06 11:12:32.000000 jlogr-0.1.13/Cargo.lock
--rw-r--r--   0        0        0      266 1970-01-01 00:00:00.000000 jlogr-0.1.13/PKG-INFO
+-rw-r--r--   0        0        0      394 1970-01-01 00:00:00.000000 jlogr-0.1.14/Cargo.toml
+-rw-r--r--   0     1001      123      583 2023-08-06 11:29:49.000000 jlogr-0.1.14/.github/workflows/publish.yml
+-rw-r--r--   0     1001      123       42 2023-08-06 11:29:49.000000 jlogr-0.1.14/.gitignore
+-rw-r--r--   0     1001      123     1062 2023-08-06 11:29:49.000000 jlogr-0.1.14/LICENSE
+-rw-r--r--   0     1001      123      123 2023-08-06 11:29:49.000000 jlogr-0.1.14/README.md
+-rw-r--r--   0     1001      123        0 2023-08-06 11:29:49.000000 jlogr-0.1.14/jlogr/__init__.py
+-rw-r--r--   0     1001      123      127 2023-08-06 11:29:49.000000 jlogr-0.1.14/pyproject.toml
+-rw-r--r--   0     1001      123     4505 2023-08-06 11:29:49.000000 jlogr-0.1.14/src/lib.rs
+-rw-r--r--   0     1001      123     2244 2023-08-06 11:29:49.000000 jlogr-0.1.14/src/structures/logger.rs
+-rw-r--r--   0     1001      123     4763 2023-08-06 11:29:49.000000 jlogr-0.1.14/src/structures/logging.rs
+-rw-r--r--   0     1001      123       33 2023-08-06 11:29:49.000000 jlogr-0.1.14/src/structures/mod.rs
+-rw-r--r--   0     1001      123    13667 2023-08-06 11:29:58.000000 jlogr-0.1.14/Cargo.lock
+-rw-r--r--   0        0        0      266 1970-01-01 00:00:00.000000 jlogr-0.1.14/PKG-INFO
```

### Comparing `jlogr-0.1.13/.github/workflows/publish.yml` & `jlogr-0.1.14/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `jlogr-0.1.13/LICENSE` & `jlogr-0.1.14/LICENSE`

 * *Files identical despite different names*

### Comparing `jlogr-0.1.13/src/lib.rs` & `jlogr-0.1.14/src/lib.rs`

 * *Files identical despite different names*

### Comparing `jlogr-0.1.13/src/structures/logger.rs` & `jlogr-0.1.14/src/structures/logger.rs`

 * *Files identical despite different names*

### Comparing `jlogr-0.1.13/src/structures/logging.rs` & `jlogr-0.1.14/src/structures/logging.rs`

 * *Files identical despite different names*

### Comparing `jlogr-0.1.13/Cargo.lock` & `jlogr-0.1.14/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "jlogr"
-version = "0.1.13"
+version = "0.1.14"
 dependencies = [
  "anyhow",
  "chrono",
  "pyo3",
  "termcolor",
 ]
```

