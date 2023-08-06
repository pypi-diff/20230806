# Comparing `tmp/lamin_utils-0.9.3.tar.gz` & `tmp/lamin_utils-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamin_utils-0.9.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "lamin_utils-0.9.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lamin_utils-0.9.3.tar` & `lamin_utils-0.9.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      977 2023-07-23 09:54:55.938805 lamin_utils-0.9.3/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-07-23 09:54:55.938918 lamin_utils-0.9.3/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2023-07-23 09:54:55.939014 lamin_utils-0.9.3/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1199 2023-07-23 09:54:55.939121 lamin_utils-0.9.3/.gitignore
--rw-r--r--   0        0        0     1798 2023-07-23 09:54:55.939232 lamin_utils-0.9.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11357 2023-07-23 09:54:55.939391 lamin_utils-0.9.3/LICENSE
--rw-r--r--   0        0        0      176 2023-07-23 09:54:55.939490 lamin_utils-0.9.3/README.md
--rw-r--r--   0        0        0     6671 2023-07-25 19:58:24.969203 lamin_utils-0.9.3/docs/changelog.md
--rw-r--r--   0        0        0     1359 2023-07-23 14:46:35.798941 lamin_utils-0.9.3/docs/quickstart.ipynb
--rw-r--r--   0        0        0      149 2023-07-23 09:54:55.939845 lamin_utils-0.9.3/lamin-project.yaml
--rw-r--r--   0        0        0      161 2023-07-25 19:58:18.819710 lamin_utils-0.9.3/lamin_utils/__init__.py
--rw-r--r--   0        0        0     1632 2023-07-25 14:09:10.077910 lamin_utils-0.9.3/lamin_utils/_core.py
--rw-r--r--   0        0        0     3825 2023-07-23 09:54:55.940185 lamin_utils-0.9.3/lamin_utils/_inspect.py
--rw-r--r--   0        0        0     7393 2023-07-23 09:54:55.940290 lamin_utils-0.9.3/lamin_utils/_logger.py
--rw-r--r--   0        0        0     4282 2023-07-23 14:49:00.466496 lamin_utils-0.9.3/lamin_utils/_lookup.py
--rw-r--r--   0        0        0     7526 2023-07-25 19:58:03.772477 lamin_utils-0.9.3/lamin_utils/_map_synonyms.py
--rw-r--r--   0        0        0      683 2023-07-23 09:54:55.940588 lamin_utils-0.9.3/lamin_utils/_python_version.py
--rw-r--r--   0        0        0     3609 2023-07-23 09:54:55.940683 lamin_utils-0.9.3/lamin_utils/_search.py
--rw-r--r--   0        0        0      285 2023-07-23 09:54:55.940763 lamin_utils-0.9.3/noxfile.py
--rw-r--r--   0        0        0      896 2023-07-23 09:54:55.940837 lamin_utils-0.9.3/pyproject.toml
--rw-r--r--   0        0        0      114 2023-07-23 09:54:55.940955 lamin_utils-0.9.3/tests/test_base.py
--rw-r--r--   0        0        0     4153 2023-07-23 09:54:55.941046 lamin_utils-0.9.3/tests/test_inspect.py
--rw-r--r--   0        0        0     1607 2023-07-23 09:54:55.941146 lamin_utils-0.9.3/tests/test_lookup.py
--rw-r--r--   0        0        0     6152 2023-07-23 09:54:55.941242 lamin_utils-0.9.3/tests/test_map_synonyms.py
--rw-r--r--   0        0        0      417 2023-07-23 09:54:55.941327 lamin_utils-0.9.3/tests/test_notebooks.py
--rw-r--r--   0        0        0     2449 2023-07-23 09:54:55.941414 lamin_utils-0.9.3/tests/test_search.py
--rw-r--r--   0        0        0     1031 1970-01-01 00:00:00.000000 lamin_utils-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0      977 2023-07-23 09:54:55.938805 lamin_utils-0.9.4/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-07-23 09:54:55.938918 lamin_utils-0.9.4/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-07-23 09:54:55.939014 lamin_utils-0.9.4/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1199 2023-07-23 09:54:55.939121 lamin_utils-0.9.4/.gitignore
+-rw-r--r--   0        0        0     1798 2023-07-23 09:54:55.939232 lamin_utils-0.9.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11357 2023-07-23 09:54:55.939391 lamin_utils-0.9.4/LICENSE
+-rw-r--r--   0        0        0      176 2023-07-23 09:54:55.939490 lamin_utils-0.9.4/README.md
+-rw-r--r--   0        0        0     7124 2023-08-06 15:33:52.714340 lamin_utils-0.9.4/docs/changelog.md
+-rw-r--r--   0        0        0     1359 2023-07-23 14:46:35.798941 lamin_utils-0.9.4/docs/quickstart.ipynb
+-rw-r--r--   0        0        0      149 2023-07-23 09:54:55.939845 lamin_utils-0.9.4/lamin-project.yaml
+-rw-r--r--   0        0        0      161 2023-08-06 15:33:43.830821 lamin_utils-0.9.4/lamin_utils/__init__.py
+-rw-r--r--   0        0        0     1632 2023-07-25 14:09:10.077910 lamin_utils-0.9.4/lamin_utils/_core.py
+-rw-r--r--   0        0        0     4971 2023-08-06 15:33:10.092855 lamin_utils-0.9.4/lamin_utils/_inspect.py
+-rw-r--r--   0        0        0     7411 2023-08-06 15:33:10.093172 lamin_utils-0.9.4/lamin_utils/_logger.py
+-rw-r--r--   0        0        0     4282 2023-07-23 14:49:00.466496 lamin_utils-0.9.4/lamin_utils/_lookup.py
+-rw-r--r--   0        0        0     6843 2023-08-06 15:33:10.093571 lamin_utils-0.9.4/lamin_utils/_map_synonyms.py
+-rw-r--r--   0        0        0      683 2023-07-23 09:54:55.940588 lamin_utils-0.9.4/lamin_utils/_python_version.py
+-rw-r--r--   0        0        0     3609 2023-07-23 09:54:55.940683 lamin_utils-0.9.4/lamin_utils/_search.py
+-rw-r--r--   0        0        0      285 2023-07-23 09:54:55.940763 lamin_utils-0.9.4/noxfile.py
+-rw-r--r--   0        0        0      896 2023-07-23 09:54:55.940837 lamin_utils-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0      114 2023-07-23 09:54:55.940955 lamin_utils-0.9.4/tests/test_base.py
+-rw-r--r--   0        0        0     4574 2023-08-06 15:33:10.093958 lamin_utils-0.9.4/tests/test_inspect.py
+-rw-r--r--   0        0        0     1607 2023-07-23 09:54:55.941146 lamin_utils-0.9.4/tests/test_lookup.py
+-rw-r--r--   0        0        0     5560 2023-08-06 15:33:10.094251 lamin_utils-0.9.4/tests/test_map_synonyms.py
+-rw-r--r--   0        0        0      417 2023-07-23 09:54:55.941327 lamin_utils-0.9.4/tests/test_notebooks.py
+-rw-r--r--   0        0        0     2449 2023-07-23 09:54:55.941414 lamin_utils-0.9.4/tests/test_search.py
+-rw-r--r--   0        0        0     1031 1970-01-01 00:00:00.000000 lamin_utils-0.9.4/PKG-INFO
```

### Comparing `lamin_utils-0.9.3/.github/workflows/build.yml` & `lamin_utils-0.9.4/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lamin_utils-0.9.3/.github/workflows/latest-changes.yml` & `lamin_utils-0.9.4/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lamin_utils-0.9.3/.gitignore` & `lamin_utils-0.9.4/.gitignore`

 * *Files identical despite different names*

### Comparing `lamin_utils-0.9.3/.pre-commit-config.yaml` & `lamin_utils-0.9.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lamin_utils-0.9.3/LICENSE` & `lamin_utils-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lamin_utils-0.9.3/docs/changelog.md` & `lamin_utils-0.9.4/docs/changelog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+🎨 Simplified params in inspect | [48](https://github.com/laminlabs/lamin-utils/pull/48) | [sunnyosun](https://github.com/sunnyosun) | 2023-08-06 | 0.9.4
+🚸 Introduce success-level verbosity | [49](https://github.com/laminlabs/lamin-utils/pull/49) | [falexwolf](https://github.com/falexwolf) | 2023-08-06 |
+Round percentages for mapping | [47](https://github.com/laminlabs/lamin-utils/pull/47) | [Zethson](https://github.com/Zethson) | 2023-07-31 |
 🐛 Fix for categorical index | [45](https://github.com/laminlabs/lamin-utils/pull/45) | [sunnyosun](https://github.com/sunnyosun) | 2023-07-25 | 0.9.3
 ✨ Added italic and underline | [44](https://github.com/laminlabs/lamin-utils/pull/44) | [sunnyosun](https://github.com/sunnyosun) | 2023-07-25 | 0.9.2
 🐛 Fix _append_records_to_list in lookup | [43](https://github.com/laminlabs/lamin-utils/pull/43) | [sunnyosun](https://github.com/sunnyosun) | 2023-07-23 |
 ✨ Allow indenting logging messages | [42](https://github.com/laminlabs/lamin-utils/pull/42) | [falexwolf](https://github.com/falexwolf) | 2023-07-21 | 0.9.0
 💚 Fix | [41](https://github.com/laminlabs/lamin-utils/pull/41) | [falexwolf](https://github.com/falexwolf) | 2023-07-21 |
 🚚 Rename `lamin_logger` to `lamin_utils` | [40](https://github.com/laminlabs/lamin-utils/pull/40) | [falexwolf](https://github.com/falexwolf) | 2023-07-21 |
 🎨 Fix for duplicated values in search | [39](https://github.com/laminlabs/lamin-logger/pull/39) | [sunnyosun](https://github.com/sunnyosun) | 2023-07-19 |
```

### Comparing `lamin_utils-0.9.3/docs/quickstart.ipynb` & `lamin_utils-0.9.4/docs/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `lamin_utils-0.9.3/lamin_utils/_core.py` & `lamin_utils-0.9.4/lamin_utils/_core.py`

 * *Files identical despite different names*

### Comparing `lamin_utils-0.9.3/lamin_utils/_logger.py` & `lamin_utils-0.9.4/lamin_utils/_logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,17 +43,18 @@
 logging.addLevelName(HINT, "HINT")
 logging.addLevelName(DOWNLOAD, "DOWNLOAD")
 logging.addLevelName(SUCCESS, "SUCCESS")
 
 VERBOSITY_TO_LOGLEVEL = {
     0: "ERROR",
     1: "WARNING",
-    2: "INFO",
-    3: "HINT",
-    4: "DEBUG",
+    2: "SUCCESS",
+    3: "INFO",
+    4: "HINT",
+    5: "DEBUG",
 }
 
 
 LEVEL_TO_ICONS = {
     40: "❌",  # error
     30: "🔶",  # warning
     25: "✅",  # success
```

### Comparing `lamin_utils-0.9.3/lamin_utils/_lookup.py` & `lamin_utils-0.9.4/lamin_utils/_lookup.py`

 * *Files identical despite different names*

### Comparing `lamin_utils-0.9.3/lamin_utils/_map_synonyms.py` & `lamin_utils-0.9.4/lamin_utils/_map_synonyms.py`

 * *Files 11% similar despite different names*

```diff
@@ -94,15 +94,15 @@
 
     if return_mapper:
         # only returns mapped synonyms
         mapper = mapped[~mapped.isna()].to_dict()
         mapper = {k: v for k, v in mapper.items() if k != v}
         if keep is False:
             logger.warning(
-                "Retuning mapper might contain lists as values when 'keep=False'"
+                "Returning mapper might contain lists as values when 'keep=False'"
             )
             return {k: v[0] if len(v) == 1 else v for k, v in mapper.items()}
         else:
             return mapper
     else:
         # returns a list in the input order with synonyms replaced
         mapped_list = mapped.fillna(mapped_df["orig_ids"]).tolist()
@@ -130,34 +130,14 @@
     else:
         values = identifiers.fillna("")
     if case_sensitive is False:
         values = values.str.lower()
     return values
 
 
-def check_if_ids_in_field_values(
-    identifiers: Iterable, field_values: Iterable, case_sensitive: bool = False
-) -> Any:
-    """Check if an iterable is in a list of values with case sensitive option."""
-    import pandas as pd
-
-    mapped_df = pd.DataFrame(index=identifiers)
-    mapped_df.index = to_str(mapped_df.index, case_sensitive=case_sensitive)
-
-    field_values = to_str(field_values, case_sensitive=case_sensitive)
-
-    # annotated what complies with the default ID
-    matches = mapped_df.index.isin(field_values)
-    mapped_df["__mapped__"] = matches
-
-    # make sure to convert back to the original identifiers
-    mapped_df.index = identifiers
-    return mapped_df
-
-
 def not_empty_none_na(values: Iterable):
     """Return values that are not empty string, None or NA."""
     import pandas as pd
 
     if not isinstance(values, (pd.Series, pd.Index)):
         values = pd.Series(values)
```

### Comparing `lamin_utils-0.9.3/lamin_utils/_python_version.py` & `lamin_utils-0.9.4/lamin_utils/_python_version.py`

 * *Files identical despite different names*

### Comparing `lamin_utils-0.9.3/lamin_utils/_search.py` & `lamin_utils-0.9.4/lamin_utils/_search.py`

 * *Files identical despite different names*

### Comparing `lamin_utils-0.9.3/pyproject.toml` & `lamin_utils-0.9.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lamin_utils-0.9.3/tests/test_inspect.py` & `lamin_utils-0.9.4/tests/test_inspect.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pandas as pd
 import pytest
 
-from lamin_utils._inspect import inspect
+from lamin_utils._inspect import inspect, validate
 
 
 @pytest.fixture(scope="module")
 def genes():
     data = {
         "gene symbol": ["A1CF", "A1BG", "FANCD1", "corrupted"],
         "hgnc id": ["HGNC:24086", "HGNC:5", "HGNC:1101", "corrupted"],
@@ -44,40 +44,40 @@
 
 
 def test_inspect_iterable(genes):
     df, data = genes
 
     mapping = inspect(df=df, identifiers=data.index, field="ensembl_gene_id")
     assert mapping == {
-        "mapped": ["ENSG00000148584", "ENSG00000121410", "ENSG00000188389"],
-        "not_mapped": ["ENSG0000corrupted"],
+        "validated": ["ENSG00000148584", "ENSG00000121410", "ENSG00000188389"],
+        "not_validated": ["ENSG0000corrupted"],
     }
 
     mapping = inspect(df=df, identifiers=data["hgnc id"], field="hgnc_id")
     assert mapping == {
-        "mapped": ["HGNC:24086", "HGNC:5", "HGNC:1101"],
-        "not_mapped": ["corrupted"],
+        "validated": ["HGNC:24086", "HGNC:5", "HGNC:1101"],
+        "not_validated": ["corrupted"],
     }
 
 
 def test_inspect_inspect_synonyms(genes):
     df, data = genes
 
     mapping = inspect(df=df, identifiers=data["gene symbol"], field="symbol")
     assert mapping == {
-        "mapped": ["A1CF", "A1BG"],
-        "not_mapped": ["FANCD1", "corrupted"],
+        "validated": ["A1CF", "A1BG"],
+        "not_validated": ["FANCD1", "corrupted"],
     }
 
     mapping = inspect(
         df=df, identifiers=data["gene symbol"], field="symbol", inspect_synonyms=False
     )
     assert mapping == {
-        "mapped": ["A1CF", "A1BG"],
-        "not_mapped": ["FANCD1", "corrupted"],
+        "validated": ["A1CF", "A1BG"],
+        "not_validated": ["FANCD1", "corrupted"],
     }
 
     df = df.drop(columns=["synonyms"])
     mapping = inspect(df=df, identifiers=data["gene symbol"], field="symbol")
 
 
 def test_inspect_return_df(genes):
@@ -91,66 +91,82 @@
         index=[
             "ENSG00000148584",
             "ENSG00000121410",
             "ENSG00000188389",
             "ENSG0000corrupted",
         ],
         data={
-            "__mapped__": [True, True, True, False],
+            "__validated__": [True, True, True, False],
         },
     )
 
     assert mapping.equals(expected_df)
 
 
 def test_inspect_case_sensitive(genes):
     df, _ = genes
 
-    mapping = inspect(df=df, identifiers=["A1CF", "A1BG", "a1cf"], field="symbol")
-    assert mapping == {"mapped": ["A1CF", "A1BG", "a1cf"], "not_mapped": []}
-
     mapping = inspect(
         df=df, identifiers=["A1CF", "A1BG", "a1cf"], field="symbol", case_sensitive=True
     )
-    assert mapping == {"mapped": ["A1CF", "A1BG"], "not_mapped": ["a1cf"]}
+    assert mapping == {"validated": ["A1CF", "A1BG"], "not_validated": ["a1cf"]}
 
 
 def test_inspect_empty_dup_input(genes):
     import numpy as np
 
     df, _ = genes
 
     mapping = inspect(
         df=df,
         identifiers=pd.Series(["A1CF", "A1BG", "A1BG", "", None, np.nan]),
         field="symbol",
     )
-    assert mapping == {"mapped": ["A1CF", "A1BG"], "not_mapped": []}
+    assert mapping == {"validated": ["A1CF", "A1BG"], "not_validated": []}
 
 
 def test_inspect_empty_df():
     import numpy as np
     import pandas as pd
 
     mapping = inspect(
         df=pd.DataFrame(),
         identifiers=pd.Series(["A1CF", "A1BG", "A1BG", "", None, np.nan]),
         field="symbol",
     )
 
-    assert mapping == {"mapped": [], "not_mapped": ["A1CF", "A1BG"]}
+    assert mapping == {"validated": [], "not_validated": ["A1CF", "A1BG"]}
 
     mapping = inspect(
         df=pd.DataFrame(),
         identifiers=pd.Series(["A1CF", "A1BG", "A1BG", "", None, np.nan]),
         field="symbol",
         return_df=True,
     )
 
     expected_df = pd.DataFrame(
         index=["A1CF", "A1BG", "A1BG", "", None, np.nan],
         data={
-            "__mapped__": [False, False, False, False, False, False],
+            "__validated__": [False, False, False, False, False, False],
         },
     )
 
     assert mapping.equals(expected_df)
+
+
+def test_validate(genes):
+    df, _ = genes
+    assert validate(
+        identifiers=["A1CF", "a1cf"],
+        field_values=df["symbol"],
+        case_sensitive=True,
+    ).tolist() == [True, False]
+    assert validate(
+        identifiers=["A1CF", "a1cf"],
+        field_values=df["symbol"],
+        case_sensitive=False,
+        return_df=True,
+    )["__validated__"].tolist() == [True, True]
+    assert validate(
+        identifiers=df["symbol"],
+        field_values=df["symbol"],
+    ).tolist() == [True, True, True]
```

### Comparing `lamin_utils-0.9.3/tests/test_lookup.py` & `lamin_utils-0.9.4/tests/test_lookup.py`

 * *Files identical despite different names*

### Comparing `lamin_utils-0.9.3/tests/test_map_synonyms.py` & `lamin_utils-0.9.4/tests/test_map_synonyms.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import pandas as pd
 import pytest
 
 from lamin_utils._map_synonyms import (
-    check_if_ids_in_field_values,
     explode_aggregated_column_to_map,
     map_synonyms,
     not_empty_none_na,
     to_str,
 )
 
 
@@ -157,27 +156,14 @@
     assert to_str(pd.Index(["A", "a", None, np.nan])).tolist() == ["a", "a", "", ""]
     assert to_str(pd.Series(["A", "a", None, np.nan])).tolist() == ["a", "a", "", ""]
     assert to_str(
         pd.Series(["A", "a", None, np.nan]), case_sensitive=True
     ).tolist() == ["A", "a", "", ""]
 
 
-def test_check_if_ids_in_field_values(genes):
-    _, df = genes
-    assert check_if_ids_in_field_values(
-        identifiers=["A1CF", "a1cf"], field_values=df["symbol"]
-    )["__mapped__"].tolist() == [True, True]
-    assert check_if_ids_in_field_values(
-        identifiers=["A1CF", "a1cf"], field_values=df["symbol"], case_sensitive=True
-    )["__mapped__"].tolist() == [True, False]
-    assert check_if_ids_in_field_values(
-        identifiers=df["symbol"], field_values=df["symbol"]
-    )["__mapped__"].tolist() == [True, True, True, True, True, True]
-
-
 def test_not_empty_none_na():
     import numpy as np
 
     assert not_empty_none_na(["a", None, "", np.nan]).loc[0] == "a"
     assert not_empty_none_na(pd.Index(["a", None, "", np.nan])).tolist() == ["a"]
     assert not_empty_none_na(
         pd.Series(["a", None, "", np.nan], index=["1", "2", "3", "4"])
```

### Comparing `lamin_utils-0.9.3/tests/test_search.py` & `lamin_utils-0.9.4/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `lamin_utils-0.9.3/PKG-INFO` & `lamin_utils-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamin_utils
-Version: 0.9.3
+Version: 0.9.4
 Summary: Lamin Utils.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

