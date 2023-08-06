# Comparing `tmp/PyArtifactory-1.9.6.tar.gz` & `tmp/PyArtifactory-1.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyArtifactory-1.9.6.tar", last modified: Fri Apr 15 08:18:57 2022, max compression
+gzip compressed data, was "PyArtifactory-1.9.7.tar", last modified: Mon May 30 20:22:46 2022, max compression
```

## Comparing `PyArtifactory-1.9.6.tar` & `PyArtifactory-1.9.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1064 2022-04-15 08:18:46.233643 PyArtifactory-1.9.6/LICENSE
--rw-r--r--   0        0        0    12600 2022-04-15 08:18:46.233643 PyArtifactory-1.9.6/README.md
--rw-r--r--   0        0        0      292 2022-04-15 08:18:46.233643 PyArtifactory-1.9.6/pyartifactory/__init__.py
--rw-r--r--   0        0        0     2456 2022-04-15 08:18:46.233643 PyArtifactory-1.9.6/pyartifactory/artifactory_object.py
--rw-r--r--   0        0        0     1232 2022-04-15 08:18:46.233643 PyArtifactory-1.9.6/pyartifactory/exception.py
--rw-r--r--   0        0        0      971 2022-04-15 08:18:46.233643 PyArtifactory-1.9.6/pyartifactory/models/__init__.py
--rw-r--r--   0        0        0     1761 2022-04-15 08:18:46.233643 PyArtifactory-1.9.6/pyartifactory/models/artifact.py
--rw-r--r--   0        0        0      726 2022-04-15 08:18:46.233643 PyArtifactory-1.9.6/pyartifactory/models/auth.py
--rw-r--r--   0        0        0      569 2022-04-15 08:18:46.233643 PyArtifactory-1.9.6/pyartifactory/models/group.py
--rw-r--r--   0        0        0     2969 2022-04-15 08:18:46.233643 PyArtifactory-1.9.6/pyartifactory/models/permission.py
--rw-r--r--   0        0        0     9469 2022-04-15 08:18:46.233643 PyArtifactory-1.9.6/pyartifactory/models/repository.py
--rw-r--r--   0        0        0     1212 2022-04-15 08:18:46.233643 PyArtifactory-1.9.6/pyartifactory/models/user.py
--rw-r--r--   0        0        0    36742 2022-04-15 08:18:46.233643 PyArtifactory-1.9.6/pyartifactory/objects.py
--rw-r--r--   0        0        0        0 2022-04-15 08:18:46.233643 PyArtifactory-1.9.6/pyartifactory/py.typed
--rw-r--r--   0        0        0      467 2022-04-15 08:18:46.233643 PyArtifactory-1.9.6/pyartifactory/utils.py
--rw-r--r--   0        0        0     1772 2022-04-15 08:18:46.233643 PyArtifactory-1.9.6/pyproject.toml
--rw-r--r--   0        0        0    13862 2022-04-15 08:18:57.319555 PyArtifactory-1.9.6/setup.py
--rw-r--r--   0        0        0    13978 2022-04-15 08:18:57.320336 PyArtifactory-1.9.6/PKG-INFO
+-rw-r--r--   0        0        0     1064 2022-05-30 20:22:38.047150 PyArtifactory-1.9.7/LICENSE
+-rw-r--r--   0        0        0    12600 2022-05-30 20:22:38.047150 PyArtifactory-1.9.7/README.md
+-rw-r--r--   0        0        0      292 2022-05-30 20:22:38.047150 PyArtifactory-1.9.7/pyartifactory/__init__.py
+-rw-r--r--   0        0        0     2456 2022-05-30 20:22:38.047150 PyArtifactory-1.9.7/pyartifactory/artifactory_object.py
+-rw-r--r--   0        0        0     1232 2022-05-30 20:22:38.047150 PyArtifactory-1.9.7/pyartifactory/exception.py
+-rw-r--r--   0        0        0      971 2022-05-30 20:22:38.047150 PyArtifactory-1.9.7/pyartifactory/models/__init__.py
+-rw-r--r--   0        0        0     1761 2022-05-30 20:22:38.047150 PyArtifactory-1.9.7/pyartifactory/models/artifact.py
+-rw-r--r--   0        0        0      726 2022-05-30 20:22:38.047150 PyArtifactory-1.9.7/pyartifactory/models/auth.py
+-rw-r--r--   0        0        0      569 2022-05-30 20:22:38.047150 PyArtifactory-1.9.7/pyartifactory/models/group.py
+-rw-r--r--   0        0        0     2969 2022-05-30 20:22:38.047150 PyArtifactory-1.9.7/pyartifactory/models/permission.py
+-rw-r--r--   0        0        0     9513 2022-05-30 20:22:38.047150 PyArtifactory-1.9.7/pyartifactory/models/repository.py
+-rw-r--r--   0        0        0     1212 2022-05-30 20:22:38.047150 PyArtifactory-1.9.7/pyartifactory/models/user.py
+-rw-r--r--   0        0        0    36742 2022-05-30 20:22:38.047150 PyArtifactory-1.9.7/pyartifactory/objects.py
+-rw-r--r--   0        0        0        0 2022-05-30 20:22:38.047150 PyArtifactory-1.9.7/pyartifactory/py.typed
+-rw-r--r--   0        0        0      467 2022-05-30 20:22:38.047150 PyArtifactory-1.9.7/pyartifactory/utils.py
+-rw-r--r--   0        0        0     1772 2022-05-30 20:22:38.047150 PyArtifactory-1.9.7/pyproject.toml
+-rw-r--r--   0        0        0    13862 2022-05-30 20:22:46.519757 PyArtifactory-1.9.7/setup.py
+-rw-r--r--   0        0        0    13978 2022-05-30 20:22:46.520544 PyArtifactory-1.9.7/PKG-INFO
```

### Comparing `PyArtifactory-1.9.6/LICENSE` & `PyArtifactory-1.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `PyArtifactory-1.9.6/README.md` & `PyArtifactory-1.9.7/README.md`

 * *Files identical despite different names*

### Comparing `PyArtifactory-1.9.6/pyartifactory/artifactory_object.py` & `PyArtifactory-1.9.7/pyartifactory/artifactory_object.py`

 * *Files identical despite different names*

### Comparing `PyArtifactory-1.9.6/pyartifactory/exception.py` & `PyArtifactory-1.9.7/pyartifactory/exception.py`

 * *Files identical despite different names*

### Comparing `PyArtifactory-1.9.6/pyartifactory/models/__init__.py` & `PyArtifactory-1.9.7/pyartifactory/models/__init__.py`

 * *Files identical despite different names*

### Comparing `PyArtifactory-1.9.6/pyartifactory/models/artifact.py` & `PyArtifactory-1.9.7/pyartifactory/models/artifact.py`

 * *Files identical despite different names*

### Comparing `PyArtifactory-1.9.6/pyartifactory/models/auth.py` & `PyArtifactory-1.9.7/pyartifactory/models/auth.py`

 * *Files identical despite different names*

### Comparing `PyArtifactory-1.9.6/pyartifactory/models/group.py` & `PyArtifactory-1.9.7/pyartifactory/models/group.py`

 * *Files identical despite different names*

### Comparing `PyArtifactory-1.9.6/pyartifactory/models/permission.py` & `PyArtifactory-1.9.7/pyartifactory/models/permission.py`

 * *Files identical despite different names*

### Comparing `PyArtifactory-1.9.6/pyartifactory/models/repository.py` & `PyArtifactory-1.9.7/pyartifactory/models/repository.py`

 * *Files 1% similar despite different names*

```diff
@@ -245,14 +245,15 @@
     blackedOut: bool = False
     storeArtifactsLocally: bool = True
     socketTimeoutMillis: int = 15000
     localAddress: Optional[str] = None
     retrievalCachePeriodSecs: int = 43200
     failedRetrievalCachePeriodSecs: int = 30
     missedRetrievalCachePeriodSecs: int = 7200
+    metadataRetrievalTimeoutSecs: int = 60
     unusedArtifactsCleanupEnabled: bool = False
     unusedArtifactsCleanupPeriodHours: int = 0
     assumedOfflinePeriodSecs: int = 300
     fetchJarsEagerly: int = False
     fetchSourcesEagerly: int = False
     shareConfiguration: bool = False
     synchronizeProperties: bool = False
```

### Comparing `PyArtifactory-1.9.6/pyartifactory/models/user.py` & `PyArtifactory-1.9.7/pyartifactory/models/user.py`

 * *Files identical despite different names*

### Comparing `PyArtifactory-1.9.6/pyartifactory/objects.py` & `PyArtifactory-1.9.7/pyartifactory/objects.py`

 * *Files identical despite different names*

### Comparing `PyArtifactory-1.9.6/pyproject.toml` & `PyArtifactory-1.9.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PyArtifactory"
-version = "1.9.6"
+version = "1.9.7"
 description = "Typed interactions with the Jfrog Artifactory REST API"
 authors = ["Ananias CARVALHO <carvalhoananias@hotmail.com>", "Thomas GAUDIN <thomas.gaudin@centraliens-lille.org>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/anancarv/python-artifactory"
 documentation = "https://github.com/anancarv/python-artifactory"
 keywords = ["artifactory"]
```

### Comparing `PyArtifactory-1.9.6/setup.py` & `PyArtifactory-1.9.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['email_validator>=1.0,<2.0',
  'pydantic>=1.4,<2.0',
  'requests>=2.21,<3.0',
  'typing_extensions>=3.7.4,<4.0.0']
 
 setup_kwargs = {
     'name': 'pyartifactory',
-    'version': '1.9.6',
+    'version': '1.9.7',
     'description': 'Typed interactions with the Jfrog Artifactory REST API',
     'long_description': '# PyArtifactory\n\n[![GitHub Actions workflow](https://github.com/anancarv/python-artifactory/workflows/Check%20code/badge.svg)](https://github.com/anancarv/python-artifactory/actions)\n[![PyPI version](https://badge.fury.io/py/pyartifactory.svg)](https://badge.fury.io/py/pyartifactory)\n[![Codacy Badge](https://app.codacy.com/project/badge/Grade/c02851e5b9f24fe299783b48eab18f54)](https://www.codacy.com/gh/anancarv/python-artifactory/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=anancarv/python-artifactory&amp;utm_campaign=Badge_Grade)\n[![Codacy Badge](https://app.codacy.com/project/badge/Coverage/c02851e5b9f24fe299783b48eab18f54)](https://www.codacy.com/gh/anancarv/python-artifactory/dashboard?utm_source=github.com&utm_medium=referral&utm_content=anancarv/python-artifactory&utm_campaign=Badge_Coverage)\n![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)\n\n\n`pyartifactory` is a Python library to access the [Artifactory REST API](https://www.jfrog.com/confluence/display/RTF/Artifactory+REST+API).\n\nThis library enables you to manage Artifactory resources such as users, groups, permissions, repositories, artifacts and access tokens in your applications. Based on Python 3.6+ type hints.\n\n<!-- toc -->\n\n- [Requirements](#requirements)\n- [Install](#install)\n- [Usage](#usage)\n  * [Authentication](#authentication)\n  * [SSL Cert Verification Options](#ssl-cert-verification-options)\n  * [Admin objects](#admin-objects)\n    + [User](#user)\n    + [Group](#group)\n    + [Security](#security)\n    + [Repository](#repository)\n    + [Permission](#permission)\n      - [Artifactory lower than 6.6.0](#artifactory-lower-than-660)\n      - [Artifactory 6.6.0 or higher](#artifactory-660-or-higher)\n  * [Artifacts](#artifacts)\n    + [Get the information about a file or folder](#get-the-information-about-a-file-or-folder)\n    + [Deploy an artifact](#deploy-an-artifact)\n    + [Download an artifact](#download-an-artifact)\n    + [Retrieve artifact properties](#retrieve-artifact-properties)\n    + [Retrieve artifact stats](#retrieve-artifact-stats)\n    + [Copy artifact to a new location](#copy-artifact-to-a-new-location)\n    + [Move artifact to a new location](#move-artifact-to-a-new-location)\n    + [Delete an artifact](#delete-an-artifact)\n  * [Contributing](#contributing)\n\n<!-- tocstop -->\n\n## Requirements\n\n* Python 3.6+\n\n\n## Install\n\n```python\npip install pyartifactory\n```\n\n## Usage\n\n### Authentication\n\nSince Artifactory 6.6.0 there is version 2 of the REST API for permission management, in case you have that version or higher, you need to pass api_version=2 to the constructor when you instantiate the class.\n\n```python\nfrom pyartifactory import Artifactory\nart = Artifactory(url="ARTIFACTORY_URL", auth=(\'USERNAME\',\'PASSWORD_OR_API_KEY\'), api_version=1)\n```\n\n### SSL Cert Verification Options\nSpecify a local cert to use as client side certificate\n\n```python\nfrom pyartifactory import Artifactory\nart = Artifactory(url="ARTIFACTORY_URL", auth=(\'USERNAME\',\'PASSORD_OR_API_KEY\'), cert="/path_to_file/server.pem",api_version=1)\n```\n\nDisable host cert verification\n\n```python\nfrom pyartifactory import Artifactory\nart = Artifactory(url="ARTIFACTORY_URL", auth=(\'USERNAME\',\'PASSORD_OR_API_KEY\'), verify=False, api_version=1)\n```\n\n### Admin objects\n\n#### User\n\nFirst, you need to create a new Artifactory object.\n```python\nfrom pyartifactory import Artifactory\nart = Artifactory(url="ARTIFACTORY_URL", auth=(\'USERNAME\',\'PASSORD_OR_API_KEY\'))\n```\n\nGet the list of users:\n```python\nusers = art.users.list()\n```\n\nGet a single user:\n```python\nuser = art.users.get("test_user")\n```\n\nCreate a user:\n```python\nfrom pyartifactory.models import NewUser\n\n# Create User\nuser = NewUser(name="test_user", password="test_password", email="user@user.com")\nnew_user = art.users.create(user)\n\n# Update user\nuser.email = "test@test.com"\nupdated_user = art.users.update(user)\n```\n\nUpdate a user:\n```python\nfrom pyartifactory.models import User\n\nuser = art.users.get("test_user")\n\n# Update user\nuser.email = "test@test.com"\nupdated_user = art.users.update(user)\n```\n\nDelete a user:\n```python\nart.users.delete("test_user")\n```\n\nUnlock a user:\n```python\nart.users.unlock("test_user")\n```\n\n#### Group\n\nGet the list of groups:\n```python\ngroups = art.groups.list()\n```\n\nGet a single group:\n```python\ngroup = art.groups.get("group_name")\n```\n\nCreate/Update a group:\n```python\nfrom pyartifactory.models import Group\n\n# Create a Group\ngroup = Group(name="test_group", description="test_group")\nnew_group = art.groups.create(group)\n\n# Update a Group\ngroup.description = "test_group_2"\nupdated_group = art.groups.update(group)\n```\n\nDelete a group:\n```python\nart.groups.delete("test_group")\n```\n\n#### Security\n\nA set of methods for performing operations on apiKeys, passwords ...\n```python\n>>> art.security.\nart.security.create_api_key(          art.security.get_encrypted_password(  art.security.revoke_api_key(\nart.security.get_api_key(             art.security.regenerate_api_key(      art.security.revoke_user_api_key(\n```\n\nCreate an access token (for a transient user):\n```python\ntoken = art.security.create_access_token(user_name=\'transient_artifactory_user\',\n                                         groups=[\'g1\', \'g2\'],\n                                         refreshable=True)\n```\n\nCreate an access token for an existing user (groups are implied from the existing user):\n```python\ntoken = art.security.create_access_token(user_name=\'existing_artifactory_user\',\n                                         refreshable=True)\n```\n\nRevoke an existing revocable token:\n```python\nart.security.revoke_access_token(token.access_token)\n```\n\n#### Repository\n\nGet the list of repositories:\n```python\nrepositories = art.repositories.list()\n```\n\nGet a single repository\n```python\nrepo = art.repositories.get_repo("repo_name")\n# According to the repo type, you\'ll have either a local, virtual or remote repository returned\n```\n\nCreate/Update a repository:\n```python\nfrom pyartifactory.models import LocalRepository, VirtualRepository, RemoteRepository\n\n# Create local repo\nlocal_repo = LocalRepository(key="test_local_repo")\nnew_local_repo = art.repositories.create_repo(local_repo)\n\n# Create virtual repo\nvirtual_repo = VirtualRepository(key="test_virtual_repo")\nnew_virtual_repo = art.repositories.create_repo(virtual_repo)\n\n# Create remote repo\nremote_repo = RemoteRepository(key="test_remote_repo")\nnew_remote_repo = art.repositories.create_repo(remote_repo)\n\n# Update a repository\nlocal_repo = art.repositories.get_repo("test_local_repo")\nlocal_repo.description = "test_local_repo"\nupdated_local_repo = art.repositories.update_repo(local_repo)\n```\n\nDelete a repository:\n```python\nart.repositories.delete("test_local_repo")\n```\n\n#### Permission\nGet the list of permissions:\n```python\npermissions = art.permissions.list()\n```\n\nGet a single permission:\n```python\nusers = art.permissions.get("test_permission")\n```\n\nCreate/Update a permission:\n\n##### Artifactory lower than 6.6.0\n\n```python\n\nfrom pyartifactory.models import Permission\n\n# Create a permission\npermission = Permission(\n    **{\n        "name": "test_permission",\n        "repositories": ["test_repository"],\n        "principals": {\n            "users": {"test_user": ["r", "w", "n", "d"]},\n            "groups": {"developers": ["r"]},\n        },\n    }\n)\nperm = art.permissions.create(permission)\n\n# Update permission\npermission.repositories = ["test_repository_2"]\nupdated_permission = art.permissions.update(permission)\n```\n\n##### Artifactory 6.6.0 or higher\n```python\nfrom pyartifactory import Artifactory\nfrom pyartifactory.models import PermissionV2\nfrom pyartifactory.models.permission import PermissionEnumV2, PrincipalsPermissionV2, RepoV2, BuildV2, ReleaseBundleV2\n\n# To use PermissionV2, make sure to set api_version=2\nart = Artifactory(url="ARTIFACTORY_URL", auth=(\'USERNAME\',\'PASSWORD_OR_API_KEY\'), api_version=2)\n\n# Create a permission\npermission = PermissionV2(\n    name="test_permission",\n    repo=RepoV2(\n        repositories=["test_repository"],\n        actions=PrincipalsPermissionV2(\n            users={\n                "test_user": [\n                    PermissionEnumV2.read,\n                    PermissionEnumV2.annotate,\n                    PermissionEnumV2.write,\n                    PermissionEnumV2.delete,\n                ]\n            },\n            groups={\n                "developers": [\n                    PermissionEnumV2.read,\n                    PermissionEnumV2.annotate,\n                    PermissionEnumV2.write,\n                    PermissionEnumV2.delete,\n                ],\n            },\n        ),\n        includePatterns=["**"],\n        excludePatterns=[],\n    ),\n    build=BuildV2(\n          actions=PrincipalsPermissionV2(\n              users={\n                  "test_user": [\n                      PermissionEnumV2.read,\n                      PermissionEnumV2.write,\n                  ]\n              },\n              groups={\n                  "developers": [\n                      PermissionEnumV2.read,\n                      PermissionEnumV2.write,\n                  ],\n              },\n          ),\n          includePatterns=[""],\n          excludePatterns=[""],\n      ),\n    releaseBundle=ReleaseBundleV2(\n          repositories=["release-bundles"],\n          actions=PrincipalsPermissionV2(\n              users={\n                  "test_user": [\n                      PermissionEnumV2.read,\n                  ]\n              },\n              groups={\n                  "developers": [\n                      PermissionEnumV2.read,\n                  ],\n              },\n          ),\n          includePatterns=[""],\n          excludePatterns=[""],\n      )\n  # You don\'t have to set all the objects repo, build and releaseBundle\n  # If you only need repo for example, you can set only the repo object\n)\nperm = art.permissions.create(permission)\n\n# Update permission\npermission.repo.repositories = ["test_repository_2"]\nupdated_permission = art.permissions.update(permission)\n```\n\nDelete a permission:\n```python\nart.permissions.delete("test_permission")\n```\n\n### Artifacts\n\n#### Get the information about a file or folder\n```python\nartifact_info = art.artifacts.info("<ARTIFACT_PATH_IN_ARTIFACTORY>")\n# file_info = art.artifacts.info("my-repository/my/artifact/directory/file.txt")\n# folder_info = art.artifacts.info("my-repository/my/artifact/directory")\n```\n\n#### Deploy an artifact\n```python\nartifact = art.artifacts.deploy("<LOCAL_FILE_LOCATION>", "<ARTIFACT_PATH_IN_ARTIFACTORY>")\n# artifact = art.artifacts.deploy("Desktop/myNewFile.txt", "my-repository/my/new/artifact/directory/file.txt")\n```\n\n#### Download an artifact\n```python\nartifact = art.artifacts.download("<ARTIFACT_PATH_IN_ARTIFACTORY>", "<LOCAL_DIRECTORY_PATH>")\n# artifact = art.artifacts.download("my-artifactory-repository/my/new/artifact/file.txt", "Desktop/my/local/directory")\n# The artifact location is returned by the download method\n# If you have not set a <LOCAL_DIRECTORY_PATH>, the artifact will be downloaded in the current directory\n```\n\n#### Retrieve artifact properties\n```python\nartifact_properties = art.artifacts.properties("<ARTIFACT_PATH_IN_ARTIFACTORY>")  # returns all properties\n# artifact_properties = art.artifacts.properties("my-repository/my/new/artifact/directory/file.txt")\nartifact_properties = art.artifacts.properties("<ARTIFACT_PATH_IN_ARTIFACTORY>", ["prop1", "prop2"])  # returns specific properties\nartifact_properties.properties["prop1"]  # ["value1", "value1-bis"]\n```\n\n#### Retrieve artifact stats\n```python\nartifact_stats = art.artifacts.stats("<ARTIFACT_PATH_IN_ARTIFACTORY>")\n# artifact_stats = art.artifacts.stats("my-repository/my/new/artifact/directory/file.txt")\n```\n\n#### Copy artifact to a new location\n```python\nartifact = art.artifacts.copy("<CURRENT_ARTIFACT_PATH_IN_ARTIFACTORY>","<NEW_ARTIFACT_PATH_IN_ARTIFACTORY>")\n\n# If you want to run a dryRun test, you can do the following:\n# artifact = art.artifacts.copy("my-repository/current/artifact/path/file.txt","my-repository/new/artifact/path/file.txt", dryrun=True)\n# It will return properties of the newly copied artifact\n```\n\n#### Move artifact to a new location\n```python\nartifact = art.artifacts.move("<CURRENT_ARTIFACT_PATH_IN_ARTIFACTORY>","<NEW_ARTIFACT_PATH_IN_ARTIFACTORY>")\n\n# You can also run a dryRun test with the move operation\n# It will return properties of the newly moved artifact\n```\n\n#### Delete an artifact\n```python\nart.artifacts.delete("<ARTIFACT_PATH_IN_ARTIFACTORY>")\n```\n\n\n### Contributing\nPlease read the [Development - Contributing](./CONTRIBUTING.md) guidelines.\n',
     'author': 'Ananias CARVALHO',
     'author_email': 'carvalhoananias@hotmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/anancarv/python-artifactory',
```

### Comparing `PyArtifactory-1.9.6/PKG-INFO` & `PyArtifactory-1.9.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyartifactory
-Version: 1.9.6
+Version: 1.9.7
 Summary: Typed interactions with the Jfrog Artifactory REST API
 Home-page: https://github.com/anancarv/python-artifactory
 License: MIT
 Keywords: artifactory
 Author: Ananias CARVALHO
 Author-email: carvalhoananias@hotmail.com
 Requires-Python: >=3.6.2,<4.0.0
```

