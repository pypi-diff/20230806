# Comparing `tmp/alibabacloud_resourcedirectorymaster20220419-1.0.3.tar.gz` & `tmp/alibabacloud_resourcedirectorymaster20220419-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_resourcedirectorymaster20220419-1.0.3.tar", last modified: Wed Jul 26 01:44:40 2023, max compression
+gzip compressed data, was "dist/alibabacloud_resourcedirectorymaster20220419-1.0.4.tar", last modified: Sun Aug  6 14:09:16 2023, max compression
```

## Comparing `alibabacloud_resourcedirectorymaster20220419-1.0.3.tar` & `alibabacloud_resourcedirectorymaster20220419-1.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 01:44:40.000000 alibabacloud_resourcedirectorymaster20220419-1.0.3/
--rw-r--r--   0 root         (0) root         (0)      258 2023-07-26 01:44:40.000000 alibabacloud_resourcedirectorymaster20220419-1.0.3/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-07-26 01:44:40.000000 alibabacloud_resourcedirectorymaster20220419-1.0.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-26 01:44:40.000000 alibabacloud_resourcedirectorymaster20220419-1.0.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2448 2023-07-26 01:44:40.000000 alibabacloud_resourcedirectorymaster20220419-1.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1082 2023-07-26 01:44:40.000000 alibabacloud_resourcedirectorymaster20220419-1.0.3/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1167 2023-07-26 01:44:40.000000 alibabacloud_resourcedirectorymaster20220419-1.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 01:44:40.000000 alibabacloud_resourcedirectorymaster20220419-1.0.3/alibabacloud_resourcedirectorymaster20220419/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-26 01:44:40.000000 alibabacloud_resourcedirectorymaster20220419-1.0.3/alibabacloud_resourcedirectorymaster20220419/__init__.py
--rw-r--r--   0 root         (0) root         (0)   254005 2023-07-26 01:44:40.000000 alibabacloud_resourcedirectorymaster20220419-1.0.3/alibabacloud_resourcedirectorymaster20220419/client.py
--rw-r--r--   0 root         (0) root         (0)   404794 2023-07-26 01:44:40.000000 alibabacloud_resourcedirectorymaster20220419-1.0.3/alibabacloud_resourcedirectorymaster20220419/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 01:44:40.000000 alibabacloud_resourcedirectorymaster20220419-1.0.3/alibabacloud_resourcedirectorymaster20220419.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2448 2023-07-26 01:44:40.000000 alibabacloud_resourcedirectorymaster20220419-1.0.3/alibabacloud_resourcedirectorymaster20220419.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      580 2023-07-26 01:44:40.000000 alibabacloud_resourcedirectorymaster20220419-1.0.3/alibabacloud_resourcedirectorymaster20220419.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 01:44:40.000000 alibabacloud_resourcedirectorymaster20220419-1.0.3/alibabacloud_resourcedirectorymaster20220419.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2023-07-26 01:44:40.000000 alibabacloud_resourcedirectorymaster20220419-1.0.3/alibabacloud_resourcedirectorymaster20220419.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       45 2023-07-26 01:44:40.000000 alibabacloud_resourcedirectorymaster20220419-1.0.3/alibabacloud_resourcedirectorymaster20220419.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-26 01:44:40.000000 alibabacloud_resourcedirectorymaster20220419-1.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2711 2023-07-26 01:44:40.000000 alibabacloud_resourcedirectorymaster20220419-1.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 14:09:16.000000 alibabacloud_resourcedirectorymaster20220419-1.0.4/
+-rw-r--r--   0 root         (0) root         (0)      393 2023-08-06 14:09:15.000000 alibabacloud_resourcedirectorymaster20220419-1.0.4/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-08-06 14:09:15.000000 alibabacloud_resourcedirectorymaster20220419-1.0.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-08-06 14:09:15.000000 alibabacloud_resourcedirectorymaster20220419-1.0.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2448 2023-08-06 14:09:16.000000 alibabacloud_resourcedirectorymaster20220419-1.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1082 2023-08-06 14:09:15.000000 alibabacloud_resourcedirectorymaster20220419-1.0.4/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1167 2023-08-06 14:09:15.000000 alibabacloud_resourcedirectorymaster20220419-1.0.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 14:09:16.000000 alibabacloud_resourcedirectorymaster20220419-1.0.4/alibabacloud_resourcedirectorymaster20220419/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-08-06 14:09:15.000000 alibabacloud_resourcedirectorymaster20220419-1.0.4/alibabacloud_resourcedirectorymaster20220419/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   261027 2023-08-06 14:09:15.000000 alibabacloud_resourcedirectorymaster20220419-1.0.4/alibabacloud_resourcedirectorymaster20220419/client.py
+-rw-r--r--   0 root         (0) root         (0)   414631 2023-08-06 14:09:15.000000 alibabacloud_resourcedirectorymaster20220419-1.0.4/alibabacloud_resourcedirectorymaster20220419/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 14:09:16.000000 alibabacloud_resourcedirectorymaster20220419-1.0.4/alibabacloud_resourcedirectorymaster20220419.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2448 2023-08-06 14:09:15.000000 alibabacloud_resourcedirectorymaster20220419-1.0.4/alibabacloud_resourcedirectorymaster20220419.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      580 2023-08-06 14:09:15.000000 alibabacloud_resourcedirectorymaster20220419-1.0.4/alibabacloud_resourcedirectorymaster20220419.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-06 14:09:15.000000 alibabacloud_resourcedirectorymaster20220419-1.0.4/alibabacloud_resourcedirectorymaster20220419.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2023-08-06 14:09:15.000000 alibabacloud_resourcedirectorymaster20220419-1.0.4/alibabacloud_resourcedirectorymaster20220419.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2023-08-06 14:09:15.000000 alibabacloud_resourcedirectorymaster20220419-1.0.4/alibabacloud_resourcedirectorymaster20220419.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-08-06 14:09:16.000000 alibabacloud_resourcedirectorymaster20220419-1.0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2711 2023-08-06 14:09:15.000000 alibabacloud_resourcedirectorymaster20220419-1.0.4/setup.py
```

### Comparing `alibabacloud_resourcedirectorymaster20220419-1.0.3/LICENSE` & `alibabacloud_resourcedirectorymaster20220419-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_resourcedirectorymaster20220419-1.0.3/PKG-INFO` & `alibabacloud_resourcedirectorymaster20220419-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_resourcedirectorymaster20220419
-Version: 1.0.3
+Version: 1.0.4
 Summary: Alibaba Cloud ResourceDirectoryMaster (20220419) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_resourcedirectorymaster20220419-1.0.3/README-CN.md` & `alibabacloud_resourcedirectorymaster20220419-1.0.4/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_resourcedirectorymaster20220419-1.0.3/README.md` & `alibabacloud_resourcedirectorymaster20220419-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_resourcedirectorymaster20220419-1.0.3/alibabacloud_resourcedirectorymaster20220419/client.py` & `alibabacloud_resourcedirectorymaster20220419-1.0.4/alibabacloud_resourcedirectorymaster20220419/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1279,17 +1279,16 @@
 
     def delete_account_with_options(
         self,
         tmp_req: resource_directory_master_20220419_models.DeleteAccountRequest,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.DeleteAccountResponse:
         """
-        > The member deletion feature is in invitational preview. You can contact the customer business manager (CBM) of Alibaba Cloud to apply for a trial.
         Before you delete a member, we recommend that you call the [CheckAccountDelete](~~CheckAccountDelete~~) and [GetAccountDeletionCheckResult](~~GetAccountDeletionCheckResult~~) operations to check whether the member meets deletion requirements. You can call the DeleteAccount operation to delete only members that meet the deletion requirements.
-        After a member is deleted, the resources and data within the member are deleted, and you can no longer use the member to log on to the Alibaba Cloud Management Console. In addition, the member cannot be recovered. Proceed with caution. For more information about how to delete a member, see [Delete a member of the resource account type](~~446078~~).
+        After you submit a deletion request for a member, you can call the [GetAccountDeletionStatus](~~GetAccountDeletionStatus~~) operation to query the deletion status of the member. After a member is deleted, the resources and data within the member are deleted, and you can no longer use the member to log on to the Alibaba Cloud Management Console. In addition, the member cannot be recovered. Proceed with caution. For more information about how to delete a member, see [Delete a member of the resource account type](~~446078~~).
         
         @param tmp_req: DeleteAccountRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteAccountResponse
         """
         UtilClient.validate_model(tmp_req)
         request = resource_directory_master_20220419_models.DeleteAccountShrinkRequest()
@@ -1322,17 +1321,16 @@
 
     async def delete_account_with_options_async(
         self,
         tmp_req: resource_directory_master_20220419_models.DeleteAccountRequest,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.DeleteAccountResponse:
         """
-        > The member deletion feature is in invitational preview. You can contact the customer business manager (CBM) of Alibaba Cloud to apply for a trial.
         Before you delete a member, we recommend that you call the [CheckAccountDelete](~~CheckAccountDelete~~) and [GetAccountDeletionCheckResult](~~GetAccountDeletionCheckResult~~) operations to check whether the member meets deletion requirements. You can call the DeleteAccount operation to delete only members that meet the deletion requirements.
-        After a member is deleted, the resources and data within the member are deleted, and you can no longer use the member to log on to the Alibaba Cloud Management Console. In addition, the member cannot be recovered. Proceed with caution. For more information about how to delete a member, see [Delete a member of the resource account type](~~446078~~).
+        After you submit a deletion request for a member, you can call the [GetAccountDeletionStatus](~~GetAccountDeletionStatus~~) operation to query the deletion status of the member. After a member is deleted, the resources and data within the member are deleted, and you can no longer use the member to log on to the Alibaba Cloud Management Console. In addition, the member cannot be recovered. Proceed with caution. For more information about how to delete a member, see [Delete a member of the resource account type](~~446078~~).
         
         @param tmp_req: DeleteAccountRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteAccountResponse
         """
         UtilClient.validate_model(tmp_req)
         request = resource_directory_master_20220419_models.DeleteAccountShrinkRequest()
@@ -1364,32 +1362,30 @@
         )
 
     def delete_account(
         self,
         request: resource_directory_master_20220419_models.DeleteAccountRequest,
     ) -> resource_directory_master_20220419_models.DeleteAccountResponse:
         """
-        > The member deletion feature is in invitational preview. You can contact the customer business manager (CBM) of Alibaba Cloud to apply for a trial.
         Before you delete a member, we recommend that you call the [CheckAccountDelete](~~CheckAccountDelete~~) and [GetAccountDeletionCheckResult](~~GetAccountDeletionCheckResult~~) operations to check whether the member meets deletion requirements. You can call the DeleteAccount operation to delete only members that meet the deletion requirements.
-        After a member is deleted, the resources and data within the member are deleted, and you can no longer use the member to log on to the Alibaba Cloud Management Console. In addition, the member cannot be recovered. Proceed with caution. For more information about how to delete a member, see [Delete a member of the resource account type](~~446078~~).
+        After you submit a deletion request for a member, you can call the [GetAccountDeletionStatus](~~GetAccountDeletionStatus~~) operation to query the deletion status of the member. After a member is deleted, the resources and data within the member are deleted, and you can no longer use the member to log on to the Alibaba Cloud Management Console. In addition, the member cannot be recovered. Proceed with caution. For more information about how to delete a member, see [Delete a member of the resource account type](~~446078~~).
         
         @param request: DeleteAccountRequest
         @return: DeleteAccountResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.delete_account_with_options(request, runtime)
 
     async def delete_account_async(
         self,
         request: resource_directory_master_20220419_models.DeleteAccountRequest,
     ) -> resource_directory_master_20220419_models.DeleteAccountResponse:
         """
-        > The member deletion feature is in invitational preview. You can contact the customer business manager (CBM) of Alibaba Cloud to apply for a trial.
         Before you delete a member, we recommend that you call the [CheckAccountDelete](~~CheckAccountDelete~~) and [GetAccountDeletionCheckResult](~~GetAccountDeletionCheckResult~~) operations to check whether the member meets deletion requirements. You can call the DeleteAccount operation to delete only members that meet the deletion requirements.
-        After a member is deleted, the resources and data within the member are deleted, and you can no longer use the member to log on to the Alibaba Cloud Management Console. In addition, the member cannot be recovered. Proceed with caution. For more information about how to delete a member, see [Delete a member of the resource account type](~~446078~~).
+        After you submit a deletion request for a member, you can call the [GetAccountDeletionStatus](~~GetAccountDeletionStatus~~) operation to query the deletion status of the member. After a member is deleted, the resources and data within the member are deleted, and you can no longer use the member to log on to the Alibaba Cloud Management Console. In addition, the member cannot be recovered. Proceed with caution. For more information about how to delete a member, see [Delete a member of the resource account type](~~446078~~).
         
         @param request: DeleteAccountRequest
         @return: DeleteAccountResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.delete_account_with_options_async(request, runtime)
 
@@ -4105,14 +4101,96 @@
     async def list_message_contacts_async(
         self,
         request: resource_directory_master_20220419_models.ListMessageContactsRequest,
     ) -> resource_directory_master_20220419_models.ListMessageContactsResponse:
         runtime = util_models.RuntimeOptions()
         return await self.list_message_contacts_with_options_async(request, runtime)
 
+    def list_tag_keys_with_options(
+        self,
+        request: resource_directory_master_20220419_models.ListTagKeysRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> resource_directory_master_20220419_models.ListTagKeysResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.key_filter):
+            query['KeyFilter'] = request.key_filter
+        if not UtilClient.is_unset(request.max_results):
+            query['MaxResults'] = request.max_results
+        if not UtilClient.is_unset(request.next_token):
+            query['NextToken'] = request.next_token
+        if not UtilClient.is_unset(request.resource_type):
+            query['ResourceType'] = request.resource_type
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListTagKeys',
+            version='2022-04-19',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            resource_directory_master_20220419_models.ListTagKeysResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def list_tag_keys_with_options_async(
+        self,
+        request: resource_directory_master_20220419_models.ListTagKeysRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> resource_directory_master_20220419_models.ListTagKeysResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.key_filter):
+            query['KeyFilter'] = request.key_filter
+        if not UtilClient.is_unset(request.max_results):
+            query['MaxResults'] = request.max_results
+        if not UtilClient.is_unset(request.next_token):
+            query['NextToken'] = request.next_token
+        if not UtilClient.is_unset(request.resource_type):
+            query['ResourceType'] = request.resource_type
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListTagKeys',
+            version='2022-04-19',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            resource_directory_master_20220419_models.ListTagKeysResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def list_tag_keys(
+        self,
+        request: resource_directory_master_20220419_models.ListTagKeysRequest,
+    ) -> resource_directory_master_20220419_models.ListTagKeysResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.list_tag_keys_with_options(request, runtime)
+
+    async def list_tag_keys_async(
+        self,
+        request: resource_directory_master_20220419_models.ListTagKeysRequest,
+    ) -> resource_directory_master_20220419_models.ListTagKeysResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.list_tag_keys_with_options_async(request, runtime)
+
     def list_tag_resources_with_options(
         self,
         request: resource_directory_master_20220419_models.ListTagResourcesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.ListTagResourcesResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -4191,14 +4269,100 @@
     async def list_tag_resources_async(
         self,
         request: resource_directory_master_20220419_models.ListTagResourcesRequest,
     ) -> resource_directory_master_20220419_models.ListTagResourcesResponse:
         runtime = util_models.RuntimeOptions()
         return await self.list_tag_resources_with_options_async(request, runtime)
 
+    def list_tag_values_with_options(
+        self,
+        request: resource_directory_master_20220419_models.ListTagValuesRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> resource_directory_master_20220419_models.ListTagValuesResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.max_results):
+            query['MaxResults'] = request.max_results
+        if not UtilClient.is_unset(request.next_token):
+            query['NextToken'] = request.next_token
+        if not UtilClient.is_unset(request.resource_type):
+            query['ResourceType'] = request.resource_type
+        if not UtilClient.is_unset(request.tag_key):
+            query['TagKey'] = request.tag_key
+        if not UtilClient.is_unset(request.value_filter):
+            query['ValueFilter'] = request.value_filter
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListTagValues',
+            version='2022-04-19',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            resource_directory_master_20220419_models.ListTagValuesResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def list_tag_values_with_options_async(
+        self,
+        request: resource_directory_master_20220419_models.ListTagValuesRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> resource_directory_master_20220419_models.ListTagValuesResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.max_results):
+            query['MaxResults'] = request.max_results
+        if not UtilClient.is_unset(request.next_token):
+            query['NextToken'] = request.next_token
+        if not UtilClient.is_unset(request.resource_type):
+            query['ResourceType'] = request.resource_type
+        if not UtilClient.is_unset(request.tag_key):
+            query['TagKey'] = request.tag_key
+        if not UtilClient.is_unset(request.value_filter):
+            query['ValueFilter'] = request.value_filter
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListTagValues',
+            version='2022-04-19',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            resource_directory_master_20220419_models.ListTagValuesResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def list_tag_values(
+        self,
+        request: resource_directory_master_20220419_models.ListTagValuesRequest,
+    ) -> resource_directory_master_20220419_models.ListTagValuesResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.list_tag_values_with_options(request, runtime)
+
+    async def list_tag_values_async(
+        self,
+        request: resource_directory_master_20220419_models.ListTagValuesRequest,
+    ) -> resource_directory_master_20220419_models.ListTagValuesResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.list_tag_values_with_options_async(request, runtime)
+
     def list_target_attachments_for_control_policy_with_options(
         self,
         request: resource_directory_master_20220419_models.ListTargetAttachmentsForControlPolicyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.ListTargetAttachmentsForControlPolicyResponse:
         UtilClient.validate_model(request)
         query = {}
```

### Comparing `alibabacloud_resourcedirectorymaster20220419-1.0.3/alibabacloud_resourcedirectorymaster20220419/models.py` & `alibabacloud_resourcedirectorymaster20220419-1.0.4/alibabacloud_resourcedirectorymaster20220419/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -243,14 +243,16 @@
         # 
         # The name must be 2 to 12 characters in length and can contain only letters.
         self.name = name
         # The mobile phone number of the contact.
         # 
         # Specify the mobile phone number in the `<Country code>-<Mobile phone number>` format.
         # 
+        # > Only mobile phone numbers in the `86-<Mobile phone number>` format in the Chinese mainland are supported.
+        # 
         # After you specify a mobile phone number, you need to call [SendPhoneVerificationForMessageContact](~~SendPhoneVerificationForMessageContact~~) to send verification information to the mobile phone number. After the verification is passed, the mobile phone number takes effect.
         self.phone_number = phone_number
         # The job title of the contact.
         # 
         # Valid values:
         # 
         # *   FinanceDirector
@@ -2482,15 +2484,15 @@
         self,
         deletion_type: str = None,
         request_id: str = None,
     ):
         # The type of the deletion. Valid values:
         # 
         # *   0: direct deletion. If the member does not have pay-as-you-go resources that are purchased within the previous 30 days, the system directly deletes the member.
-        # *   1: deletion with a silence period. If the member has pay-as-you-go resources that are purchased within the previous 30 days, the member enters a silence period of 45 days. The system starts to delete the member until the silence period ends. For more information about the silence period, see [What is the silence period for member deletion?](~~446079~~)
+        # *   1: deletion with a silence period. If the member has pay-as-you-go resources that are purchased within the previous 30 days, the member enters a silence period. The system starts to delete the member until the silence period ends. For more information about the silence period, see [What is the silence period for member deletion?](~~446079~~)
         self.deletion_type = deletion_type
         # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
@@ -5879,15 +5881,15 @@
     ):
         # The description of the invitation.
         # 
         # The description can be up to 1,024 characters in length.
         self.note = note
         # The ID of the parent folder.
         self.parent_folder_id = parent_folder_id
-        # The tag value.
+        # The tags.
         self.tag = tag
         # The ID or logon email address of the account that you want to invite.
         self.target_entity = target_entity
         # The type of the invited account. Valid values:
         # 
         # *   Account: indicates the ID of the account.
         # *   Email: indicates the logon email address of the account.
@@ -9370,14 +9372,177 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ListMessageContactsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ListTagKeysRequest(TeaModel):
+    def __init__(
+        self,
+        key_filter: str = None,
+        max_results: int = None,
+        next_token: str = None,
+        resource_type: str = None,
+    ):
+        self.key_filter = key_filter
+        self.max_results = max_results
+        self.next_token = next_token
+        self.resource_type = resource_type
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.key_filter is not None:
+            result['KeyFilter'] = self.key_filter
+        if self.max_results is not None:
+            result['MaxResults'] = self.max_results
+        if self.next_token is not None:
+            result['NextToken'] = self.next_token
+        if self.resource_type is not None:
+            result['ResourceType'] = self.resource_type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('KeyFilter') is not None:
+            self.key_filter = m.get('KeyFilter')
+        if m.get('MaxResults') is not None:
+            self.max_results = m.get('MaxResults')
+        if m.get('NextToken') is not None:
+            self.next_token = m.get('NextToken')
+        if m.get('ResourceType') is not None:
+            self.resource_type = m.get('ResourceType')
+        return self
+
+
+class ListTagKeysResponseBodyTags(TeaModel):
+    def __init__(
+        self,
+        key: str = None,
+    ):
+        self.key = key
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.key is not None:
+            result['Key'] = self.key
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Key') is not None:
+            self.key = m.get('Key')
+        return self
+
+
+class ListTagKeysResponseBody(TeaModel):
+    def __init__(
+        self,
+        next_token: str = None,
+        request_id: str = None,
+        tags: List[ListTagKeysResponseBodyTags] = None,
+    ):
+        self.next_token = next_token
+        self.request_id = request_id
+        self.tags = tags
+
+    def validate(self):
+        if self.tags:
+            for k in self.tags:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.next_token is not None:
+            result['NextToken'] = self.next_token
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        result['Tags'] = []
+        if self.tags is not None:
+            for k in self.tags:
+                result['Tags'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('NextToken') is not None:
+            self.next_token = m.get('NextToken')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        self.tags = []
+        if m.get('Tags') is not None:
+            for k in m.get('Tags'):
+                temp_model = ListTagKeysResponseBodyTags()
+                self.tags.append(temp_model.from_map(k))
+        return self
+
+
+class ListTagKeysResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ListTagKeysResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ListTagKeysResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class ListTagResourcesRequestTag(TeaModel):
     def __init__(
         self,
         key: str = None,
         value: str = None,
     ):
         # The key of the tag.
@@ -9625,14 +9790,183 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ListTagResourcesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ListTagValuesRequest(TeaModel):
+    def __init__(
+        self,
+        max_results: int = None,
+        next_token: str = None,
+        resource_type: str = None,
+        tag_key: str = None,
+        value_filter: str = None,
+    ):
+        self.max_results = max_results
+        self.next_token = next_token
+        self.resource_type = resource_type
+        self.tag_key = tag_key
+        self.value_filter = value_filter
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.max_results is not None:
+            result['MaxResults'] = self.max_results
+        if self.next_token is not None:
+            result['NextToken'] = self.next_token
+        if self.resource_type is not None:
+            result['ResourceType'] = self.resource_type
+        if self.tag_key is not None:
+            result['TagKey'] = self.tag_key
+        if self.value_filter is not None:
+            result['ValueFilter'] = self.value_filter
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('MaxResults') is not None:
+            self.max_results = m.get('MaxResults')
+        if m.get('NextToken') is not None:
+            self.next_token = m.get('NextToken')
+        if m.get('ResourceType') is not None:
+            self.resource_type = m.get('ResourceType')
+        if m.get('TagKey') is not None:
+            self.tag_key = m.get('TagKey')
+        if m.get('ValueFilter') is not None:
+            self.value_filter = m.get('ValueFilter')
+        return self
+
+
+class ListTagValuesResponseBodyTags(TeaModel):
+    def __init__(
+        self,
+        value: str = None,
+    ):
+        self.value = value
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.value is not None:
+            result['Value'] = self.value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
+class ListTagValuesResponseBody(TeaModel):
+    def __init__(
+        self,
+        next_token: str = None,
+        request_id: str = None,
+        tags: List[ListTagValuesResponseBodyTags] = None,
+    ):
+        self.next_token = next_token
+        self.request_id = request_id
+        self.tags = tags
+
+    def validate(self):
+        if self.tags:
+            for k in self.tags:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.next_token is not None:
+            result['NextToken'] = self.next_token
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        result['Tags'] = []
+        if self.tags is not None:
+            for k in self.tags:
+                result['Tags'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('NextToken') is not None:
+            self.next_token = m.get('NextToken')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        self.tags = []
+        if m.get('Tags') is not None:
+            for k in m.get('Tags'):
+                temp_model = ListTagValuesResponseBodyTags()
+                self.tags.append(temp_model.from_map(k))
+        return self
+
+
+class ListTagValuesResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ListTagValuesResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ListTagValuesResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class ListTargetAttachmentsForControlPolicyRequest(TeaModel):
     def __init__(
         self,
         page_number: int = None,
         page_size: int = None,
         policy_id: str = None,
     ):
```

### Comparing `alibabacloud_resourcedirectorymaster20220419-1.0.3/alibabacloud_resourcedirectorymaster20220419.egg-info/PKG-INFO` & `alibabacloud_resourcedirectorymaster20220419-1.0.4/alibabacloud_resourcedirectorymaster20220419.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-resourcedirectorymaster20220419
-Version: 1.0.3
+Version: 1.0.4
 Summary: Alibaba Cloud ResourceDirectoryMaster (20220419) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_resourcedirectorymaster20220419-1.0.3/alibabacloud_resourcedirectorymaster20220419.egg-info/SOURCES.txt` & `alibabacloud_resourcedirectorymaster20220419-1.0.4/alibabacloud_resourcedirectorymaster20220419.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud_resourcedirectorymaster20220419-1.0.3/setup.py` & `alibabacloud_resourcedirectorymaster20220419-1.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_resourcedirectorymaster20220419.
 
-Created on 26/07/2023
+Created on 06/08/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_resourcedirectorymaster20220419"
 NAME = "alibabacloud_resourcedirectorymaster20220419" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud ResourceDirectoryMaster (20220419) SDK Library for Python"
```

