# Comparing `tmp/svcs-23.8.0.tar.gz` & `tmp/svcs-23.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Fri Aug  4 20:16:10 2023, max compression
+gzip compressed data, last modified: Sun Aug  6 06:51:14 2023, max compression
```

## Comparing `svcs-23.8.0.tar` & `svcs-23.9.0.tar`

### file list

```diff
@@ -1,37 +1,39 @@
--rw-r--r--   0        0        0      125 2023-08-04 20:16:10.000000 svcs-23.8.0/.git_archival.txt
--rw-r--r--   0        0        0      131 2023-08-04 20:16:10.000000 svcs-23.8.0/.gitattributes
--rw-r--r--   0        0        0      732 2023-08-04 20:16:10.000000 svcs-23.8.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0        5 2023-08-04 20:16:10.000000 svcs-23.8.0/.python-version-default
--rw-r--r--   0        0        0     3558 2023-08-04 20:16:10.000000 svcs-23.8.0/CHANGELOG.md
--rw-r--r--   0        0        0    18592 2023-08-04 20:16:10.000000 svcs-23.8.0/README.md
--rw-r--r--   0        0        0     1052 2023-08-04 20:16:10.000000 svcs-23.8.0/conftest.py
--rw-r--r--   0        0        0      840 2023-08-04 20:16:10.000000 svcs-23.8.0/tox.ini
--rw-r--r--   0        0        0     5482 2023-08-04 20:16:10.000000 svcs-23.8.0/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      285 2023-08-04 20:16:10.000000 svcs-23.8.0/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0       18 2023-08-04 20:16:10.000000 svcs-23.8.0/.github/FUNDING.yml
--rw-r--r--   0        0        0      865 2023-08-04 20:16:10.000000 svcs-23.8.0/.github/SECURITY.md
--rw-r--r--   0        0        0      117 2023-08-04 20:16:10.000000 svcs-23.8.0/.github/dependabot.yml
--rw-r--r--   0        0        0     4110 2023-08-04 20:16:10.000000 svcs-23.8.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0      749 2023-08-04 20:16:10.000000 svcs-23.8.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0     1730 2023-08-04 20:16:10.000000 svcs-23.8.0/.github/workflows/pypi-package.yml
--rw-r--r--   0        0        0     4549 2023-08-04 20:16:10.000000 svcs-23.8.0/docs/_static/logo.svg
--rw-r--r--   0        0        0     3834 2023-08-04 20:16:10.000000 svcs-23.8.0/docs/_static/logo_with_name.svg
--rw-r--r--   0        0        0      650 2023-08-04 20:16:10.000000 svcs-23.8.0/src/svcs/__init__.py
--rw-r--r--   0        0        0    12105 2023-08-04 20:16:10.000000 svcs-23.8.0/src/svcs/_core.py
--rw-r--r--   0        0        0      234 2023-08-04 20:16:10.000000 svcs-23.8.0/src/svcs/exceptions.py
--rw-r--r--   0        0        0     3512 2023-08-04 20:16:10.000000 svcs-23.8.0/src/svcs/flask.py
--rw-r--r--   0        0        0        0 2023-08-04 20:16:10.000000 svcs-23.8.0/src/svcs/py.typed
--rw-r--r--   0        0        0       91 2023-08-04 20:16:10.000000 svcs-23.8.0/tests/__init__.py
--rw-r--r--   0        0        0      405 2023-08-04 20:16:10.000000 svcs-23.8.0/tests/fake_factories.py
--rw-r--r--   0        0        0      481 2023-08-04 20:16:10.000000 svcs-23.8.0/tests/ifaces.py
--rw-r--r--   0        0        0     2394 2023-08-04 20:16:10.000000 svcs-23.8.0/tests/test_container.py
--rw-r--r--   0        0        0     1663 2023-08-04 20:16:10.000000 svcs-23.8.0/tests/test_fake_factories.py
--rw-r--r--   0        0        0     6883 2023-08-04 20:16:10.000000 svcs-23.8.0/tests/test_flask.py
--rw-r--r--   0        0        0     8309 2023-08-04 20:16:10.000000 svcs-23.8.0/tests/test_integration.py
--rw-r--r--   0        0        0     8089 2023-08-04 20:16:10.000000 svcs-23.8.0/tests/test_registry.py
--rw-r--r--   0        0        0     1486 2023-08-04 20:16:10.000000 svcs-23.8.0/tests/typing/core.py
--rw-r--r--   0        0        0     1056 2023-08-04 20:16:10.000000 svcs-23.8.0/tests/typing/flask_.py
--rw-r--r--   0        0        0      112 2023-08-04 20:16:10.000000 svcs-23.8.0/.gitignore
--rw-r--r--   0        0        0     1098 2023-08-04 20:16:10.000000 svcs-23.8.0/LICENSE
--rw-r--r--   0        0        0     4845 2023-08-04 20:16:10.000000 svcs-23.8.0/pyproject.toml
--rw-r--r--   0        0        0     7974 2023-08-04 20:16:10.000000 svcs-23.8.0/PKG-INFO
+-rw-r--r--   0        0        0      125 2023-08-06 06:51:14.000000 svcs-23.9.0/.git_archival.txt
+-rw-r--r--   0        0        0      131 2023-08-06 06:51:14.000000 svcs-23.9.0/.gitattributes
+-rw-r--r--   0        0        0      732 2023-08-06 06:51:14.000000 svcs-23.9.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        5 2023-08-06 06:51:14.000000 svcs-23.9.0/.python-version-default
+-rw-r--r--   0        0        0     4432 2023-08-06 06:51:14.000000 svcs-23.9.0/CHANGELOG.md
+-rw-r--r--   0        0        0    19303 2023-08-06 06:51:14.000000 svcs-23.9.0/README.md
+-rw-r--r--   0        0        0     1052 2023-08-06 06:51:14.000000 svcs-23.9.0/conftest.py
+-rw-r--r--   0        0        0      840 2023-08-06 06:51:14.000000 svcs-23.9.0/tox.ini
+-rw-r--r--   0        0        0     5482 2023-08-06 06:51:14.000000 svcs-23.9.0/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      285 2023-08-06 06:51:14.000000 svcs-23.9.0/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0       18 2023-08-06 06:51:14.000000 svcs-23.9.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0      865 2023-08-06 06:51:14.000000 svcs-23.9.0/.github/SECURITY.md
+-rw-r--r--   0        0        0      117 2023-08-06 06:51:14.000000 svcs-23.9.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     4110 2023-08-06 06:51:14.000000 svcs-23.9.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      749 2023-08-06 06:51:14.000000 svcs-23.9.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0     1730 2023-08-06 06:51:14.000000 svcs-23.9.0/.github/workflows/pypi-package.yml
+-rw-r--r--   0        0        0    38235 2023-08-06 06:51:14.000000 svcs-23.9.0/docs/_static/logo.afdesign
+-rw-r--r--   0        0        0     2721 2023-08-06 06:51:14.000000 svcs-23.9.0/docs/_static/logo.svg
+-rw-r--r--   0        0        0    37323 2023-08-06 06:51:14.000000 svcs-23.9.0/docs/_static/logo_with_name.afdesign
+-rw-r--r--   0        0        0     4036 2023-08-06 06:51:14.000000 svcs-23.9.0/docs/_static/logo_with_name.svg
+-rw-r--r--   0        0        0      650 2023-08-06 06:51:14.000000 svcs-23.9.0/src/svcs/__init__.py
+-rw-r--r--   0        0        0    18891 2023-08-06 06:51:14.000000 svcs-23.9.0/src/svcs/_core.py
+-rw-r--r--   0        0        0      234 2023-08-06 06:51:14.000000 svcs-23.9.0/src/svcs/exceptions.py
+-rw-r--r--   0        0        0     5993 2023-08-06 06:51:14.000000 svcs-23.9.0/src/svcs/flask.py
+-rw-r--r--   0        0        0        0 2023-08-06 06:51:14.000000 svcs-23.9.0/src/svcs/py.typed
+-rw-r--r--   0        0        0       91 2023-08-06 06:51:14.000000 svcs-23.9.0/tests/__init__.py
+-rw-r--r--   0        0        0      405 2023-08-06 06:51:14.000000 svcs-23.9.0/tests/fake_factories.py
+-rw-r--r--   0        0        0      481 2023-08-06 06:51:14.000000 svcs-23.9.0/tests/ifaces.py
+-rw-r--r--   0        0        0     3603 2023-08-06 06:51:14.000000 svcs-23.9.0/tests/test_container.py
+-rw-r--r--   0        0        0     1663 2023-08-06 06:51:14.000000 svcs-23.9.0/tests/test_fake_factories.py
+-rw-r--r--   0        0        0     7292 2023-08-06 06:51:14.000000 svcs-23.9.0/tests/test_flask.py
+-rw-r--r--   0        0        0     9082 2023-08-06 06:51:14.000000 svcs-23.9.0/tests/test_integration.py
+-rw-r--r--   0        0        0     9033 2023-08-06 06:51:14.000000 svcs-23.9.0/tests/test_registry.py
+-rw-r--r--   0        0        0     2341 2023-08-06 06:51:14.000000 svcs-23.9.0/tests/typing/core.py
+-rw-r--r--   0        0        0     1134 2023-08-06 06:51:14.000000 svcs-23.9.0/tests/typing/flask_.py
+-rw-r--r--   0        0        0      112 2023-08-06 06:51:14.000000 svcs-23.9.0/.gitignore
+-rw-r--r--   0        0        0     1098 2023-08-06 06:51:14.000000 svcs-23.9.0/LICENSE
+-rw-r--r--   0        0        0     4845 2023-08-06 06:51:14.000000 svcs-23.9.0/pyproject.toml
+-rw-r--r--   0        0        0     8706 2023-08-06 06:51:14.000000 svcs-23.9.0/PKG-INFO
```

### Comparing `svcs-23.8.0/.pre-commit-config.yaml` & `svcs-23.9.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `svcs-23.8.0/CHANGELOG.md` & `svcs-23.9.0/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -9,23 +9,42 @@
 The **third number** is for emergencies when we need to start branches for older releases.
 
 You can find our backwards-compatibility policy [here](https://github.com/hynek/svcs/blob/main/.github/SECURITY.md).
 
 <!-- changelog follows -->
 
 
+## [23.9.0](https://github.com/hynek/svcs/compare/23.8.0...23.9.0) - 2023-08-06
+
+### Changed
+
+- `Container.get()` and `Container.aget()` now have type hints that only work with concrete classes but allow for type checking without repeating yourself.
+  If you want to use abstract classes like `typing.Protocol` or ABCs, you can use `Container.get_abstract()` and `Container.aget_abstract()` instead.
+
+
+### Added
+
+- `Container.get_abstract()` and `Container.aget_abstract()`.
+  They behave like `Container.get()` and `Container.aget()` before.
+
+- It is now possible to check if a service type is registered with a `Registry` by using `in`.
+
+- It is now possible to check if a service type has a cached instance within a `Container` by using `in`.
+
+- `Registry` and `Container` are now also an (async) context managers that call `close()` / `aclose()` on exit automatically.
+
+
 ## [23.8.0](https://github.com/hynek/svcs/compare/23.7.0...23.8.0) - 2023-08-04
 
 ### Added
 
 - It's now possible to request multiple services at once by passing multiple types to `Container.get()` and `Container.aget()`.
   [#15](https://github.com/hynek/svcs/pull/15)
 
 
-
 ## [23.7.0](https://github.com/hynek/svcs/compare/23.6.0...23.7.0) - 2023-08-02
 
 ### Added
 
 - Factories now may take a parameter called `svcs_container` or that is annotated to be `svcs.Container`.
   In this case the factory will receive the current container as a first positional argument.
   This allows for recursive factories without global state.
```

### Comparing `svcs-23.8.0/README.md` & `svcs-23.9.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -63,23 +63,25 @@
 - simplifies **testing** through **loose coupling**,
 - and allows for easy **health checks** across *all* resources.
 
 The goal is to minimize your business code to:
 
 ```python
 def view(request):
-    db = request.services.get(Database)
-    api = request.services.get(WebAPIClient)
+    db = request.svcs.get(Database)
+    api = request.svcs.get(WebAPIClient)
 ```
 
-You can also ask for multiple services at once:
+With proper typing: `db` has the type `Database` and `api` has the type `WebAPIClient` to the type checker.
+
+You can also ask for multiple services at once with the same typing benefits:
 
 ```python
 def view(request):
-    db, api = request.services.get(Database, WebAPIClient)
+    db, api = request.svcs.get(Database, WebAPIClient)
 ```
 
 Or, if you don't shy away from some global state and your web framework supports it, even:
 
 ```python
 def view():
     db, api = svcs.flask.get(Database, WebAPIClient)
@@ -179,14 +181,20 @@
 >>> import svcs
 >>> import uuid
 
 >>> reg = svcs.Registry()
 
 >>> reg.register_factory(uuid.UUID, uuid.uuid4)
 >>> reg.register_value(str, "Hello World")
+>>> uuid.UUID in reg
+True
+>>> str in reg
+True
+>>> int in reg
+False
 ```
 
 The values and return values of the factories don't have to be actual instances of the type they're registered for.
 But the types must be *hashable* because they're used as keys in a lookup dictionary.
 
 It's possible to register a callback that is called when the *registry* is closed:
 
@@ -199,26 +207,31 @@
     Connection, connection_factory, on_registry_close=engine.dispose
 )
 ```
 
 If this callback fails, it's logged at warning level but otherwise ignored.
 For instance, you could free a database connection pool in an [`atexit` handler](https://docs.python.org/3/library/atexit.html).
 This frees you from keeping track of registered resources yourself.
+You can also use `Registry` as an (async) context manager that (a)closes automatically on exit.
 
 
 ### Containers
 
 A **`svcs.Container`** uses a `svcs.Registry` to lookup registered types and uses that information to create instances and to take care of their life cycles:
 
 ```python
 >>> container = svcs.Container(reg)
 
+>>> uuid.UUID in container
+False
 >>> u = container.get(uuid.UUID)
 >>> u
 UUID('...')
+>>> uuid.UUID in container
+True
 >>> # Calling get() again returns the SAME UUID instance!
 >>> # Good for DB connections, bad for UUIDs.
 >>> u is container.get(uuid.UUID)
 True
 >>> container.get(str)
 'Hello World'
 ```
@@ -255,14 +268,15 @@
 #### Cleanup
 
 If a factory is a [generator](https://docs.python.org/3/tutorial/classes.html#generators) and *yields* the instance instead of returning it, the generator will be remembered by the container.
 At the end, you run `container.close()` and all generators will be finished (i.e. called `next(factory)` again).
 You can use this to close files, return database connections to a pool, et cetera.
 
 If you have async generators, use `await container.aclose()` instead which calls `await anext(factory)` on all async generators (and `next(factory)` on sync ones).
+You can also use `Registry` as an (async) context manager that (a)closes automatically on exit.
 
 Failing cleanups are logged at `warning` level but otherwise ignored.
 
 **The key idea is that your business code doesn't have to care about cleaning up resources it has requested.**
 
 That makes it even easier to test it because the business codes makes fewer assumptions about the object it's getting.
 
@@ -489,38 +503,44 @@
 def index():
     conn: Connection = services.get(Connection)
 ```
 
 🧑‍🍳💋
 
 
-## Caveats
+## Typing Caveats
+
+If you try to `get()` an abstract class like an `Protocol` or an *abstract base classes* you'll get a Mypy error like this:
+
+```
+error: Only concrete class can be given where "type[P]" is expected  [type-abstract]
+```
 
-One would expect the the `Container.get()` method would have a type signature like `get(type: type[T]) -> T`.
-Unfortunately, that's currently impossible because it [precludes the usage of `Protocols` and *abstract base classes* as service types](https://github.com/python/mypy/issues/4717), making this package pointless.
+Unfortunately it's [impossible](https://github.com/python/mypy/issues/4717) to type-hint `type[P]` when `P` is abstract.
 
-Therefore it returns `Any`, and until Mypy changes its stance, you have to use it like this:
+As a stopgap, until we get something better in Python typing, *svcs* comes with `Container.get_abstract()` and `Container.aget_abstract()` that are type-hinted to return `Any`.
+Since `Any` disables any kind of type-checking, you have to use it like this:
 
 ```python
-conn: Connection = container.get(Connection)
+ac: SomeAbstractClass = container.get_abstract(SomeAbstractClass)
 ```
 
-If types are more important to you than a unified interface, you can always wrap it:
+You can also create quality-of-life wrappers for your resources:
 
 ```python
 def get_connection() -> Connection:
     return svcs.flask.get(Connection)
 ```
 
-Or, if you don't care about `Protocols` and abstract base classes:
+Sadly, this is the best compromise to date.
 
-```python
-def get(svc_type: type[T]) -> T:
-    return svcs.flask.get(svc_type)
-```
+---
+
+Another caveat is that it's necessary to define multiple return values for `get()` for every single arity.
+We've done it for up to ten service types which should be plenty.
 
 
 ## Credits
 
 *svcs* is written by [Hynek Schlawack](https://hynek.me/) and distributed under the terms of the [MIT](./LICENSE) license.
 
 The development is kindly supported by my employer [Variomedia AG](https://www.variomedia.de/) and all my amazing [GitHub Sponsors](https://github.com/sponsors/hynek).
```

### Comparing `svcs-23.8.0/conftest.py` & `svcs-23.9.0/conftest.py`

 * *Files identical despite different names*

### Comparing `svcs-23.8.0/tox.ini` & `svcs-23.9.0/tox.ini`

 * *Files identical despite different names*

### Comparing `svcs-23.8.0/.github/CODE_OF_CONDUCT.md` & `svcs-23.9.0/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `svcs-23.8.0/.github/SECURITY.md` & `svcs-23.9.0/.github/SECURITY.md`

 * *Files identical despite different names*

### Comparing `svcs-23.8.0/.github/workflows/ci.yml` & `svcs-23.9.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `svcs-23.8.0/.github/workflows/codeql-analysis.yml` & `svcs-23.9.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `svcs-23.8.0/.github/workflows/pypi-package.yml` & `svcs-23.9.0/.github/workflows/pypi-package.yml`

 * *Files identical despite different names*

### Comparing `svcs-23.8.0/src/svcs/__init__.py` & `svcs-23.9.0/src/svcs/__init__.py`

 * *Files identical despite different names*

### Comparing `svcs-23.8.0/tests/test_container.py` & `svcs-23.9.0/tests/test_container.py`

 * *Files 25% similar despite different names*

```diff
@@ -52,14 +52,64 @@
         registry.register_factory(AnotherService, async_factory)
 
         container.get(Service)
         await container.aget(AnotherService)
 
         assert "<Container(instantiated=2, cleanups=2)>" == repr(container)
 
+    def test_contains(self, container):
+        """
+        If a service is instantiated within a container, `in` returns True,
+        False otherwise.
+        """
+        container.registry.register_value(int, 42)
+
+        assert int not in container
+
+        container.get(int)
+
+        assert int in container
+
+    def test_context_manager(self, container):
+        """
+        The container is also a context manager that closes on exit.
+        """
+        closed = False
+
+        def factory():
+            yield 42
+            nonlocal closed
+            closed = True
+
+        container.registry.register_factory(int, factory)
+
+        with container:
+            assert 42 == container.get(int)
+
+        assert closed
+
+    @pytest.mark.asyncio()
+    async def test_async_context_manager(self, container):
+        """
+        The container is also an async context manager that acloses on exit.
+        """
+        closed = False
+
+        async def factory():
+            yield 42
+            nonlocal closed
+            closed = True
+
+        container.registry.register_factory(int, factory)
+
+        async with container:
+            assert 42 == await container.aget(int)
+
+        assert closed
+
 
 class TestServicePing:
     def test_name(self, rs):
         """
         The name property proxies the correct class name.
         """
```

### Comparing `svcs-23.8.0/tests/test_fake_factories.py` & `svcs-23.9.0/tests/test_fake_factories.py`

 * *Files identical despite different names*

### Comparing `svcs-23.8.0/tests/test_flask.py` & `svcs-23.9.0/tests/test_flask.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 @pytest.fixture(name="container")
 def _container(clean_app_ctx):
     return svcs.flask._ensure_req_data()[1]
 
 
 @pytest.mark.usefixtures("clean_app_ctx")
 class TestFlask:
-    def test_register_value_multiple(self, app, registry):
+    def test_register_value_multiple(self, registry):
         """
         register_value registers a service object on an app and get returns as
         many values as are requeste.
         """
         registry.register_value(Service, 1)
         registry.register_value(AnotherService, 2)
 
@@ -182,14 +182,27 @@
 
         assert 0 == len(wi.list)
         assert (
             "Skipped async cleanup for 'tests.ifaces.Service'. "
             "Use aclose() instead." == w.message.args[0]
         )
 
+    def test_register_factory_get_abstract(self, registry, container):
+        """
+        register_factory registers a factory and get_abstract returns the service.
+
+        The service is cached.
+        """
+        registry.register_factory(Interface, Service)
+
+        svc = container.get_abstract(Interface)
+
+        assert isinstance(svc, Interface)
+        assert svc is svcs.flask.get_abstract(Interface)
+
 
 class TestNonContextHelpers:
     def test_register_factory_helper(self, registry, app):
         """
         register_factory() registers a factory to the app that is passed.
         """
         svcs.flask.init_app(app, registry)
```

### Comparing `svcs-23.8.0/tests/test_integration.py` & `svcs-23.9.0/tests/test_integration.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import asyncio
 
 import pytest
 
 import svcs
 
 from .fake_factories import nop
-from .ifaces import AnotherService, Service, YetAnotherService
+from .ifaces import AnotherService, Interface, Service, YetAnotherService
 
 
 def test_register_factory_get(registry, container):
     """
     register_factory registers a factory and get returns the service.
 
     The service is cached.
@@ -22,14 +22,28 @@
 
     svc = container.get(Service)
 
     assert isinstance(svc, Service)
     assert svc is container.get(Service)
 
 
+def test_register_factory_get_abstract(registry, container):
+    """
+    register_factory registers a factory and get_abstract returns the service.
+
+    The service is cached.
+    """
+    registry.register_factory(Interface, Service)
+
+    svc = container.get_abstract(Interface)
+
+    assert isinstance(svc, Interface)
+    assert svc is container.get(Interface)
+
+
 def test_register_value_multiple(registry, container):
     """
     register_value registers a service object and get returns as many values as
     are requeste.
     """
     registry.register_value(Service, 1)
     registry.register_value(AnotherService, 2)
@@ -199,14 +213,24 @@
         """
         registry.register_value(Service, 42)
         registry.register_value(AnotherService, 23)
 
         assert [42, 23] == (await container.aget(Service, AnotherService))
         assert [42, 23] == (await container.aget(Service, AnotherService))
 
+    async def test_aget_abstract_works_with_value(self, registry, container):
+        """
+        A value instead of a factory does not break aget_abstract().
+        """
+        registry.register_value(int, 42)
+        registry.register_value(str, "42")
+
+        assert [42, "42"] == (await container.aget_abstract(int, str))
+        assert [42, "42"] == (await container.aget_abstract(int, str))
+
     async def test_async_cleanup(self, registry, container):
         """
         Async cleanups are handled by aclose.
         """
         cleaned_up = False
 
         async def factory():
```

### Comparing `svcs-23.8.0/tests/test_registry.py` & `svcs-23.9.0/tests/test_registry.py`

 * *Files 16% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
     def test_empty_close(self):
         """
         Closing an empty registry does nothing.
         """
         svcs.Registry().close()
 
-        with contextlib.closing(svcs.Registry()):
+        with svcs.Registry():
             ...
 
     def test_close_closes(self, registry):
         """
         Calling close on Registry runs all on_close callbacks.
         """
         close_1 = Mock()
@@ -107,19 +107,43 @@
         """
         Closing failures are logged but ignored.
         """
         registry.register_factory(
             Service, Service, on_registry_close=Mock(side_effect=ValueError())
         )
 
-        with contextlib.closing(registry):
+        with registry:
             ...
 
         assert "tests.ifaces.Service" == caplog.records[0].svcs_service_name
 
+    def test_context_manager(self):
+        """
+        The registry is also a context manager that closes on exit.
+        """
+        orc = Mock()
+
+        with svcs.Registry() as registry:
+            registry.register_factory(Service, Service, on_registry_close=orc)
+
+        orc.assert_called_once_with()
+
+    @needs_working_async_mock
+    @pytest.mark.asyncio()
+    async def test_async_context_manager(self):
+        """
+        The registry is also an async context manager that acloses on exit.
+        """
+        orc = AsyncMock()
+
+        async with svcs.Registry() as registry:
+            registry.register_factory(Service, Service, on_registry_close=orc)
+
+        orc.assert_awaited_once_with()
+
     def test_detects_async_factories(self, registry):
         """
         The is_async property of the RegisteredService is True if the factory
         needs to be awaited.
         """
 
         registry.register_factory(int, async_int_factory)
@@ -161,15 +185,15 @@
     @pytest.mark.asyncio()
     async def test_async_empty_close(self, registry):
         """
         Asynchronously closing an empty registry does nothing.
         """
         await registry.aclose()
 
-        async with contextlib.aclosing(svcs.Registry()):
+        async with svcs.Registry():
             ...
 
     @pytest.mark.asyncio()
     @needs_working_async_mock
     async def test_aclose_mixed(self, registry):
         """
         aclose() closes all services, including async ones.
@@ -205,14 +229,24 @@
         )
 
         await registry.aclose()
 
         close_mock.assert_awaited_once()
         assert "tests.ifaces.Service" == caplog.records[0].svcs_service_name
 
+    def test_contains(self, registry):
+        """
+        If a service is registered with a registry, `in` returns True, False
+        otherwise.
+        """
+        registry.register_factory(Service, Service)
+
+        assert Service in registry
+        assert AnotherService not in registry
+
 
 class TestRegisteredService:
     def test_repr(self, rs):
         """
         repr uses the fully-qualified name of a svc type.
         """
```

### Comparing `svcs-23.8.0/tests/typing/core.py` & `svcs-23.9.0/tests/typing/core.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,31 +1,51 @@
 # SPDX-FileCopyrightText: 2023 Hynek Schlawack <hs@ox.cx>
 #
 # SPDX-License-Identifier: MIT
 
 import contextlib
 import sys
 
-from typing import AsyncGenerator, Generator
+from typing import AsyncGenerator, Generator, Protocol
 
 import svcs
 
 
 reg = svcs.Registry()
 con = svcs.Container(reg)
 
 reg.close()
 with contextlib.closing(reg) as reg:
     ...
+with reg as reg:
+    reg.register_factory(int, int)
 
 
-async def f() -> None:
+async def func() -> None:
     await reg.aclose()
     await con.aclose()
 
+    async with svcs.Registry() as reg2:
+        reg2.register_factory(int, int)
+
+        async with svcs.Container(reg2) as con2:
+            a: int
+            b: str
+            c: bool
+            d: tuple
+            e: object
+            f: float
+            g: list
+            h: dict
+            i: set
+            j: bytes
+            a, b, c, d, e, f, g, h, i, j = await con2.aget(
+                int, str, bool, tuple, object, float, list, dict, set, bytes
+            )
+
 
 def gen() -> Generator:
     yield 42
 
 
 async def async_gen() -> AsyncGenerator:
     yield 42
@@ -54,23 +74,46 @@
 reg.register_value(str, str, ping=lambda: None)
 reg.register_value(str, async_gen)
 
 con = svcs.Container(reg)
 
 # The type checker believes whatever we tell it.
 o1: object = con.get(object)
-o2: int = con.get(object)
+o2: int = con.get(int)
+
+a: int
+b: str
+c: bool
+d: tuple
+e: object
+f: float
+g: list
+h: dict
+i: set
+j: bytes
+a, b, c, d, e, f, g, h, i, j = con.get(
+    int, str, bool, tuple, object, float, list, dict, set, bytes
+)
+
+
+class P(Protocol):
+    def m(self) -> None:
+        ...
 
-o, i = con.get(object, int)
+
+p: P = con.get_abstract(P)
 
 con.close()
 
 with contextlib.closing(svcs.Container(reg)) as con:
     ...
 
+with svcs.Container(reg) as con:
+    i2: int = con.get(int)
+
 if sys.version_info >= (3, 10):
 
     async def ctx() -> None:
         async with contextlib.aclosing(svcs.Container(reg)):
             ...
 
         async with contextlib.aclosing(svcs.Registry()):
```

### Comparing `svcs-23.8.0/LICENSE` & `svcs-23.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `svcs-23.8.0/pyproject.toml` & `svcs-23.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `svcs-23.8.0/PKG-INFO` & `svcs-23.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: svcs
-Version: 23.8.0
+Version: 23.9.0
 Summary: A Lightweight Service Locator
 Project-URL: Changelog, https://github.com/hynek/svcs/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://github.com/hynek/svcs/blob/main/README.md
 Project-URL: Source, https://github.com/hynek/svcs
 Project-URL: Funding, https://github.com/sponsors/hynek
 Author-email: Hynek Schlawack <hs@ox.cx>
 License-Expression: MIT
@@ -77,23 +77,25 @@
 - simplifies **testing** through **loose coupling**,
 - and allows for easy **health checks** across *all* resources.
 
 The goal is to minimize your business code to:
 
 ```python
 def view(request):
-    db = request.services.get(Database)
-    api = request.services.get(WebAPIClient)
+    db = request.svcs.get(Database)
+    api = request.svcs.get(WebAPIClient)
 ```
 
-You can also ask for multiple services at once:
+With proper typing: `db` has the type `Database` and `api` has the type `WebAPIClient` to the type checker.
+
+You can also ask for multiple services at once with the same typing benefits:
 
 ```python
 def view(request):
-    db, api = request.services.get(Database, WebAPIClient)
+    db, api = request.svcs.get(Database, WebAPIClient)
 ```
 
 Or, if you don't shy away from some global state and your web framework supports it, even:
 
 ```python
 def view():
     db, api = svcs.flask.get(Database, WebAPIClient)
@@ -174,19 +176,30 @@
 ---
 
 For now, please refer to the [GitHub README](https://github.com/hynek/svcs/blob/main/README.md) for latest documentation.
 
 
 ## Release Information
 
+### Changed
+
+- `Container.get()` and `Container.aget()` now have type hints that only work with concrete classes but allow for type checking without repeating yourself.
+  If you want to use abstract classes like `typing.Protocol` or ABCs, you can use `Container.get_abstract()` and `Container.aget_abstract()` instead.
+
+
 ### Added
 
-- It's now possible to request multiple services at once by passing multiple types to `Container.get()` and `Container.aget()`.
-  [#15](https://github.com/hynek/svcs/pull/15)
+- `Container.get_abstract()` and `Container.aget_abstract()`.
+  They behave like `Container.get()` and `Container.aget()` before.
+
+- It is now possible to check if a service type is registered with a `Registry` by using `in`.
+
+- It is now possible to check if a service type has a cached instance within a `Container` by using `in`.
 
+- `Registry` and `Container` are now also an (async) context managers that call `close()` / `aclose()` on exit automatically.
 
 
 ---
 
 [→ Full Changelog](https://github.com/hynek/svcs/blob/main/CHANGELOG.md)
```

