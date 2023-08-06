# Comparing `tmp/jira_amt-1.1.2.tar.gz` & `tmp/jira_amt-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jira_amt-1.1.2.tar", max compression
+gzip compressed data, was "jira_amt-1.2.0.tar", max compression
```

## Comparing `jira_amt-1.1.2.tar` & `jira_amt-1.2.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1069 2023-07-19 16:36:32.109256 jira_amt-1.1.2/LICENSE
--rw-r--r--   0        0        0     2716 2023-07-19 16:36:32.109256 jira_amt-1.1.2/README.md
--rw-r--r--   0        0        0      263 2023-07-19 16:36:32.109256 jira_amt-1.1.2/jira_amt/__init__.py
--rw-r--r--   0        0        0      161 2023-07-19 16:36:32.109256 jira_amt-1.1.2/jira_amt/__main__.py
--rw-r--r--   0        0        0     5722 2023-07-19 16:36:32.109256 jira_amt-1.1.2/jira_amt/cli.py
--rw-r--r--   0        0        0     1971 2023-07-19 16:36:32.109256 jira_amt-1.1.2/jira_amt/config.py
--rw-r--r--   0        0        0     4552 2023-07-19 16:36:32.109256 jira_amt-1.1.2/jira_amt/jira.py
--rw-r--r--   0        0        0     1251 2023-07-19 16:36:32.109256 jira_amt-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     3759 1970-01-01 00:00:00.000000 jira_amt-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-08-06 10:14:53.763165 jira_amt-1.2.0/LICENSE
+-rw-r--r--   0        0        0     3086 2023-08-06 10:14:53.763165 jira_amt-1.2.0/README.md
+-rw-r--r--   0        0        0      263 2023-08-06 10:14:53.763165 jira_amt-1.2.0/jira_amt/__init__.py
+-rw-r--r--   0        0        0      161 2023-08-06 10:14:53.763165 jira_amt-1.2.0/jira_amt/__main__.py
+-rw-r--r--   0        0        0     5886 2023-08-06 10:14:53.763165 jira_amt-1.2.0/jira_amt/cli.py
+-rw-r--r--   0        0        0     1971 2023-08-06 10:14:53.763165 jira_amt-1.2.0/jira_amt/config.py
+-rw-r--r--   0        0        0     4574 2023-08-06 10:14:53.763165 jira_amt-1.2.0/jira_amt/jira.py
+-rw-r--r--   0        0        0     1261 2023-08-06 10:14:53.763165 jira_amt-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4129 1970-01-01 00:00:00.000000 jira_amt-1.2.0/PKG-INFO
```

### Comparing `jira_amt-1.1.2/LICENSE` & `jira_amt-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jira_amt-1.1.2/README.md` & `jira_amt-1.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -7,30 +7,19 @@
 ## Requirements
 
 - Python 3.8+
 
 ## Install
 
 ```bash
-poetry install
-jira-amt --help
+pip install jira-amt
 ```
 
 ## How-to
 
-First, you need to initialize the project:
-
-```bash
-jira-amt init
-```
-
-This will get everything from your Jira server and save them to `~/.jira` directory.
-
-### Configure
-
 You need to add these environment variables to use the CLI:
 
 | Variable    | Description                                        |
 | ----------- | -------------------------------------------------- |
 | JIRA_SERVER | Jira server address like `https://jira.domain.com` |
 | JIRA_PAT    | Your personal access token                         |
 
@@ -38,14 +27,18 @@
 
 ```bash
 jira-amt init
 ```
 
 This command will get everything from your Jira server and save them to `~/.jira` directory for later use. With this data, you don't need to know/use ID of each asset/attribute.
 
+## CLI
+
+There is some commands to manage assets. Check them using the `--help` flag.
+
 ### Update assets
 
 You can update asset's attribute using it's name. The script will get the asset id from the name automatically.
 
 ```bash
 jira-amt attr <schema> <object> <asset name> <attr name> <attr value>
 jira-amt attr "ITSM" "Servers" "Server-1" "IP" "1.2.3.4"
@@ -58,19 +51,50 @@
 ```bash
 jira-amt comment <schema> <object> <asset name> <comment>
 jira-amt comment "ITSM" "Servers" "Server-1" "This is a comment"
 ```
 
 ---
 
-## Support 💛
+## Package
+
+You can use this package in your code to manage Jira assets.
 
-[![Donate with Bitcoin](https://en.cryptobadges.io/badge/micro/bc1qmmh6vt366yzjt3grjxjjqynrrxs3frun8gnxrz)](https://en.cryptobadges.io/donate/bc1qmmh6vt366yzjt3grjxjjqynrrxs3frun8gnxrz) [![Donate with Ethereum](https://en.cryptobadges.io/badge/micro/0x0831bD72Ea8904B38Be9D6185Da2f930d6078094)](https://en.cryptobadges.io/donate/0x0831bD72Ea8904B38Be9D6185Da2f930d6078094)
+```python
+from jira_amt.jira import JiraAssetHandler
+
+jira = JiraAssetHandler(
+    server="https://jira.domain.com",
+    pat="ABCD1234"
+)
+```
+
+### Get asset
+
+```python
+asset = jira.get_asset("schema", "object", "asset's name")
+```
+
+### Create asset
+
+```python
+input = {
+    "Name": "Server-1",
+    "Status": "Running",
+    "Environment": "Production",
+    "OS": "Debian",
+    "IP": "1.2.3.4"
+}
+
+asset = jira.create_asset("schema", "object", input)
+```
+
+## Support 💛
 
-[![ko-fi](https://www.ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/D1D1WGU9)
+[![Donate with Bitcoin](https://img.shields.io/badge/Bitcoin-bc1qmmh6vt366yzjt3grjxjjqynrrxs3frun8gnxrz-orange)](https://donatebadges.ir/donate/Bitcoin/bc1qmmh6vt366yzjt3grjxjjqynrrxs3frun8gnxrz) [![Donate with Ethereum](https://img.shields.io/badge/Ethereum-0x0831bD72Ea8904B38Be9D6185Da2f930d6078094-blueviolet)](https://donatebadges.ir/donate/Ethereum/0x0831bD72Ea8904B38Be9D6185Da2f930d6078094)
 
 <div><a href="https://payping.ir/@hatamiarash7"><img src="https://cdn.payping.ir/statics/Payping-logo/Trust/blue.svg" height="128" width="128"></a></div>
 
 ## Contributing 🤝
 
 Don't be shy and reach out to us if you want to contribute 😉
```

#### html2text {}

```diff
@@ -1,33 +1,38 @@
 # Jira Asset Manager [![made-with-python](https://img.shields.io/badge/
 Made%20with-Python-1f425f.svg)](https://www.python.org/) ![GitHub release
 (release name instead of tag name)](https://img.shields.io/github/v/release/
 hatamiarash7/jira-asset-manager?sort=date) ![GitHub](https://img.shields.io/
 github/license/hatamiarash7/jira-asset-manager) Manage Jira assets in your code
-or CLI. ## Requirements - Python 3.8+ ## Install ```bash poetry install jira-
-amt --help ``` ## How-to First, you need to initialize the project: ```bash
-jira-amt init ``` This will get everything from your Jira server and save them
-to `~/.jira` directory. ### Configure You need to add these environment
-variables to use the CLI: | Variable | Description | | ----------- | ----------
----------------------------------------- | | JIRA_SERVER | Jira server address
-like `https://jira.domain.com` | | JIRA_PAT | Your personal access token |
-After setting these variables, you can configure the CLI: ```bash jira-amt init
-``` This command will get everything from your Jira server and save them to
-`~/.jira` directory for later use. With this data, you don't need to know/use
-ID of each asset/attribute. ### Update assets You can update asset's attribute
+or CLI. ## Requirements - Python 3.8+ ## Install ```bash pip install jira-amt
+``` ## How-to You need to add these environment variables to use the CLI: |
+Variable | Description | | ----------- | --------------------------------------
+------------ | | JIRA_SERVER | Jira server address like `https://
+jira.domain.com` | | JIRA_PAT | Your personal access token | After setting
+these variables, you can configure the CLI: ```bash jira-amt init ``` This
+command will get everything from your Jira server and save them to `~/.jira`
+directory for later use. With this data, you don't need to know/use ID of each
+asset/attribute. ## CLI There is some commands to manage assets. Check them
+using the `--help` flag. ### Update assets You can update asset's attribute
 using it's name. The script will get the asset id from the name automatically.
 ```bash jira-amt attr      jira-amt attr "ITSM" "Servers" "Server-1" "IP"
 "1.2.3.4" ``` ### Add comment You can add comment to an asset using it's name.
 The script will get the asset id from the name automatically. ```bash jira-amt
 comment     jira-amt comment "ITSM" "Servers" "Server-1" "This is a comment"
-``` --- ## Support ð [![Donate with Bitcoin](https://en.cryptobadges.io/
-badge/micro/bc1qmmh6vt366yzjt3grjxjjqynrrxs3frun8gnxrz)](https://
-en.cryptobadges.io/donate/bc1qmmh6vt366yzjt3grjxjjqynrrxs3frun8gnxrz) [![Donate
-with Ethereum](https://en.cryptobadges.io/badge/micro/
-0x0831bD72Ea8904B38Be9D6185Da2f930d6078094)](https://en.cryptobadges.io/donate/
-0x0831bD72Ea8904B38Be9D6185Da2f930d6078094) [![ko-fi](https://www.ko-fi.com/
-img/githubbutton_sm.svg)](https://ko-fi.com/D1D1WGU9)
+``` --- ## Package You can use this package in your code to manage Jira assets.
+```python from jira_amt.jira import JiraAssetHandler jira = JiraAssetHandler
+( server="https://jira.domain.com", pat="ABCD1234" ) ``` ### Get asset
+```python asset = jira.get_asset("schema", "object", "asset's name") ``` ###
+Create asset ```python input = { "Name": "Server-1", "Status": "Running",
+"Environment": "Production", "OS": "Debian", "IP": "1.2.3.4" } asset =
+jira.create_asset("schema", "object", input) ``` ## Support ð [![Donate with
+Bitcoin](https://img.shields.io/badge/Bitcoin-
+bc1qmmh6vt366yzjt3grjxjjqynrrxs3frun8gnxrz-orange)](https://donatebadges.ir/
+donate/Bitcoin/bc1qmmh6vt366yzjt3grjxjjqynrrxs3frun8gnxrz) [![Donate with
+Ethereum](https://img.shields.io/badge/Ethereum-
+0x0831bD72Ea8904B38Be9D6185Da2f930d6078094-blueviolet)](https://
+donatebadges.ir/donate/Ethereum/0x0831bD72Ea8904B38Be9D6185Da2f930d6078094)
 [https://cdn.payping.ir/statics/Payping-logo/Trust/blue.svg]
 ## Contributing ð¤ Don't be shy and reach out to us if you want to contribute
 ð 1. Fork it! 2. Create your feature branch: `git checkout -b my-new-
 feature` 3. Commit your changes: `git commit -am 'Add some feature'` 4. Push to
 the branch: `git push origin my-new-feature`
```

### Comparing `jira_amt-1.1.2/jira_amt/cli.py` & `jira_amt-1.2.0/jira_amt/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,19 +26,22 @@
     # Create schemas file
     schema_list = document()
     typer.secho("  -> Fetching schemas", fg=typer.colors.BRIGHT_GREEN)
     schema_list.add(
         cm(f"Jira Asset Management - Status list - v{__version__}")
     )
     schemas = json.loads(get_jira().get_schema().text)
+    objects = []
     for schema in schemas['objectschemas']:
         title = f"{schema['id']}:{schema['name']}"
         schema_list.add(title, table())
-        objects = json.loads(get_jira().get_objecttypes(schema['id']).text)
-        for object in objects:
+        objs = json.loads(get_jira().get_objecttypes(schema['id']).text)
+        for object in objs:
+            object['schema'] = schema['name']
+            objects.append(object)
             schema_list[title].add(object['name'].lower(), object['id'])
     with open(
         config.WORK_DIR+"/schemas.toml",
         mode="w",
         encoding="utf-8"
     ) as file:
         toml.dump(schema_list, file)
@@ -53,15 +56,18 @@
         result = json.loads(get_jira().get_attributes(object['id']).text)
         attributes = table()
         for attribute in result:
             attributes.add(
                 attribute['name'].lower() + "." + str(attribute['type']),
                 attribute['id']
             )
-        attr_list.add(object['name'].lower(), attributes)
+        attr_list.add(
+            object['name'].lower() + "." + str(object['schema']).lower(),
+            attributes
+        )
     with open(
         config.WORK_DIR+"/attributes.toml",
         mode="w",
         encoding="utf-8"
     ) as file:
         toml.dump(attr_list, file)
```

### Comparing `jira_amt-1.1.2/jira_amt/config.py` & `jira_amt-1.2.0/jira_amt/config.py`

 * *Files identical despite different names*

### Comparing `jira_amt-1.1.2/jira_amt/jira.py` & `jira_amt-1.2.0/jira_amt/jira.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,23 +31,23 @@
     def create_asset(self, schema, object, attributes):
         schema_id = config.getSchema(schema)
 
         input = []
 
         for attribute_name, value in attributes.items():
             object_type_attribute_id = config.getAttribute(
-                object,
+                object+"."+schema,
                 attribute_name
             )
 
             if object_type_attribute_id is not None and isinstance(value, list):
                 output_dict = {
                     "objectTypeAttributeId": object_type_attribute_id,
                     "objectAttributeValues": [{"value": config.getAttributeValue(
-                        object,
+                        object+"."+schema,
                         attribute_name,
                         v
                     )} for v in value]
                 }
 
                 input.append(output_dict)
             elif object_type_attribute_id is not None:
```

### Comparing `jira_amt-1.1.2/pyproject.toml` & `jira_amt-1.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,56 @@
 [tool.poetry]
-name = "jira-amt"
-version = "1.1.2"
-license = "MIT"
+authors = [
+  "Arash Hatami <hatamiarash7@gmail.com>",
+]
+classifiers = [
+  "Topic :: Software Development",
+  "Topic :: Software Development :: Libraries",
+  "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.8",
+  "Programming Language :: Python :: 3",
+  "License :: OSI Approved :: MIT License",
+  "Development Status :: 5 - Production/Stable",
+]
 description = "Manage Jira assets."
-authors = ["Arash Hatami <hatamiarash7@gmail.com>"]
-readme = "README.md"
 homepage = "https://arash-hatami.ir"
-repository = "https://github.com/hatamiarash7/jira-asset-manager"
-keywords = ["jira", "asset"]
-classifiers = [
-    "Topic :: Software Development",
-    "Topic :: Software Development :: Libraries",
-    "Programming Language :: Python :: 3.11",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Development Status :: 5 - Production/Stable"
+keywords = [
+  "jira",
+  "asset",
+]
+license = "MIT"
+name = "jira-amt"
+packages = [
+  {include = "jira_amt"},
 ]
-packages = [{include = "jira_amt"}]
+readme = "README.md"
+repository = "https://github.com/hatamiarash7/jira-asset-manager"
+version = "1.2.0"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-typer = {extras = ["all"], version = "^0.9.0"}
 requests = "^2"
+tomlkit = "^0.12.0"
+typer = {extras = [
+  "all",
+], version = "^0.9.0"}
 urllib3 = "^1"
-tomlkit = "^0.11.8"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7"
 
 [tool.poetry.scripts]
 jira-amt = "jira_amt.cli:app"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/hatamiarash7/jira-asset-manager/issues"
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+requires = [
+  "poetry-core>=1.0.0",
+]
```

### Comparing `jira_amt-1.1.2/PKG-INFO` & `jira_amt-1.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jira-amt
-Version: 1.1.2
+Version: 1.2.0
 Summary: Manage Jira assets.
 Home-page: https://arash-hatami.ir
 License: MIT
 Keywords: jira,asset
 Author: Arash Hatami
 Author-email: hatamiarash7@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Requires-Dist: requests (>=2,<3)
-Requires-Dist: tomlkit (>=0.11.8,<0.12.0)
+Requires-Dist: tomlkit (>=0.12.0,<0.13.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Requires-Dist: urllib3 (>=1,<2)
 Project-URL: Bug Tracker, https://github.com/hatamiarash7/jira-asset-manager/issues
 Project-URL: Repository, https://github.com/hatamiarash7/jira-asset-manager
 Description-Content-Type: text/markdown
 
 # Jira Asset Manager
@@ -34,30 +34,19 @@
 ## Requirements
 
 - Python 3.8+
 
 ## Install
 
 ```bash
-poetry install
-jira-amt --help
+pip install jira-amt
 ```
 
 ## How-to
 
-First, you need to initialize the project:
-
-```bash
-jira-amt init
-```
-
-This will get everything from your Jira server and save them to `~/.jira` directory.
-
-### Configure
-
 You need to add these environment variables to use the CLI:
 
 | Variable    | Description                                        |
 | ----------- | -------------------------------------------------- |
 | JIRA_SERVER | Jira server address like `https://jira.domain.com` |
 | JIRA_PAT    | Your personal access token                         |
 
@@ -65,14 +54,18 @@
 
 ```bash
 jira-amt init
 ```
 
 This command will get everything from your Jira server and save them to `~/.jira` directory for later use. With this data, you don't need to know/use ID of each asset/attribute.
 
+## CLI
+
+There is some commands to manage assets. Check them using the `--help` flag.
+
 ### Update assets
 
 You can update asset's attribute using it's name. The script will get the asset id from the name automatically.
 
 ```bash
 jira-amt attr <schema> <object> <asset name> <attr name> <attr value>
 jira-amt attr "ITSM" "Servers" "Server-1" "IP" "1.2.3.4"
@@ -85,19 +78,50 @@
 ```bash
 jira-amt comment <schema> <object> <asset name> <comment>
 jira-amt comment "ITSM" "Servers" "Server-1" "This is a comment"
 ```
 
 ---
 
-## Support 💛
+## Package
+
+You can use this package in your code to manage Jira assets.
 
-[![Donate with Bitcoin](https://en.cryptobadges.io/badge/micro/bc1qmmh6vt366yzjt3grjxjjqynrrxs3frun8gnxrz)](https://en.cryptobadges.io/donate/bc1qmmh6vt366yzjt3grjxjjqynrrxs3frun8gnxrz) [![Donate with Ethereum](https://en.cryptobadges.io/badge/micro/0x0831bD72Ea8904B38Be9D6185Da2f930d6078094)](https://en.cryptobadges.io/donate/0x0831bD72Ea8904B38Be9D6185Da2f930d6078094)
+```python
+from jira_amt.jira import JiraAssetHandler
+
+jira = JiraAssetHandler(
+    server="https://jira.domain.com",
+    pat="ABCD1234"
+)
+```
+
+### Get asset
+
+```python
+asset = jira.get_asset("schema", "object", "asset's name")
+```
+
+### Create asset
+
+```python
+input = {
+    "Name": "Server-1",
+    "Status": "Running",
+    "Environment": "Production",
+    "OS": "Debian",
+    "IP": "1.2.3.4"
+}
+
+asset = jira.create_asset("schema", "object", input)
+```
+
+## Support 💛
 
-[![ko-fi](https://www.ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/D1D1WGU9)
+[![Donate with Bitcoin](https://img.shields.io/badge/Bitcoin-bc1qmmh6vt366yzjt3grjxjjqynrrxs3frun8gnxrz-orange)](https://donatebadges.ir/donate/Bitcoin/bc1qmmh6vt366yzjt3grjxjjqynrrxs3frun8gnxrz) [![Donate with Ethereum](https://img.shields.io/badge/Ethereum-0x0831bD72Ea8904B38Be9D6185Da2f930d6078094-blueviolet)](https://donatebadges.ir/donate/Ethereum/0x0831bD72Ea8904B38Be9D6185Da2f930d6078094)
 
 <div><a href="https://payping.ir/@hatamiarash7"><img src="https://cdn.payping.ir/statics/Payping-logo/Trust/blue.svg" height="128" width="128"></a></div>
 
 ## Contributing 🤝
 
 Don't be shy and reach out to us if you want to contribute 😉
```

#### html2text {}

```diff
@@ -1,47 +1,51 @@
-Metadata-Version: 2.1 Name: jira-amt Version: 1.1.2 Summary: Manage Jira
+Metadata-Version: 2.1 Name: jira-amt Version: 1.2.0 Summary: Manage Jira
 assets. Home-page: https://arash-hatami.ir License: MIT Keywords: jira,asset
 Author: Arash Hatami Author-email: hatamiarash7@gmail.com Requires-Python:
 >=3.8,<4.0 Classifier: Development Status :: 5 - Production/Stable Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Topic :: Software Development Classifier: Topic :: Software Development ::
 Libraries Requires-Dist: requests (>=2,<3) Requires-Dist: tomlkit
-(>=0.11.8,<0.12.0) Requires-Dist: typer[all] (>=0.9.0,<0.10.0) Requires-Dist:
+(>=0.12.0,<0.13.0) Requires-Dist: typer[all] (>=0.9.0,<0.10.0) Requires-Dist:
 urllib3 (>=1,<2) Project-URL: Bug Tracker, https://github.com/hatamiarash7/
 jira-asset-manager/issues Project-URL: Repository, https://github.com/
 hatamiarash7/jira-asset-manager Description-Content-Type: text/markdown # Jira
 Asset Manager [![made-with-python](https://img.shields.io/badge/Made%20with-
 Python-1f425f.svg)](https://www.python.org/) ![GitHub release (release name
 instead of tag name)](https://img.shields.io/github/v/release/hatamiarash7/
 jira-asset-manager?sort=date) ![GitHub](https://img.shields.io/github/license/
 hatamiarash7/jira-asset-manager) Manage Jira assets in your code or CLI. ##
-Requirements - Python 3.8+ ## Install ```bash poetry install jira-amt --help
-``` ## How-to First, you need to initialize the project: ```bash jira-amt init
-``` This will get everything from your Jira server and save them to `~/.jira`
-directory. ### Configure You need to add these environment variables to use the
-CLI: | Variable | Description | | ----------- | -------------------------------
-------------------- | | JIRA_SERVER | Jira server address like `https://
-jira.domain.com` | | JIRA_PAT | Your personal access token | After setting
-these variables, you can configure the CLI: ```bash jira-amt init ``` This
-command will get everything from your Jira server and save them to `~/.jira`
-directory for later use. With this data, you don't need to know/use ID of each
-asset/attribute. ### Update assets You can update asset's attribute using it's
-name. The script will get the asset id from the name automatically. ```bash
-jira-amt attr      jira-amt attr "ITSM" "Servers" "Server-1" "IP" "1.2.3.4" ```
-### Add comment You can add comment to an asset using it's name. The script
-will get the asset id from the name automatically. ```bash jira-amt comment
-jira-amt comment "ITSM" "Servers" "Server-1" "This is a comment" ``` --- ##
-Support ð [![Donate with Bitcoin](https://en.cryptobadges.io/badge/micro/
-bc1qmmh6vt366yzjt3grjxjjqynrrxs3frun8gnxrz)](https://en.cryptobadges.io/donate/
-bc1qmmh6vt366yzjt3grjxjjqynrrxs3frun8gnxrz) [![Donate with Ethereum](https://
-en.cryptobadges.io/badge/micro/0x0831bD72Ea8904B38Be9D6185Da2f930d6078094)]
-(https://en.cryptobadges.io/donate/0x0831bD72Ea8904B38Be9D6185Da2f930d6078094)
-[![ko-fi](https://www.ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/
-D1D1WGU9)
+Requirements - Python 3.8+ ## Install ```bash pip install jira-amt ``` ## How-
+to You need to add these environment variables to use the CLI: | Variable |
+Description | | ----------- | -------------------------------------------------
+- | | JIRA_SERVER | Jira server address like `https://jira.domain.com` | |
+JIRA_PAT | Your personal access token | After setting these variables, you can
+configure the CLI: ```bash jira-amt init ``` This command will get everything
+from your Jira server and save them to `~/.jira` directory for later use. With
+this data, you don't need to know/use ID of each asset/attribute. ## CLI There
+is some commands to manage assets. Check them using the `--help` flag. ###
+Update assets You can update asset's attribute using it's name. The script will
+get the asset id from the name automatically. ```bash jira-amt attr      jira-
+amt attr "ITSM" "Servers" "Server-1" "IP" "1.2.3.4" ``` ### Add comment You can
+add comment to an asset using it's name. The script will get the asset id from
+the name automatically. ```bash jira-amt comment     jira-amt comment "ITSM"
+"Servers" "Server-1" "This is a comment" ``` --- ## Package You can use this
+package in your code to manage Jira assets. ```python from jira_amt.jira import
+JiraAssetHandler jira = JiraAssetHandler( server="https://jira.domain.com",
+pat="ABCD1234" ) ``` ### Get asset ```python asset = jira.get_asset("schema",
+"object", "asset's name") ``` ### Create asset ```python input = { "Name":
+"Server-1", "Status": "Running", "Environment": "Production", "OS": "Debian",
+"IP": "1.2.3.4" } asset = jira.create_asset("schema", "object", input) ``` ##
+Support ð [![Donate with Bitcoin](https://img.shields.io/badge/Bitcoin-
+bc1qmmh6vt366yzjt3grjxjjqynrrxs3frun8gnxrz-orange)](https://donatebadges.ir/
+donate/Bitcoin/bc1qmmh6vt366yzjt3grjxjjqynrrxs3frun8gnxrz) [![Donate with
+Ethereum](https://img.shields.io/badge/Ethereum-
+0x0831bD72Ea8904B38Be9D6185Da2f930d6078094-blueviolet)](https://
+donatebadges.ir/donate/Ethereum/0x0831bD72Ea8904B38Be9D6185Da2f930d6078094)
 [https://cdn.payping.ir/statics/Payping-logo/Trust/blue.svg]
 ## Contributing ð¤ Don't be shy and reach out to us if you want to contribute
 ð 1. Fork it! 2. Create your feature branch: `git checkout -b my-new-
 feature` 3. Commit your changes: `git commit -am 'Add some feature'` 4. Push to
 the branch: `git push origin my-new-feature`
```

