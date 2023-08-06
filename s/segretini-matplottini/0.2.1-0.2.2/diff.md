# Comparing `tmp/segretini-matplottini-0.2.1.tar.gz` & `tmp/segretini-matplottini-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "segretini-matplottini-0.2.1.tar", last modified: Sun Aug  6 13:34:16 2023, max compression
+gzip compressed data, was "segretini-matplottini-0.2.2.tar", last modified: Sun Aug  6 14:38:26 2023, max compression
```

## Comparing `segretini-matplottini-0.2.1.tar` & `segretini-matplottini-0.2.2.tar`

### file list

```diff
@@ -1,118 +1,119 @@
-drwxr-xr-x   0 albertoparravicini   (501) staff       (20)        0 2023-08-06 13:34:16.849855 segretini-matplottini-0.2.1/
-drwxr-xr-x   0 albertoparravicini   (501) staff       (20)        0 2023-08-06 13:34:16.797140 segretini-matplottini-0.2.1/.github/
-drwxr-xr-x   0 albertoparravicini   (501) staff       (20)        0 2023-08-06 13:34:16.803732 segretini-matplottini-0.2.1/.github/workflows/
--rw-r--r--   0 albertoparravicini   (501) staff       (20)      840 2023-07-31 19:28:52.000000 segretini-matplottini-0.2.1/.github/workflows/pull_request.yaml
--rw-r--r--   0 albertoparravicini   (501) staff       (20)      747 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/.gitignore
--rw-r--r--   0 albertoparravicini   (501) staff       (20)      587 2023-07-30 13:13:31.000000 segretini-matplottini-0.2.1/.pre-commit-config.yaml
-drwxr-xr-x   0 albertoparravicini   (501) staff       (20)        0 2023-08-06 13:34:16.804627 segretini-matplottini-0.2.1/.vscode/
--rw-r--r--   0 albertoparravicini   (501) staff       (20)      757 2023-07-22 17:05:31.000000 segretini-matplottini-0.2.1/.vscode/launch.json
--rw-r--r--   0 albertoparravicini   (501) staff       (20)      127 2023-07-23 17:29:43.000000 segretini-matplottini-0.2.1/.vscode/settings.json
--rw-r--r--   0 albertoparravicini   (501) staff       (20)     5524 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/CHANGELOG.md
--rw-r--r--   0 albertoparravicini   (501) staff       (20)     1081 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/LICENSE
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    11501 2023-08-06 13:34:16.849507 segretini-matplottini-0.2.1/PKG-INFO
--rw-r--r--   0 albertoparravicini   (501) staff       (20)     9879 2023-08-06 13:07:18.000000 segretini-matplottini-0.2.1/README.md
-drwxr-xr-x   0 albertoparravicini   (501) staff       (20)        0 2023-08-06 13:34:16.807771 segretini-matplottini-0.2.1/data/
--rw-r--r--   0 albertoparravicini   (501) staff       (20)      261 2023-07-27 18:15:28.000000 segretini-matplottini-0.2.1/data/barplot_data.csv
--rw-r--r--   0 albertoparravicini   (501) staff       (20)      340 2023-07-26 19:41:10.000000 segretini-matplottini-0.2.1/data/barplot_for_multiple_categories_data.csv
--rw-r--r--   0 albertoparravicini   (501) staff       (20)     2675 2022-02-03 08:13:39.000000 segretini-matplottini-0.2.1/data/correlation_scatterplot_data.csv
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    25669 2022-10-16 07:30:14.000000 segretini-matplottini-0.2.1/data/density_data.csv
-drwxr-xr-x   0 albertoparravicini   (501) staff       (20)        0 2023-08-06 13:34:16.797531 segretini-matplottini-0.2.1/data/notebooks/
-drwxr-xr-x   0 albertoparravicini   (501) staff       (20)        0 2023-08-06 13:34:16.808925 segretini-matplottini-0.2.1/data/notebooks/1_getting_started_with_barplots/
--rw-r--r--   0 albertoparravicini   (501) staff       (20)      277 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/data/notebooks/1_getting_started_with_barplots/barplot_data.csv
--rw-r--r--   0 albertoparravicini   (501) staff       (20)     1625 2022-02-03 08:13:39.000000 segretini-matplottini-0.2.1/data/performance_scaling_data.csv
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    60208 2022-02-03 08:13:39.000000 segretini-matplottini-0.2.1/data/ridgeplot_data.csv
--rw-r--r--   0 albertoparravicini   (501) staff       (20)   134509 2022-09-26 19:50:14.000000 segretini-matplottini-0.2.1/data/timeseries_data.csv
-drwxr-xr-x   0 albertoparravicini   (501) staff       (20)        0 2023-08-06 13:34:16.810795 segretini-matplottini-0.2.1/examples/
--rw-r--r--   0 albertoparravicini   (501) staff       (20)        0 2023-08-06 12:37:32.000000 segretini-matplottini-0.2.1/examples/__init__.py
--rw-r--r--   0 albertoparravicini   (501) staff       (20)     4135 2023-08-06 12:37:32.000000 segretini-matplottini-0.2.1/examples/plot_barplot.py
--rw-r--r--   0 albertoparravicini   (501) staff       (20)     2680 2023-08-06 12:37:32.000000 segretini-matplottini-0.2.1/examples/plot_binary_classification.py
--rw-r--r--   0 albertoparravicini   (501) staff       (20)     1962 2023-08-06 12:37:32.000000 segretini-matplottini-0.2.1/examples/plot_correlation_scatterplot.py
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    10527 2023-08-06 12:37:32.000000 segretini-matplottini-0.2.1/examples/plot_grid.py
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    10487 2023-08-06 12:37:32.000000 segretini-matplottini-0.2.1/examples/plot_performance_scaling.py
--rw-r--r--   0 albertoparravicini   (501) staff       (20)     2853 2023-08-06 12:37:32.000000 segretini-matplottini-0.2.1/examples/plot_ridgeplot.py
--rw-r--r--   0 albertoparravicini   (501) staff       (20)     6240 2023-08-06 12:37:32.000000 segretini-matplottini-0.2.1/examples/plot_roofline.py
--rw-r--r--   0 albertoparravicini   (501) staff       (20)     2765 2023-08-06 12:37:32.000000 segretini-matplottini-0.2.1/examples/plot_timeseries.py
--rw-r--r--   0 albertoparravicini   (501) staff       (20)      615 2023-07-30 13:13:31.000000 segretini-matplottini-0.2.1/mypy.ini
-drwxr-xr-x   0 albertoparravicini   (501) staff       (20)        0 2023-08-06 13:34:16.810975 segretini-matplottini-0.2.1/notebooks/
--rw-r--r--   0 albertoparravicini   (501) staff       (20)   103687 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/notebooks/1_getting_started_with_barplots.ipynb
-drwxr-xr-x   0 albertoparravicini   (501) staff       (20)        0 2023-08-06 13:34:16.834477 segretini-matplottini-0.2.1/plots/
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    11274 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/plots/barplot.pdf
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    34869 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/plots/barplot.png
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    15571 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/plots/barplot_for_multiple_categories.pdf
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    60298 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/plots/barplot_for_multiple_categories.png
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    15273 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/plots/barplots.pdf
--rw-r--r--   0 albertoparravicini   (501) staff       (20)   108326 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/plots/barplots.png
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    38357 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/plots/binary_classification.pdf
--rw-r--r--   0 albertoparravicini   (501) staff       (20)   228919 2023-08-06 12:03:23.000000 segretini-matplottini-0.2.1/plots/binary_classification.png
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    33890 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/plots/correlation_scatterplot.pdf
--rw-r--r--   0 albertoparravicini   (501) staff       (20)   206682 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/plots/correlation_scatterplot.png
--rw-r--r--   0 albertoparravicini   (501) staff       (20)   849171 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/plots/grid.pdf
--rw-r--r--   0 albertoparravicini   (501) staff       (20)   964425 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/plots/grid.png
--rw-r--r--   0 albertoparravicini   (501) staff       (20)   784156 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/plots/grid_2.pdf
--rw-r--r--   0 albertoparravicini   (501) staff       (20)   903087 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/plots/grid_2.png
-drwxr-xr-x   0 albertoparravicini   (501) staff       (20)        0 2023-08-06 13:34:16.797969 segretini-matplottini-0.2.1/plots/notebooks/
-drwxr-xr-x   0 albertoparravicini   (501) staff       (20)        0 2023-08-06 13:34:16.837716 segretini-matplottini-0.2.1/plots/notebooks/1_getting_started_with_barplots/
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    74133 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/plots/notebooks/1_getting_started_with_barplots/a_much_better_barplot.png
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    15661 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/plots/notebooks/1_getting_started_with_barplots/our_amazing_barplot.pdf
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    54750 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/plots/notebooks/1_getting_started_with_barplots/our_amazing_barplot.png
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    16746 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/plots/notebooks/1_getting_started_with_barplots/our_amazing_barplot_v2.pdf
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    56901 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/plots/notebooks/1_getting_started_with_barplots/our_amazing_barplot_v2.png
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    16615 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/plots/notebooks/1_getting_started_with_barplots/our_amazing_barplot_v3.pdf
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    53406 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/plots/notebooks/1_getting_started_with_barplots/our_amazing_barplot_v3.png
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    19563 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/plots/notebooks/1_getting_started_with_barplots/the_ugliest_barplot.png
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    30521 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/plots/performance_scaling.pdf
--rw-r--r--   0 albertoparravicini   (501) staff       (20)   264083 2023-08-06 12:03:35.000000 segretini-matplottini-0.2.1/plots/performance_scaling.png
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    96597 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/plots/ridgeplot_compact.pdf
--rw-r--r--   0 albertoparravicini   (501) staff       (20)   403977 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/plots/ridgeplot_compact.png
--rw-r--r--   0 albertoparravicini   (501) staff       (20)   100120 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/plots/ridgeplot_large.pdf
--rw-r--r--   0 albertoparravicini   (501) staff       (20)   582502 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/plots/ridgeplot_large.png
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    16056 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/plots/roofline.pdf
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    78276 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/plots/roofline.png
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    20642 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/plots/roofline_double.pdf
--rw-r--r--   0 albertoparravicini   (501) staff       (20)   215335 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/plots/roofline_double.png
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    18219 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/plots/roofline_stacked.pdf
--rw-r--r--   0 albertoparravicini   (501) staff       (20)   175021 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/plots/roofline_stacked.png
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    19875 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/plots/stem.pdf
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    83115 2023-08-06 12:03:52.000000 segretini-matplottini-0.2.1/plots/stem.png
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    29257 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/plots/timeseries.pdf
--rw-r--r--   0 albertoparravicini   (501) staff       (20)   279591 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/plots/timeseries.png
--rw-r--r--   0 albertoparravicini   (501) staff       (20)      932 2023-08-06 13:33:18.000000 segretini-matplottini-0.2.1/pyproject.toml
--rw-r--r--   0 albertoparravicini   (501) staff       (20)      445 2023-07-24 13:11:18.000000 segretini-matplottini-0.2.1/ruff.toml
-drwxr-xr-x   0 albertoparravicini   (501) staff       (20)        0 2023-08-06 13:34:16.838083 segretini-matplottini-0.2.1/segretini_matplottini/
--rw-r--r--   0 albertoparravicini   (501) staff       (20)        0 2023-07-22 19:06:31.000000 segretini-matplottini-0.2.1/segretini_matplottini/__init__.py
-drwxr-xr-x   0 albertoparravicini   (501) staff       (20)        0 2023-08-06 13:34:16.843743 segretini-matplottini-0.2.1/segretini_matplottini/plot/
--rw-r--r--   0 albertoparravicini   (501) staff       (20)      744 2023-07-29 16:04:44.000000 segretini-matplottini-0.2.1/segretini_matplottini/plot/__init__.py
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    24737 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/segretini_matplottini/plot/barplot.py
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    51366 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/segretini_matplottini/plot/binary_classification.py
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    10544 2023-07-31 19:29:13.000000 segretini-matplottini-0.2.1/segretini_matplottini/plot/correlation_scatterplot.py
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    25419 2023-07-31 19:28:52.000000 segretini-matplottini-0.2.1/segretini_matplottini/plot/ridgeplot.py
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    13206 2023-07-31 19:41:05.000000 segretini-matplottini-0.2.1/segretini_matplottini/plot/roofline.py
--rw-r--r--   0 albertoparravicini   (501) staff       (20)     9102 2023-07-31 19:28:52.000000 segretini-matplottini-0.2.1/segretini_matplottini/plot/timeseries.py
--rw-r--r--   0 albertoparravicini   (501) staff       (20)        0 2023-07-20 14:13:02.000000 segretini-matplottini-0.2.1/segretini_matplottini/py.typed
-drwxr-xr-x   0 albertoparravicini   (501) staff       (20)        0 2023-08-06 13:34:16.845256 segretini-matplottini-0.2.1/segretini_matplottini/utils/
--rw-r--r--   0 albertoparravicini   (501) staff       (20)     1146 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/segretini_matplottini/utils/__init__.py
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    17140 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/segretini_matplottini/utils/colors.py
--rw-r--r--   0 albertoparravicini   (501) staff       (20)       40 2023-07-25 09:51:34.000000 segretini-matplottini-0.2.1/segretini_matplottini/utils/constants.py
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    18079 2023-07-31 19:28:52.000000 segretini-matplottini-0.2.1/segretini_matplottini/utils/data.py
--rwxr-xr-x   0 albertoparravicini   (501) staff       (20)     4813 2023-07-24 12:56:17.000000 segretini-matplottini-0.2.1/segretini_matplottini/utils/legend.py
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    23306 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/segretini_matplottini/utils/plot.py
-drwxr-xr-x   0 albertoparravicini   (501) staff       (20)        0 2023-08-06 13:34:16.838865 segretini-matplottini-0.2.1/segretini_matplottini.egg-info/
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    11501 2023-08-06 13:34:16.000000 segretini-matplottini-0.2.1/segretini_matplottini.egg-info/PKG-INFO
--rw-r--r--   0 albertoparravicini   (501) staff       (20)     3208 2023-08-06 13:34:16.000000 segretini-matplottini-0.2.1/segretini_matplottini.egg-info/SOURCES.txt
--rw-r--r--   0 albertoparravicini   (501) staff       (20)        1 2023-08-06 13:34:16.000000 segretini-matplottini-0.2.1/segretini_matplottini.egg-info/dependency_links.txt
--rw-r--r--   0 albertoparravicini   (501) staff       (20)      216 2023-08-06 13:34:16.000000 segretini-matplottini-0.2.1/segretini_matplottini.egg-info/requires.txt
--rw-r--r--   0 albertoparravicini   (501) staff       (20)       22 2023-08-06 13:34:16.000000 segretini-matplottini-0.2.1/segretini_matplottini.egg-info/top_level.txt
--rw-r--r--   0 albertoparravicini   (501) staff       (20)       38 2023-08-06 13:34:16.849928 segretini-matplottini-0.2.1/setup.cfg
-drwxr-xr-x   0 albertoparravicini   (501) staff       (20)        0 2023-08-06 13:34:16.798699 segretini-matplottini-0.2.1/tests/
-drwxr-xr-x   0 albertoparravicini   (501) staff       (20)        0 2023-08-06 13:34:16.848607 segretini-matplottini-0.2.1/tests/plot/
--rw-r--r--   0 albertoparravicini   (501) staff       (20)        0 2023-07-25 11:55:13.000000 segretini-matplottini-0.2.1/tests/plot/__init__.py
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    11053 2023-07-27 16:39:26.000000 segretini-matplottini-0.2.1/tests/plot/test_barplot.py
--rw-r--r--   0 albertoparravicini   (501) staff       (20)     4991 2023-07-29 16:04:44.000000 segretini-matplottini-0.2.1/tests/plot/test_binary_classification.py
--rw-r--r--   0 albertoparravicini   (501) staff       (20)     1949 2023-07-31 19:28:52.000000 segretini-matplottini-0.2.1/tests/plot/test_correlation_scatterplot.py
--rw-r--r--   0 albertoparravicini   (501) staff       (20)     3579 2023-07-31 19:28:52.000000 segretini-matplottini-0.2.1/tests/plot/test_ridgeplot.py
--rw-r--r--   0 albertoparravicini   (501) staff       (20)     3877 2023-07-31 19:28:52.000000 segretini-matplottini-0.2.1/tests/plot/test_roofline.py
--rw-r--r--   0 albertoparravicini   (501) staff       (20)     1899 2023-07-26 14:29:48.000000 segretini-matplottini-0.2.1/tests/plot/test_timeseries.py
--rw-r--r--   0 albertoparravicini   (501) staff       (20)     1010 2023-07-25 12:01:20.000000 segretini-matplottini-0.2.1/tests/plot/utils.py
-drwxr-xr-x   0 albertoparravicini   (501) staff       (20)        0 2023-08-06 13:34:16.849062 segretini-matplottini-0.2.1/tests/utils/
--rw-r--r--   0 albertoparravicini   (501) staff       (20)     4222 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/tests/utils/test_colors.py
--rw-r--r--   0 albertoparravicini   (501) staff       (20)     2404 2023-07-28 09:21:40.000000 segretini-matplottini-0.2.1/tests/utils/test_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:38:26.361482 segretini-matplottini-0.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:38:26.325482 segretini-matplottini-0.2.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:38:26.329482 segretini-matplottini-0.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/.github/workflows/pull_request.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/.github/workflows/pypi_release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:38:26.333482 segretini-matplottini-0.2.2/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5524 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12102 2023-08-06 14:38:26.361482 segretini-matplottini-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10480 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:38:26.333482 segretini-matplottini-0.2.2/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/data/barplot_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/data/barplot_for_multiple_categories_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/data/correlation_scatterplot_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    25669 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/data/density_data.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:38:26.325482 segretini-matplottini-0.2.2/data/notebooks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:38:26.333482 segretini-matplottini-0.2.2/data/notebooks/1_getting_started_with_barplots/
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/data/notebooks/1_getting_started_with_barplots/barplot_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/data/performance_scaling_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    60208 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/data/ridgeplot_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   134509 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/data/timeseries_data.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:38:26.333482 segretini-matplottini-0.2.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/examples/plot_barplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/examples/plot_binary_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/examples/plot_correlation_scatterplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10527 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/examples/plot_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10487 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/examples/plot_performance_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/examples/plot_ridgeplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6240 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/examples/plot_roofline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/examples/plot_timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/mypy.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:38:26.333482 segretini-matplottini-0.2.2/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)   103687 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/notebooks/1_getting_started_with_barplots.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:38:26.349482 segretini-matplottini-0.2.2/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)    11274 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/plots/barplot.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    34869 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/plots/barplot.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15571 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/plots/barplot_for_multiple_categories.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    60298 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/plots/barplot_for_multiple_categories.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15273 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/plots/barplots.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)   108326 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/plots/barplots.png
+-rw-r--r--   0 runner    (1001) docker     (123)    38357 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/plots/binary_classification.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)   228919 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/plots/binary_classification.png
+-rw-r--r--   0 runner    (1001) docker     (123)    33890 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/plots/correlation_scatterplot.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)   206682 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/plots/correlation_scatterplot.png
+-rw-r--r--   0 runner    (1001) docker     (123)   849171 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/plots/grid.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)   964425 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/plots/grid.png
+-rw-r--r--   0 runner    (1001) docker     (123)   784156 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/plots/grid_2.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)   903087 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/plots/grid_2.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:38:26.329482 segretini-matplottini-0.2.2/plots/notebooks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:38:26.349482 segretini-matplottini-0.2.2/plots/notebooks/1_getting_started_with_barplots/
+-rw-r--r--   0 runner    (1001) docker     (123)    74133 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/plots/notebooks/1_getting_started_with_barplots/a_much_better_barplot.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15661 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/plots/notebooks/1_getting_started_with_barplots/our_amazing_barplot.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    54750 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/plots/notebooks/1_getting_started_with_barplots/our_amazing_barplot.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16746 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/plots/notebooks/1_getting_started_with_barplots/our_amazing_barplot_v2.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    56901 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/plots/notebooks/1_getting_started_with_barplots/our_amazing_barplot_v2.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16615 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/plots/notebooks/1_getting_started_with_barplots/our_amazing_barplot_v3.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    53406 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/plots/notebooks/1_getting_started_with_barplots/our_amazing_barplot_v3.png
+-rw-r--r--   0 runner    (1001) docker     (123)    19563 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/plots/notebooks/1_getting_started_with_barplots/the_ugliest_barplot.png
+-rw-r--r--   0 runner    (1001) docker     (123)    30521 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/plots/performance_scaling.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)   264083 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/plots/performance_scaling.png
+-rw-r--r--   0 runner    (1001) docker     (123)    96597 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/plots/ridgeplot_compact.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)   403977 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/plots/ridgeplot_compact.png
+-rw-r--r--   0 runner    (1001) docker     (123)   100120 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/plots/ridgeplot_large.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)   582502 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/plots/ridgeplot_large.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16056 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/plots/roofline.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    78276 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/plots/roofline.png
+-rw-r--r--   0 runner    (1001) docker     (123)    20642 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/plots/roofline_double.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)   215335 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/plots/roofline_double.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18219 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/plots/roofline_stacked.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)   175021 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/plots/roofline_stacked.png
+-rw-r--r--   0 runner    (1001) docker     (123)    19875 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/plots/stem.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    83115 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/plots/stem.png
+-rw-r--r--   0 runner    (1001) docker     (123)    29257 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/plots/timeseries.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)   279591 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/plots/timeseries.png
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/ruff.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:38:26.353482 segretini-matplottini-0.2.2/segretini_matplottini/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/segretini_matplottini/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:38:26.353482 segretini-matplottini-0.2.2/segretini_matplottini/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/segretini_matplottini/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24737 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/segretini_matplottini/plot/barplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51366 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/segretini_matplottini/plot/binary_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10544 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/segretini_matplottini/plot/correlation_scatterplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25419 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/segretini_matplottini/plot/ridgeplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13206 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/segretini_matplottini/plot/roofline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9102 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/segretini_matplottini/plot/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/segretini_matplottini/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:38:26.357482 segretini-matplottini-0.2.2/segretini_matplottini/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/segretini_matplottini/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17140 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/segretini_matplottini/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/segretini_matplottini/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18079 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/segretini_matplottini/utils/data.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4813 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/segretini_matplottini/utils/legend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23306 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/segretini_matplottini/utils/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:38:26.353482 segretini-matplottini-0.2.2/segretini_matplottini.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12102 2023-08-06 14:38:26.000000 segretini-matplottini-0.2.2/segretini_matplottini.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-08-06 14:38:26.000000 segretini-matplottini-0.2.2/segretini_matplottini.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 14:38:26.000000 segretini-matplottini-0.2.2/segretini_matplottini.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-08-06 14:38:26.000000 segretini-matplottini-0.2.2/segretini_matplottini.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-06 14:38:26.000000 segretini-matplottini-0.2.2/segretini_matplottini.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 14:38:26.361482 segretini-matplottini-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:38:26.329482 segretini-matplottini-0.2.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:38:26.357482 segretini-matplottini-0.2.2/tests/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/tests/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11053 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/tests/plot/test_barplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/tests/plot/test_binary_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/tests/plot/test_correlation_scatterplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/tests/plot/test_ridgeplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/tests/plot/test_roofline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/tests/plot/test_timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/tests/plot/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:38:26.357482 segretini-matplottini-0.2.2/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/tests/utils/test_colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-08-06 14:37:27.000000 segretini-matplottini-0.2.2/tests/utils/test_data.py
```

### Comparing `segretini-matplottini-0.2.1/.github/workflows/pull_request.yaml` & `segretini-matplottini-0.2.2/.github/workflows/pull_request.yaml`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/.gitignore` & `segretini-matplottini-0.2.2/.gitignore`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Add back specific files
 !*.py
 !pyproject.toml
 !.gitignore
 !.pre-commit-config.yaml
 !.github/
 !.github/workflows/
-!.github/workflows/pull_request.yaml
+!.github/workflows/*.yaml
 !ruff.toml
 !mypy.ini
 !README.md
 !CHANGELOG.md
 !LICENSE
 !segretini_matplottini
 !segretini_matplottini/py.typed
```

### Comparing `segretini-matplottini-0.2.1/.pre-commit-config.yaml` & `segretini-matplottini-0.2.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/.vscode/launch.json` & `segretini-matplottini-0.2.2/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/CHANGELOG.md` & `segretini-matplottini-0.2.2/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/LICENSE` & `segretini-matplottini-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/PKG-INFO` & `segretini-matplottini-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segretini-matplottini
-Version: 0.2.1
+Version: 0.2.2
 Summary: Colorful recipes and utilities for Matplolib and Seaborn, to create publication-ready plots
 Author-email: Alberto Parravicini <alberto.parravicini@polimi.it>
 License: MIT License
         
         Copyright (c) 2020-2023 Alberto Parravicini
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -44,14 +44,18 @@
 
 What do you want do to with `segretini-matplottini`? Pick the installation that suits you best.
 
 ### I want to use `segretini-matplottini` as a package in my projects
 
 Install `segretini-matplottini` with `pip`.
 
+```shell
+pip install segretini-matplottini
+```
+
 ### I want to run the examples
 
 Clone the repository and install `segretini-matplottini` with `pip`. You might want to do so in a dedicated `conda` environment.
 
 ```shell
 git clone https://github.com/AlbertoParravicini/segretini-matplottini.git
 cd segretini-matplottini
@@ -84,35 +88,42 @@
     │       ├── constants.py  -> Default values for shared settings (font size, DPI, etc.)
     │       ├── colors.py     -> List of predefined and pretty colors, plus color-related utilities
     │       ├── data.py       -> Utilities to preprocess datasets (e.g. outlier removal)
     │       ├── legend.py     -> Legend-related utilities (e.g. custom legend styles)
     │       └── plot.py       -> General utilities for plotting (e.g. adding labels, saving plots)
     ├── data         -> Sample data used in example plots
     ├── examples     -> Recipes to create fancy plots
+    ├── notebooks    -> Jupyter notebooks and tutorials
     ├── plots        -> Plots generated by examples. If you find something cool, check the code in examples
     ├── tests        -> Unit tests and end-to-end tests for plotting functions
     ├── CHANGELOG.md -> List of updates to the codebase. Check here to see what's new
     ├── README.md   -> This file!
     └── (...)       -> Configuration files for linters, and other setup files.
 ```
 
 ## 🌞 Getting started
 
 The best way to get started is to check out the [`plots`](plots/) folder, to find plots generated with `segretini-matplottini`.
 If you find a plot you like, you can find the code to generate it in the [`examples`](examples/) folder.
 
-### Some plots available in `segretini-matplottini`
+### 📚 Notebooks 
+
+If you do not know where to start from, and you do not have a lot of experience with Matplotlib and Seaborn, check out the [`notebooks`](notebooks/) folder.
+
+* `1_getting_started_with_barplots.ipynb` provides an introduction to Matplotlib and Seaborn, and guides the reader into creating a beautiful barplot. You will learn principles that lie behind any great visualization, and the basic concepts of Matplotlib and Seaborn.
+
+### 🖼️ Some plots available in `segretini-matplottini`
 
 This is a non-inclusive list of custom plots that are available out-of-the-box in `segretini-matplottini`.
 * `correlation_scatterplot` visualizes the relation between two variables, combining a scatterplot, a 2D density plot, and a linear regression with confidence intervals. Learn more with [this](examples/plot_correlation_scatterplot.py) example. 
 * `ridgeplot` shows the distribution of two variables, grouped by the specified factor. For example, one can visualize the latency of two implementations of the same algorithm, across multiple runs of different datasets. Learn more with [this](examples/plot_ridgeplot.py) example. 
 * `roofline` plots the [Roofline model](https://en.wikipedia.org/wiki/Roofline_model) for the input operational intensity and performance values. Learn more with [this](examples/plot_roofline.py) example. 
 * `binary_classfication` summarizes the performance of a binary classifier, plotting curves such as ROC, Precision-Recall, and F1 score for different classification thresholds. Learn more with [this](examples/plot_binary_classification.py) example.
 
-### Some utilities available in `segretini-matplottini`
+### 🧪 Some utilities available in `segretini-matplottini`
 
 The astute reader might say "Hey, I don't need any of those plots, why should I care about `segretini-matplottini`?".
 There's a lot more than plotting functions! The `utils` can be applied to any Matplotlib plot, to simplify your life when it comes to creating complex visualizations.
 * [`data`](segretini_matplottini/utils/data.py) contains functions to preprocess your experiment results by [removing outliers](https://github.com/AlbertoParravicini/segretini-matplottini/blob/master/segretini_matplottini/utils/data.py#L158) and computing the [relative performance](https://github.com/AlbertoParravicini/segretini-matplottini/blob/master/segretini_matplottini/utils/data.py#L242) from absolute performance numbers.
 * [`colors`](segretini_matplottini/utils/colors.py) provides utilities to convert your palettes to [grayscale](https://github.com/AlbertoParravicini/segretini-matplottini/blob/master/segretini_matplottini/utils/colors.py#L48) to check how your plot will look when printed in black-and-white or when seen by a color deficient person, and to simplify the [creation of palettes](https://github.com/AlbertoParravicini/segretini-matplottini/blob/master/segretini_matplottini/utils/colors.py#L61) given the start and end colors. It also has plenty of beautiful colors to choose from, validated for black and white printing and color blindness.
 * [`plot`](segretini_matplottini/utils/plot.py) is the source for general plotting utilities, from [computing](https://github.com/AlbertoParravicini/segretini-matplottini/blob/master/segretini_matplottini/utils/plot.py#L323) and [adding](https://github.com/AlbertoParravicini/segretini-matplottini/blob/master/segretini_matplottini/utils/plot.py#L390) labels to barplots to [saving plots](https://github.com/AlbertoParravicini/segretini-matplottini/blob/master/segretini_matplottini/utils/plot.py#L461) with a standardized structure, so they won't get lost or overwritten by accident.
 
@@ -143,14 +154,15 @@
 
 ### Building and releasing
 
 To build a new version of `segretini-matplottini`, run the following command. Make sure that you have `dev` dependencies installed.
 
 ```shell
 python -m build
+python -m twine upload dist/*
 ```
 
 ## 💡 Tips and Tricks
 
 An ever-growing collection of tips I've found or discovered along the way, together with some nice resources I like a lot.
 
 ### 📚 Resources
```

### Comparing `segretini-matplottini-0.2.1/README.md` & `segretini-matplottini-0.2.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,18 @@
 
 What do you want do to with `segretini-matplottini`? Pick the installation that suits you best.
 
 ### I want to use `segretini-matplottini` as a package in my projects
 
 Install `segretini-matplottini` with `pip`.
 
+```shell
+pip install segretini-matplottini
+```
+
 ### I want to run the examples
 
 Clone the repository and install `segretini-matplottini` with `pip`. You might want to do so in a dedicated `conda` environment.
 
 ```shell
 git clone https://github.com/AlbertoParravicini/segretini-matplottini.git
 cd segretini-matplottini
@@ -51,35 +55,42 @@
     │       ├── constants.py  -> Default values for shared settings (font size, DPI, etc.)
     │       ├── colors.py     -> List of predefined and pretty colors, plus color-related utilities
     │       ├── data.py       -> Utilities to preprocess datasets (e.g. outlier removal)
     │       ├── legend.py     -> Legend-related utilities (e.g. custom legend styles)
     │       └── plot.py       -> General utilities for plotting (e.g. adding labels, saving plots)
     ├── data         -> Sample data used in example plots
     ├── examples     -> Recipes to create fancy plots
+    ├── notebooks    -> Jupyter notebooks and tutorials
     ├── plots        -> Plots generated by examples. If you find something cool, check the code in examples
     ├── tests        -> Unit tests and end-to-end tests for plotting functions
     ├── CHANGELOG.md -> List of updates to the codebase. Check here to see what's new
     ├── README.md   -> This file!
     └── (...)       -> Configuration files for linters, and other setup files.
 ```
 
 ## 🌞 Getting started
 
 The best way to get started is to check out the [`plots`](plots/) folder, to find plots generated with `segretini-matplottini`.
 If you find a plot you like, you can find the code to generate it in the [`examples`](examples/) folder.
 
-### Some plots available in `segretini-matplottini`
+### 📚 Notebooks 
+
+If you do not know where to start from, and you do not have a lot of experience with Matplotlib and Seaborn, check out the [`notebooks`](notebooks/) folder.
+
+* `1_getting_started_with_barplots.ipynb` provides an introduction to Matplotlib and Seaborn, and guides the reader into creating a beautiful barplot. You will learn principles that lie behind any great visualization, and the basic concepts of Matplotlib and Seaborn.
+
+### 🖼️ Some plots available in `segretini-matplottini`
 
 This is a non-inclusive list of custom plots that are available out-of-the-box in `segretini-matplottini`.
 * `correlation_scatterplot` visualizes the relation between two variables, combining a scatterplot, a 2D density plot, and a linear regression with confidence intervals. Learn more with [this](examples/plot_correlation_scatterplot.py) example. 
 * `ridgeplot` shows the distribution of two variables, grouped by the specified factor. For example, one can visualize the latency of two implementations of the same algorithm, across multiple runs of different datasets. Learn more with [this](examples/plot_ridgeplot.py) example. 
 * `roofline` plots the [Roofline model](https://en.wikipedia.org/wiki/Roofline_model) for the input operational intensity and performance values. Learn more with [this](examples/plot_roofline.py) example. 
 * `binary_classfication` summarizes the performance of a binary classifier, plotting curves such as ROC, Precision-Recall, and F1 score for different classification thresholds. Learn more with [this](examples/plot_binary_classification.py) example.
 
-### Some utilities available in `segretini-matplottini`
+### 🧪 Some utilities available in `segretini-matplottini`
 
 The astute reader might say "Hey, I don't need any of those plots, why should I care about `segretini-matplottini`?".
 There's a lot more than plotting functions! The `utils` can be applied to any Matplotlib plot, to simplify your life when it comes to creating complex visualizations.
 * [`data`](segretini_matplottini/utils/data.py) contains functions to preprocess your experiment results by [removing outliers](https://github.com/AlbertoParravicini/segretini-matplottini/blob/master/segretini_matplottini/utils/data.py#L158) and computing the [relative performance](https://github.com/AlbertoParravicini/segretini-matplottini/blob/master/segretini_matplottini/utils/data.py#L242) from absolute performance numbers.
 * [`colors`](segretini_matplottini/utils/colors.py) provides utilities to convert your palettes to [grayscale](https://github.com/AlbertoParravicini/segretini-matplottini/blob/master/segretini_matplottini/utils/colors.py#L48) to check how your plot will look when printed in black-and-white or when seen by a color deficient person, and to simplify the [creation of palettes](https://github.com/AlbertoParravicini/segretini-matplottini/blob/master/segretini_matplottini/utils/colors.py#L61) given the start and end colors. It also has plenty of beautiful colors to choose from, validated for black and white printing and color blindness.
 * [`plot`](segretini_matplottini/utils/plot.py) is the source for general plotting utilities, from [computing](https://github.com/AlbertoParravicini/segretini-matplottini/blob/master/segretini_matplottini/utils/plot.py#L323) and [adding](https://github.com/AlbertoParravicini/segretini-matplottini/blob/master/segretini_matplottini/utils/plot.py#L390) labels to barplots to [saving plots](https://github.com/AlbertoParravicini/segretini-matplottini/blob/master/segretini_matplottini/utils/plot.py#L461) with a standardized structure, so they won't get lost or overwritten by accident.
 
@@ -110,14 +121,15 @@
 
 ### Building and releasing
 
 To build a new version of `segretini-matplottini`, run the following command. Make sure that you have `dev` dependencies installed.
 
 ```shell
 python -m build
+python -m twine upload dist/*
 ```
 
 ## 💡 Tips and Tricks
 
 An ever-growing collection of tips I've found or discovered along the way, together with some nice resources I like a lot.
 
 ### 📚 Resources
```

### Comparing `segretini-matplottini-0.2.1/data/correlation_scatterplot_data.csv` & `segretini-matplottini-0.2.2/data/correlation_scatterplot_data.csv`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/data/density_data.csv` & `segretini-matplottini-0.2.2/data/density_data.csv`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/data/performance_scaling_data.csv` & `segretini-matplottini-0.2.2/data/performance_scaling_data.csv`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/data/ridgeplot_data.csv` & `segretini-matplottini-0.2.2/data/ridgeplot_data.csv`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/data/timeseries_data.csv` & `segretini-matplottini-0.2.2/data/timeseries_data.csv`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/examples/plot_barplot.py` & `segretini-matplottini-0.2.2/examples/plot_barplot.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/examples/plot_binary_classification.py` & `segretini-matplottini-0.2.2/examples/plot_binary_classification.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/examples/plot_correlation_scatterplot.py` & `segretini-matplottini-0.2.2/examples/plot_correlation_scatterplot.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/examples/plot_grid.py` & `segretini-matplottini-0.2.2/examples/plot_grid.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/examples/plot_performance_scaling.py` & `segretini-matplottini-0.2.2/examples/plot_performance_scaling.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/examples/plot_ridgeplot.py` & `segretini-matplottini-0.2.2/examples/plot_ridgeplot.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/examples/plot_roofline.py` & `segretini-matplottini-0.2.2/examples/plot_roofline.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/examples/plot_timeseries.py` & `segretini-matplottini-0.2.2/examples/plot_timeseries.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/mypy.ini` & `segretini-matplottini-0.2.2/mypy.ini`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/notebooks/1_getting_started_with_barplots.ipynb` & `segretini-matplottini-0.2.2/notebooks/1_getting_started_with_barplots.ipynb`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/plots/barplot.pdf` & `segretini-matplottini-0.2.2/plots/barplot.pdf`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/plots/barplot.png` & `segretini-matplottini-0.2.2/plots/barplot.png`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/plots/barplot_for_multiple_categories.pdf` & `segretini-matplottini-0.2.2/plots/barplot_for_multiple_categories.pdf`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/plots/barplot_for_multiple_categories.png` & `segretini-matplottini-0.2.2/plots/barplot_for_multiple_categories.png`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/plots/barplots.pdf` & `segretini-matplottini-0.2.2/plots/barplots.pdf`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/plots/barplots.png` & `segretini-matplottini-0.2.2/plots/barplots.png`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/plots/binary_classification.pdf` & `segretini-matplottini-0.2.2/plots/binary_classification.pdf`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/plots/binary_classification.png` & `segretini-matplottini-0.2.2/plots/binary_classification.png`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/plots/correlation_scatterplot.pdf` & `segretini-matplottini-0.2.2/plots/correlation_scatterplot.pdf`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/plots/correlation_scatterplot.png` & `segretini-matplottini-0.2.2/plots/correlation_scatterplot.png`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/plots/grid.pdf` & `segretini-matplottini-0.2.2/plots/grid.pdf`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/plots/grid.png` & `segretini-matplottini-0.2.2/plots/grid.png`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/plots/grid_2.pdf` & `segretini-matplottini-0.2.2/plots/grid_2.pdf`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/plots/grid_2.png` & `segretini-matplottini-0.2.2/plots/grid_2.png`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/plots/notebooks/1_getting_started_with_barplots/a_much_better_barplot.png` & `segretini-matplottini-0.2.2/plots/notebooks/1_getting_started_with_barplots/a_much_better_barplot.png`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/plots/notebooks/1_getting_started_with_barplots/our_amazing_barplot.pdf` & `segretini-matplottini-0.2.2/plots/notebooks/1_getting_started_with_barplots/our_amazing_barplot.pdf`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/plots/notebooks/1_getting_started_with_barplots/our_amazing_barplot.png` & `segretini-matplottini-0.2.2/plots/notebooks/1_getting_started_with_barplots/our_amazing_barplot.png`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/plots/notebooks/1_getting_started_with_barplots/our_amazing_barplot_v2.pdf` & `segretini-matplottini-0.2.2/plots/notebooks/1_getting_started_with_barplots/our_amazing_barplot_v2.pdf`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/plots/notebooks/1_getting_started_with_barplots/our_amazing_barplot_v2.png` & `segretini-matplottini-0.2.2/plots/notebooks/1_getting_started_with_barplots/our_amazing_barplot_v2.png`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/plots/notebooks/1_getting_started_with_barplots/our_amazing_barplot_v3.pdf` & `segretini-matplottini-0.2.2/plots/notebooks/1_getting_started_with_barplots/our_amazing_barplot_v3.pdf`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/plots/notebooks/1_getting_started_with_barplots/our_amazing_barplot_v3.png` & `segretini-matplottini-0.2.2/plots/notebooks/1_getting_started_with_barplots/our_amazing_barplot_v3.png`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/plots/notebooks/1_getting_started_with_barplots/the_ugliest_barplot.png` & `segretini-matplottini-0.2.2/plots/notebooks/1_getting_started_with_barplots/the_ugliest_barplot.png`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/plots/performance_scaling.pdf` & `segretini-matplottini-0.2.2/plots/performance_scaling.pdf`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/plots/performance_scaling.png` & `segretini-matplottini-0.2.2/plots/performance_scaling.png`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/plots/ridgeplot_compact.pdf` & `segretini-matplottini-0.2.2/plots/ridgeplot_compact.pdf`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/plots/ridgeplot_compact.png` & `segretini-matplottini-0.2.2/plots/ridgeplot_compact.png`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/plots/ridgeplot_large.pdf` & `segretini-matplottini-0.2.2/plots/ridgeplot_large.pdf`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/plots/ridgeplot_large.png` & `segretini-matplottini-0.2.2/plots/ridgeplot_large.png`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/plots/roofline.pdf` & `segretini-matplottini-0.2.2/plots/roofline.pdf`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/plots/roofline.png` & `segretini-matplottini-0.2.2/plots/roofline.png`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/plots/roofline_double.pdf` & `segretini-matplottini-0.2.2/plots/roofline_double.pdf`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/plots/roofline_double.png` & `segretini-matplottini-0.2.2/plots/roofline_double.png`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/plots/roofline_stacked.pdf` & `segretini-matplottini-0.2.2/plots/roofline_stacked.pdf`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/plots/roofline_stacked.png` & `segretini-matplottini-0.2.2/plots/roofline_stacked.png`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/plots/stem.pdf` & `segretini-matplottini-0.2.2/plots/stem.pdf`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/plots/stem.png` & `segretini-matplottini-0.2.2/plots/stem.png`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/plots/timeseries.pdf` & `segretini-matplottini-0.2.2/plots/timeseries.pdf`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/plots/timeseries.png` & `segretini-matplottini-0.2.2/plots/timeseries.png`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/pyproject.toml` & `segretini-matplottini-0.2.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
-version = "0.2.1"
+version = "0.2.2"
 name = "segretini-matplottini"
 description = "Colorful recipes and utilities for Matplolib and Seaborn, to create publication-ready plots"
 authors = [{name = "Alberto Parravicini", email = "alberto.parravicini@polimi.it"}]
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">= 3.9"
 dependencies = [
@@ -23,14 +23,15 @@
     "black >= 23.7",
     "isort >= 5.12.0",
     "ruff >= 0.0.280",
     "pre-commit >= 3.3.3",
     "pytest >= 7.4.0",
     "mypy >= 1.4.1",
     "build >= 0.10.0",
+    "twine >= 4.0.2",
 ]
 notebook = [
     "notebook >= 7.0.1",
 ]
 
 [tool.setuptools]
 packages = ["segretini_matplottini"]
```

### Comparing `segretini-matplottini-0.2.1/segretini_matplottini/plot/__init__.py` & `segretini-matplottini-0.2.2/segretini_matplottini/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/segretini_matplottini/plot/barplot.py` & `segretini-matplottini-0.2.2/segretini_matplottini/plot/barplot.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/segretini_matplottini/plot/binary_classification.py` & `segretini-matplottini-0.2.2/segretini_matplottini/plot/binary_classification.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/segretini_matplottini/plot/correlation_scatterplot.py` & `segretini-matplottini-0.2.2/segretini_matplottini/plot/correlation_scatterplot.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/segretini_matplottini/plot/ridgeplot.py` & `segretini-matplottini-0.2.2/segretini_matplottini/plot/ridgeplot.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/segretini_matplottini/plot/roofline.py` & `segretini-matplottini-0.2.2/segretini_matplottini/plot/roofline.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/segretini_matplottini/plot/timeseries.py` & `segretini-matplottini-0.2.2/segretini_matplottini/plot/timeseries.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/segretini_matplottini/utils/__init__.py` & `segretini-matplottini-0.2.2/segretini_matplottini/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/segretini_matplottini/utils/colors.py` & `segretini-matplottini-0.2.2/segretini_matplottini/utils/colors.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/segretini_matplottini/utils/data.py` & `segretini-matplottini-0.2.2/segretini_matplottini/utils/data.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/segretini_matplottini/utils/legend.py` & `segretini-matplottini-0.2.2/segretini_matplottini/utils/legend.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/segretini_matplottini/utils/plot.py` & `segretini-matplottini-0.2.2/segretini_matplottini/utils/plot.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/segretini_matplottini.egg-info/PKG-INFO` & `segretini-matplottini-0.2.2/segretini_matplottini.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segretini-matplottini
-Version: 0.2.1
+Version: 0.2.2
 Summary: Colorful recipes and utilities for Matplolib and Seaborn, to create publication-ready plots
 Author-email: Alberto Parravicini <alberto.parravicini@polimi.it>
 License: MIT License
         
         Copyright (c) 2020-2023 Alberto Parravicini
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -44,14 +44,18 @@
 
 What do you want do to with `segretini-matplottini`? Pick the installation that suits you best.
 
 ### I want to use `segretini-matplottini` as a package in my projects
 
 Install `segretini-matplottini` with `pip`.
 
+```shell
+pip install segretini-matplottini
+```
+
 ### I want to run the examples
 
 Clone the repository and install `segretini-matplottini` with `pip`. You might want to do so in a dedicated `conda` environment.
 
 ```shell
 git clone https://github.com/AlbertoParravicini/segretini-matplottini.git
 cd segretini-matplottini
@@ -84,35 +88,42 @@
     │       ├── constants.py  -> Default values for shared settings (font size, DPI, etc.)
     │       ├── colors.py     -> List of predefined and pretty colors, plus color-related utilities
     │       ├── data.py       -> Utilities to preprocess datasets (e.g. outlier removal)
     │       ├── legend.py     -> Legend-related utilities (e.g. custom legend styles)
     │       └── plot.py       -> General utilities for plotting (e.g. adding labels, saving plots)
     ├── data         -> Sample data used in example plots
     ├── examples     -> Recipes to create fancy plots
+    ├── notebooks    -> Jupyter notebooks and tutorials
     ├── plots        -> Plots generated by examples. If you find something cool, check the code in examples
     ├── tests        -> Unit tests and end-to-end tests for plotting functions
     ├── CHANGELOG.md -> List of updates to the codebase. Check here to see what's new
     ├── README.md   -> This file!
     └── (...)       -> Configuration files for linters, and other setup files.
 ```
 
 ## 🌞 Getting started
 
 The best way to get started is to check out the [`plots`](plots/) folder, to find plots generated with `segretini-matplottini`.
 If you find a plot you like, you can find the code to generate it in the [`examples`](examples/) folder.
 
-### Some plots available in `segretini-matplottini`
+### 📚 Notebooks 
+
+If you do not know where to start from, and you do not have a lot of experience with Matplotlib and Seaborn, check out the [`notebooks`](notebooks/) folder.
+
+* `1_getting_started_with_barplots.ipynb` provides an introduction to Matplotlib and Seaborn, and guides the reader into creating a beautiful barplot. You will learn principles that lie behind any great visualization, and the basic concepts of Matplotlib and Seaborn.
+
+### 🖼️ Some plots available in `segretini-matplottini`
 
 This is a non-inclusive list of custom plots that are available out-of-the-box in `segretini-matplottini`.
 * `correlation_scatterplot` visualizes the relation between two variables, combining a scatterplot, a 2D density plot, and a linear regression with confidence intervals. Learn more with [this](examples/plot_correlation_scatterplot.py) example. 
 * `ridgeplot` shows the distribution of two variables, grouped by the specified factor. For example, one can visualize the latency of two implementations of the same algorithm, across multiple runs of different datasets. Learn more with [this](examples/plot_ridgeplot.py) example. 
 * `roofline` plots the [Roofline model](https://en.wikipedia.org/wiki/Roofline_model) for the input operational intensity and performance values. Learn more with [this](examples/plot_roofline.py) example. 
 * `binary_classfication` summarizes the performance of a binary classifier, plotting curves such as ROC, Precision-Recall, and F1 score for different classification thresholds. Learn more with [this](examples/plot_binary_classification.py) example.
 
-### Some utilities available in `segretini-matplottini`
+### 🧪 Some utilities available in `segretini-matplottini`
 
 The astute reader might say "Hey, I don't need any of those plots, why should I care about `segretini-matplottini`?".
 There's a lot more than plotting functions! The `utils` can be applied to any Matplotlib plot, to simplify your life when it comes to creating complex visualizations.
 * [`data`](segretini_matplottini/utils/data.py) contains functions to preprocess your experiment results by [removing outliers](https://github.com/AlbertoParravicini/segretini-matplottini/blob/master/segretini_matplottini/utils/data.py#L158) and computing the [relative performance](https://github.com/AlbertoParravicini/segretini-matplottini/blob/master/segretini_matplottini/utils/data.py#L242) from absolute performance numbers.
 * [`colors`](segretini_matplottini/utils/colors.py) provides utilities to convert your palettes to [grayscale](https://github.com/AlbertoParravicini/segretini-matplottini/blob/master/segretini_matplottini/utils/colors.py#L48) to check how your plot will look when printed in black-and-white or when seen by a color deficient person, and to simplify the [creation of palettes](https://github.com/AlbertoParravicini/segretini-matplottini/blob/master/segretini_matplottini/utils/colors.py#L61) given the start and end colors. It also has plenty of beautiful colors to choose from, validated for black and white printing and color blindness.
 * [`plot`](segretini_matplottini/utils/plot.py) is the source for general plotting utilities, from [computing](https://github.com/AlbertoParravicini/segretini-matplottini/blob/master/segretini_matplottini/utils/plot.py#L323) and [adding](https://github.com/AlbertoParravicini/segretini-matplottini/blob/master/segretini_matplottini/utils/plot.py#L390) labels to barplots to [saving plots](https://github.com/AlbertoParravicini/segretini-matplottini/blob/master/segretini_matplottini/utils/plot.py#L461) with a standardized structure, so they won't get lost or overwritten by accident.
 
@@ -143,14 +154,15 @@
 
 ### Building and releasing
 
 To build a new version of `segretini-matplottini`, run the following command. Make sure that you have `dev` dependencies installed.
 
 ```shell
 python -m build
+python -m twine upload dist/*
 ```
 
 ## 💡 Tips and Tricks
 
 An ever-growing collection of tips I've found or discovered along the way, together with some nice resources I like a lot.
 
 ### 📚 Resources
```

### Comparing `segretini-matplottini-0.2.1/segretini_matplottini.egg-info/SOURCES.txt` & `segretini-matplottini-0.2.2/segretini_matplottini.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 CHANGELOG.md
 LICENSE
 README.md
 mypy.ini
 pyproject.toml
 ruff.toml
 .github/workflows/pull_request.yaml
+.github/workflows/pypi_release.yaml
 .vscode/launch.json
 .vscode/settings.json
 data/barplot_data.csv
 data/barplot_for_multiple_categories_data.csv
 data/correlation_scatterplot_data.csv
 data/density_data.csv
 data/performance_scaling_data.csv
```

### Comparing `segretini-matplottini-0.2.1/tests/plot/test_barplot.py` & `segretini-matplottini-0.2.2/tests/plot/test_barplot.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/tests/plot/test_binary_classification.py` & `segretini-matplottini-0.2.2/tests/plot/test_binary_classification.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/tests/plot/test_correlation_scatterplot.py` & `segretini-matplottini-0.2.2/tests/plot/test_correlation_scatterplot.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/tests/plot/test_ridgeplot.py` & `segretini-matplottini-0.2.2/tests/plot/test_ridgeplot.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/tests/plot/test_roofline.py` & `segretini-matplottini-0.2.2/tests/plot/test_roofline.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/tests/plot/test_timeseries.py` & `segretini-matplottini-0.2.2/tests/plot/test_timeseries.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/tests/plot/utils.py` & `segretini-matplottini-0.2.2/tests/plot/utils.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/tests/utils/test_colors.py` & `segretini-matplottini-0.2.2/tests/utils/test_colors.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.1/tests/utils/test_data.py` & `segretini-matplottini-0.2.2/tests/utils/test_data.py`

 * *Files identical despite different names*

