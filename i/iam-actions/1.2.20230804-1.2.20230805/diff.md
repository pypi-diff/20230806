# Comparing `tmp/iam_actions-1.2.20230804.tar.gz` & `tmp/iam_actions-1.2.20230805.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20230804.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20230805.tar", max compression
```

## Comparing `iam_actions-1.2.20230804.tar` & `iam_actions-1.2.20230805.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-08-04 02:23:00.878126 iam_actions-1.2.20230804/LICENSE
--rw-r--r--   0        0        0     2302 2023-08-04 02:23:00.878126 iam_actions-1.2.20230804/README.md
--rw-r--r--   0        0        0      228 2023-08-04 02:23:00.878126 iam_actions-1.2.20230804/iam_actions/__init__.py
--rw-r--r--   0        0        0  4389954 2023-08-04 02:24:39.268079 iam_actions-1.2.20230804/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2023-08-04 02:23:00.878126 iam_actions-1.2.20230804/iam_actions/data.py
--rw-r--r--   0        0        0       80 2023-08-04 02:23:00.878126 iam_actions-1.2.20230804/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2023-08-04 02:23:00.878126 iam_actions-1.2.20230804/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2023-08-04 02:23:00.878126 iam_actions-1.2.20230804/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2023-08-04 02:23:00.878126 iam_actions-1.2.20230804/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2023-08-04 02:23:00.878126 iam_actions-1.2.20230804/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2023-08-04 02:23:00.878126 iam_actions-1.2.20230804/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2023-08-04 02:23:00.878126 iam_actions-1.2.20230804/iam_actions/generate/services.py
--rw-r--r--   0        0        0   566190 2023-08-04 02:24:39.268079 iam_actions-1.2.20230804/iam_actions/policies.json
--rw-r--r--   0        0        0   196525 2023-08-04 02:24:39.268079 iam_actions-1.2.20230804/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   549219 2023-08-04 02:24:39.268079 iam_actions-1.2.20230804/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2023-08-04 02:24:40.140096 iam_actions-1.2.20230804/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230804/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230804/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-08-05 02:20:39.954184 iam_actions-1.2.20230805/LICENSE
+-rw-r--r--   0        0        0     2302 2023-08-05 02:20:39.954184 iam_actions-1.2.20230805/README.md
+-rw-r--r--   0        0        0      228 2023-08-05 02:20:39.954184 iam_actions-1.2.20230805/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4389521 2023-08-05 02:22:13.519017 iam_actions-1.2.20230805/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2023-08-05 02:20:39.954184 iam_actions-1.2.20230805/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2023-08-05 02:20:39.954184 iam_actions-1.2.20230805/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2023-08-05 02:20:39.954184 iam_actions-1.2.20230805/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2023-08-05 02:20:39.954184 iam_actions-1.2.20230805/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2023-08-05 02:20:39.954184 iam_actions-1.2.20230805/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2023-08-05 02:20:39.954184 iam_actions-1.2.20230805/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2023-08-05 02:20:39.954184 iam_actions-1.2.20230805/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2023-08-05 02:20:39.954184 iam_actions-1.2.20230805/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   566397 2023-08-05 02:22:13.519017 iam_actions-1.2.20230805/iam_actions/policies.json
+-rw-r--r--   0        0        0   196077 2023-08-05 02:22:13.519017 iam_actions-1.2.20230805/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   549418 2023-08-05 02:22:13.519017 iam_actions-1.2.20230805/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2023-08-05 02:22:14.547025 iam_actions-1.2.20230805/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230805/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230805/PKG-INFO
```

### Comparing `iam_actions-1.2.20230804/LICENSE` & `iam_actions-1.2.20230805/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230804/README.md` & `iam_actions-1.2.20230805/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230804/iam_actions/actions.json` & `iam_actions-1.2.20230805/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994273680371424%*

 * *Differences: {"'applicationinsights'": "{'ListWorkloads': OrderedDict([('access_level', 'Undocumented'), "*

 * *                          "('action', 'ListWorkloads'), ('condition_keys', []), ('description', "*

 * *                          "'Not Documented by AWS'), ('orphan', False), ('resources', [])]), "*

 * *                          "'AddWorkload': OrderedDict([('access_level', 'Undocumented'), "*

 * *                          "('action', 'AddWorkload'), ('condition_keys', []), ('description', 'Not "*

 * *                          "Docume […]*

```diff
@@ -4868,14 +4868,22 @@
             "condition_keys": [],
             "description": "Grants permission to update an existing Application Cost Profiler Report configuration",
             "orphan": false,
             "resources": []
         }
     },
     "applicationinsights": {
+        "AddWorkload": {
+            "access_level": "Undocumented",
+            "action": "AddWorkload",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "CreateApplication": {
             "access_level": "Write",
             "action": "CreateApplication",
             "condition_keys": [],
             "description": "Grants permission to create an application from a resource group",
             "orphan": false,
             "resources": []
@@ -4980,14 +4988,22 @@
             "access_level": "Read",
             "action": "DescribeProblemObservations",
             "condition_keys": [],
             "description": "Grants permission to describe the observation in a problem",
             "orphan": false,
             "resources": []
         },
+        "DescribeWorkload": {
+            "access_level": "Undocumented",
+            "action": "DescribeWorkload",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "Link": {
             "access_level": "Write",
             "action": "Link",
             "condition_keys": [],
             "description": "Grants permission to share Application Insights resources with a monitoring account",
             "orphan": false,
             "resources": []
@@ -5044,14 +5060,30 @@
             "access_level": "Read",
             "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Grants permission to list tags for the resource",
             "orphan": false,
             "resources": []
         },
+        "ListWorkloads": {
+            "access_level": "Undocumented",
+            "action": "ListWorkloads",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "RemoveWorkload": {
+            "access_level": "Undocumented",
+            "action": "RemoveWorkload",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "TagResource": {
             "access_level": "Tagging",
             "action": "TagResource",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
@@ -5096,14 +5128,30 @@
         "UpdateLogPattern": {
             "access_level": "Write",
             "action": "UpdateLogPattern",
             "condition_keys": [],
             "description": "Grants permission to update a log pattern",
             "orphan": false,
             "resources": []
+        },
+        "UpdateProblem": {
+            "access_level": "Undocumented",
+            "action": "UpdateProblem",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "UpdateWorkload": {
+            "access_level": "Undocumented",
+            "action": "UpdateWorkload",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
         }
     },
     "appmesh": {
         "CreateGatewayRoute": {
             "access_level": "Write",
             "action": "CreateGatewayRoute",
             "condition_keys": [
@@ -32816,14 +32864,22 @@
             ],
             "description": "Grants permission to update a quick connect name and description in an Amazon Connect instance",
             "orphan": false,
             "resources": [
                 "quick-connect"
             ]
         },
+        "UpdateRoutingProfileAgentAvailabilityTimer": {
+            "access_level": "Undocumented",
+            "action": "UpdateRoutingProfileAgentAvailabilityTimer",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "UpdateRoutingProfileConcurrency": {
             "access_level": "Write",
             "action": "UpdateRoutingProfileConcurrency",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "connect:InstanceId"
             ],
@@ -34799,18 +34855,21 @@
                 "aws:TagKeys"
             ],
             "description": "Grants permission to activate an agent that you have deployed on your host",
             "orphan": false,
             "resources": []
         },
         "CreateLocationAzureBlob": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateLocationAzureBlob",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys"
+            ],
+            "description": "Grants permission to create an endpoint for a Microsoft Azure Blob Storage container",
             "orphan": false,
             "resources": []
         },
         "CreateLocationEfs": {
             "access_level": "Write",
             "action": "CreateLocationEfs",
             "condition_keys": [
@@ -34981,20 +35040,22 @@
             "description": "Grants permission to describe metadata about a discovery job",
             "orphan": false,
             "resources": [
                 "discoveryjob"
             ]
         },
         "DescribeLocationAzureBlob": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "DescribeLocationAzureBlob",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to view metadata, such as the path information about an Azure Blob Storage sync location",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "location"
+            ]
         },
         "DescribeLocationEfs": {
             "access_level": "Read",
             "action": "DescribeLocationEfs",
             "condition_keys": [],
             "description": "Grants permission to view metadata, such as the path information about an Amazon EFS sync location",
             "orphan": false,
@@ -35315,20 +35376,22 @@
             "description": "Grants permission to update a discovery job",
             "orphan": false,
             "resources": [
                 "discoveryjob"
             ]
         },
         "UpdateLocationAzureBlob": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "UpdateLocationAzureBlob",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to update an Azure Blob Storage sync location",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "location"
+            ]
         },
         "UpdateLocationHdfs": {
             "access_level": "Write",
             "action": "UpdateLocationHdfs",
             "condition_keys": [],
             "description": "Grants permission to update an HDFS sync Location",
             "orphan": false,
@@ -83440,14 +83503,22 @@
             "condition_keys": [],
             "description": "Grants permission to approve a permission request",
             "orphan": false,
             "resources": [
                 "permission"
             ]
         },
+        "AssumePermissionRole": {
+            "access_level": "Undocumented",
+            "action": "AssumePermissionRole",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "CreatePermissionRequest": {
             "access_level": "Write",
             "action": "CreatePermissionRequest",
             "condition_keys": [],
             "description": "Grants permission to create a permission request",
             "orphan": false,
             "resources": [
@@ -115027,20 +115098,22 @@
             "orphan": false,
             "resources": [
                 "cluster",
                 "cluster-snapshot"
             ]
         },
         "DeleteDBClusterAutomatedBackup": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteDBClusterAutomatedBackup",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to delete cluster automated backups based on the source cluster's DbClusterResourceId value or the restorable cluster's resource ID",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "cluster-auto-backup"
+            ]
         },
         "DeleteDBClusterEndpoint": {
             "access_level": "Write",
             "action": "DeleteDBClusterEndpoint",
             "condition_keys": [],
             "description": "Grants permission to delete a custom endpoint and removes it from an Amazon Aurora DB cluster",
             "orphan": false,
@@ -115078,15 +115151,15 @@
                 "db"
             ]
         },
         "DeleteDBInstanceAutomatedBackup": {
             "access_level": "Write",
             "action": "DeleteDBInstanceAutomatedBackup",
             "condition_keys": [],
-            "description": "Grants permission to deletes automated backups based on the source instance's DbiResourceId value or the restorable instance's resource ID",
+            "description": "Grants permission to delete automated backups based on the source instance's DbiResourceId value or the restorable instance's resource ID",
             "orphan": false,
             "resources": []
         },
         "DeleteDBParameterGroup": {
             "access_level": "Write",
             "action": "DeleteDBParameterGroup",
             "condition_keys": [],
@@ -115212,20 +115285,23 @@
             "action": "DescribeCertificates",
             "condition_keys": [],
             "description": "Grants permission to list the set of CA certificates provided by Amazon RDS for this AWS account",
             "orphan": false,
             "resources": []
         },
         "DescribeDBClusterAutomatedBackups": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeDBClusterAutomatedBackups",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to return a list of cluster automated backups for both current and deleted clusters",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "cluster",
+                "cluster-auto-backup"
+            ]
         },
         "DescribeDBClusterBacktracks": {
             "access_level": "List",
             "action": "DescribeDBClusterBacktracks",
             "condition_keys": [],
             "description": "Grants permission to return information about backtracks for a DB cluster",
             "orphan": false,
@@ -116070,14 +116146,15 @@
                 "rds:StorageSize",
                 "rds:req-tag/${TagKey}"
             ],
             "description": "Grants permission to restore a DB cluster to an arbitrary point in time",
             "orphan": false,
             "resources": [
                 "cluster",
+                "cluster-auto-backup",
                 "cluster-pg",
                 "og",
                 "subgrp"
             ]
         },
         "RestoreDBInstanceFromDBSnapshot": {
             "access_level": "Write",
@@ -119253,557 +119330,444 @@
             "resources": [
                 "streamprocessor"
             ]
         }
     },
     "resiliencehub": {
         "AddDraftAppVersionResourceMappings": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "AddDraftAppVersionResourceMappings",
             "condition_keys": [],
-            "description": "Grants permission to add draft application version resource mappings",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "application"
-            ]
+            "resources": []
         },
         "BatchUpdateRecommendationStatus": {
             "access_level": "Undocumented",
             "action": "BatchUpdateRecommendationStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "CreateApp": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateApp",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:TagKeys"
-            ],
-            "description": "Grants permission to create application",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "CreateAppVersionAppComponent": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateAppVersionAppComponent",
             "condition_keys": [],
-            "description": "Grants permission to create application app component",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "application"
-            ]
+            "resources": []
         },
         "CreateAppVersionResource": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateAppVersionResource",
             "condition_keys": [],
-            "description": "Grants permission to create application resource",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "application"
-            ]
+            "resources": []
         },
         "CreateRecommendationTemplate": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateRecommendationTemplate",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:TagKeys"
-            ],
-            "description": "Grants permission to create recommendation template",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "application"
-            ]
+            "resources": []
         },
         "CreateResiliencyPolicy": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateResiliencyPolicy",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:TagKeys"
-            ],
-            "description": "Grants permission to create resiliency policy",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DeleteApp": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteApp",
             "condition_keys": [],
-            "description": "Grants permission to batch delete application",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "application"
-            ]
+            "resources": []
         },
         "DeleteAppAssessment": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteAppAssessment",
             "condition_keys": [],
-            "description": "Grants permission to batch delete application assessment",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "application"
-            ]
+            "resources": []
         },
         "DeleteAppInputSource": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteAppInputSource",
             "condition_keys": [],
-            "description": "Grants permission to remove application input source",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "application"
-            ]
+            "resources": []
         },
         "DeleteAppVersionAppComponent": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteAppVersionAppComponent",
             "condition_keys": [],
-            "description": "Grants permission to delete application app component",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "application"
-            ]
+            "resources": []
         },
         "DeleteAppVersionResource": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteAppVersionResource",
             "condition_keys": [],
-            "description": "Grants permission to delete application resource",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "application"
-            ]
+            "resources": []
         },
         "DeleteRecommendationTemplate": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteRecommendationTemplate",
             "condition_keys": [],
-            "description": "Grants permission to batch delete recommendation template",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "application"
-            ]
+            "resources": []
         },
         "DeleteResiliencyPolicy": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteResiliencyPolicy",
             "condition_keys": [],
-            "description": "Grants permission to batch delete resiliency policy",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "resiliency-policy"
-            ]
+            "resources": []
         },
         "DescribeApp": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "DescribeApp",
             "condition_keys": [],
-            "description": "Grants permission to describe application",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "application"
-            ]
+            "resources": []
         },
         "DescribeAppAssessment": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "DescribeAppAssessment",
             "condition_keys": [],
-            "description": "Grants permission to describe application assessment",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "application"
-            ]
+            "resources": []
         },
         "DescribeAppVersion": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "DescribeAppVersion",
             "condition_keys": [],
-            "description": "Grants permission to describe application version",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "application"
-            ]
+            "resources": []
         },
         "DescribeAppVersionAppComponent": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "DescribeAppVersionAppComponent",
             "condition_keys": [],
-            "description": "Grants permission to describe application version app component",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "application"
-            ]
+            "resources": []
         },
         "DescribeAppVersionResource": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "DescribeAppVersionResource",
             "condition_keys": [],
-            "description": "Grants permission to describe application version resource",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "application"
-            ]
+            "resources": []
         },
         "DescribeAppVersionResourcesResolutionStatus": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "DescribeAppVersionResourcesResolutionStatus",
             "condition_keys": [],
-            "description": "Grants permission to describe application resolution",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "application"
-            ]
+            "resources": []
         },
         "DescribeAppVersionTemplate": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "DescribeAppVersionTemplate",
             "condition_keys": [],
-            "description": "Grants permission to describe application version template",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "application"
-            ]
+            "resources": []
         },
         "DescribeDraftAppVersionResourcesImportStatus": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "DescribeDraftAppVersionResourcesImportStatus",
             "condition_keys": [],
-            "description": "Grants permission to describe draft application version resources import status",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "application"
-            ]
+            "resources": []
         },
         "DescribeResiliencyPolicy": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "DescribeResiliencyPolicy",
             "condition_keys": [],
-            "description": "Grants permission to describe resiliency policy",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "resiliency-policy"
-            ]
+            "resources": []
         },
         "ImportResourcesToDraftAppVersion": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ImportResourcesToDraftAppVersion",
             "condition_keys": [],
-            "description": "Grants permission to import resources to draft application version",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "application"
-            ]
+            "resources": []
         },
         "ListAlarmRecommendations": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "ListAlarmRecommendations",
             "condition_keys": [],
-            "description": "Grants permission to list alarm recommendation",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "application"
-            ]
+            "resources": []
         },
         "ListAppAssessmentComplianceDrifts": {
             "access_level": "Undocumented",
             "action": "ListAppAssessmentComplianceDrifts",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListAppAssessments": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "ListAppAssessments",
             "condition_keys": [],
-            "description": "Grants permission to list application assessment",
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListAppComponentCompliances": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "ListAppComponentCompliances",
             "condition_keys": [],
-            "description": "Grants permission to list app component compliances",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "application"
-            ]
+            "resources": []
         },
         "ListAppComponentRecommendations": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "ListAppComponentRecommendations",
             "condition_keys": [],
-            "description": "Grants permission to list app component recommendations",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "application"
-            ]
+            "resources": []
         },
         "ListAppInputSources": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "ListAppInputSources",
             "condition_keys": [],
-            "description": "Grants permission to list application input sources",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "application"
-            ]
+            "resources": []
         },
         "ListAppVersionAppComponents": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "ListAppVersionAppComponents",
             "condition_keys": [],
-            "description": "Grants permission to list application version app components",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "application"
-            ]
+            "resources": []
         },
         "ListAppVersionResourceMappings": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "ListAppVersionResourceMappings",
             "condition_keys": [],
-            "description": "Grants permission to application version resource mappings",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "application"
-            ]
+            "resources": []
         },
         "ListAppVersionResources": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "ListAppVersionResources",
             "condition_keys": [],
-            "description": "Grants permission to list application resources",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "application"
-            ]
+            "resources": []
         },
         "ListAppVersions": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "ListAppVersions",
             "condition_keys": [],
-            "description": "Grants permission to list application version",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "application"
-            ]
+            "resources": []
         },
         "ListApps": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "ListApps",
             "condition_keys": [],
-            "description": "Grants permission to list applications",
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListRecommendationTemplates": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "ListRecommendationTemplates",
             "condition_keys": [],
-            "description": "Grants permission to list recommendation templates",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "application"
-            ]
+            "resources": []
         },
         "ListResiliencyPolicies": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "ListResiliencyPolicies",
             "condition_keys": [],
-            "description": "Grants permission to list resiliency policies",
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListSopRecommendations": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "ListSopRecommendations",
             "condition_keys": [],
-            "description": "Grants permission to list SOP recommendations",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "application"
-            ]
+            "resources": []
         },
         "ListSuggestedResiliencyPolicies": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "ListSuggestedResiliencyPolicies",
             "condition_keys": [],
-            "description": "Grants permission to list suggested resiliency policies",
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListTagsForResource": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "ListTagsForResource",
             "condition_keys": [],
-            "description": "Grants permission to list tags for a resource",
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListTestRecommendations": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "ListTestRecommendations",
             "condition_keys": [],
-            "description": "Grants permission to list test recommendations",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "application"
-            ]
+            "resources": []
         },
         "ListUnsupportedAppVersionResources": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "ListUnsupportedAppVersionResources",
             "condition_keys": [],
-            "description": "Grants permission to list unsupported application version resources",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "application"
-            ]
+            "resources": []
         },
         "PublishAppVersion": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "PublishAppVersion",
             "condition_keys": [],
-            "description": "Grants permission to publish application version",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "application"
-            ]
+            "resources": []
         },
         "PutDraftAppVersionTemplate": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "PutDraftAppVersionTemplate",
             "condition_keys": [],
-            "description": "Grants permission to put draft application version template",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "application"
-            ]
+            "resources": []
         },
         "RemoveDraftAppVersionResourceMappings": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "RemoveDraftAppVersionResourceMappings",
             "condition_keys": [],
-            "description": "Grants permission to remove draft application version mappings",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "application"
-            ]
+            "resources": []
         },
         "ResolveAppVersionResources": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ResolveAppVersionResources",
             "condition_keys": [],
-            "description": "Grants permission to resolve application version resources",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "application"
-            ]
+            "resources": []
         },
         "StartAppAssessment": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "StartAppAssessment",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:TagKeys"
-            ],
-            "description": "Grants permission to create application assessment",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "application"
-            ]
+            "resources": []
         },
         "TagResource": {
-            "access_level": "Tagging",
+            "access_level": "Undocumented",
             "action": "TagResource",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:TagKeys"
-            ],
-            "description": "Grants permission to assign a resource tag",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "app-assessment",
-                "application",
-                "recommendation-template",
-                "resiliency-policy"
-            ]
+            "resources": []
         },
         "UntagResource": {
-            "access_level": "Tagging",
+            "access_level": "Undocumented",
             "action": "UntagResource",
-            "condition_keys": [
-                "aws:TagKeys"
-            ],
-            "description": "Grants permission to untag a resource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "app-assessment",
-                "application",
-                "recommendation-template",
-                "resiliency-policy"
-            ]
+            "resources": []
         },
         "UpdateApp": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "UpdateApp",
             "condition_keys": [],
-            "description": "Grants permission to update application",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "application"
-            ]
+            "resources": []
         },
         "UpdateAppVersion": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "UpdateAppVersion",
             "condition_keys": [],
-            "description": "Grants permission to update application version",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "application"
-            ]
+            "resources": []
         },
         "UpdateAppVersionAppComponent": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "UpdateAppVersionAppComponent",
             "condition_keys": [],
-            "description": "Grants permission to update application app component",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "application"
-            ]
+            "resources": []
         },
         "UpdateAppVersionResource": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "UpdateAppVersionResource",
             "condition_keys": [],
-            "description": "Grants permission to update application resource",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "application"
-            ]
+            "resources": []
         },
         "UpdateResiliencyPolicy": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "UpdateResiliencyPolicy",
             "condition_keys": [],
-            "description": "Grants permission to update resiliency policy",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "resiliency-policy"
-            ]
+            "resources": []
         }
     },
     "resource-explorer": {
         "ListResourceTypes": {
             "access_level": "List",
             "action": "ListResourceTypes",
             "condition_keys": [],
```

### Comparing `iam_actions-1.2.20230804/iam_actions/generate/action_map.py` & `iam_actions-1.2.20230805/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230804/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20230805/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230804/iam_actions/generate/generate.py` & `iam_actions-1.2.20230805/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230804/iam_actions/generate/notifier.py` & `iam_actions-1.2.20230805/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230804/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20230805/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230804/iam_actions/generate/services.py` & `iam_actions-1.2.20230805/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230804/iam_actions/policies.json` & `iam_actions-1.2.20230805/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999956283248197%*

 * *Differences: {"'serviceMap'": "{'Amazon Connect': {'Actions': {insert: [(190, "*

 * *                 "'UpdateRoutingProfileAgentAvailabilityTimer')]}}, 'AWS IQ Permissions': "*

 * *                 "{'Actions': {insert: [(2, 'AssumePermissionRole')]}}, 'Amazon CloudWatch "*

 * *                 "Application Insights': {'Actions': {insert: [(0, 'AddWorkload'), (15, "*

 * *                 "'DescribeWorkload'), (24, 'ListWorkloads'), (25, 'RemoveWorkload'), (32, "*

 * *                 "'UpdateProblem'), (33, 'UpdateWorkload')]}}}"}*

```diff
@@ -4938,14 +4938,15 @@
         },
         "AWS IQ Permissions": {
             "ARNFormat": "arn:aws:iq-permission:${Region}:${Account}:${ResourceType}/${ResourceName}",
             "ARNRegex": "^arn:aws:iq-permission:.+",
             "Actions": [
                 "ApproveAccessGrant",
                 "ApprovePermissionRequest",
+                "AssumePermissionRole",
                 "CreatePermissionRequest",
                 "GetPermissionRequest",
                 "ListPermissionRequests",
                 "RejectPermissionRequest",
                 "RevokePermissionRequest",
                 "WithdrawPermissionRequest"
             ],
@@ -11123,42 +11124,48 @@
                 "cloudwatch:namespace",
                 "cloudwatch:requestInsightRuleLogGroups",
                 "cloudwatch:requestManagedResourceARNs"
             ]
         },
         "Amazon CloudWatch Application Insights": {
             "Actions": [
+                "AddWorkload",
                 "CreateApplication",
                 "CreateComponent",
                 "CreateLogPattern",
                 "DeleteApplication",
                 "DeleteComponent",
                 "DeleteLogPattern",
                 "DescribeApplication",
                 "DescribeComponent",
                 "DescribeComponentConfiguration",
                 "DescribeComponentConfigurationRecommendation",
                 "DescribeLogPattern",
                 "DescribeObservation",
                 "DescribeProblem",
                 "DescribeProblemObservations",
+                "DescribeWorkload",
                 "Link",
                 "ListApplications",
                 "ListComponents",
                 "ListConfigurationHistory",
                 "ListLogPatternSets",
                 "ListLogPatterns",
                 "ListProblems",
                 "ListTagsForResource",
+                "ListWorkloads",
+                "RemoveWorkload",
                 "TagResource",
                 "UntagResource",
                 "UpdateApplication",
                 "UpdateComponent",
                 "UpdateComponentConfiguration",
-                "UpdateLogPattern"
+                "UpdateLogPattern",
+                "UpdateProblem",
+                "UpdateWorkload"
             ],
             "HasResource": false,
             "StringPrefix": "applicationinsights",
             "conditionKeys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:ResourceTag/${TagKey}",
                 "aws:TagKeys"
@@ -12037,14 +12044,15 @@
                 "UpdateQueueHoursOfOperation",
                 "UpdateQueueMaxContacts",
                 "UpdateQueueName",
                 "UpdateQueueOutboundCallerConfig",
                 "UpdateQueueStatus",
                 "UpdateQuickConnectConfig",
                 "UpdateQuickConnectName",
+                "UpdateRoutingProfileAgentAvailabilityTimer",
                 "UpdateRoutingProfileConcurrency",
                 "UpdateRoutingProfileDefaultOutboundQueue",
                 "UpdateRoutingProfileName",
                 "UpdateRoutingProfileQueues",
                 "UpdateRule",
                 "UpdateSecurityProfile",
                 "UpdateTaskTemplate",
```

### Comparing `iam_actions-1.2.20230804/iam_actions/resourcetypes.json` & `iam_actions-1.2.20230805/iam_actions/resourcetypes.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9985694822888284%*

 * *Differences: {"'rds'": "{'cluster-auto-backup': OrderedDict([('arn_pattern', "*

 * *          "'arn:*:rds:*:*:cluster-auto-backup:*'), ('condition_keys', None)])}",*

 * * "'resiliencehub'": '{replace: OrderedDict()}'}*

```diff
@@ -4987,14 +4987,18 @@
             "arn_pattern": "arn:*:rds:*:*:cev:*/*/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
         "cluster": {
             "arn_pattern": "arn:*:rds:*:*:cluster:*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
+        "cluster-auto-backup": {
+            "arn_pattern": "arn:*:rds:*:*:cluster-auto-backup:*",
+            "condition_keys": null
+        },
         "cluster-endpoint": {
             "arn_pattern": "arn:*:rds:*:*:cluster-endpoint:*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
         "cluster-pg": {
             "arn_pattern": "arn:*:rds:*:*:cluster-pg:*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
@@ -5214,32 +5218,15 @@
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
         "streamprocessor": {
             "arn_pattern": "arn:*:rekognition:*:*:streamprocessor/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         }
     },
-    "resiliencehub": {
-        "app-assessment": {
-            "arn_pattern": "arn:*:resiliencehub:*:*:app-assessment/*",
-            "condition_keys": "aws:ResourceTag/${TagKey}"
-        },
-        "application": {
-            "arn_pattern": "arn:*:resiliencehub:*:*:app/*",
-            "condition_keys": "aws:ResourceTag/${TagKey}"
-        },
-        "recommendation-template": {
-            "arn_pattern": "arn:*:resiliencehub:*:*:recommendation-template/*",
-            "condition_keys": "aws:ResourceTag/${TagKey}"
-        },
-        "resiliency-policy": {
-            "arn_pattern": "arn:*:resiliencehub:*:*:resiliency-policy/*",
-            "condition_keys": "aws:ResourceTag/${TagKey}"
-        }
-    },
+    "resiliencehub": {},
     "resource-explorer": {},
     "resource-explorer-2": {
         "index": {
             "arn_pattern": "arn:*:resource-explorer-2:*:*:index/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
         "view": {
```

### Comparing `iam_actions-1.2.20230804/iam_actions/services.json` & `iam_actions-1.2.20230805/iam_actions/services.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999667988115035%*

 * *Differences: {"'applicationinsights'": "{'Actions': {insert: [(0, 'AddWorkload'), (15, 'DescribeWorkload'), "*

 * *                          "(24, 'ListWorkloads'), (25, 'RemoveWorkload'), (32, 'UpdateProblem'), "*

 * *                          "(33, 'UpdateWorkload')]}}",*

 * * "'connect'": "{'Actions': {insert: [(190, 'UpdateRoutingProfileAgentAvailabilityTimer')]}}",*

 * * "'iq-permission'": "{'Actions': {insert: [(2, 'AssumePermissionRole')]}}"}*

```diff
@@ -849,42 +849,48 @@
             "AWS Application Cost Profiler Service"
         ]
     },
     "applicationinsights": {
         "ARNFormats": [],
         "ARNRegexes": [],
         "Actions": [
+            "AddWorkload",
             "CreateApplication",
             "CreateComponent",
             "CreateLogPattern",
             "DeleteApplication",
             "DeleteComponent",
             "DeleteLogPattern",
             "DescribeApplication",
             "DescribeComponent",
             "DescribeComponentConfiguration",
             "DescribeComponentConfigurationRecommendation",
             "DescribeLogPattern",
             "DescribeObservation",
             "DescribeProblem",
             "DescribeProblemObservations",
+            "DescribeWorkload",
             "Link",
             "ListApplications",
             "ListComponents",
             "ListConfigurationHistory",
             "ListLogPatternSets",
             "ListLogPatterns",
             "ListProblems",
             "ListTagsForResource",
+            "ListWorkloads",
+            "RemoveWorkload",
             "TagResource",
             "UntagResource",
             "UpdateApplication",
             "UpdateComponent",
             "UpdateComponentConfiguration",
-            "UpdateLogPattern"
+            "UpdateLogPattern",
+            "UpdateProblem",
+            "UpdateWorkload"
         ],
         "ConditionKeys": [
             "aws:RequestTag/${TagKey}",
             "aws:ResourceTag/${TagKey}",
             "aws:TagKeys"
         ],
         "HasResource": false,
@@ -4851,14 +4857,15 @@
             "UpdateQueueHoursOfOperation",
             "UpdateQueueMaxContacts",
             "UpdateQueueName",
             "UpdateQueueOutboundCallerConfig",
             "UpdateQueueStatus",
             "UpdateQuickConnectConfig",
             "UpdateQuickConnectName",
+            "UpdateRoutingProfileAgentAvailabilityTimer",
             "UpdateRoutingProfileConcurrency",
             "UpdateRoutingProfileDefaultOutboundQueue",
             "UpdateRoutingProfileName",
             "UpdateRoutingProfileQueues",
             "UpdateRule",
             "UpdateSecurityProfile",
             "UpdateTaskTemplate",
@@ -11565,14 +11572,15 @@
         ],
         "ARNRegexes": [
             "^arn:aws:iq-permission:.+"
         ],
         "Actions": [
             "ApproveAccessGrant",
             "ApprovePermissionRequest",
+            "AssumePermissionRole",
             "CreatePermissionRequest",
             "GetPermissionRequest",
             "ListPermissionRequests",
             "RejectPermissionRequest",
             "RevokePermissionRequest",
             "WithdrawPermissionRequest"
         ],
```

### Comparing `iam_actions-1.2.20230804/pyproject.toml` & `iam_actions-1.2.20230805/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20230804"
+version = "1.2.20230805"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20230804/setup.py` & `iam_actions-1.2.20230805/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20230804',
+    'version': '1.2.20230805',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20230804/PKG-INFO` & `iam_actions-1.2.20230805/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20230804
+Version: 1.2.20230805
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

