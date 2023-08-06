# Comparing `tmp/tftui-0.3.0.tar.gz` & `tmp/tftui-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tftui-0.3.0.tar", last modified: Sun Jul 23 14:02:06 2023, max compression
+gzip compressed data, was "tftui-0.3.1.tar", last modified: Sun Aug  6 06:27:36 2023, max compression
```

## Comparing `tftui-0.3.0.tar` & `tftui-0.3.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:02:06.991974 tftui-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-23 14:01:52.000000 tftui-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-23 14:01:52.000000 tftui-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14254 2023-07-23 14:02:06.991974 tftui-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-23 14:01:52.000000 tftui-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-23 14:01:52.000000 tftui-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-23 14:02:06.991974 tftui-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:02:06.987974 tftui-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:02:06.987974 tftui-0.3.0/src/tftui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 14:01:52.000000 tftui-0.3.0/src/tftui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9278 2023-07-23 14:01:52.000000 tftui-0.3.0/src/tftui/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-23 14:01:52.000000 tftui-0.3.0/src/tftui/ui.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:02:06.991974 tftui-0.3.0/src/tftui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14254 2023-07-23 14:02:06.000000 tftui-0.3.0/src/tftui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-23 14:02:06.000000 tftui-0.3.0/src/tftui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 14:02:06.000000 tftui-0.3.0/src/tftui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-23 14:02:06.000000 tftui-0.3.0/src/tftui.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-23 14:02:06.000000 tftui-0.3.0/src/tftui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-23 14:02:06.000000 tftui-0.3.0/src/tftui.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 06:27:36.015064 tftui-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-06 06:27:22.000000 tftui-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-06 06:27:22.000000 tftui-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    15105 2023-08-06 06:27:36.015064 tftui-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-08-06 06:27:22.000000 tftui-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-08-06 06:27:23.000000 tftui-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 06:27:36.015064 tftui-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 06:27:36.011064 tftui-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 06:27:36.015064 tftui-0.3.1/src/tftui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 06:27:22.000000 tftui-0.3.1/src/tftui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9516 2023-08-06 06:27:22.000000 tftui-0.3.1/src/tftui/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-08-06 06:27:22.000000 tftui-0.3.1/src/tftui/ui.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 06:27:36.015064 tftui-0.3.1/src/tftui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15105 2023-08-06 06:27:36.000000 tftui-0.3.1/src/tftui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-08-06 06:27:36.000000 tftui-0.3.1/src/tftui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 06:27:36.000000 tftui-0.3.1/src/tftui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-06 06:27:36.000000 tftui-0.3.1/src/tftui.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-06 06:27:36.000000 tftui-0.3.1/src/tftui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-06 06:27:36.000000 tftui-0.3.1/src/tftui.egg-info/top_level.txt
```

### Comparing `tftui-0.3.0/LICENSE` & `tftui-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tftui-0.3.0/PKG-INFO` & `tftui-0.3.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tftui
-Version: 0.3.0
+Version: 0.3.1
 Summary: Terraform Textual User Interface
 Author: Ido Avraham
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -210,34 +210,40 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# TFTUI - The terraform textual UI
-`TFTUI` is a textual gui that disaplys a terraform state and allows the user to read and interact with it.
+# TFTUI - The Terraform textual UI
 
-## Features
+`TFTUI` is a powerful textual GUI that empowers users to effortlessly view and interact with their Terraform state.
+
+With its latest version [0.3.0](https://github.com/idoavrah/terraform-tui/releases/tag/v0.3.0) you can easily visualize the complete state tree, gaining deeper insights into your infrastructure's current configuration. Additionally, the ability to inspect individual resource states allows you to focus on specific details for better analysis and management. Lastly, it's now possible to select resources and perform actions such as tainting and untainting.
+
+## Key Features
 
 ### version 0.3
 - [x] Added loading screen and status bar
 - [x] Added selection of resources
 - [x] Added refresh state functionality
 - [x] Added taint/untaint functionality
 - [x] Refactoring
 
 ### version 0.2
-- [x] Display terraform state tree
-- [x] Display a single resource state
+- [x] Comprehensive display of the entire Terraform state tree.
+- [x] Effortlessly view and navigate through a single resource state.
 
 ## Demo
 
 ![](https://github.com/idoavrah/terraform-tui/raw/main/demo/demo.gif "demo")
 
 ## Installation
 
-| Tool            | Install             | Upgrade                       |
-|-----------------| ------------------- | ----------------------------- |
-| PIP             | `pip install tftui` | `pip install --upgrade tftui` |
-| PIPX            | `pipx install tftui`| `pipx upgrade tftui`          |
+| Tool            | Install             | Upgrade                       | Run                                      |
+|-----------------| ------------------- | ----------------------------- | ---------------------------------------- |
+| PIP             | `pip install tftui` | `pip install --upgrade tftui` | `cd /path/to/terraform/project && tftui` |
+| PIPX            | `pipx install tftui`| `pipx upgrade tftui`          | `cd /path/to/terraform/project && tftui` |
+
+## Stargazers over time
+[![Stargazers over time](https://starchart.cc/idoavrah/terraform-tui.svg)](https://starchart.cc/idoavrah/terraform-tui)
```

### Comparing `tftui-0.3.0/pyproject.toml` & `tftui-0.3.1/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tftui"
-version = "0.3.0"
+version = "0.3.1"
 description = "Terraform Textual User Interface"
 readme = "README.md"
 authors = [{ name = "Ido Avraham" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
```

### Comparing `tftui-0.3.0/src/tftui/__main__.py` & `tftui-0.3.1/src/tftui/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,110 +1,121 @@
 from textual import work
 from textual.app import App, ComposeResult, Binding
-from textual.widgets import Header, Footer, Tree, TextLog, LoadingIndicator, ContentSwitcher, Static, Button
+from textual.widgets import (
+    Header,
+    Footer,
+    Tree,
+    TextLog,
+    LoadingIndicator,
+    ContentSwitcher,
+    Static,
+    Button,
+)
 from textual.containers import Vertical, Horizontal
 from shutil import which
 import asyncio
 
 
 class StateTree(Tree):
-
     current_node = None
     selected_nodes = []
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.guide_depth = 3
         self.root.data = ""
 
     def on_tree_node_highlighted(self, node) -> None:
         self.current_node = node.node
 
     def on_tree_node_selected(self) -> None:
         if self.current_node is None:
             return
-        if self.current_node.data.startswith('module') or self.current_node.is_root:
+        if self.current_node.data.startswith("module") or self.current_node.is_root:
             return
         self.app.resource.clear()
         self.app.resource.write(self.current_node.data)
         self.app.switcher.current = "resource"
 
     def select_current_node(self) -> None:
         if self.current_node is None:
             return
-        if self.current_node.data.startswith('module') or self.current_node.data.startswith('data') or self.current_node.is_root:
+        if (
+            self.current_node.data.startswith("module")
+            or self.current_node.data.startswith("data")
+            or self.current_node.is_root
+        ):
             return
         if self.current_node in self.selected_nodes:
             self.selected_nodes.remove(self.current_node)
             label = self.current_node.label
             label.right_crop(4)
             self.current_node.set_label(label)
         else:
             self.selected_nodes.append(self.current_node)
             self.current_node.set_label(self.current_node.label.append(" [X]"))
 
     @work(exclusive=True)
     async def refresh_state(self) -> None:
-
         self.app.switcher.current = "loading"
         self.selected_nodes = []
         self.current_node = None
         self.clear()
         self.app.status.update("Executing Terraform init")
 
         returncode, stdout = await execute_async("terraform", "init", "-no-color")
         if returncode != 0:
             self.app.exit(message=stdout)
             return
 
         self.app.status.update("Executing Terraform show")
 
         returncode, stdout = await execute_async("terraform", "show", "-no-color")
-        if returncode != 0 or not stdout.startswith('#'):
+        if returncode != 0 or not stdout.startswith("#"):
             self.app.exit(message=stdout)
             return
 
         self.app.status.update("Building state tree")
         lines = stdout.splitlines()
 
         # build module tree
         modules = set()
         module_nodes = {}
         for line in lines:
-            if not line.startswith('# module'):
+            if not line.startswith("# module"):
                 continue
-            parts = line[2:-1].split('.')
+            parts = line[2:-1].split(".")
             i = 0
             module = ""
-            while parts[i] == 'module':
+            while parts[i] == "module":
                 module += f"{parts[i]}.{parts[i+1]}."
                 modules.add(module[:-1])
                 i += 2
         for module_fullname in sorted(modules):
-            parts = module_fullname.split('.')
+            parts = module_fullname.split(".")
             qualifier = ""
             i = 0
             while i < len(parts):
                 qualifier = f"{parts[i]}.{parts[i+1]}."
                 if qualifier[:-1] not in module_nodes:
                     node = self.root.add(qualifier[:-1], data=module_fullname)
                     module_nodes[qualifier[:-1]] = node
                 i += 2
 
         # parse objects
         name = ""
         for line in lines:
-            if line.startswith('#'):
-                parts = line[2:].split('.')
+            if line.startswith("#"):
+                parts = line[2:].split(".")
                 i = 0
                 qualifier = ""
-                while parts[i] == 'module':
+                while parts[i] == "module":
                     qualifier = f"{parts[i]}.{parts[i+1]}."
                     i += 2
-                name = '.'.join(parts[i:]).replace(':', '')
+                name = ".".join(parts[i:]).replace(":", "")
                 data = ""
                 if qualifier[:-1] in module_nodes:
                     module_node = module_nodes[qualifier[:-1]]
                 else:
                     module_node = self.root
             elif line == "}":
                 data += line + "\n"
@@ -115,15 +126,14 @@
         self.root.expand_all()
         self.app.status.update("")
         self.app.switcher.current = "tree"
         self.app.tree.focus()
 
 
 class TerraformTUI(App):
-
     status = None
     switcher = None
     tree = None
     resource = None
     question = None
     action = None
     selected_action = None
@@ -141,23 +151,30 @@
         ("s", "select", "Select"),
         ("t", "taint", "Taint"),
         ("u", "untaint", "Untaint"),
         ("r", "refresh", "Refresh state"),
         ("m", "toggle_dark", "Toggle dark mode"),
         Binding("y", "yes", "Yes", show=False),
         Binding("n", "no", "No", show=False),
-        ("q", "quit", "Quit")
+        ("q", "quit", "Quit"),
     ]
 
     def compose(self) -> ComposeResult:
         yield Header(classes="header")
         with ContentSwitcher(id="switcher", initial="loading"):
             yield LoadingIndicator(id="loading")
             yield StateTree("State", id="tree")
-            yield TextLog(id="resource", highlight=True, markup=True, wrap=True, classes="resource", auto_scroll=False)
+            yield TextLog(
+                id="resource",
+                highlight=True,
+                markup=True,
+                wrap=True,
+                classes="resource",
+                auto_scroll=False,
+            )
             with Vertical(id="action"):
                 yield TextLog(id="question", auto_scroll=False)
                 with Horizontal():
                     yield Button("Yes", id="yes", variant="primary")
                     yield Button("No", id="no", variant="error")
         yield Static(id="status", classes="status")
         yield Footer()
@@ -177,15 +194,19 @@
         if event.button.id == "yes":
             await self.perform_action()
         elif event.button.id == "no":
             self.action_no()
 
     async def perform_taint_untaint(self, what_to_do: str) -> None:
         resources = [
-            f"{node.parent.data}.{node.label.plain[:-4]}".lstrip(".").replace(' (tainted)', '') for node in self.tree.selected_nodes]
+            f"{node.parent.data}.{node.label.plain[:-4]}".lstrip(".").replace(
+                " (tainted)", ""
+            )
+            for node in self.tree.selected_nodes
+        ]
         for resource in resources:
             await execute_async("terraform", what_to_do, resource)
 
     async def perform_action(self) -> None:
         if self.switcher.current != "action":
             return
         if self.selected_action == "taint" or self.selected_action == "untaint":
@@ -197,15 +218,18 @@
     async def action_yes(self) -> None:
         await self.perform_action()
 
     def action_no(self) -> None:
         self.action_back()
 
     def action_back(self) -> None:
-        if not self.switcher.current == "resource" and not self.switcher.current == "action":
+        if (
+            not self.switcher.current == "resource"
+            and not self.switcher.current == "action"
+        ):
             return
         self.switcher.current = "tree"
         self.tree.focus()
 
     def action_select(self) -> None:
         if not self.switcher.current == "tree":
             return
@@ -218,17 +242,22 @@
     def action_taint_untaint(self, what_to_do: str) -> None:
         if not self.switcher.current == "tree":
             return
         if not self.tree.selected_nodes:
             return
         self.selected_action = what_to_do
         self.question.clear()
-        resources = [f"{node.parent.data}.{node.label.plain[:-4]}".lstrip('.') for node in self.tree.selected_nodes]
-        self.question.write(f"Are you sure you wish to {what_to_do} the selected resources?\n\n - " +
-                            "\n - ".join(resources))
+        resources = [
+            f"{node.parent.data}.{node.label.plain[:-4]}".lstrip(".")
+            for node in self.tree.selected_nodes
+        ]
+        self.question.write(
+            f"Are you sure you wish to {what_to_do} the selected resources?\n\n - "
+            + "\n - ".join(resources)
+        )
         self.switcher.current = "action"
 
     def action_taint(self) -> None:
         self.action_taint_untaint("taint")
 
     def action_untaint(self) -> None:
         self.action_taint_untaint("untaint")
@@ -239,26 +268,25 @@
         self.tree.refresh_state()
 
     def action_toggle_dark(self) -> None:
         self.dark = not self.dark
 
 
 async def execute_async(*command: str) -> tuple[str, str]:
-    proc = await asyncio.create_subprocess_exec(*command,
-                                                stdout=asyncio.subprocess.PIPE,
-                                                stderr=asyncio.subprocess.STDOUT)
+    proc = await asyncio.create_subprocess_exec(
+        *command, stdout=asyncio.subprocess.PIPE, stderr=asyncio.subprocess.STDOUT
+    )
 
     stdout, strerr = await proc.communicate()
-    response = stdout.decode('utf-8')
+    response = stdout.decode("utf-8")
 
     return (proc.returncode, response)
 
 
 def main() -> None:
-
     if which("terraform") is None:
         print("Terraform not found. Please install Terraform and try again.")
         return
 
     app = TerraformTUI()
     result = app.run()
     if result is not None:
```

### Comparing `tftui-0.3.0/src/tftui/ui.css` & `tftui-0.3.1/src/tftui/ui.css`

 * *Files 19% similar despite different names*

```diff
@@ -28,15 +28,15 @@
   padding: 2;
   align: center bottom;
 }
 
 Horizontal {
   column-span: 2;
   align: center middle;
-  
+
 }
 
 #question {
   width: 100%;
   height: 100%;
   column-span: 2;
   content-align: center bottom;
```

### Comparing `tftui-0.3.0/src/tftui.egg-info/PKG-INFO` & `tftui-0.3.1/src/tftui.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tftui
-Version: 0.3.0
+Version: 0.3.1
 Summary: Terraform Textual User Interface
 Author: Ido Avraham
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -210,34 +210,40 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# TFTUI - The terraform textual UI
-`TFTUI` is a textual gui that disaplys a terraform state and allows the user to read and interact with it.
+# TFTUI - The Terraform textual UI
 
-## Features
+`TFTUI` is a powerful textual GUI that empowers users to effortlessly view and interact with their Terraform state.
+
+With its latest version [0.3.0](https://github.com/idoavrah/terraform-tui/releases/tag/v0.3.0) you can easily visualize the complete state tree, gaining deeper insights into your infrastructure's current configuration. Additionally, the ability to inspect individual resource states allows you to focus on specific details for better analysis and management. Lastly, it's now possible to select resources and perform actions such as tainting and untainting.
+
+## Key Features
 
 ### version 0.3
 - [x] Added loading screen and status bar
 - [x] Added selection of resources
 - [x] Added refresh state functionality
 - [x] Added taint/untaint functionality
 - [x] Refactoring
 
 ### version 0.2
-- [x] Display terraform state tree
-- [x] Display a single resource state
+- [x] Comprehensive display of the entire Terraform state tree.
+- [x] Effortlessly view and navigate through a single resource state.
 
 ## Demo
 
 ![](https://github.com/idoavrah/terraform-tui/raw/main/demo/demo.gif "demo")
 
 ## Installation
 
-| Tool            | Install             | Upgrade                       |
-|-----------------| ------------------- | ----------------------------- |
-| PIP             | `pip install tftui` | `pip install --upgrade tftui` |
-| PIPX            | `pipx install tftui`| `pipx upgrade tftui`          |
+| Tool            | Install             | Upgrade                       | Run                                      |
+|-----------------| ------------------- | ----------------------------- | ---------------------------------------- |
+| PIP             | `pip install tftui` | `pip install --upgrade tftui` | `cd /path/to/terraform/project && tftui` |
+| PIPX            | `pipx install tftui`| `pipx upgrade tftui`          | `cd /path/to/terraform/project && tftui` |
+
+## Stargazers over time
+[![Stargazers over time](https://starchart.cc/idoavrah/terraform-tui.svg)](https://starchart.cc/idoavrah/terraform-tui)
```

