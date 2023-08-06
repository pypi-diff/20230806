# Comparing `tmp/whoisdomain-1.20230804.2.tar.gz` & `tmp/whoisdomain-1.20230806.1.tar.gz`

## Comparing `whoisdomain-1.20230804.2.tar` & `whoisdomain-1.20230806.1.tar`

### file list

```diff
@@ -1,18 +1,25 @@
--rwxr-xr-x   0        0        0     4823 2020-02-02 00:00:00.000000 whoisdomain-1.20230804.2/whoisdomain/_0_init_tld.py
--rwxr-xr-x   0        0        0     2261 2020-02-02 00:00:00.000000 whoisdomain-1.20230804.2/whoisdomain/__init__.py
--rwxr-xr-x   0        0        0    10362 2020-02-02 00:00:00.000000 whoisdomain-1.20230804.2/whoisdomain/doParse.py
--rw-r--r--   0        0        0    10047 2020-02-02 00:00:00.000000 whoisdomain-1.20230804.2/whoisdomain/doQuery.py
--rwxr-xr-x   0        0        0     6427 2020-02-02 00:00:00.000000 whoisdomain-1.20230804.2/whoisdomain/doWhoisCommand.py
--rwxr-xr-x   0        0        0     4753 2020-02-02 00:00:00.000000 whoisdomain-1.20230804.2/whoisdomain/domain.py
--rwxr-xr-x   0        0        0      544 2020-02-02 00:00:00.000000 whoisdomain-1.20230804.2/whoisdomain/exceptions.py
--rw-r--r--   0        0        0     5149 2020-02-02 00:00:00.000000 whoisdomain-1.20230804.2/whoisdomain/handleDateStrings.py
--rwxr-xr-x   0        0        0    19563 2020-02-02 00:00:00.000000 whoisdomain-1.20230804.2/whoisdomain/main.py
--rwxr-xr-x   0        0        0     6022 2020-02-02 00:00:00.000000 whoisdomain-1.20230804.2/whoisdomain/parameterContext.py
--rwxr-xr-x   0        0        0     1744 2020-02-02 00:00:00.000000 whoisdomain-1.20230804.2/whoisdomain/simpleCacheBase.py
--rwxr-xr-x   0        0        0     2279 2020-02-02 00:00:00.000000 whoisdomain-1.20230804.2/whoisdomain/simpleCacheWithFile.py
--rwxr-xr-x   0        0        0   131854 2020-02-02 00:00:00.000000 whoisdomain-1.20230804.2/whoisdomain/tld_regexpr.py
--rwxr-xr-x   0        0        0       25 2020-02-02 00:00:00.000000 whoisdomain-1.20230804.2/whoisdomain/version.py
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 whoisdomain-1.20230804.2/.gitignore
--rw-r--r--   0        0        0    10918 2020-02-02 00:00:00.000000 whoisdomain-1.20230804.2/README.md
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 whoisdomain-1.20230804.2/pyproject.toml
--rw-r--r--   0        0        0    11841 2020-02-02 00:00:00.000000 whoisdomain-1.20230804.2/PKG-INFO
+-rwxr-xr-x   0        0        0     4823 2020-02-02 00:00:00.000000 whoisdomain-1.20230806.1/whoisdomain/_0_init_tld.py
+-rwxr-xr-x   0        0        0     2486 2020-02-02 00:00:00.000000 whoisdomain-1.20230806.1/whoisdomain/__init__.py
+-rwxr-xr-x   0        0        0     2331 2020-02-02 00:00:00.000000 whoisdomain-1.20230806.1/whoisdomain/doParse.py
+-rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 whoisdomain-1.20230806.1/whoisdomain/doQuery.py
+-rwxr-xr-x   0        0        0     1860 2020-02-02 00:00:00.000000 whoisdomain-1.20230806.1/whoisdomain/doWhoisCommand.py
+-rwxr-xr-x   0        0        0     4753 2020-02-02 00:00:00.000000 whoisdomain-1.20230806.1/whoisdomain/domain.py
+-rwxr-xr-x   0        0        0      544 2020-02-02 00:00:00.000000 whoisdomain-1.20230806.1/whoisdomain/exceptions.py
+-rw-r--r--   0        0        0     5149 2020-02-02 00:00:00.000000 whoisdomain-1.20230806.1/whoisdomain/handleDateStrings.py
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 whoisdomain-1.20230806.1/whoisdomain/lastWhois.py
+-rwxr-xr-x   0        0        0    19904 2020-02-02 00:00:00.000000 whoisdomain-1.20230806.1/whoisdomain/main.py
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 whoisdomain-1.20230806.1/whoisdomain/noneStrings.py
+-rwxr-xr-x   0        0        0     6022 2020-02-02 00:00:00.000000 whoisdomain-1.20230806.1/whoisdomain/parameterContext.py
+-rw-r--r--   0        0        0     8429 2020-02-02 00:00:00.000000 whoisdomain-1.20230806.1/whoisdomain/processWhoisDomainRequest.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 whoisdomain-1.20230806.1/whoisdomain/quotaStrings.py
+-rwxr-xr-x   0        0        0     1498 2020-02-02 00:00:00.000000 whoisdomain-1.20230806.1/whoisdomain/simpleCacheBase.py
+-rwxr-xr-x   0        0        0     1681 2020-02-02 00:00:00.000000 whoisdomain-1.20230806.1/whoisdomain/simpleCacheWithFile.py
+-rwxr-xr-x   0        0        0   131874 2020-02-02 00:00:00.000000 whoisdomain-1.20230806.1/whoisdomain/tld_regexpr.py
+-rwxr-xr-x   0        0        0       25 2020-02-02 00:00:00.000000 whoisdomain-1.20230806.1/whoisdomain/version.py
+-rwxr-xr-x   0        0        0     6141 2020-02-02 00:00:00.000000 whoisdomain-1.20230806.1/whoisdomain/whoisCliInterface.py
+-rwxr-xr-x   0        0        0     8786 2020-02-02 00:00:00.000000 whoisdomain-1.20230806.1/whoisdomain/whoisParser.py
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 whoisdomain-1.20230806.1/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 whoisdomain-1.20230806.1/LICENSE
+-rw-r--r--   0        0        0    11307 2020-02-02 00:00:00.000000 whoisdomain-1.20230806.1/README.md
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 whoisdomain-1.20230806.1/pyproject.toml
+-rw-r--r--   0        0        0    12252 2020-02-02 00:00:00.000000 whoisdomain-1.20230806.1/PKG-INFO
```

### Comparing `whoisdomain-1.20230804.2/whoisdomain/_0_init_tld.py` & `whoisdomain-1.20230806.1/whoisdomain/_0_init_tld.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230804.2/whoisdomain/__init__.py` & `whoisdomain-1.20230806.1/whoisdomain/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,28 +28,23 @@
 from ._0_init_tld import (
     TLD_RE,
     validTlds,
     filterTldToSupportedPattern,
     mergeExternalDictWithRegex,
 )
 
-from .doQuery import (
-    query,
-    get_last_raw_whois_data,
-)
-
-from .doWhoisCommand import (
-    CACHE_STUB,
-)
+from .doQuery import query, q2
+from .lastWhois import get_last_raw_whois_data
+from .doWhoisCommand import CACHE_STUB
+from .noneStrings import NoneStrings, NoneStringsAdd
+from .quotaStrings import QuotaStrings, QuotaStringsAdd
+from .simpleCacheBase import SimpleCacheBase
+from .simpleCacheWithFile import SimpleCacheWithFile
 
 from .doParse import (
-    NoneStrings,
-    NoneStringsAdd,
-    QuotaStrings,
-    QuotaStringsAdd,
     cleanupWhoisResponse,
 )
 
 from .tld_regexpr import ZZ
 from .domain import Domain
 from .parameterContext import ParameterContext
 
@@ -75,26 +70,30 @@
     "TLD_RE",
     # from version
     "VERSION",
     # from parameterContext
     "ParameterContext",
     # from doQuery
     "query",
+    "q2",
     "get_last_raw_whois_data",
     # fromm this file
     "getVersion",
     "getTestHint",
     # from doWhoisCommand
     "CACHE_STUB",  # to build your own caching interface
     # from doParse
     "NoneStrings",
     "NoneStringsAdd",
     "QuotaStrings",
     "QuotaStringsAdd",
     "cleanupWhoisResponse",  # we will drop this most likely
+    # from simpleCacheWithFile
+    "SimpleCacheBase",
+    "SimpleCacheWithFile",
 ]
 
 
 def _result2dict(func: Any) -> Any:
     @wraps(func)
     def _inner(*args: str, **kw: Any) -> Dict[str, Any]:
         r = func(*args, **kw)
```

### Comparing `whoisdomain-1.20230804.2/whoisdomain/domain.py` & `whoisdomain-1.20230806.1/whoisdomain/domain.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230804.2/whoisdomain/exceptions.py` & `whoisdomain-1.20230806.1/whoisdomain/exceptions.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230804.2/whoisdomain/handleDateStrings.py` & `whoisdomain-1.20230806.1/whoisdomain/handleDateStrings.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230804.2/whoisdomain/main.py` & `whoisdomain-1.20230806.1/whoisdomain/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,27 +211,38 @@
     global SIMPLISTIC
     global WithRedacted
     global TestAllTld
     global TestRunOnly
 
     timeout = 30  # seconds
 
-    w = whois.query(
-        d,
+    withCacheTest: bool = False
+    if withCacheTest:
+        # test passing pre initialized caching stub
+        cache_file = "/tmp/testCache.json"
+        cache_age = 300
+        whois.CACHE_STUB = whois.SimpleCacheWithFile(
+            verbose=Verbose,
+            cacheFilePath=cache_file,
+            cacheMaxAge=cache_age,
+        )
+
+    pc = whois.ParameterContext(
         ignore_returncode=IgnoreReturncode,
         verbose=Verbose,
         internationalized=True,
         include_raw_whois_text=PrintGetRawWhoisResult,
-        timeout=timeout,
+        timeout=float(timeout),
         simplistic=SIMPLISTIC,
         withRedacted=WithRedacted,
-        # cache_file="/tmp/testCache.json",  # temp test
-        # cache_age=300,  # temp test
     )
 
+    # use the new query (can also simply use q2()
+    w = whois.query(domain=d, pc=pc)
+
     if w is None:
         print("None")
         print("\n", whois.get_last_raw_whois_data())
         return
 
     # the 3 date time items can be None if not present or a datetime string
     # dnssec is a bool
```

### Comparing `whoisdomain-1.20230804.2/whoisdomain/parameterContext.py` & `whoisdomain-1.20230806.1/whoisdomain/parameterContext.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230804.2/whoisdomain/simpleCacheBase.py` & `whoisdomain-1.20230806.1/whoisdomain/simpleCacheBase.py`

 * *Files 13% similar despite different names*

```diff
@@ -21,60 +21,47 @@
         verbose: bool = False,
         cacheMaxAge: int = (60 * 60 * 48),
     ) -> None:
         self.verbose = verbose
         self.memCache = {}
         self.cacheMaxAge = cacheMaxAge
 
-    def cachePut(
+    def put(
         self,
         keyString: str,
         data: str,
-    ) -> None:
+    ) -> str:
         if self.verbose:
-            print(f"cachePut: {keyString}", file=sys.stderr)
+            print(f"put: {keyString}", file=sys.stderr)
 
         # store the currentTime and data tuple (time, data)
         self.memCache[keyString] = (
             int(time.time()),
             data,
         )
+        return data
 
-    def cacheGet(
-        self,
-        keyString: str,
-    ) -> Optional[Tuple[float, str]]:
-        if self.verbose:
-            print(f"cacheGet: {keyString}", file=sys.stderr)
-
-        return self.memCache.get(keyString)
-
-    def cacheGetData(
+    def get(
         self,
         keyString: str,
     ) -> Optional[str]:
-        if self.verbose:
-            print(f"cacheGetData: {keyString}", file=sys.stderr)
-
-        tData: Optional[Tuple[float, str]] = self.cacheGet(keyString)
-        if tData is None:
-            return None
-
-        return tData[1]
-
-    def cacheExpired(
-        self,
-        keyString: str,
-    ) -> Optional[bool]:
-        if self.verbose:
-            print(f"cacheExpired: {keyString}", file=sys.stderr)
 
         cData = self.memCache.get(keyString)
         if cData is None:
+            if self.verbose:
+                print(f"get: no data for {keyString}", file=sys.stderr)
+            return None
+
+        t = time.time()
+        hasExpired = cData[0] < (t - self.cacheMaxAge)
+        if hasExpired is True:
+            if self.verbose:
+                print(f"get: data has expired {keyString} {cData[0]}, {t}, {self.cacheMaxAge}", file=sys.stderr)
             return None
 
-        hasExpired = cData[0] < (time.time() - self.cacheMaxAge)
-        return hasExpired
+        if self.verbose:
+            print(f"get: {keyString}", file=sys.stderr)
+        return cData[1]
 
 
 if __name__ == "__main__":
     pass
```

### Comparing `whoisdomain-1.20230804.2/whoisdomain/simpleCacheWithFile.py` & `whoisdomain-1.20230806.1/whoisdomain/simpleCacheWithFile.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import sys
 import os
 import json
 
 
 from typing import (
     Optional,
-    Tuple,
+    # Tuple,
 )
 
 from .simpleCacheBase import (
     SimpleCacheBase,
 )
 
 
@@ -23,77 +23,56 @@
         verbose: bool = False,
         cacheFilePath: Optional[str] = None,
         cacheMaxAge: int = (60 * 60 * 48),
     ) -> None:
         super().__init__(verbose=verbose, cacheMaxAge=cacheMaxAge)
         self.cacheFilePath = cacheFilePath
 
-    def _cacheFileLoad(
+    def _fileLoad(
         self,
     ) -> None:
         if self.cacheFilePath is None:
             return
 
         if not os.path.isfile(self.cacheFilePath):
             return
 
         if self.verbose:
-            print(f"cacheFileLoad: {self.cacheFilePath}", file=sys.stderr)
+            print(f"fileLoad: {self.cacheFilePath}", file=sys.stderr)
 
         with open(self.cacheFilePath, "r") as f:
             try:
                 self.memCache = json.load(f)
             except Exception as e:
                 print(f"ignore json load err: {e}", file=sys.stderr)
 
-    def _cacheFileSave(
+    def _fileSave(
         self,
     ) -> None:
         if self.cacheFilePath is None:
             return
 
         if self.verbose:
-            print(f"_cacheFileSave: {self.cacheFilePath}", file=sys.stderr)
+            print(f"_fileSave: {self.cacheFilePath}", file=sys.stderr)
 
         with open(self.cacheFilePath, "w") as f:
             json.dump(self.memCache, f)
 
-    def cachePut(
+    def put(
         self,
         keyString: str,
         data: str,
-    ) -> None:
-        super().cachePut(keyString=keyString, data=data)
-        self._cacheFileSave()
-
-    def cacheGet(
-        self,
-        keyString: str,
-    ) -> Optional[Tuple[float, str]]:
-        self._cacheFileLoad()
-        return super().cacheGet(keyString=keyString)
+    ) -> str:
+        super().put(keyString=keyString, data=data)
+        self._fileSave()
+        return data
 
-    def cacheExpired(
-        self,
-        keyString: str,
-    ) -> Optional[bool]:
-        if keyString not in self.memCache:
-            self.cacheGet(keyString=keyString)
-
-        return super().cacheExpired(keyString=keyString)
-
-    def cacheGetData(
+    def get(
         self,
         keyString: str,
     ) -> Optional[str]:
-        if self.verbose:
-            print(f"cacheGetData: {keyString}", file=sys.stderr)
-
-        tData: Optional[Tuple[float, str]] = self.cacheGet(keyString)
-        if tData is None:
-            return None
-
-        return tData[1]
+        self._fileLoad()
+        return super().get(keyString=keyString)
 
 
 if __name__ == "__main__":
     pass
```

### Comparing `whoisdomain-1.20230804.2/whoisdomain/tld_regexpr.py` & `whoisdomain-1.20230806.1/whoisdomain/tld_regexpr.py`

 * *Files 0% similar despite different names*

```diff
@@ -779,14 +779,15 @@
     "expiration_date": None,
     "registrant_country": None,
     "domain_name": r"Domain name:\s?(.+)",
     "name_servers": r"Domain nameservers.*:\n%s" % xStr(r"(?:\s+(\S+)\n)?", 10),
     "reseller": r"Reseller:\s?(.+)",
     "abuse_contact": r"Abuse Contact:\s?(.+)",
     "_test": "google.nl",
+    "_slowdown": 5,
 }
 
 # Norway
 ZZ["no"] = {
     "extend": None,
     "domain_name": r"Domain Name\.+:\s?(.+)",
     "registrar": r"Registrar Handle\.+:\s?(.+)",
```

### Comparing `whoisdomain-1.20230804.2/.gitignore` & `whoisdomain-1.20230806.1/.gitignore`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230804.2/README.md` & `whoisdomain-1.20230806.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -220,8 +220,12 @@
   * renaming various vars to mak them more verbose
   * preparing for capturing all parameters in one object and parring that object around instead of many arguments in methods/functions
   * switch to json so we dont need a additional dependency in ParamContext
   * finish rework args to ParameterContext, split of domain as file
   * 1.20230803.1 frenzy refactor-release
   * 1.20230804.1 testing
   * 1.20230804.2 testing after remove of leading dot in rw second level domains
-
+  * 1.20230804.3 simplefy cache implementation after feedback from `baderdean`
+  * "more lembas bread", refactor parse and query
+  * remove option to typecheck CACHE_STUB, use try/catch/exit instead, does not work when timout happens, removed ;-(
+  * refactor doQuery create processWhoisDomainRequest, split of lastWhois
+  * 1.20230806.1 testing done, prep new release: "more lembas bread"
```

### Comparing `whoisdomain-1.20230804.2/pyproject.toml` & `whoisdomain-1.20230806.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230804.2/PKG-INFO` & `whoisdomain-1.20230806.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: whoisdomain
-Version: 1.20230804.2
+Version: 1.20230806.1
 Summary: Python package for retrieving WHOIS information of domains.
 Project-URL: Bug Tracker, https://github.com/mboot-github/WhoisDomain/issues
 Project-URL: Home Page, https://github.com/mboot-github/WhoisDomain/
 Project-URL: Repository, https://github.com/mboot-github/WhoisDomain/
 Author: DannyCork
 Maintainer-email: Maarten Boot <130295084+mboot-github@users.noreply.github.com>
 License-Expression: MIT
+License-File: LICENSE
 Keywords: Python,cctld,domain,expiration,registrar,tld,whois
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Internet
@@ -241,8 +242,12 @@
   * renaming various vars to mak them more verbose
   * preparing for capturing all parameters in one object and parring that object around instead of many arguments in methods/functions
   * switch to json so we dont need a additional dependency in ParamContext
   * finish rework args to ParameterContext, split of domain as file
   * 1.20230803.1 frenzy refactor-release
   * 1.20230804.1 testing
   * 1.20230804.2 testing after remove of leading dot in rw second level domains
-
+  * 1.20230804.3 simplefy cache implementation after feedback from `baderdean`
+  * "more lembas bread", refactor parse and query
+  * remove option to typecheck CACHE_STUB, use try/catch/exit instead, does not work when timout happens, removed ;-(
+  * refactor doQuery create processWhoisDomainRequest, split of lastWhois
+  * 1.20230806.1 testing done, prep new release: "more lembas bread"
```

