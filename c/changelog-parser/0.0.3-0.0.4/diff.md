# Comparing `tmp/changelog-parser-0.0.3.tar.gz` & `tmp/changelog-parser-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "changelog-parser-0.0.3.tar", last modified: Wed Aug  2 16:34:53 2023, max compression
+gzip compressed data, was "changelog-parser-0.0.4.tar", last modified: Sun Aug  6 14:16:02 2023, max compression
```

## Comparing `changelog-parser-0.0.3.tar` & `changelog-parser-0.0.4.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:34:53.665889 changelog-parser-0.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:34:53.661889 changelog-parser-0.0.3/.github/
--rwxr-xr-x   0 runner    (1001) docker     (123)       16 2023-08-02 16:34:42.000000 changelog-parser-0.0.3/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:34:53.661889 changelog-parser-0.0.3/.github/workflows/
--rwxr-xr-x   0 runner    (1001) docker     (123)      498 2023-08-02 16:34:42.000000 changelog-parser-0.0.3/.github/workflows/publish.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)     2371 2023-08-02 16:34:42.000000 changelog-parser-0.0.3/.github/workflows/pull_request_checks.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-08-02 16:34:42.000000 changelog-parser-0.0.3/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (123)      687 2023-08-02 16:34:42.000000 changelog-parser-0.0.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-02 16:34:42.000000 changelog-parser-0.0.3/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (123)      673 2023-08-02 16:34:42.000000 changelog-parser-0.0.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-08-02 16:34:53.665889 changelog-parser-0.0.3/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     1926 2023-08-02 16:34:42.000000 changelog-parser-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:34:53.665889 changelog-parser-0.0.3/changelog_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-08-02 16:34:53.000000 changelog-parser-0.0.3/changelog_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-08-02 16:34:53.000000 changelog-parser-0.0.3/changelog_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 16:34:53.000000 changelog-parser-0.0.3/changelog_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-02 16:34:53.000000 changelog-parser-0.0.3/changelog_parser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-02 16:34:53.000000 changelog-parser-0.0.3/changelog_parser.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1384 2023-08-02 16:34:42.000000 changelog-parser-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 16:34:53.665889 changelog-parser-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:34:53.665889 changelog-parser-0.0.3/src/
--rwxr-xr-x   0 runner    (1001) docker     (123)     8846 2023-08-02 16:34:42.000000 changelog-parser-0.0.3/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:34:53.665889 changelog-parser-0.0.3/test/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1205 2023-08-02 16:34:42.000000 changelog-parser-0.0.3/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:34:53.661889 changelog-parser-0.0.3/test/projects/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:34:53.665889 changelog-parser-0.0.3/test/projects/example/
--rwxr-xr-x   0 runner    (1001) docker     (123)     8039 2023-08-02 16:34:42.000000 changelog-parser-0.0.3/test/projects/example/CHANGELOG.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     5078 2023-08-02 16:34:42.000000 changelog-parser-0.0.3/test/test_load.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:16:02.043758 changelog-parser-0.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:16:02.039758 changelog-parser-0.0.4/.github/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       16 2023-08-06 14:15:49.000000 changelog-parser-0.0.4/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:16:02.039758 changelog-parser-0.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     5713 2023-08-06 14:15:49.000000 changelog-parser-0.0.4/.github/workflows/changelog_checks.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      543 2023-08-06 14:15:49.000000 changelog-parser-0.0.4/.github/workflows/publish.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3327 2023-08-06 14:15:49.000000 changelog-parser-0.0.4/.github/workflows/testing.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-08-06 14:15:49.000000 changelog-parser-0.0.4/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (123)      902 2023-08-06 14:15:49.000000 changelog-parser-0.0.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-06 14:15:49.000000 changelog-parser-0.0.4/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1086 2023-08-06 14:15:49.000000 changelog-parser-0.0.4/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-08-06 14:16:02.043758 changelog-parser-0.0.4/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1863 2023-08-06 14:15:49.000000 changelog-parser-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:16:02.039758 changelog-parser-0.0.4/changelog_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-08-06 14:16:02.000000 changelog-parser-0.0.4/changelog_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-08-06 14:16:02.000000 changelog-parser-0.0.4/changelog_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 14:16:02.000000 changelog-parser-0.0.4/changelog_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-06 14:16:02.000000 changelog-parser-0.0.4/changelog_parser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-06 14:16:02.000000 changelog-parser-0.0.4/changelog_parser.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1718 2023-08-06 14:15:49.000000 changelog-parser-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 14:16:02.043758 changelog-parser-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:16:02.039758 changelog-parser-0.0.4/src/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12244 2023-08-06 14:15:49.000000 changelog-parser-0.0.4/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:16:02.039758 changelog-parser-0.0.4/test/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1205 2023-08-06 14:15:49.000000 changelog-parser-0.0.4/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:16:02.039758 changelog-parser-0.0.4/test/projects/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:16:02.043758 changelog-parser-0.0.4/test/projects/example/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8039 2023-08-06 14:15:49.000000 changelog-parser-0.0.4/test/projects/example/CHANGELOG.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6611 2023-08-06 14:15:49.000000 changelog-parser-0.0.4/test/test_load.py
```

### Comparing `changelog-parser-0.0.3/.gitignore` & `changelog-parser-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `changelog-parser-0.0.3/LICENSE` & `changelog-parser-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `changelog-parser-0.0.3/PKG-INFO` & `changelog-parser-0.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: changelog-parser
-Version: 0.0.3
+Version: 0.0.4
 Summary: Parses changelog files
 Author-email: Jason Stiefel <Jason.R.Stiefel@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 JasonStiefel
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -63,16 +63,15 @@
    {
      "$schema": "https://json-schema.org/draft-07/schema#",
      "title": "Loaded Changelog",
      "type": "object",
      "properties": {
        "version": {
          "oneOf": [ {
-           "type": "string",
-           "pattern": "^[Uu][Nn][Rr][Ee][Ll][Ee][Aa][Ss][Ee][Dd]$"
+           "const": "Unreleased"
          }, {
            "type": "semver.Version",
            "description": "Python object from https://pypi.org/project/semver/"
          } ]
        },
        "date": {
          "oneOf": [ {
```

### Comparing `changelog-parser-0.0.3/README.md` & `changelog-parser-0.0.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -19,16 +19,15 @@
    {
      "$schema": "https://json-schema.org/draft-07/schema#",
      "title": "Loaded Changelog",
      "type": "object",
      "properties": {
        "version": {
          "oneOf": [ {
-           "type": "string",
-           "pattern": "^[Uu][Nn][Rr][Ee][Ll][Ee][Aa][Ss][Ee][Dd]$"
+           "const": "Unreleased"
          }, {
            "type": "semver.Version",
            "description": "Python object from https://pypi.org/project/semver/"
          } ]
        },
        "date": {
          "oneOf": [ {
```

### Comparing `changelog-parser-0.0.3/changelog_parser.egg-info/PKG-INFO` & `changelog-parser-0.0.4/changelog_parser.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: changelog-parser
-Version: 0.0.3
+Version: 0.0.4
 Summary: Parses changelog files
 Author-email: Jason Stiefel <Jason.R.Stiefel@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 JasonStiefel
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -63,16 +63,15 @@
    {
      "$schema": "https://json-schema.org/draft-07/schema#",
      "title": "Loaded Changelog",
      "type": "object",
      "properties": {
        "version": {
          "oneOf": [ {
-           "type": "string",
-           "pattern": "^[Uu][Nn][Rr][Ee][Ll][Ee][Aa][Ss][Ee][Dd]$"
+           "const": "Unreleased"
          }, {
            "type": "semver.Version",
            "description": "Python object from https://pypi.org/project/semver/"
          } ]
        },
        "date": {
          "oneOf": [ {
```

### Comparing `changelog-parser-0.0.3/pyproject.toml` & `changelog-parser-0.0.4/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -32,22 +32,42 @@
 ]
 
 [tool.setuptools.dynamic]
 version = { attr = "changelog.__version__" }
 
 [project.optional-dependencies]
 test = [
-  "pytest",
   "coverage",
+  "pylint",
+  "pytest",
   "pytest-xdist"
 ]
 
+[tool.setuptools.package-dir]
+changelog = "src"
+
 [tool.pytest.ini_options]
 log_cli_level = "info"
 testpaths = [ "test" ]
 
 [tool.coverage.run]
 branch = true
 source_pkgs = [ "changelog" ]
 
-[tool.setuptools.package-dir]
-changelog = "src"
+[tool.coverage.report]
+fail_under = 95
+
+[tool.pylint.main]
+recursive = true
+good-names = [ "e", "s", "fp" ]
+fail-on = [ "error" ]
+fail-under = 9.5
+
+[tool.pylint."messages control"]
+disable = [
+  "too-many-branches",
+  "too-many-statements",
+  "unnecessary-lambda-assignment"
+]
+
+[tool.pylint.format]
+max-line-length = 110
```

### Comparing `changelog-parser-0.0.3/src/__init__.py` & `changelog-parser-0.0.4/src/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,28 @@
 # SPDX-License-Identifier: MIT
 
-__version__ = '0.0.3'
+"""
+A tool for managing changelog formatted data and objects (see
+keepachangelog.com). In Python, the data is managed as a list of
+dictionaries (see README.md for the dictionaries' structure)
+"""
+
+__version__ = '0.0.4'
 
 import re
+import textwrap
 from datetime import date
-from semver import Version
 from typing import ( Optional, Any )
-from io import ( IOBase, StringIO )
+from io import ( IOBase, TextIOBase, StringIO )
+from semver import Version
 
 class ChangelogParsingError( Exception ):
+    """
+    An error used when changelog data isn't formatted as the parser expects
+    """
     @property
     def line_number( self )-> Optional[ int ]:
         """
         Parse the line number from the error message, if defined
         """
         if ( match := re.search( r' \(at line (\d+)(?:, column \d+)?\)$', str( self ) ) ):
             return int( match.group( 1 ) )
@@ -45,17 +55,17 @@
     while ( line := fp.readline() ):
         line_no += 1
         if isinstance( line, bytes ):
             try:
                 line = line.decode( encoding )
             except Exception as e:
                 raise ChangelogParsingError(
-                    msg = f'Unable to decode line using encoding, "{ encoding }"; { e }',
+                    msg = f'Unable to decode line using encoding, "{ encoding }"',
                     line_number = line_no
-                )
+                ) from e
         if isinstance( line, str ):
             line = line.removesuffix( '\n' )
         else:
             raise ChangelogParsingError(
                 f'Parameter\'s "readline" function call returned unreadable type, "{ type( line ).__name__ }"'
             )
 
@@ -91,18 +101,18 @@
                     column_number = line.find( "]" ) + 2
                 )
             if sep:
                 try:
                     changes[ -1 ][ "date" ] = date.fromisoformat( change_date )
                 except Exception as e:
                     raise ChangelogParsingError(
-                        msg = f'Unable to parse changelog entry date, "{ change_date }"; { e }',
+                        msg = f'Unable to parse changelog entry date, "{ change_date }"',
                         line_number = line_no,
                         column_number = len( line + sep ) + 1
-                    )
+                    ) from e
 
             if line.rstrip() != line:
                 raise ChangelogParsingError(
                     msg = "Extra space(s) after version",
                     line_number = line_no,
                     column_number = len( line.rstrip() ) + 1
                 )
@@ -113,18 +123,25 @@
             if not line.startswith( "[" ) or not line.endswith( "]" ):
                 raise ChangelogParsingError(
                     msg = 'Version must be enclosed with square brackets',
                     line_number = line_no,
                     column_number = 4 if not line.startswith( "[" ) else 4 + len( line )
                 )
             line = line.removeprefix( "[" ).removesuffix( "]" )
-            try:
-                changes[ -1 ][ "version" ] = line if line.lower() == "unreleased" else Version.parse( line )
-            except Exception as e:
-                raise ChangelogParsingError( f'Failed parsing semver version, "{ line }"; { e }', line_no, 5 )
+            if line.lower() == "unreleased":
+                changes[ -1 ][ "version" ] = line.capitalize()
+            else:
+                try:
+                    changes[ -1 ][ "version" ] = Version.parse( line )
+                except Exception as e:
+                    raise ChangelogParsingError(
+                        msg = f'Failed parsing semver version, "{ line }"',
+                        line_number = line_no,
+                        column_number = 5
+                    ) from e
 
         elif not changes:
             continue
 
         elif line.startswith( '### ' ) and not in_compare_urls:
             if section is not None and changes[ -1 ][ section ]:
                 changes[ -1 ][ section ][ -1 ] = changes[ -1 ][ section ][ -1 ].rstrip()
@@ -142,28 +159,28 @@
             changes[ -1 ][ section ].append( line[ 2 : ] )
 
         elif ( line.startswith( "  " ) or not line ) and section is not None and changes[ -1 ][ section ]:
             changes[ -1 ][ section ][ -1 ] += "\n" + line.removeprefix( "  " )
 
         elif ( match := re.fullmatch( r'\[([^\]]+)\]: (https?:\/\/.*)', line ) ):
             if match.group( 1 ).lower() == "unreleased":
-                version = match.group( 1 )
+                version = match.group( 1 ).capitalize()
             else:
                 try:
                     version = Version.parse( match.group( 1 ) )
                 except Exception as e:
                     raise ChangelogParsingError(
-                        msg = f'Failed parsing semver version, "{ match.group( 1 ) }"; { e }',
+                        msg = f'Failed parsing semver version, "{ match.group( 1 ) }"',
                         line_number = line_no,
                         column_number = 2
-                    )
+                    ) from e
 
             for change in changes:
                 if isinstance( change[ "version" ], str ) and isinstance( version, str ):
-                    if change[ "version" ].lower() == version.lower():
+                    if change[ "version" ] == version:
                         break
                 if isinstance( change[ "version" ], Version ) and isinstance( version, Version ):
                     if change[ "version" ] == version:
                         break
             else:
                 raise ChangelogParsingError(
                     msg = f'No corresponding record for compare url with version, "{ match.group( 1 ) }"',
@@ -175,38 +192,100 @@
             in_compare_urls = True
 
         elif not line:
             continue
 
         elif in_compare_urls:
             raise ChangelogParsingError(
-                f'After compare URL definitions have started, no other line types are allowed',
+                'After compare URL definitions have started, no other line types are allowed',
                 line_number = line_no
             )
 
         else:
             raise ChangelogParsingError( f'Unrecognized line pattern, "{ line }"', line_no )
 
     if section is not None and changes[ -1 ][ section ]:
         changes[ -1 ][ section ][ -1 ] = changes[ -1 ][ section ][ -1 ].rstrip()
 
     return changes
 
-def loads( input: str )-> list[ dict[ str, Any ] ]:
+def loads( s: str )-> list[ dict[ str, Any ] ]:
     """
     Parse data from a changelog provided as a string
 
     :param input: the string parse as a changelog
     :return: a list of dictionaries with changelog data (see README.md for structure)
     """
-    return load( StringIO( input ) )
+    return load( StringIO( s ) )
+
+DEFAULT_HEADER = """
+# Changelog
+
+All notable changes to this project will be documented in this file.
+
+The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
+and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
+""".strip()
+
+def dump(   obj: list[ dict[ str, Any ] ],
+            fp: IOBase,
+            header: str = DEFAULT_HEADER,
+            encoding: str = 'utf-8'
+        )-> None:
+    """
+    Format and write changelog data to a stream
 
+    :param obj: the changelog data to format and write (see README.md for structure)
+    :param fp: stream to write the changelog data to
+    :param header: head text to add before changelog data
+    :param encoding: if the stream expects binary data, decode string data with this encoding
+    """
+    if not isinstance( obj, list ) or any( not isinstance( i, dict ) for i in obj ):
+        raise ValueError( '"obj" parameter must be a list of dictionaries' )
+    encode = lambda i : i if isinstance( fp, TextIOBase ) else i.encode( encoding )
+    fp.writelines( encode( header + "\n" ).splitlines( keepends = True ) )
+    for number, change in enumerate( obj, start = 1 ):
+        if "version" not in change:
+            raise ValueError( f'Changelog entry #{ number } was missing a "version" key' )
+        line = f'## [{ change[ "version" ] }]'
+        if isinstance( change.get( "date" ), date ):
+            line += " - " + change[ "date" ].isoformat()
+        if change.get( "yanked", False ):
+            line += " [YANKED]"
+        fp.writelines( ( encode( i ) for i in ( "\n", line + "\n" ) ) )
+        for key in change.keys():
+            if key in ( 'added', 'changed', 'deprecated', 'removed', 'fixed', 'security' ):
+                fp.writelines( ( encode( i ) for i in ( "\n", f'### { key.capitalize() }' + "\n" ) ) )
+                if isinstance( change[ key ], list ):
+                    fp.writelines( ( encode( i ) for i in ( "\n" ) ) )
+                    for item in change[ key ]:
+                        fp.writelines( ( encode( "-" + textwrap.indent( item, "  " )[ 1 : ] + "\n" ), ) )
+    if any( "compare_url" in change for change in obj ):
+        fp.writelines( ( encode( i ) for i in ( "\n" ) ) )
+    for change in obj:
+        if "compare_url" in change:
+            fp.writelines( ( encode( f'[{ change[ "version" ] }]: { change[ "compare_url" ] }\n' ), ) )
+
+def dumps( obj: list[ dict[ str, Any ] ], header: str = DEFAULT_HEADER )-> str:
+    """
+    Format and write changelog data to a string
+
+    :param obj: the changelog data to format and write (see README.md for structure)
+    :param header: head text to add before changelog data
+    :return: the changelog file as a string
+    """
+    stream = StringIO()
+    dump( obj, stream, header = header )
+    stream.seek( 0 )
+    return stream.read()
 
 __all__ = [
     '__version__',
     'ChangelogParsingError',
     'load',
-    'loads'
+    'loads',
+    'dump',
+    'dumps'
 ]
 
 def __dir__() -> list[str]:
     return __all__
```

### Comparing `changelog-parser-0.0.3/test/conftest.py` & `changelog-parser-0.0.4/test/conftest.py`

 * *Files identical despite different names*

### Comparing `changelog-parser-0.0.3/test/projects/example/CHANGELOG.md` & `changelog-parser-0.0.4/test/projects/example/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `changelog-parser-0.0.3/test/test_load.py` & `changelog-parser-0.0.4/test/test_load.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+import tempfile
+import os
 import changelog
 import pytest
 import semver
+from difflib import Differ
 from datetime import date
 
-def test_example( project_example_changelog_path ):
+def test_spot_check( project_example_changelog_path ):
     with open( project_example_changelog_path, "rb" ) as fp:
         changes = changelog.load( fp )
 
     assert len( changes ) == 15
 
     min_keys = { "version", "date", "yanked" }
     max_keys = min_keys | { "added", "changed", "depreciated", "removed", "fixed", "security", "compare_url" }
@@ -18,59 +21,83 @@
         "version": semver.Version( 0, 0, 2 ),
         "date": date( 2014, 7, 10 ),
         "yanked": False,
         "added": [ "Explanation of the recommended reverse chronological release ordering." ],
         "compare_url": "https://github.com/olivierlacan/keep-a-changelog/compare/v0.0.1...v0.0.2"
     }
 
+def test_write( project_example_changelog_path ):
+    with open( project_example_changelog_path, "rb" ) as fp:
+        changes = changelog.load( fp )
+
+    path, differ = tempfile.mktemp(), Differ()
+    try:
+        with open( path, 'wb' ) as fp:
+            changelog.dump( changes, fp )
+
+        with open( path, 'r' ) as fp:
+            print( fp.read() )
+
+        with open( path, 'r' ) as w_fp, open( project_example_changelog_path, 'r' ) as r_fp:
+            diffs = []
+            for line in differ.compare( w_fp.readlines(), r_fp.readlines() ):
+                if not line.startswith( "  " ):
+                    diffs.append( line )
+            assert diffs == [
+                '- [Unreleased]: https://github.com/olivierlacan/keep-a-changelog/compare/v1.1.1...HEAD\n',
+                '?  ^\n',
+                '+ [unreleased]: https://github.com/olivierlacan/keep-a-changelog/compare/v1.1.1...HEAD\n',
+                '?  ^\n'
+            ]
+    finally:
+        os.remove( path )
+
 @pytest.mark.parametrize(
     ( "changelog_contents", "error_message", "msg_line_no", "msg_col_no" ),
     [
         ( "## [1.1.1] - 2023-03-05 [YANKED] ", "Extra space(s) at end of line (at line 1, column 33)", 1, 33 ),
         ( "## [1.1.1] - 2023-03-05  [YANKED]", "Extra space(s) after date (at line 1, column 24)", 1, 24 ),
-        ( "## [1.1.1] - 2023-03-05 [ASDF]", 'Unable to parse changelog entry date, "2023-03-05 [ASDF]"; '
-            'Invalid isoformat string: \'2023-03-05 [ASDF]\' (at line 1, column 14)', 1, 14 ),
+        ( "## [1.1.1] - 2023-03-05 [ASDF]", 'Unable to parse changelog entry date, "2023-03-05 [ASDF]" '
+            '(at line 1, column 14)', 1, 14 ),
         ( "## [1.1.1] - 2023-03-05 ", "Extra space(s) at end of line (at line 1, column 24)", 1, 24 ),
-        ( "## [1.1.1] - hjksdgfwiuehf", 'Unable to parse changelog entry date, "hjksdgfwiuehf"; '
-            'Invalid isoformat string: \'hjksdgfwiuehf\' (at line 1, column 14)', 1, 14 ),
+        ( "## [1.1.1] - hjksdgfwiuehf", 'Unable to parse changelog entry date, "hjksdgfwiuehf" '
+            '(at line 1, column 14)', 1, 14 ),
         ( "## [1.1.1] -  2023-03-05", "Extra space(s) before date (at line 1, column 14)", 1, 14 ),
         ( "## [1.1.1] 2023-03-05", 'Version and date must be separated by " - " (at line 1, column 11)', 1, 11 ),
         ( "## [1.1.1]  - 2023-03-05", "Extra space(s) after version (at line 1, column 11)", 1, 11 ),
         ( "## [1.1.1] ", "Extra space(s) at end of line (at line 1, column 11)", 1, 11 ),
         ( "## [1.1.1", "Version must be enclosed with square brackets (at line 1, column 10)", 1, 10 ),
         ( "## 1.1.1]", "Version must be enclosed with square brackets (at line 1, column 4)", 1, 4 ),
         ( "##  [1.1.1] - 2023-03-05", 'Extra space(s) before version (at line 1, column 4)', 1, 4 ),
-        ( "## [asdfasdf]", 'Failed parsing semver version, "asdfasdf"; asdfasdf is not valid SemVer '
-            'string (at line 1, column 5)', 1, 5 ),
+        ( "## [asdfasdf]", 'Failed parsing semver version, "asdfasdf" '
+            '(at line 1, column 5)', 1, 5 ),
         ( "## [Unreleased]\nasdf", 'Unrecognized line pattern, "asdf" (at line 2)', 2, None ),
         ( "## [Unreleased]\n### asdf", 'Invalid change type, "asdf" (at line 2, column 5)', 2, 5 ),
         ( "## [Unreleased]\n\n### asdf", 'Invalid change type, "asdf" (at line 3, column 5)', 3, 5 ),
         ( "## [Unreleased]\n\n- Change", 'Change not under a category section (at line 3)', 3, None ),
         ( "## [Unreleased]\n\n### Added\n\n### Added", 'Multiple "Added" sections found (at line 5, column 5)', 5, 5 ),
         ( '## [Unreleased]\n\n[1.1.1]: https://asdf', 'No corresponding record for compare url with version, '
             '"1.1.1" (at line 3, column 2)', 3, 2 ),
-        ( '## [Unreleased]\n\n[1.a.1]: https://asdf', 'Failed parsing semver version, "1.a.1"; 1.a.1 is '
-            'not valid SemVer string (at line 3, column 2)', 3, 2 ),
+        ( '## [Unreleased]\n\n[1.a.1]: https://asdf', 'Failed parsing semver version, "1.a.1" '
+            '(at line 3, column 2)', 3, 2 ),
         ( '## [1.1.1]\n\n[1.1.1]: https://asdf\n\n## [Unreleased]', 'After compare URL definitions have started, '
             'no other line types are allowed (at line 5)', 5, None )
     ] )
+
 def test_basic_error_line_patterns( changelog_contents, error_message, msg_line_no, msg_col_no ):
     try:
         changelog.loads( changelog_contents )
     except Exception as e:
         assert isinstance( e, changelog.ChangelogParsingError )
         assert str( e ) == error_message
         assert e.line_number == msg_line_no
         assert e.column_number == msg_col_no
     else:
         pytest.fail( "Loading CHANGELOG did not raise an exception" )
 
-def test_dir():
-    assert "__version__" in changelog.__dir__()
-
 def test_invalid_streams( numerical_stream ):
     try:
         changelog.load( numerical_stream )
     except Exception as e:
         assert isinstance( e, changelog.ChangelogParsingError )
         assert str( e ) == 'Parameter\'s "readline" function call returned unreadable type, "int"'
         assert e.line_number is None
@@ -79,13 +106,34 @@
         pytest.fail( "Loading invalid stream did not raise an exception" )
 
 def test_non_utf_8_input_object( non_utf8_stream ):
     try:
         changelog.load( non_utf8_stream )
     except Exception as e:
         assert isinstance( e, changelog.ChangelogParsingError )
-        assert str( e ) == ( 'Unable to decode line using encoding, "utf-8"; \'utf-8\' codec '
-            'can\'t decode byte 0xff in position 0: invalid start byte (at line 1)' )
+        assert str( e ) == ( 'Unable to decode line using encoding, "utf-8" (at line 1)' )
         assert e.line_number == 1
         assert e.column_number is None
     else:
-        pytest.fail( "Loading non-utf-8 stream did not raise an exception" )
+        pytest.fail( "Loading non-utf-8 stream did not raise an exception" )
+
+def test_save_yanked_version():
+    expected = changelog.DEFAULT_HEADER + "\n\n## [Unreleased] [YANKED]\n"
+    assert changelog.dumps( [ { "version": "Unreleased", "yanked": True } ] ) == expected
+
+@pytest.mark.parametrize(
+    ( "changelog_object", "error_message" ),
+    [
+        ( "asdf", '"obj" parameter must be a list of dictionaries' ),
+        ( [{}], 'Changelog entry #1 was missing a "version" key' )
+    ] )
+def test_bad_output( changelog_object, error_message ):
+    try:
+        changelog.dumps( changelog_object )
+    except Exception as e:
+        assert isinstance( e, ValueError )
+        assert str( e ) == error_message
+    else:
+        pytest.fail( f'Expected dumping the following to fail: { changelog_object }' )
+
+def test_dir():
+    assert "__version__" in changelog.__dir__()
```

