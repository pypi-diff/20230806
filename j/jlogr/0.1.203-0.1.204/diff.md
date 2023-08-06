# Comparing `tmp/jlogr-0.1.203.tar.gz` & `tmp/jlogr-0.1.204.tar.gz`

## Comparing `jlogr-0.1.203.tar` & `jlogr-0.1.204.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      484 1970-01-01 00:00:00.000000 jlogr-0.1.203/Cargo.toml
--rw-r--r--   0     1001      123      583 2023-08-06 14:14:26.000000 jlogr-0.1.203/.github/workflows/publish.yml
--rw-r--r--   0     1001      123       42 2023-08-06 14:14:26.000000 jlogr-0.1.203/.gitignore
--rw-r--r--   0     1001      123     1062 2023-08-06 14:14:26.000000 jlogr-0.1.203/LICENSE
--rw-r--r--   0     1001      123      123 2023-08-06 14:14:26.000000 jlogr-0.1.203/README.md
--rw-r--r--   0     1001      123       92 2023-08-06 14:14:26.000000 jlogr-0.1.203/package/jlogr/__init__.py
--rw-r--r--   0     1001      123      403 2023-08-06 14:14:26.000000 jlogr-0.1.203/package/jlogr/jlogr.pyi
--rw-r--r--   0     1001      123        0 2023-08-06 14:14:26.000000 jlogr-0.1.203/package/jlogr/py.typed
--rw-r--r--   0     1001      123      255 2023-08-06 14:14:26.000000 jlogr-0.1.203/pyproject.toml
--rw-r--r--   0     1001      123     4532 2023-08-06 14:14:26.000000 jlogr-0.1.203/src/lib.rs
--rw-r--r--   0     1001      123     2244 2023-08-06 14:14:26.000000 jlogr-0.1.203/src/structures/logger.rs
--rw-r--r--   0     1001      123     4763 2023-08-06 14:14:26.000000 jlogr-0.1.203/src/structures/logging.rs
--rw-r--r--   0     1001      123       33 2023-08-06 14:14:26.000000 jlogr-0.1.203/src/structures/mod.rs
--rw-r--r--   0     1001      123    13668 2023-08-06 14:14:32.000000 jlogr-0.1.203/Cargo.lock
--rw-r--r--   0        0        0      267 1970-01-01 00:00:00.000000 jlogr-0.1.203/PKG-INFO
+-rw-r--r--   0        0        0      484 1970-01-01 00:00:00.000000 jlogr-0.1.204/Cargo.toml
+-rw-r--r--   0     1001      123      583 2023-08-06 14:20:26.000000 jlogr-0.1.204/.github/workflows/publish.yml
+-rw-r--r--   0     1001      123       42 2023-08-06 14:20:26.000000 jlogr-0.1.204/.gitignore
+-rw-r--r--   0     1001      123     1062 2023-08-06 14:20:26.000000 jlogr-0.1.204/LICENSE
+-rw-r--r--   0     1001      123      123 2023-08-06 14:20:26.000000 jlogr-0.1.204/README.md
+-rw-r--r--   0     1001      123       92 2023-08-06 14:20:26.000000 jlogr-0.1.204/package/jlogr/__init__.py
+-rw-r--r--   0     1001      123      565 2023-08-06 14:20:26.000000 jlogr-0.1.204/package/jlogr/jlogr.pyi
+-rw-r--r--   0     1001      123        0 2023-08-06 14:20:26.000000 jlogr-0.1.204/package/jlogr/py.typed
+-rw-r--r--   0     1001      123      255 2023-08-06 14:20:26.000000 jlogr-0.1.204/pyproject.toml
+-rw-r--r--   0     1001      123     4532 2023-08-06 14:20:26.000000 jlogr-0.1.204/src/lib.rs
+-rw-r--r--   0     1001      123     2244 2023-08-06 14:20:26.000000 jlogr-0.1.204/src/structures/logger.rs
+-rw-r--r--   0     1001      123     4763 2023-08-06 14:20:26.000000 jlogr-0.1.204/src/structures/logging.rs
+-rw-r--r--   0     1001      123       33 2023-08-06 14:20:26.000000 jlogr-0.1.204/src/structures/mod.rs
+-rw-r--r--   0     1001      123    13668 2023-08-06 14:20:30.000000 jlogr-0.1.204/Cargo.lock
+-rw-r--r--   0        0        0      267 1970-01-01 00:00:00.000000 jlogr-0.1.204/PKG-INFO
```

### Comparing `jlogr-0.1.203/.github/workflows/publish.yml` & `jlogr-0.1.204/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `jlogr-0.1.203/LICENSE` & `jlogr-0.1.204/LICENSE`

 * *Files identical despite different names*

### Comparing `jlogr-0.1.203/src/lib.rs` & `jlogr-0.1.204/src/lib.rs`

 * *Files identical despite different names*

### Comparing `jlogr-0.1.203/src/structures/logger.rs` & `jlogr-0.1.204/src/structures/logger.rs`

 * *Files identical despite different names*

### Comparing `jlogr-0.1.203/src/structures/logging.rs` & `jlogr-0.1.204/src/structures/logging.rs`

 * *Files identical despite different names*

### Comparing `jlogr-0.1.203/Cargo.lock` & `jlogr-0.1.204/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "jlogr"
-version = "0.1.203"
+version = "0.1.204"
 dependencies = [
  "anyhow",
  "chrono",
  "pyo3",
  "termcolor",
 ]
```

