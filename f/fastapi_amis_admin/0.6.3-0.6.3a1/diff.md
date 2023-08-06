# Comparing `tmp/fastapi_amis_admin-0.6.3.tar.gz` & `tmp/fastapi_amis_admin-0.6.3a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_amis_admin-0.6.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "fastapi_amis_admin-0.6.3a1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fastapi_amis_admin-0.6.3.tar` & `fastapi_amis_admin-0.6.3a1.tar`

### file list

```diff
@@ -1,178 +1,38 @@
--rw-r--r--   0        0        0      717 2023-08-05 10:02:59.365930 fastapi_amis_admin-0.6.3/.github/dependabot.yml
--rw-r--r--   0        0        0      781 2023-08-05 10:02:59.365930 fastapi_amis_admin-0.6.3/.github/workflows/build-docs.yml
--rw-r--r--   0        0        0     1450 2023-08-05 10:02:59.365930 fastapi_amis_admin-0.6.3/.github/workflows/pytest.yml
--rw-r--r--   0        0        0      978 2023-08-05 10:02:59.365930 fastapi_amis_admin-0.6.3/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     2121 2023-08-05 10:02:59.365930 fastapi_amis_admin-0.6.3/.gitignore
--rw-r--r--   0        0        0      266 2023-08-05 10:02:59.365930 fastapi_amis_admin-0.6.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11357 2023-08-05 10:02:59.365930 fastapi_amis_admin-0.6.3/LICENSE
--rw-r--r--   0        0        0    11455 2023-08-05 10:02:59.365930 fastapi_amis_admin-0.6.3/README.md
--rw-r--r--   0        0        0    11066 2023-08-05 10:02:59.365930 fastapi_amis_admin-0.6.3/README.zh.md
--rw-r--r--   0        0        0     1497 2023-08-05 10:02:59.365930 fastapi_amis_admin-0.6.3/demo/demo-form.py
--rw-r--r--   0        0        0     1167 2023-08-05 10:02:59.365930 fastapi_amis_admin-0.6.3/demo/demo-model.py
--rw-r--r--   0        0        0      408 2023-08-05 10:02:59.365930 fastapi_amis_admin-0.6.3/demo/demo-simple.py
--rw-r--r--   0        0        0       17 2023-08-05 10:02:59.365930 fastapi_amis_admin-0.6.3/docs/en/docs/CNAME
--rw-r--r--   0        0        0     2245 2023-08-05 10:02:59.365930 fastapi_amis_admin-0.6.3/docs/en/docs/about.md
--rw-r--r--   0        0        0     1702 2023-08-05 10:02:59.365930 fastapi_amis_admin-0.6.3/docs/en/docs/amis/types.md
--rw-r--r--   0        0        0     2631 2023-08-05 10:02:59.365930 fastapi_amis_admin-0.6.3/docs/en/docs/amis_admin/AdminApp.md
--rw-r--r--   0        0        0     1101 2023-08-05 10:02:59.365930 fastapi_amis_admin-0.6.3/docs/en/docs/amis_admin/AdminGroup.md
--rw-r--r--   0        0        0     1100 2023-08-05 10:02:59.365930 fastapi_amis_admin-0.6.3/docs/en/docs/amis_admin/AdminSite.md
--rw-r--r--   0        0        0     2780 2023-08-05 10:02:59.365930 fastapi_amis_admin-0.6.3/docs/en/docs/amis_admin/BaseAdmin.md
--rw-r--r--   0        0        0     1681 2023-08-05 10:02:59.365930 fastapi_amis_admin-0.6.3/docs/en/docs/amis_admin/FormAdmin.md
--rw-r--r--   0        0        0     1473 2023-08-05 10:02:59.365930 fastapi_amis_admin-0.6.3/docs/en/docs/amis_admin/ModelAction.md
--rw-r--r--   0        0        0     7882 2023-08-05 10:02:59.365930 fastapi_amis_admin-0.6.3/docs/en/docs/amis_admin/ModelAdmin.md
--rw-r--r--   0        0        0     1237 2023-08-05 10:02:59.365930 fastapi_amis_admin-0.6.3/docs/en/docs/amis_admin/PageAdmin.md
--rw-r--r--   0        0        0     1280 2023-08-05 10:02:59.365930 fastapi_amis_admin-0.6.3/docs/en/docs/amis_admin/PageSchemaAdmin.md
--rw-r--r--   0        0        0      353 2023-08-05 10:02:59.365930 fastapi_amis_admin-0.6.3/docs/en/docs/amis_admin/RouterAdmin.md
--rw-r--r--   0        0        0     1745 2023-08-05 10:02:59.365930 fastapi_amis_admin-0.6.3/docs/en/docs/amis_admin/Settings.md
--rw-r--r--   0        0        0      732 2023-08-05 10:02:59.365930 fastapi_amis_admin-0.6.3/docs/en/docs/amis_admin/TemplateAdmin.md
--rw-r--r--   0        0        0     3601 2023-08-05 10:02:59.365930 fastapi_amis_admin-0.6.3/docs/en/docs/crud/BaseCrud.md
--rw-r--r--   0        0        0      465 2023-08-05 10:02:59.365930 fastapi_amis_admin-0.6.3/docs/en/docs/crud/RouterMixin.md
--rw-r--r--   0        0        0     2618 2023-08-05 10:02:59.365930 fastapi_amis_admin-0.6.3/docs/en/docs/crud/SQLModelCrud.md
--rw-r--r--   0        0        0       94 2023-08-05 10:02:59.369931 fastapi_amis_admin-0.6.3/docs/en/docs/extended/SQLModel.md
--rw-r--r--   0        0        0      683 2023-08-05 10:02:59.369931 fastapi_amis_admin-0.6.3/docs/en/docs/extended/about.md
--rw-r--r--   0        0        0     1351 2023-08-05 10:02:59.369931 fastapi_amis_admin-0.6.3/docs/en/docs/extended/alembic.md
--rw-r--r--   0        0        0    11451 2023-08-05 10:02:59.369931 fastapi_amis_admin-0.6.3/docs/en/docs/index.md
--rw-r--r--   0        0        0       83 2023-08-05 10:02:59.369931 fastapi_amis_admin-0.6.3/docs/en/docs/js/chat.js
--rw-r--r--   0        0        0    19360 2023-08-05 10:02:59.369931 fastapi_amis_admin-0.6.3/docs/en/docs/js/sidecar-1.5.0.js
--rw-r--r--   0        0        0    29223 2023-08-05 10:02:59.369931 fastapi_amis_admin-0.6.3/docs/en/docs/static/Docs.png
--rw-r--r--   0        0        0    80404 2023-08-05 10:02:59.369931 fastapi_amis_admin-0.6.3/docs/en/docs/static/ModelAdmin.png
--rw-r--r--   0        0        0    21317 2023-08-05 10:02:59.369931 fastapi_amis_admin-0.6.3/docs/en/docs/static/logo.png
--rw-r--r--   0        0        0     3017 2023-08-05 10:02:59.369931 fastapi_amis_admin-0.6.3/docs/en/docs/tutorials/advanced/AdminApp.md
--rw-r--r--   0        0        0       21 2023-08-05 10:02:59.369931 fastapi_amis_admin-0.6.3/docs/en/docs/tutorials/advanced/_more.md
--rw-r--r--   0        0        0      580 2023-08-05 10:02:59.369931 fastapi_amis_admin-0.6.3/docs/en/docs/tutorials/advanced/cli.md
--rw-r--r--   0        0        0     2030 2023-08-05 10:02:59.369931 fastapi_amis_admin-0.6.3/docs/en/docs/tutorials/advanced/debug.md
--rw-r--r--   0        0        0     5125 2023-08-05 10:02:59.369931 fastapi_amis_admin-0.6.3/docs/en/docs/tutorials/advanced/permission.md
--rw-r--r--   0        0        0     2151 2023-08-05 10:02:59.369931 fastapi_amis_admin-0.6.3/docs/en/docs/tutorials/advanced/scheduler.md
--rw-r--r--   0        0        0     1944 2023-08-05 10:02:59.369931 fastapi_amis_admin-0.6.3/docs/en/docs/tutorials/advanced/structure.md
--rw-r--r--   0        0        0     7174 2023-08-05 10:02:59.369931 fastapi_amis_admin-0.6.3/docs/en/docs/tutorials/advanced/user-auth.md
--rw-r--r--   0        0        0     2464 2023-08-05 10:02:59.369931 fastapi_amis_admin-0.6.3/docs/en/docs/tutorials/basic/FormAdmin.md
--rw-r--r--   0        0        0     3974 2023-08-05 10:02:59.369931 fastapi_amis_admin-0.6.3/docs/en/docs/tutorials/basic/Inheritance.md
--rw-r--r--   0        0        0     5233 2023-08-05 10:02:59.369931 fastapi_amis_admin-0.6.3/docs/en/docs/tutorials/basic/ModelAction.md
--rw-r--r--   0        0        0     8076 2023-08-05 10:02:59.369931 fastapi_amis_admin-0.6.3/docs/en/docs/tutorials/basic/ModelAdmin.md
--rw-r--r--   0        0        0     5341 2023-08-05 10:02:59.369931 fastapi_amis_admin-0.6.3/docs/en/docs/tutorials/basic/PageAdmin.md
--rw-r--r--   0        0        0     3829 2023-08-05 10:02:59.369931 fastapi_amis_admin-0.6.3/docs/en/docs/tutorials/basic/Settings.md
--rw-r--r--   0        0        0     1088 2023-08-05 10:02:59.369931 fastapi_amis_admin-0.6.3/docs/en/docs/tutorials/basic/TemplateAdmin.md
--rw-r--r--   0        0        0       21 2023-08-05 10:02:59.369931 fastapi_amis_admin-0.6.3/docs/en/docs/tutorials/basic/_more.md
--rw-r--r--   0        0        0     1274 2023-08-05 10:02:59.369931 fastapi_amis_admin-0.6.3/docs/en/docs/tutorials/basic/i18n.md
--rw-r--r--   0        0        0     1840 2023-08-05 10:02:59.369931 fastapi_amis_admin-0.6.3/docs/en/docs/tutorials/quickstart.md
--rw-r--r--   0        0        0     2020 2023-08-05 10:02:59.369931 fastapi_amis_admin-0.6.3/docs/en/docs/utils/database.md
--rw-r--r--   0        0        0     3320 2023-08-05 10:02:59.369931 fastapi_amis_admin-0.6.3/docs/en/mkdocs.yml
--rw-r--r--   0        0        0       17 2023-08-05 10:02:59.369931 fastapi_amis_admin-0.6.3/docs/zh/docs/CNAME
--rw-r--r--   0        0        0     2075 2023-08-05 10:02:59.369931 fastapi_amis_admin-0.6.3/docs/zh/docs/about.md
--rw-r--r--   0        0        0     1596 2023-08-05 10:02:59.369931 fastapi_amis_admin-0.6.3/docs/zh/docs/amis/types.md
--rw-r--r--   0        0        0     2302 2023-08-05 10:02:59.369931 fastapi_amis_admin-0.6.3/docs/zh/docs/amis_admin/AdminApp.md
--rw-r--r--   0        0        0      960 2023-08-05 10:02:59.369931 fastapi_amis_admin-0.6.3/docs/zh/docs/amis_admin/AdminGroup.md
--rw-r--r--   0        0        0      932 2023-08-05 10:02:59.369931 fastapi_amis_admin-0.6.3/docs/zh/docs/amis_admin/AdminSite.md
--rw-r--r--   0        0        0     2669 2023-08-05 10:02:59.369931 fastapi_amis_admin-0.6.3/docs/zh/docs/amis_admin/BaseAdmin.md
--rw-r--r--   0        0        0     1572 2023-08-05 10:02:59.369931 fastapi_amis_admin-0.6.3/docs/zh/docs/amis_admin/FormAdmin.md
--rw-r--r--   0        0        0     1473 2023-08-05 10:02:59.369931 fastapi_amis_admin-0.6.3/docs/zh/docs/amis_admin/ModelAction.md
--rw-r--r--   0        0        0     7254 2023-08-05 10:02:59.369931 fastapi_amis_admin-0.6.3/docs/zh/docs/amis_admin/ModelAdmin.md
--rw-r--r--   0        0        0     1124 2023-08-05 10:02:59.369931 fastapi_amis_admin-0.6.3/docs/zh/docs/amis_admin/PageAdmin.md
--rw-r--r--   0        0        0     1163 2023-08-05 10:02:59.369931 fastapi_amis_admin-0.6.3/docs/zh/docs/amis_admin/PageSchemaAdmin.md
--rw-r--r--   0        0        0      316 2023-08-05 10:02:59.369931 fastapi_amis_admin-0.6.3/docs/zh/docs/amis_admin/RouterAdmin.md
--rw-r--r--   0        0        0     1534 2023-08-05 10:02:59.369931 fastapi_amis_admin-0.6.3/docs/zh/docs/amis_admin/Settings.md
--rw-r--r--   0        0        0      670 2023-08-05 10:02:59.369931 fastapi_amis_admin-0.6.3/docs/zh/docs/amis_admin/TemplateAdmin.md
--rw-r--r--   0        0        0     3328 2023-08-05 10:02:59.369931 fastapi_amis_admin-0.6.3/docs/zh/docs/crud/BaseCrud.md
--rw-r--r--   0        0        0      441 2023-08-05 10:02:59.369931 fastapi_amis_admin-0.6.3/docs/zh/docs/crud/RouterMixin.md
--rw-r--r--   0        0        0     2354 2023-08-05 10:02:59.369931 fastapi_amis_admin-0.6.3/docs/zh/docs/crud/SQLModelCrud.md
--rw-r--r--   0        0        0       76 2023-08-05 10:02:59.369931 fastapi_amis_admin-0.6.3/docs/zh/docs/extended/SQLModel.md
--rw-r--r--   0        0        0      610 2023-08-05 10:02:59.369931 fastapi_amis_admin-0.6.3/docs/zh/docs/extended/about.md
--rw-r--r--   0        0        0     1210 2023-08-05 10:02:59.369931 fastapi_amis_admin-0.6.3/docs/zh/docs/extended/alembic.md
--rw-r--r--   0        0        0    11065 2023-08-05 10:02:59.369931 fastapi_amis_admin-0.6.3/docs/zh/docs/index.md
--rw-r--r--   0        0        0       83 2023-08-05 10:02:59.369931 fastapi_amis_admin-0.6.3/docs/zh/docs/js/chat.js
--rw-r--r--   0        0        0    19360 2023-08-05 10:02:59.369931 fastapi_amis_admin-0.6.3/docs/zh/docs/js/sidecar-1.5.0.js
--rw-r--r--   0        0        0    29223 2023-08-05 10:02:59.369931 fastapi_amis_admin-0.6.3/docs/zh/docs/static/Docs.png
--rw-r--r--   0        0        0    80404 2023-08-05 10:02:59.369931 fastapi_amis_admin-0.6.3/docs/zh/docs/static/ModelAdmin.png
--rw-r--r--   0        0        0    21317 2023-08-05 10:02:59.373931 fastapi_amis_admin-0.6.3/docs/zh/docs/static/logo.png
--rw-r--r--   0        0        0     2660 2023-08-05 10:02:59.373931 fastapi_amis_admin-0.6.3/docs/zh/docs/tutorials/advanced/AdminApp.md
--rw-r--r--   0        0        0       20 2023-08-05 10:02:59.373931 fastapi_amis_admin-0.6.3/docs/zh/docs/tutorials/advanced/_more.md
--rw-r--r--   0        0        0      548 2023-08-05 10:02:59.373931 fastapi_amis_admin-0.6.3/docs/zh/docs/tutorials/advanced/cli.md
--rw-r--r--   0        0        0     1805 2023-08-05 10:02:59.373931 fastapi_amis_admin-0.6.3/docs/zh/docs/tutorials/advanced/debug.md
--rw-r--r--   0        0        0     4648 2023-08-05 10:02:59.373931 fastapi_amis_admin-0.6.3/docs/zh/docs/tutorials/advanced/permission.md
--rw-r--r--   0        0        0     2004 2023-08-05 10:02:59.373931 fastapi_amis_admin-0.6.3/docs/zh/docs/tutorials/advanced/scheduler.md
--rw-r--r--   0        0        0     1930 2023-08-05 10:02:59.373931 fastapi_amis_admin-0.6.3/docs/zh/docs/tutorials/advanced/structure.md
--rw-r--r--   0        0        0     6520 2023-08-05 10:02:59.373931 fastapi_amis_admin-0.6.3/docs/zh/docs/tutorials/advanced/user-auth.md
--rw-r--r--   0        0        0     2194 2023-08-05 10:02:59.373931 fastapi_amis_admin-0.6.3/docs/zh/docs/tutorials/basic/FormAdmin.md
--rw-r--r--   0        0        0     3747 2023-08-05 10:02:59.373931 fastapi_amis_admin-0.6.3/docs/zh/docs/tutorials/basic/Inheritance.md
--rw-r--r--   0        0        0     5233 2023-08-05 10:02:59.373931 fastapi_amis_admin-0.6.3/docs/zh/docs/tutorials/basic/ModelAction.md
--rw-r--r--   0        0        0     9483 2023-08-05 10:02:59.373931 fastapi_amis_admin-0.6.3/docs/zh/docs/tutorials/basic/ModelAdmin.md
--rw-r--r--   0        0        0     4756 2023-08-05 10:02:59.373931 fastapi_amis_admin-0.6.3/docs/zh/docs/tutorials/basic/PageAdmin.md
--rw-r--r--   0        0        0     3325 2023-08-05 10:02:59.373931 fastapi_amis_admin-0.6.3/docs/zh/docs/tutorials/basic/Settings.md
--rw-r--r--   0        0        0     1004 2023-08-05 10:02:59.373931 fastapi_amis_admin-0.6.3/docs/zh/docs/tutorials/basic/TemplateAdmin.md
--rw-r--r--   0        0        0       20 2023-08-05 10:02:59.373931 fastapi_amis_admin-0.6.3/docs/zh/docs/tutorials/basic/_more.md
--rw-r--r--   0        0        0     1137 2023-08-05 10:02:59.373931 fastapi_amis_admin-0.6.3/docs/zh/docs/tutorials/basic/i18n.md
--rw-r--r--   0        0        0     1751 2023-08-05 10:02:59.373931 fastapi_amis_admin-0.6.3/docs/zh/docs/tutorials/quickstart.md
--rw-r--r--   0        0        0     1989 2023-08-05 10:02:59.373931 fastapi_amis_admin-0.6.3/docs/zh/docs/utils/database.md
--rw-r--r--   0        0        0     3326 2023-08-05 10:02:59.373931 fastapi_amis_admin-0.6.3/docs/zh/mkdocs.yml
--rw-r--r--   0        0        0      555 2023-08-05 10:02:59.373931 fastapi_amis_admin-0.6.3/fastapi_amis_admin/__init__.py
--rw-r--r--   0        0        0      411 2023-08-05 10:02:59.373931 fastapi_amis_admin-0.6.3/fastapi_amis_admin/admin/__init__.py
--rw-r--r--   0        0        0    58565 2023-08-05 10:02:59.373931 fastapi_amis_admin-0.6.3/fastapi_amis_admin/admin/admin.py
--rw-r--r--   0        0        0     3393 2023-08-05 10:02:59.373931 fastapi_amis_admin-0.6.3/fastapi_amis_admin/admin/handlers.py
--rw-r--r--   0        0        0    13844 2023-08-05 10:02:59.373931 fastapi_amis_admin-0.6.3/fastapi_amis_admin/admin/parser.py
--rw-r--r--   0        0        0     2383 2023-08-05 10:02:59.373931 fastapi_amis_admin-0.6.3/fastapi_amis_admin/admin/settings.py
--rw-r--r--   0        0        0     5225 2023-08-05 10:02:59.373931 fastapi_amis_admin-0.6.3/fastapi_amis_admin/admin/site.py
--rw-r--r--   0        0        0     4007 2023-08-05 10:02:59.373931 fastapi_amis_admin-0.6.3/fastapi_amis_admin/amis/README.md
--rw-r--r--   0        0        0      466 2023-08-05 10:02:59.373931 fastapi_amis_admin-0.6.3/fastapi_amis_admin/amis/__init__.py
--rw-r--r--   0        0        0   149371 2023-08-05 10:02:59.373931 fastapi_amis_admin-0.6.3/fastapi_amis_admin/amis/components.py
--rw-r--r--   0        0        0     2353 2023-08-05 10:02:59.373931 fastapi_amis_admin-0.6.3/fastapi_amis_admin/amis/constants.py
--rw-r--r--   0        0        0     6673 2023-08-05 10:02:59.373931 fastapi_amis_admin-0.6.3/fastapi_amis_admin/amis/templates/app.html
--rw-r--r--   0        0        0     1240 2023-08-05 10:02:59.373931 fastapi_amis_admin-0.6.3/fastapi_amis_admin/amis/templates/page.html
--rw-r--r--   0        0        0     4870 2023-08-05 10:02:59.373931 fastapi_amis_admin-0.6.3/fastapi_amis_admin/amis/types.py
--rw-r--r--   0        0        0      256 2023-08-05 10:02:59.373931 fastapi_amis_admin-0.6.3/fastapi_amis_admin/amis/utils.py
--rw-r--r--   0        0        0     1663 2023-08-05 10:02:59.373931 fastapi_amis_admin-0.6.3/fastapi_amis_admin/crud/README.md
--rw-r--r--   0        0        0      206 2023-08-05 10:02:59.373931 fastapi_amis_admin-0.6.3/fastapi_amis_admin/crud/__init__.py
--rw-r--r--   0        0        0    24452 2023-08-05 10:02:59.373931 fastapi_amis_admin-0.6.3/fastapi_amis_admin/crud/_sqlalchemy.py
--rw-r--r--   0        0        0      406 2023-08-05 10:02:59.373931 fastapi_amis_admin-0.6.3/fastapi_amis_admin/crud/_sqlmodel.py
--rw-r--r--   0        0        0     8038 2023-08-05 10:02:59.373931 fastapi_amis_admin-0.6.3/fastapi_amis_admin/crud/base.py
--rw-r--r--   0        0        0    14616 2023-08-05 10:02:59.373931 fastapi_amis_admin-0.6.3/fastapi_amis_admin/crud/parser.py
--rw-r--r--   0        0        0     1652 2023-08-05 10:02:59.373931 fastapi_amis_admin-0.6.3/fastapi_amis_admin/crud/schema.py
--rw-r--r--   0        0        0     1655 2023-08-05 10:02:59.373931 fastapi_amis_admin-0.6.3/fastapi_amis_admin/crud/utils.py
--rw-r--r--   0        0        0       58 2023-08-05 10:02:59.373931 fastapi_amis_admin-0.6.3/fastapi_amis_admin/globals/__init__.py
--rw-r--r--   0        0        0     2450 2023-08-05 10:02:59.373931 fastapi_amis_admin-0.6.3/fastapi_amis_admin/globals/db.py
--rw-r--r--   0        0        0      352 2023-08-05 10:02:59.373931 fastapi_amis_admin-0.6.3/fastapi_amis_admin/globals/deps.py
--rw-r--r--   0        0        0      780 2023-08-05 10:02:59.373931 fastapi_amis_admin-0.6.3/fastapi_amis_admin/globals/sites.py
--rw-r--r--   0        0        0     1719 2023-08-05 10:02:59.373931 fastapi_amis_admin-0.6.3/fastapi_amis_admin/locale/de_DE/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     2551 2023-08-05 10:02:59.373931 fastapi_amis_admin-0.6.3/fastapi_amis_admin/locale/de_DE/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1563 2023-08-05 10:02:59.373931 fastapi_amis_admin-0.6.3/fastapi_amis_admin/locale/zh_CN/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     2598 2023-08-05 10:02:59.373931 fastapi_amis_admin-0.6.3/fastapi_amis_admin/locale/zh_CN/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0      148 2023-08-05 10:02:59.373931 fastapi_amis_admin-0.6.3/fastapi_amis_admin/models/__init__.py
--rw-r--r--   0        0        0     2825 2023-08-05 10:02:59.373931 fastapi_amis_admin-0.6.3/fastapi_amis_admin/models/enums.py
--rw-r--r--   0        0        0     2880 2023-08-05 10:02:59.373931 fastapi_amis_admin-0.6.3/fastapi_amis_admin/models/fields.py
--rw-r--r--   0        0        0        0 2023-08-05 10:02:59.373931 fastapi_amis_admin-0.6.3/fastapi_amis_admin/utils/__init__.py
--rw-r--r--   0        0        0     2097 2023-08-05 10:02:59.373931 fastapi_amis_admin-0.6.3/fastapi_amis_admin/utils/functools.py
--rw-r--r--   0        0        0     8257 2023-08-05 10:02:59.373931 fastapi_amis_admin-0.6.3/fastapi_amis_admin/utils/pydantic.py
--rw-r--r--   0        0        0     1854 2023-08-05 10:02:59.377931 fastapi_amis_admin-0.6.3/fastapi_amis_admin/utils/translation.py
--rw-r--r--   0        0        0    92226 2023-08-05 10:02:59.377931 fastapi_amis_admin-0.6.3/pdm.lock
--rw-r--r--   0        0        0     2737 2023-08-05 10:02:59.377931 fastapi_amis_admin-0.6.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-08-05 10:02:59.377931 fastapi_amis_admin-0.6.3/tests/__init__.py
--rw-r--r--   0        0        0     2820 2023-08-05 10:02:59.377931 fastapi_amis_admin-0.6.3/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-08-05 10:02:59.377931 fastapi_amis_admin-0.6.3/tests/models/__init__.py
--rw-r--r--   0        0        0     2111 2023-08-05 10:02:59.377931 fastapi_amis_admin-0.6.3/tests/models/schemas.py
--rw-r--r--   0        0        0     3292 2023-08-05 10:02:59.377931 fastapi_amis_admin-0.6.3/tests/models/sqla.py
--rw-r--r--   0        0        0     3878 2023-08-05 10:02:59.377931 fastapi_amis_admin-0.6.3/tests/models/sqla2.py
--rw-r--r--   0        0        0     2958 2023-08-05 10:02:59.377931 fastapi_amis_admin-0.6.3/tests/models/sqlm.py
--rw-r--r--   0        0        0     1588 2023-08-05 10:02:59.377931 fastapi_amis_admin-0.6.3/tests/test_admin/test_AdminApp.py
--rw-r--r--   0        0        0     1978 2023-08-05 10:02:59.377931 fastapi_amis_admin-0.6.3/tests/test_admin/test_AdminGroup.py
--rw-r--r--   0        0        0     2527 2023-08-05 10:02:59.377931 fastapi_amis_admin-0.6.3/tests/test_admin/test_FormAdmin.py
--rw-r--r--   0        0        0     4772 2023-08-05 10:02:59.377931 fastapi_amis_admin-0.6.3/tests/test_admin/test_ModelAdmin.py
--rw-r--r--   0        0        0     4533 2023-08-05 10:02:59.377931 fastapi_amis_admin-0.6.3/tests/test_admin/test_admin.py
--rw-r--r--   0        0        0    11125 2023-08-05 10:02:59.377931 fastapi_amis_admin-0.6.3/tests/test_admin/test_parser.py
--rw-r--r--   0        0        0      885 2023-08-05 10:02:59.377931 fastapi_amis_admin-0.6.3/tests/test_admin/test_settings.py
--rw-r--r--   0        0        0        0 2023-08-05 10:02:59.377931 fastapi_amis_admin-0.6.3/tests/test_amis/__init__.py
--rw-r--r--   0        0        0      591 2023-08-05 10:02:59.377931 fastapi_amis_admin-0.6.3/tests/test_amis/test_amis.py
--rw-r--r--   0        0        0        0 2023-08-05 10:02:59.377931 fastapi_amis_admin-0.6.3/tests/test_crud/__init__.py
--rw-r--r--   0        0        0     2714 2023-08-05 10:02:59.377931 fastapi_amis_admin-0.6.3/tests/test_crud/conftest.py
--rw-r--r--   0        0        0     3427 2023-08-05 10:02:59.377931 fastapi_amis_admin-0.6.3/tests/test_crud/test_Mapper_Events.py
--rw-r--r--   0        0        0    13961 2023-08-05 10:02:59.377931 fastapi_amis_admin-0.6.3/tests/test_crud/test_SqlalchemyCrud_fields.py
--rw-r--r--   0        0        0     6227 2023-08-05 10:02:59.377931 fastapi_amis_admin-0.6.3/tests/test_crud/test_SqlalchemyCrud_routes_async.py
--rw-r--r--   0        0        0     5984 2023-08-05 10:02:59.377931 fastapi_amis_admin-0.6.3/tests/test_crud/test_SqlalchemyCrud_routes_sync.py
--rw-r--r--   0        0        0     8188 2023-08-05 10:02:59.377931 fastapi_amis_admin-0.6.3/tests/test_crud/test_SqlalchemyCrud_schemas.py
--rw-r--r--   0        0        0     1395 2023-08-05 10:02:59.377931 fastapi_amis_admin-0.6.3/tests/test_crud/test_SqlalchemySelector.py
--rw-r--r--   0        0        0      338 2023-08-05 10:02:59.377931 fastapi_amis_admin-0.6.3/tests/test_crud/test_fake_users.py
--rw-r--r--   0        0        0        0 2023-08-05 10:02:59.377931 fastapi_amis_admin-0.6.3/tests/test_globals/__init__.py
--rw-r--r--   0        0        0     1146 2023-08-05 10:02:59.377931 fastapi_amis_admin-0.6.3/tests/test_globals/test_db.py
--rw-r--r--   0        0        0      734 2023-08-05 10:02:59.377931 fastapi_amis_admin-0.6.3/tests/test_globals/test_sites.py
--rw-r--r--   0        0        0        0 2023-08-05 10:02:59.377931 fastapi_amis_admin-0.6.3/tests/test_utils/__init__.py
--rw-r--r--   0        0        0     5358 2023-08-05 10:02:59.377931 fastapi_amis_admin-0.6.3/tests/test_utils/test_pydantic.py
--rw-r--r--   0        0        0        0 2023-08-05 10:02:59.377931 fastapi_amis_admin-0.6.3/tests/todo.md
--rw-r--r--   0        0        0    13866 1970-01-01 00:00:00.000000 fastapi_amis_admin-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0    11789 2023-07-11 03:47:06.502739 fastapi_amis_admin-0.6.3a1/README.md
+-rw-r--r--   0        0        0      603 2023-08-04 07:53:08.550698 fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/__init__.py
+-rw-r--r--   0        0        0      431 2023-04-09 14:42:19.167596 fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/admin/__init__.py
+-rw-r--r--   0        0        0    60045 2023-08-04 07:48:22.236266 fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/admin/admin.py
+-rw-r--r--   0        0        0     3488 2023-07-07 10:00:42.574847 fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/admin/handlers.py
+-rw-r--r--   0        0        0    14171 2023-07-17 01:57:26.105611 fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/admin/parser.py
+-rw-r--r--   0        0        0     2446 2023-08-04 02:30:10.829405 fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/admin/settings.py
+-rw-r--r--   0        0        0     5515 2023-04-10 02:48:14.773714 fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/admin/site.py
+-rw-r--r--   0        0        0     4074 2022-10-24 02:06:23.827774 fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/amis/README.md
+-rw-r--r--   0        0        0      495 2023-04-10 02:29:06.105345 fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/amis/__init__.py
+-rw-r--r--   0        0        0   152222 2023-08-04 07:48:19.695786 fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/amis/components.py
+-rw-r--r--   0        0        0     2480 2023-04-18 02:58:25.165709 fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/amis/constants.py
+-rw-r--r--   0        0        0     6850 2023-02-16 12:50:32.161558 fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/amis/templates/app.html
+-rw-r--r--   0        0        0     1275 2023-02-17 13:46:40.329429 fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/amis/templates/page.html
+-rw-r--r--   0        0        0     4977 2023-07-11 06:11:29.701954 fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/amis/types.py
+-rw-r--r--   0        0        0      265 2022-10-24 02:06:23.834769 fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/amis/utils.py
+-rw-r--r--   0        0        0     1727 2022-10-24 02:06:23.836768 fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/crud/README.md
+-rw-r--r--   0        0        0      211 2023-07-08 02:15:45.947633 fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/crud/__init__.py
+-rw-r--r--   0        0        0    25066 2023-08-04 07:48:22.238245 fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/crud/_sqlalchemy.py
+-rw-r--r--   0        0        0      419 2023-07-07 10:02:58.918305 fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/crud/_sqlmodel.py
+-rw-r--r--   0        0        0     8260 2023-08-04 07:48:22.239246 fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/crud/base.py
+-rw-r--r--   0        0        0    14984 2023-08-04 07:48:19.698800 fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/crud/parser.py
+-rw-r--r--   0        0        0     1712 2023-08-04 07:48:22.240245 fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/crud/schema.py
+-rw-r--r--   0        0        0     1714 2023-07-11 15:07:52.748913 fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/crud/utils.py
+-rw-r--r--   0        0        0     2200 2023-03-03 00:56:42.771550 fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/locale/base.pot
+-rw-r--r--   0        0        0     1719 2023-03-03 01:02:59.621695 fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/locale/de_DE/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     2652 2023-03-03 00:58:11.049585 fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/locale/de_DE/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1563 2023-03-03 01:14:57.935868 fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/locale/zh_CN/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     2709 2023-03-03 01:14:57.936867 fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/locale/zh_CN/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0      156 2023-07-06 03:28:44.283974 fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/models/__init__.py
+-rw-r--r--   0        0        0     2911 2023-04-10 02:48:14.997586 fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/models/enums.py
+-rw-r--r--   0        0        0     2964 2023-07-06 03:28:22.246379 fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/models/fields.py
+-rw-r--r--   0        0        0        0 2021-12-03 06:56:03.696000 fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/utils/__init__.py
+-rw-r--r--   0        0        0     2145 2023-04-10 02:48:15.066546 fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/utils/functools.py
+-rw-r--r--   0        0        0     8494 2023-07-28 08:46:05.738068 fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/utils/pydantic.py
+-rw-r--r--   0        0        0     1905 2023-07-06 03:28:44.284973 fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/utils/translation.py
+-rw-r--r--   0        0        0     2820 2023-07-11 07:17:31.634284 fastapi_amis_admin-0.6.3a1/pyproject.toml
+-rw-r--r--   0        0        0    13828 1970-01-01 00:00:00.000000 fastapi_amis_admin-0.6.3a1/PKG-INFO
```

### Comparing `fastapi_amis_admin-0.6.3/README.md` & `fastapi_amis_admin-0.6.3a1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,57 @@
+Metadata-Version: 2.1
+Name: fastapi_amis_admin
+Version: 0.6.3a1
+Summary: FastAPI-Amis-Admin is a high-performance, efficient and easily extensible FastAPI admin framework. Inspired by Django-admin, and has as many powerful functions as Django-admin. 
+Keywords: fastapi,fastapi-admin,fastapi-amis-admin,django-admin,sqlmodel,sqlalchemy
+Author-email: Atomi <1456417373@qq.com>
+Maintainer-email: Atomi <1456417373@qq.com>
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Classifier: Framework :: FastAPI
+Classifier: Environment :: Web Environment
+Classifier: Topic :: System :: Systems Administration
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: fastapi>=0.100.0
+Requires-Dist: pydantic>1.7.4
+Requires-Dist: sqlalchemy>=1.4.0
+Requires-Dist: python-multipart>=0.0.5
+Requires-Dist: sqlalchemy-database>=0.1.0,<0.2.0
+Requires-Dist: aiofiles>=0.17.0
+Requires-Dist: fastapi-amis-admin-cli>=0.1.3,<0.2.0 ; extra == "cli"
+Requires-Dist: pre-commit>=2.20.0 ; extra == "dev"
+Requires-Dist: ruff>=0.0.261 ; extra == "dev"
+Requires-Dist: sqlmodel>=0.0.7 ; extra == "sqlmodel"
+Requires-Dist: uvicorn[standard] >=0.19.0,<1.0 ; extra == "standard"
+Requires-Dist: fastapi-amis-admin-cli>=0.1.3,<0.2.0 ; extra == "standard"
+Requires-Dist: uvicorn[standard] >=0.19.0,<1.0 ; extra == "test"
+Requires-Dist: fastapi-amis-admin-cli>=0.1.3,<0.2.0 ; extra == "test"
+Requires-Dist: pytest >=6.2.4 ; extra == "test"
+Requires-Dist: aiosqlite>=0.15.0 ; extra == "test"
+Requires-Dist: pytest-asyncio>=0.17 ; extra == "test"
+Requires-Dist: httpx>=0.24.0,<1.0 ; extra == "test"
+Requires-Dist: jinja2 >=2.11.2,<4.0.0 ; extra == "test"
+Requires-Dist: ujson>=4.0.1 ; extra == "test"
+Requires-Dist: requests>=2.28.1 ; extra == "test"
+Requires-Dist: sqlmodel>=0.0.7 ; extra == "test"
+Project-URL: Documentation, http://docs.amis.work/
+Project-URL: Source, https://github.com/amisadmin/fastapi_amis_admin
+Provides-Extra: cli
+Provides-Extra: dev
+Provides-Extra: sqlmodel
+Provides-Extra: standard
+Provides-Extra: test
+
 [简体中文](https://github.com/amisadmin/fastapi_amis_admin/blob/master/README.zh.md)
 | [English](https://github.com/amisadmin/fastapi_amis_admin)
 
 # Introduction
 
 <h2 align="center">
   FastAPI-Amis-Admin
@@ -328,7 +378,8 @@
 - [`FastAPI-User-Auth-Demo`](https://github.com/amisadmin/fastapi_user_auth_demo): An example `FastAPI-User-Auth` application.
 
 ## License
 
 - According to the `Apache2.0` protocol, `fastapi-amis-admin` is free and open source. It can be used for commercial for
   free, but please clearly display copyright information about `FastAPI-Amis-Admin` on the display interface.
 
+
```

### Comparing `fastapi_amis_admin-0.6.3/README.zh.md` & `fastapi_amis_admin-0.6.3a1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,692 +1,737 @@
 00000000: 5be7 ae80 e4bd 93e4 b8ad e696 875d 2868  [............](h
 00000010: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
 00000020: 6d2f 616d 6973 6164 6d69 6e2f 6661 7374  m/amisadmin/fast
 00000030: 6170 695f 616d 6973 5f61 646d 696e 2f62  api_amis_admin/b
 00000040: 6c6f 622f 6d61 7374 6572 2f52 4541 444d  lob/master/READM
-00000050: 452e 7a68 2e6d 6429 0a7c 205b 456e 676c  E.zh.md).| [Engl
-00000060: 6973 685d 2868 7474 7073 3a2f 2f67 6974  ish](https://git
-00000070: 6875 622e 636f 6d2f 616d 6973 6164 6d69  hub.com/amisadmi
-00000080: 6e2f 6661 7374 6170 695f 616d 6973 5f61  n/fastapi_amis_a
-00000090: 646d 696e 290a 0a23 20e9 a1b9 e79b aee4  dmin)..# .......
-000000a0: bb8b e7bb 8d0a 0a3c 6832 2061 6c69 676e  .......<h2 align
-000000b0: 3d22 6365 6e74 6572 223e 0a20 2046 6173  ="center">.  Fas
-000000c0: 7441 5049 2d41 6d69 732d 4164 6d69 6e0a  tAPI-Amis-Admin.
-000000d0: 3c2f 6832 3e0a 3c70 2061 6c69 676e 3d22  </h2>.<p align="
-000000e0: 6365 6e74 6572 223e 0a20 2020 203c 656d  center">.    <em
-000000f0: 3e66 6173 7461 7069 2d61 6d69 732d 6164  >fastapi-amis-ad
-00000100: 6d69 6ee6 98af e4b8 80e4 b8aa e68b a5e6  min.............
-00000110: 9c89 e9ab 98e6 80a7 e883 bd2c e9ab 98e6  ...........,....
-00000120: 9588 e78e 872c e698 93e6 8b93 e5b1 95e7  .....,..........
-00000130: 9a84 6661 7374 6170 69e7 aea1 e790 86e5  ..fastapi.......
-00000140: 908e e58f b0e6 a186 e69e b62e 3c2f 656d  ............</em
-00000150: 3e3c 6272 2f3e 0a20 2020 203c 656d 3ee5  ><br/>.    <em>.
-00000160: 90af e58f 91e8 87aa 446a 616e 676f 2d41  ........Django-A
-00000170: 646d 696e 2ce5 b9b6 e4b8 94e6 8ba5 e69c  dmin,...........
-00000180: 89e4 b88d e980 8ae8 89b2 e4ba 8e44 6a61  .............Dja
-00000190: 6e67 6f2d 4164 6d69 6ee7 9a84 e5bc bae5  ngo-Admin.......
-000001a0: a4a7 e58a 9fe8 83bd 2e3c 2f65 6d3e 0a3c  .........</em>.<
-000001b0: 2f70 3e0a 3c70 2061 6c69 676e 3d22 6365  /p>.<p align="ce
-000001c0: 6e74 6572 223e 0a20 2020 203c 6120 6872  nter">.    <a hr
-000001d0: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
-000001e0: 7562 2e63 6f6d 2f61 6d69 7361 646d 696e  ub.com/amisadmin
-000001f0: 2f66 6173 7461 7069 5f61 6d69 735f 6164  /fastapi_amis_ad
-00000200: 6d69 6e2f 6163 7469 6f6e 732f 776f 726b  min/actions/work
-00000210: 666c 6f77 732f 7079 7465 7374 2e79 6d6c  flows/pytest.yml
-00000220: 2220 7461 7267 6574 3d22 5f62 6c61 6e6b  " target="_blank
-00000230: 223e 0a20 2020 2020 2020 203c 696d 6720  ">.        <img 
-00000240: 7372 633d 2268 7474 7073 3a2f 2f67 6974  src="https://git
-00000250: 6875 622e 636f 6d2f 616d 6973 6164 6d69  hub.com/amisadmi
-00000260: 6e2f 6661 7374 6170 695f 616d 6973 5f61  n/fastapi_amis_a
-00000270: 646d 696e 2f61 6374 696f 6e73 2f77 6f72  dmin/actions/wor
-00000280: 6b66 6c6f 7773 2f70 7974 6573 742e 796d  kflows/pytest.ym
-00000290: 6c2f 6261 6467 652e 7376 6722 2061 6c74  l/badge.svg" alt
-000002a0: 3d22 5079 7465 7374 223e 0a20 2020 203c  ="Pytest">.    <
-000002b0: 2f61 3e0a 2020 2020 3c61 2068 7265 663d  /a>.    <a href=
-000002c0: 2268 7474 7073 3a2f 2f70 7970 692e 6f72  "https://pypi.or
-000002d0: 672f 7072 6f6a 6563 742f 6661 7374 6170  g/project/fastap
-000002e0: 695f 616d 6973 5f61 646d 696e 2220 7461  i_amis_admin" ta
-000002f0: 7267 6574 3d22 5f62 6c61 6e6b 223e 0a20  rget="_blank">. 
-00000300: 2020 2020 2020 203c 696d 6720 7372 633d         <img src=
-00000310: 2268 7474 7073 3a2f 2f62 6164 6765 6e2e  "https://badgen.
-00000320: 6e65 742f 7079 7069 2f76 2f66 6173 7461  net/pypi/v/fasta
-00000330: 7069 2d61 6d69 732d 6164 6d69 6e3f 636f  pi-amis-admin?co
-00000340: 6c6f 723d 626c 7565 2220 616c 743d 2250  lor=blue" alt="P
-00000350: 6163 6b61 6765 2076 6572 7369 6f6e 223e  ackage version">
-00000360: 0a20 2020 203c 2f61 3e0a 2020 2020 3c61  .    </a>.    <a
-00000370: 2068 7265 663d 2268 7474 7073 3a2f 2f70   href="https://p
-00000380: 6570 792e 7465 6368 2f70 726f 6a65 6374  epy.tech/project
-00000390: 2f66 6173 7461 7069 2d61 6d69 732d 6164  /fastapi-amis-ad
-000003a0: 6d69 6e22 2074 6172 6765 743d 225f 626c  min" target="_bl
-000003b0: 616e 6b22 3e0a 2020 2020 2020 2020 3c69  ank">.        <i
-000003c0: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
-000003d0: 7065 7079 2e74 6563 682f 6261 6467 652f  pepy.tech/badge/
-000003e0: 6661 7374 6170 692d 616d 6973 2d61 646d  fastapi-amis-adm
-000003f0: 696e 2220 616c 743d 2244 6f77 6e6c 6f61  in" alt="Downloa
-00000400: 6473 223e 0a20 2020 203c 2f61 3e0a 2020  ds">.    </a>.  
-00000410: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
-00000420: 3a2f 2f67 6974 7465 722e 696d 2f61 6d69  ://gitter.im/ami
-00000430: 7361 646d 696e 2f66 6173 7461 7069 2d61  sadmin/fastapi-a
-00000440: 6d69 732d 6164 6d69 6e22 3e0a 2020 2020  mis-admin">.    
-00000450: 2020 2020 3c69 6d67 2073 7263 3d22 6874      <img src="ht
-00000460: 7470 733a 2f2f 6261 6467 6573 2e67 6974  tps://badges.git
-00000470: 7465 722e 696d 2f61 6d69 7361 646d 696e  ter.im/amisadmin
-00000480: 2f66 6173 7461 7069 2d61 6d69 732d 6164  /fastapi-amis-ad
-00000490: 6d69 6e2e 7376 6722 2061 6c74 3d22 4368  min.svg" alt="Ch
-000004a0: 6174 206f 6e20 4769 7474 6572 222f 3e0a  at on Gitter"/>.
-000004b0: 2020 2020 3c2f 613e 0a20 2020 203c 6120      </a>.    <a 
-000004c0: 6872 6566 3d22 6874 7470 733a 2f2f 6a71  href="https://jq
-000004d0: 2e71 712e 636f 6d2f 3f5f 7776 3d31 3032  .qq.com/?_wv=102
-000004e0: 3726 6b3d 5534 4476 3678 3857 2220 7461  7&k=U4Dv6x8W" ta
-000004f0: 7267 6574 3d22 5f62 6c61 6e6b 223e 0a20  rget="_blank">. 
-00000500: 2020 2020 2020 203c 696d 6720 7372 633d         <img src=
-00000510: 2268 7474 7073 3a2f 2f62 6164 6765 6e2e  "https://badgen.
-00000520: 6e65 742f 6261 6467 652f 7171 2545 3725  net/badge/qq%E7%
-00000530: 4245 2541 342f 3232 3930 3336 3639 322f  BE%A4/229036692/
-00000540: 6f72 616e 6765 2220 616c 743d 2232 3239  orange" alt="229
-00000550: 3033 3636 3932 223e 0a20 2020 203c 2f61  036692">.    </a
-00000560: 3e0a 3c2f 703e 0a3c 7020 616c 6967 6e3d  >.</p>.<p align=
-00000570: 2263 656e 7465 7222 3e0a 2020 3c61 2068  "center">.  <a h
-00000580: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
-00000590: 6875 622e 636f 6d2f 616d 6973 6164 6d69  hub.com/amisadmi
-000005a0: 6e2f 6661 7374 6170 695f 616d 6973 5f61  n/fastapi_amis_a
-000005b0: 646d 696e 2220 7461 7267 6574 3d22 5f62  dmin" target="_b
-000005c0: 6c61 6e6b 223e e6ba 90e7 a081 3c2f 613e  lank">......</a>
-000005d0: 0a20 20c2 b70a 2020 3c61 2068 7265 663d  .  ...  <a href=
-000005e0: 2268 7474 703a 2f2f 6465 6d6f 2e61 6d69  "http://demo.ami
-000005f0: 732e 776f 726b 2f61 646d 696e 2220 7461  s.work/admin" ta
-00000600: 7267 6574 3d22 5f62 6c61 6e6b 223e e59c  rget="_blank">..
-00000610: a8e7 babf e6bc 94e7 a4ba 3c2f 613e 0a20  ..........</a>. 
-00000620: 20c2 b70a 2020 3c61 2068 7265 663d 2268   ...  <a href="h
-00000630: 7474 703a 2f2f 646f 6373 2e61 6d69 732e  ttp://docs.amis.
-00000640: 776f 726b 2220 7461 7267 6574 3d22 5f62  work" target="_b
-00000650: 6c61 6e6b 223e e696 87e6 a1a3 3c2f 613e  lank">......</a>
-00000660: 0a20 20c2 b70a 2020 3c61 2068 7265 663d  .  ...  <a href=
-00000670: 2268 7474 703a 2f2f 646f 6373 2e67 682e  "http://docs.gh.
-00000680: 616d 6973 2e77 6f72 6b22 2074 6172 6765  amis.work" targe
-00000690: 743d 225f 626c 616e 6b22 3ee6 9687 e6a1  t="_blank">.....
-000006a0: a3e6 8993 e4b8 8de5 bc80 efbc 9f3c 2f61  .............</a
-000006b0: 3e0a 3c2f 703e 0a0a 0a0a 2d2d 2d2d 2d2d  >.</p>....------
-000006c0: 0a0a 6066 6173 7461 7069 2d61 6d69 732d  ..`fastapi-amis-
-000006d0: 6164 6d69 6e60 e698 afe4 b880 e4b8 aae5  admin`..........
-000006e0: 9fba e4ba 8e60 6661 7374 6170 6960 2b60  .....`fastapi`+`
-000006f0: 616d 6973 60e5 bc80 e58f 91e7 9a84 e9ab  amis`...........
-00000700: 98e6 80a7 e883 bde5 b9b6 e4b8 94e9 ab98  ................
-00000710: e695 88e7 8e87 2060 7765 622d 6164 6d69  ...... `web-admi
-00000720: 6e60 20e6 a186 e69e b6ef bc8c e4bd bfe7  n` .............
-00000730: 94a8 2050 7974 686f 6e20 332e 372b 20e5  .. Python 3.7+ .
-00000740: b9b6 e59f bae4 ba8e e6a0 87e5 8786 e79a  ................
-00000750: 8420 5079 7468 6f6e 20e7 b1bb e59e 8be6  . Python .......
-00000760: 8f90 e7a4 ba2e 0a60 6661 7374 6170 692d  .......`fastapi-
-00000770: 616d 6973 2d61 646d 696e 60e5 bc80 e58f  amis-admin`.....
-00000780: 91e7 9a84 e588 9de8 a1b7 e698 afe4 b8ba  ................
-00000790: e4ba 86e5 ae8c e596 8460 6661 7374 6170  .........`fastap
-000007a0: 6960 e5ba 94e7 94a8 e794 9fe6 8081 2c20  i`............, 
-000007b0: e4b8 ba60 6661 7374 6170 6960 2077 6562  ...`fastapi` web
-000007c0: e5ba 94e7 94a8 e7a8 8be5 ba8f e5bf abe9  ................
-000007d0: 809f e794 9fe6 8890 e4b8 80e4 b8aa e58f  ................
-000007e0: afe8 a786 e58c 96e7 aea1 e790 86e5 908e  ................
-000007f0: e58f b02e 0a0a 2323 20e5 85b3 e994 aee7  ......## .......
-00000800: 89b9 e680 a70a 0a2d 202a 2ae6 80a7 e883  .......- **.....
-00000810: bde6 9e81 e9ab 982a 2aef bc9a e59f bae4  .......**.......
-00000820: ba8e 5b46 6173 7441 5049 5d28 6874 7470  ..[FastAPI](http
-00000830: 733a 2f2f 6661 7374 6170 692e 7469 616e  s://fastapi.tian
-00000840: 676f 6c6f 2e63 6f6d 2f7a 682f 292c 20e5  golo.com/zh/), .
-00000850: 8faf e4ba abe5 8f97 6046 6173 7441 5049  ........`FastAPI
-00000860: 60e7 9a84 e585 a8e9 83a8 e4bc 98e5 8abf  `...............
-00000870: 2e0a 0a2d 202a 2ae6 9588 e78e 87e6 9bb4  ...- **.........
-00000880: e5bf ab2a 2aef bc9a e5ae 8ce5 9684 e79a  ...**...........
-00000890: 84e7 bc96 e7a0 81e7 b1bb e59e 8be6 8f90  ................
-000008a0: e7a4 ba2c 20e4 bba3 e7a0 81e5 8faf e987  ..., ...........
-000008b0: 8de7 94a8 e680 a7e6 9bb4 e9ab 982e 0a0a  ................
-000008c0: 2d20 2a2a e694 afe6 8c81 e5bc 82e6 ada5  - **............
-000008d0: e592 8ce5 908c e6ad a5e6 b7b7 e590 88e7  ................
-000008e0: bc96 e586 992a 2a3a 2060 4f52 4d60 e59f  .....**: `ORM`..
-000008f0: bae4 ba8e 6053 514c 4d6f 6465 6c60 2b60  ....`SQLModel`+`
-00000900: 5371 6c61 6c63 6865 6d79 602c 20e5 8faf  Sqlalchemy`, ...
-00000910: e887 aae7 94b1 e5ae 9ae5 88b6 e695 b0e6  ................
-00000920: 8dae e5ba 93e7 b1bb e59e 8b2c 20e6 94af  ..........., ...
-00000930: e68c 81e5 908c e6ad a5e5 8f8a e5bc 82e6  ................
-00000940: ada5 e6a8 a1e5 bc8f 2c20 e58f afe6 8b93  ........, ......
-00000950: e5b1 95e6 80a7 e5bc ba2e 0a0a 2d20 2a2a  ............- **
-00000960: e589 8de5 908e e7ab afe5 8886 e7a6 bb2a  ...............*
-00000970: 2a3a 20e5 898d e7ab afe7 94b1 6041 6d69  *: .........`Ami
-00000980: 7360 e6b8 b2e6 9f93 2c20 e590 8ee7 abaf  s`......, ......
-00000990: e68e a5e5 8fa3 e794 b160 6661 7374 6170  .........`fastap
-000009a0: 692d 616d 6973 2d61 646d 696e 60e8 87aa  i-amis-admin`...
-000009b0: e58a a8e7 949f e688 902c 20e6 8ea5 e58f  ........., .....
-000009c0: a3e5 8faf e987 8de5 a48d e588 a9e7 94a8  ................
-000009d0: 2e0a 0a2d 202a 2ae5 8faf e68b 93e5 b195  ...- **.........
-000009e0: e680 a7e5 bcba 2a2a 3a20 e590 8ee5 8fb0  ......**: ......
-000009f0: e9a1 b5e9 9da2 e694 afe6 8c81 6041 6d69  ............`Ami
-00000a00: 7360 e9a1 b5e9 9da2 e58f 8ae6 99ae e980  s`..............
-00000a10: 9a60 6874 6d6c 60e9 a1b5 e99d a22c e5bc  .`html`......,..
-00000a20: 80e5 8f91 e880 85e5 8faf e4bb a5e5 be88  ................
-00000a30: e696 b9e4 bebf e79a 84e8 87aa e794 b1e5  ................
-00000a40: ae9a e588 b6e7 958c e99d a22e 0a0a 2d20  ..............- 
-00000a50: 2a2a e887 aae5 8aa8 e794 9fe6 8890 4150  **............AP
-00000a60: 49e6 9687 e6a1 a32a 2a3a 20e7 94b1 6046  I......**: ...`F
-00000a70: 6173 7441 5049 60e8 87aa e58a a8e7 949f  astAPI`.........
-00000a80: e688 90e6 8ea5 e58f a3e6 9687 e6a1 a32c  ...............,
-00000a90: e696 b9e4 bebf e5bc 80e5 8f91 e880 85e8  ................
-00000aa0: b083 e8af 952c e4bb a5e5 8f8a e68e a5e5  .....,..........
-00000ab0: 8fa3 e588 86e4 baab 2e0a 0a23 2320 e6a0  ...........## ..
-00000ac0: b8e5 bf83 e4be 9de8 b596 0a0a 2d20 5b46  ............- [F
-00000ad0: 6173 7441 5049 5d28 6874 7470 733a 2f2f  astAPI](https://
-00000ae0: 6661 7374 6170 692e 7469 616e 676f 6c6f  fastapi.tiangolo
-00000af0: 2e63 6f6d 2920 e8b4 9fe8 b4a3 2077 6562  .com) ...... web
-00000b00: 20e9 83a8 e588 860a 2d20 5b53 514c 4d6f   .......- [SQLMo
-00000b10: 6465 6c5d 2868 7474 7073 3a2f 2f73 716c  del](https://sql
-00000b20: 6d6f 6465 6c2e 7469 616e 676f 6c6f 2e63  model.tiangolo.c
-00000b30: 6f6d 2f29 20e8 b49f e8b4 a34f 524d e6a8  om/) ......ORM..
-00000b40: a1e5 9e8b e698 a0e5 b084 280a 2020 e5ae  ..........(.  ..
-00000b50: 8ce7 be8e e7bb 93e5 9088 5b53 514c 416c  ..........[SQLAl
-00000b60: 6368 656d 795d 2868 7474 7073 3a2f 2f77  chemy](https://w
-00000b70: 7777 2e73 716c 616c 6368 656d 792e 6f72  ww.sqlalchemy.or
-00000b80: 672f 292b 5b50 7964 616e 7469 635d 2868  g/)+[Pydantic](h
-00000b90: 7474 7073 3a2f 2f70 7964 616e 7469 632d  ttps://pydantic-
-00000ba0: 646f 6373 2e68 656c 706d 616e 7561 6c2e  docs.helpmanual.
-00000bb0: 696f 2f29 2c20 e68b a5e6 9c89 6053 514c  io/), ......`SQL
-00000bc0: 416c 6368 656d 7960 0a20 20e5 928c 6050  Alchemy`.  ...`P
-00000bd0: 7964 616e 7469 6360 e79a 84e6 8980 e69c  ydantic`........
-00000be0: 89e5 8a9f e883 bd29 0a2d 205b 416d 6973  .......).- [Amis
-00000bf0: 5d28 6874 7470 733a 2f2f 6261 6964 752e  ](https://baidu.
-00000c00: 6769 7465 652e 696f 2f61 6d69 7329 20e8  gitee.io/amis) .
-00000c10: b49f e8b4 a341 646d 696e e590 8ee5 8fb0  .....Admin......
-00000c20: e9a1 b5e9 9da2 e5b1 95e7 a4ba 0a0a 2323  ..............##
-00000c30: 20e9 a1b9 e79b aee7 bb84 e688 900a 0a60   ..............`
-00000c40: 6661 7374 6170 692d 616d 6973 2d61 646d  fastapi-amis-adm
-00000c50: 696e 60e7 94b1 e4b8 89e9 83a8 e588 86e6  in`.............
-00000c60: a0b8 e5bf 83e6 a8a1 e59d 97e7 bb84 e688  ................
-00000c70: 902c e585 b6e4 b8ad 6061 6d69 7360 2c20  .,......`amis`, 
-00000c80: 6063 7275 6460 20e5 8faf e4bd 9ce4 b8ba  `crud` .........
-00000c90: e78b ace7 ab8b e6a8 a1e5 9d97 e58d 95e7  ................
-00000ca0: 8bac e4bd bfe7 94a8 2c60 6164 6d69 6e60  ........,`admin`
-00000cb0: e59f bae4 ba8e e589 8de8 8085 e585 b1e5  ................
-00000cc0: 908c e69e 84e5 bbba 2e0a 0a2d 2060 616d  ...........- `am
-00000cd0: 6973 603a 20e5 9fba e4ba 8e60 6261 6964  is`: ......`baid
-00000ce0: 7520 616d 6973 60e7 9a84 6070 7964 616e  u amis`...`pydan
-00000cf0: 7469 6360 e695 b0e6 8dae e6a8 a1e5 9e8b  tic`............
-00000d00: e69e 84e5 bbba e5ba 932c e794 a8e4 ba8e  .........,......
-00000d10: e5bf abe9 809f e794 9fe6 8890 2fe8 a7a3  ............/...
-00000d20: e69e 9060 616d 6973 6020 606a 736f 6e60  ...`amis` `json`
-00000d30: 20e6 95b0 e68d ae2e 0a2d 2060 6372 7564   ........- `crud
-00000d40: 603a 20e5 9fba e4ba 8e60 4661 7374 4150  `: ......`FastAP
-00000d50: 4960 2b60 5371 6c61 6c63 6865 6d79 602c  I`+`Sqlalchemy`,
-00000d60: 20e7 94a8 e4ba 8ee5 bfab e980 9fe6 9e84   ...............
-00000d70: e5bb ba43 7265 6174 652c 5265 6164 2c55  ...Create,Read,U
-00000d80: 7064 6174 652c 4465 6c65 7465 e980 9ae7  pdate,Delete....
-00000d90: 94a8 4150 49e6 8ea5 e58f a32e 0a2d 2060  ..API........- `
-00000da0: 6164 6d69 6e60 3a20 e590 afe5 8f91 e887  admin`: ........
-00000db0: aa60 446a 616e 676f 2d41 646d 696e 602c  .`Django-Admin`,
-00000dc0: 20e7 bb93 e590 8860 616d 6973 602b 6063   ......`amis`+`c
-00000dd0: 7275 6460 2c20 e794 a8e4 ba8e e5bf abe9  rud`, ..........
-00000de0: 809f e69e 84e5 bbba 6057 6562 2041 646d  ........`Web Adm
-00000df0: 696e 60e7 aea1 e790 86e5 908e e58f b02e  in`.............
-00000e00: 0a0a 2323 20e5 ae89 e8a3 850a 0a60 6060  ..## ........```
-00000e10: 6261 7368 0a70 6970 2069 6e73 7461 6c6c  bash.pip install
-00000e20: 2066 6173 7461 7069 5f61 6d69 735f 6164   fastapi_amis_ad
-00000e30: 6d69 6e0a 6060 600a 0a23 2323 20e6 b3a8  min.```..### ...
-00000e40: e684 8f0a 0a2d 2060 7371 6c6d 6f64 656c  .....- `sqlmodel
-00000e50: 60e7 9bae e589 8de6 9a82 e4b8 8de6 94af  `...............
-00000e60: e68c 8160 7371 6c61 6c63 6865 6d79 2032  ...`sqlalchemy 2
-00000e70: 2e30 2b60 2c20 e5a6 82e6 9e9c e4bd a0e4  .0+`, ..........
-00000e80: bdbf e794 a860 7371 6c61 6c63 6865 6d79  .....`sqlalchemy
-00000e90: 2032 2e30 2b60 e588 9be5 bbba e6a8 a1e5   2.0+`..........
-00000ea0: 9e8b 2c20 e588 99e4 b88d e58f afe5 908c  .., ............
-00000eb0: e697 b6e4 bdbf e794 a860 7371 6c6d 6f64  .........`sqlmod
-00000ec0: 656c 602e 0a2d 2060 6661 7374 6170 692d  el`..- `fastapi-
-00000ed0: 616d 6973 2d61 646d 696e 3e3d 302e 362e  amis-admin>=0.6.
-00000ee0: 3060 e789 88e6 9cac e4bb a5e5 908e 2c60  0`............,`
-00000ef0: 7371 6c6d 6f64 656c 60e4 b88d e586 8de6  sqlmodel`.......
-00000f00: 98af e5bf 85e9 a1bb e4be 9de8 b596 e5ba  ................
-00000f10: 932c e5a6 82e6 9e9c e4bd a0e4 bdbf e794  .,..............
-00000f20: a860 7371 6c6d 6f64 656c 60e5 889b e5bb  .`sqlmodel`.....
-00000f30: bae6 a8a1 e59e 8b2c 20e5 8faf e4bb a5e9  ......., .......
-00000f40: 809a e8bf 87e4 bba5 e4b8 8be5 91bd e4bb  ................
-00000f50: a4e5 ae89 e8a3 852e 0a0a 6060 6062 6173  ..........```bas
-00000f60: 680a 7069 7020 696e 7374 616c 6c20 6661  h.pip install fa
-00000f70: 7374 6170 695f 616d 6973 5f61 646d 696e  stapi_amis_admin
-00000f80: 5b73 716c 6d6f 6465 6c5d 0a60 6060 200a  [sqlmodel].``` .
-00000f90: 0a23 2320 e7ae 80e5 8d95 e7a4 bae4 be8b  .## ............
-00000fa0: 0a0a 6060 6070 7974 686f 6e0a 6672 6f6d  ..```python.from
-00000fb0: 2066 6173 7461 7069 2069 6d70 6f72 7420   fastapi import 
-00000fc0: 4661 7374 4150 490a 6672 6f6d 2066 6173  FastAPI.from fas
-00000fd0: 7461 7069 5f61 6d69 735f 6164 6d69 6e2e  tapi_amis_admin.
-00000fe0: 6164 6d69 6e2e 7365 7474 696e 6773 2069  admin.settings i
-00000ff0: 6d70 6f72 7420 5365 7474 696e 6773 0a66  mport Settings.f
-00001000: 726f 6d20 6661 7374 6170 695f 616d 6973  rom fastapi_amis
-00001010: 5f61 646d 696e 2e61 646d 696e 2e73 6974  _admin.admin.sit
-00001020: 6520 696d 706f 7274 2041 646d 696e 5369  e import AdminSi
-00001030: 7465 0a0a 2320 e588 9be5 bbba 4661 7374  te..# ......Fast
-00001040: 4150 49e5 ba94 e794 a80a 6170 7020 3d20  API.......app = 
-00001050: 4661 7374 4150 4928 290a 0a23 20e5 889b  FastAPI()..# ...
-00001060: e5bb ba41 646d 696e 5369 7465 e5ae 9ee4  ...AdminSite....
-00001070: be8b 0a73 6974 6520 3d20 4164 6d69 6e53  ...site = AdminS
-00001080: 6974 6528 7365 7474 696e 6773 3d53 6574  ite(settings=Set
-00001090: 7469 6e67 7328 6461 7461 6261 7365 5f75  tings(database_u
-000010a0: 726c 5f61 7379 6e63 3d27 7371 6c69 7465  rl_async='sqlite
-000010b0: 2b61 696f 7371 6c69 7465 3a2f 2f2f 616d  +aiosqlite:///am
-000010c0: 6973 6164 6d69 6e2e 6462 2729 290a 0a23  isadmin.db'))..#
-000010d0: 20e6 8c82 e8bd bde5 908e e58f b0e7 aea1   ...............
-000010e0: e790 86e7 b3bb e7bb 9f0a 7369 7465 2e6d  ..........site.m
-000010f0: 6f75 6e74 5f61 7070 2861 7070 290a 0a69  ount_app(app)..i
-00001100: 6620 5f5f 6e61 6d65 5f5f 203d 3d20 275f  f __name__ == '_
-00001110: 5f6d 6169 6e5f 5f27 3a0a 2020 2020 696d  _main__':.    im
-00001120: 706f 7274 2075 7669 636f 726e 0a0a 2020  port uvicorn..  
-00001130: 2020 7576 6963 6f72 6e2e 7275 6e28 6170    uvicorn.run(ap
-00001140: 7029 0a60 6060 0a0a 2323 20e6 a8a1 e59e  p).```..## .....
-00001150: 8be7 aea1 e790 86e7 a4ba e4be 8b0a 0a23  ...............#
-00001160: 2323 20e5 889b e5bb bae6 a8a1 e59e 8b0a  ## .............
-00001170: 0a2d 20e6 94af e68c 8160 5351 4c4d 6f64  .- ......`SQLMod
-00001180: 656c 60e6 a8a1 e59e 8be7 9a84 e380 8160  el`............`
-00001190: 5351 4c41 6c63 6865 6d79 60e6 a8a1 e59e  SQLAlchemy`.....
-000011a0: 8be3 8081 6053 514c 416c 6368 656d 7920  ....`SQLAlchemy 
-000011b0: 322e 3060 e6a8 a1e5 9e8b 0a2d 20e6 96b9  2.0`.......- ...
-000011c0: e5bc 8fe4 b880 3a20 e980 9ae8 bf87 6053  ......: ......`S
-000011d0: 514c 4d6f 6465 6c60 e588 9be5 bbba e6a8  QLModel`........
-000011e0: a1e5 9e8b 2e0a 0a60 6060 7079 7468 6f6e  .......```python
-000011f0: 0a66 726f 6d20 7371 6c6d 6f64 656c 2069  .from sqlmodel i
-00001200: 6d70 6f72 7420 5351 4c4d 6f64 656c 0a66  mport SQLModel.f
-00001210: 726f 6d20 6661 7374 6170 695f 616d 6973  rom fastapi_amis
-00001220: 5f61 646d 696e 2e6d 6f64 656c 732e 6669  _admin.models.fi
-00001230: 656c 6473 2069 6d70 6f72 7420 4669 656c  elds import Fiel
-00001240: 640a 0a0a 636c 6173 7320 4261 7365 2853  d...class Base(S
-00001250: 514c 4d6f 6465 6c29 3a0a 2020 2020 7061  QLModel):.    pa
-00001260: 7373 0a0a 0a23 20e5 889b e5bb ba53 514c  ss...# ......SQL
-00001270: 4d6f 6465 6ce6 a8a1 e59e 8b2c e8af a6e7  Model......,....
-00001280: bb86 e8af b7e5 8f82 e880 833a 2068 7474  ...........: htt
-00001290: 7073 3a2f 2f73 716c 6d6f 6465 6c2e 7469  ps://sqlmodel.ti
-000012a0: 616e 676f 6c6f 2e63 6f6d 2f0a 636c 6173  angolo.com/.clas
-000012b0: 7320 4361 7465 676f 7279 2853 514c 4d6f  s Category(SQLMo
-000012c0: 6465 6c2c 2074 6162 6c65 3d54 7275 6529  del, table=True)
-000012d0: 3a0a 2020 2020 6964 3a20 696e 7420 3d20  :.    id: int = 
-000012e0: 4669 656c 6428 6465 6661 756c 743d 4e6f  Field(default=No
-000012f0: 6e65 2c20 7072 696d 6172 795f 6b65 793d  ne, primary_key=
-00001300: 5472 7565 2c20 6e75 6c6c 6162 6c65 3d46  True, nullable=F
-00001310: 616c 7365 290a 2020 2020 6e61 6d65 3a20  alse).    name: 
-00001320: 7374 7220 3d20 4669 656c 6428 7469 746c  str = Field(titl
-00001330: 653d 2743 6174 6567 6f72 794e 616d 6527  e='CategoryName'
-00001340: 2c20 6d61 785f 6c65 6e67 7468 3d31 3030  , max_length=100
-00001350: 2c20 756e 6971 7565 3d54 7275 652c 2069  , unique=True, i
-00001360: 6e64 6578 3d54 7275 652c 206e 756c 6c61  ndex=True, nulla
-00001370: 626c 653d 4661 6c73 6529 0a20 2020 2064  ble=False).    d
-00001380: 6573 6372 6970 7469 6f6e 3a20 7374 7220  escription: str 
-00001390: 3d20 4669 656c 6428 6465 6661 756c 743d  = Field(default=
-000013a0: 2727 2c20 7469 746c 653d 2744 6573 6372  '', title='Descr
-000013b0: 6970 7469 6f6e 272c 206d 6178 5f6c 656e  iption', max_len
-000013c0: 6774 683d 3235 3529 0a0a 6060 600a 0a2d  gth=255)..```..-
-000013d0: 20e6 96b9 e5bc 8fe4 ba8c 3a20 e980 9ae8   .........: ....
-000013e0: bf87 6053 514c 416c 6368 656d 7960 e588  ..`SQLAlchemy`..
-000013f0: 9be5 bbba e6a8 a1e5 9e8b 2e0a 0a60 6060  .............```
-00001400: 7079 7468 6f6e 0a66 726f 6d20 7371 6c61  python.from sqla
-00001410: 6c63 6865 6d79 2069 6d70 6f72 7420 436f  lchemy import Co
-00001420: 6c75 6d6e 2c20 496e 7465 6765 722c 2053  lumn, Integer, S
-00001430: 7472 696e 670a 6672 6f6d 2073 716c 616c  tring.from sqlal
-00001440: 6368 656d 792e 6578 742e 6465 636c 6172  chemy.ext.declar
-00001450: 6174 6976 6520 696d 706f 7274 2064 6563  ative import dec
-00001460: 6c61 7261 7469 7665 5f62 6173 650a 0a42  larative_base..B
-00001470: 6173 6520 3d20 6465 636c 6172 6174 6976  ase = declarativ
-00001480: 655f 6261 7365 2829 0a0a 0a23 20e5 889b  e_base()...# ...
-00001490: e5bb ba53 514c 416c 6368 656d 79e6 a8a1  ...SQLAlchemy...
-000014a0: e59e 8b2c e8af a6e7 bb86 e8af b7e5 8f82  ...,............
-000014b0: e880 833a 2068 7474 7073 3a2f 2f64 6f63  ...: https://doc
-000014c0: 732e 7371 6c61 6c63 6865 6d79 2e6f 7267  s.sqlalchemy.org
-000014d0: 2f65 6e2f 3134 2f6f 726d 2f74 7574 6f72  /en/14/orm/tutor
-000014e0: 6961 6c2e 6874 6d6c 0a63 6c61 7373 2043  ial.html.class C
-000014f0: 6174 6567 6f72 7928 4261 7365 293a 0a20  ategory(Base):. 
-00001500: 2020 205f 5f74 6162 6c65 6e61 6d65 5f5f     __tablename__
-00001510: 203d 2027 6361 7465 676f 7279 270a 2020   = 'category'.  
-00001520: 2020 5f5f 7079 6461 6e74 6963 5f6d 6f64    __pydantic_mod
-00001530: 656c 5f5f 203d 2043 6174 6567 6f72 7953  el__ = CategoryS
-00001540: 6368 656d 6120 2023 20e6 8c87 e5ae 9ae6  chema  # .......
-00001550: a8a1 e59e 8be5 afb9 e5ba 94e7 9a84 5363  ..............Sc
-00001560: 6865 6d61 e7b1 bb2e e79c 81e7 95a5 e58f  hema............
-00001570: afe8 87aa e58a a8e7 949f e688 902c e4bd  .............,..
-00001580: 86e6 98af e5bb bae8 aeae e68c 87e5 ae9a  ................
-00001590: 2e0a 0a20 2020 2069 6420 3d20 436f 6c75  ...    id = Colu
-000015a0: 6d6e 2849 6e74 6567 6572 2c20 7072 696d  mn(Integer, prim
-000015b0: 6172 795f 6b65 793d 5472 7565 2c20 6e75  ary_key=True, nu
-000015c0: 6c6c 6162 6c65 3d46 616c 7365 290a 2020  llable=False).  
-000015d0: 2020 6e61 6d65 203d 2043 6f6c 756d 6e28    name = Column(
-000015e0: 5374 7269 6e67 2831 3030 292c 2075 6e69  String(100), uni
-000015f0: 7175 653d 5472 7565 2c20 696e 6465 783d  que=True, index=
-00001600: 5472 7565 2c20 6e75 6c6c 6162 6c65 3d46  True, nullable=F
-00001610: 616c 7365 290a 2020 2020 6465 7363 7269  alse).    descri
-00001620: 7074 696f 6e20 3d20 436f 6c75 6d6e 2853  ption = Column(S
-00001630: 7472 696e 6728 3235 3529 2c20 6465 6661  tring(255), defa
-00001640: 756c 743d 2727 290a 6060 600a 0a2d 20e6  ult='').```..- .
-00001650: 96b9 e5bc 8fe4 b889 3a20 e980 9ae8 bf87  ........: ......
-00001660: 6053 514c 416c 6368 656d 7920 322e 3060  `SQLAlchemy 2.0`
-00001670: e588 9be5 bbba e6a8 a1e5 9e8b 2e0a 0a60  ...............`
-00001680: 6060 7079 7468 6f6e 0a66 726f 6d20 7371  ``python.from sq
-00001690: 6c61 6c63 6865 6d79 2069 6d70 6f72 7420  lalchemy import 
-000016a0: 5374 7269 6e67 0a66 726f 6d20 7371 6c61  String.from sqla
-000016b0: 6c63 6865 6d79 2e6f 726d 2069 6d70 6f72  lchemy.orm impor
-000016c0: 7420 4465 636c 6172 6174 6976 6542 6173  t DeclarativeBas
-000016d0: 652c 204d 6170 7065 642c 206d 6170 7065  e, Mapped, mappe
-000016e0: 645f 636f 6c75 6d6e 0a0a 0a63 6c61 7373  d_column...class
-000016f0: 2042 6173 6528 4465 636c 6172 6174 6976   Base(Declarativ
-00001700: 6542 6173 6529 3a0a 2020 2020 7061 7373  eBase):.    pass
-00001710: 0a0a 0a23 20e5 889b e5bb ba53 514c 416c  ...# ......SQLAl
-00001720: 6368 656d 7920 322e 30e6 a8a1 e59e 8b2c  chemy 2.0......,
-00001730: e8af a6e7 bb86 e8af b7e5 8f82 e880 833a  ...............:
-00001740: 2068 7474 7073 3a2f 2f64 6f63 732e 7371   https://docs.sq
-00001750: 6c61 6c63 6865 6d79 2e6f 7267 2f65 6e2f  lalchemy.org/en/
-00001760: 3230 2f6f 726d 2f71 7569 636b 7374 6172  20/orm/quickstar
-00001770: 742e 6874 6d6c 0a63 6c61 7373 2043 6174  t.html.class Cat
-00001780: 6567 6f72 7928 4261 7365 293a 0a20 2020  egory(Base):.   
-00001790: 205f 5f74 6162 6c65 6e61 6d65 5f5f 203d   __tablename__ =
-000017a0: 2022 6361 7465 676f 7279 220a 2020 2020   "category".    
-000017b0: 5f5f 7079 6461 6e74 6963 5f6d 6f64 656c  __pydantic_model
-000017c0: 5f5f 203d 2043 6174 6567 6f72 7953 6368  __ = CategorySch
-000017d0: 656d 6120 2023 20e6 8c87 e5ae 9ae6 a8a1  ema  # .........
-000017e0: e59e 8be5 afb9 e5ba 94e7 9a84 5363 6865  ............Sche
-000017f0: 6d61 e7b1 bb2e e79c 81e7 95a5 e58f afe8  ma..............
-00001800: 87aa e58a a8e7 949f e688 902c e4bd 86e6  ...........,....
-00001810: 98af e5bb bae8 aeae e68c 87e5 ae9a 2e0a  ................
-00001820: 0a20 2020 2069 643a 204d 6170 7065 645b  .    id: Mapped[
-00001830: 696e 745d 203d 206d 6170 7065 645f 636f  int] = mapped_co
-00001840: 6c75 6d6e 2870 7269 6d61 7279 5f6b 6579  lumn(primary_key
-00001850: 3d54 7275 652c 206e 756c 6c61 626c 653d  =True, nullable=
-00001860: 4661 6c73 6529 0a20 2020 206e 616d 653a  False).    name:
-00001870: 204d 6170 7065 645b 7374 725d 203d 206d   Mapped[str] = m
-00001880: 6170 7065 645f 636f 6c75 6d6e 2853 7472  apped_column(Str
-00001890: 696e 6728 3130 3029 2c20 756e 6971 7565  ing(100), unique
-000018a0: 3d54 7275 652c 2069 6e64 6578 3d54 7275  =True, index=Tru
-000018b0: 652c 206e 756c 6c61 626c 653d 4661 6c73  e, nullable=Fals
-000018c0: 6529 0a20 2020 2064 6573 6372 6970 7469  e).    descripti
-000018d0: 6f6e 3a20 4d61 7070 6564 5b73 7472 5d20  on: Mapped[str] 
-000018e0: 3d20 6d61 7070 6564 5f63 6f6c 756d 6e28  = mapped_column(
-000018f0: 5374 7269 6e67 2832 3535 292c 2064 6566  String(255), def
-00001900: 6175 6c74 3d22 2229 0a60 6060 0a0a 2d20  ault="").```..- 
-00001910: e5a6 82e6 9e9c e4bd a0e9 809a e8bf 8760  ...............`
-00001920: 7371 6c61 6c63 6865 6d79 60e5 889b e5bb  sqlalchemy`.....
-00001930: bae6 a8a1 e59e 8b2c e5bb bae8 aeae e590  .......,........
-00001940: 8ce6 97b6 e588 9be5 bbba e4b8 80e4 b8aa  ................
-00001950: e5af b9e5 ba94 e79a 8470 7964 616e 7469  .........pydanti
-00001960: 63e6 a8a1 e59e 8b2c e5b9 b6e4 b894 e8ae  c......,........
-00001970: bee7 bdae 606f 726d 5f6d 6f64 653d 5472  ....`orm_mode=Tr
-00001980: 7565 602e 0a0a 6060 6070 7974 686f 6e0a  ue`...```python.
-00001990: 6672 6f6d 2070 7964 616e 7469 6320 696d  from pydantic im
-000019a0: 706f 7274 2042 6173 654d 6f64 656c 2c20  port BaseModel, 
-000019b0: 4669 656c 640a 0a0a 636c 6173 7320 4361  Field...class Ca
-000019c0: 7465 676f 7279 5363 6865 6d61 2842 6173  tegorySchema(Bas
-000019d0: 654d 6f64 656c 293a 0a20 2020 2069 643a  eModel):.    id:
-000019e0: 2069 6e74 203d 2046 6965 6c64 2864 6566   int = Field(def
-000019f0: 6175 6c74 3d4e 6f6e 652c 2070 7269 6d61  ault=None, prima
-00001a00: 7279 5f6b 6579 3d54 7275 652c 206e 756c  ry_key=True, nul
-00001a10: 6c61 626c 653d 4661 6c73 6529 0a20 2020  lable=False).   
-00001a20: 206e 616d 653a 2073 7472 203d 2046 6965   name: str = Fie
-00001a30: 6c64 2874 6974 6c65 3d22 4361 7465 676f  ld(title="Catego
-00001a40: 7279 4e61 6d65 2229 0a20 2020 2064 6573  ryName").    des
-00001a50: 6372 6970 7469 6f6e 3a20 7374 7220 3d20  cription: str = 
-00001a60: 4669 656c 6428 6465 6661 756c 743d 2222  Field(default=""
-00001a70: 2c20 7469 746c 653d 2243 6174 6567 6f72  , title="Categor
-00001a80: 7944 6573 6372 6970 7469 6f6e 2229 0a0a  yDescription")..
-00001a90: 2020 2020 636c 6173 7320 436f 6e66 6967      class Config
-00001aa0: 3a0a 2020 2020 2020 2020 6f72 6d5f 6d6f  :.        orm_mo
-00001ab0: 6465 203d 2054 7275 650a 6060 600a 0a23  de = True.```..#
-00001ac0: 2323 20e6 b3a8 e586 8ce6 a8a1 e59e 8be7  ## .............
-00001ad0: aea1 e790 860a 0a60 6060 7079 7468 6f6e  .......```python
-00001ae0: 0a66 726f 6d20 6661 7374 6170 6920 696d  .from fastapi im
-00001af0: 706f 7274 2046 6173 7441 5049 0a66 726f  port FastAPI.fro
-00001b00: 6d20 7371 6c6d 6f64 656c 2069 6d70 6f72  m sqlmodel impor
-00001b10: 7420 5351 4c4d 6f64 656c 0a66 726f 6d20  t SQLModel.from 
-00001b20: 6661 7374 6170 695f 616d 6973 5f61 646d  fastapi_amis_adm
-00001b30: 696e 2e61 646d 696e 2e73 6574 7469 6e67  in.admin.setting
-00001b40: 7320 696d 706f 7274 2053 6574 7469 6e67  s import Setting
-00001b50: 730a 6672 6f6d 2066 6173 7461 7069 5f61  s.from fastapi_a
-00001b60: 6d69 735f 6164 6d69 6e2e 6164 6d69 6e2e  mis_admin.admin.
-00001b70: 7369 7465 2069 6d70 6f72 7420 4164 6d69  site import Admi
-00001b80: 6e53 6974 650a 6672 6f6d 2066 6173 7461  nSite.from fasta
-00001b90: 7069 5f61 6d69 735f 6164 6d69 6e2e 6164  pi_amis_admin.ad
-00001ba0: 6d69 6e20 696d 706f 7274 2061 646d 696e  min import admin
-00001bb0: 0a0a 2320 e588 9be5 bbba 4661 7374 4150  ..# ......FastAP
-00001bc0: 49e5 ba94 e794 a80a 6170 7020 3d20 4661  I.......app = Fa
-00001bd0: 7374 4150 4928 290a 0a23 20e5 889b e5bb  stAPI()..# .....
-00001be0: ba41 646d 696e 5369 7465 e5ae 9ee4 be8b  .AdminSite......
-00001bf0: 0a73 6974 6520 3d20 4164 6d69 6e53 6974  .site = AdminSit
-00001c00: 6528 7365 7474 696e 6773 3d53 6574 7469  e(settings=Setti
-00001c10: 6e67 7328 6461 7461 6261 7365 5f75 726c  ngs(database_url
-00001c20: 5f61 7379 6e63 3d27 7371 6c69 7465 2b61  _async='sqlite+a
-00001c30: 696f 7371 6c69 7465 3a2f 2f2f 616d 6973  iosqlite:///amis
-00001c40: 6164 6d69 6e2e 6462 2729 290a 0a0a 2320  admin.db'))...# 
-00001c50: e6b3 a8e5 868c 4d6f 6465 6c41 646d 696e  ......ModelAdmin
-00001c60: 0a40 7369 7465 2e72 6567 6973 7465 725f  .@site.register_
-00001c70: 6164 6d69 6e0a 636c 6173 7320 4361 7465  admin.class Cate
-00001c80: 676f 7279 4164 6d69 6e28 6164 6d69 6e2e  goryAdmin(admin.
-00001c90: 4d6f 6465 6c41 646d 696e 293a 0a20 2020  ModelAdmin):.   
-00001ca0: 2070 6167 655f 7363 6865 6d61 203d 2027   page_schema = '
-00001cb0: e588 86e7 b1bb e7ae a1e7 9086 270a 2020  ............'.  
-00001cc0: 2020 2320 e985 8de7 bdae e7ae a1e7 9086    # ............
-00001cd0: e6a8 a1e5 9e8b 0a20 2020 206d 6f64 656c  .......    model
-00001ce0: 203d 2043 6174 6567 6f72 790a 0a0a 2320   = Category...# 
-00001cf0: e68c 82e8 bdbd e590 8ee5 8fb0 e7ae a1e7  ................
-00001d00: 9086 e7b3 bbe7 bb9f 0a73 6974 652e 6d6f  .........site.mo
-00001d10: 756e 745f 6170 7028 6170 7029 0a0a 0a23  unt_app(app)...#
-00001d20: 20e5 889b e5bb bae5 889d e5a7 8be5 8c96   ...............
-00001d30: e695 b0e6 8dae e5ba 93e8 a1a8 0a40 6170  .............@ap
-00001d40: 702e 6f6e 5f65 7665 6e74 2822 7374 6172  p.on_event("star
-00001d50: 7475 7022 290a 6173 796e 6320 6465 6620  tup").async def 
-00001d60: 7374 6172 7475 7028 293a 0a20 2020 2061  startup():.    a
-00001d70: 7761 6974 2073 6974 652e 6462 2e61 7379  wait site.db.asy
-00001d80: 6e63 5f72 756e 5f73 796e 6328 4261 7365  nc_run_sync(Base
-00001d90: 2e6d 6574 6164 6174 612e 6372 6561 7465  .metadata.create
-00001da0: 5f61 6c6c 2c20 6973 5f73 6573 7369 6f6e  _all, is_session
-00001db0: 3d46 616c 7365 290a 0a0a 6966 205f 5f6e  =False)...if __n
-00001dc0: 616d 655f 5f20 3d3d 2027 5f5f 6d61 696e  ame__ == '__main
-00001dd0: 5f5f 273a 0a20 2020 2069 6d70 6f72 7420  __':.    import 
-00001de0: 7576 6963 6f72 6e0a 0a20 2020 2075 7669  uvicorn..    uvi
-00001df0: 636f 726e 2e72 756e 2861 7070 290a 6060  corn.run(app).``
-00001e00: 600a 0a23 2320 e8a1 a8e5 8d95 e7ae a1e7  `..## ..........
-00001e10: 9086 e7a4 bae4 be8b 0a0a 6060 6070 7974  ..........```pyt
-00001e20: 686f 6e0a 6672 6f6d 2074 7970 696e 6720  hon.from typing 
-00001e30: 696d 706f 7274 2041 6e79 0a66 726f 6d20  import Any.from 
-00001e40: 6661 7374 6170 6920 696d 706f 7274 2046  fastapi import F
-00001e50: 6173 7441 5049 0a66 726f 6d20 7079 6461  astAPI.from pyda
-00001e60: 6e74 6963 2069 6d70 6f72 7420 4261 7365  ntic import Base
-00001e70: 4d6f 6465 6c0a 6672 6f6d 2073 7461 726c  Model.from starl
-00001e80: 6574 7465 2e72 6571 7565 7374 7320 696d  ette.requests im
-00001e90: 706f 7274 2052 6571 7565 7374 0a66 726f  port Request.fro
-00001ea0: 6d20 6661 7374 6170 695f 616d 6973 5f61  m fastapi_amis_a
-00001eb0: 646d 696e 2e61 6d69 732e 636f 6d70 6f6e  dmin.amis.compon
-00001ec0: 656e 7473 2069 6d70 6f72 7420 466f 726d  ents import Form
-00001ed0: 0a66 726f 6d20 6661 7374 6170 695f 616d  .from fastapi_am
-00001ee0: 6973 5f61 646d 696e 2e61 646d 696e 2069  is_admin.admin i
-00001ef0: 6d70 6f72 7420 6164 6d69 6e0a 6672 6f6d  mport admin.from
-00001f00: 2066 6173 7461 7069 5f61 6d69 735f 6164   fastapi_amis_ad
-00001f10: 6d69 6e2e 6164 6d69 6e2e 7365 7474 696e  min.admin.settin
-00001f20: 6773 2069 6d70 6f72 7420 5365 7474 696e  gs import Settin
-00001f30: 6773 0a66 726f 6d20 6661 7374 6170 695f  gs.from fastapi_
-00001f40: 616d 6973 5f61 646d 696e 2e61 646d 696e  amis_admin.admin
-00001f50: 2e73 6974 6520 696d 706f 7274 2041 646d  .site import Adm
-00001f60: 696e 5369 7465 0a66 726f 6d20 6661 7374  inSite.from fast
-00001f70: 6170 695f 616d 6973 5f61 646d 696e 2e63  api_amis_admin.c
-00001f80: 7275 642e 7363 6865 6d61 2069 6d70 6f72  rud.schema impor
-00001f90: 7420 4261 7365 4170 694f 7574 0a66 726f  t BaseApiOut.fro
-00001fa0: 6d20 6661 7374 6170 695f 616d 6973 5f61  m fastapi_amis_a
-00001fb0: 646d 696e 2e6d 6f64 656c 732e 6669 656c  dmin.models.fiel
-00001fc0: 6473 2069 6d70 6f72 7420 4669 656c 640a  ds import Field.
-00001fd0: 0a23 20e5 889b e5bb ba46 6173 7441 5049  .# ......FastAPI
-00001fe0: e5ba 94e7 94a8 0a61 7070 203d 2046 6173  .......app = Fas
-00001ff0: 7441 5049 2829 0a0a 2320 e588 9be5 bbba  tAPI()..# ......
-00002000: 4164 6d69 6e53 6974 65e5 ae9e e4be 8b0a  AdminSite.......
-00002010: 7369 7465 203d 2041 646d 696e 5369 7465  site = AdminSite
-00002020: 2873 6574 7469 6e67 733d 5365 7474 696e  (settings=Settin
-00002030: 6773 2864 6174 6162 6173 655f 7572 6c5f  gs(database_url_
-00002040: 6173 796e 633d 2773 716c 6974 652b 6169  async='sqlite+ai
-00002050: 6f73 716c 6974 653a 2f2f 2f61 6d69 7361  osqlite:///amisa
-00002060: 646d 696e 2e64 6227 2929 0a0a 0a23 20e6  dmin.db'))...# .
-00002070: b3a8 e586 8c46 6f72 6d41 646d 696e 0a40  .....FormAdmin.@
-00002080: 7369 7465 2e72 6567 6973 7465 725f 6164  site.register_ad
-00002090: 6d69 6e0a 636c 6173 7320 5573 6572 4c6f  min.class UserLo
-000020a0: 6769 6e46 6f72 6d41 646d 696e 2861 646d  ginFormAdmin(adm
-000020b0: 696e 2e46 6f72 6d41 646d 696e 293a 0a20  in.FormAdmin):. 
-000020c0: 2020 2070 6167 655f 7363 6865 6d61 203d     page_schema =
-000020d0: 2027 5573 6572 4c6f 6769 6e46 6f72 6d27   'UserLoginForm'
-000020e0: 0a20 2020 2023 20e9 858d e7bd aee8 a1a8  .    # .........
-000020f0: e58d 95e4 bfa1 e681 af2c 20e5 8faf e79c  ........., .....
-00002100: 81e7 95a5 0a20 2020 2066 6f72 6d20 3d20  .....    form = 
-00002110: 466f 726d 2874 6974 6c65 3d27 e8bf 99e6  Form(title='....
-00002120: 98af e4b8 80e4 b8aa e6b5 8be8 af95 e799  ................
-00002130: bbe5 bd95 e8a1 a8e5 8d95 272c 2073 7562  ..........', sub
-00002140: 6d69 7454 6578 743d 27e7 99bb e5bd 9527  mitText='......'
-00002150: 290a 0a20 2020 2023 20e5 889b e5bb bae8  )..    # .......
-00002160: a1a8 e58d 95e6 95b0 e68d aee6 a8a1 e59e  ................
-00002170: 8b0a 2020 2020 636c 6173 7320 7363 6865  ..    class sche
-00002180: 6d61 2842 6173 654d 6f64 656c 293a 0a20  ma(BaseModel):. 
-00002190: 2020 2020 2020 2075 7365 726e 616d 653a         username:
-000021a0: 2073 7472 203d 2046 6965 6c64 282e 2e2e   str = Field(...
-000021b0: 2c20 7469 746c 653d 27e7 94a8 e688 b7e5  , title='.......
-000021c0: 908d 272c 206d 696e 5f6c 656e 6774 683d  ..', min_length=
-000021d0: 332c 206d 6178 5f6c 656e 6774 683d 3330  3, max_length=30
-000021e0: 290a 2020 2020 2020 2020 7061 7373 776f  ).        passwo
-000021f0: 7264 3a20 7374 7220 3d20 4669 656c 6428  rd: str = Field(
-00002200: 2e2e 2e2c 2074 6974 6c65 3d27 e5af 86e7  ..., title='....
-00002210: a081 2729 0a0a 2020 2020 2320 e5a4 84e7  ..')..    # ....
-00002220: 9086 e8a1 a8e5 8d95 e68f 90e4 baa4 e695  ................
-00002230: b0e6 8dae 0a20 2020 2061 7379 6e63 2064  .....    async d
-00002240: 6566 2068 616e 646c 6528 7365 6c66 2c20  ef handle(self, 
-00002250: 7265 7175 6573 743a 2052 6571 7565 7374  request: Request
-00002260: 2c20 6461 7461 3a20 4261 7365 4d6f 6465  , data: BaseMode
-00002270: 6c2c 202a 2a6b 7761 7267 7329 202d 3e20  l, **kwargs) -> 
-00002280: 4261 7365 4170 694f 7574 5b41 6e79 5d3a  BaseApiOut[Any]:
-00002290: 0a20 2020 2020 2020 2069 6620 6461 7461  .        if data
-000022a0: 2e75 7365 726e 616d 6520 3d3d 2027 616d  .username == 'am
-000022b0: 6973 6164 6d69 6e27 2061 6e64 2064 6174  isadmin' and dat
-000022c0: 612e 7061 7373 776f 7264 203d 3d20 2761  a.password == 'a
-000022d0: 6d69 7361 646d 696e 273a 0a20 2020 2020  misadmin':.     
-000022e0: 2020 2020 2020 2072 6574 7572 6e20 4261         return Ba
-000022f0: 7365 4170 694f 7574 286d 7367 3d27 e799  seApiOut(msg='..
-00002300: bbe5 bd95 e688 90e5 8a9f 2127 2c20 6461  ..........!', da
-00002310: 7461 3d7b 2774 6f6b 656e 273a 2027 7878  ta={'token': 'xx
-00002320: 7878 7878 277d 290a 2020 2020 2020 2020  xxxx'}).        
-00002330: 7265 7475 726e 2042 6173 6541 7069 4f75  return BaseApiOu
-00002340: 7428 7374 6174 7573 3d2d 312c 206d 7367  t(status=-1, msg
-00002350: 3d27 e794 a8e6 88b7 e590 8de6 8896 e5af  ='..............
-00002360: 86e7 a081 e994 99e8 afaf 2127 290a 0a0a  ..........!')...
-00002370: 2320 e68c 82e8 bdbd e590 8ee5 8fb0 e7ae  # ..............
-00002380: a1e7 9086 e7b3 bbe7 bb9f 0a73 6974 652e  ...........site.
-00002390: 6d6f 756e 745f 6170 7028 6170 7029 0a0a  mount_app(app)..
-000023a0: 6966 205f 5f6e 616d 655f 5f20 3d3d 2027  if __name__ == '
-000023b0: 5f5f 6d61 696e 5f5f 273a 0a20 2020 2069  __main__':.    i
-000023c0: 6d70 6f72 7420 7576 6963 6f72 6e0a 0a20  mport uvicorn.. 
-000023d0: 2020 2075 7669 636f 726e 2e72 756e 2861     uvicorn.run(a
-000023e0: 7070 290a 6060 600a 0a23 2320 e4bd bfe7  pp).```..## ....
-000023f0: 94a8 e591 bde4 bba4 e8a1 8c0a 0a60 6060  .............```
-00002400: 6261 7368 0a23 20e5 ae89 e8a3 85e5 91bd  bash.# .........
-00002410: e4bb a4e8 a18c e68b 93e5 b195 0a70 6970  .............pip
-00002420: 2069 6e73 7461 6c6c 2066 6173 7461 7069   install fastapi
-00002430: 5f61 6d69 735f 6164 6d69 6e5b 636c 695d  _amis_admin[cli]
-00002440: 0a0a 2320 e69f a5e7 9c8b e5b8 aee5 8aa9  ..# ............
-00002450: 0a66 6161 202d 2d68 656c 700a 0a23 20e5  .faa --help..# .
-00002460: 889d e5a7 8be5 8c96 e4b8 80e4 b8aa 6046  ..............`F
-00002470: 6173 7441 5049 2d41 6d69 732d 4164 6d69  astAPI-Amis-Admi
-00002480: 6e60 e9a1 b9e7 9bae 0a66 6161 206e 6577  n`.......faa new
-00002490: 2070 726f 6a65 6374 5f6e 616d 6520 2d2d   project_name --
-000024a0: 696e 6974 0a0a 2320 e588 9de5 a78b e58c  init..# ........
-000024b0: 96e4 b880 e4b8 aa60 4661 7374 4150 492d  .......`FastAPI-
-000024c0: 416d 6973 2d41 646d 696e 60e5 ba94 e794  Amis-Admin`.....
-000024d0: a80a 6661 6120 6e65 7720 6170 705f 6e61  ..faa new app_na
-000024e0: 6d65 0a0a 2320 e5bf abe9 809f e8bf 90e8  me..# ..........
-000024f0: a18c e9a1 b9e7 9bae 0a66 6161 2072 756e  .........faa run
-00002500: 0a60 6060 0a0a 2323 20e7 958c e99d a2e9  .```..## .......
-00002510: a284 e8a7 880a 0a2d 204f 7065 6e20 6068  .......- Open `h
-00002520: 7474 703a 2f2f 3132 372e 302e 302e 313a  ttp://127.0.0.1:
-00002530: 3830 3030 2f61 646d 696e 2f60 2069 6e20  8000/admin/` in 
-00002540: 796f 7572 2062 726f 7773 6572 3a0a 0a21  your browser:..!
-00002550: 5b4d 6f64 656c 4164 6d69 6e5d 2868 7474  [ModelAdmin](htt
-00002560: 7073 3a2f 2f73 322e 6c6f 6c69 2e6e 6574  ps://s2.loli.net
-00002570: 2f32 3032 322f 3033 2f32 302f 4974 6746  /2022/03/20/ItgF
-00002580: 5947 554f 4e6d 316a 437a 352e 706e 6729  YGUONm1jCz5.png)
-00002590: 0a0a 2d20 4f70 656e 2060 6874 7470 3a2f  ..- Open `http:/
-000025a0: 2f31 3237 2e30 2e30 2e31 3a38 3030 302f  /127.0.0.1:8000/
-000025b0: 6164 6d69 6e2f 646f 6373 6020 696e 2079  admin/docs` in y
-000025c0: 6f75 7220 6272 6f77 7365 723a 0a0a 215b  our browser:..![
-000025d0: 446f 6373 5d28 6874 7470 733a 2f2f 7332  Docs](https://s2
-000025e0: 2e6c 6f6c 692e 6e65 742f 3230 3232 2f30  .loli.net/2022/0
-000025f0: 332f 3230 2f31 4763 4369 5064 6d58 6179  3/20/1GcCiPdmXay
-00002600: 7872 6248 2e70 6e67 290a 0a23 2320 e79b  xrbH.png)..## ..
-00002610: b8e5 85b3 e9a1 b9e7 9bae 0a0a 2d20 5b60  ............- [`
-00002620: 416d 6973 2d41 646d 696e 2d54 6865 6d65  Amis-Admin-Theme
-00002630: 2d45 6469 746f 7260 5d28 6874 7470 733a  -Editor`](https:
-00002640: 2f2f 6769 7468 7562 2e63 6f6d 2f73 7765  //github.com/swe
-00002650: 6c63 6b65 722f 616d 6973 2d61 646d 696e  lcker/amis-admin
-00002660: 2d74 6865 6d65 2d65 6469 746f 7229 3a60  -theme-editor):`
-00002670: 4661 7374 4150 492d 416d 6973 2d41 646d  FastAPI-Amis-Adm
-00002680: 696e 60e7 9a84 e4b8 bbe9 a298 e7bc 96e8  in`.............
-00002690: be91 e599 a8e3 8082 0a20 20e5 8581 e8ae  .........  .....
-000026a0: b8e6 b7bb e58a a0e8 87aa e5ae 9ae4 b989  ................
-000026b0: 6373 73e6 a0b7 e5bc 8fe5 928c e5ba 94e7  css.............
-000026c0: 94a8 e4b8 bbe9 a298 2ce5 8f98 e987 8fe6  ........,.......
-000026d0: 94b9 e58f 98e5 8f8a e697 b6e7 949f e695  ................
-000026e0: 882e 0a2d 205b 6046 6173 7441 5049 2d55  ...- [`FastAPI-U
-000026f0: 7365 722d 4175 7468 605d 2868 7474 7073  ser-Auth`](https
-00002700: 3a2f 2f67 6974 6875 622e 636f 6d2f 616d  ://github.com/am
-00002710: 6973 6164 6d69 6e2f 6661 7374 6170 695f  isadmin/fastapi_
-00002720: 7573 6572 5f61 7574 6829 3a20 e4b8 80e4  user_auth): ....
-00002730: b8aa e7ae 80e5 8d95 e880 8ce5 bcba e5a4  ................
-00002740: a7e7 9a84 6046 6173 7441 5049 60e7 94a8  ....`FastAPI`...
-00002750: e688 b760 5242 4143 60e8 aea4 e8af 81e4  ...`RBAC`.......
-00002760: b88e e68e 88e6 9d83 e5ba 932e 0a2d 205b  .............- [
-00002770: 6046 6173 7441 5049 2d53 6368 6564 756c  `FastAPI-Schedul
-00002780: 6572 605d 2868 7474 7073 3a2f 2f67 6974  er`](https://git
-00002790: 6875 622e 636f 6d2f 616d 6973 6164 6d69  hub.com/amisadmi
-000027a0: 6e2f 6661 7374 6170 695f 7363 6865 6475  n/fastapi_schedu
-000027b0: 6c65 7229 3a20 e4b8 80e4 b8aa e59f bae4  ler): ..........
-000027c0: ba8e 6041 5053 6368 6564 756c 6572 60e7  ..`APScheduler`.
-000027d0: 9a84 e7ae 80e5 8d95 e5ae 9ae6 97b6 e4bb  ................
-000027e0: bbe5 8aa1 e7ae a1e7 9086 6046 6173 7441  ..........`FastA
-000027f0: 5049 60e6 8b93 e5b1 95e5 ba93 2e0a 2d20  PI`...........- 
-00002800: 5b60 4661 7374 4150 492d 436f 6e66 6967  [`FastAPI-Config
-00002810: 605d 2868 7474 7073 3a2f 2f67 6974 6875  `](https://githu
-00002820: 622e 636f 6d2f 616d 6973 6164 6d69 6e2f  b.com/amisadmin/
-00002830: 6661 7374 6170 692d 636f 6e66 6967 293a  fastapi-config):
-00002840: 20e4 b880 e4b8 aae5 9fba e4ba 8e60 4661   ............`Fa
-00002850: 7374 4150 492d 416d 6973 2d41 646d 696e  stAPI-Amis-Admin
-00002860: 60e7 9a84 e58f afe8 a786 e58c 96e5 8aa8  `...............
-00002870: e680 81e9 858d e7bd aee7 aea1 e790 86e6  ................
-00002880: 8b93 e5b1 95e5 8c85 2e0a 2d20 5b60 4661  ..........- [`Fa
-00002890: 7374 4150 492d 416d 6973 2d41 646d 696e  stAPI-Amis-Admin
-000028a0: 2d44 656d 6f60 5d28 6874 7470 733a 2f2f  -Demo`](https://
-000028b0: 6769 7468 7562 2e63 6f6d 2f61 6d69 7361  github.com/amisa
-000028c0: 646d 696e 2f66 6173 7461 7069 5f61 6d69  dmin/fastapi_ami
-000028d0: 735f 6164 6d69 6e5f 6465 6d6f 293a 2020  s_admin_demo):  
-000028e0: e4b8 80e4 b8aa 6046 6173 7441 5049 2d41  ......`FastAPI-A
-000028f0: 6d69 732d 4164 6d69 6e60 20e5 ba94 e794  mis-Admin` .....
-00002900: a8e7 a88b e5ba 8fe7 a4ba e4be 8b2e 0a2d  ...............-
-00002910: 205b 6046 6173 7441 5049 2d55 7365 722d   [`FastAPI-User-
-00002920: 4175 7468 2d44 656d 6f60 5d28 6874 7470  Auth-Demo`](http
-00002930: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f61  s://github.com/a
-00002940: 6d69 7361 646d 696e 2f66 6173 7461 7069  misadmin/fastapi
-00002950: 5f75 7365 725f 6175 7468 5f64 656d 6f29  _user_auth_demo)
-00002960: 3a20 e4b8 80e4 b8aa 6046 6173 7441 5049  : ......`FastAPI
-00002970: 2d55 7365 722d 4175 7468 6020 e5ba 94e7  -User-Auth` ....
-00002980: 94a8 e7a8 8be5 ba8f e7a4 bae4 be8b 2e0a  ................
-00002990: 0a23 2320 e8ae b8e5 8faf e58d 8fe8 aeae  .## ............
-000029a0: 0a0a 2d20 6066 6173 7461 7069 2d61 6d69  ..- `fastapi-ami
-000029b0: 732d 6164 6d69 6e60 e59f bae4 ba8e 6041  s-admin`......`A
-000029c0: 7061 6368 6532 2e30 60e5 bc80 e6ba 90e5  pache2.0`.......
-000029d0: 858d e8b4 b9e4 bdbf e794 a8ef bc8c e58f  ................
-000029e0: afe4 bba5 e585 8de8 b4b9 e794 a8e4 ba8e  ................
-000029f0: e595 86e4 b89a e794 a8e9 8094 efbc 8ce4  ................
-00002a00: bd86 e8af b7e5 9ca8 e5b1 95e7 a4ba e795  ................
-00002a10: 8ce9 9da2 e4b8 ade6 988e e7a1 aee6 98be  ................
-00002a20: e7a4 bae5 85b3 e4ba 8e46 6173 7441 5049  .........FastAPI
-00002a30: 2d41 6d69 732d 4164 6d69 6ee7 9a84 e789  -Amis-Admin.....
-00002a40: 88e6 9d83 e4bf a1e6 81af 2e0a 0a23 2320  .............## 
-00002a50: e9b8 a3e8 b0a2 0a0a e684 9fe8 b0a2 e4bb  ................
-00002a60: a5e4 b88b e5bc 80e5 8f91 e880 85e5 afb9  ................
-00002a70: 2046 6173 7441 5049 2d41 6d69 732d 4164   FastAPI-Amis-Ad
-00002a80: 6d69 6e20 e4bd 9ce5 87ba e79a 84e8 b4a1  min ............
-00002a90: e78c aeef bc9a 0a0a 3c61 2068 7265 663d  ........<a href=
-00002aa0: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
-00002ab0: 636f 6d2f 616d 6973 6164 6d69 6e2f 6661  com/amisadmin/fa
-00002ac0: 7374 6170 695f 616d 6973 5f61 646d 696e  stapi_amis_admin
-00002ad0: 2f67 7261 7068 732f 636f 6e74 7269 6275  /graphs/contribu
-00002ae0: 746f 7273 223e 0a20 203c 696d 6720 7372  tors">.  <img sr
-00002af0: 633d 2268 7474 7073 3a2f 2f63 6f6e 7472  c="https://contr
-00002b00: 6962 2e72 6f63 6b73 2f69 6d61 6765 3f72  ib.rocks/image?r
-00002b10: 6570 6f3d 616d 6973 6164 6d69 6e2f 6661  epo=amisadmin/fa
-00002b20: 7374 6170 695f 616d 6973 5f61 646d 696e  stapi_amis_admin
-00002b30: 2220 2f3e 0a3c 2f61 3e0a                 " />.</a>.
+00000050: 452e 7a68 2e6d 6429 0d0a 7c20 5b45 6e67  E.zh.md)..| [Eng
+00000060: 6c69 7368 5d28 6874 7470 733a 2f2f 6769  lish](https://gi
+00000070: 7468 7562 2e63 6f6d 2f61 6d69 7361 646d  thub.com/amisadm
+00000080: 696e 2f66 6173 7461 7069 5f61 6d69 735f  in/fastapi_amis_
+00000090: 6164 6d69 6e29 0d0a 0d0a 2320 496e 7472  admin)....# Intr
+000000a0: 6f64 7563 7469 6f6e 0d0a 0d0a 3c68 3220  oduction....<h2 
+000000b0: 616c 6967 6e3d 2263 656e 7465 7222 3e0d  align="center">.
+000000c0: 0a20 2046 6173 7441 5049 2d41 6d69 732d  .  FastAPI-Amis-
+000000d0: 4164 6d69 6e0d 0a3c 2f68 323e 0d0a 3c70  Admin..</h2>..<p
+000000e0: 2061 6c69 676e 3d22 6365 6e74 6572 223e   align="center">
+000000f0: 0d0a 2020 2020 3c65 6d3e 6661 7374 6170  ..    <em>fastap
+00000100: 692d 616d 6973 2d61 646d 696e 2069 7320  i-amis-admin is 
+00000110: 6120 6869 6768 2d70 6572 666f 726d 616e  a high-performan
+00000120: 6365 2c20 6566 6669 6369 656e 7420 616e  ce, efficient an
+00000130: 6420 6561 7369 6c79 2065 7874 656e 7369  d easily extensi
+00000140: 626c 6520 4661 7374 4150 4920 6164 6d69  ble FastAPI admi
+00000150: 6e20 6672 616d 6577 6f72 6b2e 3c2f 656d  n framework.</em
+00000160: 3e3c 6272 2f3e 0d0a 2020 2020 3c65 6d3e  ><br/>..    <em>
+00000170: 496e 7370 6972 6564 2062 7920 446a 616e  Inspired by Djan
+00000180: 676f 2d61 646d 696e 2c20 616e 6420 6861  go-admin, and ha
+00000190: 7320 6173 206d 616e 7920 706f 7765 7266  s as many powerf
+000001a0: 756c 2066 756e 6374 696f 6e73 2061 7320  ul functions as 
+000001b0: 446a 616e 676f 2d61 646d 696e 2e3c 2f65  Django-admin.</e
+000001c0: 6d3e 0d0a 3c2f 703e 0d0a 3c70 2061 6c69  m>..</p>..<p ali
+000001d0: 676e 3d22 6365 6e74 6572 223e 0d0a 2020  gn="center">..  
+000001e0: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
+000001f0: 3a2f 2f67 6974 6875 622e 636f 6d2f 616d  ://github.com/am
+00000200: 6973 6164 6d69 6e2f 6661 7374 6170 695f  isadmin/fastapi_
+00000210: 616d 6973 5f61 646d 696e 2f61 6374 696f  amis_admin/actio
+00000220: 6e73 2f77 6f72 6b66 6c6f 7773 2f70 7974  ns/workflows/pyt
+00000230: 6573 742e 796d 6c22 2074 6172 6765 743d  est.yml" target=
+00000240: 225f 626c 616e 6b22 3e0d 0a20 2020 2020  "_blank">..     
+00000250: 2020 203c 696d 6720 7372 633d 2268 7474     <img src="htt
+00000260: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000270: 616d 6973 6164 6d69 6e2f 6661 7374 6170  amisadmin/fastap
+00000280: 695f 616d 6973 5f61 646d 696e 2f61 6374  i_amis_admin/act
+00000290: 696f 6e73 2f77 6f72 6b66 6c6f 7773 2f70  ions/workflows/p
+000002a0: 7974 6573 742e 796d 6c2f 6261 6467 652e  ytest.yml/badge.
+000002b0: 7376 6722 2061 6c74 3d22 5079 7465 7374  svg" alt="Pytest
+000002c0: 223e 0d0a 2020 2020 3c2f 613e 0d0a 2020  ">..    </a>..  
+000002d0: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
+000002e0: 3a2f 2f70 7970 692e 6f72 672f 7072 6f6a  ://pypi.org/proj
+000002f0: 6563 742f 6661 7374 6170 695f 616d 6973  ect/fastapi_amis
+00000300: 5f61 646d 696e 2220 7461 7267 6574 3d22  _admin" target="
+00000310: 5f62 6c61 6e6b 223e 0d0a 2020 2020 2020  _blank">..      
+00000320: 2020 3c69 6d67 2073 7263 3d22 6874 7470    <img src="http
+00000330: 733a 2f2f 6261 6467 656e 2e6e 6574 2f70  s://badgen.net/p
+00000340: 7970 692f 762f 6661 7374 6170 692d 616d  ypi/v/fastapi-am
+00000350: 6973 2d61 646d 696e 3f63 6f6c 6f72 3d62  is-admin?color=b
+00000360: 6c75 6522 2061 6c74 3d22 5061 636b 6167  lue" alt="Packag
+00000370: 6520 7665 7273 696f 6e22 3e0d 0a20 2020  e version">..   
+00000380: 203c 2f61 3e0d 0a20 2020 203c 6120 6872   </a>..    <a hr
+00000390: 6566 3d22 6874 7470 733a 2f2f 7065 7079  ef="https://pepy
+000003a0: 2e74 6563 682f 7072 6f6a 6563 742f 6661  .tech/project/fa
+000003b0: 7374 6170 692d 616d 6973 2d61 646d 696e  stapi-amis-admin
+000003c0: 2220 7461 7267 6574 3d22 5f62 6c61 6e6b  " target="_blank
+000003d0: 223e 0d0a 2020 2020 2020 2020 3c69 6d67  ">..        <img
+000003e0: 2073 7263 3d22 6874 7470 733a 2f2f 7065   src="https://pe
+000003f0: 7079 2e74 6563 682f 6261 6467 652f 6661  py.tech/badge/fa
+00000400: 7374 6170 692d 616d 6973 2d61 646d 696e  stapi-amis-admin
+00000410: 2220 616c 743d 2244 6f77 6e6c 6f61 6473  " alt="Downloads
+00000420: 223e 0d0a 2020 2020 3c2f 613e 0d0a 2020  ">..    </a>..  
+00000430: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
+00000440: 3a2f 2f67 6974 7465 722e 696d 2f61 6d69  ://gitter.im/ami
+00000450: 7361 646d 696e 2f66 6173 7461 7069 2d61  sadmin/fastapi-a
+00000460: 6d69 732d 6164 6d69 6e22 3e0d 0a20 2020  mis-admin">..   
+00000470: 2020 2020 203c 696d 6720 7372 633d 2268       <img src="h
+00000480: 7474 7073 3a2f 2f62 6164 6765 732e 6769  ttps://badges.gi
+00000490: 7474 6572 2e69 6d2f 616d 6973 6164 6d69  tter.im/amisadmi
+000004a0: 6e2f 6661 7374 6170 692d 616d 6973 2d61  n/fastapi-amis-a
+000004b0: 646d 696e 2e73 7667 2220 616c 743d 2243  dmin.svg" alt="C
+000004c0: 6861 7420 6f6e 2047 6974 7465 7222 2f3e  hat on Gitter"/>
+000004d0: 0d0a 2020 2020 3c2f 613e 0d0a 3c2f 703e  ..    </a>..</p>
+000004e0: 0d0a 3c70 2061 6c69 676e 3d22 6365 6e74  ..<p align="cent
+000004f0: 6572 223e 0d0a 2020 3c61 2068 7265 663d  er">..  <a href=
+00000500: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+00000510: 636f 6d2f 616d 6973 6164 6d69 6e2f 6661  com/amisadmin/fa
+00000520: 7374 6170 695f 616d 6973 5f61 646d 696e  stapi_amis_admin
+00000530: 2220 7461 7267 6574 3d22 5f62 6c61 6e6b  " target="_blank
+00000540: 223e 736f 7572 6365 2063 6f64 653c 2f61  ">source code</a
+00000550: 3e0d 0a20 20c2 b70d 0a20 203c 6120 6872  >..  ....  <a hr
+00000560: 6566 3d22 6874 7470 3a2f 2f64 656d 6f2e  ef="http://demo.
+00000570: 616d 6973 2e77 6f72 6b2f 6164 6d69 6e22  amis.work/admin"
+00000580: 2074 6172 6765 743d 225f 626c 616e 6b22   target="_blank"
+00000590: 3e6f 6e6c 696e 6520 6465 6d6f 3c2f 613e  >online demo</a>
+000005a0: 0d0a 2020 c2b7 0d0a 2020 3c61 2068 7265  ..  ....  <a hre
+000005b0: 663d 2268 7474 703a 2f2f 646f 6373 2e67  f="http://docs.g
+000005c0: 682e 616d 6973 2e77 6f72 6b22 2074 6172  h.amis.work" tar
+000005d0: 6765 743d 225f 626c 616e 6b22 3e64 6f63  get="_blank">doc
+000005e0: 756d 656e 7461 7469 6f6e 3c2f 613e 0d0a  umentation</a>..
+000005f0: 2020 c2b7 0d0a 2020 3c61 2068 7265 663d    ....  <a href=
+00000600: 2268 7474 703a 2f2f 646f 6373 2e61 6d69  "http://docs.ami
+00000610: 732e 776f 726b 2220 7461 7267 6574 3d22  s.work" target="
+00000620: 5f62 6c61 6e6b 223e 6361 6e27 7420 6f70  _blank">can't op
+00000630: 656e 2074 6865 2064 6f63 756d 656e 743f  en the document?
+00000640: 3c2f 613e 0d0a 3c2f 703e 0d0a 0d0a 0d0a  </a>..</p>......
+00000650: 2d2d 2d2d 2d2d 0d0a 0d0a 6066 6173 7461  ------....`fasta
+00000660: 7069 2d61 6d69 732d 6164 6d69 6e60 2069  pi-amis-admin` i
+00000670: 7320 6120 6869 6768 2d70 6572 666f 726d  s a high-perform
+00000680: 616e 6365 2061 6e64 2065 6666 6963 6965  ance and efficie
+00000690: 6e74 2066 7261 6d65 776f 726b 2062 6173  nt framework bas
+000006a0: 6564 206f 6e20 6066 6173 7461 7069 6020  ed on `fastapi` 
+000006b0: 2620 6061 6d69 7360 2077 6974 6820 6050  & `amis` with `P
+000006c0: 7974 686f 6e20 332e 372b 602c 2061 6e64  ython 3.7+`, and
+000006d0: 0d0a 6261 7365 6420 6f6e 2073 7461 6e64  ..based on stand
+000006e0: 6172 6420 5079 7468 6f6e 2074 7970 6520  ard Python type 
+000006f0: 6869 6e74 732e 2054 6865 206f 7269 6769  hints. The origi
+00000700: 6e61 6c20 696e 7465 6e74 696f 6e20 6f66  nal intention of
+00000710: 2074 6865 2064 6576 656c 6f70 6d65 6e74   the development
+00000720: 2069 7320 746f 2069 6d70 726f 7665 2074   is to improve t
+00000730: 6865 2061 7070 6c69 6361 7469 6f6e 2065  he application e
+00000740: 636f 6c6f 6779 2061 6e64 0d0a 746f 2071  cology and..to q
+00000750: 7569 636b 6c79 2067 656e 6572 6174 6520  uickly generate 
+00000760: 6120 7669 7375 616c 2064 6173 6862 6f61  a visual dashboa
+00000770: 7264 2066 6f72 2074 6865 2077 6562 2061  rd for the web a
+00000780: 7070 6c69 6361 7469 6f6e 202e 2041 6363  pplication . Acc
+00000790: 6f72 6469 6e67 2074 6f20 7468 6520 6041  ording to the `A
+000007a0: 7061 6368 6532 2e30 6020 7072 6f74 6f63  pache2.0` protoc
+000007b0: 6f6c 2c20 6974 2069 7320 6672 6565 2061  ol, it is free a
+000007c0: 6e64 0d0a 6f70 656e 2073 6f75 7263 6520  nd..open source 
+000007d0: 2e20 4275 7420 696e 206f 7264 6572 2074  . But in order t
+000007e0: 6f20 6265 7474 6572 206f 7065 7261 7465  o better operate
+000007f0: 2061 6e64 206d 6169 6e74 6169 6e20 7468   and maintain th
+00000800: 6973 2070 726f 6a65 6374 2069 6e20 7468  is project in th
+00000810: 6520 6c6f 6e67 2072 756e 2c20 4920 7665  e long run, I ve
+00000820: 7279 206d 7563 6820 686f 7065 2074 6f20  ry much hope to 
+00000830: 6765 740d 0a65 7665 7279 6f6e 6527 7320  get..everyone's 
+00000840: 7370 6f6e 736f 7273 6869 7020 616e 6420  sponsorship and 
+00000850: 7375 7070 6f72 742e 0d0a 0d0a 2323 2046  support.....## F
+00000860: 6561 7475 7265 730d 0a0d 0a2d 202a 2a48  eatures....- **H
+00000870: 6967 6820 7065 7266 6f72 6d61 6e63 652a  igh performance*
+00000880: 2a3a 2042 6173 6564 206f 6e20 5b46 6173  *: Based on [Fas
+00000890: 7441 5049 5d28 6874 7470 733a 2f2f 6661  tAPI](https://fa
+000008a0: 7374 6170 692e 7469 616e 676f 6c6f 2e63  stapi.tiangolo.c
+000008b0: 6f6d 2f29 2e20 456e 6a6f 7920 616c 6c20  om/). Enjoy all 
+000008c0: 7468 6520 6265 6e65 6669 7473 2e0d 0a2d  the benefits...-
+000008d0: 202a 2a48 6967 6820 6566 6669 6369 656e   **High efficien
+000008e0: 6379 2a2a 3a20 5065 7266 6563 7420 636f  cy**: Perfect co
+000008f0: 6465 2074 7970 6520 6869 6e74 732e 2048  de type hints. H
+00000900: 6967 6865 7220 636f 6465 2072 6575 7361  igher code reusa
+00000910: 6269 6c69 7479 2e0d 0a2d 202a 2a53 7570  bility...- **Sup
+00000920: 706f 7274 2061 7379 6e63 6872 6f6e 6f75  port asynchronou
+00000930: 7320 616e 6420 7379 6e63 6872 6f6e 6f75  s and synchronou
+00000940: 7320 6879 6272 6964 2077 7269 7469 6e67  s hybrid writing
+00000950: 2a2a 3a20 604f 524d 6020 2069 7320 6261  **: `ORM`  is ba
+00000960: 7365 6420 6f6e 6053 514c 4d6f 6465 6c60  sed on`SQLModel`
+00000970: 2026 2060 5371 6c61 6c63 6865 6d79 602e   & `Sqlalchemy`.
+00000980: 2046 7265 656c 7920 6375 7374 6f6d 697a   Freely customiz
+00000990: 650d 0a20 2064 6174 6162 6173 6520 7479  e..  database ty
+000009a0: 7065 2e20 5375 7070 6f72 7420 7379 6e63  pe. Support sync
+000009b0: 6872 6f6e 6f75 7320 616e 6420 6173 796e  hronous and asyn
+000009c0: 6368 726f 6e6f 7573 206d 6f64 652e 2053  chronous mode. S
+000009d0: 7472 6f6e 6720 7363 616c 6162 696c 6974  trong scalabilit
+000009e0: 792e 0d0a 2d20 2a2a 4672 6f6e 742d 656e  y...- **Front-en
+000009f0: 6420 7365 7061 7261 7469 6f6e 2a2a 3a20  d separation**: 
+00000a00: 5468 6520 6672 6f6e 742d 656e 6420 6973  The front-end is
+00000a10: 2072 656e 6465 7265 6420 6279 2060 416d   rendered by `Am
+00000a20: 6973 602c 2074 6865 2062 6163 6b2d 656e  is`, the back-en
+00000a30: 6420 696e 7465 7266 6163 6520 6973 2061  d interface is a
+00000a40: 7574 6f6d 6174 6963 616c 6c79 2067 656e  utomatically gen
+00000a50: 6572 6174 6564 0d0a 2020 6279 2060 6661  erated..  by `fa
+00000a60: 7374 6170 692d 616d 6973 2d61 646d 696e  stapi-amis-admin
+00000a70: 602e 2054 6865 2069 6e74 6572 6661 6365  `. The interface
+00000a80: 2069 7320 7265 7573 6162 6c65 2e0d 0a2d   is reusable...-
+00000a90: 202a 2a53 7472 6f6e 6720 7363 616c 6162   **Strong scalab
+00000aa0: 696c 6974 792a 2a3a 2054 6865 2062 6163  ility**: The bac
+00000ab0: 6b67 726f 756e 6420 7061 6765 2073 7570  kground page sup
+00000ac0: 706f 7274 7320 6041 6d69 7360 2070 6167  ports `Amis` pag
+00000ad0: 6573 2061 6e64 206f 7264 696e 6172 7920  es and ordinary 
+00000ae0: 6068 746d 6c60 2070 6167 6573 2e20 4561  `html` pages. Ea
+00000af0: 7369 6c79 2063 7573 746f 6d69 7a65 2074  sily customize t
+00000b00: 6865 0d0a 2020 696e 7465 7266 6163 6520  he..  interface 
+00000b10: 6672 6565 6c79 2e0d 0a2d 202a 2a41 7574  freely...- **Aut
+00000b20: 6f6d 6174 6963 2061 7069 2064 6f63 756d  omatic api docum
+00000b30: 656e 7461 7469 6f6e 2a2a 3a20 4175 746f  entation**: Auto
+00000b40: 6d61 7469 6361 6c6c 7920 6765 6e65 7261  matically genera
+00000b50: 7465 2049 6e74 6572 6661 6365 2064 6f63  te Interface doc
+00000b60: 756d 656e 7461 7469 6f6e 2062 7920 6046  umentation by `F
+00000b70: 6173 7441 5049 602e 2045 6173 696c 7920  astAPI`. Easily 
+00000b80: 6465 6275 6720 616e 6420 7368 6172 650d  debug and share.
+00000b90: 0a20 2069 6e74 6572 6661 6365 732e 0d0a  .  interfaces...
+00000ba0: 0d0a 2323 2044 6570 656e 6465 6e63 6965  ..## Dependencie
+00000bb0: 730d 0a0d 0a2d 205b 4661 7374 4150 495d  s....- [FastAPI]
+00000bc0: 2868 7474 7073 3a2f 2f66 6173 7461 7069  (https://fastapi
+00000bd0: 2e74 6961 6e67 6f6c 6f2e 636f 6d2f 293a  .tiangolo.com/):
+00000be0: 2046 696e 6973 6820 7468 6520 7765 6220   Finish the web 
+00000bf0: 7061 7274 2e0d 0a2d 205b 5351 4c4d 6f64  part...- [SQLMod
+00000c00: 656c 5d28 6874 7470 733a 2f2f 7371 6c6d  el](https://sqlm
+00000c10: 6f64 656c 2e74 6961 6e67 6f6c 6f2e 636f  odel.tiangolo.co
+00000c20: 6d2f 293a 2046 696e 6973 6820 604f 524d  m/): Finish `ORM
+00000c30: 6020 6d6f 6465 6c20 6d61 7070 696e 672e  ` model mapping.
+00000c40: 2050 6572 6665 6374 6c79 0d0a 2020 636f   Perfectly..  co
+00000c50: 6d62 696e 6520 205b 5351 4c41 6c63 6865  mbine  [SQLAlche
+00000c60: 6d79 5d28 6874 7470 733a 2f2f 7777 772e  my](https://www.
+00000c70: 7371 6c61 6c63 6865 6d79 2e6f 7267 2f29  sqlalchemy.org/)
+00000c80: 2077 6974 6820 5b50 7964 616e 7469 635d   with [Pydantic]
+00000c90: 2868 7474 7073 3a2f 2f70 7964 616e 7469  (https://pydanti
+00000ca0: 632d 646f 6373 2e68 656c 706d 616e 7561  c-docs.helpmanua
+00000cb0: 6c2e 696f 2f29 2c20 616e 6420 6861 7665  l.io/), and have
+00000cc0: 2061 6c6c 0d0a 2020 7468 6569 7220 6665   all..  their fe
+00000cd0: 6174 7572 6573 202e 0d0a 2d20 5b41 6d69  atures ...- [Ami
+00000ce0: 735d 2868 7474 7073 3a2f 2f62 6169 6475  s](https://baidu
+00000cf0: 2e67 6974 6565 2e69 6f2f 616d 6973 293a  .gitee.io/amis):
+00000d00: 2046 696e 6973 6820 6164 6d69 6e20 7061   Finish admin pa
+00000d10: 6765 2070 7265 7365 6e74 6174 696f 6e2e  ge presentation.
+00000d20: 0d0a 0d0a 2323 2043 6f6d 706f 7369 7469  ....## Compositi
+00000d30: 6f6e 0d0a 0d0a 6066 6173 7461 7069 2d61  on....`fastapi-a
+00000d40: 6d69 732d 6164 6d69 6e60 2063 6f6e 7369  mis-admin` consi
+00000d50: 7374 7320 6f66 2074 6872 6565 2063 6f72  sts of three cor
+00000d60: 6520 6d6f 6475 6c65 732c 206f 6620 7768  e modules, of wh
+00000d70: 6963 682c 2060 616d 6973 602c 2060 6372  ich, `amis`, `cr
+00000d80: 7564 6020 6361 6e20 6265 2075 7365 6420  ud` can be used 
+00000d90: 6173 2073 6570 6172 6174 650d 0a6d 6f64  as separate..mod
+00000da0: 756c 6573 2c20 6061 646d 696e 6020 6973  ules, `admin` is
+00000db0: 2064 6576 656c 6f70 6564 2062 7920 7468   developed by th
+00000dc0: 6520 666f 726d 6572 2e0d 0a0d 0a2d 2060  e former.....- `
+00000dd0: 616d 6973 603a 2042 6173 6564 206f 6e20  amis`: Based on 
+00000de0: 7468 6520 6070 7964 616e 7469 6360 2064  the `pydantic` d
+00000df0: 6174 6120 6d6f 6465 6c20 6275 696c 6469  ata model buildi
+00000e00: 6e67 206c 6962 7261 7279 206f 6620 6062  ng library of `b
+00000e10: 6169 6475 2061 6d69 7360 2e20 546f 2067  aidu amis`. To g
+00000e20: 656e 6572 6174 652f 7061 7273 6520 6461  enerate/parse da
+00000e30: 7461 2072 6170 6964 6c79 2e0d 0a2d 2060  ta rapidly...- `
+00000e40: 6372 7564 603a 2042 6173 6564 206f 6e20  crud`: Based on 
+00000e50: 6046 6173 7441 5049 6020 2660 5371 6c61  `FastAPI` &`Sqla
+00000e60: 6c63 6865 6d79 602e 2054 6f20 7175 6963  lchemy`. To quic
+00000e70: 6b6c 7920 6275 696c 6420 4372 6561 7465  kly build Create
+00000e80: 2c20 5265 6164 2c20 5570 6461 7465 2c20  , Read, Update, 
+00000e90: 4465 6c65 7465 2063 6f6d 6d6f 6e20 4150  Delete common AP
+00000ea0: 490d 0a20 2069 6e74 6572 6661 6365 202e  I..  interface .
+00000eb0: 0d0a 2d20 6061 646d 696e 603a 2049 6e73  ..- `admin`: Ins
+00000ec0: 7069 7265 6420 6279 2060 446a 616e 676f  pired by `Django
+00000ed0: 2d41 646d 696e 602e 2043 6f6d 6269 6e65  -Admin`. Combine
+00000ee0: 2060 616d 6973 6020 7769 7468 2060 6372   `amis` with `cr
+00000ef0: 7564 602e 2054 6f20 7175 6963 6b6c 7920  ud`. To quickly 
+00000f00: 6275 696c 6420 5765 6220 4164 6d69 6e0d  build Web Admin.
+00000f10: 0a20 2064 6173 6862 6f61 7264 202e 0d0a  .  dashboard ...
+00000f20: 0d0a 2323 2049 6e73 7461 6c6c 6174 696f  ..## Installatio
+00000f30: 6e0d 0a0d 0a60 6060 6261 7368 0d0a 7069  n....```bash..pi
+00000f40: 7020 696e 7374 616c 6c20 6661 7374 6170  p install fastap
+00000f50: 695f 616d 6973 5f61 646d 696e 0d0a 6060  i_amis_admin..``
+00000f60: 600d 0a0d 0a23 2323 204e 6f74 650d 0a0d  `....### Note...
+00000f70: 0a2d 2060 7371 6c6d 6f64 656c 6020 6375  .- `sqlmodel` cu
+00000f80: 7272 656e 746c 7920 646f 6573 206e 6f74  rrently does not
+00000f90: 2073 7570 706f 7274 2060 7371 6c61 6c63   support `sqlalc
+00000fa0: 6865 6d79 2032 2e30 2b60 2e20 4966 2079  hemy 2.0+`. If y
+00000fb0: 6f75 2075 7365 2060 7371 6c61 6c63 6865  ou use `sqlalche
+00000fc0: 6d79 2032 2e30 2b60 2074 6f20 6372 6561  my 2.0+` to crea
+00000fd0: 7465 2061 206d 6f64 656c 2c20 796f 7520  te a model, you 
+00000fe0: 6361 6e6e 6f74 0d0a 2020 7573 6520 6073  cannot..  use `s
+00000ff0: 716c 6d6f 6465 6c60 2061 7420 7468 6520  qlmodel` at the 
+00001000: 7361 6d65 2074 696d 652e 0d0a 2d20 4166  same time...- Af
+00001010: 7465 7220 7665 7273 696f 6e20 6066 6173  ter version `fas
+00001020: 7461 7069 2d61 6d69 732d 6164 6d69 6e3e  tapi-amis-admin>
+00001030: 3d30 2e36 2e30 602c 2060 7371 6c6d 6f64  =0.6.0`, `sqlmod
+00001040: 656c 6020 6973 206e 6f20 6c6f 6e67 6572  el` is no longer
+00001050: 2061 2072 6571 7569 7265 6420 6465 7065   a required depe
+00001060: 6e64 656e 6379 206c 6962 7261 7279 2e20  ndency library. 
+00001070: 4966 2079 6f75 2075 7365 2060 7371 6c6d  If you use `sqlm
+00001080: 6f64 656c 600d 0a20 2074 6f20 6372 6561  odel`..  to crea
+00001090: 7465 2061 206d 6f64 656c 2c20 796f 7520  te a model, you 
+000010a0: 6361 6e20 696e 7374 616c 6c20 6974 2077  can install it w
+000010b0: 6974 6820 7468 6520 666f 6c6c 6f77 696e  ith the followin
+000010c0: 6720 636f 6d6d 616e 642e 0d0a 0d0a 6060  g command.....``
+000010d0: 6062 6173 680d 0a70 6970 2069 6e73 7461  `bash..pip insta
+000010e0: 6c6c 2066 6173 7461 7069 5f61 6d69 735f  ll fastapi_amis_
+000010f0: 6164 6d69 6e5b 7371 6c6d 6f64 656c 5d0d  admin[sqlmodel].
+00001100: 0a60 6060 0d0a 0d0a 2323 2053 696d 706c  .```....## Simpl
+00001110: 6520 4578 616d 706c 650d 0a0d 0a60 6060  e Example....```
+00001120: 7079 7468 6f6e 0d0a 6672 6f6d 2066 6173  python..from fas
+00001130: 7461 7069 2069 6d70 6f72 7420 4661 7374  tapi import Fast
+00001140: 4150 490d 0a66 726f 6d20 6661 7374 6170  API..from fastap
+00001150: 695f 616d 6973 5f61 646d 696e 2e61 646d  i_amis_admin.adm
+00001160: 696e 2e73 6574 7469 6e67 7320 696d 706f  in.settings impo
+00001170: 7274 2053 6574 7469 6e67 730d 0a66 726f  rt Settings..fro
+00001180: 6d20 6661 7374 6170 695f 616d 6973 5f61  m fastapi_amis_a
+00001190: 646d 696e 2e61 646d 696e 2e73 6974 6520  dmin.admin.site 
+000011a0: 696d 706f 7274 2041 646d 696e 5369 7465  import AdminSite
+000011b0: 0d0a 0d0a 2320 6372 6561 7465 2046 6173  ....# create Fas
+000011c0: 7441 5049 2061 7070 6c69 6361 7469 6f6e  tAPI application
+000011d0: 0d0a 6170 7020 3d20 4661 7374 4150 4928  ..app = FastAPI(
+000011e0: 290d 0a0d 0a23 2063 7265 6174 6520 4164  )....# create Ad
+000011f0: 6d69 6e53 6974 6520 696e 7374 616e 6365  minSite instance
+00001200: 0d0a 7369 7465 203d 2041 646d 696e 5369  ..site = AdminSi
+00001210: 7465 2873 6574 7469 6e67 733d 5365 7474  te(settings=Sett
+00001220: 696e 6773 2864 6174 6162 6173 655f 7572  ings(database_ur
+00001230: 6c5f 6173 796e 633d 2773 716c 6974 652b  l_async='sqlite+
+00001240: 6169 6f73 716c 6974 653a 2f2f 2f61 6d69  aiosqlite:///ami
+00001250: 7361 646d 696e 2e64 6227 2929 0d0a 0d0a  sadmin.db'))....
+00001260: 2320 6d6f 756e 7420 4164 6d69 6e53 6974  # mount AdminSit
+00001270: 6520 696e 7374 616e 6365 0d0a 7369 7465  e instance..site
+00001280: 2e6d 6f75 6e74 5f61 7070 2861 7070 290d  .mount_app(app).
+00001290: 0a0d 0a69 6620 5f5f 6e61 6d65 5f5f 203d  ...if __name__ =
+000012a0: 3d20 275f 5f6d 6169 6e5f 5f27 3a0d 0a20  = '__main__':.. 
+000012b0: 2020 2069 6d70 6f72 7420 7576 6963 6f72     import uvicor
+000012c0: 6e0d 0a0d 0a20 2020 2075 7669 636f 726e  n....    uvicorn
+000012d0: 2e72 756e 2861 7070 290d 0a60 6060 0d0a  .run(app)..```..
+000012e0: 0d0a 2323 204d 6f64 656c 4164 6d69 6e20  ..## ModelAdmin 
+000012f0: 4578 616d 706c 650d 0a0d 0a23 2323 2043  Example....### C
+00001300: 7265 6174 6520 4d6f 6465 6c0d 0a0d 0a2d  reate Model....-
+00001310: 2053 7570 706f 7274 2060 5351 4c4d 6f64   Support `SQLMod
+00001320: 656c 6020 6d6f 6465 6c2c 2060 5351 4c41  el` model, `SQLA
+00001330: 6c63 6865 6d79 6020 6d6f 6465 6c2c 2060  lchemy` model, `
+00001340: 5351 4c41 6c63 6865 6d79 2032 2e30 6020  SQLAlchemy 2.0` 
+00001350: 6d6f 6465 6c0d 0a2d 204d 6574 686f 6420  model..- Method 
+00001360: 313a 2043 7265 6174 6520 6d6f 6465 6c20  1: Create model 
+00001370: 7468 726f 7567 6820 6053 514c 4d6f 6465  through `SQLMode
+00001380: 6c60 2e0d 0a0d 0a60 6060 7079 7468 6f6e  l`.....```python
+00001390: 0d0a 6672 6f6d 2073 716c 6d6f 6465 6c20  ..from sqlmodel 
+000013a0: 696d 706f 7274 2053 514c 4d6f 6465 6c0d  import SQLModel.
+000013b0: 0a66 726f 6d20 6661 7374 6170 695f 616d  .from fastapi_am
+000013c0: 6973 5f61 646d 696e 2e6d 6f64 656c 732e  is_admin.models.
+000013d0: 6669 656c 6473 2069 6d70 6f72 7420 4669  fields import Fi
+000013e0: 656c 640d 0a0d 0a0d 0a63 6c61 7373 2042  eld......class B
+000013f0: 6173 6528 5351 4c4d 6f64 656c 293a 0d0a  ase(SQLModel):..
+00001400: 2020 2020 7061 7373 0d0a 0d0a 0d0a 2320      pass......# 
+00001410: 4372 6561 7465 2061 6e20 5351 4c4d 6f64  Create an SQLMod
+00001420: 656c 2c20 7365 6520 646f 6375 6d65 6e74  el, see document
+00001430: 2066 6f72 2064 6574 6169 6c73 3a20 6874   for details: ht
+00001440: 7470 733a 2f2f 7371 6c6d 6f64 656c 2e74  tps://sqlmodel.t
+00001450: 6961 6e67 6f6c 6f2e 636f 6d2f 0d0a 636c  iangolo.com/..cl
+00001460: 6173 7320 4361 7465 676f 7279 2853 514c  ass Category(SQL
+00001470: 4d6f 6465 6c2c 2074 6162 6c65 3d54 7275  Model, table=Tru
+00001480: 6529 3a0d 0a20 2020 2069 643a 2069 6e74  e):..    id: int
+00001490: 203d 2046 6965 6c64 2864 6566 6175 6c74   = Field(default
+000014a0: 3d4e 6f6e 652c 2070 7269 6d61 7279 5f6b  =None, primary_k
+000014b0: 6579 3d54 7275 652c 206e 756c 6c61 626c  ey=True, nullabl
+000014c0: 653d 4661 6c73 6529 0d0a 2020 2020 6e61  e=False)..    na
+000014d0: 6d65 3a20 7374 7220 3d20 4669 656c 6428  me: str = Field(
+000014e0: 7469 746c 653d 2743 6174 6567 6f72 794e  title='CategoryN
+000014f0: 616d 6527 2c20 6d61 785f 6c65 6e67 7468  ame', max_length
+00001500: 3d31 3030 2c20 756e 6971 7565 3d54 7275  =100, unique=Tru
+00001510: 652c 2069 6e64 6578 3d54 7275 652c 206e  e, index=True, n
+00001520: 756c 6c61 626c 653d 4661 6c73 6529 0d0a  ullable=False)..
+00001530: 2020 2020 6465 7363 7269 7074 696f 6e3a      description:
+00001540: 2073 7472 203d 2046 6965 6c64 2864 6566   str = Field(def
+00001550: 6175 6c74 3d27 272c 2074 6974 6c65 3d27  ault='', title='
+00001560: 4465 7363 7269 7074 696f 6e27 2c20 6d61  Description', ma
+00001570: 785f 6c65 6e67 7468 3d32 3535 290d 0a0d  x_length=255)...
+00001580: 0a60 6060 0d0a 0d0a 2d20 4d65 7468 6f64  .```....- Method
+00001590: 2032 3a20 4372 6561 7465 206d 6f64 656c   2: Create model
+000015a0: 2074 6872 6f75 6768 2060 5351 4c41 6c63   through `SQLAlc
+000015b0: 6865 6d79 602e 0d0a 0d0a 6060 6070 7974  hemy`.....```pyt
+000015c0: 686f 6e0d 0a66 726f 6d20 7371 6c61 6c63  hon..from sqlalc
+000015d0: 6865 6d79 2069 6d70 6f72 7420 436f 6c75  hemy import Colu
+000015e0: 6d6e 2c20 496e 7465 6765 722c 2053 7472  mn, Integer, Str
+000015f0: 696e 670d 0a66 726f 6d20 7371 6c61 6c63  ing..from sqlalc
+00001600: 6865 6d79 2e65 7874 2e64 6563 6c61 7261  hemy.ext.declara
+00001610: 7469 7665 2069 6d70 6f72 7420 6465 636c  tive import decl
+00001620: 6172 6174 6976 655f 6261 7365 0d0a 0d0a  arative_base....
+00001630: 4261 7365 203d 2064 6563 6c61 7261 7469  Base = declarati
+00001640: 7665 5f62 6173 6528 290d 0a0d 0a0d 0a23  ve_base()......#
+00001650: 2043 7265 6174 6520 616e 2053 514c 416c   Create an SQLAl
+00001660: 6368 656d 7920 6d6f 6465 6c2c 2073 6565  chemy model, see
+00001670: 2064 6f63 756d 656e 7420 666f 7220 6465   document for de
+00001680: 7461 696c 733a 2068 7474 7073 3a2f 2f64  tails: https://d
+00001690: 6f63 732e 7371 6c61 6c63 6865 6d79 2e6f  ocs.sqlalchemy.o
+000016a0: 7267 2f65 6e2f 3134 2f6f 726d 2f74 7574  rg/en/14/orm/tut
+000016b0: 6f72 6961 6c2e 6874 6d6c 0d0a 636c 6173  orial.html..clas
+000016c0: 7320 4361 7465 676f 7279 2842 6173 6529  s Category(Base)
+000016d0: 3a0d 0a20 2020 205f 5f74 6162 6c65 6e61  :..    __tablena
+000016e0: 6d65 5f5f 203d 2027 6361 7465 676f 7279  me__ = 'category
+000016f0: 270d 0a20 2020 2023 2053 7065 6369 6679  '..    # Specify
+00001700: 2074 6865 2053 6368 656d 6120 636c 6173   the Schema clas
+00001710: 7320 636f 7272 6573 706f 6e64 696e 6720  s corresponding 
+00001720: 746f 2074 6865 206d 6f64 656c 2e20 4974  to the model. It
+00001730: 2069 7320 7265 636f 6d6d 656e 6465 6420   is recommended 
+00001740: 746f 2073 7065 6369 6679 2069 742e 2049  to specify it. I
+00001750: 6620 6f6d 6974 7465 642c 2069 7420 6361  f omitted, it ca
+00001760: 6e20 6265 2061 7574 6f6d 6174 6963 616c  n be automatical
+00001770: 6c79 2067 656e 6572 6174 6564 2e0d 0a20  ly generated... 
+00001780: 2020 205f 5f70 7964 616e 7469 635f 6d6f     __pydantic_mo
+00001790: 6465 6c5f 5f20 3d20 4361 7465 676f 7279  del__ = Category
+000017a0: 5363 6865 6d61 0d0a 0d0a 2020 2020 6964  Schema....    id
+000017b0: 203d 2043 6f6c 756d 6e28 496e 7465 6765   = Column(Intege
+000017c0: 722c 2070 7269 6d61 7279 5f6b 6579 3d54  r, primary_key=T
+000017d0: 7275 652c 206e 756c 6c61 626c 653d 4661  rue, nullable=Fa
+000017e0: 6c73 6529 0d0a 2020 2020 6e61 6d65 203d  lse)..    name =
+000017f0: 2043 6f6c 756d 6e28 5374 7269 6e67 2831   Column(String(1
+00001800: 3030 292c 2075 6e69 7175 653d 5472 7565  00), unique=True
+00001810: 2c20 696e 6465 783d 5472 7565 2c20 6e75  , index=True, nu
+00001820: 6c6c 6162 6c65 3d46 616c 7365 290d 0a20  llable=False).. 
+00001830: 2020 2064 6573 6372 6970 7469 6f6e 203d     description =
+00001840: 2043 6f6c 756d 6e28 5374 7269 6e67 2832   Column(String(2
+00001850: 3535 292c 2064 6566 6175 6c74 3d27 2729  55), default='')
+00001860: 0d0a 6060 600d 0a0d 0a2d 204d 6574 686f  ..```....- Metho
+00001870: 6420 333a 2043 7265 6174 6520 6d6f 6465  d 3: Create mode
+00001880: 6c20 7468 726f 7567 6820 6053 514c 416c  l through `SQLAl
+00001890: 6368 656d 7920 322e 3060 2e0d 0a0d 0a60  chemy 2.0`.....`
+000018a0: 6060 7079 7468 6f6e 0d0a 6672 6f6d 2073  ``python..from s
+000018b0: 716c 616c 6368 656d 7920 696d 706f 7274  qlalchemy import
+000018c0: 2053 7472 696e 670d 0a66 726f 6d20 7371   String..from sq
+000018d0: 6c61 6c63 6865 6d79 2e6f 726d 2069 6d70  lalchemy.orm imp
+000018e0: 6f72 7420 4465 636c 6172 6174 6976 6542  ort DeclarativeB
+000018f0: 6173 652c 204d 6170 7065 642c 206d 6170  ase, Mapped, map
+00001900: 7065 645f 636f 6c75 6d6e 0d0a 0d0a 0d0a  ped_column......
+00001910: 636c 6173 7320 4261 7365 2844 6563 6c61  class Base(Decla
+00001920: 7261 7469 7665 4261 7365 293a 0d0a 2020  rativeBase):..  
+00001930: 2020 7061 7373 0d0a 0d0a 0d0a 2320 4372    pass......# Cr
+00001940: 6561 7465 2061 6e20 5351 4c41 6c63 6865  eate an SQLAlche
+00001950: 6d79 2032 2e30 206d 6f64 656c 2c20 7365  my 2.0 model, se
+00001960: 6520 646f 6375 6d65 6e74 2066 6f72 2064  e document for d
+00001970: 6574 6169 6c73 3a20 6874 7470 733a 2f2f  etails: https://
+00001980: 646f 6373 2e73 716c 616c 6368 656d 792e  docs.sqlalchemy.
+00001990: 6f72 672f 656e 2f32 302f 6f72 6d2f 7175  org/en/20/orm/qu
+000019a0: 6963 6b73 7461 7274 2e68 746d 6c0d 0a63  ickstart.html..c
+000019b0: 6c61 7373 2043 6174 6567 6f72 7928 4261  lass Category(Ba
+000019c0: 7365 293a 0d0a 2020 2020 5f5f 7461 626c  se):..    __tabl
+000019d0: 656e 616d 655f 5f20 3d20 2263 6174 6567  ename__ = "categ
+000019e0: 6f72 7922 0d0a 2020 2020 2320 5370 6563  ory"..    # Spec
+000019f0: 6966 7920 7468 6520 5363 6865 6d61 2063  ify the Schema c
+00001a00: 6c61 7373 2063 6f72 7265 7370 6f6e 6469  lass correspondi
+00001a10: 6e67 2074 6f20 7468 6520 6d6f 6465 6c2e  ng to the model.
+00001a20: 2049 7420 6973 2072 6563 6f6d 6d65 6e64   It is recommend
+00001a30: 6564 2074 6f20 7370 6563 6966 7920 6974  ed to specify it
+00001a40: 2e20 4966 206f 6d69 7474 6564 2c20 6974  . If omitted, it
+00001a50: 2063 616e 2062 6520 6175 746f 6d61 7469   can be automati
+00001a60: 6361 6c6c 7920 6765 6e65 7261 7465 642e  cally generated.
+00001a70: 0d0a 2020 2020 5f5f 7079 6461 6e74 6963  ..    __pydantic
+00001a80: 5f6d 6f64 656c 5f5f 203d 2043 6174 6567  _model__ = Categ
+00001a90: 6f72 7953 6368 656d 610d 0a0d 0a20 2020  orySchema....   
+00001aa0: 2069 643a 204d 6170 7065 645b 696e 745d   id: Mapped[int]
+00001ab0: 203d 206d 6170 7065 645f 636f 6c75 6d6e   = mapped_column
+00001ac0: 2870 7269 6d61 7279 5f6b 6579 3d54 7275  (primary_key=Tru
+00001ad0: 652c 206e 756c 6c61 626c 653d 4661 6c73  e, nullable=Fals
+00001ae0: 6529 0d0a 2020 2020 6e61 6d65 3a20 4d61  e)..    name: Ma
+00001af0: 7070 6564 5b73 7472 5d20 3d20 6d61 7070  pped[str] = mapp
+00001b00: 6564 5f63 6f6c 756d 6e28 5374 7269 6e67  ed_column(String
+00001b10: 2831 3030 292c 2075 6e69 7175 653d 5472  (100), unique=Tr
+00001b20: 7565 2c20 696e 6465 783d 5472 7565 2c20  ue, index=True, 
+00001b30: 6e75 6c6c 6162 6c65 3d46 616c 7365 290d  nullable=False).
+00001b40: 0a20 2020 2064 6573 6372 6970 7469 6f6e  .    description
+00001b50: 3a20 4d61 7070 6564 5b73 7472 5d20 3d20  : Mapped[str] = 
+00001b60: 6d61 7070 6564 5f63 6f6c 756d 6e28 5374  mapped_column(St
+00001b70: 7269 6e67 2832 3535 292c 2064 6566 6175  ring(255), defau
+00001b80: 6c74 3d22 2229 0d0a 6060 600d 0a0d 0a2d  lt="")..```....-
+00001b90: 2049 6620 796f 7520 6372 6561 7465 2061   If you create a
+00001ba0: 206d 6f64 656c 2074 6872 6f75 6768 2060   model through `
+00001bb0: 7371 6c61 6c63 6865 6d79 602c 2069 7420  sqlalchemy`, it 
+00001bc0: 6973 2072 6563 6f6d 6d65 6e64 6564 2074  is recommended t
+00001bd0: 6f20 6372 6561 7465 2061 2063 6f72 7265  o create a corre
+00001be0: 7370 6f6e 6469 6e67 2070 7964 616e 7469  sponding pydanti
+00001bf0: 6320 6d6f 6465 6c20 6174 2074 6865 2073  c model at the s
+00001c00: 616d 650d 0a20 2074 696d 652c 2061 6e64  ame..  time, and
+00001c10: 2073 6574 2060 6f72 6d5f 6d6f 6465 3d54   set `orm_mode=T
+00001c20: 7275 6560 2e0d 0a0d 0a60 6060 7079 7468  rue`.....```pyth
+00001c30: 6f6e 0d0a 6672 6f6d 2070 7964 616e 7469  on..from pydanti
+00001c40: 6320 696d 706f 7274 2042 6173 654d 6f64  c import BaseMod
+00001c50: 656c 2c20 4669 656c 640d 0a0d 0a0d 0a63  el, Field......c
+00001c60: 6c61 7373 2043 6174 6567 6f72 7953 6368  lass CategorySch
+00001c70: 656d 6128 4261 7365 4d6f 6465 6c29 3a0d  ema(BaseModel):.
+00001c80: 0a20 2020 2069 643a 2069 6e74 203d 2046  .    id: int = F
+00001c90: 6965 6c64 2864 6566 6175 6c74 3d4e 6f6e  ield(default=Non
+00001ca0: 652c 2070 7269 6d61 7279 5f6b 6579 3d54  e, primary_key=T
+00001cb0: 7275 652c 206e 756c 6c61 626c 653d 4661  rue, nullable=Fa
+00001cc0: 6c73 6529 0d0a 2020 2020 6e61 6d65 3a20  lse)..    name: 
+00001cd0: 7374 7220 3d20 4669 656c 6428 7469 746c  str = Field(titl
+00001ce0: 653d 2243 6174 6567 6f72 794e 616d 6522  e="CategoryName"
+00001cf0: 290d 0a20 2020 2064 6573 6372 6970 7469  )..    descripti
+00001d00: 6f6e 3a20 7374 7220 3d20 4669 656c 6428  on: str = Field(
+00001d10: 6465 6661 756c 743d 2222 2c20 7469 746c  default="", titl
+00001d20: 653d 2243 6174 6567 6f72 7944 6573 6372  e="CategoryDescr
+00001d30: 6970 7469 6f6e 2229 0d0a 0d0a 2020 2020  iption")....    
+00001d40: 636c 6173 7320 436f 6e66 6967 3a0d 0a20  class Config:.. 
+00001d50: 2020 2020 2020 206f 726d 5f6d 6f64 6520         orm_mode 
+00001d60: 3d20 5472 7565 0d0a 6060 600d 0a0d 0a23  = True..```....#
+00001d70: 2323 2052 6567 6973 7465 7220 4d6f 6465  ## Register Mode
+00001d80: 6c41 646d 696e 0d0a 0d0a 6060 6070 7974  lAdmin....```pyt
+00001d90: 686f 6e0d 0a66 726f 6d20 6661 7374 6170  hon..from fastap
+00001da0: 6920 696d 706f 7274 2046 6173 7441 5049  i import FastAPI
+00001db0: 0d0a 6672 6f6d 2073 716c 6d6f 6465 6c20  ..from sqlmodel 
+00001dc0: 696d 706f 7274 2053 514c 4d6f 6465 6c0d  import SQLModel.
+00001dd0: 0a66 726f 6d20 6661 7374 6170 695f 616d  .from fastapi_am
+00001de0: 6973 5f61 646d 696e 2e61 646d 696e 2e73  is_admin.admin.s
+00001df0: 6574 7469 6e67 7320 696d 706f 7274 2053  ettings import S
+00001e00: 6574 7469 6e67 730d 0a66 726f 6d20 6661  ettings..from fa
+00001e10: 7374 6170 695f 616d 6973 5f61 646d 696e  stapi_amis_admin
+00001e20: 2e61 646d 696e 2e73 6974 6520 696d 706f  .admin.site impo
+00001e30: 7274 2041 646d 696e 5369 7465 0d0a 6672  rt AdminSite..fr
+00001e40: 6f6d 2066 6173 7461 7069 5f61 6d69 735f  om fastapi_amis_
+00001e50: 6164 6d69 6e2e 6164 6d69 6e20 696d 706f  admin.admin impo
+00001e60: 7274 2061 646d 696e 0d0a 0d0a 2320 6372  rt admin....# cr
+00001e70: 6561 7465 2046 6173 7441 5049 2061 7070  eate FastAPI app
+00001e80: 6c69 6361 7469 6f6e 0d0a 6170 7020 3d20  lication..app = 
+00001e90: 4661 7374 4150 4928 290d 0a0d 0a23 2063  FastAPI()....# c
+00001ea0: 7265 6174 6520 4164 6d69 6e53 6974 6520  reate AdminSite 
+00001eb0: 696e 7374 616e 6365 0d0a 7369 7465 203d  instance..site =
+00001ec0: 2041 646d 696e 5369 7465 2873 6574 7469   AdminSite(setti
+00001ed0: 6e67 733d 5365 7474 696e 6773 2864 6174  ngs=Settings(dat
+00001ee0: 6162 6173 655f 7572 6c5f 6173 796e 633d  abase_url_async=
+00001ef0: 2773 716c 6974 652b 6169 6f73 716c 6974  'sqlite+aiosqlit
+00001f00: 653a 2f2f 2f61 6d69 7361 646d 696e 2e64  e:///amisadmin.d
+00001f10: 6227 2929 0d0a 0d0a 0d0a 2320 7265 6769  b'))......# regi
+00001f20: 7374 6572 204d 6f64 656c 4164 6d69 6e0d  ster ModelAdmin.
+00001f30: 0a40 7369 7465 2e72 6567 6973 7465 725f  .@site.register_
+00001f40: 6164 6d69 6e0d 0a63 6c61 7373 2043 6174  admin..class Cat
+00001f50: 6567 6f72 7941 646d 696e 2861 646d 696e  egoryAdmin(admin
+00001f60: 2e4d 6f64 656c 4164 6d69 6e29 3a0d 0a20  .ModelAdmin):.. 
+00001f70: 2020 2070 6167 655f 7363 6865 6d61 203d     page_schema =
+00001f80: 2027 4361 7465 676f 7279 270d 0a20 2020   'Category'..   
+00001f90: 2023 2073 6574 206d 6f64 656c 0d0a 2020   # set model..  
+00001fa0: 2020 6d6f 6465 6c20 3d20 4361 7465 676f    model = Catego
+00001fb0: 7279 0d0a 0d0a 0d0a 2320 6d6f 756e 7420  ry......# mount 
+00001fc0: 4164 6d69 6e53 6974 6520 696e 7374 616e  AdminSite instan
+00001fd0: 6365 0d0a 7369 7465 2e6d 6f75 6e74 5f61  ce..site.mount_a
+00001fe0: 7070 2861 7070 290d 0a0d 0a0d 0a23 2063  pp(app)......# c
+00001ff0: 7265 6174 6520 696e 6974 6961 6c20 6461  reate initial da
+00002000: 7461 6261 7365 2074 6162 6c65 0d0a 4061  tabase table..@a
+00002010: 7070 2e6f 6e5f 6576 656e 7428 2273 7461  pp.on_event("sta
+00002020: 7274 7570 2229 0d0a 6173 796e 6320 6465  rtup")..async de
+00002030: 6620 7374 6172 7475 7028 293a 0d0a 2020  f startup():..  
+00002040: 2020 6177 6169 7420 7369 7465 2e64 622e    await site.db.
+00002050: 6173 796e 635f 7275 6e5f 7379 6e63 2842  async_run_sync(B
+00002060: 6173 652e 6d65 7461 6461 7461 2e63 7265  ase.metadata.cre
+00002070: 6174 655f 616c 6c2c 2069 735f 7365 7373  ate_all, is_sess
+00002080: 696f 6e3d 4661 6c73 6529 0d0a 0d0a 0d0a  ion=False)......
+00002090: 6966 205f 5f6e 616d 655f 5f20 3d3d 2027  if __name__ == '
+000020a0: 5f5f 6d61 696e 5f5f 273a 0d0a 2020 2020  __main__':..    
+000020b0: 696d 706f 7274 2075 7669 636f 726e 0d0a  import uvicorn..
+000020c0: 0d0a 2020 2020 7576 6963 6f72 6e2e 7275  ..    uvicorn.ru
+000020d0: 6e28 6170 7029 0d0a 6060 600d 0a0d 0a23  n(app)..```....#
+000020e0: 2320 466f 726d 4164 6d69 6e20 4578 616d  # FormAdmin Exam
+000020f0: 706c 650d 0a0d 0a60 6060 7079 7468 6f6e  ple....```python
+00002100: 0d0a 6672 6f6d 2074 7970 696e 6720 696d  ..from typing im
+00002110: 706f 7274 2041 6e79 0d0a 6672 6f6d 2066  port Any..from f
+00002120: 6173 7461 7069 2069 6d70 6f72 7420 4661  astapi import Fa
+00002130: 7374 4150 490d 0a66 726f 6d20 7079 6461  stAPI..from pyda
+00002140: 6e74 6963 2069 6d70 6f72 7420 4261 7365  ntic import Base
+00002150: 4d6f 6465 6c0d 0a66 726f 6d20 7374 6172  Model..from star
+00002160: 6c65 7474 652e 7265 7175 6573 7473 2069  lette.requests i
+00002170: 6d70 6f72 7420 5265 7175 6573 740d 0a66  mport Request..f
+00002180: 726f 6d20 6661 7374 6170 695f 616d 6973  rom fastapi_amis
+00002190: 5f61 646d 696e 2e61 6d69 732e 636f 6d70  _admin.amis.comp
+000021a0: 6f6e 656e 7473 2069 6d70 6f72 7420 466f  onents import Fo
+000021b0: 726d 0d0a 6672 6f6d 2066 6173 7461 7069  rm..from fastapi
+000021c0: 5f61 6d69 735f 6164 6d69 6e2e 6164 6d69  _amis_admin.admi
+000021d0: 6e20 696d 706f 7274 2061 646d 696e 0d0a  n import admin..
+000021e0: 6672 6f6d 2066 6173 7461 7069 5f61 6d69  from fastapi_ami
+000021f0: 735f 6164 6d69 6e2e 6164 6d69 6e2e 7365  s_admin.admin.se
+00002200: 7474 696e 6773 2069 6d70 6f72 7420 5365  ttings import Se
+00002210: 7474 696e 6773 0d0a 6672 6f6d 2066 6173  ttings..from fas
+00002220: 7461 7069 5f61 6d69 735f 6164 6d69 6e2e  tapi_amis_admin.
+00002230: 6164 6d69 6e2e 7369 7465 2069 6d70 6f72  admin.site impor
+00002240: 7420 4164 6d69 6e53 6974 650d 0a66 726f  t AdminSite..fro
+00002250: 6d20 6661 7374 6170 695f 616d 6973 5f61  m fastapi_amis_a
+00002260: 646d 696e 2e63 7275 642e 7363 6865 6d61  dmin.crud.schema
+00002270: 2069 6d70 6f72 7420 4261 7365 4170 694f   import BaseApiO
+00002280: 7574 0d0a 6672 6f6d 2066 6173 7461 7069  ut..from fastapi
+00002290: 5f61 6d69 735f 6164 6d69 6e2e 6d6f 6465  _amis_admin.mode
+000022a0: 6c73 2e66 6965 6c64 7320 696d 706f 7274  ls.fields import
+000022b0: 2046 6965 6c64 0d0a 0d0a 2320 6372 6561   Field....# crea
+000022c0: 7465 2046 6173 7441 5049 2061 7070 6c69  te FastAPI appli
+000022d0: 6361 7469 6f6e 0d0a 6170 7020 3d20 4661  cation..app = Fa
+000022e0: 7374 4150 4928 290d 0a0d 0a23 2063 7265  stAPI()....# cre
+000022f0: 6174 6520 4164 6d69 6e53 6974 6520 696e  ate AdminSite in
+00002300: 7374 616e 6365 0d0a 7369 7465 203d 2041  stance..site = A
+00002310: 646d 696e 5369 7465 2873 6574 7469 6e67  dminSite(setting
+00002320: 733d 5365 7474 696e 6773 2864 6174 6162  s=Settings(datab
+00002330: 6173 655f 7572 6c5f 6173 796e 633d 2773  ase_url_async='s
+00002340: 716c 6974 652b 6169 6f73 716c 6974 653a  qlite+aiosqlite:
+00002350: 2f2f 2f61 6d69 7361 646d 696e 2e64 6227  ///amisadmin.db'
+00002360: 2929 0d0a 0d0a 0d0a 2320 7265 6769 7374  ))......# regist
+00002370: 6572 2046 6f72 6d41 646d 696e 0d0a 4073  er FormAdmin..@s
+00002380: 6974 652e 7265 6769 7374 6572 5f61 646d  ite.register_adm
+00002390: 696e 0d0a 636c 6173 7320 5573 6572 4c6f  in..class UserLo
+000023a0: 6769 6e46 6f72 6d41 646d 696e 2861 646d  ginFormAdmin(adm
+000023b0: 696e 2e46 6f72 6d41 646d 696e 293a 0d0a  in.FormAdmin):..
+000023c0: 2020 2020 7061 6765 5f73 6368 656d 6120      page_schema 
+000023d0: 3d20 2755 7365 724c 6f67 696e 466f 726d  = 'UserLoginForm
+000023e0: 270d 0a20 2020 2023 2073 6574 2066 6f72  '..    # set for
+000023f0: 6d20 696e 666f 726d 6174 696f 6e2c 206f  m information, o
+00002400: 7074 696f 6e61 6c0d 0a20 2020 2066 6f72  ptional..    for
+00002410: 6d20 3d20 466f 726d 2874 6974 6c65 3d27  m = Form(title='
+00002420: 5468 6973 2069 7320 6120 7465 7374 206c  This is a test l
+00002430: 6f67 696e 2066 6f72 6d27 2c20 7375 626d  ogin form', subm
+00002440: 6974 5465 7874 3d27 6c6f 6769 6e27 290d  itText='login').
+00002450: 0a0d 0a20 2020 2023 2063 7265 6174 6520  ...    # create 
+00002460: 666f 726d 2073 6368 656d 610d 0a20 2020  form schema..   
+00002470: 2063 6c61 7373 2073 6368 656d 6128 4261   class schema(Ba
+00002480: 7365 4d6f 6465 6c29 3a0d 0a20 2020 2020  seModel):..     
+00002490: 2020 2075 7365 726e 616d 653a 2073 7472     username: str
+000024a0: 203d 2046 6965 6c64 282e 2e2e 2c20 7469   = Field(..., ti
+000024b0: 746c 653d 2775 7365 726e 616d 6527 2c20  tle='username', 
+000024c0: 6d69 6e5f 6c65 6e67 7468 3d33 2c20 6d61  min_length=3, ma
+000024d0: 785f 6c65 6e67 7468 3d33 3029 0d0a 2020  x_length=30)..  
+000024e0: 2020 2020 2020 7061 7373 776f 7264 3a20        password: 
+000024f0: 7374 7220 3d20 4669 656c 6428 2e2e 2e2c  str = Field(...,
+00002500: 2074 6974 6c65 3d27 7061 7373 776f 7264   title='password
+00002510: 2729 0d0a 0d0a 2020 2020 2320 6861 6e64  ')....    # hand
+00002520: 6c65 2066 6f72 6d20 7375 626d 6973 7369  le form submissi
+00002530: 6f6e 2064 6174 610d 0a20 2020 2061 7379  on data..    asy
+00002540: 6e63 2064 6566 2068 616e 646c 6528 7365  nc def handle(se
+00002550: 6c66 2c20 7265 7175 6573 743a 2052 6571  lf, request: Req
+00002560: 7565 7374 2c20 6461 7461 3a20 4261 7365  uest, data: Base
+00002570: 4d6f 6465 6c2c 202a 2a6b 7761 7267 7329  Model, **kwargs)
+00002580: 202d 3e20 4261 7365 4170 694f 7574 5b41   -> BaseApiOut[A
+00002590: 6e79 5d3a 0d0a 2020 2020 2020 2020 6966  ny]:..        if
+000025a0: 2064 6174 612e 7573 6572 6e61 6d65 203d   data.username =
+000025b0: 3d20 2761 6d69 7361 646d 696e 2720 616e  = 'amisadmin' an
+000025c0: 6420 6461 7461 2e70 6173 7377 6f72 6420  d data.password 
+000025d0: 3d3d 2027 616d 6973 6164 6d69 6e27 3a0d  == 'amisadmin':.
+000025e0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+000025f0: 7572 6e20 4261 7365 4170 694f 7574 286d  urn BaseApiOut(m
+00002600: 7367 3d27 4c6f 6769 6e20 7375 6363 6573  sg='Login succes
+00002610: 7366 756c 6c79 2127 2c20 6461 7461 3d7b  sfully!', data={
+00002620: 2774 6f6b 656e 273a 2027 7878 7878 7878  'token': 'xxxxxx
+00002630: 277d 290d 0a20 2020 2020 2020 2072 6574  '})..        ret
+00002640: 7572 6e20 4261 7365 4170 694f 7574 2873  urn BaseApiOut(s
+00002650: 7461 7475 733d 2d31 2c20 6d73 673d 2749  tatus=-1, msg='I
+00002660: 6e63 6f72 7265 6374 2075 7365 726e 616d  ncorrect usernam
+00002670: 6520 6f72 2070 6173 7377 6f72 6421 2729  e or password!')
+00002680: 0d0a 0d0a 0d0a 2320 6d6f 756e 7420 4164  ......# mount Ad
+00002690: 6d69 6e53 6974 6520 696e 7374 616e 6365  minSite instance
+000026a0: 0d0a 7369 7465 2e6d 6f75 6e74 5f61 7070  ..site.mount_app
+000026b0: 2861 7070 290d 0a0d 0a69 6620 5f5f 6e61  (app)....if __na
+000026c0: 6d65 5f5f 203d 3d20 275f 5f6d 6169 6e5f  me__ == '__main_
+000026d0: 5f27 3a0d 0a20 2020 2069 6d70 6f72 7420  _':..    import 
+000026e0: 7576 6963 6f72 6e0d 0a0d 0a20 2020 2075  uvicorn....    u
+000026f0: 7669 636f 726e 2e72 756e 2861 7070 290d  vicorn.run(app).
+00002700: 0a60 6060 0d0a 0d0a 2323 2057 6f72 6b69  .```....## Worki
+00002710: 6e67 2077 6974 6820 436f 6d6d 616e 640d  ng with Command.
+00002720: 0a0d 0a60 6060 6261 7368 0d0a 2320 496e  ...```bash..# In
+00002730: 7374 616c 6c20 636f 6d6d 616e 6420 6c69  stall command li
+00002740: 6e65 2065 7874 656e 7369 6f6e 0d0a 7069  ne extension..pi
+00002750: 7020 696e 7374 616c 6c20 6661 7374 6170  p install fastap
+00002760: 695f 616d 6973 5f61 646d 696e 5b63 6c69  i_amis_admin[cli
+00002770: 5d0d 0a0d 0a23 2056 6965 7720 6865 6c70  ]....# View help
+00002780: 0d0a 6661 6120 2d2d 6865 6c70 0d0a 0d0a  ..faa --help....
+00002790: 2320 496e 6974 6961 6c69 7a65 2061 2060  # Initialize a `
+000027a0: 4661 7374 4150 492d 416d 6973 2d41 646d  FastAPI-Amis-Adm
+000027b0: 696e 6020 7072 6f6a 6563 740d 0a66 6161  in` project..faa
+000027c0: 206e 6577 2070 726f 6a65 6374 5f6e 616d   new project_nam
+000027d0: 6520 2d2d 696e 6974 0d0a 0d0a 2320 496e  e --init....# In
+000027e0: 6974 6961 6c69 7a65 2061 2060 4661 7374  itialize a `Fast
+000027f0: 4150 492d 416d 6973 2d41 646d 696e 6020  API-Amis-Admin` 
+00002800: 6170 706c 6963 6174 696f 6e0d 0a66 6161  application..faa
+00002810: 206e 6577 2061 7070 5f6e 616d 650d 0a0d   new app_name...
+00002820: 0a23 2046 6173 7420 7275 6e6e 696e 6720  .# Fast running 
+00002830: 7072 6f6a 6563 740d 0a66 6161 2072 756e  project..faa run
+00002840: 0d0a 6060 600d 0a0d 0a23 2320 5072 6576  ..```....## Prev
+00002850: 6965 770d 0a0d 0a2d 204f 7065 6e20 6068  iew....- Open `h
+00002860: 7474 703a 2f2f 3132 372e 302e 302e 313a  ttp://127.0.0.1:
+00002870: 3830 3030 2f61 646d 696e 2f60 2069 6e20  8000/admin/` in 
+00002880: 796f 7572 2062 726f 7773 6572 3a0d 0a0d  your browser:...
+00002890: 0a21 5b4d 6f64 656c 4164 6d69 6e5d 2868  .![ModelAdmin](h
+000028a0: 7474 7073 3a2f 2f73 322e 6c6f 6c69 2e6e  ttps://s2.loli.n
+000028b0: 6574 2f32 3032 322f 3033 2f32 302f 4974  et/2022/03/20/It
+000028c0: 6746 5947 554f 4e6d 316a 437a 352e 706e  gFYGUONm1jCz5.pn
+000028d0: 6729 0d0a 0d0a 2d20 4f70 656e 2060 6874  g)....- Open `ht
+000028e0: 7470 3a2f 2f31 3237 2e30 2e30 2e31 3a38  tp://127.0.0.1:8
+000028f0: 3030 302f 6164 6d69 6e2f 646f 6373 6020  000/admin/docs` 
+00002900: 696e 2079 6f75 7220 6272 6f77 7365 723a  in your browser:
+00002910: 0d0a 0d0a 215b 446f 6373 5d28 6874 7470  ....![Docs](http
+00002920: 733a 2f2f 7332 2e6c 6f6c 692e 6e65 742f  s://s2.loli.net/
+00002930: 3230 3232 2f30 332f 3230 2f31 4763 4369  2022/03/20/1GcCi
+00002940: 5064 6d58 6179 7872 6248 2e70 6e67 290d  PdmXayxrbH.png).
+00002950: 0a0d 0a23 2320 5072 6f6a 6563 740d 0a0d  ...## Project...
+00002960: 0a2d 205b 6041 6d69 732d 4164 6d69 6e2d  .- [`Amis-Admin-
+00002970: 5468 656d 652d 4564 6974 6f72 605d 2868  Theme-Editor`](h
+00002980: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00002990: 6d2f 7377 656c 636b 6572 2f61 6d69 732d  m/swelcker/amis-
+000029a0: 6164 6d69 6e2d 7468 656d 652d 6564 6974  admin-theme-edit
+000029b0: 6f72 293a 5468 656d 652d 4564 6974 6f72  or):Theme-Editor
+000029c0: 2066 6f72 2074 6865 2066 6173 7461 7069   for the fastapi
+000029d0: 2d61 6d69 732d 6164 6d69 6e2e 0d0a 2020  -amis-admin...  
+000029e0: 416c 6c6f 7773 2074 6f20 6164 6420 6375  Allows to add cu
+000029f0: 7374 6f6d 2063 7373 2073 7479 6c65 7320  stom css styles 
+00002a00: 616e 6420 746f 2061 7070 6c79 2074 6865  and to apply the
+00002a10: 6d65 202d 2d76 6172 7320 6368 616e 6765  me --vars change
+00002a20: 206f 6e20 7468 6520 666c 792e 0d0a 2d20   on the fly...- 
+00002a30: 5b60 4661 7374 4150 492d 5573 6572 2d41  [`FastAPI-User-A
+00002a40: 7574 6860 5d28 6874 7470 733a 2f2f 6769  uth`](https://gi
+00002a50: 7468 7562 2e63 6f6d 2f61 6d69 7361 646d  thub.com/amisadm
+00002a60: 696e 2f66 6173 7461 7069 5f75 7365 725f  in/fastapi_user_
+00002a70: 6175 7468 293a 2041 2073 696d 706c 6520  auth): A simple 
+00002a80: 616e 6420 706f 7765 7266 756c 2060 4661  and powerful `Fa
+00002a90: 7374 4150 4960 2075 7365 7220 6052 4241  stAPI` user `RBA
+00002aa0: 4360 0d0a 2020 6175 7468 656e 7469 6361  C`..  authentica
+00002ab0: 7469 6f6e 2061 6e64 2061 7574 686f 7269  tion and authori
+00002ac0: 7a61 7469 6f6e 206c 6962 7261 7279 2e0d  zation library..
+00002ad0: 0a2d 205b 6046 6173 7441 5049 2d53 6368  .- [`FastAPI-Sch
+00002ae0: 6564 756c 6572 605d 2868 7474 7073 3a2f  eduler`](https:/
+00002af0: 2f67 6974 6875 622e 636f 6d2f 616d 6973  /github.com/amis
+00002b00: 6164 6d69 6e2f 6661 7374 6170 695f 7363  admin/fastapi_sc
+00002b10: 6865 6475 6c65 7229 3a20 4120 7369 6d70  heduler): A simp
+00002b20: 6c65 2073 6368 6564 756c 6564 2074 6173  le scheduled tas
+00002b30: 6b20 6d61 6e61 6765 6d65 6e74 2060 4661  k management `Fa
+00002b40: 7374 4150 4960 2065 7874 656e 7369 6f6e  stAPI` extension
+00002b50: 0d0a 2020 6261 7365 6420 6f6e 2060 4150  ..  based on `AP
+00002b60: 5363 6865 6475 6c65 7260 2e0d 0a2d 205b  Scheduler`...- [
+00002b70: 6046 6173 7441 5049 2d43 6f6e 6669 6760  `FastAPI-Config`
+00002b80: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00002b90: 2e63 6f6d 2f61 6d69 7361 646d 696e 2f66  .com/amisadmin/f
+00002ba0: 6173 7461 7069 2d63 6f6e 6669 6729 3a20  astapi-config): 
+00002bb0: 4120 7669 7375 616c 2064 796e 616d 6963  A visual dynamic
+00002bc0: 2063 6f6e 6669 6775 7261 7469 6f6e 206d   configuration m
+00002bd0: 616e 6167 656d 656e 7420 6578 7465 6e73  anagement extens
+00002be0: 696f 6e20 7061 636b 6167 650d 0a20 2062  ion package..  b
+00002bf0: 6173 6564 206f 6e20 6046 6173 7441 5049  ased on `FastAPI
+00002c00: 2d41 6d69 732d 4164 6d69 6e60 2e0d 0a2d  -Amis-Admin`...-
+00002c10: 205b 6046 6173 7441 5049 2d41 6d69 732d   [`FastAPI-Amis-
+00002c20: 4164 6d69 6e2d 4465 6d6f 605d 2868 7474  Admin-Demo`](htt
+00002c30: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00002c40: 616d 6973 6164 6d69 6e2f 6661 7374 6170  amisadmin/fastap
+00002c50: 695f 616d 6973 5f61 646d 696e 5f64 656d  i_amis_admin_dem
+00002c60: 6f29 3a20 416e 2065 7861 6d70 6c65 2060  o): An example `
+00002c70: 4661 7374 4150 492d 416d 6973 2d41 646d  FastAPI-Amis-Adm
+00002c80: 696e 6020 6170 706c 6963 6174 696f 6e2e  in` application.
+00002c90: 0d0a 2d20 5b60 4661 7374 4150 492d 5573  ..- [`FastAPI-Us
+00002ca0: 6572 2d41 7574 682d 4465 6d6f 605d 2868  er-Auth-Demo`](h
+00002cb0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00002cc0: 6d2f 616d 6973 6164 6d69 6e2f 6661 7374  m/amisadmin/fast
+00002cd0: 6170 695f 7573 6572 5f61 7574 685f 6465  api_user_auth_de
+00002ce0: 6d6f 293a 2041 6e20 6578 616d 706c 6520  mo): An example 
+00002cf0: 6046 6173 7441 5049 2d55 7365 722d 4175  `FastAPI-User-Au
+00002d00: 7468 6020 6170 706c 6963 6174 696f 6e2e  th` application.
+00002d10: 0d0a 0d0a 2323 204c 6963 656e 7365 0d0a  ....## License..
+00002d20: 0d0a 2d20 4163 636f 7264 696e 6720 746f  ..- According to
+00002d30: 2074 6865 2060 4170 6163 6865 322e 3060   the `Apache2.0`
+00002d40: 2070 726f 746f 636f 6c2c 2060 6661 7374   protocol, `fast
+00002d50: 6170 692d 616d 6973 2d61 646d 696e 6020  api-amis-admin` 
+00002d60: 6973 2066 7265 6520 616e 6420 6f70 656e  is free and open
+00002d70: 2073 6f75 7263 652e 2049 7420 6361 6e20   source. It can 
+00002d80: 6265 2075 7365 6420 666f 7220 636f 6d6d  be used for comm
+00002d90: 6572 6369 616c 2066 6f72 0d0a 2020 6672  ercial for..  fr
+00002da0: 6565 2c20 6275 7420 706c 6561 7365 2063  ee, but please c
+00002db0: 6c65 6172 6c79 2064 6973 706c 6179 2063  learly display c
+00002dc0: 6f70 7972 6967 6874 2069 6e66 6f72 6d61  opyright informa
+00002dd0: 7469 6f6e 2061 626f 7574 2060 4661 7374  tion about `Fast
+00002de0: 4150 492d 416d 6973 2d41 646d 696e 6020  API-Amis-Admin` 
+00002df0: 6f6e 2074 6865 2064 6973 706c 6179 2069  on the display i
+00002e00: 6e74 6572 6661 6365 2e0d 0a0d 0a         nterface.....
```

### Comparing `fastapi_amis_admin-0.6.3/fastapi_amis_admin/admin/admin.py` & `fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/admin/admin.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,1480 +1,1480 @@
-import asyncio
-import datetime
-import re
-from functools import lru_cache
-from typing import (
-    Any,
-    Awaitable,
-    Callable,
-    Dict,
-    Generic,
-    Iterable,
-    Iterator,
-    List,
-    Optional,
-    Tuple,
-    Type,
-    TypeVar,
-    Union,
-)
-
-from fastapi import Body, Depends, FastAPI, HTTPException, Request
-from pydantic import BaseModel
-from pydantic.utils import deep_update
-from sqlalchemy import Column, Table, delete, insert
-from sqlalchemy.orm import InstrumentedAttribute, RelationshipProperty
-from sqlalchemy.sql.elements import Label
-from sqlalchemy.util import md5_hex
-from sqlalchemy_database import AsyncDatabase, Database
-from starlette import status
-from starlette.middleware.base import BaseHTTPMiddleware
-from starlette.responses import HTMLResponse, JSONResponse, Response
-from starlette.templating import Jinja2Templates
-from typing_extensions import Annotated, Literal
-
-import fastapi_amis_admin
-from fastapi_amis_admin.admin.handlers import register_exception_handlers
-from fastapi_amis_admin.admin.parser import AmisParser
-from fastapi_amis_admin.admin.settings import Settings
-from fastapi_amis_admin.amis.components import (
-    Action,
-    ActionType,
-    App,
-    ColumnOperation,
-    Dialog,
-    Form,
-    FormItem,
-    Iframe,
-    InputExcel,
-    InputTable,
-    Page,
-    PageSchema,
-    Picker,
-    Remark,
-    Service,
-    TableColumn,
-    TableCRUD,
-    Tpl,
-)
-from fastapi_amis_admin.amis.constants import DisplayModeEnum, LevelEnum, SizeEnum
-from fastapi_amis_admin.amis.types import (
-    AmisAPI,
-    AmisNode,
-    BaseAmisApiOut,
-    BaseAmisModel,
-    SchemaNode,
-)
-from fastapi_amis_admin.crud import RouterMixin, SqlalchemyCrud
-from fastapi_amis_admin.crud.base import SchemaCreateT, SchemaFilterT, SchemaUpdateT
-from fastapi_amis_admin.crud.parser import (
-    SqlaField,
-    TableModelParser,
-    get_python_type_parse,
-)
-from fastapi_amis_admin.crud.schema import BaseApiOut, CrudEnum, Paginator
-from fastapi_amis_admin.crud.utils import (
-    IdStrQuery,
-    SqlalchemyDatabase,
-    get_engine_db,
-    parser_str_set_list,
-)
-from fastapi_amis_admin.utils.functools import cached_property
-from fastapi_amis_admin.utils.pydantic import ModelField, create_model_by_model, model_fields
-from fastapi_amis_admin.utils.translation import i18n as _
-
-BaseAdminT = TypeVar("BaseAdminT", bound="BaseAdmin")
-PageSchemaAdminT = TypeVar("PageSchemaAdminT", bound="PageSchemaAdmin")
-ActionT = Union[Action, Awaitable[Action]]
-
-
-class LinkModelForm:
-    link_model: Table
-
-    def __init__(
-        self,
-        pk_admin: "ModelAdmin",
-        display_admin: "ModelAdmin",
-        link_model: Table,
-        link_col: Column,
-        item_col: Column,
-    ):
-        self.link_model = link_model
-        self.pk_admin = pk_admin
-        self.display_admin = display_admin
-        assert self.display_admin, "display_admin is None"
-        self.link_col = link_col
-        self.item_col = item_col
-        assert self.item_col is not None, "item_col is None"
-        assert self.link_col is not None, "link_col is None"
-        self.path = f"/{self.display_admin.model.__name__}"
-
-    @classmethod
-    def bind_model_admin(cls, pk_admin: "ModelAdmin", insfield: InstrumentedAttribute) -> Optional["LinkModelForm"]:
-        if not isinstance(insfield.property, RelationshipProperty):
-            return None
-        table = insfield.property.secondary
-        if table is None:
-            return None
-        admin = None
-        link_key = None
-        item_key = None
-        for key in table.foreign_keys:
-            if key.column.table != pk_admin.model.__table__:  # Get the associated third-party table
-                admin = pk_admin.app.site.get_model_admin(key.column.table.name)
-                link_key = key
-            else:
-                item_key = key
-        if admin and link_key and item_key:
-            admin.link_models[pk_admin.model.__table__.name] = (table, link_key.parent, item_key.parent)
-            return LinkModelForm(
-                pk_admin=pk_admin,
-                display_admin=admin,
-                link_model=table,
-                link_col=link_key.parent,
-                item_col=item_key.parent,
-            )
-        return None
-
-    @property
-    def route_delete(self):
-        async def route(
-            request: Request,
-            link_id: IdStrQuery,
-            item_id: self.pk_admin.AnnotatedItemIdList,  # type: ignore
-        ):
-            if not await self.pk_admin.has_update_permission(request, item_id, None):
-                return self.pk_admin.error_no_router_permission(request)
-            stmt = (
-                delete(self.link_model)
-                .where(self.link_col.in_(list(map(get_python_type_parse(self.link_col), parser_str_set_list(link_id)))))
-                .where(self.item_col.in_(list(map(get_python_type_parse(self.item_col), item_id))))
-            )
-            result = await self.pk_admin.db.async_execute(stmt)
-            return BaseApiOut(data=result.rowcount)  # type: ignore
-
-        return route
-
-    @property
-    def route_create(self):
-        async def route(
-            request: Request,
-            link_id: IdStrQuery,
-            item_id: self.pk_admin.AnnotatedItemIdList,  # type: ignore
-        ):
-            if not await self.pk_admin.has_update_permission(request, item_id, None):
-                return self.pk_admin.error_no_router_permission(request)
-            values = []
-            for item in map(get_python_type_parse(self.item_col), item_id):
-                values.extend(
-                    {self.link_col.key: link, self.item_col.key: item}
-                    for link in map(get_python_type_parse(self.link_col), parser_str_set_list(link_id))
-                )
-            stmt = insert(self.link_model).values(values)
-            try:
-                result = await self.pk_admin.db.async_execute(stmt)
-            except Exception as error:
-                return self.pk_admin.error_execute_sql(request=request, error=error)
-            return BaseApiOut(data=result.rowcount)  # type: ignore
-
-        return route
-
-    async def get_form_item(self, request: Request):
-        url = self.display_admin.router_path + self.display_admin.page_path
-        picker = Picker(
-            name=self.display_admin.model.__table__.name,
-            label=self.display_admin.page_schema.label,
-            labelField="name",
-            valueField="id",
-            multiple=True,
-            required=False,
-            modalMode="dialog",
-            size="full",
-            pickerSchema={"&": "${body}"},
-            source={
-                "method": "post",
-                "data": "${body.api.data}",
-                "url": "${body.api.url}&link_model=" + self.pk_admin.model.__table__.name + "&op=in_&link_item_id=${"
-                "api.qsOptions.id}",
-            },
-        )
-        adaptor = None
-        if await self.pk_admin.has_update_permission(request, None, None):
-            button_create = ActionType.Ajax(
-                actionType="ajax",
-                label=_("Add Association"),
-                level=LevelEnum.danger,
-                confirmText=_("Are you sure you want to add the association?"),
-                api=f"post:{self.pk_admin.app.router_path}{self.pk_admin.router.prefix}{self.path}"
-                + '/${REPLACE(query.link_item_id, "!", "")}?link_id=${IF(ids, ids, id)}',
-            )  # query.link_item_id
-            adaptor = (
-                'if(!payload.hasOwnProperty("_payload")){payload._payload=JSON.stringify(payload);}'
-                "payload=JSON.parse(payload._payload);button_create=" + button_create.amis_json() + ";"
-                "payload.data.body.bulkActions.push(button_create);"
-                "payload.data.body.itemActions.push(button_create);"
-                "return payload;".replace("action_id", "create" + self.path.replace("/", "_"))
-            )
-            button_create_dialog = ActionType.Dialog(
-                icon="fa fa-plus pull-left",
-                label=_("Add Association"),
-                level=LevelEnum.danger,
-                dialog=Dialog(
-                    title=_("Add Association"),
-                    size="full",
-                    body=Service(
-                        schemaApi=AmisAPI(
-                            method="post",
-                            url=url,
-                            data={},
-                            cache=300000,
-                            responseData={
-                                "&": "${body}",
-                                "api.url": "${body.api.url}&op=not_in&link_model="
-                                + self.pk_admin.model.__table__.name
-                                + "&link_item_id=${api.qsOptions.id}",
-                            },
-                            qsOptions={"id": f"${self.pk_admin.pk_name}"},
-                            adaptor=adaptor,
-                        )
-                    ),
-                ),
-            )
-
-            button_delete = ActionType.Ajax(
-                actionType="ajax",
-                label=_("Remove Association"),
-                level=LevelEnum.danger,
-                confirmText=_("Are you sure you want to remove the association?"),
-                api=f"delete:{self.pk_admin.app.router_path}{self.pk_admin.router.prefix}{self.path}"
-                + "/${query.link_item_id}?link_id=${IF(ids, ids, id)}",
-            )
-            adaptor = (
-                'if(!payload.hasOwnProperty("_payload")){payload._payload=JSON.stringify(payload);}'
-                "payload=JSON.parse(payload._payload);button_delete="
-                + button_delete.amis_json()
-                + ";payload.data.body.headerToolbar.push("
-                + button_create_dialog.amis_json()
-                + ");payload.data.body.bulkActions.push(button_delete);payload.data.body.itemActions.push(button_delete);"
-                "return payload;".replace("action_id", "delete" + self.path.replace("/", "_"))
-            )
-        return Service(
-            schemaApi=AmisAPI(
-                method="post",
-                url=url,
-                data={},
-                cache=300000,
-                responseData={"controls": [picker]},
-                qsOptions={"id": f"${self.pk_admin.pk_name}"},
-                adaptor=adaptor,
-            )
-        )
-
-    def register_router(self):
-        self.pk_admin.router.add_api_route(
-            self.path + "/{item_id}",
-            self.route_delete,
-            methods=["DELETE"],
-            response_model=BaseApiOut[int],
-            name=f"{self.link_model.name}_Delete",
-        )
-
-        self.pk_admin.router.add_api_route(
-            self.path + "/{item_id}",
-            self.route_create,
-            methods=["POST"],
-            response_model=BaseApiOut[int],
-            name=f"{self.link_model.name}_Create",
-        )
-
-        return self
-
-
-class BaseAdmin:
-    def __init__(self, app: "AdminApp"):
-        self.app = app
-        assert self.app, "app is None"
-
-    @cached_property
-    def site(self) -> "BaseAdminSite":
-        return self if self.app is self else self.app.site
-
-    @cached_property
-    def unique_id(self) -> str:
-        unique_str = f"{self.__class__.__module__}:{self.__class__.__qualname__}"
-        if self.app is not self:
-            unique_str += f"{self.app.unique_id}"
-        return md5_hex(unique_str)[:16]
-
-
-class PageSchemaAdmin(BaseAdmin):
-    page_schema: Union[PageSchema, str] = PageSchema()
-
-    def __init__(self, app: "AdminApp"):
-        super().__init__(app)
-        self.page_schema = self.get_page_schema()
-        if self.page_schema and self.page_schema.url:
-            self.page_schema.url = self.page_schema.url.replace(self.site.settings.site_url, "")
-
-    async def has_page_permission(self, request: Request, obj: "PageSchemaAdmin" = None, action: str = None) -> bool:
-        return self.app is self or await self.app.has_page_permission(request, obj=obj or self, action=action)
-
-    def get_page_schema(self) -> Optional[PageSchema]:
-        if self.page_schema:
-            if isinstance(self.page_schema, str):
-                self.page_schema = PageSchema(label=self.page_schema)
-            elif isinstance(self.page_schema, PageSchema):
-                self.page_schema = self.page_schema.copy(deep=True)
-                self.page_schema.label = self.page_schema.label or self.__class__.__name__
-            else:
-                raise TypeError()
-        return self.page_schema
-
-
-class LinkAdmin(PageSchemaAdmin):
-    link: str = ""
-
-    def get_page_schema(self) -> Optional[PageSchema]:
-        if super().get_page_schema():
-            assert self.link, "link is None"
-            self.page_schema.link = self.page_schema.link or self.link
-        return self.page_schema
-
-
-class IframeAdmin(PageSchemaAdmin):
-    iframe: Iframe = None
-    src: str = ""
-
-    def get_page_schema(self) -> Optional[PageSchema]:
-        if super().get_page_schema():
-            assert self.src, "src is None"
-            iframe = self.iframe or Iframe(src=self.src)
-            if self.site.settings.site_url and iframe.src.startswith(self.site.settings.site_url):
-                self.page_schema.url = iframe.src
-            else:
-                self.page_schema.url = re.sub(r"^https?:", "", iframe.src)
-            self.page_schema.schema_ = iframe
-        return self.page_schema
-
-
-class RouterAdmin(BaseAdmin, RouterMixin):
-    def __init__(self, app: "AdminApp"):
-        BaseAdmin.__init__(self, app)
-        RouterMixin.__init__(self)
-
-    def register_router(self):
-        raise NotImplementedError()
-
-    @cached_property
-    def router_path(self) -> str:
-        if self.router is self.app.router:
-            return self.app.router_path
-        return self.app.router_path + self.router.prefix
-
-
-class PageAdmin(PageSchemaAdmin, RouterAdmin):
-    """Amis page management"""
-
-    page: Page = None
-    page_path: Optional[str] = None
-    page_parser_mode: Literal["json", "html"] = "json"
-    page_route_kwargs: Dict[str, Any] = {}
-    template_name: str = ""
-    router_prefix = "/page"
-
-    def __init__(self, app: "AdminApp"):
-        RouterAdmin.__init__(self, app)
-        if self.page_path is None:
-            self.page_path = f"/{self.__class__.__module__}/{self.__class__.__name__}"
-        PageSchemaAdmin.__init__(self, app)
-
-    async def page_permission_depend(self, request: Request) -> bool:
-        return await self.has_page_permission(request, action="page") or self.error_no_page_permission(request)
-
-    def error_no_page_permission(self, request: Request):
-        raise HTTPException(
-            status_code=status.HTTP_307_TEMPORARY_REDIRECT,
-            detail="No page permissions",
-            headers={
-                "location": f"{self.site.router_path}{self.site.router.url_path_for('login')}?redirect={request.url.path}",
-            },
-        )
-
-    async def get_page(self, request: Request) -> Page:
-        return self.page or Page()
-
-    def get_page_schema(self) -> Optional[PageSchema]:
-        if super().get_page_schema():
-            self.page_schema.url = f"{self.router_path}{self.page_path}"
-            self.page_schema.schemaApi = AmisAPI(
-                method="post",
-                url=f"{self.router_path}{self.page_path}",
-                data={},
-                cache=300000,
-            )
-            if self.page_parser_mode == "html":
-                self.page_schema.schema_ = Iframe(src=self.page_schema.url)
-        return self.page_schema
-
-    async def page_parser(self, request: Request, page: Page) -> Response:
-        if request.method == "GET":
-            result = page.amis_html(
-                template_path=self.template_name,
-                locale=_.get_language(),
-                cdn=self.site.settings.amis_cdn,
-                pkg=self.site.settings.amis_pkg,
-                theme=self.site.settings.amis_theme,
-                site_title=self.site.settings.site_title,
-                site_icon=self.site.settings.site_icon,
-            )
-            result = HTMLResponse(result)
-        else:
-            data = page.amis_dict()
-            if await request.body():
-                data = deep_update(data, (await request.json()).get("_update", {}))
-            result = BaseAmisApiOut(data=data)
-            result = JSONResponse(result.dict())
-        return result
-
-    def register_router(self):
-        self.router.add_api_route(
-            self.page_path,
-            self.route_page,
-            methods=["GET"],
-            dependencies=[Depends(self.page_permission_depend)],
-            include_in_schema=False,
-            response_class=HTMLResponse,
-            **self.page_route_kwargs,
-        )
-        self.router.add_api_route(
-            self.page_path,
-            self.route_page,
-            methods=["POST"],
-            dependencies=[Depends(self.page_permission_depend)],
-            response_model=BaseAmisApiOut,
-            include_in_schema=(self.page_parser_mode == "json"),
-            **self.page_route_kwargs,
-        )
-        return self
-
-    @property
-    def AnnotatedPage(self):
-        """Annotated Page, for fastapi dependency injection"""
-        return Annotated[Page, Depends(self.get_page)]
-
-    @property
-    def route_page(self) -> Callable:
-        async def route(
-            request: Request,
-            page: self.AnnotatedPage,  # type:ignore
-        ):
-            return await self.page_parser(request, page)
-
-        return route
-
-
-class TemplateAdmin(PageAdmin):
-    """Jinja2 render template management"""
-
-    page: Dict[str, Any] = {}
-    page_parser_mode = "html"
-    templates: Jinja2Templates = None
-
-    def __init__(self, app: "AdminApp"):
-        assert self.templates, "templates:Jinja2Templates is None"
-        assert self.template_name, "template_name is None"
-        self.page_path = self.page_path or f"/{self.template_name}"
-        super().__init__(app)
-
-    async def page_parser(self, request: Request, page: Dict[str, Any]) -> Response:
-        page["request"] = request
-        return self.templates.TemplateResponse(self.template_name, page)
-
-    async def get_page(self, request: Request) -> Dict[str, Any]:
-        return {}
-
-
-class BaseActionAdmin(PageAdmin):
-    admin_action_maker: List[Callable[["BaseActionAdmin"], "AdminAction"]] = []  # Actions
-
-    @cached_property
-    def registered_admin_actions(self) -> Dict[str, "AdminAction"]:
-        admin_actions = {}
-        for maker in self.admin_action_maker:
-            admin_action = maker(self)
-            if admin_action:
-                admin_actions[admin_action.name] = admin_action
-        return admin_actions
-
-    async def get_action(self, request: Request, name: str) -> Action:
-        admin_action = self.registered_admin_actions.get(name)
-        return await admin_action.get_action(request)
-
-    async def get_actions(self, request: Request, flag: str) -> List[Action]:
-        actions = []
-        for admin_action in self.registered_admin_actions.values():
-            if flag not in admin_action.flags:
-                continue
-            if await self.has_action_permission(request, name=admin_action.name):
-                actions.append(await admin_action.get_action(request, name=admin_action.name))
-        return list(filter(None, actions))
-
-    async def has_action_permission(self, request: Request, name: str) -> bool:
-        return True
-
-    def register_router(self):
-        for admin_action in self.registered_admin_actions.values():
-            if isinstance(admin_action, RouterAdmin):
-                admin_action.register_router()
-        return super().register_router()
-
-
-class FormAdmin(BaseActionAdmin, Generic[SchemaUpdateT]):
-    schema: Type[SchemaUpdateT] = None
-    schema_init_out: Type[Any] = Any
-    schema_submit_out: Type[Any] = Any
-    form: Form = None
-    form_init: bool = None
-    form_path: str = ""
-    router_prefix: str = "/form"
-
-    def __init__(self, app: "AdminApp"):
-        super().__init__(app)
-        assert self.schema, "schema is None"
-        self.form_path = self.form_path or f"{self.page_path}/api"
-
-    async def get_page(self, request: Request) -> Page:
-        page = await super(FormAdmin, self).get_page(request)
-        page.body = await self.get_form(request)
-        return page
-
-    async def get_form_item(self, request: Request, modelfield: ModelField) -> Union[FormItem, SchemaNode]:
-        return self.site.amis_parser.as_form_item(modelfield, set_default=True)
-
-    async def get_form(self, request: Request) -> Form:
-        form = self.form or Form()
-        form.api = AmisAPI(method="POST", url=f"{self.router_path}{self.form_path}")
-        form.initApi = AmisAPI(method="GET", url=f"{self.router_path}{self.form_path}") if self.form_init else None
-        form.title = ""
-        actions = await self.get_actions(request, flag="item")
-        if actions:
-            form.actions = actions
-        form.body = []
-        for modelfield in model_fields(self.schema).values():
-            formitem = await self.get_form_item(request, modelfield)
-            if formitem:
-                form.body.append(formitem)
-        return form
-
-    def register_router(self):
-        super().register_router()
-        self.router.add_api_route(
-            self.form_path,
-            self.route_submit,
-            methods=["POST"],
-            response_model=BaseApiOut[self.schema_submit_out],
-            dependencies=[Depends(self.page_permission_depend)],
-        )
-        if self.form_init:
-            self.schema_init_out = self.schema_init_out or create_model_by_model(
-                self.schema, f"{self.__class__.__name__}InitOut", set_none=True
-            )
-            self.router.add_api_route(
-                self.form_path,
-                self.route_init,
-                methods=["GET"],
-                response_model=BaseApiOut[self.schema_init_out],
-                dependencies=[Depends(self.page_permission_depend)],
-            )
-        return self
-
-    async def get_init_data(self, request: Request, **kwargs) -> BaseApiOut[Any]:
-        return BaseApiOut()
-
-    @property
-    def route_init(self):
-        async def route(request: Request):
-            return await self.get_init_data(request)
-
-        return route
-
-    @property
-    def route_submit(self):
-        async def route(request: Request, data: self.schema):  # type:ignore
-            return await self.handle(request, data)  # type:ignore
-
-        return route
-
-    async def handle(self, request: Request, data: SchemaUpdateT, **kwargs) -> BaseApiOut[Any]:
-        raise NotImplementedError
-
-    async def has_action_permission(self, request: Request, name: str) -> bool:
-        return await self.has_page_permission(request, action=name)
-
-
-class ModelAdmin(SqlalchemyCrud, BaseActionAdmin):
-    list_display: List[Union[SqlaField, TableColumn]] = []  # Fields to be displayed
-    list_filter: List[Union[SqlaField, FormItem]] = []  # Query filterable fields
-    list_per_page: int = 10  # Amount of data per page
-    link_model_fields: List[InstrumentedAttribute] = []  # inline field
-    link_model_forms: List[LinkModelForm] = []
-    bulk_update_fields: List[Union[SqlaField, FormItem]] = []  # Bulk edit fields
-    enable_bulk_create: bool = False  # whether to enable batch creation
-    search_fields: List[SqlaField] = []  # fuzzy search fields
-    page_schema: Union[PageSchema, str] = PageSchema()
-    page_path: str = ""
-    bind_model: bool = True
-    admin_action_maker: List[Callable[["ModelAdmin"], "AdminAction"]] = []  # Actions
-    display_item_action_as_column: bool = False  # Whether to display the item operation as a column
-
-    def __init__(self, app: "AdminApp"):
-        assert self.model, "model is None"
-        assert app, "app is None"
-        self.app = app
-        self.engine = self.engine or self.app.engine
-        self.amis_parser = self.app.site.amis_parser
-        self.parser = TableModelParser(self.model)
-        self.schema_model = self.parser.get_table_model_schema(self.model)
-        assert self.schema_model, "schema_model is None"
-        list_display_insfield = self.parser.filter_insfield(self.list_display, save_class=(Label,))
-        self.list_filter = self.list_filter and self.list_filter.copy() or list_display_insfield or []
-        self.list_filter.extend([field for field in self.search_fields if field not in self.list_filter])
-        SqlalchemyCrud.__init__(self, self.model, self.engine)
-        self.fields.extend(list_display_insfield)
-        BaseActionAdmin.__init__(self, app)
-
-    @property
-    def router_prefix(self):
-        if issubclass(self.__class__.__base__, ModelAdmin):
-            return f"/{self.__class__.__name__}"
-        return f"/{self.model.__name__}"
-
-    def get_link_model_forms(self) -> List[LinkModelForm]:
-        self.link_model_forms = list(
-            filter(
-                None,
-                [LinkModelForm.bind_model_admin(self, insfield) for insfield in self.link_model_fields],
-            )
-        )
-        return self.link_model_forms
-
-    async def get_list_display(self, request: Request) -> List[Union[SqlaField, TableColumn]]:
-        return self.list_display or list(model_fields(self.schema_list).values())
-
-    async def get_list_filter(self, request: Request) -> List[Union[SqlaField, FormItem]]:
-        return self.list_filter or list(model_fields(self.schema_filter).values())
-
-    async def get_column_quick_edit(self, request: Request, modelfield: ModelField) -> Optional[Dict[str, Any]]:
-        item = await self.get_form_item(request, modelfield, action=CrudEnum.update)
-        if not isinstance(item, (dict, BaseModel)):
-            return None
-        if isinstance(item, BaseModel):
-            item = item.dict(exclude_none=True, by_alias=True, exclude={"name", "label"})
-        item.update({"saveImmediately": True})
-        if item.get("type") == "switch":
-            item.update({"mode": "inline"})
-        return item
-
-    async def get_list_column(self, request: Request, modelfield: ModelField) -> TableColumn:
-        column = self.amis_parser.as_table_column(modelfield)
-        if await self.has_update_permission(request, None, None) and modelfield.name in model_fields(  # type: ignore
-            self.schema_update
-        ):
-            if column.type == "switch":
-                column.disabled = False
-            column.quickEdit = await self.get_column_quick_edit(request, modelfield)
-        return column
-
-    async def get_list_columns(self, request: Request) -> List[TableColumn]:
-        columns = []
-        for field in await self.get_list_display(request):
-            column = None
-            if isinstance(field, BaseAmisModel):
-                column = field
-            else:
-                modelfield = self.parser.get_modelfield(field)
-                if modelfield:
-                    column = await self.get_list_column(request, modelfield)
-            if column:
-                columns.append(column)
-        return columns
-
-    async def _get_list_columns_for_link_model(self, request) -> List[ColumnOperation]:
-        columns = []
-        for link_form in self.link_model_forms:
-            form = await link_form.get_form_item(request)
-            if not form:
-                continue
-            columns.append(
-                ColumnOperation(
-                    width=160,
-                    label=link_form.display_admin.page_schema.label,
-                    breakpoint="*",
-                    buttons=[form],
-                )
-            )
-        return columns
-
-    async def _get_list_columns_for_actions(self, request) -> List[ColumnOperation]:
-        columns = []
-        actions = await self.get_actions(request, flag="column") or []
-        action_names = {action.name for action in actions}
-        if self.display_item_action_as_column:
-            item_actions = await self.get_actions(request, flag="item") or []
-            actions.extend(action for action in item_actions if action.name not in action_names)
-        if actions:
-            columns.append(
-                ColumnOperation(
-                    fixed="right",
-                    label=_("Operation"),
-                    buttons=actions,
-                )
-            )
-        return columns
-
-    async def get_list_table_api(self, request: Request) -> AmisAPI:
-        api = AmisAPI(
-            method="POST",
-            url=f"{self.router_path}/list?" + "page=${page}&perPage=${perPage}&orderBy=${orderBy}&orderDir=${orderDir}",
-            data={"&": "$$"},
-        )
-        if not await self.has_filter_permission(request, None):
-            return api
-        for field in self.search_fields:
-            alias = self.parser.get_alias(field)
-            if alias:
-                api.data[alias] = f"[~]${alias}"
-        for field in await self.get_list_filter(request):
-            if isinstance(field, FormItem):
-                api.data[field.name] = f"${field.name}"
-            else:
-                modelfield = self.parser.get_modelfield(field)
-                if modelfield and issubclass(modelfield.type_, (datetime.datetime, datetime.date, datetime.time)):
-                    api.data[modelfield.alias] = f"[-]${modelfield.alias}"
-        return api
-
-    async def get_list_table(self, request: Request) -> TableCRUD:
-        headerToolbar = [
-            "filter-toggler",
-            "reload",
-            "bulkActions",
-            {"type": "columns-toggler", "align": "right", "draggable": True},
-            {"type": "drag-toggler", "align": "right"},
-            {"type": "pagination", "align": "right"},
-            {
-                "type": "tpl",
-                "tpl": _("SHOWING ${items|count} OF ${total} RESULT(S)"),
-                "className": "v-middle",
-                "align": "right",
-            },
-        ]
-        headerToolbar.extend(await self.get_actions(request, flag="toolbar"))
-        itemActions = []
-        if not self.display_item_action_as_column:
-            itemActions = await self.get_actions(request, flag="item")
-        filter_form = None
-        if await self.has_filter_permission(request, None):
-            filter_form = await self.get_list_filter_form(request)
-        table = TableCRUD(
-            api=await self.get_list_table_api(request),
-            autoFillHeight=True,
-            headerToolbar=headerToolbar,
-            filterTogglable=True,
-            filterDefaultVisible=False,
-            filter=filter_form,
-            syncLocation=False,
-            keepItemSelectionOnPageChange=True,
-            perPage=self.list_per_page,
-            itemActions=itemActions,
-            bulkActions=await self.get_actions(request, flag="bulk"),
-            footerToolbar=[
-                "statistics",
-                "switch-per-page",
-                "pagination",
-                "load-more",
-                "export-csv",
-                "export-excel",
-            ],
-            columns=await self.get_list_columns(request),
-            primaryField=self.pk_name,
-            quickSaveItemApi=f"put:{self.router_path}/item/${self.pk_name}",
-            defaultParams={k: v for k, v in request.query_params.items() if v},
-        )
-        # Append operation column
-        action_columns = await self._get_list_columns_for_actions(request)
-        table.columns.extend(action_columns)
-        # Append inline link model column
-        link_model_columns = await self._get_list_columns_for_link_model(request)
-        if link_model_columns:
-            table.columns.extend(link_model_columns)
-            table.footable = True
-        return table
-
-    async def get_form_item_on_foreign_key(
-        self, request: Request, modelfield: ModelField, is_filter: bool = False
-    ) -> Union[Service, SchemaNode, None]:
-        column = self.parser.get_column(modelfield.alias)
-        if column is None:
-            return None
-        foreign_keys = list(column.foreign_keys) or None
-        if foreign_keys is None:
-            return None
-        admin = self.app.site.get_model_admin(foreign_keys[0].column.table.name)
-        if not admin:
-            return None
-        url = admin.router_path + admin.page_path
-        label = modelfield.field_info.title or modelfield.name
-        remark = Remark(content=modelfield.field_info.description) if modelfield.field_info.description else None
-        picker = Picker(
-            name=modelfield.alias,
-            label=label,
-            labelField="name",
-            valueField="id",
-            required=(modelfield.required and not is_filter),
-            modalMode="dialog",
-            inline=is_filter,
-            size="full",
-            labelRemark=remark,
-            pickerSchema="${body}",
-            source="${body.api}",
-        )
-        return Service(
-            name=modelfield.alias,
-            schemaApi=AmisAPI(
-                method="post",
-                url=url,
-                data={},
-                cache=300000,
-                responseData={"controls": [picker]},
-            ),
-        )
-
-    async def get_form_item(
-        self, request: Request, modelfield: ModelField, action: CrudEnum
-    ) -> Union[FormItem, SchemaNode, None]:
-        is_filter = True if action in [CrudEnum.filter, CrudEnum.list] else False
-        set_default = action == CrudEnum.create
-        return await self.get_form_item_on_foreign_key(request, modelfield, is_filter=is_filter) or self.amis_parser.as_form_item(
-            modelfield, is_filter=is_filter, set_default=set_default
-        )
-
-    async def get_list_filter_form(self, request: Request) -> Form:
-        body = await self._conv_modelfields_to_formitems(request, await self.get_list_filter(request), CrudEnum.filter)
-        return Form(
-            type="",
-            title=_("Filter"),
-            name=CrudEnum.filter,
-            body=body,
-            mode=DisplayModeEnum.inline,
-            actions=[
-                Action(
-                    actionType="clear-and-submit",
-                    label=_("Clear"),
-                    level=LevelEnum.default,
-                ),
-                Action(
-                    actionType="reset-and-submit",
-                    label=_("Reset"),
-                    level=LevelEnum.default,
-                ),
-                Action(actionType="submit", label=_("Search"), level=LevelEnum.primary),
-            ],
-            trimValues=True,
-        )
-
-    async def get_create_form(self, request: Request, bulk: bool = False) -> Form:
-        fields = [field for field in model_fields(self.schema_create).values() if field.name != self.pk_name]
-        if not bulk:
-            return Form(
-                api=f"post:{self.router_path}/item",
-                name=CrudEnum.create,
-                body=await self._conv_modelfields_to_formitems(request, fields, CrudEnum.create),
-            )
-        columns, keys = [], {}
-        for field in fields:
-            column = await self.get_list_column(request, self.parser.get_modelfield(field))
-            keys[column.name] = "${" + column.label + "}"
-            column.name = column.label
-            columns.append(column)
-        return Form(
-            api=AmisAPI(
-                method="post",
-                url=f"{self.router_path}/item",
-                data={"&": {"$excel": keys}},
-            ),
-            name=CrudEnum.create,
-            mode=DisplayModeEnum.normal,
-            body=[
-                InputExcel(name="excel"),
-                InputTable(
-                    name="excel",
-                    showIndex=True,
-                    columns=columns,
-                    addable=True,
-                    copyable=True,
-                    editable=True,
-                    removable=True,
-                ),
-            ],
-        )
-
-    async def get_update_form(self, request: Request, bulk: bool = False) -> Form:
-        extra = {}
-        if not bulk:
-            api = f"put:{self.router_path}/item/${self.pk_name}"
-            fields = model_fields(self.schema_update).values()
-            if self.schema_read:
-                extra["initApi"] = f"get:{self.router_path}/item/${self.pk_name}"
-        else:
-            api = f"put:{self.router_path}/item/" + "${ids|raw}"
-            fields = self.bulk_update_fields
-        return Form(
-            api=api,
-            name=CrudEnum.update,
-            body=await self._conv_modelfields_to_formitems(request, fields, CrudEnum.update),
-            submitText=None,
-            trimValues=True,
-            **extra,
-        )
-
-    async def get_read_form(self, request: Request) -> Form:
-        return Form(
-            initApi=f"get:{self.router_path}/item/${self.pk_name}",
-            name=CrudEnum.read,
-            body=await self._conv_modelfields_to_formitems(request, model_fields(self.schema_read).values(), CrudEnum.read),
-            submitText=None,
-            static=True,
-        )
-
-    async def get_read_action(self, request: Request) -> Optional[Action]:
-        if not self.schema_read:
-            return None
-        return ActionType.Dialog(
-            icon="fa fa-eye",
-            tooltip=_("View"),
-            dialog=Dialog(
-                title=_("View") + " - " + _(self.page_schema.label),
-                size=SizeEnum.lg,
-                body=await self.get_read_form(request),
-            ),
-        )
-
-    async def get_create_action(self, request: Request, bulk: bool = False) -> Optional[Action]:
-        if not bulk:
-            return ActionType.Dialog(
-                icon="fa fa-plus pull-left",
-                label=_("Create"),
-                level=LevelEnum.primary,
-                dialog=Dialog(
-                    title=_("Create") + " - " + _(self.page_schema.label),
-                    size=SizeEnum.lg,
-                    body=await self.get_create_form(request, bulk=bulk),
-                ),
-            )
-        return ActionType.Dialog(
-            icon="fa fa-plus pull-left",
-            label=_("Bulk Create"),
-            level=LevelEnum.primary,
-            dialog=Dialog(
-                title=_("Bulk Create") + " - " + _(self.page_schema.label),
-                size=SizeEnum.full,
-                body=await self.get_create_form(request, bulk=bulk),
-            ),
-        )
-
-    async def get_update_action(self, request: Request, bulk: bool = False) -> Optional[Action]:
-        if not bulk:
-            return ActionType.Dialog(
-                icon="fa fa-pencil",
-                tooltip=_("Update"),
-                dialog=Dialog(
-                    title=_("Update") + " - " + _(self.page_schema.label),
-                    size=SizeEnum.lg,
-                    body=await self.get_update_form(request, bulk=bulk),
-                ),
-            )
-        elif self.bulk_update_fields:
-            return ActionType.Dialog(
-                label=_("Bulk Update"),
-                dialog=Dialog(
-                    title=_("Bulk Update") + " - " + _(self.page_schema.label),
-                    size=SizeEnum.lg,
-                    body=await self.get_update_form(request, bulk=True),
-                ),
-            )
-        else:
-            return None
-
-    async def _conv_modelfields_to_formitems(
-        self,
-        request: Request,
-        fields: Iterable[Union[SqlaField, ModelField, FormItem]],
-        action: CrudEnum = None,
-    ) -> List[FormItem]:
-        items = []
-        for field in fields:
-            if isinstance(field, FormItem):
-                items.append(field)
-            else:
-                field = self.parser.get_modelfield(field)
-                if field:
-                    item = await self.get_form_item(request, field, action)
-                    if item:
-                        items.append(item)
-        items.sort(key=lambda i: isinstance(i, Service))
-        return items
-
-    @cached_property
-    def registered_admin_actions(self) -> Dict[str, "AdminAction"]:
-        admin_actions = {
-            "create": AdminAction(
-                admin=self,
-                name="create",
-                label=_("Create"),
-                flags=["toolbar"],
-                getter=lambda request: self.get_create_action(request, bulk=False),
-            ),
-            "update": AdminAction(
-                admin=self,
-                name="update",
-                tooltip=_("Update"),
-                flags=["item"],
-                getter=lambda request: self.get_update_action(request, bulk=False),
-            ),
-            "delete": AdminAction(
-                admin=self,
-                name="delete",
-                action=ActionType.Ajax(
-                    icon="fa fa-times text-danger",
-                    tooltip=_("Delete"),
-                    confirmText=_("Are you sure you want to delete row ${%s}?") % self.pk_name,
-                    api=f"delete:{self.router_path}/item/${self.pk_name}",
-                ),
-                flags=["item"],
-            ),
-            "bulk_delete": AdminAction(
-                admin=self,
-                name="bulk_delete",
-                action=ActionType.Ajax(
-                    label=_("Bulk Delete"),
-                    confirmText=_("Are you sure you want to delete the selected rows?"),
-                    api=f"delete:{self.router_path}/item/" + "${ids|raw}",
-                ),
-                flags=["bulk"],
-            ),
-        }
-        if self.enable_bulk_create:
-            admin_actions["bulk_create"] = AdminAction(
-                admin=self,
-                name="bulk_create",
-                label=_("Bulk Create"),
-                flags=["toolbar"],
-                getter=lambda request: self.get_create_action(request, bulk=True),
-            )
-        if self.schema_read:
-            admin_actions["read"] = AdminAction(
-                admin=self,
-                name="read",
-                label=_("View"),
-                flags=["item"],
-                getter=lambda request: self.get_read_action(request),
-            )
-        if self.bulk_update_fields:
-            admin_actions["bulk_update"] = AdminAction(
-                admin=self,
-                name="bulk_update",
-                label=_("Bulk Update"),
-                flags=["bulk"],
-                getter=lambda request: self.get_update_action(request, bulk=True),
-            )
-        for maker in self.admin_action_maker:
-            admin_action = maker(self)
-            admin_actions[admin_action.name] = admin_action
-        return admin_actions
-
-    def register_router(self):
-        for form in self.link_model_forms:
-            form.register_router()
-        self.register_crud()
-        super(ModelAdmin, self).register_router()
-        return self
-
-    async def get_page(self, request: Request) -> Page:
-        page = await super(ModelAdmin, self).get_page(request)
-        page.body = await self.get_list_table(request)
-        return page
-
-    async def has_list_permission(
-        self,
-        request: Request,
-        paginator: Paginator,
-        filters: SchemaFilterT = None,
-        **kwargs,
-    ) -> bool:
-        return await self.has_page_permission(request, action=CrudEnum.list)
-
-    async def has_filter_permission(
-        self,
-        request: Request,
-        filters: Optional[SchemaFilterT],
-        **kwargs,
-    ) -> bool:
-        return await self.has_page_permission(request, action=CrudEnum.filter)
-
-    async def has_create_permission(self, request: Request, data: SchemaCreateT, **kwargs) -> bool:  # type self.schema_create
-        return await self.has_page_permission(request, action=CrudEnum.create)
-
-    async def has_read_permission(self, request: Request, item_id: List[str], **kwargs) -> bool:
-        return await self.has_page_permission(request, action=CrudEnum.read)
-
-    async def has_update_permission(
-        self,
-        request: Request,
-        item_id: List[str],
-        data: SchemaUpdateT,
-        **kwargs,
-    ) -> bool:
-        return await self.has_page_permission(request, action=CrudEnum.update)
-
-    async def has_delete_permission(self, request: Request, item_id: List[str], **kwargs) -> bool:
-        return await self.has_page_permission(request, action=CrudEnum.delete)
-
-    async def has_action_permission(self, request: Request, name: str) -> bool:
-        if not await self.has_page_permission(request, action=name):
-            return False
-        elif name in {"delete", "bulk_delete"}:
-            return await self.has_delete_permission(request, None)  # type: ignore
-        elif name in {"update", "bulk_update"}:
-            return await self.has_update_permission(request, None, None)  # type: ignore
-        elif name in {"create", "bulk_create"}:
-            return await self.has_create_permission(request, None)  # type: ignore
-        elif name in {"read"}:
-            return await self.has_read_permission(request, None)  # type: ignore
-        else:
-            return True
-
-
-class AdminAction:
-    admin: BaseActionAdmin
-    action: Action = Action()
-
-    def __init__(
-        self,
-        admin: BaseActionAdmin,
-        *,
-        name: str = None,
-        label: str = None,
-        action: Action = None,
-        flags: Union[str, List[str]] = None,
-        getter: Callable[[Request], ActionT] = None,
-        **kwargs,
-    ):
-        self.admin = admin
-        assert self.admin, "admin is None"
-        self.action = action or self.action.copy()
-        self.action = self.action.update_from_dict(kwargs)
-        self.name = name or self.action.id or self.action.name
-        assert self.name, "name is None"
-        self.label = label or self.action.label or self.action.tooltip
-        assert self.label, "label is None"
-        self.flags = flags or ["item"]
-        if isinstance(self.flags, str):
-            self.flags = [self.flags]
-        self.getter = getter
-
-    async def get_action(self, request: Request, **kwargs) -> Action:
-        if not self.getter:
-            return self.action
-        action = self.getter(request)
-        if asyncio.iscoroutine(action):
-            action = await action
-        return action
-
-    async def has_page_permission(self, request: Request, obj: "PageSchemaAdmin" = None, action: str = None) -> bool:
-        return await self.admin.has_action_permission(request, name=self.name)
-
-
-class FormAction(AdminAction, FormAdmin):
-    action: Union[ActionType.Dialog, ActionType.Drawer]
-
-    def __init__(
-        self,
-        admin: BaseActionAdmin,
-        *,
-        action: Action = None,
-        flags: List[str] = None,
-        getter: Callable[[BaseActionAdmin, Request], ActionT] = None,
-        **kwargs,
-    ):
-        AdminAction.__init__(self, admin, action=action, flags=flags, getter=getter, **kwargs)
-        self.router = self.admin.router
-        self.schema = self.schema or BaseModel
-        FormAdmin.__init__(self, self.admin.app)
-
-    async def get_action(self, request: Request, **kwargs) -> Action:
-        action = self.action and self.action.copy() or ActionType.Dialog(label=_("Custom form actions"), dialog=Dialog())
-        node: AmisNode = getattr(action, action.actionType, None)
-        if node:
-            node.title = node.title or action.label or action.tooltip  # only override if not set
-            node.size = node.size or SizeEnum.xl
-            node.body = Service(
-                schemaApi=AmisAPI(
-                    method="post",
-                    url=self.router_path + self.page_path,
-                    responseData={
-                        "&": "${body}",
-                        "submitText": "",
-                    },
-                )
-            )
-        return action
-
-    async def handle(self, request: Request, data: SchemaUpdateT, **kwargs) -> BaseApiOut[Any]:
-        return BaseApiOut(data=data)
-
-
-class ModelAction(FormAction):
-    admin: ModelAdmin
-
-    async def get_action(self, request: Request, **kwargs) -> Action:
-        action = await super().get_action(request, **kwargs)
-        node: AmisNode = getattr(action, action.actionType, None)
-        if node:
-            node.body = Service(
-                schemaApi=AmisAPI(
-                    method="post",
-                    url=self.router_path + self.page_path + "?item_id=${IF(ids, ids, id)}",
-                    responseData={
-                        "&": "${body}",
-                        "api.url": "${body.api.url}?item_id=${api.query.item_id}",
-                        "initApi.url": "${body.initApi.url}?item_id=${api.query.item_id}" if self.form_init else None,
-                        "submitText": "",
-                    },
-                )
-            )
-        return action
-
-    # noinspection PyMethodOverriding
-    async def handle(self, request: Request, item_id: List[str], data: Optional[SchemaUpdateT], **kwargs) -> BaseApiOut[Any]:
-        return BaseApiOut(data=data)
-
-    @property
-    def route_submit(self):
-        async def route(
-            request: Request,
-            item_id: self.admin.AnnotatedItemIdList,  # type:ignore
-            data: Annotated[self.schema, Body()] = None,  # type:ignore
-        ):
-            return await self.handle(request, item_id, data)
-
-        return route
-
-
-class AdminGroup(PageSchemaAdmin):
-    def __init__(self, app: "AdminApp") -> None:
-        super().__init__(app)
-        self._children: List[PageSchemaAdminT] = []
-
-    def append_child(self, child: PageSchemaAdminT) -> None:
-        self._children.append(child)
-
-    def remove_child(self, unique_id: str) -> None:
-        self._children = [admin for admin in self._children if admin.unique_id != unique_id]
-        for admin in self._children:
-            if isinstance(admin, AdminGroup):
-                admin.remove_child(unique_id)
-
-    async def get_page_schema_children(self, request: Request) -> List[PageSchema]:
-        page_schema_list = []
-        for child in self._children:
-            if not child.page_schema:
-                continue
-            if (isinstance(child, AdminGroup) and not isinstance(child, AdminApp)) or (
-                isinstance(child, AdminApp) and child.page_schema.tabsMode is None
-            ):
-                sub_children = await child.get_page_schema_children(request)
-                if sub_children:  # If there are sub-nodes, show them even if the parent node has no permission.
-                    page_schema = child.page_schema.copy(deep=True)
-                    page_schema.children = sub_children
-                    page_schema_list.append(page_schema)
-            elif await child.has_page_permission(request, action="page"):
-                page_schema_list.append(child.page_schema)
-        if page_schema_list:
-            page_schema_list.sort(key=lambda p: p.sort or 0, reverse=True)
-        return page_schema_list
-
-    def get_page_schema_child(self, unique_id: str) -> Union[Tuple[PageSchemaAdminT, "AdminGroup"], Tuple[None, None]]:
-        for child in self._children:
-            if child.unique_id == unique_id:
-                return child, self
-            if isinstance(child, AdminGroup):
-                child, parent = child.get_page_schema_child(unique_id)
-                if child:
-                    return child, parent
-        return None, None
-
-    def __iter__(self) -> Iterator[PageSchemaAdminT]:
-        return self._children.__iter__()
-
-
-class AdminApp(PageAdmin, AdminGroup):
-    """Manage applications"""
-
-    engine: SqlalchemyDatabase = None
-    page_path = "/"
-
-    def __init__(self, app: "AdminApp"):
-        PageAdmin.__init__(self, app)
-        AdminGroup.__init__(self, app)
-        self.engine = self.engine or self.app.engine
-        self.db = get_engine_db(self.engine)
-        self._registered: Dict[Type[BaseAdminT], Optional[BaseAdminT]] = {}
-        self.__register_lock = False
-
-    @property
-    def router_prefix(self):
-        return f"/{self.__class__.__name__}"
-
-    def get_admin_or_create(self, admin_cls: Type[BaseAdminT], register: bool = True) -> Optional[BaseAdminT]:
-        if admin_cls not in self._registered and (not register or self.__register_lock):
-            return None
-        admin = self._registered.get(admin_cls)
-        if admin:
-            return admin
-        admin = admin_cls(self)
-        self._registered[admin_cls] = admin
-        if isinstance(admin, PageSchemaAdmin):
-            self.append_child(admin)
-        return admin
-
-    def _create_admin_instance_all(self) -> None:
-        [self.get_admin_or_create(admin_cls) for admin_cls in self._registered.keys()]
-
-    def _register_admin_router_all_pre(self):
-        [admin.get_link_model_forms() for admin in self._registered.values() if isinstance(admin, ModelAdmin)]
-
-    def _register_admin_router_all(self):
-        for admin in self._registered.values():
-            if isinstance(admin, RouterAdmin):  # register route
-                admin.register_router()
-                self.router.include_router(admin.router)
-
-    def register_router(self):
-        if not self.__register_lock:
-            super(AdminApp, self).register_router()
-            self._create_admin_instance_all()
-            self._register_admin_router_all_pre()
-            self._register_admin_router_all()
-            self.__register_lock = True
-        return self
-
-    @lru_cache()  # noqa: B019
-    def get_model_admin(self, table_name: str) -> Optional[ModelAdmin]:
-        for admin_cls, admin in self._registered.items():
-            admin = admin or self.get_admin_or_create(admin_cls)
-            if issubclass(admin_cls, ModelAdmin) and admin.bind_model and admin.model.__table__.name == table_name:
-                return admin
-            elif isinstance(admin, AdminApp) and self.engine is admin.engine:
-                admin = admin.get_model_admin(table_name)
-                if admin:
-                    return admin
-        return None
-
-    def register_admin(self, *admin_cls: Type[BaseAdminT]) -> Type[BaseAdminT]:
-        [self._registered.update({cls: None}) for cls in admin_cls if cls]
-        return admin_cls[0]
-
-    def unregister_admin(self, *admin_cls: Type[BaseAdmin]):
-        [self._registered.pop(cls) for cls in admin_cls if cls]
-
-    def get_page_schema(self) -> Optional[PageSchema]:
-        if super().get_page_schema():
-            if self.page_schema.tabsMode is None:
-                self.page_schema.schemaApi = None
-        return self.page_schema
-
-    async def get_page(self, request: Request) -> Union[Page, App]:
-        if self.page_schema.tabsMode is None:
-            return await self._get_page_as_app(request)
-        return await self._get_page_as_tabs(request)
-
-    async def _get_page_as_app(self, request: Request) -> App:
-        app = App()
-        app.brandName = self.site.settings.site_title
-        app.logo = self.site.settings.site_icon
-        app.header = Tpl(
-            className="w-full",
-            tpl='<div class="flex justify-between"><div></div>'
-            f'<div><a href="{fastapi_amis_admin.__url__}" target="_blank" '
-            'title="Copyright"><i class="fa fa-github fa-2x"></i></a></div></div>',
-        )
-        app.footer = (
-            '<div class="p-2 text-center bg-light">Copyright © 2021 - 2022  '
-            f'<a href="{fastapi_amis_admin.__url__}" target="_blank" '
-            'class="link-secondary">fastapi-amis-admin</a>. All rights reserved. '
-            f'<a target="_blank" href="{fastapi_amis_admin.__url__}" '
-            f'class="link-secondary" rel="noopener">v{fastapi_amis_admin.__version__}</a></div> '
-        )
-        # app.asideBefore = '<div class="p-2 text-center">菜单前面区域</div>'
-        # app.asideAfter = f'<div class="p-2 text-center">' \
-        #                  f'<a href="{fastapi_amis_admin.__url__}"  target="_blank">fastapi-amis-admin</a></div>'
-        children = await self.get_page_schema_children(request)
-        app.pages = [{"children": children}] if children else []
-        return app
-
-    async def _get_page_as_tabs(self, request: Request) -> Page:
-        page = await super(AdminApp, self).get_page(request)
-        children = await self.get_page_schema_children(request)
-        page.body = PageSchema(children=children, tabsMode=self.page_schema.tabsMode).as_page_body()
-        return page
-
-
-class BaseAdminSite(AdminApp):
-    def __init__(
-        self,
-        settings: Settings,
-        fastapi: FastAPI = None,
-        engine: SqlalchemyDatabase = None,
-    ):
-        self.application = None
-        try:
-            from fastapi_user_auth.auth import Auth
-
-            self.auth: Auth = None  # type: ignore
-        except ImportError:
-            pass
-        self.settings = settings
-        self.amis_parser = AmisParser(
-            image_receiver=self.settings.amis_image_receiver,
-            file_receiver=self.settings.amis_file_receiver,
-        )
-        self.fastapi = fastapi or FastAPI(debug=settings.debug, reload=settings.debug)
-        register_exception_handlers(self.fastapi, self.settings.logger)
-        self.router = self.fastapi.router
-        if engine:
-            self.engine = engine
-        elif settings.database_url_async:
-            self.engine = AsyncDatabase.create(settings.database_url_async, echo=settings.debug)
-        elif settings.database_url:
-            self.engine = Database.create(settings.database_url, echo=settings.debug)
-        super().__init__(self)
-
-    @cached_property
-    def router_path(self) -> str:
-        return self.settings.site_url + self.settings.site_path + self.router.prefix
-
-    def mount_app(self, fastapi: FastAPI, name: str = "admin") -> None:
-        """mount app to fastapi, the path is: site.settings.site_path.
-        once mount, the site will create all registered admin instance and register router.
-        """
-        self.application = fastapi
-        self.register_router()
-        fastapi.mount(self.settings.site_path, self.fastapi, name=name)
-        fastapi.add_middleware(BaseHTTPMiddleware, dispatch=self.db.asgi_dispatch)
-        """Add SQLAlchemy Session middleware to the main application, and the session object will be bound to each request.
-        Note:
-        1. The session will be automatically closed when the request ends, so you don't need to close it manually.
-        2. In the sub-application, you can also use this middleware, but you need to pay attention that the session object
-        in the sub-application will be closed in the main application.
-        3. If the sub-application needs to use its own session object, you need to add this middleware to the sub-application.
-        4. Middleware or routes after this middleware can get the session object through `db.session`.
-        """
+import asyncio
+import datetime
+import re
+from functools import lru_cache
+from typing import (
+    Any,
+    Awaitable,
+    Callable,
+    Dict,
+    Generic,
+    Iterable,
+    Iterator,
+    List,
+    Optional,
+    Tuple,
+    Type,
+    TypeVar,
+    Union,
+)
+
+from fastapi import Body, Depends, FastAPI, HTTPException, Request
+from pydantic import BaseModel
+from pydantic.utils import deep_update
+from sqlalchemy import Column, Table, delete, insert
+from sqlalchemy.orm import InstrumentedAttribute, RelationshipProperty
+from sqlalchemy.sql.elements import Label
+from sqlalchemy.util import md5_hex
+from sqlalchemy_database import AsyncDatabase, Database
+from starlette import status
+from starlette.middleware.base import BaseHTTPMiddleware
+from starlette.responses import HTMLResponse, JSONResponse, Response
+from starlette.templating import Jinja2Templates
+from typing_extensions import Annotated, Literal
+
+import fastapi_amis_admin
+from fastapi_amis_admin.admin.handlers import register_exception_handlers
+from fastapi_amis_admin.admin.parser import AmisParser
+from fastapi_amis_admin.admin.settings import Settings
+from fastapi_amis_admin.amis.components import (
+    Action,
+    ActionType,
+    App,
+    ColumnOperation,
+    Dialog,
+    Form,
+    FormItem,
+    Iframe,
+    InputExcel,
+    InputTable,
+    Page,
+    PageSchema,
+    Picker,
+    Remark,
+    Service,
+    TableColumn,
+    TableCRUD,
+    Tpl,
+)
+from fastapi_amis_admin.amis.constants import DisplayModeEnum, LevelEnum, SizeEnum
+from fastapi_amis_admin.amis.types import (
+    AmisAPI,
+    AmisNode,
+    BaseAmisApiOut,
+    BaseAmisModel,
+    SchemaNode,
+)
+from fastapi_amis_admin.crud import RouterMixin, SqlalchemyCrud
+from fastapi_amis_admin.crud.base import SchemaCreateT, SchemaFilterT, SchemaUpdateT
+from fastapi_amis_admin.crud.parser import (
+    SqlaField,
+    TableModelParser,
+    get_python_type_parse,
+)
+from fastapi_amis_admin.crud.schema import BaseApiOut, CrudEnum, Paginator
+from fastapi_amis_admin.crud.utils import (
+    IdStrQuery,
+    SqlalchemyDatabase,
+    get_engine_db,
+    parser_str_set_list,
+)
+from fastapi_amis_admin.utils.functools import cached_property
+from fastapi_amis_admin.utils.pydantic import ModelField, create_model_by_model, model_fields
+from fastapi_amis_admin.utils.translation import i18n as _
+
+BaseAdminT = TypeVar("BaseAdminT", bound="BaseAdmin")
+PageSchemaAdminT = TypeVar("PageSchemaAdminT", bound="PageSchemaAdmin")
+ActionT = Union[Action, Awaitable[Action]]
+
+
+class LinkModelForm:
+    link_model: Table
+
+    def __init__(
+        self,
+        pk_admin: "ModelAdmin",
+        display_admin: "ModelAdmin",
+        link_model: Table,
+        link_col: Column,
+        item_col: Column,
+    ):
+        self.link_model = link_model
+        self.pk_admin = pk_admin
+        self.display_admin = display_admin
+        assert self.display_admin, "display_admin is None"
+        self.link_col = link_col
+        self.item_col = item_col
+        assert self.item_col is not None, "item_col is None"
+        assert self.link_col is not None, "link_col is None"
+        self.path = f"/{self.display_admin.model.__name__}"
+
+    @classmethod
+    def bind_model_admin(cls, pk_admin: "ModelAdmin", insfield: InstrumentedAttribute) -> Optional["LinkModelForm"]:
+        if not isinstance(insfield.property, RelationshipProperty):
+            return None
+        table = insfield.property.secondary
+        if table is None:
+            return None
+        admin = None
+        link_key = None
+        item_key = None
+        for key in table.foreign_keys:
+            if key.column.table != pk_admin.model.__table__:  # Get the associated third-party table
+                admin = pk_admin.app.site.get_model_admin(key.column.table.name)
+                link_key = key
+            else:
+                item_key = key
+        if admin and link_key and item_key:
+            admin.link_models[pk_admin.model.__table__.name] = (table, link_key.parent, item_key.parent)
+            return LinkModelForm(
+                pk_admin=pk_admin,
+                display_admin=admin,
+                link_model=table,
+                link_col=link_key.parent,
+                item_col=item_key.parent,
+            )
+        return None
+
+    @property
+    def route_delete(self):
+        async def route(
+            request: Request,
+            link_id: IdStrQuery,
+            item_id: self.pk_admin.AnnotatedItemIdList,  # type: ignore
+        ):
+            if not await self.pk_admin.has_update_permission(request, item_id, None):
+                return self.pk_admin.error_no_router_permission(request)
+            stmt = (
+                delete(self.link_model)
+                .where(self.link_col.in_(list(map(get_python_type_parse(self.link_col), parser_str_set_list(link_id)))))
+                .where(self.item_col.in_(list(map(get_python_type_parse(self.item_col), item_id))))
+            )
+            result = await self.pk_admin.db.async_execute(stmt)
+            return BaseApiOut(data=result.rowcount)  # type: ignore
+
+        return route
+
+    @property
+    def route_create(self):
+        async def route(
+            request: Request,
+            link_id: IdStrQuery,
+            item_id: self.pk_admin.AnnotatedItemIdList,  # type: ignore
+        ):
+            if not await self.pk_admin.has_update_permission(request, item_id, None):
+                return self.pk_admin.error_no_router_permission(request)
+            values = []
+            for item in map(get_python_type_parse(self.item_col), item_id):
+                values.extend(
+                    {self.link_col.key: link, self.item_col.key: item}
+                    for link in map(get_python_type_parse(self.link_col), parser_str_set_list(link_id))
+                )
+            stmt = insert(self.link_model).values(values)
+            try:
+                result = await self.pk_admin.db.async_execute(stmt)
+            except Exception as error:
+                return self.pk_admin.error_execute_sql(request=request, error=error)
+            return BaseApiOut(data=result.rowcount)  # type: ignore
+
+        return route
+
+    async def get_form_item(self, request: Request):
+        url = self.display_admin.router_path + self.display_admin.page_path
+        picker = Picker(
+            name=self.display_admin.model.__table__.name,
+            label=self.display_admin.page_schema.label,
+            labelField="name",
+            valueField="id",
+            multiple=True,
+            required=False,
+            modalMode="dialog",
+            size="full",
+            pickerSchema={"&": "${body}"},
+            source={
+                "method": "post",
+                "data": "${body.api.data}",
+                "url": "${body.api.url}&link_model=" + self.pk_admin.model.__table__.name + "&op=in_&link_item_id=${"
+                "api.qsOptions.id}",
+            },
+        )
+        adaptor = None
+        if await self.pk_admin.has_update_permission(request, None, None):
+            button_create = ActionType.Ajax(
+                actionType="ajax",
+                label=_("Add Association"),
+                level=LevelEnum.danger,
+                confirmText=_("Are you sure you want to add the association?"),
+                api=f"post:{self.pk_admin.app.router_path}{self.pk_admin.router.prefix}{self.path}"
+                + '/${REPLACE(query.link_item_id, "!", "")}?link_id=${IF(ids, ids, id)}',
+            )  # query.link_item_id
+            adaptor = (
+                'if(!payload.hasOwnProperty("_payload")){payload._payload=JSON.stringify(payload);}'
+                "payload=JSON.parse(payload._payload);button_create=" + button_create.amis_json() + ";"
+                "payload.data.body.bulkActions.push(button_create);"
+                "payload.data.body.itemActions.push(button_create);"
+                "return payload;".replace("action_id", "create" + self.path.replace("/", "_"))
+            )
+            button_create_dialog = ActionType.Dialog(
+                icon="fa fa-plus pull-left",
+                label=_("Add Association"),
+                level=LevelEnum.danger,
+                dialog=Dialog(
+                    title=_("Add Association"),
+                    size="full",
+                    body=Service(
+                        schemaApi=AmisAPI(
+                            method="post",
+                            url=url,
+                            data={},
+                            cache=300000,
+                            responseData={
+                                "&": "${body}",
+                                "api.url": "${body.api.url}&op=not_in&link_model="
+                                + self.pk_admin.model.__table__.name
+                                + "&link_item_id=${api.qsOptions.id}",
+                            },
+                            qsOptions={"id": f"${self.pk_admin.pk_name}"},
+                            adaptor=adaptor,
+                        )
+                    ),
+                ),
+            )
+
+            button_delete = ActionType.Ajax(
+                actionType="ajax",
+                label=_("Remove Association"),
+                level=LevelEnum.danger,
+                confirmText=_("Are you sure you want to remove the association?"),
+                api=f"delete:{self.pk_admin.app.router_path}{self.pk_admin.router.prefix}{self.path}"
+                + "/${query.link_item_id}?link_id=${IF(ids, ids, id)}",
+            )
+            adaptor = (
+                'if(!payload.hasOwnProperty("_payload")){payload._payload=JSON.stringify(payload);}'
+                "payload=JSON.parse(payload._payload);button_delete="
+                + button_delete.amis_json()
+                + ";payload.data.body.headerToolbar.push("
+                + button_create_dialog.amis_json()
+                + ");payload.data.body.bulkActions.push(button_delete);payload.data.body.itemActions.push(button_delete);"
+                "return payload;".replace("action_id", "delete" + self.path.replace("/", "_"))
+            )
+        return Service(
+            schemaApi=AmisAPI(
+                method="post",
+                url=url,
+                data={},
+                cache=300000,
+                responseData={"controls": [picker]},
+                qsOptions={"id": f"${self.pk_admin.pk_name}"},
+                adaptor=adaptor,
+            )
+        )
+
+    def register_router(self):
+        self.pk_admin.router.add_api_route(
+            self.path + "/{item_id}",
+            self.route_delete,
+            methods=["DELETE"],
+            response_model=BaseApiOut[int],
+            name=f"{self.link_model.name}_Delete",
+        )
+
+        self.pk_admin.router.add_api_route(
+            self.path + "/{item_id}",
+            self.route_create,
+            methods=["POST"],
+            response_model=BaseApiOut[int],
+            name=f"{self.link_model.name}_Create",
+        )
+
+        return self
+
+
+class BaseAdmin:
+    def __init__(self, app: "AdminApp"):
+        self.app = app
+        assert self.app, "app is None"
+
+    @cached_property
+    def site(self) -> "BaseAdminSite":
+        return self if self.app is self else self.app.site
+
+    @cached_property
+    def unique_id(self) -> str:
+        unique_str = f"{self.__class__.__module__}:{self.__class__.__qualname__}"
+        if self.app is not self:
+            unique_str += f"{self.app.unique_id}"
+        return md5_hex(unique_str)[:16]
+
+
+class PageSchemaAdmin(BaseAdmin):
+    page_schema: Union[PageSchema, str] = PageSchema()
+
+    def __init__(self, app: "AdminApp"):
+        super().__init__(app)
+        self.page_schema = self.get_page_schema()
+        if self.page_schema and self.page_schema.url:
+            self.page_schema.url = self.page_schema.url.replace(self.site.settings.site_url, "")
+
+    async def has_page_permission(self, request: Request, obj: "PageSchemaAdmin" = None, action: str = None) -> bool:
+        return self.app is self or await self.app.has_page_permission(request, obj=obj or self, action=action)
+
+    def get_page_schema(self) -> Optional[PageSchema]:
+        if self.page_schema:
+            if isinstance(self.page_schema, str):
+                self.page_schema = PageSchema(label=self.page_schema)
+            elif isinstance(self.page_schema, PageSchema):
+                self.page_schema = self.page_schema.copy(deep=True)
+                self.page_schema.label = self.page_schema.label or self.__class__.__name__
+            else:
+                raise TypeError()
+        return self.page_schema
+
+
+class LinkAdmin(PageSchemaAdmin):
+    link: str = ""
+
+    def get_page_schema(self) -> Optional[PageSchema]:
+        if super().get_page_schema():
+            assert self.link, "link is None"
+            self.page_schema.link = self.page_schema.link or self.link
+        return self.page_schema
+
+
+class IframeAdmin(PageSchemaAdmin):
+    iframe: Iframe = None
+    src: str = ""
+
+    def get_page_schema(self) -> Optional[PageSchema]:
+        if super().get_page_schema():
+            assert self.src, "src is None"
+            iframe = self.iframe or Iframe(src=self.src)
+            if self.site.settings.site_url and iframe.src.startswith(self.site.settings.site_url):
+                self.page_schema.url = iframe.src
+            else:
+                self.page_schema.url = re.sub(r"^https?:", "", iframe.src)
+            self.page_schema.schema_ = iframe
+        return self.page_schema
+
+
+class RouterAdmin(BaseAdmin, RouterMixin):
+    def __init__(self, app: "AdminApp"):
+        BaseAdmin.__init__(self, app)
+        RouterMixin.__init__(self)
+
+    def register_router(self):
+        raise NotImplementedError()
+
+    @cached_property
+    def router_path(self) -> str:
+        if self.router is self.app.router:
+            return self.app.router_path
+        return self.app.router_path + self.router.prefix
+
+
+class PageAdmin(PageSchemaAdmin, RouterAdmin):
+    """Amis page management"""
+
+    page: Page = None
+    page_path: Optional[str] = None
+    page_parser_mode: Literal["json", "html"] = "json"
+    page_route_kwargs: Dict[str, Any] = {}
+    template_name: str = ""
+    router_prefix = "/page"
+
+    def __init__(self, app: "AdminApp"):
+        RouterAdmin.__init__(self, app)
+        if self.page_path is None:
+            self.page_path = f"/{self.__class__.__module__}/{self.__class__.__name__}"
+        PageSchemaAdmin.__init__(self, app)
+
+    async def page_permission_depend(self, request: Request) -> bool:
+        return await self.has_page_permission(request, action="page") or self.error_no_page_permission(request)
+
+    def error_no_page_permission(self, request: Request):
+        raise HTTPException(
+            status_code=status.HTTP_307_TEMPORARY_REDIRECT,
+            detail="No page permissions",
+            headers={
+                "location": f"{self.site.router_path}{self.site.router.url_path_for('login')}?redirect={request.url.path}",
+            },
+        )
+
+    async def get_page(self, request: Request) -> Page:
+        return self.page or Page()
+
+    def get_page_schema(self) -> Optional[PageSchema]:
+        if super().get_page_schema():
+            self.page_schema.url = f"{self.router_path}{self.page_path}"
+            self.page_schema.schemaApi = AmisAPI(
+                method="post",
+                url=f"{self.router_path}{self.page_path}",
+                data={},
+                cache=300000,
+            )
+            if self.page_parser_mode == "html":
+                self.page_schema.schema_ = Iframe(src=self.page_schema.url)
+        return self.page_schema
+
+    async def page_parser(self, request: Request, page: Page) -> Response:
+        if request.method == "GET":
+            result = page.amis_html(
+                template_path=self.template_name,
+                locale=_.get_language(),
+                cdn=self.site.settings.amis_cdn,
+                pkg=self.site.settings.amis_pkg,
+                theme=self.site.settings.amis_theme,
+                site_title=self.site.settings.site_title,
+                site_icon=self.site.settings.site_icon,
+            )
+            result = HTMLResponse(result)
+        else:
+            data = page.amis_dict()
+            if await request.body():
+                data = deep_update(data, (await request.json()).get("_update", {}))
+            result = BaseAmisApiOut(data=data)
+            result = JSONResponse(result.dict())
+        return result
+
+    def register_router(self):
+        self.router.add_api_route(
+            self.page_path,
+            self.route_page,
+            methods=["GET"],
+            dependencies=[Depends(self.page_permission_depend)],
+            include_in_schema=False,
+            response_class=HTMLResponse,
+            **self.page_route_kwargs,
+        )
+        self.router.add_api_route(
+            self.page_path,
+            self.route_page,
+            methods=["POST"],
+            dependencies=[Depends(self.page_permission_depend)],
+            response_model=BaseAmisApiOut,
+            include_in_schema=(self.page_parser_mode == "json"),
+            **self.page_route_kwargs,
+        )
+        return self
+
+    @property
+    def AnnotatedPage(self):
+        """Annotated Page, for fastapi dependency injection"""
+        return Annotated[Page, Depends(self.get_page)]
+
+    @property
+    def route_page(self) -> Callable:
+        async def route(
+            request: Request,
+            page: self.AnnotatedPage,  # type:ignore
+        ):
+            return await self.page_parser(request, page)
+
+        return route
+
+
+class TemplateAdmin(PageAdmin):
+    """Jinja2 render template management"""
+
+    page: Dict[str, Any] = {}
+    page_parser_mode = "html"
+    templates: Jinja2Templates = None
+
+    def __init__(self, app: "AdminApp"):
+        assert self.templates, "templates:Jinja2Templates is None"
+        assert self.template_name, "template_name is None"
+        self.page_path = self.page_path or f"/{self.template_name}"
+        super().__init__(app)
+
+    async def page_parser(self, request: Request, page: Dict[str, Any]) -> Response:
+        page["request"] = request
+        return self.templates.TemplateResponse(self.template_name, page)
+
+    async def get_page(self, request: Request) -> Dict[str, Any]:
+        return {}
+
+
+class BaseActionAdmin(PageAdmin):
+    admin_action_maker: List[Callable[["BaseActionAdmin"], "AdminAction"]] = []  # Actions
+
+    @cached_property
+    def registered_admin_actions(self) -> Dict[str, "AdminAction"]:
+        admin_actions = {}
+        for maker in self.admin_action_maker:
+            admin_action = maker(self)
+            if admin_action:
+                admin_actions[admin_action.name] = admin_action
+        return admin_actions
+
+    async def get_action(self, request: Request, name: str) -> Action:
+        admin_action = self.registered_admin_actions.get(name)
+        return await admin_action.get_action(request)
+
+    async def get_actions(self, request: Request, flag: str) -> List[Action]:
+        actions = []
+        for admin_action in self.registered_admin_actions.values():
+            if flag not in admin_action.flags:
+                continue
+            if await self.has_action_permission(request, name=admin_action.name):
+                actions.append(await admin_action.get_action(request, name=admin_action.name))
+        return list(filter(None, actions))
+
+    async def has_action_permission(self, request: Request, name: str) -> bool:
+        return True
+
+    def register_router(self):
+        for admin_action in self.registered_admin_actions.values():
+            if isinstance(admin_action, RouterAdmin):
+                admin_action.register_router()
+        return super().register_router()
+
+
+class FormAdmin(BaseActionAdmin, Generic[SchemaUpdateT]):
+    schema: Type[SchemaUpdateT] = None
+    schema_init_out: Type[Any] = Any
+    schema_submit_out: Type[Any] = Any
+    form: Form = None
+    form_init: bool = None
+    form_path: str = ""
+    router_prefix: str = "/form"
+
+    def __init__(self, app: "AdminApp"):
+        super().__init__(app)
+        assert self.schema, "schema is None"
+        self.form_path = self.form_path or f"{self.page_path}/api"
+
+    async def get_page(self, request: Request) -> Page:
+        page = await super(FormAdmin, self).get_page(request)
+        page.body = await self.get_form(request)
+        return page
+
+    async def get_form_item(self, request: Request, modelfield: ModelField) -> Union[FormItem, SchemaNode]:
+        return self.site.amis_parser.as_form_item(modelfield, set_default=True)
+
+    async def get_form(self, request: Request) -> Form:
+        form = self.form or Form()
+        form.api = AmisAPI(method="POST", url=f"{self.router_path}{self.form_path}")
+        form.initApi = AmisAPI(method="GET", url=f"{self.router_path}{self.form_path}") if self.form_init else None
+        form.title = ""
+        actions = await self.get_actions(request, flag="item")
+        if actions:
+            form.actions = actions
+        form.body = []
+        for modelfield in model_fields(self.schema).values():
+            formitem = await self.get_form_item(request, modelfield)
+            if formitem:
+                form.body.append(formitem)
+        return form
+
+    def register_router(self):
+        super().register_router()
+        self.router.add_api_route(
+            self.form_path,
+            self.route_submit,
+            methods=["POST"],
+            response_model=BaseApiOut[self.schema_submit_out],
+            dependencies=[Depends(self.page_permission_depend)],
+        )
+        if self.form_init:
+            self.schema_init_out = self.schema_init_out or create_model_by_model(
+                self.schema, f"{self.__class__.__name__}InitOut", set_none=True
+            )
+            self.router.add_api_route(
+                self.form_path,
+                self.route_init,
+                methods=["GET"],
+                response_model=BaseApiOut[self.schema_init_out],
+                dependencies=[Depends(self.page_permission_depend)],
+            )
+        return self
+
+    async def get_init_data(self, request: Request, **kwargs) -> BaseApiOut[Any]:
+        return BaseApiOut()
+
+    @property
+    def route_init(self):
+        async def route(request: Request):
+            return await self.get_init_data(request)
+
+        return route
+
+    @property
+    def route_submit(self):
+        async def route(request: Request, data: self.schema):  # type:ignore
+            return await self.handle(request, data)  # type:ignore
+
+        return route
+
+    async def handle(self, request: Request, data: SchemaUpdateT, **kwargs) -> BaseApiOut[Any]:
+        raise NotImplementedError
+
+    async def has_action_permission(self, request: Request, name: str) -> bool:
+        return await self.has_page_permission(request, action=name)
+
+
+class ModelAdmin(SqlalchemyCrud, BaseActionAdmin):
+    list_display: List[Union[SqlaField, TableColumn]] = []  # Fields to be displayed
+    list_filter: List[Union[SqlaField, FormItem]] = []  # Query filterable fields
+    list_per_page: int = 10  # Amount of data per page
+    link_model_fields: List[InstrumentedAttribute] = []  # inline field
+    link_model_forms: List[LinkModelForm] = []
+    bulk_update_fields: List[Union[SqlaField, FormItem]] = []  # Bulk edit fields
+    enable_bulk_create: bool = False  # whether to enable batch creation
+    search_fields: List[SqlaField] = []  # fuzzy search fields
+    page_schema: Union[PageSchema, str] = PageSchema()
+    page_path: str = ""
+    bind_model: bool = True
+    admin_action_maker: List[Callable[["ModelAdmin"], "AdminAction"]] = []  # Actions
+    display_item_action_as_column: bool = False  # Whether to display the item operation as a column
+
+    def __init__(self, app: "AdminApp"):
+        assert self.model, "model is None"
+        assert app, "app is None"
+        self.app = app
+        self.engine = self.engine or self.app.engine
+        self.amis_parser = self.app.site.amis_parser
+        self.parser = TableModelParser(self.model)
+        self.schema_model = self.parser.get_table_model_schema(self.model)
+        assert self.schema_model, "schema_model is None"
+        list_display_insfield = self.parser.filter_insfield(self.list_display, save_class=(Label,))
+        self.list_filter = self.list_filter and self.list_filter.copy() or list_display_insfield or []
+        self.list_filter.extend([field for field in self.search_fields if field not in self.list_filter])
+        SqlalchemyCrud.__init__(self, self.model, self.engine)
+        self.fields.extend(list_display_insfield)
+        BaseActionAdmin.__init__(self, app)
+
+    @property
+    def router_prefix(self):
+        if issubclass(self.__class__.__base__, ModelAdmin):
+            return f"/{self.__class__.__name__}"
+        return f"/{self.model.__name__}"
+
+    def get_link_model_forms(self) -> List[LinkModelForm]:
+        self.link_model_forms = list(
+            filter(
+                None,
+                [LinkModelForm.bind_model_admin(self, insfield) for insfield in self.link_model_fields],
+            )
+        )
+        return self.link_model_forms
+
+    async def get_list_display(self, request: Request) -> List[Union[SqlaField, TableColumn]]:
+        return self.list_display or list(model_fields(self.schema_list).values())
+
+    async def get_list_filter(self, request: Request) -> List[Union[SqlaField, FormItem]]:
+        return self.list_filter or list(model_fields(self.schema_filter).values())
+
+    async def get_column_quick_edit(self, request: Request, modelfield: ModelField) -> Optional[Dict[str, Any]]:
+        item = await self.get_form_item(request, modelfield, action=CrudEnum.update)
+        if not isinstance(item, (dict, BaseModel)):
+            return None
+        if isinstance(item, BaseModel):
+            item = item.dict(exclude_none=True, by_alias=True, exclude={"name", "label"})
+        item.update({"saveImmediately": True})
+        if item.get("type") == "switch":
+            item.update({"mode": "inline"})
+        return item
+
+    async def get_list_column(self, request: Request, modelfield: ModelField) -> TableColumn:
+        column = self.amis_parser.as_table_column(modelfield)
+        if await self.has_update_permission(request, None, None) and modelfield.name in model_fields(  # type: ignore
+            self.schema_update
+        ):
+            if column.type == "switch":
+                column.disabled = False
+            column.quickEdit = await self.get_column_quick_edit(request, modelfield)
+        return column
+
+    async def get_list_columns(self, request: Request) -> List[TableColumn]:
+        columns = []
+        for field in await self.get_list_display(request):
+            column = None
+            if isinstance(field, BaseAmisModel):
+                column = field
+            else:
+                modelfield = self.parser.get_modelfield(field)
+                if modelfield:
+                    column = await self.get_list_column(request, modelfield)
+            if column:
+                columns.append(column)
+        return columns
+
+    async def _get_list_columns_for_link_model(self, request) -> List[ColumnOperation]:
+        columns = []
+        for link_form in self.link_model_forms:
+            form = await link_form.get_form_item(request)
+            if not form:
+                continue
+            columns.append(
+                ColumnOperation(
+                    width=160,
+                    label=link_form.display_admin.page_schema.label,
+                    breakpoint="*",
+                    buttons=[form],
+                )
+            )
+        return columns
+
+    async def _get_list_columns_for_actions(self, request) -> List[ColumnOperation]:
+        columns = []
+        actions = await self.get_actions(request, flag="column") or []
+        action_names = {action.name for action in actions}
+        if self.display_item_action_as_column:
+            item_actions = await self.get_actions(request, flag="item") or []
+            actions.extend(action for action in item_actions if action.name not in action_names)
+        if actions:
+            columns.append(
+                ColumnOperation(
+                    fixed="right",
+                    label=_("Operation"),
+                    buttons=actions,
+                )
+            )
+        return columns
+
+    async def get_list_table_api(self, request: Request) -> AmisAPI:
+        api = AmisAPI(
+            method="POST",
+            url=f"{self.router_path}/list?" + "page=${page}&perPage=${perPage}&orderBy=${orderBy}&orderDir=${orderDir}",
+            data={"&": "$$"},
+        )
+        if not await self.has_filter_permission(request, None):
+            return api
+        for field in self.search_fields:
+            alias = self.parser.get_alias(field)
+            if alias:
+                api.data[alias] = f"[~]${alias}"
+        for field in await self.get_list_filter(request):
+            if isinstance(field, FormItem):
+                api.data[field.name] = f"${field.name}"
+            else:
+                modelfield = self.parser.get_modelfield(field)
+                if modelfield and issubclass(modelfield.type_, (datetime.datetime, datetime.date, datetime.time)):
+                    api.data[modelfield.alias] = f"[-]${modelfield.alias}"
+        return api
+
+    async def get_list_table(self, request: Request) -> TableCRUD:
+        headerToolbar = [
+            "filter-toggler",
+            "reload",
+            "bulkActions",
+            {"type": "columns-toggler", "align": "right", "draggable": True},
+            {"type": "drag-toggler", "align": "right"},
+            {"type": "pagination", "align": "right"},
+            {
+                "type": "tpl",
+                "tpl": _("SHOWING ${items|count} OF ${total} RESULT(S)"),
+                "className": "v-middle",
+                "align": "right",
+            },
+        ]
+        headerToolbar.extend(await self.get_actions(request, flag="toolbar"))
+        itemActions = []
+        if not self.display_item_action_as_column:
+            itemActions = await self.get_actions(request, flag="item")
+        filter_form = None
+        if await self.has_filter_permission(request, None):
+            filter_form = await self.get_list_filter_form(request)
+        table = TableCRUD(
+            api=await self.get_list_table_api(request),
+            autoFillHeight=True,
+            headerToolbar=headerToolbar,
+            filterTogglable=True,
+            filterDefaultVisible=False,
+            filter=filter_form,
+            syncLocation=False,
+            keepItemSelectionOnPageChange=True,
+            perPage=self.list_per_page,
+            itemActions=itemActions,
+            bulkActions=await self.get_actions(request, flag="bulk"),
+            footerToolbar=[
+                "statistics",
+                "switch-per-page",
+                "pagination",
+                "load-more",
+                "export-csv",
+                "export-excel",
+            ],
+            columns=await self.get_list_columns(request),
+            primaryField=self.pk_name,
+            quickSaveItemApi=f"put:{self.router_path}/item/${self.pk_name}",
+            defaultParams={k: v for k, v in request.query_params.items() if v},
+        )
+        # Append operation column
+        action_columns = await self._get_list_columns_for_actions(request)
+        table.columns.extend(action_columns)
+        # Append inline link model column
+        link_model_columns = await self._get_list_columns_for_link_model(request)
+        if link_model_columns:
+            table.columns.extend(link_model_columns)
+            table.footable = True
+        return table
+
+    async def get_form_item_on_foreign_key(
+        self, request: Request, modelfield: ModelField, is_filter: bool = False
+    ) -> Union[Service, SchemaNode, None]:
+        column = self.parser.get_column(modelfield.alias)
+        if column is None:
+            return None
+        foreign_keys = list(column.foreign_keys) or None
+        if foreign_keys is None:
+            return None
+        admin = self.app.site.get_model_admin(foreign_keys[0].column.table.name)
+        if not admin:
+            return None
+        url = admin.router_path + admin.page_path
+        label = modelfield.field_info.title or modelfield.name
+        remark = Remark(content=modelfield.field_info.description) if modelfield.field_info.description else None
+        picker = Picker(
+            name=modelfield.alias,
+            label=label,
+            labelField="name",
+            valueField="id",
+            required=(modelfield.required and not is_filter),
+            modalMode="dialog",
+            inline=is_filter,
+            size="full",
+            labelRemark=remark,
+            pickerSchema="${body}",
+            source="${body.api}",
+        )
+        return Service(
+            name=modelfield.alias,
+            schemaApi=AmisAPI(
+                method="post",
+                url=url,
+                data={},
+                cache=300000,
+                responseData={"controls": [picker]},
+            ),
+        )
+
+    async def get_form_item(
+        self, request: Request, modelfield: ModelField, action: CrudEnum
+    ) -> Union[FormItem, SchemaNode, None]:
+        is_filter = True if action in [CrudEnum.filter, CrudEnum.list] else False
+        set_default = action == CrudEnum.create
+        return await self.get_form_item_on_foreign_key(request, modelfield, is_filter=is_filter) or self.amis_parser.as_form_item(
+            modelfield, is_filter=is_filter, set_default=set_default
+        )
+
+    async def get_list_filter_form(self, request: Request) -> Form:
+        body = await self._conv_modelfields_to_formitems(request, await self.get_list_filter(request), CrudEnum.filter)
+        return Form(
+            type="",
+            title=_("Filter"),
+            name=CrudEnum.filter,
+            body=body,
+            mode=DisplayModeEnum.inline,
+            actions=[
+                Action(
+                    actionType="clear-and-submit",
+                    label=_("Clear"),
+                    level=LevelEnum.default,
+                ),
+                Action(
+                    actionType="reset-and-submit",
+                    label=_("Reset"),
+                    level=LevelEnum.default,
+                ),
+                Action(actionType="submit", label=_("Search"), level=LevelEnum.primary),
+            ],
+            trimValues=True,
+        )
+
+    async def get_create_form(self, request: Request, bulk: bool = False) -> Form:
+        fields = [field for field in model_fields(self.schema_create).values() if field.name != self.pk_name]
+        if not bulk:
+            return Form(
+                api=f"post:{self.router_path}/item",
+                name=CrudEnum.create,
+                body=await self._conv_modelfields_to_formitems(request, fields, CrudEnum.create),
+            )
+        columns, keys = [], {}
+        for field in fields:
+            column = await self.get_list_column(request, self.parser.get_modelfield(field))
+            keys[column.name] = "${" + column.label + "}"
+            column.name = column.label
+            columns.append(column)
+        return Form(
+            api=AmisAPI(
+                method="post",
+                url=f"{self.router_path}/item",
+                data={"&": {"$excel": keys}},
+            ),
+            name=CrudEnum.create,
+            mode=DisplayModeEnum.normal,
+            body=[
+                InputExcel(name="excel"),
+                InputTable(
+                    name="excel",
+                    showIndex=True,
+                    columns=columns,
+                    addable=True,
+                    copyable=True,
+                    editable=True,
+                    removable=True,
+                ),
+            ],
+        )
+
+    async def get_update_form(self, request: Request, bulk: bool = False) -> Form:
+        extra = {}
+        if not bulk:
+            api = f"put:{self.router_path}/item/${self.pk_name}"
+            fields = model_fields(self.schema_update).values()
+            if self.schema_read:
+                extra["initApi"] = f"get:{self.router_path}/item/${self.pk_name}"
+        else:
+            api = f"put:{self.router_path}/item/" + "${ids|raw}"
+            fields = self.bulk_update_fields
+        return Form(
+            api=api,
+            name=CrudEnum.update,
+            body=await self._conv_modelfields_to_formitems(request, fields, CrudEnum.update),
+            submitText=None,
+            trimValues=True,
+            **extra,
+        )
+
+    async def get_read_form(self, request: Request) -> Form:
+        return Form(
+            initApi=f"get:{self.router_path}/item/${self.pk_name}",
+            name=CrudEnum.read,
+            body=await self._conv_modelfields_to_formitems(request, model_fields(self.schema_read).values(), CrudEnum.read),
+            submitText=None,
+            static=True,
+        )
+
+    async def get_read_action(self, request: Request) -> Optional[Action]:
+        if not self.schema_read:
+            return None
+        return ActionType.Dialog(
+            icon="fa fa-eye",
+            tooltip=_("View"),
+            dialog=Dialog(
+                title=_("View") + " - " + _(self.page_schema.label),
+                size=SizeEnum.lg,
+                body=await self.get_read_form(request),
+            ),
+        )
+
+    async def get_create_action(self, request: Request, bulk: bool = False) -> Optional[Action]:
+        if not bulk:
+            return ActionType.Dialog(
+                icon="fa fa-plus pull-left",
+                label=_("Create"),
+                level=LevelEnum.primary,
+                dialog=Dialog(
+                    title=_("Create") + " - " + _(self.page_schema.label),
+                    size=SizeEnum.lg,
+                    body=await self.get_create_form(request, bulk=bulk),
+                ),
+            )
+        return ActionType.Dialog(
+            icon="fa fa-plus pull-left",
+            label=_("Bulk Create"),
+            level=LevelEnum.primary,
+            dialog=Dialog(
+                title=_("Bulk Create") + " - " + _(self.page_schema.label),
+                size=SizeEnum.full,
+                body=await self.get_create_form(request, bulk=bulk),
+            ),
+        )
+
+    async def get_update_action(self, request: Request, bulk: bool = False) -> Optional[Action]:
+        if not bulk:
+            return ActionType.Dialog(
+                icon="fa fa-pencil",
+                tooltip=_("Update"),
+                dialog=Dialog(
+                    title=_("Update") + " - " + _(self.page_schema.label),
+                    size=SizeEnum.lg,
+                    body=await self.get_update_form(request, bulk=bulk),
+                ),
+            )
+        elif self.bulk_update_fields:
+            return ActionType.Dialog(
+                label=_("Bulk Update"),
+                dialog=Dialog(
+                    title=_("Bulk Update") + " - " + _(self.page_schema.label),
+                    size=SizeEnum.lg,
+                    body=await self.get_update_form(request, bulk=True),
+                ),
+            )
+        else:
+            return None
+
+    async def _conv_modelfields_to_formitems(
+        self,
+        request: Request,
+        fields: Iterable[Union[SqlaField, ModelField, FormItem]],
+        action: CrudEnum = None,
+    ) -> List[FormItem]:
+        items = []
+        for field in fields:
+            if isinstance(field, FormItem):
+                items.append(field)
+            else:
+                field = self.parser.get_modelfield(field)
+                if field:
+                    item = await self.get_form_item(request, field, action)
+                    if item:
+                        items.append(item)
+        items.sort(key=lambda i: isinstance(i, Service))
+        return items
+
+    @cached_property
+    def registered_admin_actions(self) -> Dict[str, "AdminAction"]:
+        admin_actions = {
+            "create": AdminAction(
+                admin=self,
+                name="create",
+                label=_("Create"),
+                flags=["toolbar"],
+                getter=lambda request: self.get_create_action(request, bulk=False),
+            ),
+            "update": AdminAction(
+                admin=self,
+                name="update",
+                tooltip=_("Update"),
+                flags=["item"],
+                getter=lambda request: self.get_update_action(request, bulk=False),
+            ),
+            "delete": AdminAction(
+                admin=self,
+                name="delete",
+                action=ActionType.Ajax(
+                    icon="fa fa-times text-danger",
+                    tooltip=_("Delete"),
+                    confirmText=_("Are you sure you want to delete row ${%s}?") % self.pk_name,
+                    api=f"delete:{self.router_path}/item/${self.pk_name}",
+                ),
+                flags=["item"],
+            ),
+            "bulk_delete": AdminAction(
+                admin=self,
+                name="bulk_delete",
+                action=ActionType.Ajax(
+                    label=_("Bulk Delete"),
+                    confirmText=_("Are you sure you want to delete the selected rows?"),
+                    api=f"delete:{self.router_path}/item/" + "${ids|raw}",
+                ),
+                flags=["bulk"],
+            ),
+        }
+        if self.enable_bulk_create:
+            admin_actions["bulk_create"] = AdminAction(
+                admin=self,
+                name="bulk_create",
+                label=_("Bulk Create"),
+                flags=["toolbar"],
+                getter=lambda request: self.get_create_action(request, bulk=True),
+            )
+        if self.schema_read:
+            admin_actions["read"] = AdminAction(
+                admin=self,
+                name="read",
+                label=_("View"),
+                flags=["item"],
+                getter=lambda request: self.get_read_action(request),
+            )
+        if self.bulk_update_fields:
+            admin_actions["bulk_update"] = AdminAction(
+                admin=self,
+                name="bulk_update",
+                label=_("Bulk Update"),
+                flags=["bulk"],
+                getter=lambda request: self.get_update_action(request, bulk=True),
+            )
+        for maker in self.admin_action_maker:
+            admin_action = maker(self)
+            admin_actions[admin_action.name] = admin_action
+        return admin_actions
+
+    def register_router(self):
+        for form in self.link_model_forms:
+            form.register_router()
+        self.register_crud()
+        super(ModelAdmin, self).register_router()
+        return self
+
+    async def get_page(self, request: Request) -> Page:
+        page = await super(ModelAdmin, self).get_page(request)
+        page.body = await self.get_list_table(request)
+        return page
+
+    async def has_list_permission(
+        self,
+        request: Request,
+        paginator: Paginator,
+        filters: SchemaFilterT = None,
+        **kwargs,
+    ) -> bool:
+        return await self.has_page_permission(request, action=CrudEnum.list)
+
+    async def has_filter_permission(
+        self,
+        request: Request,
+        filters: Optional[SchemaFilterT],
+        **kwargs,
+    ) -> bool:
+        return await self.has_page_permission(request, action=CrudEnum.filter)
+
+    async def has_create_permission(self, request: Request, data: SchemaCreateT, **kwargs) -> bool:  # type self.schema_create
+        return await self.has_page_permission(request, action=CrudEnum.create)
+
+    async def has_read_permission(self, request: Request, item_id: List[str], **kwargs) -> bool:
+        return await self.has_page_permission(request, action=CrudEnum.read)
+
+    async def has_update_permission(
+        self,
+        request: Request,
+        item_id: List[str],
+        data: SchemaUpdateT,
+        **kwargs,
+    ) -> bool:
+        return await self.has_page_permission(request, action=CrudEnum.update)
+
+    async def has_delete_permission(self, request: Request, item_id: List[str], **kwargs) -> bool:
+        return await self.has_page_permission(request, action=CrudEnum.delete)
+
+    async def has_action_permission(self, request: Request, name: str) -> bool:
+        if not await self.has_page_permission(request, action=name):
+            return False
+        elif name in {"delete", "bulk_delete"}:
+            return await self.has_delete_permission(request, None)  # type: ignore
+        elif name in {"update", "bulk_update"}:
+            return await self.has_update_permission(request, None, None)  # type: ignore
+        elif name in {"create", "bulk_create"}:
+            return await self.has_create_permission(request, None)  # type: ignore
+        elif name in {"read"}:
+            return await self.has_read_permission(request, None)  # type: ignore
+        else:
+            return True
+
+
+class AdminAction:
+    admin: BaseActionAdmin
+    action: Action = Action()
+
+    def __init__(
+        self,
+        admin: BaseActionAdmin,
+        *,
+        name: str = None,
+        label: str = None,
+        action: Action = None,
+        flags: Union[str, List[str]] = None,
+        getter: Callable[[Request], ActionT] = None,
+        **kwargs,
+    ):
+        self.admin = admin
+        assert self.admin, "admin is None"
+        self.action = action or self.action.copy()
+        self.action = self.action.update_from_dict(kwargs)
+        self.name = name or self.action.id or self.action.name
+        assert self.name, "name is None"
+        self.label = label or self.action.label or self.action.tooltip
+        assert self.label, "label is None"
+        self.flags = flags or ["item"]
+        if isinstance(self.flags, str):
+            self.flags = [self.flags]
+        self.getter = getter
+
+    async def get_action(self, request: Request, **kwargs) -> Action:
+        if not self.getter:
+            return self.action
+        action = self.getter(request)
+        if asyncio.iscoroutine(action):
+            action = await action
+        return action
+
+    async def has_page_permission(self, request: Request, obj: "PageSchemaAdmin" = None, action: str = None) -> bool:
+        return await self.admin.has_action_permission(request, name=self.name)
+
+
+class FormAction(AdminAction, FormAdmin):
+    action: Union[ActionType.Dialog, ActionType.Drawer]
+
+    def __init__(
+        self,
+        admin: BaseActionAdmin,
+        *,
+        action: Action = None,
+        flags: List[str] = None,
+        getter: Callable[[BaseActionAdmin, Request], ActionT] = None,
+        **kwargs,
+    ):
+        AdminAction.__init__(self, admin, action=action, flags=flags, getter=getter, **kwargs)
+        self.router = self.admin.router
+        self.schema = self.schema or BaseModel
+        FormAdmin.__init__(self, self.admin.app)
+
+    async def get_action(self, request: Request, **kwargs) -> Action:
+        action = self.action and self.action.copy() or ActionType.Dialog(label=_("Custom form actions"), dialog=Dialog())
+        node: AmisNode = getattr(action, action.actionType, None)
+        if node:
+            node.title = node.title or action.label or action.tooltip  # only override if not set
+            node.size = node.size or SizeEnum.xl
+            node.body = Service(
+                schemaApi=AmisAPI(
+                    method="post",
+                    url=self.router_path + self.page_path,
+                    responseData={
+                        "&": "${body}",
+                        "submitText": "",
+                    },
+                )
+            )
+        return action
+
+    async def handle(self, request: Request, data: SchemaUpdateT, **kwargs) -> BaseApiOut[Any]:
+        return BaseApiOut(data=data)
+
+
+class ModelAction(FormAction):
+    admin: ModelAdmin
+
+    async def get_action(self, request: Request, **kwargs) -> Action:
+        action = await super().get_action(request, **kwargs)
+        node: AmisNode = getattr(action, action.actionType, None)
+        if node:
+            node.body = Service(
+                schemaApi=AmisAPI(
+                    method="post",
+                    url=self.router_path + self.page_path + "?item_id=${IF(ids, ids, id)}",
+                    responseData={
+                        "&": "${body}",
+                        "api.url": "${body.api.url}?item_id=${api.query.item_id}",
+                        "initApi.url": "${body.initApi.url}?item_id=${api.query.item_id}" if self.form_init else None,
+                        "submitText": "",
+                    },
+                )
+            )
+        return action
+
+    # noinspection PyMethodOverriding
+    async def handle(self, request: Request, item_id: List[str], data: Optional[SchemaUpdateT], **kwargs) -> BaseApiOut[Any]:
+        return BaseApiOut(data=data)
+
+    @property
+    def route_submit(self):
+        async def route(
+            request: Request,
+            item_id: self.admin.AnnotatedItemIdList,  # type:ignore
+            data: Annotated[self.schema, Body()] = None,  # type:ignore
+        ):
+            return await self.handle(request, item_id, data)
+
+        return route
+
+
+class AdminGroup(PageSchemaAdmin):
+    def __init__(self, app: "AdminApp") -> None:
+        super().__init__(app)
+        self._children: List[PageSchemaAdminT] = []
+
+    def append_child(self, child: PageSchemaAdminT) -> None:
+        self._children.append(child)
+
+    def remove_child(self, unique_id: str) -> None:
+        self._children = [admin for admin in self._children if admin.unique_id != unique_id]
+        for admin in self._children:
+            if isinstance(admin, AdminGroup):
+                admin.remove_child(unique_id)
+
+    async def get_page_schema_children(self, request: Request) -> List[PageSchema]:
+        page_schema_list = []
+        for child in self._children:
+            if not child.page_schema:
+                continue
+            if (isinstance(child, AdminGroup) and not isinstance(child, AdminApp)) or (
+                isinstance(child, AdminApp) and child.page_schema.tabsMode is None
+            ):
+                sub_children = await child.get_page_schema_children(request)
+                if sub_children:  # If there are sub-nodes, show them even if the parent node has no permission.
+                    page_schema = child.page_schema.copy(deep=True)
+                    page_schema.children = sub_children
+                    page_schema_list.append(page_schema)
+            elif await child.has_page_permission(request, action="page"):
+                page_schema_list.append(child.page_schema)
+        if page_schema_list:
+            page_schema_list.sort(key=lambda p: p.sort or 0, reverse=True)
+        return page_schema_list
+
+    def get_page_schema_child(self, unique_id: str) -> Union[Tuple[PageSchemaAdminT, "AdminGroup"], Tuple[None, None]]:
+        for child in self._children:
+            if child.unique_id == unique_id:
+                return child, self
+            if isinstance(child, AdminGroup):
+                child, parent = child.get_page_schema_child(unique_id)
+                if child:
+                    return child, parent
+        return None, None
+
+    def __iter__(self) -> Iterator[PageSchemaAdminT]:
+        return self._children.__iter__()
+
+
+class AdminApp(PageAdmin, AdminGroup):
+    """Manage applications"""
+
+    engine: SqlalchemyDatabase = None
+    page_path = "/"
+
+    def __init__(self, app: "AdminApp"):
+        PageAdmin.__init__(self, app)
+        AdminGroup.__init__(self, app)
+        self.engine = self.engine or self.app.engine
+        self.db = get_engine_db(self.engine)
+        self._registered: Dict[Type[BaseAdminT], Optional[BaseAdminT]] = {}
+        self.__register_lock = False
+
+    @property
+    def router_prefix(self):
+        return f"/{self.__class__.__name__}"
+
+    def get_admin_or_create(self, admin_cls: Type[BaseAdminT], register: bool = True) -> Optional[BaseAdminT]:
+        if admin_cls not in self._registered and (not register or self.__register_lock):
+            return None
+        admin = self._registered.get(admin_cls)
+        if admin:
+            return admin
+        admin = admin_cls(self)
+        self._registered[admin_cls] = admin
+        if isinstance(admin, PageSchemaAdmin):
+            self.append_child(admin)
+        return admin
+
+    def _create_admin_instance_all(self) -> None:
+        [self.get_admin_or_create(admin_cls) for admin_cls in self._registered.keys()]
+
+    def _register_admin_router_all_pre(self):
+        [admin.get_link_model_forms() for admin in self._registered.values() if isinstance(admin, ModelAdmin)]
+
+    def _register_admin_router_all(self):
+        for admin in self._registered.values():
+            if isinstance(admin, RouterAdmin):  # register route
+                admin.register_router()
+                self.router.include_router(admin.router)
+
+    def register_router(self):
+        if not self.__register_lock:
+            super(AdminApp, self).register_router()
+            self._create_admin_instance_all()
+            self._register_admin_router_all_pre()
+            self._register_admin_router_all()
+            self.__register_lock = True
+        return self
+
+    @lru_cache()  # noqa: B019
+    def get_model_admin(self, table_name: str) -> Optional[ModelAdmin]:
+        for admin_cls, admin in self._registered.items():
+            admin = admin or self.get_admin_or_create(admin_cls)
+            if issubclass(admin_cls, ModelAdmin) and admin.bind_model and admin.model.__table__.name == table_name:
+                return admin
+            elif isinstance(admin, AdminApp) and self.engine is admin.engine:
+                admin = admin.get_model_admin(table_name)
+                if admin:
+                    return admin
+        return None
+
+    def register_admin(self, *admin_cls: Type[BaseAdminT]) -> Type[BaseAdminT]:
+        [self._registered.update({cls: None}) for cls in admin_cls if cls]
+        return admin_cls[0]
+
+    def unregister_admin(self, *admin_cls: Type[BaseAdmin]):
+        [self._registered.pop(cls) for cls in admin_cls if cls]
+
+    def get_page_schema(self) -> Optional[PageSchema]:
+        if super().get_page_schema():
+            if self.page_schema.tabsMode is None:
+                self.page_schema.schemaApi = None
+        return self.page_schema
+
+    async def get_page(self, request: Request) -> Union[Page, App]:
+        if self.page_schema.tabsMode is None:
+            return await self._get_page_as_app(request)
+        return await self._get_page_as_tabs(request)
+
+    async def _get_page_as_app(self, request: Request) -> App:
+        app = App()
+        app.brandName = self.site.settings.site_title
+        app.logo = self.site.settings.site_icon
+        app.header = Tpl(
+            className="w-full",
+            tpl='<div class="flex justify-between"><div></div>'
+            f'<div><a href="{fastapi_amis_admin.__url__}" target="_blank" '
+            'title="Copyright"><i class="fa fa-github fa-2x"></i></a></div></div>',
+        )
+        app.footer = (
+            '<div class="p-2 text-center bg-light">Copyright © 2021 - 2022  '
+            f'<a href="{fastapi_amis_admin.__url__}" target="_blank" '
+            'class="link-secondary">fastapi-amis-admin</a>. All rights reserved. '
+            f'<a target="_blank" href="{fastapi_amis_admin.__url__}" '
+            f'class="link-secondary" rel="noopener">v{fastapi_amis_admin.__version__}</a></div> '
+        )
+        # app.asideBefore = '<div class="p-2 text-center">菜单前面区域</div>'
+        # app.asideAfter = f'<div class="p-2 text-center">' \
+        #                  f'<a href="{fastapi_amis_admin.__url__}"  target="_blank">fastapi-amis-admin</a></div>'
+        children = await self.get_page_schema_children(request)
+        app.pages = [{"children": children}] if children else []
+        return app
+
+    async def _get_page_as_tabs(self, request: Request) -> Page:
+        page = await super(AdminApp, self).get_page(request)
+        children = await self.get_page_schema_children(request)
+        page.body = PageSchema(children=children, tabsMode=self.page_schema.tabsMode).as_page_body()
+        return page
+
+
+class BaseAdminSite(AdminApp):
+    def __init__(
+        self,
+        settings: Settings,
+        fastapi: FastAPI = None,
+        engine: SqlalchemyDatabase = None,
+    ):
+        self.application = None
+        try:
+            from fastapi_user_auth.auth import Auth
+
+            self.auth: Auth = None  # type: ignore
+        except ImportError:
+            pass
+        self.settings = settings
+        self.amis_parser = AmisParser(
+            image_receiver=self.settings.amis_image_receiver,
+            file_receiver=self.settings.amis_file_receiver,
+        )
+        self.fastapi = fastapi or FastAPI(debug=settings.debug, reload=settings.debug)
+        register_exception_handlers(self.fastapi, self.settings.logger)
+        self.router = self.fastapi.router
+        if engine:
+            self.engine = engine
+        elif settings.database_url_async:
+            self.engine = AsyncDatabase.create(settings.database_url_async, echo=settings.debug)
+        elif settings.database_url:
+            self.engine = Database.create(settings.database_url, echo=settings.debug)
+        super().__init__(self)
+
+    @cached_property
+    def router_path(self) -> str:
+        return self.settings.site_url + self.settings.site_path + self.router.prefix
+
+    def mount_app(self, fastapi: FastAPI, name: str = "admin") -> None:
+        """mount app to fastapi, the path is: site.settings.site_path.
+        once mount, the site will create all registered admin instance and register router.
+        """
+        self.application = fastapi
+        self.register_router()
+        fastapi.mount(self.settings.site_path, self.fastapi, name=name)
+        fastapi.add_middleware(BaseHTTPMiddleware, dispatch=self.db.asgi_dispatch)
+        """Add SQLAlchemy Session middleware to the main application, and the session object will be bound to each request.
+        Note:
+        1. The session will be automatically closed when the request ends, so you don't need to close it manually.
+        2. In the sub-application, you can also use this middleware, but you need to pay attention that the session object
+        in the sub-application will be closed in the main application.
+        3. If the sub-application needs to use its own session object, you need to add this middleware to the sub-application.
+        4. Middleware or routes after this middleware can get the session object through `db.session`.
+        """
```

### Comparing `fastapi_amis_admin-0.6.3/fastapi_amis_admin/admin/handlers.py` & `fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/admin/handlers.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,95 +1,95 @@
-import logging
-import traceback
-from typing import Union
-
-from fastapi import FastAPI
-from fastapi.exceptions import RequestValidationError
-from fastapi.utils import is_body_allowed_for_status_code
-from pydantic import ValidationError
-from starlette.exceptions import HTTPException
-from starlette.requests import ClientDisconnect, Request
-from starlette.responses import Response
-from starlette.status import (
-    HTTP_417_EXPECTATION_FAILED,
-    HTTP_422_UNPROCESSABLE_ENTITY,
-    HTTP_500_INTERNAL_SERVER_ERROR,
-)
-
-from fastapi_amis_admin.crud import BaseApiOut
-
-try:
-    import ujson
-    from fastapi.responses import UJSONResponse as JSONResponse
-except ImportError:
-    ujson = None
-    from fastapi.responses import JSONResponse
-
-
-def register_exception_handlers(app: FastAPI, logger: logging.Logger = None):
-    """global exception catch"""
-    app.add_exception_handler(
-        ValidationError,
-        handler=log_exception(logging.ERROR, logger)(inner_validation_exception_handler),
-    )
-    app.add_exception_handler(
-        RequestValidationError,
-        handler=log_exception(logging.WARNING, logger)(request_validation_exception_handler),
-    )
-    app.add_exception_handler(HTTPException, handler=http_exception_handler)
-    app.add_exception_handler(Exception, handler=log_exception(logging.ERROR, logger)(all_exception_handler))
-
-
-def log_exception(level: Union[int, str] = logging.ERROR, logger: logging.Logger = None):
-    """The decorator outputs exception information to the log"""
-    logger = logger or logging.getLogger("fastapi_amis_admin")
-
-    def wrapper(func):
-        async def function(request: Request, exc: Exception):
-            if isinstance(
-                exc,
-                (
-                    ClientDisconnect,
-                    Warning,
-                ),
-            ):  # Ignore client disconnection; ignore warnings for now
-                return None
-            logger.log(level, f"Error: {exc}\nTraceback: {traceback.format_exc()}")
-            return await func(request, exc)
-
-        return function
-
-    return wrapper
-
-
-def make_error_response(status: int, msg="", **extra):
-    """Construct an error response"""
-    result = BaseApiOut(status=status, msg=msg, **extra)
-    return JSONResponse(content=result.dict())
-
-
-async def http_exception_handler(request: Request, exc: HTTPException):
-    """http exception"""
-    headers = getattr(exc, "headers", None)
-    if not is_body_allowed_for_status_code(exc.status_code):
-        return Response(status_code=exc.status_code, headers=headers)
-    content = getattr(exc, "content", {"status": exc.status_code, "msg": exc.detail})
-    return JSONResponse(content=content, status_code=exc.status_code, headers=headers)
-
-
-async def request_validation_exception_handler(request: Request, exc: RequestValidationError):
-    """Request parameter validation exception"""
-    return make_error_response(
-        status=HTTP_422_UNPROCESSABLE_ENTITY,
-        body=exc.body,
-        errors=exc.errors(),
-    )
-
-
-async def inner_validation_exception_handler(request: Request, exc: ValidationError):
-    """Internal parameter validation exception"""
-    return make_error_response(status=HTTP_417_EXPECTATION_FAILED, errors=exc.errors())
-
-
-async def all_exception_handler(request: Request, exc: Exception):
-    """All exceptions"""
-    return Response(status_code=HTTP_500_INTERNAL_SERVER_ERROR)
+import logging
+import traceback
+from typing import Union
+
+from fastapi import FastAPI
+from fastapi.exceptions import RequestValidationError
+from fastapi.utils import is_body_allowed_for_status_code
+from pydantic import ValidationError
+from starlette.exceptions import HTTPException
+from starlette.requests import ClientDisconnect, Request
+from starlette.responses import Response
+from starlette.status import (
+    HTTP_417_EXPECTATION_FAILED,
+    HTTP_422_UNPROCESSABLE_ENTITY,
+    HTTP_500_INTERNAL_SERVER_ERROR,
+)
+
+from fastapi_amis_admin.crud import BaseApiOut
+
+try:
+    import ujson
+    from fastapi.responses import UJSONResponse as JSONResponse
+except ImportError:
+    ujson = None
+    from fastapi.responses import JSONResponse
+
+
+def register_exception_handlers(app: FastAPI, logger: logging.Logger = None):
+    """global exception catch"""
+    app.add_exception_handler(
+        ValidationError,
+        handler=log_exception(logging.ERROR, logger)(inner_validation_exception_handler),
+    )
+    app.add_exception_handler(
+        RequestValidationError,
+        handler=log_exception(logging.WARNING, logger)(request_validation_exception_handler),
+    )
+    app.add_exception_handler(HTTPException, handler=http_exception_handler)
+    app.add_exception_handler(Exception, handler=log_exception(logging.ERROR, logger)(all_exception_handler))
+
+
+def log_exception(level: Union[int, str] = logging.ERROR, logger: logging.Logger = None):
+    """The decorator outputs exception information to the log"""
+    logger = logger or logging.getLogger("fastapi_amis_admin")
+
+    def wrapper(func):
+        async def function(request: Request, exc: Exception):
+            if isinstance(
+                exc,
+                (
+                    ClientDisconnect,
+                    Warning,
+                ),
+            ):  # Ignore client disconnection; ignore warnings for now
+                return None
+            logger.log(level, f"Error: {exc}\nTraceback: {traceback.format_exc()}")
+            return await func(request, exc)
+
+        return function
+
+    return wrapper
+
+
+def make_error_response(status: int, msg="", **extra):
+    """Construct an error response"""
+    result = BaseApiOut(status=status, msg=msg, **extra)
+    return JSONResponse(content=result.dict())
+
+
+async def http_exception_handler(request: Request, exc: HTTPException):
+    """http exception"""
+    headers = getattr(exc, "headers", None)
+    if not is_body_allowed_for_status_code(exc.status_code):
+        return Response(status_code=exc.status_code, headers=headers)
+    content = getattr(exc, "content", {"status": exc.status_code, "msg": exc.detail})
+    return JSONResponse(content=content, status_code=exc.status_code, headers=headers)
+
+
+async def request_validation_exception_handler(request: Request, exc: RequestValidationError):
+    """Request parameter validation exception"""
+    return make_error_response(
+        status=HTTP_422_UNPROCESSABLE_ENTITY,
+        body=exc.body,
+        errors=exc.errors(),
+    )
+
+
+async def inner_validation_exception_handler(request: Request, exc: ValidationError):
+    """Internal parameter validation exception"""
+    return make_error_response(status=HTTP_417_EXPECTATION_FAILED, errors=exc.errors())
+
+
+async def all_exception_handler(request: Request, exc: Exception):
+    """All exceptions"""
+    return Response(status_code=HTTP_500_INTERNAL_SERVER_ERROR)
```

### Comparing `fastapi_amis_admin-0.6.3/fastapi_amis_admin/admin/parser.py` & `fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/admin/parser.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,327 +1,327 @@
-import datetime
-from enum import Enum
-from typing import Any, Generator, Iterable, Type, TypeVar, Union
-
-from fastapi._compat import Undefined, field_annotation_is_scalar_sequence, field_annotation_is_sequence
-from pydantic import BaseModel, Json
-from pydantic.utils import deep_update, smart_deepcopy
-
-from fastapi_amis_admin import amis
-from fastapi_amis_admin.amis import AmisNode
-from fastapi_amis_admin.amis.components import (
-    Form,
-    FormItem,
-    InputArray,
-    Remark,
-    TableColumn,
-    Validation,
-)
-from fastapi_amis_admin.amis.constants import LabelEnum
-from fastapi_amis_admin.models.enums import Choices
-from fastapi_amis_admin.utils.pydantic import (
-    PYDANTIC_V2,
-    ModelField,
-    annotation_outer_type,
-    field_allow_none,
-    field_json_schema_extra,
-    field_outer_type,
-    model_config_attr,
-    model_fields,
-    scalar_sequence_inner_type,
-)
-from fastapi_amis_admin.utils.translation import i18n as _
-
-_T = TypeVar("_T")
-
-
-class AmisParser:
-    """AmisParser,used to parse pydantic fields to amis form item or table column.
-    AmisParser can set the default image and file upload receiver.
-    """
-
-    def __init__(
-        self,
-        image_receiver: amis.API = None,
-        file_receiver: amis.API = None,
-    ):
-        """
-        Args:
-            image_receiver: Image upload receiver, used to upload images to a specified location and return the image address
-            file_receiver: File upload receiver, used to upload files to a specified location and return the file address
-        """
-        self.image_receiver = image_receiver
-        self.file_receiver = file_receiver
-
-    def _wrap_form_item(self, formitem: FormItem) -> FormItem:
-        """Wrap formitem, add image and file upload receiver."""
-        if formitem.type == "input-image" and not getattr(formitem, "receiver", None):
-            formitem.receiver = self.image_receiver
-        elif formitem.type == "input-file" and not getattr(formitem, "receiver", None):
-            formitem.receiver = self.file_receiver
-        elif formitem.type == "input-rich-text":
-            formitem.receiver = getattr(formitem, "receiver", None) or self.image_receiver
-            formitem.videoReceiver = getattr(formitem, "videoReceiver", None) or self.file_receiver
-        if formitem.type in {"input-image", "input-file"}:
-            # Add manual input file link component.
-            formitem = amis.Group(
-                name=formitem.name,
-                body=[
-                    formitem,
-                    formitem.copy(
-                        exclude={"maxLength", "receiver"},
-                        update={"type": "input-text"},
-                    ),
-                ],
-            )
-        return formitem
-
-    def as_form_item(self, modelfield: ModelField, set_default: bool = False, is_filter: bool = False) -> FormItem:
-        """
-        Get amis form item from pydantic field.
-        Args:
-            modelfield: pydantic field
-            set_default: Is set default value
-            is_filter: Is filter form
-
-        Returns:
-
-        """
-        formitem = self._get_form_item_from_kwargs(modelfield, is_filter=is_filter)
-        formitem = self.update_common_attrs(modelfield, formitem, set_default=set_default, is_filter=is_filter)
-        return self._wrap_form_item(formitem)
-
-    def as_table_column(self, modelfield: ModelField, quick_edit: bool = False) -> TableColumn:
-        column = self._get_table_column_from_kwargs(modelfield)
-        column = self.update_common_attrs(modelfield, column, set_default=False, is_filter=False)
-        column.sortable = True
-        if column.type in ["switch", "mapping"]:
-            column.sortable = False
-        if quick_edit:
-            column.quickEdit = self.as_form_item(modelfield, set_default=True).dict(
-                exclude_none=True, by_alias=True, exclude={"name", "label"}
-            )
-            column.quickEdit.update({"saveImmediately": True})
-            if column.quickEdit.get("type") == "switch":
-                column.disabled = False
-                column.quickEdit.update({"mode": "inline"})
-        return column
-
-    def as_amis_form(self, model: Type[BaseModel], set_default: bool = False, is_filter: bool = False) -> Form:
-        """Get amis form from pydantic model.
-        Args:
-            model: Pydantic model
-            set_default: Is set default value
-            is_filter: Is filter form
-        Returns:
-            amis.Form
-        """
-        form = amis.Form(title=model_config_attr(model, "title", None), size="lg")  # type: ignore
-        form.body = [
-            self.as_form_item(modelfield, set_default=set_default, is_filter=is_filter)
-            for modelfield in model_fields(model).values()
-        ]
-        # InputSubForm
-        return form
-
-    def update_common_attrs(
-        self,
-        modelfield: ModelField,
-        item: Union[FormItem, TableColumn],
-        set_default: bool = False,
-        is_filter: bool = False,
-    ):
-        """Set common attributes for FormItem and TableColumn."""
-        field_info = modelfield.field_info
-        if not is_filter:
-            if not PYDANTIC_V2:
-                if field_info.max_length:
-                    item.maxLength = field_info.max_length
-                if field_info.min_length:
-                    item.minLength = field_info.min_length
-            type_ = annotation_outer_type(modelfield.type_)
-            item.required = modelfield.required and not issubclass(type_, bool)
-            if set_default and modelfield.default is not Undefined:
-                item.value = modelfield.default
-        item.name = modelfield.alias
-        item.label = _(field_info.title) if field_info.title else _(modelfield.name)  # The use of I18N
-        label_name = "labelRemark" if isinstance(item, FormItem) else "remark"
-        if getattr(item, label_name, None) is None:
-            label = Remark(content=_(field_info.description)) if field_info.description else None  # The use of I18N
-            setattr(item, label_name, label)
-        return item
-
-    def _get_form_item_from_kwargs(self, modelfield: ModelField, is_filter: bool = False) -> FormItem:
-        formitem = self.get_field_amis_extra(modelfield, ["amis_form_item", "amis_filter_item"][is_filter])
-        # List type parse to InputArray
-        outer_type = field_outer_type(modelfield) or modelfield.type_
-        if field_annotation_is_sequence(outer_type):
-            if not isinstance(formitem, FormItem):
-                formitem = InputArray(**formitem)
-            elif not isinstance(formitem, InputArray):
-                return formitem
-            # Parse the internal type of the list.
-            type_ = scalar_sequence_inner_type(outer_type)
-            kwargs = self.get_field_amis_form_item_type(type_=type_, is_filter=is_filter)
-            update = formitem.items.amis_dict() if formitem.items else {}
-            if update:
-                kwargs = deep_update(kwargs, update)
-            formitem.items = FormItem(**kwargs)
-        if isinstance(formitem, FormItem):
-            return formitem
-        # other type parse to FormItem
-        kwargs = self.get_field_amis_form_item_type(
-            type_=modelfield.type_,
-            is_filter=is_filter,
-            required=modelfield.required and not field_allow_none(modelfield),
-        )
-        return FormItem(**kwargs).update_from_dict(formitem)
-
-    def _get_table_column_from_kwargs(self, modelfield: ModelField) -> TableColumn:
-        table_column = self.get_field_amis_extra(modelfield, "amis_table_column")
-        if isinstance(table_column, TableColumn):
-            return table_column
-        kwargs = self.get_field_amis_table_column_type(modelfield.type_)
-        return TableColumn(**kwargs).update_from_dict(table_column)
-
-    def get_field_amis_table_column_type(self, type_: Type) -> dict:
-        """Get amis table column type from pydantic model field type."""
-        kwargs = {}
-        type_ = annotation_outer_type(type_)
-        if type_ in {str, Any}:
-            pass
-        elif issubclass(type_, bool):
-            kwargs["type"] = "switch"
-            kwargs["disabled"] = True
-            kwargs["filterable"] = {
-                "options": [
-                    {"label": _("YES"), "value": True},
-                    {"label": _("NO"), "value": False},
-                ]
-            }
-        elif issubclass(type_, datetime.datetime):
-            kwargs["type"] = "datetime"
-        elif issubclass(type_, datetime.date):
-            kwargs["type"] = "date"
-        elif issubclass(type_, datetime.time):
-            kwargs["type"] = "time"
-        elif issubclass(type_, Enum):
-            items = type_.choices if issubclass(type_, Choices) else [(m.value, m.value) for m in type_]
-            kwargs["type"] = "mapping"
-            kwargs["filterable"] = {"options": [{"label": v, "value": k} for k, v in items]}
-            kwargs["map"] = {
-                k: f"<span class='label label-{label.value}'>{v}</span>"
-                for (k, v), label in zip(items, cyclic_generator(LabelEnum))
-            }
-        elif issubclass(type_, (dict, Json)):
-            kwargs["type"] = "json"
-        elif field_annotation_is_scalar_sequence(type_):
-            kwargs["type"] = "each"
-            kwargs["items"] = {
-                "type": "tpl",
-                "tpl": "<span class='label label-info m-l-sm'><%= this.item %></span>",
-            }
-        return kwargs
-
-    def get_field_amis_form_item_type(self, type_: Any, is_filter: bool, required: bool = False) -> dict:
-        """Get amis form item type from pydantic model field type."""
-        kwargs = {}
-        type_ = annotation_outer_type(type_)
-        if type_ in {str, Any}:
-            kwargs["type"] = "input-text"
-        elif issubclass(type_, Enum):
-            items = type_.choices if issubclass(type_, Choices) else [(m.value, m.value) for m in type_]
-            kwargs.update(
-                {
-                    "type": "select",
-                    "options": [{"label": label, "value": v} for v, label in items],
-                    "extractValue": True,
-                    "joinValues": False,
-                }
-            )
-            if not required or is_filter:
-                kwargs["clearable"] = True
-        elif issubclass(type_, bool):
-            kwargs["type"] = "switch"
-        elif is_filter:
-            if issubclass(type_, datetime.datetime):
-                kwargs["type"] = "input-datetime-range"
-                kwargs["format"] = "YYYY-MM-DD HH:mm:ss"
-                # 给筛选的 DateTimeRange 添加 today 标签
-                kwargs["ranges"] = "today,yesterday,7daysago,prevweek,thismonth,prevmonth,prevquarter"
-            elif issubclass(type_, datetime.date):
-                kwargs["type"] = "input-date-range"
-                kwargs["format"] = "YYYY-MM-DD"
-            elif issubclass(type_, datetime.time):
-                kwargs["type"] = "input-time-range"
-                kwargs["format"] = "HH:mm:ss"
-            else:
-                kwargs["type"] = "input-text"
-        elif issubclass(type_, int):
-            kwargs["type"] = "input-number"
-            kwargs["precision"] = 0
-            kwargs["validations"] = Validation(isInt=True).amis_dict()
-        elif issubclass(type_, float):
-            kwargs["type"] = "input-number"
-            kwargs["precision"] = 3
-            kwargs["validations"] = Validation(isFloat=True).amis_dict()
-        elif issubclass(type_, datetime.datetime):
-            kwargs["type"] = "input-datetime"
-            kwargs["format"] = "YYYY-MM-DD HH:mm:ss"
-        elif issubclass(type_, datetime.date):
-            kwargs["type"] = "input-date"
-            kwargs["format"] = "YYYY-MM-DD"
-        elif issubclass(type_, datetime.time):
-            kwargs["type"] = "input-time"
-            kwargs["format"] = "HH:mm:ss"
-        elif issubclass(type_, (dict, Json)):
-            kwargs["type"] = "json-editor"
-        elif issubclass(type_, BaseModel):
-            # pydantic model parse to InputSubForm
-            kwargs["type"] = "input-sub-form"
-            kwargs["labelField"] = get_model_label_field_name(type_)
-            kwargs["btnLabel"] = model_config_attr(type_, "title", None)
-            kwargs["form"] = self.as_amis_form(type_, is_filter=is_filter).amis_dict()
-        else:
-            kwargs["type"] = "input-text"
-        if kwargs.get("type") == "input-text":
-            kwargs["clearable"] = True
-            kwargs["clearValueOnEmpty"] = True
-        return kwargs
-
-    def get_field_amis_extra(
-        self,
-        modelfield: ModelField,
-        name: str,
-    ) -> Union[FormItem, TableColumn, dict]:
-        """Get amis extra from pydantic model field.
-        You can pass amis configuration through the extra parameter of the pydantic model field.
-        """
-        extra = field_json_schema_extra(modelfield).get(name, {})
-        if not extra:
-            return {}
-        if callable(extra):
-            return extra()
-        extra = smart_deepcopy(extra)
-        if isinstance(extra, (AmisNode, dict)):
-            pass
-        elif isinstance(extra, str):
-            extra = {"type": extra}
-        else:
-            extra = {}
-        return extra
-
-
-def cyclic_generator(iterable: Iterable[_T]) -> Generator[_T, None, None]:
-    while True:
-        yield from iterable
-
-
-def get_model_label_field_name(model: Type[BaseModel]) -> str:
-    """Get model label field name. The label field is used to display the model name in the form."""
-    label_field_name = model_config_attr(model, "label_field_name", None)
-    if label_field_name:
-        return label_field_name
-    for filed in model_fields(model).values():
-        if filed.alias in ["name", "title", "label"]:
-            return filed.alias
-    return "id"
+import datetime
+from enum import Enum
+from typing import Any, Generator, Iterable, Type, TypeVar, Union
+
+from fastapi._compat import Undefined, field_annotation_is_scalar_sequence, field_annotation_is_sequence
+from pydantic import BaseModel, Json
+from pydantic.utils import deep_update, smart_deepcopy
+
+from fastapi_amis_admin import amis
+from fastapi_amis_admin.amis import AmisNode
+from fastapi_amis_admin.amis.components import (
+    Form,
+    FormItem,
+    InputArray,
+    Remark,
+    TableColumn,
+    Validation,
+)
+from fastapi_amis_admin.amis.constants import LabelEnum
+from fastapi_amis_admin.models.enums import Choices
+from fastapi_amis_admin.utils.pydantic import (
+    PYDANTIC_V2,
+    ModelField,
+    annotation_outer_type,
+    field_allow_none,
+    field_json_schema_extra,
+    field_outer_type,
+    model_config_attr,
+    model_fields,
+    scalar_sequence_inner_type,
+)
+from fastapi_amis_admin.utils.translation import i18n as _
+
+_T = TypeVar("_T")
+
+
+class AmisParser:
+    """AmisParser,used to parse pydantic fields to amis form item or table column.
+    AmisParser can set the default image and file upload receiver.
+    """
+
+    def __init__(
+        self,
+        image_receiver: amis.API = None,
+        file_receiver: amis.API = None,
+    ):
+        """
+        Args:
+            image_receiver: Image upload receiver, used to upload images to a specified location and return the image address
+            file_receiver: File upload receiver, used to upload files to a specified location and return the file address
+        """
+        self.image_receiver = image_receiver
+        self.file_receiver = file_receiver
+
+    def _wrap_form_item(self, formitem: FormItem) -> FormItem:
+        """Wrap formitem, add image and file upload receiver."""
+        if formitem.type == "input-image" and not getattr(formitem, "receiver", None):
+            formitem.receiver = self.image_receiver
+        elif formitem.type == "input-file" and not getattr(formitem, "receiver", None):
+            formitem.receiver = self.file_receiver
+        elif formitem.type == "input-rich-text":
+            formitem.receiver = getattr(formitem, "receiver", None) or self.image_receiver
+            formitem.videoReceiver = getattr(formitem, "videoReceiver", None) or self.file_receiver
+        if formitem.type in {"input-image", "input-file"}:
+            # Add manual input file link component.
+            formitem = amis.Group(
+                name=formitem.name,
+                body=[
+                    formitem,
+                    formitem.copy(
+                        exclude={"maxLength", "receiver"},
+                        update={"type": "input-text"},
+                    ),
+                ],
+            )
+        return formitem
+
+    def as_form_item(self, modelfield: ModelField, set_default: bool = False, is_filter: bool = False) -> FormItem:
+        """
+        Get amis form item from pydantic field.
+        Args:
+            modelfield: pydantic field
+            set_default: Is set default value
+            is_filter: Is filter form
+
+        Returns:
+
+        """
+        formitem = self._get_form_item_from_kwargs(modelfield, is_filter=is_filter)
+        formitem = self.update_common_attrs(modelfield, formitem, set_default=set_default, is_filter=is_filter)
+        return self._wrap_form_item(formitem)
+
+    def as_table_column(self, modelfield: ModelField, quick_edit: bool = False) -> TableColumn:
+        column = self._get_table_column_from_kwargs(modelfield)
+        column = self.update_common_attrs(modelfield, column, set_default=False, is_filter=False)
+        column.sortable = True
+        if column.type in ["switch", "mapping"]:
+            column.sortable = False
+        if quick_edit:
+            column.quickEdit = self.as_form_item(modelfield, set_default=True).dict(
+                exclude_none=True, by_alias=True, exclude={"name", "label"}
+            )
+            column.quickEdit.update({"saveImmediately": True})
+            if column.quickEdit.get("type") == "switch":
+                column.disabled = False
+                column.quickEdit.update({"mode": "inline"})
+        return column
+
+    def as_amis_form(self, model: Type[BaseModel], set_default: bool = False, is_filter: bool = False) -> Form:
+        """Get amis form from pydantic model.
+        Args:
+            model: Pydantic model
+            set_default: Is set default value
+            is_filter: Is filter form
+        Returns:
+            amis.Form
+        """
+        form = amis.Form(title=model_config_attr(model, "title", None), size="lg")  # type: ignore
+        form.body = [
+            self.as_form_item(modelfield, set_default=set_default, is_filter=is_filter)
+            for modelfield in model_fields(model).values()
+        ]
+        # InputSubForm
+        return form
+
+    def update_common_attrs(
+        self,
+        modelfield: ModelField,
+        item: Union[FormItem, TableColumn],
+        set_default: bool = False,
+        is_filter: bool = False,
+    ):
+        """Set common attributes for FormItem and TableColumn."""
+        field_info = modelfield.field_info
+        if not is_filter:
+            if not PYDANTIC_V2:
+                if field_info.max_length:
+                    item.maxLength = field_info.max_length
+                if field_info.min_length:
+                    item.minLength = field_info.min_length
+            type_ = annotation_outer_type(modelfield.type_)
+            item.required = modelfield.required and not issubclass(type_, bool)
+            if set_default and modelfield.default is not Undefined:
+                item.value = modelfield.default
+        item.name = modelfield.alias
+        item.label = _(field_info.title) if field_info.title else _(modelfield.name)  # The use of I18N
+        label_name = "labelRemark" if isinstance(item, FormItem) else "remark"
+        if getattr(item, label_name, None) is None:
+            label = Remark(content=_(field_info.description)) if field_info.description else None  # The use of I18N
+            setattr(item, label_name, label)
+        return item
+
+    def _get_form_item_from_kwargs(self, modelfield: ModelField, is_filter: bool = False) -> FormItem:
+        formitem = self.get_field_amis_extra(modelfield, ["amis_form_item", "amis_filter_item"][is_filter])
+        # List type parse to InputArray
+        outer_type = field_outer_type(modelfield) or modelfield.type_
+        if field_annotation_is_sequence(outer_type):
+            if not isinstance(formitem, FormItem):
+                formitem = InputArray(**formitem)
+            elif not isinstance(formitem, InputArray):
+                return formitem
+            # Parse the internal type of the list.
+            type_ = scalar_sequence_inner_type(outer_type)
+            kwargs = self.get_field_amis_form_item_type(type_=type_, is_filter=is_filter)
+            update = formitem.items.amis_dict() if formitem.items else {}
+            if update:
+                kwargs = deep_update(kwargs, update)
+            formitem.items = FormItem(**kwargs)
+        if isinstance(formitem, FormItem):
+            return formitem
+        # other type parse to FormItem
+        kwargs = self.get_field_amis_form_item_type(
+            type_=modelfield.type_,
+            is_filter=is_filter,
+            required=modelfield.required and not field_allow_none(modelfield),
+        )
+        return FormItem(**kwargs).update_from_dict(formitem)
+
+    def _get_table_column_from_kwargs(self, modelfield: ModelField) -> TableColumn:
+        table_column = self.get_field_amis_extra(modelfield, "amis_table_column")
+        if isinstance(table_column, TableColumn):
+            return table_column
+        kwargs = self.get_field_amis_table_column_type(modelfield.type_)
+        return TableColumn(**kwargs).update_from_dict(table_column)
+
+    def get_field_amis_table_column_type(self, type_: Type) -> dict:
+        """Get amis table column type from pydantic model field type."""
+        kwargs = {}
+        type_ = annotation_outer_type(type_)
+        if type_ in {str, Any}:
+            pass
+        elif issubclass(type_, bool):
+            kwargs["type"] = "switch"
+            kwargs["disabled"] = True
+            kwargs["filterable"] = {
+                "options": [
+                    {"label": _("YES"), "value": True},
+                    {"label": _("NO"), "value": False},
+                ]
+            }
+        elif issubclass(type_, datetime.datetime):
+            kwargs["type"] = "datetime"
+        elif issubclass(type_, datetime.date):
+            kwargs["type"] = "date"
+        elif issubclass(type_, datetime.time):
+            kwargs["type"] = "time"
+        elif issubclass(type_, Enum):
+            items = type_.choices if issubclass(type_, Choices) else [(m.value, m.value) for m in type_]
+            kwargs["type"] = "mapping"
+            kwargs["filterable"] = {"options": [{"label": v, "value": k} for k, v in items]}
+            kwargs["map"] = {
+                k: f"<span class='label label-{label.value}'>{v}</span>"
+                for (k, v), label in zip(items, cyclic_generator(LabelEnum))
+            }
+        elif issubclass(type_, (dict, Json)):
+            kwargs["type"] = "json"
+        elif field_annotation_is_scalar_sequence(type_):
+            kwargs["type"] = "each"
+            kwargs["items"] = {
+                "type": "tpl",
+                "tpl": "<span class='label label-info m-l-sm'><%= this.item %></span>",
+            }
+        return kwargs
+
+    def get_field_amis_form_item_type(self, type_: Any, is_filter: bool, required: bool = False) -> dict:
+        """Get amis form item type from pydantic model field type."""
+        kwargs = {}
+        type_ = annotation_outer_type(type_)
+        if type_ in {str, Any}:
+            kwargs["type"] = "input-text"
+        elif issubclass(type_, Enum):
+            items = type_.choices if issubclass(type_, Choices) else [(m.value, m.value) for m in type_]
+            kwargs.update(
+                {
+                    "type": "select",
+                    "options": [{"label": label, "value": v} for v, label in items],
+                    "extractValue": True,
+                    "joinValues": False,
+                }
+            )
+            if not required or is_filter:
+                kwargs["clearable"] = True
+        elif issubclass(type_, bool):
+            kwargs["type"] = "switch"
+        elif is_filter:
+            if issubclass(type_, datetime.datetime):
+                kwargs["type"] = "input-datetime-range"
+                kwargs["format"] = "YYYY-MM-DD HH:mm:ss"
+                # 给筛选的 DateTimeRange 添加 today 标签
+                kwargs["ranges"] = "today,yesterday,7daysago,prevweek,thismonth,prevmonth,prevquarter"
+            elif issubclass(type_, datetime.date):
+                kwargs["type"] = "input-date-range"
+                kwargs["format"] = "YYYY-MM-DD"
+            elif issubclass(type_, datetime.time):
+                kwargs["type"] = "input-time-range"
+                kwargs["format"] = "HH:mm:ss"
+            else:
+                kwargs["type"] = "input-text"
+        elif issubclass(type_, int):
+            kwargs["type"] = "input-number"
+            kwargs["precision"] = 0
+            kwargs["validations"] = Validation(isInt=True).amis_dict()
+        elif issubclass(type_, float):
+            kwargs["type"] = "input-number"
+            kwargs["precision"] = 3
+            kwargs["validations"] = Validation(isFloat=True).amis_dict()
+        elif issubclass(type_, datetime.datetime):
+            kwargs["type"] = "input-datetime"
+            kwargs["format"] = "YYYY-MM-DD HH:mm:ss"
+        elif issubclass(type_, datetime.date):
+            kwargs["type"] = "input-date"
+            kwargs["format"] = "YYYY-MM-DD"
+        elif issubclass(type_, datetime.time):
+            kwargs["type"] = "input-time"
+            kwargs["format"] = "HH:mm:ss"
+        elif issubclass(type_, (dict, Json)):
+            kwargs["type"] = "json-editor"
+        elif issubclass(type_, BaseModel):
+            # pydantic model parse to InputSubForm
+            kwargs["type"] = "input-sub-form"
+            kwargs["labelField"] = get_model_label_field_name(type_)
+            kwargs["btnLabel"] = model_config_attr(type_, "title", None)
+            kwargs["form"] = self.as_amis_form(type_, is_filter=is_filter).amis_dict()
+        else:
+            kwargs["type"] = "input-text"
+        if kwargs.get("type") == "input-text":
+            kwargs["clearable"] = True
+            kwargs["clearValueOnEmpty"] = True
+        return kwargs
+
+    def get_field_amis_extra(
+        self,
+        modelfield: ModelField,
+        name: str,
+    ) -> Union[FormItem, TableColumn, dict]:
+        """Get amis extra from pydantic model field.
+        You can pass amis configuration through the extra parameter of the pydantic model field.
+        """
+        extra = field_json_schema_extra(modelfield).get(name, {})
+        if not extra:
+            return {}
+        if callable(extra):
+            return extra()
+        extra = smart_deepcopy(extra)
+        if isinstance(extra, (AmisNode, dict)):
+            pass
+        elif isinstance(extra, str):
+            extra = {"type": extra}
+        else:
+            extra = {}
+        return extra
+
+
+def cyclic_generator(iterable: Iterable[_T]) -> Generator[_T, None, None]:
+    while True:
+        yield from iterable
+
+
+def get_model_label_field_name(model: Type[BaseModel]) -> str:
+    """Get model label field name. The label field is used to display the model name in the form."""
+    label_field_name = model_config_attr(model, "label_field_name", None)
+    if label_field_name:
+        return label_field_name
+    for filed in model_fields(model).values():
+        if filed.alias in ["name", "title", "label"]:
+            return filed.alias
+    return "id"
```

### Comparing `fastapi_amis_admin-0.6.3/fastapi_amis_admin/admin/settings.py` & `fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/admin/settings.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-import logging
-from typing import Any, Union
-
-from typing_extensions import Literal
-
-from fastapi_amis_admin.amis import API
-from fastapi_amis_admin.utils.pydantic import PYDANTIC_V2, BaseSettings
-
-
-class Settings(BaseSettings):
-    """Project configuration"""
-
-    host: str = "127.0.0.1"
-    port: int = 8000
-    debug: bool = False
-    version: str = "0.0.0"
-    site_title: str = "FastAPI Amis Admin"
-    site_icon: str = "https://baidu.gitee.io/amis/static/favicon_b3b0647.png"
-    site_url: str = ""
-    site_path: str = "/admin"
-    database_url_async: str = ""
-    database_url: str = ""
-    language: Union[Literal["zh_CN", "en_US", "de_DE"], str] = ""
-    amis_cdn: str = "https://unpkg.com"
-    amis_pkg: str = "amis@3.3.0"
-    amis_theme: Literal["cxd", "antd", "dark", "ang"] = "cxd"
-    amis_image_receiver: API = None  # Image upload interface
-    amis_file_receiver: API = None  # File upload interface
-    logger: Union[logging.Logger, Any] = logging.getLogger("fastapi_amis_admin")
-
-    @classmethod
-    def valid_url_(cls, url: str):
-        return url[:-1] if url.endswith("/") else url
-
-    @classmethod
-    def valid_database_url_(cls, values):
-        # set default file upload api.
-        file_upload_api = f"post:{values.get('site_path', '')}/file/upload"
-        values.setdefault("amis_image_receiver", file_upload_api)
-        values.setdefault("amis_file_receiver", file_upload_api)
-        # set default database url.
-        if not values.get("database_url") and not values.get("database_url_async"):
-            values.setdefault(
-                "database_url_async",
-                "sqlite+aiosqlite:///amisadmin.db?check_same_thread=False",
-            )
-        return values
-
-    if PYDANTIC_V2:
-        from pydantic import field_validator, model_validator
-
-        valid_url = field_validator("amis_cdn", "site_path", "site_url", mode="before")(lambda cls, v: cls.valid_url_(v))
-        valid_database_url = model_validator(mode="before")(lambda cls, values: cls.valid_database_url_(values))
-
-    else:
-        from pydantic import root_validator, validator
-
-        valid_url = validator("amis_cdn", "site_path", "site_url", pre=True)(lambda cls, v: cls.valid_url_(v))
-        valid_database_url = root_validator(pre=True, allow_reuse=True)(lambda cls, values: cls.valid_database_url_(values))
-
-
-if PYDANTIC_V2:
-    Settings.model_rebuild()
+import logging
+from typing import Any, Union
+
+from typing_extensions import Literal
+
+from fastapi_amis_admin.amis import API
+from fastapi_amis_admin.utils.pydantic import PYDANTIC_V2, BaseSettings
+
+
+class Settings(BaseSettings):
+    """Project configuration"""
+
+    host: str = "127.0.0.1"
+    port: int = 8000
+    debug: bool = False
+    version: str = "0.0.0"
+    site_title: str = "FastAPI Amis Admin"
+    site_icon: str = "https://baidu.gitee.io/amis/static/favicon_b3b0647.png"
+    site_url: str = ""
+    site_path: str = "/admin"
+    database_url_async: str = ""
+    database_url: str = ""
+    language: Union[Literal["zh_CN", "en_US", "de_DE"], str] = ""
+    amis_cdn: str = "https://unpkg.com"
+    amis_pkg: str = "amis@3.3.0"
+    amis_theme: Literal["cxd", "antd", "dark", "ang"] = "cxd"
+    amis_image_receiver: API = None  # Image upload interface
+    amis_file_receiver: API = None  # File upload interface
+    logger: Union[logging.Logger, Any] = logging.getLogger("fastapi_amis_admin")
+
+    @classmethod
+    def valid_url_(cls, url: str):
+        return url[:-1] if url.endswith("/") else url
+
+    @classmethod
+    def valid_database_url_(cls, values):
+        # set default file upload api.
+        file_upload_api = f"post:{values.get('site_path', '')}/file/upload"
+        values.setdefault("amis_image_receiver", file_upload_api)
+        values.setdefault("amis_file_receiver", file_upload_api)
+        # set default database url.
+        if not values.get("database_url") and not values.get("database_url_async"):
+            values.setdefault(
+                "database_url_async",
+                "sqlite+aiosqlite:///amisadmin.db?check_same_thread=False",
+            )
+        return values
+
+    if PYDANTIC_V2:
+        from pydantic import field_validator, model_validator
+
+        valid_url = field_validator("amis_cdn", "site_path", "site_url", mode="before")(lambda cls, v: cls.valid_url_(v))
+        valid_database_url = model_validator(mode="before")(lambda cls, values: cls.valid_database_url_(values))
+
+    else:
+        from pydantic import root_validator, validator
+
+        valid_url = validator("amis_cdn", "site_path", "site_url", pre=True)(lambda cls, v: cls.valid_url_(v))
+        valid_database_url = root_validator(pre=True, allow_reuse=True)(lambda cls, values: cls.valid_database_url_(values))
+
+
+if PYDANTIC_V2:
+    Settings.model_rebuild()
```

### Comparing `fastapi_amis_admin-0.6.3/fastapi_amis_admin/admin/site.py` & `fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/admin/site.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,145 +1,147 @@
-import os.path
-import platform
-import time
-import uuid
-from pathlib import Path
-
-import aiofiles
-from fastapi import FastAPI, File, UploadFile
-from pydantic import BaseModel
-from starlette.requests import Request
-from starlette.staticfiles import StaticFiles
-
-import fastapi_amis_admin
-from fastapi_amis_admin import amis
-from fastapi_amis_admin.admin import AdminApp, admin
-from fastapi_amis_admin.admin.settings import Settings
-from fastapi_amis_admin.amis.components import Page, PageSchema, Property
-from fastapi_amis_admin.crud.schema import BaseApiOut
-from fastapi_amis_admin.crud.utils import SqlalchemyDatabase
-from fastapi_amis_admin.utils.translation import i18n as _
-
-
-class APIDocsApp(admin.AdminApp):
-    page_schema = PageSchema(label="APIDocs", icon="fa fa-book", sort=-100)
-
-    def __init__(self, app: "AdminApp"):
-        super().__init__(app)
-        self.register_admin(
-            DocsAdmin,
-            ReDocsAdmin,
-        )
-
-
-class DocsAdmin(admin.IframeAdmin):
-    page_schema = PageSchema(label="AdminDocs", icon="fa fa-book")
-
-    @property
-    def src(self):
-        return self.app.site.router_path + self.app.site.fastapi.docs_url
-
-
-class ReDocsAdmin(admin.IframeAdmin):
-    page_schema = PageSchema(label="AdminRedocs", icon="fa fa-book")
-
-    @property
-    def src(self):
-        return self.app.site.router_path + self.app.site.fastapi.redoc_url
-
-
-class HomeAdmin(admin.PageAdmin):
-    page_schema = PageSchema(label=_("Home"), icon="fa fa-home", url="/home", isDefaultPage=True, sort=100)
-    page_path = "/home"
-
-    async def get_page(self, request: Request) -> Page:
-        page = await super().get_page(request)
-        page.body = [
-            Property(
-                title="SiteInfo",
-                column=4,
-                items=[
-                    Property.Item(label="title", content=self.site.settings.site_title),
-                    Property.Item(label="version", content=self.site.settings.version),
-                    Property.Item(label="language", content=self.site.settings.language),
-                    Property.Item(label="debug", content=str(self.site.settings.debug)),
-                ],
-            ),
-            amis.Divider(),
-            Property(
-                title="FastAPI-Amis-Admin",
-                column=4,
-                items=[
-                    Property.Item(label="system", content=platform.system()),
-                    Property.Item(label="python", content=platform.python_version()),
-                    Property.Item(label="version", content=fastapi_amis_admin.__version__),
-                    Property.Item(label="license", content="Apache2.0"),
-                    Property.Item(label="amis-cdn", content=self.site.settings.amis_cdn),
-                    Property.Item(label="amis-pkg", content=self.site.settings.amis_pkg),
-                    Property.Item(label="amis-theme", content=self.site.settings.amis_theme),
-                ],
-            ),
-        ]
-        return page
-
-
-class FileAdmin(admin.RouterAdmin):
-    # todo perfect: Limit file size/suffixes/content_type
-    file_directory: str = "upload"
-    file_path: str = "/upload"
-    file_max_size: int = 2 * 1024 * 1024
-    router_prefix = "/file"
-
-    def __init__(self, app: "AdminApp"):
-        super().__init__(app)
-        self.file_directory = self.file_directory or self.file_path
-        os.makedirs(self.file_directory, exist_ok=True)
-        self.static_path = self.mount_staticfile()
-
-    def get_filename(self, file: UploadFile):
-        filename = str(uuid.uuid4()).replace("-", "") + os.path.splitext(file.filename)[1]
-        return Path().joinpath(time.strftime("%Y%m"), filename).as_posix()
-
-    def mount_staticfile(self) -> str:
-        self.site.fastapi.mount(
-            self.file_path,
-            StaticFiles(directory=self.file_directory),
-            self.file_directory,
-        )
-        return self.site.router_path + self.file_path
-
-    def register_router(self):
-        @self.router.post(self.file_path, response_model=BaseApiOut[self.UploadOutSchema])
-        async def file_upload(file: UploadFile = File(...)):
-            filename = self.get_filename(file)
-            file_path = Path(self.file_directory) / filename
-            try:
-                res = await file.read()
-                if self.file_max_size and len(res) > self.file_max_size:
-                    return BaseApiOut(status=-2, msg="The file size exceeds the limit")
-                async with aiofiles.open(file_path, "wb") as f:
-                    await f.write(res)
-                return BaseApiOut(
-                    data=self.UploadOutSchema(filename=filename, url=f"{self.static_path}/{filename}"),
-                )
-
-            except Exception as e:
-                return BaseApiOut(status=-1, msg=str(e))
-
-    class UploadOutSchema(BaseModel):
-        filename: str = None
-        url: str = None
-
-
-class AdminSite(admin.BaseAdminSite):
-    def __init__(
-        self,
-        settings: Settings,
-        fastapi: FastAPI = None,
-        engine: SqlalchemyDatabase = None,
-    ):
-        super().__init__(settings, fastapi, engine)
-        self.register_admin(
-            HomeAdmin,
-            APIDocsApp,
-            FileAdmin,
-        )
+import os.path
+import platform
+import time
+import uuid
+from pathlib import Path
+
+import aiofiles
+from fastapi import FastAPI, File, UploadFile
+from pydantic import BaseModel
+from starlette.requests import Request
+from starlette.staticfiles import StaticFiles
+
+import fastapi_amis_admin
+from fastapi_amis_admin import amis
+from fastapi_amis_admin.admin import AdminApp, admin
+from fastapi_amis_admin.admin.settings import Settings
+from fastapi_amis_admin.amis.components import Page, PageSchema, Property
+from fastapi_amis_admin.crud.schema import BaseApiOut
+from fastapi_amis_admin.crud.utils import SqlalchemyDatabase
+from fastapi_amis_admin.utils.translation import i18n as _
+
+
+class APIDocsApp(admin.AdminApp):
+    page_schema = PageSchema(label="APIDocs", icon="fa fa-book", sort=-100)
+
+    def __init__(self, app: "AdminApp"):
+        super().__init__(app)
+        self.register_admin(
+            DocsAdmin,
+            ReDocsAdmin,
+        )
+
+
+class DocsAdmin(admin.IframeAdmin):
+    page_schema = PageSchema(label="AdminDocs", icon="fa fa-book")
+
+    @property
+    def src(self):
+        return self.app.site.router_path + self.app.site.fastapi.docs_url
+
+
+class ReDocsAdmin(admin.IframeAdmin):
+    page_schema = PageSchema(label="AdminRedocs", icon="fa fa-book")
+
+    @property
+    def src(self):
+        return self.app.site.router_path + self.app.site.fastapi.redoc_url
+
+
+class HomeAdmin(admin.PageAdmin):
+    page_schema = PageSchema(label=_("Home"), icon="fa fa-home", url="/home", isDefaultPage=True, sort=100)
+    page_path = "/home"
+
+    async def get_page(self, request: Request) -> Page:
+        page = await super().get_page(request)
+        page.body = [
+            Property(
+                title="SiteInfo",
+                column=4,
+                items=[
+                    Property.Item(label="title", content=self.site.settings.site_title),
+                    Property.Item(label="version", content=self.site.settings.version),
+                    Property.Item(label="language", content=self.site.settings.language),
+                    Property.Item(label="debug", content=str(self.site.settings.debug)),
+                ],
+            ),
+            amis.Divider(),
+            Property(
+                title="FastAPI-Amis-Admin",
+                column=4,
+                items=[
+                    Property.Item(label="system", content=platform.system()),
+                    Property.Item(label="python", content=platform.python_version()),
+                    Property.Item(label="version", content=fastapi_amis_admin.__version__),
+                    Property.Item(label="license", content="Apache2.0"),
+                    Property.Item(label="amis-cdn", content=self.site.settings.amis_cdn),
+                    Property.Item(label="amis-pkg", content=self.site.settings.amis_pkg),
+                    Property.Item(label="amis-theme", content=self.site.settings.amis_theme),
+                ],
+            ),
+        ]
+        return page
+
+
+class FileAdmin(admin.RouterAdmin):
+    # todo perfect: Limit file size/suffixes/content_type
+    file_directory: str = "upload"
+    file_path: str = "/upload"
+    file_max_size: int = 2 * 1024 * 1024
+    router_prefix = "/file"
+
+    def __init__(self, app: "AdminApp"):
+        super().__init__(app)
+        self.file_directory = self.file_directory or self.file_path
+        self.static_path = self.mount_staticfile()
+
+    def get_filename(self, file: UploadFile):
+        filename = str(uuid.uuid4()).replace("-", "") + os.path.splitext(file.filename)[1]
+        return Path().joinpath(time.strftime("%Y%m"), filename).as_posix()
+
+    def mount_staticfile(self) -> str:
+        os.path.exists(self.file_directory) or os.makedirs(self.file_directory)
+        self.site.fastapi.mount(
+            self.file_path,
+            StaticFiles(directory=self.file_directory),
+            self.file_directory,
+        )
+        return self.site.router_path + self.file_path
+
+    def register_router(self):
+        @self.router.post(self.file_path, response_model=BaseApiOut[self.UploadOutSchema])
+        async def file_upload(file: UploadFile = File(...)):
+            filename = self.get_filename(file)
+            file_path = os.path.join(self.file_directory, filename)
+            file_dir = os.path.dirname(file_path)
+            os.path.exists(file_dir) or os.makedirs(file_dir)
+            try:
+                res = await file.read()
+                if self.file_max_size and len(res) > self.file_max_size:
+                    return BaseApiOut(status=-2, msg="The file size exceeds the limit")
+                async with aiofiles.open(file_path, "wb") as f:
+                    await f.write(res)
+                return BaseApiOut(
+                    data=self.UploadOutSchema(filename=filename, url=f"{self.static_path}/{filename}"),
+                )
+
+            except Exception as e:
+                return BaseApiOut(status=-1, msg=str(e))
+
+    class UploadOutSchema(BaseModel):
+        filename: str = None
+        url: str = None
+
+
+class AdminSite(admin.BaseAdminSite):
+    def __init__(
+        self,
+        settings: Settings,
+        fastapi: FastAPI = None,
+        engine: SqlalchemyDatabase = None,
+    ):
+        super().__init__(settings, fastapi, engine)
+        self.register_admin(
+            HomeAdmin,
+            APIDocsApp,
+            FileAdmin,
+        )
```

### Comparing `fastapi_amis_admin-0.6.3/fastapi_amis_admin/amis/README.md` & `fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/amis/README.md`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-## Amis introduction
-
-[amis](https://github.com/baidu/amis) is a low-code front-end framework developed by the `Baidu` team, which uses `JSON`
-Configuring to generate pages can reduce the workload of page development and greatly improve efficiency. `python amis`
-Based on `baidu amis`, the `amis` data structure is converted to the corresponding python data model through [pydantic](https://pydantic-docs.helpmanual.io), and some common methods are added.
-
-## Amis Highlights
-
-- **No need to know front-end**: Inside Baidu, most of the amis users have never written front-end pages before, nor `JavaScript`, but they can make professional and complex back-end interfaces, which is the same as all other front-ends.
-  UI library can't do it;
-- **Not affected by front-end technology updates**: The oldest amis page in Baidu was created more than 6 years ago and is still in use, while the `Angular/Vue/React` of that year
-  Versions are now obsolete, and the popular `Gulp` was also used by `Webpack`
-  Instead, if these pages do not use amis, the maintenance cost will now be high;
-- **Enjoy the continuous upgrade of amis**: amis has been improving the interactive experience of details, such as the freezing of the first row of the table, the lack of lag under the big data of the drop-down box, etc. The previous JSON configuration does not need to be modified at all;
-- You can **completely** use the [visual page editor](https://aisuda.github.io/amis-editor-demo/) to make pages: general front-end visual editors can only be used for static prototypes, while
-  friends
-  The page made by the visual editor can be launched directly.
-- **Provide a complete interface solution**: Other UI frameworks must use JavaScript to assemble business logic, while amis only needs JSON
-  Configuration can complete complete function development, including functions such as data acquisition, form submission and verification, and the resulting page can be launched directly without secondary development;
-- **A large number of built-in components (120+), one-stop solution**: Most of other UI frameworks only have the most common components. If you encounter some less commonly used components, you have to find a third party yourself, and these third parties Components are often inconsistent in presentation and interaction, and the integration effect is not good.
-  friends
-  There are a large number of built-in components, including business components such as rich text editor, code editor, diff, conditional combination, real-time log, etc. Most of the middle and background page development only needs to understand amis;
-- **Support extension**: In addition to low-code mode, you can also extend components through [custom components](https://baidu.gitee.io/amis/zh-CN/docs/extend/internal), in fact
-  amis can be used as normal UI
-  Libraries are used to achieve a mixed mode of 90% low code and 10% code development, which improves efficiency without losing flexibility;
-- **Container supports infinite nesting**: various layout and presentation needs can be met through nesting;
-- **Experiencing a long-term practical test**: amis is widely used within Baidu, **created 50,000 pages in more than 6 years**, from content review to machine management, from data analysis to model training, amis
-  Satisfies a variety of page needs, the most complex page has more than 10,000 lines of JSON
-  configuration.
-
-## Install
-
-```bash
-pip install amis 
-```
-
-## Simple example
-
-**main.py**:
-
-```python
-from amis.components import Page
-
-page = Page(title='title', body='Hello World!')
-# output as json
-print(page.amis_json())
-# output as dict
-print(page.amis_dict())
-# output page html
-print(page.amis_html())
-```
-
-## Development documentation
-
-Reference: [Amis official documentation](https://baidu.gitee.io/amis/zh-CN/docs/index)
-
-## Dependent projects
-
-- [pydantic](https://pydantic-docs.helpmanual.io/)
-
-- [amis](https://baidu.gitee.io/amis)
-
-## agreement
-
-The project follows the Apache2.0 license agreement.
-
-
+## Amis introduction
+
+[amis](https://github.com/baidu/amis) is a low-code front-end framework developed by the `Baidu` team, which uses `JSON`
+Configuring to generate pages can reduce the workload of page development and greatly improve efficiency. `python amis`
+Based on `baidu amis`, the `amis` data structure is converted to the corresponding python data model through [pydantic](https://pydantic-docs.helpmanual.io), and some common methods are added.
+
+## Amis Highlights
+
+- **No need to know front-end**: Inside Baidu, most of the amis users have never written front-end pages before, nor `JavaScript`, but they can make professional and complex back-end interfaces, which is the same as all other front-ends.
+  UI library can't do it;
+- **Not affected by front-end technology updates**: The oldest amis page in Baidu was created more than 6 years ago and is still in use, while the `Angular/Vue/React` of that year
+  Versions are now obsolete, and the popular `Gulp` was also used by `Webpack`
+  Instead, if these pages do not use amis, the maintenance cost will now be high;
+- **Enjoy the continuous upgrade of amis**: amis has been improving the interactive experience of details, such as the freezing of the first row of the table, the lack of lag under the big data of the drop-down box, etc. The previous JSON configuration does not need to be modified at all;
+- You can **completely** use the [visual page editor](https://aisuda.github.io/amis-editor-demo/) to make pages: general front-end visual editors can only be used for static prototypes, while
+  friends
+  The page made by the visual editor can be launched directly.
+- **Provide a complete interface solution**: Other UI frameworks must use JavaScript to assemble business logic, while amis only needs JSON
+  Configuration can complete complete function development, including functions such as data acquisition, form submission and verification, and the resulting page can be launched directly without secondary development;
+- **A large number of built-in components (120+), one-stop solution**: Most of other UI frameworks only have the most common components. If you encounter some less commonly used components, you have to find a third party yourself, and these third parties Components are often inconsistent in presentation and interaction, and the integration effect is not good.
+  friends
+  There are a large number of built-in components, including business components such as rich text editor, code editor, diff, conditional combination, real-time log, etc. Most of the middle and background page development only needs to understand amis;
+- **Support extension**: In addition to low-code mode, you can also extend components through [custom components](https://baidu.gitee.io/amis/zh-CN/docs/extend/internal), in fact
+  amis can be used as normal UI
+  Libraries are used to achieve a mixed mode of 90% low code and 10% code development, which improves efficiency without losing flexibility;
+- **Container supports infinite nesting**: various layout and presentation needs can be met through nesting;
+- **Experiencing a long-term practical test**: amis is widely used within Baidu, **created 50,000 pages in more than 6 years**, from content review to machine management, from data analysis to model training, amis
+  Satisfies a variety of page needs, the most complex page has more than 10,000 lines of JSON
+  configuration.
+
+## Install
+
+```bash
+pip install amis 
+```
+
+## Simple example
+
+**main.py**:
+
+```python
+from amis.components import Page
+
+page = Page(title='title', body='Hello World!')
+# output as json
+print(page.amis_json())
+# output as dict
+print(page.amis_dict())
+# output page html
+print(page.amis_html())
+```
+
+## Development documentation
+
+Reference: [Amis official documentation](https://baidu.gitee.io/amis/zh-CN/docs/index)
+
+## Dependent projects
+
+- [pydantic](https://pydantic-docs.helpmanual.io/)
+
+- [amis](https://baidu.gitee.io/amis)
+
+## agreement
+
+The project follows the Apache2.0 license agreement.
+
+
```

### Comparing `fastapi_amis_admin-0.6.3/fastapi_amis_admin/amis/components.py` & `fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/amis/components.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,2851 +1,2851 @@
-"""Detailed document reading address: https://baidu.gitee.io/amis/zh-CN/components"""
-import os
-from typing import Any, Dict, List, Optional, Tuple, Union
-
-from pydantic import Field
-from typing_extensions import Literal
-
-from .constants import (
-    BarcodeEnum,
-    DisplayModeEnum,
-    LevelEnum,
-    PlacementEnum,
-    ProgressEnum,
-    SizeEnum,
-    StepStatusEnum,
-    TabsModeEnum,
-    TriggerEnum,
-)
-from .types import (
-    API,
-    AmisNode,
-    BaseAmisModel,
-    Expression,
-    OptionsNode,
-    SchemaNode,
-    Template,
-    Tpl,
-)
-from .utils import amis_templates
-
-BASE_DIR = os.path.dirname(os.path.abspath(__file__))
-
-RemarkT = Union[str, "Remark"]
-
-
-class Html(AmisNode):
-    """Html"""
-
-    type: str = "html"  # specify as html component
-    html: str  # html When you need to get variables in the data field, use Tpl.
-
-
-class Icon(AmisNode):
-    """icon"""
-
-    type: str = "icon"  # specify the component type
-    className: str = None  # Outer CSS class name
-    icon: str = None  # icon name, support fontawesome v4 or use url
-    vendor: str = None  # icon vendor, icon supports fontawesome v4 by default, if you want to support fontawesome v5
-    # and v6, please set vendor to an empty string.
-
-
-class Remark(AmisNode):
-    """mark"""
-
-    type: str = "remark"  # remark
-    className: str = None  # Outer CSS class name
-    content: str = None  # prompt text
-    placement: str = None  # Popup position
-    trigger: str = None  # Trigger condition['hover','focus']
-    icon: str = None  # "fa fa-question-circle" # icon
-
-
-class Badge(AmisNode):
-    """Subscript"""
-
-    mode: str = "dot"  # Corner type, can be dot/text/ribbon
-    text: Union[int, str] = None  # Corner text, supports strings and numbers, invalid when mode='dot'
-    size: int = None  # Angular size
-    level: str = None  # The level of the corner label, which can be info/success/warning/danger, after setting the
-    # background color of the corner label is different
-    overflowCount: int = None  # 99 # Set the capped number value
-    position: str = None  # "top-right" # Corner position, can be top-right/top-left/bottom-right/bottom-left
-    offset: int = None  # The position of the corner label, the priority is greater than the position, when the
-    # offset is set, the position is positioned as the top-right reference number[top, left]
-    className: str = None  # The class name of the outer dom
-    animation: bool = None  # whether the corner icon displays animation
-    style: dict = None  # Custom style for corner labels
-    visibleOn: Expression = None  # Controls the display and hiding of corner labels
-
-
-class Page(AmisNode):
-    """page"""
-
-    __default_template_path__: str = f"{BASE_DIR}/templates/page.html"
-
-    type: str = "page"  # Specify as Page component
-    title: SchemaNode = None  # page title
-    subTitle: SchemaNode = None  # Page subtitle
-    remark: RemarkT = None  # A prompt icon will appear near the title, and the content will be prompted when the
-    # mouse is placed on it.
-    aside: SchemaNode = None  # Add content to the sidebar area of the page
-    asideResizor: bool = None  # whether the width of the sidebar area of the page can be adjusted
-    asideMinWidth: int = None  # The minimum width of the sidebar area of the page
-    asideMaxWidth: int = None  # The maximum width of the sidebar area of the page
-    toolbar: SchemaNode = None  # Add content to the upper right corner of the page. It should be noted that when
-    # there is a title, the area is in the upper right corner, and when there is no title, the area is at the top
-    body: SchemaNode = None  # Add content to the content area of the page
-    className: str = None  # Outer dom class name
-    cssVars: dict = None  # Custom CSS variables, please refer to styles
-    css: str = None  # Custom CSS styles, please refer to used theme styles
-    mobileCSS: str = None  # Custom mobile CSS styles, please refer to used theme styles
-    toolbarClassName: str = None  # "v-middle wrapper text-right bg-light bb" # Toolbar dom class name
-    bodyClassName: str = None  # "wrapper" # Body dom class name
-    asideClassName: str = None  # "w page-aside-region bg-auto" # Aside dom class name
-    headerClassName: str = None  # "bg-light bb wrapper" # Header area dom class name
-    initApi: API = None  # The api that Page uses to get initial data. The returned data can be used at the entire
-    # page level.
-    initFetch: bool = None  # True # whether to start pulling initApi
-    initFetchOn: Expression = None  # whether to start pulling initApi, configure by expression
-    interval: int = None  # refresh time (minimum 1000)
-    silentPolling: bool = None  # False # whether to show the loading animation when the configuration is refreshed
-    stopAutoRefreshWhen: Expression = None  # Configure the conditions for stopping refresh through expressions
-    regions: List[str] = None
-
-    def amis_html(
-        self,
-        template_path: str = "",
-        locale: str = "zh_CN",
-        cdn: str = "https://unpkg.com",
-        pkg: str = "amis@1.10.2",
-        site_title: str = "Amis",
-        site_icon: str = "",
-        theme: str = "cxd",
-    ):
-        """Render html template"""
-        template_path = template_path or self.__default_template_path__
-        theme_css = f'<link href="{cdn}/{pkg}/sdk/{theme}.css" rel="stylesheet"/>' if theme != "cxd" else ""
-        return amis_templates(template_path).safe_substitute(
-            {
-                "AmisSchemaJson": self.amis_json(),
-                "locale": locale.replace("_", "-"),  # Fix #50
-                "cdn": cdn,
-                "pkg": pkg,
-                "site_title": site_title,
-                "site_icon": site_icon,
-                "theme": theme,
-                "theme_css": theme_css,
-            }
-        )
-
-
-class Divider(AmisNode):
-    """Dividing line"""
-
-    type: str = "divider"  # "Divider"
-    className: str = None  # The class name of the outer Dom
-    lineStyle: str = None  # Split line style, supports dashed and solid
-
-
-class Flex(AmisNode):
-    """layout"""
-
-    type: str = "flex"  # Specify as Flex renderer
-    className: str = None  # css class name
-    justify: str = None  # "start", "flex-start", "center", "end", "flex-end", "space-around", "space-between",
-    # "space-evenly"
-    alignItems: str = None  # "stretch", "start", "flex-start", "flex-end", "end", "center", "baseline"
-    style: dict = None  # custom style
-    items: List[SchemaNode] = None  #
-
-
-class Grid(AmisNode):
-    """Horizontal layout"""
-
-    class Column(AmisNode):
-        """Column configuration"""
-
-        xs: int = None  # "auto" # Width ratio: 1 - 12
-        ClassName: str = None  # column class name
-        sm: int = None  # "auto" # Width ratio: 1 - 12
-        md: int = None  # "auto" # Width ratio: 1 - 12
-        lg: int = None  # "auto" # Width ratio: 1 - 12
-        valign: str = None  # 'top'|'middle'|'bottom'|'between = None # Vertical alignment of the current column content
-        body: List[SchemaNode] = None  #
-
-    type: str = "grid"  # Specify as Grid renderer
-    className: str = None  # The class name of the outer Dom
-    gap: str = None  # 'xs'|'sm'|'base'|'none'|'md'|'lg = None # Horizontal gap
-    valign: str = None  # 'top'|'middle'|'bottom'|'between = None # Vertical alignment
-    align: str = None  # 'left'|'right'|'between'|'center = None # Horizontal alignment
-    columns: List[SchemaNode] = None  #
-
-
-class Panel(AmisNode):
-    """panel"""
-
-    type: str = "panel"  # Specify as the Panel renderer
-    className: str = None  # "panel-default" # The class name of the outer Dom
-    headerClassName: str = None  # "panel-heading" # The class name of the header area
-    footerClassName: str = None  # "panel-footer bg-light lter wrapper" # The class name of the footer area
-    actionsClassName: str = None  # "panel-footer" # The class name of the actions area
-    bodyClassName: str = None  # "panel-body" # The class name of the body area
-    title: SchemaNode = None  # title
-    header: SchemaNode = None  # header container
-    body: SchemaNode = None  # Content container
-    footer: SchemaNode = None  # bottom container
-    affixFooter: bool = None  # whether to fix the bottom container
-    actions: List["Action"] = None  # Button area
-
-
-class Tabs(AmisNode):
-    """Tab"""
-
-    class Item(AmisNode):
-        title: str = None  # Tab title
-        icon: Union[str, Icon] = None  # Icon for Tab
-        tab: SchemaNode = None  # Content area
-        hash: str = None  # After setting, it will correspond to the hash of the url
-        reload: bool = None  # After setting, the content will be re-rendered every time, which is useful for
-        # re-pulling crud
-        unmountOnExit: bool = None  # Each exit will destroy the current tab bar content
-        className: str = None  # "bg-white bl br bb wrapper-md" # Tab area style
-        iconPosition: str = None  # "left" # Tab's icon position left / right
-        closable: bool = None  # False # whether to support deletion, the priority is higher than the closable of the
-        # component
-        disabled: bool = None  # False # whether to disable
-
-    type: str = "tabs"  # Specify as Tabs renderer
-    className: str = None  # The class name of the outer Dom
-    mode: str = None  # Display mode, the value can be line, card, radio, vertical, chrome, simple, strong, tiled,
-    # sidebar
-    tabsClassName: str = None  # Class name of Tabs Dom
-    tabs: List[Item] = None  # tabs content
-    source: str = None  # tabs associated data, tabs can be generated repeatedly after association
-    toolbar: SchemaNode = None  # toolbar in tabs
-    toolbarClassName: str = None  # The class name of the toolbar in the tabs
-    mountOnEnter: bool = None  # False # Render only when the tab is clicked
-    unmountOnExit: bool = None  # False # Destroyed when switching tabs
-    scrollable: bool = None  # False # whether the navigation supports content overflow scrolling, this property is
-    # not supported in vertical and chrome modes; chrome mode defaults to compress tags (property discarded)
-    tabsMode: TabsModeEnum = None  # Display mode, the value can be line, card, radio, vertical, chrome, simple,
-    # strong, tiled, sidebar
-    addable: bool = None  # False # whether to support adding
-    addBtnText: str = None  # "Add" # Add button text
-    closable: bool = None  # False # whether to support delete
-    draggable: bool = None  # False # whether to support draggable
-    showTip: bool = None  # False # whether to support tips
-    showTipClassName: str = None  # "'' " # Tip class
-    editable: bool = None  # False # whether to edit the tag name
-    sidePosition: str = None  # "left" # In sidebar mode, the position of the tab bar is left / right
-
-
-class Portlet(Tabs):
-    """Portal column"""
-
-    class Item(Tabs.Item):
-        toolbar: SchemaNode = None  # The toolbar in tabs, which changes with tab switching
-
-    type: str = "portlet"  # specify as portlet renderer
-    contentClassName: str = None  # Class name of Tabs content Dom
-    tabs: List[Item] = None  # tabs content
-    style: Union[str, dict] = None  # custom style
-    description: Template = None  # Information on the right side of the title
-    hideHeader: bool = None  # False # hide the header
-    divider: bool = None  # False # remove divider
-
-
-class Horizontal(AmisNode):
-    left: int = None  # The width ratio of the left label
-    right: int = None  # The width ratio of the right controller.
-    offset: int = None  # When the label is not set, the offset of the right controller
-
-
-class Action(AmisNode):
-    """Behavior button"""
-
-    type: str = "button"  # Specify as the Page renderer. button action
-    actionType: str = None  # [Required] This is the core configuration of the action to specify the action type of
-    # the action. Support: ajax, link, url, drawer, dialog, confirm, cancel, prev, next, copy, close.
-    label: str = None  # Button text. Available ${xxx} values.
-    level: LevelEnum = None  # Button style, support: link, primary, secondary, info, success, warning, danger,
-    # light, dark, default.
-    size: str = None  # Button size, support: xs, sm, md, lg.
-    icon: str = None  # Set the icon, eg fa fa-plus.
-    iconClassName: str = None  # Add a class name to the icon.
-    rightIcon: str = None  # Set the icon to the right of the button text, eg fa fa-plus.
-    rightIconClassName: str = None  # Add a class name to the right icon.
-    active: bool = None  # whether the button is highlighted.
-    activeLevel: str = None  # The style when the button is highlighted, the configuration supports the same level.
-    activeClassName: str = None  # Add a class name to the button highlight. "is-active"
-    block: bool = None  # Use display:"block" to display the button.
-    confirmText: Template = None  # When set, the action will ask the user before starting. Available ${xxx} values.
-    reload: str = None  # Specify the name of the target component that needs to be refreshed after this operation (
-    # the name value of the component, configured by yourself), please separate multiple ones with , signs.
-    tooltip: str = None  # This text pops up when the mouse stays, and the object type can also be configured: the
-    # fields are title and content. Available ${xxx} values.
-    disabledTip: str = None  # The text will pop up when the mouse stays after it is disabled. You can also configure
-    # the object type: the fields are title and content. Available ${xxx} values.
-    tooltipPlacement: str = None  # If tooltip or disabledTip is configured, specify the location of the prompt
-    # information, and you can configure top, bottom, left, and right.
-    close: Union[bool, str] = None  # When the action is configured in the actions of the dialog or drawer, configure
-    # it to true to close the current dialog or drawer after the operation. When the value is a string and is the
-    # name of the ancestor layer popup, the ancestor popup will be closed.
-    required: List[str] = None  # Configure an array of strings, specifying that the form items with the specified
-    # field name must pass validation before performing operations in the form primary:bool=None
-    onClick: str = None  # The custom click event defines the click event through onClick in the form of a string,
-    # which will be converted into a JavaScript function
-    componentId: str = None  # target component ID
-    args: Union[dict, str] = None  # event parameters
-    script: str = None  # Customize JS script code, any action can be performed by calling doAction in the code,
-    # and event action intervention can be realized through the event object event
-
-
-class ActionType:
-    """Behavior button type"""
-
-    class Ajax(Action):
-        actionType: str = "ajax"  # Show a popup after clicking
-        api: API = None  # Request address, refer to api format description.
-        redirect: Template = None  # Specify the path to redirect to after the current request ends, which can be
-        # valued by ${xxx}.
-        feedback: "Dialog" = None  # If it is of ajax type, when ajax returns to normal, a dialog can be popped up
-        # for other interactions. The returned data can be used in this dialog. For the format, please refer to Dialog
-        messages: dict = None  # success: a message will be displayed after the ajax operation is successful. It can
-        # be left unspecified. If it is not specified, the api return shall prevail. failed: Ajax operation failure
-        # message.
-
-    class Dialog(Action):
-        actionType: str = "dialog"  # Show a popup when clicked
-        dialog: Union["Dialog", "Service", SchemaNode]  # Specify the content of the pop-up box, the format can refer to Dialog
-        nextCondition: bool = None  # Can be used to set the condition of the next data, the default is true.
-
-    class Drawer(Action):
-        actionType: str = "drawer"  # Show a sidebar when clicked
-        drawer: Union["Drawer", "Service", SchemaNode]  # Specify the content of the popup box, the format can refer to Drawer
-
-    class Copy(Action):
-        actionType: str = "copy"  # Copy a piece of content to the clipboard
-        content: Template  # Specify the copied content. Available ${xxx} values.
-        copyFormat: str = None  # You can set the copy format through copyFormat, the default is text text/html
-
-    class Url(Action):
-        """Jump directly"""
-
-        actionType: str = "url"  # Jump directly
-        url: str  # When the button is clicked, the specified page will be opened. Available ${xxx} values.
-        blank: bool = None  # false If true will open in a new tab page.
-
-    class Link(Action):
-        """Single page jump"""
-
-        actionType: str = "link"  # Single page jump
-        link: str  # is used to specify the jump address. Unlike url, this is a single-page jump method, which will
-        # not render the browser. Please specify the page in the amis platform. Available ${xxx} values.
-
-    class Toast(Action):
-        """Toast light"""
-
-        class ToastItem(AmisNode):
-            title: Union[str, SchemaNode] = None  # Toast Item Title
-            body: Union[str, SchemaNode] = None  # Toast Item Content
-            level: str = None  # default 'info', Display icon, optional 'info', 'success', 'error', 'warning'
-            position: str = None  # default 'top-center', display position,
-            # 'top-right', 'top-center', 'top-left', 'bottom-center', 'bottom-left', 'bottom-right', 'center'
-            closeButton: bool = None  # default False, whether to show the close button
-            showIcon: bool = None  # default True, whether to display the icon
-            timeout: int = None  # default 5000
-
-        actionType: str = "toast"  # Single page jump
-        items: List[ToastItem] = None  # List of ToastItems
-        position: str = None  # display position,
-        # available 'top-right', 'top-center', 'top-left', 'bottom-center', 'bottom-left', 'bottom-right', 'center'
-        closeButton: bool = None  # default False, whether to display the close button, not in mobile
-        showIcon: bool = None  # default = True, whether to display the icon
-        timeout: int = None  # default 5000
-
-
-class PageSchema(AmisNode):
-    """Page configuration"""
-
-    label: str = None  # Menu name.
-    icon: str = "fa fa-flash"  # Menu icon, for example: 'fa fa-file'. For detailed icon reference:
-    # http://www.fontawesome.com.cn/faicons/
-    url: str = None  # The page routing path, when the route hits the path, the current page is enabled. When the
-    # path does not start with /, the parent path is concatenated. For example: the path of the parent is folder,
-    # and pageA is configured at this time, then this page will be hit only when the page address is /folder/pageA.
-    # When the path starts with / such as: /crud/list, the parent path will not be spliced. In addition, routes with
-    # parameters such as /crud/view/:id are supported. This value can be obtained from the page through ${params.id}.
-    schema_: Union[Page, "Iframe"] = Field(None, alias="schema")  # The configuration of the page, please go to the
-    # page page for specific configuration
-    schemaApi: API = None  # If you want to pull through the interface, please configure. The return path is
-    # json>data. Only one of schema and schemaApi can be selected.
-    link: str = None  # If you want to configure an external link menu, you only need to configure link.
-    redirect: str = None  # Jump, when hitting the current page, jump to the target page.
-    rewrite: str = None  # Change to rendering pages of other paths, the page address will not be modified in this way.
-    isDefaultPage: Union[bool, str] = None  # Useful when you need a custom 404 page, don't have multiple such pages,
-    # because only the first one will be useful.
-    visible: Union[bool, str] = None  # Some pages may not want to appear in the menu, you can configure it to false, and the
-    # route with parameters does not need to be configured, it is directly invisible.
-    className: str = None  # Menu class name.
-    children: List["PageSchema"] = None  # Submenu
-    sort: int = None  # Unofficial attribute. sort
-    tabsMode: TabsModeEnum = None  # Unofficial attribute. Display mode, the value can be line, card, radio, vertical,
-
-    # chrome, simple, strong, tiled, sidebar, collapse
-
-    def as_page_body(self, group_extra: Dict[str, Any] = None, item_extra: Dict[str, Any] = None):
-        if self.children:
-            exclude = {"type", "url", "schema_", "schemaApi", "link", "redirect", "rewrite", "isDefaultPage", "children"}
-            if self.tabsMode is None:
-                body = App(pages=[PageSchema(children=self.children)])
-            elif self.tabsMode == TabsModeEnum.collapse:
-                body = (
-                    CollapseGroup.parse_obj(self.dict(exclude=exclude, exclude_defaults=True))
-                    .update_from_kwargs(
-                        body=[
-                            CollapseGroup.CollapseItem.parse_obj(item.dict(exclude=exclude, exclude_defaults=True))
-                            .update_from_kwargs(
-                                header=item.label,
-                                body=item.as_page_body(group_extra, item_extra),
-                            )
-                            .update_from_dict(item_extra or {})
-                            for item in self.children
-                        ],
-                    )
-                    .update_from_dict(group_extra or {})
-                )
-            else:
-                body = (
-                    Tabs.parse_obj(self.dict(exclude=exclude, exclude_defaults=True))
-                    .update_from_kwargs(
-                        mountOnEnter=True,
-                        tabs=[
-                            Tabs.Item.parse_obj(item.dict(exclude=exclude, exclude_defaults=True))
-                            .update_from_kwargs(
-                                title=item.label,
-                                tab=item.as_page_body(group_extra, item_extra),
-                            )
-                            .update_from_dict(item_extra or {})
-                            for item in self.children
-                        ],
-                    )
-                    .update_from_dict(group_extra or {})
-                )
-        elif self.schema_:
-            body = self.schema_
-            if isinstance(body, Iframe):
-                body.height = body.height or 1080
-        elif self.schemaApi:
-            body = Service(schemaApi=self.schemaApi)
-        elif self.link:
-            body = Page(body=Link(href=self.link, body=self.label, blank=True))
-        else:
-            body = None
-        return body
-
-
-class App(Page):
-    """Multi-page application"""
-
-    __default_template_path__: str = f"{BASE_DIR}/templates/app.html"
-    type: str = "app"
-    api: API = None  # The page configuration interface, if you want to pull the page configuration remotely,
-    # please configure it. Return to the configuration path json>data>pages, please refer to the pages property for
-    # the specific format.
-    brandName: str = None  # app name
-    logo: str = None  # Support image address, or svg.
-    className: str = None  # css class name
-    header: str = None  # header
-    asideBefore: str = None  # The front area on the page menu.
-    asideAfter: str = None  # The front area under the page menu.
-    footer: str = None  # The page.
-    pages: List[PageSchema] = None  # Array<page configuration> specific page configuration.
-    # Usually in an array, the first layer of the array is a group, generally you only need to configure the label set,
-    # if you don't want to group, don't configure it directly, the real page should be configured in the second
-    # layer, that is, in the children of the first layer.
-
-
-class ButtonGroup(AmisNode):
-    """Button group"""
-
-    type: str = "button-group"
-    buttons: List[Action]  # Behavior button group
-    className: str = None  # The class name of the outer Dom
-    vertical: bool = None  # whether to use vertical mode
-    tiled: bool = None  # whether to use tile mode
-    btnLevel: LevelEnum = None  # button style
-    btnActiveLevel: LevelEnum = None  # Active button style
-
-
-class Custom(AmisNode):
-    """Custom Components"""
-
-    type: str = "custom"
-    id: str = None  # node id
-    name: str = None  # node name
-    className: str = None  # node class
-    inline: bool = False  # use div tag by default, if true use span tag
-    html: str = None  # initialize node html
-    onMount: str = None  # "Function" # Function called after node initialization
-    onUpdate: str = None  # "Function" # The function called when the data is updated
-    onUnmount: str = None  # "Function" # The function called when the node is destroyed
-
-
-class Service(AmisNode):
-    """Functional container"""
-
-    type: str = "service"  # designate as service renderer
-    name: str = None  # node name
-    data: dict = None  #
-    className: str = None  # The class name of the outer Dom
-    body: SchemaNode = None  # Content container
-    api: API = None  # Initialize data domain interface address
-    ws: str = None  # WebScocket address
-    dataProvider: str = None  # Data acquisition function
-    initFetch: bool = None  # whether to pull by default
-    schemaApi: API = None  # Used to get the remote schema interface address
-    initFetchSchema: bool = None  # whether to pull Schema by default
-    messages: dict = None  # Message prompt override, the default message reads the toast prompt text returned by the
-    # interface, but it can be overridden here.
-    # messages.fetchSuccess: str = None # Toast prompt text when the interface request is successful
-    # messages.fetchFailed: str = "Initialization failed" # Toast prompt text when interface request fails
-    interval: int = None  # Polling interval (minimum 3000)
-    silentPolling: bool = None  # False # whether to display the loading animation during polling
-    stopAutoRefreshWhen: Expression = None  # Configure the condition to stop polling
-
-
-class Nav(AmisNode):
-    """navigation"""
-
-    class Link(AmisNode):
-        label: str = None  # name
-        to: Template = None  # Link address
-        target: str = None  # "Link relationship" #
-        icon: str = None  # icon
-        children: List["Link"] = None  # child links
-        unfolded: bool = None  # whether to unfold initially
-        active: bool = None  # whether to highlight
-        activeOn: Expression = None  # whether to highlight the condition, leaving it blank will automatically
-        # analyze the link address
-        defer: bool = None  # mark whether it is a lazy add-in
-        deferApi: API = None  # Can not be configured, if the configuration priority is higher
-
-    type: str = "nav"  # specify as Nav renderer
-    className: str = None  # The class name of the outer Dom
-    stacked: bool = True  # Set to false to display in the form of tabs
-    source: API = None  # Navigation can be created dynamically via variable or API interface
-    deferApi: API = None  # The interface used to delay loading option details. It can be left unconfigured,
-    # and the public source interface cannot be configured.
-    itemActions: SchemaNode = None  # More operations related configuration
-    draggable: bool = None  # whether to support drag and drop sorting
-    dragOnSameLevel: bool = None  # Only allow dragging within the same level
-    saveOrderApi: API = None  # save order api
-    itemBadge: Badge = None  # Badge
-    links: list = None  # link collection
-
-
-class AnchorNav(AmisNode):
-    """Anchor Navigation"""
-
-    class Link(AmisNode):
-        label: str = None  # name
-        title: str = None  # area title
-        href: str = None  # Region ID
-        body: SchemaNode = None  # area content area
-        className: str = None  # "bg-white bl br bb wrapper-md" # Area member style
-
-    type: str = "anchor-nav"  # Specify as AnchorNav renderer
-    className: str = None  # The class name of the outer Dom
-    linkClassName: str = None  # Class name of the navigation Dom
-    sectionClassName: str = None  # The class name of the anchor area Dom
-    links: list = None  # links content
-    direction: str = None  # "vertical" # You can configure whether the navigation is displayed horizontally or
-    # vertically. The corresponding configuration items are: vertical, horizontal
-    active: str = None  # The area that needs to be located
-
-
-class ButtonToolbar(AmisNode):
-    """Button Toolbar"""
-
-    type: str = "button-toolbar"
-    buttons: List[Action]  # Behavior button group
-
-
-class Validation(BaseAmisModel):
-    isEmail: bool = None  # Must be Email.
-    isUrl: bool = None  # Must be a Url.
-    isNumeric: bool = None  # Must be a number.
-    isAlpha: bool = None  # Must be an alpha.
-    isAlphanumeric: bool = None  # Must be a letter or a number.
-    isInt: bool = None  # Must be an integer.
-    isFloat: bool = None  # Must be a float.
-    isLength: int = None  # whether the length is exactly equal to the set value.
-    minLength: int = None  # Minimum length.
-    maxLength: int = None  # Maximum length.
-    maximum: int = None  # Maximum value.
-    minimum: int = None  # Minimum value.
-    equals: str = None  # The current value must be exactly equal to xxx.
-    equalsField: str = None  # The current value must be the same as the xxx variable value.
-    isJson: bool = None  # Is it a valid Json string.
-    isUrlPath: bool = None  # is the url path.
-    isPhoneNumber: bool = None  # Is it a legal phone number
-    isTelNumber: bool = None  # Is it a valid phone number
-    isZipcode: bool = None  # whether it is a zip code
-    isId: bool = None  # whether it is an ID number, no verification is done
-    matchRegexp: str = None  # Must hit a certain regexp. /foo/
-
-
-class FormItem(AmisNode):
-    """Form item common"""
-
-    class AutoFill(BaseAmisModel):
-        showSuggestion: bool = None  # true refers to input, false automatically fills
-        api: API = None  # Automatically populate the interface/filter the CRUD request configuration with reference to entry
-        silent: bool = None  # Whether to display a data format error message. The default value is true
-        fillMappinng: SchemaNode = None  # Auto-fill/reference input data mapping configuration, key-value pair form,
-        # value support variable acquisition and expression
-        trigger: str = None  # ShowSuggestion to true, the reference input support way of trigger,
-        # currently supports change "value change" | focus "form focus"
-        mode: str = None  # When showSuggestion is true, refer to the popOver mode: dialog, drawer, popOver
-        labelField: str = None  # When showSuggestion is true, set the popup dialog,drawer,popOver picker's labelField
-        position: str = None  # If showSuggestion is true, set the popOver location as shown in the input mode Popover
-        size: str = None  # If showSuggestion is true, set the value as shown in dialog mode
-        columns: List["TableColumn"] = None  # When showSuggestion is true, the data display column configuration
-        filter: SchemaNode = None  # When showSuggestion is true, data query filter condition
-
-    type: str = "input-text"  # Specify the form item type
-    className: str = None  # The outermost class name of the form
-    inputClassName: str = None  # Form controller class name
-    labelClassName: str = None  # class name of label
-    name: str = None  # Field name, specifying the key when the form item is submitted
-    label: Union[bool, Template] = None  # form item label template or false
-    labelAlign: str = None  # "right" # Form item label alignment, default right alignment, only effective when mode is
-    labelRemark: RemarkT = None  # Form item label description
-    description: Template = None  # Form item description
-    placeholder: str = None  # Form item description
-    inline: bool = None  # whether it is inline mode
-    submitOnChange: bool = None  # whether to submit the current form when the value of the form item changes.
-    disabled: bool = None  # whether the current form item is disabled
-    disabledOn: Expression = None  # The condition for whether the current form item is disabled
-    visible: Expression = None  # whether the current form item is disabled or not
-    visibleOn: Expression = None  # The condition for whether the current form item is disabled
-    required: bool = None  # whether it is required.
-    requiredOn: Expression = None  # Use an expression to configure whether the current form item is required.
-    validations: Union[Validation, Expression] = None  # Validation of the form item value format, multiple settings
-    # are supported, and multiple rules are separated by commas.
-    validateApi: API = None  # Form validation interface
-    copyable: Union[bool, dict] = None  # whether to copy boolean or {icon: string, content:string}
-    autoFill: AutoFill = None  # Data entry configuration, automatic filling or reference entry
-    static: bool = None  # 2.4.0 Whether the current form item is static display,
-    # the current support static display of the form item
-    staticClassName: str = None  # 2.4.0 The class name for static display
-    staticLabelClassName: str = None  # 2.4.0 The class name of the Label for static display
-    staticInputClassName: str = None  # 2.4.0 The class name of value when static display
-    staticSchema: Union[str, list] = None  # SchemaNode
-
-
-class ButtonGroupSelect(FormItem):
-    """Button group select"""
-
-    type: str = "button-group-select"
-    vertical: bool = None  # Default False, use vertical mode
-    tiled: bool = None  # Default False, use tile mode
-    btnLevel: LevelEnum = LevelEnum.default  # button style
-    btnActiveLevel: LevelEnum = LevelEnum.default  # Check button style
-    options: OptionsNode = None  # option group
-    source: API = None  # dynamic group
-    multiple: bool = None  # Default False, multiple choice
-    labelField: str = None  # Default "label"
-    valueField: str = None  # Default "value"
-    joinValues: bool = None  # Default True
-    extractValue: bool = None  # Default False
-    autoFill: dict = None  # autofill
-
-
-class ListSelect(FormItem):
-    """List select, allows images"""
-
-    type: str = "list-select"
-    options: OptionsNode = None  # option group
-    source: API = None  # dynamic group
-    multiple: bool = None  # Default False, multiple choice
-    labelField: str = None  # Default "label"
-    valueField: str = None  # Default "value"
-    joinValues: bool = None  # Default True
-    extractValue: bool = None  # Default False
-    autoFill: dict = None  # autofill
-    listClassName: str = None  # Supports configuring the css class name of the list div. for example:flex justify-between
-
-
-class Form(AmisNode):
-    """Form"""
-
-    class Messages(AmisNode):
-        fetchSuccess: str = None  # Prompt when fetch is successful
-        fetchFailed: str = None  # Prompt when fetch fails
-        saveSuccess: str = None  # Prompt when saving is successful
-        saveFailed: str = None  # Prompt when saving fails
-
-    type: str = "form"  # "form" specifies the Form renderer
-    name: str = None  # After setting a name, it is convenient for other components to communicate with it
-    mode: DisplayModeEnum = None  # Form display mode, can be: normal, horizontal or inline
-    horizontal: Horizontal = None  # Useful when mode is horizontal,
-    # Used to control label {"left": "col-sm-2", "right": "col-sm-10", "offset": "col-sm-offset-2"}
-    title: Optional[str] = None  # Title of the Form
-    submitText: Optional[str] = None  # "Submit" # Default submit button name, if it is set to empty, the default
-    # button can be removed.
-    className: str = None  # The class name of the outer Dom
-    body: List[Union[FormItem, SchemaNode]] = None  # Form item collection
-    actions: List["Action"] = None  # Form submit button, the member is Action
-    actionsClassName: str = None  # class name of actions
-    messages: Messages = None  # The message prompts to be overridden. The default message reads the message returned
-    # by the API, but it can be overridden here.
-    wrapWithPanel: bool = None  # whether to wrap the Form with panel, if set to false, actions will be invalid.
-    panelClassName: str = None  # The class name of the outer panel
-    api: API = None  # The api that Form uses to save data.
-    initApi: API = None  # The api that Form uses to get initial data.
-    rules: list = None  # Form combination validation rules Array<{rule:string;message:string}>
-    interval: int = None  # refresh time (minimum 3000)
-    silentPolling: bool = None  # False # whether to show the loading animation when the configuration is refreshed
-    stopAutoRefreshWhen: str = None  # Configure the condition for stopping refresh by expression
-    initAsyncApi: API = None  # The api that Form uses to obtain initial data, which is different from initApi,
-    # will keep polling and request this interface until the returned finished attribute is true.
-    initFetch: bool = None  # After initApi or initAsyncApi is set, the request will be sent by default, and if it is
-    # set to false, the interface will not be requested at the beginning
-    initFetchOn: str = None  # Use expression to configure
-    initFinishedField: Optional[str] = None  # After setting initAsyncApi, by default, the data.finished of the
-    # returned data will be used to judge whether it is completed.
-    # Can also be set to other xxx, it will be obtained from data.xxx
-    initCheckInterval: int = None  # After setting initAsyncApi, the default pull interval
-    asyncApi: API = None  # After setting this property, after the form is submitted and sent to save the interface,
-    # it will continue to poll and request the interface, and it will not end until the returned finished property is
-    # true.
-    checkInterval: int = None  # The time interval for polling requests, the default is 3 seconds. Setting asyncApi
-    # is valid
-    finishedField: Optional[str] = None  # Set this property if the field name that decides to end is not finished,
-    # such as is_success
-    submitOnChange: bool = None  # Form modification is submitted
-    submitOnInit: bool = None  # Submit once initially
-    resetAfterSubmit: bool = None  # whether to reset the form after submitting
-    primaryField: str = None  # Set the primary key id. When set, it will only carry this data when checking whether
-    # the form is completed (asyncApi).
-    target: str = None  # The default form submission itself will save the data by sending the api, but you can also
-    # set the name value of another form, or another CRUD model name value. If the target target is a Form,
-    # the target Form will trigger initApi again, and the api can get the current form data. If the target is a CRUD
-    # model, the target model will re-trigger the search with the current Form data as the parameter. When the target
-    # is window, the data of the current form will be attached to the page address.
-    redirect: str = None  # After setting this attribute, after the Form is saved successfully, it will automatically
-    # jump to the specified page. Support relative addresses, and absolute addresses (relative to the group).
-    reload: str = None  # Refresh the target object after the operation. Please fill in the name value set by the
-    # target component. If it is filled in window, the current page will be refreshed as a whole.
-    autoFocus: bool = None  # whether to auto focus.
-    canAccessSuperData: bool = None  # Specify whether the upper layer data can be automatically obtained and mapped
-    # to the form item
-    persistData: str = None  # Specify a unique key to configure whether to enable local caching for the current form
-    clearPersistDataAfterSubmit: bool = None  # Specify whether to clear the local cache after the form is submitted
-    # successfully
-    preventEnterSubmit: bool = None  # Disable EnterSubmit form submission
-    trimValues: bool = None  # trim each value of the current form item
-    promptPageLeave: bool = None  # The form has not been saved, whether to confirm with a pop-up box before leaving
-    # the page.
-    columnCount: int = None  # The form item is displayed as several columns
-    debug: bool = None
-    inheritData: bool = None  # true # The default form is to create its own data field in the form of a data link,
-    # and only the data in this data field will be sent when the form is submitted. If you want to share the
-    # upper layer data field, you can set this attribute to false, so that the data in the upper layer data field
-    # does not need to be sent in the form with hidden fields or explicit mapping.
-    static: bool = None  # false # 2.4.0. The entire form is displayed statically.
-    # For details, please refer to the:https://aisuda.bce.baidu.com/amis/examples/form/switchDisplay.
-    staticClassName: str = None  # 2.4.0. The name of the class used when the form is statically displayed
-    labelAlign: Literal["right", "left"] = None  # "right"  # 表单项标签对齐方式，默认右对齐，仅在 mode为horizontal 时生效
-    labelWidth: Union[int, str] = None  # 表单项标签自定义宽度
-    persistDataKeys: List[str] = None  # 指指定只有哪些 key 缓存
-    closeDialogOnSubmit: bool = None  # 提交的时候是否关闭弹窗
-
-
-class InputSubForm(FormItem):
-    """Subform"""
-
-    type: str = "input-sub-form"
-    multiple: bool = None  # False # whether it is multiple selection mode
-    labelField: str = None  # When this field exists in the value, the button name will be displayed using the value
-    # of this field.
-    btnLabel: str = None  # "Settings" # Default button name
-    minLength: int = None  # 0 # Limit the minimum number.
-    maxLength: int = None  # 0 # Limit the maximum number.
-    draggable: bool = None  # whether it can be draggable and sorted
-    addable: bool = None  # whether it can be added
-    removable: bool = None  # whether it can be removed
-    addButtonClassName: str = None  # "``" # Add button CSS class name
-    itemClassName: str = None  # "``" # Value element CSS class name
-    itemsClassName: str = None  # "``" # Value wrapping element CSS class name
-    form: Form = None  # Subform configuration, same as Form
-    addButtonText: str = None  # "``" # Customize the text of the new item
-    showErrorMsg: bool = None  # True # whether to display the error message in the lower left corner
-
-
-class Button(FormItem):
-    """Button"""
-
-    className: str = None  # Specify the add button class name
-    href: str = None  # Click the jump address, specify the behavior of this attribute button is consistent with the
-    # a link
-    size: str = None  # Set button size 'xs'|'sm'|'md'|'lg'
-    actionType: str = None  # Set the button type 'button'|'reset'|'submit'| 'clear'| 'url'
-    level: LevelEnum = None  # Set button style 'link'|'primary'|'enhance'|'secondary'|'info'|'success'|'warning
-    # '|'danger'|'light'| 'dark'|'default'
-    tooltip: Union[str, dict] = None  # Bubble tip content TooltipObject
-    tooltipPlacement: str = None  # Balloon positioner 'top'|'right'|'bottom'|'left'
-    tooltipTrigger: str = None  # trigger tootip 'hover'|'focus'
-    disabled: bool = None  # button disabled state
-    block: bool = None  # Option to adjust button width to its parent width
-    loading: bool = None  # Show button loading effect
-    loadingOn: str = None  # Display button loading expression
-
-
-class InputFormula(FormItem):
-    """Input Formula Editor"""
-
-    type: str = "input-formula"
-    title: str = None  # title
-    header: str = None  # Editor header title, if not set, the form item labelfield is used by default
-    evalMode: bool = None  # default True, Expression mode or template mode (False),
-    # template mode requires the expression to be written between ${and }.
-    variables: List[dict] = None  # Available variables, {label: string; value: string; children?: any[]; tag?: string}
-    variableMode: Literal["tabs", "tree", "list"] = "list"  # Can be configured as tabs or tree ,
-    # defaults to a list, which supports grouping.
-    inputMode: Literal["button", "input-button", "input-group"] = None  # Display mode of the control
-    icon: str = None  # fa icon
-    btnLabel: str = None  # The button text, which inputModetakesbutton
-    level: LevelEnum = LevelEnum.default  # button stlye
-    allowInput: bool = None  # default -, Whether the input box can be entered
-    btnSize: Literal["xs", "sm", "md", "lg"] = None  # button size
-    borderMode: Literal["full", "half", "none"] = None  # Input box border mode
-    placeholder: str = None  # input box placeholder
-    className: str = None  # Control outer CSS style class name
-    variableClassName: str = None  # Variable panel CSS style class name
-    functionClassName: str = None  # Function panel CSS style class name
-    mixedMode: bool = None  # default False, if True it supports values in both text and formula formats
-
-
-class InputArray(FormItem):
-    """Array input box"""
-
-    type: str = "input-array"
-    items: FormItem = None  # Configure single item form type
-    addable: bool = None  # whether it can be added.
-    removable: bool = None  # whether it can be removed
-    draggable: bool = None  # False # whether drag sorting is possible, it should be noted that when drag sorting is
-    # enabled, there will be an additional $id field
-    draggableTip: str = None  # Draggable prompt text, the default is: "Order can be adjusted by dragging the [Swap]
-    # button in each row"
-    addButtonText: str = None  # "Add" # Add button text
-    minLength: int = None  # Limit the minimum length
-    maxLength: int = None  # limit max length
-    scaffold: Any = None  # 新增成员时的默认值，一般根据items的数据类型指定需要的默认值
-
-
-class Hidden(FormItem):
-    """Hidden fields"""
-
-    type: str = "hidden"
-
-
-class Checkbox(FormItem):
-    """Check box"""
-
-    type: str = "checkbox"
-    option: str = None  # option description
-    trueValue: Any = None  # identifies the true value
-    falseValue: Any = None  # identifies a false value
-    optionType: Literal["default", "button"] = None  # 设置 option 类型
-
-
-class Radios(FormItem):
-    """Single box"""
-
-    type: str = "radios"
-    options: List[Union[dict, str]] = None  # Option group
-    source: API = None  # Dynamic option group
-    labelField: bool = None  # "label" # option label field
-    valueField: bool = None  # "value" # option value field
-    columnsCount: int = None  # 1 # options are displayed in several columns, default is one column
-    inline: bool = None  # True # whether to display as one line
-    selectFirst: bool = None  # False # whether to select the first one by default
-    autoFill: dict = None  # autofill
-
-
-class ChartRadios(Radios):
-    """Single box"""
-
-    type: str = "chart-radios"
-    config: dict = None  # echart chart configuration
-    showTooltipOnHighlight: bool = None  # False # whether to show tooltip when highlighted
-    chartValueField: str = None  # "value" # Chart value field name
-
-
-class Checkboxes(FormItem):
-    """Checkbox"""
-
-    type: str = "checkboxes"
-    options: OptionsNode = None  # option group
-    source: API = None  # Dynamic option group
-    delimiter: str = None  # "," # splicer
-    labelField: str = None  # "label" # option label field
-    valueField: str = None  # "value" # option value field
-    joinValues: bool = None  # True # join values
-    extractValue: bool = None  # False # extract value
-    columnsCount: int = None  # 1 # options are displayed in several columns, default is one column
-    checkAll: bool = None  # False # whether to support select all
-    inline: bool = None  # True # whether to display as one line
-    defaultCheckAll: bool = None  # False # whether to check all by default
-    creatable: bool = None  # False # New option
-    createBtnLabel: str = None  # "Add option" # Add option
-    addControls: List[FormItem] = None  # Customize new form items
-    addApi: API = None  # Configure the new option interface
-    editable: bool = None  # False # edit options
-    editControls: List[FormItem] = None  # Customize edit form items
-    editApi: API = None  # Configure editing options interface
-    removable: bool = None  # False # remove option
-    deleteApi: API = None  # Configure delete option interface
-    optionType: Literal["default", "button"] = None  # "default"  # 按钮模式
-    itemClassName: str = None  # 选项样式类名
-    labelClassName: str = None  # 选项标签样式类名
-
-
-class InputCity(FormItem):
-    """City selector"""
-
-    type: str = "input-city"
-    allowCity: bool = None  # True # Allow city selection
-    allowDistrict: bool = None  # True # Allow region selection
-    searchable: bool = None  # False # whether to display the search box
-    extractValue: bool = None  # True# whether to extract the value, if set to false, the value format will become an
-    # object, including code, province, city and district text information.
-
-
-class InputColor(FormItem):
-    """Color picker"""
-
-    type: str = "input-color"
-    format: str = None  # "hex" # Please choose hex, hls, rgb or rgba.
-    presetColors: List[str] = None  # "Selector preset color value" # The default color at the bottom of the selector,
-    # if the array is empty, the default color will not be displayed
-    allowCustomColor: bool = None  # True # When false, only colors can be selected, use presetColors to set the
-    # color selection range
-    clearable: bool = None  # "label" # whether to display the clear button
-    resetValue: str = None  # "" # After clearing, the form item value is adjusted to this value
-
-
-class Combo(FormItem):
-    """combination"""
-
-    type: str = "combo"
-    formClassName: str = None  # The class name of a single group of form items
-    addButtonClassName: str = None  # Add button CSS class name
-    items: List[FormItem] = None  # Form items displayed in combination
-    # items[x].columnClassName: str = None # The class name of the column, which can be used to configure the column
-    # width. The default is evenly distributed. items[x].unique: bool = None # Set whether the current column value
-    # is unique, that is, repeated selection is not allowed.
-    noBorder: bool = False  # whether to display a border for a single group of form items
-    scaffold: dict = {}  # initial value for a single set of form items
-    multiple: bool = False  # whether to select multiple
-    multiLine: bool = False  # The default is to display a row horizontally, after setting it will be displayed
-    # vertically
-    minLength: int = None  # Minimum number of added bars
-    maxLength: int = None  # The maximum number of bars to add
-    flat: bool = False  # whether to flatten the result (remove the name), only valid when the length of items is 1
-    # and multiple is true.
-    joinValues: bool = True  # The default is true When flattening is enabled, whether to send it to the backend in
-    # the form of a delimiter, otherwise it is in the form of an array.
-    delimiter: str = None  # "False" # What delimiter to use when flattening is on and joinValues is true.
-    addable: bool = False  # whether it can be added
-    addButtonText: str = None  # "Add" # Add button text
-    removable: bool = False  # whether it can be removed
-    deleteApi: API = None  # If configured, an api will be sent before deletion, and the deletion will be completed
-    # after the request is successful
-    deleteConfirmText: str = None  # "Confirm to delete?" # It only takes effect when deleteApi is configured! Used
-    # for user confirmation when deleting
-    draggable: bool = False  # whether drag sorting is possible, it should be noted that when drag sorting is
-    # enabled, there will be an additional $id field
-    draggableTip: str = None  # "Order can be adjusted by dragging the [Exchange] button in each row" # Draggable
-    # prompt text
-    subFormMode: str = None  # "normal" # optional normal, horizontal, inline
-    placeholder: str = None  # "``" # Displayed when there is no member.
-    canAccessSuperData: bool = False  # Specify whether the upper layer data can be automatically obtained and mapped
-    # to the form item
-    conditions: dict = None  # The form of an array contains the rendering types of all conditions. The test in a
-    # single array is the judgment condition, and the items in the array are the schema rendered after meeting the
-    # condition.
-    typeSwitchable: bool = False  # whether to switch conditions, use with conditions
-    strictMode: bool = True  # The default is strict mode. When set to false, when other form items are updated,
-    # the form items in them can also be obtained in time, otherwise they will not.
-    syncFields: List[str] = []  # Configure sync fields. Only valid when strictMode is false.
-    # If the Combo level is deep, the data from the bottom layer may be out of sync. But configuring this property
-    # for combo can be synchronized. Input format: ["os"]
-    nullable: bool = False  # Allow null, if the validator is configured in the sub-form item, and it is a single
-    # mode. You can allow the user to choose to clear (do not fill).
-
-
-class ConditionBuilder(FormItem):
-    """Combined conditions"""
-
-    class Field(AmisNode):
-        type: str = "text"  # The field configuration is configured as "text"
-        label: str = None  # Field name.
-        placeholder: str = None  # placeholder
-        operators: List[str] = None  # If not so many, you can configure overrides.
-        # Default is ['equal','not_equal','is_empty','is_not_empty','like','not_like','starts_with','ends_with']
-        defaultOp: str = None  # defaults to "equal"
-
-    class Text(Field):
-        """text"""
-
-    class Number(Field):
-        """number"""
-
-        type: str = "number"
-        minimum: float = None  # minimum value
-        maximum: float = None  # maximum value
-        step: float = None  # step size
-
-    class Date(Field):
-        """date"""
-
-        type: str = "date"
-        defaultValue: str = None  # default value
-        format: str = None  # Default "YYYY-MM-DD" value format
-        inputFormat: str = None  # Default "YYYY-MM-DD" display date format.
-
-    class Datetime(Date):
-        """Date Time"""
-
-        type: str = "datetime"
-        timeFormat: str = None  # The default "HH:mm" time format determines which input boxes are available.
-
-    class Time(Date):
-        """time"""
-
-        type: str = "datetime"
-
-    class Select(Field):
-        """Drop down to select"""
-
-        type: str = "select"
-        options: OptionsNode = None  # options list, Array<{label: string, value: any}>
-        source: API = None  # Dynamic options, please configure api.
-        searchable: bool = None  # whether it can be searched
-        autoComplete: API = None  # Automatically prompt for completion, each time new content is entered,
-        # the interface will be called, and the update options will be returned according to the interface.
-
-    type: str = "condition-builder"
-    fields: List[Field] = None  # It is an array type, each member represents an optional field, supports multiple
-    # layers, configuration example
-    className: str = None  # Outer dom class name
-    fieldClassName: str = None  # The class name of the input field
-    source: str = None  # Pull configuration items remotely
-
-
-class Editor(FormItem):
-    """Code Editor"""
-
-    type: str = "editor"
-    language: str = None  # "javascript" # The language highlighted by the editor, which can be obtained through the
-    # ${xxx} variable
-    # bat, c, coffeescript, cpp, csharp, css, dockerfile, fsharp, go, handlebars, html, ini, java,
-    # javascript, json, less, lua, markdown, msdax, objective-c, php, plaintext, postiats, powershell,
-    # pug, python, r, razor, ruby, sb, scss, shell, sol, sql, swift, typescript, vb, xml, yaml
-    size: str = None  # "md" # Editor height, the value can be md, lg, xl, xxl
-    allowFullscreen: bool = None  # False # whether to display the full screen mode switch
-    options: dict = None  # Other configurations of the monaco editor, such as whether to display line numbers, etc.,
-    # please refer to here, but readOnly cannot be set, read-only mode needs to use disabled: true
-
-
-class DiffEditor(FormItem):
-    """Code Editor"""
-
-    type: str = "diff-editor"
-    language: str = None  # "javascript" # The language highlighted by the editor, which can be obtained through the
-    # ${xxx} variable
-    # bat, c, coffeescript, cpp, csharp, css, dockerfile, fsharp, go, handlebars, html, ini, java,
-    # javascript, json, less, lua, markdown, msdax, objective-c, php, plaintext, postiats, powershell,
-    # pug, python, r, razor, ruby, sb, scss, shell, sol, sql, swift, typescript, vb, xml, yaml
-    diffValue: Template = None  # the diff value or reference to other data entry like '${value1}'
-
-
-class Formula(AmisNode):
-    """Formula for fields, linked by 'name'"""
-
-    type: str = "formula"
-    name: str = None  # The formula result will be applied to the variable (name) specified here.
-    formula: Expression = None  # the formula itself
-    condition: Expression = None  # condition for the formula
-    initSet: bool = None  # Default True, whether to set at initialization
-    autoSet: bool = None  # Default True, Observe the formula result, if the calculation result changes,
-    # it will be automatically applied to the variable
-    id: bool = None  # Default True, Define a name. When a button's target is specified, it will trigger a formula.
-
-
-class DropDownButton(AmisNode):
-    """Formula for fields, linked by 'name'"""
-
-    type: str = "dropdown-button"
-    label: str = None  # button text
-    className: str = None  # Outer CSS class name
-    btnClassName: str = None  # Button CSS class name
-    menuClassName: str = None  # Dropdown menu CSS class name
-    block: bool = None  # Default False, block style
-    size: Literal["xs", "sm", "md", "lg"] = None  # size, support 'xs', 'sm', 'md','lg'
-    align: Literal["left", "right"] = None  # location align
-    buttons: List[Button] = []  # List of buttons
-    iconOnly: bool = None  # default False, show only icon
-    defaultIsOpened: bool = None  # default False, whether to open by default
-    closeOnOutside: bool = None  # default True, Click whether to collapse the outer area
-    closeOnClick: bool = None  # default False, automatically close dropdown menu after button click
-    trigger: TriggerEnum = TriggerEnum.click  # trigger method
-    hideCaret: bool = None  # default False, Hide drop down icon
-
-
-class EachLoop(AmisNode):
-    """Each loop renderer"""
-
-    type: str = "each"
-    value: list = []  # value for the loop
-    name: str = None  # Data field name
-    source: str = None  # Data mapping source
-    items: dict = None  # {"type": "tpl", "tpl": "< span ..."}
-    placeholder: str = None  # placeholder text when valuevalue does not exist or is an empty array
-
-
-class GridNav(AmisNode):
-    """Grid navigation
-    menu navigation, does not support the configuration of the initialization interface to initialize the data field,
-    so you need to work with similar to Service, Form or CRUD, with the configuration of the interface to initialize
-    the data field components, or manually initialize the data field, and then through the source property,
-    to obtain the data in the data chain to complete the menu display.
-    """
-
-    class OptionsItem(AmisNode):
-        icon: str = None  # default '', list item icon
-        text: str = None  # default '', list item text
-        badge: Badge = None  # Bade Schema, list item badge
-        link: str = None  # default '', Internal page path or external URL address, takes precedence over clickAction
-        blank: bool = None  # default False, Whether a new page is opened, valid when link is url
-        clickAction: Action = None  # ActionSchema
-
-    type: str = "grid-nav"
-    className: str = None  # outer dom classname
-    itemClassName: str = None  # item custom css classname
-    value: List = None  # array of images
-    source: str = None  # data source
-    square: bool = None  # default False, whether to fix list items to be square
-    center: bool = None  # default False, whether to center the content of the list item
-    border: bool = None  # default False, whether to show the list item border
-    gutter: int = None  # default -, px, the spacing between list items
-    reverse: bool = None  # default False, whether to swap the position of the icon and text
-    iconRatio: int = None  # default 60, Icon width ratio, in %
-    direction: Literal["horizontal", "vertical"] = "vertical"  # The direction in which the list items are arranged
-    columnNum: int = None  # default 4,
-    options: List[OptionsItem] = None  # the option items
-
-
-class CollapseGroup(AmisNode):
-    """Grid navigation
-    menu navigation, does not support the configuration of the initialization interface to initialize the data field,
-    so you need to work with similar to Service, Form or CRUD, with the configuration of the interface to initialize
-    the data field components, or manually initialize the data field, and then through the source property,
-    to obtain the data in the data chain to complete the menu display.
-    """
-
-    class CollapseItem(AmisNode):
-        type: str = "collapse"
-        disabled: bool = None  # default False
-        collapsed: bool = None  # default True
-        key: Union[int, str] = None  # default -, logo
-        header: Union[str, SchemaNode] = None  # default -, title
-        body: Union[str, SchemaNode] = None  # default -, content
-
-    type: str = "collapse-group"
-    activeKey: Union[str, int, List[Union[int, str]]] = None  # Initialize the key to activate the panel
-    disabled: bool = None  # default False
-    accordion: bool = None  # default False, accordion mode
-    expandIcon: SchemaNode = None  # Custom toggle icon
-    expandIconPosition: Literal["left", "right"] = "left"  # icon position
-    body: List[Union[CollapseItem, SchemaNode]] = None  # group content
-
-
-class Markdown(AmisNode):
-    """Markdown rendering"""
-
-    type: str = "markdown"
-    name: str = None  # Field name, specifying the key when the form item is submitted
-    value: Union[int, str] = None  # field value
-    className: str = None  # The outermost class name of the form
-    src: API = None  # external address
-    options: dict = None  # html, whether to support html tags, default false;
-    # linkify, whether to automatically identify the link, the default value is true; breaks, whether the carriage
-    # return is a newline, the default value is false
-
-
-class OfficeViewer(AmisNode):
-    """Office Viewer：https://aisuda.bce.baidu.com/amis/zh-CN/components/office-viewer"""
-
-    type: str = "office-viewer"
-    src: API = None  # Document address
-    loading: bool = None  # Whether to display the loading icon
-    enableVar: bool = None  # Whether to enable variable replacement function
-    wordOptions: dict = None  # Word rendering configuration
-
-
-class InputFile(FormItem):
-    """File Upload"""
-
-    type: str = "input-file"
-    receiver: API = None  # Upload file interface
-    accept: str = None  # "text/plain" # Only plain text is supported by default. To support other types,
-    # please configure this property as the file suffix .xxx
-    asBase64: bool = None  # False # Assign the file to the current component in the form of base64
-    asBlob: bool = None  # False # Assign the file to the current component in binary form
-    maxSize: int = None  # There is no limit by default, when set, the file size larger than this value will not be
-    # allowed to upload. unit is B
-    maxLength: int = None  # There is no limit by default. When set, only the specified number of files can be
-    # uploaded at a time.
-    multiple: bool = None  # False # whether to select multiple.
-    joinValues: bool = None  # True # join values
-    extractValue: bool = None  # False # extract value
-    delimiter: str = None  # "," # splicer
-    autoUpload: bool = None  # True # No selection will automatically start uploading
-    hideUploadButton: bool = None  # False # hide the upload button
-    stateTextMap: dict = None  # Upload state text Default: {init: '', pending: 'Waiting to upload', uploading:
-    # 'Uploading', error: 'Upload error', uploaded: 'Uploaded',ready: ''}
-    fileField: str = None  # "file" # You can ignore this attribute if you don't want to store it yourself.
-    nameField: str = None  # "name" # Which field is returned by the interface to identify the file name
-    valueField: str = None  # "value" # The value of the file is identified by that field.
-    urlField: str = None  # "url" # The field name of the file download address.
-    btnLabel: str = None  # The text of the upload button
-    downloadUrl: Union[bool, str] = None  # Version 1.1.6 supports post:http://xxx.com/${value}
-    # When the file path is displayed by default, it will support direct download. It can support adding a prefix
-    # such as: http://xx.dom/filename= . If you don't want this, you can set the current configuration item to false.
-    useChunk: bool = None  # The server where amis is located limits the file upload size to no more than 10M,
-    # so when amis selects a large file, it will automatically change to the chunked upload mode.
-    chunkSize: int = None  # 5 * 1024 * 1024 # chunk size
-    startChunkApi: API = None  # startChunkApi
-    chunkApi: API = None  # chunkApi
-    finishChunkApi: API = None  # finishChunkApi
-    autoFill: Dict[str, str] = None  # After the upload is successful, the value returned by the upload interface can
-    # be filled into a form item by configuring autoFill (not supported under non-form)
-
-
-class InputExcel(FormItem):
-    """Parse Excel"""
-
-    type: str = "input-excel"
-    allSheets: bool = None  # False # whether to parse all sheets
-    parseMode: str = None  # 'array' or 'object' parsing mode
-    includeEmpty: bool = None  # True # whether to include empty values
-    plainText: bool = None  # True # whether to parse as plain text
-
-
-class InputTable(FormItem):
-    """sheet"""
-
-    type: str = "input-table"  # Specify as Table renderer
-    showIndex: bool = None  # False # Show index
-    perPage: int = None  # Set how many pieces of data are displayed on one page. 10
-    addable: bool = None  # False # whether to add a line
-    editable: bool = None  # False # whether editable
-    removable: bool = None  # False # whether it can be removed
-    showAddBtn: bool = None  # True # whether to show the add button
-    addApi: API = None  # API submitted when adding
-    updateApi: API = None  # API submitted when modified
-    deleteApi: API = None  # API submitted when deleting
-    addBtnLabel: Union[bool, Template] = None  # Add button name
-    addBtnIcon: str = None  # "plus" # Add button icon
-    copyBtnLabel: Union[bool, Template] = None  # Copy button text
-    copyBtnIcon: str = None  # "copy" # Copy button icon
-    editBtnLabel: Union[bool, Template] = None  # "" # Edit button name
-    editBtnIcon: str = None  # "pencil" # edit button icon
-    deleteBtnLabel: Union[bool, Template] = None  # "" # delete button name
-    deleteBtnIcon: str = None  # "minus" # delete button icon
-    confirmBtnLabel: Union[bool, Template] = None  # "" # Confirm edit button name
-    confirmBtnIcon: str = None  # "check" # Confirm edit button icon
-    cancelBtnLabel: Union[bool, Template] = None  # "" # Cancel edit button name
-    cancelBtnIcon: str = None  # "times" # Cancel edit button icon
-    needConfirm: bool = None  # True # whether to confirm the operation, it can be used to control the operation
-    # interaction of the control table
-    canAccessSuperData: bool = None  # False # whether you can access the parent data, that is, the same level data
-    # in the form, usually need to be used with strictMode
-    strictMode: bool = None  # True # For performance, the default value of other form items will not update the
-    # current table. Sometimes, in order to obtain other form item fields synchronously, you need to enable this.
-    columns: list = None  # "[]" # Column information
-    # columns[x].quickEdit: boolean|object = None # Use with editable as true columns[x].quickEditOnUpdate:
-    # boolean|object = None # Edit configuration that can be used to distinguish between new mode and update mode
-
-
-class InputGroup(FormItem):
-    """Combination of input boxes"""
-
-    type: str = "input-group"
-    className: str = None  # CSS class name
-    body: List[FormItem] = None  # Form item collection
-
-
-class Group(InputGroup):
-    """Form item group"""
-
-    type: str = "group"
-    mode: DisplayModeEnum = None  # Display the default, the same as the mode in Form
-    gap: str = None  # Gap between form items, optional: xs, sm, normal
-    direction: str = None  # "horizontal" # Can be configured to display horizontally or vertically. The
-    # corresponding configuration items are: vertical, horizontal
-
-
-class InputImage(FormItem):
-    """upload picture"""
-
-    class CropInfo(BaseAmisModel):
-        aspectRatio: float = None  # Crop ratio. Floating point, the default is 1, which is 1:1. If you want to set
-        # 16:9, please set 1.7777777777777777, which is 16/9. .
-        rotatable: bool = None  # False # whether to rotate when cropping
-        scalable: bool = None  # False # whether it can be scaled when cropping
-        viewMode: int = None  # 1 # View mode when cropping, 0 is unlimited
-
-    class Limit(BaseAmisModel):
-        width: int = None  # Limit image width.
-        height: int = None  # Limit image height.
-        minWidth: int = None  # Limit image minimum width.
-        minHeight: int = None  # Limit image minimum height.
-        maxWidth: int = None  # Limit the maximum width of the image.
-        maxHeight: int = None  # Limit the maximum height of the image.
-        aspectRatio: float = None  # Limit the aspect ratio of the image, the format is a floating-point number,
-        # the default is 1, which is 1:1, If you want to set 16:9, please set 1.7777777777777777 which is 16/9. If
-        # you don't want to limit the ratio, set an empty string.
-
-    type: str = "input-image"
-    receiver: API = None  # Upload file interface
-    accept: str = None  # ".jpeg,.jpg,.png,.gif" # Supported picture types and formats, please configure this
-    # property as picture suffix, such as .jpg,.png
-    maxSize: int = None  # There is no limit by default, when set, the file size larger than this value will not be
-    # allowed to upload. unit is B
-    maxLength: int = None  # There is no limit by default. When set, only the specified number of files can be
-    # uploaded at a time.
-    multiple: bool = None  # False # whether to select multiple.
-    joinValues: bool = None  # True # join values
-    extractValue: bool = None  # False # extract value
-    delimiter: str = None  # "," # splicer
-    autoUpload: bool = None  # True # No selection will automatically start uploading
-    hideUploadButton: bool = None  # False # hide the upload button
-    fileField: str = None  # "file" # You can ignore this attribute if you don't want to store it yourself.
-    crop: Union[bool, CropInfo] = None  # Used to set whether to support cropping.
-    cropFormat: str = None  # "image/png" # crop file format
-    cropQuality: int = None  # 1 # The quality of the crop file format, for jpeg/webp, between 0 and 1
-    limit: Limit = None  # Limit the size of the image, beyond which it will not be allowed to upload.
-    frameImage: str = None  # Default placeholder image address
-    fixedSize: bool = None  # whether to enable fixed size, if enabled, set fixedSizeClassName at the same time
-    fixedSizeClassName: str = None  # When the fixed size is turned on, the display size is controlled according to this value.
-    # For example, h-30, that is, the height of the picture frame is h-30, AMIS will automatically set the zoom ratio
-    # to the width of the position occupied by the default image, and the final uploaded image will be scaled
-    # accordingly according to this size.
-    autoFill: Dict[str, str] = None  # After the upload is successful, the value returned by the upload interface can
-    # be filled into a form item by configuring autoFill (not supported under non-form)
-    initAutoFill: bool = None  # False  # 表单反显时是否执行 autoFill
-    uploadBtnText: Union[str, SchemaNode] = None  # 上传按钮文案。支持tpl、schema形式配置。
-    dropCrop: bool = None  # True  # 图片上传后是否进入裁剪模式
-    initCrop: bool = None  # False  # 图片选择器初始化后是否立即进入裁剪模式
-
-
-class LocationPicker(FormItem):
-    """Location"""
-
-    type: str = "location-picker"
-    vendor: str = "baidu"  # Map vendor, currently only Baidu map is implemented
-    ak: str = ...  # ak # registered address of Baidu map: http://lbsyun.baidu.com/
-    clearable: bool = None  # False # whether the input box can be cleared
-    placeholder: str = None  # "Please select a location" # Default prompt
-    coordinatesType: str = None  # "bd09" # Default is Baidu coordinates, can be set to 'gcj02'
-
-
-class InputNumber(FormItem):
-    """Number input box"""
-
-    type: str = "input-number"
-    min: Union[int, Template] = None  # minimum value
-    max: Union[int, Template] = None  # maximum value
-    step: int = None  # step size
-    precision: int = None  # Precision, i.e. a few decimal places
-    showSteps: bool = None  # True # whether to show up and down click buttons
-    prefix: str = None  # prefix
-    suffix: str = None  # suffix
-    kilobitSeparator: bool = None  # Kilobit Separator
-
-
-class Picker(FormItem):
-    """List selector"""
-
-    type: str = "picker"  # List pick, similar in function to Select, but it can display more complex information.
-    size: Union[str, SizeEnum] = None  # Supports: xs, sm, md, lg, xl, full
-    options: OptionsNode = None  # option group
-    source: API = None  # Dynamic option group
-    multiple: bool = None  # whether it is multiple choice.
-    delimiter: bool = None  # False # splicer
-    labelField: str = None  # "label" # option label field
-    valueField: str = None  # "value" # option value field
-    joinValues: bool = None  # True # join values
-    extractValue: bool = None  # False # extract value
-    autoFill: dict = None  # autofill
-    modalMode: Literal["dialog", "drawer"] = None  # "dialog" # Set dialog or drawer to configure the popup mode.
-    pickerSchema: Union["CRUD", SchemaNode] = None  # "{mode: 'list', listItem: {title: '${label}'}}"
-    # That is to use the rendering of the List type to display the list information. More configuration reference CRUD
-    embed: bool = None  # False # whether to use embedded mode
-
-
-class Switch(FormItem):
-    """switch"""
-
-    type: str = "switch"
-    option: str = None  # option description
-    onText: str = None  # Text when it is turned on
-    offText: str = None  # text when off
-    trueValue: Any = None  # "True" # identifies the true value
-    falseValue: Any = None  # "false" # identifies a false value
-
-
-class Static(FormItem):
-    """Static display/label"""
-
-    type: str = "static"  # Support to display other non-form item components static-json|static-datetime by
-
-    # configuring type as static-xxx
-
-    class Json(FormItem):
-        type: str = "static-json"
-        value: Union[dict, str]
-
-    class Datetime(FormItem):
-        """Display date"""
-
-        type: str = "static-datetime"
-        value: Union[int, str]  # support 10-bit timestamp: 1593327764
-
-
-class InputText(FormItem):
-    """Input box"""
-
-    type: str = "input-text"  # input-text|input-url|input-email|input-password|divider
-    options: Union[List[str], List[dict]] = None  # Option group
-    source: API = None  # Dynamic option group
-    autoComplete: API = None  # autocomplete
-    multiple: bool = None  # whether to select multiple
-    delimiter: str = None  # Splice ","
-    labelField: str = None  # option label field "label"
-    valueField: str = None  # option value field "value"
-    joinValues: bool = None  # True # join values
-    extractValue: bool = None  # extract value
-    addOn: SchemaNode = None  # Input box add-ons, such as with a prompt text, or with a submit button.
-    trimContents: bool = None  # whether to remove leading and trailing blank text.
-    creatable: bool = None  # whether it can be created, the default is yes, unless it is set to false, only the
-    # value in the option can be selected
-    clearable: bool = None  # whether it can be cleared
-    resetValue: str = None  # Set the value given by this configuration item after clearing.
-    prefix: str = None  # prefix
-    suffix: str = None  # suffix
-    showCounter: bool = None  # whether to show the counter
-    minLength: int = None  # Limit the minimum number of words
-    maxLength: int = None  # Limit the maximum number of characters
-
-
-class InputPassword(InputText):
-    """Password input box"""
-
-    type: str = "input-password"
-
-
-class InputRichText(FormItem):
-    """Rich Text Editor"""
-
-    type: str = "input-rich-text"
-    saveAsUbb: bool = None  # whether to save in ubb format
-    receiver: API = None  # '' # Default image save API
-    videoReceiver: API = None  # '' # Default video save API
-    size: str = None  # The size of the box, which can be set to md or lg
-    options: dict = None  # Need to refer to tinymce or froala documentation
-    buttons: List[str] = None  # froala dedicated, configure the displayed buttons, tinymce can set the toolbar
-    # string through the previous options
-    vendor: str = None  # "vendor": "froala" , configure to use froala editor
-
-
-class InputRating(FormItem):
-    """Input Rating"""
-
-    type: str = "input-rating"
-    half: bool = None  # default False, whether to use half star selection
-    count: int = None  # default 5, amount of total stars
-    readOnly: bool = None  # default False, is it read only
-    allowClear: bool = None  # default True, allow clearing after another click
-    colors: Union[str, dict] = None  # default {'2': '#abadb1', '3': '#787b81', '5': '#ffa900' }, The color in which
-    # the stars are displayed. If a string is passed in, there is only one color.
-    # If an dict is passed in, each level can be customized.
-    # The key name is the limit value of the segment, and the key value is the corresponding class name.
-    inactiveColor: str = None  # default #e7e7e8, color of unselected stars
-    texts: dict = None  # default -, The tooltip text when the star is selected.
-    # key name is the level of the segment, and the value is the corresponding text
-    textPosition: Literal["right", "left"] = "right"  # position of Tooltip
-    char: str = None  # default '*', custom character
-    charClassNme: str = None  # default -, custom char class name
-    textClassName: str = None  # default -, custom text class name
-
-
-class InputRange(FormItem):
-    """Input Range"""
-
-    type: str = "input-range"
-    min: int = None  # default 0, min value
-    max: int = None  # default 100, max value
-    step: int = None  # default 1, step size
-    showSteps: bool = None  # default False, show step size
-    parts: Union[int, List[int]] = None  # default 1, Number of blocks to split
-    marks: Union[str, dict] = None  # Tick Marks, Support Custom Styles, Set Percentages
-    # { [number | string]: ReactNode }or{ [number | string]: { style: CSSProperties, label: ReactNode } }
-    tooltipVisible: bool = None  # default False, whether to show slider labels
-    tooltipPlacement: PlacementEnum = None  # defualt 'top', tooltip placement 'top'|'right'|'bottom'|'left'
-    multiple: bool = None  # default False, support selection range
-    joinValues: bool = None  # default True, show step size
-    delimiter: str = None  # dfeault ',', value delimiter
-    unit: str = None  # unit
-    clearable: bool = None  # default False, whether the precondition can be cleared : showInputValid when enabled
-    showInput: bool = None  # default False, whether to display the input box
-
-
-class Timeline(AmisNode):
-    """Timeline"""
-
-    class TimelineItem(AmisNode):
-        time: str  # Node Time
-        title: Union[str, SchemaNode] = None  # Node Title
-        detail: str = None  # Node detailed description (collapsed)
-        detailCollapsedText: str = None  # default 'Expand'
-        detailExpandedText: str = None  # default 'Collapse'
-        color: Union[str, LevelEnum] = None  # default #DADBDD, Timeline node color
-        icon: str = None  # Icon name, support fontawesome v4 or use url (priority is higher than color)
-
-    type: str = "timeline"
-    items: List[TimelineItem] = None  # default [], Nodes
-    source: API = None  # Data source, you can obtain current variables through data mapping, or configure API objects
-    mode: Literal["left", "right", "alternate"] = "right"  # Position of the text relative to the timeline,
-    # only supported when direction=vertical
-    direction: Literal["vertical", "horizontal"] = "vertical"  # Direction of the Timeline
-    reverse: bool = None  # default False, Reverse chronological order
-
-
-class Steps(AmisNode):
-    """Steps Bar"""
-
-    class StepItem(AmisNode):
-        title: Union[str, SchemaNode] = None  # Title
-        subTitle: Union[str, SchemaNode] = None  # Sub Heading
-        description: Union[str, SchemaNode] = None  # Detail Description
-        value: str = None  # Step Value
-        icon: str = None  # Icon name, support fontawesome v4 or use url (priority is higher than color)
-        className: str = None  # Custom CSS class name
-
-    type: str = "steps"
-    steps: List[StepItem] = None  # default [], List of Steps
-    source: API = None  # Data source, you can obtain current variables through data mapping, or configure API objects
-    name: str = None  # Associated context variable
-    value: Union[int, str, None] = None  # default -, Set the default value, expressions are not supported
-    status: Union[StepStatusEnum, dict] = None  # default -, State of the steps
-    className: str = None  # Custom CSS class name
-    mode: Literal["vertical", "horizontal"] = "horizontal"  # Specifies the step bar direction.
-    labelPlacement: Literal["vertical", "horizontal"] = "horizontal"  # Specify the label placement position.
-    # The default is to place it horizontally to the right of the icon, and optional (vertical) below the icon.
-    progressDot: bool = None  # Default False, show dotted step bar
-
-
-class TooltipWrapper(AmisNode):
-    type: str = "tooltip-wrapper"
-    className: str = None  # Content area class name
-    tooltipClassName: str = None  # Text prompt floating layer class name
-    style: Union[str, dict] = None  # Custom style (inline style), highest priority
-    tooltipStyle: Union[str, dict] = None  # floating layer custom style
-    body: SchemaNode = None  # Content container
-    wrapperComponent: str = None  # "div" | "span"
-    inline: bool = None  # default False, whether the content area is displayed inline
-    rootClose: bool = None  # default True, whether to click the non-content area to close the prompt
-    mouseEnterDelay: int = None  # default 0, Floating layer delay display time, in ms
-    mouseLeaveDelay: int = None  # default 300, Floating layer delay hiding time, in ms
-    trigger: Union[TriggerEnum, List[TriggerEnum]] = None  # default 'hover', Floating layer trigger mode, support array writing
-    # "hover" | "click" | "focus" | List["hover", "click", "focus"]
-    disabled: bool = None  # default False, whether to disable overlay prompts
-    enterable: bool = None  # default True, whether the mouse can move into the floating layer
-    showArrow: bool = None  # default True, whether to display the overlay pointing arrow
-    offset: Tuple[int, int] = None  # default [0, 0], relative offset of the position of the text prompt, in px
-    tooltipTheme: Literal["light", "dark"] = "light"  # default light, Theme style
-    placement: PlacementEnum = PlacementEnum.top  # text prompts position of the floating layer
-    content: str = None  # default '',  Text prompt content
-    title: str = None  # default '', tooltip title
-
-
-class InputTag(FormItem):
-    """Input Tag"""
-
-    type: str = "input-tag"
-    options: List[Union[str, dict]] = None  # default option group
-    optionsTip: List[Union[str, dict]] = None  # default "Your most recent tags", option hint
-    source: API = None  # default 	Dynamic option group
-    delimiter: str = None  # default False, delimiter option
-    labelField: str = None  # default "label", option label field
-    valueField: str = None  # default "value", option value field
-    joinValues: bool = None  # default True, Splice value
-    extractValue: bool = None  # default False, extract value
-    clearable: bool = None  # default False, whether to show a delete icon on the right when there is a value.
-    resetValue: str = None  # default "", Set the value given by this configuration item after deletion.
-    max: int = None  # Maximum number of tags allowed to be added
-    maxTagLength: int = None  # Maximum text length for a single label
-    maxTagCount: int = None  # The maximum number of labels to be displayed. If the number is exceeded,
-    # it will be displayed in the form of a floating layer.
-    # It will only take effect when the multi-selection mode is enabled.
-    overflowTagPopover: TooltipWrapper = None  # default {"placement": "top", "trigger": "hover", "showArrow": false,
-    # "offset": [0, -10]}	Store the configuration properties of the floating layer,
-    # please refer to Tooltip for detailed configuration
-    enableBatchAdd: bool = None  # default 	False, whether to enable batch add mode
-    separator: str = None  # default "-", After batch adding is enabled, enter the delimiter of multiple labels,
-    # support multiple symbols
-
-
-class Select(FormItem):
-    """Drop down box"""
-
-    type: str = "select"
-    options: OptionsNode = None  # option group
-    source: API = None  # Dynamic option group
-    autoComplete: API = None  # Automatic prompt completion
-    delimiter: Union[bool, str] = None  # False # Splice
-    labelField: str = None  # "label" # option label field
-    valueField: str = None  # "value" # option value field
-    joinValues: bool = None  # True # join values
-    extractValue: bool = None  # False # extract value
-    checkAll: bool = None  # False # whether to support select all
-    checkAllLabel: str = None  # "Select All" # Text to be selected
-    checkAllBySearch: bool = None  # False # When there is a search, only all items hit by the search are selected
-    defaultCheckAll: bool = None  # False # whether to check all by default
-    creatable: bool = None  # False # New option
-    multiple: bool = None  # False # Multiple choice
-    searchable: bool = None  # False # search
-    createBtnLabel: str = None  # "Add option" # Add option
-    addControls: List[FormItem] = None  # Customize new form items
-    addApi: API = None  # Configure the new option interface
-    editable: bool = None  # False # edit options
-    editControls: List[FormItem] = None  # Customize edit form items
-    editApi: API = None  # Configure editing options interface
-    removable: bool = None  # False # remove option
-    deleteApi: API = None  # Configure delete option interface
-    autoFill: dict = None  # autofill
-    menuTpl: str = None  # Supports configuring custom menus
-    clearable: bool = None  # whether to support clearing in radio mode
-    hideSelected: bool = None  # False # hide the selected option
-    mobileClassName: str = None  # Mobile floating class name
-    selectMode: str = None  # Optional: group, table, tree, chained, associated. They are: list form, table form,
-    # tree selection form, Cascade selection form, association selection form (the difference from cascading
-    # selection is that the cascade is infinite, while the association has only one level, and the left side of the
-    # association can be a tree).
-    searchResultMode: str = None  # If the value of selectMode is not set, it can be configured separately. Refer to
-    # selectMode to determine the display form of search results.
-    columns: List[dict] = None  # When the display form is table, it can be used to configure which columns are
-    # displayed, which is similar to the columns configuration in table, but only has the display function.
-    leftOptions: List[dict] = None  # Used to configure the left option set when the display form is associated.
-    leftMode: str = None  # When the display form is associated, it is used to configure the left selection form,
-    # support list or tree. Default is list.
-    rightMode: str = None  # When the display form is associated, it is used to configure the right selection form,
-    # optional: list, table, tree, chained.
-
-
-class ChainedSelect(FormItem):
-    """Chained Drop down boxs"""
-
-    type: str = "chained-select"
-    options: OptionsNode = None  # option group
-    source: API = None  # Dynamic option group
-    autoComplete: API = None  # Automatic prompt completion
-    delimiter: str = None  # Default ',', Splice
-    labelField: str = None  # Default "label", option label field
-    valueField: str = None  # Default "value", option value field
-    joinValues: bool = None  # Default True, join values
-    extractValue: bool = None  # Default False, extract value
-
-
-class NestedSelect(Select):
-    """Cascade selector"""
-
-    type: str = "nested-select"
-    cascade: bool = None  # False # When set to true, child nodes are not automatically selected when the parent node
-    # is selected.
-    withChildren: bool = None  # False # When set to true, when the parent node is selected, the value of the child
-    # node will be included in the value, otherwise only the value of the parent node will be retained.
-    onlyChildren: bool = None  # False # For multiple selections, whether to add only its child nodes to the value
-    # when the parent node is selected.
-    searchPromptText: str = None  # "Enter content to search" # Search box placeholder text
-    noResultsText: str = None  # "No results found" # Text if no results
-    hideNodePathLabel: bool = None  # False # whether to hide the path label information of the selected node in the
-    # selection box
-    onlyLeaf: bool = None  # False # Only leaf nodes are allowed to be selected
-
-
-class Breadcrumb(AmisNode):
-    """Breadcrumb line"""
-
-    class BreadcrumbItem(AmisNode):
-        label: str = None  # label text
-        href: str = None  # link
-        icon: str = None  # fa icon
-        dropdown: List = None  # list of breadcrumbitems as dropdown, needs label, href, icon
-
-    type: str = "breadcrumb"
-    className: str = None  # The outer class name
-    itemClassName: str = None  # Navigation item class name
-    separatorClassName: str = None  # separator class name
-    dropdownClassName: str = None  # Dropdown menu class name
-    dropdownItemClassName: str = None  # Dropdown menu item class name
-    separator: str = ">"  # delimeter
-    labelMaxLength: int = None  # Default 16, max display length
-    tooltipPosition: PlacementEnum = PlacementEnum.top  # tooltip position
-    source: API = None  # dynamic data
-    items: List[BreadcrumbItem] = None  # list of breadcrumb icons
-
-
-class Card(AmisNode):
-    """Card"""
-
-    class Media(AmisNode):
-        type: Literal["image", "video"] = "image"  # multimedia type
-        url: str = None  # image or video link
-        position: PlacementEnum = PlacementEnum.left  # media location
-        className: str = None  # default "w-44 h-28", multimedia CSS class
-        isLive: bool = None  # default False, video is live or not
-        autoPlay: bool = None  # default False, autoplay video
-        poster: Union[bool, str] = None  # default false
-
-    class Header(AmisNode):
-        className: str = None  # The header class name
-        title: str = None  # title
-        titleClassName: str = None  # title class name
-        subTitle: Template = None  # subtitle
-        subTitleClassName: str = None  # subtitle class name
-        subTitlePlaceholder: str = None  # Subtitle placeholder
-        description: Template = None  # Description
-        descriptionClassName: str = None  # Description class name
-        descriptionPlaceholder: str = None  # Description placeholder
-        avatar: Template = None  # picture
-        avatarClassName: str = None  # default "pull-left thumb avatar b-3x m-r", Image includes layer class name
-        imageClassName: str = None  # Image class name
-        avatarText: Template = None  # If no picture is configured, the text will be displayed at the picture
-        avatarTextBackground: str = None  # avatar text background color
-        avatarTextClassName: str = None  # Image text class name
-        highlight: bool = None  # default False, whether to show the active style
-        highlightClassName: str = None  # Active style class name
-        href: str = None  # external link link
-        blank: bool = None  # default True, open link in new window
-
-    type: str = "card"
-    className: str = None  # The outer class name
-    href: str = None  # external link link
-    header: Header = None  # Header object
-    body: List = []  # Content container, mainly used to place non-form item components
-    bodyClassName: str = None  # Content area class name
-    actions: List[Action] = None  # Configure button collection
-    actionsCount: int = None  # default 4, number of buttons in each row
-    itemAction: Action = None  # clicking on a card action
-    media: Media = None  # Media object
-    secondary: Template = None  # secondary note
-    toolbar: List[Action] = None  # toolbar buttons
-    dragging: bool = None  # default False, Whether to show the drag icon
-    selectable: bool = None  # default False, can be selected
-    checkable: bool = None  # default True, selection button is disabled or not
-    selected: bool = None  # default False, selection button is selected or not
-    hideCheckToggler: bool = None  # default False, hide the selection button
-    multiple: bool = None  # default False, multi-select or not
-    useCardLabel: bool = None  # default True, Whether the form item label in the card content area uses the
-    # style inside the Card
-
-
-class Cards(AmisNode):
-    """Cards deck, allows to use data source to display data items as cards, or manual"""
-
-    type: str = "cards"
-    title: str = None  # title
-    source: str = None  # default '${items}', Data source, get the variables in the current data field
-    placeholder: str = None  # default 'No data', placeholder
-    className: str = None  # The outer CSS class name
-    headerClassName: str = None  # default 'amis-grid-header', Top outer CSS class name
-    footerClassName: str = None  # default 'amis-grid-footer', Bottom outer CSS class name
-    itemClassName: str = None  # default 'col-sm-4 col-md-3', Card CSS class name
-    card: Card = None  # configured card object for repeat
-
-
-class ListDisplay(AmisNode):
-    """Cards deck, allows to use data source to display data items as cards, or manual"""
-
-    class ListItem(AmisNode):
-        title: str = None  # title
-        titleClassName: str = None  # title class name
-        subTitle: Template = None  # subtitle
-        avatar: Template = None  # picture
-        avatarClassName: str = None  # default "thumb-sm avatar m-r", Image CSS class name
-        desc: Template = None  # Description
-        body: List = None  # Content container, mainly used to place non-form item components
-        actions: List[Action] = None  # action buttons area
-        actionsPosition: Literal["left", "right"] = "right"  # button position
-
-    type: str = "list"
-    title: str = None  # title
-    source: str = None  # default '${items}', Data source, get the variables in the current data field
-    placeholder: str = None  # default 'No data', placeholder
-    className: str = None  # The outer CSS class name
-    headerClassName: str = None  # default 'amis-grid-header', Top outer CSS class name
-    footerClassName: str = None  # default 'amis-grid-footer', Bottom outer CSS class name
-    listItem: ListItem = None  # configured list object for repeat
-
-
-class Textarea(FormItem):
-    """Multi-line text input box"""
-
-    type: str = "textarea"
-    minRows: int = None  # Minimum number of rows
-    maxRows: int = None  # maximum number of rows
-    trimContents: bool = None  # whether to remove leading and trailing blank text
-    readOnly: bool = None  # read-only
-    showCounter: bool = True  # whether to show the counter
-    minLength: int = None  # Limit the minimum number of words
-    maxLength: int = None  # Limit the maximum number of characters
-
-
-class InputMonth(FormItem):
-    """month"""
-
-    type: str = "input-month"
-    value: str = None  # default value
-    format: str = None  # "X" # Month selector value format, please refer to moment for more format types
-    inputFormat: str = None  # "YYYY-MM" # The display format of the month selector, that is, the timestamp format.
-    # For more format types, please refer to moment
-    placeholder: str = None  # "Please select a month" # placeholder text
-    clearable: bool = None  # True # whether it can be cleared
-
-
-class InputTime(FormItem):
-    """time"""
-
-    type: str = "input-time"
-    value: str = None  # default value
-    timeFormat: str = None  # "HH:mm" # Time selector value format, please refer to moment for more format types
-    format: str = None  # "X" # Time selector value format, please refer to moment for more format types
-    inputFormat: str = None  # "HH:mm" # Time selector display format, that is, timestamp format, please refer to
-    # moment for more format types
-    placeholder: str = None  # "Please select a time" # placeholder text
-    clearable: bool = None  # True # whether it can be cleared
-    timeConstraints: dict = None  # True # Please refer to: react-datetime
-
-
-class InputDatetime(FormItem):
-    """date"""
-
-    type: str = "input-datetime"
-    value: str = None  # default value
-    format: str = None  # "X" # Date time picker value format, please refer to the documentation for more format types
-    inputFormat: str = None  # "YYYY-MM-DD HH:mm:ss" # Date time picker display format, namely timestamp format,
-    # please refer to the documentation for more format types
-    placeholder: str = None  # "Please select a date and time" # placeholder text
-    shortcuts: str = None  # datetime shortcuts
-    minDate: str = None  # Limit the minimum date and time
-    maxDate: str = None  # Limit maximum date time
-    utc: bool = None  # False # save utc value
-    clearable: bool = None  # True # whether it can be cleared
-    embed: bool = None  # False # whether to inline
-    timeConstraints: dict = None  # True # Please refer to: react-datetime
-
-
-class InputDate(FormItem):
-    """date"""
-
-    type: str = "input-date"
-    value: str = None  # default value
-    format: str = None  # "X" # Date picker value format, please refer to the documentation for more format types
-    inputFormat: str = None  # "YYYY-DD-MM" # Date picker display format, that is, timestamp format, please refer to
-    # the documentation for more format types
-    placeholder: str = None  # "Please select a date" # placeholder text
-    shortcuts: str = None  # date shortcuts
-    minDate: str = None  # Limit the minimum date
-    maxDate: str = None  # limit max date
-    utc: bool = None  # False # save utc value
-    clearable: bool = None  # True # whether it can be cleared
-    embed: bool = None  # False # whether to inline mode
-    timeConstraints: dict = None  # True # Please refer to: react-datetime
-    closeOnSelect: bool = None  # False # whether to close the selection box immediately after clicking the date
-    schedules: Union[list, str] = None  # The schedule is displayed in the calendar, static data can be set or data
-    # can be taken from the context, className refers to the background color
-    scheduleClassNames: List[str] = None  # "['bg-warning','bg-danger','bg-success','bg-info','bg-secondary']"
-    # The color of the event displayed in the calendar, refer to the background color
-    scheduleAction: SchemaNode = None  # Custom schedule display
-    largeMode: bool = None  # False # zoom mode
-
-
-class InputQuarter(InputDate):
-    """InputQuarter"""
-
-    type: str = "input-quarter"
-
-
-class InputQuarterRange(FormItem):
-    """Quarter range"""
-
-    type: str = "input-quarter-range"
-    format: str = None  # Default X, date picker value format
-    inputFormat: str = None  # Default 'YYYY-DD', date picker display format
-    placeholder: str = None  # Default 'Please select a quarterly range', placeholder text
-    minDate: str = None  # Limit the minimum date and time, the usage is the same as the limit range
-    maxDate: str = None  # Limit the maximum date and time, the usage is the same as the limit range
-    minDuration: str = None  # Limit the minimum span, such as: 2quarter
-    maxDuration: str = None  # Limit the maximum span, such as: 4quarter
-    utc: bool = None  # Default False, save UTC value
-    clearable: bool = None  # Default True, Is it clearable
-    embed: bool = None  # Default False, inline mode
-    animation: bool = None  # Default True, Whether to enable cursor animation, needs min amis 2.2.0
-
-
-class Calendar(FormItem):
-    """Calendar"""
-
-    class CalendarItem(AmisNode):
-        startTime: str  # ISO 8601 string
-        endTime: str  # ISO 8601 string
-        content: Union[str, int, dict] = None  # Any, static data or get data from the context
-        className: str = None  # css background
-
-    type: str = "calendar"
-    schedules: Union[List[CalendarItem], str] = None  # List of schedule items
-    scheduleClassNames: List[str] = None  # default ['bg-warning', 'bg-danger', 'bg-success', 'bg-info', 'bg-secondary']
-    # color of the event displayed in the calendar, refer to the background color
-
-    scheduleAction: SchemaNode = None  # custom schedule display
-    largeMode: bool = None  # Default False, zoom mode full size
-    todayActiveStyle: Union[str, dict] = None  # Custom styles when activated today
-
-
-class InputKV(FormItem):
-    """Input key-value pair"""
-
-    type: str = "input-kv"
-    valueType: str = None  # Default "input-text", value item type
-    keyPlaceholder: str = None  # key placeholder information
-    valuePlaceholder: str = None  # value placeholder information
-    draggable: bool = None  # Default True, Whether to drag and drop to sort is allowed
-    defaultValue: Union[str, int, dict] = None  # default ''
-
-
-class InputKVS(FormItem):
-    """Input key-value pair, where value can be a deep structure"""
-
-    type: str = "input-kvs"
-    addButtonText: str = None  # default 'new field', butto text of the add button
-    draggable: bool = None  # Default True, Whether to drag and drop to sort is allowed
-    keyItem: Union[str, SchemaNode] = None  # key field
-    valueItems: List[Union[str, SchemaNode]] = None  # items for the key
-
-
-class InputTimeRange(FormItem):
-    """time limit"""
-
-    type: str = "input-time-range"
-    timeFormat: str = None  # "HH:mm" # Time range selector value format
-    format: str = None  # "HH:mm" # time range selector value format
-    inputFormat: str = None  # "HH:mm" # Time range selector display format
-    placeholder: str = None  # "Please select a time range" # placeholder text
-    clearable: bool = None  # True # whether it can be cleared
-    embed: bool = None  # False # whether to inline mode
-
-
-class InputDatetimeRange(InputTimeRange):
-    """Date time range"""
-
-    type: str = "input-datetime-range"
-    ranges: Union[str, List[str]] = None  # "yesterday,7daysago,prevweek,thismonth,prevmonth,prevquarter" date range
-    # shortcut keys, Optional: today,yesterday,1dayago,7daysago,30daysago,90daysago,prevweek,thismonth,thisquarter,
-    # prevmonth,prevquarter
-    minDate: str = None  # Limit the minimum date and time, the usage is the same as the limit range
-    maxDate: str = None  # Limit the maximum date and time, the usage is the same as the limit range
-    utc: bool = None  # False # save UTC value
-
-
-class InputDateRange(InputDatetimeRange):
-    """Date Range"""
-
-    type: str = "input-date-range"
-    minDuration: str = None  # Limit the minimum span, such as: 2days
-    maxDuration: str = None  # Limit the maximum span, such as: 1year
-
-
-class InputMonthRange(InputDateRange):
-    """month range"""
-
-    type: str = "input-month-range"
-
-
-class Transfer(FormItem):
-    """Shuttle"""
-
-    type: Literal["transfer", "transfer-picker", "tabs-transfer", "tabs-transfer-picker"] = "transfer"
-    options: OptionsNode = None  # option group
-    source: API = None  # Dynamic option group
-    delimiter: str = None  # "False" # splicer
-    joinValues: bool = None  # True # join values
-    extractValue: bool = None  # False # extract value
-    searchable: bool = None  # False When set to true, it means that options can be retrieved by entering partial content.
-    searchApi: API = None  # If you want to retrieve through the interface, you can set an api.
-    statistics: bool = None  # True # whether to display statistics
-    selectTitle: str = None  # "Please select" # Title text on the left
-    resultTitle: str = None  # "current selection" # title text of the result on the right
-    sortable: bool = None  # False # The result can be sorted by drag and drop
-    selectMode: str = None  # "list" # Optional: list, table, tree, chained, associated. They are: list form,
-    # table form, tree selection form, Cascade selection form, association selection form (the difference from
-    # cascading selection is that the cascade is infinite, while the association has only one level, and the left
-    # side of the association can be a tree).
-    searchResultMode: str = None  # If the value of selectMode is not set, it can be configured separately. Refer to
-    # selectMode to determine the display form of search results.
-    columns: List[dict] = None  # When the display form is table, it can be used to configure which columns are
-    # displayed, which is similar to the columns configuration in table, but only has the display function.
-    leftOptions: List[dict] = None  # Used to configure the left option set when the display form is associated.
-    leftMode: str = None  # When the display form is associated, it is used to configure the left selection form,
-    # support list or tree. Default is list.
-    rightMode: str = None  # When the display form is associated, it is used to configure the right selection form,
-    # optional: list, table, tree, chained.
-    menuTpl: SchemaNode = None  # Used to customize option display
-    valueTpl: SchemaNode = None  # Used to customize the display of the value
-
-
-class TransferPicker(Transfer):
-    """Shuttle selector"""
-
-    type: str = "transfer-picker"
-
-
-class TabsTransfer(Transfer):
-    """Combination shuttle"""
-
-    type: str = "tabs-transfer"
-
-
-class TabsTransferPicker(Transfer):
-    """Combination shuttle selector"""
-
-    type: str = "tabs-transfer-picker"
-
-
-class InputTree(FormItem):
-    """Tree selection box"""
-
-    type: str = "input-tree"
-    options: OptionsNode = None  # option group
-    source: API = None  # Dynamic option group
-    autoComplete: API = None  # Automatic prompt completion
-    multiple: bool = None  # False # whether to select multiple
-    delimiter: str = None  # "False" # splicer
-    labelField: str = None  # "label" # option label field
-    valueField: str = None  # "value" # option value field
-    iconField: str = None  # "icon" # icon value field
-    joinValues: bool = None  # True # join values
-    extractValue: bool = None  # False # extract value
-    creatable: bool = None  # False # New option
-    addControls: List[FormItem] = None  # Customize new form items
-    addApi: API = None  # Configure the new option interface
-    editable: bool = None  # False # edit options
-    editControls: List[FormItem] = None  # Customize edit form items
-    editApi: API = None  # Configure editing options interface
-    removable: bool = None  # False # remove option
-    deleteApi: API = None  # Configure delete option interface
-    searchable: bool = None  # False # whether it is searchable, it only takes effect when type is tree-select
-    hideRoot: bool = None  # True # Set to false if you want to show a top-level node
-    rootLabel: bool = None  # "top level" # Useful when hideRoot is not false, used to set the text of the top level node.
-    showIcon: bool = None  # True # whether to show the icon
-    showRadio: bool = None  # False # whether to show radio buttons, multiple is false is valid.
-    initiallyOpen: bool = None  # True # Set whether to expand all levels by default.
-    unfoldedLevel: int = None  # 0 # Set the default unfolded level, which only takes effect when initiallyOpen is
-    # not true.
-    cascade: bool = None  # False # Do not automatically select child nodes when parent node is selected.
-    withChildren: bool = None  # False # When the parent node is selected, the value will contain the value of the
-    # child node, otherwise only the value of the parent node will be retained.
-    onlyChildren: bool = None  # False # For multiple selections, whether to add only its child nodes to the value
-    # when the parent node is selected.
-    rootCreatable: bool = None  # False # whether top-level nodes can be created
-    rootCreateTip: str = None  # "Add a first-level node" # Create a hovering tip for a top-level node
-    minLength: int = None  # Minimum number of selected nodes
-    maxLength: int = None  # Maximum number of nodes selected
-    treeContainerClassName: str = None  # tree outermost container class name
-    enableNodePath: bool = None  # False # whether to enable node path mode
-    pathSeparator: str = None  # "/" # The separator of the node path, it takes effect when enableNodePath is true
-    deferApi: API = None  # For lazy loading options, please configure defer to true, and then configure deferApi to
-    # complete lazy loading
-    selectFirst: bool = None
-    showOutline: bool = None  # False  # 是否显示树层级展开线
-    autoCheckChildren: bool = None  # True  # 当选中父节点时级联选择子节点。
-    onlyLeaf: bool = None  # False  # 只允许选择叶子节点
-    highlightTxt: str = None  # None  # 标签中需要高亮的字符，支持变量
-    itemHeight: int = None  # 32  # 每个选项的高度，用于虚拟渲染
-    virtualThreshold: int = None  # 100  # 在选项数量超过多少时开启虚拟渲染
-    menuTpl: str = None  # 选项自定义渲染 HTML 片段
-    enableDefaultIcon: bool = None  # True  # 是否为选项添加默认的前缀 Icon，父节点默认为folder，叶节点默认为file
-    heightAuto: bool = None  # False  # 默认高度会有个 maxHeight，即超过一定高度就会内部滚动，如果希望自动增长请设置此属性
-
-
-class TreeSelect(InputTree):
-    """Tree selector"""
-
-    type: str = "tree-select"
-    hideNodePathLabel: bool = None  # whether to hide the path label information of the selected node in the selection box
-
-
-class Image(AmisNode):
-    """picture"""
-
-    type: str = "image"  # "image" if used in Table, Card and List; "static-image" if used as static display in Form
-    className: str = None  # Outer CSS class name
-    imageClassName: str = None  # Image CSS class name
-    thumbClassName: str = None  # Thumbnail CSS class name
-    height: int = None  # Image reduction height
-    width: int = None  # Image reduction width
-    title: str = None  # title
-    imageCaption: str = None  # description
-    placeholder: str = None  # placeholder text
-    defaultImage: str = None  # The image displayed when there is no data
-    src: str = None  # Thumbnail address
-    href: Template = None  # External link address
-    originalSrc: str = None  # Original image address
-    enlargeAble: bool = None  # Support zoom in preview
-    enlargeTitle: str = None  # enlarge the title of the preview
-    enlargeCaption: str = None  # Description of the enlarged preview
-    thumbMode: str = None  # "contain" # preview mode, optional: 'w-full','h-full','contain','cover'
-    thumbRatio: str = None  # "1:1" # Preview ratio, optional: '1:1','4:3','16:9'
-    imageMode: str = None  # "thumb" Image display mode, optional: 'thumb', 'original' ie: thumbnail mode or original
-    # image mode
-
-
-class Images(AmisNode):
-    """Photo album"""
-
-    type: str = "images"  # "images" if used in Table, Card and List; "static-images" if used as static display in Form
-    className: str = None  # Outer CSS class name
-    defaultImage: str = None  # Default display image
-    value: Union[str, List[str], List[dict]] = None  # Image array
-    source: str = None  # data source
-    delimiter: str = None  # "," # Delimiter, when value is a string, use this value to separate and split
-    src: str = None  # Preview image address, support data mapping to obtain image variables in the object
-    originalSrc: str = None  # Original image address, support data mapping to obtain image variables in the object
-    enlargeAble: bool = None  # Support zoom in preview
-    thumbMode: str = None  # "contain" # preview mode, optional: 'w-full','h-full','contain','cover'
-    thumbRatio: str = None  # "1:1" # Preview ratio, optional: '1:1','4:3','16:9'
-
-
-class Carousel(AmisNode):
-    """Carousel"""
-
-    class Item(AmisNode):
-        image: str = None  # Image link
-        href: str = None  # Image open URL link
-        imageClassName: str = None  # Image class name
-        title: str = None  # image title
-        titleClassName: str = None  # Image title class name
-        description: str = None  # Picture description
-        descriptionClassName: str = None  # Picture description class name
-        html: str = None  # HTML custom, same as Tpl
-
-    type: str = "carousel"  # Specify as the Carousel renderer
-    className: str = None  # "panel-default" # The class name of the outer Dom
-    options: List[Item] = None  # "[]" # Carousel panel data
-    itemSchema: dict = None  # custom schema to display data
-    auto: bool = True  # whether to rotate automatically
-    interval: str = None  # "5s" # Switch animation interval
-    duration: str = None  # "0.5s" # Switch animation duration
-    width: str = None  # "auto" # width
-    height: str = None  # "200px" # height
-    controls: List[str] = None  # "['dots','arrows']" # Display left and right arrows, bottom dot index
-    controlsTheme: str = None  # "light" # Left and right arrows, bottom dot index color, default light, and dark mode
-    animation: str = None  # "fade" # Switch animation effect, default fade, and slide mode
-    thumbMode: str = None  # "cover"|"contain" # The default zoom mode of the picture
-
-
-class Mapping(AmisNode):
-    """Mapping"""
-
-    type: str = "mapping"  # "mapping" if used in Table, Card and List; "static-mapping" if used as static display in Form
-    className: str = None  # Outer CSS class name
-    placeholder: str = None  # placeholder text
-    map: dict = None  # map configuration
-    source: API = None  # API or data map
-
-
-class CRUD(AmisNode):
-    """Add, delete, modify, check"""
-
-    class Messages(AmisNode):
-        fetchFailed: str = None  # Prompt when fetch fails
-        saveOrderFailed: str = None  # Failed to save order
-        saveOrderSuccess: str = None  # Save order success prompt
-        quickSaveFailed: str = None  # Quick save failure prompt
-        quickSaveSuccess: str = None  # Quick save success prompt
-
-    type: str = "crud"  # type specifies the CRUD renderer
-    mode: str = None  # "table" # "table" , "cards" or "list"
-    title: str = None  # "" # Can be set to empty, when set to empty, there is no title bar
-    className: str = None  # The class name of the outer Dom of the table
-    api: API = None  # The api that CRUD uses to get list data.
-    loadDataOnce: bool = None  # whether to load all data at once (front-end paging)
-    loadDataOnceFetchOnFilter: bool = None  # True # When loadDataOnce is turned on, whether to re-request the api
-    # when filtering
-    source: str = None  # The data mapping interface returns the value of a field. If it is not set, the ${items} or
-    # ${rows} returned by the interface will be used by default. It can also be set to the content of the upper data
-    # source.
-    filter: Union[SchemaNode, Form] = None  # Set the filter, when the form is submitted, it will bring the data to
-    # the current mode refresh list.
-    filterTogglable: bool = None  # False # whether the filter can be displayed or hidden
-    filterDefaultVisible: bool = None  # True # Set whether the filter is visible by default.
-    initFetch: bool = None  # True # whether to pull data during initialization, only for the case with filter,
-    # without filter, data will be pulled initially
-    interval: int = None  # refresh time (minimum 1000)
-    silentPolling: bool = None  # Configure whether to hide the loading animation when refreshing
-    stopAutoRefreshWhen: str = None  # Configure the condition for stopping refresh by expression
-    stopAutoRefreshWhenModalIsOpen: bool = None  # Turn off auto refresh when there is a popup, close the popup and
-    # restore
-    syncLocation: bool = None  # False # whether to synchronize the parameters of the filter conditions to the
-    # address bar, !!! After opening, the data type may be changed, and it cannot pass the fastpi data verification
-    draggable: bool = None  # whether it can be sorted by dragging
-    itemDraggableOn: bool = None  # Use expressions to configure whether drag and drop sorting is possible
-    saveOrderApi: API = None  # Save order api.
-    quickSaveApi: API = None  # API for batch saving after quick editing.
-    quickSaveItemApi: API = None  # API to use when quick edit is configured to save in time.
-    bulkActions: List[Action] = None  # Batch operation list, after configuration, the table can be selected.
-    defaultChecked: bool = None  # When batch operations are available, whether to check all by default.
-    messages: Messages = None  # Override the message prompt, if not specified, the message returned by the api will
-    # be used
-    primaryField: str = None  # Set the ID field name. 'id'
-    perPage: int = None  # Set how many pieces of data are displayed on one page. 10
-    defaultParams: dict = None  # Set the default filter default parameters, which will be sent to the backend
-    # together when querying
-    pageField: str = None  # Set the pagination page number field name. "page"
-    perPageField: str = None  # "perPage" # Set the field name of how many pieces of data are displayed on one page.
-    # Note: Best used with defaultParams, see example below.
-    perPageAvailable: List[int] = None  # [5, 10, 20, 50, 100] # Set how many data drop-down boxes can be displayed
-    # on one page.
-    orderField: str = None  # Set the field name used to determine the position. After setting, the new order will be
-    # assigned to this field.
-    hideQuickSaveBtn: bool = None  # Hide the top quick save prompt
-    autoJumpToTopOnPagerChange: bool = None  # whether to automatically jump to the top when splitting pages.
-    syncResponse2Query: bool = None  # True # Synchronize the returned data to the filter.
-    keepItemSelectionOnPageChange: bool = None  # True
-    # Retain item selection. After the default paging and searching, the user-selected item will be cleared. After
-    # this option is enabled, the user's selection will be retained, enabling cross-page batch operations.
-    labelTpl: str = None  # Single description template, keepItemSelectionOnPageChange
-    # When set to true, all selected items will be listed. This option can be used to customize the entry display copy.
-    headerToolbar: list = None  # ['bulkActions','pagination'] # Top toolbar configuration
-    footerToolbar: list = None  # ['statistics','pagination'] # Bottom toolbar configuration
-    alwaysShowPagination: bool = None  # whether to always show pagination
-    affixHeader: bool = None  # True # whether to fix the header (under table)
-    autoGenerateFilter: bool = None  # whether to open the query area, after it is enabled, the query condition form
-    # will be automatically generated according to the searchable attribute value of the column element
-    itemAction: Action = None  # Implement custom actions after clicking a row, support all configurations in action,
-    # such as pop-up boxes, refresh other components, etc.
-    resizable: bool = None  # 是否可以调整列宽度
-    orderBy: str = None  # 默认排序字段，这个是传给后端，需要后端接口实现
-    orderDir: Literal["asc", "desc"] = None  # 排序方向
-    resetPageAfterAjaxItemAction: bool = None  # False  # 单条数据 ajax 操作后是否重置页码为第一页
-    autoFillHeight: Union[bool, Dict[str, int]] = None  # 内容区域自适应高度
-
-
-class TableColumn(AmisNode):
-    """Column configuration"""
-
-    type: str = None  # Literal['text','audio','image','link','tpl','mapping','carousel','date',
-    # 'progress','status','switch','list','json','operation','tag']
-    label: Template = None  # header text content
-    name: str = None  # Associate data by name
-    tpl: Template = None  # Template
-    fixed: str = None  # whether to fix the current column left|right|none
-    popOver: Union[bool, dict] = None  # popover
-    quickEdit: Union[bool, dict] = None  # quick edit
-    copyable: Union[bool, dict] = None  # whether to copy boolean or {icon: string, content:string}
-    sortable: bool = None  # False # whether it is sortable
-    searchable: Union[bool, SchemaNode] = None  # False # whether to quickly search boolean|Schema
-    width: Union[int, str] = None  # column width
-    remark: RemarkT = None  # prompt message
-    breakpoint: str = None  # *,ls. When there are too many columns, the content cannot be displayed completely,
-    # some information can be displayed at the bottom, and users can expand to view the details
-    filterable: Union[bool, Dict[str, Any]] = None  # filter configuration
-    toggled: bool = None  # whether to expand by default, in the column configuration, you can configure toggled to
-    # false to not display this column by default
-    backgroundScale: int = None  # Can be used to automatically assign color scales based on data control
-
-
-class ColumnOperation(TableColumn):
-    """Action column"""
-
-    type: str = "operation"
-    buttons: List[Union[Action, AmisNode]] = None
-
-
-class ColumnImage(Image, TableColumn):
-    """Picture column"""
-
-    pass
-
-
-class ColumnImages(Images, TableColumn):
-    """Picture collection column"""
-
-    pass
-
-
-class ColumnMapping(Mapping, TableColumn):
-    """Map column"""
-
-    pass
-
-
-class Table(AmisNode):
-    """sheet"""
-
-    type: str = "table"  # Specify as table renderer
-    title: str = None  # title
-    source: str = None  # "${items}" # Data source, bind the current environment variable
-    affixHeader: bool = None  # True # whether to fix the header
-    columnsTogglable: Union[bool, str] = None  # "auto" # Display column display switch, automatic: it is
-    # automatically turned on when the number of columns is greater than or equal to 5
-    placeholder: str = None  # "No data" # Text prompt when there is no data
-    className: str = None  # "panel-default" # Outer CSS class name
-    tableClassName: str = None  # "table-db table-striped" # table CSS class name
-    headerClassName: str = None  # "Action.md-table-header" # Top outer CSS class name
-    footerClassName: str = None  # "Action.md-table-footer" # Bottom outer CSS class name
-    toolbarClassName: str = None  # "Action.md-table-toolbar" # Toolbar CSS class name
-    columns: List[Union[TableColumn, SchemaNode]] = None  # Used to set column information
-    combineNum: int = None  # Automatically combine cells
-    itemActions: List[Action] = None  # Floating row action button group
-    itemCheckableOn: Expression = None  # Configure the condition for whether the current row can be checked, use an
-    # expression
-    itemDraggableOn: Expression = None  # To configure whether the current row can be dragged or not, use an expression
-    checkOnItemClick: bool = None  # False # whether clicking on the data row can check the current row
-    rowClassName: str = None  # Add CSS class name to row
-    rowClassNameExpr: Template = None  # Add CSS class name to row via template
-    prefixRow: list = None  # top summary row
-    affixRow: list = None  # Bottom summary row
-    itemBadge: "Badge" = None  # Row badge configuration
-    autoFillHeight: bool = None  # Content area adaptive height
-    footable: Union[bool, dict] = None  # When there are too many columns, the content cannot be fully displayed.
-    # Some information can be displayed at the bottom, allowing users to expand to view the details. The
-    # configuration is very simple, just turn on the footable attribute, and add a breakpoint attribute to the column
-    # you want to display at the bottom as *.
-    resizable: bool = None  # 列宽度是否支持调整
-    selectable: bool = None  # 支持勾选
-    multiple: bool = None  # 勾选 icon 是否为多选样式checkbox， 默认为radio
-
-
-class Chart(AmisNode):
-    """Chart: https://echarts.apache.org/en/option.html#title"""
-
-    type: str = "chart"  # specify the chart renderer
-    className: str = None  # The class name of the outer Dom
-    body: SchemaNode = None  # Content container
-    api: API = None  # Configuration item interface address
-    source: dict = None  # Get the variable value in the data chain as configuration through data mapping
-    initFetch: bool = None  # whether to request the interface when the component is initialized
-    interval: int = None  # refresh time (minimum 1000)
-    config: Union[dict, str] = None  # Set the configuration item of eschars, when it is string, you can set
-    # configuration items such as function
-    style: dict = None  # Set the style of the root element
-    width: str = None  # Set the width of the root element
-    height: str = None  # Set the height of the root element
-    replaceChartOption: bool = None  # False # Does each update completely overwrite the configuration item or append it?
-    trackExpression: str = None  # Update the chart when the value of this expression changes
-
-
-class Code(AmisNode):
-    """Code highlighting"""
-
-    type: str = "code"
-    className: str = None  # Outer CSS class name
-    value: str = None  # display color value
-    name: str = None  # In other components, when used as variable mapping
-    language: str = None  # The highlighted language used, the default is plaintext
-    tabSize: int = None  # 4 # Default tab size
-    editorTheme: str = None  # "'vs'" # theme, and 'vs-dark'
-    wordWrap: str = None  # "True" # whether to wrap
-
-
-class Json(AmisNode):
-    """JSON display component"""
-
-    type: str = "json"  # "json" if in Table, Card and List; "static-json" if used for static display in Form
-    className: str = None  # Outer CSS class name
-    value: Union[dict, str] = None  # json value, if it is string, it will be parsed automatically
-    source: str = None  # Get the value in the data chain through the data map
-    placeholder: str = None  # placeholder text
-    levelExpand: int = None  # 1 # Default expanded level
-    jsonTheme: str = None  # "twilight" # Theme, optional twilight and eighties
-    mutable: bool = None  # False # whether it can be modified
-    displayDataTypes: bool = None  # False # whether to display data types
-
-
-class Link(AmisNode):
-    """Link"""
-
-    type: str = "link"  # "link" if used in Table, Card and List; "static-link" if used as static display in Form
-    body: str = None  # Text inside the tag
-    href: str = None  # link address
-    blank: bool = None  # whether to open in a new tab
-    htmlTarget: str = None  # The target of the a tag, which takes precedence over the blank attribute
-    title: str = None  # the title of the a tag
-    disabled: bool = None  # disable hyperlinks
-    icon: str = None  # Hyperlink icon to enhance display
-    rightIcon: str = None  # right icon
-
-
-class Log(AmisNode):
-    """Real-time log"""
-
-    type: str = "log"
-    source: API = None  # Support variables, which can be initially set to empty, so that it will not be loaded
-    # initially, and will be loaded when the variable has a value
-    height: int = None  # 500 # Display area height
-    className: str = None  # Outer CSS class name
-    autoScroll: bool = None  # True # whether to scroll automatically
-    placeholder: str = None  # The text being loaded
-    encoding: str = None  # "utf-8" # The character encoding of the returned content
-
-
-class Property(AmisNode):
-    """Property sheet"""
-
-    class Item(AmisNode):
-        label: Template = None  # attribute name
-        content: Template = None  # attribute value
-        span: int = None  # attribute values span several columns
-        visibleOn: Expression = None  # Display expression
-        hiddenOn: Expression = None  # hidden expression
-
-    type: str = "property"
-    className: str = None  # The class name of the outer dom
-    style: dict = None  # The style of the outer dom
-    labelStyle: dict = None  # style of attribute name
-    contentStyle: dict = None  # style of attribute value
-    column: int = None  # 3 # several columns per row
-    mode: str = None  # 'table' # Display mode, currently only 'table' and 'simple'
-    separator: str = None  # ',' # Separator between attribute name and value in 'simple' mode
-    source: Template = None  # data source
-    title: str = None  # title
-    items: List[Item] = None  # data items
-
-
-class QRCode(AmisNode):
-    """QR code"""
-
-    type: str = "qr-code"  # Specify as QRCode renderer
-    value: Template  # The text displayed after scanning the QR code, if you want to display a page, please enter the
-    # full url (starting with "http://..." or "https://..."), templates are supported
-    className: str = None  # The class name of the outer Dom
-    qrcodeClassName: str = None  # QR code SVG class name
-    codeSize: int = None  # 128 # The width and height of the QR code
-    backgroundColor: str = None  # "#fff" # QR code background color
-    foregroundColor: str = None  # "#000" # QR code foreground color
-    level: str = None  # "L" # QR code complexity level, there are four types ('L' 'M' 'Q' 'H')
-
-
-class Barcode(AmisNode):
-    """Barcode"""
-
-    class Options(AmisNode):
-        format: BarcodeEnum = BarcodeEnum.auto  # The format of the barcode
-        width: int = None  # default 2 width of the barcode image
-        height: int = None  # default 100 height of the barcode image
-        displayValue: bool = None  # default True
-        text: str = None
-        fontOptions: str = ""
-        font: str = None  # default "monospace"
-        textAlign: str = None  # default "center"
-        textPosition: str = None  # default "bottom"
-        textMargin: int = None  # default 2
-        fontSize: int = None  # default 20
-        background: str = None  # #ffffff CSS Color
-        lineColor: str = None  # #000000 CSS color
-        margin: int = None  # default 10
-        marginTop: int = None
-        marginBottom: int = None
-        marginLeft: int = None
-        marginRight: int = None
-        flat: bool = None  # default False, no guard bars if True
-
-    type: str = "barcode"  # Specify as QRCode renderer
-    value: str = None  # The value of the barcode
-    className: str = None  # The class name of the outer Dom
-    options: Options = None
-
-
-class Color(AmisNode):
-    type: Literal["color", "static-color"] = "color"
-    value: str = None  # The value of the color CSS code
-    className: str = None  # The class name of the outer Dom
-    defaultColor: str = None  # "#ccc" default color value
-    showValue: bool = None  # default True, whether to display the color value on the right
-
-
-class Progress(AmisNode):
-    type: Literal["progress", "static-progress"] = "progress"
-    mode: ProgressEnum = None  # The type of progress "bar", optional
-    value: Template = None  # The value of the progress
-    className: str = None  # The class name of the outer Dom
-    showLabel: bool = None  # default True, whether to show progress text
-    stripe: bool = None  # default False
-    animate: bool = None  # default False
-    map: Union[str, List[str], List[Dict]] = None  # progress colormap, as dict = {value:number, color:string}
-    # default ['bg-danger', 'bg-warning', 'bg-info', 'bg-success', 'bg-success']
-    threshold: Union[Dict, List] = None  # default -,
-    # {value: template , color?: template } | List[{value: template , color?: template }]
-    showThresholdText: bool = None  # default False, whether to display the threshold (scale) value
-    valueTpl: str = None  # default ${value}%, custom formatted content
-    strokeWidth: int = None  # default 10 by circle, 6 with dashboard
-    gapDegree: int = None  # default 75, angle of the missing corner of the instrument panel, the value can be 0 ~ 295
-    gapPosition: str = None  # default "bottom", Dashboard progress bar notch position, optional top bottom left right
-
-
-class PaginationWrapper(AmisNode):
-    type: str = "pagination-wrapper"
-    showPageInput: bool = None  # default False, whether to display the quick jump input box
-    maxButtons: int = None  # default 5, Maximum number of pagination buttons to display
-    inputName: str = None  # default 'items', input field name
-    outputName: str = None  # default 'items', output field name
-    perPage: int = None  # default 10, Display multiple pieces of data per page
-    position: Literal["top", "none", "bottom"] = "top"  # Pagination display position, if it is configured as none,
-    # you need to configure the pagination component in the content area, otherwise it will not be displayed
-    body: SchemaNode = None  # Display content
-
-
-class Pagination(AmisNode):
-    type: str = "pagination"
-    mode: Literal["simple", "normal"] = "normal"  # The mini version/simple version only displays left and right arrows,
-    # used with hasNext
-    layout: Union[str, List[str]] = None  # default 'pager', Adjust the paging structure layout by controlling
-    # the order of the layout properties
-    maxButtons: int = None  # default 10, Display multiple pieces of data per page
-    lastPage: int = None  # lastPage will be recalculated when the total number of entries is set
-    total: int = None  # total number of pages
-    activePage: int = None  # default 1, current page number
-    perPage: int = None  # default 10, Display multiple pieces of data per page
-    showPerPage: bool = None  # default False, whether to display the perPage switcher layout
-    perPageAvailable: List[int] = None  # default [10, 20, 50, 100], how many lines can be displayed per page
-    showPageInput: bool = None  # default False, whether to display the quick jump input box layout
-    disabled: bool = None  # default False, is pagination disabled
-
-
-class MatrixCheckboxes(FormItem):
-    """Matrix type input box."""
-
-    class RowItem(AmisNode):
-        label: str
-
-    class ColumnItem(AmisNode):
-        label: str
-
-    type: str = "matrix-checkboxes"
-    columns: List[ColumnItem] = None  # list of column items
-    rows: List[RowItem] = None  # list of row items
-    rowLabel: str = None  # row header description
-    source: API = None  # Api address, if the option group is not fixed.
-    multiple: bool = None  # default False, multiple choice
-    singleSelectMode: Literal["false", "cell", "row", "column"] = "column"
-
-
-class Wrapper(AmisNode):
-    type: str = "wrapper"
-    className: str = None  # The class name of the outer Dom
-    style: Union[str, dict] = None  # Custom style (inline style), highest priority
-    body: SchemaNode = None  # Display content
-    size: Union[str, SizeEnum] = None  # Specify the wrapper size, support: xs, sm, md, lg
-
-
-class WebComponent(AmisNode):
-    type: str = "web-component"
-    tag: str = None  # The specific web-component tag used
-    style: Union[str, dict] = None  # Custom style (inline style), highest priority
-    body: SchemaNode = None  # child node
-    props: dict = None  # attributes by their labels
-
-
-class UUIDField(AmisNode):
-    """Randomly generates an id that can be used to prevent repeated form submissions."""
-
-    type: str = "uuid"
-    name: str = None  # The field name
-    length: int = None  # if set, generates short random numbers, if not set it generates a UUID
-
-
-class SearchBox(AmisNode):
-    type: str = "search-box"
-    className: str = None  # The class name of the outer Dom
-    mini: bool = None  # default False, whether it is in mini mode
-    searchImediately: bool = None  # default False, whether to search now
-
-
-class Sparkline(AmisNode):
-    type: str = "sparkline"
-    width: int = None  # width of the sparkline image
-    height: int = None  # height of the sparkline image
-    value: List[Union[int, float]] = None  #
-    clickAction: Action = None  # Action when clicked
-
-
-class Tag(AmisNode):
-    type: str = "tag"
-    className: str = None  # Custom CSS style class name
-    displayMode: Literal["normal", "rounded", "status"] = "normal"  # Display mode
-    closable: bool = None  # default False, show close icon
-    color: str = None  # color theme or custom color value,
-    # 'active' | 'inactive' | 'error' | 'success' | 'processing' | 'warning'
-    label: str = None  # default '-'
-    icon: str = None  # custom font icon
-    style: Union[str, dict] = None  # Custom style (inline style), highest priority
-
-
-class Video(AmisNode):
-    """video"""
-
-    type: str = "video"  # specify the video renderer
-    className: str = None  # The class name of the outer Dom
-    src: str = None  # video address
-    isLive: bool = None  # False # whether it is a live broadcast, it needs to be added when the video is live,
-    # supports flv and hls formats
-    videoType: str = None  # Specify the live video format
-    poster: str = None  # Video cover address
-    muted: bool = None  # whether to mute
-    autoPlay: bool = None  # whether to play automatically
-    rates: List[float] = None  # Multiples in the format [1.0, 1.5, 2.0]
-
-
-class Alert(AmisNode):
-    """hint"""
-
-    type: str = "alert"  # Specify as the alert renderer
-    className: str = None  # The class name of the outer Dom
-    level: str = None  # "info" # Level, can be: info, success, warning or danger
-    body: SchemaNode = None  # Display content
-    showCloseButton: bool = None  # False # whether to show the close button
-    closeButtonClassName: str = None  # CSS class name of the close button
-    showIcon: bool = None  # False # whether to show icon
-    icon: str = None  # custom icon
-    iconClassName: str = None  # CSS class name of icon
-
-
-class Dialog(AmisNode):
-    """Dialog"""
-
-    type: str = "dialog"  # Specify as Dialog renderer
-    title: SchemaNode = None  # Popup layer title
-    body: SchemaNode = None  # Add content to the Dialog content area
-    size: Union[str, SizeEnum] = None  # Specify the dialog size, support: xs, sm, md, lg, xl, full
-    bodyClassName: str = None  # "modal-body" # The style class name of the Dialog body area
-    closeOnEsc: bool = None  # False # whether to support pressing Esc to close Dialog
-    showCloseButton: bool = None  # True # whether to show the close button in the upper right corner
-    showErrorMsg: bool = None  # True # whether to display the error message in the lower left corner of the popup
-    disabled: bool = None  # False # If this property is set, the Dialog is read-only and has no submit operation.
-    actions: List[Action] = None  # If you want to not display the bottom button, you can configure: [] "[Confirm]
-    # and [Cancel]"
-    data: dict = None  # Support data mapping, if not set, it will inherit the data in the context of the trigger
-    # button by default.
-    showLoading: bool = None  # True # 是否在弹框左下角显示 loading 动画
-
-
-class Drawer(AmisNode):
-    """drawer"""
-
-    type: str = "drawer"  # "drawer" specifies the Drawer renderer
-    title: SchemaNode = None  # Popup layer title
-    body: SchemaNode = None  # Add content to the Drawer content area
-    size: Union[str, SizeEnum] = None  # Specify Drawer size, support: xs, sm, md, lg
-    position: str = None  # 'left' # position
-    bodyClassName: str = None  # "modal-body" # The style class name of the Drawer body area
-    closeOnEsc: bool = None  # False # whether to support pressing Esc to close Drawer
-    closeOnOutside: bool = None  # False # whether to close the Drawer when clicking outside the content area
-    overlay: bool = None  # True # whether to display the overlay
-    resizable: bool = None  # False # whether the size of the Drawer can be changed by dragging and dropping
-    actions: List[Action] = None  # Can not be set, there are only two buttons by default. "[Confirm] and [Cancel]"
-    data: dict = None  # Support data mapping, if not set, it will inherit the data in the context of the trigger
-    # button by default.
-    className: str = None  # Drawer 最外层容器的样式类名
-    headerClassName: str = None  # Drawer 头部 区域的样式类名
-    footerClassName: str = None  # Drawer 页脚 区域的样式类名
-    showCloseButton: bool = True  # 是否展示关闭按钮，当值为 false 时，默认开启 closeOnOutside
-    width: Union[int, str] = "500px"  # 容器的宽度，在 position 为 left 或 right 时生效
-    height: Union[int, str] = "500px"  # 容器的高度，在 position 为 top 或 bottom 时生效
-
-
-class Iframe(AmisNode):
-    """Iframe"""
-
-    type: str = "iframe"  # Specify as iFrame renderer
-    className: str = None  # iFrame class name
-    frameBorder: list = None  # frameBorder
-    style: dict = None  # style object
-    src: str = None  # iframe address
-    allow: str = None  # allow configuration
-    sandbox: str = None  # sandbox configuration
-    referrerpolicy: str = None  # referrerpolicy configuration
-    height: Union[int, str] = None  # "100%" # iframe height
-    width: Union[int, str] = None  # "100%" # iframe width
-
-
-class Spinner(AmisNode):
-    """Loading"""
-
-    type: str = "spinner"
-
-
-class TableCRUD(CRUD, Table):
-    """Form Table CRUD"""
-
-    mode: str = "table"
-
-
-class CardCRUD(CRUD, Cards):
-    """Form Card CRUD"""
-
-    mode: str = "cards"
-
-
-class ListCRUD(CRUD, ListDisplay):
-    """Form Card CRUD"""
-
-    mode: str = "list"
-
-
-class Avatar(AmisNode):
-    """avatar"""
-
-    type: str = "avatar"
-    className: str = None  # The class name of the outer dom
-    fit: str = None  # "cover" # Image zoom type
-    src: str = None  # Image address
-    text: str = None  # text
-    icon: str = None  # icon
-    shape: str = None  # "circle" # shape, can also be square
-    size: int = None  # 40 # size
-    style: dict = None  # The style of the outer dom
-
-
-class Audio(AmisNode):
-    """Audio"""
-
-    type: str = "audio"  # specify the audio renderer
-    className: str = None  # The class name of the outer Dom
-    inline: bool = None  # True # whether it is inline mode
-    src: str = None  # audio address
-    loop: bool = None  # False # whether to loop playback
-    autoPlay: bool = None  # False # whether to play automatically
-    rates: List[float] = None  # "[]" # Configurable audio playback speed such as: [1.0, 1.5, 2.0]
-    controls: List[str] = None  # "['rates','play','time','process','volume']" # Internal module customization
-
-
-class Status(AmisNode):
-    """state"""
-
-    type: str = "status"  # Specify as Status renderer
-    className: str = None  # The class name of the outer Dom
-    placeholder: str = None  # placeholder text
-    map: dict = None  # map icon
-    labelMap: dict = None  # map text
-
-
-class Tasks(AmisNode):
-    """Task operation collection"""
-
-    class Item(AmisNode):
-        label: str = None  # task name
-        key: str = None  # Task key value, please distinguish it uniquely
-        remark: str = None  # Current task status, support html
-        status: str = None  # Task status: 0: Initial status, inoperable. 1: Ready, operational state. 2: In
-        # progress, not over yet.
-        # 3: There is an error, no retry. 4: Completed normally. 5: There is an error, and you can try again.
-
-    type: str = "tasks"  # Specify as Tasks renderer
-    className: str = None  # The class name of the outer Dom
-    tableClassName: str = None  # class name of table Dom
-    items: List[Item] = None  # task list
-    checkApi: API = None  # Return the task list, please refer to items for the returned data.
-    submitApi: API = None  # API used for submitting tasks
-    reSubmitApi: API = None  # If the task fails and can be retried, this API will be used when submitting
-    interval: int = None  # 3000 # When there is a task in progress, it will be checked again at regular intervals,
-    # and the time interval is configured through this, the default is 3s.
-    taskNameLabel: str = None  # "task name" # task name column description
-    operationLabel: str = None  # "Operation" # Operation column description
-    statusLabel: str = None  # "status" # description of status column
-    remarkLabel: RemarkT = None  # "Remark" # Remark column description
-    btnText: str = None  # "Online" # Action button text
-    retryBtnText: str = None  # "Retry" # Retry action button text
-    btnClassName: str = None  # "btn-sm btn-default" # Configure the container button className
-    retryBtnClassName: str = None  # "btn-sm btn-danger" # Configure container retry button className
-    statusLabelMap: List[str] = None  # Status display corresponding class name configuration
-    # "["label-warning", "label-info", "label-success", "label-danger", "label-default", "label-danger"]"
-    statusTextMap: List[str] = None  # "["Not started", "Ready", "In progress", "Error", "Completed", "Error"]" #
-    # Status display corresponding text display configuration
-
-
-class Wizard(AmisNode):
-    """Wizard"""
-
-    class Step(AmisNode):
-        title: str = None  # Step title
-        mode: str = None  # Display the default, the same as the mode in Form, choose: normal, horizontal or inline.
-        horizontal: Horizontal = None  # When in horizontal mode, it is used to control the ratio of left and right
-        api: API = None  # The current step saves the interface, which can be left unconfigured.
-        initApi: API = None  # The current step data initialization interface.
-        initFetch: bool = None  # whether the current step data initialization interface is initially fetched.
-        initFetchOn: Expression = None  # whether the current step data initialization interface is initially fetched
-        # is determined by an expression.
-        body: List[FormItem] = None  # The form item collection of the current step, please refer to FormItem.
-
-    type: str = "wizard"  # Specify as Wizard component
-    mode: str = None  # "horizontal" # Display mode, choose: horizontal or vertical
-    api: API = None  # The interface saved in the last step.
-    initApi: API = None  # Initialize data interface
-    initFetch: API = None  # whether to fetch data initially.
-    initFetchOn: Expression = None  # whether to pull data initially, configure by expression
-    actionPrevLabel: str = None  # "Previous" # Previous button text
-    actionNextLabel: str = None  # "Next" # Next button text
-    actionNextSaveLabel: str = None  # "Save and Next" # Save and Next button text
-    actionFinishLabel: str = None  # "Finish" # Finish button text
-    className: str = None  # Outer CSS class name
-    actionClassName: str = None  # "btn-sm btn-default" # Button CSS class name
-    reload: str = None  # Refresh the target object after the operation. Please fill in the name value set by the
-    # target component. If it is filled in window, the current page will be refreshed as a whole.
-    redirect: Template = None  # "3000" # Jump after the operation.
-    target: str = None  # "False" # You can submit data to other components instead of saving it yourself. Please
-    # fill in the name value set by the target component,
-    # If it is filled in as window, the data will be synchronized to the address bar, and the components that depend
-    # on these data will be automatically refreshed.
-    steps: List[Step] = None  # Array, configure step information
-    startStep: int = None  # "1" # Start default value, starting from the first step. Templates can be supported,
-    # but only when the component is created, the template is rendered and the current number of steps is set. When
-    # the component is refreshed later,
-    # The current step will not change according to startStep
-
-
-class AmisRender(AmisNode):
-    """Amis render"""
-
-    type: str = "amis"  # Specify as amis renderer
-    schema_: SchemaNode = Field(None, alias="schema")  # amis schema
-    props: dict = None  # amis props
-
-
-PageSchema.update_forward_refs()
-ActionType.Dialog.update_forward_refs()
-ActionType.Drawer.update_forward_refs()
-TableCRUD.update_forward_refs()
-Form.update_forward_refs()
-Tpl.update_forward_refs()
-InputText.update_forward_refs()
-InputNumber.update_forward_refs()
-Picker.update_forward_refs()
+"""Detailed document reading address: https://baidu.gitee.io/amis/zh-CN/components"""
+import os
+from typing import Any, Dict, List, Optional, Tuple, Union
+
+from pydantic import Field
+from typing_extensions import Literal
+
+from .constants import (
+    BarcodeEnum,
+    DisplayModeEnum,
+    LevelEnum,
+    PlacementEnum,
+    ProgressEnum,
+    SizeEnum,
+    StepStatusEnum,
+    TabsModeEnum,
+    TriggerEnum,
+)
+from .types import (
+    API,
+    AmisNode,
+    BaseAmisModel,
+    Expression,
+    OptionsNode,
+    SchemaNode,
+    Template,
+    Tpl,
+)
+from .utils import amis_templates
+
+BASE_DIR = os.path.dirname(os.path.abspath(__file__))
+
+RemarkT = Union[str, "Remark"]
+
+
+class Html(AmisNode):
+    """Html"""
+
+    type: str = "html"  # specify as html component
+    html: str  # html When you need to get variables in the data field, use Tpl.
+
+
+class Icon(AmisNode):
+    """icon"""
+
+    type: str = "icon"  # specify the component type
+    className: str = None  # Outer CSS class name
+    icon: str = None  # icon name, support fontawesome v4 or use url
+    vendor: str = None  # icon vendor, icon supports fontawesome v4 by default, if you want to support fontawesome v5
+    # and v6, please set vendor to an empty string.
+
+
+class Remark(AmisNode):
+    """mark"""
+
+    type: str = "remark"  # remark
+    className: str = None  # Outer CSS class name
+    content: str = None  # prompt text
+    placement: str = None  # Popup position
+    trigger: str = None  # Trigger condition['hover','focus']
+    icon: str = None  # "fa fa-question-circle" # icon
+
+
+class Badge(AmisNode):
+    """Subscript"""
+
+    mode: str = "dot"  # Corner type, can be dot/text/ribbon
+    text: Union[int, str] = None  # Corner text, supports strings and numbers, invalid when mode='dot'
+    size: int = None  # Angular size
+    level: str = None  # The level of the corner label, which can be info/success/warning/danger, after setting the
+    # background color of the corner label is different
+    overflowCount: int = None  # 99 # Set the capped number value
+    position: str = None  # "top-right" # Corner position, can be top-right/top-left/bottom-right/bottom-left
+    offset: int = None  # The position of the corner label, the priority is greater than the position, when the
+    # offset is set, the position is positioned as the top-right reference number[top, left]
+    className: str = None  # The class name of the outer dom
+    animation: bool = None  # whether the corner icon displays animation
+    style: dict = None  # Custom style for corner labels
+    visibleOn: Expression = None  # Controls the display and hiding of corner labels
+
+
+class Page(AmisNode):
+    """page"""
+
+    __default_template_path__: str = f"{BASE_DIR}/templates/page.html"
+
+    type: str = "page"  # Specify as Page component
+    title: SchemaNode = None  # page title
+    subTitle: SchemaNode = None  # Page subtitle
+    remark: RemarkT = None  # A prompt icon will appear near the title, and the content will be prompted when the
+    # mouse is placed on it.
+    aside: SchemaNode = None  # Add content to the sidebar area of the page
+    asideResizor: bool = None  # whether the width of the sidebar area of the page can be adjusted
+    asideMinWidth: int = None  # The minimum width of the sidebar area of the page
+    asideMaxWidth: int = None  # The maximum width of the sidebar area of the page
+    toolbar: SchemaNode = None  # Add content to the upper right corner of the page. It should be noted that when
+    # there is a title, the area is in the upper right corner, and when there is no title, the area is at the top
+    body: SchemaNode = None  # Add content to the content area of the page
+    className: str = None  # Outer dom class name
+    cssVars: dict = None  # Custom CSS variables, please refer to styles
+    css: str = None  # Custom CSS styles, please refer to used theme styles
+    mobileCSS: str = None  # Custom mobile CSS styles, please refer to used theme styles
+    toolbarClassName: str = None  # "v-middle wrapper text-right bg-light bb" # Toolbar dom class name
+    bodyClassName: str = None  # "wrapper" # Body dom class name
+    asideClassName: str = None  # "w page-aside-region bg-auto" # Aside dom class name
+    headerClassName: str = None  # "bg-light bb wrapper" # Header area dom class name
+    initApi: API = None  # The api that Page uses to get initial data. The returned data can be used at the entire
+    # page level.
+    initFetch: bool = None  # True # whether to start pulling initApi
+    initFetchOn: Expression = None  # whether to start pulling initApi, configure by expression
+    interval: int = None  # refresh time (minimum 1000)
+    silentPolling: bool = None  # False # whether to show the loading animation when the configuration is refreshed
+    stopAutoRefreshWhen: Expression = None  # Configure the conditions for stopping refresh through expressions
+    regions: List[str] = None
+
+    def amis_html(
+        self,
+        template_path: str = "",
+        locale: str = "zh_CN",
+        cdn: str = "https://unpkg.com",
+        pkg: str = "amis@1.10.2",
+        site_title: str = "Amis",
+        site_icon: str = "",
+        theme: str = "cxd",
+    ):
+        """Render html template"""
+        template_path = template_path or self.__default_template_path__
+        theme_css = f'<link href="{cdn}/{pkg}/sdk/{theme}.css" rel="stylesheet"/>' if theme != "cxd" else ""
+        return amis_templates(template_path).safe_substitute(
+            {
+                "AmisSchemaJson": self.amis_json(),
+                "locale": locale.replace("_", "-"),  # Fix #50
+                "cdn": cdn,
+                "pkg": pkg,
+                "site_title": site_title,
+                "site_icon": site_icon,
+                "theme": theme,
+                "theme_css": theme_css,
+            }
+        )
+
+
+class Divider(AmisNode):
+    """Dividing line"""
+
+    type: str = "divider"  # "Divider"
+    className: str = None  # The class name of the outer Dom
+    lineStyle: str = None  # Split line style, supports dashed and solid
+
+
+class Flex(AmisNode):
+    """layout"""
+
+    type: str = "flex"  # Specify as Flex renderer
+    className: str = None  # css class name
+    justify: str = None  # "start", "flex-start", "center", "end", "flex-end", "space-around", "space-between",
+    # "space-evenly"
+    alignItems: str = None  # "stretch", "start", "flex-start", "flex-end", "end", "center", "baseline"
+    style: dict = None  # custom style
+    items: List[SchemaNode] = None  #
+
+
+class Grid(AmisNode):
+    """Horizontal layout"""
+
+    class Column(AmisNode):
+        """Column configuration"""
+
+        xs: int = None  # "auto" # Width ratio: 1 - 12
+        ClassName: str = None  # column class name
+        sm: int = None  # "auto" # Width ratio: 1 - 12
+        md: int = None  # "auto" # Width ratio: 1 - 12
+        lg: int = None  # "auto" # Width ratio: 1 - 12
+        valign: str = None  # 'top'|'middle'|'bottom'|'between = None # Vertical alignment of the current column content
+        body: List[SchemaNode] = None  #
+
+    type: str = "grid"  # Specify as Grid renderer
+    className: str = None  # The class name of the outer Dom
+    gap: str = None  # 'xs'|'sm'|'base'|'none'|'md'|'lg = None # Horizontal gap
+    valign: str = None  # 'top'|'middle'|'bottom'|'between = None # Vertical alignment
+    align: str = None  # 'left'|'right'|'between'|'center = None # Horizontal alignment
+    columns: List[SchemaNode] = None  #
+
+
+class Panel(AmisNode):
+    """panel"""
+
+    type: str = "panel"  # Specify as the Panel renderer
+    className: str = None  # "panel-default" # The class name of the outer Dom
+    headerClassName: str = None  # "panel-heading" # The class name of the header area
+    footerClassName: str = None  # "panel-footer bg-light lter wrapper" # The class name of the footer area
+    actionsClassName: str = None  # "panel-footer" # The class name of the actions area
+    bodyClassName: str = None  # "panel-body" # The class name of the body area
+    title: SchemaNode = None  # title
+    header: SchemaNode = None  # header container
+    body: SchemaNode = None  # Content container
+    footer: SchemaNode = None  # bottom container
+    affixFooter: bool = None  # whether to fix the bottom container
+    actions: List["Action"] = None  # Button area
+
+
+class Tabs(AmisNode):
+    """Tab"""
+
+    class Item(AmisNode):
+        title: str = None  # Tab title
+        icon: Union[str, Icon] = None  # Icon for Tab
+        tab: SchemaNode = None  # Content area
+        hash: str = None  # After setting, it will correspond to the hash of the url
+        reload: bool = None  # After setting, the content will be re-rendered every time, which is useful for
+        # re-pulling crud
+        unmountOnExit: bool = None  # Each exit will destroy the current tab bar content
+        className: str = None  # "bg-white bl br bb wrapper-md" # Tab area style
+        iconPosition: str = None  # "left" # Tab's icon position left / right
+        closable: bool = None  # False # whether to support deletion, the priority is higher than the closable of the
+        # component
+        disabled: bool = None  # False # whether to disable
+
+    type: str = "tabs"  # Specify as Tabs renderer
+    className: str = None  # The class name of the outer Dom
+    mode: str = None  # Display mode, the value can be line, card, radio, vertical, chrome, simple, strong, tiled,
+    # sidebar
+    tabsClassName: str = None  # Class name of Tabs Dom
+    tabs: List[Item] = None  # tabs content
+    source: str = None  # tabs associated data, tabs can be generated repeatedly after association
+    toolbar: SchemaNode = None  # toolbar in tabs
+    toolbarClassName: str = None  # The class name of the toolbar in the tabs
+    mountOnEnter: bool = None  # False # Render only when the tab is clicked
+    unmountOnExit: bool = None  # False # Destroyed when switching tabs
+    scrollable: bool = None  # False # whether the navigation supports content overflow scrolling, this property is
+    # not supported in vertical and chrome modes; chrome mode defaults to compress tags (property discarded)
+    tabsMode: TabsModeEnum = None  # Display mode, the value can be line, card, radio, vertical, chrome, simple,
+    # strong, tiled, sidebar
+    addable: bool = None  # False # whether to support adding
+    addBtnText: str = None  # "Add" # Add button text
+    closable: bool = None  # False # whether to support delete
+    draggable: bool = None  # False # whether to support draggable
+    showTip: bool = None  # False # whether to support tips
+    showTipClassName: str = None  # "'' " # Tip class
+    editable: bool = None  # False # whether to edit the tag name
+    sidePosition: str = None  # "left" # In sidebar mode, the position of the tab bar is left / right
+
+
+class Portlet(Tabs):
+    """Portal column"""
+
+    class Item(Tabs.Item):
+        toolbar: SchemaNode = None  # The toolbar in tabs, which changes with tab switching
+
+    type: str = "portlet"  # specify as portlet renderer
+    contentClassName: str = None  # Class name of Tabs content Dom
+    tabs: List[Item] = None  # tabs content
+    style: Union[str, dict] = None  # custom style
+    description: Template = None  # Information on the right side of the title
+    hideHeader: bool = None  # False # hide the header
+    divider: bool = None  # False # remove divider
+
+
+class Horizontal(AmisNode):
+    left: int = None  # The width ratio of the left label
+    right: int = None  # The width ratio of the right controller.
+    offset: int = None  # When the label is not set, the offset of the right controller
+
+
+class Action(AmisNode):
+    """Behavior button"""
+
+    type: str = "button"  # Specify as the Page renderer. button action
+    actionType: str = None  # [Required] This is the core configuration of the action to specify the action type of
+    # the action. Support: ajax, link, url, drawer, dialog, confirm, cancel, prev, next, copy, close.
+    label: str = None  # Button text. Available ${xxx} values.
+    level: LevelEnum = None  # Button style, support: link, primary, secondary, info, success, warning, danger,
+    # light, dark, default.
+    size: str = None  # Button size, support: xs, sm, md, lg.
+    icon: str = None  # Set the icon, eg fa fa-plus.
+    iconClassName: str = None  # Add a class name to the icon.
+    rightIcon: str = None  # Set the icon to the right of the button text, eg fa fa-plus.
+    rightIconClassName: str = None  # Add a class name to the right icon.
+    active: bool = None  # whether the button is highlighted.
+    activeLevel: str = None  # The style when the button is highlighted, the configuration supports the same level.
+    activeClassName: str = None  # Add a class name to the button highlight. "is-active"
+    block: bool = None  # Use display:"block" to display the button.
+    confirmText: Template = None  # When set, the action will ask the user before starting. Available ${xxx} values.
+    reload: str = None  # Specify the name of the target component that needs to be refreshed after this operation (
+    # the name value of the component, configured by yourself), please separate multiple ones with , signs.
+    tooltip: str = None  # This text pops up when the mouse stays, and the object type can also be configured: the
+    # fields are title and content. Available ${xxx} values.
+    disabledTip: str = None  # The text will pop up when the mouse stays after it is disabled. You can also configure
+    # the object type: the fields are title and content. Available ${xxx} values.
+    tooltipPlacement: str = None  # If tooltip or disabledTip is configured, specify the location of the prompt
+    # information, and you can configure top, bottom, left, and right.
+    close: Union[bool, str] = None  # When the action is configured in the actions of the dialog or drawer, configure
+    # it to true to close the current dialog or drawer after the operation. When the value is a string and is the
+    # name of the ancestor layer popup, the ancestor popup will be closed.
+    required: List[str] = None  # Configure an array of strings, specifying that the form items with the specified
+    # field name must pass validation before performing operations in the form primary:bool=None
+    onClick: str = None  # The custom click event defines the click event through onClick in the form of a string,
+    # which will be converted into a JavaScript function
+    componentId: str = None  # target component ID
+    args: Union[dict, str] = None  # event parameters
+    script: str = None  # Customize JS script code, any action can be performed by calling doAction in the code,
+    # and event action intervention can be realized through the event object event
+
+
+class ActionType:
+    """Behavior button type"""
+
+    class Ajax(Action):
+        actionType: str = "ajax"  # Show a popup after clicking
+        api: API = None  # Request address, refer to api format description.
+        redirect: Template = None  # Specify the path to redirect to after the current request ends, which can be
+        # valued by ${xxx}.
+        feedback: "Dialog" = None  # If it is of ajax type, when ajax returns to normal, a dialog can be popped up
+        # for other interactions. The returned data can be used in this dialog. For the format, please refer to Dialog
+        messages: dict = None  # success: a message will be displayed after the ajax operation is successful. It can
+        # be left unspecified. If it is not specified, the api return shall prevail. failed: Ajax operation failure
+        # message.
+
+    class Dialog(Action):
+        actionType: str = "dialog"  # Show a popup when clicked
+        dialog: Union["Dialog", "Service", SchemaNode]  # Specify the content of the pop-up box, the format can refer to Dialog
+        nextCondition: bool = None  # Can be used to set the condition of the next data, the default is true.
+
+    class Drawer(Action):
+        actionType: str = "drawer"  # Show a sidebar when clicked
+        drawer: Union["Drawer", "Service", SchemaNode]  # Specify the content of the popup box, the format can refer to Drawer
+
+    class Copy(Action):
+        actionType: str = "copy"  # Copy a piece of content to the clipboard
+        content: Template  # Specify the copied content. Available ${xxx} values.
+        copyFormat: str = None  # You can set the copy format through copyFormat, the default is text text/html
+
+    class Url(Action):
+        """Jump directly"""
+
+        actionType: str = "url"  # Jump directly
+        url: str  # When the button is clicked, the specified page will be opened. Available ${xxx} values.
+        blank: bool = None  # false If true will open in a new tab page.
+
+    class Link(Action):
+        """Single page jump"""
+
+        actionType: str = "link"  # Single page jump
+        link: str  # is used to specify the jump address. Unlike url, this is a single-page jump method, which will
+        # not render the browser. Please specify the page in the amis platform. Available ${xxx} values.
+
+    class Toast(Action):
+        """Toast light"""
+
+        class ToastItem(AmisNode):
+            title: Union[str, SchemaNode] = None  # Toast Item Title
+            body: Union[str, SchemaNode] = None  # Toast Item Content
+            level: str = None  # default 'info', Display icon, optional 'info', 'success', 'error', 'warning'
+            position: str = None  # default 'top-center', display position,
+            # 'top-right', 'top-center', 'top-left', 'bottom-center', 'bottom-left', 'bottom-right', 'center'
+            closeButton: bool = None  # default False, whether to show the close button
+            showIcon: bool = None  # default True, whether to display the icon
+            timeout: int = None  # default 5000
+
+        actionType: str = "toast"  # Single page jump
+        items: List[ToastItem] = None  # List of ToastItems
+        position: str = None  # display position,
+        # available 'top-right', 'top-center', 'top-left', 'bottom-center', 'bottom-left', 'bottom-right', 'center'
+        closeButton: bool = None  # default False, whether to display the close button, not in mobile
+        showIcon: bool = None  # default = True, whether to display the icon
+        timeout: int = None  # default 5000
+
+
+class PageSchema(AmisNode):
+    """Page configuration"""
+
+    label: str = None  # Menu name.
+    icon: str = "fa fa-flash"  # Menu icon, for example: 'fa fa-file'. For detailed icon reference:
+    # http://www.fontawesome.com.cn/faicons/
+    url: str = None  # The page routing path, when the route hits the path, the current page is enabled. When the
+    # path does not start with /, the parent path is concatenated. For example: the path of the parent is folder,
+    # and pageA is configured at this time, then this page will be hit only when the page address is /folder/pageA.
+    # When the path starts with / such as: /crud/list, the parent path will not be spliced. In addition, routes with
+    # parameters such as /crud/view/:id are supported. This value can be obtained from the page through ${params.id}.
+    schema_: Union[Page, "Iframe"] = Field(None, alias="schema")  # The configuration of the page, please go to the
+    # page page for specific configuration
+    schemaApi: API = None  # If you want to pull through the interface, please configure. The return path is
+    # json>data. Only one of schema and schemaApi can be selected.
+    link: str = None  # If you want to configure an external link menu, you only need to configure link.
+    redirect: str = None  # Jump, when hitting the current page, jump to the target page.
+    rewrite: str = None  # Change to rendering pages of other paths, the page address will not be modified in this way.
+    isDefaultPage: Union[bool, str] = None  # Useful when you need a custom 404 page, don't have multiple such pages,
+    # because only the first one will be useful.
+    visible: Union[bool, str] = None  # Some pages may not want to appear in the menu, you can configure it to false, and the
+    # route with parameters does not need to be configured, it is directly invisible.
+    className: str = None  # Menu class name.
+    children: List["PageSchema"] = None  # Submenu
+    sort: int = None  # Unofficial attribute. sort
+    tabsMode: TabsModeEnum = None  # Unofficial attribute. Display mode, the value can be line, card, radio, vertical,
+
+    # chrome, simple, strong, tiled, sidebar, collapse
+
+    def as_page_body(self, group_extra: Dict[str, Any] = None, item_extra: Dict[str, Any] = None):
+        if self.children:
+            exclude = {"type", "url", "schema_", "schemaApi", "link", "redirect", "rewrite", "isDefaultPage", "children"}
+            if self.tabsMode is None:
+                body = App(pages=[PageSchema(children=self.children)])
+            elif self.tabsMode == TabsModeEnum.collapse:
+                body = (
+                    CollapseGroup.parse_obj(self.dict(exclude=exclude, exclude_defaults=True))
+                    .update_from_kwargs(
+                        body=[
+                            CollapseGroup.CollapseItem.parse_obj(item.dict(exclude=exclude, exclude_defaults=True))
+                            .update_from_kwargs(
+                                header=item.label,
+                                body=item.as_page_body(group_extra, item_extra),
+                            )
+                            .update_from_dict(item_extra or {})
+                            for item in self.children
+                        ],
+                    )
+                    .update_from_dict(group_extra or {})
+                )
+            else:
+                body = (
+                    Tabs.parse_obj(self.dict(exclude=exclude, exclude_defaults=True))
+                    .update_from_kwargs(
+                        mountOnEnter=True,
+                        tabs=[
+                            Tabs.Item.parse_obj(item.dict(exclude=exclude, exclude_defaults=True))
+                            .update_from_kwargs(
+                                title=item.label,
+                                tab=item.as_page_body(group_extra, item_extra),
+                            )
+                            .update_from_dict(item_extra or {})
+                            for item in self.children
+                        ],
+                    )
+                    .update_from_dict(group_extra or {})
+                )
+        elif self.schema_:
+            body = self.schema_
+            if isinstance(body, Iframe):
+                body.height = body.height or 1080
+        elif self.schemaApi:
+            body = Service(schemaApi=self.schemaApi)
+        elif self.link:
+            body = Page(body=Link(href=self.link, body=self.label, blank=True))
+        else:
+            body = None
+        return body
+
+
+class App(Page):
+    """Multi-page application"""
+
+    __default_template_path__: str = f"{BASE_DIR}/templates/app.html"
+    type: str = "app"
+    api: API = None  # The page configuration interface, if you want to pull the page configuration remotely,
+    # please configure it. Return to the configuration path json>data>pages, please refer to the pages property for
+    # the specific format.
+    brandName: str = None  # app name
+    logo: str = None  # Support image address, or svg.
+    className: str = None  # css class name
+    header: str = None  # header
+    asideBefore: str = None  # The front area on the page menu.
+    asideAfter: str = None  # The front area under the page menu.
+    footer: str = None  # The page.
+    pages: List[PageSchema] = None  # Array<page configuration> specific page configuration.
+    # Usually in an array, the first layer of the array is a group, generally you only need to configure the label set,
+    # if you don't want to group, don't configure it directly, the real page should be configured in the second
+    # layer, that is, in the children of the first layer.
+
+
+class ButtonGroup(AmisNode):
+    """Button group"""
+
+    type: str = "button-group"
+    buttons: List[Action]  # Behavior button group
+    className: str = None  # The class name of the outer Dom
+    vertical: bool = None  # whether to use vertical mode
+    tiled: bool = None  # whether to use tile mode
+    btnLevel: LevelEnum = None  # button style
+    btnActiveLevel: LevelEnum = None  # Active button style
+
+
+class Custom(AmisNode):
+    """Custom Components"""
+
+    type: str = "custom"
+    id: str = None  # node id
+    name: str = None  # node name
+    className: str = None  # node class
+    inline: bool = False  # use div tag by default, if true use span tag
+    html: str = None  # initialize node html
+    onMount: str = None  # "Function" # Function called after node initialization
+    onUpdate: str = None  # "Function" # The function called when the data is updated
+    onUnmount: str = None  # "Function" # The function called when the node is destroyed
+
+
+class Service(AmisNode):
+    """Functional container"""
+
+    type: str = "service"  # designate as service renderer
+    name: str = None  # node name
+    data: dict = None  #
+    className: str = None  # The class name of the outer Dom
+    body: SchemaNode = None  # Content container
+    api: API = None  # Initialize data domain interface address
+    ws: str = None  # WebScocket address
+    dataProvider: str = None  # Data acquisition function
+    initFetch: bool = None  # whether to pull by default
+    schemaApi: API = None  # Used to get the remote schema interface address
+    initFetchSchema: bool = None  # whether to pull Schema by default
+    messages: dict = None  # Message prompt override, the default message reads the toast prompt text returned by the
+    # interface, but it can be overridden here.
+    # messages.fetchSuccess: str = None # Toast prompt text when the interface request is successful
+    # messages.fetchFailed: str = "Initialization failed" # Toast prompt text when interface request fails
+    interval: int = None  # Polling interval (minimum 3000)
+    silentPolling: bool = None  # False # whether to display the loading animation during polling
+    stopAutoRefreshWhen: Expression = None  # Configure the condition to stop polling
+
+
+class Nav(AmisNode):
+    """navigation"""
+
+    class Link(AmisNode):
+        label: str = None  # name
+        to: Template = None  # Link address
+        target: str = None  # "Link relationship" #
+        icon: str = None  # icon
+        children: List["Link"] = None  # child links
+        unfolded: bool = None  # whether to unfold initially
+        active: bool = None  # whether to highlight
+        activeOn: Expression = None  # whether to highlight the condition, leaving it blank will automatically
+        # analyze the link address
+        defer: bool = None  # mark whether it is a lazy add-in
+        deferApi: API = None  # Can not be configured, if the configuration priority is higher
+
+    type: str = "nav"  # specify as Nav renderer
+    className: str = None  # The class name of the outer Dom
+    stacked: bool = True  # Set to false to display in the form of tabs
+    source: API = None  # Navigation can be created dynamically via variable or API interface
+    deferApi: API = None  # The interface used to delay loading option details. It can be left unconfigured,
+    # and the public source interface cannot be configured.
+    itemActions: SchemaNode = None  # More operations related configuration
+    draggable: bool = None  # whether to support drag and drop sorting
+    dragOnSameLevel: bool = None  # Only allow dragging within the same level
+    saveOrderApi: API = None  # save order api
+    itemBadge: Badge = None  # Badge
+    links: list = None  # link collection
+
+
+class AnchorNav(AmisNode):
+    """Anchor Navigation"""
+
+    class Link(AmisNode):
+        label: str = None  # name
+        title: str = None  # area title
+        href: str = None  # Region ID
+        body: SchemaNode = None  # area content area
+        className: str = None  # "bg-white bl br bb wrapper-md" # Area member style
+
+    type: str = "anchor-nav"  # Specify as AnchorNav renderer
+    className: str = None  # The class name of the outer Dom
+    linkClassName: str = None  # Class name of the navigation Dom
+    sectionClassName: str = None  # The class name of the anchor area Dom
+    links: list = None  # links content
+    direction: str = None  # "vertical" # You can configure whether the navigation is displayed horizontally or
+    # vertically. The corresponding configuration items are: vertical, horizontal
+    active: str = None  # The area that needs to be located
+
+
+class ButtonToolbar(AmisNode):
+    """Button Toolbar"""
+
+    type: str = "button-toolbar"
+    buttons: List[Action]  # Behavior button group
+
+
+class Validation(BaseAmisModel):
+    isEmail: bool = None  # Must be Email.
+    isUrl: bool = None  # Must be a Url.
+    isNumeric: bool = None  # Must be a number.
+    isAlpha: bool = None  # Must be an alpha.
+    isAlphanumeric: bool = None  # Must be a letter or a number.
+    isInt: bool = None  # Must be an integer.
+    isFloat: bool = None  # Must be a float.
+    isLength: int = None  # whether the length is exactly equal to the set value.
+    minLength: int = None  # Minimum length.
+    maxLength: int = None  # Maximum length.
+    maximum: int = None  # Maximum value.
+    minimum: int = None  # Minimum value.
+    equals: str = None  # The current value must be exactly equal to xxx.
+    equalsField: str = None  # The current value must be the same as the xxx variable value.
+    isJson: bool = None  # Is it a valid Json string.
+    isUrlPath: bool = None  # is the url path.
+    isPhoneNumber: bool = None  # Is it a legal phone number
+    isTelNumber: bool = None  # Is it a valid phone number
+    isZipcode: bool = None  # whether it is a zip code
+    isId: bool = None  # whether it is an ID number, no verification is done
+    matchRegexp: str = None  # Must hit a certain regexp. /foo/
+
+
+class FormItem(AmisNode):
+    """Form item common"""
+
+    class AutoFill(BaseAmisModel):
+        showSuggestion: bool = None  # true refers to input, false automatically fills
+        api: API = None  # Automatically populate the interface/filter the CRUD request configuration with reference to entry
+        silent: bool = None  # Whether to display a data format error message. The default value is true
+        fillMappinng: SchemaNode = None  # Auto-fill/reference input data mapping configuration, key-value pair form,
+        # value support variable acquisition and expression
+        trigger: str = None  # ShowSuggestion to true, the reference input support way of trigger,
+        # currently supports change "value change" | focus "form focus"
+        mode: str = None  # When showSuggestion is true, refer to the popOver mode: dialog, drawer, popOver
+        labelField: str = None  # When showSuggestion is true, set the popup dialog,drawer,popOver picker's labelField
+        position: str = None  # If showSuggestion is true, set the popOver location as shown in the input mode Popover
+        size: str = None  # If showSuggestion is true, set the value as shown in dialog mode
+        columns: List["TableColumn"] = None  # When showSuggestion is true, the data display column configuration
+        filter: SchemaNode = None  # When showSuggestion is true, data query filter condition
+
+    type: str = "input-text"  # Specify the form item type
+    className: str = None  # The outermost class name of the form
+    inputClassName: str = None  # Form controller class name
+    labelClassName: str = None  # class name of label
+    name: str = None  # Field name, specifying the key when the form item is submitted
+    label: Union[bool, Template] = None  # form item label template or false
+    labelAlign: str = None  # "right" # Form item label alignment, default right alignment, only effective when mode is
+    labelRemark: RemarkT = None  # Form item label description
+    description: Template = None  # Form item description
+    placeholder: str = None  # Form item description
+    inline: bool = None  # whether it is inline mode
+    submitOnChange: bool = None  # whether to submit the current form when the value of the form item changes.
+    disabled: bool = None  # whether the current form item is disabled
+    disabledOn: Expression = None  # The condition for whether the current form item is disabled
+    visible: Expression = None  # whether the current form item is disabled or not
+    visibleOn: Expression = None  # The condition for whether the current form item is disabled
+    required: bool = None  # whether it is required.
+    requiredOn: Expression = None  # Use an expression to configure whether the current form item is required.
+    validations: Union[Validation, Expression] = None  # Validation of the form item value format, multiple settings
+    # are supported, and multiple rules are separated by commas.
+    validateApi: API = None  # Form validation interface
+    copyable: Union[bool, dict] = None  # whether to copy boolean or {icon: string, content:string}
+    autoFill: AutoFill = None  # Data entry configuration, automatic filling or reference entry
+    static: bool = None  # 2.4.0 Whether the current form item is static display,
+    # the current support static display of the form item
+    staticClassName: str = None  # 2.4.0 The class name for static display
+    staticLabelClassName: str = None  # 2.4.0 The class name of the Label for static display
+    staticInputClassName: str = None  # 2.4.0 The class name of value when static display
+    staticSchema: Union[str, list] = None  # SchemaNode
+
+
+class ButtonGroupSelect(FormItem):
+    """Button group select"""
+
+    type: str = "button-group-select"
+    vertical: bool = None  # Default False, use vertical mode
+    tiled: bool = None  # Default False, use tile mode
+    btnLevel: LevelEnum = LevelEnum.default  # button style
+    btnActiveLevel: LevelEnum = LevelEnum.default  # Check button style
+    options: OptionsNode = None  # option group
+    source: API = None  # dynamic group
+    multiple: bool = None  # Default False, multiple choice
+    labelField: str = None  # Default "label"
+    valueField: str = None  # Default "value"
+    joinValues: bool = None  # Default True
+    extractValue: bool = None  # Default False
+    autoFill: dict = None  # autofill
+
+
+class ListSelect(FormItem):
+    """List select, allows images"""
+
+    type: str = "list-select"
+    options: OptionsNode = None  # option group
+    source: API = None  # dynamic group
+    multiple: bool = None  # Default False, multiple choice
+    labelField: str = None  # Default "label"
+    valueField: str = None  # Default "value"
+    joinValues: bool = None  # Default True
+    extractValue: bool = None  # Default False
+    autoFill: dict = None  # autofill
+    listClassName: str = None  # Supports configuring the css class name of the list div. for example:flex justify-between
+
+
+class Form(AmisNode):
+    """Form"""
+
+    class Messages(AmisNode):
+        fetchSuccess: str = None  # Prompt when fetch is successful
+        fetchFailed: str = None  # Prompt when fetch fails
+        saveSuccess: str = None  # Prompt when saving is successful
+        saveFailed: str = None  # Prompt when saving fails
+
+    type: str = "form"  # "form" specifies the Form renderer
+    name: str = None  # After setting a name, it is convenient for other components to communicate with it
+    mode: DisplayModeEnum = None  # Form display mode, can be: normal, horizontal or inline
+    horizontal: Horizontal = None  # Useful when mode is horizontal,
+    # Used to control label {"left": "col-sm-2", "right": "col-sm-10", "offset": "col-sm-offset-2"}
+    title: Optional[str] = None  # Title of the Form
+    submitText: Optional[str] = None  # "Submit" # Default submit button name, if it is set to empty, the default
+    # button can be removed.
+    className: str = None  # The class name of the outer Dom
+    body: List[Union[FormItem, SchemaNode]] = None  # Form item collection
+    actions: List["Action"] = None  # Form submit button, the member is Action
+    actionsClassName: str = None  # class name of actions
+    messages: Messages = None  # The message prompts to be overridden. The default message reads the message returned
+    # by the API, but it can be overridden here.
+    wrapWithPanel: bool = None  # whether to wrap the Form with panel, if set to false, actions will be invalid.
+    panelClassName: str = None  # The class name of the outer panel
+    api: API = None  # The api that Form uses to save data.
+    initApi: API = None  # The api that Form uses to get initial data.
+    rules: list = None  # Form combination validation rules Array<{rule:string;message:string}>
+    interval: int = None  # refresh time (minimum 3000)
+    silentPolling: bool = None  # False # whether to show the loading animation when the configuration is refreshed
+    stopAutoRefreshWhen: str = None  # Configure the condition for stopping refresh by expression
+    initAsyncApi: API = None  # The api that Form uses to obtain initial data, which is different from initApi,
+    # will keep polling and request this interface until the returned finished attribute is true.
+    initFetch: bool = None  # After initApi or initAsyncApi is set, the request will be sent by default, and if it is
+    # set to false, the interface will not be requested at the beginning
+    initFetchOn: str = None  # Use expression to configure
+    initFinishedField: Optional[str] = None  # After setting initAsyncApi, by default, the data.finished of the
+    # returned data will be used to judge whether it is completed.
+    # Can also be set to other xxx, it will be obtained from data.xxx
+    initCheckInterval: int = None  # After setting initAsyncApi, the default pull interval
+    asyncApi: API = None  # After setting this property, after the form is submitted and sent to save the interface,
+    # it will continue to poll and request the interface, and it will not end until the returned finished property is
+    # true.
+    checkInterval: int = None  # The time interval for polling requests, the default is 3 seconds. Setting asyncApi
+    # is valid
+    finishedField: Optional[str] = None  # Set this property if the field name that decides to end is not finished,
+    # such as is_success
+    submitOnChange: bool = None  # Form modification is submitted
+    submitOnInit: bool = None  # Submit once initially
+    resetAfterSubmit: bool = None  # whether to reset the form after submitting
+    primaryField: str = None  # Set the primary key id. When set, it will only carry this data when checking whether
+    # the form is completed (asyncApi).
+    target: str = None  # The default form submission itself will save the data by sending the api, but you can also
+    # set the name value of another form, or another CRUD model name value. If the target target is a Form,
+    # the target Form will trigger initApi again, and the api can get the current form data. If the target is a CRUD
+    # model, the target model will re-trigger the search with the current Form data as the parameter. When the target
+    # is window, the data of the current form will be attached to the page address.
+    redirect: str = None  # After setting this attribute, after the Form is saved successfully, it will automatically
+    # jump to the specified page. Support relative addresses, and absolute addresses (relative to the group).
+    reload: str = None  # Refresh the target object after the operation. Please fill in the name value set by the
+    # target component. If it is filled in window, the current page will be refreshed as a whole.
+    autoFocus: bool = None  # whether to auto focus.
+    canAccessSuperData: bool = None  # Specify whether the upper layer data can be automatically obtained and mapped
+    # to the form item
+    persistData: str = None  # Specify a unique key to configure whether to enable local caching for the current form
+    clearPersistDataAfterSubmit: bool = None  # Specify whether to clear the local cache after the form is submitted
+    # successfully
+    preventEnterSubmit: bool = None  # Disable EnterSubmit form submission
+    trimValues: bool = None  # trim each value of the current form item
+    promptPageLeave: bool = None  # The form has not been saved, whether to confirm with a pop-up box before leaving
+    # the page.
+    columnCount: int = None  # The form item is displayed as several columns
+    debug: bool = None
+    inheritData: bool = None  # true # The default form is to create its own data field in the form of a data link,
+    # and only the data in this data field will be sent when the form is submitted. If you want to share the
+    # upper layer data field, you can set this attribute to false, so that the data in the upper layer data field
+    # does not need to be sent in the form with hidden fields or explicit mapping.
+    static: bool = None  # false # 2.4.0. The entire form is displayed statically.
+    # For details, please refer to the:https://aisuda.bce.baidu.com/amis/examples/form/switchDisplay.
+    staticClassName: str = None  # 2.4.0. The name of the class used when the form is statically displayed
+    labelAlign: Literal["right", "left"] = None  # "right"  # 表单项标签对齐方式，默认右对齐，仅在 mode为horizontal 时生效
+    labelWidth: Union[int, str] = None  # 表单项标签自定义宽度
+    persistDataKeys: List[str] = None  # 指指定只有哪些 key 缓存
+    closeDialogOnSubmit: bool = None  # 提交的时候是否关闭弹窗
+
+
+class InputSubForm(FormItem):
+    """Subform"""
+
+    type: str = "input-sub-form"
+    multiple: bool = None  # False # whether it is multiple selection mode
+    labelField: str = None  # When this field exists in the value, the button name will be displayed using the value
+    # of this field.
+    btnLabel: str = None  # "Settings" # Default button name
+    minLength: int = None  # 0 # Limit the minimum number.
+    maxLength: int = None  # 0 # Limit the maximum number.
+    draggable: bool = None  # whether it can be draggable and sorted
+    addable: bool = None  # whether it can be added
+    removable: bool = None  # whether it can be removed
+    addButtonClassName: str = None  # "``" # Add button CSS class name
+    itemClassName: str = None  # "``" # Value element CSS class name
+    itemsClassName: str = None  # "``" # Value wrapping element CSS class name
+    form: Form = None  # Subform configuration, same as Form
+    addButtonText: str = None  # "``" # Customize the text of the new item
+    showErrorMsg: bool = None  # True # whether to display the error message in the lower left corner
+
+
+class Button(FormItem):
+    """Button"""
+
+    className: str = None  # Specify the add button class name
+    href: str = None  # Click the jump address, specify the behavior of this attribute button is consistent with the
+    # a link
+    size: str = None  # Set button size 'xs'|'sm'|'md'|'lg'
+    actionType: str = None  # Set the button type 'button'|'reset'|'submit'| 'clear'| 'url'
+    level: LevelEnum = None  # Set button style 'link'|'primary'|'enhance'|'secondary'|'info'|'success'|'warning
+    # '|'danger'|'light'| 'dark'|'default'
+    tooltip: Union[str, dict] = None  # Bubble tip content TooltipObject
+    tooltipPlacement: str = None  # Balloon positioner 'top'|'right'|'bottom'|'left'
+    tooltipTrigger: str = None  # trigger tootip 'hover'|'focus'
+    disabled: bool = None  # button disabled state
+    block: bool = None  # Option to adjust button width to its parent width
+    loading: bool = None  # Show button loading effect
+    loadingOn: str = None  # Display button loading expression
+
+
+class InputFormula(FormItem):
+    """Input Formula Editor"""
+
+    type: str = "input-formula"
+    title: str = None  # title
+    header: str = None  # Editor header title, if not set, the form item labelfield is used by default
+    evalMode: bool = None  # default True, Expression mode or template mode (False),
+    # template mode requires the expression to be written between ${and }.
+    variables: List[dict] = None  # Available variables, {label: string; value: string; children?: any[]; tag?: string}
+    variableMode: Literal["tabs", "tree", "list"] = "list"  # Can be configured as tabs or tree ,
+    # defaults to a list, which supports grouping.
+    inputMode: Literal["button", "input-button", "input-group"] = None  # Display mode of the control
+    icon: str = None  # fa icon
+    btnLabel: str = None  # The button text, which inputModetakesbutton
+    level: LevelEnum = LevelEnum.default  # button stlye
+    allowInput: bool = None  # default -, Whether the input box can be entered
+    btnSize: Literal["xs", "sm", "md", "lg"] = None  # button size
+    borderMode: Literal["full", "half", "none"] = None  # Input box border mode
+    placeholder: str = None  # input box placeholder
+    className: str = None  # Control outer CSS style class name
+    variableClassName: str = None  # Variable panel CSS style class name
+    functionClassName: str = None  # Function panel CSS style class name
+    mixedMode: bool = None  # default False, if True it supports values in both text and formula formats
+
+
+class InputArray(FormItem):
+    """Array input box"""
+
+    type: str = "input-array"
+    items: FormItem = None  # Configure single item form type
+    addable: bool = None  # whether it can be added.
+    removable: bool = None  # whether it can be removed
+    draggable: bool = None  # False # whether drag sorting is possible, it should be noted that when drag sorting is
+    # enabled, there will be an additional $id field
+    draggableTip: str = None  # Draggable prompt text, the default is: "Order can be adjusted by dragging the [Swap]
+    # button in each row"
+    addButtonText: str = None  # "Add" # Add button text
+    minLength: int = None  # Limit the minimum length
+    maxLength: int = None  # limit max length
+    scaffold: Any = None  # 新增成员时的默认值，一般根据items的数据类型指定需要的默认值
+
+
+class Hidden(FormItem):
+    """Hidden fields"""
+
+    type: str = "hidden"
+
+
+class Checkbox(FormItem):
+    """Check box"""
+
+    type: str = "checkbox"
+    option: str = None  # option description
+    trueValue: Any = None  # identifies the true value
+    falseValue: Any = None  # identifies a false value
+    optionType: Literal["default", "button"] = None  # 设置 option 类型
+
+
+class Radios(FormItem):
+    """Single box"""
+
+    type: str = "radios"
+    options: List[Union[dict, str]] = None  # Option group
+    source: API = None  # Dynamic option group
+    labelField: bool = None  # "label" # option label field
+    valueField: bool = None  # "value" # option value field
+    columnsCount: int = None  # 1 # options are displayed in several columns, default is one column
+    inline: bool = None  # True # whether to display as one line
+    selectFirst: bool = None  # False # whether to select the first one by default
+    autoFill: dict = None  # autofill
+
+
+class ChartRadios(Radios):
+    """Single box"""
+
+    type: str = "chart-radios"
+    config: dict = None  # echart chart configuration
+    showTooltipOnHighlight: bool = None  # False # whether to show tooltip when highlighted
+    chartValueField: str = None  # "value" # Chart value field name
+
+
+class Checkboxes(FormItem):
+    """Checkbox"""
+
+    type: str = "checkboxes"
+    options: OptionsNode = None  # option group
+    source: API = None  # Dynamic option group
+    delimiter: str = None  # "," # splicer
+    labelField: str = None  # "label" # option label field
+    valueField: str = None  # "value" # option value field
+    joinValues: bool = None  # True # join values
+    extractValue: bool = None  # False # extract value
+    columnsCount: int = None  # 1 # options are displayed in several columns, default is one column
+    checkAll: bool = None  # False # whether to support select all
+    inline: bool = None  # True # whether to display as one line
+    defaultCheckAll: bool = None  # False # whether to check all by default
+    creatable: bool = None  # False # New option
+    createBtnLabel: str = None  # "Add option" # Add option
+    addControls: List[FormItem] = None  # Customize new form items
+    addApi: API = None  # Configure the new option interface
+    editable: bool = None  # False # edit options
+    editControls: List[FormItem] = None  # Customize edit form items
+    editApi: API = None  # Configure editing options interface
+    removable: bool = None  # False # remove option
+    deleteApi: API = None  # Configure delete option interface
+    optionType: Literal["default", "button"] = None  # "default"  # 按钮模式
+    itemClassName: str = None  # 选项样式类名
+    labelClassName: str = None  # 选项标签样式类名
+
+
+class InputCity(FormItem):
+    """City selector"""
+
+    type: str = "input-city"
+    allowCity: bool = None  # True # Allow city selection
+    allowDistrict: bool = None  # True # Allow region selection
+    searchable: bool = None  # False # whether to display the search box
+    extractValue: bool = None  # True# whether to extract the value, if set to false, the value format will become an
+    # object, including code, province, city and district text information.
+
+
+class InputColor(FormItem):
+    """Color picker"""
+
+    type: str = "input-color"
+    format: str = None  # "hex" # Please choose hex, hls, rgb or rgba.
+    presetColors: List[str] = None  # "Selector preset color value" # The default color at the bottom of the selector,
+    # if the array is empty, the default color will not be displayed
+    allowCustomColor: bool = None  # True # When false, only colors can be selected, use presetColors to set the
+    # color selection range
+    clearable: bool = None  # "label" # whether to display the clear button
+    resetValue: str = None  # "" # After clearing, the form item value is adjusted to this value
+
+
+class Combo(FormItem):
+    """combination"""
+
+    type: str = "combo"
+    formClassName: str = None  # The class name of a single group of form items
+    addButtonClassName: str = None  # Add button CSS class name
+    items: List[FormItem] = None  # Form items displayed in combination
+    # items[x].columnClassName: str = None # The class name of the column, which can be used to configure the column
+    # width. The default is evenly distributed. items[x].unique: bool = None # Set whether the current column value
+    # is unique, that is, repeated selection is not allowed.
+    noBorder: bool = False  # whether to display a border for a single group of form items
+    scaffold: dict = {}  # initial value for a single set of form items
+    multiple: bool = False  # whether to select multiple
+    multiLine: bool = False  # The default is to display a row horizontally, after setting it will be displayed
+    # vertically
+    minLength: int = None  # Minimum number of added bars
+    maxLength: int = None  # The maximum number of bars to add
+    flat: bool = False  # whether to flatten the result (remove the name), only valid when the length of items is 1
+    # and multiple is true.
+    joinValues: bool = True  # The default is true When flattening is enabled, whether to send it to the backend in
+    # the form of a delimiter, otherwise it is in the form of an array.
+    delimiter: str = None  # "False" # What delimiter to use when flattening is on and joinValues is true.
+    addable: bool = False  # whether it can be added
+    addButtonText: str = None  # "Add" # Add button text
+    removable: bool = False  # whether it can be removed
+    deleteApi: API = None  # If configured, an api will be sent before deletion, and the deletion will be completed
+    # after the request is successful
+    deleteConfirmText: str = None  # "Confirm to delete?" # It only takes effect when deleteApi is configured! Used
+    # for user confirmation when deleting
+    draggable: bool = False  # whether drag sorting is possible, it should be noted that when drag sorting is
+    # enabled, there will be an additional $id field
+    draggableTip: str = None  # "Order can be adjusted by dragging the [Exchange] button in each row" # Draggable
+    # prompt text
+    subFormMode: str = None  # "normal" # optional normal, horizontal, inline
+    placeholder: str = None  # "``" # Displayed when there is no member.
+    canAccessSuperData: bool = False  # Specify whether the upper layer data can be automatically obtained and mapped
+    # to the form item
+    conditions: dict = None  # The form of an array contains the rendering types of all conditions. The test in a
+    # single array is the judgment condition, and the items in the array are the schema rendered after meeting the
+    # condition.
+    typeSwitchable: bool = False  # whether to switch conditions, use with conditions
+    strictMode: bool = True  # The default is strict mode. When set to false, when other form items are updated,
+    # the form items in them can also be obtained in time, otherwise they will not.
+    syncFields: List[str] = []  # Configure sync fields. Only valid when strictMode is false.
+    # If the Combo level is deep, the data from the bottom layer may be out of sync. But configuring this property
+    # for combo can be synchronized. Input format: ["os"]
+    nullable: bool = False  # Allow null, if the validator is configured in the sub-form item, and it is a single
+    # mode. You can allow the user to choose to clear (do not fill).
+
+
+class ConditionBuilder(FormItem):
+    """Combined conditions"""
+
+    class Field(AmisNode):
+        type: str = "text"  # The field configuration is configured as "text"
+        label: str = None  # Field name.
+        placeholder: str = None  # placeholder
+        operators: List[str] = None  # If not so many, you can configure overrides.
+        # Default is ['equal','not_equal','is_empty','is_not_empty','like','not_like','starts_with','ends_with']
+        defaultOp: str = None  # defaults to "equal"
+
+    class Text(Field):
+        """text"""
+
+    class Number(Field):
+        """number"""
+
+        type: str = "number"
+        minimum: float = None  # minimum value
+        maximum: float = None  # maximum value
+        step: float = None  # step size
+
+    class Date(Field):
+        """date"""
+
+        type: str = "date"
+        defaultValue: str = None  # default value
+        format: str = None  # Default "YYYY-MM-DD" value format
+        inputFormat: str = None  # Default "YYYY-MM-DD" display date format.
+
+    class Datetime(Date):
+        """Date Time"""
+
+        type: str = "datetime"
+        timeFormat: str = None  # The default "HH:mm" time format determines which input boxes are available.
+
+    class Time(Date):
+        """time"""
+
+        type: str = "datetime"
+
+    class Select(Field):
+        """Drop down to select"""
+
+        type: str = "select"
+        options: OptionsNode = None  # options list, Array<{label: string, value: any}>
+        source: API = None  # Dynamic options, please configure api.
+        searchable: bool = None  # whether it can be searched
+        autoComplete: API = None  # Automatically prompt for completion, each time new content is entered,
+        # the interface will be called, and the update options will be returned according to the interface.
+
+    type: str = "condition-builder"
+    fields: List[Field] = None  # It is an array type, each member represents an optional field, supports multiple
+    # layers, configuration example
+    className: str = None  # Outer dom class name
+    fieldClassName: str = None  # The class name of the input field
+    source: str = None  # Pull configuration items remotely
+
+
+class Editor(FormItem):
+    """Code Editor"""
+
+    type: str = "editor"
+    language: str = None  # "javascript" # The language highlighted by the editor, which can be obtained through the
+    # ${xxx} variable
+    # bat, c, coffeescript, cpp, csharp, css, dockerfile, fsharp, go, handlebars, html, ini, java,
+    # javascript, json, less, lua, markdown, msdax, objective-c, php, plaintext, postiats, powershell,
+    # pug, python, r, razor, ruby, sb, scss, shell, sol, sql, swift, typescript, vb, xml, yaml
+    size: str = None  # "md" # Editor height, the value can be md, lg, xl, xxl
+    allowFullscreen: bool = None  # False # whether to display the full screen mode switch
+    options: dict = None  # Other configurations of the monaco editor, such as whether to display line numbers, etc.,
+    # please refer to here, but readOnly cannot be set, read-only mode needs to use disabled: true
+
+
+class DiffEditor(FormItem):
+    """Code Editor"""
+
+    type: str = "diff-editor"
+    language: str = None  # "javascript" # The language highlighted by the editor, which can be obtained through the
+    # ${xxx} variable
+    # bat, c, coffeescript, cpp, csharp, css, dockerfile, fsharp, go, handlebars, html, ini, java,
+    # javascript, json, less, lua, markdown, msdax, objective-c, php, plaintext, postiats, powershell,
+    # pug, python, r, razor, ruby, sb, scss, shell, sol, sql, swift, typescript, vb, xml, yaml
+    diffValue: Template = None  # the diff value or reference to other data entry like '${value1}'
+
+
+class Formula(AmisNode):
+    """Formula for fields, linked by 'name'"""
+
+    type: str = "formula"
+    name: str = None  # The formula result will be applied to the variable (name) specified here.
+    formula: Expression = None  # the formula itself
+    condition: Expression = None  # condition for the formula
+    initSet: bool = None  # Default True, whether to set at initialization
+    autoSet: bool = None  # Default True, Observe the formula result, if the calculation result changes,
+    # it will be automatically applied to the variable
+    id: bool = None  # Default True, Define a name. When a button's target is specified, it will trigger a formula.
+
+
+class DropDownButton(AmisNode):
+    """Formula for fields, linked by 'name'"""
+
+    type: str = "dropdown-button"
+    label: str = None  # button text
+    className: str = None  # Outer CSS class name
+    btnClassName: str = None  # Button CSS class name
+    menuClassName: str = None  # Dropdown menu CSS class name
+    block: bool = None  # Default False, block style
+    size: Literal["xs", "sm", "md", "lg"] = None  # size, support 'xs', 'sm', 'md','lg'
+    align: Literal["left", "right"] = None  # location align
+    buttons: List[Button] = []  # List of buttons
+    iconOnly: bool = None  # default False, show only icon
+    defaultIsOpened: bool = None  # default False, whether to open by default
+    closeOnOutside: bool = None  # default True, Click whether to collapse the outer area
+    closeOnClick: bool = None  # default False, automatically close dropdown menu after button click
+    trigger: TriggerEnum = TriggerEnum.click  # trigger method
+    hideCaret: bool = None  # default False, Hide drop down icon
+
+
+class EachLoop(AmisNode):
+    """Each loop renderer"""
+
+    type: str = "each"
+    value: list = []  # value for the loop
+    name: str = None  # Data field name
+    source: str = None  # Data mapping source
+    items: dict = None  # {"type": "tpl", "tpl": "< span ..."}
+    placeholder: str = None  # placeholder text when valuevalue does not exist or is an empty array
+
+
+class GridNav(AmisNode):
+    """Grid navigation
+    menu navigation, does not support the configuration of the initialization interface to initialize the data field,
+    so you need to work with similar to Service, Form or CRUD, with the configuration of the interface to initialize
+    the data field components, or manually initialize the data field, and then through the source property,
+    to obtain the data in the data chain to complete the menu display.
+    """
+
+    class OptionsItem(AmisNode):
+        icon: str = None  # default '', list item icon
+        text: str = None  # default '', list item text
+        badge: Badge = None  # Bade Schema, list item badge
+        link: str = None  # default '', Internal page path or external URL address, takes precedence over clickAction
+        blank: bool = None  # default False, Whether a new page is opened, valid when link is url
+        clickAction: Action = None  # ActionSchema
+
+    type: str = "grid-nav"
+    className: str = None  # outer dom classname
+    itemClassName: str = None  # item custom css classname
+    value: List = None  # array of images
+    source: str = None  # data source
+    square: bool = None  # default False, whether to fix list items to be square
+    center: bool = None  # default False, whether to center the content of the list item
+    border: bool = None  # default False, whether to show the list item border
+    gutter: int = None  # default -, px, the spacing between list items
+    reverse: bool = None  # default False, whether to swap the position of the icon and text
+    iconRatio: int = None  # default 60, Icon width ratio, in %
+    direction: Literal["horizontal", "vertical"] = "vertical"  # The direction in which the list items are arranged
+    columnNum: int = None  # default 4,
+    options: List[OptionsItem] = None  # the option items
+
+
+class CollapseGroup(AmisNode):
+    """Grid navigation
+    menu navigation, does not support the configuration of the initialization interface to initialize the data field,
+    so you need to work with similar to Service, Form or CRUD, with the configuration of the interface to initialize
+    the data field components, or manually initialize the data field, and then through the source property,
+    to obtain the data in the data chain to complete the menu display.
+    """
+
+    class CollapseItem(AmisNode):
+        type: str = "collapse"
+        disabled: bool = None  # default False
+        collapsed: bool = None  # default True
+        key: Union[int, str] = None  # default -, logo
+        header: Union[str, SchemaNode] = None  # default -, title
+        body: Union[str, SchemaNode] = None  # default -, content
+
+    type: str = "collapse-group"
+    activeKey: Union[str, int, List[Union[int, str]]] = None  # Initialize the key to activate the panel
+    disabled: bool = None  # default False
+    accordion: bool = None  # default False, accordion mode
+    expandIcon: SchemaNode = None  # Custom toggle icon
+    expandIconPosition: Literal["left", "right"] = "left"  # icon position
+    body: List[Union[CollapseItem, SchemaNode]] = None  # group content
+
+
+class Markdown(AmisNode):
+    """Markdown rendering"""
+
+    type: str = "markdown"
+    name: str = None  # Field name, specifying the key when the form item is submitted
+    value: Union[int, str] = None  # field value
+    className: str = None  # The outermost class name of the form
+    src: API = None  # external address
+    options: dict = None  # html, whether to support html tags, default false;
+    # linkify, whether to automatically identify the link, the default value is true; breaks, whether the carriage
+    # return is a newline, the default value is false
+
+
+class OfficeViewer(AmisNode):
+    """Office Viewer：https://aisuda.bce.baidu.com/amis/zh-CN/components/office-viewer"""
+
+    type: str = "office-viewer"
+    src: API = None  # Document address
+    loading: bool = None  # Whether to display the loading icon
+    enableVar: bool = None  # Whether to enable variable replacement function
+    wordOptions: dict = None  # Word rendering configuration
+
+
+class InputFile(FormItem):
+    """File Upload"""
+
+    type: str = "input-file"
+    receiver: API = None  # Upload file interface
+    accept: str = None  # "text/plain" # Only plain text is supported by default. To support other types,
+    # please configure this property as the file suffix .xxx
+    asBase64: bool = None  # False # Assign the file to the current component in the form of base64
+    asBlob: bool = None  # False # Assign the file to the current component in binary form
+    maxSize: int = None  # There is no limit by default, when set, the file size larger than this value will not be
+    # allowed to upload. unit is B
+    maxLength: int = None  # There is no limit by default. When set, only the specified number of files can be
+    # uploaded at a time.
+    multiple: bool = None  # False # whether to select multiple.
+    joinValues: bool = None  # True # join values
+    extractValue: bool = None  # False # extract value
+    delimiter: str = None  # "," # splicer
+    autoUpload: bool = None  # True # No selection will automatically start uploading
+    hideUploadButton: bool = None  # False # hide the upload button
+    stateTextMap: dict = None  # Upload state text Default: {init: '', pending: 'Waiting to upload', uploading:
+    # 'Uploading', error: 'Upload error', uploaded: 'Uploaded',ready: ''}
+    fileField: str = None  # "file" # You can ignore this attribute if you don't want to store it yourself.
+    nameField: str = None  # "name" # Which field is returned by the interface to identify the file name
+    valueField: str = None  # "value" # The value of the file is identified by that field.
+    urlField: str = None  # "url" # The field name of the file download address.
+    btnLabel: str = None  # The text of the upload button
+    downloadUrl: Union[bool, str] = None  # Version 1.1.6 supports post:http://xxx.com/${value}
+    # When the file path is displayed by default, it will support direct download. It can support adding a prefix
+    # such as: http://xx.dom/filename= . If you don't want this, you can set the current configuration item to false.
+    useChunk: bool = None  # The server where amis is located limits the file upload size to no more than 10M,
+    # so when amis selects a large file, it will automatically change to the chunked upload mode.
+    chunkSize: int = None  # 5 * 1024 * 1024 # chunk size
+    startChunkApi: API = None  # startChunkApi
+    chunkApi: API = None  # chunkApi
+    finishChunkApi: API = None  # finishChunkApi
+    autoFill: Dict[str, str] = None  # After the upload is successful, the value returned by the upload interface can
+    # be filled into a form item by configuring autoFill (not supported under non-form)
+
+
+class InputExcel(FormItem):
+    """Parse Excel"""
+
+    type: str = "input-excel"
+    allSheets: bool = None  # False # whether to parse all sheets
+    parseMode: str = None  # 'array' or 'object' parsing mode
+    includeEmpty: bool = None  # True # whether to include empty values
+    plainText: bool = None  # True # whether to parse as plain text
+
+
+class InputTable(FormItem):
+    """sheet"""
+
+    type: str = "input-table"  # Specify as Table renderer
+    showIndex: bool = None  # False # Show index
+    perPage: int = None  # Set how many pieces of data are displayed on one page. 10
+    addable: bool = None  # False # whether to add a line
+    editable: bool = None  # False # whether editable
+    removable: bool = None  # False # whether it can be removed
+    showAddBtn: bool = None  # True # whether to show the add button
+    addApi: API = None  # API submitted when adding
+    updateApi: API = None  # API submitted when modified
+    deleteApi: API = None  # API submitted when deleting
+    addBtnLabel: Union[bool, Template] = None  # Add button name
+    addBtnIcon: str = None  # "plus" # Add button icon
+    copyBtnLabel: Union[bool, Template] = None  # Copy button text
+    copyBtnIcon: str = None  # "copy" # Copy button icon
+    editBtnLabel: Union[bool, Template] = None  # "" # Edit button name
+    editBtnIcon: str = None  # "pencil" # edit button icon
+    deleteBtnLabel: Union[bool, Template] = None  # "" # delete button name
+    deleteBtnIcon: str = None  # "minus" # delete button icon
+    confirmBtnLabel: Union[bool, Template] = None  # "" # Confirm edit button name
+    confirmBtnIcon: str = None  # "check" # Confirm edit button icon
+    cancelBtnLabel: Union[bool, Template] = None  # "" # Cancel edit button name
+    cancelBtnIcon: str = None  # "times" # Cancel edit button icon
+    needConfirm: bool = None  # True # whether to confirm the operation, it can be used to control the operation
+    # interaction of the control table
+    canAccessSuperData: bool = None  # False # whether you can access the parent data, that is, the same level data
+    # in the form, usually need to be used with strictMode
+    strictMode: bool = None  # True # For performance, the default value of other form items will not update the
+    # current table. Sometimes, in order to obtain other form item fields synchronously, you need to enable this.
+    columns: list = None  # "[]" # Column information
+    # columns[x].quickEdit: boolean|object = None # Use with editable as true columns[x].quickEditOnUpdate:
+    # boolean|object = None # Edit configuration that can be used to distinguish between new mode and update mode
+
+
+class InputGroup(FormItem):
+    """Combination of input boxes"""
+
+    type: str = "input-group"
+    className: str = None  # CSS class name
+    body: List[FormItem] = None  # Form item collection
+
+
+class Group(InputGroup):
+    """Form item group"""
+
+    type: str = "group"
+    mode: DisplayModeEnum = None  # Display the default, the same as the mode in Form
+    gap: str = None  # Gap between form items, optional: xs, sm, normal
+    direction: str = None  # "horizontal" # Can be configured to display horizontally or vertically. The
+    # corresponding configuration items are: vertical, horizontal
+
+
+class InputImage(FormItem):
+    """upload picture"""
+
+    class CropInfo(BaseAmisModel):
+        aspectRatio: float = None  # Crop ratio. Floating point, the default is 1, which is 1:1. If you want to set
+        # 16:9, please set 1.7777777777777777, which is 16/9. .
+        rotatable: bool = None  # False # whether to rotate when cropping
+        scalable: bool = None  # False # whether it can be scaled when cropping
+        viewMode: int = None  # 1 # View mode when cropping, 0 is unlimited
+
+    class Limit(BaseAmisModel):
+        width: int = None  # Limit image width.
+        height: int = None  # Limit image height.
+        minWidth: int = None  # Limit image minimum width.
+        minHeight: int = None  # Limit image minimum height.
+        maxWidth: int = None  # Limit the maximum width of the image.
+        maxHeight: int = None  # Limit the maximum height of the image.
+        aspectRatio: float = None  # Limit the aspect ratio of the image, the format is a floating-point number,
+        # the default is 1, which is 1:1, If you want to set 16:9, please set 1.7777777777777777 which is 16/9. If
+        # you don't want to limit the ratio, set an empty string.
+
+    type: str = "input-image"
+    receiver: API = None  # Upload file interface
+    accept: str = None  # ".jpeg,.jpg,.png,.gif" # Supported picture types and formats, please configure this
+    # property as picture suffix, such as .jpg,.png
+    maxSize: int = None  # There is no limit by default, when set, the file size larger than this value will not be
+    # allowed to upload. unit is B
+    maxLength: int = None  # There is no limit by default. When set, only the specified number of files can be
+    # uploaded at a time.
+    multiple: bool = None  # False # whether to select multiple.
+    joinValues: bool = None  # True # join values
+    extractValue: bool = None  # False # extract value
+    delimiter: str = None  # "," # splicer
+    autoUpload: bool = None  # True # No selection will automatically start uploading
+    hideUploadButton: bool = None  # False # hide the upload button
+    fileField: str = None  # "file" # You can ignore this attribute if you don't want to store it yourself.
+    crop: Union[bool, CropInfo] = None  # Used to set whether to support cropping.
+    cropFormat: str = None  # "image/png" # crop file format
+    cropQuality: int = None  # 1 # The quality of the crop file format, for jpeg/webp, between 0 and 1
+    limit: Limit = None  # Limit the size of the image, beyond which it will not be allowed to upload.
+    frameImage: str = None  # Default placeholder image address
+    fixedSize: bool = None  # whether to enable fixed size, if enabled, set fixedSizeClassName at the same time
+    fixedSizeClassName: str = None  # When the fixed size is turned on, the display size is controlled according to this value.
+    # For example, h-30, that is, the height of the picture frame is h-30, AMIS will automatically set the zoom ratio
+    # to the width of the position occupied by the default image, and the final uploaded image will be scaled
+    # accordingly according to this size.
+    autoFill: Dict[str, str] = None  # After the upload is successful, the value returned by the upload interface can
+    # be filled into a form item by configuring autoFill (not supported under non-form)
+    initAutoFill: bool = None  # False  # 表单反显时是否执行 autoFill
+    uploadBtnText: Union[str, SchemaNode] = None  # 上传按钮文案。支持tpl、schema形式配置。
+    dropCrop: bool = None  # True  # 图片上传后是否进入裁剪模式
+    initCrop: bool = None  # False  # 图片选择器初始化后是否立即进入裁剪模式
+
+
+class LocationPicker(FormItem):
+    """Location"""
+
+    type: str = "location-picker"
+    vendor: str = "baidu"  # Map vendor, currently only Baidu map is implemented
+    ak: str = ...  # ak # registered address of Baidu map: http://lbsyun.baidu.com/
+    clearable: bool = None  # False # whether the input box can be cleared
+    placeholder: str = None  # "Please select a location" # Default prompt
+    coordinatesType: str = None  # "bd09" # Default is Baidu coordinates, can be set to 'gcj02'
+
+
+class InputNumber(FormItem):
+    """Number input box"""
+
+    type: str = "input-number"
+    min: Union[int, Template] = None  # minimum value
+    max: Union[int, Template] = None  # maximum value
+    step: int = None  # step size
+    precision: int = None  # Precision, i.e. a few decimal places
+    showSteps: bool = None  # True # whether to show up and down click buttons
+    prefix: str = None  # prefix
+    suffix: str = None  # suffix
+    kilobitSeparator: bool = None  # Kilobit Separator
+
+
+class Picker(FormItem):
+    """List selector"""
+
+    type: str = "picker"  # List pick, similar in function to Select, but it can display more complex information.
+    size: Union[str, SizeEnum] = None  # Supports: xs, sm, md, lg, xl, full
+    options: OptionsNode = None  # option group
+    source: API = None  # Dynamic option group
+    multiple: bool = None  # whether it is multiple choice.
+    delimiter: bool = None  # False # splicer
+    labelField: str = None  # "label" # option label field
+    valueField: str = None  # "value" # option value field
+    joinValues: bool = None  # True # join values
+    extractValue: bool = None  # False # extract value
+    autoFill: dict = None  # autofill
+    modalMode: Literal["dialog", "drawer"] = None  # "dialog" # Set dialog or drawer to configure the popup mode.
+    pickerSchema: Union["CRUD", SchemaNode] = None  # "{mode: 'list', listItem: {title: '${label}'}}"
+    # That is to use the rendering of the List type to display the list information. More configuration reference CRUD
+    embed: bool = None  # False # whether to use embedded mode
+
+
+class Switch(FormItem):
+    """switch"""
+
+    type: str = "switch"
+    option: str = None  # option description
+    onText: str = None  # Text when it is turned on
+    offText: str = None  # text when off
+    trueValue: Any = None  # "True" # identifies the true value
+    falseValue: Any = None  # "false" # identifies a false value
+
+
+class Static(FormItem):
+    """Static display/label"""
+
+    type: str = "static"  # Support to display other non-form item components static-json|static-datetime by
+
+    # configuring type as static-xxx
+
+    class Json(FormItem):
+        type: str = "static-json"
+        value: Union[dict, str]
+
+    class Datetime(FormItem):
+        """Display date"""
+
+        type: str = "static-datetime"
+        value: Union[int, str]  # support 10-bit timestamp: 1593327764
+
+
+class InputText(FormItem):
+    """Input box"""
+
+    type: str = "input-text"  # input-text|input-url|input-email|input-password|divider
+    options: Union[List[str], List[dict]] = None  # Option group
+    source: API = None  # Dynamic option group
+    autoComplete: API = None  # autocomplete
+    multiple: bool = None  # whether to select multiple
+    delimiter: str = None  # Splice ","
+    labelField: str = None  # option label field "label"
+    valueField: str = None  # option value field "value"
+    joinValues: bool = None  # True # join values
+    extractValue: bool = None  # extract value
+    addOn: SchemaNode = None  # Input box add-ons, such as with a prompt text, or with a submit button.
+    trimContents: bool = None  # whether to remove leading and trailing blank text.
+    creatable: bool = None  # whether it can be created, the default is yes, unless it is set to false, only the
+    # value in the option can be selected
+    clearable: bool = None  # whether it can be cleared
+    resetValue: str = None  # Set the value given by this configuration item after clearing.
+    prefix: str = None  # prefix
+    suffix: str = None  # suffix
+    showCounter: bool = None  # whether to show the counter
+    minLength: int = None  # Limit the minimum number of words
+    maxLength: int = None  # Limit the maximum number of characters
+
+
+class InputPassword(InputText):
+    """Password input box"""
+
+    type: str = "input-password"
+
+
+class InputRichText(FormItem):
+    """Rich Text Editor"""
+
+    type: str = "input-rich-text"
+    saveAsUbb: bool = None  # whether to save in ubb format
+    receiver: API = None  # '' # Default image save API
+    videoReceiver: API = None  # '' # Default video save API
+    size: str = None  # The size of the box, which can be set to md or lg
+    options: dict = None  # Need to refer to tinymce or froala documentation
+    buttons: List[str] = None  # froala dedicated, configure the displayed buttons, tinymce can set the toolbar
+    # string through the previous options
+    vendor: str = None  # "vendor": "froala" , configure to use froala editor
+
+
+class InputRating(FormItem):
+    """Input Rating"""
+
+    type: str = "input-rating"
+    half: bool = None  # default False, whether to use half star selection
+    count: int = None  # default 5, amount of total stars
+    readOnly: bool = None  # default False, is it read only
+    allowClear: bool = None  # default True, allow clearing after another click
+    colors: Union[str, dict] = None  # default {'2': '#abadb1', '3': '#787b81', '5': '#ffa900' }, The color in which
+    # the stars are displayed. If a string is passed in, there is only one color.
+    # If an dict is passed in, each level can be customized.
+    # The key name is the limit value of the segment, and the key value is the corresponding class name.
+    inactiveColor: str = None  # default #e7e7e8, color of unselected stars
+    texts: dict = None  # default -, The tooltip text when the star is selected.
+    # key name is the level of the segment, and the value is the corresponding text
+    textPosition: Literal["right", "left"] = "right"  # position of Tooltip
+    char: str = None  # default '*', custom character
+    charClassNme: str = None  # default -, custom char class name
+    textClassName: str = None  # default -, custom text class name
+
+
+class InputRange(FormItem):
+    """Input Range"""
+
+    type: str = "input-range"
+    min: int = None  # default 0, min value
+    max: int = None  # default 100, max value
+    step: int = None  # default 1, step size
+    showSteps: bool = None  # default False, show step size
+    parts: Union[int, List[int]] = None  # default 1, Number of blocks to split
+    marks: Union[str, dict] = None  # Tick Marks, Support Custom Styles, Set Percentages
+    # { [number | string]: ReactNode }or{ [number | string]: { style: CSSProperties, label: ReactNode } }
+    tooltipVisible: bool = None  # default False, whether to show slider labels
+    tooltipPlacement: PlacementEnum = None  # defualt 'top', tooltip placement 'top'|'right'|'bottom'|'left'
+    multiple: bool = None  # default False, support selection range
+    joinValues: bool = None  # default True, show step size
+    delimiter: str = None  # dfeault ',', value delimiter
+    unit: str = None  # unit
+    clearable: bool = None  # default False, whether the precondition can be cleared : showInputValid when enabled
+    showInput: bool = None  # default False, whether to display the input box
+
+
+class Timeline(AmisNode):
+    """Timeline"""
+
+    class TimelineItem(AmisNode):
+        time: str  # Node Time
+        title: Union[str, SchemaNode] = None  # Node Title
+        detail: str = None  # Node detailed description (collapsed)
+        detailCollapsedText: str = None  # default 'Expand'
+        detailExpandedText: str = None  # default 'Collapse'
+        color: Union[str, LevelEnum] = None  # default #DADBDD, Timeline node color
+        icon: str = None  # Icon name, support fontawesome v4 or use url (priority is higher than color)
+
+    type: str = "timeline"
+    items: List[TimelineItem] = None  # default [], Nodes
+    source: API = None  # Data source, you can obtain current variables through data mapping, or configure API objects
+    mode: Literal["left", "right", "alternate"] = "right"  # Position of the text relative to the timeline,
+    # only supported when direction=vertical
+    direction: Literal["vertical", "horizontal"] = "vertical"  # Direction of the Timeline
+    reverse: bool = None  # default False, Reverse chronological order
+
+
+class Steps(AmisNode):
+    """Steps Bar"""
+
+    class StepItem(AmisNode):
+        title: Union[str, SchemaNode] = None  # Title
+        subTitle: Union[str, SchemaNode] = None  # Sub Heading
+        description: Union[str, SchemaNode] = None  # Detail Description
+        value: str = None  # Step Value
+        icon: str = None  # Icon name, support fontawesome v4 or use url (priority is higher than color)
+        className: str = None  # Custom CSS class name
+
+    type: str = "steps"
+    steps: List[StepItem] = None  # default [], List of Steps
+    source: API = None  # Data source, you can obtain current variables through data mapping, or configure API objects
+    name: str = None  # Associated context variable
+    value: Union[int, str, None] = None  # default -, Set the default value, expressions are not supported
+    status: Union[StepStatusEnum, dict] = None  # default -, State of the steps
+    className: str = None  # Custom CSS class name
+    mode: Literal["vertical", "horizontal"] = "horizontal"  # Specifies the step bar direction.
+    labelPlacement: Literal["vertical", "horizontal"] = "horizontal"  # Specify the label placement position.
+    # The default is to place it horizontally to the right of the icon, and optional (vertical) below the icon.
+    progressDot: bool = None  # Default False, show dotted step bar
+
+
+class TooltipWrapper(AmisNode):
+    type: str = "tooltip-wrapper"
+    className: str = None  # Content area class name
+    tooltipClassName: str = None  # Text prompt floating layer class name
+    style: Union[str, dict] = None  # Custom style (inline style), highest priority
+    tooltipStyle: Union[str, dict] = None  # floating layer custom style
+    body: SchemaNode = None  # Content container
+    wrapperComponent: str = None  # "div" | "span"
+    inline: bool = None  # default False, whether the content area is displayed inline
+    rootClose: bool = None  # default True, whether to click the non-content area to close the prompt
+    mouseEnterDelay: int = None  # default 0, Floating layer delay display time, in ms
+    mouseLeaveDelay: int = None  # default 300, Floating layer delay hiding time, in ms
+    trigger: Union[TriggerEnum, List[TriggerEnum]] = None  # default 'hover', Floating layer trigger mode, support array writing
+    # "hover" | "click" | "focus" | List["hover", "click", "focus"]
+    disabled: bool = None  # default False, whether to disable overlay prompts
+    enterable: bool = None  # default True, whether the mouse can move into the floating layer
+    showArrow: bool = None  # default True, whether to display the overlay pointing arrow
+    offset: Tuple[int, int] = None  # default [0, 0], relative offset of the position of the text prompt, in px
+    tooltipTheme: Literal["light", "dark"] = "light"  # default light, Theme style
+    placement: PlacementEnum = PlacementEnum.top  # text prompts position of the floating layer
+    content: str = None  # default '',  Text prompt content
+    title: str = None  # default '', tooltip title
+
+
+class InputTag(FormItem):
+    """Input Tag"""
+
+    type: str = "input-tag"
+    options: List[Union[str, dict]] = None  # default option group
+    optionsTip: List[Union[str, dict]] = None  # default "Your most recent tags", option hint
+    source: API = None  # default 	Dynamic option group
+    delimiter: str = None  # default False, delimiter option
+    labelField: str = None  # default "label", option label field
+    valueField: str = None  # default "value", option value field
+    joinValues: bool = None  # default True, Splice value
+    extractValue: bool = None  # default False, extract value
+    clearable: bool = None  # default False, whether to show a delete icon on the right when there is a value.
+    resetValue: str = None  # default "", Set the value given by this configuration item after deletion.
+    max: int = None  # Maximum number of tags allowed to be added
+    maxTagLength: int = None  # Maximum text length for a single label
+    maxTagCount: int = None  # The maximum number of labels to be displayed. If the number is exceeded,
+    # it will be displayed in the form of a floating layer.
+    # It will only take effect when the multi-selection mode is enabled.
+    overflowTagPopover: TooltipWrapper = None  # default {"placement": "top", "trigger": "hover", "showArrow": false,
+    # "offset": [0, -10]}	Store the configuration properties of the floating layer,
+    # please refer to Tooltip for detailed configuration
+    enableBatchAdd: bool = None  # default 	False, whether to enable batch add mode
+    separator: str = None  # default "-", After batch adding is enabled, enter the delimiter of multiple labels,
+    # support multiple symbols
+
+
+class Select(FormItem):
+    """Drop down box"""
+
+    type: str = "select"
+    options: OptionsNode = None  # option group
+    source: API = None  # Dynamic option group
+    autoComplete: API = None  # Automatic prompt completion
+    delimiter: Union[bool, str] = None  # False # Splice
+    labelField: str = None  # "label" # option label field
+    valueField: str = None  # "value" # option value field
+    joinValues: bool = None  # True # join values
+    extractValue: bool = None  # False # extract value
+    checkAll: bool = None  # False # whether to support select all
+    checkAllLabel: str = None  # "Select All" # Text to be selected
+    checkAllBySearch: bool = None  # False # When there is a search, only all items hit by the search are selected
+    defaultCheckAll: bool = None  # False # whether to check all by default
+    creatable: bool = None  # False # New option
+    multiple: bool = None  # False # Multiple choice
+    searchable: bool = None  # False # search
+    createBtnLabel: str = None  # "Add option" # Add option
+    addControls: List[FormItem] = None  # Customize new form items
+    addApi: API = None  # Configure the new option interface
+    editable: bool = None  # False # edit options
+    editControls: List[FormItem] = None  # Customize edit form items
+    editApi: API = None  # Configure editing options interface
+    removable: bool = None  # False # remove option
+    deleteApi: API = None  # Configure delete option interface
+    autoFill: dict = None  # autofill
+    menuTpl: str = None  # Supports configuring custom menus
+    clearable: bool = None  # whether to support clearing in radio mode
+    hideSelected: bool = None  # False # hide the selected option
+    mobileClassName: str = None  # Mobile floating class name
+    selectMode: str = None  # Optional: group, table, tree, chained, associated. They are: list form, table form,
+    # tree selection form, Cascade selection form, association selection form (the difference from cascading
+    # selection is that the cascade is infinite, while the association has only one level, and the left side of the
+    # association can be a tree).
+    searchResultMode: str = None  # If the value of selectMode is not set, it can be configured separately. Refer to
+    # selectMode to determine the display form of search results.
+    columns: List[dict] = None  # When the display form is table, it can be used to configure which columns are
+    # displayed, which is similar to the columns configuration in table, but only has the display function.
+    leftOptions: List[dict] = None  # Used to configure the left option set when the display form is associated.
+    leftMode: str = None  # When the display form is associated, it is used to configure the left selection form,
+    # support list or tree. Default is list.
+    rightMode: str = None  # When the display form is associated, it is used to configure the right selection form,
+    # optional: list, table, tree, chained.
+
+
+class ChainedSelect(FormItem):
+    """Chained Drop down boxs"""
+
+    type: str = "chained-select"
+    options: OptionsNode = None  # option group
+    source: API = None  # Dynamic option group
+    autoComplete: API = None  # Automatic prompt completion
+    delimiter: str = None  # Default ',', Splice
+    labelField: str = None  # Default "label", option label field
+    valueField: str = None  # Default "value", option value field
+    joinValues: bool = None  # Default True, join values
+    extractValue: bool = None  # Default False, extract value
+
+
+class NestedSelect(Select):
+    """Cascade selector"""
+
+    type: str = "nested-select"
+    cascade: bool = None  # False # When set to true, child nodes are not automatically selected when the parent node
+    # is selected.
+    withChildren: bool = None  # False # When set to true, when the parent node is selected, the value of the child
+    # node will be included in the value, otherwise only the value of the parent node will be retained.
+    onlyChildren: bool = None  # False # For multiple selections, whether to add only its child nodes to the value
+    # when the parent node is selected.
+    searchPromptText: str = None  # "Enter content to search" # Search box placeholder text
+    noResultsText: str = None  # "No results found" # Text if no results
+    hideNodePathLabel: bool = None  # False # whether to hide the path label information of the selected node in the
+    # selection box
+    onlyLeaf: bool = None  # False # Only leaf nodes are allowed to be selected
+
+
+class Breadcrumb(AmisNode):
+    """Breadcrumb line"""
+
+    class BreadcrumbItem(AmisNode):
+        label: str = None  # label text
+        href: str = None  # link
+        icon: str = None  # fa icon
+        dropdown: List = None  # list of breadcrumbitems as dropdown, needs label, href, icon
+
+    type: str = "breadcrumb"
+    className: str = None  # The outer class name
+    itemClassName: str = None  # Navigation item class name
+    separatorClassName: str = None  # separator class name
+    dropdownClassName: str = None  # Dropdown menu class name
+    dropdownItemClassName: str = None  # Dropdown menu item class name
+    separator: str = ">"  # delimeter
+    labelMaxLength: int = None  # Default 16, max display length
+    tooltipPosition: PlacementEnum = PlacementEnum.top  # tooltip position
+    source: API = None  # dynamic data
+    items: List[BreadcrumbItem] = None  # list of breadcrumb icons
+
+
+class Card(AmisNode):
+    """Card"""
+
+    class Media(AmisNode):
+        type: Literal["image", "video"] = "image"  # multimedia type
+        url: str = None  # image or video link
+        position: PlacementEnum = PlacementEnum.left  # media location
+        className: str = None  # default "w-44 h-28", multimedia CSS class
+        isLive: bool = None  # default False, video is live or not
+        autoPlay: bool = None  # default False, autoplay video
+        poster: Union[bool, str] = None  # default false
+
+    class Header(AmisNode):
+        className: str = None  # The header class name
+        title: str = None  # title
+        titleClassName: str = None  # title class name
+        subTitle: Template = None  # subtitle
+        subTitleClassName: str = None  # subtitle class name
+        subTitlePlaceholder: str = None  # Subtitle placeholder
+        description: Template = None  # Description
+        descriptionClassName: str = None  # Description class name
+        descriptionPlaceholder: str = None  # Description placeholder
+        avatar: Template = None  # picture
+        avatarClassName: str = None  # default "pull-left thumb avatar b-3x m-r", Image includes layer class name
+        imageClassName: str = None  # Image class name
+        avatarText: Template = None  # If no picture is configured, the text will be displayed at the picture
+        avatarTextBackground: str = None  # avatar text background color
+        avatarTextClassName: str = None  # Image text class name
+        highlight: bool = None  # default False, whether to show the active style
+        highlightClassName: str = None  # Active style class name
+        href: str = None  # external link link
+        blank: bool = None  # default True, open link in new window
+
+    type: str = "card"
+    className: str = None  # The outer class name
+    href: str = None  # external link link
+    header: Header = None  # Header object
+    body: List = []  # Content container, mainly used to place non-form item components
+    bodyClassName: str = None  # Content area class name
+    actions: List[Action] = None  # Configure button collection
+    actionsCount: int = None  # default 4, number of buttons in each row
+    itemAction: Action = None  # clicking on a card action
+    media: Media = None  # Media object
+    secondary: Template = None  # secondary note
+    toolbar: List[Action] = None  # toolbar buttons
+    dragging: bool = None  # default False, Whether to show the drag icon
+    selectable: bool = None  # default False, can be selected
+    checkable: bool = None  # default True, selection button is disabled or not
+    selected: bool = None  # default False, selection button is selected or not
+    hideCheckToggler: bool = None  # default False, hide the selection button
+    multiple: bool = None  # default False, multi-select or not
+    useCardLabel: bool = None  # default True, Whether the form item label in the card content area uses the
+    # style inside the Card
+
+
+class Cards(AmisNode):
+    """Cards deck, allows to use data source to display data items as cards, or manual"""
+
+    type: str = "cards"
+    title: str = None  # title
+    source: str = None  # default '${items}', Data source, get the variables in the current data field
+    placeholder: str = None  # default 'No data', placeholder
+    className: str = None  # The outer CSS class name
+    headerClassName: str = None  # default 'amis-grid-header', Top outer CSS class name
+    footerClassName: str = None  # default 'amis-grid-footer', Bottom outer CSS class name
+    itemClassName: str = None  # default 'col-sm-4 col-md-3', Card CSS class name
+    card: Card = None  # configured card object for repeat
+
+
+class ListDisplay(AmisNode):
+    """Cards deck, allows to use data source to display data items as cards, or manual"""
+
+    class ListItem(AmisNode):
+        title: str = None  # title
+        titleClassName: str = None  # title class name
+        subTitle: Template = None  # subtitle
+        avatar: Template = None  # picture
+        avatarClassName: str = None  # default "thumb-sm avatar m-r", Image CSS class name
+        desc: Template = None  # Description
+        body: List = None  # Content container, mainly used to place non-form item components
+        actions: List[Action] = None  # action buttons area
+        actionsPosition: Literal["left", "right"] = "right"  # button position
+
+    type: str = "list"
+    title: str = None  # title
+    source: str = None  # default '${items}', Data source, get the variables in the current data field
+    placeholder: str = None  # default 'No data', placeholder
+    className: str = None  # The outer CSS class name
+    headerClassName: str = None  # default 'amis-grid-header', Top outer CSS class name
+    footerClassName: str = None  # default 'amis-grid-footer', Bottom outer CSS class name
+    listItem: ListItem = None  # configured list object for repeat
+
+
+class Textarea(FormItem):
+    """Multi-line text input box"""
+
+    type: str = "textarea"
+    minRows: int = None  # Minimum number of rows
+    maxRows: int = None  # maximum number of rows
+    trimContents: bool = None  # whether to remove leading and trailing blank text
+    readOnly: bool = None  # read-only
+    showCounter: bool = True  # whether to show the counter
+    minLength: int = None  # Limit the minimum number of words
+    maxLength: int = None  # Limit the maximum number of characters
+
+
+class InputMonth(FormItem):
+    """month"""
+
+    type: str = "input-month"
+    value: str = None  # default value
+    format: str = None  # "X" # Month selector value format, please refer to moment for more format types
+    inputFormat: str = None  # "YYYY-MM" # The display format of the month selector, that is, the timestamp format.
+    # For more format types, please refer to moment
+    placeholder: str = None  # "Please select a month" # placeholder text
+    clearable: bool = None  # True # whether it can be cleared
+
+
+class InputTime(FormItem):
+    """time"""
+
+    type: str = "input-time"
+    value: str = None  # default value
+    timeFormat: str = None  # "HH:mm" # Time selector value format, please refer to moment for more format types
+    format: str = None  # "X" # Time selector value format, please refer to moment for more format types
+    inputFormat: str = None  # "HH:mm" # Time selector display format, that is, timestamp format, please refer to
+    # moment for more format types
+    placeholder: str = None  # "Please select a time" # placeholder text
+    clearable: bool = None  # True # whether it can be cleared
+    timeConstraints: dict = None  # True # Please refer to: react-datetime
+
+
+class InputDatetime(FormItem):
+    """date"""
+
+    type: str = "input-datetime"
+    value: str = None  # default value
+    format: str = None  # "X" # Date time picker value format, please refer to the documentation for more format types
+    inputFormat: str = None  # "YYYY-MM-DD HH:mm:ss" # Date time picker display format, namely timestamp format,
+    # please refer to the documentation for more format types
+    placeholder: str = None  # "Please select a date and time" # placeholder text
+    shortcuts: str = None  # datetime shortcuts
+    minDate: str = None  # Limit the minimum date and time
+    maxDate: str = None  # Limit maximum date time
+    utc: bool = None  # False # save utc value
+    clearable: bool = None  # True # whether it can be cleared
+    embed: bool = None  # False # whether to inline
+    timeConstraints: dict = None  # True # Please refer to: react-datetime
+
+
+class InputDate(FormItem):
+    """date"""
+
+    type: str = "input-date"
+    value: str = None  # default value
+    format: str = None  # "X" # Date picker value format, please refer to the documentation for more format types
+    inputFormat: str = None  # "YYYY-DD-MM" # Date picker display format, that is, timestamp format, please refer to
+    # the documentation for more format types
+    placeholder: str = None  # "Please select a date" # placeholder text
+    shortcuts: str = None  # date shortcuts
+    minDate: str = None  # Limit the minimum date
+    maxDate: str = None  # limit max date
+    utc: bool = None  # False # save utc value
+    clearable: bool = None  # True # whether it can be cleared
+    embed: bool = None  # False # whether to inline mode
+    timeConstraints: dict = None  # True # Please refer to: react-datetime
+    closeOnSelect: bool = None  # False # whether to close the selection box immediately after clicking the date
+    schedules: Union[list, str] = None  # The schedule is displayed in the calendar, static data can be set or data
+    # can be taken from the context, className refers to the background color
+    scheduleClassNames: List[str] = None  # "['bg-warning','bg-danger','bg-success','bg-info','bg-secondary']"
+    # The color of the event displayed in the calendar, refer to the background color
+    scheduleAction: SchemaNode = None  # Custom schedule display
+    largeMode: bool = None  # False # zoom mode
+
+
+class InputQuarter(InputDate):
+    """InputQuarter"""
+
+    type: str = "input-quarter"
+
+
+class InputQuarterRange(FormItem):
+    """Quarter range"""
+
+    type: str = "input-quarter-range"
+    format: str = None  # Default X, date picker value format
+    inputFormat: str = None  # Default 'YYYY-DD', date picker display format
+    placeholder: str = None  # Default 'Please select a quarterly range', placeholder text
+    minDate: str = None  # Limit the minimum date and time, the usage is the same as the limit range
+    maxDate: str = None  # Limit the maximum date and time, the usage is the same as the limit range
+    minDuration: str = None  # Limit the minimum span, such as: 2quarter
+    maxDuration: str = None  # Limit the maximum span, such as: 4quarter
+    utc: bool = None  # Default False, save UTC value
+    clearable: bool = None  # Default True, Is it clearable
+    embed: bool = None  # Default False, inline mode
+    animation: bool = None  # Default True, Whether to enable cursor animation, needs min amis 2.2.0
+
+
+class Calendar(FormItem):
+    """Calendar"""
+
+    class CalendarItem(AmisNode):
+        startTime: str  # ISO 8601 string
+        endTime: str  # ISO 8601 string
+        content: Union[str, int, dict] = None  # Any, static data or get data from the context
+        className: str = None  # css background
+
+    type: str = "calendar"
+    schedules: Union[List[CalendarItem], str] = None  # List of schedule items
+    scheduleClassNames: List[str] = None  # default ['bg-warning', 'bg-danger', 'bg-success', 'bg-info', 'bg-secondary']
+    # color of the event displayed in the calendar, refer to the background color
+
+    scheduleAction: SchemaNode = None  # custom schedule display
+    largeMode: bool = None  # Default False, zoom mode full size
+    todayActiveStyle: Union[str, dict] = None  # Custom styles when activated today
+
+
+class InputKV(FormItem):
+    """Input key-value pair"""
+
+    type: str = "input-kv"
+    valueType: str = None  # Default "input-text", value item type
+    keyPlaceholder: str = None  # key placeholder information
+    valuePlaceholder: str = None  # value placeholder information
+    draggable: bool = None  # Default True, Whether to drag and drop to sort is allowed
+    defaultValue: Union[str, int, dict] = None  # default ''
+
+
+class InputKVS(FormItem):
+    """Input key-value pair, where value can be a deep structure"""
+
+    type: str = "input-kvs"
+    addButtonText: str = None  # default 'new field', butto text of the add button
+    draggable: bool = None  # Default True, Whether to drag and drop to sort is allowed
+    keyItem: Union[str, SchemaNode] = None  # key field
+    valueItems: List[Union[str, SchemaNode]] = None  # items for the key
+
+
+class InputTimeRange(FormItem):
+    """time limit"""
+
+    type: str = "input-time-range"
+    timeFormat: str = None  # "HH:mm" # Time range selector value format
+    format: str = None  # "HH:mm" # time range selector value format
+    inputFormat: str = None  # "HH:mm" # Time range selector display format
+    placeholder: str = None  # "Please select a time range" # placeholder text
+    clearable: bool = None  # True # whether it can be cleared
+    embed: bool = None  # False # whether to inline mode
+
+
+class InputDatetimeRange(InputTimeRange):
+    """Date time range"""
+
+    type: str = "input-datetime-range"
+    ranges: Union[str, List[str]] = None  # "yesterday,7daysago,prevweek,thismonth,prevmonth,prevquarter" date range
+    # shortcut keys, Optional: today,yesterday,1dayago,7daysago,30daysago,90daysago,prevweek,thismonth,thisquarter,
+    # prevmonth,prevquarter
+    minDate: str = None  # Limit the minimum date and time, the usage is the same as the limit range
+    maxDate: str = None  # Limit the maximum date and time, the usage is the same as the limit range
+    utc: bool = None  # False # save UTC value
+
+
+class InputDateRange(InputDatetimeRange):
+    """Date Range"""
+
+    type: str = "input-date-range"
+    minDuration: str = None  # Limit the minimum span, such as: 2days
+    maxDuration: str = None  # Limit the maximum span, such as: 1year
+
+
+class InputMonthRange(InputDateRange):
+    """month range"""
+
+    type: str = "input-month-range"
+
+
+class Transfer(FormItem):
+    """Shuttle"""
+
+    type: Literal["transfer", "transfer-picker", "tabs-transfer", "tabs-transfer-picker"] = "transfer"
+    options: OptionsNode = None  # option group
+    source: API = None  # Dynamic option group
+    delimiter: str = None  # "False" # splicer
+    joinValues: bool = None  # True # join values
+    extractValue: bool = None  # False # extract value
+    searchable: bool = None  # False When set to true, it means that options can be retrieved by entering partial content.
+    searchApi: API = None  # If you want to retrieve through the interface, you can set an api.
+    statistics: bool = None  # True # whether to display statistics
+    selectTitle: str = None  # "Please select" # Title text on the left
+    resultTitle: str = None  # "current selection" # title text of the result on the right
+    sortable: bool = None  # False # The result can be sorted by drag and drop
+    selectMode: str = None  # "list" # Optional: list, table, tree, chained, associated. They are: list form,
+    # table form, tree selection form, Cascade selection form, association selection form (the difference from
+    # cascading selection is that the cascade is infinite, while the association has only one level, and the left
+    # side of the association can be a tree).
+    searchResultMode: str = None  # If the value of selectMode is not set, it can be configured separately. Refer to
+    # selectMode to determine the display form of search results.
+    columns: List[dict] = None  # When the display form is table, it can be used to configure which columns are
+    # displayed, which is similar to the columns configuration in table, but only has the display function.
+    leftOptions: List[dict] = None  # Used to configure the left option set when the display form is associated.
+    leftMode: str = None  # When the display form is associated, it is used to configure the left selection form,
+    # support list or tree. Default is list.
+    rightMode: str = None  # When the display form is associated, it is used to configure the right selection form,
+    # optional: list, table, tree, chained.
+    menuTpl: SchemaNode = None  # Used to customize option display
+    valueTpl: SchemaNode = None  # Used to customize the display of the value
+
+
+class TransferPicker(Transfer):
+    """Shuttle selector"""
+
+    type: str = "transfer-picker"
+
+
+class TabsTransfer(Transfer):
+    """Combination shuttle"""
+
+    type: str = "tabs-transfer"
+
+
+class TabsTransferPicker(Transfer):
+    """Combination shuttle selector"""
+
+    type: str = "tabs-transfer-picker"
+
+
+class InputTree(FormItem):
+    """Tree selection box"""
+
+    type: str = "input-tree"
+    options: OptionsNode = None  # option group
+    source: API = None  # Dynamic option group
+    autoComplete: API = None  # Automatic prompt completion
+    multiple: bool = None  # False # whether to select multiple
+    delimiter: str = None  # "False" # splicer
+    labelField: str = None  # "label" # option label field
+    valueField: str = None  # "value" # option value field
+    iconField: str = None  # "icon" # icon value field
+    joinValues: bool = None  # True # join values
+    extractValue: bool = None  # False # extract value
+    creatable: bool = None  # False # New option
+    addControls: List[FormItem] = None  # Customize new form items
+    addApi: API = None  # Configure the new option interface
+    editable: bool = None  # False # edit options
+    editControls: List[FormItem] = None  # Customize edit form items
+    editApi: API = None  # Configure editing options interface
+    removable: bool = None  # False # remove option
+    deleteApi: API = None  # Configure delete option interface
+    searchable: bool = None  # False # whether it is searchable, it only takes effect when type is tree-select
+    hideRoot: bool = None  # True # Set to false if you want to show a top-level node
+    rootLabel: bool = None  # "top level" # Useful when hideRoot is not false, used to set the text of the top level node.
+    showIcon: bool = None  # True # whether to show the icon
+    showRadio: bool = None  # False # whether to show radio buttons, multiple is false is valid.
+    initiallyOpen: bool = None  # True # Set whether to expand all levels by default.
+    unfoldedLevel: int = None  # 0 # Set the default unfolded level, which only takes effect when initiallyOpen is
+    # not true.
+    cascade: bool = None  # False # Do not automatically select child nodes when parent node is selected.
+    withChildren: bool = None  # False # When the parent node is selected, the value will contain the value of the
+    # child node, otherwise only the value of the parent node will be retained.
+    onlyChildren: bool = None  # False # For multiple selections, whether to add only its child nodes to the value
+    # when the parent node is selected.
+    rootCreatable: bool = None  # False # whether top-level nodes can be created
+    rootCreateTip: str = None  # "Add a first-level node" # Create a hovering tip for a top-level node
+    minLength: int = None  # Minimum number of selected nodes
+    maxLength: int = None  # Maximum number of nodes selected
+    treeContainerClassName: str = None  # tree outermost container class name
+    enableNodePath: bool = None  # False # whether to enable node path mode
+    pathSeparator: str = None  # "/" # The separator of the node path, it takes effect when enableNodePath is true
+    deferApi: API = None  # For lazy loading options, please configure defer to true, and then configure deferApi to
+    # complete lazy loading
+    selectFirst: bool = None
+    showOutline: bool = None  # False  # 是否显示树层级展开线
+    autoCheckChildren: bool = None  # True  # 当选中父节点时级联选择子节点。
+    onlyLeaf: bool = None  # False  # 只允许选择叶子节点
+    highlightTxt: str = None  # None  # 标签中需要高亮的字符，支持变量
+    itemHeight: int = None  # 32  # 每个选项的高度，用于虚拟渲染
+    virtualThreshold: int = None  # 100  # 在选项数量超过多少时开启虚拟渲染
+    menuTpl: str = None  # 选项自定义渲染 HTML 片段
+    enableDefaultIcon: bool = None  # True  # 是否为选项添加默认的前缀 Icon，父节点默认为folder，叶节点默认为file
+    heightAuto: bool = None  # False  # 默认高度会有个 maxHeight，即超过一定高度就会内部滚动，如果希望自动增长请设置此属性
+
+
+class TreeSelect(InputTree):
+    """Tree selector"""
+
+    type: str = "tree-select"
+    hideNodePathLabel: bool = None  # whether to hide the path label information of the selected node in the selection box
+
+
+class Image(AmisNode):
+    """picture"""
+
+    type: str = "image"  # "image" if used in Table, Card and List; "static-image" if used as static display in Form
+    className: str = None  # Outer CSS class name
+    imageClassName: str = None  # Image CSS class name
+    thumbClassName: str = None  # Thumbnail CSS class name
+    height: int = None  # Image reduction height
+    width: int = None  # Image reduction width
+    title: str = None  # title
+    imageCaption: str = None  # description
+    placeholder: str = None  # placeholder text
+    defaultImage: str = None  # The image displayed when there is no data
+    src: str = None  # Thumbnail address
+    href: Template = None  # External link address
+    originalSrc: str = None  # Original image address
+    enlargeAble: bool = None  # Support zoom in preview
+    enlargeTitle: str = None  # enlarge the title of the preview
+    enlargeCaption: str = None  # Description of the enlarged preview
+    thumbMode: str = None  # "contain" # preview mode, optional: 'w-full','h-full','contain','cover'
+    thumbRatio: str = None  # "1:1" # Preview ratio, optional: '1:1','4:3','16:9'
+    imageMode: str = None  # "thumb" Image display mode, optional: 'thumb', 'original' ie: thumbnail mode or original
+    # image mode
+
+
+class Images(AmisNode):
+    """Photo album"""
+
+    type: str = "images"  # "images" if used in Table, Card and List; "static-images" if used as static display in Form
+    className: str = None  # Outer CSS class name
+    defaultImage: str = None  # Default display image
+    value: Union[str, List[str], List[dict]] = None  # Image array
+    source: str = None  # data source
+    delimiter: str = None  # "," # Delimiter, when value is a string, use this value to separate and split
+    src: str = None  # Preview image address, support data mapping to obtain image variables in the object
+    originalSrc: str = None  # Original image address, support data mapping to obtain image variables in the object
+    enlargeAble: bool = None  # Support zoom in preview
+    thumbMode: str = None  # "contain" # preview mode, optional: 'w-full','h-full','contain','cover'
+    thumbRatio: str = None  # "1:1" # Preview ratio, optional: '1:1','4:3','16:9'
+
+
+class Carousel(AmisNode):
+    """Carousel"""
+
+    class Item(AmisNode):
+        image: str = None  # Image link
+        href: str = None  # Image open URL link
+        imageClassName: str = None  # Image class name
+        title: str = None  # image title
+        titleClassName: str = None  # Image title class name
+        description: str = None  # Picture description
+        descriptionClassName: str = None  # Picture description class name
+        html: str = None  # HTML custom, same as Tpl
+
+    type: str = "carousel"  # Specify as the Carousel renderer
+    className: str = None  # "panel-default" # The class name of the outer Dom
+    options: List[Item] = None  # "[]" # Carousel panel data
+    itemSchema: dict = None  # custom schema to display data
+    auto: bool = True  # whether to rotate automatically
+    interval: str = None  # "5s" # Switch animation interval
+    duration: str = None  # "0.5s" # Switch animation duration
+    width: str = None  # "auto" # width
+    height: str = None  # "200px" # height
+    controls: List[str] = None  # "['dots','arrows']" # Display left and right arrows, bottom dot index
+    controlsTheme: str = None  # "light" # Left and right arrows, bottom dot index color, default light, and dark mode
+    animation: str = None  # "fade" # Switch animation effect, default fade, and slide mode
+    thumbMode: str = None  # "cover"|"contain" # The default zoom mode of the picture
+
+
+class Mapping(AmisNode):
+    """Mapping"""
+
+    type: str = "mapping"  # "mapping" if used in Table, Card and List; "static-mapping" if used as static display in Form
+    className: str = None  # Outer CSS class name
+    placeholder: str = None  # placeholder text
+    map: dict = None  # map configuration
+    source: API = None  # API or data map
+
+
+class CRUD(AmisNode):
+    """Add, delete, modify, check"""
+
+    class Messages(AmisNode):
+        fetchFailed: str = None  # Prompt when fetch fails
+        saveOrderFailed: str = None  # Failed to save order
+        saveOrderSuccess: str = None  # Save order success prompt
+        quickSaveFailed: str = None  # Quick save failure prompt
+        quickSaveSuccess: str = None  # Quick save success prompt
+
+    type: str = "crud"  # type specifies the CRUD renderer
+    mode: str = None  # "table" # "table" , "cards" or "list"
+    title: str = None  # "" # Can be set to empty, when set to empty, there is no title bar
+    className: str = None  # The class name of the outer Dom of the table
+    api: API = None  # The api that CRUD uses to get list data.
+    loadDataOnce: bool = None  # whether to load all data at once (front-end paging)
+    loadDataOnceFetchOnFilter: bool = None  # True # When loadDataOnce is turned on, whether to re-request the api
+    # when filtering
+    source: str = None  # The data mapping interface returns the value of a field. If it is not set, the ${items} or
+    # ${rows} returned by the interface will be used by default. It can also be set to the content of the upper data
+    # source.
+    filter: Union[SchemaNode, Form] = None  # Set the filter, when the form is submitted, it will bring the data to
+    # the current mode refresh list.
+    filterTogglable: bool = None  # False # whether the filter can be displayed or hidden
+    filterDefaultVisible: bool = None  # True # Set whether the filter is visible by default.
+    initFetch: bool = None  # True # whether to pull data during initialization, only for the case with filter,
+    # without filter, data will be pulled initially
+    interval: int = None  # refresh time (minimum 1000)
+    silentPolling: bool = None  # Configure whether to hide the loading animation when refreshing
+    stopAutoRefreshWhen: str = None  # Configure the condition for stopping refresh by expression
+    stopAutoRefreshWhenModalIsOpen: bool = None  # Turn off auto refresh when there is a popup, close the popup and
+    # restore
+    syncLocation: bool = None  # False # whether to synchronize the parameters of the filter conditions to the
+    # address bar, !!! After opening, the data type may be changed, and it cannot pass the fastpi data verification
+    draggable: bool = None  # whether it can be sorted by dragging
+    itemDraggableOn: bool = None  # Use expressions to configure whether drag and drop sorting is possible
+    saveOrderApi: API = None  # Save order api.
+    quickSaveApi: API = None  # API for batch saving after quick editing.
+    quickSaveItemApi: API = None  # API to use when quick edit is configured to save in time.
+    bulkActions: List[Action] = None  # Batch operation list, after configuration, the table can be selected.
+    defaultChecked: bool = None  # When batch operations are available, whether to check all by default.
+    messages: Messages = None  # Override the message prompt, if not specified, the message returned by the api will
+    # be used
+    primaryField: str = None  # Set the ID field name. 'id'
+    perPage: int = None  # Set how many pieces of data are displayed on one page. 10
+    defaultParams: dict = None  # Set the default filter default parameters, which will be sent to the backend
+    # together when querying
+    pageField: str = None  # Set the pagination page number field name. "page"
+    perPageField: str = None  # "perPage" # Set the field name of how many pieces of data are displayed on one page.
+    # Note: Best used with defaultParams, see example below.
+    perPageAvailable: List[int] = None  # [5, 10, 20, 50, 100] # Set how many data drop-down boxes can be displayed
+    # on one page.
+    orderField: str = None  # Set the field name used to determine the position. After setting, the new order will be
+    # assigned to this field.
+    hideQuickSaveBtn: bool = None  # Hide the top quick save prompt
+    autoJumpToTopOnPagerChange: bool = None  # whether to automatically jump to the top when splitting pages.
+    syncResponse2Query: bool = None  # True # Synchronize the returned data to the filter.
+    keepItemSelectionOnPageChange: bool = None  # True
+    # Retain item selection. After the default paging and searching, the user-selected item will be cleared. After
+    # this option is enabled, the user's selection will be retained, enabling cross-page batch operations.
+    labelTpl: str = None  # Single description template, keepItemSelectionOnPageChange
+    # When set to true, all selected items will be listed. This option can be used to customize the entry display copy.
+    headerToolbar: list = None  # ['bulkActions','pagination'] # Top toolbar configuration
+    footerToolbar: list = None  # ['statistics','pagination'] # Bottom toolbar configuration
+    alwaysShowPagination: bool = None  # whether to always show pagination
+    affixHeader: bool = None  # True # whether to fix the header (under table)
+    autoGenerateFilter: bool = None  # whether to open the query area, after it is enabled, the query condition form
+    # will be automatically generated according to the searchable attribute value of the column element
+    itemAction: Action = None  # Implement custom actions after clicking a row, support all configurations in action,
+    # such as pop-up boxes, refresh other components, etc.
+    resizable: bool = None  # 是否可以调整列宽度
+    orderBy: str = None  # 默认排序字段，这个是传给后端，需要后端接口实现
+    orderDir: Literal["asc", "desc"] = None  # 排序方向
+    resetPageAfterAjaxItemAction: bool = None  # False  # 单条数据 ajax 操作后是否重置页码为第一页
+    autoFillHeight: Union[bool, Dict[str, int]] = None  # 内容区域自适应高度
+
+
+class TableColumn(AmisNode):
+    """Column configuration"""
+
+    type: str = None  # Literal['text','audio','image','link','tpl','mapping','carousel','date',
+    # 'progress','status','switch','list','json','operation','tag']
+    label: Template = None  # header text content
+    name: str = None  # Associate data by name
+    tpl: Template = None  # Template
+    fixed: str = None  # whether to fix the current column left|right|none
+    popOver: Union[bool, dict] = None  # popover
+    quickEdit: Union[bool, dict] = None  # quick edit
+    copyable: Union[bool, dict] = None  # whether to copy boolean or {icon: string, content:string}
+    sortable: bool = None  # False # whether it is sortable
+    searchable: Union[bool, SchemaNode] = None  # False # whether to quickly search boolean|Schema
+    width: Union[int, str] = None  # column width
+    remark: RemarkT = None  # prompt message
+    breakpoint: str = None  # *,ls. When there are too many columns, the content cannot be displayed completely,
+    # some information can be displayed at the bottom, and users can expand to view the details
+    filterable: Union[bool, Dict[str, Any]] = None  # filter configuration
+    toggled: bool = None  # whether to expand by default, in the column configuration, you can configure toggled to
+    # false to not display this column by default
+    backgroundScale: int = None  # Can be used to automatically assign color scales based on data control
+
+
+class ColumnOperation(TableColumn):
+    """Action column"""
+
+    type: str = "operation"
+    buttons: List[Union[Action, AmisNode]] = None
+
+
+class ColumnImage(Image, TableColumn):
+    """Picture column"""
+
+    pass
+
+
+class ColumnImages(Images, TableColumn):
+    """Picture collection column"""
+
+    pass
+
+
+class ColumnMapping(Mapping, TableColumn):
+    """Map column"""
+
+    pass
+
+
+class Table(AmisNode):
+    """sheet"""
+
+    type: str = "table"  # Specify as table renderer
+    title: str = None  # title
+    source: str = None  # "${items}" # Data source, bind the current environment variable
+    affixHeader: bool = None  # True # whether to fix the header
+    columnsTogglable: Union[bool, str] = None  # "auto" # Display column display switch, automatic: it is
+    # automatically turned on when the number of columns is greater than or equal to 5
+    placeholder: str = None  # "No data" # Text prompt when there is no data
+    className: str = None  # "panel-default" # Outer CSS class name
+    tableClassName: str = None  # "table-db table-striped" # table CSS class name
+    headerClassName: str = None  # "Action.md-table-header" # Top outer CSS class name
+    footerClassName: str = None  # "Action.md-table-footer" # Bottom outer CSS class name
+    toolbarClassName: str = None  # "Action.md-table-toolbar" # Toolbar CSS class name
+    columns: List[Union[TableColumn, SchemaNode]] = None  # Used to set column information
+    combineNum: int = None  # Automatically combine cells
+    itemActions: List[Action] = None  # Floating row action button group
+    itemCheckableOn: Expression = None  # Configure the condition for whether the current row can be checked, use an
+    # expression
+    itemDraggableOn: Expression = None  # To configure whether the current row can be dragged or not, use an expression
+    checkOnItemClick: bool = None  # False # whether clicking on the data row can check the current row
+    rowClassName: str = None  # Add CSS class name to row
+    rowClassNameExpr: Template = None  # Add CSS class name to row via template
+    prefixRow: list = None  # top summary row
+    affixRow: list = None  # Bottom summary row
+    itemBadge: "Badge" = None  # Row badge configuration
+    autoFillHeight: bool = None  # Content area adaptive height
+    footable: Union[bool, dict] = None  # When there are too many columns, the content cannot be fully displayed.
+    # Some information can be displayed at the bottom, allowing users to expand to view the details. The
+    # configuration is very simple, just turn on the footable attribute, and add a breakpoint attribute to the column
+    # you want to display at the bottom as *.
+    resizable: bool = None  # 列宽度是否支持调整
+    selectable: bool = None  # 支持勾选
+    multiple: bool = None  # 勾选 icon 是否为多选样式checkbox， 默认为radio
+
+
+class Chart(AmisNode):
+    """Chart: https://echarts.apache.org/en/option.html#title"""
+
+    type: str = "chart"  # specify the chart renderer
+    className: str = None  # The class name of the outer Dom
+    body: SchemaNode = None  # Content container
+    api: API = None  # Configuration item interface address
+    source: dict = None  # Get the variable value in the data chain as configuration through data mapping
+    initFetch: bool = None  # whether to request the interface when the component is initialized
+    interval: int = None  # refresh time (minimum 1000)
+    config: Union[dict, str] = None  # Set the configuration item of eschars, when it is string, you can set
+    # configuration items such as function
+    style: dict = None  # Set the style of the root element
+    width: str = None  # Set the width of the root element
+    height: str = None  # Set the height of the root element
+    replaceChartOption: bool = None  # False # Does each update completely overwrite the configuration item or append it?
+    trackExpression: str = None  # Update the chart when the value of this expression changes
+
+
+class Code(AmisNode):
+    """Code highlighting"""
+
+    type: str = "code"
+    className: str = None  # Outer CSS class name
+    value: str = None  # display color value
+    name: str = None  # In other components, when used as variable mapping
+    language: str = None  # The highlighted language used, the default is plaintext
+    tabSize: int = None  # 4 # Default tab size
+    editorTheme: str = None  # "'vs'" # theme, and 'vs-dark'
+    wordWrap: str = None  # "True" # whether to wrap
+
+
+class Json(AmisNode):
+    """JSON display component"""
+
+    type: str = "json"  # "json" if in Table, Card and List; "static-json" if used for static display in Form
+    className: str = None  # Outer CSS class name
+    value: Union[dict, str] = None  # json value, if it is string, it will be parsed automatically
+    source: str = None  # Get the value in the data chain through the data map
+    placeholder: str = None  # placeholder text
+    levelExpand: int = None  # 1 # Default expanded level
+    jsonTheme: str = None  # "twilight" # Theme, optional twilight and eighties
+    mutable: bool = None  # False # whether it can be modified
+    displayDataTypes: bool = None  # False # whether to display data types
+
+
+class Link(AmisNode):
+    """Link"""
+
+    type: str = "link"  # "link" if used in Table, Card and List; "static-link" if used as static display in Form
+    body: str = None  # Text inside the tag
+    href: str = None  # link address
+    blank: bool = None  # whether to open in a new tab
+    htmlTarget: str = None  # The target of the a tag, which takes precedence over the blank attribute
+    title: str = None  # the title of the a tag
+    disabled: bool = None  # disable hyperlinks
+    icon: str = None  # Hyperlink icon to enhance display
+    rightIcon: str = None  # right icon
+
+
+class Log(AmisNode):
+    """Real-time log"""
+
+    type: str = "log"
+    source: API = None  # Support variables, which can be initially set to empty, so that it will not be loaded
+    # initially, and will be loaded when the variable has a value
+    height: int = None  # 500 # Display area height
+    className: str = None  # Outer CSS class name
+    autoScroll: bool = None  # True # whether to scroll automatically
+    placeholder: str = None  # The text being loaded
+    encoding: str = None  # "utf-8" # The character encoding of the returned content
+
+
+class Property(AmisNode):
+    """Property sheet"""
+
+    class Item(AmisNode):
+        label: Template = None  # attribute name
+        content: Template = None  # attribute value
+        span: int = None  # attribute values span several columns
+        visibleOn: Expression = None  # Display expression
+        hiddenOn: Expression = None  # hidden expression
+
+    type: str = "property"
+    className: str = None  # The class name of the outer dom
+    style: dict = None  # The style of the outer dom
+    labelStyle: dict = None  # style of attribute name
+    contentStyle: dict = None  # style of attribute value
+    column: int = None  # 3 # several columns per row
+    mode: str = None  # 'table' # Display mode, currently only 'table' and 'simple'
+    separator: str = None  # ',' # Separator between attribute name and value in 'simple' mode
+    source: Template = None  # data source
+    title: str = None  # title
+    items: List[Item] = None  # data items
+
+
+class QRCode(AmisNode):
+    """QR code"""
+
+    type: str = "qr-code"  # Specify as QRCode renderer
+    value: Template  # The text displayed after scanning the QR code, if you want to display a page, please enter the
+    # full url (starting with "http://..." or "https://..."), templates are supported
+    className: str = None  # The class name of the outer Dom
+    qrcodeClassName: str = None  # QR code SVG class name
+    codeSize: int = None  # 128 # The width and height of the QR code
+    backgroundColor: str = None  # "#fff" # QR code background color
+    foregroundColor: str = None  # "#000" # QR code foreground color
+    level: str = None  # "L" # QR code complexity level, there are four types ('L' 'M' 'Q' 'H')
+
+
+class Barcode(AmisNode):
+    """Barcode"""
+
+    class Options(AmisNode):
+        format: BarcodeEnum = BarcodeEnum.auto  # The format of the barcode
+        width: int = None  # default 2 width of the barcode image
+        height: int = None  # default 100 height of the barcode image
+        displayValue: bool = None  # default True
+        text: str = None
+        fontOptions: str = ""
+        font: str = None  # default "monospace"
+        textAlign: str = None  # default "center"
+        textPosition: str = None  # default "bottom"
+        textMargin: int = None  # default 2
+        fontSize: int = None  # default 20
+        background: str = None  # #ffffff CSS Color
+        lineColor: str = None  # #000000 CSS color
+        margin: int = None  # default 10
+        marginTop: int = None
+        marginBottom: int = None
+        marginLeft: int = None
+        marginRight: int = None
+        flat: bool = None  # default False, no guard bars if True
+
+    type: str = "barcode"  # Specify as QRCode renderer
+    value: str = None  # The value of the barcode
+    className: str = None  # The class name of the outer Dom
+    options: Options = None
+
+
+class Color(AmisNode):
+    type: Literal["color", "static-color"] = "color"
+    value: str = None  # The value of the color CSS code
+    className: str = None  # The class name of the outer Dom
+    defaultColor: str = None  # "#ccc" default color value
+    showValue: bool = None  # default True, whether to display the color value on the right
+
+
+class Progress(AmisNode):
+    type: Literal["progress", "static-progress"] = "progress"
+    mode: ProgressEnum = None  # The type of progress "bar", optional
+    value: Template = None  # The value of the progress
+    className: str = None  # The class name of the outer Dom
+    showLabel: bool = None  # default True, whether to show progress text
+    stripe: bool = None  # default False
+    animate: bool = None  # default False
+    map: Union[str, List[str], List[Dict]] = None  # progress colormap, as dict = {value:number, color:string}
+    # default ['bg-danger', 'bg-warning', 'bg-info', 'bg-success', 'bg-success']
+    threshold: Union[Dict, List] = None  # default -,
+    # {value: template , color?: template } | List[{value: template , color?: template }]
+    showThresholdText: bool = None  # default False, whether to display the threshold (scale) value
+    valueTpl: str = None  # default ${value}%, custom formatted content
+    strokeWidth: int = None  # default 10 by circle, 6 with dashboard
+    gapDegree: int = None  # default 75, angle of the missing corner of the instrument panel, the value can be 0 ~ 295
+    gapPosition: str = None  # default "bottom", Dashboard progress bar notch position, optional top bottom left right
+
+
+class PaginationWrapper(AmisNode):
+    type: str = "pagination-wrapper"
+    showPageInput: bool = None  # default False, whether to display the quick jump input box
+    maxButtons: int = None  # default 5, Maximum number of pagination buttons to display
+    inputName: str = None  # default 'items', input field name
+    outputName: str = None  # default 'items', output field name
+    perPage: int = None  # default 10, Display multiple pieces of data per page
+    position: Literal["top", "none", "bottom"] = "top"  # Pagination display position, if it is configured as none,
+    # you need to configure the pagination component in the content area, otherwise it will not be displayed
+    body: SchemaNode = None  # Display content
+
+
+class Pagination(AmisNode):
+    type: str = "pagination"
+    mode: Literal["simple", "normal"] = "normal"  # The mini version/simple version only displays left and right arrows,
+    # used with hasNext
+    layout: Union[str, List[str]] = None  # default 'pager', Adjust the paging structure layout by controlling
+    # the order of the layout properties
+    maxButtons: int = None  # default 10, Display multiple pieces of data per page
+    lastPage: int = None  # lastPage will be recalculated when the total number of entries is set
+    total: int = None  # total number of pages
+    activePage: int = None  # default 1, current page number
+    perPage: int = None  # default 10, Display multiple pieces of data per page
+    showPerPage: bool = None  # default False, whether to display the perPage switcher layout
+    perPageAvailable: List[int] = None  # default [10, 20, 50, 100], how many lines can be displayed per page
+    showPageInput: bool = None  # default False, whether to display the quick jump input box layout
+    disabled: bool = None  # default False, is pagination disabled
+
+
+class MatrixCheckboxes(FormItem):
+    """Matrix type input box."""
+
+    class RowItem(AmisNode):
+        label: str
+
+    class ColumnItem(AmisNode):
+        label: str
+
+    type: str = "matrix-checkboxes"
+    columns: List[ColumnItem] = None  # list of column items
+    rows: List[RowItem] = None  # list of row items
+    rowLabel: str = None  # row header description
+    source: API = None  # Api address, if the option group is not fixed.
+    multiple: bool = None  # default False, multiple choice
+    singleSelectMode: Literal["false", "cell", "row", "column"] = "column"
+
+
+class Wrapper(AmisNode):
+    type: str = "wrapper"
+    className: str = None  # The class name of the outer Dom
+    style: Union[str, dict] = None  # Custom style (inline style), highest priority
+    body: SchemaNode = None  # Display content
+    size: Union[str, SizeEnum] = None  # Specify the wrapper size, support: xs, sm, md, lg
+
+
+class WebComponent(AmisNode):
+    type: str = "web-component"
+    tag: str = None  # The specific web-component tag used
+    style: Union[str, dict] = None  # Custom style (inline style), highest priority
+    body: SchemaNode = None  # child node
+    props: dict = None  # attributes by their labels
+
+
+class UUIDField(AmisNode):
+    """Randomly generates an id that can be used to prevent repeated form submissions."""
+
+    type: str = "uuid"
+    name: str = None  # The field name
+    length: int = None  # if set, generates short random numbers, if not set it generates a UUID
+
+
+class SearchBox(AmisNode):
+    type: str = "search-box"
+    className: str = None  # The class name of the outer Dom
+    mini: bool = None  # default False, whether it is in mini mode
+    searchImediately: bool = None  # default False, whether to search now
+
+
+class Sparkline(AmisNode):
+    type: str = "sparkline"
+    width: int = None  # width of the sparkline image
+    height: int = None  # height of the sparkline image
+    value: List[Union[int, float]] = None  #
+    clickAction: Action = None  # Action when clicked
+
+
+class Tag(AmisNode):
+    type: str = "tag"
+    className: str = None  # Custom CSS style class name
+    displayMode: Literal["normal", "rounded", "status"] = "normal"  # Display mode
+    closable: bool = None  # default False, show close icon
+    color: str = None  # color theme or custom color value,
+    # 'active' | 'inactive' | 'error' | 'success' | 'processing' | 'warning'
+    label: str = None  # default '-'
+    icon: str = None  # custom font icon
+    style: Union[str, dict] = None  # Custom style (inline style), highest priority
+
+
+class Video(AmisNode):
+    """video"""
+
+    type: str = "video"  # specify the video renderer
+    className: str = None  # The class name of the outer Dom
+    src: str = None  # video address
+    isLive: bool = None  # False # whether it is a live broadcast, it needs to be added when the video is live,
+    # supports flv and hls formats
+    videoType: str = None  # Specify the live video format
+    poster: str = None  # Video cover address
+    muted: bool = None  # whether to mute
+    autoPlay: bool = None  # whether to play automatically
+    rates: List[float] = None  # Multiples in the format [1.0, 1.5, 2.0]
+
+
+class Alert(AmisNode):
+    """hint"""
+
+    type: str = "alert"  # Specify as the alert renderer
+    className: str = None  # The class name of the outer Dom
+    level: str = None  # "info" # Level, can be: info, success, warning or danger
+    body: SchemaNode = None  # Display content
+    showCloseButton: bool = None  # False # whether to show the close button
+    closeButtonClassName: str = None  # CSS class name of the close button
+    showIcon: bool = None  # False # whether to show icon
+    icon: str = None  # custom icon
+    iconClassName: str = None  # CSS class name of icon
+
+
+class Dialog(AmisNode):
+    """Dialog"""
+
+    type: str = "dialog"  # Specify as Dialog renderer
+    title: SchemaNode = None  # Popup layer title
+    body: SchemaNode = None  # Add content to the Dialog content area
+    size: Union[str, SizeEnum] = None  # Specify the dialog size, support: xs, sm, md, lg, xl, full
+    bodyClassName: str = None  # "modal-body" # The style class name of the Dialog body area
+    closeOnEsc: bool = None  # False # whether to support pressing Esc to close Dialog
+    showCloseButton: bool = None  # True # whether to show the close button in the upper right corner
+    showErrorMsg: bool = None  # True # whether to display the error message in the lower left corner of the popup
+    disabled: bool = None  # False # If this property is set, the Dialog is read-only and has no submit operation.
+    actions: List[Action] = None  # If you want to not display the bottom button, you can configure: [] "[Confirm]
+    # and [Cancel]"
+    data: dict = None  # Support data mapping, if not set, it will inherit the data in the context of the trigger
+    # button by default.
+    showLoading: bool = None  # True # 是否在弹框左下角显示 loading 动画
+
+
+class Drawer(AmisNode):
+    """drawer"""
+
+    type: str = "drawer"  # "drawer" specifies the Drawer renderer
+    title: SchemaNode = None  # Popup layer title
+    body: SchemaNode = None  # Add content to the Drawer content area
+    size: Union[str, SizeEnum] = None  # Specify Drawer size, support: xs, sm, md, lg
+    position: str = None  # 'left' # position
+    bodyClassName: str = None  # "modal-body" # The style class name of the Drawer body area
+    closeOnEsc: bool = None  # False # whether to support pressing Esc to close Drawer
+    closeOnOutside: bool = None  # False # whether to close the Drawer when clicking outside the content area
+    overlay: bool = None  # True # whether to display the overlay
+    resizable: bool = None  # False # whether the size of the Drawer can be changed by dragging and dropping
+    actions: List[Action] = None  # Can not be set, there are only two buttons by default. "[Confirm] and [Cancel]"
+    data: dict = None  # Support data mapping, if not set, it will inherit the data in the context of the trigger
+    # button by default.
+    className: str = None  # Drawer 最外层容器的样式类名
+    headerClassName: str = None  # Drawer 头部 区域的样式类名
+    footerClassName: str = None  # Drawer 页脚 区域的样式类名
+    showCloseButton: bool = True  # 是否展示关闭按钮，当值为 false 时，默认开启 closeOnOutside
+    width: Union[int, str] = "500px"  # 容器的宽度，在 position 为 left 或 right 时生效
+    height: Union[int, str] = "500px"  # 容器的高度，在 position 为 top 或 bottom 时生效
+
+
+class Iframe(AmisNode):
+    """Iframe"""
+
+    type: str = "iframe"  # Specify as iFrame renderer
+    className: str = None  # iFrame class name
+    frameBorder: list = None  # frameBorder
+    style: dict = None  # style object
+    src: str = None  # iframe address
+    allow: str = None  # allow configuration
+    sandbox: str = None  # sandbox configuration
+    referrerpolicy: str = None  # referrerpolicy configuration
+    height: Union[int, str] = None  # "100%" # iframe height
+    width: Union[int, str] = None  # "100%" # iframe width
+
+
+class Spinner(AmisNode):
+    """Loading"""
+
+    type: str = "spinner"
+
+
+class TableCRUD(CRUD, Table):
+    """Form Table CRUD"""
+
+    mode: str = "table"
+
+
+class CardCRUD(CRUD, Cards):
+    """Form Card CRUD"""
+
+    mode: str = "cards"
+
+
+class ListCRUD(CRUD, ListDisplay):
+    """Form Card CRUD"""
+
+    mode: str = "list"
+
+
+class Avatar(AmisNode):
+    """avatar"""
+
+    type: str = "avatar"
+    className: str = None  # The class name of the outer dom
+    fit: str = None  # "cover" # Image zoom type
+    src: str = None  # Image address
+    text: str = None  # text
+    icon: str = None  # icon
+    shape: str = None  # "circle" # shape, can also be square
+    size: int = None  # 40 # size
+    style: dict = None  # The style of the outer dom
+
+
+class Audio(AmisNode):
+    """Audio"""
+
+    type: str = "audio"  # specify the audio renderer
+    className: str = None  # The class name of the outer Dom
+    inline: bool = None  # True # whether it is inline mode
+    src: str = None  # audio address
+    loop: bool = None  # False # whether to loop playback
+    autoPlay: bool = None  # False # whether to play automatically
+    rates: List[float] = None  # "[]" # Configurable audio playback speed such as: [1.0, 1.5, 2.0]
+    controls: List[str] = None  # "['rates','play','time','process','volume']" # Internal module customization
+
+
+class Status(AmisNode):
+    """state"""
+
+    type: str = "status"  # Specify as Status renderer
+    className: str = None  # The class name of the outer Dom
+    placeholder: str = None  # placeholder text
+    map: dict = None  # map icon
+    labelMap: dict = None  # map text
+
+
+class Tasks(AmisNode):
+    """Task operation collection"""
+
+    class Item(AmisNode):
+        label: str = None  # task name
+        key: str = None  # Task key value, please distinguish it uniquely
+        remark: str = None  # Current task status, support html
+        status: str = None  # Task status: 0: Initial status, inoperable. 1: Ready, operational state. 2: In
+        # progress, not over yet.
+        # 3: There is an error, no retry. 4: Completed normally. 5: There is an error, and you can try again.
+
+    type: str = "tasks"  # Specify as Tasks renderer
+    className: str = None  # The class name of the outer Dom
+    tableClassName: str = None  # class name of table Dom
+    items: List[Item] = None  # task list
+    checkApi: API = None  # Return the task list, please refer to items for the returned data.
+    submitApi: API = None  # API used for submitting tasks
+    reSubmitApi: API = None  # If the task fails and can be retried, this API will be used when submitting
+    interval: int = None  # 3000 # When there is a task in progress, it will be checked again at regular intervals,
+    # and the time interval is configured through this, the default is 3s.
+    taskNameLabel: str = None  # "task name" # task name column description
+    operationLabel: str = None  # "Operation" # Operation column description
+    statusLabel: str = None  # "status" # description of status column
+    remarkLabel: RemarkT = None  # "Remark" # Remark column description
+    btnText: str = None  # "Online" # Action button text
+    retryBtnText: str = None  # "Retry" # Retry action button text
+    btnClassName: str = None  # "btn-sm btn-default" # Configure the container button className
+    retryBtnClassName: str = None  # "btn-sm btn-danger" # Configure container retry button className
+    statusLabelMap: List[str] = None  # Status display corresponding class name configuration
+    # "["label-warning", "label-info", "label-success", "label-danger", "label-default", "label-danger"]"
+    statusTextMap: List[str] = None  # "["Not started", "Ready", "In progress", "Error", "Completed", "Error"]" #
+    # Status display corresponding text display configuration
+
+
+class Wizard(AmisNode):
+    """Wizard"""
+
+    class Step(AmisNode):
+        title: str = None  # Step title
+        mode: str = None  # Display the default, the same as the mode in Form, choose: normal, horizontal or inline.
+        horizontal: Horizontal = None  # When in horizontal mode, it is used to control the ratio of left and right
+        api: API = None  # The current step saves the interface, which can be left unconfigured.
+        initApi: API = None  # The current step data initialization interface.
+        initFetch: bool = None  # whether the current step data initialization interface is initially fetched.
+        initFetchOn: Expression = None  # whether the current step data initialization interface is initially fetched
+        # is determined by an expression.
+        body: List[FormItem] = None  # The form item collection of the current step, please refer to FormItem.
+
+    type: str = "wizard"  # Specify as Wizard component
+    mode: str = None  # "horizontal" # Display mode, choose: horizontal or vertical
+    api: API = None  # The interface saved in the last step.
+    initApi: API = None  # Initialize data interface
+    initFetch: API = None  # whether to fetch data initially.
+    initFetchOn: Expression = None  # whether to pull data initially, configure by expression
+    actionPrevLabel: str = None  # "Previous" # Previous button text
+    actionNextLabel: str = None  # "Next" # Next button text
+    actionNextSaveLabel: str = None  # "Save and Next" # Save and Next button text
+    actionFinishLabel: str = None  # "Finish" # Finish button text
+    className: str = None  # Outer CSS class name
+    actionClassName: str = None  # "btn-sm btn-default" # Button CSS class name
+    reload: str = None  # Refresh the target object after the operation. Please fill in the name value set by the
+    # target component. If it is filled in window, the current page will be refreshed as a whole.
+    redirect: Template = None  # "3000" # Jump after the operation.
+    target: str = None  # "False" # You can submit data to other components instead of saving it yourself. Please
+    # fill in the name value set by the target component,
+    # If it is filled in as window, the data will be synchronized to the address bar, and the components that depend
+    # on these data will be automatically refreshed.
+    steps: List[Step] = None  # Array, configure step information
+    startStep: int = None  # "1" # Start default value, starting from the first step. Templates can be supported,
+    # but only when the component is created, the template is rendered and the current number of steps is set. When
+    # the component is refreshed later,
+    # The current step will not change according to startStep
+
+
+class AmisRender(AmisNode):
+    """Amis render"""
+
+    type: str = "amis"  # Specify as amis renderer
+    schema_: SchemaNode = Field(None, alias="schema")  # amis schema
+    props: dict = None  # amis props
+
+
+PageSchema.update_forward_refs()
+ActionType.Dialog.update_forward_refs()
+ActionType.Drawer.update_forward_refs()
+TableCRUD.update_forward_refs()
+Form.update_forward_refs()
+Tpl.update_forward_refs()
+InputText.update_forward_refs()
+InputNumber.update_forward_refs()
+Picker.update_forward_refs()
```

### Comparing `fastapi_amis_admin-0.6.3/fastapi_amis_admin/amis/templates/app.html` & `fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/amis/templates/app.html`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,177 +1,177 @@
-<!DOCTYPE html>
-<html lang="">
-<head>
-    <meta charset="UTF-8"/>
-    <title>${site_title}</title>
-    <meta content="text/html; charset=utf-8" http-equiv="Content-Type"/>
-    <meta content="width=device-width, initial-scale=1, maximum-scale=1" name="viewport"/>
-    <meta content="IE=Edge" http-equiv="X-UA-Compatible"/>
-    <link href="${site_icon}" rel="shortcut icon" type="image/x-icon"/>
-    <link href="${cdn}/${pkg}/sdk/sdk.css" rel="stylesheet" title="default"/>
-    <link href="${cdn}/${pkg}/sdk/helper.css" rel="stylesheet"/>
-    <link href="${cdn}/${pkg}/sdk/iconfont.css" rel="stylesheet"/>
-    ${theme_css}
-    <script src="${cdn}/${pkg}/sdk/sdk.js"></script>
-    <script src="${cdn}/vue@2.6.14/dist/vue.js"></script>
-    <script src="${cdn}/history@5.3.0/umd/history.production.min.js"></script>
-    <style>
-        html, body,
-        .app-wrapper {
-            position: relative;
-            width: 100%;
-            height: 100%;
-            margin: 0;
-            padding: 0;
-        }
-
-        /*DropDownButton组件下拉菜单样式修改*/
-        .amis-scope .cxd-DropDown-menu {
-            min-width: 100%;
-            text-align: center;
-        }
-    </style>
-</head>
-<body>
-<div class="app-wrapper" id="root"></div>
-<script>
-    (function () {
-        let amis = amisRequire('amis/embed');
-        const match = amisRequire('path-to-regexp').match;
-
-        // 如果想用 browserHistory 请切换下这处代码, 其他不用变
-        // const history = HistoryLibrary.createBrowserHistory();
-        const history = HistoryLibrary.createHashHistory();
-        const app = ${AmisSchemaJson};
-
-        function normalizeLink(to, location = history.location) {
-            to = to || '';
-
-            if (to && to[0] === '#') {
-                to = location.pathname + location.search + to;
-            } else if (to && to[0] === '?') {
-                to = location.pathname + to;
-            }
-
-            const idx = to.indexOf('?');
-            const idx2 = to.indexOf('#');
-            let pathname = ~idx ? to.substring(0, idx) : ~idx2 ? to.substring(0, idx2) : to;
-            let search = ~idx ? to.substring(idx, ~idx2 ? idx2 : undefined) : '';
-            let hash = ~idx2 ? to.substring(idx2) : location.hash;
-            if (!pathname) {
-                pathname = location.pathname;
-            } else if (pathname[0] != '/' && !/^https?\:\/\//.test(pathname)) {
-                let relativeBase = location.pathname;
-                const paths = relativeBase.split('/');
-                paths.pop();
-                let m;
-                while ((m = /^\.\.?\//.exec(pathname))) {
-                    if (m[0] === '../') {
-                        paths.pop();
-                    }
-                    pathname = pathname.substring(m[0].length);
-                }
-                pathname = paths.concat(pathname).join('/');
-            }
-            return pathname + search + hash;
-        }
-
-        function isCurrentUrl(to, ctx) {
-            if (!to) {
-                return false;
-            }
-            const pathname = history.location.pathname;
-            const link = normalizeLink(to, {
-                ...location,
-                pathname,
-                hash: ''
-            });
-
-            if (!~link.indexOf('http') && ~link.indexOf(':')) {
-                let strict = ctx && ctx.strict;
-                return match(link, {
-                    decode: decodeURIComponent,
-                    strict: typeof strict !== 'undefined' ? strict : true
-                })(pathname);
-            }
-
-            return decodeURI(pathname) === link;
-        }
-
-        let amisInstance = amis.embed(
-            '#root',
-            app,
-            {location: history.location, locale: "${locale}"},
-            {
-                // watchRouteChange: fn => {
-                //   return history.listen(fn);
-                // },
-                updateLocation: (location, replace) => {
-                    location = normalizeLink(location);
-                    if (location === 'goBack') {
-                        return history.goBack();
-                    } else if (
-                        (!/^https?\:\/\//.test(location) &&
-                            location ===
-                            history.location.pathname + history.location.search) ||
-                        location === history.location.href
-                    ) {
-                        // 目标地址和当前地址一样，不处理，免得重复刷新
-                        return;
-                    } else if (/^https?\:\/\//.test(location) || !history) {
-                        return (window.location.href = location);
-                    }
-
-                    history[replace ? 'replace' : 'push'](location);
-                },
-                jumpTo: (to, action) => {
-                    if (to === 'goBack') {
-                        return history.goBack();
-                    }
-
-                    to = normalizeLink(to);
-
-                    if (isCurrentUrl(to)) {
-                        return;
-                    }
-
-                    if (action && action.actionType === 'url') {
-                        action.blank === false
-                            ? (window.location.href = to)
-                            : window.open(to, '_blank');
-                        return;
-                    } else if (action && action.blank) {
-                        window.open(to, '_blank');
-                        return;
-                    }
-
-                    if (/^https?:\/\//.test(to)) {
-                        window.location.href = to;
-                    } else if (
-                        (!/^https?\:\/\//.test(to) &&
-                            to === history.pathname + history.location.search) ||
-                        to === history.location.href
-                    ) {
-                        // do nothing
-                    } else if (location.hash && to.indexOf("?") > -1) {
-                        //如果当前页面有hash，且跳转的页面有参数，将hash拼接到参数后面
-                        const [hash, search] = to.split("?");
-                        window.location.href = location.pathname + "?" + search + "#" + hash;
-                    } else {
-                        history.push(to);
-                    }
-                },
-                isCurrentUrl: isCurrentUrl,
-                theme: "${theme}"
-            }
-        );
-
-        history.listen(state => {
-            amisInstance.updateProps({
-                location: state.location || state,
-                locale: "${locale}"
-            });
-        });
-    })();
-</script>
-</body>
-</html>
+<!DOCTYPE html>
+<html lang="">
+<head>
+    <meta charset="UTF-8"/>
+    <title>${site_title}</title>
+    <meta content="text/html; charset=utf-8" http-equiv="Content-Type"/>
+    <meta content="width=device-width, initial-scale=1, maximum-scale=1" name="viewport"/>
+    <meta content="IE=Edge" http-equiv="X-UA-Compatible"/>
+    <link href="${site_icon}" rel="shortcut icon" type="image/x-icon"/>
+    <link href="${cdn}/${pkg}/sdk/sdk.css" rel="stylesheet" title="default"/>
+    <link href="${cdn}/${pkg}/sdk/helper.css" rel="stylesheet"/>
+    <link href="${cdn}/${pkg}/sdk/iconfont.css" rel="stylesheet"/>
+    ${theme_css}
+    <script src="${cdn}/${pkg}/sdk/sdk.js"></script>
+    <script src="${cdn}/vue@2.6.14/dist/vue.js"></script>
+    <script src="${cdn}/history@5.3.0/umd/history.production.min.js"></script>
+    <style>
+        html, body,
+        .app-wrapper {
+            position: relative;
+            width: 100%;
+            height: 100%;
+            margin: 0;
+            padding: 0;
+        }
+
+        /*DropDownButton组件下拉菜单样式修改*/
+        .amis-scope .cxd-DropDown-menu {
+            min-width: 100%;
+            text-align: center;
+        }
+    </style>
+</head>
+<body>
+<div class="app-wrapper" id="root"></div>
+<script>
+    (function () {
+        let amis = amisRequire('amis/embed');
+        const match = amisRequire('path-to-regexp').match;
+
+        // 如果想用 browserHistory 请切换下这处代码, 其他不用变
+        // const history = HistoryLibrary.createBrowserHistory();
+        const history = HistoryLibrary.createHashHistory();
+        const app = ${AmisSchemaJson};
+
+        function normalizeLink(to, location = history.location) {
+            to = to || '';
+
+            if (to && to[0] === '#') {
+                to = location.pathname + location.search + to;
+            } else if (to && to[0] === '?') {
+                to = location.pathname + to;
+            }
+
+            const idx = to.indexOf('?');
+            const idx2 = to.indexOf('#');
+            let pathname = ~idx ? to.substring(0, idx) : ~idx2 ? to.substring(0, idx2) : to;
+            let search = ~idx ? to.substring(idx, ~idx2 ? idx2 : undefined) : '';
+            let hash = ~idx2 ? to.substring(idx2) : location.hash;
+            if (!pathname) {
+                pathname = location.pathname;
+            } else if (pathname[0] != '/' && !/^https?\:\/\//.test(pathname)) {
+                let relativeBase = location.pathname;
+                const paths = relativeBase.split('/');
+                paths.pop();
+                let m;
+                while ((m = /^\.\.?\//.exec(pathname))) {
+                    if (m[0] === '../') {
+                        paths.pop();
+                    }
+                    pathname = pathname.substring(m[0].length);
+                }
+                pathname = paths.concat(pathname).join('/');
+            }
+            return pathname + search + hash;
+        }
+
+        function isCurrentUrl(to, ctx) {
+            if (!to) {
+                return false;
+            }
+            const pathname = history.location.pathname;
+            const link = normalizeLink(to, {
+                ...location,
+                pathname,
+                hash: ''
+            });
+
+            if (!~link.indexOf('http') && ~link.indexOf(':')) {
+                let strict = ctx && ctx.strict;
+                return match(link, {
+                    decode: decodeURIComponent,
+                    strict: typeof strict !== 'undefined' ? strict : true
+                })(pathname);
+            }
+
+            return decodeURI(pathname) === link;
+        }
+
+        let amisInstance = amis.embed(
+            '#root',
+            app,
+            {location: history.location, locale: "${locale}"},
+            {
+                // watchRouteChange: fn => {
+                //   return history.listen(fn);
+                // },
+                updateLocation: (location, replace) => {
+                    location = normalizeLink(location);
+                    if (location === 'goBack') {
+                        return history.goBack();
+                    } else if (
+                        (!/^https?\:\/\//.test(location) &&
+                            location ===
+                            history.location.pathname + history.location.search) ||
+                        location === history.location.href
+                    ) {
+                        // 目标地址和当前地址一样，不处理，免得重复刷新
+                        return;
+                    } else if (/^https?\:\/\//.test(location) || !history) {
+                        return (window.location.href = location);
+                    }
+
+                    history[replace ? 'replace' : 'push'](location);
+                },
+                jumpTo: (to, action) => {
+                    if (to === 'goBack') {
+                        return history.goBack();
+                    }
+
+                    to = normalizeLink(to);
+
+                    if (isCurrentUrl(to)) {
+                        return;
+                    }
+
+                    if (action && action.actionType === 'url') {
+                        action.blank === false
+                            ? (window.location.href = to)
+                            : window.open(to, '_blank');
+                        return;
+                    } else if (action && action.blank) {
+                        window.open(to, '_blank');
+                        return;
+                    }
+
+                    if (/^https?:\/\//.test(to)) {
+                        window.location.href = to;
+                    } else if (
+                        (!/^https?\:\/\//.test(to) &&
+                            to === history.pathname + history.location.search) ||
+                        to === history.location.href
+                    ) {
+                        // do nothing
+                    } else if (location.hash && to.indexOf("?") > -1) {
+                        //如果当前页面有hash，且跳转的页面有参数，将hash拼接到参数后面
+                        const [hash, search] = to.split("?");
+                        window.location.href = location.pathname + "?" + search + "#" + hash;
+                    } else {
+                        history.push(to);
+                    }
+                },
+                isCurrentUrl: isCurrentUrl,
+                theme: "${theme}"
+            }
+        );
+
+        history.listen(state => {
+            amisInstance.updateProps({
+                location: state.location || state,
+                locale: "${locale}"
+            });
+        });
+    })();
+</script>
+</body>
+</html>
```

### Comparing `fastapi_amis_admin-0.6.3/fastapi_amis_admin/amis/types.py` & `fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/amis/types.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,107 +1,107 @@
-from typing import Any, Dict, List, Union
-
-from fastapi_amis_admin.utils.pydantic import AllowExtraModelMixin
-
-Expression = str
-
-
-OptionsNode = Union[List[Dict[str, Any]], List[str]]
-
-
-class BaseAmisModel(AllowExtraModelMixin):
-    """Base model for amis"""
-
-    def amis_json(self):
-        return self.json(exclude_none=True, by_alias=True)
-
-    def amis_dict(self):
-        return self.dict(exclude_none=True, by_alias=True)
-
-    def update_from_dict(self, kwargs: Dict[str, Any]):
-        for k, v in kwargs.items():
-            setattr(self, k, v)
-        return self
-
-    def update_from_kwargs(self, **kwargs):
-        return self.update_from_dict(kwargs)
-
-
-class BaseAmisApiOut(BaseAmisModel):
-    """api interface output data format"""
-
-    status: int = 0
-    msg: str = ""
-    data: dict = None
-
-
-class AmisNode(BaseAmisModel):
-    """Component configuration"""
-
-    type: str = None  # component type
-    visible: bool = None  # show
-    hidden: bool = None  # hide
-    visibleOn: Expression = None  # conditional display
-    hiddenOn: Expression = None  # conditional display
-    id: str = None
-    name: str = None  # In other components, when used as a variable map
-    value: Any = None  # The value of the component
-    onEvent: dict = None
-    events: Dict[str, Any] = None  # Specifies the amis behavior triggered by the component
-
-
-SchemaNode = Union[str, AmisNode, List[AmisNode], Dict[str, Any], List[Dict[str, Any]]]
-
-
-class AmisAPI(BaseAmisModel):
-    url: str  # Current interface API address
-    method: str = None  # 'GET' # Request method: get, post, put, delete
-    data: Union[str, dict] = None  # The requested data body, supports data mapping
-    dataType: str = None  # The default is json and can be configured as form or form-data.
-    # When data contains files, it will automatically use form-data (multipart/form-data) format.
-    # When configured as form, the format is application/x-www-form-urlencoded.
-    qsOptions: Union[str, dict] = None  # Useful when dataType is form or form-data.
-    # For specific parameters, please refer to here, the default setting is: { arrayFormat: 'indices',
-    # encodeValuesOnly: true }
-    headers: Dict[str, Any] = None  # Request header information
-    sendOn: Expression = None  # Configure request conditions
-    cache: int = None  # Set cache to set the cache time, the unit is milliseconds. During the set cache time,
-    # the same request will not be repeated, but the cached request response data will be obtained.
-    requestAdaptor: str = None  # Send adapter, API configuration of amis, if you can't configure the request
-    # structure you want, you can configure the requestAdaptor send adapter
-    responseData: Dict[str, Any] = None  # If the data structure returned by the interface is not as expected, it can
-    # be modified by configuring responseData, which also supports data mapping. The data that can be used for
-    # mapping is the actual data of the interface (the data part returned by the interface), plus the api variable.
-    # Among them, api.query is the query parameter sent by the interface, and api.body is the original data of the
-    # content body sent by the interface.
-    replaceData: bool = None  # Whether the returned data replaces the current data, the default is false, that is:
-    # append, set to true to completely replace.
-    adaptor: str = None  # Receive adapter, if the interface return does not meet the requirements, you can configure
-    # an adapter to handle it as required by amis.  Also supports Function or string function body format
-    responseType: str = None  # Return type, if it is a download, it needs to be set to 'blob'
-    autoRefresh: bool = None  # Configure whether to automatically refresh the interface.
-    trackExpression: str = None  # Configure the tracking variable expression. When automatic refresh is enabled,
-    # the default is the url of the api to automatically track variable changes. If you want to monitor variables
-    # outside the url, configure traceExpression.
-
-
-API = Union[str, AmisAPI, dict]
-
-
-class Tpl(AmisNode):
-    type: str = "tpl"  # Specify as Tpl component
-    tpl: str  # configuration template
-    className: str = None  # The class name of the outer Dom
-
-
-Template = Union[str, Tpl]
-
-
-class Event(BaseAmisModel):
-    actionType: str = None  # Action name
-    args: dict = None  # Action parameter {key:value}, support data mapping
-    preventDefault: Union[bool, Expression] = None  # "False" # Prevent event default behavior, > 1.10.0 and above
-    # support expressions
-    stopPropagation: Union[bool, Expression] = None  # "False" # Stop subsequent action execution, > 1.10.0 and above
-    # supports expressions
-    expression: Union[bool, Expression] = None  # Execution condition, not set means default execution
-    outputVar: str = None  # output data variable name
+from typing import Any, Dict, List, Union
+
+from fastapi_amis_admin.utils.pydantic import AllowExtraModelMixin
+
+Expression = str
+
+
+OptionsNode = Union[List[Dict[str, Any]], List[str]]
+
+
+class BaseAmisModel(AllowExtraModelMixin):
+    """Base model for amis"""
+
+    def amis_json(self):
+        return self.json(exclude_none=True, by_alias=True)
+
+    def amis_dict(self):
+        return self.dict(exclude_none=True, by_alias=True)
+
+    def update_from_dict(self, kwargs: Dict[str, Any]):
+        for k, v in kwargs.items():
+            setattr(self, k, v)
+        return self
+
+    def update_from_kwargs(self, **kwargs):
+        return self.update_from_dict(kwargs)
+
+
+class BaseAmisApiOut(BaseAmisModel):
+    """api interface output data format"""
+
+    status: int = 0
+    msg: str = ""
+    data: dict = None
+
+
+class AmisNode(BaseAmisModel):
+    """Component configuration"""
+
+    type: str = None  # component type
+    visible: bool = None  # show
+    hidden: bool = None  # hide
+    visibleOn: Expression = None  # conditional display
+    hiddenOn: Expression = None  # conditional display
+    id: str = None
+    name: str = None  # In other components, when used as a variable map
+    value: Any = None  # The value of the component
+    onEvent: dict = None
+    events: Dict[str, Any] = None  # Specifies the amis behavior triggered by the component
+
+
+SchemaNode = Union[str, AmisNode, List[AmisNode], Dict[str, Any], List[Dict[str, Any]]]
+
+
+class AmisAPI(BaseAmisModel):
+    url: str  # Current interface API address
+    method: str = None  # 'GET' # Request method: get, post, put, delete
+    data: Union[str, dict] = None  # The requested data body, supports data mapping
+    dataType: str = None  # The default is json and can be configured as form or form-data.
+    # When data contains files, it will automatically use form-data (multipart/form-data) format.
+    # When configured as form, the format is application/x-www-form-urlencoded.
+    qsOptions: Union[str, dict] = None  # Useful when dataType is form or form-data.
+    # For specific parameters, please refer to here, the default setting is: { arrayFormat: 'indices',
+    # encodeValuesOnly: true }
+    headers: Dict[str, Any] = None  # Request header information
+    sendOn: Expression = None  # Configure request conditions
+    cache: int = None  # Set cache to set the cache time, the unit is milliseconds. During the set cache time,
+    # the same request will not be repeated, but the cached request response data will be obtained.
+    requestAdaptor: str = None  # Send adapter, API configuration of amis, if you can't configure the request
+    # structure you want, you can configure the requestAdaptor send adapter
+    responseData: Dict[str, Any] = None  # If the data structure returned by the interface is not as expected, it can
+    # be modified by configuring responseData, which also supports data mapping. The data that can be used for
+    # mapping is the actual data of the interface (the data part returned by the interface), plus the api variable.
+    # Among them, api.query is the query parameter sent by the interface, and api.body is the original data of the
+    # content body sent by the interface.
+    replaceData: bool = None  # Whether the returned data replaces the current data, the default is false, that is:
+    # append, set to true to completely replace.
+    adaptor: str = None  # Receive adapter, if the interface return does not meet the requirements, you can configure
+    # an adapter to handle it as required by amis.  Also supports Function or string function body format
+    responseType: str = None  # Return type, if it is a download, it needs to be set to 'blob'
+    autoRefresh: bool = None  # Configure whether to automatically refresh the interface.
+    trackExpression: str = None  # Configure the tracking variable expression. When automatic refresh is enabled,
+    # the default is the url of the api to automatically track variable changes. If you want to monitor variables
+    # outside the url, configure traceExpression.
+
+
+API = Union[str, AmisAPI, dict]
+
+
+class Tpl(AmisNode):
+    type: str = "tpl"  # Specify as Tpl component
+    tpl: str  # configuration template
+    className: str = None  # The class name of the outer Dom
+
+
+Template = Union[str, Tpl]
+
+
+class Event(BaseAmisModel):
+    actionType: str = None  # Action name
+    args: dict = None  # Action parameter {key:value}, support data mapping
+    preventDefault: Union[bool, Expression] = None  # "False" # Prevent event default behavior, > 1.10.0 and above
+    # support expressions
+    stopPropagation: Union[bool, Expression] = None  # "False" # Stop subsequent action execution, > 1.10.0 and above
+    # supports expressions
+    expression: Union[bool, Expression] = None  # Execution condition, not set means default execution
+    outputVar: str = None  # output data variable name
```

### Comparing `fastapi_amis_admin-0.6.3/fastapi_amis_admin/crud/_sqlalchemy.py` & `fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/crud/_sqlalchemy.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,589 +1,589 @@
-import re
-from enum import Enum
-from typing import (
-    Any,
-    Callable,
-    Dict,
-    Generic,
-    Iterable,
-    List,
-    Optional,
-    Pattern,
-    Tuple,
-    Type,
-    Union,
-)
-
-from fastapi import APIRouter, Body, Depends
-from fastapi._compat import field_annotation_is_scalar
-from fastapi.types import IncEx
-from sqlalchemy import Column, Table, func
-from sqlalchemy.engine import Result
-from sqlalchemy.future import select
-from sqlalchemy.orm import InstrumentedAttribute, Session, object_session
-from sqlalchemy.sql import Select
-from sqlalchemy.sql.elements import BinaryExpression, Label, UnaryExpression
-from starlette.requests import Request
-from typing_extensions import Annotated, Literal
-
-from fastapi_amis_admin.utils.pydantic import (
-    PYDANTIC_V2,
-    ModelField,
-    ValueItems,
-    annotation_outer_type,
-    create_model_by_fields,
-    field_allow_none,
-    model_fields,
-)
-
-try:
-    from functools import cached_property
-except ImportError:
-    from sqlalchemy.util.langhelpers import memoized_property as cached_property
-
-from .base import (
-    BaseCrud,
-    SchemaCreateT,
-    SchemaFilterT,
-    SchemaListT,
-    SchemaModelT,
-    SchemaReadT,
-    SchemaUpdateT,
-)
-from .parser import (
-    SqlaField,
-    SqlaInsAttr,
-    SqlaPropertyField,
-    TableModelParser,
-    TableModelT,
-    get_modelfield_by_alias,
-    get_python_type_parse,
-    parse_obj_to_schema,
-)
-from .schema import BaseApiOut, ItemListSchema
-from .utils import (
-    IdStrQuery,
-    ItemIdListDepend,
-    SqlalchemyDatabase,
-    get_engine_db,
-    parser_str_set_list,
-)
-
-sql_operator_pattern: Pattern = re.compile(r"^\[(=|<=|<|>|>=|!|!=|<>|\*|!\*|~|!~|-)]")
-sql_operator_map: Dict[str, str] = {
-    "=": "__eq__",
-    "<=": "__le__",
-    "<": "__lt__",
-    ">": "__gt__",
-    ">=": "__ge__",
-    "!": "__ne__",
-    "!=": "__ne__",
-    "<>": "__ne__",
-    "*": "in_",
-    "!*": "not_in",
-    "~": "like",
-    "!~": "not_like",
-    "-": "between",
-}
-
-
-class SqlalchemySelector(Generic[TableModelT]):
-    model: Type[TableModelT] = None  # SQLModel,DeclarativeMeta,InspectTable
-    fields: List[SqlaField] = []  # Need to query the field from the database
-    list_filter: List[SqlaField] = []  # Query filterable fields
-    exclude: List[SqlaInsAttr] = []  # Model fields that do not need to be queried. It is not recommended to use.
-    ordering: List[Union[SqlaField, UnaryExpression]] = []  # Default sort field
-    link_models: Dict[str, Tuple[Type[Table], Column, Column]] = None  # Link table information
-    """Relate information of the target model with the current model.
-    - The Data structure is: {Target table name: (link model table,
-        Column in the link model table associated with the current model,
-        Column in the link model table associated with the target model)}
-    - E.g. the current model is Role, you can add the target model User through `User.roles` here.
-        And then you can query the Role through the primary key field of the target model User.
-    - Saved information: {auth_user: (auth_user_roles, auth_user_roles.role_id, auth_user_roles.user_id)}
-    - You can add the query parameters to the route url to access the role list of the user:
-        `?link_model=auth_user&link_item_id={user_id}`.
-    """
-    pk_name: str = "id"  # Primary key name
-
-    def __init__(self, model: Type[TableModelT] = None, fields: List[SqlaField] = None) -> None:
-        self.model = model or self.model
-        assert self.model, "model is None"
-        assert hasattr(self.model, "__table__"), "model must be has __table__ attribute."
-        self.pk_name: str = self.pk_name or self.model.__table__.primary_key.columns.keys()[0]
-        self.pk: InstrumentedAttribute = self.model.__dict__[self.pk_name]
-        self.parser = TableModelParser(self.model)
-        fields = fields or self.fields or self.model_insfields
-        exclude = self.parser.filter_insfield(self.exclude)
-        self.fields = [
-            sqlfield
-            for sqlfield in self.parser.filter_insfield(fields + [self.pk], save_class=(Label,))
-            if sqlfield not in exclude
-        ]
-        assert self.fields, "fields is None"
-        self.list_filter = self.list_filter and self.list_filter.copy() or self.fields
-        self.link_models = self.link_models or {}
-        """Make sure the value of link_models is an object attribute, not a class attribute."""
-
-    @cached_property
-    def model_insfields(self) -> List[SqlaInsAttr]:
-        return self.parser.filter_insfield(self.model.__dict__.values())
-
-    @cached_property
-    def _select_entities(self) -> Dict[str, Union[InstrumentedAttribute, Label]]:
-        return {self.parser.get_alias(insfield): insfield for insfield in self.fields}
-
-    @cached_property
-    def _filter_entities(self) -> Dict[str, Union[InstrumentedAttribute, Label]]:
-        return {
-            self.parser.get_alias(sqlfield): sqlfield
-            for sqlfield in self.parser.filter_insfield(self.list_filter, save_class=(Label,))
-        }
-
-    async def get_select(self, request: Request) -> Select:
-        return select(*self._select_entities.values())
-
-    def _calc_ordering(self, orderBy, orderDir):
-        sqlfield = self._select_entities.get(orderBy, self._filter_entities.get(orderBy))
-        order = None
-        if sqlfield is not None:
-            order = sqlfield.desc() if orderDir == "desc" else sqlfield.asc()
-            return [order]
-        elif self.ordering is not None:
-            order = self.parser.filter_insfield(
-                self.ordering,
-                save_class=(
-                    UnaryExpression,
-                    Label,
-                ),
-            )
-        return order
-
-    @property
-    def _select_maker(self):
-        if self.link_models:
-
-            def select_maker(
-                sel: Annotated[Select, Depends(self.get_select)],  # type: ignore
-                link_clause: Annotated[Optional[Any], Depends(self.get_link_clause)] = None,  # type: ignore
-            ) -> Select:
-                if link_clause is not None:
-                    sel = sel.where(link_clause)
-                return sel
-
-        else:
-            select_maker = self.get_select
-        return select_maker
-
-    async def get_link_clause(
-        self,
-        request: Request,
-        link_model: str = None,
-        link_item_id: IdStrQuery = None,
-        op: Literal["in_", "not_in", None] = None,
-    ) -> Optional[Any]:
-        if link_model and link_item_id:
-            result = self.link_models.get(link_model)
-            if not result:
-                return None
-            table, pk_col, link_col = result
-            if table is not None:
-                link_item_id = list(
-                    map(
-                        get_python_type_parse(link_col),
-                        parser_str_set_list(link_item_id),
-                    )
-                )
-                if op == "not_in":
-                    return self.pk.not_in(select(pk_col).where(link_col.in_(link_item_id)))
-                else:
-                    return self.pk.in_(select(pk_col).where(link_col.in_(link_item_id)))
-        return None
-
-    @staticmethod
-    def _parser_query_value(
-        value: Any, operator: str = "__eq__", python_type_parse: Callable = str
-    ) -> Tuple[Optional[str], Union[tuple, None]]:
-        if isinstance(value, str):
-            if not value:
-                return None, None
-            match = sql_operator_pattern.match(value)
-            if match:
-                op_key = match.group(1)
-                operator = sql_operator_map.get(op_key)
-                value = value.replace(f"[{op_key}]", "")
-                if not value:
-                    return None, None
-                if operator in ["like", "not_like"] and value.find("%") == -1:
-                    return operator, (f"%{value}%",)
-                elif operator in ["in_", "not_in"]:
-                    return operator, (list(map(python_type_parse, set(value.split(",")))),)
-                elif operator == "between":
-                    value = value.split(",")[:2]
-                    if len(value) < 2:
-                        return None, None
-                    return operator, tuple(map(python_type_parse, value))
-        return operator, (python_type_parse(value),)
-
-    def calc_filter_clause(self, data: Dict[str, Any]) -> List[BinaryExpression]:
-        lst = []
-        for k, v in data.items():
-            sqlfield = self._filter_entities.get(k)
-            if sqlfield is not None:
-                operator, val = self._parser_query_value(v, python_type_parse=get_python_type_parse(sqlfield))
-                if operator:
-                    lst.append(getattr(sqlfield, operator)(*val))
-        return lst
-
-
-class SqlalchemyCrud(
-    BaseCrud[SchemaModelT, SchemaListT, SchemaFilterT, SchemaCreateT, SchemaReadT, SchemaUpdateT], SqlalchemySelector[TableModelT]
-):
-    engine: SqlalchemyDatabase = None  # sqlalchemy engine
-    create_fields: List[SqlaInsAttr] = []  # Create item data field
-    create_exclude: Optional[IncEx] = None
-    """create exclude fields, such as: {'id', 'key', 'name'} or {'id': True, 'category': {'id', 'name'}}."""
-    update_fields: List[SqlaPropertyField] = []
-    """model update fields;support model property and relationship field."""
-    update_exclude: Optional[IncEx] = None
-    """update exclude fields, such as: {'id', 'key', 'name'} or {'id': True, 'category': {'id', 'name'}}."""
-    read_fields: List[SqlaPropertyField] = []
-    """Model read fields; used in route_read, note the difference between readonly_fields and read_fields.
-    default is None, means not use read route."""
-
-    def __init__(
-        self,
-        model: Type[TableModelT],
-        engine: SqlalchemyDatabase,
-        fields: List[SqlaField] = None,
-        router: APIRouter = None,
-    ) -> None:
-        self.engine = engine or self.engine
-        assert self.engine, "engine is None"
-        self.db = get_engine_db(self.engine)
-        SqlalchemySelector.__init__(self, model, fields)
-        schema_model: Type[SchemaModelT] = self.schema_model or TableModelParser.get_table_model_schema(model)
-        BaseCrud.__init__(self, schema_model, router)
-        # if self.readonly_fields:
-        #     logging.warning(
-        #         "readonly fields, deprecated, not recommended, will be removed in version 0.4.0."
-        #         "Please replace them with update_fields and update_exclude."
-        #     )
-
-    @property
-    def router_prefix(self):
-        return f"/{self.model.__name__}"
-
-    def _create_schema_list(self) -> Type[SchemaListT]:
-        # Get the model fields from the select entities
-        modelfields = self.parser.filter_modelfield(
-            self._select_entities.values(),
-            save_class=(
-                Label,
-                ModelField,
-            ),
-        )
-        # Create the schema using the model fields
-        return create_model_by_fields(
-            name=f"{self.schema_name_prefix}List",
-            fields=modelfields,
-            set_none=True,
-            extra="allow",
-        )
-
-    def _create_schema_filter(self) -> Type[SchemaFilterT]:
-        # Get the filter fields from the list filter or select entities
-        list_filter = self.list_filter or self._select_entities.values()
-        # Filter out the model fields from the filter fields
-        modelfields = self.parser.filter_modelfield(list_filter, save_class=(Label,))
-        # Modify the modelfields if necessary
-        for modelfield in modelfields:
-            type_ = annotation_outer_type(modelfield.type_)
-            if field_annotation_is_scalar(modelfield.type_) and issubclass(type_, (Enum, bool, str)):
-                continue
-            if PYDANTIC_V2:
-                modelfield.field_info.annotation = str
-            else:
-                modelfield.type_ = str
-                modelfield.outer_type_ = str
-                modelfield.validators = []
-        # Create the schema using the model fields
-        return create_model_by_fields(
-            name=f"{self.schema_name_prefix}Filter",
-            fields=modelfields,
-            set_none=True,
-        )
-
-    def _create_schema_read(self) -> Optional[Type[SchemaReadT]]:
-        if not self.read_fields:
-            return None
-        # Filter out any non-model fields from the read fields
-        modelfields = self.parser.filter_modelfield(self.read_fields)
-        # Create the schema using the model fields
-        return create_model_by_fields(
-            name=f"{self.schema_name_prefix}Read",
-            fields=modelfields,
-            orm_mode=True,
-        )
-
-    def _create_schema_update(self) -> Type[SchemaUpdateT]:
-        # Set the update fields to the model insfields if not provided
-        self.update_fields = self.update_fields or self.model_insfields
-        # Exclude certain fields if specified
-        exclude = {k for k, v in ValueItems.merge(self.update_exclude, {}).items() if not isinstance(v, (dict, list, set))} or {
-            self.pk_name
-        }
-        # Filter out any non-model fields from the update fields
-        modelfields = self.parser.filter_modelfield(self.update_fields, exclude=exclude)
-        # Create the schema using the model fields
-        return create_model_by_fields(
-            name=f"{self.schema_name_prefix}Update",
-            fields=modelfields,
-            set_none=True,
-        )
-
-    def _create_schema_create(self) -> Type[SchemaCreateT]:
-        # Set the create fields to the model insfields if not provided
-        self.create_fields = self.create_fields or self.model_insfields
-        # Exclude certain fields if specified
-        exclude = {k for k, v in ValueItems.merge(self.create_exclude, {}).items() if not isinstance(v, (dict, list, set))} or {
-            self.pk_name
-        }
-        # Filter out any non-model fields from the create fields
-        modelfields = self.parser.filter_modelfield(self.create_fields, exclude=exclude)
-        # Create the schema using the model fields
-        return create_model_by_fields(
-            name=f"{self.schema_name_prefix}Create",
-            fields=modelfields,
-        )
-
-    def create_item(self, item: Dict[str, Any]) -> TableModelT:
-        """Create a database orm object through a dictionary."""
-        return self.model(**item)
-
-    def read_item(self, obj: TableModelT) -> SchemaReadT:
-        """read database data and parse to schema_read"""
-        return parse_obj_to_schema(obj, self.schema_read)
-
-    def update_item(self, obj: TableModelT, values: Dict[str, Any]) -> None:
-        """update schema_update data to database,support relational attributes"""
-        for k, v in values.items():
-            field = get_modelfield_by_alias(self.model, k)
-            if not field and not hasattr(obj, k):
-                continue
-            name = field.name if field else k
-            if isinstance(v, dict):
-                # Relational attributes, nested;such as: setattr(article.content, "body", "new body")
-                sub = getattr(obj, name)
-                if not isinstance(sub, dict):  # Ensure that the attribute is an object.
-                    self.update_item(sub, v)
-                    continue
-            setattr(obj, name, v)
-
-    def delete_item(self, obj: TableModelT) -> None:
-        """delete database data"""
-        object_session(obj).delete(obj)
-
-    def list_item(self, values: Dict[str, Any]) -> SchemaListT:
-        """Parse the database data query result dictionary into schema_list."""
-        return self.schema_list.parse_obj(values)
-
-    def _fetch_item_scalars(self, session: Session, item_id: Iterable[str]) -> List[TableModelT]:
-        sel = select(self.model).where(self.pk.in_(list(map(get_python_type_parse(self.pk), item_id))))
-        return session.scalars(sel).all()
-
-    async def fetch_items(self, *item_id: str) -> List[TableModelT]:
-        """Fetch the database data by id."""
-        return await self.db.async_run_sync(self._fetch_item_scalars, item_id)
-
-    def _create_items(self, session: Session, items: List[Dict[str, Any]]) -> List[TableModelT]:
-        if not items:
-            return []
-        objs = [self.create_item(item) for item in items]
-        session.add_all(objs)
-        session.flush()
-        return objs
-
-    async def create_items(self, request: Request, items: List[SchemaCreateT]) -> List[TableModelT]:
-        """Create multiple database data."""
-        items = [await self.on_create_pre(request, obj) for obj in items]
-        return await self.db.async_run_sync(self._create_items, items)
-
-    def _read_items(self, session: Session, item_id: List[str]) -> List[SchemaReadT]:
-        items = self._fetch_item_scalars(session, item_id)
-        return [self.read_item(obj) for obj in items]
-
-    async def read_items(self, request: Request, item_id: List[str]) -> List[SchemaReadT]:
-        """Fetch the database data by id."""
-        return await self.db.async_run_sync(self._read_items, item_id)
-
-    def _update_items(self, session: Session, item_id: List[str], values: Dict[str, Any]) -> List[TableModelT]:
-        items = self._fetch_item_scalars(session, item_id)
-        for item in items:
-            self.update_item(item, values)
-        return items
-
-    async def update_items(self, request: Request, item_id: List[str], values: Dict[str, Any]) -> List[TableModelT]:
-        """Update the database data by id."""
-        return await self.db.async_run_sync(self._update_items, item_id, values)
-
-    def _delete_items(self, session: Session, item_id: List[str]) -> List[TableModelT]:
-        items = self._fetch_item_scalars(session, item_id)
-        for item in items:
-            self.delete_item(item)
-        return items
-
-    async def delete_items(self, request: Request, item_id: List[str]) -> List[TableModelT]:
-        """Delete the database data by id."""
-        return await self.db.async_run_sync(self._delete_items, item_id)
-
-    @property
-    def schema_name_prefix(self):
-        if self.__class__ is SqlalchemyCrud:
-            return self.model.__name__
-        return super().schema_name_prefix
-
-    async def on_create_pre(self, request: Request, obj: SchemaCreateT, **kwargs) -> Dict[str, Any]:
-        data = obj.dict(by_alias=True)  # exclude=set(self.pk)
-        if self.pk_name in data and not data.get(self.pk_name):
-            del data[self.pk_name]
-        return data
-
-    async def on_update_pre(
-        self,
-        request: Request,
-        obj: SchemaUpdateT,
-        item_id: Union[List[str], List[int]],
-        **kwargs,
-    ) -> Dict[str, Any]:
-        data = obj.dict(exclude=self.update_exclude, exclude_unset=True, by_alias=True)
-        data = {key: val for key, val in data.items() if val is not None or field_allow_none(model_fields(self.model)[key])}
-        return data
-
-    async def on_filter_pre(self, request: Request, obj: Optional[SchemaFilterT], **kwargs) -> Dict[str, Any]:
-        return obj and {k: v for k, v in obj.dict(exclude_unset=True, by_alias=True).items() if v is not None}
-
-    async def on_list_after(self, request: Request, result: Result, data: ItemListSchema, **kwargs) -> ItemListSchema:
-        """Parse the database data query result dictionary into schema_list."""
-        data.items = self.parser.conv_row_to_dict(result.all())
-        data.items = [self.list_item(item) for item in data.items]
-        return data
-
-    @property
-    def AnnotatedSelect(self):
-        """Annotated Select, used to automatically perform fastapi dependency injection"""
-        return Annotated[Select, Depends(self._select_maker)]
-
-    @property
-    def AnnotatedItemIdList(self):
-        """Annotated Item ID List, used to filter the id of the data that the user has permission to operate on.
-        And automatically perform fastapi dependency injection
-        """
-        return Annotated[List[str], Depends(self.filtered_item_id)]
-
-    @property
-    def filtered_item_id(self) -> Callable:
-        """Filter the id of the data that the user has permission to operate on."""
-
-        async def depend(
-            item_id: ItemIdListDepend,
-            sel: self.AnnotatedSelect,  # type: ignore
-        ):
-            item_id = list(map(get_python_type_parse(self.pk), item_id))
-            filtered_id = await self.db.async_scalars(sel.where(self.pk.in_(item_id)).with_only_columns(self.pk))
-            return filtered_id.all()
-
-        return depend
-
-    @property
-    def route_list(self) -> Callable:
-        async def route(
-            request: Request,
-            sel: self.AnnotatedSelect,  # type: ignore
-            paginator: Annotated[self.paginator, Depends()],  # type: ignore
-            filters: Annotated[self.schema_filter, Body()] = None,  # type: ignore
-        ):
-            if not await self.has_list_permission(request, paginator, filters):
-                return self.error_no_router_permission(request)
-            data = ItemListSchema(items=[])
-            data.query = request.query_params
-            if await self.has_filter_permission(request, filters):
-                data.filters = await self.on_filter_pre(request, filters)
-                if data.filters:
-                    sel = sel.filter(*self.calc_filter_clause(data.filters))
-            if paginator.show_total:
-                data.total = await self.db.async_scalar(
-                    select(func.count("*")).select_from(sel.with_only_columns(self.pk).subquery())
-                )
-            orderBy = self._calc_ordering(paginator.orderBy, paginator.orderDir)
-            if orderBy:
-                sel = sel.order_by(*orderBy)
-            sel = sel.limit(paginator.perPage).offset((paginator.page - 1) * paginator.perPage)
-            result = await self.db.async_execute(sel)
-            return BaseApiOut(data=await self.on_list_after(request, result, data))
-
-        return route
-
-    @property
-    def route_create(self) -> Callable:
-        async def route(
-            request: Request,
-            data: Annotated[Union[List[self.schema_create], self.schema_create], Body()],  # type: ignore
-        ) -> BaseApiOut[Union[int, self.schema_model]]:  # type: ignore
-            if not await self.has_create_permission(request, data):
-                return self.error_no_router_permission(request)
-            if not isinstance(data, list):
-                data = [data]
-            try:
-                items = await self.create_items(request, data)
-            except Exception as error:
-                return self.error_execute_sql(request=request, error=error)
-            result = len(items)
-            if result == 1:  # if only one item, return the first item
-                result = await self.db.async_run_sync(lambda _: parse_obj_to_schema(items[0], self.schema_model, refresh=True))
-            return BaseApiOut(data=result)
-
-        return route
-
-    @property
-    def route_read(self) -> Callable:
-        async def route(
-            request: Request,
-            item_id: self.AnnotatedItemIdList,  # type: ignore
-        ):
-            if not await self.has_read_permission(request, item_id):
-                return self.error_no_router_permission(request)
-            items = await self.read_items(request, item_id)
-            return BaseApiOut(data=items if len(items) > 1 else items[0])
-
-        return route
-
-    @property
-    def route_update(self) -> Callable:
-        async def route(
-            request: Request,
-            item_id: self.AnnotatedItemIdList,  # type: ignore
-            data: Annotated[self.schema_update, Body()],  # type: ignore
-        ):
-            if not await self.has_update_permission(request, item_id, data):
-                return self.error_no_router_permission(request)
-            values = await self.on_update_pre(request, data, item_id=item_id)
-            if not values:
-                return self.error_data_handle(request)
-            items = await self.update_items(request, item_id, values)
-            return BaseApiOut(data=len(items))
-
-        return route
-
-    @property
-    def route_delete(self) -> Callable:
-        async def route(
-            request: Request,
-            item_id: self.AnnotatedItemIdList,  # type: ignore
-        ):
-            if not await self.has_delete_permission(request, item_id):
-                return self.error_no_router_permission(request)
-            items = await self.delete_items(request, item_id)
-            return BaseApiOut(data=len(items))
-
-        return route
+import re
+from enum import Enum
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    Generic,
+    Iterable,
+    List,
+    Optional,
+    Pattern,
+    Tuple,
+    Type,
+    Union,
+)
+
+from fastapi import APIRouter, Body, Depends
+from fastapi._compat import field_annotation_is_scalar
+from fastapi.types import IncEx
+from sqlalchemy import Column, Table, func
+from sqlalchemy.engine import Result
+from sqlalchemy.future import select
+from sqlalchemy.orm import InstrumentedAttribute, Session, object_session
+from sqlalchemy.sql import Select
+from sqlalchemy.sql.elements import BinaryExpression, Label, UnaryExpression
+from starlette.requests import Request
+from typing_extensions import Annotated, Literal
+
+from fastapi_amis_admin.utils.pydantic import (
+    PYDANTIC_V2,
+    ModelField,
+    ValueItems,
+    annotation_outer_type,
+    create_model_by_fields,
+    field_allow_none,
+    model_fields,
+)
+
+try:
+    from functools import cached_property
+except ImportError:
+    from sqlalchemy.util.langhelpers import memoized_property as cached_property
+
+from .base import (
+    BaseCrud,
+    SchemaCreateT,
+    SchemaFilterT,
+    SchemaListT,
+    SchemaModelT,
+    SchemaReadT,
+    SchemaUpdateT,
+)
+from .parser import (
+    SqlaField,
+    SqlaInsAttr,
+    SqlaPropertyField,
+    TableModelParser,
+    TableModelT,
+    get_modelfield_by_alias,
+    get_python_type_parse,
+    parse_obj_to_schema,
+)
+from .schema import BaseApiOut, ItemListSchema
+from .utils import (
+    IdStrQuery,
+    ItemIdListDepend,
+    SqlalchemyDatabase,
+    get_engine_db,
+    parser_str_set_list,
+)
+
+sql_operator_pattern: Pattern = re.compile(r"^\[(=|<=|<|>|>=|!|!=|<>|\*|!\*|~|!~|-)]")
+sql_operator_map: Dict[str, str] = {
+    "=": "__eq__",
+    "<=": "__le__",
+    "<": "__lt__",
+    ">": "__gt__",
+    ">=": "__ge__",
+    "!": "__ne__",
+    "!=": "__ne__",
+    "<>": "__ne__",
+    "*": "in_",
+    "!*": "not_in",
+    "~": "like",
+    "!~": "not_like",
+    "-": "between",
+}
+
+
+class SqlalchemySelector(Generic[TableModelT]):
+    model: Type[TableModelT] = None  # SQLModel,DeclarativeMeta,InspectTable
+    fields: List[SqlaField] = []  # Need to query the field from the database
+    list_filter: List[SqlaField] = []  # Query filterable fields
+    exclude: List[SqlaInsAttr] = []  # Model fields that do not need to be queried. It is not recommended to use.
+    ordering: List[Union[SqlaField, UnaryExpression]] = []  # Default sort field
+    link_models: Dict[str, Tuple[Type[Table], Column, Column]] = None  # Link table information
+    """Relate information of the target model with the current model.
+    - The Data structure is: {Target table name: (link model table,
+        Column in the link model table associated with the current model,
+        Column in the link model table associated with the target model)}
+    - E.g. the current model is Role, you can add the target model User through `User.roles` here.
+        And then you can query the Role through the primary key field of the target model User.
+    - Saved information: {auth_user: (auth_user_roles, auth_user_roles.role_id, auth_user_roles.user_id)}
+    - You can add the query parameters to the route url to access the role list of the user:
+        `?link_model=auth_user&link_item_id={user_id}`.
+    """
+    pk_name: str = "id"  # Primary key name
+
+    def __init__(self, model: Type[TableModelT] = None, fields: List[SqlaField] = None) -> None:
+        self.model = model or self.model
+        assert self.model, "model is None"
+        assert hasattr(self.model, "__table__"), "model must be has __table__ attribute."
+        self.pk_name: str = self.pk_name or self.model.__table__.primary_key.columns.keys()[0]
+        self.pk: InstrumentedAttribute = self.model.__dict__[self.pk_name]
+        self.parser = TableModelParser(self.model)
+        fields = fields or self.fields or self.model_insfields
+        exclude = self.parser.filter_insfield(self.exclude)
+        self.fields = [
+            sqlfield
+            for sqlfield in self.parser.filter_insfield(fields + [self.pk], save_class=(Label,))
+            if sqlfield not in exclude
+        ]
+        assert self.fields, "fields is None"
+        self.list_filter = self.list_filter and self.list_filter.copy() or self.fields
+        self.link_models = self.link_models or {}
+        """Make sure the value of link_models is an object attribute, not a class attribute."""
+
+    @cached_property
+    def model_insfields(self) -> List[SqlaInsAttr]:
+        return self.parser.filter_insfield(self.model.__dict__.values())
+
+    @cached_property
+    def _select_entities(self) -> Dict[str, Union[InstrumentedAttribute, Label]]:
+        return {self.parser.get_alias(insfield): insfield for insfield in self.fields}
+
+    @cached_property
+    def _filter_entities(self) -> Dict[str, Union[InstrumentedAttribute, Label]]:
+        return {
+            self.parser.get_alias(sqlfield): sqlfield
+            for sqlfield in self.parser.filter_insfield(self.list_filter, save_class=(Label,))
+        }
+
+    async def get_select(self, request: Request) -> Select:
+        return select(*self._select_entities.values())
+
+    def _calc_ordering(self, orderBy, orderDir):
+        sqlfield = self._select_entities.get(orderBy, self._filter_entities.get(orderBy))
+        order = None
+        if sqlfield is not None:
+            order = sqlfield.desc() if orderDir == "desc" else sqlfield.asc()
+            return [order]
+        elif self.ordering is not None:
+            order = self.parser.filter_insfield(
+                self.ordering,
+                save_class=(
+                    UnaryExpression,
+                    Label,
+                ),
+            )
+        return order
+
+    @property
+    def _select_maker(self):
+        if self.link_models:
+
+            def select_maker(
+                sel: Annotated[Select, Depends(self.get_select)],  # type: ignore
+                link_clause: Annotated[Optional[Any], Depends(self.get_link_clause)] = None,  # type: ignore
+            ) -> Select:
+                if link_clause is not None:
+                    sel = sel.where(link_clause)
+                return sel
+
+        else:
+            select_maker = self.get_select
+        return select_maker
+
+    async def get_link_clause(
+        self,
+        request: Request,
+        link_model: str = None,
+        link_item_id: IdStrQuery = None,
+        op: Literal["in_", "not_in", None] = None,
+    ) -> Optional[Any]:
+        if link_model and link_item_id:
+            result = self.link_models.get(link_model)
+            if not result:
+                return None
+            table, pk_col, link_col = result
+            if table is not None:
+                link_item_id = list(
+                    map(
+                        get_python_type_parse(link_col),
+                        parser_str_set_list(link_item_id),
+                    )
+                )
+                if op == "not_in":
+                    return self.pk.not_in(select(pk_col).where(link_col.in_(link_item_id)))
+                else:
+                    return self.pk.in_(select(pk_col).where(link_col.in_(link_item_id)))
+        return None
+
+    @staticmethod
+    def _parser_query_value(
+        value: Any, operator: str = "__eq__", python_type_parse: Callable = str
+    ) -> Tuple[Optional[str], Union[tuple, None]]:
+        if isinstance(value, str):
+            if not value:
+                return None, None
+            match = sql_operator_pattern.match(value)
+            if match:
+                op_key = match.group(1)
+                operator = sql_operator_map.get(op_key)
+                value = value.replace(f"[{op_key}]", "")
+                if not value:
+                    return None, None
+                if operator in ["like", "not_like"] and value.find("%") == -1:
+                    return operator, (f"%{value}%",)
+                elif operator in ["in_", "not_in"]:
+                    return operator, (list(map(python_type_parse, set(value.split(",")))),)
+                elif operator == "between":
+                    value = value.split(",")[:2]
+                    if len(value) < 2:
+                        return None, None
+                    return operator, tuple(map(python_type_parse, value))
+        return operator, (python_type_parse(value),)
+
+    def calc_filter_clause(self, data: Dict[str, Any]) -> List[BinaryExpression]:
+        lst = []
+        for k, v in data.items():
+            sqlfield = self._filter_entities.get(k)
+            if sqlfield is not None:
+                operator, val = self._parser_query_value(v, python_type_parse=get_python_type_parse(sqlfield))
+                if operator:
+                    lst.append(getattr(sqlfield, operator)(*val))
+        return lst
+
+
+class SqlalchemyCrud(
+    BaseCrud[SchemaModelT, SchemaListT, SchemaFilterT, SchemaCreateT, SchemaReadT, SchemaUpdateT], SqlalchemySelector[TableModelT]
+):
+    engine: SqlalchemyDatabase = None  # sqlalchemy engine
+    create_fields: List[SqlaInsAttr] = []  # Create item data field
+    create_exclude: Optional[IncEx] = None
+    """create exclude fields, such as: {'id', 'key', 'name'} or {'id': True, 'category': {'id', 'name'}}."""
+    update_fields: List[SqlaPropertyField] = []
+    """model update fields;support model property and relationship field."""
+    update_exclude: Optional[IncEx] = None
+    """update exclude fields, such as: {'id', 'key', 'name'} or {'id': True, 'category': {'id', 'name'}}."""
+    read_fields: List[SqlaPropertyField] = []
+    """Model read fields; used in route_read, note the difference between readonly_fields and read_fields.
+    default is None, means not use read route."""
+
+    def __init__(
+        self,
+        model: Type[TableModelT],
+        engine: SqlalchemyDatabase,
+        fields: List[SqlaField] = None,
+        router: APIRouter = None,
+    ) -> None:
+        self.engine = engine or self.engine
+        assert self.engine, "engine is None"
+        self.db = get_engine_db(self.engine)
+        SqlalchemySelector.__init__(self, model, fields)
+        schema_model: Type[SchemaModelT] = self.schema_model or TableModelParser.get_table_model_schema(model)
+        BaseCrud.__init__(self, schema_model, router)
+        # if self.readonly_fields:
+        #     logging.warning(
+        #         "readonly fields, deprecated, not recommended, will be removed in version 0.4.0."
+        #         "Please replace them with update_fields and update_exclude."
+        #     )
+
+    @property
+    def router_prefix(self):
+        return f"/{self.model.__name__}"
+
+    def _create_schema_list(self) -> Type[SchemaListT]:
+        # Get the model fields from the select entities
+        modelfields = self.parser.filter_modelfield(
+            self._select_entities.values(),
+            save_class=(
+                Label,
+                ModelField,
+            ),
+        )
+        # Create the schema using the model fields
+        return create_model_by_fields(
+            name=f"{self.schema_name_prefix}List",
+            fields=modelfields,
+            set_none=True,
+            extra="allow",
+        )
+
+    def _create_schema_filter(self) -> Type[SchemaFilterT]:
+        # Get the filter fields from the list filter or select entities
+        list_filter = self.list_filter or self._select_entities.values()
+        # Filter out the model fields from the filter fields
+        modelfields = self.parser.filter_modelfield(list_filter, save_class=(Label,))
+        # Modify the modelfields if necessary
+        for modelfield in modelfields:
+            type_ = annotation_outer_type(modelfield.type_)
+            if field_annotation_is_scalar(modelfield.type_) and issubclass(type_, (Enum, bool, str)):
+                continue
+            if PYDANTIC_V2:
+                modelfield.field_info.annotation = str
+            else:
+                modelfield.type_ = str
+                modelfield.outer_type_ = str
+                modelfield.validators = []
+        # Create the schema using the model fields
+        return create_model_by_fields(
+            name=f"{self.schema_name_prefix}Filter",
+            fields=modelfields,
+            set_none=True,
+        )
+
+    def _create_schema_read(self) -> Optional[Type[SchemaReadT]]:
+        if not self.read_fields:
+            return None
+        # Filter out any non-model fields from the read fields
+        modelfields = self.parser.filter_modelfield(self.read_fields)
+        # Create the schema using the model fields
+        return create_model_by_fields(
+            name=f"{self.schema_name_prefix}Read",
+            fields=modelfields,
+            orm_mode=True,
+        )
+
+    def _create_schema_update(self) -> Type[SchemaUpdateT]:
+        # Set the update fields to the model insfields if not provided
+        self.update_fields = self.update_fields or self.model_insfields
+        # Exclude certain fields if specified
+        exclude = {k for k, v in ValueItems.merge(self.update_exclude, {}).items() if not isinstance(v, (dict, list, set))} or {
+            self.pk_name
+        }
+        # Filter out any non-model fields from the update fields
+        modelfields = self.parser.filter_modelfield(self.update_fields, exclude=exclude)
+        # Create the schema using the model fields
+        return create_model_by_fields(
+            name=f"{self.schema_name_prefix}Update",
+            fields=modelfields,
+            set_none=True,
+        )
+
+    def _create_schema_create(self) -> Type[SchemaCreateT]:
+        # Set the create fields to the model insfields if not provided
+        self.create_fields = self.create_fields or self.model_insfields
+        # Exclude certain fields if specified
+        exclude = {k for k, v in ValueItems.merge(self.create_exclude, {}).items() if not isinstance(v, (dict, list, set))} or {
+            self.pk_name
+        }
+        # Filter out any non-model fields from the create fields
+        modelfields = self.parser.filter_modelfield(self.create_fields, exclude=exclude)
+        # Create the schema using the model fields
+        return create_model_by_fields(
+            name=f"{self.schema_name_prefix}Create",
+            fields=modelfields,
+        )
+
+    def create_item(self, item: Dict[str, Any]) -> TableModelT:
+        """Create a database orm object through a dictionary."""
+        return self.model(**item)
+
+    def read_item(self, obj: TableModelT) -> SchemaReadT:
+        """read database data and parse to schema_read"""
+        return parse_obj_to_schema(obj, self.schema_read)
+
+    def update_item(self, obj: TableModelT, values: Dict[str, Any]) -> None:
+        """update schema_update data to database,support relational attributes"""
+        for k, v in values.items():
+            field = get_modelfield_by_alias(self.model, k)
+            if not field and not hasattr(obj, k):
+                continue
+            name = field.name if field else k
+            if isinstance(v, dict):
+                # Relational attributes, nested;such as: setattr(article.content, "body", "new body")
+                sub = getattr(obj, name)
+                if not isinstance(sub, dict):  # Ensure that the attribute is an object.
+                    self.update_item(sub, v)
+                    continue
+            setattr(obj, name, v)
+
+    def delete_item(self, obj: TableModelT) -> None:
+        """delete database data"""
+        object_session(obj).delete(obj)
+
+    def list_item(self, values: Dict[str, Any]) -> SchemaListT:
+        """Parse the database data query result dictionary into schema_list."""
+        return self.schema_list.parse_obj(values)
+
+    def _fetch_item_scalars(self, session: Session, item_id: Iterable[str]) -> List[TableModelT]:
+        sel = select(self.model).where(self.pk.in_(list(map(get_python_type_parse(self.pk), item_id))))
+        return session.scalars(sel).all()
+
+    async def fetch_items(self, *item_id: str) -> List[TableModelT]:
+        """Fetch the database data by id."""
+        return await self.db.async_run_sync(self._fetch_item_scalars, item_id)
+
+    def _create_items(self, session: Session, items: List[Dict[str, Any]]) -> List[TableModelT]:
+        if not items:
+            return []
+        objs = [self.create_item(item) for item in items]
+        session.add_all(objs)
+        session.flush()
+        return objs
+
+    async def create_items(self, request: Request, items: List[SchemaCreateT]) -> List[TableModelT]:
+        """Create multiple database data."""
+        items = [await self.on_create_pre(request, obj) for obj in items]
+        return await self.db.async_run_sync(self._create_items, items)
+
+    def _read_items(self, session: Session, item_id: List[str]) -> List[SchemaReadT]:
+        items = self._fetch_item_scalars(session, item_id)
+        return [self.read_item(obj) for obj in items]
+
+    async def read_items(self, request: Request, item_id: List[str]) -> List[SchemaReadT]:
+        """Fetch the database data by id."""
+        return await self.db.async_run_sync(self._read_items, item_id)
+
+    def _update_items(self, session: Session, item_id: List[str], values: Dict[str, Any]) -> List[TableModelT]:
+        items = self._fetch_item_scalars(session, item_id)
+        for item in items:
+            self.update_item(item, values)
+        return items
+
+    async def update_items(self, request: Request, item_id: List[str], values: Dict[str, Any]) -> List[TableModelT]:
+        """Update the database data by id."""
+        return await self.db.async_run_sync(self._update_items, item_id, values)
+
+    def _delete_items(self, session: Session, item_id: List[str]) -> List[TableModelT]:
+        items = self._fetch_item_scalars(session, item_id)
+        for item in items:
+            self.delete_item(item)
+        return items
+
+    async def delete_items(self, request: Request, item_id: List[str]) -> List[TableModelT]:
+        """Delete the database data by id."""
+        return await self.db.async_run_sync(self._delete_items, item_id)
+
+    @property
+    def schema_name_prefix(self):
+        if self.__class__ is SqlalchemyCrud:
+            return self.model.__name__
+        return super().schema_name_prefix
+
+    async def on_create_pre(self, request: Request, obj: SchemaCreateT, **kwargs) -> Dict[str, Any]:
+        data_dict = obj.dict(by_alias=True)  # exclude=set(self.pk)
+        if self.pk_name in data_dict and not data_dict.get(self.pk_name):
+            del data_dict[self.pk_name]
+        return data_dict
+
+    async def on_update_pre(
+        self,
+        request: Request,
+        obj: SchemaUpdateT,
+        item_id: Union[List[str], List[int]],
+        **kwargs,
+    ) -> Dict[str, Any]:
+        data = obj.dict(exclude=self.update_exclude, exclude_unset=True, by_alias=True)
+        data = {key: val for key, val in data.items() if val is not None or field_allow_none(model_fields(self.model)[key])}
+        return data
+
+    async def on_filter_pre(self, request: Request, obj: Optional[SchemaFilterT], **kwargs) -> Dict[str, Any]:
+        return obj and {k: v for k, v in obj.dict(exclude_unset=True, by_alias=True).items() if v is not None}
+
+    async def on_list_after(self, request: Request, result: Result, data: ItemListSchema, **kwargs) -> ItemListSchema:
+        """Parse the database data query result dictionary into schema_list."""
+        data.items = self.parser.conv_row_to_dict(result.all())
+        data.items = [self.list_item(item) for item in data.items]
+        return data
+
+    @property
+    def AnnotatedSelect(self):
+        """Annotated Select, used to automatically perform fastapi dependency injection"""
+        return Annotated[Select, Depends(self._select_maker)]
+
+    @property
+    def AnnotatedItemIdList(self):
+        """Annotated Item ID List, used to filter the id of the data that the user has permission to operate on.
+        And automatically perform fastapi dependency injection
+        """
+        return Annotated[List[str], Depends(self.filtered_item_id)]
+
+    @property
+    def filtered_item_id(self) -> Callable:
+        """Filter the id of the data that the user has permission to operate on."""
+
+        async def depend(
+            item_id: ItemIdListDepend,
+            sel: self.AnnotatedSelect,  # type: ignore
+        ):
+            item_id = list(map(get_python_type_parse(self.pk), item_id))
+            filtered_id = await self.db.async_scalars(sel.where(self.pk.in_(item_id)).with_only_columns(self.pk))
+            return filtered_id.all()
+
+        return depend
+
+    @property
+    def route_list(self) -> Callable:
+        async def route(
+            request: Request,
+            sel: self.AnnotatedSelect,  # type: ignore
+            paginator: Annotated[self.paginator, Depends()],  # type: ignore
+            filters: Annotated[self.schema_filter, Body()] = None,  # type: ignore
+        ):
+            if not await self.has_list_permission(request, paginator, filters):
+                return self.error_no_router_permission(request)
+            data = ItemListSchema(items=[])
+            data.query = request.query_params
+            if await self.has_filter_permission(request, filters):
+                data.filters = await self.on_filter_pre(request, filters)
+                if data.filters:
+                    sel = sel.filter(*self.calc_filter_clause(data.filters))
+            if paginator.show_total:
+                data.total = await self.db.async_scalar(
+                    select(func.count("*")).select_from(sel.with_only_columns(self.pk).subquery())
+                )
+            orderBy = self._calc_ordering(paginator.orderBy, paginator.orderDir)
+            if orderBy:
+                sel = sel.order_by(*orderBy)
+            sel = sel.limit(paginator.perPage).offset((paginator.page - 1) * paginator.perPage)
+            result = await self.db.async_execute(sel)
+            return BaseApiOut(data=await self.on_list_after(request, result, data))
+
+        return route
+
+    @property
+    def route_create(self) -> Callable:
+        async def route(
+            request: Request,
+            data: Annotated[Union[List[self.schema_create], self.schema_create], Body()],  # type: ignore
+        ) -> BaseApiOut[Union[int, self.schema_model]]:  # type: ignore
+            if not await self.has_create_permission(request, data):
+                return self.error_no_router_permission(request)
+            if not isinstance(data, list):
+                data = [data]
+            try:
+                items = await self.create_items(request, data)
+            except Exception as error:
+                return self.error_execute_sql(request=request, error=error)
+            result = len(items)
+            if result == 1:  # if only one item, return the first item
+                result = await self.db.async_run_sync(lambda _: parse_obj_to_schema(items[0], self.schema_model, refresh=True))
+            return BaseApiOut(data=result)
+
+        return route
+
+    @property
+    def route_read(self) -> Callable:
+        async def route(
+            request: Request,
+            item_id: self.AnnotatedItemIdList,  # type: ignore
+        ):
+            if not await self.has_read_permission(request, item_id):
+                return self.error_no_router_permission(request)
+            items = await self.read_items(request, item_id)
+            return BaseApiOut(data=items if len(items) > 1 else items[0])
+
+        return route
+
+    @property
+    def route_update(self) -> Callable:
+        async def route(
+            request: Request,
+            item_id: self.AnnotatedItemIdList,  # type: ignore
+            data: Annotated[self.schema_update, Body()],  # type: ignore
+        ):
+            if not await self.has_update_permission(request, item_id, data):
+                return self.error_no_router_permission(request)
+            values = await self.on_update_pre(request, data, item_id=item_id)
+            if not values:
+                return self.error_data_handle(request)
+            items = await self.update_items(request, item_id, values)
+            return BaseApiOut(data=len(items))
+
+        return route
+
+    @property
+    def route_delete(self) -> Callable:
+        async def route(
+            request: Request,
+            item_id: self.AnnotatedItemIdList,  # type: ignore
+        ):
+            if not await self.has_delete_permission(request, item_id):
+                return self.error_no_router_permission(request)
+            items = await self.delete_items(request, item_id)
+            return BaseApiOut(data=len(items))
+
+        return route
```

### Comparing `fastapi_amis_admin-0.6.3/fastapi_amis_admin/crud/base.py` & `fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/crud/base.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,222 +1,222 @@
-from typing import Any, Callable, Generic, List, Optional, Type, TypeVar, Union
-
-from fastapi import APIRouter, Depends
-from pydantic import BaseModel
-from sqlalchemy.exc import IntegrityError
-from starlette import status
-from starlette.exceptions import HTTPException
-from starlette.requests import Request
-
-from ..utils.pydantic import create_model_by_model
-from .schema import BaseApiOut, CrudEnum, ItemListSchema, Paginator
-
-SchemaModelT = TypeVar("SchemaModelT", bound=BaseModel)
-SchemaListT = TypeVar("SchemaListT", bound=BaseModel)
-SchemaFilterT = TypeVar("SchemaFilterT", bound=BaseModel)
-SchemaCreateT = TypeVar("SchemaCreateT", bound=BaseModel)
-SchemaReadT = TypeVar("SchemaReadT", bound=BaseModel)
-SchemaUpdateT = TypeVar("SchemaUpdateT", bound=BaseModel)
-
-
-class RouterMixin:
-    router: APIRouter = None
-    router_prefix: Optional[str] = None
-    router_permission_depend: Callable = None
-
-    def __init__(self):
-        self.router = self.get_router()
-
-    def get_router(self) -> APIRouter:
-        if self.router is None:
-            if self.router_prefix is None:
-                self.router_prefix = f"/{self.__class__.__name__}"
-            self.router = APIRouter(prefix=self.router_prefix, tags=[self.router_prefix[1:]])
-        if self.router_permission_depend is not None:
-            self.router.dependencies.insert(0, Depends(self.router_permission_depend))
-        return self.router
-
-    def error_no_router_permission(self, request: Request):
-        raise HTTPException(status_code=status.HTTP_401_UNAUTHORIZED, detail="No router permissions")
-
-
-class BaseCrud(RouterMixin, Generic[SchemaModelT, SchemaListT, SchemaFilterT, SchemaCreateT, SchemaReadT, SchemaUpdateT]):
-    schema_model: Type[SchemaModelT] = None
-    schema_list: Type[SchemaListT] = None
-    schema_filter: Type[SchemaFilterT] = None
-    schema_create: Type[SchemaCreateT] = None
-    schema_read: Type[SchemaReadT] = None
-    schema_update: Type[SchemaUpdateT] = None
-    pk_name: str = "id"
-    list_per_page_max: int = None
-
-    def __init__(self, schema_model: Type[SchemaModelT], router: APIRouter = None):
-        self.paginator = Paginator()
-        self.schema_model = schema_model or self.schema_model
-        assert self.schema_model, "schema_model is None"
-        self.router = router
-        RouterMixin.__init__(self)
-
-    @property
-    def router_prefix(self):
-        return f"/{self.schema_model.__name__}"
-
-    @property
-    def schema_name_prefix(self):
-        return self.__class__.__name__
-
-    def register_crud(
-        self,
-        schema_list: Type[SchemaListT] = None,
-        schema_filter: Type[SchemaFilterT] = None,
-        schema_create: Type[SchemaCreateT] = None,
-        schema_read: Type[SchemaReadT] = None,  # default is None, means not use read route.
-        schema_update: Type[SchemaUpdateT] = None,
-        list_per_page_max: int = None,
-        depends_list: List[Depends] = None,
-        depends_read: List[Depends] = None,
-        depends_create: List[Depends] = None,
-        depends_update: List[Depends] = None,
-        depends_delete: List[Depends] = None,
-    ) -> "BaseCrud":
-        self.schema_list = schema_list or self.schema_list or self._create_schema_list()
-        self.schema_filter = schema_filter or self.schema_filter or self._create_schema_filter()
-        self.schema_create = schema_create or self.schema_create or self._create_schema_create()
-        self.schema_read = schema_read or self.schema_read or self._create_schema_read()
-        self.schema_update = schema_update or self.schema_update or self._create_schema_update()
-        self.list_per_page_max = list_per_page_max or self.list_per_page_max
-        self.paginator = Paginator(perPageMax=self.list_per_page_max)
-        self.router.add_api_route(
-            "/list",
-            self.route_list,
-            methods=["POST"],
-            response_model=BaseApiOut[ItemListSchema[self.schema_list]],
-            dependencies=depends_list,
-            name=CrudEnum.list,
-        )
-        if self.schema_read:
-            self.router.add_api_route(
-                "/item/{item_id}",
-                self.route_read,
-                methods=["GET"],
-                response_model=BaseApiOut[Union[self.schema_read, List[self.schema_read]]],
-                dependencies=depends_read,
-                name=CrudEnum.read,
-            )
-        self.router.add_api_route(
-            "/item",
-            self.route_create,
-            methods=["POST"],
-            response_model=BaseApiOut[Union[int, self.schema_model]],
-            dependencies=depends_create,
-            name=CrudEnum.create,
-        )
-        self.router.add_api_route(
-            "/item/{item_id}",
-            self.route_update,
-            methods=["PUT"],
-            response_model=BaseApiOut[int],
-            dependencies=depends_update,
-            name=CrudEnum.update,
-        )
-        self.router.add_api_route(
-            "/item/{item_id}",
-            self.route_delete,
-            methods=["DELETE"],
-            response_model=BaseApiOut[int],
-            dependencies=depends_delete,
-            name=CrudEnum.delete,
-        )
-        return self
-
-    def _create_schema_list(self) -> Type[SchemaListT]:
-        return self.schema_model
-
-    def _create_schema_filter(self) -> Type[SchemaFilterT]:
-        return create_model_by_model(self.schema_list, f"{self.schema_name_prefix}Filter", set_none=True)
-
-    def _create_schema_read(self) -> Optional[Type[SchemaReadT]]:
-        return None
-
-    def _create_schema_update(self) -> Type[SchemaUpdateT]:
-        return create_model_by_model(
-            self.schema_model,
-            f"{self.schema_name_prefix}Update",
-            exclude={self.pk_name},
-            set_none=True,
-        )
-
-    def _create_schema_create(self) -> Type[SchemaCreateT]:
-        return create_model_by_model(
-            self.schema_model,
-            f"{self.schema_name_prefix}Create",
-            exclude={self.pk_name},
-        )
-
-    @property
-    def route_list(self) -> Callable[..., Any]:
-        raise NotImplementedError
-
-    @property
-    def route_read(self) -> Callable[..., Any]:
-        raise NotImplementedError
-
-    @property
-    def route_create(self) -> Callable[..., Any]:
-        raise NotImplementedError
-
-    @property
-    def route_update(self) -> Callable[..., Any]:
-        raise NotImplementedError
-
-    @property
-    def route_delete(self) -> Callable[..., Any]:
-        raise NotImplementedError
-
-    async def has_list_permission(
-        self,
-        request: Request,
-        paginator: Optional[Paginator],
-        filters: Optional[SchemaFilterT],
-        **kwargs,
-    ) -> bool:
-        return True
-
-    async def has_filter_permission(
-        self,
-        request: Request,
-        filters: Optional[SchemaFilterT],
-        **kwargs,
-    ) -> bool:
-        return True
-
-    async def has_create_permission(self, request: Request, obj: Optional[SchemaCreateT], **kwargs) -> bool:
-        return True
-
-    async def has_read_permission(self, request: Request, item_id: Optional[List[str]], **kwargs) -> bool:
-        return True
-
-    async def has_update_permission(
-        self,
-        request: Request,
-        item_id: Optional[List[str]],
-        obj: Optional[SchemaUpdateT],
-        **kwargs,
-    ) -> bool:
-        return True
-
-    async def has_delete_permission(self, request: Request, item_id: Optional[List[str]], **kwargs) -> bool:
-        return True
-
-    def error_data_handle(self, request: Request):
-        raise HTTPException(status.HTTP_400_BAD_REQUEST, "error data handle")
-
-    def error_execute_sql(self, request: Request, error: Exception):
-        if isinstance(error, IntegrityError):
-            raise HTTPException(
-                status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
-                detail="Key already exists",
-            ) from error
-        raise HTTPException(
-            status_code=status.HTTP_500_INTERNAL_SERVER_ERROR,
-            detail=f"Error Execute SQL：{error}",
-        ) from error
+from typing import Any, Callable, Generic, List, Optional, Type, TypeVar, Union
+
+from fastapi import APIRouter, Depends
+from pydantic import BaseModel
+from sqlalchemy.exc import IntegrityError
+from starlette import status
+from starlette.exceptions import HTTPException
+from starlette.requests import Request
+
+from ..utils.pydantic import create_model_by_model
+from .schema import BaseApiOut, CrudEnum, ItemListSchema, Paginator
+
+SchemaModelT = TypeVar("SchemaModelT", bound=BaseModel)
+SchemaListT = TypeVar("SchemaListT", bound=BaseModel)
+SchemaFilterT = TypeVar("SchemaFilterT", bound=BaseModel)
+SchemaCreateT = TypeVar("SchemaCreateT", bound=BaseModel)
+SchemaReadT = TypeVar("SchemaReadT", bound=BaseModel)
+SchemaUpdateT = TypeVar("SchemaUpdateT", bound=BaseModel)
+
+
+class RouterMixin:
+    router: APIRouter = None
+    router_prefix: Optional[str] = None
+    router_permission_depend: Callable = None
+
+    def __init__(self):
+        self.router = self.get_router()
+
+    def get_router(self) -> APIRouter:
+        if self.router is None:
+            if self.router_prefix is None:
+                self.router_prefix = f"/{self.__class__.__name__}"
+            self.router = APIRouter(prefix=self.router_prefix, tags=[self.router_prefix[1:]])
+        if self.router_permission_depend is not None:
+            self.router.dependencies.insert(0, Depends(self.router_permission_depend))
+        return self.router
+
+    def error_no_router_permission(self, request: Request):
+        raise HTTPException(status_code=status.HTTP_401_UNAUTHORIZED, detail="No router permissions")
+
+
+class BaseCrud(RouterMixin, Generic[SchemaModelT, SchemaListT, SchemaFilterT, SchemaCreateT, SchemaReadT, SchemaUpdateT]):
+    schema_model: Type[SchemaModelT] = None
+    schema_list: Type[SchemaListT] = None
+    schema_filter: Type[SchemaFilterT] = None
+    schema_create: Type[SchemaCreateT] = None
+    schema_read: Type[SchemaReadT] = None
+    schema_update: Type[SchemaUpdateT] = None
+    pk_name: str = "id"
+    list_per_page_max: int = None
+
+    def __init__(self, schema_model: Type[SchemaModelT], router: APIRouter = None):
+        self.paginator = Paginator()
+        self.schema_model = schema_model or self.schema_model
+        assert self.schema_model, "schema_model is None"
+        self.router = router
+        RouterMixin.__init__(self)
+
+    @property
+    def router_prefix(self):
+        return f"/{self.schema_model.__name__}"
+
+    @property
+    def schema_name_prefix(self):
+        return self.__class__.__name__
+
+    def register_crud(
+        self,
+        schema_list: Type[SchemaListT] = None,
+        schema_filter: Type[SchemaFilterT] = None,
+        schema_create: Type[SchemaCreateT] = None,
+        schema_read: Type[SchemaReadT] = None,  # default is None, means not use read route.
+        schema_update: Type[SchemaUpdateT] = None,
+        list_per_page_max: int = None,
+        depends_list: List[Depends] = None,
+        depends_read: List[Depends] = None,
+        depends_create: List[Depends] = None,
+        depends_update: List[Depends] = None,
+        depends_delete: List[Depends] = None,
+    ) -> "BaseCrud":
+        self.schema_list = schema_list or self.schema_list or self._create_schema_list()
+        self.schema_filter = schema_filter or self.schema_filter or self._create_schema_filter()
+        self.schema_create = schema_create or self.schema_create or self._create_schema_create()
+        self.schema_read = schema_read or self.schema_read or self._create_schema_read()
+        self.schema_update = schema_update or self.schema_update or self._create_schema_update()
+        self.list_per_page_max = list_per_page_max or self.list_per_page_max
+        self.paginator = Paginator(perPageMax=self.list_per_page_max)
+        self.router.add_api_route(
+            "/list",
+            self.route_list,
+            methods=["POST"],
+            response_model=BaseApiOut[ItemListSchema[self.schema_list]],
+            dependencies=depends_list,
+            name=CrudEnum.list,
+        )
+        if self.schema_read:
+            self.router.add_api_route(
+                "/item/{item_id}",
+                self.route_read,
+                methods=["GET"],
+                response_model=BaseApiOut[Union[self.schema_read, List[self.schema_read]]],
+                dependencies=depends_read,
+                name=CrudEnum.read,
+            )
+        self.router.add_api_route(
+            "/item",
+            self.route_create,
+            methods=["POST"],
+            response_model=BaseApiOut[Union[int, self.schema_model]],
+            dependencies=depends_create,
+            name=CrudEnum.create,
+        )
+        self.router.add_api_route(
+            "/item/{item_id}",
+            self.route_update,
+            methods=["PUT"],
+            response_model=BaseApiOut[int],
+            dependencies=depends_update,
+            name=CrudEnum.update,
+        )
+        self.router.add_api_route(
+            "/item/{item_id}",
+            self.route_delete,
+            methods=["DELETE"],
+            response_model=BaseApiOut[int],
+            dependencies=depends_delete,
+            name=CrudEnum.delete,
+        )
+        return self
+
+    def _create_schema_list(self) -> Type[SchemaListT]:
+        return self.schema_model
+
+    def _create_schema_filter(self) -> Type[SchemaFilterT]:
+        return create_model_by_model(self.schema_list, f"{self.schema_name_prefix}Filter", set_none=True)
+
+    def _create_schema_read(self) -> Optional[Type[SchemaReadT]]:
+        return None
+
+    def _create_schema_update(self) -> Type[SchemaUpdateT]:
+        return create_model_by_model(
+            self.schema_model,
+            f"{self.schema_name_prefix}Update",
+            exclude={self.pk_name},
+            set_none=True,
+        )
+
+    def _create_schema_create(self) -> Type[SchemaCreateT]:
+        return create_model_by_model(
+            self.schema_model,
+            f"{self.schema_name_prefix}Create",
+            exclude={self.pk_name},
+        )
+
+    @property
+    def route_list(self) -> Callable[..., Any]:
+        raise NotImplementedError
+
+    @property
+    def route_read(self) -> Callable[..., Any]:
+        raise NotImplementedError
+
+    @property
+    def route_create(self) -> Callable[..., Any]:
+        raise NotImplementedError
+
+    @property
+    def route_update(self) -> Callable[..., Any]:
+        raise NotImplementedError
+
+    @property
+    def route_delete(self) -> Callable[..., Any]:
+        raise NotImplementedError
+
+    async def has_list_permission(
+        self,
+        request: Request,
+        paginator: Optional[Paginator],
+        filters: Optional[SchemaFilterT],
+        **kwargs,
+    ) -> bool:
+        return True
+
+    async def has_filter_permission(
+        self,
+        request: Request,
+        filters: Optional[SchemaFilterT],
+        **kwargs,
+    ) -> bool:
+        return True
+
+    async def has_create_permission(self, request: Request, obj: Optional[SchemaCreateT], **kwargs) -> bool:
+        return True
+
+    async def has_read_permission(self, request: Request, item_id: Optional[List[str]], **kwargs) -> bool:
+        return True
+
+    async def has_update_permission(
+        self,
+        request: Request,
+        item_id: Optional[List[str]],
+        obj: Optional[SchemaUpdateT],
+        **kwargs,
+    ) -> bool:
+        return True
+
+    async def has_delete_permission(self, request: Request, item_id: Optional[List[str]], **kwargs) -> bool:
+        return True
+
+    def error_data_handle(self, request: Request):
+        raise HTTPException(status.HTTP_400_BAD_REQUEST, "error data handle")
+
+    def error_execute_sql(self, request: Request, error: Exception):
+        if isinstance(error, IntegrityError):
+            raise HTTPException(
+                status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
+                detail="Key already exists",
+            ) from error
+        raise HTTPException(
+            status_code=status.HTTP_500_INTERNAL_SERVER_ERROR,
+            detail=f"Error Execute SQL：{error}",
+        ) from error
```

### Comparing `fastapi_amis_admin-0.6.3/fastapi_amis_admin/crud/schema.py` & `fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/crud/schema.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-from enum import Enum
-from typing import Any, Dict, Generic, List, Optional, TypeVar, Union
-
-from fastapi_amis_admin.utils.pydantic import AllowExtraModelMixin, GenericModel
-
-_T = TypeVar("_T")
-
-
-class BaseApiSchema(AllowExtraModelMixin):
-    pass
-
-
-class BaseApiOut(BaseApiSchema, GenericModel, Generic[_T]):
-    status: int = 0
-    msg: str = "success"
-    data: Optional[_T] = None
-    code: Optional[int] = None
-
-
-class ItemListSchema(BaseApiSchema, GenericModel, Generic[_T]):
-    """Data list query return format."""
-
-    items: List[_T] = []  # Data list
-    total: Optional[int] = None  # Data total
-    query: Optional[Dict[str, Any]] = None
-    filter: Optional[Dict[str, Any]] = None
-
-
-class CrudEnum(str, Enum):
-    list = "list"
-    filter = "filter"
-    create = "create"
-    read = "read"
-    update = "update"
-    delete = "delete"
-
-
-class Paginator:
-    """Used for data paging when querying a data list."""
-
-    def __init__(self, perPageMax: int = None, perPageDefault: int = 10):
-        self.perPageMax = perPageMax
-        self.perPageDefault = perPageDefault
-
-    def __call__(
-        self,
-        page: Union[int, str] = 1,
-        perPage: Union[int, str] = None,
-        show_total: int = 1,
-        orderBy: str = None,
-        orderDir: str = "asc",
-    ):
-        self.page = page if page and page > 0 else self.perPageDefault
-        self.perPage = perPage if perPage and perPage > 0 else self.perPageDefault
-        if self.perPageMax:
-            self.perPage = min(self.perPage, self.perPageMax)
-        self.show_total = show_total
-        self.orderBy = orderBy
-        self.orderDir = orderDir
-        return self
+from enum import Enum
+from typing import Any, Dict, Generic, List, Optional, TypeVar, Union
+
+from fastapi_amis_admin.utils.pydantic import AllowExtraModelMixin, GenericModel
+
+_T = TypeVar("_T")
+
+
+class BaseApiSchema(AllowExtraModelMixin):
+    pass
+
+
+class BaseApiOut(BaseApiSchema, GenericModel, Generic[_T]):
+    status: int = 0
+    msg: str = "success"
+    data: Optional[_T] = None
+    code: Optional[int] = None
+
+
+class ItemListSchema(BaseApiSchema, GenericModel, Generic[_T]):
+    """Data list query return format."""
+
+    items: List[_T] = []  # Data list
+    total: Optional[int] = None  # Data total
+    query: Optional[Dict[str, Any]] = None
+    filter: Optional[Dict[str, Any]] = None
+
+
+class CrudEnum(str, Enum):
+    list = "list"
+    filter = "filter"
+    create = "create"
+    read = "read"
+    update = "update"
+    delete = "delete"
+
+
+class Paginator:
+    """Used for data paging when querying a data list."""
+
+    def __init__(self, perPageMax: int = None, perPageDefault: int = 10):
+        self.perPageMax = perPageMax
+        self.perPageDefault = perPageDefault
+
+    def __call__(
+        self,
+        page: Union[int, str] = 1,
+        perPage: Union[int, str] = None,
+        show_total: int = 1,
+        orderBy: str = None,
+        orderDir: str = "asc",
+    ):
+        self.page = page if page and page > 0 else self.perPageDefault
+        self.perPage = perPage if perPage and perPage > 0 else self.perPageDefault
+        if self.perPageMax:
+            self.perPage = min(self.perPage, self.perPageMax)
+        self.show_total = show_total
+        self.orderBy = orderBy
+        self.orderDir = orderDir
+        return self
```

### Comparing `fastapi_amis_admin-0.6.3/fastapi_amis_admin/crud/utils.py` & `fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/crud/utils.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-import warnings
-from typing import List, Union
-
-from fastapi import Depends, Path, Query
-from sqlalchemy.engine import Engine
-from sqlalchemy.ext.asyncio import AsyncEngine
-from sqlalchemy_database import AsyncDatabase, Database
-from typing_extensions import Annotated
-
-SqlalchemyDatabase = Union[Engine, AsyncEngine, Database, AsyncDatabase]
-
-
-IdStrQuery = Annotated[
-    str,
-    Query(
-        title="ids",
-        examples=["1", "1,2,3"],
-        description="Primary key or list of primary keys",
-    ),
-]
-
-
-def parser_str_set_list(item_id: Union[int, str]) -> List[str]:
-    if isinstance(item_id, int):
-        return [str(item_id)]
-    elif not isinstance(item_id, str):
-        return []
-    return list(set(item_id.split(",")))
-
-
-ItemIdListDepend = Annotated[List[str], Depends(parser_str_set_list)]
-
-
-def parser_item_id(
-    item_id: str = Path(
-        ...,
-        min_length=1,
-        title="pk",
-        examples=["1", "1,2,3"],
-        description="Primary key or list of primary keys",
-    )
-) -> List[str]:
-    """Deprecated, use ItemIdListDepend and parser_str_set_list instead"""
-    warnings.warn(
-        "Deprecated, use ItemIdListDepend and parser_str_set_list instead",
-        DeprecationWarning,
-        stacklevel=2,
-    )
-    return parser_str_set_list(item_id)
-
-
-def get_engine_db(engine: SqlalchemyDatabase) -> Union[Database, AsyncDatabase]:
-    if isinstance(engine, (Database, AsyncDatabase)):
-        return engine
-    if isinstance(engine, Engine):
-        return Database(engine)
-    if isinstance(engine, AsyncEngine):
-        return AsyncDatabase(engine)
-    raise TypeError(f"Unknown engine type: {type(engine)}")
+import warnings
+from typing import List, Union
+
+from fastapi import Depends, Path, Query
+from sqlalchemy.engine import Engine
+from sqlalchemy.ext.asyncio import AsyncEngine
+from sqlalchemy_database import AsyncDatabase, Database
+from typing_extensions import Annotated
+
+SqlalchemyDatabase = Union[Engine, AsyncEngine, Database, AsyncDatabase]
+
+
+IdStrQuery = Annotated[
+    str,
+    Query(
+        title="ids",
+        examples=["1", "1,2,3"],
+        description="Primary key or list of primary keys",
+    ),
+]
+
+
+def parser_str_set_list(item_id: Union[int, str]) -> List[str]:
+    if isinstance(item_id, int):
+        return [str(item_id)]
+    elif not isinstance(item_id, str):
+        return []
+    return list(set(item_id.split(",")))
+
+
+ItemIdListDepend = Annotated[List[str], Depends(parser_str_set_list)]
+
+
+def parser_item_id(
+    item_id: str = Path(
+        ...,
+        min_length=1,
+        title="pk",
+        examples=["1", "1,2,3"],
+        description="Primary key or list of primary keys",
+    )
+) -> List[str]:
+    """Deprecated, use ItemIdListDepend and parser_str_set_list instead"""
+    warnings.warn(
+        "Deprecated, use ItemIdListDepend and parser_str_set_list instead",
+        DeprecationWarning,
+        stacklevel=2,
+    )
+    return parser_str_set_list(item_id)
+
+
+def get_engine_db(engine: SqlalchemyDatabase) -> Union[Database, AsyncDatabase]:
+    if isinstance(engine, (Database, AsyncDatabase)):
+        return engine
+    if isinstance(engine, Engine):
+        return Database(engine)
+    if isinstance(engine, AsyncEngine):
+        return AsyncDatabase(engine)
+    raise TypeError(f"Unknown engine type: {type(engine)}")
```

### Comparing `fastapi_amis_admin-0.6.3/fastapi_amis_admin/locale/de_DE/LC_MESSAGES/messages.mo` & `fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/locale/de_DE/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.6.3/fastapi_amis_admin/locale/zh_CN/LC_MESSAGES/messages.mo` & `fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/locale/zh_CN/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.6.3/fastapi_amis_admin/locale/zh_CN/LC_MESSAGES/messages.po` & `fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/locale/zh_CN/LC_MESSAGES/messages.po`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,112 +1,112 @@
-# Chinese (Simplified, China) translations for PROJECT.
-# Copyright (C) 2023 ORGANIZATION
-# This file is distributed under the same license as the PROJECT project.
-# FIRST AUTHOR <EMAIL@ADDRESS>, 2023.
-#
-msgid ""
-msgstr ""
-"Project-Id-Version: PROJECT VERSION\n"
-"Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-03-03 08:56+0800\n"
-"PO-Revision-Date: 2023-03-03 08:57+0800\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
-"Language: zh_Hans_CN\n"
-"Language-Team: zh_Hans_CN <LL@li.org>\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
-"MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=utf-8\n"
-"Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.12.1\n"
-
-#: admin/admin.py:235 admin/admin.py:252 admin/admin.py:255
-msgid "Add Association"
-msgstr "添加关联"
-
-#: admin/admin.py:237
-msgid "Are you sure you want to add the association?"
-msgstr "你确定要添加关联吗?"
-
-#: admin/admin.py:278
-msgid "Remove Association"
-msgstr "移除关联"
-
-#: admin/admin.py:280
-msgid "Are you sure you want to remove the association?"
-msgstr "你确定要移除关联吗?"
-
-#: admin/admin.py:401
-msgid "Operation"
-msgstr "操作"
-
-#: admin/admin.py:449
-msgid "SHOWING ${items|count} OF ${total} RESULT(S)"
-msgstr "显示${total}条结果中的${items|count}条"
-
-#: admin/admin.py:535
-msgid "Filter"
-msgstr "数据筛选"
-
-#: admin/admin.py:542
-msgid "Clear"
-msgstr "清空"
-
-#: admin/admin.py:547
-msgid "Reset"
-msgstr "重置"
-
-#: admin/admin.py:550
-msgid "Search"
-msgstr "搜索"
-
-#: admin/admin.py:623 admin/admin.py:626 admin/admin.py:1065
-msgid "View"
-msgstr "查看"
-
-#: admin/admin.py:636 admin/admin.py:639 admin/admin.py:1020
-msgid "Create"
-msgstr "新增"
-
-#: admin/admin.py:646 admin/admin.py:649 admin/admin.py:1057
-msgid "Bulk Create"
-msgstr "批量新增"
-
-#: admin/admin.py:659 admin/admin.py:661 admin/admin.py:1027
-msgid "Update"
-msgstr "更新"
-
-#: admin/admin.py:668 admin/admin.py:670 admin/admin.py:1073
-msgid "Bulk Update"
-msgstr "批量更新"
-
-#: amis_admin/admin.py:484
-msgid "Bulk Delete"
-msgstr "批量删除"
-
-#: admin/admin.py:1036
-msgid "Delete"
-msgstr "删除"
-
-#: admin/admin.py:1037
-#, python-format
-msgid "Are you sure you want to delete row ${%s}?"
-msgstr "你确定要删除行${%s}?"
-
-#: admin/admin.py:1047
-msgid "Are you sure you want to delete the selected rows?"
-msgstr "你确定要批量删除选中行吗?"
-
-#: admin/admin.py:1194
-msgid "Custom form actions"
-msgstr "自定义表单动作"
-
-#: admin/parser.py:183
-msgid "YES"
-msgstr "是"
-
-#: admin/parser.py:184
-msgid "NO"
-msgstr "否"
-
-#: admin/site.py:50
-msgid "Home"
+# Chinese (Simplified, China) translations for PROJECT.
+# Copyright (C) 2023 ORGANIZATION
+# This file is distributed under the same license as the PROJECT project.
+# FIRST AUTHOR <EMAIL@ADDRESS>, 2023.
+#
+msgid ""
+msgstr ""
+"Project-Id-Version: PROJECT VERSION\n"
+"Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
+"POT-Creation-Date: 2023-03-03 08:56+0800\n"
+"PO-Revision-Date: 2023-03-03 08:57+0800\n"
+"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"Language: zh_Hans_CN\n"
+"Language-Team: zh_Hans_CN <LL@li.org>\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
+"MIME-Version: 1.0\n"
+"Content-Type: text/plain; charset=utf-8\n"
+"Content-Transfer-Encoding: 8bit\n"
+"Generated-By: Babel 2.12.1\n"
+
+#: admin/admin.py:235 admin/admin.py:252 admin/admin.py:255
+msgid "Add Association"
+msgstr "添加关联"
+
+#: admin/admin.py:237
+msgid "Are you sure you want to add the association?"
+msgstr "你确定要添加关联吗?"
+
+#: admin/admin.py:278
+msgid "Remove Association"
+msgstr "移除关联"
+
+#: admin/admin.py:280
+msgid "Are you sure you want to remove the association?"
+msgstr "你确定要移除关联吗?"
+
+#: admin/admin.py:401
+msgid "Operation"
+msgstr "操作"
+
+#: admin/admin.py:449
+msgid "SHOWING ${items|count} OF ${total} RESULT(S)"
+msgstr "显示${total}条结果中的${items|count}条"
+
+#: admin/admin.py:535
+msgid "Filter"
+msgstr "数据筛选"
+
+#: admin/admin.py:542
+msgid "Clear"
+msgstr "清空"
+
+#: admin/admin.py:547
+msgid "Reset"
+msgstr "重置"
+
+#: admin/admin.py:550
+msgid "Search"
+msgstr "搜索"
+
+#: admin/admin.py:623 admin/admin.py:626 admin/admin.py:1065
+msgid "View"
+msgstr "查看"
+
+#: admin/admin.py:636 admin/admin.py:639 admin/admin.py:1020
+msgid "Create"
+msgstr "新增"
+
+#: admin/admin.py:646 admin/admin.py:649 admin/admin.py:1057
+msgid "Bulk Create"
+msgstr "批量新增"
+
+#: admin/admin.py:659 admin/admin.py:661 admin/admin.py:1027
+msgid "Update"
+msgstr "更新"
+
+#: admin/admin.py:668 admin/admin.py:670 admin/admin.py:1073
+msgid "Bulk Update"
+msgstr "批量更新"
+
+#: amis_admin/admin.py:484
+msgid "Bulk Delete"
+msgstr "批量删除"
+
+#: admin/admin.py:1036
+msgid "Delete"
+msgstr "删除"
+
+#: admin/admin.py:1037
+#, python-format
+msgid "Are you sure you want to delete row ${%s}?"
+msgstr "你确定要删除行${%s}?"
+
+#: admin/admin.py:1047
+msgid "Are you sure you want to delete the selected rows?"
+msgstr "你确定要批量删除选中行吗?"
+
+#: admin/admin.py:1194
+msgid "Custom form actions"
+msgstr "自定义表单动作"
+
+#: admin/parser.py:183
+msgid "YES"
+msgstr "是"
+
+#: admin/parser.py:184
+msgid "NO"
+msgstr "否"
+
+#: admin/site.py:50
+msgid "Home"
 msgstr "首页"
```

### Comparing `fastapi_amis_admin-0.6.3/fastapi_amis_admin/models/enums.py` & `fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/models/enums.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,86 +1,86 @@
-import enum
-
-__all__ = ["Choices", "IntegerChoices", "TextChoices"]
-
-
-class ChoicesMeta(enum.EnumMeta):
-    """A metaclass for creating a enum choices."""
-
-    def __new__(metacls, classname, bases, classdict, **kwds):
-        labels = []
-        for key in classdict._member_names:
-            value = classdict[key]
-            if isinstance(value, (list, tuple)) and len(value) > 1 and isinstance(value[-1], (Promise, str)):
-                *value, label = value
-                value = tuple(value)
-            else:
-                label = key.replace("_", " ").title()
-            labels.append(label)
-            # Use dict.__setitem__() to suppress defenses against double
-            # assignment in enum's classdict.
-            dict.__setitem__(classdict, key, value)
-        cls = super().__new__(metacls, classname, bases, classdict, **kwds)
-        cls._value2label_map_ = dict(zip(cls._value2member_map_, labels))
-        # Add a label property to instances of enum which uses the enum member
-        # that is passed in as "self" as the value to use when looking up the
-        # label in the choices.
-        cls.label = property(lambda self: cls._value2label_map_.get(self.value))
-        cls.do_not_call_in_templates = True
-        return enum.unique(cls)
-
-    def __contains__(cls, member):
-        if not isinstance(member, enum.Enum):
-            # Allow non-enums to match against member values.
-            return any(x.value == member for x in cls)
-        return super().__contains__(member)
-
-    @property
-    def names(cls):
-        empty = ["__empty__"] if hasattr(cls, "__empty__") else []
-        return empty + [member.name for member in cls]
-
-    @property
-    def choices(cls):
-        empty = [(None, cls.__empty__)] if hasattr(cls, "__empty__") else []
-        return empty + [(member.value, member.label) for member in cls]
-
-    @property
-    def labels(cls):
-        return [label for _, label in cls.choices]
-
-    @property
-    def values(cls):
-        return [value for value, _ in cls.choices]
-
-
-class Choices(enum.Enum, metaclass=ChoicesMeta):
-    """Class for creating enumerated choices."""
-
-    def __str__(self):
-        """
-        Use value when cast to str, so that Choices set as model instance
-        attributes are rendered as expected in templates and similar contexts.
-        """
-        return str(self.value)
-
-
-class IntegerChoices(enum.IntEnum, Choices):
-    """Class for creating enumerated integer choices."""
-
-    pass
-
-
-class TextChoices(str, Choices):
-    """Class for creating enumerated string choices."""
-
-    def _generate_next_value_(name, start, count, last_values):
-        return name
-
-
-class Promise:
-    """
-    Base class for the proxy class created in the closure of the lazy function.
-    It's used to recognize promises in code.
-    """
-
-    pass
+import enum
+
+__all__ = ["Choices", "IntegerChoices", "TextChoices"]
+
+
+class ChoicesMeta(enum.EnumMeta):
+    """A metaclass for creating a enum choices."""
+
+    def __new__(metacls, classname, bases, classdict, **kwds):
+        labels = []
+        for key in classdict._member_names:
+            value = classdict[key]
+            if isinstance(value, (list, tuple)) and len(value) > 1 and isinstance(value[-1], (Promise, str)):
+                *value, label = value
+                value = tuple(value)
+            else:
+                label = key.replace("_", " ").title()
+            labels.append(label)
+            # Use dict.__setitem__() to suppress defenses against double
+            # assignment in enum's classdict.
+            dict.__setitem__(classdict, key, value)
+        cls = super().__new__(metacls, classname, bases, classdict, **kwds)
+        cls._value2label_map_ = dict(zip(cls._value2member_map_, labels))
+        # Add a label property to instances of enum which uses the enum member
+        # that is passed in as "self" as the value to use when looking up the
+        # label in the choices.
+        cls.label = property(lambda self: cls._value2label_map_.get(self.value))
+        cls.do_not_call_in_templates = True
+        return enum.unique(cls)
+
+    def __contains__(cls, member):
+        if not isinstance(member, enum.Enum):
+            # Allow non-enums to match against member values.
+            return any(x.value == member for x in cls)
+        return super().__contains__(member)
+
+    @property
+    def names(cls):
+        empty = ["__empty__"] if hasattr(cls, "__empty__") else []
+        return empty + [member.name for member in cls]
+
+    @property
+    def choices(cls):
+        empty = [(None, cls.__empty__)] if hasattr(cls, "__empty__") else []
+        return empty + [(member.value, member.label) for member in cls]
+
+    @property
+    def labels(cls):
+        return [label for _, label in cls.choices]
+
+    @property
+    def values(cls):
+        return [value for value, _ in cls.choices]
+
+
+class Choices(enum.Enum, metaclass=ChoicesMeta):
+    """Class for creating enumerated choices."""
+
+    def __str__(self):
+        """
+        Use value when cast to str, so that Choices set as model instance
+        attributes are rendered as expected in templates and similar contexts.
+        """
+        return str(self.value)
+
+
+class IntegerChoices(enum.IntEnum, Choices):
+    """Class for creating enumerated integer choices."""
+
+    pass
+
+
+class TextChoices(str, Choices):
+    """Class for creating enumerated string choices."""
+
+    def _generate_next_value_(name, start, count, last_values):
+        return name
+
+
+class Promise:
+    """
+    Base class for the proxy class created in the closure of the lazy function.
+    It's used to recognize promises in code.
+    """
+
+    pass
```

### Comparing `fastapi_amis_admin-0.6.3/fastapi_amis_admin/models/fields.py` & `fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/models/fields.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,84 +1,84 @@
-from typing import AbstractSet, Any, Callable, Dict, Mapping, Optional, Sequence, Union
-
-from pydantic.fields import Undefined, UndefinedType
-from pydantic.typing import NoArgAnyCallable
-from sqlalchemy import Column
-from sqlalchemy.orm import ColumnProperty
-from sqlmodel.main import FieldInfo
-
-from fastapi_amis_admin.amis import FormItem, TableColumn
-
-
-def Field(
-    default: Any = Undefined,
-    *,
-    default_factory: Optional[NoArgAnyCallable] = None,
-    alias: str = None,
-    title: str = None,
-    description: str = None,
-    exclude: Union[AbstractSet[Union[int, str]], Mapping[Union[int, str], Any], Any] = None,
-    include: Union[AbstractSet[Union[int, str]], Mapping[Union[int, str], Any], Any] = None,
-    const: bool = None,
-    gt: float = None,
-    ge: float = None,
-    lt: float = None,
-    le: float = None,
-    multiple_of: float = None,
-    min_items: int = None,
-    max_items: int = None,
-    min_length: int = None,
-    max_length: int = None,
-    allow_mutation: bool = True,
-    regex: str = None,
-    primary_key: bool = False,
-    foreign_key: Optional[Any] = None,
-    unique: bool = False,
-    nullable: Union[bool, UndefinedType] = Undefined,
-    index: Union[bool, UndefinedType] = Undefined,
-    sa_column: Union[Column, ColumnProperty, UndefinedType] = Undefined,
-    sa_column_args: Union[Sequence[Any], UndefinedType] = Undefined,
-    sa_column_kwargs: Union[Mapping[str, Any], UndefinedType] = Undefined,
-    schema_extra: Optional[Dict[str, Any]] = None,
-    amis_form_item: Union[FormItem, dict, str, Callable] = None,
-    amis_filter_item: Union[FormItem, dict, str, Callable] = None,
-    amis_table_column: Union[TableColumn, dict, str, Callable] = None,
-) -> FieldInfo:
-    current_schema_extra = schema_extra or {}
-    if amis_form_item:
-        current_schema_extra["amis_form_item"] = amis_form_item
-    if amis_filter_item:
-        current_schema_extra["amis_filter_item"] = amis_filter_item
-    if amis_table_column:
-        current_schema_extra["amis_table_column"] = amis_table_column
-    field_info = FieldInfo(
-        default,
-        default_factory=default_factory,
-        alias=alias,
-        title=title,
-        description=description,
-        exclude=exclude,
-        include=include,
-        const=const,
-        gt=gt,
-        ge=ge,
-        lt=lt,
-        le=le,
-        multiple_of=multiple_of,
-        min_items=min_items,
-        max_items=max_items,
-        min_length=min_length,
-        max_length=max_length,
-        allow_mutation=allow_mutation,
-        regex=regex,
-        primary_key=primary_key,
-        foreign_key=foreign_key,
-        unique=unique,
-        nullable=nullable,
-        index=index,
-        sa_column=sa_column,
-        sa_column_args=sa_column_args,
-        sa_column_kwargs=sa_column_kwargs,
-        **current_schema_extra,
-    )
-    field_info._validate()
-    return field_info
+from typing import AbstractSet, Any, Callable, Dict, Mapping, Optional, Sequence, Union
+
+from pydantic.fields import Undefined, UndefinedType
+from pydantic.typing import NoArgAnyCallable
+from sqlalchemy import Column
+from sqlalchemy.orm import ColumnProperty
+from sqlmodel.main import FieldInfo
+
+from fastapi_amis_admin.amis import FormItem, TableColumn
+
+
+def Field(
+    default: Any = Undefined,
+    *,
+    default_factory: Optional[NoArgAnyCallable] = None,
+    alias: str = None,
+    title: str = None,
+    description: str = None,
+    exclude: Union[AbstractSet[Union[int, str]], Mapping[Union[int, str], Any], Any] = None,
+    include: Union[AbstractSet[Union[int, str]], Mapping[Union[int, str], Any], Any] = None,
+    const: bool = None,
+    gt: float = None,
+    ge: float = None,
+    lt: float = None,
+    le: float = None,
+    multiple_of: float = None,
+    min_items: int = None,
+    max_items: int = None,
+    min_length: int = None,
+    max_length: int = None,
+    allow_mutation: bool = True,
+    regex: str = None,
+    primary_key: bool = False,
+    foreign_key: Optional[Any] = None,
+    unique: bool = False,
+    nullable: Union[bool, UndefinedType] = Undefined,
+    index: Union[bool, UndefinedType] = Undefined,
+    sa_column: Union[Column, ColumnProperty, UndefinedType] = Undefined,
+    sa_column_args: Union[Sequence[Any], UndefinedType] = Undefined,
+    sa_column_kwargs: Union[Mapping[str, Any], UndefinedType] = Undefined,
+    schema_extra: Optional[Dict[str, Any]] = None,
+    amis_form_item: Union[FormItem, dict, str, Callable] = None,
+    amis_filter_item: Union[FormItem, dict, str, Callable] = None,
+    amis_table_column: Union[TableColumn, dict, str, Callable] = None,
+) -> FieldInfo:
+    current_schema_extra = schema_extra or {}
+    if amis_form_item:
+        current_schema_extra["amis_form_item"] = amis_form_item
+    if amis_filter_item:
+        current_schema_extra["amis_filter_item"] = amis_filter_item
+    if amis_table_column:
+        current_schema_extra["amis_table_column"] = amis_table_column
+    field_info = FieldInfo(
+        default,
+        default_factory=default_factory,
+        alias=alias,
+        title=title,
+        description=description,
+        exclude=exclude,
+        include=include,
+        const=const,
+        gt=gt,
+        ge=ge,
+        lt=lt,
+        le=le,
+        multiple_of=multiple_of,
+        min_items=min_items,
+        max_items=max_items,
+        min_length=min_length,
+        max_length=max_length,
+        allow_mutation=allow_mutation,
+        regex=regex,
+        primary_key=primary_key,
+        foreign_key=foreign_key,
+        unique=unique,
+        nullable=nullable,
+        index=index,
+        sa_column=sa_column,
+        sa_column_args=sa_column_args,
+        sa_column_kwargs=sa_column_kwargs,
+        **current_schema_extra,
+    )
+    field_info._validate()
+    return field_info
```

### Comparing `fastapi_amis_admin-0.6.3/fastapi_amis_admin/utils/functools.py` & `fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/utils/functools.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-try:
-    from functools import cached_property
-except ImportError:
-    from threading import RLock
-
-    _NOT_FOUND = object()
-
-    class cached_property:  # noqa: E303
-        def __init__(self, func):
-            self.func = func
-            self.attrname = None
-            self.__doc__ = func.__doc__
-            self.lock = RLock()
-
-        def __set_name__(self, owner, name):
-            if self.attrname is None:
-                self.attrname = name
-            elif name != self.attrname:
-                raise TypeError(
-                    "Cannot assign the same cached_property to two different names " f"({self.attrname!r} and {name!r})."
-                )
-
-        def __get__(self, instance, owner=None):
-            if instance is None:
-                return self
-            if self.attrname is None:
-                raise TypeError("Cannot use cached_property instance without calling __set_name__ on it.")
-            try:
-                cache = instance.__dict__
-            except AttributeError:  # not all objects have __dict__ (e.g. class defines slots)
-                msg = f"No '__dict__' attribute on {type(instance).__name__!r} " f"instance to cache {self.attrname!r} property."
-                raise TypeError(msg) from None
-            val = cache.get(self.attrname, _NOT_FOUND)
-            if val is _NOT_FOUND:
-                with self.lock:
-                    # check if another thread filled cache while we awaited lock
-                    val = cache.get(self.attrname, _NOT_FOUND)
-                    if val is _NOT_FOUND:
-                        val = self.func(instance)
-                        try:
-                            cache[self.attrname] = val
-                        except TypeError:
-                            msg = (
-                                f"The '__dict__' attribute on {type(instance).__name__!r} instance "
-                                f"does not support item assignment for caching {self.attrname!r} property."
-                            )
-                            raise TypeError(msg) from None
-            return val
+try:
+    from functools import cached_property
+except ImportError:
+    from threading import RLock
+
+    _NOT_FOUND = object()
+
+    class cached_property:  # noqa: E303
+        def __init__(self, func):
+            self.func = func
+            self.attrname = None
+            self.__doc__ = func.__doc__
+            self.lock = RLock()
+
+        def __set_name__(self, owner, name):
+            if self.attrname is None:
+                self.attrname = name
+            elif name != self.attrname:
+                raise TypeError(
+                    "Cannot assign the same cached_property to two different names " f"({self.attrname!r} and {name!r})."
+                )
+
+        def __get__(self, instance, owner=None):
+            if instance is None:
+                return self
+            if self.attrname is None:
+                raise TypeError("Cannot use cached_property instance without calling __set_name__ on it.")
+            try:
+                cache = instance.__dict__
+            except AttributeError:  # not all objects have __dict__ (e.g. class defines slots)
+                msg = f"No '__dict__' attribute on {type(instance).__name__!r} " f"instance to cache {self.attrname!r} property."
+                raise TypeError(msg) from None
+            val = cache.get(self.attrname, _NOT_FOUND)
+            if val is _NOT_FOUND:
+                with self.lock:
+                    # check if another thread filled cache while we awaited lock
+                    val = cache.get(self.attrname, _NOT_FOUND)
+                    if val is _NOT_FOUND:
+                        val = self.func(instance)
+                        try:
+                            cache[self.attrname] = val
+                        except TypeError:
+                            msg = (
+                                f"The '__dict__' attribute on {type(instance).__name__!r} instance "
+                                f"does not support item assignment for caching {self.attrname!r} property."
+                            )
+                            raise TypeError(msg) from None
+            return val
```

### Comparing `fastapi_amis_admin-0.6.3/fastapi_amis_admin/utils/pydantic.py` & `fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/utils/pydantic.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,237 +1,237 @@
-from enum import Enum
-from typing import Any, Dict, Optional, Sequence, Set, Type, Union
-
-from fastapi._compat import (  # noqa: F401
-    ModelField,
-    Undefined,
-    field_annotation_is_scalar_sequence,
-    sequence_annotation_to_type,
-)
-from fastapi.utils import create_cloned_field
-from pydantic import BaseModel, ConfigDict, create_model
-from pydantic.version import VERSION as PYDANTIC_VERSION
-from typing_extensions import Annotated, get_args, get_origin
-
-PYDANTIC_V2 = PYDANTIC_VERSION.startswith("2.")
-# todo: Deprecated `dict`,`json`,`from_orm`,`parse_obj` methods in pydantic v2
-if PYDANTIC_V2:
-    from pydantic._internal._utils import ValueItems  # noqa: F401
-    from pydantic.v1.datetime_parse import parse_date, parse_datetime  # noqa: F401
-    from pydantic.v1.utils import lenient_issubclass
-    from pydantic_settings import BaseSettings  # noqa: F401
-
-    GenericModel = BaseModel
-    from pydantic import model_validator
-    from pydantic.v1.typing import is_literal_type, is_none_type, is_union
-
-    class AllowExtraModelMixin(BaseModel):
-        model_config = ConfigDict(extra="allow")
-
-    class ORMModelMixin(BaseModel):
-        model_config = ConfigDict(from_attributes=True)
-
-    def create_model_by_fields(
-        name: str,
-        fields: Sequence[ModelField],
-        *,
-        set_none: bool = False,
-        extra: str = "ignore",
-        **kwargs,
-    ) -> Type[BaseModel]:
-        if kwargs.pop("orm_mode", False):
-            kwargs.setdefault("from_attributes", True)
-        __config__ = marge_model_config(AllowExtraModelMixin, {"extra": extra, **kwargs})
-        __validators__ = None
-
-        if set_none:
-            __validators__ = {"root_validator_skip_blank": model_validator(mode="before")(root_validator_skip_blank)}
-            for f in fields:
-                f.field_info.annotation = Optional[f.field_info.annotation]
-                f.field_info.default = None
-        field_params = {f.name: (f.field_info.annotation, f.field_info) for f in fields}
-        model: Type[BaseModel] = create_model(name, __config__=__config__, __validators__=__validators__, **field_params)
-        return model
-
-    def model_update_forward_refs(model: Type[BaseModel]):
-        model.model_rebuild()
-
-    def field_json_schema_extra(field: ModelField) -> Dict[str, Any]:
-        return field.field_info.json_schema_extra or {}
-
-    def field_outer_type(field: ModelField) -> Any:
-        return field.field_info.annotation
-
-    def field_allow_none(field: ModelField) -> bool:
-        if is_union(field.field_info.annotation):
-            for t in get_args(field.field_info.annotation):
-                if is_none_type(t):
-                    return True
-        return False
-
-    def model_fields(model: Type[BaseModel]) -> Dict[str, ModelField]:
-        fields = {}
-        for field_name, field in model.model_fields.items():
-            fields[field_name] = ModelField(field_info=field, name=field_name)
-        return fields
-
-    def model_config(model: Type[BaseModel]) -> Union[type, Dict[str, Any]]:
-        return model.model_config
-
-    def marge_model_config(model: Type[BaseModel], update: Dict[str, Any]) -> Union[type, Dict[str, Any]]:
-        return {**model.model_config, **update}
-
-    def model_config_attr(model: Type[BaseModel], name: str, default: Any = None) -> Any:
-        return model.model_config.get(name, default)
-
-else:
-    from pydantic import (
-        BaseSettings,  # noqa: F401
-        root_validator,
-    )
-    from pydantic.datetime_parse import parse_date, parse_datetime  # noqa: F401
-    from pydantic.fields import ModelField
-    from pydantic.generics import GenericModel  # noqa: F401
-    from pydantic.typing import is_literal_type, is_none_type, is_union
-    from pydantic.utils import (
-        ValueItems,  # noqa: F401
-        lenient_issubclass,
-    )
-
-    class AllowExtraModelMixin(BaseModel):
-        class Config:
-            extra = "allow"
-
-    class ORMModelMixin(BaseModel):
-        class Config:
-            orm_mode = True
-
-    def create_model_by_fields(
-        name: str,
-        fields: Sequence[ModelField],
-        *,
-        set_none: bool = False,
-        extra: str = "ignore",
-        **kwargs,
-    ) -> Type[BaseModel]:
-        __config__ = marge_model_config(AllowExtraModelMixin, {"extra": extra, **kwargs})
-        __validators__ = None
-        if set_none:
-            __validators__ = {"root_validator_skip_blank": root_validator(pre=True, allow_reuse=True)(root_validator_skip_blank)}
-            for f in fields:
-                f.required = False
-                f.allow_none = True
-        model = create_model(name, __config__=__config__, __validators__=__validators__)  # type: ignore
-        model.__fields__ = {f.name: f for f in fields}
-        return model
-
-    def model_update_forward_refs(model: Type[BaseModel]):
-        model.update_forward_refs()
-
-    def field_json_schema_extra(field: ModelField) -> Dict[str, Any]:
-        return field.field_info.extra or {}
-
-    def field_outer_type(field: ModelField) -> Any:
-        return field.outer_type_
-
-    def field_allow_none(field: ModelField) -> bool:
-        return field.allow_none
-
-    def model_fields(model: Type[BaseModel]) -> Dict[str, ModelField]:
-        return model.__fields__
-
-    def model_config(model: Type[BaseModel]) -> Union[type, Dict[str, Any]]:
-        return model.Config
-
-    def marge_model_config(model: Type[BaseModel], update: Dict[str, Any]) -> Union[type, Dict[str, Any]]:
-        return type("Config", (model.Config,), update)
-
-    def model_config_attr(model: Type[BaseModel], name: str, default: Any = None) -> Any:
-        return getattr(model.Config, name, default)
-
-
-def annotation_outer_type(tp: Any) -> Any:
-    """Get the base type of the annotation."""
-    if tp is Ellipsis:
-        return Any
-    origin = get_origin(tp)
-    if origin is None:
-        return tp
-    elif is_union(origin) or origin is Annotated:
-        pass
-    elif origin in sequence_annotation_to_type:
-        return sequence_annotation_to_type[origin]
-    elif origin in {Dict, dict}:
-        return dict
-    elif lenient_issubclass(origin, BaseModel):
-        return origin
-    args = get_args(tp)
-    for arg in args:
-        if is_literal_type(tp):
-            arg = type(arg)
-        if is_none_type(arg):
-            continue
-        return annotation_outer_type(arg)
-    return tp
-
-
-def scalar_sequence_inner_type(tp: Any) -> Any:
-    origin = get_origin(tp)
-    if origin is None:
-        return Any
-    elif is_union(origin) or origin is Annotated:  # Return the type of the first element
-        return scalar_sequence_inner_type(get_args(tp)[0])
-    args = get_args(tp)
-    return annotation_outer_type(args[0]) if args else Any
-
-
-def validator_skip_blank(v, type_: type):
-    if isinstance(v, str):
-        if not v:
-            if issubclass(type_, Enum):
-                if "" not in type_._value2member_map_:
-                    return None
-                return ""
-            if not issubclass(type_, str):
-                return None
-            return ""
-        if issubclass(type_, int):
-            v = int(v)
-    elif isinstance(v, int) and issubclass(type_, str):
-        v = str(v)
-    return v
-
-
-def root_validator_skip_blank(cls, values: Dict[str, Any]):
-    fields = model_fields(cls)
-
-    def get_field_by_alias(alias: str) -> Optional[ModelField]:
-        for f in fields.values():
-            if f.alias == alias:
-                return f
-        return None
-
-    for k, v in values.items():
-        field = get_field_by_alias(k)
-        if field:
-            values[k] = validator_skip_blank(v, annotation_outer_type(field.type_))
-    return values
-
-
-def create_model_by_model(
-    model: Type[BaseModel],
-    name: str,
-    *,
-    include: Set[str] = None,
-    exclude: Set[str] = None,
-    set_none: bool = False,
-    **kwargs,
-) -> Type[BaseModel]:
-    """Create a new model by the BaseModel."""
-    fields = model_fields(model)
-    keys = set(fields.keys())
-    if include:
-        keys &= include
-    if exclude:
-        keys -= exclude
-    fields = {name: create_cloned_field(field) for name, field in fields.items() if name in keys}
-    return create_model_by_fields(name, list(fields.values()), set_none=set_none, **kwargs)
+from enum import Enum
+from typing import Any, Dict, Optional, Sequence, Set, Type, Union
+
+from fastapi._compat import (  # noqa: F401
+    ModelField,
+    Undefined,
+    field_annotation_is_scalar_sequence,
+    sequence_annotation_to_type,
+)
+from fastapi.utils import create_cloned_field
+from pydantic import BaseModel, ConfigDict, create_model
+from pydantic.version import VERSION as PYDANTIC_VERSION
+from typing_extensions import Annotated, get_args, get_origin
+
+PYDANTIC_V2 = PYDANTIC_VERSION.startswith("2.")
+# todo: Deprecated `dict`,`json`,`from_orm`,`parse_obj` methods in pydantic v2
+if PYDANTIC_V2:
+    from pydantic._internal._utils import ValueItems  # noqa: F401
+    from pydantic.v1.datetime_parse import parse_date, parse_datetime  # noqa: F401
+    from pydantic.v1.utils import lenient_issubclass
+    from pydantic_settings import BaseSettings  # noqa: F401
+
+    GenericModel = BaseModel
+    from pydantic import model_validator
+    from pydantic.v1.typing import is_literal_type, is_none_type, is_union
+
+    class AllowExtraModelMixin(BaseModel):
+        model_config = ConfigDict(extra="allow")
+
+    class ORMModelMixin(BaseModel):
+        model_config = ConfigDict(from_attributes=True)
+
+    def create_model_by_fields(
+        name: str,
+        fields: Sequence[ModelField],
+        *,
+        set_none: bool = False,
+        extra: str = "ignore",
+        **kwargs,
+    ) -> Type[BaseModel]:
+        if kwargs.pop("orm_mode", False):
+            kwargs.setdefault("from_attributes", True)
+        __config__ = marge_model_config(AllowExtraModelMixin, {"extra": extra, **kwargs})
+        __validators__ = None
+
+        if set_none:
+            __validators__ = {"root_validator_skip_blank": model_validator(mode="before")(root_validator_skip_blank)}
+            for f in fields:
+                f.field_info.annotation = Optional[f.field_info.annotation]
+                f.field_info.default = None
+        field_params = {f.name: (f.field_info.annotation, f.field_info) for f in fields}
+        model: Type[BaseModel] = create_model(name, __config__=__config__, __validators__=__validators__, **field_params)
+        return model
+
+    def model_update_forward_refs(model: Type[BaseModel]):
+        model.model_rebuild()
+
+    def field_json_schema_extra(field: ModelField) -> Dict[str, Any]:
+        return field.field_info.json_schema_extra or {}
+
+    def field_outer_type(field: ModelField) -> Any:
+        return field.field_info.annotation
+
+    def field_allow_none(field: ModelField) -> bool:
+        if is_union(field.field_info.annotation):
+            for t in get_args(field.field_info.annotation):
+                if is_none_type(t):
+                    return True
+        return False
+
+    def model_fields(model: Type[BaseModel]) -> Dict[str, ModelField]:
+        fields = {}
+        for field_name, field in model.model_fields.items():
+            fields[field_name] = ModelField(field_info=field, name=field_name)
+        return fields
+
+    def model_config(model: Type[BaseModel]) -> Union[type, Dict[str, Any]]:
+        return model.model_config
+
+    def marge_model_config(model: Type[BaseModel], update: Dict[str, Any]) -> Union[type, Dict[str, Any]]:
+        return {**model.model_config, **update}
+
+    def model_config_attr(model: Type[BaseModel], name: str, default: Any = None) -> Any:
+        return model.model_config.get(name, default)
+
+else:
+    from pydantic import (
+        BaseSettings,  # noqa: F401
+        root_validator,
+    )
+    from pydantic.datetime_parse import parse_date, parse_datetime  # noqa: F401
+    from pydantic.fields import ModelField
+    from pydantic.generics import GenericModel  # noqa: F401
+    from pydantic.typing import is_literal_type, is_none_type, is_union
+    from pydantic.utils import (
+        ValueItems,  # noqa: F401
+        lenient_issubclass,
+    )
+
+    class AllowExtraModelMixin(BaseModel):
+        class Config:
+            extra = "allow"
+
+    class ORMModelMixin(BaseModel):
+        class Config:
+            orm_mode = True
+
+    def create_model_by_fields(
+        name: str,
+        fields: Sequence[ModelField],
+        *,
+        set_none: bool = False,
+        extra: str = "ignore",
+        **kwargs,
+    ) -> Type[BaseModel]:
+        __config__ = marge_model_config(AllowExtraModelMixin, {"extra": extra, **kwargs})
+        __validators__ = None
+        if set_none:
+            __validators__ = {"root_validator_skip_blank": root_validator(pre=True, allow_reuse=True)(root_validator_skip_blank)}
+            for f in fields:
+                f.required = False
+                f.allow_none = True
+        model = create_model(name, __config__=__config__, __validators__=__validators__)  # type: ignore
+        model.__fields__ = {f.name: f for f in fields}
+        return model
+
+    def model_update_forward_refs(model: Type[BaseModel]):
+        model.update_forward_refs()
+
+    def field_json_schema_extra(field: ModelField) -> Dict[str, Any]:
+        return field.field_info.extra or {}
+
+    def field_outer_type(field: ModelField) -> Any:
+        return field.outer_type_
+
+    def field_allow_none(field: ModelField) -> bool:
+        return field.allow_none
+
+    def model_fields(model: Type[BaseModel]) -> Dict[str, ModelField]:
+        return model.__fields__
+
+    def model_config(model: Type[BaseModel]) -> Union[type, Dict[str, Any]]:
+        return model.Config
+
+    def marge_model_config(model: Type[BaseModel], update: Dict[str, Any]) -> Union[type, Dict[str, Any]]:
+        return type("Config", (model.Config,), update)
+
+    def model_config_attr(model: Type[BaseModel], name: str, default: Any = None) -> Any:
+        return getattr(model.Config, name, default)
+
+
+def annotation_outer_type(tp: Any) -> Any:
+    """Get the base type of the annotation."""
+    if tp is Ellipsis:
+        return Any
+    origin = get_origin(tp)
+    if origin is None:
+        return tp
+    elif is_union(origin) or origin is Annotated:
+        pass
+    elif origin in sequence_annotation_to_type:
+        return sequence_annotation_to_type[origin]
+    elif origin in {Dict, dict}:
+        return dict
+    elif lenient_issubclass(origin, BaseModel):
+        return origin
+    args = get_args(tp)
+    for arg in args:
+        if is_literal_type(tp):
+            arg = type(arg)
+        if is_none_type(arg):
+            continue
+        return annotation_outer_type(arg)
+    return tp
+
+
+def scalar_sequence_inner_type(tp: Any) -> Any:
+    origin = get_origin(tp)
+    if origin is None:
+        return Any
+    elif is_union(origin) or origin is Annotated:  # Return the type of the first element
+        return scalar_sequence_inner_type(get_args(tp)[0])
+    args = get_args(tp)
+    return annotation_outer_type(args[0]) if args else Any
+
+
+def validator_skip_blank(v, type_: type):
+    if isinstance(v, str):
+        if not v:
+            if issubclass(type_, Enum):
+                if "" not in type_._value2member_map_:
+                    return None
+                return ""
+            if not issubclass(type_, str):
+                return None
+            return ""
+        if issubclass(type_, int):
+            v = int(v)
+    elif isinstance(v, int) and issubclass(type_, str):
+        v = str(v)
+    return v
+
+
+def root_validator_skip_blank(cls, values: Dict[str, Any]):
+    fields = model_fields(cls)
+
+    def get_field_by_alias(alias: str) -> Optional[ModelField]:
+        for f in fields.values():
+            if f.alias == alias:
+                return f
+        return None
+
+    for k, v in values.items():
+        field = get_field_by_alias(k)
+        if field:
+            values[k] = validator_skip_blank(v, annotation_outer_type(field.type_))
+    return values
+
+
+def create_model_by_model(
+    model: Type[BaseModel],
+    name: str,
+    *,
+    include: Set[str] = None,
+    exclude: Set[str] = None,
+    set_none: bool = False,
+    **kwargs,
+) -> Type[BaseModel]:
+    """Create a new model by the BaseModel."""
+    fields = model_fields(model)
+    keys = set(fields.keys())
+    if include:
+        keys &= include
+    if exclude:
+        keys -= exclude
+    fields = {name: create_cloned_field(field) for name, field in fields.items() if name in keys}
+    return create_model_by_fields(name, list(fields.values()), set_none=set_none, **kwargs)
```

### Comparing `fastapi_amis_admin-0.6.3/fastapi_amis_admin/utils/translation.py` & `fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/utils/translation.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-import gc
-import locale
-import os
-from functools import lru_cache
-from gettext import GNUTranslations
-from typing import Dict, Set
-
-
-class I18N:
-    def __init__(self):
-        self._locales: Dict[str, Set[GNUTranslations]] = {}
-        self._language: str = self.set_language()
-
-    def load_translations(self, translations: Dict[str, GNUTranslations]):
-        for language, trans in translations.items():
-            if language in self._locales:
-                self._locales[language].add(trans)
-            else:
-                self._locales[language] = {trans}
-
-    def set_language(self, language: str = None) -> str:
-        """
-        Set the i18n localization language. If it is empty, try to read the environment variable `LANGUAGE`/`LANG`,
-        the system default language, in turn.
-        :param language: the language to try to set
-        :return: the language after the successful setting
-        """
-        language = language or os.getenv("LANGUAGE") or os.getenv("LANG") or locale.getlocale()[0] or "en_US"
-        self._language = "zh_CN" if language.lower().startswith(("zh", "chinese")) else language
-        I18N.gettext.cache_clear()  # clear cache after language has changed
-        gc.collect()
-        return self._language
-
-    def get_language(self):
-        return self._language
-
-    @lru_cache()  # noqa: B019
-    def gettext(self, value: str, language: str = None) -> str:
-        language = language or self._language
-        if language in self._locales:
-            for trans in self._locales[language]:
-                # noinspection PyProtectedMember
-                if value in trans._catalog:  # type: ignore
-                    value = trans.gettext(value)
-        return value
-
-    def __call__(self, value, language: str = None) -> str:
-        return self.gettext(str(value), language)
-
-
-i18n = I18N()
+import gc
+import locale
+import os
+from functools import lru_cache
+from gettext import GNUTranslations
+from typing import Dict, Set
+
+
+class I18N:
+    def __init__(self):
+        self._locales: Dict[str, Set[GNUTranslations]] = {}
+        self._language: str = self.set_language()
+
+    def load_translations(self, translations: Dict[str, GNUTranslations]):
+        for language, trans in translations.items():
+            if language in self._locales:
+                self._locales[language].add(trans)
+            else:
+                self._locales[language] = {trans}
+
+    def set_language(self, language: str = None) -> str:
+        """
+        Set the i18n localization language. If it is empty, try to read the environment variable `LANGUAGE`/`LANG`,
+        the system default language, in turn.
+        :param language: the language to try to set
+        :return: the language after the successful setting
+        """
+        language = language or os.getenv("LANGUAGE") or os.getenv("LANG") or locale.getlocale()[0] or "en_US"
+        self._language = "zh_CN" if language.lower().startswith(("zh", "chinese")) else language
+        I18N.gettext.cache_clear()  # clear cache after language has changed
+        gc.collect()
+        return self._language
+
+    def get_language(self):
+        return self._language
+
+    @lru_cache()  # noqa: B019
+    def gettext(self, value: str, language: str = None) -> str:
+        language = language or self._language
+        if language in self._locales:
+            for trans in self._locales[language]:
+                # noinspection PyProtectedMember
+                if value in trans._catalog:  # type: ignore
+                    value = trans.gettext(value)
+        return value
+
+    def __call__(self, value, language: str = None) -> str:
+        return self.gettext(str(value), language)
+
+
+i18n = I18N()
```

### Comparing `fastapi_amis_admin-0.6.3/pyproject.toml` & `fastapi_amis_admin-0.6.3a1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,117 +1,116 @@
-[build-system]
-requires = ["flit_core >=3.2,<4"]
-build-backend = "flit_core.buildapi"
-
-[project]
-name = "fastapi_amis_admin"
-authors = [
-    { name = "Atomi", email = "1456417373@qq.com" },
-]
-maintainers = [
-    { name = "Atomi", email = "1456417373@qq.com" },
-]
-description = "FastAPI-Amis-Admin is a high-performance, efficient and easily extensible FastAPI admin framework. Inspired by Django-admin, and has as many powerful functions as Django-admin. "
-readme = "README.md"
-requires-python = ">=3.7"
-dynamic = ["version"]
-keywords = [
-    "fastapi",
-    "fastapi-admin",
-    "fastapi-amis-admin",
-    "django-admin",
-    "sqlmodel",
-    "sqlalchemy",
-]
-classifiers = [
-    "Framework :: FastAPI",
-    "Environment :: Web Environment",
-    "Topic :: System :: Systems Administration",
-    "License :: OSI Approved :: Apache Software License",
-    "Operating System :: OS Independent",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-]
-dependencies = [
-    "fastapi>=0.100.0",
-    "pydantic>1.7.4",
-    "sqlalchemy>=1.4.0",
-    "python-multipart>=0.0.5",
-    "sqlalchemy-database>=0.1.0,<0.2.0",
-    "aiofiles>=0.17.0",
-    "lazy-object-proxy>=1.9.0",
-]
-
-
-[project.urls]
-Documentation = "http://docs.amis.work/"
-Source = "https://github.com/amisadmin/fastapi_amis_admin"
-
-[project.optional-dependencies]
-sqlmodel = [
-    "sqlmodel>=0.0.7",
-]
-standard = [
-    "uvicorn[standard] >=0.19.0,<1.0",
-    "fastapi-amis-admin-cli>=0.1.3,<0.2.0",
-]
-test = [
-    "uvicorn[standard] >=0.19.0,<1.0",
-    "fastapi-amis-admin-cli>=0.1.3,<0.2.0",
-    "pytest >=6.2.4",
-    "aiosqlite>=0.15.0",
-    "pytest-asyncio>=0.17",
-    "httpx>=0.24.0,<1.0",
-    "jinja2 >=2.11.2,<4.0.0",
-    "ujson>=4.0.1",
-    "requests>=2.28.1",
-    "sqlmodel>=0.0.7",
-]
-dev = [
-    "pre-commit>=2.20.0",
-    "ruff>=0.0.261",
-]
-cli = [
-    "fastapi-amis-admin-cli>=0.1.3,<0.2.0",
-]
-
-# pytest
-[tool.pytest.ini_options]
-minversion = "6.0"
-testpaths = [
-    "tests",
-]
-# pytest-asyncio
-asyncio_mode = "auto"
-
-[tool.black]
-line-length = 130
-include = '\.pyi?$'
-
-[tool.ruff]
-select = [
-    "E",  # pycodestyle errors
-    "W",  # pycodestyle warnings
-    "F",  # pyflakes
-    "I",  # isort
-    "C",  # flake8-comprehensions
-    "B",  # flake8-bugbear
-]
-ignore = [
-    "B008",  # do not perform function calls in argument defaults
-    "C901",  # too complex
-]
-# Same as Black.
-line-length = 130
-
-[tool.ruff.per-file-ignores]
-"__init__.py" = ["F401"]
-
-[tool.pdm]
-[tool.pdm.dev-dependencies]
-[tool.pdm.scripts]
-lint = "pre-commit run --all-files"
+[build-system]
+requires = ["flit_core >=3.2,<4"]
+build-backend = "flit_core.buildapi"
+
+[project]
+name = "fastapi_amis_admin"
+authors = [
+    { name = "Atomi", email = "1456417373@qq.com" },
+]
+maintainers = [
+    { name = "Atomi", email = "1456417373@qq.com" },
+]
+description = "FastAPI-Amis-Admin is a high-performance, efficient and easily extensible FastAPI admin framework. Inspired by Django-admin, and has as many powerful functions as Django-admin. "
+readme = "README.md"
+requires-python = ">=3.7"
+dynamic = ["version"]
+keywords = [
+    "fastapi",
+    "fastapi-admin",
+    "fastapi-amis-admin",
+    "django-admin",
+    "sqlmodel",
+    "sqlalchemy",
+]
+classifiers = [
+    "Framework :: FastAPI",
+    "Environment :: Web Environment",
+    "Topic :: System :: Systems Administration",
+    "License :: OSI Approved :: Apache Software License",
+    "Operating System :: OS Independent",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+]
+dependencies = [
+    "fastapi>=0.100.0",
+    "pydantic>1.7.4",
+    "sqlalchemy>=1.4.0",
+    "python-multipart>=0.0.5",
+    "sqlalchemy-database>=0.1.0,<0.2.0",
+    "aiofiles>=0.17.0",
+]
+
+
+[project.urls]
+Documentation = "http://docs.amis.work/"
+Source = "https://github.com/amisadmin/fastapi_amis_admin"
+
+[project.optional-dependencies]
+sqlmodel = [
+    "sqlmodel>=0.0.7",
+]
+standard = [
+    "uvicorn[standard] >=0.19.0,<1.0",
+    "fastapi-amis-admin-cli>=0.1.3,<0.2.0",
+]
+test = [
+    "uvicorn[standard] >=0.19.0,<1.0",
+    "fastapi-amis-admin-cli>=0.1.3,<0.2.0",
+    "pytest >=6.2.4",
+    "aiosqlite>=0.15.0",
+    "pytest-asyncio>=0.17",
+    "httpx>=0.24.0,<1.0",
+    "jinja2 >=2.11.2,<4.0.0",
+    "ujson>=4.0.1",
+    "requests>=2.28.1",
+    "sqlmodel>=0.0.7",
+]
+dev = [
+    "pre-commit>=2.20.0",
+    "ruff>=0.0.261",
+]
+cli = [
+    "fastapi-amis-admin-cli>=0.1.3,<0.2.0",
+]
+
+# pytest
+[tool.pytest.ini_options]
+minversion = "6.0"
+testpaths = [
+    "tests",
+]
+# pytest-asyncio
+asyncio_mode = "auto"
+
+[tool.black]
+line-length = 130
+include = '\.pyi?$'
+
+[tool.ruff]
+select = [
+    "E",  # pycodestyle errors
+    "W",  # pycodestyle warnings
+    "F",  # pyflakes
+    "I",  # isort
+    "C",  # flake8-comprehensions
+    "B",  # flake8-bugbear
+]
+ignore = [
+    "B008",  # do not perform function calls in argument defaults
+    "C901",  # too complex
+]
+# Same as Black.
+line-length = 130
+
+[tool.ruff.per-file-ignores]
+"__init__.py" = ["F401"]
+
+[tool.pdm]
+[tool.pdm.dev-dependencies]
+[tool.pdm.scripts]
+lint = "pre-commit run --all-files"
 test= "pytest"
```

