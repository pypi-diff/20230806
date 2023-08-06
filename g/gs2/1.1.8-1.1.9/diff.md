# Comparing `tmp/gs2-1.1.8.tar.gz` & `tmp/gs2-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gs2-1.1.8.tar", last modified: Wed Sep 21 12:41:34 2022, max compression
+gzip compressed data, was "gs2-1.1.9.tar", last modified: Wed Sep 28 06:10:27 2022, max compression
```

## Comparing `gs2-1.1.8.tar` & `gs2-1.1.9.tar`

### file list

```diff
@@ -1,275 +1,275 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-21 12:41:34.192271 gs2-1.1.8/
--rw-r--r--   0 root         (0) root         (0)      364 2022-09-21 12:41:34.192271 gs2-1.1.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2022-09-21 12:41:34.192271 gs2-1.1.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1384 2022-09-21 12:29:59.000000 gs2-1.1.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-21 12:41:34.144271 gs2-1.1.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-21 12:41:34.148271 gs2-1.1.8/src/gs2/
--rw-r--r--   0 root         (0) root         (0)      792 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-21 12:41:34.148271 gs2-1.1.8/src/gs2/account/
--rw-r--r--   0 root         (0) root         (0)      696 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/account/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21039 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/account/model.py
--rw-r--r--   0 root         (0) root         (0)    44584 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/account/request.py
--rw-r--r--   0 root         (0) root         (0)    61603 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/account/rest.py
--rw-r--r--   0 root         (0) root         (0)    26232 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/account/result.py
--rw-r--r--   0 root         (0) root         (0)    59296 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/account/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-21 12:41:34.152271 gs2-1.1.8/src/gs2/auth/
--rw-r--r--   0 root         (0) root         (0)      696 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2133 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/auth/model.py
--rw-r--r--   0 root         (0) root         (0)     3054 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/auth/request.py
--rw-r--r--   0 root         (0) root         (0)     4777 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/auth/rest.py
--rw-r--r--   0 root         (0) root         (0)     3127 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/auth/result.py
--rw-r--r--   0 root         (0) root         (0)     4771 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/auth/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-21 12:41:34.152271 gs2-1.1.8/src/gs2/chat/
--rw-r--r--   0 root         (0) root         (0)      696 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/chat/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25666 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/chat/model.py
--rw-r--r--   0 root         (0) root         (0)    63678 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/chat/request.py
--rw-r--r--   0 root         (0) root         (0)    78812 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/chat/rest.py
--rw-r--r--   0 root         (0) root         (0)    32032 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/chat/result.py
--rw-r--r--   0 root         (0) root         (0)    75904 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/chat/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-21 12:41:34.152271 gs2-1.1.8/src/gs2/core/
--rw-r--r--   0 root         (0) root         (0)      188 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-21 12:41:34.152271 gs2-1.1.8/src/gs2/core/domain/
--rw-r--r--   0 root         (0) root         (0)    10812 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/core/domain/__init__.py
--rw-r--r--   0 root         (0) root         (0)      274 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/core/domain/access_token.py
--rw-r--r--   0 root         (0) root         (0)     3658 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/core/exception.py
--rw-r--r--   0 root         (0) root         (0)     6581 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/core/model.py
--rw-r--r--   0 root         (0) root         (0)    10580 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/core/rest.py
--rw-r--r--   0 root         (0) root         (0)     1233 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/core/util.py
--rw-r--r--   0 root         (0) root         (0)    10955 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/core/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-21 12:41:34.156271 gs2-1.1.8/src/gs2/datastore/
--rw-r--r--   0 root         (0) root         (0)      696 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/datastore/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17622 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/datastore/model.py
--rw-r--r--   0 root         (0) root         (0)    57176 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/datastore/request.py
--rw-r--r--   0 root         (0) root         (0)    77053 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/datastore/rest.py
--rw-r--r--   0 root         (0) root         (0)    37260 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/datastore/result.py
--rw-r--r--   0 root         (0) root         (0)    74625 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/datastore/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-21 12:41:34.156271 gs2-1.1.8/src/gs2/deploy/
--rw-r--r--   0 root         (0) root         (0)      696 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/deploy/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19443 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/deploy/model.py
--rw-r--r--   0 root         (0) root         (0)    21473 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/deploy/request.py
--rw-r--r--   0 root         (0) root         (0)    38731 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/deploy/rest.py
--rw-r--r--   0 root         (0) root         (0)    18118 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/deploy/result.py
--rw-r--r--   0 root         (0) root         (0)    37185 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/deploy/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-21 12:41:34.156271 gs2-1.1.8/src/gs2/dictionary/
--rw-r--r--   0 root         (0) root         (0)      696 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/dictionary/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23778 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/dictionary/model.py
--rw-r--r--   0 root         (0) root         (0)    37763 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/dictionary/request.py
--rw-r--r--   0 root         (0) root         (0)    60038 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/dictionary/rest.py
--rw-r--r--   0 root         (0) root         (0)    27656 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/dictionary/result.py
--rw-r--r--   0 root         (0) root         (0)    57798 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/dictionary/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-21 12:41:34.156271 gs2-1.1.8/src/gs2/distributor/
--rw-r--r--   0 root         (0) root         (0)      696 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/distributor/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30294 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/distributor/model.py
--rw-r--r--   0 root         (0) root         (0)    40153 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/distributor/request.py
--rw-r--r--   0 root         (0) root         (0)    63369 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/distributor/rest.py
--rw-r--r--   0 root         (0) root         (0)    29638 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/distributor/result.py
--rw-r--r--   0 root         (0) root         (0)    61505 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/distributor/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-21 12:41:34.160271 gs2-1.1.8/src/gs2/enhance/
--rw-r--r--   0 root         (0) root         (0)      696 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/enhance/__init__.py
--rw-r--r--   0 root         (0) root         (0)    36059 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/enhance/model.py
--rw-r--r--   0 root         (0) root         (0)    62716 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/enhance/request.py
--rw-r--r--   0 root         (0) root         (0)    78687 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/enhance/rest.py
--rw-r--r--   0 root         (0) root         (0)    43712 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/enhance/result.py
--rw-r--r--   0 root         (0) root         (0)    75846 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/enhance/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-21 12:41:34.160271 gs2-1.1.8/src/gs2/exchange/
--rw-r--r--   0 root         (0) root         (0)      696 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/exchange/__init__.py
--rw-r--r--   0 root         (0) root         (0)    34652 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/exchange/model.py
--rw-r--r--   0 root         (0) root         (0)    63736 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/exchange/request.py
--rw-r--r--   0 root         (0) root         (0)    82386 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/exchange/rest.py
--rw-r--r--   0 root         (0) root         (0)    44513 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/exchange/result.py
--rw-r--r--   0 root         (0) root         (0)    79193 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/exchange/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-21 12:41:34.160271 gs2-1.1.8/src/gs2/experience/
--rw-r--r--   0 root         (0) root         (0)      696 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/experience/__init__.py
--rw-r--r--   0 root         (0) root         (0)    34902 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/experience/model.py
--rw-r--r--   0 root         (0) root         (0)    63688 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/experience/request.py
--rw-r--r--   0 root         (0) root         (0)    88409 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/experience/rest.py
--rw-r--r--   0 root         (0) root         (0)    37534 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/experience/result.py
--rw-r--r--   0 root         (0) root         (0)    84658 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/experience/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-21 12:41:34.164271 gs2-1.1.8/src/gs2/formation/
--rw-r--r--   0 root         (0) root         (0)      696 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/formation/__init__.py
--rw-r--r--   0 root         (0) root         (0)    52495 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/formation/model.py
--rw-r--r--   0 root         (0) root         (0)   100988 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/formation/request.py
--rw-r--r--   0 root         (0) root         (0)   141633 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/formation/rest.py
--rw-r--r--   0 root         (0) root         (0)    78524 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/formation/result.py
--rw-r--r--   0 root         (0) root         (0)   135549 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/formation/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-21 12:41:34.164271 gs2-1.1.8/src/gs2/friend/
--rw-r--r--   0 root         (0) root         (0)      696 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/friend/__init__.py
--rw-r--r--   0 root         (0) root         (0)    43298 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/friend/model.py
--rw-r--r--   0 root         (0) root         (0)    86971 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/friend/request.py
--rw-r--r--   0 root         (0) root         (0)   116120 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/friend/rest.py
--rw-r--r--   0 root         (0) root         (0)    49523 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/friend/result.py
--rw-r--r--   0 root         (0) root         (0)   111985 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/friend/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-21 12:41:34.164271 gs2-1.1.8/src/gs2/gateway/
--rw-r--r--   0 root         (0) root         (0)      696 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/gateway/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13068 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/gateway/model.py
--rw-r--r--   0 root         (0) root         (0)    30343 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/gateway/request.py
--rw-r--r--   0 root         (0) root         (0)    46374 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/gateway/rest.py
--rw-r--r--   0 root         (0) root         (0)    20062 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/gateway/result.py
--rw-r--r--   0 root         (0) root         (0)    45043 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/gateway/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-21 12:41:34.168271 gs2-1.1.8/src/gs2/identifier/
--rw-r--r--   0 root         (0) root         (0)      696 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/identifier/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13178 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/identifier/model.py
--rw-r--r--   0 root         (0) root         (0)    27417 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/identifier/request.py
--rw-r--r--   0 root         (0) root         (0)    51631 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/identifier/rest.py
--rw-r--r--   0 root         (0) root         (0)    26226 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/identifier/result.py
--rw-r--r--   0 root         (0) root         (0)    49813 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/identifier/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-21 12:41:34.168271 gs2-1.1.8/src/gs2/inbox/
--rw-r--r--   0 root         (0) root         (0)      696 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/inbox/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39659 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/inbox/model.py
--rw-r--r--   0 root         (0) root         (0)    60409 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/inbox/request.py
--rw-r--r--   0 root         (0) root         (0)    83314 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/inbox/rest.py
--rw-r--r--   0 root         (0) root         (0)    38119 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/inbox/result.py
--rw-r--r--   0 root         (0) root         (0)    80466 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/inbox/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-21 12:41:34.168271 gs2-1.1.8/src/gs2/inventory/
--rw-r--r--   0 root         (0) root         (0)      696 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/inventory/__init__.py
--rw-r--r--   0 root         (0) root         (0)    47883 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/inventory/model.py
--rw-r--r--   0 root         (0) root         (0)   106987 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/inventory/request.py
--rw-r--r--   0 root         (0) root         (0)   145526 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/inventory/rest.py
--rw-r--r--   0 root         (0) root         (0)    83791 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/inventory/result.py
--rw-r--r--   0 root         (0) root         (0)   138438 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/inventory/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-21 12:41:34.172271 gs2-1.1.8/src/gs2/job_queue/
--rw-r--r--   0 root         (0) root         (0)      696 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/job_queue/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25092 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/job_queue/model.py
--rw-r--r--   0 root         (0) root         (0)    28055 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/job_queue/request.py
--rw-r--r--   0 root         (0) root         (0)    41824 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/job_queue/rest.py
--rw-r--r--   0 root         (0) root         (0)    20203 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/job_queue/result.py
--rw-r--r--   0 root         (0) root         (0)    40098 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/job_queue/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-21 12:41:34.172271 gs2-1.1.8/src/gs2/key/
--rw-r--r--   0 root         (0) root         (0)      696 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/key/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11874 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/key/model.py
--rw-r--r--   0 root         (0) root         (0)    24617 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/key/request.py
--rw-r--r--   0 root         (0) root         (0)    40001 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/key/rest.py
--rw-r--r--   0 root         (0) root         (0)    17815 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/key/result.py
--rw-r--r--   0 root         (0) root         (0)    38327 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/key/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-21 12:41:34.172271 gs2-1.1.8/src/gs2/limit/
--rw-r--r--   0 root         (0) root         (0)      696 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/limit/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23601 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/limit/model.py
--rw-r--r--   0 root         (0) root         (0)    40251 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/limit/request.py
--rw-r--r--   0 root         (0) root         (0)    60806 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/limit/rest.py
--rw-r--r--   0 root         (0) root         (0)    26781 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/limit/result.py
--rw-r--r--   0 root         (0) root         (0)    58511 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/limit/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-21 12:41:34.172271 gs2-1.1.8/src/gs2/lock/
--rw-r--r--   0 root         (0) root         (0)      696 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/lock/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8758 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/lock/model.py
--rw-r--r--   0 root         (0) root         (0)    23181 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/lock/request.py
--rw-r--r--   0 root         (0) root         (0)    34491 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/lock/rest.py
--rw-r--r--   0 root         (0) root         (0)    15295 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/lock/result.py
--rw-r--r--   0 root         (0) root         (0)    33213 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/lock/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-21 12:41:34.176271 gs2-1.1.8/src/gs2/log/
--rw-r--r--   0 root         (0) root         (0)      696 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/log/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25728 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/log/model.py
--rw-r--r--   0 root         (0) root         (0)    41864 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/log/request.py
--rw-r--r--   0 root         (0) root         (0)    49307 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/log/rest.py
--rw-r--r--   0 root         (0) root         (0)    27100 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/log/result.py
--rw-r--r--   0 root         (0) root         (0)    47078 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/log/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-21 12:41:34.176271 gs2-1.1.8/src/gs2/lottery/
--rw-r--r--   0 root         (0) root         (0)      696 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/lottery/__init__.py
--rw-r--r--   0 root         (0) root         (0)    49829 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/lottery/model.py
--rw-r--r--   0 root         (0) root         (0)    59242 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/lottery/request.py
--rw-r--r--   0 root         (0) root         (0)    87536 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/lottery/rest.py
--rw-r--r--   0 root         (0) root         (0)    40742 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/lottery/result.py
--rw-r--r--   0 root         (0) root         (0)    83914 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/lottery/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-21 12:41:34.176271 gs2-1.1.8/src/gs2/matchmaking/
--rw-r--r--   0 root         (0) root         (0)      696 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/matchmaking/__init__.py
--rw-r--r--   0 root         (0) root         (0)    50049 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/matchmaking/model.py
--rw-r--r--   0 root         (0) root         (0)    77767 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/matchmaking/request.py
--rw-r--r--   0 root         (0) root         (0)    98096 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/matchmaking/rest.py
--rw-r--r--   0 root         (0) root         (0)    41546 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/matchmaking/result.py
--rw-r--r--   0 root         (0) root         (0)    94510 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/matchmaking/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-21 12:41:34.180271 gs2-1.1.8/src/gs2/mega_field/
--rw-r--r--   0 root         (0) root         (0)      696 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/mega_field/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39586 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/mega_field/model.py
--rw-r--r--   0 root         (0) root         (0)    53867 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/mega_field/request.py
--rw-r--r--   0 root         (0) root         (0)    76865 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/mega_field/rest.py
--rw-r--r--   0 root         (0) root         (0)    32973 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/mega_field/result.py
--rw-r--r--   0 root         (0) root         (0)    73270 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/mega_field/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-21 12:41:34.180271 gs2-1.1.8/src/gs2/mission/
--rw-r--r--   0 root         (0) root         (0)      696 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/mission/__init__.py
--rw-r--r--   0 root         (0) root         (0)    64956 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/mission/model.py
--rw-r--r--   0 root         (0) root         (0)    86838 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/mission/request.py
--rw-r--r--   0 root         (0) root         (0)   116464 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/mission/rest.py
--rw-r--r--   0 root         (0) root         (0)    51500 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/mission/result.py
--rw-r--r--   0 root         (0) root         (0)   111559 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/mission/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-21 12:41:34.180271 gs2-1.1.8/src/gs2/money/
--rw-r--r--   0 root         (0) root         (0)      696 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/money/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20794 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/money/model.py
--rw-r--r--   0 root         (0) root         (0)    33783 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/money/request.py
--rw-r--r--   0 root         (0) root         (0)    45386 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/money/rest.py
--rw-r--r--   0 root         (0) root         (0)    20827 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/money/result.py
--rw-r--r--   0 root         (0) root         (0)    43924 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/money/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-21 12:41:34.180271 gs2-1.1.8/src/gs2/news/
--rw-r--r--   0 root         (0) root         (0)      696 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/news/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10517 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/news/model.py
--rw-r--r--   0 root         (0) root         (0)    16136 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/news/request.py
--rw-r--r--   0 root         (0) root         (0)    28973 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/news/rest.py
--rw-r--r--   0 root         (0) root         (0)    15986 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/news/result.py
--rw-r--r--   0 root         (0) root         (0)    28179 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/news/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-21 12:41:34.184271 gs2-1.1.8/src/gs2/quest/
--rw-r--r--   0 root         (0) root         (0)      696 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/quest/__init__.py
--rw-r--r--   0 root         (0) root         (0)    55308 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/quest/model.py
--rw-r--r--   0 root         (0) root         (0)    77678 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/quest/request.py
--rw-r--r--   0 root         (0) root         (0)   101117 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/quest/rest.py
--rw-r--r--   0 root         (0) root         (0)    48230 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/quest/result.py
--rw-r--r--   0 root         (0) root         (0)    97317 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/quest/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-21 12:41:34.184271 gs2-1.1.8/src/gs2/ranking/
--rw-r--r--   0 root         (0) root         (0)      696 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/ranking/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39347 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/ranking/model.py
--rw-r--r--   0 root         (0) root         (0)    67281 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/ranking/request.py
--rw-r--r--   0 root         (0) root         (0)    91769 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/ranking/rest.py
--rw-r--r--   0 root         (0) root         (0)    38368 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/ranking/result.py
--rw-r--r--   0 root         (0) root         (0)    87350 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/ranking/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-21 12:41:34.184271 gs2-1.1.8/src/gs2/realtime/
--rw-r--r--   0 root         (0) root         (0)      696 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/realtime/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11834 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/realtime/model.py
--rw-r--r--   0 root         (0) root         (0)    14978 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/realtime/request.py
--rw-r--r--   0 root         (0) root         (0)    22667 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/realtime/rest.py
--rw-r--r--   0 root         (0) root         (0)    10364 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/realtime/result.py
--rw-r--r--   0 root         (0) root         (0)    21848 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/realtime/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-21 12:41:34.188271 gs2-1.1.8/src/gs2/schedule/
--rw-r--r--   0 root         (0) root         (0)      696 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/schedule/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27411 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/schedule/model.py
--rw-r--r--   0 root         (0) root         (0)    46255 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/schedule/request.py
--rw-r--r--   0 root         (0) root         (0)    66261 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/schedule/rest.py
--rw-r--r--   0 root         (0) root         (0)    28460 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/schedule/result.py
--rw-r--r--   0 root         (0) root         (0)    63762 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/schedule/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-21 12:41:34.188271 gs2-1.1.8/src/gs2/script/
--rw-r--r--   0 root         (0) root         (0)      696 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/script/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10923 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/script/model.py
--rw-r--r--   0 root         (0) root         (0)    20581 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/script/request.py
--rw-r--r--   0 root         (0) root         (0)    33346 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/script/rest.py
--rw-r--r--   0 root         (0) root         (0)    17019 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/script/result.py
--rw-r--r--   0 root         (0) root         (0)    32201 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/script/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-21 12:41:34.188271 gs2-1.1.8/src/gs2/serial_key/
--rw-r--r--   0 root         (0) root         (0)      696 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/serial_key/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26449 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/serial_key/model.py
--rw-r--r--   0 root         (0) root         (0)    36692 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/serial_key/request.py
--rw-r--r--   0 root         (0) root         (0)    59697 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/serial_key/rest.py
--rw-r--r--   0 root         (0) root         (0)    28304 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/serial_key/result.py
--rw-r--r--   0 root         (0) root         (0)    57135 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/serial_key/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-21 12:41:34.188271 gs2-1.1.8/src/gs2/showcase/
--rw-r--r--   0 root         (0) root         (0)      696 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/showcase/__init__.py
--rw-r--r--   0 root         (0) root         (0)    44174 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/showcase/model.py
--rw-r--r--   0 root         (0) root         (0)    53664 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/showcase/request.py
--rw-r--r--   0 root         (0) root         (0)    74863 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/showcase/rest.py
--rw-r--r--   0 root         (0) root         (0)    34249 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/showcase/result.py
--rw-r--r--   0 root         (0) root         (0)    72013 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/showcase/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-21 12:41:34.192271 gs2-1.1.8/src/gs2/stamina/
--rw-r--r--   0 root         (0) root         (0)      696 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/stamina/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56778 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/stamina/model.py
--rw-r--r--   0 root         (0) root         (0)    96095 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/stamina/request.py
--rw-r--r--   0 root         (0) root         (0)   133258 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/stamina/rest.py
--rw-r--r--   0 root         (0) root         (0)    62943 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/stamina/result.py
--rw-r--r--   0 root         (0) root         (0)   128508 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/stamina/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-21 12:41:34.192271 gs2-1.1.8/src/gs2/version/
--rw-r--r--   0 root         (0) root         (0)      696 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/version/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33415 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/version/model.py
--rw-r--r--   0 root         (0) root         (0)    46417 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/version/request.py
--rw-r--r--   0 root         (0) root         (0)    66565 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/version/rest.py
--rw-r--r--   0 root         (0) root         (0)    31007 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/version/result.py
--rw-r--r--   0 root         (0) root         (0)    64446 2022-09-21 12:29:59.000000 gs2-1.1.8/src/gs2/version/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-21 12:41:34.148271 gs2-1.1.8/src/gs2.egg-info/
--rw-r--r--   0 root         (0) root         (0)      364 2022-09-21 12:41:34.000000 gs2-1.1.8/src/gs2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6176 2022-09-21 12:41:34.000000 gs2-1.1.8/src/gs2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-09-21 12:41:34.000000 gs2-1.1.8/src/gs2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       61 2022-09-21 12:41:34.000000 gs2-1.1.8/src/gs2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2022-09-21 12:41:34.000000 gs2-1.1.8/src/gs2.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-28 06:10:27.867616 gs2-1.1.9/
+-rw-r--r--   0 root         (0) root         (0)      364 2022-09-28 06:10:27.867616 gs2-1.1.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-28 06:10:27.867616 gs2-1.1.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1384 2022-09-28 06:05:43.000000 gs2-1.1.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-28 06:10:27.831616 gs2-1.1.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-28 06:10:27.835615 gs2-1.1.9/src/gs2/
+-rw-r--r--   0 root         (0) root         (0)      792 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-28 06:10:27.835615 gs2-1.1.9/src/gs2/account/
+-rw-r--r--   0 root         (0) root         (0)      696 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/account/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21039 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/account/model.py
+-rw-r--r--   0 root         (0) root         (0)    44584 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/account/request.py
+-rw-r--r--   0 root         (0) root         (0)    61603 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/account/rest.py
+-rw-r--r--   0 root         (0) root         (0)    26232 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/account/result.py
+-rw-r--r--   0 root         (0) root         (0)    59296 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/account/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-28 06:10:27.835615 gs2-1.1.9/src/gs2/auth/
+-rw-r--r--   0 root         (0) root         (0)      696 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2133 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/auth/model.py
+-rw-r--r--   0 root         (0) root         (0)     3054 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/auth/request.py
+-rw-r--r--   0 root         (0) root         (0)     4777 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/auth/rest.py
+-rw-r--r--   0 root         (0) root         (0)     3127 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/auth/result.py
+-rw-r--r--   0 root         (0) root         (0)     4771 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/auth/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-28 06:10:27.835615 gs2-1.1.9/src/gs2/chat/
+-rw-r--r--   0 root         (0) root         (0)      696 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/chat/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25666 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/chat/model.py
+-rw-r--r--   0 root         (0) root         (0)    63678 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/chat/request.py
+-rw-r--r--   0 root         (0) root         (0)    78812 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/chat/rest.py
+-rw-r--r--   0 root         (0) root         (0)    32032 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/chat/result.py
+-rw-r--r--   0 root         (0) root         (0)    75904 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/chat/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-28 06:10:27.835615 gs2-1.1.9/src/gs2/core/
+-rw-r--r--   0 root         (0) root         (0)      188 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-28 06:10:27.835615 gs2-1.1.9/src/gs2/core/domain/
+-rw-r--r--   0 root         (0) root         (0)    10812 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/core/domain/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      274 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/core/domain/access_token.py
+-rw-r--r--   0 root         (0) root         (0)     3658 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/core/exception.py
+-rw-r--r--   0 root         (0) root         (0)     6581 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/core/model.py
+-rw-r--r--   0 root         (0) root         (0)    10580 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/core/rest.py
+-rw-r--r--   0 root         (0) root         (0)     1233 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/core/util.py
+-rw-r--r--   0 root         (0) root         (0)    10955 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/core/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-28 06:10:27.839615 gs2-1.1.9/src/gs2/datastore/
+-rw-r--r--   0 root         (0) root         (0)      696 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/datastore/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17622 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/datastore/model.py
+-rw-r--r--   0 root         (0) root         (0)    57176 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/datastore/request.py
+-rw-r--r--   0 root         (0) root         (0)    77053 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/datastore/rest.py
+-rw-r--r--   0 root         (0) root         (0)    37260 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/datastore/result.py
+-rw-r--r--   0 root         (0) root         (0)    74625 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/datastore/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-28 06:10:27.839615 gs2-1.1.9/src/gs2/deploy/
+-rw-r--r--   0 root         (0) root         (0)      696 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/deploy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19443 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/deploy/model.py
+-rw-r--r--   0 root         (0) root         (0)    21473 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/deploy/request.py
+-rw-r--r--   0 root         (0) root         (0)    38731 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/deploy/rest.py
+-rw-r--r--   0 root         (0) root         (0)    18118 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/deploy/result.py
+-rw-r--r--   0 root         (0) root         (0)    37185 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/deploy/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-28 06:10:27.839615 gs2-1.1.9/src/gs2/dictionary/
+-rw-r--r--   0 root         (0) root         (0)      696 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/dictionary/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23778 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/dictionary/model.py
+-rw-r--r--   0 root         (0) root         (0)    37763 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/dictionary/request.py
+-rw-r--r--   0 root         (0) root         (0)    60038 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/dictionary/rest.py
+-rw-r--r--   0 root         (0) root         (0)    27656 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/dictionary/result.py
+-rw-r--r--   0 root         (0) root         (0)    57798 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/dictionary/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-28 06:10:27.839615 gs2-1.1.9/src/gs2/distributor/
+-rw-r--r--   0 root         (0) root         (0)      696 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/distributor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30294 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/distributor/model.py
+-rw-r--r--   0 root         (0) root         (0)    40153 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/distributor/request.py
+-rw-r--r--   0 root         (0) root         (0)    63369 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/distributor/rest.py
+-rw-r--r--   0 root         (0) root         (0)    29638 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/distributor/result.py
+-rw-r--r--   0 root         (0) root         (0)    61505 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/distributor/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-28 06:10:27.839615 gs2-1.1.9/src/gs2/enhance/
+-rw-r--r--   0 root         (0) root         (0)      696 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/enhance/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    36059 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/enhance/model.py
+-rw-r--r--   0 root         (0) root         (0)    62716 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/enhance/request.py
+-rw-r--r--   0 root         (0) root         (0)    78687 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/enhance/rest.py
+-rw-r--r--   0 root         (0) root         (0)    43712 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/enhance/result.py
+-rw-r--r--   0 root         (0) root         (0)    75846 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/enhance/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-28 06:10:27.843616 gs2-1.1.9/src/gs2/exchange/
+-rw-r--r--   0 root         (0) root         (0)      696 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/exchange/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    34652 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/exchange/model.py
+-rw-r--r--   0 root         (0) root         (0)    63736 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/exchange/request.py
+-rw-r--r--   0 root         (0) root         (0)    82386 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/exchange/rest.py
+-rw-r--r--   0 root         (0) root         (0)    44513 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/exchange/result.py
+-rw-r--r--   0 root         (0) root         (0)    79193 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/exchange/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-28 06:10:27.843616 gs2-1.1.9/src/gs2/experience/
+-rw-r--r--   0 root         (0) root         (0)      696 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/experience/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    34902 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/experience/model.py
+-rw-r--r--   0 root         (0) root         (0)    63688 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/experience/request.py
+-rw-r--r--   0 root         (0) root         (0)    88409 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/experience/rest.py
+-rw-r--r--   0 root         (0) root         (0)    37534 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/experience/result.py
+-rw-r--r--   0 root         (0) root         (0)    84658 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/experience/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-28 06:10:27.843616 gs2-1.1.9/src/gs2/formation/
+-rw-r--r--   0 root         (0) root         (0)      696 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/formation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    52495 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/formation/model.py
+-rw-r--r--   0 root         (0) root         (0)   100988 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/formation/request.py
+-rw-r--r--   0 root         (0) root         (0)   141633 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/formation/rest.py
+-rw-r--r--   0 root         (0) root         (0)    78524 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/formation/result.py
+-rw-r--r--   0 root         (0) root         (0)   135549 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/formation/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-28 06:10:27.843616 gs2-1.1.9/src/gs2/friend/
+-rw-r--r--   0 root         (0) root         (0)      696 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/friend/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    43298 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/friend/model.py
+-rw-r--r--   0 root         (0) root         (0)    86971 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/friend/request.py
+-rw-r--r--   0 root         (0) root         (0)   116120 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/friend/rest.py
+-rw-r--r--   0 root         (0) root         (0)    49523 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/friend/result.py
+-rw-r--r--   0 root         (0) root         (0)   111985 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/friend/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-28 06:10:27.843616 gs2-1.1.9/src/gs2/gateway/
+-rw-r--r--   0 root         (0) root         (0)      696 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/gateway/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13068 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/gateway/model.py
+-rw-r--r--   0 root         (0) root         (0)    30343 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/gateway/request.py
+-rw-r--r--   0 root         (0) root         (0)    46374 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/gateway/rest.py
+-rw-r--r--   0 root         (0) root         (0)    20062 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/gateway/result.py
+-rw-r--r--   0 root         (0) root         (0)    45043 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/gateway/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-28 06:10:27.847616 gs2-1.1.9/src/gs2/identifier/
+-rw-r--r--   0 root         (0) root         (0)      696 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/identifier/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13178 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/identifier/model.py
+-rw-r--r--   0 root         (0) root         (0)    27417 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/identifier/request.py
+-rw-r--r--   0 root         (0) root         (0)    51631 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/identifier/rest.py
+-rw-r--r--   0 root         (0) root         (0)    26226 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/identifier/result.py
+-rw-r--r--   0 root         (0) root         (0)    49813 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/identifier/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-28 06:10:27.847616 gs2-1.1.9/src/gs2/inbox/
+-rw-r--r--   0 root         (0) root         (0)      696 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/inbox/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39659 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/inbox/model.py
+-rw-r--r--   0 root         (0) root         (0)    60409 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/inbox/request.py
+-rw-r--r--   0 root         (0) root         (0)    83314 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/inbox/rest.py
+-rw-r--r--   0 root         (0) root         (0)    38119 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/inbox/result.py
+-rw-r--r--   0 root         (0) root         (0)    80466 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/inbox/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-28 06:10:27.847616 gs2-1.1.9/src/gs2/inventory/
+-rw-r--r--   0 root         (0) root         (0)      696 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/inventory/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    47883 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/inventory/model.py
+-rw-r--r--   0 root         (0) root         (0)   106987 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/inventory/request.py
+-rw-r--r--   0 root         (0) root         (0)   145526 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/inventory/rest.py
+-rw-r--r--   0 root         (0) root         (0)    83791 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/inventory/result.py
+-rw-r--r--   0 root         (0) root         (0)   138438 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/inventory/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-28 06:10:27.847616 gs2-1.1.9/src/gs2/job_queue/
+-rw-r--r--   0 root         (0) root         (0)      696 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/job_queue/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25092 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/job_queue/model.py
+-rw-r--r--   0 root         (0) root         (0)    28055 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/job_queue/request.py
+-rw-r--r--   0 root         (0) root         (0)    41824 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/job_queue/rest.py
+-rw-r--r--   0 root         (0) root         (0)    20203 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/job_queue/result.py
+-rw-r--r--   0 root         (0) root         (0)    40098 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/job_queue/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-28 06:10:27.851616 gs2-1.1.9/src/gs2/key/
+-rw-r--r--   0 root         (0) root         (0)      696 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/key/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11874 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/key/model.py
+-rw-r--r--   0 root         (0) root         (0)    24617 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/key/request.py
+-rw-r--r--   0 root         (0) root         (0)    40001 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/key/rest.py
+-rw-r--r--   0 root         (0) root         (0)    17815 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/key/result.py
+-rw-r--r--   0 root         (0) root         (0)    38327 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/key/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-28 06:10:27.851616 gs2-1.1.9/src/gs2/limit/
+-rw-r--r--   0 root         (0) root         (0)      696 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/limit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23601 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/limit/model.py
+-rw-r--r--   0 root         (0) root         (0)    40251 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/limit/request.py
+-rw-r--r--   0 root         (0) root         (0)    60806 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/limit/rest.py
+-rw-r--r--   0 root         (0) root         (0)    26781 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/limit/result.py
+-rw-r--r--   0 root         (0) root         (0)    58511 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/limit/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-28 06:10:27.851616 gs2-1.1.9/src/gs2/lock/
+-rw-r--r--   0 root         (0) root         (0)      696 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/lock/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8758 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/lock/model.py
+-rw-r--r--   0 root         (0) root         (0)    23181 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/lock/request.py
+-rw-r--r--   0 root         (0) root         (0)    34491 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/lock/rest.py
+-rw-r--r--   0 root         (0) root         (0)    15295 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/lock/result.py
+-rw-r--r--   0 root         (0) root         (0)    33213 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/lock/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-28 06:10:27.855616 gs2-1.1.9/src/gs2/log/
+-rw-r--r--   0 root         (0) root         (0)      696 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25728 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/log/model.py
+-rw-r--r--   0 root         (0) root         (0)    41864 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/log/request.py
+-rw-r--r--   0 root         (0) root         (0)    49307 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/log/rest.py
+-rw-r--r--   0 root         (0) root         (0)    27100 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/log/result.py
+-rw-r--r--   0 root         (0) root         (0)    47078 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/log/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-28 06:10:27.855616 gs2-1.1.9/src/gs2/lottery/
+-rw-r--r--   0 root         (0) root         (0)      696 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/lottery/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    49829 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/lottery/model.py
+-rw-r--r--   0 root         (0) root         (0)    59242 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/lottery/request.py
+-rw-r--r--   0 root         (0) root         (0)    87536 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/lottery/rest.py
+-rw-r--r--   0 root         (0) root         (0)    40742 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/lottery/result.py
+-rw-r--r--   0 root         (0) root         (0)    83914 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/lottery/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-28 06:10:27.855616 gs2-1.1.9/src/gs2/matchmaking/
+-rw-r--r--   0 root         (0) root         (0)      696 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/matchmaking/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    50049 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/matchmaking/model.py
+-rw-r--r--   0 root         (0) root         (0)    77767 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/matchmaking/request.py
+-rw-r--r--   0 root         (0) root         (0)    98096 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/matchmaking/rest.py
+-rw-r--r--   0 root         (0) root         (0)    41546 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/matchmaking/result.py
+-rw-r--r--   0 root         (0) root         (0)    94510 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/matchmaking/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-28 06:10:27.855616 gs2-1.1.9/src/gs2/mega_field/
+-rw-r--r--   0 root         (0) root         (0)      696 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/mega_field/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39586 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/mega_field/model.py
+-rw-r--r--   0 root         (0) root         (0)    53867 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/mega_field/request.py
+-rw-r--r--   0 root         (0) root         (0)    76865 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/mega_field/rest.py
+-rw-r--r--   0 root         (0) root         (0)    32973 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/mega_field/result.py
+-rw-r--r--   0 root         (0) root         (0)    73270 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/mega_field/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-28 06:10:27.855616 gs2-1.1.9/src/gs2/mission/
+-rw-r--r--   0 root         (0) root         (0)      696 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/mission/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    64956 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/mission/model.py
+-rw-r--r--   0 root         (0) root         (0)    86838 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/mission/request.py
+-rw-r--r--   0 root         (0) root         (0)   116464 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/mission/rest.py
+-rw-r--r--   0 root         (0) root         (0)    51500 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/mission/result.py
+-rw-r--r--   0 root         (0) root         (0)   111559 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/mission/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-28 06:10:27.859616 gs2-1.1.9/src/gs2/money/
+-rw-r--r--   0 root         (0) root         (0)      696 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/money/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20794 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/money/model.py
+-rw-r--r--   0 root         (0) root         (0)    33783 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/money/request.py
+-rw-r--r--   0 root         (0) root         (0)    45386 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/money/rest.py
+-rw-r--r--   0 root         (0) root         (0)    20827 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/money/result.py
+-rw-r--r--   0 root         (0) root         (0)    43924 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/money/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-28 06:10:27.859616 gs2-1.1.9/src/gs2/news/
+-rw-r--r--   0 root         (0) root         (0)      696 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/news/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10517 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/news/model.py
+-rw-r--r--   0 root         (0) root         (0)    16136 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/news/request.py
+-rw-r--r--   0 root         (0) root         (0)    28973 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/news/rest.py
+-rw-r--r--   0 root         (0) root         (0)    15986 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/news/result.py
+-rw-r--r--   0 root         (0) root         (0)    28179 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/news/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-28 06:10:27.859616 gs2-1.1.9/src/gs2/quest/
+-rw-r--r--   0 root         (0) root         (0)      696 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/quest/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    55308 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/quest/model.py
+-rw-r--r--   0 root         (0) root         (0)    77678 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/quest/request.py
+-rw-r--r--   0 root         (0) root         (0)   101117 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/quest/rest.py
+-rw-r--r--   0 root         (0) root         (0)    48230 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/quest/result.py
+-rw-r--r--   0 root         (0) root         (0)    97317 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/quest/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-28 06:10:27.859616 gs2-1.1.9/src/gs2/ranking/
+-rw-r--r--   0 root         (0) root         (0)      696 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/ranking/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39347 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/ranking/model.py
+-rw-r--r--   0 root         (0) root         (0)    67281 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/ranking/request.py
+-rw-r--r--   0 root         (0) root         (0)    91769 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/ranking/rest.py
+-rw-r--r--   0 root         (0) root         (0)    38368 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/ranking/result.py
+-rw-r--r--   0 root         (0) root         (0)    87350 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/ranking/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-28 06:10:27.859616 gs2-1.1.9/src/gs2/realtime/
+-rw-r--r--   0 root         (0) root         (0)      696 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/realtime/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11834 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/realtime/model.py
+-rw-r--r--   0 root         (0) root         (0)    15593 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/realtime/request.py
+-rw-r--r--   0 root         (0) root         (0)    24405 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/realtime/rest.py
+-rw-r--r--   0 root         (0) root         (0)    11177 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/realtime/result.py
+-rw-r--r--   0 root         (0) root         (0)    23545 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/realtime/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-28 06:10:27.863616 gs2-1.1.9/src/gs2/schedule/
+-rw-r--r--   0 root         (0) root         (0)      696 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/schedule/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27411 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/schedule/model.py
+-rw-r--r--   0 root         (0) root         (0)    46255 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/schedule/request.py
+-rw-r--r--   0 root         (0) root         (0)    66261 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/schedule/rest.py
+-rw-r--r--   0 root         (0) root         (0)    28460 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/schedule/result.py
+-rw-r--r--   0 root         (0) root         (0)    63762 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/schedule/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-28 06:10:27.863616 gs2-1.1.9/src/gs2/script/
+-rw-r--r--   0 root         (0) root         (0)      696 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/script/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10923 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/script/model.py
+-rw-r--r--   0 root         (0) root         (0)    20581 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/script/request.py
+-rw-r--r--   0 root         (0) root         (0)    33346 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/script/rest.py
+-rw-r--r--   0 root         (0) root         (0)    17019 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/script/result.py
+-rw-r--r--   0 root         (0) root         (0)    32201 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/script/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-28 06:10:27.863616 gs2-1.1.9/src/gs2/serial_key/
+-rw-r--r--   0 root         (0) root         (0)      696 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/serial_key/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26449 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/serial_key/model.py
+-rw-r--r--   0 root         (0) root         (0)    36692 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/serial_key/request.py
+-rw-r--r--   0 root         (0) root         (0)    59697 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/serial_key/rest.py
+-rw-r--r--   0 root         (0) root         (0)    28304 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/serial_key/result.py
+-rw-r--r--   0 root         (0) root         (0)    57135 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/serial_key/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-28 06:10:27.863616 gs2-1.1.9/src/gs2/showcase/
+-rw-r--r--   0 root         (0) root         (0)      696 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/showcase/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    44174 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/showcase/model.py
+-rw-r--r--   0 root         (0) root         (0)    53664 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/showcase/request.py
+-rw-r--r--   0 root         (0) root         (0)    74863 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/showcase/rest.py
+-rw-r--r--   0 root         (0) root         (0)    34249 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/showcase/result.py
+-rw-r--r--   0 root         (0) root         (0)    72013 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/showcase/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-28 06:10:27.863616 gs2-1.1.9/src/gs2/stamina/
+-rw-r--r--   0 root         (0) root         (0)      696 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/stamina/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56778 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/stamina/model.py
+-rw-r--r--   0 root         (0) root         (0)    96095 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/stamina/request.py
+-rw-r--r--   0 root         (0) root         (0)   133258 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/stamina/rest.py
+-rw-r--r--   0 root         (0) root         (0)    62943 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/stamina/result.py
+-rw-r--r--   0 root         (0) root         (0)   128508 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/stamina/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-28 06:10:27.867616 gs2-1.1.9/src/gs2/version/
+-rw-r--r--   0 root         (0) root         (0)      696 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/version/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    33415 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/version/model.py
+-rw-r--r--   0 root         (0) root         (0)    46417 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/version/request.py
+-rw-r--r--   0 root         (0) root         (0)    66565 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/version/rest.py
+-rw-r--r--   0 root         (0) root         (0)    31007 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/version/result.py
+-rw-r--r--   0 root         (0) root         (0)    64446 2022-09-28 06:05:43.000000 gs2-1.1.9/src/gs2/version/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-28 06:10:27.835615 gs2-1.1.9/src/gs2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      364 2022-09-28 06:10:27.000000 gs2-1.1.9/src/gs2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6176 2022-09-28 06:10:27.000000 gs2-1.1.9/src/gs2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-28 06:10:27.000000 gs2-1.1.9/src/gs2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       61 2022-09-28 06:10:27.000000 gs2-1.1.9/src/gs2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2022-09-28 06:10:27.000000 gs2-1.1.9/src/gs2.egg-info/top_level.txt
```

### Comparing `gs2-1.1.8/setup.py` & `gs2-1.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 from setuptools import setup, find_packages
 
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='gs2',
-    version='1.1.8',
+    version='1.1.9',
     package_dir={'': 'src'},
     py_modules=["gs2"],
     packages=find_packages('src'),
     install_requires=[
         'websocket_client >= 0.59.0',
         'simplejson >= 3.17.2',
         'requests >= 2.25.1',
```

### Comparing `gs2-1.1.8/src/gs2/__init__.py` & `gs2-1.1.9/src/gs2/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/account/__init__.py` & `gs2-1.1.9/src/gs2/account/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/account/model.py` & `gs2-1.1.9/src/gs2/account/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/account/request.py` & `gs2-1.1.9/src/gs2/account/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/account/rest.py` & `gs2-1.1.9/src/gs2/account/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/account/result.py` & `gs2-1.1.9/src/gs2/account/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/account/web_socket.py` & `gs2-1.1.9/src/gs2/account/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/auth/__init__.py` & `gs2-1.1.9/src/gs2/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/auth/model.py` & `gs2-1.1.9/src/gs2/auth/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/auth/request.py` & `gs2-1.1.9/src/gs2/auth/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/auth/rest.py` & `gs2-1.1.9/src/gs2/auth/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/auth/result.py` & `gs2-1.1.9/src/gs2/auth/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/auth/web_socket.py` & `gs2-1.1.9/src/gs2/auth/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/chat/__init__.py` & `gs2-1.1.9/src/gs2/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/chat/model.py` & `gs2-1.1.9/src/gs2/chat/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/chat/request.py` & `gs2-1.1.9/src/gs2/chat/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/chat/rest.py` & `gs2-1.1.9/src/gs2/chat/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/chat/result.py` & `gs2-1.1.9/src/gs2/chat/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/chat/web_socket.py` & `gs2-1.1.9/src/gs2/chat/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/core/domain/__init__.py` & `gs2-1.1.9/src/gs2/core/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/core/exception.py` & `gs2-1.1.9/src/gs2/core/exception.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/core/model.py` & `gs2-1.1.9/src/gs2/core/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/core/rest.py` & `gs2-1.1.9/src/gs2/core/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/core/util.py` & `gs2-1.1.9/src/gs2/core/util.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/core/web_socket.py` & `gs2-1.1.9/src/gs2/core/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/datastore/__init__.py` & `gs2-1.1.9/src/gs2/datastore/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/datastore/model.py` & `gs2-1.1.9/src/gs2/datastore/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/datastore/request.py` & `gs2-1.1.9/src/gs2/datastore/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/datastore/rest.py` & `gs2-1.1.9/src/gs2/datastore/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/datastore/result.py` & `gs2-1.1.9/src/gs2/datastore/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/datastore/web_socket.py` & `gs2-1.1.9/src/gs2/datastore/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/deploy/__init__.py` & `gs2-1.1.9/src/gs2/deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/deploy/model.py` & `gs2-1.1.9/src/gs2/deploy/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/deploy/request.py` & `gs2-1.1.9/src/gs2/deploy/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/deploy/rest.py` & `gs2-1.1.9/src/gs2/deploy/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/deploy/result.py` & `gs2-1.1.9/src/gs2/deploy/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/deploy/web_socket.py` & `gs2-1.1.9/src/gs2/deploy/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/dictionary/__init__.py` & `gs2-1.1.9/src/gs2/dictionary/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/dictionary/model.py` & `gs2-1.1.9/src/gs2/dictionary/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/dictionary/request.py` & `gs2-1.1.9/src/gs2/dictionary/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/dictionary/rest.py` & `gs2-1.1.9/src/gs2/dictionary/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/dictionary/result.py` & `gs2-1.1.9/src/gs2/dictionary/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/dictionary/web_socket.py` & `gs2-1.1.9/src/gs2/dictionary/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/distributor/__init__.py` & `gs2-1.1.9/src/gs2/distributor/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/distributor/model.py` & `gs2-1.1.9/src/gs2/distributor/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/distributor/request.py` & `gs2-1.1.9/src/gs2/distributor/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/distributor/rest.py` & `gs2-1.1.9/src/gs2/distributor/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/distributor/result.py` & `gs2-1.1.9/src/gs2/distributor/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/distributor/web_socket.py` & `gs2-1.1.9/src/gs2/distributor/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/enhance/__init__.py` & `gs2-1.1.9/src/gs2/enhance/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/enhance/model.py` & `gs2-1.1.9/src/gs2/enhance/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/enhance/request.py` & `gs2-1.1.9/src/gs2/enhance/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/enhance/rest.py` & `gs2-1.1.9/src/gs2/enhance/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/enhance/result.py` & `gs2-1.1.9/src/gs2/enhance/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/enhance/web_socket.py` & `gs2-1.1.9/src/gs2/enhance/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/exchange/__init__.py` & `gs2-1.1.9/src/gs2/exchange/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/exchange/model.py` & `gs2-1.1.9/src/gs2/exchange/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/exchange/request.py` & `gs2-1.1.9/src/gs2/exchange/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/exchange/rest.py` & `gs2-1.1.9/src/gs2/exchange/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/exchange/result.py` & `gs2-1.1.9/src/gs2/exchange/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/exchange/web_socket.py` & `gs2-1.1.9/src/gs2/exchange/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/experience/__init__.py` & `gs2-1.1.9/src/gs2/experience/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/experience/model.py` & `gs2-1.1.9/src/gs2/experience/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/experience/request.py` & `gs2-1.1.9/src/gs2/experience/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/experience/rest.py` & `gs2-1.1.9/src/gs2/experience/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/experience/result.py` & `gs2-1.1.9/src/gs2/experience/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/experience/web_socket.py` & `gs2-1.1.9/src/gs2/experience/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/formation/__init__.py` & `gs2-1.1.9/src/gs2/formation/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/formation/model.py` & `gs2-1.1.9/src/gs2/formation/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/formation/request.py` & `gs2-1.1.9/src/gs2/formation/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/formation/rest.py` & `gs2-1.1.9/src/gs2/formation/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/formation/result.py` & `gs2-1.1.9/src/gs2/formation/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/formation/web_socket.py` & `gs2-1.1.9/src/gs2/formation/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/friend/__init__.py` & `gs2-1.1.9/src/gs2/friend/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/friend/model.py` & `gs2-1.1.9/src/gs2/friend/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/friend/request.py` & `gs2-1.1.9/src/gs2/friend/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/friend/rest.py` & `gs2-1.1.9/src/gs2/friend/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/friend/result.py` & `gs2-1.1.9/src/gs2/friend/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/friend/web_socket.py` & `gs2-1.1.9/src/gs2/friend/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/gateway/__init__.py` & `gs2-1.1.9/src/gs2/gateway/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/gateway/model.py` & `gs2-1.1.9/src/gs2/gateway/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/gateway/request.py` & `gs2-1.1.9/src/gs2/gateway/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/gateway/rest.py` & `gs2-1.1.9/src/gs2/gateway/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/gateway/result.py` & `gs2-1.1.9/src/gs2/gateway/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/gateway/web_socket.py` & `gs2-1.1.9/src/gs2/gateway/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/identifier/__init__.py` & `gs2-1.1.9/src/gs2/identifier/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/identifier/model.py` & `gs2-1.1.9/src/gs2/identifier/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/identifier/request.py` & `gs2-1.1.9/src/gs2/identifier/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/identifier/rest.py` & `gs2-1.1.9/src/gs2/identifier/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/identifier/result.py` & `gs2-1.1.9/src/gs2/identifier/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/identifier/web_socket.py` & `gs2-1.1.9/src/gs2/identifier/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/inbox/__init__.py` & `gs2-1.1.9/src/gs2/inbox/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/inbox/model.py` & `gs2-1.1.9/src/gs2/inbox/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/inbox/request.py` & `gs2-1.1.9/src/gs2/inbox/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/inbox/rest.py` & `gs2-1.1.9/src/gs2/inbox/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/inbox/result.py` & `gs2-1.1.9/src/gs2/inbox/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/inbox/web_socket.py` & `gs2-1.1.9/src/gs2/inbox/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/inventory/__init__.py` & `gs2-1.1.9/src/gs2/inventory/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/inventory/model.py` & `gs2-1.1.9/src/gs2/inventory/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/inventory/request.py` & `gs2-1.1.9/src/gs2/inventory/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/inventory/rest.py` & `gs2-1.1.9/src/gs2/inventory/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/inventory/result.py` & `gs2-1.1.9/src/gs2/inventory/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/inventory/web_socket.py` & `gs2-1.1.9/src/gs2/inventory/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/job_queue/__init__.py` & `gs2-1.1.9/src/gs2/job_queue/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/job_queue/model.py` & `gs2-1.1.9/src/gs2/job_queue/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/job_queue/request.py` & `gs2-1.1.9/src/gs2/job_queue/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/job_queue/rest.py` & `gs2-1.1.9/src/gs2/job_queue/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/job_queue/result.py` & `gs2-1.1.9/src/gs2/job_queue/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/job_queue/web_socket.py` & `gs2-1.1.9/src/gs2/job_queue/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/key/__init__.py` & `gs2-1.1.9/src/gs2/key/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/key/model.py` & `gs2-1.1.9/src/gs2/key/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/key/request.py` & `gs2-1.1.9/src/gs2/key/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/key/rest.py` & `gs2-1.1.9/src/gs2/key/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/key/result.py` & `gs2-1.1.9/src/gs2/key/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/key/web_socket.py` & `gs2-1.1.9/src/gs2/key/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/limit/__init__.py` & `gs2-1.1.9/src/gs2/limit/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/limit/model.py` & `gs2-1.1.9/src/gs2/limit/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/limit/request.py` & `gs2-1.1.9/src/gs2/limit/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/limit/rest.py` & `gs2-1.1.9/src/gs2/limit/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/limit/result.py` & `gs2-1.1.9/src/gs2/limit/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/limit/web_socket.py` & `gs2-1.1.9/src/gs2/limit/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/lock/__init__.py` & `gs2-1.1.9/src/gs2/lock/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/lock/model.py` & `gs2-1.1.9/src/gs2/lock/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/lock/request.py` & `gs2-1.1.9/src/gs2/lock/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/lock/rest.py` & `gs2-1.1.9/src/gs2/lock/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/lock/result.py` & `gs2-1.1.9/src/gs2/lock/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/lock/web_socket.py` & `gs2-1.1.9/src/gs2/lock/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/log/__init__.py` & `gs2-1.1.9/src/gs2/log/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/log/model.py` & `gs2-1.1.9/src/gs2/log/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/log/request.py` & `gs2-1.1.9/src/gs2/log/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/log/rest.py` & `gs2-1.1.9/src/gs2/log/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/log/result.py` & `gs2-1.1.9/src/gs2/log/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/log/web_socket.py` & `gs2-1.1.9/src/gs2/log/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/lottery/__init__.py` & `gs2-1.1.9/src/gs2/lottery/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/lottery/model.py` & `gs2-1.1.9/src/gs2/lottery/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/lottery/request.py` & `gs2-1.1.9/src/gs2/lottery/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/lottery/rest.py` & `gs2-1.1.9/src/gs2/lottery/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/lottery/result.py` & `gs2-1.1.9/src/gs2/lottery/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/lottery/web_socket.py` & `gs2-1.1.9/src/gs2/lottery/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/matchmaking/__init__.py` & `gs2-1.1.9/src/gs2/matchmaking/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/matchmaking/model.py` & `gs2-1.1.9/src/gs2/matchmaking/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/matchmaking/request.py` & `gs2-1.1.9/src/gs2/matchmaking/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/matchmaking/rest.py` & `gs2-1.1.9/src/gs2/matchmaking/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/matchmaking/result.py` & `gs2-1.1.9/src/gs2/matchmaking/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/matchmaking/web_socket.py` & `gs2-1.1.9/src/gs2/matchmaking/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/mega_field/__init__.py` & `gs2-1.1.9/src/gs2/mega_field/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/mega_field/model.py` & `gs2-1.1.9/src/gs2/mega_field/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/mega_field/request.py` & `gs2-1.1.9/src/gs2/mega_field/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/mega_field/rest.py` & `gs2-1.1.9/src/gs2/mega_field/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/mega_field/result.py` & `gs2-1.1.9/src/gs2/mega_field/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/mega_field/web_socket.py` & `gs2-1.1.9/src/gs2/mega_field/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/mission/__init__.py` & `gs2-1.1.9/src/gs2/mission/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/mission/model.py` & `gs2-1.1.9/src/gs2/mission/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/mission/request.py` & `gs2-1.1.9/src/gs2/mission/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/mission/rest.py` & `gs2-1.1.9/src/gs2/mission/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/mission/result.py` & `gs2-1.1.9/src/gs2/mission/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/mission/web_socket.py` & `gs2-1.1.9/src/gs2/mission/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/money/__init__.py` & `gs2-1.1.9/src/gs2/money/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/money/model.py` & `gs2-1.1.9/src/gs2/money/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/money/request.py` & `gs2-1.1.9/src/gs2/money/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/money/rest.py` & `gs2-1.1.9/src/gs2/money/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/money/result.py` & `gs2-1.1.9/src/gs2/money/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/money/web_socket.py` & `gs2-1.1.9/src/gs2/money/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/news/__init__.py` & `gs2-1.1.9/src/gs2/news/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/news/model.py` & `gs2-1.1.9/src/gs2/news/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/news/request.py` & `gs2-1.1.9/src/gs2/news/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/news/rest.py` & `gs2-1.1.9/src/gs2/news/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/news/result.py` & `gs2-1.1.9/src/gs2/news/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/news/web_socket.py` & `gs2-1.1.9/src/gs2/news/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/quest/__init__.py` & `gs2-1.1.9/src/gs2/quest/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/quest/model.py` & `gs2-1.1.9/src/gs2/quest/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/quest/request.py` & `gs2-1.1.9/src/gs2/quest/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/quest/rest.py` & `gs2-1.1.9/src/gs2/quest/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/quest/result.py` & `gs2-1.1.9/src/gs2/quest/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/quest/web_socket.py` & `gs2-1.1.9/src/gs2/quest/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/ranking/__init__.py` & `gs2-1.1.9/src/gs2/ranking/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/ranking/model.py` & `gs2-1.1.9/src/gs2/ranking/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/ranking/request.py` & `gs2-1.1.9/src/gs2/ranking/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/ranking/rest.py` & `gs2-1.1.9/src/gs2/ranking/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/ranking/result.py` & `gs2-1.1.9/src/gs2/ranking/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/ranking/web_socket.py` & `gs2-1.1.9/src/gs2/ranking/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/realtime/__init__.py` & `gs2-1.1.9/src/gs2/realtime/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/realtime/model.py` & `gs2-1.1.9/src/gs2/realtime/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/realtime/request.py` & `gs2-1.1.9/src/gs2/realtime/request.py`

 * *Files 1% similar despite different names*

```diff
@@ -306,14 +306,43 @@
 
     def to_dict(self) -> Dict[str, Any]:
         return {
             "namespaceName": self.namespace_name,
         }
 
 
+class NowRequest(core.Gs2Request):
+
+    context_stack: str = None
+
+    def get(self, key, default=None):
+        items = self.to_dict()
+        if key in items.keys():
+            return items[key]
+        return default
+
+    def __getitem__(self, key):
+        items = self.to_dict()
+        if key in items.keys():
+            return items[key]
+        return None
+
+    @staticmethod
+    def from_dict(
+        data: Dict[str, Any],
+    ) -> Optional[NowRequest]:
+        if data is None:
+            return None
+        return NowRequest()\
+
+    def to_dict(self) -> Dict[str, Any]:
+        return {
+        }
+
+
 class DescribeRoomsRequest(core.Gs2Request):
 
     context_stack: str = None
     namespace_name: str = None
     page_token: str = None
     limit: int = None
```

### Comparing `gs2-1.1.8/src/gs2/realtime/rest.py` & `gs2-1.1.9/src/gs2/realtime/rest.py`

 * *Files 5% similar despite different names*

```diff
@@ -465,14 +465,83 @@
             while not async_result:
                 await asyncio.sleep(0.01)
 
         if async_result[0].error:
             raise async_result[0].error
         return async_result[0].result
 
+    def _now(
+        self,
+        request: NowRequest,
+        callback: Callable[[AsyncResult[NowResult]], None],
+        is_blocking: bool,
+    ):
+        url = Gs2Constant.ENDPOINT_HOST.format(
+            service='realtime',
+            region=self.session.region,
+        ) + "/now"
+
+        headers = self._create_authorized_headers()
+        query_strings = {
+            'contextStack': request.context_stack,
+        }
+
+        if request.request_id:
+            headers["X-GS2-REQUEST-ID"] = request.request_id
+        _job = rest.NetworkJob(
+            url=url,
+            method='GET',
+            result_type=NowResult,
+            callback=callback,
+            headers=headers,
+            query_strings=query_strings,
+        )
+
+        self.session.send(
+            job=_job,
+            is_blocking=is_blocking,
+        )
+
+    def now(
+        self,
+        request: NowRequest,
+    ) -> NowResult:
+        async_result = []
+        with timeout(30):
+            self._now(
+                request,
+                lambda result: async_result.append(result),
+                is_blocking=True,
+            )
+
+        if async_result[0].error:
+            raise async_result[0].error
+        return async_result[0].result
+
+
+    async def now_async(
+        self,
+        request: NowRequest,
+    ) -> NowResult:
+        async_result = []
+        self._now(
+            request,
+            lambda result: async_result.append(result),
+            is_blocking=False,
+        )
+
+        import asyncio
+        with timeout(30):
+            while not async_result:
+                await asyncio.sleep(0.01)
+
+        if async_result[0].error:
+            raise async_result[0].error
+        return async_result[0].result
+
     def _describe_rooms(
         self,
         request: DescribeRoomsRequest,
         callback: Callable[[AsyncResult[DescribeRoomsResult]], None],
         is_blocking: bool,
     ):
         url = Gs2Constant.ENDPOINT_HOST.format(
```

### Comparing `gs2-1.1.8/src/gs2/realtime/result.py` & `gs2-1.1.9/src/gs2/realtime/result.py`

 * *Files 2% similar despite different names*

```diff
@@ -230,14 +230,48 @@
 
     def to_dict(self) -> Dict[str, Any]:
         return {
             "item": self.item.to_dict() if self.item else None,
         }
 
 
+class NowResult(core.Gs2Result):
+    timestamp: int = None
+
+    def with_timestamp(self, timestamp: int) -> NowResult:
+        self.timestamp = timestamp
+        return self
+
+    def get(self, key, default=None):
+        items = self.to_dict()
+        if key in items.keys():
+            return items[key]
+        return default
+
+    def __getitem__(self, key):
+        items = self.to_dict()
+        if key in items.keys():
+            return items[key]
+        return None
+
+    @staticmethod
+    def from_dict(
+        data: Dict[str, Any],
+    ) -> Optional[NowResult]:
+        if data is None:
+            return None
+        return NowResult()\
+            .with_timestamp(data.get('timestamp'))
+
+    def to_dict(self) -> Dict[str, Any]:
+        return {
+            "timestamp": self.timestamp,
+        }
+
+
 class DescribeRoomsResult(core.Gs2Result):
     items: List[Room] = None
     next_page_token: str = None
 
     def with_items(self, items: List[Room]) -> DescribeRoomsResult:
         self.items = items
         return self
```

### Comparing `gs2-1.1.8/src/gs2/realtime/web_socket.py` & `gs2-1.1.9/src/gs2/realtime/web_socket.py`

 * *Files 5% similar despite different names*

```diff
@@ -465,14 +465,83 @@
             while not async_result:
                 await asyncio.sleep(0.01)
 
         if async_result[0].error:
             raise async_result[0].error
         return async_result[0].result
 
+    def _now(
+        self,
+        request: NowRequest,
+        callback: Callable[[AsyncResult[NowResult]], None],
+    ):
+        import uuid
+
+        request_id = str(uuid.uuid4())
+        body = self._create_metadata(
+            service="realtime",
+            component='namespace',
+            function='now',
+            request_id=request_id,
+        )
+
+        if request.context_stack:
+            body['contextStack'] = str(request.context_stack)
+
+        if request.request_id:
+            body["xGs2RequestId"] = request.request_id
+
+        self.session.send(
+            web_socket.NetworkJob(
+                request_id=request_id,
+                result_type=NowResult,
+                callback=callback,
+                body=body,
+            )
+        )
+
+    def now(
+        self,
+        request: NowRequest,
+    ) -> NowResult:
+        async_result = []
+        with timeout(30):
+            self._now(
+                request,
+                lambda result: async_result.append(result),
+            )
+
+        with timeout(30):
+            while not async_result:
+                time.sleep(0.01)
+
+        if async_result[0].error:
+            raise async_result[0].error
+        return async_result[0].result
+
+
+    async def now_async(
+        self,
+        request: NowRequest,
+    ) -> NowResult:
+        async_result = []
+        self._now(
+            request,
+            lambda result: async_result.append(result),
+        )
+
+        import asyncio
+        with timeout(30):
+            while not async_result:
+                await asyncio.sleep(0.01)
+
+        if async_result[0].error:
+            raise async_result[0].error
+        return async_result[0].result
+
     def _describe_rooms(
         self,
         request: DescribeRoomsRequest,
         callback: Callable[[AsyncResult[DescribeRoomsResult]], None],
     ):
         import uuid
```

### Comparing `gs2-1.1.8/src/gs2/schedule/__init__.py` & `gs2-1.1.9/src/gs2/schedule/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/schedule/model.py` & `gs2-1.1.9/src/gs2/schedule/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/schedule/request.py` & `gs2-1.1.9/src/gs2/schedule/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/schedule/rest.py` & `gs2-1.1.9/src/gs2/schedule/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/schedule/result.py` & `gs2-1.1.9/src/gs2/schedule/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/schedule/web_socket.py` & `gs2-1.1.9/src/gs2/schedule/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/script/__init__.py` & `gs2-1.1.9/src/gs2/script/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/script/model.py` & `gs2-1.1.9/src/gs2/script/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/script/request.py` & `gs2-1.1.9/src/gs2/script/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/script/rest.py` & `gs2-1.1.9/src/gs2/script/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/script/result.py` & `gs2-1.1.9/src/gs2/script/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/script/web_socket.py` & `gs2-1.1.9/src/gs2/script/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/serial_key/__init__.py` & `gs2-1.1.9/src/gs2/serial_key/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/serial_key/model.py` & `gs2-1.1.9/src/gs2/serial_key/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/serial_key/request.py` & `gs2-1.1.9/src/gs2/serial_key/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/serial_key/rest.py` & `gs2-1.1.9/src/gs2/serial_key/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/serial_key/result.py` & `gs2-1.1.9/src/gs2/serial_key/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/serial_key/web_socket.py` & `gs2-1.1.9/src/gs2/serial_key/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/showcase/__init__.py` & `gs2-1.1.9/src/gs2/showcase/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/showcase/model.py` & `gs2-1.1.9/src/gs2/showcase/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/showcase/request.py` & `gs2-1.1.9/src/gs2/showcase/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/showcase/rest.py` & `gs2-1.1.9/src/gs2/showcase/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/showcase/result.py` & `gs2-1.1.9/src/gs2/showcase/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/showcase/web_socket.py` & `gs2-1.1.9/src/gs2/showcase/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/stamina/__init__.py` & `gs2-1.1.9/src/gs2/stamina/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/stamina/model.py` & `gs2-1.1.9/src/gs2/stamina/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/stamina/request.py` & `gs2-1.1.9/src/gs2/stamina/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/stamina/rest.py` & `gs2-1.1.9/src/gs2/stamina/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/stamina/result.py` & `gs2-1.1.9/src/gs2/stamina/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/stamina/web_socket.py` & `gs2-1.1.9/src/gs2/stamina/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/version/__init__.py` & `gs2-1.1.9/src/gs2/version/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/version/model.py` & `gs2-1.1.9/src/gs2/version/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/version/request.py` & `gs2-1.1.9/src/gs2/version/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/version/rest.py` & `gs2-1.1.9/src/gs2/version/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/version/result.py` & `gs2-1.1.9/src/gs2/version/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2/version/web_socket.py` & `gs2-1.1.9/src/gs2/version/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.8/src/gs2.egg-info/SOURCES.txt` & `gs2-1.1.9/src/gs2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

