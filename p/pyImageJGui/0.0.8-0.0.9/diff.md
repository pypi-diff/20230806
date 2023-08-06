# Comparing `tmp/pyimagejgui-0.0.8.tar.gz` & `tmp/pyimagejgui-0.0.9.tar.gz`

## Comparing `pyimagejgui-0.0.8.tar` & `pyimagejgui-0.0.9.tar`

### file list

```diff
@@ -1,35 +1,36 @@
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 pyimagejgui-0.0.8/init.bat
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 pyimagejgui-0.0.8/init.sh
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 pyimagejgui-0.0.8/main.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 pyimagejgui-0.0.8/requirements.txt
--rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 pyimagejgui-0.0.8/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 pyimagejgui-0.0.8/src/pyImageJGui/__init__.py
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 pyimagejgui-0.0.8/src/pyImageJGui/icon/angle.svg
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 pyimagejgui-0.0.8/src/pyImageJGui/icon/circle.svg
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 pyimagejgui-0.0.8/src/pyImageJGui/icon/clear.svg
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 pyimagejgui-0.0.8/src/pyImageJGui/icon/elliptical.svg
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 pyimagejgui-0.0.8/src/pyImageJGui/icon/file.svg
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 pyimagejgui-0.0.8/src/pyImageJGui/icon/freehand.svg
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 pyimagejgui-0.0.8/src/pyImageJGui/icon/hand.svg
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 pyimagejgui-0.0.8/src/pyImageJGui/icon/line.svg
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 pyimagejgui-0.0.8/src/pyImageJGui/icon/magnifier.svg
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 pyimagejgui-0.0.8/src/pyImageJGui/icon/polygon.svg
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 pyimagejgui-0.0.8/src/pyImageJGui/icon/rectangle.svg
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 pyimagejgui-0.0.8/src/pyImageJGui/icon/rotate.svg
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 pyimagejgui-0.0.8/src/pyImageJGui/icon/save.svg
--rwxr-xr-x   0        0        0     4254 2020-02-02 00:00:00.000000 pyimagejgui-0.0.8/src/pyImageJGui/style/main.qss
--rwxr-xr-x   0        0        0      478 2020-02-02 00:00:00.000000 pyimagejgui-0.0.8/src/pyImageJGui/style/qssloader.py
--rw-r--r--   0        0        0     7177 2020-02-02 00:00:00.000000 pyimagejgui-0.0.8/src/pyImageJGui/ui/AngleRoi.py
--rw-r--r--   0        0        0     6388 2020-02-02 00:00:00.000000 pyimagejgui-0.0.8/src/pyImageJGui/ui/CircleRoi.py
--rw-r--r--   0        0        0     7092 2020-02-02 00:00:00.000000 pyimagejgui-0.0.8/src/pyImageJGui/ui/EllipseRoi.py
--rw-r--r--   0        0        0     4365 2020-02-02 00:00:00.000000 pyimagejgui-0.0.8/src/pyImageJGui/ui/LineRoi.py
--rw-r--r--   0        0        0     6110 2020-02-02 00:00:00.000000 pyimagejgui-0.0.8/src/pyImageJGui/ui/RectangleRoi.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 pyimagejgui-0.0.8/src/pyImageJGui/ui/constant.py
--rw-r--r--   0        0        0    14769 2020-02-02 00:00:00.000000 pyimagejgui-0.0.8/src/pyImageJGui/ui/gui.py
--rw-r--r--   0        0        0    15058 2020-02-02 00:00:00.000000 pyimagejgui-0.0.8/src/pyImageJGui/ui/imageView.py
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 pyimagejgui-0.0.8/src/pyImageJGui/utils/function.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 pyimagejgui-0.0.8/.gitignore
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 pyimagejgui-0.0.8/LICENSE
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 pyimagejgui-0.0.8/README.md
--rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 pyimagejgui-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 pyimagejgui-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 pyimagejgui-0.0.9/init.bat
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 pyimagejgui-0.0.9/init.sh
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 pyimagejgui-0.0.9/main.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 pyimagejgui-0.0.9/requirements.txt
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 pyimagejgui-0.0.9/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 pyimagejgui-0.0.9/src/pyImageJGui/__init__.py
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 pyimagejgui-0.0.9/src/pyImageJGui/icon/angle.svg
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 pyimagejgui-0.0.9/src/pyImageJGui/icon/circle.svg
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 pyimagejgui-0.0.9/src/pyImageJGui/icon/clear.svg
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 pyimagejgui-0.0.9/src/pyImageJGui/icon/elliptical.svg
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 pyimagejgui-0.0.9/src/pyImageJGui/icon/file.svg
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 pyimagejgui-0.0.9/src/pyImageJGui/icon/freehand.svg
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 pyimagejgui-0.0.9/src/pyImageJGui/icon/hand.svg
+-rw-r--r--   0        0        0     4192 2020-02-02 00:00:00.000000 pyimagejgui-0.0.9/src/pyImageJGui/icon/icon.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 pyimagejgui-0.0.9/src/pyImageJGui/icon/line.svg
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 pyimagejgui-0.0.9/src/pyImageJGui/icon/magnifier.svg
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 pyimagejgui-0.0.9/src/pyImageJGui/icon/polygon.svg
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 pyimagejgui-0.0.9/src/pyImageJGui/icon/rectangle.svg
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 pyimagejgui-0.0.9/src/pyImageJGui/icon/rotate.svg
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 pyimagejgui-0.0.9/src/pyImageJGui/icon/save.svg
+-rwxr-xr-x   0        0        0     4254 2020-02-02 00:00:00.000000 pyimagejgui-0.0.9/src/pyImageJGui/style/main.qss
+-rwxr-xr-x   0        0        0      478 2020-02-02 00:00:00.000000 pyimagejgui-0.0.9/src/pyImageJGui/style/qssloader.py
+-rw-r--r--   0        0        0     7177 2020-02-02 00:00:00.000000 pyimagejgui-0.0.9/src/pyImageJGui/ui/AngleRoi.py
+-rw-r--r--   0        0        0     6388 2020-02-02 00:00:00.000000 pyimagejgui-0.0.9/src/pyImageJGui/ui/CircleRoi.py
+-rw-r--r--   0        0        0     7092 2020-02-02 00:00:00.000000 pyimagejgui-0.0.9/src/pyImageJGui/ui/EllipseRoi.py
+-rw-r--r--   0        0        0     4365 2020-02-02 00:00:00.000000 pyimagejgui-0.0.9/src/pyImageJGui/ui/LineRoi.py
+-rw-r--r--   0        0        0     6110 2020-02-02 00:00:00.000000 pyimagejgui-0.0.9/src/pyImageJGui/ui/RectangleRoi.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 pyimagejgui-0.0.9/src/pyImageJGui/ui/constant.py
+-rw-r--r--   0        0        0    14343 2020-02-02 00:00:00.000000 pyimagejgui-0.0.9/src/pyImageJGui/ui/gui.py
+-rw-r--r--   0        0        0    15058 2020-02-02 00:00:00.000000 pyimagejgui-0.0.9/src/pyImageJGui/ui/imageView.py
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 pyimagejgui-0.0.9/src/pyImageJGui/utils/function.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 pyimagejgui-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 pyimagejgui-0.0.9/LICENSE
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 pyimagejgui-0.0.9/README.md
+-rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 pyimagejgui-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 pyimagejgui-0.0.9/PKG-INFO
```

### Comparing `pyimagejgui-0.0.8/main.py` & `pyimagejgui-0.0.9/main.py`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.8/.github/workflows/python-publish.yml` & `pyimagejgui-0.0.9/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.8/src/pyImageJGui/icon/angle.svg` & `pyimagejgui-0.0.9/src/pyImageJGui/icon/angle.svg`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.8/src/pyImageJGui/icon/clear.svg` & `pyimagejgui-0.0.9/src/pyImageJGui/icon/clear.svg`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.8/src/pyImageJGui/icon/elliptical.svg` & `pyimagejgui-0.0.9/src/pyImageJGui/icon/elliptical.svg`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.8/src/pyImageJGui/icon/file.svg` & `pyimagejgui-0.0.9/src/pyImageJGui/icon/file.svg`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.8/src/pyImageJGui/icon/freehand.svg` & `pyimagejgui-0.0.9/src/pyImageJGui/icon/freehand.svg`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.8/src/pyImageJGui/icon/hand.svg` & `pyimagejgui-0.0.9/src/pyImageJGui/icon/hand.svg`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.8/src/pyImageJGui/icon/magnifier.svg` & `pyimagejgui-0.0.9/src/pyImageJGui/icon/magnifier.svg`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.8/src/pyImageJGui/icon/polygon.svg` & `pyimagejgui-0.0.9/src/pyImageJGui/icon/polygon.svg`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.8/src/pyImageJGui/icon/rectangle.svg` & `pyimagejgui-0.0.9/src/pyImageJGui/icon/rectangle.svg`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.8/src/pyImageJGui/icon/rotate.svg` & `pyimagejgui-0.0.9/src/pyImageJGui/icon/rotate.svg`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.8/src/pyImageJGui/icon/save.svg` & `pyimagejgui-0.0.9/src/pyImageJGui/icon/save.svg`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.8/src/pyImageJGui/style/main.qss` & `pyimagejgui-0.0.9/src/pyImageJGui/style/main.qss`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.8/src/pyImageJGui/ui/AngleRoi.py` & `pyimagejgui-0.0.9/src/pyImageJGui/ui/AngleRoi.py`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.8/src/pyImageJGui/ui/CircleRoi.py` & `pyimagejgui-0.0.9/src/pyImageJGui/ui/CircleRoi.py`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.8/src/pyImageJGui/ui/EllipseRoi.py` & `pyimagejgui-0.0.9/src/pyImageJGui/ui/EllipseRoi.py`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.8/src/pyImageJGui/ui/LineRoi.py` & `pyimagejgui-0.0.9/src/pyImageJGui/ui/LineRoi.py`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.8/src/pyImageJGui/ui/RectangleRoi.py` & `pyimagejgui-0.0.9/src/pyImageJGui/ui/RectangleRoi.py`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.8/src/pyImageJGui/ui/gui.py` & `pyimagejgui-0.0.9/src/pyImageJGui/ui/gui.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,49 +17,43 @@
 from .constant import ROI
 from ..utils.function import *
 from .RectangleRoi import RectangleRoi
 from .CircleRoi import CircleRoi
 from .LineRoi import LineRoi
 from .AngleRoi import AngleRoi
 from .EllipseRoi import EllipseRoi
+from ..icon.icon import *
 
 path = os.path.dirname(os.path.dirname(__file__))
 
 
 class ImageWidget(QWidget):
     def __init__(self, parent=None):
         QWidget.__init__(self, parent)
         self.layout = QVBoxLayout(self)
         self.button_layout = QHBoxLayout()
 
         self.last_open_dir = '/Users/sdb/image'
         self.roi = ROI.Hand
 
-        self.rectangle_button = Button(QIcon(os.path.join(path, 'icon', 'rectangle.svg')), '', ROI.Rectangle)
-        icon_size = self.rectangle_button.style().pixelMetric(QStyle.PixelMetric.PM_ButtonIconSize)
-        self.rectangle_button.setIconSize(QSize(icon_size, icon_size))
-        self.angle_button = Button(QIcon(os.path.join(path, 'icon', 'angle.svg')), '', ROI.Angle)
-        self.angle_button.setIconSize(QSize(icon_size, icon_size))
-        self.circle_button = Button(QIcon(os.path.join(path, 'icon', 'circle.svg')), '', ROI.Circle)
-        self.circle_button.setIconSize(QSize(icon_size, icon_size))
-        self.rotate_button = QPushButton(QIcon(os.path.join(path, 'icon', 'rotate.svg')), '')
-        self.rotate_button.setIconSize(QSize(icon_size, icon_size))
-        self.line_button = Button(QIcon(os.path.join(path, 'icon', 'line.svg')), '', ROI.Line)
-        self.line_button.setIconSize(QSize(icon_size, icon_size))
-        self.ellipse_button = Button(QIcon(os.path.join(path, 'icon', 'elliptical.svg')), '', ROI.Ellipse)
-        self.ellipse_button.setIconSize(QSize(icon_size, icon_size))
-        self.save_button = QPushButton(QIcon(os.path.join(path, 'icon', 'save.svg')), '')
-        self.save_button.setIconSize(QSize(icon_size, icon_size))
-        self.hand_button = Button(QIcon(os.path.join(path, 'icon', 'hand.svg')), '', ROI.Hand)
-        self.hand_button.setIconSize(QSize(icon_size, icon_size))
+        icon_size = 20
+        self.rectangle_button = Button(rectangle_icon(QSize(icon_size * 100, icon_size * 90)), '', ROI.Rectangle)
+        self.angle_button = Button(angle_icon(QSize(icon_size * 100, icon_size * 100)), '', ROI.Angle)
+        self.circle_button = Button(oval_icon(QSize(icon_size * 100, icon_size * 100)), '', ROI.Circle)
+        rotate_icon = QApplication.style().standardIcon(QStyle.SP_BrowserReload)
+        self.rotate_button = QPushButton(rotate_icon, '')
+        self.line_button = Button(line_icon(QSize(icon_size * 100, icon_size * 100)), '', ROI.Line)
+        self.ellipse_button = Button(oval_icon(QSize(icon_size * 100, icon_size * 90)), '', ROI.Ellipse)
+        save_icon = QApplication.style().standardIcon(QStyle.SP_DialogSaveButton)
+        self.save_button = QPushButton(save_icon, '')
+        self.hand_button = Button(QIcon(hand_icon(QSize(icon_size * 100, icon_size * 100))), '', ROI.Hand)
         self.hand_button.setEnabled(False)
-        self.clear_button = QPushButton(QIcon(os.path.join(path, 'icon', 'clear.svg')), '')
-        self.clear_button.setIconSize(QSize(icon_size, icon_size))
-        self.file_button = QPushButton(QIcon(os.path.join(path, 'icon', 'file.svg')), '')
-        self.file_button.setIconSize(QSize(icon_size, icon_size))
+        self.clear_button = QPushButton(clear_icon(QSize(icon_size * 100, icon_size * 100)), '')
+        file_icon = QApplication.style().standardIcon(QStyle.SP_DirIcon)
+        self.file_button = QPushButton(file_icon, '')
         self.button_layout.addWidget(self.rectangle_button)
         self.button_layout.addWidget(self.circle_button)
         self.button_layout.addWidget(self.ellipse_button)
         self.button_layout.addWidget(self.line_button)
         self.button_layout.addWidget(self.angle_button)
         self.button_layout.addWidget(self.rotate_button)
         self.button_layout.addWidget(self.hand_button)
@@ -277,14 +271,17 @@
 
             angle = round(math.degrees(angle), 3)
             roi_table.setItem(roi_table.rowCount() - 1, 0, QTableWidgetItem(str(angle)))
 
         dialog.show()
 
     def rotate_btn_click(self):
+        if self.figure.image is None:
+            show_message_box("请先加载图片!")
+            return
         transform = QTransform()
 
         dialog = QDialog(self)
         dialog.setWindowModality(Qt.WindowModality.ApplicationModal)
         dialog.setMinimumSize(QSize(300, 100))
         layout = QVBoxLayout(dialog)
         angle_label = QLabel("Rotation Angle")
@@ -314,18 +311,20 @@
         allOrRoi = QComboBox()
         allOrRoi.addItems(["ROI", "ALL"])
         save_path_btn = QPushButton("Select storage path")
         layout.addWidget(allOrRoi)
         layout.addWidget(save_path_btn)
 
         def save_path_btn_click():
+            file_filter = "BMP Files (*.bmp)"
             filePath, _ = QFileDialog.getSaveFileName(
-                self,  # 父窗口对象
-                "Select storage path",  # 标题
-                self.last_open_dir  # 起始目录
+                self,
+                "Select storage path",
+                self.last_open_dir,
+                file_filter
             )
             self.last_open_dir = os.path.dirname(filePath)
             if filePath:
                 if allOrRoi.currentText() == "ALL":
                     save_pixmap(filePath, self.figure.pixmap_item.pixmap())
                 else:
                     if isinstance(self.figure.roi, RectangleRoi):
```

### Comparing `pyimagejgui-0.0.8/src/pyImageJGui/ui/imageView.py` & `pyimagejgui-0.0.9/src/pyImageJGui/ui/imageView.py`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.8/src/pyImageJGui/utils/function.py` & `pyimagejgui-0.0.9/src/pyImageJGui/utils/function.py`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.8/LICENSE` & `pyimagejgui-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.8/pyproject.toml` & `pyimagejgui-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyImageJGui"
-version = "0.0.8"
+version = "0.0.9"
 description = "Python for ImageJ GUI"
 authors = [{name = "sdb", email = "sdb20200101@gmail.com"}]
 readme = "README.md"
 keywords = ["imagej", "GUI", "PySide6"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
```

### Comparing `pyimagejgui-0.0.8/PKG-INFO` & `pyimagejgui-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyImageJGui
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python for ImageJ GUI
 Project-URL: homepage, https://github.com/aghb123/pyImageJGui
 Author-email: sdb <sdb20200101@gmail.com>
 License-File: LICENSE
 Keywords: GUI,PySide6,imagej
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

