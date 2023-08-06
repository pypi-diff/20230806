# Comparing `tmp/datafusion-27.0.0.tar.gz` & `tmp/datafusion-28.0.0.tar.gz`

## Comparing `datafusion-27.0.0.tar` & `datafusion-28.0.0.tar`

### file list

```diff
@@ -1,101 +1,105 @@
--rw-r--r--   0        0        0     2298 1970-01-01 00:00:00.000000 datafusion-27.0.0/Cargo.toml
--rw-rw-r--   0     1000     1000    11358 2023-07-03 17:26:58.000000 datafusion-27.0.0/LICENSE.txt
--rw-rw-r--   0     1000     1000     8888 2023-07-03 17:26:58.000000 datafusion-27.0.0/README.md
--rw-rw-r--   0     1000     1000     4404 2023-07-03 17:26:58.000000 datafusion-27.0.0/datafusion/__init__.py
--rw-rw-r--   0     1000     1000      875 2023-07-03 17:26:58.000000 datafusion-27.0.0/datafusion/common.py
--rw-rw-r--   0     1000     1000     3664 2023-07-03 17:26:58.000000 datafusion-27.0.0/datafusion/context.py
--rw-rw-r--   0     1000     1000     3546 2023-07-03 17:26:58.000000 datafusion-27.0.0/datafusion/cudf.py
--rw-rw-r--   0     1000     1000      871 2023-07-03 17:26:58.000000 datafusion-27.0.0/datafusion/expr.py
--rw-rw-r--   0     1000     1000      881 2023-07-03 17:26:58.000000 datafusion-27.0.0/datafusion/functions.py
--rw-rw-r--   0     1000     1000      887 2023-07-03 17:26:58.000000 datafusion-27.0.0/datafusion/object_store.py
--rw-rw-r--   0     1000     1000     3507 2023-07-03 17:26:58.000000 datafusion-27.0.0/datafusion/pandas.py
--rw-rw-r--   0     1000     1000     4062 2023-07-03 17:26:58.000000 datafusion-27.0.0/datafusion/polars.py
--rw-rw-r--   0     1000     1000      881 2023-07-03 17:26:58.000000 datafusion-27.0.0/datafusion/substrait.py
--rw-rw-r--   0     1000     1000      785 2023-07-03 17:26:58.000000 datafusion-27.0.0/datafusion/tests/__init__.py
--rw-rw-r--   0     1000     1000     1443 2023-07-03 17:26:58.000000 datafusion-27.0.0/datafusion/tests/conftest.py
--rw-rw-r--   0     1000     1000       57 2023-07-03 17:26:58.000000 datafusion-27.0.0/datafusion/tests/data_test_context/data.json
--rw-rw-r--   0     1000     1000     2319 2023-07-03 17:26:58.000000 datafusion-27.0.0/datafusion/tests/generic.py
--rw-rw-r--   0     1000     1000     4339 2023-07-03 17:26:58.000000 datafusion-27.0.0/datafusion/tests/test_aggregation.py
--rw-rw-r--   0     1000     1000     1432 2023-07-03 17:26:58.000000 datafusion-27.0.0/datafusion/tests/test_catalog.py
--rw-rw-r--   0     1000     1000     1365 2023-07-03 17:26:58.000000 datafusion-27.0.0/datafusion/tests/test_config.py
--rw-rw-r--   0     1000     1000     9833 2023-07-03 17:26:58.000000 datafusion-27.0.0/datafusion/tests/test_context.py
--rw-rw-r--   0     1000     1000    17013 2023-07-03 17:26:58.000000 datafusion-27.0.0/datafusion/tests/test_dataframe.py
--rw-rw-r--   0     1000     1000     3179 2023-07-03 17:26:58.000000 datafusion-27.0.0/datafusion/tests/test_expr.py
--rw-rw-r--   0     1000     1000    14842 2023-07-03 17:26:58.000000 datafusion-27.0.0/datafusion/tests/test_functions.py
--rw-rw-r--   0     1000     1000     3984 2023-07-03 17:26:58.000000 datafusion-27.0.0/datafusion/tests/test_imports.py
--rw-rw-r--   0     1000     1000     1631 2023-07-03 17:26:58.000000 datafusion-27.0.0/datafusion/tests/test_indexing.py
--rw-rw-r--   0     1000     1000     9040 2023-07-03 17:26:58.000000 datafusion-27.0.0/datafusion/tests/test_sql.py
--rw-rw-r--   0     1000     1000     1370 2023-07-03 17:26:58.000000 datafusion-27.0.0/datafusion/tests/test_store.py
--rw-rw-r--   0     1000     1000     1949 2023-07-03 17:26:58.000000 datafusion-27.0.0/datafusion/tests/test_substrait.py
--rw-rw-r--   0     1000     1000     3619 2023-07-03 17:26:58.000000 datafusion-27.0.0/datafusion/tests/test_udaf.py
--rw-rw-r--   0     1000     1000     2177 2023-07-03 17:26:58.000000 datafusion-27.0.0/pyproject.toml
--rw-rw-r--   0     1000     1000     3950 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/catalog.rs
--rw-rw-r--   0     1000     1000    24898 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/common/data_type.rs
--rw-rw-r--   0     1000     1000     3557 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/common/df_field.rs
--rw-rw-r--   0     1000     1000     1651 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/common/df_schema.rs
--rw-rw-r--   0     1000     1000     1836 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/common/function.rs
--rw-rw-r--   0     1000     1000     6256 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/common/schema.rs
--rw-rw-r--   0     1000     1000     1613 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/common.rs
--rw-rw-r--   0     1000     1000     3308 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/config.rs
--rw-rw-r--   0     1000     1000    26405 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/context.rs
--rw-rw-r--   0     1000     1000    15226 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/dataframe.rs
--rw-rw-r--   0     1000     1000     4760 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/dataset.rs
--rw-rw-r--   0     1000     1000     9973 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/dataset_exec.rs
--rw-rw-r--   0     1000     1000     3054 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/errors.rs
--rw-rw-r--   0     1000     1000     3243 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/aggregate.rs
--rw-rw-r--   0     1000     1000     2313 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/aggregate_expr.rs
--rw-rw-r--   0     1000     1000     1867 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/alias.rs
--rw-rw-r--   0     1000     1000     2331 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/analyze.rs
--rw-rw-r--   0     1000     1000     2101 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/between.rs
--rw-rw-r--   0     1000     1000     1626 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/binary_expr.rs
--rw-rw-r--   0     1000     1000     6317 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/bool_expr.rs
--rw-rw-r--   0     1000     1000     1662 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/case.rs
--rw-rw-r--   0     1000     1000     2060 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/cast.rs
--rw-rw-r--   0     1000     1000     1688 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/column.rs
--rw-rw-r--   0     1000     1000     2716 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/create_memory_table.rs
--rw-rw-r--   0     1000     1000     2967 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/create_view.rs
--rw-rw-r--   0     1000     1000     2867 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/cross_join.rs
--rw-rw-r--   0     1000     1000     2206 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/distinct.rs
--rw-rw-r--   0     1000     1000     2338 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/drop_table.rs
--rw-rw-r--   0     1000     1000     2522 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/empty_relation.rs
--rw-rw-r--   0     1000     1000     1334 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/exists.rs
--rw-rw-r--   0     1000     1000     3168 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/explain.rs
--rw-rw-r--   0     1000     1000     1535 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/extension.rs
--rw-rw-r--   0     1000     1000     2502 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/filter.rs
--rw-rw-r--   0     1000     1000     1293 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/grouping_set.rs
--rw-rw-r--   0     1000     1000     1495 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/in_list.rs
--rw-rw-r--   0     1000     1000     1531 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/in_subquery.rs
--rw-rw-r--   0     1000     1000     2093 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/indexed_field.rs
--rw-rw-r--   0     1000     1000     5153 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/join.rs
--rw-rw-r--   0     1000     1000     4441 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/like.rs
--rw-rw-r--   0     1000     1000     2584 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/limit.rs
--rw-rw-r--   0     1000     1000     5048 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/literal.rs
--rw-rw-r--   0     1000     1000     1199 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/logical_node.rs
--rw-rw-r--   0     1000     1000     1456 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/placeholder.rs
--rw-rw-r--   0     1000     1000     3557 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/projection.rs
--rw-rw-r--   0     1000     1000     3884 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/repartition.rs
--rw-rw-r--   0     1000     1000     2101 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/scalar_function.rs
--rw-rw-r--   0     1000     1000     1431 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/scalar_subquery.rs
--rw-rw-r--   0     1000     1000     1674 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/scalar_variable.rs
--rw-rw-r--   0     1000     1000     1310 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/signature.rs
--rw-rw-r--   0     1000     1000     2736 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/sort.rs
--rw-rw-r--   0     1000     1000     2228 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/subquery.rs
--rw-rw-r--   0     1000     1000     2754 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/subquery_alias.rs
--rw-rw-r--   0     1000     1000     4489 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/table_scan.rs
--rw-rw-r--   0     1000     1000     2470 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr/union.rs
--rw-rw-r--   0     1000     1000    25260 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/expr.rs
--rw-rw-r--   0     1000     1000    17966 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/functions.rs
--rw-rw-r--   0     1000     1000     3778 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/lib.rs
--rw-rw-r--   0     1000     1000     2270 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/physical_plan.rs
--rw-rw-r--   0     1000     1000     8547 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/pyarrow_filter_expression.rs
--rw-rw-r--   0     1000     1000     2050 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/record_batch.rs
--rw-rw-r--   0     1000     1000     1716 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/sql/exceptions.rs
--rw-rw-r--   0     1000     1000     4524 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/sql/logical.rs
--rw-rw-r--   0     1000     1000      839 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/sql.rs
--rw-rw-r--   0     1000     1000     7397 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/store.rs
--rw-rw-r--   0     1000     1000     5211 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/substrait.rs
--rw-rw-r--   0     1000     1000     4747 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/udaf.rs
--rw-rw-r--   0     1000     1000     3543 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/udf.rs
--rw-rw-r--   0     1000     1000     1961 2023-07-03 17:26:58.000000 datafusion-27.0.0/src/utils.rs
--rw-rw-r--   0     1000     1000    80851 2023-07-03 17:26:58.000000 datafusion-27.0.0/Cargo.lock
--rw-r--r--   0        0        0     9574 1970-01-01 00:00:00.000000 datafusion-27.0.0/PKG-INFO
+-rw-r--r--   0        0        0     2353 1970-01-01 00:00:00.000000 datafusion-28.0.0/Cargo.toml
+-rw-rw-r--   0     1000     1000    11358 2023-07-25 16:01:34.000000 datafusion-28.0.0/LICENSE.txt
+-rw-rw-r--   0     1000     1000     8888 2023-07-25 16:01:34.000000 datafusion-28.0.0/README.md
+-rw-rw-r--   0     1000     1000     4404 2023-07-25 16:01:34.000000 datafusion-28.0.0/datafusion/__init__.py
+-rw-rw-r--   0     1000     1000      875 2023-07-25 16:01:34.000000 datafusion-28.0.0/datafusion/common.py
+-rw-rw-r--   0     1000     1000     3689 2023-07-25 16:01:34.000000 datafusion-28.0.0/datafusion/context.py
+-rw-rw-r--   0     1000     1000     3546 2023-07-25 16:01:34.000000 datafusion-28.0.0/datafusion/cudf.py
+-rw-rw-r--   0     1000     1000      871 2023-07-25 16:01:34.000000 datafusion-28.0.0/datafusion/expr.py
+-rw-rw-r--   0     1000     1000      881 2023-07-25 16:01:34.000000 datafusion-28.0.0/datafusion/functions.py
+-rw-rw-r--   0     1000     1000      868 2023-07-25 16:01:34.000000 datafusion-28.0.0/datafusion/input/__init__.py
+-rw-rw-r--   0     1000     1000     1521 2023-07-25 16:01:34.000000 datafusion-28.0.0/datafusion/input/base.py
+-rw-rw-r--   0     1000     1000     3169 2023-07-25 16:01:34.000000 datafusion-28.0.0/datafusion/input/location.py
+-rw-rw-r--   0     1000     1000      887 2023-07-25 16:01:34.000000 datafusion-28.0.0/datafusion/object_store.py
+-rw-rw-r--   0     1000     1000     3507 2023-07-25 16:01:34.000000 datafusion-28.0.0/datafusion/pandas.py
+-rw-rw-r--   0     1000     1000     4062 2023-07-25 16:01:34.000000 datafusion-28.0.0/datafusion/polars.py
+-rw-rw-r--   0     1000     1000      881 2023-07-25 16:01:34.000000 datafusion-28.0.0/datafusion/substrait.py
+-rw-rw-r--   0     1000     1000      785 2023-07-25 16:01:34.000000 datafusion-28.0.0/datafusion/tests/__init__.py
+-rw-rw-r--   0     1000     1000     1443 2023-07-25 16:01:34.000000 datafusion-28.0.0/datafusion/tests/conftest.py
+-rw-rw-r--   0     1000     1000       57 2023-07-25 16:01:34.000000 datafusion-28.0.0/datafusion/tests/data_test_context/data.json
+-rw-rw-r--   0     1000     1000     2319 2023-07-25 16:01:34.000000 datafusion-28.0.0/datafusion/tests/generic.py
+-rw-rw-r--   0     1000     1000     4339 2023-07-25 16:01:34.000000 datafusion-28.0.0/datafusion/tests/test_aggregation.py
+-rw-rw-r--   0     1000     1000     1432 2023-07-25 16:01:34.000000 datafusion-28.0.0/datafusion/tests/test_catalog.py
+-rw-rw-r--   0     1000     1000     1365 2023-07-25 16:01:34.000000 datafusion-28.0.0/datafusion/tests/test_config.py
+-rw-rw-r--   0     1000     1000     9833 2023-07-25 16:01:34.000000 datafusion-28.0.0/datafusion/tests/test_context.py
+-rw-rw-r--   0     1000     1000    17313 2023-07-25 16:01:34.000000 datafusion-28.0.0/datafusion/tests/test_dataframe.py
+-rw-rw-r--   0     1000     1000     3393 2023-07-25 16:01:34.000000 datafusion-28.0.0/datafusion/tests/test_expr.py
+-rw-rw-r--   0     1000     1000    14842 2023-07-25 16:01:34.000000 datafusion-28.0.0/datafusion/tests/test_functions.py
+-rw-rw-r--   0     1000     1000     3984 2023-07-25 16:01:34.000000 datafusion-28.0.0/datafusion/tests/test_imports.py
+-rw-rw-r--   0     1000     1000     1631 2023-07-25 16:01:34.000000 datafusion-28.0.0/datafusion/tests/test_indexing.py
+-rw-rw-r--   0     1000     1000     1243 2023-07-25 16:01:34.000000 datafusion-28.0.0/datafusion/tests/test_input.py
+-rw-rw-r--   0     1000     1000     9040 2023-07-25 16:01:34.000000 datafusion-28.0.0/datafusion/tests/test_sql.py
+-rw-rw-r--   0     1000     1000     1370 2023-07-25 16:01:34.000000 datafusion-28.0.0/datafusion/tests/test_store.py
+-rw-rw-r--   0     1000     1000     1949 2023-07-25 16:01:34.000000 datafusion-28.0.0/datafusion/tests/test_substrait.py
+-rw-rw-r--   0     1000     1000     3619 2023-07-25 16:01:34.000000 datafusion-28.0.0/datafusion/tests/test_udaf.py
+-rw-rw-r--   0     1000     1000     2177 2023-07-25 16:01:34.000000 datafusion-28.0.0/pyproject.toml
+-rw-rw-r--   0     1000     1000     3950 2023-07-25 16:01:34.000000 datafusion-28.0.0/src/catalog.rs
+-rw-rw-r--   0     1000     1000    27910 2023-07-25 16:01:34.000000 datafusion-28.0.0/src/common/data_type.rs
+-rw-rw-r--   0     1000     1000     3557 2023-07-25 16:01:34.000000 datafusion-28.0.0/src/common/df_field.rs
+-rw-rw-r--   0     1000     1000     1651 2023-07-25 16:01:34.000000 datafusion-28.0.0/src/common/df_schema.rs
+-rw-rw-r--   0     1000     1000     1836 2023-07-25 16:01:34.000000 datafusion-28.0.0/src/common/function.rs
+-rw-rw-r--   0     1000     1000     6256 2023-07-25 16:01:34.000000 datafusion-28.0.0/src/common/schema.rs
+-rw-rw-r--   0     1000     1000     1613 2023-07-25 16:01:34.000000 datafusion-28.0.0/src/common.rs
+-rw-rw-r--   0     1000     1000     3308 2023-07-25 16:01:34.000000 datafusion-28.0.0/src/config.rs
+-rw-rw-r--   0     1000     1000    26405 2023-07-25 16:01:34.000000 datafusion-28.0.0/src/context.rs
+-rw-rw-r--   0     1000     1000    15289 2023-07-25 16:01:34.000000 datafusion-28.0.0/src/dataframe.rs
+-rw-rw-r--   0     1000     1000     4760 2023-07-25 16:01:34.000000 datafusion-28.0.0/src/dataset.rs
+-rw-rw-r--   0     1000     1000    10023 2023-07-25 16:01:34.000000 datafusion-28.0.0/src/dataset_exec.rs
+-rw-rw-r--   0     1000     1000     3054 2023-07-25 16:01:34.000000 datafusion-28.0.0/src/errors.rs
+-rw-rw-r--   0     1000     1000     3243 2023-07-25 16:01:34.000000 datafusion-28.0.0/src/expr/aggregate.rs
+-rw-rw-r--   0     1000     1000     2313 2023-07-25 16:01:34.000000 datafusion-28.0.0/src/expr/aggregate_expr.rs
+-rw-rw-r--   0     1000     1000     1867 2023-07-25 16:01:34.000000 datafusion-28.0.0/src/expr/alias.rs
+-rw-rw-r--   0     1000     1000     2331 2023-07-25 16:01:34.000000 datafusion-28.0.0/src/expr/analyze.rs
+-rw-rw-r--   0     1000     1000     2101 2023-07-25 16:01:34.000000 datafusion-28.0.0/src/expr/between.rs
+-rw-rw-r--   0     1000     1000     1626 2023-07-25 16:01:34.000000 datafusion-28.0.0/src/expr/binary_expr.rs
+-rw-rw-r--   0     1000     1000     6317 2023-07-25 16:01:34.000000 datafusion-28.0.0/src/expr/bool_expr.rs
+-rw-rw-r--   0     1000     1000     1662 2023-07-25 16:01:34.000000 datafusion-28.0.0/src/expr/case.rs
+-rw-rw-r--   0     1000     1000     2060 2023-07-25 16:01:34.000000 datafusion-28.0.0/src/expr/cast.rs
+-rw-rw-r--   0     1000     1000     1688 2023-07-25 16:01:34.000000 datafusion-28.0.0/src/expr/column.rs
+-rw-rw-r--   0     1000     1000     2716 2023-07-25 16:01:34.000000 datafusion-28.0.0/src/expr/create_memory_table.rs
+-rw-rw-r--   0     1000     1000     2967 2023-07-25 16:01:34.000000 datafusion-28.0.0/src/expr/create_view.rs
+-rw-rw-r--   0     1000     1000     2867 2023-07-25 16:01:34.000000 datafusion-28.0.0/src/expr/cross_join.rs
+-rw-rw-r--   0     1000     1000     2206 2023-07-25 16:01:34.000000 datafusion-28.0.0/src/expr/distinct.rs
+-rw-rw-r--   0     1000     1000     2338 2023-07-25 16:01:34.000000 datafusion-28.0.0/src/expr/drop_table.rs
+-rw-rw-r--   0     1000     1000     2522 2023-07-25 16:01:34.000000 datafusion-28.0.0/src/expr/empty_relation.rs
+-rw-rw-r--   0     1000     1000     1334 2023-07-25 16:01:34.000000 datafusion-28.0.0/src/expr/exists.rs
+-rw-rw-r--   0     1000     1000     3168 2023-07-25 16:01:34.000000 datafusion-28.0.0/src/expr/explain.rs
+-rw-rw-r--   0     1000     1000     1535 2023-07-25 16:01:34.000000 datafusion-28.0.0/src/expr/extension.rs
+-rw-rw-r--   0     1000     1000     2502 2023-07-25 16:01:34.000000 datafusion-28.0.0/src/expr/filter.rs
+-rw-rw-r--   0     1000     1000     1293 2023-07-25 16:01:34.000000 datafusion-28.0.0/src/expr/grouping_set.rs
+-rw-rw-r--   0     1000     1000     1495 2023-07-25 16:01:34.000000 datafusion-28.0.0/src/expr/in_list.rs
+-rw-rw-r--   0     1000     1000     1531 2023-07-25 16:01:34.000000 datafusion-28.0.0/src/expr/in_subquery.rs
+-rw-rw-r--   0     1000     1000     2093 2023-07-25 16:01:34.000000 datafusion-28.0.0/src/expr/indexed_field.rs
+-rw-rw-r--   0     1000     1000     5153 2023-07-25 16:01:34.000000 datafusion-28.0.0/src/expr/join.rs
+-rw-rw-r--   0     1000     1000     4441 2023-07-25 16:01:34.000000 datafusion-28.0.0/src/expr/like.rs
+-rw-rw-r--   0     1000     1000     2584 2023-07-25 16:01:34.000000 datafusion-28.0.0/src/expr/limit.rs
+-rw-rw-r--   0     1000     1000     5048 2023-07-25 16:01:34.000000 datafusion-28.0.0/src/expr/literal.rs
+-rw-rw-r--   0     1000     1000     1199 2023-07-25 16:01:34.000000 datafusion-28.0.0/src/expr/logical_node.rs
+-rw-rw-r--   0     1000     1000     1456 2023-07-25 16:01:34.000000 datafusion-28.0.0/src/expr/placeholder.rs
+-rw-rw-r--   0     1000     1000     3557 2023-07-25 16:01:34.000000 datafusion-28.0.0/src/expr/projection.rs
+-rw-rw-r--   0     1000     1000     3884 2023-07-25 16:01:34.000000 datafusion-28.0.0/src/expr/repartition.rs
+-rw-rw-r--   0     1000     1000     2101 2023-07-25 16:01:34.000000 datafusion-28.0.0/src/expr/scalar_function.rs
+-rw-rw-r--   0     1000     1000     1431 2023-07-25 16:01:34.000000 datafusion-28.0.0/src/expr/scalar_subquery.rs
+-rw-rw-r--   0     1000     1000     1674 2023-07-25 16:01:34.000000 datafusion-28.0.0/src/expr/scalar_variable.rs
+-rw-rw-r--   0     1000     1000     1310 2023-07-25 16:01:34.000000 datafusion-28.0.0/src/expr/signature.rs
+-rw-rw-r--   0     1000     1000     2736 2023-07-25 16:01:34.000000 datafusion-28.0.0/src/expr/sort.rs
+-rw-rw-r--   0     1000     1000     2228 2023-07-25 16:01:34.000000 datafusion-28.0.0/src/expr/subquery.rs
+-rw-rw-r--   0     1000     1000     2754 2023-07-25 16:01:34.000000 datafusion-28.0.0/src/expr/subquery_alias.rs
+-rw-rw-r--   0     1000     1000     4955 2023-07-25 16:01:34.000000 datafusion-28.0.0/src/expr/table_scan.rs
+-rw-rw-r--   0     1000     1000     2470 2023-07-25 16:01:34.000000 datafusion-28.0.0/src/expr/union.rs
+-rw-rw-r--   0     1000     1000    25373 2023-07-25 16:01:34.000000 datafusion-28.0.0/src/expr.rs
+-rw-rw-r--   0     1000     1000    17988 2023-07-25 16:01:34.000000 datafusion-28.0.0/src/functions.rs
+-rw-rw-r--   0     1000     1000     3778 2023-07-25 16:01:34.000000 datafusion-28.0.0/src/lib.rs
+-rw-rw-r--   0     1000     1000     2270 2023-07-25 16:01:34.000000 datafusion-28.0.0/src/physical_plan.rs
+-rw-rw-r--   0     1000     1000     8547 2023-07-25 16:01:34.000000 datafusion-28.0.0/src/pyarrow_filter_expression.rs
+-rw-rw-r--   0     1000     1000     2050 2023-07-25 16:01:34.000000 datafusion-28.0.0/src/record_batch.rs
+-rw-rw-r--   0     1000     1000     1716 2023-07-25 16:01:34.000000 datafusion-28.0.0/src/sql/exceptions.rs
+-rw-rw-r--   0     1000     1000     4524 2023-07-25 16:01:34.000000 datafusion-28.0.0/src/sql/logical.rs
+-rw-rw-r--   0     1000     1000      839 2023-07-25 16:01:34.000000 datafusion-28.0.0/src/sql.rs
+-rw-rw-r--   0     1000     1000     7397 2023-07-25 16:01:34.000000 datafusion-28.0.0/src/store.rs
+-rw-rw-r--   0     1000     1000     5211 2023-07-25 16:01:34.000000 datafusion-28.0.0/src/substrait.rs
+-rw-rw-r--   0     1000     1000     4747 2023-07-25 16:01:34.000000 datafusion-28.0.0/src/udaf.rs
+-rw-rw-r--   0     1000     1000     3543 2023-07-25 16:01:34.000000 datafusion-28.0.0/src/udf.rs
+-rw-rw-r--   0     1000     1000     1961 2023-07-25 16:01:34.000000 datafusion-28.0.0/src/utils.rs
+-rw-rw-r--   0     1000     1000    80518 2023-07-25 16:01:34.000000 datafusion-28.0.0/Cargo.lock
+-rw-r--r--   0        0        0     9574 1970-01-01 00:00:00.000000 datafusion-28.0.0/PKG-INFO
```

### Comparing `datafusion-27.0.0/Cargo.toml` & `datafusion-28.0.0/Cargo.toml`

 * *Files 9% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 [package]
 name = "datafusion-python"
-version = "27.0.0"
+version = "28.0.0"
 homepage = "https://github.com/apache/arrow-datafusion-python"
 repository = "https://github.com/apache/arrow-datafusion-python"
 authors = ["Apache Arrow <dev@arrow.apache.org>"]
 description = "Apache Arrow DataFusion DataFrame and SQL Query Engine"
 readme = "README.md"
 license = "Apache-2.0"
 edition = "2021"
@@ -32,20 +32,20 @@
 default = ["mimalloc"]
 protoc = [ "datafusion-substrait/protoc" ]
 
 [dependencies]
 tokio = { version = "1.24", features = ["macros", "rt", "rt-multi-thread", "sync"] }
 rand = "0.8"
 pyo3 = { version = "0.19", features = ["extension-module", "abi3", "abi3-py38"] }
-datafusion = { version = "27.0.0" , features = ["pyarrow", "avro"] }
-datafusion-common = { version = "27.0.0", features = ["pyarrow"] }
-datafusion-expr = "27.0.0"
-datafusion-optimizer = "27.0.0"
-datafusion-sql = "27.0.0"
-datafusion-substrait = "27.0.0"
+datafusion = { version = "28.0.0", features = ["pyarrow", "avro"] }
+datafusion-common = { version = "28.0.0", features = ["pyarrow"] }
+datafusion-expr = { version = "28.0.0" }
+datafusion-optimizer = { version = "28.0.0" }
+datafusion-sql = { version = "28.0.0" }
+datafusion-substrait = { version = "28.0.0" }
 prost = "0.11"
 prost-types = "0.11"
 uuid = { version = "1.3", features = ["v4"] }
 mimalloc = { version = "0.1", optional = true, default-features = false }
 async-trait = "0.1"
 futures = "0.3"
 object_store = { version = "0.6.1", features = ["aws", "gcp", "azure"] }
```

### Comparing `datafusion-27.0.0/LICENSE.txt` & `datafusion-28.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/README.md` & `datafusion-28.0.0/README.md`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/datafusion/__init__.py` & `datafusion-28.0.0/datafusion/__init__.py`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/datafusion/common.py` & `datafusion-28.0.0/datafusion/common.py`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/datafusion/context.py` & `datafusion-28.0.0/datafusion/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from abc import ABC, abstractmethod
-from typing import Dict, List
+from typing import Any, Dict, List
 
 from datafusion.common import SqlSchema, SqlTable
 
 
 class BaseSessionContext(ABC):
     """
     Abstraction defining all methods, properties, and common functionality
@@ -75,16 +75,17 @@
         Return all schemas in the current SessionContext impl.
         """
         pass
 
     @abstractmethod
     def create_table(
         self,
+        schema_name: str,
         table_name: str,
-        schema_name: str = None,
+        input_source: Any,
         **kwargs,
     ):
         """
         Creates/Registers a table in the specied schema instance
         """
         pass
```

### Comparing `datafusion-27.0.0/datafusion/cudf.py` & `datafusion-28.0.0/datafusion/cudf.py`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/datafusion/expr.py` & `datafusion-28.0.0/datafusion/expr.py`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/datafusion/functions.py` & `datafusion-28.0.0/datafusion/functions.py`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/datafusion/object_store.py` & `datafusion-28.0.0/datafusion/object_store.py`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/datafusion/pandas.py` & `datafusion-28.0.0/datafusion/pandas.py`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/datafusion/polars.py` & `datafusion-28.0.0/datafusion/polars.py`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/datafusion/substrait.py` & `datafusion-28.0.0/datafusion/substrait.py`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/datafusion/tests/__init__.py` & `datafusion-28.0.0/datafusion/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/datafusion/tests/conftest.py` & `datafusion-28.0.0/datafusion/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/datafusion/tests/generic.py` & `datafusion-28.0.0/datafusion/tests/generic.py`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/datafusion/tests/test_aggregation.py` & `datafusion-28.0.0/datafusion/tests/test_aggregation.py`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/datafusion/tests/test_catalog.py` & `datafusion-28.0.0/datafusion/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/datafusion/tests/test_config.py` & `datafusion-28.0.0/datafusion/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/datafusion/tests/test_context.py` & `datafusion-28.0.0/datafusion/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/datafusion/tests/test_dataframe.py` & `datafusion-28.0.0/datafusion/tests/test_dataframe.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,14 +111,25 @@
     # execute and collect the first (and only) batch
     result = df.collect()[0]
 
     assert len(result.column(0)) == 1
     assert len(result.column(1)) == 1
 
 
+def test_limit_with_offset(df):
+    # only 3 rows, but limit past the end to ensure that offset is working
+    df = df.limit(5, offset=2)
+
+    # execute and collect the first (and only) batch
+    result = df.collect()[0]
+
+    assert len(result.column(0)) == 1
+    assert len(result.column(1)) == 1
+
+
 def test_with_column(df):
     df = df.with_column("c", column("a") + column("b"))
 
     # execute and collect the first (and only) batch
     result = df.collect()[0]
 
     assert result.schema.field(0).name == "a"
```

### Comparing `datafusion-27.0.0/datafusion/tests/test_expr.py` & `datafusion-28.0.0/datafusion/tests/test_expr.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,14 +77,22 @@
 
 def test_limit(test_ctx):
     df = test_ctx.sql("select c1 from test LIMIT 10")
     plan = df.logical_plan()
 
     plan = plan.to_variant()
     assert isinstance(plan, Limit)
+    assert plan.skip() == 0
+
+    df = test_ctx.sql("select c1 from test LIMIT 10 OFFSET 5")
+    plan = df.logical_plan()
+
+    plan = plan.to_variant()
+    assert isinstance(plan, Limit)
+    assert plan.skip() == 5
 
 
 def test_aggregate_query(test_ctx):
     df = test_ctx.sql("select c1, count(*) from test group by c1")
     plan = df.logical_plan()
 
     projection = plan.to_variant()
```

### Comparing `datafusion-27.0.0/datafusion/tests/test_functions.py` & `datafusion-28.0.0/datafusion/tests/test_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -378,19 +378,19 @@
     result = df.collect()
     assert len(result) == 1
     result = result[0]
     assert result.column(0) == pa.array([12, 6, 7], type=pa.float64())
     assert result.column(1) == pa.array([2022, 2027, 2020], type=pa.float64())
     assert result.column(2) == pa.array(
         [datetime(2022, 12, 1), datetime(2027, 6, 1), datetime(2020, 7, 1)],
-        type=pa.timestamp("ns"),
+        type=pa.timestamp("us"),
     )
     assert result.column(3) == pa.array(
         [datetime(2022, 12, 31), datetime(2027, 6, 26), datetime(2020, 7, 2)],
-        type=pa.timestamp("ns"),
+        type=pa.timestamp("us"),
     )
     assert result.column(4) == pa.array(
         [
             datetime(2022, 12, 30, 23, 47, 30),
             datetime(2027, 6, 25, 23, 47, 30),
             datetime(2020, 7, 1, 23, 47, 30),
         ],
```

### Comparing `datafusion-27.0.0/datafusion/tests/test_imports.py` & `datafusion-28.0.0/datafusion/tests/test_imports.py`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/datafusion/tests/test_indexing.py` & `datafusion-28.0.0/datafusion/tests/test_indexing.py`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/datafusion/tests/test_sql.py` & `datafusion-28.0.0/datafusion/tests/test_sql.py`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/datafusion/tests/test_store.py` & `datafusion-28.0.0/datafusion/tests/test_store.py`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/datafusion/tests/test_substrait.py` & `datafusion-28.0.0/datafusion/tests/test_substrait.py`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/datafusion/tests/test_udaf.py` & `datafusion-28.0.0/datafusion/tests/test_udaf.py`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/pyproject.toml` & `datafusion-28.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/src/catalog.rs` & `datafusion-28.0.0/src/catalog.rs`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/src/common/data_type.rs` & `datafusion-28.0.0/src/common/data_type.rs`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
 use datafusion::arrow::datatypes::{DataType, IntervalUnit, TimeUnit};
 use datafusion_common::{DataFusionError, ScalarValue};
-use pyo3::prelude::*;
+use pyo3::{exceptions::PyValueError, prelude::*};
 
 use crate::errors::py_datafusion_err;
 
 #[derive(Debug, Clone, PartialEq, Eq, Hash, PartialOrd, Ord)]
 #[pyclass(name = "RexType", module = "datafusion.common")]
 pub enum RexType {
     Alias,
@@ -284,14 +284,21 @@
             ScalarValue::IntervalDayTime(..) => Ok(DataType::Interval(IntervalUnit::DayTime)),
             ScalarValue::IntervalMonthDayNano(..) => {
                 Ok(DataType::Interval(IntervalUnit::MonthDayNano))
             }
             ScalarValue::List(_val, field_ref) => Ok(DataType::List(field_ref.to_owned())),
             ScalarValue::Struct(_, fields) => Ok(DataType::Struct(fields.to_owned())),
             ScalarValue::FixedSizeBinary(size, _) => Ok(DataType::FixedSizeBinary(*size)),
+            ScalarValue::Fixedsizelist(_, field_ref, size) => {
+                Ok(DataType::FixedSizeList(field_ref.to_owned(), *size))
+            }
+            ScalarValue::DurationSecond(_) => Ok(DataType::Duration(TimeUnit::Second)),
+            ScalarValue::DurationMillisecond(_) => Ok(DataType::Duration(TimeUnit::Millisecond)),
+            ScalarValue::DurationMicrosecond(_) => Ok(DataType::Duration(TimeUnit::Microsecond)),
+            ScalarValue::DurationNanosecond(_) => Ok(DataType::Duration(TimeUnit::Nanosecond)),
         }
     }
 }
 
 #[pymethods]
 impl DataTypeMap {
     #[new]
@@ -300,20 +307,51 @@
             arrow_type,
             python_type,
             sql_type,
         }
     }
 
     #[staticmethod]
+    #[pyo3(name = "from_parquet_type_str")]
+    /// When using pyarrow.parquet.read_metadata().schema.column(x).physical_type you are presented
+    /// with a String type for schema rather than an object type. Here we make a best effort
+    /// to convert that to a physical type.
+    pub fn py_map_from_parquet_type_str(parquet_str_type: String) -> PyResult<DataTypeMap> {
+        let arrow_dtype = match parquet_str_type.to_lowercase().as_str() {
+            "boolean" => Ok(DataType::Boolean),
+            "int32" => Ok(DataType::Int32),
+            "int64" => Ok(DataType::Int64),
+            "int96" => {
+                // Int96 is an old parquet datatype that is now deprecated. We convert to nanosecond timestamp
+                Ok(DataType::Timestamp(TimeUnit::Nanosecond, None))
+            }
+            "float" => Ok(DataType::Float32),
+            "double" => Ok(DataType::Float64),
+            _ => Err(PyValueError::new_err(format!(
+                "Unable to determine Arrow Data Type from Parquet String type: {:?}",
+                parquet_str_type
+            ))),
+        };
+        DataTypeMap::map_from_arrow_type(&arrow_dtype?)
+    }
+
+    #[staticmethod]
     #[pyo3(name = "arrow")]
     pub fn py_map_from_arrow_type(arrow_type: &PyDataType) -> PyResult<DataTypeMap> {
         DataTypeMap::map_from_arrow_type(&arrow_type.data_type)
     }
 
     #[staticmethod]
+    #[pyo3(name = "arrow_str")]
+    pub fn py_map_from_arrow_type_str(arrow_type_str: String) -> PyResult<DataTypeMap> {
+        let data_type = PyDataType::py_map_from_arrow_type_str(arrow_type_str);
+        DataTypeMap::map_from_arrow_type(&data_type?.data_type)
+    }
+
+    #[staticmethod]
     #[pyo3(name = "sql")]
     pub fn py_map_from_sql_type(sql_type: &SqlType) -> PyResult<DataTypeMap> {
         match sql_type {
             SqlType::ANY => Err(py_datafusion_err(DataFusionError::NotImplemented(format!(
                 "{:?}",
                 sql_type
             )))),
@@ -554,14 +592,37 @@
 /// `DataType` as `PyDataType` This exists solely to satisfy those constraints.
 #[derive(Debug, Clone, PartialEq, Eq, Hash, PartialOrd, Ord)]
 #[pyclass(name = "DataType", module = "datafusion.common")]
 pub struct PyDataType {
     pub data_type: DataType,
 }
 
+impl PyDataType {
+    /// There are situations when obtaining dtypes on the Python side where the Arrow type
+    /// is presented as a String rather than an actual DataType. This function is used to
+    /// convert that String to a DataType for the Python side to use.
+    pub fn py_map_from_arrow_type_str(arrow_str_type: String) -> PyResult<PyDataType> {
+        let arrow_dtype = match arrow_str_type.to_lowercase().as_str() {
+            "boolean" => Ok(DataType::Boolean),
+            "int32" => Ok(DataType::Int32),
+            "int64" => Ok(DataType::Int64),
+            "float" => Ok(DataType::Float32),
+            "double" => Ok(DataType::Float64),
+            "float64" => Ok(DataType::Float64),
+            _ => Err(PyValueError::new_err(format!(
+                "Unable to determine Arrow Data Type from Arrow String type: {:?}",
+                arrow_str_type
+            ))),
+        };
+        Ok(PyDataType {
+            data_type: arrow_dtype?,
+        })
+    }
+}
+
 impl From<PyDataType> for DataType {
     fn from(data_type: PyDataType) -> DataType {
         data_type.data_type
     }
 }
 
 impl From<DataType> for PyDataType {
```

### Comparing `datafusion-27.0.0/src/common/df_field.rs` & `datafusion-28.0.0/src/common/df_field.rs`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/src/common/df_schema.rs` & `datafusion-28.0.0/src/common/df_schema.rs`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/src/common/function.rs` & `datafusion-28.0.0/src/common/function.rs`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/src/common/schema.rs` & `datafusion-28.0.0/src/common/schema.rs`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/src/common.rs` & `datafusion-28.0.0/src/common.rs`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/src/config.rs` & `datafusion-28.0.0/src/config.rs`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/src/context.rs` & `datafusion-28.0.0/src/context.rs`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/src/dataframe.rs` & `datafusion-28.0.0/src/dataframe.rs`

 * *Files 0% similar despite different names*

```diff
@@ -132,16 +132,17 @@
     #[pyo3(signature = (*exprs))]
     fn sort(&self, exprs: Vec<PyExpr>) -> PyResult<Self> {
         let exprs = exprs.into_iter().map(|e| e.into()).collect();
         let df = self.df.as_ref().clone().sort(exprs)?;
         Ok(Self::new(df))
     }
 
-    fn limit(&self, count: usize) -> PyResult<Self> {
-        let df = self.df.as_ref().clone().limit(0, Some(count))?;
+    #[pyo3(signature = (count, offset=0))]
+    fn limit(&self, count: usize, offset: usize) -> PyResult<Self> {
+        let df = self.df.as_ref().clone().limit(offset, Some(count))?;
         Ok(Self::new(df))
     }
 
     /// Executes the plan, returning a list of `RecordBatch`es.
     /// Unless some order is specified in the plan, there is no
     /// guarantee of the order of the result.
     fn collect(&self, py: Python) -> PyResult<Vec<PyObject>> {
```

### Comparing `datafusion-27.0.0/src/dataset.rs` & `datafusion-28.0.0/src/dataset.rs`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/src/dataset_exec.rs` & `datafusion-28.0.0/src/dataset_exec.rs`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,16 @@
 use datafusion::arrow::pyarrow::PyArrowType;
 use datafusion::arrow::record_batch::RecordBatch;
 use datafusion::error::{DataFusionError as InnerDataFusionError, Result as DFResult};
 use datafusion::execution::context::TaskContext;
 use datafusion::physical_expr::PhysicalSortExpr;
 use datafusion::physical_plan::stream::RecordBatchStreamAdapter;
 use datafusion::physical_plan::{
-    DisplayFormatType, ExecutionPlan, Partitioning, SendableRecordBatchStream, Statistics,
+    DisplayAs, DisplayFormatType, ExecutionPlan, Partitioning, SendableRecordBatchStream,
+    Statistics,
 };
 use datafusion_expr::Expr;
 use datafusion_optimizer::utils::conjunction;
 
 use crate::errors::DataFusionError;
 use crate::pyarrow_filter_expression::PyArrowFilterExpression;
 
@@ -231,14 +232,20 @@
             let record_batch_stream: SendableRecordBatchStream = Box::pin(
                 RecordBatchStreamAdapter::new(schema, record_batch_stream.map_err(|e| e.into())),
             );
             Ok(record_batch_stream)
         })
     }
 
+    fn statistics(&self) -> Statistics {
+        self.projected_statistics.clone()
+    }
+}
+
+impl DisplayAs for DatasetExec {
     fn fmt_as(&self, t: DisplayFormatType, f: &mut std::fmt::Formatter) -> std::fmt::Result {
         Python::with_gil(|py| {
             let number_of_fragments = self.fragments.as_ref(py).len();
             match t {
                 DisplayFormatType::Default | DisplayFormatType::Verbose => {
                     let projected_columns: Vec<String> = self
                         .schema
@@ -263,12 +270,8 @@
                             projected_columns.join(", "),
                         )
                     }
                 }
             }
         })
     }
-
-    fn statistics(&self) -> Statistics {
-        self.projected_statistics.clone()
-    }
 }
```

### Comparing `datafusion-27.0.0/src/errors.rs` & `datafusion-28.0.0/src/errors.rs`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/src/expr/aggregate.rs` & `datafusion-28.0.0/src/expr/aggregate.rs`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/src/expr/aggregate_expr.rs` & `datafusion-28.0.0/src/expr/aggregate_expr.rs`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/src/expr/alias.rs` & `datafusion-28.0.0/src/expr/alias.rs`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/src/expr/analyze.rs` & `datafusion-28.0.0/src/expr/analyze.rs`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/src/expr/between.rs` & `datafusion-28.0.0/src/expr/between.rs`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/src/expr/binary_expr.rs` & `datafusion-28.0.0/src/expr/binary_expr.rs`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/src/expr/bool_expr.rs` & `datafusion-28.0.0/src/expr/bool_expr.rs`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/src/expr/case.rs` & `datafusion-28.0.0/src/expr/case.rs`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/src/expr/cast.rs` & `datafusion-28.0.0/src/expr/cast.rs`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/src/expr/column.rs` & `datafusion-28.0.0/src/expr/column.rs`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/src/expr/create_memory_table.rs` & `datafusion-28.0.0/src/expr/create_memory_table.rs`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/src/expr/create_view.rs` & `datafusion-28.0.0/src/expr/create_view.rs`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/src/expr/cross_join.rs` & `datafusion-28.0.0/src/expr/cross_join.rs`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/src/expr/distinct.rs` & `datafusion-28.0.0/src/expr/distinct.rs`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/src/expr/drop_table.rs` & `datafusion-28.0.0/src/expr/drop_table.rs`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/src/expr/empty_relation.rs` & `datafusion-28.0.0/src/expr/empty_relation.rs`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/src/expr/exists.rs` & `datafusion-28.0.0/src/expr/exists.rs`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/src/expr/explain.rs` & `datafusion-28.0.0/src/expr/explain.rs`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/src/expr/extension.rs` & `datafusion-28.0.0/src/expr/extension.rs`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/src/expr/filter.rs` & `datafusion-28.0.0/src/expr/filter.rs`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/src/expr/grouping_set.rs` & `datafusion-28.0.0/src/expr/grouping_set.rs`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/src/expr/in_list.rs` & `datafusion-28.0.0/src/expr/in_list.rs`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/src/expr/in_subquery.rs` & `datafusion-28.0.0/src/expr/in_subquery.rs`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/src/expr/indexed_field.rs` & `datafusion-28.0.0/src/expr/indexed_field.rs`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/src/expr/join.rs` & `datafusion-28.0.0/src/expr/join.rs`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/src/expr/like.rs` & `datafusion-28.0.0/src/expr/like.rs`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/src/expr/limit.rs` & `datafusion-28.0.0/src/expr/limit.rs`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/src/expr/literal.rs` & `datafusion-28.0.0/src/expr/literal.rs`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/src/expr/logical_node.rs` & `datafusion-28.0.0/src/expr/logical_node.rs`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/src/expr/placeholder.rs` & `datafusion-28.0.0/src/expr/placeholder.rs`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/src/expr/projection.rs` & `datafusion-28.0.0/src/expr/projection.rs`

 * *Files 2% similar despite different names*

```diff
@@ -94,16 +94,16 @@
 }
 
 impl PyProjection {
     /// Projection: Gets the names of the fields that should be projected
     pub fn projected_expressions(local_expr: &PyExpr) -> Vec<PyExpr> {
         let mut projs: Vec<PyExpr> = Vec::new();
         match &local_expr.expr {
-            Expr::Alias(expr, _name) => {
-                let py_expr: PyExpr = PyExpr::from(*expr.clone());
+            Expr::Alias(alias) => {
+                let py_expr: PyExpr = PyExpr::from(*alias.expr.clone());
                 projs.extend_from_slice(Self::projected_expressions(&py_expr).as_slice());
             }
             _ => projs.push(local_expr.clone()),
         }
         projs
     }
 }
```

### Comparing `datafusion-27.0.0/src/expr/repartition.rs` & `datafusion-28.0.0/src/expr/repartition.rs`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/src/expr/scalar_function.rs` & `datafusion-28.0.0/src/expr/scalar_function.rs`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/src/expr/scalar_subquery.rs` & `datafusion-28.0.0/src/expr/scalar_subquery.rs`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/src/expr/scalar_variable.rs` & `datafusion-28.0.0/src/expr/scalar_variable.rs`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/src/expr/signature.rs` & `datafusion-28.0.0/src/expr/signature.rs`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/src/expr/sort.rs` & `datafusion-28.0.0/src/expr/sort.rs`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/src/expr/subquery.rs` & `datafusion-28.0.0/src/expr/subquery.rs`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/src/expr/subquery_alias.rs` & `datafusion-28.0.0/src/expr/subquery_alias.rs`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/src/expr/table_scan.rs` & `datafusion-28.0.0/src/expr/table_scan.rs`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 // Unless required by applicable law or agreed to in writing,
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
+use datafusion_common::TableReference;
 use datafusion_expr::logical_plan::TableScan;
 use pyo3::prelude::*;
 use std::fmt::{self, Display, Formatter};
 
 use crate::expr::logical_node::LogicalNode;
 use crate::sql::logical::PyLogicalPlan;
 use crate::{common::df_schema::PyDFSchema, expr::PyExpr};
@@ -67,20 +68,33 @@
 impl PyTableScan {
     /// Retrieves the name of the table represented by this `TableScan` instance
     #[pyo3(name = "table_name")]
     fn py_table_name(&self) -> PyResult<String> {
         Ok(format!("{}", self.table_scan.table_name))
     }
 
-    /// TODO: Bindings for `TableSource` need to exist first. Left as a
-    /// placeholder to display intention to add when able to.
-    // #[pyo3(name = "source")]
-    // fn py_source(&self) -> PyResult<Arc<dyn TableSource>> {
-    //     Ok(self.table_scan.source)
-    // }
+    #[pyo3(name = "fqn")]
+    fn fqn(&self) -> PyResult<(Option<String>, Option<String>, String)> {
+        let table_ref: TableReference = self.table_scan.table_name.clone();
+        Ok(match table_ref {
+            TableReference::Bare { table } => (None, None, table.to_string()),
+            TableReference::Partial { schema, table } => {
+                (None, Some(schema.to_string()), table.to_string())
+            }
+            TableReference::Full {
+                catalog,
+                schema,
+                table,
+            } => (
+                Some(catalog.to_string()),
+                Some(schema.to_string()),
+                table.to_string(),
+            ),
+        })
+    }
 
     /// The column indexes that should be. Note if this is empty then
     /// all columns should be read by the `TableProvider`. This function
     /// provides a Tuple of the (index, column_name) to make things simplier
     /// for the calling code since often times the name is preferred to
     /// the index which is a lower level abstraction.
     #[pyo3(name = "projection")]
```

### Comparing `datafusion-27.0.0/src/expr/union.rs` & `datafusion-28.0.0/src/expr/union.rs`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/src/expr.rs` & `datafusion-28.0.0/src/expr.rs`

 * *Files 2% similar despite different names*

```diff
@@ -111,15 +111,15 @@
 }
 
 #[pymethods]
 impl PyExpr {
     /// Return the specific expression
     fn to_variant(&self, py: Python) -> PyResult<PyObject> {
         Python::with_gil(|_| match &self.expr {
-            Expr::Alias(alias, name) => Ok(PyAlias::new(alias, name).into_py(py)),
+            Expr::Alias(alias) => Ok(PyAlias::new(&alias.expr, &alias.name).into_py(py)),
             Expr::Column(col) => Ok(PyColumn::from(col.clone()).into_py(py)),
             Expr::ScalarVariable(data_type, variables) => {
                 Ok(PyScalarVariable::new(data_type, variables).into_py(py))
             }
             Expr::Literal(value) => Ok(PyLiteral::from(value.clone()).into_py(py)),
             Expr::BinaryExpr(expr) => Ok(PyBinaryExpr::from(expr.clone()).into_py(py)),
             Expr::Not(expr) => Ok(PyNot::new(*expr.clone()).into_py(py)),
@@ -261,15 +261,14 @@
             Expr::ScalarVariable(..) | Expr::Literal(..) => RexType::Literal,
             Expr::BinaryExpr { .. }
             | Expr::Not(..)
             | Expr::IsNotNull(..)
             | Expr::Negative(..)
             | Expr::IsNull(..)
             | Expr::Like { .. }
-            | Expr::ILike { .. }
             | Expr::SimilarTo { .. }
             | Expr::Between { .. }
             | Expr::Case { .. }
             | Expr::Cast { .. }
             | Expr::TryCast { .. }
             | Expr::Sort { .. }
             | Expr::ScalarFunction { .. }
@@ -332,16 +331,21 @@
                 ScalarValue::TimestampSecond(v, _) => v.into_py(py),
                 ScalarValue::TimestampMillisecond(v, _) => v.into_py(py),
                 ScalarValue::TimestampMicrosecond(v, _) => v.into_py(py),
                 ScalarValue::TimestampNanosecond(v, _) => v.into_py(py),
                 ScalarValue::IntervalYearMonth(v) => v.into_py(py),
                 ScalarValue::IntervalDayTime(v) => v.into_py(py),
                 ScalarValue::IntervalMonthDayNano(v) => v.into_py(py),
+                ScalarValue::DurationSecond(v) => v.into_py(py),
+                ScalarValue::DurationMicrosecond(v) => v.into_py(py),
+                ScalarValue::DurationNanosecond(v) => v.into_py(py),
+                ScalarValue::DurationMillisecond(v) => v.into_py(py),
                 ScalarValue::Struct(_, _) => todo!(),
                 ScalarValue::Dictionary(_, _) => todo!(),
+                ScalarValue::Fixedsizelist(_, _, _) => todo!(),
             }),
             _ => Err(py_type_err(format!(
                 "Non Expr::Literal encountered in types: {:?}",
                 &self.expr
             ))),
         }
     }
@@ -352,17 +356,18 @@
     pub fn rex_call_operands(&self) -> PyResult<Vec<PyExpr>> {
         match &self.expr {
             // Expr variants that are themselves the operand to return
             Expr::Column(..) | Expr::ScalarVariable(..) | Expr::Literal(..) => {
                 Ok(vec![PyExpr::from(self.expr.clone())])
             }
 
+            Expr::Alias(alias) => Ok(vec![PyExpr::from(*alias.expr.clone())]),
+
             // Expr(s) that house the Expr instance to return in their bounded params
-            Expr::Alias(expr, ..)
-            | Expr::Not(expr)
+            Expr::Not(expr)
             | Expr::IsNull(expr)
             | Expr::IsNotNull(expr)
             | Expr::IsTrue(expr)
             | Expr::IsFalse(expr)
             | Expr::IsUnknown(expr)
             | Expr::IsNotTrue(expr)
             | Expr::IsNotFalse(expr)
@@ -425,18 +430,14 @@
                 PyExpr::from(*left.clone()),
                 PyExpr::from(*right.clone()),
             ]),
             Expr::Like(Like { expr, pattern, .. }) => Ok(vec![
                 PyExpr::from(*expr.clone()),
                 PyExpr::from(*pattern.clone()),
             ]),
-            Expr::ILike(Like { expr, pattern, .. }) => Ok(vec![
-                PyExpr::from(*expr.clone()),
-                PyExpr::from(*pattern.clone()),
-            ]),
             Expr::SimilarTo(Like { expr, pattern, .. }) => Ok(vec![
                 PyExpr::from(*expr.clone()),
                 PyExpr::from(*pattern.clone()),
             ]),
             Expr::Between(Between {
                 expr,
                 negated: _,
@@ -482,26 +483,24 @@
             Expr::IsUnknown(_) => "is unknown".to_string(),
             Expr::IsNotTrue(_) => "is not true".to_string(),
             Expr::IsNotFalse(_) => "is not false".to_string(),
             Expr::IsNotUnknown(_) => "is not unknown".to_string(),
             Expr::InList { .. } => "in list".to_string(),
             Expr::Negative(..) => "negative".to_string(),
             Expr::Not(..) => "not".to_string(),
-            Expr::Like(Like { negated, .. }) => {
-                if *negated {
-                    "not like".to_string()
-                } else {
-                    "like".to_string()
-                }
-            }
-            Expr::ILike(Like { negated, .. }) => {
+            Expr::Like(Like {
+                negated,
+                case_insensitive,
+                ..
+            }) => {
+                let name = if *case_insensitive { "ilike" } else { "like" };
                 if *negated {
-                    "not ilike".to_string()
+                    format!("not {name}")
                 } else {
-                    "ilike".to_string()
+                    name.to_string()
                 }
             }
             Expr::SimilarTo(Like { negated, .. }) => {
                 if *negated {
                     "not similar to".to_string()
                 } else {
                     "similar to".to_string()
```

### Comparing `datafusion-27.0.0/src/functions.rs` & `datafusion-28.0.0/src/functions.rs`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
 use pyo3::{prelude::*, wrap_pyfunction};
 
 use datafusion_common::Column;
+use datafusion_expr::expr::Alias;
 use datafusion_expr::{
     aggregate_function,
     expr::{AggregateFunction, ScalarFunction, Sort, WindowFunction},
     lit,
     window_function::find_df_window_func,
     BuiltinScalarFunction, Expr, WindowFrame,
 };
@@ -81,15 +82,15 @@
     })
 }
 
 /// Creates a new Alias Expr
 #[pyfunction]
 fn alias(expr: PyExpr, name: &str) -> PyResult<PyExpr> {
     Ok(PyExpr {
-        expr: datafusion_expr::Expr::Alias(Box::new(expr.expr), String::from(name)),
+        expr: datafusion_expr::Expr::Alias(Alias::new(expr.expr, name)),
     })
 }
 
 /// Create a column reference Expr
 #[pyfunction]
 fn col(name: &str) -> PyResult<PyExpr> {
     Ok(PyExpr {
```

### Comparing `datafusion-27.0.0/src/lib.rs` & `datafusion-28.0.0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/src/physical_plan.rs` & `datafusion-28.0.0/src/physical_plan.rs`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/src/pyarrow_filter_expression.rs` & `datafusion-28.0.0/src/pyarrow_filter_expression.rs`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/src/record_batch.rs` & `datafusion-28.0.0/src/record_batch.rs`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/src/sql/exceptions.rs` & `datafusion-28.0.0/src/sql/exceptions.rs`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/src/sql/logical.rs` & `datafusion-28.0.0/src/sql/logical.rs`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/src/sql.rs` & `datafusion-28.0.0/src/sql.rs`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/src/store.rs` & `datafusion-28.0.0/src/store.rs`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/src/substrait.rs` & `datafusion-28.0.0/src/substrait.rs`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/src/udaf.rs` & `datafusion-28.0.0/src/udaf.rs`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/src/udf.rs` & `datafusion-28.0.0/src/udf.rs`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/src/utils.rs` & `datafusion-28.0.0/src/utils.rs`

 * *Files identical despite different names*

### Comparing `datafusion-27.0.0/Cargo.lock` & `datafusion-28.0.0/Cargo.lock`

 * *Files 4% similar despite different names*

```diff
@@ -58,17 +58,17 @@
 checksum = "94fb8275041c72129eb51b7d0322c29b8387a0386127718b096429201a5d6ece"
 dependencies = [
  "alloc-no-stdlib",
 ]
 
 [[package]]
 name = "allocator-api2"
-version = "0.2.15"
+version = "0.2.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "56fc6cf8dc8c4158eed8649f9b8b0ea1518eb62b544fe9490d66fa0b349eafe9"
+checksum = "0942ffc6dcaadf03badf6e6a2d0228460359d5e34b57ccdc720b7382dfbd5ec5"
 
 [[package]]
 name = "android-tzdata"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e999941b234f3131b00bc13c22d06e8c5ff726d1b6318ac7eb276997bbb4fef0"
 
@@ -79,17 +79,17 @@
 checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "anyhow"
-version = "1.0.71"
+version = "1.0.72"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c7d0618f0e0b7e8ff11427422b64564d5fb0be1940354bfe2e0529b18a9d9b8"
+checksum = "3b13c32d80ecc7ab747b80c3784bce54ee8a7a0cc4fbda9bf4cda2cf6fe90854"
 
 [[package]]
 name = "apache-avro"
 version = "0.14.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8cf4144857f9e4d7dd6cc4ba4c78efd2a46bad682b029bd0d91e76a021af1b2a"
 dependencies = [
@@ -124,17 +124,17 @@
 name = "arrayvec"
 version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "96d30a06541fbafbc7f82ed10c06164cfbd2c401138f6addd8404629c4b16711"
 
 [[package]]
 name = "arrow"
-version = "42.0.0"
+version = "43.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "773d18d72cd290f3f9e2149a714c8ac404b6c3fd614c684f0015449940fca899"
+checksum = "2feeebd77b34b0bc88f224e06d01c27da4733997cc4789a4e056196656cdc59a"
 dependencies = [
  "ahash",
  "arrow-arith",
  "arrow-array",
  "arrow-buffer",
  "arrow-cast",
  "arrow-csv",
@@ -147,59 +147,59 @@
  "arrow-select",
  "arrow-string",
  "pyo3",
 ]
 
 [[package]]
 name = "arrow-arith"
-version = "42.0.0"
+version = "43.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "93bc0da4b22ba63807fa2a74998e21209179c93c67856ae65d9218b81f3ef918"
+checksum = "7173f5dc49c0ecb5135f52565af33afd3fdc9a12d13bd6f9973e8b96305e4b2e"
 dependencies = [
  "arrow-array",
  "arrow-buffer",
  "arrow-data",
  "arrow-schema",
  "chrono",
  "half",
  "num",
 ]
 
 [[package]]
 name = "arrow-array"
-version = "42.0.0"
+version = "43.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ea9a0fd21121304cad96f307c938d861cb1e7f0c151b93047462cd9817d760fb"
+checksum = "63d7ea725f7d1f8bb2cffc53ef538557e95fc802e217d5be25122d402e22f3d0"
 dependencies = [
  "ahash",
  "arrow-buffer",
  "arrow-data",
  "arrow-schema",
  "chrono",
  "chrono-tz",
  "half",
  "hashbrown 0.14.0",
  "num",
 ]
 
 [[package]]
 name = "arrow-buffer"
-version = "42.0.0"
+version = "43.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "30ce342ecf5971004e23cef8b5fb3bacd2bbc48a381464144925074e1472e9eb"
+checksum = "bdbe439e077f484e5000b9e1d47b5e4c0d15f2b311a8f5bcc682553d5d67a722"
 dependencies = [
  "half",
  "num",
 ]
 
 [[package]]
 name = "arrow-cast"
-version = "42.0.0"
+version = "43.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4b94a0ce7d27abbb02e2ee4db770f593127610f57b32625b0bc6a1a90d65f085"
+checksum = "93913cc14875770aa1eef5e310765e855effa352c094cb1c7c00607d0f37b4e1"
 dependencies = [
  "arrow-array",
  "arrow-buffer",
  "arrow-data",
  "arrow-schema",
  "arrow-select",
  "chrono",
@@ -207,17 +207,17 @@
  "half",
  "lexical-core",
  "num",
 ]
 
 [[package]]
 name = "arrow-csv"
-version = "42.0.0"
+version = "43.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0f3be10a00a43c4bf0d243c070754ebdde17c5d576b4928d9c3efbe3005a3853"
+checksum = "ef55b67c55ed877e6fe7b923121c19dae5e31ca70249ea2779a17b58fb0fbd9a"
 dependencies = [
  "arrow-array",
  "arrow-buffer",
  "arrow-cast",
  "arrow-data",
  "arrow-schema",
  "chrono",
@@ -226,130 +226,131 @@
  "lazy_static",
  "lexical-core",
  "regex",
 ]
 
 [[package]]
 name = "arrow-data"
-version = "42.0.0"
+version = "43.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1d9a83dad6a53d6907765106d3bc61d6d9d313cfe1751701b3ef0948e7283dc2"
+checksum = "d4f4f4a3c54614126a71ab91f6631c9743eb4643d6e9318b74191da9dc6e028b"
 dependencies = [
  "arrow-buffer",
  "arrow-schema",
  "half",
  "num",
 ]
 
 [[package]]
 name = "arrow-ipc"
-version = "42.0.0"
+version = "43.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a46da5e438a854e0386b38774da88a98782c0973c6dbc5c949ca4e02faf9b016"
+checksum = "d41a3659f984a524ef1c2981d43747b24d8eec78e2425267fcd0ef34ce71cd18"
 dependencies = [
  "arrow-array",
  "arrow-buffer",
  "arrow-cast",
  "arrow-data",
  "arrow-schema",
  "flatbuffers",
 ]
 
 [[package]]
 name = "arrow-json"
-version = "42.0.0"
+version = "43.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d5f27a1fbc76553ad92dc1a9583e56b7058d8c418c4089b0b689f5b87e2da5e1"
+checksum = "10b95faa95a378f56ef32d84cc0104ea998c39ef7cd1faaa6b4cebf8ea92846d"
 dependencies = [
  "arrow-array",
  "arrow-buffer",
  "arrow-cast",
  "arrow-data",
  "arrow-schema",
  "chrono",
  "half",
- "indexmap 1.9.3",
+ "indexmap 2.0.0",
  "lexical-core",
  "num",
  "serde",
  "serde_json",
 ]
 
 [[package]]
 name = "arrow-ord"
-version = "42.0.0"
+version = "43.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f2373661f6c2233e18f6fa69c40999a9440231d1e8899be8bbbe73c7e24aa3b4"
+checksum = "c68549a4284d9f8b39586afb8d5ff8158b8f0286353a4844deb1d11cf1ba1f26"
 dependencies = [
  "arrow-array",
  "arrow-buffer",
  "arrow-data",
  "arrow-schema",
  "arrow-select",
  "half",
  "num",
 ]
 
 [[package]]
 name = "arrow-row"
-version = "42.0.0"
+version = "43.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "377cd5158b7de4034a175e296726c40c3236e65d71d90a5dab2fb4fab526a8f4"
+checksum = "0a75a4a757afc301ce010adadff54d79d66140c4282ed3de565f6ccb716a5cf3"
 dependencies = [
  "ahash",
  "arrow-array",
  "arrow-buffer",
  "arrow-data",
  "arrow-schema",
  "half",
  "hashbrown 0.14.0",
 ]
 
 [[package]]
 name = "arrow-schema"
-version = "42.0.0"
+version = "43.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ba9ed245bd2d7d97ad1457cb281d4296e8b593588758b8fec6d67b2b2b0f2265"
+checksum = "2bebcb57eef570b15afbcf2d07d813eb476fde9f6dd69c81004d6476c197e87e"
 dependencies = [
  "bitflags 2.3.3",
 ]
 
 [[package]]
 name = "arrow-select"
-version = "42.0.0"
+version = "43.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0dc9bd6aebc565b1d04bae64a0f4dda3abc677190eb7d960471b1b20e1cebed0"
+checksum = "f6e2943fa433a48921e914417173816af64eef61c0a3d448280e6c40a62df221"
 dependencies = [
  "arrow-array",
  "arrow-buffer",
  "arrow-data",
  "arrow-schema",
  "num",
 ]
 
 [[package]]
 name = "arrow-string"
-version = "42.0.0"
+version = "43.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "23cf2baea2ef53787332050decf7d71aca836a352e188c8ad062892405955d2b"
+checksum = "bbc92ed638851774f6d7af1ad900b92bc1486746497511868b4298fcbcfa35af"
 dependencies = [
  "arrow-array",
  "arrow-buffer",
  "arrow-data",
  "arrow-schema",
  "arrow-select",
+ "num",
  "regex",
  "regex-syntax",
 ]
 
 [[package]]
 name = "async-compression"
-version = "0.4.0"
+version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5b0122885821398cc923ece939e24d1056a2384ee719432397fa9db87230ff11"
+checksum = "62b74f44609f0f91493e3082d3734d98497e094777144380ea4db9f9905dd5b6"
 dependencies = [
  "bzip2",
  "flate2",
  "futures-core",
  "futures-io",
  "memchr",
  "pin-project-lite",
@@ -363,26 +364,26 @@
 name = "async-recursion"
 version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0e97ce7de6cf12de5d7226c73f5ba9811622f4db3a5b91b55c53e987e5f91cba"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.22",
+ "syn 2.0.27",
 ]
 
 [[package]]
 name = "async-trait"
-version = "0.1.68"
+version = "0.1.72"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b9ccdd8f2a161be9bd5c023df56f1b2a0bd1d83872ae53b71a84a12c9bf6e842"
+checksum = "cc6dde6e4ed435a4c1ee4e73592f5ba9da2151af10076cc04858746af9352d09"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.22",
+ "syn 2.0.27",
 ]
 
 [[package]]
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
@@ -436,17 +437,17 @@
 checksum = "46502ad458c9a52b69d4d4d32775c788b7a1b85e8bc9d482d92250fc0e3f8efe"
 dependencies = [
  "digest",
 ]
 
 [[package]]
 name = "blake3"
-version = "1.4.0"
+version = "1.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "729b71f35bd3fa1a4c86b85d32c8b9069ea7fe14f7a53cfabb65f62d4265b888"
+checksum = "199c42ab6972d92c9f8995f086273d25c42fc0f7b2a1fcefba465c1352d25ba5"
 dependencies = [
  "arrayref",
  "arrayvec",
  "cc",
  "cfg-if",
  "constant_time_eq",
  "digest",
@@ -602,29 +603,29 @@
  "once_cell",
  "proc-macro-hack",
  "tiny-keccak",
 ]
 
 [[package]]
 name = "constant_time_eq"
-version = "0.2.6"
+version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "21a53c0a4d288377e7415b53dcfc3c04da5cdc2cc95c8d5ac178b58f0b861ad6"
+checksum = "f7144d30dcf0fafbce74250a3963025d8d52177934239851c917d29f1df280c2"
 
 [[package]]
 name = "core-foundation-sys"
 version = "0.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e496a50fda8aacccc86d7529e2c1e0892dbd0f898a6b5645b5561b89c3210efa"
 
 [[package]]
 name = "cpufeatures"
-version = "0.2.8"
+version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "03e69e28e9f7f77debdedbaafa2866e1de9ba56df55a8bd7cfc724c25a09987c"
+checksum = "a17b76ff3a4162b0b27f354a0c87015ddad39d35f9c0c36607a3bdd175dde1f1"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "crc32fast"
 version = "1.3.2"
@@ -669,30 +670,30 @@
 checksum = "2b2466559f260f48ad25fe6317b3c8dac77b5bdb5763ac7d9d6103530663bc90"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "dashmap"
-version = "5.4.0"
+version = "5.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "907076dfda823b0b36d2a1bb5f90c96660a5bbcd7729e10727f07858f22c4edc"
+checksum = "6943ae99c34386c84a470c499d3414f66502a41340aa895406e0d2e4a207b91d"
 dependencies = [
  "cfg-if",
- "hashbrown 0.12.3",
+ "hashbrown 0.14.0",
  "lock_api",
  "once_cell",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "datafusion"
-version = "27.0.0"
+version = "28.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e96f6e4eb10bd3e6b709686858246466983e8c5354a928ff77ee34919aa60d00"
+checksum = "5ddbcb2dda5b5033537457992ebde78938014390b2b19f9f4282e3be0e18b0c3"
 dependencies = [
  "ahash",
  "apache-avro",
  "arrow",
  "arrow-array",
  "arrow-schema",
  "async-compression",
@@ -702,21 +703,21 @@
  "chrono",
  "dashmap",
  "datafusion-common",
  "datafusion-execution",
  "datafusion-expr",
  "datafusion-optimizer",
  "datafusion-physical-expr",
- "datafusion-row",
  "datafusion-sql",
  "flate2",
  "futures",
  "glob",
+ "half",
  "hashbrown 0.14.0",
- "indexmap 1.9.3",
+ "indexmap 2.0.0",
  "itertools 0.11.0",
  "lazy_static",
  "log",
  "num-traits",
  "num_cpus",
  "object_store",
  "parking_lot",
@@ -733,34 +734,34 @@
  "uuid",
  "xz2",
  "zstd",
 ]
 
 [[package]]
 name = "datafusion-common"
-version = "27.0.0"
+version = "28.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "00e5fddcc0dd49bbe199e43aa406f39c46c790bb2a43c7b36a478e5f3f971235"
+checksum = "85fbb7b4da925031311743ab96662d55f0f7342d3692744f184f99b2257ef435"
 dependencies = [
  "apache-avro",
  "arrow",
  "arrow-array",
  "chrono",
  "num_cpus",
  "object_store",
  "parquet",
  "pyo3",
  "sqlparser",
 ]
 
 [[package]]
 name = "datafusion-execution"
-version = "27.0.0"
+version = "28.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cfd50b6cb17acc78d2473c0d28014b8fd4e2e0a2c067c07645d6547b33b0aeeb"
+checksum = "5bb3617466d894eb0ad11d06bab1e6e89c571c0a27d660685d327d0c6e1e1ccd"
 dependencies = [
  "dashmap",
  "datafusion-common",
  "datafusion-expr",
  "hashbrown 0.14.0",
  "log",
  "object_store",
@@ -768,32 +769,32 @@
  "rand",
  "tempfile",
  "url",
 ]
 
 [[package]]
 name = "datafusion-expr"
-version = "27.0.0"
+version = "28.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e1a35dc2cd9eac18063d636f7ddf4f090fe1f34284d80192ac7ade38cc3c6991"
+checksum = "3bd8220a0dfcdfddcc785cd7e71770ef1ce54fbe1e08984e5adf537027ecb6de"
 dependencies = [
  "ahash",
  "arrow",
  "datafusion-common",
  "lazy_static",
  "sqlparser",
  "strum 0.25.0",
- "strum_macros 0.25.0",
+ "strum_macros 0.25.1",
 ]
 
 [[package]]
 name = "datafusion-optimizer"
-version = "27.0.0"
+version = "28.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5f5043afeb45ec1c0f45519e1eed6a477f2d30732e8f975d9cf9a75fba0ca716"
+checksum = "1d685a100c66952aaadd0cbe766df46d1887d58fc8bcf3589e6387787f18492b"
 dependencies = [
  "arrow",
  "async-trait",
  "chrono",
  "datafusion-common",
  "datafusion-expr",
  "datafusion-physical-expr",
@@ -801,48 +802,50 @@
  "itertools 0.11.0",
  "log",
  "regex-syntax",
 ]
 
 [[package]]
 name = "datafusion-physical-expr"
-version = "27.0.0"
+version = "28.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6cc892a24f4b829ee7718ad3950884c0346dbdf1517f3df153af4bcf54d8ca4d"
+checksum = "0f2c635da9b05b4b4c6c8d935f46fd99f9b6225f834091cf4e3c8a045b68beab"
 dependencies = [
  "ahash",
  "arrow",
  "arrow-array",
  "arrow-buffer",
  "arrow-schema",
+ "base64",
  "blake2",
  "blake3",
  "chrono",
  "datafusion-common",
  "datafusion-expr",
- "datafusion-row",
  "half",
  "hashbrown 0.14.0",
- "indexmap 1.9.3",
+ "hex",
+ "indexmap 2.0.0",
  "itertools 0.11.0",
  "lazy_static",
  "libc",
+ "log",
  "md-5",
  "paste",
  "petgraph",
  "rand",
  "regex",
  "sha2",
  "unicode-segmentation",
  "uuid",
 ]
 
 [[package]]
 name = "datafusion-python"
-version = "27.0.0"
+version = "28.0.0"
 dependencies = [
  "async-trait",
  "datafusion",
  "datafusion-common",
  "datafusion-expr",
  "datafusion-optimizer",
  "datafusion-sql",
@@ -853,51 +856,39 @@
  "parking_lot",
  "prost",
  "prost-types",
  "pyo3",
  "pyo3-build-config",
  "rand",
  "regex-syntax",
- "syn 2.0.22",
+ "syn 2.0.27",
  "tokio",
  "url",
  "uuid",
 ]
 
 [[package]]
-name = "datafusion-row"
-version = "27.0.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ce75c660bbddfdd254109e668e5b5bd69df31ea26e3768e15cef0c68015e650e"
-dependencies = [
- "arrow",
- "datafusion-common",
- "paste",
- "rand",
-]
-
-[[package]]
 name = "datafusion-sql"
-version = "27.0.0"
+version = "28.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "49cab87e4933a452e0b7b3f0cbd0e760daf7d33fb54d09d70d3ffba229eaa652"
+checksum = "b3ef8abf4dd84d3f20c910822b52779c035ab7f4f2d5e7125ede3bae618e9de8"
 dependencies = [
  "arrow",
  "arrow-schema",
  "datafusion-common",
  "datafusion-expr",
  "log",
  "sqlparser",
 ]
 
 [[package]]
 name = "datafusion-substrait"
-version = "27.0.0"
+version = "28.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ba77d22232053f6cdd98bd6f5328940850844450253f25b8c50bfc5199c505d4"
+checksum = "2c97d351bbd6bd6497e7c9606ddd3c00cd63e9d185d7ab96fc8a66cf3c449177"
 dependencies = [
  "async-recursion",
  "chrono",
  "datafusion",
  "itertools 0.11.0",
  "object_store",
  "prost",
@@ -921,38 +912,38 @@
 name = "doc-comment"
 version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fea41bba32d969b513997752735605054bc0dfa92b4c56bf1189f2e174be7a10"
 
 [[package]]
 name = "dyn-clone"
-version = "1.0.11"
+version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "68b0cf012f1230e43cd00ebb729c6bb58707ecfa8ad08b52ef3a4ccd2697fc30"
+checksum = "304e6508efa593091e97a9abbc10f90aa7ca635b6d2784feff3c89d41dd12272"
 
 [[package]]
 name = "either"
-version = "1.8.1"
+version = "1.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7fcaabb2fef8c910e7f4c7ce9f67a1283a1715879a7c230ca9d6d1ae31f16d91"
+checksum = "a26ae43d7bcc3b814de94796a5e736d4029efb0ee900c12e2d54c993ad1a1e07"
 
 [[package]]
 name = "encoding_rs"
 version = "0.8.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "071a31f4ee85403370b58aca746f01041ede6f0da2730960ad001edc2b71b394"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "equivalent"
-version = "1.0.0"
+version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "88bffebc5d80432c9b140ee17875ff173a8ab62faad5b257da912bd2f6c1c0a1"
+checksum = "5443807d6dff69373d433ab9ef5378ad8df50ca6298caf15de6e52e24aaf54d5"
 
 [[package]]
 name = "errno"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4bcfec3a70f97c962c307b2d2c56e358cf1d00b558d74262b5f929ee8cc7e73a"
 dependencies = [
@@ -969,20 +960,17 @@
 dependencies = [
  "cc",
  "libc",
 ]
 
 [[package]]
 name = "fastrand"
-version = "1.9.0"
+version = "2.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e51093e27b0797c359783294ca4f0a911c270184cb10f85783b118614a1501be"
-dependencies = [
- "instant",
-]
+checksum = "6999dc1837253364c2ebb0704ba97994bd874e8f195d665c50b7548f6ea92764"
 
 [[package]]
 name = "fixedbitset"
 version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ce7134b9999ecaf8bcd65542e436736ef32ddca1b3e06094cb6ec5755203b80"
 
@@ -1073,15 +1061,15 @@
 name = "futures-macro"
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "89ca545a94061b6365f2c7355b4b32bd20df3ff95f02da9329b34ccc3bd6ee72"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.22",
+ "syn 2.0.27",
 ]
 
 [[package]]
 name = "futures-sink"
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f43be4fe21a13b9781a69afa4985b0f6ee0e1afab2c6f454a8cf30e2b2237b6e"
@@ -1215,17 +1203,23 @@
 name = "heck"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
 [[package]]
 name = "hermit-abi"
-version = "0.3.1"
+version = "0.3.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "443144c8cdadd93ebf52ddb4056d257f5b52c04d3c804e657d19eb73fc33668b"
+
+[[package]]
+name = "hex"
+version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fed44880c466736ef9a5c5b5facefb5ed0785676d0c02d612db14e54f0d84286"
+checksum = "7f24254aa9a54b5c858eaee2f5bccdb46aaf0e486a595ed5fd8f86ba55232a70"
 
 [[package]]
 name = "http"
 version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bd6effc99afb63425aff9b05836f029929e345a6148a14b7ecd5ab67af944482"
 dependencies = [
@@ -1285,18 +1279,19 @@
  "tower-service",
  "tracing",
  "want",
 ]
 
 [[package]]
 name = "hyper-rustls"
-version = "0.24.0"
+version = "0.24.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0646026eb1b3eea4cd9ba47912ea5ce9cc07713d105b1a14698f4e6433d348b7"
+checksum = "8d78e1e73ec14cf7375674f74d7dde185c8206fd9dea6fb6295e8a98098aaa97"
 dependencies = [
+ "futures-util",
  "http",
  "hyper",
  "rustls",
  "tokio",
  "tokio-rustls",
 ]
 
@@ -1356,40 +1351,20 @@
 [[package]]
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
-name = "instant"
-version = "0.1.12"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7a5bbe824c507c5da5956355e86a746d82e0e1464f65d862cc5e71da70e94b2c"
-dependencies = [
- "cfg-if",
-]
-
-[[package]]
 name = "integer-encoding"
 version = "3.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8bb03732005da905c88227371639bf1ad885cc712789c011c31c5fb3ab3ccf02"
 
 [[package]]
-name = "io-lifetimes"
-version = "1.0.11"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "eae7b9aee968036d54dce06cebaefd919e4472e753296daccd6d344e3e2df0c2"
-dependencies = [
- "hermit-abi",
- "libc",
- "windows-sys",
-]
-
-[[package]]
 name = "ipnet"
 version = "2.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "28b29a3cd74f0f4598934efe3aeba42bae0eb4680554128851ebbecb02af14e6"
 
 [[package]]
 name = "itertools"
@@ -1407,17 +1382,17 @@
 checksum = "b1c173a5686ce8bfa551b3563d0c2170bf24ca44da99c7ca4bfdab5418c3fe57"
 dependencies = [
  "either",
 ]
 
 [[package]]
 name = "itoa"
-version = "1.0.6"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "453ad9f582a441959e5f0d088b02ce04cfe8d51a8eaf077f12ac6d3e94164ca6"
+checksum = "af150ab688ff2122fcef229be89cb50dd66af9e01a4ff320cc137eecc9bacc38"
 
 [[package]]
 name = "jobserver"
 version = "0.1.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "936cfd212a0155903bcbc060e316fb6cc7cbf2e1907329391ebadc1fe0ce77c2"
 dependencies = [
@@ -1555,29 +1530,29 @@
 dependencies = [
  "cc",
  "libc",
 ]
 
 [[package]]
 name = "libz-sys"
-version = "1.1.9"
+version = "1.1.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "56ee889ecc9568871456d42f603d6a0ce59ff328d291063a45cbdf0036baf6db"
+checksum = "24e6ab01971eb092ffe6a7d42f49f9ff42662f17604681e2843ad65077ba47dc"
 dependencies = [
  "cc",
  "libc",
  "pkg-config",
  "vcpkg",
 ]
 
 [[package]]
 name = "linux-raw-sys"
-version = "0.3.8"
+version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ef53942eb7bf7ff43a617b3e2c1c4a5ecf5944a7c1bc12d7ee39bbb15e5c1519"
+checksum = "09fc20d2ca12cb9f044c93e3bd6d32d523e6e2ec3db4f7b2939cd99026ecd3f0"
 
 [[package]]
 name = "lock_api"
 version = "0.4.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
 dependencies = [
@@ -1685,17 +1660,17 @@
 name = "multimap"
 version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e5ce46fe64a9d73be07dcbe690a38ce1b293be448fd8ce1e6c1b8062c9f72c6a"
 
 [[package]]
 name = "num"
-version = "0.4.0"
+version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "43db66d1170d347f9a065114077f7dccb00c1b9478c89384490a3425279a4606"
+checksum = "b05180d69e3da0e530ba2a1dae5110317e49e3b7f3d41be227dc5f92e49ee7af"
 dependencies = [
  "num-bigint",
  "num-complex",
  "num-integer",
  "num-iter",
  "num-rational",
  "num-traits",
@@ -1752,17 +1727,17 @@
  "num-bigint",
  "num-integer",
  "num-traits",
 ]
 
 [[package]]
 name = "num-traits"
-version = "0.2.15"
+version = "0.2.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
+checksum = "f30b0abd723be7e2ffca1272140fac1a2f084c77ec3e123c192b66af1ee9e6c2"
 dependencies = [
  "autocfg",
  "libm",
 ]
 
 [[package]]
 name = "num_cpus"
@@ -1849,17 +1824,17 @@
  "redox_syscall",
  "smallvec",
  "windows-targets",
 ]
 
 [[package]]
 name = "parquet"
-version = "42.0.0"
+version = "43.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "baab9c36b1c8300b81b4d577d306a0a733f9d34021363098d3548e37757ed6c8"
+checksum = "ec7267a9607c3f955d4d0ac41b88a67cecc0d8d009173ad3da390699a6cb3750"
 dependencies = [
  "ahash",
  "arrow-array",
  "arrow-buffer",
  "arrow-cast",
  "arrow-data",
  "arrow-ipc",
@@ -1892,17 +1867,17 @@
 checksum = "c705f256449c60da65e11ff6626e0c16a0a0b96aaa348de61376b249bc340f41"
 dependencies = [
  "regex",
 ]
 
 [[package]]
 name = "paste"
-version = "1.0.12"
+version = "1.0.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9f746c4065a8fa3fe23974dd82f15431cc8d40779821001404d10d2e79ca7d79"
+checksum = "de3145af08024dea9fa9914f381a17b8fc6034dfb00f3a84013f7ff43f29ed4c"
 
 [[package]]
 name = "percent-encoding"
 version = "2.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9b2a4787296e9989611394c33f193f676704af1686e70b8f8033ab5ba9a35a94"
 
@@ -1952,17 +1927,17 @@
 checksum = "90fcb95eef784c2ac79119d1dd819e162b5da872ce6f3c3abe1e8ca1c082f72b"
 dependencies = [
  "siphasher",
 ]
 
 [[package]]
 name = "pin-project-lite"
-version = "0.2.9"
+version = "0.2.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e0a7ae3ac2f1173085d398531c705756c94a4c56843785df85a60c1a0afac116"
+checksum = "4c40d25201921e5ff0c862a505c6557ea88568a4e3ace775ab55e93f2f4f9d57"
 
 [[package]]
 name = "pin-utils"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b870d8c151b6f2fb93e84a13146138f05d02ed11c7e7c54f8826aaaf7c9f184"
 
@@ -1976,33 +1951,33 @@
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "prettyplease"
-version = "0.2.9"
+version = "0.2.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9825a04601d60621feed79c4e6b56d65db77cdca55cef43b46b0de1096d1c282"
+checksum = "6c64d9ba0963cdcea2e1b2230fbae2bab30eb25a174be395c41e764bfb65dd62"
 dependencies = [
  "proc-macro2",
- "syn 2.0.22",
+ "syn 2.0.27",
 ]
 
 [[package]]
 name = "proc-macro-hack"
 version = "0.5.20+deprecated"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc375e1527247fe1a97d8b7156678dfe7c1af2fc075c9a4db3690ecd2a148068"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.63"
+version = "1.0.66"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b368fba921b0dce7e60f5e04ec15e565b3303972b42bcfde1d0713b881959eb"
+checksum = "18fb31db3f9bddb2ea821cde30a9f70117e3f119938b5ee630b7403aa6e2ead9"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "prost"
 version = "0.11.9"
@@ -2062,66 +2037,66 @@
 checksum = "c7ac8852baeb3cc6fb83b93646fb93c0ffe5d14bf138c945ceb4b9948ee0e3c1"
 dependencies = [
  "autotools",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.19.0"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cffef52f74ec3b1a1baf295d9b8fcc3070327aefc39a6d00656b13c1d0b8885c"
+checksum = "ffb88ae05f306b4bfcde40ac4a51dc0b05936a9207a4b75b798c7729c4258a59"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.19.0"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "713eccf888fb05f1a96eb78c0dbc51907fee42b3377272dc902eb38985f418d5"
+checksum = "554db24f0b3c180a9c0b1268f91287ab3f17c162e15b54caaae5a6b3773396b0"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.19.0"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5b2ecbdcfb01cbbf56e179ce969a048fd7305a66d4cdf3303e0da09d69afe4c3"
+checksum = "922ede8759e8600ad4da3195ae41259654b9c55da4f7eec84a0ccc7d067a70a4"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.19.0"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b78fdc0899f2ea781c463679b20cb08af9247febc8d052de941951024cd8aea0"
+checksum = "8a5caec6a1dd355964a841fcbeeb1b89fe4146c87295573f94228911af3cc5a2"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.19.0"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "60da7b84f1227c3e2fe7593505de274dcf4c8928b4e0a1c23d551a14e4e80a0f"
+checksum = "e0b78ccbb160db1556cdb6fd96c50334c5d4ec44dc5e0a968d0a1208fa0efa8b"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
@@ -2138,17 +2113,17 @@
 dependencies = [
  "memchr",
  "serde",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.29"
+version = "1.0.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "573015e8ab27661678357f27dc26460738fd2b6c86e46f386fde94cb5d913105"
+checksum = "50f3b39ccfb720540debaa0164757101c08ecb8d326b15358ce76a62c7e85965"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.8.5"
@@ -2186,28 +2161,40 @@
 checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
 dependencies = [
  "bitflags 1.3.2",
 ]
 
 [[package]]
 name = "regex"
-version = "1.8.4"
+version = "1.9.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b2eae68fc220f7cf2532e4494aded17545fce192d59cd996e0fe7887f4ceb575"
+dependencies = [
+ "aho-corasick",
+ "memchr",
+ "regex-automata",
+ "regex-syntax",
+]
+
+[[package]]
+name = "regex-automata"
+version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d0ab3ca65655bb1e41f2a8c8cd662eb4fb035e67c3f78da1d61dffe89d07300f"
+checksum = "39354c10dd07468c2e73926b23bb9c2caca74c5501e38a35da70406f1d923310"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.7.2"
+version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "436b050e76ed2903236f032a59761c1eb99e1b0aead2c257922771dab1fc8c78"
+checksum = "e5ea92a5b6195c6ef2a0295ea818b312502c6fc94dde986c5553242e18fd4ce2"
 
 [[package]]
 name = "regress"
 version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "82a9ecfa0cb04d0b04dddb99b8ccf4f66bc8dfd23df694b398570bd8ae3a50fb"
 dependencies = [
@@ -2290,31 +2277,30 @@
 checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
 dependencies = [
  "semver",
 ]
 
 [[package]]
 name = "rustix"
-version = "0.37.21"
+version = "0.38.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "62f25693a73057a1b4cb56179dd3c7ea21a7c6c5ee7d85781f5749b46f34b79c"
+checksum = "0a962918ea88d644592894bc6dc55acc6c0956488adcebbfb6e273506b7fd6e5"
 dependencies = [
- "bitflags 1.3.2",
+ "bitflags 2.3.3",
  "errno",
- "io-lifetimes",
  "libc",
  "linux-raw-sys",
  "windows-sys",
 ]
 
 [[package]]
 name = "rustls"
-version = "0.21.2"
+version = "0.21.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e32ca28af694bc1bbf399c33a516dbdf1c90090b8ab23c2bc24f834aa2247f5f"
+checksum = "79ea77c539259495ce8ca47f53e66ae0330a8819f67e23ac96ca02f50e7b7d36"
 dependencies = [
  "log",
  "ring",
  "rustls-webpki",
  "sct",
 ]
 
@@ -2325,33 +2311,33 @@
 checksum = "2d3987094b1d07b653b7dfdc3f70ce9a1da9c51ac18c1b06b662e4f9a0e9f4b2"
 dependencies = [
  "base64",
 ]
 
 [[package]]
 name = "rustls-webpki"
-version = "0.100.1"
+version = "0.101.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d6207cd5ed3d8dca7816f8f3725513a34609c0c765bf652b8c3cb4cfd87db46b"
+checksum = "15f36a6828982f422756984e47912a7a51dcbc2a197aa791158f8ca61cd8204e"
 dependencies = [
  "ring",
  "untrusted",
 ]
 
 [[package]]
 name = "rustversion"
-version = "1.0.12"
+version = "1.0.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4f3208ce4d8448b3f3e7d168a73f5e0c43a61e32930de3bceeccedb388b6bf06"
+checksum = "7ffc183a10b4478d04cbbbfc96d0873219d962dd5accaff2ffbd4ceb7df837f4"
 
 [[package]]
 name = "ryu"
-version = "1.0.13"
+version = "1.0.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f91339c0467de62360649f8d3e185ca8de4224ff281f66000de5eb2a77a79041"
+checksum = "1ad4cc8da4ef723ed60bced201181d83791ad433213d8c24efffda1eec85d741"
 
 [[package]]
 name = "same-file"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "93fc1dc3aaa9bfed95e02e6eadabb4baf7e3078b0bd1b4d7b6b0b68378900502"
 dependencies = [
@@ -2380,58 +2366,58 @@
  "quote",
  "serde_derive_internals",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "scopeguard"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
+checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "sct"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d53dcdb7c9f8158937a7981b48accfd39a43af418591a5d008c7b22b5e1b7ca4"
 dependencies = [
  "ring",
  "untrusted",
 ]
 
 [[package]]
 name = "semver"
-version = "1.0.17"
+version = "1.0.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bebd363326d05ec3e2f532ab7660680f3b02130d780c299bca73469d521bc0ed"
+checksum = "b0293b4b29daaf487284529cc2f5675b8e57c61f70167ba415a463651fd6a918"
 
 [[package]]
 name = "seq-macro"
-version = "0.3.3"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e6b44e8fc93a14e66336d230954dda83d18b4605ccace8fe09bc7514a71ad0bc"
+checksum = "a3f0bf26fd526d2a95683cd0f87bf103b8539e2ca1ef48ce002d67aad59aa0b4"
 
 [[package]]
 name = "serde"
-version = "1.0.164"
+version = "1.0.175"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9e8c8cf938e98f769bc164923b06dce91cea1751522f46f8466461af04c9027d"
+checksum = "5d25439cd7397d044e2748a6fe2432b5e85db703d6d097bd014b3c0ad1ebff0b"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.164"
+version = "1.0.175"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d9735b638ccc51c28bf6914d90a2e9725b377144fc612c49a611fddd1b631d68"
+checksum = "b23f7ade6f110613c0d63858ddb8b94c1041f550eab58a16b371bdf2c9c80ab4"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.22",
+ "syn 2.0.27",
 ]
 
 [[package]]
 name = "serde_derive_internals"
 version = "0.26.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "85bf8229e7920a9f636479437026331ce11aa132b4dde37d121944a44d6e5f3c"
@@ -2439,17 +2425,17 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.99"
+version = "1.0.103"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "46266871c240a00b8f503b877622fe33430b3c7d963bdc0f2adc511e54a1eae3"
+checksum = "d03b412469450d4404fe8499a268edd7f8b79fecb074b0d812ad64ca21f4031b"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -2457,15 +2443,15 @@
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8a00ffd23fd882d096f09fcaae2a9de8329a328628e86027e049ee051dc1621f"
 dependencies = [
  "proc-macro2",
  "quote",
  "serde",
- "syn 2.0.22",
+ "syn 2.0.27",
 ]
 
 [[package]]
 name = "serde_urlencoded"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d3491c14715ca2294c4d6a88f15e84739788c1d030eed8c110436aafdaa2f3fd"
@@ -2474,17 +2460,17 @@
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
 name = "serde_yaml"
-version = "0.9.22"
+version = "0.9.25"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "452e67b9c20c37fa79df53201dc03839651086ed9bbe92b3ca585ca9fdaa7d85"
+checksum = "1a49e178e4452f45cb61d0cd8cebc1b0fafd3e41929e996cef79aa3aca91f574"
 dependencies = [
  "indexmap 2.0.0",
  "itoa",
  "ryu",
  "serde",
  "unsafe-libyaml",
 ]
@@ -2513,33 +2499,33 @@
 checksum = "6528351c9bc8ab22353f9d776db39a20288e8d6c37ef8cfe3317cf875eecfc2d"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "smallvec"
-version = "1.10.0"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
+checksum = "62bb4feee49fdd9f707ef802e22365a35de4b7b299de4763d44bfea899442ff9"
 
 [[package]]
 name = "snafu"
-version = "0.7.4"
+version = "0.7.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cb0656e7e3ffb70f6c39b3c2a86332bb74aa3c679da781642590f3c1118c5045"
+checksum = "e4de37ad025c587a29e8f3f5605c00f70b98715ef90b9061a815b9e59e9042d6"
 dependencies = [
  "doc-comment",
  "snafu-derive",
 ]
 
 [[package]]
 name = "snafu-derive"
-version = "0.7.4"
+version = "0.7.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "475b3bbe5245c26f2d8a6f62d67c1f30eb9fffeccee721c45d162c3ebbdf81b2"
+checksum = "990079665f075b699031e9c08fd3ab99be5029b96f3b78dc0709e8f77e4efebf"
 dependencies = [
  "heck",
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
@@ -2600,15 +2586,15 @@
 
 [[package]]
 name = "strum"
 version = "0.25.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "290d54ea6f91c969195bdbcd7442c8c2a2ba87da8bf60a7ee86a235d4bc1e125"
 dependencies = [
- "strum_macros 0.25.0",
+ "strum_macros 0.25.1",
 ]
 
 [[package]]
 name = "strum_macros"
 version = "0.24.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1e385be0d24f186b4ce2f9982191e7101bb737312ad61c1f2f984f34bcf85d59"
@@ -2618,44 +2604,44 @@
  "quote",
  "rustversion",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "strum_macros"
-version = "0.25.0"
+version = "0.25.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fe9f3bd7d2e45dcc5e265fbb88d6513e4747d8ef9444cf01a533119bce28a157"
+checksum = "6069ca09d878a33f883cc06aaa9718ede171841d3832450354410b718b097232"
 dependencies = [
  "heck",
  "proc-macro2",
  "quote",
  "rustversion",
- "syn 2.0.22",
+ "syn 2.0.27",
 ]
 
 [[package]]
 name = "substrait"
-version = "0.11.0"
+version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7d3b77ddddd080d1bb5ebfe6b62d1c4e2f33c9f6a4586d5eac5306a08f3d4585"
+checksum = "2ac1ce8315086b127ca0abf162c62279550942bb26ebf7946fe17fe114446472"
 dependencies = [
  "git2",
  "heck",
  "prettyplease",
  "prost",
  "prost-build",
  "prost-types",
  "protobuf-src",
  "schemars",
  "semver",
  "serde",
  "serde_json",
  "serde_yaml",
- "syn 2.0.22",
+ "syn 2.0.27",
  "typify",
  "walkdir",
 ]
 
 [[package]]
 name = "subtle"
 version = "2.5.0"
@@ -2671,61 +2657,60 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.22"
+version = "2.0.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2efbeae7acf4eabd6bcdcbd11c92f45231ddda7539edc7806bd1a04a03b24616"
+checksum = "b60f673f44a8255b9c8c657daf66a596d435f2da81a555b06dc644d080ba45e0"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.8"
+version = "0.12.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1b1c7f239eb94671427157bd93b3694320f3668d4e1eff08c7285366fd777fac"
+checksum = "1d2faeef5759ab89935255b1a4cd98e0baf99d1085e37d36599c625dac49ae8e"
 
 [[package]]
 name = "tempfile"
-version = "3.6.0"
+version = "3.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "31c0432476357e58790aaa47a8efb0c5138f137343f3b5f23bd36a27e3b0a6d6"
+checksum = "5486094ee78b2e5038a6382ed7645bc084dc2ec433426ca4c3cb61e2007b8998"
 dependencies = [
- "autocfg",
  "cfg-if",
  "fastrand",
  "redox_syscall",
  "rustix",
  "windows-sys",
 ]
 
 [[package]]
 name = "thiserror"
-version = "1.0.40"
+version = "1.0.44"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "978c9a314bd8dc99be594bc3c175faaa9794be04a5a5e153caba6915336cebac"
+checksum = "611040a08a0439f8248d1990b111c95baa9c704c805fa1f62104b39655fd7f90"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.40"
+version = "1.0.44"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
+checksum = "090198534930841fab3a5d1bb637cde49e339654e606195f8d9c76eeb081dc96"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.22",
+ "syn 2.0.27",
 ]
 
 [[package]]
 name = "thrift"
 version = "0.17.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7e54bc85fc7faa8bc175c4bab5b92ba8d9a3ce893d0e9f42cc455c8ab16a9e09"
@@ -2782,15 +2767,15 @@
 name = "tokio-macros"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "630bdcf245f78637c13ec01ffae6187cca34625e8c63150d424b59e55af2675e"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.22",
+ "syn 2.0.27",
 ]
 
 [[package]]
 name = "tokio-rustls"
 version = "0.24.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c28327cf380ac148141087fbfb9de9d7bd4e84ab5d2c28fbc911d753de8a7081"
@@ -2835,15 +2820,15 @@
 name = "tracing-attributes"
 version = "0.1.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5f4f31f56159e98206da9efd823404b79b6ef3143b4a7ab76e67b1751b25a4ab"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.22",
+ "syn 2.0.27",
 ]
 
 [[package]]
 name = "tracing-core"
 version = "0.1.31"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0955b8137a1df6f1a2e9a37d8a6656291ff0297c1a97c24e0d8425fe2312f79a"
@@ -2903,15 +2888,15 @@
  "heck",
  "log",
  "proc-macro2",
  "quote",
  "regress",
  "schemars",
  "serde_json",
- "syn 2.0.22",
+ "syn 2.0.27",
  "thiserror",
  "unicode-ident",
 ]
 
 [[package]]
 name = "typify-macro"
 version = "0.0.13"
@@ -2920,29 +2905,29 @@
 dependencies = [
  "proc-macro2",
  "quote",
  "schemars",
  "serde",
  "serde_json",
  "serde_tokenstream",
- "syn 2.0.22",
+ "syn 2.0.27",
  "typify-impl",
 ]
 
 [[package]]
 name = "unicode-bidi"
 version = "0.3.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "92888ba5573ff080736b3648696b70cafad7d250551175acbaa4e0385b3e1460"
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.9"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b15811caf2415fb889178633e7724bad2509101cde276048e013b9def5e51fa0"
+checksum = "301abaae475aa91687eb82514b328ab47a211a533026cb25fc3e519b86adfc3c"
 
 [[package]]
 name = "unicode-normalization"
 version = "0.1.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c5713f0fc4b5db668a2ac63cdb7bb4469d8c9fed047b1d0292cc7b0ce2ba921"
 dependencies = [
@@ -2965,17 +2950,17 @@
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
 [[package]]
 name = "unsafe-libyaml"
-version = "0.2.8"
+version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1865806a559042e51ab5414598446a5871b561d21b6764f2eabb0dd481d880a6"
+checksum = "f28467d3e1d3c6586d8f25fa243f544f5800fec42d97032474e17222c2b75cfa"
 
 [[package]]
 name = "untrusted"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a156c684c91ea7d62626509bce3cb4e1d9ed5c4d978f7b4352658f96a4c26b4a"
 
@@ -2988,17 +2973,17 @@
  "form_urlencoded",
  "idna",
  "percent-encoding",
 ]
 
 [[package]]
 name = "uuid"
-version = "1.4.0"
+version = "1.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d023da39d1fde5a8a3fe1f3e01ca9632ada0a63e9797de55a879d6e2236277be"
+checksum = "79daa5ed5740825c40b389c5e50312b9c86df53fccd33f281df655642b43869d"
 dependencies = [
  "getrandom",
  "serde",
 ]
 
 [[package]]
 name = "vcpkg"
@@ -3054,15 +3039,15 @@
 checksum = "5ef2b6d3c510e9625e5fe6f509ab07d66a760f0885d858736483c32ed7809abd"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.22",
+ "syn 2.0.27",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-futures"
 version = "0.4.37"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -3088,15 +3073,15 @@
 name = "wasm-bindgen-macro-support"
 version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "54681b18a46765f095758388f2d0cf16eb8d4169b639ab575a8f5693af210c7b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.22",
+ "syn 2.0.27",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.87"
@@ -3299,26 +3284,26 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "zstd"
-version = "0.12.3+zstd.1.5.2"
+version = "0.12.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "76eea132fb024e0e13fd9c2f5d5d595d8a967aa72382ac2f9d39fcc95afd0806"
+checksum = "1a27595e173641171fc74a1232b7b1c7a7cb6e18222c11e9dfb9888fa424c53c"
 dependencies = [
  "zstd-safe",
 ]
 
 [[package]]
 name = "zstd-safe"
-version = "6.0.5+zstd.1.5.4"
+version = "6.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d56d9e60b4b1758206c238a10165fbcae3ca37b01744e394c463463f6529d23b"
+checksum = "ee98ffd0b48ee95e6c5168188e44a54550b1564d9d530ee21d5f0eaed1069581"
 dependencies = [
  "libc",
  "zstd-sys",
 ]
 
 [[package]]
 name = "zstd-sys"
```

### Comparing `datafusion-27.0.0/PKG-INFO` & `datafusion-28.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datafusion
-Version: 27.0.0
+Version: 28.0.0
 Requires-Dist: pyarrow >=11.0.0
 License-File: LICENSE.txt
 Summary: Build and run queries against data
 Keywords: datafusion,dataframe,rust,query-engine
 Home-Page: https://github.com/apache/arrow-datafusion-python
 Author: Apache Arrow <dev@arrow.apache.org>
 Author-email: Apache Arrow <dev@arrow.apache.org>
```

