# Comparing `tmp/soagen-0.3.0.tar.gz` & `tmp/soagen-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soagen-0.3.0.tar", last modified: Fri Aug  4 16:22:18 2023, max compression
+gzip compressed data, was "soagen-0.4.0.tar", last modified: Sun Aug  6 15:06:20 2023, max compression
```

## Comparing `soagen-0.3.0.tar` & `soagen-0.4.0.tar`

### file list

```diff
@@ -1,60 +1,63 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 16:22:18.651346 soagen-0.3.0/
--rw-rw-rw-   0        0        0      751 2023-08-04 16:21:27.000000 soagen-0.3.0/CHANGELOG.md
--rw-rw-rw-   0        0        0     1064 2023-07-21 10:29:49.000000 soagen-0.3.0/LICENSE.txt
--rw-rw-rw-   0        0        0     2087 2023-08-04 16:22:18.650346 soagen-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0      466 2023-07-30 08:46:14.000000 soagen-0.3.0/README.md
--rw-rw-rw-   0        0        0     1893 2023-08-03 12:48:33.000000 soagen-0.3.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-04 16:22:18.651346 soagen-0.3.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-08-04 16:22:18.606346 soagen-0.3.0/src/
-drwxrwxrwx   0        0        0        0 2023-08-04 16:22:18.629346 soagen-0.3.0/src/soagen/
--rw-rw-rw-   0        0        0      477 2023-07-29 16:15:31.000000 soagen-0.3.0/src/soagen/__init__.py
--rw-rw-rw-   0        0        0      870 2023-07-30 13:58:17.000000 soagen-0.3.0/src/soagen/column.py
--rw-rw-rw-   0        0        0     5264 2023-08-04 15:13:48.000000 soagen-0.3.0/src/soagen/config.py
--rw-rw-rw-   0        0        0      952 2023-07-29 16:15:31.000000 soagen-0.3.0/src/soagen/configurable.py
--rw-rw-rw-   0        0        0    19130 2023-08-01 16:02:29.000000 soagen-0.3.0/src/soagen/cpp.py
--rw-rw-rw-   0        0        0      574 2023-07-29 16:15:31.000000 soagen-0.3.0/src/soagen/errors.py
--rw-rw-rw-   0        0        0    11685 2023-08-04 15:13:48.000000 soagen-0.3.0/src/soagen/header_file.py
-drwxrwxrwx   0        0        0        0 2023-08-04 16:22:18.646349 soagen-0.3.0/src/soagen/hpp/
--rw-rw-rw-   0        0        0     5693 2023-08-04 16:20:02.000000 soagen-0.3.0/src/soagen/hpp/.clang-format
--rw-rw-rw-   0        0        0    11287 2023-07-29 16:15:31.000000 soagen-0.3.0/src/soagen/hpp/allocator.hpp
--rw-rw-rw-   0        0        0    32796 2023-08-04 15:13:48.000000 soagen-0.3.0/src/soagen/hpp/column_traits.hpp
--rw-rw-rw-   0        0        0    29618 2023-08-04 15:13:48.000000 soagen-0.3.0/src/soagen/hpp/core.hpp
-drwxrwxrwx   0        0        0        0 2023-08-04 16:22:18.649346 soagen-0.3.0/src/soagen/hpp/generated/
--rw-rw-rw-   0        0        0     9858 2023-08-04 16:20:03.000000 soagen-0.3.0/src/soagen/hpp/generated/compressed_pair.hpp
--rw-rw-rw-   0        0        0     6006 2023-08-04 16:20:03.000000 soagen-0.3.0/src/soagen/hpp/generated/functions.hpp
--rw-rw-rw-   0        0        0    43899 2023-08-04 16:20:05.000000 soagen-0.3.0/src/soagen/hpp/generated/preprocessor.hpp
--rw-rw-rw-   0        0        0      420 2023-08-03 12:44:35.000000 soagen-0.3.0/src/soagen/hpp/generated/version.hpp
--rw-rw-rw-   0        0        0      816 2023-07-29 16:15:31.000000 soagen-0.3.0/src/soagen/hpp/header_end.hpp
--rw-rw-rw-   0        0        0      929 2023-07-29 16:15:31.000000 soagen-0.3.0/src/soagen/hpp/header_start.hpp
--rw-rw-rw-   0        0        0    15734 2023-08-01 12:49:39.000000 soagen-0.3.0/src/soagen/hpp/iterator.hpp
--rw-rw-rw-   0        0        0     5469 2023-08-04 15:13:48.000000 soagen-0.3.0/src/soagen/hpp/mixins.hpp
--rw-rw-rw-   0        0        0     7841 2023-08-04 15:13:48.000000 soagen-0.3.0/src/soagen/hpp/row.hpp
-drwxrwxrwx   0        0        0        0 2023-08-04 16:22:18.649346 soagen-0.3.0/src/soagen/hpp/single/
--rw-rw-rw-   0        0        0   233911 2023-08-04 16:21:27.000000 soagen-0.3.0/src/soagen/hpp/single/soagen.hpp
--rw-rw-rw-   0        0        0      979 2023-07-29 16:15:31.000000 soagen-0.3.0/src/soagen/hpp/soagen.hpp
--rw-rw-rw-   0        0        0    56712 2023-08-01 18:52:09.000000 soagen-0.3.0/src/soagen/hpp/table.hpp
--rw-rw-rw-   0        0        0    34607 2023-08-04 16:21:27.000000 soagen-0.3.0/src/soagen/hpp/table_traits.hpp
--rw-rw-rw-   0        0        0     1067 2023-07-30 13:01:18.000000 soagen-0.3.0/src/soagen/includes.py
--rw-rw-rw-   0        0        0     1534 2023-08-01 12:05:38.000000 soagen-0.3.0/src/soagen/injectors.py
--rw-rw-rw-   0        0        0     3926 2023-07-29 16:15:31.000000 soagen-0.3.0/src/soagen/log.py
--rw-rw-rw-   0        0        0    22644 2023-08-04 15:13:48.000000 soagen-0.3.0/src/soagen/main.py
--rw-rw-rw-   0        0        0     3529 2023-08-04 15:13:48.000000 soagen-0.3.0/src/soagen/metavars.py
--rw-rw-rw-   0        0        0     6453 2023-08-04 15:13:48.000000 soagen-0.3.0/src/soagen/natvis_file.py
--rw-rw-rw-   0        0        0     1971 2023-07-29 16:15:31.000000 soagen-0.3.0/src/soagen/paths.py
--rw-rw-rw-   0        0        0     5873 2023-08-04 15:13:48.000000 soagen-0.3.0/src/soagen/preprocessor.py
--rw-rw-rw-   0        0        0     2516 2023-08-01 12:07:40.000000 soagen-0.3.0/src/soagen/schemas.py
--rw-rw-rw-   0        0        0    69716 2023-08-04 16:21:27.000000 soagen-0.3.0/src/soagen/struct.py
--rw-rw-rw-   0        0        0     2165 2023-07-29 16:15:31.000000 soagen-0.3.0/src/soagen/type_list.py
--rw-rw-rw-   0        0        0     1657 2023-08-03 12:36:06.000000 soagen-0.3.0/src/soagen/utils.py
--rw-rw-rw-   0        0        0     3576 2023-07-30 14:09:00.000000 soagen-0.3.0/src/soagen/variable.py
--rw-rw-rw-   0        0        0      616 2023-07-29 16:15:31.000000 soagen-0.3.0/src/soagen/version.py
--rw-rw-rw-   0        0        0        6 2023-08-03 12:44:35.000000 soagen-0.3.0/src/soagen/version.txt
--rw-rw-rw-   0        0        0    12339 2023-07-31 14:15:42.000000 soagen-0.3.0/src/soagen/writer.py
-drwxrwxrwx   0        0        0        0 2023-08-04 16:22:18.635346 soagen-0.3.0/src/soagen.egg-info/
--rw-rw-rw-   0        0        0     2087 2023-08-04 16:22:18.000000 soagen-0.3.0/src/soagen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1353 2023-08-04 16:22:18.000000 soagen-0.3.0/src/soagen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 16:22:18.000000 soagen-0.3.0/src/soagen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-08-04 16:22:18.000000 soagen-0.3.0/src/soagen.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       51 2023-08-04 16:22:18.000000 soagen-0.3.0/src/soagen.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-08-04 16:22:18.000000 soagen-0.3.0/src/soagen.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-07-28 06:00:37.000000 soagen-0.3.0/src/soagen.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-08-06 15:06:20.058867 soagen-0.4.0/
+-rw-rw-rw-   0        0        0     1154 2023-08-06 15:05:21.000000 soagen-0.4.0/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1064 2023-07-21 10:29:49.000000 soagen-0.4.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     2499 2023-08-06 15:06:20.058867 soagen-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0      466 2023-07-30 08:46:14.000000 soagen-0.4.0/README.md
+-rw-rw-rw-   0        0        0     1893 2023-08-03 12:48:33.000000 soagen-0.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-06 15:06:20.059866 soagen-0.4.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-06 15:06:20.010866 soagen-0.4.0/src/
+drwxrwxrwx   0        0        0        0 2023-08-06 15:06:20.034867 soagen-0.4.0/src/soagen/
+-rw-rw-rw-   0        0        0      477 2023-07-29 16:15:31.000000 soagen-0.4.0/src/soagen/__init__.py
+-rw-rw-rw-   0        0        0      870 2023-07-30 13:58:17.000000 soagen-0.4.0/src/soagen/column.py
+-rw-rw-rw-   0        0        0     5264 2023-08-04 15:13:48.000000 soagen-0.4.0/src/soagen/config.py
+-rw-rw-rw-   0        0        0      952 2023-07-29 16:15:31.000000 soagen-0.4.0/src/soagen/configurable.py
+-rw-rw-rw-   0        0        0    19094 2023-08-05 12:32:31.000000 soagen-0.4.0/src/soagen/cpp.py
+-rw-rw-rw-   0        0        0      574 2023-07-29 16:15:31.000000 soagen-0.4.0/src/soagen/errors.py
+-rw-rw-rw-   0        0        0    11685 2023-08-04 15:13:48.000000 soagen-0.4.0/src/soagen/header_file.py
+drwxrwxrwx   0        0        0        0 2023-08-06 15:06:20.053869 soagen-0.4.0/src/soagen/hpp/
+-rw-rw-rw-   0        0        0     5693 2023-08-06 15:03:06.000000 soagen-0.4.0/src/soagen/hpp/.clang-format
+-rw-rw-rw-   0        0        0    11199 2023-08-06 12:21:38.000000 soagen-0.4.0/src/soagen/hpp/allocator.hpp
+-rw-rw-rw-   0        0        0    36529 2023-08-06 09:59:43.000000 soagen-0.4.0/src/soagen/hpp/column_traits.hpp
+-rw-rw-rw-   0        0        0    27306 2023-08-06 12:56:25.000000 soagen-0.4.0/src/soagen/hpp/core.hpp
+-rw-rw-rw-   0        0        0     1680 2023-08-06 09:10:24.000000 soagen-0.4.0/src/soagen/hpp/emplacer.hpp
+drwxrwxrwx   0        0        0        0 2023-08-06 15:06:20.056869 soagen-0.4.0/src/soagen/hpp/generated/
+-rw-rw-rw-   0        0        0     9858 2023-08-06 15:03:06.000000 soagen-0.4.0/src/soagen/hpp/generated/compressed_pair.hpp
+-rw-rw-rw-   0        0        0     3859 2023-08-06 15:03:06.000000 soagen-0.4.0/src/soagen/hpp/generated/functions.hpp
+-rw-rw-rw-   0        0        0    42666 2023-08-06 15:03:08.000000 soagen-0.4.0/src/soagen/hpp/generated/preprocessor.hpp
+-rw-rw-rw-   0        0        0      420 2023-08-05 21:19:05.000000 soagen-0.4.0/src/soagen/hpp/generated/version.hpp
+-rw-rw-rw-   0        0        0      868 2023-08-05 10:16:57.000000 soagen-0.4.0/src/soagen/hpp/header_end.hpp
+-rw-rw-rw-   0        0        0     1073 2023-08-05 13:12:06.000000 soagen-0.4.0/src/soagen/hpp/header_start.hpp
+-rw-rw-rw-   0        0        0     3250 2023-08-06 09:18:47.000000 soagen-0.4.0/src/soagen/hpp/invoke.hpp
+-rw-rw-rw-   0        0        0    12689 2023-08-06 12:17:28.000000 soagen-0.4.0/src/soagen/hpp/iterator.hpp
+-rw-rw-rw-   0        0        0     5481 2023-08-06 09:45:57.000000 soagen-0.4.0/src/soagen/hpp/mixins.hpp
+-rw-rw-rw-   0        0        0    12609 2023-08-06 12:56:31.000000 soagen-0.4.0/src/soagen/hpp/row.hpp
+drwxrwxrwx   0        0        0        0 2023-08-06 15:06:20.057867 soagen-0.4.0/src/soagen/hpp/single/
+-rw-rw-rw-   0        0        0   234028 2023-08-06 15:05:21.000000 soagen-0.4.0/src/soagen/hpp/single/soagen.hpp
+-rw-rw-rw-   0        0        0      979 2023-07-29 16:15:31.000000 soagen-0.4.0/src/soagen/hpp/soagen.hpp
+-rw-rw-rw-   0        0        0    56937 2023-08-06 09:40:50.000000 soagen-0.4.0/src/soagen/hpp/table.hpp
+-rw-rw-rw-   0        0        0    34687 2023-08-06 09:19:24.000000 soagen-0.4.0/src/soagen/hpp/table_traits.hpp
+-rw-rw-rw-   0        0        0     3680 2023-08-06 15:05:21.000000 soagen-0.4.0/src/soagen/hpp/tuples.hpp
+-rw-rw-rw-   0        0        0     1067 2023-07-30 13:01:18.000000 soagen-0.4.0/src/soagen/includes.py
+-rw-rw-rw-   0        0        0     1534 2023-08-01 12:05:38.000000 soagen-0.4.0/src/soagen/injectors.py
+-rw-rw-rw-   0        0        0     3926 2023-07-29 16:15:31.000000 soagen-0.4.0/src/soagen/log.py
+-rw-rw-rw-   0        0        0    22644 2023-08-04 15:13:48.000000 soagen-0.4.0/src/soagen/main.py
+-rw-rw-rw-   0        0        0     3529 2023-08-04 15:13:48.000000 soagen-0.4.0/src/soagen/metavars.py
+-rw-rw-rw-   0        0        0     6453 2023-08-04 15:13:48.000000 soagen-0.4.0/src/soagen/natvis_file.py
+-rw-rw-rw-   0        0        0     1971 2023-07-29 16:15:31.000000 soagen-0.4.0/src/soagen/paths.py
+-rw-rw-rw-   0        0        0     6808 2023-08-05 11:46:44.000000 soagen-0.4.0/src/soagen/preprocessor.py
+-rw-rw-rw-   0        0        0     2516 2023-08-01 12:07:40.000000 soagen-0.4.0/src/soagen/schemas.py
+-rw-rw-rw-   0        0        0    70014 2023-08-05 21:07:07.000000 soagen-0.4.0/src/soagen/struct.py
+-rw-rw-rw-   0        0        0     2165 2023-07-29 16:15:31.000000 soagen-0.4.0/src/soagen/type_list.py
+-rw-rw-rw-   0        0        0     1657 2023-08-03 12:36:06.000000 soagen-0.4.0/src/soagen/utils.py
+-rw-rw-rw-   0        0        0     3544 2023-08-05 12:31:21.000000 soagen-0.4.0/src/soagen/variable.py
+-rw-rw-rw-   0        0        0      616 2023-07-29 16:15:31.000000 soagen-0.4.0/src/soagen/version.py
+-rw-rw-rw-   0        0        0        6 2023-08-05 21:19:05.000000 soagen-0.4.0/src/soagen/version.txt
+-rw-rw-rw-   0        0        0    12339 2023-07-31 14:15:42.000000 soagen-0.4.0/src/soagen/writer.py
+drwxrwxrwx   0        0        0        0 2023-08-06 15:06:20.040866 soagen-0.4.0/src/soagen.egg-info/
+-rw-rw-rw-   0        0        0     2499 2023-08-06 15:06:19.000000 soagen-0.4.0/src/soagen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1433 2023-08-06 15:06:20.000000 soagen-0.4.0/src/soagen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-06 15:06:19.000000 soagen-0.4.0/src/soagen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-08-06 15:06:19.000000 soagen-0.4.0/src/soagen.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       51 2023-08-06 15:06:19.000000 soagen-0.4.0/src/soagen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-08-06 15:06:19.000000 soagen-0.4.0/src/soagen.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-07-28 06:00:37.000000 soagen-0.4.0/src/soagen.egg-info/zip-safe
```

### Comparing `soagen-0.3.0/LICENSE.txt` & `soagen-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `soagen-0.3.0/PKG-INFO` & `soagen-0.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soagen
-Version: 0.3.0
+Version: 0.4.0
 Summary: Struct-of-Arrays generator for C++ projects.
 Author-email: Mark Gillard <mark.gillard@outlook.com.au>
 License: MIT
 Project-URL: Source, https://github.com/marzer/soagen
 Project-URL: Tracker, https://github.com/marzer/soagen/issues
 Project-URL: Funding, https://github.com/sponsors/marzer
 Keywords: c++,soa,struct-of-arrays,structure-of-arrays,struct of arrays,structure of arrays,parallel-arrays,parallel arrays,std::vector
@@ -33,14 +33,23 @@
 <br><br>
 
 [gitter]: https://gitter.im/marzer/community
 [sponsor]: https://github.com/sponsors/marzer
 
 # Changelog
 
+## v0.4.0
+
+-   Fixed `soagen::is_table<>`
+-   Added support for emplace-constructing column values by unpacking all `std::tuple`-like types (not just the `emplacer`)
+-   Added support for taking `std::integral_constants` in `for_each_column()`
+-   Added `soagen::same_table_type<>`
+-   Added conversions between `soagen::row<>` specializations
+-   Optimized instantiation overhead for most type-traits
+
 ## v0.3.0
 
 -   Added `hpp.combined`
 -   Added `std::integral_constant<size_t>` to the overload set used by `for_each_column()`
 -   Added support for constructing rows from all `std::tuple`-like types
 -   Optimized bulk-swap operations
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: soagen Version: 0.3.0 Summary: Struct-of-Arrays
+Metadata-Version: 2.1 Name: soagen Version: 0.4.0 Summary: Struct-of-Arrays
 generator for C++ projects. Author-email: Mark Gillard
 gillard@outlook.com.au> License: MIT Project-URL: Source, https://github.com/
 marzer/soagen Project-URL: Tracker, https://github.com/marzer/soagen/issues
 Project-URL: Funding, https://github.com/sponsors/marzer Keywords:
 c++,soa,struct-of-arrays,structure-of-arrays,struct of arrays,structure of
 arrays,parallel-arrays,parallel arrays,std::vector Classifier: Development
 Status :: 3 - Alpha Classifier: License :: OSI Approved :: MIT License
@@ -13,17 +13,22 @@
 badge-sponsor.svg)][sponsor] [![Gitter](docs/images/badge-gitter.svg)][gitter]
 
      â¨&#xFE0F; This README is a stub. Please see the HTML documentation:
                       marzer.github.io/soagenâ¨&#xFE0F;
 
 
 [gitter]: https://gitter.im/marzer/community [sponsor]: https://github.com/
-sponsors/marzer # Changelog ## v0.3.0 - Added `hpp.combined` - Added `std::
-integral_constant` to the overload set used by `for_each_column()` - Added
-support for constructing rows from all `std::tuple`-like types - Optimized
-bulk-swap operations ## v0.2.0 - Added `structs.annotations` - Added
+sponsors/marzer # Changelog ## v0.4.0 - Fixed `soagen::is_table<>` - Added
+support for emplace-constructing column values by unpacking all `std::tuple`-
+like types (not just the `emplacer`) - Added support for taking `std::
+integral_constants` in `for_each_column()` - Added `soagen::same_table_type<>`
+- Added conversions between `soagen::row<>` specializations - Optimized
+instantiation overhead for most type-traits ## v0.3.0 - Added `hpp.combined` -
+Added `std::integral_constant` to the overload set used by `for_each_column()`
+- Added support for constructing rows from all `std::tuple`-like types -
+Optimized bulk-swap operations ## v0.2.0 - Added `structs.annotations` - Added
 `structs.attributes` - Added `auto` option for `structs.default_constructible`
 - Added `soagen::row_base` - Added `soagen::table_base` - Added `soagen::
 iterator_base` - Added `Base` template argument to `soagen::table` for CRTP -
 Added `swap_columns<>()` - Made `column_indices` member struct into `enum class
 columns` ## v0.1.2 - Minor refactors. ## v0.1.1 - Minor refactors. ## v0.1.0 -
 First public release ð&#xFE0F;
```

### Comparing `soagen-0.3.0/pyproject.toml` & `soagen-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `soagen-0.3.0/src/soagen/column.py` & `soagen-0.4.0/src/soagen/column.py`

 * *Files identical despite different names*

### Comparing `soagen-0.3.0/src/soagen/config.py` & `soagen-0.4.0/src/soagen/config.py`

 * *Files identical despite different names*

### Comparing `soagen-0.3.0/src/soagen/configurable.py` & `soagen-0.4.0/src/soagen/configurable.py`

 * *Files identical despite different names*

### Comparing `soagen-0.3.0/src/soagen/cpp.py` & `soagen-0.4.0/src/soagen/cpp.py`

 * *Files 2% similar despite different names*

```diff
@@ -648,15 +648,15 @@
     if text is not None:
         for header, regex in HEADER_MATCHERS:
             if regex.search(text) is not None:
                 out.append(header)
     return out
 
 
-IMPLICIT_INCLUDES = (
+IMPLICIT_INCLUDES = make_regex(
     r'version',
     r'cstdint',
     r'cstddef',
     r'cstdlib',
     r'numeric',
     r'type_traits',
     r'new',
@@ -665,18 +665,18 @@
     r'stdexcept',
     r'iterator',
     r'soagen.hpp',
 )
 
 
 def remove_implicit_includes(includes: list[str]) -> list[str]:
-    return [inc for inc in includes if inc not in IMPLICIT_INCLUDES]
+    return [inc for inc in includes if not IMPLICIT_INCLUDES.fullmatch(inc)]
 
 
-RESERVED_CPP_KEYWORDS = (
+RESERVED_CPP_KEYWORDS = make_regex(
     r'alignas',
     r'alignof',
     r'and',
     r'and_eq',
     r'asm',
     r'atomic_cancel',
     r'atomic_commit',
@@ -766,17 +766,16 @@
     r'void',
     r'volatile',
     r'wchar_t',
     r'while',
     r'xor',
     r'xor_eq',
 )
-RESERVED_CPP_KEYWORDS = set(RESERVED_CPP_KEYWORDS)
 
-RESERVED_SOAGEN = (
+RESERVED_SOAGEN = make_regex(
     # std::vector-like interface:
     r'allocator_type',
     r'assign',
     r'at',
     r'begin',
     r'capacity',
     r'cbegin',
@@ -838,15 +837,14 @@
     r'update',
     r'zerofill_column',
     r'zerofill',
     # other
     r'soagen',
     r'std',
 )
-RESERVED_SOAGEN = set(RESERVED_SOAGEN)
 
 VALID_IDENTIFIER = re.compile(r'^[A-Za-z][A-Za-z_0-9]*$')
 
 
 def is_valid_identifier(s: str) -> tuple[bool, str]:
     if not s:
         return (False, 'may not be blank')
@@ -854,15 +852,15 @@
         return (False, 'may not begin with an underscore')
     if s.find('__') != -1:
         return (False, 'may not contain double-underscores')
     if re.fullmatch(r'^[0-9].*$', s):
         return (False, 'may not begin with a digit')
     if not VALID_IDENTIFIER.fullmatch(s):
         return (False, 'may contain only a-z, A-Z, 0-9, and underscores')
-    if s in RESERVED_CPP_KEYWORDS:
+    if RESERVED_CPP_KEYWORDS.fullmatch(s):
         return (False, 'may not be a C++ keyword')
-    if s in RESERVED_SOAGEN:
+    if RESERVED_SOAGEN.fullmatch(s):
         return (False, 'reserved by soagen')
     return (True,)
 
 
 __all__ = [r'detect_includes', r'remove_implicit_includes', r'is_valid_identifier']
```

### Comparing `soagen-0.3.0/src/soagen/errors.py` & `soagen-0.4.0/src/soagen/errors.py`

 * *Files identical despite different names*

### Comparing `soagen-0.3.0/src/soagen/header_file.py` & `soagen-0.4.0/src/soagen/header_file.py`

 * *Files identical despite different names*

### Comparing `soagen-0.3.0/src/soagen/hpp/.clang-format` & `soagen-0.4.0/src/soagen/hpp/.clang-format`

 * *Files identical despite different names*

### Comparing `soagen-0.3.0/src/soagen/hpp/allocator.hpp` & `soagen-0.4.0/src/soagen/hpp/allocator.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,14 @@
 //# Copyright (c) Mark Gillard <mark.gillard@outlook.com.au>
 //# See https://github.com/marzer/soagen/blob/master/LICENSE for the full license text.
 //# SPDX-License-Identifier: MIT
 #pragma once
 
 #include "generated/functions.hpp"
 #include "header_start.hpp"
-#if SOAGEN_CLANG >= 16
-	#pragma clang diagnostic ignored "-Wunsafe-buffer-usage"
-#endif
 
 namespace soagen
 {
 	/// @brief The default allocator used by soagen tables.
 	///
 	/// @note Use of this allocator is not required; you can use any allocator compatible with the
 	/// 		 std::allocator protocol, so long as its `value_type` is `char`, `unsigned char` or `std::byte`.
```

### Comparing `soagen-0.3.0/src/soagen/hpp/column_traits.hpp` & `soagen-0.4.0/src/soagen/hpp/column_traits.hpp`

 * *Files 6% similar despite different names*

```diff
@@ -1,72 +1,119 @@
 //# This file is a part of marzer/soagen and is subject to the the terms of the MIT license.
 //# Copyright (c) Mark Gillard <mark.gillard@outlook.com.au>
 //# See https://github.com/marzer/soagen/blob/master/LICENSE for the full license text.
 //# SPDX-License-Identifier: MIT
 #pragma once
 
 #include "generated/functions.hpp"
+#include "emplacer.hpp"
+#include "tuples.hpp"
 #include "header_start.hpp"
-#if SOAGEN_CLANG >= 16
-	#pragma clang diagnostic ignored "-Wunsafe-buffer-usage"
+
+#ifndef SOAGEN_LAUNDER
+	#if defined(__cpp_lib_launder) && __cpp_lib_launder >= 201606
+		#define SOAGEN_LAUNDER(...) std::launder(__VA_ARGS__)
+	#elif SOAGEN_CLANG >= 8 || SOAGEN_GCC >= 7 || SOAGEN_ICC >= 1910 || SOAGEN_MSVC >= 1914                            \
+		|| SOAGEN_HAS_BUILTIN(__builtin_launder)
+		#define SOAGEN_LAUNDER(...) __builtin_launder(__VA_ARGS__)
+	#else
+		#define SOAGEN_LAUNDER(...) __VA_ARGS__
+	#endif
+#endif
+
+#ifndef SOAGEN_COLUMN
+	#define SOAGEN_COLUMN(I)                                                                                           \
+		SOAGEN_PURE_INLINE_GETTER                                                                                      \
+		SOAGEN_ATTR(returns_nonnull)
+#endif
+
+#ifndef SOAGEN_ALIGNED_COLUMN
+	#define SOAGEN_ALIGNED_COLUMN(I)                                                                                   \
+		SOAGEN_COLUMN(I)                                                                                               \
+		SOAGEN_ATTR(assume_aligned(                                                                                    \
+			soagen::detail::actual_column_alignment<table_traits, allocator_type, static_cast<std::size_t>(I)>))
 #endif
 
-#define soagen_storage_ptr(...) soagen::assume_aligned<alignof(storage_type)>(__VA_ARGS__)
+#define soagen_aligned_storage(...) soagen::assume_aligned<alignof(storage_type)>(__VA_ARGS__)
 
 /// @cond
 namespace soagen::detail
 {
 	// a base class for the column traits that handles all the non-alignment-dependent stuff
 	// (to minimize template instantiation explosion)
 	template <typename StorageType>
 	struct column_traits_base
 	{
 		using storage_type = StorageType;
 		static_assert(!is_cvref<storage_type>, "column storage_type may not be cvref-qualified");
 		static_assert(!std::is_void_v<storage_type>, "column storage_type may not be void");
 		static_assert(std::is_destructible_v<storage_type>, "column storage_type must be destructible");
 
-		//--- dereferencing --------------------------------------------------------------------------------------------
+		//--- pointers -------------------------------------------------------------------------------------------------
 
 		SOAGEN_PURE_GETTER
 		SOAGEN_ATTR(nonnull)
-		static constexpr storage_type& get(std::byte* ptr) noexcept
+		static constexpr storage_type* ptr(std::byte* p) noexcept
 		{
-			SOAGEN_ASSUME(ptr != nullptr);
+			SOAGEN_ASSUME(p != nullptr);
 
-			return *SOAGEN_LAUNDER(reinterpret_cast<storage_type*>(soagen_storage_ptr(ptr)));
+			if constexpr (std::is_same_v<storage_type, std::byte>)
+				return p;
+			else
+				return SOAGEN_LAUNDER(reinterpret_cast<storage_type*>(p));
 		}
 
 		SOAGEN_PURE_GETTER
 		SOAGEN_ATTR(nonnull)
-		static constexpr const storage_type& get(const std::byte* ptr) noexcept
+		static constexpr const storage_type* ptr(const std::byte* p) noexcept
 		{
-			SOAGEN_ASSUME(ptr != nullptr);
+			SOAGEN_ASSUME(p != nullptr);
 
-			return *SOAGEN_LAUNDER(reinterpret_cast<const storage_type*>(soagen_storage_ptr(ptr)));
+			if constexpr (std::is_same_v<storage_type, std::byte>)
+				return p;
+			else
+				return SOAGEN_LAUNDER(reinterpret_cast<const storage_type*>(p));
+		}
+
+		//--- dereferencing --------------------------------------------------------------------------------------------
+
+		SOAGEN_PURE_INLINE_GETTER
+		SOAGEN_ATTR(nonnull)
+		static constexpr storage_type& get(std::byte* p) noexcept
+		{
+			return *ptr(p);
+		}
+
+		SOAGEN_PURE_INLINE_GETTER
+		SOAGEN_ATTR(nonnull)
+		static constexpr const storage_type& get(const std::byte* p) noexcept
+		{
+			SOAGEN_ASSUME(p != nullptr);
+
+			return *ptr(p);
 		}
 
 		//--- default construction -------------------------------------------------------------------------------------
 
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = std::is_default_constructible_v<storage_type>)
 		SOAGEN_ATTR(nonnull)
 		static constexpr storage_type& default_construct(std::byte* destination) //
 			noexcept(std::is_nothrow_default_constructible_v<storage_type>)
 		{
 			SOAGEN_ASSUME(destination != nullptr);
 
 #if defined(__cpp_lib_start_lifetime_as) && __cpp_lib_start_lifetime_as >= 202207
 			if constexpr (is_implicit_lifetime_type<storage_type>)
 			{
-				return *(std::start_lifetime_as<storage_type>(soagen_storage_ptr(destination)));
+				return *(std::start_lifetime_as<storage_type>(destination));
 			}
 			else
 			{
 #endif
-				return *(::new (static_cast<void*>(soagen_storage_ptr(destination))) storage_type);
+				return *(::new (static_cast<void*>(destination)) storage_type);
 
 #if defined(__cpp_lib_start_lifetime_as) && __cpp_lib_start_lifetime_as >= 202207
 			}
 #endif
 		}
 
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = std::is_default_constructible_v<storage_type>)
@@ -87,15 +134,15 @@
 		{
 			SOAGEN_ASSUME(buffer != nullptr);
 			SOAGEN_ASSUME(count);
 
 #if defined(__cpp_lib_start_lifetime_as) && __cpp_lib_start_lifetime_as >= 2022071
 			if constexpr (is_implicit_lifetime_type<storage_type>)
 			{
-				std::start_lifetime_as_array<storage_type>(soagen_storage_ptr(destination), count);
+				std::start_lifetime_as_array<storage_type>(destination, count);
 			}
 			else
 #endif
 				if constexpr (std::is_nothrow_default_constructible_v<storage_type>
 							  || std::is_trivially_destructible_v<storage_type>)
 			{
 				for (const size_t e = index + count; index < e; index++)
@@ -121,118 +168,164 @@
 			}
 		}
 
 		//--- construction ---------------------------------------------------------------------------------------------
 
 		static constexpr bool is_trivially_copyable = std::is_trivially_copyable_v<storage_type>;
 
+		// constructibility using memcpy
+
 	  private:
-		// note: these *should* just be regular variable templates but evidently GCC
-		// chokes on partial variable template specialization at class scope:
-		// https://gcc.gnu.org/bugzilla/show_bug.cgi?id=71954
+		template <typename Arg>
+		struct is_constructible_with_memcpy_
+			: std::conjunction<
+				  std::bool_constant<sizeof(storage_type) == sizeof(remove_cvref<Arg>)>, //
+				  std::is_trivially_copyable<storage_type>,								 //
+				  is_implicit_lifetime_type_<storage_type>,								 //
+				  std::is_trivially_copyable<remove_cvref<Arg>>,						 //
+				  std::disjunction<
+					  std::is_same<storage_type, remove_cvref<Arg>>,
+					  std::bool_constant<any_same<storage_type, char, unsigned char, std::byte>
+										 && any_same<remove_cvref<Arg>, char, unsigned char, std::byte>>,
+					  std::conjunction<std::is_same<storage_type, void*>, std::is_pointer<remove_cvref<Arg>>>>>
+		{};
 
+	  public:
+		template <typename Arg>
+		static constexpr bool is_constructible_with_memcpy = is_constructible_with_memcpy_<Arg>::value;
+
+		// constructibility by unpacking a tuple
+
+	  private:
+		template <typename Arg>
+		struct is_constructible_by_unpacking_tuple_ //
+			: detail::is_constructible_by_unpacking_tuple_<storage_type, Arg>
+		{};
+
+	  public:
+		template <typename Arg>
+		static constexpr bool is_constructible_by_unpacking_tuple = is_constructible_by_unpacking_tuple_<Arg>::value;
+
+		// trivial-constructibility
+
+	  private:
 		template <typename... Args>
-		struct is_constructible_with_memcpy_ : std::false_type
+		struct is_trivially_constructible_ : std::is_trivially_constructible<storage_type, remove_cvref<Args>...>
 		{};
+
 		template <typename Arg>
-		struct is_constructible_with_memcpy_<Arg>
-			: std::bool_constant<sizeof(storage_type) == sizeof(remove_cvref<Arg>)	//
-								 && is_trivially_copyable							//
-								 && is_implicit_lifetime_type<storage_type>			//
-								 && std::is_trivially_copyable_v<remove_cvref<Arg>> //
-								 && (std::is_same_v<storage_type, remove_cvref<Arg>>
-									 || (any_same<storage_type, char, unsigned char, std::byte>
-										 && any_same<remove_cvref<Arg>, char, unsigned char, std::byte>)
-									 || (std::is_same_v<storage_type, void*> && std::is_pointer_v<remove_cvref<Arg>>))>
+		struct is_trivially_constructible_<Arg>
+			: std::disjunction<std::is_trivially_constructible<storage_type, remove_cvref<Arg>>,
+							   is_constructible_with_memcpy_<remove_cvref<Arg>>,
+							   typename is_constructible_by_unpacking_tuple_<Arg>::is_trivial>
 		{};
 
 	  public:
 		template <typename... Args>
-		static constexpr bool is_constructible_with_memcpy = is_constructible_with_memcpy_<Args...>::value;
+		static constexpr bool is_trivially_constructible = is_trivially_constructible_<Args...>::value;
 
-		template <typename... Args>
-		static constexpr bool is_trivially_constructible =
-			is_constructible_with_memcpy<Args...>
-			|| std::is_trivially_constructible_v<storage_type, remove_cvref<Args>...>;
+		// constructibility from arbitrary args
 
-	  private:
 		template <typename... Args>
-		struct is_constructible_
-			: std::bool_constant<is_trivially_constructible<Args...> || std::is_constructible_v<storage_type, Args...>>
+		struct is_constructible_trait : std::disjunction<is_trivially_constructible_<Args...>, //
+														 std::is_constructible<storage_type, Args...>>
+		{};
+		template <typename Arg>
+		struct is_constructible_trait<Arg> : std::disjunction<is_trivially_constructible_<Arg>, //
+															  std::is_constructible<storage_type, Arg>,
+															  is_constructible_by_unpacking_tuple_<Arg>>
 		{};
 		template <typename T>
-		struct is_constructible_<T*> : std::bool_constant<std::is_same_v<storage_type, void*> //
-														  || is_trivially_constructible<T*>	  //
-														  || std::is_constructible_v<storage_type, T*>>
+		struct is_constructible_trait<T*> : std::disjunction<std::is_same<storage_type, void*>, //
+															 is_trivially_constructible_<T*>,	//
+															 std::is_constructible<storage_type, T*>>
 		{};
 		template <typename T>
-		struct is_constructible_<T*&> : std::bool_constant<std::is_same_v<storage_type, void*> //
-														   || is_trivially_constructible<T*&>  //
-														   || std::is_constructible_v<storage_type, T*&>>
+		struct is_constructible_trait<T*&> : std::disjunction<std::is_same<storage_type, void*>, //
+															  is_trivially_constructible_<T*&>,	 //
+															  std::is_constructible<storage_type, T*&>>
 		{};
 		template <typename T>
-		struct is_constructible_<T*&&> : std::bool_constant<std::is_same_v<storage_type, void*> //
-															|| is_trivially_constructible<T*&&> //
-															|| std::is_constructible_v<storage_type, T*&&>>
+		struct is_constructible_trait<T*&&> : std::disjunction<std::is_same<storage_type, void*>, //
+															   is_trivially_constructible_<T*&&>, //
+															   std::is_constructible<storage_type, T*&&>>
 		{};
 		template <typename... Args>
-		struct is_constructible_<emplacer<Args...>&&> : is_constructible_<Args...>
+		struct is_constructible_trait<emplacer<Args...>&&> : is_constructible_trait<Args...>
 		{};
 
-	  public:
 		template <typename... Args>
-		static constexpr bool is_constructible = is_constructible_<Args...>::value;
+		static constexpr bool is_constructible = is_constructible_trait<Args...>::value;
+
+		// nothrow-constructibility from arbitrary args
 
-	  private:
 		template <typename... Args>
-		struct is_nothrow_constructible_ : std::bool_constant<is_trivially_constructible<Args...>
-															  || std::is_nothrow_constructible_v<storage_type, Args...>>
+		struct is_nothrow_constructible_trait : std::disjunction<is_trivially_constructible_<Args...>,
+																 std::is_nothrow_constructible<storage_type, Args...>>
+		{};
+		template <typename Arg>
+		struct is_nothrow_constructible_trait<Arg>
+			: std::disjunction<is_trivially_constructible_<Arg>,
+							   std::is_nothrow_constructible<storage_type, Arg>,
+							   typename is_constructible_by_unpacking_tuple_<Arg>::is_nothrow>
 		{};
 		template <typename T>
-		struct is_nothrow_constructible_<T*> : std::bool_constant<std::is_same_v<storage_type, void*> //
-																  || is_trivially_constructible<T*>	  //
-																  || std::is_nothrow_constructible_v<storage_type, T*>>
+		struct is_nothrow_constructible_trait<T*> : std::disjunction<std::is_same<storage_type, void*>, //
+																	 is_trivially_constructible_<T*>,	//
+																	 std::is_nothrow_constructible<storage_type, T*>>
 		{};
 		template <typename T>
-		struct is_nothrow_constructible_<T*&>
-			: std::bool_constant<std::is_same_v<storage_type, void*> //
-								 || is_trivially_constructible<T*&>	 //
-								 || std::is_nothrow_constructible_v<storage_type, T*&>>
+		struct is_nothrow_constructible_trait<T*&> : std::disjunction<std::is_same<storage_type, void*>, //
+																	  is_trivially_constructible_<T*&>,	 //
+																	  std::is_nothrow_constructible<storage_type, T*&>>
 		{};
 		template <typename T>
-		struct is_nothrow_constructible_<T*&&>
-			: std::bool_constant<std::is_same_v<storage_type, void*> //
-								 || is_trivially_constructible<T*&&> //
-								 || std::is_nothrow_constructible_v<storage_type, T*&&>>
+		struct is_nothrow_constructible_trait<T*&&>
+			: std::disjunction<std::is_same<storage_type, void*>, //
+							   is_trivially_constructible_<T*&&>, //
+							   std::is_nothrow_constructible<storage_type, T*&&>>
 		{};
 		template <typename... Args>
-		struct is_nothrow_constructible_<emplacer<Args...>&&> : is_nothrow_constructible_<Args...>
+		struct is_nothrow_constructible_trait<emplacer<Args...>&&> : is_nothrow_constructible_trait<Args...>
 		{};
 
-	  public:
 		template <typename... Args>
-		static constexpr bool is_nothrow_constructible = is_nothrow_constructible_<Args...>::value;
+		static constexpr bool is_nothrow_constructible = is_nothrow_constructible_trait<Args...>::value;
 
 	  private:
 		template <typename... Args, size_t... Indices>
 		SOAGEN_ATTR(nonnull)
+		SOAGEN_ALWAYS_INLINE
 		static constexpr storage_type& construct_from_emplacer(std::byte* destination,
 															   emplacer<Args...>&& args,
 															   std::index_sequence<Indices...>) //
 			noexcept(is_nothrow_constructible<Args...>)
 		{
 			static_assert((std::is_reference_v<Args> && ...));
 			static_assert(sizeof...(Args) == sizeof...(Indices));
 			SOAGEN_ASSUME(destination != nullptr);
 
 			return construct(destination,
 							 static_cast<Args>(*static_cast<std::add_pointer_t<std::remove_reference_t<Args>>>(
 								 args.ptrs[Indices]))...);
 		}
 
+		template <typename Tuple, size_t... Indices>
+		SOAGEN_ATTR(nonnull)
+		SOAGEN_ALWAYS_INLINE
+		static constexpr storage_type& construct_from_tuple(std::byte* destination,
+															Tuple&& tuple,
+															std::index_sequence<Indices...>) //
+			noexcept(is_constructible_by_unpacking_tuple_<Tuple&&>::is_nothrow::value)
+		{
+			SOAGEN_ASSUME(destination != nullptr);
+
+			return construct(destination, get_from_tuple<Indices>(static_cast<Tuple&&>(tuple))...);
+		}
+
 	  public:
 		SOAGEN_CONSTRAINED_TEMPLATE(is_constructible<Args&&...>, typename... Args)
 		SOAGEN_ATTR(nonnull)
 		static constexpr storage_type& construct(std::byte* destination, Args&&... args) //
 			noexcept(is_nothrow_constructible<Args&&...>)
 		{
 			SOAGEN_ASSUME(destination != nullptr);
@@ -246,29 +339,36 @@
 				if constexpr (sizeof...(Args) == 1 && (is_emplacer<std::remove_reference_t<Args>> && ...))
 				{
 					return construct_from_emplacer(
 						destination,
 						static_cast<Args&&>(args)...,
 						std::make_index_sequence<std::tuple_size_v<remove_cvref<Args>>>{}...);
 				}
-				else if constexpr (is_constructible_with_memcpy<Args&&...>)
+				else if constexpr (sizeof...(Args) == 1 && (is_constructible_with_memcpy<Args&&> && ...))
 				{
-					std::memcpy(soagen_storage_ptr(destination), soagen_storage_ptr(&args)..., sizeof(storage_type));
+					std::memcpy(soagen_aligned_storage(destination), &args..., sizeof(storage_type));
 
 					return get(destination);
 				}
-				else if constexpr (std::is_aggregate_v<storage_type>)
+				else if constexpr (std::is_constructible_v<storage_type, Args&&...>)
 				{
-					return *(::new (static_cast<void*>(soagen_storage_ptr(destination)))
-								 storage_type{ static_cast<Args&&>(args)... });
+					if constexpr (std::is_aggregate_v<storage_type>)
+					{
+						return *(::new (static_cast<void*>(destination)) storage_type{ static_cast<Args&&>(args)... });
+					}
+					else
+					{
+						return *(::new (static_cast<void*>(destination)) storage_type(static_cast<Args&&>(args)...));
+					}
 				}
-				else
+				else if constexpr (sizeof...(Args) == 1 && (is_constructible_by_unpacking_tuple<Args&&> && ...))
 				{
-					return *(::new (static_cast<void*>(soagen_storage_ptr(destination)))
-								 storage_type(static_cast<Args&&>(args)...));
+					return construct_from_tuple(destination,
+												static_cast<Args&&>(args)...,
+												std::make_index_sequence<std::tuple_size_v<remove_cvref<Args>>>{}...);
 				}
 			}
 		}
 
 		SOAGEN_CONSTRAINED_TEMPLATE(is_constructible<Args&&...>, typename... Args)
 		SOAGEN_ATTR(nonnull)
 		static constexpr storage_type& construct_at(std::byte* buffer, size_t index, Args&&... args) //
@@ -482,16 +582,16 @@
 		{
 			SOAGEN_ASSUME(destination != nullptr);
 			SOAGEN_ASSUME(source != nullptr);
 			SOAGEN_ASSUME(destination != source);
 
 			if constexpr (is_constructible_with_memcpy<storage_type&&>)
 			{
-				std::memcpy(soagen_storage_ptr(destination),
-							soagen_storage_ptr(static_cast<std::byte*>(source)),
+				std::memcpy(soagen_aligned_storage(destination),
+							soagen_aligned_storage(static_cast<std::byte*>(source)),
 							sizeof(storage_type));
 
 				return get(destination);
 			}
 			else if constexpr (is_trivially_move_assignable || std::is_move_assignable_v<storage_type>)
 			{
 				return get(destination) = static_cast<storage_type&&>(get(static_cast<std::byte*>(source)));
@@ -549,16 +649,16 @@
 		{
 			SOAGEN_ASSUME(destination != nullptr);
 			SOAGEN_ASSUME(source != nullptr);
 			SOAGEN_ASSUME(destination != source);
 
 			if constexpr (is_constructible_with_memcpy<storage_type&&>)
 			{
-				std::memcpy(soagen_storage_ptr(destination),
-							soagen_storage_ptr(static_cast<const std::byte*>(source)),
+				std::memcpy(soagen_aligned_storage(destination),
+							soagen_aligned_storage(static_cast<const std::byte*>(source)),
 							sizeof(storage_type));
 
 				return get(destination);
 			}
 			else if constexpr (is_trivially_copy_assignable || std::is_copy_assignable_v<storage_type>)
 			{
 				return get(destination) = static_cast<const storage_type&>(get(source));
@@ -617,17 +717,17 @@
 			SOAGEN_ASSUME(lhs != nullptr);
 			SOAGEN_ASSUME(rhs != nullptr);
 			SOAGEN_ASSUME(lhs != rhs);
 
 			if constexpr (is_trivially_swappable)
 			{
 				alignas(storage_type) std::byte buf[sizeof(storage_type)];
-				std::memcpy(soagen_storage_ptr(buf), soagen_storage_ptr(lhs), sizeof(storage_type));
-				std::memcpy(soagen_storage_ptr(lhs), soagen_storage_ptr(rhs), sizeof(storage_type));
-				std::memcpy(soagen_storage_ptr(rhs), soagen_storage_ptr(buf), sizeof(storage_type));
+				std::memcpy(soagen_aligned_storage(buf), soagen_aligned_storage(lhs), sizeof(storage_type));
+				std::memcpy(soagen_aligned_storage(lhs), soagen_aligned_storage(rhs), sizeof(storage_type));
+				std::memcpy(soagen_aligned_storage(rhs), soagen_aligned_storage(buf), sizeof(storage_type));
 			}
 			else if constexpr (std::is_swappable_v<storage_type>)
 			{
 				using std::swap;
 				swap(get(lhs), get(rhs));
 			}
 			else
@@ -652,32 +752,32 @@
 		{
 			SOAGEN_ASSUME(lhs_buffer != nullptr);
 			SOAGEN_ASSUME(rhs_buffer != nullptr);
 
 			if SOAGEN_UNLIKELY(!count)
 				return;
 
-			lhs_buffer = soagen_storage_ptr(lhs_buffer + lhs_index * sizeof(storage_type));
-			rhs_buffer = soagen_storage_ptr(rhs_buffer + rhs_index * sizeof(storage_type));
+			lhs_buffer = soagen_aligned_storage(lhs_buffer + lhs_index * sizeof(storage_type));
+			rhs_buffer = soagen_aligned_storage(rhs_buffer + rhs_index * sizeof(storage_type));
 
 			[[maybe_unused]] SOAGEN_CPP23_STATIC_CONSTEXPR size_t trivial_buf_size = 2048u / sizeof(storage_type);
 
 			if constexpr (is_trivially_swappable && trivial_buf_size > 1)
 			{
 				for (size_t i = 0; i < count; i += trivial_buf_size)
 				{
 					const auto num = soagen::min(trivial_buf_size, count - i);
 
 					alignas(storage_type) std::byte buf[sizeof(storage_type) * trivial_buf_size];
 					std::memcpy(buf, lhs_buffer, sizeof(storage_type) * num);
 					std::memcpy(lhs_buffer, rhs_buffer, sizeof(storage_type) * num);
 					std::memcpy(rhs_buffer, buf, sizeof(storage_type) * num);
 
-					lhs_buffer = soagen_storage_ptr(lhs_buffer + trivial_buf_size * sizeof(storage_type));
-					rhs_buffer = soagen_storage_ptr(rhs_buffer + trivial_buf_size * sizeof(storage_type));
+					lhs_buffer = soagen_aligned_storage(lhs_buffer + trivial_buf_size * sizeof(storage_type));
+					rhs_buffer = soagen_aligned_storage(rhs_buffer + trivial_buf_size * sizeof(storage_type));
 				}
 			}
 			else
 			{
 				const auto end = lhs_buffer + count * sizeof(storage_type);
 				for (; lhs_buffer < end; lhs_buffer += sizeof(storage_type), rhs_buffer += sizeof(storage_type))
 				{
@@ -694,16 +794,16 @@
 									  const std::byte* source_buffer,
 									  size_t source_index,
 									  size_t count = 1) noexcept
 		{
 			SOAGEN_ASSUME(dest_buffer != nullptr);
 			SOAGEN_ASSUME(source_buffer != nullptr);
 
-			std::memmove(soagen_storage_ptr(dest_buffer + dest_index * sizeof(storage_type)),
-						 soagen_storage_ptr(source_buffer + source_index * sizeof(storage_type)),
+			std::memmove(soagen_aligned_storage(dest_buffer + dest_index * sizeof(storage_type)),
+						 soagen_aligned_storage(source_buffer + source_index * sizeof(storage_type)),
 						 count * sizeof(storage_type));
 		}
 
 		//--- equality -------------------------------------------------------------------------------------------------
 
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = is_equality_comparable<storage_type>)
 		SOAGEN_NODISCARD
@@ -878,10 +978,10 @@
 	};
 
 	template <typename T>
 	using to_base_traits = typename to_base_traits_<T>::type;
 }
 /// @endcond
 
-#undef soagen_storage_ptr
+#undef soagen_aligned_storage
 
 #include "header_end.hpp"
```

### Comparing `soagen-0.3.0/src/soagen/hpp/core.hpp` & `soagen-0.4.0/src/soagen/hpp/core.hpp`

 * *Files 10% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 #include <cstring>
 #include <numeric>
 #include <type_traits>
 #include <new>
 #include <utility>
 #include <memory>
 #include <optional>
+#include <iterator>
 
 #ifndef SOAGEN_COLUMN_SPAN_TYPE
 	#if SOAGEN_CPP >= 20 && SOAGEN_HAS_INCLUDE(<span>)
 		#include <span>
 		#define SOAGEN_COLUMN_SPAN_TYPE std::span
 	#elif SOAGEN_HAS_INCLUDE(<muu/span.h>)
 		#include <muu/span.h>
@@ -40,25 +41,14 @@
 	#include <optional>
 	#define SOAGEN_OPTIONAL_TYPE std::optional
 #endif
 
 SOAGEN_ENABLE_WARNINGS;
 #include "header_start.hpp"
 
-#ifndef SOAGEN_LAUNDER
-	#if defined(__cpp_lib_launder) && __cpp_lib_launder >= 201606
-		#define SOAGEN_LAUNDER(...) std::launder(__VA_ARGS__)
-	#elif SOAGEN_CLANG >= 8 || SOAGEN_GCC >= 7 || SOAGEN_ICC >= 1910 || SOAGEN_MSVC >= 1914                            \
-		|| SOAGEN_HAS_BUILTIN(__builtin_launder)
-		#define SOAGEN_LAUNDER(...) __builtin_launder(__VA_ARGS__)
-	#else
-		#define SOAGEN_LAUNDER(...) __VA_ARGS__
-	#endif
-#endif
-
 #ifndef SOAGEN_MAKE_NAME
 	#define SOAGEN_MAKE_NAME(Name)                                                                                     \
                                                                                                                        \
 		struct name_constant_##Name                                                                                    \
 		{                                                                                                              \
 			static constexpr const char value[] = #Name;                                                               \
 		};                                                                                                             \
@@ -155,35 +145,48 @@
 	template <typename... T>
 	inline constexpr bool all_integer = (!!sizeof...(T) && ... && is_integer<T>);
 
 	/// @brief	True if `T` is a (non-bool) unsigned integer.
 	template <typename T>
 	inline constexpr bool is_unsigned = is_integer<T> && std::is_unsigned_v<T>;
 
-	/// @brief	True if all `U` are the same as `T`.
+	/// @brief	True if any `U` are the same as `T`.
 	template <typename T, typename... U>
 	inline constexpr bool any_same = (false || ... || std::is_same_v<T, U>);
 
+	/// @brief	True if `Value` is in the list `Values`.
+	template <auto Value, auto... Values>
+	inline constexpr bool any_same_value = ((Value == Values) || ...);
+
 	/// @brief	True if `T` is a soagen-generated SoA table type.
 	template <typename T>
 	inline constexpr bool is_soa = POXY_IMPLEMENTATION_DETAIL(false); // specialized in generated code
 	/// @cond
 	template <typename T>
 	inline constexpr bool is_soa<const T> = is_soa<T>;
 	template <typename T>
 	inline constexpr bool is_soa<volatile T> = is_soa<T>;
 	template <typename T>
 	inline constexpr bool is_soa<const volatile T> = is_soa<T>;
+
+	namespace detail
+	{
+		template <typename T>
+		using is_implicit_lifetime_type_ = std::disjunction<std::is_scalar<T>,
+															std::is_array<T>,
+															std::conjunction<std::is_aggregate<T>,
+																			 std::is_trivially_constructible<T>,
+																			 std::is_trivially_destructible<T>>>;
+	}
 	/// @endcond
 
 	/// @brief  True if `T` meets the `ImplicitLifetimeType` named requirement.
 	template <typename T>
 	inline constexpr bool is_implicit_lifetime_type =
-		std::is_scalar_v<T> || std::is_array_v<T>
-		|| (std::is_aggregate_v<T> && std::is_trivially_constructible_v<T> && std::is_trivially_destructible_v<T>);
+		POXY_IMPLEMENTATION_DETAIL(detail::is_implicit_lifetime_type_<T>::value);
 
 	/// @brief  Alias for `std::integral_constant<std::size_t, Value>`
 	template <auto Value>
 	using index_constant = std::integral_constant<size_t, static_cast<size_t>(Value)>;
 
 	/// @brief  The type that would result from `std::forward<T>()`.
 	template <typename T>
@@ -228,182 +231,195 @@
 		template <template <typename...> typename Trait, typename Enabler, typename... Args>
 		struct is_detected_impl : std::false_type
 		{};
 		template <template <typename...> typename Trait, typename... Args>
 		struct is_detected_impl<Trait, std::void_t<Trait<Args...>>, Args...> : std::true_type
 		{};
 		template <template <typename...> typename Trait, typename... Args>
-		inline constexpr auto is_detected_ = is_detected_impl<Trait, void, Args...>::value;
+		using is_detected_ = is_detected_impl<Trait, void, Args...>;
 	}
 	/// @endcond
 
-	/// @brief Detects if a Trait can be applied to a set of Args.
+	/// @brief Detects if `Trait` can be applied to a set of `Args`.
 	template <template <typename...> typename Trait, typename... Args>
-	inline constexpr auto is_detected = detail::is_detected_<Trait, Args...>;
+	inline constexpr auto is_detected = POXY_IMPLEMENTATION_DETAIL(detail::is_detected_<Trait, Args...>::value);
 
 	/// @cond
 	namespace detail
 	{
 		template <typename T>
-		using has_swap_member_ = decltype(std::declval<T&>().swap(std::declval<T&>()));
+		using has_swap_member_impl_ = decltype(std::declval<T&>().swap(std::declval<T&>()));
+		template <typename T>
+		using has_swap_member_ = is_detected_<has_swap_member_impl_, T>;
 
 		template <typename T, typename Arg>
-		using has_resize_member_ = decltype(std::declval<T&>().resize(std::declval<const Arg&>()));
+		using has_resize_member_impl_ = decltype(std::declval<T&>().resize(std::declval<const Arg&>()));
+		template <typename T, typename Arg = size_t>
+		using has_resize_member_ = is_detected_<has_resize_member_impl_, T, Arg>;
 
 		template <typename T, typename Arg>
-		using has_erase_member_ = decltype(std::declval<T&>().erase(std::declval<const Arg&>()));
+		using has_erase_member_impl_ = decltype(std::declval<T&>().erase(std::declval<const Arg&>()));
+		template <typename T, typename Arg = size_t>
+		using has_erase_member_ = is_detected_<has_erase_member_impl_, T, Arg>;
 
 		template <typename T, typename Arg>
-		using has_unordered_erase_member_ = decltype(std::declval<T&>().unordered_erase(std::declval<const Arg&>()));
+		using has_unordered_erase_member_impl_ =
+			decltype(std::declval<T&>().unordered_erase(std::declval<const Arg&>()));
+		template <typename T, typename Arg = size_t>
+		using has_unordered_erase_member_ = is_detected_<has_unordered_erase_member_impl_, T, Arg>;
 
 		template <typename T>
-		using has_data_member_ = decltype(std::declval<T&>().data());
+		using has_data_member_impl_ = decltype(std::declval<T&>().data());
+		template <typename T>
+		using has_data_member_ = is_detected_<has_data_member_impl_, T>;
 
 		template <typename T, typename U>
-		using is_equality_comparable_ = decltype(std::declval<const std::remove_reference_t<T>&>()
-												 == std::declval<const std::remove_reference_t<U>&>());
+		using is_equality_comparable_impl_ = decltype(std::declval<const std::remove_reference_t<T>&>()
+													  == std::declval<const std::remove_reference_t<U>&>());
+		template <typename T, typename U = T>
+		using is_equality_comparable_ = is_detected_<is_equality_comparable_impl_, T, U>;
 
 		template <typename T, typename U>
-		using is_less_than_comparable_ = decltype(std::declval<const std::remove_reference_t<T>&>()
-												  < std::declval<const std::remove_reference_t<U>&>());
+		using is_less_than_comparable_impl_ = decltype(std::declval<const std::remove_reference_t<T>&>()
+													   < std::declval<const std::remove_reference_t<U>&>());
+		template <typename T, typename U = T>
+		using is_less_than_comparable_ = is_detected_<is_less_than_comparable_impl_, T, U>;
 	}
 	/// @endcond
 
-	/// @brief	True if `T` has a `swap(T&)` member.
-	template <typename T>
-	inline constexpr bool has_swap_member = is_detected<detail::has_swap_member_, T>;
+	/// @brief	True if all `T` have a `swap(T&)` member.
+	template <typename... T>
+	inline constexpr bool has_swap_member =
+		POXY_IMPLEMENTATION_DETAIL(std::conjunction<detail::has_swap_member_<T>...>::value);
 
-	/// @brief	True if `T` has a `resize(size_t)` member.
-	template <typename T, typename Arg = size_t>
-	inline constexpr bool has_resize_member = is_detected<detail::has_resize_member_, T, Arg>;
+	/// @brief	True if all `T` have a `resize(size_t)` member.
+	template <typename... T>
+	inline constexpr bool has_resize_member =
+		POXY_IMPLEMENTATION_DETAIL(std::conjunction<detail::has_resize_member_<T, size_t>...>::value);
 
-	/// @brief	True if `T` has an `erase(size_t)` member.
-	template <typename T, typename Arg = size_t>
-	inline constexpr bool has_erase_member = is_detected<detail::has_erase_member_, T, Arg>;
+	/// @brief	True if all `T` have an `erase(size_t)` member.
+	template <typename... T>
+	inline constexpr bool has_erase_member =
+		POXY_IMPLEMENTATION_DETAIL(std::conjunction<detail::has_erase_member_<T, size_t>...>::value);
 
-	/// @brief	True if `T` has an `unordered_erase(size_t)` member.
-	template <typename T, typename Arg = size_t>
-	inline constexpr bool has_unordered_erase_member = is_detected<detail::has_unordered_erase_member_, T, Arg>;
+	/// @brief	True if all `T` have an `unordered_erase(size_t)` member.
+	template <typename... T>
+	inline constexpr bool has_unordered_erase_member =
+		POXY_IMPLEMENTATION_DETAIL(std::conjunction<detail::has_unordered_erase_member_<T, size_t>...>::value);
 
-	/// @brief	True if `T` has a `data()` member.
-	template <typename T>
-	inline constexpr bool has_data_member = is_detected<detail::has_data_member_, T>;
+	/// @brief	True if all `T` have a `data()` member.
+	template <typename... T>
+	inline constexpr bool has_data_member =
+		POXY_IMPLEMENTATION_DETAIL(std::conjunction<detail::has_data_member_<T>...>::value);
 
 	/// @brief	True if `T` and `U` meet the `EqualityComparable` named requirement.
 	template <typename T, typename U = T>
-	inline constexpr bool is_equality_comparable = is_detected<detail::is_equality_comparable_, T, U>;
+	inline constexpr bool is_equality_comparable =
+		POXY_IMPLEMENTATION_DETAIL(detail::is_equality_comparable_<T, U>::value);
 
 	/// @brief	True if `T` and `U` meet the `LessThanComparable` named requirement.
 	template <typename T, typename U = T>
-	inline constexpr bool is_less_than_comparable = is_detected<detail::is_less_than_comparable_, T, U>;
+	inline constexpr bool is_less_than_comparable =
+		POXY_IMPLEMENTATION_DETAIL(detail::is_less_than_comparable_<T, U>::value);
 
 	/// @cond
 	namespace detail
 	{
 		template <typename T, bool = has_swap_member<T>>
 		struct has_nothrow_swap_member_ : std::bool_constant<noexcept(std::declval<T&>().swap(std::declval<T&>()))>
 		{};
 		template <typename T>
 		struct has_nothrow_swap_member_<T, false> : std::false_type
 		{};
 
-		template <typename T, typename Arg, bool = has_resize_member<T, Arg>>
+		template <typename T, typename Arg = size_t, bool = has_resize_member<T, Arg>>
 		struct has_nothrow_resize_member_
 			: std::bool_constant<noexcept(std::declval<T&>().resize(std::declval<const Arg&>()))>
 		{};
 		template <typename T, typename Arg>
 		struct has_nothrow_resize_member_<T, Arg, false> : std::false_type
 		{};
 
-		template <typename T, typename Arg, bool = has_erase_member<T, Arg>>
+		template <typename T, typename Arg = size_t, bool = has_erase_member<T, Arg>>
 		struct has_nothrow_erase_member_
 			: std::bool_constant<noexcept(std::declval<T&>().erase(std::declval<const Arg&>()))>
 		{};
 		template <typename T, typename Arg>
 		struct has_nothrow_erase_member_<T, Arg, false> : std::false_type
 		{};
 
-		template <typename T, typename Arg, bool = has_unordered_erase_member<T, Arg>>
+		template <typename T, typename Arg = size_t, bool = has_unordered_erase_member<T, Arg>>
 		struct has_nothrow_unordered_erase_member_
 			: std::bool_constant<noexcept(std::declval<T&>().unordered_erase(std::declval<const Arg&>()))>
 		{};
 		template <typename T, typename Arg>
 		struct has_nothrow_unordered_erase_member_<T, Arg, false> : std::false_type
 		{};
 
 		template <typename T, bool = has_data_member<T>>
 		struct has_nothrow_data_member_ : std::bool_constant<noexcept(std::declval<T&>().data())>
 		{};
 		template <typename T>
 		struct has_nothrow_data_member_<T, false> : std::false_type
 		{};
 
-		template <typename T, typename U, bool = is_equality_comparable<T, U>>
+		template <typename T, typename U = T, bool = is_equality_comparable<T, U>>
 		struct is_nothrow_equality_comparable_
 			: std::bool_constant<noexcept(std::declval<const std::remove_reference_t<T>&>()
 										  == std::declval<const std::remove_reference_t<U>&>())>
 		{};
 		template <typename T, typename U>
 		struct is_nothrow_equality_comparable_<T, U, false> : std::false_type
 		{};
 
-		template <typename T, typename U, bool = is_less_than_comparable<T, U>>
+		template <typename T, typename U = T, bool = is_less_than_comparable<T, U>>
 		struct is_nothrow_less_than_comparable_
 			: std::bool_constant<noexcept(std::declval<const std::remove_reference_t<T>&>()
 										  < std::declval<const std::remove_reference_t<U>&>())>
 		{};
 		template <typename T, typename U>
 		struct is_nothrow_less_than_comparable_<T, U, false> : std::false_type
 		{};
 	}
 	/// @endcond
 
-	/// @brief	True if `T` has a non-throwing `swap(T&)` member.
-	template <typename T>
-	inline constexpr bool has_nothrow_swap_member = detail::has_nothrow_swap_member_<T>::value;
+	/// @brief	True if all `T` have a non-throwing `swap(T&)` member.
+	template <typename... T>
+	inline constexpr bool has_nothrow_swap_member =
+		POXY_IMPLEMENTATION_DETAIL(std::conjunction<detail::has_nothrow_swap_member_<T>...>::value);
 
-	/// @brief	True if `T` has a non-throwing `resize(size_t)` member.
-	template <typename T, typename Arg = size_t>
-	inline constexpr bool has_nothrow_resize_member = detail::has_nothrow_resize_member_<T, Arg>::value;
+	/// @brief	True if all `T` have a non-throwing `resize(size_t)` member.
+	template <typename... T>
+	inline constexpr bool has_nothrow_resize_member =
+		POXY_IMPLEMENTATION_DETAIL(std::conjunction<detail::has_nothrow_resize_member_<T, size_t>...>::value);
 
-	/// @brief	True if `T` has a non-throwing `erase(size_t)` member.
-	template <typename T, typename Arg = size_t>
-	inline constexpr bool has_nothrow_erase_member = detail::has_nothrow_erase_member_<T, Arg>::value;
+	/// @brief	True if all `T` have a non-throwing `erase(size_t)` member.
+	template <typename... T>
+	inline constexpr bool has_nothrow_erase_member =
+		POXY_IMPLEMENTATION_DETAIL(std::conjunction<detail::has_nothrow_erase_member_<T, size_t>...>::value);
 
-	/// @brief	True if `T` has a non-throwing `unordered_erase(size_t)` member.
-	template <typename T, typename Arg = size_t>
+	/// @brief	True if all `T` have a non-throwing `unordered_erase(size_t)` member.
+	template <typename... T>
 	inline constexpr bool has_nothrow_unordered_erase_member =
-		detail::has_nothrow_unordered_erase_member_<T, Arg>::value;
+		POXY_IMPLEMENTATION_DETAIL(std::conjunction<detail::has_nothrow_unordered_erase_member_<T, size_t>...>::value);
 
-	/// @brief	True if `T` has a non-throwing `data()` member.
-	template <typename T>
-	inline constexpr bool has_nothrow_data_member = detail::has_nothrow_data_member_<T>::value;
+	/// @brief	True if all `T` have a non-throwing `data()` member.
+	template <typename... T>
+	inline constexpr bool has_nothrow_data_member =
+		POXY_IMPLEMENTATION_DETAIL(std::conjunction<detail::has_nothrow_data_member_<T>...>::value);
 
 	/// @brief	True if `T` and `U` meet the `EqualityComparable` named requirement without throwing.
 	template <typename T, typename U = T>
-	inline constexpr bool is_nothrow_equality_comparable = detail::is_nothrow_equality_comparable_<T, U>::value;
+	inline constexpr bool is_nothrow_equality_comparable =
+		POXY_IMPLEMENTATION_DETAIL(detail::is_nothrow_equality_comparable_<T, U>::value);
 
 	/// @brief	True if `T` and `U` meet the `LessThanComparable` named requirement without throwing.
 	template <typename T, typename U = T>
-	inline constexpr bool is_nothrow_less_than_comparable = detail::is_nothrow_less_than_comparable_<T, U>::value;
-
-	/// @cond
-	namespace detail
-	{
-		template <typename T>
-		using has_tuple_size_ = decltype(std::tuple_size<remove_cvref<T>>::value);
-		template <typename T>
-		using has_tuple_element_ = decltype(std::declval<typename std::tuple_element<0, remove_cvref<T>>::type>());
-	}
-	/// @endcond
-
-	/// @brief	True if `T` implements std::tuple_size and std::tuple_element.
-	template <typename T>
-	inline constexpr bool is_tuple_like =
-		is_detected<detail::has_tuple_size_, T> && is_detected<detail::has_tuple_element_, T>;
+	inline constexpr bool is_nothrow_less_than_comparable =
+		POXY_IMPLEMENTATION_DETAIL(detail::is_nothrow_less_than_comparable_<T, U>::value);
 
 #if !SOAGEN_DOXYGEN && SOAGEN_HAS_BUILTIN(__type_pack_element)
 
 	template <size_t I, typename... T>
 	using type_at_index = __type_pack_element<I, T...>;
 
 #else
@@ -442,14 +458,19 @@
 	}
 	/// @endcond
 
 	/// @brief Gets the underlying #soagen::table of an SoA type.
 	template <typename T>
 	using table_type = POXY_IMPLEMENTATION_DETAIL(typename detail::table_type_<std::remove_cv_t<T>>::type);
 
+	/// @brief True if two types have the same underlying #soagen::table type.
+	template <typename A, typename B>
+	inline constexpr bool same_table_type =
+		POXY_IMPLEMENTATION_DETAIL(std::is_same_v<table_type<remove_cvref<A>>, table_type<remove_cvref<B>>>);
+
 	/// @cond
 	namespace detail
 	{
 		template <typename T>
 		struct table_traits_type_
 		{
 			using type = typename T::table_traits;
@@ -612,161 +633,52 @@
 	}
 	/// @endcond
 
 	/// @brief		The type soagen will use for a column in rvalue parameter contexts (e.g. `push_back(&&)`).
 	template <typename ParamType>
 	using rvalue_type = POXY_IMPLEMENTATION_DETAIL(typename detail::rvalue_type_<ParamType>::type);
 
-	/// @brief Helper class for #table::emplace() and #table::emplace_back().
-	template <typename... Args>
-	struct emplacer
-	{
-		static_assert(sizeof...(Args));
-		static_assert((std::is_reference_v<Args> && ...));
-
-		void* ptrs[sizeof...(Args)];
-
-		SOAGEN_DEFAULT_RULE_OF_FIVE(emplacer);
-
-		SOAGEN_NODISCARD_CTOR
-		constexpr emplacer(Args&&... args) noexcept //
-			: ptrs{ const_cast<void*>(static_cast<const volatile void*>(&args))... }
-		{}
-	};
-
-	/// @cond
-	template <>
-	struct emplacer<>
-	{};
-	template <typename... Args>
-	emplacer(Args&&...) -> emplacer<Args&&...>;
-	/// @endcond
-
-	/// @brief True if `T` is an instance of #soagen::emplacer.
-	template <typename T>
-	inline constexpr bool is_emplacer = POXY_IMPLEMENTATION_DETAIL(false);
-	/// @cond
-	template <typename... T>
-	inline constexpr bool is_emplacer<emplacer<T...>> = true;
-	template <typename T>
-	inline constexpr bool is_emplacer<const T> = is_emplacer<T>;
-	template <typename T>
-	inline constexpr bool is_emplacer<volatile T> = is_emplacer<T>;
-	template <typename T>
-	inline constexpr bool is_emplacer<const volatile T> = is_emplacer<T>;
-	/// @endcond
-
 	/// @cond
 	namespace detail
 	{
-		// note: this machinery is so that we only instantiate the is_nothrow version
-		// when the regular version is true
+		// machinery to only instantiate one or more secondary traits when the primary one is true
+		// e.g. for traits that come in pairs like is_invocable / is_nothrow_invocable
 
 		template <typename...>
-		struct is_nothrow_invocable_indirect_ : std::false_type
-		{};
+		struct types_;
 
-		template <typename Func, typename... Args>
-		struct is_nothrow_invocable_indirect_<std::true_type, Func, Args...> : std::is_nothrow_invocable<Func, Args...>
+		template <bool, template <typename...> typename, typename...>
+		struct nested_trait_indirect_ : std::false_type
 		{};
 
-		template <typename Func, typename... Args>
-		struct is_invocable_ : std::is_invocable<Func, Args...>
-		{
-			using is_nothrow =
-				is_nothrow_invocable_indirect_<std::bool_constant<std::is_invocable<Func, Args...>::value>,
-											   Func,
-											   Args...>;
-		};
-	}
-	/// @endcond
-
-	/// @brief	True if `Func` is invocable with `Args`.
-	template <typename Func, typename... Args>
-	inline constexpr bool is_invocable = detail::is_invocable_<Func, Args...>::value;
-
-	/// @brief	True if `Func` is nothrow-invocable with `Args`.
-	template <typename Func, typename... Args>
-	inline constexpr bool is_nothrow_invocable = detail::is_invocable_<Func, Args...>::is_nothrow::value;
-
-	/// @cond
-	namespace detail
-	{
-		template <size_t I, typename Func, typename Arg>
-		struct is_invocable_with_optional_index_							//
-			: std::disjunction<is_invocable_<Func, Arg, index_constant<I>>, //
-							   is_invocable_<Func, Arg, size_t>,			//
-							   is_invocable_<Func, index_constant<I>, Arg>, //
-							   is_invocable_<Func, size_t, Arg>,			//
-							   is_invocable_<Func, Arg>>
+		template <template <typename...> typename Trait, typename... Args>
+		struct nested_trait_indirect_<true, Trait, Args...> : Trait<Args...>
 		{};
-	}
-	/// @endcond
-
-	/// @brief	True if `Func` is invocable with `Arg` and an index_constant and/or size_t.
-	template <size_t I, typename Func, typename Arg>
-	inline constexpr bool is_invocable_with_optional_index =
-		detail::is_invocable_with_optional_index_<I, Func, Arg>::value;
 
-	/// @brief	True if `Func` is nothrow-invocable with `Arg` and an index_constant and/or size_t.
-	template <size_t I, typename Func, typename Arg>
-	inline constexpr bool is_nothrow_invocable_with_optional_index =
-		detail::is_invocable_with_optional_index_<I, Func, Arg>::is_nothrow::value;
+		template <typename, template <typename...> typename, template <typename...> typename...>
+		struct nested_trait_;
 
-	template <size_t I, typename Func, typename Arg>
-	SOAGEN_ALWAYS_INLINE
-	constexpr decltype(auto) invoke_with_optional_index(Func&& func,
-														Arg&& arg) //
-		noexcept(is_nothrow_invocable_with_optional_index<I, Func&&, Arg&&>)
-	{
-		static_assert(is_invocable_with_optional_index<I, Func&&, Arg&&>);
-
-		if constexpr (is_invocable<Func&&, Arg&&, index_constant<I>>)
-		{
-			return static_cast<Func&&>(func)(static_cast<Arg&&>(arg), index_constant<I>{});
-		}
-		else if constexpr (is_invocable<Func&&, Arg&&, size_t>)
-		{
-			return static_cast<Func&&>(func)(static_cast<Arg&&>(arg), I);
-		}
-		else if constexpr (is_invocable<Func&&, index_constant<I>, Arg&&>)
-		{
-			return static_cast<Func&&>(func)(index_constant<I>{}, static_cast<Arg&&>(arg));
-		}
-		else if constexpr (is_invocable<Func&&, size_t, Arg&&>)
+		template <template <typename...> typename Trait,
+				  template <typename...>
+				  typename... NestedTraits,
+				  typename... Args>
+		struct nested_trait_<types_<Args...>, Trait, NestedTraits...> : Trait<Args...>
 		{
-			return static_cast<Func&&>(func)(I, static_cast<Arg&&>(arg));
-		}
-		else
-		{
-			static_assert(is_invocable<Func&&, Arg&&>);
-
-			return static_cast<Func&&>(func)(static_cast<Arg&&>(arg));
-		}
+			template <size_t Index>
+			using nested =
+				type_at_index<Index, nested_trait_indirect_<Trait<Args...>::value, NestedTraits, Args...>...>;
+		};
 	}
+	/// @endcond
 
 	/// @cond
 	namespace detail
 	{
 		template <typename Table, size_t ColumnIndex>
 		struct column_name;
 		template <typename Table, size_t ColumnIndex>
 		struct column_ref;
-
-		template <typename A, typename B>
-		inline constexpr bool same_table_type =
-			std::is_same_v<table_type<remove_cvref<A>>, table_type<remove_cvref<B>>>;
 	}
 	/// @endcond
 }
 
-/// @cond
-namespace std
-{
-	template <typename... Args>
-	struct tuple_size<soagen::emplacer<Args...>> //
-		: std::integral_constant<size_t, sizeof...(Args)>
-	{};
-}
-/// @endcond
-
 #include "header_end.hpp"
```

### Comparing `soagen-0.3.0/src/soagen/hpp/generated/compressed_pair.hpp` & `soagen-0.4.0/src/soagen/hpp/generated/compressed_pair.hpp`

 * *Files identical despite different names*

### Comparing `soagen-0.3.0/src/soagen/hpp/generated/functions.hpp` & `soagen-0.4.0/src/soagen/hpp/generated/functions.hpp`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 //#---------------------------------------------------------------------------------------------------------------------
 //#     !!!!! THIS FILE WAS ASSEMBLED FROM MULTIPLE HEADER FILES BY A SCRIPT - PLEASE DON'T EDIT IT DIRECTLY !!!!!
 //#---------------------------------------------------------------------------------------------------------------------
 
 #pragma once
 
 #include "../core.hpp"
-#if SOAGEN_CPP >= 20 && defined(__cpp_lib_bit_cast) && __cpp_lib_bit_cast >= 201806
-	#include <bit>
-#endif
 #include "../header_start.hpp"
 
 namespace soagen
 {
 	SOAGEN_CONST_INLINE_GETTER
 	constexpr bool is_constant_evaluated() noexcept
 	{
@@ -161,92 +158,10 @@
 				return ptr;
 
 #endif
 			}
 		}
 	}
 
-	namespace detail
-	{
-		template <typename T>
-		using has_tuple_get_member_ = decltype(std::declval<T>().template get<0>());
-	}
-
-	template <size_t I, typename T>
-	SOAGEN_NODISCARD
-	SOAGEN_ALWAYS_INLINE
-	constexpr decltype(auto) get_from_tuple_like(T&& tuple_like) noexcept
-	{
-		if constexpr (is_detected<detail::has_tuple_get_member_, T&&>)
-		{
-			return static_cast<T&&>(tuple_like).template get<I>();
-		}
-		else // adl
-		{
-			using std::get;
-			return get<I>(static_cast<T&&>(tuple_like));
-		}
-	}
-
-#if SOAGEN_CPP >= 20 && defined(__cpp_lib_bit_cast) && __cpp_lib_bit_cast >= 201806
-
-	#define SOAGEN_HAS_INTRINSIC_BIT_CAST 1
-
-	using std::bit_cast;
-
-#else
-
-	SOAGEN_CONSTRAINED_TEMPLATE((std::is_trivially_copyable_v<From>	 //
-								 && std::is_trivially_copyable_v<To> //
-								 && sizeof(From) == sizeof(To)),
-								typename To,
-								typename From)
-	SOAGEN_PURE_INLINE_GETTER
-	constexpr To bit_cast(const From& from) noexcept
-	{
-		static_assert(!std::is_reference_v<To> && !std::is_reference_v<From>);
-
-	#if SOAGEN_CLANG >= 11 || SOAGEN_GCC >= 11 || SOAGEN_MSVC >= 1926                                                  \
-		|| (!SOAGEN_CLANG && !SOAGEN_GCC && SOAGEN_HAS_BUILTIN(__builtin_bit_cast))
-
-		#define SOAGEN_HAS_INTRINSIC_BIT_CAST 1
-		return __builtin_bit_cast(To, from);
-
-	#else
-
-		#define SOAGEN_HAS_INTRINSIC_BIT_CAST 0
-
-		if constexpr (std::is_same_v<std::remove_cv_t<From>, std::remove_cv_t<To>>)
-		{
-			return from;
-		}
-		else if constexpr (!std::is_nothrow_default_constructible_v<std::remove_cv_t<To>>)
-		{
-			union proxy_t
-			{
-				alignas(To) unsigned char dummy[sizeof(To)];
-				std::remove_cv_t<To> to;
-
-				proxy_t() noexcept
-				{}
-			};
-
-			proxy_t proxy;
-			std::memcpy(&proxy.to, &from, sizeof(To));
-			return proxy.to;
-		}
-		else
-		{
-			static_assert(std::is_nothrow_default_constructible_v<std::remove_cv_t<To>>,
-						  "Bit-cast fallback requires the To type be nothrow default-constructible");
-
-			std::remove_cv_t<To> to;
-			std::memcpy(&to, &from, sizeof(To));
-			return to;
-		}
-	#endif
-	}
-
-#endif
 }
 
 #include "../header_end.hpp"
```

### Comparing `soagen-0.3.0/src/soagen/hpp/generated/preprocessor.hpp` & `soagen-0.4.0/src/soagen/hpp/generated/preprocessor.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -481,25 +481,14 @@
 	#if !SOAGEN_DOXYGEN
 		#define SOAGEN_HIDDEN_CONSTRAINT(condition, ...) SOAGEN_CONSTRAINED_TEMPLATE(condition, __VA_ARGS__)
 	#else
 		#define SOAGEN_HIDDEN_CONSTRAINT(condition, ...)
 	#endif
 #endif
 
-/// @cond
-#ifndef SOAGEN_CONSTRAINED_COLUMN
-	#define SOAGEN_CONSTRAINED_COLUMN(I, ...)                                                                          \
-		SOAGEN_CONSTRAINED_TEMPLATE(sfinae_col_idx == static_cast<std::size_t>(I) && (__VA_ARGS__),                    \
-									std::size_t sfinae_col_idx = static_cast<std::size_t>(I))
-#endif
-/// @endcond
-#ifndef SOAGEN_CONSTRAINED_COLUMN
-	#define SOAGEN_CONSTRAINED_COLUMN(I, ...)
-#endif
-
 #ifndef SOAGEN_PUSH_WARNINGS
 	#if SOAGEN_CLANG
 		#define SOAGEN_PUSH_WARNINGS                                                                                   \
 			_Pragma("clang diagnostic push")                                                                           \
 			static_assert(true)
 	#elif SOAGEN_MSVC || SOAGEN_ICC
 		#define SOAGEN_PUSH_WARNINGS                                                                                   \
@@ -924,27 +913,14 @@
 					}                                                                                                  \
 				}                                                                                                      \
 			}                                                                                                          \
 			while (false)
 	#endif
 #endif
 
-#ifndef SOAGEN_COLUMN
-	#define SOAGEN_COLUMN(I)                                                                                           \
-		SOAGEN_PURE_INLINE_GETTER                                                                                      \
-		SOAGEN_ATTR(returns_nonnull)
-#endif
-
-#ifndef SOAGEN_ALIGNED_COLUMN
-	#define SOAGEN_ALIGNED_COLUMN(I)                                                                                   \
-		SOAGEN_COLUMN(I)                                                                                               \
-		SOAGEN_ATTR(assume_aligned(                                                                                    \
-			soagen::detail::actual_column_alignment<table_traits, allocator_type, static_cast<std::size_t>(I)>))
-#endif
-
 #ifndef SOAGEN_ALWAYS_OPTIMIZE
 	#define SOAGEN_ALWAYS_OPTIMIZE 1
 #endif
 
 #ifndef SOAGEN_COMMA
 	#define SOAGEN_COMMA ,
 #endif
```

### Comparing `soagen-0.3.0/src/soagen/hpp/header_end.hpp` & `soagen-0.4.0/src/soagen/hpp/header_end.hpp`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 //# See https://github.com/marzer/soagen/blob/master/LICENSE for the full license text.
 //# SPDX-License-Identifier: MIT
 
 //# note: this header is the exact reverse of header_start.hpp
 
 #include "generated/preprocessor.hpp"
 
+// __SOAGEN_HEADER_END{{
+
 //# reset optimizations
 #if SOAGEN_ALWAYS_OPTIMIZE
 	#if SOAGEN_MSVC
 		#pragma strict_gs_check(pop)
 		#pragma runtime_checks("", restore)
 		#pragma optimize("", on)
 		#pragma inline_recursion(off)
@@ -23,7 +25,9 @@
 #if SOAGEN_MSVC_LIKE
 	#pragma pop_macro("min")
 	#pragma pop_macro("max")
 #endif
 
 //# pop the current warning state
 SOAGEN_POP_WARNINGS;
+
+// }}__SOAGEN_HEADER_END
```

### Comparing `soagen-0.3.0/src/soagen/hpp/header_start.hpp` & `soagen-0.4.0/src/soagen/hpp/header_start.hpp`

 * *Files 20% similar despite different names*

```diff
@@ -3,17 +3,22 @@
 //# See https://github.com/marzer/soagen/blob/master/LICENSE for the full license text.
 //# SPDX-License-Identifier: MIT
 
 //# note: any preprocessor/compiler state modified here must be undone in header_end.hpp
 
 #include "generated/preprocessor.hpp"
 
+// __SOAGEN_HEADER_START{{
+
 //# push the current warning state
 SOAGEN_PUSH_WARNINGS;
 SOAGEN_DISABLE_SPAM_WARNINGS;
+#if SOAGEN_CLANG >= 16
+	#pragma clang diagnostic ignored "-Wunsafe-buffer-usage"
+#endif
 
 //# disable windows.h min/max macro crimes
 #if SOAGEN_MSVC_LIKE
 	#pragma push_macro("min")
 	#pragma push_macro("max")
 	#undef min
 	#undef max
@@ -27,7 +32,9 @@
 		#pragma runtime_checks("", off)
 		#pragma strict_gs_check(push, off)
 	#elif SOAGEN_GCC
 		#pragma GCC push_options
 		#pragma GCC optimize("O2")
 	#endif
 #endif
+
+// }}__SOAGEN_HEADER_START
```

### Comparing `soagen-0.3.0/src/soagen/hpp/iterator.hpp` & `soagen-0.4.0/src/soagen/hpp/iterator.hpp`

 * *Files 14% similar despite different names*

```diff
@@ -1,79 +1,21 @@
 //# This file is a part of marzer/soagen and is subject to the the terms of the MIT license.
 //# Copyright (c) Mark Gillard <mark.gillard@outlook.com.au>
 //# See https://github.com/marzer/soagen/blob/master/LICENSE for the full license text.
 //# SPDX-License-Identifier: MIT
 #pragma once
 
 #include "row.hpp"
-SOAGEN_DISABLE_WARNINGS;
-#include <iterator>
-SOAGEN_ENABLE_WARNINGS;
 #include "header_start.hpp"
 
 namespace soagen
 {
 	/// @cond
-	template <typename, size_t...>
-	class iterator;
-
 	namespace detail
 	{
-		// iterator implicit conversions are allowed when:
-		// - changing columns
-		// - losing rvalue (Table&& -> Table&), (const Table&& -> const Table&)
-		// - gaining const (Table& -> const Table&, Table&& -> const Table&&)
-		// - any combination of the three
-
-		template <typename From, typename To>
-		inline constexpr bool iterator_implicit_conversion_ok = false;
-
-		template <typename Table, size_t... ColumnsA, size_t... ColumnsB>
-		inline constexpr bool iterator_implicit_conversion_ok<iterator<Table, ColumnsA...>, //
-															  iterator<Table, ColumnsB...>> = true;
-
-		template <typename Table, size_t... ColumnsA, size_t... ColumnsB>
-		inline constexpr bool iterator_implicit_conversion_ok<iterator<Table&&, ColumnsA...>, //
-															  iterator<Table&, ColumnsB...>> = true;
-
-		template <typename Table, size_t... ColumnsA, size_t... ColumnsB>
-		inline constexpr bool iterator_implicit_conversion_ok<iterator<const Table&&, ColumnsA...>, //
-															  iterator<const Table&, ColumnsB...>> = true;
-
-		template <typename Table, size_t... ColumnsA, size_t... ColumnsB>
-		inline constexpr bool iterator_implicit_conversion_ok<iterator<Table&, ColumnsA...>, //
-															  iterator<const Table&, ColumnsB...>> = true;
-
-		template <typename Table, size_t... ColumnsA, size_t... ColumnsB>
-		inline constexpr bool iterator_implicit_conversion_ok<iterator<Table&&, ColumnsA...>, //
-															  iterator<const Table&&, ColumnsB...>> = true;
-
-		template <typename Table, size_t... ColumnsA, size_t... ColumnsB>
-		inline constexpr bool iterator_implicit_conversion_ok<iterator<Table&&, ColumnsA...>, //
-															  iterator<const Table&, ColumnsB...>> = true;
-
-		// iterator explicit conversions are allowed when gaining rvalue and optionally gaining const
-		// (note that we specifically avoid providing anything that would be the moral equivalent of
-		// a const_cast because that armory is filled with very large and powerful footguns)
-
-		template <typename From, typename To>
-		inline constexpr bool iterator_explicit_conversion_ok = false;
-
-		template <typename Table, size_t... ColumnsA, size_t... ColumnsB>
-		inline constexpr bool iterator_explicit_conversion_ok<iterator<Table&, ColumnsA...>, //
-															  iterator<Table&&, ColumnsB...>> = true;
-
-		template <typename Table, size_t... ColumnsA, size_t... ColumnsB>
-		inline constexpr bool iterator_explicit_conversion_ok<iterator<const Table&, ColumnsA...>, //
-															  iterator<const Table&&, ColumnsB...>> = true;
-
-		template <typename Table, size_t... ColumnsA, size_t... ColumnsB>
-		inline constexpr bool iterator_explicit_conversion_ok<iterator<Table&, ColumnsA...>, //
-															  iterator<const Table&&, ColumnsB...>> = true;
-
 		template <typename T>
 		struct arrow_proxy
 		{
 			mutable T value;
 
 			SOAGEN_PURE_INLINE_GETTER
 			constexpr T* operator->() const noexcept
@@ -235,15 +177,15 @@
 
 		/// @}
 
 		/// @name Difference
 		/// @{
 
 		/// @brief Returns the difference between two iterators.
-		SOAGEN_CONSTRAINED_TEMPLATE((detail::same_table_type<Table, T>), typename T, size_t... Cols)
+		SOAGEN_CONSTRAINED_TEMPLATE((same_table_type<Table, T>), typename T, size_t... Cols)
 		SOAGEN_PURE_GETTER
 		constexpr difference_type operator-(const iterator<T, Cols...>& rhs) const noexcept
 		{
 			return base::offset - rhs.offset;
 		}
 
 		/// @}
@@ -282,60 +224,60 @@
 
 		/// @}
 
 		/// @name Equality
 		/// @{
 
 		/// @brief Returns true if two iterators refer to the same row in the same table.
-		SOAGEN_CONSTRAINED_TEMPLATE((detail::same_table_type<Table, T>), typename T, size_t... Cols)
+		SOAGEN_CONSTRAINED_TEMPLATE((same_table_type<Table, T>), typename T, size_t... Cols)
 		SOAGEN_PURE_GETTER
 		constexpr bool operator==(const iterator<T, Cols...>& rhs) const noexcept
 		{
 			return base::table == rhs.table && base::offset == rhs.offset;
 		}
 
 		/// @brief Returns true if two iterators do not refer to the same row in the same table.
-		SOAGEN_CONSTRAINED_TEMPLATE((detail::same_table_type<Table, T>), typename T, size_t... Cols)
+		SOAGEN_CONSTRAINED_TEMPLATE((same_table_type<Table, T>), typename T, size_t... Cols)
 		SOAGEN_PURE_INLINE_GETTER
 		friend constexpr bool operator!=(const iterator& lhs, const iterator<T, Cols...>& rhs) noexcept
 		{
 			return !(lhs == rhs);
 		}
 
 		/// @}
 
 		/// @name Comparison
 		/// @{
 
 		/// @brief Returns true if the LHS iterator refers to a row less-than the RHS iterator.
-		SOAGEN_CONSTRAINED_TEMPLATE((detail::same_table_type<Table, T>), typename T, size_t... Cols)
+		SOAGEN_CONSTRAINED_TEMPLATE((same_table_type<Table, T>), typename T, size_t... Cols)
 		SOAGEN_PURE_INLINE_GETTER
 		constexpr bool operator<(const iterator<T, Cols...>& rhs) const noexcept
 		{
 			return base::offset < rhs.offset;
 		}
 
 		/// @brief Returns true if the LHS iterator refers to a row less-than-or-equal-to the RHS iterator.
-		SOAGEN_CONSTRAINED_TEMPLATE((detail::same_table_type<Table, T>), typename T, size_t... Cols)
+		SOAGEN_CONSTRAINED_TEMPLATE((same_table_type<Table, T>), typename T, size_t... Cols)
 		SOAGEN_PURE_INLINE_GETTER
 		constexpr bool operator<=(const iterator<T, Cols...>& rhs) const noexcept
 		{
 			return base::offset <= rhs.offset;
 		}
 
 		/// @brief Returns true if the LHS iterator refers to a row greater-than the RHS iterator.
-		SOAGEN_CONSTRAINED_TEMPLATE((detail::same_table_type<Table, T>), typename T, size_t... Cols)
+		SOAGEN_CONSTRAINED_TEMPLATE((same_table_type<Table, T>), typename T, size_t... Cols)
 		SOAGEN_PURE_INLINE_GETTER
 		constexpr bool operator>(const iterator<T, Cols...>& rhs) const noexcept
 		{
 			return base::offset > rhs.offset;
 		}
 
 		/// @brief Returns true if the LHS iterator refers to a row greater-than-or-equal-to the RHS iterator.
-		SOAGEN_CONSTRAINED_TEMPLATE((detail::same_table_type<Table, T>), typename T, size_t... Cols)
+		SOAGEN_CONSTRAINED_TEMPLATE((same_table_type<Table, T>), typename T, size_t... Cols)
 		SOAGEN_PURE_INLINE_GETTER
 		constexpr bool operator>=(const iterator<T, Cols...>& rhs) const noexcept
 		{
 			return base::offset >= rhs.offset;
 		}
 
 		/// @}
@@ -358,29 +300,28 @@
 		/// </table>
 		///
 		///	@note	Any of these conversions can also change the columns viewed by the iterator - iterators to a table
 		///			share the same underlying data structure regardless of the columns they are viewing.
 		///
 		/// @attention 	There are no conversions provided which offer the equivalent of a `const_cast`-by-proxy.
 		///				This is by design.
-		///
-		SOAGEN_CONSTRAINED_TEMPLATE((detail::iterator_implicit_conversion_ok<iterator, iterator<T, Cols...>>
-									 && !detail::iterator_explicit_conversion_ok<iterator, iterator<T, Cols...>>),
+		SOAGEN_CONSTRAINED_TEMPLATE((detail::implicit_conversion_ok<Table, T>
+									 && !detail::explicit_conversion_ok<Table, T>),
 									typename T,
 									size_t... Cols)
 		SOAGEN_PURE_INLINE_GETTER
 		constexpr operator iterator<T, Cols...>() const noexcept
 		{
 			return iterator<T, Cols...>{ static_cast<const base&>(*this) };
 		}
 
 		/// @cond
 
-		SOAGEN_CONSTRAINED_TEMPLATE((!detail::iterator_implicit_conversion_ok<iterator, iterator<T, Cols...>>
-									 && detail::iterator_explicit_conversion_ok<iterator, iterator<T, Cols...>>),
+		SOAGEN_CONSTRAINED_TEMPLATE((!detail::implicit_conversion_ok<Table, T>
+									 && detail::explicit_conversion_ok<Table, T>),
 									typename T,
 									size_t... Cols)
 		SOAGEN_PURE_INLINE_GETTER
 		explicit constexpr operator iterator<T, Cols...>() const noexcept
 		{
 			return iterator<T, Cols...>{ static_cast<const base&>(*this) };
 		}
```

### Comparing `soagen-0.3.0/src/soagen/hpp/mixins.hpp` & `soagen-0.4.0/src/soagen/hpp/mixins.hpp`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 //# This file is a part of marzer/soagen and is subject to the the terms of the MIT license.
 //# Copyright (c) Mark Gillard <mark.gillard@outlook.com.au>
 //# See https://github.com/marzer/soagen/blob/master/LICENSE for the full license text.
 //# SPDX-License-Identifier: MIT
 #pragma once
 
-#include "core.hpp"
+#include "column_traits.hpp"
+#include "header_start.hpp"
 
 namespace soagen::mixins
 {
 	//--- resize() -----------------------------------------------------------------------------------------------------
 
-	template <typename Derived, bool = has_resize_member<table_type<Derived>, typename table_type<Derived>::size_type>>
+	template <typename Derived, bool = has_resize_member<table_type<Derived>>>
 	struct SOAGEN_EMPTY_BASES resizable
 	{
 		using table_type = soagen::table_type<Derived>;
 		using size_type	 = typename table_type::size_type;
 
 		SOAGEN_ALWAYS_INLINE
 		SOAGEN_CPP20_CONSTEXPR
 		Derived& resize(size_type new_size) //
-			noexcept(soagen::has_nothrow_resize_member<table_type, size_type>)
+			noexcept(soagen::has_nothrow_resize_member<table_type>)
 		{
 			static_cast<Derived&>(*this).table().resize(new_size);
 			return static_cast<Derived&>(*this);
 		}
 	};
 
 	template <typename Derived>
@@ -162,7 +163,9 @@
 		}
 	};
 
 	template <typename Derived>
 	struct SOAGEN_EMPTY_BASES const_data_ptr<Derived, false>
 	{};
 }
+
+#include "header_end.hpp"
```

### Comparing `soagen-0.3.0/src/soagen/hpp/single/soagen.hpp` & `soagen-0.4.0/src/soagen/hpp/single/soagen.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 //----------------------------------------------------------------------------------------------------------------------
 //
-// soagen.hpp v0.3.0
+// soagen.hpp v0.4.0
 // https://github.com/marzer/soagen
 // SPDX-License-Identifier: MIT
 //
 //----------------------------------------------------------------------------------------------------------------------
 //     !!!!! THIS FILE WAS ASSEMBLED FROM MULTIPLE HEADER FILES BY A SCRIPT - PLEASE DON'T EDIT IT DIRECTLY !!!!!
 //----------------------------------------------------------------------------------------------------------------------
 //
@@ -28,17 +28,17 @@
 //----------------------------------------------------------------------------------------------------------------------
 #ifndef SOAGEN_HPP
 #define SOAGEN_HPP
 
 //********  generated/version.hpp  *************************************************************************************
 
 #define SOAGEN_VERSION_MAJOR 0
-#define SOAGEN_VERSION_MINOR 3
+#define SOAGEN_VERSION_MINOR 4
 #define SOAGEN_VERSION_PATCH 0
-#define SOAGEN_VERSION_STRING "0.3.0"
+#define SOAGEN_VERSION_STRING "0.4.0"
 
 //********  generated/preprocessor.hpp  ********************************************************************************
 
 #ifndef SOAGEN_CPP
 	#ifdef _MSVC_LANG
 		#if _MSVC_LANG > __cplusplus
 			#define SOAGEN_CPP _MSVC_LANG
@@ -515,24 +515,14 @@
 	#if !SOAGEN_DOXYGEN
 		#define SOAGEN_HIDDEN_CONSTRAINT(condition, ...) SOAGEN_CONSTRAINED_TEMPLATE(condition, __VA_ARGS__)
 	#else
 		#define SOAGEN_HIDDEN_CONSTRAINT(condition, ...)
 	#endif
 #endif
 
-#ifndef SOAGEN_CONSTRAINED_COLUMN
-	#define SOAGEN_CONSTRAINED_COLUMN(I, ...)                                                                          \
-		SOAGEN_CONSTRAINED_TEMPLATE(sfinae_col_idx == static_cast<std::size_t>(I) && (__VA_ARGS__),                    \
-									std::size_t sfinae_col_idx = static_cast<std::size_t>(I))
-#endif
-
-#ifndef SOAGEN_CONSTRAINED_COLUMN
-	#define SOAGEN_CONSTRAINED_COLUMN(I, ...)
-#endif
-
 #ifndef SOAGEN_PUSH_WARNINGS
 	#if SOAGEN_CLANG
 		#define SOAGEN_PUSH_WARNINGS                                                                                   \
 			_Pragma("clang diagnostic push")                                                                           \
 			static_assert(true)
 	#elif SOAGEN_MSVC || SOAGEN_ICC
 		#define SOAGEN_PUSH_WARNINGS                                                                                   \
@@ -957,27 +947,14 @@
 					}                                                                                                  \
 				}                                                                                                      \
 			}                                                                                                          \
 			while (false)
 	#endif
 #endif
 
-#ifndef SOAGEN_COLUMN
-	#define SOAGEN_COLUMN(I)                                                                                           \
-		SOAGEN_PURE_INLINE_GETTER                                                                                      \
-		SOAGEN_ATTR(returns_nonnull)
-#endif
-
-#ifndef SOAGEN_ALIGNED_COLUMN
-	#define SOAGEN_ALIGNED_COLUMN(I)                                                                                   \
-		SOAGEN_COLUMN(I)                                                                                               \
-		SOAGEN_ATTR(assume_aligned(                                                                                    \
-			soagen::detail::actual_column_alignment<table_traits, allocator_type, static_cast<std::size_t>(I)>))
-#endif
-
 #ifndef SOAGEN_ALWAYS_OPTIMIZE
 	#define SOAGEN_ALWAYS_OPTIMIZE 1
 #endif
 
 #ifndef SOAGEN_COMMA
 	#define SOAGEN_COMMA ,
 #endif
@@ -1047,14 +1024,15 @@
 #include <cstring>
 #include <numeric>
 #include <type_traits>
 #include <new>
 #include <utility>
 #include <memory>
 #include <optional>
+#include <iterator>
 
 #ifndef SOAGEN_COLUMN_SPAN_TYPE
 	#if SOAGEN_CPP >= 20 && SOAGEN_HAS_INCLUDE(<span>)
 		#include <span>
 		#define SOAGEN_COLUMN_SPAN_TYPE std::span
 	#elif SOAGEN_HAS_INCLUDE(<muu/span.h>)
 		#include <muu/span.h>
@@ -1075,14 +1053,17 @@
 	#define SOAGEN_OPTIONAL_TYPE std::optional
 #endif
 
 SOAGEN_ENABLE_WARNINGS;
 
 SOAGEN_PUSH_WARNINGS;
 SOAGEN_DISABLE_SPAM_WARNINGS;
+#if SOAGEN_CLANG >= 16
+	#pragma clang diagnostic ignored "-Wunsafe-buffer-usage"
+#endif
 
 #if SOAGEN_MSVC_LIKE
 	#pragma push_macro("min")
 	#pragma push_macro("max")
 	#undef min
 	#undef max
 #endif
@@ -1095,25 +1076,14 @@
 		#pragma strict_gs_check(push, off)
 	#elif SOAGEN_GCC
 		#pragma GCC push_options
 		#pragma GCC optimize("O2")
 	#endif
 #endif
 
-#ifndef SOAGEN_LAUNDER
-	#if defined(__cpp_lib_launder) && __cpp_lib_launder >= 201606
-		#define SOAGEN_LAUNDER(...) std::launder(__VA_ARGS__)
-	#elif SOAGEN_CLANG >= 8 || SOAGEN_GCC >= 7 || SOAGEN_ICC >= 1910 || SOAGEN_MSVC >= 1914                            \
-		|| SOAGEN_HAS_BUILTIN(__builtin_launder)
-		#define SOAGEN_LAUNDER(...) __builtin_launder(__VA_ARGS__)
-	#else
-		#define SOAGEN_LAUNDER(...) __VA_ARGS__
-	#endif
-#endif
-
 #ifndef SOAGEN_MAKE_NAME
 	#define SOAGEN_MAKE_NAME(Name)                                                                                     \
                                                                                                                        \
 		struct name_constant_##Name                                                                                    \
 		{                                                                                                              \
 			static constexpr const char value[] = #Name;                                                               \
 		};                                                                                                             \
@@ -1202,28 +1172,40 @@
 
 	template <typename T>
 	inline constexpr bool is_unsigned = is_integer<T> && std::is_unsigned_v<T>;
 
 	template <typename T, typename... U>
 	inline constexpr bool any_same = (false || ... || std::is_same_v<T, U>);
 
+	template <auto Value, auto... Values>
+	inline constexpr bool any_same_value = ((Value == Values) || ...);
+
 	template <typename T>
 	inline constexpr bool is_soa = POXY_IMPLEMENTATION_DETAIL(false); // specialized in generated code
 
 	template <typename T>
 	inline constexpr bool is_soa<const T> = is_soa<T>;
 	template <typename T>
 	inline constexpr bool is_soa<volatile T> = is_soa<T>;
 	template <typename T>
 	inline constexpr bool is_soa<const volatile T> = is_soa<T>;
 
+	namespace detail
+	{
+		template <typename T>
+		using is_implicit_lifetime_type_ = std::disjunction<std::is_scalar<T>,
+															std::is_array<T>,
+															std::conjunction<std::is_aggregate<T>,
+																			 std::is_trivially_constructible<T>,
+																			 std::is_trivially_destructible<T>>>;
+	}
+
 	template <typename T>
 	inline constexpr bool is_implicit_lifetime_type =
-		std::is_scalar_v<T> || std::is_array_v<T>
-		|| (std::is_aggregate_v<T> && std::is_trivially_constructible_v<T> && std::is_trivially_destructible_v<T>);
+		POXY_IMPLEMENTATION_DETAIL(detail::is_implicit_lifetime_type_<T>::value);
 
 	template <auto Value>
 	using index_constant = std::integral_constant<size_t, static_cast<size_t>(Value)>;
 
 	template <typename T>
 	using forward_type = POXY_IMPLEMENTATION_DETAIL(
 		std::conditional_t<std::is_lvalue_reference_v<T>, T, std::add_rvalue_reference_t<T>>);
@@ -1254,159 +1236,175 @@
 		template <template <typename...> typename Trait, typename Enabler, typename... Args>
 		struct is_detected_impl : std::false_type
 		{};
 		template <template <typename...> typename Trait, typename... Args>
 		struct is_detected_impl<Trait, std::void_t<Trait<Args...>>, Args...> : std::true_type
 		{};
 		template <template <typename...> typename Trait, typename... Args>
-		inline constexpr auto is_detected_ = is_detected_impl<Trait, void, Args...>::value;
+		using is_detected_ = is_detected_impl<Trait, void, Args...>;
 	}
 
 	template <template <typename...> typename Trait, typename... Args>
-	inline constexpr auto is_detected = detail::is_detected_<Trait, Args...>;
+	inline constexpr auto is_detected = POXY_IMPLEMENTATION_DETAIL(detail::is_detected_<Trait, Args...>::value);
 
 	namespace detail
 	{
 		template <typename T>
-		using has_swap_member_ = decltype(std::declval<T&>().swap(std::declval<T&>()));
+		using has_swap_member_impl_ = decltype(std::declval<T&>().swap(std::declval<T&>()));
+		template <typename T>
+		using has_swap_member_ = is_detected_<has_swap_member_impl_, T>;
 
 		template <typename T, typename Arg>
-		using has_resize_member_ = decltype(std::declval<T&>().resize(std::declval<const Arg&>()));
+		using has_resize_member_impl_ = decltype(std::declval<T&>().resize(std::declval<const Arg&>()));
+		template <typename T, typename Arg = size_t>
+		using has_resize_member_ = is_detected_<has_resize_member_impl_, T, Arg>;
 
 		template <typename T, typename Arg>
-		using has_erase_member_ = decltype(std::declval<T&>().erase(std::declval<const Arg&>()));
+		using has_erase_member_impl_ = decltype(std::declval<T&>().erase(std::declval<const Arg&>()));
+		template <typename T, typename Arg = size_t>
+		using has_erase_member_ = is_detected_<has_erase_member_impl_, T, Arg>;
 
 		template <typename T, typename Arg>
-		using has_unordered_erase_member_ = decltype(std::declval<T&>().unordered_erase(std::declval<const Arg&>()));
+		using has_unordered_erase_member_impl_ =
+			decltype(std::declval<T&>().unordered_erase(std::declval<const Arg&>()));
+		template <typename T, typename Arg = size_t>
+		using has_unordered_erase_member_ = is_detected_<has_unordered_erase_member_impl_, T, Arg>;
 
 		template <typename T>
-		using has_data_member_ = decltype(std::declval<T&>().data());
+		using has_data_member_impl_ = decltype(std::declval<T&>().data());
+		template <typename T>
+		using has_data_member_ = is_detected_<has_data_member_impl_, T>;
 
 		template <typename T, typename U>
-		using is_equality_comparable_ = decltype(std::declval<const std::remove_reference_t<T>&>()
-												 == std::declval<const std::remove_reference_t<U>&>());
+		using is_equality_comparable_impl_ = decltype(std::declval<const std::remove_reference_t<T>&>()
+													  == std::declval<const std::remove_reference_t<U>&>());
+		template <typename T, typename U = T>
+		using is_equality_comparable_ = is_detected_<is_equality_comparable_impl_, T, U>;
 
 		template <typename T, typename U>
-		using is_less_than_comparable_ = decltype(std::declval<const std::remove_reference_t<T>&>()
-												  < std::declval<const std::remove_reference_t<U>&>());
+		using is_less_than_comparable_impl_ = decltype(std::declval<const std::remove_reference_t<T>&>()
+													   < std::declval<const std::remove_reference_t<U>&>());
+		template <typename T, typename U = T>
+		using is_less_than_comparable_ = is_detected_<is_less_than_comparable_impl_, T, U>;
 	}
 
-	template <typename T>
-	inline constexpr bool has_swap_member = is_detected<detail::has_swap_member_, T>;
+	template <typename... T>
+	inline constexpr bool has_swap_member =
+		POXY_IMPLEMENTATION_DETAIL(std::conjunction<detail::has_swap_member_<T>...>::value);
 
-	template <typename T, typename Arg = size_t>
-	inline constexpr bool has_resize_member = is_detected<detail::has_resize_member_, T, Arg>;
+	template <typename... T>
+	inline constexpr bool has_resize_member =
+		POXY_IMPLEMENTATION_DETAIL(std::conjunction<detail::has_resize_member_<T, size_t>...>::value);
 
-	template <typename T, typename Arg = size_t>
-	inline constexpr bool has_erase_member = is_detected<detail::has_erase_member_, T, Arg>;
+	template <typename... T>
+	inline constexpr bool has_erase_member =
+		POXY_IMPLEMENTATION_DETAIL(std::conjunction<detail::has_erase_member_<T, size_t>...>::value);
 
-	template <typename T, typename Arg = size_t>
-	inline constexpr bool has_unordered_erase_member = is_detected<detail::has_unordered_erase_member_, T, Arg>;
+	template <typename... T>
+	inline constexpr bool has_unordered_erase_member =
+		POXY_IMPLEMENTATION_DETAIL(std::conjunction<detail::has_unordered_erase_member_<T, size_t>...>::value);
 
-	template <typename T>
-	inline constexpr bool has_data_member = is_detected<detail::has_data_member_, T>;
+	template <typename... T>
+	inline constexpr bool has_data_member =
+		POXY_IMPLEMENTATION_DETAIL(std::conjunction<detail::has_data_member_<T>...>::value);
 
 	template <typename T, typename U = T>
-	inline constexpr bool is_equality_comparable = is_detected<detail::is_equality_comparable_, T, U>;
+	inline constexpr bool is_equality_comparable =
+		POXY_IMPLEMENTATION_DETAIL(detail::is_equality_comparable_<T, U>::value);
 
 	template <typename T, typename U = T>
-	inline constexpr bool is_less_than_comparable = is_detected<detail::is_less_than_comparable_, T, U>;
+	inline constexpr bool is_less_than_comparable =
+		POXY_IMPLEMENTATION_DETAIL(detail::is_less_than_comparable_<T, U>::value);
 
 	namespace detail
 	{
 		template <typename T, bool = has_swap_member<T>>
 		struct has_nothrow_swap_member_ : std::bool_constant<noexcept(std::declval<T&>().swap(std::declval<T&>()))>
 		{};
 		template <typename T>
 		struct has_nothrow_swap_member_<T, false> : std::false_type
 		{};
 
-		template <typename T, typename Arg, bool = has_resize_member<T, Arg>>
+		template <typename T, typename Arg = size_t, bool = has_resize_member<T, Arg>>
 		struct has_nothrow_resize_member_
 			: std::bool_constant<noexcept(std::declval<T&>().resize(std::declval<const Arg&>()))>
 		{};
 		template <typename T, typename Arg>
 		struct has_nothrow_resize_member_<T, Arg, false> : std::false_type
 		{};
 
-		template <typename T, typename Arg, bool = has_erase_member<T, Arg>>
+		template <typename T, typename Arg = size_t, bool = has_erase_member<T, Arg>>
 		struct has_nothrow_erase_member_
 			: std::bool_constant<noexcept(std::declval<T&>().erase(std::declval<const Arg&>()))>
 		{};
 		template <typename T, typename Arg>
 		struct has_nothrow_erase_member_<T, Arg, false> : std::false_type
 		{};
 
-		template <typename T, typename Arg, bool = has_unordered_erase_member<T, Arg>>
+		template <typename T, typename Arg = size_t, bool = has_unordered_erase_member<T, Arg>>
 		struct has_nothrow_unordered_erase_member_
 			: std::bool_constant<noexcept(std::declval<T&>().unordered_erase(std::declval<const Arg&>()))>
 		{};
 		template <typename T, typename Arg>
 		struct has_nothrow_unordered_erase_member_<T, Arg, false> : std::false_type
 		{};
 
 		template <typename T, bool = has_data_member<T>>
 		struct has_nothrow_data_member_ : std::bool_constant<noexcept(std::declval<T&>().data())>
 		{};
 		template <typename T>
 		struct has_nothrow_data_member_<T, false> : std::false_type
 		{};
 
-		template <typename T, typename U, bool = is_equality_comparable<T, U>>
+		template <typename T, typename U = T, bool = is_equality_comparable<T, U>>
 		struct is_nothrow_equality_comparable_
 			: std::bool_constant<noexcept(std::declval<const std::remove_reference_t<T>&>()
 										  == std::declval<const std::remove_reference_t<U>&>())>
 		{};
 		template <typename T, typename U>
 		struct is_nothrow_equality_comparable_<T, U, false> : std::false_type
 		{};
 
-		template <typename T, typename U, bool = is_less_than_comparable<T, U>>
+		template <typename T, typename U = T, bool = is_less_than_comparable<T, U>>
 		struct is_nothrow_less_than_comparable_
 			: std::bool_constant<noexcept(std::declval<const std::remove_reference_t<T>&>()
 										  < std::declval<const std::remove_reference_t<U>&>())>
 		{};
 		template <typename T, typename U>
 		struct is_nothrow_less_than_comparable_<T, U, false> : std::false_type
 		{};
 	}
 
-	template <typename T>
-	inline constexpr bool has_nothrow_swap_member = detail::has_nothrow_swap_member_<T>::value;
+	template <typename... T>
+	inline constexpr bool has_nothrow_swap_member =
+		POXY_IMPLEMENTATION_DETAIL(std::conjunction<detail::has_nothrow_swap_member_<T>...>::value);
 
-	template <typename T, typename Arg = size_t>
-	inline constexpr bool has_nothrow_resize_member = detail::has_nothrow_resize_member_<T, Arg>::value;
+	template <typename... T>
+	inline constexpr bool has_nothrow_resize_member =
+		POXY_IMPLEMENTATION_DETAIL(std::conjunction<detail::has_nothrow_resize_member_<T, size_t>...>::value);
 
-	template <typename T, typename Arg = size_t>
-	inline constexpr bool has_nothrow_erase_member = detail::has_nothrow_erase_member_<T, Arg>::value;
+	template <typename... T>
+	inline constexpr bool has_nothrow_erase_member =
+		POXY_IMPLEMENTATION_DETAIL(std::conjunction<detail::has_nothrow_erase_member_<T, size_t>...>::value);
 
-	template <typename T, typename Arg = size_t>
+	template <typename... T>
 	inline constexpr bool has_nothrow_unordered_erase_member =
-		detail::has_nothrow_unordered_erase_member_<T, Arg>::value;
+		POXY_IMPLEMENTATION_DETAIL(std::conjunction<detail::has_nothrow_unordered_erase_member_<T, size_t>...>::value);
 
-	template <typename T>
-	inline constexpr bool has_nothrow_data_member = detail::has_nothrow_data_member_<T>::value;
+	template <typename... T>
+	inline constexpr bool has_nothrow_data_member =
+		POXY_IMPLEMENTATION_DETAIL(std::conjunction<detail::has_nothrow_data_member_<T>...>::value);
 
 	template <typename T, typename U = T>
-	inline constexpr bool is_nothrow_equality_comparable = detail::is_nothrow_equality_comparable_<T, U>::value;
+	inline constexpr bool is_nothrow_equality_comparable =
+		POXY_IMPLEMENTATION_DETAIL(detail::is_nothrow_equality_comparable_<T, U>::value);
 
 	template <typename T, typename U = T>
-	inline constexpr bool is_nothrow_less_than_comparable = detail::is_nothrow_less_than_comparable_<T, U>::value;
-
-	namespace detail
-	{
-		template <typename T>
-		using has_tuple_size_ = decltype(std::tuple_size<remove_cvref<T>>::value);
-		template <typename T>
-		using has_tuple_element_ = decltype(std::declval<typename std::tuple_element<0, remove_cvref<T>>::type>());
-	}
-
-	template <typename T>
-	inline constexpr bool is_tuple_like =
-		is_detected<detail::has_tuple_size_, T> && is_detected<detail::has_tuple_element_, T>;
+	inline constexpr bool is_nothrow_less_than_comparable =
+		POXY_IMPLEMENTATION_DETAIL(detail::is_nothrow_less_than_comparable_<T, U>::value);
 
 #if !SOAGEN_DOXYGEN && SOAGEN_HAS_BUILTIN(__type_pack_element)
 
 	template <size_t I, typename... T>
 	using type_at_index = __type_pack_element<I, T...>;
 
 #else
@@ -1439,14 +1437,18 @@
 			using type = typename T::table_type;
 		};
 	}
 
 	template <typename T>
 	using table_type = POXY_IMPLEMENTATION_DETAIL(typename detail::table_type_<std::remove_cv_t<T>>::type);
 
+	template <typename A, typename B>
+	inline constexpr bool same_table_type =
+		POXY_IMPLEMENTATION_DETAIL(std::is_same_v<table_type<remove_cvref<A>>, table_type<remove_cvref<B>>>);
+
 	namespace detail
 	{
 		template <typename T>
 		struct table_traits_type_
 		{
 			using type = typename T::table_traits;
 		};
@@ -1576,194 +1578,129 @@
 					std::add_rvalue_reference_t<remove_cvref<T>>>>;
 		};
 	}
 
 	template <typename ParamType>
 	using rvalue_type = POXY_IMPLEMENTATION_DETAIL(typename detail::rvalue_type_<ParamType>::type);
 
-	template <typename... Args>
-	struct emplacer
-	{
-		static_assert(sizeof...(Args));
-		static_assert((std::is_reference_v<Args> && ...));
-
-		void* ptrs[sizeof...(Args)];
-
-		SOAGEN_DEFAULT_RULE_OF_FIVE(emplacer);
-
-		SOAGEN_NODISCARD_CTOR
-		constexpr emplacer(Args&&... args) noexcept //
-			: ptrs{ const_cast<void*>(static_cast<const volatile void*>(&args))... }
-		{}
-	};
-
-	template <>
-	struct emplacer<>
-	{};
-	template <typename... Args>
-	emplacer(Args&&...) -> emplacer<Args&&...>;
-
-	template <typename T>
-	inline constexpr bool is_emplacer = POXY_IMPLEMENTATION_DETAIL(false);
-
-	template <typename... T>
-	inline constexpr bool is_emplacer<emplacer<T...>> = true;
-	template <typename T>
-	inline constexpr bool is_emplacer<const T> = is_emplacer<T>;
-	template <typename T>
-	inline constexpr bool is_emplacer<volatile T> = is_emplacer<T>;
-	template <typename T>
-	inline constexpr bool is_emplacer<const volatile T> = is_emplacer<T>;
-
 	namespace detail
 	{
-		// note: this machinery is so that we only instantiate the is_nothrow version
-		// when the regular version is true
+		// machinery to only instantiate one or more secondary traits when the primary one is true
+		// e.g. for traits that come in pairs like is_invocable / is_nothrow_invocable
 
 		template <typename...>
-		struct is_nothrow_invocable_indirect_ : std::false_type
+		struct types_;
+
+		template <bool, template <typename...> typename, typename...>
+		struct nested_trait_indirect_ : std::false_type
 		{};
 
-		template <typename Func, typename... Args>
-		struct is_nothrow_invocable_indirect_<std::true_type, Func, Args...> : std::is_nothrow_invocable<Func, Args...>
+		template <template <typename...> typename Trait, typename... Args>
+		struct nested_trait_indirect_<true, Trait, Args...> : Trait<Args...>
 		{};
 
-		template <typename Func, typename... Args>
-		struct is_invocable_ : std::is_invocable<Func, Args...>
+		template <typename, template <typename...> typename, template <typename...> typename...>
+		struct nested_trait_;
+
+		template <template <typename...> typename Trait,
+				  template <typename...>
+				  typename... NestedTraits,
+				  typename... Args>
+		struct nested_trait_<types_<Args...>, Trait, NestedTraits...> : Trait<Args...>
 		{
-			using is_nothrow =
-				is_nothrow_invocable_indirect_<std::bool_constant<std::is_invocable<Func, Args...>::value>,
-											   Func,
-											   Args...>;
+			template <size_t Index>
+			using nested =
+				type_at_index<Index, nested_trait_indirect_<Trait<Args...>::value, NestedTraits, Args...>...>;
 		};
 	}
 
-	template <typename Func, typename... Args>
-	inline constexpr bool is_invocable = detail::is_invocable_<Func, Args...>::value;
-
-	template <typename Func, typename... Args>
-	inline constexpr bool is_nothrow_invocable = detail::is_invocable_<Func, Args...>::is_nothrow::value;
-
 	namespace detail
 	{
-		template <size_t I, typename Func, typename Arg>
-		struct is_invocable_with_optional_index_							//
-			: std::disjunction<is_invocable_<Func, Arg, index_constant<I>>, //
-							   is_invocable_<Func, Arg, size_t>,			//
-							   is_invocable_<Func, index_constant<I>, Arg>, //
-							   is_invocable_<Func, size_t, Arg>,			//
-							   is_invocable_<Func, Arg>>
-		{};
+		template <typename Table, size_t ColumnIndex>
+		struct column_name;
+		template <typename Table, size_t ColumnIndex>
+		struct column_ref;
 	}
+}
 
-	template <size_t I, typename Func, typename Arg>
-	inline constexpr bool is_invocable_with_optional_index =
-		detail::is_invocable_with_optional_index_<I, Func, Arg>::value;
+//********  row.hpp  ***************************************************************************************************
 
-	template <size_t I, typename Func, typename Arg>
-	inline constexpr bool is_nothrow_invocable_with_optional_index =
-		detail::is_invocable_with_optional_index_<I, Func, Arg>::is_nothrow::value;
+namespace soagen
+{
+	template <typename, size_t...>
+	struct row;
 
-	template <size_t I, typename Func, typename Arg>
-	SOAGEN_ALWAYS_INLINE
-	constexpr decltype(auto) invoke_with_optional_index(Func&& func,
-														Arg&& arg) //
-		noexcept(is_nothrow_invocable_with_optional_index<I, Func&&, Arg&&>)
+	namespace detail
 	{
-		static_assert(is_invocable_with_optional_index<I, Func&&, Arg&&>);
+		// general rules for allowing implicit conversions:
+		// - losing rvalue (T&& -> T&), (const T&& -> const T&)
+		// - gaining const (T& -> const T&, T&& -> const T&&)
+		// - both
 
-		if constexpr (is_invocable<Func&&, Arg&&, index_constant<I>>)
-		{
-			return static_cast<Func&&>(func)(static_cast<Arg&&>(arg), index_constant<I>{});
-		}
-		else if constexpr (is_invocable<Func&&, Arg&&, size_t>)
-		{
-			return static_cast<Func&&>(func)(static_cast<Arg&&>(arg), I);
-		}
-		else if constexpr (is_invocable<Func&&, index_constant<I>, Arg&&>)
-		{
-			return static_cast<Func&&>(func)(index_constant<I>{}, static_cast<Arg&&>(arg));
-		}
-		else if constexpr (is_invocable<Func&&, size_t, Arg&&>)
-		{
-			return static_cast<Func&&>(func)(I, static_cast<Arg&&>(arg));
-		}
-		else
-		{
-			static_assert(is_invocable<Func&&, Arg&&>);
+		template <typename From, typename To>
+		inline constexpr bool implicit_conversion_ok = false;
 
-			return static_cast<Func&&>(func)(static_cast<Arg&&>(arg));
-		}
-	}
+		template <typename T>
+		inline constexpr bool implicit_conversion_ok<T, T> = true;
 
-	namespace detail
-	{
-		template <typename Table, size_t ColumnIndex>
-		struct column_name;
-		template <typename Table, size_t ColumnIndex>
-		struct column_ref;
+		template <typename T>
+		inline constexpr bool implicit_conversion_ok<T&, const T&> = true;
 
-		template <typename A, typename B>
-		inline constexpr bool same_table_type =
-			std::is_same_v<table_type<remove_cvref<A>>, table_type<remove_cvref<B>>>;
-	}
-}
+		template <typename T>
+		inline constexpr bool implicit_conversion_ok<T&&, T&> = true;
 
-namespace std
-{
-	template <typename... Args>
-	struct tuple_size<soagen::emplacer<Args...>> //
-		: std::integral_constant<size_t, sizeof...(Args)>
-	{};
-}
+		template <typename T>
+		inline constexpr bool implicit_conversion_ok<T&&, const T&> = true;
 
-#if SOAGEN_ALWAYS_OPTIMIZE
-	#if SOAGEN_MSVC
-		#pragma strict_gs_check(pop)
-		#pragma runtime_checks("", restore)
-		#pragma optimize("", on)
-		#pragma inline_recursion(off)
-	#elif SOAGEN_GCC
-		#pragma GCC pop_options
-	#endif
-#endif
+		template <typename T>
+		inline constexpr bool implicit_conversion_ok<T&&, const T&&> = true;
 
-#if SOAGEN_MSVC_LIKE
-	#pragma pop_macro("min")
-	#pragma pop_macro("max")
-#endif
+		// general rules for allowing explicit conversions:
+		template <typename From, typename To>
+		inline constexpr bool explicit_conversion_ok = false;
 
-SOAGEN_POP_WARNINGS;
+		template <typename T>
+		inline constexpr bool explicit_conversion_ok<T&, T&&> = true;
 
-//********  row.hpp  ***************************************************************************************************
+		template <typename T>
+		inline constexpr bool explicit_conversion_ok<T&, const T&&> = true;
 
-SOAGEN_PUSH_WARNINGS;
-SOAGEN_DISABLE_SPAM_WARNINGS;
+		// tests for compatible column permutations:
+		template <typename From, typename To>
+		inline constexpr bool column_conversion_ok = false;
 
-#if SOAGEN_MSVC_LIKE
-	#pragma push_macro("min")
-	#pragma push_macro("max")
-	#undef min
-	#undef max
-#endif
+		template <size_t... Columns>
+		inline constexpr bool column_conversion_ok<std::index_sequence<Columns...>, std::index_sequence<Columns...>> =
+			true;
 
-#if SOAGEN_ALWAYS_OPTIMIZE
-	#if SOAGEN_MSVC
-		#pragma inline_recursion(on)
-		#pragma optimize("gt", on)
-		#pragma runtime_checks("", off)
-		#pragma strict_gs_check(push, off)
-	#elif SOAGEN_GCC
-		#pragma GCC push_options
-		#pragma GCC optimize("O2")
-	#endif
-#endif
+		template <size_t... ColumnsA, size_t... ColumnsB>
+		inline constexpr bool column_conversion_ok<std::index_sequence<ColumnsA...>, std::index_sequence<ColumnsB...>> =
+			(any_same_value<ColumnsB, ColumnsA...> && ...);
+
+		// row implicit conversions:
+		template <typename From, typename To>
+		inline constexpr bool row_implicit_conversion_ok = false;
+
+		template <typename TableA, size_t... ColumnsA, typename TableB, size_t... ColumnsB>
+		inline constexpr bool row_implicit_conversion_ok<row<TableA, ColumnsA...>, //
+														 row<TableB, ColumnsB...>> =
+			implicit_conversion_ok<TableA, TableB>
+			&& column_conversion_ok<std::index_sequence<ColumnsA...>, std::index_sequence<ColumnsB...>>;
+
+		// row explicit conversions:
+		template <typename From, typename To>
+		inline constexpr bool row_explicit_conversion_ok = false;
+
+		template <typename TableA, size_t... ColumnsA, typename TableB, size_t... ColumnsB>
+		inline constexpr bool row_explicit_conversion_ok<row<TableA, ColumnsA...>, //
+														 row<TableB, ColumnsB...>> =
+			explicit_conversion_ok<TableA, TableB>
+			&& column_conversion_ok<std::index_sequence<ColumnsA...>, std::index_sequence<ColumnsB...>>;
+	}
 
-namespace soagen
-{
 	template <typename Derived>
 	struct SOAGEN_EMPTY_BASES row_base
 	{};
 
 	template <typename Table, size_t... Columns>
 	struct SOAGEN_EMPTY_BASES row //
 	SOAGEN_HIDDEN_BASE(public detail::column_ref<Table, Columns>..., public row_base<row<Table, Columns...>>)
@@ -1791,25 +1728,25 @@
 		constexpr decltype(auto) get() const noexcept
 		{
 			static_assert(Member < sizeof...(Columns), "member index out of range");
 
 			return type_at_index<Member, detail::column_ref<Table, Columns>...>::get_named_member();
 		}
 
-		SOAGEN_CONSTRAINED_TEMPLATE((detail::same_table_type<Table, T>
+		SOAGEN_CONSTRAINED_TEMPLATE((same_table_type<Table, T>
 									 && table_traits_type<remove_cvref<Table>>::all_equality_comparable),
 									typename T)
 		SOAGEN_NODISCARD
 		friend constexpr bool operator==(const row& lhs, const row<T, Columns...>& rhs) //
 			noexcept(table_traits_type<remove_cvref<Table>>::all_nothrow_equality_comparable)
 		{
 			return ((lhs.template column<Columns>() == rhs.template column<Columns>()) && ...);
 		}
 
-		SOAGEN_CONSTRAINED_TEMPLATE((detail::same_table_type<Table, T>
+		SOAGEN_CONSTRAINED_TEMPLATE((same_table_type<Table, T>
 									 && table_traits_type<remove_cvref<Table>>::all_equality_comparable),
 									typename T)
 		SOAGEN_NODISCARD
 		SOAGEN_ALWAYS_INLINE
 		friend constexpr bool operator!=(const row& lhs, const row<T, Columns...>& rhs) //
 			noexcept(table_traits_type<remove_cvref<Table>>::all_nothrow_equality_comparable)
 		{
@@ -1831,53 +1768,75 @@
 			if constexpr (Member + 1u == sizeof...(Columns))
 				return 0;
 			else
 				return row_compare_impl<Member + 1u>(lhs, rhs);
 		}
 
 	  public:
-		SOAGEN_CONSTRAINED_TEMPLATE((detail::same_table_type<Table, T>
+		SOAGEN_CONSTRAINED_TEMPLATE((same_table_type<Table, T>
 									 && table_traits_type<remove_cvref<Table>>::all_less_than_comparable),
 									typename T)
 		SOAGEN_NODISCARD
 		friend constexpr bool operator<(const row& lhs, const row<T, Columns...>& rhs) //
 			noexcept(table_traits_type<remove_cvref<Table>>::all_nothrow_less_than_comparable)
 		{
 			return row_compare_impl<0>(lhs, rhs) < 0;
 		}
 
-		SOAGEN_CONSTRAINED_TEMPLATE((detail::same_table_type<Table, T>
+		SOAGEN_CONSTRAINED_TEMPLATE((same_table_type<Table, T>
 									 && table_traits_type<remove_cvref<Table>>::all_less_than_comparable),
 									typename T)
 		SOAGEN_NODISCARD
 		friend constexpr bool operator<=(const row& lhs, const row<T, Columns...>& rhs) //
 			noexcept(table_traits_type<remove_cvref<Table>>::all_nothrow_less_than_comparable)
 		{
 			return row_compare_impl<0>(lhs, rhs) <= 0;
 		}
 
-		SOAGEN_CONSTRAINED_TEMPLATE((detail::same_table_type<Table, T>
+		SOAGEN_CONSTRAINED_TEMPLATE((same_table_type<Table, T>
 									 && table_traits_type<remove_cvref<Table>>::all_less_than_comparable),
 									typename T)
 		SOAGEN_NODISCARD
 		friend constexpr bool operator>(const row& lhs, const row<T, Columns...>& rhs) //
 			noexcept(table_traits_type<remove_cvref<Table>>::all_nothrow_less_than_comparable)
 		{
 			return row_compare_impl<0>(lhs, rhs) > 0;
 		}
 
-		SOAGEN_CONSTRAINED_TEMPLATE((detail::same_table_type<Table, T>
+		SOAGEN_CONSTRAINED_TEMPLATE((same_table_type<Table, T>
 									 && table_traits_type<remove_cvref<Table>>::all_less_than_comparable),
 									typename T)
 		SOAGEN_NODISCARD
 		friend constexpr bool operator>=(const row& lhs, const row<T, Columns...>& rhs) //
 			noexcept(table_traits_type<remove_cvref<Table>>::all_nothrow_less_than_comparable)
 		{
 			return row_compare_impl<0>(lhs, rhs) >= 0;
 		}
+
+		SOAGEN_CONSTRAINED_TEMPLATE((detail::row_implicit_conversion_ok<row, row<T, Cols...>>
+									 && !detail::row_explicit_conversion_ok<row, row<T, Cols...>>),
+									typename T,
+									size_t... Cols)
+		SOAGEN_PURE_INLINE_GETTER
+		constexpr operator row<T, Cols...>() const noexcept
+		{
+			return row<T, Cols...>{ { static_cast<decltype(std::declval<row<T, Cols...>>().template column<Cols>())>(
+				this->template column<Cols>()) }... };
+		}
+
+		SOAGEN_CONSTRAINED_TEMPLATE((!detail::row_implicit_conversion_ok<row, row<T, Cols...>>
+									 && detail::row_explicit_conversion_ok<row, row<T, Cols...>>),
+									typename T,
+									size_t... Cols)
+		SOAGEN_PURE_INLINE_GETTER
+		explicit constexpr operator row<T, Cols...>() const noexcept
+		{
+			return row<T, Cols...>{ { static_cast<decltype(std::declval<row<T, Cols...>>().template column<Cols>())>(
+				this->template column<Cols>()) }... };
+		}
 	};
 
 	template <typename T>
 	inline constexpr bool is_row = POXY_IMPLEMENTATION_DETAIL(false);
 
 	template <typename Table, size_t... Columns>
 	inline constexpr bool is_row<row<Table, Columns...>> = true;
@@ -1929,56 +1888,16 @@
 	template <size_t Member, typename Table, size_t... Columns>
 	struct tuple_element<Member, soagen::row<Table, Columns...>>
 	{
 		using type = decltype(std::declval<soagen::row<Table, Columns...>>().template get<Member>());
 	};
 }
 
-#if SOAGEN_ALWAYS_OPTIMIZE
-	#if SOAGEN_MSVC
-		#pragma strict_gs_check(pop)
-		#pragma runtime_checks("", restore)
-		#pragma optimize("", on)
-		#pragma inline_recursion(off)
-	#elif SOAGEN_GCC
-		#pragma GCC pop_options
-	#endif
-#endif
-
-#if SOAGEN_MSVC_LIKE
-	#pragma pop_macro("min")
-	#pragma pop_macro("max")
-#endif
-
-SOAGEN_POP_WARNINGS;
-
 //********  generated/compressed_pair.hpp  *****************************************************************************
 
-SOAGEN_PUSH_WARNINGS;
-SOAGEN_DISABLE_SPAM_WARNINGS;
-
-#if SOAGEN_MSVC_LIKE
-	#pragma push_macro("min")
-	#pragma push_macro("max")
-	#undef min
-	#undef max
-#endif
-
-#if SOAGEN_ALWAYS_OPTIMIZE
-	#if SOAGEN_MSVC
-		#pragma inline_recursion(on)
-		#pragma optimize("gt", on)
-		#pragma runtime_checks("", off)
-		#pragma strict_gs_check(push, off)
-	#elif SOAGEN_GCC
-		#pragma GCC push_options
-		#pragma GCC optimize("O2")
-	#endif
-#endif
-
 namespace soagen
 {
 	namespace detail
 	{
 #define SOAGEN_COMPRESSED_PAIR_BASE_GETTERS(T, name, expression)                                                       \
 	SOAGEN_PURE_INLINE_GETTER                                                                                          \
 	constexpr T& name()& noexcept                                                                                      \
@@ -2216,60 +2135,16 @@
 	struct tuple_element<I, soagen::compressed_pair<First, Second>>
 	{
 		static_assert(I < 2);
 		using type = std::conditional_t<I == 1, Second, First>;
 	};
 }
 
-#if SOAGEN_ALWAYS_OPTIMIZE
-	#if SOAGEN_MSVC
-		#pragma strict_gs_check(pop)
-		#pragma runtime_checks("", restore)
-		#pragma optimize("", on)
-		#pragma inline_recursion(off)
-	#elif SOAGEN_GCC
-		#pragma GCC pop_options
-	#endif
-#endif
-
-#if SOAGEN_MSVC_LIKE
-	#pragma pop_macro("min")
-	#pragma pop_macro("max")
-#endif
-
-SOAGEN_POP_WARNINGS;
-
 //********  generated/functions.hpp  ***********************************************************************************
 
-#if SOAGEN_CPP >= 20 && defined(__cpp_lib_bit_cast) && __cpp_lib_bit_cast >= 201806
-	#include <bit>
-#endif
-
-SOAGEN_PUSH_WARNINGS;
-SOAGEN_DISABLE_SPAM_WARNINGS;
-
-#if SOAGEN_MSVC_LIKE
-	#pragma push_macro("min")
-	#pragma push_macro("max")
-	#undef min
-	#undef max
-#endif
-
-#if SOAGEN_ALWAYS_OPTIMIZE
-	#if SOAGEN_MSVC
-		#pragma inline_recursion(on)
-		#pragma optimize("gt", on)
-		#pragma runtime_checks("", off)
-		#pragma strict_gs_check(push, off)
-	#elif SOAGEN_GCC
-		#pragma GCC push_options
-		#pragma GCC optimize("O2")
-	#endif
-#endif
-
 namespace soagen
 {
 	SOAGEN_CONST_INLINE_GETTER
 	constexpr bool is_constant_evaluated() noexcept
 	{
 #if SOAGEN_HAS_IF_CONSTEVAL
 
@@ -2416,145 +2291,18 @@
 
 				return ptr;
 
 #endif
 			}
 		}
 	}
-
-	namespace detail
-	{
-		template <typename T>
-		using has_tuple_get_member_ = decltype(std::declval<T>().template get<0>());
-	}
-
-	template <size_t I, typename T>
-	SOAGEN_NODISCARD
-	SOAGEN_ALWAYS_INLINE
-	constexpr decltype(auto) get_from_tuple_like(T&& tuple_like) noexcept
-	{
-		if constexpr (is_detected<detail::has_tuple_get_member_, T&&>)
-		{
-			return static_cast<T&&>(tuple_like).template get<I>();
-		}
-		else // adl
-		{
-			using std::get;
-			return get<I>(static_cast<T&&>(tuple_like));
-		}
-	}
-
-#if SOAGEN_CPP >= 20 && defined(__cpp_lib_bit_cast) && __cpp_lib_bit_cast >= 201806
-
-	#define SOAGEN_HAS_INTRINSIC_BIT_CAST 1
-
-	using std::bit_cast;
-
-#else
-
-	SOAGEN_CONSTRAINED_TEMPLATE((std::is_trivially_copyable_v<From>	 //
-								 && std::is_trivially_copyable_v<To> //
-								 && sizeof(From) == sizeof(To)),
-								typename To,
-								typename From)
-	SOAGEN_PURE_INLINE_GETTER
-	constexpr To bit_cast(const From& from) noexcept
-	{
-		static_assert(!std::is_reference_v<To> && !std::is_reference_v<From>);
-
-	#if SOAGEN_CLANG >= 11 || SOAGEN_GCC >= 11 || SOAGEN_MSVC >= 1926                                                  \
-		|| (!SOAGEN_CLANG && !SOAGEN_GCC && SOAGEN_HAS_BUILTIN(__builtin_bit_cast))
-
-		#define SOAGEN_HAS_INTRINSIC_BIT_CAST 1
-		return __builtin_bit_cast(To, from);
-
-	#else
-
-		#define SOAGEN_HAS_INTRINSIC_BIT_CAST 0
-
-		if constexpr (std::is_same_v<std::remove_cv_t<From>, std::remove_cv_t<To>>)
-		{
-			return from;
-		}
-		else if constexpr (!std::is_nothrow_default_constructible_v<std::remove_cv_t<To>>)
-		{
-			union proxy_t
-			{
-				alignas(To) unsigned char dummy[sizeof(To)];
-				std::remove_cv_t<To> to;
-
-				proxy_t() noexcept
-				{}
-			};
-
-			proxy_t proxy;
-			std::memcpy(&proxy.to, &from, sizeof(To));
-			return proxy.to;
-		}
-		else
-		{
-			static_assert(std::is_nothrow_default_constructible_v<std::remove_cv_t<To>>,
-						  "Bit-cast fallback requires the To type be nothrow default-constructible");
-
-			std::remove_cv_t<To> to;
-			std::memcpy(&to, &from, sizeof(To));
-			return to;
-		}
-	#endif
-	}
-
-#endif
 }
 
-#if SOAGEN_ALWAYS_OPTIMIZE
-	#if SOAGEN_MSVC
-		#pragma strict_gs_check(pop)
-		#pragma runtime_checks("", restore)
-		#pragma optimize("", on)
-		#pragma inline_recursion(off)
-	#elif SOAGEN_GCC
-		#pragma GCC pop_options
-	#endif
-#endif
-
-#if SOAGEN_MSVC_LIKE
-	#pragma pop_macro("min")
-	#pragma pop_macro("max")
-#endif
-
-SOAGEN_POP_WARNINGS;
-
 //********  allocator.hpp  *********************************************************************************************
 
-SOAGEN_PUSH_WARNINGS;
-SOAGEN_DISABLE_SPAM_WARNINGS;
-
-#if SOAGEN_MSVC_LIKE
-	#pragma push_macro("min")
-	#pragma push_macro("max")
-	#undef min
-	#undef max
-#endif
-
-#if SOAGEN_ALWAYS_OPTIMIZE
-	#if SOAGEN_MSVC
-		#pragma inline_recursion(on)
-		#pragma optimize("gt", on)
-		#pragma runtime_checks("", off)
-		#pragma strict_gs_check(push, off)
-	#elif SOAGEN_GCC
-		#pragma GCC push_options
-		#pragma GCC optimize("O2")
-	#endif
-#endif
-
-#if SOAGEN_CLANG >= 16
-	#pragma clang diagnostic ignored "-Wunsafe-buffer-usage"
-#endif
-
 namespace soagen
 {
 	struct allocator
 	{
 		using value_type		 = std::byte;
 		using pointer			 = value_type*;
 		using const_pointer		 = const value_type*;
@@ -2773,112 +2521,259 @@
 			SOAGEN_ASSERT(n == info.requested_size);
 
 			alloc.deallocate(info.ptr, info.actual_size);
 		}
 	};
 }
 
-#if SOAGEN_ALWAYS_OPTIMIZE
-	#if SOAGEN_MSVC
-		#pragma strict_gs_check(pop)
-		#pragma runtime_checks("", restore)
-		#pragma optimize("", on)
-		#pragma inline_recursion(off)
-	#elif SOAGEN_GCC
-		#pragma GCC pop_options
-	#endif
-#endif
+//********  emplacer.hpp  **********************************************************************************************
 
-#if SOAGEN_MSVC_LIKE
-	#pragma pop_macro("min")
-	#pragma pop_macro("max")
-#endif
+namespace soagen
+{
+	template <typename... Args>
+	struct emplacer
+	{
+		static_assert(sizeof...(Args));
+		static_assert((std::is_reference_v<Args> && ...));
 
-SOAGEN_POP_WARNINGS;
+		void* ptrs[sizeof...(Args)];
 
-//********  column_traits.hpp  *****************************************************************************************
+		SOAGEN_DEFAULT_RULE_OF_FIVE(emplacer);
 
-SOAGEN_PUSH_WARNINGS;
-SOAGEN_DISABLE_SPAM_WARNINGS;
+		SOAGEN_NODISCARD_CTOR
+		constexpr emplacer(Args&&... args) noexcept //
+			: ptrs{ const_cast<void*>(static_cast<const volatile void*>(&args))... }
+		{}
+	};
 
-#if SOAGEN_MSVC_LIKE
-	#pragma push_macro("min")
-	#pragma push_macro("max")
-	#undef min
-	#undef max
-#endif
+	template <>
+	struct emplacer<>
+	{};
 
-#if SOAGEN_ALWAYS_OPTIMIZE
-	#if SOAGEN_MSVC
-		#pragma inline_recursion(on)
-		#pragma optimize("gt", on)
-		#pragma runtime_checks("", off)
-		#pragma strict_gs_check(push, off)
-	#elif SOAGEN_GCC
-		#pragma GCC push_options
-		#pragma GCC optimize("O2")
+	template <typename... Args>
+	emplacer(Args&&...) -> emplacer<Args&&...>;
+
+	template <typename T>
+	inline constexpr bool is_emplacer = POXY_IMPLEMENTATION_DETAIL(false);
+
+	template <typename... T>
+	inline constexpr bool is_emplacer<emplacer<T...>> = true;
+	template <typename T>
+	inline constexpr bool is_emplacer<const T> = is_emplacer<T>;
+	template <typename T>
+	inline constexpr bool is_emplacer<volatile T> = is_emplacer<T>;
+	template <typename T>
+	inline constexpr bool is_emplacer<const volatile T> = is_emplacer<T>;
+}
+
+namespace std
+{
+	template <typename... Args>
+	struct tuple_size<soagen::emplacer<Args...>> //
+		: std::integral_constant<size_t, sizeof...(Args)>
+	{};
+}
+
+//********  tuples.hpp  ************************************************************************************************
+
+namespace soagen
+{
+	namespace detail
+	{
+		template <typename T>
+		using has_tuple_size_impl_ = decltype(std::tuple_size<remove_cvref<T>>::value);
+		template <typename T>
+		using has_tuple_element_impl_ = decltype(std::declval<typename std::tuple_element<0, remove_cvref<T>>::type>());
+		template <typename T>
+		using has_tuple_get_member_impl_ = decltype(std::declval<T>().template get<0>());
+		namespace adl_dummy
+		{
+			template <size_t>
+			auto get();
+			template <typename T>
+			using has_tuple_get_adl_impl_ = decltype(get<0>(std::declval<T>()));
+		}
+
+		template <typename T>
+		using has_tuple_size_ = is_detected_<has_tuple_size_impl_, remove_cvref<T>>;
+		template <typename T>
+		using has_tuple_element_ = is_detected_<has_tuple_element_impl_, remove_cvref<T>>;
+		template <typename T>
+		using has_tuple_get_member_ = is_detected_<has_tuple_get_member_impl_, T>;
+		template <typename T>
+		using has_tuple_get_adl_ = is_detected_<adl_dummy::has_tuple_get_adl_impl_, T>;
+	}
+
+	template <typename T>
+	inline constexpr bool is_tuple = POXY_IMPLEMENTATION_DETAIL(
+		std::conjunction_v<detail::has_tuple_size_<T>,
+						   detail::has_tuple_element_<T>,
+						   std::disjunction<detail::has_tuple_get_member_<T>, detail::has_tuple_get_adl_<T>>>);
+
+	template <size_t I, typename T>
+	SOAGEN_NODISCARD
+	SOAGEN_ALWAYS_INLINE
+	constexpr decltype(auto) get_from_tuple(T&& tuple) noexcept
+	{
+		if constexpr (detail::has_tuple_get_member_<T&&>::value)
+		{
+			return static_cast<T&&>(tuple).template get<I>();
+		}
+		else if constexpr (detail::has_tuple_get_adl_<T&&>::value)
+		{
+			using std::get;
+			return get<I>(static_cast<T&&>(tuple));
+		}
+	}
+
+	namespace detail
+	{
+		template <typename...>
+		struct is_constructible_by_unpacking_tuple_impl_ : std::false_type
+		{};
+
+		template <typename T, typename Tuple, size_t... Members>
+		struct is_constructible_by_unpacking_tuple_impl_<T, Tuple, std::index_sequence<Members...>>
+			: nested_trait_<types_<T, decltype(get_from_tuple<Members>(std::declval<Tuple>()))...>,
+							std::is_constructible,
+							std::is_nothrow_constructible,
+							std::is_trivially_constructible>
+		{};
+
+		template <typename T, typename Tuple, bool = is_tuple<Tuple>>
+		struct is_constructible_by_unpacking_tuple_ : std::false_type
+		{
+			using is_nothrow = std::false_type;
+			using is_trivial = std::false_type;
+		};
+
+		template <typename T, typename Tuple>
+		struct is_constructible_by_unpacking_tuple_<T, Tuple, true>
+			: is_constructible_by_unpacking_tuple_impl_<
+				  T,
+				  Tuple,
+				  std::make_index_sequence<std::tuple_size_v<remove_cvref<Tuple>>>>
+		{
+			using base = is_constructible_by_unpacking_tuple_impl_<
+				T,
+				Tuple,
+				std::make_index_sequence<std::tuple_size_v<remove_cvref<Tuple>>>>;
+
+			using is_nothrow = typename base::template nested<0>;
+			using is_trivial = typename base::template nested<1>;
+		};
+	}
+
+	template <typename T, typename Tuple>
+	inline constexpr bool is_constructible_by_unpacking_tuple =
+		POXY_IMPLEMENTATION_DETAIL(detail::is_constructible_by_unpacking_tuple_<T, Tuple>::value);
+}
+
+//********  column_traits.hpp  *****************************************************************************************
+
+#ifndef SOAGEN_LAUNDER
+	#if defined(__cpp_lib_launder) && __cpp_lib_launder >= 201606
+		#define SOAGEN_LAUNDER(...) std::launder(__VA_ARGS__)
+	#elif SOAGEN_CLANG >= 8 || SOAGEN_GCC >= 7 || SOAGEN_ICC >= 1910 || SOAGEN_MSVC >= 1914                            \
+		|| SOAGEN_HAS_BUILTIN(__builtin_launder)
+		#define SOAGEN_LAUNDER(...) __builtin_launder(__VA_ARGS__)
+	#else
+		#define SOAGEN_LAUNDER(...) __VA_ARGS__
 	#endif
 #endif
 
-#if SOAGEN_CLANG >= 16
-	#pragma clang diagnostic ignored "-Wunsafe-buffer-usage"
+#ifndef SOAGEN_COLUMN
+	#define SOAGEN_COLUMN(I)                                                                                           \
+		SOAGEN_PURE_INLINE_GETTER                                                                                      \
+		SOAGEN_ATTR(returns_nonnull)
 #endif
 
-#define soagen_storage_ptr(...) soagen::assume_aligned<alignof(storage_type)>(__VA_ARGS__)
+#ifndef SOAGEN_ALIGNED_COLUMN
+	#define SOAGEN_ALIGNED_COLUMN(I)                                                                                   \
+		SOAGEN_COLUMN(I)                                                                                               \
+		SOAGEN_ATTR(assume_aligned(                                                                                    \
+			soagen::detail::actual_column_alignment<table_traits, allocator_type, static_cast<std::size_t>(I)>))
+#endif
+
+#define soagen_aligned_storage(...) soagen::assume_aligned<alignof(storage_type)>(__VA_ARGS__)
 
 namespace soagen::detail
 {
 	// a base class for the column traits that handles all the non-alignment-dependent stuff
 	// (to minimize template instantiation explosion)
 	template <typename StorageType>
 	struct column_traits_base
 	{
 		using storage_type = StorageType;
 		static_assert(!is_cvref<storage_type>, "column storage_type may not be cvref-qualified");
 		static_assert(!std::is_void_v<storage_type>, "column storage_type may not be void");
 		static_assert(std::is_destructible_v<storage_type>, "column storage_type must be destructible");
 
-		//--- dereferencing --------------------------------------------------------------------------------------------
+		//--- pointers -------------------------------------------------------------------------------------------------
 
 		SOAGEN_PURE_GETTER
 		SOAGEN_ATTR(nonnull)
-		static constexpr storage_type& get(std::byte* ptr) noexcept
+		static constexpr storage_type* ptr(std::byte* p) noexcept
 		{
-			SOAGEN_ASSUME(ptr != nullptr);
+			SOAGEN_ASSUME(p != nullptr);
 
-			return *SOAGEN_LAUNDER(reinterpret_cast<storage_type*>(soagen_storage_ptr(ptr)));
+			if constexpr (std::is_same_v<storage_type, std::byte>)
+				return p;
+			else
+				return SOAGEN_LAUNDER(reinterpret_cast<storage_type*>(p));
 		}
 
 		SOAGEN_PURE_GETTER
 		SOAGEN_ATTR(nonnull)
-		static constexpr const storage_type& get(const std::byte* ptr) noexcept
+		static constexpr const storage_type* ptr(const std::byte* p) noexcept
 		{
-			SOAGEN_ASSUME(ptr != nullptr);
+			SOAGEN_ASSUME(p != nullptr);
+
+			if constexpr (std::is_same_v<storage_type, std::byte>)
+				return p;
+			else
+				return SOAGEN_LAUNDER(reinterpret_cast<const storage_type*>(p));
+		}
 
-			return *SOAGEN_LAUNDER(reinterpret_cast<const storage_type*>(soagen_storage_ptr(ptr)));
+		//--- dereferencing --------------------------------------------------------------------------------------------
+
+		SOAGEN_PURE_INLINE_GETTER
+		SOAGEN_ATTR(nonnull)
+		static constexpr storage_type& get(std::byte* p) noexcept
+		{
+			return *ptr(p);
+		}
+
+		SOAGEN_PURE_INLINE_GETTER
+		SOAGEN_ATTR(nonnull)
+		static constexpr const storage_type& get(const std::byte* p) noexcept
+		{
+			SOAGEN_ASSUME(p != nullptr);
+
+			return *ptr(p);
 		}
 
 		//--- default construction -------------------------------------------------------------------------------------
 
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = std::is_default_constructible_v<storage_type>)
 		SOAGEN_ATTR(nonnull)
 		static constexpr storage_type& default_construct(std::byte* destination) //
 			noexcept(std::is_nothrow_default_constructible_v<storage_type>)
 		{
 			SOAGEN_ASSUME(destination != nullptr);
 
 #if defined(__cpp_lib_start_lifetime_as) && __cpp_lib_start_lifetime_as >= 202207
 			if constexpr (is_implicit_lifetime_type<storage_type>)
 			{
-				return *(std::start_lifetime_as<storage_type>(soagen_storage_ptr(destination)));
+				return *(std::start_lifetime_as<storage_type>(destination));
 			}
 			else
 			{
 #endif
-				return *(::new (static_cast<void*>(soagen_storage_ptr(destination))) storage_type);
+				return *(::new (static_cast<void*>(destination)) storage_type);
 
 #if defined(__cpp_lib_start_lifetime_as) && __cpp_lib_start_lifetime_as >= 202207
 			}
 #endif
 		}
 
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = std::is_default_constructible_v<storage_type>)
@@ -2899,15 +2794,15 @@
 		{
 			SOAGEN_ASSUME(buffer != nullptr);
 			SOAGEN_ASSUME(count);
 
 #if defined(__cpp_lib_start_lifetime_as) && __cpp_lib_start_lifetime_as >= 2022071
 			if constexpr (is_implicit_lifetime_type<storage_type>)
 			{
-				std::start_lifetime_as_array<storage_type>(soagen_storage_ptr(destination), count);
+				std::start_lifetime_as_array<storage_type>(destination, count);
 			}
 			else
 #endif
 				if constexpr (std::is_nothrow_default_constructible_v<storage_type>
 							  || std::is_trivially_destructible_v<storage_type>)
 			{
 				for (const size_t e = index + count; index < e; index++)
@@ -2933,118 +2828,164 @@
 			}
 		}
 
 		//--- construction ---------------------------------------------------------------------------------------------
 
 		static constexpr bool is_trivially_copyable = std::is_trivially_copyable_v<storage_type>;
 
+		// constructibility using memcpy
+
 	  private:
-		// note: these *should* just be regular variable templates but evidently GCC
-		// chokes on partial variable template specialization at class scope:
-		// https://gcc.gnu.org/bugzilla/show_bug.cgi?id=71954
+		template <typename Arg>
+		struct is_constructible_with_memcpy_
+			: std::conjunction<
+				  std::bool_constant<sizeof(storage_type) == sizeof(remove_cvref<Arg>)>, //
+				  std::is_trivially_copyable<storage_type>,								 //
+				  is_implicit_lifetime_type_<storage_type>,								 //
+				  std::is_trivially_copyable<remove_cvref<Arg>>,						 //
+				  std::disjunction<
+					  std::is_same<storage_type, remove_cvref<Arg>>,
+					  std::bool_constant<any_same<storage_type, char, unsigned char, std::byte>
+										 && any_same<remove_cvref<Arg>, char, unsigned char, std::byte>>,
+					  std::conjunction<std::is_same<storage_type, void*>, std::is_pointer<remove_cvref<Arg>>>>>
+		{};
+
+	  public:
+		template <typename Arg>
+		static constexpr bool is_constructible_with_memcpy = is_constructible_with_memcpy_<Arg>::value;
+
+		// constructibility by unpacking a tuple
 
+	  private:
+		template <typename Arg>
+		struct is_constructible_by_unpacking_tuple_ //
+			: detail::is_constructible_by_unpacking_tuple_<storage_type, Arg>
+		{};
+
+	  public:
+		template <typename Arg>
+		static constexpr bool is_constructible_by_unpacking_tuple = is_constructible_by_unpacking_tuple_<Arg>::value;
+
+		// trivial-constructibility
+
+	  private:
 		template <typename... Args>
-		struct is_constructible_with_memcpy_ : std::false_type
+		struct is_trivially_constructible_ : std::is_trivially_constructible<storage_type, remove_cvref<Args>...>
 		{};
+
 		template <typename Arg>
-		struct is_constructible_with_memcpy_<Arg>
-			: std::bool_constant<sizeof(storage_type) == sizeof(remove_cvref<Arg>)	//
-								 && is_trivially_copyable							//
-								 && is_implicit_lifetime_type<storage_type>			//
-								 && std::is_trivially_copyable_v<remove_cvref<Arg>> //
-								 && (std::is_same_v<storage_type, remove_cvref<Arg>>
-									 || (any_same<storage_type, char, unsigned char, std::byte>
-										 && any_same<remove_cvref<Arg>, char, unsigned char, std::byte>)
-									 || (std::is_same_v<storage_type, void*> && std::is_pointer_v<remove_cvref<Arg>>))>
+		struct is_trivially_constructible_<Arg>
+			: std::disjunction<std::is_trivially_constructible<storage_type, remove_cvref<Arg>>,
+							   is_constructible_with_memcpy_<remove_cvref<Arg>>,
+							   typename is_constructible_by_unpacking_tuple_<Arg>::is_trivial>
 		{};
 
 	  public:
 		template <typename... Args>
-		static constexpr bool is_constructible_with_memcpy = is_constructible_with_memcpy_<Args...>::value;
+		static constexpr bool is_trivially_constructible = is_trivially_constructible_<Args...>::value;
 
-		template <typename... Args>
-		static constexpr bool is_trivially_constructible =
-			is_constructible_with_memcpy<Args...>
-			|| std::is_trivially_constructible_v<storage_type, remove_cvref<Args>...>;
+		// constructibility from arbitrary args
 
-	  private:
 		template <typename... Args>
-		struct is_constructible_
-			: std::bool_constant<is_trivially_constructible<Args...> || std::is_constructible_v<storage_type, Args...>>
+		struct is_constructible_trait : std::disjunction<is_trivially_constructible_<Args...>, //
+														 std::is_constructible<storage_type, Args...>>
+		{};
+		template <typename Arg>
+		struct is_constructible_trait<Arg> : std::disjunction<is_trivially_constructible_<Arg>, //
+															  std::is_constructible<storage_type, Arg>,
+															  is_constructible_by_unpacking_tuple_<Arg>>
 		{};
 		template <typename T>
-		struct is_constructible_<T*> : std::bool_constant<std::is_same_v<storage_type, void*> //
-														  || is_trivially_constructible<T*>	  //
-														  || std::is_constructible_v<storage_type, T*>>
+		struct is_constructible_trait<T*> : std::disjunction<std::is_same<storage_type, void*>, //
+															 is_trivially_constructible_<T*>,	//
+															 std::is_constructible<storage_type, T*>>
 		{};
 		template <typename T>
-		struct is_constructible_<T*&> : std::bool_constant<std::is_same_v<storage_type, void*> //
-														   || is_trivially_constructible<T*&>  //
-														   || std::is_constructible_v<storage_type, T*&>>
+		struct is_constructible_trait<T*&> : std::disjunction<std::is_same<storage_type, void*>, //
+															  is_trivially_constructible_<T*&>,	 //
+															  std::is_constructible<storage_type, T*&>>
 		{};
 		template <typename T>
-		struct is_constructible_<T*&&> : std::bool_constant<std::is_same_v<storage_type, void*> //
-															|| is_trivially_constructible<T*&&> //
-															|| std::is_constructible_v<storage_type, T*&&>>
+		struct is_constructible_trait<T*&&> : std::disjunction<std::is_same<storage_type, void*>, //
+															   is_trivially_constructible_<T*&&>, //
+															   std::is_constructible<storage_type, T*&&>>
 		{};
 		template <typename... Args>
-		struct is_constructible_<emplacer<Args...>&&> : is_constructible_<Args...>
+		struct is_constructible_trait<emplacer<Args...>&&> : is_constructible_trait<Args...>
 		{};
 
-	  public:
 		template <typename... Args>
-		static constexpr bool is_constructible = is_constructible_<Args...>::value;
+		static constexpr bool is_constructible = is_constructible_trait<Args...>::value;
+
+		// nothrow-constructibility from arbitrary args
 
-	  private:
 		template <typename... Args>
-		struct is_nothrow_constructible_ : std::bool_constant<is_trivially_constructible<Args...>
-															  || std::is_nothrow_constructible_v<storage_type, Args...>>
+		struct is_nothrow_constructible_trait : std::disjunction<is_trivially_constructible_<Args...>,
+																 std::is_nothrow_constructible<storage_type, Args...>>
+		{};
+		template <typename Arg>
+		struct is_nothrow_constructible_trait<Arg>
+			: std::disjunction<is_trivially_constructible_<Arg>,
+							   std::is_nothrow_constructible<storage_type, Arg>,
+							   typename is_constructible_by_unpacking_tuple_<Arg>::is_nothrow>
 		{};
 		template <typename T>
-		struct is_nothrow_constructible_<T*> : std::bool_constant<std::is_same_v<storage_type, void*> //
-																  || is_trivially_constructible<T*>	  //
-																  || std::is_nothrow_constructible_v<storage_type, T*>>
+		struct is_nothrow_constructible_trait<T*> : std::disjunction<std::is_same<storage_type, void*>, //
+																	 is_trivially_constructible_<T*>,	//
+																	 std::is_nothrow_constructible<storage_type, T*>>
 		{};
 		template <typename T>
-		struct is_nothrow_constructible_<T*&>
-			: std::bool_constant<std::is_same_v<storage_type, void*> //
-								 || is_trivially_constructible<T*&>	 //
-								 || std::is_nothrow_constructible_v<storage_type, T*&>>
+		struct is_nothrow_constructible_trait<T*&> : std::disjunction<std::is_same<storage_type, void*>, //
+																	  is_trivially_constructible_<T*&>,	 //
+																	  std::is_nothrow_constructible<storage_type, T*&>>
 		{};
 		template <typename T>
-		struct is_nothrow_constructible_<T*&&>
-			: std::bool_constant<std::is_same_v<storage_type, void*> //
-								 || is_trivially_constructible<T*&&> //
-								 || std::is_nothrow_constructible_v<storage_type, T*&&>>
+		struct is_nothrow_constructible_trait<T*&&>
+			: std::disjunction<std::is_same<storage_type, void*>, //
+							   is_trivially_constructible_<T*&&>, //
+							   std::is_nothrow_constructible<storage_type, T*&&>>
 		{};
 		template <typename... Args>
-		struct is_nothrow_constructible_<emplacer<Args...>&&> : is_nothrow_constructible_<Args...>
+		struct is_nothrow_constructible_trait<emplacer<Args...>&&> : is_nothrow_constructible_trait<Args...>
 		{};
 
-	  public:
 		template <typename... Args>
-		static constexpr bool is_nothrow_constructible = is_nothrow_constructible_<Args...>::value;
+		static constexpr bool is_nothrow_constructible = is_nothrow_constructible_trait<Args...>::value;
 
 	  private:
 		template <typename... Args, size_t... Indices>
 		SOAGEN_ATTR(nonnull)
+		SOAGEN_ALWAYS_INLINE
 		static constexpr storage_type& construct_from_emplacer(std::byte* destination,
 															   emplacer<Args...>&& args,
 															   std::index_sequence<Indices...>) //
 			noexcept(is_nothrow_constructible<Args...>)
 		{
 			static_assert((std::is_reference_v<Args> && ...));
 			static_assert(sizeof...(Args) == sizeof...(Indices));
 			SOAGEN_ASSUME(destination != nullptr);
 
 			return construct(destination,
 							 static_cast<Args>(*static_cast<std::add_pointer_t<std::remove_reference_t<Args>>>(
 								 args.ptrs[Indices]))...);
 		}
 
+		template <typename Tuple, size_t... Indices>
+		SOAGEN_ATTR(nonnull)
+		SOAGEN_ALWAYS_INLINE
+		static constexpr storage_type& construct_from_tuple(std::byte* destination,
+															Tuple&& tuple,
+															std::index_sequence<Indices...>) //
+			noexcept(is_constructible_by_unpacking_tuple_<Tuple&&>::is_nothrow::value)
+		{
+			SOAGEN_ASSUME(destination != nullptr);
+
+			return construct(destination, get_from_tuple<Indices>(static_cast<Tuple&&>(tuple))...);
+		}
+
 	  public:
 		SOAGEN_CONSTRAINED_TEMPLATE(is_constructible<Args&&...>, typename... Args)
 		SOAGEN_ATTR(nonnull)
 		static constexpr storage_type& construct(std::byte* destination, Args&&... args) //
 			noexcept(is_nothrow_constructible<Args&&...>)
 		{
 			SOAGEN_ASSUME(destination != nullptr);
@@ -3058,29 +2999,36 @@
 				if constexpr (sizeof...(Args) == 1 && (is_emplacer<std::remove_reference_t<Args>> && ...))
 				{
 					return construct_from_emplacer(
 						destination,
 						static_cast<Args&&>(args)...,
 						std::make_index_sequence<std::tuple_size_v<remove_cvref<Args>>>{}...);
 				}
-				else if constexpr (is_constructible_with_memcpy<Args&&...>)
+				else if constexpr (sizeof...(Args) == 1 && (is_constructible_with_memcpy<Args&&> && ...))
 				{
-					std::memcpy(soagen_storage_ptr(destination), soagen_storage_ptr(&args)..., sizeof(storage_type));
+					std::memcpy(soagen_aligned_storage(destination), &args..., sizeof(storage_type));
 
 					return get(destination);
 				}
-				else if constexpr (std::is_aggregate_v<storage_type>)
+				else if constexpr (std::is_constructible_v<storage_type, Args&&...>)
 				{
-					return *(::new (static_cast<void*>(soagen_storage_ptr(destination)))
-								 storage_type{ static_cast<Args&&>(args)... });
+					if constexpr (std::is_aggregate_v<storage_type>)
+					{
+						return *(::new (static_cast<void*>(destination)) storage_type{ static_cast<Args&&>(args)... });
+					}
+					else
+					{
+						return *(::new (static_cast<void*>(destination)) storage_type(static_cast<Args&&>(args)...));
+					}
 				}
-				else
+				else if constexpr (sizeof...(Args) == 1 && (is_constructible_by_unpacking_tuple<Args&&> && ...))
 				{
-					return *(::new (static_cast<void*>(soagen_storage_ptr(destination)))
-								 storage_type(static_cast<Args&&>(args)...));
+					return construct_from_tuple(destination,
+												static_cast<Args&&>(args)...,
+												std::make_index_sequence<std::tuple_size_v<remove_cvref<Args>>>{}...);
 				}
 			}
 		}
 
 		SOAGEN_CONSTRAINED_TEMPLATE(is_constructible<Args&&...>, typename... Args)
 		SOAGEN_ATTR(nonnull)
 		static constexpr storage_type& construct_at(std::byte* buffer, size_t index, Args&&... args) //
@@ -3294,16 +3242,16 @@
 		{
 			SOAGEN_ASSUME(destination != nullptr);
 			SOAGEN_ASSUME(source != nullptr);
 			SOAGEN_ASSUME(destination != source);
 
 			if constexpr (is_constructible_with_memcpy<storage_type&&>)
 			{
-				std::memcpy(soagen_storage_ptr(destination),
-							soagen_storage_ptr(static_cast<std::byte*>(source)),
+				std::memcpy(soagen_aligned_storage(destination),
+							soagen_aligned_storage(static_cast<std::byte*>(source)),
 							sizeof(storage_type));
 
 				return get(destination);
 			}
 			else if constexpr (is_trivially_move_assignable || std::is_move_assignable_v<storage_type>)
 			{
 				return get(destination) = static_cast<storage_type&&>(get(static_cast<std::byte*>(source)));
@@ -3361,16 +3309,16 @@
 		{
 			SOAGEN_ASSUME(destination != nullptr);
 			SOAGEN_ASSUME(source != nullptr);
 			SOAGEN_ASSUME(destination != source);
 
 			if constexpr (is_constructible_with_memcpy<storage_type&&>)
 			{
-				std::memcpy(soagen_storage_ptr(destination),
-							soagen_storage_ptr(static_cast<const std::byte*>(source)),
+				std::memcpy(soagen_aligned_storage(destination),
+							soagen_aligned_storage(static_cast<const std::byte*>(source)),
 							sizeof(storage_type));
 
 				return get(destination);
 			}
 			else if constexpr (is_trivially_copy_assignable || std::is_copy_assignable_v<storage_type>)
 			{
 				return get(destination) = static_cast<const storage_type&>(get(source));
@@ -3429,17 +3377,17 @@
 			SOAGEN_ASSUME(lhs != nullptr);
 			SOAGEN_ASSUME(rhs != nullptr);
 			SOAGEN_ASSUME(lhs != rhs);
 
 			if constexpr (is_trivially_swappable)
 			{
 				alignas(storage_type) std::byte buf[sizeof(storage_type)];
-				std::memcpy(soagen_storage_ptr(buf), soagen_storage_ptr(lhs), sizeof(storage_type));
-				std::memcpy(soagen_storage_ptr(lhs), soagen_storage_ptr(rhs), sizeof(storage_type));
-				std::memcpy(soagen_storage_ptr(rhs), soagen_storage_ptr(buf), sizeof(storage_type));
+				std::memcpy(soagen_aligned_storage(buf), soagen_aligned_storage(lhs), sizeof(storage_type));
+				std::memcpy(soagen_aligned_storage(lhs), soagen_aligned_storage(rhs), sizeof(storage_type));
+				std::memcpy(soagen_aligned_storage(rhs), soagen_aligned_storage(buf), sizeof(storage_type));
 			}
 			else if constexpr (std::is_swappable_v<storage_type>)
 			{
 				using std::swap;
 				swap(get(lhs), get(rhs));
 			}
 			else
@@ -3464,32 +3412,32 @@
 		{
 			SOAGEN_ASSUME(lhs_buffer != nullptr);
 			SOAGEN_ASSUME(rhs_buffer != nullptr);
 
 			if SOAGEN_UNLIKELY(!count)
 				return;
 
-			lhs_buffer = soagen_storage_ptr(lhs_buffer + lhs_index * sizeof(storage_type));
-			rhs_buffer = soagen_storage_ptr(rhs_buffer + rhs_index * sizeof(storage_type));
+			lhs_buffer = soagen_aligned_storage(lhs_buffer + lhs_index * sizeof(storage_type));
+			rhs_buffer = soagen_aligned_storage(rhs_buffer + rhs_index * sizeof(storage_type));
 
 			[[maybe_unused]] SOAGEN_CPP23_STATIC_CONSTEXPR size_t trivial_buf_size = 2048u / sizeof(storage_type);
 
 			if constexpr (is_trivially_swappable && trivial_buf_size > 1)
 			{
 				for (size_t i = 0; i < count; i += trivial_buf_size)
 				{
 					const auto num = soagen::min(trivial_buf_size, count - i);
 
 					alignas(storage_type) std::byte buf[sizeof(storage_type) * trivial_buf_size];
 					std::memcpy(buf, lhs_buffer, sizeof(storage_type) * num);
 					std::memcpy(lhs_buffer, rhs_buffer, sizeof(storage_type) * num);
 					std::memcpy(rhs_buffer, buf, sizeof(storage_type) * num);
 
-					lhs_buffer = soagen_storage_ptr(lhs_buffer + trivial_buf_size * sizeof(storage_type));
-					rhs_buffer = soagen_storage_ptr(rhs_buffer + trivial_buf_size * sizeof(storage_type));
+					lhs_buffer = soagen_aligned_storage(lhs_buffer + trivial_buf_size * sizeof(storage_type));
+					rhs_buffer = soagen_aligned_storage(rhs_buffer + trivial_buf_size * sizeof(storage_type));
 				}
 			}
 			else
 			{
 				const auto end = lhs_buffer + count * sizeof(storage_type);
 				for (; lhs_buffer < end; lhs_buffer += sizeof(storage_type), rhs_buffer += sizeof(storage_type))
 				{
@@ -3506,16 +3454,16 @@
 									  const std::byte* source_buffer,
 									  size_t source_index,
 									  size_t count = 1) noexcept
 		{
 			SOAGEN_ASSUME(dest_buffer != nullptr);
 			SOAGEN_ASSUME(source_buffer != nullptr);
 
-			std::memmove(soagen_storage_ptr(dest_buffer + dest_index * sizeof(storage_type)),
-						 soagen_storage_ptr(source_buffer + source_index * sizeof(storage_type)),
+			std::memmove(soagen_aligned_storage(dest_buffer + dest_index * sizeof(storage_type)),
+						 soagen_aligned_storage(source_buffer + source_index * sizeof(storage_type)),
 						 count * sizeof(storage_type));
 		}
 
 		//--- equality -------------------------------------------------------------------------------------------------
 
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = is_equality_comparable<storage_type>)
 		SOAGEN_NODISCARD
@@ -3652,61 +3600,92 @@
 		static_assert(std::is_base_of_v<type, column_traits<ValueType, Align, ParamType>>);
 	};
 
 	template <typename T>
 	using to_base_traits = typename to_base_traits_<T>::type;
 }
 
-#undef soagen_storage_ptr
+#undef soagen_aligned_storage
 
-#if SOAGEN_ALWAYS_OPTIMIZE
-	#if SOAGEN_MSVC
-		#pragma strict_gs_check(pop)
-		#pragma runtime_checks("", restore)
-		#pragma optimize("", on)
-		#pragma inline_recursion(off)
-	#elif SOAGEN_GCC
-		#pragma GCC pop_options
-	#endif
-#endif
+//********  invoke.hpp  ************************************************************************************************
 
-#if SOAGEN_MSVC_LIKE
-	#pragma pop_macro("min")
-	#pragma pop_macro("max")
-#endif
+namespace soagen
+{
+	namespace detail
+	{
+		template <typename Func, typename... Args>
+		struct is_invocable_ : nested_trait_<types_<Func, Args...>, std::is_invocable, std::is_nothrow_invocable>
+		{
+			using base = nested_trait_<types_<Func, Args...>, std::is_invocable, std::is_nothrow_invocable>;
 
-SOAGEN_POP_WARNINGS;
+			using is_nothrow = typename base::template nested<0>;
+		};
+	}
 
-//********  table_traits.hpp  ******************************************************************************************
+	template <typename Func, typename... Args>
+	inline constexpr bool is_invocable = POXY_IMPLEMENTATION_DETAIL(detail::is_invocable_<Func, Args...>::value);
 
-SOAGEN_PUSH_WARNINGS;
-SOAGEN_DISABLE_SPAM_WARNINGS;
+	template <typename Func, typename... Args>
+	inline constexpr bool is_nothrow_invocable =
+		POXY_IMPLEMENTATION_DETAIL(detail::is_invocable_<Func, Args...>::is_nothrow::value);
 
-#if SOAGEN_MSVC_LIKE
-	#pragma push_macro("min")
-	#pragma push_macro("max")
-	#undef min
-	#undef max
-#endif
+	namespace detail
+	{
+		template <size_t I, typename Func, typename Arg>
+		struct is_invocable_with_optional_index_							//
+			: std::disjunction<is_invocable_<Func, Arg, index_constant<I>>, //
+							   is_invocable_<Func, Arg, size_t>,			//
+							   is_invocable_<Func, index_constant<I>, Arg>, //
+							   is_invocable_<Func, size_t, Arg>,			//
+							   is_invocable_<Func, Arg>>
+		{};
+	}
 
-#if SOAGEN_ALWAYS_OPTIMIZE
-	#if SOAGEN_MSVC
-		#pragma inline_recursion(on)
-		#pragma optimize("gt", on)
-		#pragma runtime_checks("", off)
-		#pragma strict_gs_check(push, off)
-	#elif SOAGEN_GCC
-		#pragma GCC push_options
-		#pragma GCC optimize("O2")
-	#endif
-#endif
+	template <size_t I, typename Func, typename Arg>
+	inline constexpr bool is_invocable_with_optional_index =
+		POXY_IMPLEMENTATION_DETAIL(detail::is_invocable_with_optional_index_<I, Func, Arg>::value);
 
-#if SOAGEN_CLANG >= 16
-	#pragma clang diagnostic ignored "-Wunsafe-buffer-usage"
-#endif
+	template <size_t I, typename Func, typename Arg>
+	inline constexpr bool is_nothrow_invocable_with_optional_index =
+		POXY_IMPLEMENTATION_DETAIL(detail::is_invocable_with_optional_index_<I, Func, Arg>::is_nothrow::value);
+
+	template <size_t I, typename Func, typename Arg>
+	SOAGEN_ALWAYS_INLINE
+	constexpr decltype(auto) invoke_with_optional_index(Func&& func,
+														Arg&& arg) //
+		noexcept(is_nothrow_invocable_with_optional_index<I, Func&&, Arg&&>)
+	{
+		static_assert(is_invocable_with_optional_index<I, Func&&, Arg&&>);
+
+		if constexpr (is_invocable<Func&&, Arg&&, index_constant<I>>)
+		{
+			return static_cast<Func&&>(func)(static_cast<Arg&&>(arg), index_constant<I>{});
+		}
+		else if constexpr (is_invocable<Func&&, Arg&&, size_t>)
+		{
+			return static_cast<Func&&>(func)(static_cast<Arg&&>(arg), I);
+		}
+		else if constexpr (is_invocable<Func&&, index_constant<I>, Arg&&>)
+		{
+			return static_cast<Func&&>(func)(index_constant<I>{}, static_cast<Arg&&>(arg));
+		}
+		else if constexpr (is_invocable<Func&&, size_t, Arg&&>)
+		{
+			return static_cast<Func&&>(func)(I, static_cast<Arg&&>(arg));
+		}
+		else
+		{
+			static_assert(is_invocable<Func&&, Arg&&>);
+
+			return static_cast<Func&&>(func)(static_cast<Arg&&>(arg));
+		}
+	}
+}
+
+//********  table_traits.hpp  ******************************************************************************************
 
 namespace soagen::detail
 {
 	// a base class for the table traits that handles all the non-alignment-dependent stuff -
 	// the 'Columns' argument seen by this class should be the column_base_traits, NOT soagen::column_traits
 	// (to minimize template instantiation explosion)
 	template <typename...>
@@ -3737,21 +3716,21 @@
 		using const_column_pointers = std::byte* const[column_count];
 
 		static constexpr size_t column_sizes[column_count] = { sizeof(typename Columns::storage_type)... };
 
 		// default constructibility
 
 		static constexpr bool all_default_constructible =
-			(std::is_default_constructible_v<typename Columns::storage_type> && ...);
+			std::conjunction<std::is_default_constructible<typename Columns::storage_type>...>::value;
 
 		static constexpr bool all_nothrow_default_constructible =
-			(std::is_nothrow_default_constructible_v<typename Columns::storage_type> && ...);
+			std::conjunction<std::is_nothrow_default_constructible<typename Columns::storage_type>...>::value;
 
 		static constexpr bool all_trivially_default_constructible =
-			(std::is_trivially_default_constructible_v<typename Columns::storage_type> && ...);
+			std::conjunction<std::is_trivially_default_constructible<typename Columns::storage_type>...>::value;
 
 		// trivial-copyability (memcpy + memmove)
 
 		static constexpr bool all_trivially_copyable = (Columns::is_trivially_copyable && ...);
 
 		static constexpr bool any_trivially_copyable = (false || ... || Columns::is_trivially_copyable);
 
@@ -3785,115 +3764,114 @@
 
 		static constexpr bool all_nothrow_move_assignable = (Columns::is_nothrow_move_assignable && ...);
 
 		static constexpr bool all_trivially_move_assignable = (Columns::is_trivially_move_assignable && ...);
 
 		// destructibility
 
-		static constexpr bool all_destructible = (std::is_destructible_v<typename Columns::storage_type> && ...);
+		static constexpr bool all_destructible =
+			std::conjunction<std::is_destructible<typename Columns::storage_type>...>::value;
 
 		static constexpr bool all_nothrow_destructible =
-			(std::is_nothrow_destructible_v<typename Columns::storage_type> && ...);
+			std::conjunction<std::is_nothrow_destructible<typename Columns::storage_type>...>::value;
 
 		static constexpr bool all_trivially_destructible =
-			(std::is_trivially_destructible_v<typename Columns::storage_type> && ...);
+			std::conjunction<std::is_trivially_destructible<typename Columns::storage_type>...>::value;
 
 		// swappability
 
 		static constexpr bool all_swappable = (Columns::is_swappable && ...);
 
 		static constexpr bool all_nothrow_swappable = (Columns::is_nothrow_swappable && ...);
 
 		// equality comparability
 
-		static constexpr bool all_equality_comparable = (is_equality_comparable<typename Columns::storage_type> && ...);
+		static constexpr bool all_equality_comparable =
+			std::conjunction<is_equality_comparable_<typename Columns::storage_type>...>::value;
 
 		static constexpr bool all_nothrow_equality_comparable =
-			(is_nothrow_equality_comparable<typename Columns::storage_type> && ...);
+			std::conjunction<is_nothrow_equality_comparable_<typename Columns::storage_type>...>::value;
 
 		// less-than comparability
 
 		static constexpr bool all_less_than_comparable =
-			(is_less_than_comparable<typename Columns::storage_type> && ...);
+			std::conjunction<is_less_than_comparable_<typename Columns::storage_type>...>::value;
 
 		static constexpr bool all_nothrow_less_than_comparable =
-			(is_nothrow_less_than_comparable<typename Columns::storage_type> && ...);
+			std::conjunction<is_nothrow_less_than_comparable_<typename Columns::storage_type>...>::value;
 
 		// row constructibility
 
 	  private:
 		template <size_t, typename...>
 		struct row_constructible_from_tuple_ : std::false_type
 		{};
 		template <typename Tuple, size_t... Members>
 		struct row_constructible_from_tuple_<column_count, Tuple, std::index_sequence<Members...>>
-			: std::bool_constant<(
-				  Columns::template is_constructible<decltype(get_from_tuple_like<Members>(std::declval<Tuple>()))>
-				  && ...)>
+			: std::conjunction<typename Columns::template is_constructible_trait<decltype(get_from_tuple<Members>(
+				  std::declval<Tuple>()))>...>
 		{
 			static_assert(std::is_same_v<std::index_sequence<Members...>, std::make_index_sequence<column_count>>);
 		};
 
 		template <bool, size_t, typename... Args>
 		struct row_constructible_from_ : std::false_type
 		{};
 		template <typename... Args>
 		struct row_constructible_from_<false, column_count, Args...>
-			: std::bool_constant<(Columns::template is_constructible<Args> && ...)>
+			: std::conjunction<typename Columns::template is_constructible_trait<Args>...>
 		{
 			static_assert(sizeof...(Args) == column_count);
 		};
 		template <typename Tuple>
 		struct row_constructible_from_<true, 1, Tuple>
 			: row_constructible_from_tuple_<std::tuple_size_v<remove_cvref<Tuple>>,
 											remove_cvref<Tuple>,
 											std::make_index_sequence<std::tuple_size_v<remove_cvref<Tuple>>>>
 		{};
 
 	  public:
 		template <typename... Args>
 		static constexpr bool row_constructible_from =
-			row_constructible_from_<(is_tuple_like<remove_cvref<Args>> && ...), sizeof...(Args), Args...>::value;
+			row_constructible_from_<(is_tuple<remove_cvref<Args>> && ...), sizeof...(Args), Args...>::value;
 
 		// row constructibility (nothrow)
 
 	  private:
 		template <size_t, typename...>
 		struct row_nothrow_constructible_from_tuple_ : std::false_type
 		{};
 		template <typename Tuple, size_t... Members>
 		struct row_nothrow_constructible_from_tuple_<column_count, Tuple, std::index_sequence<Members...>>
-			: std::bool_constant<(Columns::template is_nothrow_constructible<decltype(get_from_tuple_like<Members>(
-									  std::declval<Tuple>()))>
-								  && ...)>
+			: std::conjunction<typename Columns::template is_nothrow_constructible_trait<
+				  decltype(get_from_tuple<Members>(std::declval<Tuple>()))>...>
 		{
 			static_assert(std::is_same_v<std::index_sequence<Members...>, std::make_index_sequence<column_count>>);
 		};
 
 		template <bool, size_t, typename... Args>
 		struct row_nothrow_constructible_from_ : std::false_type
 		{};
 		template <typename... Args>
 		struct row_nothrow_constructible_from_<false, column_count, Args...>
-			: std::bool_constant<(Columns::template is_nothrow_constructible<Args> && ...)>
+			: std::conjunction<typename Columns::template is_nothrow_constructible_trait<Args>...>
 		{
 			static_assert(sizeof...(Args) == column_count);
 		};
 		template <typename Tuple>
 		struct row_nothrow_constructible_from_<true, 1, Tuple>
 			: row_nothrow_constructible_from_tuple_<std::tuple_size_v<remove_cvref<Tuple>>,
 													remove_cvref<Tuple>,
 													std::make_index_sequence<std::tuple_size_v<remove_cvref<Tuple>>>>
 		{};
 
 	  public:
 		template <typename... Args>
 		static constexpr bool row_nothrow_constructible_from =
-			row_nothrow_constructible_from_<(is_tuple_like<remove_cvref<Args>> && ...), sizeof...(Args), Args...>::
-				value;
+			row_nothrow_constructible_from_<(is_tuple<remove_cvref<Args>> && ...), sizeof...(Args), Args...>::value;
 
 		//--- memmove --------------------------------------------------------------------------------------------------
 
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = all_trivially_copyable)
 		SOAGEN_CPP20_CONSTEXPR
 		static void memmove(column_pointers& dest,
 							size_t dest_start,
@@ -4051,36 +4029,36 @@
 		}
 
 		//--- construction ---------------------------------------------------------------------------------------------
 
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, typename Tuple, auto sfinae = row_constructible_from<Tuple&&>)
 		SOAGEN_ALWAYS_INLINE
 		SOAGEN_CPP20_CONSTEXPR
-		static void construct_row_from_tuple_like(column_pointers& columns,
-												  size_t index,
-												  Tuple&& tuple) //
+		static void construct_row_from_tuple(column_pointers& columns,
+											 size_t index,
+											 Tuple&& tuple) //
 			noexcept(row_nothrow_constructible_from<Tuple&&>)
 		{
 			static_assert(std::tuple_size_v<remove_cvref<Tuple>> == column_count);
 
-			construct_row(columns, index, get_from_tuple_like<I>(static_cast<Tuple&&>(tuple))...);
+			construct_row(columns, index, get_from_tuple<I>(static_cast<Tuple&&>(tuple))...);
 		}
 
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, typename... Args, auto sfinae = row_constructible_from<Args&&...>)
 		SOAGEN_CPP20_CONSTEXPR
 		static void construct_row(column_pointers& columns, size_t index, Args&&... args) //
 			noexcept(row_nothrow_constructible_from<Args&&...>)
 		{
 			if constexpr (sizeof...(Args) == 0)
 			{
 				default_construct_row(columns, index, static_cast<Args&&>(args)...);
 			}
-			else if constexpr (sizeof...(Args) == 1 && (is_tuple_like<remove_cvref<Args>> && ...))
+			else if constexpr (sizeof...(Args) == 1 && (is_tuple<remove_cvref<Args>> && ...))
 			{
-				construct_row_from_tuple_like(columns, index, static_cast<Args&&>(args)...);
+				construct_row_from_tuple(columns, index, static_cast<Args&&>(args)...);
 			}
 			else
 			{
 				static_assert(sizeof...(Args) == sizeof...(I));
 
 				if constexpr (row_nothrow_constructible_from<Args&&...> || all_trivially_destructible)
 				{
@@ -4634,60 +4612,16 @@
 	template <typename... Columns>
 	struct table_traits_type_<table_traits<Columns...>>
 	{
 		using type = table_traits<Columns...>;
 	};
 }
 
-#if SOAGEN_ALWAYS_OPTIMIZE
-	#if SOAGEN_MSVC
-		#pragma strict_gs_check(pop)
-		#pragma runtime_checks("", restore)
-		#pragma optimize("", on)
-		#pragma inline_recursion(off)
-	#elif SOAGEN_GCC
-		#pragma GCC pop_options
-	#endif
-#endif
-
-#if SOAGEN_MSVC_LIKE
-	#pragma pop_macro("min")
-	#pragma pop_macro("max")
-#endif
-
-SOAGEN_POP_WARNINGS;
-
 //********  table.hpp  *************************************************************************************************
 
-SOAGEN_PUSH_WARNINGS;
-SOAGEN_DISABLE_SPAM_WARNINGS;
-
-#if SOAGEN_MSVC_LIKE
-	#pragma push_macro("min")
-	#pragma push_macro("max")
-	#undef min
-	#undef max
-#endif
-
-#if SOAGEN_ALWAYS_OPTIMIZE
-	#if SOAGEN_MSVC
-		#pragma inline_recursion(on)
-		#pragma optimize("gt", on)
-		#pragma runtime_checks("", off)
-		#pragma strict_gs_check(push, off)
-	#elif SOAGEN_GCC
-		#pragma GCC push_options
-		#pragma GCC optimize("O2")
-	#endif
-#endif
-
-#if SOAGEN_CLANG >= 16
-	#pragma clang diagnostic ignored "-Wunsafe-buffer-usage"
-#endif
-
 namespace soagen::detail
 {
 	SOAGEN_CONSTRAINED_TEMPLATE(is_unsigned<T>, typename T)
 	SOAGEN_NODISCARD
 	constexpr bool add_without_overflowing(T lhs, T rhs, T& result) noexcept
 	{
 		if (lhs > static_cast<T>(-1) - rhs)
@@ -6153,42 +6087,53 @@
 
 		~table() = default;
 
 		using SOAGEN_BASE_TYPE::SOAGEN_BASE_NAME;
 
 		template <auto Column>
 		SOAGEN_ALIGNED_COLUMN(Column)
-		column_type<Column>* column() noexcept
+		constexpr column_type<Column>* column() noexcept
 		{
 			static_assert(static_cast<size_t>(Column) < table_traits::column_count, "column index out of range");
 
-			return soagen::assume_aligned<
-				detail::actual_column_alignment<table_traits, allocator_type, static_cast<size_t>(Column)>>(
-				SOAGEN_LAUNDER(reinterpret_cast<column_type<static_cast<size_t>(Column)>*>(
-					base::alloc_.columns[static_cast<size_t>(Column)])));
+			using column	   = column_traits<static_cast<size_t>(Column)>;
+			using storage_type = typename column::storage_type;
+			using value_type   = typename column::value_type;
+
+			SOAGEN_CPP23_STATIC_CONSTEXPR size_t align =
+				detail::actual_column_alignment<table_traits, allocator_type, static_cast<size_t>(Column)>;
+
+			if constexpr (std::is_pointer_v<storage_type>)
+			{
+				static_assert(std::is_same_v<storage_type, void*>);
+
+				return soagen::assume_aligned<align>(
+					SOAGEN_LAUNDER(reinterpret_cast<value_type*>(base::alloc_.columns[static_cast<size_t>(Column)])));
+			}
+			else
+			{
+				static_assert(std::is_same_v<storage_type, std::remove_cv_t<value_type>>);
+
+				return soagen::assume_aligned<align>(column::ptr(base::alloc_.columns[static_cast<size_t>(Column)]));
+			}
 		}
 
 		template <auto Column>
 		SOAGEN_ALIGNED_COLUMN(Column)
-		std::add_const_t<column_type<Column>>* column() const noexcept
+		constexpr std::add_const_t<column_type<Column>>* column() const noexcept
 		{
-			static_assert(static_cast<size_t>(Column) < table_traits::column_count, "column index out of range");
-
-			return soagen::assume_aligned<
-				detail::actual_column_alignment<table_traits, allocator_type, static_cast<size_t>(Column)>>(
-				SOAGEN_LAUNDER(reinterpret_cast<column_type<static_cast<size_t>(Column)>*>(
-					base::alloc_.columns[static_cast<size_t>(Column)])));
+			return const_cast<table&>(*this).template column<static_cast<size_t>(Column)>();
 		}
 	};
 
 	template <typename>
 	inline constexpr bool is_table = POXY_IMPLEMENTATION_DETAIL(false);
 
-	template <typename... Args>
-	inline constexpr bool is_table<table<Args...>> = true;
+	template <typename Traits, typename Allocator, template <typename> typename Base>
+	inline constexpr bool is_table<table<Traits, Allocator, Base>> = true;
 	template <typename T>
 	inline constexpr bool is_table<const T> = is_table<T>;
 	template <typename T>
 	inline constexpr bool is_table<volatile T> = is_table<T>;
 	template <typename T>
 	inline constexpr bool is_table<const volatile T> = is_table<T>;
 	namespace detail
@@ -6208,48 +6153,30 @@
 		lhs.swap(rhs);
 	}
 }
 
 #undef SOAGEN_BASE_NAME
 #undef SOAGEN_BASE_TYPE
 
-#if SOAGEN_ALWAYS_OPTIMIZE
-	#if SOAGEN_MSVC
-		#pragma strict_gs_check(pop)
-		#pragma runtime_checks("", restore)
-		#pragma optimize("", on)
-		#pragma inline_recursion(off)
-	#elif SOAGEN_GCC
-		#pragma GCC pop_options
-	#endif
-#endif
-
-#if SOAGEN_MSVC_LIKE
-	#pragma pop_macro("min")
-	#pragma pop_macro("max")
-#endif
-
-SOAGEN_POP_WARNINGS;
-
 //********  mixins.hpp  ************************************************************************************************
 
 namespace soagen::mixins
 {
 	//--- resize() -----------------------------------------------------------------------------------------------------
 
-	template <typename Derived, bool = has_resize_member<table_type<Derived>, typename table_type<Derived>::size_type>>
+	template <typename Derived, bool = has_resize_member<table_type<Derived>>>
 	struct SOAGEN_EMPTY_BASES resizable
 	{
 		using table_type = soagen::table_type<Derived>;
 		using size_type	 = typename table_type::size_type;
 
 		SOAGEN_ALWAYS_INLINE
 		SOAGEN_CPP20_CONSTEXPR
 		Derived& resize(size_type new_size) //
-			noexcept(soagen::has_nothrow_resize_member<table_type, size_type>)
+			noexcept(soagen::has_nothrow_resize_member<table_type>)
 		{
 			static_cast<Derived&>(*this).table().resize(new_size);
 			return static_cast<Derived&>(*this);
 		}
 	};
 
 	template <typename Derived>
@@ -6391,99 +6318,18 @@
 	template <typename Derived>
 	struct SOAGEN_EMPTY_BASES const_data_ptr<Derived, false>
 	{};
 }
 
 //********  iterator.hpp  **********************************************************************************************
 
-SOAGEN_DISABLE_WARNINGS;
-#include <iterator>
-SOAGEN_ENABLE_WARNINGS;
-
-SOAGEN_PUSH_WARNINGS;
-SOAGEN_DISABLE_SPAM_WARNINGS;
-
-#if SOAGEN_MSVC_LIKE
-	#pragma push_macro("min")
-	#pragma push_macro("max")
-	#undef min
-	#undef max
-#endif
-
-#if SOAGEN_ALWAYS_OPTIMIZE
-	#if SOAGEN_MSVC
-		#pragma inline_recursion(on)
-		#pragma optimize("gt", on)
-		#pragma runtime_checks("", off)
-		#pragma strict_gs_check(push, off)
-	#elif SOAGEN_GCC
-		#pragma GCC push_options
-		#pragma GCC optimize("O2")
-	#endif
-#endif
-
 namespace soagen
 {
-	template <typename, size_t...>
-	class iterator;
-
 	namespace detail
 	{
-		// iterator implicit conversions are allowed when:
-		// - changing columns
-		// - losing rvalue (Table&& -> Table&), (const Table&& -> const Table&)
-		// - gaining const (Table& -> const Table&, Table&& -> const Table&&)
-		// - any combination of the three
-
-		template <typename From, typename To>
-		inline constexpr bool iterator_implicit_conversion_ok = false;
-
-		template <typename Table, size_t... ColumnsA, size_t... ColumnsB>
-		inline constexpr bool iterator_implicit_conversion_ok<iterator<Table, ColumnsA...>, //
-															  iterator<Table, ColumnsB...>> = true;
-
-		template <typename Table, size_t... ColumnsA, size_t... ColumnsB>
-		inline constexpr bool iterator_implicit_conversion_ok<iterator<Table&&, ColumnsA...>, //
-															  iterator<Table&, ColumnsB...>> = true;
-
-		template <typename Table, size_t... ColumnsA, size_t... ColumnsB>
-		inline constexpr bool iterator_implicit_conversion_ok<iterator<const Table&&, ColumnsA...>, //
-															  iterator<const Table&, ColumnsB...>> = true;
-
-		template <typename Table, size_t... ColumnsA, size_t... ColumnsB>
-		inline constexpr bool iterator_implicit_conversion_ok<iterator<Table&, ColumnsA...>, //
-															  iterator<const Table&, ColumnsB...>> = true;
-
-		template <typename Table, size_t... ColumnsA, size_t... ColumnsB>
-		inline constexpr bool iterator_implicit_conversion_ok<iterator<Table&&, ColumnsA...>, //
-															  iterator<const Table&&, ColumnsB...>> = true;
-
-		template <typename Table, size_t... ColumnsA, size_t... ColumnsB>
-		inline constexpr bool iterator_implicit_conversion_ok<iterator<Table&&, ColumnsA...>, //
-															  iterator<const Table&, ColumnsB...>> = true;
-
-		// iterator explicit conversions are allowed when gaining rvalue and optionally gaining const
-		// (note that we specifically avoid providing anything that would be the moral equivalent of
-		// a const_cast because that armory is filled with very large and powerful footguns)
-
-		template <typename From, typename To>
-		inline constexpr bool iterator_explicit_conversion_ok = false;
-
-		template <typename Table, size_t... ColumnsA, size_t... ColumnsB>
-		inline constexpr bool iterator_explicit_conversion_ok<iterator<Table&, ColumnsA...>, //
-															  iterator<Table&&, ColumnsB...>> = true;
-
-		template <typename Table, size_t... ColumnsA, size_t... ColumnsB>
-		inline constexpr bool iterator_explicit_conversion_ok<iterator<const Table&, ColumnsA...>, //
-															  iterator<const Table&&, ColumnsB...>> = true;
-
-		template <typename Table, size_t... ColumnsA, size_t... ColumnsB>
-		inline constexpr bool iterator_explicit_conversion_ok<iterator<Table&, ColumnsA...>, //
-															  iterator<const Table&&, ColumnsB...>> = true;
-
 		template <typename T>
 		struct arrow_proxy
 		{
 			mutable T value;
 
 			SOAGEN_PURE_INLINE_GETTER
 			constexpr T* operator->() const noexcept
@@ -6606,15 +6452,15 @@
 
 		SOAGEN_PURE_INLINE_GETTER
 		friend constexpr iterator operator-(const iterator& it, difference_type n) noexcept
 		{
 			return it + (-n);
 		}
 
-		SOAGEN_CONSTRAINED_TEMPLATE((detail::same_table_type<Table, T>), typename T, size_t... Cols)
+		SOAGEN_CONSTRAINED_TEMPLATE((same_table_type<Table, T>), typename T, size_t... Cols)
 		SOAGEN_PURE_GETTER
 		constexpr difference_type operator-(const iterator<T, Cols...>& rhs) const noexcept
 		{
 			return base::offset - rhs.offset;
 		}
 
 		SOAGEN_PURE_GETTER
@@ -6639,68 +6485,68 @@
 			SOAGEN_ASSUME(!!base::table);
 			SOAGEN_ASSUME(base::offset + offset >= 0);
 
 			return static_cast<table_ref>(*const_cast<table_ptr>(base::table))
 				.template row<Columns...>(static_cast<size_type>(base::offset + offset));
 		}
 
-		SOAGEN_CONSTRAINED_TEMPLATE((detail::same_table_type<Table, T>), typename T, size_t... Cols)
+		SOAGEN_CONSTRAINED_TEMPLATE((same_table_type<Table, T>), typename T, size_t... Cols)
 		SOAGEN_PURE_GETTER
 		constexpr bool operator==(const iterator<T, Cols...>& rhs) const noexcept
 		{
 			return base::table == rhs.table && base::offset == rhs.offset;
 		}
 
-		SOAGEN_CONSTRAINED_TEMPLATE((detail::same_table_type<Table, T>), typename T, size_t... Cols)
+		SOAGEN_CONSTRAINED_TEMPLATE((same_table_type<Table, T>), typename T, size_t... Cols)
 		SOAGEN_PURE_INLINE_GETTER
 		friend constexpr bool operator!=(const iterator& lhs, const iterator<T, Cols...>& rhs) noexcept
 		{
 			return !(lhs == rhs);
 		}
 
-		SOAGEN_CONSTRAINED_TEMPLATE((detail::same_table_type<Table, T>), typename T, size_t... Cols)
+		SOAGEN_CONSTRAINED_TEMPLATE((same_table_type<Table, T>), typename T, size_t... Cols)
 		SOAGEN_PURE_INLINE_GETTER
 		constexpr bool operator<(const iterator<T, Cols...>& rhs) const noexcept
 		{
 			return base::offset < rhs.offset;
 		}
 
-		SOAGEN_CONSTRAINED_TEMPLATE((detail::same_table_type<Table, T>), typename T, size_t... Cols)
+		SOAGEN_CONSTRAINED_TEMPLATE((same_table_type<Table, T>), typename T, size_t... Cols)
 		SOAGEN_PURE_INLINE_GETTER
 		constexpr bool operator<=(const iterator<T, Cols...>& rhs) const noexcept
 		{
 			return base::offset <= rhs.offset;
 		}
 
-		SOAGEN_CONSTRAINED_TEMPLATE((detail::same_table_type<Table, T>), typename T, size_t... Cols)
+		SOAGEN_CONSTRAINED_TEMPLATE((same_table_type<Table, T>), typename T, size_t... Cols)
 		SOAGEN_PURE_INLINE_GETTER
 		constexpr bool operator>(const iterator<T, Cols...>& rhs) const noexcept
 		{
 			return base::offset > rhs.offset;
 		}
 
-		SOAGEN_CONSTRAINED_TEMPLATE((detail::same_table_type<Table, T>), typename T, size_t... Cols)
+		SOAGEN_CONSTRAINED_TEMPLATE((same_table_type<Table, T>), typename T, size_t... Cols)
 		SOAGEN_PURE_INLINE_GETTER
 		constexpr bool operator>=(const iterator<T, Cols...>& rhs) const noexcept
 		{
 			return base::offset >= rhs.offset;
 		}
 
-		SOAGEN_CONSTRAINED_TEMPLATE((detail::iterator_implicit_conversion_ok<iterator, iterator<T, Cols...>>
-									 && !detail::iterator_explicit_conversion_ok<iterator, iterator<T, Cols...>>),
+		SOAGEN_CONSTRAINED_TEMPLATE((detail::implicit_conversion_ok<Table, T>
+									 && !detail::explicit_conversion_ok<Table, T>),
 									typename T,
 									size_t... Cols)
 		SOAGEN_PURE_INLINE_GETTER
 		constexpr operator iterator<T, Cols...>() const noexcept
 		{
 			return iterator<T, Cols...>{ static_cast<const base&>(*this) };
 		}
 
-		SOAGEN_CONSTRAINED_TEMPLATE((!detail::iterator_implicit_conversion_ok<iterator, iterator<T, Cols...>>
-									 && detail::iterator_explicit_conversion_ok<iterator, iterator<T, Cols...>>),
+		SOAGEN_CONSTRAINED_TEMPLATE((!detail::implicit_conversion_ok<Table, T>
+									 && detail::explicit_conversion_ok<Table, T>),
 									typename T,
 									size_t... Cols)
 		SOAGEN_PURE_INLINE_GETTER
 		explicit constexpr operator iterator<T, Cols...>() const noexcept
 		{
 			return iterator<T, Cols...>{ static_cast<const base&>(*this) };
 		}
```

### Comparing `soagen-0.3.0/src/soagen/hpp/soagen.hpp` & `soagen-0.4.0/src/soagen/hpp/soagen.hpp`

 * *Files identical despite different names*

### Comparing `soagen-0.3.0/src/soagen/hpp/table.hpp` & `soagen-0.4.0/src/soagen/hpp/table.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -5,18 +5,14 @@
 #pragma once
 
 #include "generated/compressed_pair.hpp"
 #include "allocator.hpp"
 #include "table_traits.hpp"
 #include "header_start.hpp"
 
-#if SOAGEN_CLANG >= 16
-	#pragma clang diagnostic ignored "-Wunsafe-buffer-usage"
-#endif
-
 /// @cond
 namespace soagen::detail
 {
 	SOAGEN_CONSTRAINED_TEMPLATE(is_unsigned<T>, typename T)
 	SOAGEN_NODISCARD
 	constexpr bool add_without_overflowing(T lhs, T rhs, T& result) noexcept
 	{
@@ -1644,46 +1640,57 @@
 		/// @availability This method is only available when all the column types are trivially-copyable.
 		constexpr const std::byte* data() const noexcept;
 #endif
 
 		/// @brief Returns a pointer to the elements of a specific column.
 		template <auto Column>
 		SOAGEN_ALIGNED_COLUMN(Column)
-		column_type<Column>* column() noexcept
+		constexpr column_type<Column>* column() noexcept
 		{
 			static_assert(static_cast<size_t>(Column) < table_traits::column_count, "column index out of range");
 
-			return soagen::assume_aligned<
-				detail::actual_column_alignment<table_traits, allocator_type, static_cast<size_t>(Column)>>(
-				SOAGEN_LAUNDER(reinterpret_cast<column_type<static_cast<size_t>(Column)>*>(
-					base::alloc_.columns[static_cast<size_t>(Column)])));
+			using column	   = column_traits<static_cast<size_t>(Column)>;
+			using storage_type = typename column::storage_type;
+			using value_type   = typename column::value_type;
+
+			SOAGEN_CPP23_STATIC_CONSTEXPR size_t align =
+				detail::actual_column_alignment<table_traits, allocator_type, static_cast<size_t>(Column)>;
+
+			if constexpr (std::is_pointer_v<storage_type>)
+			{
+				static_assert(std::is_same_v<storage_type, void*>);
+
+				return soagen::assume_aligned<align>(
+					SOAGEN_LAUNDER(reinterpret_cast<value_type*>(base::alloc_.columns[static_cast<size_t>(Column)])));
+			}
+			else
+			{
+				static_assert(std::is_same_v<storage_type, std::remove_cv_t<value_type>>);
+
+				return soagen::assume_aligned<align>(column::ptr(base::alloc_.columns[static_cast<size_t>(Column)]));
+			}
 		}
 
 		/// @brief Returns a pointer to the elements of a specific column.
 		template <auto Column>
 		SOAGEN_ALIGNED_COLUMN(Column)
-		std::add_const_t<column_type<Column>>* column() const noexcept
+		constexpr std::add_const_t<column_type<Column>>* column() const noexcept
 		{
-			static_assert(static_cast<size_t>(Column) < table_traits::column_count, "column index out of range");
-
-			return soagen::assume_aligned<
-				detail::actual_column_alignment<table_traits, allocator_type, static_cast<size_t>(Column)>>(
-				SOAGEN_LAUNDER(reinterpret_cast<column_type<static_cast<size_t>(Column)>*>(
-					base::alloc_.columns[static_cast<size_t>(Column)])));
+			return const_cast<table&>(*this).template column<static_cast<size_t>(Column)>();
 		}
 
 		/// @}
 	};
 
 	/// @brief True if `T` is an instance of #soagen::table.
 	template <typename>
 	inline constexpr bool is_table = POXY_IMPLEMENTATION_DETAIL(false);
 	/// @cond
-	template <typename... Args>
-	inline constexpr bool is_table<table<Args...>> = true;
+	template <typename Traits, typename Allocator, template <typename> typename Base>
+	inline constexpr bool is_table<table<Traits, Allocator, Base>> = true;
 	template <typename T>
 	inline constexpr bool is_table<const T> = is_table<T>;
 	template <typename T>
 	inline constexpr bool is_table<volatile T> = is_table<T>;
 	template <typename T>
 	inline constexpr bool is_table<const volatile T> = is_table<T>;
 	namespace detail
```

### Comparing `soagen-0.3.0/src/soagen/hpp/table_traits.hpp` & `soagen-0.4.0/src/soagen/hpp/table_traits.hpp`

 * *Files 10% similar despite different names*

```diff
@@ -2,18 +2,16 @@
 //# Copyright (c) Mark Gillard <mark.gillard@outlook.com.au>
 //# See https://github.com/marzer/soagen/blob/master/LICENSE for the full license text.
 //# SPDX-License-Identifier: MIT
 #pragma once
 
 #include "column_traits.hpp"
 #include "row.hpp"
+#include "invoke.hpp"
 #include "header_start.hpp"
-#if SOAGEN_CLANG >= 16
-	#pragma clang diagnostic ignored "-Wunsafe-buffer-usage"
-#endif
 
 /// @cond
 namespace soagen::detail
 {
 	// a base class for the table traits that handles all the non-alignment-dependent stuff -
 	// the 'Columns' argument seen by this class should be the column_base_traits, NOT soagen::column_traits
 	// (to minimize template instantiation explosion)
@@ -45,21 +43,21 @@
 		using const_column_pointers = std::byte* const[column_count];
 
 		static constexpr size_t column_sizes[column_count] = { sizeof(typename Columns::storage_type)... };
 
 		// default constructibility
 
 		static constexpr bool all_default_constructible =
-			(std::is_default_constructible_v<typename Columns::storage_type> && ...);
+			std::conjunction<std::is_default_constructible<typename Columns::storage_type>...>::value;
 
 		static constexpr bool all_nothrow_default_constructible =
-			(std::is_nothrow_default_constructible_v<typename Columns::storage_type> && ...);
+			std::conjunction<std::is_nothrow_default_constructible<typename Columns::storage_type>...>::value;
 
 		static constexpr bool all_trivially_default_constructible =
-			(std::is_trivially_default_constructible_v<typename Columns::storage_type> && ...);
+			std::conjunction<std::is_trivially_default_constructible<typename Columns::storage_type>...>::value;
 
 		// trivial-copyability (memcpy + memmove)
 
 		static constexpr bool all_trivially_copyable = (Columns::is_trivially_copyable && ...);
 
 		static constexpr bool any_trivially_copyable = (false || ... || Columns::is_trivially_copyable);
 
@@ -93,115 +91,114 @@
 
 		static constexpr bool all_nothrow_move_assignable = (Columns::is_nothrow_move_assignable && ...);
 
 		static constexpr bool all_trivially_move_assignable = (Columns::is_trivially_move_assignable && ...);
 
 		// destructibility
 
-		static constexpr bool all_destructible = (std::is_destructible_v<typename Columns::storage_type> && ...);
+		static constexpr bool all_destructible =
+			std::conjunction<std::is_destructible<typename Columns::storage_type>...>::value;
 
 		static constexpr bool all_nothrow_destructible =
-			(std::is_nothrow_destructible_v<typename Columns::storage_type> && ...);
+			std::conjunction<std::is_nothrow_destructible<typename Columns::storage_type>...>::value;
 
 		static constexpr bool all_trivially_destructible =
-			(std::is_trivially_destructible_v<typename Columns::storage_type> && ...);
+			std::conjunction<std::is_trivially_destructible<typename Columns::storage_type>...>::value;
 
 		// swappability
 
 		static constexpr bool all_swappable = (Columns::is_swappable && ...);
 
 		static constexpr bool all_nothrow_swappable = (Columns::is_nothrow_swappable && ...);
 
 		// equality comparability
 
-		static constexpr bool all_equality_comparable = (is_equality_comparable<typename Columns::storage_type> && ...);
+		static constexpr bool all_equality_comparable =
+			std::conjunction<is_equality_comparable_<typename Columns::storage_type>...>::value;
 
 		static constexpr bool all_nothrow_equality_comparable =
-			(is_nothrow_equality_comparable<typename Columns::storage_type> && ...);
+			std::conjunction<is_nothrow_equality_comparable_<typename Columns::storage_type>...>::value;
 
 		// less-than comparability
 
 		static constexpr bool all_less_than_comparable =
-			(is_less_than_comparable<typename Columns::storage_type> && ...);
+			std::conjunction<is_less_than_comparable_<typename Columns::storage_type>...>::value;
 
 		static constexpr bool all_nothrow_less_than_comparable =
-			(is_nothrow_less_than_comparable<typename Columns::storage_type> && ...);
+			std::conjunction<is_nothrow_less_than_comparable_<typename Columns::storage_type>...>::value;
 
 		// row constructibility
 
 	  private:
 		template <size_t, typename...>
 		struct row_constructible_from_tuple_ : std::false_type
 		{};
 		template <typename Tuple, size_t... Members>
 		struct row_constructible_from_tuple_<column_count, Tuple, std::index_sequence<Members...>>
-			: std::bool_constant<(
-				  Columns::template is_constructible<decltype(get_from_tuple_like<Members>(std::declval<Tuple>()))>
-				  && ...)>
+			: std::conjunction<typename Columns::template is_constructible_trait<decltype(get_from_tuple<Members>(
+				  std::declval<Tuple>()))>...>
 		{
 			static_assert(std::is_same_v<std::index_sequence<Members...>, std::make_index_sequence<column_count>>);
 		};
 
 		template <bool, size_t, typename... Args>
 		struct row_constructible_from_ : std::false_type
 		{};
 		template <typename... Args>
 		struct row_constructible_from_<false, column_count, Args...>
-			: std::bool_constant<(Columns::template is_constructible<Args> && ...)>
+			: std::conjunction<typename Columns::template is_constructible_trait<Args>...>
 		{
 			static_assert(sizeof...(Args) == column_count);
 		};
 		template <typename Tuple>
 		struct row_constructible_from_<true, 1, Tuple>
 			: row_constructible_from_tuple_<std::tuple_size_v<remove_cvref<Tuple>>,
 											remove_cvref<Tuple>,
 											std::make_index_sequence<std::tuple_size_v<remove_cvref<Tuple>>>>
 		{};
 
 	  public:
 		template <typename... Args>
 		static constexpr bool row_constructible_from =
-			row_constructible_from_<(is_tuple_like<remove_cvref<Args>> && ...), sizeof...(Args), Args...>::value;
+			row_constructible_from_<(is_tuple<remove_cvref<Args>> && ...), sizeof...(Args), Args...>::value;
 
 		// row constructibility (nothrow)
 
 	  private:
 		template <size_t, typename...>
 		struct row_nothrow_constructible_from_tuple_ : std::false_type
 		{};
 		template <typename Tuple, size_t... Members>
 		struct row_nothrow_constructible_from_tuple_<column_count, Tuple, std::index_sequence<Members...>>
-			: std::bool_constant<(Columns::template is_nothrow_constructible<decltype(get_from_tuple_like<Members>(
-									  std::declval<Tuple>()))>
-								  && ...)>
+			: std::conjunction<typename Columns::template is_nothrow_constructible_trait<
+				  decltype(get_from_tuple<Members>(std::declval<Tuple>()))>...>
 		{
 			static_assert(std::is_same_v<std::index_sequence<Members...>, std::make_index_sequence<column_count>>);
 		};
 
 		template <bool, size_t, typename... Args>
 		struct row_nothrow_constructible_from_ : std::false_type
 		{};
 		template <typename... Args>
 		struct row_nothrow_constructible_from_<false, column_count, Args...>
-			: std::bool_constant<(Columns::template is_nothrow_constructible<Args> && ...)>
+			: std::conjunction<typename Columns::template is_nothrow_constructible_trait<Args>...>
 		{
 			static_assert(sizeof...(Args) == column_count);
 		};
 		template <typename Tuple>
 		struct row_nothrow_constructible_from_<true, 1, Tuple>
 			: row_nothrow_constructible_from_tuple_<std::tuple_size_v<remove_cvref<Tuple>>,
 													remove_cvref<Tuple>,
 													std::make_index_sequence<std::tuple_size_v<remove_cvref<Tuple>>>>
 		{};
 
 	  public:
 		template <typename... Args>
 		static constexpr bool row_nothrow_constructible_from =
-			row_nothrow_constructible_from_<(is_tuple_like<remove_cvref<Args>> && ...), sizeof...(Args), Args...>::
-				value;
+			row_nothrow_constructible_from_<(is_tuple<remove_cvref<Args>> && ...), sizeof...(Args), Args...>::value;
 
 		//--- memmove --------------------------------------------------------------------------------------------------
 
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = all_trivially_copyable)
 		SOAGEN_CPP20_CONSTEXPR
 		static void memmove(column_pointers& dest,
 							size_t dest_start,
@@ -359,36 +356,36 @@
 		}
 
 		//--- construction ---------------------------------------------------------------------------------------------
 
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, typename Tuple, auto sfinae = row_constructible_from<Tuple&&>)
 		SOAGEN_ALWAYS_INLINE
 		SOAGEN_CPP20_CONSTEXPR
-		static void construct_row_from_tuple_like(column_pointers& columns,
-												  size_t index,
-												  Tuple&& tuple) //
+		static void construct_row_from_tuple(column_pointers& columns,
+											 size_t index,
+											 Tuple&& tuple) //
 			noexcept(row_nothrow_constructible_from<Tuple&&>)
 		{
 			static_assert(std::tuple_size_v<remove_cvref<Tuple>> == column_count);
 
-			construct_row(columns, index, get_from_tuple_like<I>(static_cast<Tuple&&>(tuple))...);
+			construct_row(columns, index, get_from_tuple<I>(static_cast<Tuple&&>(tuple))...);
 		}
 
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, typename... Args, auto sfinae = row_constructible_from<Args&&...>)
 		SOAGEN_CPP20_CONSTEXPR
 		static void construct_row(column_pointers& columns, size_t index, Args&&... args) //
 			noexcept(row_nothrow_constructible_from<Args&&...>)
 		{
 			if constexpr (sizeof...(Args) == 0)
 			{
 				default_construct_row(columns, index, static_cast<Args&&>(args)...);
 			}
-			else if constexpr (sizeof...(Args) == 1 && (is_tuple_like<remove_cvref<Args>> && ...))
+			else if constexpr (sizeof...(Args) == 1 && (is_tuple<remove_cvref<Args>> && ...))
 			{
-				construct_row_from_tuple_like(columns, index, static_cast<Args&&>(args)...);
+				construct_row_from_tuple(columns, index, static_cast<Args&&>(args)...);
 			}
 			else
 			{
 				static_assert(sizeof...(Args) == sizeof...(I));
 
 				if constexpr (row_nothrow_constructible_from<Args&&...> || all_trivially_destructible)
 				{
```

### Comparing `soagen-0.3.0/src/soagen/includes.py` & `soagen-0.4.0/src/soagen/includes.py`

 * *Files identical despite different names*

### Comparing `soagen-0.3.0/src/soagen/injectors.py` & `soagen-0.4.0/src/soagen/injectors.py`

 * *Files identical despite different names*

### Comparing `soagen-0.3.0/src/soagen/log.py` & `soagen-0.4.0/src/soagen/log.py`

 * *Files identical despite different names*

### Comparing `soagen-0.3.0/src/soagen/main.py` & `soagen-0.4.0/src/soagen/main.py`

 * *Files identical despite different names*

### Comparing `soagen-0.3.0/src/soagen/metavars.py` & `soagen-0.4.0/src/soagen/metavars.py`

 * *Files identical despite different names*

### Comparing `soagen-0.3.0/src/soagen/natvis_file.py` & `soagen-0.4.0/src/soagen/natvis_file.py`

 * *Files identical despite different names*

### Comparing `soagen-0.3.0/src/soagen/paths.py` & `soagen-0.4.0/src/soagen/paths.py`

 * *Files identical despite different names*

### Comparing `soagen-0.3.0/src/soagen/schemas.py` & `soagen-0.4.0/src/soagen/schemas.py`

 * *Files identical despite different names*

### Comparing `soagen-0.3.0/src/soagen/struct.py` & `soagen-0.4.0/src/soagen/struct.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
         vals = Struct.__schema.validate(vals)
         self.__dict__.update(vals)
 
         self.name = name
         valid = cpp.is_valid_identifier(self.name)
         if not valid[0]:
-            raise SchemaError(rf"name: '{self.name}': {valid[1]}", None)
+            raise SchemaError(rf"name {valid[1]}", None)
         self.type = name
 
         if self.reverse_iterators:
             log.w(rf'{current_schema_context()}reverse_iterators: not currently implemented')
             self.reverse_iterators = False
 
         self.qualified_type = rf'{self.config.namespace}::{self.type}' if self.config.namespace else self.type
@@ -604,19 +604,19 @@
                             return *this;
                         }}
 
                         {doxygen(r"""
                         @brief Erases the row at the given position.
 
                         @availability This method is only available when all the column types are move-assignable.""")}
-                        SOAGEN_HIDDEN(template <bool sfinae = soagen::has_erase_member<table_type, size_type>>)
+                        SOAGEN_HIDDEN(template <bool sfinae = soagen::has_erase_member<table_type>>)
                         SOAGEN_ALWAYS_INLINE
                         SOAGEN_CPP20_CONSTEXPR
                         SOAGEN_ENABLE_IF_T({self.name}&, sfinae) erase(size_type pos) //
-                            noexcept(soagen::has_nothrow_erase_member<table_type, size_type>)
+                            noexcept(soagen::has_nothrow_erase_member<table_type>)
                         {{
                             table_.erase(pos);
                             return *this;
                         }}
 
                         {doxygen(r"""
                         @brief	Erases the row at the given position without preserving order.
@@ -627,19 +627,19 @@
 
                         @note		If you are tracking row indices in some other place and need to maintain that invariant,
                                     you can use the return value to update your data accordingly.
 
                         @returns	The position of the row that was moved into the erased row's position, if any.
 
                         @availability This method is only available when all the column types are move-assignable.""")}
-                        SOAGEN_HIDDEN(template <bool sfinae = soagen::has_unordered_erase_member<table_type, size_type>>)
+                        SOAGEN_HIDDEN(template <bool sfinae = soagen::has_unordered_erase_member<table_type>>)
                         SOAGEN_ALWAYS_INLINE
                         SOAGEN_CPP20_CONSTEXPR
                         SOAGEN_ENABLE_IF_T(soagen::optional<size_type>, sfinae) unordered_erase(size_type pos) //
-                            noexcept(soagen::has_nothrow_unordered_erase_member<table_type, size_type>)
+                            noexcept(soagen::has_nothrow_unordered_erase_member<table_type>)
                         {{
                             return table_.unordered_erase(pos);
                         }}
                         '''
                         )
 
                         if self.iterators:
@@ -649,19 +649,19 @@
                                     {doxygen(rf"""
                                     @brief Erases the row at the given iterator.
 
                                     @returns    An iterator to the row immediately following the one which was removed,
                                                 or #{"c" if const else ""}end() if the one removed was the last row in the table.
 
                                     @availability This method is only available when all the column types are move-assignable.""")}
-                                    SOAGEN_HIDDEN(template <bool sfinae = soagen::has_erase_member<table_type, size_type>>)
+                                    SOAGEN_HIDDEN(template <bool sfinae = soagen::has_erase_member<table_type>>)
                                     SOAGEN_ALWAYS_INLINE
                                     SOAGEN_CPP20_CONSTEXPR
                                     SOAGEN_ENABLE_IF_T({const}iterator, sfinae) erase({const}iterator pos) //
-                                        noexcept(soagen::has_nothrow_erase_member<table_type, size_type>)
+                                        noexcept(soagen::has_nothrow_erase_member<table_type>)
                                     {{
                                         table_.erase(static_cast<size_type>(pos));
                                         return pos;
                                     }}
 
                                     {doxygen(r"""
                                     @brief	Erases the row at the given position without preserving order.
@@ -672,19 +672,19 @@
 
                                     @note		If you are tracking row indices in some other place and need to maintain that invariant,
                                                 you can use the return value to update your data accordingly.
 
                                     @returns	The position of the row that was moved into the erased row's position, if any.
 
                                     @availability This method is only available when all the column types are move-assignable.""")}
-                                    SOAGEN_HIDDEN(template <bool sfinae = soagen::has_unordered_erase_member<table_type, size_type>>)
+                                    SOAGEN_HIDDEN(template <bool sfinae = soagen::has_unordered_erase_member<table_type>>)
                                     SOAGEN_ALWAYS_INLINE
                                     SOAGEN_CPP20_CONSTEXPR
                                     SOAGEN_ENABLE_IF_T(soagen::optional<{const}iterator>, sfinae) unordered_erase({const}iterator pos) //
-                                        noexcept(soagen::has_nothrow_unordered_erase_member<table_type, size_type>)
+                                        noexcept(soagen::has_nothrow_unordered_erase_member<table_type>)
                                     {{
                                         if (auto moved_pos = table_.unordered_erase(static_cast<size_type>(pos)); moved_pos)
                                             return {const}iterator{{ *this, static_cast<difference_type>(*moved_pos) }};
                                         return {{}};
                                     }}
 
 
@@ -722,15 +722,15 @@
                         #if SOAGEN_DOXYGEN
 
                         {doxygen(r"""
                         @brief Resizes the table to the given number of rows.
 
                         @availability This method is only available when all the column types are default-constructible.""")}
                         {self.name}& resize(size_type new_size) //
-                            noexcept(soagen::has_nothrow_resize_member<table_type, size_type>);
+                            noexcept(soagen::has_nothrow_resize_member<table_type>);
 
                         '''
                         )
 
                         if self.swappable:
                             o(
                                 rf'''
@@ -841,14 +841,19 @@
                                                 sfinae.append(r'table_traits::row_constructible_from<Tuple&&>')
                                                 sfinae_template_dependent = True
                                             if rvalue_overload:
                                                 sfinae.append(r'table_traits::rvalue_type_list_is_distinct')
                                             if func in (r'insert', r'emplace'):
                                                 sfinae.append(r'table_traits::all_move_constructible')
                                                 sfinae.append(r'table_traits::all_move_assignable')
+                                            if func in (r'emplace_back', r'emplace'):
+                                                sfinae.append(
+                                                    rf'table_traits::row_constructible_from<{",".join(types[-len(self.columns):])}>'
+                                                )
+                                                sfinae_template_dependent = True
                                             hidden_template = bool(sfinae) and not template_params
                                             if sfinae:
                                                 if len(sfinae) > 2:
                                                     sfinae_condition_string = f'\n{o.indent_str*7}&& '.join(sfinae)
                                                 else:
                                                     sfinae_condition_string = r' && '.join(sfinae)
                                                 if len(sfinae) >= 2:
```

### Comparing `soagen-0.3.0/src/soagen/type_list.py` & `soagen-0.4.0/src/soagen/type_list.py`

 * *Files identical despite different names*

### Comparing `soagen-0.3.0/src/soagen/utils.py` & `soagen-0.4.0/src/soagen/utils.py`

 * *Files identical despite different names*

### Comparing `soagen-0.3.0/src/soagen/variable.py` & `soagen-0.4.0/src/soagen/variable.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         self.index = -1  # set by the struct
 
         vals = Variable.__schema.validate(vals)
         self.__dict__.update(vals)
 
         valid = cpp.is_valid_identifier(self.name)
         if not valid[0]:
-            raise SchemaError(rf"name: '{self.name}': {valid[1]}", None)
+            raise SchemaError(rf"name {valid[1]}", None)
 
         if self.default is None:
             self.default = ''
 
         self.pointer_type = rf'{self.type}*'
         if re.fullmatch(r'[a-zA-Z_][a-zA-Z_0-9:]*', self.type):
             self.const_pointer_type = rf'const {self.pointer_type}'
@@ -69,15 +69,15 @@
 
     def __init__(self, cfg, vals):
         super().__init__(cfg)
         self.__dict__.update(StaticVariable.__schema.validate(vals))
 
         valid = cpp.is_valid_identifier(self.name)
         if not valid[0]:
-            raise SchemaError(rf"name: '{self.name}': {valid[1]}", None)
+            raise SchemaError(rf"name {valid[1]}", None)
 
         if not self.value:
             raise SchemaError(rf"value: cannot be blank", None)
 
         if self.const is None:
             self.const = 'constexpr'
         elif isinstance(self.const, bool):
```

### Comparing `soagen-0.3.0/src/soagen/version.py` & `soagen-0.4.0/src/soagen/version.py`

 * *Files identical despite different names*

### Comparing `soagen-0.3.0/src/soagen/writer.py` & `soagen-0.4.0/src/soagen/writer.py`

 * *Files identical despite different names*

### Comparing `soagen-0.3.0/src/soagen.egg-info/PKG-INFO` & `soagen-0.4.0/src/soagen.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soagen
-Version: 0.3.0
+Version: 0.4.0
 Summary: Struct-of-Arrays generator for C++ projects.
 Author-email: Mark Gillard <mark.gillard@outlook.com.au>
 License: MIT
 Project-URL: Source, https://github.com/marzer/soagen
 Project-URL: Tracker, https://github.com/marzer/soagen/issues
 Project-URL: Funding, https://github.com/sponsors/marzer
 Keywords: c++,soa,struct-of-arrays,structure-of-arrays,struct of arrays,structure of arrays,parallel-arrays,parallel arrays,std::vector
@@ -33,14 +33,23 @@
 <br><br>
 
 [gitter]: https://gitter.im/marzer/community
 [sponsor]: https://github.com/sponsors/marzer
 
 # Changelog
 
+## v0.4.0
+
+-   Fixed `soagen::is_table<>`
+-   Added support for emplace-constructing column values by unpacking all `std::tuple`-like types (not just the `emplacer`)
+-   Added support for taking `std::integral_constants` in `for_each_column()`
+-   Added `soagen::same_table_type<>`
+-   Added conversions between `soagen::row<>` specializations
+-   Optimized instantiation overhead for most type-traits
+
 ## v0.3.0
 
 -   Added `hpp.combined`
 -   Added `std::integral_constant<size_t>` to the overload set used by `for_each_column()`
 -   Added support for constructing rows from all `std::tuple`-like types
 -   Optimized bulk-swap operations
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: soagen Version: 0.3.0 Summary: Struct-of-Arrays
+Metadata-Version: 2.1 Name: soagen Version: 0.4.0 Summary: Struct-of-Arrays
 generator for C++ projects. Author-email: Mark Gillard
 gillard@outlook.com.au> License: MIT Project-URL: Source, https://github.com/
 marzer/soagen Project-URL: Tracker, https://github.com/marzer/soagen/issues
 Project-URL: Funding, https://github.com/sponsors/marzer Keywords:
 c++,soa,struct-of-arrays,structure-of-arrays,struct of arrays,structure of
 arrays,parallel-arrays,parallel arrays,std::vector Classifier: Development
 Status :: 3 - Alpha Classifier: License :: OSI Approved :: MIT License
@@ -13,17 +13,22 @@
 badge-sponsor.svg)][sponsor] [![Gitter](docs/images/badge-gitter.svg)][gitter]
 
      â¨&#xFE0F; This README is a stub. Please see the HTML documentation:
                       marzer.github.io/soagenâ¨&#xFE0F;
 
 
 [gitter]: https://gitter.im/marzer/community [sponsor]: https://github.com/
-sponsors/marzer # Changelog ## v0.3.0 - Added `hpp.combined` - Added `std::
-integral_constant` to the overload set used by `for_each_column()` - Added
-support for constructing rows from all `std::tuple`-like types - Optimized
-bulk-swap operations ## v0.2.0 - Added `structs.annotations` - Added
+sponsors/marzer # Changelog ## v0.4.0 - Fixed `soagen::is_table<>` - Added
+support for emplace-constructing column values by unpacking all `std::tuple`-
+like types (not just the `emplacer`) - Added support for taking `std::
+integral_constants` in `for_each_column()` - Added `soagen::same_table_type<>`
+- Added conversions between `soagen::row<>` specializations - Optimized
+instantiation overhead for most type-traits ## v0.3.0 - Added `hpp.combined` -
+Added `std::integral_constant` to the overload set used by `for_each_column()`
+- Added support for constructing rows from all `std::tuple`-like types -
+Optimized bulk-swap operations ## v0.2.0 - Added `structs.annotations` - Added
 `structs.attributes` - Added `auto` option for `structs.default_constructible`
 - Added `soagen::row_base` - Added `soagen::table_base` - Added `soagen::
 iterator_base` - Added `Base` template argument to `soagen::table` for CRTP -
 Added `swap_columns<>()` - Made `column_indices` member struct into `enum class
 columns` ## v0.1.2 - Minor refactors. ## v0.1.1 - Minor refactors. ## v0.1.0 -
 First public release ð&#xFE0F;
```

### Comparing `soagen-0.3.0/src/soagen.egg-info/SOURCES.txt` & `soagen-0.4.0/src/soagen.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -33,20 +33,23 @@
 src/soagen.egg-info/requires.txt
 src/soagen.egg-info/top_level.txt
 src/soagen.egg-info/zip-safe
 src/soagen/hpp/.clang-format
 src/soagen/hpp/allocator.hpp
 src/soagen/hpp/column_traits.hpp
 src/soagen/hpp/core.hpp
+src/soagen/hpp/emplacer.hpp
 src/soagen/hpp/header_end.hpp
 src/soagen/hpp/header_start.hpp
+src/soagen/hpp/invoke.hpp
 src/soagen/hpp/iterator.hpp
 src/soagen/hpp/mixins.hpp
 src/soagen/hpp/row.hpp
 src/soagen/hpp/soagen.hpp
 src/soagen/hpp/table.hpp
 src/soagen/hpp/table_traits.hpp
+src/soagen/hpp/tuples.hpp
 src/soagen/hpp/generated/compressed_pair.hpp
 src/soagen/hpp/generated/functions.hpp
 src/soagen/hpp/generated/preprocessor.hpp
 src/soagen/hpp/generated/version.hpp
 src/soagen/hpp/single/soagen.hpp
```

