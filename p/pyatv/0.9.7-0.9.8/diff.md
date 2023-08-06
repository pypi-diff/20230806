# Comparing `tmp/pyatv-0.9.7.tar.gz` & `tmp/pyatv-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyatv-0.9.7.tar", last modified: Mon Dec  6 08:00:11 2021, max compression
+gzip compressed data, was "dist/pyatv-0.9.8.tar", last modified: Wed Dec 15 18:56:39 2021, max compression
```

## Comparing `pyatv-0.9.7.tar` & `pyatv-0.9.8.tar`

### file list

```diff
@@ -1,528 +1,531 @@
-drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-06 08:00:11.347011 pyatv-0.9.7/
--rw-r--r--   0 postlund  (1000) postlund  (1000)    74612 2021-12-06 07:58:28.000000 pyatv-0.9.7/CHANGES.md
--rw-r--r--   0 postlund  (1000) postlund  (1000)       90 2021-09-10 16:43:01.000000 pyatv-0.9.7/CONTRIBUTORS.md
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1081 2021-09-10 16:43:01.000000 pyatv-0.9.7/LICENSE.md
--rw-r--r--   0 postlund  (1000) postlund  (1000)      276 2021-09-10 16:43:01.000000 pyatv-0.9.7/MANIFEST.in
--rw-r--r--   0 postlund  (1000) postlund  (1000)     4651 2021-12-06 08:00:11.347011 pyatv-0.9.7/PKG-INFO
--rw-r--r--   0 postlund  (1000) postlund  (1000)     3523 2021-10-25 17:59:14.000000 pyatv-0.9.7/README.md
--rw-r--r--   0 postlund  (1000) postlund  (1000)      156 2021-10-20 08:10:37.000000 pyatv-0.9.7/base_versions.txt
-drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-06 08:00:11.279010 pyatv-0.9.7/docs/
--rw-r--r--   0 postlund  (1000) postlund  (1000)      399 2019-11-15 09:37:48.000000 pyatv-0.9.7/docs/404.html
--rw-r--r--   0 postlund  (1000) postlund  (1000)        9 2021-09-10 16:43:01.000000 pyatv-0.9.7/docs/CNAME
--rw-r--r--   0 postlund  (1000) postlund  (1000)      991 2019-11-15 09:37:48.000000 pyatv-0.9.7/docs/Gemfile
--rw-r--r--   0 postlund  (1000) postlund  (1000)     7953 2021-12-04 20:39:30.000000 pyatv-0.9.7/docs/Gemfile.lock
--rw-r--r--   0 postlund  (1000) postlund  (1000)     2920 2021-09-10 16:43:01.000000 pyatv-0.9.7/docs/_config.yml
-drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-06 08:00:11.283010 pyatv-0.9.7/docs/_includes/
--rw-r--r--   0 postlund  (1000) postlund  (1000)      399 2021-09-10 16:43:01.000000 pyatv-0.9.7/docs/_includes/api
--rw-r--r--   0 postlund  (1000) postlund  (1000)      244 2021-09-10 16:43:01.000000 pyatv-0.9.7/docs/_includes/code
--rw-r--r--   0 postlund  (1000) postlund  (1000)      423 2021-09-10 16:43:01.000000 pyatv-0.9.7/docs/_includes/issue
--rw-r--r--   0 postlund  (1000) postlund  (1000)      160 2021-09-10 16:43:01.000000 pyatv-0.9.7/docs/_includes/pypi
-drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-06 08:00:11.283010 pyatv-0.9.7/docs/_layouts/
--rw-r--r--   0 postlund  (1000) postlund  (1000)     4758 2021-09-10 16:43:01.000000 pyatv-0.9.7/docs/_layouts/template.html
-drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-06 08:00:11.283010 pyatv-0.9.7/docs/api/
-drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-06 08:00:11.283010 pyatv-0.9.7/docs/api/pyatv/
--rw-r--r--   0 postlund  (1000) postlund  (1000)    19304 2021-12-06 08:00:09.000000 pyatv-0.9.7/docs/api/pyatv/conf.html
--rw-r--r--   0 postlund  (1000) postlund  (1000)    40437 2021-12-06 08:00:09.000000 pyatv-0.9.7/docs/api/pyatv/const.html
--rw-r--r--   0 postlund  (1000) postlund  (1000)     4610 2021-12-06 08:00:09.000000 pyatv-0.9.7/docs/api/pyatv/convert.html
--rw-r--r--   0 postlund  (1000) postlund  (1000)     3168 2021-09-29 20:18:54.000000 pyatv-0.9.7/docs/api/pyatv/core.html
--rw-r--r--   0 postlund  (1000) postlund  (1000)    16760 2021-12-06 08:00:09.000000 pyatv-0.9.7/docs/api/pyatv/exceptions.html
--rw-r--r--   0 postlund  (1000) postlund  (1000)     3785 2021-12-06 08:00:09.000000 pyatv-0.9.7/docs/api/pyatv/helpers.html
--rw-r--r--   0 postlund  (1000) postlund  (1000)   107961 2021-12-06 08:00:10.000000 pyatv-0.9.7/docs/api/pyatv/interface.html
--rw-r--r--   0 postlund  (1000) postlund  (1000)     5076 2021-12-06 08:00:09.000000 pyatv-0.9.7/docs/api/pyatv.html
-drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-06 08:00:11.275010 pyatv-0.9.7/docs/assets/
-drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-06 08:00:11.283010 pyatv-0.9.7/docs/assets/css/
--rw-r--r--   0 postlund  (1000) postlund  (1000)      296 2021-09-10 16:43:01.000000 pyatv-0.9.7/docs/assets/css/custom.css
--rw-r--r--   0 postlund  (1000) postlund  (1000)      872 2021-09-10 16:43:01.000000 pyatv-0.9.7/docs/assets/css/hljs.css
--rw-r--r--   0 postlund  (1000) postlund  (1000)     6138 2021-09-10 16:43:01.000000 pyatv-0.9.7/docs/assets/css/normalize.css
--rw-r--r--   0 postlund  (1000) postlund  (1000)     3861 2021-09-10 16:43:01.000000 pyatv-0.9.7/docs/assets/css/pdoc.css
--rw-r--r--   0 postlund  (1000) postlund  (1000)     9527 2021-09-10 16:43:01.000000 pyatv-0.9.7/docs/assets/css/sanitize.css
--rw-r--r--   0 postlund  (1000) postlund  (1000)      147 2021-09-10 16:43:01.000000 pyatv-0.9.7/docs/assets/css/style.scss
-drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-06 08:00:11.283010 pyatv-0.9.7/docs/assets/img/
--rw-r--r--   0 postlund  (1000) postlund  (1000)     3024 2021-09-10 16:43:01.000000 pyatv-0.9.7/docs/assets/img/logo.svg
-drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-06 08:00:11.291010 pyatv-0.9.7/docs/assets/js/
--rw-r--r--   0 postlund  (1000) postlund  (1000)    46003 2021-09-10 16:43:01.000000 pyatv-0.9.7/docs/assets/js/highlight.9.12.0.min.js
--rw-r--r--   0 postlund  (1000) postlund  (1000)   873682 2021-09-10 16:43:01.000000 pyatv-0.9.7/docs/assets/js/mermaid.8.9.2.min.js
--rw-r--r--   0 postlund  (1000) postlund  (1000)  3255902 2021-09-10 16:43:01.000000 pyatv-0.9.7/docs/assets/js/mermaid.min.js.map
-drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-06 08:00:11.295010 pyatv-0.9.7/docs/development/
--rw-r--r--   0 postlund  (1000) postlund  (1000)      832 2021-09-10 16:43:01.000000 pyatv-0.9.7/docs/development/apps.md
--rw-r--r--   0 postlund  (1000) postlund  (1000)      780 2021-09-10 16:43:01.000000 pyatv-0.9.7/docs/development/audio.md
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1302 2021-09-10 16:43:01.000000 pyatv-0.9.7/docs/development/control.md
--rw-r--r--   0 postlund  (1000) postlund  (1000)      468 2021-09-10 16:43:01.000000 pyatv-0.9.7/docs/development/development.md
--rw-r--r--   0 postlund  (1000) postlund  (1000)      917 2021-09-10 16:43:01.000000 pyatv-0.9.7/docs/development/device_info.md
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1679 2021-11-01 07:00:26.000000 pyatv-0.9.7/docs/development/examples.md
--rw-r--r--   0 postlund  (1000) postlund  (1000)     3080 2021-09-10 16:43:01.000000 pyatv-0.9.7/docs/development/features.md
--rw-r--r--   0 postlund  (1000) postlund  (1000)     3011 2021-09-10 16:43:01.000000 pyatv-0.9.7/docs/development/listeners.md
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1581 2021-09-10 16:43:01.000000 pyatv-0.9.7/docs/development/logging.md
--rw-r--r--   0 postlund  (1000) postlund  (1000)     3697 2021-09-10 16:43:01.000000 pyatv-0.9.7/docs/development/metadata.md
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1336 2021-09-10 16:43:01.000000 pyatv-0.9.7/docs/development/power_management.md
--rw-r--r--   0 postlund  (1000) postlund  (1000)    10685 2021-12-05 20:49:29.000000 pyatv-0.9.7/docs/development/scan_pair_and_connect.md
--rw-r--r--   0 postlund  (1000) postlund  (1000)      182 2019-11-15 09:37:48.000000 pyatv-0.9.7/docs/development/services.md
--rw-r--r--   0 postlund  (1000) postlund  (1000)     6851 2021-12-05 20:49:29.000000 pyatv-0.9.7/docs/development/stream.md
--rw-r--r--   0 postlund  (1000) postlund  (1000)      180 2019-11-15 09:37:48.000000 pyatv-0.9.7/docs/development/testing.md
-drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-06 08:00:11.295010 pyatv-0.9.7/docs/documentation/
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1326 2021-09-10 16:43:01.000000 pyatv-0.9.7/docs/documentation/atvlog.md
--rw-r--r--   0 postlund  (1000) postlund  (1000)     6417 2021-09-10 16:43:01.000000 pyatv-0.9.7/docs/documentation/atvproxy.md
--rw-r--r--   0 postlund  (1000) postlund  (1000)    11116 2021-10-08 10:29:18.000000 pyatv-0.9.7/docs/documentation/atvremote.md
--rw-r--r--   0 postlund  (1000) postlund  (1000)     6835 2021-09-10 16:43:01.000000 pyatv-0.9.7/docs/documentation/atvscript.md
--rw-r--r--   0 postlund  (1000) postlund  (1000)    11265 2021-10-08 10:26:03.000000 pyatv-0.9.7/docs/documentation/concepts.md
--rw-r--r--   0 postlund  (1000) postlund  (1000)     4012 2021-10-25 17:59:14.000000 pyatv-0.9.7/docs/documentation/documentation.md
--rw-r--r--   0 postlund  (1000) postlund  (1000)     4534 2021-09-10 16:43:01.000000 pyatv-0.9.7/docs/documentation/getting_started.md
--rw-r--r--   0 postlund  (1000) postlund  (1000)    78769 2021-12-05 20:49:29.000000 pyatv-0.9.7/docs/documentation/protocols.md
--rw-r--r--   0 postlund  (1000) postlund  (1000)    13650 2021-12-06 07:52:37.000000 pyatv-0.9.7/docs/documentation/supported_features.md
--rw-r--r--   0 postlund  (1000) postlund  (1000)    34262 2021-10-08 10:29:18.000000 pyatv-0.9.7/docs/documentation/tutorial.md
--rw-r--r--   0 postlund  (1000) postlund  (1000)       47 2021-09-10 16:43:01.000000 pyatv-0.9.7/docs/documentation/workspace.code-workspace
--rw-r--r--   0 postlund  (1000) postlund  (1000)   186268 2021-09-10 16:43:01.000000 pyatv-0.9.7/docs/favicon.ico
--rw-r--r--   0 postlund  (1000) postlund  (1000)     5806 2021-10-08 10:26:03.000000 pyatv-0.9.7/docs/index.md
-drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-06 08:00:11.299011 pyatv-0.9.7/docs/internals/
--rw-r--r--   0 postlund  (1000) postlund  (1000)    13784 2021-10-08 10:26:03.000000 pyatv-0.9.7/docs/internals/design.md
--rw-r--r--   0 postlund  (1000) postlund  (1000)     4562 2021-10-25 17:59:14.000000 pyatv-0.9.7/docs/internals/documentation.md
--rw-r--r--   0 postlund  (1000) postlund  (1000)     4352 2021-09-10 16:43:01.000000 pyatv-0.9.7/docs/internals/interfaces.md
--rw-r--r--   0 postlund  (1000) postlund  (1000)     5419 2021-10-25 17:59:14.000000 pyatv-0.9.7/docs/internals/internals.md
--rw-r--r--   0 postlund  (1000) postlund  (1000)     2449 2021-10-25 17:59:14.000000 pyatv-0.9.7/docs/internals/submit_pr.md
--rw-r--r--   0 postlund  (1000) postlund  (1000)    10489 2021-09-10 16:43:01.000000 pyatv-0.9.7/docs/internals/testing.md
--rw-r--r--   0 postlund  (1000) postlund  (1000)    20281 2021-12-05 20:49:29.000000 pyatv-0.9.7/docs/internals/tools.md
-drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-06 08:00:11.299011 pyatv-0.9.7/docs/pdoc_templates/
--rw-r--r--   0 postlund  (1000) postlund  (1000)     2095 2021-09-10 16:43:01.000000 pyatv-0.9.7/docs/pdoc_templates/config.mako
--rw-r--r--   0 postlund  (1000) postlund  (1000)    12068 2021-09-10 16:43:01.000000 pyatv-0.9.7/docs/pdoc_templates/html.mako
-drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-06 08:00:11.299011 pyatv-0.9.7/docs/support/
--rw-r--r--   0 postlund  (1000) postlund  (1000)     2680 2021-09-10 16:43:01.000000 pyatv-0.9.7/docs/support/acknowledgements.md
--rw-r--r--   0 postlund  (1000) postlund  (1000)     9777 2021-09-29 20:18:54.000000 pyatv-0.9.7/docs/support/faq.md
--rw-r--r--   0 postlund  (1000) postlund  (1000)     5144 2021-12-06 07:55:59.000000 pyatv-0.9.7/docs/support/migration.md
--rw-r--r--   0 postlund  (1000) postlund  (1000)     4944 2021-09-10 16:43:01.000000 pyatv-0.9.7/docs/support/scanning_issues.md
--rw-r--r--   0 postlund  (1000) postlund  (1000)      707 2021-09-10 16:43:01.000000 pyatv-0.9.7/docs/support/support.md
--rw-r--r--   0 postlund  (1000) postlund  (1000)     2338 2021-09-10 16:43:01.000000 pyatv-0.9.7/docs/support/troubleshooting.md
-drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-06 08:00:11.299011 pyatv-0.9.7/examples/
--rw-r--r--   0 postlund  (1000) postlund  (1000)       35 2019-10-30 11:09:35.000000 pyatv-0.9.7/examples/__init__.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)      447 2021-09-10 16:43:01.000000 pyatv-0.9.7/examples/auto_connect.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1588 2021-11-01 07:00:26.000000 pyatv-0.9.7/examples/connect_with_credentials.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)      937 2021-10-08 10:29:18.000000 pyatv-0.9.7/examples/manual_connect.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)      976 2021-09-10 16:43:01.000000 pyatv-0.9.7/examples/pairing.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)      973 2021-09-10 16:43:01.000000 pyatv-0.9.7/examples/play_url.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)      867 2021-10-28 20:26:32.000000 pyatv-0.9.7/examples/scan_and_connect.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1501 2021-09-21 11:06:52.000000 pyatv-0.9.7/examples/stream.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     6272 2021-09-10 16:43:01.000000 pyatv-0.9.7/examples/tutorial.py
-drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-06 08:00:11.299011 pyatv-0.9.7/pyatv/
--rw-r--r--   0 postlund  (1000) postlund  (1000)     4056 2021-12-05 20:49:29.000000 pyatv-0.9.7/pyatv/__init__.py
-drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-06 08:00:11.303011 pyatv-0.9.7/pyatv/auth/
--rw-r--r--   0 postlund  (1000) postlund  (1000)     3186 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/auth/hap_channel.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     4288 2021-09-29 20:18:54.000000 pyatv-0.9.7/pyatv/auth/hap_pairing.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     2164 2021-09-29 20:18:54.000000 pyatv-0.9.7/pyatv/auth/hap_session.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     7738 2021-12-02 20:27:15.000000 pyatv-0.9.7/pyatv/auth/hap_srp.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     3980 2021-09-29 20:18:54.000000 pyatv-0.9.7/pyatv/auth/hap_tlv8.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     7212 2021-12-05 20:49:29.000000 pyatv-0.9.7/pyatv/conf.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     7333 2021-12-05 21:05:33.000000 pyatv-0.9.7/pyatv/const.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     2314 2021-10-08 10:29:18.000000 pyatv-0.9.7/pyatv/convert.py
-drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-06 08:00:11.303011 pyatv-0.9.7/pyatv/core/
--rw-r--r--   0 postlund  (1000) postlund  (1000)     2568 2021-12-05 20:49:29.000000 pyatv-0.9.7/pyatv/core/__init__.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)    22280 2021-11-01 07:00:26.000000 pyatv-0.9.7/pyatv/core/facade.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)    18555 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/core/mdns.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     3334 2021-11-01 07:00:26.000000 pyatv-0.9.7/pyatv/core/protocol.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     4422 2021-10-20 08:10:37.000000 pyatv-0.9.7/pyatv/core/relayer.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     9888 2021-10-08 10:29:18.000000 pyatv-0.9.7/pyatv/core/scan.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     2743 2021-10-20 08:10:37.000000 pyatv-0.9.7/pyatv/exceptions.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     3005 2021-12-04 17:12:29.000000 pyatv-0.9.7/pyatv/helpers.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)    39469 2021-12-05 20:49:29.000000 pyatv-0.9.7/pyatv/interface.py
-drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-06 08:00:11.303011 pyatv-0.9.7/pyatv/protocols/
--rw-r--r--   0 postlund  (1000) postlund  (1000)     2406 2021-10-20 08:10:37.000000 pyatv-0.9.7/pyatv/protocols/__init__.py
-drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-06 08:00:11.303011 pyatv-0.9.7/pyatv/protocols/airplay/
--rw-r--r--   0 postlund  (1000) postlund  (1000)    10273 2021-12-05 20:49:29.000000 pyatv-0.9.7/pyatv/protocols/airplay/__init__.py
-drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-06 08:00:11.303011 pyatv-0.9.7/pyatv/protocols/airplay/auth/
--rw-r--r--   0 postlund  (1000) postlund  (1000)     4411 2021-11-04 07:35:14.000000 pyatv-0.9.7/pyatv/protocols/airplay/auth/__init__.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     4607 2021-12-02 20:27:15.000000 pyatv-0.9.7/pyatv/protocols/airplay/auth/hap.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     3012 2021-10-20 11:55:10.000000 pyatv-0.9.7/pyatv/protocols/airplay/auth/hap_transient.py
--rwxr-xr-x   0 postlund  (1000) postlund  (1000)     3877 2021-11-04 07:35:14.000000 pyatv-0.9.7/pyatv/protocols/airplay/auth/legacy.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     5607 2021-11-26 08:48:44.000000 pyatv-0.9.7/pyatv/protocols/airplay/channels.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     2756 2021-11-04 07:35:14.000000 pyatv-0.9.7/pyatv/protocols/airplay/mrp_connection.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     3274 2021-10-20 11:48:25.000000 pyatv-0.9.7/pyatv/protocols/airplay/pairing.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     3163 2021-11-04 07:35:14.000000 pyatv-0.9.7/pyatv/protocols/airplay/player.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     6432 2021-11-04 07:35:14.000000 pyatv-0.9.7/pyatv/protocols/airplay/remote_control.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)    11558 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/airplay/server_auth.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     7323 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/airplay/srp.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     4799 2021-10-08 10:29:18.000000 pyatv-0.9.7/pyatv/protocols/airplay/utils.py
-drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-06 08:00:11.307011 pyatv-0.9.7/pyatv/protocols/companion/
--rw-r--r--   0 postlund  (1000) postlund  (1000)    14081 2021-11-01 07:00:26.000000 pyatv-0.9.7/pyatv/protocols/companion/__init__.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     7965 2021-11-01 07:00:26.000000 pyatv-0.9.7/pyatv/protocols/companion/api.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     5693 2021-11-01 07:00:26.000000 pyatv-0.9.7/pyatv/protocols/companion/auth.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     5110 2021-11-01 07:00:26.000000 pyatv-0.9.7/pyatv/protocols/companion/connection.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     7788 2021-12-05 20:49:29.000000 pyatv-0.9.7/pyatv/protocols/companion/opack.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     2807 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/companion/pairing.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     8166 2021-11-01 07:00:26.000000 pyatv-0.9.7/pyatv/protocols/companion/protocol.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     8368 2021-10-08 10:29:18.000000 pyatv-0.9.7/pyatv/protocols/companion/server_auth.py
-drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-06 08:00:11.307011 pyatv-0.9.7/pyatv/protocols/dmap/
--rw-r--r--   0 postlund  (1000) postlund  (1000)    24754 2021-10-20 08:10:37.000000 pyatv-0.9.7/pyatv/protocols/dmap/__init__.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     6046 2021-10-08 10:29:18.000000 pyatv-0.9.7/pyatv/protocols/dmap/daap.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     5909 2021-10-29 10:55:43.000000 pyatv-0.9.7/pyatv/protocols/dmap/pairing.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     2586 2021-10-08 10:29:18.000000 pyatv-0.9.7/pyatv/protocols/dmap/parser.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     5993 2021-10-20 08:10:37.000000 pyatv-0.9.7/pyatv/protocols/dmap/tag_definitions.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     2521 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/dmap/tags.py
-drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-06 08:00:11.307011 pyatv-0.9.7/pyatv/protocols/mrp/
--rw-r--r--   0 postlund  (1000) postlund  (1000)    34407 2021-12-05 20:49:29.000000 pyatv-0.9.7/pyatv/protocols/mrp/__init__.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     4022 2021-12-02 20:27:15.000000 pyatv-0.9.7/pyatv/protocols/mrp/auth.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     6092 2021-12-02 20:27:15.000000 pyatv-0.9.7/pyatv/protocols/mrp/connection.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     6500 2021-10-20 08:10:17.000000 pyatv-0.9.7/pyatv/protocols/mrp/messages.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     2900 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/pairing.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)    12221 2021-11-01 07:00:26.000000 pyatv-0.9.7/pyatv/protocols/mrp/player_state.py
-drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-06 08:00:11.335011 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/
--rw-r--r--   0 postlund  (1000) postlund  (1000)      190 2019-11-01 04:29:58.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/#GetKeyboardSessionMessage.proto#
--rw-r--r--   0 postlund  (1000) postlund  (1000)      315 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/AudioFadeMessage.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)     4064 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/AudioFadeMessage_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1451 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/AudioFadeMessage_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)      249 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/AudioFadeResponseMessage.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)     3447 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/AudioFadeResponseMessage_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1170 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/AudioFadeResponseMessage_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)       97 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/AudioFormatSettingsMessage.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)     2284 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/AudioFormatSettingsMessage_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)      933 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/AudioFormatSettingsMessage_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)      409 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/ClientUpdatesConfigMessage.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)     5431 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/ClientUpdatesConfigMessage_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     2128 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/ClientUpdatesConfigMessage_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)     3179 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/CommandInfo.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)    37321 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/CommandInfo_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)    15637 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/CommandInfo_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1351 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/CommandOptions.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)    16502 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/CommandOptions_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     8037 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/CommandOptions_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1071 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/Common.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)    18104 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/Common_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     7036 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/Common_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)      913 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/ContentItem.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)     5962 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/ContentItemMetadata.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)    75715 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/ContentItemMetadata_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)    34219 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/ContentItemMetadata_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)    10997 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/ContentItem_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     5359 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/ContentItem_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)      409 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/CryptoPairingMessage.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)     5144 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/CryptoPairingMessage_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1972 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/CryptoPairingMessage_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1946 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/DeviceInfoMessage.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)    21385 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/DeviceInfoMessage_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)    10144 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/DeviceInfoMessage_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)      239 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/GenericMessage.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)     3578 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/GenericMessage_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1213 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/GenericMessage_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)      199 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/GetKeyboardSessionMessage.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)     2904 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/GetKeyboardSessionMessage_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)      734 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/GetKeyboardSessionMessage_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)      238 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/GetRemoteTextInputSessionMessage.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)     3163 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/GetRemoteTextInputSessionMessage_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)      778 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/GetRemoteTextInputSessionMessage_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)      229 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/GetVolumeMessage.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)     3238 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/GetVolumeMessage_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1149 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/GetVolumeMessage_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)      237 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/GetVolumeResultMessage.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)     3364 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/GetVolumeResultMessage_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1122 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/GetVolumeResultMessage_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1806 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/KeyboardMessage.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)    25455 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/KeyboardMessage_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)    10768 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/KeyboardMessage_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)      216 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/LanguageOption.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)     3970 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/LanguageOption_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1692 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/LanguageOption_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)      265 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/NotificationMessage.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)     3741 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/NotificationMessage_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1442 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/NotificationMessage_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)      398 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/NowPlayingClient.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)     5131 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/NowPlayingClient_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     2613 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/NowPlayingClient_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)      765 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/NowPlayingInfo.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)    10541 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/NowPlayingInfo_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     4535 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/NowPlayingInfo_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)      155 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/NowPlayingPlayer.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)     3113 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/NowPlayingPlayer_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1247 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/NowPlayingPlayer_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)      308 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/Origin.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)      273 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/OriginClientPropertiesMessage.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)     3592 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/OriginClientPropertiesMessage_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1255 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/OriginClientPropertiesMessage_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)     4876 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/Origin_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     2104 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/Origin_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)      514 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/PlaybackQueue.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)      174 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/PlaybackQueueCapabilities.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)     3292 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/PlaybackQueueCapabilities_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1380 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/PlaybackQueueCapabilities_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)       85 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/PlaybackQueueContext.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)     2233 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/PlaybackQueueContext_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)      825 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/PlaybackQueueContext_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1011 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/PlaybackQueueRequestMessage.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)    12067 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/PlaybackQueueRequestMessage_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     5234 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/PlaybackQueueRequestMessage_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)     6215 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/PlaybackQueue_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     2795 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/PlaybackQueue_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)      367 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/PlayerClientPropertiesMessage.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)     4466 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/PlayerClientPropertiesMessage_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1604 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/PlayerClientPropertiesMessage_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)      329 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/PlayerPath.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)     4166 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/PlayerPath_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1625 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/PlayerPath_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)     6792 2021-10-20 08:10:17.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/ProtocolMessage.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)    43485 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/ProtocolMessage_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)    22102 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/ProtocolMessage_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)      397 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/RegisterForGameControllerEventsMessage.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)     5494 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/RegisterForGameControllerEventsMessage_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     2238 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/RegisterForGameControllerEventsMessage_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)      356 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/RegisterHIDDeviceMessage.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)     4026 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/RegisterHIDDeviceMessage_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1469 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/RegisterHIDDeviceMessage_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)      302 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/RegisterHIDDeviceResultMessage.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)     4067 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/RegisterHIDDeviceResultMessage_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1410 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/RegisterHIDDeviceResultMessage_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)      373 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/RegisterVoiceInputDeviceMessage.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)     4202 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/RegisterVoiceInputDeviceMessage_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1494 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/RegisterVoiceInputDeviceMessage_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)      321 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/RegisterVoiceInputDeviceResponseMessage.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)     4286 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/RegisterVoiceInputDeviceResponseMessage_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1399 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/RegisterVoiceInputDeviceResponseMessage_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)      299 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/RemoteTextInputMessage.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)     4260 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/RemoteTextInputMessage_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1462 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/RemoteTextInputMessage_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)      301 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/RemoveClientMessage.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)     3721 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/RemoveClientMessage_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1293 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/RemoveClientMessage_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)      244 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/RemoveEndpointsMessage.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)     3374 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/RemoveEndpointsMessage_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1193 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/RemoveEndpointsMessage_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)      295 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/RemoveOutputDevicesMessage.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)     3975 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/RemoveOutputDevicesMessage_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1512 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/RemoveOutputDevicesMessage_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)      293 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/RemovePlayerMessage.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)     3687 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/RemovePlayerMessage_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1291 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/RemovePlayerMessage_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)      302 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SendButtonEventMessage.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)     4254 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SendButtonEventMessage_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1484 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SendButtonEventMessage_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)      476 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SendCommandMessage.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)     5367 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SendCommandMessage_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1938 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SendCommandMessage_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)     2676 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SendCommandResultMessage.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)    28775 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SendCommandResultMessage_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)    13028 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SendCommandResultMessage_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1701 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SendHIDEventMessage.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)     3295 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SendHIDEventMessage_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     2575 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SendHIDEventMessage_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)      587 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SendPackedVirtualTouchEventMessage.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)     5278 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SendPackedVirtualTouchEventMessage_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     2390 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SendPackedVirtualTouchEventMessage_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)      971 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SendVoiceInputMessage.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)    14053 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SendVoiceInputMessage_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     5974 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SendVoiceInputMessage_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)      224 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SetArtworkMessage.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)     3229 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SetArtworkMessage_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1111 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SetArtworkMessage_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)      360 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SetConnectionStateMessage.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)     5025 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SetConnectionStateMessage_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     2038 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SetConnectionStateMessage_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1186 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SetDefaultSupportedCommandsMessage.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)    11313 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SetDefaultSupportedCommandsMessage_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     4577 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SetDefaultSupportedCommandsMessage_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)      269 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SetDiscoveryModeMessage.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)     3834 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SetDiscoveryModeMessage_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1284 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SetDiscoveryModeMessage_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)      235 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SetHiliteModeMessage.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)     3310 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SetHiliteModeMessage_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1136 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SetHiliteModeMessage_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)      322 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SetNowPlayingClientMessage.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)     3917 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SetNowPlayingClientMessage_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1328 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SetNowPlayingClientMessage_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)      314 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SetNowPlayingPlayerMessage.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)     3886 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SetNowPlayingPlayerMessage_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1326 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SetNowPlayingPlayerMessage_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)      342 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SetRecordingStateMessage.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)     4769 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SetRecordingStateMessage_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     2005 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SetRecordingStateMessage_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1085 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SetStateMessage.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)    10502 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SetStateMessage_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     4432 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SetStateMessage_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)      258 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SetVolumeMessage.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)     3682 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SetVolumeMessage_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1314 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SetVolumeMessage_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)      154 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SupportedCommands.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)     2631 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SupportedCommands_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1049 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SupportedCommands_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)      476 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/TextInputMessage.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)     6451 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/TextInputMessage_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     2530 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/TextInputMessage_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)      115 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/TransactionKey.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)     2586 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/TransactionKey_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1000 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/TransactionKey_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)      430 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/TransactionMessage.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)     4990 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/TransactionMessage_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1801 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/TransactionMessage_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)      299 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/TransactionPacket.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)     4452 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/TransactionPacket_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1784 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/TransactionPacket_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)      158 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/TransactionPackets.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)     2652 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/TransactionPackets_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1032 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/TransactionPackets_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)      301 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/UpdateClientMessage.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)     3718 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/UpdateClientMessage_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1293 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/UpdateClientMessage_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)      427 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/UpdateContentItemArtworkMessage.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)     4914 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/UpdateContentItemArtworkMessage_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1817 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/UpdateContentItemArtworkMessage_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)      406 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/UpdateContentItemMessage.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)     4707 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/UpdateContentItemMessage_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1782 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/UpdateContentItemMessage_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)      727 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/UpdateEndPointsMessage.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)     8226 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/UpdateEndPointsMessage_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     3565 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/UpdateEndPointsMessage_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)     2561 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/UpdateOutputDeviceMessage.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)    30545 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/UpdateOutputDeviceMessage_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)    15050 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/UpdateOutputDeviceMessage_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)      206 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/VirtualTouchDeviceDescriptorMessage.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)     3839 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/VirtualTouchDeviceDescriptorMessage_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1556 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/VirtualTouchDeviceDescriptorMessage_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)      234 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/VoiceInputDeviceDescriptorMessage.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)     3567 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/VoiceInputDeviceDescriptorMessage_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1586 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/VoiceInputDeviceDescriptorMessage_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)      592 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/VolumeControlAvailabilityMessage.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)     6497 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/VolumeControlAvailabilityMessage_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     2580 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/VolumeControlAvailabilityMessage_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)      479 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/VolumeControlCapabilitiesDidChangeMessage.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)     5475 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/VolumeControlCapabilitiesDidChangeMessage_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1941 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/VolumeControlCapabilitiesDidChangeMessage_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)      310 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/VolumeDidChangeMessage.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)     4327 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/VolumeDidChangeMessage_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1538 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/VolumeDidChangeMessage_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)      194 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/WakeDeviceMessage.proto
--rw-r--r--   0 postlund  (1000) postlund  (1000)     2784 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/WakeDeviceMessage_pb2.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)      703 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/WakeDeviceMessage_pb2.pyi
--rw-r--r--   0 postlund  (1000) postlund  (1000)    18352 2021-12-05 12:45:08.000000 pyatv-0.9.7/pyatv/protocols/mrp/protobuf/__init__.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     9196 2021-11-24 12:44:27.000000 pyatv-0.9.7/pyatv/protocols/mrp/protocol.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     9100 2021-10-08 10:29:18.000000 pyatv-0.9.7/pyatv/protocols/mrp/server_auth.py
-drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-06 08:00:11.335011 pyatv-0.9.7/pyatv/protocols/raop/
--rw-r--r--   0 postlund  (1000) postlund  (1000)    19424 2021-12-05 20:49:29.000000 pyatv-0.9.7/pyatv/protocols/raop/__init__.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)    15838 2021-12-05 20:49:29.000000 pyatv-0.9.7/pyatv/protocols/raop/audio_source.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     2537 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/raop/fifo.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)      759 2021-10-08 10:29:18.000000 pyatv-0.9.7/pyatv/protocols/raop/packets.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     2660 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/raop/parsers.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)    27734 2021-11-04 07:35:14.000000 pyatv-0.9.7/pyatv/protocols/raop/raop.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1345 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/protocols/raop/timing.py
-drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-06 08:00:11.335011 pyatv-0.9.7/pyatv/scripts/
--rw-r--r--   0 postlund  (1000) postlund  (1000)     3053 2021-10-25 17:59:14.000000 pyatv-0.9.7/pyatv/scripts/__init__.py
--rwxr-xr-x   0 postlund  (1000) postlund  (1000)     8737 2021-09-29 20:18:54.000000 pyatv-0.9.7/pyatv/scripts/atvlog.py
--rwxr-xr-x   0 postlund  (1000) postlund  (1000)    19020 2021-11-01 07:00:26.000000 pyatv-0.9.7/pyatv/scripts/atvproxy.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)    23193 2021-12-05 11:31:42.000000 pyatv-0.9.7/pyatv/scripts/atvremote.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     9363 2021-10-25 17:59:14.000000 pyatv-0.9.7/pyatv/scripts/atvscript.py
-drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-06 08:00:11.335011 pyatv-0.9.7/pyatv/support/
--rw-r--r--   0 postlund  (1000) postlund  (1000)     3179 2021-11-01 21:02:02.000000 pyatv-0.9.7/pyatv/support/__init__.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1291 2021-09-10 16:43:01.000000 pyatv-0.9.7/pyatv/support/cache.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1498 2021-11-24 09:34:48.000000 pyatv-0.9.7/pyatv/support/chacha20.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     5073 2021-11-01 07:00:26.000000 pyatv-0.9.7/pyatv/support/collections.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     2185 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/support/device_info.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)    15849 2021-10-08 10:29:18.000000 pyatv-0.9.7/pyatv/support/dns.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)    19388 2021-12-02 20:27:15.000000 pyatv-0.9.7/pyatv/support/http.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1872 2021-10-20 08:10:37.000000 pyatv-0.9.7/pyatv/support/knock.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1057 2021-09-29 20:18:54.000000 pyatv-0.9.7/pyatv/support/metadata.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     4328 2021-12-05 20:49:29.000000 pyatv-0.9.7/pyatv/support/net.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1080 2021-09-29 20:18:54.000000 pyatv-0.9.7/pyatv/support/packet.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     9983 2021-11-04 07:35:14.000000 pyatv-0.9.7/pyatv/support/rtsp.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     2777 2021-10-08 10:26:03.000000 pyatv-0.9.7/pyatv/support/state_producer.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)      586 2021-09-29 20:18:54.000000 pyatv-0.9.7/pyatv/support/variant.py
-drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-06 08:00:11.303011 pyatv-0.9.7/pyatv.egg-info/
--rw-r--r--   0 postlund  (1000) postlund  (1000)     4651 2021-12-06 08:00:10.000000 pyatv-0.9.7/pyatv.egg-info/PKG-INFO
--rw-r--r--   0 postlund  (1000) postlund  (1000)    20699 2021-12-06 08:00:11.000000 pyatv-0.9.7/pyatv.egg-info/SOURCES.txt
--rw-r--r--   0 postlund  (1000) postlund  (1000)        1 2021-12-06 08:00:10.000000 pyatv-0.9.7/pyatv.egg-info/dependency_links.txt
--rw-r--r--   0 postlund  (1000) postlund  (1000)      175 2021-12-06 08:00:10.000000 pyatv-0.9.7/pyatv.egg-info/entry_points.txt
--rw-r--r--   0 postlund  (1000) postlund  (1000)        1 2019-09-26 04:23:23.000000 pyatv-0.9.7/pyatv.egg-info/not-zip-safe
--rw-r--r--   0 postlund  (1000) postlund  (1000)      156 2021-12-06 08:00:10.000000 pyatv-0.9.7/pyatv.egg-info/requires.txt
--rw-r--r--   0 postlund  (1000) postlund  (1000)        6 2021-12-06 08:00:10.000000 pyatv-0.9.7/pyatv.egg-info/top_level.txt
--rw-r--r--   0 postlund  (1000) postlund  (1000)      560 2021-11-02 11:15:39.000000 pyatv-0.9.7/pyproject.toml
--rw-r--r--   0 postlund  (1000) postlund  (1000)      302 2021-12-06 08:00:11.347011 pyatv-0.9.7/setup.cfg
--rw-r--r--   0 postlund  (1000) postlund  (1000)     2465 2021-10-25 17:59:14.000000 pyatv-0.9.7/setup.py
-drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-06 08:00:11.339011 pyatv-0.9.7/tests/
--rw-r--r--   0 postlund  (1000) postlund  (1000)       28 2019-10-30 11:09:35.000000 pyatv-0.9.7/tests/__init__.py
-drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-06 08:00:11.339011 pyatv-0.9.7/tests/auth/
--rw-r--r--   0 postlund  (1000) postlund  (1000)     3265 2021-09-29 20:18:54.000000 pyatv-0.9.7/tests/auth/test_hap_tlv8.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)    21468 2021-11-03 10:10:51.000000 pyatv-0.9.7/tests/common_functional_tests.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     4934 2021-10-08 10:26:03.000000 pyatv-0.9.7/tests/conftest.py
-drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-06 08:00:11.339011 pyatv-0.9.7/tests/core/
--rw-r--r--   0 postlund  (1000) postlund  (1000)    18344 2021-10-20 08:10:37.000000 pyatv-0.9.7/tests/core/test_facade.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     8129 2021-10-08 10:26:03.000000 pyatv-0.9.7/tests/core/test_mdns.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     9060 2021-10-08 10:26:03.000000 pyatv-0.9.7/tests/core/test_mdns_functional.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     4296 2021-11-01 07:00:26.000000 pyatv-0.9.7/tests/core/test_protocol.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     6945 2021-10-20 08:10:37.000000 pyatv-0.9.7/tests/core/test_relayer.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1106 2021-10-08 10:26:03.000000 pyatv-0.9.7/tests/core/test_scan.py
-drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-06 08:00:11.339011 pyatv-0.9.7/tests/data/
--rw-r--r--   0 postlund  (1000) postlund  (1000)      803 2021-09-10 16:43:01.000000 pyatv-0.9.7/tests/data/README
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1174 2021-09-10 16:43:01.000000 pyatv-0.9.7/tests/data/audio_10_frames.wav
--rw-r--r--   0 postlund  (1000) postlund  (1000)     2548 2021-09-10 16:43:01.000000 pyatv-0.9.7/tests/data/audio_1_packet_metadata.wav
--rw-r--r--   0 postlund  (1000) postlund  (1000)     5358 2021-09-10 16:43:01.000000 pyatv-0.9.7/tests/data/audio_3_packets.wav
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1140 2021-09-10 16:43:01.000000 pyatv-0.9.7/tests/data/only_metadata.wav
--rw-r--r--   0 postlund  (1000) postlund  (1000)     4341 2021-09-10 16:43:01.000000 pyatv-0.9.7/tests/data/static_3sec.ogg
--rw-r--r--   0 postlund  (1000) postlund  (1000)       18 2021-09-10 16:43:01.000000 pyatv-0.9.7/tests/data/testfile.txt
-drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-06 08:00:11.339011 pyatv-0.9.7/tests/fake_device/
--rw-r--r--   0 postlund  (1000) postlund  (1000)     2830 2021-09-30 12:54:47.000000 pyatv-0.9.7/tests/fake_device/__init__.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)    10163 2021-09-21 11:54:22.000000 pyatv-0.9.7/tests/fake_device/airplay.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)    10955 2021-11-01 07:00:26.000000 pyatv-0.9.7/tests/fake_device/companion.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)    16851 2021-10-08 10:26:03.000000 pyatv-0.9.7/tests/fake_device/dmap.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)    27790 2021-10-27 10:53:51.000000 pyatv-0.9.7/tests/fake_device/mrp.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)    19146 2021-10-08 10:26:03.000000 pyatv-0.9.7/tests/fake_device/raop.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)      847 2021-09-10 16:43:01.000000 pyatv-0.9.7/tests/fake_knock.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     9070 2021-10-08 10:29:18.000000 pyatv-0.9.7/tests/fake_udns.py
-drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-06 08:00:11.275010 pyatv-0.9.7/tests/protocols/
-drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-06 08:00:11.339011 pyatv-0.9.7/tests/protocols/airplay/
-drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-06 08:00:11.339011 pyatv-0.9.7/tests/protocols/airplay/auth/
--rw-r--r--   0 postlund  (1000) postlund  (1000)     2496 2021-10-08 10:26:03.000000 pyatv-0.9.7/tests/protocols/airplay/auth/test_airplay_legacy_auth.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     2149 2021-10-08 10:26:03.000000 pyatv-0.9.7/tests/protocols/airplay/auth/test_auth.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1249 2021-10-08 10:26:03.000000 pyatv-0.9.7/tests/protocols/airplay/conftest.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     4257 2021-10-08 10:29:18.000000 pyatv-0.9.7/tests/protocols/airplay/test_airplay.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)      743 2021-10-08 10:26:03.000000 pyatv-0.9.7/tests/protocols/airplay/test_airplay_interface.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     2096 2021-10-08 10:26:03.000000 pyatv-0.9.7/tests/protocols/airplay/test_airplay_pair.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1850 2021-10-08 10:26:03.000000 pyatv-0.9.7/tests/protocols/airplay/test_airplay_player.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1149 2021-10-08 10:26:03.000000 pyatv-0.9.7/tests/protocols/airplay/test_airplay_scan.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     3161 2021-10-25 11:56:50.000000 pyatv-0.9.7/tests/protocols/airplay/test_utils.py
-drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-06 08:00:11.343011 pyatv-0.9.7/tests/protocols/companion/
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1695 2021-11-01 07:00:26.000000 pyatv-0.9.7/tests/protocols/companion/conftest.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     2086 2021-10-08 10:29:18.000000 pyatv-0.9.7/tests/protocols/companion/test_companion.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     3339 2021-11-03 10:10:51.000000 pyatv-0.9.7/tests/protocols/companion/test_companion_auth.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     5037 2021-11-01 07:00:26.000000 pyatv-0.9.7/tests/protocols/companion/test_companion_functional.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1784 2021-10-08 10:26:03.000000 pyatv-0.9.7/tests/protocols/companion/test_companion_scan.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     7756 2021-12-05 20:49:29.000000 pyatv-0.9.7/tests/protocols/companion/test_opack.py
-drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-06 08:00:11.343011 pyatv-0.9.7/tests/protocols/dmap/
--rw-r--r--   0 postlund  (1000) postlund  (1000)     4100 2021-10-08 10:26:03.000000 pyatv-0.9.7/tests/protocols/dmap/test_daap.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     2990 2021-10-08 10:29:18.000000 pyatv-0.9.7/tests/protocols/dmap/test_dmap.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)    11453 2021-10-08 10:29:18.000000 pyatv-0.9.7/tests/protocols/dmap/test_dmap_functional.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     5216 2021-10-25 17:59:14.000000 pyatv-0.9.7/tests/protocols/dmap/test_dmap_pairing.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     3341 2021-10-08 10:26:03.000000 pyatv-0.9.7/tests/protocols/dmap/test_dmap_scan.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     3911 2021-10-08 10:26:03.000000 pyatv-0.9.7/tests/protocols/dmap/test_parser.py
-drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-06 08:00:11.343011 pyatv-0.9.7/tests/protocols/mrp/
--rw-r--r--   0 postlund  (1000) postlund  (1000)        0 2021-10-08 10:26:03.000000 pyatv-0.9.7/tests/protocols/mrp/__init__.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)      746 2021-11-01 07:00:26.000000 pyatv-0.9.7/tests/protocols/mrp/conftest.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     3052 2021-10-08 10:29:18.000000 pyatv-0.9.7/tests/protocols/mrp/test_mrp.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     3442 2021-10-08 10:26:03.000000 pyatv-0.9.7/tests/protocols/mrp/test_mrp_auth.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)    23024 2021-10-27 10:53:51.000000 pyatv-0.9.7/tests/protocols/mrp/test_mrp_functional.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     2821 2021-11-01 07:00:26.000000 pyatv-0.9.7/tests/protocols/mrp/test_mrp_interface.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1158 2021-10-08 10:26:03.000000 pyatv-0.9.7/tests/protocols/mrp/test_mrp_scan.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)    14466 2021-11-01 07:00:26.000000 pyatv-0.9.7/tests/protocols/mrp/test_player_state.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1659 2021-10-08 10:26:03.000000 pyatv-0.9.7/tests/protocols/mrp/test_protocol.py
-drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-06 08:00:11.343011 pyatv-0.9.7/tests/protocols/raop/
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1364 2021-11-01 21:02:02.000000 pyatv-0.9.7/tests/protocols/raop/conftest.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     2149 2021-10-08 10:26:03.000000 pyatv-0.9.7/tests/protocols/raop/test_fifo.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     2352 2021-10-08 10:26:03.000000 pyatv-0.9.7/tests/protocols/raop/test_parsers.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     5236 2021-10-08 10:29:18.000000 pyatv-0.9.7/tests/protocols/raop/test_raop.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)    19939 2021-11-03 10:10:51.000000 pyatv-0.9.7/tests/protocols/raop/test_raop_functional.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1057 2021-10-08 10:26:03.000000 pyatv-0.9.7/tests/protocols/raop/test_raop_scan.py
-drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-06 08:00:11.343011 pyatv-0.9.7/tests/scripts/
--rw-r--r--   0 postlund  (1000) postlund  (1000)     3997 2021-09-29 20:18:54.000000 pyatv-0.9.7/tests/scripts/script_env.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     3704 2021-10-08 10:29:18.000000 pyatv-0.9.7/tests/scripts/test_atvremote.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     2823 2021-10-27 10:53:51.000000 pyatv-0.9.7/tests/scripts/test_atvscript.py
-drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-06 08:00:11.347011 pyatv-0.9.7/tests/support/
--rw-r--r--   0 postlund  (1000) postlund  (1000)     2630 2021-10-08 10:26:03.000000 pyatv-0.9.7/tests/support/dns_utils.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1711 2021-09-10 16:43:01.000000 pyatv-0.9.7/tests/support/test_cache.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     3146 2021-11-01 07:00:26.000000 pyatv-0.9.7/tests/support/test_collections.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1127 2021-10-08 10:29:18.000000 pyatv-0.9.7/tests/support/test_device_info.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)    10011 2021-09-10 16:43:01.000000 pyatv-0.9.7/tests/support/test_dns.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     7886 2021-12-04 17:12:17.000000 pyatv-0.9.7/tests/support/test_http.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1062 2021-09-21 11:54:22.000000 pyatv-0.9.7/tests/support/test_knock.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     4193 2021-11-26 08:58:01.000000 pyatv-0.9.7/tests/support/test_net.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)      953 2021-09-29 20:18:54.000000 pyatv-0.9.7/tests/support/test_packet.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     2241 2021-10-08 10:26:03.000000 pyatv-0.9.7/tests/support/test_state_producer.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     4769 2021-10-08 10:26:03.000000 pyatv-0.9.7/tests/support/test_support.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)      892 2021-10-08 10:26:03.000000 pyatv-0.9.7/tests/support/test_variant.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     7295 2021-12-05 20:49:29.000000 pyatv-0.9.7/tests/test_conf.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     2626 2021-10-08 10:29:18.000000 pyatv-0.9.7/tests/test_convert.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     2692 2021-12-04 17:12:17.000000 pyatv-0.9.7/tests/test_helpers.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)    13243 2021-10-27 10:53:51.000000 pyatv-0.9.7/tests/test_interface.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     6307 2021-12-05 20:49:29.000000 pyatv-0.9.7/tests/test_scan_functional.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     4450 2021-12-04 17:12:17.000000 pyatv-0.9.7/tests/utils.py
--rw-r--r--   0 postlund  (1000) postlund  (1000)     1543 2021-09-10 16:43:01.000000 pyatv-0.9.7/tests/zeroconf_stub.py
+drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-15 18:56:39.509239 pyatv-0.9.8/
+-rw-r--r--   0 postlund  (1000) postlund  (1000)    77436 2021-12-15 18:56:06.000000 pyatv-0.9.8/CHANGES.md
+-rw-r--r--   0 postlund  (1000) postlund  (1000)       90 2021-09-10 16:43:01.000000 pyatv-0.9.8/CONTRIBUTORS.md
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1081 2021-09-10 16:43:01.000000 pyatv-0.9.8/LICENSE.md
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      276 2021-09-10 16:43:01.000000 pyatv-0.9.8/MANIFEST.in
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     4651 2021-12-15 18:56:39.509239 pyatv-0.9.8/PKG-INFO
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     3523 2021-12-15 12:44:35.000000 pyatv-0.9.8/README.md
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      152 2021-12-15 12:44:35.000000 pyatv-0.9.8/base_versions.txt
+drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-15 18:56:39.461239 pyatv-0.9.8/docs/
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      399 2019-11-15 09:37:48.000000 pyatv-0.9.8/docs/404.html
+-rw-r--r--   0 postlund  (1000) postlund  (1000)        9 2021-09-10 16:43:01.000000 pyatv-0.9.8/docs/CNAME
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      991 2019-11-15 09:37:48.000000 pyatv-0.9.8/docs/Gemfile
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     7953 2021-12-04 20:39:30.000000 pyatv-0.9.8/docs/Gemfile.lock
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     2920 2021-09-10 16:43:01.000000 pyatv-0.9.8/docs/_config.yml
+drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-15 18:56:39.461239 pyatv-0.9.8/docs/_includes/
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      399 2021-09-10 16:43:01.000000 pyatv-0.9.8/docs/_includes/api
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      244 2021-09-10 16:43:01.000000 pyatv-0.9.8/docs/_includes/code
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      423 2021-09-10 16:43:01.000000 pyatv-0.9.8/docs/_includes/issue
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      160 2021-09-10 16:43:01.000000 pyatv-0.9.8/docs/_includes/pypi
+drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-15 18:56:39.461239 pyatv-0.9.8/docs/_layouts/
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     4758 2021-09-10 16:43:01.000000 pyatv-0.9.8/docs/_layouts/template.html
+drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-15 18:56:39.461239 pyatv-0.9.8/docs/api/
+drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-15 18:56:39.461239 pyatv-0.9.8/docs/api/pyatv/
+-rw-r--r--   0 postlund  (1000) postlund  (1000)    19304 2021-12-15 18:56:38.000000 pyatv-0.9.8/docs/api/pyatv/conf.html
+-rw-r--r--   0 postlund  (1000) postlund  (1000)    40437 2021-12-15 18:56:38.000000 pyatv-0.9.8/docs/api/pyatv/const.html
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     4610 2021-12-15 18:56:38.000000 pyatv-0.9.8/docs/api/pyatv/convert.html
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     3168 2021-09-29 20:18:54.000000 pyatv-0.9.8/docs/api/pyatv/core.html
+-rw-r--r--   0 postlund  (1000) postlund  (1000)    17722 2021-12-15 18:56:38.000000 pyatv-0.9.8/docs/api/pyatv/exceptions.html
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     3785 2021-12-15 18:56:38.000000 pyatv-0.9.8/docs/api/pyatv/helpers.html
+-rw-r--r--   0 postlund  (1000) postlund  (1000)   107219 2021-12-15 18:56:38.000000 pyatv-0.9.8/docs/api/pyatv/interface.html
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     5076 2021-12-15 18:56:38.000000 pyatv-0.9.8/docs/api/pyatv.html
+drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-15 18:56:39.457239 pyatv-0.9.8/docs/assets/
+drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-15 18:56:39.461239 pyatv-0.9.8/docs/assets/css/
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      296 2021-09-10 16:43:01.000000 pyatv-0.9.8/docs/assets/css/custom.css
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      872 2021-09-10 16:43:01.000000 pyatv-0.9.8/docs/assets/css/hljs.css
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     6138 2021-09-10 16:43:01.000000 pyatv-0.9.8/docs/assets/css/normalize.css
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     3861 2021-09-10 16:43:01.000000 pyatv-0.9.8/docs/assets/css/pdoc.css
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     9527 2021-09-10 16:43:01.000000 pyatv-0.9.8/docs/assets/css/sanitize.css
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      147 2021-09-10 16:43:01.000000 pyatv-0.9.8/docs/assets/css/style.scss
+drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-15 18:56:39.461239 pyatv-0.9.8/docs/assets/img/
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     3024 2021-09-10 16:43:01.000000 pyatv-0.9.8/docs/assets/img/logo.svg
+drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-15 18:56:39.461239 pyatv-0.9.8/docs/assets/js/
+-rw-r--r--   0 postlund  (1000) postlund  (1000)    46003 2021-09-10 16:43:01.000000 pyatv-0.9.8/docs/assets/js/highlight.9.12.0.min.js
+-rw-r--r--   0 postlund  (1000) postlund  (1000)   873682 2021-09-10 16:43:01.000000 pyatv-0.9.8/docs/assets/js/mermaid.8.9.2.min.js
+-rw-r--r--   0 postlund  (1000) postlund  (1000)  3255902 2021-09-10 16:43:01.000000 pyatv-0.9.8/docs/assets/js/mermaid.min.js.map
+drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-15 18:56:39.465239 pyatv-0.9.8/docs/development/
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      832 2021-09-10 16:43:01.000000 pyatv-0.9.8/docs/development/apps.md
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      780 2021-09-10 16:43:01.000000 pyatv-0.9.8/docs/development/audio.md
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1302 2021-09-10 16:43:01.000000 pyatv-0.9.8/docs/development/control.md
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      468 2021-09-10 16:43:01.000000 pyatv-0.9.8/docs/development/development.md
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      917 2021-09-10 16:43:01.000000 pyatv-0.9.8/docs/development/device_info.md
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1679 2021-12-15 12:44:35.000000 pyatv-0.9.8/docs/development/examples.md
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     3080 2021-09-10 16:43:01.000000 pyatv-0.9.8/docs/development/features.md
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     3011 2021-09-10 16:43:01.000000 pyatv-0.9.8/docs/development/listeners.md
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1581 2021-09-10 16:43:01.000000 pyatv-0.9.8/docs/development/logging.md
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     3697 2021-09-10 16:43:01.000000 pyatv-0.9.8/docs/development/metadata.md
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1336 2021-09-10 16:43:01.000000 pyatv-0.9.8/docs/development/power_management.md
+-rw-r--r--   0 postlund  (1000) postlund  (1000)    10685 2021-12-15 12:44:35.000000 pyatv-0.9.8/docs/development/scan_pair_and_connect.md
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      182 2019-11-15 09:37:48.000000 pyatv-0.9.8/docs/development/services.md
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     6851 2021-12-15 12:44:35.000000 pyatv-0.9.8/docs/development/stream.md
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      180 2019-11-15 09:37:48.000000 pyatv-0.9.8/docs/development/testing.md
+drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-15 18:56:39.469239 pyatv-0.9.8/docs/documentation/
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1326 2021-09-10 16:43:01.000000 pyatv-0.9.8/docs/documentation/atvlog.md
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     6417 2021-09-10 16:43:01.000000 pyatv-0.9.8/docs/documentation/atvproxy.md
+-rw-r--r--   0 postlund  (1000) postlund  (1000)    11116 2021-12-15 12:44:35.000000 pyatv-0.9.8/docs/documentation/atvremote.md
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     6835 2021-09-10 16:43:01.000000 pyatv-0.9.8/docs/documentation/atvscript.md
+-rw-r--r--   0 postlund  (1000) postlund  (1000)    11265 2021-12-15 12:44:35.000000 pyatv-0.9.8/docs/documentation/concepts.md
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     4012 2021-12-15 12:44:35.000000 pyatv-0.9.8/docs/documentation/documentation.md
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     4534 2021-09-10 16:43:01.000000 pyatv-0.9.8/docs/documentation/getting_started.md
+-rw-r--r--   0 postlund  (1000) postlund  (1000)    78769 2021-12-15 12:44:35.000000 pyatv-0.9.8/docs/documentation/protocols.md
+-rw-r--r--   0 postlund  (1000) postlund  (1000)    13650 2021-12-15 12:44:35.000000 pyatv-0.9.8/docs/documentation/supported_features.md
+-rw-r--r--   0 postlund  (1000) postlund  (1000)    34262 2021-12-15 12:44:35.000000 pyatv-0.9.8/docs/documentation/tutorial.md
+-rw-r--r--   0 postlund  (1000) postlund  (1000)       47 2021-09-10 16:43:01.000000 pyatv-0.9.8/docs/documentation/workspace.code-workspace
+-rw-r--r--   0 postlund  (1000) postlund  (1000)   186268 2021-09-10 16:43:01.000000 pyatv-0.9.8/docs/favicon.ico
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     5806 2021-12-15 12:44:35.000000 pyatv-0.9.8/docs/index.md
+drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-15 18:56:39.469239 pyatv-0.9.8/docs/internals/
+-rw-r--r--   0 postlund  (1000) postlund  (1000)    13784 2021-12-15 12:44:35.000000 pyatv-0.9.8/docs/internals/design.md
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     4562 2021-12-15 12:44:35.000000 pyatv-0.9.8/docs/internals/documentation.md
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     4352 2021-09-10 16:43:01.000000 pyatv-0.9.8/docs/internals/interfaces.md
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     5419 2021-12-15 12:44:35.000000 pyatv-0.9.8/docs/internals/internals.md
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     2449 2021-12-15 12:44:35.000000 pyatv-0.9.8/docs/internals/submit_pr.md
+-rw-r--r--   0 postlund  (1000) postlund  (1000)    10489 2021-09-10 16:43:01.000000 pyatv-0.9.8/docs/internals/testing.md
+-rw-r--r--   0 postlund  (1000) postlund  (1000)    20281 2021-12-15 12:44:35.000000 pyatv-0.9.8/docs/internals/tools.md
+drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-15 18:56:39.469239 pyatv-0.9.8/docs/pdoc_templates/
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     2095 2021-09-10 16:43:01.000000 pyatv-0.9.8/docs/pdoc_templates/config.mako
+-rw-r--r--   0 postlund  (1000) postlund  (1000)    12068 2021-09-10 16:43:01.000000 pyatv-0.9.8/docs/pdoc_templates/html.mako
+drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-15 18:56:39.469239 pyatv-0.9.8/docs/support/
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     2680 2021-09-10 16:43:01.000000 pyatv-0.9.8/docs/support/acknowledgements.md
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     9777 2021-09-29 20:18:54.000000 pyatv-0.9.8/docs/support/faq.md
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     5144 2021-12-15 12:44:35.000000 pyatv-0.9.8/docs/support/migration.md
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     4944 2021-09-10 16:43:01.000000 pyatv-0.9.8/docs/support/scanning_issues.md
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      707 2021-09-10 16:43:01.000000 pyatv-0.9.8/docs/support/support.md
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     2338 2021-09-10 16:43:01.000000 pyatv-0.9.8/docs/support/troubleshooting.md
+drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-15 18:56:39.469239 pyatv-0.9.8/examples/
+-rw-r--r--   0 postlund  (1000) postlund  (1000)       35 2019-10-30 11:09:35.000000 pyatv-0.9.8/examples/__init__.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      447 2021-09-10 16:43:01.000000 pyatv-0.9.8/examples/auto_connect.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1588 2021-12-15 12:44:35.000000 pyatv-0.9.8/examples/connect_with_credentials.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      937 2021-12-15 12:44:35.000000 pyatv-0.9.8/examples/manual_connect.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      976 2021-09-10 16:43:01.000000 pyatv-0.9.8/examples/pairing.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      973 2021-09-10 16:43:01.000000 pyatv-0.9.8/examples/play_url.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      867 2021-12-15 12:44:35.000000 pyatv-0.9.8/examples/scan_and_connect.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1501 2021-09-21 11:06:52.000000 pyatv-0.9.8/examples/stream.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     6272 2021-09-10 16:43:01.000000 pyatv-0.9.8/examples/tutorial.py
+drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-15 18:56:39.469239 pyatv-0.9.8/pyatv/
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     4331 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/__init__.py
+drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-15 18:56:39.473239 pyatv-0.9.8/pyatv/auth/
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     3186 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/auth/hap_channel.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     4292 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/auth/hap_pairing.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     2164 2021-09-29 20:18:54.000000 pyatv-0.9.8/pyatv/auth/hap_session.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     7841 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/auth/hap_srp.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     3980 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/auth/hap_tlv8.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     7212 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/conf.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     7333 2021-12-15 18:37:05.000000 pyatv-0.9.8/pyatv/const.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     2314 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/convert.py
+drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-15 18:56:39.473239 pyatv-0.9.8/pyatv/core/
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     5451 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/core/__init__.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)    25336 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/core/facade.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)    18562 2021-12-15 17:49:48.000000 pyatv-0.9.8/pyatv/core/mdns.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     3934 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/core/protocol.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     4708 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/core/relayer.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     9888 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/core/scan.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     3057 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/exceptions.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     3005 2021-12-04 17:12:29.000000 pyatv-0.9.8/pyatv/helpers.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)    39104 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/interface.py
+drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-15 18:56:39.473239 pyatv-0.9.8/pyatv/protocols/
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     2485 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/__init__.py
+drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-15 18:56:39.473239 pyatv-0.9.8/pyatv/protocols/airplay/
+-rw-r--r--   0 postlund  (1000) postlund  (1000)    10377 2021-12-15 17:49:48.000000 pyatv-0.9.8/pyatv/protocols/airplay/__init__.py
+drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-15 18:56:39.473239 pyatv-0.9.8/pyatv/protocols/airplay/auth/
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     4411 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/airplay/auth/__init__.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     4611 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/airplay/auth/hap.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     3012 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/airplay/auth/hap_transient.py
+-rwxr-xr-x   0 postlund  (1000) postlund  (1000)     3881 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/airplay/auth/legacy.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     5607 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/airplay/channels.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     2892 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/airplay/mrp_connection.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     3274 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/airplay/pairing.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     3163 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/airplay/player.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     6432 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/airplay/remote_control.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)    11558 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/airplay/server_auth.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     7323 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/airplay/srp.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     5182 2021-12-15 17:49:48.000000 pyatv-0.9.8/pyatv/protocols/airplay/utils.py
+drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-15 18:56:39.473239 pyatv-0.9.8/pyatv/protocols/companion/
+-rw-r--r--   0 postlund  (1000) postlund  (1000)    14178 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/companion/__init__.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     7965 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/companion/api.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     5693 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/companion/auth.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     5110 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/companion/connection.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     7788 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/companion/opack.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     2807 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/companion/pairing.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     8166 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/companion/protocol.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     8368 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/companion/server_auth.py
+drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-15 18:56:39.473239 pyatv-0.9.8/pyatv/protocols/dmap/
+-rw-r--r--   0 postlund  (1000) postlund  (1000)    24967 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/dmap/__init__.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     6046 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/dmap/daap.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     5482 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/dmap/pairing.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     2586 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/dmap/parser.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     5993 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/dmap/tag_definitions.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     2521 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/dmap/tags.py
+drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-15 18:56:39.477239 pyatv-0.9.8/pyatv/protocols/mrp/
+-rw-r--r--   0 postlund  (1000) postlund  (1000)    35064 2021-12-15 17:49:48.000000 pyatv-0.9.8/pyatv/protocols/mrp/__init__.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     4026 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/auth.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     6270 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/connection.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     6798 2021-12-15 17:49:48.000000 pyatv-0.9.8/pyatv/protocols/mrp/messages.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     2900 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/pairing.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)    12221 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/player_state.py
+drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-15 18:56:39.497239 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      190 2019-11-01 04:29:58.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/#GetKeyboardSessionMessage.proto#
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      315 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/AudioFadeMessage.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     4064 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/AudioFadeMessage_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1451 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/AudioFadeMessage_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      249 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/AudioFadeResponseMessage.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     3447 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/AudioFadeResponseMessage_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1170 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/AudioFadeResponseMessage_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)       97 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/AudioFormatSettingsMessage.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     2284 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/AudioFormatSettingsMessage_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      933 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/AudioFormatSettingsMessage_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      409 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/ClientUpdatesConfigMessage.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     5431 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/ClientUpdatesConfigMessage_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     2128 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/ClientUpdatesConfigMessage_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     3179 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/CommandInfo.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)    37321 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/CommandInfo_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)    15637 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/CommandInfo_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1351 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/CommandOptions.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)    16502 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/CommandOptions_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     8037 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/CommandOptions_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1071 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/Common.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)    18104 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/Common_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     7036 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/Common_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      913 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/ContentItem.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     5962 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/ContentItemMetadata.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)    75715 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/ContentItemMetadata_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)    34219 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/ContentItemMetadata_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)    10997 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/ContentItem_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     5359 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/ContentItem_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      409 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/CryptoPairingMessage.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     5144 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/CryptoPairingMessage_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1972 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/CryptoPairingMessage_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1946 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/DeviceInfoMessage.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)    21385 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/DeviceInfoMessage_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)    10144 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/DeviceInfoMessage_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      239 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/GenericMessage.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     3578 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/GenericMessage_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1213 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/GenericMessage_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      199 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/GetKeyboardSessionMessage.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     2904 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/GetKeyboardSessionMessage_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      734 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/GetKeyboardSessionMessage_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      238 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/GetRemoteTextInputSessionMessage.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     3163 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/GetRemoteTextInputSessionMessage_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      778 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/GetRemoteTextInputSessionMessage_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      229 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/GetVolumeMessage.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     3238 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/GetVolumeMessage_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1149 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/GetVolumeMessage_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      237 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/GetVolumeResultMessage.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     3364 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/GetVolumeResultMessage_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1122 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/GetVolumeResultMessage_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1806 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/KeyboardMessage.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)    25455 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/KeyboardMessage_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)    10768 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/KeyboardMessage_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      216 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/LanguageOption.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     3970 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/LanguageOption_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1692 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/LanguageOption_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      265 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/NotificationMessage.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     3741 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/NotificationMessage_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1442 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/NotificationMessage_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      398 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/NowPlayingClient.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     5131 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/NowPlayingClient_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     2613 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/NowPlayingClient_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      765 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/NowPlayingInfo.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)    10541 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/NowPlayingInfo_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     4535 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/NowPlayingInfo_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      155 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/NowPlayingPlayer.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     3113 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/NowPlayingPlayer_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1247 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/NowPlayingPlayer_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      308 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/Origin.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      273 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/OriginClientPropertiesMessage.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     3592 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/OriginClientPropertiesMessage_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1255 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/OriginClientPropertiesMessage_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     4876 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/Origin_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     2104 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/Origin_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      514 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/PlaybackQueue.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      174 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/PlaybackQueueCapabilities.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     3292 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/PlaybackQueueCapabilities_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1380 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/PlaybackQueueCapabilities_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)       85 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/PlaybackQueueContext.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     2233 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/PlaybackQueueContext_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      825 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/PlaybackQueueContext_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1011 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/PlaybackQueueRequestMessage.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)    12067 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/PlaybackQueueRequestMessage_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     5234 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/PlaybackQueueRequestMessage_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     6215 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/PlaybackQueue_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     2795 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/PlaybackQueue_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      367 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/PlayerClientPropertiesMessage.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     4466 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/PlayerClientPropertiesMessage_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1604 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/PlayerClientPropertiesMessage_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      329 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/PlayerPath.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     4166 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/PlayerPath_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1625 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/PlayerPath_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     6800 2021-12-15 17:49:48.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/ProtocolMessage.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)    43501 2021-12-15 17:49:48.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/ProtocolMessage_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)    22118 2021-12-15 17:49:48.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/ProtocolMessage_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      397 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/RegisterForGameControllerEventsMessage.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     5494 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/RegisterForGameControllerEventsMessage_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     2238 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/RegisterForGameControllerEventsMessage_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      356 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/RegisterHIDDeviceMessage.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     4026 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/RegisterHIDDeviceMessage_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1469 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/RegisterHIDDeviceMessage_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      302 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/RegisterHIDDeviceResultMessage.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     4067 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/RegisterHIDDeviceResultMessage_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1410 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/RegisterHIDDeviceResultMessage_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      373 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/RegisterVoiceInputDeviceMessage.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     4202 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/RegisterVoiceInputDeviceMessage_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1494 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/RegisterVoiceInputDeviceMessage_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      321 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/RegisterVoiceInputDeviceResponseMessage.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     4286 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/RegisterVoiceInputDeviceResponseMessage_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1399 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/RegisterVoiceInputDeviceResponseMessage_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      299 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/RemoteTextInputMessage.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     4260 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/RemoteTextInputMessage_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1462 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/RemoteTextInputMessage_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      301 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/RemoveClientMessage.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     3721 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/RemoveClientMessage_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1293 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/RemoveClientMessage_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      244 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/RemoveEndpointsMessage.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     3374 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/RemoveEndpointsMessage_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1193 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/RemoveEndpointsMessage_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      295 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/RemoveOutputDevicesMessage.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     3975 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/RemoveOutputDevicesMessage_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1512 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/RemoveOutputDevicesMessage_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      293 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/RemovePlayerMessage.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     3687 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/RemovePlayerMessage_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1291 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/RemovePlayerMessage_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      302 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SendButtonEventMessage.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     4254 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SendButtonEventMessage_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1484 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SendButtonEventMessage_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      476 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SendCommandMessage.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     5367 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SendCommandMessage_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1938 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SendCommandMessage_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     2676 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SendCommandResultMessage.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)    28775 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SendCommandResultMessage_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)    13028 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SendCommandResultMessage_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1701 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SendHIDEventMessage.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     3295 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SendHIDEventMessage_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     2575 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SendHIDEventMessage_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      587 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SendPackedVirtualTouchEventMessage.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     5278 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SendPackedVirtualTouchEventMessage_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     2390 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SendPackedVirtualTouchEventMessage_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      971 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SendVoiceInputMessage.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)    14053 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SendVoiceInputMessage_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     5974 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SendVoiceInputMessage_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      224 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SetArtworkMessage.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     3229 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SetArtworkMessage_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1111 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SetArtworkMessage_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      360 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SetConnectionStateMessage.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     5025 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SetConnectionStateMessage_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     2038 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SetConnectionStateMessage_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1186 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SetDefaultSupportedCommandsMessage.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)    11313 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SetDefaultSupportedCommandsMessage_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     4577 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SetDefaultSupportedCommandsMessage_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      269 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SetDiscoveryModeMessage.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     3834 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SetDiscoveryModeMessage_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1284 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SetDiscoveryModeMessage_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      235 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SetHiliteModeMessage.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     3310 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SetHiliteModeMessage_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1136 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SetHiliteModeMessage_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      322 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SetNowPlayingClientMessage.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     3917 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SetNowPlayingClientMessage_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1328 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SetNowPlayingClientMessage_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      314 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SetNowPlayingPlayerMessage.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     3886 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SetNowPlayingPlayerMessage_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1326 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SetNowPlayingPlayerMessage_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      342 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SetRecordingStateMessage.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     4769 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SetRecordingStateMessage_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     2005 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SetRecordingStateMessage_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1085 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SetStateMessage.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)    10502 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SetStateMessage_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     4432 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SetStateMessage_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      258 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SetVolumeMessage.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     3682 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SetVolumeMessage_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1314 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SetVolumeMessage_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      154 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SupportedCommands.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     2631 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SupportedCommands_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1049 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SupportedCommands_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      476 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/TextInputMessage.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     6451 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/TextInputMessage_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     2530 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/TextInputMessage_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      115 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/TransactionKey.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     2586 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/TransactionKey_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1000 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/TransactionKey_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      430 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/TransactionMessage.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     4990 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/TransactionMessage_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1801 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/TransactionMessage_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      299 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/TransactionPacket.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     4452 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/TransactionPacket_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1784 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/TransactionPacket_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      158 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/TransactionPackets.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     2652 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/TransactionPackets_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1032 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/TransactionPackets_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      301 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/UpdateClientMessage.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     3718 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/UpdateClientMessage_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1293 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/UpdateClientMessage_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      427 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/UpdateContentItemArtworkMessage.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     4914 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/UpdateContentItemArtworkMessage_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1817 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/UpdateContentItemArtworkMessage_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      406 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/UpdateContentItemMessage.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     4707 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/UpdateContentItemMessage_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1782 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/UpdateContentItemMessage_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      727 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/UpdateEndPointsMessage.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     8226 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/UpdateEndPointsMessage_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     3565 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/UpdateEndPointsMessage_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     2561 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/UpdateOutputDeviceMessage.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)    30545 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/UpdateOutputDeviceMessage_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)    15050 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/UpdateOutputDeviceMessage_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      206 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/VirtualTouchDeviceDescriptorMessage.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     3839 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/VirtualTouchDeviceDescriptorMessage_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1556 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/VirtualTouchDeviceDescriptorMessage_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      234 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/VoiceInputDeviceDescriptorMessage.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     3567 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/VoiceInputDeviceDescriptorMessage_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1586 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/VoiceInputDeviceDescriptorMessage_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      592 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/VolumeControlAvailabilityMessage.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     6497 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/VolumeControlAvailabilityMessage_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     2580 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/VolumeControlAvailabilityMessage_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      479 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/VolumeControlCapabilitiesDidChangeMessage.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     5475 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/VolumeControlCapabilitiesDidChangeMessage_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1941 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/VolumeControlCapabilitiesDidChangeMessage_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      310 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/VolumeDidChangeMessage.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     4327 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/VolumeDidChangeMessage_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1538 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/VolumeDidChangeMessage_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      194 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/WakeDeviceMessage.proto
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     2784 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/WakeDeviceMessage_pb2.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      703 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/WakeDeviceMessage_pb2.pyi
+-rw-r--r--   0 postlund  (1000) postlund  (1000)    18561 2021-12-15 17:49:48.000000 pyatv-0.9.8/pyatv/protocols/mrp/protobuf/__init__.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)    10188 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/protocol.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     9100 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/mrp/server_auth.py
+drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-15 18:56:39.497239 pyatv-0.9.8/pyatv/protocols/raop/
+-rw-r--r--   0 postlund  (1000) postlund  (1000)    19932 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/raop/__init__.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)    15838 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/raop/audio_source.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     2537 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/raop/fifo.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      759 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/raop/packets.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     2660 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/raop/parsers.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)    27734 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/raop/raop.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1345 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/protocols/raop/timing.py
+drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-15 18:56:39.497239 pyatv-0.9.8/pyatv/scripts/
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     3053 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/scripts/__init__.py
+-rwxr-xr-x   0 postlund  (1000) postlund  (1000)     8737 2021-09-29 20:18:54.000000 pyatv-0.9.8/pyatv/scripts/atvlog.py
+-rwxr-xr-x   0 postlund  (1000) postlund  (1000)    19020 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/scripts/atvproxy.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)    23193 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/scripts/atvremote.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     9363 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/scripts/atvscript.py
+drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-15 18:56:39.501239 pyatv-0.9.8/pyatv/support/
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     3179 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/support/__init__.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1291 2021-09-10 16:43:01.000000 pyatv-0.9.8/pyatv/support/cache.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1498 2021-11-24 09:34:48.000000 pyatv-0.9.8/pyatv/support/chacha20.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     5073 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/support/collections.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     2185 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/support/device_info.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)    15849 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/support/dns.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)    19388 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/support/http.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     2323 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/support/knock.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1057 2021-09-29 20:18:54.000000 pyatv-0.9.8/pyatv/support/metadata.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     4413 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/support/net.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1080 2021-09-29 20:18:54.000000 pyatv-0.9.8/pyatv/support/packet.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     9983 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/support/rtsp.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1812 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/support/shield.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     2777 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyatv/support/state_producer.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      586 2021-09-29 20:18:54.000000 pyatv-0.9.8/pyatv/support/variant.py
+drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-15 18:56:39.473239 pyatv-0.9.8/pyatv.egg-info/
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     4651 2021-12-15 18:56:39.000000 pyatv-0.9.8/pyatv.egg-info/PKG-INFO
+-rw-r--r--   0 postlund  (1000) postlund  (1000)    20776 2021-12-15 18:56:39.000000 pyatv-0.9.8/pyatv.egg-info/SOURCES.txt
+-rw-r--r--   0 postlund  (1000) postlund  (1000)        1 2021-12-15 18:56:39.000000 pyatv-0.9.8/pyatv.egg-info/dependency_links.txt
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      175 2021-12-15 18:56:39.000000 pyatv-0.9.8/pyatv.egg-info/entry_points.txt
+-rw-r--r--   0 postlund  (1000) postlund  (1000)        1 2019-09-26 04:23:23.000000 pyatv-0.9.8/pyatv.egg-info/not-zip-safe
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      152 2021-12-15 18:56:39.000000 pyatv-0.9.8/pyatv.egg-info/requires.txt
+-rw-r--r--   0 postlund  (1000) postlund  (1000)        6 2021-12-15 18:56:39.000000 pyatv-0.9.8/pyatv.egg-info/top_level.txt
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      543 2021-12-15 12:44:35.000000 pyatv-0.9.8/pyproject.toml
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      302 2021-12-15 18:56:39.509239 pyatv-0.9.8/setup.cfg
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     2465 2021-12-15 12:44:35.000000 pyatv-0.9.8/setup.py
+drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-15 18:56:39.501239 pyatv-0.9.8/tests/
+-rw-r--r--   0 postlund  (1000) postlund  (1000)       28 2019-10-30 11:09:35.000000 pyatv-0.9.8/tests/__init__.py
+drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-15 18:56:39.501239 pyatv-0.9.8/tests/auth/
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     3265 2021-09-29 20:18:54.000000 pyatv-0.9.8/tests/auth/test_hap_tlv8.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)    21468 2021-12-15 12:44:35.000000 pyatv-0.9.8/tests/common_functional_tests.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     4651 2021-12-15 12:44:35.000000 pyatv-0.9.8/tests/conftest.py
+drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-15 18:56:39.501239 pyatv-0.9.8/tests/core/
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1878 2021-12-15 12:44:35.000000 pyatv-0.9.8/tests/core/test_core.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)    27620 2021-12-15 12:44:35.000000 pyatv-0.9.8/tests/core/test_facade.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     8129 2021-12-15 12:44:35.000000 pyatv-0.9.8/tests/core/test_mdns.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     9060 2021-12-15 12:44:35.000000 pyatv-0.9.8/tests/core/test_mdns_functional.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     4855 2021-12-15 12:44:35.000000 pyatv-0.9.8/tests/core/test_protocol.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     7801 2021-12-15 12:44:35.000000 pyatv-0.9.8/tests/core/test_relayer.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1106 2021-12-15 12:44:35.000000 pyatv-0.9.8/tests/core/test_scan.py
+drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-15 18:56:39.501239 pyatv-0.9.8/tests/data/
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      803 2021-09-10 16:43:01.000000 pyatv-0.9.8/tests/data/README
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1174 2021-09-10 16:43:01.000000 pyatv-0.9.8/tests/data/audio_10_frames.wav
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     2548 2021-09-10 16:43:01.000000 pyatv-0.9.8/tests/data/audio_1_packet_metadata.wav
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     5358 2021-09-10 16:43:01.000000 pyatv-0.9.8/tests/data/audio_3_packets.wav
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1140 2021-09-10 16:43:01.000000 pyatv-0.9.8/tests/data/only_metadata.wav
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     4341 2021-09-10 16:43:01.000000 pyatv-0.9.8/tests/data/static_3sec.ogg
+-rw-r--r--   0 postlund  (1000) postlund  (1000)       18 2021-09-10 16:43:01.000000 pyatv-0.9.8/tests/data/testfile.txt
+drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-15 18:56:39.505239 pyatv-0.9.8/tests/fake_device/
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     2830 2021-09-30 12:54:47.000000 pyatv-0.9.8/tests/fake_device/__init__.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)    10163 2021-09-21 11:54:22.000000 pyatv-0.9.8/tests/fake_device/airplay.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)    10955 2021-12-15 12:44:35.000000 pyatv-0.9.8/tests/fake_device/companion.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)    16851 2021-12-15 12:44:35.000000 pyatv-0.9.8/tests/fake_device/dmap.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)    27790 2021-12-15 12:44:35.000000 pyatv-0.9.8/tests/fake_device/mrp.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)    19146 2021-12-15 12:44:35.000000 pyatv-0.9.8/tests/fake_device/raop.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      847 2021-09-10 16:43:01.000000 pyatv-0.9.8/tests/fake_knock.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     9070 2021-12-15 12:44:35.000000 pyatv-0.9.8/tests/fake_udns.py
+drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-15 18:56:39.457239 pyatv-0.9.8/tests/protocols/
+drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-15 18:56:39.505239 pyatv-0.9.8/tests/protocols/airplay/
+drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-15 18:56:39.505239 pyatv-0.9.8/tests/protocols/airplay/auth/
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     2496 2021-12-15 12:44:35.000000 pyatv-0.9.8/tests/protocols/airplay/auth/test_airplay_legacy_auth.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     2149 2021-12-15 12:44:35.000000 pyatv-0.9.8/tests/protocols/airplay/auth/test_auth.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1249 2021-12-15 12:44:35.000000 pyatv-0.9.8/tests/protocols/airplay/conftest.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     4257 2021-12-15 12:44:35.000000 pyatv-0.9.8/tests/protocols/airplay/test_airplay.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      743 2021-12-15 12:44:35.000000 pyatv-0.9.8/tests/protocols/airplay/test_airplay_interface.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     2096 2021-12-15 12:44:35.000000 pyatv-0.9.8/tests/protocols/airplay/test_airplay_pair.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1850 2021-12-15 12:44:35.000000 pyatv-0.9.8/tests/protocols/airplay/test_airplay_player.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1149 2021-12-15 12:44:35.000000 pyatv-0.9.8/tests/protocols/airplay/test_airplay_scan.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     3880 2021-12-15 17:49:48.000000 pyatv-0.9.8/tests/protocols/airplay/test_utils.py
+drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-15 18:56:39.505239 pyatv-0.9.8/tests/protocols/companion/
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1695 2021-12-15 12:44:35.000000 pyatv-0.9.8/tests/protocols/companion/conftest.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     2086 2021-12-15 12:44:35.000000 pyatv-0.9.8/tests/protocols/companion/test_companion.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     3339 2021-12-15 12:44:35.000000 pyatv-0.9.8/tests/protocols/companion/test_companion_auth.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     5037 2021-12-15 12:44:35.000000 pyatv-0.9.8/tests/protocols/companion/test_companion_functional.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1784 2021-12-15 12:44:35.000000 pyatv-0.9.8/tests/protocols/companion/test_companion_scan.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     7756 2021-12-15 12:44:35.000000 pyatv-0.9.8/tests/protocols/companion/test_opack.py
+drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-15 18:56:39.505239 pyatv-0.9.8/tests/protocols/dmap/
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     4100 2021-12-15 12:44:35.000000 pyatv-0.9.8/tests/protocols/dmap/test_daap.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     2990 2021-12-15 12:44:35.000000 pyatv-0.9.8/tests/protocols/dmap/test_dmap.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)    11453 2021-12-15 12:44:35.000000 pyatv-0.9.8/tests/protocols/dmap/test_dmap_functional.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     5216 2021-12-15 12:44:35.000000 pyatv-0.9.8/tests/protocols/dmap/test_dmap_pairing.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     3341 2021-12-15 12:44:35.000000 pyatv-0.9.8/tests/protocols/dmap/test_dmap_scan.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     3911 2021-12-15 12:44:35.000000 pyatv-0.9.8/tests/protocols/dmap/test_parser.py
+drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-15 18:56:39.505239 pyatv-0.9.8/tests/protocols/mrp/
+-rw-r--r--   0 postlund  (1000) postlund  (1000)        0 2021-12-15 12:44:35.000000 pyatv-0.9.8/tests/protocols/mrp/__init__.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      746 2021-12-15 12:44:35.000000 pyatv-0.9.8/tests/protocols/mrp/conftest.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     3052 2021-12-15 12:44:35.000000 pyatv-0.9.8/tests/protocols/mrp/test_mrp.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     3442 2021-12-15 12:44:35.000000 pyatv-0.9.8/tests/protocols/mrp/test_mrp_auth.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)    23024 2021-12-15 12:44:35.000000 pyatv-0.9.8/tests/protocols/mrp/test_mrp_functional.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     2821 2021-12-15 12:44:35.000000 pyatv-0.9.8/tests/protocols/mrp/test_mrp_interface.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1158 2021-12-15 12:44:35.000000 pyatv-0.9.8/tests/protocols/mrp/test_mrp_scan.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)    14466 2021-12-15 12:44:35.000000 pyatv-0.9.8/tests/protocols/mrp/test_player_state.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1659 2021-12-15 12:44:35.000000 pyatv-0.9.8/tests/protocols/mrp/test_protocol.py
+drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-15 18:56:39.505239 pyatv-0.9.8/tests/protocols/raop/
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1364 2021-12-15 12:44:35.000000 pyatv-0.9.8/tests/protocols/raop/conftest.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     2149 2021-12-15 12:44:35.000000 pyatv-0.9.8/tests/protocols/raop/test_fifo.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     2352 2021-12-15 12:44:35.000000 pyatv-0.9.8/tests/protocols/raop/test_parsers.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     5236 2021-12-15 12:44:35.000000 pyatv-0.9.8/tests/protocols/raop/test_raop.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)    20062 2021-12-15 12:44:35.000000 pyatv-0.9.8/tests/protocols/raop/test_raop_functional.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1057 2021-12-15 12:44:35.000000 pyatv-0.9.8/tests/protocols/raop/test_raop_scan.py
+drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-15 18:56:39.505239 pyatv-0.9.8/tests/scripts/
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     3997 2021-09-29 20:18:54.000000 pyatv-0.9.8/tests/scripts/script_env.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     3704 2021-12-15 12:44:35.000000 pyatv-0.9.8/tests/scripts/test_atvremote.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     2823 2021-12-15 12:44:35.000000 pyatv-0.9.8/tests/scripts/test_atvscript.py
+drwxr-xr-x   0 postlund  (1000) postlund  (1000)        0 2021-12-15 18:56:39.509239 pyatv-0.9.8/tests/support/
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     2630 2021-12-15 12:44:35.000000 pyatv-0.9.8/tests/support/dns_utils.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1711 2021-09-10 16:43:01.000000 pyatv-0.9.8/tests/support/test_cache.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     3146 2021-12-15 12:44:35.000000 pyatv-0.9.8/tests/support/test_collections.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1127 2021-12-15 12:44:35.000000 pyatv-0.9.8/tests/support/test_device_info.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)    10011 2021-09-10 16:43:01.000000 pyatv-0.9.8/tests/support/test_dns.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     7886 2021-12-04 17:12:17.000000 pyatv-0.9.8/tests/support/test_http.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     2061 2021-12-15 12:44:35.000000 pyatv-0.9.8/tests/support/test_knock.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     4028 2021-12-15 12:44:35.000000 pyatv-0.9.8/tests/support/test_net.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      953 2021-09-29 20:18:54.000000 pyatv-0.9.8/tests/support/test_packet.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1270 2021-12-15 12:44:35.000000 pyatv-0.9.8/tests/support/test_shield.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     2241 2021-12-15 12:44:35.000000 pyatv-0.9.8/tests/support/test_state_producer.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     4769 2021-12-15 12:44:35.000000 pyatv-0.9.8/tests/support/test_support.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)      892 2021-12-15 12:44:35.000000 pyatv-0.9.8/tests/support/test_variant.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     7295 2021-12-15 12:44:35.000000 pyatv-0.9.8/tests/test_conf.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     2626 2021-12-15 12:44:35.000000 pyatv-0.9.8/tests/test_convert.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     2692 2021-12-04 17:12:17.000000 pyatv-0.9.8/tests/test_helpers.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)    12169 2021-12-15 12:44:35.000000 pyatv-0.9.8/tests/test_interface.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     6307 2021-12-15 12:44:35.000000 pyatv-0.9.8/tests/test_scan_functional.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     4450 2021-12-04 17:12:17.000000 pyatv-0.9.8/tests/utils.py
+-rw-r--r--   0 postlund  (1000) postlund  (1000)     1543 2021-09-10 16:43:01.000000 pyatv-0.9.8/tests/zeroconf_stub.py
```

### Comparing `pyatv-0.9.7/CHANGES.md` & `pyatv-0.9.8/CHANGES.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,88 @@
 # CHANGES
 
+## 0.9.8 Vanny (2021-12-15)
+
+Here is yet another release with a bunch of bug fixes and improvements:
+
+* Calling public interface methods after disconnecting now results
+  in `BlockedStateError` being raised
+* `power_state` now depends on `device_state`. Because of the unreliable
+  method used to derive `power_state`, a device could be reported as
+  powered off while playing some media, which doesn't make sense. As
+  long as `device_state` is not `idle`, the power state will be reported
+  as on.
+* Button presses in MRP should be more reliable and not skipped or
+  repeated now.
+* `netifaces` has been replaced by `ifaddr` due to lack of a maintainer.
+* A few fixes have been made for MRP on devices running tvOS <= 14.
+* The pause `pause` in RAOP will now stops playback. This is merely
+  because it's not implemented yet and aligns better with Home
+  Assistant for now.
+
+**Changes:**
+
+*Protocol: MRP:*
+
+```
+18d7a6e mrp: Do not disable MRP service for older tvOS
+9541d21 mrp: Fix erroneous button press behavior (#1521)
+74d38b2 mrp: Add enable_encryption to connection
+```
+
+*Protocol: AirPlay:*
+
+```
+3065d6c airplay: Be stricter when setting up remotecontrol
+```
+
+*Protocol: RAOP:*
+
+```
+f0c4c33 raop: Let pause button stop playback
+```
+
+*Other:*
+
+```
+6540c49 facade: Block calls to public methods after close
+c6e9466 facade: Make Power interface respect play status
+4b0136b dep: Migrate from netifaces to ifaddr
+```
+
+**All changes:**
+
+```
+732339f protobuf: Fix support on Windows
+ba5e6bb protobuf: Use version from base_versions.txt
+4d565d8 gh: Update question issue
+23be7cb build(deps): bump cryptography from 36.0.0 to 36.0.1 in /requirements
+ff13e68 mdns: Quiet error log if address cannot be added
+3065d6c airplay: Be stricter when setting up remotecontrol
+18d7a6e mrp: Do not disable MRP service for older tvOS
+9541d21 mrp: Fix erroneous button press behavior (#1521)
+6713225 build(deps): bump pytest-timeout from 2.0.1 to 2.0.2 in /requirements (#1529)
+2009c18 knock Ensure knock yields to the event loop often enough to avoid blocking (#1515)
+6540c49 facade: Block calls to public methods after close
+2d4d526 support: Add shield module
+b00dbf4 build(deps): bump pytest-xdist from 2.4.0 to 2.5.0 in /requirements
+f555e46 core: Clean up dispatchers
+67fcb09 core: Specialize StateDispatcher in protcols
+a72947d core: Prevent duplicates from state producer
+f27c5a4 if: Remove loop argument to PushUpdater
+c6e9466 facade: Make Power interface respect play status
+c67819b core: Add main_protocol to Relayer
+c84bf4a core: Add base support for internal state updates
+605b1a6 core: Add filtering to MessageDispatcher
+2d0a1ca core: Support plain functions in MessageDispatcher
+4b0136b dep: Migrate from netifaces to ifaddr
+f0c4c33 raop: Let pause button stop playback
+74d38b2 mrp: Add enable_encryption to connection
+```
+
 ## 0.9.7 Springtrap (2021-12-05)
 
 It's already Decemeber, how did that happen? Not sure... Anyways, I've
 prepared a small update with few neat things:
 
 * Implemented a missing type in OPACK that raised an exception when
   connecting to Companion for some people (`TypeError: 0xc0`)
```

### Comparing `pyatv-0.9.7/LICENSE.md` & `pyatv-0.9.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/PKG-INFO` & `pyatv-0.9.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pyatv
-Version: 0.9.7
+Version: 0.9.8
 Summary: A client library for Apple TV and AirPlay devices
 Home-page: https://pyatv.dev
 Author: Pierre Ståhl
 Author-email: pierre.staahl@gmail.com
 License: MIT
-Download-URL: https://github.com/postlund/pyatv/archive/refs/tags/v0.9.7.zip
+Download-URL: https://github.com/postlund/pyatv/archive/refs/tags/v0.9.8.zip
 Project-URL: Repository, https://github.com/postlund/pyatv
 Project-URL: Bug Reports, https://github.com/postlund/pyatv/issues
 Keywords: apple,tv,airplay,raop,companion,dmap,dacp
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyatv-0.9.7/README.md` & `pyatv-0.9.8/README.md`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/docs/Gemfile` & `pyatv-0.9.8/docs/Gemfile`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/docs/Gemfile.lock` & `pyatv-0.9.8/docs/Gemfile.lock`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/docs/_config.yml` & `pyatv-0.9.8/docs/_config.yml`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/docs/_layouts/template.html` & `pyatv-0.9.8/docs/_layouts/template.html`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/docs/api/pyatv/conf.html` & `pyatv-0.9.8/docs/api/pyatv/conf.html`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/docs/api/pyatv/const.html` & `pyatv-0.9.8/docs/api/pyatv/const.html`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/docs/api/pyatv/convert.html` & `pyatv-0.9.8/docs/api/pyatv/convert.html`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/docs/api/pyatv/core.html` & `pyatv-0.9.8/docs/api/pyatv/core.html`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/docs/api/pyatv/exceptions.html` & `pyatv-0.9.8/docs/api/pyatv/exceptions.html`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,17 @@
 <li>
 <h4><code><a title="pyatv.exceptions.AuthenticationError" href="#pyatv.exceptions.AuthenticationError">AuthenticationError</a></code></h4>
 </li>
 <li>
 <h4><code><a title="pyatv.exceptions.BackOffError" href="#pyatv.exceptions.BackOffError">BackOffError</a></code></h4>
 </li>
 <li>
+<h4><code><a title="pyatv.exceptions.BlockedStateError" href="#pyatv.exceptions.BlockedStateError">BlockedStateError</a></code></h4>
+</li>
+<li>
 <h4><code><a title="pyatv.exceptions.CommandError" href="#pyatv.exceptions.CommandError">CommandError</a></code></h4>
 </li>
 <li>
 <h4><code><a title="pyatv.exceptions.ConnectionFailedError" href="#pyatv.exceptions.ConnectionFailedError">ConnectionFailedError</a></code></h4>
 </li>
 <li>
 <h4><code><a title="pyatv.exceptions.DeviceIdMissingError" href="#pyatv.exceptions.DeviceIdMissingError">DeviceIdMissingError</a></code></h4>
@@ -89,15 +92,15 @@
 </nav>
 <article id="content">
 <header>
 <h1 class="title">Module <code>pyatv.exceptions</code></h1>
 </header>
 <section id="section-intro">
 <p>Local exceptions used by library.</p>
-<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/exceptions.py#L1-L106" class="git-link">Browse git</a></div>
+<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/exceptions.py#L1-L115" class="git-link">Browse git</a></div>
 </section>
 <section>
 </section>
 <section>
 </section>
 <section>
 </section>
@@ -126,14 +129,30 @@
 <div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/exceptions.py#L59-L60" class="git-link">Browse git</a></div>
 <h3>Ancestors</h3>
 <ul class="hlist">
 <li>builtins.Exception</li>
 <li>builtins.BaseException</li>
 </ul>
 </dd>
+<dt id="pyatv.exceptions.BlockedStateError"><code class="flex name class">
+<span>class <span class="ident">BlockedStateError</span></span>
+<span>(</span><span>*args, **kwargs)</span>
+</code></dt>
+<dd>
+<section class="desc"><p>Thrown when calling a blocked method.</p>
+<p>Typically, public interface methods (e.g. any method available via the object
+returned by <code><a title="pyatv.connect" href="index#pyatv.connect">connect()</a></code>) becomes blocked after either calling close or because
+the connection was closed for some other reason.</p></section>
+<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/exceptions.py#L109-L115" class="git-link">Browse git</a></div>
+<h3>Ancestors</h3>
+<ul class="hlist">
+<li>builtins.Exception</li>
+<li>builtins.BaseException</li>
+</ul>
+</dd>
 <dt id="pyatv.exceptions.CommandError"><code class="flex name class">
 <span>class <span class="ident">CommandError</span></span>
 <span>(</span><span>*args, **kwargs)</span>
 </code></dt>
 <dd>
 <section class="desc"><p>Thrown when a command (e.g. play or pause) failed.</p></section>
 <div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/exceptions.py#L67-L68" class="git-link">Browse git</a></div>
```

#### html2text {}

```diff
@@ -2,14 +2,15 @@
 link_group: api ---
 ****** Index ******
     * **** Super-module ****
           o pyatv
     * **** Classes ****
           o *** AuthenticationError ***
           o *** BackOffError ***
+          o *** BlockedStateError ***
           o *** CommandError ***
           o *** ConnectionFailedError ***
           o *** DeviceIdMissingError ***
           o *** HttpError ***
                 # status_code
           o *** InvalidConfigError ***
           o *** InvalidCredentialsError ***
@@ -41,14 +42,23 @@
           * builtins.BaseException
   class BackOffError (*args, **kwargs)
       Thrown when device mandates a backoff period.
       Browse_git
       **** Ancestors ****
           * builtins.Exception
           * builtins.BaseException
+  class BlockedStateError (*args, **kwargs)
+      Thrown when calling a blocked method.
+      Typically, public interface methods (e.g. any method available via the
+      object returned by connect()) becomes blocked after either calling close
+      or because the connection was closed for some other reason.
+      Browse_git
+      **** Ancestors ****
+          * builtins.Exception
+          * builtins.BaseException
   class CommandError (*args, **kwargs)
       Thrown when a command (e.g. play or pause) failed.
       Browse_git
       **** Ancestors ****
           * builtins.Exception
           * builtins.BaseException
   class ConnectionFailedError (*args, **kwargs)
```

### Comparing `pyatv-0.9.7/docs/api/pyatv/helpers.html` & `pyatv-0.9.8/docs/api/pyatv/helpers.html`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/docs/api/pyatv/interface.html` & `pyatv-0.9.8/docs/api/pyatv/interface.html`

 * *Files 1% similar despite different names*

```diff
@@ -198,15 +198,14 @@
 <li><code><a title="pyatv.interface.PushListener.playstatus_update" href="#pyatv.interface.PushListener.playstatus_update">playstatus_update</a></code></li>
 </ul>
 </li>
 <li>
 <h4><code><a title="pyatv.interface.PushUpdater" href="#pyatv.interface.PushUpdater">PushUpdater</a></code></h4>
 <ul class="">
 <li><code><a title="pyatv.interface.PushUpdater.active" href="#pyatv.interface.PushUpdater.active">active</a></code></li>
-<li><code><a title="pyatv.interface.PushUpdater.post_update" href="#pyatv.interface.PushUpdater.post_update">post_update</a></code></li>
 <li><code><a title="pyatv.interface.PushUpdater.start" href="#pyatv.interface.PushUpdater.start">start</a></code></li>
 <li><code><a title="pyatv.interface.PushUpdater.stop" href="#pyatv.interface.PushUpdater.stop">stop</a></code></li>
 </ul>
 </li>
 <li>
 <h4><code><a title="pyatv.interface.RemoteControl" href="#pyatv.interface.RemoteControl">RemoteControl</a></code></h4>
 <ul class="two-column">
@@ -252,15 +251,15 @@
 <header>
 <h1 class="title">Module <code>pyatv.interface</code></h1>
 </header>
 <section id="section-intro">
 <p>Public interface exposed by library.</p>
 <p>This module contains all the interfaces that represents a generic Apple TV device and
 all its features.</p>
-<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L1-L1231" class="git-link">Browse git</a></div>
+<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L1-L1221" class="git-link">Browse git</a></div>
 </section>
 <section>
 </section>
 <section>
 </section>
 <section>
 <h2 class="section-title" id="header-functions">Functions</h2>
@@ -305,15 +304,15 @@
 <span>class <span class="ident">AppleTV</span></span>
 <span>(</span><span>max_calls: int = 0)</span>
 </code></dt>
 <dd>
 <section class="desc"><p>Base class representing an Apple TV.</p>
 <p>Listener interface: <code>pyatv.interfaces.DeviceListener</code></p>
 <p>Initialize a new StateProducer instance.</p></section>
-<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L1166-L1231" class="git-link">Browse git</a></div>
+<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L1156-L1221" class="git-link">Browse git</a></div>
 <h3>Ancestors</h3>
 <ul class="hlist">
 <li>abc.ABC</li>
 <li>pyatv.support.state_producer.StateProducer</li>
 <li>typing.Generic</li>
 </ul>
 <h3>Subclasses</h3>
@@ -321,82 +320,82 @@
 <li>pyatv.core.facade.FacadeAppleTV</li>
 </ul>
 <h3>Instance variables</h3>
 <dl>
 <dt id="pyatv.interface.AppleTV.apps"><code class="name">var <span class="ident">apps</span> -> <a title="pyatv.interface.Apps" href="#pyatv.interface.Apps">Apps</a></code></dt>
 <dd>
 <section class="desc"><p>Return apps interface.</p></section>
-<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L1223-L1226" class="git-link">Browse git</a></div>
+<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L1213-L1216" class="git-link">Browse git</a></div>
 </dd>
 <dt id="pyatv.interface.AppleTV.audio"><code class="name">var <span class="ident">audio</span> -> <a title="pyatv.interface.Audio" href="#pyatv.interface.Audio">Audio</a></code></dt>
 <dd>
 <section class="desc"><p>Return audio interface.</p></section>
-<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L1228-L1231" class="git-link">Browse git</a></div>
+<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L1218-L1221" class="git-link">Browse git</a></div>
 </dd>
 <dt id="pyatv.interface.AppleTV.device_info"><code class="name">var <span class="ident">device_info</span> -> <a title="pyatv.interface.DeviceInfo" href="#pyatv.interface.DeviceInfo">DeviceInfo</a></code></dt>
 <dd>
 <section class="desc"><p>Return API for device information.</p></section>
-<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L1183-L1186" class="git-link">Browse git</a></div>
+<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L1173-L1176" class="git-link">Browse git</a></div>
 </dd>
 <dt id="pyatv.interface.AppleTV.features"><code class="name">var <span class="ident">features</span> -> <a title="pyatv.interface.Features" href="#pyatv.interface.Features">Features</a></code></dt>
 <dd>
 <section class="desc"><p>Return features interface.</p></section>
-<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L1218-L1221" class="git-link">Browse git</a></div>
+<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L1208-L1211" class="git-link">Browse git</a></div>
 </dd>
 <dt id="pyatv.interface.AppleTV.metadata"><code class="name">var <span class="ident">metadata</span> -> <a title="pyatv.interface.Metadata" href="#pyatv.interface.Metadata">Metadata</a></code></dt>
 <dd>
 <section class="desc"><p>Return API for retrieving metadata from the Apple TV.</p></section>
-<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L1198-L1201" class="git-link">Browse git</a></div>
+<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L1188-L1191" class="git-link">Browse git</a></div>
 </dd>
 <dt id="pyatv.interface.AppleTV.power"><code class="name">var <span class="ident">power</span> -> <a title="pyatv.interface.Power" href="#pyatv.interface.Power">Power</a></code></dt>
 <dd>
 <section class="desc"><p>Return API for power management.</p></section>
-<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L1213-L1216" class="git-link">Browse git</a></div>
+<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L1203-L1206" class="git-link">Browse git</a></div>
 </dd>
 <dt id="pyatv.interface.AppleTV.push_updater"><code class="name">var <span class="ident">push_updater</span> -> <a title="pyatv.interface.PushUpdater" href="#pyatv.interface.PushUpdater">PushUpdater</a></code></dt>
 <dd>
 <section class="desc"><p>Return API for handling push update from the Apple TV.</p></section>
-<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L1203-L1206" class="git-link">Browse git</a></div>
+<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L1193-L1196" class="git-link">Browse git</a></div>
 </dd>
 <dt id="pyatv.interface.AppleTV.remote_control"><code class="name">var <span class="ident">remote_control</span> -> <a title="pyatv.interface.RemoteControl" href="#pyatv.interface.RemoteControl">RemoteControl</a></code></dt>
 <dd>
 <section class="desc"><p>Return API for controlling the Apple TV.</p></section>
-<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L1193-L1196" class="git-link">Browse git</a></div>
+<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L1183-L1186" class="git-link">Browse git</a></div>
 </dd>
 <dt id="pyatv.interface.AppleTV.service"><code class="name">var <span class="ident">service</span> -> <a title="pyatv.interface.BaseService" href="#pyatv.interface.BaseService">BaseService</a></code></dt>
 <dd>
 <section class="desc"><p>Return service used to connect to the Apple TV.</p></section>
-<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L1188-L1191" class="git-link">Browse git</a></div>
+<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L1178-L1181" class="git-link">Browse git</a></div>
 </dd>
 <dt id="pyatv.interface.AppleTV.stream"><code class="name">var <span class="ident">stream</span> -> <a title="pyatv.interface.Stream" href="#pyatv.interface.Stream">Stream</a></code></dt>
 <dd>
 <section class="desc"><p>Return API for streaming media.</p></section>
-<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L1208-L1211" class="git-link">Browse git</a></div>
+<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L1198-L1201" class="git-link">Browse git</a></div>
 </dd>
 </dl>
 <h3>Methods</h3>
 <dl>
 <dt id="pyatv.interface.AppleTV.close">
 <code class="name flex">
 <span>def <span class="ident">close</span></span>(<span>self) -> Set[_asyncio.Task]</span>
 </code>
 </dt>
 <dd>
 <section class="desc"><p>Close connection and release allocated resources.</p></section>
-<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L1179-L1181" class="git-link">Browse git</a></div>
+<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L1169-L1171" class="git-link">Browse git</a></div>
 </dd>
 <dt id="pyatv.interface.AppleTV.connect">
 <code class="name flex">
 <span>async def <span class="ident">connect</span></span>(<span>self) -> None</span>
 </code>
 </dt>
 <dd>
 <section class="desc"><p>Initiate connection to device.</p>
 <p>No need to call it yourself, it's done automatically.</p></section>
-<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L1172-L1177" class="git-link">Browse git</a></div>
+<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L1162-L1167" class="git-link">Browse git</a></div>
 </dd>
 </dl>
 </dd>
 <dt id="pyatv.interface.Apps"><code class="flex name class">
 <span>class <span class="ident">Apps</span></span>
 </code></dt>
 <dd>
@@ -470,15 +469,15 @@
 </dd>
 <dt id="pyatv.interface.Audio"><code class="flex name class">
 <span>class <span class="ident">Audio</span></span>
 </code></dt>
 <dd>
 <section class="desc"><p>Base class for audio functionality.</p>
 <p>Volume level is managed in percent where 0 is muted and 100 is max volume.</p></section>
-<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L988-L1033" class="git-link">Browse git</a></div>
+<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L978-L1023" class="git-link">Browse git</a></div>
 <h3>Subclasses</h3>
 <ul class="hlist">
 <li>pyatv.core.facade.FacadeAudio</li>
 <li>pyatv.protocols.companion.CompanionAudio</li>
 <li>pyatv.protocols.dmap.DmapAudio</li>
 <li>pyatv.protocols.mrp.MrpAudio</li>
 <li>pyatv.protocols.raop.RaopAudio</li>
@@ -489,15 +488,15 @@
 <dd>
 <div class="api_feature">
 <span>Feature: <a title="pyatv.const.FeatureName.Volume" href="const#pyatv.const.FeatureName.Volume">FeatureName.Volume</a>,</span>
 <span>Supported by: <a title="pyatv.const.Protocol.Companion" href="const#pyatv.const.Protocol.Companion">Protocol.Companion</a>, <a title="pyatv.const.Protocol.MRP" href="const#pyatv.const.Protocol.MRP">Protocol.MRP</a>, <a title="pyatv.const.Protocol.RAOP" href="const#pyatv.const.Protocol.RAOP">Protocol.RAOP</a></span>
 </div>
 <section class="desc"><p>Return current volume level.</p>
 <p>Range is in percent, i.e. [0.0-100.0].</p></section>
-<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L994-L1001" class="git-link">Browse git</a></div>
+<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L984-L991" class="git-link">Browse git</a></div>
 </dd>
 </dl>
 <h3>Methods</h3>
 <dl>
 <dt id="pyatv.interface.Audio.set_volume">
 <code class="name flex">
 <span>async def <span class="ident">set_volume</span></span>(<span>self, level: float) -> None</span>
@@ -506,15 +505,15 @@
 <dd>
 <div class="api_feature">
 <span>Feature: <a title="pyatv.const.FeatureName.SetVolume" href="const#pyatv.const.FeatureName.SetVolume">FeatureName.SetVolume</a>,</span>
 <span>Supported by: <a title="pyatv.const.Protocol.Companion" href="const#pyatv.const.Protocol.Companion">Protocol.Companion</a>, <a title="pyatv.const.Protocol.MRP" href="const#pyatv.const.Protocol.MRP">Protocol.MRP</a>, <a title="pyatv.const.Protocol.RAOP" href="const#pyatv.const.Protocol.RAOP">Protocol.RAOP</a></span>
 </div>
 <section class="desc"><p>Change current volume level.</p>
 <p>Range is in percent, i.e. [0.0-100.0].</p></section>
-<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L1003-L1009" class="git-link">Browse git</a></div>
+<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L993-L999" class="git-link">Browse git</a></div>
 </dd>
 <dt id="pyatv.interface.Audio.volume_down">
 <code class="name flex">
 <span>async def <span class="ident">volume_down</span></span>(<span>self) -> None</span>
 </code>
 </dt>
 <dd>
@@ -523,15 +522,15 @@
 <span>Supported by: <a title="pyatv.const.Protocol.Companion" href="const#pyatv.const.Protocol.Companion">Protocol.Companion</a>, <a title="pyatv.const.Protocol.DMAP" href="const#pyatv.const.Protocol.DMAP">Protocol.DMAP</a>, <a title="pyatv.const.Protocol.MRP" href="const#pyatv.const.Protocol.MRP">Protocol.MRP</a>, <a title="pyatv.const.Protocol.RAOP" href="const#pyatv.const.Protocol.RAOP">Protocol.RAOP</a></span>
 </div>
 <section class="desc"><p>Decrease volume by one step.</p>
 <p>Step size is device dependent, but usually around 2.5% of the total volume
 range. It is not necessarily linear.</p>
 <p>Call will block until volume change has been acknowledged by the device (when
 possible and supported).</p></section>
-<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L1023-L1033" class="git-link">Browse git</a></div>
+<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L1013-L1023" class="git-link">Browse git</a></div>
 </dd>
 <dt id="pyatv.interface.Audio.volume_up">
 <code class="name flex">
 <span>async def <span class="ident">volume_up</span></span>(<span>self) -> None</span>
 </code>
 </dt>
 <dd>
@@ -540,125 +539,125 @@
 <span>Supported by: <a title="pyatv.const.Protocol.Companion" href="const#pyatv.const.Protocol.Companion">Protocol.Companion</a>, <a title="pyatv.const.Protocol.DMAP" href="const#pyatv.const.Protocol.DMAP">Protocol.DMAP</a>, <a title="pyatv.const.Protocol.MRP" href="const#pyatv.const.Protocol.MRP">Protocol.MRP</a>, <a title="pyatv.const.Protocol.RAOP" href="const#pyatv.const.Protocol.RAOP">Protocol.RAOP</a></span>
 </div>
 <section class="desc"><p>Increase volume by one step.</p>
 <p>Step size is device dependent, but usually around 2,5% of the total volume
 range. It is not necessarily linear.</p>
 <p>Call will block until volume change has been acknowledged by the device (when
 possible and supported).</p></section>
-<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L1011-L1021" class="git-link">Browse git</a></div>
+<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L1001-L1011" class="git-link">Browse git</a></div>
 </dd>
 </dl>
 </dd>
 <dt id="pyatv.interface.BaseConfig"><code class="flex name class">
 <span>class <span class="ident">BaseConfig</span></span>
 <span>(</span><span>properties: Mapping[str, Mapping[str, Any]])</span>
 </code></dt>
 <dd>
 <section class="desc"><p>Representation of a device configuration.</p>
 <p>An instance of this class represents a single device. A device can have
 several services depending on the protocols it supports, e.g. DMAP or
 AirPlay.</p>
 <p>Initialize a new BaseConfig instance.</p></section>
-<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L1036-L1163" class="git-link">Browse git</a></div>
+<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L1026-L1153" class="git-link">Browse git</a></div>
 <h3>Ancestors</h3>
 <ul class="hlist">
 <li>abc.ABC</li>
 </ul>
 <h3>Subclasses</h3>
 <ul class="hlist">
 <li><a title="pyatv.conf.AppleTV" href="conf#pyatv.conf.AppleTV">AppleTV</a></li>
 </ul>
 <h3>Instance variables</h3>
 <dl>
 <dt id="pyatv.interface.BaseConfig.address"><code class="name">var <span class="ident">address</span> -> ipaddress.IPv4Address</code></dt>
 <dd>
 <section class="desc"><p>IP address of device.</p></section>
-<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L1048-L1051" class="git-link">Browse git</a></div>
+<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L1038-L1041" class="git-link">Browse git</a></div>
 </dd>
 <dt id="pyatv.interface.BaseConfig.all_identifiers"><code class="name">var <span class="ident">all_identifiers</span> -> List[str]</code></dt>
 <dd>
 <section class="desc"><p>Return all unique identifiers for this device.</p></section>
-<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L1110-L1113" class="git-link">Browse git</a></div>
+<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L1100-L1103" class="git-link">Browse git</a></div>
 </dd>
 <dt id="pyatv.interface.BaseConfig.deep_sleep"><code class="name">var <span class="ident">deep_sleep</span> -> bool</code></dt>
 <dd>
 <section class="desc"><p>If device is in deep sleep.</p></section>
-<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L1058-L1061" class="git-link">Browse git</a></div>
+<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L1048-L1051" class="git-link">Browse git</a></div>
 </dd>
 <dt id="pyatv.interface.BaseConfig.device_info"><code class="name">var <span class="ident">device_info</span> -> <a title="pyatv.interface.DeviceInfo" href="#pyatv.interface.DeviceInfo">DeviceInfo</a></code></dt>
 <dd>
 <section class="desc"><p>Return general device information.</p></section>
-<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L1068-L1071" class="git-link">Browse git</a></div>
+<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L1058-L1061" class="git-link">Browse git</a></div>
 </dd>
 <dt id="pyatv.interface.BaseConfig.identifier"><code class="name">var <span class="ident">identifier</span> -> Optional[str]</code></dt>
 <dd>
 <section class="desc"><p>Return the main identifier associated with this device.</p></section>
-<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L1101-L1108" class="git-link">Browse git</a></div>
+<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L1091-L1098" class="git-link">Browse git</a></div>
 </dd>
 <dt id="pyatv.interface.BaseConfig.name"><code class="name">var <span class="ident">name</span> -> str</code></dt>
 <dd>
 <section class="desc"><p>Name of device.</p></section>
-<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L1053-L1056" class="git-link">Browse git</a></div>
+<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L1043-L1046" class="git-link">Browse git</a></div>
 </dd>
 <dt id="pyatv.interface.BaseConfig.properties"><code class="name">var <span class="ident">properties</span> -> Mapping[str, Mapping[str, str]]</code></dt>
 <dd>
 <section class="desc"><p>Return Zeroconf properties.</p></section>
-<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L1088-L1091" class="git-link">Browse git</a></div>
+<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L1078-L1081" class="git-link">Browse git</a></div>
 </dd>
 <dt id="pyatv.interface.BaseConfig.ready"><code class="name">var <span class="ident">ready</span> -> bool</code></dt>
 <dd>
 <section class="desc"><p>Return if configuration is ready, (at least one service with identifier).</p></section>
-<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L1093-L1099" class="git-link">Browse git</a></div>
+<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L1083-L1089" class="git-link">Browse git</a></div>
 </dd>
 <dt id="pyatv.interface.BaseConfig.services"><code class="name">var <span class="ident">services</span> -> List[<a title="pyatv.interface.BaseService" href="#pyatv.interface.BaseService">BaseService</a>]</code></dt>
 <dd>
 <section class="desc"><p>Return all supported services.</p></section>
-<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L1063-L1066" class="git-link">Browse git</a></div>
+<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L1053-L1056" class="git-link">Browse git</a></div>
 </dd>
 </dl>
 <h3>Methods</h3>
 <dl>
 <dt id="pyatv.interface.BaseConfig.add_service">
 <code class="name flex">
 <span>def <span class="ident">add_service</span></span>(<span>self, service: <a title="pyatv.interface.BaseService" href="#pyatv.interface.BaseService">BaseService</a>) -> None</span>
 </code>
 </dt>
 <dd>
 <section class="desc"><p>Add a new service.</p>
 <p>If the service already exists, it will be merged.</p></section>
-<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L1073-L1078" class="git-link">Browse git</a></div>
+<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L1063-L1068" class="git-link">Browse git</a></div>
 </dd>
 <dt id="pyatv.interface.BaseConfig.get_service">
 <code class="name flex">
 <span>def <span class="ident">get_service</span></span>(<span>self, protocol: <a title="pyatv.const.Protocol" href="const#pyatv.const.Protocol">Protocol</a>) -> Optional[<a title="pyatv.interface.BaseService" href="#pyatv.interface.BaseService">BaseService</a>]</span>
 </code>
 </dt>
 <dd>
 <section class="desc"><p>Look up a service based on protocol.</p>
 <p>If a service with the specified protocol is not available, None is
 returned.</p></section>
-<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L1080-L1086" class="git-link">Browse git</a></div>
+<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L1070-L1076" class="git-link">Browse git</a></div>
 </dd>
 <dt id="pyatv.interface.BaseConfig.main_service">
 <code class="name flex">
 <span>def <span class="ident">main_service</span></span>(<span>self, protocol: Optional[<a title="pyatv.const.Protocol" href="const#pyatv.const.Protocol">Protocol</a>] = None) -> <a title="pyatv.interface.BaseService" href="#pyatv.interface.BaseService">BaseService</a></span>
 </code>
 </dt>
 <dd>
 <section class="desc"><p>Return suggested service used to establish connection.</p></section>
-<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L1115-L1128" class="git-link">Browse git</a></div>
+<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L1105-L1118" class="git-link">Browse git</a></div>
 </dd>
 <dt id="pyatv.interface.BaseConfig.set_credentials">
 <code class="name flex">
 <span>def <span class="ident">set_credentials</span></span>(<span>self, protocol: <a title="pyatv.const.Protocol" href="const#pyatv.const.Protocol">Protocol</a>, credentials: str) -> bool</span>
 </code>
 </dt>
 <dd>
 <section class="desc"><p>Set credentials for a protocol if it exists.</p></section>
-<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L1130-L1136" class="git-link">Browse git</a></div>
+<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L1120-L1126" class="git-link">Browse git</a></div>
 </dd>
 </dl>
 </dd>
 <dt id="pyatv.interface.BaseService"><code class="flex name class">
 <span>class <span class="ident">BaseService</span></span>
 <span>(</span><span>identifier: Optional[str], protocol: <a title="pyatv.const.Protocol" href="const#pyatv.const.Protocol">Protocol</a>, port: int, properties: Optional[Mapping[str, str]], credentials: Optional[str] = None, password: Optional[str] = None, enabled: bool = True)</span>
 </code></dt>
@@ -730,57 +729,57 @@
 <dt id="pyatv.interface.DeviceInfo"><code class="flex name class">
 <span>class <span class="ident">DeviceInfo</span></span>
 <span>(</span><span>device_info: Mapping[str, Any])</span>
 </code></dt>
 <dd>
 <section class="desc"><p>General information about device.</p>
 <p>Initialize a new DeviceInfo instance.</p></section>
-<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L839-L950" class="git-link">Browse git</a></div>
+<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L829-L940" class="git-link">Browse git</a></div>
 <h3>Instance variables</h3>
 <dl>
 <dt id="pyatv.interface.DeviceInfo.build_number"><code class="name">var <span class="ident">build_number</span> -> Optional[str]</code></dt>
 <dd>
 <section class="desc"><p>Operating system build number, e.g. 17K795.</p></section>
-<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L901-L904" class="git-link">Browse git</a></div>
+<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L891-L894" class="git-link">Browse git</a></div>
 </dd>
 <dt id="pyatv.interface.DeviceInfo.mac"><code class="name">var <span class="ident">mac</span> -> Optional[str]</code></dt>
 <dd>
 <section class="desc"><p>Device MAC address.</p></section>
-<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L920-L923" class="git-link">Browse git</a></div>
+<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L910-L913" class="git-link">Browse git</a></div>
 </dd>
 <dt id="pyatv.interface.DeviceInfo.model"><code class="name">var <span class="ident">model</span> -> <a title="pyatv.const.DeviceModel" href="const#pyatv.const.DeviceModel">DeviceModel</a></code></dt>
 <dd>
 <section class="desc"><p>Hardware model name, e.g. 3, 4 or 4K.</p></section>
-<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L906-L909" class="git-link">Browse git</a></div>
+<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L896-L899" class="git-link">Browse git</a></div>
 </dd>
 <dt id="pyatv.interface.DeviceInfo.operating_system"><code class="name">var <span class="ident">operating_system</span> -> <a title="pyatv.const.OperatingSystem" href="const#pyatv.const.OperatingSystem">OperatingSystem</a></code></dt>
 <dd>
 <section class="desc"><p>Operating system running on device.</p></section>
-<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L868-L887" class="git-link">Browse git</a></div>
+<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L858-L877" class="git-link">Browse git</a></div>
 </dd>
 <dt id="pyatv.interface.DeviceInfo.raw_model"><code class="name">var <span class="ident">raw_model</span> -> Optional[str]</code></dt>
 <dd>
 <section class="desc"><p>Return raw model description.</p>
 <p>If <code><a title="pyatv.interface.DeviceInfo.model" href="#pyatv.interface.DeviceInfo.model">DeviceInfo.model</a></code> returns <code><a title="pyatv.const.DeviceModel.Unknown" href="const#pyatv.const.DeviceModel.Unknown">DeviceModel.Unknown</a></code>
 then this property contains the raw model string (if any is available).</p></section>
-<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L911-L918" class="git-link">Browse git</a></div>
+<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L901-L908" class="git-link">Browse git</a></div>
 </dd>
 <dt id="pyatv.interface.DeviceInfo.version"><code class="name">var <span class="ident">version</span> -> Optional[str]</code></dt>
 <dd>
 <section class="desc"><p>Operating system version.</p></section>
-<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L889-L899" class="git-link">Browse git</a></div>
+<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L879-L889" class="git-link">Browse git</a></div>
 </dd>
 </dl>
 </dd>
 <dt id="pyatv.interface.DeviceListener"><code class="flex name class">
 <span>class <span class="ident">DeviceListener</span></span>
 </code></dt>
 <dd>
 <section class="desc"><p>Listener interface for generic device updates.</p></section>
-<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L791-L802" class="git-link">Browse git</a></div>
+<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L781-L792" class="git-link">Browse git</a></div>
 <h3>Ancestors</h3>
 <ul class="hlist">
 <li>abc.ABC</li>
 </ul>
 <h3>Subclasses</h3>
 <ul class="hlist">
 <li>pyatv.scripts.atvremote.DeviceListener</li>
@@ -791,24 +790,24 @@
 <dt id="pyatv.interface.DeviceListener.connection_closed">
 <code class="name flex">
 <span>def <span class="ident">connection_closed</span></span>(<span>self) -> None</span>
 </code>
 </dt>
 <dd>
 <section class="desc"><p>Device connection was (intentionally) closed.</p></section>
-<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L799-L802" class="git-link">Browse git</a></div>
+<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L789-L792" class="git-link">Browse git</a></div>
 </dd>
 <dt id="pyatv.interface.DeviceListener.connection_lost">
 <code class="name flex">
 <span>def <span class="ident">connection_lost</span></span>(<span>self, exception: Exception) -> None</span>
 </code>
 </dt>
 <dd>
 <section class="desc"><p>Device was unexpectedly disconnected.</p></section>
-<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L794-L797" class="git-link">Browse git</a></div>
+<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L784-L787" class="git-link">Browse git</a></div>
 </dd>
 </dl>
 </dd>
 <dt id="pyatv.interface.FeatureInfo"><code class="flex name class">
 <span>class <span class="ident">FeatureInfo</span></span>
 <span>(</span><span>state: <a title="pyatv.const.FeatureState" href="const#pyatv.const.FeatureState">FeatureState</a>, options: Optional[Dict[str, object]] = {})</span>
 </code></dt>
@@ -832,15 +831,15 @@
 </dl>
 </dd>
 <dt id="pyatv.interface.Features"><code class="flex name class">
 <span>class <span class="ident">Features</span></span>
 </code></dt>
 <dd>
 <section class="desc"><p>Base class for supported feature functionality.</p></section>
-<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L953-L985" class="git-link">Browse git</a></div>
+<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L943-L975" class="git-link">Browse git</a></div>
 <h3>Subclasses</h3>
 <ul class="hlist">
 <li>pyatv.core.facade.FacadeFeatures</li>
 <li>pyatv.protocols.airplay.AirPlayFeatures</li>
 <li>pyatv.protocols.companion.CompanionFeatures</li>
 <li>pyatv.protocols.dmap.DmapFeatures</li>
 <li>pyatv.protocols.mrp.MrpFeatures</li>
@@ -851,36 +850,36 @@
 <dt id="pyatv.interface.Features.all_features">
 <code class="name flex">
 <span>def <span class="ident">all_features</span></span>(<span>self, include_unsupported=False) -> Dict[<a title="pyatv.const.FeatureName" href="const#pyatv.const.FeatureName">FeatureName</a>, <a title="pyatv.interface.FeatureInfo" href="#pyatv.interface.FeatureInfo">FeatureInfo</a>]</span>
 </code>
 </dt>
 <dd>
 <section class="desc"><p>Return state of all features.</p></section>
-<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L960-L967" class="git-link">Browse git</a></div>
+<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L950-L957" class="git-link">Browse git</a></div>
 </dd>
 <dt id="pyatv.interface.Features.get_feature">
 <code class="name flex">
 <span>def <span class="ident">get_feature</span></span>(<span>self, feature_name: <a title="pyatv.const.FeatureName" href="const#pyatv.const.FeatureName">FeatureName</a>) -> <a title="pyatv.interface.FeatureInfo" href="#pyatv.interface.FeatureInfo">FeatureInfo</a></span>
 </code>
 </dt>
 <dd>
 <section class="desc"><p>Return current state of a feature.</p></section>
-<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L956-L958" class="git-link">Browse git</a></div>
+<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L946-L948" class="git-link">Browse git</a></div>
 </dd>
 <dt id="pyatv.interface.Features.in_state">
 <code class="name flex">
 <span>def <span class="ident">in_state</span></span>(<span>self, states: Union[List[<a title="pyatv.const.FeatureState" href="const#pyatv.const.FeatureState">FeatureState</a>], <a title="pyatv.const.FeatureState" href="const#pyatv.const.FeatureState">FeatureState</a>], *feature_names: <a title="pyatv.const.FeatureName" href="const#pyatv.const.FeatureName">FeatureName</a>)</span>
 </code>
 </dt>
 <dd>
 <section class="desc"><p>Return if features are in a specific state.</p>
 <p>This method will return True if all given features are in the state specified
 by "states". If "states" is a list of states, it is enough for the feature to be
 in one of the listed states.</p></section>
-<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L969-L985" class="git-link">Browse git</a></div>
+<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L959-L975" class="git-link">Browse git</a></div>
 </dd>
 </dl>
 </dd>
 <dt id="pyatv.interface.Metadata"><code class="flex name class">
 <span>class <span class="ident">Metadata</span></span>
 </code></dt>
 <dd>
@@ -1172,15 +1171,15 @@
 <span>class <span class="ident">Power</span></span>
 <span>(</span><span>max_calls: int = 0)</span>
 </code></dt>
 <dd>
 <section class="desc"><p>Base class for retrieving power state from an Apple TV.</p>
 <p>Listener interface: <code>pyatv.interfaces.PowerListener</code></p>
 <p>Initialize a new StateProducer instance.</p></section>
-<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L816-L836" class="git-link">Browse git</a></div>
+<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L806-L826" class="git-link">Browse git</a></div>
 <h3>Ancestors</h3>
 <ul class="hlist">
 <li>abc.ABC</li>
 <li>pyatv.support.state_producer.StateProducer</li>
 <li>typing.Generic</li>
 </ul>
 <h3>Subclasses</h3>
@@ -1194,15 +1193,15 @@
 <dt id="pyatv.interface.Power.power_state"><code class="name">var <span class="ident">power_state</span> -> <a title="pyatv.const.PowerState" href="const#pyatv.const.PowerState">PowerState</a></code></dt>
 <dd>
 <div class="api_feature">
 <span>Feature: <a title="pyatv.const.FeatureName.PowerState" href="const#pyatv.const.FeatureName.PowerState">FeatureName.PowerState</a>,</span>
 <span>Supported by: <a title="pyatv.const.Protocol.MRP" href="const#pyatv.const.Protocol.MRP">Protocol.MRP</a></span>
 </div>
 <section class="desc"><p>Return device power state.</p></section>
-<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L822-L826" class="git-link">Browse git</a></div>
+<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L812-L816" class="git-link">Browse git</a></div>
 </dd>
 </dl>
 <h3>Methods</h3>
 <dl>
 <dt id="pyatv.interface.Power.turn_off">
 <code class="name flex">
 <span>async def <span class="ident">turn_off</span></span>(<span>self, await_new_state: bool = False) -> None</span>
@@ -1210,37 +1209,37 @@
 </dt>
 <dd>
 <div class="api_feature">
 <span>Feature: <a title="pyatv.const.FeatureName.TurnOff" href="const#pyatv.const.FeatureName.TurnOff">FeatureName.TurnOff</a>,</span>
 <span>Supported by: <a title="pyatv.const.Protocol.Companion" href="const#pyatv.const.Protocol.Companion">Protocol.Companion</a>, <a title="pyatv.const.Protocol.MRP" href="const#pyatv.const.Protocol.MRP">Protocol.MRP</a></span>
 </div>
 <section class="desc"><p>Turn device off.</p></section>
-<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L833-L836" class="git-link">Browse git</a></div>
+<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L823-L826" class="git-link">Browse git</a></div>
 </dd>
 <dt id="pyatv.interface.Power.turn_on">
 <code class="name flex">
 <span>async def <span class="ident">turn_on</span></span>(<span>self, await_new_state: bool = False) -> None</span>
 </code>
 </dt>
 <dd>
 <div class="api_feature">
 <span>Feature: <a title="pyatv.const.FeatureName.TurnOn" href="const#pyatv.const.FeatureName.TurnOn">FeatureName.TurnOn</a>,</span>
 <span>Supported by: <a title="pyatv.const.Protocol.Companion" href="const#pyatv.const.Protocol.Companion">Protocol.Companion</a>, <a title="pyatv.const.Protocol.MRP" href="const#pyatv.const.Protocol.MRP">Protocol.MRP</a></span>
 </div>
 <section class="desc"><p>Turn device on.</p></section>
-<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L828-L831" class="git-link">Browse git</a></div>
+<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L818-L821" class="git-link">Browse git</a></div>
 </dd>
 </dl>
 </dd>
 <dt id="pyatv.interface.PowerListener"><code class="flex name class">
 <span>class <span class="ident">PowerListener</span></span>
 </code></dt>
 <dd>
 <section class="desc"><p>Listener interface for power updates.</p></section>
-<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L805-L813" class="git-link">Browse git</a></div>
+<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L795-L803" class="git-link">Browse git</a></div>
 <h3>Ancestors</h3>
 <ul class="hlist">
 <li>abc.ABC</li>
 </ul>
 <h3>Subclasses</h3>
 <ul class="hlist">
 <li>pyatv.core.facade.FacadePower</li>
@@ -1251,15 +1250,15 @@
 <dt id="pyatv.interface.PowerListener.powerstate_update">
 <code class="name flex">
 <span>def <span class="ident">powerstate_update</span></span>(<span>self, old_state: <a title="pyatv.const.PowerState" href="const#pyatv.const.PowerState">PowerState</a>, new_state: <a title="pyatv.const.PowerState" href="const#pyatv.const.PowerState">PowerState</a>)</span>
 </code>
 </dt>
 <dd>
 <section class="desc"><p>Device power state was updated.</p></section>
-<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L808-L813" class="git-link">Browse git</a></div>
+<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L798-L803" class="git-link">Browse git</a></div>
 </dd>
 </dl>
 </dd>
 <dt id="pyatv.interface.PushListener"><code class="flex name class">
 <span>class <span class="ident">PushListener</span></span>
 </code></dt>
 <dd>
@@ -1295,75 +1294,66 @@
 <section class="desc"><p>Inform about changes to what is currently playing.</p></section>
 <div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L719-L721" class="git-link">Browse git</a></div>
 </dd>
 </dl>
 </dd>
 <dt id="pyatv.interface.PushUpdater"><code class="flex name class">
 <span>class <span class="ident">PushUpdater</span></span>
-<span>(</span><span>loop: asyncio.events.AbstractEventLoop)</span>
+<span>(</span><span>max_calls: int = 0)</span>
 </code></dt>
 <dd>
 <section class="desc"><p>Base class for push/async updates from an Apple TV.</p>
-<p>Listener interface: <code><a title="pyatv.interface.PushListener" href="#pyatv.interface.PushListener">PushListener</a></code></p>
-<p>Initialize a new PushUpdater.</p></section>
-<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L728-L765" class="git-link">Browse git</a></div>
+<p>A <code><a title="pyatv.interface.PushUpdater" href="#pyatv.interface.PushUpdater">PushUpdater</a></code> shall only publish update in case the state
+actually changes.</p>
+<p>Listener interface: <code><a title="pyatv.interface.PushListener" href="#pyatv.interface.PushListener">PushListener</a></code>.</p>
+<p>Initialize a new StateProducer instance.</p></section>
+<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L728-L755" class="git-link">Browse git</a></div>
 <h3>Ancestors</h3>
 <ul class="hlist">
 <li>abc.ABC</li>
 <li>pyatv.support.state_producer.StateProducer</li>
 <li>typing.Generic</li>
 </ul>
 <h3>Subclasses</h3>
 <ul class="hlist">
+<li>pyatv.core.AbstractPushUpdater</li>
 <li>pyatv.core.facade.FacadePushUpdater</li>
-<li>pyatv.protocols.dmap.DmapPushUpdater</li>
-<li>pyatv.protocols.mrp.MrpPushUpdater</li>
-<li>pyatv.protocols.raop.RaopPushUpdater</li>
 </ul>
 <h3>Instance variables</h3>
 <dl>
 <dt id="pyatv.interface.PushUpdater.active"><code class="name">var <span class="ident">active</span> -> bool</code></dt>
 <dd>
 <section class="desc"><p>Return if push updater has been started.</p></section>
-<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L740-L744" class="git-link">Browse git</a></div>
+<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L737-L741" class="git-link">Browse git</a></div>
 </dd>
 </dl>
 <h3>Methods</h3>
 <dl>
-<dt id="pyatv.interface.PushUpdater.post_update">
-<code class="name flex">
-<span>def <span class="ident">post_update</span></span>(<span>self, playing: <a title="pyatv.interface.Playing" href="#pyatv.interface.Playing">Playing</a>) -> None</span>
-</code>
-</dt>
-<dd>
-<section class="desc"><p>Post an update to listener.</p></section>
-<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L760-L765" class="git-link">Browse git</a></div>
-</dd>
 <dt id="pyatv.interface.PushUpdater.start">
 <code class="name flex">
 <span>def <span class="ident">start</span></span>(<span>self, initial_delay: int = 0) -> None</span>
 </code>
 </dt>
 <dd>
 <div class="api_feature">
 <span>Feature: <a title="pyatv.const.FeatureName.PushUpdates" href="const#pyatv.const.FeatureName.PushUpdates">FeatureName.PushUpdates</a>,</span>
-<span>Supported by: <a title="pyatv.const.Protocol.DMAP" href="const#pyatv.const.Protocol.DMAP">Protocol.DMAP</a>, <a title="pyatv.const.Protocol.MRP" href="const#pyatv.const.Protocol.MRP">Protocol.MRP</a>, <a title="pyatv.const.Protocol.RAOP" href="const#pyatv.const.Protocol.RAOP">Protocol.RAOP</a></span>
+<span>Supported by: </span>
 </div>
 <section class="desc"><p>Begin to listen to updates.</p>
 <p>If an error occurs, start must be called again.</p></section>
-<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L746-L753" class="git-link">Browse git</a></div>
+<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L743-L750" class="git-link">Browse git</a></div>
 </dd>
 <dt id="pyatv.interface.PushUpdater.stop">
 <code class="name flex">
 <span>def <span class="ident">stop</span></span>(<span>self) -> None</span>
 </code>
 </dt>
 <dd>
 <section class="desc"><p>No longer forward updates to listener.</p></section>
-<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L755-L758" class="git-link">Browse git</a></div>
+<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L752-L755" class="git-link">Browse git</a></div>
 </dd>
 </dl>
 </dd>
 <dt id="pyatv.interface.RemoteControl"><code class="flex name class">
 <span>class <span class="ident">RemoteControl</span></span>
 </code></dt>
 <dd>
@@ -1461,15 +1451,15 @@
 <code class="name flex">
 <span>async def <span class="ident">pause</span></span>(<span>self) -> None</span>
 </code>
 </dt>
 <dd>
 <div class="api_feature">
 <span>Feature: <a title="pyatv.const.FeatureName.Pause" href="const#pyatv.const.FeatureName.Pause">FeatureName.Pause</a>,</span>
-<span>Supported by: <a title="pyatv.const.Protocol.Companion" href="const#pyatv.const.Protocol.Companion">Protocol.Companion</a>, <a title="pyatv.const.Protocol.DMAP" href="const#pyatv.const.Protocol.DMAP">Protocol.DMAP</a>, <a title="pyatv.const.Protocol.MRP" href="const#pyatv.const.Protocol.MRP">Protocol.MRP</a></span>
+<span>Supported by: <a title="pyatv.const.Protocol.Companion" href="const#pyatv.const.Protocol.Companion">Protocol.Companion</a>, <a title="pyatv.const.Protocol.DMAP" href="const#pyatv.const.Protocol.DMAP">Protocol.DMAP</a>, <a title="pyatv.const.Protocol.MRP" href="const#pyatv.const.Protocol.MRP">Protocol.MRP</a>, <a title="pyatv.const.Protocol.RAOP" href="const#pyatv.const.Protocol.RAOP">Protocol.RAOP</a></span>
 </div>
 <section class="desc"><p>Press key play.</p></section>
 <div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L293-L296" class="git-link">Browse git</a></div>
 </dd>
 <dt id="pyatv.interface.RemoteControl.play">
 <code class="name flex">
 <span>async def <span class="ident">play</span></span>(<span>self) -> None</span>
@@ -1700,15 +1690,15 @@
 </dl>
 </dd>
 <dt id="pyatv.interface.Stream"><code class="flex name class">
 <span>class <span class="ident">Stream</span></span>
 </code></dt>
 <dd>
 <section class="desc"><p>Base class for stream functionality.</p></section>
-<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L768-L788" class="git-link">Browse git</a></div>
+<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L758-L778" class="git-link">Browse git</a></div>
 <h3>Subclasses</h3>
 <ul class="hlist">
 <li>pyatv.core.facade.FacadeStream</li>
 <li>pyatv.protocols.airplay.AirPlayStream</li>
 <li>pyatv.protocols.raop.RaopStream</li>
 </ul>
 <h3>Methods</h3>
@@ -1716,43 +1706,43 @@
 <dt id="pyatv.interface.Stream.close">
 <code class="name flex">
 <span>def <span class="ident">close</span></span>(<span>self) -> None</span>
 </code>
 </dt>
 <dd>
 <section class="desc"><p>Close connection and release allocated resources.</p></section>
-<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L771-L773" class="git-link">Browse git</a></div>
+<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L761-L763" class="git-link">Browse git</a></div>
 </dd>
 <dt id="pyatv.interface.Stream.play_url">
 <code class="name flex">
 <span>async def <span class="ident">play_url</span></span>(<span>self, url: str, **kwargs) -> None</span>
 </code>
 </dt>
 <dd>
 <div class="api_feature">
 <span>Feature: <a title="pyatv.const.FeatureName.PlayUrl" href="const#pyatv.const.FeatureName.PlayUrl">FeatureName.PlayUrl</a>,</span>
 <span>Supported by: <a title="pyatv.const.Protocol.AirPlay" href="const#pyatv.const.Protocol.AirPlay">Protocol.AirPlay</a></span>
 </div>
 <section class="desc"><p>Play media from an URL on the device.</p></section>
-<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L775-L778" class="git-link">Browse git</a></div>
+<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L765-L768" class="git-link">Browse git</a></div>
 </dd>
 <dt id="pyatv.interface.Stream.stream_file">
 <code class="name flex">
 <span>async def <span class="ident">stream_file</span></span>(<span>self, file: Union[str, _io.BufferedReader], **kwargs) -> None</span>
 </code>
 </dt>
 <dd>
 <div class="api_feature">
 <span>Feature: <a title="pyatv.const.FeatureName.StreamFile" href="const#pyatv.const.FeatureName.StreamFile">FeatureName.StreamFile</a>,</span>
 <span>Supported by: <a title="pyatv.const.Protocol.RAOP" href="const#pyatv.const.Protocol.RAOP">Protocol.RAOP</a></span>
 </div>
 <section class="desc"><p>Stream local or remote file to device.</p>
 <p>Supports either local file paths or a HTTP(s) address.</p>
 <p>INCUBATING METHOD - MIGHT CHANGE IN THE FUTURE!</p></section>
-<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L780-L788" class="git-link">Browse git</a></div>
+<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/interface.py#L770-L778" class="git-link">Browse git</a></div>
 </dd>
 </dl>
 </dd>
 </dl>
 </section>
 </article>
 <footer id="footer">
```

#### html2text {}

```diff
@@ -112,15 +112,14 @@
           o *** PowerListener ***
                 # powerstate_update
           o *** PushListener ***
                 # playstatus_error
                 # playstatus_update
           o *** PushUpdater ***
                 # active
-                # post_update
                 # start
                 # stop
           o *** RemoteControl ***
                 # down
                 # home
                 # home_hold
                 # left
@@ -667,39 +666,35 @@
       **** Methods ****
         def playstatus_error(self, updater, exception:Â Exception) ->Â None
             Inform about an error when updating play status.
             Browse_git
         def playstatus_update(self, updater, playstatus:Â Playing) ->Â None
             Inform about changes to what is currently playing.
             Browse_git
-  class PushUpdater (loop:Â asyncio.events.AbstractEventLoop)
+  class PushUpdater (max_calls:Â intÂ =Â 0)
       Base class for push/async updates from an Apple TV.
-      Listener interface: PushListener
-      Initialize a new PushUpdater.
+      A PushUpdater shall only publish update in case the state actually
+      changes.
+      Listener interface: PushListener.
+      Initialize a new StateProducer instance.
       Browse_git
       **** Ancestors ****
           * abc.ABC
           * pyatv.support.state_producer.StateProducer
           * typing.Generic
       **** Subclasses ****
+          * pyatv.core.AbstractPushUpdater
           * pyatv.core.facade.FacadePushUpdater
-          * pyatv.protocols.dmap.DmapPushUpdater
-          * pyatv.protocols.mrp.MrpPushUpdater
-          * pyatv.protocols.raop.RaopPushUpdater
       **** Instance variables ****
         var active ->Â bool
             Return if push updater has been started.
             Browse_git
       **** Methods ****
-        def post_update(self, playing:Â Playing) ->Â None
-            Post an update to listener.
-            Browse_git
         def start(self, initial_delay:Â intÂ =Â 0) ->Â None
-            Feature: FeatureName.PushUpdates, Supported by: Protocol.DMAP,
-            Protocol.MRP, Protocol.RAOP
+            Feature: FeatureName.PushUpdates, Supported by:
             Begin to listen to updates.
             If an error occurs, start must be called again.
             Browse_git
         def stop(self) ->Â None
             No longer forward updates to listener.
             Browse_git
   class RemoteControl
@@ -743,15 +738,15 @@
         async def next(self) ->Â None
             Feature: FeatureName.Next, Supported by: Protocol.Companion,
             Protocol.DMAP, Protocol.MRP
             Press key next.
             Browse_git
         async def pause(self) ->Â None
             Feature: FeatureName.Pause, Supported by: Protocol.Companion,
-            Protocol.DMAP, Protocol.MRP
+            Protocol.DMAP, Protocol.MRP, Protocol.RAOP
             Press key play.
             Browse_git
         async def play(self) ->Â None
             Feature: FeatureName.Play, Supported by: Protocol.Companion,
             Protocol.DMAP, Protocol.MRP
             Press key play.
             Browse_git
```

### Comparing `pyatv-0.9.7/docs/api/pyatv.html` & `pyatv-0.9.8/docs/api/pyatv.html`

 * *Files 7% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 </nav>
 <article id="content">
 <header>
 <h1 class="title">Module <code>pyatv</code></h1>
 </header>
 <section id="section-intro">
 <p>Main routines for interacting with an Apple TV.</p>
-<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/__init__.py#L1-L131" class="git-link">Browse git</a></div>
+<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/__init__.py#L1-L139" class="git-link">Browse git</a></div>
 </section>
 <section>
 <h2 class="section-title" id="header-submodules">Sub-modules</h2>
 <dl>
 <dt><code class="name"><a title="pyatv.conf" href="conf">pyatv.conf</a></code></dt>
 <dd>
 <section class="desc"><p>Configuration used when connecting to a device …</p></section>
@@ -74,33 +74,33 @@
 <dt id="pyatv.connect">
 <code class="name flex">
 <span>async def <span class="ident">connect</span></span>(<span>config: <a title="pyatv.interface.BaseConfig" href="interface#pyatv.interface.BaseConfig">BaseConfig</a>, loop: asyncio.events.AbstractEventLoop, protocol: <a title="pyatv.const.Protocol" href="const#pyatv.const.Protocol">Protocol</a> = None, session: aiohttp.client.ClientSession = None) -> <a title="pyatv.interface.AppleTV" href="interface#pyatv.interface.AppleTV">AppleTV</a></span>
 </code>
 </dt>
 <dd>
 <section class="desc"><p>Connect to a device based on a configuration.</p></section>
-<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/__init__.py#L70-L107" class="git-link">Browse git</a></div>
+<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/__init__.py#L71-L115" class="git-link">Browse git</a></div>
 </dd>
 <dt id="pyatv.pair">
 <code class="name flex">
 <span>async def <span class="ident">pair</span></span>(<span>config: <a title="pyatv.interface.BaseConfig" href="interface#pyatv.interface.BaseConfig">BaseConfig</a>, protocol: <a title="pyatv.const.Protocol" href="const#pyatv.const.Protocol">Protocol</a>, loop: asyncio.events.AbstractEventLoop, session: aiohttp.client.ClientSession = None, **kwargs)</span>
 </code>
 </dt>
 <dd>
 <section class="desc"><p>Pair a protocol for an Apple TV.</p></section>
-<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/__init__.py#L110-L131" class="git-link">Browse git</a></div>
+<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/__init__.py#L118-L139" class="git-link">Browse git</a></div>
 </dd>
 <dt id="pyatv.scan">
 <code class="name flex">
 <span>async def <span class="ident">scan</span></span>(<span>loop: asyncio.events.AbstractEventLoop, timeout: int = 5, identifier: Union[str, Set[str], None] = None, protocol: Union[<a title="pyatv.const.Protocol" href="const#pyatv.const.Protocol">Protocol</a>, Set[<a title="pyatv.const.Protocol" href="const#pyatv.const.Protocol">Protocol</a>], None] = None, hosts: List[str] = None) -> List[<a title="pyatv.interface.BaseConfig" href="interface#pyatv.interface.BaseConfig">BaseConfig</a>]</span>
 </code>
 </dt>
 <dd>
 <section class="desc"><p>Scan for Apple TVs on network and return their configurations.</p></section>
-<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/__init__.py#L23-L67" class="git-link">Browse git</a></div>
+<div class="git-link-div"><a href="https://github.com/postlund/pyatv/blob/master/pyatv/__init__.py#L24-L68" class="git-link">Browse git</a></div>
 </dd>
 </dl>
 </section>
 <section>
 </section>
 </article>
 <footer id="footer">
```

### Comparing `pyatv-0.9.7/docs/assets/css/hljs.css` & `pyatv-0.9.8/docs/assets/css/hljs.css`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/docs/assets/css/normalize.css` & `pyatv-0.9.8/docs/assets/css/normalize.css`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/docs/assets/css/pdoc.css` & `pyatv-0.9.8/docs/assets/css/pdoc.css`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/docs/assets/css/sanitize.css` & `pyatv-0.9.8/docs/assets/css/sanitize.css`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/docs/assets/img/logo.svg` & `pyatv-0.9.8/docs/assets/img/logo.svg`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/docs/assets/js/highlight.9.12.0.min.js` & `pyatv-0.9.8/docs/assets/js/highlight.9.12.0.min.js`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/docs/assets/js/mermaid.8.9.2.min.js` & `pyatv-0.9.8/docs/assets/js/mermaid.8.9.2.min.js`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/docs/assets/js/mermaid.min.js.map` & `pyatv-0.9.8/docs/assets/js/mermaid.min.js.map`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/docs/development/apps.md` & `pyatv-0.9.8/docs/development/apps.md`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/docs/development/audio.md` & `pyatv-0.9.8/docs/development/audio.md`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/docs/development/control.md` & `pyatv-0.9.8/docs/development/control.md`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/docs/development/device_info.md` & `pyatv-0.9.8/docs/development/device_info.md`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/docs/development/examples.md` & `pyatv-0.9.8/docs/development/examples.md`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/docs/development/features.md` & `pyatv-0.9.8/docs/development/features.md`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/docs/development/listeners.md` & `pyatv-0.9.8/docs/development/listeners.md`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/docs/development/logging.md` & `pyatv-0.9.8/docs/development/logging.md`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/docs/development/metadata.md` & `pyatv-0.9.8/docs/development/metadata.md`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/docs/development/power_management.md` & `pyatv-0.9.8/docs/development/power_management.md`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/docs/development/scan_pair_and_connect.md` & `pyatv-0.9.8/docs/development/scan_pair_and_connect.md`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/docs/development/stream.md` & `pyatv-0.9.8/docs/development/stream.md`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/docs/documentation/atvlog.md` & `pyatv-0.9.8/docs/documentation/atvlog.md`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/docs/documentation/atvproxy.md` & `pyatv-0.9.8/docs/documentation/atvproxy.md`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/docs/documentation/atvremote.md` & `pyatv-0.9.8/docs/documentation/atvremote.md`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/docs/documentation/atvscript.md` & `pyatv-0.9.8/docs/documentation/atvscript.md`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/docs/documentation/concepts.md` & `pyatv-0.9.8/docs/documentation/concepts.md`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/docs/documentation/documentation.md` & `pyatv-0.9.8/docs/documentation/documentation.md`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/docs/documentation/getting_started.md` & `pyatv-0.9.8/docs/documentation/getting_started.md`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/docs/documentation/protocols.md` & `pyatv-0.9.8/docs/documentation/protocols.md`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/docs/documentation/supported_features.md` & `pyatv-0.9.8/docs/documentation/supported_features.md`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/docs/documentation/tutorial.md` & `pyatv-0.9.8/docs/documentation/tutorial.md`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/docs/favicon.ico` & `pyatv-0.9.8/docs/favicon.ico`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/docs/index.md` & `pyatv-0.9.8/docs/index.md`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/docs/internals/design.md` & `pyatv-0.9.8/docs/internals/design.md`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/docs/internals/documentation.md` & `pyatv-0.9.8/docs/internals/documentation.md`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/docs/internals/interfaces.md` & `pyatv-0.9.8/docs/internals/interfaces.md`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/docs/internals/internals.md` & `pyatv-0.9.8/docs/internals/internals.md`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/docs/internals/submit_pr.md` & `pyatv-0.9.8/docs/internals/submit_pr.md`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/docs/internals/testing.md` & `pyatv-0.9.8/docs/internals/testing.md`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/docs/internals/tools.md` & `pyatv-0.9.8/docs/internals/tools.md`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/docs/pdoc_templates/config.mako` & `pyatv-0.9.8/docs/pdoc_templates/config.mako`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/docs/pdoc_templates/html.mako` & `pyatv-0.9.8/docs/pdoc_templates/html.mako`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/docs/support/acknowledgements.md` & `pyatv-0.9.8/docs/support/acknowledgements.md`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/docs/support/faq.md` & `pyatv-0.9.8/docs/support/faq.md`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/docs/support/migration.md` & `pyatv-0.9.8/docs/support/migration.md`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/docs/support/scanning_issues.md` & `pyatv-0.9.8/docs/support/scanning_issues.md`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/docs/support/support.md` & `pyatv-0.9.8/docs/support/support.md`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/docs/support/troubleshooting.md` & `pyatv-0.9.8/docs/support/troubleshooting.md`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/examples/connect_with_credentials.py` & `pyatv-0.9.8/examples/connect_with_credentials.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/examples/manual_connect.py` & `pyatv-0.9.8/examples/manual_connect.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/examples/pairing.py` & `pyatv-0.9.8/examples/pairing.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/examples/play_url.py` & `pyatv-0.9.8/examples/play_url.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/examples/scan_and_connect.py` & `pyatv-0.9.8/examples/scan_and_connect.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/examples/stream.py` & `pyatv-0.9.8/examples/stream.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/examples/tutorial.py` & `pyatv-0.9.8/examples/tutorial.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/__init__.py` & `pyatv-0.9.8/pyatv/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import logging
 from typing import List, Optional, Set, Union
 
 import aiohttp
 
 from pyatv import exceptions, interface
 from pyatv.const import Protocol
+from pyatv.core import CoreStateDispatcher, ProtocolStateDispatcher
 from pyatv.core.facade import FacadeAppleTV
 from pyatv.core.scan import BaseScanner, MulticastMdnsScanner, UnicastMdnsScanner
 from pyatv.protocols import PROTOCOLS
 from pyatv.support import http
 
 _LOGGER = logging.getLogger(__name__)
 
@@ -78,28 +79,35 @@
         raise exceptions.NoServiceError("no service to connect to")
 
     if config.identifier is None:
         raise exceptions.DeviceIdMissingError("no device identifier")
 
     config_copy = deepcopy(config)
     session_manager = await http.create_session(session)
-    atv = FacadeAppleTV(config_copy, session_manager)
+    core_dispatcher = CoreStateDispatcher()
+    atv = FacadeAppleTV(config_copy, session_manager, core_dispatcher)
 
     try:
         for proto, proto_methods in PROTOCOLS.items():
             service = config_copy.get_service(proto)
             if service is None or not service.enabled:
                 continue
 
             # Lock protocol argument so protocol does not have to deal
             # with that
             takeover_method = partial(atv.takeover, proto)
 
             for setup_data in proto_methods.setup(
-                loop, config_copy, service, atv, session_manager, takeover_method
+                loop,
+                config_copy,
+                service,
+                atv,
+                session_manager,
+                takeover_method,
+                ProtocolStateDispatcher(proto, core_dispatcher),
             ):
                 atv.add_protocol(setup_data)
 
         await atv.connect()
     except Exception:
         await session_manager.close()
         raise
```

### Comparing `pyatv-0.9.7/pyatv/auth/hap_channel.py` & `pyatv-0.9.8/pyatv/auth/hap_channel.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/auth/hap_pairing.py` & `pyatv-0.9.8/pyatv/auth/hap_pairing.py`

 * *Files 4% similar despite different names*

```diff
@@ -104,15 +104,15 @@
     """Verify if credentials are valid and derive encryption keys."""
 
     async def verify_credentials(self) -> bool:
         """Verify if credentials are valid and returns True if keys are generated."""
 
     def encryption_keys(
         self, salt: str, output_info: str, input_info: str
-    ) -> Tuple[str, str]:
+    ) -> Tuple[bytes, bytes]:
         """Return derived encryption keys."""
 
 
 NO_CREDENTIALS = HapCredentials()
 TRANSIENT_CREDENTIALS = HapCredentials(b"transient")
```

### Comparing `pyatv-0.9.7/pyatv/auth/hap_session.py` & `pyatv-0.9.8/pyatv/auth/hap_session.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/auth/hap_srp.py` & `pyatv-0.9.8/pyatv/auth/hap_srp.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """SRP implementation for HAP."""
 
 import binascii
 import hashlib
 import logging
 import os
+from typing import Tuple
 import uuid
 
 from cryptography.exceptions import InvalidSignature
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import hashes, serialization
 from cryptography.hazmat.primitives.asymmetric.ed25519 import (
     Ed25519PrivateKey,
@@ -24,15 +25,15 @@
 from pyatv.auth.hap_pairing import HapCredentials
 from pyatv.auth.hap_tlv8 import TlvValue, read_tlv, write_tlv
 from pyatv.support import chacha20, log_binary
 
 _LOGGER = logging.getLogger(__name__)
 
 
-def hkdf_expand(salt, info, shared_secret):
+def hkdf_expand(salt: str, info: str, shared_secret: bytes) -> bytes:
     """Derive encryption keys from shared secret."""
     hkdf = HKDF(
         algorithm=hashes.SHA512(),
         length=32,
         salt=salt.encode(),
         info=info.encode(),
         backend=default_backend(),
@@ -118,15 +119,17 @@
                 TlvValue.Identifier: credentials.client_id,
                 TlvValue.Signature: device_signature,
             }
         )
 
         return chacha.encrypt(tlv, nounce="PV-Msg03".encode())
 
-    def verify2(self, salt, output_info, input_info):
+    def verify2(
+        self, salt: str, output_info: str, input_info: str
+    ) -> Tuple[bytes, bytes]:
         """Last verification step.
 
         The derived keys (output, input) are returned here.
         """
         output_key = hkdf_expand(salt, output_info, self._shared)
         input_key = hkdf_expand(salt, input_info, self._shared)
         log_binary(_LOGGER, "Keys", Output=output_key, Input=input_key)
```

### Comparing `pyatv-0.9.7/pyatv/auth/hap_tlv8.py` & `pyatv-0.9.8/pyatv/auth/hap_tlv8.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/conf.py` & `pyatv-0.9.8/pyatv/conf.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/const.py` & `pyatv-0.9.8/pyatv/const.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Constants used in the public API."""
 # pylint: disable=invalid-name
 
 from enum import Enum
 
 MAJOR_VERSION = "0"
 MINOR_VERSION = "9"
-PATCH_VERSION = "7"
+PATCH_VERSION = "8"
 __short_version__ = f"{MAJOR_VERSION}.{MINOR_VERSION}"
 __version__ = f"{__short_version__}.{PATCH_VERSION}"
 
 
 class Protocol(Enum):
     """All supported protocols."""
```

### Comparing `pyatv-0.9.7/pyatv/convert.py` & `pyatv-0.9.8/pyatv/convert.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/core/facade.py` & `pyatv-0.9.8/pyatv/core/facade.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,18 +13,25 @@
 import asyncio
 import io
 import logging
 from queue import Queue
 from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Union, cast
 
 from pyatv import const, exceptions, interface
-from pyatv.const import FeatureName, FeatureState, InputAction, Protocol
-from pyatv.core import SetupData
+from pyatv.const import (
+    DeviceState,
+    FeatureName,
+    FeatureState,
+    InputAction,
+    PowerState,
+    Protocol,
+)
+from pyatv.core import CoreStateDispatcher, SetupData, StateMessage, UpdatedState
 from pyatv.core.relayer import Relayer
-from pyatv.support import deprecated
+from pyatv.support import deprecated, shield
 from pyatv.support.collections import dict_merge
 from pyatv.support.http import ClientSessionManager
 
 _LOGGER = logging.getLogger(__name__)
 
 DEFAULT_PRIORITIES = [
     Protocol.MRP,
@@ -39,154 +46,183 @@
     """Facade implementation for API used to control an Apple TV."""
 
     def __init__(self):
         """Initialize a new FacadeRemoteControl instance."""
         super().__init__(interface.RemoteControl, DEFAULT_PRIORITIES)
 
     # pylint: disable=invalid-name
+    @shield.guard
     async def up(self, action: InputAction = InputAction.SingleTap) -> None:
         """Press key up."""
         return await self.relay("up")(action=action)
 
+    @shield.guard
     async def down(self, action: InputAction = InputAction.SingleTap) -> None:
         """Press key down."""
         return await self.relay("down")(action=action)
 
+    @shield.guard
     async def left(self, action: InputAction = InputAction.SingleTap) -> None:
         """Press key left."""
         return await self.relay("left")(action=action)
 
+    @shield.guard
     async def right(self, action: InputAction = InputAction.SingleTap) -> None:
         """Press key right."""
         return await self.relay("right")(action=action)
 
+    @shield.guard
     async def play(self) -> None:
         """Press key play."""
         return await self.relay("play")()
 
+    @shield.guard
     async def play_pause(self) -> None:
         """Toggle between play and pause."""
         return await self.relay("play_pause")()
 
+    @shield.guard
     async def pause(self) -> None:
         """Press key play."""
         return await self.relay("pause")()
 
+    @shield.guard
     async def stop(self) -> None:
         """Press key stop."""
         return await self.relay("stop")()
 
+    @shield.guard
     async def next(self) -> None:
         """Press key next."""
         return await self.relay("next")()
 
+    @shield.guard
     async def previous(self) -> None:
         """Press key previous."""
         return await self.relay("previous")()
 
+    @shield.guard
     async def select(self, action: InputAction = InputAction.SingleTap) -> None:
         """Press key select."""
         return await self.relay("select")(action=action)
 
+    @shield.guard
     async def menu(self, action: InputAction = InputAction.SingleTap) -> None:
         """Press key menu."""
         return await self.relay("menu")(action=action)
 
     @deprecated
+    @shield.guard
     async def volume_up(self) -> None:
         """Press key volume up."""
         return await self.relay("volume_up")()
 
     @deprecated
+    @shield.guard
     async def volume_down(self) -> None:
         """Press key volume down."""
         return await self.relay("volume_down")()
 
+    @shield.guard
     async def home(self, action: InputAction = InputAction.SingleTap) -> None:
         """Press key home."""
         return await self.relay("home")(action=action)
 
+    @shield.guard
     async def home_hold(self) -> None:
         """Hold key home."""
         return await self.relay("home_hold")()
 
+    @shield.guard
     async def top_menu(self) -> None:
         """Go to main menu (long press menu)."""
         return await self.relay("top_menu")()
 
     @deprecated
+    @shield.guard
     async def suspend(self) -> None:
         """Suspend the device."""
         return await self.relay("suspend")()
 
     @deprecated
+    @shield.guard
     async def wakeup(self) -> None:
         """Wake up the device."""
         return await self.relay("wakeup")()
 
+    @shield.guard
     async def skip_forward(self) -> None:
         """Skip forward a time interval.
 
         Skip interval is typically 15-30s, but is decided by the app.
         """
         return await self.relay("skip_forward")()
 
+    @shield.guard
     async def skip_backward(self) -> None:
         """Skip backwards a time interval.
 
         Skip interval is typically 15-30s, but is decided by the app.
         """
         return await self.relay("skip_backward")()
 
+    @shield.guard
     async def set_position(self, pos: int) -> None:
         """Seek in the current playing media."""
         return await self.relay("set_position")(pos=pos)
 
+    @shield.guard
     async def set_shuffle(self, shuffle_state: const.ShuffleState) -> None:
         """Change shuffle mode to on or off."""
         return await self.relay("set_shuffle")(shuffle_state=shuffle_state)
 
+    @shield.guard
     async def set_repeat(self, repeat_state: const.RepeatState) -> None:
         """Change repeat state."""
         return await self.relay("set_repeat")(repeat_state=repeat_state)
 
 
 class FacadeMetadata(Relayer, interface.Metadata):
     """Facade implementation for retrieving metadata from an Apple TV."""
 
     def __init__(self):
         """Initialize a new FacadeMetadata instance."""
         super().__init__(interface.Metadata, DEFAULT_PRIORITIES)
 
-    @property
+    @property  # type: ignore
+    @shield.guard
     def device_id(self) -> Optional[str]:
         """Return a unique identifier for current device."""
         return self.relay("device_id")
 
+    @shield.guard
     async def artwork(self, width=512, height=None) -> Optional[interface.ArtworkInfo]:
         """Return artwork for what is currently playing (or None).
 
         The parameters "width" and "height" makes it possible to request artwork of a
         specific size. This is just a request, the device might impose restrictions and
         return artwork of a different size. Set both parameters to None to request
         default size. Set one of them and let the other one be None to keep original
         aspect ratio.
         """
         return await self.relay("artwork")(width=width, height=height)
 
-    @property
+    @property  # type: ignore
+    @shield.guard
     def artwork_id(self) -> str:
         """Return a unique identifier for current artwork."""
         return self.relay("artwork_id")
 
+    @shield.guard
     async def playing(self) -> interface.Playing:
         """Return what is currently playing."""
         return await self.relay("playing")()
 
-    @property
+    @property  # type: ignore
+    @shield.guard
     def app(self) -> Optional[interface.App]:
         """Return information about current app playing something.
 
         Do note that this property returns which app is currently playing something and
         not which app is currently active. If nothing is playing, the corresponding
         feature will be unavailable.
         """
@@ -214,14 +250,15 @@
                 # Add feature to map if missing OR replace if this protocol has higher
                 # priority than previous mapping
                 if feature not in self._feature_map or self._has_higher_priority(
                     protocol, self._feature_map[feature][0]
                 ):
                     self._feature_map[feature] = (protocol, instance)
 
+    @shield.guard
     def get_feature(self, feature_name: FeatureName) -> interface.FeatureInfo:
         """Return current state of a feature."""
         if feature_name == FeatureName.PushUpdates:
             # Multiple protocols can register a push updater implementation, but only
             # one of them will ever be used (i.e. relaying is not done on method
             # level). So if at least one push updater is available, then we can return
             # "Available" here.
@@ -247,40 +284,71 @@
         Protocol.Companion,
         Protocol.MRP,
         Protocol.DMAP,
         Protocol.AirPlay,
         Protocol.RAOP,
     ]
 
-    def __init__(self):
+    def __init__(self, core_dispatcher: CoreStateDispatcher):
         """Initialize a new FacadePower instance."""
         # This is border line, maybe need another structure to support this
         Relayer.__init__(self, interface.Power, DEFAULT_PRIORITIES)
         interface.Power.__init__(self)
+        self._is_playing: Optional[bool] = None
+        core_dispatcher.listen_to(
+            UpdatedState.Playing,
+            self._playing_changed,
+            message_filter=lambda message: message.protocol == self.main_protocol,
+        )
+
+    def _playing_changed(self, message: StateMessage) -> None:
+        """State of something changed."""
+        playing = cast(interface.Playing, message.value)
+
+        # Initially we must ask the protocol about power state so we don't send
+        # duplicate updates
+        if self._is_playing is None:
+            self._is_playing = self.relay("power_state") == PowerState.On
+
+        # Computer new state so we can know if we should update or not
+        old_state = self.power_state
+        self._is_playing = playing.device_state != DeviceState.Idle
+        new_state = self.power_state
+
+        # Do not update state in case it didn't change
+        if new_state != old_state:
+            self.listener.powerstate_update(old_state, new_state)
 
     def powerstate_update(
         self, old_state: const.PowerState, new_state: const.PowerState
     ):
         """Device power state was updated.
 
         Forward power state updates from protocol implementations to actual listener.
         """
-        self.listener.powerstate_update(old_state, new_state)
+        if not self._is_playing:
+            self.listener.powerstate_update(old_state, new_state)
 
-    @property
+    @property  # type: ignore
+    @shield.guard
     def power_state(self) -> const.PowerState:
         """Return device power state."""
+        # Override power state in case something is playing
+        if self._is_playing:
+            return const.PowerState.On
         return self.relay("power_state")
 
+    @shield.guard
     async def turn_on(self, await_new_state: bool = False) -> None:
         """Turn device on."""
         await self.relay("turn_on", priority=self.OVERRIDE_PRIORITIES)(
             await_new_state=await_new_state
         )
 
+    @shield.guard
     async def turn_off(self, await_new_state: bool = False) -> None:
         """Turn device off."""
         await self.relay("turn_off", priority=self.OVERRIDE_PRIORITIES)(
             await_new_state=await_new_state
         )
 
 
@@ -288,25 +356,28 @@
     """Facade implementation for stream functionality."""
 
     def __init__(self, features: interface.Features):
         """Initialize a new FacadeStream instance."""
         super().__init__(interface.Stream, DEFAULT_PRIORITIES)
         self._features = features
 
+    @shield.guard
     def close(self) -> None:
         """Close connection and release allocated resources."""
         self.relay("close")()
 
+    @shield.guard
     async def play_url(self, url: str, **kwargs) -> None:
         """Play media from an URL on the device."""
         if not self._features.in_state(FeatureState.Available, FeatureName.PlayUrl):
             raise exceptions.NotSupportedError("play_url is not supported")
 
         await self.relay("play_url")(url, **kwargs)
 
+    @shield.guard
     async def stream_file(self, file: Union[str, io.BufferedReader], **kwargs) -> None:
         """Stream local file to device.
 
         INCUBATING METHOD - MIGHT CHANGE IN THE FUTURE!
         """
         await self.relay("stream_file")(file, **kwargs)
 
@@ -314,46 +385,52 @@
 class FacadeApps(Relayer, interface.Apps):
     """Facade implementation for app handling."""
 
     def __init__(self):
         """Initialize a new FacadeApps instance."""
         super().__init__(interface.Apps, DEFAULT_PRIORITIES)
 
+    @shield.guard
     async def app_list(self) -> List[interface.App]:
         """Fetch a list of apps that can be launched."""
         return await self.relay("app_list")()
 
+    @shield.guard
     async def launch_app(self, bundle_id: str) -> None:
         """Launch an app based on bundle ID."""
         await self.relay("launch_app")(bundle_id)
 
 
 class FacadeAudio(Relayer, interface.Audio):
     """Facade implementation for audio functionality."""
 
     def __init__(self):
         """Initialize a new FacadeAudio instance."""
         super().__init__(interface.Audio, DEFAULT_PRIORITIES)
 
+    @shield.guard
     async def volume_up(self) -> None:
         """Press key volume up."""
         return await self.relay("volume_up")()
 
+    @shield.guard
     async def volume_down(self) -> None:
         """Press key volume down."""
         return await self.relay("volume_down")()
 
-    @property
+    @property  # type: ignore
+    @shield.guard
     def volume(self) -> float:
         """Return current volume level."""
         volume = self.relay("volume")
         if 0.0 <= volume <= 100.0:
             return volume
         raise exceptions.ProtocolError(f"volume {volume} is out of range")
 
+    @shield.guard
     async def set_volume(self, level: float) -> None:
         """Change current volume level."""
         if 0.0 <= level <= 100.0:
             await self.relay("set_volume")(level)
         else:
             raise exceptions.ProtocolError(f"volume {level} is out of range")
 
@@ -368,30 +445,33 @@
 
     def __init__(self):
         """Initialize a new PushUpdater."""
         # TODO: python 3.6 seems to have problem with this sometimes
         Relayer.__init__(  # pylint: disable=non-parent-init-called
             self, interface.PushUpdater, DEFAULT_PRIORITIES
         )
-        interface.PushUpdater.__init__(self, asyncio.get_event_loop())
+        interface.PushUpdater.__init__(self)
 
-    @property
+    @property  # type: ignore
+    @shield.guard
     def active(self) -> bool:
         """Return if push updater has been started."""
         return self.relay("active")
 
+    @shield.guard
     def start(self, initial_delay: int = 0) -> None:
         """Begin to listen to updates.
 
         If an error occurs, start must be called again.
         """
         for instance in self.instances:
             instance.listener = self
             instance.start(initial_delay)
 
+    @shield.guard
     def stop(self) -> None:
         """No longer forward updates to listener."""
         for instance in self.instances:
             instance.listener = None
             instance.stop()
 
     def playstatus_update(self, updater, playstatus: interface.Playing) -> None:
@@ -405,15 +485,18 @@
             self.listener.playstatus_error(updater, exception)
 
 
 class FacadeAppleTV(interface.AppleTV):
     """Facade implementation of the external interface."""
 
     def __init__(
-        self, config: interface.BaseConfig, session_manager: ClientSessionManager
+        self,
+        config: interface.BaseConfig,
+        session_manager: ClientSessionManager,
+        core_dispatcher: CoreStateDispatcher,
     ):
         """Initialize a new FacadeAppleTV instance."""
         super().__init__(max_calls=1)  # To StateProducer via interface.AppleTV
         self._config = config
         self._session_manager = session_manager
         self._protocols_to_setup: Queue[SetupData] = Queue()
         self._protocol_handlers: Dict[Protocol, SetupData] = {}
@@ -421,33 +504,45 @@
         self._features = FacadeFeatures(self._push_updates)
         self._pending_tasks: Optional[set] = None
         self._device_info = interface.DeviceInfo({})
         self._interfaces = {
             interface.Features: self._features,
             interface.RemoteControl: FacadeRemoteControl(),
             interface.Metadata: FacadeMetadata(),
-            interface.Power: FacadePower(),
+            interface.Power: FacadePower(core_dispatcher),
             interface.PushUpdater: self._push_updates,
             interface.Stream: FacadeStream(self._features),
             interface.Apps: FacadeApps(),
             interface.Audio: FacadeAudio(),
         }
+        self._shield_everything()
+
+    def _shield_everything(self):
+        shield.shield(self)
+        for instance in self._interfaces.values():
+            shield.shield(instance)
+
+    def _block_everything(self):
+        shield.block(self)
+        for instance in self._interfaces.values():
+            shield.block(instance)
 
     def add_protocol(self, setup_data: SetupData):
         """Add a new protocol to the relay."""
         # Connecting commits current configuration, thus adding new protocols is not
         # allowed anymore after that
         if self._protocol_handlers:
             raise exceptions.InvalidStateError(
                 "cannot add protocol after connect was called"
             )
 
         _LOGGER.debug("Adding handler for protocol %s", setup_data.protocol)
         self._protocols_to_setup.put(setup_data)
 
+    @shield.guard
     async def connect(self) -> None:
         """Initiate connection to device."""
         # No protocols to setup + no protocols previously set up => no service
         if self._protocols_to_setup.empty() and not self._protocol_handlers:
             raise exceptions.NoServiceError("no service to connect to")
 
         # Protocols set up already => we have already connected
@@ -494,14 +589,18 @@
         if self._pending_tasks is not None:
             return self._pending_tasks
 
         self._pending_tasks = set()
         asyncio.ensure_future(self._session_manager.close())
         for setup_data in self._protocol_handlers.values():
             self._pending_tasks.update(setup_data.close())
+
+        # Block access to everything in the public interface
+        self._block_everything()
+
         return self._pending_tasks
 
     def takeover(self, protocol: Protocol, *interfaces: Any) -> Callable[[], None]:
         """Perform takeover of one of one or more protocol.
 
         Returns a function, that when called, returns the protocols taken over.
         """
@@ -525,65 +624,75 @@
                 _release()
                 raise
             else:
                 taken_over.append(relayer)
 
         return _release
 
-    @property
+    @property  # type: ignore
+    @shield.guard
     def device_info(self) -> interface.DeviceInfo:
         """Return API for device information."""
         return self._device_info
 
-    @property
+    @property  # type: ignore
+    @shield.guard
     def service(self) -> interface.BaseService:
         """Return main service used to connect to the Apple TV."""
         for protocol in DEFAULT_PRIORITIES:
             service = self._config.get_service(protocol)
             if service:
                 return service
 
         raise RuntimeError("no service (bug)")
 
-    @property
+    @property  # type: ignore
+    @shield.guard
     def remote_control(self) -> interface.RemoteControl:
         """Return API for controlling the Apple TV."""
         return cast(interface.RemoteControl, self._interfaces[interface.RemoteControl])
 
-    @property
+    @property  # type: ignore
+    @shield.guard
     def metadata(self) -> interface.Metadata:
         """Return API for retrieving metadata from the Apple TV."""
         return cast(interface.Metadata, self._interfaces[interface.Metadata])
 
-    @property
+    @property  # type: ignore
+    @shield.guard
     def push_updater(self) -> interface.PushUpdater:
         """Return API for handling push update from the Apple TV."""
         return cast(interface.PushUpdater, self._interfaces[interface.PushUpdater])
 
-    @property
+    @property  # type: ignore
+    @shield.guard
     def stream(self) -> interface.Stream:
         """Return API for streaming media."""
         return cast(interface.Stream, self._interfaces[interface.Stream])
 
-    @property
+    @property  # type: ignore
+    @shield.guard
     def power(self) -> interface.Power:
         """Return API for power management."""
         return cast(interface.Power, self._interfaces[interface.Power])
 
-    @property
+    @property  # type: ignore
+    @shield.guard
     def features(self) -> interface.Features:
         """Return features interface."""
         return cast(interface.Features, self._interfaces[interface.Features])
 
-    @property
+    @property  # type: ignore
+    @shield.guard
     def apps(self) -> interface.Apps:
         """Return apps interface."""
         return cast(interface.Apps, self._interfaces[interface.Apps])
 
-    @property
+    @property  # type: ignore
+    @shield.guard
     def audio(self) -> interface.Audio:
         """Return audio interface."""
         return cast(interface.Audio, self._interfaces[interface.Audio])
 
     def state_was_updated(self) -> None:
         """Call when state was updated.
```

### Comparing `pyatv-0.9.7/pyatv/core/mdns.py` & `pyatv-0.9.8/pyatv/core/mdns.py`

 * *Files 1% similar despite different names*

```diff
@@ -517,15 +517,15 @@
     await protocol.add_socket(net.mcast_socket(None, 5353))
 
     # One socket per local IP address
     for addr in net.get_private_addresses():
         try:
             await protocol.add_socket(net.mcast_socket(str(addr)))
         except Exception:  # pylint: disable=broad-except
-            _LOGGER.exception("failed to add listener for %s", addr)
+            _LOGGER.debug("Failed to add listener for %s (ignoring)", addr)
 
     return await typing.cast(MulticastDnsSdClientProtocol, protocol).get_response(
         timeout
     )
 
 
 async def publish(loop: asyncio.AbstractEventLoop, service: Service, zconf: Zeroconf):
```

### Comparing `pyatv-0.9.7/pyatv/core/protocol.py` & `pyatv-0.9.8/pyatv/core/protocol.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,38 @@
 """Generic functions for protocol logic."""
 import asyncio
+import inspect
 import logging
-from typing import Awaitable, Callable, Dict, Generic, List, Optional, TypeVar
+from typing import (
+    Awaitable,
+    Callable,
+    Dict,
+    Generic,
+    List,
+    Optional,
+    Tuple,
+    TypeVar,
+    Union,
+)
 
 _LOGGER = logging.getLogger(__name__)
 
 HEARTBEAT_INTERVAL = 30
 HEARTBEAT_RETRIES = 1  # One regular attempt + retries
 
 MessageType = TypeVar("MessageType")
 
 DispatchType = TypeVar("DispatchType")
 DispatchMessage = TypeVar("DispatchMessage")
-DispatchFunc = Callable[[DispatchMessage], Awaitable[None]]
+DispatchFunc = Callable[[DispatchMessage], Union[None, Awaitable[None]]]
+DispatchFilterFunc = Callable[[DispatchMessage], bool]
+
+
+def _no_filter(message: MessageType) -> bool:
+    return True
 
 
 async def heartbeater(
     name: str,
     sender_func: Callable[[Optional[MessageType]], Awaitable],
     finish_func: Callable[[], None] = lambda: None,
     failure_func: Callable[[Exception], None] = lambda exc: None,
@@ -60,19 +76,26 @@
 
 
 class MessageDispatcher(Generic[DispatchType, DispatchMessage]):
     """Dispatch message to listeners based on a type."""
 
     def __init__(self):
         """Initialize a new MessageDispatcher instance."""
-        self.__listeners: Dict[DispatchType, List[DispatchFunc]] = {}
-
-    def listen_to(self, dispatch_type: DispatchType, func: DispatchFunc) -> None:
+        self.__listeners: Dict[
+            DispatchType, List[Tuple[DispatchFilterFunc, DispatchFunc]]
+        ] = {}
+
+    def listen_to(
+        self,
+        dispatch_type: DispatchType,
+        func: DispatchFunc,
+        message_filter: DispatchFilterFunc = _no_filter,
+    ) -> None:
         """Listen to a specific type of message type."""
-        self.__listeners.setdefault(dispatch_type, []).append(func)
+        self.__listeners.setdefault(dispatch_type, []).append((message_filter, func))
 
     def dispatch(
         self, dispatch_type: DispatchType, message: DispatchMessage
     ) -> List[asyncio.Task]:
         """Dispatch a message to listeners."""
 
         async def _call_listener(func):
@@ -82,16 +105,20 @@
                 await func
             except asyncio.CancelledError:
                 pass
             except Exception:
                 _LOGGER.exception("error during dispatch")
 
         tasks = []
-        for func in self.__listeners.get(dispatch_type, []):
+        loop = asyncio.get_event_loop()
+        listeners = self.__listeners.get(dispatch_type, [])
+        for func in [func for filter_func, func in listeners if filter_func(message)]:
             _LOGGER.debug(
                 "Dispatching message with type %s to %s",
                 dispatch_type,
                 func,
             )
-            tasks.append(asyncio.ensure_future(_call_listener(func(message))))
-
+            if inspect.iscoroutinefunction(func):
+                tasks.append(asyncio.ensure_future(_call_listener(func(message))))
+            else:
+                loop.call_soon(func, message)
         return tasks
```

### Comparing `pyatv-0.9.7/pyatv/core/relayer.py` & `pyatv-0.9.8/pyatv/core/relayer.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,14 +58,22 @@
         """Return main instance based on priority."""
         for priority in chain(self._takeover_protocol, self._priorities):
             if priority in self._interfaces:
                 return self._interfaces[priority]
         raise exceptions.NotSupportedError()
 
     @property
+    def main_protocol(self) -> Optional[Protocol]:
+        """Return Protocol for main instance."""
+        for priority in chain(self._takeover_protocol, self._priorities):
+            if priority in self._interfaces:
+                return priority
+        return None
+
+    @property
     def instances(self) -> Sequence[T]:
         """Return all instances added to this relayer."""
         return list(self._interfaces.values())
 
     def register(self, instance: T, protocol: Protocol) -> None:
         """Register a new instance for an interface."""
         if protocol not in self._priorities:
```

### Comparing `pyatv-0.9.7/pyatv/core/scan.py` & `pyatv-0.9.8/pyatv/core/scan.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/exceptions.py` & `pyatv-0.9.8/pyatv/exceptions.py`

 * *Files 16% similar despite different names*

```diff
@@ -100,7 +100,16 @@
     def status_code(self) -> int:
         """Return status code that triggered the error."""
         return self._status_code
 
 
 class InvalidConfigError(Exception):
     """Thrown when something is wrong or missing in the config."""
+
+
+class BlockedStateError(Exception):
+    """Thrown when calling a blocked method.
+
+    Typically, public interface methods (e.g. any method available via the object
+    returned by `pyatv.connect`) becomes blocked after either calling close or because
+    the connection was closed for some other reason.
+    """
```

### Comparing `pyatv-0.9.7/pyatv/helpers.py` & `pyatv-0.9.8/pyatv/helpers.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/interface.py` & `pyatv-0.9.8/pyatv/interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -724,22 +724,19 @@
     def playstatus_error(self, updater, exception: Exception) -> None:
         """Inform about an error when updating play status."""
 
 
 class PushUpdater(ABC, StateProducer):
     """Base class for push/async updates from an Apple TV.
 
-    Listener interface: `pyatv.interface.PushListener`
-    """
+    A `pyatv.interface.PushUpdater` shall only publish update in case the state
+    actually changes.
 
-    def __init__(self, loop: asyncio.AbstractEventLoop):
-        """Initialize a new PushUpdater."""
-        super().__init__()
-        self.loop = loop
-        self._previous_state: Optional[Playing] = None
+    Listener interface: `pyatv.interface.PushListener`.
+    """
 
     @property
     @abstractmethod
     def active(self) -> bool:
         """Return if push updater has been started."""
         raise NotImplementedError
 
@@ -753,21 +750,14 @@
         raise NotImplementedError
 
     @abstractmethod
     def stop(self) -> None:
         """No longer forward updates to listener."""
         raise NotImplementedError
 
-    def post_update(self, playing: Playing) -> None:
-        """Post an update to listener."""
-        if playing != self._previous_state:
-            self.loop.call_soon(self.listener.playstatus_update, self, playing)
-
-        self._previous_state = playing
-
 
 class Stream:  # pylint: disable=too-few-public-methods
     """Base class for stream functionality."""
 
     def close(self) -> None:  # pylint: disable=no-self-use
         """Close connection and release allocated resources."""
         raise exceptions.NotSupportedError()
```

### Comparing `pyatv-0.9.7/pyatv/protocols/__init__.py` & `pyatv-0.9.8/pyatv/protocols/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 """Module containing all protocol logic."""
 import asyncio
 from typing import Any, Awaitable, Callable, Dict, Generator, Mapping, NamedTuple
 
 from pyatv import interface
 from pyatv.const import Protocol
-from pyatv.core import MutableService, SetupData, TakeoverMethod
+from pyatv.core import (
+    MutableService,
+    ProtocolStateDispatcher,
+    SetupData,
+    TakeoverMethod,
+)
 from pyatv.core.scan import ScanMethod
 from pyatv.interface import BaseService, DeviceInfo
 from pyatv.protocols import airplay as airplay_proto
 from pyatv.protocols import companion as companion_proto
 from pyatv.protocols import dmap as dmap_proto
 from pyatv.protocols import mrp as mrp_proto
 from pyatv.protocols import raop as raop_proto
@@ -19,14 +24,15 @@
     [
         asyncio.AbstractEventLoop,
         interface.BaseConfig,
         interface.BaseService,
         StateProducer,
         ClientSessionManager,
         TakeoverMethod,
+        ProtocolStateDispatcher,
     ],
     Generator[SetupData, None, None],
 ]
 PairMethod = Callable[..., interface.PairingHandler]
 DeviceInfoMethod = Callable[[str, Mapping[str, Any]], Dict[str, Any]]
 ServiceInfoMethod = Callable[
     [MutableService, DeviceInfo, Mapping[Protocol, BaseService]], Awaitable[None]
```

### Comparing `pyatv-0.9.7/pyatv/protocols/airplay/__init__.py` & `pyatv-0.9.8/pyatv/protocols/airplay/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,21 @@
 import logging
 import os
 from typing import Any, Dict, Generator, Mapping, Optional, Set
 
 from pyatv import exceptions
 from pyatv.auth.hap_pairing import AuthenticationType, HapCredentials, parse_credentials
 from pyatv.const import DeviceModel, FeatureName, PairingRequirement, Protocol
-from pyatv.core import MutableService, SetupData, TakeoverMethod, mdns
+from pyatv.core import (
+    MutableService,
+    ProtocolStateDispatcher,
+    SetupData,
+    TakeoverMethod,
+    mdns,
+)
 from pyatv.core.scan import ScanHandler, ScanHandlerReturn
 from pyatv.helpers import get_unique_id
 from pyatv.interface import (
     BaseConfig,
     BaseService,
     DeviceInfo,
     FeatureInfo,
@@ -182,14 +188,15 @@
 def setup(  # pylint: disable=too-many-locals
     loop: asyncio.AbstractEventLoop,
     config: BaseConfig,
     service: BaseService,
     device_listener: StateProducer,
     session_manager: ClientSessionManager,
     takeover: TakeoverMethod,
+    state_dispatcher: ProtocolStateDispatcher,
 ) -> Generator[SetupData, None, None]:
     """Set up a new AirPlay service."""
     # TODO: Split up in connect/protocol and Stream implementation
     stream = AirPlayStream(config, service)
 
     interfaces = {
         Features: AirPlayFeatures(service),
@@ -214,15 +221,15 @@
         interfaces,
         set([FeatureName.PlayUrl]),
     )
 
     credentials = extract_credentials(service)
 
     # Set up remote control channel if it is supported
-    if not is_remote_control_supported(service):
+    if not is_remote_control_supported(service, credentials):
         _LOGGER.debug("Remote control not supported by device")
     elif credentials.type not in [AuthenticationType.HAP, AuthenticationType.Transient]:
         _LOGGER.debug("%s not supported by remote control channel", credentials.type)
     else:
         _LOGGER.debug("Remote control channel is supported")
 
         control = RemoteControl(device_listener)
@@ -230,15 +237,14 @@
 
         # A protocol requires its correaponding service to function, so add a
         # dummy one if we don't have one yet
         mrp_service = config.get_service(Protocol.MRP)
         if mrp_service is None:
             mrp_service = MutableService(None, Protocol.MRP, 0, {})
             config.add_service(mrp_service)
-        mrp_service.enabled = False
 
         (
             _,
             mrp_connect,
             mrp_close,
             mrp_device_info,
             mrp_interfaces,
@@ -246,14 +252,15 @@
         ) = mrp.create_with_connection(
             loop,
             config,
             mrp_service,
             device_listener,
             session_manager,
             takeover,
+            state_dispatcher,
             AirPlayMrpConnection(control, device_listener),
             requires_heatbeat=False,  # Already have heartbeat on control channel
         )
 
         async def _connect_rc() -> bool:
             try:
```

### Comparing `pyatv-0.9.7/pyatv/protocols/airplay/auth/__init__.py` & `pyatv-0.9.8/pyatv/protocols/airplay/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/airplay/auth/hap.py` & `pyatv-0.9.8/pyatv/protocols/airplay/auth/hap.py`

 * *Files 4% similar despite different names*

```diff
@@ -131,10 +131,10 @@
         headers["Content-Type"] = "application/octet-stream"
         return await self.http.post(
             "/pair-verify", body=hap_tlv8.write_tlv(data), headers=headers
         )
 
     def encryption_keys(
         self, salt: str, output_info: str, input_info: str
-    ) -> Tuple[str, str]:
+    ) -> Tuple[bytes, bytes]:
         """Return derived encryption keys."""
         return self.srp.verify2(salt, output_info, input_info)
```

### Comparing `pyatv-0.9.7/pyatv/protocols/airplay/auth/hap_transient.py` & `pyatv-0.9.8/pyatv/protocols/airplay/auth/hap_transient.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/airplay/auth/legacy.py` & `pyatv-0.9.8/pyatv/protocols/airplay/auth/legacy.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,12 +104,12 @@
         headers = _AIRPLAY_HEADERS.copy()
         headers["Content-Type"] = "application/octet-stream"
         return await self.http.post("/pair-verify", headers=headers, body=data)
 
     @staticmethod
     def encryption_keys(
         salt: str, output_info: str, input_info: str
-    ) -> Tuple[str, str]:
+    ) -> Tuple[bytes, bytes]:
         """Return derived encryption keys."""
         raise exceptions.NotSupportedError(
             "encryption keys not supported by legacy auth"
         )
```

### Comparing `pyatv-0.9.7/pyatv/protocols/airplay/channels.py` & `pyatv-0.9.8/pyatv/protocols/airplay/channels.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/airplay/mrp_connection.py` & `pyatv-0.9.8/pyatv/protocols/airplay/mrp_connection.py`

 * *Files 14% similar despite different names*

```diff
@@ -33,14 +33,17 @@
         """Connect to device."""
         if self.remote_control.data_channel is None:
             raise exceptions.InvalidStateError("remote control channel not connected")
 
         self.data_channel = self.remote_control.data_channel
         self.data_channel.listener = self
 
+    def enable_encryption(self, output_key: bytes, input_key: bytes) -> None:
+        """Enable encryption with the specified keys."""
+
     @property
     def connected(self) -> bool:
         """If a connection is open or not."""
         return True
 
     def close(self) -> None:
         """Close connection to device."""
```

### Comparing `pyatv-0.9.7/pyatv/protocols/airplay/pairing.py` & `pyatv-0.9.8/pyatv/protocols/airplay/pairing.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/airplay/player.py` & `pyatv-0.9.8/pyatv/protocols/airplay/player.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/airplay/remote_control.py` & `pyatv-0.9.8/pyatv/protocols/airplay/remote_control.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/airplay/server_auth.py` & `pyatv-0.9.8/pyatv/protocols/airplay/server_auth.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/airplay/srp.py` & `pyatv-0.9.8/pyatv/protocols/airplay/srp.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/airplay/utils.py` & `pyatv-0.9.8/pyatv/protocols/airplay/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 """Manage announced AirPlay features."""
 from enum import IntFlag
 import re
 from typing import Mapping
 
+from pyatv.auth.hap_pairing import (
+    TRANSIENT_CREDENTIALS,
+    AuthenticationType,
+    HapCredentials,
+)
 from pyatv.const import PairingRequirement
 from pyatv.interface import BaseService
 
 # pylint: disable=invalid-name
 
 PASSWORD_BIT = 0x80
 LEGACY_PAIRING_BIT = 0x200
@@ -131,18 +136,23 @@
 
 
 # TODO: It is not fully understood how to determine if a device supports remote control
 # over AirPlay, so this method makes a pure guess. We know that Apple TVs running tvOS
 # X (X>=13?) support it as well as HomePods, something we can identify from the model
 # string. This implementation should however be improved when it's properly known how
 # to check for support.
-def is_remote_control_supported(service: BaseService) -> bool:
+def is_remote_control_supported(
+    service: BaseService, credentials: HapCredentials
+) -> bool:
     """Return if device supports remote control tunneling."""
     model = service.properties.get("model", "")
+
+    # HomePod supports remote control but only with transient credentials
     if model.startswith("AudioAccessory"):
-        return True
+        return credentials == TRANSIENT_CREDENTIALS
 
     if not model.startswith("AppleTV"):
         return False
 
+    # tvOS must be at least version 13 and HAP credentials are required by Apple TV
     version = service.properties.get("osvers", "0.0").split(".", maxsplit=1)[0]
-    return float(version) >= 13.0
+    return float(version) >= 13.0 and credentials.type == AuthenticationType.HAP
```

### Comparing `pyatv-0.9.7/pyatv/protocols/companion/__init__.py` & `pyatv-0.9.8/pyatv/protocols/companion/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,21 @@
     DeviceModel,
     FeatureName,
     FeatureState,
     InputAction,
     PairingRequirement,
     Protocol,
 )
-from pyatv.core import MutableService, SetupData, TakeoverMethod, mdns
+from pyatv.core import (
+    MutableService,
+    ProtocolStateDispatcher,
+    SetupData,
+    TakeoverMethod,
+    mdns,
+)
 from pyatv.core.scan import ScanHandler, ScanHandlerReturn
 from pyatv.interface import (
     App,
     Apps,
     Audio,
     BaseConfig,
     BaseService,
@@ -371,14 +377,15 @@
 def setup(
     loop: asyncio.AbstractEventLoop,
     config: BaseConfig,
     service: BaseService,
     device_listener: StateProducer,
     session_manager: ClientSessionManager,
     takeover: TakeoverMethod,
+    state_dispatcher: ProtocolStateDispatcher,
 ) -> Generator[SetupData, None, None]:
     """Set up a new Companion service."""
     # Companion doesn't work without credentials, so don't setup if none exists
     if not service.credentials:
         _LOGGER.debug("Not adding Companion as credentials are missing")
         return None
```

### Comparing `pyatv-0.9.7/pyatv/protocols/companion/api.py` & `pyatv-0.9.8/pyatv/protocols/companion/api.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/companion/auth.py` & `pyatv-0.9.8/pyatv/protocols/companion/auth.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/companion/connection.py` & `pyatv-0.9.8/pyatv/protocols/companion/connection.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/companion/opack.py` & `pyatv-0.9.8/pyatv/protocols/companion/opack.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/companion/pairing.py` & `pyatv-0.9.8/pyatv/protocols/companion/pairing.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/companion/protocol.py` & `pyatv-0.9.8/pyatv/protocols/companion/protocol.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/companion/server_auth.py` & `pyatv-0.9.8/pyatv/protocols/companion/server_auth.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/dmap/__init__.py` & `pyatv-0.9.8/pyatv/protocols/dmap/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,22 @@
     MediaType,
     OperatingSystem,
     PairingRequirement,
     Protocol,
     RepeatState,
     ShuffleState,
 )
-from pyatv.core import MutableService, SetupData, TakeoverMethod, mdns
+from pyatv.core import (
+    AbstractPushUpdater,
+    MutableService,
+    ProtocolStateDispatcher,
+    SetupData,
+    TakeoverMethod,
+    mdns,
+)
 from pyatv.core.scan import ScanHandler, ScanHandlerReturn
 from pyatv.helpers import get_unique_id
 from pyatv.interface import (
     ArtworkInfo,
     Audio,
     BaseConfig,
     BaseService,
@@ -429,20 +436,22 @@
         return self.apple_tv.latest_hash
 
     async def playing(self):
         """Return current device state."""
         return await self.apple_tv.playstatus()
 
 
-class DmapPushUpdater(PushUpdater):
+class DmapPushUpdater(AbstractPushUpdater):
     """Implementation of API for handling push update from an Apple TV."""
 
-    def __init__(self, loop, apple_tv, listener):
+    def __init__(
+        self, apple_tv, state_dispatcher: ProtocolStateDispatcher, listener
+    ) -> None:
         """Initialize a new DmapPushUpdater instance."""
-        super().__init__(loop)
+        super().__init__(state_dispatcher)
         self._atv = apple_tv
         self._listener = weakref.ref(listener)
         self._future = None
         self._initial_delay = 0
 
     @property
     def active(self):
@@ -646,23 +655,24 @@
 def setup(  # pylint: disable=too-many-locals
     loop: asyncio.AbstractEventLoop,
     config: BaseConfig,
     service: BaseService,
     device_listener: StateProducer,
     session_manager: ClientSessionManager,
     takeover: TakeoverMethod,
+    state_dispatcher: ProtocolStateDispatcher,
 ) -> Generator[SetupData, None, None]:
     """Set up a new DMAP service."""
     daap_http = HttpSession(
         session_manager.session,
         f"http://{config.address}:{service.port}/",
     )
     requester = DaapRequester(daap_http, service.credentials)
     apple_tv = BaseDmapAppleTV(requester)
-    push_updater = DmapPushUpdater(loop, apple_tv, device_listener)
+    push_updater = DmapPushUpdater(apple_tv, state_dispatcher, device_listener)
     metadata = DmapMetadata(config.identifier, apple_tv)
     audio = DmapAudio(apple_tv)
 
     interfaces = {
         RemoteControl: DmapRemoteControl(apple_tv),
         Metadata: metadata,
         PushUpdater: push_updater,
```

### Comparing `pyatv-0.9.7/pyatv/protocols/dmap/daap.py` & `pyatv-0.9.8/pyatv/protocols/dmap/daap.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/dmap/pairing.py` & `pyatv-0.9.8/pyatv/protocols/dmap/pairing.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,46 +1,32 @@
 """Module used for pairing pyatv with a device."""
 
 import asyncio
 import hashlib
 from io import StringIO
-from ipaddress import IPv4Address, ip_address
+from ipaddress import IPv4Address
 import logging
 import random
 from typing import List, Optional
 
 from aiohttp import web
-import netifaces
 from zeroconf import Zeroconf
 
 from pyatv.core import mdns
 from pyatv.interface import BaseConfig, BaseService, PairingHandler
 from pyatv.protocols.dmap import tags
 from pyatv.support.http import ClientSessionManager
-from pyatv.support.net import unused_port
+from pyatv.support.net import get_private_addresses, unused_port
 
 _LOGGER = logging.getLogger(__name__)
 
 
-# Maybe replace with pyatv.net.get_local_address_reaching?
-def _get_private_ip_addresses():
-    for iface in netifaces.interfaces():
-        addresses = netifaces.ifaddresses(iface)
-        if netifaces.AF_INET not in addresses:
-            continue
-
-        for addr in addresses[netifaces.AF_INET]:
-            ipaddr = ip_address(addr["addr"])
-            if ipaddr.is_private and not ipaddr.is_loopback:
-                yield ipaddr
-
-
 def _get_zeroconf_addresses(addresses: Optional[List[str]]) -> List[IPv4Address]:
     if addresses is None:
-        return list(_get_private_ip_addresses())
+        return list(get_private_addresses(include_loopback=False))
 
     return [IPv4Address(address) for address in addresses]
 
 
 def _generate_random_guid():
     return hex(random.getrandbits(64)).upper()
```

### Comparing `pyatv-0.9.7/pyatv/protocols/dmap/parser.py` & `pyatv-0.9.8/pyatv/protocols/dmap/parser.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/dmap/tag_definitions.py` & `pyatv-0.9.8/pyatv/protocols/dmap/tag_definitions.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/dmap/tags.py` & `pyatv-0.9.8/pyatv/protocols/dmap/tags.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/__init__.py` & `pyatv-0.9.8/pyatv/protocols/mrp/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,22 @@
     OperatingSystem,
     PairingRequirement,
     PowerState,
     Protocol,
     RepeatState,
     ShuffleState,
 )
-from pyatv.core import MutableService, SetupData, TakeoverMethod, mdns
+from pyatv.core import (
+    AbstractPushUpdater,
+    MutableService,
+    ProtocolStateDispatcher,
+    SetupData,
+    TakeoverMethod,
+    mdns,
+)
 from pyatv.core.scan import ScanHandler, ScanHandlerReturn
 from pyatv.helpers import get_unique_id
 from pyatv.interface import (
     App,
     ArtworkInfo,
     Audio,
     BaseConfig,
@@ -258,24 +265,30 @@
         series_name=series_name(),
         season_number=season_number(),
         episode_number=episode_number(),
         content_identifier=content_identifier(),
     )
 
 
-async def _send_hid_key(protocol: MrpProtocol, key: str, action: InputAction) -> None:
+async def _send_hid_key(
+    protocol: MrpProtocol, key: str, action: InputAction, flush: bool = True
+) -> None:
     async def _do_press(keycode: Tuple[int, int], hold: bool):
         await protocol.send(messages.send_hid_event(keycode[0], keycode[1], True))
 
         if hold:
             # Hardcoded hold time for one second
             await asyncio.sleep(1)
 
         await protocol.send(messages.send_hid_event(keycode[0], keycode[1], False))
 
+        # Send and receive a generic message as some kind of "flush" mechanism
+        if flush:
+            await protocol.send_and_receive(messages.create(protobuf.GENERIC_MESSAGE))
+
     keycode = _KEY_LOOKUP.get(key)
     if not keycode:
         raise exceptions.NotSupportedError(f"unsupported key: {key}")
 
     if action == InputAction.SingleTap:
         await _do_press(keycode, False)
     elif action == InputAction.DoubleTap:
@@ -591,20 +604,25 @@
         if logical_device_count >= 1:
             return PowerState.On
         if logical_device_count == 0:
             return PowerState.Off
         return PowerState.Unknown
 
 
-class MrpPushUpdater(PushUpdater):
+class MrpPushUpdater(AbstractPushUpdater):
     """Implementation of API for handling push update from an Apple TV."""
 
-    def __init__(self, loop, metadata, psm):
+    def __init__(
+        self,
+        metadata: MrpMetadata,
+        psm: PlayerStateManager,
+        state_dispatcher: ProtocolStateDispatcher,
+    ) -> None:
         """Initialize a new MrpPushUpdater instance."""
-        super().__init__(loop)
+        super().__init__(state_dispatcher)
         self.metadata = metadata
         self.psm = psm
 
     @property
     def active(self):
         """Return if push updater has been started."""
         return self.psm.listener == self
@@ -719,21 +737,25 @@
 
         if self._volume != level:
             await asyncio.wait_for(self._volume_event.wait(), timeout=5.0)
 
     async def volume_up(self) -> None:
         """Increase volume by one step."""
         if self._volume < 100.0:
-            await _send_hid_key(self.protocol, "volume_up", InputAction.SingleTap)
+            await _send_hid_key(
+                self.protocol, "volume_up", InputAction.SingleTap, flush=False
+            )
             await asyncio.wait_for(self._volume_event.wait(), timeout=5.0)
 
     async def volume_down(self) -> None:
         """Decrease volume by one step."""
         if self._volume > 0.0:
-            await _send_hid_key(self.protocol, "volume_down", InputAction.SingleTap)
+            await _send_hid_key(
+                self.protocol, "volume_down", InputAction.SingleTap, flush=False
+            )
             await asyncio.wait_for(self._volume_event.wait(), timeout=5.0)
 
 
 class MrpFeatures(Features):
     """Implementation of API for supported feature functionality."""
 
     def __init__(self, config: BaseConfig, psm: PlayerStateManager, audio: MrpAudio):
@@ -874,25 +896,26 @@
 def create_with_connection(  # pylint: disable=too-many-locals
     loop: asyncio.AbstractEventLoop,
     config: BaseConfig,
     service: BaseService,
     device_listener: StateProducer,
     session_manager: ClientSessionManager,
     takeover: TakeoverMethod,
+    state_dispatcher: ProtocolStateDispatcher,
     connection: AbstractMrpConnection,
     requires_heatbeat: bool = True,
 ) -> SetupData:
     """Set up a new MRP service from a connection."""
     protocol = MrpProtocol(connection, SRPAuthHandler(), service)
     psm = PlayerStateManager(protocol)
 
     remote_control = MrpRemoteControl(loop, psm, protocol)
     metadata = MrpMetadata(protocol, psm, config.identifier)
     power = MrpPower(loop, protocol, remote_control)
-    push_updater = MrpPushUpdater(loop, metadata, psm)
+    push_updater = MrpPushUpdater(metadata, psm, state_dispatcher)
     audio = MrpAudio(protocol)
 
     interfaces = {
         RemoteControl: remote_control,
         Metadata: metadata,
         Power: power,
         PushUpdater: push_updater,
@@ -912,15 +935,15 @@
         return set()
 
     def _device_info() -> Dict[str, Any]:
         devinfo = device_info(list(scan().keys())[0], service.properties)
 
         # Extract build number from DEVICE_INFO_MESSAGE from device
         if protocol.device_info:
-            info = protocol.device_info.inner()
+            info = protocol.device_info.inner()  # type: ignore
             devinfo[DeviceInfo.BUILD_NUMBER] = info.systemBuildVersion
             if info.modelID:
                 devinfo[DeviceInfo.RAW_MODEL] = info.modelID
                 devinfo[DeviceInfo.MODEL] = lookup_model(info.modelID)
 
         return devinfo
 
@@ -945,23 +968,25 @@
 def setup(
     loop: asyncio.AbstractEventLoop,
     config: BaseConfig,
     service: BaseService,
     device_listener: StateProducer,
     session_manager: ClientSessionManager,
     takeover: TakeoverMethod,
+    state_dispatcher: ProtocolStateDispatcher,
 ) -> Generator[SetupData, None, None]:
     """Set up a new MRP service."""
     yield create_with_connection(
         loop,
         config,
         service,
         device_listener,
         session_manager,
         takeover,
+        state_dispatcher,
         MrpConnection(config.address, service.port, loop, atv=device_listener),
     )
 
 
 def pair(
     config: BaseConfig,
     service: BaseService,
```

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/auth.py` & `pyatv-0.9.8/pyatv/protocols/mrp/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,10 +111,10 @@
 
         # TODO: check status code
 
         return True
 
     def encryption_keys(
         self, salt: str, output_info: str, input_info: str
-    ) -> Tuple[str, str]:
+    ) -> Tuple[bytes, bytes]:
         """Return derived encryption keys."""
         return self.srp.verify2(salt, output_info, input_info)
```

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/connection.py` & `pyatv-0.9.8/pyatv/protocols/mrp/connection.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,14 +17,18 @@
 class AbstractMrpConnection(asyncio.Protocol, StateProducer):
     """Abstract base class for an MRP connection."""
 
     @abstractmethod
     async def connect(self) -> None:
         """Connect to device."""
 
+    @abstractmethod
+    def enable_encryption(self, output_key: bytes, input_key: bytes) -> None:
+        """Enable encryption with the specified keys."""
+
     @property
     @abstractmethod
     def connected(self) -> bool:
         """If a connection is open or not."""
 
     @abstractmethod
     def close(self) -> None:
@@ -82,15 +86,15 @@
     def eof_received(self):
         """Device sent EOF (no more data)."""
         _LOGGER.debug("%s Received EOF from server", self._log_str)
         if self._transport.can_write_eof():
             self._transport.write_eof()
         self._transport.close()
 
-    def enable_encryption(self, output_key, input_key):
+    def enable_encryption(self, output_key: bytes, input_key: bytes) -> None:
         """Enable encryption with the specified keys."""
         self._chacha = chacha20.Chacha20Cipher(output_key, input_key)
 
     @property
     def connected(self) -> bool:
         """If a connection is open or not."""
         return self._transport is not None
```

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/messages.py` & `pyatv-0.9.8/pyatv/protocols/mrp/messages.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,14 +132,24 @@
         + data
         + binascii.unhexlify(b"0000000000000001000000")
     )
 
     return message
 
 
+def send_button(usage_page, usage, button_down):
+    """Create a new SEND_BUTTON_EVENT_MESSAGE.."""
+    message = create(protobuf.SEND_BUTTON_EVENT_MESSAGE)
+    inner = message.inner()
+    inner.usagePage = usage_page
+    inner.usage = usage
+    inner.buttonDown = button_down
+    return message
+
+
 def command(cmd, **kwargs):
     """Playback command request."""
     message = create(protobuf.SEND_COMMAND_MESSAGE)
     send_command = message.inner()
     send_command.command = cmd
     for key, value in kwargs.items():
         setattr(send_command.options, key, value)
```

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/pairing.py` & `pyatv-0.9.8/pyatv/protocols/mrp/pairing.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/player_state.py` & `pyatv-0.9.8/pyatv/protocols/mrp/player_state.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/AudioFadeMessage_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/AudioFadeMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/AudioFadeMessage_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/AudioFadeMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/AudioFadeResponseMessage_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/AudioFadeResponseMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/AudioFadeResponseMessage_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/AudioFadeResponseMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/AudioFormatSettingsMessage_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/AudioFormatSettingsMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/AudioFormatSettingsMessage_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/AudioFormatSettingsMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/ClientUpdatesConfigMessage_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/ClientUpdatesConfigMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/ClientUpdatesConfigMessage_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/ClientUpdatesConfigMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/CommandInfo.proto` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/CommandInfo.proto`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/CommandInfo_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/CommandInfo_pb2.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/CommandInfo_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/CommandInfo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/CommandOptions.proto` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/CommandOptions.proto`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/CommandOptions_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/CommandOptions_pb2.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/CommandOptions_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/CommandOptions_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/Common.proto` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/Common.proto`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/Common_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/Common_pb2.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/Common_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/Common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/ContentItem.proto` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/ContentItem.proto`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/ContentItemMetadata.proto` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/ContentItemMetadata.proto`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/ContentItemMetadata_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/ContentItemMetadata_pb2.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/ContentItemMetadata_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/ContentItemMetadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/ContentItem_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/ContentItem_pb2.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/ContentItem_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/ContentItem_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/CryptoPairingMessage_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/CryptoPairingMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/CryptoPairingMessage_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/CryptoPairingMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/DeviceInfoMessage.proto` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/DeviceInfoMessage.proto`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/DeviceInfoMessage_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/DeviceInfoMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/DeviceInfoMessage_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/DeviceInfoMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/GenericMessage_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/GenericMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/GenericMessage_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/GenericMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/GetKeyboardSessionMessage_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/GetKeyboardSessionMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/GetKeyboardSessionMessage_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/GetKeyboardSessionMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/GetRemoteTextInputSessionMessage_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/GetRemoteTextInputSessionMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/GetRemoteTextInputSessionMessage_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/GetRemoteTextInputSessionMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/GetVolumeMessage_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/GetVolumeMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/GetVolumeMessage_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/GetVolumeMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/GetVolumeResultMessage_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/GetVolumeResultMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/GetVolumeResultMessage_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/GetVolumeResultMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/KeyboardMessage.proto` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/KeyboardMessage.proto`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/KeyboardMessage_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/KeyboardMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/KeyboardMessage_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/KeyboardMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/LanguageOption_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/LanguageOption_pb2.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/LanguageOption_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/LanguageOption_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/NotificationMessage_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/NotificationMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/NotificationMessage_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/NotificationMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/NowPlayingClient_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/NowPlayingClient_pb2.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/NowPlayingClient_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/NowPlayingClient_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/NowPlayingInfo.proto` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/NowPlayingInfo.proto`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/NowPlayingInfo_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/NowPlayingInfo_pb2.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/NowPlayingInfo_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/NowPlayingInfo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/NowPlayingPlayer_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/NowPlayingPlayer_pb2.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/NowPlayingPlayer_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/NowPlayingPlayer_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/OriginClientPropertiesMessage_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/OriginClientPropertiesMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/OriginClientPropertiesMessage_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/OriginClientPropertiesMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/Origin_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/Origin_pb2.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/Origin_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/Origin_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/PlaybackQueue.proto` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/PlaybackQueue.proto`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/PlaybackQueueCapabilities_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/PlaybackQueueCapabilities_pb2.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/PlaybackQueueCapabilities_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/PlaybackQueueCapabilities_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/PlaybackQueueContext_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/PlaybackQueueContext_pb2.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/PlaybackQueueContext_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/PlaybackQueueContext_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/PlaybackQueueRequestMessage.proto` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/PlaybackQueueRequestMessage.proto`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/PlaybackQueueRequestMessage_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/PlaybackQueueRequestMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/PlaybackQueueRequestMessage_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/PlaybackQueueRequestMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/PlaybackQueue_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/PlaybackQueue_pb2.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/PlaybackQueue_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/PlaybackQueue_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/PlayerClientPropertiesMessage_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/PlayerClientPropertiesMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/PlayerClientPropertiesMessage_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/PlayerClientPropertiesMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/PlayerPath_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/PlayerPath_pb2.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/PlayerPath_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/PlayerPath_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/ProtocolMessage.proto` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/ProtocolMessage.proto`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
     PLAYBACK_QUEUE_REQUEST_MESSAGE = 32;
     TRANSACTION_MESSAGE = 33;
     CRYPTO_PAIRING_MESSAGE = 34; 
     GAME_CONTROLLER_PROPERTIES_MESSAGE = 35;
     SET_READY_STATE_MESSAGE = 36;
     DEVICE_INFO_UPDATE_MESSAGE = 37;
     SET_CONNECTION_STATE_MESSAGE = 38;
-    SEND_BUTTON_EVENT = 39;
+    SEND_BUTTON_EVENT_MESSAGE = 39;
     SET_HILITE_MODE_MESSAGE = 40;
     WAKE_DEVICE_MESSAGE = 41;
     GENERIC_MESSAGE = 42;
     SEND_PACKED_VIRTUAL_TOUCH_EVENT_MESSAGE = 43;
     SEND_LYRICS_EVENT = 44;
     SET_NOW_PLAYING_CLIENT_MESSAGE = 46;
     SET_NOW_PLAYING_PLAYER_MESSAGE = 47;
```

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/ProtocolMessage_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/ProtocolMessage_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='pyatv/protocols/mrp/protobuf/ProtocolMessage.proto',
   package='',
   syntax='proto2',
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n2pyatv/protocols/mrp/protobuf/ProtocolMessage.proto\"\xe1\x14\n\tErrorCode\"\xd3\x14\n\x04\x45num\x12\x0b\n\x07NoError\x10\x00\x12\x10\n\x0cUnknownError\x10\x01\x12\x14\n\x10InvalidOperation\x10\x02\x12\x19\n\x15OperationNotPermitted\x10\x03\x12\x16\n\x12\x43lientDoesNotExist\x10\x04\x12\x16\n\x12OriginDoesNotExist\x10\x05\x12\x18\n\x14UnsupportedOperation\x10\x06\x12\x1a\n\x16\x46\x61iledToSetPickedRoute\x10\x07\x12 \n\x1c\x46\x61iledToRegisterCustomOrigin\x10\x08\x12\x1e\n\x1a\x46\x61iledToRemoveCustomOrigin\x10\t\x12&\n\"TheApplicationActivityDoesNotExist\x10\n\x12.\n*TheAppHasNotSetupABrowsableContentEndpoint\x10\x0b\x12\x41\n=TheRequestedBrowsableContentApiIsNotSupportedByTheApplication\x10\x0c\x12\x32\n.TheNotficationHasNotBeenWhitelistedByTheServer\x10\r\x12\x38\n4OperationRequiresAClientCallbackToHaveBeenRegistered\x10\x0e\x12:\n6OperationRequiresAClientDataSourceToHaveBeenRegistered\x10\x0f\x12\x35\n1RequestedDataIsOutOfDateAndShouldBeRequestedAgain\x10\x10\x12\x30\n,TheDevicesEnforcedVolumeLimitHasBeenExceeded\x10\x11\x12\x1b\n\x17VolumeValueIsOutOfRange\x10\x12\x12$\n VolumeIsAlreadyAtTheMaximumValue\x10\x13\x12\x18\n\x14VolumeIsAlreadyMuted\x10\x14\x12\"\n\x1eVoiceInputEndpointDoesNotExist\x10\x15\x12\x34\n0TheVoiceInputDeviceIsNotRegisteredOrDoesNotExist\x10\x16\x12\x15\n\x11\x45ncryptionFailure\x10\x17\x12\x18\n\x14\x45ndpointDoesNotExist\x10\x18\x12.\n*TheClientsApplicationCancelledTheOperation\x10\x19\x12\x18\n\x14TheOperationTimedOut\x10\x1a\x12*\n&TheSpecifiedPlayerPathObjectWasInvalid\x10\x1b\x12:\n6AddingOrRemovingDevicesFromTheAvOutputContextHasFailed\x10\x1c\x12,\n(CouldNotFindTheSpecifiedNowPlayingPlayer\x10\x1d\x12\'\n#TheSpecifiedContentItemDoesNotExist\x10\x1e\x12\x1f\n\x1bTheSpecifiedOffsetIsInvalid\x10\x1f\x12&\n\"TheSpecifiedOutputContextIsInvalid\x10 \x12\x32\n.OneOrMoreSpecifiedOutputDevicesAreNotGroupable\x10!\x12H\nDTheSpecifiedOutputContextDoesNotSupportAddingMoreThanOneOutputDevice\x10\"\x12,\n(CouldNotFindTheSpecifiedNowPlayingClient\x10#\x12P\nLEndpointVolumeControlIsOnlyPossibleIfTheEndpointIsPickedOrRemoteControllable\x10$\x12T\nPOutputDeviceVolumeControlIsOnlyPossibleIfTheEndpointIsPickedOrRemoteControllable\x10%\x12\"\n\x1e\x43oderMustSupportKeyValueCoding\x10&\x12$\n CouldNotFindTheGivenOutputdevice\x10\'\x12!\n\x1d\x46\x61iledToConnectToRemoteDevice\x10\x64\x12 \n\x1c\x41uthenticationTokenIsInvalid\x10\x65\x12\x33\n/RecordingSessionIsAlreadyInProgressOnThisDevice\x10\x66\x12$\n TheDeviceIsNotCurrentlyRecording\x10g\x12\x1c\n\x18TheClientHasDisconnected\x10h\x12\x1c\n\x18TheServerHasDisconnected\x10i\x12,\n(TheConnectionHasBeenCancelledByTheClient\x10j\x12\x34\n0PairingFunctionalityIsLockedDueToSecurityReasons\x10k\x12,\n(TheClientsOperatingSystemVersionIsTooOld\x10l\x12(\n$TheClientsApplicationVersionIsTooOld\x10m\x12\x18\n\x14TheDeviceIsNotPaired\x10n\x12?\n;ThePinPairingDialogWasRemovedByTheUserBeforePairingOccoured\x10o\x12@\n<ThePinPairingDialogWasRemovedByATimeoutBeforePairingOccoured\x10p\x12\x19\n\x15TheConnectionTimedout\x10q\x12\"\n\x1ePairingWithThisDeviceIsBlocked\x10r\x12\x1b\n\x17TheDeviceIsGoingToSleep\x10s\x12\x1d\n\x19\x43onnectionBlockedByServer\x10t\x12<\n8MravendpointWasDeallocatedWhileWaitingForDeviceToConnect\x10u\x12H\nCOutputContextModificationCausedADeviceToNoLongerBeAProxyGroupPlayer\x10\xc8\x01\x12\x44\n?OutputContextModificationCausedADeviceToBecomeAProxyGroupPlayer\x10\xc9\x01\x12\x37\n2OutputContextModificationRequestedNoTopologyChange\x10\xca\x01\x12\x16\n\x11OtherUnknownError\x10\xab\x02\"\xeb\x17\n\x0fProtocolMessage\x12#\n\x04type\x18\x01 \x01(\x0e\x32\x15.ProtocolMessage.Type\x12\x12\n\nidentifier\x18\x02 \x01(\t\x12\x1b\n\x13\x61uthenticationToken\x18\x03 \x01(\t\x12\"\n\terrorCode\x18\x04 \x01(\x0e\x32\x0f.ErrorCode.Enum\x12\x11\n\ttimestamp\x18\x05 \x01(\x04\x12\x18\n\x10\x65rrorDescription\x18N \x01(\t\x12\x18\n\x10uniqueIdentifier\x18U \x01(\t\"\x80\x16\n\x04Type\x12\x13\n\x0fUNKNOWN_MESSAGE\x10\x00\x12\x18\n\x14SEND_COMMAND_MESSAGE\x10\x01\x12\x1f\n\x1bSEND_COMMAND_RESULT_MESSAGE\x10\x02\x12\x15\n\x11GET_STATE_MESSAGE\x10\x03\x12\x15\n\x11SET_STATE_MESSAGE\x10\x04\x12\x17\n\x13SET_ARTWORK_MESSAGE\x10\x05\x12\x1f\n\x1bREGISTER_HID_DEVICE_MESSAGE\x10\x06\x12&\n\"REGISTER_HID_DEVICE_RESULT_MESSAGE\x10\x07\x12\x1a\n\x16SEND_HID_EVENT_MESSAGE\x10\x08\x12\x1b\n\x17SEND_HID_REPORT_MESSAGE\x10\t\x12$\n SEND_VIRTUAL_TOUCH_EVENT_MESSAGE\x10\n\x12\x18\n\x14NOTIFICATION_MESSAGE\x10\x0b\x12.\n*CONTENT_ITEMS_CHANGED_NOTIFICATION_MESSAGE\x10\x0c\x12\x17\n\x13\x44\x45VICE_INFO_MESSAGE\x10\x0f\x12!\n\x1d\x43LIENT_UPDATES_CONFIG_MESSAGE\x10\x10\x12\'\n#VOLUME_CONTROL_AVAILABILITY_MESSAGE\x10\x11\x12\x1b\n\x17GAME_CONTROLLER_MESSAGE\x10\x12\x12$\n REGISTER_GAME_CONTROLLER_MESSAGE\x10\x13\x12-\n)REGISTER_GAME_CONTROLLER_RESPONSE_MESSAGE\x10\x14\x12&\n\"UNREGISTER_GAME_CONTROLLER_MESSAGE\x10\x15\x12/\n+REGISTER_FOR_GAME_CONTROLLER_EVENTS_MESSAGE\x10\x16\x12\x14\n\x10KEYBOARD_MESSAGE\x10\x17\x12 \n\x1cGET_KEYBOARD_SESSION_MESSAGE\x10\x18\x12\x16\n\x12TEXT_INPUT_MESSAGE\x10\x19\x12#\n\x1fGET_VOICE_INPUT_DEVICES_MESSAGE\x10\x1a\x12,\n(GET_VOICE_INPUT_DEVICES_RESPONSE_MESSAGE\x10\x1b\x12\'\n#REGISTER_VOICE_INPUT_DEVICE_MESSAGE\x10\x1c\x12\x30\n,REGISTER_VOICE_INPUT_DEVICE_RESPONSE_MESSAGE\x10\x1d\x12\x1f\n\x1bSET_RECORDING_STATE_MESSAGE\x10\x1e\x12\x1c\n\x18SEND_VOICE_INPUT_MESSAGE\x10\x1f\x12\"\n\x1ePLAYBACK_QUEUE_REQUEST_MESSAGE\x10 \x12\x17\n\x13TRANSACTION_MESSAGE\x10!\x12\x1a\n\x16\x43RYPTO_PAIRING_MESSAGE\x10\"\x12&\n\"GAME_CONTROLLER_PROPERTIES_MESSAGE\x10#\x12\x1b\n\x17SET_READY_STATE_MESSAGE\x10$\x12\x1e\n\x1a\x44\x45VICE_INFO_UPDATE_MESSAGE\x10%\x12 \n\x1cSET_CONNECTION_STATE_MESSAGE\x10&\x12\x15\n\x11SEND_BUTTON_EVENT\x10\'\x12\x1b\n\x17SET_HILITE_MODE_MESSAGE\x10(\x12\x17\n\x13WAKE_DEVICE_MESSAGE\x10)\x12\x13\n\x0fGENERIC_MESSAGE\x10*\x12+\n\'SEND_PACKED_VIRTUAL_TOUCH_EVENT_MESSAGE\x10+\x12\x15\n\x11SEND_LYRICS_EVENT\x10,\x12\"\n\x1eSET_NOW_PLAYING_CLIENT_MESSAGE\x10.\x12\"\n\x1eSET_NOW_PLAYING_PLAYER_MESSAGE\x10/\x12\x16\n\x12GET_VOLUME_MESSAGE\x10\x31\x12\x1d\n\x19GET_VOLUME_RESULT_MESSAGE\x10\x32\x12\x16\n\x12SET_VOLUME_MESSAGE\x10\x33\x12\x1d\n\x19VOLUME_DID_CHANGE_MESSAGE\x10\x34\x12\x19\n\x15REMOVE_CLIENT_MESSAGE\x10\x35\x12\x19\n\x15REMOVE_PLAYER_MESSAGE\x10\x36\x12\x19\n\x15UPDATE_CLIENT_MESSAGE\x10\x37\x12\x1f\n\x1bUPDATE_CONTENT_ITEM_MESSAGE\x10\x38\x12\'\n#UPDATE_CONTENT_ITEM_ARTWORK_MESSAGE\x10\x39\x12\x19\n\x15UPDATE_PLAYER_MESSAGE\x10:\x12*\n&PROMPT_FOR_ROUTE_AUTHORIZATION_MESSAGE\x10;\x12\x33\n/PROMPT_FOR_ROUTE_AUTHORIZATION_RESPONSE_MESSAGE\x10<\x12.\n*PRESENT_ROUTE_AUTHORIZATION_STATUS_MESSAGE\x10=\x12+\n\'GET_VOLUME_CONTROL_CAPABILITIES_MESSAGE\x10>\x12\x32\n.GET_VOLUME_CONTROL_CAPABILITIES_RESULT_MESSAGE\x10?\x12\x32\n.VOLUME_CONTROL_CAPABILITIES_DID_CHANGE_MESSAGE\x10@\x12 \n\x1cUPDATE_OUTPUT_DEVICE_MESSAGE\x10\x41\x12!\n\x1dREMOVE_OUTPUT_DEVICES_MESSAGE\x10\x42\x12\x1d\n\x19REMOTE_TEXT_INPUT_MESSAGE\x10\x43\x12)\n%GET_REMOTE_TEXT_INPUT_SESSION_MESSAGE\x10\x44\x12\"\n\x1eREMOVE_OUTPUT_DEVICES_MESSAGE2\x10\x45\x12$\n PLAYBACK_SESSION_REQUEST_MESSAGE\x10\x46\x12%\n!PLAYBACK_SESSION_RESPONSE_MESSAGE\x10G\x12*\n&SET_DEFAULT_SUPPORTED_COMMANDS_MESSAGE\x10H\x12,\n(PLAYBACK_SESSION_MIGRATE_REQUEST_MESSAGE\x10I\x12-\n)PLAYBACK_SESSION_MIGRATE_RESPONSE_MESSAGE\x10J\x12*\n&PLAYBACK_SESSION_MIGRATE_BEGIN_MESSAGE\x10K\x12(\n$PLAYBACK_SESSION_MIGRATE_END_MESSAGE\x10L\x12)\n%UPDATE_ACTIVE_SYSTEM_ENDPOINT_MESSAGE\x10M\x12\x1e\n\x1aSET_DISCOVERY_MODE_MESSAGE\x10\x65\x12\x1d\n\x19UPDATE_END_POINTS_MESSAGE\x10\x66\x12\x1c\n\x18REMOVE_ENDPOINTS_MESSAGE\x10g\x12$\n PLAYER_CLIENT_PROPERTIES_MESSAGE\x10h\x12$\n ORIGIN_CLIENT_PROPERTIES_MESSAGE\x10i\x12\x16\n\x12\x41UDIO_FADE_MESSAGE\x10j\x12\x1f\n\x1b\x41UDIO_FADE_RESPONSE_MESSAGE\x10k*\x04\x08\x06\x10N*\x04\x08O\x10U*\x08\x08V\x10\x80\x80\x80\x80\x02'
+  serialized_pb=b'\n2pyatv/protocols/mrp/protobuf/ProtocolMessage.proto\"\xe1\x14\n\tErrorCode\"\xd3\x14\n\x04\x45num\x12\x0b\n\x07NoError\x10\x00\x12\x10\n\x0cUnknownError\x10\x01\x12\x14\n\x10InvalidOperation\x10\x02\x12\x19\n\x15OperationNotPermitted\x10\x03\x12\x16\n\x12\x43lientDoesNotExist\x10\x04\x12\x16\n\x12OriginDoesNotExist\x10\x05\x12\x18\n\x14UnsupportedOperation\x10\x06\x12\x1a\n\x16\x46\x61iledToSetPickedRoute\x10\x07\x12 \n\x1c\x46\x61iledToRegisterCustomOrigin\x10\x08\x12\x1e\n\x1a\x46\x61iledToRemoveCustomOrigin\x10\t\x12&\n\"TheApplicationActivityDoesNotExist\x10\n\x12.\n*TheAppHasNotSetupABrowsableContentEndpoint\x10\x0b\x12\x41\n=TheRequestedBrowsableContentApiIsNotSupportedByTheApplication\x10\x0c\x12\x32\n.TheNotficationHasNotBeenWhitelistedByTheServer\x10\r\x12\x38\n4OperationRequiresAClientCallbackToHaveBeenRegistered\x10\x0e\x12:\n6OperationRequiresAClientDataSourceToHaveBeenRegistered\x10\x0f\x12\x35\n1RequestedDataIsOutOfDateAndShouldBeRequestedAgain\x10\x10\x12\x30\n,TheDevicesEnforcedVolumeLimitHasBeenExceeded\x10\x11\x12\x1b\n\x17VolumeValueIsOutOfRange\x10\x12\x12$\n VolumeIsAlreadyAtTheMaximumValue\x10\x13\x12\x18\n\x14VolumeIsAlreadyMuted\x10\x14\x12\"\n\x1eVoiceInputEndpointDoesNotExist\x10\x15\x12\x34\n0TheVoiceInputDeviceIsNotRegisteredOrDoesNotExist\x10\x16\x12\x15\n\x11\x45ncryptionFailure\x10\x17\x12\x18\n\x14\x45ndpointDoesNotExist\x10\x18\x12.\n*TheClientsApplicationCancelledTheOperation\x10\x19\x12\x18\n\x14TheOperationTimedOut\x10\x1a\x12*\n&TheSpecifiedPlayerPathObjectWasInvalid\x10\x1b\x12:\n6AddingOrRemovingDevicesFromTheAvOutputContextHasFailed\x10\x1c\x12,\n(CouldNotFindTheSpecifiedNowPlayingPlayer\x10\x1d\x12\'\n#TheSpecifiedContentItemDoesNotExist\x10\x1e\x12\x1f\n\x1bTheSpecifiedOffsetIsInvalid\x10\x1f\x12&\n\"TheSpecifiedOutputContextIsInvalid\x10 \x12\x32\n.OneOrMoreSpecifiedOutputDevicesAreNotGroupable\x10!\x12H\nDTheSpecifiedOutputContextDoesNotSupportAddingMoreThanOneOutputDevice\x10\"\x12,\n(CouldNotFindTheSpecifiedNowPlayingClient\x10#\x12P\nLEndpointVolumeControlIsOnlyPossibleIfTheEndpointIsPickedOrRemoteControllable\x10$\x12T\nPOutputDeviceVolumeControlIsOnlyPossibleIfTheEndpointIsPickedOrRemoteControllable\x10%\x12\"\n\x1e\x43oderMustSupportKeyValueCoding\x10&\x12$\n CouldNotFindTheGivenOutputdevice\x10\'\x12!\n\x1d\x46\x61iledToConnectToRemoteDevice\x10\x64\x12 \n\x1c\x41uthenticationTokenIsInvalid\x10\x65\x12\x33\n/RecordingSessionIsAlreadyInProgressOnThisDevice\x10\x66\x12$\n TheDeviceIsNotCurrentlyRecording\x10g\x12\x1c\n\x18TheClientHasDisconnected\x10h\x12\x1c\n\x18TheServerHasDisconnected\x10i\x12,\n(TheConnectionHasBeenCancelledByTheClient\x10j\x12\x34\n0PairingFunctionalityIsLockedDueToSecurityReasons\x10k\x12,\n(TheClientsOperatingSystemVersionIsTooOld\x10l\x12(\n$TheClientsApplicationVersionIsTooOld\x10m\x12\x18\n\x14TheDeviceIsNotPaired\x10n\x12?\n;ThePinPairingDialogWasRemovedByTheUserBeforePairingOccoured\x10o\x12@\n<ThePinPairingDialogWasRemovedByATimeoutBeforePairingOccoured\x10p\x12\x19\n\x15TheConnectionTimedout\x10q\x12\"\n\x1ePairingWithThisDeviceIsBlocked\x10r\x12\x1b\n\x17TheDeviceIsGoingToSleep\x10s\x12\x1d\n\x19\x43onnectionBlockedByServer\x10t\x12<\n8MravendpointWasDeallocatedWhileWaitingForDeviceToConnect\x10u\x12H\nCOutputContextModificationCausedADeviceToNoLongerBeAProxyGroupPlayer\x10\xc8\x01\x12\x44\n?OutputContextModificationCausedADeviceToBecomeAProxyGroupPlayer\x10\xc9\x01\x12\x37\n2OutputContextModificationRequestedNoTopologyChange\x10\xca\x01\x12\x16\n\x11OtherUnknownError\x10\xab\x02\"\xf3\x17\n\x0fProtocolMessage\x12#\n\x04type\x18\x01 \x01(\x0e\x32\x15.ProtocolMessage.Type\x12\x12\n\nidentifier\x18\x02 \x01(\t\x12\x1b\n\x13\x61uthenticationToken\x18\x03 \x01(\t\x12\"\n\terrorCode\x18\x04 \x01(\x0e\x32\x0f.ErrorCode.Enum\x12\x11\n\ttimestamp\x18\x05 \x01(\x04\x12\x18\n\x10\x65rrorDescription\x18N \x01(\t\x12\x18\n\x10uniqueIdentifier\x18U \x01(\t\"\x88\x16\n\x04Type\x12\x13\n\x0fUNKNOWN_MESSAGE\x10\x00\x12\x18\n\x14SEND_COMMAND_MESSAGE\x10\x01\x12\x1f\n\x1bSEND_COMMAND_RESULT_MESSAGE\x10\x02\x12\x15\n\x11GET_STATE_MESSAGE\x10\x03\x12\x15\n\x11SET_STATE_MESSAGE\x10\x04\x12\x17\n\x13SET_ARTWORK_MESSAGE\x10\x05\x12\x1f\n\x1bREGISTER_HID_DEVICE_MESSAGE\x10\x06\x12&\n\"REGISTER_HID_DEVICE_RESULT_MESSAGE\x10\x07\x12\x1a\n\x16SEND_HID_EVENT_MESSAGE\x10\x08\x12\x1b\n\x17SEND_HID_REPORT_MESSAGE\x10\t\x12$\n SEND_VIRTUAL_TOUCH_EVENT_MESSAGE\x10\n\x12\x18\n\x14NOTIFICATION_MESSAGE\x10\x0b\x12.\n*CONTENT_ITEMS_CHANGED_NOTIFICATION_MESSAGE\x10\x0c\x12\x17\n\x13\x44\x45VICE_INFO_MESSAGE\x10\x0f\x12!\n\x1d\x43LIENT_UPDATES_CONFIG_MESSAGE\x10\x10\x12\'\n#VOLUME_CONTROL_AVAILABILITY_MESSAGE\x10\x11\x12\x1b\n\x17GAME_CONTROLLER_MESSAGE\x10\x12\x12$\n REGISTER_GAME_CONTROLLER_MESSAGE\x10\x13\x12-\n)REGISTER_GAME_CONTROLLER_RESPONSE_MESSAGE\x10\x14\x12&\n\"UNREGISTER_GAME_CONTROLLER_MESSAGE\x10\x15\x12/\n+REGISTER_FOR_GAME_CONTROLLER_EVENTS_MESSAGE\x10\x16\x12\x14\n\x10KEYBOARD_MESSAGE\x10\x17\x12 \n\x1cGET_KEYBOARD_SESSION_MESSAGE\x10\x18\x12\x16\n\x12TEXT_INPUT_MESSAGE\x10\x19\x12#\n\x1fGET_VOICE_INPUT_DEVICES_MESSAGE\x10\x1a\x12,\n(GET_VOICE_INPUT_DEVICES_RESPONSE_MESSAGE\x10\x1b\x12\'\n#REGISTER_VOICE_INPUT_DEVICE_MESSAGE\x10\x1c\x12\x30\n,REGISTER_VOICE_INPUT_DEVICE_RESPONSE_MESSAGE\x10\x1d\x12\x1f\n\x1bSET_RECORDING_STATE_MESSAGE\x10\x1e\x12\x1c\n\x18SEND_VOICE_INPUT_MESSAGE\x10\x1f\x12\"\n\x1ePLAYBACK_QUEUE_REQUEST_MESSAGE\x10 \x12\x17\n\x13TRANSACTION_MESSAGE\x10!\x12\x1a\n\x16\x43RYPTO_PAIRING_MESSAGE\x10\"\x12&\n\"GAME_CONTROLLER_PROPERTIES_MESSAGE\x10#\x12\x1b\n\x17SET_READY_STATE_MESSAGE\x10$\x12\x1e\n\x1a\x44\x45VICE_INFO_UPDATE_MESSAGE\x10%\x12 \n\x1cSET_CONNECTION_STATE_MESSAGE\x10&\x12\x1d\n\x19SEND_BUTTON_EVENT_MESSAGE\x10\'\x12\x1b\n\x17SET_HILITE_MODE_MESSAGE\x10(\x12\x17\n\x13WAKE_DEVICE_MESSAGE\x10)\x12\x13\n\x0fGENERIC_MESSAGE\x10*\x12+\n\'SEND_PACKED_VIRTUAL_TOUCH_EVENT_MESSAGE\x10+\x12\x15\n\x11SEND_LYRICS_EVENT\x10,\x12\"\n\x1eSET_NOW_PLAYING_CLIENT_MESSAGE\x10.\x12\"\n\x1eSET_NOW_PLAYING_PLAYER_MESSAGE\x10/\x12\x16\n\x12GET_VOLUME_MESSAGE\x10\x31\x12\x1d\n\x19GET_VOLUME_RESULT_MESSAGE\x10\x32\x12\x16\n\x12SET_VOLUME_MESSAGE\x10\x33\x12\x1d\n\x19VOLUME_DID_CHANGE_MESSAGE\x10\x34\x12\x19\n\x15REMOVE_CLIENT_MESSAGE\x10\x35\x12\x19\n\x15REMOVE_PLAYER_MESSAGE\x10\x36\x12\x19\n\x15UPDATE_CLIENT_MESSAGE\x10\x37\x12\x1f\n\x1bUPDATE_CONTENT_ITEM_MESSAGE\x10\x38\x12\'\n#UPDATE_CONTENT_ITEM_ARTWORK_MESSAGE\x10\x39\x12\x19\n\x15UPDATE_PLAYER_MESSAGE\x10:\x12*\n&PROMPT_FOR_ROUTE_AUTHORIZATION_MESSAGE\x10;\x12\x33\n/PROMPT_FOR_ROUTE_AUTHORIZATION_RESPONSE_MESSAGE\x10<\x12.\n*PRESENT_ROUTE_AUTHORIZATION_STATUS_MESSAGE\x10=\x12+\n\'GET_VOLUME_CONTROL_CAPABILITIES_MESSAGE\x10>\x12\x32\n.GET_VOLUME_CONTROL_CAPABILITIES_RESULT_MESSAGE\x10?\x12\x32\n.VOLUME_CONTROL_CAPABILITIES_DID_CHANGE_MESSAGE\x10@\x12 \n\x1cUPDATE_OUTPUT_DEVICE_MESSAGE\x10\x41\x12!\n\x1dREMOVE_OUTPUT_DEVICES_MESSAGE\x10\x42\x12\x1d\n\x19REMOTE_TEXT_INPUT_MESSAGE\x10\x43\x12)\n%GET_REMOTE_TEXT_INPUT_SESSION_MESSAGE\x10\x44\x12\"\n\x1eREMOVE_OUTPUT_DEVICES_MESSAGE2\x10\x45\x12$\n PLAYBACK_SESSION_REQUEST_MESSAGE\x10\x46\x12%\n!PLAYBACK_SESSION_RESPONSE_MESSAGE\x10G\x12*\n&SET_DEFAULT_SUPPORTED_COMMANDS_MESSAGE\x10H\x12,\n(PLAYBACK_SESSION_MIGRATE_REQUEST_MESSAGE\x10I\x12-\n)PLAYBACK_SESSION_MIGRATE_RESPONSE_MESSAGE\x10J\x12*\n&PLAYBACK_SESSION_MIGRATE_BEGIN_MESSAGE\x10K\x12(\n$PLAYBACK_SESSION_MIGRATE_END_MESSAGE\x10L\x12)\n%UPDATE_ACTIVE_SYSTEM_ENDPOINT_MESSAGE\x10M\x12\x1e\n\x1aSET_DISCOVERY_MODE_MESSAGE\x10\x65\x12\x1d\n\x19UPDATE_END_POINTS_MESSAGE\x10\x66\x12\x1c\n\x18REMOVE_ENDPOINTS_MESSAGE\x10g\x12$\n PLAYER_CLIENT_PROPERTIES_MESSAGE\x10h\x12$\n ORIGIN_CLIENT_PROPERTIES_MESSAGE\x10i\x12\x16\n\x12\x41UDIO_FADE_MESSAGE\x10j\x12\x1f\n\x1b\x41UDIO_FADE_RESPONSE_MESSAGE\x10k*\x04\x08\x06\x10N*\x04\x08O\x10U*\x08\x08V\x10\x80\x80\x80\x80\x02'
 )
 
 
 
 _ERRORCODE_ENUM = _descriptor.EnumDescriptor(
   name='Enum',
   full_name='ErrorCode.Enum',
@@ -538,15 +538,15 @@
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
       name='SET_CONNECTION_STATE_MESSAGE', index=36, number=38,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='SEND_BUTTON_EVENT', index=37, number=39,
+      name='SEND_BUTTON_EVENT_MESSAGE', index=37, number=39,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
       name='SET_HILITE_MODE_MESSAGE', index=38, number=40,
       serialized_options=None,
       type=None,
@@ -761,15 +761,15 @@
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
   serialized_start=2928,
-  serialized_end=5744,
+  serialized_end=5752,
 )
 _sym_db.RegisterEnumDescriptor(_PROTOCOLMESSAGE_TYPE)
 
 
 _ERRORCODE = _descriptor.Descriptor(
   name='ErrorCode',
   full_name='ErrorCode',
@@ -863,15 +863,15 @@
   serialized_options=None,
   is_extendable=True,
   syntax='proto2',
   extension_ranges=[(6, 78), (79, 85), (86, 536870912), ],
   oneofs=[
   ],
   serialized_start=2715,
-  serialized_end=5766,
+  serialized_end=5774,
 )
 
 _ERRORCODE_ENUM.containing_type = _ERRORCODE
 _PROTOCOLMESSAGE.fields_by_name['type'].enum_type = _PROTOCOLMESSAGE_TYPE
 _PROTOCOLMESSAGE.fields_by_name['errorCode'].enum_type = _ERRORCODE_ENUM
 _PROTOCOLMESSAGE_TYPE.containing_type = _PROTOCOLMESSAGE
 DESCRIPTOR.message_types_by_name['ErrorCode'] = _ERRORCODE
```

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/ProtocolMessage_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/ProtocolMessage_pb2.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -198,15 +198,15 @@
         PLAYBACK_QUEUE_REQUEST_MESSAGE = ProtocolMessage.Type.V(32)
         TRANSACTION_MESSAGE = ProtocolMessage.Type.V(33)
         CRYPTO_PAIRING_MESSAGE = ProtocolMessage.Type.V(34)
         GAME_CONTROLLER_PROPERTIES_MESSAGE = ProtocolMessage.Type.V(35)
         SET_READY_STATE_MESSAGE = ProtocolMessage.Type.V(36)
         DEVICE_INFO_UPDATE_MESSAGE = ProtocolMessage.Type.V(37)
         SET_CONNECTION_STATE_MESSAGE = ProtocolMessage.Type.V(38)
-        SEND_BUTTON_EVENT = ProtocolMessage.Type.V(39)
+        SEND_BUTTON_EVENT_MESSAGE = ProtocolMessage.Type.V(39)
         SET_HILITE_MODE_MESSAGE = ProtocolMessage.Type.V(40)
         WAKE_DEVICE_MESSAGE = ProtocolMessage.Type.V(41)
         GENERIC_MESSAGE = ProtocolMessage.Type.V(42)
         SEND_PACKED_VIRTUAL_TOUCH_EVENT_MESSAGE = ProtocolMessage.Type.V(43)
         SEND_LYRICS_EVENT = ProtocolMessage.Type.V(44)
         SET_NOW_PLAYING_CLIENT_MESSAGE = ProtocolMessage.Type.V(46)
         SET_NOW_PLAYING_PLAYER_MESSAGE = ProtocolMessage.Type.V(47)
@@ -282,15 +282,15 @@
     PLAYBACK_QUEUE_REQUEST_MESSAGE = ProtocolMessage.Type.V(32)
     TRANSACTION_MESSAGE = ProtocolMessage.Type.V(33)
     CRYPTO_PAIRING_MESSAGE = ProtocolMessage.Type.V(34)
     GAME_CONTROLLER_PROPERTIES_MESSAGE = ProtocolMessage.Type.V(35)
     SET_READY_STATE_MESSAGE = ProtocolMessage.Type.V(36)
     DEVICE_INFO_UPDATE_MESSAGE = ProtocolMessage.Type.V(37)
     SET_CONNECTION_STATE_MESSAGE = ProtocolMessage.Type.V(38)
-    SEND_BUTTON_EVENT = ProtocolMessage.Type.V(39)
+    SEND_BUTTON_EVENT_MESSAGE = ProtocolMessage.Type.V(39)
     SET_HILITE_MODE_MESSAGE = ProtocolMessage.Type.V(40)
     WAKE_DEVICE_MESSAGE = ProtocolMessage.Type.V(41)
     GENERIC_MESSAGE = ProtocolMessage.Type.V(42)
     SEND_PACKED_VIRTUAL_TOUCH_EVENT_MESSAGE = ProtocolMessage.Type.V(43)
     SEND_LYRICS_EVENT = ProtocolMessage.Type.V(44)
     SET_NOW_PLAYING_CLIENT_MESSAGE = ProtocolMessage.Type.V(46)
     SET_NOW_PLAYING_PLAYER_MESSAGE = ProtocolMessage.Type.V(47)
```

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/RegisterForGameControllerEventsMessage_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/RegisterForGameControllerEventsMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/RegisterForGameControllerEventsMessage_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/RegisterForGameControllerEventsMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/RegisterHIDDeviceMessage_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/RegisterHIDDeviceMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/RegisterHIDDeviceMessage_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/RegisterHIDDeviceMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/RegisterHIDDeviceResultMessage_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/RegisterHIDDeviceResultMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/RegisterHIDDeviceResultMessage_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/RegisterHIDDeviceResultMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/RegisterVoiceInputDeviceMessage_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/RegisterVoiceInputDeviceMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/RegisterVoiceInputDeviceMessage_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/RegisterVoiceInputDeviceMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/RegisterVoiceInputDeviceResponseMessage_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/RegisterVoiceInputDeviceResponseMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/RegisterVoiceInputDeviceResponseMessage_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/RegisterVoiceInputDeviceResponseMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/RemoteTextInputMessage_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/RemoteTextInputMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/RemoteTextInputMessage_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/RemoteTextInputMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/RemoveClientMessage_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/RemoveClientMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/RemoveClientMessage_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/RemoveClientMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/RemoveEndpointsMessage_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/RemoveEndpointsMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/RemoveEndpointsMessage_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/RemoveEndpointsMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/RemoveOutputDevicesMessage_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/RemoveOutputDevicesMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/RemoveOutputDevicesMessage_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/RemoveOutputDevicesMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/RemovePlayerMessage_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/RemovePlayerMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/RemovePlayerMessage_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/RemovePlayerMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SendButtonEventMessage_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SendButtonEventMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SendButtonEventMessage_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SendButtonEventMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SendCommandMessage_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SendCommandMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SendCommandMessage_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SendCommandMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SendCommandResultMessage.proto` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SendCommandResultMessage.proto`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SendCommandResultMessage_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SendCommandResultMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SendCommandResultMessage_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SendCommandResultMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SendHIDEventMessage.proto` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SendHIDEventMessage.proto`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SendHIDEventMessage_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SendHIDEventMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SendHIDEventMessage_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SendHIDEventMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SendPackedVirtualTouchEventMessage.proto` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SendPackedVirtualTouchEventMessage.proto`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SendPackedVirtualTouchEventMessage_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SendPackedVirtualTouchEventMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SendPackedVirtualTouchEventMessage_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SendPackedVirtualTouchEventMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SendVoiceInputMessage.proto` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SendVoiceInputMessage.proto`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SendVoiceInputMessage_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SendVoiceInputMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SendVoiceInputMessage_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SendVoiceInputMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SetArtworkMessage_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SetArtworkMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SetArtworkMessage_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SetArtworkMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SetConnectionStateMessage_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SetConnectionStateMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SetConnectionStateMessage_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SetConnectionStateMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SetDefaultSupportedCommandsMessage.proto` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SetDefaultSupportedCommandsMessage.proto`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SetDefaultSupportedCommandsMessage_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SetDefaultSupportedCommandsMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SetDefaultSupportedCommandsMessage_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SetDefaultSupportedCommandsMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SetDiscoveryModeMessage_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SetDiscoveryModeMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SetDiscoveryModeMessage_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SetDiscoveryModeMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SetHiliteModeMessage_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SetHiliteModeMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SetHiliteModeMessage_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SetHiliteModeMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SetNowPlayingClientMessage_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SetNowPlayingClientMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SetNowPlayingClientMessage_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SetNowPlayingClientMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SetNowPlayingPlayerMessage_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SetNowPlayingPlayerMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SetNowPlayingPlayerMessage_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SetNowPlayingPlayerMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SetRecordingStateMessage_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SetRecordingStateMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SetRecordingStateMessage_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SetRecordingStateMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SetStateMessage.proto` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SetStateMessage.proto`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SetStateMessage_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SetStateMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SetStateMessage_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SetStateMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SetVolumeMessage_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SetVolumeMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SetVolumeMessage_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SetVolumeMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SupportedCommands_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SupportedCommands_pb2.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/SupportedCommands_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/SupportedCommands_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/TextInputMessage_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/TextInputMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/TextInputMessage_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/TextInputMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/TransactionKey_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/TransactionKey_pb2.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/TransactionKey_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/TransactionKey_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/TransactionMessage_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/TransactionMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/TransactionMessage_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/TransactionMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/TransactionPacket_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/TransactionPacket_pb2.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/TransactionPacket_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/TransactionPacket_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/TransactionPackets_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/TransactionPackets_pb2.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/TransactionPackets_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/TransactionPackets_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/UpdateClientMessage_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/UpdateClientMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/UpdateClientMessage_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/UpdateClientMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/UpdateContentItemArtworkMessage_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/UpdateContentItemArtworkMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/UpdateContentItemArtworkMessage_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/UpdateContentItemArtworkMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/UpdateContentItemMessage_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/UpdateContentItemMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/UpdateContentItemMessage_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/UpdateContentItemMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/UpdateEndPointsMessage.proto` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/UpdateEndPointsMessage.proto`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/UpdateEndPointsMessage_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/UpdateEndPointsMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/UpdateEndPointsMessage_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/UpdateEndPointsMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/UpdateOutputDeviceMessage.proto` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/UpdateOutputDeviceMessage.proto`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/UpdateOutputDeviceMessage_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/UpdateOutputDeviceMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/UpdateOutputDeviceMessage_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/UpdateOutputDeviceMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/VirtualTouchDeviceDescriptorMessage_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/VirtualTouchDeviceDescriptorMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/VirtualTouchDeviceDescriptorMessage_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/VirtualTouchDeviceDescriptorMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/VoiceInputDeviceDescriptorMessage_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/VoiceInputDeviceDescriptorMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/VoiceInputDeviceDescriptorMessage_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/VoiceInputDeviceDescriptorMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/VolumeControlAvailabilityMessage.proto` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/VolumeControlAvailabilityMessage.proto`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/VolumeControlAvailabilityMessage_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/VolumeControlAvailabilityMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/VolumeControlAvailabilityMessage_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/VolumeControlAvailabilityMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/VolumeControlCapabilitiesDidChangeMessage_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/VolumeControlCapabilitiesDidChangeMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/VolumeControlCapabilitiesDidChangeMessage_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/VolumeControlCapabilitiesDidChangeMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/VolumeDidChangeMessage_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/VolumeDidChangeMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/VolumeDidChangeMessage_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/VolumeDidChangeMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/WakeDeviceMessage_pb2.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/WakeDeviceMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/WakeDeviceMessage_pb2.pyi` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/WakeDeviceMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protobuf/__init__.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protobuf/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 from . import RegisterVoiceInputDeviceMessage_pb2
 from . import RegisterVoiceInputDeviceResponseMessage_pb2
 from . import RemoteTextInputMessage_pb2
 from . import RemoveClientMessage_pb2
 from . import RemoveEndpointsMessage_pb2
 from . import RemoveOutputDevicesMessage_pb2
 from . import RemovePlayerMessage_pb2
+from . import SendButtonEventMessage_pb2
 from . import SendCommandMessage_pb2
 from . import SendCommandResultMessage_pb2
 from . import SendHIDEventMessage_pb2
 from . import SendPackedVirtualTouchEventMessage_pb2
 from . import SendVoiceInputMessage_pb2
 from . import SetArtworkMessage_pb2
 from . import SetConnectionStateMessage_pb2
@@ -196,14 +197,15 @@
     ProtocolMessage.REGISTER_VOICE_INPUT_DEVICE_MESSAGE: RegisterVoiceInputDeviceMessage_pb2.registerVoiceInputDeviceMessage,
     ProtocolMessage.REGISTER_VOICE_INPUT_DEVICE_RESPONSE_MESSAGE: RegisterVoiceInputDeviceResponseMessage_pb2.registerVoiceInputDeviceResponseMessage,
     ProtocolMessage.REMOTE_TEXT_INPUT_MESSAGE: RemoteTextInputMessage_pb2.remoteTextInputMessage,
     ProtocolMessage.REMOVE_CLIENT_MESSAGE: RemoveClientMessage_pb2.removeClientMessage,
     ProtocolMessage.REMOVE_ENDPOINTS_MESSAGE: RemoveEndpointsMessage_pb2.removeEndpointsMessage,
     ProtocolMessage.REMOVE_OUTPUT_DEVICES_MESSAGE: RemoveOutputDevicesMessage_pb2.removeOutputDevicesMessage,
     ProtocolMessage.REMOVE_PLAYER_MESSAGE: RemovePlayerMessage_pb2.removePlayerMessage,
+    ProtocolMessage.SEND_BUTTON_EVENT_MESSAGE: SendButtonEventMessage_pb2.sendButtonEventMessage,
     ProtocolMessage.SEND_COMMAND_MESSAGE: SendCommandMessage_pb2.sendCommandMessage,
     ProtocolMessage.SEND_COMMAND_RESULT_MESSAGE: SendCommandResultMessage_pb2.sendCommandResultMessage,
     ProtocolMessage.SEND_HID_EVENT_MESSAGE: SendHIDEventMessage_pb2.sendHIDEventMessage,
     ProtocolMessage.SEND_PACKED_VIRTUAL_TOUCH_EVENT_MESSAGE: SendPackedVirtualTouchEventMessage_pb2.sendPackedVirtualTouchEventMessage,
     ProtocolMessage.SEND_VOICE_INPUT_MESSAGE: SendVoiceInputMessage_pb2.sendVoiceInputMessage,
     ProtocolMessage.SET_ARTWORK_MESSAGE: SetArtworkMessage_pb2.setArtworkMessage,
     ProtocolMessage.SET_CONNECTION_STATE_MESSAGE: SetConnectionStateMessage_pb2.setConnectionStateMessage,
@@ -251,14 +253,15 @@
 REGISTER_VOICE_INPUT_DEVICE_MESSAGE = ProtocolMessage.REGISTER_VOICE_INPUT_DEVICE_MESSAGE
 REGISTER_VOICE_INPUT_DEVICE_RESPONSE_MESSAGE = ProtocolMessage.REGISTER_VOICE_INPUT_DEVICE_RESPONSE_MESSAGE
 REMOTE_TEXT_INPUT_MESSAGE = ProtocolMessage.REMOTE_TEXT_INPUT_MESSAGE
 REMOVE_CLIENT_MESSAGE = ProtocolMessage.REMOVE_CLIENT_MESSAGE
 REMOVE_ENDPOINTS_MESSAGE = ProtocolMessage.REMOVE_ENDPOINTS_MESSAGE
 REMOVE_OUTPUT_DEVICES_MESSAGE = ProtocolMessage.REMOVE_OUTPUT_DEVICES_MESSAGE
 REMOVE_PLAYER_MESSAGE = ProtocolMessage.REMOVE_PLAYER_MESSAGE
+SEND_BUTTON_EVENT_MESSAGE = ProtocolMessage.SEND_BUTTON_EVENT_MESSAGE
 SEND_COMMAND_MESSAGE = ProtocolMessage.SEND_COMMAND_MESSAGE
 SEND_COMMAND_RESULT_MESSAGE = ProtocolMessage.SEND_COMMAND_RESULT_MESSAGE
 SEND_HID_EVENT_MESSAGE = ProtocolMessage.SEND_HID_EVENT_MESSAGE
 SEND_PACKED_VIRTUAL_TOUCH_EVENT_MESSAGE = ProtocolMessage.SEND_PACKED_VIRTUAL_TOUCH_EVENT_MESSAGE
 SEND_VOICE_INPUT_MESSAGE = ProtocolMessage.SEND_VOICE_INPUT_MESSAGE
 SET_ARTWORK_MESSAGE = ProtocolMessage.SET_ARTWORK_MESSAGE
 SET_CONNECTION_STATE_MESSAGE = ProtocolMessage.SET_CONNECTION_STATE_MESSAGE
```

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/protocol.py` & `pyatv-0.9.8/pyatv/protocols/mrp/protocol.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,42 @@
 """Implementation of the MRP protocol."""
 
 import asyncio
 from collections import namedtuple
 from enum import Enum
 import logging
+from typing import Dict, NamedTuple, Optional
 import uuid
 
 from pyatv import exceptions
 from pyatv.auth.hap_pairing import parse_credentials
+from pyatv.auth.hap_srp import SRPAuthHandler
 from pyatv.core.protocol import MessageDispatcher, heartbeater
+from pyatv.interface import BaseService
 from pyatv.protocols.mrp import messages, protobuf
 from pyatv.protocols.mrp.auth import MrpPairVerifyProcedure
+from pyatv.protocols.mrp.connection import AbstractMrpConnection
 
 _LOGGER = logging.getLogger(__name__)
 
 HEARTBEAT_INTERVAL = 30
 HEARTBEAT_RETRIES = 1  # One regular attempt + retries
 
 SRP_SALT = "MediaRemote-Salt"
 SRP_OUTPUT_INFO = "MediaRemote-Write-Encryption-Key"
 SRP_INPUT_INFO = "MediaRemote-Read-Encryption-Key"
 
 Listener = namedtuple("Listener", "func data")
-OutstandingMessage = namedtuple("OutstandingMessage", "semaphore response")
+
+
+class OutstandingMessage(NamedTuple):
+    """Sent message waiting for response."""
+
+    semaphore: asyncio.Semaphore
+    response: protobuf.ProtocolMessage
 
 
 class ProtocolState(Enum):
     """Protocol internal state."""
 
     NOT_CONNECTED = 0
     """Protocol state is not connected."""
@@ -85,28 +95,32 @@
     * Connect whenever it is needed
     * Send necessary messages automatically, e.g. DEVICE_INFORMATION
     * Enable encryption at the right time
 
     It provides an API for sending and receiving messages.
     """
 
-    def __init__(self, connection, srp, service):
+    def __init__(
+        self,
+        connection: AbstractMrpConnection,
+        srp: SRPAuthHandler,
+        service: BaseService,
+    ) -> None:
         """Initialize a new MrpProtocol."""
         super().__init__()
         self.connection = connection
         self.connection.listener = self
         self.srp = srp
         self.service = service
-        self.device_info = None
-        self._heartbeat_task = None
-        self._outstanding = {}
-        self._listeners = {}
-        self._state = ProtocolState.NOT_CONNECTED
+        self.device_info: Optional[protobuf.ProtocolMessage] = None
+        self._heartbeat_task: Optional[asyncio.Task] = None
+        self._outstanding: Dict[str, OutstandingMessage] = {}
+        self._state: ProtocolState = ProtocolState.NOT_CONNECTED
 
-    async def start(self, skip_initial_messages=False):
+    async def start(self, skip_initial_messages: bool = False) -> None:
         """Connect to device and listen to incoming messages."""
         if self._state != ProtocolState.NOT_CONNECTED:
             raise exceptions.InvalidStateError(self._state.name)
 
         self._state = ProtocolState.CONNECTING
 
         try:
@@ -145,15 +159,15 @@
             # Something went wrong, let's do cleanup
             self.stop()
             raise
         else:
             # We're now ready
             self._state = ProtocolState.READY
 
-    def stop(self):
+    def stop(self) -> None:
         """Disconnect from device."""
         if self._outstanding:
             _LOGGER.warning(
                 "There were %d outstanding requests", len(self._outstanding)
             )
 
         if self._heartbeat_task is not None:
@@ -161,24 +175,32 @@
             self._heartbeat_task = None
         self._outstanding = {}
         self.connection.close()
         self._state = ProtocolState.STOPPED
 
     def enable_heartbeat(self) -> None:
         """Enable sending periodic heartbeat messages."""
+
+        async def _sender_func(message: Optional[protobuf.ProtocolMessage]) -> None:
+            if message is not None:
+                await self.send_and_receive(message)
+
+        def _failure_func(exc: Exception):
+            self.connection.close()
+
         self._heartbeat_task = asyncio.ensure_future(
             heartbeater(
                 name=str(self.connection),
-                sender_func=self.send_and_receive,
-                failure_func=lambda exc: self.connection.close,
+                sender_func=_sender_func,
+                failure_func=_failure_func,
                 message_factory=lambda: messages.create(protobuf.GENERIC_MESSAGE),
             )
         )
 
-    async def _enable_encryption(self):
+    async def _enable_encryption(self) -> None:
         # Encryption can be enabled whenever credentials are available but only
         # after DEVICE_INFORMATION has been sent
         if self.service.credentials is None:
             return
 
         # Verify credentials and generate keys
         credentials = parse_credentials(self.service.credentials)
@@ -189,25 +211,30 @@
             output_key, input_key = pair_verifier.encryption_keys(
                 SRP_SALT, SRP_OUTPUT_INFO, SRP_INPUT_INFO
             )
             self.connection.enable_encryption(output_key, input_key)
         except Exception as ex:
             raise exceptions.AuthenticationError(str(ex)) from ex
 
-    async def send(self, message):
+    async def send(self, message: protobuf.ProtocolMessage) -> None:
         """Send a message and expect no response."""
         if self._state not in [
             ProtocolState.CONNECTED,
             ProtocolState.READY,
         ]:
             raise exceptions.InvalidStateError(self._state.name)
 
         self.connection.send(message)
 
-    async def send_and_receive(self, message, generate_identifier=True, timeout=5):
+    async def send_and_receive(
+        self,
+        message: protobuf.ProtocolMessage,
+        generate_identifier: bool = True,
+        timeout: float = 5.0,
+    ) -> protobuf.ProtocolMessage:
         """Send a message and wait for a response."""
         if self._state not in [
             ProtocolState.CONNECTED,
             ProtocolState.READY,
         ]:
             raise exceptions.InvalidStateError(self._state.name)
 
@@ -223,31 +250,35 @@
             message.identifier = identifier
         else:
             identifier = "type_" + str(message.type)
 
         self.connection.send(message)
         return await self._receive(identifier, timeout)
 
-    async def _receive(self, identifier, timeout):
+    async def _receive(
+        self, identifier: str, timeout: float
+    ) -> protobuf.ProtocolMessage:
         semaphore = asyncio.Semaphore(value=0)
-        self._outstanding[identifier] = OutstandingMessage(semaphore, None)
+        self._outstanding[identifier] = OutstandingMessage(
+            semaphore, protobuf.ProtocolMessage()
+        )
 
         try:
             # The connection instance will dispatch the message
             await asyncio.wait_for(semaphore.acquire(), timeout)
 
         except Exception:
             del self._outstanding[identifier]
             raise
 
         response = self._outstanding[identifier].response
         del self._outstanding[identifier]
         return response
 
-    def message_received(self, message, _):
+    def message_received(self, message: protobuf.ProtocolMessage, _) -> None:
         """Message was received from device."""
         # If the message identifier is outstanding, then someone is
         # waiting for the respone so we save it here
         identifier = message.identifier or "type_" + str(message.type)
         if identifier in self._outstanding:
             outstanding = OutstandingMessage(
                 self._outstanding[identifier].semaphore, message
```

### Comparing `pyatv-0.9.7/pyatv/protocols/mrp/server_auth.py` & `pyatv-0.9.8/pyatv/protocols/mrp/server_auth.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/raop/__init__.py` & `pyatv-0.9.8/pyatv/protocols/raop/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,22 @@
 from pyatv.const import (
     DeviceModel,
     FeatureName,
     FeatureState,
     PairingRequirement,
     Protocol,
 )
-from pyatv.core import MutableService, SetupData, TakeoverMethod, mdns
+from pyatv.core import (
+    AbstractPushUpdater,
+    MutableService,
+    ProtocolStateDispatcher,
+    SetupData,
+    TakeoverMethod,
+    mdns,
+)
 from pyatv.core.scan import ScanHandler, ScanHandlerReturn
 from pyatv.helpers import get_unique_id
 from pyatv.interface import (
     Audio,
     BaseConfig,
     BaseService,
     DeviceInfo,
@@ -57,20 +64,20 @@
 
 DBFS_MIN = -30.0
 DBFS_MAX = 0.0
 PERCENTAGE_MIN = 0.0
 PERCENTAGE_MAX = 100.0
 
 
-class RaopPushUpdater(PushUpdater):
+class RaopPushUpdater(AbstractPushUpdater):
     """Implementation of push update support for RAOP."""
 
-    def __init__(self, metadata: Metadata, loop: asyncio.AbstractEventLoop):
+    def __init__(self, metadata: Metadata, state_dispatcher: ProtocolStateDispatcher):
         """Initialize a new RaopPushUpdater instance."""
-        super().__init__(loop)
+        super().__init__(state_dispatcher)
         self._activated = False
         self.metadata = metadata
 
     @property
     def active(self) -> bool:
         """Return if push updater has been started."""
         return self._activated
@@ -212,15 +219,15 @@
             FeatureName.SetVolume,
             FeatureName.Volume,
             FeatureName.VolumeDown,
             FeatureName.VolumeUp,
         ]:
             return FeatureInfo(FeatureState.Available)
 
-        if feature_name == FeatureName.Stop:
+        if feature_name in [FeatureName.Stop, FeatureName.Pause]:
             is_streaming = self.playback_manager.raop is not None
             return FeatureInfo(
                 FeatureState.Available if is_streaming else FeatureState.Unavailable
             )
 
         return FeatureInfo(FeatureState.Unavailable)
 
@@ -373,14 +380,21 @@
     """Implementation of remote control functionality."""
 
     def __init__(self, audio: RaopAudio, playback_manager: RaopPlaybackManager):
         """Initialize a new RaopRemoteControl instance."""
         self.audio = audio
         self.playback_manager = playback_manager
 
+    # At the moment, pause will stop playback until it is properly implemented. This
+    # gives a better experience in Home Assistant.
+    async def pause(self) -> None:
+        """Press key pause."""
+        if self.playback_manager.raop:
+            self.playback_manager.raop.stop()
+
     async def stop(self) -> None:
         """Press key stop."""
         if self.playback_manager.raop:
             self.playback_manager.raop.stop()
 
     async def volume_up(self) -> None:
         """Press key volume up."""
@@ -456,19 +470,20 @@
 def setup(  # pylint: disable=too-many-locals
     loop: asyncio.AbstractEventLoop,
     config: BaseConfig,
     service: BaseService,
     device_listener: StateProducer,
     session_manager: ClientSessionManager,
     takeover: TakeoverMethod,
+    state_dispatcher: ProtocolStateDispatcher,
 ) -> Generator[SetupData, None, None]:
     """Set up a new RAOP service."""
     playback_manager = RaopPlaybackManager(str(config.address), service.port)
     metadata = RaopMetadata(playback_manager)
-    push_updater = RaopPushUpdater(metadata, loop)
+    push_updater = RaopPushUpdater(metadata, state_dispatcher)
 
     class RaopStateListener(RaopListener):
         """Listener for RAOP state changes."""
 
         def playing(self, playback_info: PlaybackInfo) -> None:
             """Media started playing with metadata."""
             playback_manager.playback_info = playback_info
@@ -529,14 +544,15 @@
                 FeatureName.Position,
                 FeatureName.TotalTime,
                 FeatureName.SetVolume,
                 FeatureName.Volume,
                 FeatureName.VolumeUp,
                 FeatureName.VolumeDown,
                 FeatureName.Stop,
+                FeatureName.Pause,
             ]
         ),
     )
 
 
 def pair(
     config: BaseConfig,
```

### Comparing `pyatv-0.9.7/pyatv/protocols/raop/audio_source.py` & `pyatv-0.9.8/pyatv/protocols/raop/audio_source.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/raop/fifo.py` & `pyatv-0.9.8/pyatv/protocols/raop/fifo.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/raop/packets.py` & `pyatv-0.9.8/pyatv/protocols/raop/packets.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/raop/parsers.py` & `pyatv-0.9.8/pyatv/protocols/raop/parsers.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/raop/raop.py` & `pyatv-0.9.8/pyatv/protocols/raop/raop.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/protocols/raop/timing.py` & `pyatv-0.9.8/pyatv/protocols/raop/timing.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/scripts/__init__.py` & `pyatv-0.9.8/pyatv/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/scripts/atvlog.py` & `pyatv-0.9.8/pyatv/scripts/atvlog.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/scripts/atvproxy.py` & `pyatv-0.9.8/pyatv/scripts/atvproxy.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/scripts/atvremote.py` & `pyatv-0.9.8/pyatv/scripts/atvremote.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/scripts/atvscript.py` & `pyatv-0.9.8/pyatv/scripts/atvscript.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/support/__init__.py` & `pyatv-0.9.8/pyatv/support/__init__.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/support/cache.py` & `pyatv-0.9.8/pyatv/support/cache.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/support/chacha20.py` & `pyatv-0.9.8/pyatv/support/chacha20.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/support/collections.py` & `pyatv-0.9.8/pyatv/support/collections.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/support/device_info.py` & `pyatv-0.9.8/pyatv/support/device_info.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/support/dns.py` & `pyatv-0.9.8/pyatv/support/dns.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/support/http.py` & `pyatv-0.9.8/pyatv/support/http.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/support/knock.py` & `pyatv-0.9.8/pyatv/support/knock.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,61 +3,69 @@
 This module will open a TCP-connection to one or more ports on a given host and
 immediately close it. The use case for this is to wake a device sleeping via a Bonjour
 sleep proxy. Such a device will automatically be woken up in case any of its services
 are accessed, something this module will try to emulate.
 """
 
 import asyncio
+from asyncio.tasks import FIRST_EXCEPTION
+import errno
 from ipaddress import IPv4Address
 import logging
-import math
 from typing import List
 
 _LOGGER = logging.getLogger(__name__)
 
-SEND_INTERVAL = 2.0
+_ABORT_KNOCK_ERRNOS = {errno.EHOSTDOWN, errno.EHOSTUNREACH}
 
+_SLEEP_AFTER_CONNECT = 0.1
+_KNOCK_TIMEOUT_BUFFER = _SLEEP_AFTER_CONNECT * 2
 
-async def _async_knock(address: IPv4Address, port: int):
+
+async def _async_knock(address: IPv4Address, port: int, timeout: float) -> None:
+    """Open a connection to the device to wake a given host."""
+    writer = None
     try:
-        _, writer = await asyncio.open_connection(str(address), port)
-    except (OSError, asyncio.CancelledError):
+        _, writer = await asyncio.wait_for(
+            asyncio.open_connection(str(address), port), timeout=timeout
+        )
+    except asyncio.TimeoutError:
         pass
+    except OSError as ex:
+        # If we get EHOSTDOWN or EHOSTUNREACH we
+        # can give up as its not going to wake
+        # a device that is not there
+        if ex.errno in _ABORT_KNOCK_ERRNOS:
+            raise
     else:
-        await asyncio.sleep(0.1)
-        writer.close()
+        await asyncio.sleep(_SLEEP_AFTER_CONNECT)
+    finally:
+        if writer:
+            writer.close()
 
 
-async def knock(
-    address: IPv4Address, ports: List[int], loop: asyncio.AbstractEventLoop
-):
+async def knock(address: IPv4Address, ports: List[int], timeout: float) -> None:
     """Knock on a set of ports for a given host."""
-    _LOGGER.debug("Knocking at ports %s on %s", ports, address)
-    await asyncio.wait(
-        [asyncio.ensure_future(_async_knock(address, port)) for port in ports]
-    )
+    tasks = []
+    knock_runtime = timeout - _KNOCK_TIMEOUT_BUFFER
+    for port in ports:
+        # yield to the event loop to ensure we do not block
+        await asyncio.sleep(0)
+        _LOGGER.debug("Knocking at port %s on %s", port, address)
+        tasks.append(asyncio.ensure_future(_async_knock(address, port, knock_runtime)))
+    _, pending = await asyncio.wait(tasks, return_when=FIRST_EXCEPTION)
+    for task in pending:
+        task.cancel()
 
 
 async def knocker(
     address: IPv4Address,
     ports: List[int],
     loop: asyncio.AbstractEventLoop,
     timeout: int = 4,
 ) -> asyncio.Future:
     """Continuously knock on a set of ports.
 
     New port knocks are sent every two seconds, so a timeout of 4 seconds will result in
     two knocks.
     """
-    no_of_sends = math.ceil(timeout / SEND_INTERVAL)
-
-    async def _repeat():
-        for _ in range(no_of_sends):
-            try:
-                await knock(address, ports, loop)
-                await asyncio.sleep(SEND_INTERVAL)
-            except asyncio.CancelledError:
-                break
-            except Exception:  # pylint: disable=broad-except
-                _LOGGER.exception("failed to port knock")
-
-    return asyncio.ensure_future(_repeat())
+    return asyncio.ensure_future(knock(address, ports, timeout))
```

### Comparing `pyatv-0.9.7/pyatv/support/metadata.py` & `pyatv-0.9.8/pyatv/support/metadata.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/support/net.py` & `pyatv-0.9.8/pyatv/support/net.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from ipaddress import IPv4Address, IPv4Interface
 import logging
 import platform
 import socket
 import struct
 from typing import List, Optional
 
-import netifaces
+from ifaddr import get_adapters
 
 from pyatv import exceptions
 
 _LOGGER = logging.getLogger(__name__)
 
 
 def unused_port() -> int:
@@ -50,30 +50,33 @@
     _LOGGER.debug("Binding on %s:%d", address or "*", port)
     sock.bind((address or "", port))
     return sock
 
 
 def get_local_address_reaching(dest_ip: IPv4Address) -> Optional[IPv4Address]:
     """Get address of a local interface within same subnet as provided address."""
-    for iface in netifaces.interfaces():
-        for addr in netifaces.ifaddresses(iface).get(netifaces.AF_INET, []):
-            iface = IPv4Interface(addr["addr"] + "/" + addr["netmask"])
+    for adapter in get_adapters():
+        for addr in [addr for addr in adapter.ips if addr.is_IPv4]:
+            iface = IPv4Interface(f"{addr.ip}/{addr.network_prefix}")
             if dest_ip in iface.network:
                 return iface.ip
     return None
 
 
-def get_private_addresses() -> List[IPv4Address]:
+def get_private_addresses(include_loopback=True) -> List[IPv4Address]:
     """Get private (RFC1918 + loopback) addresses from all interfaces."""
     addresses: List[IPv4Address] = []
-    for iface in netifaces.interfaces():
-        for addr in netifaces.ifaddresses(iface).get(netifaces.AF_INET, []):
-            ipaddr = IPv4Address(addr["addr"])
+    for adapter in get_adapters():
+        for addr in [addr for addr in adapter.ips if addr.is_IPv4]:
+            ipaddr = IPv4Address(addr.ip)
+            if ipaddr.is_loopback and not include_loopback:
+                continue
             if ipaddr.is_private:
                 addresses.append(ipaddr)
+
     return addresses
 
 
 # Reference: https://stackoverflow.com/a/14855726
 def tcp_keepalive(sock) -> None:
     """Configure keep-alive on a socket."""
     current_platform = platform.system()
```

### Comparing `pyatv-0.9.7/pyatv/support/packet.py` & `pyatv-0.9.8/pyatv/support/packet.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/support/rtsp.py` & `pyatv-0.9.8/pyatv/support/rtsp.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/support/state_producer.py` & `pyatv-0.9.8/pyatv/support/state_producer.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv/support/variant.py` & `pyatv-0.9.8/pyatv/support/variant.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/pyatv.egg-info/PKG-INFO` & `pyatv-0.9.8/pyatv.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pyatv
-Version: 0.9.7
+Version: 0.9.8
 Summary: A client library for Apple TV and AirPlay devices
 Home-page: https://pyatv.dev
 Author: Pierre Ståhl
 Author-email: pierre.staahl@gmail.com
 License: MIT
-Download-URL: https://github.com/postlund/pyatv/archive/refs/tags/v0.9.7.zip
+Download-URL: https://github.com/postlund/pyatv/archive/refs/tags/v0.9.8.zip
 Project-URL: Repository, https://github.com/postlund/pyatv
 Project-URL: Bug Reports, https://github.com/postlund/pyatv/issues
 Keywords: apple,tv,airplay,raop,companion,dmap,dacp
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyatv-0.9.7/pyatv.egg-info/SOURCES.txt` & `pyatv-0.9.8/pyatv.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -392,14 +392,15 @@
 pyatv/support/dns.py
 pyatv/support/http.py
 pyatv/support/knock.py
 pyatv/support/metadata.py
 pyatv/support/net.py
 pyatv/support/packet.py
 pyatv/support/rtsp.py
+pyatv/support/shield.py
 pyatv/support/state_producer.py
 pyatv/support/variant.py
 tests/__init__.py
 tests/common_functional_tests.py
 tests/conftest.py
 tests/fake_knock.py
 tests/fake_udns.py
@@ -407,14 +408,15 @@
 tests/test_convert.py
 tests/test_helpers.py
 tests/test_interface.py
 tests/test_scan_functional.py
 tests/utils.py
 tests/zeroconf_stub.py
 tests/auth/test_hap_tlv8.py
+tests/core/test_core.py
 tests/core/test_facade.py
 tests/core/test_mdns.py
 tests/core/test_mdns_functional.py
 tests/core/test_protocol.py
 tests/core/test_relayer.py
 tests/core/test_scan.py
 tests/data/README
@@ -474,10 +476,11 @@
 tests/support/test_collections.py
 tests/support/test_device_info.py
 tests/support/test_dns.py
 tests/support/test_http.py
 tests/support/test_knock.py
 tests/support/test_net.py
 tests/support/test_packet.py
+tests/support/test_shield.py
 tests/support/test_state_producer.py
 tests/support/test_support.py
 tests/support/test_variant.py
```

### Comparing `pyatv-0.9.7/pyproject.toml` & `pyatv-0.9.8/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -17,12 +17,11 @@
     "scripts",
 ]
 
 [[tool.mypy.overrides]]
 module = [
     "miniaudio",
     "audio_metadata",
-    "netifaces",
     "srptools",
     "bitarray",
 ]
 ignore_missing_imports = true
```

### Comparing `pyatv-0.9.7/setup.py` & `pyatv-0.9.8/setup.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/tests/auth/test_hap_tlv8.py` & `pyatv-0.9.8/tests/auth/test_hap_tlv8.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/tests/common_functional_tests.py` & `pyatv-0.9.8/tests/common_functional_tests.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/tests/conftest.py` & `pyatv-0.9.8/tests/conftest.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 from types import SimpleNamespace
 import typing
 from unittest.mock import Mock, patch
 
-import netifaces
+from ifaddr import IP, Adapter
 import pytest
 
 import pyatv
 from pyatv.auth.hap_pairing import parse_credentials
 from pyatv.interface import BaseConfig
 from pyatv.support.http import create_session
 from pyatv.support.net import unused_port
@@ -25,35 +25,24 @@
 
 
 def pytest_configure(config):
     config.addinivalue_line("markers", "use_heartbeat: enable MRP heart beata")
 
 
 @pytest.fixture(autouse=True)
-def stub_netifaces():
+def stub_ifaddr():
     methods = {
-        "interfaces": Mock(return_value=["eth0"]),
-        "ifaddresses": Mock(
-            return_value={
-                netifaces.AF_INET: [
-                    {
-                        "addr": "10.0.10.1",
-                        "netmask": "255.255.255.0",
-                        "broadcast": "10.0.10.255",
-                    },
-                    {
-                        "addr": "127.0.0.1",
-                        "netmask": "255.0.0.0",
-                    },
-                ]
-            }
-        ),
+        "get_adapters": Mock(
+            return_value=[
+                Adapter("eth0", "eth0", [IP("10.0.10.1", 24, "eth0")]),
+                Adapter("lo", "lo", [IP("127.0.0.1", 8, "lo")]),
+            ]
+        )
     }
-
-    with patch.multiple("netifaces", **methods):
+    with patch.multiple("pyatv.support.net", **methods):
         yield
 
 
 @pytest.fixture(autouse=True, name="stub_sleep")
 def stub_sleep_fixture():
     stub_sleep()
     yield
```

### Comparing `pyatv-0.9.7/tests/core/test_mdns.py` & `pyatv-0.9.8/tests/core/test_mdns.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/tests/core/test_mdns_functional.py` & `pyatv-0.9.8/tests/core/test_mdns_functional.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/tests/core/test_protocol.py` & `pyatv-0.9.8/tests/core/test_protocol.py`

 * *Files 5% similar despite different names*

```diff
@@ -139,15 +139,15 @@
     dispatched_msg1 = None
     dispatched_msg2 = None
 
     async def dispatch_func1(message: bytes) -> None:
         nonlocal dispatched_msg1
         dispatched_msg1 = message
 
-    async def dispatch_func2(message: bytes) -> None:
+    def dispatch_func2(message: bytes) -> None:
         nonlocal dispatched_msg2
         dispatched_msg2 = message
 
     dispatcher = MessageDispatcher[int, bytes]()
     dispatcher.listen_to(1, dispatch_func1)
     dispatcher.listen_to(2, dispatch_func2)
 
@@ -156,7 +156,26 @@
     assert dispatched_msg2 is None
 
     dispatched_msg1 = None
 
     await asyncio.wait_for(asyncio.gather(*dispatcher.dispatch(2, b"456")), 5.0)
     assert dispatched_msg1 is None
     assert dispatched_msg2 == b"456"
+
+
+async def test_dispatch_with_filter():
+    dispatched_value = None
+
+    async def dispatch_func(value: int) -> None:
+        nonlocal dispatched_value
+        dispatched_value = value
+
+    dispatcher = MessageDispatcher[int, int]()
+    dispatcher.listen_to(
+        1, dispatch_func, message_filter=lambda message: (message % 2) == 0
+    )
+
+    await asyncio.wait_for(asyncio.gather(*dispatcher.dispatch(1, 1)), 5.0)
+    assert dispatched_value == None
+
+    await asyncio.wait_for(asyncio.gather(*dispatcher.dispatch(1, 2)), 5.0)
+    assert dispatched_value == 2
```

### Comparing `pyatv-0.9.7/tests/core/test_relayer.py` & `pyatv-0.9.8/tests/core/test_relayer.py`

 * *Files 3% similar despite different names*

```diff
@@ -153,14 +153,42 @@
 
 def test_main_instance_missing_instance_for_priority():
     relayer = Relayer(BaseClass, [Protocol.MRP])
     with pytest.raises(exceptions.NotSupportedError):
         relayer.main_instance
 
 
+def test_main_protocol():
+    relayer = Relayer(BaseClass, [Protocol.MRP, Protocol.DMAP, Protocol.AirPlay])
+
+    relayer.register(SubClass1(), Protocol.AirPlay)
+    assert relayer.main_protocol == Protocol.AirPlay
+
+    relayer.register(SubClass1(), Protocol.DMAP)
+    assert relayer.main_protocol == Protocol.DMAP
+
+    relayer.register(SubClass1(), Protocol.MRP)
+    assert relayer.main_protocol == Protocol.MRP
+
+
+def test_main_protocol_with_no_instance():
+    relayer = Relayer(BaseClass, [Protocol.MRP])
+    assert relayer.main_protocol is None
+
+
+def test_takeover_overrides_main_protocol():
+    relayer = Relayer(BaseClass, [Protocol.MRP, Protocol.DMAP])
+    relayer.register(SubClass4("mrp"), Protocol.MRP)
+    relayer.register(SubClass4("dmap"), Protocol.DMAP)
+
+    relayer.takeover(Protocol.DMAP)
+
+    assert relayer.main_protocol == Protocol.DMAP
+
+
 def test_get_instance_of_type():
     instance1 = SubClass1()
     instance2 = SubClass2()
     relayer = Relayer(BaseClass, [Protocol.MRP, Protocol.DMAP, Protocol.AirPlay])
     relayer.register(instance1, Protocol.MRP)
     relayer.register(instance2, Protocol.DMAP)
```

### Comparing `pyatv-0.9.7/tests/core/test_scan.py` & `pyatv-0.9.8/tests/core/test_scan.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/tests/data/README` & `pyatv-0.9.8/tests/data/README`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/tests/data/audio_10_frames.wav` & `pyatv-0.9.8/tests/data/audio_10_frames.wav`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/tests/data/audio_1_packet_metadata.wav` & `pyatv-0.9.8/tests/data/audio_1_packet_metadata.wav`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/tests/data/audio_3_packets.wav` & `pyatv-0.9.8/tests/data/audio_3_packets.wav`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/tests/data/only_metadata.wav` & `pyatv-0.9.8/tests/data/only_metadata.wav`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/tests/data/static_3sec.ogg` & `pyatv-0.9.8/tests/data/static_3sec.ogg`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/tests/fake_device/__init__.py` & `pyatv-0.9.8/tests/fake_device/__init__.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/tests/fake_device/airplay.py` & `pyatv-0.9.8/tests/fake_device/airplay.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/tests/fake_device/companion.py` & `pyatv-0.9.8/tests/fake_device/companion.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/tests/fake_device/dmap.py` & `pyatv-0.9.8/tests/fake_device/dmap.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/tests/fake_device/mrp.py` & `pyatv-0.9.8/tests/fake_device/mrp.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/tests/fake_device/raop.py` & `pyatv-0.9.8/tests/fake_device/raop.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/tests/fake_knock.py` & `pyatv-0.9.8/tests/fake_knock.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/tests/fake_udns.py` & `pyatv-0.9.8/tests/fake_udns.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/tests/protocols/airplay/auth/test_airplay_legacy_auth.py` & `pyatv-0.9.8/tests/protocols/airplay/auth/test_airplay_legacy_auth.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/tests/protocols/airplay/auth/test_auth.py` & `pyatv-0.9.8/tests/protocols/airplay/auth/test_auth.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/tests/protocols/airplay/conftest.py` & `pyatv-0.9.8/tests/protocols/airplay/conftest.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/tests/protocols/airplay/test_airplay.py` & `pyatv-0.9.8/tests/protocols/airplay/test_airplay.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/tests/protocols/airplay/test_airplay_interface.py` & `pyatv-0.9.8/tests/protocols/airplay/test_airplay_interface.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/tests/protocols/airplay/test_airplay_pair.py` & `pyatv-0.9.8/tests/protocols/airplay/test_airplay_pair.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/tests/protocols/airplay/test_airplay_player.py` & `pyatv-0.9.8/tests/protocols/airplay/test_airplay_player.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/tests/protocols/airplay/test_airplay_scan.py` & `pyatv-0.9.8/tests/protocols/airplay/test_airplay_scan.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/tests/protocols/companion/conftest.py` & `pyatv-0.9.8/tests/protocols/companion/conftest.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/tests/protocols/companion/test_companion.py` & `pyatv-0.9.8/tests/protocols/companion/test_companion.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/tests/protocols/companion/test_companion_auth.py` & `pyatv-0.9.8/tests/protocols/companion/test_companion_auth.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/tests/protocols/companion/test_companion_functional.py` & `pyatv-0.9.8/tests/protocols/companion/test_companion_functional.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/tests/protocols/companion/test_companion_scan.py` & `pyatv-0.9.8/tests/protocols/companion/test_companion_scan.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/tests/protocols/companion/test_opack.py` & `pyatv-0.9.8/tests/protocols/companion/test_opack.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/tests/protocols/dmap/test_daap.py` & `pyatv-0.9.8/tests/protocols/dmap/test_daap.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/tests/protocols/dmap/test_dmap.py` & `pyatv-0.9.8/tests/protocols/dmap/test_dmap.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/tests/protocols/dmap/test_dmap_functional.py` & `pyatv-0.9.8/tests/protocols/dmap/test_dmap_functional.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/tests/protocols/dmap/test_dmap_pairing.py` & `pyatv-0.9.8/tests/protocols/dmap/test_dmap_pairing.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/tests/protocols/dmap/test_dmap_scan.py` & `pyatv-0.9.8/tests/protocols/dmap/test_dmap_scan.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/tests/protocols/dmap/test_parser.py` & `pyatv-0.9.8/tests/protocols/dmap/test_parser.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/tests/protocols/mrp/conftest.py` & `pyatv-0.9.8/tests/protocols/mrp/conftest.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/tests/protocols/mrp/test_mrp.py` & `pyatv-0.9.8/tests/protocols/mrp/test_mrp.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/tests/protocols/mrp/test_mrp_auth.py` & `pyatv-0.9.8/tests/protocols/mrp/test_mrp_auth.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/tests/protocols/mrp/test_mrp_functional.py` & `pyatv-0.9.8/tests/protocols/mrp/test_mrp_functional.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/tests/protocols/mrp/test_mrp_interface.py` & `pyatv-0.9.8/tests/protocols/mrp/test_mrp_interface.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/tests/protocols/mrp/test_mrp_scan.py` & `pyatv-0.9.8/tests/protocols/mrp/test_mrp_scan.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/tests/protocols/mrp/test_player_state.py` & `pyatv-0.9.8/tests/protocols/mrp/test_player_state.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/tests/protocols/mrp/test_protocol.py` & `pyatv-0.9.8/tests/protocols/mrp/test_protocol.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/tests/protocols/raop/conftest.py` & `pyatv-0.9.8/tests/protocols/raop/conftest.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/tests/protocols/raop/test_fifo.py` & `pyatv-0.9.8/tests/protocols/raop/test_fifo.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/tests/protocols/raop/test_parsers.py` & `pyatv-0.9.8/tests/protocols/raop/test_parsers.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/tests/protocols/raop/test_raop.py` & `pyatv-0.9.8/tests/protocols/raop/test_raop.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/tests/protocols/raop/test_raop_functional.py` & `pyatv-0.9.8/tests/protocols/raop/test_raop_functional.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 PROGRESS_FIELDS = [FeatureName.Position, FeatureName.TotalTime]
 VOLUME_FIELDS = [
     FeatureName.SetVolume,
     FeatureName.Volume,
     FeatureName.VolumeUp,
     FeatureName.VolumeDown,
 ]
-REMOTE_CONTROL_FIELDS = [FeatureName.Stop]
+REMOTE_CONTROL_FIELDS = [FeatureName.Stop, FeatureName.Pause]
 
 
 @pytest.fixture(name="playing_listener")
 async def playing_listener_fixture(raop_client):
     class PlayingListener(PushListener):
         def __init__(self):
             """Initialize a new PlayingListener instance."""
@@ -543,21 +543,24 @@
     assert raop_state.metadata.album == "raop"
     assert raop_state.metadata.title == "pyatv"
 
     # TODO: stability problems here, need to look into it
     # assert await audio_matches(raop_state.raw_audio, frames=FRAMES_PER_PACKET)
 
 
-@pytest.mark.parametrize("raop_properties", [({"et": "0"})])
-async def test_stop_playback(raop_client, raop_state):
+@pytest.mark.parametrize(
+    "raop_properties,button",
+    [({"et": "0"}, "stop"), ({"et": "0"}, "pause")],  # We treat pause as stop for now
+)
+async def test_stop_playback(raop_client, raop_state, button):
     async def _fake_sleep(time: float = None, loop=None):
         async def dummy():
             pass
 
-        await raop_client.remote_control.stop()
+        await getattr(raop_client.remote_control, button)()
         await asyncio.ensure_future(dummy())
 
     # The idea here is to simulate calling "stop" after the first frame has been sent,
     # i.e. after the first "sleep" has been made. It's a bit tied to implementation
     # details but good enough.
     stub_sleep(fn=_fake_sleep)
```

### Comparing `pyatv-0.9.7/tests/protocols/raop/test_raop_scan.py` & `pyatv-0.9.8/tests/protocols/raop/test_raop_scan.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/tests/scripts/script_env.py` & `pyatv-0.9.8/tests/scripts/script_env.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/tests/scripts/test_atvremote.py` & `pyatv-0.9.8/tests/scripts/test_atvremote.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/tests/scripts/test_atvscript.py` & `pyatv-0.9.8/tests/scripts/test_atvscript.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/tests/support/dns_utils.py` & `pyatv-0.9.8/tests/support/dns_utils.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/tests/support/test_cache.py` & `pyatv-0.9.8/tests/support/test_cache.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/tests/support/test_collections.py` & `pyatv-0.9.8/tests/support/test_collections.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/tests/support/test_device_info.py` & `pyatv-0.9.8/tests/support/test_device_info.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/tests/support/test_dns.py` & `pyatv-0.9.8/tests/support/test_dns.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/tests/support/test_http.py` & `pyatv-0.9.8/tests/support/test_http.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/tests/support/test_net.py` & `pyatv-0.9.8/tests/support/test_net.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from ipaddress import IPv4Address, ip_address
 import platform
 import socket
 import sys
 from typing import Dict, List
 from unittest.mock import patch
 
-import netifaces
+from ifaddr import IP, Adapter
 import pytest
 
 from pyatv.exceptions import NotSupportedError
 from pyatv.support.net import get_private_addresses, tcp_keepalive
 
 skip_darwin = pytest.mark.skipif(
     platform.system() == "Darwin",
@@ -30,34 +30,23 @@
         ),
         reason="Windows build number too low",
     )
 
 
 @pytest.fixture(autouse=True)
 def mock_address():
+    adapters: List[Adapter] = []
     addresses: Dict[str, List[str]] = {}
 
-    def _add(interface: str, address: IPv4Address):
-        addresses.setdefault(interface, []).append(address)
+    def _add(interface: str, address: str):
+        adapters.append(Adapter(interface, interface, [IP(address, 32, interface)]))
 
-    def _ifaddresses(interface: str):
-        iface_addresses = addresses.get(interface)
-        if not iface_addresses:
-            return {}
-
-        inet_addresses = [
-            {"addr": str(addr), "netmask": "255.255.255.0"} for addr in iface_addresses
-        ]
-        return {netifaces.AF_INET: inet_addresses}
-
-    with patch("netifaces.interfaces") as mock_interfaces:
-        with patch("netifaces.ifaddresses") as mock_ifaddr:
-            mock_interfaces.side_effect = lambda: list(addresses.keys())
-            mock_ifaddr.side_effect = _ifaddresses
-            yield _add
+    with patch("pyatv.support.net.get_adapters") as mock_adapters:
+        mock_adapters.side_effect = lambda: adapters
+        yield _add
 
 
 @pytest.fixture
 def mock_server():
     sock = socket.socket()
     # 127.0.0.1 *must* be used when testing on macOS
     sock.bind(("127.0.0.1", 0))
@@ -86,14 +75,23 @@
     assert get_private_addresses() == [
         ip_address("10.0.0.1"),
         ip_address("192.168.0.1"),
         ip_address("172.16.0.1"),
     ]
 
 
+def test_private_addresses(mock_address):
+    mock_address("wlan0", "10.0.0.1")
+    mock_address("lo", "127.0.0.1")
+
+    assert get_private_addresses(include_loopback=False) == [
+        ip_address("10.0.0.1"),
+    ]
+
+
 def test_public_addresses(mock_address):
     mock_address("eth0", "1.2.3.4")
     mock_address("eth1", "8.8.8.8")
     assert get_private_addresses() == []
 
 
 def test_localhost(mock_address):
```

### Comparing `pyatv-0.9.7/tests/support/test_packet.py` & `pyatv-0.9.8/tests/support/test_packet.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/tests/support/test_state_producer.py` & `pyatv-0.9.8/tests/support/test_state_producer.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/tests/support/test_support.py` & `pyatv-0.9.8/tests/support/test_support.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/tests/support/test_variant.py` & `pyatv-0.9.8/tests/support/test_variant.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/tests/test_conf.py` & `pyatv-0.9.8/tests/test_conf.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/tests/test_convert.py` & `pyatv-0.9.8/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/tests/test_helpers.py` & `pyatv-0.9.8/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/tests/test_interface.py` & `pyatv-0.9.8/tests/test_interface.py`

 * *Files 7% similar despite different names*

```diff
@@ -77,31 +77,14 @@
         if feature not in self.feature_map:
             state = FeatureState.Unsupported
         else:
             state = self.feature_map[feature]
         return FeatureInfo(state=state)
 
 
-class PushUpdaterDummy(interface.PushUpdater):
-    def active(self) -> bool:
-        """Return if push updater has been started."""
-        raise exceptions.NotSupportedError()
-
-    def start(self, initial_delay: int = 0) -> None:
-        """Begin to listen to updates.
-
-        If an error occurs, start must be called again.
-        """
-        raise exceptions.NotSupportedError()
-
-    def stop(self) -> None:
-        """No longer forward updates to listener."""
-        raise exceptions.NotSupportedError()
-
-
 @pytest.fixture
 def methods():
     yield interface.retrieve_commands(TestClass)
 
 
 # COMMANDS
 
@@ -440,27 +423,7 @@
     assert App(None, None) != "test"
     assert App(None, None) == App(None, None)
     assert App("test", None) != App(None, None)
     assert App("test", None) == App("test", None)
     assert App(None, "test") != App(None, None)
     assert App(None, "test") == App(None, "test")
     assert App("test", "test2") == App("test", "test2")
-
-
-# PUSH UPDATER
-
-
-@pytest.mark.parametrize("updates", [1, 2, 3])
-def test_post_ignore_duplicate_update(event_loop, updates):
-    listener = MagicMock()
-    playing = Playing()
-
-    async def _post_updates(repeats: int):
-        updater = PushUpdaterDummy(event_loop)
-        updater.listener = listener
-        for _ in range(repeats):
-            updater.post_update(playing)
-
-    event_loop.run_until_complete(_post_updates(updates))
-
-    assert listener.playstatus_update.call_count == 1
-    listener.playstatus_update.assert_called_once_with(ANY, playing)
```

### Comparing `pyatv-0.9.7/tests/test_scan_functional.py` & `pyatv-0.9.8/tests/test_scan_functional.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/tests/utils.py` & `pyatv-0.9.8/tests/utils.py`

 * *Files identical despite different names*

### Comparing `pyatv-0.9.7/tests/zeroconf_stub.py` & `pyatv-0.9.8/tests/zeroconf_stub.py`

 * *Files identical despite different names*

