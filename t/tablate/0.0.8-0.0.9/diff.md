# Comparing `tmp/tablate-0.0.8.tar.gz` & `tmp/tablate-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tablate-0.0.8.tar", last modified: Mon Jul 31 08:45:20 2023, max compression
+gzip compressed data, was "tablate-0.0.9.tar", last modified: Mon Jul 31 08:50:08 2023, max compression
```

## Comparing `tablate-0.0.8.tar` & `tablate-0.0.9.tar`

### file list

```diff
@@ -1,200 +1,200 @@
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.552162 tablate-0.0.8/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1069 2023-07-13 22:13:22.000000 tablate-0.0.8/LICENCE
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      554 2023-07-31 08:45:20.552162 tablate-0.0.8/PKG-INFO
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-24 14:23:22.000000 tablate-0.0.8/README.md
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      628 2023-07-31 08:44:51.000000 tablate-0.0.8/pyproject.toml
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       38 2023-07-31 08:45:20.552162 tablate-0.0.8/setup.cfg
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.524162 tablate-0.0.8/tablate/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      392 2023-07-25 22:27:18.000000 tablate-0.0.8/tablate/__init__.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.529162 tablate-0.0.8/tablate/api/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)    18347 2023-07-31 07:08:49.000000 tablate-0.0.8/tablate/api/Future.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 03:31:19.000000 tablate-0.0.8/tablate/api/ITablate.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     8378 2023-07-31 05:10:14.000000 tablate-0.0.8/tablate/api/Tablate.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 22:41:07.000000 tablate-0.0.8/tablate/api/__init__.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.529162 tablate-0.0.8/tablate/api/functions/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-23 04:48:05.000000 tablate-0.0.8/tablate/api/functions/__init__.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      993 2023-07-25 19:43:31.000000 tablate-0.0.8/tablate/api/functions/concat.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.530161 tablate-0.0.8/tablate/api/modules/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2115 2023-07-26 02:21:08.000000 tablate-0.0.8/tablate/api/modules/Grid.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3627 2023-07-28 12:18:13.000000 tablate-0.0.8/tablate/api/modules/Table.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2031 2023-07-25 02:00:37.000000 tablate-0.0.8/tablate/api/modules/Text.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-21 01:25:25.000000 tablate-0.0.8/tablate/api/modules/__init__.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.530161 tablate-0.0.8/tablate/classes/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-22 22:53:19.000000 tablate-0.0.8/tablate/classes/__init__.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.531162 tablate-0.0.8/tablate/classes/bases/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 03:32:45.000000 tablate-0.0.8/tablate/classes/bases/ITablateApi.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     5597 2023-07-31 04:47:30.000000 tablate-0.0.8/tablate/classes/bases/TablateApi.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      173 2023-07-26 01:09:49.000000 tablate-0.0.8/tablate/classes/bases/TablateBase.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 03:32:13.000000 tablate-0.0.8/tablate/classes/bases/TablateInit.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1329 2023-07-25 00:08:00.000000 tablate-0.0.8/tablate/classes/bases/TablateSet.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-22 22:25:16.000000 tablate-0.0.8/tablate/classes/bases/__init__.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      311 2023-07-25 22:32:01.000000 tablate-0.0.8/tablate/classes/classes.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.531162 tablate-0.0.8/tablate/classes/options/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 22:41:07.000000 tablate-0.0.8/tablate/classes/options/__init__.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.531162 tablate-0.0.8/tablate/classes/options/html/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-21 13:24:20.000000 tablate-0.0.8/tablate/classes/options/html/__init__.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.531162 tablate-0.0.8/tablate/classes/options/html/style/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     4877 2023-07-30 03:03:58.000000 tablate-0.0.8/tablate/classes/options/html/style/CssStyler.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-21 13:24:20.000000 tablate-0.0.8/tablate/classes/options/html/style/__init__.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.532162 tablate-0.0.8/tablate/classes/options/html/style/mixins/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      611 2023-07-30 04:43:48.000000 tablate-0.0.8/tablate/classes/options/html/style/mixins/AddStyleMixin.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      549 2023-07-25 00:34:59.000000 tablate-0.0.8/tablate/classes/options/html/style/mixins/ClassNameMixin.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-22 01:07:40.000000 tablate-0.0.8/tablate/classes/options/html/style/mixins/__init__.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.532162 tablate-0.0.8/tablate/classes/options/html/style/subclasses/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2587 2023-07-30 03:03:58.000000 tablate-0.0.8/tablate/classes/options/html/style/subclasses/ElementStyler.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      616 2023-07-30 03:03:58.000000 tablate-0.0.8/tablate/classes/options/html/style/subclasses/TableStyler.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      717 2023-07-30 03:03:58.000000 tablate-0.0.8/tablate/classes/options/html/style/subclasses/TextStyler.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-21 13:24:20.000000 tablate-0.0.8/tablate/classes/options/html/style/subclasses/__init__.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.533161 tablate-0.0.8/tablate/classes/options/html/style/utilities/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-21 15:13:12.000000 tablate-0.0.8/tablate/classes/options/html/style/utilities/__init__.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      286 2023-07-25 00:34:59.000000 tablate-0.0.8/tablate/classes/options/html/style/utilities/base_values.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3007 2023-07-30 03:15:25.000000 tablate-0.0.8/tablate/classes/options/html/style/utilities/css_factory.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1210 2023-07-25 00:34:59.000000 tablate-0.0.8/tablate/classes/options/html/style/utilities/selectors.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      876 2023-07-30 03:03:58.000000 tablate-0.0.8/tablate/classes/options/html/style/utilities/style_dict.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1102 2023-07-30 03:00:29.000000 tablate-0.0.8/tablate/classes/options/html/style/utilities/style_types.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.533161 tablate-0.0.8/tablate/library/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 01:14:04.000000 tablate-0.0.8/tablate/library/__init__.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.533161 tablate-0.0.8/tablate/library/ascii/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-23 07:07:45.000000 tablate-0.0.8/tablate/library/ascii/__init__.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.534162 tablate-0.0.8/tablate/library/ascii/chars/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 01:14:04.000000 tablate-0.0.8/tablate/library/ascii/chars/__init__.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      378 2023-07-16 22:19:15.000000 tablate-0.0.8/tablate/library/ascii/chars/corners.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       89 2023-07-16 22:19:15.000000 tablate-0.0.8/tablate/library/ascii/chars/line_h.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      108 2023-07-20 01:11:40.000000 tablate-0.0.8/tablate/library/ascii/chars/line_v.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2343 2023-07-19 23:07:53.000000 tablate-0.0.8/tablate/library/ascii/chars/matrix_cross.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      965 2023-07-16 22:19:15.000000 tablate-0.0.8/tablate/library/ascii/chars/matrix_side.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.534162 tablate-0.0.8/tablate/library/ascii/colors/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      479 2023-07-31 05:59:34.000000 tablate-0.0.8/tablate/library/ascii/colors/background.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      471 2023-07-31 05:59:34.000000 tablate-0.0.8/tablate/library/ascii/colors/characters.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.535162 tablate-0.0.8/tablate/library/ascii/styles/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      110 2023-07-31 05:58:51.000000 tablate-0.0.8/tablate/library/ascii/styles/styles.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.535162 tablate-0.0.8/tablate/library/calcs/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 22:51:23.000000 tablate-0.0.8/tablate/library/calcs/__init__.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      833 2023-07-29 00:59:58.000000 tablate-0.0.8/tablate/library/calcs/calc_column_percent.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3035 2023-07-30 04:43:48.000000 tablate-0.0.8/tablate/library/calcs/calc_column_widths.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      587 2023-07-19 21:45:43.000000 tablate-0.0.8/tablate/library/calcs/get_row_colspan.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      150 2023-07-23 04:37:08.000000 tablate-0.0.8/tablate/library/calcs/random_string.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.536162 tablate-0.0.8/tablate/library/checkers/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 03:34:30.000000 tablate-0.0.8/tablate/library/checkers/__init__.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       89 2023-07-16 05:52:57.000000 tablate-0.0.8/tablate/library/checkers/is_last_element.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      256 2023-07-30 03:50:35.000000 tablate-0.0.8/tablate/library/checkers/set_attr_resolver.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      174 2023-07-31 06:00:43.000000 tablate-0.0.8/tablate/library/checkers/set_key_resolver.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.536162 tablate-0.0.8/tablate/library/formatters/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 03:38:58.000000 tablate-0.0.8/tablate/library/formatters/__init__.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.537161 tablate-0.0.8/tablate/library/formatters/console/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 03:58:20.000000 tablate-0.0.8/tablate/library/formatters/console/__init__.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1065 2023-07-31 06:41:45.000000 tablate-0.0.8/tablate/library/formatters/console/ascii_styler.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     5248 2023-07-31 06:38:14.000000 tablate-0.0.8/tablate/library/formatters/console/cell_string.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      648 2023-07-31 06:55:06.000000 tablate-0.0.8/tablate/library/formatters/console/row_colors.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3458 2023-07-28 21:39:04.000000 tablate-0.0.8/tablate/library/formatters/console/row_line_divider.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      826 2023-07-28 20:40:34.000000 tablate-0.0.8/tablate/library/formatters/console/row_outer_border.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.537161 tablate-0.0.8/tablate/library/formatters/html/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 03:38:58.000000 tablate-0.0.8/tablate/library/formatters/html/__init__.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.538162 tablate-0.0.8/tablate/library/formatters/html/element/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 11:42:52.000000 tablate-0.0.8/tablate/library/formatters/html/element/__init__.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      721 2023-07-29 21:18:27.000000 tablate-0.0.8/tablate/library/formatters/html/element/column.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      490 2023-07-29 21:18:27.000000 tablate-0.0.8/tablate/library/formatters/html/element/frame.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      273 2023-07-30 04:59:45.000000 tablate-0.0.8/tablate/library/formatters/html/element/row.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      278 2023-07-29 21:18:27.000000 tablate-0.0.8/tablate/library/formatters/html/element/text.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.538162 tablate-0.0.8/tablate/library/formatters/html/style/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 11:43:30.000000 tablate-0.0.8/tablate/library/formatters/html/style/__init__.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.539162 tablate-0.0.8/tablate/library/formatters/html/style/attributes/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-29 02:34:03.000000 tablate-0.0.8/tablate/library/formatters/html/style/attributes/__init__.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1144 2023-07-31 07:15:41.000000 tablate-0.0.8/tablate/library/formatters/html/style/attributes/color.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      546 2023-07-31 02:08:02.000000 tablate-0.0.8/tablate/library/formatters/html/style/attributes/divider.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      161 2023-07-29 02:49:27.000000 tablate-0.0.8/tablate/library/formatters/html/style/attributes/padding.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      387 2023-07-29 07:37:01.000000 tablate-0.0.8/tablate/library/formatters/html/style/attributes/text.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.540161 tablate-0.0.8/tablate/library/formatters/html/style/elements/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-22 12:02:02.000000 tablate-0.0.8/tablate/library/formatters/html/style/elements/__init__.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     4439 2023-07-31 02:13:45.000000 tablate-0.0.8/tablate/library/formatters/html/style/elements/style_column.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2128 2023-07-31 01:51:02.000000 tablate-0.0.8/tablate/library/formatters/html/style/elements/style_frame.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1734 2023-07-31 06:57:10.000000 tablate-0.0.8/tablate/library/formatters/html/style/elements/style_rows.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1364 2023-07-31 01:27:34.000000 tablate-0.0.8/tablate/library/formatters/html/style/elements/style_text.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.541162 tablate-0.0.8/tablate/library/initializers/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-23 07:32:48.000000 tablate-0.0.8/tablate/library/initializers/__init__.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     4324 2023-07-31 04:59:57.000000 tablate-0.0.8/tablate/library/initializers/grid_init.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.541162 tablate-0.0.8/tablate/library/initializers/mappers/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-27 09:01:39.000000 tablate-0.0.8/tablate/library/initializers/mappers/__init__.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.541162 tablate-0.0.8/tablate/library/initializers/mappers/attribute/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-28 12:24:21.000000 tablate-0.0.8/tablate/library/initializers/mappers/attribute/__init__.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     4880 2023-07-31 06:57:30.000000 tablate-0.0.8/tablate/library/initializers/mappers/attribute/column_attr.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.541162 tablate-0.0.8/tablate/library/initializers/mappers/element/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-28 12:21:58.000000 tablate-0.0.8/tablate/library/initializers/mappers/element/__init__.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.543161 tablate-0.0.8/tablate/library/initializers/mappers/element/base/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-27 09:01:39.000000 tablate-0.0.8/tablate/library/initializers/mappers/element/base/__init__.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1520 2023-07-31 01:00:20.000000 tablate-0.0.8/tablate/library/initializers/mappers/element/base/base_column_mapper.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2980 2023-07-31 04:59:31.000000 tablate-0.0.8/tablate/library/initializers/mappers/element/base/base_frame_mapper.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1895 2023-07-31 01:00:20.000000 tablate-0.0.8/tablate/library/initializers/mappers/element/base/base_rows_mapper.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1930 2023-07-31 01:00:20.000000 tablate-0.0.8/tablate/library/initializers/mappers/element/base/base_text_mapper.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.544161 tablate-0.0.8/tablate/library/initializers/mappers/element/html/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-27 09:01:47.000000 tablate-0.0.8/tablate/library/initializers/mappers/element/html/__init__.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2241 2023-07-31 01:48:15.000000 tablate-0.0.8/tablate/library/initializers/mappers/element/html/html_column_mapper.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3128 2023-07-31 01:00:20.000000 tablate-0.0.8/tablate/library/initializers/mappers/element/html/html_frame_mapper.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2758 2023-07-31 01:00:20.000000 tablate-0.0.8/tablate/library/initializers/mappers/element/html/html_outer_mapper.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2500 2023-07-31 01:00:20.000000 tablate-0.0.8/tablate/library/initializers/mappers/element/html/html_rows_mapper.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2485 2023-07-31 01:00:20.000000 tablate-0.0.8/tablate/library/initializers/mappers/element/html/html_text_mapper.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3889 2023-07-31 01:04:05.000000 tablate-0.0.8/tablate/library/initializers/mappers/element/style_mapper.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)    11255 2023-07-31 04:59:14.000000 tablate-0.0.8/tablate/library/initializers/table_init.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     4780 2023-07-31 04:59:41.000000 tablate-0.0.8/tablate/library/initializers/text_init.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.544161 tablate-0.0.8/tablate/library/renderers/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 22:51:33.000000 tablate-0.0.8/tablate/library/renderers/__init__.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.545162 tablate-0.0.8/tablate/library/renderers/console/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 03:40:13.000000 tablate-0.0.8/tablate/library/renderers/console/__init__.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.545162 tablate-0.0.8/tablate/library/renderers/console/frames/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 06:15:27.000000 tablate-0.0.8/tablate/library/renderers/console/frames/__init__.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1783 2023-07-29 00:45:05.000000 tablate-0.0.8/tablate/library/renderers/console/frames/render_console_columns.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1991 2023-07-29 00:52:54.000000 tablate-0.0.8/tablate/library/renderers/console/frames/render_console_frame_grid.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3950 2023-07-31 06:56:57.000000 tablate-0.0.8/tablate/library/renderers/console/frames/render_console_frame_table.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      766 2023-07-26 01:09:49.000000 tablate-0.0.8/tablate/library/renderers/console/render_console.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      848 2023-07-28 20:40:34.000000 tablate-0.0.8/tablate/library/renderers/console/render_console_foot.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2059 2023-07-30 07:09:26.000000 tablate-0.0.8/tablate/library/renderers/console/render_console_frames.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      825 2023-07-28 20:40:34.000000 tablate-0.0.8/tablate/library/renderers/console/render_console_head.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.546162 tablate-0.0.8/tablate/library/renderers/html/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 03:40:21.000000 tablate-0.0.8/tablate/library/renderers/html/__init__.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.547161 tablate-0.0.8/tablate/library/renderers/html/frames/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2752 2023-07-31 01:22:49.000000 tablate-0.0.8/tablate/library/renderers/html/frames/render_html_columns.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2757 2023-07-31 01:28:00.000000 tablate-0.0.8/tablate/library/renderers/html/frames/render_html_table_body.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1330 2023-07-29 21:18:27.000000 tablate-0.0.8/tablate/library/renderers/html/render_html.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       51 2023-07-19 21:52:25.000000 tablate-0.0.8/tablate/library/renderers/html/render_html_foot.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1517 2023-07-31 01:59:19.000000 tablate-0.0.8/tablate/library/renderers/html/render_html_frames.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2078 2023-07-29 08:51:58.000000 tablate-0.0.8/tablate/library/renderers/html/render_html_head.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.548162 tablate-0.0.8/tablate/tests/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-22 00:41:48.000000 tablate-0.0.8/tablate/tests/__init__.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.550161 tablate-0.0.8/tablate/tests/old/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      121 2023-07-23 05:13:34.000000 tablate-0.0.8/tablate/tests/old/test_api_grid.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      362 2023-07-23 04:53:06.000000 tablate-0.0.8/tablate/tests/old/test_api_table.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       71 2023-07-23 05:12:51.000000 tablate-0.0.8/tablate/tests/old/test_api_text.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3544 2023-07-24 00:06:28.000000 tablate-0.0.8/tablate/tests/old/test_defs.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     8030 2023-07-23 07:18:53.000000 tablate-0.0.8/tablate/tests/old/test_objs.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       74 2023-07-22 22:51:46.000000 tablate-0.0.8/tablate/tests/old/test_out_html.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       66 2023-07-21 00:20:53.000000 tablate-0.0.8/tablate/tests/old/test_out_text.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      954 2023-07-29 21:18:27.000000 tablate-0.0.8/tablate/tests/old/test_styles.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.551162 tablate-0.0.8/tablate/tests/playpen/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      965 2023-07-26 21:51:22.000000 tablate-0.0.8/tablate/tests/playpen/classsy.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-25 00:44:00.000000 tablate-0.0.8/tablate/tests/playpen/func_maps.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      273 2023-07-27 06:35:01.000000 tablate-0.0.8/tablate/tests/playpen/func_sigs.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-25 00:44:00.000000 tablate-0.0.8/tablate/tests/playpen/key_of_dict.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2448 2023-07-23 08:39:36.000000 tablate-0.0.8/tablate/tests/playpen/loopy_test.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       95 2023-07-31 06:17:44.000000 tablate-0.0.8/tablate/tests/playpen/modulus.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      195 2023-07-25 23:32:08.000000 tablate-0.0.8/tablate/tests/playpen/prototype_test.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      121 2023-07-23 05:13:34.000000 tablate-0.0.8/tablate/tests/test_api_grid.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      362 2023-07-23 04:53:06.000000 tablate-0.0.8/tablate/tests/test_api_table.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       71 2023-07-23 05:12:51.000000 tablate-0.0.8/tablate/tests/test_api_text.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3544 2023-07-24 00:06:28.000000 tablate-0.0.8/tablate/tests/test_defs.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     8030 2023-07-23 07:18:53.000000 tablate-0.0.8/tablate/tests/test_objs.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       74 2023-07-22 22:51:46.000000 tablate-0.0.8/tablate/tests/test_out_html.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       66 2023-07-21 00:20:53.000000 tablate-0.0.8/tablate/tests/test_out_text.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      954 2023-07-29 21:18:27.000000 tablate-0.0.8/tablate/tests/test_styles.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.552162 tablate-0.0.8/tablate/type/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 07:43:04.000000 tablate-0.0.8/tablate/type/__init__.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2774 2023-07-31 03:58:54.000000 tablate-0.0.8/tablate/type/defaults.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2280 2023-07-31 03:58:54.000000 tablate-0.0.8/tablate/type/primitives.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3558 2023-07-31 01:00:20.000000 tablate-0.0.8/tablate/type/type_base.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      914 2023-07-31 04:59:15.000000 tablate-0.0.8/tablate/type/type_global.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3847 2023-07-30 04:43:48.000000 tablate-0.0.8/tablate/type/type_input.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2652 2023-07-31 04:59:14.000000 tablate-0.0.8/tablate/type/type_store.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.528162 tablate-0.0.8/tablate.egg-info/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      554 2023-07-31 08:45:20.000000 tablate-0.0.8/tablate.egg-info/PKG-INFO
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     6883 2023-07-31 08:45:20.000000 tablate-0.0.8/tablate.egg-info/SOURCES.txt
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        1 2023-07-31 08:45:20.000000 tablate-0.0.8/tablate.egg-info/dependency_links.txt
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        8 2023-07-31 08:45:20.000000 tablate-0.0.8/tablate.egg-info/top_level.txt
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:50:08.972175 tablate-0.0.9/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1069 2023-07-13 22:13:22.000000 tablate-0.0.9/LICENCE
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      554 2023-07-31 08:50:08.972175 tablate-0.0.9/PKG-INFO
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-24 14:23:22.000000 tablate-0.0.9/README.md
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      628 2023-07-31 08:50:02.000000 tablate-0.0.9/pyproject.toml
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       38 2023-07-31 08:50:08.972175 tablate-0.0.9/setup.cfg
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:50:08.952175 tablate-0.0.9/tablate/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      386 2023-07-31 08:50:02.000000 tablate-0.0.9/tablate/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:50:08.954175 tablate-0.0.9/tablate/api/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)    18347 2023-07-31 07:08:49.000000 tablate-0.0.9/tablate/api/Future.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 03:31:19.000000 tablate-0.0.9/tablate/api/ITablate.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)    18347 2023-07-31 08:50:02.000000 tablate-0.0.9/tablate/api/Tablate.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 22:41:07.000000 tablate-0.0.9/tablate/api/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:50:08.954175 tablate-0.0.9/tablate/api/functions/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-23 04:48:05.000000 tablate-0.0.9/tablate/api/functions/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      993 2023-07-25 19:43:31.000000 tablate-0.0.9/tablate/api/functions/concat.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:50:08.955175 tablate-0.0.9/tablate/api/modules/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2115 2023-07-26 02:21:08.000000 tablate-0.0.9/tablate/api/modules/Grid.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3627 2023-07-28 12:18:13.000000 tablate-0.0.9/tablate/api/modules/Table.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2031 2023-07-25 02:00:37.000000 tablate-0.0.9/tablate/api/modules/Text.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-21 01:25:25.000000 tablate-0.0.9/tablate/api/modules/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:50:08.955175 tablate-0.0.9/tablate/classes/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-22 22:53:19.000000 tablate-0.0.9/tablate/classes/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:50:08.956175 tablate-0.0.9/tablate/classes/bases/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 03:32:45.000000 tablate-0.0.9/tablate/classes/bases/ITablateApi.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     5597 2023-07-31 04:47:30.000000 tablate-0.0.9/tablate/classes/bases/TablateApi.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      173 2023-07-26 01:09:49.000000 tablate-0.0.9/tablate/classes/bases/TablateBase.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 03:32:13.000000 tablate-0.0.9/tablate/classes/bases/TablateInit.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1329 2023-07-25 00:08:00.000000 tablate-0.0.9/tablate/classes/bases/TablateSet.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-22 22:25:16.000000 tablate-0.0.9/tablate/classes/bases/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      311 2023-07-25 22:32:01.000000 tablate-0.0.9/tablate/classes/classes.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:50:08.956175 tablate-0.0.9/tablate/classes/options/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 22:41:07.000000 tablate-0.0.9/tablate/classes/options/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:50:08.957175 tablate-0.0.9/tablate/classes/options/html/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-21 13:24:20.000000 tablate-0.0.9/tablate/classes/options/html/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:50:08.957175 tablate-0.0.9/tablate/classes/options/html/style/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     4877 2023-07-30 03:03:58.000000 tablate-0.0.9/tablate/classes/options/html/style/CssStyler.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-21 13:24:20.000000 tablate-0.0.9/tablate/classes/options/html/style/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:50:08.958175 tablate-0.0.9/tablate/classes/options/html/style/mixins/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      611 2023-07-30 04:43:48.000000 tablate-0.0.9/tablate/classes/options/html/style/mixins/AddStyleMixin.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      549 2023-07-25 00:34:59.000000 tablate-0.0.9/tablate/classes/options/html/style/mixins/ClassNameMixin.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-22 01:07:40.000000 tablate-0.0.9/tablate/classes/options/html/style/mixins/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:50:08.958175 tablate-0.0.9/tablate/classes/options/html/style/subclasses/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2587 2023-07-30 03:03:58.000000 tablate-0.0.9/tablate/classes/options/html/style/subclasses/ElementStyler.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      616 2023-07-30 03:03:58.000000 tablate-0.0.9/tablate/classes/options/html/style/subclasses/TableStyler.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      717 2023-07-30 03:03:58.000000 tablate-0.0.9/tablate/classes/options/html/style/subclasses/TextStyler.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-21 13:24:20.000000 tablate-0.0.9/tablate/classes/options/html/style/subclasses/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:50:08.959175 tablate-0.0.9/tablate/classes/options/html/style/utilities/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-21 15:13:12.000000 tablate-0.0.9/tablate/classes/options/html/style/utilities/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      286 2023-07-25 00:34:59.000000 tablate-0.0.9/tablate/classes/options/html/style/utilities/base_values.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3007 2023-07-30 03:15:25.000000 tablate-0.0.9/tablate/classes/options/html/style/utilities/css_factory.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1210 2023-07-25 00:34:59.000000 tablate-0.0.9/tablate/classes/options/html/style/utilities/selectors.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      876 2023-07-30 03:03:58.000000 tablate-0.0.9/tablate/classes/options/html/style/utilities/style_dict.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1102 2023-07-30 03:00:29.000000 tablate-0.0.9/tablate/classes/options/html/style/utilities/style_types.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:50:08.959175 tablate-0.0.9/tablate/library/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 01:14:04.000000 tablate-0.0.9/tablate/library/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:50:08.959175 tablate-0.0.9/tablate/library/ascii/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-23 07:07:45.000000 tablate-0.0.9/tablate/library/ascii/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:50:08.960175 tablate-0.0.9/tablate/library/ascii/chars/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 01:14:04.000000 tablate-0.0.9/tablate/library/ascii/chars/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      378 2023-07-16 22:19:15.000000 tablate-0.0.9/tablate/library/ascii/chars/corners.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       89 2023-07-16 22:19:15.000000 tablate-0.0.9/tablate/library/ascii/chars/line_h.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      108 2023-07-20 01:11:40.000000 tablate-0.0.9/tablate/library/ascii/chars/line_v.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2343 2023-07-19 23:07:53.000000 tablate-0.0.9/tablate/library/ascii/chars/matrix_cross.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      965 2023-07-16 22:19:15.000000 tablate-0.0.9/tablate/library/ascii/chars/matrix_side.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:50:08.960175 tablate-0.0.9/tablate/library/ascii/colors/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      479 2023-07-31 05:59:34.000000 tablate-0.0.9/tablate/library/ascii/colors/background.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      471 2023-07-31 05:59:34.000000 tablate-0.0.9/tablate/library/ascii/colors/characters.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:50:08.961175 tablate-0.0.9/tablate/library/ascii/styles/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      110 2023-07-31 05:58:51.000000 tablate-0.0.9/tablate/library/ascii/styles/styles.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:50:08.961175 tablate-0.0.9/tablate/library/calcs/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 22:51:23.000000 tablate-0.0.9/tablate/library/calcs/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      833 2023-07-29 00:59:58.000000 tablate-0.0.9/tablate/library/calcs/calc_column_percent.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3035 2023-07-30 04:43:48.000000 tablate-0.0.9/tablate/library/calcs/calc_column_widths.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      587 2023-07-19 21:45:43.000000 tablate-0.0.9/tablate/library/calcs/get_row_colspan.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      150 2023-07-23 04:37:08.000000 tablate-0.0.9/tablate/library/calcs/random_string.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:50:08.961175 tablate-0.0.9/tablate/library/checkers/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 03:34:30.000000 tablate-0.0.9/tablate/library/checkers/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       89 2023-07-16 05:52:57.000000 tablate-0.0.9/tablate/library/checkers/is_last_element.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      256 2023-07-30 03:50:35.000000 tablate-0.0.9/tablate/library/checkers/set_attr_resolver.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      174 2023-07-31 06:00:43.000000 tablate-0.0.9/tablate/library/checkers/set_key_resolver.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:50:08.962175 tablate-0.0.9/tablate/library/formatters/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 03:38:58.000000 tablate-0.0.9/tablate/library/formatters/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:50:08.962175 tablate-0.0.9/tablate/library/formatters/console/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 03:58:20.000000 tablate-0.0.9/tablate/library/formatters/console/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1065 2023-07-31 06:41:45.000000 tablate-0.0.9/tablate/library/formatters/console/ascii_styler.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     5248 2023-07-31 06:38:14.000000 tablate-0.0.9/tablate/library/formatters/console/cell_string.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      648 2023-07-31 06:55:06.000000 tablate-0.0.9/tablate/library/formatters/console/row_colors.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3458 2023-07-28 21:39:04.000000 tablate-0.0.9/tablate/library/formatters/console/row_line_divider.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      826 2023-07-28 20:40:34.000000 tablate-0.0.9/tablate/library/formatters/console/row_outer_border.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:50:08.963175 tablate-0.0.9/tablate/library/formatters/html/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 03:38:58.000000 tablate-0.0.9/tablate/library/formatters/html/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:50:08.963175 tablate-0.0.9/tablate/library/formatters/html/element/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 11:42:52.000000 tablate-0.0.9/tablate/library/formatters/html/element/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      721 2023-07-29 21:18:27.000000 tablate-0.0.9/tablate/library/formatters/html/element/column.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      490 2023-07-29 21:18:27.000000 tablate-0.0.9/tablate/library/formatters/html/element/frame.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      273 2023-07-30 04:59:45.000000 tablate-0.0.9/tablate/library/formatters/html/element/row.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      278 2023-07-29 21:18:27.000000 tablate-0.0.9/tablate/library/formatters/html/element/text.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:50:08.963175 tablate-0.0.9/tablate/library/formatters/html/style/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 11:43:30.000000 tablate-0.0.9/tablate/library/formatters/html/style/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:50:08.964175 tablate-0.0.9/tablate/library/formatters/html/style/attributes/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-29 02:34:03.000000 tablate-0.0.9/tablate/library/formatters/html/style/attributes/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1144 2023-07-31 07:15:41.000000 tablate-0.0.9/tablate/library/formatters/html/style/attributes/color.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      546 2023-07-31 02:08:02.000000 tablate-0.0.9/tablate/library/formatters/html/style/attributes/divider.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      161 2023-07-29 02:49:27.000000 tablate-0.0.9/tablate/library/formatters/html/style/attributes/padding.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      387 2023-07-29 07:37:01.000000 tablate-0.0.9/tablate/library/formatters/html/style/attributes/text.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:50:08.965175 tablate-0.0.9/tablate/library/formatters/html/style/elements/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-22 12:02:02.000000 tablate-0.0.9/tablate/library/formatters/html/style/elements/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     4439 2023-07-31 02:13:45.000000 tablate-0.0.9/tablate/library/formatters/html/style/elements/style_column.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2128 2023-07-31 01:51:02.000000 tablate-0.0.9/tablate/library/formatters/html/style/elements/style_frame.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1734 2023-07-31 06:57:10.000000 tablate-0.0.9/tablate/library/formatters/html/style/elements/style_rows.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1364 2023-07-31 01:27:34.000000 tablate-0.0.9/tablate/library/formatters/html/style/elements/style_text.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:50:08.965175 tablate-0.0.9/tablate/library/initializers/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-23 07:32:48.000000 tablate-0.0.9/tablate/library/initializers/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     4324 2023-07-31 04:59:57.000000 tablate-0.0.9/tablate/library/initializers/grid_init.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:50:08.965175 tablate-0.0.9/tablate/library/initializers/mappers/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-27 09:01:39.000000 tablate-0.0.9/tablate/library/initializers/mappers/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:50:08.965175 tablate-0.0.9/tablate/library/initializers/mappers/attribute/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-28 12:24:21.000000 tablate-0.0.9/tablate/library/initializers/mappers/attribute/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     4880 2023-07-31 06:57:30.000000 tablate-0.0.9/tablate/library/initializers/mappers/attribute/column_attr.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:50:08.966175 tablate-0.0.9/tablate/library/initializers/mappers/element/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-28 12:21:58.000000 tablate-0.0.9/tablate/library/initializers/mappers/element/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:50:08.966175 tablate-0.0.9/tablate/library/initializers/mappers/element/base/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-27 09:01:39.000000 tablate-0.0.9/tablate/library/initializers/mappers/element/base/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1520 2023-07-31 01:00:20.000000 tablate-0.0.9/tablate/library/initializers/mappers/element/base/base_column_mapper.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2980 2023-07-31 04:59:31.000000 tablate-0.0.9/tablate/library/initializers/mappers/element/base/base_frame_mapper.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1895 2023-07-31 01:00:20.000000 tablate-0.0.9/tablate/library/initializers/mappers/element/base/base_rows_mapper.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1930 2023-07-31 01:00:20.000000 tablate-0.0.9/tablate/library/initializers/mappers/element/base/base_text_mapper.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:50:08.967175 tablate-0.0.9/tablate/library/initializers/mappers/element/html/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-27 09:01:47.000000 tablate-0.0.9/tablate/library/initializers/mappers/element/html/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2241 2023-07-31 01:48:15.000000 tablate-0.0.9/tablate/library/initializers/mappers/element/html/html_column_mapper.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3128 2023-07-31 01:00:20.000000 tablate-0.0.9/tablate/library/initializers/mappers/element/html/html_frame_mapper.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2758 2023-07-31 01:00:20.000000 tablate-0.0.9/tablate/library/initializers/mappers/element/html/html_outer_mapper.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2500 2023-07-31 01:00:20.000000 tablate-0.0.9/tablate/library/initializers/mappers/element/html/html_rows_mapper.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2485 2023-07-31 01:00:20.000000 tablate-0.0.9/tablate/library/initializers/mappers/element/html/html_text_mapper.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3889 2023-07-31 01:04:05.000000 tablate-0.0.9/tablate/library/initializers/mappers/element/style_mapper.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)    11255 2023-07-31 04:59:14.000000 tablate-0.0.9/tablate/library/initializers/table_init.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     4780 2023-07-31 04:59:41.000000 tablate-0.0.9/tablate/library/initializers/text_init.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:50:08.967175 tablate-0.0.9/tablate/library/renderers/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 22:51:33.000000 tablate-0.0.9/tablate/library/renderers/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:50:08.968175 tablate-0.0.9/tablate/library/renderers/console/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 03:40:13.000000 tablate-0.0.9/tablate/library/renderers/console/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:50:08.968175 tablate-0.0.9/tablate/library/renderers/console/frames/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 06:15:27.000000 tablate-0.0.9/tablate/library/renderers/console/frames/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1783 2023-07-29 00:45:05.000000 tablate-0.0.9/tablate/library/renderers/console/frames/render_console_columns.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1991 2023-07-29 00:52:54.000000 tablate-0.0.9/tablate/library/renderers/console/frames/render_console_frame_grid.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3950 2023-07-31 06:56:57.000000 tablate-0.0.9/tablate/library/renderers/console/frames/render_console_frame_table.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      766 2023-07-26 01:09:49.000000 tablate-0.0.9/tablate/library/renderers/console/render_console.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      848 2023-07-28 20:40:34.000000 tablate-0.0.9/tablate/library/renderers/console/render_console_foot.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2059 2023-07-30 07:09:26.000000 tablate-0.0.9/tablate/library/renderers/console/render_console_frames.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      825 2023-07-28 20:40:34.000000 tablate-0.0.9/tablate/library/renderers/console/render_console_head.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:50:08.968175 tablate-0.0.9/tablate/library/renderers/html/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 03:40:21.000000 tablate-0.0.9/tablate/library/renderers/html/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:50:08.969174 tablate-0.0.9/tablate/library/renderers/html/frames/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2752 2023-07-31 01:22:49.000000 tablate-0.0.9/tablate/library/renderers/html/frames/render_html_columns.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2757 2023-07-31 01:28:00.000000 tablate-0.0.9/tablate/library/renderers/html/frames/render_html_table_body.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1330 2023-07-29 21:18:27.000000 tablate-0.0.9/tablate/library/renderers/html/render_html.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       51 2023-07-19 21:52:25.000000 tablate-0.0.9/tablate/library/renderers/html/render_html_foot.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1517 2023-07-31 01:59:19.000000 tablate-0.0.9/tablate/library/renderers/html/render_html_frames.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2078 2023-07-29 08:51:58.000000 tablate-0.0.9/tablate/library/renderers/html/render_html_head.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:50:08.970175 tablate-0.0.9/tablate/tests/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-22 00:41:48.000000 tablate-0.0.9/tablate/tests/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:50:08.970175 tablate-0.0.9/tablate/tests/old/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      121 2023-07-23 05:13:34.000000 tablate-0.0.9/tablate/tests/old/test_api_grid.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      362 2023-07-23 04:53:06.000000 tablate-0.0.9/tablate/tests/old/test_api_table.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       71 2023-07-23 05:12:51.000000 tablate-0.0.9/tablate/tests/old/test_api_text.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3544 2023-07-24 00:06:28.000000 tablate-0.0.9/tablate/tests/old/test_defs.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     8030 2023-07-23 07:18:53.000000 tablate-0.0.9/tablate/tests/old/test_objs.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       74 2023-07-22 22:51:46.000000 tablate-0.0.9/tablate/tests/old/test_out_html.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       66 2023-07-21 00:20:53.000000 tablate-0.0.9/tablate/tests/old/test_out_text.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      954 2023-07-29 21:18:27.000000 tablate-0.0.9/tablate/tests/old/test_styles.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:50:08.971175 tablate-0.0.9/tablate/tests/playpen/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      965 2023-07-26 21:51:22.000000 tablate-0.0.9/tablate/tests/playpen/classsy.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-25 00:44:00.000000 tablate-0.0.9/tablate/tests/playpen/func_maps.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      273 2023-07-27 06:35:01.000000 tablate-0.0.9/tablate/tests/playpen/func_sigs.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-25 00:44:00.000000 tablate-0.0.9/tablate/tests/playpen/key_of_dict.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2448 2023-07-23 08:39:36.000000 tablate-0.0.9/tablate/tests/playpen/loopy_test.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       95 2023-07-31 06:17:44.000000 tablate-0.0.9/tablate/tests/playpen/modulus.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      195 2023-07-25 23:32:08.000000 tablate-0.0.9/tablate/tests/playpen/prototype_test.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      121 2023-07-23 05:13:34.000000 tablate-0.0.9/tablate/tests/test_api_grid.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      362 2023-07-23 04:53:06.000000 tablate-0.0.9/tablate/tests/test_api_table.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       71 2023-07-23 05:12:51.000000 tablate-0.0.9/tablate/tests/test_api_text.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3544 2023-07-24 00:06:28.000000 tablate-0.0.9/tablate/tests/test_defs.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     8030 2023-07-23 07:18:53.000000 tablate-0.0.9/tablate/tests/test_objs.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       74 2023-07-22 22:51:46.000000 tablate-0.0.9/tablate/tests/test_out_html.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       66 2023-07-21 00:20:53.000000 tablate-0.0.9/tablate/tests/test_out_text.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      954 2023-07-29 21:18:27.000000 tablate-0.0.9/tablate/tests/test_styles.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:50:08.972175 tablate-0.0.9/tablate/type/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 07:43:04.000000 tablate-0.0.9/tablate/type/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2774 2023-07-31 03:58:54.000000 tablate-0.0.9/tablate/type/defaults.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2280 2023-07-31 03:58:54.000000 tablate-0.0.9/tablate/type/primitives.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3558 2023-07-31 01:00:20.000000 tablate-0.0.9/tablate/type/type_base.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      914 2023-07-31 04:59:15.000000 tablate-0.0.9/tablate/type/type_global.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3847 2023-07-30 04:43:48.000000 tablate-0.0.9/tablate/type/type_input.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2652 2023-07-31 04:59:14.000000 tablate-0.0.9/tablate/type/type_store.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:50:08.953175 tablate-0.0.9/tablate.egg-info/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      554 2023-07-31 08:50:08.000000 tablate-0.0.9/tablate.egg-info/PKG-INFO
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     6883 2023-07-31 08:50:08.000000 tablate-0.0.9/tablate.egg-info/SOURCES.txt
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        1 2023-07-31 08:50:08.000000 tablate-0.0.9/tablate.egg-info/dependency_links.txt
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        8 2023-07-31 08:50:08.000000 tablate-0.0.9/tablate.egg-info/top_level.txt
```

### Comparing `tablate-0.0.8/LICENCE` & `tablate-0.0.9/LICENCE`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/PKG-INFO` & `tablate-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tablate
-Version: 0.0.8
+Version: 0.0.9
 Summary: A highly customizable and dynamic table renderer for IPython & CLI applications.
 Author-email: Guy de Winton <guy@codehippie.io>
 Project-URL: Homepage, https://gitlab.com/guydewinton/tablate
 Project-URL: Bug Tracker, https://gitlab.com/guydewinton/tablate/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tablate-0.0.8/pyproject.toml` & `tablate-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tablate"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Guy de Winton", email="guy@codehippie.io" },
 ]
 description = "A highly customizable and dynamic table renderer for IPython & CLI applications."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `tablate-0.0.8/tablate/api/Future.py` & `tablate-0.0.9/tablate/api/Future.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate/api/functions/concat.py` & `tablate-0.0.9/tablate/api/functions/concat.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate/api/modules/Grid.py` & `tablate-0.0.9/tablate/api/modules/Grid.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate/api/modules/Table.py` & `tablate-0.0.9/tablate/api/modules/Table.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate/api/modules/Text.py` & `tablate-0.0.9/tablate/api/modules/Text.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate/classes/bases/TablateApi.py` & `tablate-0.0.9/tablate/classes/bases/TablateApi.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate/classes/bases/TablateSet.py` & `tablate-0.0.9/tablate/classes/bases/TablateSet.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate/classes/options/html/style/CssStyler.py` & `tablate-0.0.9/tablate/classes/options/html/style/CssStyler.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate/classes/options/html/style/mixins/AddStyleMixin.py` & `tablate-0.0.9/tablate/classes/options/html/style/mixins/AddStyleMixin.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate/classes/options/html/style/mixins/ClassNameMixin.py` & `tablate-0.0.9/tablate/classes/options/html/style/mixins/ClassNameMixin.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate/classes/options/html/style/subclasses/ElementStyler.py` & `tablate-0.0.9/tablate/classes/options/html/style/subclasses/ElementStyler.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate/classes/options/html/style/subclasses/TableStyler.py` & `tablate-0.0.9/tablate/classes/options/html/style/subclasses/TableStyler.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate/classes/options/html/style/subclasses/TextStyler.py` & `tablate-0.0.9/tablate/classes/options/html/style/subclasses/TextStyler.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate/classes/options/html/style/utilities/css_factory.py` & `tablate-0.0.9/tablate/classes/options/html/style/utilities/css_factory.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate/classes/options/html/style/utilities/selectors.py` & `tablate-0.0.9/tablate/classes/options/html/style/utilities/selectors.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate/classes/options/html/style/utilities/style_dict.py` & `tablate-0.0.9/tablate/classes/options/html/style/utilities/style_dict.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate/classes/options/html/style/utilities/style_types.py` & `tablate-0.0.9/tablate/classes/options/html/style/utilities/style_types.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate/library/ascii/chars/matrix_cross.py` & `tablate-0.0.9/tablate/library/ascii/chars/matrix_cross.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate/library/ascii/chars/matrix_side.py` & `tablate-0.0.9/tablate/library/ascii/chars/matrix_side.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate/library/calcs/calc_column_percent.py` & `tablate-0.0.9/tablate/library/calcs/calc_column_percent.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate/library/calcs/calc_column_widths.py` & `tablate-0.0.9/tablate/library/calcs/calc_column_widths.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate/library/calcs/get_row_colspan.py` & `tablate-0.0.9/tablate/library/calcs/get_row_colspan.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate/library/formatters/console/ascii_styler.py` & `tablate-0.0.9/tablate/library/formatters/console/ascii_styler.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate/library/formatters/console/cell_string.py` & `tablate-0.0.9/tablate/library/formatters/console/cell_string.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate/library/formatters/console/row_colors.py` & `tablate-0.0.9/tablate/library/formatters/console/row_colors.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate/library/formatters/console/row_line_divider.py` & `tablate-0.0.9/tablate/library/formatters/console/row_line_divider.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate/library/formatters/console/row_outer_border.py` & `tablate-0.0.9/tablate/library/formatters/console/row_outer_border.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate/library/formatters/html/element/column.py` & `tablate-0.0.9/tablate/library/formatters/html/element/column.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate/library/formatters/html/style/attributes/color.py` & `tablate-0.0.9/tablate/library/formatters/html/style/attributes/color.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate/library/formatters/html/style/attributes/divider.py` & `tablate-0.0.9/tablate/library/formatters/html/style/attributes/divider.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate/library/formatters/html/style/elements/style_column.py` & `tablate-0.0.9/tablate/library/formatters/html/style/elements/style_column.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate/library/formatters/html/style/elements/style_frame.py` & `tablate-0.0.9/tablate/library/formatters/html/style/elements/style_frame.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate/library/formatters/html/style/elements/style_rows.py` & `tablate-0.0.9/tablate/library/formatters/html/style/elements/style_rows.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate/library/formatters/html/style/elements/style_text.py` & `tablate-0.0.9/tablate/library/formatters/html/style/elements/style_text.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate/library/initializers/grid_init.py` & `tablate-0.0.9/tablate/library/initializers/grid_init.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate/library/initializers/mappers/attribute/column_attr.py` & `tablate-0.0.9/tablate/library/initializers/mappers/attribute/column_attr.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate/library/initializers/mappers/element/base/base_column_mapper.py` & `tablate-0.0.9/tablate/library/initializers/mappers/element/base/base_column_mapper.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate/library/initializers/mappers/element/base/base_frame_mapper.py` & `tablate-0.0.9/tablate/library/initializers/mappers/element/base/base_frame_mapper.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate/library/initializers/mappers/element/base/base_rows_mapper.py` & `tablate-0.0.9/tablate/library/initializers/mappers/element/base/base_rows_mapper.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate/library/initializers/mappers/element/base/base_text_mapper.py` & `tablate-0.0.9/tablate/library/initializers/mappers/element/base/base_text_mapper.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate/library/initializers/mappers/element/html/html_column_mapper.py` & `tablate-0.0.9/tablate/library/initializers/mappers/element/html/html_column_mapper.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate/library/initializers/mappers/element/html/html_frame_mapper.py` & `tablate-0.0.9/tablate/library/initializers/mappers/element/html/html_frame_mapper.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate/library/initializers/mappers/element/html/html_outer_mapper.py` & `tablate-0.0.9/tablate/library/initializers/mappers/element/html/html_outer_mapper.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate/library/initializers/mappers/element/html/html_rows_mapper.py` & `tablate-0.0.9/tablate/library/initializers/mappers/element/html/html_rows_mapper.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate/library/initializers/mappers/element/html/html_text_mapper.py` & `tablate-0.0.9/tablate/library/initializers/mappers/element/html/html_text_mapper.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate/library/initializers/mappers/element/style_mapper.py` & `tablate-0.0.9/tablate/library/initializers/mappers/element/style_mapper.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate/library/initializers/table_init.py` & `tablate-0.0.9/tablate/library/initializers/table_init.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate/library/initializers/text_init.py` & `tablate-0.0.9/tablate/library/initializers/text_init.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate/library/renderers/console/frames/render_console_columns.py` & `tablate-0.0.9/tablate/library/renderers/console/frames/render_console_columns.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate/library/renderers/console/frames/render_console_frame_grid.py` & `tablate-0.0.9/tablate/library/renderers/console/frames/render_console_frame_grid.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate/library/renderers/console/frames/render_console_frame_table.py` & `tablate-0.0.9/tablate/library/renderers/console/frames/render_console_frame_table.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate/library/renderers/console/render_console.py` & `tablate-0.0.9/tablate/library/renderers/console/render_console.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate/library/renderers/console/render_console_foot.py` & `tablate-0.0.9/tablate/library/renderers/console/render_console_foot.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate/library/renderers/console/render_console_frames.py` & `tablate-0.0.9/tablate/library/renderers/console/render_console_frames.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate/library/renderers/console/render_console_head.py` & `tablate-0.0.9/tablate/library/renderers/console/render_console_head.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate/library/renderers/html/frames/render_html_columns.py` & `tablate-0.0.9/tablate/library/renderers/html/frames/render_html_columns.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate/library/renderers/html/frames/render_html_table_body.py` & `tablate-0.0.9/tablate/library/renderers/html/frames/render_html_table_body.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate/library/renderers/html/render_html.py` & `tablate-0.0.9/tablate/library/renderers/html/render_html.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate/library/renderers/html/render_html_frames.py` & `tablate-0.0.9/tablate/library/renderers/html/render_html_frames.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate/library/renderers/html/render_html_head.py` & `tablate-0.0.9/tablate/library/renderers/html/render_html_head.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate/tests/old/test_defs.py` & `tablate-0.0.9/tablate/tests/old/test_defs.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate/tests/old/test_objs.py` & `tablate-0.0.9/tablate/tests/old/test_objs.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate/tests/old/test_styles.py` & `tablate-0.0.9/tablate/tests/old/test_styles.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate/tests/playpen/classsy.py` & `tablate-0.0.9/tablate/tests/playpen/classsy.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate/tests/playpen/loopy_test.py` & `tablate-0.0.9/tablate/tests/playpen/loopy_test.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate/tests/test_defs.py` & `tablate-0.0.9/tablate/tests/test_defs.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate/tests/test_objs.py` & `tablate-0.0.9/tablate/tests/test_objs.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate/tests/test_styles.py` & `tablate-0.0.9/tablate/tests/test_styles.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate/type/defaults.py` & `tablate-0.0.9/tablate/type/defaults.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate/type/primitives.py` & `tablate-0.0.9/tablate/type/primitives.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate/type/type_base.py` & `tablate-0.0.9/tablate/type/type_base.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate/type/type_global.py` & `tablate-0.0.9/tablate/type/type_global.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate/type/type_input.py` & `tablate-0.0.9/tablate/type/type_input.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate/type/type_store.py` & `tablate-0.0.9/tablate/type/type_store.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.8/tablate.egg-info/PKG-INFO` & `tablate-0.0.9/tablate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tablate
-Version: 0.0.8
+Version: 0.0.9
 Summary: A highly customizable and dynamic table renderer for IPython & CLI applications.
 Author-email: Guy de Winton <guy@codehippie.io>
 Project-URL: Homepage, https://gitlab.com/guydewinton/tablate
 Project-URL: Bug Tracker, https://gitlab.com/guydewinton/tablate/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tablate-0.0.8/tablate.egg-info/SOURCES.txt` & `tablate-0.0.9/tablate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

