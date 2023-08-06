# Comparing `tmp/pyfireconsole-0.0.3.tar.gz` & `tmp/pyfireconsole-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfireconsole-0.0.3.tar", last modified: Fri Aug  4 09:52:26 2023, max compression
+gzip compressed data, was "pyfireconsole-0.0.4.tar", last modified: Sun Aug  6 14:41:57 2023, max compression
```

## Comparing `pyfireconsole-0.0.3.tar` & `pyfireconsole-0.0.4.tar`

### file list

```diff
@@ -1,31 +1,34 @@
-drwxr-xr-x   0 tanji      (501) staff       (20)        0 2023-08-04 09:52:26.830631 pyfireconsole-0.0.3/
--rw-r--r--   0 tanji      (501) staff       (20)     1069 2023-08-02 11:27:52.000000 pyfireconsole-0.0.3/LICENSE
--rw-r--r--   0 tanji      (501) staff       (20)     5880 2023-08-04 09:52:26.830449 pyfireconsole-0.0.3/PKG-INFO
--rw-r--r--   0 tanji      (501) staff       (20)     5366 2023-08-04 09:47:45.000000 pyfireconsole-0.0.3/README.md
-drwxr-xr-x   0 tanji      (501) staff       (20)        0 2023-08-04 09:52:26.826426 pyfireconsole-0.0.3/pyfireconsole/
--rw-r--r--   0 tanji      (501) staff       (20)      251 2023-08-04 09:47:45.000000 pyfireconsole-0.0.3/pyfireconsole/__init__.py
-drwxr-xr-x   0 tanji      (501) staff       (20)        0 2023-08-04 09:52:26.827908 pyfireconsole-0.0.3/pyfireconsole/console/
--rw-r--r--   0 tanji      (501) staff       (20)        0 2023-08-03 05:24:39.000000 pyfireconsole-0.0.3/pyfireconsole/console/__init__.py
--rw-r--r--   0 tanji      (501) staff       (20)     1797 2023-08-04 09:47:45.000000 pyfireconsole-0.0.3/pyfireconsole/console/pyfireconsole.py
-drwxr-xr-x   0 tanji      (501) staff       (20)        0 2023-08-04 09:52:26.828415 pyfireconsole-0.0.3/pyfireconsole/db/
--rw-r--r--   0 tanji      (501) staff       (20)        0 2023-08-02 11:34:51.000000 pyfireconsole-0.0.3/pyfireconsole/db/__init__.py
--rw-r--r--   0 tanji      (501) staff       (20)     1285 2023-08-04 09:47:45.000000 pyfireconsole-0.0.3/pyfireconsole/db/connection.py
-drwxr-xr-x   0 tanji      (501) staff       (20)        0 2023-08-04 09:52:26.828821 pyfireconsole-0.0.3/pyfireconsole/models/
--rw-r--r--   0 tanji      (501) staff       (20)        0 2023-08-02 11:34:51.000000 pyfireconsole-0.0.3/pyfireconsole/models/__init__.py
--rw-r--r--   0 tanji      (501) staff       (20)     5013 2023-08-04 09:47:45.000000 pyfireconsole-0.0.3/pyfireconsole/models/pyfire_model.py
-drwxr-xr-x   0 tanji      (501) staff       (20)        0 2023-08-04 09:52:26.830167 pyfireconsole-0.0.3/pyfireconsole/queries/
--rw-r--r--   0 tanji      (501) staff       (20)        0 2023-08-02 11:34:51.000000 pyfireconsole-0.0.3/pyfireconsole/queries/__init__.py
--rw-r--r--   0 tanji      (501) staff       (20)      959 2023-08-04 09:47:45.000000 pyfireconsole-0.0.3/pyfireconsole/queries/abstract_query.py
--rw-r--r--   0 tanji      (501) staff       (20)      371 2023-08-04 09:47:45.000000 pyfireconsole-0.0.3/pyfireconsole/queries/all_query.py
--rw-r--r--   0 tanji      (501) staff       (20)      540 2023-08-04 09:47:45.000000 pyfireconsole-0.0.3/pyfireconsole/queries/get_query.py
--rw-r--r--   0 tanji      (501) staff       (20)      768 2023-08-04 09:47:45.000000 pyfireconsole-0.0.3/pyfireconsole/queries/query_runner.py
--rw-r--r--   0 tanji      (501) staff       (20)      651 2023-08-04 09:47:45.000000 pyfireconsole-0.0.3/pyfireconsole/queries/where_query.py
-drwxr-xr-x   0 tanji      (501) staff       (20)        0 2023-08-04 09:52:26.827576 pyfireconsole-0.0.3/pyfireconsole.egg-info/
--rw-r--r--   0 tanji      (501) staff       (20)     5880 2023-08-04 09:52:26.000000 pyfireconsole-0.0.3/pyfireconsole.egg-info/PKG-INFO
--rw-r--r--   0 tanji      (501) staff       (20)      673 2023-08-04 09:52:26.000000 pyfireconsole-0.0.3/pyfireconsole.egg-info/SOURCES.txt
--rw-r--r--   0 tanji      (501) staff       (20)        1 2023-08-04 09:52:26.000000 pyfireconsole-0.0.3/pyfireconsole.egg-info/dependency_links.txt
--rw-r--r--   0 tanji      (501) staff       (20)      130 2023-08-04 09:52:26.000000 pyfireconsole-0.0.3/pyfireconsole.egg-info/requires.txt
--rw-r--r--   0 tanji      (501) staff       (20)       14 2023-08-04 09:52:26.000000 pyfireconsole-0.0.3/pyfireconsole.egg-info/top_level.txt
--rw-r--r--   0 tanji      (501) staff       (20)      520 2023-08-04 09:48:03.000000 pyfireconsole-0.0.3/pyproject.toml
--rw-r--r--   0 tanji      (501) staff       (20)       38 2023-08-04 09:52:26.830677 pyfireconsole-0.0.3/setup.cfg
--rw-r--r--   0 tanji      (501) staff       (20)      892 2023-08-04 09:49:06.000000 pyfireconsole-0.0.3/setup.py
+drwxr-xr-x   0 tanji      (501) staff       (20)        0 2023-08-06 14:41:57.950095 pyfireconsole-0.0.4/
+-rw-r--r--   0 tanji      (501) staff       (20)     1069 2023-08-02 11:27:52.000000 pyfireconsole-0.0.4/LICENSE
+-rw-r--r--   0 tanji      (501) staff       (20)     7020 2023-08-06 14:41:57.949901 pyfireconsole-0.0.4/PKG-INFO
+-rw-r--r--   0 tanji      (501) staff       (20)     6507 2023-08-06 14:40:20.000000 pyfireconsole-0.0.4/README.md
+drwxr-xr-x   0 tanji      (501) staff       (20)        0 2023-08-06 14:41:57.945366 pyfireconsole-0.0.4/pyfireconsole/
+-rw-r--r--   0 tanji      (501) staff       (20)      251 2023-08-04 09:47:45.000000 pyfireconsole-0.0.4/pyfireconsole/__init__.py
+drwxr-xr-x   0 tanji      (501) staff       (20)        0 2023-08-06 14:41:57.946534 pyfireconsole-0.0.4/pyfireconsole/console/
+-rw-r--r--   0 tanji      (501) staff       (20)        0 2023-08-03 05:24:39.000000 pyfireconsole-0.0.4/pyfireconsole/console/__init__.py
+-rw-r--r--   0 tanji      (501) staff       (20)     1797 2023-08-04 09:47:45.000000 pyfireconsole-0.0.4/pyfireconsole/console/pyfireconsole.py
+drwxr-xr-x   0 tanji      (501) staff       (20)        0 2023-08-06 14:41:57.946927 pyfireconsole-0.0.4/pyfireconsole/db/
+-rw-r--r--   0 tanji      (501) staff       (20)        0 2023-08-02 11:34:51.000000 pyfireconsole-0.0.4/pyfireconsole/db/__init__.py
+-rw-r--r--   0 tanji      (501) staff       (20)     1395 2023-08-06 14:01:12.000000 pyfireconsole-0.0.4/pyfireconsole/db/connection.py
+drwxr-xr-x   0 tanji      (501) staff       (20)        0 2023-08-06 14:41:57.947533 pyfireconsole-0.0.4/pyfireconsole/models/
+-rw-r--r--   0 tanji      (501) staff       (20)        0 2023-08-02 11:34:51.000000 pyfireconsole-0.0.4/pyfireconsole/models/__init__.py
+-rw-r--r--   0 tanji      (501) staff       (20)     3614 2023-08-06 14:01:12.000000 pyfireconsole-0.0.4/pyfireconsole/models/association.py
+-rw-r--r--   0 tanji      (501) staff       (20)     6859 2023-08-06 14:01:12.000000 pyfireconsole-0.0.4/pyfireconsole/models/pyfire_model.py
+drwxr-xr-x   0 tanji      (501) staff       (20)        0 2023-08-06 14:41:57.949549 pyfireconsole-0.0.4/pyfireconsole/queries/
+-rw-r--r--   0 tanji      (501) staff       (20)        0 2023-08-02 11:34:51.000000 pyfireconsole-0.0.4/pyfireconsole/queries/__init__.py
+-rw-r--r--   0 tanji      (501) staff       (20)      959 2023-08-04 13:15:42.000000 pyfireconsole-0.0.4/pyfireconsole/queries/abstract_query.py
+-rw-r--r--   0 tanji      (501) staff       (20)      374 2023-08-06 14:01:12.000000 pyfireconsole-0.0.4/pyfireconsole/queries/all_query.py
+-rw-r--r--   0 tanji      (501) staff       (20)      600 2023-08-06 14:01:12.000000 pyfireconsole-0.0.4/pyfireconsole/queries/get_query.py
+-rw-r--r--   0 tanji      (501) staff       (20)     1096 2023-08-06 14:01:12.000000 pyfireconsole-0.0.4/pyfireconsole/queries/query_runner.py
+-rw-r--r--   0 tanji      (501) staff       (20)      589 2023-08-06 14:01:12.000000 pyfireconsole-0.0.4/pyfireconsole/queries/save_query.py
+-rw-r--r--   0 tanji      (501) staff       (20)      290 2023-08-04 11:30:04.000000 pyfireconsole-0.0.4/pyfireconsole/queries/where_clouse.py
+-rw-r--r--   0 tanji      (501) staff       (20)      795 2023-08-06 14:01:12.000000 pyfireconsole-0.0.4/pyfireconsole/queries/where_query.py
+drwxr-xr-x   0 tanji      (501) staff       (20)        0 2023-08-06 14:41:57.946195 pyfireconsole-0.0.4/pyfireconsole.egg-info/
+-rw-r--r--   0 tanji      (501) staff       (20)     7020 2023-08-06 14:41:57.000000 pyfireconsole-0.0.4/pyfireconsole.egg-info/PKG-INFO
+-rw-r--r--   0 tanji      (501) staff       (20)      783 2023-08-06 14:41:57.000000 pyfireconsole-0.0.4/pyfireconsole.egg-info/SOURCES.txt
+-rw-r--r--   0 tanji      (501) staff       (20)        1 2023-08-06 14:41:57.000000 pyfireconsole-0.0.4/pyfireconsole.egg-info/dependency_links.txt
+-rw-r--r--   0 tanji      (501) staff       (20)      130 2023-08-06 14:41:57.000000 pyfireconsole-0.0.4/pyfireconsole.egg-info/requires.txt
+-rw-r--r--   0 tanji      (501) staff       (20)       14 2023-08-06 14:41:57.000000 pyfireconsole-0.0.4/pyfireconsole.egg-info/top_level.txt
+-rw-r--r--   0 tanji      (501) staff       (20)      678 2023-08-06 14:40:26.000000 pyfireconsole-0.0.4/pyproject.toml
+-rw-r--r--   0 tanji      (501) staff       (20)       38 2023-08-06 14:41:57.950154 pyfireconsole-0.0.4/setup.cfg
+-rw-r--r--   0 tanji      (501) staff       (20)      891 2023-08-06 14:40:27.000000 pyfireconsole-0.0.4/setup.py
```

### Comparing `pyfireconsole-0.0.3/LICENSE` & `pyfireconsole-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfireconsole-0.0.3/PKG-INFO` & `pyfireconsole-0.0.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,8 @@
-Metadata-Version: 2.1
-Name: pyfireconsole
-Version: 0.0.3
-Summary: An interactive console for Firestore based on Python ORM
-Home-page: https://github.com/tan-z-tan/pyfireconsole
-Author: Makoto Tanji
-Author-email: tanji.makoto@gmail.com
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.10.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
+[![Python package](https://github.com/tan-z-tan/PyFireConsole/actions/workflows/test.yml/badge.svg)](https://github.com/tan-z-tan/PyFireConsole/actions/workflows/test.yml)
 
 <h1 style="text-align: center;">
   <img src="https://raw.githubusercontent.com/tan-z-tan/pyfireconsole/main/logo.png" alt="PyFireConsole">
 </h1>
 
 ## Introduction
 Inspired by Rails console, PyFireConsole provides a seamless interface to Google's Firestore in Python, simplifying tasks such as connection, ORM, and data associations. It makes managing Firestore a breeze.
@@ -30,47 +17,71 @@
 pip install pyfireconsole
 ```
 
 ## Getting Started
 ```python
 from datetime import datetime
 from typing import Optional
-from pyfireconsole.models.pyfire_model import PyfireDoc, PyfireCollection, DocumentRef
+from pyfireconsole.models.association import belongs_to
+from pyfireconsole.models.pyfire_model import PyfireCollection, DocumentRef, PyfireDoc
 from pyfireconsole.db.connection import FirestoreConnection
 
-# Define your models 
+"""
+We assume that you have a firestore database with the following structure:
+- users Collection
+    - {user_id} Document
+        - name: str
+        - email: str
+- publishers Collection
+    - {publisher_id} Document
+        - name: str
+        - address: str
+- books Collection
+    - {book_id} Document
+        - title: str
+        - user_id: str
+        - published_at: datetime
+        - authors: list[str]
+        - tags: Sub Collection
+            - {tag_id} Document
+                - name: str
+        - publisher_ref: Reference
+"""
+
+
 class User(PyfireDoc):
     name: str
     email: str
 
 class Publisher(PyfireDoc):
     name: str
     address: Optional[str]
 
 class Tag(PyfireDoc):
     name: str
 
+
+@belongs_to(User, "user_id")
 class Book(PyfireDoc):
     title: str
     user_id: str
-    PyfireDoc.belongs_to(User)  # Make accessible via book.user
     published_at: datetime
     authors: list[str]
     tags: PyfireCollection[Tag] = PyfireCollection(Tag)
     publisher_ref: DocumentRef[Publisher]
 
 
 # Initialize FirestoreConnection using your default credentials of gcloud. (use `gcloud auth application-default login` or set GOOGLE_APPLICATION_CREDENTIALS)
 FirestoreConnection().initialize(project_id="YOUR-PROJECT-ID")
 
 # Or you can specify service_account_key_path
 # FirestoreConnection().initialize(service_account_key_path="./service-account.json", project_id="YOUR-PROJECT-ID")
 
 print("==================== find ====================")
-book = Book.find("12345")  # => Book
+book = Book.find("XlvQHeGi3cODbI4MQpI3")  # => Book
 print(book.model_dump())  # => dict
 print(f"ID: {book.id} | Title: {book.title} | Authors: {book.authors} | Published At: {book.published_at.isoformat()}")
 
 print("==================== belongs_to ====================")
 print(book.user)  # => User
 print(book.user.name)  # => str
 
@@ -110,48 +121,65 @@
 This feature is inspired by the Rails console.
 
 How to setup interactive console:
 
 ```python
 from datetime import datetime
 from typing import Optional
-from pyfireconsole.models.pyfire_model import PyfireDoc, PyfireCollection, DocumentRef
+from pyfireconsole.models.association import belongs_to, has_many, resolve_pyfire_model_names
+from pyfireconsole.models.pyfire_model import PyfireCollection, DocumentRef, PyfireDoc
 from pyfireconsole.db.connection import FirestoreConnection
 from pyfireconsole import PyFireConsole
 
+
+@has_many('Book', "user_id")
 class User(PyfireDoc):
     name: str
     email: str
 
+
 class Publisher(PyfireDoc):
     name: str
     address: Optional[str]
 
+
 class Tag(PyfireDoc):
     name: str
 
+
+@belongs_to(User, "user_id")
 class Book(PyfireDoc):
     title: str
     user_id: str
-    PyfireDoc.belongs_to(User)  # Make accessible via book.user
     published_at: datetime
     authors: list[str]
     tags: PyfireCollection[Tag] = PyfireCollection(Tag)
     publisher_ref: DocumentRef[Publisher]
 
-FirestoreConnection().initialize(project_id="YOUR-PROJECT-ID")
+# Resolve PyfireModel names
+# Call this function when you define your models by using str class name.
+# e.g. @has_many('Book', "user_id")
+resolve_pyfire_model_names(globals())
+
+
+FirestoreConnection().initialize(project_id="YOUR_PROJECT_ID")
 PyFireConsole().run()
 ```
 
 
 Alternatively, you can define your model files in `app/models/` and initialize the console as follows:
 
 ```python
 from pyfireconsole.db.connection import FirestoreConnection
 from pyfireconsole import PyFireConsole
+from pyfireconsole.models.association import resolve_pyfire_model_names
+
+# Resolve PyfireModel names
+resolve_pyfire_model_names(globals())
+
 
 FirestoreConnection().initialize(project_id="YOUR-PROJECT-ID")
 PyFireConsole(model_dir="app/models").run()
 ```
 
 Through the interactive console, you can conveniently test and experiment with your Firestore data models.
```

### Comparing `pyfireconsole-0.0.3/README.md` & `pyfireconsole-0.0.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: pyfireconsole
+Version: 0.0.4
+Summary: An interactive console for Firestore based on Python ORM
+Home-page: https://github.com/tan-z-tan/pyfireconsole
+Author: Makoto Tanji
+Author-email: tanji.makoto@gmail.com
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.8.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![Python package](https://github.com/tan-z-tan/PyFireConsole/actions/workflows/test.yml/badge.svg)](https://github.com/tan-z-tan/PyFireConsole/actions/workflows/test.yml)
+
 <h1 style="text-align: center;">
   <img src="https://raw.githubusercontent.com/tan-z-tan/pyfireconsole/main/logo.png" alt="PyFireConsole">
 </h1>
 
 ## Introduction
 Inspired by Rails console, PyFireConsole provides a seamless interface to Google's Firestore in Python, simplifying tasks such as connection, ORM, and data associations. It makes managing Firestore a breeze.
 
@@ -15,47 +32,71 @@
 pip install pyfireconsole
 ```
 
 ## Getting Started
 ```python
 from datetime import datetime
 from typing import Optional
-from pyfireconsole.models.pyfire_model import PyfireDoc, PyfireCollection, DocumentRef
+from pyfireconsole.models.association import belongs_to
+from pyfireconsole.models.pyfire_model import PyfireCollection, DocumentRef, PyfireDoc
 from pyfireconsole.db.connection import FirestoreConnection
 
-# Define your models 
+"""
+We assume that you have a firestore database with the following structure:
+- users Collection
+    - {user_id} Document
+        - name: str
+        - email: str
+- publishers Collection
+    - {publisher_id} Document
+        - name: str
+        - address: str
+- books Collection
+    - {book_id} Document
+        - title: str
+        - user_id: str
+        - published_at: datetime
+        - authors: list[str]
+        - tags: Sub Collection
+            - {tag_id} Document
+                - name: str
+        - publisher_ref: Reference
+"""
+
+
 class User(PyfireDoc):
     name: str
     email: str
 
 class Publisher(PyfireDoc):
     name: str
     address: Optional[str]
 
 class Tag(PyfireDoc):
     name: str
 
+
+@belongs_to(User, "user_id")
 class Book(PyfireDoc):
     title: str
     user_id: str
-    PyfireDoc.belongs_to(User)  # Make accessible via book.user
     published_at: datetime
     authors: list[str]
     tags: PyfireCollection[Tag] = PyfireCollection(Tag)
     publisher_ref: DocumentRef[Publisher]
 
 
 # Initialize FirestoreConnection using your default credentials of gcloud. (use `gcloud auth application-default login` or set GOOGLE_APPLICATION_CREDENTIALS)
 FirestoreConnection().initialize(project_id="YOUR-PROJECT-ID")
 
 # Or you can specify service_account_key_path
 # FirestoreConnection().initialize(service_account_key_path="./service-account.json", project_id="YOUR-PROJECT-ID")
 
 print("==================== find ====================")
-book = Book.find("12345")  # => Book
+book = Book.find("XlvQHeGi3cODbI4MQpI3")  # => Book
 print(book.model_dump())  # => dict
 print(f"ID: {book.id} | Title: {book.title} | Authors: {book.authors} | Published At: {book.published_at.isoformat()}")
 
 print("==================== belongs_to ====================")
 print(book.user)  # => User
 print(book.user.name)  # => str
 
@@ -95,48 +136,65 @@
 This feature is inspired by the Rails console.
 
 How to setup interactive console:
 
 ```python
 from datetime import datetime
 from typing import Optional
-from pyfireconsole.models.pyfire_model import PyfireDoc, PyfireCollection, DocumentRef
+from pyfireconsole.models.association import belongs_to, has_many, resolve_pyfire_model_names
+from pyfireconsole.models.pyfire_model import PyfireCollection, DocumentRef, PyfireDoc
 from pyfireconsole.db.connection import FirestoreConnection
 from pyfireconsole import PyFireConsole
 
+
+@has_many('Book', "user_id")
 class User(PyfireDoc):
     name: str
     email: str
 
+
 class Publisher(PyfireDoc):
     name: str
     address: Optional[str]
 
+
 class Tag(PyfireDoc):
     name: str
 
+
+@belongs_to(User, "user_id")
 class Book(PyfireDoc):
     title: str
     user_id: str
-    PyfireDoc.belongs_to(User)  # Make accessible via book.user
     published_at: datetime
     authors: list[str]
     tags: PyfireCollection[Tag] = PyfireCollection(Tag)
     publisher_ref: DocumentRef[Publisher]
 
-FirestoreConnection().initialize(project_id="YOUR-PROJECT-ID")
+# Resolve PyfireModel names
+# Call this function when you define your models by using str class name.
+# e.g. @has_many('Book', "user_id")
+resolve_pyfire_model_names(globals())
+
+
+FirestoreConnection().initialize(project_id="YOUR_PROJECT_ID")
 PyFireConsole().run()
 ```
 
 
 Alternatively, you can define your model files in `app/models/` and initialize the console as follows:
 
 ```python
 from pyfireconsole.db.connection import FirestoreConnection
 from pyfireconsole import PyFireConsole
+from pyfireconsole.models.association import resolve_pyfire_model_names
+
+# Resolve PyfireModel names
+resolve_pyfire_model_names(globals())
+
 
 FirestoreConnection().initialize(project_id="YOUR-PROJECT-ID")
 PyFireConsole(model_dir="app/models").run()
 ```
 
 Through the interactive console, you can conveniently test and experiment with your Firestore data models.
```

### Comparing `pyfireconsole-0.0.3/pyfireconsole/console/pyfireconsole.py` & `pyfireconsole-0.0.4/pyfireconsole/console/pyfireconsole.py`

 * *Files identical despite different names*

### Comparing `pyfireconsole-0.0.3/pyfireconsole/db/connection.py` & `pyfireconsole-0.0.4/pyfireconsole/db/connection.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 from typing import Optional
 
 from google.cloud import firestore
 from google.oauth2.service_account import Credentials as ServiceAccountCredentials  # type: ignore
 
 
+class NotConnectedException(Exception):
+    pass
+
+
 class FirestoreConnection:
     _instance: Optional['FirestoreConnection'] = None
     db: Optional[firestore.Client] = None
 
     def __new__(cls, *args, **kwargs):
         if cls._instance is None:
             cls._instance = super().__new__(cls, *args, **kwargs)
@@ -18,15 +22,18 @@
         if self.db is None:
             if service_account_key_path:
                 creds = ServiceAccountCredentials.from_service_account_file(service_account_key_path)
                 self.db = firestore.Client(credentials=creds, project=project_id)
             else:
                 self.db = firestore.Client(project=project_id)
 
+    def set_db(self, db):
+        self.db = db
+
     def collection(self, collection_name):
         if self.db is None:
-            raise ValueError("FirestoreConnection is not initialized. Call initialize() first.")
+            raise NotConnectedException("FirestoreConnection is not initialized. Call initialize() first.")
         return self.db.collection(collection_name)
 
 
 # global singleton instance
 conn = FirestoreConnection()
```

### Comparing `pyfireconsole-0.0.3/pyfireconsole/models/pyfire_model.py` & `pyfireconsole-0.0.4/pyfireconsole/models/pyfire_model.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,27 @@
-from typing import Generic, Iterable, Optional, Type, TypeVar
+from typing import Generic, Iterable, Optional, Type, TypeVar, get_origin
 
 import inflect
 from pydantic import BaseModel
 
+from pyfireconsole.queries.get_query import DocNotFoundException
 from pyfireconsole.queries.query_runner import QueryRunner
+from pyfireconsole.queries.where_clouse import WhereCondition
 
 ModelType = TypeVar('ModelType', bound='PyfireDoc')
 
 
 class PyfireCollection(Generic[ModelType]):
     model_class: Type[ModelType]
-    _parent_model: Optional['PyfireDoc']
-    _collection: Iterable[ModelType] = []
+    _parent_model: Optional['PyfireDoc'] = None
+    _collection: Optional[Iterable[dict]] = None
+    _where_cond: Optional[WhereCondition] = None
 
     def __init__(self, model_class: Type[ModelType]):
         self.model_class = model_class
-        self._parent_model = None
 
     def obj_ref_key(self) -> str:
         """ Represents the key of firestore entity """
         return self.obj_collection_name()
 
     def set_parent(self, parent_model: 'PyfireDoc'):
         self._parent_model = parent_model
@@ -28,29 +30,53 @@
         leaf_collection_name = self.model_class.collection_name()
         if self._parent_model is None:
             return leaf_collection_name  # e.g. "users"
         else:
             return f"{self._parent_model.obj_ref_key()}/{leaf_collection_name}"  # e.g. "users/123/books"
 
     def __iter__(self):
-        docs = QueryRunner(self.obj_ref_key()).all()
+        if self._where_cond is not None:
+            self._collection = QueryRunner(self.obj_ref_key()).where(self._where_cond.field, self._where_cond.operator, self._where_cond.value)
+        else:
+            self._collection = QueryRunner(self.obj_ref_key()).all()
 
-        for doc in docs:
+        for doc in self._collection:
+            doc = self.model_class.model_field_load(doc)
             obj = self.model_class(**doc)
-            obj._parent = self._parent_model
+            obj._parent = self
             yield obj
 
+    def first(self) -> ModelType | None:
+        try:
+            return next(iter(self))
+        except StopIteration:
+            return None
+
     def where(self, field: str, operator: str, value: str) -> 'PyfireCollection[ModelType]':
         coll = PyfireCollection(self.model_class)
+        coll._where_cond = WhereCondition(field, operator, value)
         if self._parent_model is not None:
             coll.set_parent(self._parent_model)
-        docs = QueryRunner(self.obj_collection_name()).where(field, operator, value)
-        coll._collection = [self.model_class.model_validate(d) for d in docs]
+
         return coll
 
+    def add(self, entity: ModelType) -> ModelType:
+        assert isinstance(entity, self.model_class)
+
+        entity._parent = self
+        data = entity.model_field_dump()
+        if entity.id is None:
+            _id = QueryRunner(self.obj_collection_name()).create(data)
+            if _id:
+                entity.id = _id
+        else:
+            raise ValueError("Could not save document")
+
+        return entity
+
     def __str__(self) -> str:
         if self._parent_model is None:
             return f"{self.__class__.__name__}[{self.model_class.__name__}]"
         return f"{self.__class__.__name__}[{self.model_class.__name__}](parent={self._parent_model.__class__.__name__})"
 
 
 class DocumentRef(BaseModel, Generic[ModelType]):
@@ -60,15 +86,15 @@
     # book.user_ref.get() => User object
 
 
 class PyfireDoc(BaseModel):
     class Config:
         arbitrary_types_allowed = True
 
-    id: str  # Firestore document id
+    id: Optional[str] = None  # Firestore document id
     _parent: Optional[PyfireCollection] = None  # when a model is a subcollection, this is the parent model
 
     def __init__(self, **data):
         super().__init__(**data)
         self._setup_collections()
 
     def _setup_collections(self):
@@ -78,64 +104,100 @@
             if isinstance(attr, PyfireCollection):
                 attr.set_parent(self)
             elif isinstance(attr, DocumentRef):
                 pass
 
     def obj_ref_key(self) -> str:
         """ Represents the key of firestore entity """
+        return f"{self.obj_collection_name()}/{self.id}"
+
+    def obj_collection_name(self) -> str:
+        """ Represents the name of firestore collection """
         db_name = self.__class__.collection_name()
         if self._parent is None:
-            return f"{db_name}/{self.id}"
+            return f"{db_name}"
         else:
-            return f"{self._parent.obj_ref_key()}/{db_name}/{self.id}"
+            return self._parent.obj_ref_key()
 
-    def save(self) -> None:
-        raise NotImplementedError
+    def model_field_dump(self) -> dict:
+        """
+        Returns the model fields as dict. This is used for saving the model to firestore.
+        Does not include collection fields.
+        """
+        data = self.model_dump()
+
+        for name, _ in self.__annotations__.items():
+            attr = getattr(self, name, None)
+            if isinstance(attr, PyfireCollection):
+                data.pop(name)
+        # if "id" in data:  # TODO when original doc has id field. This should be False?
+        #     data.pop('id')
+
+        return data
 
     @classmethod
-    def find(cls, id: str, allow_empty: bool = False) -> 'PyfireDoc':
-        d = QueryRunner(cls.collection_name()).get(id)
+    def model_field_load(cls, data: dict) -> dict:
+        """
+        Filters out collection fields from the data dict.
+        """
+        for name, klass in cls.__annotations__.items():
+            if name not in data:
+                continue
+            if get_origin(klass) == PyfireCollection:
+                data.pop(name)
+        return data
+
+    def save(self) -> 'PyfireDoc':
+        data = self.model_field_dump()
+        if self.id is None:
+            _id = QueryRunner(self.obj_collection_name()).create(data)
+            if _id:
+                self.id = _id
+        else:
+            _id = QueryRunner(self.obj_collection_name()).save(self.id, data)
+
+        if _id is None:
+            raise ValueError("Could not save document")
+        return self
 
-        if d is None:
+    @classmethod
+    def new(cls, **kwargs) -> 'PyfireDoc':
+        doc = cls(**kwargs)
+        return doc
+
+    @classmethod
+    def find(cls, id: str, allow_empty: bool = False) -> 'PyfireDoc':
+        try:
+            d = QueryRunner(cls.collection_name()).get(id)
+            if d is None:
+                raise DocNotFoundException(f"Document {cls.collection_name()}/{id} not found")
+            d = cls.model_field_load(d)
+        except DocNotFoundException as e:
             if allow_empty:
                 return cls.empty_doc(id)
             else:
-                raise ValueError(f"Could not find {cls.__name__} with id {id}")
+                raise e
         return cls.model_validate(d)
 
     @classmethod
+    def first(cls) -> Optional['PyfireDoc']:
+        coll = PyfireCollection(cls)
+        return coll.first()
+
+    @classmethod
     def empty_doc(cls, id) -> 'PyfireDoc':
         doc = cls.model_construct(id=id)
         doc._setup_collections()
         return doc
 
     @classmethod
     def where(cls, field: str, operator: str, value: str) -> PyfireCollection['PyfireDoc']:
         coll = PyfireCollection(cls)
-        docs = QueryRunner(cls.collection_name()).where(field, operator, value)
-        coll._collection = [cls.model_validate(d) for d in docs]
+        coll._where_cond = WhereCondition(field, operator, value)
         return coll
-        # docs = QueryRunner(cls.collection_name()).where(field, operator, value)
-        # return [cls.model_validate(d) for d in docs]
 
     @classmethod
     def collection_name(cls) -> str:
         """
         Override this method to change the name of the collection in Firestore
         """
         return inflect.engine().plural(cls.__name__).lower()
-
-    @classmethod
-    def belongs_to(cls, model_class: Type[ModelType], db_field: Optional[str] = None, attr_name: Optional[str] = None):
-        def getter_method(self):
-            model_id = getattr(self, db_field)
-            if model_id:
-                return model_class.find(model_id)
-            else:
-                return None
-
-        db_field = db_field or f"{model_class.__name__.lower()}_id"
-        attr_name = attr_name or model_class.__name__.lower()
-        setattr(cls, model_class.__name__.lower(), property(getter_method))
-
-    def __str__(self) -> str:
-        return f"{self.__class__.__name__}({super().__str__()})"
```

### Comparing `pyfireconsole-0.0.3/pyfireconsole/queries/abstract_query.py` & `pyfireconsole-0.0.4/pyfireconsole/queries/abstract_query.py`

 * *Files identical despite different names*

### Comparing `pyfireconsole-0.0.3/pyfireconsole/queries/get_query.py` & `pyfireconsole-0.0.4/pyfireconsole/queries/get_query.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,8 +11,8 @@
         self.doc_id = doc_id
 
     def exec(self) -> dict | None:
         doc_ref = self.collection_ref(self.collection_key).document(self.doc_id)
         doc = doc_ref.get()
         if doc.exists:
             return dict(_doc_to_dict(doc) or {}, id=doc.id)
-        return None
+        raise DocNotFoundException(f"Document with id {self.doc_id} not found")
```

### Comparing `pyfireconsole-0.0.3/pyfireconsole/queries/query_runner.py` & `pyfireconsole-0.0.4/pyfireconsole/queries/query_runner.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Dict
 
 from pyfireconsole.db.connection import conn
 from pyfireconsole.queries.all_query import AllQuery
 from pyfireconsole.queries.get_query import GetQuery
+from pyfireconsole.queries.save_query import SaveQuery
 from pyfireconsole.queries.where_query import WhereQuery
 
 
 class QueryRunner:
     def __init__(self, collection_key: str):
         self.conn = conn
         self.collection_key = collection_key
@@ -15,7 +16,13 @@
         return GetQuery(self.collection_key, id).set_conn(self.conn).exec()
 
     def where(self, field: str, operator: str, value: str) -> list[Dict]:
         return WhereQuery(self.collection_key, field, operator, value).set_conn(self.conn).exec()
 
     def all(self) -> list[Dict]:
         return AllQuery(self.collection_key).set_conn(self.conn).exec()
+
+    def save(self, id: str, data: dict) -> str | None:
+        return SaveQuery(self.collection_key, id, data).set_conn(self.conn).exec()
+
+    def create(self, data: dict) -> str | None:
+        return SaveQuery(self.collection_key, None, data).set_conn(self.conn).exec()
```

### Comparing `pyfireconsole-0.0.3/pyfireconsole.egg-info/PKG-INFO` & `pyfireconsole-0.0.4/pyfireconsole.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: pyfireconsole
-Version: 0.0.3
+Version: 0.0.4
 Summary: An interactive console for Firestore based on Python ORM
 Home-page: https://github.com/tan-z-tan/pyfireconsole
 Author: Makoto Tanji
 Author-email: tanji.makoto@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.10.0
+Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+[![Python package](https://github.com/tan-z-tan/PyFireConsole/actions/workflows/test.yml/badge.svg)](https://github.com/tan-z-tan/PyFireConsole/actions/workflows/test.yml)
+
 <h1 style="text-align: center;">
   <img src="https://raw.githubusercontent.com/tan-z-tan/pyfireconsole/main/logo.png" alt="PyFireConsole">
 </h1>
 
 ## Introduction
 Inspired by Rails console, PyFireConsole provides a seamless interface to Google's Firestore in Python, simplifying tasks such as connection, ORM, and data associations. It makes managing Firestore a breeze.
 
@@ -30,47 +32,71 @@
 pip install pyfireconsole
 ```
 
 ## Getting Started
 ```python
 from datetime import datetime
 from typing import Optional
-from pyfireconsole.models.pyfire_model import PyfireDoc, PyfireCollection, DocumentRef
+from pyfireconsole.models.association import belongs_to
+from pyfireconsole.models.pyfire_model import PyfireCollection, DocumentRef, PyfireDoc
 from pyfireconsole.db.connection import FirestoreConnection
 
-# Define your models 
+"""
+We assume that you have a firestore database with the following structure:
+- users Collection
+    - {user_id} Document
+        - name: str
+        - email: str
+- publishers Collection
+    - {publisher_id} Document
+        - name: str
+        - address: str
+- books Collection
+    - {book_id} Document
+        - title: str
+        - user_id: str
+        - published_at: datetime
+        - authors: list[str]
+        - tags: Sub Collection
+            - {tag_id} Document
+                - name: str
+        - publisher_ref: Reference
+"""
+
+
 class User(PyfireDoc):
     name: str
     email: str
 
 class Publisher(PyfireDoc):
     name: str
     address: Optional[str]
 
 class Tag(PyfireDoc):
     name: str
 
+
+@belongs_to(User, "user_id")
 class Book(PyfireDoc):
     title: str
     user_id: str
-    PyfireDoc.belongs_to(User)  # Make accessible via book.user
     published_at: datetime
     authors: list[str]
     tags: PyfireCollection[Tag] = PyfireCollection(Tag)
     publisher_ref: DocumentRef[Publisher]
 
 
 # Initialize FirestoreConnection using your default credentials of gcloud. (use `gcloud auth application-default login` or set GOOGLE_APPLICATION_CREDENTIALS)
 FirestoreConnection().initialize(project_id="YOUR-PROJECT-ID")
 
 # Or you can specify service_account_key_path
 # FirestoreConnection().initialize(service_account_key_path="./service-account.json", project_id="YOUR-PROJECT-ID")
 
 print("==================== find ====================")
-book = Book.find("12345")  # => Book
+book = Book.find("XlvQHeGi3cODbI4MQpI3")  # => Book
 print(book.model_dump())  # => dict
 print(f"ID: {book.id} | Title: {book.title} | Authors: {book.authors} | Published At: {book.published_at.isoformat()}")
 
 print("==================== belongs_to ====================")
 print(book.user)  # => User
 print(book.user.name)  # => str
 
@@ -110,48 +136,65 @@
 This feature is inspired by the Rails console.
 
 How to setup interactive console:
 
 ```python
 from datetime import datetime
 from typing import Optional
-from pyfireconsole.models.pyfire_model import PyfireDoc, PyfireCollection, DocumentRef
+from pyfireconsole.models.association import belongs_to, has_many, resolve_pyfire_model_names
+from pyfireconsole.models.pyfire_model import PyfireCollection, DocumentRef, PyfireDoc
 from pyfireconsole.db.connection import FirestoreConnection
 from pyfireconsole import PyFireConsole
 
+
+@has_many('Book', "user_id")
 class User(PyfireDoc):
     name: str
     email: str
 
+
 class Publisher(PyfireDoc):
     name: str
     address: Optional[str]
 
+
 class Tag(PyfireDoc):
     name: str
 
+
+@belongs_to(User, "user_id")
 class Book(PyfireDoc):
     title: str
     user_id: str
-    PyfireDoc.belongs_to(User)  # Make accessible via book.user
     published_at: datetime
     authors: list[str]
     tags: PyfireCollection[Tag] = PyfireCollection(Tag)
     publisher_ref: DocumentRef[Publisher]
 
-FirestoreConnection().initialize(project_id="YOUR-PROJECT-ID")
+# Resolve PyfireModel names
+# Call this function when you define your models by using str class name.
+# e.g. @has_many('Book', "user_id")
+resolve_pyfire_model_names(globals())
+
+
+FirestoreConnection().initialize(project_id="YOUR_PROJECT_ID")
 PyFireConsole().run()
 ```
 
 
 Alternatively, you can define your model files in `app/models/` and initialize the console as follows:
 
 ```python
 from pyfireconsole.db.connection import FirestoreConnection
 from pyfireconsole import PyFireConsole
+from pyfireconsole.models.association import resolve_pyfire_model_names
+
+# Resolve PyfireModel names
+resolve_pyfire_model_names(globals())
+
 
 FirestoreConnection().initialize(project_id="YOUR-PROJECT-ID")
 PyFireConsole(model_dir="app/models").run()
 ```
 
 Through the interactive console, you can conveniently test and experiment with your Firestore data models.
```

### Comparing `pyfireconsole-0.0.3/pyfireconsole.egg-info/SOURCES.txt` & `pyfireconsole-0.0.4/pyfireconsole.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 pyfireconsole.egg-info/requires.txt
 pyfireconsole.egg-info/top_level.txt
 pyfireconsole/console/__init__.py
 pyfireconsole/console/pyfireconsole.py
 pyfireconsole/db/__init__.py
 pyfireconsole/db/connection.py
 pyfireconsole/models/__init__.py
+pyfireconsole/models/association.py
 pyfireconsole/models/pyfire_model.py
 pyfireconsole/queries/__init__.py
 pyfireconsole/queries/abstract_query.py
 pyfireconsole/queries/all_query.py
 pyfireconsole/queries/get_query.py
 pyfireconsole/queries/query_runner.py
+pyfireconsole/queries/save_query.py
+pyfireconsole/queries/where_clouse.py
 pyfireconsole/queries/where_query.py
```

### Comparing `pyfireconsole-0.0.3/setup.py` & `pyfireconsole-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pyfireconsole',
-    version='0.0.3',
+    version='0.0.4',
     author='Makoto Tanji',
     author_email='tanji.makoto@gmail.com',
     description='An interactive console for Firestore based on Python ORM',
     long_description=open('README.md', 'r').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/tan-z-tan/pyfireconsole',
     packages=find_packages(),
-    python_requires='>=3.10.0',
+    python_requires='>=3.8.0',
     install_requires=[
         'google-cloud-firestore>=2.0.0,<3.0.0',
         'google-auth>=2.0.0,<3.0.0',
         'inflect>=6.0.0,<8.0.0',
         'pydantic>=2.0.1,<3.0.0',
         'ipython>=7.0.1,<9.0.0',
     ],
```

