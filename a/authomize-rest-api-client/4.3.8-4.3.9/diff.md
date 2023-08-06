# Comparing `tmp/authomize-rest-api-client-4.3.8.tar.gz` & `tmp/authomize-rest-api-client-4.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "authomize-rest-api-client-4.3.8.tar", last modified: Thu Aug  3 13:10:38 2023, max compression
+gzip compressed data, was "authomize-rest-api-client-4.3.9.tar", last modified: Sun Aug  6 08:47:41 2023, max compression
```

## Comparing `authomize-rest-api-client-4.3.8.tar` & `authomize-rest-api-client-4.3.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 13:10:38.459387 authomize-rest-api-client-4.3.8/
--rw-r--r--   0 root         (0) root         (0)     1072 2023-08-03 13:10:19.000000 authomize-rest-api-client-4.3.8/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      134 2023-08-03 13:10:19.000000 authomize-rest-api-client-4.3.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      251 2023-08-03 13:10:38.459387 authomize-rest-api-client-4.3.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2201 2023-08-03 13:10:19.000000 authomize-rest-api-client-4.3.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 13:10:38.459387 authomize-rest-api-client-4.3.8/authomize/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 13:10:38.459387 authomize-rest-api-client-4.3.8/authomize/rest_api_client/
--rw-r--r--   0 root         (0) root         (0)      627 2023-08-03 13:10:19.000000 authomize-rest-api-client-4.3.8/authomize/rest_api_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 13:10:38.459387 authomize-rest-api-client-4.3.8/authomize/rest_api_client/client/
--rw-r--r--   0 root         (0) root         (0)       81 2023-08-03 13:10:19.000000 authomize-rest-api-client-4.3.8/authomize/rest_api_client/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2566 2023-08-03 13:10:19.000000 authomize-rest-api-client-4.3.8/authomize/rest_api_client/client/base_client.py
--rw-r--r--   0 root         (0) root         (0)    10358 2023-08-03 13:10:19.000000 authomize-rest-api-client-4.3.8/authomize/rest_api_client/client/client.py
--rw-r--r--   0 root         (0) root         (0)    13027 2023-08-03 13:10:19.000000 authomize-rest-api-client-4.3.8/authomize/rest_api_client/client/connectors_client.py
--rw-r--r--   0 root         (0) root         (0)     1102 2023-08-03 13:10:19.000000 authomize-rest-api-client-4.3.8/authomize/rest_api_client/client/platform_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 13:10:38.459387 authomize-rest-api-client-4.3.8/authomize/rest_api_client/configuration/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 13:10:19.000000 authomize-rest-api-client-4.3.8/authomize/rest_api_client/configuration/__init__.py
--rw-r--r--   0 root         (0) root         (0)      330 2023-08-03 13:10:19.000000 authomize-rest-api-client-4.3.8/authomize/rest_api_client/configuration/authomize_api_configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 13:10:38.459387 authomize-rest-api-client-4.3.8/authomize/rest_api_client/generated/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 13:10:19.000000 authomize-rest-api-client-4.3.8/authomize/rest_api_client/generated/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 13:10:38.459387 authomize-rest-api-client-4.3.8/authomize/rest_api_client/generated/connectors_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 13:10:19.000000 authomize-rest-api-client-4.3.8/authomize/rest_api_client/generated/connectors_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    90538 2023-08-03 13:10:19.000000 authomize-rest-api-client-4.3.8/authomize/rest_api_client/generated/connectors_rest_api/schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 13:10:38.459387 authomize-rest-api-client-4.3.8/authomize/rest_api_client/generated/external_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 13:10:19.000000 authomize-rest-api-client-4.3.8/authomize/rest_api_client/generated/external_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    49496 2023-08-03 13:10:19.000000 authomize-rest-api-client-4.3.8/authomize/rest_api_client/generated/external_rest_api/schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 13:10:38.459387 authomize-rest-api-client-4.3.8/authomize/rest_api_client/openapi/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 13:10:19.000000 authomize-rest-api-client-4.3.8/authomize/rest_api_client/openapi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 13:10:38.459387 authomize-rest-api-client-4.3.8/authomize/rest_api_client/openapi/connectors_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 13:10:19.000000 authomize-rest-api-client-4.3.8/authomize/rest_api_client/openapi/connectors_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)   210449 2023-08-03 13:10:19.000000 authomize-rest-api-client-4.3.8/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 13:10:38.459387 authomize-rest-api-client-4.3.8/authomize/rest_api_client/openapi/external_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 13:10:19.000000 authomize-rest-api-client-4.3.8/authomize/rest_api_client/openapi/external_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)   115488 2023-08-03 13:10:19.000000 authomize-rest-api-client-4.3.8/authomize/rest_api_client/openapi/external_rest_api/openapi.json
--rw-r--r--   0 root         (0) root         (0)       26 2023-08-03 13:10:19.000000 authomize-rest-api-client-4.3.8/authomize/rest_api_client/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 13:10:38.459387 authomize-rest-api-client-4.3.8/authomize_rest_api_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)      251 2023-08-03 13:10:38.000000 authomize-rest-api-client-4.3.8/authomize_rest_api_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1356 2023-08-03 13:10:38.000000 authomize-rest-api-client-4.3.8/authomize_rest_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 13:10:38.000000 authomize-rest-api-client-4.3.8/authomize_rest_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      189 2023-08-03 13:10:38.000000 authomize-rest-api-client-4.3.8/authomize_rest_api_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-08-03 13:10:38.000000 authomize-rest-api-client-4.3.8/authomize_rest_api_client.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      336 2023-08-03 13:10:38.459387 authomize-rest-api-client-4.3.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1117 2023-08-03 13:10:22.000000 authomize-rest-api-client-4.3.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 08:47:41.561026 authomize-rest-api-client-4.3.9/
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-08-06 08:47:19.000000 authomize-rest-api-client-4.3.9/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      134 2023-08-06 08:47:19.000000 authomize-rest-api-client-4.3.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      251 2023-08-06 08:47:41.561026 authomize-rest-api-client-4.3.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2201 2023-08-06 08:47:19.000000 authomize-rest-api-client-4.3.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 08:47:41.557026 authomize-rest-api-client-4.3.9/authomize/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 08:47:41.557026 authomize-rest-api-client-4.3.9/authomize/rest_api_client/
+-rw-r--r--   0 root         (0) root         (0)      627 2023-08-06 08:47:19.000000 authomize-rest-api-client-4.3.9/authomize/rest_api_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 08:47:41.561026 authomize-rest-api-client-4.3.9/authomize/rest_api_client/client/
+-rw-r--r--   0 root         (0) root         (0)       81 2023-08-06 08:47:19.000000 authomize-rest-api-client-4.3.9/authomize/rest_api_client/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2566 2023-08-06 08:47:19.000000 authomize-rest-api-client-4.3.9/authomize/rest_api_client/client/base_client.py
+-rw-r--r--   0 root         (0) root         (0)    10675 2023-08-06 08:47:19.000000 authomize-rest-api-client-4.3.9/authomize/rest_api_client/client/client.py
+-rw-r--r--   0 root         (0) root         (0)    13450 2023-08-06 08:47:19.000000 authomize-rest-api-client-4.3.9/authomize/rest_api_client/client/connectors_client.py
+-rw-r--r--   0 root         (0) root         (0)     1102 2023-08-06 08:47:19.000000 authomize-rest-api-client-4.3.9/authomize/rest_api_client/client/platform_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 08:47:41.561026 authomize-rest-api-client-4.3.9/authomize/rest_api_client/configuration/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-06 08:47:19.000000 authomize-rest-api-client-4.3.9/authomize/rest_api_client/configuration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      330 2023-08-06 08:47:19.000000 authomize-rest-api-client-4.3.9/authomize/rest_api_client/configuration/authomize_api_configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 08:47:41.561026 authomize-rest-api-client-4.3.9/authomize/rest_api_client/generated/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-06 08:47:19.000000 authomize-rest-api-client-4.3.9/authomize/rest_api_client/generated/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 08:47:41.561026 authomize-rest-api-client-4.3.9/authomize/rest_api_client/generated/connectors_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-06 08:47:19.000000 authomize-rest-api-client-4.3.9/authomize/rest_api_client/generated/connectors_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    90538 2023-08-06 08:47:19.000000 authomize-rest-api-client-4.3.9/authomize/rest_api_client/generated/connectors_rest_api/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 08:47:41.561026 authomize-rest-api-client-4.3.9/authomize/rest_api_client/generated/external_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-06 08:47:19.000000 authomize-rest-api-client-4.3.9/authomize/rest_api_client/generated/external_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    48660 2023-08-06 08:47:19.000000 authomize-rest-api-client-4.3.9/authomize/rest_api_client/generated/external_rest_api/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 08:47:41.561026 authomize-rest-api-client-4.3.9/authomize/rest_api_client/openapi/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-06 08:47:19.000000 authomize-rest-api-client-4.3.9/authomize/rest_api_client/openapi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 08:47:41.561026 authomize-rest-api-client-4.3.9/authomize/rest_api_client/openapi/connectors_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-06 08:47:19.000000 authomize-rest-api-client-4.3.9/authomize/rest_api_client/openapi/connectors_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   210449 2023-08-06 08:47:19.000000 authomize-rest-api-client-4.3.9/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 08:47:41.561026 authomize-rest-api-client-4.3.9/authomize/rest_api_client/openapi/external_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-06 08:47:19.000000 authomize-rest-api-client-4.3.9/authomize/rest_api_client/openapi/external_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   115692 2023-08-06 08:47:19.000000 authomize-rest-api-client-4.3.9/authomize/rest_api_client/openapi/external_rest_api/openapi.json
+-rw-r--r--   0 root         (0) root         (0)       26 2023-08-06 08:47:19.000000 authomize-rest-api-client-4.3.9/authomize/rest_api_client/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 08:47:41.561026 authomize-rest-api-client-4.3.9/authomize_rest_api_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      251 2023-08-06 08:47:41.000000 authomize-rest-api-client-4.3.9/authomize_rest_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1356 2023-08-06 08:47:41.000000 authomize-rest-api-client-4.3.9/authomize_rest_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-06 08:47:41.000000 authomize-rest-api-client-4.3.9/authomize_rest_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      189 2023-08-06 08:47:41.000000 authomize-rest-api-client-4.3.9/authomize_rest_api_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-08-06 08:47:41.000000 authomize-rest-api-client-4.3.9/authomize_rest_api_client.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      336 2023-08-06 08:47:41.561026 authomize-rest-api-client-4.3.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1117 2023-08-06 08:47:23.000000 authomize-rest-api-client-4.3.9/setup.py
```

### Comparing `authomize-rest-api-client-4.3.8/LICENSE.txt` & `authomize-rest-api-client-4.3.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.8/README.md` & `authomize-rest-api-client-4.3.9/README.md`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.8/authomize/rest_api_client/__init__.py` & `authomize-rest-api-client-4.3.9/authomize/rest_api_client/__init__.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.8/authomize/rest_api_client/client/base_client.py` & `authomize-rest-api-client-4.3.9/authomize/rest_api_client/client/base_client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.8/authomize/rest_api_client/client/client.py` & `authomize-rest-api-client-4.3.9/authomize/rest_api_client/client/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,16 @@
     ItemsBundleSchema,
     NewAccountsAssociationResponseSchema,
     NewAccountsAssociationsListRequestSchema,
     NewAssetsInheritanceListRequestSchema,
     NewAssetsInheritanceResponseSchema,
     NewAssetsListRequestSchema,
     NewAssetsResponseSchema,
+    NewGitRepoListRequestSchema,
+    NewGitRepoResponseSchema,
     NewGroupingResponseSchema,
     NewGroupingsAssociationResponseSchema,
     NewGroupingsAssociationsListRequestSchema,
     NewGroupingsListRequestSchema,
     NewIdentitiesListRequestSchema,
     NewIdentityResponseSchema,
     NewPermissionsListRequestSchema,
@@ -304,14 +306,24 @@
         body: NewAssetsListRequestSchema,
     ) -> NewAssetsResponseSchema:
         return self.connectors_client.create_assets(
             app_id=app_id,
             body=body,
         )
 
+    def create_git_repo(
+        self,
+        app_id: str,
+        body: NewGitRepoListRequestSchema,
+    ) -> NewGitRepoResponseSchema:
+        return self.connectors_client.create_git_repo(
+            app_id=app_id,
+            body=body,
+        )
+
     def search_assets_inheritance(
         self,
         app_id: str,
         start_date: Optional[datetime] = None,
     ) -> SearchAssetsInheritanceListResponseSchema:
         return self.connectors_client.search_assets_inheritance(
             app_id=app_id,
```

### Comparing `authomize-rest-api-client-4.3.8/authomize/rest_api_client/client/connectors_client.py` & `authomize-rest-api-client-4.3.9/authomize/rest_api_client/client/connectors_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,16 @@
     ItemsBundleSchema,
     NewAccountsAssociationResponseSchema,
     NewAccountsAssociationsListRequestSchema,
     NewAssetsInheritanceListRequestSchema,
     NewAssetsInheritanceResponseSchema,
     NewAssetsListRequestSchema,
     NewAssetsResponseSchema,
+    NewGitRepoListRequestSchema,
+    NewGitRepoResponseSchema,
     NewGroupingResponseSchema,
     NewGroupingsAssociationResponseSchema,
     NewGroupingsAssociationsListRequestSchema,
     NewGroupingsListRequestSchema,
     NewIdentitiesListRequestSchema,
     NewIdentityResponseSchema,
     NewPermissionsListRequestSchema,
@@ -119,19 +121,15 @@
         self,
         app_id: str,
         body: UpdateAppSchema,
     ) -> SubmitResponse:
         if not app_id:
             raise ValueError('Missing app_id')
         return self.http_patch(
-            url=f"/v2/apps/{app_id}",
-            body=json.dumps(
-                body,
-                default=pydantic_encoder
-            )
+            url=f"/v2/apps/{app_id}", body=json.dumps(body, default=pydantic_encoder)
         )
 
     def search_users(
         self,
         app_id: str,
         start_date: Optional[datetime] = None,
     ) -> SearchUsersListResponseSchema:
@@ -382,14 +380,29 @@
             url=f'/v2/apps/{app_id}/assets',
             body=json.dumps(
                 body,
                 default=pydantic_encoder,
             ),
         )
 
+    def create_git_repo(
+        self,
+        app_id: str,
+        body: NewGitRepoListRequestSchema,
+    ) -> NewGitRepoResponseSchema:
+        if not app_id:
+            raise ValueError('Missing app_id')
+        return self.http_post(
+            url=f'/v2/apps/{app_id}/assets/git-repository',
+            body=json.dumps(
+                body,
+                default=pydantic_encoder,
+            ),
+        )
+
     def search_assets_inheritance(
         self,
         app_id: str,
         start_date: Optional[datetime] = None,
     ) -> SearchAssetsInheritanceListResponseSchema:
         if not app_id:
             raise ValueError('Missing app_id')
```

### Comparing `authomize-rest-api-client-4.3.8/authomize/rest_api_client/client/platform_client.py` & `authomize-rest-api-client-4.3.9/authomize/rest_api_client/client/platform_client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.8/authomize/rest_api_client/generated/connectors_rest_api/schemas.py` & `authomize-rest-api-client-4.3.9/authomize/rest_api_client/generated/connectors_rest_api/schemas.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.8/authomize/rest_api_client/generated/external_rest_api/schemas.py` & `authomize-rest-api-client-4.3.9/authomize/rest_api_client/generated/external_rest_api/schemas.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  openapi.json
-#   timestamp: 2023-07-26T10:45:11+00:00
+#   timestamp: 2023-08-03T14:01:37+00:00
 
 from __future__ import annotations
 
 from datetime import datetime
 from enum import Enum
 from typing import List, Optional, Union
 
@@ -87,31 +87,27 @@
     Account_Impersonation__PE__LM_ = 'Account Impersonation (PE, LM)'
 
 
 class AppIdFilter(BaseModel):
     class Config:
         extra = Extra.forbid
 
-    field_eq: Optional[str] = Field(
-        default=None, alias='$eq', description='Equals To', title='$Eq'
-    )
+    field_eq: Optional[str] = Field(default=None, alias='$eq', description='Equals To', title='$Eq')
 
 
 class AssetExpansion(Enum):
     sourceApp = 'sourceApp'
     tags = 'tags'
 
 
 class AssetIdFilter(BaseModel):
     class Config:
         extra = Extra.forbid
 
-    field_in: Optional[List[str]] = Field(
-        default=[], alias='$in', description='In', title='$In'
-    )
+    field_in: Optional[List[str]] = Field(default=[], alias='$in', description='In', title='$In')
 
 
 class AttackTacticType(Enum):
     Collection = 'Collection'
     Credential_Access = 'Credential Access'
     Defense_Evasion = 'Defense Evasion'
     Discovery = 'Discovery'
@@ -137,17 +133,15 @@
     overdue = 'overdue'
 
 
 class CampaignStatusFilter(BaseModel):
     class Config:
         extra = Extra.forbid
 
-    field_in: Optional[List[CampaignStatus]] = Field(
-        default=[], alias='$in', description='In'
-    )
+    field_in: Optional[List[CampaignStatus]] = Field(default=[], alias='$in', description='In')
 
 
 class Ccm301Standard(Enum):
     AIS_04 = 'AIS-04'
     IAM_01 = 'IAM-01'
     IAM_02 = 'IAM-02'
     IAM_03 = 'IAM-03'
@@ -229,17 +223,15 @@
     )
 
 
 class EmailFilter(BaseModel):
     class Config:
         extra = Extra.forbid
 
-    field_in: Optional[List[str]] = Field(
-        default=[], alias='$in', description='In', title='$In'
-    )
+    field_in: Optional[List[str]] = Field(default=[], alias='$in', description='In', title='$In')
 
 
 class EventStatusType(Enum):
     Open = 'Open'
     InProgress = 'InProgress'
     WaitingForInput = 'WaitingForInput'
     Closed = 'Closed'
@@ -277,17 +269,15 @@
     )
 
 
 class IdFilter(BaseModel):
     class Config:
         extra = Extra.forbid
 
-    field_in: Optional[List[str]] = Field(
-        default=[], alias='$in', description='In', title='$In'
-    )
+    field_in: Optional[List[str]] = Field(default=[], alias='$in', description='In', title='$In')
 
 
 class IdentityExpansion(Enum):
     account = 'account'
     tags = 'tags'
 
 
@@ -340,35 +330,29 @@
     )
 
 
 class IncidentsPolicyIdFilter(BaseModel):
     class Config:
         extra = Extra.forbid
 
-    field_eq: Optional[str] = Field(
-        default=None, alias='$eq', description='Equals To', title='$Eq'
-    )
+    field_eq: Optional[str] = Field(default=None, alias='$eq', description='Equals To', title='$Eq')
 
 
 class IncidentsPolicyTempalteIdFilter(BaseModel):
     class Config:
         extra = Extra.forbid
 
-    field_eq: Optional[str] = Field(
-        default=None, alias='$eq', description='Equals To', title='$Eq'
-    )
+    field_eq: Optional[str] = Field(default=None, alias='$eq', description='Equals To', title='$Eq')
 
 
 class IncidentsStatusFilter(BaseModel):
     class Config:
         extra = Extra.forbid
 
-    field_in: Optional[List[EventStatusType]] = Field(
-        default=[], alias='$in', description='In'
-    )
+    field_in: Optional[List[EventStatusType]] = Field(default=[], alias='$in', description='In')
 
 
 class IncidentsUpdatedAtFilter(BaseModel):
     class Config:
         extra = Extra.forbid
 
     field_lte: Optional[datetime] = Field(
@@ -419,17 +403,15 @@
     A_9_4_5 = 'A.9.4.5'
     A_8_2_3 = 'A.8.2.3'
     A_7_3_1 = 'A.7.3.1'
     A_8_1_4 = 'A.8.1.4'
 
 
 class MeResponse(BaseModel):
-    version: Optional[str] = Field(
-        default='4.3.0', description='**version**', title='Version'
-    )
+    version: Optional[str] = Field(default='4.3.7', description='**version**', title='Version')
     id: str = Field(..., description='**id**', title='Id')
     tenant: str = Field(..., description='**tenant**', title='Tenant')
 
 
 class NonPaginatedResponseSchemaCommentSchema(BaseModel):
     class Config:
         extra = Extra.forbid
@@ -441,17 +423,15 @@
     ok: Optional[bool] = Field(default=True, description='OK\n', title='Ok')
 
 
 class OriginIdFilter(BaseModel):
     class Config:
         extra = Extra.forbid
 
-    field_in: Optional[List[str]] = Field(
-        default=[], alias='$in', description='In', title='$In'
-    )
+    field_in: Optional[List[str]] = Field(default=[], alias='$in', description='In', title='$In')
 
 
 class PaginationRequestSchema(BaseModel):
     class Config:
         extra = Extra.forbid
 
     limit: Optional[int] = Field(
@@ -526,74 +506,62 @@
     )
 
 
 class SearchAccountsIdFilter(BaseModel):
     class Config:
         extra = Extra.forbid
 
-    field_in: Optional[List[str]] = Field(
-        default=[], alias='$in', description='In', title='$In'
-    )
+    field_in: Optional[List[str]] = Field(default=[], alias='$in', description='In', title='$In')
 
 
 class SearchAccountsOriginIdFilter(BaseModel):
     class Config:
         extra = Extra.forbid
 
-    field_in: Optional[List[str]] = Field(
-        default=[], alias='$in', description='In', title='$In'
-    )
+    field_in: Optional[List[str]] = Field(default=[], alias='$in', description='In', title='$In')
 
 
 class SearchAccountsSortFields(Enum):
     account_name = 'account.name'
 
 
 class SearchAssetsSortFields(Enum):
     asset_name = 'asset.name'
 
 
 class SearchGroupsAppIdFilter(BaseModel):
     class Config:
         extra = Extra.forbid
 
-    field_eq: Optional[str] = Field(
-        default=None, alias='$eq', description='Equals To', title='$Eq'
-    )
+    field_eq: Optional[str] = Field(default=None, alias='$eq', description='Equals To', title='$Eq')
 
 
 class SearchGroupsIdFilter(BaseModel):
     class Config:
         extra = Extra.forbid
 
-    field_in: Optional[List[str]] = Field(
-        default=[], alias='$in', description='In', title='$In'
-    )
+    field_in: Optional[List[str]] = Field(default=[], alias='$in', description='In', title='$In')
 
 
 class SearchGroupsOriginIdFilter(BaseModel):
     class Config:
         extra = Extra.forbid
 
-    field_in: Optional[List[str]] = Field(
-        default=[], alias='$in', description='In', title='$In'
-    )
+    field_in: Optional[List[str]] = Field(default=[], alias='$in', description='In', title='$In')
 
 
 class SearchGroupsSortFields(Enum):
     group_name = 'group.name'
 
 
 class SearchGroupsUniqueIdFilter(BaseModel):
     class Config:
         extra = Extra.forbid
 
-    field_in: Optional[List[str]] = Field(
-        default=[], alias='$in', description='In', title='$In'
-    )
+    field_in: Optional[List[str]] = Field(default=[], alias='$in', description='In', title='$In')
 
 
 class SearchIdentitiesFilterBody(BaseModel):
     class Config:
         extra = Extra.forbid
 
     email: Optional[EmailFilter] = Field(
@@ -738,17 +706,15 @@
     )
 
 
 class UniqueIdFilter(BaseModel):
     class Config:
         extra = Extra.forbid
 
-    field_in: Optional[List[str]] = Field(
-        default=[], alias='$in', description='In', title='$In'
-    )
+    field_in: Optional[List[str]] = Field(default=[], alias='$in', description='In', title='$In')
 
 
 class UpdateIncidentRequestSchema(BaseModel):
     class Config:
         extra = Extra.forbid
 
     assigneeId: Optional[str] = Field(
@@ -764,20 +730,16 @@
         default=None,
         description='The severity of the incident (Low, Medium, High or Critical).',
     )
 
 
 class UserSchema(BaseModel):
     id: str = Field(..., description='Unique ID', title='Id')
-    firstName: Optional[str] = Field(
-        default=None, description='First Name', title='Firstname'
-    )
-    lastName: Optional[str] = Field(
-        default=None, description='Last Name', title='Lastname'
-    )
+    firstName: Optional[str] = Field(default=None, description='First Name', title='Firstname')
+    lastName: Optional[str] = Field(default=None, description='Last Name', title='Lastname')
     email: Optional[str] = Field(default=None, description='Email', title='Email')
 
 
 class UserStatus(Enum):
     Deleted = 'Deleted'
     Disabled = 'Disabled'
     Enabled = 'Enabled'
@@ -802,20 +764,16 @@
     risks: List[RiskFactorIn] = Field(
         ..., description='List of risks to add to the identity', title='Risks'
     )
 
 
 class AicpaTsc2017(BaseModel):
     values: List[AicpaTsc2017Standard] = Field(..., description='Values')
-    id: Optional[str] = Field(
-        default='aicpaTsc2017', description='UniqueID', title='Id'
-    )
-    name: Optional[str] = Field(
-        default='SOC 2 (TSC 2017)', description='Name', title='Name'
-    )
+    id: Optional[str] = Field(default='aicpaTsc2017', description='UniqueID', title='Id')
+    name: Optional[str] = Field(default='SOC 2 (TSC 2017)', description='Name', title='Name')
 
 
 class AssetSchema(BaseModel):
     authomizeId: str = Field(
         ..., description='Authomize ID of source application', title='Authomizeid'
     )
     name: Optional[str] = Field(
@@ -859,30 +817,28 @@
         description='The ID of the asset on the source system',
         title='Originid',
     )
     description: Optional[str] = Field(
         default=None, description='A description of the asset', title='Description'
     )
     tags: Optional[List[TagSchema]] = Field(
-        default=None, description='List of tags associated with the asset', title='Tags'
+        default=[], description='List of tags associated with the asset', title='Tags'
     )
     incidentsCount: Optional[int] = Field(
         default=None,
         description='Number of associated incidents',
         title='Incidentscount',
     )
 
 
 class CampaignPermissionDecisionFilter(BaseModel):
     class Config:
         extra = Extra.forbid
 
-    field_in: Optional[List[Selection]] = Field(
-        default=[], alias='$in', description='In'
-    )
+    field_in: Optional[List[Selection]] = Field(default=[], alias='$in', description='In')
 
 
 class CampaignPermissionsSearchFilterBody(BaseModel):
     class Config:
         extra = Extra.forbid
 
     decision: Optional[CampaignPermissionDecisionFilter] = Field(
@@ -892,26 +848,18 @@
     )
 
 
 class CampaignSchema(BaseModel):
     id: str = Field(..., description='Unique ID of campaign', title='Id')
     name: str = Field(..., description='Name of the campaign', title='Name')
     status: CampaignStatus = Field(..., description='The campaign status')
-    startDate: datetime = Field(
-        ..., description='Date when the campaign starts', title='Startdate'
-    )
-    endDate: datetime = Field(
-        ..., description='Date when campaign ends', title='Enddate'
-    )
-    createdAt: datetime = Field(
-        ..., description='Time of creation of campaign', title='Createdat'
-    )
-    ownerUserId: str = Field(
-        ..., description='User ID of the campaign owner', title='Owneruserid'
-    )
+    startDate: datetime = Field(..., description='Date when the campaign starts', title='Startdate')
+    endDate: datetime = Field(..., description='Date when campaign ends', title='Enddate')
+    createdAt: datetime = Field(..., description='Time of creation of campaign', title='Createdat')
+    ownerUserId: str = Field(..., description='User ID of the campaign owner', title='Owneruserid')
     owner: Optional[UserSchema] = Field(
         default=None, description='User Schema of the campaign owner', title='Owner'
     )
 
 
 class CampaignSearchFilterBody(BaseModel):
     class Config:
@@ -923,44 +871,34 @@
         title='Status',
     )
 
 
 class Ccm301(BaseModel):
     values: List[Ccm301Standard] = Field(..., description='Values')
     id: Optional[str] = Field(default='ccm301', description='UniqueID', title='Id')
-    name: Optional[str] = Field(
-        default='CSA STAR (CCM 3.0.1)', description='Name', title='Name'
-    )
+    name: Optional[str] = Field(default='CSA STAR (CCM 3.0.1)', description='Name', title='Name')
 
 
 class Ccm402(BaseModel):
     values: List[Ccm402Standard] = Field(..., description='Values')
     id: Optional[str] = Field(default='ccm402', description='UniqueID', title='Id')
-    name: Optional[str] = Field(
-        default='CSA STAR (CCM 4.0.2)', description='Name', title='Name'
-    )
+    name: Optional[str] = Field(default='CSA STAR (CCM 4.0.2)', description='Name', title='Name')
 
 
 class GroupSchema(BaseModel):
-    authomizeId: str = Field(
-        ..., description='Authomize ID of the Group.', title='Authomizeid'
-    )
-    name: Optional[str] = Field(
-        default=None, description='Name of the Group.', title='Name'
-    )
-    type: Optional[str] = Field(
-        default=None, description='Type of the group.', title='Type'
-    )
+    authomizeId: str = Field(..., description='Authomize ID of the Group.', title='Authomizeid')
+    name: Optional[str] = Field(default=None, description='Name of the Group.', title='Name')
+    type: Optional[str] = Field(default=None, description='Type of the group.', title='Type')
     incidentsCount: Optional[int] = Field(
         default=None,
         description='Number of incidents associated with the group.',
         title='Incidentscount',
     )
     tags: Optional[List[TagSchema]] = Field(
-        default=None, description='List of tags associated with the group', title='Tags'
+        default=[], description='List of tags associated with the group', title='Tags'
     )
     members: Optional[List[GroupMembership]] = Field(
         default=[],
         description='Entities that have direct access to the group.',
         title='Members',
     )
     sourceApp: Optional[SourceAppSchema] = Field(
@@ -976,62 +914,52 @@
     )
     uniqueId: Optional[str] = Field(
         default=None,
         description='The unique ID of the group (as provided by the connector)',
         title='Uniqueid',
     )
     createdAt: Optional[str] = Field(
-        default=None,
-        description='Type of the group in source system.',
-        title='Createdat',
+        default=None, description='Date when group was created.', title='Createdat'
     )
     originType: Optional[str] = Field(
-        default=None, description='Date when group was created.', title='Origintype'
+        default=None,
+        description='Type of the group in source system.',
+        title='Origintype',
     )
 
 
 class HTTPValidationError(BaseModel):
     detail: Optional[List[ValidationError]] = Field(default=None, title='Detail')
 
 
 class IncidentEntitiesSchema(BaseModel):
     id: str = Field(..., description='Unique id of entity.', title='Id')
-    name: Optional[str] = Field(
-        default=None, description='Name of entity.', title='Name'
-    )
+    name: Optional[str] = Field(default=None, description='Name of entity.', title='Name')
     object: Union[InventoryObjects, str] = Field(
         ..., description='Identity | Account | Asset', title='Object'
     )
     email: Optional[str] = Field(default=None, description='Email', title='Email')
-    originId: Optional[str] = Field(
-        default=None, description='Origin ID', title='Originid'
-    )
-    originType: Optional[str] = Field(
-        default=None, description='Origin Type', title='Origintype'
-    )
+    originId: Optional[str] = Field(default=None, description='Origin ID', title='Originid')
+    originType: Optional[str] = Field(default=None, description='Origin Type', title='Origintype')
     riskScore: Optional[IdentityRiskScore] = Field(
         default=None, description='Risk Scores', title='Riskscore'
     )
 
 
 class IncidentsSeverityFilter(BaseModel):
     class Config:
         extra = Extra.forbid
 
-    field_in: Optional[List[SeverityType]] = Field(
-        default=[], alias='$in', description='In'
-    )
+    field_in: Optional[List[SeverityType]] = Field(default=[], alias='$in', description='In')
 
 
 class IsoIec27001(BaseModel):
     values: List[IsoIec27001Standard] = Field(..., description='Values')
     id: Optional[str] = Field(default='isoIec27001', description='UniqueID', title='Id')
-    name: Optional[str] = Field(
-        default='ISO/IEC 27001', description='Name', title='Name'
-    )
+    name: Optional[str] = Field(default='ISO/IEC 27001', description='Name', title='Name')
 
 
 class NonPaginatedResponseSchemaCampaignSchema(BaseModel):
     class Config:
         extra = Extra.forbid
 
     data: CampaignSchema = Field(..., description='Actual Data', title='Data')
@@ -1040,73 +968,61 @@
 class PaginatedResponseSchemaAssetSchema(BaseModel):
     class Config:
         extra = Extra.forbid
 
     pagination: Optional[PaginationResponseSchema] = Field(
         default=None, description='Pagination Metadata', title='Pagination'
     )
-    data: List[AssetSchema] = Field(
-        ..., description='List of Actual Data', title='Data'
-    )
+    data: List[AssetSchema] = Field(..., description='List of Actual Data', title='Data')
 
 
 class PaginatedResponseSchemaCampaignSchema(BaseModel):
     class Config:
         extra = Extra.forbid
 
     pagination: Optional[PaginationResponseSchema] = Field(
         default=None, description='Pagination Metadata', title='Pagination'
     )
-    data: List[CampaignSchema] = Field(
-        ..., description='List of Actual Data', title='Data'
-    )
+    data: List[CampaignSchema] = Field(..., description='List of Actual Data', title='Data')
 
 
 class PaginatedResponseSchemaGroupSchema(BaseModel):
     class Config:
         extra = Extra.forbid
 
     pagination: Optional[PaginationResponseSchema] = Field(
         default=None, description='Pagination Metadata', title='Pagination'
     )
-    data: List[GroupSchema] = Field(
-        ..., description='List of Actual Data', title='Data'
-    )
+    data: List[GroupSchema] = Field(..., description='List of Actual Data', title='Data')
 
 
 class RawIdentitySchema(BaseModel):
     authomizeId: str = Field(..., description='Unique ID', title='Authomizeid')
-    name: Optional[str] = Field(
-        default=None, description='Name of the identity', title='Name'
-    )
-    title: Optional[str] = Field(
-        default=None, description='Title of the identity', title='Title'
-    )
+    name: Optional[str] = Field(default=None, description='Name of the identity', title='Name')
+    title: Optional[str] = Field(default=None, description='Title of the identity', title='Title')
     department: Optional[str] = Field(
         default=None,
         description='The department in which the identity works',
         title='Department',
     )
     accountIds: Optional[List[str]] = Field(
         default=[],
         description='The account IDs associated with the identity',
         title='Accountids',
     )
     email: Optional[str] = Field(
         default=None, description='The email of the identity', title='Email'
     )
     tags: Optional[List[TagSchema]] = Field(
-        default=None, description='The tags provided for the identity', title='Tags'
+        default=[], description='The tags provided for the identity', title='Tags'
     )
     terminatedAt: Optional[str] = Field(
         default=None, description='Time of termination', title='Terminatedat'
     )
-    hiredAt: Optional[str] = Field(
-        default=None, description='Hired At', title='Hiredat'
-    )
+    hiredAt: Optional[str] = Field(default=None, description='Hired At', title='Hiredat')
     incidentsCount: Optional[int] = Field(
         default=None,
         description='Number of associated incidents',
         title='Incidentscount',
     )
 
 
@@ -1127,17 +1043,15 @@
 
 class ReviewerSchema(BaseModel):
     userId: str = Field(..., description='User ID of the Reviewer', title='Userid')
     campaignId: str = Field(..., description='Campaign ID', title='Campaignid')
     lastNotifiedAt: datetime = Field(
         ..., description='Time of last notified', title='Lastnotifiedat'
     )
-    lastActiveAt: datetime = Field(
-        ..., description='Time of last activity', title='Lastactiveat'
-    )
+    lastActiveAt: datetime = Field(..., description='Time of last activity', title='Lastactiveat')
     reviewStatus: Union[ReviewStatus, str] = Field(
         ..., description='Review Status', title='Reviewstatus'
     )
     id: str = Field(..., description='Unique ID', title='Id')
     user: Optional[UserSchema] = Field(
         default=None, description='User Schema of the reviewer', title='User'
     )
@@ -1162,17 +1076,15 @@
 class SearchAccountsRequestSchema(BaseModel):
     class Config:
         extra = Extra.forbid
 
     pagination: Optional[PaginationRequestSchema] = Field(
         default=None, description='Pagination metadata', title='Pagination'
     )
-    expand: Optional[List[AccountExpansion]] = Field(
-        default=None, description='Expand Fields'
-    )
+    expand: Optional[List[AccountExpansion]] = Field(default=None, description='Expand Fields')
     sort: Optional[List[SortSchemaSearchAccountsSortFields]] = Field(
         default=None,
         description='Sort the results by account fields in ascending or descending order',
         title='Sort',
     )
     filter: Optional[SearchAccountsFilterBody] = Field(
         default=None, description='Search Accounts Filter', title='Filter'
@@ -1239,17 +1151,15 @@
 class SearchCampaignsRequestSchema(BaseModel):
     class Config:
         extra = Extra.forbid
 
     filter: Optional[CampaignSearchFilterBody] = Field(
         default=None, description='Status filter', title='Filter'
     )
-    expand: Optional[List[CampaignExpansion]] = Field(
-        default=None, description='Expand Fields'
-    )
+    expand: Optional[List[CampaignExpansion]] = Field(default=None, description='Expand Fields')
     pagination: Optional[PaginationRequestSchema] = Field(
         default=None, description='Pagination metadata', title='Pagination'
     )
     sort: Optional[List[SortSchemaFieldName]] = Field(
         default=None,
         description='Sort the results by campaign fields in ascending or descending order',
         title='Sort',
@@ -1349,48 +1259,40 @@
 class SearchIncidentsRequestSchema(BaseModel):
     class Config:
         extra = Extra.forbid
 
     filter: Optional[SearchIncidentsFilter] = Field(
         default=None, description='Filter', title='Filter'
     )
-    expand: Optional[List[IncidentExpansion]] = Field(
-        default=None, description='Expend'
-    )
+    expand: Optional[List[IncidentExpansion]] = Field(default=None, description='Expend')
     sort: Optional[List[SortSchemaSearchIncidentsSortFields]] = Field(
         default=None,
         description='Sort the results by incident fields in ascending or descending order',
         title='Sort',
     )
     pagination: Optional[PaginationRequestSchema] = Field(
         default=None, description='Pagination metadata', title='Pagination'
     )
 
 
 class AccountSchema(BaseModel):
-    authomizeId: str = Field(
-        ..., description='Authomize ID of the account', title='Authomizeid'
-    )
+    authomizeId: str = Field(..., description='Authomize ID of the account', title='Authomizeid')
     originId: Optional[str] = Field(
         default=None,
         description='The identifier of the account from the source system.',
         title='Originid',
     )
     uniqueId: Optional[str] = Field(
         default=None,
         description='Unique ID is an identifier coming from the connector that is unique across all accounts coming from that connector',
         title='Uniqueid',
     )
-    name: Optional[str] = Field(
-        default=None, description='Name of account', title='Name'
-    )
+    name: Optional[str] = Field(default=None, description='Name of account', title='Name')
     type: str = Field(..., description='Type of account', title='Type')
-    isExternal: bool = Field(
-        ..., description='Is account external (Yes or No)', title='Isexternal'
-    )
+    isExternal: bool = Field(..., description='Is account external (Yes or No)', title='Isexternal')
     email: Optional[str] = Field(
         default=None, description='Email address of account', title='Email'
     )
     identity: Optional[RawIdentitySchema] = Field(
         default=None, description='Associated Identity', title='Identity'
     )
     sourceApp: Optional[SourceAppSchema] = Field(
@@ -1416,26 +1318,24 @@
         description='Does the account have MFA enabled (Yes or No)',
         title='Hasmfa',
     )
     lastLoginAt: Optional[str] = Field(
         default=None, description='Account Last Logged date', title='Lastloginat'
     )
     tags: Optional[List[TagSchema]] = Field(
-        default=None, description='Tags associated with the account.', title='Tags'
+        default=[], description='Tags associated with the account.', title='Tags'
     )
     riskScore: Optional[AccountRiskScore] = Field(
         default=None, description='Risk Scores for the Account.', title='Riskscore'
     )
 
 
 class CampaignsPermissionSchema(BaseModel):
     id: str = Field(..., description='Campaign ID (unique). \n', title='Id')
-    campaignId: str = Field(
-        ..., description='ID of the Campaign.\n', title='Campaignid'
-    )
+    campaignId: str = Field(..., description='ID of the Campaign.\n', title='Campaignid')
     reviewerId: str = Field(..., description='Reviewer ID', title='Reviewerid')
     reviewer: Optional[ReviewerSchema] = Field(
         default=None, description='Details of the reviewer.\n', title='Reviewer'
     )
     actorId: str = Field(
         ...,
         description='Actor ID (Account or Grouping ID) that their access was reviewed. \n',
@@ -1466,42 +1366,36 @@
         description='Reviewer decision for keeping or revoking the reviewed access.  \n',
         title='Decisionreason',
     )
 
 
 class IdentitySchema(BaseModel):
     authomizeId: str = Field(..., description='Unique ID', title='Authomizeid')
-    name: Optional[str] = Field(
-        default=None, description='Name of the identity', title='Name'
-    )
-    title: Optional[str] = Field(
-        default=None, description='Title of the identity', title='Title'
-    )
+    name: Optional[str] = Field(default=None, description='Name of the identity', title='Name')
+    title: Optional[str] = Field(default=None, description='Title of the identity', title='Title')
     department: Optional[str] = Field(
         default=None,
         description='The department in which the identity works',
         title='Department',
     )
     accountIds: Optional[List[str]] = Field(
         default=[],
         description='The account IDs associated with the identity',
         title='Accountids',
     )
     email: Optional[str] = Field(
         default=None, description='The email of the identity', title='Email'
     )
     tags: Optional[List[TagSchema]] = Field(
-        default=None, description='The tags provided for the identity', title='Tags'
+        default=[], description='The tags provided for the identity', title='Tags'
     )
     terminatedAt: Optional[str] = Field(
         default=None, description='Time of termination', title='Terminatedat'
     )
-    hiredAt: Optional[str] = Field(
-        default=None, description='Hired At', title='Hiredat'
-    )
+    hiredAt: Optional[str] = Field(default=None, description='Hired At', title='Hiredat')
     incidentsCount: Optional[int] = Field(
         default=None,
         description='Number of associated incidents',
         title='Incidentscount',
     )
     accounts: Optional[List[AccountSchema]] = Field(
         default=[],
@@ -1529,43 +1423,37 @@
         default=[], description='Entity', title='Entities'
     )
     apps: Optional[List[SourceAppSchema]] = Field(
         default=[], description='Applications', title='Apps'
     )
     category: Optional[AlertCategoryType] = Field(default=None, description='Category')
     tactics: Optional[List[AttackTacticType]] = Field(default=[], description='Tactics')
-    compliance: Optional[
-        List[Union[IsoIec27001, AicpaTsc2017, Ccm402, Ccm301, Cisv8]]
-    ] = Field(default=[], description='Compliance', title='Compliance')
+    compliance: Optional[List[Union[IsoIec27001, AicpaTsc2017, Ccm402, Ccm301, Cisv8]]] = Field(
+        default=[], description='Compliance', title='Compliance'
+    )
     techniques: Optional[List[str]] = Field(
         default=[], description='Techniques', title='Techniques'
     )
     status: Optional[EventStatusType] = Field(
         default=None,
         description='The status of the incident (Open, In Progress, Waiting for Input, or Closed)',
     )
     severity: SeverityType = Field(
         ..., description='The severity of the incident (Low, Medium, High or Critical).'
     )
     policyId: str = Field(..., description='Unique id of policy.', title='Policyid')
-    policy: Optional[PolicySchema] = Field(
-        default=None, description='Policy', title='Policy'
-    )
+    policy: Optional[PolicySchema] = Field(default=None, description='Policy', title='Policy')
     assigneeId: Optional[str] = Field(
         default=None, description='Unique id of assignee.', title='Assigneeid'
     )
-    assignee: Optional[UserSchema] = Field(
-        default=None, description='Assignee', title='Assignee'
-    )
+    assignee: Optional[UserSchema] = Field(default=None, description='Assignee', title='Assignee')
     recommendation: Optional[str] = Field(
         default=None, description='Recommendation', title='Recommendation'
     )
-    description: Optional[str] = Field(
-        default=None, description='Description', title='Description'
-    )
+    description: Optional[str] = Field(default=None, description='Description', title='Description')
     isResolved: bool = Field(..., description='Is Resolved?', title='Isresolved')
     url: str = Field(..., description='URL', title='Url')
 
 
 class NonPaginatedResponseSchemaIncidentSchema(BaseModel):
     class Config:
         extra = Extra.forbid
@@ -1583,17 +1471,15 @@
 class PaginatedResponseSchemaAccountSchema(BaseModel):
     class Config:
         extra = Extra.forbid
 
     pagination: Optional[PaginationResponseSchema] = Field(
         default=None, description='Pagination Metadata', title='Pagination'
     )
-    data: List[AccountSchema] = Field(
-        ..., description='List of Actual Data', title='Data'
-    )
+    data: List[AccountSchema] = Field(..., description='List of Actual Data', title='Data')
 
 
 class PaginatedResponseSchemaCampaignsPermissionSchema(BaseModel):
     class Config:
         extra = Extra.forbid
 
     pagination: Optional[PaginationResponseSchema] = Field(
@@ -1607,22 +1493,18 @@
 class PaginatedResponseSchemaIdentitySchema(BaseModel):
     class Config:
         extra = Extra.forbid
 
     pagination: Optional[PaginationResponseSchema] = Field(
         default=None, description='Pagination Metadata', title='Pagination'
     )
-    data: List[IdentitySchema] = Field(
-        ..., description='List of Actual Data', title='Data'
-    )
+    data: List[IdentitySchema] = Field(..., description='List of Actual Data', title='Data')
 
 
 class PaginatedResponseSchemaIncidentSchema(BaseModel):
     class Config:
         extra = Extra.forbid
 
     pagination: Optional[PaginationResponseSchema] = Field(
         default=None, description='Pagination Metadata', title='Pagination'
     )
-    data: List[IncidentSchema] = Field(
-        ..., description='List of Actual Data', title='Data'
-    )
+    data: List[IncidentSchema] = Field(..., description='List of Actual Data', title='Data')
```

### Comparing `authomize-rest-api-client-4.3.8/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json` & `authomize-rest-api-client-4.3.9/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.8/authomize/rest_api_client/openapi/external_rest_api/openapi.json` & `authomize-rest-api-client-4.3.9/authomize/rest_api_client/openapi/external_rest_api/openapi.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9873799640765014%*

 * *Differences: {"'components'": "{'schemas': {'AccountSchema': {'properties': {'tags': {'default': []}}}, "*

 * *                 "'AssetSchema': {'properties': {'tags': {'default': []}}}, 'GroupSchema': "*

 * *                 "{'properties': {'tags': {'default': []}, 'createdAt': {'description': 'Date when "*

 * *                 "group was created.'}, 'originType': {'description': 'Type of the group in source "*

 * *                 "system.'}}}, 'IdentitySchema': {'properties': {'tags': {'default': []}}}, "*

 * *                 "'MeResponse' […]*

```diff
@@ -140,14 +140,15 @@
                             {
                                 "$ref": "#/components/schemas/UserStatus"
                             }
                         ],
                         "description": "The account status"
                     },
                     "tags": {
+                        "default": [],
                         "description": "Tags associated with the account.",
                         "items": {
                             "$ref": "#/components/schemas/TagSchema"
                         },
                         "title": "Tags",
                         "type": "array"
                     },
@@ -376,14 +377,15 @@
                                 "$ref": "#/components/schemas/SourceAppSchema"
                             }
                         ],
                         "description": "The source application of the asset",
                         "title": "Sourceapp"
                     },
                     "tags": {
+                        "default": [],
                         "description": "List of tags associated with the asset",
                         "items": {
                             "$ref": "#/components/schemas/TagSchema"
                         },
                         "title": "Tags",
                         "type": "array"
                     },
@@ -915,15 +917,15 @@
                 "properties": {
                     "authomizeId": {
                         "description": "Authomize ID of the Group.",
                         "title": "Authomizeid",
                         "type": "string"
                     },
                     "createdAt": {
-                        "description": "Type of the group in source system.",
+                        "description": "Date when group was created.",
                         "title": "Createdat",
                         "type": "string"
                     },
                     "incidentsCount": {
                         "description": "Number of incidents associated with the group.",
                         "title": "Incidentscount",
                         "type": "integer"
@@ -944,15 +946,15 @@
                     },
                     "originId": {
                         "description": "The ID of the group on the source system",
                         "title": "Originid",
                         "type": "string"
                     },
                     "originType": {
-                        "description": "Date when group was created.",
+                        "description": "Type of the group in source system.",
                         "title": "Origintype",
                         "type": "string"
                     },
                     "ownerId": {
                         "description": "Authomize ID of the Group Owner.",
                         "title": "Ownerid",
                         "type": "string"
@@ -963,14 +965,15 @@
                                 "$ref": "#/components/schemas/SourceAppSchema"
                             }
                         ],
                         "description": "Authomize ID of the Group.",
                         "title": "Sourceapp"
                     },
                     "tags": {
+                        "default": [],
                         "description": "List of tags associated with the group",
                         "items": {
                             "$ref": "#/components/schemas/TagSchema"
                         },
                         "title": "Tags",
                         "type": "array"
                     },
@@ -1106,14 +1109,15 @@
                                 "$ref": "#/components/schemas/IdentityRiskScore"
                             }
                         ],
                         "description": "Risk Scores",
                         "title": "Riskscore"
                     },
                     "tags": {
+                        "default": [],
                         "description": "The tags provided for the identity",
                         "items": {
                             "$ref": "#/components/schemas/TagSchema"
                         },
                         "title": "Tags",
                         "type": "array"
                     },
@@ -1577,15 +1581,15 @@
                     },
                     "tenant": {
                         "description": "**tenant**",
                         "title": "Tenant",
                         "type": "string"
                     },
                     "version": {
-                        "default": "4.3.0",
+                        "default": "4.3.7",
                         "description": "**version**",
                         "title": "Version",
                         "type": "string"
                     }
                 },
                 "required": [
                     "id",
@@ -2000,14 +2004,15 @@
                     },
                     "name": {
                         "description": "Name of the identity",
                         "title": "Name",
                         "type": "string"
                     },
                     "tags": {
+                        "default": [],
                         "description": "The tags provided for the identity",
                         "items": {
                             "$ref": "#/components/schemas/TagSchema"
                         },
                         "title": "Tags",
                         "type": "array"
                     },
@@ -3176,15 +3181,15 @@
                 "type": "apiKey"
             }
         }
     },
     "info": {
         "description": "Authomize enables users to integrate your applications with Authomize via custom connectors.\n\nYou can use the APIs described in this document to create your connector.\n\nOnce data is uploaded and processed successfully, your custom connector will function in the same way as the connectors created by Authomize.\n\n## How does Authomize work?\nAuthomize works by gathering information about:\n\n\u00b7 individuals, teams and functions.\n\n\u00b7 apps, assets and accounts.\n\n\u00b7 all the relationships between them.\n\n![img.png](https://storagetry1.blob.core.windows.net/public/78d82650-71b0-4909-8444-022aab79add5.png)\n\n## Connector APIs\n\nAuthomize connector APIs enable pushing data into Authomize from external sources.\n\nThese APIs enable data extracted from outside applications (via application APIs) to be delivered to Authomize.\n\nA connector processes extracted application data to transform it into a format compatible with Authomize.\n\n![img_1.png](https://storagetry1.blob.core.windows.net/public/341bf6ef-2e5b-4284-b715-45105ffbf0f8.png)\n\n## Authentication\nTo Authenticate use the API Token, with the format: `Authorization: API_Token`.\n\nAn API Token is a token you provide when making API calls. \n\n\nThe API Token should be included in every request to the API in an `Authorization` header.\n```\ncurl -v -X POST \\n\n     -H \"Authorization: {API_Token}\" \\n\n     ...\n```\n\n## Limits\nRequests cannot exceed a size of 1MB.\n",
         "title": "Authomize API Reference",
-        "version": "4.3.0",
+        "version": "4.3.7",
         "x-logo": {
             "url": "https://static.authomize.com/public/icons/authomize-green.svg"
         }
     },
     "openapi": "3.0.2",
     "paths": {
         "/is_alive": {
@@ -3745,15 +3750,15 @@
                 "tags": [
                     "Incident"
                 ]
             }
         },
         "/v2/inventory/accounts/search": {
             "post": {
-                "description": "Search Accounts",
+                "description": "Find specific accounts on Authomize and get related data such as ID, status and more",
                 "operationId": "search_accounts_v2_inventory_accounts_search_post",
                 "requestBody": {
                     "content": {
                         "application/json": {
                             "schema": {
                                 "$ref": "#/components/schemas/SearchAccountsRequestSchema"
                             }
```

### Comparing `authomize-rest-api-client-4.3.8/authomize_rest_api_client.egg-info/SOURCES.txt` & `authomize-rest-api-client-4.3.9/authomize_rest_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.8/setup.py` & `authomize-rest-api-client-4.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_namespace_packages, setup
 
 if __name__ == '__main__':
     setup(
-        version='4.3.8',
+        version='4.3.9',
         name='authomize-rest-api-client',
         author='Authomize inc.',
         license='MIT',
         author_email='info@authomize.com',
         description='Authomize REST API Python Client',
         packages=find_namespace_packages(include=['authomize.*']),
         package_data={
```

