# Comparing `tmp/oglio-0.7.7.tar.gz` & `tmp/oglio-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oglio-0.7.7.tar", last modified: Fri Jun  9 22:30:08 2023, max compression
+gzip compressed data, was "oglio-1.0.0.tar", last modified: Sun Aug  6 04:01:07 2023, max compression
```

## Comparing `oglio-0.7.7.tar` & `oglio-1.0.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-09 22:30:08.461722 oglio-0.7.7/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2022-07-20 17:57:30.000000 oglio-0.7.7/LICENSE
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2335 2023-06-09 22:30:08.461610 oglio-0.7.7/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2011 2023-04-13 20:29:58.000000 oglio-0.7.7/README.md
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-09 22:30:08.458952 oglio-0.7.7/oglio/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1016 2023-05-08 19:24:39.000000 oglio-0.7.7/oglio/IDFactory.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       82 2023-02-13 18:01:45.000000 oglio-0.7.7/oglio/OglVersion.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4580 2023-05-06 14:32:39.000000 oglio-0.7.7/oglio/Reader.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3826 2023-05-06 14:32:39.000000 oglio-0.7.7/oglio/Types.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      123 2022-10-13 12:50:37.000000 oglio-0.7.7/oglio/UnsupportedFileTypeException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2111 2023-05-06 14:32:39.000000 oglio-0.7.7/oglio/Writer.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-05-15 01:03:15.000000 oglio-0.7.7/oglio/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       27 2023-06-09 22:19:37.000000 oglio-0.7.7/oglio/_version.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-08-07 19:55:58.000000 oglio-0.7.7/oglio/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-09 22:30:08.461470 oglio-0.7.7/oglio/toXmlV10/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1913 2023-05-06 19:50:19.000000 oglio-0.7.7/oglio/toXmlV10/BaseOglToDom.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      569 2022-08-26 20:55:45.000000 oglio-0.7.7/oglio/toXmlV10/BasePyutToDom.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      132 2023-05-08 00:21:01.000000 oglio-0.7.7/oglio/toXmlV10/BaseToDom.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1646 2023-05-06 19:50:36.000000 oglio-0.7.7/oglio/toXmlV10/OglClassesToDom.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5803 2023-05-06 19:50:47.000000 oglio-0.7.7/oglio/toXmlV10/OglLinksToDom.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1598 2023-05-06 19:51:01.000000 oglio-0.7.7/oglio/toXmlV10/OglNotesToDom.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2622 2023-05-10 20:43:22.000000 oglio-0.7.7/oglio/toXmlV10/OglSequenceToDom.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1569 2023-05-06 14:32:39.000000 oglio-0.7.7/oglio/toXmlV10/OglTextsToDom.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6676 2023-05-06 14:32:39.000000 oglio-0.7.7/oglio/toXmlV10/OglToDom.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2787 2023-05-06 19:51:31.000000 oglio-0.7.7/oglio/toXmlV10/OglUseCasesToDom.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    14155 2023-05-08 17:31:58.000000 oglio-0.7.7/oglio/toXmlV10/PyutToDom.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3831 2022-08-19 17:25:32.000000 oglio-0.7.7/oglio/toXmlV10/XmlConstants.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-08-16 17:46:46.000000 oglio-0.7.7/oglio/toXmlV10/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-08-07 19:55:58.000000 oglio-0.7.7/oglio/toXmlV10/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-09 22:30:08.459524 oglio-0.7.7/oglio.egg-info/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2335 2023-06-09 22:30:08.000000 oglio-0.7.7/oglio.egg-info/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      773 2023-06-09 22:30:08.000000 oglio-0.7.7/oglio.egg-info/SOURCES.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2023-06-09 22:30:08.000000 oglio-0.7.7/oglio.egg-info/dependency_links.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      104 2023-06-09 22:30:08.000000 oglio-0.7.7/oglio.egg-info/requires.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        6 2023-06-09 22:30:08.000000 oglio-0.7.7/oglio.egg-info/top_level.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-06-09 22:30:08.461755 oglio-0.7.7/setup.cfg
--rw-------   0 humberto.a.sanchez.ii   (501) staff       (20)      965 2023-06-09 22:16:24.000000 oglio-0.7.7/setup.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-08-06 04:01:07.532020 oglio-1.0.0/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2022-07-20 17:57:30.000000 oglio-1.0.0/LICENSE
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2335 2023-08-06 04:01:07.531899 oglio-1.0.0/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2011 2023-04-13 20:29:58.000000 oglio-1.0.0/README.md
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-08-06 04:01:07.528646 oglio-1.0.0/oglio/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1016 2023-05-08 19:24:39.000000 oglio-1.0.0/oglio/IDFactory.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       82 2023-02-13 18:01:45.000000 oglio-1.0.0/oglio/OglVersion.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4580 2023-05-06 14:32:39.000000 oglio-1.0.0/oglio/Reader.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3826 2023-05-06 14:32:39.000000 oglio-1.0.0/oglio/Types.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      123 2022-10-13 12:50:37.000000 oglio-1.0.0/oglio/UnsupportedFileTypeException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2200 2023-08-06 03:59:50.000000 oglio-1.0.0/oglio/Writer.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-05-15 01:03:15.000000 oglio-1.0.0/oglio/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       27 2023-08-06 03:59:50.000000 oglio-1.0.0/oglio/_version.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-08-07 19:55:58.000000 oglio-1.0.0/oglio/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-08-06 04:01:07.531758 oglio-1.0.0/oglio/toXmlV10/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1913 2023-05-06 19:50:19.000000 oglio-1.0.0/oglio/toXmlV10/BaseOglToDom.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      569 2022-08-26 20:55:45.000000 oglio-1.0.0/oglio/toXmlV10/BasePyutToDom.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      132 2023-05-08 00:21:01.000000 oglio-1.0.0/oglio/toXmlV10/BaseToDom.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1646 2023-05-06 19:50:36.000000 oglio-1.0.0/oglio/toXmlV10/OglClassesToDom.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5792 2023-08-06 03:59:50.000000 oglio-1.0.0/oglio/toXmlV10/OglLinksToDom.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1598 2023-05-06 19:51:01.000000 oglio-1.0.0/oglio/toXmlV10/OglNotesToDom.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2622 2023-05-10 20:43:22.000000 oglio-1.0.0/oglio/toXmlV10/OglSequenceToDom.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1569 2023-05-06 14:32:39.000000 oglio-1.0.0/oglio/toXmlV10/OglTextsToDom.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     7158 2023-08-06 03:59:50.000000 oglio-1.0.0/oglio/toXmlV10/OglToDom.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2787 2023-05-06 19:51:31.000000 oglio-1.0.0/oglio/toXmlV10/OglUseCasesToDom.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    14155 2023-05-08 17:31:58.000000 oglio-1.0.0/oglio/toXmlV10/PyutToDom.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3831 2022-08-19 17:25:32.000000 oglio-1.0.0/oglio/toXmlV10/XmlConstants.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-08-16 17:46:46.000000 oglio-1.0.0/oglio/toXmlV10/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-08-07 19:55:58.000000 oglio-1.0.0/oglio/toXmlV10/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-08-06 04:01:07.529172 oglio-1.0.0/oglio.egg-info/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2335 2023-08-06 04:01:07.000000 oglio-1.0.0/oglio.egg-info/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      773 2023-08-06 04:01:07.000000 oglio-1.0.0/oglio.egg-info/SOURCES.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2023-08-06 04:01:07.000000 oglio-1.0.0/oglio.egg-info/dependency_links.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      103 2023-08-06 04:01:07.000000 oglio-1.0.0/oglio.egg-info/requires.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        6 2023-08-06 04:01:07.000000 oglio-1.0.0/oglio.egg-info/top_level.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-08-06 04:01:07.532051 oglio-1.0.0/setup.cfg
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      964 2023-08-06 03:59:50.000000 oglio-1.0.0/setup.py
```

### Comparing `oglio-0.7.7/LICENSE` & `oglio-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oglio-0.7.7/PKG-INFO` & `oglio-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oglio
-Version: 0.7.7
+Version: 1.0.0
 Summary: External Pyut Persistence
 Home-page: https://github.com/hasii2011/oglio
 Author-email: Humberto.A.Sanchez.II@gmail.com
 Maintainer: Humberto A. Sanchez II
 Maintainer-email: humberto.a.sanchez.ii@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: oglio Version: 0.7.7 Summary: External Pyut
+Metadata-Version: 2.1 Name: oglio Version: 1.0.0 Summary: External Pyut
 Persistence Home-page: https://github.com/hasii2011/oglio Author-email:
 Humberto.A.Sanchez.II@gmail.com Maintainer: Humberto A. Sanchez II Maintainer-
 email: humberto.a.sanchez.ii@gmail.com Description-Content-Type: text/markdown
 License-File: LICENSE [./docs/agpl-license-web-badge-version-2-256x48.png] [!
 [Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https:
 //GitHub.com/Naereen/StrapDown.js/graphs/commit-activity) [![CircleCI](https://
 dl.circleci.com/status-badge/img/gh/hasii2011/oglio/tree/
```

### Comparing `oglio-0.7.7/README.md` & `oglio-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `oglio-0.7.7/oglio/IDFactory.py` & `oglio-1.0.0/oglio/IDFactory.py`

 * *Files identical despite different names*

### Comparing `oglio-0.7.7/oglio/Reader.py` & `oglio-1.0.0/oglio/Reader.py`

 * *Files identical despite different names*

### Comparing `oglio-0.7.7/oglio/Types.py` & `oglio-1.0.0/oglio/Types.py`

 * *Files identical despite different names*

### Comparing `oglio-0.7.7/oglio/Writer.py` & `oglio-1.0.0/oglio/Writer.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,15 +24,14 @@
     def writeFile(self, oglProject: OglProject, fqFileName: str):
         """
         Writes to a compressed Pyut file
 
         Args:
             oglProject:     The project we have to serialize
             fqFileName:     Where to write the XML;  Should be a full qualified file name
-
         """
         if fqFileName.endswith('.put') is False:
             fqFileName = f'{fqFileName}.put'
 
         oglToMiniDom: OglToMiniDomV10 = OglToMiniDomV10(projectVersion=oglProject.version, projectCodePath=oglProject.codePath)
 
         for oglDocument in oglProject.oglDocuments.values():
@@ -43,24 +42,24 @@
         self.logger.info(f'{ZLIB_VERSION=}')
         byteText:        bytes  = rawXml.encode()
         compressedBytes: bytes = compress(byteText)
 
         with open(fqFileName, "wb") as binaryIO:
             binaryIO.write(compressedBytes)
 
-    def writeXmlFile(self, oglProject: OglProject, fqFileName: str):
+    def writeXmlFile(self, oglProject: OglProject, fqFileName: str, prettyXml: bool = True):
         """
         Writes to an XML file
         Args:
             oglProject:     The project we have to serialize
             fqFileName:     Where to write the XML;  Should be a full qualified file name
+            prettyXml:      Format it or not?
         """
         if fqFileName.endswith('.xml') is False:
             fqFileName = f'{fqFileName}.xml'
 
         oglToMiniDom: OglToMiniDomV10 = OglToMiniDomV10(projectVersion=oglProject.version, projectCodePath=oglProject.codePath)
 
         for oglDocument in oglProject.oglDocuments.values():
             oglToMiniDom.serialize(oglDocument=oglDocument)
 
-        oglToMiniDom.writeXml(fqFileName=fqFileName)
-
+        oglToMiniDom.writeXml(fqFileName=fqFileName, prettyXml=prettyXml)
```

### Comparing `oglio-0.7.7/oglio/toXmlV10/BaseOglToDom.py` & `oglio-1.0.0/oglio/toXmlV10/BaseOglToDom.py`

 * *Files identical despite different names*

### Comparing `oglio-0.7.7/oglio/toXmlV10/BasePyutToDom.py` & `oglio-1.0.0/oglio/toXmlV10/BasePyutToDom.py`

 * *Files identical despite different names*

### Comparing `oglio-0.7.7/oglio/toXmlV10/OglClassesToDom.py` & `oglio-1.0.0/oglio/toXmlV10/OglClassesToDom.py`

 * *Files identical despite different names*

### Comparing `oglio-0.7.7/oglio/toXmlV10/OglLinksToDom.py` & `oglio-1.0.0/oglio/toXmlV10/OglLinksToDom.py`

 * *Files 7% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 
             assocLabels = {
                 XmlConstants.ELEMENT_ASSOC_CENTER_LABEL:      center,
                 XmlConstants.ELEMENT_ASSOC_SOURCE_LABEL:      src,
                 XmlConstants.ELEMENT_ASSOC_DESTINATION_LABEL: dst
             }
             for eltName in assocLabels:
-                elt: Element = self.__createAssocLabelElement(eltName, xmlDoc, assocLabels[eltName])
+                elt: Element = self._createAssocLabelElement(eltName, xmlDoc, assocLabels[eltName])
                 root.appendChild(elt)
 
         # save control points (not anchors!)
         for x, y in oglLink.segments[1:-1]:
             item = xmlDoc.createElement(XmlConstants.ELEMENT_MODEL_CONTROL_POINT)
             item.setAttribute(XmlConstants.ATTR_X, str(x))
             item.setAttribute(XmlConstants.ATTR_Y, str(y))
@@ -120,20 +120,20 @@
         # adding the data layer object
 
         root.appendChild(self._pyutToMiniDom.pyutLinkToDom(oglLink.pyutObject, xmlDoc))
 
         return root
 
     # noinspection SpellCheckingInspection
-    def __createAssocLabelElement(self, eltText: str, xmlDoc: Document, oglLabel: OglAssociationLabel) -> Element:
+    def _createAssocLabelElement(self, eltText: str, xmlDoc: Document, oglLabel: OglAssociationLabel) -> Element:
         """
         Creates an element of the form:
 
         ```html
-        `<eltText x="nnnn.n" y="nnnn.n"/>`
+        `<eltText x="nnnn" y="nnnn"/>`
         ```
 
         e.g.
 
         ```html
             `<LabelCenter x="1811" y="1137"/>`
         ```
@@ -144,16 +144,15 @@
             oglLabel:   A description of a label includes text and position
 
         Returns:
             A new minidom element
         """
         label: Element = xmlDoc.createElement(eltText)
 
-        x: int = oglLabel.oglPosition.x
-        y: int = oglLabel.oglPosition.y
+        x, y = oglLabel.GetPosition()
 
-        simpleX, simpleY = self._getSimpleCoordinates(x, y)
-        self.linksLogger.debug(f'x,y = ({x},{y})   simpleX,simpleY = ({simpleX},{simpleY})')
-        label.setAttribute(XmlConstants.ATTR_X, simpleX)
-        label.setAttribute(XmlConstants.ATTR_Y, simpleY)
+        relativeX, relativeY = oglLabel.ConvertCoordToRelative(x=x, y=y)
+        self.linksLogger.warning(f'x,y = ({x},{y})   relativeX,relativeY = ({relativeX},{relativeY})')
+        label.setAttribute(XmlConstants.ATTR_X, str(relativeX))
+        label.setAttribute(XmlConstants.ATTR_Y, str(relativeY))
 
         return label
```

### Comparing `oglio-0.7.7/oglio/toXmlV10/OglNotesToDom.py` & `oglio-1.0.0/oglio/toXmlV10/OglNotesToDom.py`

 * *Files identical despite different names*

### Comparing `oglio-0.7.7/oglio/toXmlV10/OglSequenceToDom.py` & `oglio-1.0.0/oglio/toXmlV10/OglSequenceToDom.py`

 * *Files identical despite different names*

### Comparing `oglio-0.7.7/oglio/toXmlV10/OglTextsToDom.py` & `oglio-1.0.0/oglio/toXmlV10/OglTextsToDom.py`

 * *Files identical despite different names*

### Comparing `oglio-0.7.7/oglio/toXmlV10/OglToDom.py` & `oglio-1.0.0/oglio/toXmlV10/OglToDom.py`

 * *Files 8% similar despite different names*

```diff
@@ -78,16 +78,31 @@
 
     @property
     def xml(self) -> str:
         """
 
         Returns:  The serialized XML in pretty print format
         """
-        xmlText:    str = self._xmlDocument.toprettyxml()
-        updatedXml: str = OglToDom.setAsISOLatin(xmlText)
+        updatedXml: str = ''
+        try:
+            xmlText:    str = self._xmlDocument.toxml()
+            updatedXml = OglToDom.setAsISOLatin(xmlText)
+        except (ValueError, Exception) as e:
+            self.logger.error(f'{e=}')
+
+        return updatedXml
+
+    @property
+    def prettyXml(self) -> str:
+        updatedXml: str = ''
+        try:
+            xmlText:    str = self._xmlDocument.toprettyxml()
+            updatedXml = OglToDom.setAsISOLatin(xmlText)
+        except (ValueError, Exception) as e:
+            self.logger.error(f'{e=}')
 
         return updatedXml
 
     def serialize(self, oglDocument: OglDocument):
 
         documentNode: Element = self._oglDocumentToXml(oglDocument=oglDocument)
 
@@ -107,25 +122,26 @@
         documentNode = self._oglTextsToDom.serialize(documentNode=documentNode, oglTexts=oglTexts)
         documentNode = self._oglUseCasesToMiniDom.serialize(documentNode=documentNode, oglUseCases=oglUseCases, oglActors=oglActors)
         documentNode = self._oglLinksToMiniDom.serialize(documentNode=documentNode, oglLinks=oglLinks)
 
         # noinspection PyUnusedLocal
         documentNode = self._oglSequenceToDom.serialize(documentNode=documentNode, oglSDMessages=oglSDMessages, oglSDInstances=oglSDInstances)
 
-    def writeXml(self, fqFileName):
+    def writeXml(self, fqFileName: str, prettyXml: bool = True):
         """
         Persist the XML
 
         Args:
             fqFileName:  The fully qualified file name
+            prettyXml:   Do you Barbie XML?
         """
-
-        # xmlText:    str = self._xmlDocument.toprettyxml()
-        # updatedXml: str = OglToDom.setAsISOLatin(xmlText)
-        updatedXml: str = self.xml
+        if prettyXml is True:
+            updatedXml: str = self.prettyXml
+        else:
+            updatedXml = self.xml
 
         with open(fqFileName, 'w') as fd:
             fd.write(updatedXml)
 
     @classmethod
     def setAsISOLatin(cls, xmlTextToUpdate: str) -> str:
         """
```

### Comparing `oglio-0.7.7/oglio/toXmlV10/OglUseCasesToDom.py` & `oglio-1.0.0/oglio/toXmlV10/OglUseCasesToDom.py`

 * *Files identical despite different names*

### Comparing `oglio-0.7.7/oglio/toXmlV10/PyutToDom.py` & `oglio-1.0.0/oglio/toXmlV10/PyutToDom.py`

 * *Files identical despite different names*

### Comparing `oglio-0.7.7/oglio/toXmlV10/XmlConstants.py` & `oglio-1.0.0/oglio/toXmlV10/XmlConstants.py`

 * *Files identical despite different names*

### Comparing `oglio-0.7.7/oglio.egg-info/PKG-INFO` & `oglio-1.0.0/oglio.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oglio
-Version: 0.7.7
+Version: 1.0.0
 Summary: External Pyut Persistence
 Home-page: https://github.com/hasii2011/oglio
 Author-email: Humberto.A.Sanchez.II@gmail.com
 Maintainer: Humberto A. Sanchez II
 Maintainer-email: humberto.a.sanchez.ii@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: oglio Version: 0.7.7 Summary: External Pyut
+Metadata-Version: 2.1 Name: oglio Version: 1.0.0 Summary: External Pyut
 Persistence Home-page: https://github.com/hasii2011/oglio Author-email:
 Humberto.A.Sanchez.II@gmail.com Maintainer: Humberto A. Sanchez II Maintainer-
 email: humberto.a.sanchez.ii@gmail.com Description-Content-Type: text/markdown
 License-File: LICENSE [./docs/agpl-license-web-badge-version-2-256x48.png] [!
 [Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https:
 //GitHub.com/Naereen/StrapDown.js/graphs/commit-activity) [![CircleCI](https://
 dl.circleci.com/status-badge/img/gh/hasii2011/oglio/tree/
```

### Comparing `oglio-0.7.7/oglio.egg-info/SOURCES.txt` & `oglio-1.0.0/oglio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oglio-0.7.7/setup.py` & `oglio-1.0.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -22,10 +22,10 @@
     packages=[
         'oglio', 'oglio.toXmlV10'
     ],
     package_data={
         'oglio':          ['py.typed'],
         'oglio.toXmlV10': ['py.typed']
     },
-    install_requires=['wxPython==4.2.1', 'hasiihelper~=0.2.1', 'hasiicommon~=0.3.1', 'pyutmodel~=1.4.4', 'ogl==0.70.52', 'untanglepyut==0.7.0',
+    install_requires=['wxPython==4.2.1', 'hasiihelper~=0.2.1', 'hasiicommon~=0.3.1', 'pyutmodel~=1.4.4', 'ogl==0.85.0', 'untanglepyut==1.1.0',
     ],
 )
```

