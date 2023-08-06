# Comparing `tmp/poxy-0.9.0.tar.gz` & `tmp/poxy-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poxy-0.9.0.tar", last modified: Mon Oct  3 06:37:03 2022, max compression
+gzip compressed data, was "poxy-0.9.1.tar", last modified: Tue Oct  4 09:51:45 2022, max compression
```

## Comparing `poxy-0.9.0.tar` & `poxy-0.9.1.tar`

### file list

```diff
@@ -1,194 +1,194 @@
-drwxrwxrwx   0        0        0        0 2022-10-03 06:37:03.564770 poxy-0.9.0/
--rw-rw-rw-   0        0        0     1064 2022-09-26 12:08:35.000000 poxy-0.9.0/LICENSE.txt
--rw-rw-rw-   0        0        0    13773 2022-10-03 06:37:03.564770 poxy-0.9.0/PKG-INFO
--rw-rw-rw-   0        0        0     6995 2022-10-03 06:32:28.000000 poxy-0.9.0/README.md
-drwxrwxrwx   0        0        0        0 2022-10-03 06:37:03.047438 poxy-0.9.0/poxy/
--rw-rw-rw-   0        0        0      499 2022-09-26 12:08:35.000000 poxy-0.9.0/poxy/__init__.py
--rw-rw-rw-   0        0        0      398 2022-09-26 12:08:35.000000 poxy-0.9.0/poxy/__main__.py
--rw-rw-rw-   0        0        0     5796 2022-09-29 08:39:11.000000 poxy-0.9.0/poxy/css.py
-drwxrwxrwx   0        0        0        0 2022-10-03 06:37:03.279428 poxy-0.9.0/poxy/data/
--rw-rw-rw-   0        0        0  2153881 2022-09-26 12:08:35.000000 poxy-0.9.0/poxy/data/cppreference-doxygen-web.tag.xml
-drwxrwxrwx   0        0        0        0 2022-10-03 06:37:03.332837 poxy-0.9.0/poxy/data/css/
--rw-rw-rw-   0        0        0     4644 2022-09-28 12:52:00.000000 poxy-0.9.0/poxy/data/css/m-special.css
--rw-rw-rw-   0        0        0     4186 2022-09-28 12:52:00.000000 poxy-0.9.0/poxy/data/css/m-theme-dark.css
--rw-rw-rw-   0        0        0     8035 2022-10-01 07:33:55.000000 poxy-0.9.0/poxy/data/css/m-theme-light.css
--rw-rw-rw-   0        0        0     8784 2022-10-01 07:43:34.000000 poxy-0.9.0/poxy/data/css/poxy-overrides.css
--rw-rw-rw-   0        0        0     8617 2022-09-28 12:52:00.000000 poxy-0.9.0/poxy/data/css/poxy-pygments.css
--rw-rw-rw-   0        0        0      804 2022-09-28 12:52:00.000000 poxy-0.9.0/poxy/data/css/poxy-theme-dark.css
--rw-rw-rw-   0        0        0     1253 2022-09-29 08:39:11.000000 poxy-0.9.0/poxy/data/css/poxy-theme-light.css
--rw-rw-rw-   0        0        0     1377 2022-09-28 12:52:00.000000 poxy-0.9.0/poxy/data/css/poxy.css
-drwxrwxrwx   0        0        0        0 2022-10-03 06:37:03.348523 poxy-0.9.0/poxy/data/generated/
--rw-rw-rw-   0        0        0    15568 2022-10-02 08:02:44.000000 poxy-0.9.0/poxy/data/generated/6aa12ac32e258617e37a0030dc54f789b894368b.css
--rw-rw-rw-   0        0        0   250504 2022-10-01 07:50:45.000000 poxy-0.9.0/poxy/data/generated/emoji.json
-drwxrwxrwx   0        0        0        0 2022-10-03 06:37:03.433158 poxy-0.9.0/poxy/data/generated/fonts/
--rw-rw-rw-   0        0        0      908 2022-10-02 08:02:51.000000 poxy-0.9.0/poxy/data/generated/fonts/6xK1dSBYKcSV-LCoeQqfX1RYOo3qPZ7jsDJT9g.woff2
--rw-rw-rw-   0        0        0     1212 2022-10-02 08:02:51.000000 poxy-0.9.0/poxy/data/generated/fonts/6xK1dSBYKcSV-LCoeQqfX1RYOo3qPZ7ksDJT9g.woff2
--rw-rw-rw-   0        0        0    12580 2022-10-02 08:02:52.000000 poxy-0.9.0/poxy/data/generated/fonts/6xK1dSBYKcSV-LCoeQqfX1RYOo3qPZ7nsDI.woff2
--rw-rw-rw-   0        0        0     4248 2022-10-02 08:02:52.000000 poxy-0.9.0/poxy/data/generated/fonts/6xK1dSBYKcSV-LCoeQqfX1RYOo3qPZ7osDJT9g.woff2
--rw-rw-rw-   0        0        0    11792 2022-10-02 08:02:52.000000 poxy-0.9.0/poxy/data/generated/fonts/6xK1dSBYKcSV-LCoeQqfX1RYOo3qPZ7psDJT9g.woff2
--rw-rw-rw-   0        0        0     1028 2022-10-02 08:02:51.000000 poxy-0.9.0/poxy/data/generated/fonts/6xK1dSBYKcSV-LCoeQqfX1RYOo3qPZ7qsDJT9g.woff2
--rw-rw-rw-   0        0        0      908 2022-10-02 08:02:51.000000 poxy-0.9.0/poxy/data/generated/fonts/6xK1dSBYKcSV-LCoeQqfX1RYOo3qPZ7rsDJT9g.woff2
--rw-rw-rw-   0        0        0     4216 2022-10-02 08:02:56.000000 poxy-0.9.0/poxy/data/generated/fonts/6xK3dSBYKcSV-LCoeQqfX1RYOo3qN67lqDY.woff2
--rw-rw-rw-   0        0        0     6004 2022-10-02 08:02:55.000000 poxy-0.9.0/poxy/data/generated/fonts/6xK3dSBYKcSV-LCoeQqfX1RYOo3qNK7lqDY.woff2
--rw-rw-rw-   0        0        0     5024 2022-10-02 08:02:54.000000 poxy-0.9.0/poxy/data/generated/fonts/6xK3dSBYKcSV-LCoeQqfX1RYOo3qNa7lqDY.woff2
--rw-rw-rw-   0        0        0    11792 2022-10-02 08:02:56.000000 poxy-0.9.0/poxy/data/generated/fonts/6xK3dSBYKcSV-LCoeQqfX1RYOo3qNq7lqDY.woff2
--rw-rw-rw-   0        0        0     7036 2022-10-02 08:02:55.000000 poxy-0.9.0/poxy/data/generated/fonts/6xK3dSBYKcSV-LCoeQqfX1RYOo3qO67lqDY.woff2
--rw-rw-rw-   0        0        0    13036 2022-10-02 08:02:56.000000 poxy-0.9.0/poxy/data/generated/fonts/6xK3dSBYKcSV-LCoeQqfX1RYOo3qOK7l.woff2
--rw-rw-rw-   0        0        0     7448 2022-10-02 08:02:55.000000 poxy-0.9.0/poxy/data/generated/fonts/6xK3dSBYKcSV-LCoeQqfX1RYOo3qPK7lqDY.woff2
--rw-rw-rw-   0        0        0      892 2022-10-02 08:02:53.000000 poxy-0.9.0/poxy/data/generated/fonts/6xKwdSBYKcSV-LCoeQqfX1RYOo3qPZY4lCdg18Smxg.woff2
--rw-rw-rw-   0        0        0     1108 2022-10-02 08:02:53.000000 poxy-0.9.0/poxy/data/generated/fonts/6xKwdSBYKcSV-LCoeQqfX1RYOo3qPZY4lCdh18Smxg.woff2
--rw-rw-rw-   0        0        0    11924 2022-10-02 08:02:54.000000 poxy-0.9.0/poxy/data/generated/fonts/6xKwdSBYKcSV-LCoeQqfX1RYOo3qPZY4lCdi18Smxg.woff2
--rw-rw-rw-   0        0        0     4252 2022-10-02 08:02:54.000000 poxy-0.9.0/poxy/data/generated/fonts/6xKwdSBYKcSV-LCoeQqfX1RYOo3qPZY4lCdj18Smxg.woff2
--rw-rw-rw-   0        0        0      892 2022-10-02 08:02:53.000000 poxy-0.9.0/poxy/data/generated/fonts/6xKwdSBYKcSV-LCoeQqfX1RYOo3qPZY4lCdo18Smxg.woff2
--rw-rw-rw-   0        0        0    12564 2022-10-02 08:02:54.000000 poxy-0.9.0/poxy/data/generated/fonts/6xKwdSBYKcSV-LCoeQqfX1RYOo3qPZY4lCds18Q.woff2
--rw-rw-rw-   0        0        0     1192 2022-10-02 08:02:53.000000 poxy-0.9.0/poxy/data/generated/fonts/6xKwdSBYKcSV-LCoeQqfX1RYOo3qPZY4lCdv18Smxg.woff2
--rw-rw-rw-   0        0        0     7428 2022-10-02 08:02:56.000000 poxy-0.9.0/poxy/data/generated/fonts/6xKydSBYKcSV-LCoeQqfX1RYOo3i54rwkxduz8A.woff2
--rw-rw-rw-   0        0        0     6912 2022-10-02 08:02:57.000000 poxy-0.9.0/poxy/data/generated/fonts/6xKydSBYKcSV-LCoeQqfX1RYOo3i54rwlBduz8A.woff2
--rw-rw-rw-   0        0        0    13052 2022-10-02 08:02:57.000000 poxy-0.9.0/poxy/data/generated/fonts/6xKydSBYKcSV-LCoeQqfX1RYOo3i54rwlxdu.woff2
--rw-rw-rw-   0        0        0     4112 2022-10-02 08:02:57.000000 poxy-0.9.0/poxy/data/generated/fonts/6xKydSBYKcSV-LCoeQqfX1RYOo3i54rwmBduz8A.woff2
--rw-rw-rw-   0        0        0    11696 2022-10-02 08:02:57.000000 poxy-0.9.0/poxy/data/generated/fonts/6xKydSBYKcSV-LCoeQqfX1RYOo3i54rwmRduz8A.woff2
--rw-rw-rw-   0        0        0     5016 2022-10-02 08:02:56.000000 poxy-0.9.0/poxy/data/generated/fonts/6xKydSBYKcSV-LCoeQqfX1RYOo3i54rwmhduz8A.woff2
--rw-rw-rw-   0        0        0     5944 2022-10-02 08:02:56.000000 poxy-0.9.0/poxy/data/generated/fonts/6xKydSBYKcSV-LCoeQqfX1RYOo3i54rwmxduz8A.woff2
--rw-rw-rw-   0        0        0    18580 2022-10-02 08:02:50.000000 poxy-0.9.0/poxy/data/generated/fonts/HI_SiYsKILxRpg3hIP6sJ7fM7PqlM-vWjMY.woff2
--rw-rw-rw-   0        0        0     8568 2022-10-02 08:02:49.000000 poxy-0.9.0/poxy/data/generated/fonts/HI_SiYsKILxRpg3hIP6sJ7fM7PqlMOvWjMY.woff2
--rw-rw-rw-   0        0        0     2932 2022-10-02 08:02:49.000000 poxy-0.9.0/poxy/data/generated/fonts/HI_SiYsKILxRpg3hIP6sJ7fM7PqlMevWjMY.woff2
--rw-rw-rw-   0        0        0     6484 2022-10-02 08:02:50.000000 poxy-0.9.0/poxy/data/generated/fonts/HI_SiYsKILxRpg3hIP6sJ7fM7PqlMuvWjMY.woff2
--rw-rw-rw-   0        0        0    13948 2022-10-02 08:02:49.000000 poxy-0.9.0/poxy/data/generated/fonts/HI_SiYsKILxRpg3hIP6sJ7fM7PqlOevWjMY.woff2
--rw-rw-rw-   0        0        0    19680 2022-10-02 08:02:50.000000 poxy-0.9.0/poxy/data/generated/fonts/HI_SiYsKILxRpg3hIP6sJ7fM7PqlPevW.woff2
--rw-rw-rw-   0        0        0    10236 2022-10-02 08:02:49.000000 poxy-0.9.0/poxy/data/generated/fonts/HI_SiYsKILxRpg3hIP6sJ7fM7PqlPuvWjMY.woff2
--rw-rw-rw-   0        0        0      920 2022-10-02 08:02:44.000000 poxy-0.9.0/poxy/data/generated/fonts/HI_jiYsKILxRpg3hIP6sJ7fM7PqlOPHYvDP_W9O7GQTTbI1bQ10YVJg.woff2
--rw-rw-rw-   0        0        0     9872 2022-10-02 08:02:46.000000 poxy-0.9.0/poxy/data/generated/fonts/HI_jiYsKILxRpg3hIP6sJ7fM7PqlOPHYvDP_W9O7GQTTbI1bQF0YVJg.woff2
--rw-rw-rw-   0        0        0     3668 2022-10-02 08:02:46.000000 poxy-0.9.0/poxy/data/generated/fonts/HI_jiYsKILxRpg3hIP6sJ7fM7PqlOPHYvDP_W9O7GQTTbI1bQV0YVJg.woff2
--rw-rw-rw-   0        0        0      728 2022-10-02 08:02:45.000000 poxy-0.9.0/poxy/data/generated/fonts/HI_jiYsKILxRpg3hIP6sJ7fM7PqlOPHYvDP_W9O7GQTTbI1bQl0YVJg.woff2
--rw-rw-rw-   0        0        0     1036 2022-10-02 08:02:45.000000 poxy-0.9.0/poxy/data/generated/fonts/HI_jiYsKILxRpg3hIP6sJ7fM7PqlOPHYvDP_W9O7GQTTbI1bSl0YVJg.woff2
--rw-rw-rw-   0        0        0      888 2022-10-02 08:02:45.000000 poxy-0.9.0/poxy/data/generated/fonts/HI_jiYsKILxRpg3hIP6sJ7fM7PqlOPHYvDP_W9O7GQTTbI1bTV0YVJg.woff2
--rw-rw-rw-   0        0        0    10404 2022-10-02 08:02:46.000000 poxy-0.9.0/poxy/data/generated/fonts/HI_jiYsKILxRpg3hIP6sJ7fM7PqlOPHYvDP_W9O7GQTTbI1bTl0Y.woff2
--rw-rw-rw-   0        0        0   142513 2022-10-02 08:02:57.000000 poxy-0.9.0/poxy/data/generated/poxy.css
--rw-rw-rw-   0        0        0    72372 2022-09-26 12:08:35.000000 poxy-0.9.0/poxy/data/jquery-3.6.0.slim.min.js
-drwxrwxrwx   0        0        0        0 2022-10-03 06:37:03.433158 poxy-0.9.0/poxy/data/m.css/
--rw-rw-rw-   0        0        0     1117 2022-09-26 11:43:33.000000 poxy-0.9.0/poxy/data/m.css/COPYING
-drwxrwxrwx   0        0        0        0 2022-10-03 06:37:03.433158 poxy-0.9.0/poxy/data/m.css/css/
--rw-rw-rw-   0        0        0    61301 2022-10-03 04:55:43.000000 poxy-0.9.0/poxy/data/m.css/css/m-components.css
--rw-rw-rw-   0        0        0     3332 2022-09-26 11:43:33.000000 poxy-0.9.0/poxy/data/m.css/css/m-debug.css
--rw-rw-rw-   0        0        0    10955 2022-09-26 11:43:33.000000 poxy-0.9.0/poxy/data/m.css/css/m-documentation.css
--rw-rw-rw-   0        0        0    13379 2022-09-26 11:43:33.000000 poxy-0.9.0/poxy/data/m.css/css/m-grid.css
--rw-rw-rw-   0        0        0    31260 2022-09-26 11:43:33.000000 poxy-0.9.0/poxy/data/m.css/css/m-layout.css
--rw-rw-rw-   0        0        0     3345 2022-09-26 11:43:33.000000 poxy-0.9.0/poxy/data/m.css/css/pygments-console.css
--rw-rw-rw-   0        0        0     3919 2022-09-26 11:43:33.000000 poxy-0.9.0/poxy/data/m.css/css/pygments-dark.css
-drwxrwxrwx   0        0        0        0 2022-10-03 06:37:03.448835 poxy-0.9.0/poxy/data/m.css/documentation/
--rw-rw-rw-   0        0        0     1253 2022-09-26 11:43:33.000000 poxy-0.9.0/poxy/data/m.css/documentation/__init__.py
--rw-rw-rw-   0        0        0    36579 2022-09-26 11:43:33.000000 poxy-0.9.0/poxy/data/m.css/documentation/_search.py
--rw-rw-rw-   0        0        0   193996 2022-10-03 06:32:28.000000 poxy-0.9.0/poxy/data/m.css/documentation/doxygen.py
--rw-rw-rw-   0        0        0      380 2022-09-26 11:43:33.000000 poxy-0.9.0/poxy/data/m.css/documentation/favicon-dark.png
--rw-rw-rw-   0        0        0      360 2022-09-26 11:43:33.000000 poxy-0.9.0/poxy/data/m.css/documentation/favicon-light.png
--rw-rw-rw-   0        0        0   128792 2022-09-26 11:43:33.000000 poxy-0.9.0/poxy/data/m.css/documentation/python.py
--rw-rw-rw-   0        0        0    43044 2022-09-26 11:43:33.000000 poxy-0.9.0/poxy/data/m.css/documentation/search.js
-drwxrwxrwx   0        0        0        0 2022-10-03 06:37:03.012646 poxy-0.9.0/poxy/data/m.css/documentation/templates/
-drwxrwxrwx   0        0        0        0 2022-10-03 06:37:03.533486 poxy-0.9.0/poxy/data/m.css/documentation/templates/doxygen/
--rw-rw-rw-   0        0        0     1590 2022-10-03 06:32:28.000000 poxy-0.9.0/poxy/data/m.css/documentation/templates/doxygen/annotated.html
--rw-rw-rw-   0        0        0    22207 2022-10-03 06:32:28.000000 poxy-0.9.0/poxy/data/m.css/documentation/templates/doxygen/base-class-reference.html
--rw-rw-rw-   0        0        0      920 2022-09-26 11:43:33.000000 poxy-0.9.0/poxy/data/m.css/documentation/templates/doxygen/base-index.html
--rw-rw-rw-   0        0        0    11432 2022-10-03 06:32:28.000000 poxy-0.9.0/poxy/data/m.css/documentation/templates/doxygen/base-reference.html
--rw-rw-rw-   0        0        0     9029 2022-09-26 11:43:33.000000 poxy-0.9.0/poxy/data/m.css/documentation/templates/doxygen/base.html
--rw-rw-rw-   0        0        0       43 2022-09-26 11:43:33.000000 poxy-0.9.0/poxy/data/m.css/documentation/templates/doxygen/class.html
--rw-rw-rw-   0        0        0       42 2022-10-03 06:32:28.000000 poxy-0.9.0/poxy/data/m.css/documentation/templates/doxygen/concept.html
--rw-rw-rw-   0        0        0     1247 2022-10-03 06:32:28.000000 poxy-0.9.0/poxy/data/m.css/documentation/templates/doxygen/concepts.html
--rw-rw-rw-   0        0        0     1952 2022-09-26 11:43:33.000000 poxy-0.9.0/poxy/data/m.css/documentation/templates/doxygen/details-define.html
--rw-rw-rw-   0        0        0     2530 2022-09-26 11:43:33.000000 poxy-0.9.0/poxy/data/m.css/documentation/templates/doxygen/details-enum.html
--rw-rw-rw-   0        0        0     6776 2022-09-26 11:43:33.000000 poxy-0.9.0/poxy/data/m.css/documentation/templates/doxygen/details-func.html
--rw-rw-rw-   0        0        0     3093 2022-09-26 11:43:33.000000 poxy-0.9.0/poxy/data/m.css/documentation/templates/doxygen/details-typedef.html
--rw-rw-rw-   0        0        0     2690 2022-09-26 11:43:33.000000 poxy-0.9.0/poxy/data/m.css/documentation/templates/doxygen/details-var.html
--rw-rw-rw-   0        0        0      617 2022-09-26 11:43:33.000000 poxy-0.9.0/poxy/data/m.css/documentation/templates/doxygen/dir.html
--rw-rw-rw-   0        0        0      971 2022-09-26 11:43:33.000000 poxy-0.9.0/poxy/data/m.css/documentation/templates/doxygen/entry-class.html
--rw-rw-rw-   0        0        0      816 2022-10-03 06:32:28.000000 poxy-0.9.0/poxy/data/m.css/documentation/templates/doxygen/entry-concept.html
--rw-rw-rw-   0        0        0      806 2022-09-26 11:43:33.000000 poxy-0.9.0/poxy/data/m.css/documentation/templates/doxygen/entry-define.html
--rw-rw-rw-   0        0        0      266 2022-09-26 11:43:33.000000 poxy-0.9.0/poxy/data/m.css/documentation/templates/doxygen/entry-dir.html
--rw-rw-rw-   0        0        0     1186 2022-09-26 11:43:33.000000 poxy-0.9.0/poxy/data/m.css/documentation/templates/doxygen/entry-enum.html
--rw-rw-rw-   0        0        0      267 2022-09-26 11:43:33.000000 poxy-0.9.0/poxy/data/m.css/documentation/templates/doxygen/entry-file.html
--rw-rw-rw-   0        0        0     2724 2022-09-26 11:43:33.000000 poxy-0.9.0/poxy/data/m.css/documentation/templates/doxygen/entry-func.html
--rw-rw-rw-   0        0        0      283 2022-09-26 11:43:33.000000 poxy-0.9.0/poxy/data/m.css/documentation/templates/doxygen/entry-module.html
--rw-rw-rw-   0        0        0      396 2022-09-26 11:43:33.000000 poxy-0.9.0/poxy/data/m.css/documentation/templates/doxygen/entry-namespace.html
--rw-rw-rw-   0        0        0     1147 2022-09-26 11:43:33.000000 poxy-0.9.0/poxy/data/m.css/documentation/templates/doxygen/entry-typedef.html
--rw-rw-rw-   0        0        0     1182 2022-09-26 11:43:33.000000 poxy-0.9.0/poxy/data/m.css/documentation/templates/doxygen/entry-var.html
--rw-rw-rw-   0        0        0     1603 2022-09-26 11:43:33.000000 poxy-0.9.0/poxy/data/m.css/documentation/templates/doxygen/example.html
--rw-rw-rw-   0        0        0      605 2022-09-26 11:43:33.000000 poxy-0.9.0/poxy/data/m.css/documentation/templates/doxygen/file.html
--rw-rw-rw-   0        0        0     1112 2022-09-26 11:43:33.000000 poxy-0.9.0/poxy/data/m.css/documentation/templates/doxygen/files.html
--rw-rw-rw-   0        0        0      567 2022-09-26 11:43:33.000000 poxy-0.9.0/poxy/data/m.css/documentation/templates/doxygen/group.html
--rw-rw-rw-   0        0        0     1052 2022-09-26 11:43:33.000000 poxy-0.9.0/poxy/data/m.css/documentation/templates/doxygen/modules.html
--rw-rw-rw-   0        0        0      957 2022-09-26 11:43:33.000000 poxy-0.9.0/poxy/data/m.css/documentation/templates/doxygen/namespace.html
--rw-rw-rw-   0        0        0     1318 2022-09-26 11:43:33.000000 poxy-0.9.0/poxy/data/m.css/documentation/templates/doxygen/namespaces.html
--rw-rw-rw-   0        0        0      508 2022-09-26 11:43:33.000000 poxy-0.9.0/poxy/data/m.css/documentation/templates/doxygen/opensearch.xml
--rw-rw-rw-   0        0        0     2395 2022-09-26 11:43:33.000000 poxy-0.9.0/poxy/data/m.css/documentation/templates/doxygen/page.html
--rw-rw-rw-   0        0        0     1019 2022-09-26 11:43:33.000000 poxy-0.9.0/poxy/data/m.css/documentation/templates/doxygen/pages.html
--rw-rw-rw-   0        0        0       43 2022-09-26 11:43:33.000000 poxy-0.9.0/poxy/data/m.css/documentation/templates/doxygen/struct.html
--rw-rw-rw-   0        0        0       43 2022-10-03 03:29:49.000000 poxy-0.9.0/poxy/data/m.css/documentation/templates/doxygen/union.html
-drwxrwxrwx   0        0        0        0 2022-10-03 06:37:03.533486 poxy-0.9.0/poxy/data/m.css/plugins/
--rw-rw-rw-   0        0        0    11935 2022-09-26 11:43:33.000000 poxy-0.9.0/poxy/data/m.css/plugins/ansilexer.py
--rw-rw-rw-   0        0        0     5369 2022-09-26 11:43:33.000000 poxy-0.9.0/poxy/data/m.css/plugins/dot2svg.py
--rw-rw-rw-   0        0        0     5851 2022-09-26 11:43:33.000000 poxy-0.9.0/poxy/data/m.css/plugins/latex2svg.py
--rw-rw-rw-   0        0        0     8367 2022-09-26 11:43:33.000000 poxy-0.9.0/poxy/data/m.css/plugins/latex2svgextra.py
-drwxrwxrwx   0        0        0        0 2022-10-03 06:37:03.564770 poxy-0.9.0/poxy/data/m.css/plugins/m/
--rw-rw-rw-   0        0        0     1340 2022-09-26 11:43:33.000000 poxy-0.9.0/poxy/data/m.css/plugins/m/__init__.py
--rw-rw-rw-   0        0        0     2132 2022-09-26 11:43:33.000000 poxy-0.9.0/poxy/data/m.css/plugins/m/abbr.py
--rw-rw-rw-   0        0        0     3472 2022-09-26 11:43:33.000000 poxy-0.9.0/poxy/data/m.css/plugins/m/alias.py
--rw-rw-rw-   0        0        0    15384 2022-09-26 11:43:33.000000 poxy-0.9.0/poxy/data/m.css/plugins/m/code.py
--rw-rw-rw-   0        0        0    16363 2022-09-26 11:43:33.000000 poxy-0.9.0/poxy/data/m.css/plugins/m/components.py
--rw-rw-rw-   0        0        0     5409 2022-09-26 11:43:33.000000 poxy-0.9.0/poxy/data/m.css/plugins/m/dot.py
--rw-rw-rw-   0        0        0     8549 2022-09-26 11:43:33.000000 poxy-0.9.0/poxy/data/m.css/plugins/m/dox.py
--rw-rw-rw-   0        0        0     3202 2022-09-26 11:43:33.000000 poxy-0.9.0/poxy/data/m.css/plugins/m/filesize.py
--rw-rw-rw-   0        0        0     3471 2022-09-26 11:43:33.000000 poxy-0.9.0/poxy/data/m.css/plugins/m/gh.py
--rw-rw-rw-   0        0        0     3633 2022-09-26 11:43:33.000000 poxy-0.9.0/poxy/data/m.css/plugins/m/gl.py
--rw-rw-rw-   0        0        0    34464 2022-09-26 11:43:33.000000 poxy-0.9.0/poxy/data/m.css/plugins/m/htmlsanity.py
--rw-rw-rw-   0        0        0    13459 2022-09-26 11:43:33.000000 poxy-0.9.0/poxy/data/m.css/plugins/m/images.py
--rw-rw-rw-   0        0        0     2269 2022-09-26 11:43:33.000000 poxy-0.9.0/poxy/data/m.css/plugins/m/link.py
--rw-rw-rw-   0        0        0     6997 2022-09-26 11:43:33.000000 poxy-0.9.0/poxy/data/m.css/plugins/m/math.py
--rw-rw-rw-   0        0        0     3606 2022-09-26 11:43:33.000000 poxy-0.9.0/poxy/data/m.css/plugins/m/metadata.py
--rw-rw-rw-   0        0        0    15346 2022-09-26 11:43:33.000000 poxy-0.9.0/poxy/data/m.css/plugins/m/plots.py
--rw-rw-rw-   0        0        0     4276 2022-09-26 11:43:33.000000 poxy-0.9.0/poxy/data/m.css/plugins/m/qr.py
--rw-rw-rw-   0        0        0    31668 2022-09-26 11:43:33.000000 poxy-0.9.0/poxy/data/m.css/plugins/m/sphinx.py
--rw-rw-rw-   0        0        0     3176 2022-09-26 11:43:34.000000 poxy-0.9.0/poxy/data/m.css/plugins/m/vk.py
--rw-rw-rw-   0        0        0     1658 2022-09-26 12:08:35.000000 poxy-0.9.0/poxy/data/poxy-badge-c++03.svg
--rw-rw-rw-   0        0        0     1658 2022-09-26 12:08:35.000000 poxy-0.9.0/poxy/data/poxy-badge-c++11.svg
--rw-rw-rw-   0        0        0     1658 2022-09-26 12:08:35.000000 poxy-0.9.0/poxy/data/poxy-badge-c++14.svg
--rw-rw-rw-   0        0        0     1658 2022-09-26 12:08:35.000000 poxy-0.9.0/poxy/data/poxy-badge-c++17.svg
--rw-rw-rw-   0        0        0     1658 2022-09-26 12:08:35.000000 poxy-0.9.0/poxy/data/poxy-badge-c++20.svg
--rw-rw-rw-   0        0        0     1660 2022-09-26 12:08:35.000000 poxy-0.9.0/poxy/data/poxy-badge-c++23.svg
--rw-rw-rw-   0        0        0     1660 2022-09-26 12:08:35.000000 poxy-0.9.0/poxy/data/poxy-badge-c++26.svg
--rw-rw-rw-   0        0        0     1660 2022-09-26 12:08:35.000000 poxy-0.9.0/poxy/data/poxy-badge-c++29.svg
--rw-rw-rw-   0        0        0     1658 2022-09-26 12:08:35.000000 poxy-0.9.0/poxy/data/poxy-badge-c++98.svg
--rw-rw-rw-   0        0        0      645 2022-09-26 12:08:35.000000 poxy-0.9.0/poxy/data/poxy-badge-license-apache_2.svg
--rw-rw-rw-   0        0        0      651 2022-09-26 12:08:35.000000 poxy-0.9.0/poxy/data/poxy-badge-license-bsd_2_clause.svg
--rw-rw-rw-   0        0        0      651 2022-09-26 12:08:35.000000 poxy-0.9.0/poxy/data/poxy-badge-license-bsd_3_clause.svg
--rw-rw-rw-   0        0        0      623 2022-09-26 12:08:35.000000 poxy-0.9.0/poxy/data/poxy-badge-license-gpl.svg
--rw-rw-rw-   0        0        0      636 2022-09-26 12:08:35.000000 poxy-0.9.0/poxy/data/poxy-badge-license-gpl_2.svg
--rw-rw-rw-   0        0        0      636 2022-09-26 12:08:35.000000 poxy-0.9.0/poxy/data/poxy-badge-license-gpl_3.svg
--rw-rw-rw-   0        0        0      626 2022-09-26 12:08:35.000000 poxy-0.9.0/poxy/data/poxy-badge-license-lgpl.svg
--rw-rw-rw-   0        0        0      639 2022-09-26 12:08:35.000000 poxy-0.9.0/poxy/data/poxy-badge-license-lgpl_2.svg
--rw-rw-rw-   0        0        0      639 2022-09-26 12:08:35.000000 poxy-0.9.0/poxy/data/poxy-badge-license-lgpl_2_1.svg
--rw-rw-rw-   0        0        0      639 2022-09-26 12:08:35.000000 poxy-0.9.0/poxy/data/poxy-badge-license-lgpl_3.svg
--rw-rw-rw-   0        0        0      482 2022-09-26 12:08:35.000000 poxy-0.9.0/poxy/data/poxy-badge-license-mit.svg
--rw-rw-rw-   0        0        0      661 2022-09-26 12:08:35.000000 poxy-0.9.0/poxy/data/poxy-icon-github.svg
--rw-rw-rw-   0        0        0      478 2022-09-26 12:08:35.000000 poxy-0.9.0/poxy/data/poxy-icon-gitlab.svg
--rw-rw-rw-   0        0        0     1808 2022-09-26 12:08:35.000000 poxy-0.9.0/poxy/data/poxy-icon-theme.svg
--rw-rw-rw-   0        0        0      896 2022-09-27 02:56:23.000000 poxy-0.9.0/poxy/data/poxy.js
--rw-rw-rw-   0        0        0        6 2022-10-03 06:32:28.000000 poxy-0.9.0/poxy/data/version.txt
--rw-rw-rw-   0        0        0      995 2022-09-27 14:55:42.000000 poxy-0.9.0/poxy/dirs.py
--rw-rw-rw-   0        0        0     6157 2022-09-27 14:55:42.000000 poxy-0.9.0/poxy/doxygen.py
--rw-rw-rw-   0        0        0     2912 2022-09-29 08:39:12.000000 poxy-0.9.0/poxy/emoji.py
--rw-rw-rw-   0        0        0    27131 2022-10-03 06:32:28.000000 poxy-0.9.0/poxy/fixers.py
--rw-rw-rw-   0        0        0     8059 2022-10-03 06:32:28.000000 poxy-0.9.0/poxy/main.py
--rw-rw-rw-   0        0        0    69873 2022-10-03 06:32:28.000000 poxy-0.9.0/poxy/project.py
--rw-rw-rw-   0        0        0     3582 2022-09-29 08:39:12.000000 poxy-0.9.0/poxy/repos.py
--rw-rw-rw-   0        0        0    49709 2022-10-03 06:32:28.000000 poxy-0.9.0/poxy/run.py
--rw-rw-rw-   0        0        0     5955 2022-09-30 00:36:57.000000 poxy-0.9.0/poxy/soup.py
--rw-rw-rw-   0        0        0     1964 2022-10-03 06:32:28.000000 poxy-0.9.0/poxy/svg.py
--rw-rw-rw-   0        0        0     7246 2022-10-03 06:32:28.000000 poxy-0.9.0/poxy/utils.py
-drwxrwxrwx   0        0        0        0 2022-10-03 06:37:03.078680 poxy-0.9.0/poxy.egg-info/
--rw-rw-rw-   0        0        0    13773 2022-10-03 06:37:02.000000 poxy-0.9.0/poxy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     8516 2022-10-03 06:37:02.000000 poxy-0.9.0/poxy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-03 06:37:02.000000 poxy-0.9.0/poxy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       76 2022-10-03 06:37:02.000000 poxy-0.9.0/poxy.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       78 2022-10-03 06:37:02.000000 poxy-0.9.0/poxy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2022-10-03 06:37:02.000000 poxy-0.9.0/poxy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-10-03 06:37:03.564770 poxy-0.9.0/setup.cfg
--rw-rw-rw-   0        0        0     3058 2022-09-30 04:04:10.000000 poxy-0.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2022-10-04 09:51:45.773052 poxy-0.9.1/
+-rw-rw-rw-   0        0        0     1064 2022-09-26 12:08:35.000000 poxy-0.9.1/LICENSE.txt
+-rw-rw-rw-   0        0        0    13945 2022-10-04 09:51:45.773052 poxy-0.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6655 2022-10-04 09:43:20.000000 poxy-0.9.1/README.md
+drwxrwxrwx   0        0        0        0 2022-10-04 09:51:45.433481 poxy-0.9.1/poxy/
+-rw-rw-rw-   0        0        0      499 2022-09-26 12:08:35.000000 poxy-0.9.1/poxy/__init__.py
+-rw-rw-rw-   0        0        0      398 2022-09-26 12:08:35.000000 poxy-0.9.1/poxy/__main__.py
+-rw-rw-rw-   0        0        0     5796 2022-09-29 08:39:11.000000 poxy-0.9.1/poxy/css.py
+drwxrwxrwx   0        0        0        0 2022-10-04 09:51:45.525612 poxy-0.9.1/poxy/data/
+-rw-rw-rw-   0        0        0  2153881 2022-09-26 12:08:35.000000 poxy-0.9.1/poxy/data/cppreference-doxygen-web.tag.xml
+drwxrwxrwx   0        0        0        0 2022-10-04 09:51:45.541250 poxy-0.9.1/poxy/data/css/
+-rw-rw-rw-   0        0        0     4644 2022-09-28 12:52:00.000000 poxy-0.9.1/poxy/data/css/m-special.css
+-rw-rw-rw-   0        0        0     4186 2022-09-28 12:52:00.000000 poxy-0.9.1/poxy/data/css/m-theme-dark.css
+-rw-rw-rw-   0        0        0     8035 2022-10-01 07:33:55.000000 poxy-0.9.1/poxy/data/css/m-theme-light.css
+-rw-rw-rw-   0        0        0     8785 2022-10-04 09:43:20.000000 poxy-0.9.1/poxy/data/css/poxy-overrides.css
+-rw-rw-rw-   0        0        0     8617 2022-09-28 12:52:00.000000 poxy-0.9.1/poxy/data/css/poxy-pygments.css
+-rw-rw-rw-   0        0        0      804 2022-09-28 12:52:00.000000 poxy-0.9.1/poxy/data/css/poxy-theme-dark.css
+-rw-rw-rw-   0        0        0     1253 2022-09-29 08:39:11.000000 poxy-0.9.1/poxy/data/css/poxy-theme-light.css
+-rw-rw-rw-   0        0        0     1377 2022-09-28 12:52:00.000000 poxy-0.9.1/poxy/data/css/poxy.css
+drwxrwxrwx   0        0        0        0 2022-10-04 09:51:45.541250 poxy-0.9.1/poxy/data/generated/
+-rw-rw-rw-   0        0        0    15568 2022-10-04 09:41:31.000000 poxy-0.9.1/poxy/data/generated/6aa12ac32e258617e37a0030dc54f789b894368b.css
+-rw-rw-rw-   0        0        0   250504 2022-10-01 07:50:45.000000 poxy-0.9.1/poxy/data/generated/emoji.json
+drwxrwxrwx   0        0        0        0 2022-10-04 09:51:45.625892 poxy-0.9.1/poxy/data/generated/fonts/
+-rw-rw-rw-   0        0        0      908 2022-10-04 09:41:34.000000 poxy-0.9.1/poxy/data/generated/fonts/6xK1dSBYKcSV-LCoeQqfX1RYOo3qPZ7jsDJT9g.woff2
+-rw-rw-rw-   0        0        0     1212 2022-10-04 09:41:34.000000 poxy-0.9.1/poxy/data/generated/fonts/6xK1dSBYKcSV-LCoeQqfX1RYOo3qPZ7ksDJT9g.woff2
+-rw-rw-rw-   0        0        0    12580 2022-10-04 09:41:35.000000 poxy-0.9.1/poxy/data/generated/fonts/6xK1dSBYKcSV-LCoeQqfX1RYOo3qPZ7nsDI.woff2
+-rw-rw-rw-   0        0        0     4248 2022-10-04 09:41:35.000000 poxy-0.9.1/poxy/data/generated/fonts/6xK1dSBYKcSV-LCoeQqfX1RYOo3qPZ7osDJT9g.woff2
+-rw-rw-rw-   0        0        0    11792 2022-10-04 09:41:35.000000 poxy-0.9.1/poxy/data/generated/fonts/6xK1dSBYKcSV-LCoeQqfX1RYOo3qPZ7psDJT9g.woff2
+-rw-rw-rw-   0        0        0     1028 2022-10-04 09:41:34.000000 poxy-0.9.1/poxy/data/generated/fonts/6xK1dSBYKcSV-LCoeQqfX1RYOo3qPZ7qsDJT9g.woff2
+-rw-rw-rw-   0        0        0      908 2022-10-04 09:41:34.000000 poxy-0.9.1/poxy/data/generated/fonts/6xK1dSBYKcSV-LCoeQqfX1RYOo3qPZ7rsDJT9g.woff2
+-rw-rw-rw-   0        0        0     4216 2022-10-04 09:41:37.000000 poxy-0.9.1/poxy/data/generated/fonts/6xK3dSBYKcSV-LCoeQqfX1RYOo3qN67lqDY.woff2
+-rw-rw-rw-   0        0        0     6004 2022-10-04 09:41:36.000000 poxy-0.9.1/poxy/data/generated/fonts/6xK3dSBYKcSV-LCoeQqfX1RYOo3qNK7lqDY.woff2
+-rw-rw-rw-   0        0        0     5024 2022-10-04 09:41:36.000000 poxy-0.9.1/poxy/data/generated/fonts/6xK3dSBYKcSV-LCoeQqfX1RYOo3qNa7lqDY.woff2
+-rw-rw-rw-   0        0        0    11792 2022-10-04 09:41:37.000000 poxy-0.9.1/poxy/data/generated/fonts/6xK3dSBYKcSV-LCoeQqfX1RYOo3qNq7lqDY.woff2
+-rw-rw-rw-   0        0        0     7036 2022-10-04 09:41:37.000000 poxy-0.9.1/poxy/data/generated/fonts/6xK3dSBYKcSV-LCoeQqfX1RYOo3qO67lqDY.woff2
+-rw-rw-rw-   0        0        0    13036 2022-10-04 09:41:37.000000 poxy-0.9.1/poxy/data/generated/fonts/6xK3dSBYKcSV-LCoeQqfX1RYOo3qOK7l.woff2
+-rw-rw-rw-   0        0        0     7448 2022-10-04 09:41:36.000000 poxy-0.9.1/poxy/data/generated/fonts/6xK3dSBYKcSV-LCoeQqfX1RYOo3qPK7lqDY.woff2
+-rw-rw-rw-   0        0        0      892 2022-10-04 09:41:35.000000 poxy-0.9.1/poxy/data/generated/fonts/6xKwdSBYKcSV-LCoeQqfX1RYOo3qPZY4lCdg18Smxg.woff2
+-rw-rw-rw-   0        0        0     1108 2022-10-04 09:41:35.000000 poxy-0.9.1/poxy/data/generated/fonts/6xKwdSBYKcSV-LCoeQqfX1RYOo3qPZY4lCdh18Smxg.woff2
+-rw-rw-rw-   0        0        0    11924 2022-10-04 09:41:36.000000 poxy-0.9.1/poxy/data/generated/fonts/6xKwdSBYKcSV-LCoeQqfX1RYOo3qPZY4lCdi18Smxg.woff2
+-rw-rw-rw-   0        0        0     4252 2022-10-04 09:41:36.000000 poxy-0.9.1/poxy/data/generated/fonts/6xKwdSBYKcSV-LCoeQqfX1RYOo3qPZY4lCdj18Smxg.woff2
+-rw-rw-rw-   0        0        0      892 2022-10-04 09:41:35.000000 poxy-0.9.1/poxy/data/generated/fonts/6xKwdSBYKcSV-LCoeQqfX1RYOo3qPZY4lCdo18Smxg.woff2
+-rw-rw-rw-   0        0        0    12564 2022-10-04 09:41:36.000000 poxy-0.9.1/poxy/data/generated/fonts/6xKwdSBYKcSV-LCoeQqfX1RYOo3qPZY4lCds18Q.woff2
+-rw-rw-rw-   0        0        0     1192 2022-10-04 09:41:36.000000 poxy-0.9.1/poxy/data/generated/fonts/6xKwdSBYKcSV-LCoeQqfX1RYOo3qPZY4lCdv18Smxg.woff2
+-rw-rw-rw-   0        0        0     7428 2022-10-04 09:41:37.000000 poxy-0.9.1/poxy/data/generated/fonts/6xKydSBYKcSV-LCoeQqfX1RYOo3i54rwkxduz8A.woff2
+-rw-rw-rw-   0        0        0     6912 2022-10-04 09:41:38.000000 poxy-0.9.1/poxy/data/generated/fonts/6xKydSBYKcSV-LCoeQqfX1RYOo3i54rwlBduz8A.woff2
+-rw-rw-rw-   0        0        0    13052 2022-10-04 09:41:38.000000 poxy-0.9.1/poxy/data/generated/fonts/6xKydSBYKcSV-LCoeQqfX1RYOo3i54rwlxdu.woff2
+-rw-rw-rw-   0        0        0     4112 2022-10-04 09:41:38.000000 poxy-0.9.1/poxy/data/generated/fonts/6xKydSBYKcSV-LCoeQqfX1RYOo3i54rwmBduz8A.woff2
+-rw-rw-rw-   0        0        0    11696 2022-10-04 09:41:38.000000 poxy-0.9.1/poxy/data/generated/fonts/6xKydSBYKcSV-LCoeQqfX1RYOo3i54rwmRduz8A.woff2
+-rw-rw-rw-   0        0        0     5016 2022-10-04 09:41:37.000000 poxy-0.9.1/poxy/data/generated/fonts/6xKydSBYKcSV-LCoeQqfX1RYOo3i54rwmhduz8A.woff2
+-rw-rw-rw-   0        0        0     5944 2022-10-04 09:41:38.000000 poxy-0.9.1/poxy/data/generated/fonts/6xKydSBYKcSV-LCoeQqfX1RYOo3i54rwmxduz8A.woff2
+-rw-rw-rw-   0        0        0    18580 2022-10-04 09:41:34.000000 poxy-0.9.1/poxy/data/generated/fonts/HI_SiYsKILxRpg3hIP6sJ7fM7PqlM-vWjMY.woff2
+-rw-rw-rw-   0        0        0     8568 2022-10-04 09:41:33.000000 poxy-0.9.1/poxy/data/generated/fonts/HI_SiYsKILxRpg3hIP6sJ7fM7PqlMOvWjMY.woff2
+-rw-rw-rw-   0        0        0     2932 2022-10-04 09:41:33.000000 poxy-0.9.1/poxy/data/generated/fonts/HI_SiYsKILxRpg3hIP6sJ7fM7PqlMevWjMY.woff2
+-rw-rw-rw-   0        0        0     6484 2022-10-04 09:41:34.000000 poxy-0.9.1/poxy/data/generated/fonts/HI_SiYsKILxRpg3hIP6sJ7fM7PqlMuvWjMY.woff2
+-rw-rw-rw-   0        0        0    13948 2022-10-04 09:41:33.000000 poxy-0.9.1/poxy/data/generated/fonts/HI_SiYsKILxRpg3hIP6sJ7fM7PqlOevWjMY.woff2
+-rw-rw-rw-   0        0        0    19680 2022-10-04 09:41:34.000000 poxy-0.9.1/poxy/data/generated/fonts/HI_SiYsKILxRpg3hIP6sJ7fM7PqlPevW.woff2
+-rw-rw-rw-   0        0        0    10236 2022-10-04 09:41:33.000000 poxy-0.9.1/poxy/data/generated/fonts/HI_SiYsKILxRpg3hIP6sJ7fM7PqlPuvWjMY.woff2
+-rw-rw-rw-   0        0        0      920 2022-10-04 09:41:31.000000 poxy-0.9.1/poxy/data/generated/fonts/HI_jiYsKILxRpg3hIP6sJ7fM7PqlOPHYvDP_W9O7GQTTbI1bQ10YVJg.woff2
+-rw-rw-rw-   0        0        0     9872 2022-10-04 09:41:32.000000 poxy-0.9.1/poxy/data/generated/fonts/HI_jiYsKILxRpg3hIP6sJ7fM7PqlOPHYvDP_W9O7GQTTbI1bQF0YVJg.woff2
+-rw-rw-rw-   0        0        0     3668 2022-10-04 09:41:32.000000 poxy-0.9.1/poxy/data/generated/fonts/HI_jiYsKILxRpg3hIP6sJ7fM7PqlOPHYvDP_W9O7GQTTbI1bQV0YVJg.woff2
+-rw-rw-rw-   0        0        0      728 2022-10-04 09:41:31.000000 poxy-0.9.1/poxy/data/generated/fonts/HI_jiYsKILxRpg3hIP6sJ7fM7PqlOPHYvDP_W9O7GQTTbI1bQl0YVJg.woff2
+-rw-rw-rw-   0        0        0     1036 2022-10-04 09:41:31.000000 poxy-0.9.1/poxy/data/generated/fonts/HI_jiYsKILxRpg3hIP6sJ7fM7PqlOPHYvDP_W9O7GQTTbI1bSl0YVJg.woff2
+-rw-rw-rw-   0        0        0      888 2022-10-04 09:41:31.000000 poxy-0.9.1/poxy/data/generated/fonts/HI_jiYsKILxRpg3hIP6sJ7fM7PqlOPHYvDP_W9O7GQTTbI1bTV0YVJg.woff2
+-rw-rw-rw-   0        0        0    10404 2022-10-04 09:41:32.000000 poxy-0.9.1/poxy/data/generated/fonts/HI_jiYsKILxRpg3hIP6sJ7fM7PqlOPHYvDP_W9O7GQTTbI1bTl0Y.woff2
+-rw-rw-rw-   0        0        0   142523 2022-10-04 09:43:20.000000 poxy-0.9.1/poxy/data/generated/poxy.css
+-rw-rw-rw-   0        0        0    72372 2022-09-26 12:08:35.000000 poxy-0.9.1/poxy/data/jquery-3.6.0.slim.min.js
+drwxrwxrwx   0        0        0        0 2022-10-04 09:51:45.625892 poxy-0.9.1/poxy/data/m.css/
+-rw-rw-rw-   0        0        0     1117 2022-09-26 11:43:33.000000 poxy-0.9.1/poxy/data/m.css/COPYING
+drwxrwxrwx   0        0        0        0 2022-10-04 09:51:45.641528 poxy-0.9.1/poxy/data/m.css/css/
+-rw-rw-rw-   0        0        0    61301 2022-10-03 01:49:55.000000 poxy-0.9.1/poxy/data/m.css/css/m-components.css
+-rw-rw-rw-   0        0        0     3332 2022-09-26 11:43:33.000000 poxy-0.9.1/poxy/data/m.css/css/m-debug.css
+-rw-rw-rw-   0        0        0    10955 2022-09-26 11:43:33.000000 poxy-0.9.1/poxy/data/m.css/css/m-documentation.css
+-rw-rw-rw-   0        0        0    13379 2022-09-26 11:43:33.000000 poxy-0.9.1/poxy/data/m.css/css/m-grid.css
+-rw-rw-rw-   0        0        0    31260 2022-09-26 11:43:33.000000 poxy-0.9.1/poxy/data/m.css/css/m-layout.css
+-rw-rw-rw-   0        0        0     3345 2022-09-26 11:43:33.000000 poxy-0.9.1/poxy/data/m.css/css/pygments-console.css
+-rw-rw-rw-   0        0        0     3919 2022-09-26 11:43:33.000000 poxy-0.9.1/poxy/data/m.css/css/pygments-dark.css
+drwxrwxrwx   0        0        0        0 2022-10-04 09:51:45.657168 poxy-0.9.1/poxy/data/m.css/documentation/
+-rw-rw-rw-   0        0        0     1253 2022-09-26 11:43:33.000000 poxy-0.9.1/poxy/data/m.css/documentation/__init__.py
+-rw-rw-rw-   0        0        0    36579 2022-09-26 11:43:33.000000 poxy-0.9.1/poxy/data/m.css/documentation/_search.py
+-rw-rw-rw-   0        0        0   193996 2022-10-03 03:35:53.000000 poxy-0.9.1/poxy/data/m.css/documentation/doxygen.py
+-rw-rw-rw-   0        0        0      380 2022-09-26 11:43:33.000000 poxy-0.9.1/poxy/data/m.css/documentation/favicon-dark.png
+-rw-rw-rw-   0        0        0      360 2022-09-26 11:43:33.000000 poxy-0.9.1/poxy/data/m.css/documentation/favicon-light.png
+-rw-rw-rw-   0        0        0   128792 2022-09-26 11:43:33.000000 poxy-0.9.1/poxy/data/m.css/documentation/python.py
+-rw-rw-rw-   0        0        0    43044 2022-09-26 11:43:33.000000 poxy-0.9.1/poxy/data/m.css/documentation/search.js
+drwxrwxrwx   0        0        0        0 2022-10-04 09:51:45.403437 poxy-0.9.1/poxy/data/m.css/documentation/templates/
+drwxrwxrwx   0        0        0        0 2022-10-04 09:51:45.726170 poxy-0.9.1/poxy/data/m.css/documentation/templates/doxygen/
+-rw-rw-rw-   0        0        0     1590 2022-10-03 03:35:53.000000 poxy-0.9.1/poxy/data/m.css/documentation/templates/doxygen/annotated.html
+-rw-rw-rw-   0        0        0    22207 2022-10-03 03:35:53.000000 poxy-0.9.1/poxy/data/m.css/documentation/templates/doxygen/base-class-reference.html
+-rw-rw-rw-   0        0        0      920 2022-09-26 11:43:33.000000 poxy-0.9.1/poxy/data/m.css/documentation/templates/doxygen/base-index.html
+-rw-rw-rw-   0        0        0    11432 2022-10-03 03:35:53.000000 poxy-0.9.1/poxy/data/m.css/documentation/templates/doxygen/base-reference.html
+-rw-rw-rw-   0        0        0     9029 2022-09-26 11:43:33.000000 poxy-0.9.1/poxy/data/m.css/documentation/templates/doxygen/base.html
+-rw-rw-rw-   0        0        0       43 2022-09-26 11:43:33.000000 poxy-0.9.1/poxy/data/m.css/documentation/templates/doxygen/class.html
+-rw-rw-rw-   0        0        0       42 2022-10-03 01:50:25.000000 poxy-0.9.1/poxy/data/m.css/documentation/templates/doxygen/concept.html
+-rw-rw-rw-   0        0        0     1247 2022-10-03 03:35:53.000000 poxy-0.9.1/poxy/data/m.css/documentation/templates/doxygen/concepts.html
+-rw-rw-rw-   0        0        0     1952 2022-09-26 11:43:33.000000 poxy-0.9.1/poxy/data/m.css/documentation/templates/doxygen/details-define.html
+-rw-rw-rw-   0        0        0     2530 2022-09-26 11:43:33.000000 poxy-0.9.1/poxy/data/m.css/documentation/templates/doxygen/details-enum.html
+-rw-rw-rw-   0        0        0     6776 2022-09-26 11:43:33.000000 poxy-0.9.1/poxy/data/m.css/documentation/templates/doxygen/details-func.html
+-rw-rw-rw-   0        0        0     3093 2022-09-26 11:43:33.000000 poxy-0.9.1/poxy/data/m.css/documentation/templates/doxygen/details-typedef.html
+-rw-rw-rw-   0        0        0     2690 2022-09-26 11:43:33.000000 poxy-0.9.1/poxy/data/m.css/documentation/templates/doxygen/details-var.html
+-rw-rw-rw-   0        0        0      617 2022-09-26 11:43:33.000000 poxy-0.9.1/poxy/data/m.css/documentation/templates/doxygen/dir.html
+-rw-rw-rw-   0        0        0      971 2022-09-26 11:43:33.000000 poxy-0.9.1/poxy/data/m.css/documentation/templates/doxygen/entry-class.html
+-rw-rw-rw-   0        0        0      816 2022-10-03 01:50:25.000000 poxy-0.9.1/poxy/data/m.css/documentation/templates/doxygen/entry-concept.html
+-rw-rw-rw-   0        0        0      806 2022-09-26 11:43:33.000000 poxy-0.9.1/poxy/data/m.css/documentation/templates/doxygen/entry-define.html
+-rw-rw-rw-   0        0        0      266 2022-09-26 11:43:33.000000 poxy-0.9.1/poxy/data/m.css/documentation/templates/doxygen/entry-dir.html
+-rw-rw-rw-   0        0        0     1186 2022-09-26 11:43:33.000000 poxy-0.9.1/poxy/data/m.css/documentation/templates/doxygen/entry-enum.html
+-rw-rw-rw-   0        0        0      267 2022-09-26 11:43:33.000000 poxy-0.9.1/poxy/data/m.css/documentation/templates/doxygen/entry-file.html
+-rw-rw-rw-   0        0        0     2724 2022-09-26 11:43:33.000000 poxy-0.9.1/poxy/data/m.css/documentation/templates/doxygen/entry-func.html
+-rw-rw-rw-   0        0        0      283 2022-09-26 11:43:33.000000 poxy-0.9.1/poxy/data/m.css/documentation/templates/doxygen/entry-module.html
+-rw-rw-rw-   0        0        0      396 2022-09-26 11:43:33.000000 poxy-0.9.1/poxy/data/m.css/documentation/templates/doxygen/entry-namespace.html
+-rw-rw-rw-   0        0        0     1147 2022-09-26 11:43:33.000000 poxy-0.9.1/poxy/data/m.css/documentation/templates/doxygen/entry-typedef.html
+-rw-rw-rw-   0        0        0     1182 2022-09-26 11:43:33.000000 poxy-0.9.1/poxy/data/m.css/documentation/templates/doxygen/entry-var.html
+-rw-rw-rw-   0        0        0     1603 2022-09-26 11:43:33.000000 poxy-0.9.1/poxy/data/m.css/documentation/templates/doxygen/example.html
+-rw-rw-rw-   0        0        0      605 2022-09-26 11:43:33.000000 poxy-0.9.1/poxy/data/m.css/documentation/templates/doxygen/file.html
+-rw-rw-rw-   0        0        0     1112 2022-09-26 11:43:33.000000 poxy-0.9.1/poxy/data/m.css/documentation/templates/doxygen/files.html
+-rw-rw-rw-   0        0        0      567 2022-09-26 11:43:33.000000 poxy-0.9.1/poxy/data/m.css/documentation/templates/doxygen/group.html
+-rw-rw-rw-   0        0        0     1052 2022-09-26 11:43:33.000000 poxy-0.9.1/poxy/data/m.css/documentation/templates/doxygen/modules.html
+-rw-rw-rw-   0        0        0      966 2022-10-04 09:43:20.000000 poxy-0.9.1/poxy/data/m.css/documentation/templates/doxygen/namespace.html
+-rw-rw-rw-   0        0        0     1318 2022-09-26 11:43:33.000000 poxy-0.9.1/poxy/data/m.css/documentation/templates/doxygen/namespaces.html
+-rw-rw-rw-   0        0        0      508 2022-09-26 11:43:33.000000 poxy-0.9.1/poxy/data/m.css/documentation/templates/doxygen/opensearch.xml
+-rw-rw-rw-   0        0        0     2395 2022-09-26 11:43:33.000000 poxy-0.9.1/poxy/data/m.css/documentation/templates/doxygen/page.html
+-rw-rw-rw-   0        0        0     1019 2022-09-26 11:43:33.000000 poxy-0.9.1/poxy/data/m.css/documentation/templates/doxygen/pages.html
+-rw-rw-rw-   0        0        0       43 2022-09-26 11:43:33.000000 poxy-0.9.1/poxy/data/m.css/documentation/templates/doxygen/struct.html
+-rw-rw-rw-   0        0        0       42 2022-10-04 02:45:41.000000 poxy-0.9.1/poxy/data/m.css/documentation/templates/doxygen/union.html
+drwxrwxrwx   0        0        0        0 2022-10-04 09:51:45.741809 poxy-0.9.1/poxy/data/m.css/plugins/
+-rw-rw-rw-   0        0        0    11935 2022-09-26 11:43:33.000000 poxy-0.9.1/poxy/data/m.css/plugins/ansilexer.py
+-rw-rw-rw-   0        0        0     5369 2022-09-26 11:43:33.000000 poxy-0.9.1/poxy/data/m.css/plugins/dot2svg.py
+-rw-rw-rw-   0        0        0     5851 2022-09-26 11:43:33.000000 poxy-0.9.1/poxy/data/m.css/plugins/latex2svg.py
+-rw-rw-rw-   0        0        0     8367 2022-09-26 11:43:33.000000 poxy-0.9.1/poxy/data/m.css/plugins/latex2svgextra.py
+drwxrwxrwx   0        0        0        0 2022-10-04 09:51:45.773052 poxy-0.9.1/poxy/data/m.css/plugins/m/
+-rw-rw-rw-   0        0        0     1340 2022-09-26 11:43:33.000000 poxy-0.9.1/poxy/data/m.css/plugins/m/__init__.py
+-rw-rw-rw-   0        0        0     2132 2022-09-26 11:43:33.000000 poxy-0.9.1/poxy/data/m.css/plugins/m/abbr.py
+-rw-rw-rw-   0        0        0     3472 2022-09-26 11:43:33.000000 poxy-0.9.1/poxy/data/m.css/plugins/m/alias.py
+-rw-rw-rw-   0        0        0    15384 2022-09-26 11:43:33.000000 poxy-0.9.1/poxy/data/m.css/plugins/m/code.py
+-rw-rw-rw-   0        0        0    16363 2022-09-26 11:43:33.000000 poxy-0.9.1/poxy/data/m.css/plugins/m/components.py
+-rw-rw-rw-   0        0        0     5409 2022-09-26 11:43:33.000000 poxy-0.9.1/poxy/data/m.css/plugins/m/dot.py
+-rw-rw-rw-   0        0        0     8549 2022-09-26 11:43:33.000000 poxy-0.9.1/poxy/data/m.css/plugins/m/dox.py
+-rw-rw-rw-   0        0        0     3202 2022-09-26 11:43:33.000000 poxy-0.9.1/poxy/data/m.css/plugins/m/filesize.py
+-rw-rw-rw-   0        0        0     3471 2022-09-26 11:43:33.000000 poxy-0.9.1/poxy/data/m.css/plugins/m/gh.py
+-rw-rw-rw-   0        0        0     3633 2022-09-26 11:43:33.000000 poxy-0.9.1/poxy/data/m.css/plugins/m/gl.py
+-rw-rw-rw-   0        0        0    34464 2022-09-26 11:43:33.000000 poxy-0.9.1/poxy/data/m.css/plugins/m/htmlsanity.py
+-rw-rw-rw-   0        0        0    13459 2022-09-26 11:43:33.000000 poxy-0.9.1/poxy/data/m.css/plugins/m/images.py
+-rw-rw-rw-   0        0        0     2269 2022-09-26 11:43:33.000000 poxy-0.9.1/poxy/data/m.css/plugins/m/link.py
+-rw-rw-rw-   0        0        0     6997 2022-09-26 11:43:33.000000 poxy-0.9.1/poxy/data/m.css/plugins/m/math.py
+-rw-rw-rw-   0        0        0     3606 2022-09-26 11:43:33.000000 poxy-0.9.1/poxy/data/m.css/plugins/m/metadata.py
+-rw-rw-rw-   0        0        0    15346 2022-09-26 11:43:33.000000 poxy-0.9.1/poxy/data/m.css/plugins/m/plots.py
+-rw-rw-rw-   0        0        0     4276 2022-09-26 11:43:33.000000 poxy-0.9.1/poxy/data/m.css/plugins/m/qr.py
+-rw-rw-rw-   0        0        0    31668 2022-09-26 11:43:33.000000 poxy-0.9.1/poxy/data/m.css/plugins/m/sphinx.py
+-rw-rw-rw-   0        0        0     3176 2022-09-26 11:43:34.000000 poxy-0.9.1/poxy/data/m.css/plugins/m/vk.py
+-rw-rw-rw-   0        0        0     1658 2022-09-26 12:08:35.000000 poxy-0.9.1/poxy/data/poxy-badge-c++03.svg
+-rw-rw-rw-   0        0        0     1658 2022-09-26 12:08:35.000000 poxy-0.9.1/poxy/data/poxy-badge-c++11.svg
+-rw-rw-rw-   0        0        0     1658 2022-09-26 12:08:35.000000 poxy-0.9.1/poxy/data/poxy-badge-c++14.svg
+-rw-rw-rw-   0        0        0     1658 2022-09-26 12:08:35.000000 poxy-0.9.1/poxy/data/poxy-badge-c++17.svg
+-rw-rw-rw-   0        0        0     1658 2022-09-26 12:08:35.000000 poxy-0.9.1/poxy/data/poxy-badge-c++20.svg
+-rw-rw-rw-   0        0        0     1660 2022-09-26 12:08:35.000000 poxy-0.9.1/poxy/data/poxy-badge-c++23.svg
+-rw-rw-rw-   0        0        0     1660 2022-09-26 12:08:35.000000 poxy-0.9.1/poxy/data/poxy-badge-c++26.svg
+-rw-rw-rw-   0        0        0     1660 2022-09-26 12:08:35.000000 poxy-0.9.1/poxy/data/poxy-badge-c++29.svg
+-rw-rw-rw-   0        0        0     1658 2022-09-26 12:08:35.000000 poxy-0.9.1/poxy/data/poxy-badge-c++98.svg
+-rw-rw-rw-   0        0        0      645 2022-09-26 12:08:35.000000 poxy-0.9.1/poxy/data/poxy-badge-license-apache_2.svg
+-rw-rw-rw-   0        0        0      651 2022-09-26 12:08:35.000000 poxy-0.9.1/poxy/data/poxy-badge-license-bsd_2_clause.svg
+-rw-rw-rw-   0        0        0      651 2022-09-26 12:08:35.000000 poxy-0.9.1/poxy/data/poxy-badge-license-bsd_3_clause.svg
+-rw-rw-rw-   0        0        0      623 2022-09-26 12:08:35.000000 poxy-0.9.1/poxy/data/poxy-badge-license-gpl.svg
+-rw-rw-rw-   0        0        0      636 2022-09-26 12:08:35.000000 poxy-0.9.1/poxy/data/poxy-badge-license-gpl_2.svg
+-rw-rw-rw-   0        0        0      636 2022-09-26 12:08:35.000000 poxy-0.9.1/poxy/data/poxy-badge-license-gpl_3.svg
+-rw-rw-rw-   0        0        0      626 2022-09-26 12:08:35.000000 poxy-0.9.1/poxy/data/poxy-badge-license-lgpl.svg
+-rw-rw-rw-   0        0        0      639 2022-09-26 12:08:35.000000 poxy-0.9.1/poxy/data/poxy-badge-license-lgpl_2.svg
+-rw-rw-rw-   0        0        0      639 2022-09-26 12:08:35.000000 poxy-0.9.1/poxy/data/poxy-badge-license-lgpl_2_1.svg
+-rw-rw-rw-   0        0        0      639 2022-09-26 12:08:35.000000 poxy-0.9.1/poxy/data/poxy-badge-license-lgpl_3.svg
+-rw-rw-rw-   0        0        0      482 2022-09-26 12:08:35.000000 poxy-0.9.1/poxy/data/poxy-badge-license-mit.svg
+-rw-rw-rw-   0        0        0      661 2022-09-26 12:08:35.000000 poxy-0.9.1/poxy/data/poxy-icon-github.svg
+-rw-rw-rw-   0        0        0      478 2022-09-26 12:08:35.000000 poxy-0.9.1/poxy/data/poxy-icon-gitlab.svg
+-rw-rw-rw-   0        0        0     1808 2022-09-26 12:08:35.000000 poxy-0.9.1/poxy/data/poxy-icon-theme.svg
+-rw-rw-rw-   0        0        0      896 2022-10-04 00:41:52.000000 poxy-0.9.1/poxy/data/poxy.js
+-rw-rw-rw-   0        0        0        6 2022-10-03 10:44:52.000000 poxy-0.9.1/poxy/data/version.txt
+-rw-rw-rw-   0        0        0      995 2022-09-27 14:55:42.000000 poxy-0.9.1/poxy/dirs.py
+-rw-rw-rw-   0        0        0     6157 2022-09-27 14:55:42.000000 poxy-0.9.1/poxy/doxygen.py
+-rw-rw-rw-   0        0        0     2912 2022-09-29 08:39:12.000000 poxy-0.9.1/poxy/emoji.py
+-rw-rw-rw-   0        0        0    27748 2022-10-04 09:43:20.000000 poxy-0.9.1/poxy/fixers.py
+-rw-rw-rw-   0        0        0     7895 2022-10-04 09:43:20.000000 poxy-0.9.1/poxy/main.py
+-rw-rw-rw-   0        0        0    70349 2022-10-04 09:43:20.000000 poxy-0.9.1/poxy/project.py
+-rw-rw-rw-   0        0        0     3582 2022-09-29 08:39:12.000000 poxy-0.9.1/poxy/repos.py
+-rw-rw-rw-   0        0        0    49181 2022-10-04 09:43:20.000000 poxy-0.9.1/poxy/run.py
+-rw-rw-rw-   0        0        0     6175 2022-10-04 09:43:20.000000 poxy-0.9.1/poxy/soup.py
+-rw-rw-rw-   0        0        0     2405 2022-10-04 09:43:20.000000 poxy-0.9.1/poxy/svg.py
+-rw-rw-rw-   0        0        0     7318 2022-10-04 09:43:20.000000 poxy-0.9.1/poxy/utils.py
+drwxrwxrwx   0        0        0        0 2022-10-04 09:51:45.464749 poxy-0.9.1/poxy.egg-info/
+-rw-rw-rw-   0        0        0    13945 2022-10-04 09:51:45.000000 poxy-0.9.1/poxy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     8516 2022-10-04 09:51:45.000000 poxy-0.9.1/poxy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-10-04 09:51:45.000000 poxy-0.9.1/poxy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2022-10-04 09:51:45.000000 poxy-0.9.1/poxy.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       78 2022-10-04 09:51:45.000000 poxy-0.9.1/poxy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2022-10-04 09:51:45.000000 poxy-0.9.1/poxy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-10-04 09:51:45.773052 poxy-0.9.1/setup.cfg
+-rw-rw-rw-   0        0        0     3058 2022-09-30 04:04:10.000000 poxy-0.9.1/setup.py
```

### Comparing `poxy-0.9.0/LICENSE.txt` & `poxy-0.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/PKG-INFO` & `poxy-0.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poxy
-Version: 0.9.0
+Version: 0.9.1
 Summary: Documentation generator for C++.
 Home-page: https://github.com/marzer/poxy
 Download-URL: https://pypi.org/project/poxy/
 Author: Mark Gillard
 Author-email: mark.gillard@outlook.com.au
 License: MIT
 Project-URL: Source, https://github.com/marzer/poxy
@@ -84,47 +84,43 @@
 <br><br>
 
 ## Usage
 
 Poxy is a command-line application.
 
 ```
-poxy [-h] [-v] [--doxygen <path>] [--dry] [--threads N] [--version] [--werror] [--xmlonly]
-            [--ppinclude <regex>] [--ppexclude <regex>] [--theme {auto,light,dark,custom}]
-            [config]
+poxy [-h] [-v] [--doxygen <path>] [--ppinclude <regex>] [--ppexclude <regex>]
+     [--theme {auto,light,dark,custom}] [--threads N] [--version] [--werror] [--xmlonly]
+     [config]
 
 Generate fancy C++ documentation.
 
 positional arguments:
   config                path to poxy.toml or a directory containing it (default: .)
 
 options:
   -h, --help            show this help message and exit
   -v, --verbose         enable very noisy diagnostic output
   --doxygen <path>      specify the Doxygen executable to use (default: find on system path)
-  --dry                 do a 'dry run' only, stopping after emitting the effective Doxyfile
-  --threads N           set the number of threads to use (default: automatic)
-  --version             print the version and exit
-  --werror              always treat warnings as errors regardless of config file settings
-  --xmlonly             stop after generating and preprocessing the Doxygen xml
   --ppinclude <regex>   pattern matching HTML file names to post-process (default: all)
   --ppexclude <regex>   pattern matching HTML file names to exclude from post-processing (default: none)
   --theme {auto,light,dark,custom}
                         the CSS theme to use (default: auto)
+  --threads N           set the number of threads to use (default: automatic)
+  --version             print the version and exit
+  --werror              always treat warnings as errors regardless of config file settings
+  --xmlonly             stop after generating and preprocessing the Doxygen xml
 ```
 
 The basic three-step to using Poxy is similar to Doxygen:
 
 1. Create your `poxy.toml` (Poxy's answer to the `Doxyfile`)
 2. Invoke Poxy on it: `poxy path/to/poxy.toml` (or simply `poxy` if the cwd contains the config file)
 3. See your HTML documentation `<cwd>/html`
 
-ℹ&#xFE0F; If there exists a `Doxyfile` or `Doxyfile-mcss` in the same directory as your `poxy.toml` it will be loaded
-first, then the Poxy overrides applied on top of it. Otherwise a 'default' Doxyfile is used as the base.
-
 <br><br>
 
 ## Config file options
 
 For a self-contained `poxy.toml` example to copy and paste from, see [the one used by toml++](https://github.com/marzer/tomlplusplus/blob/master/docs/poxy.toml).
 
 For a full list of options, with full descriptions, schemas and usage examples, see the [Configuration options] wiki page.
@@ -184,14 +180,26 @@
 [c++ feature test macros]: https://en.cppreference.com/w/cpp/feature_test
 [configuration options]: https://github.com/marzer/poxy/wiki/Configuration-options
 [feature request]: https://github.com/marzer/poxy/issues/new
 [`currentcolor`]: https://gomakethings.com/currentcolor-and-svgs
 
 # Changelog
 
+## v0.9.1 - 2022-10-04
+
+-   fixed SVG inlining not preserving original image class attributes
+-   fixed `ValueError` when reading some SVG files
+-   fixed `navbar` option allowing duplicates
+-   fixed custom navbar items always being transformed to lowercase
+-   fixed navbar generating links to empty pages
+-   added `concepts` to the default set of links in `navbar`
+-   added `navbar` values `all` and `default`
+-   reduced I/O churn during HTML post-processing
+-   removed command-line option `dry`
+
 ## v0.9.0 - 2022-10-03
 
 -   added support for C++20 concepts
 
 ## v0.8.2 - 2022-10-01
 
 -   added post-process to inline all local SVGs
```

### Comparing `poxy-0.9.0/README.md` & `poxy-0.9.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -62,47 +62,43 @@
 <br><br>
 
 ## Usage
 
 Poxy is a command-line application.
 
 ```
-poxy [-h] [-v] [--doxygen <path>] [--dry] [--threads N] [--version] [--werror] [--xmlonly]
-            [--ppinclude <regex>] [--ppexclude <regex>] [--theme {auto,light,dark,custom}]
-            [config]
+poxy [-h] [-v] [--doxygen <path>] [--ppinclude <regex>] [--ppexclude <regex>]
+     [--theme {auto,light,dark,custom}] [--threads N] [--version] [--werror] [--xmlonly]
+     [config]
 
 Generate fancy C++ documentation.
 
 positional arguments:
   config                path to poxy.toml or a directory containing it (default: .)
 
 options:
   -h, --help            show this help message and exit
   -v, --verbose         enable very noisy diagnostic output
   --doxygen <path>      specify the Doxygen executable to use (default: find on system path)
-  --dry                 do a 'dry run' only, stopping after emitting the effective Doxyfile
-  --threads N           set the number of threads to use (default: automatic)
-  --version             print the version and exit
-  --werror              always treat warnings as errors regardless of config file settings
-  --xmlonly             stop after generating and preprocessing the Doxygen xml
   --ppinclude <regex>   pattern matching HTML file names to post-process (default: all)
   --ppexclude <regex>   pattern matching HTML file names to exclude from post-processing (default: none)
   --theme {auto,light,dark,custom}
                         the CSS theme to use (default: auto)
+  --threads N           set the number of threads to use (default: automatic)
+  --version             print the version and exit
+  --werror              always treat warnings as errors regardless of config file settings
+  --xmlonly             stop after generating and preprocessing the Doxygen xml
 ```
 
 The basic three-step to using Poxy is similar to Doxygen:
 
 1. Create your `poxy.toml` (Poxy's answer to the `Doxyfile`)
 2. Invoke Poxy on it: `poxy path/to/poxy.toml` (or simply `poxy` if the cwd contains the config file)
 3. See your HTML documentation `<cwd>/html`
 
-ℹ&#xFE0F; If there exists a `Doxyfile` or `Doxyfile-mcss` in the same directory as your `poxy.toml` it will be loaded
-first, then the Poxy overrides applied on top of it. Otherwise a 'default' Doxyfile is used as the base.
-
 <br><br>
 
 ## Config file options
 
 For a self-contained `poxy.toml` example to copy and paste from, see [the one used by toml++](https://github.com/marzer/tomlplusplus/blob/master/docs/poxy.toml).
 
 For a full list of options, with full descriptions, schemas and usage examples, see the [Configuration options] wiki page.
```

### Comparing `poxy-0.9.0/poxy/css.py` & `poxy-0.9.1/poxy/css.py`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/cppreference-doxygen-web.tag.xml` & `poxy-0.9.1/poxy/data/cppreference-doxygen-web.tag.xml`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/css/m-special.css` & `poxy-0.9.1/poxy/data/css/m-special.css`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/css/m-theme-dark.css` & `poxy-0.9.1/poxy/data/css/m-theme-dark.css`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/css/m-theme-light.css` & `poxy-0.9.1/poxy/data/css/m-theme-light.css`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/css/poxy-overrides.css` & `poxy-0.9.1/poxy/data/css/poxy-overrides.css`

 * *Files 5% similar despite different names*

```diff
@@ -146,42 +146,42 @@
 }
 .m-doc-details div > table.m-table td > strong:not(:first-child) > em,
 .m-doc-details div > table.m-table td > p:not(:first-child) > strong > em
 {
 	margin-top: 1.0rem;
 }
 
-/* github badges (index.html) */
-.gh-badges
+/* index page badges */
+#poxy-badges
 {
 	padding-bottom: 0.25rem;
 	margin-left: -0.9rem;
 	margin-right: -0.9rem;
 	margin-top: -0.5rem;
 }
 @media screen and (min-width: 992px)
 {
-	.gh-badges
+	#poxy-badges
 	{
 		display: flex;
 		justify-content: space-between;
 	}
-	.gh-badges br
+	#poxy-badges br
 	{
 		display: none;
 	}
 }
 @media screen and (max-width: 992px)
 {
-	.gh-badges
+	#poxy-badges
 	{
 		text-align: center;
 		line-height: 1.75rem;
 	}
-	.gh-badges a
+	#poxy-badges a
 	{
 		margin-left: 0.2rem;
 		margin-right: 0.2rem;
 		margin-bottom: 0.4rem;
 	}
 }
```

### Comparing `poxy-0.9.0/poxy/data/css/poxy-pygments.css` & `poxy-0.9.1/poxy/data/css/poxy-pygments.css`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/css/poxy-theme-dark.css` & `poxy-0.9.1/poxy/data/css/poxy-theme-dark.css`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/css/poxy-theme-light.css` & `poxy-0.9.1/poxy/data/css/poxy-theme-light.css`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/css/poxy.css` & `poxy-0.9.1/poxy/data/css/poxy.css`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/generated/6aa12ac32e258617e37a0030dc54f789b894368b.css` & `poxy-0.9.1/poxy/data/generated/6aa12ac32e258617e37a0030dc54f789b894368b.css`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/generated/emoji.json` & `poxy-0.9.1/poxy/data/generated/emoji.json`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/generated/fonts/6xK1dSBYKcSV-LCoeQqfX1RYOo3qPZ7jsDJT9g.woff2` & `poxy-0.9.1/poxy/data/generated/fonts/6xK1dSBYKcSV-LCoeQqfX1RYOo3qPZ7jsDJT9g.woff2`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/generated/fonts/6xK1dSBYKcSV-LCoeQqfX1RYOo3qPZ7ksDJT9g.woff2` & `poxy-0.9.1/poxy/data/generated/fonts/6xK1dSBYKcSV-LCoeQqfX1RYOo3qPZ7ksDJT9g.woff2`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/generated/fonts/6xK1dSBYKcSV-LCoeQqfX1RYOo3qPZ7nsDI.woff2` & `poxy-0.9.1/poxy/data/generated/fonts/6xK1dSBYKcSV-LCoeQqfX1RYOo3qPZ7nsDI.woff2`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/generated/fonts/6xK1dSBYKcSV-LCoeQqfX1RYOo3qPZ7osDJT9g.woff2` & `poxy-0.9.1/poxy/data/generated/fonts/6xK1dSBYKcSV-LCoeQqfX1RYOo3qPZ7osDJT9g.woff2`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/generated/fonts/6xK1dSBYKcSV-LCoeQqfX1RYOo3qPZ7psDJT9g.woff2` & `poxy-0.9.1/poxy/data/generated/fonts/6xK1dSBYKcSV-LCoeQqfX1RYOo3qPZ7psDJT9g.woff2`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/generated/fonts/6xK1dSBYKcSV-LCoeQqfX1RYOo3qPZ7qsDJT9g.woff2` & `poxy-0.9.1/poxy/data/generated/fonts/6xK1dSBYKcSV-LCoeQqfX1RYOo3qPZ7qsDJT9g.woff2`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/generated/fonts/6xK1dSBYKcSV-LCoeQqfX1RYOo3qPZ7rsDJT9g.woff2` & `poxy-0.9.1/poxy/data/generated/fonts/6xK1dSBYKcSV-LCoeQqfX1RYOo3qPZ7rsDJT9g.woff2`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/generated/fonts/6xK3dSBYKcSV-LCoeQqfX1RYOo3qN67lqDY.woff2` & `poxy-0.9.1/poxy/data/generated/fonts/6xK3dSBYKcSV-LCoeQqfX1RYOo3qN67lqDY.woff2`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/generated/fonts/6xK3dSBYKcSV-LCoeQqfX1RYOo3qNK7lqDY.woff2` & `poxy-0.9.1/poxy/data/generated/fonts/6xK3dSBYKcSV-LCoeQqfX1RYOo3qNK7lqDY.woff2`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/generated/fonts/6xK3dSBYKcSV-LCoeQqfX1RYOo3qNa7lqDY.woff2` & `poxy-0.9.1/poxy/data/generated/fonts/6xK3dSBYKcSV-LCoeQqfX1RYOo3qNa7lqDY.woff2`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/generated/fonts/6xK3dSBYKcSV-LCoeQqfX1RYOo3qNq7lqDY.woff2` & `poxy-0.9.1/poxy/data/generated/fonts/6xK3dSBYKcSV-LCoeQqfX1RYOo3qNq7lqDY.woff2`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/generated/fonts/6xK3dSBYKcSV-LCoeQqfX1RYOo3qO67lqDY.woff2` & `poxy-0.9.1/poxy/data/generated/fonts/6xK3dSBYKcSV-LCoeQqfX1RYOo3qO67lqDY.woff2`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/generated/fonts/6xK3dSBYKcSV-LCoeQqfX1RYOo3qOK7l.woff2` & `poxy-0.9.1/poxy/data/generated/fonts/6xK3dSBYKcSV-LCoeQqfX1RYOo3qOK7l.woff2`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/generated/fonts/6xK3dSBYKcSV-LCoeQqfX1RYOo3qPK7lqDY.woff2` & `poxy-0.9.1/poxy/data/generated/fonts/6xK3dSBYKcSV-LCoeQqfX1RYOo3qPK7lqDY.woff2`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/generated/fonts/6xKwdSBYKcSV-LCoeQqfX1RYOo3qPZY4lCdg18Smxg.woff2` & `poxy-0.9.1/poxy/data/generated/fonts/6xKwdSBYKcSV-LCoeQqfX1RYOo3qPZY4lCdg18Smxg.woff2`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/generated/fonts/6xKwdSBYKcSV-LCoeQqfX1RYOo3qPZY4lCdh18Smxg.woff2` & `poxy-0.9.1/poxy/data/generated/fonts/6xKwdSBYKcSV-LCoeQqfX1RYOo3qPZY4lCdh18Smxg.woff2`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/generated/fonts/6xKwdSBYKcSV-LCoeQqfX1RYOo3qPZY4lCdi18Smxg.woff2` & `poxy-0.9.1/poxy/data/generated/fonts/6xKwdSBYKcSV-LCoeQqfX1RYOo3qPZY4lCdi18Smxg.woff2`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/generated/fonts/6xKwdSBYKcSV-LCoeQqfX1RYOo3qPZY4lCdj18Smxg.woff2` & `poxy-0.9.1/poxy/data/generated/fonts/6xKwdSBYKcSV-LCoeQqfX1RYOo3qPZY4lCdj18Smxg.woff2`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/generated/fonts/6xKwdSBYKcSV-LCoeQqfX1RYOo3qPZY4lCdo18Smxg.woff2` & `poxy-0.9.1/poxy/data/generated/fonts/6xKwdSBYKcSV-LCoeQqfX1RYOo3qPZY4lCdo18Smxg.woff2`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/generated/fonts/6xKwdSBYKcSV-LCoeQqfX1RYOo3qPZY4lCds18Q.woff2` & `poxy-0.9.1/poxy/data/generated/fonts/6xKwdSBYKcSV-LCoeQqfX1RYOo3qPZY4lCds18Q.woff2`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/generated/fonts/6xKwdSBYKcSV-LCoeQqfX1RYOo3qPZY4lCdv18Smxg.woff2` & `poxy-0.9.1/poxy/data/generated/fonts/6xKwdSBYKcSV-LCoeQqfX1RYOo3qPZY4lCdv18Smxg.woff2`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/generated/fonts/6xKydSBYKcSV-LCoeQqfX1RYOo3i54rwkxduz8A.woff2` & `poxy-0.9.1/poxy/data/generated/fonts/6xKydSBYKcSV-LCoeQqfX1RYOo3i54rwkxduz8A.woff2`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/generated/fonts/6xKydSBYKcSV-LCoeQqfX1RYOo3i54rwlBduz8A.woff2` & `poxy-0.9.1/poxy/data/generated/fonts/6xKydSBYKcSV-LCoeQqfX1RYOo3i54rwlBduz8A.woff2`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/generated/fonts/6xKydSBYKcSV-LCoeQqfX1RYOo3i54rwlxdu.woff2` & `poxy-0.9.1/poxy/data/generated/fonts/6xKydSBYKcSV-LCoeQqfX1RYOo3i54rwlxdu.woff2`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/generated/fonts/6xKydSBYKcSV-LCoeQqfX1RYOo3i54rwmBduz8A.woff2` & `poxy-0.9.1/poxy/data/generated/fonts/6xKydSBYKcSV-LCoeQqfX1RYOo3i54rwmBduz8A.woff2`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/generated/fonts/6xKydSBYKcSV-LCoeQqfX1RYOo3i54rwmRduz8A.woff2` & `poxy-0.9.1/poxy/data/generated/fonts/6xKydSBYKcSV-LCoeQqfX1RYOo3i54rwmRduz8A.woff2`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/generated/fonts/6xKydSBYKcSV-LCoeQqfX1RYOo3i54rwmhduz8A.woff2` & `poxy-0.9.1/poxy/data/generated/fonts/6xKydSBYKcSV-LCoeQqfX1RYOo3i54rwmhduz8A.woff2`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/generated/fonts/6xKydSBYKcSV-LCoeQqfX1RYOo3i54rwmxduz8A.woff2` & `poxy-0.9.1/poxy/data/generated/fonts/6xKydSBYKcSV-LCoeQqfX1RYOo3i54rwmxduz8A.woff2`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/generated/fonts/HI_SiYsKILxRpg3hIP6sJ7fM7PqlM-vWjMY.woff2` & `poxy-0.9.1/poxy/data/generated/fonts/HI_SiYsKILxRpg3hIP6sJ7fM7PqlM-vWjMY.woff2`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/generated/fonts/HI_SiYsKILxRpg3hIP6sJ7fM7PqlMOvWjMY.woff2` & `poxy-0.9.1/poxy/data/generated/fonts/HI_SiYsKILxRpg3hIP6sJ7fM7PqlMOvWjMY.woff2`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/generated/fonts/HI_SiYsKILxRpg3hIP6sJ7fM7PqlMevWjMY.woff2` & `poxy-0.9.1/poxy/data/generated/fonts/HI_SiYsKILxRpg3hIP6sJ7fM7PqlMevWjMY.woff2`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/generated/fonts/HI_SiYsKILxRpg3hIP6sJ7fM7PqlMuvWjMY.woff2` & `poxy-0.9.1/poxy/data/generated/fonts/HI_SiYsKILxRpg3hIP6sJ7fM7PqlMuvWjMY.woff2`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/generated/fonts/HI_SiYsKILxRpg3hIP6sJ7fM7PqlOevWjMY.woff2` & `poxy-0.9.1/poxy/data/generated/fonts/HI_SiYsKILxRpg3hIP6sJ7fM7PqlOevWjMY.woff2`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/generated/fonts/HI_SiYsKILxRpg3hIP6sJ7fM7PqlPevW.woff2` & `poxy-0.9.1/poxy/data/generated/fonts/HI_SiYsKILxRpg3hIP6sJ7fM7PqlPevW.woff2`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/generated/fonts/HI_SiYsKILxRpg3hIP6sJ7fM7PqlPuvWjMY.woff2` & `poxy-0.9.1/poxy/data/generated/fonts/HI_SiYsKILxRpg3hIP6sJ7fM7PqlPuvWjMY.woff2`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/generated/fonts/HI_jiYsKILxRpg3hIP6sJ7fM7PqlOPHYvDP_W9O7GQTTbI1bQ10YVJg.woff2` & `poxy-0.9.1/poxy/data/generated/fonts/HI_jiYsKILxRpg3hIP6sJ7fM7PqlOPHYvDP_W9O7GQTTbI1bQ10YVJg.woff2`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/generated/fonts/HI_jiYsKILxRpg3hIP6sJ7fM7PqlOPHYvDP_W9O7GQTTbI1bQF0YVJg.woff2` & `poxy-0.9.1/poxy/data/generated/fonts/HI_jiYsKILxRpg3hIP6sJ7fM7PqlOPHYvDP_W9O7GQTTbI1bQF0YVJg.woff2`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/generated/fonts/HI_jiYsKILxRpg3hIP6sJ7fM7PqlOPHYvDP_W9O7GQTTbI1bQV0YVJg.woff2` & `poxy-0.9.1/poxy/data/generated/fonts/HI_jiYsKILxRpg3hIP6sJ7fM7PqlOPHYvDP_W9O7GQTTbI1bQV0YVJg.woff2`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/generated/fonts/HI_jiYsKILxRpg3hIP6sJ7fM7PqlOPHYvDP_W9O7GQTTbI1bQl0YVJg.woff2` & `poxy-0.9.1/poxy/data/generated/fonts/HI_jiYsKILxRpg3hIP6sJ7fM7PqlOPHYvDP_W9O7GQTTbI1bQl0YVJg.woff2`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/generated/fonts/HI_jiYsKILxRpg3hIP6sJ7fM7PqlOPHYvDP_W9O7GQTTbI1bSl0YVJg.woff2` & `poxy-0.9.1/poxy/data/generated/fonts/HI_jiYsKILxRpg3hIP6sJ7fM7PqlOPHYvDP_W9O7GQTTbI1bSl0YVJg.woff2`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/generated/fonts/HI_jiYsKILxRpg3hIP6sJ7fM7PqlOPHYvDP_W9O7GQTTbI1bTV0YVJg.woff2` & `poxy-0.9.1/poxy/data/generated/fonts/HI_jiYsKILxRpg3hIP6sJ7fM7PqlOPHYvDP_W9O7GQTTbI1bTV0YVJg.woff2`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/generated/fonts/HI_jiYsKILxRpg3hIP6sJ7fM7PqlOPHYvDP_W9O7GQTTbI1bTl0Y.woff2` & `poxy-0.9.1/poxy/data/generated/fonts/HI_jiYsKILxRpg3hIP6sJ7fM7PqlOPHYvDP_W9O7GQTTbI1bTl0Y.woff2`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/generated/poxy.css` & `poxy-0.9.1/poxy/data/generated/poxy.css`

 * *Files 0% similar despite different names*

```diff
@@ -2663,22 +2663,22 @@
 .m-doc-details div > table.m-table td > h6,
 .m-doc-details div > table.m-table td > strong > em,
 .m-doc-details div > table.m-table td > p > strong > em { font-style: normal; color: var(--article-heading-color); }
 .m-doc-details div > table.m-table td > strong > em,
 .m-doc-details div > table.m-table td > p > strong > em { display: block; }
 .m-doc-details div > table.m-table td > strong:not(:first-child) > em,
 .m-doc-details div > table.m-table td > p:not(:first-child) > strong > em { margin-top: 1.0rem; }
-.gh-badges { padding-bottom: 0.25rem; margin-left: -0.9rem; margin-right: -0.9rem; margin-top: -0.5rem; }
+#poxy-badges { padding-bottom: 0.25rem; margin-left: -0.9rem; margin-right: -0.9rem; margin-top: -0.5rem; }
 @media screen and (min-width: 992px) {
-.gh-badges { display: flex; justify-content: space-between; }
-.gh-badges br { display: none; }
+#poxy-badges { display: flex; justify-content: space-between; }
+#poxy-badges br { display: none; }
 }
 @media screen and (max-width: 992px) {
-.gh-badges { text-align: center; line-height: 1.75rem; }
-.gh-badges a { margin-left: 0.2rem; margin-right: 0.2rem; margin-bottom: 0.4rem; }
+#poxy-badges { text-align: center; line-height: 1.75rem; }
+#poxy-badges a { margin-left: 0.2rem; margin-right: 0.2rem; margin-bottom: 0.4rem; }
 }
 h1 span.m-thin { color: var(--dim-color); }
 #poxy-main-banner {
 margin-left: -1rem !important;
 margin-right: -1rem !important;
 margin-top: -1.75rem !important;
 max-width: calc(100% + 2rem) !important;
```

### Comparing `poxy-0.9.0/poxy/data/jquery-3.6.0.slim.min.js` & `poxy-0.9.1/poxy/data/jquery-3.6.0.slim.min.js`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/m.css/COPYING` & `poxy-0.9.1/poxy/data/m.css/COPYING`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/m.css/css/m-components.css` & `poxy-0.9.1/poxy/data/m.css/css/m-components.css`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/m.css/css/m-debug.css` & `poxy-0.9.1/poxy/data/m.css/css/m-debug.css`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/m.css/css/m-documentation.css` & `poxy-0.9.1/poxy/data/m.css/css/m-documentation.css`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/m.css/css/m-grid.css` & `poxy-0.9.1/poxy/data/m.css/css/m-grid.css`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/m.css/css/m-layout.css` & `poxy-0.9.1/poxy/data/m.css/css/m-layout.css`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/m.css/css/pygments-console.css` & `poxy-0.9.1/poxy/data/m.css/css/pygments-console.css`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/m.css/css/pygments-dark.css` & `poxy-0.9.1/poxy/data/m.css/css/pygments-dark.css`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/m.css/documentation/__init__.py` & `poxy-0.9.1/poxy/data/m.css/documentation/__init__.py`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/m.css/documentation/_search.py` & `poxy-0.9.1/poxy/data/m.css/documentation/_search.py`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/m.css/documentation/doxygen.py` & `poxy-0.9.1/poxy/data/m.css/documentation/doxygen.py`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/m.css/documentation/python.py` & `poxy-0.9.1/poxy/data/m.css/documentation/python.py`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/m.css/documentation/search.js` & `poxy-0.9.1/poxy/data/m.css/documentation/search.js`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/m.css/documentation/templates/doxygen/annotated.html` & `poxy-0.9.1/poxy/data/m.css/documentation/templates/doxygen/annotated.html`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/m.css/documentation/templates/doxygen/base-class-reference.html` & `poxy-0.9.1/poxy/data/m.css/documentation/templates/doxygen/base-class-reference.html`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/m.css/documentation/templates/doxygen/base-index.html` & `poxy-0.9.1/poxy/data/m.css/documentation/templates/doxygen/base-index.html`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/m.css/documentation/templates/doxygen/base-reference.html` & `poxy-0.9.1/poxy/data/m.css/documentation/templates/doxygen/base-reference.html`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/m.css/documentation/templates/doxygen/base.html` & `poxy-0.9.1/poxy/data/m.css/documentation/templates/doxygen/base.html`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/m.css/documentation/templates/doxygen/concepts.html` & `poxy-0.9.1/poxy/data/m.css/documentation/templates/doxygen/concepts.html`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/m.css/documentation/templates/doxygen/details-define.html` & `poxy-0.9.1/poxy/data/m.css/documentation/templates/doxygen/details-define.html`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/m.css/documentation/templates/doxygen/details-enum.html` & `poxy-0.9.1/poxy/data/m.css/documentation/templates/doxygen/details-enum.html`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/m.css/documentation/templates/doxygen/details-func.html` & `poxy-0.9.1/poxy/data/m.css/documentation/templates/doxygen/details-func.html`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/m.css/documentation/templates/doxygen/details-typedef.html` & `poxy-0.9.1/poxy/data/m.css/documentation/templates/doxygen/details-typedef.html`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/m.css/documentation/templates/doxygen/details-var.html` & `poxy-0.9.1/poxy/data/m.css/documentation/templates/doxygen/details-var.html`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/m.css/documentation/templates/doxygen/dir.html` & `poxy-0.9.1/poxy/data/m.css/documentation/templates/doxygen/dir.html`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/m.css/documentation/templates/doxygen/entry-class.html` & `poxy-0.9.1/poxy/data/m.css/documentation/templates/doxygen/entry-class.html`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/m.css/documentation/templates/doxygen/entry-concept.html` & `poxy-0.9.1/poxy/data/m.css/documentation/templates/doxygen/entry-concept.html`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/m.css/documentation/templates/doxygen/entry-define.html` & `poxy-0.9.1/poxy/data/m.css/documentation/templates/doxygen/entry-define.html`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/m.css/documentation/templates/doxygen/entry-enum.html` & `poxy-0.9.1/poxy/data/m.css/documentation/templates/doxygen/entry-enum.html`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/m.css/documentation/templates/doxygen/entry-func.html` & `poxy-0.9.1/poxy/data/m.css/documentation/templates/doxygen/entry-func.html`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/m.css/documentation/templates/doxygen/entry-typedef.html` & `poxy-0.9.1/poxy/data/m.css/documentation/templates/doxygen/entry-typedef.html`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/m.css/documentation/templates/doxygen/entry-var.html` & `poxy-0.9.1/poxy/data/m.css/documentation/templates/doxygen/entry-var.html`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/m.css/documentation/templates/doxygen/example.html` & `poxy-0.9.1/poxy/data/m.css/documentation/templates/doxygen/example.html`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/m.css/documentation/templates/doxygen/file.html` & `poxy-0.9.1/poxy/data/m.css/documentation/templates/doxygen/file.html`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/m.css/documentation/templates/doxygen/files.html` & `poxy-0.9.1/poxy/data/m.css/documentation/templates/doxygen/files.html`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/m.css/documentation/templates/doxygen/group.html` & `poxy-0.9.1/poxy/data/m.css/documentation/templates/doxygen/group.html`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/m.css/documentation/templates/doxygen/modules.html` & `poxy-0.9.1/poxy/data/m.css/documentation/templates/doxygen/modules.html`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/m.css/documentation/templates/doxygen/namespaces.html` & `poxy-0.9.1/poxy/data/m.css/documentation/templates/doxygen/namespaces.html`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/m.css/documentation/templates/doxygen/page.html` & `poxy-0.9.1/poxy/data/m.css/documentation/templates/doxygen/page.html`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/m.css/documentation/templates/doxygen/pages.html` & `poxy-0.9.1/poxy/data/m.css/documentation/templates/doxygen/pages.html`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/m.css/plugins/ansilexer.py` & `poxy-0.9.1/poxy/data/m.css/plugins/ansilexer.py`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/m.css/plugins/dot2svg.py` & `poxy-0.9.1/poxy/data/m.css/plugins/dot2svg.py`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/m.css/plugins/latex2svg.py` & `poxy-0.9.1/poxy/data/m.css/plugins/latex2svg.py`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/m.css/plugins/latex2svgextra.py` & `poxy-0.9.1/poxy/data/m.css/plugins/latex2svgextra.py`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/m.css/plugins/m/__init__.py` & `poxy-0.9.1/poxy/data/m.css/plugins/m/__init__.py`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/m.css/plugins/m/abbr.py` & `poxy-0.9.1/poxy/data/m.css/plugins/m/abbr.py`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/m.css/plugins/m/alias.py` & `poxy-0.9.1/poxy/data/m.css/plugins/m/alias.py`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/m.css/plugins/m/code.py` & `poxy-0.9.1/poxy/data/m.css/plugins/m/code.py`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/m.css/plugins/m/components.py` & `poxy-0.9.1/poxy/data/m.css/plugins/m/components.py`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/m.css/plugins/m/dot.py` & `poxy-0.9.1/poxy/data/m.css/plugins/m/dot.py`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/m.css/plugins/m/dox.py` & `poxy-0.9.1/poxy/data/m.css/plugins/m/dox.py`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/m.css/plugins/m/filesize.py` & `poxy-0.9.1/poxy/data/m.css/plugins/m/filesize.py`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/m.css/plugins/m/gh.py` & `poxy-0.9.1/poxy/data/m.css/plugins/m/gh.py`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/m.css/plugins/m/gl.py` & `poxy-0.9.1/poxy/data/m.css/plugins/m/gl.py`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/m.css/plugins/m/htmlsanity.py` & `poxy-0.9.1/poxy/data/m.css/plugins/m/htmlsanity.py`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/m.css/plugins/m/images.py` & `poxy-0.9.1/poxy/data/m.css/plugins/m/images.py`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/m.css/plugins/m/link.py` & `poxy-0.9.1/poxy/data/m.css/plugins/m/link.py`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/m.css/plugins/m/math.py` & `poxy-0.9.1/poxy/data/m.css/plugins/m/math.py`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/m.css/plugins/m/metadata.py` & `poxy-0.9.1/poxy/data/m.css/plugins/m/metadata.py`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/m.css/plugins/m/plots.py` & `poxy-0.9.1/poxy/data/m.css/plugins/m/plots.py`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/m.css/plugins/m/qr.py` & `poxy-0.9.1/poxy/data/m.css/plugins/m/qr.py`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/m.css/plugins/m/sphinx.py` & `poxy-0.9.1/poxy/data/m.css/plugins/m/sphinx.py`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/m.css/plugins/m/vk.py` & `poxy-0.9.1/poxy/data/m.css/plugins/m/vk.py`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/poxy-badge-c++03.svg` & `poxy-0.9.1/poxy/data/poxy-badge-c++03.svg`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/poxy-badge-c++11.svg` & `poxy-0.9.1/poxy/data/poxy-badge-c++11.svg`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/poxy-badge-c++14.svg` & `poxy-0.9.1/poxy/data/poxy-badge-c++14.svg`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/poxy-badge-c++17.svg` & `poxy-0.9.1/poxy/data/poxy-badge-c++17.svg`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/poxy-badge-c++20.svg` & `poxy-0.9.1/poxy/data/poxy-badge-c++20.svg`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/poxy-badge-c++23.svg` & `poxy-0.9.1/poxy/data/poxy-badge-c++23.svg`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/poxy-badge-c++26.svg` & `poxy-0.9.1/poxy/data/poxy-badge-c++26.svg`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/poxy-badge-c++29.svg` & `poxy-0.9.1/poxy/data/poxy-badge-c++29.svg`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/poxy-badge-c++98.svg` & `poxy-0.9.1/poxy/data/poxy-badge-c++98.svg`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/poxy-badge-license-apache_2.svg` & `poxy-0.9.1/poxy/data/poxy-badge-license-apache_2.svg`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/poxy-badge-license-bsd_2_clause.svg` & `poxy-0.9.1/poxy/data/poxy-badge-license-bsd_2_clause.svg`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/poxy-badge-license-bsd_3_clause.svg` & `poxy-0.9.1/poxy/data/poxy-badge-license-bsd_3_clause.svg`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/poxy-badge-license-gpl.svg` & `poxy-0.9.1/poxy/data/poxy-badge-license-gpl.svg`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/poxy-badge-license-gpl_2.svg` & `poxy-0.9.1/poxy/data/poxy-badge-license-gpl_2.svg`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/poxy-badge-license-gpl_3.svg` & `poxy-0.9.1/poxy/data/poxy-badge-license-gpl_3.svg`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/poxy-badge-license-lgpl.svg` & `poxy-0.9.1/poxy/data/poxy-badge-license-lgpl.svg`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/poxy-badge-license-lgpl_2.svg` & `poxy-0.9.1/poxy/data/poxy-badge-license-lgpl_2.svg`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/poxy-badge-license-lgpl_2_1.svg` & `poxy-0.9.1/poxy/data/poxy-badge-license-lgpl_2_1.svg`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/poxy-badge-license-lgpl_3.svg` & `poxy-0.9.1/poxy/data/poxy-badge-license-lgpl_3.svg`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/poxy-icon-github.svg` & `poxy-0.9.1/poxy/data/poxy-icon-github.svg`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/poxy-icon-theme.svg` & `poxy-0.9.1/poxy/data/poxy-icon-theme.svg`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/data/poxy.js` & `poxy-0.9.1/poxy/data/poxy.js`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/dirs.py` & `poxy-0.9.1/poxy/dirs.py`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/doxygen.py` & `poxy-0.9.1/poxy/doxygen.py`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/emoji.py` & `poxy-0.9.1/poxy/emoji.py`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/fixers.py` & `poxy-0.9.1/poxy/fixers.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 'Fixer' function objects used during various post-process steps.
 """
 
 import html
 from bs4 import NavigableString
 from .utils import *
 from .svg import SVG
+from .project import Context
 from . import soup
 
 #=======================================================================================================================
 # base classes
 #=======================================================================================================================
 
 
@@ -103,15 +104,15 @@
 		elif tag_name in (r'set_name', r'parent_set_name', r'set_parent_name'):
 			if tag_content:
 				out.append((tag_name, tag_content))
 			return ''
 		else:
 			return f'<{m[1]}{(" " + tag_content) if tag_content else ""}>'
 
-	def __call__(self, doc, context):
+	def __call__(self, context: Context, doc: soup.HTMLDocument, path: Path):
 		if doc.article_content is None:
 			return False
 		changed = False
 		changed_this_pass = True
 		while changed_this_pass:
 			changed_this_pass = False
 			for name in self.__allowed_parents:
@@ -191,15 +192,15 @@
 	__expression = re.compile(rf'(\s+)({_CPPModifiersBase._modifierRegex})(\s+)')
 	__sections = ('pub-static-methods', 'pub-methods', 'friends', 'func-members')
 
 	@classmethod
 	def __substitute(cls, m, out):
 		return f'{m[1]}<span class="poxy-injected m-label m-flat {cls._modifierClasses[m[2]]}">{m[2]}</span>{m[3]}'
 
-	def __call__(self, doc, context):
+	def __call__(self, context: Context, doc: soup.HTMLDocument, path: Path):
 		if doc.article_content is None:
 			return False
 		changed = False
 		for sect in self.__sections:
 			tags = doc.find_all_from_sections('dt', select='span.m-doc-wrap', section=sect)
 			for tag in tags:
 				replacer = RegexReplacer(self.__expression, self.__substitute, str(tag))
@@ -217,15 +218,15 @@
 	__expression = re.compile(rf'\s+({_CPPModifiersBase._modifierRegex})\s+')
 
 	@classmethod
 	def __substitute(cls, m, matches):
 		matches.append(m[1])
 		return ' '
 
-	def __call__(self, doc, context):
+	def __call__(self, context: Context, doc: soup.HTMLDocument, path: Path):
 		if doc.article_content is None:
 			return False
 		changed = False
 		sections = doc.find_all_from_sections(section=False)  # all sections without an id
 		section = None
 		for s in sections:
 			if (str(s.h2.string) == 'Function documentation'):
@@ -263,15 +264,15 @@
 	'''
 	__expression = re.compile(r'(template&lt;.+?&gt;)\s+(template&lt;)', re.S)
 
 	@classmethod
 	def __substitute(cls, m):
 		return f'{m[1]}<br>\n{m[2]}'
 
-	def __call__(self, doc, context):
+	def __call__(self, context: Context, doc: soup.HTMLDocument, path: Path):
 		changed = False
 		for template in doc.body('div', class_='m-doc-template'):
 			replacer = RegexReplacer(self.__expression, lambda m, out: self.__substitute(m), str(template))
 			if replacer:
 				soup.replace_tag(template, str(replacer))
 				changed = True
 		return changed
@@ -279,15 +280,15 @@
 
 
 class StripIncludes(HTMLFixer):
 	'''
 	Strips #include <paths/to/headers.h> based on context.sources.strip_includes.
 	'''
 
-	def __call__(self, doc, context):
+	def __call__(self, context: Context, doc: soup.HTMLDocument, path: Path):
 		if doc.article is None or not context.sources.strip_includes:
 			return False
 		changed = False
 		for include_div in doc.article.find_all(r'div', class_=r'm-doc-include'):
 			anchor = include_div.find('a', href=True, class_=r'cpf')
 			if anchor is None:
 				continue
@@ -310,16 +311,16 @@
 
 
 class Banner(HTMLFixer):
 	'''
 	Makes the first image on index.html a 'banner'
 	'''
 
-	def __call__(self, doc, context):
-		if doc.article_content is None or doc.path.name.lower() != 'index.html':
+	def __call__(self, context: Context, doc: soup.HTMLDocument, path: Path):
+		if doc.article_content is None or path.name.lower() != 'index.html':
 			return False
 		parent = doc.article_content
 
 		h1 = parent.find('h1', recursive=False)
 		banner = parent.find('img', recursive=False)
 		if not banner or not h1 or r'src' not in banner.attrs or not banner[r'src']:
 			return False
@@ -329,23 +330,25 @@
 			sibling = banner.find_previous_sibling(sibling_tag)
 			if sibling is not None:
 				return False
 
 		banner = banner.extract()
 		h1.replace_with(banner)
 		banner[r'id'] = r'poxy-main-banner'
+		soup.add_class(doc.body, r'poxy-has-main-banner')
 
 		if context.badges:
-			parent = doc.new_tag('div', class_='gh-badges', after=banner)
+			parent = doc.new_tag('div', id='poxy-badges', after=banner)
 			for (alt, src, href) in context.badges:
 				if alt is None and src is None and href is None:
 					doc.new_tag('br', parent=parent)
 				else:
 					anchor = doc.new_tag('a', parent=parent, href=href, target='_blank')
 					doc.new_tag('img', parent=anchor, src=src, alt=alt)
+			soup.add_class(doc.body, r'poxy-has-badges')
 		return True
 
 
 
 class CodeBlocks(HTMLFixer):
 	'''
 	Fixes various issues and improves syntax highlighting in <code> blocks.
@@ -443,15 +446,15 @@
 			return False
 		if not isinstance(mid, NavigableString):
 			return False
 		if len(mid.string.strip()) > 0:
 			return False
 		return True
 
-	def __call__(self, doc, context):
+	def __call__(self, context: Context, doc: soup.HTMLDocument, path: Path):
 		changed = False
 
 		# fix up syntax highlighting
 		code_blocks = doc.body(('pre', 'code'), class_='m-code')
 		changed_this_pass = True
 		while changed_this_pass:
 			changed_this_pass = False
@@ -622,15 +625,15 @@
 	__allowedNames = ('dd', 'p', 'dt', 'h3', 'td', 'div', 'figcaption')
 
 	@classmethod
 	def __substitute(cls, m, uri):
 		external = uri.startswith('http')
 		return rf'''<a href="{uri}" class="m-doc poxy-injected{' poxy-external' if external else ''}"{' target="_blank"' if external else ''}>{m[0]}</a>'''
 
-	def __call__(self, doc, context):
+	def __call__(self, context: Context, doc: soup.HTMLDocument, path: Path):
 		if doc.article_content is None:
 			return False
 
 		changed = False
 
 		# first check all existing doc links to make sure they aren't erroneously linked to the wrong thing
 		if 1:
@@ -654,15 +657,15 @@
 					if link.has_attr('href'):
 						href = str(link['href'])
 						anchor = href.rfind('#')
 						if anchor == 0:
 							continue  # don't override internal self-links
 						if anchor != -1:
 							href = href[:anchor]
-						if href == uri or href == doc.path.name:  # don't override internal self-links
+						if href == uri or href == path.name:  # don't override internal self-links
 							continue
 					link['href'] = uri
 					soup.set_class(link, ['m-doc', 'poxy-injected'])
 					if uri.startswith('http'):
 						soup.add_class(link, 'poxy-external')
 					done = True
 					changed = True
@@ -677,15 +680,15 @@
 				lambda t: soup.find_parent(t, 'a', doc.article_content) is None
 			)
 			strings = []
 			for tag in tags:
 				strings = strings + soup.string_descendants(tag, lambda t: soup.find_parent(t, 'a', tag) is None)
 			strings = [s for s in strings if s.parent is not None]
 			for expr, uri in context.autolinks:
-				if uri == doc.path.name:  # don't create unnecessary self-links
+				if uri == path.name:  # don't create unnecessary self-links
 					continue
 				i = 0
 				while i < len(strings):
 					string = strings[i]
 					parent = string.parent
 					replacer = RegexReplacer(
 						expr, lambda m, out: self.__substitute(m, uri), html.escape(str(string), quote=False)
@@ -713,15 +716,15 @@
 	Fixes various minor issues with anchor tags.
 	'''
 	__external_href = re.compile(r'^(?:https?|s?ftp|mailto)[:].+$', re.I)
 	__internal_doc_id = re.compile(r'^[a-fA-F0-9]+$')
 	__godbolt = re.compile(r'^\s*https[:]//godbolt.org/z/.+?$', re.I)
 	__local_href = re.compile(r'^([-/_a-zA-Z0-9]+\.[a-zA-Z]+)(?:#(.*))?$')
 
-	def __call__(self, doc, context):
+	def __call__(self, context: Context, doc: soup.HTMLDocument, path: Path):
 		changed = False
 		for anchor in doc.body('a', href=True):
 			href = anchor['href']
 
 			# make sure links to external sources are correctly marked as such
 			if self.__external_href.fullmatch(href) is not None:
 				if 'target' not in anchor.attrs or anchor['target'] != '_blank':
@@ -742,15 +745,15 @@
 						changed = True
 				continue
 
 			is_mdoc = r'class' in anchor.attrs and (r'm-doc' in anchor['class'] or r'm-doc-self' in anchor['class'])
 
 			# make sure links to local files point to actual existing files
 			match = self.__local_href.fullmatch(href)
-			if match and not coerce_path(doc.path.parent, match[1]).exists():
+			if match and not coerce_path(path.parent, match[1]).exists():
 				changed = True
 				if is_mdoc:
 					href = r'#'
 					anchor[r'href'] = r'#'  # will by fixed by the next step
 				else:
 					for attr in (
 						r'download', r'href', r'hreflang', r'media', r'ping', r'referrerpolicy', r'rel', r'target',
@@ -783,15 +786,15 @@
 
 
 class EmptyTags(HTMLFixer):
 	'''
 	Prunes the tree of various empty tags (happens as a side-effect of some other operations).
 	'''
 
-	def __call__(self, doc, context):
+	def __call__(self, context: Context, doc: soup.HTMLDocument, path: Path):
 		changed = False
 		for tag in doc.body((r'p', r'span')):
 			if not tag.contents or (
 				len(tag.contents) == 1 and isinstance(tag.contents[0], NavigableString) and not tag.string
 			):
 				soup.destroy_node(tag)
 				changed = True
@@ -800,50 +803,49 @@
 
 
 class MarkTOC(HTMLFixer):
 	'''
 	Marks any table-of-contents with a custom class.
 	'''
 
-	def __call__(self, doc, context):
+	def __call__(self, context: Context, doc: soup.HTMLDocument, path: Path):
 		if doc.table_of_contents is None:
 			return False
 		soup.add_class(doc.table_of_contents, r'poxy-toc')
 		doc.table_of_contents['id'] = r'poxy-toc'
 		soup.add_class(doc.body, r'poxy-has-toc')
 		return True
 
 
 
 class InjectSVGs(HTMLFixer):
 	'''
 	Injects the contents of SVG <img> tags directly into the document.
 	'''
 
-	def __call__(self, doc, context):
+	def __call__(self, context: Context, doc: soup.HTMLDocument, path: Path):
 		imgs = doc.body.find_all(r'img')
 		if not imgs:
 			return False
 		imgs = [
 			i for i in imgs
 			if r'src' in i.attrs and i[r'src'] and not is_uri(i[r'src']) and i[r'src'].lower().endswith(r'.svg')
 		]
 		count = 0
 		for img in imgs:
-			src = Path(doc.path.parent, img[r'src'])
-			if not src.exists() or not src.is_file():
+			src = Path(path.parent, img[r'src'])
+			if not src.exists() or not src.is_file() or src.stat().st_size > (1024 * 16):  # max 16 kb
 				continue
-			img_id = img[r'id'] if r'id' in img.attrs else rf'poxy-injected-svg-{count}'
 			svg = SVG(
 				src,  #
 				logger=context.verbose_logger,
-				root_id=img_id
+				root_id=img[r'id'] if r'id' in img.attrs else rf'poxy-injected-svg-{count}',
+				root_classes=(*soup.get_classes(img), r'poxy-injected-svg')
 			)
 			img = soup.replace_tag(img, str(svg))[0]
-			soup.add_class(img, r'poxy-injected-svg')
 			count += 1
 		return count > 0
 
 
 
 #=======================================================================================================================
 # plain text post-processes
@@ -853,35 +855,30 @@
 
 class ImplementationDetails(PlainTextFixer):
 	'''
 	Replaces implementation details with appropriate shorthands.
 	'''
 	__shorthands = ((r'POXY_IMPLEMENTATION_DETAIL_IMPL', r'<code class="m-note m-dim poxy-impl">/* ... */</code>'), )
 
-	def __call__(self, doc, context):
-		changed = False
+	def __call__(self, context: Context, text: str, path: Path) -> str:
 		for shorthand, replacement in self.__shorthands:
-			idx = doc[0].find(shorthand)
+			idx = text.find(shorthand)
 			while idx >= 0:
-				doc[0] = doc[0][:idx] + replacement + doc[0][idx + len(shorthand):]
-				changed = True
-				idx = doc[0].find(shorthand)
-		return changed
+				text = text[:idx] + replacement + text[idx + len(shorthand):]
+				idx = text.find(shorthand)
+		return text
 
 
 
 class MarkdownPages(PlainTextFixer):
 	'''
 	Cleans up some HTML snafus from markdown-based pages.
 	'''
 
-	def __call__(self, doc, context):
-		if not doc[1].name.lower().startswith(r'md_') and not doc[1].name.lower().startswith(r'm_d__'):
-			return False
-
-		WBR = r'(?:<wbr[ \t]*/?>)?'
-		PREFIX = rf'_{WBR}_{WBR}poxy_{WBR}thiswasan_{WBR}'
-		doc[0] = re.sub(rf'{PREFIX}amp', r'&amp;', doc[0])
-		doc[0] = re.sub(rf'{PREFIX}at', r'@', doc[0])
-		doc[0] = re.sub(rf'{PREFIX}fe0f', r'&#xFE0F;', doc[0])
-
-		return True
+	def __call__(self, context: Context, text: str, path: Path) -> str:
+		if path.name.lower().startswith(r'md_') or path.name.lower().startswith(r'm_d__'):
+			WBR = r'(?:<wbr[ \t]*/?>)?'
+			PREFIX = rf'_{WBR}_{WBR}poxy_{WBR}thiswasan_{WBR}'
+			text = re.sub(rf'{PREFIX}amp', r'&amp;', text)
+			text = re.sub(rf'{PREFIX}at', r'@', text)
+			text = re.sub(rf'{PREFIX}fe0f', r'&#xFE0F;', text)
+		return text
```

### Comparing `poxy-0.9.0/poxy/main.py` & `poxy-0.9.1/poxy/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 	#--------------------------------------------------------------
 	# public user-facing arguments
 	#--------------------------------------------------------------
 	args.add_argument(
 		r'config',
 		type=Path,
 		nargs='?',
-		default=None,
+		default=Path('.'),
 		help=r'path to poxy.toml or a directory containing it (default: %(default)s)'
 	)
 	args.add_argument(
 		r'-v',  #
 		r'--verbose',
 		action=r'store_true',
 		help=r"enable very noisy diagnostic output"
@@ -69,17 +69,32 @@
 		r'--doxygen',  #
 		type=Path,
 		default=None,
 		metavar=r'<path>',
 		help=r"specify the Doxygen executable to use (default: find on system path)"
 	)
 	args.add_argument(
-		r'--dry',  #
-		action=r'store_true',
-		help=r"do a 'dry run' only, stopping after emitting the effective Doxyfile"
+		r'--ppinclude',  #
+		type=str,
+		default=None,
+		metavar=r'<regex>',
+		help=r"pattern matching HTML file names to post-process (default: all)"
+	)
+	args.add_argument(
+		r'--ppexclude',  #
+		type=str,
+		default=None,
+		metavar=r'<regex>',
+		help=r"pattern matching HTML file names to exclude from post-processing (default: none)"
+	)
+	args.add_argument(
+		r'--theme',  #
+		choices=[r'auto', r'light', r'dark', r'custom'],
+		default=r'auto',
+		help=r'the CSS theme to use (default: %(default)s)'
 	)
 	args.add_argument(
 		r'--threads',  #
 		type=int,
 		default=0,
 		metavar=r'N',
 		help=r"set the number of threads to use (default: automatic)"
@@ -96,34 +111,14 @@
 		help=r"always treat warnings as errors regardless of config file settings"
 	)
 	args.add_argument(
 		r'--xmlonly',  #
 		action=r'store_true',
 		help=r"stop after generating and preprocessing the Doxygen xml"
 	)
-	args.add_argument(
-		r'--ppinclude',  #
-		type=str,
-		default=None,
-		metavar=r'<regex>',
-		help=r"pattern matching HTML file names to post-process (default: all)"
-	)
-	args.add_argument(
-		r'--ppexclude',  #
-		type=str,
-		default=None,
-		metavar=r'<regex>',
-		help=r"pattern matching HTML file names to exclude from post-processing (default: none)"
-	)
-	args.add_argument(
-		r'--theme',  #
-		choices=[r'auto', r'light', r'dark', r'custom'],
-		default=r'auto',
-		help=r'the CSS theme to use (default: %(default)s)'
-	)
 	#--------------------------------------------------------------
 	# hidden developer-only/diagnostic arguments
 	#--------------------------------------------------------------
 	args.add_argument(
 		r'--nocleanup',  #
 		action=r'store_true',
 		help=argparse.SUPPRESS
@@ -219,24 +214,23 @@
 
 	if args.update_emoji:
 		emoji.update_database_file()
 
 	if args.update_styles or args.update_fonts or args.update_emoji or args.mcss is not None:
 		return
 
-	with ScopeTimer(r'All tasks', print_start=False, print_end=not args.dry) as timer:
+	with ScopeTimer(r'All tasks', print_start=False, print_end=True) as timer:
 		run(
 			config_path=args.config,
 			output_dir=Path.cwd(),
 			threads=args.threads,
 			cleanup=not args.nocleanup,
 			verbose=args.verbose,
 			doxygen_path=args.doxygen,
 			logger=True,  # stderr + stdout
-			dry_run=args.dry,
 			xml_only=args.xmlonly,
 			html_include=args.ppinclude,
 			html_exclude=args.ppexclude,
 			treat_warnings_as_errors=True if args.werror else None,
 			theme=None if args.theme == r'auto' else args.theme,
 			copy_assets=not args.noassets
 		)
```

### Comparing `poxy-0.9.0/poxy/project.py` & `poxy-0.9.1/poxy/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -655,15 +655,16 @@
 		r'(?:::)?FPositionVertexBuffer(?:s)?':
 			r'https://docs.unrealengine.com/4.27/en-US/API/Runtime/Engine/Rendering/FPositionVertexBuffer/',
 		r'(?:::)?TArrayView(?:s)?':
 			r'https://docs.unrealengine.com/4.27/en-US/API/Runtime/Core/Containers/TArrayView/',
 		r'(?:::)?TArray(?:s)?':
 			r'https://docs.unrealengine.com/4.27/en-US/API/Runtime/Core/Containers/TArray/',
 	}
-	navbar = [r'files', r'groups', r'namespaces', r'classes']
+	navbar = (r'files', r'groups', r'namespaces', r'classes', r'concepts')
+	navbar_all = (r'pages', *navbar, r'repo', r'theme')
 	aliases = {
 		# poxy
 		r'cpp':
 			r'@code{.cpp}',
 		r'ecpp':
 			r'@endcode',
 		r'endcpp':
@@ -1260,36 +1261,33 @@
 		if isinstance(obj, (tuple, list, dict)):
 			self.verbose_value(name, obj)
 		else:
 			for k, v in obj.__dict__.items():
 				self.verbose_value(rf'{name}.{k}', v)
 
 	def __init__(
-		self, config_path, output_dir, threads, cleanup, verbose, doxygen_path, logger, dry_run, xml_only, html_include,
+		self, config_path, output_dir, threads, cleanup, verbose, doxygen_path, logger, xml_only, html_include,
 		html_exclude, treat_warnings_as_errors, theme, copy_assets
 	):
 
 		self.logger = logger
 		self.__verbose = bool(verbose)
-		self.dry_run = bool(dry_run)
 		self.xml_only = bool(xml_only)
 		self.cleanup = bool(cleanup)
 		self.copy_assets = bool(copy_assets)
 		self.verbose_logger = logger if self.__verbose else None
 
 		self.version = lib_version()
 		self.version_string = r'.'.join([str(v) for v in lib_version()])
-		if not self.dry_run or self.__verbose:
-			self.info(rf'Poxy v{self.version_string}')
+		self.info(rf'Poxy v{self.version_string}')
 
-		self.verbose_value(r'Context.dry_run', self.dry_run)
 		self.verbose_value(r'Context.xml_only', self.xml_only)
 		self.verbose_value(r'Context.cleanup', self.cleanup)
 
-		threads = int(threads)
+		threads = int(threads) if threads is not None else 0
 		if threads <= 0:
 			threads = os.cpu_count()
 		self.threads = max(1, min(os.cpu_count(), threads))
 		self.verbose_value(r'Context.threads', self.threads)
 
 		self.fixers = None
 		self.tagfile_path = None
@@ -1376,21 +1374,20 @@
 			self.verbose_value(r'Context.temp_dir', self.temp_dir)
 			self.temp_pages_dir = Path(self.temp_dir, r'pages')
 			self.verbose_value(r'Context.temp_pages_dir', self.temp_pages_dir)
 			assert self.temp_dir.is_absolute()
 			assert self.temp_pages_dir.is_absolute()
 
 			# delete leftovers from previous run and initialize various dirs
-			if not self.dry_run:
-				delete_directory(self.xml_dir, logger=self.verbose_logger)
-				delete_directory(self.temp_dir, logger=self.verbose_logger)
-				if not self.xml_only:
-					delete_directory(self.html_dir, logger=self.verbose_logger)
-				self.temp_dir.mkdir(exist_ok=True, parents=True)
-				self.temp_pages_dir.mkdir(exist_ok=True, parents=True)
+			delete_directory(self.xml_dir, logger=self.verbose_logger)
+			delete_directory(self.temp_dir, logger=self.verbose_logger)
+			if not self.xml_only:
+				delete_directory(self.html_dir, logger=self.verbose_logger)
+			self.temp_dir.mkdir(exist_ok=True, parents=True)
+			self.temp_pages_dir.mkdir(exist_ok=True, parents=True)
 
 			# doxygen
 			if doxygen_path is not None:
 				doxygen_path = coerce_path(doxygen_path).resolve()
 				if not doxygen_path.exists() and Path(str(doxygen_path) + r'.exe').exists():
 					doxygen_path = Path(str(doxygen_path) + r'.exe')
 			else:
@@ -1454,17 +1451,15 @@
 				if not p.is_absolute():
 					p = Path(dirs.DATA, p)
 				extra_files.append((p, rf'poxy/{p.name}'))
 
 			config = dict()
 			if self.config_path.exists():
 				assert_existing_file(self.config_path)
-				config = pytomlpp.loads(
-					read_all_text_from_file(self.config_path, logger=self.verbose_logger if dry_run else self.logger)
-				)
+				config = pytomlpp.loads(read_all_text_from_file(self.config_path, logger=self.logger))
 			config = assert_no_unexpected_keys(config, self.__config_schema.validate(config))
 
 			self.warnings = Warnings(config)
 			if treat_warnings_as_errors:
 				self.warnings.treat_as_errors = True
 			self.verbose_value(r'Context.warnings', self.warnings)
 
@@ -1647,41 +1642,42 @@
 								if candidate_file.exists() and candidate_file.is_file(
 								) and candidate_file.stat().st_size <= 1024 * 1024 * 2:
 									self.changelog = candidate_file
 									break
 							if self.changelog or candidate_dir.parent == candidate_dir:
 								break
 							candidate_dir = candidate_dir.parent
-						if not self.changelog and not self.dry_run:
+						if not self.changelog:
 							self.warning(
 								rf'changelog: Option was set to true but no file with a known changelog file name could be found! Consider using an explicit path.'
 							)
 
 				else:
 					self.changelog = coerce_path(config['changelog'])
 					if not self.changelog.is_absolute():
 						self.changelog = Path(self.input_dir, self.changelog)
 					if not self.changelog.exists() or not self.changelog.is_file():
 						raise Error(rf'changelog: {config["changelog"]} did not exist or was not a file')
+			if self.changelog:
+				temp_changelog_path = Path(self.temp_pages_dir, r'poxy_changelog.md')
+				copy_file(self.changelog, temp_changelog_path, logger=self.verbose_logger)
+				self.changelog = temp_changelog_path
 			self.verbose_value(r'Context.changelog', self.changelog)
-			if self.changelog and not self.dry_run:
-				self.temp_pages_dir.mkdir(exist_ok=True, parents=True)
-				copy_file(self.changelog, Path(self.temp_pages_dir, r'poxy_changelog.md'), logger=self.verbose_logger)
-				self.changelog = Path(self.temp_pages_dir, r'poxy_changelog.md')
 
 			# sources (INPUT, FILE_PATTERNS, STRIP_FROM_PATH, STRIP_FROM_INC_PATH, EXTRACT_ALL)
 			self.sources = Sources(
 				config,
 				r'sources',
 				self.input_dir,
 				additional_inputs=(
-				self.temp_pages_dir if not self.dry_run else None,
-				self.changelog if self.changelog and not self.dry_run else None, *[f for f, d in self.blog_files]
+				self.temp_pages_dir,  #
+				self.changelog if self.changelog else None,
+				*[f for f, d in self.blog_files]
 				),
-				additional_strip_paths=(self.temp_pages_dir if not self.dry_run else None, )
+				additional_strip_paths=(self.temp_pages_dir, )
 			)
 			self.verbose_object(r'Context.sources', self.sources)
 
 			# images (IMAGE_PATH)
 			self.images = Inputs(
 				config,
 				r'images',
@@ -1719,53 +1715,84 @@
 						source = source.resolve()
 						self.tagfiles[str(source)] = (source, dest)
 			for k, v in self.tagfiles.items():
 				if isinstance(v, (Path, str)):
 					assert_existing_file(k)
 			self.verbose_value(r'Context.tagfiles', self.tagfiles)
 
-			# m.css navbar
-			if r'navbar' in config:
+			# navbar
+			if 1:
+				# initialize
 				self.navbar = []
-				for v in coerce_collection(config['navbar']):
-					val = v.strip().lower()
-					if val:
-						self.navbar.append(val)
-			else:
-				self.navbar = copy.deepcopy(Defaults.navbar)
-			for i in range(len(self.navbar)):
-				if self.navbar[i] == 'classes':
-					self.navbar[i] = 'annotated'
-				elif self.navbar[i] == 'groups':
-					self.navbar[i] = 'modules'
-			# repo buttons
-			if not self.repo:
-				# remove all repo buttons if there's no repo
-				for KEY in (r'repo', r'repository', *repos.KEYS):
-					if KEY in self.navbar:
-						self.navbar.remove(KEY)
-			else:
-				# remove repo buttons matching an uninstantiated repo type
-				for TYPE in repos.TYPES:
-					if not isinstance(self.repo, TYPE) and TYPE.KEY in self.navbar:
-						self.navbar.remove(TYPE.KEY)
-				# sub all remaining repo key aliases for simply 'repo'
+				if r'navbar' in config:
+					for v in coerce_collection(config['navbar']):
+						val = v.strip()
+						if val:
+							self.navbar.append(val)
+				else:
+					self.navbar = list(copy.deepcopy(Defaults.navbar))
+
+				# expand 'default' and 'all'
+				new_navbar = []
+				for link in self.navbar:
+					if link == r'all':
+						new_navbar += [*Defaults.navbar_all]
+					elif link == r'default':
+						new_navbar += [*Defaults.navbar]
+					else:
+						new_navbar.append(link)
+				self.navbar = new_navbar
+
+				# normalize aliases
 				for i in range(len(self.navbar)):
-					if self.navbar[i] in (r'repository', *repos.KEYS):
+					if self.navbar[i] == r'annotated':  # 'annotated' is doxygen-speak for 'classes'
+						self.navbar[i] = r'classes'
+					elif self.navbar[i] == r'modules':  # 'modules' is doxygen-speak for 'groups'
+						self.navbar[i] = r'groups'
+					elif self.navbar[i] == r'repository':
 						self.navbar[i] = r'repo'
-				# add a repo button to the end if none was present
-				if r'repo' not in self.navbar:
-					self.navbar.append(r'repo')
-			# theme button
-			if self.theme != r'custom' and r'theme' not in self.navbar:
-				self.navbar.append(r'theme')
-			if self.theme == r'custom' and r'theme' in self.navbar:
-				self.navbar.remove(r'theme')
-			self.navbar = tuple(self.navbar)
-			self.verbose_value(r'Context.navbar', self.navbar)
+
+				# repo logic
+				if not self.repo:
+					for KEY in (r'repo', *repos.KEYS):
+						if KEY in self.navbar:
+							self.navbar.remove(KEY)
+				else:
+					# remove repo buttons matching an uninstantiated repo type
+					for TYPE in repos.TYPES:
+						if not isinstance(self.repo, TYPE) and TYPE.KEY in self.navbar:
+							self.navbar.remove(TYPE.KEY)
+					# sub all remaining repo key aliases for simply 'repo'
+					for i in range(len(self.navbar)):
+						if self.navbar[i] in repos.KEYS:
+							self.navbar[i] = r'repo'
+					# add a repo button to the end if none was present
+					if r'repo' not in self.navbar:
+						self.navbar.append(r'repo')
+
+				# theme logic
+				if self.theme != r'custom' and r'theme' not in self.navbar:
+					self.navbar.append(r'theme')
+				if self.theme == r'custom' and r'theme' in self.navbar:
+					self.navbar.remove(r'theme')
+
+				# remove duplicate keywords
+				seen_keywords = set()
+				new_navbar = []
+				for nav in self.navbar:
+					if nav in (
+						r'files', r'pages', r'modules', r'namespaces', r'annotated', r'concepts', r'repo', r'theme'
+					):
+						if nav not in seen_keywords:
+							seen_keywords.add(nav)
+							new_navbar.append(nav)
+					else:
+						new_navbar.append(nav)
+				self.navbar = tuple(new_navbar)
+				self.verbose_value(r'Context.navbar', self.navbar)
 
 			# <meta> tags
 			self.meta_tags = {}
 			for k, v in extract_kvps(config, 'meta_tags', allow_blank_values=True).items():
 				self.meta_tags[k] = v
 			self.verbose_value(r'Context.meta_tags', self.meta_tags)
 
@@ -1927,22 +1954,20 @@
 			# html_header (HTML_HEADER in m.css)
 			self.html_header = ''
 			if r'html_header' in config:
 				self.html_header = str(config[r'html_header']).strip()
 			self.verbose_value(r'Context.html_header', self.html_header)
 
 		# init emoji db
-		self.emoji = None
-		if not self.dry_run:
-			self.emoji = emoji.Database()
+		self.emoji = emoji.Database()
 
 	def __enter__(self):
 		return self
 
 	def __exit__(self, type, value, traceback):
-		if not self.dry_run and self.cleanup:
+		if self.cleanup:
 			delete_directory(self.temp_dir, logger=self.verbose_logger)
 			if not self.xml_only:
 				delete_directory(self.xml_dir, logger=self.verbose_logger)
 
 	def __bool__(self):
 		return True
```

### Comparing `poxy-0.9.0/poxy/repos.py` & `poxy-0.9.1/poxy/repos.py`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/poxy/run.py` & `poxy-0.9.1/poxy/run.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,26 +7,36 @@
 The 'actually do the thing' module.
 """
 
 import os
 import subprocess
 import concurrent.futures as futures
 import tempfile
-import requests
 from lxml import etree
 from io import BytesIO, StringIO
 from .utils import *
-from . import project
+from .project import Context
 from . import doxygen
 from . import soup
 from . import fixers
 from .svg import SVG
 from distutils.dir_util import copy_tree
 
 #=======================================================================================================================
+# HELPERS
+#=======================================================================================================================
+
+
+
+def make_temp_file():
+	return tempfile.SpooledTemporaryFile(mode='w+', newline='\n', encoding='utf-8')
+
+
+
+#=======================================================================================================================
 # PRE/POST PROCESSORS
 #=======================================================================================================================
 
 _doxygen_overrides = (
 	(r'ALLEXTERNALS', False),
 	(r'ALLOW_UNICODE_NAMES', False),
 	(r'ALWAYS_DETAILED_SEC', False),
@@ -137,959 +147,1052 @@
 	(r'WARN_LOGFILE', None),
 	(r'XML_NS_MEMB_FILE_SCOPE', True),
 	(r'XML_PROGRAMLISTING', False),
 )
 
 
 
-def preprocess_doxyfile(context):
+def preprocess_doxyfile(context: Context):
 	assert context is not None
-	assert isinstance(context, project.Context)
+	assert isinstance(context, Context)
 
 	with doxygen.Doxyfile(
 		input_path=None,
-		output_path=context.doxyfile_path if not context.dry_run else None,
+		output_path=context.doxyfile_path,
 		cwd=context.input_dir,
 		logger=context.verbose_logger,
 		doxygen_path=context.doxygen_path
-	) as df, StringIO(newline='\n') as conf_py:
+	) as df:
 
 		df.append()
 		df.append(r'#---------------------------------------------------------------------------')
 		df.append(r'# marzer/poxy')
 		df.append(r'#---------------------------------------------------------------------------', end='\n\n')
 
-		# apply regular doxygen settings
-		if 1:
+		df.append(r'# doxygen default overrides', end='\n\n')  # ----------------------------------------
 
-			df.append(r'# doxygen default overrides', end='\n\n')  # ----------------------------------------
+		global _doxygen_overrides
+		for k, v in _doxygen_overrides:
+			df.set_value(k, v)
 
-			global _doxygen_overrides
-			for k, v in _doxygen_overrides:
-				df.set_value(k, v)
+		df.append()
+		df.append(r'# general config', end='\n\n')  # ---------------------------------------------------
 
-			df.append()
-			df.append(r'# general config', end='\n\n')  # ---------------------------------------------------
+		df.set_value(r'OUTPUT_DIRECTORY', context.output_dir)
+		df.set_value(r'XML_OUTPUT', context.xml_dir)
+		df.set_value(r'PROJECT_NAME', context.name)
+		df.set_value(r'PROJECT_BRIEF', context.description)
+		df.set_value(r'PROJECT_LOGO', context.logo)
+		df.set_value(r'SHOW_INCLUDE_FILES', context.show_includes)
+		df.set_value(r'INTERNAL_DOCS', context.internal_docs)
+		df.add_value(
+			r'ENABLED_SECTIONS', (r'private', r'internal') if context.internal_docs else (r'public', r'external')
+		)
+		df.add_value(r'ENABLED_SECTIONS', r'poxy_supports_concepts')
 
-			df.set_value(r'OUTPUT_DIRECTORY', context.output_dir)
-			df.set_value(r'XML_OUTPUT', context.xml_dir)
-			df.set_value(r'PROJECT_NAME', context.name)
-			df.set_value(r'PROJECT_BRIEF', context.description)
-			df.set_value(r'PROJECT_LOGO', context.logo)
-			df.set_value(r'SHOW_INCLUDE_FILES', context.show_includes)
-			df.set_value(r'INTERNAL_DOCS', context.internal_docs)
-			df.add_value(
-				r'ENABLED_SECTIONS', (r'private', r'internal') if context.internal_docs else (r'public', r'external')
+		if context.generate_tagfile:
+			context.tagfile_path = Path(
+				context.output_dir, rf'{context.name.replace(" ","_")}.tagfile.xml' if context.name else r'tagfile.xml'
 			)
-			df.add_value(r'ENABLED_SECTIONS', r'poxy_supports_concepts')
+			df.set_value(r'GENERATE_TAGFILE', context.tagfile_path.name)
+		else:
+			df.set_value(r'GENERATE_TAGFILE', None)
 
-			if context.generate_tagfile:
-				context.tagfile_path = Path(
-					context.output_dir,
-					rf'{context.name.replace(" ","_")}.tagfile.xml' if context.name else r'tagfile.xml'
-				)
-				df.set_value(r'GENERATE_TAGFILE', context.tagfile_path.name)
-			else:
-				df.set_value(r'GENERATE_TAGFILE', None)
+		df.set_value(r'NUM_PROC_THREADS', min(context.threads, 32))
+		df.add_value(r'CLANG_OPTIONS', rf'-std=c++{context.cpp%100}')
+		df.add_value(r'CLANG_OPTIONS', r'-Wno-everything')
+
+		home_md_path = None
+		for home_md in (r'HOME.md', r'home.md', r'INDEX.md', r'index.md', r'README.md', r'readme.md'):
+			p = Path(context.input_dir, home_md)
+			if p.exists() and p.is_file():
+				home_md_path = p
+				break
+		if home_md_path is not None:
+			home_md_temp_path = Path(context.temp_pages_dir, r'home.md')
+			copy_file(home_md_path, home_md_temp_path, logger=context.verbose_logger)
+			df.set_value(r'USE_MDFILE_AS_MAINPAGE', home_md_temp_path)
 
-			df.set_value(r'NUM_PROC_THREADS', min(context.threads, 32))
-			df.add_value(r'CLANG_OPTIONS', rf'-std=c++{context.cpp%100}')
-			df.add_value(r'CLANG_OPTIONS', r'-Wno-everything')
-
-			home_md_path = None
-			for home_md in (r'HOME.md', r'home.md', r'INDEX.md', r'index.md', r'README.md', r'readme.md'):
-				p = Path(context.input_dir, home_md)
-				if p.exists() and p.is_file():
-					home_md_path = p
-					break
-			if home_md_path is not None:
-				home_md_temp_path = Path(context.temp_pages_dir, r'home.md')
-				if not context.dry_run:
-					copy_file(home_md_path, home_md_temp_path, logger=context.verbose_logger)
-				df.set_value(r'USE_MDFILE_AS_MAINPAGE', home_md_temp_path)
+		df.append()
+		df.append(r'# context.warnings', end='\n\n')  # ---------------------------------------------------
 
-			df.append()
-			df.append(r'# context.warnings', end='\n\n')  # ---------------------------------------------------
+		df.set_value(r'WARNINGS', context.warnings.enabled)
+		df.set_value(r'WARN_AS_ERROR', False)  # we do this ourself
+		df.set_value(r'WARN_IF_UNDOCUMENTED', context.warnings.undocumented)
 
-			df.set_value(r'WARNINGS', context.warnings.enabled)
-			df.set_value(r'WARN_AS_ERROR', False)  # we do this ourself
-			df.set_value(r'WARN_IF_UNDOCUMENTED', context.warnings.undocumented)
+		df.append()
+		df.append(r'# context.sources', end='\n\n')  # ----------------------------------------------------
+
+		df.add_value(r'INPUT', context.sources.paths)
+		df.set_value(r'FILE_PATTERNS', context.sources.patterns)
+		df.add_value(r'EXCLUDE', context.html_dir)
+		df.add_value(r'STRIP_FROM_PATH', context.sources.strip_paths)
+		df.set_value(r'EXTRACT_ALL', context.sources.extract_all)
+
+		df.append()
+		df.append(r'# context.examples', end='\n\n')  # ----------------------------------------------------
+
+		df.add_value(r'EXAMPLE_PATH', context.examples.paths)
+		df.set_value(r'EXAMPLE_PATTERNS', context.examples.patterns)
 
+		if context.images.paths:  # ----------------------------------------------------
 			df.append()
-			df.append(r'# context.sources', end='\n\n')  # ----------------------------------------------------
+			df.append(r'# context.images', end='\n\n')
+			df.add_value(r'IMAGE_PATH', context.images.paths)
 
-			df.add_value(r'INPUT', context.sources.paths)
-			df.set_value(r'FILE_PATTERNS', context.sources.patterns)
-			df.add_value(r'EXCLUDE', context.html_dir)
-			df.add_value(r'STRIP_FROM_PATH', context.sources.strip_paths)
-			df.set_value(r'EXTRACT_ALL', context.sources.extract_all)
+		if context.tagfiles:  # ----------------------------------------------------
+			df.append()
+			df.append(r'# context.tagfiles', end='\n\n')
+			df.add_value(r'TAGFILES', [rf'{file}={dest}' for _, (file, dest) in context.tagfiles.items()])
 
+		if context.aliases:  # ----------------------------------------------------
 			df.append()
-			df.append(r'# context.examples', end='\n\n')  # ----------------------------------------------------
+			df.append(r'# context.aliases', end='\n\n')
+			df.add_value(r'ALIASES', [rf'{k}={v}' for k, v in context.aliases.items()])
 
-			df.add_value(r'EXAMPLE_PATH', context.examples.paths)
-			df.set_value(r'EXAMPLE_PATTERNS', context.examples.patterns)
+		if context.macros:  # ----------------------------------------------------
+			df.append()
+			df.append(r'# context.macros', end='\n\n')
+			df.add_value(r'PREDEFINED', [rf'{k}={v}' for k, v in context.macros.items()])
 
-			if context.images.paths:  # ----------------------------------------------------
-				df.append()
-				df.append(r'# context.images', end='\n\n')
-				df.add_value(r'IMAGE_PATH', context.images.paths)
-
-			if context.tagfiles:  # ----------------------------------------------------
-				df.append()
-				df.append(r'# context.tagfiles', end='\n\n')
-				df.add_value(r'TAGFILES', [rf'{file}={dest}' for _, (file, dest) in context.tagfiles.items()])
-
-			if context.aliases:  # ----------------------------------------------------
-				df.append()
-				df.append(r'# context.aliases', end='\n\n')
-				df.add_value(r'ALIASES', [rf'{k}={v}' for k, v in context.aliases.items()])
-
-			if context.macros:  # ----------------------------------------------------
-				df.append()
-				df.append(r'# context.macros', end='\n\n')
-				df.add_value(r'PREDEFINED', [rf'{k}={v}' for k, v in context.macros.items()])
+		df.cleanup()
+		context.verbose(r'Doxyfile:')
+		context.verbose(df.get_text(), indent=r'    ')
 
-		# build HTML_HEADER
-		html_header = ''
-		if 1:
-			# stylesheets
-			for stylesheet in context.stylesheets:
-				html_header += f'<link href="{stylesheet}" rel="stylesheet" referrerpolicy="no-referrer" />\n'
-			# scripts
-			for script in context.scripts:
-				html_header += f'<script src="{script}"></script>\n'
-			if context.theme != r'custom':
-				html_header += f'<script>initialize_theme("{context.theme}");</script>\n'
-			# metadata
-			def add_meta_kvp(key_name, key, content):
-				nonlocal html_header
-				html_header += f'<meta {key_name}="{key}" content="{content}">\n'
-
-			add_meta = lambda key, content: add_meta_kvp(r'name', key, content)
-			add_property = lambda key, content: add_meta_kvp(r'property', key, content)
-			add_itemprop = lambda key, content: add_meta_kvp(r'itemprop', key, content)
-			# metadata - project name
-			if context.name:
-				if r'twitter:title' not in context.meta_tags:
-					add_meta(r'twitter:title', context.name)
-				add_property(r'og:title', context.name)
-				add_itemprop(r'name', context.name)
-			# metadata - project author
-			if context.author:
-				if r'author' not in context.meta_tags:
-					add_meta(r'author', context.author)
-				add_property(r'article:author', context.author)
-			# metadata - project description
-			if context.description:
-				if r'description' not in context.meta_tags:
-					add_meta(r'description', context.description)
-				if r'twitter:description' not in context.meta_tags:
-					add_meta(r'twitter:description', context.description)
-				add_property(r'og:description', context.description)
-				add_itemprop(r'description', context.description)
-			# metadata - robots
-			if not context.robots:
-				if r'robots' not in context.meta_tags:
-					add_meta(r'robots', r'noindex, nofollow')
-				if r'googlebot' not in context.meta_tags:
-					add_meta(r'googlebot', r'noindex, nofollow')
-			# metadata - misc
-			if r'format-detection' not in context.meta_tags:
-				add_meta(r'format-detection', r'telephone=no')
-			if r'generator' not in context.meta_tags:
-				add_meta(r'generator', rf'Poxy v{context.version_string}')
-			if r'referrer' not in context.meta_tags:
-				add_meta(r'referrer', r'strict-origin-when-cross-origin')
-			# metadata - additional user-specified tags
-			for name, content in context.meta_tags.items():
-				add_meta(name, content)
-			# html_header
-			if context.html_header:
-				html_header += f'{context.html_header}\n'
-			html_header = html_header.rstrip()
 
-		# build m.css conf.py
-		if 1:
-			conf = lambda s='', end='\n': print(reindent(s, indent=''), file=conf_py, end=end)
-			conf(rf"DOXYFILE = r'{context.doxyfile_path}'")
-			conf(r"STYLESHEETS = []")  # suppress the default behaviour
-			conf(rf'HTML_HEADER = """{html_header}"""')
-			if context.theme == r'dark':
-				conf(r"THEME_COLOR = '#22272e'")
-			elif context.theme == r'light':
-				conf(r"THEME_COLOR = '#cb4b16'")
-			if not df.contains(r'M_FAVICON'):
-				if context.favicon:
-					conf(rf"FAVICON = r'{context.favicon}'")
-				elif context.theme == r'dark':
-					conf(rf"FAVICON = 'favicon-dark.png'")
-				elif context.theme == r'light':
-					conf(rf"FAVICON = 'favicon-light.png'")
-			if not df.contains(r'M_SHOW_UNDOCUMENTED'):
-				conf(rf'SHOW_UNDOCUMENTED = {context.sources.extract_all}')
-			if not df.contains(r'M_CLASS_TREE_EXPAND_LEVELS'):
-				conf(r'CLASS_INDEX_EXPAND_LEVELS = 3')
-			if not df.contains(r'M_FILE_TREE_EXPAND_LEVELS'):
-				conf(r'FILE_INDEX_EXPAND_LEVELS = 3')
-			if not df.contains(r'M_EXPAND_INNER_TYPES'):
-				conf(r'CLASS_INDEX_EXPAND_INNER = True')
-			if not df.contains(r'M_SEARCH_DOWNLOAD_BINARY'):
-				conf(r'SEARCH_DOWNLOAD_BINARY = False')
-			if not df.contains(r'M_SEARCH_DISABLED'):
-				conf(r'SEARCH_DISABLED = False')
-			if not df.contains(r'M_LINKS_NAVBAR1') and not df.contains(r'M_LINKS_NAVBAR2'):
-				navbars = ([], [])
-				if context.navbar:
-					bar = [v for v in context.navbar]
-					for i in range(len(bar)):
-						if bar[i] == r'repo' and context.repo:
-							icon_path = Path(dirs.DATA, context.repo.icon_filename)
-							if icon_path.exists():
-								svg = SVG(icon_path, logger=context.verbose_logger, root_id=r'poxy-repo-icon')
-								bar[i] = (
-									rf'<a title="View on {type(context.repo).__name__}" '
-									+ rf'target="_blank" href="{context.repo.uri}" '
-									+ rf'class="poxy-icon repo {context.repo.KEY}">{svg}</a>', []
-								)
-							else:
-								bar[i] = None
-						elif bar[i] == r'theme':
-							svg = SVG(
-								Path(dirs.DATA, r'poxy-icon-theme.svg'),
-								logger=context.verbose_logger,
-								root_id=r'poxy-theme-switch-img'
-							)
-							bar[i] = (
-								r'<a title="Toggle dark and light themes" '
-								+ r'id="poxy-theme-switch" href="javascript:void(null);" role="button" '
-								+ rf'class="poxy-icon theme" onClick="toggle_theme();">{svg}</a>', []
-							)
-					bar = [b for b in bar if b is not None]
-					split = min(max(int(len(bar) / 2) + len(bar) % 2, 2), len(bar))
-					for b, i in ((bar[:split], 0), (bar[split:], 1)):
-						for j in range(len(b)):
-							if isinstance(b[j], tuple):
-								navbars[i].append(b[j])
-							else:
-								navbars[i].append((None, b[j], []))
-				for i in (0, 1):
-					if navbars[i]:
-						conf(f'LINKS_NAVBAR{i+1} = [\n\t', end='')
-						conf(',\n\t'.join([rf'{b}' for b in navbars[i]]))
-						conf(r']')
-					else:
-						conf(rf'LINKS_NAVBAR{i+1} = []')
-			if not df.contains(r'M_PAGE_FINE_PRINT'):
-				conf(r"FINE_PRINT = r'''")
-				footer = []
-				if context.repo:
-					footer.append(rf'<a href="{context.repo.uri}" target="_blank">{type(context.repo).__name__}</a>')
-					footer.append(rf'<a href="{context.repo.issues_uri}" target="_blank">Report an issue</a>')
-				if context.changelog:
-					footer.append(rf'<a href="md_poxy_changelog.html">Changelog</a>')
-				if context.license and context.license[r'uri']:
-					footer.append(rf'<a href="{context.license["uri"]}" target="_blank">License</a>')
-				if context.generate_tagfile:
-					footer.append(
-						rf'<a href="{context.tagfile_path.name}" target="_blank" type="text/xml" download>Doxygen tagfile</a>'
-					)
-				if footer:
-					for i in range(1, len(footer)):
-						footer[i] = r' &bull; ' + footer[i]
-					footer.append(r'<br><br>')
-				footer.append(r'Site generated using <a href="https://github.com/marzer/poxy/">Poxy</a>')
-				for i in range(len(footer)):
-					conf(rf"    {footer[i]}")
-				conf(r"'''")
 
-		conf_py_text = conf_py.getvalue()
+def preprocess_changelog(context: Context):
+	assert context is not None
+	assert isinstance(context, Context)
+	if not context.changelog:
+		return
 
-		# write conf.py
-		if not context.dry_run:
-			context.verbose(rf'Writing {context.mcss_conf_path}')
-			with open(context.mcss_conf_path, r'w', encoding=r'utf-8', newline='\n') as f:
-				f.write(conf_py_text)
+	# make sure we're working with a temp copy, not the user's actual changelog
+	# (the actual copying should already be done in the context's initialization)
+	assert context.changelog.parent == context.temp_pages_dir
+	assert_existing_file(context.changelog)
+
+	text = read_all_text_from_file(context.changelog, logger=context.verbose_logger).strip()
+	text = text.replace('\r\n', '\n')
+	text = re.sub(r'\n<br[ \t]*/?><br[ \t]*/?>\n', r'', text)
+	if context.repo:
+		text = re.sub(r'#([0-9]+)', lambda m: rf'[#{m[1]}]({context.repo.make_issue_uri(m[1])})', text)
+		text = re.sub(r'!([0-9]+)', lambda m: rf'[!{m[1]}]({context.repo.make_pull_request_uri(m[1])})', text)
+		text = re.sub(r'@([a-zA-Z0-9_-]+)', lambda m: rf'[@{m[1]}]({context.repo.make_user_uri(m[1])})', text)
+	text = text.replace(r'&amp;', r'__poxy_thiswasan_amp')
+	text = text.replace(r'&#xFE0F;', r'__poxy_thiswasan_fe0f')
+	text = text.replace(r'@', r'__poxy_thiswasan_at')
+	if text.find(r'@tableofcontents') == -1 and text.find('\\tableofcontents') == -1 and text.find(r'[TOC]') == -1:
+		#text = f'[TOC]\n\n{text}'
+		nlnl = text.find(r'\n\n')
+		if nlnl != -1:
+			text = f'{text[:nlnl]}\n\n\\tableofcontents\n\n{text[nlnl:]}'
+		pass
+	text += '\n\n'
+	context.verbose(rf'Writing {context.changelog}')
+	with open(context.changelog, r'w', encoding=r'utf-8', newline='\n') as f:
+		f.write(text)
 
-		# clean and debug dump final doxyfile
-		df.cleanup()
-		if context.dry_run:
-			context.info(r'#====================================================================================')
-			context.info(rf'# generated by Poxy v{context.version_string}')
-			context.info(r'#====================================================================================')
-			context.info(df.get_text())
-			context.info(r'## ---------------------------------------------------------------------------------')
-			context.info(r'## m.css conf.py:')
-			context.info(r'## ---------------------------------------------------------------------------------')
-			context.info(conf_py_text, indent='## ')
-			context.info(r'#====================================================================================')
-		else:
-			context.verbose(r'Effective Doxyfile:')
-			context.verbose(df.get_text(), indent=r'    ')
-			context.verbose(r'    ## --------------------------------------------------------------------------')
-			context.verbose(r'    ## m.css conf.py:')
-			context.verbose(r'    ## --------------------------------------------------------------------------')
-			context.verbose(conf_py_text, indent='## ')
 
 
+def preprocess_tagfiles(context: Context):
+	assert context is not None
+	assert isinstance(context, Context)
+	if not context.unresolved_tagfiles:
+		return
+	with ScopeTimer(r'Resolving remote tagfiles', print_start=True, print_end=context.verbose_logger) as t:
+		for source, (file, _) in context.tagfiles.items():
+			if file.exists() or not is_uri(source):
+				continue
+			context.verbose(rf'Downloading {source}')
+			text = download_text(source, timeout=30)
+			context.verbose(rf'Writing {file}')
+			with open(file, 'w', encoding='utf-8', newline='\n') as f:
+				f.write(text)
 
-def postprocess_xml(context):
+
+
+def postprocess_xml(context: Context):
 	assert context is not None
-	assert isinstance(context, project.Context)
+	assert isinstance(context, Context)
 
 	xml_files = get_all_files(context.xml_dir, any=(r'*.xml'))
 	if not xml_files:
 		return
 
-	with ScopeTimer(
-		rf'Post-processing {len(xml_files) + len(context.tagfiles)} XML files',
-		print_start=True,
-		print_end=context.verbose_logger
-	):
-
-		pretty_print_xml = False
-		xml_parser = etree.XMLParser(
-			encoding='utf-8', remove_blank_text=pretty_print_xml, recover=True, remove_comments=True, ns_clean=True
-		)
-		write_xml_to_file = lambda xml, f: xml.write(
-			str(f), encoding='utf-8', xml_declaration=True, pretty_print=pretty_print_xml
-		)
+	context.info(rf'Post-processing {len(xml_files) + len(context.tagfiles)} XML files...')
 
-		inline_namespace_ids = None
-		if context.inline_namespaces:
-			inline_namespace_ids = [f'namespace{doxygen.mangle_name(ns)}' for ns in context.inline_namespaces]
-
-		implementation_header_data = None
-		implementation_header_mappings = None
-		implementation_header_innernamespaces = None
-		implementation_header_sectiondefs = None
-		implementation_header_unused_keys = None
-		implementation_header_unused_values = None
-		if context.implementation_headers:
-			implementation_header_data = [(
-				hp, os.path.basename(hp), doxygen.mangle_name(os.path.basename(hp)),
-				[(i, os.path.basename(i), doxygen.mangle_name(os.path.basename(i))) for i in impl]
-			) for hp, impl in context.implementation_headers]
-			implementation_header_unused_keys = set()
-			for hp, impl in context.implementation_headers:
-				implementation_header_unused_keys.add(hp)
-			implementation_header_unused_values = dict()
-			for hdata in implementation_header_data:
-				for (ip, ifn, iid) in hdata[3]:
-					implementation_header_unused_values[iid] = (ip, hdata[0])
-			implementation_header_mappings = dict()
-			implementation_header_innernamespaces = dict()
-			implementation_header_sectiondefs = dict()
-			for hdata in implementation_header_data:
-				implementation_header_innernamespaces[hdata[2]] = []
-				implementation_header_sectiondefs[hdata[2]] = []
-				for (ip, ifn, iid) in hdata[3]:
-					implementation_header_mappings[iid] = hdata
+	pretty_print_xml = False
+	xml_parser = etree.XMLParser(
+		encoding='utf-8', remove_blank_text=pretty_print_xml, recover=True, remove_comments=True, ns_clean=True
+	)
+	write_xml_to_file = lambda xml, f: xml.write(
+		str(f), encoding='utf-8', xml_declaration=True, pretty_print=pretty_print_xml
+	)
 
-		# process xml files
-		if 1:
+	inline_namespace_ids = None
+	if context.inline_namespaces:
+		inline_namespace_ids = [f'namespace{doxygen.mangle_name(ns)}' for ns in context.inline_namespaces]
+
+	implementation_header_data = None
+	implementation_header_mappings = None
+	implementation_header_innernamespaces = None
+	implementation_header_sectiondefs = None
+	implementation_header_unused_keys = None
+	implementation_header_unused_values = None
+	if context.implementation_headers:
+		implementation_header_data = [(
+			hp, os.path.basename(hp), doxygen.mangle_name(os.path.basename(hp)),
+			[(i, os.path.basename(i), doxygen.mangle_name(os.path.basename(i))) for i in impl]
+		) for hp, impl in context.implementation_headers]
+		implementation_header_unused_keys = set()
+		for hp, impl in context.implementation_headers:
+			implementation_header_unused_keys.add(hp)
+		implementation_header_unused_values = dict()
+		for hdata in implementation_header_data:
+			for (ip, ifn, iid) in hdata[3]:
+				implementation_header_unused_values[iid] = (ip, hdata[0])
+		implementation_header_mappings = dict()
+		implementation_header_innernamespaces = dict()
+		implementation_header_sectiondefs = dict()
+		for hdata in implementation_header_data:
+			implementation_header_innernamespaces[hdata[2]] = []
+			implementation_header_sectiondefs[hdata[2]] = []
+			for (ip, ifn, iid) in hdata[3]:
+				implementation_header_mappings[iid] = hdata
 
-			# pre-pass to delete junk files
-			if 1:
-				# 'file' entries for markdown and dox files
-				dox_files = [rf'*{doxygen.mangle_name(ext)}.xml' for ext in (r'.dox', r'.md')]
-				dox_files.append(r'md_home.xml')
-				for xml_file in get_all_files(context.xml_dir, any=dox_files):
-					delete_file(xml_file, logger=context.verbose_logger)
-
-				# 'dir' entries for empty directories
-				deleted = True
-				while deleted:
-					deleted = False
-					for xml_file in get_all_files(context.xml_dir, all=(r'dir*.xml')):
-						xml = etree.parse(str(xml_file), parser=xml_parser)
-						compounddef = xml.getroot().find(r'compounddef')
-						if compounddef is None or compounddef.get(r'kind') != r'dir':
-							continue
-						existing_inners = 0
-						for subtype in (r'innerfile', r'innerdir'):
-							for inner in compounddef.findall(subtype):
-								ref_file = Path(context.xml_dir, rf'{inner.get(r"refid")}.xml')
-								if ref_file.exists():
-									existing_inners = existing_inners + 1
-						if not existing_inners:
-							delete_file(xml_file, logger=context.verbose_logger)
-							deleted = True
-
-			extracted_implementation = False
-			tentative_macros = regex_or(context.code_blocks.macros)
-			macros = set()
-			cpp_tree = CppTree()
-			xml_files = get_all_files(context.xml_dir, any=(r'*.xml'))
-			tagfiles = [f for _, (f, _) in context.tagfiles.items()]
-			xml_files = xml_files + tagfiles
-			all_inners_by_type = {r'namespace': set(), r'class': set(), r'concept': set()}
-			for xml_file in xml_files:
+	setattr(context, r'compound_pages', dict())
+	setattr(context, r'compound_kinds', set())
 
-				context.verbose(rf'Pre-processing {xml_file}')
-				if xml_file.name == r'Doxyfile.xml':
-					continue
+	# process xml files
+	if 1:
 
-				xml = etree.parse(str(xml_file), parser=xml_parser)
-				root = xml.getroot()
-				changed = False
+		# pre-pass to delete junk files
+		if 1:
+			# 'file' entries for markdown and dox files
+			dox_files = [rf'*{doxygen.mangle_name(ext)}.xml' for ext in (r'.dox', r'.md')]
+			dox_files.append(r'md_home.xml')
+			for xml_file in get_all_files(context.xml_dir, any=dox_files):
+				delete_file(xml_file, logger=context.verbose_logger)
+
+			# 'dir' entries for empty directories
+			deleted = True
+			while deleted:
+				deleted = False
+				for xml_file in get_all_files(context.xml_dir, all=(r'dir*.xml')):
+					xml = etree.parse(str(xml_file), parser=xml_parser)
+					compounddef = xml.getroot().find(r'compounddef')
+					if compounddef is None or compounddef.get(r'kind') != r'dir':
+						continue
+					existing_inners = 0
+					for subtype in (r'innerfile', r'innerdir'):
+						for inner in compounddef.findall(subtype):
+							ref_file = Path(context.xml_dir, rf'{inner.get(r"refid")}.xml')
+							if ref_file.exists():
+								existing_inners = existing_inners + 1
+					if not existing_inners:
+						delete_file(xml_file, logger=context.verbose_logger)
+						deleted = True
+
+		extracted_implementation = False
+		tentative_macros = regex_or(context.code_blocks.macros)
+		macros = set()
+		cpp_tree = CppTree()
+		xml_files = get_all_files(context.xml_dir, any=(r'*.xml'))
+		tagfiles = [f for _, (f, _) in context.tagfiles.items()]
+		xml_files = xml_files + tagfiles
+		all_inners_by_type = {r'namespace': set(), r'class': set(), r'concept': set()}
+		for xml_file in xml_files:
+
+			context.verbose(rf'Pre-processing {xml_file}')
+			if xml_file.name == r'Doxyfile.xml':
+				continue
+
+			xml = etree.parse(str(xml_file), parser=xml_parser)
+			root = xml.getroot()
+			changed = False
+
+			# the doxygen index
+			if root.tag == r'doxygenindex':
+
+				# remove entries for files we might have explicitly deleted above
+				for compound in [
+					tag for tag in root.findall(r'compound') if tag.get(r'kind') in (r'file', r'dir', r'concept')
+				]:
+					ref_file = Path(context.xml_dir, rf'{compound.get(r"refid")}.xml')
+					if not ref_file.exists():
+						root.remove(compound)
+						changed = True
+
+				# extract namespaces, types and enum values for syntax highlighting
+				scopes = [
+					tag for tag in root.findall(r'compound')
+					if tag.get(r'kind') in (r'namespace', r'class', r'struct', r'union')
+				]
+				for scope in scopes:
+					scope_name = scope.find(r'name').text
 
-				# the doxygen index
-				if root.tag == r'doxygenindex':
+					# skip template members because they'll break the regex matchers
+					if scope_name.find(r'<') != -1:
+						continue
 
-					# remove entries for files we might have explicitly deleted above
-					for compound in [
-						tag for tag in root.findall(r'compound') if tag.get(r'kind') in (r'file', r'dir', r'concept')
-					]:
-						ref_file = Path(context.xml_dir, rf'{compound.get(r"refid")}.xml')
-						if not ref_file.exists():
-							root.remove(compound)
-							changed = True
-
-					# extract namespaces, types and enum values for syntax highlighting
-					scopes = [
-						tag for tag in root.findall(r'compound')
-						if tag.get(r'kind') in (r'namespace', r'class', r'struct', r'union')
-					]
-					for scope in scopes:
-						scope_name = scope.find(r'name').text
+					# regular types and namespaces
+					if scope.get(r'kind') in (r'class', r'struct', r'union'):
+						cpp_tree.add_type(scope_name)
+					elif scope.get(r'kind') == r'namespace':
+						cpp_tree.add_namespace(scope_name)
+
+					# nested enums
+					enum_tags = [tag for tag in scope.findall(r'member') if tag.get(r'kind') in (r'enum', r'enumvalue')]
+					enum_name = ''
+					for tag in enum_tags:
+						if tag.get(r'kind') == r'enum':
+							enum_name = rf'{scope_name}::{tag.find("name").text}'
+							cpp_tree.add_type(enum_name)
+						else:
+							assert enum_name
+							cpp_tree.add_enum_value(rf'{enum_name}::{tag.find("name").text}')
 
-						# skip template members because they'll break the regex matchers
-						if scope_name.find(r'<') != -1:
-							continue
+					# nested typedefs
+					typedefs = [tag for tag in scope.findall(r'member') if tag.get(r'kind') == r'typedef']
+					for typedef in typedefs:
+						cpp_tree.add_type(rf'{scope_name}::{typedef.find("name").text}')
+
+				# enumerate all compound pages and their types for later (e.g. HTML post-process)
+				for tag in root.findall(r'compound'):
+					refid = tag.get(r'refid')
+					filename = refid
+					if filename == r'indexpage':
+						filename = r'index'
+					filename = filename + r'.html'
+					context.compound_pages[filename] = {
+						r'kind': tag.get(r'kind'),
+						r'name': tag.find(r'name').text,
+						r'refid': refid
+					}
+					context.compound_kinds.add(tag.get(r'kind'))
+				context.verbose_value(r'Context.compound_pages', context.compound_pages)
+				context.verbose_value(r'Context.compound_kinds', context.compound_kinds)
+
+			# a tag file
+			elif root.tag == r'tagfile':
+				for compound in [
+					tag for tag in root.findall(r'compound')
+					if tag.get(r'kind') in (r'namespace', r'class', r'struct', r'union', r'concept')
+				]:
 
-						# regular types and namespaces
-						if scope.get(r'kind') in (r'class', r'struct', r'union'):
-							cpp_tree.add_type(scope_name)
-						elif scope.get(r'kind') == r'namespace':
-							cpp_tree.add_namespace(scope_name)
-
-						# nested enums
-						enum_tags = [
-							tag for tag in scope.findall(r'member') if tag.get(r'kind') in (r'enum', r'enumvalue')
-						]
-						enum_name = ''
-						for tag in enum_tags:
-							if tag.get(r'kind') == r'enum':
-								enum_name = rf'{scope_name}::{tag.find("name").text}'
-								cpp_tree.add_type(enum_name)
-							else:
-								assert enum_name
-								cpp_tree.add_enum_value(rf'{enum_name}::{tag.find("name").text}')
-
-						# nested typedefs
-						typedefs = [tag for tag in scope.findall(r'member') if tag.get(r'kind') == r'typedef']
-						for typedef in typedefs:
-							cpp_tree.add_type(rf'{scope_name}::{typedef.find("name").text}')
-
-					# enumerate all compound pages and their types for use later in the HTML post-process
-					pages = {}
-					for tag in root.findall(r'compound'):
-						refid = tag.get(r'refid')
-						filename = refid
-						if filename == r'indexpage':
-							filename = r'index'
-						filename = filename + r'.html'
-						pages[filename] = {r'kind': tag.get(r'kind'), r'name': tag.find(r'name').text, r'refid': refid}
-					context.__dict__[r'compound_pages'] = pages
-					context.verbose_value(r'Context.compound_pages', pages)
-
-				# a tag file
-				elif root.tag == r'tagfile':
-					for compound in [
-						tag for tag in root.findall(r'compound')
+					compound_name = compound.find(r'name').text
+					if compound_name.find(r'<') != -1:
+						continue
+
+					compound_type = compound.get(r'kind')
+					if compound_type in (r'class', r'struct', r'union', r'concept'):
+						cpp_tree.add_type(compound_name)
+					else:
+						cpp_tree.add_namespace(compound_name)
+
+					for member in [
+						tag for tag in compound.findall(r'member')
 						if tag.get(r'kind') in (r'namespace', r'class', r'struct', r'union', r'concept')
 					]:
 
-						compound_name = compound.find(r'name').text
-						if compound_name.find(r'<') != -1:
+						member_name = member.find(r'name').text
+						if member_name.find(r'<') != -1:
 							continue
 
-						compound_type = compound.get(r'kind')
-						if compound_type in (r'class', r'struct', r'union', r'concept'):
+						member_type = member.get(r'kind')
+						if member_type in (r'class', r'struct', r'union', r'concept'):
 							cpp_tree.add_type(compound_name)
 						else:
 							cpp_tree.add_namespace(compound_name)
 
-						for member in [
-							tag for tag in compound.findall(r'member')
-							if tag.get(r'kind') in (r'namespace', r'class', r'struct', r'union', r'concept')
-						]:
+			# some other compound definition
+			else:
+				compounddef = root.find(r'compounddef')
+				if compounddef is None:
+					context.warning(rf'{xml_file} did not contain a <compounddef>!')
+					continue
 
-							member_name = member.find(r'name').text
-							if member_name.find(r'<') != -1:
-								continue
-
-							member_type = member.get(r'kind')
-							if member_type in (r'class', r'struct', r'union', r'concept'):
-								cpp_tree.add_type(compound_name)
-							else:
-								cpp_tree.add_namespace(compound_name)
-
-				# some other compound definition
-				else:
-					compounddef = root.find(r'compounddef')
-					if compounddef is None:
-						context.warning(rf'{xml_file} did not contain a <compounddef>!')
-						continue
+				compound_id = compounddef.get(r'id')
+				if compound_id is None or not compound_id:
+					context.warning(rf'{xml_file} did not have attribute "id"!')
+					continue
 
-					compound_id = compounddef.get(r'id')
-					if compound_id is None or not compound_id:
-						context.warning(rf'{xml_file} did not have attribute "id"!')
-						continue
+				compound_kind = compounddef.get(r'kind')
+				if compound_kind is None or not compound_kind:
+					context.warning(rf'{xml_file} did not have attribute "kind"!')
+					continue
 
-					compound_kind = compounddef.get(r'kind')
-					if compound_kind is None or not compound_kind:
-						context.warning(rf'{xml_file} did not have attribute "kind"!')
-						continue
+				compound_name = compounddef.find(r'compoundname')
+				if compound_name is None or not compound_name.text:
+					context.warning(rf'{xml_file} did not contain a valid <compoundname>!')
+					continue
+				compound_name = str(compound_name.text).strip()
 
-					compound_name = compounddef.find(r'compoundname')
-					if compound_name is None or not compound_name.text:
-						context.warning(rf'{xml_file} did not contain a valid <compoundname>!')
-						continue
-					compound_name = str(compound_name.text).strip()
+				if compound_kind != r'page':
 
-					if compound_kind in (
-						r'namespace', r'class', r'struct', r'union', r'enum', r'file', r'group', r'concept'
-					):
-
-						# merge user-defined sections with the same name
-						sectiondefs = [
-							s for s in compounddef.findall(r'sectiondef') if s.get(r'kind') == r'user-defined'
-						]
-						sections = dict()
-						for section in sectiondefs:
-							header = section.find(r'header')
-							if header is not None and header.text:
-								if header.text not in sections:
-									sections[header.text] = []
-							sections[header.text].append(section)
-						for key, vals in sections.items():
-							if len(vals) > 1:
-								first_section = vals.pop(0)
-								for section in vals:
-									for member in section.findall(r'memberdef'):
-										section.remove(member)
-										first_section.append(member)
-									compounddef.remove(section)
+					# merge user-defined sections with the same name
+					sectiondefs = [s for s in compounddef.findall(r'sectiondef') if s.get(r'kind') == r'user-defined']
+					sections = dict()
+					for section in sectiondefs:
+						header = section.find(r'header')
+						if header is not None and header.text:
+							if header.text not in sections:
+								sections[header.text] = []
+						sections[header.text].append(section)
+					for key, vals in sections.items():
+						if len(vals) > 1:
+							first_section = vals.pop(0)
+							for section in vals:
+								for member in section.findall(r'memberdef'):
+									section.remove(member)
+									first_section.append(member)
+								compounddef.remove(section)
+								changed = True
+
+					# sort user-defined sections based on their name
+					sectiondefs = [s for s in compounddef.findall(r'sectiondef') if s.get(r'kind') == r'user-defined']
+					sectiondefs = [s for s in sectiondefs if s.find(r'header') is not None]
+					for section in sectiondefs:
+						compounddef.remove(section)
+					sectiondefs.sort(key=lambda s: s.find(r'header').text)
+					for section in sectiondefs:
+						compounddef.append(section)
+						changed = True
+
+					# per-section stuff
+					for section in compounddef.findall(r'sectiondef'):
+
+						# remove members which are listed multiple times because doxygen is idiotic:
+						members = [tag for tag in section.findall(r'memberdef')]
+						for i in range(len(members) - 1, 0, -1):
+							for j in range(i):
+								if members[i].get(r'id') == members[j].get(r'id'):
+									section.remove(members[i])
 									changed = True
+									break
 
-						# sort user-defined sections based on their name
-						sectiondefs = [
-							s for s in compounddef.findall(r'sectiondef') if s.get(r'kind') == r'user-defined'
-						]
-						sectiondefs = [s for s in sectiondefs if s.find(r'header') is not None]
-						for section in sectiondefs:
-							compounddef.remove(section)
-						sectiondefs.sort(key=lambda s: s.find(r'header').text)
-						for section in sectiondefs:
-							compounddef.append(section)
-							changed = True
-
-						# per-section stuff
-						for section in compounddef.findall(r'sectiondef'):
-
-							# remove members which are listed multiple times because doxygen is idiotic:
-							members = [tag for tag in section.findall(r'memberdef')]
-							for i in range(len(members) - 1, 0, -1):
-								for j in range(i):
-									if members[i].get(r'id') == members[j].get(r'id'):
-										section.remove(members[i])
-										changed = True
-										break
-
-							# fix functions where keywords like 'friend' have been erroneously included in the return type
-							if 1:
-								members = [
-									m for m in section.findall(r'memberdef')
-									if m.get(r'kind') in (r'friend', r'function')
-								]
-								attribute_keywords = ((r'constexpr', r'constexpr',
-									r'yes'), (r'consteval', r'consteval', r'yes'), (r'explicit', r'explicit',
-									r'yes'), (r'static', r'static', r'yes'), (r'friend', None, None),
-									(r'inline', r'inline', r'yes'), (r'virtual', r'virt', r'virtual'))
-								for member in members:
-									type = member.find(r'type')
-									if type is None or type.text is None:
-										continue
-									matched_bad_keyword = True
-									while matched_bad_keyword:
-										matched_bad_keyword = False
-										for kw, attr, attr_value in attribute_keywords:
-											if type.text == kw:  # constructors
-												type.text = ''
-											elif type.text.startswith(kw + ' '):
-												type.text = type.text[len(kw):].strip()
-											elif type.text.endswith(' ' + kw):
-												type.text = type.text[:len(kw)].strip()
-											else:
-												continue
-											matched_bad_keyword = True
-											changed = True
-											if attr is not None:
-												member.set(attr, attr_value)
-											elif kw == r'friend':
-												member.set(r'kind', r'friend')
-
-							# re-sort members to override Doxygen's weird and stupid sorting 'rules'
-							if 1:
-								sort_members_by_name = lambda tag: tag.find(r'name').text
-								members = [tag for tag in section.findall(r'memberdef')]
-								for tag in members:
-									section.remove(tag)
-								# fmt: off
-								# yapf: disable
-								groups = [
-									([tag for tag in members if tag.get(r'kind') == r'define'], True),  #
-									([tag for tag in members if tag.get(r'kind') == r'typedef'], True),
-									([tag for tag in members if tag.get(r'kind') == r'concept'], True),
-									([tag for tag in members if tag.get(r'kind') == r'enum'], True),
-									([tag for tag in members if tag.get(r'kind') == r'variable' and tag.get(r'static') == r'yes'], True),
-									([tag for tag in members if tag.get(r'kind') == r'variable' and tag.get(r'static') == r'no'], compound_kind not in (r'class', r'struct', r'union')),
-									([tag for tag in members if tag.get(r'kind') == r'function' and tag.get(r'static') == r'yes'], True),
-									([tag for tag in members if tag.get(r'kind') == r'function' and tag.get(r'static') == r'no'], True),
-									([tag for tag in members if tag.get(r'kind') == r'friend'], True)
-								]
-								# yapf: enable
-								# fmt: on
-								for group, sort in groups:
-									if sort:
-										group.sort(key=sort_members_by_name)
-									for tag in group:
-										members.remove(tag)
-										section.append(tag)
+						# fix functions where keywords like 'friend' have been erroneously included in the return type
+						if 1:
+							members = [
+								m for m in section.findall(r'memberdef') if m.get(r'kind') in (r'friend', r'function')
+							]
+							attribute_keywords = ((r'constexpr', r'constexpr',
+								r'yes'), (r'consteval', r'consteval', r'yes'), (r'explicit', r'explicit', r'yes'),
+								(r'static', r'static', r'yes'), (r'friend', None, None), (r'inline', r'inline',
+								r'yes'), (r'virtual', r'virt', r'virtual'))
+							for member in members:
+								type = member.find(r'type')
+								if type is None or type.text is None:
+									continue
+								matched_bad_keyword = True
+								while matched_bad_keyword:
+									matched_bad_keyword = False
+									for kw, attr, attr_value in attribute_keywords:
+										if type.text == kw:  # constructors
+											type.text = ''
+										elif type.text.startswith(kw + ' '):
+											type.text = type.text[len(kw):].strip()
+										elif type.text.endswith(' ' + kw):
+											type.text = type.text[:len(kw)].strip()
+										else:
+											continue
+										matched_bad_keyword = True
 										changed = True
-								# if we've missed any groups just glob them on the end
-								if members:
-									members.sort(key=sort_members_by_name)
+										if attr is not None:
+											member.set(attr, attr_value)
+										elif kw == r'friend':
+											member.set(r'kind', r'friend')
+
+						# re-sort members to override Doxygen's weird and stupid sorting 'rules'
+						if 1:
+							sort_members_by_name = lambda tag: tag.find(r'name').text
+							members = [tag for tag in section.findall(r'memberdef')]
+							for tag in members:
+								section.remove(tag)
+							# fmt: off
+							# yapf: disable
+							groups = [
+								([tag for tag in members if tag.get(r'kind') == r'define'], True),  #
+								([tag for tag in members if tag.get(r'kind') == r'typedef'], True),
+								([tag for tag in members if tag.get(r'kind') == r'concept'], True),
+								([tag for tag in members if tag.get(r'kind') == r'enum'], True),
+								([tag for tag in members if tag.get(r'kind') == r'variable' and tag.get(r'static') == r'yes'], True),
+								([tag for tag in members if tag.get(r'kind') == r'variable' and tag.get(r'static') == r'no'], compound_kind not in (r'class', r'struct', r'union')),
+								([tag for tag in members if tag.get(r'kind') == r'function' and tag.get(r'static') == r'yes'], True),
+								([tag for tag in members if tag.get(r'kind') == r'function' and tag.get(r'static') == r'no'], True),
+								([tag for tag in members if tag.get(r'kind') == r'friend'], True)
+							]
+							# yapf: enable
+							# fmt: on
+							for group, sort in groups:
+								if sort:
+									group.sort(key=sort_members_by_name)
+								for tag in group:
+									members.remove(tag)
+									section.append(tag)
 									changed = True
-									for tag in members:
-										section.append(tag)
+							# if we've missed any groups just glob them on the end
+							if members:
+								members.sort(key=sort_members_by_name)
+								changed = True
+								for tag in members:
+									section.append(tag)
 
-					# namespaces
-					if compound_kind == r'namespace':
+				# namespaces
+				if compound_kind == r'namespace':
 
-						# set inline namespaces
-						if context.inline_namespaces:
-							for nsid in inline_namespace_ids:
-								if compound_id == nsid:
-									compounddef.set(r'inline', r'yes')
-									changed = True
-									break
+					# set inline namespaces
+					if context.inline_namespaces:
+						for nsid in inline_namespace_ids:
+							if compound_id == nsid:
+								compounddef.set(r'inline', r'yes')
+								changed = True
+								break
 
-					# dirs
-					if compound_kind == r'dir':
+				# dirs
+				if compound_kind == r'dir':
 
-						# remove implementation headers
-						if context.implementation_headers:
-							for innerfile in compounddef.findall(r'innerfile'):
-								if innerfile.get(r'refid') in implementation_header_mappings:
-									compounddef.remove(innerfile)
+					# remove implementation headers
+					if context.implementation_headers:
+						for innerfile in compounddef.findall(r'innerfile'):
+							if innerfile.get(r'refid') in implementation_header_mappings:
+								compounddef.remove(innerfile)
+								changed = True
+
+				# files
+				if compound_kind == r'file':
+
+					# simplify the XML by removing junk not used by mcss
+					if not context.xml_only:
+						for tag in (r'includes', r'includedby', r'incdepgraph', r'invincdepgraph'):
+							for t in compounddef.findall(tag):
+								compounddef.remove(t)
+								changed = True
+
+					# get any macros for the syntax highlighter
+					for sectiondef in [
+						tag for tag in compounddef.findall(r'sectiondef') if tag.get(r'kind') == r'define'
+					]:
+						for memberdef in [
+							tag for tag in sectiondef.findall(r'memberdef') if tag.get(r'kind') == r'define'
+						]:
+							macro = memberdef.find(r'name').text
+							if not tentative_macros.fullmatch(macro):
+								macros.add(macro)
+
+					# rip the good bits out of implementation headers
+					if context.implementation_headers:
+						iid = compound_id
+						if iid in implementation_header_mappings:
+							hid = implementation_header_mappings[iid][2]
+							innernamespaces = compounddef.findall(r'innernamespace')
+							if innernamespaces:
+								implementation_header_innernamespaces[
+									hid] = implementation_header_innernamespaces[hid] + innernamespaces
+								extracted_implementation = True
+								if iid in implementation_header_unused_values:
+									del implementation_header_unused_values[iid]
+								for tag in innernamespaces:
+									compounddef.remove(tag)
 									changed = True
-
-					# files
-					if compound_kind == r'file':
-
-						# simplify the XML by removing junk not used by mcss
-						if not context.xml_only:
-							for tag in (r'includes', r'includedby', r'incdepgraph', r'invincdepgraph'):
-								for t in compounddef.findall(tag):
-									compounddef.remove(t)
+							sectiondefs = compounddef.findall(r'sectiondef')
+							if sectiondefs:
+								implementation_header_sectiondefs[
+									hid] = implementation_header_sectiondefs[hid] + sectiondefs
+								extracted_implementation = True
+								if iid in implementation_header_unused_values:
+									del implementation_header_unused_values[iid]
+								for tag in sectiondefs:
+									compounddef.remove(tag)
 									changed = True
 
-						# get any macros for the syntax highlighter
-						for sectiondef in [
-							tag for tag in compounddef.findall(r'sectiondef') if tag.get(r'kind') == r'define'
-						]:
-							for memberdef in [
-								tag for tag in sectiondef.findall(r'memberdef') if tag.get(r'kind') == r'define'
-							]:
-								macro = memberdef.find(r'name').text
-								if not tentative_macros.fullmatch(macro):
-									macros.add(macro)
-
-						# rip the good bits out of implementation headers
-						if context.implementation_headers:
-							iid = compound_id
-							if iid in implementation_header_mappings:
-								hid = implementation_header_mappings[iid][2]
-								innernamespaces = compounddef.findall(r'innernamespace')
-								if innernamespaces:
-									implementation_header_innernamespaces[
-										hid] = implementation_header_innernamespaces[hid] + innernamespaces
-									extracted_implementation = True
-									if iid in implementation_header_unused_values:
-										del implementation_header_unused_values[iid]
-									for tag in innernamespaces:
-										compounddef.remove(tag)
-										changed = True
-								sectiondefs = compounddef.findall(r'sectiondef')
-								if sectiondefs:
-									implementation_header_sectiondefs[
-										hid] = implementation_header_sectiondefs[hid] + sectiondefs
-									extracted_implementation = True
-									if iid in implementation_header_unused_values:
-										del implementation_header_unused_values[iid]
-									for tag in sectiondefs:
-										compounddef.remove(tag)
-										changed = True
+				# groups and namespaces
+				if compound_kind in (r'group', r'namespace'):
+
+					# fix inner(class|namespace|group|concept) sorting
+					inners = [tag for tag in compounddef.iterchildren() if tag.tag.startswith(r'inner')]
+					if inners:
+						changed = True
+						for tag in inners:
+							compounddef.remove(tag)
+						inners.sort(key=lambda tag: tag.text)
+						for tag in inners:
+							compounddef.append(tag)
+
+				# all namespace 'innerXXXXXX'
+				if compound_kind in (r'namespace', r'struct', r'class', r'union', r'concept'):
+					if compound_name.rfind(r'::') != -1:
+						all_inners_by_type[r'class' if compound_kind in (r'struct', r'union') else compound_kind].add(
+							(compound_id, compound_name)
+						)
 
-					# groups and namespaces
-					if compound_kind in (r'group', r'namespace'):
+			if changed and xml_file not in tagfiles:  # tagfiles are read-only - ensure we don't modify them
+				write_xml_to_file(xml, xml_file)
 
-						# fix inner(class|namespace|group|concept) sorting
-						inners = [tag for tag in compounddef.iterchildren() if tag.tag.startswith(r'inner')]
-						if inners:
-							changed = True
-							for tag in inners:
-								compounddef.remove(tag)
-							inners.sort(key=lambda tag: tag.text)
-							for tag in inners:
-								compounddef.append(tag)
-
-					# all namespace 'innerXXXXXX'
-					if compound_kind in (r'namespace', r'struct', r'class', r'union', r'concept'):
-						if compound_name.rfind(r'::') != -1:
-							all_inners_by_type[r'class' if compound_kind in (r'struct',
-								r'union') else compound_kind].add((compound_id, compound_name))
+		# add to syntax highlighter
+		context.code_blocks.namespaces.add(cpp_tree.matcher(CppTree.NAMESPACES))
+		context.code_blocks.types.add(cpp_tree.matcher(CppTree.TYPES))
+		context.code_blocks.enums.add(cpp_tree.matcher(CppTree.ENUM_VALUES))
+		for macro in macros:
+			context.code_blocks.macros.add(macro)
+		context.verbose_object(r'Context.code_blocks', context.code_blocks)
 
+		# fix up namespaces/classes that are missing <innerXXXX> nodes
+		if 1:
+			outer_namespaces = dict()
+			for inner_type, ids_and_names in all_inners_by_type.items():
+				for id, name in ids_and_names:
+					ns = name[:name.rfind(r'::')]
+					assert ns
+					if ns not in outer_namespaces:
+						outer_namespaces[ns] = []
+					outer_namespaces[ns].append((inner_type, id, name))
+			for ns, vals in outer_namespaces.items():
+				xml_file = None
+				for outer_type in (r'namespace', r'struct', r'class', r'union'):
+					f = Path(context.xml_dir, rf'{outer_type}{doxygen.mangle_name(ns)}.xml')
+					if f.exists():
+						xml_file = f
+						break
+				if not xml_file:
+					continue
+				xml = etree.parse(str(xml_file), parser=xml_parser)
+				compounddef = xml.getroot().find(r'compounddef')
+				if compounddef is None:
+					continue
+				changed = False
+				existing_inner_ids = set()
+				for inner_type in (r'class', r'namespace', r'concept'):
+					for elem in compounddef.findall(rf'inner{inner_type}'):
+						id = elem.get(r'refid')
+						if id:
+							existing_inner_ids.add(str(id))
+				for (inner_type, id, name) in vals:
+					if id not in existing_inner_ids:
+						elem = etree.SubElement(compounddef, rf'inner{inner_type}')
+						elem.text = name
+						elem.set(r'refid', id)
+						elem.set(r'prot', r'public')  # todo: this isn't necessarily correct
+						existing_inner_ids.add(id)
+						changed = True
 				if changed:
 					write_xml_to_file(xml, xml_file)
 
-			# add to syntax highlighter
-			context.code_blocks.namespaces.add(cpp_tree.matcher(CppTree.NAMESPACES))
-			context.code_blocks.types.add(cpp_tree.matcher(CppTree.TYPES))
-			context.code_blocks.enums.add(cpp_tree.matcher(CppTree.ENUM_VALUES))
-			for macro in macros:
-				context.code_blocks.macros.add(macro)
-
-			# fix up namespaces/classes that are missing <innerXXXX> nodes
-			if 1:
-				outer_namespaces = dict()
-				for inner_type, ids_and_names in all_inners_by_type.items():
-					for id, name in ids_and_names:
-						ns = name[:name.rfind(r'::')]
-						assert ns
-						if ns not in outer_namespaces:
-							outer_namespaces[ns] = []
-						outer_namespaces[ns].append((inner_type, id, name))
-				for ns, vals in outer_namespaces.items():
-					xml_file = None
-					for outer_type in (r'namespace', r'struct', r'class', r'union'):
-						f = Path(context.xml_dir, rf'{outer_type}{doxygen.mangle_name(ns)}.xml')
-						if f.exists():
-							xml_file = f
+		# merge extracted implementations
+		if extracted_implementation:
+			for (hp, hfn, hid, impl) in implementation_header_data:
+				xml_file = Path(context.xml_dir, rf'{hid}.xml')
+				context.verbose(rf'Merging implementation nodes into {xml_file}')
+				xml = etree.parse(str(xml_file), parser=xml_parser)
+				compounddef = xml.getroot().find(r'compounddef')
+				changed = False
+
+				innernamespaces = compounddef.findall(r'innernamespace')
+				for new_tag in implementation_header_innernamespaces[hid]:
+					matched = False
+					for existing_tag in innernamespaces:
+						if existing_tag.get(r'refid') == new_tag.get(r'refid'):
+							matched = True
 							break
-					if not xml_file:
-						continue
-					xml = etree.parse(str(xml_file), parser=xml_parser)
-					compounddef = xml.getroot().find(r'compounddef')
-					if compounddef is None:
-						continue
-					changed = False
-					existing_inner_ids = set()
-					for inner_type in (r'class', r'namespace', r'concept'):
-						for elem in compounddef.findall(rf'inner{inner_type}'):
-							id = elem.get(r'refid')
-							if id:
-								existing_inner_ids.add(str(id))
-					for (inner_type, id, name) in vals:
-						if id not in existing_inner_ids:
-							elem = etree.SubElement(compounddef, rf'inner{inner_type}')
-							elem.text = name
-							elem.set(r'refid', id)
-							elem.set(r'prot', r'public')  # todo: this isn't necessarily correct
-							existing_inner_ids.add(id)
-							changed = True
-					if changed:
-						write_xml_to_file(xml, xml_file)
-
-			# merge extracted implementations
-			if extracted_implementation:
-				for (hp, hfn, hid, impl) in implementation_header_data:
-					xml_file = Path(context.xml_dir, rf'{hid}.xml')
-					context.verbose(rf'Merging implementation nodes into {xml_file}')
-					xml = etree.parse(str(xml_file), parser=xml_parser)
-					compounddef = xml.getroot().find(r'compounddef')
-					changed = False
+					if not matched:
+						compounddef.append(new_tag)
+						innernamespaces.append(new_tag)
+						changed = True
+
+				sectiondefs = compounddef.findall(r'sectiondef')
+				for new_section in implementation_header_sectiondefs[hid]:
+					matched_section = False
+					for existing_section in sectiondefs:
+						if existing_section.get(r'kind') == new_section.get(r'kind'):
+							matched_section = True
+
+							memberdefs = existing_section.findall(r'memberdef')
+							new_memberdefs = new_section.findall(r'memberdef')
+							for new_memberdef in new_memberdefs:
+								matched = False
+								for existing_memberdef in memberdefs:
+									if existing_memberdef.get(r'id') == new_memberdef.get(r'id'):
+										matched = True
+										break
 
-					innernamespaces = compounddef.findall(r'innernamespace')
-					for new_tag in implementation_header_innernamespaces[hid]:
-						matched = False
-						for existing_tag in innernamespaces:
-							if existing_tag.get(r'refid') == new_tag.get(r'refid'):
-								matched = True
-								break
-						if not matched:
-							compounddef.append(new_tag)
-							innernamespaces.append(new_tag)
-							changed = True
-
-					sectiondefs = compounddef.findall(r'sectiondef')
-					for new_section in implementation_header_sectiondefs[hid]:
-						matched_section = False
-						for existing_section in sectiondefs:
-							if existing_section.get(r'kind') == new_section.get(r'kind'):
-								matched_section = True
-
-								memberdefs = existing_section.findall(r'memberdef')
-								new_memberdefs = new_section.findall(r'memberdef')
-								for new_memberdef in new_memberdefs:
-									matched = False
-									for existing_memberdef in memberdefs:
-										if existing_memberdef.get(r'id') == new_memberdef.get(r'id'):
-											matched = True
-											break
-
-									if not matched:
-										new_section.remove(new_memberdef)
-										existing_section.append(new_memberdef)
-										memberdefs.append(new_memberdef)
-										changed = True
-								break
+								if not matched:
+									new_section.remove(new_memberdef)
+									existing_section.append(new_memberdef)
+									memberdefs.append(new_memberdef)
+									changed = True
+							break
+
+					if not matched_section:
+						compounddef.append(new_section)
+						sectiondefs.append(new_section)
+						changed = True
 
-						if not matched_section:
-							compounddef.append(new_section)
-							sectiondefs.append(new_section)
-							changed = True
-
-					if changed:
-						implementation_header_unused_keys.remove(hp)
-						write_xml_to_file(xml, xml_file)
-
-			# sanity-check implementation header state
-			if implementation_header_unused_keys:
-				for key in implementation_header_unused_keys:
-					context.warning(rf"implementation_header: nothing extracted for '{key}'")
-			if implementation_header_unused_values:
-				for iid, idata in implementation_header_unused_values.items():
-					context.warning(rf"implementation_header: nothing extracted from '{idata[0]}' for '{idata[1]}'")
-
-		# delete the impl header xml files
-		if 1 and context.implementation_headers:
-			for hdata in implementation_header_data:
-				for (ip, ifn, iid) in hdata[3]:
-					delete_file(Path(context.xml_dir, rf'{iid}.xml'), logger=context.verbose_logger)
-
-		# scan through the files and substitute impl header ids and paths as appropriate
-		if 1 and context.implementation_headers:
-			xml_files = get_all_files(context.xml_dir, any=('*.xml'))
-			for xml_file in xml_files:
-				context.verbose(rf"Re-linking implementation headers in '{xml_file}'")
-				xml_text = read_all_text_from_file(xml_file, logger=context.verbose_logger)
-				for (hp, hfn, hid, impl) in implementation_header_data:
-					for (ip, ifn, iid) in impl:
-						#xml_text = xml_text.replace(f'refid="{iid}"',f'refid="{hid}"')
-						xml_text = xml_text.replace(rf'compoundref="{iid}"', f'compoundref="{hid}"')
-						xml_text = xml_text.replace(ip, hp)
-				with BytesIO(bytes(xml_text, 'utf-8')) as b:
-					xml = etree.parse(b, parser=xml_parser)
+				if changed:
+					implementation_header_unused_keys.remove(hp)
 					write_xml_to_file(xml, xml_file)
 
+		# sanity-check implementation header state
+		if implementation_header_unused_keys:
+			for key in implementation_header_unused_keys:
+				context.warning(rf"implementation_header: nothing extracted for '{key}'")
+		if implementation_header_unused_values:
+			for iid, idata in implementation_header_unused_values.items():
+				context.warning(rf"implementation_header: nothing extracted from '{idata[0]}' for '{idata[1]}'")
+
+	# delete the impl header xml files
+	if 1 and context.implementation_headers:
+		for hdata in implementation_header_data:
+			for (ip, ifn, iid) in hdata[3]:
+				delete_file(Path(context.xml_dir, rf'{iid}.xml'), logger=context.verbose_logger)
+
+	# scan through the files and substitute impl header ids and paths as appropriate
+	if 1 and context.implementation_headers:
+		xml_files = get_all_files(context.xml_dir, any=('*.xml'))
+		for xml_file in xml_files:
+			context.verbose(rf"Re-linking implementation headers in '{xml_file}'")
+			xml_text = read_all_text_from_file(xml_file, logger=context.verbose_logger)
+			for (hp, hfn, hid, impl) in implementation_header_data:
+				for (ip, ifn, iid) in impl:
+					#xml_text = xml_text.replace(f'refid="{iid}"',f'refid="{hid}"')
+					xml_text = xml_text.replace(rf'compoundref="{iid}"', f'compoundref="{hid}"')
+					xml_text = xml_text.replace(ip, hp)
+			with BytesIO(bytes(xml_text, 'utf-8')) as b:
+				xml = etree.parse(b, parser=xml_parser)
+				write_xml_to_file(xml, xml_file)
+
+	# convert the definition lists into compiled regexes since we've now extracted everything useful
+	context.code_blocks.namespaces = regex_or(
+		context.code_blocks.namespaces, pattern_prefix='(?:::)?', pattern_suffix='(?:::)?'
+	)
+	context.code_blocks.types = regex_or(context.code_blocks.types, pattern_prefix='(?:::)?', pattern_suffix='(?:::)?')
+	context.code_blocks.enums = regex_or(context.code_blocks.enums, pattern_prefix='(?:::)?')
+	context.code_blocks.string_literals = regex_or(context.code_blocks.string_literals)
+	context.code_blocks.numeric_literals = regex_or(context.code_blocks.numeric_literals)
+	context.code_blocks.macros = regex_or(context.code_blocks.macros)
+	context.autolinks = tuple([(re.compile('(?<![a-zA-Z_])' + expr + '(?![a-zA-Z_])'), uri)
+		for expr, uri in context.autolinks])
+
+
+
+def preprocess_mcss_config(context: Context):
+	assert context is not None
+	assert isinstance(context, Context)
+
+	# build HTML_HEADER
+	html_header = ''
+	if 1:
+		# stylesheets
+		for stylesheet in context.stylesheets:
+			html_header += f'<link href="{stylesheet}" rel="stylesheet" referrerpolicy="no-referrer" />\n'
+		# scripts
+		for script in context.scripts:
+			html_header += f'<script src="{script}"></script>\n'
+		if context.theme != r'custom':
+			html_header += f'<script>initialize_theme("{context.theme}");</script>\n'
+		# metadata
+		def add_meta_kvp(key_name, key, content):
+			nonlocal html_header
+			html_header += f'<meta {key_name}="{key}" content="{content}">\n'
+
+		add_meta = lambda key, content: add_meta_kvp(r'name', key, content)
+		add_property = lambda key, content: add_meta_kvp(r'property', key, content)
+		add_itemprop = lambda key, content: add_meta_kvp(r'itemprop', key, content)
+		# metadata - project name
+		if context.name:
+			if r'twitter:title' not in context.meta_tags:
+				add_meta(r'twitter:title', context.name)
+			add_property(r'og:title', context.name)
+			add_itemprop(r'name', context.name)
+		# metadata - project author
+		if context.author:
+			if r'author' not in context.meta_tags:
+				add_meta(r'author', context.author)
+			add_property(r'article:author', context.author)
+		# metadata - project description
+		if context.description:
+			if r'description' not in context.meta_tags:
+				add_meta(r'description', context.description)
+			if r'twitter:description' not in context.meta_tags:
+				add_meta(r'twitter:description', context.description)
+			add_property(r'og:description', context.description)
+			add_itemprop(r'description', context.description)
+		# metadata - robots
+		if not context.robots:
+			if r'robots' not in context.meta_tags:
+				add_meta(r'robots', r'noindex, nofollow')
+			if r'googlebot' not in context.meta_tags:
+				add_meta(r'googlebot', r'noindex, nofollow')
+		# metadata - misc
+		if r'format-detection' not in context.meta_tags:
+			add_meta(r'format-detection', r'telephone=no')
+		if r'generator' not in context.meta_tags:
+			add_meta(r'generator', rf'Poxy v{context.version_string}')
+		if r'referrer' not in context.meta_tags:
+			add_meta(r'referrer', r'strict-origin-when-cross-origin')
+		# metadata - additional user-specified tags
+		for name, content in context.meta_tags.items():
+			add_meta(name, content)
+		# html_header
+		if context.html_header:
+			html_header += f'{context.html_header}\n'
+		html_header = html_header.rstrip()
+
+	# build + write conf.py
+	with StringIO(newline='\n') as conf_py:
+		conf = lambda s='', end='\n': print(reindent(s, indent=''), file=conf_py, end=end)
+
+		# basic properties
+		conf(rf"DOXYFILE = r'{context.doxyfile_path}'")
+		conf(r"STYLESHEETS = []")  # suppress the default behaviour
+		conf(rf'HTML_HEADER = """{html_header}"""')
+		if context.theme == r'dark':
+			conf(r"THEME_COLOR = '#22272e'")
+		elif context.theme == r'light':
+			conf(r"THEME_COLOR = '#cb4b16'")
+		if context.favicon:
+			conf(rf"FAVICON = r'{context.favicon}'")
+		elif context.theme == r'dark':
+			conf(rf"FAVICON = 'favicon-dark.png'")
+		elif context.theme == r'light':
+			conf(rf"FAVICON = 'favicon-light.png'")
+		conf(rf'SHOW_UNDOCUMENTED = {context.sources.extract_all}')
+		conf(r'CLASS_INDEX_EXPAND_LEVELS = 3')
+		conf(r'FILE_INDEX_EXPAND_LEVELS = 3')
+		conf(r'CLASS_INDEX_EXPAND_INNER = True')
+		conf(r'SEARCH_DOWNLOAD_BINARY = False')
+		conf(r'SEARCH_DISABLED = False')
+
+		# navbar
+		NAVBAR_ALIASES = {
+			# poxy -> doxygen
+			r'classes': r'annotated',
+			r'groups': r'modules'
+		}
+		NAVBAR_TO_KIND = {
+			r'annotated': (r'class', r'struct', r'union'),
+			r'concepts': (r'concept', ),
+			r'namespaces': (r'namespace', ),
+			r'pages': (r'page', ),
+			r'modules': (r'group', ),
+			r'files': (r'file', r'dir')
+		}
+		navbar = ([], [])
+		if context.navbar:
+			# populate the navbar
+			bar = [(NAVBAR_ALIASES[b] if b in NAVBAR_ALIASES else b) for b in context.navbar]
+			# remove links to index pages that will have no entries
+			for i in range(len(bar)):
+				if bar[i] not in NAVBAR_TO_KIND:
+					continue
+				found = False
+				for kind in NAVBAR_TO_KIND[bar[i]]:
+					if kind in context.compound_kinds:
+						found = True
+						break
+				if not found:
+					bar[i] = None
+			bar = [b for b in bar if b is not None]
+			# handle theme and repo links
+			for i in range(len(bar)):
+				if bar[i] == r'repo' and context.repo:
+					icon_path = Path(dirs.DATA, context.repo.icon_filename)
+					if icon_path.exists():
+						svg = SVG(icon_path, logger=context.verbose_logger, root_id=r'poxy-repo-icon')
+						bar[i] = (
+							rf'<a title="View on {type(context.repo).__name__}" '
+							+ rf'target="_blank" href="{context.repo.uri}" '
+							+ rf'class="poxy-icon repo {context.repo.KEY}">{svg}</a>', []
+						)
+					else:
+						bar[i] = None
+				elif bar[i] == r'theme':
+					svg = SVG(
+						Path(dirs.DATA, r'poxy-icon-theme.svg'),
+						logger=context.verbose_logger,
+						root_id=r'poxy-theme-switch-img'
+					)
+					bar[i] = (
+						r'<a title="Toggle dark and light themes" '
+						+ r'id="poxy-theme-switch" href="javascript:void(null);" role="button" '
+						+ rf'class="poxy-icon theme" onClick="toggle_theme(); return false;">{svg}</a>', []
+					)
+			bar = [b for b in bar if b is not None]
+			# automatically overflow onto the second row
+			split = min(max(int(len(bar) / 2) + len(bar) % 2, 2), len(bar))
+			for b, i in ((bar[:split], 0), (bar[split:], 1)):
+				for j in range(len(b)):
+					if isinstance(b[j], tuple):
+						navbar[i].append(b[j])
+					else:
+						navbar[i].append((None, b[j], []))
+		for i in (0, 1):
+			if navbar[i]:
+				conf(f'LINKS_NAVBAR{i+1} = [\n\t', end='')
+				conf(',\n\t'.join([rf'{b}' for b in navbar[i]]))
+				conf(r']')
+			else:
+				conf(rf'LINKS_NAVBAR{i+1} = []')
+
+		# footer
+		conf(r"FINE_PRINT = r'''")
+		footer = []
+		if context.repo:
+			footer.append(rf'<a href="{context.repo.uri}" target="_blank">{type(context.repo).__name__}</a>')
+			footer.append(rf'<a href="{context.repo.issues_uri}" target="_blank">Report an issue</a>')
+		if context.changelog:
+			footer.append(rf'<a href="md_poxy_changelog.html">Changelog</a>')
+		if context.license and context.license[r'uri']:
+			footer.append(rf'<a href="{context.license["uri"]}" target="_blank">License</a>')
+		if context.generate_tagfile:
+			footer.append(
+				rf'<a href="{context.tagfile_path.name}" target="_blank" type="text/xml" download>Doxygen tagfile</a>'
+			)
+		if footer:
+			for i in range(1, len(footer)):
+				footer[i] = r' &bull; ' + footer[i]
+			footer.append(r'<br><br>')
+		footer.append(r'Site generated using <a href="https://github.com/marzer/poxy/">Poxy</a>')
+		for i in range(len(footer)):
+			conf(rf"    {footer[i]}")
+		conf(r"'''")
+
+		conf_py_text = conf_py.getvalue()
+		context.verbose(r'm.css conf.py:')
+		context.verbose(conf_py_text, indent=r'   ')
+
+		# write conf.py
+		context.verbose(rf'Writing {context.mcss_conf_path}')
+		with open(context.mcss_conf_path, r'w', encoding=r'utf-8', newline='\n') as f:
+			f.write(conf_py_text)
+
 
 
 _worker_context = None
 
 
 
 def _initialize_worker(context):
 	global _worker_context
 	_worker_context = context
 
 
 
-def postprocess_html_file(path, context=None):
+def postprocess_html_file(path, context: Context = None):
 	assert path is not None
 	assert isinstance(path, Path)
 	assert path.is_absolute()
 	assert path.exists()
 
 	if context is None:
 		global _worker_context
 		context = _worker_context
 	assert context is not None
-	assert isinstance(context, project.Context)
+	assert isinstance(context, Context)
 
 	context.info(rf'Post-processing {path}')
-	changed = False
+	text = None
+	html = None
+
+	def switch_to_html():
+		nonlocal context
+		nonlocal text
+		nonlocal html
+		if html is not None:
+			return
+		html = soup.HTMLDocument(text, logger=context.verbose_logger)
+
+	def switch_to_text():
+		nonlocal context
+		nonlocal text
+		nonlocal html
+		if html is None:
+			return
+		html.smooth()
+		text = str(html)
+		html = None
+
 	try:
+		text = read_all_text_from_file(path, logger=context.verbose_logger)
+		changed = False
+
 		for fix in context.fixers:
 			if isinstance(fix, fixers.HTMLFixer):
-				doc = soup.HTMLDocument(path, logger=context.verbose_logger)
-				if fix(doc, context):
-					doc.smooth()
-					doc.flush()
+				switch_to_html()
+				if fix(context, html, path):
 					changed = True
+					html.smooth()
 			elif isinstance(fix, fixers.PlainTextFixer):
-				doc = [read_all_text_from_file(path, logger=context.verbose_logger), path]
-				if fix(doc, context):
-					context.verbose(rf'Writing {path}')
-					with open(path, 'w', encoding='utf-8', newline='\n') as f:
-						f.write(doc[0])
-					changed = True
+				switch_to_text()
+				prev_text = text
+				text = fix(context, prev_text, path)
+				changed = changed or prev_text != text
+
+		if changed:
+			switch_to_text()
+			context.verbose(rf'Writing {path}')
+			with open(path, 'w', encoding='utf-8', newline='\n') as f:
+				f.write(text)
 
 	except Exception as e:
 		context.info(rf'{type(e).__name__} raised while post-processing {path}')
 		raise
 	except:
 		context.info(rf'Error occurred while post-processing {path}')
 		raise
 
-	return changed
 
 
-
-def postprocess_html(context):
+def postprocess_html(context: Context):
 	assert context is not None
-	assert isinstance(context, project.Context)
+	assert isinstance(context, Context)
 
 	files = filter_filenames(
 		get_all_files(context.html_dir, any=('*.html', '*.htm')), context.html_include, context.html_exclude
 	)
 	if not files:
 		return
 
-	threads = min(len(files), context.threads, 8)  # diminishing returns after 8
+	context.fixers = (
+		fixers.MarkTOC(),
+		fixers.CodeBlocks(),
+		fixers.Banner(),
+		fixers.CPPModifiers1(),
+		fixers.CPPModifiers2(),
+		fixers.CPPTemplateTemplate(),
+		fixers.StripIncludes(),
+		fixers.AutoDocLinks(),
+		fixers.Links(),
+		fixers.CustomTags(),
+		fixers.EmptyTags(),
+		fixers.ImplementationDetails(),
+		fixers.MarkdownPages(),
+		fixers.InjectSVGs(),
+	)
 
-	with ScopeTimer(rf'Post-processing {len(files)} HTML files', print_start=True, print_end=context.verbose_logger):
-		context.fixers = (
-			fixers.MarkTOC(),
-			fixers.CodeBlocks(),
-			fixers.Banner(),
-			fixers.CPPModifiers1(),
-			fixers.CPPModifiers2(),
-			fixers.CPPTemplateTemplate(),
-			fixers.StripIncludes(),
-			fixers.AutoDocLinks(),
-			fixers.Links(),
-			fixers.CustomTags(),
-			fixers.EmptyTags(),
-			fixers.ImplementationDetails(),
-			fixers.MarkdownPages(),
-			fixers.InjectSVGs(),
-		)
-		context.verbose(rf'Post-processing {len(files)} HTML files...')
-		if threads > 1:
-			with futures.ProcessPoolExecutor(
-				max_workers=threads, initializer=_initialize_worker, initargs=(context, )
-			) as executor:
-				jobs = [executor.submit(postprocess_html_file, file) for file in files]
-				for future in futures.as_completed(jobs):
+	threads = min(len(files), context.threads, 16)
+	context.info(rf'Post-processing {len(files)} HTML files on {threads} thread{"s" if threads > 1 else ""}...')
+	if threads > 1:
+		with futures.ProcessPoolExecutor(
+			max_workers=threads, initializer=_initialize_worker, initargs=(context, )
+		) as executor:
+			jobs = [executor.submit(postprocess_html_file, file) for file in files]
+			for future in futures.as_completed(jobs):
+				try:
+					future.result()
+				except:
 					try:
-						future.result()
-					except:
-						try:
-							executor.shutdown(wait=False, cancel_futures=True)
-						except TypeError:
-							executor.shutdown(wait=False)
-						raise
-
-		else:
-			for file in files:
-				postprocess_html_file(file, context)
+						executor.shutdown(wait=False, cancel_futures=True)
+					except TypeError:
+						executor.shutdown(wait=False)
+					raise
+
+	else:
+		for file in files:
+			postprocess_html_file(file, context)
 
 
 
 #=======================================================================================================================
 # RUN
 #=======================================================================================================================
 
@@ -1165,179 +1268,127 @@
 					else:
 						warnings.append(text)
 					break
 	return warnings
 
 
 
+def run_doxygen(context: Context):
+	assert context is not None
+	assert isinstance(context, Context)
+	with make_temp_file() as stdout, make_temp_file() as stderr:
+		try:
+			subprocess.run([str(context.doxygen_path), str(context.doxyfile_path)],
+				check=True,
+				stdout=stdout,
+				stderr=stderr,
+				cwd=context.input_dir)
+		except:
+			context.info(r'Doxygen failed!')
+			dump_output_streams(context, read_output_streams(stdout, stderr), source=r'Doxygen')
+			raise
+		if context.is_verbose() or context.warnings.enabled:
+			outputs = read_output_streams(stdout, stderr)
+			if context.is_verbose():
+				dump_output_streams(context, outputs, source=r'Doxygen')
+			if context.warnings.enabled:
+				warnings = extract_warnings(outputs)
+				for w in warnings:
+					context.warning(w)
+
+	# remove the local paths from the tagfile since they're meaningless (and a privacy breach)
+	if context.tagfile_path:
+		text = read_all_text_from_file(context.tagfile_path, logger=context.verbose_logger)
+		text = re.sub(r'\n\s*?<path>.+?</path>\s*?\n', '\n', text, re.S)
+		context.verbose(rf'Writing {context.tagfile_path}')
+		with open(context.tagfile_path, 'w', encoding='utf-8', newline='\n') as f:
+			f.write(text)
+
+
+
+def run_mcss(context: Context):
+	assert context is not None
+	assert isinstance(context, Context)
+	with make_temp_file() as stdout, make_temp_file() as stderr:
+		doxy_args = [str(context.mcss_conf_path), r'--no-doxygen', r'--sort-globbed-files']
+		if context.is_verbose():
+			doxy_args.append(r'--debug')
+		try:
+			run_python_script(
+				Path(dirs.MCSS, r'documentation/doxygen.py'),
+				*doxy_args,
+				stdout=stdout,
+				stderr=stderr,
+				cwd=context.input_dir
+			)
+		except:
+			context.info(r'm.css failed!')
+			dump_output_streams(context, read_output_streams(stdout, stderr), source=r'm.css')
+			raise
+		if context.is_verbose() or context.warnings.enabled:
+			outputs = read_output_streams(stdout, stderr)
+			if context.is_verbose():
+				dump_output_streams(context, outputs, source=r'm.css')
+			if context.warnings.enabled:
+				warnings = extract_warnings(outputs)
+				for w in warnings:
+					context.warning(w)
+
+
+
 def run(
 	config_path=None,
 	output_dir='.',
 	threads=-1,
 	cleanup=True,
 	verbose=False,
 	doxygen_path=None,
 	logger=None,
-	dry_run=False,
 	xml_only=False,
 	html_include=None,
 	html_exclude=None,
 	treat_warnings_as_errors=None,
 	theme=None,
 	copy_assets=True
 ):
 
-	with project.Context(
+	timer = lambda desc: ScopeTimer(desc, print_start=True, print_end=context.verbose_logger)
+
+	with Context(
 		config_path=config_path,
 		output_dir=output_dir,
 		threads=threads,
 		cleanup=cleanup,
 		verbose=verbose,
 		doxygen_path=doxygen_path,
 		logger=logger,
-		dry_run=dry_run,
 		xml_only=xml_only,
 		html_include=html_include,
 		html_exclude=html_exclude,
 		treat_warnings_as_errors=treat_warnings_as_errors,
 		theme=theme,
 		copy_assets=copy_assets
 	) as context:
 
-		# preprocess the doxyfile
 		preprocess_doxyfile(context)
-		context.verbose_object(r'Context.warnings', context.warnings)
-
-		if context.dry_run:
-			return
-
-		# resolve any uri tagfiles
-		if context.unresolved_tagfiles:
-			with ScopeTimer(r'Resolving remote tagfiles', print_start=True, print_end=context.verbose_logger) as t:
-				for source, (file, _) in context.tagfiles.items():
-					if file.exists() or not is_uri(source):
-						continue
-					context.verbose(rf'Downloading {source} => {file}')
-					response = requests.get(source, allow_redirects=True, stream=False, timeout=30)
-					context.verbose(rf'Writing {file}')
-					with open(file, 'w', encoding='utf-8', newline='\n') as f:
-						f.write(response.text)
-
-		make_temp_file = lambda: tempfile.SpooledTemporaryFile(mode='w+', newline='\n', encoding='utf-8')
-
-		# precondition the change log page (at this point it is already a temp copy)
-		if context.changelog:
-			text = read_all_text_from_file(context.changelog, logger=context.verbose_logger).strip()
-			text = text.replace('\r\n', '\n')
-			text = re.sub(r'\n<br[ \t]*/?><br[ \t]*/?>\n', r'', text)
-			if context.repo:
-				text = re.sub(r'#([0-9]+)', lambda m: rf'[#{m[1]}]({context.repo.make_issue_uri(m[1])})', text)
-				text = re.sub(r'!([0-9]+)', lambda m: rf'[!{m[1]}]({context.repo.make_pull_request_uri(m[1])})', text)
-				text = re.sub(r'@([a-zA-Z0-9_-]+)', lambda m: rf'[@{m[1]}]({context.repo.make_user_uri(m[1])})', text)
-			text = text.replace(r'&amp;', r'__poxy_thiswasan_amp')
-			text = text.replace(r'&#xFE0F;', r'__poxy_thiswasan_fe0f')
-			text = text.replace(r'@', r'__poxy_thiswasan_at')
-			if text.find(r'@tableofcontents') == -1 and text.find('\\tableofcontents'
-																	) == -1 and text.find(r'[TOC]') == -1:
-				#text = f'[TOC]\n\n{text}'
-				nlnl = text.find(r'\n\n')
-				if nlnl != -1:
-					text = f'{text[:nlnl]}\n\n\\tableofcontents\n\n{text[nlnl:]}'
-				pass
-			text += '\n\n'
-			with open(context.changelog, r'w', encoding=r'utf-8', newline='\n') as f:
-				f.write(text)
-
-		# run doxygen to generate the xml
-		if 1:
-			with ScopeTimer(
-				r'Generating XML files with Doxygen', print_start=True, print_end=context.verbose_logger
-			) as t:
-				with make_temp_file() as stdout, make_temp_file() as stderr:
-					try:
-						subprocess.run([str(context.doxygen_path),
-							str(context.doxyfile_path)],
-							check=True,
-							stdout=stdout,
-							stderr=stderr,
-							cwd=context.input_dir)
-					except:
-						context.info(r'Doxygen failed!')
-						dump_output_streams(context, read_output_streams(stdout, stderr), source=r'Doxygen')
-						raise
-					if context.is_verbose() or context.warnings.enabled:
-						outputs = read_output_streams(stdout, stderr)
-						if context.is_verbose():
-							dump_output_streams(context, outputs, source=r'Doxygen')
-						if context.warnings.enabled:
-							warnings = extract_warnings(outputs)
-							for w in warnings:
-								context.warning(w)
-
-				# remove the local paths from the tagfile since they're meaningless (and a privacy breach)
-				if context.tagfile_path is not None and context.tagfile_path.exists():
-					text = read_all_text_from_file(context.tagfile_path, logger=context.verbose_logger)
-					text = re.sub(r'\n\s*?<path>.+?</path>\s*?\n', '\n', text, re.S)
-					context.verbose(rf'Writing {context.tagfile_path}')
-					with open(context.tagfile_path, 'w', encoding='utf-8', newline='\n') as f:
-						f.write(text)
+		preprocess_tagfiles(context)
+		preprocess_changelog(context)
 
-		# post-process xml files
-		if 1:
+		# generate + postprocess XML
+		with timer(r'Generating XML files with Doxygen') as t:
+			run_doxygen(context)
+		with timer(r'Post-processing XML files') as t:
 			postprocess_xml(context)
-
 		if context.xml_only:
 			return
 
-		context.verbose_object(r'Context.code_blocks', context.code_blocks)
-
-		# compile regexes
-		# (done here because doxygen and xml preprocessing adds additional values to these lists)
-		context.code_blocks.namespaces = regex_or(
-			context.code_blocks.namespaces, pattern_prefix='(?:::)?', pattern_suffix='(?:::)?'
-		)
-		context.code_blocks.types = regex_or(
-			context.code_blocks.types, pattern_prefix='(?:::)?', pattern_suffix='(?:::)?'
-		)
-		context.code_blocks.enums = regex_or(context.code_blocks.enums, pattern_prefix='(?:::)?')
-		context.code_blocks.string_literals = regex_or(context.code_blocks.string_literals)
-		context.code_blocks.numeric_literals = regex_or(context.code_blocks.numeric_literals)
-		context.code_blocks.macros = regex_or(context.code_blocks.macros)
-		context.autolinks = tuple([(re.compile('(?<![a-zA-Z_])' + expr + '(?![a-zA-Z_])'), uri)
-			for expr, uri in context.autolinks])
-
-		# run m.css to generate the html
-		if 1:
-			with ScopeTimer(
-				r'Generating HTML files with m.css', print_start=True, print_end=context.verbose_logger
-			) as t:
-				with make_temp_file() as stdout, make_temp_file() as stderr:
-					doxy_args = [str(context.mcss_conf_path), r'--no-doxygen', r'--sort-globbed-files']
-					if context.is_verbose():
-						doxy_args.append(r'--debug')
-					try:
-						run_python_script(
-							Path(dirs.MCSS, r'documentation/doxygen.py'),
-							*doxy_args,
-							stdout=stdout,
-							stderr=stderr,
-							cwd=context.input_dir
-						)
-					except:
-						context.info(r'm.css failed!')
-						dump_output_streams(context, read_output_streams(stdout, stderr), source=r'm.css')
-						raise
-					if context.is_verbose() or context.warnings.enabled:
-						outputs = read_output_streams(stdout, stderr)
-						if context.is_verbose():
-							dump_output_streams(context, outputs, source=r'm.css')
-						if context.warnings.enabled:
-							warnings = extract_warnings(outputs)
-							for w in warnings:
-								context.warning(w)
+		# generate HTML with mcss
+		preprocess_mcss_config(context)
+		with timer(r'Generating HTML files with m.css') as t:
+			run_mcss(context)
 
 		# copy extra_files
 		with ScopeTimer(r'Copying extra_files', print_start=True, print_end=context.verbose_logger) as t:
 			for dest_name, source_path in context.extra_files.items():
 				dest_path = Path(context.html_dir, dest_name).resolve()
 				dest_path.parent.mkdir(exist_ok=True)
 				copy_file(source_path, dest_path, logger=context.verbose_logger)
@@ -1351,9 +1402,9 @@
 		if context.generate_tagfile:
 			if context.tagfile_path.exists():
 				move_file(context.tagfile_path, Path(context.output_dir, r'html'), logger=context.verbose_logger)
 			else:
 				context.warning(rf'Doxygen tagfile {context.tagfile_path} not found!')
 
 		# post-process html files
-		if 1:
+		with timer(r'Post-processing HTML files') as t:
 			postprocess_html(context)
```

### Comparing `poxy-0.9.0/poxy/soup.py` & `poxy-0.9.1/poxy/soup.py`

 * *Files 5% similar despite different names*

```diff
@@ -127,27 +127,41 @@
 
 def set_class(tag, classes):
 	tag['class'] = []
 	add_class(tag, classes)
 
 
 
+def get_classes(tag):
+	if 'class' not in tag.attrs:
+		return []
+	classes = tag['class']
+	if not is_collection(classes):
+		classes = [classes]
+	return [str(c) for c in classes]
+
+
+
 #=======================================================================================================================
 # HTML DOCUMENT
 #=======================================================================================================================
 
 
 
 class HTMLDocument(object):
 
-	def __init__(self, path, logger):
+	def __init__(self, source: Union[str, Path], logger):
 		self.__logger = logger
-		self.path = path
-		with open(self.path, 'r', encoding='utf-8') as f:
-			self.__doc = bs4.BeautifulSoup(f, 'html5lib', from_encoding='utf-8')
+
+		assert source is not None
+		if isinstance(source, Path):
+			with open(str(source), 'r', encoding='utf-8') as f:
+				self.__doc = bs4.BeautifulSoup(f, 'html5lib', from_encoding='utf-8')
+		else:
+			self.__doc = bs4.BeautifulSoup(source, 'html5lib')
 
 		self.html = self.__doc.html
 		self.head = self.__doc.head
 		self.body = self.__doc.body
 
 		self.article = None
 		self.article_content = None
@@ -168,26 +182,21 @@
 				if self.table_of_contents is not None:
 					break
 			self.sections = self.article_content('section', recursive=False)
 
 	def smooth(self):
 		self.__doc.smooth()
 
-	def flush(self):
-		log(self.__logger, rf'Writing {self.path}')
+	def write(self, path):
+		log(self.__logger, rf'Writing {path}')
 		with open(self.path, 'w', encoding='utf-8', newline='\n') as f:
 			f.write(str(self.__doc))
 
-	def __enter__(self):
-		return self
-
-	def __exit__(self, type, value, traceback):
-		if traceback is None:
-			self.smooth()
-			self.flush()
+	def __str__(self) -> str:
+		return str(self.__doc)
 
 	def new_tag(self, tag_name, parent=None, string=None, class_=None, index=None, before=None, after=None, **kwargs):
 		tag = self.__doc.new_tag(tag_name, **kwargs)
 		if (string is not None):
 			if (tag.string is not None):
 				tag.string.replace_with(string)
 			else:
```

### Comparing `poxy-0.9.0/poxy/svg.py` & `poxy-0.9.1/poxy/svg.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 # SPDX-License-Identifier: MIT
 """
 Functions and classes for working with SVG files.
 """
 
 from lxml import etree
 from .utils import *
-from typing import Union
-from io import StringIO
+from typing import Union, Sequence
 
 
 
 class SVG(object):
 	pass
 
 	def __init__(
 		self,  #
 		file_path: Union[Path, str],
 		logger=None,
 		root_id: str = None,
-		id_namespace: str = None
+		id_namespace: str = None,
+		root_classes: Union[str, Sequence[str]] = None
 	):
 
 		# read file
 		svg = read_all_text_from_file(file_path, logger=logger)
 
 		# add a namespace prefix to the #ids if requested
 		# (so they're unique when injected into HTML etc)
@@ -45,23 +45,35 @@
 		parser = etree.XMLParser(
 			remove_blank_text=True,  #
 			recover=True,
 			remove_comments=True,
 			ns_clean=True,
 			encoding=r'utf-8'
 		)
-		self.__xml = etree.parse(StringIO(svg), parser=parser)
-		root = self.__xml.getroot()
-		attrs = root.attrib
+		self.__xml = etree.fromstring(svg.encode(r'utf-8'), parser=parser)
+		attrs = self.__xml.attrib
 
 		# set/normalize various attributes
 		if r'xmlns' not in attrs:
 			attrs[r'xmlns'] = r'http://www.w3.org/2000/svg'
 		# if r'xmlns:xlink' not in attrs:
 		#	attrs[r'xmlns:xlink'] = r'http://www.w3.org/1999/xlink')
 		if r'version' not in attrs:
 			attrs[r'version'] = r'1.1'
 		if root_id:
 			attrs[r'id'] = root_id
 
+		# some editors use the root attribute to store a bunch of metadata
+		# and tracking garbage so delete it
+		if r'content' in attrs:
+			del attrs[r'content']
+
+		# set class attribute if specified
+		if root_classes is not None:
+			root_classes = list(coerce_collection(root_classes))
+			if root_classes:
+				attrs[r'class'] = r' '.join(list(coerce_collection(root_classes)))
+			elif r'class' in attrs:
+				del attrs[r'class']
+
 	def __str__(self) -> str:
-		return etree.tostring(self.__xml.getroot(), encoding=r'unicode', xml_declaration=False, pretty_print=True)
+		return etree.tostring(self.__xml, encoding=r'unicode', xml_declaration=False, pretty_print=False)
```

### Comparing `poxy-0.9.0/poxy/utils.py` & `poxy-0.9.1/poxy/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -88,25 +88,25 @@
 DOWNLOAD_HEADERS = {r'User-Agent': r'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:104.0) Gecko/20100101 Firefox/104.0'}
 
 
 
 def download_text(uri: str, timeout=10, encoding='utf-8') -> str:
 	assert uri is not None
 	global DOWNLOAD_HEADERS
-	response = requests.get(str(uri), headers=DOWNLOAD_HEADERS, timeout=timeout)
+	response = requests.get(str(uri), headers=DOWNLOAD_HEADERS, timeout=timeout, stream=False, allow_redirects=True)
 	if encoding is not None:
 		response.encoding = encoding
 	return response.text
 
 
 
 def download_binary(uri: str, timeout=10) -> bytes:
 	assert uri is not None
 	global DOWNLOAD_HEADERS
-	response = requests.get(str(uri), headers=DOWNLOAD_HEADERS, timeout=timeout)
+	response = requests.get(str(uri), headers=DOWNLOAD_HEADERS, timeout=timeout, stream=False, allow_redirects=True)
 	return response.content
 
 
 
 #=======================================================================================================================
 # REGEX REPLACER
 #=======================================================================================================================
```

### Comparing `poxy-0.9.0/poxy.egg-info/PKG-INFO` & `poxy-0.9.1/poxy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poxy
-Version: 0.9.0
+Version: 0.9.1
 Summary: Documentation generator for C++.
 Home-page: https://github.com/marzer/poxy
 Download-URL: https://pypi.org/project/poxy/
 Author: Mark Gillard
 Author-email: mark.gillard@outlook.com.au
 License: MIT
 Project-URL: Source, https://github.com/marzer/poxy
@@ -84,47 +84,43 @@
 <br><br>
 
 ## Usage
 
 Poxy is a command-line application.
 
 ```
-poxy [-h] [-v] [--doxygen <path>] [--dry] [--threads N] [--version] [--werror] [--xmlonly]
-            [--ppinclude <regex>] [--ppexclude <regex>] [--theme {auto,light,dark,custom}]
-            [config]
+poxy [-h] [-v] [--doxygen <path>] [--ppinclude <regex>] [--ppexclude <regex>]
+     [--theme {auto,light,dark,custom}] [--threads N] [--version] [--werror] [--xmlonly]
+     [config]
 
 Generate fancy C++ documentation.
 
 positional arguments:
   config                path to poxy.toml or a directory containing it (default: .)
 
 options:
   -h, --help            show this help message and exit
   -v, --verbose         enable very noisy diagnostic output
   --doxygen <path>      specify the Doxygen executable to use (default: find on system path)
-  --dry                 do a 'dry run' only, stopping after emitting the effective Doxyfile
-  --threads N           set the number of threads to use (default: automatic)
-  --version             print the version and exit
-  --werror              always treat warnings as errors regardless of config file settings
-  --xmlonly             stop after generating and preprocessing the Doxygen xml
   --ppinclude <regex>   pattern matching HTML file names to post-process (default: all)
   --ppexclude <regex>   pattern matching HTML file names to exclude from post-processing (default: none)
   --theme {auto,light,dark,custom}
                         the CSS theme to use (default: auto)
+  --threads N           set the number of threads to use (default: automatic)
+  --version             print the version and exit
+  --werror              always treat warnings as errors regardless of config file settings
+  --xmlonly             stop after generating and preprocessing the Doxygen xml
 ```
 
 The basic three-step to using Poxy is similar to Doxygen:
 
 1. Create your `poxy.toml` (Poxy's answer to the `Doxyfile`)
 2. Invoke Poxy on it: `poxy path/to/poxy.toml` (or simply `poxy` if the cwd contains the config file)
 3. See your HTML documentation `<cwd>/html`
 
-ℹ&#xFE0F; If there exists a `Doxyfile` or `Doxyfile-mcss` in the same directory as your `poxy.toml` it will be loaded
-first, then the Poxy overrides applied on top of it. Otherwise a 'default' Doxyfile is used as the base.
-
 <br><br>
 
 ## Config file options
 
 For a self-contained `poxy.toml` example to copy and paste from, see [the one used by toml++](https://github.com/marzer/tomlplusplus/blob/master/docs/poxy.toml).
 
 For a full list of options, with full descriptions, schemas and usage examples, see the [Configuration options] wiki page.
@@ -184,14 +180,26 @@
 [c++ feature test macros]: https://en.cppreference.com/w/cpp/feature_test
 [configuration options]: https://github.com/marzer/poxy/wiki/Configuration-options
 [feature request]: https://github.com/marzer/poxy/issues/new
 [`currentcolor`]: https://gomakethings.com/currentcolor-and-svgs
 
 # Changelog
 
+## v0.9.1 - 2022-10-04
+
+-   fixed SVG inlining not preserving original image class attributes
+-   fixed `ValueError` when reading some SVG files
+-   fixed `navbar` option allowing duplicates
+-   fixed custom navbar items always being transformed to lowercase
+-   fixed navbar generating links to empty pages
+-   added `concepts` to the default set of links in `navbar`
+-   added `navbar` values `all` and `default`
+-   reduced I/O churn during HTML post-processing
+-   removed command-line option `dry`
+
 ## v0.9.0 - 2022-10-03
 
 -   added support for C++20 concepts
 
 ## v0.8.2 - 2022-10-01
 
 -   added post-process to inline all local SVGs
```

### Comparing `poxy-0.9.0/poxy.egg-info/SOURCES.txt` & `poxy-0.9.1/poxy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `poxy-0.9.0/setup.py` & `poxy-0.9.1/setup.py`

 * *Files identical despite different names*

