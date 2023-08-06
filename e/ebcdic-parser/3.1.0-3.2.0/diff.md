# Comparing `tmp/ebcdic_parser-3.1.0.tar.gz` & `tmp/ebcdic_parser-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\Projects\ebcdic-parser\dist\.tmp-oqnuh1lu\ebcdic_parser-3.1.0.tar", last modified: Sun Jul 30 14:50:51 2023, max compression
+gzip compressed data, was "D:\Projects\ebcdic-parser\dist\.tmp-t1z0pc84\ebcdic_parser-3.2.0.tar", last modified: Sat Aug  5 03:42:31 2023, max compression
```

## Comparing `ebcdic_parser-3.1.0.tar` & `ebcdic_parser-3.2.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 14:50:51.000000 ebcdic_parser-3.1.0/
--rw-rw-rw-   0        0        0       16 2020-07-12 02:48:58.000000 ebcdic_parser-3.1.0/AUTHORS
--rw-rw-rw-   0        0        0     1066 2020-07-12 02:48:58.000000 ebcdic_parser-3.1.0/LICENSE
--rw-rw-rw-   0        0        0    11978 2023-07-30 14:50:51.000000 ebcdic_parser-3.1.0/PKG-INFO
--rw-rw-rw-   0        0        0    11042 2023-07-30 14:47:33.000000 ebcdic_parser-3.1.0/README.md
--rw-rw-rw-   0        0        0       86 2023-07-18 03:12:01.000000 ebcdic_parser-3.1.0/pyproject.toml
--rw-rw-rw-   0        0        0      783 2023-07-30 14:50:51.000000 ebcdic_parser-3.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-30 14:50:51.000000 ebcdic_parser-3.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-07-30 14:50:51.000000 ebcdic_parser-3.1.0/src/ebcdic_parser/
--rw-rw-rw-   0        0        0        0 2023-07-18 02:52:18.000000 ebcdic_parser-3.1.0/src/ebcdic_parser/__init__.py
--rw-rw-rw-   0        0        0    59241 2023-07-30 14:36:53.000000 ebcdic_parser-3.1.0/src/ebcdic_parser/convert.py
-drwxrwxrwx   0        0        0        0 2023-07-30 14:50:51.000000 ebcdic_parser-3.1.0/src/ebcdic_parser.egg-info/
--rw-rw-rw-   0        0        0    11978 2023-07-30 14:50:51.000000 ebcdic_parser-3.1.0/src/ebcdic_parser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      390 2023-07-30 14:50:51.000000 ebcdic_parser-3.1.0/src/ebcdic_parser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-30 14:50:51.000000 ebcdic_parser-3.1.0/src/ebcdic_parser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-07-30 14:50:51.000000 ebcdic_parser-3.1.0/src/ebcdic_parser.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 14:50:51.000000 ebcdic_parser-3.1.0/tests/
--rw-rw-rw-   0        0        0    17737 2020-07-12 02:48:58.000000 ebcdic_parser-3.1.0/tests/test_functional.py
--rw-rw-rw-   0        0        0     6168 2020-07-12 02:48:58.000000 ebcdic_parser-3.1.0/tests/test_system_311_calls_for_service_requests_all_strings.py
--rw-rw-rw-   0        0        0     5949 2020-07-12 02:48:58.000000 ebcdic_parser-3.1.0/tests/test_system_common.py
+drwxrwxrwx   0        0        0        0 2023-08-05 03:42:31.000000 ebcdic_parser-3.2.0/
+-rw-rw-rw-   0        0        0       16 2020-07-12 02:48:58.000000 ebcdic_parser-3.2.0/AUTHORS
+-rw-rw-rw-   0        0        0     1066 2020-07-12 02:48:58.000000 ebcdic_parser-3.2.0/LICENSE
+-rw-rw-rw-   0        0        0    12308 2023-08-05 03:42:31.000000 ebcdic_parser-3.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0    11372 2023-07-30 15:09:27.000000 ebcdic_parser-3.2.0/README.md
+-rw-rw-rw-   0        0        0       86 2023-07-18 03:12:01.000000 ebcdic_parser-3.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0      783 2023-08-05 03:42:31.000000 ebcdic_parser-3.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-05 03:42:31.000000 ebcdic_parser-3.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-08-05 03:42:31.000000 ebcdic_parser-3.2.0/src/ebcdic_parser/
+-rw-rw-rw-   0        0        0        0 2023-07-18 02:52:18.000000 ebcdic_parser-3.2.0/src/ebcdic_parser/__init__.py
+-rw-rw-rw-   0        0        0       67 2023-08-03 03:22:06.000000 ebcdic_parser-3.2.0/src/ebcdic_parser/__main__.py
+-rw-rw-rw-   0        0        0    59935 2023-08-05 03:40:08.000000 ebcdic_parser-3.2.0/src/ebcdic_parser/convert.py
+drwxrwxrwx   0        0        0        0 2023-08-05 03:42:31.000000 ebcdic_parser-3.2.0/src/ebcdic_parser.egg-info/
+-rw-rw-rw-   0        0        0    12308 2023-08-05 03:42:31.000000 ebcdic_parser-3.2.0/src/ebcdic_parser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      420 2023-08-05 03:42:31.000000 ebcdic_parser-3.2.0/src/ebcdic_parser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 03:42:31.000000 ebcdic_parser-3.2.0/src/ebcdic_parser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-08-05 03:42:31.000000 ebcdic_parser-3.2.0/src/ebcdic_parser.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-05 03:42:31.000000 ebcdic_parser-3.2.0/tests/
+-rw-rw-rw-   0        0        0    17737 2020-07-12 02:48:58.000000 ebcdic_parser-3.2.0/tests/test_functional.py
+-rw-rw-rw-   0        0        0     6168 2020-07-12 02:48:58.000000 ebcdic_parser-3.2.0/tests/test_system_311_calls_for_service_requests_all_strings.py
+-rw-rw-rw-   0        0        0     5949 2020-07-12 02:48:58.000000 ebcdic_parser-3.2.0/tests/test_system_common.py
```

### Comparing `ebcdic_parser-3.1.0/LICENSE` & `ebcdic_parser-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ebcdic_parser-3.1.0/PKG-INFO` & `ebcdic_parser-3.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebcdic_parser
-Version: 3.1.0
+Version: 3.2.0
 Summary: Convert mainframe EBCDIC data into Unicode ASCII delimited text files
 Home-page: https://github.com/larandvit/ebcdic-parser
 Author: Vitaly Saversky
 Author-email: larandvit@hotmail.com
 Project-URL: Bug Tracker, https://github.com/larandvit/ebcdic-parser/issues
 Project-URL: repository, https://github.com/larandvit/ebcdic-parser
 Classifier: Programming Language :: Python :: 3
@@ -26,20 +26,20 @@
  
 Conversion rules are a driver to parse EBCDIC data.
 
 ## Features
 
 * Supported layouts
     1. Single schema
-       * Original [COBOL layout](tests/test_data/pr_p1_p2_gas_disposition/oga0861.pdf) and corresponding [conversion rules](tests/layout_repository/gsf102_rules.json) file
+       * Original [COBOL layout](https://github.com/larandvit/ebcdic-parser/blob/master/tests/test_data/pr_p1_p2_gas_disposition/oga0861.pdf) and corresponding [conversion rules](https://github.com/larandvit/ebcdic-parser/blob/master/tests/layout_repository/gsf102_rules.json) file
     2. Multi-schema fixed record length
-       * Original [COBOL layout](tests/test_data/ola013k/ola013k.pdf) and corresponding [conversion rules](tests/layout_repository/ola013k_rules.json) file
+       * Original [COBOL layout](https://github.com/larandvit/ebcdic-parser/blob/master/tests/test_data/ola013k/ola013k.pdf) and corresponding [conversion rules](https://github.com/larandvit/ebcdic-parser/blob/master/tests/layout_repository/ola013k_rules.json) file
     3. Multi-schema variable record length
     4. Single schema variable record length
-       * Original [COBOL layout](tests/test_data/service_segment_data/129.1DP.pdf) and corresponding [conversion rules](tests/layout_repository/service_segment_data.json) file
+       * Original [COBOL layout](https://github.com/larandvit/ebcdic-parser/blob/master/tests/test_data/service_segment_data/129.1DP.pdf) and corresponding [conversion rules](https://github.com/larandvit/ebcdic-parser/blob/master/tests/layout_repository/service_segment_data.json) file
  
 * Fixing anomalies in EBCDIC files
     1. Skip header
     2. Skip footer
     3. Remove invalid characters
   
 * Adding relationship keys
```

### Comparing `ebcdic_parser-3.1.0/README.md` & `ebcdic_parser-3.2.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -9,20 +9,20 @@
  
 Conversion rules are a driver to parse EBCDIC data.
 
 ## Features
 
 * Supported layouts
     1. Single schema
-       * Original [COBOL layout](tests/test_data/pr_p1_p2_gas_disposition/oga0861.pdf) and corresponding [conversion rules](tests/layout_repository/gsf102_rules.json) file
+       * Original [COBOL layout](https://github.com/larandvit/ebcdic-parser/blob/master/tests/test_data/pr_p1_p2_gas_disposition/oga0861.pdf) and corresponding [conversion rules](https://github.com/larandvit/ebcdic-parser/blob/master/tests/layout_repository/gsf102_rules.json) file
     2. Multi-schema fixed record length
-       * Original [COBOL layout](tests/test_data/ola013k/ola013k.pdf) and corresponding [conversion rules](tests/layout_repository/ola013k_rules.json) file
+       * Original [COBOL layout](https://github.com/larandvit/ebcdic-parser/blob/master/tests/test_data/ola013k/ola013k.pdf) and corresponding [conversion rules](https://github.com/larandvit/ebcdic-parser/blob/master/tests/layout_repository/ola013k_rules.json) file
     3. Multi-schema variable record length
     4. Single schema variable record length
-       * Original [COBOL layout](tests/test_data/service_segment_data/129.1DP.pdf) and corresponding [conversion rules](tests/layout_repository/service_segment_data.json) file
+       * Original [COBOL layout](https://github.com/larandvit/ebcdic-parser/blob/master/tests/test_data/service_segment_data/129.1DP.pdf) and corresponding [conversion rules](https://github.com/larandvit/ebcdic-parser/blob/master/tests/layout_repository/service_segment_data.json) file
  
 * Fixing anomalies in EBCDIC files
     1. Skip header
     2. Skip footer
     3. Remove invalid characters
   
 * Adding relationship keys
```

### Comparing `ebcdic_parser-3.1.0/setup.cfg` & `ebcdic_parser-3.2.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2065 6263 6469 635f 7061 7273 6572   = ebcdic_parser
-00000020: 0d0a 7665 7273 696f 6e20 3d20 332e 312e  ..version = 3.1.
+00000020: 0d0a 7665 7273 696f 6e20 3d20 332e 322e  ..version = 3.2.
 00000030: 300d 0a61 7574 686f 7220 3d20 5669 7461  0..author = Vita
 00000040: 6c79 2053 6176 6572 736b 790d 0a61 7574  ly Saversky..aut
 00000050: 686f 725f 656d 6169 6c20 3d20 6c61 7261  hor_email = lara
 00000060: 6e64 7669 7440 686f 746d 6169 6c2e 636f  ndvit@hotmail.co
 00000070: 6d0d 0a64 6573 6372 6970 7469 6f6e 203d  m..description =
 00000080: 2043 6f6e 7665 7274 206d 6169 6e66 7261   Convert mainfra
 00000090: 6d65 2045 4243 4449 4320 6461 7461 2069  me EBCDIC data i
```

### Comparing `ebcdic_parser-3.1.0/src/ebcdic_parser/convert.py` & `ebcdic_parser-3.2.0/src/ebcdic_parser/convert.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,41 +34,54 @@
 import re
 
 import unicodedata
 
 __author__ = "Vitaly Saversky"
 __date__ = "2017-10-04"
 __credits__ = ["Vitaly Saversky"]
-__version__ = "3.1.0"
+__version__ = "3.2.0"
 __maintainer__ = "Vitaly Saversky"
 __email__ = "larandvit@hotmail.com"
 __status__ = "Production"
 
 class FileFormat(IntEnum):
     SingleSchema = 1
     MultiSchemaFixed = 2
     MultiSchemaVariable = 3
     SingleSchemaVariable = 4
     
+class ParameterDefaults:
+    DELIMITER = "\t"
+    OUTPUTFILEEXTENSION = ".txt"
+    IGNORECONVERSIONERRORS = False
+    VERBOSE = True
+    GROUPRECORDS = False
+    GROUPRECORDSLEVEL2 = False
+    DEBUG_MODE = False
+
+    PYTHONENCODING = True
+    INPUTENCODING = "cp037"
+    OUTPUTENCODING = "utf_8"
+    
 NEWLINE = "\n"
 LOGFILENAME = "ebcdic_parser.log"
 
 SKIPFIELDTYPENAME = 'skip'
 
-DELIMITER = "\t"
-OUTPUTFILEEXTENSION = ".txt"
-IGNORECONVERSIONERRORS = False
-VERBOSE = True
-GROUPRECORDS = False
-GROUPRECORDSLEVEL2 = False
-DEBUG_MODE = False
-
-PYTHONENCODING = True
-INPUTENCODING = "cp037"
-OUTPUTENCODING = "utf_8"
+DELIMITER = ParameterDefaults.DELIMITER
+OUTPUTFILEEXTENSION = ParameterDefaults.OUTPUTFILEEXTENSION
+IGNORECONVERSIONERRORS = ParameterDefaults.IGNORECONVERSIONERRORS
+VERBOSE = ParameterDefaults.VERBOSE
+GROUPRECORDS = ParameterDefaults.GROUPRECORDS
+GROUPRECORDSLEVEL2 = ParameterDefaults.GROUPRECORDSLEVEL2
+DEBUG_MODE = ParameterDefaults.DEBUG_MODE
+
+PYTHONENCODING = ParameterDefaults.PYTHONENCODING
+INPUTENCODING = ParameterDefaults.INPUTENCODING
+OUTPUTENCODING = ParameterDefaults.OUTPUTENCODING
 
 LAYOUTELEMENT_DESCRIPTION = "description"
 LAYOUTELEMENT_KEYFIELDS = "keyfields"
 LAYOUTELEMENT_LAYOUTS = "layouts"
 LAYOUTELEMENT_LAYOUTTYPE = "layouttype"
 LAYOUTELEMENT_LAYOUTTYPECONDITIONAL = "layouttypeconditional"
 LAYOUTELEMENT_LAYOUT = "layout"
@@ -1021,16 +1034,15 @@
         
         # destroy conversion engine. There are resource which have to be released
         if dataConverter!=None:
             dataConverter.release()
                 
         sys.exit(returnCode)
 
-if __name__=="__main__":
-
+def main():
     returnCode = 1
     
     # it will allow don't show print statemnet in finally of catch
     wrongArgumentsFlag = True
     
     try:
         appDescription = "Convert EBCDIC data into delimited text format. Version " + __version__
@@ -1048,24 +1060,24 @@
     
         parser = argparse.ArgumentParser(description=appDescription, 
                                          epilog="Exit codes: 0 - successful completion, 1 - completion with any error",
                                          formatter_class=RawTextHelpFormatter)
         parser.add_argument("--inputfile", nargs=1, required=True, help="Input EBCDIC file path", metavar='"input file path"')
         parser.add_argument("--outputfolder", nargs=1, required=True, help="Output folder to store delimited files", metavar='"output folder"')
         parser.add_argument("--layoutfile", nargs=1, required=True, help="Layout file path", metavar='"layout file"')
-        parser.add_argument("--outputdelimiter", nargs="?", default=DELIMITER, help="output text file delimiter", metavar='delimiter')
-        parser.add_argument("--outputfileextension", nargs="?", default=OUTPUTFILEEXTENSION, help="output text file extension", metavar='extension')
-        parser.add_argument("--ignoreconversionerrors", nargs="?", default="yes" if IGNORECONVERSIONERRORS else "no", choices=["yes","no"], help="ignore any conversion error", metavar='yes/no')
+        parser.add_argument("--outputdelimiter", nargs="?", default=ParameterDefaults.DELIMITER, help="output text file delimiter", metavar='delimiter')
+        parser.add_argument("--outputfileextension", nargs="?", default=ParameterDefaults.OUTPUTFILEEXTENSION, help="output text file extension", metavar='extension')
+        parser.add_argument("--ignoreconversionerrors", nargs="?", default="yes" if ParameterDefaults.IGNORECONVERSIONERRORS else "no", choices=["yes","no"], help="ignore any conversion error", metavar='yes/no')
         parser.add_argument("--logfolder", nargs="?", default="", help="Output folder to store log file", metavar='log folder')
-        parser.add_argument("--pythonencoding", nargs="?", default="yes" if PYTHONENCODING else "no", choices=["yes","no"], help="use Python encoding rather than Java", metavar='yes/no')
-        parser.add_argument("--encodingname", nargs="?", default=INPUTENCODING, help="Code page name to encode characters (Python or Java)", metavar='encoding name')
-        parser.add_argument("--grouprecords", nargs="?", default="yes" if GROUPRECORDS else "no", choices=["yes","no"], help="create relationships between records", metavar='yes/no')
-        parser.add_argument("--grouprecordslevel2", nargs="?", default="yes" if GROUPRECORDSLEVEL2 else "no", choices=["yes","no"], help="create relationships between records for level 2", metavar='yes/no')
-        parser.add_argument("--verbose", nargs="?", default="yes" if VERBOSE else "no", choices=["yes","no"], help="show information on screen", metavar='yes/no')
-        parser.add_argument("--debug", nargs="?", default="yes" if DEBUG_MODE else "no", choices=["yes","no"], help="show debug information", metavar='yes/no')
+        parser.add_argument("--pythonencoding", nargs="?", default="yes" if ParameterDefaults.PYTHONENCODING else "no", choices=["yes","no"], help="use Python encoding rather than Java", metavar='yes/no')
+        parser.add_argument("--encodingname", nargs="?", default=ParameterDefaults.INPUTENCODING, help="Code page name to encode characters (Python or Java)", metavar='encoding name')
+        parser.add_argument("--grouprecords", nargs="?", default="yes" if ParameterDefaults.GROUPRECORDS else "no", choices=["yes","no"], help="create relationships between records", metavar='yes/no')
+        parser.add_argument("--grouprecordslevel2", nargs="?", default="yes" if ParameterDefaults.GROUPRECORDSLEVEL2 else "no", choices=["yes","no"], help="create relationships between records for level 2", metavar='yes/no')
+        parser.add_argument("--verbose", nargs="?", default="yes" if ParameterDefaults.VERBOSE else "no", choices=["yes","no"], help="show information on screen", metavar='yes/no')
+        parser.add_argument("--debug", nargs="?", default="yes" if ParameterDefaults.DEBUG_MODE else "no", choices=["yes","no"], help="show debug information", metavar='yes/no')
     
         args = parser.parse_args()
         wrongArgumentsFlag = False
         
         # mandatory arguments########################################################
         filePath = (current_folder() / args.inputfile[0]).resolve()
         outputFolder = (current_folder() / args.outputfolder[0]).resolve()
@@ -1083,15 +1095,14 @@
         GROUPRECORDSLEVEL2 = True if args.grouprecordslevel2=="yes" else False
         VERBOSE = True if args.verbose=="yes" else False
         DEBUG_MODE = True if args.debug=="yes" else False
         ##############################################################################
         
         sys.stdout = Logger(LOGFILEPATH, VERBOSE)
         fileFolder = path.dirname(filePath)
-        fileName, fileExtension  = path.splitext(path.basename(filePath))
         
         print()
         print("Application version:", __version__)
         print("Stated:", datetime.datetime.now())
         print("Parameters:")
         print("-----------------------------------")
         print(f"Data folder: {fileFolder}")
@@ -1152,7 +1163,11 @@
         
     finally:
         
         if(not wrongArgumentsFlag):
             print("Completed:", datetime.datetime.now())
         
         sys.exit(returnCode)
+
+if __name__=="__main__":
+
+    main()
```

### Comparing `ebcdic_parser-3.1.0/src/ebcdic_parser.egg-info/PKG-INFO` & `ebcdic_parser-3.2.0/src/ebcdic_parser.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebcdic-parser
-Version: 3.1.0
+Version: 3.2.0
 Summary: Convert mainframe EBCDIC data into Unicode ASCII delimited text files
 Home-page: https://github.com/larandvit/ebcdic-parser
 Author: Vitaly Saversky
 Author-email: larandvit@hotmail.com
 Project-URL: Bug Tracker, https://github.com/larandvit/ebcdic-parser/issues
 Project-URL: repository, https://github.com/larandvit/ebcdic-parser
 Classifier: Programming Language :: Python :: 3
@@ -26,20 +26,20 @@
  
 Conversion rules are a driver to parse EBCDIC data.
 
 ## Features
 
 * Supported layouts
     1. Single schema
-       * Original [COBOL layout](tests/test_data/pr_p1_p2_gas_disposition/oga0861.pdf) and corresponding [conversion rules](tests/layout_repository/gsf102_rules.json) file
+       * Original [COBOL layout](https://github.com/larandvit/ebcdic-parser/blob/master/tests/test_data/pr_p1_p2_gas_disposition/oga0861.pdf) and corresponding [conversion rules](https://github.com/larandvit/ebcdic-parser/blob/master/tests/layout_repository/gsf102_rules.json) file
     2. Multi-schema fixed record length
-       * Original [COBOL layout](tests/test_data/ola013k/ola013k.pdf) and corresponding [conversion rules](tests/layout_repository/ola013k_rules.json) file
+       * Original [COBOL layout](https://github.com/larandvit/ebcdic-parser/blob/master/tests/test_data/ola013k/ola013k.pdf) and corresponding [conversion rules](https://github.com/larandvit/ebcdic-parser/blob/master/tests/layout_repository/ola013k_rules.json) file
     3. Multi-schema variable record length
     4. Single schema variable record length
-       * Original [COBOL layout](tests/test_data/service_segment_data/129.1DP.pdf) and corresponding [conversion rules](tests/layout_repository/service_segment_data.json) file
+       * Original [COBOL layout](https://github.com/larandvit/ebcdic-parser/blob/master/tests/test_data/service_segment_data/129.1DP.pdf) and corresponding [conversion rules](https://github.com/larandvit/ebcdic-parser/blob/master/tests/layout_repository/service_segment_data.json) file
  
 * Fixing anomalies in EBCDIC files
     1. Skip header
     2. Skip footer
     3. Remove invalid characters
   
 * Adding relationship keys
```

### Comparing `ebcdic_parser-3.1.0/tests/test_functional.py` & `ebcdic_parser-3.2.0/tests/test_functional.py`

 * *Files identical despite different names*

### Comparing `ebcdic_parser-3.1.0/tests/test_system_311_calls_for_service_requests_all_strings.py` & `ebcdic_parser-3.2.0/tests/test_system_311_calls_for_service_requests_all_strings.py`

 * *Files identical despite different names*

### Comparing `ebcdic_parser-3.1.0/tests/test_system_common.py` & `ebcdic_parser-3.2.0/tests/test_system_common.py`

 * *Files identical despite different names*

