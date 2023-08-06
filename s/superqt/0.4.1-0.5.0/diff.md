# Comparing `tmp/superqt-0.4.1.tar.gz` & `tmp/superqt-0.5.0.tar.gz`

## Comparing `superqt-0.4.1.tar` & `superqt-0.5.0.tar`

### file list

```diff
@@ -1,66 +1,72 @@
--rw-r--r--   0        0        0    13863 2020-02-02 00:00:00.000000 superqt-0.4.1/CHANGELOG.md
--rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 superqt-0.4.1/src/superqt/__init__.py
--rw-r--r--   0        0        0     3779 2020-02-02 00:00:00.000000 superqt-0.4.1/src/superqt/_eliding_label.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 superqt-0.4.1/src/superqt/py.typed
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 superqt-0.4.1/src/superqt/collapsible/__init__.py
--rw-r--r--   0        0        0     7782 2020-02-02 00:00:00.000000 superqt-0.4.1/src/superqt/collapsible/_collapsible.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 superqt-0.4.1/src/superqt/combobox/__init__.py
--rw-r--r--   0        0        0     3864 2020-02-02 00:00:00.000000 superqt-0.4.1/src/superqt/combobox/_enum_combobox.py
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 superqt-0.4.1/src/superqt/combobox/_searchable_combo_box.py
--rw-r--r--   0        0        0     7889 2020-02-02 00:00:00.000000 superqt-0.4.1/src/superqt/fonticon/__init__.py
--rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 superqt-0.4.1/src/superqt/fonticon/_animations.py
--rw-r--r--   0        0        0     2862 2020-02-02 00:00:00.000000 superqt-0.4.1/src/superqt/fonticon/_iconfont.py
--rw-r--r--   0        0        0     3164 2020-02-02 00:00:00.000000 superqt-0.4.1/src/superqt/fonticon/_plugins.py
--rw-r--r--   0        0        0    19963 2020-02-02 00:00:00.000000 superqt-0.4.1/src/superqt/fonticon/_qfont_icon.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 superqt-0.4.1/src/superqt/qtcompat/__init__.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 superqt-0.4.1/src/superqt/selection/__init__.py
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 superqt-0.4.1/src/superqt/selection/_searchable_list_widget.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 superqt-0.4.1/src/superqt/sliders/__init__.py
--rw-r--r--   0        0        0    13769 2020-02-02 00:00:00.000000 superqt-0.4.1/src/superqt/sliders/_generic_range_slider.py
--rw-r--r--   0        0        0    19942 2020-02-02 00:00:00.000000 superqt-0.4.1/src/superqt/sliders/_generic_slider.py
--rw-r--r--   0        0        0    19868 2020-02-02 00:00:00.000000 superqt-0.4.1/src/superqt/sliders/_labeled.py
--rw-r--r--   0        0        0     9490 2020-02-02 00:00:00.000000 superqt-0.4.1/src/superqt/sliders/_range_style.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 superqt-0.4.1/src/superqt/sliders/_sliders.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 superqt-0.4.1/src/superqt/spinbox/__init__.py
--rw-r--r--   0        0        0     5632 2020-02-02 00:00:00.000000 superqt-0.4.1/src/superqt/spinbox/_intspin.py
--rw-r--r--   0        0        0     8544 2020-02-02 00:00:00.000000 superqt-0.4.1/src/superqt/spinbox/_quantity.py
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 superqt-0.4.1/src/superqt/utils/__init__.py
--rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 superqt-0.4.1/src/superqt/utils/_code_syntax_highlight.py
--rw-r--r--   0        0        0     5003 2020-02-02 00:00:00.000000 superqt-0.4.1/src/superqt/utils/_ensure_thread.py
--rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 superqt-0.4.1/src/superqt/utils/_message_handler.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 superqt-0.4.1/src/superqt/utils/_misc.py
--rw-r--r--   0        0        0    30765 2020-02-02 00:00:00.000000 superqt-0.4.1/src/superqt/utils/_qthreading.py
--rw-r--r--   0        0        0    12315 2020-02-02 00:00:00.000000 superqt-0.4.1/src/superqt/utils/_throttler.py
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 superqt-0.4.1/tests/test_code_highlight.py
--rw-r--r--   0        0        0     3957 2020-02-02 00:00:00.000000 superqt-0.4.1/tests/test_collapsible.py
--rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 superqt-0.4.1/tests/test_eliding_label.py
--rw-r--r--   0        0        0     6777 2020-02-02 00:00:00.000000 superqt-0.4.1/tests/test_ensure_thread.py
--rw-r--r--   0        0        0     3248 2020-02-02 00:00:00.000000 superqt-0.4.1/tests/test_enum_comb_box.py
--rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 superqt-0.4.1/tests/test_large_int_spinbox.py
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 superqt-0.4.1/tests/test_qmessage_handler.py
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 superqt-0.4.1/tests/test_quantity.py
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 superqt-0.4.1/tests/test_searchable_combobox.py
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 superqt-0.4.1/tests/test_searchable_list.py
--rw-r--r--   0        0        0     7803 2020-02-02 00:00:00.000000 superqt-0.4.1/tests/test_threadworker.py
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 superqt-0.4.1/tests/test_throttler.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 superqt-0.4.1/tests/test_utils.py
--rw-r--r--   0        0        0     4159 2020-02-02 00:00:00.000000 superqt-0.4.1/tests/test_fonticon/test_fonticon.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 superqt-0.4.1/tests/test_fonticon/test_plugins.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 superqt-0.4.1/tests/test_fonticon/fixtures/fake_plugin/__init__.py
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 superqt-0.4.1/tests/test_fonticon/fixtures/fake_plugin/icontest.ttf
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 superqt-0.4.1/tests/test_fonticon/fixtures/fake_plugin.dist-info/METADATA
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 superqt-0.4.1/tests/test_fonticon/fixtures/fake_plugin.dist-info/entry_points.txt
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 superqt-0.4.1/tests/test_fonticon/fixtures/fake_plugin.dist-info/top_level.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 superqt-0.4.1/tests/test_sliders/__init__.py
--rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 superqt-0.4.1/tests/test_sliders/_testutil.py
--rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 superqt-0.4.1/tests/test_sliders/test_float.py
--rw-r--r--   0        0        0     6060 2020-02-02 00:00:00.000000 superqt-0.4.1/tests/test_sliders/test_generic_slider.py
--rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 superqt-0.4.1/tests/test_sliders/test_labeled_slider.py
--rw-r--r--   0        0        0     7778 2020-02-02 00:00:00.000000 superqt-0.4.1/tests/test_sliders/test_range_slider.py
--rw-r--r--   0        0        0     7658 2020-02-02 00:00:00.000000 superqt-0.4.1/tests/test_sliders/test_single_value_sliders.py
--rw-r--r--   0        0        0     4231 2020-02-02 00:00:00.000000 superqt-0.4.1/tests/test_sliders/test_slider.py
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 superqt-0.4.1/.gitignore
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 superqt-0.4.1/LICENSE
--rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 superqt-0.4.1/README.md
--rw-r--r--   0        0        0     4917 2020-02-02 00:00:00.000000 superqt-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     5590 2020-02-02 00:00:00.000000 superqt-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0    15575 2020-02-02 00:00:00.000000 superqt-0.5.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 superqt-0.5.0/src/superqt/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 superqt-0.5.0/src/superqt/py.typed
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 superqt-0.5.0/src/superqt/collapsible/__init__.py
+-rw-r--r--   0        0        0     7795 2020-02-02 00:00:00.000000 superqt-0.5.0/src/superqt/collapsible/_collapsible.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 superqt-0.5.0/src/superqt/combobox/__init__.py
+-rw-r--r--   0        0        0     3864 2020-02-02 00:00:00.000000 superqt-0.5.0/src/superqt/combobox/_enum_combobox.py
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 superqt-0.5.0/src/superqt/combobox/_searchable_combo_box.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 superqt-0.5.0/src/superqt/elidable/__init__.py
+-rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 superqt-0.5.0/src/superqt/elidable/_eliding.py
+-rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 superqt-0.5.0/src/superqt/elidable/_eliding_label.py
+-rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 superqt-0.5.0/src/superqt/elidable/_eliding_line_edit.py
+-rw-r--r--   0        0        0     7862 2020-02-02 00:00:00.000000 superqt-0.5.0/src/superqt/fonticon/__init__.py
+-rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 superqt-0.5.0/src/superqt/fonticon/_animations.py
+-rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 superqt-0.5.0/src/superqt/fonticon/_iconfont.py
+-rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 superqt-0.5.0/src/superqt/fonticon/_plugins.py
+-rw-r--r--   0        0        0    20115 2020-02-02 00:00:00.000000 superqt-0.5.0/src/superqt/fonticon/_qfont_icon.py
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 superqt-0.5.0/src/superqt/qtcompat/__init__.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 superqt-0.5.0/src/superqt/selection/__init__.py
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 superqt-0.5.0/src/superqt/selection/_searchable_list_widget.py
+-rw-r--r--   0        0        0     4400 2020-02-02 00:00:00.000000 superqt-0.5.0/src/superqt/selection/_searchable_tree_widget.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 superqt-0.5.0/src/superqt/sliders/__init__.py
+-rw-r--r--   0        0        0    13740 2020-02-02 00:00:00.000000 superqt-0.5.0/src/superqt/sliders/_generic_range_slider.py
+-rw-r--r--   0        0        0    19918 2020-02-02 00:00:00.000000 superqt-0.5.0/src/superqt/sliders/_generic_slider.py
+-rw-r--r--   0        0        0    20188 2020-02-02 00:00:00.000000 superqt-0.5.0/src/superqt/sliders/_labeled.py
+-rw-r--r--   0        0        0     9489 2020-02-02 00:00:00.000000 superqt-0.5.0/src/superqt/sliders/_range_style.py
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 superqt-0.5.0/src/superqt/sliders/_sliders.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 superqt-0.5.0/src/superqt/spinbox/__init__.py
+-rw-r--r--   0        0        0     6604 2020-02-02 00:00:00.000000 superqt-0.5.0/src/superqt/spinbox/_intspin.py
+-rw-r--r--   0        0        0     8685 2020-02-02 00:00:00.000000 superqt-0.5.0/src/superqt/spinbox/_quantity.py
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 superqt-0.5.0/src/superqt/utils/__init__.py
+-rw-r--r--   0        0        0     3043 2020-02-02 00:00:00.000000 superqt-0.5.0/src/superqt/utils/_code_syntax_highlight.py
+-rw-r--r--   0        0        0     5023 2020-02-02 00:00:00.000000 superqt-0.5.0/src/superqt/utils/_ensure_thread.py
+-rw-r--r--   0        0        0     3121 2020-02-02 00:00:00.000000 superqt-0.5.0/src/superqt/utils/_message_handler.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 superqt-0.5.0/src/superqt/utils/_misc.py
+-rw-r--r--   0        0        0    30825 2020-02-02 00:00:00.000000 superqt-0.5.0/src/superqt/utils/_qthreading.py
+-rw-r--r--   0        0        0    12286 2020-02-02 00:00:00.000000 superqt-0.5.0/src/superqt/utils/_throttler.py
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 superqt-0.5.0/tests/test_code_highlight.py
+-rw-r--r--   0        0        0     3957 2020-02-02 00:00:00.000000 superqt-0.5.0/tests/test_collapsible.py
+-rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 superqt-0.5.0/tests/test_eliding_label.py
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 superqt-0.5.0/tests/test_eliding_line_edit.py
+-rw-r--r--   0        0        0     6783 2020-02-02 00:00:00.000000 superqt-0.5.0/tests/test_ensure_thread.py
+-rw-r--r--   0        0        0     3248 2020-02-02 00:00:00.000000 superqt-0.5.0/tests/test_enum_comb_box.py
+-rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 superqt-0.5.0/tests/test_large_int_spinbox.py
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 superqt-0.5.0/tests/test_qmessage_handler.py
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 superqt-0.5.0/tests/test_quantity.py
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 superqt-0.5.0/tests/test_searchable_combobox.py
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 superqt-0.5.0/tests/test_searchable_list.py
+-rw-r--r--   0        0        0     4490 2020-02-02 00:00:00.000000 superqt-0.5.0/tests/test_searchable_tree.py
+-rw-r--r--   0        0        0     7835 2020-02-02 00:00:00.000000 superqt-0.5.0/tests/test_threadworker.py
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 superqt-0.5.0/tests/test_throttler.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 superqt-0.5.0/tests/test_utils.py
+-rw-r--r--   0        0        0     4159 2020-02-02 00:00:00.000000 superqt-0.5.0/tests/test_fonticon/test_fonticon.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 superqt-0.5.0/tests/test_fonticon/test_plugins.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 superqt-0.5.0/tests/test_fonticon/fixtures/fake_plugin/__init__.py
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 superqt-0.5.0/tests/test_fonticon/fixtures/fake_plugin/icontest.ttf
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 superqt-0.5.0/tests/test_fonticon/fixtures/fake_plugin.dist-info/METADATA
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 superqt-0.5.0/tests/test_fonticon/fixtures/fake_plugin.dist-info/entry_points.txt
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 superqt-0.5.0/tests/test_fonticon/fixtures/fake_plugin.dist-info/top_level.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 superqt-0.5.0/tests/test_sliders/__init__.py
+-rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 superqt-0.5.0/tests/test_sliders/_testutil.py
+-rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 superqt-0.5.0/tests/test_sliders/test_float.py
+-rw-r--r--   0        0        0     6059 2020-02-02 00:00:00.000000 superqt-0.5.0/tests/test_sliders/test_generic_slider.py
+-rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 superqt-0.5.0/tests/test_sliders/test_labeled_slider.py
+-rw-r--r--   0        0        0     7776 2020-02-02 00:00:00.000000 superqt-0.5.0/tests/test_sliders/test_range_slider.py
+-rw-r--r--   0        0        0     7654 2020-02-02 00:00:00.000000 superqt-0.5.0/tests/test_sliders/test_single_value_sliders.py
+-rw-r--r--   0        0        0     4217 2020-02-02 00:00:00.000000 superqt-0.5.0/tests/test_sliders/test_slider.py
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 superqt-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 superqt-0.5.0/LICENSE
+-rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 superqt-0.5.0/README.md
+-rw-r--r--   0        0        0     5074 2020-02-02 00:00:00.000000 superqt-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     5337 2020-02-02 00:00:00.000000 superqt-0.5.0/PKG-INFO
```

### Comparing `superqt-0.4.1/CHANGELOG.md` & `superqt-0.5.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,44 @@
 # Changelog
 
-## [0.4.1](https://github.com/pyapp-kit/superqt/tree/0.4.1) (2022-12-01)
+## [v0.5.0](https://github.com/pyapp-kit/superqt/tree/v0.5.0) (2023-08-06)
 
-[Full Changelog](https://github.com/pyapp-kit/superqt/compare/v0.4.0...0.4.1)
+[Full Changelog](https://github.com/pyapp-kit/superqt/compare/v0.4.1...v0.5.0)
+
+**Implemented enhancements:**
+
+- feat: add stepType to largeInt spinbox [\#179](https://github.com/pyapp-kit/superqt/pull/179) ([tlambert03](https://github.com/tlambert03))
+- Searchable tree widget from a mapping [\#158](https://github.com/pyapp-kit/superqt/pull/158) ([andy-sweet](https://github.com/andy-sweet))
+- Add `QElidingLineEdit` class for elidable `QLineEdit`s [\#154](https://github.com/pyapp-kit/superqt/pull/154) ([dalthviz](https://github.com/dalthviz))
+
+**Fixed bugs:**
+
+- fix: focus events on QLabeledSlider [\#175](https://github.com/pyapp-kit/superqt/pull/175) ([tlambert03](https://github.com/tlambert03))
+- Set parent of timer in throttler [\#171](https://github.com/pyapp-kit/superqt/pull/171) ([Czaki](https://github.com/Czaki))
+- fix: fix double slider label editing [\#168](https://github.com/pyapp-kit/superqt/pull/168) ([tlambert03](https://github.com/tlambert03))
+
+**Documentation updates:**
+
+- Fix typos [\#147](https://github.com/pyapp-kit/superqt/pull/147) ([kianmeng](https://github.com/kianmeng))
+
+**Tests & CI:**
+
+- tests: add qtbot to test to fix windows segfault [\#165](https://github.com/pyapp-kit/superqt/pull/165) ([tlambert03](https://github.com/tlambert03))
+- test: fixing tests \[wip\] [\#164](https://github.com/pyapp-kit/superqt/pull/164) ([tlambert03](https://github.com/tlambert03))
+
+**Merged pull requests:**
+
+- build: unpin pyside6.5 [\#178](https://github.com/pyapp-kit/superqt/pull/178) ([tlambert03](https://github.com/tlambert03))
+- build: pin pyside6 to \<6.5.1 [\#169](https://github.com/pyapp-kit/superqt/pull/169) ([tlambert03](https://github.com/tlambert03))
+- pin pyside6\<6.5 [\#160](https://github.com/pyapp-kit/superqt/pull/160) ([tlambert03](https://github.com/tlambert03))
+- ci: \[pre-commit.ci\] autoupdate [\#146](https://github.com/pyapp-kit/superqt/pull/146) ([pre-commit-ci[bot]](https://github.com/apps/pre-commit-ci))
+
+## [v0.4.1](https://github.com/pyapp-kit/superqt/tree/v0.4.1) (2022-12-01)
+
+[Full Changelog](https://github.com/pyapp-kit/superqt/compare/v0.4.0...v0.4.1)
 
 **Implemented enhancements:**
 
 - feat: Add signal to QCollapsible [\#142](https://github.com/pyapp-kit/superqt/pull/142) ([ppwadhwa](https://github.com/ppwadhwa))
 - feat: Change icon used in Collapsible widget [\#140](https://github.com/pyapp-kit/superqt/pull/140) ([ppwadhwa](https://github.com/ppwadhwa))
 
 **Fixed bugs:**
@@ -250,25 +282,17 @@
 
 **Documentation updates:**
 
 - fix broken link [\#18](https://github.com/pyapp-kit/superqt/pull/18) ([haesleinhuepf](https://github.com/haesleinhuepf))
 
 ## [v0.2.1](https://github.com/pyapp-kit/superqt/tree/v0.2.1) (2021-07-10)
 
-[Full Changelog](https://github.com/pyapp-kit/superqt/compare/v0.2.0rc1...v0.2.1)
+[Full Changelog](https://github.com/pyapp-kit/superqt/compare/v0.2.0...v0.2.1)
 
 **Fixed bugs:**
 
 - Fix QLabeledRangeSlider API \(fix slider proxy\) [\#10](https://github.com/pyapp-kit/superqt/pull/10) ([tlambert03](https://github.com/tlambert03))
 - Fix range slider with negative min range [\#9](https://github.com/pyapp-kit/superqt/pull/9) ([tlambert03](https://github.com/tlambert03))
 
-## [v0.2.0rc1](https://github.com/pyapp-kit/superqt/tree/v0.2.0rc1) (2021-06-26)
-
-[Full Changelog](https://github.com/pyapp-kit/superqt/compare/v0.2.0rc0...v0.2.0rc1)
-
-## [v0.2.0rc0](https://github.com/pyapp-kit/superqt/tree/v0.2.0rc0) (2021-06-26)
-
-[Full Changelog](https://github.com/pyapp-kit/superqt/compare/v0.2.0...v0.2.0rc0)
-
 
 
 \* *This Changelog was automatically generated by [github_changelog_generator](https://github.com/github-changelog-generator/github-changelog-generator)*
```

### Comparing `superqt-0.4.1/src/superqt/__init__.py` & `superqt-0.5.0/src/superqt/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,18 +5,18 @@
     from ._version import version as __version__
 except ImportError:
     __version__ = "unknown"
 
 if TYPE_CHECKING:
     from .spinbox._quantity import QQuantity
 
-from ._eliding_label import QElidingLabel
 from .collapsible import QCollapsible
 from .combobox import QEnumComboBox, QSearchableComboBox
-from .selection import QSearchableListWidget
+from .elidable import QElidingLabel, QElidingLineEdit
+from .selection import QSearchableListWidget, QSearchableTreeWidget
 from .sliders import (
     QDoubleRangeSlider,
     QDoubleSlider,
     QLabeledDoubleRangeSlider,
     QLabeledDoubleSlider,
     QLabeledRangeSlider,
     QLabeledSlider,
@@ -28,25 +28,27 @@
 __all__ = [
     "ensure_main_thread",
     "ensure_object_thread",
     "QDoubleRangeSlider",
     "QCollapsible",
     "QDoubleSlider",
     "QElidingLabel",
+    "QElidingLineEdit",
     "QEnumComboBox",
     "QLabeledDoubleRangeSlider",
     "QLabeledDoubleSlider",
     "QLabeledRangeSlider",
     "QLabeledSlider",
     "QLargeIntSpinBox",
     "QMessageHandler",
     "QQuantity",
     "QRangeSlider",
     "QSearchableComboBox",
     "QSearchableListWidget",
+    "QSearchableTreeWidget",
 ]
 
 
 def __getattr__(name: str) -> Any:
     if name == "QQuantity":
         from .spinbox._quantity import QQuantity
```

### Comparing `superqt-0.4.1/src/superqt/_eliding_label.py` & `superqt-0.5.0/src/superqt/elidable/_eliding_line_edit.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,110 +1,91 @@
-from typing import List
+from qtpy.QtCore import Qt
+from qtpy.QtGui import QFocusEvent, QResizeEvent
+from qtpy.QtWidgets import QLineEdit
 
-from qtpy.QtCore import QPoint, QRect, QSize, Qt
-from qtpy.QtGui import QFont, QFontMetrics, QResizeEvent, QTextLayout
-from qtpy.QtWidgets import QLabel
+from ._eliding import _GenericEliding
 
 
-class QElidingLabel(QLabel):
-    """A QLabel variant that will elide text (add '…') to fit width.
+class QElidingLineEdit(_GenericEliding, QLineEdit):
+    """A QLineEdit variant that will elide text (could add '…') to fit width.
 
-    QElidingLabel()
-    QElidingLabel(parent: Optional[QWidget], f: Qt.WindowFlags = ...)
-    QElidingLabel(text: str, parent: Optional[QWidget] = None, f: Qt.WindowFlags = ...)
+    QElidingLineEdit()
+    QElidingLineEdit(parent: Optional[QWidget])
+    QElidingLineEdit(text: str, parent: Optional[QWidget] = None)
 
-    For a multiline eliding label, use `setWordWrap(True)`.  In this case, text
-    will wrap to fit the width, and only the last line will be elided.
-    When `wordWrap()` is True, `sizeHint()` will return the size required to fit
-    the full text.
     """
 
     def __init__(self, *args, **kwargs) -> None:
-        self._elide_mode = Qt.TextElideMode.ElideRight
         super().__init__(*args, **kwargs)
-        self.setText(args[0] if args and isinstance(args[0], str) else "")
+        if args and isinstance(args[0], str):
+            self.setText(args[0])
+        # The `textEdited` signal doesn't trigger the `textChanged` signal if
+        # text is changed with `setText`, so we connect to `textEdited` to only
+        # update _text when text is being edited by the user graphically.
+        self.textEdited.connect(self._update_text)
 
-    # New Public methods
+    # Reimplemented _GenericEliding methods
 
-    def elideMode(self) -> Qt.TextElideMode:
-        """The current Qt.TextElideMode."""
-        return self._elide_mode
+    def setElideMode(self, mode: Qt.TextElideMode) -> None:
+        """Set the elide mode to a Qt.TextElideMode.
 
-    def setElideMode(self, mode: Qt.TextElideMode):
-        """Set the elide mode to a Qt.TextElideMode."""
-        self._elide_mode = Qt.TextElideMode(mode)
-        super().setText(self._elidedText())
-
-    @staticmethod
-    def wrapText(text, width, font=None) -> List[str]:
-        """Returns `text`, split as it would be wrapped for `width`, given `font`.
-
-        Static method.
+        The text shown is updated to the elided version only if the widget is not
+        focused.
+        """
+        super().setElideMode(mode)
+        if not self.hasFocus():
+            super().setText(self._elidedText())
+
+    def setEllipsesWidth(self, width: int) -> None:
+        """A width value to take into account ellipses width when eliding text.
+
+        The value is deducted from the widget width when computing the elided version
+        of the text. The text shown is updated to the elided version only if the widget
+        is not focused.
         """
-        tl = QTextLayout(text, font or QFont())
-        tl.beginLayout()
-        lines = []
-        while True:
-            ln = tl.createLine()
-            if not ln.isValid():
-                break
-            ln.setLineWidth(width)
-            start = ln.textStart()
-            lines.append(text[start : start + ln.textLength()])
-        tl.endLayout()
-        return lines
+        super().setEllipsesWidth(width)
+        if not self.hasFocus():
+            super().setText(self._elidedText())
 
     # Reimplemented QT methods
 
     def text(self) -> str:
-        """Return the label's text.
+        """Return the label's text being shown.
 
         If no text has been set this will return an empty string.
         """
         return self._text
 
-    def setText(self, txt: str):
-        """Set the label's text.
+    def setText(self, text) -> None:
+        """Set the line edit's text.
 
         Setting the text clears any previous content.
-        NOTE: we set the QLabel private text to the elided version
+        NOTE: we set the QLineEdit private text to the elided version
         """
-        self._text = txt
-        super().setText(self._elidedText())
-
-    def resizeEvent(self, ev: QResizeEvent) -> None:
-        ev.accept()
-        super().setText(self._elidedText())
+        self._text = text
+        if not self.hasFocus():
+            super().setText(self._elidedText())
+
+    def focusInEvent(self, event: QFocusEvent) -> None:
+        """Set the full text when the widget is focused."""
+        super().setText(self._text)
+        super().focusInEvent(event)
 
-    def setWordWrap(self, wrap: bool) -> None:
-        super().setWordWrap(wrap)
+    def focusOutEvent(self, event: QFocusEvent) -> None:
+        """Set an elided version of the text (if needed) when the focus is out."""
         super().setText(self._elidedText())
+        super().focusOutEvent(event)
 
-    def sizeHint(self) -> QSize:
-        if not self.wordWrap():
-            return super().sizeHint()
-        fm = QFontMetrics(self.font())
-        flags = int(self.alignment() | Qt.TextFlag.TextWordWrap)
-        r = fm.boundingRect(QRect(QPoint(0, 0), self.size()), flags, self._text)
-        return QSize(self.width(), r.height())
+    def resizeEvent(self, event: QResizeEvent) -> None:
+        """Update elided text being shown when the widget is resized."""
+        if not self.hasFocus():
+            super().setText(self._elidedText())
+        super().resizeEvent(event)
 
     # private implementation methods
 
-    def _elidedText(self) -> str:
-        """Return `self._text` elided to `width`."""
-        fm = QFontMetrics(self.font())
-        # the 2 is a magic number that prevents the ellipses from going missing
-        # in certain cases (?)
-        width = self.width() - 2
-        if not self.wordWrap():
-            return fm.elidedText(self._text, self._elide_mode, width)
-
-        # get number of lines we can fit without eliding
-        nlines = self.height() // fm.height() - 1
-        # get the last line (elided)
-        text = self._wrappedText()
-        last_line = fm.elidedText("".join(text[nlines:]), self._elide_mode, width)
-        # join them
-        return "".join(text[:nlines] + [last_line])
+    def _update_text(self, text: str) -> None:
+        """Update only the actual text of the widget.
 
-    def _wrappedText(self) -> List[str]:
-        return QElidingLabel.wrapText(self._text, self.width(), self.font())
+        The actual text is the text the widget has without eliding.
+        """
+        self._text = text
```

### Comparing `superqt-0.4.1/src/superqt/collapsible/_collapsible.py` & `superqt-0.5.0/src/superqt/collapsible/_collapsible.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,41 +124,41 @@
             self._toggle_btn.setIcon(self._collapsed_icon)
 
     def setDuration(self, msecs: int) -> None:
         """Set duration of the collapse/expand animation."""
         self._animation.setDuration(msecs)
 
     def setEasingCurve(self, easing: QEasingCurve) -> None:
-        """Set the easing curve for the collapse/expand animation"""
+        """Set the easing curve for the collapse/expand animation."""
         self._animation.setEasingCurve(easing)
 
     def addWidget(self, widget: QWidget) -> None:
         """Add a widget to the central content widget's layout."""
         widget.installEventFilter(self)
         self._content.layout().addWidget(widget)
 
     def removeWidget(self, widget: QWidget) -> None:
         """Remove widget from the central content widget's layout."""
         self._content.layout().removeWidget(widget)
         widget.removeEventFilter(self)
 
     def expand(self, animate: bool = True) -> None:
-        """Expand (show) the collapsible section"""
+        """Expand (show) the collapsible section."""
         self._expand_collapse(QPropertyAnimation.Direction.Forward, animate)
 
     def collapse(self, animate: bool = True) -> None:
-        """Collapse (hide) the collapsible section"""
+        """Collapse (hide) the collapsible section."""
         self._expand_collapse(QPropertyAnimation.Direction.Backward, animate)
 
     def isExpanded(self) -> bool:
         """Return whether the collapsible section is visible."""
         return self._toggle_btn.isChecked()
 
     def setLocked(self, locked: bool = True) -> None:
-        """Set whether collapse/expand is disabled"""
+        """Set whether collapse/expand is disabled."""
         self._locked = locked
         self._toggle_btn.setCheckable(not locked)
 
     def locked(self) -> bool:
         """Return True if collapse/expand is disabled."""
         return self._locked
 
@@ -168,15 +168,16 @@
         animate: bool = True,
         emit: bool = True,
     ) -> None:
         """Set values for the widget based on whether it is expanding or collapsing.
 
         An emit flag is included so that the toggle signal is only called once (it
         was being emitted a few times via eventFilter when the widget was expanding
-        previously)."""
+        previously).
+        """
         if self._locked:
             return
 
         forward = direction == QPropertyAnimation.Direction.Forward
         icon = self._expanded_icon if forward else self._collapsed_icon
         self._toggle_btn.setIcon(icon)
         self._toggle_btn.setChecked(forward)
```

### Comparing `superqt-0.4.1/src/superqt/combobox/_enum_combobox.py` & `superqt-0.5.0/src/superqt/combobox/_enum_combobox.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,19 +48,19 @@
         self._enum_class = enum
         self._allow_none = allow_none and enum is not None
         if allow_none:
             super().addItem(NONE_STRING)
         super().addItems(list(map(_get_name, self._enum_class.__members__.values())))
 
     def enumClass(self) -> Optional[EnumMeta]:
-        """return current Enum class."""
+        """Return current Enum class."""
         return self._enum_class
 
     def isOptional(self) -> bool:
-        """return if current enum is with optional annotation."""
+        """Return if current enum is with optional annotation."""
         return self._allow_none
 
     def clear(self):
         self._enum_class = None
         self._allow_none = False
         super().clear()
```

### Comparing `superqt-0.4.1/src/superqt/combobox/_searchable_combo_box.py` & `superqt-0.5.0/src/superqt/combobox/_searchable_combo_box.py`

 * *Files identical despite different names*

### Comparing `superqt-0.4.1/src/superqt/fonticon/__init__.py` & `superqt-0.5.0/src/superqt/fonticon/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     opacity: float = 1,
     animation: Animation | None = None,
     transform: QTransform | None = None,
     states: dict[str, IconOptionDict | IconOpts] | None = None,
 ) -> QFontIcon:
     """Create a QIcon for `glyph_key`, with a number of optional settings.
 
-    The `glyph_key` (e.g. 'fa5s.smile') represents a Font-family & style, and a glpyh.
+    The `glyph_key` (e.g. 'fa5s.smile') represents a Font-family & style, and a glyph.
     In most cases, the key should be provided by a plugin in the environment, like:
 
     - [fonticon-fontawesome5](https://pypi.org/project/fonticon-fontawesome5/) ('fa5s' &
       'fa5r' prefixes)
     - [fonticon-materialdesignicons6](https://pypi.org/project/fonticon-materialdesignicons6/)
       ('mdi6' prefix)
 
@@ -85,15 +85,15 @@
           "active", "selected", "disabled"), or any combination of a state & mode
           separated by an underscore (e.g. "off_active", "selected_on", etc...).
         - the value is a dict with all of the same key/value meanings listed above as
           parameters to this function (e.g. `glyph_key`, `color`,`scale_factor`,
           `animation`, etc...)
 
         Missing keys in the state dicts will be taken from the default options, provided
-        by the paramters above.
+        by the parameters above.
 
     Returns
     -------
     QFontIcon
         A subclass of QIcon.  Can be used wherever QIcons are used, such as
         `widget.setIcon()`
 
@@ -133,15 +133,15 @@
     ...             },
     ...         },
     ...     )
     ... )
     >>> btn.setIconSize(QSize(256, 256))
     >>> btn.show()
 
-    """  # noqa: E501
+    """
     return _QFIS.instance().icon(
         glyph_key,
         scale_factor=scale_factor,
         color=color,
         opacity=opacity,
         animation=animation,
         transform=transform,
@@ -214,12 +214,12 @@
         See note above.
 
     Returns
     -------
     Tuple[str, str], optional
         font-family and font-style for the file just registered, or `None` if
         something goes wrong.
-    """  # noqa: E501
+    """
     return _QFIS.instance().addFont(filepath, prefix, charmap)
 
 
 del DEFAULT_SCALING_FACTOR
```

### Comparing `superqt-0.4.1/src/superqt/fonticon/_animations.py` & `superqt-0.5.0/src/superqt/fonticon/_animations.py`

 * *Files identical despite different names*

### Comparing `superqt-0.4.1/src/superqt/fonticon/_iconfont.py` & `superqt-0.5.0/src/superqt/fonticon/_iconfont.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,17 +68,18 @@
     __slots__ = ()
     __font_file__ = "..."
 
 
 def namespace2font(namespace: Union[Mapping, Type], name: str) -> Type[IconFont]:
     """Convenience to convert a namespace (class, module, dict) into an IconFont."""
     if isinstance(namespace, type):
-        assert isinstance(
-            getattr(namespace, FONTFILE_ATTR), str
-        ), "Not a valid font type"
+        if not isinstance(getattr(namespace, FONTFILE_ATTR), str):
+            raise TypeError(
+                f"Invalid Font: must declare {FONTFILE_ATTR!r} attribute or classmethod"
+            )
         return namespace
     elif hasattr(namespace, "__dict__"):
         ns = dict(namespace.__dict__)
     else:
         raise ValueError(
             "namespace must be a mapping or an object with __dict__ attribute."
         )
```

### Comparing `superqt-0.4.1/src/superqt/fonticon/_plugins.py` & `superqt-0.5.0/src/superqt/fonticon/_plugins.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from typing import Dict, List, Set, Tuple
+import contextlib
+from typing import ClassVar, Dict, List, Set, Tuple
 
 from ._iconfont import IconFontMeta, namespace2font
 
 try:
     from importlib.metadata import EntryPoint, entry_points
 except ImportError:
     from importlib_metadata import EntryPoint, entry_points  # type: ignore
 
 
 class FontIconManager:
-
-    ENTRY_POINT = "superqt.fonticon"
-    _PLUGINS: Dict[str, EntryPoint] = {}
-    _LOADED: Dict[str, IconFontMeta] = {}
-    _BLOCKED: Set[EntryPoint] = set()
+    ENTRY_POINT: ClassVar[str] = "superqt.fonticon"
+    _PLUGINS: ClassVar[Dict[str, EntryPoint]] = {}
+    _LOADED: ClassVar[Dict[str, IconFontMeta]] = {}
+    _BLOCKED: ClassVar[Set[EntryPoint]] = set()
 
     def _discover_fonts(self) -> None:
         self._PLUGINS.clear()
         entries = entry_points()
         if hasattr(entries, "select"):  # python>3.10
             _entries = entries.select(group=self.ENTRY_POINT)  # type: ignore
         else:
@@ -94,15 +94,13 @@
     return tuple(_manager._PLUGINS)
 
 
 def loaded(load_all=False) -> Dict[str, List[str]]:
     if load_all:
         discover()
         for x in available():
-            try:
+            with contextlib.suppress(Exception):
                 _manager._get_font_class(x)
-            except Exception:
-                continue
     return {
         key: sorted(filter(lambda x: not x.startswith("_"), cls.__dict__))
         for key, cls in _manager._LOADED.items()
     }
```

### Comparing `superqt-0.4.1/src/superqt/fonticon/_qfont_icon.py` & `superqt-0.5.0/src/superqt/fonticon/_qfont_icon.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import warnings
-from collections import abc
+from collections import abc, defaultdict
 from dataclasses import dataclass
 from pathlib import Path
-from typing import DefaultDict, Sequence, Tuple, Union, cast
+from typing import ClassVar, DefaultDict, Sequence, Tuple, Union, cast
 
 from qtpy import QT_VERSION
 from qtpy.QtCore import QObject, QPoint, QRect, QSize, Qt
 from qtpy.QtGui import (
     QColor,
     QFont,
     QFontDatabase,
@@ -19,15 +19,16 @@
     QPixmap,
     QPixmapCache,
     QTransform,
 )
 from qtpy.QtWidgets import QApplication, QStyleOption, QWidget
 from typing_extensions import TypedDict
 
-from ..utils import QMessageHandler
+from superqt.utils import QMessageHandler
+
 from ._animations import Animation
 
 
 class Unset:
     def __repr__(self) -> str:
         return "UNSET"
 
@@ -41,16 +42,16 @@
 DEFAULT_SCALING_FACTOR = 0.875
 DEFAULT_OPACITY = 1
 ValidColor = Union[
     QColor,
     int,
     str,
     Qt.GlobalColor,
-    Tuple[int, int, int, int],  # noqa: U006
-    Tuple[int, int, int],  # noqa: U006
+    Tuple[int, int, int, int],
+    Tuple[int, int, int],
     None,
 ]
 
 StateOrMode = Union[QIcon.State, QIcon.Mode]
 StateModeKey = Union[StateOrMode, str, Sequence[StateOrMode]]
 _SM_MAP: dict[str, StateOrMode] = {
     "on": QIcon.State.On,
@@ -152,15 +153,15 @@
 
 
 class _QFontIconEngine(QIconEngine):
     _opt_hash: str = ""
 
     def __init__(self, options: _IconOptions):
         super().__init__()
-        self._opts: DefaultDict[
+        self._opts: defaultdict[
             QIcon.State, dict[QIcon.Mode, _IconOptions | None]
         ] = DefaultDict(dict)
         self._opts[QIcon.State.Off][QIcon.Mode.Normal] = options
         self.update_hash()
 
     @property
     def _default_opts(self) -> _IconOptions:
@@ -226,15 +227,15 @@
     ) -> None:
         opts = self._get_opts(state, mode)
 
         char, family, style = QFontIconStore.key2glyph(opts.glyph_key)
 
         # font
         font = QFont()
-        font.setFamily(family)  # set sepeartely for Qt6
+        font.setFamily(family)  # set separately for Qt6
         font.setPixelSize(round(rect.height() * opts.scale_factor))
         if style:
             font.setStyleName(style)
 
         # color
         if isinstance(opts.color, tuple):
             color_args = opts.color
@@ -340,23 +341,22 @@
             animation=animation,
             transform=transform,
         )
         self._engine._add_opts(state, mode, _opts)
 
 
 class QFontIconStore(QObject):
-
     # map of key -> (font_family, font_style)
-    _LOADED_KEYS: dict[str, tuple[str, str]] = {}
+    _LOADED_KEYS: ClassVar[dict[str, tuple[str, str]]] = {}
 
     # map of (font_family, font_style) -> character (char may include key)
-    _CHARMAPS: dict[tuple[str, str | None], dict[str, str]] = {}
+    _CHARMAPS: ClassVar[dict[tuple[str, str | None], dict[str, str]]] = {}
 
     # singleton instance, use `instance()` to retrieve
-    __instance: QFontIconStore | None = None
+    __instance: ClassVar[QFontIconStore | None] = None
 
     def __init__(self, parent: QObject | None = None) -> None:
         super().__init__(parent=parent)
         if tuple(cast(str, QT_VERSION).split(".")) < ("6", "0"):
             # QT6 drops this
             QApplication.setAttribute(Qt.ApplicationAttribute.AA_UseHighDpiPixmaps)
 
@@ -393,15 +393,15 @@
                     f"Known plugin keys include: {_plugins.available()}.\n"
                     f"Loaded keys include: {list(cls._LOADED_KEYS)}."
                 ) from e
         return cls._LOADED_KEYS[key]
 
     @classmethod
     def _ensure_char(cls, char: str, family: str, style: str) -> str:
-        """make sure that `char` is a glyph provided by `family` and `style`."""
+        """Make sure that `char` is a glyph provided by `family` and `style`."""
         if len(char) == 1 and ord(char) > 256:
             return char
         try:
             charmap = cls._CHARMAPS[(family, style)]
         except KeyError as e:
             raise KeyError(
                 f"No charmap registered for font '{family} ({style})'"
@@ -427,15 +427,15 @@
         char = cls._ensure_char(char, family, style)
         return char, family, style
 
     @classmethod
     def addFont(
         cls, filepath: str, prefix: str, charmap: dict[str, str] | None = None
     ) -> tuple[str, str] | None:
-        """Add font at `filepath` to the registry under `key`.
+        r"""Add font at `filepath` to the registry under `key`.
 
         If you'd like to later use a fontkey in the form of `key.some-name`, then
         `charmap` must be provided and provide a mapping for all of the glyph names
         to their unicode numbers. If a charmap is not provided, glyphs must be directly
         accessed with their unicode as something like `key.\\uffff`.
 
         Parameters
@@ -452,46 +452,47 @@
         Returns
         -------
         Tuple[str, str], optional
             font-family and font-style for the file just registered, or None if
             something goes wrong.
         """
         if prefix in cls._LOADED_KEYS:
-            warnings.warn(f"Prefix {prefix} already loaded")
+            warnings.warn(f"Prefix {prefix} already loaded", stacklevel=2)
             return None
 
         if not Path(filepath).exists():
             raise FileNotFoundError(f"Font file doesn't exist: {filepath}")
         if QApplication.instance() is None:
             raise RuntimeError("Please create QApplication before adding a Font")
 
         fontId = QFontDatabase.addApplicationFont(str(Path(filepath).absolute()))
         if fontId < 0:  # pragma: no cover
-            warnings.warn(f"Cannot load font file: {filepath}")
+            warnings.warn(f"Cannot load font file: {filepath}", stacklevel=2)
             return None
 
         families = QFontDatabase.applicationFontFamilies(fontId)
         if not families:  # pragma: no cover
-            warnings.warn(f"Font file is empty!: {filepath}")
+            warnings.warn(f"Font file is empty!: {filepath}", stacklevel=2)
             return None
         family: str = families[0]
 
         # in Qt6, everything becomes a static member
-        QFd: QFontDatabase | "type[QFontDatabase]" = (
+        QFd: QFontDatabase | type[QFontDatabase] = (
             QFontDatabase()
             if tuple(cast(str, QT_VERSION).split(".")) < ("6", "0")
             else QFontDatabase
         )
 
         styles = QFd.styles(family)
         style: str = styles[-1] if styles else ""
         if not QFd.isSmoothlyScalable(family, style):  # pragma: no cover
             warnings.warn(
                 f"Registered font {family} ({style}) is not smoothly scalable. "
-                "Icons may not look attractive."
+                "Icons may not look attractive.",
+                stacklevel=2,
             )
 
         cls._LOADED_KEYS[prefix] = (family, style)
         if charmap:
             cls._CHARMAPS[(family, style)] = charmap
         return (family, style)
 
@@ -567,9 +568,10 @@
     # add _ to end of reserved keywords
     if keyword.iskeyword(name):
         name += "_"
 
     # replace dashes and spaces with underscores
     name = name.replace("-", "_").replace(" ", "_")
 
-    assert str.isidentifier(name), f"Could not canonicalize name: {name}"
+    if not str.isidentifier(name):
+        raise ValueError(f"Could not canonicalize name: {name!r}. (not an identifier)")
     return name
```

### Comparing `superqt-0.4.1/src/superqt/qtcompat/__init__.py` & `superqt-0.5.0/src/superqt/qtcompat/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,19 +2,21 @@
 import warnings
 from importlib import abc, util
 
 from qtpy import *  # noqa
 
 warnings.warn(
     "The superqt.qtcompat module is deprecated as of v0.3.0. "
-    "Please import from `qtpy` instead."
+    "Please import from `qtpy` instead.",
+    stacklevel=2,
 )
 
 
 # forward any requests for superqt.qtcompat.* to qtpy.*
 class SuperQtImporter(abc.MetaPathFinder):
     def find_spec(self, fullname: str, path, target=None):  # type: ignore
+        """Forward any requests for superqt.qtcompat.* to qtpy.*."""
         if fullname.startswith(__name__):
             return util.find_spec(fullname.replace(__name__, "qtpy"))
 
 
 sys.meta_path.append(SuperQtImporter())
```

### Comparing `superqt-0.4.1/src/superqt/selection/_searchable_list_widget.py` & `superqt-0.5.0/src/superqt/selection/_searchable_list_widget.py`

 * *Files identical despite different names*

### Comparing `superqt-0.4.1/src/superqt/sliders/_generic_range_slider.py` & `superqt-0.5.0/src/superqt/sliders/_generic_range_slider.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Generic, List, Optional, Sequence, Tuple, TypeVar, Union
+from typing import List, Optional, Sequence, Tuple, TypeVar, Union
 
 from qtpy import QtGui
 from qtpy.QtCore import Property, QEvent, QPoint, QPointF, QRect, QRectF, Qt, Signal
 from qtpy.QtWidgets import QSlider, QStyle, QStyleOptionSlider, QStylePainter
 
 from ._generic_slider import CC_SLIDER, SC_GROOVE, SC_HANDLE, SC_NONE, _GenericSlider
 from ._range_style import (
@@ -13,15 +13,15 @@
 
 _T = TypeVar("_T")
 
 
 SC_BAR = QStyle.SubControl.SC_ScrollBarSubPage
 
 
-class _GenericRangeSlider(_GenericSlider[Tuple], Generic[_T]):
+class _GenericRangeSlider(_GenericSlider):
     """MultiHandle Range Slider widget.
 
     Same API as QSlider, but `value`, `setValue`, `sliderPosition`, and
     `setSliderPosition` are all sequences of integers.
 
     The `valueChanged` and `sliderMoved` signals also both emit a tuple of
     integers.
```

### Comparing `superqt-0.4.1/src/superqt/sliders/_generic_slider.py` & `superqt-0.5.0/src/superqt/sliders/_generic_slider.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Generic Sliders with internal python-based models.
 
 This module reimplements most of the logic from qslider.cpp in python:
 https://code.woboq.org/qt5/qtbase/src/widgets/widgets/qslider.cpp.html
 
 This probably looks like tremendous overkill at first (and it may be!),
-since a it's possible to acheive a very reasonable "float slider" by
+since a it's possible to achieve a very reasonable "float slider" by
 scaling input float values to some internal integer range for the QSlider,
 and converting back to float when getting `value()`.  However, one still
 runs into overflow limitations due to the internal integer model.
 
 In order to circumvent them, one needs to reimplement more and more of
 the attributes from QSliderPrivate in order to have the slider behave
 like a native slider (with all of the proper signals and options).
@@ -17,15 +17,15 @@
 `_GenericRangeSlider` is a variant that expects `value()` and
 `sliderPosition()` to be a sequence of scalars rather than a single
 scalar (with one handle per item), and it forms the basis of
 QRangeSlider.
 """
 import os
 import platform
-from typing import Generic, TypeVar
+from typing import TypeVar
 
 from qtpy import QT_VERSION, QtGui
 from qtpy.QtCore import QEvent, QPoint, QPointF, QRect, Qt, Signal
 from qtpy.QtWidgets import (
     QApplication,
     QSlider,
     QStyle,
@@ -54,23 +54,22 @@
     and int(QT_VERSION.split(".")[0]) < 6
     and platform.system() == "Darwin"
     and int(platform.mac_ver()[0].split(".", maxsplit=1)[0]) >= 12
     and os.getenv("USE_MAC_SLIDER_PATCH", "0") not in ("0", "False", "false")
 )
 
 
-class _GenericSlider(QSlider, Generic[_T]):
+class _GenericSlider(QSlider):
     _fvalueChanged = Signal(int)
     _fsliderMoved = Signal(int)
     _frangeChanged = Signal(int, int)
 
     MAX_DISPLAY = 5000
 
     def __init__(self, *args, **kwargs) -> None:
-
         self._minimum = 0.0
         self._maximum = 99.0
         self._pageStep = 10.0
         self._value: _T = 0.0  # type: ignore
         self._position: _T = 0.0
         self._singleStep = 1.0
         self._offsetAccumulated = 0.0
@@ -272,15 +271,14 @@
         self._pressedControl = SC_NONE
         self.setRepeatAction(QSlider.SliderAction.SliderNoAction)
         if oldPressed != SC_NONE:
             self.setSliderDown(False)
         self.update()
 
     def wheelEvent(self, e: QtGui.QWheelEvent) -> None:
-
         e.ignore()
         vertical = bool(e.angleDelta().y())
         delta = e.angleDelta().y() if vertical else e.angleDelta().x()
         if e.inverted():
             delta *= -1
 
         orientation = Qt.Orientation.Vertical if vertical else Qt.Orientation.Horizontal
```

### Comparing `superqt-0.4.1/src/superqt/sliders/_labeled.py` & `superqt-0.5.0/src/superqt/sliders/_labeled.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import contextlib
 from enum import IntEnum
 from functools import partial
 from typing import Any
 
 from qtpy.QtCore import QPoint, QSize, Qt, Signal
 from qtpy.QtGui import QFontMetrics, QValidator
 from qtpy.QtWidgets import (
@@ -13,15 +14,16 @@
     QSpinBox,
     QStyle,
     QStyleOptionSpinBox,
     QVBoxLayout,
     QWidget,
 )
 
-from ..utils import signals_blocked
+from superqt.utils import signals_blocked
+
 from ._sliders import QDoubleRangeSlider, QDoubleSlider, QRangeSlider
 
 
 class LabelPosition(IntEnum):
     NoLabel = 0
     LabelsAbove = 1
     LabelsBelow = 2
@@ -125,14 +127,17 @@
     _slider_class = QSlider
     _slider: QSlider
 
     def __init__(self, *args, **kwargs) -> None:
         parent, orientation = _handle_overloaded_slider_sig(args, kwargs)
 
         super().__init__(parent)
+        # accept focus events
+        fp = self.style().styleHint(QStyle.StyleHint.SH_Button_FocusPolicy)
+        self.setFocusPolicy(Qt.FocusPolicy(fp))
 
         self._slider = self._slider_class()
         self._label = SliderLabel(self._slider, connect=self._setValue)
         self._edge_label_mode: EdgeLabelMode = EdgeLabelMode.LabelIsValue
 
         self._rename_signals()
         self._slider.actionTriggered.connect(self.actionTriggered.emit)
@@ -215,14 +220,18 @@
     _fsliderMoved = Signal(float)
     _frangeChanged = Signal(float, float)
 
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
         self.setDecimals(2)
 
+    def _setValue(self, value: float):
+        """Convert the value from float to int before setting the slider value."""
+        self._slider.setValue(value)
+
     def _rename_signals(self):
         self.valueChanged = self._fvalueChanged
         self.sliderMoved = self._fsliderMoved
         self.rangeChanged = self._frangeChanged
 
     def decimals(self) -> int:
         return self._label.decimals()
@@ -561,18 +570,16 @@
     def setMode(self, opt: EdgeLabelMode):
         # when the edge labels are controlling slider range,
         # we want them to have a big range, but not have a huge label
         self._mode = opt
         if opt == EdgeLabelMode.LabelIsRange:
             self.setMinimum(-9999999)
             self.setMaximum(9999999)
-            try:
+            with contextlib.suppress(Exception):
                 self._slider.rangeChanged.disconnect(self.setRange)
-            except Exception:
-                pass
         else:
             self.setMinimum(self._slider.minimum())
             self.setMaximum(self._slider.maximum())
             self._slider.rangeChanged.connect(self.setRange)
         self._update_size()
 
     def validate(self, input: str, pos: int):
```

### Comparing `superqt-0.4.1/src/superqt/sliders/_range_style.py` & `superqt-0.5.0/src/superqt/sliders/_range_style.py`

 * *Files 0% similar despite different names*

```diff
@@ -256,15 +256,14 @@
         return grad
 
     # fallback to dark gray
     return QColor(getattr(SYSTEM_STYLE, default_attr))
 
 
 def update_styles_from_stylesheet(obj: _GenericRangeSlider):
-
     qss: str = obj.styleSheet()
 
     parent = obj.parent()
     while parent is not None:
         qss = parent.styleSheet() + qss
         parent = parent.parent()
     qss = QApplication.instance().styleSheet() + qss
```

### Comparing `superqt-0.4.1/src/superqt/sliders/_sliders.py` & `superqt-0.5.0/src/superqt/sliders/_sliders.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,19 +23,19 @@
         self._singleStep = 0.01
         self._pageStep = 0.1
 
     def _type_cast(self, value) -> float:
         return float(value)
 
 
-class QDoubleSlider(_FloatMixin, _GenericSlider[float]):
+class QDoubleSlider(_FloatMixin, _GenericSlider):
     pass
 
 
-class QIntSlider(_IntMixin, _GenericSlider[int]):
+class QIntSlider(_IntMixin, _GenericSlider):
     # mostly just an example... use QSlider instead.
     valueChanged = Signal(int)
 
 
 class QRangeSlider(_IntMixin, _GenericRangeSlider):
     pass
```

### Comparing `superqt-0.4.1/src/superqt/spinbox/_intspin.py` & `superqt-0.5.0/src/superqt/spinbox/_intspin.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import math
 from enum import Enum
 
 from qtpy.QtCore import QSize, Qt, Signal
 from qtpy.QtGui import QFontMetrics, QValidator
 from qtpy.QtWidgets import QAbstractSpinBox, QStyle, QStyleOptionSpinBox
 
 
@@ -38,14 +39,17 @@
 
     def __init__(self, parent=None) -> None:
         super().__init__(parent)
         self._value: int = 0
         self._minimum: int = 0
         self._maximum: int = 2**64 - 1
         self._single_step: int = 1
+        self._step_type: QAbstractSpinBox.StepType = (
+            QAbstractSpinBox.StepType.DefaultStepType
+        )
         self._pending_emit = False
         validator = _AnyIntValidator(self)
         self.lineEdit().setValidator(validator)
         self.lineEdit().textChanged.connect(self._editor_text_changed)
         self.setValue(0)
 
     # ###############  Public Functions  #######################
@@ -74,15 +78,21 @@
 
     def singleStep(self):
         return self._single_step
 
     def setSingleStep(self, step):
         self._single_step = int(step)
 
-    # TODO: add prefix/suffix/stepType
+    def setStepType(self, stepType: QAbstractSpinBox.StepType) -> None:
+        self._step_type = stepType
+
+    def stepType(self) -> QAbstractSpinBox.StepType:
+        return self._step_type
+
+    # TODO: add prefix/suffix
 
     # ###############  QtOverrides  #######################
 
     def focusOutEvent(self, e) -> None:
         if self._pending_emit:
             self._interpret(_EmitPolicy.EmitIfChanged)
         return super().focusOutEvent(e)
@@ -98,21 +108,24 @@
                 _EmitPolicy.AlwaysEmit
                 if self.keyboardTracking()
                 else _EmitPolicy.EmitIfChanged
             )
         return super().keyPressEvent(e)
 
     def stepBy(self, steps: int) -> None:
-        step = self._single_step
         old = self._value
         e = _EmitPolicy.EmitIfChanged
         if self._pending_emit:
             self._interpret(_EmitPolicy.NeverEmit)
             if self._value != old:
                 e = _EmitPolicy.AlwaysEmit
+        if self._step_type == QAbstractSpinBox.StepType.AdaptiveDecimalStepType:
+            step = self._calculate_adaptive_decimal_step(steps)
+        else:
+            step = self._single_step
         self._setValue(self._bound(self._value + (step * steps)), e)
 
     def stepEnabled(self):
         flags = QAbstractSpinBox.StepEnabledFlag.StepNone
         if self.isReadOnly():
             return flags
         if self._value < self._maximum:
@@ -160,17 +173,32 @@
         self.lineEdit().setText(new_text)
 
     def _interpret(self, policy):
         text = self.lineEdit().displayText() or str(self._value)
         v = int(text)
         self._setValue(v, policy)
 
-    def _editor_text_changed(self, t):
+    def _editor_text_changed(self, t: str) -> None:
         if self.keyboardTracking():
-            self._setValue(int(t), _EmitPolicy.EmitIfChanged)
+            try:
+                self._setValue(int(t), _EmitPolicy.EmitIfChanged)
+            except ValueError:
+                pass
             self.lineEdit().setFocus()
             self._pending_emit = False
         else:
             self._pending_emit = True
 
     def _bound(self, value):
         return max(self._minimum, min(self._maximum, value))
+
+    def _calculate_adaptive_decimal_step(self, steps: int) -> int:
+        abs_value = abs(self._value)
+        if abs_value < 100:
+            return 1
+
+        value_negative = self._value < 0
+        steps_negative = steps < 0
+        sign_compensation = 0 if value_negative == steps_negative else 1
+
+        log = int(math.log10(abs_value - sign_compensation)) - 1
+        return int(math.pow(10, log))
```

### Comparing `superqt-0.4.1/src/superqt/spinbox/_quantity.py` & `superqt-0.5.0/src/superqt/spinbox/_quantity.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     raise ImportError(
         "pint is required to use QQuantity.  Install it with `pip install pint`"
     ) from e
 
 from qtpy.QtCore import Signal
 from qtpy.QtWidgets import QComboBox, QDoubleSpinBox, QHBoxLayout, QSizePolicy, QWidget
 
-from ..utils import signals_blocked
+from superqt.utils import signals_blocked
 
 if TYPE_CHECKING:
     from decimal import Decimal
 
 
 Number = Union[int, float, "Decimal"]
 UREG = UnitRegistry()
@@ -74,15 +74,18 @@
         ureg: Optional[UnitRegistry] = None,
         parent: Optional[QWidget] = None,
     ) -> None:
         super().__init__(parent=parent)
         if ureg is None:
             ureg = value._REGISTRY if isinstance(value, Quantity) else UREG
         else:
-            assert isinstance(ureg, UnitRegistry)
+            if not isinstance(ureg, UnitRegistry):
+                raise TypeError(
+                    f"ureg must be a pint.UnitRegistry, not {type(ureg).__name__}"
+                )
 
         self._ureg = ureg
         self._value: Quantity = self._ureg.Quantity(value, units=units)
 
         # whether to preserve quantity equality when changing units or magnitude
         self._preserve_quantity: bool = False
         self._abbreviate_units: bool = True  # TODO: implement
```

### Comparing `superqt-0.4.1/src/superqt/utils/__init__.py` & `superqt-0.5.0/src/superqt/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `superqt-0.4.1/src/superqt/utils/_code_syntax_highlight.py` & `superqt-0.5.0/src/superqt/utils/_code_syntax_highlight.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,14 +75,14 @@
 
         enters = sum(1 for _ in takewhile(lambda x: x == "\n", text_))
         # pygments lexer ignore leading empty lines, so we need to do correction
         # here calculating the number of empty lines.
 
         # dirty, dirty hack
         # The core problem is that pygemnts by default use string streams,
-        # that will not handle QTextCharFormat, so wee need use `data` property to
+        # that will not handle QTextCharFormat, so we need use `data` property to
         # work around this.
         for i in range(len(text)):
             try:
                 self.setFormat(i, 1, self.formatter.data[p + i - enters])
             except IndexError:  # pragma: no cover
                 pass
```

### Comparing `superqt-0.4.1/src/superqt/utils/_ensure_thread.py` & `superqt-0.5.0/src/superqt/utils/_ensure_thread.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # https://gist.github.com/FlorianRhiem/41a1ad9b694c14fb9ac3
 from __future__ import annotations
 
 from concurrent.futures import Future
 from functools import wraps
-from typing import TYPE_CHECKING, Callable, overload
+from typing import TYPE_CHECKING, Callable, ClassVar, overload
 
 from qtpy.QtCore import (
     QCoreApplication,
     QMetaObject,
     QObject,
     Qt,
     QThread,
@@ -22,15 +22,15 @@
 
     P = ParamSpec("P")
     R = TypeVar("R")
 
 
 class CallCallable(QObject):
     finished = Signal(object)
-    instances: list[CallCallable] = []
+    instances: ClassVar[list[CallCallable]] = []
 
     def __init__(self, callable, *args, **kwargs):
         super().__init__()
         self._callable = callable
         self._args = args
         self._kwargs = kwargs
         CallCallable.instances.append(self)
```

### Comparing `superqt-0.4.1/src/superqt/utils/_message_handler.py` & `superqt-0.5.0/src/superqt/utils/_message_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+from __future__ import annotations
+
 import logging
 from contextlib import suppress
-from typing import List, NamedTuple, Optional
+from typing import ClassVar, NamedTuple
 
 from qtpy.QtCore import QMessageLogContext, QtMsgType, qInstallMessageHandler
 
 
 class Record(NamedTuple):
     level: int
     message: str
@@ -35,27 +37,27 @@
     ...     ...
 
     >>> logger = logging.getLogger(__name__)
     >>> with QMessageHandler(logger):  # re-reoute Qt messages to a python logger.
     ...    ...
     """
 
-    _qt2loggertype = {
+    _qt2loggertype: ClassVar[dict[QtMsgType, int]] = {
         QtMsgType.QtDebugMsg: logging.DEBUG,
         QtMsgType.QtInfoMsg: logging.INFO,
         QtMsgType.QtWarningMsg: logging.WARNING,
         QtMsgType.QtCriticalMsg: logging.ERROR,  # note
         QtMsgType.QtFatalMsg: logging.CRITICAL,  # note
         QtMsgType.QtSystemMsg: logging.CRITICAL,
     }
 
-    def __init__(self, logger: Optional[logging.Logger] = None):
-        self.records: List[Record] = []
+    def __init__(self, logger: logging.Logger | None = None):
+        self.records: list[Record] = []
         self._logger = logger
-        self._previous_handler: Optional[object] = "__uninstalled__"
+        self._previous_handler: object | None = "__uninstalled__"
 
     def install(self):
         """Install this handler (override the current QtMessageHandler)."""
         self._previous_handler = qInstallMessageHandler(self)
 
     def uninstall(self):
         """Uninstall this handler, restoring the previous handler."""
```

### Comparing `superqt-0.4.1/src/superqt/utils/_qthreading.py` & `superqt-0.5.0/src/superqt/utils/_qthreading.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import time
 import warnings
 from functools import partial, wraps
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
+    ClassVar,
     Generator,
     Generic,
     Sequence,
     TypeVar,
     overload,
 )
 
@@ -60,18 +61,17 @@
         yield
         return func(*args, **kwargs)
 
     return genwrapper
 
 
 class WorkerBaseSignals(QObject):
-
     started = Signal()  # emitted when the work is started
     finished = Signal()  # emitted when the work is finished
-    _finished = Signal(object)  # emitted when the work is finished ro delete
+    _finished = Signal(object)  # emitted when the work is finished to delete
     returned = Signal(object)  # emitted with return value
     errored = Signal(object)  # emitted with error object on Exception
     warned = Signal(tuple)  # emitted with showwarning args on warning
 
 
 class WorkerBase(QRunnable, Generic[_R]):
     """Base class for creating a Worker that can run in another thread.
@@ -84,15 +84,15 @@
     Attributes
     ----------
     signals: WorkerBaseSignals
         signal emitter object. To allow identify which worker thread emitted signal.
     """
 
     #: A set of Workers.  Add to set using `WorkerBase.start`
-    _worker_set: set[WorkerBase] = set()
+    _worker_set: ClassVar[set[WorkerBase]] = set()
     returned: SigInst[_R]
     errored: SigInst[Exception]
     warned: SigInst[tuple]
     started: SigInst[None]
     finished: SigInst[None]
 
     def __init__(
@@ -181,14 +181,15 @@
                     # The Worker object has likely been deleted.
                     # A deleted wrapped C/C++ object may result in a runtime
                     # error that will cause segfault if we try to do much other
                     # than simply notify the user.
                     warnings.warn(
                         f"RuntimeError in aborted thread: {result}",
                         RuntimeWarning,
+                        stacklevel=2,
                     )
                     return
                 else:
                     raise result
             if not self.abort_requested:
                 self.returned.emit(result)
         except Exception as exc:
@@ -354,15 +355,14 @@
         self._kwargs = kwargs
 
     def work(self) -> _R:
         return self._func(*self._args, **self._kwargs)
 
 
 class GeneratorWorkerSignals(WorkerBaseSignals):
-
     yielded = Signal(object)  # emitted with yielded values (if generator used)
     paused = Signal()  # emitted when a running job has successfully paused
     resumed = Signal()  # emitted when a paused job has successfully resumed
     aborted = Signal()  # emitted when a running job is successfully aborted
 
 
 class GeneratorWorker(WorkerBase, Generic[_Y, _S, _R]):
```

### Comparing `superqt-0.4.1/src/superqt/utils/_throttler.py` & `superqt-0.5.0/src/superqt/utils/_throttler.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,14 @@
 
 class EmissionPolicy(IntFlag):
     Trailing = auto()
     Leading = auto()
 
 
 class GenericSignalThrottler(QObject):
-
     triggered = Signal()
     timeoutChanged = Signal(int)
     timerTypeChanged = Signal(Qt.TimerType)
 
     def __init__(
         self,
         kind: Kind,
@@ -75,15 +74,15 @@
     ) -> None:
         super().__init__(parent)
 
         self._kind = kind
         self._emissionPolicy = emissionPolicy
         self._hasPendingEmission = False
 
-        self._timer = QTimer()
+        self._timer = QTimer(parent=self)
         self._timer.setSingleShot(True)
         self._timer.setTimerType(Qt.TimerType.PreciseTimer)
         self._timer.timeout.connect(self._maybeEmitTriggered)
 
     def kind(self) -> Kind:
         """Return the kind of throttler (throttler or debouncer)."""
         return self._kind
@@ -129,16 +128,14 @@
         # (unless we get ANOTHER signal).
         if self._kind is Kind.Throttler:  # sourcery skip: merge-duplicate-blocks
             if not self._timer.isActive():
                 self._timer.start()  # actual start, not restart
         elif self._kind is Kind.Debouncer:
             self._timer.start()  # restart
 
-        assert self._timer.isActive()
-
     def cancel(self) -> None:
         """Cancel any pending emissions."""
         self._hasPendingEmission = False
 
     def flush(self) -> None:
         """Force emission of any pending emissions."""
         self._maybeEmitTriggered()
```

### Comparing `superqt-0.4.1/tests/test_code_highlight.py` & `superqt-0.5.0/tests/test_code_highlight.py`

 * *Files identical despite different names*

### Comparing `superqt-0.4.1/tests/test_collapsible.py` & `superqt-0.5.0/tests/test_collapsible.py`

 * *Files identical despite different names*

### Comparing `superqt-0.4.1/tests/test_eliding_label.py` & `superqt-0.5.0/tests/test_eliding_label.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,22 +27,22 @@
 
 
 def test_wrapped_eliding_label(qtbot):
     wdg = QElidingLabel(TEXT)
     qtbot.addWidget(wdg)
     assert not wdg.wordWrap()
     assert 630 < wdg.sizeHint().width() < 640
-    assert wdg._elidedText().endswith("…")
+    assert wdg._elidedText().endswith(ELLIPSIS)
     wdg.resize(QSize(200, 100))
     assert wdg.text() == TEXT
-    assert wdg._elidedText().endswith("…")
+    assert wdg._elidedText().endswith(ELLIPSIS)
     wdg.setWordWrap(True)
     assert wdg.wordWrap()
     assert wdg.text() == TEXT
-    assert wdg._elidedText().endswith("…")
+    assert wdg._elidedText().endswith(ELLIPSIS)
     # just empirically from CI ... stupid
     if platform.system() == "Linux":
         assert wdg.sizeHint() in (QSize(200, 198), QSize(200, 154))
     elif platform.system() == "Windows":
         assert wdg.sizeHint() in (QSize(200, 160), QSize(200, 118))
     elif platform.system() == "Darwin":
         assert wdg.sizeHint() == QSize(200, 176)
```

### Comparing `superqt-0.4.1/tests/test_ensure_thread.py` & `superqt-0.5.0/tests/test_ensure_thread.py`

 * *Files 4% similar despite different names*

```diff
@@ -154,16 +154,16 @@
     assert (
         ob.check_object_thread_return_future.__name__
         == "check_object_thread_return_future"
     )
     assert ob.check_object_thread_return_future.__doc__ == "sample docstring"
     signature = inspect.signature(ob.check_object_thread_return_future)
     assert len(signature.parameters) == 1
-    assert list(signature.parameters.values())[0].name == "a"
-    assert list(signature.parameters.values())[0].annotation == int
+    assert next(iter(signature.parameters.values())).name == "a"
+    assert next(iter(signature.parameters.values())).annotation == int
     assert ob.check_main_thread_return.__name__ == "check_main_thread_return"
 
 
 @skip_on_ci
 def test_object_thread_return(qtbot):
     ob = SampleObject()
     thread = QThread()
```

### Comparing `superqt-0.4.1/tests/test_enum_comb_box.py` & `superqt-0.5.0/tests/test_enum_comb_box.py`

 * *Files identical despite different names*

### Comparing `superqt-0.4.1/tests/test_large_int_spinbox.py` & `superqt-0.5.0/tests/test_large_int_spinbox.py`

 * *Files 17% similar despite different names*

```diff
@@ -68,7 +68,20 @@
     assert sb._pending_emit is False
 
     sb.setKeyboardTracking(True)
     with qtbot.waitSignal(sb.valueChanged) as sgnl:
         sb.lineEdit().setText("25")
     assert sb._pending_emit is False
     assert sgnl.args == [25]
+
+
+def test_large_spinbox_step_type(qtbot):
+    sb = QLargeIntSpinBox()
+    qtbot.addWidget(sb)
+    sb.setMaximum(1_000_000_000)
+    sb.setStepType(sb.StepType.AdaptiveDecimalStepType)
+    sb.setValue(1_000_000)
+    sb.stepBy(1)
+    assert sb.value() == 1_100_000
+    sb.setStepType(sb.StepType.DefaultStepType)
+    sb.stepBy(1)
+    assert sb.value() == 1_100_001
```

### Comparing `superqt-0.4.1/tests/test_qmessage_handler.py` & `superqt-0.5.0/tests/test_qmessage_handler.py`

 * *Files identical despite different names*

### Comparing `superqt-0.4.1/tests/test_quantity.py` & `superqt-0.5.0/tests/test_quantity.py`

 * *Files identical despite different names*

### Comparing `superqt-0.4.1/tests/test_searchable_combobox.py` & `superqt-0.5.0/tests/test_searchable_combobox.py`

 * *Files identical despite different names*

### Comparing `superqt-0.4.1/tests/test_searchable_list.py` & `superqt-0.5.0/tests/test_searchable_list.py`

 * *Files identical despite different names*

### Comparing `superqt-0.4.1/tests/test_threadworker.py` & `superqt-0.5.0/tests/test_threadworker.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,17 +94,17 @@
 
     def check_warning(w):
         return str(w) == "hey!"
 
     @qthreading.thread_worker(connect={"warned": check_warning}, start_thread=False)
     def func():
         yield 1
-        warnings.warn("hey!")
+        warnings.warn("hey!")  # noqa: B028
         yield 3
-        warnings.warn("hey!")
+        warnings.warn("hey!")  # noqa: B028
         return 1
 
     wrkr = func()
     assert isinstance(wrkr, qthreading.GeneratorWorker)
 
     signals = [wrkr.yielded, wrkr.warned, wrkr.yielded, wrkr.returned]
     checks = [equals_1, None, equals_3, equals_1]
@@ -232,15 +232,15 @@
 def test_worker_base_attribute(qapp):
     obj = qthreading.WorkerBase()
     assert obj.started is not None
     assert obj.finished is not None
     assert obj.returned is not None
     assert obj.errored is not None
     with pytest.raises(AttributeError):
-        obj.aa
+        _ = obj.aa
 
 
 def test_abort_does_not_return(qtbot):
     loop_counter = 0
 
     def long_running_func():
         nonlocal loop_counter
```

### Comparing `superqt-0.4.1/tests/test_throttler.py` & `superqt-0.5.0/tests/test_throttler.py`

 * *Files identical despite different names*

### Comparing `superqt-0.4.1/tests/test_utils.py` & `superqt-0.5.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `superqt-0.4.1/tests/test_fonticon/test_fonticon.py` & `superqt-0.5.0/tests/test_fonticon/test_fonticon.py`

 * *Files identical despite different names*

### Comparing `superqt-0.4.1/tests/test_fonticon/test_plugins.py` & `superqt-0.5.0/tests/test_fonticon/test_plugins.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from superqt.fonticon._qfont_icon import QFontIconStore
 
 FIXTURES = Path(__file__).parent / "fixtures"
 
 
 @pytest.fixture
 def plugin_store(qapp, monkeypatch):
-    _path = [str(FIXTURES)] + sys.path.copy()
+    _path = [str(FIXTURES), *sys.path.copy()]
     store = QFontIconStore().instance()
     with monkeypatch.context() as m:
         m.setattr(sys, "path", _path)
         yield store
     store.clear()
```

### Comparing `superqt-0.4.1/tests/test_fonticon/fixtures/fake_plugin/icontest.ttf` & `superqt-0.5.0/tests/test_fonticon/fixtures/fake_plugin/icontest.ttf`

 * *Files identical despite different names*

### Comparing `superqt-0.4.1/tests/test_sliders/_testutil.py` & `superqt-0.5.0/tests/test_sliders/_testutil.py`

 * *Files identical despite different names*

### Comparing `superqt-0.4.1/tests/test_sliders/test_float.py` & `superqt-0.5.0/tests/test_sliders/test_float.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     cls = request.param
     wdg = cls()
     qtbot.addWidget(wdg)
 
     def assert_val_type():
         type_ = float
         if cls in range_types:
-            assert all([isinstance(i, type_) for i in wdg.value()])  # sourcery skip
+            assert all(isinstance(i, type_) for i in wdg.value())  # sourcery skip
         else:
             assert isinstance(wdg.value(), type_)
 
     def assert_val_eq(val):
         assert wdg.value() == val if cls is QDoubleRangeSlider else val[0]
 
     wdg.assert_val_type = assert_val_type
```

### Comparing `superqt-0.4.1/tests/test_sliders/test_generic_slider.py` & `superqt-0.5.0/tests/test_sliders/test_generic_slider.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,14 @@
     gslider.show()
     with qtbot.waitSignal(gslider.sliderPressed):
         qtbot.mousePress(gslider, Qt.MouseButton.LeftButton, pos=handle_pos)
 
 
 @skip_on_linux_qt6
 def test_hover(gslider: _GenericSlider):
-
     # stub
     opt = QStyleOptionSlider()
     gslider.initStyleOption(opt)
     style = gslider.style()
     hrect = style.subControlRect(
         QStyle.ComplexControl.CC_Slider, opt, QStyle.SubControl.SC_SliderHandle
     )
```

### Comparing `superqt-0.4.1/tests/test_sliders/test_labeled_slider.py` & `superqt-0.5.0/tests/test_sliders/test_labeled_slider.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
     slider._label.editingFinished.emit()
 
 
 def _assert_types(args: Iterable[Any], type_: type):
     # sourcery skip: comprehension-to-generator
     if sys.version_info >= (3, 8):
-        assert all([isinstance(v, type_) for v in args]), "invalid type"
+        assert all(isinstance(v, type_) for v in args), "invalid type"
 
 
 @pytest.mark.parametrize("cls", [QLabeledDoubleSlider, QLabeledSlider])
 def test_labeled_signals(cls, qtbot):
     gslider = cls()
     qtbot.addWidget(gslider)
 
@@ -63,16 +63,25 @@
     mock.assert_called_once_with(1, 2)
     _assert_types(mock.call_args.args, type_)
 
 
 @pytest.mark.parametrize(
     "cls", [QLabeledDoubleSlider, QLabeledRangeSlider, QLabeledSlider]
 )
-def test_editing_finished_signal(cls):
-    slider = cls()
+def test_editing_finished_signal(cls, qtbot):
     mock = Mock()
+    slider = cls()
+    qtbot.addWidget(slider)
     slider.editingFinished.connect(mock)
     if hasattr(slider, "_label"):
         slider._label.editingFinished.emit()
     else:
         slider._min_label.editingFinished.emit()
     mock.assert_called_once()
+
+
+def test_editing_float(qtbot):
+    slider = QLabeledDoubleSlider()
+    qtbot.addWidget(slider)
+    slider._label.setValue(0.5)
+    slider._label.editingFinished.emit()
+    assert slider.value() == 0.5
```

### Comparing `superqt-0.4.1/tests/test_sliders/test_range_slider.py` & `superqt-0.5.0/tests/test_sliders/test_range_slider.py`

 * *Files 0% similar despite different names*

```diff
@@ -215,15 +215,15 @@
 
     sld.wheelEvent(_wheel_event(0))
 
 
 def _assert_types(args: Iterable[Any], type_: type):
     # sourcery skip: comprehension-to-generator
     if sys.version_info >= (3, 8):
-        assert all([isinstance(v, type_) for v in args]), "invalid type"
+        assert all(isinstance(v, type_) for v in args), "invalid type"
 
 
 @pytest.mark.parametrize("cls, orientation", ALL_SLIDER_COMBOS)
 def test_rangeslider_signals(cls, orientation, qtbot):
     sld = cls(orientation)
     qtbot.addWidget(sld)
```

### Comparing `superqt-0.4.1/tests/test_sliders/test_single_value_sliders.py` & `superqt-0.5.0/tests/test_sliders/test_single_value_sliders.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,15 +150,14 @@
     sld.show()
     with qtbot.waitSignal(_real_sld.sliderPressed, timeout=300):
         qtbot.mousePress(_real_sld, Qt.MouseButton.LeftButton, pos=handle_pos)
 
 
 @skip_on_linux_qt6
 def test_hover(sld: _GenericSlider):
-
     _real_sld = getattr(sld, "_slider", sld)
 
     opt = QStyleOptionSlider()
     _real_sld.initStyleOption(opt)
     hrect = _real_sld.style().subControlRect(
         QStyle.ComplexControl.CC_Slider, opt, QStyle.SubControl.SC_SliderHandle
     )
@@ -175,15 +174,14 @@
         _hover_event(QEvent.Type.HoverLeave, QPointF(-1000, -1000), handle_pos, sld)
     )
     with suppress(AttributeError):  # for QSlider
         assert _real_sld._hoverControl == QStyle.SubControl.SC_None
 
 
 def test_wheel(sld: _GenericSlider, qtbot):
-
     if type(sld) is QLabeledSlider and QT_VERSION < (5, 12):
         pytest.skip()
 
     _real_sld = getattr(sld, "_slider", sld)
     with qtbot.waitSignal(sld.valueChanged, timeout=400):
         _real_sld.wheelEvent(_wheel_event(120))
 
@@ -196,23 +194,21 @@
 
     if type(sld) is not QLabeledSlider:
         sld.setSliderPosition(21.5)
         assert sld.sliderPosition() == 21.5
 
 
 def test_steps(sld: _GenericSlider, qtbot):
-
     sld.setSingleStep(11)
     assert sld.singleStep() == 11
 
     sld.setPageStep(16)
     assert sld.pageStep() == 16
 
     if type(sld) is not QLabeledSlider:
-
         sld.setSingleStep(0.1)
         assert sld.singleStep() == 0.1
 
         sld.setSingleStep(1.5e20)
         assert sld.singleStep() == 1.5e20
 
         sld.setPageStep(0.2)
```

### Comparing `superqt-0.4.1/tests/test_sliders/test_slider.py` & `superqt-0.5.0/tests/test_sliders/test_slider.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 import pytest
 from qtpy import API_NAME
 from qtpy.QtCore import Qt
 
 from superqt import QRangeSlider
 from superqt.sliders._generic_range_slider import SC_BAR, SC_HANDLE, SC_NONE
 
-NOT_LINUX = platform.system() != "Linux"
-NOT_PYSIDE2 = API_NAME != "PySide2"
+LINUX = platform.system() == "Linux"
+NOT_PYQT6 = API_NAME != "PyQt6"
 
-skipmouse = pytest.mark.skipif(NOT_LINUX or NOT_PYSIDE2, reason="mouse tests finicky")
+skipmouse = pytest.mark.skipif(LINUX or NOT_PYQT6, reason="mouse tests finicky")
 
 
 @pytest.mark.parametrize("orientation", ["Horizontal", "Vertical"])
 def test_basic(qtbot, orientation):
     rs = QRangeSlider(getattr(Qt.Orientation, orientation))
     qtbot.addWidget(rs)
```

### Comparing `superqt-0.4.1/.gitignore` & `superqt-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `superqt-0.4.1/LICENSE` & `superqt-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `superqt-0.4.1/README.md` & `superqt-0.5.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 <img src="https://raw.githubusercontent.com/pyapp-kit/superqt/main/docs/images/labeled_qslider.png" alt="range sliders" width=680>
 
 <img src="https://raw.githubusercontent.com/pyapp-kit/superqt/main/docs/images/labeled_range.png" alt="range sliders" width=680>
 
 ## Utilities
 
-superqt includes a number of utitlities for working with Qt, including:
+superqt includes a number of utilities for working with Qt, including:
 
 - tools and decorators for working with threads in qt.
 - `superqt.fonticon` for generating icons from font files (such as [Material Design Icons](https://materialdesignicons.com/) and [Font Awesome](https://fontawesome.com/))
 
 See the [utilities documentation](https://pyapp-kit.github.io/superqt/utilities/) for a full list of utilities.
 
 ## Contributing
```

### Comparing `superqt-0.4.1/pyproject.toml` & `superqt-0.5.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -44,42 +44,39 @@
     "qtpy>=1.1.0",
     "typing-extensions",
 ]
 
 # extras
 # https://peps.python.org/pep-0621/#dependencies-optional-dependencies
 [project.optional-dependencies]
-test = ["pint", "pytest", "pytest-cov", "pytest-qt", "tox", "tox-conda"]
+test = ["pint", "pytest", "pytest-cov", "pytest-qt"]
 dev = [
     "black",
     "ipython",
-    "isort",
-    "jedi<0.18.0",
+    "ruff",
     "mypy",
     "pdbpp",
     "pre-commit",
     "pydocstyle",
-    "pyside2",
-    "pytest-cov",
-    "pytest-qt",
-    "pytest",
     "rich",
-    "tox-conda",
-    "tox",
     "types-Pygments",
 ]
 docs = ["mkdocs-macros-plugin", "mkdocs-material", "mkdocstrings[python]"]
 quantity = ["pint"]
 pyside2 = ["pyside2"]
-pyside6 = ["pyside6"]
+# see issues surrounding usage of Generics in pyside6.5.x
+# https://github.com/pyapp-kit/superqt/pull/177
+# https://github.com/pyapp-kit/superqt/pull/164
+pyside6 = ["pyside6 !=6.5.0,!=6.5.1"]
 pyqt5 = ["pyqt5"]
 pyqt6 = ["pyqt6"]
 font-fa5 = ["fonticon-fontawesome5"]
 font-fa6 = ["fonticon-fontawesome6"]
-font-mi5 = ["fonticon-materialdesignicons5"]
+font-mi6 = ["fonticon-materialdesignicons6"]
+font-mi7 = ["fonticon-materialdesignicons7"]
 
 [project.urls]
 Source = "https://github.com/pyapp-kit/superqt"
 Tracker = "https://github.com/pyapp-kit/superqt/issues"
 Changelog = "https://github.com/pyapp-kit/superqt/blob/main/CHANGELOG.md"
 
 [tool.hatch.version]
@@ -93,45 +90,46 @@
 profile = "black"
 src_paths = ["src/superqt", "tests"]
 
 # https://github.com/charliermarsh/ruff
 [tool.ruff]
 line-length = 88
 target-version = "py37"
-src = ["src","tests"]
-extend-select = [
+src = ["src", "tests"]
+select = [
     "E",    # style errors
     "F",    # flakes
-    # "D",    # pydocstyle
-    "I001", # isort
-    "U",    # pyupgrade
-    # "N",  # pep8-naming
-    # "S",  # bandit
+    "D",    # pydocstyle
+    "I",    # isort
+    "UP",   # pyupgrade
+    "S",    # bandit
     "C",    # flake8-comprehensions
     "B",    # flake8-bugbear
     "A001", # flake8-builtins
     "RUF",  # ruff-specific rules
-    "M001", # Unused noqa directive
 ]
-extend-ignore = [
+ignore = [
     "D100", # Missing docstring in public module
+    "D101", # Missing docstring in public class
+    "D104", # Missing docstring in public package
     "D107", # Missing docstring in __init__
     "D203", # 1 blank line required before class docstring
     "D212", # Multi-line docstring summary should start at the first line
     "D213", # Multi-line docstring summary should start at the second line
+    "D401", # First line should be in imperative mood
     "D413", # Missing blank line after last section
     "D416", # Section name should end with a colon
     "C901", # Function is too complex
 ]
 
 
 [tool.ruff.per-file-ignores]
-"tests/*.py" = ["D"]
+"tests/*.py" = ["D", "S101"]
 "examples/demo_widget.py" = ["E501"]
-"examples/*.py" = ["B"]
+"examples/*.py" = ["B", "D"]
 
 # https://docs.pytest.org/en/6.2.x/customize.html
 [tool.pytest.ini_options]
 minversion = "6.0"
 testpaths = ["tests"]
 filterwarnings = [
     "error",
@@ -170,18 +168,17 @@
 
 # https://github.com/mgedmin/check-manifest#configuration
 [tool.check-manifest]
 ignore = [
     ".github_changelog_generator",
     ".pre-commit-config.yaml",
     "tests/**/*",
-    "tox.ini",
     "src/superqt/_version.py",
     "mkdocs.yml",
     "docs/**/*",
     "examples/**/*",
     "CHANGELOG.md",
     "CONTRIBUTING.md",
     "codecov.yml",
     ".ruff_cache/**/*",
-    "setup.py"
+    "setup.py",
 ]
```

### Comparing `superqt-0.4.1/PKG-INFO` & `superqt-0.5.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superqt
-Version: 0.4.1
+Version: 0.5.0
 Summary: Missing widgets and components for PyQt/PySide
 Project-URL: Source, https://github.com/pyapp-kit/superqt
 Project-URL: Tracker, https://github.com/pyapp-kit/superqt/issues
 Project-URL: Changelog, https://github.com/pyapp-kit/superqt/blob/main/CHANGELOG.md
 Author: Talley Lambert
 Author-email: talley.lambert@gmail.com
 License: BSD 3-Clause License
@@ -29,55 +29,48 @@
 Requires-Dist: packaging
 Requires-Dist: pygments>=2.4.0
 Requires-Dist: qtpy>=1.1.0
 Requires-Dist: typing-extensions
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: ipython; extra == 'dev'
-Requires-Dist: isort; extra == 'dev'
-Requires-Dist: jedi<0.18.0; extra == 'dev'
 Requires-Dist: mypy; extra == 'dev'
 Requires-Dist: pdbpp; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
 Requires-Dist: pydocstyle; extra == 'dev'
-Requires-Dist: pyside2; extra == 'dev'
-Requires-Dist: pytest; extra == 'dev'
-Requires-Dist: pytest-cov; extra == 'dev'
-Requires-Dist: pytest-qt; extra == 'dev'
 Requires-Dist: rich; extra == 'dev'
-Requires-Dist: tox; extra == 'dev'
-Requires-Dist: tox-conda; extra == 'dev'
+Requires-Dist: ruff; extra == 'dev'
 Requires-Dist: types-pygments; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: mkdocs-macros-plugin; extra == 'docs'
 Requires-Dist: mkdocs-material; extra == 'docs'
 Requires-Dist: mkdocstrings[python]; extra == 'docs'
 Provides-Extra: font-fa5
 Requires-Dist: fonticon-fontawesome5; extra == 'font-fa5'
 Provides-Extra: font-fa6
 Requires-Dist: fonticon-fontawesome6; extra == 'font-fa6'
-Provides-Extra: font-mi5
-Requires-Dist: fonticon-materialdesignicons5; extra == 'font-mi5'
+Provides-Extra: font-mi6
+Requires-Dist: fonticon-materialdesignicons6; extra == 'font-mi6'
+Provides-Extra: font-mi7
+Requires-Dist: fonticon-materialdesignicons7; extra == 'font-mi7'
 Provides-Extra: pyqt5
 Requires-Dist: pyqt5; extra == 'pyqt5'
 Provides-Extra: pyqt6
 Requires-Dist: pyqt6; extra == 'pyqt6'
 Provides-Extra: pyside2
 Requires-Dist: pyside2; extra == 'pyside2'
 Provides-Extra: pyside6
-Requires-Dist: pyside6; extra == 'pyside6'
+Requires-Dist: pyside6!=6.5.0,!=6.5.1; extra == 'pyside6'
 Provides-Extra: quantity
 Requires-Dist: pint; extra == 'quantity'
 Provides-Extra: test
 Requires-Dist: pint; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Requires-Dist: pytest-qt; extra == 'test'
-Requires-Dist: tox; extra == 'test'
-Requires-Dist: tox-conda; extra == 'test'
 Description-Content-Type: text/markdown
 
 # ![tiny](https://user-images.githubusercontent.com/1609449/120636353-8c3f3800-c43b-11eb-8732-a14dec578897.png)  superqt!
 
 [![License](https://img.shields.io/pypi/l/superqt.svg?color=green)](https://github.com/pyapp-kit/superqt/raw/master/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/superqt.svg?color=green)](https://pypi.org/project/superqt)
 [![Python
@@ -113,15 +106,15 @@
 
 <img src="https://raw.githubusercontent.com/pyapp-kit/superqt/main/docs/images/labeled_qslider.png" alt="range sliders" width=680>
 
 <img src="https://raw.githubusercontent.com/pyapp-kit/superqt/main/docs/images/labeled_range.png" alt="range sliders" width=680>
 
 ## Utilities
 
-superqt includes a number of utitlities for working with Qt, including:
+superqt includes a number of utilities for working with Qt, including:
 
 - tools and decorators for working with threads in qt.
 - `superqt.fonticon` for generating icons from font files (such as [Material Design Icons](https://materialdesignicons.com/) and [Font Awesome](https://fontawesome.com/))
 
 See the [utilities documentation](https://pyapp-kit.github.io/superqt/utilities/) for a full list of utilities.
 
 ## Contributing
```

