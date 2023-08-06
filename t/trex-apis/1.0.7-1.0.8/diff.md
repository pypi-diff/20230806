# Comparing `tmp/trex-apis-1.0.7.tar.gz` & `tmp/trex-apis-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trex-apis-1.0.7.tar", last modified: Fri Aug  4 06:32:54 2023, max compression
+gzip compressed data, was "trex-apis-1.0.8.tar", last modified: Sun Aug  6 12:16:18 2023, max compression
```

## Comparing `trex-apis-1.0.7.tar` & `trex-apis-1.0.8.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-04 06:32:54.427461 trex-apis-1.0.7/
--rw-r--r--   0 jacklok    (501) staff       (20)      447 2023-08-04 06:32:54.427730 trex-apis-1.0.7/PKG-INFO
--rw-r--r--   0 jacklok    (501) staff       (20)       25 2021-06-30 02:28:26.000000 trex-apis-1.0.7/README.md
--rw-r--r--   0 jacklok    (501) staff       (20)       75 2023-08-04 06:32:54.428414 trex-apis-1.0.7/setup.cfg
--rw-r--r--   0 jacklok    (501) staff       (20)      713 2023-08-04 06:32:32.000000 trex-apis-1.0.7/setup.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-04 06:32:54.386372 trex-apis-1.0.7/trex_apis.egg-info/
--rw-r--r--   0 jacklok    (501) staff       (20)      447 2023-08-04 06:32:54.000000 trex-apis-1.0.7/trex_apis.egg-info/PKG-INFO
--rw-r--r--   0 jacklok    (501) staff       (20)     1371 2023-08-04 06:32:54.000000 trex-apis-1.0.7/trex_apis.egg-info/SOURCES.txt
--rw-r--r--   0 jacklok    (501) staff       (20)        1 2023-08-04 06:32:54.000000 trex-apis-1.0.7/trex_apis.egg-info/dependency_links.txt
--rw-r--r--   0 jacklok    (501) staff       (20)       23 2023-08-04 06:32:54.000000 trex-apis-1.0.7/trex_apis.egg-info/requires.txt
--rw-r--r--   0 jacklok    (501) staff       (20)        8 2023-08-04 06:32:54.000000 trex-apis-1.0.7/trex_apis.egg-info/top_level.txt
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-04 06:32:54.387356 trex-apis-1.0.7/trexapi/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-06-30 02:30:07.000000 trex-apis-1.0.7/trexapi/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)      937 2023-07-20 09:41:39.000000 trex-apis-1.0.7/trexapi/conf.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-04 06:32:54.412939 trex-apis-1.0.7/trexapi/controllers/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-06-30 02:45:28.000000 trex-apis-1.0.7/trexapi/controllers/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     4523 2023-05-23 05:00:09.000000 trex-apis-1.0.7/trexapi/controllers/api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     3850 2023-05-25 08:10:20.000000 trex-apis-1.0.7/trexapi/controllers/app_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    35947 2023-05-18 03:00:00.000000 trex-apis-1.0.7/trexapi/controllers/customer_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     6945 2023-04-13 05:36:42.000000 trex-apis-1.0.7/trexapi/controllers/customer_membership_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     4750 2023-01-30 07:03:11.000000 trex-apis-1.0.7/trexapi/controllers/customer_reward_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    13204 2023-05-15 02:06:38.000000 trex-apis-1.0.7/trexapi/controllers/loyalty_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    13485 2023-07-12 07:15:15.000000 trex-apis-1.0.7/trexapi/controllers/lucky_draw_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    15269 2023-07-10 09:47:14.000000 trex-apis-1.0.7/trexapi/controllers/merchant_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    11170 2023-05-16 03:00:59.000000 trex-apis-1.0.7/trexapi/controllers/outlet_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1430 2022-09-26 04:18:01.000000 trex-apis-1.0.7/trexapi/controllers/payment_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    24944 2023-05-23 09:32:47.000000 trex-apis-1.0.7/trexapi/controllers/pos_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    27329 2023-04-18 07:01:48.000000 trex-apis-1.0.7/trexapi/controllers/reward_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    12777 2023-07-25 03:49:49.000000 trex-apis-1.0.7/trexapi/controllers/sales_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)      998 2023-04-18 06:08:18.000000 trex-apis-1.0.7/trexapi/controllers/transaction_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    52259 2023-08-04 05:57:17.000000 trex-apis-1.0.7/trexapi/controllers/user_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     2980 2023-01-30 02:56:35.000000 trex-apis-1.0.7/trexapi/controllers/user_reward_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    16314 2023-07-05 09:44:39.000000 trex-apis-1.0.7/trexapi/controllers/voucher_api_routes.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-04 06:32:54.414640 trex-apis-1.0.7/trexapi/decorators/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-01 08:42:13.000000 trex-apis-1.0.7/trexapi/decorators/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     5778 2023-06-30 15:57:30.000000 trex-apis-1.0.7/trexapi/decorators/api_decorators.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-04 06:32:54.420851 trex-apis-1.0.7/trexapi/forms/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-12 06:42:53.000000 trex-apis-1.0.7/trexapi/forms/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     7419 2023-02-08 10:14:32.000000 trex-apis-1.0.7/trexapi/forms/customer_api_forms.py
--rw-r--r--   0 jacklok    (501) staff       (20)     7285 2023-04-18 02:42:03.000000 trex-apis-1.0.7/trexapi/forms/reward_api_forms.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1547 2023-04-18 02:41:54.000000 trex-apis-1.0.7/trexapi/forms/sales_api_forms.py
--rw-r--r--   0 jacklok    (501) staff       (20)     3922 2023-05-29 03:02:06.000000 trex-apis-1.0.7/trexapi/forms/user_api_forms.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-04 06:32:54.422275 trex-apis-1.0.7/trexapi/libs/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-05 10:17:19.000000 trex-apis-1.0.7/trexapi/libs/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1143 2021-07-05 10:57:23.000000 trex-apis-1.0.7/trexapi/libs/flask_auth_wrapper.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-04 06:32:54.425588 trex-apis-1.0.7/trexapi/utils/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-08 10:01:06.000000 trex-apis-1.0.7/trexapi/utils/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1347 2022-12-20 01:23:01.000000 trex-apis-1.0.7/trexapi/utils/api_helpers.py
--rw-r--r--   0 jacklok    (501) staff       (20)    78420 2023-06-30 14:45:12.000000 trex-apis-1.0.7/trexapi/utils/reward_transaction_helper.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-06 12:16:18.560687 trex-apis-1.0.8/
+-rw-r--r--   0 jacklok    (501) staff       (20)      447 2023-08-06 12:16:18.560834 trex-apis-1.0.8/PKG-INFO
+-rw-r--r--   0 jacklok    (501) staff       (20)       25 2021-06-30 02:28:26.000000 trex-apis-1.0.8/README.md
+-rw-r--r--   0 jacklok    (501) staff       (20)       75 2023-08-06 12:16:18.561298 trex-apis-1.0.8/setup.cfg
+-rw-r--r--   0 jacklok    (501) staff       (20)      713 2023-08-06 12:15:59.000000 trex-apis-1.0.8/setup.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-06 12:16:18.536532 trex-apis-1.0.8/trex_apis.egg-info/
+-rw-r--r--   0 jacklok    (501) staff       (20)      447 2023-08-06 12:16:18.000000 trex-apis-1.0.8/trex_apis.egg-info/PKG-INFO
+-rw-r--r--   0 jacklok    (501) staff       (20)     1371 2023-08-06 12:16:18.000000 trex-apis-1.0.8/trex_apis.egg-info/SOURCES.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)        1 2023-08-06 12:16:18.000000 trex-apis-1.0.8/trex_apis.egg-info/dependency_links.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)       23 2023-08-06 12:16:18.000000 trex-apis-1.0.8/trex_apis.egg-info/requires.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)        8 2023-08-06 12:16:18.000000 trex-apis-1.0.8/trex_apis.egg-info/top_level.txt
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-06 12:16:18.537332 trex-apis-1.0.8/trexapi/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-06-30 02:30:07.000000 trex-apis-1.0.8/trexapi/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      937 2023-07-20 09:41:39.000000 trex-apis-1.0.8/trexapi/conf.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-06 12:16:18.552741 trex-apis-1.0.8/trexapi/controllers/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-06-30 02:45:28.000000 trex-apis-1.0.8/trexapi/controllers/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     4523 2023-05-23 05:00:09.000000 trex-apis-1.0.8/trexapi/controllers/api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     3850 2023-05-25 08:10:20.000000 trex-apis-1.0.8/trexapi/controllers/app_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    35947 2023-05-18 03:00:00.000000 trex-apis-1.0.8/trexapi/controllers/customer_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     6945 2023-04-13 05:36:42.000000 trex-apis-1.0.8/trexapi/controllers/customer_membership_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     4750 2023-01-30 07:03:11.000000 trex-apis-1.0.8/trexapi/controllers/customer_reward_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    13204 2023-05-15 02:06:38.000000 trex-apis-1.0.8/trexapi/controllers/loyalty_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    13485 2023-07-12 07:15:15.000000 trex-apis-1.0.8/trexapi/controllers/lucky_draw_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    15269 2023-07-10 09:47:14.000000 trex-apis-1.0.8/trexapi/controllers/merchant_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    11170 2023-05-16 03:00:59.000000 trex-apis-1.0.8/trexapi/controllers/outlet_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1430 2022-09-26 04:18:01.000000 trex-apis-1.0.8/trexapi/controllers/payment_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    24944 2023-05-23 09:32:47.000000 trex-apis-1.0.8/trexapi/controllers/pos_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    27329 2023-04-18 07:01:48.000000 trex-apis-1.0.8/trexapi/controllers/reward_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    12777 2023-07-25 03:49:49.000000 trex-apis-1.0.8/trexapi/controllers/sales_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      998 2023-04-18 06:08:18.000000 trex-apis-1.0.8/trexapi/controllers/transaction_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    53747 2023-08-06 10:06:40.000000 trex-apis-1.0.8/trexapi/controllers/user_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     2980 2023-01-30 02:56:35.000000 trex-apis-1.0.8/trexapi/controllers/user_reward_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    16314 2023-07-05 09:44:39.000000 trex-apis-1.0.8/trexapi/controllers/voucher_api_routes.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-06 12:16:18.553726 trex-apis-1.0.8/trexapi/decorators/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-01 08:42:13.000000 trex-apis-1.0.8/trexapi/decorators/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     5778 2023-06-30 15:57:30.000000 trex-apis-1.0.8/trexapi/decorators/api_decorators.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-06 12:16:18.556820 trex-apis-1.0.8/trexapi/forms/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-12 06:42:53.000000 trex-apis-1.0.8/trexapi/forms/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     7419 2023-02-08 10:14:32.000000 trex-apis-1.0.8/trexapi/forms/customer_api_forms.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     7285 2023-04-18 02:42:03.000000 trex-apis-1.0.8/trexapi/forms/reward_api_forms.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1547 2023-04-18 02:41:54.000000 trex-apis-1.0.8/trexapi/forms/sales_api_forms.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     3922 2023-05-29 03:02:06.000000 trex-apis-1.0.8/trexapi/forms/user_api_forms.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-06 12:16:18.557739 trex-apis-1.0.8/trexapi/libs/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-05 10:17:19.000000 trex-apis-1.0.8/trexapi/libs/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1143 2021-07-05 10:57:23.000000 trex-apis-1.0.8/trexapi/libs/flask_auth_wrapper.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-06 12:16:18.559408 trex-apis-1.0.8/trexapi/utils/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-08 10:01:06.000000 trex-apis-1.0.8/trexapi/utils/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1347 2022-12-20 01:23:01.000000 trex-apis-1.0.8/trexapi/utils/api_helpers.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    78420 2023-06-30 14:45:12.000000 trex-apis-1.0.8/trexapi/utils/reward_transaction_helper.py
```

### Comparing `trex-apis-1.0.7/setup.py` & `trex-apis-1.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setuptools.setup(
      name='trex-apis',  
-     version='1.0.7',
+     version='1.0.8',
      author="Jack Lok",
      author_email="sglok77@gmail.com",
      description="TRex APIs package",
      long_description=long_description,
      long_description_content_type="text/markdown",
      url="https://bitbucket.org/lokjac/trex-apis",
      packages=setuptools.find_packages(),
```

### Comparing `trex-apis-1.0.7/trex_apis.egg-info/SOURCES.txt` & `trex-apis-1.0.8/trex_apis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.7/trexapi/conf.py` & `trex-apis-1.0.8/trexapi/conf.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.7/trexapi/controllers/api_routes.py` & `trex-apis-1.0.8/trexapi/controllers/api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.7/trexapi/controllers/app_api_routes.py` & `trex-apis-1.0.8/trexapi/controllers/app_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.7/trexapi/controllers/customer_api_routes.py` & `trex-apis-1.0.8/trexapi/controllers/customer_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.7/trexapi/controllers/customer_membership_api_routes.py` & `trex-apis-1.0.8/trexapi/controllers/customer_membership_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.7/trexapi/controllers/customer_reward_api_routes.py` & `trex-apis-1.0.8/trexapi/controllers/customer_reward_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.7/trexapi/controllers/loyalty_api_routes.py` & `trex-apis-1.0.8/trexapi/controllers/loyalty_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.7/trexapi/controllers/lucky_draw_api_routes.py` & `trex-apis-1.0.8/trexapi/controllers/lucky_draw_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.7/trexapi/controllers/merchant_api_routes.py` & `trex-apis-1.0.8/trexapi/controllers/merchant_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.7/trexapi/controllers/outlet_api_routes.py` & `trex-apis-1.0.8/trexapi/controllers/outlet_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.7/trexapi/controllers/payment_api_routes.py` & `trex-apis-1.0.8/trexapi/controllers/payment_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.7/trexapi/controllers/pos_api_routes.py` & `trex-apis-1.0.8/trexapi/controllers/pos_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.7/trexapi/controllers/reward_api_routes.py` & `trex-apis-1.0.8/trexapi/controllers/reward_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.7/trexapi/controllers/sales_api_routes.py` & `trex-apis-1.0.8/trexapi/controllers/sales_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.7/trexapi/controllers/transaction_api_routes.py` & `trex-apis-1.0.8/trexapi/controllers/transaction_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.7/trexapi/controllers/user_api_routes.py` & `trex-apis-1.0.8/trexapi/controllers/user_api_routes.py`

 * *Files 5% similar despite different names*

```diff
@@ -279,15 +279,41 @@
             
         else:
             return create_rest_message('User email or password is not match', status_code=StatusCode.BAD_REQUEST)
             
     else:
         logger.warn('auth_user: user verify input is invalid')
         return create_rest_message('Missing email or password', status_code=StatusCode.BAD_REQUEST)
+
+
+
+@user_api_bp.route('/set-email-verified', methods=['POST'])
+@user_auth_token_required
+def set_email_verified():
+    
+    reference_code      = request.headers.get('x-reference-code')
+    
     
+    db_client = create_db_client(caller_info="set_email_verified")
+    
+    logger.debug('set_email_verified: going to find user account by reference code=%s', reference_code)
+    
+    with db_client.context():
+        user_acct   = User.get_by_reference_code(reference_code)
+    
+    if user_acct:
+        with db_client.context():
+            user_acct.mark_email_verified()
+        
+        return create_rest_message(status_code=StatusCode.OK)
+    
+    else:
+        return create_rest_message(status_code=StatusCode.BAD_REQUEST)
+            
+      
 @user_api_bp.route('/verify-email', methods=['POST'])
 def verify_email_account():
     
     user_data_in_json   = request.get_json()
     email               = user_data_in_json.get('email')
     verification_code   = user_data_in_json.get('verification_code')
     
@@ -479,25 +505,25 @@
     
     email_vc_expiry_datetime            = None
     mobile_phone_vc_expiry_datetime     = None
     
     email_verified_datetime             = None
     mobile_phone_verified_datetime      = None
     
-    if is_email_verified == False and is_not_empty(user_acct.email_vc_expiry_datetime):
-        #vg_generated_datetime = user_acct.vg_generated_datetime.strftime(user_acct.vg_generated_datetime, '%d/%m/%Y, %H:%M:%S')
-        email_vc_expiry_datetime = str(user_acct.email_vc_expiry_datetime)
+    if is_email_verified == False and user_acct.email_vc_expiry_datetime is not None:
+        email_vc_expiry_datetime = user_acct.email_vc_expiry_datetime.strftime('%d-%m-%Y %H:%M:%S') 
     else:
-        email_verified_datetime = str(user_acct.email_verified_datetime)
+        if user_acct.email_verified_datetime is not None:
+            email_verified_datetime = user_acct.email_verified_datetime.strftime('%d-%m-%Y %H:%M:%S') 
             
-    if is_mobile_phone_verified == False and is_not_empty(user_acct.mobile_phone_vc_expiry_datetime):
-        #vg_generated_datetime = user_acct.vg_generated_datetime.strftime(user_acct.vg_generated_datetime, '%d/%m/%Y, %H:%M:%S')
+    if is_mobile_phone_verified == False and user_acct.mobile_phone_vc_expiry_datetime is not None:
         mobile_phone_vc_expiry_datetime = user_acct.mobile_phone_vc_expiry_datetime.strftime('%d-%m-%Y %H:%M:%S')
     else:
-        mobile_phone_verified_datetime = user_acct.mobile_phone_verified_datetime.strftime('%d-%m-%Y %H:%M:%S')
+        if user_acct.mobile_phone_verified_datetime is not None:
+            mobile_phone_verified_datetime = user_acct.mobile_phone_verified_datetime.strftime('%d-%m-%Y %H:%M:%S')
         
     birth_date_str = None
     if is_not_empty(user_acct.birth_date):
         birth_date_str = user_acct.birth_date.strftime('%d-%m-%Y')
          
     
     user_details = {
@@ -787,15 +813,29 @@
                 
             return create_rest_message(status_code=StatusCode.OK, 
                                        #email_vc_expiry_datetime          = str(email_vc_expiry_datetime),
                                        expiry_datetime     = email_vc_expiry_datetime.strftime('%d-%m-%Y %H:%M:%S'),
                                        code                = email_vc,
                                        )
         else:
-            return create_rest_message('The email have been taken %s' % email, status_code=StatusCode.BAD_REQUEST)
+            reference_code = request.headers.get('x-reference-code')
+            
+            if reference_code == user_acct.reference_code:
+                email_vc_expiry_datetime    = datetime.utcnow() + timedelta(minutes=2)
+                email_vc                    = random_number(6)
+                
+                send_email_verification_code_email(email, email_vc)
+                
+                return create_rest_message(status_code=StatusCode.OK, 
+                                       #email_vc_expiry_datetime          = str(email_vc_expiry_datetime),
+                                       expiry_datetime     = email_vc_expiry_datetime.strftime('%d-%m-%Y %H:%M:%S'),
+                                       code                = email_vc,
+                                       )
+            else:
+                return create_rest_message('The email have been taken %s' % email, status_code=StatusCode.BAD_REQUEST)
             
     else:
         logger.warn('reset_email_verification_code: reference code is invalid')
         return create_rest_message(status_code=StatusCode.BAD_REQUEST) 
     
 @user_api_bp.route('/reset-mobile-phone-vc', methods=['PUT'])
 @user_auth_token_required
```

### Comparing `trex-apis-1.0.7/trexapi/controllers/user_reward_api_routes.py` & `trex-apis-1.0.8/trexapi/controllers/user_reward_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.7/trexapi/controllers/voucher_api_routes.py` & `trex-apis-1.0.8/trexapi/controllers/voucher_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.7/trexapi/decorators/api_decorators.py` & `trex-apis-1.0.8/trexapi/decorators/api_decorators.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.7/trexapi/forms/customer_api_forms.py` & `trex-apis-1.0.8/trexapi/forms/customer_api_forms.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.7/trexapi/forms/reward_api_forms.py` & `trex-apis-1.0.8/trexapi/forms/reward_api_forms.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.7/trexapi/forms/sales_api_forms.py` & `trex-apis-1.0.8/trexapi/forms/sales_api_forms.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.7/trexapi/forms/user_api_forms.py` & `trex-apis-1.0.8/trexapi/forms/user_api_forms.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.7/trexapi/libs/flask_auth_wrapper.py` & `trex-apis-1.0.8/trexapi/libs/flask_auth_wrapper.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.7/trexapi/utils/api_helpers.py` & `trex-apis-1.0.8/trexapi/utils/api_helpers.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.7/trexapi/utils/reward_transaction_helper.py` & `trex-apis-1.0.8/trexapi/utils/reward_transaction_helper.py`

 * *Files identical despite different names*

