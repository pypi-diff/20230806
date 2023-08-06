# Comparing `tmp/tcia_utils-1.6.1.tar.gz` & `tmp/tcia_utils-1.6.2.tar.gz`

## Comparing `tcia_utils-1.6.1.tar` & `tcia_utils-1.6.2.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 tcia_utils-1.6.1/src/tcia_utils/__init__.py
--rw-r--r--   0        0        0     6773 2020-02-02 00:00:00.000000 tcia_utils-1.6.1/src/tcia_utils/datacite.py
--rw-r--r--   0        0        0    71871 2020-02-02 00:00:00.000000 tcia_utils-1.6.1/src/tcia_utils/nbia.py
--rw-r--r--   0        0        0     4947 2020-02-02 00:00:00.000000 tcia_utils-1.6.1/src/tcia_utils/pathdb.py
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 tcia_utils-1.6.1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 tcia_utils-1.6.1/LICENSE
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 tcia_utils-1.6.1/README.md
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 tcia_utils-1.6.1/pyproject.toml
--rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 tcia_utils-1.6.1/PKG-INFO
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 tcia_utils-1.6.2/src/tcia_utils/__init__.py
+-rw-r--r--   0        0        0     6303 2020-02-02 00:00:00.000000 tcia_utils-1.6.2/src/tcia_utils/datacite.py
+-rw-r--r--   0        0        0    72518 2020-02-02 00:00:00.000000 tcia_utils-1.6.2/src/tcia_utils/nbia.py
+-rw-r--r--   0        0        0     4947 2020-02-02 00:00:00.000000 tcia_utils-1.6.2/src/tcia_utils/pathdb.py
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 tcia_utils-1.6.2/src/tcia_utils/utils.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 tcia_utils-1.6.2/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 tcia_utils-1.6.2/LICENSE
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 tcia_utils-1.6.2/README.md
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 tcia_utils-1.6.2/pyproject.toml
+-rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 tcia_utils-1.6.2/PKG-INFO
```

### Comparing `tcia_utils-1.6.1/src/tcia_utils/datacite.py` & `tcia_utils-1.6.2/src/tcia_utils/datacite.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,58 +1,46 @@
 import pandas as pd
 import requests
 from datetime import datetime
 import logging
+from tcia_utils.utils import searchDf
 
 _log = logging.getLogger(__name__)
 logging.basicConfig(
     format='%(asctime)s:%(levelname)s:%(message)s'
     , level=logging.INFO
 )
 
-####### getDoi function
-# Gets metadata for one or more DOIs
-# Returns all TCIA DOIs if no parameters are specified
-# query parameter searches all metadata fields
-# created parameter expects a 4 digit year
-# license parameter requires an exact match. currently supported licenses:
-#    ['cc-by-3.0', 'cc-by-4.0', 'cc-by-nc-4.0', 'nctn data archive license',
-#    'tcia limited access license', 'cc-by-nc-3.0']
-# See https://support.datacite.org/docs/api-get-doi for more details
-
-def getDoi(query = "",
-           created = "",
-           license = "",
-           format = ""):
-
+def getDoi(format = ""):
+    """ 
+        Gets metadata for all TCIA DOIs.
+        Returns a dataframe by default, but format can be set to CSV or JSON.
+        See https://support.datacite.org/docs/api-get-doi for more details.
+    """
     datacite_url = "https://api.datacite.org/dois/"
     datacite_headers = {"accept": "application/vnd.api+json"}
     df = pd.DataFrame()
 
     # set query parameters
     options = {}
     options['provider-id'] = "tciar"
     options['page[size]'] = 1000
-    if query:
-        options['query'] = query
-    if created:
-        options['created'] = created
-    if license:
-        options['license'] = license
     _log.info(f'Calling... {datacite_url} with parameters {options}')
 
     try:
         data = requests.get(datacite_url, headers = datacite_headers, params = options)
         data.raise_for_status()
 
         # check for empty results and format output
         if data.text != "":
             data = data.json()
             # format the output (optional)
-            if format == "df" or format == "csv":
+            if format == "json":
+                return data
+            else:
                 dois = []
                 for item in data["data"]:
                     doi = item["id"]
                     try:
                         identifier = item["attributes"]["identifiers"][0]["identifier"]
                     except (KeyError, IndexError):
                         identifier = None
@@ -83,43 +71,42 @@
                         relation_type = None
                     try:
                         related_identifier = item["attributes"]["relatedIdentifiers"][0]["relatedIdentifier"]
                     except (KeyError, IndexError):
                         related_identifier = None
                     version = item["attributes"]["version"]
                     try:
-                        rights = item["attributes"]["rightsList"][0]["rights"]
+                        rights = item["attributes"]["rightsList"]
+                        rights_list = [r["rights"] for r in rights]
+                        rights_uri_list = [r["rightsUri"] for r in rights]
                     except (KeyError, IndexError):
-                        rights = None
-                    try:
-                        rights_uri = item["attributes"]["rightsList"][0]["rightsUri"]
-                    except (KeyError, IndexError):
-                        rights_uri = None
+                        rights_list = []
+                        rights_uri_list = []
                     try:
                         description = item["attributes"]["descriptions"][0]["description"]
                     except (KeyError, IndexError):
                         description = None
                     try:
                         funding_references = item["attributes"]["fundingReferences"]
                     except KeyError:
                         funding_references = None
                     url = item["attributes"]["url"]
                     citation_count = item["attributes"]["citationCount"]
                     reference_count = item["attributes"]["referenceCount"]
                     related = f"{relation_type}: {related_identifier}" if relation_type and related_identifier else None
                     dois.append({"DOI": doi, 
                                 "Identifier": identifier, 
-                                "CreatorNames": ", ".join(creator_names),
+                                "CreatorNames": "; ".join(creator_names),
                                 "Title": title, 
                                 "Created": created, 
                                 "Updated": updated, 
                                 "Related": related, 
                                 "Version": version, 
-                                "Rights": rights, 
-                                "RightsURI": rights_uri, 
+                                "Rights": "; ".join(rights_list),
+                                "RightsURI": "; ".join(rights_uri_list),
                                 "Description": description, 
                                 "FundingReferences": funding_references, 
                                 "URL": url, 
                                 "CitationCount": citation_count, 
                                 "ReferenceCount": reference_count})
 
                 df = pd.DataFrame(dois, columns=["DOI", "Identifier", "CreatorNames", "Title", "Created", "Updated", "Related", 
@@ -127,16 +114,14 @@
                                                   "CitationCount", "ReferenceCount"])  
                 if format == "csv":
                     now = datetime.now()
                     dt_string = now.strftime("%Y-%m-%d_%H%M")
                     df.to_csv('datacite_' + dt_string + '.csv')
                     _log.info(f"Report saved as datacite_{dt_string}.csv")
                 return df
-            else:
-                return data
         else:
             _log.info(f'No results found.')
             
     # handle errors
     except requests.exceptions.HTTPError as errh:
         _log.error(f'Error: {errh}')
     except requests.exceptions.ConnectionError as errc:
```

### Comparing `tcia_utils-1.6.1/src/tcia_utils/nbia.py` & `tcia_utils-1.6.2/src/tcia_utils/nbia.py`

 * *Files 1% similar despite different names*

```diff
@@ -1680,47 +1680,50 @@
 
     if slices[0].SeriesInstanceUID != result.referenced_series_uid:
         raise Exception("The selected reference series and the annotative series don't match!")
     
     colorPaleatte = ["blue", "orange", "green", "red", "cyan", "brown", "lime", "purple", "yellow", "pink", "olive"] 
     def seg_animation(x, **kwargs):
         plt.imshow(pixel_data[x], cmap = plt.cm.gray)
-        if reader == pydicom_seg.MultiClassReader():
-            mask_data = result.data
-            cmap = matplotlib.colors.ListedColormap(colorPaleatte[i])
-            plt.imshow(mask_data[x], cmap = cmap, alpha = 0.5*(mask_data[x] > 0), interpolation = None)
+        if isinstance(reader, pydicom_seg.reader.MultiClassReader):
+            if kwargs[list(kwargs)[0]] == True:
+                mask_data = result.data
+                plt.imshow(mask_data[x], cmap = plt.cm.rainbow, alpha = 0.5*(mask_data[x] > 0), interpolation = None)
         else:
             for i in result.available_segments:
                 if kwargs[list(kwargs)[i-1]] == True:
                     mask_data = result.segment_data(i)
                     cmap = matplotlib.colors.ListedColormap(colorPaleatte[i])
                     plt.imshow(mask_data[x], cmap = cmap, alpha = 0.5*(mask_data[x] > 0), interpolation = None)
         plt.axis('scaled')
         plt.show()
 
-    if reader == pydicom_seg.MultiClassReader():
-        interact(seg_animation, x=(0, len(pixel_data)-1))
+    if isinstance(reader, pydicom_seg.reader.MultiClassReader):
+        kwargs = {"Show Segments": True}
+        interact(seg_animation, x=(0, len(pixel_data)-1), **kwargs)
     else:
         kwargs = {v.SegmentDescription:True for i, v in enumerate(SEG_data.SegmentSequence)}
         interact(seg_animation, x=(0, len(pixel_data)-1), **kwargs)
 
 
 ####### viewSeriesRT function
 # Visualizes a Series (scan) you've downloaded in the notebook
 # Adds an overlay from the RTSTRUCT series
 # Requires a path parameter for the reference series
 # Requires the file path for the annotative series
+# Currenly not able to visualize seed points
 # Not recommended to be used as a standalone function
 def viewSeriesRT(seriesPath = "", RTPath = ""):
     import rt_utils 
     """
     Visualizes a Series (scan) you've downloaded in the notebook
     Adds an overlay from the RTSTRUCT series
     Requires a path parameter for the reference series
     Requires the file path for the annotative series
+    Currenly not able to visualize seed points
     Not recommended to be used as a standalone function
     """
     rtstruct = rt_utils.RTStructBuilder.create_from(seriesPath, RTPath)
     roi_names = rtstruct.get_roi_names()
     
     slices = rtstruct.series_data
     try:
@@ -1749,17 +1752,28 @@
 
     pixel_data = np.array(image, dtype=np.int16)
     colorPaleatte = ["blue", "orange", "green", "red", "cyan", "brown", "lime", "purple", "yellow", "pink", "olive"] 
     def rt_animation(x, **kwargs):
         plt.imshow(pixel_data[x], cmap = plt.cm.gray, interpolation = None)
         for i in range(len(roi_names)):
             if kwargs[roi_names[i]] == True:
-                mask_data = rtstruct.get_roi_mask_by_name(roi_names[i])
-                cmap = matplotlib.colors.ListedColormap(colorPaleatte[i])
-                plt.imshow(mask_data[:, :, x], cmap = cmap, alpha = 0.5*(mask_data[:, :, x] > 0), interpolation = None)
+                try:
+                    mask_data = rtstruct.get_roi_mask_by_name(roi_names[i])
+                    cmap = matplotlib.colors.ListedColormap(colorPaleatte[i])
+                    plt.imshow(mask_data[:, :, x], cmap = cmap, alpha = 0.5*(mask_data[:, :, x] > 0), interpolation = None)
+                except Exception as e:
+                    try:
+                        if e.code == -215:
+                            _log.error(f"\nThe ROI '{roi_names[i]}' contains seed point(s), which is currently not supported.")
+                        else:
+                            _log.error(f"\n{e}")
+                        pass
+                    except:
+                        _log.error(f"\n{e}")
+                        pass
         plt.axis('scaled')
         plt.show()
     
     kwargs = {v: True for i, v in enumerate(roi_names)}
     interact(rt_animation, x = (0, len(pixel_data)-1), **kwargs)
```

### Comparing `tcia_utils-1.6.1/src/tcia_utils/pathdb.py` & `tcia_utils-1.6.2/src/tcia_utils/pathdb.py`

 * *Files identical despite different names*

### Comparing `tcia_utils-1.6.1/.gitignore` & `tcia_utils-1.6.2/.gitignore`

 * *Files identical despite different names*

### Comparing `tcia_utils-1.6.1/LICENSE` & `tcia_utils-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tcia_utils-1.6.1/README.md` & `tcia_utils-1.6.2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # Overview
 The [tcia_utils](https://pypi.org/project/tcia-utils/) package contains functions to simplify common tasks one might perform when interacting with The Cancer Imaging Archive (TCIA) via Jupyter/Python. Learn more about TCIA and its open-access datasets at https://www.cancerimagingarchive.net/.  Please be sure to comply with the [TCIA Data Usage Policy](https://wiki.cancerimagingarchive.net/x/c4hF).
 
+[![Downloads](https://static.pepy.tech/personalized-badge/tcia-utils?period=month&units=international_system&left_color=blue&right_color=grey&left_text=Downloads%20/%20Month)](https://pepy.tech/project/tcia-utils)
+
 # Installation
 ```
 pip install tcia_utils
 ```
 
 # Usage
```

### Comparing `tcia_utils-1.6.1/pyproject.toml` & `tcia_utils-1.6.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "tcia_utils"
-version = "1.6.1"
+version = "1.6.2"
 authors = [
   { name="Justin Kirby", email="justin.kirby@nih.gov" },
 ]
 description = "A package to simplify common tasks one might perform when interacting with The Cancer Imaging Archive (TCIA) via Jupyter/Python."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `tcia_utils-1.6.1/PKG-INFO` & `tcia_utils-1.6.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tcia_utils
-Version: 1.6.1
+Version: 1.6.2
 Summary: A package to simplify common tasks one might perform when interacting with The Cancer Imaging Archive (TCIA) via Jupyter/Python.
 Project-URL: Homepage, https://github.com/kirbyju/tcia_utils
 Project-URL: Bug Tracker, https://github.com/kirbyju/tcia_utils/issues
 Author-email: Justin Kirby <justin.kirby@nih.gov>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -19,14 +19,16 @@
 Requires-Dist: requests
 Requires-Dist: rt-utils
 Description-Content-Type: text/markdown
 
 # Overview
 The [tcia_utils](https://pypi.org/project/tcia-utils/) package contains functions to simplify common tasks one might perform when interacting with The Cancer Imaging Archive (TCIA) via Jupyter/Python. Learn more about TCIA and its open-access datasets at https://www.cancerimagingarchive.net/.  Please be sure to comply with the [TCIA Data Usage Policy](https://wiki.cancerimagingarchive.net/x/c4hF).
 
+[![Downloads](https://static.pepy.tech/personalized-badge/tcia-utils?period=month&units=international_system&left_color=blue&right_color=grey&left_text=Downloads%20/%20Month)](https://pepy.tech/project/tcia-utils)
+
 # Installation
 ```
 pip install tcia_utils
 ```
 
 # Usage
```

