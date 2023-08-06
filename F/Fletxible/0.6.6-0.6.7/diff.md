# Comparing `tmp/Fletxible-0.6.6.tar.gz` & `tmp/Fletxible-0.6.7-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Fletxible-0.6.6.tar", last modified: Sun Aug  6 13:06:48 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

