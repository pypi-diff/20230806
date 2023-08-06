# Comparing `tmp/cougar-0.2.0.tar.gz` & `tmp/cougar-0.2.14-cp39-cp39-manylinux1_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cougar-0.2.0.tar", last modified: Sun Jul 30 13:05:10 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

