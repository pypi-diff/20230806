# Comparing `tmp/yaylib-1.0.8.tar.gz` & `tmp/yaylib-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaylib-1.0.8.tar", last modified: Fri Aug  4 11:48:25 2023, max compression
+gzip compressed data, was "yaylib-1.0.9.tar", last modified: Sun Aug  6 09:06:43 2023, max compression
```

## Comparing `yaylib-1.0.8.tar` & `yaylib-1.0.9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 11:48:25.264502 yaylib-1.0.8/
--rw-rw-rw-   0        0        0     1096 2023-07-09 07:25:01.000000 yaylib-1.0.8/LICENSE
--rw-rw-rw-   0        0        0    12901 2023-08-04 11:48:25.264502 yaylib-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0    11986 2023-08-03 05:52:33.000000 yaylib-1.0.8/README.md
--rw-rw-rw-   0        0        0       42 2023-08-04 11:48:25.264502 yaylib-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1646 2023-08-03 05:52:33.000000 yaylib-1.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-04 11:48:25.213107 yaylib-1.0.8/tests/
--rw-rw-rw-   0        0        0        0 2023-08-03 05:52:33.000000 yaylib-1.0.8/tests/__init__.py
--rw-rw-rw-   0        0        0     2205 2023-08-03 05:52:33.000000 yaylib-1.0.8/tests/config.py
--rw-rw-rw-   0        0        0     1335 2023-07-09 07:25:01.000000 yaylib-1.0.8/tests/test_call.py
--rw-rw-rw-   0        0        0     1935 2023-07-09 07:25:01.000000 yaylib-1.0.8/tests/test_cassandra.py
--rw-rw-rw-   0        0        0     1335 2023-07-09 07:25:01.000000 yaylib-1.0.8/tests/test_chat.py
--rw-rw-rw-   0        0        0     1337 2023-07-09 07:25:01.000000 yaylib-1.0.8/tests/test_group.py
--rw-rw-rw-   0        0        0     1335 2023-07-09 07:25:01.000000 yaylib-1.0.8/tests/test_misc.py
--rw-rw-rw-   0        0        0     3723 2023-07-09 07:25:01.000000 yaylib-1.0.8/tests/test_post.py
--rw-rw-rw-   0        0        0     2028 2023-07-09 07:25:01.000000 yaylib-1.0.8/tests/test_review.py
--rw-rw-rw-   0        0        0     1339 2023-07-09 07:25:01.000000 yaylib-1.0.8/tests/test_thread.py
--rw-rw-rw-   0        0        0     1335 2023-07-09 07:25:01.000000 yaylib-1.0.8/tests/test_user.py
--rw-rw-rw-   0        0        0     1908 2023-08-03 05:52:33.000000 yaylib-1.0.8/tests/test_utils.py
-drwxrwxrwx   0        0        0        0 2023-08-04 11:48:25.222441 yaylib-1.0.8/yaylib/
--rw-rw-rw-   0        0        0      668 2023-08-04 08:28:13.000000 yaylib-1.0.8/yaylib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-04 11:48:25.263292 yaylib-1.0.8/yaylib/api/
--rw-rw-rw-   0        0        0      715 2023-08-03 05:52:33.000000 yaylib-1.0.8/yaylib/api/__init__.py
--rw-rw-rw-   0        0        0    14777 2023-08-04 08:22:26.000000 yaylib-1.0.8/yaylib/api/api.py
--rw-rw-rw-   0        0        0     9429 2023-08-03 05:52:33.000000 yaylib-1.0.8/yaylib/api/call.py
--rw-rw-rw-   0        0        0     2713 2023-08-03 05:52:33.000000 yaylib-1.0.8/yaylib/api/cassandra.py
--rw-rw-rw-   0        0        0    14964 2023-08-03 05:52:33.000000 yaylib-1.0.8/yaylib/api/chat.py
--rw-rw-rw-   0        0        0    23520 2023-08-04 11:39:54.000000 yaylib-1.0.8/yaylib/api/group.py
--rw-rw-rw-   0        0        0     8253 2023-08-03 05:52:33.000000 yaylib-1.0.8/yaylib/api/login.py
--rw-rw-rw-   0        0        0     7417 2023-07-18 08:52:45.000000 yaylib-1.0.8/yaylib/api/misc.py
--rw-rw-rw-   0        0        0    33647 2023-08-03 05:52:33.000000 yaylib-1.0.8/yaylib/api/post.py
--rw-rw-rw-   0        0        0     4445 2023-08-03 05:52:33.000000 yaylib-1.0.8/yaylib/api/review.py
--rw-rw-rw-   0        0        0     5945 2023-07-18 08:52:45.000000 yaylib-1.0.8/yaylib/api/thread.py
--rw-rw-rw-   0        0        0    23685 2023-08-03 05:52:33.000000 yaylib-1.0.8/yaylib/api/user.py
--rw-rw-rw-   0        0        0     9409 2023-08-03 05:52:33.000000 yaylib-1.0.8/yaylib/api/websocket.py
--rw-rw-rw-   0        0        0    86748 2023-08-04 11:40:27.000000 yaylib-1.0.8/yaylib/client.py
--rw-rw-rw-   0        0        0    18880 2023-08-04 11:46:28.000000 yaylib-1.0.8/yaylib/config.py
--rw-rw-rw-   0        0        0     2131 2023-07-18 08:52:45.000000 yaylib-1.0.8/yaylib/errors.py
--rw-rw-rw-   0        0        0    56916 2023-08-04 11:41:18.000000 yaylib-1.0.8/yaylib/models.py
--rw-rw-rw-   0        0        0    34292 2023-08-03 05:52:33.000000 yaylib-1.0.8/yaylib/responses.py
--rw-rw-rw-   0        0        0     1643 2023-08-03 05:52:33.000000 yaylib-1.0.8/yaylib/utils.py
-drwxrwxrwx   0        0        0        0 2023-08-04 11:48:25.246967 yaylib-1.0.8/yaylib.egg-info/
--rw-rw-rw-   0        0        0    12901 2023-08-04 11:48:25.000000 yaylib-1.0.8/yaylib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      799 2023-08-04 11:48:25.000000 yaylib-1.0.8/yaylib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 11:48:25.000000 yaylib-1.0.8/yaylib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-08-04 11:48:25.000000 yaylib-1.0.8/yaylib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-08-04 11:48:25.000000 yaylib-1.0.8/yaylib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-06 09:06:43.111930 yaylib-1.0.9/
+-rw-rw-rw-   0        0        0     1096 2023-07-09 07:25:01.000000 yaylib-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0    12869 2023-08-06 09:06:43.111930 yaylib-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0    11954 2023-08-06 00:16:10.000000 yaylib-1.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-06 09:06:43.111930 yaylib-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1646 2023-08-03 05:52:33.000000 yaylib-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-06 09:06:43.079844 yaylib-1.0.9/tests/
+-rw-rw-rw-   0        0        0        0 2023-08-03 05:52:33.000000 yaylib-1.0.9/tests/__init__.py
+-rw-rw-rw-   0        0        0     2205 2023-08-03 05:52:33.000000 yaylib-1.0.9/tests/config.py
+-rw-rw-rw-   0        0        0     1335 2023-07-09 07:25:01.000000 yaylib-1.0.9/tests/test_call.py
+-rw-rw-rw-   0        0        0     1935 2023-07-09 07:25:01.000000 yaylib-1.0.9/tests/test_cassandra.py
+-rw-rw-rw-   0        0        0     1335 2023-07-09 07:25:01.000000 yaylib-1.0.9/tests/test_chat.py
+-rw-rw-rw-   0        0        0     1337 2023-07-09 07:25:01.000000 yaylib-1.0.9/tests/test_group.py
+-rw-rw-rw-   0        0        0     1335 2023-07-09 07:25:01.000000 yaylib-1.0.9/tests/test_misc.py
+-rw-rw-rw-   0        0        0     3723 2023-07-09 07:25:01.000000 yaylib-1.0.9/tests/test_post.py
+-rw-rw-rw-   0        0        0     2028 2023-07-09 07:25:01.000000 yaylib-1.0.9/tests/test_review.py
+-rw-rw-rw-   0        0        0     1339 2023-07-09 07:25:01.000000 yaylib-1.0.9/tests/test_thread.py
+-rw-rw-rw-   0        0        0     1335 2023-07-09 07:25:01.000000 yaylib-1.0.9/tests/test_user.py
+-rw-rw-rw-   0        0        0     1908 2023-08-03 05:52:33.000000 yaylib-1.0.9/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-08-06 09:06:43.086952 yaylib-1.0.9/yaylib/
+-rw-rw-rw-   0        0        0      668 2023-08-04 08:28:13.000000 yaylib-1.0.9/yaylib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-06 09:06:43.109922 yaylib-1.0.9/yaylib/api/
+-rw-rw-rw-   0        0        0      962 2023-08-06 00:16:10.000000 yaylib-1.0.9/yaylib/api/__init__.py
+-rw-rw-rw-   0        0        0    15177 2023-08-06 08:47:39.000000 yaylib-1.0.9/yaylib/api/api.py
+-rw-rw-rw-   0        0        0     9429 2023-08-03 05:52:33.000000 yaylib-1.0.9/yaylib/api/call.py
+-rw-rw-rw-   0        0        0     2713 2023-08-03 05:52:33.000000 yaylib-1.0.9/yaylib/api/cassandra.py
+-rw-rw-rw-   0        0        0    14964 2023-08-03 05:52:33.000000 yaylib-1.0.9/yaylib/api/chat.py
+-rw-rw-rw-   0        0        0    23518 2023-08-06 00:16:10.000000 yaylib-1.0.9/yaylib/api/group.py
+-rw-rw-rw-   0        0        0     8090 2023-08-06 00:16:10.000000 yaylib-1.0.9/yaylib/api/login.py
+-rw-rw-rw-   0        0        0     7206 2023-08-06 00:16:10.000000 yaylib-1.0.9/yaylib/api/misc.py
+-rw-rw-rw-   0        0        0    33647 2023-08-03 05:52:33.000000 yaylib-1.0.9/yaylib/api/post.py
+-rw-rw-rw-   0        0        0     4445 2023-08-03 05:52:33.000000 yaylib-1.0.9/yaylib/api/review.py
+-rw-rw-rw-   0        0        0     5945 2023-07-18 08:52:45.000000 yaylib-1.0.9/yaylib/api/thread.py
+-rw-rw-rw-   0        0        0    23680 2023-08-06 08:59:07.000000 yaylib-1.0.9/yaylib/api/user.py
+-rw-rw-rw-   0        0        0     9409 2023-08-03 05:52:33.000000 yaylib-1.0.9/yaylib/api/websocket.py
+-rw-rw-rw-   0        0        0    86683 2023-08-06 08:59:01.000000 yaylib-1.0.9/yaylib/client.py
+-rw-rw-rw-   0        0        0    19024 2023-08-06 09:03:50.000000 yaylib-1.0.9/yaylib/config.py
+-rw-rw-rw-   0        0        0     2131 2023-07-18 08:52:45.000000 yaylib-1.0.9/yaylib/errors.py
+-rw-rw-rw-   0        0        0    55668 2023-08-06 00:16:10.000000 yaylib-1.0.9/yaylib/models.py
+-rw-rw-rw-   0        0        0    34186 2023-08-06 00:16:10.000000 yaylib-1.0.9/yaylib/responses.py
+-rw-rw-rw-   0        0        0     1643 2023-08-03 05:52:33.000000 yaylib-1.0.9/yaylib/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-06 09:06:43.098359 yaylib-1.0.9/yaylib.egg-info/
+-rw-rw-rw-   0        0        0    12869 2023-08-06 09:06:43.000000 yaylib-1.0.9/yaylib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      799 2023-08-06 09:06:43.000000 yaylib-1.0.9/yaylib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-06 09:06:43.000000 yaylib-1.0.9/yaylib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-08-06 09:06:43.000000 yaylib-1.0.9/yaylib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-08-06 09:06:43.000000 yaylib-1.0.9/yaylib.egg-info/top_level.txt
```

### Comparing `yaylib-1.0.8/LICENSE` & `yaylib-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.8/PKG-INFO` & `yaylib-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaylib
-Version: 1.0.8
+Version: 1.0.9
 Summary: 同世代と趣味の通話コミュニティ - Yay! (イェイ) で、投稿やタイムラインの取得、リツイートやいいねの実行、フォローや投稿の検索など様々な機能を利用可能なAPIクライアントツールです。
 Home-page: https://github.com/qvco/yaylib
 Download-URL: https://github.com/qvco/yaylib
 Author: Qvco, Konn
 Author-email: nikola.desuga@gmail.com
 Maintainer: Qvco, Konn
 Maintainer-email: nikola.desuga@gmail.com
@@ -27,15 +27,15 @@
 <br />
 <p align="center">
     <a href="https://github.com/othneildrew/Best-README-Template">
         <img src="https://github.com/qvco/yaylib/assets/77382767/45c45b21-d812-4cad-8f27-315ffef53201" alt="Logo" height="300px">
     </a>
     <h3 align="center">yaylib</h3>
     <p align="center">
-        「<strong>yaylib</strong>」は同世代でつながるチャットアプリ、Yay!（イェイ）の API ラッパーです。<br />
+        同世代でつながるチャットアプリ、Yay!（イェイ）の API ラッパーです。<br />
         あらゆる操作の自動化や、ボットの開発が可能です。
         <br />
         <br />
         <a href="https://github.com/qvco/yaylib/blob/master/docs/README.md">
             <strong>ドキュメントはこちらから »</strong>
         </a>
         <br />
@@ -335,15 +335,15 @@
 
 <a href="https://www.buymeacoffee.com/qvco" target="_blank"><img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" alt="Buy Me A Coffee" style="height: auto !important;width: auto !important;" ></a>
 
 <!-- 免責事項 -->
 
 ## 免責事項
 
-yaylib は、API の公式なサポートやメンテナンスを提供するものではありません。このクライアントを使用する場合、利用者は**リスクや責任を自己負担**できるものとします。このクライアントによって提供される情報やデータの正確性、信頼性、完全性、適時性について、いかなる保証も行いません。また、このクライアントの使用によって生じた損害や不利益について、一切の責任を負いかねます。利用者は自己の責任において、このクライアントを使用し、API にアクセスするものとします。なお、この免責事項は予告なく変更される場合があります。
+yaylib は、API の公式なサポートやメンテナンスを提供するものではありません。このクライアントを使用する場合、**利用者はリスクや責任を自己負担できるもの**とします。このクライアントによって提供される情報やデータの正確性、信頼性、完全性、適時性について、いかなる保証も行いません。また、このクライアントの使用によって生じた損害や不利益について、一切の責任を負いかねます。利用者は自己の責任において、このクライアントを使用し、API にアクセスするものとします。なお、この免責事項は予告なく変更される場合があります。
 
 <!-- ライセンス -->
 
 ## ライセンス
 
 <p align="center">
   <a href="https://github.com/qvco">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: yaylib Version: 1.0.8 Summary:
+Metadata-Version: 2.1 Name: yaylib Version: 1.0.9 Summary:
 åä¸ä»£ã¨è¶£å³ã®éè©±ã³ãã¥ããã£ - Yay! (ã¤ã§ã¤)
 ã§ãæç¨¿ãã¿ã¤ã ã©ã¤ã³ã®åå¾ããªãã¤ã¼ããããã­ã®å®è¡ããã©ã­ã¼ãæç¨¿ã®æ¤ç´¢ãªã©æ§ããªæ©è½ãå©ç¨å¯è½ãªAPIã¯ã©ã¤ã¢ã³ããã¼ã«ã§ãã
 Home-page: https://github.com/qvco/yaylib Download-URL: https://github.com/
 qvco/yaylib Author: Qvco, Konn Author-email: nikola.desuga@gmail.com
 Maintainer: Qvco, Konn Maintainer-email: nikola.desuga@gmail.com License: MIT
 Keywords:
 yay,yaylib,api,bot,tool,client,library,wrapper,ããã,ã©ã¤ãã©ãª,ãã¼ã«
@@ -15,16 +15,16 @@
  yaylib?style=for-the-badge&logo=appveyor&color=blue] [https://img.shields.io/
                    github/issues/qvco/yaylib?style=for-the-
 badge&logo=appveyor&color=informational] [https://img.shields.io/github/issues-
      pr/qvco/yaylib?style=for-the-badge&logo=appveyor&color=informational]
 
                                     [Logo]
                                **** yaylib ****
-ãyaylibãã¯åä¸ä»£ã§ã¤ãªãããã£ããã¢ããªãYay!ï¼ã¤ã§ã¤ï¼ã®
-                           API ã©ããã¼ã§ãã
+  åä¸ä»£ã§ã¤ãªãããã£ããã¢ããªãYay!ï¼ã¤ã§ã¤ï¼ã® API
+                             ã©ããã¼ã§ãã
    ããããæä½ã®èªååãããããã®éçºãå¯è½ã§ãã
 
                    ãã­ã¥ã¡ã³ãã¯ãã¡ããã_Â»
 
                Report_Bug Â· Request_Feature Â· Join_the_discord
   Table of Contents
    1. ã¤ã³ã¹ãã¼ã«
@@ -105,15 +105,15 @@
 ã®ããããã®æ¹æ³ã§ç¹ããã¾ããããè©³ããã¯
 [ãã¡ããã](https://github.com/qvco/yaylib/blob/master/
 CONTRIBUTING.md)ï¼  ## Buy me a coffee
 ãã®ã©ã¤ãã©ãªãæ°ã«å¥ã£ã¦ããã ãããã**ãªãã¸ããªã«ã¹ã¿ã¼ããé¡ããã¾ã
 (â­)** ã¾ããBuy Me a Coffee
 ãããæ¯æ´ããã ãã¾ãã¨å¹¸ãã§ãã [Buy_Me_A_Coffee]  ##
 åè²¬äºé  yaylib ã¯ãAPI
-ã®å¬å¼ãªãµãã¼ããã¡ã³ããã³ã¹ãæä¾ãããã®ã§ã¯ããã¾ããããã®ã¯ã©ã¤ã¢ã³ããä½¿ç¨ããå ´åãå©ç¨èã¯**ãªã¹ã¯ãè²¬ä»»ãèªå·±è² æ**ã§ãããã®ã¨ãã¾ãããã®ã¯ã©ã¤ã¢ã³ãã«ãã£ã¦æä¾ãããæå ±ããã¼ã¿ã®æ­£ç¢ºæ§ãä¿¡é ¼æ§ãå®å¨æ§ãé©ææ§ã«ã¤ãã¦ããããªãä¿è¨¼ãè¡ãã¾ãããã¾ãããã®ã¯ã©ã¤ã¢ã³ãã®ä½¿ç¨ã«ãã£ã¦çããæå®³ãä¸å©çã«ã¤ãã¦ãä¸åã®è²¬ä»»ãè² ããã­ã¾ããå©ç¨èã¯èªå·±ã®è²¬ä»»ã«ããã¦ããã®ã¯ã©ã¤ã¢ã³ããä½¿ç¨ããAPI
+ã®å¬å¼ãªãµãã¼ããã¡ã³ããã³ã¹ãæä¾ãããã®ã§ã¯ããã¾ããããã®ã¯ã©ã¤ã¢ã³ããä½¿ç¨ããå ´åã**å©ç¨èã¯ãªã¹ã¯ãè²¬ä»»ãèªå·±è² æã§ãããã®**ã¨ãã¾ãããã®ã¯ã©ã¤ã¢ã³ãã«ãã£ã¦æä¾ãããæå ±ããã¼ã¿ã®æ­£ç¢ºæ§ãä¿¡é ¼æ§ãå®å¨æ§ãé©ææ§ã«ã¤ãã¦ããããªãä¿è¨¼ãè¡ãã¾ãããã¾ãããã®ã¯ã©ã¤ã¢ã³ãã®ä½¿ç¨ã«ãã£ã¦çããæå®³ãä¸å©çã«ã¤ãã¦ãä¸åã®è²¬ä»»ãè² ããã­ã¾ããå©ç¨èã¯èªå·±ã®è²¬ä»»ã«ããã¦ããã®ã¯ã©ã¤ã¢ã³ããä½¿ç¨ããAPI
 ã«ã¢ã¯ã»ã¹ãããã®ã¨ãã¾ãããªãããã®åè²¬äºé ã¯äºåãªãå¤æ´ãããå ´åãããã¾ãã
 ## ã©ã¤ã»ã³ã¹
    [https://github.com/qvco/yaylib/assets/77382767/5d6aef18-5d98-4c9b-9f54-
                                  791308b393af]
                               MIT Â© Qvco & Konn
 ãã«ã©ã¤ã»ã³ã¹ã¯ [ãã¡ã](https://github.com/qvco/yaylib/blob/
 master/LICENSE) ãããç¢ºèªããã ãã¾ãã
```

### Comparing `yaylib-1.0.8/README.md` & `yaylib-1.0.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 <br />
 <p align="center">
     <a href="https://github.com/othneildrew/Best-README-Template">
         <img src="https://github.com/qvco/yaylib/assets/77382767/45c45b21-d812-4cad-8f27-315ffef53201" alt="Logo" height="300px">
     </a>
     <h3 align="center">yaylib</h3>
     <p align="center">
-        「<strong>yaylib</strong>」は同世代でつながるチャットアプリ、Yay!（イェイ）の API ラッパーです。<br />
+        同世代でつながるチャットアプリ、Yay!（イェイ）の API ラッパーです。<br />
         あらゆる操作の自動化や、ボットの開発が可能です。
         <br />
         <br />
         <a href="https://github.com/qvco/yaylib/blob/master/docs/README.md">
             <strong>ドキュメントはこちらから »</strong>
         </a>
         <br />
@@ -316,15 +316,15 @@
 
 <a href="https://www.buymeacoffee.com/qvco" target="_blank"><img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" alt="Buy Me A Coffee" style="height: auto !important;width: auto !important;" ></a>
 
 <!-- 免責事項 -->
 
 ## 免責事項
 
-yaylib は、API の公式なサポートやメンテナンスを提供するものではありません。このクライアントを使用する場合、利用者は**リスクや責任を自己負担**できるものとします。このクライアントによって提供される情報やデータの正確性、信頼性、完全性、適時性について、いかなる保証も行いません。また、このクライアントの使用によって生じた損害や不利益について、一切の責任を負いかねます。利用者は自己の責任において、このクライアントを使用し、API にアクセスするものとします。なお、この免責事項は予告なく変更される場合があります。
+yaylib は、API の公式なサポートやメンテナンスを提供するものではありません。このクライアントを使用する場合、**利用者はリスクや責任を自己負担できるもの**とします。このクライアントによって提供される情報やデータの正確性、信頼性、完全性、適時性について、いかなる保証も行いません。また、このクライアントの使用によって生じた損害や不利益について、一切の責任を負いかねます。利用者は自己の責任において、このクライアントを使用し、API にアクセスするものとします。なお、この免責事項は予告なく変更される場合があります。
 
 <!-- ライセンス -->
 
 ## ライセンス
 
 <p align="center">
   <a href="https://github.com/qvco">
```

#### html2text {}

```diff
@@ -3,16 +3,16 @@
  yaylib?style=for-the-badge&logo=appveyor&color=blue] [https://img.shields.io/
                    github/issues/qvco/yaylib?style=for-the-
 badge&logo=appveyor&color=informational] [https://img.shields.io/github/issues-
      pr/qvco/yaylib?style=for-the-badge&logo=appveyor&color=informational]
 
                                     [Logo]
                                **** yaylib ****
-ãyaylibãã¯åä¸ä»£ã§ã¤ãªãããã£ããã¢ããªãYay!ï¼ã¤ã§ã¤ï¼ã®
-                           API ã©ããã¼ã§ãã
+  åä¸ä»£ã§ã¤ãªãããã£ããã¢ããªãYay!ï¼ã¤ã§ã¤ï¼ã® API
+                             ã©ããã¼ã§ãã
    ããããæä½ã®èªååãããããã®éçºãå¯è½ã§ãã
 
                    ãã­ã¥ã¡ã³ãã¯ãã¡ããã_Â»
 
                Report_Bug Â· Request_Feature Â· Join_the_discord
   Table of Contents
    1. ã¤ã³ã¹ãã¼ã«
@@ -93,15 +93,15 @@
 ã®ããããã®æ¹æ³ã§ç¹ããã¾ããããè©³ããã¯
 [ãã¡ããã](https://github.com/qvco/yaylib/blob/master/
 CONTRIBUTING.md)ï¼  ## Buy me a coffee
 ãã®ã©ã¤ãã©ãªãæ°ã«å¥ã£ã¦ããã ãããã**ãªãã¸ããªã«ã¹ã¿ã¼ããé¡ããã¾ã
 (â­)** ã¾ããBuy Me a Coffee
 ãããæ¯æ´ããã ãã¾ãã¨å¹¸ãã§ãã [Buy_Me_A_Coffee]  ##
 åè²¬äºé  yaylib ã¯ãAPI
-ã®å¬å¼ãªãµãã¼ããã¡ã³ããã³ã¹ãæä¾ãããã®ã§ã¯ããã¾ããããã®ã¯ã©ã¤ã¢ã³ããä½¿ç¨ããå ´åãå©ç¨èã¯**ãªã¹ã¯ãè²¬ä»»ãèªå·±è² æ**ã§ãããã®ã¨ãã¾ãããã®ã¯ã©ã¤ã¢ã³ãã«ãã£ã¦æä¾ãããæå ±ããã¼ã¿ã®æ­£ç¢ºæ§ãä¿¡é ¼æ§ãå®å¨æ§ãé©ææ§ã«ã¤ãã¦ããããªãä¿è¨¼ãè¡ãã¾ãããã¾ãããã®ã¯ã©ã¤ã¢ã³ãã®ä½¿ç¨ã«ãã£ã¦çããæå®³ãä¸å©çã«ã¤ãã¦ãä¸åã®è²¬ä»»ãè² ããã­ã¾ããå©ç¨èã¯èªå·±ã®è²¬ä»»ã«ããã¦ããã®ã¯ã©ã¤ã¢ã³ããä½¿ç¨ããAPI
+ã®å¬å¼ãªãµãã¼ããã¡ã³ããã³ã¹ãæä¾ãããã®ã§ã¯ããã¾ããããã®ã¯ã©ã¤ã¢ã³ããä½¿ç¨ããå ´åã**å©ç¨èã¯ãªã¹ã¯ãè²¬ä»»ãèªå·±è² æã§ãããã®**ã¨ãã¾ãããã®ã¯ã©ã¤ã¢ã³ãã«ãã£ã¦æä¾ãããæå ±ããã¼ã¿ã®æ­£ç¢ºæ§ãä¿¡é ¼æ§ãå®å¨æ§ãé©ææ§ã«ã¤ãã¦ããããªãä¿è¨¼ãè¡ãã¾ãããã¾ãããã®ã¯ã©ã¤ã¢ã³ãã®ä½¿ç¨ã«ãã£ã¦çããæå®³ãä¸å©çã«ã¤ãã¦ãä¸åã®è²¬ä»»ãè² ããã­ã¾ããå©ç¨èã¯èªå·±ã®è²¬ä»»ã«ããã¦ããã®ã¯ã©ã¤ã¢ã³ããä½¿ç¨ããAPI
 ã«ã¢ã¯ã»ã¹ãããã®ã¨ãã¾ãããªãããã®åè²¬äºé ã¯äºåãªãå¤æ´ãããå ´åãããã¾ãã
 ## ã©ã¤ã»ã³ã¹
    [https://github.com/qvco/yaylib/assets/77382767/5d6aef18-5d98-4c9b-9f54-
                                  791308b393af]
                               MIT Â© Qvco & Konn
 ãã«ã©ã¤ã»ã³ã¹ã¯ [ãã¡ã](https://github.com/qvco/yaylib/blob/
 master/LICENSE) ãããç¢ºèªããã ãã¾ãã
```

### Comparing `yaylib-1.0.8/setup.py` & `yaylib-1.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.8/tests/config.py` & `yaylib-1.0.9/tests/config.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.8/tests/test_call.py` & `yaylib-1.0.9/tests/test_call.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.8/tests/test_cassandra.py` & `yaylib-1.0.9/tests/test_cassandra.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.8/tests/test_chat.py` & `yaylib-1.0.9/tests/test_chat.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.8/tests/test_group.py` & `yaylib-1.0.9/tests/test_group.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.8/tests/test_misc.py` & `yaylib-1.0.9/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.8/tests/test_post.py` & `yaylib-1.0.9/tests/test_post.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.8/tests/test_review.py` & `yaylib-1.0.9/tests/test_review.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.8/tests/test_thread.py` & `yaylib-1.0.9/tests/test_thread.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.8/tests/test_user.py` & `yaylib-1.0.9/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.8/tests/test_utils.py` & `yaylib-1.0.9/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.8/yaylib/__init__.py` & `yaylib-1.0.9/yaylib/__init__.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.8/yaylib/api/api.py` & `yaylib-1.0.9/yaylib/api/api.py`

 * *Files 9% similar despite different names*

```diff
@@ -40,15 +40,14 @@
     AuthenticationError,
     ForbiddenError,
     NotFoundError,
     RateLimitError,
     YayServerError,
 )
 
-
 try:
     from json.decoder import JSONDecodeError
 except ImportError:
     JSONDecodeError = ValueError
 
 
 current_path = os.path.abspath(os.getcwd())
@@ -72,16 +71,16 @@
         self.api_version = Configs.YAY_API_VERSION
         self.api_key = Configs.YAY_API_KEY
         self.fernet = None
         self._secret_key = None
 
         self.proxy = {}
         if proxy is not None:
-            self.proxy["http"] = proxy
-            self.proxy["https"] = proxy
+            self.proxy["http://"] = proxy
+            self.proxy["https://"] = proxy
 
         self.max_retries = max_retries
         self.retry_statuses = [500, 502, 503, 504]
         self.backoff_factor = backoff_factor
         self.timeout = timeout
         self.err_lang = err_lang
         self.base_path = base_path
@@ -89,26 +88,28 @@
         self.cookie_filename = cookie_filename
         self._cookies = {}
 
         self._generate_all_uuids()
         self.session = httpx.Client(proxies=self.proxy, timeout=self.timeout)
         self.session.headers.update(Configs.REQUEST_HEADERS)
         self.session.headers.update({"X-Device-Uuid": self.device_uuid})
-        if access_token:
+        if access_token is not None:
             self.session.headers.setdefault("Authorization", f"Bearer {access_token}")
 
         self.logger = logging.getLogger("yaylib version: " + self.yaylib_version)
 
         if not os.path.exists(base_path):
             os.makedirs(base_path)
 
         ch = logging.StreamHandler()
         ch.setLevel(loglevel)
         ch.setFormatter(logging.Formatter("%(asctime)s - %(levelname)s - %(message)s"))
 
+        # check if a stream handler is already present in the logger
+        # to avoid adding duplicate handlers
         handler_existed = False
         for handler in self.logger.handlers:
             if isinstance(handler, logging.StreamHandler):
                 handler_existed = True
                 break
         if not handler_existed:
             self.logger.addHandler(ch)
@@ -135,14 +136,15 @@
             del headers["Authorization"]
 
         response = None
         backoff_duration = 0
         auth_retry_count = 0
         max_auth_retries = 2
 
+        # retry the request based on max_retries
         for i in range(self.max_retries):
             time.sleep(backoff_duration)
 
             self.logger.debug(
                 "Making API request:\n\n"
                 f"{method}: {endpoint}\n\n"
                 f"Parameters: {params}\n\n"
@@ -151,22 +153,26 @@
             )
 
             response = self.session.request(
                 method, endpoint, params=params, json=payload, headers=headers
             )
 
             if self.save_cookie_file is True and response.status_code == 401:
+                # remove the cookie file and stop the proccessing if refresh token has expired
+                # (/api/v1/oauth/token in the endpoint which means already retried but failed)
                 if "/api/v1/oauth/token" in endpoint:
                     os.remove(self.base_path + self.cookie_filename + ".json")
-                    message = "Refresh token expired. Try logging in again."
-                    raise AuthenticationError(message)
+                    raise AuthenticationError(
+                        "Refresh token expired. Try logging in again."
+                    )
 
                 auth_retry_count += 1
 
                 if auth_retry_count < max_auth_retries:
+                    # refresh access token using the stored refresh token
                     self.logger.debug("Access token expired. Refreshing tokens...")
 
                     cookies = self.load_cookies()
 
                     if cookies is not None and self.fernet is not None:
                         cookies = self.decrypt_cookies(self.fernet, cookies)
                         response = get_token(
@@ -177,30 +183,28 @@
                         self._cookies.update(
                             {
                                 "access_token": response.access_token,
                                 "refresh_token": response.refresh_token,
                                 "user_id": response.user_id,
                             }
                         )
-                        self.save_cookies(
-                            access_token=response.access_token,
-                            refresh_token=response.refresh_token,
-                            user_id=response.user_id,
-                        )
+                        self.save_cookies(self.cookies)
+
                         self.session.headers[
                             "Authorization"
                         ] = f"Bearer {response.access_token}"
+
+                        # continue to the next retry iteration
                         continue
 
                 else:
                     os.remove(self.base_path + self.cookie_filename + ".json")
-                    message = (
+                    raise AuthenticationError(
                         "Maximum authentication retries exceeded. Try logging in again."
                     )
-                    raise AuthenticationError(message)
 
             if response.status_code not in self.retry_statuses:
                 break
 
             if response is not None:
                 self.logger.error(
                     f"Request failed with status code {response.status_code}. Retrying...",
@@ -340,37 +344,38 @@
             return None
 
         with open(self.base_path + self.cookie_filename + ".json", "r") as f:
             cookies = json.load(f)
 
         result = all(key in cookies for key in Configs.COOKIE_PROPERTIES)
         if result is False:
-            raise ValueError("Invalid cookies.")
+            os.remove(self.base_path + self.cookie_filename + ".json")
+            raise ValueError("Invalid cookie properties.")
 
+        # check if the provided email matches the stored email in cookies
+        # if not, set cookies to none
         if email is not None and email != cookies.get("email"):
             cookies = None if email != cookies.get("email") else cookies
         if self.fernet is not None and cookies is not None:
             cookies = self.decrypt_cookies(self.fernet, cookies)
+
         return cookies
 
-    def save_cookies(self, access_token, refresh_token, user_id, email=None):
-        updated_cookies = {
-            "access_token": access_token,
-            "refresh_token": refresh_token,
-            "user_id": user_id,
-            "email": email,
-        }
+    def save_cookies(self, cookies):
+        if cookies.get("email") is None:
+            cookies["email"] = self.load_cookies().get("email")
 
-        if email is None:
-            updated_cookies["email"] = self.load_cookies().get("email")
+        result = all(key in cookies for key in Configs.COOKIE_PROPERTIES)
+        if result is False:
+            raise ValueError("Invalid cookie properties.")
 
-        updated_cookies = self.encrypt_cookies(self.fernet, updated_cookies)
+        cookies = self.encrypt_cookies(self.fernet, cookies)
 
         with open(self.base_path + self.cookie_filename + ".json", "w") as f:
-            json.dump(updated_cookies, f, indent=4)
+            json.dump(cookies, f, indent=4)
 
     @staticmethod
     def _construct_response(data, data_type):
         if data_type is not None:
             if isinstance(data, list):
                 data = [data_type(result) for result in data]
             elif data is not None:
@@ -396,14 +401,15 @@
             raise NotFoundError(formatted_response)
         if response.status_code == 429:
             raise RateLimitError(formatted_response)
         if response.status_code == 500:
             raise YayServerError(formatted_response)
         if response.status_code and not 200 <= response.status_code < 300:
             raise HTTPError(formatted_response)
+
         return formatted_response
 
     def _translate_error_message(self, response):
         if self.err_lang == "ja":
             try:
                 error_code = response.get("error_code", None)
                 if error_code is not None:
```

### Comparing `yaylib-1.0.8/yaylib/api/call.py` & `yaylib-1.0.9/yaylib/api/call.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.8/yaylib/api/cassandra.py` & `yaylib-1.0.9/yaylib/api/cassandra.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.8/yaylib/api/chat.py` & `yaylib-1.0.9/yaylib/api/chat.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.8/yaylib/api/group.py` & `yaylib-1.0.9/yaylib/api/group.py`

 * *Files 1% similar despite different names*

```diff
@@ -675,15 +675,15 @@
     cover_image_filename: str = None,
     sub_category_id: str = None,
     hide_from_game_eight: bool = None,
     allow_members_to_post_media: bool = None,
     allow_members_to_post_url: bool = None,
     guidelines: str = None,
     access_token: str = None,
-) -> GroupResponse:
+) -> Group:
     self._check_authorization(access_token)
     timestamp = int(datetime.now().timestamp())
     response = self._make_request(
         "POST",
         endpoint=f"{Endpoints.GROUPS_V3}/{group_id}/update",
         payload={
             "topic": topic,
@@ -709,15 +709,15 @@
             "hide_from_game_eight": hide_from_game_eight,
             "allow_members_to_post_image_and_video": allow_members_to_post_media,
             "allow_members_to_post_url": allow_members_to_post_url,
             "guidelines": guidelines,
         },
         data_type=GroupResponse,
         access_token=access_token,
-    )
+    ).group
     self.logger.info("Group details have been updated.")
     return response
 
 
 def withdraw_moderator_offer(
     self, group_id: int, user_id: int, access_token: str = None
 ):
```

### Comparing `yaylib-1.0.8/yaylib/api/login.py` & `yaylib-1.0.9/yaylib/api/login.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,20 +156,15 @@
         self.cookies = {
             "access_token": response.access_token,
             "refresh_token": response.refresh_token,
             "user_id": response.user_id,
             "email": email,
         }
 
-        self.save_cookies(
-            access_token=response.access_token,
-            refresh_token=response.refresh_token,
-            user_id=response.user_id,
-            email=email,
-        )
+        self.save_cookies(self.cookies)
 
     return response
 
 
 def logout(self, access_token: str = None):
     try:
         self._check_authorization(access_token)
```

### Comparing `yaylib-1.0.8/yaylib/api/misc.py` & `yaylib-1.0.9/yaylib/api/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -191,23 +191,18 @@
 ) -> str:
     """
 
     画像をアップロードしてattachment_filenameを返します。
 
     Parameteres
     -----------
-        - image_type: str - (required): "post", "user_avatar" のどちらか
+        - image_type: str - (required): 画像の種類
         - image_path: str - (required): "画像のパス
 
     """
-    valid_types = ["post", "user_avatar"]
-    if image_type not in valid_types:
-        message = f"Invalid post type. Must be one of {valid_types}"
-        raise ValueError(message)
-
     date = datetime.now()
     timestamp = int(date.timestamp() * 1000)
     filename, ext = os.path.splitext(image_path)
 
     with Image.open(image_path) as image:
         width, height = image.size
```

### Comparing `yaylib-1.0.8/yaylib/api/post.py` & `yaylib-1.0.9/yaylib/api/post.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.8/yaylib/api/review.py` & `yaylib-1.0.9/yaylib/api/review.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.8/yaylib/api/thread.py` & `yaylib-1.0.9/yaylib/api/thread.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.8/yaylib/api/user.py` & `yaylib-1.0.9/yaylib/api/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -428,15 +428,15 @@
         payload={"counter": counter},
         access_token=access_token,
     )
     self.logger.info("Requested counter refresh.")
     return response
 
 
-def register_user(
+def register(
     self,
     email: str,
     email_grant_token: str,
     password: str,
     nickname: str,
     birth_date: str,
     gender: int = -1,
```

### Comparing `yaylib-1.0.8/yaylib/api/websocket.py` & `yaylib-1.0.9/yaylib/api/websocket.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.8/yaylib/client.py` & `yaylib-1.0.9/yaylib/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -236,15 +236,15 @@
     get_user_email,
     get_user_followers,
     get_user_followings,
     get_user_from_qr,
     get_user_without_leaving_footprint,
     get_users,
     refresh_counter,
-    register_user,
+    register,
     remove_user_avatar,
     remove_user_cover,
     report_user,
     reset_password,
     search_lobi_users,
     search_users,
     set_follow_permission_enabled,
@@ -291,15 +291,14 @@
     CreateGroupResponse,
     CreateChatRoomResponse,
     FollowRecommendationsResponse,
     FollowUsersResponse,
     GamesResponse,
     GenresResponse,
     GroupCategoriesResponse,
-    GroupResponse,
     GroupsRelatedResponse,
     GroupsResponse,
     GroupThreadListResponse,
     GroupUserResponse,
     GroupUsersResponse,
     HiddenResponse,
     LoginUserResponse,
@@ -1473,15 +1472,15 @@
         cover_image_filename: str = None,
         sub_category_id: str = None,
         hide_from_game_eight: bool = None,
         allow_members_to_post_media: bool = None,
         allow_members_to_post_url: bool = None,
         guidelines: str = None,
         access_token: str = None,
-    ) -> GroupResponse:
+    ) -> Group:
         """
 
         サークルを編集します
 
         """
         return update_group(
             group_id,
@@ -1700,15 +1699,15 @@
     ) -> str:
         """
 
         画像をアップロードしてattachment_filenameを返します。
 
         Parameteres
         -----------
-            - image_type: str - (required): "post", "user_avatar" のどちらか
+            - image_type: str - (required): 画像の種類
             - image_path: str - (required): "画像のパス
 
         """
         return upload_image(self, image_type, image_path, access_token)
 
     # -POST
 
@@ -2949,15 +2948,15 @@
         """
 
         カウンターを更新します
 
         """
         return refresh_counter(self, counter, access_token)
 
-    def register_user(
+    def register(
         self,
         email: str,
         email_grant_token: str,
         password: str,
         nickname: str,
         birth_date: str,
         gender: int = -1,
@@ -2971,15 +2970,15 @@
         vn: int = None,
     ):
         """
 
         Register user
 
         """
-        return register_user(
+        return register(
             self,
             email,
             email_grant_token,
             password,
             nickname,
             birth_date,
             gender,
```

### Comparing `yaylib-1.0.8/yaylib/config.py` & `yaylib-1.0.9/yaylib/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 SOFTWARE.
 """
 
 from enum import Enum
 
 
 class Configs:
-    YAYLIB_VERSION = "1.0.8"
+    YAYLIB_VERSION = "1.0.9"
     YAY_API_VERSION = "3.21"
     YAY_VERSION_NAME = "3.21.0"
     YAY_API_VERSION_KEY = "c687e24f6a454896891acd68868c7979"
     YAY_API_KEY = "ccd59ee269c01511ba763467045c115779fcae3050238a252f1bd1a4b65cfec6"
     YAY_SHARED_KEY = "yayZ1"
     YAY_STORE_KEY = "yayZ1payment"
     AGORA_APP_ID = "79046b8c9be54945b7f10a4d128d5395"
@@ -242,14 +242,15 @@
     GroupInviteExceeded = -404
     PhoneVerificationRequired = -405
     ContentTooOld = -406
     PasswordTooShort = -407
     PasswordTooLong = -408
     PasswordNotAllowed = -409
     CommonPassword = -410
+    EmailNotAuthorized = -411
     UnableToMovePostToThread = -412
     UnableToPostUrl = -413
     UnableToSetCall = -977
     PhoneNumberBanned = -1000
     TooManyRequests = -5302
 
 
@@ -345,12 +346,13 @@
     GroupInviteExceeded = "サークルにおける招待の許容数を超えました。時間をあけてから再度行ってください。"
     PhoneVerificationRequired = "参加するには電話番号認証が必要です。Yay! アプリから電話番号認証を行なってください。"
     ContentTooOld = "一定期間の経過後、投稿の編集はできません"
     PasswordTooShort = "パスワードが短すぎます"
     PasswordTooLong = "パスワードが長すぎます"
     PasswordNotAllowed = "他のパスワードを使用してください。無効な文字列が含まれています"
     CommonPassword = "他のパスワードを使用してください。文字列や数字、または記号などの組み合わせをお試しください"
+    EmailNotAuthorized = "このメールアドレスを使用するには承認される必要があります"
     UnableToMovePostToThread = "投稿をスレッドに移動できません"
     UnableToPostUrl = "URLを投稿できません"
     UnableToSetCall = "通話を開始できませんでした"
     PhoneNumberBanned = "電話番号がBanされています"
     TooManyRequests = "リクエストが多すぎます"
```

### Comparing `yaylib-1.0.8/yaylib/errors.py` & `yaylib-1.0.9/yaylib/errors.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.8/yaylib/models.py` & `yaylib-1.0.9/yaylib/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -119,27 +119,26 @@
         self.order = data.get("order")
 
     def __repr__(self):
         return f"Bgm(data={self.data})"
 
 
 class CallGiftHistory:
-    __slots__ = ("data", "gifts_count", "sent_at", "sent_at_parsed", "sender")
+    __slots__ = ("data", "gifts_count", "sent_at", "sender")
 
     def __init__(self, data):
         self.data = data
 
         self.gifts_count = data.get("gifts_count")
         if self.gifts_count is not None:
             self.gifts_count = [
                 GiftCount(gifts_count) for gifts_count in self.gifts_count
             ]
 
         self.sent_at = data.get("sent_at")
-        self.sent_at_parsed = parse_datetime(data.get("sent_at"))
 
         self.sender = data.get("sender")
         if self.sender is not None:
             self.sender = User(self.sender)
 
     def __repr__(self):
         return f"CallGiftHistory(data={self.data})"
@@ -147,15 +146,14 @@
 
 class ChatRoom:
     __slots__ = (
         "data",
         "id",
         "unread_count",
         "updated_at",
-        "updated_at_parsed",
         "members",
         "background",
         "last_message",
         "name",
         "is_group",
         "owner",
         "is_request",
@@ -163,15 +161,14 @@
     )
 
     def __init__(self, data):
         self.data = data
         self.id = data.get("id")
         self.unread_count = data.get("unread_count")
         self.updated_at = data.get("updated_at")
-        self.updated_at_parsed = parse_datetime(data.get("updated_at"))
 
         self.members = data.get("members")
         if self.members is not None:
             self.members = [User(member) for member in self.members]
 
         self.background = data.get("background")
 
@@ -465,25 +462,24 @@
         self.action = data.get("action")
 
     def __repr__(self):
         return f"Error(data={self.data})"
 
 
 class Footprint:
-    __slots__ = ("data", "user", "visited_at", "visited_at_parsed", "id")
+    __slots__ = ("data", "user", "visited_at", "id")
 
     def __init__(self, data):
         self.data = data
 
         self.user = data.get("user")
         if self.user is not None:
             self.user = User(self.user)
 
         self.visited_at = data.get("visited_at")
-        self.visited_at_parsed = parse_datetime(data.get("visited_at"))
         self.id = data.get("id")
 
     def __repr__(self):
         return f"Footprint(data={self.data})"
 
 
 class Game:
@@ -938,17 +934,15 @@
         "post_type",
         "group_id",
         "font_size",
         "color",
         "likes_count",
         "created_at",
         "updated_at",
-        "updated_at_parsed",
         "edited_at",
-        "edited_at_parsed",
         "liked",
         "tag",
         "reposts_count",
         "reposted",
         "repostable",
         "reported_count",
         "conversation_id",
@@ -997,17 +991,15 @@
         self.post_type = data.get("post_type")
         self.group_id = data.get("group_id")
         self.font_size = data.get("font_size")
         self.color = data.get("color")
         self.likes_count = data.get("likes_count")
         self.created_at = data.get("created_at")
         self.updated_at = data.get("updated_at")
-        self.updated_at_parsed = parse_datetime(data.get("updated_at"))
         self.edited_at = data.get("edited_at")
-        self.edited_at_parsed = parse_datetime(data.get("edited_at"))
         self.liked = data.get("liked")
         self.tag = data.get("tag")
         self.reposts_count = data.get("reposts_count")
         self.reposted = data.get("reposted")
         self.repostable = data.get("repostable")
         self.reported_count = data.get("reported_count")
         self.conversation_id = data.get("conversation_id")
@@ -1212,15 +1204,14 @@
         "data",
         "id",
         "comment",
         "reported_count",
         "user",
         "reviewer",
         "created_at",
-        "created_at_parsed",
         "mutual_review",
     )
 
     def __init__(self, data):
         self.data = data
         self.id = data.get("id")
         self.comment = data.get("comment")
@@ -1228,15 +1219,14 @@
 
         self.user = data.get("user")
         if self.user is not None:
             self.user = User(self.user)
 
         self.reviewer = data.get("reviewer")
         self.created_at = data.get("created_at")
-        self.created_at_parsed = parse_datetime(data.get("created_at"))
         self.mutual_review = data.get("mutual_review")
 
     def __repr__(self):
         return f"Review(data={self.data})"
 
 
 class SearchCriteria:
@@ -1538,17 +1528,15 @@
         "id",
         "title",
         "owner",
         "last_post",
         "unread_count",
         "posts_count",
         "created_at",
-        "created_at_parsed",
         "updated_at",
-        "updated_at_parsed",
         "thread_icon",
         "is_joined",
         "new_updates",
     )
 
     def __init__(self, data):
         self.data = data
@@ -1562,17 +1550,15 @@
         self.last_post = data.get("last_post")
         if self.last_post is not None:
             self.last_post = Post(self.last_post)
 
         self.unread_count = data.get("unread_count")
         self.posts_count = data.get("posts_count")
         self.created_at = data.get("created_at")
-        self.created_at_parsed = parse_datetime(data.get("created_at"))
         self.updated_at = data.get("updated_at")
-        self.updated_at_parsed = parse_datetime(data.get("updated_at"))
         self.thread_icon = data.get("thread_icon")
         self.is_joined = data.get("is_joined")
         self.new_updates = data.get("new_updates")
 
     def __repr__(self):
         return f"ThreadInfo(data={self.data})"
 
@@ -1585,17 +1571,15 @@
         "id",
         "nickname",
         "prefecture",
         "biography",
         "gender",
         "generation",
         "last_logged_in_at",
-        "last_logged_in_at_parsed",
         "created_at",
-        "created_at_parsed",
         "badge",
         "followers_count",
         "followings_count",
         "posts_count",
         "groups_users_count",
         "reviews_count",
         "login_streak_count",
@@ -1621,29 +1605,26 @@
         "is_following",
         "is_followed_by",
         "is_follow_pending",
         "is_hidden",
         "connected_by",
         "contact_phones",
         "updated_time_millis",
-        "updated_time_millis_parsed",
     )
 
     def __init__(self, data):
         self.data = data
         self.id = data.get("id")
         self.nickname = data.get("nickname")
         self.prefecture = data.get("prefecture")
         self.biography = data.get("biography")
         self.gender = data.get("gender")
         self.generation = data.get("generation")
         self.last_logged_in_at = data.get("last_logged_in_at")
-        self.last_logged_in_at_parsed = parse_datetime(data.get("last_logged_in_at"))
         self.created_at = data.get("created_at")
-        self.created_at_parsed = parse_datetime(data.get("created_at"))
         self.badge = data.get("title")
         self.followers_count = data.get("followers_count")
         self.followings_count = data.get("followings_count")
         self.posts_count = data.get("posts_count")
         self.groups_users_count = data.get("groups_users_count")
         self.reviews_count = data.get("reviews_count")
         self.login_streak_count = data.get("login_streak_count")
@@ -1675,17 +1656,14 @@
         self.is_following = data.get("following")
         self.is_followed_by = data.get("followed_by")
         self.is_follow_pending = data.get("follow_pending")
         self.is_hidden = data.get("hidden")
         self.connected_by = data.get("connected_by")
         self.contact_phones = data.get("contact_phones")
         self.updated_time_millis = data.get("updated_time_millis")
-        self.updated_time_millis_parsed = parse_datetime(
-            data.get("updated_time_millis")
-        )
 
     def __repr__(self):
         return f"User(data={self.data})"
 
 
 class UserAuth:
     __slots__ = ("data", "user_id", "access_token", "refresh_token", "expires_in")
@@ -1765,15 +1743,14 @@
 class WalletTransaction:
     __slots__ = ("data", "id", "created_at", "description", "amount", "coins")
 
     def __init__(self, data):
         self.data = data
         self.id = data.get("id")
         self.created_at = data.get("created_at")
-        self.created_at_parsed = parse_datetime(data.get("created_at"))
         self.description = data.get("description")
         self.amount = data.get("amount")
 
         self.coins = data.get("coins")
         if self.coins is not None:
             self.coins = CoinAmount(self.coins)
```

### Comparing `yaylib-1.0.8/yaylib/responses.py` & `yaylib-1.0.9/yaylib/responses.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,25 +101,24 @@
             self.users = [User(user) for user in self.users]
 
     def __repr__(self):
         return f"ActiveFollowingsResponse(data={self.data})"
 
 
 class ActivitiesResponse:
-    __slots__ = ("data", "activities", "last_timestamp", "parsed_last_timestamp")
+    __slots__ = ("data", "activities", "last_timestamp")
 
     def __init__(self, data):
         self.data = data
 
         self.activities = data.get("activities")
         if self.activities is not None:
             self.activities = [Activity(activity) for activity in self.activities]
 
         self.last_timestamp = data.get("last_timestamp")
-        self.parsed_last_timestamp = parse_datetime(data.get("last_timestamp"))
 
     def __repr__(self):
         return f"ActivitiesResponse(data={self.data})"
 
 
 class AdditionalSettingsResponse:
     __slots__ = ("data", "settings")
```

### Comparing `yaylib-1.0.8/yaylib/utils.py` & `yaylib-1.0.9/yaylib/utils.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.8/yaylib.egg-info/PKG-INFO` & `yaylib-1.0.9/yaylib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaylib
-Version: 1.0.8
+Version: 1.0.9
 Summary: 同世代と趣味の通話コミュニティ - Yay! (イェイ) で、投稿やタイムラインの取得、リツイートやいいねの実行、フォローや投稿の検索など様々な機能を利用可能なAPIクライアントツールです。
 Home-page: https://github.com/qvco/yaylib
 Download-URL: https://github.com/qvco/yaylib
 Author: Qvco, Konn
 Author-email: nikola.desuga@gmail.com
 Maintainer: Qvco, Konn
 Maintainer-email: nikola.desuga@gmail.com
@@ -27,15 +27,15 @@
 <br />
 <p align="center">
     <a href="https://github.com/othneildrew/Best-README-Template">
         <img src="https://github.com/qvco/yaylib/assets/77382767/45c45b21-d812-4cad-8f27-315ffef53201" alt="Logo" height="300px">
     </a>
     <h3 align="center">yaylib</h3>
     <p align="center">
-        「<strong>yaylib</strong>」は同世代でつながるチャットアプリ、Yay!（イェイ）の API ラッパーです。<br />
+        同世代でつながるチャットアプリ、Yay!（イェイ）の API ラッパーです。<br />
         あらゆる操作の自動化や、ボットの開発が可能です。
         <br />
         <br />
         <a href="https://github.com/qvco/yaylib/blob/master/docs/README.md">
             <strong>ドキュメントはこちらから »</strong>
         </a>
         <br />
@@ -335,15 +335,15 @@
 
 <a href="https://www.buymeacoffee.com/qvco" target="_blank"><img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" alt="Buy Me A Coffee" style="height: auto !important;width: auto !important;" ></a>
 
 <!-- 免責事項 -->
 
 ## 免責事項
 
-yaylib は、API の公式なサポートやメンテナンスを提供するものではありません。このクライアントを使用する場合、利用者は**リスクや責任を自己負担**できるものとします。このクライアントによって提供される情報やデータの正確性、信頼性、完全性、適時性について、いかなる保証も行いません。また、このクライアントの使用によって生じた損害や不利益について、一切の責任を負いかねます。利用者は自己の責任において、このクライアントを使用し、API にアクセスするものとします。なお、この免責事項は予告なく変更される場合があります。
+yaylib は、API の公式なサポートやメンテナンスを提供するものではありません。このクライアントを使用する場合、**利用者はリスクや責任を自己負担できるもの**とします。このクライアントによって提供される情報やデータの正確性、信頼性、完全性、適時性について、いかなる保証も行いません。また、このクライアントの使用によって生じた損害や不利益について、一切の責任を負いかねます。利用者は自己の責任において、このクライアントを使用し、API にアクセスするものとします。なお、この免責事項は予告なく変更される場合があります。
 
 <!-- ライセンス -->
 
 ## ライセンス
 
 <p align="center">
   <a href="https://github.com/qvco">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: yaylib Version: 1.0.8 Summary:
+Metadata-Version: 2.1 Name: yaylib Version: 1.0.9 Summary:
 åä¸ä»£ã¨è¶£å³ã®éè©±ã³ãã¥ããã£ - Yay! (ã¤ã§ã¤)
 ã§ãæç¨¿ãã¿ã¤ã ã©ã¤ã³ã®åå¾ããªãã¤ã¼ããããã­ã®å®è¡ããã©ã­ã¼ãæç¨¿ã®æ¤ç´¢ãªã©æ§ããªæ©è½ãå©ç¨å¯è½ãªAPIã¯ã©ã¤ã¢ã³ããã¼ã«ã§ãã
 Home-page: https://github.com/qvco/yaylib Download-URL: https://github.com/
 qvco/yaylib Author: Qvco, Konn Author-email: nikola.desuga@gmail.com
 Maintainer: Qvco, Konn Maintainer-email: nikola.desuga@gmail.com License: MIT
 Keywords:
 yay,yaylib,api,bot,tool,client,library,wrapper,ããã,ã©ã¤ãã©ãª,ãã¼ã«
@@ -15,16 +15,16 @@
  yaylib?style=for-the-badge&logo=appveyor&color=blue] [https://img.shields.io/
                    github/issues/qvco/yaylib?style=for-the-
 badge&logo=appveyor&color=informational] [https://img.shields.io/github/issues-
      pr/qvco/yaylib?style=for-the-badge&logo=appveyor&color=informational]
 
                                     [Logo]
                                **** yaylib ****
-ãyaylibãã¯åä¸ä»£ã§ã¤ãªãããã£ããã¢ããªãYay!ï¼ã¤ã§ã¤ï¼ã®
-                           API ã©ããã¼ã§ãã
+  åä¸ä»£ã§ã¤ãªãããã£ããã¢ããªãYay!ï¼ã¤ã§ã¤ï¼ã® API
+                             ã©ããã¼ã§ãã
    ããããæä½ã®èªååãããããã®éçºãå¯è½ã§ãã
 
                    ãã­ã¥ã¡ã³ãã¯ãã¡ããã_Â»
 
                Report_Bug Â· Request_Feature Â· Join_the_discord
   Table of Contents
    1. ã¤ã³ã¹ãã¼ã«
@@ -105,15 +105,15 @@
 ã®ããããã®æ¹æ³ã§ç¹ããã¾ããããè©³ããã¯
 [ãã¡ããã](https://github.com/qvco/yaylib/blob/master/
 CONTRIBUTING.md)ï¼  ## Buy me a coffee
 ãã®ã©ã¤ãã©ãªãæ°ã«å¥ã£ã¦ããã ãããã**ãªãã¸ããªã«ã¹ã¿ã¼ããé¡ããã¾ã
 (â­)** ã¾ããBuy Me a Coffee
 ãããæ¯æ´ããã ãã¾ãã¨å¹¸ãã§ãã [Buy_Me_A_Coffee]  ##
 åè²¬äºé  yaylib ã¯ãAPI
-ã®å¬å¼ãªãµãã¼ããã¡ã³ããã³ã¹ãæä¾ãããã®ã§ã¯ããã¾ããããã®ã¯ã©ã¤ã¢ã³ããä½¿ç¨ããå ´åãå©ç¨èã¯**ãªã¹ã¯ãè²¬ä»»ãèªå·±è² æ**ã§ãããã®ã¨ãã¾ãããã®ã¯ã©ã¤ã¢ã³ãã«ãã£ã¦æä¾ãããæå ±ããã¼ã¿ã®æ­£ç¢ºæ§ãä¿¡é ¼æ§ãå®å¨æ§ãé©ææ§ã«ã¤ãã¦ããããªãä¿è¨¼ãè¡ãã¾ãããã¾ãããã®ã¯ã©ã¤ã¢ã³ãã®ä½¿ç¨ã«ãã£ã¦çããæå®³ãä¸å©çã«ã¤ãã¦ãä¸åã®è²¬ä»»ãè² ããã­ã¾ããå©ç¨èã¯èªå·±ã®è²¬ä»»ã«ããã¦ããã®ã¯ã©ã¤ã¢ã³ããä½¿ç¨ããAPI
+ã®å¬å¼ãªãµãã¼ããã¡ã³ããã³ã¹ãæä¾ãããã®ã§ã¯ããã¾ããããã®ã¯ã©ã¤ã¢ã³ããä½¿ç¨ããå ´åã**å©ç¨èã¯ãªã¹ã¯ãè²¬ä»»ãèªå·±è² æã§ãããã®**ã¨ãã¾ãããã®ã¯ã©ã¤ã¢ã³ãã«ãã£ã¦æä¾ãããæå ±ããã¼ã¿ã®æ­£ç¢ºæ§ãä¿¡é ¼æ§ãå®å¨æ§ãé©ææ§ã«ã¤ãã¦ããããªãä¿è¨¼ãè¡ãã¾ãããã¾ãããã®ã¯ã©ã¤ã¢ã³ãã®ä½¿ç¨ã«ãã£ã¦çããæå®³ãä¸å©çã«ã¤ãã¦ãä¸åã®è²¬ä»»ãè² ããã­ã¾ããå©ç¨èã¯èªå·±ã®è²¬ä»»ã«ããã¦ããã®ã¯ã©ã¤ã¢ã³ããä½¿ç¨ããAPI
 ã«ã¢ã¯ã»ã¹ãããã®ã¨ãã¾ãããªãããã®åè²¬äºé ã¯äºåãªãå¤æ´ãããå ´åãããã¾ãã
 ## ã©ã¤ã»ã³ã¹
    [https://github.com/qvco/yaylib/assets/77382767/5d6aef18-5d98-4c9b-9f54-
                                  791308b393af]
                               MIT Â© Qvco & Konn
 ãã«ã©ã¤ã»ã³ã¹ã¯ [ãã¡ã](https://github.com/qvco/yaylib/blob/
 master/LICENSE) ãããç¢ºèªããã ãã¾ãã
```

### Comparing `yaylib-1.0.8/yaylib.egg-info/SOURCES.txt` & `yaylib-1.0.9/yaylib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

