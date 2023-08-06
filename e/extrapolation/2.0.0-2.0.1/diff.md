# Comparing `tmp/extrapolation-2.0.0.tar.gz` & `tmp/extrapolation-2.0.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extrapolation-2.0.0.tar", last modified: Fri Aug  4 03:58:06 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

