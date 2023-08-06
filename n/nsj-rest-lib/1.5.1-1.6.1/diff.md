# Comparing `tmp/nsj_rest_lib-1.5.1.tar.gz` & `tmp/nsj_rest_lib-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsj_rest_lib-1.5.1.tar", last modified: Wed Aug  2 23:57:36 2023, max compression
+gzip compressed data, was "nsj_rest_lib-1.6.1.tar", last modified: Sun Aug  6 01:08:01 2023, max compression
```

## Comparing `nsj_rest_lib-1.5.1.tar` & `nsj_rest_lib-1.6.1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-08-02 23:57:36.385750 nsj_rest_lib-1.5.1/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      743 2023-08-02 23:57:36.385750 nsj_rest_lib-1.5.1/PKG-INFO
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      130 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/README.md
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      103 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/pyproject.toml
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      888 2023-08-02 23:57:36.385750 nsj_rest_lib-1.5.1/setup.cfg
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-08-02 23:57:36.381750 nsj_rest_lib-1.5.1/src/
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-08-02 23:57:36.381750 nsj_rest_lib-1.5.1/src/nsj_rest_lib/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/__init__.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-08-02 23:57:36.381750 nsj_rest_lib-1.5.1/src/nsj_rest_lib/controller/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/controller/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)       74 2023-07-22 20:03:52.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/controller/constants.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)       75 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/controller/controller_util.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     3298 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/controller/delete_route.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      944 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/controller/funtion_route_wrapper.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     3907 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/controller/get_route.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4590 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/controller/list_route.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4351 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/controller/patch_route.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     3931 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/controller/post_route.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4341 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/controller/put_route.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4664 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/controller/route_base.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-08-02 23:57:36.385750 nsj_rest_lib-1.5.1/src/nsj_rest_lib/dao/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/dao/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)    21249 2023-07-31 18:42:01.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/dao/dao_base.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     1235 2023-08-02 23:56:53.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/db_pool_config.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-08-02 23:57:36.385750 nsj_rest_lib-1.5.1/src/nsj_rest_lib/decorator/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/decorator/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4737 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/decorator/dto.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-08-02 23:57:36.385750 nsj_rest_lib-1.5.1/src/nsj_rest_lib/descriptor/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/descriptor/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      418 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/descriptor/conjunto_type.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)    13146 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/descriptor/dto_field.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     7563 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/descriptor/dto_field_validators.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     5408 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/descriptor/dto_list_field.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      320 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/descriptor/filter_operator.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     2295 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/doc_route_generator.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-08-02 23:57:36.385750 nsj_rest_lib-1.5.1/src/nsj_rest_lib/dto/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/dto/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     7760 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/dto/dto_base.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-08-02 23:57:36.385750 nsj_rest_lib-1.5.1/src/nsj_rest_lib/entity/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/entity/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      710 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/entity/entity_base.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      322 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/entity/filter.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      483 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/exception.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     2856 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/healthcheck_config.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      825 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/injector_factory_base.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-08-02 23:57:36.385750 nsj_rest_lib-1.5.1/src/nsj_rest_lib/service/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/service/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)    24142 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/service/service_base.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      707 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/settings.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-08-02 23:57:36.385750 nsj_rest_lib-1.5.1/src/nsj_rest_lib/validator/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/validator/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4196 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/validator/cpf_cnpj.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      527 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/validator/validate_data.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-08-02 23:57:36.381750 nsj_rest_lib-1.5.1/src/nsj_rest_lib.egg-info/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      743 2023-08-02 23:57:36.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib.egg-info/PKG-INFO
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     1738 2023-08-02 23:57:36.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        1 2023-08-02 23:57:36.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      113 2023-08-02 23:57:36.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib.egg-info/requires.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)       13 2023-08-02 23:57:36.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib.egg-info/top_level.txt
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-08-06 01:08:01.919211 nsj_rest_lib-1.6.1/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      743 2023-08-06 01:08:01.919211 nsj_rest_lib-1.6.1/PKG-INFO
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      130 2023-07-21 15:01:40.000000 nsj_rest_lib-1.6.1/README.md
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      103 2023-07-21 15:01:40.000000 nsj_rest_lib-1.6.1/pyproject.toml
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      888 2023-08-06 01:08:01.919211 nsj_rest_lib-1.6.1/setup.cfg
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-08-06 01:08:01.911211 nsj_rest_lib-1.6.1/src/
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-08-06 01:08:01.915211 nsj_rest_lib-1.6.1/src/nsj_rest_lib/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-1.6.1/src/nsj_rest_lib/__init__.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-08-06 01:08:01.915211 nsj_rest_lib-1.6.1/src/nsj_rest_lib/controller/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-1.6.1/src/nsj_rest_lib/controller/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)       74 2023-07-22 20:03:52.000000 nsj_rest_lib-1.6.1/src/nsj_rest_lib/controller/constants.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)       75 2023-07-21 15:01:40.000000 nsj_rest_lib-1.6.1/src/nsj_rest_lib/controller/controller_util.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     3298 2023-07-21 15:01:40.000000 nsj_rest_lib-1.6.1/src/nsj_rest_lib/controller/delete_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      944 2023-07-21 15:01:40.000000 nsj_rest_lib-1.6.1/src/nsj_rest_lib/controller/funtion_route_wrapper.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     3907 2023-07-21 15:01:40.000000 nsj_rest_lib-1.6.1/src/nsj_rest_lib/controller/get_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4590 2023-07-21 15:01:40.000000 nsj_rest_lib-1.6.1/src/nsj_rest_lib/controller/list_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4351 2023-07-21 15:01:40.000000 nsj_rest_lib-1.6.1/src/nsj_rest_lib/controller/patch_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     3931 2023-07-21 15:01:40.000000 nsj_rest_lib-1.6.1/src/nsj_rest_lib/controller/post_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4341 2023-07-21 15:01:40.000000 nsj_rest_lib-1.6.1/src/nsj_rest_lib/controller/put_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4664 2023-07-21 15:01:40.000000 nsj_rest_lib-1.6.1/src/nsj_rest_lib/controller/route_base.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-08-06 01:08:01.915211 nsj_rest_lib-1.6.1/src/nsj_rest_lib/dao/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-1.6.1/src/nsj_rest_lib/dao/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)    23343 2023-08-06 00:46:06.000000 nsj_rest_lib-1.6.1/src/nsj_rest_lib/dao/dao_base.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     1235 2023-08-02 23:56:53.000000 nsj_rest_lib-1.6.1/src/nsj_rest_lib/db_pool_config.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-08-06 01:08:01.915211 nsj_rest_lib-1.6.1/src/nsj_rest_lib/decorator/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-1.6.1/src/nsj_rest_lib/decorator/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4737 2023-07-21 15:01:40.000000 nsj_rest_lib-1.6.1/src/nsj_rest_lib/decorator/dto.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-08-06 01:08:01.915211 nsj_rest_lib-1.6.1/src/nsj_rest_lib/descriptor/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-1.6.1/src/nsj_rest_lib/descriptor/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      418 2023-07-21 15:01:40.000000 nsj_rest_lib-1.6.1/src/nsj_rest_lib/descriptor/conjunto_type.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)    13263 2023-08-05 23:30:05.000000 nsj_rest_lib-1.6.1/src/nsj_rest_lib/descriptor/dto_field.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     7563 2023-07-21 15:01:40.000000 nsj_rest_lib-1.6.1/src/nsj_rest_lib/descriptor/dto_field_validators.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     5408 2023-07-21 15:01:40.000000 nsj_rest_lib-1.6.1/src/nsj_rest_lib/descriptor/dto_list_field.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      320 2023-07-21 15:01:40.000000 nsj_rest_lib-1.6.1/src/nsj_rest_lib/descriptor/filter_operator.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     2295 2023-07-21 15:01:40.000000 nsj_rest_lib-1.6.1/src/nsj_rest_lib/doc_route_generator.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-08-06 01:08:01.915211 nsj_rest_lib-1.6.1/src/nsj_rest_lib/dto/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-1.6.1/src/nsj_rest_lib/dto/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     7760 2023-07-21 15:01:40.000000 nsj_rest_lib-1.6.1/src/nsj_rest_lib/dto/dto_base.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-08-06 01:08:01.919211 nsj_rest_lib-1.6.1/src/nsj_rest_lib/entity/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-1.6.1/src/nsj_rest_lib/entity/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      710 2023-07-21 15:01:40.000000 nsj_rest_lib-1.6.1/src/nsj_rest_lib/entity/entity_base.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      322 2023-07-21 15:01:40.000000 nsj_rest_lib-1.6.1/src/nsj_rest_lib/entity/filter.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      483 2023-07-21 15:01:40.000000 nsj_rest_lib-1.6.1/src/nsj_rest_lib/exception.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     2856 2023-07-21 15:01:40.000000 nsj_rest_lib-1.6.1/src/nsj_rest_lib/healthcheck_config.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      825 2023-07-21 15:01:40.000000 nsj_rest_lib-1.6.1/src/nsj_rest_lib/injector_factory_base.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-08-06 01:08:01.919211 nsj_rest_lib-1.6.1/src/nsj_rest_lib/service/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-1.6.1/src/nsj_rest_lib/service/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)    24839 2023-08-06 00:29:55.000000 nsj_rest_lib-1.6.1/src/nsj_rest_lib/service/service_base.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      707 2023-07-21 15:01:40.000000 nsj_rest_lib-1.6.1/src/nsj_rest_lib/settings.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-08-06 01:08:01.919211 nsj_rest_lib-1.6.1/src/nsj_rest_lib/validator/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-1.6.1/src/nsj_rest_lib/validator/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4196 2023-07-21 15:01:40.000000 nsj_rest_lib-1.6.1/src/nsj_rest_lib/validator/cpf_cnpj.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      527 2023-07-21 15:01:40.000000 nsj_rest_lib-1.6.1/src/nsj_rest_lib/validator/validate_data.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-08-06 01:08:01.915211 nsj_rest_lib-1.6.1/src/nsj_rest_lib.egg-info/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      743 2023-08-06 01:08:01.000000 nsj_rest_lib-1.6.1/src/nsj_rest_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     1738 2023-08-06 01:08:01.000000 nsj_rest_lib-1.6.1/src/nsj_rest_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        1 2023-08-06 01:08:01.000000 nsj_rest_lib-1.6.1/src/nsj_rest_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      113 2023-08-06 01:08:01.000000 nsj_rest_lib-1.6.1/src/nsj_rest_lib.egg-info/requires.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)       13 2023-08-06 01:08:01.000000 nsj_rest_lib-1.6.1/src/nsj_rest_lib.egg-info/top_level.txt
```

### Comparing `nsj_rest_lib-1.5.1/PKG-INFO` & `nsj_rest_lib-1.6.1/src/nsj_rest_lib.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: nsj_rest_lib
-Version: 1.5.1
+Name: nsj-rest-lib
+Version: 1.6.1
 Summary: Biblioteca para construção de APIs Rest Python, de acordo com o guidelines interno, e com paradigma declarativo.
 Home-page: https://github.com/Nasajon/nsj_rest_lib
 Author: Nasajon Sistemas
 Author-email: contact.dev@nasajon.com.br
 Project-URL: Source, https://github.com/Nasajon/nsj_rest_lib
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `nsj_rest_lib-1.5.1/setup.cfg` & `nsj_rest_lib-1.6.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nsj_rest_lib
-version = 1.5.1
+version = 1.6.1
 author = Nasajon Sistemas
 author_email = contact.dev@nasajon.com.br
 description = Biblioteca para construção de APIs Rest Python, de acordo com o guidelines interno, e com paradigma declarativo.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Nasajon/nsj_rest_lib
 project_urls =
```

### Comparing `nsj_rest_lib-1.5.1/src/nsj_rest_lib/controller/delete_route.py` & `nsj_rest_lib-1.6.1/src/nsj_rest_lib/controller/delete_route.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.5.1/src/nsj_rest_lib/controller/funtion_route_wrapper.py` & `nsj_rest_lib-1.6.1/src/nsj_rest_lib/controller/funtion_route_wrapper.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.5.1/src/nsj_rest_lib/controller/get_route.py` & `nsj_rest_lib-1.6.1/src/nsj_rest_lib/controller/get_route.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.5.1/src/nsj_rest_lib/controller/list_route.py` & `nsj_rest_lib-1.6.1/src/nsj_rest_lib/controller/list_route.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.5.1/src/nsj_rest_lib/controller/patch_route.py` & `nsj_rest_lib-1.6.1/src/nsj_rest_lib/controller/patch_route.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.5.1/src/nsj_rest_lib/controller/post_route.py` & `nsj_rest_lib-1.6.1/src/nsj_rest_lib/controller/post_route.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.5.1/src/nsj_rest_lib/controller/put_route.py` & `nsj_rest_lib-1.6.1/src/nsj_rest_lib/controller/put_route.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.5.1/src/nsj_rest_lib/controller/route_base.py` & `nsj_rest_lib-1.6.1/src/nsj_rest_lib/controller/route_base.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.5.1/src/nsj_rest_lib/dao/dao_base.py` & `nsj_rest_lib-1.6.1/src/nsj_rest_lib/dao/dao_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,20 +59,21 @@
 
         # Creating entity instance
         entity = self._entity_class()
 
         # Building SQL fields
         if fields is None:
             fields = [
-                f"t0.{k}"
+                f"k"
                 for k in entity.__dict__
                 if not callable(getattr(entity, k, None)) and not k.startswith("_")
             ]
 
-        return ", ".join(fields)
+        resp = ", t0.".join(fields)
+        return f"t0.{resp}"
 
     def get(self, id: uuid.UUID, fields: List[str] = None, filters=None) -> EntityBase:
         """
         Returns an entity instance by its ID.
         """
 
         # Creating a entity instance
@@ -385,14 +386,62 @@
             "grupo_empresarial_conjunto_codigo": tuple(valores_filtro),
         }
 
         del filters[conjunto_field]
 
         return join_conjuntos, with_conjunto, fields_conjunto, conjunto_map
 
+    def insert_relacionamento_conjunto(
+        self,
+        id: str,
+        conjunto_field_value: str,
+        conjunto_type: ConjuntoType = None,
+    ):
+        # Recuperando o conjunto correspondente ao grupo_empresarial
+        tabela_conjunto = f"ns.conjuntos{conjunto_type.name.lower()}"
+        cadastro = conjunto_type.value
+
+        sql = f"""
+        select
+            gemp0.grupoempresarial as grupo_empresarial_pk,
+            est_c0.conjunto
+        from ns.gruposempresariais gemp0
+        join ns.empresas emp0 on (emp0.grupoempresarial = gemp0.grupoempresarial and gemp0.codigo = :grupo_empresarial_conjunto_codigo)
+        join ns.estabelecimentos est0 on (est0.empresa = emp0.empresa)
+        join ns.estabelecimentosconjuntos est_c0 on (
+            est_c0.estabelecimento = est0.estabelecimento
+            and est_c0.cadastro = :conjunto_cadastro
+        )
+        group by gemp0.grupoempresarial, est_c0.conjunto
+        """
+
+        data = {
+            "conjunto_cadastro": cadastro,
+            "grupo_empresarial_conjunto_codigo": conjunto_field_value,
+        }
+        resp = self._db.execute_query(sql, **data)
+
+        if len(resp) > 1:
+            raise Exception(
+                f"A biblioteca nsj_rest_lib ainda não suporta inserção de registros onde há mais de um conjunto, de um mesmo tipo ({cadastro}), num mesmo grupo_empresarial ({conjunto_field_value})."
+            )
+
+        if len(resp) < 1:
+            raise Exception(
+                f"Não foi encontrado um conjunto correspondente ao grupo empresarial {conjunto_field_value}, para um tipo de cadastro {cadastro}."
+            )
+
+        # Inserindo o relacionamento com o conjunto
+        sql = f"""
+        insert into {tabela_conjunto} (conjunto, registro) values (:conjunto, :registro)
+        """
+
+        data = {"conjunto": resp[0]["conjunto"], "registro": id}
+        self._db.execute(sql, **data)
+
     def _sql_insert_fields(self) -> str:
         """
         Retorna uma tupla com duas partes: (sql_fields, sql_ref_values), onde:
         - sql_fields: Lista de campos a inserir no insert
         - sql_ref_values: Lista das referências aos campos, a inserir no insert (parte values)
         """
 
@@ -432,16 +481,21 @@
             {sql_ref_values}
 
         )
         """
 
         # Montando as cláusulas returning
         returning_fields = entity.get_insert_returning_fields()
+        if returning_fields is None:
+            returning_fields = []
+
+        if entity.get_pk_field() not in returning_fields:
+            returning_fields.append(entity.get_pk_field())
 
-        if returning_fields is not None and USE_SQL_RETURNING_CLAUSE:
+        if USE_SQL_RETURNING_CLAUSE:
             sql_returning = ", ".join(returning_fields)
 
             sql += "\n"
             sql += f"returning {sql_returning}"
 
         # Montando um dicionário com valores das propriedades
         values_map = convert_to_dumps(entity)
```

### Comparing `nsj_rest_lib-1.5.1/src/nsj_rest_lib/db_pool_config.py` & `nsj_rest_lib-1.6.1/src/nsj_rest_lib/db_pool_config.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.5.1/src/nsj_rest_lib/decorator/dto.py` & `nsj_rest_lib-1.6.1/src/nsj_rest_lib/decorator/dto.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.5.1/src/nsj_rest_lib/descriptor/dto_field.py` & `nsj_rest_lib-1.6.1/src/nsj_rest_lib/descriptor/dto_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,22 +89,28 @@
     def __get__(self, instance, owner):
         if instance is None:
             return self
         else:
             return instance.__dict__[self.storage_name]
 
     def __set__(self, instance, value):
-        if not ("escape_validator" in instance.__dict__ and instance.__dict__["escape_validator"] == True):
+        try:
             if self.validator is None:
                 if self.use_default_validator:
                     value = self.validate(self, value)
             else:
                 if self.use_default_validator:
                     value = self.validate(self, value)
                 value = self.validator(self, value)
+        except ValueError as e:
+            if not (
+                "escape_validator" in instance.__dict__
+                and instance.__dict__["escape_validator"] == True
+            ):
+                raise
 
         instance.__dict__[self.storage_name] = value
 
     def validate(self, dto_field: "DTOField", value):
         """
         Default validator (ckecking default constraints: not null, type, min, max and enum types).
         """
```

### Comparing `nsj_rest_lib-1.5.1/src/nsj_rest_lib/descriptor/dto_field_validators.py` & `nsj_rest_lib-1.6.1/src/nsj_rest_lib/descriptor/dto_field_validators.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.5.1/src/nsj_rest_lib/descriptor/dto_list_field.py` & `nsj_rest_lib-1.6.1/src/nsj_rest_lib/descriptor/dto_list_field.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.5.1/src/nsj_rest_lib/doc_route_generator.py` & `nsj_rest_lib-1.6.1/src/nsj_rest_lib/doc_route_generator.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.5.1/src/nsj_rest_lib/dto/dto_base.py` & `nsj_rest_lib-1.6.1/src/nsj_rest_lib/dto/dto_base.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.5.1/src/nsj_rest_lib/entity/entity_base.py` & `nsj_rest_lib-1.6.1/src/nsj_rest_lib/entity/entity_base.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.5.1/src/nsj_rest_lib/healthcheck_config.py` & `nsj_rest_lib-1.6.1/src/nsj_rest_lib/healthcheck_config.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.5.1/src/nsj_rest_lib/injector_factory_base.py` & `nsj_rest_lib-1.6.1/src/nsj_rest_lib/injector_factory_base.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.5.1/src/nsj_rest_lib/service/service_base.py` & `nsj_rest_lib-1.6.1/src/nsj_rest_lib/service/service_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -212,15 +212,17 @@
             order_fields,
             entity_filters,
             conjunto_type=self._dto_class.conjunto_type,
             conjunto_field=self._dto_class.conjunto_field,
         )
 
         # Convertendo para uma lista de DTOs
-        dto_list = [self._dto_class(entity, escape_validator=True) for entity in entity_list]
+        dto_list = [
+            self._dto_class(entity, escape_validator=True) for entity in entity_list
+        ]
 
         # Retrieving related lists
         if len(self._dto_class.list_fields_map) > 0:
             self._retrieve_related_lists(dto_list, fields)
 
         # Returning
         return dto_list
@@ -365,19 +367,32 @@
                         if value is None or value == "":
                             raise ValueError(
                                 f"É necessário preencher o campo '{self._updated_by_property}'"
                             )
 
             # Invocando o DAO
             if insert:
+                # Verificando se há outro registro com mesma PK
+                # TODO Verificar a existência considerando os conjuntos
                 if self.entity_exists(entity, aditional_filters):
                     raise ConflictException(
                         f"Já existe um registro no banco com o identificador '{getattr(entity, entity_pk_field)}'"
                     )
+
+                # Inserindo o registro no banco
                 entity = self._dao.insert(entity)
+
+                # Inserindo os conjuntos (se necessário)
+                if self._dto_class.conjunto_type is not None:
+                    pk_value = getattr(entity, entity.get_pk_field())
+                    conjunto_field_value = getattr(dto, self._dto_class.conjunto_field)
+
+                    self._dao.insert_relacionamento_conjunto(
+                        pk_value, conjunto_field_value, self._dto_class.conjunto_type
+                    )
             else:
                 # Montando os filtros
                 id_condiction = Filter(FilterOperator.EQUALS, id)
                 id_filters = {entity_pk_field: [id_condiction]}
 
                 if aditional_filters is not None:
                     aditional_entity_filters = self._create_entity_filters(
@@ -389,15 +404,17 @@
                 entity_filters = {**id_filters, **aditional_entity_filters}
 
                 # Executando o update pelo DAO
                 entity = self._dao.update(entity, entity_filters, partial_update)
 
             # Convertendo a entity para o DTO de resposta (se houver um)
             if self._dto_post_response_class is not None:
-                response_dto = self._dto_post_response_class(entity, escape_validator=True)
+                response_dto = self._dto_post_response_class(
+                    entity, escape_validator=True
+                )
             else:
                 # Retorna None, se não se espera um DTO de resposta
                 response_dto = None
 
             # Salvando as lista de DTO detalhe
             if len(self._dto_class.list_fields_map) > 0:
                 self._save_related_lists(
```

### Comparing `nsj_rest_lib-1.5.1/src/nsj_rest_lib/settings.py` & `nsj_rest_lib-1.6.1/src/nsj_rest_lib/settings.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.5.1/src/nsj_rest_lib/validator/cpf_cnpj.py` & `nsj_rest_lib-1.6.1/src/nsj_rest_lib/validator/cpf_cnpj.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.5.1/src/nsj_rest_lib/validator/validate_data.py` & `nsj_rest_lib-1.6.1/src/nsj_rest_lib/validator/validate_data.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.5.1/src/nsj_rest_lib.egg-info/PKG-INFO` & `nsj_rest_lib-1.6.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: nsj-rest-lib
-Version: 1.5.1
+Name: nsj_rest_lib
+Version: 1.6.1
 Summary: Biblioteca para construção de APIs Rest Python, de acordo com o guidelines interno, e com paradigma declarativo.
 Home-page: https://github.com/Nasajon/nsj_rest_lib
 Author: Nasajon Sistemas
 Author-email: contact.dev@nasajon.com.br
 Project-URL: Source, https://github.com/Nasajon/nsj_rest_lib
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `nsj_rest_lib-1.5.1/src/nsj_rest_lib.egg-info/SOURCES.txt` & `nsj_rest_lib-1.6.1/src/nsj_rest_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

