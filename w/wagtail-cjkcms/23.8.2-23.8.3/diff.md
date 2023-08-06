# Comparing `tmp/wagtail-cjkcms-23.8.2.tar.gz` & `tmp/wagtail-cjkcms-23.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-cjkcms-23.8.2.tar", last modified: Fri Aug  4 21:45:20 2023, max compression
+gzip compressed data, was "wagtail-cjkcms-23.8.3.tar", last modified: Sat Aug  5 15:14:10 2023, max compression
```

## Comparing `wagtail-cjkcms-23.8.2.tar` & `wagtail-cjkcms-23.8.3.tar`

### file list

```diff
@@ -1,399 +1,399 @@
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.949976 wagtail-cjkcms-23.8.2/
--rw-r--r--   0 grze      (1000) grze      (1000)     8339 2023-08-04 21:44:44.000000 wagtail-cjkcms-23.8.2/CHANGELOG.md
--rw-r--r--   0 grze      (1000) grze      (1000)     1542 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/LICENSE
--rw-r--r--   0 grze      (1000) grze      (1000)      158 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/MANIFEST.in
--rw-r--r--   0 grze      (1000) grze      (1000)     4857 2023-08-04 21:45:20.949976 wagtail-cjkcms-23.8.2/PKG-INFO
--rw-r--r--   0 grze      (1000) grze      (1000)     1884 2023-08-02 09:54:30.000000 wagtail-cjkcms-23.8.2/README.md
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.895809 wagtail-cjkcms-23.8.2/cjkcms/
--rw-r--r--   0 grze      (1000) grze      (1000)      272 2023-08-04 21:42:19.000000 wagtail-cjkcms-23.8.2/cjkcms/__init__.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.895809 wagtail-cjkcms-23.8.2/cjkcms/api/
--rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/api/__init__.py
--rw-r--r--   0 grze      (1000) grze      (1000)     2832 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/api/mailchimp.py
--rw-r--r--   0 grze      (1000) grze      (1000)      173 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/apps.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.895809 wagtail-cjkcms-23.8.2/cjkcms/bin/
--rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/bin/__init__.py
--rw-r--r--   0 grze      (1000) grze      (1000)     5752 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/bin/cjkcms.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.895809 wagtail-cjkcms-23.8.2/cjkcms/blocks/
--rw-r--r--   0 grze      (1000) grze      (1000)     3223 2023-08-04 20:26:53.000000 wagtail-cjkcms-23.8.2/cjkcms/blocks/__init__.py
--rw-r--r--   0 grze      (1000) grze      (1000)    10539 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/blocks/base_blocks.py
--rw-r--r--   0 grze      (1000) grze      (1000)     8757 2023-08-04 21:37:50.000000 wagtail-cjkcms-23.8.2/cjkcms/blocks/content_blocks.py
--rw-r--r--   0 grze      (1000) grze      (1000)     9537 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/blocks/html_blocks.py
--rw-r--r--   0 grze      (1000) grze      (1000)     3337 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/blocks/layout_blocks.py
--rw-r--r--   0 grze      (1000) grze      (1000)      171 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/blocks/searchable_html_block.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.895809 wagtail-cjkcms-23.8.2/cjkcms/draftail/
--rw-r--r--   0 grze      (1000) grze      (1000)      305 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/draftail/__init__.py
--rw-r--r--   0 grze      (1000) grze      (1000)     3157 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/draftail/draftail_extensions.py
--rw-r--r--   0 grze      (1000) grze      (1000)     5157 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/draftail/draftail_icons.py
--rw-r--r--   0 grze      (1000) grze      (1000)     3191 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/fields.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.895809 wagtail-cjkcms-23.8.2/cjkcms/finders/
--rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/finders/__init__.py
--rw-r--r--   0 grze      (1000) grze      (1000)     2459 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/finders/oembed.py
--rw-r--r--   0 grze      (1000) grze      (1000)      361 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/forms.py
--rw-r--r--   0 grze      (1000) grze      (1000)     1804 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/image_formats.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.874143 wagtail-cjkcms-23.8.2/cjkcms/management/
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.895809 wagtail-cjkcms-23.8.2/cjkcms/management/commands/
--rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/management/commands/__init__.py
--rw-r--r--   0 grze      (1000) grze      (1000)      453 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/management/commands/clear-embeds.py
--rw-r--r--   0 grze      (1000) grze      (1000)     2565 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/management/commands/import-csv.py
--rw-r--r--   0 grze      (1000) grze      (1000)      952 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/management/commands/init-collections.py
--rw-r--r--   0 grze      (1000) grze      (1000)     3560 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/management/commands/init-navbar.py
--rw-r--r--   0 grze      (1000) grze      (1000)     3820 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/management/commands/init-website.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.874143 wagtail-cjkcms-23.8.2/cjkcms/media/
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.895809 wagtail-cjkcms-23.8.2/cjkcms/media/images/
--rw-r--r--   0 grze      (1000) grze      (1000)     1938 2023-08-04 21:41:03.000000 wagtail-cjkcms-23.8.2/cjkcms/media/images/test.original.png
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.895809 wagtail-cjkcms-23.8.2/cjkcms/media/original_images/
--rw-r--r--   0 grze      (1000) grze      (1000)     2306 2023-08-04 21:41:03.000000 wagtail-cjkcms-23.8.2/cjkcms/media/original_images/test.png
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.895809 wagtail-cjkcms-23.8.2/cjkcms/migrations/
--rw-r--r--   0 grze      (1000) grze      (1000)   216350 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/migrations/0001_initial.py
--rw-r--r--   0 grze      (1000) grze      (1000)      835 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/migrations/0002_alter_body_to_cjkcmsstreamfield.py
--rw-r--r--   0 grze      (1000) grze      (1000)      668 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/migrations/0003_alter_footer_content_alter_navbar_menu_items.py
--rw-r--r--   0 grze      (1000) grze      (1000)     1027 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/migrations/0004_layoutsettings_articles_date_format_and_more.py
--rw-r--r--   0 grze      (1000) grze      (1000)     1709 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/migrations/0005_layoutsettings_custom_font_and_more.py
--rw-r--r--   0 grze      (1000) grze      (1000)     2886 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/migrations/0006_analyticssettings_consent_modal_layout_and_more.py
--rw-r--r--   0 grze      (1000) grze      (1000)      594 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/migrations/0007_layoutsettings_bootstrap_icons.py
--rw-r--r--   0 grze      (1000) grze      (1000)     1334 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/migrations/0008_alter_layoutsettings_navbar_langselector.py
--rw-r--r--   0 grze      (1000) grze      (1000)      685 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/migrations/0009_navbar_language.py
--rw-r--r--   0 grze      (1000) grze      (1000)     3479 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/migrations/0010_filmstrip_filmpanel.py
--rw-r--r--   0 grze      (1000) grze      (1000)     1393 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/migrations/0011_cjkcmspage_related_classifier_term_and_more.py
--rw-r--r--   0 grze      (1000) grze      (1000)     1466 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/migrations/0012_remove_analyticssettings_ga_tracking_id_and_more.py
--rw-r--r--   0 grze      (1000) grze      (1000)      780 2023-08-04 20:23:14.000000 wagtail-cjkcms-23.8.2/cjkcms/migrations/0013_socialmediasettings_location.py
--rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/migrations/__init__.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.895809 wagtail-cjkcms-23.8.2/cjkcms/models/
--rw-r--r--   0 grze      (1000) grze      (1000)      232 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/models/__init__.py
--rw-r--r--   0 grze      (1000) grze      (1000)      392 2023-08-04 11:19:34.000000 wagtail-cjkcms-23.8.2/cjkcms/models/admin_sidebar.py
--rw-r--r--   0 grze      (1000) grze      (1000)     2356 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/models/cms_models.py
--rw-r--r--   0 grze      (1000) grze      (1000)     6302 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/models/integration_models.py
--rw-r--r--   0 grze      (1000) grze      (1000)    23813 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/models/page_models.py
--rw-r--r--   0 grze      (1000) grze      (1000)    15371 2023-08-04 11:17:41.000000 wagtail-cjkcms-23.8.2/cjkcms/models/snippet_models.py
--rw-r--r--   0 grze      (1000) grze      (1000)    19301 2023-08-04 20:16:16.000000 wagtail-cjkcms-23.8.2/cjkcms/models/wagtailsettings_models.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.874143 wagtail-cjkcms-23.8.2/cjkcms/project_template/
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.895809 wagtail-cjkcms-23.8.2/cjkcms/project_template/basic/
--rw-r--r--   0 grze      (1000) grze      (1000)      722 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/basic/.editorconfig
--rw-r--r--   0 grze      (1000) grze      (1000)      364 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/basic/.gitattributes
--rw-r--r--   0 grze      (1000) grze      (1000)      275 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/basic/.gitignore
--rw-r--r--   0 grze      (1000) grze      (1000)      792 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/basic/README.md
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.895809 wagtail-cjkcms-23.8.2/cjkcms/project_template/basic/home/
--rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/basic/home/__init__.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.895809 wagtail-cjkcms-23.8.2/cjkcms/project_template/basic/home/blocks/
--rw-r--r--   0 grze      (1000) grze      (1000)      137 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/basic/home/blocks/__init__.py
--rw-r--r--   0 grze      (1000) grze      (1000)     2141 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/basic/home/blocks/blocks.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.895809 wagtail-cjkcms-23.8.2/cjkcms/project_template/basic/home/migrations/
--rw-r--r--   0 grze      (1000) grze      (1000)     4982 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/basic/home/migrations/0001_initial.py
--rw-r--r--   0 grze      (1000) grze      (1000)     2047 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/basic/home/migrations/0002_create_homepage.py
--rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/basic/home/migrations/__init__.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.895809 wagtail-cjkcms-23.8.2/cjkcms/project_template/basic/home/models/
--rw-r--r--   0 grze      (1000) grze      (1000)      295 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/basic/home/models/__init__.py
--rw-r--r--   0 grze      (1000) grze      (1000)     2819 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/basic/home/models/cms_models.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.874143 wagtail-cjkcms-23.8.2/cjkcms/project_template/basic/home/templates/
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.874143 wagtail-cjkcms-23.8.2/cjkcms/project_template/basic/home/templates/home/
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.895809 wagtail-cjkcms-23.8.2/cjkcms/project_template/basic/home/templates/home/blocks/
--rw-r--r--   0 grze      (1000) grze      (1000)     2282 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/basic/home/templates/home/blocks/event_presentation.html
--rw-r--r--   0 grze      (1000) grze      (1000)      678 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/basic/manage.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.906643 wagtail-cjkcms-23.8.2/cjkcms/project_template/basic/project_name/
--rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/basic/project_name/__init__.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.906643 wagtail-cjkcms-23.8.2/cjkcms/project_template/basic/project_name/settings/
--rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/basic/project_name/settings/__init__.py
--rw-r--r--   0 grze      (1000) grze      (1000)     5312 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/basic/project_name/settings/base.py
--rw-r--r--   0 grze      (1000) grze      (1000)      324 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/basic/project_name/settings/dev.py
--rw-r--r--   0 grze      (1000) grze      (1000)      705 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/basic/project_name/settings/local.py
--rw-r--r--   0 grze      (1000) grze      (1000)     1595 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/basic/project_name/settings/production.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.874143 wagtail-cjkcms-23.8.2/cjkcms/project_template/basic/project_name/static/
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.906643 wagtail-cjkcms-23.8.2/cjkcms/project_template/basic/project_name/static/css/
--rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/basic/project_name/static/css/devsite.css
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.906643 wagtail-cjkcms-23.8.2/cjkcms/project_template/basic/project_name/static/js/
--rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/basic/project_name/static/js/devsite.js
--rw-r--r--   0 grze      (1000) grze      (1000)      911 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/basic/project_name/urls.py
--rw-r--r--   0 grze      (1000) grze      (1000)      438 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/basic/project_name/wsgi.py
--rw-r--r--   0 grze      (1000) grze      (1000)      123 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/basic/requirements.txt
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.906643 wagtail-cjkcms-23.8.2/cjkcms/project_template/basic/search/
--rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/basic/search/__init__.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.874143 wagtail-cjkcms-23.8.2/cjkcms/project_template/basic/search/templates/
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.906643 wagtail-cjkcms-23.8.2/cjkcms/project_template/basic/search/templates/search/
--rw-r--r--   0 grze      (1000) grze      (1000)     1097 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/basic/search/templates/search/search.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1019 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/basic/search/views.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.906643 wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/
--rw-r--r--   0 grze      (1000) grze      (1000)      245 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/.babelrc
--rw-r--r--   0 grze      (1000) grze      (1000)      159 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/.browserslistrc
--rw-r--r--   0 grze      (1000) grze      (1000)      722 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/.editorconfig
--rw-r--r--   0 grze      (1000) grze      (1000)      277 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/.eslintrc
--rw-r--r--   0 grze      (1000) grze      (1000)      364 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/.gitattributes
--rw-r--r--   0 grze      (1000) grze      (1000)      270 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/.gitignore
--rw-r--r--   0 grze      (1000) grze      (1000)       13 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/.nvmrc
--rw-r--r--   0 grze      (1000) grze      (1000)      182 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/.stylelintrc.json
--rw-r--r--   0 grze      (1000) grze      (1000)      792 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/README.md
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.906643 wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/frontend/
--rw-r--r--   0 grze      (1000) grze      (1000)      131 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/frontend/.gitignore
--rw-r--r--   0 grze      (1000) grze      (1000)      733 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/frontend/README.md
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.884976 wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/frontend/src/
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.906643 wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/frontend/src/application/
--rw-r--r--   0 grze      (1000) grze      (1000)      574 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/frontend/src/application/app.js
--rw-r--r--   0 grze      (1000) grze      (1000)      226 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/frontend/src/application/app2.js
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.906643 wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/frontend/src/components/
--rw-r--r--   0 grze      (1000) grze      (1000)       41 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/frontend/src/components/sidebar.js
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.906643 wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/frontend/src/styles/
--rw-r--r--   0 grze      (1000) grze      (1000)      380 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/frontend/src/styles/index.scss
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.906643 wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/frontend/vendors/
--rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/frontend/vendors/.gitkeep
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.906643 wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/frontend/vendors/images/
--rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/frontend/vendors/images/.gitkeep
--rw-r--r--   0 grze      (1000) grze      (1000)   273404 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/frontend/vendors/images/sample.jpg
--rw-r--r--   0 grze      (1000) grze      (1000)   238213 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/frontend/vendors/images/webpack.png
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.906643 wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/frontend/webpack/
--rw-r--r--   0 grze      (1000) grze      (1000)     1473 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/frontend/webpack/webpack.common.js
--rw-r--r--   0 grze      (1000) grze      (1000)     1716 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/frontend/webpack/webpack.config.dev.js
--rw-r--r--   0 grze      (1000) grze      (1000)      986 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/frontend/webpack/webpack.config.prod.js
--rw-r--r--   0 grze      (1000) grze      (1000)     1485 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/frontend/webpack/webpack.config.watch.js
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.906643 wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/home/
--rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/home/__init__.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.906643 wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/home/blocks/
--rw-r--r--   0 grze      (1000) grze      (1000)      137 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/home/blocks/__init__.py
--rw-r--r--   0 grze      (1000) grze      (1000)     2141 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/home/blocks/blocks.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.906643 wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/home/migrations/
--rw-r--r--   0 grze      (1000) grze      (1000)     4982 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/home/migrations/0001_initial.py
--rw-r--r--   0 grze      (1000) grze      (1000)     2047 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/home/migrations/0002_create_homepage.py
--rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/home/migrations/__init__.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.906643 wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/home/models/
--rw-r--r--   0 grze      (1000) grze      (1000)      295 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/home/models/__init__.py
--rw-r--r--   0 grze      (1000) grze      (1000)     2819 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/home/models/cms_models.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.884976 wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/home/templates/
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.884976 wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/home/templates/home/
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.906643 wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/home/templates/home/blocks/
--rw-r--r--   0 grze      (1000) grze      (1000)     2282 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/home/templates/home/blocks/event_presentation.html
--rw-r--r--   0 grze      (1000) grze      (1000)      678 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/manage.py
--rw-r--r--   0 grze      (1000) grze      (1000)   683340 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/package-lock.json
--rw-r--r--   0 grze      (1000) grze      (1000)     1741 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/package.json
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.917476 wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/project_name/
--rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/project_name/__init__.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.917476 wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/project_name/settings/
--rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/project_name/settings/__init__.py
--rw-r--r--   0 grze      (1000) grze      (1000)     5312 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/project_name/settings/base.py
--rw-r--r--   0 grze      (1000) grze      (1000)      324 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/project_name/settings/dev.py
--rw-r--r--   0 grze      (1000) grze      (1000)      705 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/project_name/settings/local.py
--rw-r--r--   0 grze      (1000) grze      (1000)     1595 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/project_name/settings/production.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.884976 wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/project_name/static/
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.917476 wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/project_name/static/css/
--rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/project_name/static/css/devsite.css
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.917476 wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/project_name/static/js/
--rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/project_name/static/js/devsite.js
--rw-r--r--   0 grze      (1000) grze      (1000)      911 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/project_name/urls.py
--rw-r--r--   0 grze      (1000) grze      (1000)      438 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/project_name/wsgi.py
--rw-r--r--   0 grze      (1000) grze      (1000)      123 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/requirements.txt
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.917476 wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/search/
--rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/search/__init__.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.884976 wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/search/templates/
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.917476 wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/search/templates/search/
--rw-r--r--   0 grze      (1000) grze      (1000)     1097 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/search/templates/search/search.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1019 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/search/views.py
--rw-r--r--   0 grze      (1000) grze      (1000)      125 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/search_urls.py
--rw-r--r--   0 grze      (1000) grze      (1000)     9799 2023-08-04 20:22:09.000000 wagtail-cjkcms-23.8.2/cjkcms/settings.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.884976 wagtail-cjkcms-23.8.2/cjkcms/static/
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.884976 wagtail-cjkcms-23.8.2/cjkcms/static/cjkcms/
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.917476 wagtail-cjkcms-23.8.2/cjkcms/static/cjkcms/bi/
--rw-r--r--   0 grze      (1000) grze      (1000)    93729 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/static/cjkcms/bi/bootstrap-icons.css
--rw-r--r--   0 grze      (1000) grze      (1000)    49971 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/static/cjkcms/bi/bootstrap-icons.json
--rw-r--r--   0 grze      (1000) grze      (1000)    55169 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/static/cjkcms/bi/bootstrap-icons.scss
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.917476 wagtail-cjkcms-23.8.2/cjkcms/static/cjkcms/bi/fonts/
--rw-r--r--   0 grze      (1000) grze      (1000)   164360 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/static/cjkcms/bi/fonts/bootstrap-icons.woff
--rw-r--r--   0 grze      (1000) grze      (1000)   121340 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/static/cjkcms/bi/fonts/bootstrap-icons.woff2
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.917476 wagtail-cjkcms-23.8.2/cjkcms/static/cjkcms/css/
--rw-r--r--   0 grze      (1000) grze      (1000)      846 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/static/cjkcms/css/cjkcms-admin.css
--rw-r--r--   0 grze      (1000) grze      (1000)     1104 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/static/cjkcms/css/cjkcms-editor.css
--rw-r--r--   0 grze      (1000) grze      (1000)     4614 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/static/cjkcms/css/cjkcms-front.css
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.884976 wagtail-cjkcms-23.8.2/cjkcms/static/cjkcms/images/
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.917476 wagtail-cjkcms-23.8.2/cjkcms/static/cjkcms/images/avatars/
--rw-r--r--   0 grze      (1000) grze      (1000)      535 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/static/cjkcms/images/avatars/default.png
--rw-r--r--   0 grze      (1000) grze      (1000)      384 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/static/cjkcms/images/avatars/default.svg
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.917476 wagtail-cjkcms-23.8.2/cjkcms/static/cjkcms/images/icons/
--rw-r--r--   0 grze      (1000) grze      (1000)      705 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/static/cjkcms/images/icons/quote.svg
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.917476 wagtail-cjkcms-23.8.2/cjkcms/static/cjkcms/images/logos/
--rw-r--r--   0 grze      (1000) grze      (1000)     4166 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/static/cjkcms/images/logos/cms-logo-long.svg
--rw-r--r--   0 grze      (1000) grze      (1000)     4218 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/static/cjkcms/images/logos/cms-logo-square.svg
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.917476 wagtail-cjkcms-23.8.2/cjkcms/static/cjkcms/images/patterns/
--rw-r--r--   0 grze      (1000) grze      (1000)    47935 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/static/cjkcms/images/patterns/pattern1.jpg
--rw-r--r--   0 grze      (1000) grze      (1000)    31707 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/static/cjkcms/images/patterns/pattern2.jpg
--rw-r--r--   0 grze      (1000) grze      (1000)    38190 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/static/cjkcms/images/patterns/pattern3.jpg
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.917476 wagtail-cjkcms-23.8.2/cjkcms/static/cjkcms/js/
--rw-r--r--   0 grze      (1000) grze      (1000)      444 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/static/cjkcms/js/cjkcms-editor.js
--rw-r--r--   0 grze      (1000) grze      (1000)     5565 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/static/cjkcms/js/cjkcms-front.js
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.917476 wagtail-cjkcms-23.8.2/cjkcms/static/cookieconsent/
--rw-r--r--   0 grze      (1000) grze      (1000)    18803 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/static/cookieconsent/cookieconsent.css
--rw-r--r--   0 grze      (1000) grze      (1000)    18743 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/static/cookieconsent/cookieconsent.js
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.928309 wagtail-cjkcms-23.8.2/cjkcms/templates/
--rw-r--r--   0 grze      (1000) grze      (1000)     4176 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/404.html
--rw-r--r--   0 grze      (1000) grze      (1000)     4802 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/500.html
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.928309 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.928309 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/
--rw-r--r--   0 grze      (1000) grze      (1000)     1443 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/accordion_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      974 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/article_block_card.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1132 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/article_masonry_card.html
--rw-r--r--   0 grze      (1000) grze      (1000)      188 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/base_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)     2634 2023-08-04 20:24:22.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/base_link_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      740 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/button_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      746 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/card_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      856 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/card_blurb.html
--rw-r--r--   0 grze      (1000) grze      (1000)      786 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/card_foot.html
--rw-r--r--   0 grze      (1000) grze      (1000)      730 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/card_head.html
--rw-r--r--   0 grze      (1000) grze      (1000)      771 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/card_head_foot.html
--rw-r--r--   0 grze      (1000) grze      (1000)      990 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/card_horizontal.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1104 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/card_horizontal2.html
--rw-r--r--   0 grze      (1000) grze      (1000)      786 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/card_img.html
--rw-r--r--   0 grze      (1000) grze      (1000)     2618 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/card_landing1.html
--rw-r--r--   0 grze      (1000) grze      (1000)     2758 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/card_landing2.html
--rw-r--r--   0 grze      (1000) grze      (1000)      678 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/cardgrid_columns.html
--rw-r--r--   0 grze      (1000) grze      (1000)      450 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/cardgrid_deck.html
--rw-r--r--   0 grze      (1000) grze      (1000)      277 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/cardgrid_group.html
--rw-r--r--   0 grze      (1000) grze      (1000)      276 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/cardgrid_zero.html
--rw-r--r--   0 grze      (1000) grze      (1000)     2698 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/carousel_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      406 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/column_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      137 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/document_link_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      920 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/download_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      103 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/embed_video_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)       95 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/external_link_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1484 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/film_strip_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      424 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/grid_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      200 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/h1_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      200 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/h2_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      200 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/h3_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      790 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/hero_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      275 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/image_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1400 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/image_gallery_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      627 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/image_link_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1020 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/modal_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      164 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/page_link_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      787 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/pagelist_article_card_columns.html
--rw-r--r--   0 grze      (1000) grze      (1000)      642 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/pagelist_article_card_deck.html
--rw-r--r--   0 grze      (1000) grze      (1000)      361 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/pagelist_article_card_group.html
--rw-r--r--   0 grze      (1000) grze      (1000)      956 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/pagelist_article_media.html
--rw-r--r--   0 grze      (1000) grze      (1000)      858 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/pagelist_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      610 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/pagelist_list_group.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1224 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/pagelist_toc_nextprev.html
--rw-r--r--   0 grze      (1000) grze      (1000)      200 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/pagepreview_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      793 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/pagepreview_card.html
--rw-r--r--   0 grze      (1000) grze      (1000)      244 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/pricelist_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      513 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/pricelistitem_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      353 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/quote_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      852 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/quote_block_leftbar.html
--rw-r--r--   0 grze      (1000) grze      (1000)      998 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/quote_block_start_end_quote.html
--rw-r--r--   0 grze      (1000) grze      (1000)      216 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/reusable_content_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)       91 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/rich_text_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1095 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/table_block.html
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.928309 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/cookieconsent/
--rw-r--r--   0 grze      (1000) grze      (1000)     3672 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/cookieconsent/languages.html
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.928309 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/formfields/
--rw-r--r--   0 grze      (1000) grze      (1000)      267 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/formfields/date.html
--rw-r--r--   0 grze      (1000) grze      (1000)      416 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/formfields/datetime.html
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.939143 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/formfields/mailchimp/
--rw-r--r--   0 grze      (1000) grze      (1000)     9267 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/formfields/mailchimp/_2vanilla_subscriber_integration_js.html
--rw-r--r--   0 grze      (1000) grze      (1000)     6469 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/formfields/mailchimp/subscriber_integration_js.html
--rw-r--r--   0 grze      (1000) grze      (1000)      793 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/formfields/mailchimp/subscriber_integration_widget.html
--rw-r--r--   0 grze      (1000) grze      (1000)      264 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/formfields/time.html
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.939143 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/icons/
--rw-r--r--   0 grze      (1000) grze      (1000)      465 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/icons/align-left.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      573 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/icons/check-square-o.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      277 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/icons/columns.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      359 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/icons/desktop.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      571 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/icons/font.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      292 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/icons/google.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      813 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/icons/hand-pointer-o.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      666 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/icons/hashtag.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      840 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/icons/header.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      835 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/icons/list-alt.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      459 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/icons/map.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      448 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/icons/newspaper-o.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      721 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/icons/puzzle-piece.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      635 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/icons/recycle.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      174 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/icons/stop.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      505 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/icons/th-large.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      762 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/icons/universal-access.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      548 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/icons/usd.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      225 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/icons/window-maximize.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      199 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/icons/window-minimize.svg
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.939143 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/includes/
--rw-r--r--   0 grze      (1000) grze      (1000)      286 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/includes/cjkcms_banner.html
--rw-r--r--   0 grze      (1000) grze      (1000)      689 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/includes/classifier_dropdowns.html
--rw-r--r--   0 grze      (1000) grze      (1000)      579 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/includes/classifier_nav.html
--rw-r--r--   0 grze      (1000) grze      (1000)      286 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/includes/codered_banner.html
--rw-r--r--   0 grze      (1000) grze      (1000)      268 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/includes/form_honeypot.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1061 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/includes/pagination.html
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.939143 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/includes/stream_forms/
--rw-r--r--   0 grze      (1000) grze      (1000)      532 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/includes/stream_forms/render_field.html
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.939143 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/pages/
--rw-r--r--   0 grze      (1000) grze      (1000)     2002 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/pages/article_index_page.html
--rw-r--r--   0 grze      (1000) grze      (1000)     2031 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/pages/article_page.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1018 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/pages/article_page.search.html
--rw-r--r--   0 grze      (1000) grze      (1000)     9291 2023-08-04 21:16:07.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/pages/base.html
--rw-r--r--   0 grze      (1000) grze      (1000)      248 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/pages/form_page_landing.html
--rw-r--r--   0 grze      (1000) grze      (1000)       50 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/pages/home_page.html
--rw-r--r--   0 grze      (1000) grze      (1000)      491 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/pages/page.mini.html
--rw-r--r--   0 grze      (1000) grze      (1000)     2610 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/pages/search.html
--rw-r--r--   0 grze      (1000) grze      (1000)      582 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/pages/search_result.html
--rw-r--r--   0 grze      (1000) grze      (1000)      594 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/pages/web_page.html
--rw-r--r--   0 grze      (1000) grze      (1000)      200 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/pages/web_page_notitle.html
--rw-r--r--   0 grze      (1000) grze      (1000)      122 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/robots.txt
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.939143 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/snippets/
--rw-r--r--   0 grze      (1000) grze      (1000)     1943 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/snippets/bottom_corner_lang_selector.html
--rw-r--r--   0 grze      (1000) grze      (1000)      430 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/snippets/footer.html
--rw-r--r--   0 grze      (1000) grze      (1000)     2027 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/snippets/frontend_assets.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1196 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/snippets/frontend_scripts.html
--rw-r--r--   0 grze      (1000) grze      (1000)     2934 2023-08-04 20:44:06.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/snippets/navbar.html
--rw-r--r--   0 grze      (1000) grze      (1000)      836 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/snippets/navbar_lang_selector.html
--rw-r--r--   0 grze      (1000) grze      (1000)      386 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/snippets/navbar_search.html
--rw-r--r--   0 grze      (1000) grze      (1000)      330 2023-08-04 21:22:38.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/snippets/social_media.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1875 2023-08-04 21:26:54.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/snippets/social_media_icons.html
--rw-r--r--   0 grze      (1000) grze      (1000)      171 2023-08-04 21:23:34.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/snippets/social_media_nav_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      158 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/snippets/tracking_g3.html
--rw-r--r--   0 grze      (1000) grze      (1000)      832 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/snippets/tracking_g4.html
--rw-r--r--   0 grze      (1000) grze      (1000)      694 2023-08-02 09:54:30.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/snippets/tracking_matomo.html
--rw-r--r--   0 grze      (1000) grze      (1000)      230 2023-08-02 09:54:30.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/snippets/tracking_matomo_noscript.html
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.939143 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/widgets/
--rw-r--r--   0 grze      (1000) grze      (1000)     1444 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/widgets/checkbox_classifiers.html
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.884976 wagtail-cjkcms-23.8.2/cjkcms/templates/wagtailadmin/
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.939143 wagtail-cjkcms-23.8.2/cjkcms/templates/wagtailadmin/block_forms/
--rw-r--r--   0 grze      (1000) grze      (1000)      839 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/wagtailadmin/block_forms/base_block_settings_struct.html
--rw-r--r--   0 grze      (1000) grze      (1000)      550 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/wagtailadmin/block_forms/struct.html
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.939143 wagtail-cjkcms-23.8.2/cjkcms/templates/wagtailadmin/shared/
--rw-r--r--   0 grze      (1000) grze      (1000)      885 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templates/wagtailadmin/shared/cr_main_nav_2fix.html
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.949976 wagtail-cjkcms-23.8.2/cjkcms/templatetags/
--rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templatetags/__init__.py
--rw-r--r--   0 grze      (1000) grze      (1000)      327 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templatetags/auth_extras.py
--rw-r--r--   0 grze      (1000) grze      (1000)     6845 2023-08-04 21:38:58.000000 wagtail-cjkcms-23.8.2/cjkcms/templatetags/cjkcms_tags.py
--rw-r--r--   0 grze      (1000) grze      (1000)     4962 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templatetags/friendly_loader.py
--rw-r--r--   0 grze      (1000) grze      (1000)     1127 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templatetags/gravatar.py
--rw-r--r--   0 grze      (1000) grze      (1000)     1224 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/templatetags/txtutils_tags.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.949976 wagtail-cjkcms-23.8.2/cjkcms/tests/
--rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/tests/__init__.py
--rw-r--r--   0 grze      (1000) grze      (1000)     4226 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/tests/test_articlepages.py
--rw-r--r--   0 grze      (1000) grze      (1000)     3506 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/tests/test_bin.py
--rw-r--r--   0 grze      (1000) grze      (1000)     2629 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/tests/test_gravatar.py
--rw-r--r--   0 grze      (1000) grze      (1000)     4760 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/tests/test_search_blocks.py
--rw-r--r--   0 grze      (1000) grze      (1000)     2665 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/tests/test_settings.py
--rw-r--r--   0 grze      (1000) grze      (1000)     3762 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/tests/test_templatetags.py
--rw-r--r--   0 grze      (1000) grze      (1000)     2673 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/tests/test_urls.py
--rw-r--r--   0 grze      (1000) grze      (1000)     1520 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/tests/test_webpage.py
--rw-r--r--   0 grze      (1000) grze      (1000)      506 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/urls.py
--rw-r--r--   0 grze      (1000) grze      (1000)      573 2023-07-16 21:02:27.000000 wagtail-cjkcms-23.8.2/cjkcms/utils.py
--rw-r--r--   0 grze      (1000) grze      (1000)     4488 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/views.py
--rw-r--r--   0 grze      (1000) grze      (1000)     6613 2023-08-04 11:20:28.000000 wagtail-cjkcms-23.8.2/cjkcms/wagtail_hooks.py
--rw-r--r--   0 grze      (1000) grze      (1000)     1531 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/cjkcms/widgets.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.949976 wagtail-cjkcms-23.8.2/docs/
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.949976 wagtail-cjkcms-23.8.2/docs/how-to/
--rw-r--r--   0 grze      (1000) grze      (1000)     1481 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/docs/how-to/oembed_finder.md
--rw-r--r--   0 grze      (1000) grze      (1000)      537 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/docs/index.md
--rw-r--r--   0 grze      (1000) grze      (1000)     5520 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/docs/installation.md
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.949976 wagtail-cjkcms-23.8.2/docs/management_commands/
--rw-r--r--   0 grze      (1000) grze      (1000)      318 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/docs/management_commands/clear-embeds.md
--rw-r--r--   0 grze      (1000) grze      (1000)      193 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/docs/management_commands/index.md
--rw-r--r--   0 grze      (1000) grze      (1000)      420 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/docs/management_commands/init-collections.md
--rw-r--r--   0 grze      (1000) grze      (1000)      936 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/docs/quick-start.md
--rw-r--r--   0 grze      (1000) grze      (1000)       13 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/docs/requirements.txt
--rw-r--r--   0 grze      (1000) grze      (1000)     1220 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/docs/why-another-cms.md
--rw-r--r--   0 grze      (1000) grze      (1000)     2154 2023-08-02 09:54:30.000000 wagtail-cjkcms-23.8.2/pyproject.toml
--rw-r--r--   0 grze      (1000) grze      (1000)      230 2023-08-04 21:45:20.949976 wagtail-cjkcms-23.8.2/setup.cfg
--rw-r--r--   0 grze      (1000) grze      (1000)       38 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.2/setup.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-04 21:45:20.949976 wagtail-cjkcms-23.8.2/wagtail_cjkcms.egg-info/
--rw-r--r--   0 grze      (1000) grze      (1000)     4857 2023-08-04 21:45:20.000000 wagtail-cjkcms-23.8.2/wagtail_cjkcms.egg-info/PKG-INFO
--rw-r--r--   0 grze      (1000) grze      (1000)    14486 2023-08-04 21:45:20.000000 wagtail-cjkcms-23.8.2/wagtail_cjkcms.egg-info/SOURCES.txt
--rw-r--r--   0 grze      (1000) grze      (1000)        1 2023-08-04 21:45:20.000000 wagtail-cjkcms-23.8.2/wagtail_cjkcms.egg-info/dependency_links.txt
--rw-r--r--   0 grze      (1000) grze      (1000)       50 2023-08-04 21:45:20.000000 wagtail-cjkcms-23.8.2/wagtail_cjkcms.egg-info/entry_points.txt
--rw-r--r--   0 grze      (1000) grze      (1000)      189 2023-08-04 21:45:20.000000 wagtail-cjkcms-23.8.2/wagtail_cjkcms.egg-info/requires.txt
--rw-r--r--   0 grze      (1000) grze      (1000)        7 2023-08-04 21:45:20.000000 wagtail-cjkcms-23.8.2/wagtail_cjkcms.egg-info/top_level.txt
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.504493 wagtail-cjkcms-23.8.3/
+-rw-r--r--   0 grze      (1000) grze      (1000)     8462 2023-08-05 15:13:30.000000 wagtail-cjkcms-23.8.3/CHANGELOG.md
+-rw-r--r--   0 grze      (1000) grze      (1000)     1542 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/LICENSE
+-rw-r--r--   0 grze      (1000) grze      (1000)      158 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/MANIFEST.in
+-rw-r--r--   0 grze      (1000) grze      (1000)     4857 2023-08-05 15:14:10.504493 wagtail-cjkcms-23.8.3/PKG-INFO
+-rw-r--r--   0 grze      (1000) grze      (1000)     1884 2023-08-02 09:54:30.000000 wagtail-cjkcms-23.8.3/README.md
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.444493 wagtail-cjkcms-23.8.3/cjkcms/
+-rw-r--r--   0 grze      (1000) grze      (1000)      272 2023-08-05 15:12:51.000000 wagtail-cjkcms-23.8.3/cjkcms/__init__.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.444493 wagtail-cjkcms-23.8.3/cjkcms/api/
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/api/__init__.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     2832 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/api/mailchimp.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      173 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/apps.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.444493 wagtail-cjkcms-23.8.3/cjkcms/bin/
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/bin/__init__.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     5752 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/bin/cjkcms.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.444493 wagtail-cjkcms-23.8.3/cjkcms/blocks/
+-rw-r--r--   0 grze      (1000) grze      (1000)     3223 2023-08-04 20:26:53.000000 wagtail-cjkcms-23.8.3/cjkcms/blocks/__init__.py
+-rw-r--r--   0 grze      (1000) grze      (1000)    10539 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/blocks/base_blocks.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     8757 2023-08-04 21:37:50.000000 wagtail-cjkcms-23.8.3/cjkcms/blocks/content_blocks.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     9537 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/blocks/html_blocks.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     3337 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/blocks/layout_blocks.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      171 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/blocks/searchable_html_block.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.444493 wagtail-cjkcms-23.8.3/cjkcms/draftail/
+-rw-r--r--   0 grze      (1000) grze      (1000)      305 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/draftail/__init__.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     3157 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/draftail/draftail_extensions.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     5157 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/draftail/draftail_icons.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     3191 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/fields.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.444493 wagtail-cjkcms-23.8.3/cjkcms/finders/
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/finders/__init__.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     2459 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/finders/oembed.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      361 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/forms.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     1804 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/image_formats.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.424493 wagtail-cjkcms-23.8.3/cjkcms/management/
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.444493 wagtail-cjkcms-23.8.3/cjkcms/management/commands/
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/management/commands/__init__.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      453 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/management/commands/clear-embeds.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     2565 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/management/commands/import-csv.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      952 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/management/commands/init-collections.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     3560 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/management/commands/init-navbar.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     3820 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/management/commands/init-website.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.424493 wagtail-cjkcms-23.8.3/cjkcms/media/
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.444493 wagtail-cjkcms-23.8.3/cjkcms/media/images/
+-rw-r--r--   0 grze      (1000) grze      (1000)     1938 2023-08-04 21:41:03.000000 wagtail-cjkcms-23.8.3/cjkcms/media/images/test.original.png
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.444493 wagtail-cjkcms-23.8.3/cjkcms/media/original_images/
+-rw-r--r--   0 grze      (1000) grze      (1000)     2306 2023-08-04 21:41:03.000000 wagtail-cjkcms-23.8.3/cjkcms/media/original_images/test.png
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.454493 wagtail-cjkcms-23.8.3/cjkcms/migrations/
+-rw-r--r--   0 grze      (1000) grze      (1000)   216350 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/migrations/0001_initial.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      835 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/migrations/0002_alter_body_to_cjkcmsstreamfield.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      668 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/migrations/0003_alter_footer_content_alter_navbar_menu_items.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     1027 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/migrations/0004_layoutsettings_articles_date_format_and_more.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     1709 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/migrations/0005_layoutsettings_custom_font_and_more.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     2886 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/migrations/0006_analyticssettings_consent_modal_layout_and_more.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      594 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/migrations/0007_layoutsettings_bootstrap_icons.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     1334 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/migrations/0008_alter_layoutsettings_navbar_langselector.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      685 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/migrations/0009_navbar_language.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     3479 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/migrations/0010_filmstrip_filmpanel.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     1393 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/migrations/0011_cjkcmspage_related_classifier_term_and_more.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     1466 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/migrations/0012_remove_analyticssettings_ga_tracking_id_and_more.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      780 2023-08-04 20:23:14.000000 wagtail-cjkcms-23.8.3/cjkcms/migrations/0013_socialmediasettings_location.py
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/migrations/__init__.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.454493 wagtail-cjkcms-23.8.3/cjkcms/models/
+-rw-r--r--   0 grze      (1000) grze      (1000)      232 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/models/__init__.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      392 2023-08-04 11:19:34.000000 wagtail-cjkcms-23.8.3/cjkcms/models/admin_sidebar.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     2356 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/models/cms_models.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     6302 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/models/integration_models.py
+-rw-r--r--   0 grze      (1000) grze      (1000)    23813 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/models/page_models.py
+-rw-r--r--   0 grze      (1000) grze      (1000)    15371 2023-08-04 11:17:41.000000 wagtail-cjkcms-23.8.3/cjkcms/models/snippet_models.py
+-rw-r--r--   0 grze      (1000) grze      (1000)    19301 2023-08-04 20:16:16.000000 wagtail-cjkcms-23.8.3/cjkcms/models/wagtailsettings_models.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.424493 wagtail-cjkcms-23.8.3/cjkcms/project_template/
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.454493 wagtail-cjkcms-23.8.3/cjkcms/project_template/basic/
+-rw-r--r--   0 grze      (1000) grze      (1000)      722 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/basic/.editorconfig
+-rw-r--r--   0 grze      (1000) grze      (1000)      364 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/basic/.gitattributes
+-rw-r--r--   0 grze      (1000) grze      (1000)      275 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/basic/.gitignore
+-rw-r--r--   0 grze      (1000) grze      (1000)      792 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/basic/README.md
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.454493 wagtail-cjkcms-23.8.3/cjkcms/project_template/basic/home/
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/basic/home/__init__.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.454493 wagtail-cjkcms-23.8.3/cjkcms/project_template/basic/home/blocks/
+-rw-r--r--   0 grze      (1000) grze      (1000)      137 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/basic/home/blocks/__init__.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     2141 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/basic/home/blocks/blocks.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.454493 wagtail-cjkcms-23.8.3/cjkcms/project_template/basic/home/migrations/
+-rw-r--r--   0 grze      (1000) grze      (1000)     4982 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/basic/home/migrations/0001_initial.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     2047 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/basic/home/migrations/0002_create_homepage.py
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/basic/home/migrations/__init__.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.454493 wagtail-cjkcms-23.8.3/cjkcms/project_template/basic/home/models/
+-rw-r--r--   0 grze      (1000) grze      (1000)      295 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/basic/home/models/__init__.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     2819 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/basic/home/models/cms_models.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.424493 wagtail-cjkcms-23.8.3/cjkcms/project_template/basic/home/templates/
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.424493 wagtail-cjkcms-23.8.3/cjkcms/project_template/basic/home/templates/home/
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.454493 wagtail-cjkcms-23.8.3/cjkcms/project_template/basic/home/templates/home/blocks/
+-rw-r--r--   0 grze      (1000) grze      (1000)     2282 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/basic/home/templates/home/blocks/event_presentation.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      678 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/basic/manage.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.454493 wagtail-cjkcms-23.8.3/cjkcms/project_template/basic/project_name/
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/basic/project_name/__init__.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.454493 wagtail-cjkcms-23.8.3/cjkcms/project_template/basic/project_name/settings/
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/basic/project_name/settings/__init__.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     5312 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/basic/project_name/settings/base.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      324 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/basic/project_name/settings/dev.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      705 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/basic/project_name/settings/local.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     1595 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/basic/project_name/settings/production.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.424493 wagtail-cjkcms-23.8.3/cjkcms/project_template/basic/project_name/static/
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.454493 wagtail-cjkcms-23.8.3/cjkcms/project_template/basic/project_name/static/css/
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/basic/project_name/static/css/devsite.css
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.454493 wagtail-cjkcms-23.8.3/cjkcms/project_template/basic/project_name/static/js/
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/basic/project_name/static/js/devsite.js
+-rw-r--r--   0 grze      (1000) grze      (1000)      911 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/basic/project_name/urls.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      438 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/basic/project_name/wsgi.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      123 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/basic/requirements.txt
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.454493 wagtail-cjkcms-23.8.3/cjkcms/project_template/basic/search/
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/basic/search/__init__.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.424493 wagtail-cjkcms-23.8.3/cjkcms/project_template/basic/search/templates/
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.454493 wagtail-cjkcms-23.8.3/cjkcms/project_template/basic/search/templates/search/
+-rw-r--r--   0 grze      (1000) grze      (1000)     1097 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/basic/search/templates/search/search.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     1019 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/basic/search/views.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.464493 wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/
+-rw-r--r--   0 grze      (1000) grze      (1000)      245 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/.babelrc
+-rw-r--r--   0 grze      (1000) grze      (1000)      159 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/.browserslistrc
+-rw-r--r--   0 grze      (1000) grze      (1000)      722 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/.editorconfig
+-rw-r--r--   0 grze      (1000) grze      (1000)      277 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/.eslintrc
+-rw-r--r--   0 grze      (1000) grze      (1000)      364 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/.gitattributes
+-rw-r--r--   0 grze      (1000) grze      (1000)      270 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/.gitignore
+-rw-r--r--   0 grze      (1000) grze      (1000)       13 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/.nvmrc
+-rw-r--r--   0 grze      (1000) grze      (1000)      182 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/.stylelintrc.json
+-rw-r--r--   0 grze      (1000) grze      (1000)      792 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/README.md
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.464493 wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/frontend/
+-rw-r--r--   0 grze      (1000) grze      (1000)      131 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/frontend/.gitignore
+-rw-r--r--   0 grze      (1000) grze      (1000)      733 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/frontend/README.md
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.434493 wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/frontend/src/
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.464493 wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/frontend/src/application/
+-rw-r--r--   0 grze      (1000) grze      (1000)      574 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/frontend/src/application/app.js
+-rw-r--r--   0 grze      (1000) grze      (1000)      226 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/frontend/src/application/app2.js
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.464493 wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/frontend/src/components/
+-rw-r--r--   0 grze      (1000) grze      (1000)       41 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/frontend/src/components/sidebar.js
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.464493 wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/frontend/src/styles/
+-rw-r--r--   0 grze      (1000) grze      (1000)      380 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/frontend/src/styles/index.scss
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.464493 wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/frontend/vendors/
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/frontend/vendors/.gitkeep
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.464493 wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/frontend/vendors/images/
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/frontend/vendors/images/.gitkeep
+-rw-r--r--   0 grze      (1000) grze      (1000)   273404 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/frontend/vendors/images/sample.jpg
+-rw-r--r--   0 grze      (1000) grze      (1000)   238213 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/frontend/vendors/images/webpack.png
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.464493 wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/frontend/webpack/
+-rw-r--r--   0 grze      (1000) grze      (1000)     1473 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/frontend/webpack/webpack.common.js
+-rw-r--r--   0 grze      (1000) grze      (1000)     1716 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/frontend/webpack/webpack.config.dev.js
+-rw-r--r--   0 grze      (1000) grze      (1000)      986 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/frontend/webpack/webpack.config.prod.js
+-rw-r--r--   0 grze      (1000) grze      (1000)     1485 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/frontend/webpack/webpack.config.watch.js
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.464493 wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/home/
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/home/__init__.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.464493 wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/home/blocks/
+-rw-r--r--   0 grze      (1000) grze      (1000)      137 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/home/blocks/__init__.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     2141 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/home/blocks/blocks.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.474493 wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/home/migrations/
+-rw-r--r--   0 grze      (1000) grze      (1000)     4982 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/home/migrations/0001_initial.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     2047 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/home/migrations/0002_create_homepage.py
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/home/migrations/__init__.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.474493 wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/home/models/
+-rw-r--r--   0 grze      (1000) grze      (1000)      295 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/home/models/__init__.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     2819 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/home/models/cms_models.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.434493 wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/home/templates/
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.434493 wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/home/templates/home/
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.474493 wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/home/templates/home/blocks/
+-rw-r--r--   0 grze      (1000) grze      (1000)     2282 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/home/templates/home/blocks/event_presentation.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      678 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/manage.py
+-rw-r--r--   0 grze      (1000) grze      (1000)   683340 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/package-lock.json
+-rw-r--r--   0 grze      (1000) grze      (1000)     1741 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/package.json
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.474493 wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/project_name/
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/project_name/__init__.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.474493 wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/project_name/settings/
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/project_name/settings/__init__.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     5312 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/project_name/settings/base.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      324 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/project_name/settings/dev.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      705 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/project_name/settings/local.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     1595 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/project_name/settings/production.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.434493 wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/project_name/static/
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.474493 wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/project_name/static/css/
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/project_name/static/css/devsite.css
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.474493 wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/project_name/static/js/
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/project_name/static/js/devsite.js
+-rw-r--r--   0 grze      (1000) grze      (1000)      911 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/project_name/urls.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      438 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/project_name/wsgi.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      123 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/requirements.txt
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.474493 wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/search/
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/search/__init__.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.434493 wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/search/templates/
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.474493 wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/search/templates/search/
+-rw-r--r--   0 grze      (1000) grze      (1000)     1097 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/search/templates/search/search.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     1019 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/search/views.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      125 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/search_urls.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     9799 2023-08-04 20:22:09.000000 wagtail-cjkcms-23.8.3/cjkcms/settings.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.434493 wagtail-cjkcms-23.8.3/cjkcms/static/
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.434493 wagtail-cjkcms-23.8.3/cjkcms/static/cjkcms/
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.474493 wagtail-cjkcms-23.8.3/cjkcms/static/cjkcms/bi/
+-rw-r--r--   0 grze      (1000) grze      (1000)    93729 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/static/cjkcms/bi/bootstrap-icons.css
+-rw-r--r--   0 grze      (1000) grze      (1000)    49971 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/static/cjkcms/bi/bootstrap-icons.json
+-rw-r--r--   0 grze      (1000) grze      (1000)    55169 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/static/cjkcms/bi/bootstrap-icons.scss
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.474493 wagtail-cjkcms-23.8.3/cjkcms/static/cjkcms/bi/fonts/
+-rw-r--r--   0 grze      (1000) grze      (1000)   164360 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/static/cjkcms/bi/fonts/bootstrap-icons.woff
+-rw-r--r--   0 grze      (1000) grze      (1000)   121340 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/static/cjkcms/bi/fonts/bootstrap-icons.woff2
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.474493 wagtail-cjkcms-23.8.3/cjkcms/static/cjkcms/css/
+-rw-r--r--   0 grze      (1000) grze      (1000)      846 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/static/cjkcms/css/cjkcms-admin.css
+-rw-r--r--   0 grze      (1000) grze      (1000)     1104 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/static/cjkcms/css/cjkcms-editor.css
+-rw-r--r--   0 grze      (1000) grze      (1000)     4614 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/static/cjkcms/css/cjkcms-front.css
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.434493 wagtail-cjkcms-23.8.3/cjkcms/static/cjkcms/images/
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.474493 wagtail-cjkcms-23.8.3/cjkcms/static/cjkcms/images/avatars/
+-rw-r--r--   0 grze      (1000) grze      (1000)      535 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/static/cjkcms/images/avatars/default.png
+-rw-r--r--   0 grze      (1000) grze      (1000)      384 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/static/cjkcms/images/avatars/default.svg
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.474493 wagtail-cjkcms-23.8.3/cjkcms/static/cjkcms/images/icons/
+-rw-r--r--   0 grze      (1000) grze      (1000)      705 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/static/cjkcms/images/icons/quote.svg
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.474493 wagtail-cjkcms-23.8.3/cjkcms/static/cjkcms/images/logos/
+-rw-r--r--   0 grze      (1000) grze      (1000)     4166 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/static/cjkcms/images/logos/cms-logo-long.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)     4218 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/static/cjkcms/images/logos/cms-logo-square.svg
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.474493 wagtail-cjkcms-23.8.3/cjkcms/static/cjkcms/images/patterns/
+-rw-r--r--   0 grze      (1000) grze      (1000)    47935 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/static/cjkcms/images/patterns/pattern1.jpg
+-rw-r--r--   0 grze      (1000) grze      (1000)    31707 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/static/cjkcms/images/patterns/pattern2.jpg
+-rw-r--r--   0 grze      (1000) grze      (1000)    38190 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/static/cjkcms/images/patterns/pattern3.jpg
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.474493 wagtail-cjkcms-23.8.3/cjkcms/static/cjkcms/js/
+-rw-r--r--   0 grze      (1000) grze      (1000)      444 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/static/cjkcms/js/cjkcms-editor.js
+-rw-r--r--   0 grze      (1000) grze      (1000)     5565 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/static/cjkcms/js/cjkcms-front.js
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.474493 wagtail-cjkcms-23.8.3/cjkcms/static/cookieconsent/
+-rw-r--r--   0 grze      (1000) grze      (1000)    18803 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/static/cookieconsent/cookieconsent.css
+-rw-r--r--   0 grze      (1000) grze      (1000)    18743 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/static/cookieconsent/cookieconsent.js
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.484493 wagtail-cjkcms-23.8.3/cjkcms/templates/
+-rw-r--r--   0 grze      (1000) grze      (1000)     4176 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/404.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     4802 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/500.html
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.484493 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.494493 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/
+-rw-r--r--   0 grze      (1000) grze      (1000)     1443 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/accordion_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      974 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/article_block_card.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     1132 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/article_masonry_card.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      188 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/base_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     2634 2023-08-04 20:24:22.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/base_link_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      740 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/button_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      746 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/card_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      856 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/card_blurb.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      786 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/card_foot.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      730 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/card_head.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      771 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/card_head_foot.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      990 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/card_horizontal.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     1104 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/card_horizontal2.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      786 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/card_img.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     2618 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/card_landing1.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     2758 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/card_landing2.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      678 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/cardgrid_columns.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      450 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/cardgrid_deck.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      277 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/cardgrid_group.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      276 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/cardgrid_zero.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     2698 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/carousel_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      406 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/column_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      137 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/document_link_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      920 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/download_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      103 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/embed_video_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)       95 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/external_link_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     1484 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/film_strip_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      424 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/grid_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      200 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/h1_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      200 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/h2_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      200 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/h3_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      790 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/hero_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      275 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/image_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     1400 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/image_gallery_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      627 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/image_link_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     1020 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/modal_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      164 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/page_link_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      787 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/pagelist_article_card_columns.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      642 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/pagelist_article_card_deck.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      361 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/pagelist_article_card_group.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      956 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/pagelist_article_media.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      858 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/pagelist_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      610 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/pagelist_list_group.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     1224 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/pagelist_toc_nextprev.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      200 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/pagepreview_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      793 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/pagepreview_card.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      244 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/pricelist_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      513 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/pricelistitem_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      353 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/quote_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      852 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/quote_block_leftbar.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      998 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/quote_block_start_end_quote.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      216 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/reusable_content_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)       91 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/rich_text_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     1095 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/table_block.html
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.494493 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/cookieconsent/
+-rw-r--r--   0 grze      (1000) grze      (1000)     3672 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/cookieconsent/languages.html
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.494493 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/formfields/
+-rw-r--r--   0 grze      (1000) grze      (1000)      267 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/formfields/date.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      416 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/formfields/datetime.html
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.494493 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/formfields/mailchimp/
+-rw-r--r--   0 grze      (1000) grze      (1000)     9267 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/formfields/mailchimp/_2vanilla_subscriber_integration_js.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     6469 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/formfields/mailchimp/subscriber_integration_js.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      793 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/formfields/mailchimp/subscriber_integration_widget.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      264 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/formfields/time.html
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.494493 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/icons/
+-rw-r--r--   0 grze      (1000) grze      (1000)      465 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/icons/align-left.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      573 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/icons/check-square-o.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      277 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/icons/columns.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      359 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/icons/desktop.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      571 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/icons/font.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      292 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/icons/google.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      813 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/icons/hand-pointer-o.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      666 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/icons/hashtag.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      840 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/icons/header.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      835 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/icons/list-alt.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      459 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/icons/map.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      448 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/icons/newspaper-o.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      721 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/icons/puzzle-piece.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      635 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/icons/recycle.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      174 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/icons/stop.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      505 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/icons/th-large.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      762 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/icons/universal-access.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      548 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/icons/usd.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      225 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/icons/window-maximize.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      199 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/icons/window-minimize.svg
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.494493 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/includes/
+-rw-r--r--   0 grze      (1000) grze      (1000)      286 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/includes/cjkcms_banner.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      689 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/includes/classifier_dropdowns.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      579 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/includes/classifier_nav.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      286 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/includes/codered_banner.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      268 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/includes/form_honeypot.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     1061 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/includes/pagination.html
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.494493 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/includes/stream_forms/
+-rw-r--r--   0 grze      (1000) grze      (1000)      532 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/includes/stream_forms/render_field.html
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.494493 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/pages/
+-rw-r--r--   0 grze      (1000) grze      (1000)     2002 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/pages/article_index_page.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     2031 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/pages/article_page.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     1018 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/pages/article_page.search.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     9291 2023-08-04 21:16:07.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/pages/base.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      248 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/pages/form_page_landing.html
+-rw-r--r--   0 grze      (1000) grze      (1000)       50 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/pages/home_page.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      491 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/pages/page.mini.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     2610 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/pages/search.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      582 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/pages/search_result.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      594 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/pages/web_page.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      200 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/pages/web_page_notitle.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      122 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/robots.txt
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.494493 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/snippets/
+-rw-r--r--   0 grze      (1000) grze      (1000)     1943 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/snippets/bottom_corner_lang_selector.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      430 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/snippets/footer.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     2027 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/snippets/frontend_assets.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     1196 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/snippets/frontend_scripts.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     2934 2023-08-04 20:44:06.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/snippets/navbar.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      836 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/snippets/navbar_lang_selector.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      386 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/snippets/navbar_search.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      330 2023-08-04 21:22:38.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/snippets/social_media.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     2035 2023-08-05 15:11:46.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/snippets/social_media_icons.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      171 2023-08-04 21:23:34.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/snippets/social_media_nav_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      158 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/snippets/tracking_g3.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      832 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/snippets/tracking_g4.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      694 2023-08-02 09:54:30.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/snippets/tracking_matomo.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      230 2023-08-02 09:54:30.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/snippets/tracking_matomo_noscript.html
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.494493 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/widgets/
+-rw-r--r--   0 grze      (1000) grze      (1000)     1444 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/widgets/checkbox_classifiers.html
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.434493 wagtail-cjkcms-23.8.3/cjkcms/templates/wagtailadmin/
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.494493 wagtail-cjkcms-23.8.3/cjkcms/templates/wagtailadmin/block_forms/
+-rw-r--r--   0 grze      (1000) grze      (1000)      839 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/wagtailadmin/block_forms/base_block_settings_struct.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      550 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/wagtailadmin/block_forms/struct.html
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.494493 wagtail-cjkcms-23.8.3/cjkcms/templates/wagtailadmin/shared/
+-rw-r--r--   0 grze      (1000) grze      (1000)      885 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templates/wagtailadmin/shared/cr_main_nav_2fix.html
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.504493 wagtail-cjkcms-23.8.3/cjkcms/templatetags/
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templatetags/__init__.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      327 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templatetags/auth_extras.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     6845 2023-08-04 21:38:58.000000 wagtail-cjkcms-23.8.3/cjkcms/templatetags/cjkcms_tags.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     4962 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templatetags/friendly_loader.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     1127 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templatetags/gravatar.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     1224 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/templatetags/txtutils_tags.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.504493 wagtail-cjkcms-23.8.3/cjkcms/tests/
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/tests/__init__.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     4226 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/tests/test_articlepages.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     3506 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/tests/test_bin.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     2629 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/tests/test_gravatar.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     4760 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/tests/test_search_blocks.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     2665 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/tests/test_settings.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     3762 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/tests/test_templatetags.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     2673 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/tests/test_urls.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     1520 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/tests/test_webpage.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      506 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/urls.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      573 2023-07-16 21:02:27.000000 wagtail-cjkcms-23.8.3/cjkcms/utils.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     4488 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/views.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     6613 2023-08-04 11:20:28.000000 wagtail-cjkcms-23.8.3/cjkcms/wagtail_hooks.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     1531 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/cjkcms/widgets.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.504493 wagtail-cjkcms-23.8.3/docs/
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.504493 wagtail-cjkcms-23.8.3/docs/how-to/
+-rw-r--r--   0 grze      (1000) grze      (1000)     1481 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/docs/how-to/oembed_finder.md
+-rw-r--r--   0 grze      (1000) grze      (1000)      537 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/docs/index.md
+-rw-r--r--   0 grze      (1000) grze      (1000)     5520 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/docs/installation.md
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.504493 wagtail-cjkcms-23.8.3/docs/management_commands/
+-rw-r--r--   0 grze      (1000) grze      (1000)      318 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/docs/management_commands/clear-embeds.md
+-rw-r--r--   0 grze      (1000) grze      (1000)      193 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/docs/management_commands/index.md
+-rw-r--r--   0 grze      (1000) grze      (1000)      420 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/docs/management_commands/init-collections.md
+-rw-r--r--   0 grze      (1000) grze      (1000)      936 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/docs/quick-start.md
+-rw-r--r--   0 grze      (1000) grze      (1000)       13 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/docs/requirements.txt
+-rw-r--r--   0 grze      (1000) grze      (1000)     1220 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/docs/why-another-cms.md
+-rw-r--r--   0 grze      (1000) grze      (1000)     2154 2023-08-02 09:54:30.000000 wagtail-cjkcms-23.8.3/pyproject.toml
+-rw-r--r--   0 grze      (1000) grze      (1000)      230 2023-08-05 15:14:10.504493 wagtail-cjkcms-23.8.3/setup.cfg
+-rw-r--r--   0 grze      (1000) grze      (1000)       38 2023-07-16 20:02:40.000000 wagtail-cjkcms-23.8.3/setup.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-05 15:14:10.504493 wagtail-cjkcms-23.8.3/wagtail_cjkcms.egg-info/
+-rw-r--r--   0 grze      (1000) grze      (1000)     4857 2023-08-05 15:14:10.000000 wagtail-cjkcms-23.8.3/wagtail_cjkcms.egg-info/PKG-INFO
+-rw-r--r--   0 grze      (1000) grze      (1000)    14486 2023-08-05 15:14:10.000000 wagtail-cjkcms-23.8.3/wagtail_cjkcms.egg-info/SOURCES.txt
+-rw-r--r--   0 grze      (1000) grze      (1000)        1 2023-08-05 15:14:10.000000 wagtail-cjkcms-23.8.3/wagtail_cjkcms.egg-info/dependency_links.txt
+-rw-r--r--   0 grze      (1000) grze      (1000)       50 2023-08-05 15:14:10.000000 wagtail-cjkcms-23.8.3/wagtail_cjkcms.egg-info/entry_points.txt
+-rw-r--r--   0 grze      (1000) grze      (1000)      189 2023-08-05 15:14:10.000000 wagtail-cjkcms-23.8.3/wagtail_cjkcms.egg-info/requires.txt
+-rw-r--r--   0 grze      (1000) grze      (1000)        7 2023-08-05 15:14:10.000000 wagtail-cjkcms-23.8.3/wagtail_cjkcms.egg-info/top_level.txt
```

### Comparing `wagtail-cjkcms-23.8.2/CHANGELOG.md` & `wagtail-cjkcms-23.8.3/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -203,7 +203,10 @@
 
 # 23.8.1 (2023-08-02)
 - Break down matomo tracking code snippet into two, moving the "noscript" section to the bottom of html file
 - Add instructions for using pytest excluding the project_template folder
 
 # 23.8.2 (2023-08-05)
  - Removed previously under construction Navbar Social Media link item. Replaced with a location field added to SocialMediaSettings, with four locations: none, inside menu bar, float left, and float right. Requires loading font awesome icons in settings -> layout.
+
+# 23.8.3 (2023-08-06)
+ - Fixed error in social media template twitter link. Added target _blank to all social media links.
```

### Comparing `wagtail-cjkcms-23.8.2/LICENSE` & `wagtail-cjkcms-23.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/PKG-INFO` & `wagtail-cjkcms-23.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-cjkcms
-Version: 23.8.2
+Version: 23.8.3
 Summary: Wagtail Content Management System, installable as a Django app into any Wagtail 4.1.x/5.x site.
 Author-email: Grzegorz Krol <gk@cjk.pl>
 License: BSD-3-Clause
         
         Copyright (2022) Grzegorz Krol, Filip Wozniak
         All rights reserved.
```

### Comparing `wagtail-cjkcms-23.8.2/README.md` & `wagtail-cjkcms-23.8.3/README.md`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/api/mailchimp.py` & `wagtail-cjkcms-23.8.3/cjkcms/api/mailchimp.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/bin/cjkcms.py` & `wagtail-cjkcms-23.8.3/cjkcms/bin/cjkcms.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/blocks/__init__.py` & `wagtail-cjkcms-23.8.3/cjkcms/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/blocks/base_blocks.py` & `wagtail-cjkcms-23.8.3/cjkcms/blocks/base_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/blocks/content_blocks.py` & `wagtail-cjkcms-23.8.3/cjkcms/blocks/content_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/blocks/html_blocks.py` & `wagtail-cjkcms-23.8.3/cjkcms/blocks/html_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/blocks/layout_blocks.py` & `wagtail-cjkcms-23.8.3/cjkcms/blocks/layout_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/draftail/draftail_extensions.py` & `wagtail-cjkcms-23.8.3/cjkcms/draftail/draftail_extensions.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/draftail/draftail_icons.py` & `wagtail-cjkcms-23.8.3/cjkcms/draftail/draftail_icons.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/fields.py` & `wagtail-cjkcms-23.8.3/cjkcms/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/finders/oembed.py` & `wagtail-cjkcms-23.8.3/cjkcms/finders/oembed.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/image_formats.py` & `wagtail-cjkcms-23.8.3/cjkcms/image_formats.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/management/commands/import-csv.py` & `wagtail-cjkcms-23.8.3/cjkcms/management/commands/import-csv.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/management/commands/init-collections.py` & `wagtail-cjkcms-23.8.3/cjkcms/management/commands/init-collections.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/management/commands/init-navbar.py` & `wagtail-cjkcms-23.8.3/cjkcms/management/commands/init-navbar.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/management/commands/init-website.py` & `wagtail-cjkcms-23.8.3/cjkcms/management/commands/init-website.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/media/images/test.original.png` & `wagtail-cjkcms-23.8.3/cjkcms/media/images/test.original.png`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/media/original_images/test.png` & `wagtail-cjkcms-23.8.3/cjkcms/media/original_images/test.png`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/migrations/0001_initial.py` & `wagtail-cjkcms-23.8.3/cjkcms/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/migrations/0002_alter_body_to_cjkcmsstreamfield.py` & `wagtail-cjkcms-23.8.3/cjkcms/migrations/0002_alter_body_to_cjkcmsstreamfield.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/migrations/0003_alter_footer_content_alter_navbar_menu_items.py` & `wagtail-cjkcms-23.8.3/cjkcms/migrations/0003_alter_footer_content_alter_navbar_menu_items.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/migrations/0004_layoutsettings_articles_date_format_and_more.py` & `wagtail-cjkcms-23.8.3/cjkcms/migrations/0004_layoutsettings_articles_date_format_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/migrations/0005_layoutsettings_custom_font_and_more.py` & `wagtail-cjkcms-23.8.3/cjkcms/migrations/0005_layoutsettings_custom_font_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/migrations/0006_analyticssettings_consent_modal_layout_and_more.py` & `wagtail-cjkcms-23.8.3/cjkcms/migrations/0006_analyticssettings_consent_modal_layout_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/migrations/0007_layoutsettings_bootstrap_icons.py` & `wagtail-cjkcms-23.8.3/cjkcms/migrations/0007_layoutsettings_bootstrap_icons.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/migrations/0008_alter_layoutsettings_navbar_langselector.py` & `wagtail-cjkcms-23.8.3/cjkcms/migrations/0008_alter_layoutsettings_navbar_langselector.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/migrations/0009_navbar_language.py` & `wagtail-cjkcms-23.8.3/cjkcms/migrations/0009_navbar_language.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/migrations/0010_filmstrip_filmpanel.py` & `wagtail-cjkcms-23.8.3/cjkcms/migrations/0010_filmstrip_filmpanel.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/migrations/0011_cjkcmspage_related_classifier_term_and_more.py` & `wagtail-cjkcms-23.8.3/cjkcms/migrations/0011_cjkcmspage_related_classifier_term_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/migrations/0012_remove_analyticssettings_ga_tracking_id_and_more.py` & `wagtail-cjkcms-23.8.3/cjkcms/migrations/0012_remove_analyticssettings_ga_tracking_id_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/migrations/0013_socialmediasettings_location.py` & `wagtail-cjkcms-23.8.3/cjkcms/migrations/0013_socialmediasettings_location.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/models/cms_models.py` & `wagtail-cjkcms-23.8.3/cjkcms/models/cms_models.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/models/integration_models.py` & `wagtail-cjkcms-23.8.3/cjkcms/models/integration_models.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/models/page_models.py` & `wagtail-cjkcms-23.8.3/cjkcms/models/page_models.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/models/snippet_models.py` & `wagtail-cjkcms-23.8.3/cjkcms/models/snippet_models.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/models/wagtailsettings_models.py` & `wagtail-cjkcms-23.8.3/cjkcms/models/wagtailsettings_models.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/project_template/basic/.editorconfig` & `wagtail-cjkcms-23.8.3/cjkcms/project_template/basic/.editorconfig`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/project_template/basic/README.md` & `wagtail-cjkcms-23.8.3/cjkcms/project_template/basic/README.md`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/project_template/basic/home/blocks/blocks.py` & `wagtail-cjkcms-23.8.3/cjkcms/project_template/basic/home/blocks/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/project_template/basic/home/migrations/0001_initial.py` & `wagtail-cjkcms-23.8.3/cjkcms/project_template/basic/home/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/project_template/basic/home/migrations/0002_create_homepage.py` & `wagtail-cjkcms-23.8.3/cjkcms/project_template/basic/home/migrations/0002_create_homepage.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/project_template/basic/home/models/cms_models.py` & `wagtail-cjkcms-23.8.3/cjkcms/project_template/basic/home/models/cms_models.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/project_template/basic/home/templates/home/blocks/event_presentation.html` & `wagtail-cjkcms-23.8.3/cjkcms/project_template/basic/home/templates/home/blocks/event_presentation.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/project_template/basic/manage.py` & `wagtail-cjkcms-23.8.3/cjkcms/project_template/basic/manage.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/project_template/basic/project_name/settings/base.py` & `wagtail-cjkcms-23.8.3/cjkcms/project_template/basic/project_name/settings/base.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/project_template/basic/project_name/settings/local.py` & `wagtail-cjkcms-23.8.3/cjkcms/project_template/basic/project_name/settings/local.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/project_template/basic/project_name/settings/production.py` & `wagtail-cjkcms-23.8.3/cjkcms/project_template/basic/project_name/settings/production.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/project_template/basic/project_name/urls.py` & `wagtail-cjkcms-23.8.3/cjkcms/project_template/basic/project_name/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/project_template/basic/search/templates/search/search.html` & `wagtail-cjkcms-23.8.3/cjkcms/project_template/basic/search/templates/search/search.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/project_template/basic/search/views.py` & `wagtail-cjkcms-23.8.3/cjkcms/project_template/basic/search/views.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/.editorconfig` & `wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/.editorconfig`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/README.md` & `wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/README.md`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/frontend/README.md` & `wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/frontend/README.md`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/frontend/src/application/app.js` & `wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/frontend/src/application/app.js`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/frontend/vendors/images/sample.jpg` & `wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/frontend/vendors/images/sample.jpg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/frontend/vendors/images/webpack.png` & `wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/frontend/vendors/images/webpack.png`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/frontend/webpack/webpack.common.js` & `wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/frontend/webpack/webpack.common.js`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/frontend/webpack/webpack.config.dev.js` & `wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/frontend/webpack/webpack.config.dev.js`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/frontend/webpack/webpack.config.prod.js` & `wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/frontend/webpack/webpack.config.prod.js`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/frontend/webpack/webpack.config.watch.js` & `wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/frontend/webpack/webpack.config.watch.js`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/home/blocks/blocks.py` & `wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/home/blocks/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/home/migrations/0001_initial.py` & `wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/home/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/home/migrations/0002_create_homepage.py` & `wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/home/migrations/0002_create_homepage.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/home/models/cms_models.py` & `wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/home/models/cms_models.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/home/templates/home/blocks/event_presentation.html` & `wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/home/templates/home/blocks/event_presentation.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/manage.py` & `wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/manage.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/package-lock.json` & `wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/package-lock.json`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/package.json` & `wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/package.json`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/project_name/settings/base.py` & `wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/project_name/settings/base.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/project_name/settings/local.py` & `wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/project_name/settings/local.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/project_name/settings/production.py` & `wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/project_name/settings/production.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/project_name/urls.py` & `wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/project_name/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/search/templates/search/search.html` & `wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/search/templates/search/search.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/project_template/webpack/search/views.py` & `wagtail-cjkcms-23.8.3/cjkcms/project_template/webpack/search/views.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/settings.py` & `wagtail-cjkcms-23.8.3/cjkcms/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/static/cjkcms/bi/bootstrap-icons.css` & `wagtail-cjkcms-23.8.3/cjkcms/static/cjkcms/bi/bootstrap-icons.css`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/static/cjkcms/bi/bootstrap-icons.json` & `wagtail-cjkcms-23.8.3/cjkcms/static/cjkcms/bi/bootstrap-icons.json`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/static/cjkcms/bi/bootstrap-icons.scss` & `wagtail-cjkcms-23.8.3/cjkcms/static/cjkcms/bi/bootstrap-icons.scss`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/static/cjkcms/bi/fonts/bootstrap-icons.woff` & `wagtail-cjkcms-23.8.3/cjkcms/static/cjkcms/bi/fonts/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/static/cjkcms/bi/fonts/bootstrap-icons.woff2` & `wagtail-cjkcms-23.8.3/cjkcms/static/cjkcms/bi/fonts/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/static/cjkcms/css/cjkcms-admin.css` & `wagtail-cjkcms-23.8.3/cjkcms/static/cjkcms/css/cjkcms-admin.css`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/static/cjkcms/css/cjkcms-editor.css` & `wagtail-cjkcms-23.8.3/cjkcms/static/cjkcms/css/cjkcms-editor.css`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/static/cjkcms/css/cjkcms-front.css` & `wagtail-cjkcms-23.8.3/cjkcms/static/cjkcms/css/cjkcms-front.css`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/static/cjkcms/images/avatars/default.png` & `wagtail-cjkcms-23.8.3/cjkcms/static/cjkcms/images/avatars/default.png`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/static/cjkcms/images/icons/quote.svg` & `wagtail-cjkcms-23.8.3/cjkcms/static/cjkcms/images/icons/quote.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/static/cjkcms/images/logos/cms-logo-long.svg` & `wagtail-cjkcms-23.8.3/cjkcms/static/cjkcms/images/logos/cms-logo-long.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/static/cjkcms/images/logos/cms-logo-square.svg` & `wagtail-cjkcms-23.8.3/cjkcms/static/cjkcms/images/logos/cms-logo-square.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/static/cjkcms/images/patterns/pattern1.jpg` & `wagtail-cjkcms-23.8.3/cjkcms/static/cjkcms/images/patterns/pattern1.jpg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/static/cjkcms/images/patterns/pattern2.jpg` & `wagtail-cjkcms-23.8.3/cjkcms/static/cjkcms/images/patterns/pattern2.jpg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/static/cjkcms/images/patterns/pattern3.jpg` & `wagtail-cjkcms-23.8.3/cjkcms/static/cjkcms/images/patterns/pattern3.jpg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/static/cjkcms/js/cjkcms-front.js` & `wagtail-cjkcms-23.8.3/cjkcms/static/cjkcms/js/cjkcms-front.js`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/static/cookieconsent/cookieconsent.css` & `wagtail-cjkcms-23.8.3/cjkcms/static/cookieconsent/cookieconsent.css`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/static/cookieconsent/cookieconsent.js` & `wagtail-cjkcms-23.8.3/cjkcms/static/cookieconsent/cookieconsent.js`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templates/404.html` & `wagtail-cjkcms-23.8.3/cjkcms/templates/404.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templates/500.html` & `wagtail-cjkcms-23.8.3/cjkcms/templates/500.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/accordion_block.html` & `wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/accordion_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/article_block_card.html` & `wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/article_block_card.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/article_masonry_card.html` & `wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/article_masonry_card.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/base_link_block.html` & `wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/base_link_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/button_block.html` & `wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/button_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/card_block.html` & `wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/card_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/card_blurb.html` & `wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/card_blurb.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/card_foot.html` & `wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/card_foot.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/card_head.html` & `wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/card_head.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/card_head_foot.html` & `wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/card_head_foot.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/card_horizontal.html` & `wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/card_horizontal.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/card_horizontal2.html` & `wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/card_horizontal2.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/card_img.html` & `wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/card_img.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/card_landing1.html` & `wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/card_landing1.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/card_landing2.html` & `wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/card_landing2.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/cardgrid_columns.html` & `wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/cardgrid_columns.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/carousel_block.html` & `wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/carousel_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/download_block.html` & `wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/download_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/film_strip_block.html` & `wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/film_strip_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/hero_block.html` & `wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/hero_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/image_gallery_block.html` & `wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/image_gallery_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/image_link_block.html` & `wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/image_link_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/modal_block.html` & `wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/modal_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/pagelist_article_card_columns.html` & `wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/pagelist_article_card_columns.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/pagelist_article_card_deck.html` & `wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/pagelist_article_card_deck.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/pagelist_article_media.html` & `wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/pagelist_article_media.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/pagelist_block.html` & `wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/pagelist_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/pagelist_list_group.html` & `wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/pagelist_list_group.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/pagelist_toc_nextprev.html` & `wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/pagelist_toc_nextprev.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/pagepreview_card.html` & `wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/pagepreview_card.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/pricelistitem_block.html` & `wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/pricelistitem_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/quote_block_leftbar.html` & `wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/quote_block_leftbar.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/quote_block_start_end_quote.html` & `wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/quote_block_start_end_quote.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/blocks/table_block.html` & `wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/blocks/table_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/cookieconsent/languages.html` & `wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/cookieconsent/languages.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/formfields/mailchimp/_2vanilla_subscriber_integration_js.html` & `wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/formfields/mailchimp/_2vanilla_subscriber_integration_js.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/formfields/mailchimp/subscriber_integration_js.html` & `wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/formfields/mailchimp/subscriber_integration_js.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/formfields/mailchimp/subscriber_integration_widget.html` & `wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/formfields/mailchimp/subscriber_integration_widget.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/icons/check-square-o.svg` & `wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/icons/check-square-o.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/icons/font.svg` & `wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/icons/font.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/icons/hand-pointer-o.svg` & `wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/icons/hand-pointer-o.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/icons/hashtag.svg` & `wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/icons/hashtag.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/icons/header.svg` & `wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/icons/header.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/icons/list-alt.svg` & `wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/icons/list-alt.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/icons/puzzle-piece.svg` & `wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/icons/puzzle-piece.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/icons/recycle.svg` & `wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/icons/recycle.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/icons/universal-access.svg` & `wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/icons/universal-access.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/icons/usd.svg` & `wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/icons/usd.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/includes/classifier_dropdowns.html` & `wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/includes/classifier_dropdowns.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/includes/classifier_nav.html` & `wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/includes/classifier_nav.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/includes/pagination.html` & `wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/includes/pagination.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/includes/stream_forms/render_field.html` & `wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/includes/stream_forms/render_field.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/pages/article_index_page.html` & `wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/pages/article_index_page.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/pages/article_page.html` & `wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/pages/article_page.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/pages/article_page.search.html` & `wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/pages/article_page.search.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/pages/base.html` & `wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/pages/base.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/pages/search.html` & `wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/pages/search.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/pages/search_result.html` & `wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/pages/search_result.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/pages/web_page.html` & `wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/pages/web_page.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/snippets/bottom_corner_lang_selector.html` & `wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/snippets/bottom_corner_lang_selector.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/snippets/frontend_assets.html` & `wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/snippets/frontend_assets.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/snippets/frontend_scripts.html` & `wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/snippets/frontend_scripts.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/snippets/navbar.html` & `wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/snippets/navbar.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/snippets/navbar_lang_selector.html` & `wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/snippets/navbar_lang_selector.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/snippets/tracking_g4.html` & `wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/snippets/tracking_g4.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/snippets/tracking_matomo.html` & `wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/snippets/tracking_matomo.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templates/cjkcms/widgets/checkbox_classifiers.html` & `wagtail-cjkcms-23.8.3/cjkcms/templates/cjkcms/widgets/checkbox_classifiers.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templates/wagtailadmin/block_forms/base_block_settings_struct.html` & `wagtail-cjkcms-23.8.3/cjkcms/templates/wagtailadmin/block_forms/base_block_settings_struct.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templates/wagtailadmin/block_forms/struct.html` & `wagtail-cjkcms-23.8.3/cjkcms/templates/wagtailadmin/block_forms/struct.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templates/wagtailadmin/shared/cr_main_nav_2fix.html` & `wagtail-cjkcms-23.8.3/cjkcms/templates/wagtailadmin/shared/cr_main_nav_2fix.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templatetags/cjkcms_tags.py` & `wagtail-cjkcms-23.8.3/cjkcms/templatetags/cjkcms_tags.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templatetags/friendly_loader.py` & `wagtail-cjkcms-23.8.3/cjkcms/templatetags/friendly_loader.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templatetags/gravatar.py` & `wagtail-cjkcms-23.8.3/cjkcms/templatetags/gravatar.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/templatetags/txtutils_tags.py` & `wagtail-cjkcms-23.8.3/cjkcms/templatetags/txtutils_tags.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/tests/test_articlepages.py` & `wagtail-cjkcms-23.8.3/cjkcms/tests/test_articlepages.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/tests/test_bin.py` & `wagtail-cjkcms-23.8.3/cjkcms/tests/test_bin.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/tests/test_gravatar.py` & `wagtail-cjkcms-23.8.3/cjkcms/tests/test_gravatar.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/tests/test_search_blocks.py` & `wagtail-cjkcms-23.8.3/cjkcms/tests/test_search_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/tests/test_settings.py` & `wagtail-cjkcms-23.8.3/cjkcms/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/tests/test_templatetags.py` & `wagtail-cjkcms-23.8.3/cjkcms/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/tests/test_urls.py` & `wagtail-cjkcms-23.8.3/cjkcms/tests/test_urls.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/tests/test_webpage.py` & `wagtail-cjkcms-23.8.3/cjkcms/tests/test_webpage.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/utils.py` & `wagtail-cjkcms-23.8.3/cjkcms/utils.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/views.py` & `wagtail-cjkcms-23.8.3/cjkcms/views.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/wagtail_hooks.py` & `wagtail-cjkcms-23.8.3/cjkcms/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/cjkcms/widgets.py` & `wagtail-cjkcms-23.8.3/cjkcms/widgets.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/docs/how-to/oembed_finder.md` & `wagtail-cjkcms-23.8.3/docs/how-to/oembed_finder.md`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/docs/index.md` & `wagtail-cjkcms-23.8.3/docs/index.md`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/docs/installation.md` & `wagtail-cjkcms-23.8.3/docs/installation.md`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/docs/quick-start.md` & `wagtail-cjkcms-23.8.3/docs/quick-start.md`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/docs/why-another-cms.md` & `wagtail-cjkcms-23.8.3/docs/why-another-cms.md`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/pyproject.toml` & `wagtail-cjkcms-23.8.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.8.2/wagtail_cjkcms.egg-info/PKG-INFO` & `wagtail-cjkcms-23.8.3/wagtail_cjkcms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-cjkcms
-Version: 23.8.2
+Version: 23.8.3
 Summary: Wagtail Content Management System, installable as a Django app into any Wagtail 4.1.x/5.x site.
 Author-email: Grzegorz Krol <gk@cjk.pl>
 License: BSD-3-Clause
         
         Copyright (2022) Grzegorz Krol, Filip Wozniak
         All rights reserved.
```

### Comparing `wagtail-cjkcms-23.8.2/wagtail_cjkcms.egg-info/SOURCES.txt` & `wagtail-cjkcms-23.8.3/wagtail_cjkcms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

