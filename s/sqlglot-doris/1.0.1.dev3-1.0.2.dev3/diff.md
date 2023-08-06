# Comparing `tmp/sqlglot-doris-1.0.1.dev3.tar.gz` & `tmp/sqlglot-doris-1.0.2.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlglot-doris-1.0.1.dev3.tar", last modified: Fri Aug  4 11:01:44 2023, max compression
+gzip compressed data, was "sqlglot-doris-1.0.2.dev3.tar", last modified: Sun Aug  6 11:26:19 2023, max compression
```

## Comparing `sqlglot-doris-1.0.1.dev3.tar` & `sqlglot-doris-1.0.2.dev3.tar`

### file list

```diff
@@ -1,311 +1,314 @@
-drwxr-xr-x   0 liujiwen   (501) staff       (20)        0 2023-08-04 11:01:44.821770 sqlglot-doris-1.0.1.dev3/
-drwxr-xr-x   0 liujiwen   (501) staff       (20)        0 2023-08-04 11:01:44.593322 sqlglot-doris-1.0.1.dev3/.github/
-drwxr-xr-x   0 liujiwen   (501) staff       (20)        0 2023-08-04 11:01:44.609266 sqlglot-doris-1.0.1.dev3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 liujiwen   (501) staff       (20)      488 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 liujiwen   (501) staff       (20)      595 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 liujiwen   (501) staff       (20)        0 2023-08-04 11:01:44.609793 sqlglot-doris-1.0.1.dev3/.github/workflows/
--rw-r--r--   0 liujiwen   (501) staff       (20)      629 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/.github/workflows/python-package.yml
--rw-r--r--   0 liujiwen   (501) staff       (20)     1125 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/.github/workflows/python-publish.yml
--rw-r--r--   0 liujiwen   (501) staff       (20)     1923 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/.gitignore
--rw-r--r--   0 liujiwen   (501) staff       (20)      815 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/.pre-commit-config.yaml
--rw-r--r--   0 liujiwen   (501) staff       (20)   110654 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/CHANGELOG.md
--rw-r--r--   0 liujiwen   (501) staff       (20)     2374 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/CONTRIBUTING.md
--rw-r--r--   0 liujiwen   (501) staff       (20)     1065 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/LICENSE
--rw-r--r--   0 liujiwen   (501) staff       (20)      401 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/Makefile
--rw-r--r--   0 liujiwen   (501) staff       (20)     4133 2023-08-04 11:01:44.821864 sqlglot-doris-1.0.1.dev3/PKG-INFO
--rw-r--r--   0 liujiwen   (501) staff       (20)     3476 2023-08-04 10:47:19.000000 sqlglot-doris-1.0.1.dev3/README.md
-drwxr-xr-x   0 liujiwen   (501) staff       (20)        0 2023-08-04 11:01:44.609979 sqlglot-doris-1.0.1.dev3/benchmarks/
--rw-r--r--   0 liujiwen   (501) staff       (20)     6977 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/benchmarks/bench.py
-drwxr-xr-x   0 liujiwen   (501) staff       (20)        0 2023-08-04 11:01:44.624659 sqlglot-doris-1.0.1.dev3/docs/
--rw-r--r--   0 liujiwen   (501) staff       (20)       11 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/docs/CNAME
--rw-r--r--   0 liujiwen   (501) staff       (20)      138 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/docs/index.html
--rw-r--r--   0 liujiwen   (501) staff       (20) 10482048 2023-08-04 09:00:00.000000 sqlglot-doris-1.0.1.dev3/docs/search.js
-drwxr-xr-x   0 liujiwen   (501) staff       (20)        0 2023-08-04 11:01:44.678298 sqlglot-doris-1.0.1.dev3/docs/sqlglot/
--rw-r--r--   0 liujiwen   (501) staff       (20)    36724 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/docs/sqlglot/_typing.html
--rw-r--r--   0 liujiwen   (501) staff       (20)    36080 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/docs/sqlglot/_version.html
-drwxr-xr-x   0 liujiwen   (501) staff       (20)        0 2023-08-04 11:01:44.679817 sqlglot-doris-1.0.1.dev3/docs/sqlglot/dataframe/
--rw-r--r--   0 liujiwen   (501) staff       (20)   985439 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/docs/sqlglot/dataframe/sql.html
--rw-r--r--   0 liujiwen   (501) staff       (20)    66466 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/docs/sqlglot/dataframe.html
-drwxr-xr-x   0 liujiwen   (501) staff       (20)        0 2023-08-04 11:01:44.744797 sqlglot-doris-1.0.1.dev3/docs/sqlglot/dialects/
--rw-r--r--   0 liujiwen   (501) staff       (20)   682043 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/docs/sqlglot/dialects/bigquery.html
--rw-r--r--   0 liujiwen   (501) staff       (20)   604442 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/docs/sqlglot/dialects/clickhouse.html
--rw-r--r--   0 liujiwen   (501) staff       (20)   234037 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/docs/sqlglot/dialects/databricks.html
--rw-r--r--   0 liujiwen   (501) staff       (20)   504902 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/docs/sqlglot/dialects/dialect.html
--rw-r--r--   0 liujiwen   (501) staff       (20)   323631 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/docs/sqlglot/dialects/drill.html
--rw-r--r--   0 liujiwen   (501) staff       (20)   456420 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/docs/sqlglot/dialects/duckdb.html
--rw-r--r--   0 liujiwen   (501) staff       (20)   576965 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/docs/sqlglot/dialects/hive.html
--rw-r--r--   0 liujiwen   (501) staff       (20)   773372 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/docs/sqlglot/dialects/mysql.html
--rw-r--r--   0 liujiwen   (501) staff       (20)   369087 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/docs/sqlglot/dialects/oracle.html
--rw-r--r--   0 liujiwen   (501) staff       (20)   480863 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/docs/sqlglot/dialects/postgres.html
--rw-r--r--   0 liujiwen   (501) staff       (20)   519013 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/docs/sqlglot/dialects/presto.html
--rw-r--r--   0 liujiwen   (501) staff       (20)   363269 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/docs/sqlglot/dialects/redshift.html
--rw-r--r--   0 liujiwen   (501) staff       (20)   535303 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/docs/sqlglot/dialects/snowflake.html
--rw-r--r--   0 liujiwen   (501) staff       (20)   227931 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/docs/sqlglot/dialects/spark.html
--rw-r--r--   0 liujiwen   (501) staff       (20)   395132 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/docs/sqlglot/dialects/spark2.html
--rw-r--r--   0 liujiwen   (501) staff       (20)   353049 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/docs/sqlglot/dialects/sqlite.html
--rw-r--r--   0 liujiwen   (501) staff       (20)   221352 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/docs/sqlglot/dialects/starrocks.html
--rw-r--r--   0 liujiwen   (501) staff       (20)   219461 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/docs/sqlglot/dialects/tableau.html
--rw-r--r--   0 liujiwen   (501) staff       (20)   382689 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/docs/sqlglot/dialects/teradata.html
--rw-r--r--   0 liujiwen   (501) staff       (20)   147383 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/docs/sqlglot/dialects/trino.html
--rw-r--r--   0 liujiwen   (501) staff       (20)   715570 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/docs/sqlglot/dialects/tsql.html
--rw-r--r--   0 liujiwen   (501) staff       (20)    55816 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/docs/sqlglot/dialects.html
--rw-r--r--   0 liujiwen   (501) staff       (20)   283781 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/docs/sqlglot/diff.html
--rw-r--r--   0 liujiwen   (501) staff       (20)   100430 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/docs/sqlglot/errors.html
-drwxr-xr-x   0 liujiwen   (501) staff       (20)        0 2023-08-04 11:01:44.751825 sqlglot-doris-1.0.1.dev3/docs/sqlglot/executor/
--rw-r--r--   0 liujiwen   (501) staff       (20)   117988 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/docs/sqlglot/executor/context.html
--rw-r--r--   0 liujiwen   (501) staff       (20)   131973 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/docs/sqlglot/executor/env.html
--rw-r--r--   0 liujiwen   (501) staff       (20)   506241 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/docs/sqlglot/executor/python.html
--rw-r--r--   0 liujiwen   (501) staff       (20)   118949 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/docs/sqlglot/executor/table.html
--rw-r--r--   0 liujiwen   (501) staff       (20)    92941 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/docs/sqlglot/executor.html
--rw-r--r--   0 liujiwen   (501) staff       (20)  6751372 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/docs/sqlglot/expressions.html
--rw-r--r--   0 liujiwen   (501) staff       (20)  2963956 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/docs/sqlglot/generator.html
--rw-r--r--   0 liujiwen   (501) staff       (20)   226523 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/docs/sqlglot/helper.html
--rw-r--r--   0 liujiwen   (501) staff       (20)   190366 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/docs/sqlglot/lineage.html
-drwxr-xr-x   0 liujiwen   (501) staff       (20)        0 2023-08-04 11:01:44.767272 sqlglot-doris-1.0.1.dev3/docs/sqlglot/optimizer/
--rw-r--r--   0 liujiwen   (501) staff       (20)   294349 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/docs/sqlglot/optimizer/annotate_types.html
--rw-r--r--   0 liujiwen   (501) staff       (20)    76888 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/docs/sqlglot/optimizer/canonicalize.html
--rw-r--r--   0 liujiwen   (501) staff       (20)    53615 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/docs/sqlglot/optimizer/eliminate_ctes.html
--rw-r--r--   0 liujiwen   (501) staff       (20)    99196 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/docs/sqlglot/optimizer/eliminate_joins.html
--rw-r--r--   0 liujiwen   (501) staff       (20)   100353 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/docs/sqlglot/optimizer/eliminate_subqueries.html
--rw-r--r--   0 liujiwen   (501) staff       (20)    51199 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/docs/sqlglot/optimizer/expand_laterals.html
--rw-r--r--   0 liujiwen   (501) staff       (20)    45966 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/docs/sqlglot/optimizer/expand_multi_table_selects.html
--rw-r--r--   0 liujiwen   (501) staff       (20)    51584 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/docs/sqlglot/optimizer/isolate_table_selects.html
--rw-r--r--   0 liujiwen   (501) staff       (20)    63180 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/docs/sqlglot/optimizer/lower_identities.html
--rw-r--r--   0 liujiwen   (501) staff       (20)   150542 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/docs/sqlglot/optimizer/merge_subqueries.html
--rw-r--r--   0 liujiwen   (501) staff       (20)   107750 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/docs/sqlglot/optimizer/normalize.html
--rw-r--r--   0 liujiwen   (501) staff       (20)    48102 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/docs/sqlglot/optimizer/normalize_identifiers.html
--rw-r--r--   0 liujiwen   (501) staff       (20)    76872 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/docs/sqlglot/optimizer/optimize_joins.html
--rw-r--r--   0 liujiwen   (501) staff       (20)    73565 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/docs/sqlglot/optimizer/optimizer.html
--rw-r--r--   0 liujiwen   (501) staff       (20)   134865 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/docs/sqlglot/optimizer/pushdown_predicates.html
--rw-r--r--   0 liujiwen   (501) staff       (20)    83923 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/docs/sqlglot/optimizer/pushdown_projections.html
--rw-r--r--   0 liujiwen   (501) staff       (20)    70870 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/docs/sqlglot/optimizer/qualify.html
--rw-r--r--   0 liujiwen   (501) staff       (20)   263034 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/docs/sqlglot/optimizer/qualify_columns.html
--rw-r--r--   0 liujiwen   (501) staff       (20)    91897 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/docs/sqlglot/optimizer/qualify_tables.html
--rw-r--r--   0 liujiwen   (501) staff       (20)   392396 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/docs/sqlglot/optimizer/scope.html
--rw-r--r--   0 liujiwen   (501) staff       (20)   288965 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/docs/sqlglot/optimizer/simplify.html
--rw-r--r--   0 liujiwen   (501) staff       (20)   161494 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/docs/sqlglot/optimizer/unnest_subqueries.html
--rw-r--r--   0 liujiwen   (501) staff       (20)    37556 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/docs/sqlglot/optimizer.html
--rw-r--r--   0 liujiwen   (501) staff       (20)  2838889 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/docs/sqlglot/parser.html
--rw-r--r--   0 liujiwen   (501) staff       (20)   376114 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/docs/sqlglot/planner.html
--rw-r--r--   0 liujiwen   (501) staff       (20)   359917 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/docs/sqlglot/schema.html
--rw-r--r--   0 liujiwen   (501) staff       (20)    71553 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/docs/sqlglot/serde.html
--rw-r--r--   0 liujiwen   (501) staff       (20)    58338 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/docs/sqlglot/time.html
--rw-r--r--   0 liujiwen   (501) staff       (20)   832183 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/docs/sqlglot/tokens.html
--rw-r--r--   0 liujiwen   (501) staff       (20)   200755 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/docs/sqlglot/transforms.html
--rw-r--r--   0 liujiwen   (501) staff       (20)    71915 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/docs/sqlglot/trie.html
--rw-r--r--   0 liujiwen   (501) staff       (20)   145333 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/docs/sqlglot.html
-drwxr-xr-x   0 liujiwen   (501) staff       (20)        0 2023-08-04 11:01:44.768064 sqlglot-doris-1.0.1.dev3/pdoc/
--rwxr-xr-x   0 liujiwen   (501) staff       (20)     1114 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/pdoc/cli.py
-drwxr-xr-x   0 liujiwen   (501) staff       (20)        0 2023-08-04 11:01:44.768376 sqlglot-doris-1.0.1.dev3/pdoc/templates/
--rw-r--r--   0 liujiwen   (501) staff       (20)      131 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/pdoc/templates/module.html.jinja2
-drwxr-xr-x   0 liujiwen   (501) staff       (20)        0 2023-08-04 11:01:44.768778 sqlglot-doris-1.0.1.dev3/posts/
--rw-r--r--   0 liujiwen   (501) staff       (20)    12086 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/posts/python_sql_engine.md
-drwxr-xr-x   0 liujiwen   (501) staff       (20)        0 2023-08-04 11:01:44.772543 sqlglot-doris-1.0.1.dev3/posts/python_sql_engine_images/
--rw-r--r--   0 liujiwen   (501) staff       (20)    32441 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/posts/python_sql_engine_images/executor.png
--rw-r--r--   0 liujiwen   (501) staff       (20)    82195 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/posts/python_sql_engine_images/optimizer.png
--rw-r--r--   0 liujiwen   (501) staff       (20)   157268 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/posts/python_sql_engine_images/parser.png
--rw-r--r--   0 liujiwen   (501) staff       (20)   123866 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/posts/python_sql_engine_images/planner.png
--rw-r--r--   0 liujiwen   (501) staff       (20)   341375 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/posts/python_sql_engine_images/tokenizer.png
--rw-r--r--   0 liujiwen   (501) staff       (20)    26210 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/posts/sql_diff.md
-drwxr-xr-x   0 liujiwen   (501) staff       (20)        0 2023-08-04 11:01:44.779394 sqlglot-doris-1.0.1.dev3/posts/sql_diff_images/
--rw-r--r--   0 liujiwen   (501) staff       (20)    22582 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/posts/sql_diff_images/dice_coef.png
--rw-r--r--   0 liujiwen   (501) staff       (20)    57550 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/posts/sql_diff_images/figure_1.png
--rw-r--r--   0 liujiwen   (501) staff       (20)  1511115 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/posts/sql_diff_images/figure_2.gif
--rw-r--r--   0 liujiwen   (501) staff       (20)   327145 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/posts/sql_diff_images/figure_3.gif
--rw-r--r--   0 liujiwen   (501) staff       (20)    41567 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/posts/sql_diff_images/git_diff_output.png
--rw-r--r--   0 liujiwen   (501) staff       (20)    35159 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/posts/sql_diff_images/matching_criteria_1.png
--rw-r--r--   0 liujiwen   (501) staff       (20)    48555 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/posts/sql_diff_images/matching_criteria_2.png
--rw-r--r--   0 liujiwen   (501) staff       (20)      529 2023-08-04 11:01:44.822168 sqlglot-doris-1.0.1.dev3/setup.cfg
--rw-r--r--   0 liujiwen   (501) staff       (20)     1368 2023-08-04 11:01:20.000000 sqlglot-doris-1.0.1.dev3/setup.py
-drwxr-xr-x   0 liujiwen   (501) staff       (20)        0 2023-08-04 11:01:44.784484 sqlglot-doris-1.0.1.dev3/sqlglot/
--rw-r--r--   0 liujiwen   (501) staff       (20)     4882 2023-08-04 08:59:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/__init__.py
--rw-r--r--   0 liujiwen   (501) staff       (20)     1936 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/__main__.py
--rw-r--r--   0 liujiwen   (501) staff       (20)      142 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/_typing.py
--rw-r--r--   0 liujiwen   (501) staff       (20)      175 2023-08-04 10:57:10.000000 sqlglot-doris-1.0.1.dev3/sqlglot/_version.py
-drwxr-xr-x   0 liujiwen   (501) staff       (20)        0 2023-08-04 11:01:44.784759 sqlglot-doris-1.0.1.dev3/sqlglot/dataframe/
--rw-r--r--   0 liujiwen   (501) staff       (20)     7885 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/dataframe/README.md
--rw-r--r--   0 liujiwen   (501) staff       (20)       37 2023-08-04 08:59:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/dataframe/__init__.py
-drwxr-xr-x   0 liujiwen   (501) staff       (20)        0 2023-08-04 11:01:44.787001 sqlglot-doris-1.0.1.dev3/sqlglot/dataframe/sql/
--rw-r--r--   0 liujiwen   (501) staff       (20)      560 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/dataframe/sql/__init__.py
--rw-r--r--   0 liujiwen   (501) staff       (20)      643 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/dataframe/sql/_typing.py
--rw-r--r--   0 liujiwen   (501) staff       (20)    12583 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/dataframe/sql/column.py
--rw-r--r--   0 liujiwen   (501) staff       (20)    37147 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/dataframe/sql/dataframe.py
--rw-r--r--   0 liujiwen   (501) staff       (20)    42238 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/dataframe/sql/functions.py
--rw-r--r--   0 liujiwen   (501) staff       (20)     2162 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/dataframe/sql/group.py
--rw-r--r--   0 liujiwen   (501) staff       (20)     3326 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/dataframe/sql/normalize.py
--rw-r--r--   0 liujiwen   (501) staff       (20)     1765 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/dataframe/sql/operations.py
--rw-r--r--   0 liujiwen   (501) staff       (20)     3085 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/dataframe/sql/readwriter.py
--rw-r--r--   0 liujiwen   (501) staff       (20)     5338 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/dataframe/sql/session.py
--rw-r--r--   0 liujiwen   (501) staff       (20)      301 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/dataframe/sql/transforms.py
--rw-r--r--   0 liujiwen   (501) staff       (20)     5189 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/dataframe/sql/types.py
--rw-r--r--   0 liujiwen   (501) staff       (20)     1142 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/dataframe/sql/util.py
--rw-r--r--   0 liujiwen   (501) staff       (20)     4675 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/dataframe/sql/window.py
-drwxr-xr-x   0 liujiwen   (501) staff       (20)        0 2023-08-04 11:01:44.790836 sqlglot-doris-1.0.1.dev3/sqlglot/dialects/
--rw-r--r--   0 liujiwen   (501) staff       (20)     3041 2023-08-04 02:52:53.000000 sqlglot-doris-1.0.1.dev3/sqlglot/dialects/__init__.py
--rw-r--r--   0 liujiwen   (501) staff       (20)    22780 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/dialects/bigquery.py
--rw-r--r--   0 liujiwen   (501) staff       (20)    15734 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/dialects/clickhouse.py
--rw-r--r--   0 liujiwen   (501) staff       (20)     1501 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/dialects/databricks.py
--rw-r--r--   0 liujiwen   (501) staff       (20)    24291 2023-08-04 02:48:47.000000 sqlglot-doris-1.0.1.dev3/sqlglot/dialects/dialect.py
--rw-r--r--   0 liujiwen   (501) staff       (20)     2866 2023-08-04 09:15:52.000000 sqlglot-doris-1.0.1.dev3/sqlglot/dialects/doris.py
--rw-r--r--   0 liujiwen   (501) staff       (20)     5805 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/dialects/drill.py
--rw-r--r--   0 liujiwen   (501) staff       (20)    12542 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/dialects/duckdb.py
--rw-r--r--   0 liujiwen   (501) staff       (20)    19667 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/dialects/hive.py
--rw-r--r--   0 liujiwen   (501) staff       (20)    25564 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/dialects/mysql.py
--rw-r--r--   0 liujiwen   (501) staff       (20)     7330 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/dialects/oracle.py
--rw-r--r--   0 liujiwen   (501) staff       (20)    15380 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/dialects/postgres.py
--rw-r--r--   0 liujiwen   (501) staff       (20)    16583 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/dialects/presto.py
--rw-r--r--   0 liujiwen   (501) staff       (20)     6127 2023-08-04 06:20:47.000000 sqlglot-doris-1.0.1.dev3/sqlglot/dialects/redshift.py
--rw-r--r--   0 liujiwen   (501) staff       (20)    16583 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/dialects/snowflake.py
--rw-r--r--   0 liujiwen   (501) staff       (20)     2073 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/dialects/spark.py
--rw-r--r--   0 liujiwen   (501) staff       (20)    10739 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/dialects/spark2.py
--rw-r--r--   0 liujiwen   (501) staff       (20)     7543 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/dialects/sqlite.py
--rw-r--r--   0 liujiwen   (501) staff       (20)     1678 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/dialects/starrocks.py
--rw-r--r--   0 liujiwen   (501) staff       (20)     1402 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/dialects/tableau.py
--rw-r--r--   0 liujiwen   (501) staff       (20)     8478 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/dialects/teradata.py
--rw-r--r--   0 liujiwen   (501) staff       (20)      429 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/dialects/trino.py
--rw-r--r--   0 liujiwen   (501) staff       (20)    24905 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/dialects/tsql.py
--rw-r--r--   0 liujiwen   (501) staff       (20)    14048 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/diff.py
--rw-r--r--   0 liujiwen   (501) staff       (20)     2126 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/errors.py
-drwxr-xr-x   0 liujiwen   (501) staff       (20)        0 2023-08-04 11:01:44.791495 sqlglot-doris-1.0.1.dev3/sqlglot/executor/
--rw-r--r--   0 liujiwen   (501) staff       (20)     2620 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/executor/__init__.py
--rw-r--r--   0 liujiwen   (501) staff       (20)     3357 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/executor/context.py
--rw-r--r--   0 liujiwen   (501) staff       (20)     6679 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/executor/env.py
--rw-r--r--   0 liujiwen   (501) staff       (20)    15435 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/executor/python.py
--rw-r--r--   0 liujiwen   (501) staff       (20)     3423 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/executor/table.py
--rw-r--r--   0 liujiwen   (501) staff       (20)   162320 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/expressions.py
--rw-r--r--   0 liujiwen   (501) staff       (20)   111731 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/generator.py
--rw-r--r--   0 liujiwen   (501) staff       (20)    11200 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/helper.py
--rw-r--r--   0 liujiwen   (501) staff       (20)     8863 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/lineage.py
-drwxr-xr-x   0 liujiwen   (501) staff       (20)        0 2023-08-04 11:01:44.794335 sqlglot-doris-1.0.1.dev3/sqlglot/optimizer/
--rw-r--r--   0 liujiwen   (501) staff       (20)      127 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/optimizer/__init__.py
--rw-r--r--   0 liujiwen   (501) staff       (20)    14230 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/optimizer/annotate_types.py
--rw-r--r--   0 liujiwen   (501) staff       (20)     2755 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/optimizer/canonicalize.py
--rw-r--r--   0 liujiwen   (501) staff       (20)     1434 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/optimizer/eliminate_ctes.py
--rw-r--r--   0 liujiwen   (501) staff       (20)     5874 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/optimizer/eliminate_joins.py
--rw-r--r--   0 liujiwen   (501) staff       (20)     6473 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/optimizer/eliminate_subqueries.py
--rw-r--r--   0 liujiwen   (501) staff       (20)     1128 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/optimizer/isolate_table_selects.py
--rw-r--r--   0 liujiwen   (501) staff       (20)    14646 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/optimizer/merge_subqueries.py
--rw-r--r--   0 liujiwen   (501) staff       (20)     5547 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/optimizer/normalize.py
--rw-r--r--   0 liujiwen   (501) staff       (20)     1018 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/optimizer/normalize_identifiers.py
--rw-r--r--   0 liujiwen   (501) staff       (20)     2604 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/optimizer/optimize_joins.py
--rw-r--r--   0 liujiwen   (501) staff       (20)     3537 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/optimizer/optimizer.py
--rw-r--r--   0 liujiwen   (501) staff       (20)     7266 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/optimizer/pushdown_predicates.py
--rw-r--r--   0 liujiwen   (501) staff       (20)     4690 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/optimizer/pushdown_projections.py
--rw-r--r--   0 liujiwen   (501) staff       (20)     3098 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/optimizer/qualify.py
--rw-r--r--   0 liujiwen   (501) staff       (20)    22230 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/optimizer/qualify_columns.py
--rw-r--r--   0 liujiwen   (501) staff       (20)     4160 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/optimizer/qualify_tables.py
--rw-r--r--   0 liujiwen   (501) staff       (20)    26360 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/optimizer/scope.py
--rw-r--r--   0 liujiwen   (501) staff       (20)    18184 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/optimizer/simplify.py
--rw-r--r--   0 liujiwen   (501) staff       (20)     9494 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/optimizer/unnest_subqueries.py
--rw-r--r--   0 liujiwen   (501) staff       (20)   179631 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/parser.py
--rw-r--r--   0 liujiwen   (501) staff       (20)    14144 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/planner.py
--rw-r--r--   0 liujiwen   (501) staff       (20)        0 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/py.typed
--rw-r--r--   0 liujiwen   (501) staff       (20)    18067 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/schema.py
--rw-r--r--   0 liujiwen   (501) staff       (20)     2031 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/serde.py
--rw-r--r--   0 liujiwen   (501) staff       (20)     1418 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/time.py
--rw-r--r--   0 liujiwen   (501) staff       (20)    35304 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/tokens.py
--rw-r--r--   0 liujiwen   (501) staff       (20)    11699 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/transforms.py
--rw-r--r--   0 liujiwen   (501) staff       (20)     2245 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot/trie.py
--rw-r--r--   0 liujiwen   (501) staff       (20)     4208 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/sqlglot.svg
-drwxr-xr-x   0 liujiwen   (501) staff       (20)        0 2023-08-04 11:01:44.794825 sqlglot-doris-1.0.1.dev3/sqlglot_doris.egg-info/
--rw-r--r--   0 liujiwen   (501) staff       (20)     4133 2023-08-04 11:01:44.000000 sqlglot-doris-1.0.1.dev3/sqlglot_doris.egg-info/PKG-INFO
--rw-r--r--   0 liujiwen   (501) staff       (20)     8959 2023-08-04 11:01:44.000000 sqlglot-doris-1.0.1.dev3/sqlglot_doris.egg-info/SOURCES.txt
--rw-r--r--   0 liujiwen   (501) staff       (20)        1 2023-08-04 11:01:44.000000 sqlglot-doris-1.0.1.dev3/sqlglot_doris.egg-info/dependency_links.txt
--rw-r--r--   0 liujiwen   (501) staff       (20)      100 2023-08-04 11:01:44.000000 sqlglot-doris-1.0.1.dev3/sqlglot_doris.egg-info/requires.txt
--rw-r--r--   0 liujiwen   (501) staff       (20)        8 2023-08-04 11:01:44.000000 sqlglot-doris-1.0.1.dev3/sqlglot_doris.egg-info/top_level.txt
-drwxr-xr-x   0 liujiwen   (501) staff       (20)        0 2023-08-04 11:01:44.800730 sqlglot-doris-1.0.1.dev3/tests/
--rw-r--r--   0 liujiwen   (501) staff       (20)        0 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/__init__.py
-drwxr-xr-x   0 liujiwen   (501) staff       (20)        0 2023-08-04 11:01:44.800861 sqlglot-doris-1.0.1.dev3/tests/dataframe/
--rw-r--r--   0 liujiwen   (501) staff       (20)        0 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/dataframe/__init__.py
-drwxr-xr-x   0 liujiwen   (501) staff       (20)        0 2023-08-04 11:01:44.801666 sqlglot-doris-1.0.1.dev3/tests/dataframe/integration/
--rw-r--r--   0 liujiwen   (501) staff       (20)        0 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/dataframe/integration/__init__.py
--rw-r--r--   0 liujiwen   (501) staff       (20)     7670 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/dataframe/integration/dataframe_validator.py
--rw-r--r--   0 liujiwen   (501) staff       (20)    52342 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/dataframe/integration/test_dataframe.py
--rw-r--r--   0 liujiwen   (501) staff       (20)     3173 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/dataframe/integration/test_grouped_data.py
--rw-r--r--   0 liujiwen   (501) staff       (20)     1088 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/dataframe/integration/test_session.py
-drwxr-xr-x   0 liujiwen   (501) staff       (20)        0 2023-08-04 11:01:44.802912 sqlglot-doris-1.0.1.dev3/tests/dataframe/unit/
--rw-r--r--   0 liujiwen   (501) staff       (20)        0 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/dataframe/unit/__init__.py
--rw-r--r--   0 liujiwen   (501) staff       (20)     1582 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/dataframe/unit/dataframe_sql_validator.py
--rw-r--r--   0 liujiwen   (501) staff       (20)     6376 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/dataframe/unit/test_column.py
--rw-r--r--   0 liujiwen   (501) staff       (20)     2577 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/dataframe/unit/test_dataframe.py
--rw-r--r--   0 liujiwen   (501) staff       (20)     9354 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/dataframe/unit/test_dataframe_writer.py
--rw-r--r--   0 liujiwen   (501) staff       (20)    70790 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/dataframe/unit/test_functions.py
--rw-r--r--   0 liujiwen   (501) staff       (20)     5865 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/dataframe/unit/test_session.py
--rw-r--r--   0 liujiwen   (501) staff       (20)     2388 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/dataframe/unit/test_types.py
--rw-r--r--   0 liujiwen   (501) staff       (20)     3320 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/dataframe/unit/test_window.py
-drwxr-xr-x   0 liujiwen   (501) staff       (20)        0 2023-08-04 11:01:44.809760 sqlglot-doris-1.0.1.dev3/tests/dialects/
--rw-r--r--   0 liujiwen   (501) staff       (20)        0 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/dialects/__init__.py
--rw-r--r--   0 liujiwen   (501) staff       (20)    29997 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/dialects/test_bigquery.py
--rw-r--r--   0 liujiwen   (501) staff       (20)    18974 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/dialects/test_clickhouse.py
--rw-r--r--   0 liujiwen   (501) staff       (20)     8193 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/dialects/test_databricks.py
--rw-r--r--   0 liujiwen   (501) staff       (20)    69752 2023-08-04 03:30:02.000000 sqlglot-doris-1.0.1.dev3/tests/dialects/test_dialect.py
--rw-r--r--   0 liujiwen   (501) staff       (20)     2326 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/dialects/test_drill.py
--rw-r--r--   0 liujiwen   (501) staff       (20)    24085 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/dialects/test_duckdb.py
--rw-r--r--   0 liujiwen   (501) staff       (20)    26497 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/dialects/test_hive.py
--rw-r--r--   0 liujiwen   (501) staff       (20)    35751 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/dialects/test_mysql.py
--rw-r--r--   0 liujiwen   (501) staff       (20)     6695 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/dialects/test_oracle.py
--rw-r--r--   0 liujiwen   (501) staff       (20)    26820 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/dialects/test_postgres.py
--rw-r--r--   0 liujiwen   (501) staff       (20)    35008 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/dialects/test_presto.py
--rw-r--r--   0 liujiwen   (501) staff       (20)    14724 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/dialects/test_redshift.py
--rw-r--r--   0 liujiwen   (501) staff       (20)    43592 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/dialects/test_snowflake.py
--rw-r--r--   0 liujiwen   (501) staff       (20)    23040 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/dialects/test_spark.py
--rw-r--r--   0 liujiwen   (501) staff       (20)     6221 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/dialects/test_sqlite.py
--rw-r--r--   0 liujiwen   (501) staff       (20)      571 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/dialects/test_starrocks.py
--rw-r--r--   0 liujiwen   (501) staff       (20)     1715 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/dialects/test_tableau.py
--rw-r--r--   0 liujiwen   (501) staff       (20)     7216 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/dialects/test_teradata.py
--rw-r--r--   0 liujiwen   (501) staff       (20)    42172 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/dialects/test_tsql.py
-drwxr-xr-x   0 liujiwen   (501) staff       (20)        0 2023-08-04 11:01:44.810662 sqlglot-doris-1.0.1.dev3/tests/fixtures/
--rw-r--r--   0 liujiwen   (501) staff       (20)    34464 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/fixtures/identity.sql
-drwxr-xr-x   0 liujiwen   (501) staff       (20)        0 2023-08-04 11:01:44.814462 sqlglot-doris-1.0.1.dev3/tests/fixtures/optimizer/
--rw-r--r--   0 liujiwen   (501) staff       (20)     1059 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/fixtures/optimizer/canonicalize.sql
--rw-r--r--   0 liujiwen   (501) staff       (20)      374 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/fixtures/optimizer/eliminate_ctes.sql
--rw-r--r--   0 liujiwen   (501) staff       (20)     3414 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/fixtures/optimizer/eliminate_joins.sql
--rw-r--r--   0 liujiwen   (501) staff       (20)     5112 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/fixtures/optimizer/eliminate_subqueries.sql
--rw-r--r--   0 liujiwen   (501) staff       (20)      978 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/fixtures/optimizer/isolate_table_selects.sql
--rw-r--r--   0 liujiwen   (501) staff       (20)    14181 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/fixtures/optimizer/merge_subqueries.sql
--rw-r--r--   0 liujiwen   (501) staff       (20)     1483 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/fixtures/optimizer/normalize.sql
--rw-r--r--   0 liujiwen   (501) staff       (20)     1121 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/fixtures/optimizer/normalize_identifiers.sql
--rw-r--r--   0 liujiwen   (501) staff       (20)     1010 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/fixtures/optimizer/optimize_joins.sql
--rw-r--r--   0 liujiwen   (501) staff       (20)    18320 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/fixtures/optimizer/optimizer.sql
--rw-r--r--   0 liujiwen   (501) staff       (20)     2939 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/fixtures/optimizer/pushdown_predicates.sql
--rw-r--r--   0 liujiwen   (501) staff       (20)     4807 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/fixtures/optimizer/pushdown_projections.sql
--rw-r--r--   0 liujiwen   (501) staff       (20)    18496 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/fixtures/optimizer/qualify_columns.sql
--rw-r--r--   0 liujiwen   (501) staff       (20)      559 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/fixtures/optimizer/qualify_columns__invalid.sql
--rw-r--r--   0 liujiwen   (501) staff       (20)     1109 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/fixtures/optimizer/qualify_columns__with_invisible.sql
--rw-r--r--   0 liujiwen   (501) staff       (20)     1966 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/fixtures/optimizer/qualify_columns_ddl.sql
--rw-r--r--   0 liujiwen   (501) staff       (20)     4887 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/fixtures/optimizer/qualify_tables.sql
--rw-r--r--   0 liujiwen   (501) staff       (20)      146 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/fixtures/optimizer/quote_identities.sql
--rw-r--r--   0 liujiwen   (501) staff       (20)     7194 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/fixtures/optimizer/simplify.sql
-drwxr-xr-x   0 liujiwen   (501) staff       (20)        0 2023-08-04 11:01:44.814628 sqlglot-doris-1.0.1.dev3/tests/fixtures/optimizer/tpc-ds/
--rw-r--r--   0 liujiwen   (501) staff       (20)   475514 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/fixtures/optimizer/tpc-ds/tpc-ds.sql
-drwxr-xr-x   0 liujiwen   (501) staff       (20)        0 2023-08-04 11:01:44.821565 sqlglot-doris-1.0.1.dev3/tests/fixtures/optimizer/tpc-h/
--rw-r--r--   0 liujiwen   (501) staff       (20)   125178 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/fixtures/optimizer/tpc-h/customer.csv.gz
--rw-r--r--   0 liujiwen   (501) staff       (20)   304069 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/fixtures/optimizer/tpc-h/lineitem.csv.gz
--rw-r--r--   0 liujiwen   (501) staff       (20)     1002 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/fixtures/optimizer/tpc-h/nation.csv.gz
--rw-r--r--   0 liujiwen   (501) staff       (20)    66113 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/fixtures/optimizer/tpc-h/orders.csv.gz
--rw-r--r--   0 liujiwen   (501) staff       (20)   251365 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/fixtures/optimizer/tpc-h/part.csv.gz
--rw-r--r--   0 liujiwen   (501) staff       (20)   303483 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/fixtures/optimizer/tpc-h/partsupp.csv.gz
--rw-r--r--   0 liujiwen   (501) staff       (20)      284 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/fixtures/optimizer/tpc-h/region.csv.gz
--rw-r--r--   0 liujiwen   (501) staff       (20)   317596 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/fixtures/optimizer/tpc-h/supplier.csv.gz
--rw-r--r--   0 liujiwen   (501) staff       (20)    41698 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/fixtures/optimizer/tpc-h/tpc-h.sql
--rw-r--r--   0 liujiwen   (501) staff       (20)     3637 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/fixtures/optimizer/unnest_subqueries.sql
--rw-r--r--   0 liujiwen   (501) staff       (20)      145 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/fixtures/partial.sql
--rw-r--r--   0 liujiwen   (501) staff       (20)     7006 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/fixtures/pretty.sql
--rw-r--r--   0 liujiwen   (501) staff       (20)    19626 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/helpers.py
--rw-r--r--   0 liujiwen   (501) staff       (20)    26548 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/test_build.py
--rw-r--r--   0 liujiwen   (501) staff       (20)     6133 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/test_diff.py
--rw-r--r--   0 liujiwen   (501) staff       (20)      563 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/test_docs.py
--rw-r--r--   0 liujiwen   (501) staff       (20)    23673 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/test_executor.py
--rw-r--r--   0 liujiwen   (501) staff       (20)    38711 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/test_expressions.py
--rw-r--r--   0 liujiwen   (501) staff       (20)     1753 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/test_generator.py
--rw-r--r--   0 liujiwen   (501) staff       (20)     2376 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/test_helper.py
--rw-r--r--   0 liujiwen   (501) staff       (20)     6944 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/test_lineage.py
--rw-r--r--   0 liujiwen   (501) staff       (20)    32230 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/test_optimizer.py
--rw-r--r--   0 liujiwen   (501) staff       (20)    26127 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/test_parser.py
--rw-r--r--   0 liujiwen   (501) staff       (20)     9427 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/test_schema.py
--rw-r--r--   0 liujiwen   (501) staff       (20)     1234 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/test_serde.py
--rw-r--r--   0 liujiwen   (501) staff       (20)      505 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/test_time.py
--rw-r--r--   0 liujiwen   (501) staff       (20)     4506 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/test_tokens.py
--rw-r--r--   0 liujiwen   (501) staff       (20)     5982 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/test_transforms.py
--rw-r--r--   0 liujiwen   (501) staff       (20)    25029 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/test_transpile.py
--rw-r--r--   0 liujiwen   (501) staff       (20)     3182 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.1.dev3/tests/tpch.py
+drwxr-xr-x   0 liujiwen   (501) staff       (20)        0 2023-08-06 11:26:19.029991 sqlglot-doris-1.0.2.dev3/
+drwxr-xr-x   0 liujiwen   (501) staff       (20)        0 2023-08-06 11:26:18.855194 sqlglot-doris-1.0.2.dev3/.github/
+drwxr-xr-x   0 liujiwen   (501) staff       (20)        0 2023-08-06 11:26:18.860466 sqlglot-doris-1.0.2.dev3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 liujiwen   (501) staff       (20)      488 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 liujiwen   (501) staff       (20)      595 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 liujiwen   (501) staff       (20)        0 2023-08-06 11:26:18.860845 sqlglot-doris-1.0.2.dev3/.github/workflows/
+-rw-r--r--   0 liujiwen   (501) staff       (20)      629 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/.github/workflows/python-package.yml
+-rw-r--r--   0 liujiwen   (501) staff       (20)     1125 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/.github/workflows/python-publish.yml
+-rw-r--r--   0 liujiwen   (501) staff       (20)     1923 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/.gitignore
+-rw-r--r--   0 liujiwen   (501) staff       (20)      815 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/.pre-commit-config.yaml
+-rw-r--r--   0 liujiwen   (501) staff       (20)   110654 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/CHANGELOG.md
+-rw-r--r--   0 liujiwen   (501) staff       (20)     2374 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/CONTRIBUTING.md
+-rw-r--r--   0 liujiwen   (501) staff       (20)     1065 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/LICENSE
+-rw-r--r--   0 liujiwen   (501) staff       (20)      401 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/Makefile
+-rw-r--r--   0 liujiwen   (501) staff       (20)     4133 2023-08-06 11:26:19.030119 sqlglot-doris-1.0.2.dev3/PKG-INFO
+-rw-r--r--   0 liujiwen   (501) staff       (20)     3476 2023-08-04 10:47:19.000000 sqlglot-doris-1.0.2.dev3/README.md
+-rw-r--r--   0 liujiwen   (501) staff       (20)    14107 2023-08-04 08:30:57.000000 sqlglot-doris-1.0.2.dev3/READMEBASE.md
+drwxr-xr-x   0 liujiwen   (501) staff       (20)        0 2023-08-06 11:26:18.861081 sqlglot-doris-1.0.2.dev3/benchmarks/
+-rw-r--r--   0 liujiwen   (501) staff       (20)     6977 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/benchmarks/bench.py
+drwxr-xr-x   0 liujiwen   (501) staff       (20)        0 2023-08-06 11:26:18.869335 sqlglot-doris-1.0.2.dev3/docs/
+-rw-r--r--   0 liujiwen   (501) staff       (20)       11 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/docs/CNAME
+-rw-r--r--   0 liujiwen   (501) staff       (20)      138 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/docs/index.html
+-rw-r--r--   0 liujiwen   (501) staff       (20) 10482048 2023-08-04 09:00:00.000000 sqlglot-doris-1.0.2.dev3/docs/search.js
+drwxr-xr-x   0 liujiwen   (501) staff       (20)        0 2023-08-06 11:26:18.910398 sqlglot-doris-1.0.2.dev3/docs/sqlglot/
+-rw-r--r--   0 liujiwen   (501) staff       (20)    36724 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/docs/sqlglot/_typing.html
+-rw-r--r--   0 liujiwen   (501) staff       (20)    36080 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/docs/sqlglot/_version.html
+drwxr-xr-x   0 liujiwen   (501) staff       (20)        0 2023-08-06 11:26:18.911330 sqlglot-doris-1.0.2.dev3/docs/sqlglot/dataframe/
+-rw-r--r--   0 liujiwen   (501) staff       (20)   985439 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/docs/sqlglot/dataframe/sql.html
+-rw-r--r--   0 liujiwen   (501) staff       (20)    66466 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/docs/sqlglot/dataframe.html
+drwxr-xr-x   0 liujiwen   (501) staff       (20)        0 2023-08-06 11:26:18.945072 sqlglot-doris-1.0.2.dev3/docs/sqlglot/dialects/
+-rw-r--r--   0 liujiwen   (501) staff       (20)   682043 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/docs/sqlglot/dialects/bigquery.html
+-rw-r--r--   0 liujiwen   (501) staff       (20)   604442 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/docs/sqlglot/dialects/clickhouse.html
+-rw-r--r--   0 liujiwen   (501) staff       (20)   234037 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/docs/sqlglot/dialects/databricks.html
+-rw-r--r--   0 liujiwen   (501) staff       (20)   504902 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/docs/sqlglot/dialects/dialect.html
+-rw-r--r--   0 liujiwen   (501) staff       (20)   323631 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/docs/sqlglot/dialects/drill.html
+-rw-r--r--   0 liujiwen   (501) staff       (20)   456420 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/docs/sqlglot/dialects/duckdb.html
+-rw-r--r--   0 liujiwen   (501) staff       (20)   576965 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/docs/sqlglot/dialects/hive.html
+-rw-r--r--   0 liujiwen   (501) staff       (20)   773372 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/docs/sqlglot/dialects/mysql.html
+-rw-r--r--   0 liujiwen   (501) staff       (20)   369087 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/docs/sqlglot/dialects/oracle.html
+-rw-r--r--   0 liujiwen   (501) staff       (20)   480863 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/docs/sqlglot/dialects/postgres.html
+-rw-r--r--   0 liujiwen   (501) staff       (20)   519013 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/docs/sqlglot/dialects/presto.html
+-rw-r--r--   0 liujiwen   (501) staff       (20)   363269 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/docs/sqlglot/dialects/redshift.html
+-rw-r--r--   0 liujiwen   (501) staff       (20)   535303 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/docs/sqlglot/dialects/snowflake.html
+-rw-r--r--   0 liujiwen   (501) staff       (20)   227931 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/docs/sqlglot/dialects/spark.html
+-rw-r--r--   0 liujiwen   (501) staff       (20)   395132 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/docs/sqlglot/dialects/spark2.html
+-rw-r--r--   0 liujiwen   (501) staff       (20)   353049 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/docs/sqlglot/dialects/sqlite.html
+-rw-r--r--   0 liujiwen   (501) staff       (20)   221352 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/docs/sqlglot/dialects/starrocks.html
+-rw-r--r--   0 liujiwen   (501) staff       (20)   219461 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/docs/sqlglot/dialects/tableau.html
+-rw-r--r--   0 liujiwen   (501) staff       (20)   382689 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/docs/sqlglot/dialects/teradata.html
+-rw-r--r--   0 liujiwen   (501) staff       (20)   147383 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/docs/sqlglot/dialects/trino.html
+-rw-r--r--   0 liujiwen   (501) staff       (20)   715570 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/docs/sqlglot/dialects/tsql.html
+-rw-r--r--   0 liujiwen   (501) staff       (20)    55816 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/docs/sqlglot/dialects.html
+-rw-r--r--   0 liujiwen   (501) staff       (20)   283781 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/docs/sqlglot/diff.html
+-rw-r--r--   0 liujiwen   (501) staff       (20)   100430 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/docs/sqlglot/errors.html
+drwxr-xr-x   0 liujiwen   (501) staff       (20)        0 2023-08-06 11:26:18.949052 sqlglot-doris-1.0.2.dev3/docs/sqlglot/executor/
+-rw-r--r--   0 liujiwen   (501) staff       (20)   117988 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/docs/sqlglot/executor/context.html
+-rw-r--r--   0 liujiwen   (501) staff       (20)   131973 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/docs/sqlglot/executor/env.html
+-rw-r--r--   0 liujiwen   (501) staff       (20)   506241 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/docs/sqlglot/executor/python.html
+-rw-r--r--   0 liujiwen   (501) staff       (20)   118949 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/docs/sqlglot/executor/table.html
+-rw-r--r--   0 liujiwen   (501) staff       (20)    92941 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/docs/sqlglot/executor.html
+-rw-r--r--   0 liujiwen   (501) staff       (20)  6751372 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/docs/sqlglot/expressions.html
+-rw-r--r--   0 liujiwen   (501) staff       (20)  2963956 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/docs/sqlglot/generator.html
+-rw-r--r--   0 liujiwen   (501) staff       (20)   226523 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/docs/sqlglot/helper.html
+-rw-r--r--   0 liujiwen   (501) staff       (20)   190366 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/docs/sqlglot/lineage.html
+drwxr-xr-x   0 liujiwen   (501) staff       (20)        0 2023-08-06 11:26:18.964445 sqlglot-doris-1.0.2.dev3/docs/sqlglot/optimizer/
+-rw-r--r--   0 liujiwen   (501) staff       (20)   294349 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/docs/sqlglot/optimizer/annotate_types.html
+-rw-r--r--   0 liujiwen   (501) staff       (20)    76888 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/docs/sqlglot/optimizer/canonicalize.html
+-rw-r--r--   0 liujiwen   (501) staff       (20)    53615 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/docs/sqlglot/optimizer/eliminate_ctes.html
+-rw-r--r--   0 liujiwen   (501) staff       (20)    99196 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/docs/sqlglot/optimizer/eliminate_joins.html
+-rw-r--r--   0 liujiwen   (501) staff       (20)   100353 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/docs/sqlglot/optimizer/eliminate_subqueries.html
+-rw-r--r--   0 liujiwen   (501) staff       (20)    51199 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/docs/sqlglot/optimizer/expand_laterals.html
+-rw-r--r--   0 liujiwen   (501) staff       (20)    45966 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/docs/sqlglot/optimizer/expand_multi_table_selects.html
+-rw-r--r--   0 liujiwen   (501) staff       (20)    51584 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/docs/sqlglot/optimizer/isolate_table_selects.html
+-rw-r--r--   0 liujiwen   (501) staff       (20)    63180 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/docs/sqlglot/optimizer/lower_identities.html
+-rw-r--r--   0 liujiwen   (501) staff       (20)   150542 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/docs/sqlglot/optimizer/merge_subqueries.html
+-rw-r--r--   0 liujiwen   (501) staff       (20)   107750 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/docs/sqlglot/optimizer/normalize.html
+-rw-r--r--   0 liujiwen   (501) staff       (20)    48102 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/docs/sqlglot/optimizer/normalize_identifiers.html
+-rw-r--r--   0 liujiwen   (501) staff       (20)    76872 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/docs/sqlglot/optimizer/optimize_joins.html
+-rw-r--r--   0 liujiwen   (501) staff       (20)    73565 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/docs/sqlglot/optimizer/optimizer.html
+-rw-r--r--   0 liujiwen   (501) staff       (20)   134865 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/docs/sqlglot/optimizer/pushdown_predicates.html
+-rw-r--r--   0 liujiwen   (501) staff       (20)    83923 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/docs/sqlglot/optimizer/pushdown_projections.html
+-rw-r--r--   0 liujiwen   (501) staff       (20)    70870 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/docs/sqlglot/optimizer/qualify.html
+-rw-r--r--   0 liujiwen   (501) staff       (20)   263034 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/docs/sqlglot/optimizer/qualify_columns.html
+-rw-r--r--   0 liujiwen   (501) staff       (20)    91897 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/docs/sqlglot/optimizer/qualify_tables.html
+-rw-r--r--   0 liujiwen   (501) staff       (20)   392396 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/docs/sqlglot/optimizer/scope.html
+-rw-r--r--   0 liujiwen   (501) staff       (20)   288965 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/docs/sqlglot/optimizer/simplify.html
+-rw-r--r--   0 liujiwen   (501) staff       (20)   161494 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/docs/sqlglot/optimizer/unnest_subqueries.html
+-rw-r--r--   0 liujiwen   (501) staff       (20)    37556 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/docs/sqlglot/optimizer.html
+-rw-r--r--   0 liujiwen   (501) staff       (20)  2838889 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/docs/sqlglot/parser.html
+-rw-r--r--   0 liujiwen   (501) staff       (20)   376114 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/docs/sqlglot/planner.html
+-rw-r--r--   0 liujiwen   (501) staff       (20)   359917 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/docs/sqlglot/schema.html
+-rw-r--r--   0 liujiwen   (501) staff       (20)    71553 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/docs/sqlglot/serde.html
+-rw-r--r--   0 liujiwen   (501) staff       (20)    58338 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/docs/sqlglot/time.html
+-rw-r--r--   0 liujiwen   (501) staff       (20)   832183 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/docs/sqlglot/tokens.html
+-rw-r--r--   0 liujiwen   (501) staff       (20)   200755 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/docs/sqlglot/transforms.html
+-rw-r--r--   0 liujiwen   (501) staff       (20)    71915 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/docs/sqlglot/trie.html
+-rw-r--r--   0 liujiwen   (501) staff       (20)   145333 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/docs/sqlglot.html
+drwxr-xr-x   0 liujiwen   (501) staff       (20)        0 2023-08-06 11:26:18.965205 sqlglot-doris-1.0.2.dev3/pdoc/
+-rwxr-xr-x   0 liujiwen   (501) staff       (20)     1114 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/pdoc/cli.py
+drwxr-xr-x   0 liujiwen   (501) staff       (20)        0 2023-08-06 11:26:18.965434 sqlglot-doris-1.0.2.dev3/pdoc/templates/
+-rw-r--r--   0 liujiwen   (501) staff       (20)      131 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/pdoc/templates/module.html.jinja2
+drwxr-xr-x   0 liujiwen   (501) staff       (20)        0 2023-08-06 11:26:18.965777 sqlglot-doris-1.0.2.dev3/posts/
+-rw-r--r--   0 liujiwen   (501) staff       (20)    12086 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/posts/python_sql_engine.md
+drwxr-xr-x   0 liujiwen   (501) staff       (20)        0 2023-08-06 11:26:18.969010 sqlglot-doris-1.0.2.dev3/posts/python_sql_engine_images/
+-rw-r--r--   0 liujiwen   (501) staff       (20)    32441 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/posts/python_sql_engine_images/executor.png
+-rw-r--r--   0 liujiwen   (501) staff       (20)    82195 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/posts/python_sql_engine_images/optimizer.png
+-rw-r--r--   0 liujiwen   (501) staff       (20)   157268 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/posts/python_sql_engine_images/parser.png
+-rw-r--r--   0 liujiwen   (501) staff       (20)   123866 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/posts/python_sql_engine_images/planner.png
+-rw-r--r--   0 liujiwen   (501) staff       (20)   341375 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/posts/python_sql_engine_images/tokenizer.png
+-rw-r--r--   0 liujiwen   (501) staff       (20)    26210 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/posts/sql_diff.md
+drwxr-xr-x   0 liujiwen   (501) staff       (20)        0 2023-08-06 11:26:18.979014 sqlglot-doris-1.0.2.dev3/posts/sql_diff_images/
+-rw-r--r--   0 liujiwen   (501) staff       (20)    22582 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/posts/sql_diff_images/dice_coef.png
+-rw-r--r--   0 liujiwen   (501) staff       (20)    57550 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/posts/sql_diff_images/figure_1.png
+-rw-r--r--   0 liujiwen   (501) staff       (20)  1511115 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/posts/sql_diff_images/figure_2.gif
+-rw-r--r--   0 liujiwen   (501) staff       (20)   327145 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/posts/sql_diff_images/figure_3.gif
+-rw-r--r--   0 liujiwen   (501) staff       (20)    41567 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/posts/sql_diff_images/git_diff_output.png
+-rw-r--r--   0 liujiwen   (501) staff       (20)    35159 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/posts/sql_diff_images/matching_criteria_1.png
+-rw-r--r--   0 liujiwen   (501) staff       (20)    48555 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/posts/sql_diff_images/matching_criteria_2.png
+-rw-r--r--   0 liujiwen   (501) staff       (20)      529 2023-08-06 11:26:19.030554 sqlglot-doris-1.0.2.dev3/setup.cfg
+-rw-r--r--   0 liujiwen   (501) staff       (20)     1368 2023-08-06 11:25:53.000000 sqlglot-doris-1.0.2.dev3/setup.py
+drwxr-xr-x   0 liujiwen   (501) staff       (20)        0 2023-08-06 11:26:18.985332 sqlglot-doris-1.0.2.dev3/sqlglot/
+-rw-r--r--   0 liujiwen   (501) staff       (20)     4882 2023-08-04 08:59:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/__init__.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)     1936 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/__main__.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)      142 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/_typing.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)      175 2023-08-04 10:57:10.000000 sqlglot-doris-1.0.2.dev3/sqlglot/_version.py
+drwxr-xr-x   0 liujiwen   (501) staff       (20)        0 2023-08-06 11:26:18.985629 sqlglot-doris-1.0.2.dev3/sqlglot/dataframe/
+-rw-r--r--   0 liujiwen   (501) staff       (20)     7885 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/dataframe/README.md
+-rw-r--r--   0 liujiwen   (501) staff       (20)       37 2023-08-04 08:59:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/dataframe/__init__.py
+drwxr-xr-x   0 liujiwen   (501) staff       (20)        0 2023-08-06 11:26:18.988150 sqlglot-doris-1.0.2.dev3/sqlglot/dataframe/sql/
+-rw-r--r--   0 liujiwen   (501) staff       (20)      560 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/dataframe/sql/__init__.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)      643 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/dataframe/sql/_typing.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)    12583 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/dataframe/sql/column.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)    37147 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/dataframe/sql/dataframe.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)    42238 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/dataframe/sql/functions.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)     2162 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/dataframe/sql/group.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)     3326 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/dataframe/sql/normalize.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)     1765 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/dataframe/sql/operations.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)     3085 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/dataframe/sql/readwriter.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)     5338 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/dataframe/sql/session.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)      301 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/dataframe/sql/transforms.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)     5189 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/dataframe/sql/types.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)     1142 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/dataframe/sql/util.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)     4675 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/dataframe/sql/window.py
+drwxr-xr-x   0 liujiwen   (501) staff       (20)        0 2023-08-06 11:26:18.992602 sqlglot-doris-1.0.2.dev3/sqlglot/dialects/
+-rw-r--r--   0 liujiwen   (501) staff       (20)     3041 2023-08-04 02:52:53.000000 sqlglot-doris-1.0.2.dev3/sqlglot/dialects/__init__.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)    22780 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/dialects/bigquery.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)    15734 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/dialects/clickhouse.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)     1501 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/dialects/databricks.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)    24291 2023-08-04 02:48:47.000000 sqlglot-doris-1.0.2.dev3/sqlglot/dialects/dialect.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)     4037 2023-08-05 10:18:19.000000 sqlglot-doris-1.0.2.dev3/sqlglot/dialects/doris.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)     5805 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/dialects/drill.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)    12542 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/dialects/duckdb.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)    19667 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/dialects/hive.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)    25564 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/dialects/mysql.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)     7330 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/dialects/oracle.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)    15380 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/dialects/postgres.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)    16583 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/dialects/presto.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)     6127 2023-08-04 06:20:47.000000 sqlglot-doris-1.0.2.dev3/sqlglot/dialects/redshift.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)    16583 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/dialects/snowflake.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)     2073 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/dialects/spark.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)    10739 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/dialects/spark2.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)     7543 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/dialects/sqlite.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)     1678 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/dialects/starrocks.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)     1402 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/dialects/tableau.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)     8478 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/dialects/teradata.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)      429 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/dialects/trino.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)    24905 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/dialects/tsql.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)    14048 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/diff.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)     2126 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/errors.py
+drwxr-xr-x   0 liujiwen   (501) staff       (20)        0 2023-08-06 11:26:18.993392 sqlglot-doris-1.0.2.dev3/sqlglot/executor/
+-rw-r--r--   0 liujiwen   (501) staff       (20)     2620 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/executor/__init__.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)     3357 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/executor/context.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)     6679 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/executor/env.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)    15435 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/executor/python.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)     3423 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/executor/table.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)   162320 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/expressions.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)   111731 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/generator.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)    11200 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/helper.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)     8863 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/lineage.py
+drwxr-xr-x   0 liujiwen   (501) staff       (20)        0 2023-08-06 11:26:18.996585 sqlglot-doris-1.0.2.dev3/sqlglot/optimizer/
+-rw-r--r--   0 liujiwen   (501) staff       (20)      127 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/optimizer/__init__.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)    14230 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/optimizer/annotate_types.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)     2755 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/optimizer/canonicalize.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)     1434 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/optimizer/eliminate_ctes.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)     5874 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/optimizer/eliminate_joins.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)     6473 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/optimizer/eliminate_subqueries.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)     1128 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/optimizer/isolate_table_selects.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)    14646 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/optimizer/merge_subqueries.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)     5547 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/optimizer/normalize.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)     1018 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/optimizer/normalize_identifiers.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)     2604 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/optimizer/optimize_joins.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)     3537 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/optimizer/optimizer.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)     7266 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/optimizer/pushdown_predicates.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)     4690 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/optimizer/pushdown_projections.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)     3098 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/optimizer/qualify.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)    22230 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/optimizer/qualify_columns.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)     4160 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/optimizer/qualify_tables.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)    26360 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/optimizer/scope.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)    18184 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/optimizer/simplify.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)     9494 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/optimizer/unnest_subqueries.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)   179631 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/parser.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)    14144 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/planner.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)        0 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/py.typed
+-rw-r--r--   0 liujiwen   (501) staff       (20)    18067 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/schema.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)     2031 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/serde.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)     1418 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/time.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)    35304 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/tokens.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)    11699 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/transforms.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)     2245 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot/trie.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)     4208 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/sqlglot.svg
+drwxr-xr-x   0 liujiwen   (501) staff       (20)        0 2023-08-06 11:26:18.997148 sqlglot-doris-1.0.2.dev3/sqlglot_doris.egg-info/
+-rw-r--r--   0 liujiwen   (501) staff       (20)     4133 2023-08-06 11:26:18.000000 sqlglot-doris-1.0.2.dev3/sqlglot_doris.egg-info/PKG-INFO
+-rw-r--r--   0 liujiwen   (501) staff       (20)     9016 2023-08-06 11:26:18.000000 sqlglot-doris-1.0.2.dev3/sqlglot_doris.egg-info/SOURCES.txt
+-rw-r--r--   0 liujiwen   (501) staff       (20)        1 2023-08-06 11:26:18.000000 sqlglot-doris-1.0.2.dev3/sqlglot_doris.egg-info/dependency_links.txt
+-rw-r--r--   0 liujiwen   (501) staff       (20)      100 2023-08-06 11:26:18.000000 sqlglot-doris-1.0.2.dev3/sqlglot_doris.egg-info/requires.txt
+-rw-r--r--   0 liujiwen   (501) staff       (20)        8 2023-08-06 11:26:18.000000 sqlglot-doris-1.0.2.dev3/sqlglot_doris.egg-info/top_level.txt
+-rw-r--r--   0 liujiwen   (501) staff       (20)      484 2023-08-05 15:53:20.000000 sqlglot-doris-1.0.2.dev3/test_doris.py
+drwxr-xr-x   0 liujiwen   (501) staff       (20)        0 2023-08-06 11:26:19.001136 sqlglot-doris-1.0.2.dev3/tests/
+-rw-r--r--   0 liujiwen   (501) staff       (20)        0 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/__init__.py
+drwxr-xr-x   0 liujiwen   (501) staff       (20)        0 2023-08-06 11:26:19.001281 sqlglot-doris-1.0.2.dev3/tests/dataframe/
+-rw-r--r--   0 liujiwen   (501) staff       (20)        0 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/dataframe/__init__.py
+drwxr-xr-x   0 liujiwen   (501) staff       (20)        0 2023-08-06 11:26:19.002365 sqlglot-doris-1.0.2.dev3/tests/dataframe/integration/
+-rw-r--r--   0 liujiwen   (501) staff       (20)        0 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/dataframe/integration/__init__.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)     7670 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/dataframe/integration/dataframe_validator.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)    52342 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/dataframe/integration/test_dataframe.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)     3173 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/dataframe/integration/test_grouped_data.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)     1088 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/dataframe/integration/test_session.py
+drwxr-xr-x   0 liujiwen   (501) staff       (20)        0 2023-08-06 11:26:19.004143 sqlglot-doris-1.0.2.dev3/tests/dataframe/unit/
+-rw-r--r--   0 liujiwen   (501) staff       (20)        0 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/dataframe/unit/__init__.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)     1582 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/dataframe/unit/dataframe_sql_validator.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)     6376 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/dataframe/unit/test_column.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)     2577 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/dataframe/unit/test_dataframe.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)     9354 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/dataframe/unit/test_dataframe_writer.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)    70790 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/dataframe/unit/test_functions.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)     5865 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/dataframe/unit/test_session.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)     2388 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/dataframe/unit/test_types.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)     3320 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/dataframe/unit/test_window.py
+drwxr-xr-x   0 liujiwen   (501) staff       (20)        0 2023-08-06 11:26:19.008721 sqlglot-doris-1.0.2.dev3/tests/dialects/
+-rw-r--r--   0 liujiwen   (501) staff       (20)        0 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/dialects/__init__.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)    29997 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/dialects/test_bigquery.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)    18974 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/dialects/test_clickhouse.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)     8193 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/dialects/test_databricks.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)    69752 2023-08-04 03:30:02.000000 sqlglot-doris-1.0.2.dev3/tests/dialects/test_dialect.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)      563 2023-08-04 02:58:47.000000 sqlglot-doris-1.0.2.dev3/tests/dialects/test_doris.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)     2326 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/dialects/test_drill.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)    24085 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/dialects/test_duckdb.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)    26497 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/dialects/test_hive.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)    35751 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/dialects/test_mysql.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)     6695 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/dialects/test_oracle.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)    26820 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/dialects/test_postgres.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)    35008 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/dialects/test_presto.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)    14724 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/dialects/test_redshift.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)    43592 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/dialects/test_snowflake.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)    23040 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/dialects/test_spark.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)     6221 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/dialects/test_sqlite.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)      571 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/dialects/test_starrocks.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)     1715 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/dialects/test_tableau.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)     7216 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/dialects/test_teradata.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)    42172 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/dialects/test_tsql.py
+drwxr-xr-x   0 liujiwen   (501) staff       (20)        0 2023-08-06 11:26:19.009354 sqlglot-doris-1.0.2.dev3/tests/fixtures/
+-rw-r--r--   0 liujiwen   (501) staff       (20)    34464 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/fixtures/identity.sql
+drwxr-xr-x   0 liujiwen   (501) staff       (20)        0 2023-08-06 11:26:19.014955 sqlglot-doris-1.0.2.dev3/tests/fixtures/optimizer/
+-rw-r--r--   0 liujiwen   (501) staff       (20)     1059 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/fixtures/optimizer/canonicalize.sql
+-rw-r--r--   0 liujiwen   (501) staff       (20)      374 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/fixtures/optimizer/eliminate_ctes.sql
+-rw-r--r--   0 liujiwen   (501) staff       (20)     3414 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/fixtures/optimizer/eliminate_joins.sql
+-rw-r--r--   0 liujiwen   (501) staff       (20)     5112 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/fixtures/optimizer/eliminate_subqueries.sql
+-rw-r--r--   0 liujiwen   (501) staff       (20)      978 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/fixtures/optimizer/isolate_table_selects.sql
+-rw-r--r--   0 liujiwen   (501) staff       (20)    14181 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/fixtures/optimizer/merge_subqueries.sql
+-rw-r--r--   0 liujiwen   (501) staff       (20)     1483 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/fixtures/optimizer/normalize.sql
+-rw-r--r--   0 liujiwen   (501) staff       (20)     1121 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/fixtures/optimizer/normalize_identifiers.sql
+-rw-r--r--   0 liujiwen   (501) staff       (20)     1010 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/fixtures/optimizer/optimize_joins.sql
+-rw-r--r--   0 liujiwen   (501) staff       (20)    18320 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/fixtures/optimizer/optimizer.sql
+-rw-r--r--   0 liujiwen   (501) staff       (20)     2939 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/fixtures/optimizer/pushdown_predicates.sql
+-rw-r--r--   0 liujiwen   (501) staff       (20)     4807 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/fixtures/optimizer/pushdown_projections.sql
+-rw-r--r--   0 liujiwen   (501) staff       (20)    18496 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/fixtures/optimizer/qualify_columns.sql
+-rw-r--r--   0 liujiwen   (501) staff       (20)      559 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/fixtures/optimizer/qualify_columns__invalid.sql
+-rw-r--r--   0 liujiwen   (501) staff       (20)     1109 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/fixtures/optimizer/qualify_columns__with_invisible.sql
+-rw-r--r--   0 liujiwen   (501) staff       (20)     1966 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/fixtures/optimizer/qualify_columns_ddl.sql
+-rw-r--r--   0 liujiwen   (501) staff       (20)     4887 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/fixtures/optimizer/qualify_tables.sql
+-rw-r--r--   0 liujiwen   (501) staff       (20)      146 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/fixtures/optimizer/quote_identities.sql
+-rw-r--r--   0 liujiwen   (501) staff       (20)     7194 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/fixtures/optimizer/simplify.sql
+drwxr-xr-x   0 liujiwen   (501) staff       (20)        0 2023-08-06 11:26:19.015115 sqlglot-doris-1.0.2.dev3/tests/fixtures/optimizer/tpc-ds/
+-rw-r--r--   0 liujiwen   (501) staff       (20)   475514 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/fixtures/optimizer/tpc-ds/tpc-ds.sql
+drwxr-xr-x   0 liujiwen   (501) staff       (20)        0 2023-08-06 11:26:19.029732 sqlglot-doris-1.0.2.dev3/tests/fixtures/optimizer/tpc-h/
+-rw-r--r--   0 liujiwen   (501) staff       (20)   125178 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/fixtures/optimizer/tpc-h/customer.csv.gz
+-rw-r--r--   0 liujiwen   (501) staff       (20)   304069 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/fixtures/optimizer/tpc-h/lineitem.csv.gz
+-rw-r--r--   0 liujiwen   (501) staff       (20)     1002 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/fixtures/optimizer/tpc-h/nation.csv.gz
+-rw-r--r--   0 liujiwen   (501) staff       (20)    66113 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/fixtures/optimizer/tpc-h/orders.csv.gz
+-rw-r--r--   0 liujiwen   (501) staff       (20)   251365 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/fixtures/optimizer/tpc-h/part.csv.gz
+-rw-r--r--   0 liujiwen   (501) staff       (20)   303483 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/fixtures/optimizer/tpc-h/partsupp.csv.gz
+-rw-r--r--   0 liujiwen   (501) staff       (20)      284 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/fixtures/optimizer/tpc-h/region.csv.gz
+-rw-r--r--   0 liujiwen   (501) staff       (20)   317596 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/fixtures/optimizer/tpc-h/supplier.csv.gz
+-rw-r--r--   0 liujiwen   (501) staff       (20)    41698 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/fixtures/optimizer/tpc-h/tpc-h.sql
+-rw-r--r--   0 liujiwen   (501) staff       (20)     3637 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/fixtures/optimizer/unnest_subqueries.sql
+-rw-r--r--   0 liujiwen   (501) staff       (20)      145 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/fixtures/partial.sql
+-rw-r--r--   0 liujiwen   (501) staff       (20)     7006 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/fixtures/pretty.sql
+-rw-r--r--   0 liujiwen   (501) staff       (20)    19626 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/helpers.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)    26548 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/test_build.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)     6133 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/test_diff.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)      563 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/test_docs.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)    23673 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/test_executor.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)    38711 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/test_expressions.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)     1753 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/test_generator.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)     2376 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/test_helper.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)     6944 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/test_lineage.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)    32230 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/test_optimizer.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)    26127 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/test_parser.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)     9427 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/test_schema.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)     1234 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/test_serde.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)      505 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/test_time.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)     4506 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/test_tokens.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)     5982 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/test_transforms.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)    25029 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/test_transpile.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)     3182 2023-08-03 05:03:58.000000 sqlglot-doris-1.0.2.dev3/tests/tpch.py
```

### Comparing `sqlglot-doris-1.0.1.dev3/.github/ISSUE_TEMPLATE/feature_request.md` & `sqlglot-doris-1.0.2.dev3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/.github/workflows/python-package.yml` & `sqlglot-doris-1.0.2.dev3/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/.github/workflows/python-publish.yml` & `sqlglot-doris-1.0.2.dev3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/.gitignore` & `sqlglot-doris-1.0.2.dev3/.gitignore`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/.pre-commit-config.yaml` & `sqlglot-doris-1.0.2.dev3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/CHANGELOG.md` & `sqlglot-doris-1.0.2.dev3/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/CONTRIBUTING.md` & `sqlglot-doris-1.0.2.dev3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/LICENSE` & `sqlglot-doris-1.0.2.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/PKG-INFO` & `sqlglot-doris-1.0.2.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlglot-doris
-Version: 1.0.1.dev3
+Version: 1.0.2.dev3
 Summary: An easily customizable SQL parser and transpiler
 Home-page: https://github.com/tobymao/sqlglot
 Author: Toby Mao
 Author-email: toby.mao@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `sqlglot-doris-1.0.1.dev3/README.md` & `sqlglot-doris-1.0.2.dev3/README.md`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/benchmarks/bench.py` & `sqlglot-doris-1.0.2.dev3/benchmarks/bench.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/docs/search.js` & `sqlglot-doris-1.0.2.dev3/docs/search.js`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/docs/sqlglot/_typing.html` & `sqlglot-doris-1.0.2.dev3/docs/sqlglot/_typing.html`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/docs/sqlglot/_version.html` & `sqlglot-doris-1.0.2.dev3/docs/sqlglot/_version.html`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/docs/sqlglot/dataframe/sql.html` & `sqlglot-doris-1.0.2.dev3/docs/sqlglot/dataframe/sql.html`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/docs/sqlglot/dataframe.html` & `sqlglot-doris-1.0.2.dev3/docs/sqlglot/dataframe.html`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/docs/sqlglot/dialects/bigquery.html` & `sqlglot-doris-1.0.2.dev3/docs/sqlglot/dialects/bigquery.html`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/docs/sqlglot/dialects/clickhouse.html` & `sqlglot-doris-1.0.2.dev3/docs/sqlglot/dialects/clickhouse.html`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/docs/sqlglot/dialects/databricks.html` & `sqlglot-doris-1.0.2.dev3/docs/sqlglot/dialects/databricks.html`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/docs/sqlglot/dialects/dialect.html` & `sqlglot-doris-1.0.2.dev3/docs/sqlglot/dialects/dialect.html`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/docs/sqlglot/dialects/drill.html` & `sqlglot-doris-1.0.2.dev3/docs/sqlglot/dialects/drill.html`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/docs/sqlglot/dialects/duckdb.html` & `sqlglot-doris-1.0.2.dev3/docs/sqlglot/dialects/duckdb.html`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/docs/sqlglot/dialects/hive.html` & `sqlglot-doris-1.0.2.dev3/docs/sqlglot/dialects/hive.html`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/docs/sqlglot/dialects/mysql.html` & `sqlglot-doris-1.0.2.dev3/docs/sqlglot/dialects/mysql.html`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/docs/sqlglot/dialects/oracle.html` & `sqlglot-doris-1.0.2.dev3/docs/sqlglot/dialects/oracle.html`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/docs/sqlglot/dialects/postgres.html` & `sqlglot-doris-1.0.2.dev3/docs/sqlglot/dialects/postgres.html`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/docs/sqlglot/dialects/presto.html` & `sqlglot-doris-1.0.2.dev3/docs/sqlglot/dialects/presto.html`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/docs/sqlglot/dialects/redshift.html` & `sqlglot-doris-1.0.2.dev3/docs/sqlglot/dialects/redshift.html`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/docs/sqlglot/dialects/snowflake.html` & `sqlglot-doris-1.0.2.dev3/docs/sqlglot/dialects/snowflake.html`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/docs/sqlglot/dialects/spark.html` & `sqlglot-doris-1.0.2.dev3/docs/sqlglot/dialects/spark.html`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/docs/sqlglot/dialects/spark2.html` & `sqlglot-doris-1.0.2.dev3/docs/sqlglot/dialects/spark2.html`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/docs/sqlglot/dialects/sqlite.html` & `sqlglot-doris-1.0.2.dev3/docs/sqlglot/dialects/sqlite.html`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/docs/sqlglot/dialects/starrocks.html` & `sqlglot-doris-1.0.2.dev3/docs/sqlglot/dialects/starrocks.html`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/docs/sqlglot/dialects/tableau.html` & `sqlglot-doris-1.0.2.dev3/docs/sqlglot/dialects/tableau.html`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/docs/sqlglot/dialects/teradata.html` & `sqlglot-doris-1.0.2.dev3/docs/sqlglot/dialects/teradata.html`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/docs/sqlglot/dialects/trino.html` & `sqlglot-doris-1.0.2.dev3/docs/sqlglot/dialects/trino.html`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/docs/sqlglot/dialects/tsql.html` & `sqlglot-doris-1.0.2.dev3/docs/sqlglot/dialects/tsql.html`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/docs/sqlglot/dialects.html` & `sqlglot-doris-1.0.2.dev3/docs/sqlglot/dialects.html`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/docs/sqlglot/diff.html` & `sqlglot-doris-1.0.2.dev3/docs/sqlglot/diff.html`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/docs/sqlglot/errors.html` & `sqlglot-doris-1.0.2.dev3/docs/sqlglot/errors.html`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/docs/sqlglot/executor/context.html` & `sqlglot-doris-1.0.2.dev3/docs/sqlglot/executor/context.html`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/docs/sqlglot/executor/env.html` & `sqlglot-doris-1.0.2.dev3/docs/sqlglot/executor/env.html`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/docs/sqlglot/executor/python.html` & `sqlglot-doris-1.0.2.dev3/docs/sqlglot/executor/python.html`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/docs/sqlglot/executor/table.html` & `sqlglot-doris-1.0.2.dev3/docs/sqlglot/executor/table.html`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/docs/sqlglot/executor.html` & `sqlglot-doris-1.0.2.dev3/docs/sqlglot/executor.html`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/docs/sqlglot/expressions.html` & `sqlglot-doris-1.0.2.dev3/docs/sqlglot/expressions.html`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/docs/sqlglot/generator.html` & `sqlglot-doris-1.0.2.dev3/docs/sqlglot/generator.html`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/docs/sqlglot/helper.html` & `sqlglot-doris-1.0.2.dev3/docs/sqlglot/helper.html`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/docs/sqlglot/lineage.html` & `sqlglot-doris-1.0.2.dev3/docs/sqlglot/lineage.html`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/docs/sqlglot/optimizer/annotate_types.html` & `sqlglot-doris-1.0.2.dev3/docs/sqlglot/optimizer/annotate_types.html`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/docs/sqlglot/optimizer/canonicalize.html` & `sqlglot-doris-1.0.2.dev3/docs/sqlglot/optimizer/canonicalize.html`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/docs/sqlglot/optimizer/eliminate_ctes.html` & `sqlglot-doris-1.0.2.dev3/docs/sqlglot/optimizer/eliminate_ctes.html`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/docs/sqlglot/optimizer/eliminate_joins.html` & `sqlglot-doris-1.0.2.dev3/docs/sqlglot/optimizer/eliminate_joins.html`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/docs/sqlglot/optimizer/eliminate_subqueries.html` & `sqlglot-doris-1.0.2.dev3/docs/sqlglot/optimizer/eliminate_subqueries.html`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/docs/sqlglot/optimizer/expand_laterals.html` & `sqlglot-doris-1.0.2.dev3/docs/sqlglot/optimizer/expand_laterals.html`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/docs/sqlglot/optimizer/expand_multi_table_selects.html` & `sqlglot-doris-1.0.2.dev3/docs/sqlglot/optimizer/expand_multi_table_selects.html`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/docs/sqlglot/optimizer/isolate_table_selects.html` & `sqlglot-doris-1.0.2.dev3/docs/sqlglot/optimizer/isolate_table_selects.html`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/docs/sqlglot/optimizer/lower_identities.html` & `sqlglot-doris-1.0.2.dev3/docs/sqlglot/optimizer/lower_identities.html`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/docs/sqlglot/optimizer/merge_subqueries.html` & `sqlglot-doris-1.0.2.dev3/docs/sqlglot/optimizer/merge_subqueries.html`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/docs/sqlglot/optimizer/normalize.html` & `sqlglot-doris-1.0.2.dev3/docs/sqlglot/optimizer/normalize.html`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/docs/sqlglot/optimizer/normalize_identifiers.html` & `sqlglot-doris-1.0.2.dev3/docs/sqlglot/optimizer/normalize_identifiers.html`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/docs/sqlglot/optimizer/optimize_joins.html` & `sqlglot-doris-1.0.2.dev3/docs/sqlglot/optimizer/optimize_joins.html`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/docs/sqlglot/optimizer/optimizer.html` & `sqlglot-doris-1.0.2.dev3/docs/sqlglot/optimizer/optimizer.html`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/docs/sqlglot/optimizer/pushdown_predicates.html` & `sqlglot-doris-1.0.2.dev3/docs/sqlglot/optimizer/pushdown_predicates.html`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/docs/sqlglot/optimizer/pushdown_projections.html` & `sqlglot-doris-1.0.2.dev3/docs/sqlglot/optimizer/pushdown_projections.html`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/docs/sqlglot/optimizer/qualify.html` & `sqlglot-doris-1.0.2.dev3/docs/sqlglot/optimizer/qualify.html`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/docs/sqlglot/optimizer/qualify_columns.html` & `sqlglot-doris-1.0.2.dev3/docs/sqlglot/optimizer/qualify_columns.html`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/docs/sqlglot/optimizer/qualify_tables.html` & `sqlglot-doris-1.0.2.dev3/docs/sqlglot/optimizer/qualify_tables.html`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/docs/sqlglot/optimizer/scope.html` & `sqlglot-doris-1.0.2.dev3/docs/sqlglot/optimizer/scope.html`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/docs/sqlglot/optimizer/simplify.html` & `sqlglot-doris-1.0.2.dev3/docs/sqlglot/optimizer/simplify.html`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/docs/sqlglot/optimizer/unnest_subqueries.html` & `sqlglot-doris-1.0.2.dev3/docs/sqlglot/optimizer/unnest_subqueries.html`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/docs/sqlglot/optimizer.html` & `sqlglot-doris-1.0.2.dev3/docs/sqlglot/optimizer.html`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/docs/sqlglot/parser.html` & `sqlglot-doris-1.0.2.dev3/docs/sqlglot/parser.html`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/docs/sqlglot/planner.html` & `sqlglot-doris-1.0.2.dev3/docs/sqlglot/planner.html`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/docs/sqlglot/schema.html` & `sqlglot-doris-1.0.2.dev3/docs/sqlglot/schema.html`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/docs/sqlglot/serde.html` & `sqlglot-doris-1.0.2.dev3/docs/sqlglot/serde.html`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/docs/sqlglot/time.html` & `sqlglot-doris-1.0.2.dev3/docs/sqlglot/time.html`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/docs/sqlglot/tokens.html` & `sqlglot-doris-1.0.2.dev3/docs/sqlglot/tokens.html`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/docs/sqlglot/transforms.html` & `sqlglot-doris-1.0.2.dev3/docs/sqlglot/transforms.html`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/docs/sqlglot/trie.html` & `sqlglot-doris-1.0.2.dev3/docs/sqlglot/trie.html`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/docs/sqlglot.html` & `sqlglot-doris-1.0.2.dev3/docs/sqlglot.html`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/pdoc/cli.py` & `sqlglot-doris-1.0.2.dev3/pdoc/cli.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/posts/python_sql_engine.md` & `sqlglot-doris-1.0.2.dev3/posts/python_sql_engine.md`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/posts/python_sql_engine_images/executor.png` & `sqlglot-doris-1.0.2.dev3/posts/python_sql_engine_images/executor.png`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/posts/python_sql_engine_images/optimizer.png` & `sqlglot-doris-1.0.2.dev3/posts/python_sql_engine_images/optimizer.png`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/posts/python_sql_engine_images/parser.png` & `sqlglot-doris-1.0.2.dev3/posts/python_sql_engine_images/parser.png`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/posts/python_sql_engine_images/planner.png` & `sqlglot-doris-1.0.2.dev3/posts/python_sql_engine_images/planner.png`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/posts/python_sql_engine_images/tokenizer.png` & `sqlglot-doris-1.0.2.dev3/posts/python_sql_engine_images/tokenizer.png`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/posts/sql_diff.md` & `sqlglot-doris-1.0.2.dev3/posts/sql_diff.md`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/posts/sql_diff_images/dice_coef.png` & `sqlglot-doris-1.0.2.dev3/posts/sql_diff_images/dice_coef.png`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/posts/sql_diff_images/figure_1.png` & `sqlglot-doris-1.0.2.dev3/posts/sql_diff_images/figure_1.png`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/posts/sql_diff_images/figure_2.gif` & `sqlglot-doris-1.0.2.dev3/posts/sql_diff_images/figure_2.gif`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/posts/sql_diff_images/figure_3.gif` & `sqlglot-doris-1.0.2.dev3/posts/sql_diff_images/figure_3.gif`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/posts/sql_diff_images/git_diff_output.png` & `sqlglot-doris-1.0.2.dev3/posts/sql_diff_images/git_diff_output.png`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/posts/sql_diff_images/matching_criteria_1.png` & `sqlglot-doris-1.0.2.dev3/posts/sql_diff_images/matching_criteria_1.png`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/posts/sql_diff_images/matching_criteria_2.png` & `sqlglot-doris-1.0.2.dev3/posts/sql_diff_images/matching_criteria_2.png`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/setup.cfg` & `sqlglot-doris-1.0.2.dev3/setup.cfg`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/setup.py` & `sqlglot-doris-1.0.2.dev3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="sqlglot-doris",
-    version="1.0.1.dev3",
+    version="1.0.2.dev3",
     description="An easily customizable SQL parser and transpiler",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/tobymao/sqlglot",
     author="Toby Mao",
     author_email="toby.mao@gmail.com",
     license="MIT",
```

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/__init__.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/__main__.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/__main__.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/dataframe/README.md` & `sqlglot-doris-1.0.2.dev3/sqlglot/dataframe/README.md`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/dataframe/sql/__init__.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/dataframe/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/dataframe/sql/_typing.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/dataframe/sql/_typing.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/dataframe/sql/column.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/dataframe/sql/column.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/dataframe/sql/dataframe.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/dataframe/sql/dataframe.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/dataframe/sql/functions.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/dataframe/sql/functions.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/dataframe/sql/group.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/dataframe/sql/group.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/dataframe/sql/normalize.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/dataframe/sql/normalize.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/dataframe/sql/operations.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/dataframe/sql/operations.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/dataframe/sql/readwriter.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/dataframe/sql/readwriter.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/dataframe/sql/session.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/dataframe/sql/session.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/dataframe/sql/types.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/dataframe/sql/types.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/dataframe/sql/util.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/dataframe/sql/util.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/dataframe/sql/window.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/dataframe/sql/window.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/dialects/__init__.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/dialects/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/dialects/bigquery.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/dialects/bigquery.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/dialects/clickhouse.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/dialects/clickhouse.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/dialects/databricks.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/dialects/databricks.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/dialects/dialect.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/dialects/dialect.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/dialects/doris.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/dialects/doris.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,46 @@
 from __future__ import annotations
 
-from sqlglot import exp
+from sqlglot import exp, generator, parser, tokens, transforms
 from sqlglot.dialects.dialect import (
     approx_count_distinct_sql,
     arrow_json_extract_sql,
     rename_func,
 )
 from sqlglot.dialects.mysql import MySQL
 from sqlglot.helper import seq_get
 from sqlglot.tokens import TokenType
 
+# (FuncType, Multiplier)
+DATE_DELTA_INTERVAL = {
+    "YEAR": ("ADD_MONTHS", 12),
+    "MONTH": ("ADD_MONTHS", 1),
+    "QUARTER": ("ADD_MONTHS", 3),
+    "WEEK": ("DATE_ADD", 7),
+    "DAY": ("DATE_ADD", 1),
+}
+
+# TRANSFORMS.pop(exp.DateTrunc)
+def _add_date_sql(self: generator.Generator, expression: exp.DateAdd | exp.DateSub) -> str:
+    unit = expression.text("unit").upper()
+    func, multiplier = DATE_DELTA_INTERVAL.get(unit, ("DATE_ADD", 1))
+
+    if isinstance(expression, exp.DateSub):
+        multiplier *= -1
+
+    if expression.expression.is_number:
+        modified_increment = exp.Literal.number(int(expression.text("expression")) * multiplier)
+    else:
+        modified_increment = expression.expression
+        if multiplier != 1:
+            modified_increment = exp.Mul(  # type: ignore
+                this=modified_increment, expression=exp.Literal.number(multiplier)
+            )
+
+    return self.func(func, expression.this, modified_increment)
 class Doris(MySQL):
     class Parser(MySQL.Parser):
         FUNCTIONS = {
             **MySQL.Parser.FUNCTIONS,
             "DATE_TRUNC": lambda args: exp.TimestampTrunc(
                 this=seq_get(args, 1), unit=seq_get(args, 0)
             ),
@@ -62,10 +89,15 @@
             exp.StrToUnix: lambda self, e: f"UNIX_TIMESTAMP({self.sql(e, 'this')}, {self.format_time(e)})",
             exp.TimestampTrunc: lambda self, e: self.func(
                 "DATE_TRUNC", exp.Literal.string(e.text("unit")), e.this
             ),
             exp.TimeStrToDate: rename_func("TO_DATE"),
             exp.UnixToStr: lambda self, e: f"FROM_UNIXTIME({self.sql(e, 'this')}, {self.format_time(e)})",
             exp.UnixToTime: rename_func("FROM_UNIXTIME"),
+            exp.ArrayAgg: rename_func("COLLECT_LIST"),
+            exp.SetAgg: rename_func("COLLECT_SET"),
+            exp.TsOrDsAdd: rename_func("DATE_ADD"),
+            exp.DateSub: rename_func("DATE_ADD"),
         }
 
-        # TRANSFORMS.pop(exp.DateTrunc)
+
+
```

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/dialects/drill.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/dialects/drill.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/dialects/duckdb.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/dialects/duckdb.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/dialects/hive.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/dialects/hive.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/dialects/mysql.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/dialects/mysql.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/dialects/oracle.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/dialects/oracle.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/dialects/postgres.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/dialects/postgres.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/dialects/presto.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/dialects/presto.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/dialects/redshift.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/dialects/redshift.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/dialects/snowflake.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/dialects/snowflake.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/dialects/spark.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/dialects/spark.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/dialects/spark2.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/dialects/spark2.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/dialects/sqlite.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/dialects/sqlite.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/dialects/starrocks.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/dialects/starrocks.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/dialects/tableau.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/dialects/tableau.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/dialects/teradata.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/dialects/teradata.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/dialects/tsql.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/dialects/tsql.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/diff.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/diff.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/errors.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/errors.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/executor/__init__.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/executor/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/executor/context.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/executor/context.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/executor/env.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/executor/env.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/executor/python.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/executor/python.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/executor/table.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/executor/table.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/expressions.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/expressions.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/generator.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/generator.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/helper.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/helper.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/lineage.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/lineage.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/optimizer/annotate_types.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/optimizer/annotate_types.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/optimizer/canonicalize.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/optimizer/canonicalize.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/optimizer/eliminate_ctes.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/optimizer/eliminate_ctes.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/optimizer/eliminate_joins.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/optimizer/eliminate_joins.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/optimizer/eliminate_subqueries.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/optimizer/eliminate_subqueries.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/optimizer/isolate_table_selects.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/optimizer/isolate_table_selects.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/optimizer/merge_subqueries.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/optimizer/merge_subqueries.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/optimizer/normalize.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/optimizer/normalize.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/optimizer/normalize_identifiers.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/optimizer/normalize_identifiers.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/optimizer/optimize_joins.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/optimizer/optimize_joins.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/optimizer/optimizer.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/optimizer/optimizer.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/optimizer/pushdown_predicates.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/optimizer/pushdown_predicates.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/optimizer/pushdown_projections.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/optimizer/pushdown_projections.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/optimizer/qualify.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/optimizer/qualify.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/optimizer/qualify_columns.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/optimizer/qualify_columns.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/optimizer/qualify_tables.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/optimizer/qualify_tables.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/optimizer/scope.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/optimizer/scope.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/optimizer/simplify.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/optimizer/simplify.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/optimizer/unnest_subqueries.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/optimizer/unnest_subqueries.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/parser.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/parser.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/planner.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/planner.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/schema.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/schema.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/serde.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/serde.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/time.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/time.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/tokens.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/tokens.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/transforms.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/transforms.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot/trie.py` & `sqlglot-doris-1.0.2.dev3/sqlglot/trie.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot.svg` & `sqlglot-doris-1.0.2.dev3/sqlglot.svg`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot_doris.egg-info/PKG-INFO` & `sqlglot-doris-1.0.2.dev3/sqlglot_doris.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlglot-doris
-Version: 1.0.1.dev3
+Version: 1.0.2.dev3
 Summary: An easily customizable SQL parser and transpiler
 Home-page: https://github.com/tobymao/sqlglot
 Author: Toby Mao
 Author-email: toby.mao@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `sqlglot-doris-1.0.1.dev3/sqlglot_doris.egg-info/SOURCES.txt` & `sqlglot-doris-1.0.2.dev3/sqlglot_doris.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 .gitignore
 .pre-commit-config.yaml
 CHANGELOG.md
 CONTRIBUTING.md
 LICENSE
 Makefile
 README.md
+READMEBASE.md
 setup.cfg
 setup.py
 sqlglot.svg
+test_doris.py
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/feature_request.md
 .github/workflows/python-package.yml
 .github/workflows/python-publish.yml
 benchmarks/bench.py
 docs/CNAME
 docs/index.html
@@ -224,14 +226,15 @@
 tests/dataframe/unit/test_types.py
 tests/dataframe/unit/test_window.py
 tests/dialects/__init__.py
 tests/dialects/test_bigquery.py
 tests/dialects/test_clickhouse.py
 tests/dialects/test_databricks.py
 tests/dialects/test_dialect.py
+tests/dialects/test_doris.py
 tests/dialects/test_drill.py
 tests/dialects/test_duckdb.py
 tests/dialects/test_hive.py
 tests/dialects/test_mysql.py
 tests/dialects/test_oracle.py
 tests/dialects/test_postgres.py
 tests/dialects/test_presto.py
```

### Comparing `sqlglot-doris-1.0.1.dev3/tests/dataframe/integration/dataframe_validator.py` & `sqlglot-doris-1.0.2.dev3/tests/dataframe/integration/dataframe_validator.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/dataframe/integration/test_dataframe.py` & `sqlglot-doris-1.0.2.dev3/tests/dataframe/integration/test_dataframe.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/dataframe/integration/test_grouped_data.py` & `sqlglot-doris-1.0.2.dev3/tests/dataframe/integration/test_grouped_data.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/dataframe/integration/test_session.py` & `sqlglot-doris-1.0.2.dev3/tests/dataframe/integration/test_session.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/dataframe/unit/dataframe_sql_validator.py` & `sqlglot-doris-1.0.2.dev3/tests/dataframe/unit/dataframe_sql_validator.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/dataframe/unit/test_column.py` & `sqlglot-doris-1.0.2.dev3/tests/dataframe/unit/test_column.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/dataframe/unit/test_dataframe.py` & `sqlglot-doris-1.0.2.dev3/tests/dataframe/unit/test_dataframe.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/dataframe/unit/test_dataframe_writer.py` & `sqlglot-doris-1.0.2.dev3/tests/dataframe/unit/test_dataframe_writer.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/dataframe/unit/test_functions.py` & `sqlglot-doris-1.0.2.dev3/tests/dataframe/unit/test_functions.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/dataframe/unit/test_session.py` & `sqlglot-doris-1.0.2.dev3/tests/dataframe/unit/test_session.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/dataframe/unit/test_types.py` & `sqlglot-doris-1.0.2.dev3/tests/dataframe/unit/test_types.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/dataframe/unit/test_window.py` & `sqlglot-doris-1.0.2.dev3/tests/dataframe/unit/test_window.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/dialects/test_bigquery.py` & `sqlglot-doris-1.0.2.dev3/tests/dialects/test_bigquery.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/dialects/test_clickhouse.py` & `sqlglot-doris-1.0.2.dev3/tests/dialects/test_clickhouse.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/dialects/test_databricks.py` & `sqlglot-doris-1.0.2.dev3/tests/dialects/test_databricks.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/dialects/test_dialect.py` & `sqlglot-doris-1.0.2.dev3/tests/dialects/test_dialect.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/dialects/test_drill.py` & `sqlglot-doris-1.0.2.dev3/tests/dialects/test_drill.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/dialects/test_duckdb.py` & `sqlglot-doris-1.0.2.dev3/tests/dialects/test_duckdb.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/dialects/test_hive.py` & `sqlglot-doris-1.0.2.dev3/tests/dialects/test_hive.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/dialects/test_mysql.py` & `sqlglot-doris-1.0.2.dev3/tests/dialects/test_mysql.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/dialects/test_oracle.py` & `sqlglot-doris-1.0.2.dev3/tests/dialects/test_oracle.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/dialects/test_postgres.py` & `sqlglot-doris-1.0.2.dev3/tests/dialects/test_postgres.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/dialects/test_presto.py` & `sqlglot-doris-1.0.2.dev3/tests/dialects/test_presto.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/dialects/test_redshift.py` & `sqlglot-doris-1.0.2.dev3/tests/dialects/test_redshift.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/dialects/test_snowflake.py` & `sqlglot-doris-1.0.2.dev3/tests/dialects/test_snowflake.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/dialects/test_spark.py` & `sqlglot-doris-1.0.2.dev3/tests/dialects/test_spark.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/dialects/test_sqlite.py` & `sqlglot-doris-1.0.2.dev3/tests/dialects/test_sqlite.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/dialects/test_starrocks.py` & `sqlglot-doris-1.0.2.dev3/tests/dialects/test_starrocks.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/dialects/test_tableau.py` & `sqlglot-doris-1.0.2.dev3/tests/dialects/test_tableau.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/dialects/test_teradata.py` & `sqlglot-doris-1.0.2.dev3/tests/dialects/test_teradata.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/dialects/test_tsql.py` & `sqlglot-doris-1.0.2.dev3/tests/dialects/test_tsql.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/fixtures/identity.sql` & `sqlglot-doris-1.0.2.dev3/tests/fixtures/identity.sql`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/fixtures/optimizer/canonicalize.sql` & `sqlglot-doris-1.0.2.dev3/tests/fixtures/optimizer/canonicalize.sql`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/fixtures/optimizer/eliminate_joins.sql` & `sqlglot-doris-1.0.2.dev3/tests/fixtures/optimizer/eliminate_joins.sql`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/fixtures/optimizer/eliminate_subqueries.sql` & `sqlglot-doris-1.0.2.dev3/tests/fixtures/optimizer/eliminate_subqueries.sql`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/fixtures/optimizer/isolate_table_selects.sql` & `sqlglot-doris-1.0.2.dev3/tests/fixtures/optimizer/isolate_table_selects.sql`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/fixtures/optimizer/merge_subqueries.sql` & `sqlglot-doris-1.0.2.dev3/tests/fixtures/optimizer/merge_subqueries.sql`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/fixtures/optimizer/normalize.sql` & `sqlglot-doris-1.0.2.dev3/tests/fixtures/optimizer/normalize.sql`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/fixtures/optimizer/normalize_identifiers.sql` & `sqlglot-doris-1.0.2.dev3/tests/fixtures/optimizer/normalize_identifiers.sql`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/fixtures/optimizer/optimize_joins.sql` & `sqlglot-doris-1.0.2.dev3/tests/fixtures/optimizer/optimize_joins.sql`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/fixtures/optimizer/optimizer.sql` & `sqlglot-doris-1.0.2.dev3/tests/fixtures/optimizer/optimizer.sql`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/fixtures/optimizer/pushdown_predicates.sql` & `sqlglot-doris-1.0.2.dev3/tests/fixtures/optimizer/pushdown_predicates.sql`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/fixtures/optimizer/pushdown_projections.sql` & `sqlglot-doris-1.0.2.dev3/tests/fixtures/optimizer/pushdown_projections.sql`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/fixtures/optimizer/qualify_columns.sql` & `sqlglot-doris-1.0.2.dev3/tests/fixtures/optimizer/qualify_columns.sql`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/fixtures/optimizer/qualify_columns__invalid.sql` & `sqlglot-doris-1.0.2.dev3/tests/fixtures/optimizer/qualify_columns__invalid.sql`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/fixtures/optimizer/qualify_columns__with_invisible.sql` & `sqlglot-doris-1.0.2.dev3/tests/fixtures/optimizer/qualify_columns__with_invisible.sql`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/fixtures/optimizer/qualify_columns_ddl.sql` & `sqlglot-doris-1.0.2.dev3/tests/fixtures/optimizer/qualify_columns_ddl.sql`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/fixtures/optimizer/qualify_tables.sql` & `sqlglot-doris-1.0.2.dev3/tests/fixtures/optimizer/qualify_tables.sql`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/fixtures/optimizer/simplify.sql` & `sqlglot-doris-1.0.2.dev3/tests/fixtures/optimizer/simplify.sql`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/fixtures/optimizer/tpc-ds/tpc-ds.sql` & `sqlglot-doris-1.0.2.dev3/tests/fixtures/optimizer/tpc-ds/tpc-ds.sql`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/fixtures/optimizer/tpc-h/customer.csv.gz` & `sqlglot-doris-1.0.2.dev3/tests/fixtures/optimizer/tpc-h/customer.csv.gz`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/fixtures/optimizer/tpc-h/lineitem.csv.gz` & `sqlglot-doris-1.0.2.dev3/tests/fixtures/optimizer/tpc-h/lineitem.csv.gz`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/fixtures/optimizer/tpc-h/nation.csv.gz` & `sqlglot-doris-1.0.2.dev3/tests/fixtures/optimizer/tpc-h/nation.csv.gz`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/fixtures/optimizer/tpc-h/orders.csv.gz` & `sqlglot-doris-1.0.2.dev3/tests/fixtures/optimizer/tpc-h/orders.csv.gz`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/fixtures/optimizer/tpc-h/part.csv.gz` & `sqlglot-doris-1.0.2.dev3/tests/fixtures/optimizer/tpc-h/part.csv.gz`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/fixtures/optimizer/tpc-h/partsupp.csv.gz` & `sqlglot-doris-1.0.2.dev3/tests/fixtures/optimizer/tpc-h/partsupp.csv.gz`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/fixtures/optimizer/tpc-h/supplier.csv.gz` & `sqlglot-doris-1.0.2.dev3/tests/fixtures/optimizer/tpc-h/supplier.csv.gz`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/fixtures/optimizer/tpc-h/tpc-h.sql` & `sqlglot-doris-1.0.2.dev3/tests/fixtures/optimizer/tpc-h/tpc-h.sql`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/fixtures/optimizer/unnest_subqueries.sql` & `sqlglot-doris-1.0.2.dev3/tests/fixtures/optimizer/unnest_subqueries.sql`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/fixtures/pretty.sql` & `sqlglot-doris-1.0.2.dev3/tests/fixtures/pretty.sql`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/helpers.py` & `sqlglot-doris-1.0.2.dev3/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/test_build.py` & `sqlglot-doris-1.0.2.dev3/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/test_diff.py` & `sqlglot-doris-1.0.2.dev3/tests/test_diff.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/test_docs.py` & `sqlglot-doris-1.0.2.dev3/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/test_executor.py` & `sqlglot-doris-1.0.2.dev3/tests/test_executor.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/test_expressions.py` & `sqlglot-doris-1.0.2.dev3/tests/test_expressions.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/test_generator.py` & `sqlglot-doris-1.0.2.dev3/tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/test_helper.py` & `sqlglot-doris-1.0.2.dev3/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/test_lineage.py` & `sqlglot-doris-1.0.2.dev3/tests/test_lineage.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/test_optimizer.py` & `sqlglot-doris-1.0.2.dev3/tests/test_optimizer.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/test_parser.py` & `sqlglot-doris-1.0.2.dev3/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/test_schema.py` & `sqlglot-doris-1.0.2.dev3/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/test_serde.py` & `sqlglot-doris-1.0.2.dev3/tests/test_serde.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/test_tokens.py` & `sqlglot-doris-1.0.2.dev3/tests/test_tokens.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/test_transforms.py` & `sqlglot-doris-1.0.2.dev3/tests/test_transforms.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/test_transpile.py` & `sqlglot-doris-1.0.2.dev3/tests/test_transpile.py`

 * *Files identical despite different names*

### Comparing `sqlglot-doris-1.0.1.dev3/tests/tpch.py` & `sqlglot-doris-1.0.2.dev3/tests/tpch.py`

 * *Files identical despite different names*

