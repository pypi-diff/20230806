# Comparing `tmp/untanglepyut-0.7.0.tar.gz` & `tmp/untanglepyut-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "untanglepyut-0.7.0.tar", last modified: Fri Jun  9 22:03:56 2023, max compression
+gzip compressed data, was "untanglepyut-1.1.0.tar", last modified: Sun Aug  6 03:40:16 2023, max compression
```

## Comparing `untanglepyut-0.7.0.tar` & `untanglepyut-1.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-09 22:03:56.235884 untanglepyut-0.7.0/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2022-08-15 19:41:01.000000 untanglepyut-0.7.0/LICENSE
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3477 2023-06-09 22:03:56.235774 untanglepyut-0.7.0/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3226 2023-04-13 20:32:39.000000 untanglepyut-0.7.0/README.md
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-06-09 22:03:56.235914 untanglepyut-0.7.0/setup.cfg
--rw-------   0 humberto.a.sanchez.ii   (501) staff       (20)      821 2023-06-09 21:53:23.000000 untanglepyut-0.7.0/setup.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-09 22:03:56.235046 untanglepyut-0.7.0/untanglepyut/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      886 2023-01-03 16:20:29.000000 untanglepyut-0.7.0/untanglepyut/BaseUnTangle.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1774 2022-08-29 19:49:16.000000 untanglepyut-0.7.0/untanglepyut/Common.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1078 2022-10-13 01:16:21.000000 untanglepyut-0.7.0/untanglepyut/Types.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    15843 2023-03-19 16:02:08.000000 untanglepyut-0.7.0/untanglepyut/UnTangleOglLinks.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    14445 2023-05-08 16:55:26.000000 untanglepyut-0.7.0/untanglepyut/UnTanglePyut.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4154 2022-08-23 19:21:04.000000 untanglepyut-0.7.0/untanglepyut/UnTangleUseCaseDiagram.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    13009 2023-05-10 17:16:32.000000 untanglepyut-0.7.0/untanglepyut/UnTangler.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3918 2023-01-31 19:27:38.000000 untanglepyut-0.7.0/untanglepyut/UntangleSequenceDiagram.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       45 2023-05-15 00:32:46.000000 untanglepyut-0.7.0/untanglepyut/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       27 2023-06-09 20:48:03.000000 untanglepyut-0.7.0/untanglepyut/_version.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-25 14:46:48.000000 untanglepyut-0.7.0/untanglepyut/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-09 22:03:56.235612 untanglepyut-0.7.0/untanglepyut.egg-info/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3477 2023-06-09 22:03:56.000000 untanglepyut-0.7.0/untanglepyut.egg-info/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      518 2023-06-09 22:03:56.000000 untanglepyut-0.7.0/untanglepyut.egg-info/SOURCES.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2023-06-09 22:03:56.000000 untanglepyut-0.7.0/untanglepyut.egg-info/dependency_links.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       84 2023-06-09 22:03:56.000000 untanglepyut-0.7.0/untanglepyut.egg-info/requires.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       13 2023-06-09 22:03:56.000000 untanglepyut-0.7.0/untanglepyut.egg-info/top_level.txt
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-08-06 03:40:16.827620 untanglepyut-1.1.0/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2022-08-15 19:41:01.000000 untanglepyut-1.1.0/LICENSE
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3477 2023-08-06 03:40:16.827507 untanglepyut-1.1.0/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3226 2023-04-13 20:32:39.000000 untanglepyut-1.1.0/README.md
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-08-06 03:40:16.827651 untanglepyut-1.1.0/setup.cfg
+-rw-------   0 humberto.a.sanchez.ii   (501) staff       (20)      820 2023-08-06 03:18:34.000000 untanglepyut-1.1.0/setup.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-08-06 03:40:16.826750 untanglepyut-1.1.0/untanglepyut/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      886 2023-01-03 16:20:29.000000 untanglepyut-1.1.0/untanglepyut/BaseUnTangle.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1774 2022-08-29 19:49:16.000000 untanglepyut-1.1.0/untanglepyut/Common.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1078 2022-10-13 01:16:21.000000 untanglepyut-1.1.0/untanglepyut/Types.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    15590 2023-08-05 19:03:58.000000 untanglepyut-1.1.0/untanglepyut/UnTangleOglLinks.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    14445 2023-05-08 16:55:26.000000 untanglepyut-1.1.0/untanglepyut/UnTanglePyut.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4154 2022-08-23 19:21:04.000000 untanglepyut-1.1.0/untanglepyut/UnTangleUseCaseDiagram.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    13009 2023-05-10 17:16:32.000000 untanglepyut-1.1.0/untanglepyut/UnTangler.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3918 2023-01-31 19:27:38.000000 untanglepyut-1.1.0/untanglepyut/UntangleSequenceDiagram.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       45 2023-05-15 00:32:46.000000 untanglepyut-1.1.0/untanglepyut/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       27 2023-08-06 03:18:37.000000 untanglepyut-1.1.0/untanglepyut/_version.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-25 14:46:48.000000 untanglepyut-1.1.0/untanglepyut/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-08-06 03:40:16.827335 untanglepyut-1.1.0/untanglepyut.egg-info/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3477 2023-08-06 03:40:16.000000 untanglepyut-1.1.0/untanglepyut.egg-info/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      518 2023-08-06 03:40:16.000000 untanglepyut-1.1.0/untanglepyut.egg-info/SOURCES.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2023-08-06 03:40:16.000000 untanglepyut-1.1.0/untanglepyut.egg-info/dependency_links.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       83 2023-08-06 03:40:16.000000 untanglepyut-1.1.0/untanglepyut.egg-info/requires.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       13 2023-08-06 03:40:16.000000 untanglepyut-1.1.0/untanglepyut.egg-info/top_level.txt
```

### Comparing `untanglepyut-0.7.0/LICENSE` & `untanglepyut-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `untanglepyut-0.7.0/PKG-INFO` & `untanglepyut-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: untanglepyut
-Version: 0.7.0
+Version: 1.1.0
 Summary: XML to Ogl Object Model
 Home-page: https://github.com/hasii2011/untanglepyut
 Author-email: Humberto.A.Sanchez.II@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <img src="./docs/agpl-license-web-badge-version-2-256x48.png"/>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: untanglepyut Version: 0.7.0 Summary: XML to Ogl
+Metadata-Version: 2.1 Name: untanglepyut Version: 1.1.0 Summary: XML to Ogl
 Object Model Home-page: https://github.com/hasii2011/untanglepyut Author-email:
 Humberto.A.Sanchez.II@gmail.com Description-Content-Type: text/markdown
 License-File: LICENSE [./docs/agpl-license-web-badge-version-2-256x48.png] [!
 [CircleCI](https://dl.circleci.com/insights-snapshot/gh/hasii2011/untanglepyut/
 master/main/badge.svg?window=30d)](https://app.circleci.com/insights/github/
 hasii2011/untanglepyut/workflows/main/overview?branch=master&reporting-
 window=last-30-days&insights-snapshot=true) [![CircleCI](https://
```

### Comparing `untanglepyut-0.7.0/README.md` & `untanglepyut-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `untanglepyut-0.7.0/setup.py` & `untanglepyut-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,9 +20,9 @@
     packages=[
         'untanglepyut'
     ],
     package_data={
         'untanglepyut': ['py.typed'],
     },
 
-    install_requires=['hasiihelper==0.2.1', 'hasiicommon==0.3.1', 'pyutmodel~=1.4.4', 'ogl==0.70.52', 'untangle==1.2.1'],
+    install_requires=['hasiihelper==0.2.1', 'hasiicommon==0.3.1', 'pyutmodel~=1.4.4', 'ogl==0.85.0', 'untangle==1.2.1'],
 )
```

### Comparing `untanglepyut-0.7.0/untanglepyut/BaseUnTangle.py` & `untanglepyut-1.1.0/untanglepyut/BaseUnTangle.py`

 * *Files identical despite different names*

### Comparing `untanglepyut-0.7.0/untanglepyut/Common.py` & `untanglepyut-1.1.0/untanglepyut/Common.py`

 * *Files identical despite different names*

### Comparing `untanglepyut-0.7.0/untanglepyut/Types.py` & `untanglepyut-1.1.0/untanglepyut/Types.py`

 * *Files identical despite different names*

### Comparing `untanglepyut-0.7.0/untanglepyut/UnTangleOglLinks.py` & `untanglepyut-1.1.0/untanglepyut/UnTangleOglLinks.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 
-from logging import Logger
-from logging import getLogger
 from typing import Dict
 from typing import List
 from typing import NewType
 from typing import Union
 from typing import cast
 
+from logging import Logger
+from logging import getLogger
+
 from dataclasses import dataclass
 
-from miniogl.AttachmentSide import AttachmentSide
 from pyutmodel.PyutClass import PyutClass
-from untangle import Element
 
+from untangle import Element
 
+from miniogl.AttachmentSide import AttachmentSide
 from miniogl.ControlPoint import ControlPoint
 from miniogl.SelectAnchorPoint import SelectAnchorPoint
 
 from pyutmodel.PyutLinkType import PyutLinkType
 from pyutmodel.PyutInterface import PyutInterface
 from pyutmodel.PyutLink import PyutLink
 
@@ -182,15 +183,15 @@
             oglLink.AddControl(control=controlPoint, after=None)
             if selfLink:
                 x, y = controlPoint.GetPosition()
                 controlPoint.SetParent(parent)
                 controlPoint.SetPosition(x, y)
 
         if isinstance(oglLink, OglAssociation):
-            oglLink = self.__furtherCustomizeAssociationLink(graphicLink, oglLink)
+            self._addAssociationLabels(graphicLink, oglLink)
 
         self._reconstituteLinkDataModel(oglLink)
 
         return oglLink
 
     def _oglLinkFactory(self, srcShape, pyutLink, destShape, linkType: PyutLinkType, srcPos=None, dstPos=None):
         """
@@ -353,51 +354,41 @@
             childPyutClass:  PyutClass = cast(PyutClass, srcShape.pyutObject)
             parentPyutClass: PyutClass = cast(PyutClass, destShape.pyutObject)
             childPyutClass.addParent(parentPyutClass)
         else:
             srcPyutClass:  PyutClass = cast(PyutClass, srcShape.pyutObject)
             srcPyutClass.addLink(pyutLink)
 
-    def __furtherCustomizeAssociationLink(self, graphicLink: Element, oglLink: OglAssociation) -> OglAssociation:
+    def _addAssociationLabels(self, graphicLink: Element, oglAssociation: OglAssociation):
         """
-        Customize the visual aspects of an Association link
-
-        TODO:  There is no support for this yet.  Need to add it to OglAssociation
+        The association labels are now separate components;  We need to handle that
 
         Args:
-            graphicLink:  The top level GraphicLink Element
-            oglLink:      The current OGL representation of the graphicLink
+            graphicLink:    The top level GraphicLink Element
+            oglAssociation: The current OGL representation of the graphicLink
 
         Returns:  The updated association link
         """
-        center: OglAssociationLabel = oglLink.centerLabel
-        src:    OglAssociationLabel = oglLink.sourceCardinality
-        dest:   OglAssociationLabel = oglLink.destinationCardinality
-
-        oglLink.centerLabel            = self.__setAssociationLabelPosition(graphicLink, 'LabelCenter', center)
-        oglLink.sourceCardinality      = self.__setAssociationLabelPosition(graphicLink, 'LabelSrc',    src)
-        oglLink.destinationCardinality = self.__setAssociationLabelPosition(graphicLink, 'LabelDst',    dest)
 
-        return oglLink
+        pyutLink:         PyutLink            = oglAssociation.pyutObject
 
-    def __setAssociationLabelPosition(self, graphicLink: Element, tagName: str, associationLabel: OglAssociationLabel) -> OglAssociationLabel:
-        """
+        oglAssociation.centerLabel            = self._createALabel(oglAssociation, graphicLink, text=pyutLink.name, tagName='LabelCenter')
+        oglAssociation.sourceCardinality      = self._createALabel(oglAssociation, graphicLink, text=pyutLink.sourceCardinality, tagName='LabelSrc')
+        oglAssociation.destinationCardinality = self._createALabel(oglAssociation, graphicLink, text=pyutLink.destinationCardinality, tagName='LabelDst')
 
-        Args:
-            graphicLink:  The top level GraphicLink Element
-            tagName:      The XML Element name
-            associationLabel:  The Ogl association label to update
+    def _createALabel(self, parentAssociation: OglAssociation, graphicLink: Element, text: str, tagName: str) -> OglAssociationLabel:
 
-        Returns:  The updated association label
-        """
         labels:  List[Element]   = graphicLink.get_elements(tagName)
         assert len(labels) == 1, 'There can be only one'
+
         label: Element = labels[0]
-        x: int = int(label['x'])
-        y: int = int(label['y'])
+        x:     int     = int(label['x'])
+        y:     int     = int(label['y'])
 
-        self.logger.debug(f'tagName: {tagName} `{associationLabel.text=}`  pos: ({x},{y})')
+        self.logger.debug(f'{tagName=} `{text=}` pos: ({x},{y})')
 
-        associationLabel.oglPosition.x = x
-        associationLabel.oglPosition.y = y
+        updatedLabelText: str = text
+        if updatedLabelText is None:
+            updatedLabelText = ''
+        oglAssociationLabel: OglAssociationLabel = OglAssociationLabel(x=x, y=y, text=updatedLabelText, parent=parentAssociation)
 
-        return associationLabel
+        return oglAssociationLabel
```

### Comparing `untanglepyut-0.7.0/untanglepyut/UnTanglePyut.py` & `untanglepyut-1.1.0/untanglepyut/UnTanglePyut.py`

 * *Files identical despite different names*

### Comparing `untanglepyut-0.7.0/untanglepyut/UnTangleUseCaseDiagram.py` & `untanglepyut-1.1.0/untanglepyut/UnTangleUseCaseDiagram.py`

 * *Files identical despite different names*

### Comparing `untanglepyut-0.7.0/untanglepyut/UnTangler.py` & `untanglepyut-1.1.0/untanglepyut/UnTangler.py`

 * *Files identical despite different names*

### Comparing `untanglepyut-0.7.0/untanglepyut/UntangleSequenceDiagram.py` & `untanglepyut-1.1.0/untanglepyut/UntangleSequenceDiagram.py`

 * *Files identical despite different names*

### Comparing `untanglepyut-0.7.0/untanglepyut.egg-info/PKG-INFO` & `untanglepyut-1.1.0/untanglepyut.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: untanglepyut
-Version: 0.7.0
+Version: 1.1.0
 Summary: XML to Ogl Object Model
 Home-page: https://github.com/hasii2011/untanglepyut
 Author-email: Humberto.A.Sanchez.II@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <img src="./docs/agpl-license-web-badge-version-2-256x48.png"/>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: untanglepyut Version: 0.7.0 Summary: XML to Ogl
+Metadata-Version: 2.1 Name: untanglepyut Version: 1.1.0 Summary: XML to Ogl
 Object Model Home-page: https://github.com/hasii2011/untanglepyut Author-email:
 Humberto.A.Sanchez.II@gmail.com Description-Content-Type: text/markdown
 License-File: LICENSE [./docs/agpl-license-web-badge-version-2-256x48.png] [!
 [CircleCI](https://dl.circleci.com/insights-snapshot/gh/hasii2011/untanglepyut/
 master/main/badge.svg?window=30d)](https://app.circleci.com/insights/github/
 hasii2011/untanglepyut/workflows/main/overview?branch=master&reporting-
 window=last-30-days&insights-snapshot=true) [![CircleCI](https://
```

### Comparing `untanglepyut-0.7.0/untanglepyut.egg-info/SOURCES.txt` & `untanglepyut-1.1.0/untanglepyut.egg-info/SOURCES.txt`

 * *Files identical despite different names*

