# Comparing `tmp/torch_rim-0.2.1.tar.gz` & `tmp/torch_rim-0.2.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_rim-0.2.1.tar", last modified: Sat Aug  5 22:48:34 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

