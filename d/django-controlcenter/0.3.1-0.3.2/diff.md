# Comparing `tmp/django-controlcenter-0.3.1.tar.gz` & `tmp/django-controlcenter-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-controlcenter-0.3.1.tar", last modified: Sat Jan 22 03:58:23 2022, max compression
+gzip compressed data, was "django-controlcenter-0.3.2.tar", last modified: Sun Aug  6 17:01:58 2023, max compression
```

## Comparing `django-controlcenter-0.3.1.tar` & `django-controlcenter-0.3.2.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 byashimov   (501) staff       (20)        0 2022-01-22 03:58:23.000000 django-controlcenter-0.3.1/
--rw-r--r--   0 byashimov   (501) staff       (20)     1535 2017-03-28 20:34:04.000000 django-controlcenter-0.3.1/LICENSE
--rw-r--r--   0 byashimov   (501) staff       (20)      179 2018-12-11 21:57:54.000000 django-controlcenter-0.3.1/MANIFEST.in
--rw-r--r--   0 byashimov   (501) staff       (20)     7925 2022-01-22 03:58:23.000000 django-controlcenter-0.3.1/PKG-INFO
--rw-r--r--   0 byashimov   (501) staff       (20)     5034 2022-01-22 03:45:21.000000 django-controlcenter-0.3.1/README.rst
-drwxr-xr-x   0 byashimov   (501) staff       (20)        0 2022-01-22 03:58:23.000000 django-controlcenter-0.3.1/controlcenter/
--rw-r--r--   0 byashimov   (501) staff       (20)       42 2017-12-11 07:46:20.000000 django-controlcenter-0.3.1/controlcenter/__init__.py
--rw-r--r--   0 byashimov   (501) staff       (20)      122 2017-12-11 07:46:20.000000 django-controlcenter-0.3.1/controlcenter/app_settings.py
--rw-r--r--   0 byashimov   (501) staff       (20)      320 2017-12-11 07:46:20.000000 django-controlcenter-0.3.1/controlcenter/base.py
--rw-r--r--   0 byashimov   (501) staff       (20)     1615 2022-01-21 19:21:10.000000 django-controlcenter-0.3.1/controlcenter/dashboards.py
-drwxr-xr-x   0 byashimov   (501) staff       (20)        0 2022-01-22 03:58:23.000000 django-controlcenter-0.3.1/controlcenter/images/
--rw-r--r--   0 byashimov   (501) staff       (20)      126 2016-04-06 08:08:13.000000 django-controlcenter-0.3.1/controlcenter/images/chart-no-data.png
--rw-r--r--   0 byashimov   (501) staff       (20)      370 2016-04-06 08:08:13.000000 django-controlcenter-0.3.1/controlcenter/images/widget-out.png
--rw-r--r--   0 byashimov   (501) staff       (20)      121 2016-04-06 08:08:13.000000 django-controlcenter-0.3.1/controlcenter/images/widget-stripes.png
--rw-r--r--   0 byashimov   (501) staff       (20)      113 2016-04-06 08:08:13.000000 django-controlcenter-0.3.1/controlcenter/images/widget-tab.png
-drwxr-xr-x   0 byashimov   (501) staff       (20)        0 2022-01-22 03:58:23.000000 django-controlcenter-0.3.1/controlcenter/static/
-drwxr-xr-x   0 byashimov   (501) staff       (20)        0 2022-01-22 03:58:23.000000 django-controlcenter-0.3.1/controlcenter/static/controlcenter/
-drwxr-xr-x   0 byashimov   (501) staff       (20)        0 2022-01-22 03:58:23.000000 django-controlcenter-0.3.1/controlcenter/static/controlcenter/css/
--rw-r--r--   0 byashimov   (501) staff       (20)     9746 2019-01-27 20:59:16.000000 django-controlcenter-0.3.1/controlcenter/static/controlcenter/css/all.css
--rw-r--r--   0 byashimov   (501) staff       (20)     3480 2016-04-06 08:10:44.000000 django-controlcenter-0.3.1/controlcenter/static/controlcenter/css/chartist-default-colors.css
--rw-r--r--   0 byashimov   (501) staff       (20)     3480 2016-04-06 08:10:49.000000 django-controlcenter-0.3.1/controlcenter/static/controlcenter/css/chartist-material-colors.css
--rw-r--r--   0 byashimov   (501) staff       (20)    14435 2018-11-05 16:04:17.000000 django-controlcenter-0.3.1/controlcenter/static/controlcenter/css/chartist.css
-drwxr-xr-x   0 byashimov   (501) staff       (20)        0 2022-01-22 03:58:23.000000 django-controlcenter-0.3.1/controlcenter/static/controlcenter/js/
-drwxr-xr-x   0 byashimov   (501) staff       (20)        0 2022-01-22 03:58:23.000000 django-controlcenter-0.3.1/controlcenter/static/controlcenter/js/chartist/
--rw-r--r--   0 byashimov   (501) staff       (20)     1309 2018-11-05 16:04:17.000000 django-controlcenter-0.3.1/controlcenter/static/controlcenter/js/chartist/chartist-plugin-pointlabels.min.js
--rw-r--r--   0 byashimov   (501) staff       (20)    40214 2018-11-05 16:04:17.000000 django-controlcenter-0.3.1/controlcenter/static/controlcenter/js/chartist/chartist.min.js
--rw-r--r--   0 byashimov   (501) staff       (20)    22945 2016-04-06 08:08:13.000000 django-controlcenter-0.3.1/controlcenter/static/controlcenter/js/masonry.pkgd.min.js
--rw-r--r--   0 byashimov   (501) staff       (20)      883 2016-04-06 08:08:13.000000 django-controlcenter-0.3.1/controlcenter/static/controlcenter/js/scripts.js
--rw-r--r--   0 byashimov   (501) staff       (20)     3398 2016-04-06 08:08:13.000000 django-controlcenter-0.3.1/controlcenter/static/controlcenter/js/sortable.min.js
-drwxr-xr-x   0 byashimov   (501) staff       (20)        0 2022-01-22 03:58:23.000000 django-controlcenter-0.3.1/controlcenter/stylus/
--rw-r--r--   0 byashimov   (501) staff       (20)     8064 2019-01-27 20:59:16.000000 django-controlcenter-0.3.1/controlcenter/stylus/all.styl
--rw-r--r--   0 byashimov   (501) staff       (20)      221 2016-04-06 08:08:13.000000 django-controlcenter-0.3.1/controlcenter/stylus/chartist-default-colors.styl
--rw-r--r--   0 byashimov   (501) staff       (20)      221 2016-04-06 08:08:13.000000 django-controlcenter-0.3.1/controlcenter/stylus/chartist-material-colors.styl
--rw-r--r--   0 byashimov   (501) staff       (20)      534 2016-04-06 08:11:42.000000 django-controlcenter-0.3.1/controlcenter/stylus/mixins.styl
--rw-r--r--   0 byashimov   (501) staff       (20)      281 2018-11-05 16:04:17.000000 django-controlcenter-0.3.1/controlcenter/stylus/variables.styl
-drwxr-xr-x   0 byashimov   (501) staff       (20)        0 2022-01-22 03:58:23.000000 django-controlcenter-0.3.1/controlcenter/templates/
-drwxr-xr-x   0 byashimov   (501) staff       (20)        0 2022-01-22 03:58:23.000000 django-controlcenter-0.3.1/controlcenter/templates/controlcenter/
--rw-r--r--   0 byashimov   (501) staff       (20)     2821 2018-11-05 16:04:17.000000 django-controlcenter-0.3.1/controlcenter/templates/controlcenter/dashboard.html
-drwxr-xr-x   0 byashimov   (501) staff       (20)        0 2022-01-22 03:58:23.000000 django-controlcenter-0.3.1/controlcenter/templates/controlcenter/snippets/
--rw-r--r--   0 byashimov   (501) staff       (20)      285 2018-11-05 16:04:17.000000 django-controlcenter-0.3.1/controlcenter/templates/controlcenter/snippets/generic_item.html
-drwxr-xr-x   0 byashimov   (501) staff       (20)        0 2022-01-22 03:58:23.000000 django-controlcenter-0.3.1/controlcenter/templates/controlcenter/widgets/
--rw-r--r--   0 byashimov   (501) staff       (20)     2553 2019-01-27 20:59:16.000000 django-controlcenter-0.3.1/controlcenter/templates/controlcenter/widgets/chart.html
-drwxr-xr-x   0 byashimov   (501) staff       (20)        0 2022-01-22 03:58:23.000000 django-controlcenter-0.3.1/controlcenter/templates/controlcenter/widgets/contrib/
--rw-r--r--   0 byashimov   (501) staff       (20)     1490 2018-12-11 21:57:54.000000 django-controlcenter-0.3.1/controlcenter/templates/controlcenter/widgets/contrib/key_value_list.html
--rw-r--r--   0 byashimov   (501) staff       (20)     1058 2018-11-05 16:04:17.000000 django-controlcenter-0.3.1/controlcenter/templates/controlcenter/widgets/contrib/value_list.html
--rw-r--r--   0 byashimov   (501) staff       (20)     2958 2019-01-27 20:59:16.000000 django-controlcenter-0.3.1/controlcenter/templates/controlcenter/widgets/itemlist.html
-drwxr-xr-x   0 byashimov   (501) staff       (20)        0 2022-01-22 03:58:23.000000 django-controlcenter-0.3.1/controlcenter/templatetags/
--rw-r--r--   0 byashimov   (501) staff       (20)        0 2017-12-11 07:46:20.000000 django-controlcenter-0.3.1/controlcenter/templatetags/__init__.py
--rw-r--r--   0 byashimov   (501) staff       (20)     5811 2022-01-21 19:21:10.000000 django-controlcenter-0.3.1/controlcenter/templatetags/controlcenter_tags.py
--rw-r--r--   0 byashimov   (501) staff       (20)      801 2022-01-21 19:21:10.000000 django-controlcenter-0.3.1/controlcenter/utils.py
--rw-r--r--   0 byashimov   (501) staff       (20)     2650 2022-01-21 22:16:56.000000 django-controlcenter-0.3.1/controlcenter/views.py
-drwxr-xr-x   0 byashimov   (501) staff       (20)        0 2022-01-22 03:58:23.000000 django-controlcenter-0.3.1/controlcenter/widgets/
--rw-r--r--   0 byashimov   (501) staff       (20)       58 2017-12-11 07:46:20.000000 django-controlcenter-0.3.1/controlcenter/widgets/__init__.py
--rw-r--r--   0 byashimov   (501) staff       (20)     3414 2022-01-21 19:20:31.000000 django-controlcenter-0.3.1/controlcenter/widgets/charts.py
-drwxr-xr-x   0 byashimov   (501) staff       (20)        0 2022-01-22 03:58:23.000000 django-controlcenter-0.3.1/controlcenter/widgets/contrib/
--rw-r--r--   0 byashimov   (501) staff       (20)        0 2018-11-05 16:04:17.000000 django-controlcenter-0.3.1/controlcenter/widgets/contrib/__init__.py
--rw-r--r--   0 byashimov   (501) staff       (20)      999 2018-11-05 16:04:17.000000 django-controlcenter-0.3.1/controlcenter/widgets/contrib/simple.py
--rw-r--r--   0 byashimov   (501) staff       (20)     4616 2022-01-21 19:21:10.000000 django-controlcenter-0.3.1/controlcenter/widgets/core.py
-drwxr-xr-x   0 byashimov   (501) staff       (20)        0 2022-01-22 03:58:23.000000 django-controlcenter-0.3.1/django_controlcenter.egg-info/
--rw-r--r--   0 byashimov   (501) staff       (20)     7925 2022-01-22 03:58:22.000000 django-controlcenter-0.3.1/django_controlcenter.egg-info/PKG-INFO
--rw-r--r--   0 byashimov   (501) staff       (20)     2291 2022-01-22 03:58:23.000000 django-controlcenter-0.3.1/django_controlcenter.egg-info/SOURCES.txt
--rw-r--r--   0 byashimov   (501) staff       (20)        1 2022-01-22 03:58:22.000000 django-controlcenter-0.3.1/django_controlcenter.egg-info/dependency_links.txt
--rw-r--r--   0 byashimov   (501) staff       (20)       22 2022-01-22 03:58:22.000000 django-controlcenter-0.3.1/django_controlcenter.egg-info/requires.txt
--rw-r--r--   0 byashimov   (501) staff       (20)       20 2022-01-22 03:58:22.000000 django-controlcenter-0.3.1/django_controlcenter.egg-info/top_level.txt
--rw-r--r--   0 byashimov   (501) staff       (20)       38 2022-01-22 03:58:23.000000 django-controlcenter-0.3.1/setup.cfg
--rw-r--r--   0 byashimov   (501) staff       (20)     1536 2022-01-22 03:42:18.000000 django-controlcenter-0.3.1/setup.py
-drwxr-xr-x   0 byashimov   (501) staff       (20)        0 2022-01-22 03:58:23.000000 django-controlcenter-0.3.1/test_project/
--rw-r--r--   0 byashimov   (501) staff       (20)      339 2018-11-05 16:04:17.000000 django-controlcenter-0.3.1/test_project/dashboards.py
--rwxr-xr-x   0 byashimov   (501) staff       (20)      241 2017-08-13 09:44:01.000000 django-controlcenter-0.3.1/test_project/manage.py
--rw-r--r--   0 byashimov   (501) staff       (20)     1518 2022-01-21 22:10:23.000000 django-controlcenter-0.3.1/test_project/settings.py
--rwxr-xr-x   0 byashimov   (501) staff       (20)      738 2022-01-21 22:08:24.000000 django-controlcenter-0.3.1/test_project/test_models.py
--rw-r--r--   0 byashimov   (501) staff       (20)      291 2022-01-22 03:25:57.000000 django-controlcenter-0.3.1/test_project/urls.py
-drwxr-xr-x   0 byashimov   (501) staff       (20)        0 2022-01-22 03:58:23.000000 django-controlcenter-0.3.1/tests/
--rw-r--r--   0 byashimov   (501) staff       (20)      290 2022-01-22 03:35:22.000000 django-controlcenter-0.3.1/tests/__init__.py
--rw-r--r--   0 byashimov   (501) staff       (20)     1108 2022-01-22 03:34:26.000000 django-controlcenter-0.3.1/tests/test_app_settings.py
--rw-r--r--   0 byashimov   (501) staff       (20)      890 2022-01-22 03:34:26.000000 django-controlcenter-0.3.1/tests/test_base.py
--rw-r--r--   0 byashimov   (501) staff       (20)     5054 2022-01-22 03:34:26.000000 django-controlcenter-0.3.1/tests/test_dashboards.py
--rw-r--r--   0 byashimov   (501) staff       (20)    11715 2022-01-22 03:34:26.000000 django-controlcenter-0.3.1/tests/test_templatetags.py
--rw-r--r--   0 byashimov   (501) staff       (20)     2441 2022-01-22 03:34:26.000000 django-controlcenter-0.3.1/tests/test_utils.py
--rw-r--r--   0 byashimov   (501) staff       (20)     4334 2022-01-22 03:34:26.000000 django-controlcenter-0.3.1/tests/test_widgets_charts.py
--rw-r--r--   0 byashimov   (501) staff       (20)     5695 2022-01-22 03:34:26.000000 django-controlcenter-0.3.1/tests/test_widgets_core.py
--rw-r--r--   0 byashimov   (501) staff       (20)     1214 2022-01-22 03:34:26.000000 django-controlcenter-0.3.1/tests/test_widgets_simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:01:58.897898 django-controlcenter-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-08-06 17:01:45.000000 django-controlcenter-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-08-06 17:01:45.000000 django-controlcenter-0.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6333 2023-08-06 17:01:58.897898 django-controlcenter-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-08-06 17:01:45.000000 django-controlcenter-0.3.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:01:58.893898 django-controlcenter-0.3.2/controlcenter/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-06 17:01:45.000000 django-controlcenter-0.3.2/controlcenter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-08-06 17:01:45.000000 django-controlcenter-0.3.2/controlcenter/app_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-08-06 17:01:45.000000 django-controlcenter-0.3.2/controlcenter/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-08-06 17:01:45.000000 django-controlcenter-0.3.2/controlcenter/dashboards.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:01:58.893898 django-controlcenter-0.3.2/controlcenter/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-08-06 17:01:45.000000 django-controlcenter-0.3.2/controlcenter/images/chart-no-data.png
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-08-06 17:01:45.000000 django-controlcenter-0.3.2/controlcenter/images/widget-out.png
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-08-06 17:01:45.000000 django-controlcenter-0.3.2/controlcenter/images/widget-stripes.png
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-08-06 17:01:45.000000 django-controlcenter-0.3.2/controlcenter/images/widget-tab.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:01:58.889898 django-controlcenter-0.3.2/controlcenter/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:01:58.889898 django-controlcenter-0.3.2/controlcenter/static/controlcenter/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:01:58.893898 django-controlcenter-0.3.2/controlcenter/static/controlcenter/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     9746 2023-08-06 17:01:45.000000 django-controlcenter-0.3.2/controlcenter/static/controlcenter/css/all.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-08-06 17:01:45.000000 django-controlcenter-0.3.2/controlcenter/static/controlcenter/css/chartist-default-colors.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-08-06 17:01:45.000000 django-controlcenter-0.3.2/controlcenter/static/controlcenter/css/chartist-material-colors.css
+-rw-r--r--   0 runner    (1001) docker     (123)    14435 2023-08-06 17:01:45.000000 django-controlcenter-0.3.2/controlcenter/static/controlcenter/css/chartist.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:01:58.893898 django-controlcenter-0.3.2/controlcenter/static/controlcenter/js/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:01:58.893898 django-controlcenter-0.3.2/controlcenter/static/controlcenter/js/chartist/
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-08-06 17:01:45.000000 django-controlcenter-0.3.2/controlcenter/static/controlcenter/js/chartist/chartist-plugin-pointlabels.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    40214 2023-08-06 17:01:45.000000 django-controlcenter-0.3.2/controlcenter/static/controlcenter/js/chartist/chartist.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    22945 2023-08-06 17:01:45.000000 django-controlcenter-0.3.2/controlcenter/static/controlcenter/js/masonry.pkgd.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-08-06 17:01:45.000000 django-controlcenter-0.3.2/controlcenter/static/controlcenter/js/scripts.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-08-06 17:01:45.000000 django-controlcenter-0.3.2/controlcenter/static/controlcenter/js/sortable.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:01:58.893898 django-controlcenter-0.3.2/controlcenter/stylus/
+-rw-r--r--   0 runner    (1001) docker     (123)     8064 2023-08-06 17:01:45.000000 django-controlcenter-0.3.2/controlcenter/stylus/all.styl
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-08-06 17:01:45.000000 django-controlcenter-0.3.2/controlcenter/stylus/chartist-default-colors.styl
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-08-06 17:01:45.000000 django-controlcenter-0.3.2/controlcenter/stylus/chartist-material-colors.styl
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-08-06 17:01:45.000000 django-controlcenter-0.3.2/controlcenter/stylus/mixins.styl
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-08-06 17:01:45.000000 django-controlcenter-0.3.2/controlcenter/stylus/variables.styl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:01:58.889898 django-controlcenter-0.3.2/controlcenter/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:01:58.893898 django-controlcenter-0.3.2/controlcenter/templates/controlcenter/
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-08-06 17:01:45.000000 django-controlcenter-0.3.2/controlcenter/templates/controlcenter/dashboard.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:01:58.893898 django-controlcenter-0.3.2/controlcenter/templates/controlcenter/snippets/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-08-06 17:01:45.000000 django-controlcenter-0.3.2/controlcenter/templates/controlcenter/snippets/generic_item.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:01:58.893898 django-controlcenter-0.3.2/controlcenter/templates/controlcenter/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-08-06 17:01:45.000000 django-controlcenter-0.3.2/controlcenter/templates/controlcenter/widgets/chart.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:01:58.893898 django-controlcenter-0.3.2/controlcenter/templates/controlcenter/widgets/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-08-06 17:01:45.000000 django-controlcenter-0.3.2/controlcenter/templates/controlcenter/widgets/contrib/key_value_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-08-06 17:01:45.000000 django-controlcenter-0.3.2/controlcenter/templates/controlcenter/widgets/contrib/value_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-08-06 17:01:45.000000 django-controlcenter-0.3.2/controlcenter/templates/controlcenter/widgets/itemlist.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:01:58.893898 django-controlcenter-0.3.2/controlcenter/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 17:01:45.000000 django-controlcenter-0.3.2/controlcenter/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5811 2023-08-06 17:01:45.000000 django-controlcenter-0.3.2/controlcenter/templatetags/controlcenter_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-08-06 17:01:45.000000 django-controlcenter-0.3.2/controlcenter/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-08-06 17:01:45.000000 django-controlcenter-0.3.2/controlcenter/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:01:58.893898 django-controlcenter-0.3.2/controlcenter/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-06 17:01:45.000000 django-controlcenter-0.3.2/controlcenter/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-08-06 17:01:45.000000 django-controlcenter-0.3.2/controlcenter/widgets/charts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:01:58.897898 django-controlcenter-0.3.2/controlcenter/widgets/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 17:01:45.000000 django-controlcenter-0.3.2/controlcenter/widgets/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-08-06 17:01:45.000000 django-controlcenter-0.3.2/controlcenter/widgets/contrib/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-08-06 17:01:45.000000 django-controlcenter-0.3.2/controlcenter/widgets/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:01:58.897898 django-controlcenter-0.3.2/django_controlcenter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6333 2023-08-06 17:01:58.000000 django-controlcenter-0.3.2/django_controlcenter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-08-06 17:01:58.000000 django-controlcenter-0.3.2/django_controlcenter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 17:01:58.000000 django-controlcenter-0.3.2/django_controlcenter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-06 17:01:58.000000 django-controlcenter-0.3.2/django_controlcenter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-06 17:01:58.000000 django-controlcenter-0.3.2/django_controlcenter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 17:01:58.897898 django-controlcenter-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-08-06 17:01:45.000000 django-controlcenter-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:01:58.897898 django-controlcenter-0.3.2/test_project/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-08-06 17:01:45.000000 django-controlcenter-0.3.2/test_project/dashboards.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      241 2023-08-06 17:01:45.000000 django-controlcenter-0.3.2/test_project/manage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-08-06 17:01:45.000000 django-controlcenter-0.3.2/test_project/settings.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      738 2023-08-06 17:01:45.000000 django-controlcenter-0.3.2/test_project/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-08-06 17:01:45.000000 django-controlcenter-0.3.2/test_project/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:01:58.897898 django-controlcenter-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-08-06 17:01:45.000000 django-controlcenter-0.3.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-08-06 17:01:45.000000 django-controlcenter-0.3.2/tests/test_app_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-08-06 17:01:45.000000 django-controlcenter-0.3.2/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-08-06 17:01:45.000000 django-controlcenter-0.3.2/tests/test_dashboards.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11715 2023-08-06 17:01:45.000000 django-controlcenter-0.3.2/tests/test_templatetags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-08-06 17:01:45.000000 django-controlcenter-0.3.2/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4334 2023-08-06 17:01:45.000000 django-controlcenter-0.3.2/tests/test_widgets_charts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-08-06 17:01:45.000000 django-controlcenter-0.3.2/tests/test_widgets_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-08-06 17:01:45.000000 django-controlcenter-0.3.2/tests/test_widgets_simple.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-controlcenter-0.3.1/LICENSE` & `django-controlcenter-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-controlcenter-0.3.1/PKG-INFO` & `django-controlcenter-0.3.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,229 +1,16 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: django-controlcenter
-Version: 0.3.1
+Version: 0.3.2
 Summary: Set of widgets to build dashboards for your Django-project.
 Home-page: https://github.com/byashimov/django-controlcenter
 Author: Murad Byashimov
 Author-email: byashimov@gmail.com
 License: BSD
-Description: Welcome to django-controlcenter!
-        ================================
-        
-        Get all your project models on one single page with charts and whistles.
-        
-        .. image:: https://cloud.githubusercontent.com/assets/1560043/14309295/b8c9aad0-fc05-11e5-96d0-44293d2d07ff.png
-            :alt: django-controlcenter
-        
-        Attention!
-        ----------
-        
-        Unfortunately, I have no time to add new features.
-        Please make PR if you need one:
-        
-        - branch from master
-        - provide tests
-        - add docs
-        - update changelog
-        
-        That's it.
-        
-        
-        Rationale
-        ---------
-        
-        Django-admin_ is a great tool to control your project activity: new orders, comments, replies, users, feedback -- everything is here. The only struggle is to switch between all those pages constantly just to check them out for new entries.
-        
-        With django-controlcenter you can have all of your models on one single page and build beautiful charts with Chartist.js_. Actually they don't even have to be a django models, get your data from wherever you want: RDBMS, NOSQL, text file or even from an external web-page, it doesn't matter.
-        
-        
-        Quickstart
-        ----------
-        
-        Install django-controlcenter:
-        
-        .. code-block:: console
-        
-            pip install -U django-controlcenter
-        
-        Create a dashboard file with unlimited number of widgets and dashboards:
-        
-        .. code-block:: python
-        
-            from controlcenter import Dashboard, widgets
-            from project.app.models import Model
-        
-            class ModelItemList(widgets.ItemList):
-                model = Model
-                list_display = ('pk', 'field')
-        
-            class MyDashboard(Dashboard):
-                widgets = (
-                    ModelItemList,
-                )
-        
-        Update settings file:
-        
-        .. code-block:: python
-        
-            INSTALLED_APPS = [
-                ...
-                'controlcenter',
-                ...
-            ]
-        
-            CONTROLCENTER_DASHBOARDS = (
-                ('mydash', 'project.dashboards.MyDashboard'),
-            )
-        
-        Plug in urls:
-        
-        .. code-block:: python
-        
-            from django.urls import path
-            from django.contrib import admin
-            from controlcenter.views import controlcenter
-        
-            urlpatterns = [
-                path('admin/', admin.site.urls),
-                path('admin/dashboard/', controlcenter.urls),
-                ...
-            ]
-        
-        Open ``/admin/dashboard/mydash/`` in browser.
-        
-        
-        Documentation
-        -------------
-        
-        Check out the docs_ for more complete examples.
-        
-        
-        Compatibility
-        -------------
-        
-        .. image:: https://travis-ci.org/byashimov/django-controlcenter.svg?branch=master
-            :alt: Build Status
-            :target: https://travis-ci.org/byashimov/django-controlcenter
-        
-        .. image:: https://codecov.io/github/byashimov/django-controlcenter/coverage.svg?branch=master
-            :alt: Codecov
-            :target: https://codecov.io/github/byashimov/django-controlcenter?branch=master
-        
-        Tested on py 3.5—3.10 and django 1—4.
-        
-        
-        Credits
-        -------
-        
-        This project uses Chartist.js_, Masonry.js_ and Sortable.js_.
-        
-        
-        Changelog
-        ---------
-        
-        0.3.1
-        ~~~~~
-        
-        - Support django 4.0, python 3.10. Thanks to @mick88.
-        - Fixed LineChart example. Thanks to @virtosubogdan.
-        
-        0.3.0
-        ~~~~~
-        
-        - Support django 3.0
-        - Python 3 only
-        
-        0.2.9
-        ~~~~~
-        
-        - ``chartist-plugin-pointlabels`` temporary fix
-        - Added sorting triangles to ``ItemList``
-        - ``ItemList`` header is now always displayed regardless sortability
-        - Other misc improvements
-        
-        Thanks to @minusf.
-        
-        0.2.8
-        ~~~~~
-        
-        - Fixed ``key_value_list.html`` widget template syntax error.
-        - Fixed attribute typo ``widget.chartist.point_labels -> point_lables``.
-        
-        Thanks to @minusf.
-        
-        0.2.7
-        ~~~~~
-        
-        - New ``TimeSeriesChart`` widget. Thanks to @pjdelport.
-        - New "simple" widgets: ``ValueList`` and ``KeyValueList``. Thanks to @tonysyu.
-        - Bunch of fixes and improvements, thanks again to @pjdelport.
-        
-        
-        0.2.6
-        ~~~~~
-        
-        - Fixed navigation menu links, thanks to @editorgit
-        
-        0.2.5
-        ~~~~~
-        
-        - It's now possible to use slugs for dashboards instead of those indexes in ``CONTROLCENTER_DASHBOARDS``.
-          The old behaviour is supported too.
-        
-        0.2.4
-        ~~~~~
-        
-        - It's compatible with django 1.8—2.1 now
-        - Custom app name can be passed to ``ControlCenter`` class
-        
-        0.2.3
-        ~~~~~
-        - Updated column grid, thanks to @pauloxnet.
-        - Grammar fixes, thanks to @danielquinn.
-        - It's should be possible now to use a custom dashboard view with a custom template.
-        
-        0.2.2
-        ~~~~~
-        - ``dashboard.html`` now extends ``admin/base_site.html`` instead of ``admin/base.html``
-          in order to display *branding* block. Thanks to @chadgh.
-        - Updated ``jsonify`` tag filter, thanks to @k8n.
-        
-        0.2.1
-        ~~~~~
-        - Django 1.10 support. Tested in tox *only*.
-        - Updated the SingleBarChart example, thanks to @greeve.
-        
-        0.2.0
-        ~~~~~
-        - Unlimited dashboards support.
-        - Configuration constructor is moved to a separate project -- django-pkgconf_. It's a dependency now.
-        
-        0.1.2
-        ~~~~~
-        - Chart ``i`` series color fix. Thanks to @uncleNight.
-        - Docs. Finally.
-        
-        0.1.1
-        ~~~~~
-        - Better responsive experience.
-        
-        0.1.0
-        ~~~~~
-        - First public release.
-        
-        .. _Chartist.js: http://gionkunz.github.io/chartist-js/
-        .. _Masonry.js:  http://masonry.desandro.com/
-        .. _Sortable.js: http://github.hubspot.com/sortable/docs/welcome/
-        .. _Django-admin: https://docs.djangoproject.com/en/stable/ref/contrib/admin/
-        .. _django-pkgconf: https://github.com/byashimov/django-pkgconf
-        .. _docs: http://django-controlcenter.readthedocs.io/en/latest/
-        
 Keywords: django admin dashboard
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -235,7 +22,225 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 1
 Classifier: Framework :: Django :: 2
 Classifier: Framework :: Django :: 3
 Classifier: Framework :: Django :: 4
+License-File: LICENSE
+
+Welcome to django-controlcenter!
+================================
+
+Get all your project models on one single page with charts and whistles.
+
+.. image:: https://cloud.githubusercontent.com/assets/1560043/14309295/b8c9aad0-fc05-11e5-96d0-44293d2d07ff.png
+    :alt: django-controlcenter
+
+Attention!
+----------
+
+Unfortunately, I have no time to add new features.
+Please make PR if you need one:
+
+- branch from master
+- provide tests
+- add docs
+- update changelog
+
+That's it.
+
+
+Rationale
+---------
+
+Django-admin_ is a great tool to control your project activity: new orders, comments, replies, users, feedback -- everything is here. The only struggle is to switch between all those pages constantly just to check them out for new entries.
+
+With django-controlcenter you can have all of your models on one single page and build beautiful charts with Chartist.js_. Actually they don't even have to be a django models, get your data from wherever you want: RDBMS, NOSQL, text file or even from an external web-page, it doesn't matter.
+
+
+Quickstart
+----------
+
+Install django-controlcenter:
+
+.. code-block:: console
+
+    pip install -U django-controlcenter
+
+Create a dashboard file with unlimited number of widgets and dashboards:
+
+.. code-block:: python
+
+    from controlcenter import Dashboard, widgets
+    from project.app.models import Model
+
+    class ModelItemList(widgets.ItemList):
+        model = Model
+        list_display = ('pk', 'field')
+
+    class MyDashboard(Dashboard):
+        widgets = (
+            ModelItemList,
+        )
+
+Update settings file:
+
+.. code-block:: python
+
+    INSTALLED_APPS = [
+        ...
+        'controlcenter',
+        ...
+    ]
+
+    CONTROLCENTER_DASHBOARDS = (
+        ('mydash', 'project.dashboards.MyDashboard'),
+    )
+
+Plug in urls:
+
+.. code-block:: python
+
+    from django.urls import path
+    from django.contrib import admin
+    from controlcenter.views import controlcenter
+
+    urlpatterns = [
+        path('admin/dashboard/', controlcenter.urls),
+        path('admin/', admin.site.urls),
+        ...
+    ]
+
+Open ``/admin/dashboard/mydash/`` in browser.
+
+
+Documentation
+-------------
+
+Check out the docs_ for more complete examples.
+
+
+Compatibility
+-------------
+
+.. image:: https://travis-ci.org/byashimov/django-controlcenter.svg?branch=master
+    :alt: Build Status
+    :target: https://travis-ci.org/byashimov/django-controlcenter
+
+.. image:: https://codecov.io/github/byashimov/django-controlcenter/coverage.svg?branch=master
+    :alt: Codecov
+    :target: https://codecov.io/github/byashimov/django-controlcenter?branch=master
+
+Tested on py 3.5—3.10 and django 1—4.
+
+
+Credits
+-------
+
+This project uses Chartist.js_, Masonry.js_ and Sortable.js_.
+
+
+Changelog
+---------
+
+0.3.2
+~~~~~
+
+- Automatically redirect the main app url to the first dashboard. Thanks to @fabiocaccamo.
+
+0.3.1
+~~~~~
+
+- Support django 4.0, python 3.10. Thanks to @mick88.
+- Fixed LineChart example. Thanks to @virtosubogdan.
+
+0.3.0
+~~~~~
+
+- Support django 3.0
+- Python 3 only
+
+0.2.9
+~~~~~
+
+- ``chartist-plugin-pointlabels`` temporary fix
+- Added sorting triangles to ``ItemList``
+- ``ItemList`` header is now always displayed regardless sortability
+- Other misc improvements
+
+Thanks to @minusf.
+
+0.2.8
+~~~~~
+
+- Fixed ``key_value_list.html`` widget template syntax error.
+- Fixed attribute typo ``widget.chartist.point_labels -> point_lables``.
+
+Thanks to @minusf.
+
+0.2.7
+~~~~~
+
+- New ``TimeSeriesChart`` widget. Thanks to @pjdelport.
+- New "simple" widgets: ``ValueList`` and ``KeyValueList``. Thanks to @tonysyu.
+- Bunch of fixes and improvements, thanks again to @pjdelport.
+
+
+0.2.6
+~~~~~
+
+- Fixed navigation menu links, thanks to @editorgit
+
+0.2.5
+~~~~~
+
+- It's now possible to use slugs for dashboards instead of those indexes in ``CONTROLCENTER_DASHBOARDS``.
+  The old behaviour is supported too.
+
+0.2.4
+~~~~~
+
+- It's compatible with django 1.8—2.1 now
+- Custom app name can be passed to ``ControlCenter`` class
+
+0.2.3
+~~~~~
+- Updated column grid, thanks to @pauloxnet.
+- Grammar fixes, thanks to @danielquinn.
+- It's should be possible now to use a custom dashboard view with a custom template.
+
+0.2.2
+~~~~~
+- ``dashboard.html`` now extends ``admin/base_site.html`` instead of ``admin/base.html``
+  in order to display *branding* block. Thanks to @chadgh.
+- Updated ``jsonify`` tag filter, thanks to @k8n.
+
+0.2.1
+~~~~~
+- Django 1.10 support. Tested in tox *only*.
+- Updated the SingleBarChart example, thanks to @greeve.
+
+0.2.0
+~~~~~
+- Unlimited dashboards support.
+- Configuration constructor is moved to a separate project -- django-pkgconf_. It's a dependency now.
+
+0.1.2
+~~~~~
+- Chart ``i`` series color fix. Thanks to @uncleNight.
+- Docs. Finally.
+
+0.1.1
+~~~~~
+- Better responsive experience.
+
+0.1.0
+~~~~~
+- First public release.
+
+.. _Chartist.js: http://gionkunz.github.io/chartist-js/
+.. _Masonry.js:  http://masonry.desandro.com/
+.. _Sortable.js: http://github.hubspot.com/sortable/docs/welcome/
+.. _Django-admin: https://docs.djangoproject.com/en/stable/ref/contrib/admin/
+.. _django-pkgconf: https://github.com/byashimov/django-pkgconf
+.. _docs: http://django-controlcenter.readthedocs.io/en/latest/
```

### Comparing `django-controlcenter-0.3.1/README.rst` & `django-controlcenter-0.3.2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -72,16 +72,16 @@
 .. code-block:: python
 
     from django.urls import path
     from django.contrib import admin
     from controlcenter.views import controlcenter
 
     urlpatterns = [
-        path('admin/', admin.site.urls),
         path('admin/dashboard/', controlcenter.urls),
+        path('admin/', admin.site.urls),
         ...
     ]
 
 Open ``/admin/dashboard/mydash/`` in browser.
 
 
 Documentation
@@ -109,14 +109,19 @@
 
 This project uses Chartist.js_, Masonry.js_ and Sortable.js_.
 
 
 Changelog
 ---------
 
+0.3.2
+~~~~~
+
+- Automatically redirect the main app url to the first dashboard. Thanks to @fabiocaccamo.
+
 0.3.1
 ~~~~~
 
 - Support django 4.0, python 3.10. Thanks to @mick88.
 - Fixed LineChart example. Thanks to @virtosubogdan.
 
 0.3.0
```

### Comparing `django-controlcenter-0.3.1/controlcenter/dashboards.py` & `django-controlcenter-0.3.2/controlcenter/dashboards.py`

 * *Files identical despite different names*

### Comparing `django-controlcenter-0.3.1/controlcenter/static/controlcenter/css/all.css` & `django-controlcenter-0.3.2/controlcenter/static/controlcenter/css/all.css`

 * *Files identical despite different names*

### Comparing `django-controlcenter-0.3.1/controlcenter/static/controlcenter/css/chartist-default-colors.css` & `django-controlcenter-0.3.2/controlcenter/static/controlcenter/css/chartist-default-colors.css`

 * *Files identical despite different names*

### Comparing `django-controlcenter-0.3.1/controlcenter/static/controlcenter/css/chartist-material-colors.css` & `django-controlcenter-0.3.2/controlcenter/static/controlcenter/css/chartist-material-colors.css`

 * *Files identical despite different names*

### Comparing `django-controlcenter-0.3.1/controlcenter/static/controlcenter/css/chartist.css` & `django-controlcenter-0.3.2/controlcenter/static/controlcenter/css/chartist.css`

 * *Files identical despite different names*

### Comparing `django-controlcenter-0.3.1/controlcenter/static/controlcenter/js/chartist/chartist-plugin-pointlabels.min.js` & `django-controlcenter-0.3.2/controlcenter/static/controlcenter/js/chartist/chartist-plugin-pointlabels.min.js`

 * *Files identical despite different names*

### Comparing `django-controlcenter-0.3.1/controlcenter/static/controlcenter/js/chartist/chartist.min.js` & `django-controlcenter-0.3.2/controlcenter/static/controlcenter/js/chartist/chartist.min.js`

 * *Files identical despite different names*

### Comparing `django-controlcenter-0.3.1/controlcenter/static/controlcenter/js/masonry.pkgd.min.js` & `django-controlcenter-0.3.2/controlcenter/static/controlcenter/js/masonry.pkgd.min.js`

 * *Files identical despite different names*

### Comparing `django-controlcenter-0.3.1/controlcenter/static/controlcenter/js/scripts.js` & `django-controlcenter-0.3.2/controlcenter/static/controlcenter/js/scripts.js`

 * *Files identical despite different names*

### Comparing `django-controlcenter-0.3.1/controlcenter/static/controlcenter/js/sortable.min.js` & `django-controlcenter-0.3.2/controlcenter/static/controlcenter/js/sortable.min.js`

 * *Files identical despite different names*

### Comparing `django-controlcenter-0.3.1/controlcenter/stylus/all.styl` & `django-controlcenter-0.3.2/controlcenter/stylus/all.styl`

 * *Files identical despite different names*

### Comparing `django-controlcenter-0.3.1/controlcenter/stylus/mixins.styl` & `django-controlcenter-0.3.2/controlcenter/stylus/mixins.styl`

 * *Files identical despite different names*

### Comparing `django-controlcenter-0.3.1/controlcenter/templates/controlcenter/dashboard.html` & `django-controlcenter-0.3.2/controlcenter/templates/controlcenter/dashboard.html`

 * *Files identical despite different names*

### Comparing `django-controlcenter-0.3.1/controlcenter/templates/controlcenter/widgets/chart.html` & `django-controlcenter-0.3.2/controlcenter/templates/controlcenter/widgets/chart.html`

 * *Files identical despite different names*

### Comparing `django-controlcenter-0.3.1/controlcenter/templates/controlcenter/widgets/contrib/key_value_list.html` & `django-controlcenter-0.3.2/controlcenter/templates/controlcenter/widgets/contrib/key_value_list.html`

 * *Files identical despite different names*

### Comparing `django-controlcenter-0.3.1/controlcenter/templates/controlcenter/widgets/contrib/value_list.html` & `django-controlcenter-0.3.2/controlcenter/templates/controlcenter/widgets/contrib/value_list.html`

 * *Files identical despite different names*

### Comparing `django-controlcenter-0.3.1/controlcenter/templates/controlcenter/widgets/itemlist.html` & `django-controlcenter-0.3.2/controlcenter/templates/controlcenter/widgets/itemlist.html`

 * *Files identical despite different names*

### Comparing `django-controlcenter-0.3.1/controlcenter/templatetags/controlcenter_tags.py` & `django-controlcenter-0.3.2/controlcenter/templatetags/controlcenter_tags.py`

 * *Files identical despite different names*

### Comparing `django-controlcenter-0.3.1/controlcenter/utils.py` & `django-controlcenter-0.3.2/controlcenter/utils.py`

 * *Files identical despite different names*

### Comparing `django-controlcenter-0.3.1/controlcenter/views.py` & `django-controlcenter-0.3.2/controlcenter/views.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from collections import OrderedDict
 
 from django.contrib import admin
 from django.contrib.admin.views.decorators import staff_member_required
 from django.core.exceptions import ImproperlyConfigured
-from django.http import Http404
+from django.http import Http404, HttpResponseRedirect
+from django.shortcuts import redirect
 from django.utils.decorators import method_decorator
 from django.utils.functional import cached_property
 from django.utils.module_loading import import_string
 from django.views.generic.base import TemplateView
 
 from . import app_settings
 
@@ -24,14 +25,15 @@
         self.view_class = view_class
 
     def get_view(self):
         return self.view_class.as_view(controlcenter=self)
 
     def get_urls(self):
         urlpatterns = [
+            re_path(r'^$', self.get_view(), name='index'),
             re_path(r'^(?P<pk>\w+)/$', self.get_view(), name='dashboard'),
         ]
         return urlpatterns
 
     @property
     def urls(self):
         return self.get_urls(), 'controlcenter', self.name
@@ -43,19 +45,25 @@
     template_name = 'controlcenter/dashboard.html'
 
     @method_decorator(staff_member_required)
     def dispatch(self, *args, **kwargs):
         return super(DashboardView, self).dispatch(*args, **kwargs)
 
     def get(self, request, *args, **kwargs):
-        pk = str(self.kwargs['pk'])
+        pk = self.kwargs.get('pk')
+
+        # Redirects to the first dashboard if pk is not provided
+        if not pk and self.dashboards:
+            dashboard = next(iter(self.dashboards.values()))
+            return redirect(dashboard.get_absolute_url())
+
         try:
             self.dashboard = self.dashboards[pk]
         except KeyError:
-            raise Http404('Dashboard not found.')
+            raise Http404(f'Dashboard "{pk}" not found')
         return super(DashboardView, self).get(request, *args, **kwargs)
 
     @cached_property
     def dashboards(self):
         dashboards = OrderedDict()
         for slug, path in enumerate(app_settings.DASHBOARDS):
             if isinstance(path, (list, tuple)):
```

### Comparing `django-controlcenter-0.3.1/controlcenter/widgets/charts.py` & `django-controlcenter-0.3.2/controlcenter/widgets/charts.py`

 * *Files identical despite different names*

### Comparing `django-controlcenter-0.3.1/controlcenter/widgets/contrib/simple.py` & `django-controlcenter-0.3.2/controlcenter/widgets/contrib/simple.py`

 * *Files identical despite different names*

### Comparing `django-controlcenter-0.3.1/controlcenter/widgets/core.py` & `django-controlcenter-0.3.2/controlcenter/widgets/core.py`

 * *Files identical despite different names*

### Comparing `django-controlcenter-0.3.1/django_controlcenter.egg-info/PKG-INFO` & `django-controlcenter-0.3.2/django_controlcenter.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,229 +1,16 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: django-controlcenter
-Version: 0.3.1
+Version: 0.3.2
 Summary: Set of widgets to build dashboards for your Django-project.
 Home-page: https://github.com/byashimov/django-controlcenter
 Author: Murad Byashimov
 Author-email: byashimov@gmail.com
 License: BSD
-Description: Welcome to django-controlcenter!
-        ================================
-        
-        Get all your project models on one single page with charts and whistles.
-        
-        .. image:: https://cloud.githubusercontent.com/assets/1560043/14309295/b8c9aad0-fc05-11e5-96d0-44293d2d07ff.png
-            :alt: django-controlcenter
-        
-        Attention!
-        ----------
-        
-        Unfortunately, I have no time to add new features.
-        Please make PR if you need one:
-        
-        - branch from master
-        - provide tests
-        - add docs
-        - update changelog
-        
-        That's it.
-        
-        
-        Rationale
-        ---------
-        
-        Django-admin_ is a great tool to control your project activity: new orders, comments, replies, users, feedback -- everything is here. The only struggle is to switch between all those pages constantly just to check them out for new entries.
-        
-        With django-controlcenter you can have all of your models on one single page and build beautiful charts with Chartist.js_. Actually they don't even have to be a django models, get your data from wherever you want: RDBMS, NOSQL, text file or even from an external web-page, it doesn't matter.
-        
-        
-        Quickstart
-        ----------
-        
-        Install django-controlcenter:
-        
-        .. code-block:: console
-        
-            pip install -U django-controlcenter
-        
-        Create a dashboard file with unlimited number of widgets and dashboards:
-        
-        .. code-block:: python
-        
-            from controlcenter import Dashboard, widgets
-            from project.app.models import Model
-        
-            class ModelItemList(widgets.ItemList):
-                model = Model
-                list_display = ('pk', 'field')
-        
-            class MyDashboard(Dashboard):
-                widgets = (
-                    ModelItemList,
-                )
-        
-        Update settings file:
-        
-        .. code-block:: python
-        
-            INSTALLED_APPS = [
-                ...
-                'controlcenter',
-                ...
-            ]
-        
-            CONTROLCENTER_DASHBOARDS = (
-                ('mydash', 'project.dashboards.MyDashboard'),
-            )
-        
-        Plug in urls:
-        
-        .. code-block:: python
-        
-            from django.urls import path
-            from django.contrib import admin
-            from controlcenter.views import controlcenter
-        
-            urlpatterns = [
-                path('admin/', admin.site.urls),
-                path('admin/dashboard/', controlcenter.urls),
-                ...
-            ]
-        
-        Open ``/admin/dashboard/mydash/`` in browser.
-        
-        
-        Documentation
-        -------------
-        
-        Check out the docs_ for more complete examples.
-        
-        
-        Compatibility
-        -------------
-        
-        .. image:: https://travis-ci.org/byashimov/django-controlcenter.svg?branch=master
-            :alt: Build Status
-            :target: https://travis-ci.org/byashimov/django-controlcenter
-        
-        .. image:: https://codecov.io/github/byashimov/django-controlcenter/coverage.svg?branch=master
-            :alt: Codecov
-            :target: https://codecov.io/github/byashimov/django-controlcenter?branch=master
-        
-        Tested on py 3.5—3.10 and django 1—4.
-        
-        
-        Credits
-        -------
-        
-        This project uses Chartist.js_, Masonry.js_ and Sortable.js_.
-        
-        
-        Changelog
-        ---------
-        
-        0.3.1
-        ~~~~~
-        
-        - Support django 4.0, python 3.10. Thanks to @mick88.
-        - Fixed LineChart example. Thanks to @virtosubogdan.
-        
-        0.3.0
-        ~~~~~
-        
-        - Support django 3.0
-        - Python 3 only
-        
-        0.2.9
-        ~~~~~
-        
-        - ``chartist-plugin-pointlabels`` temporary fix
-        - Added sorting triangles to ``ItemList``
-        - ``ItemList`` header is now always displayed regardless sortability
-        - Other misc improvements
-        
-        Thanks to @minusf.
-        
-        0.2.8
-        ~~~~~
-        
-        - Fixed ``key_value_list.html`` widget template syntax error.
-        - Fixed attribute typo ``widget.chartist.point_labels -> point_lables``.
-        
-        Thanks to @minusf.
-        
-        0.2.7
-        ~~~~~
-        
-        - New ``TimeSeriesChart`` widget. Thanks to @pjdelport.
-        - New "simple" widgets: ``ValueList`` and ``KeyValueList``. Thanks to @tonysyu.
-        - Bunch of fixes and improvements, thanks again to @pjdelport.
-        
-        
-        0.2.6
-        ~~~~~
-        
-        - Fixed navigation menu links, thanks to @editorgit
-        
-        0.2.5
-        ~~~~~
-        
-        - It's now possible to use slugs for dashboards instead of those indexes in ``CONTROLCENTER_DASHBOARDS``.
-          The old behaviour is supported too.
-        
-        0.2.4
-        ~~~~~
-        
-        - It's compatible with django 1.8—2.1 now
-        - Custom app name can be passed to ``ControlCenter`` class
-        
-        0.2.3
-        ~~~~~
-        - Updated column grid, thanks to @pauloxnet.
-        - Grammar fixes, thanks to @danielquinn.
-        - It's should be possible now to use a custom dashboard view with a custom template.
-        
-        0.2.2
-        ~~~~~
-        - ``dashboard.html`` now extends ``admin/base_site.html`` instead of ``admin/base.html``
-          in order to display *branding* block. Thanks to @chadgh.
-        - Updated ``jsonify`` tag filter, thanks to @k8n.
-        
-        0.2.1
-        ~~~~~
-        - Django 1.10 support. Tested in tox *only*.
-        - Updated the SingleBarChart example, thanks to @greeve.
-        
-        0.2.0
-        ~~~~~
-        - Unlimited dashboards support.
-        - Configuration constructor is moved to a separate project -- django-pkgconf_. It's a dependency now.
-        
-        0.1.2
-        ~~~~~
-        - Chart ``i`` series color fix. Thanks to @uncleNight.
-        - Docs. Finally.
-        
-        0.1.1
-        ~~~~~
-        - Better responsive experience.
-        
-        0.1.0
-        ~~~~~
-        - First public release.
-        
-        .. _Chartist.js: http://gionkunz.github.io/chartist-js/
-        .. _Masonry.js:  http://masonry.desandro.com/
-        .. _Sortable.js: http://github.hubspot.com/sortable/docs/welcome/
-        .. _Django-admin: https://docs.djangoproject.com/en/stable/ref/contrib/admin/
-        .. _django-pkgconf: https://github.com/byashimov/django-pkgconf
-        .. _docs: http://django-controlcenter.readthedocs.io/en/latest/
-        
 Keywords: django admin dashboard
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -235,7 +22,225 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 1
 Classifier: Framework :: Django :: 2
 Classifier: Framework :: Django :: 3
 Classifier: Framework :: Django :: 4
+License-File: LICENSE
+
+Welcome to django-controlcenter!
+================================
+
+Get all your project models on one single page with charts and whistles.
+
+.. image:: https://cloud.githubusercontent.com/assets/1560043/14309295/b8c9aad0-fc05-11e5-96d0-44293d2d07ff.png
+    :alt: django-controlcenter
+
+Attention!
+----------
+
+Unfortunately, I have no time to add new features.
+Please make PR if you need one:
+
+- branch from master
+- provide tests
+- add docs
+- update changelog
+
+That's it.
+
+
+Rationale
+---------
+
+Django-admin_ is a great tool to control your project activity: new orders, comments, replies, users, feedback -- everything is here. The only struggle is to switch between all those pages constantly just to check them out for new entries.
+
+With django-controlcenter you can have all of your models on one single page and build beautiful charts with Chartist.js_. Actually they don't even have to be a django models, get your data from wherever you want: RDBMS, NOSQL, text file or even from an external web-page, it doesn't matter.
+
+
+Quickstart
+----------
+
+Install django-controlcenter:
+
+.. code-block:: console
+
+    pip install -U django-controlcenter
+
+Create a dashboard file with unlimited number of widgets and dashboards:
+
+.. code-block:: python
+
+    from controlcenter import Dashboard, widgets
+    from project.app.models import Model
+
+    class ModelItemList(widgets.ItemList):
+        model = Model
+        list_display = ('pk', 'field')
+
+    class MyDashboard(Dashboard):
+        widgets = (
+            ModelItemList,
+        )
+
+Update settings file:
+
+.. code-block:: python
+
+    INSTALLED_APPS = [
+        ...
+        'controlcenter',
+        ...
+    ]
+
+    CONTROLCENTER_DASHBOARDS = (
+        ('mydash', 'project.dashboards.MyDashboard'),
+    )
+
+Plug in urls:
+
+.. code-block:: python
+
+    from django.urls import path
+    from django.contrib import admin
+    from controlcenter.views import controlcenter
+
+    urlpatterns = [
+        path('admin/dashboard/', controlcenter.urls),
+        path('admin/', admin.site.urls),
+        ...
+    ]
+
+Open ``/admin/dashboard/mydash/`` in browser.
+
+
+Documentation
+-------------
+
+Check out the docs_ for more complete examples.
+
+
+Compatibility
+-------------
+
+.. image:: https://travis-ci.org/byashimov/django-controlcenter.svg?branch=master
+    :alt: Build Status
+    :target: https://travis-ci.org/byashimov/django-controlcenter
+
+.. image:: https://codecov.io/github/byashimov/django-controlcenter/coverage.svg?branch=master
+    :alt: Codecov
+    :target: https://codecov.io/github/byashimov/django-controlcenter?branch=master
+
+Tested on py 3.5—3.10 and django 1—4.
+
+
+Credits
+-------
+
+This project uses Chartist.js_, Masonry.js_ and Sortable.js_.
+
+
+Changelog
+---------
+
+0.3.2
+~~~~~
+
+- Automatically redirect the main app url to the first dashboard. Thanks to @fabiocaccamo.
+
+0.3.1
+~~~~~
+
+- Support django 4.0, python 3.10. Thanks to @mick88.
+- Fixed LineChart example. Thanks to @virtosubogdan.
+
+0.3.0
+~~~~~
+
+- Support django 3.0
+- Python 3 only
+
+0.2.9
+~~~~~
+
+- ``chartist-plugin-pointlabels`` temporary fix
+- Added sorting triangles to ``ItemList``
+- ``ItemList`` header is now always displayed regardless sortability
+- Other misc improvements
+
+Thanks to @minusf.
+
+0.2.8
+~~~~~
+
+- Fixed ``key_value_list.html`` widget template syntax error.
+- Fixed attribute typo ``widget.chartist.point_labels -> point_lables``.
+
+Thanks to @minusf.
+
+0.2.7
+~~~~~
+
+- New ``TimeSeriesChart`` widget. Thanks to @pjdelport.
+- New "simple" widgets: ``ValueList`` and ``KeyValueList``. Thanks to @tonysyu.
+- Bunch of fixes and improvements, thanks again to @pjdelport.
+
+
+0.2.6
+~~~~~
+
+- Fixed navigation menu links, thanks to @editorgit
+
+0.2.5
+~~~~~
+
+- It's now possible to use slugs for dashboards instead of those indexes in ``CONTROLCENTER_DASHBOARDS``.
+  The old behaviour is supported too.
+
+0.2.4
+~~~~~
+
+- It's compatible with django 1.8—2.1 now
+- Custom app name can be passed to ``ControlCenter`` class
+
+0.2.3
+~~~~~
+- Updated column grid, thanks to @pauloxnet.
+- Grammar fixes, thanks to @danielquinn.
+- It's should be possible now to use a custom dashboard view with a custom template.
+
+0.2.2
+~~~~~
+- ``dashboard.html`` now extends ``admin/base_site.html`` instead of ``admin/base.html``
+  in order to display *branding* block. Thanks to @chadgh.
+- Updated ``jsonify`` tag filter, thanks to @k8n.
+
+0.2.1
+~~~~~
+- Django 1.10 support. Tested in tox *only*.
+- Updated the SingleBarChart example, thanks to @greeve.
+
+0.2.0
+~~~~~
+- Unlimited dashboards support.
+- Configuration constructor is moved to a separate project -- django-pkgconf_. It's a dependency now.
+
+0.1.2
+~~~~~
+- Chart ``i`` series color fix. Thanks to @uncleNight.
+- Docs. Finally.
+
+0.1.1
+~~~~~
+- Better responsive experience.
+
+0.1.0
+~~~~~
+- First public release.
+
+.. _Chartist.js: http://gionkunz.github.io/chartist-js/
+.. _Masonry.js:  http://masonry.desandro.com/
+.. _Sortable.js: http://github.hubspot.com/sortable/docs/welcome/
+.. _Django-admin: https://docs.djangoproject.com/en/stable/ref/contrib/admin/
+.. _django-pkgconf: https://github.com/byashimov/django-pkgconf
+.. _docs: http://django-controlcenter.readthedocs.io/en/latest/
```

### Comparing `django-controlcenter-0.3.1/django_controlcenter.egg-info/SOURCES.txt` & `django-controlcenter-0.3.2/django_controlcenter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-controlcenter-0.3.1/setup.py` & `django-controlcenter-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.rst', 'r') as f:
     long_description = f.read()
 
 setup(
     name='django-controlcenter',
-    version='0.3.1',
+    version='0.3.2',
     description='Set of widgets to build dashboards for your Django-project.',
     long_description=long_description,
     url='https://github.com/byashimov/django-controlcenter',
     author='Murad Byashimov',
     author_email='byashimov@gmail.com',
     packages=find_packages(
         exclude=['controlcenter.stylus', 'controlcenter.images']),
```

### Comparing `django-controlcenter-0.3.1/test_project/settings.py` & `django-controlcenter-0.3.2/test_project/settings.py`

 * *Files identical despite different names*

### Comparing `django-controlcenter-0.3.1/test_project/test_models.py` & `django-controlcenter-0.3.2/test_project/test_models.py`

 * *Files identical despite different names*

### Comparing `django-controlcenter-0.3.1/tests/test_app_settings.py` & `django-controlcenter-0.3.2/tests/test_app_settings.py`

 * *Files identical despite different names*

### Comparing `django-controlcenter-0.3.1/tests/test_base.py` & `django-controlcenter-0.3.2/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `django-controlcenter-0.3.1/tests/test_dashboards.py` & `django-controlcenter-0.3.2/tests/test_dashboards.py`

 * *Files 8% similar despite different names*

```diff
@@ -118,7 +118,22 @@
                 'href="/admin/dashboard/baz/">Non empty dashboard</a>',
             )
 
             content = response.content.decode()
             for chunk in expected:
                 # fixme: use subtest someday
                 self.assertInHTML(chunk, content)
+
+    def test_redirect_to_first_dashboard(self):
+        self.client.login(username='superuser', password='superpassword')
+        dashboards = (
+            ('foo', 'dashboards.EmptyDashboard'),
+            ('bar', 'dashboards.EmptyDashboard'),
+            ('baz', 'dashboards.EmptyDashboard'),
+        )
+        with self.settings(CONTROLCENTER_DASHBOARDS=dashboards):
+            url = reverse('controlcenter:index')
+            self.assertEqual(url, '/admin/dashboard/')
+            expected_url = reverse('controlcenter:dashboard', kwargs={'pk':'foo'})
+            self.assertEqual(expected_url, '/admin/dashboard/foo/')
+            response = self.client.get(url)
+            self.assertRedirects(response, expected_url)
```

### Comparing `django-controlcenter-0.3.1/tests/test_templatetags.py` & `django-controlcenter-0.3.2/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `django-controlcenter-0.3.1/tests/test_utils.py` & `django-controlcenter-0.3.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django-controlcenter-0.3.1/tests/test_widgets_charts.py` & `django-controlcenter-0.3.2/tests/test_widgets_charts.py`

 * *Files identical despite different names*

### Comparing `django-controlcenter-0.3.1/tests/test_widgets_core.py` & `django-controlcenter-0.3.2/tests/test_widgets_core.py`

 * *Files identical despite different names*

### Comparing `django-controlcenter-0.3.1/tests/test_widgets_simple.py` & `django-controlcenter-0.3.2/tests/test_widgets_simple.py`

 * *Files identical despite different names*

