# Comparing `tmp/eolymp-0.8.1.tar.gz` & `tmp/eolymp-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eolymp-0.8.1.tar", last modified: Sat Aug  5 15:23:54 2023, max compression
+gzip compressed data, was "eolymp-0.8.2.tar", last modified: Sun Aug  6 19:36:16 2023, max compression
```

## Comparing `eolymp-0.8.1.tar` & `eolymp-0.8.2.tar`

### file list

```diff
@@ -1,396 +1,396 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 15:23:54.603536 eolymp-0.8.1/
--rw-r--r--   0 root         (0) root         (0)      911 2023-08-05 15:23:54.603536 eolymp-0.8.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      512 2023-08-05 15:23:53.000000 eolymp-0.8.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 15:23:54.531530 eolymp-0.8.1/eolymp/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 15:23:54.535531 eolymp-0.8.1/eolymp/acl/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/acl/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2478 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/acl/acl_service_http.py
--rw-r--r--   0 root         (0) root         (0)     6121 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/acl/acl_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4305 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/acl/acl_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)      842 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/acl/entitlement_service_http.py
--rw-r--r--   0 root         (0) root         (0)     2215 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/acl/entitlement_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)      798 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/acl/entitlement_service_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 15:23:54.535531 eolymp-0.8.1/eolymp/annotations/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/annotations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1690 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/annotations/endpoint_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1042 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/annotations/endpoint_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2308 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/annotations/http_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2402 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/annotations/http_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1536 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/annotations/ratelimit_pb2.py
--rw-r--r--   0 root         (0) root         (0)      623 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/annotations/ratelimit_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1462 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/annotations/scope_pb2.py
--rw-r--r--   0 root         (0) root         (0)      654 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/annotations/scope_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 15:23:54.535531 eolymp-0.8.1/eolymp/apollo/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/apollo/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1364 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/apollo/events_pb2.py
--rw-r--r--   0 root         (0) root         (0)      820 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/apollo/events_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 15:23:54.539531 eolymp-0.8.1/eolymp/asset/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/asset/__init__.py
--rw-r--r--   0 root         (0) root         (0)      809 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/asset/asset_http.py
--rw-r--r--   0 root         (0) root         (0)     2995 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/asset/asset_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2354 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/asset/asset_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)      816 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/asset/asset_service_http.py
--rw-r--r--   0 root         (0) root         (0)     2124 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/asset/asset_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)      355 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/asset/asset_service_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 15:23:54.551532 eolymp-0.8.1/eolymp/atlas/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/atlas/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2072 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/asset_service_http.py
--rw-r--r--   0 root         (0) root         (0)     5722 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/asset_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3872 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/asset_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)    25164 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/atlas_http.py
--rw-r--r--   0 root         (0) root         (0)    30169 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/atlas_pb2.py
--rw-r--r--   0 root         (0) root         (0)      957 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/atlas_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1239 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/attachment_pb2.py
--rw-r--r--   0 root         (0) root         (0)      664 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/attachment_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2564 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/attachment_service_http.py
--rw-r--r--   0 root         (0) root         (0)     7093 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/attachment_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4619 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/attachment_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1132 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/bookmark_service_http.py
--rw-r--r--   0 root         (0) root         (0)     2831 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/bookmark_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1124 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/bookmark_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1218 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/code_template_file_pb2.py
--rw-r--r--   0 root         (0) root         (0)      602 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/code_template_file_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1640 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/code_template_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1625 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/code_template_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2896 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/code_template_service_http.py
--rw-r--r--   0 root         (0) root         (0)     7639 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/code_template_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4356 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/code_template_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1413 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/editorial_pb2.py
--rw-r--r--   0 root         (0) root         (0)      948 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/editorial_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     3205 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/editorial_service_http.py
--rw-r--r--   0 root         (0) root         (0)     8288 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/editorial_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4418 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/editorial_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1859 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/events_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1298 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/events_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2046 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/library_service_http.py
--rw-r--r--   0 root         (0) root         (0)     8197 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/library_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     7646 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/library_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2772 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/problem_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1592 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/problem_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2416 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/problem_service_http.py
--rw-r--r--   0 root         (0) root         (0)     5937 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/problem_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2958 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/problem_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1445 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/scoring_score_pb2.py
--rw-r--r--   0 root         (0) root         (0)      953 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/scoring_score_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1595 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/scoring_service_http.py
--rw-r--r--   0 root         (0) root         (0)     4331 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/scoring_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2529 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/scoring_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1955 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/solution_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1871 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/solution_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1764 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/statement_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1539 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/statement_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     3195 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/statement_service_http.py
--rw-r--r--   0 root         (0) root         (0)     8504 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/statement_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     5202 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/statement_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     4906 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/submission_pb2.py
--rw-r--r--   0 root         (0) root         (0)     7543 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/submission_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2105 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/submission_service_http.py
--rw-r--r--   0 root         (0) root         (0)     6050 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/submission_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     5292 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/submission_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1155 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/testing_config_pb2.py
--rw-r--r--   0 root         (0) root         (0)      407 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/testing_config_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1244 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/testing_feedback_pb2.py
--rw-r--r--   0 root         (0) root         (0)      381 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/testing_feedback_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1270 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/testing_scoring_pb2.py
--rw-r--r--   0 root         (0) root         (0)      396 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/testing_scoring_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     7275 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/testing_service_http.py
--rw-r--r--   0 root         (0) root         (0)    18070 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/testing_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    11063 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/testing_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1372 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/testing_test_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1029 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/testing_test_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1867 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/testing_testset_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1867 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/testing_testset_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1443 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/version_pb2.py
--rw-r--r--   0 root         (0) root         (0)      995 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/version_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 15:23:54.551532 eolymp-0.8.1/eolymp/auth/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1650 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/auth/claims_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1830 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/auth/claims_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)      493 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/auth/oauth2_service_http.py
--rw-r--r--   0 root         (0) root         (0)     6035 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/auth/oauth2_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     5486 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/auth/oauth2_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)      490 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/auth/sso_service_http.py
--rw-r--r--   0 root         (0) root         (0)     2894 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/auth/sso_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1917 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/auth/sso_service_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 15:23:54.555532 eolymp-0.8.1/eolymp/cognito/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/cognito/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1483 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/cognito/access_key_pb2.py
--rw-r--r--   0 root         (0) root         (0)      997 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/cognito/access_key_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     8102 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/cognito/cognito_http.py
--rw-r--r--   0 root         (0) root         (0)    25518 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/cognito/cognito_pb2.py
--rw-r--r--   0 root         (0) root         (0)    21124 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/cognito/cognito_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1170 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/cognito/quota_pb2.py
--rw-r--r--   0 root         (0) root         (0)      482 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/cognito/quota_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2297 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/cognito/user_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2923 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/cognito/user_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 15:23:54.559533 eolymp-0.8.1/eolymp/community/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/community/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3544 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/community/account_service_http.py
--rw-r--r--   0 root         (0) root         (0)     9900 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/community/account_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     6329 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/community/account_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2632 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/community/attribute_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3348 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/community/attribute_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2568 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/community/attribute_service_http.py
--rw-r--r--   0 root         (0) root         (0)     7127 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/community/attribute_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4511 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/community/attribute_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1627 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/community/configuration_idp_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1447 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/community/configuration_idp_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1188 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/community/configuration_service_http.py
--rw-r--r--   0 root         (0) root         (0)     3759 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/community/configuration_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1478 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/community/configuration_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1696 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/community/events_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1025 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/community/events_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1158 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/community/member_ghost_pb2.py
--rw-r--r--   0 root         (0) root         (0)      379 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/community/member_ghost_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2173 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/community/member_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1896 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/community/member_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     4017 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/community/member_service_http.py
--rw-r--r--   0 root         (0) root         (0)    11354 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/community/member_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     8833 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/community/member_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1195 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/community/member_team_pb2.py
--rw-r--r--   0 root         (0) root         (0)      469 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/community/member_team_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2124 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/community/member_user_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2513 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/community/member_user_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1187 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/community/membership_service_http.py
--rw-r--r--   0 root         (0) root         (0)     3546 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/community/membership_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1415 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/community/membership_service_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 15:23:54.563533 eolymp-0.8.1/eolymp/content/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/content/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3542 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/content/content_service_http.py
--rw-r--r--   0 root         (0) root         (0)    10435 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/content/content_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     7524 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/content/content_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1450 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/content/fragment_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1126 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/content/fragment_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 15:23:54.563533 eolymp-0.8.1/eolymp/core/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1489 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/core/http_client.py
--rw-r--r--   0 root         (0) root         (0)     2288 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/core/oauth_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 15:23:54.567533 eolymp-0.8.1/eolymp/discussion/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/discussion/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2180 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/discussion/discussion_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2032 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/discussion/discussion_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     3064 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/discussion/discussion_service_http.py
--rw-r--r--   0 root         (0) root         (0)     8074 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/discussion/discussion_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4433 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/discussion/discussion_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1438 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/discussion/events_pb2.py
--rw-r--r--   0 root         (0) root         (0)      693 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/discussion/events_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1784 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/discussion/forum_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1387 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/discussion/forum_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2478 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/discussion/forum_service_http.py
--rw-r--r--   0 root         (0) root         (0)     6622 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/discussion/forum_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3860 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/discussion/forum_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1825 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/discussion/message_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1646 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/discussion/message_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2979 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/discussion/message_service_http.py
--rw-r--r--   0 root         (0) root         (0)     8680 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/discussion/message_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     6502 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/discussion/message_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1442 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/discussion/subscription_pb2.py
--rw-r--r--   0 root         (0) root         (0)      734 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/discussion/subscription_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1185 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/discussion/subscription_service_http.py
--rw-r--r--   0 root         (0) root         (0)     3644 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/discussion/subscription_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1289 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/discussion/subscription_service_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 15:23:54.567533 eolymp-0.8.1/eolymp/ecm/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/ecm/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1378 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/ecm/content_pb2.py
--rw-r--r--   0 root         (0) root         (0)      784 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/ecm/content_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1487 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/ecm/node_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1105 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/ecm/node_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 15:23:54.571534 eolymp-0.8.1/eolymp/executor/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/executor/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1617 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/executor/events_pb2.py
--rw-r--r--   0 root         (0) root         (0)      834 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/executor/events_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2558 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/executor/executor_http.py
--rw-r--r--   0 root         (0) root         (0)     8384 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/executor/executor_pb2.py
--rw-r--r--   0 root         (0) root         (0)     5724 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/executor/executor_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1705 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/executor/interactor_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1572 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/executor/interactor_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     6109 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/executor/job_pb2.py
--rw-r--r--   0 root         (0) root         (0)    11298 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/executor/job_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1225 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/executor/language_pb2.py
--rw-r--r--   0 root         (0) root         (0)      565 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/executor/language_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     5233 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/executor/report_pb2.py
--rw-r--r--   0 root         (0) root         (0)     7802 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/executor/report_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1290 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/executor/runtime_pb2.py
--rw-r--r--   0 root         (0) root         (0)      752 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/executor/runtime_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2965 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/executor/status_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4284 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/executor/status_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     3640 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/executor/task_pb2.py
--rw-r--r--   0 root         (0) root         (0)     6288 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/executor/task_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1565 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/executor/usage_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1635 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/executor/usage_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1950 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/executor/verifier_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2026 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/executor/verifier_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 15:23:54.575534 eolymp-0.8.1/eolymp/geography/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/geography/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1223 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/geography/country_pb2.py
--rw-r--r--   0 root         (0) root         (0)      549 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/geography/country_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2233 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/geography/geography_http.py
--rw-r--r--   0 root         (0) root         (0)     4943 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/geography/geography_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2558 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/geography/geography_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1252 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/geography/region_pb2.py
--rw-r--r--   0 root         (0) root         (0)      660 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/geography/region_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 15:23:54.575534 eolymp-0.8.1/eolymp/harmony/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/harmony/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1265 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/harmony/agreement_pb2.py
--rw-r--r--   0 root         (0) root         (0)      686 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/harmony/agreement_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1727 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/harmony/consent_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1332 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/harmony/consent_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2234 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/harmony/harmony_http.py
--rw-r--r--   0 root         (0) root         (0)     4871 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/harmony/harmony_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2717 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/harmony/harmony_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 15:23:54.579534 eolymp-0.8.1/eolymp/helpdesk/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/helpdesk/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1422 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/helpdesk/auto_reply_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1035 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/helpdesk/auto_reply_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1458 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/helpdesk/document_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1126 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/helpdesk/document_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2439 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/helpdesk/events_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2041 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/helpdesk/events_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     3573 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/helpdesk/helpdesk_http.py
--rw-r--r--   0 root         (0) root         (0)    10284 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/helpdesk/helpdesk_pb2.py
--rw-r--r--   0 root         (0) root         (0)     7297 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/helpdesk/helpdesk_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     8600 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/helpdesk/support_http.py
--rw-r--r--   0 root         (0) root         (0)    19983 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/helpdesk/support_pb2.py
--rw-r--r--   0 root         (0) root         (0)    13222 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/helpdesk/support_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     3595 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/helpdesk/ticket_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4215 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/helpdesk/ticket_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 15:23:54.587535 eolymp-0.8.1/eolymp/judge/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/judge/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2179 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/judge/acl_http.py
--rw-r--r--   0 root         (0) root         (0)     5512 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/judge/acl_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3991 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/judge/acl_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2389 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/judge/activity_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2641 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/judge/activity_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1498 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/judge/announcement_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1044 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/judge/announcement_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     3524 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/judge/contest_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4623 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/judge/contest_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     3285 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/judge/events_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3207 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/judge/events_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)    37756 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/judge/judge_http.py
--rw-r--r--   0 root         (0) root         (0)    78184 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/judge/judge_pb2.py
--rw-r--r--   0 root         (0) root         (0)    54096 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/judge/judge_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2522 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/judge/participant_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3192 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/judge/participant_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     3088 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/judge/problem_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4266 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/judge/problem_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1519 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/judge/reply_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1141 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/judge/reply_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1491 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/judge/result_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1178 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/judge/result_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2586 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/judge/score_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3589 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/judge/score_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     4771 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/judge/submission_pb2.py
--rw-r--r--   0 root         (0) root         (0)     7066 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/judge/submission_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1557 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/judge/template_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1421 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/judge/template_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1768 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/judge/ticket_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1841 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/judge/ticket_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 15:23:54.587535 eolymp-0.8.1/eolymp/keeper/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/keeper/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1257 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/keeper/blob_pb2.py
--rw-r--r--   0 root         (0) root         (0)      726 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/keeper/blob_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2965 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/keeper/keeper_http.py
--rw-r--r--   0 root         (0) root         (0)     7328 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/keeper/keeper_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4406 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/keeper/keeper_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 15:23:54.587535 eolymp-0.8.1/eolymp/l10n/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/l10n/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9434 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/l10n/localization_service_http.py
--rw-r--r--   0 root         (0) root         (0)    23464 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/l10n/localization_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    15558 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/l10n/localization_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1252 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/l10n/project_pb2.py
--rw-r--r--   0 root         (0) root         (0)      753 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/l10n/project_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1267 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/l10n/project_service_http.py
--rw-r--r--   0 root         (0) root         (0)     3835 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/l10n/project_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2221 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/l10n/project_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1460 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/l10n/term_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1055 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/l10n/term_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1851 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/l10n/translation_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1657 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/l10n/translation_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 15:23:54.591535 eolymp-0.8.1/eolymp/oauth2/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/oauth2/__init__.py
--rw-r--r--   0 root         (0) root         (0)      486 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/oauth2/oauth2_http.py
--rw-r--r--   0 root         (0) root         (0)     8147 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/oauth2/oauth2_pb2.py
--rw-r--r--   0 root         (0) root         (0)     9528 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/oauth2/oauth2_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 15:23:54.591535 eolymp-0.8.1/eolymp/playground/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/playground/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1689 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/playground/playground_http.py
--rw-r--r--   0 root         (0) root         (0)     4248 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/playground/playground_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1982 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/playground/playground_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2162 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/playground/run_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2275 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/playground/run_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 15:23:54.591535 eolymp-0.8.1/eolymp/ranker/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/ranker/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2245 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/ranker/activity_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2299 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/ranker/activity_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1258 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/ranker/events_pb2.py
--rw-r--r--   0 root         (0) root         (0)      652 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/ranker/events_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1165 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/ranker/format_pb2.py
--rw-r--r--   0 root         (0) root         (0)      335 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/ranker/format_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     8724 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/ranker/ranker_http.py
--rw-r--r--   0 root         (0) root         (0)    21385 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/ranker/ranker_pb2.py
--rw-r--r--   0 root         (0) root         (0)    15143 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/ranker/ranker_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     4876 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/ranker/scoreboard_pb2.py
--rw-r--r--   0 root         (0) root         (0)     8126 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/ranker/scoreboard_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 15:23:54.595536 eolymp-0.8.1/eolymp/resolver/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/resolver/__init__.py
--rw-r--r--   0 root         (0) root         (0)      923 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/resolver/resolver_http.py
--rw-r--r--   0 root         (0) root         (0)     3800 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/resolver/resolver_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3246 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/resolver/resolver_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 15:23:54.595536 eolymp-0.8.1/eolymp/taxonomy/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/taxonomy/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1145 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/taxonomy/link_service_http.py
--rw-r--r--   0 root         (0) root         (0)     3120 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/taxonomy/link_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1167 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/taxonomy/link_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1496 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/taxonomy/topic_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1377 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/taxonomy/topic_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     4010 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/taxonomy/topic_service_http.py
--rw-r--r--   0 root         (0) root         (0)    10053 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/taxonomy/topic_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     6654 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/taxonomy/topic_service_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 15:23:54.599536 eolymp-0.8.1/eolymp/typewriter/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/typewriter/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7630 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/typewriter/block_pb2.py
--rw-r--r--   0 root         (0) root         (0)    11265 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/typewriter/block_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1443 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/typewriter/events_pb2.py
--rw-r--r--   0 root         (0) root         (0)      704 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/typewriter/events_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1456 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/typewriter/fragment_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1108 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/typewriter/fragment_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2640 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/typewriter/inline_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2997 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/typewriter/inline_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     3884 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/typewriter/typewriter_http.py
--rw-r--r--   0 root         (0) root         (0)    11054 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/typewriter/typewriter_pb2.py
--rw-r--r--   0 root         (0) root         (0)     7632 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/typewriter/typewriter_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 15:23:54.599536 eolymp-0.8.1/eolymp/universe/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/universe/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1501 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/universe/permission_pb2.py
--rw-r--r--   0 root         (0) root         (0)      921 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/universe/permission_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2830 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/universe/space_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3986 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/universe/space_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     6381 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/universe/universe_http.py
--rw-r--r--   0 root         (0) root         (0)    14148 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/universe/universe_pb2.py
--rw-r--r--   0 root         (0) root         (0)     9254 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/universe/universe_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 15:23:54.599536 eolymp-0.8.1/eolymp/wellknown/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/wellknown/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1190 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/wellknown/direction_pb2.py
--rw-r--r--   0 root         (0) root         (0)      331 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/wellknown/direction_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2426 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/wellknown/errors_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2458 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/wellknown/errors_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     4481 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/wellknown/expression_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3915 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/wellknown/expression_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 15:23:54.603536 eolymp-0.8.1/eolymp/worker/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/worker/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1274 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/worker/events_pb2.py
--rw-r--r--   0 root         (0) root         (0)      505 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/worker/events_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2649 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/worker/job_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2880 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/worker/job_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2751 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/worker/worker_service_http.py
--rw-r--r--   0 root         (0) root         (0)     6564 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/worker/worker_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3389 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/worker/worker_service_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 15:23:54.531530 eolymp-0.8.1/eolymp.egg-info/
--rw-r--r--   0 root         (0) root         (0)      911 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11858 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-05 15:23:54.603536 eolymp-0.8.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      974 2023-08-05 15:23:54.000000 eolymp-0.8.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 19:36:16.103243 eolymp-0.8.2/
+-rw-r--r--   0 root         (0) root         (0)      911 2023-08-06 19:36:16.103243 eolymp-0.8.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      512 2023-08-06 19:36:15.000000 eolymp-0.8.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 19:36:15.959242 eolymp-0.8.2/eolymp/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 19:36:15.967242 eolymp-0.8.2/eolymp/acl/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/acl/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2478 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/acl/acl_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     6121 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/acl/acl_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4305 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/acl/acl_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)      842 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/acl/entitlement_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     2215 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/acl/entitlement_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      798 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/acl/entitlement_service_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 19:36:15.971243 eolymp-0.8.2/eolymp/annotations/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/annotations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1690 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/annotations/endpoint_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1042 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/annotations/endpoint_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2308 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/annotations/http_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2402 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/annotations/http_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1536 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/annotations/ratelimit_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      623 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/annotations/ratelimit_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1462 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/annotations/scope_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      654 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/annotations/scope_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 19:36:15.971243 eolymp-0.8.2/eolymp/apollo/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/apollo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1364 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/apollo/events_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      820 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/apollo/events_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 19:36:15.975242 eolymp-0.8.2/eolymp/asset/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/asset/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      809 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/asset/asset_http.py
+-rw-r--r--   0 root         (0) root         (0)     2995 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/asset/asset_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2354 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/asset/asset_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)      816 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/asset/asset_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     2124 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/asset/asset_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      355 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/asset/asset_service_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 19:36:16.003243 eolymp-0.8.2/eolymp/atlas/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/atlas/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2072 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/atlas/asset_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     5722 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/atlas/asset_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3872 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/atlas/asset_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)    25620 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/atlas/atlas_http.py
+-rw-r--r--   0 root         (0) root         (0)    30703 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/atlas/atlas_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      957 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/atlas/atlas_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1239 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/atlas/attachment_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      664 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/atlas/attachment_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2564 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/atlas/attachment_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     7093 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/atlas/attachment_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4619 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/atlas/attachment_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1132 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/atlas/bookmark_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     2831 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/atlas/bookmark_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1124 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/atlas/bookmark_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1218 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/atlas/code_template_file_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      602 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/atlas/code_template_file_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1640 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/atlas/code_template_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1625 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/atlas/code_template_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2896 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/atlas/code_template_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     7639 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/atlas/code_template_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4356 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/atlas/code_template_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1413 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/atlas/editorial_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      948 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/atlas/editorial_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     3205 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/atlas/editorial_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     8288 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/atlas/editorial_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4418 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/atlas/editorial_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1859 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/atlas/events_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1298 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/atlas/events_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2046 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/atlas/library_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     8485 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/atlas/library_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     7990 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/atlas/library_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2806 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/atlas/problem_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1688 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/atlas/problem_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2731 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/atlas/problem_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     6445 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/atlas/problem_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2958 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/atlas/problem_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1445 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/atlas/scoring_score_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      953 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/atlas/scoring_score_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1595 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/atlas/scoring_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     4331 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/atlas/scoring_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2529 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/atlas/scoring_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1955 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/atlas/solution_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1871 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/atlas/solution_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1764 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/atlas/statement_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1539 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/atlas/statement_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     3195 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/atlas/statement_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     8504 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/atlas/statement_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     5202 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/atlas/statement_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     4906 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/atlas/submission_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     7543 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/atlas/submission_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2105 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/atlas/submission_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     6050 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/atlas/submission_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     5292 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/atlas/submission_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1155 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/atlas/testing_config_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      407 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/atlas/testing_config_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1244 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/atlas/testing_feedback_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      381 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/atlas/testing_feedback_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1270 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/atlas/testing_scoring_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      396 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/atlas/testing_scoring_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     7275 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/atlas/testing_service_http.py
+-rw-r--r--   0 root         (0) root         (0)    18070 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/atlas/testing_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    11063 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/atlas/testing_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1372 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/atlas/testing_test_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1029 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/atlas/testing_test_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1867 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/atlas/testing_testset_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1867 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/atlas/testing_testset_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1443 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/atlas/version_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      995 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/atlas/version_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 19:36:16.007243 eolymp-0.8.2/eolymp/auth/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1650 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/auth/claims_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1830 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/auth/claims_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)      493 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/auth/oauth2_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     6035 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/auth/oauth2_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     5486 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/auth/oauth2_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)      490 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/auth/sso_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     2894 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/auth/sso_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1917 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/auth/sso_service_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 19:36:16.011243 eolymp-0.8.2/eolymp/cognito/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/cognito/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1483 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/cognito/access_key_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      997 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/cognito/access_key_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     8102 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/cognito/cognito_http.py
+-rw-r--r--   0 root         (0) root         (0)    25518 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/cognito/cognito_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    21124 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/cognito/cognito_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1170 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/cognito/quota_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      482 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/cognito/quota_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2297 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/cognito/user_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2923 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/cognito/user_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 19:36:16.023243 eolymp-0.8.2/eolymp/community/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/community/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3544 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/community/account_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     9900 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/community/account_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     6329 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/community/account_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2632 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/community/attribute_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3348 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/community/attribute_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2568 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/community/attribute_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     7127 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/community/attribute_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4511 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/community/attribute_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1627 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/community/configuration_idp_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1447 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/community/configuration_idp_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1188 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/community/configuration_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     3759 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/community/configuration_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1478 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/community/configuration_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1696 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/community/events_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1025 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/community/events_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1158 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/community/member_ghost_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      379 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/community/member_ghost_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2173 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/community/member_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1896 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/community/member_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     4017 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/community/member_service_http.py
+-rw-r--r--   0 root         (0) root         (0)    11354 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/community/member_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     8833 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/community/member_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1195 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/community/member_team_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      469 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/community/member_team_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2124 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/community/member_user_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2513 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/community/member_user_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1187 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/community/membership_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     3546 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/community/membership_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1415 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/community/membership_service_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 19:36:16.027243 eolymp-0.8.2/eolymp/content/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/content/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3542 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/content/content_service_http.py
+-rw-r--r--   0 root         (0) root         (0)    10435 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/content/content_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     7524 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/content/content_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1450 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/content/fragment_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1126 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/content/fragment_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 19:36:16.027243 eolymp-0.8.2/eolymp/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1489 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/core/http_client.py
+-rw-r--r--   0 root         (0) root         (0)     2288 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/core/oauth_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 19:36:16.035243 eolymp-0.8.2/eolymp/discussion/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/discussion/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2180 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/discussion/discussion_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2032 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/discussion/discussion_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     3064 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/discussion/discussion_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     8074 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/discussion/discussion_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4433 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/discussion/discussion_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1438 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/discussion/events_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      693 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/discussion/events_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1784 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/discussion/forum_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1387 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/discussion/forum_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2478 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/discussion/forum_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     6622 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/discussion/forum_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3860 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/discussion/forum_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1825 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/discussion/message_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1646 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/discussion/message_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2979 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/discussion/message_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     8680 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/discussion/message_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     6502 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/discussion/message_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1442 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/discussion/subscription_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      734 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/discussion/subscription_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1185 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/discussion/subscription_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     3644 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/discussion/subscription_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1289 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/discussion/subscription_service_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 19:36:16.039243 eolymp-0.8.2/eolymp/ecm/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/ecm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1378 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/ecm/content_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      784 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/ecm/content_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1487 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/ecm/node_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1105 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/ecm/node_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 19:36:16.047243 eolymp-0.8.2/eolymp/executor/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/executor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1617 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/executor/events_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      834 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/executor/events_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2558 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/executor/executor_http.py
+-rw-r--r--   0 root         (0) root         (0)     8384 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/executor/executor_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     5724 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/executor/executor_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1705 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/executor/interactor_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1572 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/executor/interactor_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     6109 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/executor/job_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    11298 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/executor/job_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1225 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/executor/language_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      565 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/executor/language_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     5233 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/executor/report_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     7802 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/executor/report_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1290 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/executor/runtime_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      752 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/executor/runtime_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2965 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/executor/status_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4284 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/executor/status_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     3640 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/executor/task_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     6288 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/executor/task_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1565 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/executor/usage_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1635 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/executor/usage_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1950 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/executor/verifier_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2026 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/executor/verifier_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 19:36:16.051243 eolymp-0.8.2/eolymp/geography/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/geography/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1223 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/geography/country_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      549 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/geography/country_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2233 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/geography/geography_http.py
+-rw-r--r--   0 root         (0) root         (0)     4943 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/geography/geography_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2558 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/geography/geography_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1252 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/geography/region_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      660 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/geography/region_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 19:36:16.051243 eolymp-0.8.2/eolymp/harmony/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/harmony/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1265 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/harmony/agreement_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      686 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/harmony/agreement_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1727 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/harmony/consent_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1332 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/harmony/consent_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2234 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/harmony/harmony_http.py
+-rw-r--r--   0 root         (0) root         (0)     4871 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/harmony/harmony_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2717 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/harmony/harmony_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 19:36:16.059243 eolymp-0.8.2/eolymp/helpdesk/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/helpdesk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1422 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/helpdesk/auto_reply_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1035 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/helpdesk/auto_reply_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1458 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/helpdesk/document_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1126 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/helpdesk/document_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2439 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/helpdesk/events_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2041 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/helpdesk/events_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     3573 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/helpdesk/helpdesk_http.py
+-rw-r--r--   0 root         (0) root         (0)    10284 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/helpdesk/helpdesk_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     7297 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/helpdesk/helpdesk_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     8600 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/helpdesk/support_http.py
+-rw-r--r--   0 root         (0) root         (0)    19983 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/helpdesk/support_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    13222 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/helpdesk/support_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     3595 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/helpdesk/ticket_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4215 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/helpdesk/ticket_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 19:36:16.071243 eolymp-0.8.2/eolymp/judge/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/judge/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2179 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/judge/acl_http.py
+-rw-r--r--   0 root         (0) root         (0)     5512 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/judge/acl_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3991 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/judge/acl_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2389 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/judge/activity_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2641 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/judge/activity_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1498 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/judge/announcement_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1044 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/judge/announcement_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     3524 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/judge/contest_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4623 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/judge/contest_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     3285 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/judge/events_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3207 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/judge/events_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)    37756 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/judge/judge_http.py
+-rw-r--r--   0 root         (0) root         (0)    78184 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/judge/judge_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    54096 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/judge/judge_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2522 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/judge/participant_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3192 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/judge/participant_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     3088 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/judge/problem_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4266 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/judge/problem_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1519 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/judge/reply_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1141 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/judge/reply_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1491 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/judge/result_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1178 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/judge/result_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2586 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/judge/score_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3589 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/judge/score_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     4771 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/judge/submission_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     7066 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/judge/submission_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1557 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/judge/template_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1421 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/judge/template_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1768 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/judge/ticket_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1841 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/judge/ticket_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 19:36:16.071243 eolymp-0.8.2/eolymp/keeper/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/keeper/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1257 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/keeper/blob_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      726 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/keeper/blob_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2965 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/keeper/keeper_http.py
+-rw-r--r--   0 root         (0) root         (0)     7328 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/keeper/keeper_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4406 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/keeper/keeper_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 19:36:16.079243 eolymp-0.8.2/eolymp/l10n/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/l10n/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9434 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/l10n/localization_service_http.py
+-rw-r--r--   0 root         (0) root         (0)    23464 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/l10n/localization_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    15558 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/l10n/localization_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1252 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/l10n/project_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      753 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/l10n/project_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1267 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/l10n/project_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     3835 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/l10n/project_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2221 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/l10n/project_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1460 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/l10n/term_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1055 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/l10n/term_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1851 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/l10n/translation_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1657 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/l10n/translation_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 19:36:16.079243 eolymp-0.8.2/eolymp/oauth2/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/oauth2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      486 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/oauth2/oauth2_http.py
+-rw-r--r--   0 root         (0) root         (0)     8147 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/oauth2/oauth2_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9528 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/oauth2/oauth2_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 19:36:16.079243 eolymp-0.8.2/eolymp/playground/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/playground/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1689 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/playground/playground_http.py
+-rw-r--r--   0 root         (0) root         (0)     4248 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/playground/playground_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1982 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/playground/playground_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2162 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/playground/run_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2275 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/playground/run_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 19:36:16.087243 eolymp-0.8.2/eolymp/ranker/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/ranker/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2245 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/ranker/activity_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2299 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/ranker/activity_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1258 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/ranker/events_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      652 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/ranker/events_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1165 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/ranker/format_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      335 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/ranker/format_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     8724 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/ranker/ranker_http.py
+-rw-r--r--   0 root         (0) root         (0)    21385 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/ranker/ranker_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    15143 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/ranker/ranker_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     4876 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/ranker/scoreboard_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     8126 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/ranker/scoreboard_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 19:36:16.087243 eolymp-0.8.2/eolymp/resolver/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/resolver/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      923 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/resolver/resolver_http.py
+-rw-r--r--   0 root         (0) root         (0)     3800 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/resolver/resolver_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3246 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/resolver/resolver_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 19:36:16.091243 eolymp-0.8.2/eolymp/taxonomy/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/taxonomy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1145 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/taxonomy/link_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     3120 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/taxonomy/link_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1167 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/taxonomy/link_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1496 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/taxonomy/topic_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1377 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/taxonomy/topic_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     4010 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/taxonomy/topic_service_http.py
+-rw-r--r--   0 root         (0) root         (0)    10053 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/taxonomy/topic_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     6654 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/taxonomy/topic_service_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 19:36:16.095243 eolymp-0.8.2/eolymp/typewriter/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/typewriter/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7630 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/typewriter/block_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    11265 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/typewriter/block_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1443 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/typewriter/events_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      704 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/typewriter/events_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1456 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/typewriter/fragment_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1108 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/typewriter/fragment_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2640 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/typewriter/inline_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2997 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/typewriter/inline_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     3884 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/typewriter/typewriter_http.py
+-rw-r--r--   0 root         (0) root         (0)    11054 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/typewriter/typewriter_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     7632 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/typewriter/typewriter_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 19:36:16.095243 eolymp-0.8.2/eolymp/universe/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/universe/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1501 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/universe/permission_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      921 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/universe/permission_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2830 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/universe/space_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3986 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/universe/space_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     6381 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/universe/universe_http.py
+-rw-r--r--   0 root         (0) root         (0)    14148 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/universe/universe_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9254 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/universe/universe_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 19:36:16.099243 eolymp-0.8.2/eolymp/wellknown/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/wellknown/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1190 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/wellknown/direction_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      331 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/wellknown/direction_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2426 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/wellknown/errors_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2458 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/wellknown/errors_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     4481 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/wellknown/expression_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3915 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/wellknown/expression_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 19:36:16.103243 eolymp-0.8.2/eolymp/worker/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/worker/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1274 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/worker/events_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      505 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/worker/events_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2649 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/worker/job_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2880 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/worker/job_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2751 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/worker/worker_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     6564 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/worker/worker_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3389 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp/worker/worker_service_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 19:36:15.963242 eolymp-0.8.2/eolymp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      911 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11858 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-08-06 19:36:15.000000 eolymp-0.8.2/eolymp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-06 19:36:16.103243 eolymp-0.8.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      974 2023-08-06 19:36:15.000000 eolymp-0.8.2/setup.py
```

### Comparing `eolymp-0.8.1/PKG-INFO` & `eolymp-0.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eolymp
-Version: 0.8.1
+Version: 0.8.2
 Summary: Eolymp SDK for Python
 Home-page: https://github.com/eolymp/contracts
 Author: Sergey Kolodyazhnyy
 Author-email: sergey@eolymp.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `eolymp-0.8.1/README.md` & `eolymp-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/acl/acl_service_http.py` & `eolymp-0.8.2/eolymp/acl/acl_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/acl/acl_service_pb2.py` & `eolymp-0.8.2/eolymp/acl/acl_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/acl/acl_service_pb2.pyi` & `eolymp-0.8.2/eolymp/acl/acl_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/acl/entitlement_service_http.py` & `eolymp-0.8.2/eolymp/acl/entitlement_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/acl/entitlement_service_pb2.py` & `eolymp-0.8.2/eolymp/acl/entitlement_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/acl/entitlement_service_pb2.pyi` & `eolymp-0.8.2/eolymp/acl/entitlement_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/annotations/endpoint_pb2.py` & `eolymp-0.8.2/eolymp/annotations/endpoint_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/annotations/endpoint_pb2.pyi` & `eolymp-0.8.2/eolymp/annotations/endpoint_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/annotations/http_pb2.py` & `eolymp-0.8.2/eolymp/annotations/http_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/annotations/http_pb2.pyi` & `eolymp-0.8.2/eolymp/annotations/http_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/annotations/ratelimit_pb2.py` & `eolymp-0.8.2/eolymp/annotations/ratelimit_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/annotations/ratelimit_pb2.pyi` & `eolymp-0.8.2/eolymp/annotations/ratelimit_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/annotations/scope_pb2.py` & `eolymp-0.8.2/eolymp/annotations/scope_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/annotations/scope_pb2.pyi` & `eolymp-0.8.2/eolymp/annotations/scope_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/apollo/events_pb2.py` & `eolymp-0.8.2/eolymp/apollo/events_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/apollo/events_pb2.pyi` & `eolymp-0.8.2/eolymp/apollo/events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/asset/asset_http.py` & `eolymp-0.8.2/eolymp/asset/asset_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/asset/asset_pb2.py` & `eolymp-0.8.2/eolymp/asset/asset_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/asset/asset_pb2.pyi` & `eolymp-0.8.2/eolymp/asset/asset_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/asset/asset_service_http.py` & `eolymp-0.8.2/eolymp/asset/asset_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/asset/asset_service_pb2.py` & `eolymp-0.8.2/eolymp/asset/asset_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/atlas/asset_service_http.py` & `eolymp-0.8.2/eolymp/atlas/asset_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/atlas/asset_service_pb2.py` & `eolymp-0.8.2/eolymp/atlas/asset_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/atlas/asset_service_pb2.pyi` & `eolymp-0.8.2/eolymp/atlas/asset_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/atlas/atlas_http.py` & `eolymp-0.8.2/eolymp/atlas/atlas_http.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,14 +74,28 @@
             method="PUT",
             url=self.url+path,
             request_data=request,
             response_symbol=_sym_db.GetSymbol("eolymp.atlas.UpdateProblemOutput"),
             **kwargs,
         )
 
+    def SyncProblem(self, request, **kwargs):
+        path = "/problems/"+urllib.parse.quote(request.problem_id)+"/sync"
+
+        # Cleanup URL parameters to avoid any ambiguity
+        request.problem_id = ""
+
+        return self.transport.request(
+            method="POST",
+            url=self.url+path,
+            request_data=request,
+            response_symbol=_sym_db.GetSymbol("eolymp.atlas.SyncProblemOutput"),
+            **kwargs,
+        )
+
     def SetBookmark(self, request, **kwargs):
         path = "/problems/"+urllib.parse.quote(request.problem_id)+"/bookmark"
 
         # Cleanup URL parameters to avoid any ambiguity
         request.problem_id = ""
 
         return self.transport.request(
```

### Comparing `eolymp-0.8.1/eolymp/atlas/atlas_pb2.py` & `eolymp-0.8.2/eolymp/atlas/atlas_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from eolymp.atlas import problem_service_pb2 as eolymp_dot_atlas_dot_problem__service__pb2
 from eolymp.atlas import scoring_service_pb2 as eolymp_dot_atlas_dot_scoring__service__pb2
 from eolymp.atlas import statement_service_pb2 as eolymp_dot_atlas_dot_statement__service__pb2
 from eolymp.atlas import submission_service_pb2 as eolymp_dot_atlas_dot_submission__service__pb2
 from eolymp.atlas import testing_service_pb2 as eolymp_dot_atlas_dot_testing__service__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18\x65olymp/atlas/atlas.proto\x12\x0c\x65olymp.atlas\x1a\x1d\x65olymp/annotations/http.proto\x1a\"eolymp/annotations/ratelimit.proto\x1a\x1e\x65olymp/annotations/scope.proto\x1a%eolymp/atlas/attachment_service.proto\x1a#eolymp/atlas/bookmark_service.proto\x1a(eolymp/atlas/code_template_service.proto\x1a\"eolymp/atlas/library_service.proto\x1a\"eolymp/atlas/problem_service.proto\x1a\"eolymp/atlas/scoring_service.proto\x1a$eolymp/atlas/statement_service.proto\x1a%eolymp/atlas/submission_service.proto\x1a\"eolymp/atlas/testing_service.proto2\xcb\x45\n\x05\x41tlas\x12\x91\x01\n\rCreateProblem\x12 .eolymp.atlas.CreateProblemInput\x1a!.eolymp.atlas.CreateProblemOutput\";\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\n\xd7#>\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x0b\"\t/problems\x12\x9e\x01\n\rDeleteProblem\x12 .eolymp.atlas.DeleteProblemInput\x1a!.eolymp.atlas.DeleteProblemOutput\"H\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\n\xd7#>\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x18*\x16/problems/{problem_id}\x12\x8d\x01\n\x0cListProblems\x12\x1f.eolymp.atlas.ListProblemsInput\x1a .eolymp.atlas.ListProblemsOutput\":\x82\xe3\n\x16\x8a\xe3\n\x12\x61tlas:problem:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0\x41\xf8\xe2\nd\x82\xd3\xe4\x93\x02\x0b\x12\t/problems\x12\xa3\x01\n\x0f\x44\x65scribeProblem\x12\".eolymp.atlas.DescribeProblemInput\x1a#.eolymp.atlas.DescribeProblemOutput\"G\x82\xe3\n\x16\x8a\xe3\n\x12\x61tlas:problem:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0\x41\xf8\xe2\nd\x82\xd3\xe4\x93\x02\x18\x12\x16/problems/{problem_id}\x12\x9e\x01\n\rUpdateProblem\x12 .eolymp.atlas.UpdateProblemInput\x1a!.eolymp.atlas.UpdateProblemOutput\"H\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0\x41\xf8\xe2\nd\x82\xd3\xe4\x93\x02\x18\x1a\x16/problems/{problem_id}\x12\x86\x01\n\x0bSetBookmark\x12\x1e.eolymp.atlas.SetBookmarkInput\x1a\x1f.eolymp.atlas.SetBookmarkOutput\"6\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x00@\xf8\xe2\n\n\x82\xd3\xe4\x93\x02!\"\x1f/problems/{problem_id}/bookmark\x12\x86\x01\n\x0bGetBookmark\x12\x1e.eolymp.atlas.GetBookmarkInput\x1a\x1f.eolymp.atlas.GetBookmarkOutput\"6\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xc8\x41\xf8\xe2\nd\x82\xd3\xe4\x93\x02!\x12\x1f/problems/{problem_id}/bookmark\x12\xa3\x01\n\x0cListExamples\x12\x1f.eolymp.atlas.ListExamplesInput\x1a .eolymp.atlas.ListExamplesOutput\"P\x82\xe3\n\x16\x8a\xe3\n\x12\x61tlas:problem:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0\x41\xf8\xe2\nd\x82\xd3\xe4\x93\x02!\x12\x1f/problems/{problem_id}/examples\x12\xb8\x01\n\x13UpdateTestingConfig\x12&.eolymp.atlas.UpdateTestingConfigInput\x1a\'.eolymp.atlas.UpdateTestingConfigOutput\"P\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\n\xd7#>\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02 \x1a\x1e/problems/{problem_id}/testing\x12\xbe\x01\n\x15\x44\x65scribeTestingConfig\x12(.eolymp.atlas.DescribeTestingConfigInput\x1a).eolymp.atlas.DescribeTestingConfigOutput\"P\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x00@\xf8\xe2\n\n\x82\xd3\xe4\x93\x02 \x12\x1e/problems/{problem_id}/testing\x12\xaa\x01\n\x0eUpdateVerifier\x12!.eolymp.atlas.UpdateVerifierInput\x1a\".eolymp.atlas.UpdateVerifierOutput\"Q\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\n\xd7#>\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02!\x1a\x1f/problems/{problem_id}/verifier\x12\xb0\x01\n\x10\x44\x65scribeVerifier\x12#.eolymp.atlas.DescribeVerifierInput\x1a$.eolymp.atlas.DescribeVerifierOutput\"Q\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x00@\xf8\xe2\n\n\x82\xd3\xe4\x93\x02!\x12\x1f/problems/{problem_id}/verifier\x12\xb2\x01\n\x10UpdateInteractor\x12#.eolymp.atlas.UpdateInteractorInput\x1a$.eolymp.atlas.UpdateInteractorOutput\"S\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\n\xd7#>\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02#\x1a!/problems/{problem_id}/interactor\x12\xb8\x01\n\x12\x44\x65scribeInteractor\x12%.eolymp.atlas.DescribeInteractorInput\x1a&.eolymp.atlas.DescribeInteractorOutput\"S\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x00@\xf8\xe2\n\n\x82\xd3\xe4\x93\x02#\x12!/problems/{problem_id}/interactor\x12\xaf\x01\n\x0f\x43reateStatement\x12\".eolymp.atlas.CreateStatementInput\x1a#.eolymp.atlas.CreateStatementOutput\"S\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02#\x1a!/problems/{problem_id}/statements\x12\xbe\x01\n\x0fUpdateStatement\x12\".eolymp.atlas.UpdateStatementInput\x1a#.eolymp.atlas.UpdateStatementOutput\"b\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x32\x1a\x30/problems/{problem_id}/statements/{statement_id}\x12\xbe\x01\n\x0f\x44\x65leteStatement\x12\".eolymp.atlas.DeleteStatementInput\x1a#.eolymp.atlas.DeleteStatementOutput\"b\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x32*0/problems/{problem_id}/statements/{statement_id}\x12\xab\x01\n\x0eListStatements\x12!.eolymp.atlas.ListStatementsInput\x1a\".eolymp.atlas.ListStatementsOutput\"R\x82\xe3\n\x16\x8a\xe3\n\x12\x61tlas:problem:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0\x41\xf8\xe2\nd\x82\xd3\xe4\x93\x02#\x12!/problems/{problem_id}/statements\x12\xc3\x01\n\x11\x44\x65scribeStatement\x12$.eolymp.atlas.DescribeStatementInput\x1a%.eolymp.atlas.DescribeStatementOutput\"a\x82\xe3\n\x16\x8a\xe3\n\x12\x61tlas:problem:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0\x41\xf8\xe2\nd\x82\xd3\xe4\x93\x02\x32\x12\x30/problems/{problem_id}/statements/{statement_id}\x12\xad\x01\n\x0fLookupStatement\x12\".eolymp.atlas.LookupStatementInput\x1a#.eolymp.atlas.LookupStatementOutput\"Q\x82\xe3\n\x16\x8a\xe3\n\x12\x61tlas:problem:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0\x41\xf8\xe2\nd\x82\xd3\xe4\x93\x02\"\x12 /problems/{problem_id}/translate\x12\xae\x01\n\x10PreviewStatement\x12#.eolymp.atlas.PreviewStatementInput\x1a$.eolymp.atlas.PreviewStatementOutput\"O\x82\xe3\n\x16\x8a\xe3\n\x12\x61tlas:problem:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0\x41\xf8\xe2\nd\x82\xd3\xe4\x93\x02 \"\x1e/problems/{problem_id}/renders\x12\xa7\x01\n\rCreateTestset\x12 .eolymp.atlas.CreateTestsetInput\x1a!.eolymp.atlas.CreateTestsetOutput\"Q\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n2\x82\xd3\xe4\x93\x02!\"\x1f/problems/{problem_id}/testsets\x12\xb4\x01\n\rUpdateTestset\x12 .eolymp.atlas.UpdateTestsetInput\x1a!.eolymp.atlas.UpdateTestsetOutput\"^\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n2\x82\xd3\xe4\x93\x02.\x1a,/problems/{problem_id}/testsets/{testset_id}\x12\xb4\x01\n\rDeleteTestset\x12 .eolymp.atlas.DeleteTestsetInput\x1a!.eolymp.atlas.DeleteTestsetOutput\"^\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n2\x82\xd3\xe4\x93\x02.*,/problems/{problem_id}/testsets/{testset_id}\x12\xa4\x01\n\x0cListTestsets\x12\x1f.eolymp.atlas.ListTestsetsInput\x1a .eolymp.atlas.ListTestsetsOutput\"Q\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\n2\x82\xd3\xe4\x93\x02!\x12\x1f/problems/{problem_id}/testsets\x12\xba\x01\n\x0f\x44\x65scribeTestset\x12\".eolymp.atlas.DescribeTestsetInput\x1a#.eolymp.atlas.DescribeTestsetOutput\"^\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\n2\x82\xd3\xe4\x93\x02.\x12,/problems/{problem_id}/testsets/{testset_id}\x12\xb2\x01\n\nCreateTest\x12\x1d.eolymp.atlas.CreateTestInput\x1a\x1e.eolymp.atlas.CreateTestOutput\"e\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0c\xf5\xe2\n\x00\x00 A\xf8\xe2\n\xc8\x01\x82\xd3\xe4\x93\x02\x34\"2/problems/{problem_id}/testsets/{testset_id}/tests\x12\xbc\x01\n\nUpdateTest\x12\x1d.eolymp.atlas.UpdateTestInput\x1a\x1e.eolymp.atlas.UpdateTestOutput\"o\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0c\xf5\xe2\n\x00\x00 A\xf8\xe2\n\xc8\x01\x82\xd3\xe4\x93\x02>\x1a</problems/{problem_id}/testsets/{testset_id}/tests/{test_id}\x12\xbc\x01\n\nDeleteTest\x12\x1d.eolymp.atlas.DeleteTestInput\x1a\x1e.eolymp.atlas.DeleteTestOutput\"o\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0c\xf5\xe2\n\x00\x00 A\xf8\xe2\n\xc8\x01\x82\xd3\xe4\x93\x02>*</problems/{problem_id}/testsets/{testset_id}/tests/{test_id}\x12\xae\x01\n\tListTests\x12\x1c.eolymp.atlas.ListTestsInput\x1a\x1d.eolymp.atlas.ListTestsOutput\"d\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\n2\x82\xd3\xe4\x93\x02\x34\x12\x32/problems/{problem_id}/testsets/{testset_id}/tests\x12\xc1\x01\n\x0c\x44\x65scribeTest\x12\x1f.eolymp.atlas.DescribeTestInput\x1a .eolymp.atlas.DescribeTestOutput\"n\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\n2\x82\xd3\xe4\x93\x02>\x12</problems/{problem_id}/testsets/{testset_id}/tests/{test_id}\x12\xb7\x01\n\x12\x43reateCodeTemplate\x12%.eolymp.atlas.CreateCodeTemplateInput\x1a&.eolymp.atlas.CreateCodeTemplateOutput\"R\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\n\xd7#>\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\"\" /problems/{problem_id}/templates\x12\xc5\x01\n\x12UpdateCodeTemplate\x12%.eolymp.atlas.UpdateCodeTemplateInput\x1a&.eolymp.atlas.UpdateCodeTemplateOutput\"`\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\n\xd7#>\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x30\"./problems/{problem_id}/templates/{template_id}\x12\xc5\x01\n\x12\x44\x65leteCodeTemplate\x12%.eolymp.atlas.DeleteCodeTemplateInput\x1a&.eolymp.atlas.DeleteCodeTemplateOutput\"`\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\n\xd7#>\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x30*./problems/{problem_id}/templates/{template_id}\x12\xb3\x01\n\x11ListCodeTemplates\x12$.eolymp.atlas.ListCodeTemplatesInput\x1a%.eolymp.atlas.ListCodeTemplatesOutput\"Q\x82\xe3\n\x16\x8a\xe3\n\x12\x61tlas:problem:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0\x41\xf8\xe2\nd\x82\xd3\xe4\x93\x02\"\x12 /problems/{problem_id}/templates\x12\xca\x01\n\x14\x44\x65scribeCodeTemplate\x12\'.eolymp.atlas.DescribeCodeTemplateInput\x1a(.eolymp.atlas.DescribeCodeTemplateOutput\"_\x82\xe3\n\x16\x8a\xe3\n\x12\x61tlas:problem:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0\x41\xf8\xe2\nd\x82\xd3\xe4\x93\x02\x30\x12./problems/{problem_id}/templates/{template_id}\x12\xb5\x01\n\x12LookupCodeTemplate\x12%.eolymp.atlas.LookupCodeTemplateInput\x1a&.eolymp.atlas.LookupCodeTemplateOutput\"P\x82\xe3\n\x16\x8a\xe3\n\x12\x61tlas:problem:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02!\x12\x1f/problems/{problem_id}/template\x12\xb3\x01\n\x10\x43reateAttachment\x12#.eolymp.atlas.CreateAttachmentInput\x1a$.eolymp.atlas.CreateAttachmentOutput\"T\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\n\xd7#>\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02$\"\"/problems/{problem_id}/attachments\x12\xc3\x01\n\x10UpdateAttachment\x12#.eolymp.atlas.UpdateAttachmentInput\x1a$.eolymp.atlas.UpdateAttachmentOutput\"d\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\n\xd7#>\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x34\"2/problems/{problem_id}/attachments/{attachment_id}\x12\xc3\x01\n\x10\x44\x65leteAttachment\x12#.eolymp.atlas.DeleteAttachmentInput\x1a$.eolymp.atlas.DeleteAttachmentOutput\"d\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\n\xd7#>\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x34*2/problems/{problem_id}/attachments/{attachment_id}\x12\xaf\x01\n\x0fListAttachments\x12\".eolymp.atlas.ListAttachmentsInput\x1a#.eolymp.atlas.ListAttachmentsOutput\"S\x82\xe3\n\x16\x8a\xe3\n\x12\x61tlas:problem:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0\x41\xf8\xe2\nd\x82\xd3\xe4\x93\x02$\x12\"/problems/{problem_id}/attachments\x12\xc8\x01\n\x12\x44\x65scribeAttachment\x12%.eolymp.atlas.DescribeAttachmentInput\x1a&.eolymp.atlas.DescribeAttachmentOutput\"c\x82\xe3\n\x16\x8a\xe3\n\x12\x61tlas:problem:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0\x41\xf8\xe2\nd\x82\xd3\xe4\x93\x02\x34\x12\x32/problems/{problem_id}/attachments/{attachment_id}\x12\x95\x01\n\x0cListVersions\x12\x1f.eolymp.atlas.ListVersionsInput\x1a .eolymp.atlas.ListVersionsOutput\"B\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\x82\xd3\xe4\x93\x02!\x12\x1f/problems/{problem_id}/versions\x12\x95\x01\n\x0eListProblemTop\x12!.eolymp.atlas.ListProblemTopInput\x1a\".eolymp.atlas.ListProblemTopOutput\"<\x82\xe3\n\x16\x8a\xe3\n\x12\x61tlas:problem:read\x82\xd3\xe4\x93\x02\x1c\x12\x1a/problems/{problem_id}/top\x12\xb1\x01\n\x16\x44\x65scribeProblemGrading\x12).eolymp.atlas.DescribeProblemGradingInput\x1a*.eolymp.atlas.DescribeProblemGradingOutput\"@\x82\xe3\n\x16\x8a\xe3\n\x12\x61tlas:problem:read\x82\xd3\xe4\x93\x02 \x12\x1e/problems/{problem_id}/grading\x12\xa7\x01\n\x10\x43reateSubmission\x12#.eolymp.atlas.CreateSubmissionInput\x1a$.eolymp.atlas.CreateSubmissionOutput\"H\x82\xe3\n\x1a\x8a\xe3\n\x16\x61tlas:submission:write\x82\xd3\xe4\x93\x02$\"\"/problems/{problem_id}/submissions\x12\xbc\x01\n\x12\x44\x65scribeSubmission\x12%.eolymp.atlas.DescribeSubmissionInput\x1a&.eolymp.atlas.DescribeSubmissionOutput\"W\x82\xe3\n\x19\x8a\xe3\n\x15\x61tlas:submission:read\x82\xd3\xe4\x93\x02\x34\x12\x32/problems/{problem_id}/submissions/{submission_id}\x12\xbe\x01\n\x10RetestSubmission\x12#.eolymp.atlas.RetestSubmissionInput\x1a$.eolymp.atlas.RetestSubmissionOutput\"_\x82\xe3\n\x1a\x8a\xe3\n\x16\x61tlas:submission:write\x82\xd3\xe4\x93\x02;\"9/problems/{problem_id}/submissions/{submission_id}/retest\x12\x8d\x01\n\x0fListSubmissions\x12\".eolymp.atlas.ListSubmissionsInput\x1a#.eolymp.atlas.ListSubmissionsOutput\"1\x82\xe3\n\x19\x8a\xe3\n\x15\x61tlas:submission:read\x82\xd3\xe4\x93\x02\x0e\x12\x0c/submissions\x12\xa2\x01\n\rDescribeScore\x12 .eolymp.atlas.DescribeScoreInput\x1a!.eolymp.atlas.DescribeScoreOutput\"L\x82\xe3\n\x19\x8a\xe3\n\x15\x61tlas:submission:read\x82\xd3\xe4\x93\x02)\x12\'/problems/{problem_id}/scores/{user_id}B-Z+github.com/eolymp/go-sdk/eolymp/atlas;atlasb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18\x65olymp/atlas/atlas.proto\x12\x0c\x65olymp.atlas\x1a\x1d\x65olymp/annotations/http.proto\x1a\"eolymp/annotations/ratelimit.proto\x1a\x1e\x65olymp/annotations/scope.proto\x1a%eolymp/atlas/attachment_service.proto\x1a#eolymp/atlas/bookmark_service.proto\x1a(eolymp/atlas/code_template_service.proto\x1a\"eolymp/atlas/library_service.proto\x1a\"eolymp/atlas/problem_service.proto\x1a\"eolymp/atlas/scoring_service.proto\x1a$eolymp/atlas/statement_service.proto\x1a%eolymp/atlas/submission_service.proto\x1a\"eolymp/atlas/testing_service.proto2\xeb\x46\n\x05\x41tlas\x12\x91\x01\n\rCreateProblem\x12 .eolymp.atlas.CreateProblemInput\x1a!.eolymp.atlas.CreateProblemOutput\";\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\n\xd7#>\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x0b\"\t/problems\x12\x9e\x01\n\rDeleteProblem\x12 .eolymp.atlas.DeleteProblemInput\x1a!.eolymp.atlas.DeleteProblemOutput\"H\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\n\xd7#>\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x18*\x16/problems/{problem_id}\x12\x8d\x01\n\x0cListProblems\x12\x1f.eolymp.atlas.ListProblemsInput\x1a .eolymp.atlas.ListProblemsOutput\":\x82\xe3\n\x16\x8a\xe3\n\x12\x61tlas:problem:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0\x41\xf8\xe2\nd\x82\xd3\xe4\x93\x02\x0b\x12\t/problems\x12\xa3\x01\n\x0f\x44\x65scribeProblem\x12\".eolymp.atlas.DescribeProblemInput\x1a#.eolymp.atlas.DescribeProblemOutput\"G\x82\xe3\n\x16\x8a\xe3\n\x12\x61tlas:problem:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0\x41\xf8\xe2\nd\x82\xd3\xe4\x93\x02\x18\x12\x16/problems/{problem_id}\x12\x9e\x01\n\rUpdateProblem\x12 .eolymp.atlas.UpdateProblemInput\x1a!.eolymp.atlas.UpdateProblemOutput\"H\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0\x41\xf8\xe2\nd\x82\xd3\xe4\x93\x02\x18\x1a\x16/problems/{problem_id}\x12\x9d\x01\n\x0bSyncProblem\x12\x1e.eolymp.atlas.SyncProblemInput\x1a\x1f.eolymp.atlas.SyncProblemOutput\"M\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\n\xd7#>\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x1d\"\x1b/problems/{problem_id}/sync\x12\x86\x01\n\x0bSetBookmark\x12\x1e.eolymp.atlas.SetBookmarkInput\x1a\x1f.eolymp.atlas.SetBookmarkOutput\"6\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x00@\xf8\xe2\n\n\x82\xd3\xe4\x93\x02!\"\x1f/problems/{problem_id}/bookmark\x12\x86\x01\n\x0bGetBookmark\x12\x1e.eolymp.atlas.GetBookmarkInput\x1a\x1f.eolymp.atlas.GetBookmarkOutput\"6\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xc8\x41\xf8\xe2\nd\x82\xd3\xe4\x93\x02!\x12\x1f/problems/{problem_id}/bookmark\x12\xa3\x01\n\x0cListExamples\x12\x1f.eolymp.atlas.ListExamplesInput\x1a .eolymp.atlas.ListExamplesOutput\"P\x82\xe3\n\x16\x8a\xe3\n\x12\x61tlas:problem:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0\x41\xf8\xe2\nd\x82\xd3\xe4\x93\x02!\x12\x1f/problems/{problem_id}/examples\x12\xb8\x01\n\x13UpdateTestingConfig\x12&.eolymp.atlas.UpdateTestingConfigInput\x1a\'.eolymp.atlas.UpdateTestingConfigOutput\"P\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\n\xd7#>\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02 \x1a\x1e/problems/{problem_id}/testing\x12\xbe\x01\n\x15\x44\x65scribeTestingConfig\x12(.eolymp.atlas.DescribeTestingConfigInput\x1a).eolymp.atlas.DescribeTestingConfigOutput\"P\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x00@\xf8\xe2\n\n\x82\xd3\xe4\x93\x02 \x12\x1e/problems/{problem_id}/testing\x12\xaa\x01\n\x0eUpdateVerifier\x12!.eolymp.atlas.UpdateVerifierInput\x1a\".eolymp.atlas.UpdateVerifierOutput\"Q\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\n\xd7#>\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02!\x1a\x1f/problems/{problem_id}/verifier\x12\xb0\x01\n\x10\x44\x65scribeVerifier\x12#.eolymp.atlas.DescribeVerifierInput\x1a$.eolymp.atlas.DescribeVerifierOutput\"Q\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x00@\xf8\xe2\n\n\x82\xd3\xe4\x93\x02!\x12\x1f/problems/{problem_id}/verifier\x12\xb2\x01\n\x10UpdateInteractor\x12#.eolymp.atlas.UpdateInteractorInput\x1a$.eolymp.atlas.UpdateInteractorOutput\"S\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\n\xd7#>\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02#\x1a!/problems/{problem_id}/interactor\x12\xb8\x01\n\x12\x44\x65scribeInteractor\x12%.eolymp.atlas.DescribeInteractorInput\x1a&.eolymp.atlas.DescribeInteractorOutput\"S\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x00@\xf8\xe2\n\n\x82\xd3\xe4\x93\x02#\x12!/problems/{problem_id}/interactor\x12\xaf\x01\n\x0f\x43reateStatement\x12\".eolymp.atlas.CreateStatementInput\x1a#.eolymp.atlas.CreateStatementOutput\"S\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02#\x1a!/problems/{problem_id}/statements\x12\xbe\x01\n\x0fUpdateStatement\x12\".eolymp.atlas.UpdateStatementInput\x1a#.eolymp.atlas.UpdateStatementOutput\"b\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x32\x1a\x30/problems/{problem_id}/statements/{statement_id}\x12\xbe\x01\n\x0f\x44\x65leteStatement\x12\".eolymp.atlas.DeleteStatementInput\x1a#.eolymp.atlas.DeleteStatementOutput\"b\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x32*0/problems/{problem_id}/statements/{statement_id}\x12\xab\x01\n\x0eListStatements\x12!.eolymp.atlas.ListStatementsInput\x1a\".eolymp.atlas.ListStatementsOutput\"R\x82\xe3\n\x16\x8a\xe3\n\x12\x61tlas:problem:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0\x41\xf8\xe2\nd\x82\xd3\xe4\x93\x02#\x12!/problems/{problem_id}/statements\x12\xc3\x01\n\x11\x44\x65scribeStatement\x12$.eolymp.atlas.DescribeStatementInput\x1a%.eolymp.atlas.DescribeStatementOutput\"a\x82\xe3\n\x16\x8a\xe3\n\x12\x61tlas:problem:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0\x41\xf8\xe2\nd\x82\xd3\xe4\x93\x02\x32\x12\x30/problems/{problem_id}/statements/{statement_id}\x12\xad\x01\n\x0fLookupStatement\x12\".eolymp.atlas.LookupStatementInput\x1a#.eolymp.atlas.LookupStatementOutput\"Q\x82\xe3\n\x16\x8a\xe3\n\x12\x61tlas:problem:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0\x41\xf8\xe2\nd\x82\xd3\xe4\x93\x02\"\x12 /problems/{problem_id}/translate\x12\xae\x01\n\x10PreviewStatement\x12#.eolymp.atlas.PreviewStatementInput\x1a$.eolymp.atlas.PreviewStatementOutput\"O\x82\xe3\n\x16\x8a\xe3\n\x12\x61tlas:problem:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0\x41\xf8\xe2\nd\x82\xd3\xe4\x93\x02 \"\x1e/problems/{problem_id}/renders\x12\xa7\x01\n\rCreateTestset\x12 .eolymp.atlas.CreateTestsetInput\x1a!.eolymp.atlas.CreateTestsetOutput\"Q\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n2\x82\xd3\xe4\x93\x02!\"\x1f/problems/{problem_id}/testsets\x12\xb4\x01\n\rUpdateTestset\x12 .eolymp.atlas.UpdateTestsetInput\x1a!.eolymp.atlas.UpdateTestsetOutput\"^\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n2\x82\xd3\xe4\x93\x02.\x1a,/problems/{problem_id}/testsets/{testset_id}\x12\xb4\x01\n\rDeleteTestset\x12 .eolymp.atlas.DeleteTestsetInput\x1a!.eolymp.atlas.DeleteTestsetOutput\"^\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n2\x82\xd3\xe4\x93\x02.*,/problems/{problem_id}/testsets/{testset_id}\x12\xa4\x01\n\x0cListTestsets\x12\x1f.eolymp.atlas.ListTestsetsInput\x1a .eolymp.atlas.ListTestsetsOutput\"Q\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\n2\x82\xd3\xe4\x93\x02!\x12\x1f/problems/{problem_id}/testsets\x12\xba\x01\n\x0f\x44\x65scribeTestset\x12\".eolymp.atlas.DescribeTestsetInput\x1a#.eolymp.atlas.DescribeTestsetOutput\"^\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\n2\x82\xd3\xe4\x93\x02.\x12,/problems/{problem_id}/testsets/{testset_id}\x12\xb2\x01\n\nCreateTest\x12\x1d.eolymp.atlas.CreateTestInput\x1a\x1e.eolymp.atlas.CreateTestOutput\"e\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0c\xf5\xe2\n\x00\x00 A\xf8\xe2\n\xc8\x01\x82\xd3\xe4\x93\x02\x34\"2/problems/{problem_id}/testsets/{testset_id}/tests\x12\xbc\x01\n\nUpdateTest\x12\x1d.eolymp.atlas.UpdateTestInput\x1a\x1e.eolymp.atlas.UpdateTestOutput\"o\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0c\xf5\xe2\n\x00\x00 A\xf8\xe2\n\xc8\x01\x82\xd3\xe4\x93\x02>\x1a</problems/{problem_id}/testsets/{testset_id}/tests/{test_id}\x12\xbc\x01\n\nDeleteTest\x12\x1d.eolymp.atlas.DeleteTestInput\x1a\x1e.eolymp.atlas.DeleteTestOutput\"o\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0c\xf5\xe2\n\x00\x00 A\xf8\xe2\n\xc8\x01\x82\xd3\xe4\x93\x02>*</problems/{problem_id}/testsets/{testset_id}/tests/{test_id}\x12\xae\x01\n\tListTests\x12\x1c.eolymp.atlas.ListTestsInput\x1a\x1d.eolymp.atlas.ListTestsOutput\"d\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\n2\x82\xd3\xe4\x93\x02\x34\x12\x32/problems/{problem_id}/testsets/{testset_id}/tests\x12\xc1\x01\n\x0c\x44\x65scribeTest\x12\x1f.eolymp.atlas.DescribeTestInput\x1a .eolymp.atlas.DescribeTestOutput\"n\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\n2\x82\xd3\xe4\x93\x02>\x12</problems/{problem_id}/testsets/{testset_id}/tests/{test_id}\x12\xb7\x01\n\x12\x43reateCodeTemplate\x12%.eolymp.atlas.CreateCodeTemplateInput\x1a&.eolymp.atlas.CreateCodeTemplateOutput\"R\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\n\xd7#>\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\"\" /problems/{problem_id}/templates\x12\xc5\x01\n\x12UpdateCodeTemplate\x12%.eolymp.atlas.UpdateCodeTemplateInput\x1a&.eolymp.atlas.UpdateCodeTemplateOutput\"`\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\n\xd7#>\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x30\"./problems/{problem_id}/templates/{template_id}\x12\xc5\x01\n\x12\x44\x65leteCodeTemplate\x12%.eolymp.atlas.DeleteCodeTemplateInput\x1a&.eolymp.atlas.DeleteCodeTemplateOutput\"`\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\n\xd7#>\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x30*./problems/{problem_id}/templates/{template_id}\x12\xb3\x01\n\x11ListCodeTemplates\x12$.eolymp.atlas.ListCodeTemplatesInput\x1a%.eolymp.atlas.ListCodeTemplatesOutput\"Q\x82\xe3\n\x16\x8a\xe3\n\x12\x61tlas:problem:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0\x41\xf8\xe2\nd\x82\xd3\xe4\x93\x02\"\x12 /problems/{problem_id}/templates\x12\xca\x01\n\x14\x44\x65scribeCodeTemplate\x12\'.eolymp.atlas.DescribeCodeTemplateInput\x1a(.eolymp.atlas.DescribeCodeTemplateOutput\"_\x82\xe3\n\x16\x8a\xe3\n\x12\x61tlas:problem:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0\x41\xf8\xe2\nd\x82\xd3\xe4\x93\x02\x30\x12./problems/{problem_id}/templates/{template_id}\x12\xb5\x01\n\x12LookupCodeTemplate\x12%.eolymp.atlas.LookupCodeTemplateInput\x1a&.eolymp.atlas.LookupCodeTemplateOutput\"P\x82\xe3\n\x16\x8a\xe3\n\x12\x61tlas:problem:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02!\x12\x1f/problems/{problem_id}/template\x12\xb3\x01\n\x10\x43reateAttachment\x12#.eolymp.atlas.CreateAttachmentInput\x1a$.eolymp.atlas.CreateAttachmentOutput\"T\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\n\xd7#>\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02$\"\"/problems/{problem_id}/attachments\x12\xc3\x01\n\x10UpdateAttachment\x12#.eolymp.atlas.UpdateAttachmentInput\x1a$.eolymp.atlas.UpdateAttachmentOutput\"d\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\n\xd7#>\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x34\"2/problems/{problem_id}/attachments/{attachment_id}\x12\xc3\x01\n\x10\x44\x65leteAttachment\x12#.eolymp.atlas.DeleteAttachmentInput\x1a$.eolymp.atlas.DeleteAttachmentOutput\"d\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\n\xd7#>\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x34*2/problems/{problem_id}/attachments/{attachment_id}\x12\xaf\x01\n\x0fListAttachments\x12\".eolymp.atlas.ListAttachmentsInput\x1a#.eolymp.atlas.ListAttachmentsOutput\"S\x82\xe3\n\x16\x8a\xe3\n\x12\x61tlas:problem:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0\x41\xf8\xe2\nd\x82\xd3\xe4\x93\x02$\x12\"/problems/{problem_id}/attachments\x12\xc8\x01\n\x12\x44\x65scribeAttachment\x12%.eolymp.atlas.DescribeAttachmentInput\x1a&.eolymp.atlas.DescribeAttachmentOutput\"c\x82\xe3\n\x16\x8a\xe3\n\x12\x61tlas:problem:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0\x41\xf8\xe2\nd\x82\xd3\xe4\x93\x02\x34\x12\x32/problems/{problem_id}/attachments/{attachment_id}\x12\x95\x01\n\x0cListVersions\x12\x1f.eolymp.atlas.ListVersionsInput\x1a .eolymp.atlas.ListVersionsOutput\"B\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\x82\xd3\xe4\x93\x02!\x12\x1f/problems/{problem_id}/versions\x12\x95\x01\n\x0eListProblemTop\x12!.eolymp.atlas.ListProblemTopInput\x1a\".eolymp.atlas.ListProblemTopOutput\"<\x82\xe3\n\x16\x8a\xe3\n\x12\x61tlas:problem:read\x82\xd3\xe4\x93\x02\x1c\x12\x1a/problems/{problem_id}/top\x12\xb1\x01\n\x16\x44\x65scribeProblemGrading\x12).eolymp.atlas.DescribeProblemGradingInput\x1a*.eolymp.atlas.DescribeProblemGradingOutput\"@\x82\xe3\n\x16\x8a\xe3\n\x12\x61tlas:problem:read\x82\xd3\xe4\x93\x02 \x12\x1e/problems/{problem_id}/grading\x12\xa7\x01\n\x10\x43reateSubmission\x12#.eolymp.atlas.CreateSubmissionInput\x1a$.eolymp.atlas.CreateSubmissionOutput\"H\x82\xe3\n\x1a\x8a\xe3\n\x16\x61tlas:submission:write\x82\xd3\xe4\x93\x02$\"\"/problems/{problem_id}/submissions\x12\xbc\x01\n\x12\x44\x65scribeSubmission\x12%.eolymp.atlas.DescribeSubmissionInput\x1a&.eolymp.atlas.DescribeSubmissionOutput\"W\x82\xe3\n\x19\x8a\xe3\n\x15\x61tlas:submission:read\x82\xd3\xe4\x93\x02\x34\x12\x32/problems/{problem_id}/submissions/{submission_id}\x12\xbe\x01\n\x10RetestSubmission\x12#.eolymp.atlas.RetestSubmissionInput\x1a$.eolymp.atlas.RetestSubmissionOutput\"_\x82\xe3\n\x1a\x8a\xe3\n\x16\x61tlas:submission:write\x82\xd3\xe4\x93\x02;\"9/problems/{problem_id}/submissions/{submission_id}/retest\x12\x8d\x01\n\x0fListSubmissions\x12\".eolymp.atlas.ListSubmissionsInput\x1a#.eolymp.atlas.ListSubmissionsOutput\"1\x82\xe3\n\x19\x8a\xe3\n\x15\x61tlas:submission:read\x82\xd3\xe4\x93\x02\x0e\x12\x0c/submissions\x12\xa2\x01\n\rDescribeScore\x12 .eolymp.atlas.DescribeScoreInput\x1a!.eolymp.atlas.DescribeScoreOutput\"L\x82\xe3\n\x19\x8a\xe3\n\x15\x61tlas:submission:read\x82\xd3\xe4\x93\x02)\x12\'/problems/{problem_id}/scores/{user_id}B-Z+github.com/eolymp/go-sdk/eolymp/atlas;atlasb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'eolymp.atlas.atlas_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z+github.com/eolymp/go-sdk/eolymp/atlas;atlas'
@@ -39,14 +39,16 @@
   _ATLAS.methods_by_name['DeleteProblem']._serialized_options = b'\202\343\n\027\212\343\n\023atlas:problem:write\352\342\n\013\365\342\n\n\327#>\370\342\n\005\202\323\344\223\002\030*\026/problems/{problem_id}'
   _ATLAS.methods_by_name['ListProblems']._options = None
   _ATLAS.methods_by_name['ListProblems']._serialized_options = b'\202\343\n\026\212\343\n\022atlas:problem:read\352\342\n\013\365\342\n\000\000\240A\370\342\nd\202\323\344\223\002\013\022\t/problems'
   _ATLAS.methods_by_name['DescribeProblem']._options = None
   _ATLAS.methods_by_name['DescribeProblem']._serialized_options = b'\202\343\n\026\212\343\n\022atlas:problem:read\352\342\n\013\365\342\n\000\000\240A\370\342\nd\202\323\344\223\002\030\022\026/problems/{problem_id}'
   _ATLAS.methods_by_name['UpdateProblem']._options = None
   _ATLAS.methods_by_name['UpdateProblem']._serialized_options = b'\202\343\n\027\212\343\n\023atlas:problem:write\352\342\n\013\365\342\n\000\000\240A\370\342\nd\202\323\344\223\002\030\032\026/problems/{problem_id}'
+  _ATLAS.methods_by_name['SyncProblem']._options = None
+  _ATLAS.methods_by_name['SyncProblem']._serialized_options = b'\202\343\n\027\212\343\n\023atlas:problem:write\352\342\n\013\365\342\n\n\327#>\370\342\n\005\202\323\344\223\002\035\"\033/problems/{problem_id}/sync'
   _ATLAS.methods_by_name['SetBookmark']._options = None
   _ATLAS.methods_by_name['SetBookmark']._serialized_options = b'\352\342\n\013\365\342\n\000\000\000@\370\342\n\n\202\323\344\223\002!\"\037/problems/{problem_id}/bookmark'
   _ATLAS.methods_by_name['GetBookmark']._options = None
   _ATLAS.methods_by_name['GetBookmark']._serialized_options = b'\352\342\n\013\365\342\n\000\000\310A\370\342\nd\202\323\344\223\002!\022\037/problems/{problem_id}/bookmark'
   _ATLAS.methods_by_name['ListExamples']._options = None
   _ATLAS.methods_by_name['ListExamples']._serialized_options = b'\202\343\n\026\212\343\n\022atlas:problem:read\352\342\n\013\365\342\n\000\000\240A\370\342\nd\202\323\344\223\002!\022\037/problems/{problem_id}/examples'
   _ATLAS.methods_by_name['UpdateTestingConfig']._options = None
@@ -130,9 +132,9 @@
   _ATLAS.methods_by_name['RetestSubmission']._options = None
   _ATLAS.methods_by_name['RetestSubmission']._serialized_options = b'\202\343\n\032\212\343\n\026atlas:submission:write\202\323\344\223\002;\"9/problems/{problem_id}/submissions/{submission_id}/retest'
   _ATLAS.methods_by_name['ListSubmissions']._options = None
   _ATLAS.methods_by_name['ListSubmissions']._serialized_options = b'\202\343\n\031\212\343\n\025atlas:submission:read\202\323\344\223\002\016\022\014/submissions'
   _ATLAS.methods_by_name['DescribeScore']._options = None
   _ATLAS.methods_by_name['DescribeScore']._serialized_options = b'\202\343\n\031\212\343\n\025atlas:submission:read\202\323\344\223\002)\022\'/problems/{problem_id}/scores/{user_id}'
   _ATLAS._serialized_start=481
-  _ATLAS._serialized_end=9388
+  _ATLAS._serialized_end=9548
 # @@protoc_insertion_point(module_scope)
```

### Comparing `eolymp-0.8.1/eolymp/atlas/atlas_pb2.pyi` & `eolymp-0.8.2/eolymp/atlas/atlas_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/atlas/attachment_pb2.py` & `eolymp-0.8.2/eolymp/atlas/attachment_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/atlas/attachment_pb2.pyi` & `eolymp-0.8.2/eolymp/atlas/attachment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/atlas/attachment_service_http.py` & `eolymp-0.8.2/eolymp/atlas/attachment_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/atlas/attachment_service_pb2.py` & `eolymp-0.8.2/eolymp/atlas/attachment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/atlas/attachment_service_pb2.pyi` & `eolymp-0.8.2/eolymp/atlas/attachment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/atlas/bookmark_service_http.py` & `eolymp-0.8.2/eolymp/atlas/bookmark_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/atlas/bookmark_service_pb2.py` & `eolymp-0.8.2/eolymp/atlas/bookmark_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/atlas/bookmark_service_pb2.pyi` & `eolymp-0.8.2/eolymp/atlas/bookmark_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/atlas/code_template_file_pb2.py` & `eolymp-0.8.2/eolymp/atlas/code_template_file_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/atlas/code_template_file_pb2.pyi` & `eolymp-0.8.2/eolymp/atlas/code_template_file_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/atlas/code_template_pb2.py` & `eolymp-0.8.2/eolymp/atlas/code_template_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/atlas/code_template_pb2.pyi` & `eolymp-0.8.2/eolymp/atlas/code_template_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/atlas/code_template_service_http.py` & `eolymp-0.8.2/eolymp/atlas/code_template_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/atlas/code_template_service_pb2.py` & `eolymp-0.8.2/eolymp/atlas/code_template_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/atlas/code_template_service_pb2.pyi` & `eolymp-0.8.2/eolymp/atlas/code_template_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/atlas/editorial_pb2.py` & `eolymp-0.8.2/eolymp/atlas/editorial_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/atlas/editorial_pb2.pyi` & `eolymp-0.8.2/eolymp/atlas/editorial_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/atlas/editorial_service_http.py` & `eolymp-0.8.2/eolymp/atlas/editorial_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/atlas/editorial_service_pb2.py` & `eolymp-0.8.2/eolymp/atlas/editorial_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/atlas/editorial_service_pb2.pyi` & `eolymp-0.8.2/eolymp/atlas/editorial_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/atlas/events_pb2.py` & `eolymp-0.8.2/eolymp/atlas/events_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/atlas/events_pb2.pyi` & `eolymp-0.8.2/eolymp/atlas/events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/atlas/library_service_http.py` & `eolymp-0.8.2/eolymp/atlas/library_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/atlas/library_service_pb2.py` & `eolymp-0.8.2/eolymp/atlas/library_service_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from eolymp.annotations import scope_pb2 as eolymp_dot_annotations_dot_scope__pb2
 from eolymp.atlas import problem_pb2 as eolymp_dot_atlas_dot_problem__pb2
 from eolymp.atlas import statement_pb2 as eolymp_dot_atlas_dot_statement__pb2
 from eolymp.wellknown import direction_pb2 as eolymp_dot_wellknown_dot_direction__pb2
 from eolymp.wellknown import expression_pb2 as eolymp_dot_wellknown_dot_expression__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\"eolymp/atlas/library_service.proto\x12\x0c\x65olymp.atlas\x1a\x1d\x65olymp/annotations/http.proto\x1a\"eolymp/annotations/ratelimit.proto\x1a\x1e\x65olymp/annotations/scope.proto\x1a\x1a\x65olymp/atlas/problem.proto\x1a\x1c\x65olymp/atlas/statement.proto\x1a eolymp/wellknown/direction.proto\x1a!eolymp/wellknown/expression.proto\"h\n\x12\x43reateProblemInput\x12&\n\x07problem\x18\x01 \x01(\x0b\x32\x15.eolymp.atlas.Problem\x12*\n\tstatement\x18\x02 \x01(\x0b\x32\x17.eolymp.atlas.Statement\")\n\x13\x43reateProblemOutput\x12\x12\n\nproblem_id\x18\x01 \x01(\t\"(\n\x12\x44\x65leteProblemInput\x12\x12\n\nproblem_id\x18\x01 \x01(\t\"\x15\n\x13\x44\x65leteProblemOutput\"*\n\x14\x44\x65scribeProblemInput\x12\x12\n\nproblem_id\x18\x01 \x01(\t\"?\n\x15\x44\x65scribeProblemOutput\x12&\n\x07problem\x18\x01 \x01(\x0b\x32\x15.eolymp.atlas.Problem\"\xe7\x05\n\x11ListProblemsInput\x12\x0e\n\x06offset\x18\n \x01(\x05\x12\x0c\n\x04size\x18\x0b \x01(\x05\x12\x37\n\x07\x66ilters\x18( \x01(\x0b\x32&.eolymp.atlas.ListProblemsInput.Filter\x12\x36\n\x04sort\x18\x32 \x01(\x0e\x32(.eolymp.atlas.ListProblemsInput.Sortable\x12*\n\x05order\x18\x33 \x01(\x0e\x32\x1b.eolymp.wellknown.Direction\x1a\xe4\x03\n\x06\x46ilter\x12\r\n\x05query\x18\n \x01(\t\x12*\n\x02id\x18\x01 \x03(\x0b\x32\x1e.eolymp.wellknown.ExpressionID\x12\x30\n\x08topic_id\x18\x02 \x03(\x0b\x32\x1e.eolymp.wellknown.ExpressionID\x12\x34\n\nis_visible\x18\x03 \x03(\x0b\x32 .eolymp.wellknown.ExpressionBool\x12\x34\n\nis_private\x18\x04 \x03(\x0b\x32 .eolymp.wellknown.ExpressionBool\x12/\n\x06number\x18\x05 \x03(\x0b\x32\x1f.eolymp.wellknown.ExpressionInt\x12\x33\n\ndifficulty\x18\x06 \x03(\x0b\x32\x1f.eolymp.wellknown.ExpressionInt\x12\x30\n\x06status\x18\x07 \x03(\x0b\x32 .eolymp.wellknown.ExpressionEnum\x12\x30\n\x05score\x18\t \x03(\x0b\x32!.eolymp.wellknown.ExpressionFloat\x12\x37\n\ris_bookmarked\x18\x08 \x03(\x0b\x32 .eolymp.wellknown.ExpressionBool\"0\n\x08Sortable\x12\x0b\n\x07\x44\x45\x46\x41ULT\x10\x00\x12\n\n\x06RECENT\x10\x01\x12\x0b\n\x07POPULAR\x10\x02\"I\n\x12ListProblemsOutput\x12\r\n\x05total\x18\x01 \x01(\x05\x12$\n\x05items\x18\x02 \x03(\x0b\x32\x15.eolymp.atlas.Problem\"<\n\x15UpdateVisibilityInput\x12\x12\n\nproblem_id\x18\x01 \x01(\t\x12\x0f\n\x07visible\x18\x02 \x01(\x08\"\x18\n\x16UpdateVisibilityOutput\"9\n\x12UpdatePrivacyInput\x12\x12\n\nproblem_id\x18\x01 \x01(\t\x12\x0f\n\x07private\x18\x02 \x01(\x08\"\x15\n\x13UpdatePrivacyOutput\"\xcf\x01\n\x12UpdateProblemInput\x12\x35\n\x05patch\x18\x01 \x03(\x0e\x32&.eolymp.atlas.UpdateProblemInput.Patch\x12\x12\n\nproblem_id\x18\x02 \x01(\t\x12&\n\x07problem\x18\x03 \x01(\x0b\x32\x15.eolymp.atlas.Problem\"F\n\x05Patch\x12\x07\n\x03\x41LL\x10\x00\x12\x0b\n\x07VISIBLE\x10\x01\x12\x0b\n\x07PRIVATE\x10\x02\x12\n\n\x06TOPICS\x10\x03\x12\x0e\n\nDIFFICULTY\x10\x04\"\x15\n\x13UpdateProblemOutput2\xfb\x04\n\x0eLibraryService\x12\x91\x01\n\rCreateProblem\x12 .eolymp.atlas.CreateProblemInput\x1a!.eolymp.atlas.CreateProblemOutput\";\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\n\xd7#>\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x0b\"\t/problems\x12\x9e\x01\n\rDeleteProblem\x12 .eolymp.atlas.DeleteProblemInput\x1a!.eolymp.atlas.DeleteProblemOutput\"H\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\n\xd7#>\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x18*\x16/problems/{problem_id}\x12\xa3\x01\n\x0f\x44\x65scribeProblem\x12\".eolymp.atlas.DescribeProblemInput\x1a#.eolymp.atlas.DescribeProblemOutput\"G\x82\xe3\n\x16\x8a\xe3\n\x12\x61tlas:problem:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0\x41\xf8\xe2\nd\x82\xd3\xe4\x93\x02\x18\x12\x16/problems/{problem_id}\x12\x8d\x01\n\x0cListProblems\x12\x1f.eolymp.atlas.ListProblemsInput\x1a .eolymp.atlas.ListProblemsOutput\":\x82\xe3\n\x16\x8a\xe3\n\x12\x61tlas:problem:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0\x41\xf8\xe2\nd\x82\xd3\xe4\x93\x02\x0b\x12\t/problemsB-Z+github.com/eolymp/go-sdk/eolymp/atlas;atlasb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\"eolymp/atlas/library_service.proto\x12\x0c\x65olymp.atlas\x1a\x1d\x65olymp/annotations/http.proto\x1a\"eolymp/annotations/ratelimit.proto\x1a\x1e\x65olymp/annotations/scope.proto\x1a\x1a\x65olymp/atlas/problem.proto\x1a\x1c\x65olymp/atlas/statement.proto\x1a eolymp/wellknown/direction.proto\x1a!eolymp/wellknown/expression.proto\"h\n\x12\x43reateProblemInput\x12&\n\x07problem\x18\x01 \x01(\x0b\x32\x15.eolymp.atlas.Problem\x12*\n\tstatement\x18\x02 \x01(\x0b\x32\x17.eolymp.atlas.Statement\")\n\x13\x43reateProblemOutput\x12\x12\n\nproblem_id\x18\x01 \x01(\t\"(\n\x12\x44\x65leteProblemInput\x12\x12\n\nproblem_id\x18\x01 \x01(\t\"\x15\n\x13\x44\x65leteProblemOutput\"*\n\x14\x44\x65scribeProblemInput\x12\x12\n\nproblem_id\x18\x01 \x01(\t\"?\n\x15\x44\x65scribeProblemOutput\x12&\n\x07problem\x18\x01 \x01(\x0b\x32\x15.eolymp.atlas.Problem\"\xe7\x05\n\x11ListProblemsInput\x12\x0e\n\x06offset\x18\n \x01(\x05\x12\x0c\n\x04size\x18\x0b \x01(\x05\x12\x37\n\x07\x66ilters\x18( \x01(\x0b\x32&.eolymp.atlas.ListProblemsInput.Filter\x12\x36\n\x04sort\x18\x32 \x01(\x0e\x32(.eolymp.atlas.ListProblemsInput.Sortable\x12*\n\x05order\x18\x33 \x01(\x0e\x32\x1b.eolymp.wellknown.Direction\x1a\xe4\x03\n\x06\x46ilter\x12\r\n\x05query\x18\n \x01(\t\x12*\n\x02id\x18\x01 \x03(\x0b\x32\x1e.eolymp.wellknown.ExpressionID\x12\x30\n\x08topic_id\x18\x02 \x03(\x0b\x32\x1e.eolymp.wellknown.ExpressionID\x12\x34\n\nis_visible\x18\x03 \x03(\x0b\x32 .eolymp.wellknown.ExpressionBool\x12\x34\n\nis_private\x18\x04 \x03(\x0b\x32 .eolymp.wellknown.ExpressionBool\x12/\n\x06number\x18\x05 \x03(\x0b\x32\x1f.eolymp.wellknown.ExpressionInt\x12\x33\n\ndifficulty\x18\x06 \x03(\x0b\x32\x1f.eolymp.wellknown.ExpressionInt\x12\x30\n\x06status\x18\x07 \x03(\x0b\x32 .eolymp.wellknown.ExpressionEnum\x12\x30\n\x05score\x18\t \x03(\x0b\x32!.eolymp.wellknown.ExpressionFloat\x12\x37\n\ris_bookmarked\x18\x08 \x03(\x0b\x32 .eolymp.wellknown.ExpressionBool\"0\n\x08Sortable\x12\x0b\n\x07\x44\x45\x46\x41ULT\x10\x00\x12\n\n\x06RECENT\x10\x01\x12\x0b\n\x07POPULAR\x10\x02\"I\n\x12ListProblemsOutput\x12\r\n\x05total\x18\x01 \x01(\x05\x12$\n\x05items\x18\x02 \x03(\x0b\x32\x15.eolymp.atlas.Problem\"<\n\x15UpdateVisibilityInput\x12\x12\n\nproblem_id\x18\x01 \x01(\t\x12\x0f\n\x07visible\x18\x02 \x01(\x08\"\x18\n\x16UpdateVisibilityOutput\"9\n\x12UpdatePrivacyInput\x12\x12\n\nproblem_id\x18\x01 \x01(\t\x12\x0f\n\x07private\x18\x02 \x01(\x08\"\x15\n\x13UpdatePrivacyOutput\"\xdb\x01\n\x12UpdateProblemInput\x12\x35\n\x05patch\x18\x01 \x03(\x0e\x32&.eolymp.atlas.UpdateProblemInput.Patch\x12\x12\n\nproblem_id\x18\x02 \x01(\t\x12&\n\x07problem\x18\x03 \x01(\x0b\x32\x15.eolymp.atlas.Problem\"R\n\x05Patch\x12\x07\n\x03\x41LL\x10\x00\x12\x0b\n\x07VISIBLE\x10\x01\x12\x0b\n\x07PRIVATE\x10\x02\x12\n\n\x06TOPICS\x10\x03\x12\x0e\n\nDIFFICULTY\x10\x04\x12\n\n\x06ORIGIN\x10\x05\"\x15\n\x13UpdateProblemOutput\"&\n\x10SyncProblemInput\x12\x12\n\nproblem_id\x18\x01 \x01(\t\"\x13\n\x11SyncProblemOutput2\xfb\x04\n\x0eLibraryService\x12\x91\x01\n\rCreateProblem\x12 .eolymp.atlas.CreateProblemInput\x1a!.eolymp.atlas.CreateProblemOutput\";\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\n\xd7#>\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x0b\"\t/problems\x12\x9e\x01\n\rDeleteProblem\x12 .eolymp.atlas.DeleteProblemInput\x1a!.eolymp.atlas.DeleteProblemOutput\"H\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\n\xd7#>\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x18*\x16/problems/{problem_id}\x12\xa3\x01\n\x0f\x44\x65scribeProblem\x12\".eolymp.atlas.DescribeProblemInput\x1a#.eolymp.atlas.DescribeProblemOutput\"G\x82\xe3\n\x16\x8a\xe3\n\x12\x61tlas:problem:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0\x41\xf8\xe2\nd\x82\xd3\xe4\x93\x02\x18\x12\x16/problems/{problem_id}\x12\x8d\x01\n\x0cListProblems\x12\x1f.eolymp.atlas.ListProblemsInput\x1a .eolymp.atlas.ListProblemsOutput\":\x82\xe3\n\x16\x8a\xe3\n\x12\x61tlas:problem:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0\x41\xf8\xe2\nd\x82\xd3\xe4\x93\x02\x0b\x12\t/problemsB-Z+github.com/eolymp/go-sdk/eolymp/atlas;atlasb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'eolymp.atlas.library_service_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z+github.com/eolymp/go-sdk/eolymp/atlas;atlas'
@@ -61,15 +61,19 @@
   _UPDATEVISIBILITYOUTPUT._serialized_start=1484
   _UPDATEVISIBILITYOUTPUT._serialized_end=1508
   _UPDATEPRIVACYINPUT._serialized_start=1510
   _UPDATEPRIVACYINPUT._serialized_end=1567
   _UPDATEPRIVACYOUTPUT._serialized_start=1569
   _UPDATEPRIVACYOUTPUT._serialized_end=1590
   _UPDATEPROBLEMINPUT._serialized_start=1593
-  _UPDATEPROBLEMINPUT._serialized_end=1800
+  _UPDATEPROBLEMINPUT._serialized_end=1812
   _UPDATEPROBLEMINPUT_PATCH._serialized_start=1730
-  _UPDATEPROBLEMINPUT_PATCH._serialized_end=1800
-  _UPDATEPROBLEMOUTPUT._serialized_start=1802
-  _UPDATEPROBLEMOUTPUT._serialized_end=1823
-  _LIBRARYSERVICE._serialized_start=1826
-  _LIBRARYSERVICE._serialized_end=2461
+  _UPDATEPROBLEMINPUT_PATCH._serialized_end=1812
+  _UPDATEPROBLEMOUTPUT._serialized_start=1814
+  _UPDATEPROBLEMOUTPUT._serialized_end=1835
+  _SYNCPROBLEMINPUT._serialized_start=1837
+  _SYNCPROBLEMINPUT._serialized_end=1875
+  _SYNCPROBLEMOUTPUT._serialized_start=1877
+  _SYNCPROBLEMOUTPUT._serialized_end=1896
+  _LIBRARYSERVICE._serialized_start=1899
+  _LIBRARYSERVICE._serialized_end=2534
 # @@protoc_insertion_point(module_scope)
```

### Comparing `eolymp-0.8.1/eolymp/atlas/library_service_pb2.pyi` & `eolymp-0.8.2/eolymp/atlas/library_service_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -95,14 +95,24 @@
     __slots__ = ["items", "total"]
     ITEMS_FIELD_NUMBER: _ClassVar[int]
     TOTAL_FIELD_NUMBER: _ClassVar[int]
     items: _containers.RepeatedCompositeFieldContainer[_problem_pb2.Problem]
     total: int
     def __init__(self, total: _Optional[int] = ..., items: _Optional[_Iterable[_Union[_problem_pb2.Problem, _Mapping]]] = ...) -> None: ...
 
+class SyncProblemInput(_message.Message):
+    __slots__ = ["problem_id"]
+    PROBLEM_ID_FIELD_NUMBER: _ClassVar[int]
+    problem_id: str
+    def __init__(self, problem_id: _Optional[str] = ...) -> None: ...
+
+class SyncProblemOutput(_message.Message):
+    __slots__ = []
+    def __init__(self) -> None: ...
+
 class UpdatePrivacyInput(_message.Message):
     __slots__ = ["private", "problem_id"]
     PRIVATE_FIELD_NUMBER: _ClassVar[int]
     PROBLEM_ID_FIELD_NUMBER: _ClassVar[int]
     private: bool
     problem_id: str
     def __init__(self, problem_id: _Optional[str] = ..., private: bool = ...) -> None: ...
@@ -113,14 +123,15 @@
 
 class UpdateProblemInput(_message.Message):
     __slots__ = ["patch", "problem", "problem_id"]
     class Patch(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = []
     ALL: UpdateProblemInput.Patch
     DIFFICULTY: UpdateProblemInput.Patch
+    ORIGIN: UpdateProblemInput.Patch
     PATCH_FIELD_NUMBER: _ClassVar[int]
     PRIVATE: UpdateProblemInput.Patch
     PROBLEM_FIELD_NUMBER: _ClassVar[int]
     PROBLEM_ID_FIELD_NUMBER: _ClassVar[int]
     TOPICS: UpdateProblemInput.Patch
     VISIBLE: UpdateProblemInput.Patch
     patch: _containers.RepeatedScalarFieldContainer[UpdateProblemInput.Patch]
```

### Comparing `eolymp-0.8.1/eolymp/atlas/problem_pb2.py` & `eolymp-0.8.2/eolymp/atlas/problem_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,24 +10,24 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from eolymp.annotations import endpoint_pb2 as eolymp_dot_annotations_dot_endpoint__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1a\x65olymp/atlas/problem.proto\x12\x0c\x65olymp.atlas\x1a!eolymp/annotations/endpoint.proto\"\x9c\x04\n\x07Problem\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x03url\x18\xaa\x05 \x01(\t\x12\x30\n\x05links\x18\xab\x05 \x03(\x0b\x32 .eolymp.atlas.Problem.LinksEntry\x12\x0e\n\x06number\x18\n \x01(\x05\x12\x0f\n\x07visible\x18\x0b \x01(\x08\x12\x0f\n\x07private\x18\x0c \x01(\x08\x12\x0e\n\x06topics\x18\x14 \x03(\t\x12\x12\n\ndifficulty\x18\x15 \x01(\r\x1a,\n\nLinksEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01:\xc0\x02\xda\xe3\n\xbb\x02\x12\x17\n\x15\x65olymp.acl.AclService\x12\x1b\n\x19\x65olymp.atlas.AssetService\x12 \n\x1e\x65olymp.atlas.AttachmentService\x12\"\n eolymp.atlas.CodeTemplateService\x12\x1d\n\x1b\x65olymp.atlas.ProblemService\x12\x1d\n\x1b\x65olymp.atlas.ScoringService\x12\x1f\n\x1d\x65olymp.atlas.StatementService\x12 \n\x1e\x65olymp.atlas.SubmissionService\x12\x1d\n\x1b\x65olymp.atlas.TestingService\x12\x1d\n\x1b\x65olymp.worker.WorkerServiceB-Z+github.com/eolymp/go-sdk/eolymp/atlas;atlasb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1a\x65olymp/atlas/problem.proto\x12\x0c\x65olymp.atlas\x1a!eolymp/annotations/endpoint.proto\"\xac\x04\n\x07Problem\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x03url\x18\xaa\x05 \x01(\t\x12\x30\n\x05links\x18\xab\x05 \x03(\x0b\x32 .eolymp.atlas.Problem.LinksEntry\x12\x0e\n\x06number\x18\n \x01(\x05\x12\x0f\n\x07visible\x18\x0b \x01(\x08\x12\x0f\n\x07private\x18\x0c \x01(\x08\x12\x0e\n\x06origin\x18\r \x01(\t\x12\x0e\n\x06topics\x18\x14 \x03(\t\x12\x12\n\ndifficulty\x18\x15 \x01(\r\x1a,\n\nLinksEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01:\xc0\x02\xda\xe3\n\xbb\x02\x12\x17\n\x15\x65olymp.acl.AclService\x12\x1b\n\x19\x65olymp.atlas.AssetService\x12 \n\x1e\x65olymp.atlas.AttachmentService\x12\"\n eolymp.atlas.CodeTemplateService\x12\x1d\n\x1b\x65olymp.atlas.ProblemService\x12\x1d\n\x1b\x65olymp.atlas.ScoringService\x12\x1f\n\x1d\x65olymp.atlas.StatementService\x12 \n\x1e\x65olymp.atlas.SubmissionService\x12\x1d\n\x1b\x65olymp.atlas.TestingService\x12\x1d\n\x1b\x65olymp.worker.WorkerServiceB-Z+github.com/eolymp/go-sdk/eolymp/atlas;atlasb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'eolymp.atlas.problem_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z+github.com/eolymp/go-sdk/eolymp/atlas;atlas'
   _PROBLEM_LINKSENTRY._options = None
   _PROBLEM_LINKSENTRY._serialized_options = b'8\001'
   _PROBLEM._options = None
   _PROBLEM._serialized_options = b'\332\343\n\273\002\022\027\n\025eolymp.acl.AclService\022\033\n\031eolymp.atlas.AssetService\022 \n\036eolymp.atlas.AttachmentService\022\"\n eolymp.atlas.CodeTemplateService\022\035\n\033eolymp.atlas.ProblemService\022\035\n\033eolymp.atlas.ScoringService\022\037\n\035eolymp.atlas.StatementService\022 \n\036eolymp.atlas.SubmissionService\022\035\n\033eolymp.atlas.TestingService\022\035\n\033eolymp.worker.WorkerService'
   _PROBLEM._serialized_start=80
-  _PROBLEM._serialized_end=620
-  _PROBLEM_LINKSENTRY._serialized_start=253
-  _PROBLEM_LINKSENTRY._serialized_end=297
+  _PROBLEM._serialized_end=636
+  _PROBLEM_LINKSENTRY._serialized_start=269
+  _PROBLEM_LINKSENTRY._serialized_end=313
 # @@protoc_insertion_point(module_scope)
```

### Comparing `eolymp-0.8.1/eolymp/atlas/problem_pb2.pyi` & `eolymp-0.8.2/eolymp/atlas/problem_pb2.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -3,32 +3,34 @@
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class Problem(_message.Message):
-    __slots__ = ["difficulty", "id", "links", "number", "private", "topics", "url", "visible"]
+    __slots__ = ["difficulty", "id", "links", "number", "origin", "private", "topics", "url", "visible"]
     class LinksEntry(_message.Message):
         __slots__ = ["key", "value"]
         KEY_FIELD_NUMBER: _ClassVar[int]
         VALUE_FIELD_NUMBER: _ClassVar[int]
         key: str
         value: str
         def __init__(self, key: _Optional[str] = ..., value: _Optional[str] = ...) -> None: ...
     DIFFICULTY_FIELD_NUMBER: _ClassVar[int]
     ID_FIELD_NUMBER: _ClassVar[int]
     LINKS_FIELD_NUMBER: _ClassVar[int]
     NUMBER_FIELD_NUMBER: _ClassVar[int]
+    ORIGIN_FIELD_NUMBER: _ClassVar[int]
     PRIVATE_FIELD_NUMBER: _ClassVar[int]
     TOPICS_FIELD_NUMBER: _ClassVar[int]
     URL_FIELD_NUMBER: _ClassVar[int]
     VISIBLE_FIELD_NUMBER: _ClassVar[int]
     difficulty: int
     id: str
     links: _containers.ScalarMap[str, str]
     number: int
+    origin: str
     private: bool
     topics: _containers.RepeatedScalarFieldContainer[str]
     url: str
     visible: bool
-    def __init__(self, id: _Optional[str] = ..., url: _Optional[str] = ..., links: _Optional[_Mapping[str, str]] = ..., number: _Optional[int] = ..., visible: bool = ..., private: bool = ..., topics: _Optional[_Iterable[str]] = ..., difficulty: _Optional[int] = ...) -> None: ...
+    def __init__(self, id: _Optional[str] = ..., url: _Optional[str] = ..., links: _Optional[_Mapping[str, str]] = ..., number: _Optional[int] = ..., visible: bool = ..., private: bool = ..., origin: _Optional[str] = ..., topics: _Optional[_Iterable[str]] = ..., difficulty: _Optional[int] = ...) -> None: ...
```

### Comparing `eolymp-0.8.1/eolymp/atlas/problem_service_http.py` & `eolymp-0.8.2/eolymp/worker/worker_service_http.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,78 +5,89 @@
 
 import urllib.parse
 from google.protobuf import symbol_database as _symbol_database
 
 _sym_db = _symbol_database.Default()
 
 
-class ProblemServiceClient:
+class WorkerClient:
     def __init__(self, transport, url="https://api.eolymp.com"):
         self.transport = transport
         self.url = url
 
-    def DeleteProblem(self, request, **kwargs):
-        path = "/"
+    def CreateJob(self, request, **kwargs):
+        path = "/jobs"
 
         return self.transport.request(
-            method="DELETE",
+            method="POST",
             url=self.url+path,
             request_data=request,
-            response_symbol=_sym_db.GetSymbol("eolymp.atlas.DeleteProblemOutput"),
+            response_symbol=_sym_db.GetSymbol("eolymp.worker.CreateJobOutput"),
             **kwargs,
         )
 
-    def UpdateProblem(self, request, **kwargs):
-        path = "/"
+    def DescribeJob(self, request, **kwargs):
+        path = "/jobs/"+urllib.parse.quote(request.job_id)
+
+        # Cleanup URL parameters to avoid any ambiguity
+        request.job_id = ""
 
         return self.transport.request(
-            method="PUT",
+            method="GET",
             url=self.url+path,
             request_data=request,
-            response_symbol=_sym_db.GetSymbol("eolymp.atlas.UpdateProblemOutput"),
+            response_symbol=_sym_db.GetSymbol("eolymp.worker.DescribeJobOutput"),
             **kwargs,
         )
 
-    def DescribeProblem(self, request, **kwargs):
-        path = "/"
+    def ListJobs(self, request, **kwargs):
+        path = "/jobs"
 
         return self.transport.request(
             method="GET",
             url=self.url+path,
             request_data=request,
-            response_symbol=_sym_db.GetSymbol("eolymp.atlas.DescribeProblemOutput"),
+            response_symbol=_sym_db.GetSymbol("eolymp.worker.ListJobsOutput"),
             **kwargs,
         )
 
-    def UpdateVisibility(self, request, **kwargs):
-        path = "/visibility"
+class WorkerServiceClient:
+    def __init__(self, transport, url="https://api.eolymp.com"):
+        self.transport = transport
+        self.url = url
+
+    def CreateJob(self, request, **kwargs):
+        path = "/jobs"
 
         return self.transport.request(
             method="POST",
             url=self.url+path,
             request_data=request,
-            response_symbol=_sym_db.GetSymbol("eolymp.atlas.UpdateVisibilityOutput"),
+            response_symbol=_sym_db.GetSymbol("eolymp.worker.CreateJobOutput"),
             **kwargs,
         )
 
-    def UpdatePrivacy(self, request, **kwargs):
-        path = "/privacy"
+    def DescribeJob(self, request, **kwargs):
+        path = "/jobs/"+urllib.parse.quote(request.job_id)
+
+        # Cleanup URL parameters to avoid any ambiguity
+        request.job_id = ""
 
         return self.transport.request(
-            method="POST",
+            method="GET",
             url=self.url+path,
             request_data=request,
-            response_symbol=_sym_db.GetSymbol("eolymp.atlas.UpdatePrivacyOutput"),
+            response_symbol=_sym_db.GetSymbol("eolymp.worker.DescribeJobOutput"),
             **kwargs,
         )
 
-    def ListVersions(self, request, **kwargs):
-        path = "/versions"
+    def ListJobs(self, request, **kwargs):
+        path = "/jobs"
 
         return self.transport.request(
             method="GET",
             url=self.url+path,
             request_data=request,
-            response_symbol=_sym_db.GetSymbol("eolymp.atlas.ListVersionsOutput"),
+            response_symbol=_sym_db.GetSymbol("eolymp.worker.ListJobsOutput"),
             **kwargs,
         )
```

### Comparing `eolymp-0.8.1/eolymp/atlas/problem_service_pb2.py` & `eolymp-0.8.2/eolymp/atlas/problem_service_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,26 +15,28 @@
 from eolymp.annotations import ratelimit_pb2 as eolymp_dot_annotations_dot_ratelimit__pb2
 from eolymp.annotations import scope_pb2 as eolymp_dot_annotations_dot_scope__pb2
 from eolymp.atlas import library_service_pb2 as eolymp_dot_atlas_dot_library__service__pb2
 from eolymp.atlas import version_pb2 as eolymp_dot_atlas_dot_version__pb2
 from eolymp.wellknown import expression_pb2 as eolymp_dot_wellknown_dot_expression__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\"eolymp/atlas/problem_service.proto\x12\x0c\x65olymp.atlas\x1a\x1d\x65olymp/annotations/http.proto\x1a\"eolymp/annotations/ratelimit.proto\x1a\x1e\x65olymp/annotations/scope.proto\x1a\"eolymp/atlas/library_service.proto\x1a\x1a\x65olymp/atlas/version.proto\x1a!eolymp/wellknown/expression.proto\"\x97\x03\n\x11ListVersionsInput\x12\x12\n\nproblem_id\x18\x01 \x01(\t\x12\x0e\n\x06offset\x18\n \x01(\x05\x12\x0c\n\x04size\x18\x0b \x01(\x05\x12\x37\n\x07\x66ilters\x18( \x01(\x0b\x32&.eolymp.atlas.ListVersionsInput.Filter\x1a\x96\x02\n\x06\x46ilter\x12/\n\x06number\x18\x01 \x03(\x0b\x32\x1f.eolymp.wellknown.ExpressionInt\x12\x32\n\ncreated_by\x18\x02 \x03(\x0b\x32\x1e.eolymp.wellknown.ExpressionID\x12\x39\n\ncreated_at\x18\x03 \x03(\x0b\x32%.eolymp.wellknown.ExpressionTimestamp\x12\x33\n\tchange_op\x18\x04 \x03(\x0b\x32 .eolymp.wellknown.ExpressionEnum\x12\x37\n\x0b\x63hange_path\x18\x05 \x03(\x0b\x32\".eolymp.wellknown.ExpressionString\"I\n\x12ListVersionsOutput\x12\r\n\x05total\x18\x01 \x01(\x05\x12$\n\x05items\x18\x02 \x03(\x0b\x32\x15.eolymp.atlas.Version2\xe9\x06\n\x0eProblemService\x12\x88\x01\n\rDeleteProblem\x12 .eolymp.atlas.DeleteProblemInput\x1a!.eolymp.atlas.DeleteProblemOutput\"2\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\n\xd7#>\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x02*\x00\x12\x88\x01\n\rUpdateProblem\x12 .eolymp.atlas.UpdateProblemInput\x1a!.eolymp.atlas.UpdateProblemOutput\"2\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0\x41\xf8\xe2\nd\x82\xd3\xe4\x93\x02\x02\x1a\x00\x12\x8d\x01\n\x0f\x44\x65scribeProblem\x12\".eolymp.atlas.DescribeProblemInput\x1a#.eolymp.atlas.DescribeProblemOutput\"1\x82\xe3\n\x16\x8a\xe3\n\x12\x61tlas:problem:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0\x41\xf8\xe2\nd\x82\xd3\xe4\x93\x02\x02\x12\x00\x12\x9c\x01\n\x10UpdateVisibility\x12#.eolymp.atlas.UpdateVisibilityInput\x1a$.eolymp.atlas.UpdateVisibilityOutput\"=\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0\x41\xf8\xe2\nd\x82\xd3\xe4\x93\x02\r\"\x0b/visibility\x12\x90\x01\n\rUpdatePrivacy\x12 .eolymp.atlas.UpdatePrivacyInput\x1a!.eolymp.atlas.UpdatePrivacyOutput\":\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0\x41\xf8\xe2\nd\x82\xd3\xe4\x93\x02\n\"\x08/privacy\x12\x7f\n\x0cListVersions\x12\x1f.eolymp.atlas.ListVersionsInput\x1a .eolymp.atlas.ListVersionsOutput\",\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\x82\xd3\xe4\x93\x02\x0b\x12\t/versionsB-Z+github.com/eolymp/go-sdk/eolymp/atlas;atlasb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\"eolymp/atlas/problem_service.proto\x12\x0c\x65olymp.atlas\x1a\x1d\x65olymp/annotations/http.proto\x1a\"eolymp/annotations/ratelimit.proto\x1a\x1e\x65olymp/annotations/scope.proto\x1a\"eolymp/atlas/library_service.proto\x1a\x1a\x65olymp/atlas/version.proto\x1a!eolymp/wellknown/expression.proto\"\x97\x03\n\x11ListVersionsInput\x12\x12\n\nproblem_id\x18\x01 \x01(\t\x12\x0e\n\x06offset\x18\n \x01(\x05\x12\x0c\n\x04size\x18\x0b \x01(\x05\x12\x37\n\x07\x66ilters\x18( \x01(\x0b\x32&.eolymp.atlas.ListVersionsInput.Filter\x1a\x96\x02\n\x06\x46ilter\x12/\n\x06number\x18\x01 \x03(\x0b\x32\x1f.eolymp.wellknown.ExpressionInt\x12\x32\n\ncreated_by\x18\x02 \x03(\x0b\x32\x1e.eolymp.wellknown.ExpressionID\x12\x39\n\ncreated_at\x18\x03 \x03(\x0b\x32%.eolymp.wellknown.ExpressionTimestamp\x12\x33\n\tchange_op\x18\x04 \x03(\x0b\x32 .eolymp.wellknown.ExpressionEnum\x12\x37\n\x0b\x63hange_path\x18\x05 \x03(\x0b\x32\".eolymp.wellknown.ExpressionString\"I\n\x12ListVersionsOutput\x12\r\n\x05total\x18\x01 \x01(\x05\x12$\n\x05items\x18\x02 \x03(\x0b\x32\x15.eolymp.atlas.Version2\xf3\x07\n\x0eProblemService\x12\x88\x01\n\rDeleteProblem\x12 .eolymp.atlas.DeleteProblemInput\x1a!.eolymp.atlas.DeleteProblemOutput\"2\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\n\xd7#>\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x02*\x00\x12\x88\x01\n\rUpdateProblem\x12 .eolymp.atlas.UpdateProblemInput\x1a!.eolymp.atlas.UpdateProblemOutput\"2\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0\x41\xf8\xe2\nd\x82\xd3\xe4\x93\x02\x02\x1a\x00\x12\x87\x01\n\x0bSyncProblem\x12\x1e.eolymp.atlas.SyncProblemInput\x1a\x1f.eolymp.atlas.SyncProblemOutput\"7\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\n\xd7#>\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x07\"\x05/sync\x12\x8d\x01\n\x0f\x44\x65scribeProblem\x12\".eolymp.atlas.DescribeProblemInput\x1a#.eolymp.atlas.DescribeProblemOutput\"1\x82\xe3\n\x16\x8a\xe3\n\x12\x61tlas:problem:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0\x41\xf8\xe2\nd\x82\xd3\xe4\x93\x02\x02\x12\x00\x12\x9c\x01\n\x10UpdateVisibility\x12#.eolymp.atlas.UpdateVisibilityInput\x1a$.eolymp.atlas.UpdateVisibilityOutput\"=\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0\x41\xf8\xe2\nd\x82\xd3\xe4\x93\x02\r\"\x0b/visibility\x12\x90\x01\n\rUpdatePrivacy\x12 .eolymp.atlas.UpdatePrivacyInput\x1a!.eolymp.atlas.UpdatePrivacyOutput\":\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0\x41\xf8\xe2\nd\x82\xd3\xe4\x93\x02\n\"\x08/privacy\x12\x7f\n\x0cListVersions\x12\x1f.eolymp.atlas.ListVersionsInput\x1a .eolymp.atlas.ListVersionsOutput\",\x82\xe3\n\x17\x8a\xe3\n\x13\x61tlas:problem:write\x82\xd3\xe4\x93\x02\x0b\x12\t/versionsB-Z+github.com/eolymp/go-sdk/eolymp/atlas;atlasb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'eolymp.atlas.problem_service_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z+github.com/eolymp/go-sdk/eolymp/atlas;atlas'
   _PROBLEMSERVICE.methods_by_name['DeleteProblem']._options = None
   _PROBLEMSERVICE.methods_by_name['DeleteProblem']._serialized_options = b'\202\343\n\027\212\343\n\023atlas:problem:write\352\342\n\013\365\342\n\n\327#>\370\342\n\005\202\323\344\223\002\002*\000'
   _PROBLEMSERVICE.methods_by_name['UpdateProblem']._options = None
   _PROBLEMSERVICE.methods_by_name['UpdateProblem']._serialized_options = b'\202\343\n\027\212\343\n\023atlas:problem:write\352\342\n\013\365\342\n\000\000\240A\370\342\nd\202\323\344\223\002\002\032\000'
+  _PROBLEMSERVICE.methods_by_name['SyncProblem']._options = None
+  _PROBLEMSERVICE.methods_by_name['SyncProblem']._serialized_options = b'\202\343\n\027\212\343\n\023atlas:problem:write\352\342\n\013\365\342\n\n\327#>\370\342\n\005\202\323\344\223\002\007\"\005/sync'
   _PROBLEMSERVICE.methods_by_name['DescribeProblem']._options = None
   _PROBLEMSERVICE.methods_by_name['DescribeProblem']._serialized_options = b'\202\343\n\026\212\343\n\022atlas:problem:read\352\342\n\013\365\342\n\000\000\240A\370\342\nd\202\323\344\223\002\002\022\000'
   _PROBLEMSERVICE.methods_by_name['UpdateVisibility']._options = None
   _PROBLEMSERVICE.methods_by_name['UpdateVisibility']._serialized_options = b'\202\343\n\027\212\343\n\023atlas:problem:write\352\342\n\013\365\342\n\000\000\240A\370\342\nd\202\323\344\223\002\r\"\013/visibility'
   _PROBLEMSERVICE.methods_by_name['UpdatePrivacy']._options = None
   _PROBLEMSERVICE.methods_by_name['UpdatePrivacy']._serialized_options = b'\202\343\n\027\212\343\n\023atlas:problem:write\352\342\n\013\365\342\n\000\000\240A\370\342\nd\202\323\344\223\002\n\"\010/privacy'
   _PROBLEMSERVICE.methods_by_name['ListVersions']._options = None
@@ -42,9 +44,9 @@
   _LISTVERSIONSINPUT._serialized_start=251
   _LISTVERSIONSINPUT._serialized_end=658
   _LISTVERSIONSINPUT_FILTER._serialized_start=380
   _LISTVERSIONSINPUT_FILTER._serialized_end=658
   _LISTVERSIONSOUTPUT._serialized_start=660
   _LISTVERSIONSOUTPUT._serialized_end=733
   _PROBLEMSERVICE._serialized_start=736
-  _PROBLEMSERVICE._serialized_end=1609
+  _PROBLEMSERVICE._serialized_end=1747
 # @@protoc_insertion_point(module_scope)
```

### Comparing `eolymp-0.8.1/eolymp/atlas/problem_service_pb2.pyi` & `eolymp-0.8.2/eolymp/atlas/problem_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/atlas/scoring_score_pb2.py` & `eolymp-0.8.2/eolymp/atlas/scoring_score_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/atlas/scoring_score_pb2.pyi` & `eolymp-0.8.2/eolymp/atlas/scoring_score_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/atlas/scoring_service_http.py` & `eolymp-0.8.2/eolymp/atlas/scoring_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/atlas/scoring_service_pb2.py` & `eolymp-0.8.2/eolymp/atlas/scoring_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/atlas/scoring_service_pb2.pyi` & `eolymp-0.8.2/eolymp/atlas/scoring_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/atlas/solution_pb2.py` & `eolymp-0.8.2/eolymp/atlas/solution_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/atlas/solution_pb2.pyi` & `eolymp-0.8.2/eolymp/atlas/solution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/atlas/statement_pb2.py` & `eolymp-0.8.2/eolymp/atlas/statement_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/atlas/statement_pb2.pyi` & `eolymp-0.8.2/eolymp/atlas/statement_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/atlas/statement_service_http.py` & `eolymp-0.8.2/eolymp/atlas/statement_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/atlas/statement_service_pb2.py` & `eolymp-0.8.2/eolymp/atlas/statement_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/atlas/statement_service_pb2.pyi` & `eolymp-0.8.2/eolymp/atlas/statement_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/atlas/submission_pb2.py` & `eolymp-0.8.2/eolymp/atlas/submission_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/atlas/submission_pb2.pyi` & `eolymp-0.8.2/eolymp/atlas/submission_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/atlas/submission_service_http.py` & `eolymp-0.8.2/eolymp/atlas/submission_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/atlas/submission_service_pb2.py` & `eolymp-0.8.2/eolymp/atlas/submission_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/atlas/submission_service_pb2.pyi` & `eolymp-0.8.2/eolymp/atlas/submission_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/atlas/testing_config_pb2.py` & `eolymp-0.8.2/eolymp/atlas/testing_config_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/atlas/testing_feedback_pb2.py` & `eolymp-0.8.2/eolymp/atlas/testing_feedback_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/atlas/testing_scoring_pb2.py` & `eolymp-0.8.2/eolymp/atlas/testing_scoring_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/atlas/testing_service_http.py` & `eolymp-0.8.2/eolymp/atlas/testing_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/atlas/testing_service_pb2.py` & `eolymp-0.8.2/eolymp/atlas/testing_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/atlas/testing_service_pb2.pyi` & `eolymp-0.8.2/eolymp/atlas/testing_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/atlas/testing_test_pb2.py` & `eolymp-0.8.2/eolymp/atlas/testing_test_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/atlas/testing_test_pb2.pyi` & `eolymp-0.8.2/eolymp/atlas/testing_test_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/atlas/testing_testset_pb2.py` & `eolymp-0.8.2/eolymp/atlas/testing_testset_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/atlas/testing_testset_pb2.pyi` & `eolymp-0.8.2/eolymp/atlas/testing_testset_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/atlas/version_pb2.py` & `eolymp-0.8.2/eolymp/atlas/version_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/atlas/version_pb2.pyi` & `eolymp-0.8.2/eolymp/atlas/version_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/auth/claims_pb2.py` & `eolymp-0.8.2/eolymp/auth/claims_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/auth/claims_pb2.pyi` & `eolymp-0.8.2/eolymp/auth/claims_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/auth/oauth2_service_pb2.py` & `eolymp-0.8.2/eolymp/auth/oauth2_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/auth/oauth2_service_pb2.pyi` & `eolymp-0.8.2/eolymp/auth/oauth2_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/auth/sso_service_pb2.py` & `eolymp-0.8.2/eolymp/auth/sso_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/auth/sso_service_pb2.pyi` & `eolymp-0.8.2/eolymp/auth/sso_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/cognito/access_key_pb2.py` & `eolymp-0.8.2/eolymp/cognito/access_key_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/cognito/access_key_pb2.pyi` & `eolymp-0.8.2/eolymp/cognito/access_key_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/cognito/cognito_http.py` & `eolymp-0.8.2/eolymp/cognito/cognito_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/cognito/cognito_pb2.py` & `eolymp-0.8.2/eolymp/cognito/cognito_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/cognito/cognito_pb2.pyi` & `eolymp-0.8.2/eolymp/cognito/cognito_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/cognito/quota_pb2.py` & `eolymp-0.8.2/eolymp/cognito/quota_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/cognito/user_pb2.py` & `eolymp-0.8.2/eolymp/cognito/user_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/cognito/user_pb2.pyi` & `eolymp-0.8.2/eolymp/cognito/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/community/account_service_http.py` & `eolymp-0.8.2/eolymp/community/account_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/community/account_service_pb2.py` & `eolymp-0.8.2/eolymp/community/account_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/community/account_service_pb2.pyi` & `eolymp-0.8.2/eolymp/community/account_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/community/attribute_pb2.py` & `eolymp-0.8.2/eolymp/community/attribute_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/community/attribute_pb2.pyi` & `eolymp-0.8.2/eolymp/community/attribute_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/community/attribute_service_http.py` & `eolymp-0.8.2/eolymp/community/attribute_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/community/attribute_service_pb2.py` & `eolymp-0.8.2/eolymp/community/attribute_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/community/attribute_service_pb2.pyi` & `eolymp-0.8.2/eolymp/community/attribute_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/community/configuration_idp_pb2.py` & `eolymp-0.8.2/eolymp/community/configuration_idp_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/community/configuration_idp_pb2.pyi` & `eolymp-0.8.2/eolymp/community/configuration_idp_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/community/configuration_service_http.py` & `eolymp-0.8.2/eolymp/community/configuration_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/community/configuration_service_pb2.py` & `eolymp-0.8.2/eolymp/community/configuration_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/community/configuration_service_pb2.pyi` & `eolymp-0.8.2/eolymp/community/configuration_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/community/events_pb2.py` & `eolymp-0.8.2/eolymp/community/events_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/community/events_pb2.pyi` & `eolymp-0.8.2/eolymp/community/events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/community/member_ghost_pb2.py` & `eolymp-0.8.2/eolymp/community/member_ghost_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/community/member_pb2.py` & `eolymp-0.8.2/eolymp/community/member_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/community/member_pb2.pyi` & `eolymp-0.8.2/eolymp/community/member_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/community/member_service_http.py` & `eolymp-0.8.2/eolymp/community/member_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/community/member_service_pb2.py` & `eolymp-0.8.2/eolymp/community/member_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/community/member_service_pb2.pyi` & `eolymp-0.8.2/eolymp/community/member_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/community/member_team_pb2.py` & `eolymp-0.8.2/eolymp/community/member_team_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/community/member_user_pb2.py` & `eolymp-0.8.2/eolymp/community/member_user_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/community/member_user_pb2.pyi` & `eolymp-0.8.2/eolymp/community/member_user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/community/membership_service_http.py` & `eolymp-0.8.2/eolymp/community/membership_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/community/membership_service_pb2.py` & `eolymp-0.8.2/eolymp/community/membership_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/community/membership_service_pb2.pyi` & `eolymp-0.8.2/eolymp/community/membership_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/content/content_service_http.py` & `eolymp-0.8.2/eolymp/content/content_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/content/content_service_pb2.py` & `eolymp-0.8.2/eolymp/content/content_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/content/content_service_pb2.pyi` & `eolymp-0.8.2/eolymp/content/content_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/content/fragment_pb2.py` & `eolymp-0.8.2/eolymp/content/fragment_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/content/fragment_pb2.pyi` & `eolymp-0.8.2/eolymp/content/fragment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/core/http_client.py` & `eolymp-0.8.2/eolymp/core/http_client.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/core/oauth_client.py` & `eolymp-0.8.2/eolymp/core/oauth_client.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/discussion/discussion_pb2.py` & `eolymp-0.8.2/eolymp/discussion/discussion_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/discussion/discussion_pb2.pyi` & `eolymp-0.8.2/eolymp/discussion/discussion_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/discussion/discussion_service_http.py` & `eolymp-0.8.2/eolymp/discussion/discussion_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/discussion/discussion_service_pb2.py` & `eolymp-0.8.2/eolymp/discussion/discussion_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/discussion/discussion_service_pb2.pyi` & `eolymp-0.8.2/eolymp/discussion/discussion_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/discussion/events_pb2.py` & `eolymp-0.8.2/eolymp/discussion/events_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/discussion/events_pb2.pyi` & `eolymp-0.8.2/eolymp/discussion/events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/discussion/forum_pb2.py` & `eolymp-0.8.2/eolymp/discussion/forum_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/discussion/forum_pb2.pyi` & `eolymp-0.8.2/eolymp/discussion/forum_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/discussion/forum_service_http.py` & `eolymp-0.8.2/eolymp/discussion/forum_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/discussion/forum_service_pb2.py` & `eolymp-0.8.2/eolymp/discussion/forum_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/discussion/forum_service_pb2.pyi` & `eolymp-0.8.2/eolymp/discussion/forum_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/discussion/message_pb2.py` & `eolymp-0.8.2/eolymp/discussion/message_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/discussion/message_pb2.pyi` & `eolymp-0.8.2/eolymp/discussion/message_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/discussion/message_service_http.py` & `eolymp-0.8.2/eolymp/discussion/message_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/discussion/message_service_pb2.py` & `eolymp-0.8.2/eolymp/discussion/message_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/discussion/message_service_pb2.pyi` & `eolymp-0.8.2/eolymp/discussion/message_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/discussion/subscription_pb2.py` & `eolymp-0.8.2/eolymp/discussion/subscription_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/discussion/subscription_pb2.pyi` & `eolymp-0.8.2/eolymp/discussion/subscription_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/discussion/subscription_service_http.py` & `eolymp-0.8.2/eolymp/discussion/subscription_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/discussion/subscription_service_pb2.py` & `eolymp-0.8.2/eolymp/discussion/subscription_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/discussion/subscription_service_pb2.pyi` & `eolymp-0.8.2/eolymp/discussion/subscription_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/ecm/content_pb2.py` & `eolymp-0.8.2/eolymp/ecm/content_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/ecm/content_pb2.pyi` & `eolymp-0.8.2/eolymp/ecm/content_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/ecm/node_pb2.py` & `eolymp-0.8.2/eolymp/ecm/node_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/ecm/node_pb2.pyi` & `eolymp-0.8.2/eolymp/ecm/node_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/executor/events_pb2.py` & `eolymp-0.8.2/eolymp/executor/events_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/executor/events_pb2.pyi` & `eolymp-0.8.2/eolymp/executor/events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/executor/executor_http.py` & `eolymp-0.8.2/eolymp/executor/executor_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/executor/executor_pb2.py` & `eolymp-0.8.2/eolymp/executor/executor_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/executor/executor_pb2.pyi` & `eolymp-0.8.2/eolymp/executor/executor_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/executor/interactor_pb2.py` & `eolymp-0.8.2/eolymp/executor/interactor_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/executor/interactor_pb2.pyi` & `eolymp-0.8.2/eolymp/executor/interactor_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/executor/job_pb2.py` & `eolymp-0.8.2/eolymp/executor/job_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/executor/job_pb2.pyi` & `eolymp-0.8.2/eolymp/executor/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/executor/language_pb2.py` & `eolymp-0.8.2/eolymp/executor/language_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/executor/language_pb2.pyi` & `eolymp-0.8.2/eolymp/executor/language_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/executor/report_pb2.py` & `eolymp-0.8.2/eolymp/executor/report_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/executor/report_pb2.pyi` & `eolymp-0.8.2/eolymp/executor/report_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/executor/runtime_pb2.py` & `eolymp-0.8.2/eolymp/executor/runtime_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/executor/runtime_pb2.pyi` & `eolymp-0.8.2/eolymp/executor/runtime_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/executor/status_pb2.py` & `eolymp-0.8.2/eolymp/executor/status_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/executor/status_pb2.pyi` & `eolymp-0.8.2/eolymp/executor/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/executor/task_pb2.py` & `eolymp-0.8.2/eolymp/executor/task_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/executor/task_pb2.pyi` & `eolymp-0.8.2/eolymp/executor/task_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/executor/usage_pb2.py` & `eolymp-0.8.2/eolymp/executor/usage_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/executor/usage_pb2.pyi` & `eolymp-0.8.2/eolymp/executor/usage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/executor/verifier_pb2.py` & `eolymp-0.8.2/eolymp/executor/verifier_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/executor/verifier_pb2.pyi` & `eolymp-0.8.2/eolymp/executor/verifier_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/geography/country_pb2.py` & `eolymp-0.8.2/eolymp/geography/country_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/geography/country_pb2.pyi` & `eolymp-0.8.2/eolymp/geography/country_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/geography/geography_http.py` & `eolymp-0.8.2/eolymp/geography/geography_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/geography/geography_pb2.py` & `eolymp-0.8.2/eolymp/geography/geography_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/geography/geography_pb2.pyi` & `eolymp-0.8.2/eolymp/geography/geography_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/geography/region_pb2.py` & `eolymp-0.8.2/eolymp/geography/region_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/geography/region_pb2.pyi` & `eolymp-0.8.2/eolymp/geography/region_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/harmony/agreement_pb2.py` & `eolymp-0.8.2/eolymp/harmony/agreement_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/harmony/agreement_pb2.pyi` & `eolymp-0.8.2/eolymp/harmony/agreement_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/harmony/consent_pb2.py` & `eolymp-0.8.2/eolymp/harmony/consent_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/harmony/consent_pb2.pyi` & `eolymp-0.8.2/eolymp/harmony/consent_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/harmony/harmony_http.py` & `eolymp-0.8.2/eolymp/harmony/harmony_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/harmony/harmony_pb2.py` & `eolymp-0.8.2/eolymp/harmony/harmony_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/harmony/harmony_pb2.pyi` & `eolymp-0.8.2/eolymp/harmony/harmony_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/helpdesk/auto_reply_pb2.py` & `eolymp-0.8.2/eolymp/helpdesk/auto_reply_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/helpdesk/auto_reply_pb2.pyi` & `eolymp-0.8.2/eolymp/helpdesk/auto_reply_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/helpdesk/document_pb2.py` & `eolymp-0.8.2/eolymp/helpdesk/document_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/helpdesk/document_pb2.pyi` & `eolymp-0.8.2/eolymp/helpdesk/document_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/helpdesk/events_pb2.py` & `eolymp-0.8.2/eolymp/helpdesk/events_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/helpdesk/events_pb2.pyi` & `eolymp-0.8.2/eolymp/helpdesk/events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/helpdesk/helpdesk_http.py` & `eolymp-0.8.2/eolymp/helpdesk/helpdesk_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/helpdesk/helpdesk_pb2.py` & `eolymp-0.8.2/eolymp/helpdesk/helpdesk_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/helpdesk/helpdesk_pb2.pyi` & `eolymp-0.8.2/eolymp/helpdesk/helpdesk_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/helpdesk/support_http.py` & `eolymp-0.8.2/eolymp/helpdesk/support_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/helpdesk/support_pb2.py` & `eolymp-0.8.2/eolymp/helpdesk/support_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/helpdesk/support_pb2.pyi` & `eolymp-0.8.2/eolymp/helpdesk/support_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/helpdesk/ticket_pb2.py` & `eolymp-0.8.2/eolymp/helpdesk/ticket_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/helpdesk/ticket_pb2.pyi` & `eolymp-0.8.2/eolymp/helpdesk/ticket_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/judge/acl_http.py` & `eolymp-0.8.2/eolymp/judge/acl_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/judge/acl_pb2.py` & `eolymp-0.8.2/eolymp/judge/acl_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/judge/acl_pb2.pyi` & `eolymp-0.8.2/eolymp/judge/acl_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/judge/activity_pb2.py` & `eolymp-0.8.2/eolymp/judge/activity_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/judge/activity_pb2.pyi` & `eolymp-0.8.2/eolymp/judge/activity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/judge/announcement_pb2.py` & `eolymp-0.8.2/eolymp/judge/announcement_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/judge/announcement_pb2.pyi` & `eolymp-0.8.2/eolymp/judge/announcement_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/judge/contest_pb2.py` & `eolymp-0.8.2/eolymp/judge/contest_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/judge/contest_pb2.pyi` & `eolymp-0.8.2/eolymp/judge/contest_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/judge/events_pb2.py` & `eolymp-0.8.2/eolymp/judge/events_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/judge/events_pb2.pyi` & `eolymp-0.8.2/eolymp/judge/events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/judge/judge_http.py` & `eolymp-0.8.2/eolymp/judge/judge_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/judge/judge_pb2.py` & `eolymp-0.8.2/eolymp/judge/judge_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/judge/judge_pb2.pyi` & `eolymp-0.8.2/eolymp/judge/judge_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/judge/participant_pb2.py` & `eolymp-0.8.2/eolymp/judge/participant_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/judge/participant_pb2.pyi` & `eolymp-0.8.2/eolymp/judge/participant_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/judge/problem_pb2.py` & `eolymp-0.8.2/eolymp/judge/problem_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/judge/problem_pb2.pyi` & `eolymp-0.8.2/eolymp/judge/problem_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/judge/reply_pb2.py` & `eolymp-0.8.2/eolymp/judge/reply_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/judge/reply_pb2.pyi` & `eolymp-0.8.2/eolymp/judge/reply_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/judge/result_pb2.py` & `eolymp-0.8.2/eolymp/judge/result_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/judge/result_pb2.pyi` & `eolymp-0.8.2/eolymp/judge/result_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/judge/score_pb2.py` & `eolymp-0.8.2/eolymp/judge/score_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/judge/score_pb2.pyi` & `eolymp-0.8.2/eolymp/judge/score_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/judge/submission_pb2.py` & `eolymp-0.8.2/eolymp/judge/submission_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/judge/submission_pb2.pyi` & `eolymp-0.8.2/eolymp/judge/submission_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/judge/template_pb2.py` & `eolymp-0.8.2/eolymp/judge/template_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/judge/template_pb2.pyi` & `eolymp-0.8.2/eolymp/judge/template_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/judge/ticket_pb2.py` & `eolymp-0.8.2/eolymp/judge/ticket_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/judge/ticket_pb2.pyi` & `eolymp-0.8.2/eolymp/judge/ticket_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/keeper/blob_pb2.py` & `eolymp-0.8.2/eolymp/keeper/blob_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/keeper/blob_pb2.pyi` & `eolymp-0.8.2/eolymp/keeper/blob_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/keeper/keeper_http.py` & `eolymp-0.8.2/eolymp/keeper/keeper_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/keeper/keeper_pb2.py` & `eolymp-0.8.2/eolymp/keeper/keeper_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/keeper/keeper_pb2.pyi` & `eolymp-0.8.2/eolymp/keeper/keeper_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/l10n/localization_service_http.py` & `eolymp-0.8.2/eolymp/l10n/localization_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/l10n/localization_service_pb2.py` & `eolymp-0.8.2/eolymp/l10n/localization_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/l10n/localization_service_pb2.pyi` & `eolymp-0.8.2/eolymp/l10n/localization_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/l10n/project_pb2.py` & `eolymp-0.8.2/eolymp/l10n/project_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/l10n/project_pb2.pyi` & `eolymp-0.8.2/eolymp/l10n/project_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/l10n/project_service_http.py` & `eolymp-0.8.2/eolymp/l10n/project_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/l10n/project_service_pb2.py` & `eolymp-0.8.2/eolymp/l10n/project_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/l10n/project_service_pb2.pyi` & `eolymp-0.8.2/eolymp/l10n/project_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/l10n/term_pb2.py` & `eolymp-0.8.2/eolymp/l10n/term_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/l10n/term_pb2.pyi` & `eolymp-0.8.2/eolymp/l10n/term_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/l10n/translation_pb2.py` & `eolymp-0.8.2/eolymp/l10n/translation_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/l10n/translation_pb2.pyi` & `eolymp-0.8.2/eolymp/l10n/translation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/oauth2/oauth2_pb2.py` & `eolymp-0.8.2/eolymp/oauth2/oauth2_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/oauth2/oauth2_pb2.pyi` & `eolymp-0.8.2/eolymp/oauth2/oauth2_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/playground/playground_http.py` & `eolymp-0.8.2/eolymp/playground/playground_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/playground/playground_pb2.py` & `eolymp-0.8.2/eolymp/playground/playground_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/playground/playground_pb2.pyi` & `eolymp-0.8.2/eolymp/playground/playground_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/playground/run_pb2.py` & `eolymp-0.8.2/eolymp/playground/run_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/playground/run_pb2.pyi` & `eolymp-0.8.2/eolymp/playground/run_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/ranker/activity_pb2.py` & `eolymp-0.8.2/eolymp/ranker/activity_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/ranker/activity_pb2.pyi` & `eolymp-0.8.2/eolymp/ranker/activity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/ranker/events_pb2.py` & `eolymp-0.8.2/eolymp/ranker/events_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/ranker/events_pb2.pyi` & `eolymp-0.8.2/eolymp/ranker/events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/ranker/format_pb2.py` & `eolymp-0.8.2/eolymp/ranker/format_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/ranker/ranker_http.py` & `eolymp-0.8.2/eolymp/ranker/ranker_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/ranker/ranker_pb2.py` & `eolymp-0.8.2/eolymp/ranker/ranker_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/ranker/ranker_pb2.pyi` & `eolymp-0.8.2/eolymp/ranker/ranker_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/ranker/scoreboard_pb2.py` & `eolymp-0.8.2/eolymp/ranker/scoreboard_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/ranker/scoreboard_pb2.pyi` & `eolymp-0.8.2/eolymp/ranker/scoreboard_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/resolver/resolver_http.py` & `eolymp-0.8.2/eolymp/resolver/resolver_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/resolver/resolver_pb2.py` & `eolymp-0.8.2/eolymp/resolver/resolver_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/resolver/resolver_pb2.pyi` & `eolymp-0.8.2/eolymp/resolver/resolver_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/taxonomy/link_service_http.py` & `eolymp-0.8.2/eolymp/taxonomy/link_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/taxonomy/link_service_pb2.py` & `eolymp-0.8.2/eolymp/taxonomy/link_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/taxonomy/link_service_pb2.pyi` & `eolymp-0.8.2/eolymp/taxonomy/link_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/taxonomy/topic_pb2.py` & `eolymp-0.8.2/eolymp/taxonomy/topic_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/taxonomy/topic_pb2.pyi` & `eolymp-0.8.2/eolymp/taxonomy/topic_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/taxonomy/topic_service_http.py` & `eolymp-0.8.2/eolymp/taxonomy/topic_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/taxonomy/topic_service_pb2.py` & `eolymp-0.8.2/eolymp/taxonomy/topic_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/taxonomy/topic_service_pb2.pyi` & `eolymp-0.8.2/eolymp/taxonomy/topic_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/typewriter/block_pb2.py` & `eolymp-0.8.2/eolymp/typewriter/block_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/typewriter/block_pb2.pyi` & `eolymp-0.8.2/eolymp/typewriter/block_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/typewriter/events_pb2.py` & `eolymp-0.8.2/eolymp/typewriter/events_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/typewriter/events_pb2.pyi` & `eolymp-0.8.2/eolymp/typewriter/events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/typewriter/fragment_pb2.py` & `eolymp-0.8.2/eolymp/typewriter/fragment_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/typewriter/fragment_pb2.pyi` & `eolymp-0.8.2/eolymp/typewriter/fragment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/typewriter/inline_pb2.py` & `eolymp-0.8.2/eolymp/typewriter/inline_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/typewriter/inline_pb2.pyi` & `eolymp-0.8.2/eolymp/typewriter/inline_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/typewriter/typewriter_http.py` & `eolymp-0.8.2/eolymp/typewriter/typewriter_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/typewriter/typewriter_pb2.py` & `eolymp-0.8.2/eolymp/typewriter/typewriter_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/typewriter/typewriter_pb2.pyi` & `eolymp-0.8.2/eolymp/typewriter/typewriter_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/universe/permission_pb2.py` & `eolymp-0.8.2/eolymp/universe/permission_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/universe/permission_pb2.pyi` & `eolymp-0.8.2/eolymp/universe/permission_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/universe/space_pb2.py` & `eolymp-0.8.2/eolymp/universe/space_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/universe/space_pb2.pyi` & `eolymp-0.8.2/eolymp/universe/space_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/universe/universe_http.py` & `eolymp-0.8.2/eolymp/universe/universe_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/universe/universe_pb2.py` & `eolymp-0.8.2/eolymp/universe/universe_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/universe/universe_pb2.pyi` & `eolymp-0.8.2/eolymp/universe/universe_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/wellknown/direction_pb2.py` & `eolymp-0.8.2/eolymp/wellknown/direction_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/wellknown/errors_pb2.py` & `eolymp-0.8.2/eolymp/wellknown/errors_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/wellknown/errors_pb2.pyi` & `eolymp-0.8.2/eolymp/wellknown/errors_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/wellknown/expression_pb2.py` & `eolymp-0.8.2/eolymp/wellknown/expression_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/wellknown/expression_pb2.pyi` & `eolymp-0.8.2/eolymp/wellknown/expression_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/worker/events_pb2.py` & `eolymp-0.8.2/eolymp/worker/events_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/worker/job_pb2.py` & `eolymp-0.8.2/eolymp/worker/job_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/worker/job_pb2.pyi` & `eolymp-0.8.2/eolymp/worker/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/worker/worker_service_pb2.py` & `eolymp-0.8.2/eolymp/worker/worker_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp/worker/worker_service_pb2.pyi` & `eolymp-0.8.2/eolymp/worker/worker_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/eolymp.egg-info/PKG-INFO` & `eolymp-0.8.2/eolymp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eolymp
-Version: 0.8.1
+Version: 0.8.2
 Summary: Eolymp SDK for Python
 Home-page: https://github.com/eolymp/contracts
 Author: Sergey Kolodyazhnyy
 Author-email: sergey@eolymp.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `eolymp-0.8.1/eolymp.egg-info/SOURCES.txt` & `eolymp-0.8.2/eolymp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.1/setup.py` & `eolymp-0.8.2/setup.py`

 * *Files identical despite different names*

