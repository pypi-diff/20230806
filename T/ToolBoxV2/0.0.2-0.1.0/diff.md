# Comparing `tmp/ToolBoxV2-0.0.2.tar.gz` & `tmp/ToolBoxV2-0.1.0-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ToolBoxV2-0.0.2.tar", last modified: Mon Jan  2 16:20:45 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

