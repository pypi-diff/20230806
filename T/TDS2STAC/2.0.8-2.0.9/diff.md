# Comparing `tmp/TDS2STAC-2.0.8.tar.gz` & `tmp/TDS2STAC-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TDS2STAC-2.0.8.tar", last modified: Fri Jul 21 17:38:45 2023, max compression
+gzip compressed data, was "TDS2STAC-2.0.9.tar", last modified: Sat Jul 22 16:07:11 2023, max compression
```

## Comparing `TDS2STAC-2.0.8.tar` & `TDS2STAC-2.0.9.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 hadizadeh-m (15144)      901        0 2023-07-21 17:38:45.948110 TDS2STAC-2.0.8/
--rw-r--r--   0 hadizadeh-m (15144)      901      168 2023-07-21 09:18:37.000000 TDS2STAC-2.0.8/AUTHORS.rst
--rw-r--r--   0 hadizadeh-m (15144)      901     3603 2023-07-21 09:18:37.000000 TDS2STAC-2.0.8/CONTRIBUTING.rst
--rw-r--r--   0 hadizadeh-m (15144)      901    13807 2023-07-21 09:18:37.000000 TDS2STAC-2.0.8/LICENSE
--rw-r--r--   0 hadizadeh-m (15144)      901      389 2023-07-21 09:18:37.000000 TDS2STAC-2.0.8/MANIFEST.in
--rw-r--r--   0 hadizadeh-m (15144)      901    10810 2023-07-21 17:38:45.948222 TDS2STAC-2.0.8/PKG-INFO
--rw-r--r--   0 hadizadeh-m (15144)      901     9403 2023-07-21 09:18:37.000000 TDS2STAC-2.0.8/README.rst
-drwxr-xr-x   0 hadizadeh-m (15144)      901        0 2023-07-21 17:38:45.944575 TDS2STAC-2.0.8/TDS2STAC.egg-info/
--rw-r--r--   0 hadizadeh-m (15144)      901    10810 2023-07-21 17:38:45.000000 TDS2STAC-2.0.8/TDS2STAC.egg-info/PKG-INFO
--rw-r--r--   0 hadizadeh-m (15144)      901      624 2023-07-21 17:38:45.000000 TDS2STAC-2.0.8/TDS2STAC.egg-info/SOURCES.txt
--rw-r--r--   0 hadizadeh-m (15144)      901        1 2023-07-21 17:38:45.000000 TDS2STAC-2.0.8/TDS2STAC.egg-info/dependency_links.txt
--rw-r--r--   0 hadizadeh-m (15144)      901      553 2023-07-21 17:38:45.000000 TDS2STAC-2.0.8/TDS2STAC.egg-info/requires.txt
--rw-r--r--   0 hadizadeh-m (15144)      901        9 2023-07-21 17:38:45.000000 TDS2STAC-2.0.8/TDS2STAC.egg-info/top_level.txt
-drwxr-xr-x   0 hadizadeh-m (15144)      901        0 2023-07-21 17:38:45.946355 TDS2STAC-2.0.8/docs/
--rw-r--r--   0 hadizadeh-m (15144)      901      609 2023-07-21 09:18:37.000000 TDS2STAC-2.0.8/docs/Makefile
--rw-r--r--   0 hadizadeh-m (15144)      901       28 2023-07-21 09:18:37.000000 TDS2STAC-2.0.8/docs/authors.rst
--rwxr-xr-x   0 hadizadeh-m (15144)      901     4870 2023-07-21 09:18:37.000000 TDS2STAC-2.0.8/docs/conf.py
--rw-r--r--   0 hadizadeh-m (15144)      901       33 2023-07-21 09:18:37.000000 TDS2STAC-2.0.8/docs/contributing.rst
--rw-r--r--   0 hadizadeh-m (15144)      901       28 2023-07-21 09:18:37.000000 TDS2STAC-2.0.8/docs/history.rst
--rw-r--r--   0 hadizadeh-m (15144)      901      296 2023-07-21 09:18:37.000000 TDS2STAC-2.0.8/docs/index.rst
--rw-r--r--   0 hadizadeh-m (15144)      901     1174 2023-07-21 09:18:37.000000 TDS2STAC-2.0.8/docs/installation.rst
--rw-r--r--   0 hadizadeh-m (15144)      901      806 2023-07-21 09:18:37.000000 TDS2STAC-2.0.8/docs/make.bat
--rw-r--r--   0 hadizadeh-m (15144)      901       27 2023-07-21 09:18:37.000000 TDS2STAC-2.0.8/docs/readme.rst
--rw-r--r--   0 hadizadeh-m (15144)      901       71 2023-07-21 09:18:37.000000 TDS2STAC-2.0.8/docs/usage.rst
--rw-r--r--   0 hadizadeh-m (15144)      901      181 2023-07-21 09:18:37.000000 TDS2STAC-2.0.8/pyproject.toml
--rw-r--r--   0 hadizadeh-m (15144)      901      227 2023-07-21 11:23:02.000000 TDS2STAC-2.0.8/requirements_dev.txt
--rw-r--r--   0 hadizadeh-m (15144)      901     1903 2023-07-21 17:38:45.948737 TDS2STAC-2.0.8/setup.cfg
--rw-r--r--   0 hadizadeh-m (15144)      901      427 2023-07-21 09:18:37.000000 TDS2STAC-2.0.8/setup.py
-drwxr-xr-x   0 hadizadeh-m (15144)      901        0 2023-07-21 17:38:45.948998 TDS2STAC-2.0.8/tds2stac/
--rw-r--r--   0 hadizadeh-m (15144)      901       99 2023-07-21 09:18:37.000000 TDS2STAC-2.0.8/tds2stac/__init__.py
--rw-r--r--   0 hadizadeh-m (15144)      901      497 2023-07-21 17:38:45.949040 TDS2STAC-2.0.8/tds2stac/_version.py
--rw-r--r--   0 hadizadeh-m (15144)      901    59101 2023-07-21 17:37:19.000000 TDS2STAC-2.0.8/tds2stac/app.py
--rw-r--r--   0 hadizadeh-m (15144)      901     2579 2023-07-21 09:18:37.000000 TDS2STAC-2.0.8/tds2stac/cli.py
--rw-r--r--   0 hadizadeh-m (15144)      901     3286 2023-07-21 09:18:37.000000 TDS2STAC-2.0.8/tds2stac/constants.py
--rw-r--r--   0 hadizadeh-m (15144)      901     7868 2023-07-21 09:18:37.000000 TDS2STAC-2.0.8/tds2stac/core.py
--rw-r--r--   0 hadizadeh-m (15144)      901     3696 2023-07-21 09:18:37.000000 TDS2STAC-2.0.8/tds2stac/utils.py
-drwxr-xr-x   0 hadizadeh-m (15144)      901        0 2023-07-21 17:38:45.947960 TDS2STAC-2.0.8/tests/
--rw-r--r--   0 hadizadeh-m (15144)      901       38 2023-07-21 09:18:37.000000 TDS2STAC-2.0.8/tests/__init__.py
--rw-r--r--   0 hadizadeh-m (15144)      901     1828 2023-07-21 09:18:37.000000 TDS2STAC-2.0.8/tests/test_tds2stac.py
--rw-r--r--   0 hadizadeh-m (15144)      901    84134 2023-07-21 09:18:37.000000 TDS2STAC-2.0.8/versioneer.py
+drwxr-xr-x   0 hadizadeh-m (15144)      901        0 2023-07-22 16:07:11.315666 TDS2STAC-2.0.9/
+-rw-r--r--   0 hadizadeh-m (15144)      901      168 2023-07-22 10:24:27.000000 TDS2STAC-2.0.9/AUTHORS.rst
+-rw-r--r--   0 hadizadeh-m (15144)      901     3603 2023-07-22 10:24:27.000000 TDS2STAC-2.0.9/CONTRIBUTING.rst
+-rw-r--r--   0 hadizadeh-m (15144)      901    13807 2023-07-22 10:24:27.000000 TDS2STAC-2.0.9/LICENSE
+-rw-r--r--   0 hadizadeh-m (15144)      901      389 2023-07-22 10:24:27.000000 TDS2STAC-2.0.9/MANIFEST.in
+-rw-r--r--   0 hadizadeh-m (15144)      901    10810 2023-07-22 16:07:11.315769 TDS2STAC-2.0.9/PKG-INFO
+-rw-r--r--   0 hadizadeh-m (15144)      901     9403 2023-07-22 10:24:27.000000 TDS2STAC-2.0.9/README.rst
+drwxr-xr-x   0 hadizadeh-m (15144)      901        0 2023-07-22 16:07:11.311636 TDS2STAC-2.0.9/TDS2STAC.egg-info/
+-rw-r--r--   0 hadizadeh-m (15144)      901    10810 2023-07-22 16:07:11.000000 TDS2STAC-2.0.9/TDS2STAC.egg-info/PKG-INFO
+-rw-r--r--   0 hadizadeh-m (15144)      901      624 2023-07-22 16:07:11.000000 TDS2STAC-2.0.9/TDS2STAC.egg-info/SOURCES.txt
+-rw-r--r--   0 hadizadeh-m (15144)      901        1 2023-07-22 16:07:11.000000 TDS2STAC-2.0.9/TDS2STAC.egg-info/dependency_links.txt
+-rw-r--r--   0 hadizadeh-m (15144)      901      553 2023-07-22 16:07:11.000000 TDS2STAC-2.0.9/TDS2STAC.egg-info/requires.txt
+-rw-r--r--   0 hadizadeh-m (15144)      901        9 2023-07-22 16:07:11.000000 TDS2STAC-2.0.9/TDS2STAC.egg-info/top_level.txt
+drwxr-xr-x   0 hadizadeh-m (15144)      901        0 2023-07-22 16:07:11.313509 TDS2STAC-2.0.9/docs/
+-rw-r--r--   0 hadizadeh-m (15144)      901      609 2023-07-22 10:24:27.000000 TDS2STAC-2.0.9/docs/Makefile
+-rw-r--r--   0 hadizadeh-m (15144)      901       28 2023-07-22 10:24:27.000000 TDS2STAC-2.0.9/docs/authors.rst
+-rwxr-xr-x   0 hadizadeh-m (15144)      901     4870 2023-07-22 10:24:27.000000 TDS2STAC-2.0.9/docs/conf.py
+-rw-r--r--   0 hadizadeh-m (15144)      901       33 2023-07-22 10:24:27.000000 TDS2STAC-2.0.9/docs/contributing.rst
+-rw-r--r--   0 hadizadeh-m (15144)      901       28 2023-07-22 10:24:27.000000 TDS2STAC-2.0.9/docs/history.rst
+-rw-r--r--   0 hadizadeh-m (15144)      901      296 2023-07-22 10:24:27.000000 TDS2STAC-2.0.9/docs/index.rst
+-rw-r--r--   0 hadizadeh-m (15144)      901     1174 2023-07-22 10:24:27.000000 TDS2STAC-2.0.9/docs/installation.rst
+-rw-r--r--   0 hadizadeh-m (15144)      901      806 2023-07-22 10:24:27.000000 TDS2STAC-2.0.9/docs/make.bat
+-rw-r--r--   0 hadizadeh-m (15144)      901       27 2023-07-22 10:24:27.000000 TDS2STAC-2.0.9/docs/readme.rst
+-rw-r--r--   0 hadizadeh-m (15144)      901       71 2023-07-22 10:24:27.000000 TDS2STAC-2.0.9/docs/usage.rst
+-rw-r--r--   0 hadizadeh-m (15144)      901      181 2023-07-22 10:24:27.000000 TDS2STAC-2.0.9/pyproject.toml
+-rw-r--r--   0 hadizadeh-m (15144)      901      227 2023-07-22 10:24:27.000000 TDS2STAC-2.0.9/requirements_dev.txt
+-rw-r--r--   0 hadizadeh-m (15144)      901     1903 2023-07-22 16:07:11.316248 TDS2STAC-2.0.9/setup.cfg
+-rw-r--r--   0 hadizadeh-m (15144)      901      427 2023-07-22 10:24:27.000000 TDS2STAC-2.0.9/setup.py
+drwxr-xr-x   0 hadizadeh-m (15144)      901        0 2023-07-22 16:07:11.316399 TDS2STAC-2.0.9/tds2stac/
+-rw-r--r--   0 hadizadeh-m (15144)      901       99 2023-07-22 10:24:27.000000 TDS2STAC-2.0.9/tds2stac/__init__.py
+-rw-r--r--   0 hadizadeh-m (15144)      901      497 2023-07-22 16:07:11.316432 TDS2STAC-2.0.9/tds2stac/_version.py
+-rw-r--r--   0 hadizadeh-m (15144)      901    59976 2023-07-22 16:04:59.000000 TDS2STAC-2.0.9/tds2stac/app.py
+-rw-r--r--   0 hadizadeh-m (15144)      901     2579 2023-07-22 10:24:27.000000 TDS2STAC-2.0.9/tds2stac/cli.py
+-rw-r--r--   0 hadizadeh-m (15144)      901     3286 2023-07-22 10:24:27.000000 TDS2STAC-2.0.9/tds2stac/constants.py
+-rw-r--r--   0 hadizadeh-m (15144)      901     7868 2023-07-22 10:24:27.000000 TDS2STAC-2.0.9/tds2stac/core.py
+-rw-r--r--   0 hadizadeh-m (15144)      901     3696 2023-07-22 10:24:27.000000 TDS2STAC-2.0.9/tds2stac/utils.py
+drwxr-xr-x   0 hadizadeh-m (15144)      901        0 2023-07-22 16:07:11.315533 TDS2STAC-2.0.9/tests/
+-rw-r--r--   0 hadizadeh-m (15144)      901       38 2023-07-22 10:24:27.000000 TDS2STAC-2.0.9/tests/__init__.py
+-rw-r--r--   0 hadizadeh-m (15144)      901     1828 2023-07-22 10:24:27.000000 TDS2STAC-2.0.9/tests/test_tds2stac.py
+-rw-r--r--   0 hadizadeh-m (15144)      901    84134 2023-07-22 10:24:27.000000 TDS2STAC-2.0.9/versioneer.py
```

### Comparing `TDS2STAC-2.0.8/CONTRIBUTING.rst` & `TDS2STAC-2.0.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `TDS2STAC-2.0.8/LICENSE` & `TDS2STAC-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `TDS2STAC-2.0.8/PKG-INFO` & `TDS2STAC-2.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TDS2STAC
-Version: 2.0.8
+Version: 2.0.9
 Summary: A STAC catalog creator from Thredds data server
 Home-page: https://codebase.helmholtz.cloud/CAT4KIT/tds2stac
 Author: Mostafa Hadizadeh
 Author-email: mostafa.hadizadeh@kit.edu
 License: EUPL-1.2
 Project-URL: Documentation, https://tds2stac.readthedocs.io/
 Project-URL: Source, https://codebase.helmholtz.cloud/CAT4KIT/tds2stac
```

### Comparing `TDS2STAC-2.0.8/README.rst` & `TDS2STAC-2.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `TDS2STAC-2.0.8/TDS2STAC.egg-info/PKG-INFO` & `TDS2STAC-2.0.9/TDS2STAC.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TDS2STAC
-Version: 2.0.8
+Version: 2.0.9
 Summary: A STAC catalog creator from Thredds data server
 Home-page: https://codebase.helmholtz.cloud/CAT4KIT/tds2stac
 Author: Mostafa Hadizadeh
 Author-email: mostafa.hadizadeh@kit.edu
 License: EUPL-1.2
 Project-URL: Documentation, https://tds2stac.readthedocs.io/
 Project-URL: Source, https://codebase.helmholtz.cloud/CAT4KIT/tds2stac
```

### Comparing `TDS2STAC-2.0.8/TDS2STAC.egg-info/SOURCES.txt` & `TDS2STAC-2.0.9/TDS2STAC.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TDS2STAC-2.0.8/TDS2STAC.egg-info/requires.txt` & `TDS2STAC-2.0.9/TDS2STAC.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `TDS2STAC-2.0.8/docs/Makefile` & `TDS2STAC-2.0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `TDS2STAC-2.0.8/docs/conf.py` & `TDS2STAC-2.0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `TDS2STAC-2.0.8/docs/installation.rst` & `TDS2STAC-2.0.9/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `TDS2STAC-2.0.8/docs/make.bat` & `TDS2STAC-2.0.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `TDS2STAC-2.0.8/setup.cfg` & `TDS2STAC-2.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `TDS2STAC-2.0.8/tds2stac/app.py` & `TDS2STAC-2.0.9/tds2stac/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -93,14 +93,15 @@
         httpHandler.setLevel(logging.DEBUG)
 
         self.logger.addHandler(httpHandler)
 
         xml_url_catalog, id_catalog, xml = utils.xml_processing(
             main_catalog_url
         )
+
         self.logger.info("Start Scanning datasets")
         print("Start Scanning datasets of %s" % xml_url_catalog)
 
         # This function displays a summary of datasets that are going to harvest
         Scanning = list(self.datasets_summary(xml_url_catalog, xml))
 
         # Writing description in the first step of scanning
@@ -198,14 +199,26 @@
             else:
                 self.aggregated_dataset_url = aggregated_dataset_url
             # All collections will be saved in the `urls` list
             urls = list(
                 self.datasets_harvester(xml_url_catalog, web_service, xml)
             )
             if len(urls) != 0:
+                ###############################################
+                # THE FOLLOWING LINE IS ADDED TO FIX ISSUE #75
+                ################################################
+                collections = list(self.catalog[id_catalog].get_collections())
+                for collection in collections:
+                    print(collection.id)
+                    if len(list(collection.get_all_items())) == 0:
+                        self.catalog[id_catalog].remove_child(collection.id)
+                    print(
+                        len(list(self.catalog[collection.id].get_all_items()))
+                    )
+
                 # Saving STAC catalog in the `stac_dir` directory
                 self.catalog[id_catalog].normalize_hrefs(
                     os.path.join(stac_dir, "stac")
                 )
                 self.catalog[id_catalog].save(
                     catalog_type=pystac.CatalogType.SELF_CONTAINED
                 )
@@ -243,14 +256,21 @@
         if url in self.scanned:
             self.logger.warning("Already Scanned %s " % url)
             # print("Already Scanned %s " % url)
             return
         self.scanned.append(url)
 
         url, catalog_colleciton_id, xml = utils.xml_processing(url)
+
+        ###############################################
+        # THE FOLLOWING LINE IS ADDED TO FIX ISSUE #75
+        ################################################
+
+        catalog_colleciton_id = self.id_catalog
+
         tree = etree.XML(xml_content)
 
         try:
             tree = etree.XML(xml_content)
         except BaseException:
             return
         # Finding datasets and consider each of them as a collection
@@ -284,15 +304,14 @@
                         self.catalog[collection_id] = pystac.Collection(
                             id=collection_id,
                             extent=pystac.Extent(spatial=None, temporal=None),
                             description="[Link to TDS]("
                             + utils.xml2html(url)
                             + ")",
                         )
-                        # self.catalog_all.add_child(self.catalog[convert_xml_x])
                         self.catalog[catalog_colleciton_id].add_child(
                             self.catalog[collection_id]
                         )
                     # it considers single data that is adjacent to other catalogRefs in main catalog as a single collection
                     elif "dataset" in str(c) and catalogRef_list != []:
                         branches_main.append(
                             url
@@ -315,15 +334,15 @@
                             + "?dataset="
                             + c.get("ID").replace("html", "xml")
                             + ")",
                         )
                         self.catalog[catalog_colleciton_id].add_child(
                             self.catalog[collection_id]
                         )
-                # when it harvests a dataset withou any catalogRef and sub-dataset
+                # when it harvests a dataset without any catalogRef and sub-dataset
                 if (
                     dataset_list != []
                     and catalogRef_list == []
                     and url == self.xml_url_catalog
                 ):
                     branches_main.append(utils.html2xml(url))
                     collection_id = utils.replacement_func(
@@ -354,14 +373,15 @@
                     + url.replace("xml", "html")
                     + ")",
                 )
 
                 self.catalog[catalog_colleciton_id].add_child(
                     self.catalog[collection_id]
                 )
+
         # Finding all data in datasets to create items
         data_main = []
         for e in branches_main:
             try:
                 url_stat = requests.get(e, None, verify=False)
                 content = url_stat.text.encode("utf-8")
             except BaseException:
@@ -1101,27 +1121,31 @@
                         ):
                             collection_item_id = (
                                 collection_item_id + " Aggregated"
                             )
 
                         # the condition below is for the case that the collection's id is not the same as the catalog's id
                         # Also it prevents the item to be added to the catalog separately without any connection to the collection
+
                         if collection_item_id != self.id_catalog:
                             self.catalog[
                                 collection_item_id
                             ].extent = pystac.Extent(
                                 spatial=spatial_extent,
                                 temporal=temporal_extent,
                             )
                             self.catalog[collection_item_id].add_item(item)
                 except Exception as e:
                     ex_type, ex_value, ex_traceback = sys.exc_info()
-                    print("Exception type : %s " % ex_type.__name__)
-                    print("Exception message : %s" % ex_value)
-                    self.logger.critical("%s : %s" % (ex_type.__name__, ex_value))
+                    # print("Exception type : %s " % ex_type.__name__)
+                    # print("Exception message : %s" % ex_value)
+                    # print(traceback.format_exc())
+                    self.logger.critical(
+                        "%s : %s" % (ex_type.__name__, ex_value)
+                    )
 
                     continue
 
             yield str(url) + "?dataset=" + str(elem.get("ID"))
         # When a collection doesn't have Spatial or Temporal extent
         if (
             type(self.catalog[catalog_colleciton_id])
```

### Comparing `TDS2STAC-2.0.8/tds2stac/cli.py` & `TDS2STAC-2.0.9/tds2stac/cli.py`

 * *Files identical despite different names*

### Comparing `TDS2STAC-2.0.8/tds2stac/constants.py` & `TDS2STAC-2.0.9/tds2stac/constants.py`

 * *Files identical despite different names*

### Comparing `TDS2STAC-2.0.8/tds2stac/core.py` & `TDS2STAC-2.0.9/tds2stac/core.py`

 * *Files identical despite different names*

### Comparing `TDS2STAC-2.0.8/tds2stac/utils.py` & `TDS2STAC-2.0.9/tds2stac/utils.py`

 * *Files identical despite different names*

### Comparing `TDS2STAC-2.0.8/tests/test_tds2stac.py` & `TDS2STAC-2.0.9/tests/test_tds2stac.py`

 * *Files identical despite different names*

### Comparing `TDS2STAC-2.0.8/versioneer.py` & `TDS2STAC-2.0.9/versioneer.py`

 * *Files identical despite different names*

