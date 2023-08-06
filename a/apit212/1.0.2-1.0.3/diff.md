# Comparing `tmp/apit212-1.0.2.tar.gz` & `tmp/apit212-1.0.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apit212-1.0.2.tar", last modified: Fri Jul 28 13:33:38 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

