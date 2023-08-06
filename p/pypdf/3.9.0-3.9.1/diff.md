# Comparing `tmp/pypdf-3.9.0.tar.gz` & `tmp/pypdf-3.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypdf-3.9.0.tar", last modified: Sun May 21 14:56:59 2023, max compression
+gzip compressed data, was "pypdf-3.9.1.tar", last modified: Sun Jun  4 18:57:11 2023, max compression
```

## Comparing `pypdf-3.9.0.tar` & `pypdf-3.9.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0      488 2022-12-10 23:30:58.176669 pypdf-3.9.0/.git-blame-ignore-revs
--rw-r--r--   0        0        0      542 2023-03-29 15:43:03.262713 pypdf-3.9.0/.readthedocs.yaml
--rw-r--r--   0        0        0    36621 2023-05-21 14:54:48.403973 pypdf-3.9.0/CHANGELOG.md
--rw-r--r--   0        0        0     3524 2023-04-23 19:34:52.051441 pypdf-3.9.0/CONTRIBUTORS.md
--rw-r--r--   0        0        0     1605 2022-12-10 23:30:58.184669 pypdf-3.9.0/LICENSE
--rw-r--r--   0        0        0       34 2022-12-10 23:30:58.184669 pypdf-3.9.0/MANIFEST.in
--rw-r--r--   0        0        0     4729 2023-04-09 16:59:02.663368 pypdf-3.9.0/README.md
--rw-r--r--   0        0        0     1234 2023-03-04 08:55:07.145847 pypdf-3.9.0/pypdf/__init__.py
--rw-r--r--   0        0        0    15026 2023-05-01 06:46:17.882777 pypdf-3.9.0/pypdf/_cmap.py
--rw-r--r--   0        0        0     1674 2023-02-28 08:12:53.909178 pypdf-3.9.0/pypdf/_codecs/__init__.py
--rw-r--r--   0        0        0   431492 2022-12-31 10:47:18.999493 pypdf-3.9.0/pypdf/_codecs/adobe_glyphs.py
--rw-r--r--   0        0        0     4269 2022-12-31 10:47:18.999493 pypdf-3.9.0/pypdf/_codecs/pdfdoc.py
--rw-r--r--   0        0        0     2630 2023-02-28 08:12:53.909178 pypdf-3.9.0/pypdf/_codecs/std.py
--rw-r--r--   0        0        0     3734 2022-12-31 10:47:18.999493 pypdf-3.9.0/pypdf/_codecs/symbol.py
--rw-r--r--   0        0        0     3742 2022-12-31 10:47:18.999493 pypdf-3.9.0/pypdf/_codecs/zapfding.py
--rw-r--r--   0        0        0    47438 2023-05-01 06:46:17.882777 pypdf-3.9.0/pypdf/_encryption.py
--rw-r--r--   0        0        0    30706 2023-04-19 17:12:20.725394 pypdf-3.9.0/pypdf/_merger.py
--rw-r--r--   0        0        0    82680 2023-05-21 14:54:31.239909 pypdf-3.9.0/pypdf/_page.py
--rw-r--r--   0        0        0     7186 2023-03-04 08:55:07.145847 pypdf-3.9.0/pypdf/_page_labels.py
--rw-r--r--   0        0        0     1927 2023-04-30 11:32:55.458233 pypdf-3.9.0/pypdf/_protocols.py
--rw-r--r--   0        0        0    86233 2023-05-21 14:54:31.239909 pypdf-3.9.0/pypdf/_reader.py
--rw-r--r--   0        0        0    12788 2023-03-31 16:21:44.806544 pypdf-3.9.0/pypdf/_security.py
--rw-r--r--   0        0        0    10008 2023-03-12 09:43:33.014879 pypdf-3.9.0/pypdf/_text_extraction/__init__.py
--rw-r--r--   0        0        0    14912 2023-04-19 17:12:20.729394 pypdf-3.9.0/pypdf/_utils.py
--rw-r--r--   0        0        0       22 2023-05-21 14:54:53.255991 pypdf-3.9.0/pypdf/_version.py
--rw-r--r--   0        0        0   124317 2023-05-21 14:54:31.243909 pypdf-3.9.0/pypdf/_writer.py
--rw-r--r--   0        0        0    16147 2023-04-09 16:59:02.667368 pypdf-3.9.0/pypdf/constants.py
--rw-r--r--   0        0        0     1631 2023-03-04 08:55:07.149847 pypdf-3.9.0/pypdf/errors.py
--rw-r--r--   0        0        0    26910 2023-05-01 06:46:17.882777 pypdf-3.9.0/pypdf/filters.py
--rw-r--r--   0        0        0     4549 2023-04-09 16:59:02.667368 pypdf-3.9.0/pypdf/generic/__init__.py
--rw-r--r--   0        0        0    17368 2023-04-08 20:27:58.309582 pypdf-3.9.0/pypdf/generic/_annotations.py
--rw-r--r--   0        0        0    24911 2023-04-30 11:32:55.462233 pypdf-3.9.0/pypdf/generic/_base.py
--rw-r--r--   0        0        0    55007 2023-05-21 14:54:31.243909 pypdf-3.9.0/pypdf/generic/_data_structures.py
--rw-r--r--   0        0        0     5427 2023-03-04 08:55:07.149847 pypdf-3.9.0/pypdf/generic/_fit.py
--rw-r--r--   0        0        0     1202 2023-04-30 11:32:55.462233 pypdf-3.9.0/pypdf/generic/_outline.py
--rw-r--r--   0        0        0     8826 2023-03-04 08:55:07.149847 pypdf-3.9.0/pypdf/generic/_rectangle.py
--rw-r--r--   0        0        0     6405 2023-03-04 11:49:14.882511 pypdf-3.9.0/pypdf/generic/_utils.py
--rw-r--r--   0        0        0     6880 2023-03-04 08:55:07.153847 pypdf-3.9.0/pypdf/pagerange.py
--rw-r--r--   0        0        0     1369 2023-02-28 08:12:53.917178 pypdf-3.9.0/pypdf/papersizes.py
--rw-r--r--   0        0        0        0 2022-12-31 10:47:19.003493 pypdf-3.9.0/pypdf/py.typed
--rw-r--r--   0        0        0     2135 2023-03-29 15:43:03.266713 pypdf-3.9.0/pypdf/types.py
--rw-r--r--   0        0        0    17886 2023-04-30 11:32:55.462233 pypdf-3.9.0/pypdf/xmp.py
--rw-r--r--   0        0        0     7480 2023-05-01 06:46:17.882777 pypdf-3.9.0/pyproject.toml
--rw-r--r--   0        0        0     1585 2023-02-05 10:26:02.030123 pypdf-3.9.0/setup.cfg
--rw-r--r--   0        0        0     6763 1970-01-01 00:00:00.000000 pypdf-3.9.0/PKG-INFO
+-rw-r--r--   0        0        0      488 2022-12-10 23:30:58.176669 pypdf-3.9.1/.git-blame-ignore-revs
+-rw-r--r--   0        0        0      542 2023-03-29 15:43:03.262713 pypdf-3.9.1/.readthedocs.yaml
+-rw-r--r--   0        0        0    36714 2023-06-04 18:56:05.919284 pypdf-3.9.1/CHANGELOG.md
+-rw-r--r--   0        0        0     3710 2023-06-03 08:30:05.889279 pypdf-3.9.1/CONTRIBUTORS.md
+-rw-r--r--   0        0        0     1605 2022-12-10 23:30:58.184669 pypdf-3.9.1/LICENSE
+-rw-r--r--   0        0        0       34 2022-12-10 23:30:58.184669 pypdf-3.9.1/MANIFEST.in
+-rw-r--r--   0        0        0     4729 2023-04-09 16:59:02.663368 pypdf-3.9.1/README.md
+-rw-r--r--   0        0        0     1234 2023-03-04 08:55:07.145847 pypdf-3.9.1/pypdf/__init__.py
+-rw-r--r--   0        0        0    15026 2023-05-01 06:46:17.882777 pypdf-3.9.1/pypdf/_cmap.py
+-rw-r--r--   0        0        0     1674 2023-02-28 08:12:53.909178 pypdf-3.9.1/pypdf/_codecs/__init__.py
+-rw-r--r--   0        0        0   431492 2022-12-31 10:47:18.999493 pypdf-3.9.1/pypdf/_codecs/adobe_glyphs.py
+-rw-r--r--   0        0        0     4269 2022-12-31 10:47:18.999493 pypdf-3.9.1/pypdf/_codecs/pdfdoc.py
+-rw-r--r--   0        0        0     2630 2023-02-28 08:12:53.909178 pypdf-3.9.1/pypdf/_codecs/std.py
+-rw-r--r--   0        0        0     3734 2022-12-31 10:47:18.999493 pypdf-3.9.1/pypdf/_codecs/symbol.py
+-rw-r--r--   0        0        0     3742 2022-12-31 10:47:18.999493 pypdf-3.9.1/pypdf/_codecs/zapfding.py
+-rw-r--r--   0        0        0    47438 2023-05-01 06:46:17.882777 pypdf-3.9.1/pypdf/_encryption.py
+-rw-r--r--   0        0        0    30418 2023-06-04 18:54:50.606965 pypdf-3.9.1/pypdf/_merger.py
+-rw-r--r--   0        0        0    82680 2023-05-21 14:54:31.239909 pypdf-3.9.1/pypdf/_page.py
+-rw-r--r--   0        0        0     7186 2023-03-04 08:55:07.145847 pypdf-3.9.1/pypdf/_page_labels.py
+-rw-r--r--   0        0        0     1927 2023-04-30 11:32:55.458233 pypdf-3.9.1/pypdf/_protocols.py
+-rw-r--r--   0        0        0    86233 2023-05-21 14:54:31.239909 pypdf-3.9.1/pypdf/_reader.py
+-rw-r--r--   0        0        0    12788 2023-03-31 16:21:44.806544 pypdf-3.9.1/pypdf/_security.py
+-rw-r--r--   0        0        0    10008 2023-03-12 09:43:33.014879 pypdf-3.9.1/pypdf/_text_extraction/__init__.py
+-rw-r--r--   0        0        0    14912 2023-04-19 17:12:20.729394 pypdf-3.9.1/pypdf/_utils.py
+-rw-r--r--   0        0        0       22 2023-06-04 18:55:50.923222 pypdf-3.9.1/pypdf/_version.py
+-rw-r--r--   0        0        0   124460 2023-06-03 08:30:05.893279 pypdf-3.9.1/pypdf/_writer.py
+-rw-r--r--   0        0        0    16147 2023-04-09 16:59:02.667368 pypdf-3.9.1/pypdf/constants.py
+-rw-r--r--   0        0        0     1631 2023-03-04 08:55:07.149847 pypdf-3.9.1/pypdf/errors.py
+-rw-r--r--   0        0        0    26910 2023-05-01 06:46:17.882777 pypdf-3.9.1/pypdf/filters.py
+-rw-r--r--   0        0        0     4549 2023-04-09 16:59:02.667368 pypdf-3.9.1/pypdf/generic/__init__.py
+-rw-r--r--   0        0        0    17368 2023-04-08 20:27:58.309582 pypdf-3.9.1/pypdf/generic/_annotations.py
+-rw-r--r--   0        0        0    24911 2023-04-30 11:32:55.462233 pypdf-3.9.1/pypdf/generic/_base.py
+-rw-r--r--   0        0        0    55007 2023-05-21 14:54:31.243909 pypdf-3.9.1/pypdf/generic/_data_structures.py
+-rw-r--r--   0        0        0     5427 2023-03-04 08:55:07.149847 pypdf-3.9.1/pypdf/generic/_fit.py
+-rw-r--r--   0        0        0     1202 2023-04-30 11:32:55.462233 pypdf-3.9.1/pypdf/generic/_outline.py
+-rw-r--r--   0        0        0     8826 2023-03-04 08:55:07.149847 pypdf-3.9.1/pypdf/generic/_rectangle.py
+-rw-r--r--   0        0        0     6414 2023-06-03 08:30:05.893279 pypdf-3.9.1/pypdf/generic/_utils.py
+-rw-r--r--   0        0        0     6880 2023-03-04 08:55:07.153847 pypdf-3.9.1/pypdf/pagerange.py
+-rw-r--r--   0        0        0     1369 2023-02-28 08:12:53.917178 pypdf-3.9.1/pypdf/papersizes.py
+-rw-r--r--   0        0        0        0 2022-12-31 10:47:19.003493 pypdf-3.9.1/pypdf/py.typed
+-rw-r--r--   0        0        0     2135 2023-03-29 15:43:03.266713 pypdf-3.9.1/pypdf/types.py
+-rw-r--r--   0        0        0    17886 2023-04-30 11:32:55.462233 pypdf-3.9.1/pypdf/xmp.py
+-rw-r--r--   0        0        0     7480 2023-05-01 06:46:17.882777 pypdf-3.9.1/pyproject.toml
+-rw-r--r--   0        0        0     1585 2023-02-05 10:26:02.030123 pypdf-3.9.1/setup.cfg
+-rw-r--r--   0        0        0     6763 1970-01-01 00:00:00.000000 pypdf-3.9.1/PKG-INFO
```

### Comparing `pypdf-3.9.0/.readthedocs.yaml` & `pypdf-3.9.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `pypdf-3.9.0/CHANGELOG.md` & `pypdf-3.9.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,45 +1,52 @@
-Version 3.9.0, 2023-05-21
--------------------------
+# CHANGELOG
+
+## Version 3.9.1, 2023-06-04
+
+### Deprecations (DEP)
+-  Deprecate PdfMerger (#1866)
+
+### Bug Fixes (BUG)
+-  Ignore UTF-8 decode errors (#1865)
+
+### Robustness (ROB)
+-  Handle missing /Type entry in Page tree (#1859)
+
 
-New Features (ENH):
+[Full Changelog](https://github.com/py-pdf/pypdf/compare/3.9.0...3.9.1)
+
+## Version 3.9.0, 2023-05-21
+
+### New Features (ENH)
 -  Simplify metadata input (Document Information Dictionary) (#1851)
 -  Extend cmap compatibilty to GBK_EUC_H/V (#1812)
 
-Bug Fixes (BUG):
+### Bug Fixes (BUG)
 -  Prevent infinite loop when no character follows after a comment (#1828)
 -  get_contents does not return ContentStream (#1847)
 -  Accept XYZ destination with zoom missing (default to zoom=0.0) (#1844)
 -  Cope with 1 Bit images (#1815)
 
-Robustness (ROB):
+### Robustness (ROB)
 -  Handle missing /Type entry in Page tree (#1845)
 
-Documentation (DOC):
+### Documentation (DOC)
 -  Expand file size explanations (#1835)
 -  Add comparison with pdfplumber (#1837)
 -  Clarify that PyPDF2 is dead (#1827)
 -  Add Hunter King as Contributor for #1806
 
-Maintenance (MAINT):
+### Maintenance (MAINT)
 -  Refactor internal Encryption class (#1821)
 -  Add R parameter to generate_values (#1820)
 -  Make encryption_key parameter of write_to_stream optional (#1819)
 -  Prepare for adding AES enryption support (#1818)
 
-Testing (TST):
--  Parametrize test_cmap_encodings (#1823)
+[Full Changelog](https://github.com/py-pdf/pypdf/compare/3.8.1...3.9.0)
 
-Code Style (STY):
--  Iterate directly over the list instead of using range (#1839)
--  Minor refactorings in _encryption.py (#1822)
-
-[Full Changelog](https://github.com/py-pdf/pypdf/compare/3.8.1...3.8.2)
-
-# CHANGELOG
 
 ## Version 3.8.1, 2023-04-23
 
 ### Bug Fixes (BUG)
 -  Convert color space before saving (#1802)
 
 ### Documentation (DOC)
```

### Comparing `pypdf-3.9.0/CONTRIBUTORS.md` & `pypdf-3.9.1/CONTRIBUTORS.md`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 * [McNeil, Karen](https://github.com/karenlmcneil): Arabic Language Support
 * [Mérino, Antoine](https://github.com/Merinorus)
 * [Paternault, Louis](https://framagit.org/spalax)
 * [Perrensen, Olsen](https://github.com/olsonperrensen)
 * [Pinheiro, Arthur](https://github.com/xilopaint)
 * [programmarchy](https://github.com/programmarchy)
 * [pubpub-zz](https://github.com/pubpub-zz): involved in community development
+* [RitchieP](https://github.com/RitchieP) | [LinkedIn](https://www.linkedin.com/in/ritchie-p-892b31115/) | [StackOverflow](https://stackoverflow.com/users/13328625/casual-r?tab=profile)
 * [Rogmann, Sascha](https://github.com/srogmann)
 * [robbiebusinessacc](https://github.com/robbiebusinessacc)
 * [sietzeberends](https://github.com/sietzeberends)
 * [Stüber, Timo](https://github.com/omit66)
 * [Thoma, Martin](https://github.com/MartinThoma): Maintainer of pypdf since April 2022. I hope to build a great community with many awesome contributors. [LinkedIn](https://www.linkedin.com/in/martin-thoma/) | [StackOverflow](https://stackoverflow.com/users/562769/martin-thoma) | [Blog](https://martin-thoma.com/)
 * [Thomas, Reuben](https://github.com/rrthomas)
 * [WevertonGomes](https://github.com/WevertonGomesCosta)
```

### Comparing `pypdf-3.9.0/LICENSE` & `pypdf-3.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pypdf-3.9.0/README.md` & `pypdf-3.9.1/README.md`

 * *Files identical despite different names*

### Comparing `pypdf-3.9.0/pypdf/__init__.py` & `pypdf-3.9.1/pypdf/__init__.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.9.0/pypdf/_cmap.py` & `pypdf-3.9.1/pypdf/_cmap.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.9.0/pypdf/_codecs/__init__.py` & `pypdf-3.9.1/pypdf/_codecs/__init__.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.9.0/pypdf/_codecs/adobe_glyphs.py` & `pypdf-3.9.1/pypdf/_codecs/adobe_glyphs.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.9.0/pypdf/_codecs/pdfdoc.py` & `pypdf-3.9.1/pypdf/_codecs/pdfdoc.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.9.0/pypdf/_codecs/std.py` & `pypdf-3.9.1/pypdf/_codecs/std.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.9.0/pypdf/_codecs/symbol.py` & `pypdf-3.9.1/pypdf/_codecs/symbol.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.9.0/pypdf/_codecs/zapfding.py` & `pypdf-3.9.1/pypdf/_codecs/zapfding.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.9.0/pypdf/_encryption.py` & `pypdf-3.9.1/pypdf/_encryption.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.9.0/pypdf/_merger.py` & `pypdf-3.9.1/pypdf/_merger.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 )
 
 from ._encryption import Encryption
 from ._page import PageObject
 from ._reader import PdfReader
 from ._utils import (
     StrByteType,
+    deprecate_with_replacement,
     deprecation_bookmark,
     deprecation_with_replacement,
     str_,
 )
 from ._writer import PdfWriter
 from .constants import GoToActionArguments, TypArguments, TypFitArguments
 from .constants import PagesAttributes as PA
@@ -82,45 +83,36 @@
         self.pagedata = pagedata
         self.out_pagedata = None
         self.id = id
 
 
 class PdfMerger:
     """
-    Initialize a ``PdfMerger`` object.
+    Use :class:`PdfWriter` instead.
 
-    ``PdfMerger`` merges multiple PDFs into a single PDF.
-    It can concatenate, slice, insert, or any combination of the above.
-
-    See the functions :meth:`merge()<merge>` (or :meth:`append()<append>`)
-    and :meth:`write()<write>` for usage information.
-
-    Args:
-        strict: Determines whether user should be warned of all
-            problems and also causes some correctable problems to be fatal.
-            Defaults to ``False``.
-        fileobj: Output file. Can be a filename or any kind of
-            file-like object.
+    .. deprecated:: 5.0.0
     """
 
     @deprecation_bookmark(bookmarks="outline")
     def __init__(
         self, strict: bool = False, fileobj: Union[Path, StrByteType] = ""
     ) -> None:
+        deprecate_with_replacement("PdfMerger", "PdfWriter", "5.0.0")
         self.inputs: List[Tuple[Any, PdfReader]] = []
         self.pages: List[Any] = []
         self.output: Optional[PdfWriter] = PdfWriter()
         self.outline: OutlineType = []
         self.named_dests: List[Any] = []
         self.id_count = 0
         self.fileobj = fileobj
         self.strict = strict
 
     def __enter__(self) -> "PdfMerger":
         # There is nothing to do.
+        deprecate_with_replacement("PdfMerger", "PdfWriter", "5.0.0")
         return self
 
     def __exit__(
         self,
         exc_type: Optional[Type[BaseException]],
         exc: Optional[BaseException],
         traceback: Optional[TracebackType],
@@ -518,21 +510,21 @@
         return new_outline
 
     def _write_dests(self) -> None:
         if self.output is None:
             raise RuntimeError(ERR_CLOSED_WRITER)
         for named_dest in self.named_dests:
             page_index = None
-            if "/Page" in named_dest:
+            if "/Page" in named_dest:  # deprecated
                 for page_index, page in enumerate(self.pages):  # noqa: B007
                     if page.id == named_dest["/Page"]:
                         named_dest[NameObject("/Page")] = page.out_pagedata
                         break
 
-            if page_index is not None:
+            if page_index is not None:  # deprecated
                 self.output.add_named_destination_object(named_dest)
 
     @deprecation_bookmark(bookmarks="outline")
     def _write_outline(
         self,
         outline: Optional[Iterable[OutlineItem]] = None,
         parent: Optional[TreeObject] = None,
@@ -602,15 +594,15 @@
             if isinstance(np, NumberObject):
                 continue
 
             for page in pages:
                 if np.get_object() == page.pagedata.get_object():
                     page_index = page.id
 
-            if page_index is None:
+            if page_index is None:  # deprecated
                 raise ValueError(
                     f"Unresolved named destination '{named_dest['/Title']}'"
                 )
             named_dest[NameObject("/Page")] = NumberObject(page_index)
 
     @deprecation_bookmark(bookmarks="outline")
     def _associate_outline_items_to_pages(
@@ -647,15 +639,15 @@
             root = self.outline
 
         for i, oi_enum in enumerate(root):
             if isinstance(oi_enum, list):
                 # oi_enum is still an inner node
                 # (OutlineType, if recursive types were supported by mypy)
                 res = self.find_outline_item(outline_item, oi_enum)  # type: ignore
-                if res:
+                if res:  # deprecated
                     return [i] + res
             elif (
                 oi_enum == outline_item
                 or cast(Dict[Any, Any], oi_enum["/Title"]) == outline_item
             ):
                 # we found a leaf node
                 return [i]
```

### Comparing `pypdf-3.9.0/pypdf/_page.py` & `pypdf-3.9.1/pypdf/_page.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.9.0/pypdf/_page_labels.py` & `pypdf-3.9.1/pypdf/_page_labels.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.9.0/pypdf/_protocols.py` & `pypdf-3.9.1/pypdf/_protocols.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.9.0/pypdf/_reader.py` & `pypdf-3.9.1/pypdf/_reader.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.9.0/pypdf/_security.py` & `pypdf-3.9.1/pypdf/_security.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.9.0/pypdf/_text_extraction/__init__.py` & `pypdf-3.9.1/pypdf/_text_extraction/__init__.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.9.0/pypdf/_utils.py` & `pypdf-3.9.1/pypdf/_utils.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.9.0/pypdf/_writer.py` & `pypdf-3.9.1/pypdf/_writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -936,17 +936,22 @@
         )
         if inherit is None:
             inherit = {}
         if pages is None:
             pages = cast(DictionaryObject, self._root_object["/Pages"])
             self.flattened_pages = ArrayObject()
         assert pages is not None  # hint for mypy
-        t = "/Pages"
+
         if PA.TYPE in pages:
-            t = cast(str, pages[PA.TYPE])
+            t = str(pages[PA.TYPE])
+        # if pdf has no type, considered as a page if /Kids is missing
+        elif PA.KIDS not in pages:
+            t = "/Page"
+        else:
+            t = "/Pages"
 
         if t == "/Pages":
             for attr in inheritable_page_attributes:
                 if attr in pages:
                     inherit[attr] = pages[attr]
             for page in cast(ArrayObject, cast(DictionaryObject, pages)[PA.KIDS]):
                 addt = {}
```

### Comparing `pypdf-3.9.0/pypdf/constants.py` & `pypdf-3.9.1/pypdf/constants.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.9.0/pypdf/errors.py` & `pypdf-3.9.1/pypdf/errors.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.9.0/pypdf/filters.py` & `pypdf-3.9.1/pypdf/filters.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.9.0/pypdf/generic/__init__.py` & `pypdf-3.9.1/pypdf/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.9.0/pypdf/generic/_annotations.py` & `pypdf-3.9.1/pypdf/generic/_annotations.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.9.0/pypdf/generic/_base.py` & `pypdf-3.9.1/pypdf/generic/_base.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.9.0/pypdf/generic/_data_structures.py` & `pypdf-3.9.1/pypdf/generic/_data_structures.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.9.0/pypdf/generic/_fit.py` & `pypdf-3.9.1/pypdf/generic/_fit.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.9.0/pypdf/generic/_outline.py` & `pypdf-3.9.1/pypdf/generic/_outline.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.9.0/pypdf/generic/_rectangle.py` & `pypdf-3.9.1/pypdf/generic/_rectangle.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.9.0/pypdf/generic/_utils.py` & `pypdf-3.9.1/pypdf/generic/_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,15 @@
                     tok = stream.read(1)
                     if tok not in b"\n\r":
                         stream.seek(-1, 1)
                     # Then don't add anything to the actual string, since this
                     # line break was escaped:
                     tok = b""
                 else:
-                    msg = rf"Unexpected escaped string: {tok.decode('utf8')}"
+                    msg = f"Unexpected escaped string: {tok.decode('utf-8','ignore')}"
                     logger_warning(msg, __name__)
         txt.append(tok)
     return create_string_object(b"".join(txt), forced_encoding)
 
 
 def create_string_object(
     string: Union[str, bytes],
```

### Comparing `pypdf-3.9.0/pypdf/pagerange.py` & `pypdf-3.9.1/pypdf/pagerange.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.9.0/pypdf/papersizes.py` & `pypdf-3.9.1/pypdf/papersizes.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.9.0/pypdf/types.py` & `pypdf-3.9.1/pypdf/types.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.9.0/pypdf/xmp.py` & `pypdf-3.9.1/pypdf/xmp.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.9.0/pyproject.toml` & `pypdf-3.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pypdf-3.9.0/setup.cfg` & `pypdf-3.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pypdf-3.9.0/PKG-INFO` & `pypdf-3.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypdf
-Version: 3.9.0
+Version: 3.9.1
 Summary: A pure-python PDF library capable of splitting, merging, cropping, and transforming PDF files
 Author-email: Mathieu Fenniak <biziqe@mathieu.fenniak.net>
 Maintainer-email: Martin Thoma <info@martin-thoma.de>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

