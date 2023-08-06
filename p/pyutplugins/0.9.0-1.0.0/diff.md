# Comparing `tmp/pyutplugins-0.9.0.tar.gz` & `tmp/pyutplugins-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyutplugins-0.9.0.tar", last modified: Thu Jun 29 15:11:33 2023, max compression
+gzip compressed data, was "pyutplugins-1.0.0.tar", last modified: Sun Aug  6 15:38:43 2023, max compression
```

## Comparing `pyutplugins-0.9.0.tar` & `pyutplugins-1.0.0.tar`

### file list

```diff
@@ -1,148 +1,148 @@
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-29 15:11:33.273498 pyutplugins-0.9.0/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2023-01-04 04:11:16.000000 pyutplugins-0.9.0/LICENSE
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2310 2023-06-29 15:11:33.273377 pyutplugins-0.9.0/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1956 2023-04-14 20:22:33.000000 pyutplugins-0.9.0/README.md
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-29 15:11:33.260925 pyutplugins-0.9.0/pyutplugins/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6615 2023-06-09 22:58:23.000000 pyutplugins-0.9.0/pyutplugins/ExternalTypes.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3210 2023-01-20 18:33:44.000000 pyutplugins-0.9.0/pyutplugins/IPluginAdapter.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8054 2023-03-31 00:30:02.000000 pyutplugins-0.9.0/pyutplugins/PluginManager.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       45 2023-05-15 01:25:03.000000 pyutplugins-0.9.0/pyutplugins/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       27 2023-06-09 22:52:00.000000 pyutplugins-0.9.0/pyutplugins/_version.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-29 15:11:33.262010 pyutplugins-0.9.0/pyutplugins/common/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1130 2023-01-04 04:11:16.000000 pyutplugins-0.9.0/pyutplugins/common/ElementTreeData.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2353 2023-01-04 04:11:16.000000 pyutplugins-0.9.0/pyutplugins/common/LinkMakerMixin.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      469 2023-01-19 02:57:18.000000 pyutplugins-0.9.0/pyutplugins/common/PluginTypes.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.9.0/pyutplugins/common/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.9.0/pyutplugins/common/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-29 15:11:33.262289 pyutplugins-0.9.0/pyutplugins/common/ui/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2224 2023-01-20 15:07:17.000000 pyutplugins-0.9.0/pyutplugins/common/ui/BaseEditDialog.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.9.0/pyutplugins/common/ui/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-29 15:11:33.262502 pyutplugins-0.9.0/pyutplugins/common/ui/preferences/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5175 2023-05-03 19:43:51.000000 pyutplugins-0.9.0/pyutplugins/common/ui/preferences/PluginPreferencesPage.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-02-01 02:55:47.000000 pyutplugins-0.9.0/pyutplugins/common/ui/preferences/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.9.0/pyutplugins/common/ui/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-29 15:11:33.263040 pyutplugins-0.9.0/pyutplugins/exceptions/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       66 2023-01-04 04:11:16.000000 pyutplugins-0.9.0/pyutplugins/exceptions/AbstractMethodNotImplementedException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       60 2023-01-04 04:11:16.000000 pyutplugins-0.9.0/pyutplugins/exceptions/InvalidPluginExtensionException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       55 2023-01-04 04:11:16.000000 pyutplugins-0.9.0/pyutplugins/exceptions/InvalidPluginNameException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.9.0/pyutplugins/exceptions/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.9.0/pyutplugins/exceptions/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-29 15:11:33.264192 pyutplugins-0.9.0/pyutplugins/ioplugins/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1924 2023-01-20 18:45:21.000000 pyutplugins-0.9.0/pyutplugins/ioplugins/IOAscii.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2893 2023-01-20 18:45:20.000000 pyutplugins-0.9.0/pyutplugins/ioplugins/IODTD.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2849 2023-01-20 18:45:20.000000 pyutplugins-0.9.0/pyutplugins/ioplugins/IOGML.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4134 2023-01-20 18:45:20.000000 pyutplugins-0.9.0/pyutplugins/ioplugins/IOJava.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3245 2023-01-30 01:49:48.000000 pyutplugins-0.9.0/pyutplugins/ioplugins/IOMermaid.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3864 2023-02-03 02:52:30.000000 pyutplugins-0.9.0/pyutplugins/ioplugins/IOPdf.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     7942 2023-05-05 01:14:03.000000 pyutplugins-0.9.0/pyutplugins/ioplugins/IOPython.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4078 2023-01-20 18:45:20.000000 pyutplugins-0.9.0/pyutplugins/ioplugins/IOWxImage.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8266 2023-01-30 01:49:48.000000 pyutplugins-0.9.0/pyutplugins/ioplugins/IOXml.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.9.0/pyutplugins/ioplugins/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-29 15:11:33.264673 pyutplugins-0.9.0/pyutplugins/ioplugins/dtd/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      326 2023-01-04 04:11:16.000000 pyutplugins-0.9.0/pyutplugins/ioplugins/dtd/DTDAttribute.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      430 2023-01-04 04:11:16.000000 pyutplugins-0.9.0/pyutplugins/ioplugins/dtd/DTDElementTypes.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    10397 2023-01-20 18:33:44.000000 pyutplugins-0.9.0/pyutplugins/ioplugins/dtd/DTDParser.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.9.0/pyutplugins/ioplugins/dtd/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.9.0/pyutplugins/ioplugins/dtd/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-29 15:11:33.265079 pyutplugins-0.9.0/pyutplugins/ioplugins/gml/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8647 2023-02-01 01:59:25.000000 pyutplugins-0.9.0/pyutplugins/ioplugins/gml/GMLExporter.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       49 2023-01-04 04:11:16.000000 pyutplugins-0.9.0/pyutplugins/ioplugins/gml/UnsupportedOperation.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.9.0/pyutplugins/ioplugins/gml/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.9.0/pyutplugins/ioplugins/gml/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-29 15:11:33.265473 pyutplugins-0.9.0/pyutplugins/ioplugins/java/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    27944 2023-01-20 18:45:21.000000 pyutplugins-0.9.0/pyutplugins/ioplugins/java/JavaReader.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    11156 2023-02-01 01:52:43.000000 pyutplugins-0.9.0/pyutplugins/ioplugins/java/JavaWriter.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.9.0/pyutplugins/ioplugins/java/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.9.0/pyutplugins/ioplugins/java/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-29 15:11:33.265846 pyutplugins-0.9.0/pyutplugins/ioplugins/mermaid/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      994 2023-02-01 20:38:32.000000 pyutplugins-0.9.0/pyutplugins/ioplugins/mermaid/MermaidDirection.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    12464 2023-04-17 23:17:22.000000 pyutplugins-0.9.0/pyutplugins/ioplugins/mermaid/MermaidWriter.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-30 01:49:48.000000 pyutplugins-0.9.0/pyutplugins/ioplugins/mermaid/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.9.0/pyutplugins/ioplugins/mermaid/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-29 15:11:33.266327 pyutplugins-0.9.0/pyutplugins/ioplugins/pdf/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      132 2023-01-04 04:11:16.000000 pyutplugins-0.9.0/pyutplugins/ioplugins/pdf/ImageFormat.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      554 2023-01-04 04:11:16.000000 pyutplugins-0.9.0/pyutplugins/ioplugins/pdf/ImageOptions.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     9562 2023-06-18 22:27:15.000000 pyutplugins-0.9.0/pyutplugins/ioplugins/pdf/OglToPyUmlDefinition.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.9.0/pyutplugins/ioplugins/pdf/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.9.0/pyutplugins/ioplugins/pdf/py.typed
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.9.0/pyutplugins/ioplugins/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-29 15:11:33.267342 pyutplugins-0.9.0/pyutplugins/ioplugins/python/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6135 2023-05-05 01:14:03.000000 pyutplugins-0.9.0/pyutplugins/ioplugins/python/DlgSelectMultiplePackages.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3579 2023-01-04 04:11:16.000000 pyutplugins-0.9.0/pyutplugins/ioplugins/python/Python3LexerBase.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      192 2023-01-04 04:11:16.000000 pyutplugins-0.9.0/pyutplugins/ioplugins/python/Python3ParserBase.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       49 2023-01-04 04:11:16.000000 pyutplugins-0.9.0/pyutplugins/ioplugins/python/PythonParseException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    12836 2023-01-04 04:11:16.000000 pyutplugins-0.9.0/pyutplugins/ioplugins/python/PyutPythonVisitor.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    12487 2023-01-04 04:11:16.000000 pyutplugins-0.9.0/pyutplugins/ioplugins/python/PyutToPython.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    18319 2023-05-05 01:14:03.000000 pyutplugins-0.9.0/pyutplugins/ioplugins/python/ReverseEngineerPython2.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.9.0/pyutplugins/ioplugins/python/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.9.0/pyutplugins/ioplugins/python/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-29 15:11:33.268151 pyutplugins-0.9.0/pyutplugins/ioplugins/python/pyantlrparser/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    47673 2023-01-04 04:11:16.000000 pyutplugins-0.9.0/pyutplugins/ioplugins/python/pyantlrparser/Python3Lexer.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)   399206 2023-01-04 04:11:16.000000 pyutplugins-0.9.0/pyutplugins/ioplugins/python/pyantlrparser/Python3Parser.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    37475 2023-01-04 04:11:16.000000 pyutplugins-0.9.0/pyutplugins/ioplugins/python/pyantlrparser/Python3ParserListener.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    22412 2023-01-04 04:11:16.000000 pyutplugins-0.9.0/pyutplugins/ioplugins/python/pyantlrparser/Python3ParserVisitor.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.9.0/pyutplugins/ioplugins/python/pyantlrparser/py.typed
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      804 2023-01-04 04:11:16.000000 pyutplugins-0.9.0/pyutplugins/ioplugins/python/transformGrammar.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-29 15:11:33.268538 pyutplugins-0.9.0/pyutplugins/ioplugins/wximage/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4853 2023-05-05 01:14:03.000000 pyutplugins-0.9.0/pyutplugins/ioplugins/wximage/DlgWxImageOptions.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      929 2023-01-04 04:11:16.000000 pyutplugins-0.9.0/pyutplugins/ioplugins/wximage/WxImageFormat.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.9.0/pyutplugins/ioplugins/wximage/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.9.0/pyutplugins/ioplugins/wximage/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-29 15:11:33.269029 pyutplugins-0.9.0/pyutplugins/plugininterfaces/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    11797 2023-05-03 19:43:51.000000 pyutplugins-0.9.0/pyutplugins/plugininterfaces/BasePluginInterface.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5202 2023-01-20 21:59:06.000000 pyutplugins-0.9.0/pyutplugins/plugininterfaces/IOPluginInterface.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1226 2023-01-20 15:37:30.000000 pyutplugins-0.9.0/pyutplugins/plugininterfaces/ToolPluginInterface.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.9.0/pyutplugins/plugininterfaces/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.9.0/pyutplugins/plugininterfaces/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-29 15:11:33.270195 pyutplugins-0.9.0/pyutplugins/plugintypes/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2131 2023-02-03 02:56:53.000000 pyutplugins-0.9.0/pyutplugins/plugintypes/BaseFormat.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      112 2023-01-04 04:11:16.000000 pyutplugins-0.9.0/pyutplugins/plugintypes/BaseRequestResponse.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      225 2023-01-20 18:45:20.000000 pyutplugins-0.9.0/pyutplugins/plugintypes/ExportDirectoryResponse.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      205 2023-01-20 18:45:20.000000 pyutplugins-0.9.0/pyutplugins/plugintypes/ImportDirectoryResponse.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      532 2023-01-20 18:45:20.000000 pyutplugins-0.9.0/pyutplugins/plugintypes/InputFormat.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      330 2023-01-20 18:45:21.000000 pyutplugins-0.9.0/pyutplugins/plugintypes/MultipleFileRequestResponse.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      533 2023-01-20 18:45:20.000000 pyutplugins-0.9.0/pyutplugins/plugintypes/OutputFormat.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1766 2023-01-20 18:45:20.000000 pyutplugins-0.9.0/pyutplugins/plugintypes/PluginDataTypes.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      202 2023-01-20 18:45:21.000000 pyutplugins-0.9.0/pyutplugins/plugintypes/SingleFileRequestResponse.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       52 2023-01-04 04:11:16.000000 pyutplugins-0.9.0/pyutplugins/plugintypes/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.9.0/pyutplugins/plugintypes/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-29 15:11:33.270482 pyutplugins-0.9.0/pyutplugins/preferences/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     7651 2023-03-31 00:30:24.000000 pyutplugins-0.9.0/pyutplugins/preferences/PluginPreferences.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-18 02:02:54.000000 pyutplugins-0.9.0/pyutplugins/preferences/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 pyutplugins-0.9.0/pyutplugins/preferences/py.typed
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.9.0/pyutplugins/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-29 15:11:33.271278 pyutplugins-0.9.0/pyutplugins/toolplugins/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1730 2023-01-20 18:45:20.000000 pyutplugins-0.9.0/pyutplugins/toolplugins/ToolArrangeLinks.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3592 2023-01-20 18:45:20.000000 pyutplugins-0.9.0/pyutplugins/toolplugins/ToolAscii.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4402 2023-01-20 18:45:21.000000 pyutplugins-0.9.0/pyutplugins/toolplugins/ToolOrthogonalLayoutV2.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3159 2023-01-20 18:45:20.000000 pyutplugins-0.9.0/pyutplugins/toolplugins/ToolSugiyama.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1989 2023-01-20 18:45:20.000000 pyutplugins-0.9.0/pyutplugins/toolplugins/ToolTransforms.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.9.0/pyutplugins/toolplugins/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-29 15:11:33.271960 pyutplugins-0.9.0/pyutplugins/toolplugins/orthogonal/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1996 2023-05-03 19:43:51.000000 pyutplugins-0.9.0/pyutplugins/toolplugins/orthogonal/DlgLayoutSize.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      737 2023-01-19 03:33:52.000000 pyutplugins-0.9.0/pyutplugins/toolplugins/orthogonal/LayoutAreaSize.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5230 2023-01-20 18:33:44.000000 pyutplugins-0.9.0/pyutplugins/toolplugins/orthogonal/OrthogonalAdapter.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       55 2023-01-04 04:11:16.000000 pyutplugins-0.9.0/pyutplugins/toolplugins/orthogonal/OrthogonalAdapterException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.9.0/pyutplugins/toolplugins/orthogonal/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.9.0/pyutplugins/toolplugins/orthogonal/py.typed
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.9.0/pyutplugins/toolplugins/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-29 15:11:33.273229 pyutplugins-0.9.0/pyutplugins/toolplugins/sugiyama/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3545 2023-02-22 02:39:48.000000 pyutplugins-0.9.0/pyutplugins/toolplugins/sugiyama/ALayoutLink.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1025 2023-01-04 04:11:16.000000 pyutplugins-0.9.0/pyutplugins/toolplugins/sugiyama/ALayoutNode.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3262 2023-01-04 04:11:16.000000 pyutplugins-0.9.0/pyutplugins/toolplugins/sugiyama/RealSugiyamaNode.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    28462 2023-02-01 01:51:21.000000 pyutplugins-0.9.0/pyutplugins/toolplugins/sugiyama/Sugiyama.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      263 2023-01-04 04:11:16.000000 pyutplugins-0.9.0/pyutplugins/toolplugins/sugiyama/SugiyamaConstants.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2108 2023-01-20 15:25:55.000000 pyutplugins-0.9.0/pyutplugins/toolplugins/sugiyama/SugiyamaGlobals.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3228 2023-01-04 04:11:16.000000 pyutplugins-0.9.0/pyutplugins/toolplugins/sugiyama/SugiyamaLink.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    14778 2023-01-04 04:11:16.000000 pyutplugins-0.9.0/pyutplugins/toolplugins/sugiyama/SugiyamaNode.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1387 2023-01-04 04:11:16.000000 pyutplugins-0.9.0/pyutplugins/toolplugins/sugiyama/VirtualSugiyamaNode.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.9.0/pyutplugins/toolplugins/sugiyama/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.9.0/pyutplugins/toolplugins/sugiyama/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-29 15:11:33.261450 pyutplugins-0.9.0/pyutplugins.egg-info/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2310 2023-06-29 15:11:33.000000 pyutplugins-0.9.0/pyutplugins.egg-info/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5185 2023-06-29 15:11:33.000000 pyutplugins-0.9.0/pyutplugins.egg-info/SOURCES.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2023-06-29 15:11:33.000000 pyutplugins-0.9.0/pyutplugins.egg-info/dependency_links.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      202 2023-06-29 15:11:33.000000 pyutplugins-0.9.0/pyutplugins.egg-info/requires.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       12 2023-06-29 15:11:33.000000 pyutplugins-0.9.0/pyutplugins.egg-info/top_level.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-06-29 15:11:33.273530 pyutplugins-0.9.0/setup.cfg
--rw-------   0 humberto.a.sanchez.ii   (501) staff       (20)     3112 2023-06-18 20:58:33.000000 pyutplugins-0.9.0/setup.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-08-06 15:38:43.901741 pyutplugins-1.0.0/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2023-01-04 04:11:16.000000 pyutplugins-1.0.0/LICENSE
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2310 2023-08-06 15:38:43.901600 pyutplugins-1.0.0/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1956 2023-04-14 20:22:33.000000 pyutplugins-1.0.0/README.md
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-08-06 15:38:43.875845 pyutplugins-1.0.0/pyutplugins/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6615 2023-06-09 22:58:23.000000 pyutplugins-1.0.0/pyutplugins/ExternalTypes.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3210 2023-01-20 18:33:44.000000 pyutplugins-1.0.0/pyutplugins/IPluginAdapter.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8054 2023-03-31 00:30:02.000000 pyutplugins-1.0.0/pyutplugins/PluginManager.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       45 2023-05-15 01:25:03.000000 pyutplugins-1.0.0/pyutplugins/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       27 2023-08-06 04:08:43.000000 pyutplugins-1.0.0/pyutplugins/_version.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-08-06 15:38:43.877416 pyutplugins-1.0.0/pyutplugins/common/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1130 2023-01-04 04:11:16.000000 pyutplugins-1.0.0/pyutplugins/common/ElementTreeData.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2353 2023-01-04 04:11:16.000000 pyutplugins-1.0.0/pyutplugins/common/LinkMakerMixin.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      469 2023-01-19 02:57:18.000000 pyutplugins-1.0.0/pyutplugins/common/PluginTypes.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-1.0.0/pyutplugins/common/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-1.0.0/pyutplugins/common/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-08-06 15:38:43.877884 pyutplugins-1.0.0/pyutplugins/common/ui/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2224 2023-01-20 15:07:17.000000 pyutplugins-1.0.0/pyutplugins/common/ui/BaseEditDialog.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-1.0.0/pyutplugins/common/ui/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-08-06 15:38:43.878286 pyutplugins-1.0.0/pyutplugins/common/ui/preferences/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5175 2023-05-03 19:43:51.000000 pyutplugins-1.0.0/pyutplugins/common/ui/preferences/PluginPreferencesPage.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-02-01 02:55:47.000000 pyutplugins-1.0.0/pyutplugins/common/ui/preferences/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-1.0.0/pyutplugins/common/ui/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-08-06 15:38:43.879218 pyutplugins-1.0.0/pyutplugins/exceptions/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       66 2023-01-04 04:11:16.000000 pyutplugins-1.0.0/pyutplugins/exceptions/AbstractMethodNotImplementedException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       60 2023-01-04 04:11:16.000000 pyutplugins-1.0.0/pyutplugins/exceptions/InvalidPluginExtensionException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       55 2023-01-04 04:11:16.000000 pyutplugins-1.0.0/pyutplugins/exceptions/InvalidPluginNameException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-1.0.0/pyutplugins/exceptions/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-1.0.0/pyutplugins/exceptions/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-08-06 15:38:43.881579 pyutplugins-1.0.0/pyutplugins/ioplugins/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1924 2023-01-20 18:45:21.000000 pyutplugins-1.0.0/pyutplugins/ioplugins/IOAscii.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2893 2023-01-20 18:45:20.000000 pyutplugins-1.0.0/pyutplugins/ioplugins/IODTD.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2849 2023-01-20 18:45:20.000000 pyutplugins-1.0.0/pyutplugins/ioplugins/IOGML.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4134 2023-01-20 18:45:20.000000 pyutplugins-1.0.0/pyutplugins/ioplugins/IOJava.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3245 2023-01-30 01:49:48.000000 pyutplugins-1.0.0/pyutplugins/ioplugins/IOMermaid.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3864 2023-02-03 02:52:30.000000 pyutplugins-1.0.0/pyutplugins/ioplugins/IOPdf.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     7942 2023-05-05 01:14:03.000000 pyutplugins-1.0.0/pyutplugins/ioplugins/IOPython.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4078 2023-01-20 18:45:20.000000 pyutplugins-1.0.0/pyutplugins/ioplugins/IOWxImage.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8278 2023-08-04 16:55:54.000000 pyutplugins-1.0.0/pyutplugins/ioplugins/IOXml.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-1.0.0/pyutplugins/ioplugins/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-08-06 15:38:43.882417 pyutplugins-1.0.0/pyutplugins/ioplugins/dtd/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      326 2023-01-04 04:11:16.000000 pyutplugins-1.0.0/pyutplugins/ioplugins/dtd/DTDAttribute.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      430 2023-01-04 04:11:16.000000 pyutplugins-1.0.0/pyutplugins/ioplugins/dtd/DTDElementTypes.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    10397 2023-01-20 18:33:44.000000 pyutplugins-1.0.0/pyutplugins/ioplugins/dtd/DTDParser.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-1.0.0/pyutplugins/ioplugins/dtd/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-1.0.0/pyutplugins/ioplugins/dtd/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-08-06 15:38:43.883046 pyutplugins-1.0.0/pyutplugins/ioplugins/gml/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8647 2023-02-01 01:59:25.000000 pyutplugins-1.0.0/pyutplugins/ioplugins/gml/GMLExporter.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       49 2023-01-04 04:11:16.000000 pyutplugins-1.0.0/pyutplugins/ioplugins/gml/UnsupportedOperation.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-1.0.0/pyutplugins/ioplugins/gml/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-1.0.0/pyutplugins/ioplugins/gml/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-08-06 15:38:43.885145 pyutplugins-1.0.0/pyutplugins/ioplugins/java/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    27944 2023-01-20 18:45:21.000000 pyutplugins-1.0.0/pyutplugins/ioplugins/java/JavaReader.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    11156 2023-02-01 01:52:43.000000 pyutplugins-1.0.0/pyutplugins/ioplugins/java/JavaWriter.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-1.0.0/pyutplugins/ioplugins/java/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-1.0.0/pyutplugins/ioplugins/java/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-08-06 15:38:43.885915 pyutplugins-1.0.0/pyutplugins/ioplugins/mermaid/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      994 2023-02-01 20:38:32.000000 pyutplugins-1.0.0/pyutplugins/ioplugins/mermaid/MermaidDirection.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    12464 2023-04-17 23:17:22.000000 pyutplugins-1.0.0/pyutplugins/ioplugins/mermaid/MermaidWriter.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-30 01:49:48.000000 pyutplugins-1.0.0/pyutplugins/ioplugins/mermaid/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-1.0.0/pyutplugins/ioplugins/mermaid/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-08-06 15:38:43.886683 pyutplugins-1.0.0/pyutplugins/ioplugins/pdf/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      132 2023-01-04 04:11:16.000000 pyutplugins-1.0.0/pyutplugins/ioplugins/pdf/ImageFormat.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      554 2023-01-04 04:11:16.000000 pyutplugins-1.0.0/pyutplugins/ioplugins/pdf/ImageOptions.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     9562 2023-06-18 22:27:15.000000 pyutplugins-1.0.0/pyutplugins/ioplugins/pdf/OglToPyUmlDefinition.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-1.0.0/pyutplugins/ioplugins/pdf/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-1.0.0/pyutplugins/ioplugins/pdf/py.typed
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-1.0.0/pyutplugins/ioplugins/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-08-06 15:38:43.888477 pyutplugins-1.0.0/pyutplugins/ioplugins/python/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6135 2023-05-05 01:14:03.000000 pyutplugins-1.0.0/pyutplugins/ioplugins/python/DlgSelectMultiplePackages.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3579 2023-01-04 04:11:16.000000 pyutplugins-1.0.0/pyutplugins/ioplugins/python/Python3LexerBase.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      192 2023-01-04 04:11:16.000000 pyutplugins-1.0.0/pyutplugins/ioplugins/python/Python3ParserBase.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       49 2023-01-04 04:11:16.000000 pyutplugins-1.0.0/pyutplugins/ioplugins/python/PythonParseException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    12836 2023-01-04 04:11:16.000000 pyutplugins-1.0.0/pyutplugins/ioplugins/python/PyutPythonVisitor.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    12487 2023-01-04 04:11:16.000000 pyutplugins-1.0.0/pyutplugins/ioplugins/python/PyutToPython.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    18319 2023-05-05 01:14:03.000000 pyutplugins-1.0.0/pyutplugins/ioplugins/python/ReverseEngineerPython2.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-1.0.0/pyutplugins/ioplugins/python/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-1.0.0/pyutplugins/ioplugins/python/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-08-06 15:38:43.890139 pyutplugins-1.0.0/pyutplugins/ioplugins/python/pyantlrparser/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    47673 2023-01-04 04:11:16.000000 pyutplugins-1.0.0/pyutplugins/ioplugins/python/pyantlrparser/Python3Lexer.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)   399206 2023-01-04 04:11:16.000000 pyutplugins-1.0.0/pyutplugins/ioplugins/python/pyantlrparser/Python3Parser.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    37475 2023-01-04 04:11:16.000000 pyutplugins-1.0.0/pyutplugins/ioplugins/python/pyantlrparser/Python3ParserListener.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    22412 2023-01-04 04:11:16.000000 pyutplugins-1.0.0/pyutplugins/ioplugins/python/pyantlrparser/Python3ParserVisitor.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-1.0.0/pyutplugins/ioplugins/python/pyantlrparser/py.typed
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      804 2023-01-04 04:11:16.000000 pyutplugins-1.0.0/pyutplugins/ioplugins/python/transformGrammar.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-08-06 15:38:43.890659 pyutplugins-1.0.0/pyutplugins/ioplugins/wximage/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4853 2023-05-05 01:14:03.000000 pyutplugins-1.0.0/pyutplugins/ioplugins/wximage/DlgWxImageOptions.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      929 2023-01-04 04:11:16.000000 pyutplugins-1.0.0/pyutplugins/ioplugins/wximage/WxImageFormat.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-1.0.0/pyutplugins/ioplugins/wximage/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-1.0.0/pyutplugins/ioplugins/wximage/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-08-06 15:38:43.893531 pyutplugins-1.0.0/pyutplugins/plugininterfaces/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    11797 2023-05-03 19:43:51.000000 pyutplugins-1.0.0/pyutplugins/plugininterfaces/BasePluginInterface.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5202 2023-01-20 21:59:06.000000 pyutplugins-1.0.0/pyutplugins/plugininterfaces/IOPluginInterface.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1226 2023-01-20 15:37:30.000000 pyutplugins-1.0.0/pyutplugins/plugininterfaces/ToolPluginInterface.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-1.0.0/pyutplugins/plugininterfaces/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-1.0.0/pyutplugins/plugininterfaces/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-08-06 15:38:43.895784 pyutplugins-1.0.0/pyutplugins/plugintypes/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2131 2023-02-03 02:56:53.000000 pyutplugins-1.0.0/pyutplugins/plugintypes/BaseFormat.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      112 2023-01-04 04:11:16.000000 pyutplugins-1.0.0/pyutplugins/plugintypes/BaseRequestResponse.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      225 2023-01-20 18:45:20.000000 pyutplugins-1.0.0/pyutplugins/plugintypes/ExportDirectoryResponse.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      205 2023-01-20 18:45:20.000000 pyutplugins-1.0.0/pyutplugins/plugintypes/ImportDirectoryResponse.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      532 2023-01-20 18:45:20.000000 pyutplugins-1.0.0/pyutplugins/plugintypes/InputFormat.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      330 2023-01-20 18:45:21.000000 pyutplugins-1.0.0/pyutplugins/plugintypes/MultipleFileRequestResponse.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      533 2023-01-20 18:45:20.000000 pyutplugins-1.0.0/pyutplugins/plugintypes/OutputFormat.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1766 2023-01-20 18:45:20.000000 pyutplugins-1.0.0/pyutplugins/plugintypes/PluginDataTypes.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      202 2023-01-20 18:45:21.000000 pyutplugins-1.0.0/pyutplugins/plugintypes/SingleFileRequestResponse.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       52 2023-01-04 04:11:16.000000 pyutplugins-1.0.0/pyutplugins/plugintypes/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-1.0.0/pyutplugins/plugintypes/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-08-06 15:38:43.896220 pyutplugins-1.0.0/pyutplugins/preferences/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     7651 2023-03-31 00:30:24.000000 pyutplugins-1.0.0/pyutplugins/preferences/PluginPreferences.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-18 02:02:54.000000 pyutplugins-1.0.0/pyutplugins/preferences/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 pyutplugins-1.0.0/pyutplugins/preferences/py.typed
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-1.0.0/pyutplugins/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-08-06 15:38:43.897660 pyutplugins-1.0.0/pyutplugins/toolplugins/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1730 2023-01-20 18:45:20.000000 pyutplugins-1.0.0/pyutplugins/toolplugins/ToolArrangeLinks.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3592 2023-01-20 18:45:20.000000 pyutplugins-1.0.0/pyutplugins/toolplugins/ToolAscii.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4402 2023-01-20 18:45:21.000000 pyutplugins-1.0.0/pyutplugins/toolplugins/ToolOrthogonalLayoutV2.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3159 2023-01-20 18:45:20.000000 pyutplugins-1.0.0/pyutplugins/toolplugins/ToolSugiyama.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1989 2023-01-20 18:45:20.000000 pyutplugins-1.0.0/pyutplugins/toolplugins/ToolTransforms.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-1.0.0/pyutplugins/toolplugins/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-08-06 15:38:43.898914 pyutplugins-1.0.0/pyutplugins/toolplugins/orthogonal/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1996 2023-05-03 19:43:51.000000 pyutplugins-1.0.0/pyutplugins/toolplugins/orthogonal/DlgLayoutSize.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      737 2023-01-19 03:33:52.000000 pyutplugins-1.0.0/pyutplugins/toolplugins/orthogonal/LayoutAreaSize.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5230 2023-01-20 18:33:44.000000 pyutplugins-1.0.0/pyutplugins/toolplugins/orthogonal/OrthogonalAdapter.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       55 2023-01-04 04:11:16.000000 pyutplugins-1.0.0/pyutplugins/toolplugins/orthogonal/OrthogonalAdapterException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-1.0.0/pyutplugins/toolplugins/orthogonal/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-1.0.0/pyutplugins/toolplugins/orthogonal/py.typed
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-1.0.0/pyutplugins/toolplugins/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-08-06 15:38:43.901430 pyutplugins-1.0.0/pyutplugins/toolplugins/sugiyama/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3545 2023-02-22 02:39:48.000000 pyutplugins-1.0.0/pyutplugins/toolplugins/sugiyama/ALayoutLink.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1025 2023-01-04 04:11:16.000000 pyutplugins-1.0.0/pyutplugins/toolplugins/sugiyama/ALayoutNode.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3262 2023-01-04 04:11:16.000000 pyutplugins-1.0.0/pyutplugins/toolplugins/sugiyama/RealSugiyamaNode.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    28462 2023-02-01 01:51:21.000000 pyutplugins-1.0.0/pyutplugins/toolplugins/sugiyama/Sugiyama.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      263 2023-01-04 04:11:16.000000 pyutplugins-1.0.0/pyutplugins/toolplugins/sugiyama/SugiyamaConstants.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2108 2023-01-20 15:25:55.000000 pyutplugins-1.0.0/pyutplugins/toolplugins/sugiyama/SugiyamaGlobals.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3228 2023-01-04 04:11:16.000000 pyutplugins-1.0.0/pyutplugins/toolplugins/sugiyama/SugiyamaLink.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    14778 2023-01-04 04:11:16.000000 pyutplugins-1.0.0/pyutplugins/toolplugins/sugiyama/SugiyamaNode.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1387 2023-01-04 04:11:16.000000 pyutplugins-1.0.0/pyutplugins/toolplugins/sugiyama/VirtualSugiyamaNode.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-1.0.0/pyutplugins/toolplugins/sugiyama/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-1.0.0/pyutplugins/toolplugins/sugiyama/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-08-06 15:38:43.876413 pyutplugins-1.0.0/pyutplugins.egg-info/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2310 2023-08-06 15:38:43.000000 pyutplugins-1.0.0/pyutplugins.egg-info/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5185 2023-08-06 15:38:43.000000 pyutplugins-1.0.0/pyutplugins.egg-info/SOURCES.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2023-08-06 15:38:43.000000 pyutplugins-1.0.0/pyutplugins.egg-info/dependency_links.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      201 2023-08-06 15:38:43.000000 pyutplugins-1.0.0/pyutplugins.egg-info/requires.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       12 2023-08-06 15:38:43.000000 pyutplugins-1.0.0/pyutplugins.egg-info/top_level.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-08-06 15:38:43.901777 pyutplugins-1.0.0/setup.cfg
+-rw-------   0 humberto.a.sanchez.ii   (501) staff       (20)     3111 2023-08-06 04:11:08.000000 pyutplugins-1.0.0/setup.py
```

### Comparing `pyutplugins-0.9.0/LICENSE` & `pyutplugins-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.9.0/PKG-INFO` & `pyutplugins-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyutplugins
-Version: 0.9.0
+Version: 1.0.0
 Summary: Pyut Plugins
 Home-page: https://github.com/hasii2011/pyutplugins
 Author: Humberto A. Sanchez II
 Author-email: humberto.a.sanchez.ii@gmail.com
 Maintainer: Humberto A. Sanchez II
 Maintainer-email: humberto.a.sanchez.ii@gmail.com
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyutplugins Version: 0.9.0 Summary: Pyut Plugins
+Metadata-Version: 2.1 Name: pyutplugins Version: 1.0.0 Summary: Pyut Plugins
 Home-page: https://github.com/hasii2011/pyutplugins Author: Humberto A. Sanchez
 II Author-email: humberto.a.sanchez.ii@gmail.com Maintainer: Humberto A.
 Sanchez II Maintainer-email: humberto.a.sanchez.ii@gmail.com Description-
 Content-Type: text/markdown License-File: LICENSE [./developer/agpl-license-
 web-badge-version-2-256x48.png] [![Maintenance](https://img.shields.io/badge/
 Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/
 commit-activity) [![CircleCI](https://dl.circleci.com/status-badge/img/gh/
```

### Comparing `pyutplugins-0.9.0/README.md` & `pyutplugins-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.9.0/pyutplugins/ExternalTypes.py` & `pyutplugins-1.0.0/pyutplugins/ExternalTypes.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.9.0/pyutplugins/IPluginAdapter.py` & `pyutplugins-1.0.0/pyutplugins/IPluginAdapter.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.9.0/pyutplugins/PluginManager.py` & `pyutplugins-1.0.0/pyutplugins/PluginManager.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.9.0/pyutplugins/common/ElementTreeData.py` & `pyutplugins-1.0.0/pyutplugins/common/ElementTreeData.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.9.0/pyutplugins/common/LinkMakerMixin.py` & `pyutplugins-1.0.0/pyutplugins/common/LinkMakerMixin.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.9.0/pyutplugins/common/ui/BaseEditDialog.py` & `pyutplugins-1.0.0/pyutplugins/common/ui/BaseEditDialog.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.9.0/pyutplugins/common/ui/preferences/PluginPreferencesPage.py` & `pyutplugins-1.0.0/pyutplugins/common/ui/preferences/PluginPreferencesPage.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.9.0/pyutplugins/ioplugins/IOAscii.py` & `pyutplugins-1.0.0/pyutplugins/ioplugins/IOAscii.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.9.0/pyutplugins/ioplugins/IODTD.py` & `pyutplugins-1.0.0/pyutplugins/ioplugins/IODTD.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.9.0/pyutplugins/ioplugins/IOGML.py` & `pyutplugins-1.0.0/pyutplugins/ioplugins/IOGML.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.9.0/pyutplugins/ioplugins/IOJava.py` & `pyutplugins-1.0.0/pyutplugins/ioplugins/IOJava.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.9.0/pyutplugins/ioplugins/IOMermaid.py` & `pyutplugins-1.0.0/pyutplugins/ioplugins/IOMermaid.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.9.0/pyutplugins/ioplugins/IOPdf.py` & `pyutplugins-1.0.0/pyutplugins/ioplugins/IOPdf.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.9.0/pyutplugins/ioplugins/IOPython.py` & `pyutplugins-1.0.0/pyutplugins/ioplugins/IOPython.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.9.0/pyutplugins/ioplugins/IOWxImage.py` & `pyutplugins-1.0.0/pyutplugins/ioplugins/IOWxImage.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.9.0/pyutplugins/ioplugins/IOXml.py` & `pyutplugins-1.0.0/pyutplugins/ioplugins/IOXml.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,24 +91,26 @@
     def setExportOptions(self) -> bool:
         """
         Prepare the export.
 
         Returns:
         """
         prettPrintAnswer: int = MessageBox("Do you want pretty xml ?", "Export option", style=YES_NO | CANCEL | CENTRE | ICON_QUESTION)
+
         if prettPrintAnswer is YES:
             self._prettyPrint = True
-            response: SingleFileRequestResponse = self.askForFileToExport()
-            if response.cancelled is True:
-                exportAnswer: bool = False
-            else:
-                self._fileToExport = response.fileName
-                exportAnswer = True
         else:
-            exportAnswer = False
+            self._prettyPrint = False
+
+        response: SingleFileRequestResponse = self.askForFileToExport()
+        if response.cancelled is True:
+            exportAnswer: bool = False
+        else:
+            self._fileToExport = response.fileName
+            exportAnswer = True
 
         return exportAnswer
 
     def read(self) -> bool:
         reader: Reader = Reader()
 
         oglProject: OglProject = reader.readXmlFile(fqFileName=self._fileToImport)
@@ -186,8 +188,8 @@
 
             self.logger.debug(f'{oglDocument=}')
 
             oglProject.oglDocuments[oglDocument.documentTitle] = oglDocument
 
         writer:     Writer = Writer()
 
-        writer.writeXmlFile(oglProject=oglProject, fqFileName=self._fileToExport)
+        writer.writeXmlFile(oglProject=oglProject, fqFileName=self._fileToExport, prettyXml=self._prettyPrint)
```

### Comparing `pyutplugins-0.9.0/pyutplugins/ioplugins/dtd/DTDParser.py` & `pyutplugins-1.0.0/pyutplugins/ioplugins/dtd/DTDParser.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.9.0/pyutplugins/ioplugins/gml/GMLExporter.py` & `pyutplugins-1.0.0/pyutplugins/ioplugins/gml/GMLExporter.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.9.0/pyutplugins/ioplugins/java/JavaReader.py` & `pyutplugins-1.0.0/pyutplugins/ioplugins/java/JavaReader.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.9.0/pyutplugins/ioplugins/java/JavaWriter.py` & `pyutplugins-1.0.0/pyutplugins/ioplugins/java/JavaWriter.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.9.0/pyutplugins/ioplugins/mermaid/MermaidDirection.py` & `pyutplugins-1.0.0/pyutplugins/ioplugins/mermaid/MermaidDirection.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.9.0/pyutplugins/ioplugins/mermaid/MermaidWriter.py` & `pyutplugins-1.0.0/pyutplugins/ioplugins/mermaid/MermaidWriter.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.9.0/pyutplugins/ioplugins/pdf/ImageOptions.py` & `pyutplugins-1.0.0/pyutplugins/ioplugins/pdf/ImageOptions.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.9.0/pyutplugins/ioplugins/pdf/OglToPyUmlDefinition.py` & `pyutplugins-1.0.0/pyutplugins/ioplugins/pdf/OglToPyUmlDefinition.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.9.0/pyutplugins/ioplugins/python/DlgSelectMultiplePackages.py` & `pyutplugins-1.0.0/pyutplugins/ioplugins/python/DlgSelectMultiplePackages.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.9.0/pyutplugins/ioplugins/python/Python3LexerBase.py` & `pyutplugins-1.0.0/pyutplugins/ioplugins/python/Python3LexerBase.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.9.0/pyutplugins/ioplugins/python/PyutPythonVisitor.py` & `pyutplugins-1.0.0/pyutplugins/ioplugins/python/PyutPythonVisitor.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.9.0/pyutplugins/ioplugins/python/PyutToPython.py` & `pyutplugins-1.0.0/pyutplugins/ioplugins/python/PyutToPython.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.9.0/pyutplugins/ioplugins/python/ReverseEngineerPython2.py` & `pyutplugins-1.0.0/pyutplugins/ioplugins/python/ReverseEngineerPython2.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.9.0/pyutplugins/ioplugins/python/pyantlrparser/Python3Lexer.py` & `pyutplugins-1.0.0/pyutplugins/ioplugins/python/pyantlrparser/Python3Lexer.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.9.0/pyutplugins/ioplugins/python/pyantlrparser/Python3Parser.py` & `pyutplugins-1.0.0/pyutplugins/ioplugins/python/pyantlrparser/Python3Parser.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.9.0/pyutplugins/ioplugins/python/pyantlrparser/Python3ParserListener.py` & `pyutplugins-1.0.0/pyutplugins/ioplugins/python/pyantlrparser/Python3ParserListener.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.9.0/pyutplugins/ioplugins/python/pyantlrparser/Python3ParserVisitor.py` & `pyutplugins-1.0.0/pyutplugins/ioplugins/python/pyantlrparser/Python3ParserVisitor.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.9.0/pyutplugins/ioplugins/python/transformGrammar.py` & `pyutplugins-1.0.0/pyutplugins/ioplugins/python/transformGrammar.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.9.0/pyutplugins/ioplugins/wximage/DlgWxImageOptions.py` & `pyutplugins-1.0.0/pyutplugins/ioplugins/wximage/DlgWxImageOptions.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.9.0/pyutplugins/ioplugins/wximage/WxImageFormat.py` & `pyutplugins-1.0.0/pyutplugins/ioplugins/wximage/WxImageFormat.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.9.0/pyutplugins/plugininterfaces/BasePluginInterface.py` & `pyutplugins-1.0.0/pyutplugins/plugininterfaces/BasePluginInterface.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.9.0/pyutplugins/plugininterfaces/IOPluginInterface.py` & `pyutplugins-1.0.0/pyutplugins/plugininterfaces/IOPluginInterface.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.9.0/pyutplugins/plugininterfaces/ToolPluginInterface.py` & `pyutplugins-1.0.0/pyutplugins/plugininterfaces/ToolPluginInterface.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.9.0/pyutplugins/plugintypes/BaseFormat.py` & `pyutplugins-1.0.0/pyutplugins/plugintypes/BaseFormat.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.9.0/pyutplugins/plugintypes/InputFormat.py` & `pyutplugins-1.0.0/pyutplugins/plugintypes/InputFormat.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.9.0/pyutplugins/plugintypes/OutputFormat.py` & `pyutplugins-1.0.0/pyutplugins/plugintypes/OutputFormat.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.9.0/pyutplugins/plugintypes/PluginDataTypes.py` & `pyutplugins-1.0.0/pyutplugins/plugintypes/PluginDataTypes.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.9.0/pyutplugins/preferences/PluginPreferences.py` & `pyutplugins-1.0.0/pyutplugins/preferences/PluginPreferences.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.9.0/pyutplugins/toolplugins/ToolArrangeLinks.py` & `pyutplugins-1.0.0/pyutplugins/toolplugins/ToolArrangeLinks.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.9.0/pyutplugins/toolplugins/ToolAscii.py` & `pyutplugins-1.0.0/pyutplugins/toolplugins/ToolAscii.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.9.0/pyutplugins/toolplugins/ToolOrthogonalLayoutV2.py` & `pyutplugins-1.0.0/pyutplugins/toolplugins/ToolOrthogonalLayoutV2.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.9.0/pyutplugins/toolplugins/ToolSugiyama.py` & `pyutplugins-1.0.0/pyutplugins/toolplugins/ToolSugiyama.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.9.0/pyutplugins/toolplugins/ToolTransforms.py` & `pyutplugins-1.0.0/pyutplugins/toolplugins/ToolTransforms.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.9.0/pyutplugins/toolplugins/orthogonal/DlgLayoutSize.py` & `pyutplugins-1.0.0/pyutplugins/toolplugins/orthogonal/DlgLayoutSize.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.9.0/pyutplugins/toolplugins/orthogonal/LayoutAreaSize.py` & `pyutplugins-1.0.0/pyutplugins/toolplugins/orthogonal/LayoutAreaSize.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.9.0/pyutplugins/toolplugins/orthogonal/OrthogonalAdapter.py` & `pyutplugins-1.0.0/pyutplugins/toolplugins/orthogonal/OrthogonalAdapter.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.9.0/pyutplugins/toolplugins/sugiyama/ALayoutLink.py` & `pyutplugins-1.0.0/pyutplugins/toolplugins/sugiyama/ALayoutLink.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.9.0/pyutplugins/toolplugins/sugiyama/ALayoutNode.py` & `pyutplugins-1.0.0/pyutplugins/toolplugins/sugiyama/ALayoutNode.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.9.0/pyutplugins/toolplugins/sugiyama/RealSugiyamaNode.py` & `pyutplugins-1.0.0/pyutplugins/toolplugins/sugiyama/RealSugiyamaNode.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.9.0/pyutplugins/toolplugins/sugiyama/Sugiyama.py` & `pyutplugins-1.0.0/pyutplugins/toolplugins/sugiyama/Sugiyama.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.9.0/pyutplugins/toolplugins/sugiyama/SugiyamaGlobals.py` & `pyutplugins-1.0.0/pyutplugins/toolplugins/sugiyama/SugiyamaGlobals.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.9.0/pyutplugins/toolplugins/sugiyama/SugiyamaLink.py` & `pyutplugins-1.0.0/pyutplugins/toolplugins/sugiyama/SugiyamaLink.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.9.0/pyutplugins/toolplugins/sugiyama/SugiyamaNode.py` & `pyutplugins-1.0.0/pyutplugins/toolplugins/sugiyama/SugiyamaNode.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.9.0/pyutplugins/toolplugins/sugiyama/VirtualSugiyamaNode.py` & `pyutplugins-1.0.0/pyutplugins/toolplugins/sugiyama/VirtualSugiyamaNode.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.9.0/pyutplugins.egg-info/PKG-INFO` & `pyutplugins-1.0.0/pyutplugins.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyutplugins
-Version: 0.9.0
+Version: 1.0.0
 Summary: Pyut Plugins
 Home-page: https://github.com/hasii2011/pyutplugins
 Author: Humberto A. Sanchez II
 Author-email: humberto.a.sanchez.ii@gmail.com
 Maintainer: Humberto A. Sanchez II
 Maintainer-email: humberto.a.sanchez.ii@gmail.com
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyutplugins Version: 0.9.0 Summary: Pyut Plugins
+Metadata-Version: 2.1 Name: pyutplugins Version: 1.0.0 Summary: Pyut Plugins
 Home-page: https://github.com/hasii2011/pyutplugins Author: Humberto A. Sanchez
 II Author-email: humberto.a.sanchez.ii@gmail.com Maintainer: Humberto A.
 Sanchez II Maintainer-email: humberto.a.sanchez.ii@gmail.com Description-
 Content-Type: text/markdown License-File: LICENSE [./developer/agpl-license-
 web-badge-version-2-256x48.png] [![Maintenance](https://img.shields.io/badge/
 Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/
 commit-activity) [![CircleCI](https://dl.circleci.com/status-badge/img/gh/
```

### Comparing `pyutplugins-0.9.0/pyutplugins.egg-info/SOURCES.txt` & `pyutplugins-1.0.0/pyutplugins.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.9.0/setup.py` & `pyutplugins-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         'pyutplugins.ioplugins.mermaid', 'pyutplugins.ioplugins.pdf', 'pyutplugins.ioplugins.python', 'pyutplugins.ioplugins.python.pyantlrparser',
         'pyutplugins.ioplugins.wximage',
         'pyutplugins.plugininterfaces',
         'pyutplugins.plugintypes',
         'pyutplugins.preferences',
         'pyutplugins.toolplugins', 'pyutplugins.toolplugins.orthogonal', 'pyutplugins.toolplugins.sugiyama',
     ],
-    install_requires=['pyutmodel==1.4.4', 'ogl==0.70.52', 'untanglepyut==0.7.0', 'oglio==0.7.7', 'hasiihelper~=0.2.1', 'hasiicommon~=0.3.1',
+    install_requires=['pyutmodel==1.4.4', 'ogl==0.85.0', 'untanglepyut==1.1.0', 'oglio==1.0.0', 'hasiihelper~=0.2.1', 'hasiicommon~=0.3.1',
                       'wxPython~=4.2.1',
                       'antlr4-python3-runtime==4.11.1',
                       'networkx==3.0',
                       'pyumldiagrams==2.40.0',
                       'orthogonal==1.1.8',
                       ]
 )
```

