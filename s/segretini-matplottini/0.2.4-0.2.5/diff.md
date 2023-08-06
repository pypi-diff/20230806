# Comparing `tmp/segretini-matplottini-0.2.4.tar.gz` & `tmp/segretini-matplottini-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "segretini-matplottini-0.2.4.tar", last modified: Sun Aug  6 19:30:35 2023, max compression
+gzip compressed data, was "segretini-matplottini-0.2.5.tar", last modified: Sun Aug  6 19:43:44 2023, max compression
```

## Comparing `segretini-matplottini-0.2.4.tar` & `segretini-matplottini-0.2.5.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:30:35.462364 segretini-matplottini-0.2.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:30:35.430364 segretini-matplottini-0.2.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:30:35.430364 segretini-matplottini-0.2.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/.github/workflows/pull_request.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/.github/workflows/pypi_release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:30:35.434364 segretini-matplottini-0.2.4/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     5524 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12122 2023-08-06 19:30:35.458364 segretini-matplottini-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10500 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:30:35.434364 segretini-matplottini-0.2.4/data/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/data/barplot_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/data/barplot_for_multiple_categories_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/data/correlation_scatterplot_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)    25669 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/data/density_data.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:30:35.430364 segretini-matplottini-0.2.4/data/notebooks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:30:35.434364 segretini-matplottini-0.2.4/data/notebooks/1_getting_started_with_barplots/
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/data/notebooks/1_getting_started_with_barplots/barplot_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/data/performance_scaling_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)    60208 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/data/ridgeplot_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)   134509 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/data/timeseries_data.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:30:35.434364 segretini-matplottini-0.2.4/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/examples/plot_barplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/examples/plot_binary_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/examples/plot_correlation_scatterplot.py
--rw-r--r--   0 runner    (1001) docker     (123)    10527 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/examples/plot_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    10487 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/examples/plot_performance_scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/examples/plot_ridgeplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6240 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/examples/plot_roofline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/examples/plot_timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/mypy.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:30:35.434364 segretini-matplottini-0.2.4/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)   103687 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/notebooks/1_getting_started_with_barplots.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:30:35.450364 segretini-matplottini-0.2.4/plots/
--rw-r--r--   0 runner    (1001) docker     (123)    11274 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/plots/barplot.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    34869 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/plots/barplot.png
--rw-r--r--   0 runner    (1001) docker     (123)    15571 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/plots/barplot_for_multiple_categories.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    60298 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/plots/barplot_for_multiple_categories.png
--rw-r--r--   0 runner    (1001) docker     (123)    15273 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/plots/barplots.pdf
--rw-r--r--   0 runner    (1001) docker     (123)   108326 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/plots/barplots.png
--rw-r--r--   0 runner    (1001) docker     (123)    38357 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/plots/binary_classification.pdf
--rw-r--r--   0 runner    (1001) docker     (123)   228919 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/plots/binary_classification.png
--rw-r--r--   0 runner    (1001) docker     (123)    33890 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/plots/correlation_scatterplot.pdf
--rw-r--r--   0 runner    (1001) docker     (123)   206682 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/plots/correlation_scatterplot.png
--rw-r--r--   0 runner    (1001) docker     (123)   851461 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/plots/grid.pdf
--rw-r--r--   0 runner    (1001) docker     (123)   965535 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/plots/grid.png
--rw-r--r--   0 runner    (1001) docker     (123)   782002 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/plots/grid_2.pdf
--rw-r--r--   0 runner    (1001) docker     (123)   900189 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/plots/grid_2.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:30:35.430364 segretini-matplottini-0.2.4/plots/notebooks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:30:35.454364 segretini-matplottini-0.2.4/plots/notebooks/1_getting_started_with_barplots/
--rw-r--r--   0 runner    (1001) docker     (123)    74133 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/plots/notebooks/1_getting_started_with_barplots/a_much_better_barplot.png
--rw-r--r--   0 runner    (1001) docker     (123)    15661 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/plots/notebooks/1_getting_started_with_barplots/our_amazing_barplot.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    54750 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/plots/notebooks/1_getting_started_with_barplots/our_amazing_barplot.png
--rw-r--r--   0 runner    (1001) docker     (123)    16746 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/plots/notebooks/1_getting_started_with_barplots/our_amazing_barplot_v2.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    56901 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/plots/notebooks/1_getting_started_with_barplots/our_amazing_barplot_v2.png
--rw-r--r--   0 runner    (1001) docker     (123)    16615 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/plots/notebooks/1_getting_started_with_barplots/our_amazing_barplot_v3.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    53406 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/plots/notebooks/1_getting_started_with_barplots/our_amazing_barplot_v3.png
--rw-r--r--   0 runner    (1001) docker     (123)    19563 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/plots/notebooks/1_getting_started_with_barplots/the_ugliest_barplot.png
--rw-r--r--   0 runner    (1001) docker     (123)    30521 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/plots/performance_scaling.pdf
--rw-r--r--   0 runner    (1001) docker     (123)   264083 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/plots/performance_scaling.png
--rw-r--r--   0 runner    (1001) docker     (123)    96597 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/plots/ridgeplot_compact.pdf
--rw-r--r--   0 runner    (1001) docker     (123)   403977 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/plots/ridgeplot_compact.png
--rw-r--r--   0 runner    (1001) docker     (123)   100120 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/plots/ridgeplot_large.pdf
--rw-r--r--   0 runner    (1001) docker     (123)   582502 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/plots/ridgeplot_large.png
--rw-r--r--   0 runner    (1001) docker     (123)    16056 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/plots/roofline.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    78276 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/plots/roofline.png
--rw-r--r--   0 runner    (1001) docker     (123)    20642 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/plots/roofline_double.pdf
--rw-r--r--   0 runner    (1001) docker     (123)   215335 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/plots/roofline_double.png
--rw-r--r--   0 runner    (1001) docker     (123)    18219 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/plots/roofline_stacked.pdf
--rw-r--r--   0 runner    (1001) docker     (123)   175021 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/plots/roofline_stacked.png
--rw-r--r--   0 runner    (1001) docker     (123)    19875 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/plots/stem.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    83115 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/plots/stem.png
--rw-r--r--   0 runner    (1001) docker     (123)    29257 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/plots/timeseries.pdf
--rw-r--r--   0 runner    (1001) docker     (123)   279591 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/plots/timeseries.png
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/ruff.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:30:35.454364 segretini-matplottini-0.2.4/segretini_matplottini/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/segretini_matplottini/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:30:35.454364 segretini-matplottini-0.2.4/segretini_matplottini/plot/
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/segretini_matplottini/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24737 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/segretini_matplottini/plot/barplot.py
--rw-r--r--   0 runner    (1001) docker     (123)    51366 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/segretini_matplottini/plot/binary_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)    10544 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/segretini_matplottini/plot/correlation_scatterplot.py
--rw-r--r--   0 runner    (1001) docker     (123)    25419 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/segretini_matplottini/plot/ridgeplot.py
--rw-r--r--   0 runner    (1001) docker     (123)    13206 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/segretini_matplottini/plot/roofline.py
--rw-r--r--   0 runner    (1001) docker     (123)     9102 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/segretini_matplottini/plot/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/segretini_matplottini/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:30:35.458364 segretini-matplottini-0.2.4/segretini_matplottini/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/segretini_matplottini/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17140 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/segretini_matplottini/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/segretini_matplottini/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    18079 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/segretini_matplottini/utils/data.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4813 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/segretini_matplottini/utils/legend.py
--rw-r--r--   0 runner    (1001) docker     (123)    23306 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/segretini_matplottini/utils/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:30:35.454364 segretini-matplottini-0.2.4/segretini_matplottini.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12122 2023-08-06 19:30:35.000000 segretini-matplottini-0.2.4/segretini_matplottini.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-08-06 19:30:35.000000 segretini-matplottini-0.2.4/segretini_matplottini.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 19:30:35.000000 segretini-matplottini-0.2.4/segretini_matplottini.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-08-06 19:30:35.000000 segretini-matplottini-0.2.4/segretini_matplottini.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-06 19:30:35.000000 segretini-matplottini-0.2.4/segretini_matplottini.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 19:30:35.462364 segretini-matplottini-0.2.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:30:35.430364 segretini-matplottini-0.2.4/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:30:35.458364 segretini-matplottini-0.2.4/tests/plot/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/tests/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11053 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/tests/plot/test_barplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/tests/plot/test_binary_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/tests/plot/test_correlation_scatterplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/tests/plot/test_ridgeplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/tests/plot/test_roofline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/tests/plot/test_timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/tests/plot/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:30:35.458364 segretini-matplottini-0.2.4/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/tests/utils/test_colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-08-06 19:29:41.000000 segretini-matplottini-0.2.4/tests/utils/test_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:43:44.348914 segretini-matplottini-0.2.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:43:44.328914 segretini-matplottini-0.2.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:43:44.332914 segretini-matplottini-0.2.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/.github/workflows/pull_request.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/.github/workflows/pypi_release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:43:44.332914 segretini-matplottini-0.2.5/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5524 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12122 2023-08-06 19:43:44.348914 segretini-matplottini-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10500 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:43:44.332914 segretini-matplottini-0.2.5/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/data/barplot_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/data/barplot_for_multiple_categories_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/data/correlation_scatterplot_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    25669 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/data/density_data.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:43:44.328914 segretini-matplottini-0.2.5/data/notebooks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:43:44.332914 segretini-matplottini-0.2.5/data/notebooks/1_getting_started_with_barplots/
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/data/notebooks/1_getting_started_with_barplots/barplot_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/data/performance_scaling_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    60208 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/data/ridgeplot_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   134509 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/data/timeseries_data.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:43:44.332914 segretini-matplottini-0.2.5/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/examples/plot_barplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/examples/plot_binary_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/examples/plot_correlation_scatterplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10527 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/examples/plot_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10487 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/examples/plot_performance_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/examples/plot_ridgeplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6240 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/examples/plot_roofline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/examples/plot_timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/mypy.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:43:44.332914 segretini-matplottini-0.2.5/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)   103687 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/notebooks/1_getting_started_with_barplots.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:43:44.344914 segretini-matplottini-0.2.5/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)    11274 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/plots/barplot.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    34869 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/plots/barplot.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15571 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/plots/barplot_for_multiple_categories.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    60298 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/plots/barplot_for_multiple_categories.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15273 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/plots/barplots.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)   108326 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/plots/barplots.png
+-rw-r--r--   0 runner    (1001) docker     (123)    38357 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/plots/binary_classification.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)   228919 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/plots/binary_classification.png
+-rw-r--r--   0 runner    (1001) docker     (123)    33890 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/plots/correlation_scatterplot.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)   206682 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/plots/correlation_scatterplot.png
+-rw-r--r--   0 runner    (1001) docker     (123)   851461 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/plots/grid.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)   965535 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/plots/grid.png
+-rw-r--r--   0 runner    (1001) docker     (123)   782002 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/plots/grid_2.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)   900189 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/plots/grid_2.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:43:44.328914 segretini-matplottini-0.2.5/plots/notebooks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:43:44.344914 segretini-matplottini-0.2.5/plots/notebooks/1_getting_started_with_barplots/
+-rw-r--r--   0 runner    (1001) docker     (123)    74133 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/plots/notebooks/1_getting_started_with_barplots/a_much_better_barplot.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15661 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/plots/notebooks/1_getting_started_with_barplots/our_amazing_barplot.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    54750 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/plots/notebooks/1_getting_started_with_barplots/our_amazing_barplot.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16746 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/plots/notebooks/1_getting_started_with_barplots/our_amazing_barplot_v2.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    56901 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/plots/notebooks/1_getting_started_with_barplots/our_amazing_barplot_v2.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16615 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/plots/notebooks/1_getting_started_with_barplots/our_amazing_barplot_v3.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    53406 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/plots/notebooks/1_getting_started_with_barplots/our_amazing_barplot_v3.png
+-rw-r--r--   0 runner    (1001) docker     (123)    19563 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/plots/notebooks/1_getting_started_with_barplots/the_ugliest_barplot.png
+-rw-r--r--   0 runner    (1001) docker     (123)    30521 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/plots/performance_scaling.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)   264083 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/plots/performance_scaling.png
+-rw-r--r--   0 runner    (1001) docker     (123)    96597 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/plots/ridgeplot_compact.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)   403977 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/plots/ridgeplot_compact.png
+-rw-r--r--   0 runner    (1001) docker     (123)   100120 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/plots/ridgeplot_large.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)   582502 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/plots/ridgeplot_large.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16056 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/plots/roofline.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    78276 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/plots/roofline.png
+-rw-r--r--   0 runner    (1001) docker     (123)    20642 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/plots/roofline_double.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)   215335 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/plots/roofline_double.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18219 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/plots/roofline_stacked.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)   175021 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/plots/roofline_stacked.png
+-rw-r--r--   0 runner    (1001) docker     (123)    19875 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/plots/stem.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    83115 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/plots/stem.png
+-rw-r--r--   0 runner    (1001) docker     (123)    29257 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/plots/timeseries.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)   279591 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/plots/timeseries.png
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/ruff.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:43:44.344914 segretini-matplottini-0.2.5/segretini_matplottini/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/segretini_matplottini/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:43:44.348914 segretini-matplottini-0.2.5/segretini_matplottini/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/segretini_matplottini/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24737 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/segretini_matplottini/plot/barplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51366 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/segretini_matplottini/plot/binary_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10544 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/segretini_matplottini/plot/correlation_scatterplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25419 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/segretini_matplottini/plot/ridgeplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13206 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/segretini_matplottini/plot/roofline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9102 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/segretini_matplottini/plot/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/segretini_matplottini/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:43:44.348914 segretini-matplottini-0.2.5/segretini_matplottini/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/segretini_matplottini/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17140 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/segretini_matplottini/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/segretini_matplottini/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18079 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/segretini_matplottini/utils/data.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4813 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/segretini_matplottini/utils/legend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23306 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/segretini_matplottini/utils/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:43:44.344914 segretini-matplottini-0.2.5/segretini_matplottini.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12122 2023-08-06 19:43:44.000000 segretini-matplottini-0.2.5/segretini_matplottini.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-08-06 19:43:44.000000 segretini-matplottini-0.2.5/segretini_matplottini.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 19:43:44.000000 segretini-matplottini-0.2.5/segretini_matplottini.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-08-06 19:43:44.000000 segretini-matplottini-0.2.5/segretini_matplottini.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-06 19:43:44.000000 segretini-matplottini-0.2.5/segretini_matplottini.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 19:43:44.348914 segretini-matplottini-0.2.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:43:44.332914 segretini-matplottini-0.2.5/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:43:44.348914 segretini-matplottini-0.2.5/tests/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/tests/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11053 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/tests/plot/test_barplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/tests/plot/test_binary_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/tests/plot/test_correlation_scatterplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/tests/plot/test_ridgeplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/tests/plot/test_roofline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/tests/plot/test_timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/tests/plot/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:43:44.348914 segretini-matplottini-0.2.5/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/tests/utils/test_colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-08-06 19:42:57.000000 segretini-matplottini-0.2.5/tests/utils/test_data.py
```

### Comparing `segretini-matplottini-0.2.4/.github/workflows/pull_request.yaml` & `segretini-matplottini-0.2.5/.github/workflows/pull_request.yaml`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/.github/workflows/pypi_release.yaml` & `segretini-matplottini-0.2.5/.github/workflows/pypi_release.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -15,41 +15,46 @@
     if: github.event.pull_request.merged == true
     environment:
       name: pypi
       url: https://pypi.org/project/segretini-matplottini/
     permissions:
       id-token: write
       contents: write
-
+    outputs:
+      tag_name: ${{ steps.get_tag_name.outputs.tag_name }}
+  
     steps:
     - name: Checkout code
       uses: actions/checkout@v3
     - name: Set up Python
       uses: actions/setup-python@v4
       with:
         python-version: "3.x"
     - name: Install dependencies
       run: |
         python -m pip install ".[dev]" --upgrade pip
     - name: Build package
       run: python -m build
     - name: Publish distribution to PyPI 📦
       uses: pypa/gh-action-pypi-publish@release/v1
+    - name: Extract tag name
+      id: get_tag_name
+      run: echo "tag_name=v$(grep -E '^version = ".*"$' pyproject.toml | cut -d'"' -f2)" >> $GITHUB_OUTPUT
     - name: Create GitHub Release
       uses: "marvinpinto/action-automatic-releases@latest"
       with:
         repo_token: ${{ secrets.GITHUB_TOKEN }}
-        automatic_release_tag: v$(grep -E '^version = ".*"$' pyproject.toml | cut -d'"' -f2)
+        automatic_release_tag: ${{ steps.get_tag_name.outputs.tag_name }}
         prerelease: false
         draft: false
-        title: "Automated release with tag ${{ steps.create_release.outputs.tag_name }}."
+        title: "Automated release with tag ${{ steps.get_tag_name.outputs.tag_name }}."
         files: |
           dist/*
           CHANGELOG.md
           LICENSE
 
     - name: Commit changes
       run: |
         git config --local user.email "action@github.com"
         git config --local user.name "GitHub Action"
-        git commit -am "Bump version to v${{ steps.create_release.outputs.tag_name }}"
+        git commit -am "Bump version to ${{ steps.get_tag_name.outputs.TAG_NAME }}"
         git push
```

### Comparing `segretini-matplottini-0.2.4/.gitignore` & `segretini-matplottini-0.2.5/.gitignore`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/.pre-commit-config.yaml` & `segretini-matplottini-0.2.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/.vscode/launch.json` & `segretini-matplottini-0.2.5/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/CHANGELOG.md` & `segretini-matplottini-0.2.5/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/LICENSE` & `segretini-matplottini-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/PKG-INFO` & `segretini-matplottini-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segretini-matplottini
-Version: 0.2.4
+Version: 0.2.5
 Summary: Colorful recipes and utilities for Matplolib and Seaborn, to create publication-ready plots
 Author-email: Alberto Parravicini <alberto.parravicini@polimi.it>
 License: MIT License
         
         Copyright (c) 2020-2023 Alberto Parravicini
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `segretini-matplottini-0.2.4/README.md` & `segretini-matplottini-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/data/correlation_scatterplot_data.csv` & `segretini-matplottini-0.2.5/data/correlation_scatterplot_data.csv`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/data/density_data.csv` & `segretini-matplottini-0.2.5/data/density_data.csv`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/data/performance_scaling_data.csv` & `segretini-matplottini-0.2.5/data/performance_scaling_data.csv`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/data/ridgeplot_data.csv` & `segretini-matplottini-0.2.5/data/ridgeplot_data.csv`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/data/timeseries_data.csv` & `segretini-matplottini-0.2.5/data/timeseries_data.csv`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/examples/plot_barplot.py` & `segretini-matplottini-0.2.5/examples/plot_barplot.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/examples/plot_binary_classification.py` & `segretini-matplottini-0.2.5/examples/plot_binary_classification.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/examples/plot_correlation_scatterplot.py` & `segretini-matplottini-0.2.5/examples/plot_correlation_scatterplot.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/examples/plot_grid.py` & `segretini-matplottini-0.2.5/examples/plot_grid.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/examples/plot_performance_scaling.py` & `segretini-matplottini-0.2.5/examples/plot_performance_scaling.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/examples/plot_ridgeplot.py` & `segretini-matplottini-0.2.5/examples/plot_ridgeplot.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/examples/plot_roofline.py` & `segretini-matplottini-0.2.5/examples/plot_roofline.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/examples/plot_timeseries.py` & `segretini-matplottini-0.2.5/examples/plot_timeseries.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/mypy.ini` & `segretini-matplottini-0.2.5/mypy.ini`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/notebooks/1_getting_started_with_barplots.ipynb` & `segretini-matplottini-0.2.5/notebooks/1_getting_started_with_barplots.ipynb`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/plots/barplot.pdf` & `segretini-matplottini-0.2.5/plots/barplot.pdf`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/plots/barplot.png` & `segretini-matplottini-0.2.5/plots/barplot.png`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/plots/barplot_for_multiple_categories.pdf` & `segretini-matplottini-0.2.5/plots/barplot_for_multiple_categories.pdf`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/plots/barplot_for_multiple_categories.png` & `segretini-matplottini-0.2.5/plots/barplot_for_multiple_categories.png`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/plots/barplots.pdf` & `segretini-matplottini-0.2.5/plots/barplots.pdf`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/plots/barplots.png` & `segretini-matplottini-0.2.5/plots/barplots.png`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/plots/binary_classification.pdf` & `segretini-matplottini-0.2.5/plots/binary_classification.pdf`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/plots/binary_classification.png` & `segretini-matplottini-0.2.5/plots/binary_classification.png`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/plots/correlation_scatterplot.pdf` & `segretini-matplottini-0.2.5/plots/correlation_scatterplot.pdf`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/plots/correlation_scatterplot.png` & `segretini-matplottini-0.2.5/plots/correlation_scatterplot.png`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/plots/grid.pdf` & `segretini-matplottini-0.2.5/plots/grid.pdf`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/plots/grid.png` & `segretini-matplottini-0.2.5/plots/grid.png`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/plots/grid_2.pdf` & `segretini-matplottini-0.2.5/plots/grid_2.pdf`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/plots/grid_2.png` & `segretini-matplottini-0.2.5/plots/grid_2.png`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/plots/notebooks/1_getting_started_with_barplots/a_much_better_barplot.png` & `segretini-matplottini-0.2.5/plots/notebooks/1_getting_started_with_barplots/a_much_better_barplot.png`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/plots/notebooks/1_getting_started_with_barplots/our_amazing_barplot.pdf` & `segretini-matplottini-0.2.5/plots/notebooks/1_getting_started_with_barplots/our_amazing_barplot.pdf`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/plots/notebooks/1_getting_started_with_barplots/our_amazing_barplot.png` & `segretini-matplottini-0.2.5/plots/notebooks/1_getting_started_with_barplots/our_amazing_barplot.png`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/plots/notebooks/1_getting_started_with_barplots/our_amazing_barplot_v2.pdf` & `segretini-matplottini-0.2.5/plots/notebooks/1_getting_started_with_barplots/our_amazing_barplot_v2.pdf`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/plots/notebooks/1_getting_started_with_barplots/our_amazing_barplot_v2.png` & `segretini-matplottini-0.2.5/plots/notebooks/1_getting_started_with_barplots/our_amazing_barplot_v2.png`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/plots/notebooks/1_getting_started_with_barplots/our_amazing_barplot_v3.pdf` & `segretini-matplottini-0.2.5/plots/notebooks/1_getting_started_with_barplots/our_amazing_barplot_v3.pdf`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/plots/notebooks/1_getting_started_with_barplots/our_amazing_barplot_v3.png` & `segretini-matplottini-0.2.5/plots/notebooks/1_getting_started_with_barplots/our_amazing_barplot_v3.png`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/plots/notebooks/1_getting_started_with_barplots/the_ugliest_barplot.png` & `segretini-matplottini-0.2.5/plots/notebooks/1_getting_started_with_barplots/the_ugliest_barplot.png`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/plots/performance_scaling.pdf` & `segretini-matplottini-0.2.5/plots/performance_scaling.pdf`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/plots/performance_scaling.png` & `segretini-matplottini-0.2.5/plots/performance_scaling.png`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/plots/ridgeplot_compact.pdf` & `segretini-matplottini-0.2.5/plots/ridgeplot_compact.pdf`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/plots/ridgeplot_compact.png` & `segretini-matplottini-0.2.5/plots/ridgeplot_compact.png`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/plots/ridgeplot_large.pdf` & `segretini-matplottini-0.2.5/plots/ridgeplot_large.pdf`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/plots/ridgeplot_large.png` & `segretini-matplottini-0.2.5/plots/ridgeplot_large.png`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/plots/roofline.pdf` & `segretini-matplottini-0.2.5/plots/roofline.pdf`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/plots/roofline.png` & `segretini-matplottini-0.2.5/plots/roofline.png`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/plots/roofline_double.pdf` & `segretini-matplottini-0.2.5/plots/roofline_double.pdf`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/plots/roofline_double.png` & `segretini-matplottini-0.2.5/plots/roofline_double.png`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/plots/roofline_stacked.pdf` & `segretini-matplottini-0.2.5/plots/roofline_stacked.pdf`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/plots/roofline_stacked.png` & `segretini-matplottini-0.2.5/plots/roofline_stacked.png`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/plots/stem.pdf` & `segretini-matplottini-0.2.5/plots/stem.pdf`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/plots/stem.png` & `segretini-matplottini-0.2.5/plots/stem.png`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/plots/timeseries.pdf` & `segretini-matplottini-0.2.5/plots/timeseries.pdf`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/plots/timeseries.png` & `segretini-matplottini-0.2.5/plots/timeseries.png`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/pyproject.toml` & `segretini-matplottini-0.2.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
-version = "0.2.4"
+version = "0.2.5"
 name = "segretini-matplottini"
 description = "Colorful recipes and utilities for Matplolib and Seaborn, to create publication-ready plots"
 authors = [{name = "Alberto Parravicini", email = "alberto.parravicini@polimi.it"}]
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">= 3.9"
 dependencies = [
```

### Comparing `segretini-matplottini-0.2.4/segretini_matplottini/plot/__init__.py` & `segretini-matplottini-0.2.5/segretini_matplottini/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/segretini_matplottini/plot/barplot.py` & `segretini-matplottini-0.2.5/segretini_matplottini/plot/barplot.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/segretini_matplottini/plot/binary_classification.py` & `segretini-matplottini-0.2.5/segretini_matplottini/plot/binary_classification.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/segretini_matplottini/plot/correlation_scatterplot.py` & `segretini-matplottini-0.2.5/segretini_matplottini/plot/correlation_scatterplot.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/segretini_matplottini/plot/ridgeplot.py` & `segretini-matplottini-0.2.5/segretini_matplottini/plot/ridgeplot.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/segretini_matplottini/plot/roofline.py` & `segretini-matplottini-0.2.5/segretini_matplottini/plot/roofline.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/segretini_matplottini/plot/timeseries.py` & `segretini-matplottini-0.2.5/segretini_matplottini/plot/timeseries.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/segretini_matplottini/utils/__init__.py` & `segretini-matplottini-0.2.5/segretini_matplottini/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/segretini_matplottini/utils/colors.py` & `segretini-matplottini-0.2.5/segretini_matplottini/utils/colors.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/segretini_matplottini/utils/data.py` & `segretini-matplottini-0.2.5/segretini_matplottini/utils/data.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/segretini_matplottini/utils/legend.py` & `segretini-matplottini-0.2.5/segretini_matplottini/utils/legend.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/segretini_matplottini/utils/plot.py` & `segretini-matplottini-0.2.5/segretini_matplottini/utils/plot.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/segretini_matplottini.egg-info/PKG-INFO` & `segretini-matplottini-0.2.5/segretini_matplottini.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segretini-matplottini
-Version: 0.2.4
+Version: 0.2.5
 Summary: Colorful recipes and utilities for Matplolib and Seaborn, to create publication-ready plots
 Author-email: Alberto Parravicini <alberto.parravicini@polimi.it>
 License: MIT License
         
         Copyright (c) 2020-2023 Alberto Parravicini
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `segretini-matplottini-0.2.4/segretini_matplottini.egg-info/SOURCES.txt` & `segretini-matplottini-0.2.5/segretini_matplottini.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/tests/plot/test_barplot.py` & `segretini-matplottini-0.2.5/tests/plot/test_barplot.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/tests/plot/test_binary_classification.py` & `segretini-matplottini-0.2.5/tests/plot/test_binary_classification.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/tests/plot/test_correlation_scatterplot.py` & `segretini-matplottini-0.2.5/tests/plot/test_correlation_scatterplot.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/tests/plot/test_ridgeplot.py` & `segretini-matplottini-0.2.5/tests/plot/test_ridgeplot.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/tests/plot/test_roofline.py` & `segretini-matplottini-0.2.5/tests/plot/test_roofline.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/tests/plot/test_timeseries.py` & `segretini-matplottini-0.2.5/tests/plot/test_timeseries.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/tests/plot/utils.py` & `segretini-matplottini-0.2.5/tests/plot/utils.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/tests/utils/test_colors.py` & `segretini-matplottini-0.2.5/tests/utils/test_colors.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.4/tests/utils/test_data.py` & `segretini-matplottini-0.2.5/tests/utils/test_data.py`

 * *Files identical despite different names*

