# Comparing `tmp/aorta_sirius-0.8.tar.gz` & `tmp/aorta_sirius-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aorta_sirius-0.8.tar", last modified: Mon Jun 19 06:13:16 2023, max compression
+gzip compressed data, was "aorta_sirius-0.9.tar", last modified: Mon Jun 19 06:24:24 2023, max compression
```

## Comparing `aorta_sirius-0.8.tar` & `aorta_sirius-0.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:13:16.530640 aorta_sirius-0.8/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-19 06:13:16.530640 aorta_sirius-0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-19 06:12:58.000000 aorta_sirius-0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 06:13:16.530640 aorta_sirius-0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-19 06:12:58.000000 aorta_sirius-0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:13:16.526641 aorta_sirius-0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:13:16.526641 aorta_sirius-0.8/src/aorta_sirius.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-19 06:13:16.000000 aorta_sirius-0.8/src/aorta_sirius.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-19 06:13:16.000000 aorta_sirius-0.8/src/aorta_sirius.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 06:13:16.000000 aorta_sirius-0.8/src/aorta_sirius.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-19 06:13:16.000000 aorta_sirius-0.8/src/aorta_sirius.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-19 06:13:16.000000 aorta_sirius-0.8/src/aorta_sirius.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:13:16.526641 aorta_sirius-0.8/src/sirius/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 06:12:58.000000 aorta_sirius-0.8/src/sirius/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:13:16.526641 aorta_sirius-0.8/src/sirius/application_performance_monitoring/
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-06-19 06:12:58.000000 aorta_sirius-0.8/src/sirius/application_performance_monitoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-19 06:12:58.000000 aorta_sirius-0.8/src/sirius/application_performance_monitoring/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-06-19 06:12:58.000000 aorta_sirius-0.8/src/sirius/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:13:16.526641 aorta_sirius-0.8/src/sirius/communication/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 06:12:58.000000 aorta_sirius-0.8/src/sirius/communication/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:13:16.526641 aorta_sirius-0.8/src/sirius/communication/discord/
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-06-19 06:12:58.000000 aorta_sirius-0.8/src/sirius/communication/discord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-19 06:12:58.000000 aorta_sirius-0.8/src/sirius/communication/discord/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-19 06:12:58.000000 aorta_sirius-0.8/src/sirius/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:13:16.526641 aorta_sirius-0.8/src/sirius/database/
--rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-06-19 06:12:58.000000 aorta_sirius-0.8/src/sirius/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-19 06:12:58.000000 aorta_sirius-0.8/src/sirius/database/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-19 06:12:58.000000 aorta_sirius-0.8/src/sirius/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:13:16.526641 aorta_sirius-0.8/src/sirius/http_requests/
--rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-06-19 06:12:58.000000 aorta_sirius-0.8/src/sirius/http_requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-19 06:12:58.000000 aorta_sirius-0.8/src/sirius/http_requests/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:24:24.012643 aorta_sirius-0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-19 06:24:24.012643 aorta_sirius-0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-19 06:23:18.000000 aorta_sirius-0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 06:24:24.012643 aorta_sirius-0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-19 06:23:18.000000 aorta_sirius-0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:24:24.012643 aorta_sirius-0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:24:24.012643 aorta_sirius-0.9/src/aorta_sirius.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-19 06:24:23.000000 aorta_sirius-0.9/src/aorta_sirius.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-19 06:24:23.000000 aorta_sirius-0.9/src/aorta_sirius.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 06:24:23.000000 aorta_sirius-0.9/src/aorta_sirius.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-19 06:24:23.000000 aorta_sirius-0.9/src/aorta_sirius.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-19 06:24:23.000000 aorta_sirius-0.9/src/aorta_sirius.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:24:24.012643 aorta_sirius-0.9/src/sirius/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 06:23:18.000000 aorta_sirius-0.9/src/sirius/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:24:24.012643 aorta_sirius-0.9/src/sirius/application_performance_monitoring/
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-06-19 06:23:18.000000 aorta_sirius-0.9/src/sirius/application_performance_monitoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-19 06:23:18.000000 aorta_sirius-0.9/src/sirius/application_performance_monitoring/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-06-19 06:23:18.000000 aorta_sirius-0.9/src/sirius/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:24:24.012643 aorta_sirius-0.9/src/sirius/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 06:23:18.000000 aorta_sirius-0.9/src/sirius/communication/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:24:24.012643 aorta_sirius-0.9/src/sirius/communication/discord/
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-06-19 06:23:18.000000 aorta_sirius-0.9/src/sirius/communication/discord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-19 06:23:18.000000 aorta_sirius-0.9/src/sirius/communication/discord/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-19 06:23:18.000000 aorta_sirius-0.9/src/sirius/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:24:24.012643 aorta_sirius-0.9/src/sirius/database/
+-rw-r--r--   0 runner    (1001) docker     (123)     4371 2023-06-19 06:23:18.000000 aorta_sirius-0.9/src/sirius/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-19 06:23:18.000000 aorta_sirius-0.9/src/sirius/database/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-19 06:23:18.000000 aorta_sirius-0.9/src/sirius/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:24:24.012643 aorta_sirius-0.9/src/sirius/http_requests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-06-19 06:23:18.000000 aorta_sirius-0.9/src/sirius/http_requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-19 06:23:18.000000 aorta_sirius-0.9/src/sirius/http_requests/exceptions.py
```

### Comparing `aorta_sirius-0.8/setup.py` & `aorta_sirius-0.9/setup.py`

 * *Files identical despite different names*

### Comparing `aorta_sirius-0.8/src/aorta_sirius.egg-info/SOURCES.txt` & `aorta_sirius-0.9/src/aorta_sirius.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aorta_sirius-0.8/src/sirius/application_performance_monitoring/__init__.py` & `aorta_sirius-0.9/src/sirius/application_performance_monitoring/__init__.py`

 * *Files identical despite different names*

### Comparing `aorta_sirius-0.8/src/sirius/common.py` & `aorta_sirius-0.9/src/sirius/common.py`

 * *Files identical despite different names*

### Comparing `aorta_sirius-0.8/src/sirius/communication/discord/__init__.py` & `aorta_sirius-0.9/src/sirius/communication/discord/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         channel: TextChannel = await _get_text_channel(channel_name)
         await channel.send(message)
         await client.close()
 
     await client.start(common.get_environmental_variable(EnvironmentVariable.DISCORD_BOT_TOKEN), reconnect=True)
 
 
-async def _get_server() -> Guild:
+async def _get_server() -> Guild:  # type: ignore[return]
     global client
     server_name: str = common.get_environmental_variable(EnvironmentVariable.DISCORD_SERVER_NAME)
     if not common.is_production_environment():
         server_name = server_name + " [Dev]"
 
     guild_list: List[Guild] = list(filter(lambda g: g.name == server_name, client.guilds))
```

### Comparing `aorta_sirius-0.8/src/sirius/database/__init__.py` & `aorta_sirius-0.9/src/sirius/database/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 
     client = AsyncIOMotorClient(common.get_environmental_variable(EnvironmentVariable.MONGO_DB_CONNECTION_STRING))
     await init_beanie(database=client[database_name], document_models=DatabaseDocument.__subclasses__())
 
 
 def transaction(transaction_name: Optional[str] = None) -> Callable:
     def decorator(function: Callable) -> Callable:
-
         @application_performance_monitoring.transaction(Operation.AORTA_SIRIUS, transaction_name)
         @functools.wraps(function)
         async def wrapper(*args: List[Any], **kwargs: Dict[str, Any]) -> Any:
             await initialize()
             return await function(*args, **kwargs)
 
         return wrapper
@@ -49,17 +48,17 @@
         state_management_save_previous = True
 
     def __init__(self, *args: List[Any], **kwargs: Dict[Any, Any]) -> None:
         for key, value in kwargs.items():
             if isinstance(value, DatabaseDocument):
                 if value.id is None:
                     raise UncommittedRelationalDocumentException(f"Uncommitted document is trying to be related\nUncommitted Object: {str(object)}\nObject being related: {str(self)}")
-                kwargs[key] = value.id
+                kwargs[key] = value.id  # type: ignore[assignment]
 
-        super().__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)  # type: ignore[no-untyped-call]
 
     @application_performance_monitoring.transaction(Operation.DATABASE, "Save")
     async def commit(self) -> "DatabaseDocument":
         if self.id is None:
             return await super().save(link_rule=beanie.WriteRules.WRITE)
         else:
             return await super().save_changes()
@@ -67,33 +66,33 @@
     @application_performance_monitoring.transaction(Operation.DATABASE, "Delete")
     async def remove(self) -> None:
         return await super().delete()
 
     @classmethod
     @application_performance_monitoring.transaction(Operation.DATABASE, "Find Single")
     async def find_unique(cls, *args: List[Any], fetch_links: bool = False) -> Optional["DatabaseDocument"]:
-        results_list: List[DatabaseDocument] = await super().find_many(*args).to_list()
+        results_list: List[DatabaseDocument] = await super().find_many(*args).to_list()  # type: ignore[call-overload]
 
         if len(results_list) == 1:
             result: DatabaseDocument = results_list[0]
         elif len(results_list) == 0:
             return None
         else:
             raise NonUniqueResultException(f"Non-unique result found\nCollection: {cls.__name__}\nSearch Criteria: {str(*args)}")
 
         if fetch_links:
-            await result.fetch_all_links()
+            await result.fetch_all_links()  # type: ignore[no-untyped-call]
         return result
 
     @classmethod
     @application_performance_monitoring.transaction(Operation.DATABASE, "Find Multiple")
     async def find_multiple(cls, search_criteria: Dict[Any, Any], fetch_links: bool = False) -> List["DatabaseDocument"]:
         results_list: List[DatabaseDocument] = await super().find_many(search_criteria).to_list()
         if fetch_links:
             for result in results_list:
-                await result.fetch_all_links()
+                await result.fetch_all_links()  # type: ignore[no-untyped-call]
         return results_list
 
     @staticmethod
     @application_performance_monitoring.transaction(Operation.DATABASE, "Save All")
     async def commit_all(database_document_list: List["DatabaseDocument"]) -> List["DatabaseDocument"]:
         return [await database_document.commit() for database_document in database_document_list]
```

### Comparing `aorta_sirius-0.8/src/sirius/http_requests/__init__.py` & `aorta_sirius-0.9/src/sirius/http_requests/__init__.py`

 * *Files identical despite different names*

