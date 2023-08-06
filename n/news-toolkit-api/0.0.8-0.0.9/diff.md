# Comparing `tmp/news_toolkit_api-0.0.8.tar.gz` & `tmp/news_toolkit_api-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "news_toolkit_api-0.0.8.tar", max compression
+gzip compressed data, was "news_toolkit_api-0.0.9.tar", max compression
```

## Comparing `news_toolkit_api-0.0.8.tar` & `news_toolkit_api-0.0.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0        0 2023-07-31 14:36:43.243763 news_toolkit_api-0.0.8/README.md
--rw-r--r--   0        0        0        0 2023-07-31 14:33:41.949127 news_toolkit_api-0.0.8/news_toolkit_api/__init__.py
--rw-r--r--   0        0        0        0 2023-07-31 14:37:42.991442 news_toolkit_api-0.0.8/news_toolkit_api/api/__init__.py
--rw-r--r--   0        0        0        0 2023-07-31 14:37:51.893138 news_toolkit_api-0.0.8/news_toolkit_api/api/v1/__init__.py
--rw-r--r--   0        0        0      141 2023-07-31 14:48:20.474554 news_toolkit_api-0.0.8/news_toolkit_api/api/v1/db.py
--rw-r--r--   0        0        0      503 2023-07-31 18:04:25.893255 news_toolkit_api-0.0.8/news_toolkit_api/api/v1/response/__init__.py
--rw-r--r--   0        0        0      413 2023-07-31 17:17:55.468722 news_toolkit_api-0.0.8/news_toolkit_api/api/v1/response/article.py
--rw-r--r--   0        0        0      112 2023-07-31 15:23:52.955109 news_toolkit_api-0.0.8/news_toolkit_api/api/v1/response/category.py
--rw-r--r--   0        0        0      562 2023-07-31 18:12:42.744676 news_toolkit_api-0.0.8/news_toolkit_api/api/v1/response/feed.py
--rw-r--r--   0        0        0      524 2023-07-31 17:56:44.386755 news_toolkit_api-0.0.8/news_toolkit_api/api/v1/response/related_articles.py
--rw-r--r--   0        0        0      425 2023-07-31 16:56:03.922534 news_toolkit_api-0.0.8/news_toolkit_api/api/v1/response/subscription.py
--rw-r--r--   0        0        0     8096 2023-07-31 18:23:16.572703 news_toolkit_api-0.0.8/news_toolkit_api/api/v1/routers.py
--rw-r--r--   0        0        0      479 2023-07-31 17:34:29.932031 news_toolkit_api-0.0.8/news_toolkit_api/app.py
--rw-r--r--   0        0        0        0 2023-07-31 15:25:16.529314 news_toolkit_api-0.0.8/news_toolkit_api/background_tasks/__init__.py
--rw-r--r--   0        0        0      833 2023-07-31 17:09:23.910533 news_toolkit_api-0.0.8/news_toolkit_api/background_tasks/article.py
--rw-r--r--   0        0        0     1030 2023-07-31 18:44:07.483312 news_toolkit_api-0.0.8/news_toolkit_api/background_tasks/feed.py
--rw-r--r--   0        0        0      722 2023-07-31 17:30:01.061321 news_toolkit_api-0.0.8/news_toolkit_api/client.py
--rw-r--r--   0        0        0      267 2023-07-31 17:56:44.375693 news_toolkit_api-0.0.8/news_toolkit_api/db/__init__.py
--rw-r--r--   0        0        0      947 2023-07-31 17:06:06.542261 news_toolkit_api-0.0.8/news_toolkit_api/db/article.py
--rw-r--r--   0        0        0      103 2023-07-31 15:23:52.957324 news_toolkit_api-0.0.8/news_toolkit_api/db/category.py
--rw-r--r--   0        0        0      429 2023-07-31 17:52:45.739386 news_toolkit_api-0.0.8/news_toolkit_api/db/feed.py
--rw-r--r--   0        0        0      557 2023-07-31 16:01:54.164641 news_toolkit_api-0.0.8/news_toolkit_api/db/subscription.py
--rw-r--r--   0        0        0      516 2023-07-31 17:56:44.390573 news_toolkit_api-0.0.8/news_toolkit_api/news_blocks/__init__.py
--rw-r--r--   0        0        0      380 2023-07-31 15:15:00.695109 news_toolkit_api-0.0.8/news_toolkit_api/news_blocks/article_introduction_block.py
--rw-r--r--   0        0        0      380 2023-07-31 15:15:00.691257 news_toolkit_api-0.0.8/news_toolkit_api/news_blocks/banner_ad_block.py
--rw-r--r--   0        0        0      115 2023-07-31 17:52:45.740226 news_toolkit_api-0.0.8/news_toolkit_api/news_blocks/block_type.py
--rw-r--r--   0        0        0      217 2023-07-31 17:52:45.741799 news_toolkit_api-0.0.8/news_toolkit_api/news_blocks/navigate_to_article.py
--rw-r--r--   0        0        0      216 2023-07-31 17:56:41.480758 news_toolkit_api-0.0.8/news_toolkit_api/news_blocks/section_header_block.py
--rw-r--r--   0        0        0      224 2023-07-31 15:15:00.693386 news_toolkit_api-0.0.8/news_toolkit_api/news_blocks/text_lead_paragraph_block.py
--rw-r--r--   0        0        0       66 2023-07-31 16:54:58.270780 news_toolkit_api-0.0.8/news_toolkit_api/repository/__init__.py
--rw-r--r--   0        0        0     2812 2023-07-31 18:20:11.188625 news_toolkit_api-0.0.8/news_toolkit_api/repository/article.py
--rw-r--r--   0        0        0        0 2023-07-31 18:31:25.293622 news_toolkit_api-0.0.8/news_toolkit_api/tool/__init__.py
--rw-r--r--   0        0        0      599 2023-07-31 18:40:33.361105 news_toolkit_api-0.0.8/news_toolkit_api/tool/populate_categories.py
--rw-r--r--   0        0        0      949 2023-07-31 17:30:43.852193 news_toolkit_api-0.0.8/news_toolkit_api/utils.py
--rw-r--r--   0        0        0      845 2023-07-31 18:44:32.594944 news_toolkit_api-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      566 1970-01-01 00:00:00.000000 news_toolkit_api-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-31 14:36:43.243763 news_toolkit_api-0.0.9/README.md
+-rw-r--r--   0        0        0        0 2023-07-31 14:33:41.949127 news_toolkit_api-0.0.9/news_toolkit_api/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-31 14:37:42.991442 news_toolkit_api-0.0.9/news_toolkit_api/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-31 14:37:51.893138 news_toolkit_api-0.0.9/news_toolkit_api/api/v1/__init__.py
+-rw-r--r--   0        0        0      141 2023-07-31 14:48:20.474554 news_toolkit_api-0.0.9/news_toolkit_api/api/v1/db.py
+-rw-r--r--   0        0        0      503 2023-07-31 18:04:25.893255 news_toolkit_api-0.0.9/news_toolkit_api/api/v1/response/__init__.py
+-rw-r--r--   0        0        0      413 2023-07-31 17:17:55.468722 news_toolkit_api-0.0.9/news_toolkit_api/api/v1/response/article.py
+-rw-r--r--   0        0        0      112 2023-07-31 15:23:52.955109 news_toolkit_api-0.0.9/news_toolkit_api/api/v1/response/category.py
+-rw-r--r--   0        0        0      562 2023-07-31 18:12:42.744676 news_toolkit_api-0.0.9/news_toolkit_api/api/v1/response/feed.py
+-rw-r--r--   0        0        0      524 2023-07-31 17:56:44.386755 news_toolkit_api-0.0.9/news_toolkit_api/api/v1/response/related_articles.py
+-rw-r--r--   0        0        0      425 2023-07-31 16:56:03.922534 news_toolkit_api-0.0.9/news_toolkit_api/api/v1/response/subscription.py
+-rw-r--r--   0        0        0     8096 2023-07-31 18:23:16.572703 news_toolkit_api-0.0.9/news_toolkit_api/api/v1/routers.py
+-rw-r--r--   0        0        0      479 2023-07-31 17:34:29.932031 news_toolkit_api-0.0.9/news_toolkit_api/app.py
+-rw-r--r--   0        0        0        0 2023-07-31 15:25:16.529314 news_toolkit_api-0.0.9/news_toolkit_api/background_tasks/__init__.py
+-rw-r--r--   0        0        0      833 2023-07-31 17:09:23.910533 news_toolkit_api-0.0.9/news_toolkit_api/background_tasks/article.py
+-rw-r--r--   0        0        0     1026 2023-07-31 19:08:16.206437 news_toolkit_api-0.0.9/news_toolkit_api/background_tasks/feed.py
+-rw-r--r--   0        0        0      722 2023-07-31 17:30:01.061321 news_toolkit_api-0.0.9/news_toolkit_api/client.py
+-rw-r--r--   0        0        0      267 2023-07-31 17:56:44.375693 news_toolkit_api-0.0.9/news_toolkit_api/db/__init__.py
+-rw-r--r--   0        0        0      947 2023-07-31 17:06:06.542261 news_toolkit_api-0.0.9/news_toolkit_api/db/article.py
+-rw-r--r--   0        0        0      103 2023-07-31 15:23:52.957324 news_toolkit_api-0.0.9/news_toolkit_api/db/category.py
+-rw-r--r--   0        0        0      428 2023-07-31 19:00:01.557197 news_toolkit_api-0.0.9/news_toolkit_api/db/feed.py
+-rw-r--r--   0        0        0      557 2023-07-31 16:01:54.164641 news_toolkit_api-0.0.9/news_toolkit_api/db/subscription.py
+-rw-r--r--   0        0        0      516 2023-07-31 17:56:44.390573 news_toolkit_api-0.0.9/news_toolkit_api/news_blocks/__init__.py
+-rw-r--r--   0        0        0      380 2023-07-31 15:15:00.695109 news_toolkit_api-0.0.9/news_toolkit_api/news_blocks/article_introduction_block.py
+-rw-r--r--   0        0        0      380 2023-07-31 15:15:00.691257 news_toolkit_api-0.0.9/news_toolkit_api/news_blocks/banner_ad_block.py
+-rw-r--r--   0        0        0      115 2023-07-31 17:52:45.740226 news_toolkit_api-0.0.9/news_toolkit_api/news_blocks/block_type.py
+-rw-r--r--   0        0        0      217 2023-07-31 17:52:45.741799 news_toolkit_api-0.0.9/news_toolkit_api/news_blocks/navigate_to_article.py
+-rw-r--r--   0        0        0      216 2023-07-31 17:56:41.480758 news_toolkit_api-0.0.9/news_toolkit_api/news_blocks/section_header_block.py
+-rw-r--r--   0        0        0      224 2023-07-31 15:15:00.693386 news_toolkit_api-0.0.9/news_toolkit_api/news_blocks/text_lead_paragraph_block.py
+-rw-r--r--   0        0        0       66 2023-07-31 16:54:58.270780 news_toolkit_api-0.0.9/news_toolkit_api/repository/__init__.py
+-rw-r--r--   0        0        0     2812 2023-07-31 18:20:11.188625 news_toolkit_api-0.0.9/news_toolkit_api/repository/article.py
+-rw-r--r--   0        0        0        0 2023-07-31 18:31:25.293622 news_toolkit_api-0.0.9/news_toolkit_api/tool/__init__.py
+-rw-r--r--   0        0        0      599 2023-07-31 19:08:08.531007 news_toolkit_api-0.0.9/news_toolkit_api/tool/populate_categories.py
+-rw-r--r--   0        0        0      949 2023-07-31 17:30:43.852193 news_toolkit_api-0.0.9/news_toolkit_api/utils.py
+-rw-r--r--   0        0        0      845 2023-07-31 19:00:01.563090 news_toolkit_api-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      566 1970-01-01 00:00:00.000000 news_toolkit_api-0.0.9/PKG-INFO
```

### Comparing `news_toolkit_api-0.0.8/news_toolkit_api/api/v1/response/feed.py` & `news_toolkit_api-0.0.9/news_toolkit_api/api/v1/response/feed.py`

 * *Files identical despite different names*

### Comparing `news_toolkit_api-0.0.8/news_toolkit_api/api/v1/response/related_articles.py` & `news_toolkit_api-0.0.9/news_toolkit_api/api/v1/response/related_articles.py`

 * *Files identical despite different names*

### Comparing `news_toolkit_api-0.0.8/news_toolkit_api/api/v1/routers.py` & `news_toolkit_api-0.0.9/news_toolkit_api/api/v1/routers.py`

 * *Files identical despite different names*

### Comparing `news_toolkit_api-0.0.8/news_toolkit_api/background_tasks/article.py` & `news_toolkit_api-0.0.9/news_toolkit_api/background_tasks/article.py`

 * *Files identical despite different names*

### Comparing `news_toolkit_api-0.0.8/news_toolkit_api/background_tasks/feed.py` & `news_toolkit_api-0.0.9/news_toolkit_api/background_tasks/feed.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
     feeds = await article_repository.fetch_feed(category)
     if not feeds:
         return None
 
     with client.context():
         for feed in feeds:
-            feed.key = ndb.Key(Feed, sha3_256_hash(feed.article_id))
-            feed.parent = ndb.Key(Category, sha3_256_hash(category))
+            feed.key = ndb.Key(
+                Category, sha3_256_hash(category), Feed, sha3_256_hash(feed.article_id)
+            )
         ndb.put_multi(feeds)
 
     for feed in feeds:
         await background_task_article(client, article_repository, feed.article_id, True)
     return feeds
```

### Comparing `news_toolkit_api-0.0.8/news_toolkit_api/client.py` & `news_toolkit_api-0.0.9/news_toolkit_api/client.py`

 * *Files identical despite different names*

### Comparing `news_toolkit_api-0.0.8/news_toolkit_api/db/article.py` & `news_toolkit_api-0.0.9/news_toolkit_api/db/article.py`

 * *Files identical despite different names*

### Comparing `news_toolkit_api-0.0.8/news_toolkit_api/db/subscription.py` & `news_toolkit_api-0.0.9/news_toolkit_api/db/subscription.py`

 * *Files identical despite different names*

### Comparing `news_toolkit_api-0.0.8/news_toolkit_api/news_blocks/__init__.py` & `news_toolkit_api-0.0.9/news_toolkit_api/news_blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `news_toolkit_api-0.0.8/news_toolkit_api/repository/article.py` & `news_toolkit_api-0.0.9/news_toolkit_api/repository/article.py`

 * *Files identical despite different names*

### Comparing `news_toolkit_api-0.0.8/news_toolkit_api/tool/populate_categories.py` & `news_toolkit_api-0.0.9/news_toolkit_api/tool/populate_categories.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from google.cloud import ndb
-
 import argparse
 
+from google.cloud import ndb
+
 from news_toolkit_api.db import Category
 from news_toolkit_api.utils import sha3_256_hash
 
 client = ndb.Client()
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
```

### Comparing `news_toolkit_api-0.0.8/news_toolkit_api/utils.py` & `news_toolkit_api-0.0.9/news_toolkit_api/utils.py`

 * *Files identical despite different names*

### Comparing `news_toolkit_api-0.0.8/pyproject.toml` & `news_toolkit_api-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "news-toolkit-api"
-version = "0.0.8"
+version = "0.0.9"
 description = ""
 authors = ["wakita181009 <wakita181009@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "news_toolkit_api" }]
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.12"
```

### Comparing `news_toolkit_api-0.0.8/PKG-INFO` & `news_toolkit_api-0.0.9/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: news-toolkit-api
-Version: 0.0.8
+Version: 0.0.9
 Summary: 
 Author: wakita181009
 Author-email: wakita181009@gmail.com
 Requires-Python: >=3.11,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.5,<4.0.0)
```

