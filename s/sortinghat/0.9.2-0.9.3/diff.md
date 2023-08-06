# Comparing `tmp/sortinghat-0.9.2.tar.gz` & `tmp/sortinghat-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sortinghat-0.9.2.tar", max compression
+gzip compressed data, was "sortinghat-0.9.3.tar", max compression
```

## Comparing `sortinghat-0.9.2.tar` & `sortinghat-0.9.3.tar`

### file list

```diff
@@ -1,180 +1,180 @@
--rw-r--r--   0        0        0      363 2023-04-27 08:59:41.311368 sortinghat-0.9.2/AUTHORS
--rw-r--r--   0        0        0    35147 2023-04-27 08:59:41.311368 sortinghat-0.9.2/LICENSE
--rw-r--r--   0        0        0    14737 2023-04-27 08:59:41.311368 sortinghat-0.9.2/NEWS
--rw-r--r--   0        0        0     8566 2023-04-27 08:59:41.311368 sortinghat-0.9.2/README.md
--rw-r--r--   0        0        0     2049 2023-04-27 08:59:41.315369 sortinghat-0.9.2/pyproject.toml
--rw-r--r--   0        0        0       86 2023-04-27 08:59:41.315369 sortinghat-0.9.2/sortinghat/_version.py
--rw-r--r--   0        0        0        0 2023-04-27 08:59:41.315369 sortinghat-0.9.2/sortinghat/app/__init__.py
--rw-r--r--   0        0        0     1250 2023-04-27 08:59:41.315369 sortinghat-0.9.2/sortinghat/app/schema.py
--rw-r--r--   0        0        0      518 2023-04-27 08:59:41.315369 sortinghat-0.9.2/sortinghat/app/urls.py
--rw-r--r--   0        0        0      196 2023-04-27 08:59:41.315369 sortinghat-0.9.2/sortinghat/app/wsgi.py
--rw-r--r--   0        0        0        0 2023-04-27 08:59:41.315369 sortinghat-0.9.2/sortinghat/cli/__init__.py
--rw-r--r--   0        0        0      977 2023-04-27 08:59:41.315369 sortinghat-0.9.2/sortinghat/cli/client/__init__.py
--rw-r--r--   0        0        0     5738 2023-04-27 08:59:41.315369 sortinghat-0.9.2/sortinghat/cli/client/client.py
--rw-r--r--   0        0        0    43408 2023-04-27 08:59:41.315369 sortinghat-0.9.2/sortinghat/cli/client/schema.py
--rw-r--r--   0        0        0        0 2023-04-27 08:59:41.315369 sortinghat-0.9.2/sortinghat/cli/cmds/__init__.py
--rw-r--r--   0        0        0     3072 2023-04-27 08:59:41.315369 sortinghat-0.9.2/sortinghat/cli/cmds/add.py
--rw-r--r--   0        0        0     6145 2023-04-27 08:59:41.315369 sortinghat-0.9.2/sortinghat/cli/cmds/config.py
--rw-r--r--   0        0        0     3219 2023-04-27 08:59:41.315369 sortinghat-0.9.2/sortinghat/cli/cmds/countries.py
--rw-r--r--   0        0        0     3462 2023-04-27 08:59:41.315369 sortinghat-0.9.2/sortinghat/cli/cmds/enroll.py
--rw-r--r--   0        0        0     2860 2023-04-27 08:59:41.315369 sortinghat-0.9.2/sortinghat/cli/cmds/lock.py
--rw-r--r--   0        0        0     2342 2023-04-27 08:59:41.315369 sortinghat-0.9.2/sortinghat/cli/cmds/merge.py
--rw-r--r--   0        0        0     2352 2023-04-27 08:59:41.315369 sortinghat-0.9.2/sortinghat/cli/cmds/mv.py
--rw-r--r--   0        0        0     7466 2023-04-27 08:59:41.315369 sortinghat-0.9.2/sortinghat/cli/cmds/orgs.py
--rw-r--r--   0        0        0     2934 2023-04-27 08:59:41.315369 sortinghat-0.9.2/sortinghat/cli/cmds/profile.py
--rw-r--r--   0        0        0     1992 2023-04-27 08:59:41.315369 sortinghat-0.9.2/sortinghat/cli/cmds/rm.py
--rw-r--r--   0        0        0     2909 2023-04-27 08:59:41.315369 sortinghat-0.9.2/sortinghat/cli/cmds/show.py
--rw-r--r--   0        0        0     2365 2023-04-27 08:59:41.315369 sortinghat-0.9.2/sortinghat/cli/cmds/split.py
--rw-r--r--   0        0        0     3364 2023-04-27 08:59:41.315369 sortinghat-0.9.2/sortinghat/cli/cmds/withdraw.py
--rwxr-xr-x   0        0        0     2857 2023-04-27 08:59:41.315369 sortinghat-0.9.2/sortinghat/cli/sortinghat.py
--rw-r--r--   0        0        0       43 2023-04-27 08:59:41.315369 sortinghat-0.9.2/sortinghat/cli/templates/add.tmpl
--rw-r--r--   0        0        0       23 2023-04-27 08:59:41.315369 sortinghat-0.9.2/sortinghat/cli/templates/config.tmpl
--rw-r--r--   0        0        0       83 2023-04-27 08:59:41.315369 sortinghat-0.9.2/sortinghat/cli/templates/countries.tmpl
--rw-r--r--   0        0        0       54 2023-04-27 08:59:41.315369 sortinghat-0.9.2/sortinghat/cli/templates/lock.tmpl
--rw-r--r--   0        0        0      169 2023-04-27 08:59:41.315369 sortinghat-0.9.2/sortinghat/cli/templates/mv.tmpl
--rw-r--r--   0        0        0      208 2023-04-27 08:59:41.315369 sortinghat-0.9.2/sortinghat/cli/templates/organizations.tmpl
--rw-r--r--   0        0        0      375 2023-04-27 08:59:41.315369 sortinghat-0.9.2/sortinghat/cli/templates/profile.tmpl
--rw-r--r--   0        0        0      106 2023-04-27 08:59:41.315369 sortinghat-0.9.2/sortinghat/cli/templates/rm.tmpl
--rw-r--r--   0        0        0     1016 2023-04-27 08:59:41.315369 sortinghat-0.9.2/sortinghat/cli/templates/show.tmpl
--rw-r--r--   0        0        0       69 2023-04-27 08:59:41.315369 sortinghat-0.9.2/sortinghat/cli/templates/split.tmpl
--rw-r--r--   0        0        0     4856 2023-04-27 08:59:41.315369 sortinghat-0.9.2/sortinghat/cli/utils.py
--rw-r--r--   0        0        0        0 2023-04-27 08:59:41.315369 sortinghat-0.9.2/sortinghat/config/__init__.py
--rw-r--r--   0        0        0     9252 2023-04-27 08:59:41.315369 sortinghat-0.9.2/sortinghat/config/settings.py
--rw-r--r--   0        0        0       20 2023-04-27 08:59:41.315369 sortinghat-0.9.2/sortinghat/config/tenants.json
--rw-r--r--   0        0        0     1544 2023-04-27 08:59:41.315369 sortinghat-0.9.2/sortinghat/core/admin.py
--rw-r--r--   0        0        0    50534 2023-04-27 08:59:41.315369 sortinghat-0.9.2/sortinghat/core/api.py
--rw-r--r--   0        0        0      926 2023-04-27 08:59:41.315369 sortinghat-0.9.2/sortinghat/core/apps.py
--rw-r--r--   0        0        0     5169 2023-04-27 08:59:41.315369 sortinghat-0.9.2/sortinghat/core/aux.py
--rw-r--r--   0        0        0      997 2023-04-27 08:59:41.315369 sortinghat-0.9.2/sortinghat/core/context.py
--rw-r--r--   0        0        0    37055 2023-04-27 08:59:41.315369 sortinghat-0.9.2/sortinghat/core/db.py
--rw-r--r--   0        0        0     3019 2023-04-27 08:59:41.315369 sortinghat-0.9.2/sortinghat/core/decorators.py
--rw-r--r--   0        0        0     3875 2023-04-27 08:59:41.315369 sortinghat-0.9.2/sortinghat/core/errors.py
--rw-r--r--   0        0        0    41236 2023-04-27 08:59:41.315369 sortinghat-0.9.2/sortinghat/core/fixtures/countries.json
--rw-r--r--   0        0        0     7820 2023-04-27 08:59:41.315369 sortinghat-0.9.2/sortinghat/core/importer/backend.py
--rw-r--r--   0        0        0     7136 2023-04-27 08:59:41.315369 sortinghat-0.9.2/sortinghat/core/importer/backends/mailmap.py
--rw-r--r--   0        0        0     5817 2023-04-27 08:59:41.315369 sortinghat-0.9.2/sortinghat/core/importer/base.py
--rw-r--r--   0        0        0     2143 2023-04-27 08:59:41.315369 sortinghat-0.9.2/sortinghat/core/importer/models.py
--rw-r--r--   0        0        0     2059 2023-04-27 08:59:41.315369 sortinghat-0.9.2/sortinghat/core/importer/utils.py
--rw-r--r--   0        0        0    25814 2023-04-27 08:59:41.315369 sortinghat-0.9.2/sortinghat/core/jobs.py
--rw-r--r--   0        0        0     7298 2023-04-27 08:59:41.315369 sortinghat-0.9.2/sortinghat/core/log.py
--rw-r--r--   0        0        0        0 2023-04-27 08:59:41.315369 sortinghat-0.9.2/sortinghat/core/management/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 08:59:41.315369 sortinghat-0.9.2/sortinghat/core/management/commands/__init__.py
--rw-r--r--   0        0        0     4155 2023-04-27 08:59:41.319369 sortinghat-0.9.2/sortinghat/core/management/commands/create_groups.py
--rw-r--r--   0        0        0     4354 2023-04-27 08:59:41.319369 sortinghat-0.9.2/sortinghat/core/middleware.py
--rw-r--r--   0        0        0    14035 2023-04-27 08:59:41.319369 sortinghat-0.9.2/sortinghat/core/migrations/0001_sortinghat.py
--rw-r--r--   0        0        0     1717 2023-04-27 08:59:41.319369 sortinghat-0.9.2/sortinghat/core/migrations/0002_importidentitiestask.py
--rw-r--r--   0        0        0     1502 2023-04-27 08:59:41.319369 sortinghat-0.9.2/sortinghat/core/migrations/0003_multi_tenancy.py
--rw-r--r--   0        0        0        0 2023-04-27 08:59:41.319369 sortinghat-0.9.2/sortinghat/core/migrations/__init__.py
--rw-r--r--   0        0        0    11931 2023-04-27 08:59:41.319369 sortinghat-0.9.2/sortinghat/core/models.py
--rw-r--r--   0        0        0      839 2023-04-27 08:59:41.319369 sortinghat-0.9.2/sortinghat/core/recommendations/__init__.py
--rw-r--r--   0        0        0     4272 2023-04-27 08:59:41.319369 sortinghat-0.9.2/sortinghat/core/recommendations/affiliation.py
--rw-r--r--   0        0        0     3137 2023-04-27 08:59:41.319369 sortinghat-0.9.2/sortinghat/core/recommendations/engine.py
--rw-r--r--   0        0        0     5313 2023-04-27 08:59:41.319369 sortinghat-0.9.2/sortinghat/core/recommendations/exclusion.py
--rw-r--r--   0        0        0     5642 2023-04-27 08:59:41.319369 sortinghat-0.9.2/sortinghat/core/recommendations/gender.py
--rw-r--r--   0        0        0     9134 2023-04-27 08:59:41.319369 sortinghat-0.9.2/sortinghat/core/recommendations/matching.py
--rw-r--r--   0        0        0    74254 2023-04-27 08:59:41.319369 sortinghat-0.9.2/sortinghat/core/schema.py
--rw-r--r--   0        0        0     3482 2023-04-27 09:01:29.286169 sortinghat-0.9.2/sortinghat/core/static/css/366.d54629c5.css
--rw-r--r--   0        0        0    20345 2023-04-27 09:01:29.286169 sortinghat-0.9.2/sortinghat/core/static/css/5.5bd7783b.css
--rw-r--r--   0        0        0     3482 2023-04-27 09:01:29.282169 sortinghat-0.9.2/sortinghat/core/static/css/56.d54629c5.css
--rw-r--r--   0        0        0    12938 2023-04-27 09:01:29.286169 sortinghat-0.9.2/sortinghat/core/static/css/561.91f3ebe2.css
--rw-r--r--   0        0        0    42743 2023-04-27 09:01:29.286169 sortinghat-0.9.2/sortinghat/core/static/css/574.5889fc28.css
--rw-r--r--   0        0        0    30992 2023-04-27 09:01:29.286169 sortinghat-0.9.2/sortinghat/core/static/css/762.6b2ccfca.css
--rw-r--r--   0        0        0    14063 2023-04-27 09:01:29.286169 sortinghat-0.9.2/sortinghat/core/static/css/841.73b7a8e2.css
--rw-r--r--   0        0        0    26518 2023-04-27 09:01:29.286169 sortinghat-0.9.2/sortinghat/core/static/css/894.f7e21c66.css
--rw-r--r--   0        0        0     6382 2023-04-27 09:01:29.282169 sortinghat-0.9.2/sortinghat/core/static/css/981.cb0d0293.css
--rw-r--r--   0        0        0    49100 2023-04-27 09:01:29.282169 sortinghat-0.9.2/sortinghat/core/static/css/987.a5ced4b6.css
--rw-r--r--   0        0        0     5085 2023-04-27 09:01:29.282169 sortinghat-0.9.2/sortinghat/core/static/css/app.28a862de.css
--rw-r--r--   0        0        0   557520 2023-04-27 09:01:29.286169 sortinghat-0.9.2/sortinghat/core/static/css/chunk-vendors.7dc1bb68.css
--rw-r--r--   0        0        0    15086 2023-04-27 09:01:29.286169 sortinghat-0.9.2/sortinghat/core/static/favicon-grimoirelab.ico
--rw-r--r--   0        0        0   140029 2023-04-27 09:01:29.278169 sortinghat-0.9.2/sortinghat/core/static/fonts/Roboto-Italic.6a5b2eb0.woff2
--rw-r--r--   0        0        0    99428 2023-04-27 09:01:29.278169 sortinghat-0.9.2/sortinghat/core/static/fonts/Roboto-Italic.76b8308b.woff
--rw-r--r--   0        0        0   173516 2023-04-27 09:01:29.282169 sortinghat-0.9.2/sortinghat/core/static/fonts/Roboto-Italic.991def81.ttf
--rw-r--r--   0        0        0    93472 2023-04-27 09:01:29.278169 sortinghat-0.9.2/sortinghat/core/static/fonts/Roboto-Light.2d3c72a3.woff
--rw-r--r--   0        0        0    65564 2023-04-27 09:01:29.278169 sortinghat-0.9.2/sortinghat/core/static/fonts/Roboto-Light.41cb61ed.woff2
--rw-r--r--   0        0        0   170012 2023-04-27 09:01:29.278169 sortinghat-0.9.2/sortinghat/core/static/fonts/Roboto-Light.f2e7274e.ttf
--rw-r--r--   0        0        0    72036 2023-04-27 09:01:29.278169 sortinghat-0.9.2/sortinghat/core/static/fonts/Roboto-LightItalic.07369d23.woff2
--rw-r--r--   0        0        0   101120 2023-04-27 09:01:29.278169 sortinghat-0.9.2/sortinghat/core/static/fonts/Roboto-LightItalic.45582c0c.woff
--rw-r--r--   0        0        0   176184 2023-04-27 09:01:29.278169 sortinghat-0.9.2/sortinghat/core/static/fonts/Roboto-LightItalic.b694f0fe.ttf
--rw-r--r--   0        0        0   133998 2023-04-27 09:01:29.282169 sortinghat-0.9.2/sortinghat/core/static/fonts/Roboto-Medium.13e0be98.woff2
--rw-r--r--   0        0        0    94364 2023-04-27 09:01:29.282169 sortinghat-0.9.2/sortinghat/core/static/fonts/Roboto-Medium.483a3bd1.woff
--rw-r--r--   0        0        0   171656 2023-04-27 09:01:29.282169 sortinghat-0.9.2/sortinghat/core/static/fonts/Roboto-Medium.af9d0139.ttf
--rw-r--r--   0        0        0   176428 2023-04-27 09:01:29.282169 sortinghat-0.9.2/sortinghat/core/static/fonts/Roboto-MediumItalic.3723a2e7.ttf
--rw-r--r--   0        0        0   101008 2023-04-27 09:01:29.282169 sortinghat-0.9.2/sortinghat/core/static/fonts/Roboto-MediumItalic.8b19cc18.woff
--rw-r--r--   0        0        0   139529 2023-04-27 09:01:29.282169 sortinghat-0.9.2/sortinghat/core/static/fonts/Roboto-MediumItalic.b35d3641.woff2
--rw-r--r--   0        0        0    93784 2023-04-27 09:01:29.278169 sortinghat-0.9.2/sortinghat/core/static/fonts/Roboto-Regular.36d4503d.woff
--rw-r--r--   0        0        0   171272 2023-04-27 09:01:29.278169 sortinghat-0.9.2/sortinghat/core/static/fonts/Roboto-Regular.ae3a8db9.ttf
--rw-r--r--   0        0        0    66012 2023-04-27 09:01:29.278169 sortinghat-0.9.2/sortinghat/core/static/fonts/Roboto-Regular.e0553e00.woff2
--rw-r--r--   0        0        0   862480 2023-04-27 09:01:29.278169 sortinghat-0.9.2/sortinghat/core/static/fonts/materialdesignicons-webfont.67f3950a.ttf
--rw-r--r--   0        0        0   399520 2023-04-27 09:01:29.278169 sortinghat-0.9.2/sortinghat/core/static/fonts/materialdesignicons-webfont.83bc1470.woff
--rw-r--r--   0        0        0   282384 2023-04-27 09:01:29.278169 sortinghat-0.9.2/sortinghat/core/static/fonts/materialdesignicons-webfont.d819e534.woff2
--rw-r--r--   0        0        0   862700 2023-04-27 09:01:29.278169 sortinghat-0.9.2/sortinghat/core/static/fonts/materialdesignicons-webfont.fbaf9d97.eot
--rw-r--r--   0        0        0     7811 2023-04-27 09:01:29.286169 sortinghat-0.9.2/sortinghat/core/static/js/366.db9f9acd.js
--rw-r--r--   0        0        0    23622 2023-04-27 09:01:29.286169 sortinghat-0.9.2/sortinghat/core/static/js/5.8197bd56.js
--rw-r--r--   0        0        0    27508 2023-04-27 09:01:29.282169 sortinghat-0.9.2/sortinghat/core/static/js/56.66e710bd.js
--rw-r--r--   0        0        0    22737 2023-04-27 09:01:29.286169 sortinghat-0.9.2/sortinghat/core/static/js/561.5943719e.js
--rw-r--r--   0        0        0    92334 2023-04-27 09:01:29.286169 sortinghat-0.9.2/sortinghat/core/static/js/574.bfb992b9.js
--rw-r--r--   0        0        0    27820 2023-04-27 09:01:29.286169 sortinghat-0.9.2/sortinghat/core/static/js/762.2ca33633.js
--rw-r--r--   0        0        0    13871 2023-04-27 09:01:29.286169 sortinghat-0.9.2/sortinghat/core/static/js/841.db6bdce9.js
--rw-r--r--   0        0        0    10855 2023-04-27 09:01:29.286169 sortinghat-0.9.2/sortinghat/core/static/js/894.1119152d.js
--rw-r--r--   0        0        0    11812 2023-04-27 09:01:29.286169 sortinghat-0.9.2/sortinghat/core/static/js/966.7c5c17a8.js
--rw-r--r--   0        0        0    17769 2023-04-27 09:01:29.282169 sortinghat-0.9.2/sortinghat/core/static/js/981.ba53d6b4.js
--rw-r--r--   0        0        0   144555 2023-04-27 09:01:29.282169 sortinghat-0.9.2/sortinghat/core/static/js/987.8a763c50.js
--rw-r--r--   0        0        0    26012 2023-04-27 09:01:29.286169 sortinghat-0.9.2/sortinghat/core/static/js/993.cda825ec.js
--rw-r--r--   0        0        0    22368 2023-04-27 09:01:29.282169 sortinghat-0.9.2/sortinghat/core/static/js/app.2b031f67.js
--rw-r--r--   0        0        0   496792 2023-04-27 09:01:29.286169 sortinghat-0.9.2/sortinghat/core/static/js/chunk-vendors.26a9eb41.js
--rw-r--r--   0        0        0      851 2023-04-27 09:01:29.286169 sortinghat-0.9.2/sortinghat/core/templates/index.html
--rw-r--r--   0        0        0     2394 2023-04-27 08:59:41.319369 sortinghat-0.9.2/sortinghat/core/tenant.py
--rw-r--r--   0        0        0     2944 2023-04-27 08:59:41.319369 sortinghat-0.9.2/sortinghat/core/views.py
--rw-r--r--   0        0        0        0 2023-04-27 08:59:41.319369 sortinghat-0.9.2/sortinghat/server/__init__.py
--rw-r--r--   0        0        0    13705 2023-04-27 08:59:41.319369 sortinghat-0.9.2/sortinghat/server/sortinghat_admin.py
--rw-r--r--   0        0        0     2884 2023-04-27 08:59:41.319369 sortinghat-0.9.2/sortinghat/server/sortinghatd.py
--rw-r--r--   0        0        0     2365 2023-04-27 08:59:41.319369 sortinghat-0.9.2/sortinghat/server/sortinghatw.py
--rwxr-xr-x   0        0        0     9218 2023-04-27 08:59:41.319369 sortinghat-0.9.2/sortinghat/server/utils/create_sh_0_7_fixture.py
--rw-r--r--   0        0        0     3485 2023-04-27 08:59:41.319369 sortinghat-0.9.2/sortinghat/utils/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 08:59:41.319369 sortinghat-0.9.2/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 08:59:41.319369 sortinghat-0.9.2/tests/cli/__init__.py
--rw-r--r--   0        0        0       57 2023-04-27 08:59:41.319369 sortinghat-0.9.2/tests/cli/config_file.cfg
--rw-r--r--   0        0        0     7601 2023-04-27 08:59:41.319369 sortinghat-0.9.2/tests/cli/test_cmd_add.py
--rw-r--r--   0        0        0    17698 2023-04-27 08:59:41.319369 sortinghat-0.9.2/tests/cli/test_cmd_config.py
--rw-r--r--   0        0        0    10234 2023-04-27 08:59:41.319369 sortinghat-0.9.2/tests/cli/test_cmd_countries.py
--rw-r--r--   0        0        0     7597 2023-04-27 08:59:41.319369 sortinghat-0.9.2/tests/cli/test_cmd_enroll.py
--rw-r--r--   0        0        0     5397 2023-04-27 08:59:41.319369 sortinghat-0.9.2/tests/cli/test_cmd_lock.py
--rw-r--r--   0        0        0     3851 2023-04-27 08:59:41.319369 sortinghat-0.9.2/tests/cli/test_cmd_merge.py
--rw-r--r--   0        0        0     5041 2023-04-27 08:59:41.319369 sortinghat-0.9.2/tests/cli/test_cmd_mv.py
--rw-r--r--   0        0        0    13658 2023-04-27 08:59:41.319369 sortinghat-0.9.2/tests/cli/test_cmd_orgs.py
--rw-r--r--   0        0        0     9117 2023-04-27 08:59:41.319369 sortinghat-0.9.2/tests/cli/test_cmd_profile.py
--rw-r--r--   0        0        0     4599 2023-04-27 08:59:41.319369 sortinghat-0.9.2/tests/cli/test_cmd_rm.py
--rw-r--r--   0        0        0    10993 2023-04-27 08:59:41.319369 sortinghat-0.9.2/tests/cli/test_cmd_show.py
--rw-r--r--   0        0        0     5280 2023-04-27 08:59:41.319369 sortinghat-0.9.2/tests/cli/test_cmd_split.py
--rw-r--r--   0        0        0     6294 2023-04-27 08:59:41.319369 sortinghat-0.9.2/tests/cli/test_cmd_withdraw.py
--rw-r--r--   0        0        0        0 2023-04-27 08:59:41.319369 sortinghat-0.9.2/tests/importer/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 08:59:41.319369 sortinghat-0.9.2/tests/importer/mocked_package/__init__.py
--rw-r--r--   0        0        0     1055 2023-04-27 08:59:41.319369 sortinghat-0.9.2/tests/importer/mocked_package/backend_a.py
--rw-r--r--   0        0        0        0 2023-04-27 08:59:41.319369 sortinghat-0.9.2/tests/importer/mocked_package/nested_package/__init__.py
--rw-r--r--   0        0        0      950 2023-04-27 08:59:41.319369 sortinghat-0.9.2/tests/importer/mocked_package/nested_package/nested_backend_b.py
--rw-r--r--   0        0        0     1050 2023-04-27 08:59:41.319369 sortinghat-0.9.2/tests/importer/mocked_package/nested_package/nested_backend_c.py
--rw-r--r--   0        0        0      865 2023-04-27 08:59:41.319369 sortinghat-0.9.2/tests/importer/mocked_package/nested_package/nested_not_backend.py
--rw-r--r--   0        0        0     4797 2023-04-27 08:59:41.319369 sortinghat-0.9.2/tests/importer/test_backend.py
--rw-r--r--   0        0        0     2416 2023-04-27 08:59:41.319369 sortinghat-0.9.2/tests/importer/test_utils.py
--rw-r--r--   0        0        0        0 2023-04-27 08:59:41.319369 sortinghat-0.9.2/tests/rec/__init__.py
--rw-r--r--   0        0        0     7474 2023-04-27 08:59:41.319369 sortinghat-0.9.2/tests/rec/test_affiliations.py
--rw-r--r--   0        0        0     2922 2023-04-27 08:59:41.319369 sortinghat-0.9.2/tests/rec/test_engine.py
--rw-r--r--   0        0        0     3937 2023-04-27 08:59:41.319369 sortinghat-0.9.2/tests/rec/test_exclusion.py
--rw-r--r--   0        0        0     8536 2023-04-27 08:59:41.319369 sortinghat-0.9.2/tests/rec/test_gender.py
--rw-r--r--   0        0        0    11764 2023-04-27 08:59:41.319369 sortinghat-0.9.2/tests/rec/test_matches.py
--rw-r--r--   0        0        0      825 2023-04-27 08:59:41.319369 sortinghat-0.9.2/tests/runners.py
--rw-r--r--   0        0        0        0 2023-04-27 08:59:41.319369 sortinghat-0.9.2/tests/tenants/__init__.py
--rw-r--r--   0        0        0     3781 2023-04-27 08:59:41.319369 sortinghat-0.9.2/tests/tenants/test_jobs.py
--rw-r--r--   0        0        0     2273 2023-04-27 08:59:41.319369 sortinghat-0.9.2/tests/tenants/test_middleware.py
--rw-r--r--   0        0        0     5872 2023-04-27 08:59:41.319369 sortinghat-0.9.2/tests/tenants/test_schema.py
--rw-r--r--   0        0        0   258794 2023-04-27 08:59:41.319369 sortinghat-0.9.2/tests/test_api.py
--rw-r--r--   0        0        0    18369 2023-04-27 08:59:41.319369 sortinghat-0.9.2/tests/test_aux.py
--rw-r--r--   0        0        0    10449 2023-04-27 08:59:41.319369 sortinghat-0.9.2/tests/test_client.py
--rw-r--r--   0        0        0   125568 2023-04-27 08:59:41.323369 sortinghat-0.9.2/tests/test_db.py
--rw-r--r--   0        0        0     9257 2023-04-27 08:59:41.323369 sortinghat-0.9.2/tests/test_errors.py
--rw-r--r--   0        0        0    54990 2023-04-27 08:59:41.323369 sortinghat-0.9.2/tests/test_jobs.py
--rw-r--r--   0        0        0    14074 2023-04-27 08:59:41.323369 sortinghat-0.9.2/tests/test_log.py
--rw-r--r--   0        0        0    47504 2023-04-27 08:59:41.323369 sortinghat-0.9.2/tests/test_model.py
--rw-r--r--   0        0        0   399040 2023-04-27 08:59:41.323369 sortinghat-0.9.2/tests/test_schema.py
--rw-r--r--   0        0        0     6316 2023-04-27 08:59:41.323369 sortinghat-0.9.2/tests/test_utils.py
--rw-r--r--   0        0        0    10399 1970-01-01 00:00:00.000000 sortinghat-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0      363 2023-04-28 16:00:58.825470 sortinghat-0.9.3/AUTHORS
+-rw-r--r--   0        0        0    35147 2023-04-28 16:00:58.825470 sortinghat-0.9.3/LICENSE
+-rw-r--r--   0        0        0    14918 2023-04-28 16:00:58.825470 sortinghat-0.9.3/NEWS
+-rw-r--r--   0        0        0     8566 2023-04-28 16:00:58.825470 sortinghat-0.9.3/README.md
+-rw-r--r--   0        0        0     2049 2023-04-28 16:00:58.825470 sortinghat-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0       86 2023-04-28 16:00:58.829470 sortinghat-0.9.3/sortinghat/_version.py
+-rw-r--r--   0        0        0        0 2023-04-28 16:00:58.829470 sortinghat-0.9.3/sortinghat/app/__init__.py
+-rw-r--r--   0        0        0     1250 2023-04-28 16:00:58.829470 sortinghat-0.9.3/sortinghat/app/schema.py
+-rw-r--r--   0        0        0      518 2023-04-28 16:00:58.829470 sortinghat-0.9.3/sortinghat/app/urls.py
+-rw-r--r--   0        0        0      196 2023-04-28 16:00:58.829470 sortinghat-0.9.3/sortinghat/app/wsgi.py
+-rw-r--r--   0        0        0        0 2023-04-28 16:00:58.829470 sortinghat-0.9.3/sortinghat/cli/__init__.py
+-rw-r--r--   0        0        0      977 2023-04-28 16:00:58.829470 sortinghat-0.9.3/sortinghat/cli/client/__init__.py
+-rw-r--r--   0        0        0     5738 2023-04-28 16:00:58.829470 sortinghat-0.9.3/sortinghat/cli/client/client.py
+-rw-r--r--   0        0        0    43408 2023-04-28 16:00:58.829470 sortinghat-0.9.3/sortinghat/cli/client/schema.py
+-rw-r--r--   0        0        0        0 2023-04-28 16:00:58.829470 sortinghat-0.9.3/sortinghat/cli/cmds/__init__.py
+-rw-r--r--   0        0        0     3072 2023-04-28 16:00:58.829470 sortinghat-0.9.3/sortinghat/cli/cmds/add.py
+-rw-r--r--   0        0        0     6145 2023-04-28 16:00:58.829470 sortinghat-0.9.3/sortinghat/cli/cmds/config.py
+-rw-r--r--   0        0        0     3219 2023-04-28 16:00:58.829470 sortinghat-0.9.3/sortinghat/cli/cmds/countries.py
+-rw-r--r--   0        0        0     3462 2023-04-28 16:00:58.829470 sortinghat-0.9.3/sortinghat/cli/cmds/enroll.py
+-rw-r--r--   0        0        0     2860 2023-04-28 16:00:58.829470 sortinghat-0.9.3/sortinghat/cli/cmds/lock.py
+-rw-r--r--   0        0        0     2342 2023-04-28 16:00:58.829470 sortinghat-0.9.3/sortinghat/cli/cmds/merge.py
+-rw-r--r--   0        0        0     2352 2023-04-28 16:00:58.829470 sortinghat-0.9.3/sortinghat/cli/cmds/mv.py
+-rw-r--r--   0        0        0     7466 2023-04-28 16:00:58.829470 sortinghat-0.9.3/sortinghat/cli/cmds/orgs.py
+-rw-r--r--   0        0        0     2934 2023-04-28 16:00:58.829470 sortinghat-0.9.3/sortinghat/cli/cmds/profile.py
+-rw-r--r--   0        0        0     1992 2023-04-28 16:00:58.829470 sortinghat-0.9.3/sortinghat/cli/cmds/rm.py
+-rw-r--r--   0        0        0     2909 2023-04-28 16:00:58.829470 sortinghat-0.9.3/sortinghat/cli/cmds/show.py
+-rw-r--r--   0        0        0     2365 2023-04-28 16:00:58.829470 sortinghat-0.9.3/sortinghat/cli/cmds/split.py
+-rw-r--r--   0        0        0     3364 2023-04-28 16:00:58.829470 sortinghat-0.9.3/sortinghat/cli/cmds/withdraw.py
+-rwxr-xr-x   0        0        0     2857 2023-04-28 16:00:58.829470 sortinghat-0.9.3/sortinghat/cli/sortinghat.py
+-rw-r--r--   0        0        0       43 2023-04-28 16:00:58.829470 sortinghat-0.9.3/sortinghat/cli/templates/add.tmpl
+-rw-r--r--   0        0        0       23 2023-04-28 16:00:58.829470 sortinghat-0.9.3/sortinghat/cli/templates/config.tmpl
+-rw-r--r--   0        0        0       83 2023-04-28 16:00:58.829470 sortinghat-0.9.3/sortinghat/cli/templates/countries.tmpl
+-rw-r--r--   0        0        0       54 2023-04-28 16:00:58.829470 sortinghat-0.9.3/sortinghat/cli/templates/lock.tmpl
+-rw-r--r--   0        0        0      169 2023-04-28 16:00:58.829470 sortinghat-0.9.3/sortinghat/cli/templates/mv.tmpl
+-rw-r--r--   0        0        0      208 2023-04-28 16:00:58.829470 sortinghat-0.9.3/sortinghat/cli/templates/organizations.tmpl
+-rw-r--r--   0        0        0      375 2023-04-28 16:00:58.829470 sortinghat-0.9.3/sortinghat/cli/templates/profile.tmpl
+-rw-r--r--   0        0        0      106 2023-04-28 16:00:58.829470 sortinghat-0.9.3/sortinghat/cli/templates/rm.tmpl
+-rw-r--r--   0        0        0     1016 2023-04-28 16:00:58.829470 sortinghat-0.9.3/sortinghat/cli/templates/show.tmpl
+-rw-r--r--   0        0        0       69 2023-04-28 16:00:58.829470 sortinghat-0.9.3/sortinghat/cli/templates/split.tmpl
+-rw-r--r--   0        0        0     4856 2023-04-28 16:00:58.829470 sortinghat-0.9.3/sortinghat/cli/utils.py
+-rw-r--r--   0        0        0        0 2023-04-28 16:00:58.829470 sortinghat-0.9.3/sortinghat/config/__init__.py
+-rw-r--r--   0        0        0     9252 2023-04-28 16:00:58.829470 sortinghat-0.9.3/sortinghat/config/settings.py
+-rw-r--r--   0        0        0       20 2023-04-28 16:00:58.829470 sortinghat-0.9.3/sortinghat/config/tenants.json
+-rw-r--r--   0        0        0     1544 2023-04-28 16:00:58.829470 sortinghat-0.9.3/sortinghat/core/admin.py
+-rw-r--r--   0        0        0    50534 2023-04-28 16:00:58.829470 sortinghat-0.9.3/sortinghat/core/api.py
+-rw-r--r--   0        0        0      926 2023-04-28 16:00:58.829470 sortinghat-0.9.3/sortinghat/core/apps.py
+-rw-r--r--   0        0        0     5169 2023-04-28 16:00:58.829470 sortinghat-0.9.3/sortinghat/core/aux.py
+-rw-r--r--   0        0        0      997 2023-04-28 16:00:58.829470 sortinghat-0.9.3/sortinghat/core/context.py
+-rw-r--r--   0        0        0    37055 2023-04-28 16:00:58.829470 sortinghat-0.9.3/sortinghat/core/db.py
+-rw-r--r--   0        0        0     3205 2023-04-28 16:00:58.829470 sortinghat-0.9.3/sortinghat/core/decorators.py
+-rw-r--r--   0        0        0     3875 2023-04-28 16:00:58.829470 sortinghat-0.9.3/sortinghat/core/errors.py
+-rw-r--r--   0        0        0    41236 2023-04-28 16:00:58.829470 sortinghat-0.9.3/sortinghat/core/fixtures/countries.json
+-rw-r--r--   0        0        0     7820 2023-04-28 16:00:58.829470 sortinghat-0.9.3/sortinghat/core/importer/backend.py
+-rw-r--r--   0        0        0     7136 2023-04-28 16:00:58.833469 sortinghat-0.9.3/sortinghat/core/importer/backends/mailmap.py
+-rw-r--r--   0        0        0     5817 2023-04-28 16:00:58.833469 sortinghat-0.9.3/sortinghat/core/importer/base.py
+-rw-r--r--   0        0        0     2143 2023-04-28 16:00:58.833469 sortinghat-0.9.3/sortinghat/core/importer/models.py
+-rw-r--r--   0        0        0     2059 2023-04-28 16:00:58.833469 sortinghat-0.9.3/sortinghat/core/importer/utils.py
+-rw-r--r--   0        0        0    25814 2023-04-28 16:00:58.833469 sortinghat-0.9.3/sortinghat/core/jobs.py
+-rw-r--r--   0        0        0     7298 2023-04-28 16:00:58.833469 sortinghat-0.9.3/sortinghat/core/log.py
+-rw-r--r--   0        0        0        0 2023-04-28 16:00:58.833469 sortinghat-0.9.3/sortinghat/core/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-28 16:00:58.833469 sortinghat-0.9.3/sortinghat/core/management/commands/__init__.py
+-rw-r--r--   0        0        0     4155 2023-04-28 16:00:58.833469 sortinghat-0.9.3/sortinghat/core/management/commands/create_groups.py
+-rw-r--r--   0        0        0     4354 2023-04-28 16:00:58.833469 sortinghat-0.9.3/sortinghat/core/middleware.py
+-rw-r--r--   0        0        0    14035 2023-04-28 16:00:58.833469 sortinghat-0.9.3/sortinghat/core/migrations/0001_sortinghat.py
+-rw-r--r--   0        0        0     1717 2023-04-28 16:00:58.833469 sortinghat-0.9.3/sortinghat/core/migrations/0002_importidentitiestask.py
+-rw-r--r--   0        0        0     1502 2023-04-28 16:00:58.833469 sortinghat-0.9.3/sortinghat/core/migrations/0003_multi_tenancy.py
+-rw-r--r--   0        0        0        0 2023-04-28 16:00:58.833469 sortinghat-0.9.3/sortinghat/core/migrations/__init__.py
+-rw-r--r--   0        0        0    11931 2023-04-28 16:00:58.833469 sortinghat-0.9.3/sortinghat/core/models.py
+-rw-r--r--   0        0        0      839 2023-04-28 16:00:58.833469 sortinghat-0.9.3/sortinghat/core/recommendations/__init__.py
+-rw-r--r--   0        0        0     4272 2023-04-28 16:00:58.833469 sortinghat-0.9.3/sortinghat/core/recommendations/affiliation.py
+-rw-r--r--   0        0        0     3137 2023-04-28 16:00:58.833469 sortinghat-0.9.3/sortinghat/core/recommendations/engine.py
+-rw-r--r--   0        0        0     5313 2023-04-28 16:00:58.833469 sortinghat-0.9.3/sortinghat/core/recommendations/exclusion.py
+-rw-r--r--   0        0        0     5642 2023-04-28 16:00:58.833469 sortinghat-0.9.3/sortinghat/core/recommendations/gender.py
+-rw-r--r--   0        0        0     9134 2023-04-28 16:00:58.833469 sortinghat-0.9.3/sortinghat/core/recommendations/matching.py
+-rw-r--r--   0        0        0    74254 2023-04-28 16:00:58.833469 sortinghat-0.9.3/sortinghat/core/schema.py
+-rw-r--r--   0        0        0     3482 2023-04-28 16:03:31.657948 sortinghat-0.9.3/sortinghat/core/static/css/366.d54629c5.css
+-rw-r--r--   0        0        0    20345 2023-04-28 16:03:31.669948 sortinghat-0.9.3/sortinghat/core/static/css/5.5bd7783b.css
+-rw-r--r--   0        0        0     3482 2023-04-28 16:03:31.645948 sortinghat-0.9.3/sortinghat/core/static/css/56.d54629c5.css
+-rw-r--r--   0        0        0    12938 2023-04-28 16:03:31.657948 sortinghat-0.9.3/sortinghat/core/static/css/561.91f3ebe2.css
+-rw-r--r--   0        0        0    42743 2023-04-28 16:03:31.673948 sortinghat-0.9.3/sortinghat/core/static/css/574.5889fc28.css
+-rw-r--r--   0        0        0    30992 2023-04-28 16:03:31.669948 sortinghat-0.9.3/sortinghat/core/static/css/762.6b2ccfca.css
+-rw-r--r--   0        0        0    14063 2023-04-28 16:03:31.657948 sortinghat-0.9.3/sortinghat/core/static/css/841.73b7a8e2.css
+-rw-r--r--   0        0        0    26518 2023-04-28 16:03:31.657948 sortinghat-0.9.3/sortinghat/core/static/css/894.f7e21c66.css
+-rw-r--r--   0        0        0     6382 2023-04-28 16:03:31.645948 sortinghat-0.9.3/sortinghat/core/static/css/981.cb0d0293.css
+-rw-r--r--   0        0        0    49100 2023-04-28 16:03:31.645948 sortinghat-0.9.3/sortinghat/core/static/css/987.a5ced4b6.css
+-rw-r--r--   0        0        0     5085 2023-04-28 16:03:31.645948 sortinghat-0.9.3/sortinghat/core/static/css/app.28a862de.css
+-rw-r--r--   0        0        0   557520 2023-04-28 16:03:31.669948 sortinghat-0.9.3/sortinghat/core/static/css/chunk-vendors.7dc1bb68.css
+-rw-r--r--   0        0        0    15086 2023-04-28 16:03:31.673948 sortinghat-0.9.3/sortinghat/core/static/favicon-grimoirelab.ico
+-rw-r--r--   0        0        0   140029 2023-04-28 16:03:31.605948 sortinghat-0.9.3/sortinghat/core/static/fonts/Roboto-Italic.6a5b2eb0.woff2
+-rw-r--r--   0        0        0    99428 2023-04-28 16:03:31.605948 sortinghat-0.9.3/sortinghat/core/static/fonts/Roboto-Italic.76b8308b.woff
+-rw-r--r--   0        0        0   173516 2023-04-28 16:03:31.629948 sortinghat-0.9.3/sortinghat/core/static/fonts/Roboto-Italic.991def81.ttf
+-rw-r--r--   0        0        0    93472 2023-04-28 16:03:31.601948 sortinghat-0.9.3/sortinghat/core/static/fonts/Roboto-Light.2d3c72a3.woff
+-rw-r--r--   0        0        0    65564 2023-04-28 16:03:31.601948 sortinghat-0.9.3/sortinghat/core/static/fonts/Roboto-Light.41cb61ed.woff2
+-rw-r--r--   0        0        0   170012 2023-04-28 16:03:31.601948 sortinghat-0.9.3/sortinghat/core/static/fonts/Roboto-Light.f2e7274e.ttf
+-rw-r--r--   0        0        0    72036 2023-04-28 16:03:31.601948 sortinghat-0.9.3/sortinghat/core/static/fonts/Roboto-LightItalic.07369d23.woff2
+-rw-r--r--   0        0        0   101120 2023-04-28 16:03:31.601948 sortinghat-0.9.3/sortinghat/core/static/fonts/Roboto-LightItalic.45582c0c.woff
+-rw-r--r--   0        0        0   176184 2023-04-28 16:03:31.601948 sortinghat-0.9.3/sortinghat/core/static/fonts/Roboto-LightItalic.b694f0fe.ttf
+-rw-r--r--   0        0        0   133998 2023-04-28 16:03:31.645948 sortinghat-0.9.3/sortinghat/core/static/fonts/Roboto-Medium.13e0be98.woff2
+-rw-r--r--   0        0        0    94364 2023-04-28 16:03:31.645948 sortinghat-0.9.3/sortinghat/core/static/fonts/Roboto-Medium.483a3bd1.woff
+-rw-r--r--   0        0        0   171656 2023-04-28 16:03:31.645948 sortinghat-0.9.3/sortinghat/core/static/fonts/Roboto-Medium.af9d0139.ttf
+-rw-r--r--   0        0        0   176428 2023-04-28 16:03:31.645948 sortinghat-0.9.3/sortinghat/core/static/fonts/Roboto-MediumItalic.3723a2e7.ttf
+-rw-r--r--   0        0        0   101008 2023-04-28 16:03:31.645948 sortinghat-0.9.3/sortinghat/core/static/fonts/Roboto-MediumItalic.8b19cc18.woff
+-rw-r--r--   0        0        0   139529 2023-04-28 16:03:31.645948 sortinghat-0.9.3/sortinghat/core/static/fonts/Roboto-MediumItalic.b35d3641.woff2
+-rw-r--r--   0        0        0    93784 2023-04-28 16:03:31.601948 sortinghat-0.9.3/sortinghat/core/static/fonts/Roboto-Regular.36d4503d.woff
+-rw-r--r--   0        0        0   171272 2023-04-28 16:03:31.605948 sortinghat-0.9.3/sortinghat/core/static/fonts/Roboto-Regular.ae3a8db9.ttf
+-rw-r--r--   0        0        0    66012 2023-04-28 16:03:31.601948 sortinghat-0.9.3/sortinghat/core/static/fonts/Roboto-Regular.e0553e00.woff2
+-rw-r--r--   0        0        0   862480 2023-04-28 16:03:31.597948 sortinghat-0.9.3/sortinghat/core/static/fonts/materialdesignicons-webfont.67f3950a.ttf
+-rw-r--r--   0        0        0   399520 2023-04-28 16:03:31.597948 sortinghat-0.9.3/sortinghat/core/static/fonts/materialdesignicons-webfont.83bc1470.woff
+-rw-r--r--   0        0        0   282384 2023-04-28 16:03:31.597948 sortinghat-0.9.3/sortinghat/core/static/fonts/materialdesignicons-webfont.d819e534.woff2
+-rw-r--r--   0        0        0   862700 2023-04-28 16:03:31.597948 sortinghat-0.9.3/sortinghat/core/static/fonts/materialdesignicons-webfont.fbaf9d97.eot
+-rw-r--r--   0        0        0     7811 2023-04-28 16:03:31.657948 sortinghat-0.9.3/sortinghat/core/static/js/366.db9f9acd.js
+-rw-r--r--   0        0        0    23622 2023-04-28 16:03:31.669948 sortinghat-0.9.3/sortinghat/core/static/js/5.8197bd56.js
+-rw-r--r--   0        0        0    27508 2023-04-28 16:03:31.645948 sortinghat-0.9.3/sortinghat/core/static/js/56.66e710bd.js
+-rw-r--r--   0        0        0    22737 2023-04-28 16:03:31.657948 sortinghat-0.9.3/sortinghat/core/static/js/561.5943719e.js
+-rw-r--r--   0        0        0    92334 2023-04-28 16:03:31.673948 sortinghat-0.9.3/sortinghat/core/static/js/574.bfb992b9.js
+-rw-r--r--   0        0        0    27820 2023-04-28 16:03:31.669948 sortinghat-0.9.3/sortinghat/core/static/js/762.2ca33633.js
+-rw-r--r--   0        0        0    13871 2023-04-28 16:03:31.657948 sortinghat-0.9.3/sortinghat/core/static/js/841.db6bdce9.js
+-rw-r--r--   0        0        0    10855 2023-04-28 16:03:31.657948 sortinghat-0.9.3/sortinghat/core/static/js/894.1119152d.js
+-rw-r--r--   0        0        0    11812 2023-04-28 16:03:31.673948 sortinghat-0.9.3/sortinghat/core/static/js/966.7c5c17a8.js
+-rw-r--r--   0        0        0    17769 2023-04-28 16:03:31.645948 sortinghat-0.9.3/sortinghat/core/static/js/981.ba53d6b4.js
+-rw-r--r--   0        0        0   144555 2023-04-28 16:03:31.645948 sortinghat-0.9.3/sortinghat/core/static/js/987.8a763c50.js
+-rw-r--r--   0        0        0    26012 2023-04-28 16:03:31.669948 sortinghat-0.9.3/sortinghat/core/static/js/993.cda825ec.js
+-rw-r--r--   0        0        0    22368 2023-04-28 16:03:31.645948 sortinghat-0.9.3/sortinghat/core/static/js/app.2b031f67.js
+-rw-r--r--   0        0        0   496792 2023-04-28 16:03:31.669948 sortinghat-0.9.3/sortinghat/core/static/js/chunk-vendors.26a9eb41.js
+-rw-r--r--   0        0        0      851 2023-04-28 16:03:31.673948 sortinghat-0.9.3/sortinghat/core/templates/index.html
+-rw-r--r--   0        0        0     2394 2023-04-28 16:00:58.833469 sortinghat-0.9.3/sortinghat/core/tenant.py
+-rw-r--r--   0        0        0     2944 2023-04-28 16:00:58.833469 sortinghat-0.9.3/sortinghat/core/views.py
+-rw-r--r--   0        0        0        0 2023-04-28 16:00:58.833469 sortinghat-0.9.3/sortinghat/server/__init__.py
+-rw-r--r--   0        0        0    13705 2023-04-28 16:00:58.833469 sortinghat-0.9.3/sortinghat/server/sortinghat_admin.py
+-rw-r--r--   0        0        0     2884 2023-04-28 16:00:58.833469 sortinghat-0.9.3/sortinghat/server/sortinghatd.py
+-rw-r--r--   0        0        0     2365 2023-04-28 16:00:58.833469 sortinghat-0.9.3/sortinghat/server/sortinghatw.py
+-rwxr-xr-x   0        0        0     9218 2023-04-28 16:00:58.833469 sortinghat-0.9.3/sortinghat/server/utils/create_sh_0_7_fixture.py
+-rw-r--r--   0        0        0     3485 2023-04-28 16:00:58.833469 sortinghat-0.9.3/sortinghat/utils/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-28 16:00:58.833469 sortinghat-0.9.3/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-28 16:00:58.833469 sortinghat-0.9.3/tests/cli/__init__.py
+-rw-r--r--   0        0        0       57 2023-04-28 16:00:58.833469 sortinghat-0.9.3/tests/cli/config_file.cfg
+-rw-r--r--   0        0        0     7601 2023-04-28 16:00:58.833469 sortinghat-0.9.3/tests/cli/test_cmd_add.py
+-rw-r--r--   0        0        0    17698 2023-04-28 16:00:58.833469 sortinghat-0.9.3/tests/cli/test_cmd_config.py
+-rw-r--r--   0        0        0    10234 2023-04-28 16:00:58.833469 sortinghat-0.9.3/tests/cli/test_cmd_countries.py
+-rw-r--r--   0        0        0     7597 2023-04-28 16:00:58.833469 sortinghat-0.9.3/tests/cli/test_cmd_enroll.py
+-rw-r--r--   0        0        0     5397 2023-04-28 16:00:58.833469 sortinghat-0.9.3/tests/cli/test_cmd_lock.py
+-rw-r--r--   0        0        0     3851 2023-04-28 16:00:58.833469 sortinghat-0.9.3/tests/cli/test_cmd_merge.py
+-rw-r--r--   0        0        0     5041 2023-04-28 16:00:58.833469 sortinghat-0.9.3/tests/cli/test_cmd_mv.py
+-rw-r--r--   0        0        0    13658 2023-04-28 16:00:58.833469 sortinghat-0.9.3/tests/cli/test_cmd_orgs.py
+-rw-r--r--   0        0        0     9117 2023-04-28 16:00:58.833469 sortinghat-0.9.3/tests/cli/test_cmd_profile.py
+-rw-r--r--   0        0        0     4599 2023-04-28 16:00:58.833469 sortinghat-0.9.3/tests/cli/test_cmd_rm.py
+-rw-r--r--   0        0        0    10993 2023-04-28 16:00:58.833469 sortinghat-0.9.3/tests/cli/test_cmd_show.py
+-rw-r--r--   0        0        0     5280 2023-04-28 16:00:58.833469 sortinghat-0.9.3/tests/cli/test_cmd_split.py
+-rw-r--r--   0        0        0     6294 2023-04-28 16:00:58.833469 sortinghat-0.9.3/tests/cli/test_cmd_withdraw.py
+-rw-r--r--   0        0        0        0 2023-04-28 16:00:58.833469 sortinghat-0.9.3/tests/importer/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-28 16:00:58.833469 sortinghat-0.9.3/tests/importer/mocked_package/__init__.py
+-rw-r--r--   0        0        0     1055 2023-04-28 16:00:58.833469 sortinghat-0.9.3/tests/importer/mocked_package/backend_a.py
+-rw-r--r--   0        0        0        0 2023-04-28 16:00:58.833469 sortinghat-0.9.3/tests/importer/mocked_package/nested_package/__init__.py
+-rw-r--r--   0        0        0      950 2023-04-28 16:00:58.833469 sortinghat-0.9.3/tests/importer/mocked_package/nested_package/nested_backend_b.py
+-rw-r--r--   0        0        0     1050 2023-04-28 16:00:58.833469 sortinghat-0.9.3/tests/importer/mocked_package/nested_package/nested_backend_c.py
+-rw-r--r--   0        0        0      865 2023-04-28 16:00:58.833469 sortinghat-0.9.3/tests/importer/mocked_package/nested_package/nested_not_backend.py
+-rw-r--r--   0        0        0     4797 2023-04-28 16:00:58.833469 sortinghat-0.9.3/tests/importer/test_backend.py
+-rw-r--r--   0        0        0     2416 2023-04-28 16:00:58.833469 sortinghat-0.9.3/tests/importer/test_utils.py
+-rw-r--r--   0        0        0        0 2023-04-28 16:00:58.833469 sortinghat-0.9.3/tests/rec/__init__.py
+-rw-r--r--   0        0        0     7474 2023-04-28 16:00:58.833469 sortinghat-0.9.3/tests/rec/test_affiliations.py
+-rw-r--r--   0        0        0     2922 2023-04-28 16:00:58.833469 sortinghat-0.9.3/tests/rec/test_engine.py
+-rw-r--r--   0        0        0     3937 2023-04-28 16:00:58.837470 sortinghat-0.9.3/tests/rec/test_exclusion.py
+-rw-r--r--   0        0        0     8536 2023-04-28 16:00:58.837470 sortinghat-0.9.3/tests/rec/test_gender.py
+-rw-r--r--   0        0        0    11764 2023-04-28 16:00:58.837470 sortinghat-0.9.3/tests/rec/test_matches.py
+-rw-r--r--   0        0        0      825 2023-04-28 16:00:58.837470 sortinghat-0.9.3/tests/runners.py
+-rw-r--r--   0        0        0        0 2023-04-28 16:00:58.837470 sortinghat-0.9.3/tests/tenants/__init__.py
+-rw-r--r--   0        0        0     3781 2023-04-28 16:00:58.837470 sortinghat-0.9.3/tests/tenants/test_jobs.py
+-rw-r--r--   0        0        0     2273 2023-04-28 16:00:58.837470 sortinghat-0.9.3/tests/tenants/test_middleware.py
+-rw-r--r--   0        0        0     5872 2023-04-28 16:00:58.837470 sortinghat-0.9.3/tests/tenants/test_schema.py
+-rw-r--r--   0        0        0   258794 2023-04-28 16:00:58.837470 sortinghat-0.9.3/tests/test_api.py
+-rw-r--r--   0        0        0    18369 2023-04-28 16:00:58.837470 sortinghat-0.9.3/tests/test_aux.py
+-rw-r--r--   0        0        0    10449 2023-04-28 16:00:58.837470 sortinghat-0.9.3/tests/test_client.py
+-rw-r--r--   0        0        0   125568 2023-04-28 16:00:58.837470 sortinghat-0.9.3/tests/test_db.py
+-rw-r--r--   0        0        0     9257 2023-04-28 16:00:58.837470 sortinghat-0.9.3/tests/test_errors.py
+-rw-r--r--   0        0        0    54990 2023-04-28 16:00:58.837470 sortinghat-0.9.3/tests/test_jobs.py
+-rw-r--r--   0        0        0    14074 2023-04-28 16:00:58.837470 sortinghat-0.9.3/tests/test_log.py
+-rw-r--r--   0        0        0    47504 2023-04-28 16:00:58.837470 sortinghat-0.9.3/tests/test_model.py
+-rw-r--r--   0        0        0   399040 2023-04-28 16:00:58.841470 sortinghat-0.9.3/tests/test_schema.py
+-rw-r--r--   0        0        0     6316 2023-04-28 16:00:58.841470 sortinghat-0.9.3/tests/test_utils.py
+-rw-r--r--   0        0        0    10399 1970-01-01 00:00:00.000000 sortinghat-0.9.3/PKG-INFO
```

### Comparing `sortinghat-0.9.2/LICENSE` & `sortinghat-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/NEWS` & `sortinghat-0.9.3/NEWS`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,18 @@
 # Releases
 
+## sortinghat 0.9.3 - (2023-04-28)
+
+**Bug fixes:**
+
+ * Tenant selection in job fixed\
+   Tenant selection raised an error when the job context was defined as
+   keyword argument.
+
+
 ## sortinghat 0.9.2 - (2023-04-27)
 
 **Bug fixes:**
 
  * Static files not included in wheel package\
    SortingHat static files were not included in the Python package. The
    problem was in the GitHub action.
```

### Comparing `sortinghat-0.9.2/README.md` & `sortinghat-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/pyproject.toml` & `sortinghat-0.9.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sortinghat"
-version = "0.9.2"
+version = "0.9.3"
 description = "A tool to manage identities."
 authors = [
     "GrimoireLab Developers"
 ]
 license = "GPL-3.0+"
 
 readme = "README.md"
```

### Comparing `sortinghat-0.9.2/sortinghat/app/schema.py` & `sortinghat-0.9.3/sortinghat/app/schema.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/app/urls.py` & `sortinghat-0.9.3/sortinghat/app/urls.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/cli/client/__init__.py` & `sortinghat-0.9.3/sortinghat/cli/client/__init__.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/cli/client/client.py` & `sortinghat-0.9.3/sortinghat/cli/client/client.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/cli/client/schema.py` & `sortinghat-0.9.3/sortinghat/cli/client/schema.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/cli/cmds/add.py` & `sortinghat-0.9.3/sortinghat/cli/cmds/add.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/cli/cmds/config.py` & `sortinghat-0.9.3/sortinghat/cli/cmds/config.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/cli/cmds/countries.py` & `sortinghat-0.9.3/sortinghat/cli/cmds/countries.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/cli/cmds/enroll.py` & `sortinghat-0.9.3/sortinghat/cli/cmds/enroll.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/cli/cmds/lock.py` & `sortinghat-0.9.3/sortinghat/cli/cmds/lock.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/cli/cmds/merge.py` & `sortinghat-0.9.3/sortinghat/cli/cmds/merge.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/cli/cmds/mv.py` & `sortinghat-0.9.3/sortinghat/cli/cmds/mv.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/cli/cmds/orgs.py` & `sortinghat-0.9.3/sortinghat/cli/cmds/orgs.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/cli/cmds/profile.py` & `sortinghat-0.9.3/sortinghat/cli/cmds/profile.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/cli/cmds/rm.py` & `sortinghat-0.9.3/sortinghat/cli/cmds/rm.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/cli/cmds/show.py` & `sortinghat-0.9.3/sortinghat/cli/cmds/show.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/cli/cmds/split.py` & `sortinghat-0.9.3/sortinghat/cli/cmds/split.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/cli/cmds/withdraw.py` & `sortinghat-0.9.3/sortinghat/cli/cmds/withdraw.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/cli/sortinghat.py` & `sortinghat-0.9.3/sortinghat/cli/sortinghat.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/cli/templates/show.tmpl` & `sortinghat-0.9.3/sortinghat/cli/templates/show.tmpl`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/cli/utils.py` & `sortinghat-0.9.3/sortinghat/cli/utils.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/config/settings.py` & `sortinghat-0.9.3/sortinghat/config/settings.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/admin.py` & `sortinghat-0.9.3/sortinghat/core/admin.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/api.py` & `sortinghat-0.9.3/sortinghat/core/api.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/apps.py` & `sortinghat-0.9.3/sortinghat/core/apps.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/aux.py` & `sortinghat-0.9.3/sortinghat/core/aux.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/context.py` & `sortinghat-0.9.3/sortinghat/core/context.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/db.py` & `sortinghat-0.9.3/sortinghat/core/db.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/decorators.py` & `sortinghat-0.9.3/sortinghat/core/decorators.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 from django.http import HttpResponse
 from graphql_jwt.decorators import user_passes_test
 from graphql_jwt.utils import get_credentials
 from graphql_jwt.shortcuts import get_user_by_token
 from graphql_jwt.exceptions import JSONWebTokenError
 
 from . import tenant
+from .errors import InvalidValueError
 
 # This custom decorator takes the `user` object from the request's
 # context and checks the value of the `is_authenticated` variable
 # and the `AUTHENTICATION_REQUIRED` variable from the config settings.
 check_auth = user_passes_test(
     lambda u: u.is_authenticated or not settings.SORTINGHAT_AUTHENTICATION_REQUIRED
 )
@@ -76,14 +77,19 @@
     return using_tenant
 
 
 def job_using_tenant(func):
     """Use the tenant provided in the context argument for the job"""
     @wraps(func)
     def using_tenant(*args, **kwargs):
-        ctx = kwargs.get('ctx', args[0])
+        ctx = kwargs.get('ctx', None)
+        if not ctx and args:
+            ctx = args[0]
+        if not ctx:
+            raise InvalidValueError(msg="Context not provided to the Job")
+
         tenant.set_db_tenant(ctx.tenant)
         try:
             return func(*args, **kwargs)
         finally:
             tenant.unset_db_tenant()
     return using_tenant
```

### Comparing `sortinghat-0.9.2/sortinghat/core/errors.py` & `sortinghat-0.9.3/sortinghat/core/errors.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/fixtures/countries.json` & `sortinghat-0.9.3/sortinghat/core/fixtures/countries.json`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/importer/backend.py` & `sortinghat-0.9.3/sortinghat/core/importer/backend.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/importer/backends/mailmap.py` & `sortinghat-0.9.3/sortinghat/core/importer/backends/mailmap.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/importer/base.py` & `sortinghat-0.9.3/sortinghat/core/importer/base.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/importer/models.py` & `sortinghat-0.9.3/sortinghat/core/importer/models.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/importer/utils.py` & `sortinghat-0.9.3/sortinghat/core/importer/utils.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/jobs.py` & `sortinghat-0.9.3/sortinghat/core/jobs.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/log.py` & `sortinghat-0.9.3/sortinghat/core/log.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/management/commands/create_groups.py` & `sortinghat-0.9.3/sortinghat/core/management/commands/create_groups.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/middleware.py` & `sortinghat-0.9.3/sortinghat/core/middleware.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/migrations/0001_sortinghat.py` & `sortinghat-0.9.3/sortinghat/core/migrations/0001_sortinghat.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/migrations/0002_importidentitiestask.py` & `sortinghat-0.9.3/sortinghat/core/migrations/0002_importidentitiestask.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/migrations/0003_multi_tenancy.py` & `sortinghat-0.9.3/sortinghat/core/migrations/0003_multi_tenancy.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/models.py` & `sortinghat-0.9.3/sortinghat/core/models.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/recommendations/__init__.py` & `sortinghat-0.9.3/sortinghat/core/recommendations/__init__.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/recommendations/affiliation.py` & `sortinghat-0.9.3/sortinghat/core/recommendations/affiliation.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/recommendations/engine.py` & `sortinghat-0.9.3/sortinghat/core/recommendations/engine.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/recommendations/exclusion.py` & `sortinghat-0.9.3/sortinghat/core/recommendations/exclusion.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/recommendations/gender.py` & `sortinghat-0.9.3/sortinghat/core/recommendations/gender.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/recommendations/matching.py` & `sortinghat-0.9.3/sortinghat/core/recommendations/matching.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/schema.py` & `sortinghat-0.9.3/sortinghat/core/schema.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/static/css/366.d54629c5.css` & `sortinghat-0.9.3/sortinghat/core/static/css/366.d54629c5.css`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/static/css/5.5bd7783b.css` & `sortinghat-0.9.3/sortinghat/core/static/css/5.5bd7783b.css`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/static/css/56.d54629c5.css` & `sortinghat-0.9.3/sortinghat/core/static/css/56.d54629c5.css`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/static/css/561.91f3ebe2.css` & `sortinghat-0.9.3/sortinghat/core/static/css/561.91f3ebe2.css`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/static/css/574.5889fc28.css` & `sortinghat-0.9.3/sortinghat/core/static/css/574.5889fc28.css`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/static/css/762.6b2ccfca.css` & `sortinghat-0.9.3/sortinghat/core/static/css/762.6b2ccfca.css`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/static/css/841.73b7a8e2.css` & `sortinghat-0.9.3/sortinghat/core/static/css/841.73b7a8e2.css`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/static/css/894.f7e21c66.css` & `sortinghat-0.9.3/sortinghat/core/static/css/894.f7e21c66.css`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/static/css/981.cb0d0293.css` & `sortinghat-0.9.3/sortinghat/core/static/css/981.cb0d0293.css`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/static/css/987.a5ced4b6.css` & `sortinghat-0.9.3/sortinghat/core/static/css/987.a5ced4b6.css`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/static/css/app.28a862de.css` & `sortinghat-0.9.3/sortinghat/core/static/css/app.28a862de.css`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/static/css/chunk-vendors.7dc1bb68.css` & `sortinghat-0.9.3/sortinghat/core/static/css/chunk-vendors.7dc1bb68.css`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/static/favicon-grimoirelab.ico` & `sortinghat-0.9.3/sortinghat/core/static/favicon-grimoirelab.ico`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/static/fonts/Roboto-Italic.6a5b2eb0.woff2` & `sortinghat-0.9.3/sortinghat/core/static/fonts/Roboto-Italic.6a5b2eb0.woff2`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/static/fonts/Roboto-Italic.76b8308b.woff` & `sortinghat-0.9.3/sortinghat/core/static/fonts/Roboto-Italic.76b8308b.woff`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/static/fonts/Roboto-Italic.991def81.ttf` & `sortinghat-0.9.3/sortinghat/core/static/fonts/Roboto-Italic.991def81.ttf`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/static/fonts/Roboto-Light.2d3c72a3.woff` & `sortinghat-0.9.3/sortinghat/core/static/fonts/Roboto-Light.2d3c72a3.woff`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/static/fonts/Roboto-Light.41cb61ed.woff2` & `sortinghat-0.9.3/sortinghat/core/static/fonts/Roboto-Light.41cb61ed.woff2`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/static/fonts/Roboto-Light.f2e7274e.ttf` & `sortinghat-0.9.3/sortinghat/core/static/fonts/Roboto-Light.f2e7274e.ttf`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/static/fonts/Roboto-LightItalic.07369d23.woff2` & `sortinghat-0.9.3/sortinghat/core/static/fonts/Roboto-LightItalic.07369d23.woff2`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/static/fonts/Roboto-LightItalic.45582c0c.woff` & `sortinghat-0.9.3/sortinghat/core/static/fonts/Roboto-LightItalic.45582c0c.woff`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/static/fonts/Roboto-LightItalic.b694f0fe.ttf` & `sortinghat-0.9.3/sortinghat/core/static/fonts/Roboto-LightItalic.b694f0fe.ttf`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/static/fonts/Roboto-Medium.13e0be98.woff2` & `sortinghat-0.9.3/sortinghat/core/static/fonts/Roboto-Medium.13e0be98.woff2`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/static/fonts/Roboto-Medium.483a3bd1.woff` & `sortinghat-0.9.3/sortinghat/core/static/fonts/Roboto-Medium.483a3bd1.woff`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/static/fonts/Roboto-Medium.af9d0139.ttf` & `sortinghat-0.9.3/sortinghat/core/static/fonts/Roboto-Medium.af9d0139.ttf`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/static/fonts/Roboto-MediumItalic.3723a2e7.ttf` & `sortinghat-0.9.3/sortinghat/core/static/fonts/Roboto-MediumItalic.3723a2e7.ttf`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/static/fonts/Roboto-MediumItalic.8b19cc18.woff` & `sortinghat-0.9.3/sortinghat/core/static/fonts/Roboto-MediumItalic.8b19cc18.woff`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/static/fonts/Roboto-MediumItalic.b35d3641.woff2` & `sortinghat-0.9.3/sortinghat/core/static/fonts/Roboto-MediumItalic.b35d3641.woff2`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/static/fonts/Roboto-Regular.36d4503d.woff` & `sortinghat-0.9.3/sortinghat/core/static/fonts/Roboto-Regular.36d4503d.woff`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/static/fonts/Roboto-Regular.ae3a8db9.ttf` & `sortinghat-0.9.3/sortinghat/core/static/fonts/Roboto-Regular.ae3a8db9.ttf`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/static/fonts/Roboto-Regular.e0553e00.woff2` & `sortinghat-0.9.3/sortinghat/core/static/fonts/Roboto-Regular.e0553e00.woff2`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/static/fonts/materialdesignicons-webfont.67f3950a.ttf` & `sortinghat-0.9.3/sortinghat/core/static/fonts/materialdesignicons-webfont.67f3950a.ttf`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/static/fonts/materialdesignicons-webfont.83bc1470.woff` & `sortinghat-0.9.3/sortinghat/core/static/fonts/materialdesignicons-webfont.83bc1470.woff`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/static/fonts/materialdesignicons-webfont.d819e534.woff2` & `sortinghat-0.9.3/sortinghat/core/static/fonts/materialdesignicons-webfont.d819e534.woff2`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/static/fonts/materialdesignicons-webfont.fbaf9d97.eot` & `sortinghat-0.9.3/sortinghat/core/static/fonts/materialdesignicons-webfont.fbaf9d97.eot`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/static/js/366.db9f9acd.js` & `sortinghat-0.9.3/sortinghat/core/static/js/366.db9f9acd.js`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/static/js/5.8197bd56.js` & `sortinghat-0.9.3/sortinghat/core/static/js/5.8197bd56.js`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/static/js/56.66e710bd.js` & `sortinghat-0.9.3/sortinghat/core/static/js/56.66e710bd.js`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/static/js/561.5943719e.js` & `sortinghat-0.9.3/sortinghat/core/static/js/561.5943719e.js`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/static/js/574.bfb992b9.js` & `sortinghat-0.9.3/sortinghat/core/static/js/574.bfb992b9.js`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/static/js/762.2ca33633.js` & `sortinghat-0.9.3/sortinghat/core/static/js/762.2ca33633.js`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/static/js/841.db6bdce9.js` & `sortinghat-0.9.3/sortinghat/core/static/js/841.db6bdce9.js`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/static/js/894.1119152d.js` & `sortinghat-0.9.3/sortinghat/core/static/js/894.1119152d.js`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/static/js/966.7c5c17a8.js` & `sortinghat-0.9.3/sortinghat/core/static/js/966.7c5c17a8.js`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/static/js/981.ba53d6b4.js` & `sortinghat-0.9.3/sortinghat/core/static/js/981.ba53d6b4.js`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/static/js/987.8a763c50.js` & `sortinghat-0.9.3/sortinghat/core/static/js/987.8a763c50.js`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/static/js/993.cda825ec.js` & `sortinghat-0.9.3/sortinghat/core/static/js/993.cda825ec.js`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/static/js/app.2b031f67.js` & `sortinghat-0.9.3/sortinghat/core/static/js/app.2b031f67.js`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/static/js/chunk-vendors.26a9eb41.js` & `sortinghat-0.9.3/sortinghat/core/static/js/chunk-vendors.26a9eb41.js`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/templates/index.html` & `sortinghat-0.9.3/sortinghat/core/templates/index.html`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/tenant.py` & `sortinghat-0.9.3/sortinghat/core/tenant.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/core/views.py` & `sortinghat-0.9.3/sortinghat/core/views.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/server/sortinghat_admin.py` & `sortinghat-0.9.3/sortinghat/server/sortinghat_admin.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/server/sortinghatd.py` & `sortinghat-0.9.3/sortinghat/server/sortinghatd.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/server/sortinghatw.py` & `sortinghat-0.9.3/sortinghat/server/sortinghatw.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/server/utils/create_sh_0_7_fixture.py` & `sortinghat-0.9.3/sortinghat/server/utils/create_sh_0_7_fixture.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/sortinghat/utils/__init__.py` & `sortinghat-0.9.3/sortinghat/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/tests/cli/test_cmd_add.py` & `sortinghat-0.9.3/tests/cli/test_cmd_add.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/tests/cli/test_cmd_config.py` & `sortinghat-0.9.3/tests/cli/test_cmd_config.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/tests/cli/test_cmd_countries.py` & `sortinghat-0.9.3/tests/cli/test_cmd_countries.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/tests/cli/test_cmd_enroll.py` & `sortinghat-0.9.3/tests/cli/test_cmd_enroll.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/tests/cli/test_cmd_lock.py` & `sortinghat-0.9.3/tests/cli/test_cmd_lock.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/tests/cli/test_cmd_merge.py` & `sortinghat-0.9.3/tests/cli/test_cmd_merge.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/tests/cli/test_cmd_mv.py` & `sortinghat-0.9.3/tests/cli/test_cmd_mv.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/tests/cli/test_cmd_orgs.py` & `sortinghat-0.9.3/tests/cli/test_cmd_orgs.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/tests/cli/test_cmd_profile.py` & `sortinghat-0.9.3/tests/cli/test_cmd_profile.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/tests/cli/test_cmd_rm.py` & `sortinghat-0.9.3/tests/cli/test_cmd_rm.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/tests/cli/test_cmd_show.py` & `sortinghat-0.9.3/tests/cli/test_cmd_show.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/tests/cli/test_cmd_split.py` & `sortinghat-0.9.3/tests/cli/test_cmd_split.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/tests/cli/test_cmd_withdraw.py` & `sortinghat-0.9.3/tests/cli/test_cmd_withdraw.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/tests/importer/mocked_package/backend_a.py` & `sortinghat-0.9.3/tests/importer/mocked_package/backend_a.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/tests/importer/mocked_package/nested_package/nested_backend_b.py` & `sortinghat-0.9.3/tests/importer/mocked_package/nested_package/nested_backend_b.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/tests/importer/mocked_package/nested_package/nested_backend_c.py` & `sortinghat-0.9.3/tests/importer/mocked_package/nested_package/nested_backend_c.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/tests/importer/mocked_package/nested_package/nested_not_backend.py` & `sortinghat-0.9.3/tests/importer/mocked_package/nested_package/nested_not_backend.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/tests/importer/test_backend.py` & `sortinghat-0.9.3/tests/importer/test_backend.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/tests/importer/test_utils.py` & `sortinghat-0.9.3/tests/importer/test_utils.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/tests/rec/test_affiliations.py` & `sortinghat-0.9.3/tests/rec/test_affiliations.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/tests/rec/test_engine.py` & `sortinghat-0.9.3/tests/rec/test_engine.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/tests/rec/test_exclusion.py` & `sortinghat-0.9.3/tests/rec/test_exclusion.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/tests/rec/test_gender.py` & `sortinghat-0.9.3/tests/rec/test_gender.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/tests/rec/test_matches.py` & `sortinghat-0.9.3/tests/rec/test_matches.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/tests/runners.py` & `sortinghat-0.9.3/tests/runners.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/tests/tenants/test_jobs.py` & `sortinghat-0.9.3/tests/tenants/test_jobs.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/tests/tenants/test_middleware.py` & `sortinghat-0.9.3/tests/tenants/test_middleware.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/tests/tenants/test_schema.py` & `sortinghat-0.9.3/tests/tenants/test_schema.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/tests/test_api.py` & `sortinghat-0.9.3/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/tests/test_aux.py` & `sortinghat-0.9.3/tests/test_aux.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/tests/test_client.py` & `sortinghat-0.9.3/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/tests/test_db.py` & `sortinghat-0.9.3/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/tests/test_errors.py` & `sortinghat-0.9.3/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/tests/test_jobs.py` & `sortinghat-0.9.3/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/tests/test_log.py` & `sortinghat-0.9.3/tests/test_log.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/tests/test_model.py` & `sortinghat-0.9.3/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/tests/test_schema.py` & `sortinghat-0.9.3/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/tests/test_utils.py` & `sortinghat-0.9.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `sortinghat-0.9.2/PKG-INFO` & `sortinghat-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sortinghat
-Version: 0.9.2
+Version: 0.9.3
 Summary: A tool to manage identities.
 Home-page: https://chaoss.github.io/grimoirelab/
 License: GPL-3.0+
 Keywords: development,grimoirelab
 Author: GrimoireLab Developers
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: Development Status :: 4 - Beta
```

