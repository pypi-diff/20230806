# Comparing `tmp/pandasmemuc-0.14.tar.gz` & `tmp/pandasmemuc-0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasmemuc-0.14.tar", last modified: Fri Aug  4 06:17:24 2023, max compression
+gzip compressed data, was "pandasmemuc-0.15.tar", last modified: Sun Aug  6 04:54:42 2023, max compression
```

## Comparing `pandasmemuc-0.14.tar` & `pandasmemuc-0.15.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 06:17:24.452740 pandasmemuc-0.14/
--rw-rw-rw-   0        0        0     1148 2023-08-04 06:17:07.000000 pandasmemuc-0.14/LICENSE.rst
--rw-rw-rw-   0        0        0      104 2023-08-04 06:17:07.000000 pandasmemuc-0.14/MANIFEST.in
--rw-rw-rw-   0        0        0     2347 2023-08-04 06:17:24.453736 pandasmemuc-0.14/PKG-INFO
--rw-rw-rw-   0        0        0     1732 2023-07-30 22:20:11.000000 pandasmemuc-0.14/README.md
-drwxrwxrwx   0        0        0        0 2023-08-04 06:17:24.449748 pandasmemuc-0.14/pandasmemuc/
--rw-rw-rw-   0        0        0     1732 2023-07-30 22:20:11.000000 pandasmemuc-0.14/pandasmemuc/README.MD
--rw-rw-rw-   0        0        0   107576 2023-08-04 06:16:35.000000 pandasmemuc-0.14/pandasmemuc/__init__.py
--rw-rw-rw-   0        0        0      177 2023-08-04 06:17:23.000000 pandasmemuc-0.14/pandasmemuc/requirements.txt
--rw-rw-rw-   0        0        0    35393 2023-08-04 06:17:23.000000 pandasmemuc-0.14/pandasmemuc/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-08-04 06:17:24.452740 pandasmemuc-0.14/pandasmemuc.egg-info/
--rw-rw-rw-   0        0        0     2347 2023-08-04 06:17:24.000000 pandasmemuc-0.14/pandasmemuc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      329 2023-08-04 06:17:24.000000 pandasmemuc-0.14/pandasmemuc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 06:17:24.000000 pandasmemuc-0.14/pandasmemuc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      167 2023-08-04 06:17:24.000000 pandasmemuc-0.14/pandasmemuc.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-08-04 06:17:24.000000 pandasmemuc-0.14/pandasmemuc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2023-08-04 06:17:24.454734 pandasmemuc-0.14/setup.cfg
--rw-rw-rw-   0        0        0     1656 2023-08-04 06:17:23.000000 pandasmemuc-0.14/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-06 04:54:42.797895 pandasmemuc-0.15/
+-rw-rw-rw-   0        0        0     1148 2023-08-06 04:54:28.000000 pandasmemuc-0.15/LICENSE.rst
+-rw-rw-rw-   0        0        0      104 2023-08-06 04:54:27.000000 pandasmemuc-0.15/MANIFEST.in
+-rw-rw-rw-   0        0        0     2347 2023-08-06 04:54:42.797895 pandasmemuc-0.15/PKG-INFO
+-rw-rw-rw-   0        0        0     1732 2023-07-30 22:20:11.000000 pandasmemuc-0.15/README.md
+drwxrwxrwx   0        0        0        0 2023-08-06 04:54:42.792668 pandasmemuc-0.15/pandasmemuc/
+-rw-rw-rw-   0        0        0     1732 2023-07-30 22:20:11.000000 pandasmemuc-0.15/pandasmemuc/README.MD
+-rw-rw-rw-   0        0        0   108195 2023-08-06 04:53:17.000000 pandasmemuc-0.15/pandasmemuc/__init__.py
+-rw-rw-rw-   0        0        0      177 2023-08-06 04:54:41.000000 pandasmemuc-0.15/pandasmemuc/requirements.txt
+-rw-rw-rw-   0        0        0    35393 2023-08-06 04:54:41.000000 pandasmemuc-0.15/pandasmemuc/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-08-06 04:54:42.797149 pandasmemuc-0.15/pandasmemuc.egg-info/
+-rw-rw-rw-   0        0        0     2347 2023-08-06 04:54:42.000000 pandasmemuc-0.15/pandasmemuc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2023-08-06 04:54:42.000000 pandasmemuc-0.15/pandasmemuc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-06 04:54:42.000000 pandasmemuc-0.15/pandasmemuc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      167 2023-08-06 04:54:42.000000 pandasmemuc-0.15/pandasmemuc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-08-06 04:54:42.000000 pandasmemuc-0.15/pandasmemuc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-08-06 04:54:42.798642 pandasmemuc-0.15/setup.cfg
+-rw-rw-rw-   0        0        0     1656 2023-08-06 04:54:41.000000 pandasmemuc-0.15/setup.py
```

### Comparing `pandasmemuc-0.14/LICENSE.rst` & `pandasmemuc-0.15/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `pandasmemuc-0.14/PKG-INFO` & `pandasmemuc-0.15/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasmemuc
-Version: 0.14
+Version: 0.15
 Summary: Automating memu emulator with pandas
 Home-page: https://github.com/hansalemaos/pandasmemuc
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: memu,memnuc,pandas
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pandasmemuc-0.14/README.md` & `pandasmemuc-0.15/README.md`

 * *Files identical despite different names*

### Comparing `pandasmemuc-0.14/pandasmemuc/README.MD` & `pandasmemuc-0.15/pandasmemuc/README.MD`

 * *Files identical despite different names*

### Comparing `pandasmemuc-0.14/pandasmemuc/__init__.py` & `pandasmemuc-0.15/pandasmemuc/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3302,52 +3302,49 @@
         )
         self.change_config(0)
         return self
 
     def patch_hosts(
         self,
         vms_aa_index,
-        timeout=120,
+        timeout=60,
         addkillerlink="https://github.com/AdAway/AdAway/releases/download/v6.1.1/AdAway-6.1.1-20230620.apk",
     ):
         install_instance_patch_host(
             self, vms_aa_index, timeout=timeout, addkillerlink=addkillerlink
         )
         self.update_status()
         return self
 
     def change_config(self, i):
         self.df.iloc[i].set_enable_audio(0)
         try:
             sa = phoneconfig.phone_dataframe.sample(1)
 
-            self.df.iloc[i].set_linenum(sa.phone_number.iloc[0])
-            self.df.iloc[i].set_imei(sa.imei.iloc[0])
-            self.df.iloc[i].set_imsi(sa.cc_imsi.iloc[0])
-            self.df.iloc[i].set_simserial(sa.cc_simerial.iloc[0])
+            self.iloc[i].set_memory(sa.iloc[0].aa_ram_totalmem)
+            self.iloc[i].set_resolution_width(sa.iloc[0].aa_width)
+            self.iloc[i].set_resolution_height(sa.iloc[0].aa_height)
+            self.iloc[i].set_vbox_dpi(sa.iloc[0].aa_screen_densities)
+            self.iloc[i].set_linenum(f'+{sa.iloc[0].cc_phone_number}')
+            self.iloc[i].set_imei(sa.iloc[0].cc_imei)
+            self.iloc[i].set_imsi(sa.iloc[0].cc_imsi)
+            self.iloc[i].set_simserial(sa.iloc[0].cc_iccid)
+            self.iloc[i].set_microvirt_vm_brand(sa.iloc[0].aa_brand)
+            self.iloc[i].set_microvirt_vm_manufacturer(sa.iloc[0].aa_manufacturer)
+            self.iloc[i].set_microvirt_vm_model(" ".join(sa.iloc[0].aa_model_name.split()))
+            self.iloc[i].modifyvm_macaddress(
+                1,
+                (
+                        sa.iloc[0].cc_macaddress
+                ).replace(":", ""),
+            )
+
         except Exception:
             pass
 
-        self.df.modifyvm_macaddress.iloc[0](
-            1,
-            (
-                str(phoneconfig.mac_address_prefix)
-                + ":%02x:%02x:%02x" % tuple(random.randint(0, 255) for v in range(3))
-            ).replace(":", ""),
-        )
-
-        self.df.modifyvm_macaddress.iloc[0](
-            2,
-            (
-                str(phoneconfig.mac_address_prefix)
-                + ":%02x:%02x:%02x" % tuple(random.randint(0, 255) for v in range(3))
-            ).replace(":", ""),
-        )
-        self.df.iloc[i].set_enable_su(0)
-
         self.df = get_all_config(list_all_emulators())
         return self
 
     def update_status(self):
         self.df = get_all_config(list_all_emulators())
         return self
 
@@ -3371,14 +3368,25 @@
         self._create_vm(v="90", timeout=timeout)
         return self
 
     def create_vm_96(self, timeout=120):
         self._create_vm(v="96", timeout=timeout)
         return self
 
+    def create_vm_96_and_patch(self, timeout=120):
+        oldones = set(self.df.aa_index.to_list())
+        self._create_vm(v="96", timeout=timeout)
+        machinelist=self.df.aa_index.to_list()
+        aindex=list(set(machinelist) - oldones)[0]
+        self.patch_hosts([aindex])
+        iindex=self.df.loc[self.df.aa_index == aindex].index[0]
+        self.df.loc[self.df.aa_index == aindex].bb_stop.iloc[0]()
+        self.change_config(iindex)
+        return self
+
     def get_ui_automator_df(
         self,
         i,
         screenshotfolder=None,
         save_screenshot=False,
         max_variation_percent_x=10,
         max_variation_percent_y=10,
```

### Comparing `pandasmemuc-0.14/pandasmemuc/thirdparty.json` & `pandasmemuc-0.15/pandasmemuc/thirdparty.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9895833333333334%*

 * *Differences: {'3': "{'Version': '0.25'}"}*

```diff
@@ -17,15 +17,15 @@
         "Name": "a-pandas-ex-xml2df",
         "Version": "0.13"
     },
     {
         "License": "MIT",
         "LicenseText": "\n\n The MIT License (MIT)\n\n Copyright (c) 2023 Johannes Fischer\n\n \n\n Permission is hereby granted, free of charge, to any person obtaining a copy\n\n of this software and associated documentation files (the \"Software\"), to deal\n\n in the Software without restriction, including without limitation the rights\n\n to use, copy, modify, merge, publish, distribute, sublicense, and/or sell\n\n copies of the Software, and to permit persons to whom the Software is\n\n furnished to do so, subject to the following conditions:\n\n \n\n The above copyright notice and this permission notice shall be included in all\n\n copies or substantial portions of the Software.\n\n \n\n THE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND,\n\n EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\n\n MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\n\n IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,\n\n DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR\n\n OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE\n\n OR OTHER DEALINGS IN THE SOFTWARE.\n\n\n\n",
         "Name": "adbkit",
-        "Version": "0.24"
+        "Version": "0.25"
     },
     {
         "License": "MIT",
         "LicenseText": "\n\n The MIT License (MIT)\n\n Copyright (c) 2022 Johannes Fischer\n\n \n\n Permission is hereby granted, free of charge, to any person obtaining a copy\n\n of this software and associated documentation files (the \"Software\"), to deal\n\n in the Software without restriction, including without limitation the rights\n\n to use, copy, modify, merge, publish, distribute, sublicense, and/or sell\n\n copies of the Software, and to permit persons to whom the Software is\n\n furnished to do so, subject to the following conditions:\n\n \n\n The above copyright notice and this permission notice shall be included in all\n\n copies or substantial portions of the Software.\n\n \n\n THE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND,\n\n EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\n\n MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\n\n IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,\n\n DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR\n\n OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE\n\n OR OTHER DEALINGS IN THE SOFTWARE.\n\n\n\n",
         "Name": "flexible-partial",
         "Version": "0.12"
     },
```

### Comparing `pandasmemuc-0.14/pandasmemuc.egg-info/PKG-INFO` & `pandasmemuc-0.15/pandasmemuc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasmemuc
-Version: 0.14
+Version: 0.15
 Summary: Automating memu emulator with pandas
 Home-page: https://github.com/hansalemaos/pandasmemuc
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: memu,memnuc,pandas
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pandasmemuc-0.14/setup.py` & `pandasmemuc-0.15/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 with open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()\
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 #long_description = (this_directory / "README.md").read_text()
 
-VERSION = '''0.14'''
+VERSION = '''0.15'''
 DESCRIPTION = '''Automating memu emulator with pandas'''
 
 # Setting up
 setup(
     name="pandasmemuc",
     version=VERSION,
     license='MIT',
```

