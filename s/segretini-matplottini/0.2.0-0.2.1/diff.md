# Comparing `tmp/segretini-matplottini-0.2.0.tar.gz` & `tmp/segretini-matplottini-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "segretini-matplottini-0.2.0.tar", last modified: Sun Aug  6 13:07:14 2023, max compression
+gzip compressed data, was "segretini-matplottini-0.2.1.tar", last modified: Sun Aug  6 13:34:16 2023, max compression
```

## Comparing `segretini-matplottini-0.2.0.tar` & `segretini-matplottini-0.2.1.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxr-xr-x   0 albertoparravicini   (501) staff       (20)        0 2023-08-06 13:07:14.677993 segretini-matplottini-0.2.0/
-drwxr-xr-x   0 albertoparravicini   (501) staff       (20)        0 2023-08-06 13:07:14.626082 segretini-matplottini-0.2.0/.github/
-drwxr-xr-x   0 albertoparravicini   (501) staff       (20)        0 2023-08-06 13:07:14.630032 segretini-matplottini-0.2.0/.github/workflows/
--rw-r--r--   0 albertoparravicini   (501) staff       (20)      840 2023-07-31 19:28:52.000000 segretini-matplottini-0.2.0/.github/workflows/pull_request.yaml
--rw-r--r--   0 albertoparravicini   (501) staff       (20)      747 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.0/.gitignore
--rw-r--r--   0 albertoparravicini   (501) staff       (20)      587 2023-07-30 13:13:31.000000 segretini-matplottini-0.2.0/.pre-commit-config.yaml
-drwxr-xr-x   0 albertoparravicini   (501) staff       (20)        0 2023-08-06 13:07:14.630792 segretini-matplottini-0.2.0/.vscode/
--rw-r--r--   0 albertoparravicini   (501) staff       (20)      757 2023-07-22 17:05:31.000000 segretini-matplottini-0.2.0/.vscode/launch.json
--rw-r--r--   0 albertoparravicini   (501) staff       (20)      127 2023-07-23 17:29:43.000000 segretini-matplottini-0.2.0/.vscode/settings.json
--rw-r--r--   0 albertoparravicini   (501) staff       (20)     5524 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.0/CHANGELOG.md
--rw-r--r--   0 albertoparravicini   (501) staff       (20)     1081 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.0/LICENSE
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    11502 2023-08-06 13:07:14.677643 segretini-matplottini-0.2.0/PKG-INFO
--rw-r--r--   0 albertoparravicini   (501) staff       (20)     9880 2023-08-06 13:05:44.000000 segretini-matplottini-0.2.0/README.md
-drwxr-xr-x   0 albertoparravicini   (501) staff       (20)        0 2023-08-06 13:07:14.634417 segretini-matplottini-0.2.0/data/
--rw-r--r--   0 albertoparravicini   (501) staff       (20)      261 2023-07-27 18:15:28.000000 segretini-matplottini-0.2.0/data/barplot_data.csv
--rw-r--r--   0 albertoparravicini   (501) staff       (20)      340 2023-07-26 19:41:10.000000 segretini-matplottini-0.2.0/data/barplot_for_multiple_categories_data.csv
--rw-r--r--   0 albertoparravicini   (501) staff       (20)     2675 2022-02-03 08:13:39.000000 segretini-matplottini-0.2.0/data/correlation_scatterplot_data.csv
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    25669 2022-10-16 07:30:14.000000 segretini-matplottini-0.2.0/data/density_data.csv
-drwxr-xr-x   0 albertoparravicini   (501) staff       (20)        0 2023-08-06 13:07:14.626527 segretini-matplottini-0.2.0/data/notebooks/
-drwxr-xr-x   0 albertoparravicini   (501) staff       (20)        0 2023-08-06 13:07:14.635627 segretini-matplottini-0.2.0/data/notebooks/1_getting_started_with_barplots/
--rw-r--r--   0 albertoparravicini   (501) staff       (20)      277 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.0/data/notebooks/1_getting_started_with_barplots/barplot_data.csv
--rw-r--r--   0 albertoparravicini   (501) staff       (20)     1625 2022-02-03 08:13:39.000000 segretini-matplottini-0.2.0/data/performance_scaling_data.csv
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    60208 2022-02-03 08:13:39.000000 segretini-matplottini-0.2.0/data/ridgeplot_data.csv
--rw-r--r--   0 albertoparravicini   (501) staff       (20)   134509 2022-09-26 19:50:14.000000 segretini-matplottini-0.2.0/data/timeseries_data.csv
-drwxr-xr-x   0 albertoparravicini   (501) staff       (20)        0 2023-08-06 13:07:14.637559 segretini-matplottini-0.2.0/examples/
--rw-r--r--   0 albertoparravicini   (501) staff       (20)        0 2023-08-06 12:37:32.000000 segretini-matplottini-0.2.0/examples/__init__.py
--rw-r--r--   0 albertoparravicini   (501) staff       (20)     4135 2023-08-06 12:37:32.000000 segretini-matplottini-0.2.0/examples/plot_barplot.py
--rw-r--r--   0 albertoparravicini   (501) staff       (20)     2680 2023-08-06 12:37:32.000000 segretini-matplottini-0.2.0/examples/plot_binary_classification.py
--rw-r--r--   0 albertoparravicini   (501) staff       (20)     1962 2023-08-06 12:37:32.000000 segretini-matplottini-0.2.0/examples/plot_correlation_scatterplot.py
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    10527 2023-08-06 12:37:32.000000 segretini-matplottini-0.2.0/examples/plot_grid.py
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    10487 2023-08-06 12:37:32.000000 segretini-matplottini-0.2.0/examples/plot_performance_scaling.py
--rw-r--r--   0 albertoparravicini   (501) staff       (20)     2853 2023-08-06 12:37:32.000000 segretini-matplottini-0.2.0/examples/plot_ridgeplot.py
--rw-r--r--   0 albertoparravicini   (501) staff       (20)     6240 2023-08-06 12:37:32.000000 segretini-matplottini-0.2.0/examples/plot_roofline.py
--rw-r--r--   0 albertoparravicini   (501) staff       (20)     2765 2023-08-06 12:37:32.000000 segretini-matplottini-0.2.0/examples/plot_timeseries.py
--rw-r--r--   0 albertoparravicini   (501) staff       (20)      615 2023-07-30 13:13:31.000000 segretini-matplottini-0.2.0/mypy.ini
-drwxr-xr-x   0 albertoparravicini   (501) staff       (20)        0 2023-08-06 13:07:14.637740 segretini-matplottini-0.2.0/notebooks/
--rw-r--r--   0 albertoparravicini   (501) staff       (20)   103687 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.0/notebooks/1_getting_started_with_barplots.ipynb
-drwxr-xr-x   0 albertoparravicini   (501) staff       (20)        0 2023-08-06 13:07:14.664287 segretini-matplottini-0.2.0/plots/
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    11274 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.0/plots/barplot.pdf
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    34869 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.0/plots/barplot.png
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    15571 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.0/plots/barplot_for_multiple_categories.pdf
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    60298 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.0/plots/barplot_for_multiple_categories.png
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    15273 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.0/plots/barplots.pdf
--rw-r--r--   0 albertoparravicini   (501) staff       (20)   108326 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.0/plots/barplots.png
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    38357 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.0/plots/binary_classification.pdf
--rw-r--r--   0 albertoparravicini   (501) staff       (20)   228919 2023-08-06 12:03:23.000000 segretini-matplottini-0.2.0/plots/binary_classification.png
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    33890 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.0/plots/correlation_scatterplot.pdf
--rw-r--r--   0 albertoparravicini   (501) staff       (20)   206682 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.0/plots/correlation_scatterplot.png
--rw-r--r--   0 albertoparravicini   (501) staff       (20)   849171 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.0/plots/grid.pdf
--rw-r--r--   0 albertoparravicini   (501) staff       (20)   964425 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.0/plots/grid.png
--rw-r--r--   0 albertoparravicini   (501) staff       (20)   784156 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.0/plots/grid_2.pdf
--rw-r--r--   0 albertoparravicini   (501) staff       (20)   903087 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.0/plots/grid_2.png
-drwxr-xr-x   0 albertoparravicini   (501) staff       (20)        0 2023-08-06 13:07:14.626991 segretini-matplottini-0.2.0/plots/notebooks/
-drwxr-xr-x   0 albertoparravicini   (501) staff       (20)        0 2023-08-06 13:07:14.667859 segretini-matplottini-0.2.0/plots/notebooks/1_getting_started_with_barplots/
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    74133 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.0/plots/notebooks/1_getting_started_with_barplots/a_much_better_barplot.png
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    15661 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.0/plots/notebooks/1_getting_started_with_barplots/our_amazing_barplot.pdf
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    54750 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.0/plots/notebooks/1_getting_started_with_barplots/our_amazing_barplot.png
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    16746 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.0/plots/notebooks/1_getting_started_with_barplots/our_amazing_barplot_v2.pdf
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    56901 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.0/plots/notebooks/1_getting_started_with_barplots/our_amazing_barplot_v2.png
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    16615 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.0/plots/notebooks/1_getting_started_with_barplots/our_amazing_barplot_v3.pdf
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    53406 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.0/plots/notebooks/1_getting_started_with_barplots/our_amazing_barplot_v3.png
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    19563 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.0/plots/notebooks/1_getting_started_with_barplots/the_ugliest_barplot.png
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    30521 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.0/plots/performance_scaling.pdf
--rw-r--r--   0 albertoparravicini   (501) staff       (20)   264083 2023-08-06 12:03:35.000000 segretini-matplottini-0.2.0/plots/performance_scaling.png
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    96597 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.0/plots/ridgeplot_compact.pdf
--rw-r--r--   0 albertoparravicini   (501) staff       (20)   403977 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.0/plots/ridgeplot_compact.png
--rw-r--r--   0 albertoparravicini   (501) staff       (20)   100120 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.0/plots/ridgeplot_large.pdf
--rw-r--r--   0 albertoparravicini   (501) staff       (20)   582502 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.0/plots/ridgeplot_large.png
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    16056 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.0/plots/roofline.pdf
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    78276 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.0/plots/roofline.png
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    20642 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.0/plots/roofline_double.pdf
--rw-r--r--   0 albertoparravicini   (501) staff       (20)   215335 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.0/plots/roofline_double.png
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    18219 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.0/plots/roofline_stacked.pdf
--rw-r--r--   0 albertoparravicini   (501) staff       (20)   175021 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.0/plots/roofline_stacked.png
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    19875 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.0/plots/stem.pdf
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    83115 2023-08-06 12:03:52.000000 segretini-matplottini-0.2.0/plots/stem.png
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    29257 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.0/plots/timeseries.pdf
--rw-r--r--   0 albertoparravicini   (501) staff       (20)   279591 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.0/plots/timeseries.png
--rw-r--r--   0 albertoparravicini   (501) staff       (20)      932 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.0/pyproject.toml
--rw-r--r--   0 albertoparravicini   (501) staff       (20)      445 2023-07-24 13:11:18.000000 segretini-matplottini-0.2.0/ruff.toml
-drwxr-xr-x   0 albertoparravicini   (501) staff       (20)        0 2023-08-06 13:07:14.668251 segretini-matplottini-0.2.0/segretini_matplottini/
--rw-r--r--   0 albertoparravicini   (501) staff       (20)        0 2023-07-22 19:06:31.000000 segretini-matplottini-0.2.0/segretini_matplottini/__init__.py
-drwxr-xr-x   0 albertoparravicini   (501) staff       (20)        0 2023-08-06 13:07:14.671565 segretini-matplottini-0.2.0/segretini_matplottini/plot/
--rw-r--r--   0 albertoparravicini   (501) staff       (20)      744 2023-07-29 16:04:44.000000 segretini-matplottini-0.2.0/segretini_matplottini/plot/__init__.py
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    24737 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.0/segretini_matplottini/plot/barplot.py
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    51366 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.0/segretini_matplottini/plot/binary_classification.py
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    10544 2023-07-31 19:29:13.000000 segretini-matplottini-0.2.0/segretini_matplottini/plot/correlation_scatterplot.py
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    25419 2023-07-31 19:28:52.000000 segretini-matplottini-0.2.0/segretini_matplottini/plot/ridgeplot.py
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    13206 2023-07-31 19:41:05.000000 segretini-matplottini-0.2.0/segretini_matplottini/plot/roofline.py
--rw-r--r--   0 albertoparravicini   (501) staff       (20)     9102 2023-07-31 19:28:52.000000 segretini-matplottini-0.2.0/segretini_matplottini/plot/timeseries.py
--rw-r--r--   0 albertoparravicini   (501) staff       (20)        0 2023-07-20 14:13:02.000000 segretini-matplottini-0.2.0/segretini_matplottini/py.typed
-drwxr-xr-x   0 albertoparravicini   (501) staff       (20)        0 2023-08-06 13:07:14.673366 segretini-matplottini-0.2.0/segretini_matplottini/utils/
--rw-r--r--   0 albertoparravicini   (501) staff       (20)     1146 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.0/segretini_matplottini/utils/__init__.py
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    17140 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.0/segretini_matplottini/utils/colors.py
--rw-r--r--   0 albertoparravicini   (501) staff       (20)       40 2023-07-25 09:51:34.000000 segretini-matplottini-0.2.0/segretini_matplottini/utils/constants.py
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    18079 2023-07-31 19:28:52.000000 segretini-matplottini-0.2.0/segretini_matplottini/utils/data.py
--rwxr-xr-x   0 albertoparravicini   (501) staff       (20)     4813 2023-07-24 12:56:17.000000 segretini-matplottini-0.2.0/segretini_matplottini/utils/legend.py
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    23306 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.0/segretini_matplottini/utils/plot.py
-drwxr-xr-x   0 albertoparravicini   (501) staff       (20)        0 2023-08-06 13:07:14.668971 segretini-matplottini-0.2.0/segretini_matplottini.egg-info/
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    11502 2023-08-06 13:07:14.000000 segretini-matplottini-0.2.0/segretini_matplottini.egg-info/PKG-INFO
--rw-r--r--   0 albertoparravicini   (501) staff       (20)     3208 2023-08-06 13:07:14.000000 segretini-matplottini-0.2.0/segretini_matplottini.egg-info/SOURCES.txt
--rw-r--r--   0 albertoparravicini   (501) staff       (20)        1 2023-08-06 13:07:14.000000 segretini-matplottini-0.2.0/segretini_matplottini.egg-info/dependency_links.txt
--rw-r--r--   0 albertoparravicini   (501) staff       (20)      216 2023-08-06 13:07:14.000000 segretini-matplottini-0.2.0/segretini_matplottini.egg-info/requires.txt
--rw-r--r--   0 albertoparravicini   (501) staff       (20)       22 2023-08-06 13:07:14.000000 segretini-matplottini-0.2.0/segretini_matplottini.egg-info/top_level.txt
--rw-r--r--   0 albertoparravicini   (501) staff       (20)       38 2023-08-06 13:07:14.678053 segretini-matplottini-0.2.0/setup.cfg
-drwxr-xr-x   0 albertoparravicini   (501) staff       (20)        0 2023-08-06 13:07:14.627643 segretini-matplottini-0.2.0/tests/
-drwxr-xr-x   0 albertoparravicini   (501) staff       (20)        0 2023-08-06 13:07:14.676387 segretini-matplottini-0.2.0/tests/plot/
--rw-r--r--   0 albertoparravicini   (501) staff       (20)        0 2023-07-25 11:55:13.000000 segretini-matplottini-0.2.0/tests/plot/__init__.py
--rw-r--r--   0 albertoparravicini   (501) staff       (20)    11053 2023-07-27 16:39:26.000000 segretini-matplottini-0.2.0/tests/plot/test_barplot.py
--rw-r--r--   0 albertoparravicini   (501) staff       (20)     4991 2023-07-29 16:04:44.000000 segretini-matplottini-0.2.0/tests/plot/test_binary_classification.py
--rw-r--r--   0 albertoparravicini   (501) staff       (20)     1949 2023-07-31 19:28:52.000000 segretini-matplottini-0.2.0/tests/plot/test_correlation_scatterplot.py
--rw-r--r--   0 albertoparravicini   (501) staff       (20)     3579 2023-07-31 19:28:52.000000 segretini-matplottini-0.2.0/tests/plot/test_ridgeplot.py
--rw-r--r--   0 albertoparravicini   (501) staff       (20)     3877 2023-07-31 19:28:52.000000 segretini-matplottini-0.2.0/tests/plot/test_roofline.py
--rw-r--r--   0 albertoparravicini   (501) staff       (20)     1899 2023-07-26 14:29:48.000000 segretini-matplottini-0.2.0/tests/plot/test_timeseries.py
--rw-r--r--   0 albertoparravicini   (501) staff       (20)     1010 2023-07-25 12:01:20.000000 segretini-matplottini-0.2.0/tests/plot/utils.py
-drwxr-xr-x   0 albertoparravicini   (501) staff       (20)        0 2023-08-06 13:07:14.677167 segretini-matplottini-0.2.0/tests/utils/
--rw-r--r--   0 albertoparravicini   (501) staff       (20)     4222 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.0/tests/utils/test_colors.py
--rw-r--r--   0 albertoparravicini   (501) staff       (20)     2404 2023-07-28 09:21:40.000000 segretini-matplottini-0.2.0/tests/utils/test_data.py
+drwxr-xr-x   0 albertoparravicini   (501) staff       (20)        0 2023-08-06 13:34:16.849855 segretini-matplottini-0.2.1/
+drwxr-xr-x   0 albertoparravicini   (501) staff       (20)        0 2023-08-06 13:34:16.797140 segretini-matplottini-0.2.1/.github/
+drwxr-xr-x   0 albertoparravicini   (501) staff       (20)        0 2023-08-06 13:34:16.803732 segretini-matplottini-0.2.1/.github/workflows/
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)      840 2023-07-31 19:28:52.000000 segretini-matplottini-0.2.1/.github/workflows/pull_request.yaml
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)      747 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/.gitignore
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)      587 2023-07-30 13:13:31.000000 segretini-matplottini-0.2.1/.pre-commit-config.yaml
+drwxr-xr-x   0 albertoparravicini   (501) staff       (20)        0 2023-08-06 13:34:16.804627 segretini-matplottini-0.2.1/.vscode/
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)      757 2023-07-22 17:05:31.000000 segretini-matplottini-0.2.1/.vscode/launch.json
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)      127 2023-07-23 17:29:43.000000 segretini-matplottini-0.2.1/.vscode/settings.json
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)     5524 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/CHANGELOG.md
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)     1081 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/LICENSE
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)    11501 2023-08-06 13:34:16.849507 segretini-matplottini-0.2.1/PKG-INFO
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)     9879 2023-08-06 13:07:18.000000 segretini-matplottini-0.2.1/README.md
+drwxr-xr-x   0 albertoparravicini   (501) staff       (20)        0 2023-08-06 13:34:16.807771 segretini-matplottini-0.2.1/data/
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)      261 2023-07-27 18:15:28.000000 segretini-matplottini-0.2.1/data/barplot_data.csv
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)      340 2023-07-26 19:41:10.000000 segretini-matplottini-0.2.1/data/barplot_for_multiple_categories_data.csv
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)     2675 2022-02-03 08:13:39.000000 segretini-matplottini-0.2.1/data/correlation_scatterplot_data.csv
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)    25669 2022-10-16 07:30:14.000000 segretini-matplottini-0.2.1/data/density_data.csv
+drwxr-xr-x   0 albertoparravicini   (501) staff       (20)        0 2023-08-06 13:34:16.797531 segretini-matplottini-0.2.1/data/notebooks/
+drwxr-xr-x   0 albertoparravicini   (501) staff       (20)        0 2023-08-06 13:34:16.808925 segretini-matplottini-0.2.1/data/notebooks/1_getting_started_with_barplots/
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)      277 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/data/notebooks/1_getting_started_with_barplots/barplot_data.csv
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)     1625 2022-02-03 08:13:39.000000 segretini-matplottini-0.2.1/data/performance_scaling_data.csv
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)    60208 2022-02-03 08:13:39.000000 segretini-matplottini-0.2.1/data/ridgeplot_data.csv
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)   134509 2022-09-26 19:50:14.000000 segretini-matplottini-0.2.1/data/timeseries_data.csv
+drwxr-xr-x   0 albertoparravicini   (501) staff       (20)        0 2023-08-06 13:34:16.810795 segretini-matplottini-0.2.1/examples/
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)        0 2023-08-06 12:37:32.000000 segretini-matplottini-0.2.1/examples/__init__.py
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)     4135 2023-08-06 12:37:32.000000 segretini-matplottini-0.2.1/examples/plot_barplot.py
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)     2680 2023-08-06 12:37:32.000000 segretini-matplottini-0.2.1/examples/plot_binary_classification.py
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)     1962 2023-08-06 12:37:32.000000 segretini-matplottini-0.2.1/examples/plot_correlation_scatterplot.py
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)    10527 2023-08-06 12:37:32.000000 segretini-matplottini-0.2.1/examples/plot_grid.py
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)    10487 2023-08-06 12:37:32.000000 segretini-matplottini-0.2.1/examples/plot_performance_scaling.py
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)     2853 2023-08-06 12:37:32.000000 segretini-matplottini-0.2.1/examples/plot_ridgeplot.py
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)     6240 2023-08-06 12:37:32.000000 segretini-matplottini-0.2.1/examples/plot_roofline.py
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)     2765 2023-08-06 12:37:32.000000 segretini-matplottini-0.2.1/examples/plot_timeseries.py
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)      615 2023-07-30 13:13:31.000000 segretini-matplottini-0.2.1/mypy.ini
+drwxr-xr-x   0 albertoparravicini   (501) staff       (20)        0 2023-08-06 13:34:16.810975 segretini-matplottini-0.2.1/notebooks/
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)   103687 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/notebooks/1_getting_started_with_barplots.ipynb
+drwxr-xr-x   0 albertoparravicini   (501) staff       (20)        0 2023-08-06 13:34:16.834477 segretini-matplottini-0.2.1/plots/
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)    11274 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/plots/barplot.pdf
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)    34869 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/plots/barplot.png
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)    15571 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/plots/barplot_for_multiple_categories.pdf
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)    60298 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/plots/barplot_for_multiple_categories.png
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)    15273 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/plots/barplots.pdf
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)   108326 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/plots/barplots.png
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)    38357 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/plots/binary_classification.pdf
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)   228919 2023-08-06 12:03:23.000000 segretini-matplottini-0.2.1/plots/binary_classification.png
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)    33890 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/plots/correlation_scatterplot.pdf
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)   206682 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/plots/correlation_scatterplot.png
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)   849171 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/plots/grid.pdf
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)   964425 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/plots/grid.png
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)   784156 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/plots/grid_2.pdf
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)   903087 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/plots/grid_2.png
+drwxr-xr-x   0 albertoparravicini   (501) staff       (20)        0 2023-08-06 13:34:16.797969 segretini-matplottini-0.2.1/plots/notebooks/
+drwxr-xr-x   0 albertoparravicini   (501) staff       (20)        0 2023-08-06 13:34:16.837716 segretini-matplottini-0.2.1/plots/notebooks/1_getting_started_with_barplots/
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)    74133 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/plots/notebooks/1_getting_started_with_barplots/a_much_better_barplot.png
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)    15661 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/plots/notebooks/1_getting_started_with_barplots/our_amazing_barplot.pdf
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)    54750 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/plots/notebooks/1_getting_started_with_barplots/our_amazing_barplot.png
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)    16746 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/plots/notebooks/1_getting_started_with_barplots/our_amazing_barplot_v2.pdf
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)    56901 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/plots/notebooks/1_getting_started_with_barplots/our_amazing_barplot_v2.png
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)    16615 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/plots/notebooks/1_getting_started_with_barplots/our_amazing_barplot_v3.pdf
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)    53406 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/plots/notebooks/1_getting_started_with_barplots/our_amazing_barplot_v3.png
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)    19563 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/plots/notebooks/1_getting_started_with_barplots/the_ugliest_barplot.png
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)    30521 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/plots/performance_scaling.pdf
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)   264083 2023-08-06 12:03:35.000000 segretini-matplottini-0.2.1/plots/performance_scaling.png
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)    96597 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/plots/ridgeplot_compact.pdf
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)   403977 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/plots/ridgeplot_compact.png
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)   100120 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/plots/ridgeplot_large.pdf
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)   582502 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/plots/ridgeplot_large.png
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)    16056 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/plots/roofline.pdf
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)    78276 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/plots/roofline.png
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)    20642 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/plots/roofline_double.pdf
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)   215335 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/plots/roofline_double.png
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)    18219 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/plots/roofline_stacked.pdf
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)   175021 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/plots/roofline_stacked.png
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)    19875 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/plots/stem.pdf
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)    83115 2023-08-06 12:03:52.000000 segretini-matplottini-0.2.1/plots/stem.png
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)    29257 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/plots/timeseries.pdf
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)   279591 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/plots/timeseries.png
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)      932 2023-08-06 13:33:18.000000 segretini-matplottini-0.2.1/pyproject.toml
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)      445 2023-07-24 13:11:18.000000 segretini-matplottini-0.2.1/ruff.toml
+drwxr-xr-x   0 albertoparravicini   (501) staff       (20)        0 2023-08-06 13:34:16.838083 segretini-matplottini-0.2.1/segretini_matplottini/
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)        0 2023-07-22 19:06:31.000000 segretini-matplottini-0.2.1/segretini_matplottini/__init__.py
+drwxr-xr-x   0 albertoparravicini   (501) staff       (20)        0 2023-08-06 13:34:16.843743 segretini-matplottini-0.2.1/segretini_matplottini/plot/
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)      744 2023-07-29 16:04:44.000000 segretini-matplottini-0.2.1/segretini_matplottini/plot/__init__.py
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)    24737 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/segretini_matplottini/plot/barplot.py
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)    51366 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/segretini_matplottini/plot/binary_classification.py
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)    10544 2023-07-31 19:29:13.000000 segretini-matplottini-0.2.1/segretini_matplottini/plot/correlation_scatterplot.py
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)    25419 2023-07-31 19:28:52.000000 segretini-matplottini-0.2.1/segretini_matplottini/plot/ridgeplot.py
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)    13206 2023-07-31 19:41:05.000000 segretini-matplottini-0.2.1/segretini_matplottini/plot/roofline.py
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)     9102 2023-07-31 19:28:52.000000 segretini-matplottini-0.2.1/segretini_matplottini/plot/timeseries.py
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)        0 2023-07-20 14:13:02.000000 segretini-matplottini-0.2.1/segretini_matplottini/py.typed
+drwxr-xr-x   0 albertoparravicini   (501) staff       (20)        0 2023-08-06 13:34:16.845256 segretini-matplottini-0.2.1/segretini_matplottini/utils/
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)     1146 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/segretini_matplottini/utils/__init__.py
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)    17140 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/segretini_matplottini/utils/colors.py
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)       40 2023-07-25 09:51:34.000000 segretini-matplottini-0.2.1/segretini_matplottini/utils/constants.py
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)    18079 2023-07-31 19:28:52.000000 segretini-matplottini-0.2.1/segretini_matplottini/utils/data.py
+-rwxr-xr-x   0 albertoparravicini   (501) staff       (20)     4813 2023-07-24 12:56:17.000000 segretini-matplottini-0.2.1/segretini_matplottini/utils/legend.py
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)    23306 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/segretini_matplottini/utils/plot.py
+drwxr-xr-x   0 albertoparravicini   (501) staff       (20)        0 2023-08-06 13:34:16.838865 segretini-matplottini-0.2.1/segretini_matplottini.egg-info/
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)    11501 2023-08-06 13:34:16.000000 segretini-matplottini-0.2.1/segretini_matplottini.egg-info/PKG-INFO
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)     3208 2023-08-06 13:34:16.000000 segretini-matplottini-0.2.1/segretini_matplottini.egg-info/SOURCES.txt
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)        1 2023-08-06 13:34:16.000000 segretini-matplottini-0.2.1/segretini_matplottini.egg-info/dependency_links.txt
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)      216 2023-08-06 13:34:16.000000 segretini-matplottini-0.2.1/segretini_matplottini.egg-info/requires.txt
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)       22 2023-08-06 13:34:16.000000 segretini-matplottini-0.2.1/segretini_matplottini.egg-info/top_level.txt
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)       38 2023-08-06 13:34:16.849928 segretini-matplottini-0.2.1/setup.cfg
+drwxr-xr-x   0 albertoparravicini   (501) staff       (20)        0 2023-08-06 13:34:16.798699 segretini-matplottini-0.2.1/tests/
+drwxr-xr-x   0 albertoparravicini   (501) staff       (20)        0 2023-08-06 13:34:16.848607 segretini-matplottini-0.2.1/tests/plot/
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)        0 2023-07-25 11:55:13.000000 segretini-matplottini-0.2.1/tests/plot/__init__.py
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)    11053 2023-07-27 16:39:26.000000 segretini-matplottini-0.2.1/tests/plot/test_barplot.py
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)     4991 2023-07-29 16:04:44.000000 segretini-matplottini-0.2.1/tests/plot/test_binary_classification.py
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)     1949 2023-07-31 19:28:52.000000 segretini-matplottini-0.2.1/tests/plot/test_correlation_scatterplot.py
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)     3579 2023-07-31 19:28:52.000000 segretini-matplottini-0.2.1/tests/plot/test_ridgeplot.py
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)     3877 2023-07-31 19:28:52.000000 segretini-matplottini-0.2.1/tests/plot/test_roofline.py
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)     1899 2023-07-26 14:29:48.000000 segretini-matplottini-0.2.1/tests/plot/test_timeseries.py
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)     1010 2023-07-25 12:01:20.000000 segretini-matplottini-0.2.1/tests/plot/utils.py
+drwxr-xr-x   0 albertoparravicini   (501) staff       (20)        0 2023-08-06 13:34:16.849062 segretini-matplottini-0.2.1/tests/utils/
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)     4222 2023-08-06 13:01:58.000000 segretini-matplottini-0.2.1/tests/utils/test_colors.py
+-rw-r--r--   0 albertoparravicini   (501) staff       (20)     2404 2023-07-28 09:21:40.000000 segretini-matplottini-0.2.1/tests/utils/test_data.py
```

### Comparing `segretini-matplottini-0.2.0/.github/workflows/pull_request.yaml` & `segretini-matplottini-0.2.1/.github/workflows/pull_request.yaml`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/.gitignore` & `segretini-matplottini-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/.pre-commit-config.yaml` & `segretini-matplottini-0.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/.vscode/launch.json` & `segretini-matplottini-0.2.1/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/CHANGELOG.md` & `segretini-matplottini-0.2.1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/LICENSE` & `segretini-matplottini-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/PKG-INFO` & `segretini-matplottini-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segretini-matplottini
-Version: 0.2.0
+Version: 0.2.1
 Summary: Colorful recipes and utilities for Matplolib and Seaborn, to create publication-ready plots
 Author-email: Alberto Parravicini <alberto.parravicini@polimi.it>
 License: MIT License
         
         Copyright (c) 2020-2023 Alberto Parravicini
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -142,15 +142,15 @@
 ```
 
 ### Building and releasing
 
 To build a new version of `segretini-matplottini`, run the following command. Make sure that you have `dev` dependencies installed.
 
 ```shell
-python3 -m build
+python -m build
 ```
 
 ## 💡 Tips and Tricks
 
 An ever-growing collection of tips I've found or discovered along the way, together with some nice resources I like a lot.
 
 ### 📚 Resources
```

### Comparing `segretini-matplottini-0.2.0/README.md` & `segretini-matplottini-0.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,15 @@
 ```
 
 ### Building and releasing
 
 To build a new version of `segretini-matplottini`, run the following command. Make sure that you have `dev` dependencies installed.
 
 ```shell
-python3 -m build
+python -m build
 ```
 
 ## 💡 Tips and Tricks
 
 An ever-growing collection of tips I've found or discovered along the way, together with some nice resources I like a lot.
 
 ### 📚 Resources
```

### Comparing `segretini-matplottini-0.2.0/data/correlation_scatterplot_data.csv` & `segretini-matplottini-0.2.1/data/correlation_scatterplot_data.csv`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/data/density_data.csv` & `segretini-matplottini-0.2.1/data/density_data.csv`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/data/performance_scaling_data.csv` & `segretini-matplottini-0.2.1/data/performance_scaling_data.csv`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/data/ridgeplot_data.csv` & `segretini-matplottini-0.2.1/data/ridgeplot_data.csv`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/data/timeseries_data.csv` & `segretini-matplottini-0.2.1/data/timeseries_data.csv`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/examples/plot_barplot.py` & `segretini-matplottini-0.2.1/examples/plot_barplot.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/examples/plot_binary_classification.py` & `segretini-matplottini-0.2.1/examples/plot_binary_classification.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/examples/plot_correlation_scatterplot.py` & `segretini-matplottini-0.2.1/examples/plot_correlation_scatterplot.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/examples/plot_grid.py` & `segretini-matplottini-0.2.1/examples/plot_grid.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/examples/plot_performance_scaling.py` & `segretini-matplottini-0.2.1/examples/plot_performance_scaling.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/examples/plot_ridgeplot.py` & `segretini-matplottini-0.2.1/examples/plot_ridgeplot.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/examples/plot_roofline.py` & `segretini-matplottini-0.2.1/examples/plot_roofline.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/examples/plot_timeseries.py` & `segretini-matplottini-0.2.1/examples/plot_timeseries.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/mypy.ini` & `segretini-matplottini-0.2.1/mypy.ini`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/notebooks/1_getting_started_with_barplots.ipynb` & `segretini-matplottini-0.2.1/notebooks/1_getting_started_with_barplots.ipynb`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/plots/barplot.pdf` & `segretini-matplottini-0.2.1/plots/barplot.pdf`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/plots/barplot.png` & `segretini-matplottini-0.2.1/plots/barplot.png`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/plots/barplot_for_multiple_categories.pdf` & `segretini-matplottini-0.2.1/plots/barplot_for_multiple_categories.pdf`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/plots/barplot_for_multiple_categories.png` & `segretini-matplottini-0.2.1/plots/barplot_for_multiple_categories.png`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/plots/barplots.pdf` & `segretini-matplottini-0.2.1/plots/barplots.pdf`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/plots/barplots.png` & `segretini-matplottini-0.2.1/plots/barplots.png`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/plots/binary_classification.pdf` & `segretini-matplottini-0.2.1/plots/binary_classification.pdf`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/plots/binary_classification.png` & `segretini-matplottini-0.2.1/plots/binary_classification.png`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/plots/correlation_scatterplot.pdf` & `segretini-matplottini-0.2.1/plots/correlation_scatterplot.pdf`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/plots/correlation_scatterplot.png` & `segretini-matplottini-0.2.1/plots/correlation_scatterplot.png`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/plots/grid.pdf` & `segretini-matplottini-0.2.1/plots/grid.pdf`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/plots/grid.png` & `segretini-matplottini-0.2.1/plots/grid.png`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/plots/grid_2.pdf` & `segretini-matplottini-0.2.1/plots/grid_2.pdf`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/plots/grid_2.png` & `segretini-matplottini-0.2.1/plots/grid_2.png`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/plots/notebooks/1_getting_started_with_barplots/a_much_better_barplot.png` & `segretini-matplottini-0.2.1/plots/notebooks/1_getting_started_with_barplots/a_much_better_barplot.png`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/plots/notebooks/1_getting_started_with_barplots/our_amazing_barplot.pdf` & `segretini-matplottini-0.2.1/plots/notebooks/1_getting_started_with_barplots/our_amazing_barplot.pdf`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/plots/notebooks/1_getting_started_with_barplots/our_amazing_barplot.png` & `segretini-matplottini-0.2.1/plots/notebooks/1_getting_started_with_barplots/our_amazing_barplot.png`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/plots/notebooks/1_getting_started_with_barplots/our_amazing_barplot_v2.pdf` & `segretini-matplottini-0.2.1/plots/notebooks/1_getting_started_with_barplots/our_amazing_barplot_v2.pdf`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/plots/notebooks/1_getting_started_with_barplots/our_amazing_barplot_v2.png` & `segretini-matplottini-0.2.1/plots/notebooks/1_getting_started_with_barplots/our_amazing_barplot_v2.png`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/plots/notebooks/1_getting_started_with_barplots/our_amazing_barplot_v3.pdf` & `segretini-matplottini-0.2.1/plots/notebooks/1_getting_started_with_barplots/our_amazing_barplot_v3.pdf`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/plots/notebooks/1_getting_started_with_barplots/our_amazing_barplot_v3.png` & `segretini-matplottini-0.2.1/plots/notebooks/1_getting_started_with_barplots/our_amazing_barplot_v3.png`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/plots/notebooks/1_getting_started_with_barplots/the_ugliest_barplot.png` & `segretini-matplottini-0.2.1/plots/notebooks/1_getting_started_with_barplots/the_ugliest_barplot.png`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/plots/performance_scaling.pdf` & `segretini-matplottini-0.2.1/plots/performance_scaling.pdf`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/plots/performance_scaling.png` & `segretini-matplottini-0.2.1/plots/performance_scaling.png`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/plots/ridgeplot_compact.pdf` & `segretini-matplottini-0.2.1/plots/ridgeplot_compact.pdf`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/plots/ridgeplot_compact.png` & `segretini-matplottini-0.2.1/plots/ridgeplot_compact.png`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/plots/ridgeplot_large.pdf` & `segretini-matplottini-0.2.1/plots/ridgeplot_large.pdf`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/plots/ridgeplot_large.png` & `segretini-matplottini-0.2.1/plots/ridgeplot_large.png`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/plots/roofline.pdf` & `segretini-matplottini-0.2.1/plots/roofline.pdf`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/plots/roofline.png` & `segretini-matplottini-0.2.1/plots/roofline.png`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/plots/roofline_double.pdf` & `segretini-matplottini-0.2.1/plots/roofline_double.pdf`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/plots/roofline_double.png` & `segretini-matplottini-0.2.1/plots/roofline_double.png`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/plots/roofline_stacked.pdf` & `segretini-matplottini-0.2.1/plots/roofline_stacked.pdf`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/plots/roofline_stacked.png` & `segretini-matplottini-0.2.1/plots/roofline_stacked.png`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/plots/stem.pdf` & `segretini-matplottini-0.2.1/plots/stem.pdf`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/plots/stem.png` & `segretini-matplottini-0.2.1/plots/stem.png`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/plots/timeseries.pdf` & `segretini-matplottini-0.2.1/plots/timeseries.pdf`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/plots/timeseries.png` & `segretini-matplottini-0.2.1/plots/timeseries.png`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/pyproject.toml` & `segretini-matplottini-0.2.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
-version = "0.2.0"
+version = "0.2.1"
 name = "segretini-matplottini"
 description = "Colorful recipes and utilities for Matplolib and Seaborn, to create publication-ready plots"
 authors = [{name = "Alberto Parravicini", email = "alberto.parravicini@polimi.it"}]
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">= 3.9"
 dependencies = [
```

### Comparing `segretini-matplottini-0.2.0/segretini_matplottini/plot/__init__.py` & `segretini-matplottini-0.2.1/segretini_matplottini/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/segretini_matplottini/plot/barplot.py` & `segretini-matplottini-0.2.1/segretini_matplottini/plot/barplot.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/segretini_matplottini/plot/binary_classification.py` & `segretini-matplottini-0.2.1/segretini_matplottini/plot/binary_classification.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/segretini_matplottini/plot/correlation_scatterplot.py` & `segretini-matplottini-0.2.1/segretini_matplottini/plot/correlation_scatterplot.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/segretini_matplottini/plot/ridgeplot.py` & `segretini-matplottini-0.2.1/segretini_matplottini/plot/ridgeplot.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/segretini_matplottini/plot/roofline.py` & `segretini-matplottini-0.2.1/segretini_matplottini/plot/roofline.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/segretini_matplottini/plot/timeseries.py` & `segretini-matplottini-0.2.1/segretini_matplottini/plot/timeseries.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/segretini_matplottini/utils/__init__.py` & `segretini-matplottini-0.2.1/segretini_matplottini/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/segretini_matplottini/utils/colors.py` & `segretini-matplottini-0.2.1/segretini_matplottini/utils/colors.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/segretini_matplottini/utils/data.py` & `segretini-matplottini-0.2.1/segretini_matplottini/utils/data.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/segretini_matplottini/utils/legend.py` & `segretini-matplottini-0.2.1/segretini_matplottini/utils/legend.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/segretini_matplottini/utils/plot.py` & `segretini-matplottini-0.2.1/segretini_matplottini/utils/plot.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/segretini_matplottini.egg-info/PKG-INFO` & `segretini-matplottini-0.2.1/segretini_matplottini.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segretini-matplottini
-Version: 0.2.0
+Version: 0.2.1
 Summary: Colorful recipes and utilities for Matplolib and Seaborn, to create publication-ready plots
 Author-email: Alberto Parravicini <alberto.parravicini@polimi.it>
 License: MIT License
         
         Copyright (c) 2020-2023 Alberto Parravicini
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -142,15 +142,15 @@
 ```
 
 ### Building and releasing
 
 To build a new version of `segretini-matplottini`, run the following command. Make sure that you have `dev` dependencies installed.
 
 ```shell
-python3 -m build
+python -m build
 ```
 
 ## 💡 Tips and Tricks
 
 An ever-growing collection of tips I've found or discovered along the way, together with some nice resources I like a lot.
 
 ### 📚 Resources
```

### Comparing `segretini-matplottini-0.2.0/segretini_matplottini.egg-info/SOURCES.txt` & `segretini-matplottini-0.2.1/segretini_matplottini.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/tests/plot/test_barplot.py` & `segretini-matplottini-0.2.1/tests/plot/test_barplot.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/tests/plot/test_binary_classification.py` & `segretini-matplottini-0.2.1/tests/plot/test_binary_classification.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/tests/plot/test_correlation_scatterplot.py` & `segretini-matplottini-0.2.1/tests/plot/test_correlation_scatterplot.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/tests/plot/test_ridgeplot.py` & `segretini-matplottini-0.2.1/tests/plot/test_ridgeplot.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/tests/plot/test_roofline.py` & `segretini-matplottini-0.2.1/tests/plot/test_roofline.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/tests/plot/test_timeseries.py` & `segretini-matplottini-0.2.1/tests/plot/test_timeseries.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/tests/plot/utils.py` & `segretini-matplottini-0.2.1/tests/plot/utils.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/tests/utils/test_colors.py` & `segretini-matplottini-0.2.1/tests/utils/test_colors.py`

 * *Files identical despite different names*

### Comparing `segretini-matplottini-0.2.0/tests/utils/test_data.py` & `segretini-matplottini-0.2.1/tests/utils/test_data.py`

 * *Files identical despite different names*

