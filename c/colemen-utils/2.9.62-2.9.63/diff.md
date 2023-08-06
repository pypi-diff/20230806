# Comparing `tmp/colemen_utils-2.9.62.tar.gz` & `tmp/colemen_utils-2.9.63.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colemen_utils-2.9.62.tar", last modified: Wed Dec 14 20:09:45 2022, max compression
+gzip compressed data, was "colemen_utils-2.9.63.tar", last modified: Wed Dec 14 20:12:55 2022, max compression
```

## Comparing `colemen_utils-2.9.62.tar` & `colemen_utils-2.9.63.tar`

### file list

```diff
@@ -1,107 +1,108 @@
-drwxrwxrwx   0        0        0        0 2022-12-14 20:09:45.941861 colemen_utils-2.9.62/
--rw-rw-rw-   0        0        0      522 2022-12-14 20:09:45.940861 colemen_utils-2.9.62/PKG-INFO
--rw-rw-rw-   0        0        0     6350 2022-12-14 17:11:51.000000 colemen_utils-2.9.62/colemen_config.py
-drwxrwxrwx   0        0        0        0 2022-12-14 20:09:45.848861 colemen_utils-2.9.62/colemen_utilities/
-drwxrwxrwx   0        0        0        0 2022-12-14 20:09:45.850863 colemen_utils-2.9.62/colemen_utilities/console_utils/
--rw-rw-rw-   0        0        0      987 2022-08-08 17:30:21.000000 colemen_utils-2.9.62/colemen_utilities/console_utils/__init__.py
--rw-rw-rw-   0        0        0     6231 2022-12-07 18:30:59.000000 colemen_utils-2.9.62/colemen_utilities/console_utils/print.py
-drwxrwxrwx   0        0        0        0 2022-12-14 20:09:45.854862 colemen_utils-2.9.62/colemen_utilities/database_utils/
--rw-rw-rw-   0        0        0    83866 2022-12-12 19:18:38.000000 colemen_utils-2.9.62/colemen_utilities/database_utils/DatabaseManager.py
-drwxrwxrwx   0        0        0        0 2022-12-14 20:09:45.862862 colemen_utils-2.9.62/colemen_utilities/database_utils/MySQL/
--rw-rw-rw-   0        0        0     9434 2022-12-12 17:33:07.000000 colemen_utils-2.9.62/colemen_utilities/database_utils/MySQL/CacheFile.py
-drwxrwxrwx   0        0        0        0 2022-12-14 20:09:45.866867 colemen_utils-2.9.62/colemen_utilities/database_utils/MySQL/Column/
--rw-rw-rw-   0        0        0    30265 2022-12-14 15:32:52.000000 colemen_utils-2.9.62/colemen_utilities/database_utils/MySQL/Column/Column.py
--rw-rw-rw-   0        0        0      307 2022-12-12 19:20:38.000000 colemen_utils-2.9.62/colemen_utilities/database_utils/MySQL/Column/__init__.py
--rw-rw-rw-   0        0        0     3134 2022-12-14 15:24:31.000000 colemen_utils-2.9.62/colemen_utilities/database_utils/MySQL/Column/column_utils.py
--rw-rw-rw-   0        0        0     3141 2022-12-14 20:00:13.000000 colemen_utils-2.9.62/colemen_utilities/database_utils/MySQL/DeleteQuery.py
--rw-rw-rw-   0        0        0    51931 2022-12-14 19:59:56.000000 colemen_utils-2.9.62/colemen_utilities/database_utils/MySQL/MySQLDatabase.py
--rw-rw-rw-   0        0        0    15870 2022-12-14 20:08:00.000000 colemen_utils-2.9.62/colemen_utilities/database_utils/MySQL/QueryBase.py
--rw-rw-rw-   0        0        0    16602 2022-12-14 19:52:54.000000 colemen_utils-2.9.62/colemen_utilities/database_utils/MySQL/SelectQuery.py
-drwxrwxrwx   0        0        0        0 2022-12-14 20:09:45.868862 colemen_utils-2.9.62/colemen_utilities/database_utils/MySQL/Table/
--rw-rw-rw-   0        0        0    23081 2022-12-14 19:38:50.000000 colemen_utils-2.9.62/colemen_utilities/database_utils/MySQL/Table/Table.py
--rw-rw-rw-   0        0        0      301 2022-12-13 18:25:40.000000 colemen_utils-2.9.62/colemen_utilities/database_utils/MySQL/Table/__init__.py
--rw-rw-rw-   0        0        0     5765 2022-12-14 19:26:56.000000 colemen_utils-2.9.62/colemen_utilities/database_utils/MySQL/UpdateQuery.py
--rw-rw-rw-   0        0        0     1170 2022-12-13 18:26:22.000000 colemen_utils-2.9.62/colemen_utilities/database_utils/MySQL/__init__.py
--rw-rw-rw-   0        0        0    24755 2022-08-16 16:00:24.000000 colemen_utils-2.9.62/colemen_utilities/database_utils/TableDataManager.py
--rw-rw-rw-   0        0        0    51813 2022-08-16 15:59:58.000000 colemen_utils-2.9.62/colemen_utilities/database_utils/TableManager.py
--rw-rw-rw-   0        0        0     1168 2022-12-13 18:22:22.000000 colemen_utils-2.9.62/colemen_utilities/database_utils/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-14 20:09:45.875862 colemen_utils-2.9.62/colemen_utilities/database_utils/drawio/
--rw-rw-rw-   0        0        0    16961 2022-08-08 17:33:54.000000 colemen_utils-2.9.62/colemen_utilities/database_utils/drawio/ForeignKey.py
--rw-rw-rw-   0        0        0    21691 2022-08-08 17:33:54.000000 colemen_utils-2.9.62/colemen_utilities/database_utils/drawio/Parser.py
--rw-rw-rw-   0        0        0    31046 2022-08-08 17:33:54.000000 colemen_utils-2.9.62/colemen_utilities/database_utils/drawio/Row.py
--rw-rw-rw-   0        0        0     4740 2022-08-08 17:33:54.000000 colemen_utils-2.9.62/colemen_utilities/database_utils/drawio/Schema.py
--rw-rw-rw-   0        0        0    28804 2022-08-08 17:33:54.000000 colemen_utils-2.9.62/colemen_utilities/database_utils/drawio/Table.py
--rw-rw-rw-   0        0        0       71 2022-08-08 17:30:21.000000 colemen_utils-2.9.62/colemen_utilities/database_utils/drawio/__init__.py
--rw-rw-rw-   0        0        0     8434 2022-08-08 17:33:54.000000 colemen_utils-2.9.62/colemen_utilities/database_utils/drawio/entity_utils.py
-drwxrwxrwx   0        0        0        0 2022-12-14 20:09:45.877862 colemen_utils-2.9.62/colemen_utilities/dict_utils/
--rw-rw-rw-   0        0        0      557 2022-08-08 17:30:21.000000 colemen_utils-2.9.62/colemen_utilities/dict_utils/__init__.py
--rw-rw-rw-   0        0        0    25194 2022-12-14 15:06:08.000000 colemen_utils-2.9.62/colemen_utilities/dict_utils/dict_utils.py
-drwxrwxrwx   0        0        0        0 2022-12-14 20:09:45.885863 colemen_utils-2.9.62/colemen_utilities/directory_utils/
--rw-rw-rw-   0        0        0     1160 2022-08-08 17:30:21.000000 colemen_utils-2.9.62/colemen_utilities/directory_utils/__init__.py
--rw-rw-rw-   0        0        0    30357 2022-08-08 17:30:21.000000 colemen_utils-2.9.62/colemen_utilities/directory_utils/dir.py
--rw-rw-rw-   0        0        0     2136 2022-08-08 17:30:21.000000 colemen_utils-2.9.62/colemen_utilities/directory_utils/dir_compression.py
--rw-rw-rw-   0        0        0    15095 2022-08-08 17:30:21.000000 colemen_utils-2.9.62/colemen_utilities/directory_utils/dir_create.py
--rw-rw-rw-   0        0        0     3454 2022-08-08 17:30:21.000000 colemen_utils-2.9.62/colemen_utilities/directory_utils/dir_delete.py
--rw-rw-rw-   0        0        0    12180 2022-08-08 17:30:21.000000 colemen_utils-2.9.62/colemen_utilities/directory_utils/dir_read.py
--rw-rw-rw-   0        0        0     3692 2022-08-08 17:30:21.000000 colemen_utils-2.9.62/colemen_utilities/directory_utils/dir_search.py
-drwxrwxrwx   0        0        0        0 2022-12-14 20:09:45.895862 colemen_utils-2.9.62/colemen_utilities/drawio/
--rw-rw-rw-   0        0        0     4203 2022-08-08 17:33:54.000000 colemen_utils-2.9.62/colemen_utilities/drawio/Connector.py
--rw-rw-rw-   0        0        0    16617 2022-08-08 17:33:54.000000 colemen_utils-2.9.62/colemen_utilities/drawio/Diagram.py
--rw-rw-rw-   0        0        0    10045 2022-08-08 17:33:54.000000 colemen_utils-2.9.62/colemen_utilities/drawio/Drawing.py
--rw-rw-rw-   0        0        0     6189 2022-08-08 17:33:54.000000 colemen_utils-2.9.62/colemen_utilities/drawio/Mxcell.py
--rw-rw-rw-   0        0        0    35265 2022-08-08 17:33:54.000000 colemen_utils-2.9.62/colemen_utilities/drawio/NodeBase.py
--rw-rw-rw-   0        0        0    13812 2022-08-08 17:33:54.000000 colemen_utils-2.9.62/colemen_utilities/drawio/Onode.py
--rw-rw-rw-   0        0        0      277 2022-08-08 17:30:21.000000 colemen_utils-2.9.62/colemen_utilities/drawio/__init__.py
--rw-rw-rw-   0        0        0     4545 2022-08-08 17:33:54.000000 colemen_utils-2.9.62/colemen_utilities/drawio/diagram_utils.py
--rw-rw-rw-   0        0        0    32154 2022-08-08 17:33:54.000000 colemen_utils-2.9.62/colemen_utilities/drawio/nodes.py
-drwxrwxrwx   0        0        0        0 2022-12-14 20:09:45.909862 colemen_utils-2.9.62/colemen_utilities/file_utils/
--rw-rw-rw-   0        0        0    14264 2022-08-15 15:05:17.000000 colemen_utils-2.9.62/colemen_utilities/file_utils/File.py
--rw-rw-rw-   0        0        0     2057 2022-08-15 15:05:38.000000 colemen_utils-2.9.62/colemen_utilities/file_utils/__init__.py
--rw-rw-rw-   0        0        0    27148 2022-01-26 22:09:44.000000 colemen_utils-2.9.62/colemen_utilities/file_utils/exiftool.py
--rw-rw-rw-   0        0        0     8353 2022-08-08 17:30:21.000000 colemen_utils-2.9.62/colemen_utilities/file_utils/file_compression.py
--rw-rw-rw-   0        0        0    12456 2022-08-08 17:30:22.000000 colemen_utils-2.9.62/colemen_utilities/file_utils/file_convert.py
--rw-rw-rw-   0        0        0    32721 2022-08-08 17:30:22.000000 colemen_utils-2.9.62/colemen_utilities/file_utils/file_image.py
--rw-rw-rw-   0        0        0     6630 2022-08-15 14:48:40.000000 colemen_utils-2.9.62/colemen_utilities/file_utils/file_read.py
--rw-rw-rw-   0        0        0     3939 2022-08-08 17:30:21.000000 colemen_utils-2.9.62/colemen_utilities/file_utils/file_search.py
--rw-rw-rw-   0        0        0      312 2022-08-08 17:30:21.000000 colemen_utils-2.9.62/colemen_utilities/file_utils/file_string_facade.py
--rw-rw-rw-   0        0        0    69198 2022-08-15 14:01:01.000000 colemen_utils-2.9.62/colemen_utilities/file_utils/file_utils.py
--rw-rw-rw-   0        0        0     2208 2022-08-08 17:30:21.000000 colemen_utils-2.9.62/colemen_utilities/file_utils/file_write.py
--rw-rw-rw-   0        0        0      279 2022-06-04 17:28:32.000000 colemen_utils-2.9.62/colemen_utilities/file_utils/resources.py
-drwxrwxrwx   0        0        0        0 2022-12-14 20:09:45.910862 colemen_utils-2.9.62/colemen_utilities/list_utils/
--rw-rw-rw-   0        0        0      589 2022-08-08 17:30:21.000000 colemen_utils-2.9.62/colemen_utilities/list_utils/__init__.py
--rw-rw-rw-   0        0        0     7801 2022-08-31 14:13:14.000000 colemen_utils-2.9.62/colemen_utilities/list_utils/list_utils.py
--rw-rw-rw-   0        0        0        0 2022-12-06 14:26:55.000000 colemen_utils-2.9.62/colemen_utilities/parse_sql.py
--rw-rw-rw-   0        0        0        0 2022-06-04 20:21:34.000000 colemen_utils-2.9.62/colemen_utilities/parse_utils.py
-drwxrwxrwx   0        0        0        0 2022-12-14 20:09:45.914863 colemen_utils-2.9.62/colemen_utilities/random_utils/
--rw-rw-rw-   0        0        0      901 2022-08-08 17:30:21.000000 colemen_utils-2.9.62/colemen_utilities/random_utils/__init__.py
--rw-rw-rw-   0        0        0    29815 2022-08-08 17:50:08.000000 colemen_utils-2.9.62/colemen_utilities/random_utils/rand_generation.py
--rw-rw-rw-   0        0        0     6603 2022-08-08 17:30:21.000000 colemen_utils-2.9.62/colemen_utilities/random_utils/rand_utils.py
-drwxrwxrwx   0        0        0        0 2022-12-14 20:09:45.918862 colemen_utils-2.9.62/colemen_utilities/sql_utils/
--rw-rw-rw-   0        0        0      626 2022-08-08 17:30:21.000000 colemen_utils-2.9.62/colemen_utilities/sql_utils/__init__.py
--rw-rw-rw-   0        0        0     7618 2022-08-08 17:30:21.000000 colemen_utils-2.9.62/colemen_utilities/sql_utils/sql_format.py
--rw-rw-rw-   0        0        0    46142 2022-12-13 18:59:34.000000 colemen_utils-2.9.62/colemen_utilities/sql_utils/sql_parse.py
--rw-rw-rw-   0        0        0    58169 2022-12-09 21:39:20.000000 colemen_utils-2.9.62/colemen_utilities/sql_utils/sql_utils.py
-drwxrwxrwx   0        0        0        0 2022-12-14 20:09:45.926862 colemen_utils-2.9.62/colemen_utilities/string_utils/
--rw-rw-rw-   0        0        0     1295 2022-08-08 17:30:21.000000 colemen_utils-2.9.62/colemen_utilities/string_utils/__init__.py
--rw-rw-rw-   0        0        0     6436 2022-08-08 17:30:21.000000 colemen_utils-2.9.62/colemen_utilities/string_utils/string_conversion.py
--rw-rw-rw-   0        0        0    17480 2022-12-14 19:58:02.000000 colemen_utils-2.9.62/colemen_utilities/string_utils/string_escaping.py
--rw-rw-rw-   0        0        0    29280 2022-11-29 17:06:13.000000 colemen_utils-2.9.62/colemen_utilities/string_utils/string_format.py
--rw-rw-rw-   0        0        0    10123 2022-08-08 17:30:21.000000 colemen_utils-2.9.62/colemen_utilities/string_utils/string_generation.py
--rw-rw-rw-   0        0        0     3635 2022-08-08 17:30:21.000000 colemen_utils-2.9.62/colemen_utilities/string_utils/string_parsing.py
--rw-rw-rw-   0        0        0     5497 2022-08-08 17:30:21.000000 colemen_utils-2.9.62/colemen_utilities/string_utils/string_strip.py
-drwxrwxrwx   0        0        0        0 2022-12-14 20:09:45.927861 colemen_utils-2.9.62/colemen_utilities/type_utils/
--rw-rw-rw-   0        0        0      528 2022-08-08 17:30:21.000000 colemen_utils-2.9.62/colemen_utilities/type_utils/__init__.py
--rw-rw-rw-   0        0        0     9173 2022-12-06 15:07:15.000000 colemen_utils-2.9.62/colemen_utilities/type_utils/type_utils.py
-drwxrwxrwx   0        0        0        0 2022-12-14 20:09:45.931863 colemen_utils-2.9.62/colemen_utilities/validate_utils/
--rw-rw-rw-   0        0        0      626 2022-12-09 19:06:02.000000 colemen_utils-2.9.62/colemen_utilities/validate_utils/__init__.py
--rw-rw-rw-   0        0        0     3902 2022-12-12 21:22:26.000000 colemen_utils-2.9.62/colemen_utilities/validate_utils/cerberus.py
--rw-rw-rw-   0        0        0     2950 2022-12-09 20:45:04.000000 colemen_utils-2.9.62/colemen_utilities/validate_utils/general.py
-drwxrwxrwx   0        0        0        0 2022-12-14 20:09:45.939861 colemen_utils-2.9.62/colemen_utils.egg-info/
--rw-rw-rw-   0        0        0      522 2022-12-14 20:09:45.000000 colemen_utils-2.9.62/colemen_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3802 2022-12-14 20:09:45.000000 colemen_utils-2.9.62/colemen_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-14 20:09:45.000000 colemen_utils-2.9.62/colemen_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      152 2022-12-14 20:09:45.000000 colemen_utils-2.9.62/colemen_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       47 2022-12-14 20:09:45.000000 colemen_utils-2.9.62/colemen_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      920 2022-12-09 18:54:19.000000 colemen_utils-2.9.62/colemen_utils.py
--rw-rw-rw-   0        0        0       42 2022-12-14 20:09:45.941861 colemen_utils-2.9.62/setup.cfg
--rw-rw-rw-   0        0        0     5576 2022-12-14 20:09:23.000000 colemen_utils-2.9.62/setup.py
+drwxrwxrwx   0        0        0        0 2022-12-14 20:12:55.982559 colemen_utils-2.9.63/
+-rw-rw-rw-   0        0        0      522 2022-12-14 20:12:55.982559 colemen_utils-2.9.63/PKG-INFO
+-rw-rw-rw-   0        0        0     6350 2022-12-14 17:11:51.000000 colemen_utils-2.9.63/colemen_config.py
+drwxrwxrwx   0        0        0        0 2022-12-14 20:12:55.843531 colemen_utils-2.9.63/colemen_utilities/
+drwxrwxrwx   0        0        0        0 2022-12-14 20:12:55.845528 colemen_utils-2.9.63/colemen_utilities/console_utils/
+-rw-rw-rw-   0        0        0      987 2022-08-08 17:30:21.000000 colemen_utils-2.9.63/colemen_utilities/console_utils/__init__.py
+-rw-rw-rw-   0        0        0     6231 2022-12-07 18:30:59.000000 colemen_utils-2.9.63/colemen_utilities/console_utils/print.py
+drwxrwxrwx   0        0        0        0 2022-12-14 20:12:55.849529 colemen_utils-2.9.63/colemen_utilities/database_utils/
+-rw-rw-rw-   0        0        0    83866 2022-12-12 19:18:38.000000 colemen_utils-2.9.63/colemen_utilities/database_utils/DatabaseManager.py
+drwxrwxrwx   0        0        0        0 2022-12-14 20:12:55.858530 colemen_utils-2.9.63/colemen_utilities/database_utils/MySQL/
+-rw-rw-rw-   0        0        0     9434 2022-12-12 17:33:07.000000 colemen_utils-2.9.63/colemen_utilities/database_utils/MySQL/CacheFile.py
+drwxrwxrwx   0        0        0        0 2022-12-14 20:12:55.862531 colemen_utils-2.9.63/colemen_utilities/database_utils/MySQL/Column/
+-rw-rw-rw-   0        0        0    30265 2022-12-14 15:32:52.000000 colemen_utils-2.9.63/colemen_utilities/database_utils/MySQL/Column/Column.py
+-rw-rw-rw-   0        0        0      307 2022-12-12 19:20:38.000000 colemen_utils-2.9.63/colemen_utilities/database_utils/MySQL/Column/__init__.py
+-rw-rw-rw-   0        0        0     3134 2022-12-14 15:24:31.000000 colemen_utils-2.9.63/colemen_utilities/database_utils/MySQL/Column/column_utils.py
+-rw-rw-rw-   0        0        0     3141 2022-12-14 20:00:13.000000 colemen_utils-2.9.63/colemen_utilities/database_utils/MySQL/DeleteQuery.py
+-rw-rw-rw-   0        0        0     7818 2022-12-14 19:47:39.000000 colemen_utils-2.9.63/colemen_utilities/database_utils/MySQL/InsertQuery.py
+-rw-rw-rw-   0        0        0    51931 2022-12-14 19:59:56.000000 colemen_utils-2.9.63/colemen_utilities/database_utils/MySQL/MySQLDatabase.py
+-rw-rw-rw-   0        0        0    15870 2022-12-14 20:08:00.000000 colemen_utils-2.9.63/colemen_utilities/database_utils/MySQL/QueryBase.py
+-rw-rw-rw-   0        0        0    16602 2022-12-14 19:52:54.000000 colemen_utils-2.9.63/colemen_utilities/database_utils/MySQL/SelectQuery.py
+drwxrwxrwx   0        0        0        0 2022-12-14 20:12:55.864529 colemen_utils-2.9.63/colemen_utilities/database_utils/MySQL/Table/
+-rw-rw-rw-   0        0        0    23081 2022-12-14 19:38:50.000000 colemen_utils-2.9.63/colemen_utilities/database_utils/MySQL/Table/Table.py
+-rw-rw-rw-   0        0        0      301 2022-12-13 18:25:40.000000 colemen_utils-2.9.63/colemen_utilities/database_utils/MySQL/Table/__init__.py
+-rw-rw-rw-   0        0        0     5765 2022-12-14 19:26:56.000000 colemen_utils-2.9.63/colemen_utilities/database_utils/MySQL/UpdateQuery.py
+-rw-rw-rw-   0        0        0     1170 2022-12-13 18:26:22.000000 colemen_utils-2.9.63/colemen_utilities/database_utils/MySQL/__init__.py
+-rw-rw-rw-   0        0        0    24755 2022-08-16 16:00:24.000000 colemen_utils-2.9.63/colemen_utilities/database_utils/TableDataManager.py
+-rw-rw-rw-   0        0        0    51813 2022-08-16 15:59:58.000000 colemen_utils-2.9.63/colemen_utilities/database_utils/TableManager.py
+-rw-rw-rw-   0        0        0     1168 2022-12-13 18:22:22.000000 colemen_utils-2.9.63/colemen_utilities/database_utils/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-14 20:12:55.872529 colemen_utils-2.9.63/colemen_utilities/database_utils/drawio/
+-rw-rw-rw-   0        0        0    16961 2022-08-08 17:33:54.000000 colemen_utils-2.9.63/colemen_utilities/database_utils/drawio/ForeignKey.py
+-rw-rw-rw-   0        0        0    21691 2022-08-08 17:33:54.000000 colemen_utils-2.9.63/colemen_utilities/database_utils/drawio/Parser.py
+-rw-rw-rw-   0        0        0    31046 2022-08-08 17:33:54.000000 colemen_utils-2.9.63/colemen_utilities/database_utils/drawio/Row.py
+-rw-rw-rw-   0        0        0     4740 2022-08-08 17:33:54.000000 colemen_utils-2.9.63/colemen_utilities/database_utils/drawio/Schema.py
+-rw-rw-rw-   0        0        0    28804 2022-08-08 17:33:54.000000 colemen_utils-2.9.63/colemen_utilities/database_utils/drawio/Table.py
+-rw-rw-rw-   0        0        0       71 2022-08-08 17:30:21.000000 colemen_utils-2.9.63/colemen_utilities/database_utils/drawio/__init__.py
+-rw-rw-rw-   0        0        0     8434 2022-08-08 17:33:54.000000 colemen_utils-2.9.63/colemen_utilities/database_utils/drawio/entity_utils.py
+drwxrwxrwx   0        0        0        0 2022-12-14 20:12:55.874528 colemen_utils-2.9.63/colemen_utilities/dict_utils/
+-rw-rw-rw-   0        0        0      557 2022-08-08 17:30:21.000000 colemen_utils-2.9.63/colemen_utilities/dict_utils/__init__.py
+-rw-rw-rw-   0        0        0    25194 2022-12-14 15:06:08.000000 colemen_utils-2.9.63/colemen_utilities/dict_utils/dict_utils.py
+drwxrwxrwx   0        0        0        0 2022-12-14 20:12:55.890528 colemen_utils-2.9.63/colemen_utilities/directory_utils/
+-rw-rw-rw-   0        0        0     1160 2022-08-08 17:30:21.000000 colemen_utils-2.9.63/colemen_utilities/directory_utils/__init__.py
+-rw-rw-rw-   0        0        0    30357 2022-08-08 17:30:21.000000 colemen_utils-2.9.63/colemen_utilities/directory_utils/dir.py
+-rw-rw-rw-   0        0        0     2136 2022-08-08 17:30:21.000000 colemen_utils-2.9.63/colemen_utilities/directory_utils/dir_compression.py
+-rw-rw-rw-   0        0        0    15095 2022-08-08 17:30:21.000000 colemen_utils-2.9.63/colemen_utilities/directory_utils/dir_create.py
+-rw-rw-rw-   0        0        0     3454 2022-08-08 17:30:21.000000 colemen_utils-2.9.63/colemen_utilities/directory_utils/dir_delete.py
+-rw-rw-rw-   0        0        0    12180 2022-08-08 17:30:21.000000 colemen_utils-2.9.63/colemen_utilities/directory_utils/dir_read.py
+-rw-rw-rw-   0        0        0     3692 2022-08-08 17:30:21.000000 colemen_utils-2.9.63/colemen_utilities/directory_utils/dir_search.py
+drwxrwxrwx   0        0        0        0 2022-12-14 20:12:55.915528 colemen_utils-2.9.63/colemen_utilities/drawio/
+-rw-rw-rw-   0        0        0     4203 2022-08-08 17:33:54.000000 colemen_utils-2.9.63/colemen_utilities/drawio/Connector.py
+-rw-rw-rw-   0        0        0    16617 2022-08-08 17:33:54.000000 colemen_utils-2.9.63/colemen_utilities/drawio/Diagram.py
+-rw-rw-rw-   0        0        0    10045 2022-08-08 17:33:54.000000 colemen_utils-2.9.63/colemen_utilities/drawio/Drawing.py
+-rw-rw-rw-   0        0        0     6189 2022-08-08 17:33:54.000000 colemen_utils-2.9.63/colemen_utilities/drawio/Mxcell.py
+-rw-rw-rw-   0        0        0    35265 2022-08-08 17:33:54.000000 colemen_utils-2.9.63/colemen_utilities/drawio/NodeBase.py
+-rw-rw-rw-   0        0        0    13812 2022-08-08 17:33:54.000000 colemen_utils-2.9.63/colemen_utilities/drawio/Onode.py
+-rw-rw-rw-   0        0        0      277 2022-08-08 17:30:21.000000 colemen_utils-2.9.63/colemen_utilities/drawio/__init__.py
+-rw-rw-rw-   0        0        0     4545 2022-08-08 17:33:54.000000 colemen_utils-2.9.63/colemen_utilities/drawio/diagram_utils.py
+-rw-rw-rw-   0        0        0    32154 2022-08-08 17:33:54.000000 colemen_utils-2.9.63/colemen_utilities/drawio/nodes.py
+drwxrwxrwx   0        0        0        0 2022-12-14 20:12:55.928528 colemen_utils-2.9.63/colemen_utilities/file_utils/
+-rw-rw-rw-   0        0        0    14264 2022-08-15 15:05:17.000000 colemen_utils-2.9.63/colemen_utilities/file_utils/File.py
+-rw-rw-rw-   0        0        0     2057 2022-08-15 15:05:38.000000 colemen_utils-2.9.63/colemen_utilities/file_utils/__init__.py
+-rw-rw-rw-   0        0        0    27148 2022-01-26 22:09:44.000000 colemen_utils-2.9.63/colemen_utilities/file_utils/exiftool.py
+-rw-rw-rw-   0        0        0     8353 2022-08-08 17:30:21.000000 colemen_utils-2.9.63/colemen_utilities/file_utils/file_compression.py
+-rw-rw-rw-   0        0        0    12456 2022-08-08 17:30:22.000000 colemen_utils-2.9.63/colemen_utilities/file_utils/file_convert.py
+-rw-rw-rw-   0        0        0    32721 2022-08-08 17:30:22.000000 colemen_utils-2.9.63/colemen_utilities/file_utils/file_image.py
+-rw-rw-rw-   0        0        0     6630 2022-08-15 14:48:40.000000 colemen_utils-2.9.63/colemen_utilities/file_utils/file_read.py
+-rw-rw-rw-   0        0        0     3939 2022-08-08 17:30:21.000000 colemen_utils-2.9.63/colemen_utilities/file_utils/file_search.py
+-rw-rw-rw-   0        0        0      312 2022-08-08 17:30:21.000000 colemen_utils-2.9.63/colemen_utilities/file_utils/file_string_facade.py
+-rw-rw-rw-   0        0        0    69198 2022-08-15 14:01:01.000000 colemen_utils-2.9.63/colemen_utilities/file_utils/file_utils.py
+-rw-rw-rw-   0        0        0     2208 2022-08-08 17:30:21.000000 colemen_utils-2.9.63/colemen_utilities/file_utils/file_write.py
+-rw-rw-rw-   0        0        0      279 2022-06-04 17:28:32.000000 colemen_utils-2.9.63/colemen_utilities/file_utils/resources.py
+drwxrwxrwx   0        0        0        0 2022-12-14 20:12:55.944528 colemen_utils-2.9.63/colemen_utilities/list_utils/
+-rw-rw-rw-   0        0        0      589 2022-08-08 17:30:21.000000 colemen_utils-2.9.63/colemen_utilities/list_utils/__init__.py
+-rw-rw-rw-   0        0        0     7801 2022-08-31 14:13:14.000000 colemen_utils-2.9.63/colemen_utilities/list_utils/list_utils.py
+-rw-rw-rw-   0        0        0        0 2022-12-06 14:26:55.000000 colemen_utils-2.9.63/colemen_utilities/parse_sql.py
+-rw-rw-rw-   0        0        0        0 2022-06-04 20:21:34.000000 colemen_utils-2.9.63/colemen_utilities/parse_utils.py
+drwxrwxrwx   0        0        0        0 2022-12-14 20:12:55.947528 colemen_utils-2.9.63/colemen_utilities/random_utils/
+-rw-rw-rw-   0        0        0      901 2022-08-08 17:30:21.000000 colemen_utils-2.9.63/colemen_utilities/random_utils/__init__.py
+-rw-rw-rw-   0        0        0    29815 2022-08-08 17:50:08.000000 colemen_utils-2.9.63/colemen_utilities/random_utils/rand_generation.py
+-rw-rw-rw-   0        0        0     6603 2022-08-08 17:30:21.000000 colemen_utils-2.9.63/colemen_utilities/random_utils/rand_utils.py
+drwxrwxrwx   0        0        0        0 2022-12-14 20:12:55.951530 colemen_utils-2.9.63/colemen_utilities/sql_utils/
+-rw-rw-rw-   0        0        0      626 2022-08-08 17:30:21.000000 colemen_utils-2.9.63/colemen_utilities/sql_utils/__init__.py
+-rw-rw-rw-   0        0        0     7618 2022-08-08 17:30:21.000000 colemen_utils-2.9.63/colemen_utilities/sql_utils/sql_format.py
+-rw-rw-rw-   0        0        0    46142 2022-12-13 18:59:34.000000 colemen_utils-2.9.63/colemen_utilities/sql_utils/sql_parse.py
+-rw-rw-rw-   0        0        0    58169 2022-12-09 21:39:20.000000 colemen_utils-2.9.63/colemen_utilities/sql_utils/sql_utils.py
+drwxrwxrwx   0        0        0        0 2022-12-14 20:12:55.958527 colemen_utils-2.9.63/colemen_utilities/string_utils/
+-rw-rw-rw-   0        0        0     1295 2022-08-08 17:30:21.000000 colemen_utils-2.9.63/colemen_utilities/string_utils/__init__.py
+-rw-rw-rw-   0        0        0     6436 2022-08-08 17:30:21.000000 colemen_utils-2.9.63/colemen_utilities/string_utils/string_conversion.py
+-rw-rw-rw-   0        0        0    17480 2022-12-14 19:58:02.000000 colemen_utils-2.9.63/colemen_utilities/string_utils/string_escaping.py
+-rw-rw-rw-   0        0        0    29280 2022-11-29 17:06:13.000000 colemen_utils-2.9.63/colemen_utilities/string_utils/string_format.py
+-rw-rw-rw-   0        0        0    10123 2022-08-08 17:30:21.000000 colemen_utils-2.9.63/colemen_utilities/string_utils/string_generation.py
+-rw-rw-rw-   0        0        0     3635 2022-08-08 17:30:21.000000 colemen_utils-2.9.63/colemen_utilities/string_utils/string_parsing.py
+-rw-rw-rw-   0        0        0     5497 2022-08-08 17:30:21.000000 colemen_utils-2.9.63/colemen_utilities/string_utils/string_strip.py
+drwxrwxrwx   0        0        0        0 2022-12-14 20:12:55.960528 colemen_utils-2.9.63/colemen_utilities/type_utils/
+-rw-rw-rw-   0        0        0      528 2022-08-08 17:30:21.000000 colemen_utils-2.9.63/colemen_utilities/type_utils/__init__.py
+-rw-rw-rw-   0        0        0     9173 2022-12-06 15:07:15.000000 colemen_utils-2.9.63/colemen_utilities/type_utils/type_utils.py
+drwxrwxrwx   0        0        0        0 2022-12-14 20:12:55.963531 colemen_utils-2.9.63/colemen_utilities/validate_utils/
+-rw-rw-rw-   0        0        0      626 2022-12-09 19:06:02.000000 colemen_utils-2.9.63/colemen_utilities/validate_utils/__init__.py
+-rw-rw-rw-   0        0        0     3902 2022-12-12 21:22:26.000000 colemen_utils-2.9.63/colemen_utilities/validate_utils/cerberus.py
+-rw-rw-rw-   0        0        0     2950 2022-12-09 20:45:04.000000 colemen_utils-2.9.63/colemen_utilities/validate_utils/general.py
+drwxrwxrwx   0        0        0        0 2022-12-14 20:12:55.981531 colemen_utils-2.9.63/colemen_utils.egg-info/
+-rw-rw-rw-   0        0        0      522 2022-12-14 20:12:55.000000 colemen_utils-2.9.63/colemen_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3856 2022-12-14 20:12:55.000000 colemen_utils-2.9.63/colemen_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-12-14 20:12:55.000000 colemen_utils-2.9.63/colemen_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      152 2022-12-14 20:12:55.000000 colemen_utils-2.9.63/colemen_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       47 2022-12-14 20:12:55.000000 colemen_utils-2.9.63/colemen_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      920 2022-12-09 18:54:19.000000 colemen_utils-2.9.63/colemen_utils.py
+-rw-rw-rw-   0        0        0       42 2022-12-14 20:12:55.983528 colemen_utils-2.9.63/setup.cfg
+-rw-rw-rw-   0        0        0     5639 2022-12-14 20:12:49.000000 colemen_utils-2.9.63/setup.py
```

### Comparing `colemen_utils-2.9.62/PKG-INFO` & `colemen_utils-2.9.63/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colemen_utils
-Version: 2.9.62
+Version: 2.9.63
 Summary: Colemen Utils
 Author: Colemen Atwood
 Author-email: <atwoodcolemen@gmail.com>
 Keywords: python
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `colemen_utils-2.9.62/colemen_config.py` & `colemen_utils-2.9.63/colemen_config.py`

 * *Files identical despite different names*

### Comparing `colemen_utils-2.9.62/colemen_utilities/console_utils/__init__.py` & `colemen_utils-2.9.63/colemen_utilities/console_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `colemen_utils-2.9.62/colemen_utilities/console_utils/print.py` & `colemen_utils-2.9.63/colemen_utilities/console_utils/print.py`

 * *Files identical despite different names*

### Comparing `colemen_utils-2.9.62/colemen_utilities/database_utils/DatabaseManager.py` & `colemen_utils-2.9.63/colemen_utilities/database_utils/DatabaseManager.py`

 * *Files identical despite different names*

### Comparing `colemen_utils-2.9.62/colemen_utilities/database_utils/MySQL/CacheFile.py` & `colemen_utils-2.9.63/colemen_utilities/database_utils/MySQL/CacheFile.py`

 * *Files identical despite different names*

### Comparing `colemen_utils-2.9.62/colemen_utilities/database_utils/MySQL/Column/Column.py` & `colemen_utils-2.9.63/colemen_utilities/database_utils/MySQL/Column/Column.py`

 * *Files identical despite different names*

### Comparing `colemen_utils-2.9.62/colemen_utilities/database_utils/MySQL/Column/column_utils.py` & `colemen_utils-2.9.63/colemen_utilities/database_utils/MySQL/Column/column_utils.py`

 * *Files identical despite different names*

### Comparing `colemen_utils-2.9.62/colemen_utilities/database_utils/MySQL/DeleteQuery.py` & `colemen_utils-2.9.63/colemen_utilities/database_utils/MySQL/DeleteQuery.py`

 * *Files identical despite different names*

### Comparing `colemen_utils-2.9.62/colemen_utilities/database_utils/MySQL/MySQLDatabase.py` & `colemen_utils-2.9.63/colemen_utilities/database_utils/MySQL/MySQLDatabase.py`

 * *Files identical despite different names*

### Comparing `colemen_utils-2.9.62/colemen_utilities/database_utils/MySQL/QueryBase.py` & `colemen_utils-2.9.63/colemen_utilities/database_utils/MySQL/QueryBase.py`

 * *Files identical despite different names*

### Comparing `colemen_utils-2.9.62/colemen_utilities/database_utils/MySQL/SelectQuery.py` & `colemen_utils-2.9.63/colemen_utilities/database_utils/MySQL/SelectQuery.py`

 * *Files identical despite different names*

### Comparing `colemen_utils-2.9.62/colemen_utilities/database_utils/MySQL/Table/Table.py` & `colemen_utils-2.9.63/colemen_utilities/database_utils/MySQL/Table/Table.py`

 * *Files identical despite different names*

### Comparing `colemen_utils-2.9.62/colemen_utilities/database_utils/MySQL/UpdateQuery.py` & `colemen_utils-2.9.63/colemen_utilities/database_utils/MySQL/UpdateQuery.py`

 * *Files identical despite different names*

### Comparing `colemen_utils-2.9.62/colemen_utilities/database_utils/MySQL/__init__.py` & `colemen_utils-2.9.63/colemen_utilities/database_utils/MySQL/__init__.py`

 * *Files identical despite different names*

### Comparing `colemen_utils-2.9.62/colemen_utilities/database_utils/TableDataManager.py` & `colemen_utils-2.9.63/colemen_utilities/database_utils/TableDataManager.py`

 * *Files identical despite different names*

### Comparing `colemen_utils-2.9.62/colemen_utilities/database_utils/TableManager.py` & `colemen_utils-2.9.63/colemen_utilities/database_utils/TableManager.py`

 * *Files identical despite different names*

### Comparing `colemen_utils-2.9.62/colemen_utilities/database_utils/__init__.py` & `colemen_utils-2.9.63/colemen_utilities/database_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `colemen_utils-2.9.62/colemen_utilities/database_utils/drawio/ForeignKey.py` & `colemen_utils-2.9.63/colemen_utilities/database_utils/drawio/ForeignKey.py`

 * *Files identical despite different names*

### Comparing `colemen_utils-2.9.62/colemen_utilities/database_utils/drawio/Parser.py` & `colemen_utils-2.9.63/colemen_utilities/database_utils/drawio/Parser.py`

 * *Files identical despite different names*

### Comparing `colemen_utils-2.9.62/colemen_utilities/database_utils/drawio/Row.py` & `colemen_utils-2.9.63/colemen_utilities/database_utils/drawio/Row.py`

 * *Files identical despite different names*

### Comparing `colemen_utils-2.9.62/colemen_utilities/database_utils/drawio/Schema.py` & `colemen_utils-2.9.63/colemen_utilities/database_utils/drawio/Schema.py`

 * *Files identical despite different names*

### Comparing `colemen_utils-2.9.62/colemen_utilities/database_utils/drawio/Table.py` & `colemen_utils-2.9.63/colemen_utilities/database_utils/drawio/Table.py`

 * *Files identical despite different names*

### Comparing `colemen_utils-2.9.62/colemen_utilities/database_utils/drawio/entity_utils.py` & `colemen_utils-2.9.63/colemen_utilities/database_utils/drawio/entity_utils.py`

 * *Files identical despite different names*

### Comparing `colemen_utils-2.9.62/colemen_utilities/dict_utils/__init__.py` & `colemen_utils-2.9.63/colemen_utilities/dict_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `colemen_utils-2.9.62/colemen_utilities/dict_utils/dict_utils.py` & `colemen_utils-2.9.63/colemen_utilities/dict_utils/dict_utils.py`

 * *Files identical despite different names*

### Comparing `colemen_utils-2.9.62/colemen_utilities/directory_utils/__init__.py` & `colemen_utils-2.9.63/colemen_utilities/directory_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `colemen_utils-2.9.62/colemen_utilities/directory_utils/dir.py` & `colemen_utils-2.9.63/colemen_utilities/directory_utils/dir.py`

 * *Files identical despite different names*

### Comparing `colemen_utils-2.9.62/colemen_utilities/directory_utils/dir_compression.py` & `colemen_utils-2.9.63/colemen_utilities/directory_utils/dir_compression.py`

 * *Files identical despite different names*

### Comparing `colemen_utils-2.9.62/colemen_utilities/directory_utils/dir_create.py` & `colemen_utils-2.9.63/colemen_utilities/directory_utils/dir_create.py`

 * *Files identical despite different names*

### Comparing `colemen_utils-2.9.62/colemen_utilities/directory_utils/dir_delete.py` & `colemen_utils-2.9.63/colemen_utilities/directory_utils/dir_delete.py`

 * *Files identical despite different names*

### Comparing `colemen_utils-2.9.62/colemen_utilities/directory_utils/dir_read.py` & `colemen_utils-2.9.63/colemen_utilities/directory_utils/dir_read.py`

 * *Files identical despite different names*

### Comparing `colemen_utils-2.9.62/colemen_utilities/directory_utils/dir_search.py` & `colemen_utils-2.9.63/colemen_utilities/directory_utils/dir_search.py`

 * *Files identical despite different names*

### Comparing `colemen_utils-2.9.62/colemen_utilities/drawio/Connector.py` & `colemen_utils-2.9.63/colemen_utilities/drawio/Connector.py`

 * *Files identical despite different names*

### Comparing `colemen_utils-2.9.62/colemen_utilities/drawio/Diagram.py` & `colemen_utils-2.9.63/colemen_utilities/drawio/Diagram.py`

 * *Files identical despite different names*

### Comparing `colemen_utils-2.9.62/colemen_utilities/drawio/Drawing.py` & `colemen_utils-2.9.63/colemen_utilities/drawio/Drawing.py`

 * *Files identical despite different names*

### Comparing `colemen_utils-2.9.62/colemen_utilities/drawio/Mxcell.py` & `colemen_utils-2.9.63/colemen_utilities/drawio/Mxcell.py`

 * *Files identical despite different names*

### Comparing `colemen_utils-2.9.62/colemen_utilities/drawio/NodeBase.py` & `colemen_utils-2.9.63/colemen_utilities/drawio/NodeBase.py`

 * *Files identical despite different names*

### Comparing `colemen_utils-2.9.62/colemen_utilities/drawio/Onode.py` & `colemen_utils-2.9.63/colemen_utilities/drawio/Onode.py`

 * *Files identical despite different names*

### Comparing `colemen_utils-2.9.62/colemen_utilities/drawio/diagram_utils.py` & `colemen_utils-2.9.63/colemen_utilities/drawio/diagram_utils.py`

 * *Files identical despite different names*

### Comparing `colemen_utils-2.9.62/colemen_utilities/drawio/nodes.py` & `colemen_utils-2.9.63/colemen_utilities/drawio/nodes.py`

 * *Files identical despite different names*

### Comparing `colemen_utils-2.9.62/colemen_utilities/file_utils/File.py` & `colemen_utils-2.9.63/colemen_utilities/file_utils/File.py`

 * *Files identical despite different names*

### Comparing `colemen_utils-2.9.62/colemen_utilities/file_utils/__init__.py` & `colemen_utils-2.9.63/colemen_utilities/file_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `colemen_utils-2.9.62/colemen_utilities/file_utils/exiftool.py` & `colemen_utils-2.9.63/colemen_utilities/file_utils/exiftool.py`

 * *Files identical despite different names*

### Comparing `colemen_utils-2.9.62/colemen_utilities/file_utils/file_compression.py` & `colemen_utils-2.9.63/colemen_utilities/file_utils/file_compression.py`

 * *Files identical despite different names*

### Comparing `colemen_utils-2.9.62/colemen_utilities/file_utils/file_convert.py` & `colemen_utils-2.9.63/colemen_utilities/file_utils/file_convert.py`

 * *Files identical despite different names*

### Comparing `colemen_utils-2.9.62/colemen_utilities/file_utils/file_image.py` & `colemen_utils-2.9.63/colemen_utilities/file_utils/file_image.py`

 * *Files identical despite different names*

### Comparing `colemen_utils-2.9.62/colemen_utilities/file_utils/file_read.py` & `colemen_utils-2.9.63/colemen_utilities/file_utils/file_read.py`

 * *Files identical despite different names*

### Comparing `colemen_utils-2.9.62/colemen_utilities/file_utils/file_search.py` & `colemen_utils-2.9.63/colemen_utilities/file_utils/file_search.py`

 * *Files identical despite different names*

### Comparing `colemen_utils-2.9.62/colemen_utilities/file_utils/file_utils.py` & `colemen_utils-2.9.63/colemen_utilities/file_utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `colemen_utils-2.9.62/colemen_utilities/file_utils/file_write.py` & `colemen_utils-2.9.63/colemen_utilities/file_utils/file_write.py`

 * *Files identical despite different names*

### Comparing `colemen_utils-2.9.62/colemen_utilities/list_utils/__init__.py` & `colemen_utils-2.9.63/colemen_utilities/list_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `colemen_utils-2.9.62/colemen_utilities/list_utils/list_utils.py` & `colemen_utils-2.9.63/colemen_utilities/list_utils/list_utils.py`

 * *Files identical despite different names*

### Comparing `colemen_utils-2.9.62/colemen_utilities/random_utils/__init__.py` & `colemen_utils-2.9.63/colemen_utilities/random_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `colemen_utils-2.9.62/colemen_utilities/random_utils/rand_generation.py` & `colemen_utils-2.9.63/colemen_utilities/random_utils/rand_generation.py`

 * *Files identical despite different names*

### Comparing `colemen_utils-2.9.62/colemen_utilities/random_utils/rand_utils.py` & `colemen_utils-2.9.63/colemen_utilities/random_utils/rand_utils.py`

 * *Files identical despite different names*

### Comparing `colemen_utils-2.9.62/colemen_utilities/sql_utils/__init__.py` & `colemen_utils-2.9.63/colemen_utilities/sql_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `colemen_utils-2.9.62/colemen_utilities/sql_utils/sql_format.py` & `colemen_utils-2.9.63/colemen_utilities/sql_utils/sql_format.py`

 * *Files identical despite different names*

### Comparing `colemen_utils-2.9.62/colemen_utilities/sql_utils/sql_parse.py` & `colemen_utils-2.9.63/colemen_utilities/sql_utils/sql_parse.py`

 * *Files identical despite different names*

### Comparing `colemen_utils-2.9.62/colemen_utilities/sql_utils/sql_utils.py` & `colemen_utils-2.9.63/colemen_utilities/sql_utils/sql_utils.py`

 * *Files identical despite different names*

### Comparing `colemen_utils-2.9.62/colemen_utilities/string_utils/__init__.py` & `colemen_utils-2.9.63/colemen_utilities/string_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `colemen_utils-2.9.62/colemen_utilities/string_utils/string_conversion.py` & `colemen_utils-2.9.63/colemen_utilities/string_utils/string_conversion.py`

 * *Files identical despite different names*

### Comparing `colemen_utils-2.9.62/colemen_utilities/string_utils/string_escaping.py` & `colemen_utils-2.9.63/colemen_utilities/string_utils/string_escaping.py`

 * *Files identical despite different names*

### Comparing `colemen_utils-2.9.62/colemen_utilities/string_utils/string_format.py` & `colemen_utils-2.9.63/colemen_utilities/string_utils/string_format.py`

 * *Files identical despite different names*

### Comparing `colemen_utils-2.9.62/colemen_utilities/string_utils/string_generation.py` & `colemen_utils-2.9.63/colemen_utilities/string_utils/string_generation.py`

 * *Files identical despite different names*

### Comparing `colemen_utils-2.9.62/colemen_utilities/string_utils/string_parsing.py` & `colemen_utils-2.9.63/colemen_utilities/string_utils/string_parsing.py`

 * *Files identical despite different names*

### Comparing `colemen_utils-2.9.62/colemen_utilities/string_utils/string_strip.py` & `colemen_utils-2.9.63/colemen_utilities/string_utils/string_strip.py`

 * *Files identical despite different names*

### Comparing `colemen_utils-2.9.62/colemen_utilities/type_utils/__init__.py` & `colemen_utils-2.9.63/colemen_utilities/type_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `colemen_utils-2.9.62/colemen_utilities/type_utils/type_utils.py` & `colemen_utils-2.9.63/colemen_utilities/type_utils/type_utils.py`

 * *Files identical despite different names*

### Comparing `colemen_utils-2.9.62/colemen_utilities/validate_utils/__init__.py` & `colemen_utils-2.9.63/colemen_utilities/validate_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `colemen_utils-2.9.62/colemen_utilities/validate_utils/cerberus.py` & `colemen_utils-2.9.63/colemen_utilities/validate_utils/cerberus.py`

 * *Files identical despite different names*

### Comparing `colemen_utils-2.9.62/colemen_utilities/validate_utils/general.py` & `colemen_utils-2.9.63/colemen_utilities/validate_utils/general.py`

 * *Files identical despite different names*

### Comparing `colemen_utils-2.9.62/colemen_utils.egg-info/PKG-INFO` & `colemen_utils-2.9.63/colemen_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colemen-utils
-Version: 2.9.62
+Version: 2.9.63
 Summary: Colemen Utils
 Author: Colemen Atwood
 Author-email: <atwoodcolemen@gmail.com>
 Keywords: python
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `colemen_utils-2.9.62/colemen_utils.egg-info/SOURCES.txt` & `colemen_utils-2.9.63/colemen_utils.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 colemen_utilities/console_utils/print.py
 colemen_utilities/database_utils/DatabaseManager.py
 colemen_utilities/database_utils/TableDataManager.py
 colemen_utilities/database_utils/TableManager.py
 colemen_utilities/database_utils/__init__.py
 colemen_utilities/database_utils/MySQL/CacheFile.py
 colemen_utilities/database_utils/MySQL/DeleteQuery.py
+colemen_utilities/database_utils/MySQL/InsertQuery.py
 colemen_utilities/database_utils/MySQL/MySQLDatabase.py
 colemen_utilities/database_utils/MySQL/QueryBase.py
 colemen_utilities/database_utils/MySQL/SelectQuery.py
 colemen_utilities/database_utils/MySQL/UpdateQuery.py
 colemen_utilities/database_utils/MySQL/__init__.py
 colemen_utilities/database_utils/MySQL/Column/Column.py
 colemen_utilities/database_utils/MySQL/Column/__init__.py
```

### Comparing `colemen_utils-2.9.62/colemen_utils.py` & `colemen_utils-2.9.63/colemen_utils.py`

 * *Files identical despite different names*

### Comparing `colemen_utils-2.9.62/setup.py` & `colemen_utils-2.9.63/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 import build_utils as _bu
-VERSION = '2.9.62'
+VERSION = '2.9.63'
 DESCRIPTION = 'Colemen Utils'
 LONG_DESCRIPTION = 'Colemen Utils is a composite library of shit I find useful.'
 
 
 _bu.purge_dist()
 
 # Setting up
@@ -32,14 +32,15 @@
         'colemen_utilities.database_utils.MySQL.DeleteQuery',
         'colemen_utilities.database_utils.MySQL.MySQLDatabase',
         'colemen_utilities.database_utils.MySQL.SelectQuery',
         'colemen_utilities.database_utils.MySQL.Table',
         'colemen_utilities.database_utils.MySQL.Table.Table',
         'colemen_utilities.database_utils.MySQL.UpdateQuery',
         'colemen_utilities.database_utils.MySQL.QueryBase',
+        'colemen_utilities.database_utils.MySQL.InsertQuery',
         'colemen_utilities.database_utils.TableDataManager',
         'colemen_utilities.database_utils.TableManager',
         'colemen_utilities.database_utils.drawio',
         'colemen_utilities.database_utils.drawio.ForeignKey',
         'colemen_utilities.database_utils.drawio.Parser',
         'colemen_utilities.database_utils.drawio.Row',
         'colemen_utilities.database_utils.drawio.Schema',
```

