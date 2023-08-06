# Comparing `tmp/stigg_api_client-0.522.0.tar.gz` & `tmp/stigg_api_client-0.523.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stigg_api_client-0.522.0.tar", max compression
+gzip compressed data, was "stigg_api_client-0.523.0.tar", max compression
```

## Comparing `stigg_api_client-0.522.0.tar` & `stigg_api_client-0.523.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2479 2023-08-03 12:58:34.798600 stigg_api_client-0.522.0/README.md
--rw-r--r--   0        0        0      480 2023-08-03 12:59:09.115447 stigg_api_client-0.522.0/pyproject.toml
--rw-r--r--   0        0        0       44 2023-08-03 12:58:34.798600 stigg_api_client-0.522.0/stigg/__init__.py
--rw-r--r--   0        0        0     3699 2023-08-03 12:58:34.798600 stigg_api_client-0.522.0/stigg/client.py
--rw-r--r--   0        0        0        0 2023-08-03 12:59:07.115406 stigg_api_client-0.522.0/stigg/generated/__init__.py
--rw-r--r--   0        0        0    51059 2023-08-03 12:59:07.607416 stigg_api_client-0.522.0/stigg/generated/operations.py
--rw-r--r--   0        0        0   471091 2023-08-03 12:59:07.379412 stigg_api_client-0.522.0/stigg/generated/schema.py
--rw-r--r--   0        0        0     3122 1970-01-01 00:00:00.000000 stigg_api_client-0.522.0/PKG-INFO
+-rw-r--r--   0        0        0     2479 2023-08-05 17:43:55.751829 stigg_api_client-0.523.0/README.md
+-rw-r--r--   0        0        0      480 2023-08-05 17:44:32.980558 stigg_api_client-0.523.0/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-08-05 17:43:55.751829 stigg_api_client-0.523.0/stigg/__init__.py
+-rw-r--r--   0        0        0     3699 2023-08-05 17:43:55.751829 stigg_api_client-0.523.0/stigg/client.py
+-rw-r--r--   0        0        0        0 2023-08-05 17:44:30.876522 stigg_api_client-0.523.0/stigg/generated/__init__.py
+-rw-r--r--   0        0        0    51059 2023-08-05 17:44:31.328530 stigg_api_client-0.523.0/stigg/generated/operations.py
+-rw-r--r--   0        0        0   471274 2023-08-05 17:44:31.160527 stigg_api_client-0.523.0/stigg/generated/schema.py
+-rw-r--r--   0        0        0     3122 1970-01-01 00:00:00.000000 stigg_api_client-0.523.0/PKG-INFO
```

### Comparing `stigg_api_client-0.522.0/README.md` & `stigg_api_client-0.523.0/README.md`

 * *Files identical despite different names*

### Comparing `stigg_api_client-0.522.0/stigg/client.py` & `stigg_api_client-0.523.0/stigg/client.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client-0.522.0/stigg/generated/operations.py` & `stigg_api_client-0.523.0/stigg/generated/operations.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client-0.522.0/stigg/generated/schema.py` & `stigg_api_client-0.523.0/stigg/generated/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -3776,15 +3776,15 @@
     __schema__ = schema
     __field_names__ = ('id',)
     id = sgqlc.types.Field(Float, graphql_name='id')
 
 
 class Customer(sgqlc.types.Type):
     __schema__ = schema
-    __field_names__ = ('additional_meta_data', 'billing_currency', 'billing_id', 'billing_link_url', 'coupon', 'created_at', 'crm_hubspot_company_id', 'crm_hubspot_company_url', 'crm_id', 'customer_id', 'default_payment_expiration_month', 'default_payment_expiration_year', 'default_payment_method_id', 'default_payment_method_last4_digits', 'default_payment_method_type', 'deleted_at', 'eligible_for_trial', 'email', 'environment', 'environment_id', 'exclude_from_experiment', 'experiment', 'experiment_info', 'has_active_resource', 'has_active_subscription', 'has_payment_method', 'id', 'name', 'promotional_entitlements', 'ref_id', 'subscriptions', 'sync_states', 'total_active_subscription', 'trialed_plans', 'updated_at')
+    __field_names__ = ('additional_meta_data', 'billing_currency', 'billing_id', 'billing_link_url', 'coupon', 'created_at', 'crm_hubspot_company_id', 'crm_hubspot_company_url', 'crm_id', 'customer_id', 'default_payment_expiration_month', 'default_payment_expiration_year', 'default_payment_method_id', 'default_payment_method_last4_digits', 'default_payment_method_type', 'deleted_at', 'eligible_for_trial', 'email', 'environment', 'environment_id', 'exclude_from_experiment', 'experiment', 'experiment_info', 'has_active_resource', 'has_active_subscription', 'has_payment_method', 'id', 'name', 'promotional_entitlements', 'ref_id', 'subscriptions', 'sync_states', 'total_active_promotional_entitlements', 'total_active_subscription', 'trialed_plans', 'updated_at')
     additional_meta_data = sgqlc.types.Field(JSON, graphql_name='additionalMetaData')
     billing_currency = sgqlc.types.Field(Currency, graphql_name='billingCurrency')
     billing_id = sgqlc.types.Field(String, graphql_name='billingId')
     billing_link_url = sgqlc.types.Field(String, graphql_name='billingLinkUrl')
     coupon = sgqlc.types.Field(Coupon, graphql_name='coupon')
     created_at = sgqlc.types.Field(DateTime, graphql_name='createdAt')
     crm_hubspot_company_id = sgqlc.types.Field(String, graphql_name='crmHubspotCompanyId')
@@ -3817,14 +3817,15 @@
     ref_id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='refId')
     subscriptions = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('CustomerSubscription')), graphql_name='subscriptions', args=sgqlc.types.ArgDict((
         ('filter', sgqlc.types.Arg(CustomerSubscriptionFilter, graphql_name='filter', default={'status': {'in': ['ACTIVE', 'IN_TRIAL']}})),
         ('sorting', sgqlc.types.Arg(sgqlc.types.list_of(sgqlc.types.non_null(CustomerSubscriptionSort)), graphql_name='sorting', default=[{'direction': 'DESC', 'field': 'createdAt'}])),
 ))
     )
     sync_states = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('SyncState')), graphql_name='syncStates')
+    total_active_promotional_entitlements = sgqlc.types.Field(sgqlc.types.non_null(Float), graphql_name='totalActivePromotionalEntitlements')
     total_active_subscription = sgqlc.types.Field(sgqlc.types.non_null(Float), graphql_name='totalActiveSubscription')
     trialed_plans = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('TrialedPlan')), graphql_name='trialedPlans')
     updated_at = sgqlc.types.Field(sgqlc.types.non_null(DateTime), graphql_name='updatedAt')
 
 
 class CustomerAggregateGroupBy(sgqlc.types.Type):
     __schema__ = schema
```

### Comparing `stigg_api_client-0.522.0/PKG-INFO` & `stigg_api_client-0.523.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stigg-api-client
-Version: 0.522.0
+Version: 0.523.0
 Summary: 
 Author: Stigg
 Author-email: support@stigg.io
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

