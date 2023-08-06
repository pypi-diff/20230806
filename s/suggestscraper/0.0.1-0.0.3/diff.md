# Comparing `tmp/suggestscraper-0.0.1.tar.gz` & `tmp/suggestscraper-0.0.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "suggestscraper-0.0.1.tar", last modified: Sat Aug  5 00:30:26 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

