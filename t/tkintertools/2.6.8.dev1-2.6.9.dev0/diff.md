# Comparing `tmp/tkintertools-2.6.8.dev1.tar.gz` & `tmp/tkintertools-2.6.9.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkintertools-2.6.8.dev1.tar", last modified: Fri Jul 28 11:43:33 2023, max compression
+gzip compressed data, was "tkintertools-2.6.9.dev0.tar", last modified: Sun Aug  6 09:09:21 2023, max compression
```

## Comparing `tkintertools-2.6.8.dev1.tar` & `tkintertools-2.6.9.dev0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 11:43:33.805291 tkintertools-2.6.8.dev1/
--rw-rw-rw-   0        0        0     9267 2023-06-20 19:03:57.000000 tkintertools-2.6.8.dev1/LICENSE.txt
--rw-rw-rw-   0        0        0     9451 2023-07-28 11:43:33.804288 tkintertools-2.6.8.dev1/PKG-INFO
--rw-rw-rw-   0        0        0     8817 2023-07-28 11:41:26.000000 tkintertools-2.6.8.dev1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-28 11:43:33.806291 tkintertools-2.6.8.dev1/setup.cfg
--rw-rw-rw-   0        0        0     1630 2023-07-28 11:43:01.000000 tkintertools-2.6.8.dev1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-28 11:43:33.763293 tkintertools-2.6.8.dev1/tkintertools/
--rw-rw-rw-   0        0        0     2250 2023-07-28 11:42:30.000000 tkintertools-2.6.8.dev1/tkintertools/__init__.py
--rw-rw-rw-   0        0        0    67848 2023-07-20 16:33:47.000000 tkintertools-2.6.8.dev1/tkintertools/__main__.py
--rw-rw-rw-   0        0        0     2580 2023-07-20 07:07:46.000000 tkintertools-2.6.8.dev1/tkintertools/constants.py
--rw-rw-rw-   0        0        0    24186 2023-07-06 15:11:02.000000 tkintertools-2.6.8.dev1/tkintertools/tools_3d.py
-drwxrwxrwx   0        0        0        0 2023-07-28 11:43:33.802288 tkintertools-2.6.8.dev1/tkintertools.egg-info/
--rw-rw-rw-   0        0        0     9451 2023-07-28 11:43:33.000000 tkintertools-2.6.8.dev1/tkintertools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2023-07-28 11:43:33.000000 tkintertools-2.6.8.dev1/tkintertools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 11:43:33.000000 tkintertools-2.6.8.dev1/tkintertools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-28 11:43:33.000000 tkintertools-2.6.8.dev1/tkintertools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-06 09:09:21.951249 tkintertools-2.6.9.dev0/
+-rw-rw-rw-   0        0        0     9267 2023-06-20 19:03:57.000000 tkintertools-2.6.9.dev0/LICENSE.txt
+-rw-rw-rw-   0        0        0     7658 2023-08-06 09:09:21.950250 tkintertools-2.6.9.dev0/PKG-INFO
+-rw-rw-rw-   0        0        0     7024 2023-08-06 09:04:42.000000 tkintertools-2.6.9.dev0/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-06 09:09:21.951249 tkintertools-2.6.9.dev0/setup.cfg
+-rw-rw-rw-   0        0        0     1630 2023-08-06 08:46:47.000000 tkintertools-2.6.9.dev0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-06 09:09:21.920421 tkintertools-2.6.9.dev0/tkintertools/
+-rw-rw-rw-   0        0        0     2285 2023-08-06 08:46:12.000000 tkintertools-2.6.9.dev0/tkintertools/__init__.py
+-rw-rw-rw-   0        0        0    72017 2023-08-06 09:08:04.000000 tkintertools-2.6.9.dev0/tkintertools/__main__.py
+-rw-rw-rw-   0        0        0     2937 2023-08-06 08:44:14.000000 tkintertools-2.6.9.dev0/tkintertools/constants.py
+-rw-rw-rw-   0        0        0    24186 2023-08-04 04:36:12.000000 tkintertools-2.6.9.dev0/tkintertools/tools_3d.py
+drwxrwxrwx   0        0        0        0 2023-08-06 09:09:21.947270 tkintertools-2.6.9.dev0/tkintertools.egg-info/
+-rw-rw-rw-   0        0        0     7658 2023-08-06 09:09:21.000000 tkintertools-2.6.9.dev0/tkintertools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2023-08-06 09:09:21.000000 tkintertools-2.6.9.dev0/tkintertools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-06 09:09:21.000000 tkintertools-2.6.9.dev0/tkintertools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-08-06 09:09:21.000000 tkintertools-2.6.9.dev0/tkintertools.egg-info/top_level.txt
```

### Comparing `tkintertools-2.6.8.dev1/LICENSE.txt` & `tkintertools-2.6.9.dev0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tkintertools-2.6.8.dev1/PKG-INFO` & `tkintertools-2.6.9.dev0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkintertools
-Version: 2.6.8.dev1
+Version: 2.6.9.dev0
 Summary: An auxiliary module of the tkinter module.
 Home-page: https://github.com/Xiaokang2022/tkintertools
 Author: Xiaokang2022
 Author-email: 2951256653@qq.com
 Maintainer: Xiaokang2022
 Maintainer-email: 2951256653@qq.com
 License: MulanPSL-2.0
@@ -23,16 +23,16 @@
 <img src="tkt.png" style="height: 128px" alt="Logo" />
 
 `tkintertools` 模块是 `tkinter` 模块的一个辅助模块\
 The `tkintertools` module is an auxiliary module of the `tkinter` module
 
 [![Version](https://img.shields.io/pypi/v/tkintertools?label=Version)](.)
 [![License](https://img.shields.io/pypi/l/tkintertools?label=License)](LICENSE.txt)
-[![ChangeLog](https://img.shields.io/badge/ChangeLog-2023/07/28-orange)](CHANGELOG.md)
-[![ToDo](https://img.shields.io/badge/ToDo-16-yellow)](TODO.md)
+[![ChangeLog](https://img.shields.io/badge/ChangeLog-2023/08/06-orange)](CHANGELOG.md)
+[![ToDo](https://img.shields.io/badge/ToDo-15-yellow)](TODO.md)
 [![Size](https://img.shields.io/github/languages/code-size/Xiaokang2022/tkintertools?label=Size)](tkintertools)
 [![Wiki](https://img.shields.io/badge/Wiki-14-purple)](https://github.com/Xiaokang2022/tkintertools/wiki)\
 [![Downloads](https://img.shields.io/pypi/dm/tkintertools?label=Downloads&logo=pypi)](https://pypistats.org/packages/tkintertools)
 [![Owner](https://img.shields.io/badge/Owner-Xiaokang2022-white)](https://github.com/Xiaokang2022)
 [![Blog](https://img.shields.io/badge/Blog-小康2022@CSDN-red)](https://xiaokang2022.blog.csdn.net)
 [![Email](https://img.shields.io/badge/Email-2951256653@qq.com-cyan)](mailto:2951256653@qq.com)
 
@@ -41,36 +41,36 @@
 </div>
 
 Install/模块安装👇
 -----------------
 
 ### Stable Version/稳定版本
 
-* Version/最新版本 : `2.6.7`
-* Release/发布日期 : 2023/07/06 (UTC+08)
+* Version/最新版本 : `2.6.8`
+* Release/发布日期 : 2023/08/03 (UTC+08)
 
 这个是目前的最新稳定版，相对于开发版本而言比较稳定，bug 大体上是没有那么多的，推荐使用这个。稳定版和开发版相比，它在发布之前有个测试的步骤，经过测试之后（各项功能正常运行，多平台兼容）才会发布。
 
 **PIP Cmd/安装命令：**
 
 ```
-pip install tkintertools==2.6.7
+pip install tkintertools==2.6.8
 ```
 
 ### Development Version/开发版本
 
-* Version/最新版本 : `2.6.8.dev1` (第 1 个预发布版本)
-* Release/发布日期 : 2023/07/28 (UTC+08)
+* Version/最新版本 : `2.6.9.dev0` (第 1 个预发布版本)
+* Release/发布日期 : 2023/08/06 (UTC+08)
 
 这个是我正在开发的版本，可能有新功能，bug 可能会比较多，但也可能会比原来的版本更加稳定。开发版没有经过多操作系统的测试，仅能保证在 Windows 系统下运行所有功能，在其他的操作系统上，可能有部分功能无法正常运行。大家可以在 Issues 中提出一些建议，我可能会适当采纳一些并在开发版本中更改或实现。
 
 **PIP Cmd/安装命令：**
 
 ```
-pip install tkintertools==2.6.8.dev1
+pip install tkintertools==2.6.9.dev0
 ```
 
 > **Warning**  
 > 开发版仅作示例，各函数或类的 API 并非最终确定结果，直接使用开发版可能导致后续无法与稳定版兼容！  
 > 若不指定具体的版本号，则会下载最新的稳定版本，也就是说，开发版本只能通过指定的版本号获取！
 
 ### Requirements/环境需求
@@ -91,101 +91,45 @@
 ![Python3.12.*](https://img.shields.io/badge/Python-3.12.*-blue?logo=python)
 
 News/最新功能👇
 --------------
 
 ### Release Notes/版本说明
 
-**最新版本: `tkintertools-v2.6.8.dev1`**
+**最新版本: `tkintertools-v2.6.9.dev0`**
 
 > **Note**   
 > tkintertools 的介绍、使用教程和开发文档均在 [Wiki](https://github.com/Xiaokang2022/tkintertools/wiki) 中，大家可前往查阅
 
-下面是本次开发版本（`v2.6.7` -> `v2.6.8.dev1`）的更新内容条目：
+下面是本次开发版本（`v2.6.8` -> `v2.6.9.dev0`）的更新内容条目：
 
-- [X] Added class `Animation` to achieve more efficient, convenient and functional animation effects  
-新增类 `Animation` 来实现更加高效、更加方便和功能性更强的动画效果
-- [X] Added constant `CONTROL`  
-新增常量 `CONTROL`
-- [X] Modified the name of the constant `FRAMES` to `FPS`  
-修改常量 `FRAMES` 的名称为 `FPS`
-- [X] The function `move` is about to be deprecated, please replace it with the new class `Animation`  
-函数 `move` 即将被弃用，请用新类 `Animation` 来代替
-- [X] The class `Singleton` is about to be deprecated and singleton mode classes will no longer be available in subsequent releases  
-类 `Singleton` 即将被弃用，后续版本中将不再提供单例模式类
-- [X] The class `Animation` adds the parameter `callback` to extend the functionality  
-类 `Animation` 新增参数 `callback` 来扩展功能
+- [X] Added widget Tip (`ToolTip`) and all virtual widgets added the parameter `tooltip`  
+新增控件提示框（`ToolTip`），且所有虚拟控件新增参数 `tooltip`
+- [X] Added constants `DURATION`、`TOOLTIP_FG`、`TOOLTIP_BG`、`TOOLTIP_HIGNLIGHT_THICKNESS` and `TOOLTIP_HIGNLIGHT_BACKGROUND`  
+新增常量 `DURATION`、`TOOLTIP_FG`、`TOOLTIP_BG`、`TOOLTIP_HIGNLIGHT_THICKNESS` 和 `TOOLTIP_HIGNLIGHT_BACKGROUND`
+- [X] Fixed an issue where the text class widget called method `clear` was invalid  
+修复了文本类控件调用方法 `clear` 无效的问题
+- [X] Optimized the method `wm_geometry` of class `Tk` to accommodate some specially formatted parameters  
+优化了类 `Tk` 的方法 `wm_geometry` 以适应某些特殊格式的参数
 
 ### Template Demo/模板演示
 
-下面是一个主要新功能的示例程序，运行下面的示例程序时，其拥有以下功能：
-
-* 按住鼠标左键拖动可以旋转这多个几何体；
-* 按住鼠标右键拖动可以移动这些几何体在空间中的位置；
-* 滚动鼠标中键可以放大和缩小画面；
-* 这多个几何体会自动地旋转以及上下浮动；
+下面是一个主要新功能的示例程序，当按照示例代码方式给虚拟控件传入一个名为 `tooltip` 的参数之后，便可以让这个控件拥有提示框
 
 下面是示例程序的效果图（运行环境为 Windows11-Python3.11.4）：
 
-![news](news.gif)
+![news](news.png)
 
 <details><summary><b>CODE/源代码</b></summary>
 
 ```python
-import math  # 数学支持
-
-import tkintertools as tkt  # 引入基础模块
-from tkintertools import tools_3d as t3d  # 引入 3d 子模块
-
-root = tkt.Tk('3D', 1280, 720)  # 创建窗口
-space = t3d.Space(root, 1280, 720, 0, 0)  # 创建空间
-
-for a in -100, 0, 100:
-    for b in -100, 0, 100:
-        for c in -100, 0, 100:
-            t3d.Cuboid(space, a-50, b-50, c-50, 100, 100, 100,  # 创建正方体
-                       color_up='white', color_down='yellow', color_left='red',
-                       color_right='orange', color_front='blue', color_back='green')
-
-
-def spin():
-    """ 自动旋转 """
-    for geo in space.geos():
-        geo.rotate(dz=0.01)
-
-
-def floating(value):
-    """ 上下浮动 """
-    for geo in space.geos():
-        geo.translate(dz=math.sin(value))
-
-
-def animation(value=0):
-    """ 形成动画 """
-    spin()
-    floating(value)
-    space.space_sort()  # 给它们的空间位置排序以正确显示
-    for geo in space.geos():
-        geo.update()
-    space.after(10, animation, value+math.pi/60)
-
-
-def scale(event):
-    """ 缩放事件 """
-    k = 1.05 if event.keysym == 'equal' else 0.95 if event.keysym == 'minus' else 1  # 缩放比率
-    for geo in space.geos():  # 遍历所有的几何体（不包括基本 3D 对象）
-        geo.scale(k, k, k)  # 缩放
-        geo.update()  # 更新改对象的实际画面
-    space.space_sort()  # 空间前后位置排序
-
+# 此处只展示核心代码
 
-animation()
-root.bind('<Key-equal>', scale)  # 绑定等号按键
-root.bind('<Key-minus>', scale)  # 绑定减号按键
-root.mainloop()  # 消息事件循环
+tip = tkt.ToolTip('模块介绍\nToolTip 测试')
+tkt.Button(canvas, 10, 660, 200, 50, text='Doc', tooltip=tip)
 ```
 
 </details>
 
 More/更多👇
 -----------
```

### Comparing `tkintertools-2.6.8.dev1/README.md` & `tkintertools-2.6.9.dev0/tkintertools.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,38 @@
+Metadata-Version: 2.1
+Name: tkintertools
+Version: 2.6.9.dev0
+Summary: An auxiliary module of the tkinter module.
+Home-page: https://github.com/Xiaokang2022/tkintertools
+Author: Xiaokang2022
+Author-email: 2951256653@qq.com
+Maintainer: Xiaokang2022
+Maintainer-email: 2951256653@qq.com
+License: MulanPSL-2.0
+Keywords: tkinter,tkintertools,GUI
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 <div align="center">
 
 # 🚀tkintertools🚀
 
 <img src="tkt.png" style="height: 128px" alt="Logo" />
 
 `tkintertools` 模块是 `tkinter` 模块的一个辅助模块\
 The `tkintertools` module is an auxiliary module of the `tkinter` module
 
 [![Version](https://img.shields.io/pypi/v/tkintertools?label=Version)](.)
 [![License](https://img.shields.io/pypi/l/tkintertools?label=License)](LICENSE.txt)
-[![ChangeLog](https://img.shields.io/badge/ChangeLog-2023/07/28-orange)](CHANGELOG.md)
-[![ToDo](https://img.shields.io/badge/ToDo-16-yellow)](TODO.md)
+[![ChangeLog](https://img.shields.io/badge/ChangeLog-2023/08/06-orange)](CHANGELOG.md)
+[![ToDo](https://img.shields.io/badge/ToDo-15-yellow)](TODO.md)
 [![Size](https://img.shields.io/github/languages/code-size/Xiaokang2022/tkintertools?label=Size)](tkintertools)
 [![Wiki](https://img.shields.io/badge/Wiki-14-purple)](https://github.com/Xiaokang2022/tkintertools/wiki)\
 [![Downloads](https://img.shields.io/pypi/dm/tkintertools?label=Downloads&logo=pypi)](https://pypistats.org/packages/tkintertools)
 [![Owner](https://img.shields.io/badge/Owner-Xiaokang2022-white)](https://github.com/Xiaokang2022)
 [![Blog](https://img.shields.io/badge/Blog-小康2022@CSDN-red)](https://xiaokang2022.blog.csdn.net)
 [![Email](https://img.shields.io/badge/Email-2951256653@qq.com-cyan)](mailto:2951256653@qq.com)
 
@@ -23,36 +41,36 @@
 </div>
 
 Install/模块安装👇
 -----------------
 
 ### Stable Version/稳定版本
 
-* Version/最新版本 : `2.6.7`
-* Release/发布日期 : 2023/07/06 (UTC+08)
+* Version/最新版本 : `2.6.8`
+* Release/发布日期 : 2023/08/03 (UTC+08)
 
 这个是目前的最新稳定版，相对于开发版本而言比较稳定，bug 大体上是没有那么多的，推荐使用这个。稳定版和开发版相比，它在发布之前有个测试的步骤，经过测试之后（各项功能正常运行，多平台兼容）才会发布。
 
 **PIP Cmd/安装命令：**
 
 ```
-pip install tkintertools==2.6.7
+pip install tkintertools==2.6.8
 ```
 
 ### Development Version/开发版本
 
-* Version/最新版本 : `2.6.8.dev1` (第 1 个预发布版本)
-* Release/发布日期 : 2023/07/28 (UTC+08)
+* Version/最新版本 : `2.6.9.dev0` (第 1 个预发布版本)
+* Release/发布日期 : 2023/08/06 (UTC+08)
 
 这个是我正在开发的版本，可能有新功能，bug 可能会比较多，但也可能会比原来的版本更加稳定。开发版没有经过多操作系统的测试，仅能保证在 Windows 系统下运行所有功能，在其他的操作系统上，可能有部分功能无法正常运行。大家可以在 Issues 中提出一些建议，我可能会适当采纳一些并在开发版本中更改或实现。
 
 **PIP Cmd/安装命令：**
 
 ```
-pip install tkintertools==2.6.8.dev1
+pip install tkintertools==2.6.9.dev0
 ```
 
 > **Warning**  
 > 开发版仅作示例，各函数或类的 API 并非最终确定结果，直接使用开发版可能导致后续无法与稳定版兼容！  
 > 若不指定具体的版本号，则会下载最新的稳定版本，也就是说，开发版本只能通过指定的版本号获取！
 
 ### Requirements/环境需求
@@ -73,101 +91,45 @@
 ![Python3.12.*](https://img.shields.io/badge/Python-3.12.*-blue?logo=python)
 
 News/最新功能👇
 --------------
 
 ### Release Notes/版本说明
 
-**最新版本: `tkintertools-v2.6.8.dev1`**
+**最新版本: `tkintertools-v2.6.9.dev0`**
 
 > **Note**   
 > tkintertools 的介绍、使用教程和开发文档均在 [Wiki](https://github.com/Xiaokang2022/tkintertools/wiki) 中，大家可前往查阅
 
-下面是本次开发版本（`v2.6.7` -> `v2.6.8.dev1`）的更新内容条目：
+下面是本次开发版本（`v2.6.8` -> `v2.6.9.dev0`）的更新内容条目：
 
-- [X] Added class `Animation` to achieve more efficient, convenient and functional animation effects  
-新增类 `Animation` 来实现更加高效、更加方便和功能性更强的动画效果
-- [X] Added constant `CONTROL`  
-新增常量 `CONTROL`
-- [X] Modified the name of the constant `FRAMES` to `FPS`  
-修改常量 `FRAMES` 的名称为 `FPS`
-- [X] The function `move` is about to be deprecated, please replace it with the new class `Animation`  
-函数 `move` 即将被弃用，请用新类 `Animation` 来代替
-- [X] The class `Singleton` is about to be deprecated and singleton mode classes will no longer be available in subsequent releases  
-类 `Singleton` 即将被弃用，后续版本中将不再提供单例模式类
-- [X] The class `Animation` adds the parameter `callback` to extend the functionality  
-类 `Animation` 新增参数 `callback` 来扩展功能
+- [X] Added widget Tip (`ToolTip`) and all virtual widgets added the parameter `tooltip`  
+新增控件提示框（`ToolTip`），且所有虚拟控件新增参数 `tooltip`
+- [X] Added constants `DURATION`、`TOOLTIP_FG`、`TOOLTIP_BG`、`TOOLTIP_HIGNLIGHT_THICKNESS` and `TOOLTIP_HIGNLIGHT_BACKGROUND`  
+新增常量 `DURATION`、`TOOLTIP_FG`、`TOOLTIP_BG`、`TOOLTIP_HIGNLIGHT_THICKNESS` 和 `TOOLTIP_HIGNLIGHT_BACKGROUND`
+- [X] Fixed an issue where the text class widget called method `clear` was invalid  
+修复了文本类控件调用方法 `clear` 无效的问题
+- [X] Optimized the method `wm_geometry` of class `Tk` to accommodate some specially formatted parameters  
+优化了类 `Tk` 的方法 `wm_geometry` 以适应某些特殊格式的参数
 
 ### Template Demo/模板演示
 
-下面是一个主要新功能的示例程序，运行下面的示例程序时，其拥有以下功能：
-
-* 按住鼠标左键拖动可以旋转这多个几何体；
-* 按住鼠标右键拖动可以移动这些几何体在空间中的位置；
-* 滚动鼠标中键可以放大和缩小画面；
-* 这多个几何体会自动地旋转以及上下浮动；
+下面是一个主要新功能的示例程序，当按照示例代码方式给虚拟控件传入一个名为 `tooltip` 的参数之后，便可以让这个控件拥有提示框
 
 下面是示例程序的效果图（运行环境为 Windows11-Python3.11.4）：
 
-![news](news.gif)
+![news](news.png)
 
 <details><summary><b>CODE/源代码</b></summary>
 
 ```python
-import math  # 数学支持
-
-import tkintertools as tkt  # 引入基础模块
-from tkintertools import tools_3d as t3d  # 引入 3d 子模块
-
-root = tkt.Tk('3D', 1280, 720)  # 创建窗口
-space = t3d.Space(root, 1280, 720, 0, 0)  # 创建空间
-
-for a in -100, 0, 100:
-    for b in -100, 0, 100:
-        for c in -100, 0, 100:
-            t3d.Cuboid(space, a-50, b-50, c-50, 100, 100, 100,  # 创建正方体
-                       color_up='white', color_down='yellow', color_left='red',
-                       color_right='orange', color_front='blue', color_back='green')
-
-
-def spin():
-    """ 自动旋转 """
-    for geo in space.geos():
-        geo.rotate(dz=0.01)
-
-
-def floating(value):
-    """ 上下浮动 """
-    for geo in space.geos():
-        geo.translate(dz=math.sin(value))
-
-
-def animation(value=0):
-    """ 形成动画 """
-    spin()
-    floating(value)
-    space.space_sort()  # 给它们的空间位置排序以正确显示
-    for geo in space.geos():
-        geo.update()
-    space.after(10, animation, value+math.pi/60)
-
-
-def scale(event):
-    """ 缩放事件 """
-    k = 1.05 if event.keysym == 'equal' else 0.95 if event.keysym == 'minus' else 1  # 缩放比率
-    for geo in space.geos():  # 遍历所有的几何体（不包括基本 3D 对象）
-        geo.scale(k, k, k)  # 缩放
-        geo.update()  # 更新改对象的实际画面
-    space.space_sort()  # 空间前后位置排序
-
+# 此处只展示核心代码
 
-animation()
-root.bind('<Key-equal>', scale)  # 绑定等号按键
-root.bind('<Key-minus>', scale)  # 绑定减号按键
-root.mainloop()  # 消息事件循环
+tip = tkt.ToolTip('模块介绍\nToolTip 测试')
+tkt.Button(canvas, 10, 660, 200, 50, text='Doc', tooltip=tip)
 ```
 
 </details>
 
 More/更多👇
 -----------
```

### Comparing `tkintertools-2.6.8.dev1/setup.py` & `tkintertools-2.6.9.dev0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 9. 删除多余文件
 """
 
 import setuptools
 
 setuptools.setup(
     name='tkintertools',
-    version='2.6.8.dev1',
+    version='2.6.9.dev0',
     description='An auxiliary module of the tkinter module.',
     long_description=open('README.md', encoding='utf-8').read(),
     author='Xiaokang2022',
     author_email='2951256653@qq.com',
     maintainer='Xiaokang2022',
     maintainer_email='2951256653@qq.com',
     url='https://github.com/Xiaokang2022/tkintertools',
```

### Comparing `tkintertools-2.6.8.dev1/tkintertools/__init__.py` & `tkintertools-2.6.9.dev0/tkintertools/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 * Convenient, inheritable singleton pattern class
 * 3D drawing
 
 Contents
 --------
 * Container Widgets: `Tk`, `Toplevel`, `Canvas`
 * Virtual Canvas Widgets: `Label`, `Button`, `CheckButton`, `Entry`, `Text`, `Progressbar`
-* Tool Classes: `PhotoImage`, `Singleton`
+* Tool Classes: `PhotoImage`, `ToolTip`, `Singleton`, `Animation`
 * Tool Functions: `move`, `text`, `color`, `askfont`, `SetProcessDpiAwareness`
 * Tool Submodules: `tool_3d`
 
 More
 ----
 [GitHub](https://github.com/Xiaokang2022/tkintertools) ·
 [License](https://github.com/Xiaokang2022/tkintertools/blob/master/LICENSE.txt) ·
@@ -44,18 +44,18 @@
 if sys.version_info < (3, 8):  # Version Check
     raise RuntimeError('Python version is too low (>=3.8)')
 
 from .__main__ import *
 from .constants import *
 
 __author__ = 'Xiaokang2022<2951256653@qq.com>'
-__version__ = '2.6.8.dev1'
+__version__ = '2.6.9.dev0'
 __all__ = [
     # Container Widgets
     'Tk', 'Toplevel', 'Canvas',
     # Virtual Canvas Widgets
     'Label', 'Button', 'CheckButton', 'Entry', 'Text', 'Progressbar',
     # Tool Classes
-    'PhotoImage', 'Singleton', 'Animation',
+    'PhotoImage', 'ToolTip', 'Singleton', 'Animation',
     # Tool Functions
     'move', 'text', 'color', 'askfont', 'SetProcessDpiAwareness',
 ] + all_constants
```

### Comparing `tkintertools-2.6.8.dev1/tkintertools/__main__.py` & `tkintertools-2.6.9.dev0/tkintertools/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,19 @@
 import math  # 数学支持
 import sys  # DPI 适配
 import tkinter  # 基础模块
 from fractions import Fraction  # 图片缩放
 from typing import (Any, Callable, Generator, Iterable, Literal,  # 类型提示
                     overload)
 
+try:  # 尝试引入 PIL
+    from PIL import Image, ImageTk
+except ImportError:
+    Image = None
+
 if sys.platform == 'win32':  # 仅在 Windows 平台下支持设置 DPI 级别
     from ctypes import WinDLL
 else:
     WinDLL = None
 
 from .constants import *
 
@@ -90,17 +95,27 @@
 
         self.width[1], self.height[1] = width, height  # 更新窗口当前的宽高值
 
     def wm_geometry(self, newGeometry=None):  # type: (str | None) -> str | None
         # override: 添加修改初始宽高值的功能并兼容不同的 DPI 缩放
         if newGeometry:
             width, height, _width, _height, * \
-                _ = map(int, (newGeometry+'+0+0').replace('+', 'x').split('x'))
+                _ = (newGeometry+'+0+0').replace('+', 'x').split('x')
+            if width != '':
+                width = int(width)
+                height = int(height)
+            if _width != '':
+                _width = int(_width)
+                _height = int(_height)
+
             self.width, self.height = [width]*2, [height]*2
-            geometry = '%dx%d+%d+%d' % (width, height, _width, _height)
+            if width != '':
+                geometry = '%sx%s+%s+%s' % (width, height, _width, _height)
+            else:
+                geometry = '+%s+%s' % (_width, _height)
             if not _:
                 geometry = geometry.split('+')[0]
             return tkinter.Tk.wm_geometry(self, geometry)
         geometry = tkinter.Tk.wm_geometry(self, newGeometry)
         width, height, _width, _height, * \
             _ = map(int, (geometry+'+0+0').replace('+', 'x').split('x'))
         return '%dx%d+%d+%d' % (width, height, _width, _height)
@@ -286,15 +301,15 @@
             font = self._font[item][:]
             font[1] = int(font[1])
             self.itemconfigure(item, font=font)
 
         for item in self._image:  # 图像大小缩放（采用相对的绝对缩放）
             if self._image[item][0] and self._image[item][0].extension != 'gif':
                 self._image[item][1] = self._image[item][0].zoom(
-                    temp_x*rate_x, temp_y*rate_y, 1.2)
+                    temp_x*rate_x, temp_y*rate_y, precision=1.2)
                 self.itemconfigure(item, image=self._image[item][1])
 
     def _touch(self, event, flag=True):  # type: (tkinter.Event, bool) -> None
         """ 鼠标触碰控件事件 """
         if self._lock:
             for widget in self._widget[::-1]:
                 if widget.live and widget._touch(event) and flag:
@@ -401,14 +416,15 @@
         height,  # type: float
         radius,  # type: float
         text,  # type: str
         justify,  # type: str
         borderwidth,  # type: float
         font,  # type: tuple[str, int, str]
         image,  # type: PhotoImage | None
+        tooltip,  # type: ToolTip | None
         color_text,  # type: tuple[str, str, str]
         color_fill,  # type: tuple[str, str, str]
         color_outline  # type: tuple[str, str, str]
     ):  # type: (...) -> None
         """
         ### 标准参数
         标准参数是所有控件都有的 \n 
@@ -420,14 +436,15 @@
         `height`: 控件的高度 \ 
         `radius`: 控件圆角化半径 \ 
         `text`: 控件显示的文本，对于文本控件而言，可以为一个元组：(默认文本, 鼠标触碰文本) \ 
         `justify`: 文本的对齐方式 \ 
         `borderwidth`: 外框的宽度 \ 
         `font`: 控件的字体设定 (字体, 大小, 样式) \ 
         `image`: 控件的背景（支持 png 类型，大小必须小于控件，否则会溢出控件边框） \ 
+        `tooltip`: 提示框 \ 
         `color_text`: 控件文本的颜色 \ 
         `color_fill`: 控件内部的颜色 \ 
         `color_outline`: 控件外框的颜色
         ---
         ### 特定参数
         特定参数只有某些控件类才有 \n 
         ---
@@ -448,14 +465,15 @@
             * 特别地，进度条控件的参数 `color_bar` 为: `(底色, 进度条颜色)`
         """
         self.master = canvas
         self.value = text
         self.justify = justify
         self.font = font
         self.photoimage = image
+        self.tooltip = tooltip
         self.color_text = list(color_text)
         self.color_fill = list(color_fill)
         self.color_outline = list(color_outline)
 
         x *= canvas.rx
         y *= canvas.ry
         width *= canvas.rx
@@ -575,14 +593,21 @@
         elif self._state == 'touch':
             mode = 1
         elif self._state == 'click':
             mode = 2
         else:
             mode = 3
 
+        if self.tooltip is not None:
+            if self._state == 'normal':
+                self.tooltip._cancel(self.master)
+                self.tooltip._destroy()
+            if self._state == 'touch':
+                self.tooltip._countdown(self.master)
+
         self.master.itemconfigure(self.text, fill=self.color_text[mode])
         if isinstance(self, (Text, CheckButton)):
             self.master.itemconfigure(self._text, fill=self.color_text[mode])
 
         if self.radius:
             for item in self.inside:  # 修改色块
                 self.master.itemconfigure(item, fill=self.color_fill[mode])
@@ -743,30 +768,32 @@
         text,  # type: tuple[str] | str
         limit,  # type: int
         justify,  # type: str
         icursor,  # type: str
         borderwidth,  # type: int
         font,  # type: tuple[str, int, str]
         image,  # type: PhotoImage | None
+        tooltip,  # type: ToolTip | None
         color_text,  # type: tuple[str, str, str]
         color_fill,  # type: tuple[str, str, str]
         color_outline  # type: tuple[str, str, str]
     ):  # type: (...) -> None
 
         self.canvas = canvas
         self.limit = limit
         self.icursor = icursor
 
         self.interval = 300  # 光标闪烁间
         self.flag = False  # 光标闪烁标志
         # 隐式值
         self._value = ['', text, ''] if type(text) == str else ['', *text]
 
-        BaseWidget.__init__(self, canvas, x, y, width, height, radius, '', justify,
-                            borderwidth, font, image, color_text, color_fill, color_outline)
+        BaseWidget.__init__(
+            self, canvas, x, y, width, height, radius, '', justify, borderwidth,
+            font, image, tooltip, color_text, color_fill, color_outline)
 
         # NOTE: 提示光标代码的位置顺序不可乱动，font 不可乱改
         self._cursor = canvas.create_text(0, 0, fill=color_text[2], font=font)
         canvas._font[self._cursor][1] = canvas._font[self.text][1]
         font = canvas.itemcget(self.text, 'font')
         canvas.itemconfigure(self._cursor, font=font)
 
@@ -834,15 +861,15 @@
     def _paste(self):  # type: () -> bool
         """ 快捷键粘贴 """
         condition = self._state == 'click' and not getattr(self, 'show', None)
         if condition:
             self.append(self.master.clipboard_get())
         return condition
 
-    def _clear(self):  # type: () -> None
+    def clear(self):  # type: () -> None
         """ 清空文本类控件的内容 """
         if isinstance(self, Text):
             event = tkinter.Event()
             event.keysym = 'BackSpace'
             self._click_on()
             for _ in range(len(self.value)):
                 self._input(event, True)
@@ -860,19 +887,19 @@
         self.value = self._value[0] = value
         self.master.itemconfigure(self.text, text=self._value[0])
 
     def append(self, value):  # type: (str) -> None
         """ 添加输入框的值 """
         event = tkinter.Event()
         event.keysym = None
-        self.click_on()
+        self._click_on()
         for s in value:
             event.char = s
-            self.input(event, True)
-        self.click_off()
+            self._input(event, True)
+        self._click_off()
 
 
 class Label(BaseWidget):
     """ 虚拟标签控件 """
 
     def __init__(
         self,
@@ -884,20 +911,22 @@
         *,
         radius=RADIUS,  # type: float
         text='',  # type: str
         borderwidth=BORDERWIDTH,  # type: int
         justify='center',  # type: Literal['left', 'center', 'right']
         font=(FONT, SIZE),  # type: tuple[str, int, str]
         image=None,  # type: PhotoImage | None
+        tooltip=None,  # type: ToolTip | None
         color_text=COLOR_TEXT,  # type: tuple[str, str, str]
         color_fill=COLOR_BUTTON_FILL,  # type: tuple[str, str, str]
         color_outline=COLOR_BUTTON_OUTLINE  # type: tuple[str, str, str]
     ):  # type: (...) -> None
-        BaseWidget.__init__(self, canvas, x, y, width, height, radius, text, justify,
-                            borderwidth, font, image, color_text, color_fill, color_outline)
+        BaseWidget.__init__(
+            self, canvas, x, y, width, height, radius, text, justify, borderwidth,
+            font, image, tooltip, color_text, color_fill, color_outline)
 
     def _touch(self, event):  # type: (tkinter.Event) -> bool
         """ 触碰状态检测 """
         condition = self.x1 <= event.x <= self.x2 and self.y1 <= event.y <= self.y2
         self.state('touch' if condition else 'normal')
         return condition
 
@@ -916,20 +945,22 @@
         radius=RADIUS,  # type: float
         text='',  # type: str
         borderwidth: int = BORDERWIDTH,  # type: int
         justify='center',  # type: Literal['left', 'center', 'right']
         font=(FONT, SIZE),  # type: tuple[str, int, str]
         command=None,  # type: Callable | None
         image=None,  # type: PhotoImage | None
+        tooltip=None,  # type: ToolTip | None
         color_text=COLOR_TEXT,  # type: tuple[str, str, str]
         color_fill=COLOR_BUTTON_FILL,  # type: tuple[str, str, str]
         color_outline=COLOR_BUTTON_OUTLINE,  # type: tuple[str, str, str]
     ):  # type: (...) -> None
-        BaseWidget.__init__(self, canvas, x, y, width, height, radius, text, justify,
-                            borderwidth, font, image, color_text, color_fill, color_outline)
+        BaseWidget.__init__(
+            self, canvas, x, y, width, height, radius, text, justify, borderwidth,
+            font, image, tooltip, color_text, color_fill, color_outline)
         self.command = command
 
     def _execute(self, event):  # type: (tkinter.Event) -> None
         """ 执行关联函数 """
         condition = self.x1 <= event.x <= self.x2 and self.y1 <= event.y <= self.y2
         if condition and self.command:
             self.command()
@@ -960,20 +991,22 @@
         *,
         radius=RADIUS,  # type: float
         text='',  # type: str
         value=False,  # type: bool
         borderwidth=BORDERWIDTH,  # type: int
         justify='right',  # type: Literal['right', 'left']
         image=None,  # type: PhotoImage | None
+        tooltip=None,  # type: ToolTip | None
         color_text=COLOR_TEXT,  # type: tuple[str, str, str]
         color_fill=COLOR_BUTTON_FILL,  # type: tuple[str, str, str]
         color_outline=COLOR_BUTTON_OUTLINE  # type: tuple[str, str, str]
     ):  # type: (...) -> None
-        Button.__init__(self, canvas, x, y, length, length, radius=radius, borderwidth=borderwidth, image=image,
-                        color_text=color_text, color_fill=color_fill, color_outline=color_outline)
+        Button.__init__(
+            self, canvas, x, y, length, length, radius=radius, borderwidth=borderwidth, image=image,
+            tooltip=tooltip, color_text=color_text, color_fill=color_fill, color_outline=color_outline)
         if justify == 'right':
             self._text = canvas.create_text(
                 x+1.25*length, y+length/2, text=text, anchor='w')
         else:
             self._text = canvas.create_text(
                 x-0.25*length, y+length/2, text=text, anchor='e')
         self.command = lambda: self.set(not bool(self.value))
@@ -1006,20 +1039,22 @@
         show=None,  # type: str | None
         limit=LIMIT,  # type: int
         cursor=CURSOR,  # type: str
         borderwidth=BORDERWIDTH,  # type: int
         justify='left',  # type: Literal['left', 'center', 'right']
         font=(FONT, SIZE),  # type: tuple[str, int, str]
         image=None,  # type: PhotoImage | None
+        tooltip=None,  # type: ToolTip | None
         color_text=COLOR_TEXT,  # type: tuple[str, str, str]
         color_fill=COLOR_TEXT_FILL,  # type: tuple[str, str, str]
         color_outline=COLOR_TEXT_OUTLINE  # type: tuple[str, str, str]
     ):  # type: (...) -> None
-        TextWidget.__init__(self, canvas, x, y, width, height, radius, text, limit, justify,
-                            cursor, borderwidth, font, image, color_text, color_fill, color_outline)
+        TextWidget.__init__(
+            self, canvas, x, y, width, height, radius, text, limit, justify, cursor,
+            borderwidth, font, image, tooltip, color_text, color_fill, color_outline)
         self.master.itemconfigure(self.text, text=self._value[1])
         self.show = show
 
     def _click_on(self):  # type: () -> None
         """ 控件获得焦点 """
         self.state('click')
         self.master.itemconfigure(self.text, text=self._value[0])
@@ -1086,20 +1121,22 @@
         limit=LIMIT,  # type: int
         read=False,  # type: bool
         cursor=CURSOR,  # type: str
         borderwidth=BORDERWIDTH,  # type: int
         justify='left',  # type: Literal['left', 'center', 'right']
         font=(FONT, SIZE),  # type: tuple[str, int, str]
         image=None,  # type: PhotoImage | None
+        tooltip=None,  # type: ToolTip | None
         color_text=COLOR_TEXT,  # type: tuple[str, str, str]
         color_fill=COLOR_TEXT_FILL,  # type: tuple[str, str, str]
         color_outline=COLOR_TEXT_OUTLINE  # type: tuple[str, str, str]
     ):  # type: (...) -> None
-        TextWidget.__init__(self, canvas, x, y, width, height, radius, text, limit, justify,
-                            cursor, borderwidth, font, image, color_text, color_fill, color_outline)
+        TextWidget.__init__(
+            self, canvas, x, y, width, height, radius, text, limit, justify, cursor,
+            borderwidth, font, image, tooltip, color_text, color_fill, color_outline)
 
         _x = x + (width-radius-3 if justify == 'right' else width /
                   2 if justify == 'center' else radius+2)
         _anchor = 'n' if justify == 'center' else 'ne' if justify == 'right' else 'nw'
 
         self._text = canvas.create_text(  # NOTE: 位置确定文本，位置不要乱动
             _x, y+radius+2,
@@ -1237,25 +1274,27 @@
         width,  # type: int
         height,  # type: int
         *,
         borderwidth=BORDERWIDTH,  # type: int
         justify='center',  # type: Literal['left', 'center', 'right']
         font=(FONT, SIZE),  # type: tuple[str, int, str]
         image=None,  # type: PhotoImage | None
+        tooltip=None,  # type: ToolTip | None
         color_text=COLOR_TEXT,  # type: tuple[str, str, str]
         color_outline=COLOR_TEXT_OUTLINE,  # type: tuple[str, str, str]
         color_bar=COLOR_BAR  # type: tuple[str, str]
     ):  # type: (...) -> None
         self.bottom = canvas.create_rectangle(
             x, y, x+width, y+height, width=borderwidth, fill=color_bar[0])
         self.bar = canvas.create_rectangle(
             x, y, x, y+height, width=borderwidth, outline='', fill=color_bar[1])
 
-        BaseWidget.__init__(self, canvas, x, y, width, height, 0, '0.00%', justify,
-                            borderwidth, font, image, color_text, COLOR_NONE, color_outline)
+        BaseWidget.__init__(
+            self, canvas, x, y, width, height, 0, '0.00%', justify, borderwidth,
+            font, image, tooltip, color_text, COLOR_NONE, color_outline)
 
         self.color_fill = list(color_bar)
 
     def _touch(self, event):  # type: (tkinter.Event) -> bool
         """ 触碰状态检测 """
         condition = self.x1 <= event.x <= self.x2 and self.y1 <= event.y <= self.y2
         self.state('touch' if condition else 'normal')
@@ -1268,14 +1307,81 @@
         """
         percentage = 0 if percentage < 0 else 1 if percentage > 1 else percentage
         x2 = self.x1 + self.width * percentage * self.master.rx
         self.master.coords(self.bar, self.x1, self.y1, x2, self.y2)
         self.configure(text='%.2f%%' % (percentage * 100))
 
 
+class ToolTip:
+    """ 提示框 """
+
+    def __init__(
+        self,
+        text,  # type: str
+        *,
+        font=(FONT,),
+        # type: tuple[str, int, str] | tuple[str, int] | str
+        fg=TOOLTIP_FG,  # type: str
+        bg=TOOLTIP_BG,  # type: str
+        justify='left',  # type: Literal['left', 'center', 'right']
+        highlightthickness=TOOLTIP_HIGNLIGHT_THICKNESS,  # type: int
+        highlightbackground=TOOLTIP_HIGNLIGHT_BACKGROUND,  # type: str
+        duration=DURATION,  # type: int
+    ):
+        """
+        `text`: 要显示的文本 \ 
+        `font`: 文本字体 \ 
+        `fg`: 前景色，默认为黑色 \ 
+        `bg`: 背景色，默认为淡黄色 \ 
+        `justify`: 文本对齐方式 \ 
+        `highlightthickness`: 边框厚度，默认为 1 像素 \ 
+        `highlightbackground`: 边框颜色，默认为黑色 \ 
+        `duration`: 持续时间，默认为 4000 毫秒
+        """
+        self.text = text
+        self.font = font
+        self.fg = fg
+        self.bg = bg
+        self.justify = justify
+        self.highlightthickness = highlightthickness
+        self.highlightbackground = highlightbackground
+        self.duration = duration
+
+        self.toplevel = None  # type: Toplevel | None
+        self.cd = None  # type: str | None
+
+    def _countdown(self, master):  # type: (tkinter.Widget) -> None
+        """ 倒计时 """
+        if self.cd is None:
+            self.cd = master.after(1000, self._place)
+
+    def _cancel(self, master):  # type: (tkinter.Widget) -> None
+        """ 取消倒计时 """
+        if self.cd is not None:
+            master.after_cancel(self.cd)
+            self.cd = None
+
+    def _place(self):  # type: () -> None
+        """ 显示 """
+        self.toplevel = tkinter.Toplevel(
+            highlightthickness=self.highlightthickness, highlightbackground=self.highlightbackground)
+        self.toplevel.overrideredirect(True)
+        x, y = self.toplevel.winfo_pointerxy()
+        self.toplevel.geometry('+%d+%d' % (x, y+26))
+        tkinter.Label(self.toplevel, text=self.text, font=self.font,
+                      fg=self.fg, bg=self.bg, justify=self.justify).pack()
+        self.toplevel.after(self.duration, self._destroy)
+
+    def _destroy(self):
+        """ 消失 """
+        if self.toplevel is not None:
+            self.toplevel.destroy()
+            self.toplevel = None
+
+
 class PhotoImage(tkinter.PhotoImage):
     """ 图片类 """
 
     def __init__(
         self,
         file,  # type: str | bytes
         **kw
@@ -1350,24 +1456,30 @@
         if clear:  # 清除背景
             self._item[item].itemconfigure(item, image=None)
 
     def zoom(
         self,
         rate_x,  # type: float
         rate_y,  # type: float
+        *,
         precision=None  # type: float | None
     ):  # type: (...) -> tkinter.PhotoImage
         """
         ### 缩放图片
         不会缩放该图片对象本身，只是返回一个缩放后的图片对象 \n 
         ---
         `rate_x`: 横向缩放倍率 \ 
         `rate_y`: 纵向缩放倍率 \ 
-        `precision`: 精度到小数点后的位数（推荐 1.2），越大运算就越慢（默认值代表绝对精确）
+        `precision`: 精度到小数点后的位数（推荐 1.2），越大运算就越慢（默认值代表绝对精确）\ 
+        注意：若有 PIL 库，请忽略参数 precision
         """
+        if Image is not None:
+            new_size = map(int, [self.width()*rate_x, self.height()*rate_y])
+            image = Image.open(self.file).resize(new_size)
+            return ImageTk.PhotoImage(image)
         if precision is not None:
             limit = round(10**precision)
             rate_x = Fraction(str(rate_x)).limit_denominator(limit)
             rate_y = Fraction(str(rate_y)).limit_denominator(limit)
             image = tkinter.PhotoImage.zoom(
                 self, rate_x.numerator, rate_y.numerator)
             image = image.subsample(rate_x.denominator, rate_y.denominator)
@@ -1394,35 +1506,38 @@
         translation=None,  # type: Iterable[float, float] | None
         color=None,  # type: tuple[Callable[[str], None], str, str] | None
         fps=FPS,  # type: int
         start=None,  # type: Callable | None
         step=None,  # type: Callable | None
         stop=None,  # type: Callable | None
         callback=None,  # type: Callable[[float]] | None
-        canvas=None  # type: tkinter.Canvas | None
+        canvas=None,  # type: tkinter.Canvas | None
+        loop=False,  # type: bool
     ):  # type: (...) -> None
         """
         `widget`: 进行动画的控件 \ 
         `ms`: 动画总时长（单位：毫秒） \ 
         `control`: 控制函数，为元组 (函数, 起始值, 终止值) 的形式 \ 
         `translation`: 平移运动 \ 
         `color`: 颜色变换 \ 
         `fps`: 每秒帧数 \ 
         `start`: 动画开始前执行的函数 \ 
         `step`: 动画每一帧结束后执行的函数（包括开始和结束）\ 
         `stop`: 动画结束后执行的函数 \ 
         `callback`: 回调函数，每一帧调用一次，传入参数为单帧占比 \ 
-        `canvas`: 当 widget 是画布中的绘制对象时，应指定 canvas
+        `canvas`: 当 widget 是画布中的绘制对象时，应指定 canvas \ 
+        `loop`: 是否循环播放动画，默认不循环，循环时参数 stop 失效
         """
         self.widget = widget
         self.master = canvas if isinstance(widget, int) else widget.master if isinstance(
             widget, tkinter.Widget) else widget
         self.start = start
         self.step = step
         self.stop = stop
+        self.loop = loop
         self.translation = translation
         self.color = color
         self.sec = 1000 // fps  # 单帧间隔时间
         self.count = ms * fps // 1000  # 总帧数
         if self.count == 0:
             self.count = 1  # 至少一帧
         self.callback = callback
@@ -1435,14 +1550,16 @@
         parts = [control(key * value) for value in range(1, self.count + 1)]
         total = sum(parts)
         return [elem / total for elem in parts]
 
     def _run(self, _ind=0):  # type: (int) -> None
         """ 执行动画 """
         if _ind == self.count:
+            if self.loop:
+                return self._run()  # 循环播放动画
             return None if self.stop is None else self.stop()
         self.master.after(self.sec, self._run, _ind + 1)
 
         if self.translation is not None:
             self._translate(*[value * self.parts[_ind]
                             for value in self.translation])
         if self.color is not None:
```

### Comparing `tkintertools-2.6.8.dev1/tkintertools/constants.py` & `tkintertools-2.6.9.dev0/tkintertools/constants.py`

 * *Files 13% similar despite different names*

```diff
@@ -64,14 +64,29 @@
 
 TICK = '✓'
 """ Default checkbox symbol """
 
 CONTROL = lambda _: 1, 0, 1
 """ Default control function """
 
+DURATION = 4000
+""" Default ToolTip duration """
+
+TOOLTIP_FG = 'black'
+""" Default ToolTip foreground color """
+
+TOOLTIP_BG = 'lightyellow'
+""" Default ToolTip background color """
+
+TOOLTIP_HIGNLIGHT_THICKNESS = 1
+""" Default ToolTip highlightthickness """
+
+TOOLTIP_HIGNLIGHT_BACKGROUND = 'black'
+""" Default ToolTip highlightbackground """
+
 
 ### 3D constants ###
 
 
 COLOR_POINT_FILL = '#000000'
 """ Default point fill color """
```

### Comparing `tkintertools-2.6.8.dev1/tkintertools/tools_3d.py` & `tkintertools-2.6.9.dev0/tkintertools/tools_3d.py`

 * *Files identical despite different names*

