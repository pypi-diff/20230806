# Comparing `tmp/pih-mio-1.48027.tar.gz` & `tmp/pih-mio-1.48028.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-mio-1.48027.tar", last modified: Sat Aug  5 01:23:08 2023, max compression
+gzip compressed data, was "pih-mio-1.48028.tar", last modified: Sat Aug  5 14:22:39 2023, max compression
```

## Comparing `pih-mio-1.48027.tar` & `pih-mio-1.48028.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-08-05 01:23:08.316552 pih-mio-1.48027/
-drwxrwxrwx   0        0        0        0 2023-08-05 01:23:08.550935 pih-mio-1.48027/MobileHelperCore/
--rw-rw-rw-   0        0        0        0 2023-03-23 02:22:16.000000 pih-mio-1.48027/MobileHelperCore/__init__.py
--rw-rw-rw-   0        0        0      158 2023-07-28 13:41:38.000000 pih-mio-1.48027/MobileHelperCore/__main__.py
--rw-rw-rw-   0        0        0   168458 2023-08-05 01:21:48.000000 pih-mio-1.48027/MobileHelperCore/api.py
--rw-rw-rw-   0        0        0      718 2023-07-28 13:36:37.000000 pih-mio-1.48027/MobileHelperCore/service.py
--rw-rw-rw-   0        0        0     9589 2023-08-05 00:19:42.000000 pih-mio-1.48027/MobileHelperCore/service_api.py
--rw-rw-rw-   0        0        0      986 2023-06-21 05:38:40.000000 pih-mio-1.48027/MobileHelperCore/tools.py
--rw-rw-rw-   0        0        0      279 2023-08-05 01:23:08.790007 pih-mio-1.48027/PKG-INFO
--rw-rw-rw-   0        0        0     1651 2023-08-03 07:25:38.000000 pih-mio-1.48027/pih-mio_setup.py
-drwxrwxrwx   0        0        0        0 2023-08-05 01:23:08.754044 pih-mio-1.48027/pih_mio.egg-info/
--rw-rw-rw-   0        0        0      279 2023-08-05 01:23:07.000000 pih-mio-1.48027/pih_mio.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      372 2023-08-05 01:23:08.000000 pih-mio-1.48027/pih_mio.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-05 01:23:07.000000 pih-mio-1.48027/pih_mio.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-08-05 01:23:07.000000 pih-mio-1.48027/pih_mio.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       20 2023-08-05 01:23:07.000000 pih-mio-1.48027/pih_mio.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-08-05 01:23:07.000000 pih-mio-1.48027/pih_mio.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-05 01:23:08.800922 pih-mio-1.48027/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-05 14:22:39.136757 pih-mio-1.48028/
+drwxrwxrwx   0        0        0        0 2023-08-05 14:22:39.183637 pih-mio-1.48028/MobileHelperService/
+-rw-rw-rw-   0        0        0        0 2023-03-23 02:22:16.000000 pih-mio-1.48028/MobileHelperService/__init__.py
+-rw-rw-rw-   0        0        0      161 2023-08-05 09:47:04.000000 pih-mio-1.48028/MobileHelperService/__main__.py
+-rw-rw-rw-   0        0        0   168461 2023-08-05 14:21:36.000000 pih-mio-1.48028/MobileHelperService/api.py
+-rw-rw-rw-   0        0        0      721 2023-08-05 09:47:04.000000 pih-mio-1.48028/MobileHelperService/service.py
+-rw-rw-rw-   0        0        0     9592 2023-08-05 09:47:04.000000 pih-mio-1.48028/MobileHelperService/service_api.py
+-rw-rw-rw-   0        0        0      989 2023-08-05 09:47:04.000000 pih-mio-1.48028/MobileHelperService/tools.py
+-rw-rw-rw-   0        0        0      279 2023-08-05 14:22:39.683623 pih-mio-1.48028/PKG-INFO
+-rw-rw-rw-   0        0        0     1658 2023-08-05 09:44:51.000000 pih-mio-1.48028/pih-mio_setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 14:22:39.652377 pih-mio-1.48028/pih_mio.egg-info/
+-rw-rw-rw-   0        0        0      279 2023-08-05 14:22:38.000000 pih-mio-1.48028/pih_mio.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      390 2023-08-05 14:22:38.000000 pih-mio-1.48028/pih_mio.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 14:22:38.000000 pih-mio-1.48028/pih_mio.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-08-05 14:22:38.000000 pih-mio-1.48028/pih_mio.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       20 2023-08-05 14:22:38.000000 pih-mio-1.48028/pih_mio.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-08-05 14:22:38.000000 pih-mio-1.48028/pih_mio.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-05 14:22:39.699461 pih-mio-1.48028/setup.cfg
```

### Comparing `pih-mio-1.48027/MobileHelperCore/api.py` & `pih-mio-1.48028/MobileHelperService/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 from MobileHelperContent.content import MEDIA_CONTENT
 import requests
 from io import BytesIO
 
 class MIO:
 
     NAME: str = "mio"       
-    VERSION: str = "1.48027"  
+    VERSION: str = "1.48028"  
 
 class InternalInterrupt(Exception):
 
     @property
     def type(self) -> int:
         return self.args[0]
 
@@ -1309,15 +1309,15 @@
         section_list = section_list or CheckableSections.all()
         self.console_apps_api.resources_and_indications_check(section_list, False, self.is_forced, all)
 
     def register_ct_indications_handler(self) -> None:
         self.console_apps_api.register_ct_indications()
 
     def create_polibase_db_backup_handler(self) -> None:
-        from PolibaseDBCore.api import PolibaseDBApi
+        from PolibaseDBService.api import PolibaseDBApi
         dump_name: str = PolibaseDBApi.get_default_name()
         answer: bool = self.input.yes_no(
             f"Изменить имя файла дампа базы данных", False, b("Отправьте имя"), f"Использовать имя: {b(dump_name)} - отправьте {A.CT.VISUAL.NUMBER_SYMBOLS[0]}")
         if A.A_P.DB.backup(self.input.answer if answer else dump_name):
             self.write_line(i(f"{self.user_given_name}, ожидайте уведовление об процессе создания бекапа база данных Polibase в telegram-группе {b('Backup Console')}"))
 
     def robocopy_job_run_handler(self) -> None:
```

### Comparing `pih-mio-1.48027/MobileHelperCore/service.py` & `pih-mio-1.48028/MobileHelperService/service.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import importlib.util
 
 pih_is_exists = importlib.util.find_spec("pih") is not None
 if not pih_is_exists:
     sys.path.append("//pih/facade")
 from pih import A
 
-from MobileHelperCore.service_api import MobileHelperService as Service, as_developer
+from MobileHelperService.service_api import MobileHelperService as Service, as_developer
 
 host: str = A.OS.host()
 
 def checker(telephone_number: str) -> bool:
     if not A.D_C.empty(A.SRV.get_support_host_list(A.CT_SR.MOBILE_HELPER)):
         am_i_tester: bool = A.D.is_not_none(A.CT.TEST.USER) and A.D_TN.by_login(A.CT.TEST.USER) == telephone_number
         if as_developer() or A.D.contains(host, A.CT_H.DEVELOPER.NAME):
```

### Comparing `pih-mio-1.48027/MobileHelperCore/service_api.py` & `pih-mio-1.48028/MobileHelperService/service_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
    
     sender_profile_id: A.CT_ME_WH_W.Profiles = A.ME_WH_W.get_profile_id(A.D_TN.it_administrator())
 
     if A.U.update_for_service(ROLE):
         from pih import PIH, Stdin, NotFound, SubscribtionResult
         from pih.tools import ParameterList, BitMask as BM
         from pih.collection import WhatsAppMessage, User
-        from MobileHelperCore.api import (MobileHelper as Api, MobileSession, MobileOutput, 
+        from MobileHelperService.api import (MobileHelper as Api, MobileSession, MobileOutput, 
                         MobileInput, MobileUserInput, MobileMarkInput, 
                         InternalInterrupt, AddressedInterruption, Flags)
         
         INIT = True
 
     mobile_helper_client_map: dict[str, Api] = {}
```

### Comparing `pih-mio-1.48027/MobileHelperCore/tools.py` & `pih-mio-1.48028/MobileHelperService/tools.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 pih_is_exists = importlib.util.find_spec("pih") is not None
 if not pih_is_exists:
     sys.path.append("//pih/facade")
 from pih import Output
 from PIL import Image
 import numpy as np
-from DocsCore.tools import Converter
+from DocsService.tools import Converter
 
 class Logger:
 
     def __init__(self,  logger: Output, log_level: int):
         self.output = logger
         self.level = log_level
```

### Comparing `pih-mio-1.48027/pih-mio_setup.py` & `pih-mio-1.48028/pih-mio_setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,47 +5,47 @@
 from setuptools import setup
 
 pih_is_exists = importlib.util.find_spec("pih") is not None
 if not pih_is_exists:
     sys.path.append("//pih/facade")
 from pih import A
 from pih.tools import j
-from MobileHelperCore.api import MIO
+from MobileHelperService.api import MIO
 
 #########################################################################################################
 """
 1. python mio_setup.py sdist --dist-dir mio_dist bdist_wheel --dist-dir mio_dist build --build-base pih_mio_build
 2. twine upload --repository pypi mio_dist/*
 3. pip install pih_mio -U
 """
 folder = "//pih/facade/pih-mio_dist"
 for filename in os.listdir(folder):
-    file_path = os.path.join(folder, filename)
+    file_path = A.PTH.join(folder, filename)
     try:
         if os.path.isfile(file_path) or os.path.islink(file_path):
             os.unlink(file_path)
         elif os.path.isdir(file_path):
             shutil.rmtree(file_path)
     except Exception as error:
         print("Failed to delete %s. Reason: %s" % (file_path, error))
 
 #This call to setup() does all the work
 name: str = j((A.root.NAME, MIO.NAME), "-")
 setup(
     name=name,
     entry_points={
         "console_scripts": [
-            f"{name}=MobileHelperCore.__main__:start",
+            f"{name}=MobileHelperService.__main__:start",
         ]
     },
     version=MIO.VERSION,
     description="PIH Mobile Helper library",
     long_description_content_type="text/markdown",
     url="https://pacifichosp.com/",
     author="Nikita Karachentsev",
     author_email="it@pacifichosp.com",
     license="MIT",
     classifiers=[],
-    packages=["MobileHelperCore"],
+    packages=["MobileHelperService"],
     include_package_data=True,
     install_requires=["pih", "pih-mio-content"]
 )
```

