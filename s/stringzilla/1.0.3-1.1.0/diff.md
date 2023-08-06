# Comparing `tmp/stringzilla-1.0.3-cp39-cp39-win_amd64.whl.zip` & `tmp/stringzilla-1.1.0-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 103121 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat   256000 b- defN 23-Jul-31 07:05 stringzilla.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     4573 b- defN 23-Jul-31 07:05 stringzilla-1.0.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Jul-31 07:05 stringzilla-1.0.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 23-Jul-31 07:05 stringzilla-1.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      404 b- defN 23-Jul-31 07:05 stringzilla-1.0.3.dist-info/RECORD
-5 files, 261089 bytes uncompressed, 102371 bytes compressed:  60.8%
+Zip file size: 114188 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat   283136 b- defN 23-Aug-06 16:59 stringzilla.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     4968 b- defN 23-Aug-06 16:59 stringzilla-1.1.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Aug-06 16:59 stringzilla-1.1.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 23-Aug-06 16:59 stringzilla-1.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      404 b- defN 23-Aug-06 16:59 stringzilla-1.1.0.dist-info/RECORD
+5 files, 288620 bytes uncompressed, 113438 bytes compressed:  60.7%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: stringzilla.cp39-win_amd64.pyd
 Comment: 
 
-Filename: stringzilla-1.0.3.dist-info/METADATA
+Filename: stringzilla-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: stringzilla-1.0.3.dist-info/WHEEL
+Filename: stringzilla-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: stringzilla-1.0.3.dist-info/top_level.txt
+Filename: stringzilla-1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: stringzilla-1.0.3.dist-info/RECORD
+Filename: stringzilla-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `stringzilla-1.0.3.dist-info/METADATA` & `stringzilla-1.1.0.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stringzilla
-Version: 1.0.3
+Version: 1.1.0
 Summary: Crunch 100+ GB Strings in Python with ease
 License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
@@ -92,14 +92,15 @@
 
 Once constructed, the following interfaces are supported:
 
 ```python
 len(text) -> int
 'substring' in text -> bool
 text[42] -> str
+text[42:46] -> str
 
 text.contains(
     'subtring',
     start=0, # optional
     end=9223372036854775807, # optional
 ) -> bool
 
@@ -127,14 +128,29 @@
     separator=' ', # optional
     maxsplit=9223372036854775807, # optional
     **, # non-traditional arguments:
     keepseparator=False, # optional
 ) -> Strs # similar to list[str]
 ```
 
+Once split, you can sort, shuffle, and perform other collection-level operations on strings:
+
+```py
+lines: Strs = text.split(separator='\n')
+lines.sort()
+lines.shuffle(seed=42)
+
+sorted_copy: Strs = lines.sorted()
+shuffled_copy: Strs = lines.shuffled(seed=42)
+
+lines.append(shuffled_copy.pop(0))
+lines.append('Pythonic string')
+lines.extend(shuffled_copy)
+```
+
 ## Development
 
 ```sh
 rm -rf build && pip install -e . && pytest scripts/test.py -s -x
 
 pip install -e . --no-index --no-deps
 ```
```

