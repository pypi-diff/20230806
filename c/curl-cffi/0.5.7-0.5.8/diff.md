# Comparing `tmp/curl_cffi-0.5.7.tar.gz` & `tmp/curl_cffi-0.5.8-cp37-abi3-macosx_11_0_arm64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curl_cffi-0.5.7.tar", last modified: Tue Jul  4 10:50:13 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

