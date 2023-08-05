# Comparing `tmp/Fletxible-0.5.9.tar.gz` & `tmp/Fletxible-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Fletxible-0.5.9.tar", last modified: Tue May 30 15:37:29 2023, max compression
+gzip compressed data, was "Fletxible-0.6.0.tar", last modified: Sat Aug  5 22:17:19 2023, max compression
```

## Comparing `Fletxible-0.5.9.tar` & `Fletxible-0.6.0.tar`

### file list

```diff
@@ -1,43 +1,46 @@
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-30 15:37:29.765561 Fletxible-0.5.9/
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-30 15:37:29.757663 Fletxible-0.5.9/Fletxible.egg-info/
--rw-r--r--   0 ahmad      (501) staff       (20)      824 2023-05-30 15:37:29.000000 Fletxible-0.5.9/Fletxible.egg-info/PKG-INFO
--rw-r--r--   0 ahmad      (501) staff       (20)      727 2023-05-30 15:37:29.000000 Fletxible-0.5.9/Fletxible.egg-info/SOURCES.txt
--rw-r--r--   0 ahmad      (501) staff       (20)        1 2023-05-30 15:37:29.000000 Fletxible-0.5.9/Fletxible.egg-info/dependency_links.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       58 2023-05-30 15:37:29.000000 Fletxible-0.5.9/Fletxible.egg-info/entry_points.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       37 2023-05-30 15:37:29.000000 Fletxible-0.5.9/Fletxible.egg-info/requires.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       36 2023-05-30 15:37:29.000000 Fletxible-0.5.9/Fletxible.egg-info/top_level.txt
--rw-r--r--   0 ahmad      (501) staff       (20)     1079 2023-04-29 15:25:05.000000 Fletxible-0.5.9/LICENSE
--rw-r--r--   0 ahmad      (501) staff       (20)      824 2023-05-30 15:37:29.765346 Fletxible-0.5.9/PKG-INFO
--rw-r--r--   0 ahmad      (501) staff       (20)     4768 2023-05-30 15:35:48.000000 Fletxible-0.5.9/README.md
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-30 15:37:29.758381 Fletxible-0.5.9/components/
--rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-05-26 14:46:31.000000 Fletxible-0.5.9/components/__init__.py
--rw-r--r--   0 ahmad      (501) staff       (20)     3313 2023-05-26 14:46:31.000000 Fletxible-0.5.9/components/block.py
--rw-r--r--   0 ahmad      (501) staff       (20)      274 2023-05-26 14:46:31.000000 Fletxible-0.5.9/components/typography.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-30 15:37:29.761611 Fletxible-0.5.9/core/
--rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-05-26 14:46:31.000000 Fletxible-0.5.9/core/__init__.py
--rw-r--r--   0 ahmad      (501) staff       (20)     1193 2023-05-30 13:09:25.000000 Fletxible-0.5.9/core/drawer.py
--rw-r--r--   0 ahmad      (501) staff       (20)     4190 2023-05-30 13:09:25.000000 Fletxible-0.5.9/core/header.py
--rw-r--r--   0 ahmad      (501) staff       (20)      318 2023-05-26 14:46:31.000000 Fletxible-0.5.9/core/left_panel.py
--rw-r--r--   0 ahmad      (501) staff       (20)     1185 2023-05-30 12:19:20.000000 Fletxible-0.5.9/core/middle_panel.py
--rw-r--r--   0 ahmad      (501) staff       (20)     4525 2023-05-28 17:50:12.000000 Fletxible-0.5.9/core/mobile_drop_down.py
--rw-r--r--   0 ahmad      (501) staff       (20)      419 2023-05-26 14:46:31.000000 Fletxible-0.5.9/core/mobile_navigation.py
--rw-r--r--   0 ahmad      (501) staff       (20)     2022 2023-05-30 13:09:25.000000 Fletxible-0.5.9/core/navigation.py
--rw-r--r--   0 ahmad      (501) staff       (20)     1109 2023-05-29 09:33:45.000000 Fletxible-0.5.9/core/repo.py
--rw-r--r--   0 ahmad      (501) staff       (20)     1252 2023-05-26 14:46:31.000000 Fletxible-0.5.9/core/right_panel.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-30 15:37:29.763158 Fletxible-0.5.9/fletxible/
--rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-05-30 15:37:12.000000 Fletxible-0.5.9/fletxible/__init__.py
--rw-r--r--   0 ahmad      (501) staff       (20)     4533 2023-05-30 15:36:50.000000 Fletxible-0.5.9/fletxible/base.py
--rw-r--r--   0 ahmad      (501) staff       (20)     2116 2023-05-30 15:36:50.000000 Fletxible-0.5.9/fletxible/command.py
--rw-r--r--   0 ahmad      (501) staff       (20)     2066 2023-05-30 15:36:50.000000 Fletxible-0.5.9/fletxible/fx_template.py
--rw-r--r--   0 ahmad      (501) staff       (20)     1089 2023-05-30 15:36:50.000000 Fletxible-0.5.9/fletxible/main.py
--rw-r--r--   0 ahmad      (501) staff       (20)     4216 2023-05-30 15:36:50.000000 Fletxible-0.5.9/fletxible/script.py
--rw-r--r--   0 ahmad      (501) staff       (20)       38 2023-05-30 15:37:29.765631 Fletxible-0.5.9/setup.cfg
--rw-r--r--   0 ahmad      (501) staff       (20)     1213 2023-05-30 15:37:03.000000 Fletxible-0.5.9/setup.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-30 15:37:29.763411 Fletxible-0.5.9/tests/
--rw-r--r--   0 ahmad      (501) staff       (20)        5 2023-05-01 14:25:50.000000 Fletxible-0.5.9/tests/test_route.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-30 15:37:29.765008 Fletxible-0.5.9/utilities/
--rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-05-26 17:08:22.000000 Fletxible-0.5.9/utilities/__init__.py
--rw-r--r--   0 ahmad      (501) staff       (20)      195 2023-05-26 16:04:02.000000 Fletxible-0.5.9/utilities/config.py
--rw-r--r--   0 ahmad      (501) staff       (20)      660 2023-05-29 12:14:30.000000 Fletxible-0.5.9/utilities/links.py
--rw-r--r--   0 ahmad      (501) staff       (20)      666 2023-05-30 09:09:24.000000 Fletxible-0.5.9/utilities/rail.py
--rw-r--r--   0 ahmad      (501) staff       (20)      366 2023-05-26 14:46:31.000000 Fletxible-0.5.9/utilities/router.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-08-05 22:17:19.614362 Fletxible-0.6.0/
+-rw-r--r--   0 ahmad      (501) staff       (20)     1079 2023-08-02 17:47:19.000000 Fletxible-0.6.0/LICENSE
+-rw-r--r--   0 ahmad      (501) staff       (20)      824 2023-08-05 22:17:19.614142 Fletxible-0.6.0/PKG-INFO
+-rw-r--r--   0 ahmad      (501) staff       (20)     4768 2023-08-02 17:47:19.000000 Fletxible-0.6.0/README.md
+-rw-r--r--   0 ahmad      (501) staff       (20)       38 2023-08-05 22:17:19.614431 Fletxible-0.6.0/setup.cfg
+-rw-r--r--   0 ahmad      (501) staff       (20)     1279 2023-08-05 22:16:12.000000 Fletxible-0.6.0/setup.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-08-05 22:17:19.603581 Fletxible-0.6.0/src/
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-08-05 22:17:19.605638 Fletxible-0.6.0/src/Fletxible.egg-info/
+-rw-r--r--   0 ahmad      (501) staff       (20)      824 2023-08-05 22:17:19.000000 Fletxible-0.6.0/src/Fletxible.egg-info/PKG-INFO
+-rw-r--r--   0 ahmad      (501) staff       (20)      929 2023-08-05 22:17:19.000000 Fletxible-0.6.0/src/Fletxible.egg-info/SOURCES.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)        1 2023-08-05 22:17:19.000000 Fletxible-0.6.0/src/Fletxible.egg-info/dependency_links.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       60 2023-08-05 22:17:19.000000 Fletxible-0.6.0/src/Fletxible.egg-info/entry_points.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       48 2023-08-05 22:17:19.000000 Fletxible-0.6.0/src/Fletxible.egg-info/requires.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       35 2023-08-05 22:17:19.000000 Fletxible-0.6.0/src/Fletxible.egg-info/top_level.txt
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-08-05 22:17:19.609192 Fletxible-0.6.0/src/core/
+-rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-08-02 17:47:19.000000 Fletxible-0.6.0/src/core/__init__.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     5332 2023-08-04 18:54:13.000000 Fletxible-0.6.0/src/core/base.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     2133 2023-08-03 12:18:42.000000 Fletxible-0.6.0/src/core/drawer.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     4647 2023-08-03 12:14:58.000000 Fletxible-0.6.0/src/core/header.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     1176 2023-08-05 09:36:32.000000 Fletxible-0.6.0/src/core/left_panel.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     1257 2023-08-02 17:47:19.000000 Fletxible-0.6.0/src/core/middle_panel.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     4678 2023-08-04 18:55:35.000000 Fletxible-0.6.0/src/core/mobile_drop_down.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      419 2023-08-02 17:47:19.000000 Fletxible-0.6.0/src/core/mobile_navigation.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      638 2023-08-04 18:58:27.000000 Fletxible-0.6.0/src/core/navigation.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     3073 2023-08-03 11:47:17.000000 Fletxible-0.6.0/src/core/repo_data.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     1801 2023-08-05 09:39:08.000000 Fletxible-0.6.0/src/core/right_panel.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-08-05 22:17:19.610303 Fletxible-0.6.0/src/fx_material/
+-rw-r--r--   0 ahmad      (501) staff       (20)      193 2023-08-02 17:47:19.000000 Fletxible-0.6.0/src/fx_material/__init__.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     1449 2023-08-02 17:47:19.000000 Fletxible-0.6.0/src/fx_material/annotation.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     3313 2023-08-02 17:47:19.000000 Fletxible-0.6.0/src/fx_material/block.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      274 2023-08-03 20:55:56.000000 Fletxible-0.6.0/src/fx_material/typography.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-08-05 22:17:19.611095 Fletxible-0.6.0/src/scripts/
+-rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-08-05 18:02:28.000000 Fletxible-0.6.0/src/scripts/__init__.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     4849 2023-08-05 17:57:44.000000 Fletxible-0.6.0/src/scripts/build.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     2203 2023-08-05 22:04:24.000000 Fletxible-0.6.0/src/scripts/create.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-08-05 22:17:19.613415 Fletxible-0.6.0/src/utilities/
+-rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-08-05 18:02:39.000000 Fletxible-0.6.0/src/utilities/__init__.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     2116 2023-05-30 15:27:55.000000 Fletxible-0.6.0/src/utilities/fx_cli.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      314 2023-08-02 17:47:19.000000 Fletxible-0.6.0/src/utilities/fx_config.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     1027 2023-08-05 17:55:14.000000 Fletxible-0.6.0/src/utilities/fx_error.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      567 2023-08-03 20:51:41.000000 Fletxible-0.6.0/src/utilities/fx_scratch.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      403 2023-08-05 17:51:41.000000 Fletxible-0.6.0/src/utilities/fx_sub_router.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     1042 2023-08-05 17:52:40.000000 Fletxible-0.6.0/src/utilities/fx_sub_template.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      903 2023-08-05 17:52:50.000000 Fletxible-0.6.0/src/utilities/fx_template.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-08-05 22:17:19.613704 Fletxible-0.6.0/tests/
+-rw-r--r--   0 ahmad      (501) staff       (20)        5 2023-08-02 17:52:36.000000 Fletxible-0.6.0/tests/test_template.py
```

### Comparing `Fletxible-0.5.9/Fletxible.egg-info/PKG-INFO` & `Fletxible-0.6.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Fletxible
-Version: 0.5.9
+Version: 0.6.0
 Summary: Web Boilerplate for Flet Library
 Home-page: https://github.com/LineIndent/fletxible
 Author: S. Ahmad P. Hakimi
 Author-email: pourhakimi@pm.me
 Keywords: python web template,web application,theme
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Fletxible-0.5.9/LICENSE` & `Fletxible-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Fletxible-0.5.9/PKG-INFO` & `Fletxible-0.6.0/src/Fletxible.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Fletxible
-Version: 0.5.9
+Version: 0.6.0
 Summary: Web Boilerplate for Flet Library
 Home-page: https://github.com/LineIndent/fletxible
 Author: S. Ahmad P. Hakimi
 Author-email: pourhakimi@pm.me
 Keywords: python web template,web application,theme
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Fletxible-0.5.9/README.md` & `Fletxible-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `Fletxible-0.5.9/components/block.py` & `Fletxible-0.6.0/src/fx_material/block.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
             self.copy_box.update()
 
             self.copy_box.disabled = False
             self.copy_box.update()
 
             break
 
-        if self._hovered == True:
+        if self._hovered is True:
             self.copy_box.content.opacity = 1
 
         else:
             self.copy_box.content.opacity = 0
 
         self.copy_box.content.update()
```

### Comparing `Fletxible-0.5.9/core/drawer.py` & `Fletxible-0.6.0/src/core/drawer.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,50 +1,72 @@
 import flet as ft
-import yaml
-
-with open("fx_config.yml", "r") as file:
-    docs = yaml.safe_load(file)
-
-
-background_color = docs["theme"][0]["bgcolor"]
+from core.repo_data import RepoData
 
 
 class Drawer(ft.Container):
     def __init__(
         self,
+        docs: dict,
+        page: ft.Page,
         expand=True,
         width=0,
         bgcolor="#23262d",
         shadow=None,
         animate=ft.Animation(550, "ease"),
         content=ft.Column(
             expand=True,
-            opacity=0,
-            animate_opacity=ft.Animation(200, "easeIn"),
+            # opacity=0,
+            spacing=0,
+            animate_opacity=ft.Animation(100, "ease"),
         ),
     ):
+        self.page = page
+        self.docs = docs
+        self.repo = RepoData(self.docs)
+
+        name = self.docs.get("repo-name", "")
+        url = self.docs.get("repo-url", "")
+        background_color = self.docs.get("theme", "").get("bgcolor", "")
+        primary = self.docs.get("theme", "").get("primary", "")
+
         super().__init__(
             expand=expand,
             width=width,
             bgcolor=bgcolor,
             shadow=shadow,
             animate=animate,
             content=content,
         )
 
         self.content.controls = [
             ft.Container(
                 bgcolor=background_color,
                 height=60,
+                padding=ft.padding.only(left=14),
                 content=ft.Row(
-                    alignment="center",
+                    alignment="start",
                     controls=[
                         ft.Text(
                             # start #
-'fletxible.',# end #
-                            size=21,
+                            name,  # end #
+                            size=19,
                             weight="w700",
+                            color="white",
                         )
                     ],
                 ),
-            )
+            ),
+            ft.Container(
+                padding=ft.padding.only(left=14),
+                bgcolor=primary,
+                height=45,
+                on_click=lambda __: self.page.launch_url(url=url),
+                content=ft.Tooltip(
+                    padding=10,
+                    vertical_offset=30,
+                    message="Go to repository",
+                    bgcolor="#20222c",
+                    text_style=ft.TextStyle(color="white", size=9),
+                    content=self.repo,
+                ),
+            ),
         ]
```

### Comparing `Fletxible-0.5.9/core/header.py` & `Fletxible-0.6.0/src/core/mobile_drop_down.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,141 +1,136 @@
 import flet as ft
-import yaml
-from bs4 import BeautifulSoup
-import httpx
-import asyncio
 
-with open("fx_config.yml", "r") as file:
-    docs = yaml.safe_load(file)
 
-name = docs["site-name"]
-repo = docs["repo-url"]
-background_color = docs["theme"][0]["bgcolor"]
-
-
-class Header(ft.Container):
+class MobileDropDownNavigation(ft.Container):
     def __init__(
         self,
-        full_nav: ft.Row,
-        mobile_nav: ft.IconButton,
-        bgcolor=background_color,
-        height=90,
-        padding=ft.padding.only(left=60, right=60),
+        title: str,
+        max_height: int,
+        drop_rail: list[list],
+        middle_panel: ft.Container,
+        visible=False,
+        height=45,
+        bgcolor=ft.colors.with_opacity(0.95, "#20222c"),
+        border=ft.border.all(0.85, "white24"),
+        border_radius=6,
+        clip_behavior=ft.ClipBehavior.HARD_EDGE,
+        animate=ft.Animation(300, "decelerate"),
+        alignment=ft.alignment.top_left,
         shadow=ft.BoxShadow(
             spread_radius=2,
             blur_radius=4,
             color=ft.colors.with_opacity(0.25, "black"),
-            offset=ft.Offset(2, 2),
+            offset=ft.Offset(4, 4),
         ),
-        animate=ft.Animation(500, "ease"),
-        clip_behavior=ft.ClipBehavior.HARD_EDGE,
     ):
-        self.name = name
-        self.full_nav = full_nav
-        self.mobile_nav = mobile_nav
-        self.navigation = ft.Row(
-            alignment="start",
-            opacity=1,
-            animate_opacity=ft.Animation(500, "ease"),
-            vertical_alignment="start",
-            controls=[
-                self.full_nav,
-            ],
-        )
-        self.repo_data = asyncio.run(self.get_repo_data())
+        self.title = title
+        self.middle_panel = middle_panel
+        self.drop_rail = drop_rail
+
+        self.max_height = max_height
+        if self.max_height != 0:
+            self.max_height = (max_height * 30) + 60
 
-        self.repo = ft.Row(
-            alignment="end",
-            controls=[
-                self.mobile_nav,
-                ft.Column(
-                    opacity=1,
-                    animate_opacity=ft.Animation(500, "ease"),
-                    alignment="center",
-                    horizontal_alignment="start",
-                    spacing=5,
-                    controls=[
-                        ft.Text("LineIndent/fletxible", size=11, weight="bold"),
-                        ft.Row(
-                            alignment="center",
-                            vertical_alignment="center",
-                            controls=self.repo_data,
-                        ),
-                    ],
-                ),
-            ],
-        )
+        self.drop_rail = self.generate_right_rail_logic(self.drop_rail)
 
         super().__init__(
-            bgcolor=bgcolor,
+            visible=visible,
             height=height,
-            padding=padding,
+            bgcolor=bgcolor,
+            border=border,
+            border_radius=border_radius,
             shadow=shadow,
-            animate=animate,
             clip_behavior=clip_behavior,
+            animate=animate,
+            alignment=alignment,
         )
 
         self.content = ft.Column(
-            alignment="center",
-            spacing=20,
+            expand=True,
+            alignment="start",
+            spacing=0,
             controls=[
-                #
-                ft.Row(
-                    alignment="spaceBetween",
-                    vertical_alignment="center",
-                    controls=[
-                        ft.Text(
-                            # start #
-'fletxible.',# end #
-                            size=21,
-                            weight="w700",
-                        ),
-                        self.repo,
-                    ],
+                ft.Container(
+                    bgcolor="#20222c",
+                    padding=ft.padding.only(left=20),
+                    content=ft.Row(
+                        height=42,
+                        alignment="spaceBetween",
+                        controls=[
+                            ft.Row(
+                                vertical_alignment="center",
+                                alignment="start",
+                                spacing=10,
+                                controls=[
+                                    ft.Text(
+                                        self.title.capitalize(),
+                                        size=11,
+                                        weight="w700",
+                                        color="white",
+                                    ),
+                                ],
+                            ),
+                            ft.IconButton(
+                                icon=ft.icons.ADD,
+                                icon_size=15,
+                                icon_color="white24",
+                                rotate=ft.Rotate(0, ft.alignment.center),
+                                animate_rotation=ft.Animation(400, "easeOutBack"),
+                                on_click=lambda e: self.resize_admonition(e),
+                            ),
+                        ],
+                    ),
+                ),
+                ft.Container(
+                    padding=ft.padding.only(left=20, right=20, bottom=10, top=15),
+                    expand=True,
+                    content=ft.Column(
+                        expand=True,
+                        alignment="spaceEven",
+                        horizontal_alignment="start",
+                        controls=self.drop_rail,
+                    ),
                 ),
-                #
-                self.navigation,
             ],
         )
 
-    # Method: gets the repo details based on the input repo URL ...
-    async def get_repo_data(self):
-        # await asyncio.sleep(5)
-        controls_list: list = []
-
-        icon_elements = ["LABEL_OUTLINED", "STAR_BORDER_SHARP", "CALL_SPLIT_SHARP"]
-
-        span_elements: list = [
-            "css-truncate css-truncate-target text-bold mr-2",
-            "Counter js-social-count",
-            "Counter",
-        ]
-
-        async with httpx.AsyncClient() as client:
-            response = await client.get(repo)
-            data = response.content
-
-        soup = BeautifulSoup(data, "html.parser")
-
-        for i, span in enumerate(span_elements):
-            span_element = soup.find("span", span)
-            if span_element is not None:
-                text_content = span_element.text.strip()
-                controls_list.append(
-                    ft.Row(
-                        alignment="center",
-                        spacing=0,
-                        controls=[
-                            ft.Icon(name=icon_elements[i], size=10),
-                            ft.Text(
-                                text_content,
-                                size=10,
-                                weight="w200",
-                            ),
-                        ],
+    def resize_admonition(self, e):
+        if self.height != self.max_height:
+            self.height = self.max_height
+            e.control.rotate = ft.Rotate(0.75, ft.alignment.center)
+        else:
+            self.height = 45
+            e.control.rotate = ft.Rotate(0, ft.alignment.center)
+
+        self.update()
+
+    def rail_hover_color(self, e):
+        if e.data == "true":
+            e.control.content.color = "white"
+
+        else:
+            e.control.content.color = ft.colors.with_opacity(0.55, "white10")
+
+        e.control.content.update()
+
+    def generate_right_rail_logic(self, fx_rail_list):
+        nav_rail = []
+        if len(fx_rail_list) != 0:
+            for item in fx_rail_list:
+                key = item[0]
+                nav_rail.append(
+                    ft.Container(
+                        content=ft.Text(
+                            item[1],
+                            size=12,
+                            color=ft.colors.with_opacity(0.55, "white10"),
+                        ),
+                        on_hover=lambda e,: self.rail_hover_color(e),
+                        on_click=lambda _, key=key: self.scroll_to_key(key),
                     )
                 )
 
-            else:
-                pass
+        return nav_rail
 
-        return controls_list
+    def scroll_to_key(self, key):
+        self.middle_panel.main_column.scroll_to(key=str(key), duration=500)
```

### Comparing `Fletxible-0.5.9/core/middle_panel.py` & `Fletxible-0.6.0/src/core/middle_panel.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,38 @@
 import flet as ft
-import yaml
-
-with open("fx_config.yml", "r") as file:
-    docs = yaml.safe_load(file)
-
-name = docs["site-name"]
 
 
 class MiddlePanel(ft.Container):
     def __init__(
         self,
-        controls: list,
+        components: list,
         function: list[callable],
         page: ft.Page,
+        header_name: str,
         expand=5,
         padding=ft.padding.only(top=65, right=15, left=15),
         alignment=ft.alignment.top_center,
-        content=ft.Column(
-            expand=True,
-            alignment="start",
-            scroll="hidden",
-            spacing=0,
-        ),
     ):
-        super().__init__(
-            expand=expand, padding=padding, alignment=alignment, content=content
-        )
         self.page = page
+        self.components = components
+        self.header_name = header_name
         self.function = function
-        self.controls = controls
-        self.content.on_scroll = lambda e: self.get_scroll(e)
-        self.content.controls = self.controls
+
+        self.main_column = ft.Column(
+            expand=True, alignment="start", scroll="hidden", spacing=0
+        )
+        self.main_column.controls = self.components
+        self.main_column.on_scroll = lambda e: self.get_scroll(e)
+        super().__init__(expand=expand, padding=padding, alignment=alignment)
+        self.content = self.main_column
 
     def get_scroll(self, e: ft.OnScrollEvent) -> None:
         if e.pixels >= float(2.0):
             self.function[0](60)
             self.function[1](0, False)
+            self.function[2](self.page.route.replace("/", "").capitalize())
 
         if e.pixels <= float(1.9):
+            self.function[2](self.header_name.name)
             if self.page.width >= 850:
                 self.function[1](1, True)
                 self.function[0](90)
```

### Comparing `Fletxible-0.5.9/fletxible/command.py` & `Fletxible-0.6.0/src/utilities/fx_cli.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.5.9/setup.py` & `Fletxible-0.6.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,31 @@
-from setuptools import setup
+from setuptools import find_packages, setup
 
 setup(
     name="Fletxible",
-    version="0.5.9",
+    version="0.6.0",
     author="S. Ahmad P. Hakimi",
     author_email="pourhakimi@pm.me",
     description="Web Boilerplate for Flet Library",
-    long_description="Fletxible is a Python web boilerplate project designed to provide a solid foundation for building web applications with Python and Flet. The project comes pre-configured with a range of tools and features to make it easy for developers to get started building their applications, without the need to spend time setting up infrastructure or configuring tools.",
+    long_description="Fletxible is a Python web boilerplate project designed to provide a solid foundation for building web applications with Python and Flet. The project comes pre-configured with a range of tools and features to make it easy for developers to get started building their applications, without the need to spend time setting up infrastructure or configuring tools.",  # noqa: E501
     long_description_content_type="text/markdown",
     url="https://github.com/LineIndent/fletxible",
-    packages=[
-        "core",
-        "components",
-        "utilities",
-        "fletxible",
+    packages=find_packages("src"),
+    package_dir={"": "src"},
+    include_package_data=True,
+    install_requires=[
+        "click>=8.1.3",
+        "flet>=0.9.0",
+        "beautifulsoup4>=4.12.2",
     ],
-    install_requires=["click>=8.1.3", "flet>=0.7.4", "PyYAML>=6.0"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     entry_points={
         "console_scripts": [
-            "fletxible-init=fletxible.command:init",
+            "fletxible-init=fletxible.command:create",
         ],
     },
     keywords=["python web template", "web application", "theme"],
 )
```

