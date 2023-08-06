# Comparing `tmp/prettier_prints-1.3.2-py3-none-any.whl.zip` & `tmp/prettier_prints-1.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 2683 bytes, number of entries: 5
--rw-r--r--  2.0 unx     1071 b- defN 23-Aug-03 04:27 prettier_prints-1.3.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     2295 b- defN 23-Aug-03 04:27 prettier_prints-1.3.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Aug-03 04:27 prettier_prints-1.3.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Aug-03 04:27 prettier_prints-1.3.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      425 b- defN 23-Aug-03 04:27 prettier_prints-1.3.2.dist-info/RECORD
-5 files, 3884 bytes uncompressed, 1883 bytes compressed:  51.5%
+Zip file size: 2706 bytes, number of entries: 5
+-rw-r--r--  2.0 unx     1071 b- defN 23-Aug-06 19:18 prettier_prints-1.4.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2328 b- defN 23-Aug-06 19:18 prettier_prints-1.4.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-06 19:18 prettier_prints-1.4.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Aug-06 19:18 prettier_prints-1.4.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      425 b- defN 23-Aug-06 19:18 prettier_prints-1.4.0.dist-info/RECORD
+5 files, 3917 bytes uncompressed, 1906 bytes compressed:  51.3%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
-Filename: prettier_prints-1.3.2.dist-info/LICENSE
+Filename: prettier_prints-1.4.0.dist-info/LICENSE
 Comment: 
 
-Filename: prettier_prints-1.3.2.dist-info/METADATA
+Filename: prettier_prints-1.4.0.dist-info/METADATA
 Comment: 
 
-Filename: prettier_prints-1.3.2.dist-info/WHEEL
+Filename: prettier_prints-1.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: prettier_prints-1.3.2.dist-info/top_level.txt
+Filename: prettier_prints-1.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: prettier_prints-1.3.2.dist-info/RECORD
+Filename: prettier_prints-1.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `prettier_prints-1.3.2.dist-info/LICENSE` & `prettier_prints-1.4.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `prettier_prints-1.3.2.dist-info/METADATA` & `prettier_prints-1.4.0.dist-info/METADATA`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: prettier-prints
-Version: 1.3.2
-Summary: Lightweight library for prettier terminal outputs and debugging similar to chalk for Java
+Version: 1.4.0
+Summary: Lightweight library for prettier terminal outputs and debugging similar to chalk for Javascript
 Author: Dylan Stocking
 License: MIT
 Project-URL: Code Repo, https://github.com/PhantomLeak/prettier_prints
 Project-URL: Bug Tracker, https://github.com/PhantomLeak/prettier_prints/issues
 Keywords: prints,chalk,output
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -19,14 +19,28 @@
 Helping make Python outputs easier to read and styled to your desires.
 
 ### Install
 ```python
 pip install prettier-prints
 ```
 
+Example:
+```python
+    from prettier_prints.prettier_prints import PrettierPrints
+    pp = PrettierPrints()
+    pp.style = 'red;underline'  # <-- Can optionally predefine styling and can be overwritten
+
+    print(pp.out(msg="Lets test the output"))
+    print(pp.out(msg="Lets override the styling here", style="blue;bold"))
+    print(pp.out(print_msg={'msg': 'For those who prefer a JSON object param, this works too'}))
+    print(pp.out(print_msg={'msg': 'Can also overwrite this way', 'style': 'yellow;highlight'}))
+    print(f'Works great for output messages as well -> {pp.out(msg="See :)", style="magenta")}')
+```
+![output image](https://github.com/PhantomLeak/prettier_prints/blob/main/print_output.png?raw=true)
+
 ### Current functions:
  - out()
 
 ### Current available styling:
 | Modifiers | Colors / Background Colors |    
 |:----------|:--------------------------:|
 | Bold      |            Red             |
@@ -40,19 +54,7 @@
 |           |        Bright Green        |
 |           |       Bright Yellow        |
 |           |        Bright Blue         |
 |           |       Bright Magenta       |
 |           |        Bright Cyan         |
 |           |        Bright White        |
 
-
-Example:
-```python
-    from prettier_prints.prettier_prints import PrettierPrints
-    pp = PrettierPrints()
-    print(pp.out({'msg': "Let's turn this message red", 'style': 'red'}))
-    print(pp.out({'msg': "Lets also underline it", 'style': 'red;underline'}))
-    print(pp.out({'msg': "May as well bold it too", 'style': 'red;underline;bold'}))
-    print(pp.out({'msg': "What about a blue background?", 'style': 'blue;highlight'}))
-    print(f'This also works for output messages -> {pp.out(print_msg={"msg": "See :)", "style": "magenta;bold;underline"})}')
-```
-![output image](https://github.com/PhantomLeak/prettier_prints/blob/main/Screenshot%20from%202023-08-02%2023-48-41.png?raw=true)
```

