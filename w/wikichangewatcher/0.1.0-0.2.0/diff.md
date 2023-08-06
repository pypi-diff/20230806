# Comparing `tmp/wikichangewatcher-0.1.0-py3-none-any.whl.zip` & `tmp/wikichangewatcher-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 11713 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat      486 b- defN 23-Jul-31 03:08 wikichangewatcher/__init__.py
--rw-rw-rw-  2.0 fat    10526 b- defN 23-Jul-31 01:46 wikichangewatcher/wikichangewatcher.py
--rw-rw-rw-  2.0 fat    10761 b- defN 23-Jul-31 03:11 wikichangewatcher-0.1.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    16417 b- defN 23-Jul-31 03:11 wikichangewatcher-0.1.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-31 03:11 wikichangewatcher-0.1.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       18 b- defN 23-Jul-31 03:11 wikichangewatcher-0.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      619 b- defN 23-Jul-31 03:11 wikichangewatcher-0.1.0.dist-info/RECORD
-7 files, 38919 bytes uncompressed, 10607 bytes compressed:  72.7%
+Zip file size: 11888 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat      498 b- defN 23-Aug-06 18:46 wikichangewatcher/__init__.py
+-rw-rw-rw-  2.0 fat    12743 b- defN 23-Aug-06 18:09 wikichangewatcher/wikichangewatcher.py
+-rw-rw-rw-  2.0 fat    10761 b- defN 23-Aug-06 18:54 wikichangewatcher-0.2.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    16752 b- defN 23-Aug-06 18:54 wikichangewatcher-0.2.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-06 18:54 wikichangewatcher-0.2.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       18 b- defN 23-Aug-06 18:54 wikichangewatcher-0.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      619 b- defN 23-Aug-06 18:54 wikichangewatcher-0.2.0.dist-info/RECORD
+7 files, 41483 bytes uncompressed, 10782 bytes compressed:  74.0%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: wikichangewatcher/__init__.py
 Comment: 
 
 Filename: wikichangewatcher/wikichangewatcher.py
 Comment: 
 
-Filename: wikichangewatcher-0.1.0.dist-info/LICENSE
+Filename: wikichangewatcher-0.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: wikichangewatcher-0.1.0.dist-info/METADATA
+Filename: wikichangewatcher-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: wikichangewatcher-0.1.0.dist-info/WHEEL
+Filename: wikichangewatcher-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: wikichangewatcher-0.1.0.dist-info/top_level.txt
+Filename: wikichangewatcher-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: wikichangewatcher-0.1.0.dist-info/RECORD
+Filename: wikichangewatcher-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## wikichangewatcher/__init__.py

```diff
@@ -1,7 +1,7 @@
-__version__ = "0.1.0"
+__version__ = "0.2.0"
 
-from wikichangewatcher.wikichangewatcher import FieldFilter, FilterCollection, IpV4Filter, WikiChangeWatcher, MatchType
+from wikichangewatcher.wikichangewatcher import FieldFilter, FilterCollection, IpV4Filter, IpV6Filter, WikiChangeWatcher, MatchType
 from wikichangewatcher.wikichangewatcher import FieldStringFilter, FieldRegexMatchFilter, FieldRegexSearchFilter
 from wikichangewatcher.wikichangewatcher import UsernameFilter, UsernameRegexMatchFilter, UsernameRegexSearchFilter
 from wikichangewatcher.wikichangewatcher import PageUrlFilter, PageUrlRegexMatchFilter, PageUrlRegexSearchFilter
```

## wikichangewatcher/wikichangewatcher.py

```diff
@@ -143,14 +143,86 @@
 
             elif self.ip_addr_pattern[i] != fields[i]:
                 return False
 
         return True
 
 
+def _ipv6_field_tostr(stringval: str) -> int:
+    intval = int(stringval, 16)
+    if not (0 <= intval <= 65535):
+        raise ValueError
+
+    return intval
+
+
+class IpV6Filter(FieldFilter):
+    """
+    FieldWatcher implementation to watch for "user" fields that contain IPv6 addresses
+    in the specified ranges
+    """
+    def __init__(self, ip_addr_pattern="*:*:*:*:*:*:*:*"):
+        super(IpV6Filter, self).__init__()
+        self.ip_addr_pattern = []
+
+        for x in ip_addr_pattern.split(":"):
+            error = False
+
+            if x == "*":
+                self.ip_addr_pattern.append(None)
+            else:
+                ranges = x.split('-')
+                if len(ranges) == 2:
+                    try:
+                        self.ip_addr_pattern.append((_ipv6_field_tostr(ranges[0]), _ipv6_field_tostr(ranges[1])))
+                    except ValueError:
+                        error = True
+
+                else:
+                    try:
+                        self.ip_addr_pattern.append(_ipv6_field_tostr(x))
+                    except ValueError:
+                        error = True
+
+            if error:
+                raise ValueError(f"Invalid field '{x}' in IP address pattern '{ip_addr_pattern}'")
+
+        if len(self.ip_addr_pattern) != 8:
+            raise ValueError(f"Invalid number of fields ({len(self.ip_addr_pattern)}) for IP address pattern (expected 8)")
+
+    def _handler(self, json_data: dict) -> bool:
+        if "user" not in json_data:
+            return False
+
+        ipaddr = json_data["user"]
+
+        try:
+            fields = [int(x, 16) for x in ipaddr.split(":")]
+        except ValueError:
+            return False
+
+        if len(fields) != 8:
+            return False
+
+        for i in range(len(fields)):
+            if self.ip_addr_pattern[i] is None:
+                continue
+
+            elif type(self.ip_addr_pattern[i]) == tuple:
+                range_lo = self.ip_addr_pattern[i][0]
+                range_hi = self.ip_addr_pattern[i][1]
+                if (fields[i] < range_lo) or (fields[i] > range_hi):
+                    return False
+
+            elif self.ip_addr_pattern[i] != fields[i]:
+                return False
+
+        return True
+
+
 class FieldStringFilter(FieldFilter):
     """
     FieldFilter implementation to watch for a named field with a specific fixed string
     """
     def __init__(self, fieldname: str, value: str):
         super(FieldStringFilter, self).__init__()
         self.fieldname = fieldname
```

## Comparing `wikichangewatcher-0.1.0.dist-info/LICENSE` & `wikichangewatcher-0.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `wikichangewatcher-0.1.0.dist-info/METADATA` & `wikichangewatcher-0.2.0.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wikichangewatcher
-Version: 0.1.0
+Version: 0.2.0
 Summary: Real-time monitoring/filtering of global Wikipedia page edits
 Home-page: http://github.com/eriknyquist/wikichangewatcher
 Author: Erik Nyquist
 Author-email: eknyquist@gmail.com
 License: Apache 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -18,20 +18,20 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 License-File: LICENSE
 Requires-Dist: sseclient
 
-WikiChangeWatcher
-=================
+WikiChangeWatcher 0.2.0
+=======================
 
-.. contents:: Table of Contents
+.. image:: images/wikiwatcher_github_banner.png
 
-.. image:: https://github.com/eriknyquist/wikichangewatcher/blob/80ffe25fd4d0d694bba545bd46dcc31a37d664e7/images/wikiwatcher_logo.png
+.. contents:: Table of Contents
 
 Introduction
 ============
 
 Wikipedia provides an `SSE Stream <https://en.wikipedia.org/wiki/Server-sent_events>`_  of
 all edits made to any page across Wikipedia, which allows you to watch all edits made to all wikipedia
 pages in real time.
@@ -66,32 +66,31 @@
 
 .. code:: python
 
     # Example script showing how to use WikiChangeWatcher to watch for "anonymous" edits to any
     # wikipedia page from specific IP address ranges
 
     import time
-    from wikichangewatcher import WikiChangeWatcher, IpV4Filter
+    from wikichangewatcher import WikiChangeWatcher, IpV4Filter, IpV6Filter
 
     # Callback function to run whenever an event matching our IPv4 address pattern is seen
     def match_handler(json_data):
         """
         json_data is a JSON-encoded event from the WikiMedia "recent changes" event stream,
         as described here: https://www.mediawiki.org/wiki/Manual:RCFeed
         """
         print("{user} edited {title_url}".format(**json_data))
 
     # Watch for anonymous edits from some specific IP address ranges
     wc = WikiChangeWatcher(IpV4Filter("192.60.38.225-230").on_match(match_handler),
-                           IpV4Filter("194.60.38.200-205").on_match(match_handler),
-                           IpV4Filter("194.60.38.215-219").on_match(match_handler))
+                           IpV6Filter("2601:205:4882:810:5D1D:BC41:61BB:0-ffff").on_match(match_handler))
 
-    # You can also use the wildcard '*' character within IP addresses; the following line
-    # sets up a watcher that triggers on any IP address (all anonymous edits)
-    #wc = WikiChangeWatcher(IpV4Filter("*.*.*.*").on_match(match_handler))
+    # Wildcard '*' character can be used in place of a IPv4 or IP46 address field, to ignore that field entirely.
+    # IPV6 filter with some fields ignored: IpV6Filter("*:*:*:810:5D1D:BC41:*:0-ffff")
+    # IPV6 filter with some fields ignored: IpV4Filter("192.*.*.225-230")
 
     wc.run()
 
     # Watch for page edits forever until KeyboardInterrupt
     try:
         while True:
             time.sleep(0.1)
@@ -272,49 +271,50 @@
 
 .. code:: python
 
     # Example script showing how to use WikiChangeWatcher to watch for "anonymous" edits to any
     # wikipedia page from IP address ranges that are publicly listed as being owned by various US government departments
 
     import time
-    from wikichangewatcher import WikiChangeWatcher, IpV4Filter, FilterCollection, MatchType
+    from wikichangewatcher import WikiChangeWatcher, FilterCollection, IpV4Filter, IpV6Filter, MatchType
 
     # Callback function to run whenever an event matching one of our IPv4 address ranges is seen
     def match_handler(json_data):
         """
         json_data is a JSON-encoded event from the WikiMedia "recent changes" event stream,
         as described here: https://www.mediawiki.org/wiki/Manual:RCFeed
         """
         print("{user} edited {title_url}".format(**json_data))
 
-    filters = [
-        IpV4Filter("136.200.0-255.0-255").on_match(match_handler),  # IP range assigned to CA dept. of water resources
-        IpV4Filter("151.143.0-255.0-255").on_match(match_handler),  # IP range assigned to CA dept. of technology
-        IpV4Filter("160.88.0-255.0-255").on_match(match_handler),   # IP range assigned to CA dept. of insurance
-        IpV4Filter("192.56.110.0-255").on_match(match_handler),     # IP range #1 assigned to CA dept. of corrections
-        IpV4Filter("153.48.0-255.0-255").on_match(match_handler),   # IP range #2 assigned to CA dept. of corrections
-        IpV4Filter("149.136.0-255.0-255").on_match(match_handler),  # IP range assigned to CA dept. of transportation
-        IpV4Filter("192.251.92.0-255").on_match(match_handler),     # IP range assigned to CA dept. of general services
-        IpV4Filter("159.145.0-255.0-255").on_match(match_handler),  # IP range assigned to CA dept. of consumer affairs
-        IpV4Filter("167.10.0-255.0-255").on_match(match_handler),   # IP range assigned to CA dept. of justice
-        IpV4Filter("192.58.200-203.0-255").on_match(match_handler)  # IP range assigned to Bureau of Justice Statistics in WA
-    ]
 
-    wc = WikiChangeWatcher(*filters)
+    filter_collection = FilterCollection(
+        IpV4Filter("136.200.0-255.0-255"),                                    # IP4 range assigned to CA dept. of water resources
+        IpV4Filter("151.143.0-255.0-255"),                                    # IP4 range assigned to CA dept. of technology
+        IpV4Filter("160.88.0-255.0-255"),                                     # IP4 range assigned to CA dept. of insurance
+        IpV4Filter("192.56.110.0-255"),                                       # IP4 range #1 assigned to CA dept. of corrections
+        IpV4Filter("153.48.0-255.0-255"),                                     # IP4 range #2 assigned to CA dept. of corrections
+        IpV4Filter("149.136.0-255.0-255"),                                    # IP4 range assigned to CA dept. of transportation
+        IpV6Filter("2602:814:5000-5fff:0-ffff:0-ffff:0-ffff:0-ffff:0-ffff"),  # IP6 range assigned CA dept. of transportation
+        IpV4Filter("192.251.92.0-255"),                                       # IP4 range assigned to CA dept. of general services
+        IpV4Filter("159.145.0-255.0-255"),                                    # IP4 range assigned to CA dept. of consumer affairs
+        IpV4Filter("167.10.0-255.0-255"),                                     # IP4 range assigned to CA dept. of justice
+        IpV4Filter("192.58.200-203.0-255"),                                   # IP4 range assigned to Bureau of Justice Statistics in WA
+        IpV6Filter("2607:f330:0-ffff:0-ffff:0-ffff:0-ffff:0-ffff:0-ffff")     # IP6 range assigned to the US dept. of justice in WA
+    ).set_match_type(MatchType.ALL).on_match(match_handler)
 
+    wc = WikiChangeWatcher(filter_collection)
     wc.run()
 
     # Watch for page edits forever until KeyboardInterrupt
     try:
         while True:
             time.sleep(0.1)
     except KeyboardInterrupt:
         wc.stop()
 
-
 Calculating a running average of page-edits-per-minute for all of wikipedia
 ---------------------------------------------------------------------------
 
 The following example watches for any edit to any wikipedia page, and updates a
 running average of the rate of page edits per minute, which is printed to stdout
 once every 5 seconds.
 
@@ -322,15 +322,14 @@
 
     # Example script showing how to use WikiChangeWatcher to watch for "anonymous" edits to any
     # wikipedia page from specific IP address ranges
 
     import time
     import statistics
     import queue
-    from typing import Callable, Self
 
     from wikichangewatcher import WikiChangeWatcher
 
 
     # Max. number of samples in the averaging window
     MAX_WINDOW_LEN = 6
 
@@ -383,15 +382,14 @@
             try:
                 ret = self._queue.get(block=False)
             except queue.Empty:
                 pass
 
             return ret
 
-
     # Create rate counter class to monitor page edit rate over time
     ratecounter = EditRateCounter()
 
     # Create a watcher with no filters-- we want to see every single edit
     wc = WikiChangeWatcher().on_edit(ratecounter.edit_handler)
 
     wc.run()
```

## Comparing `wikichangewatcher-0.1.0.dist-info/RECORD` & `wikichangewatcher-0.2.0.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-wikichangewatcher/__init__.py,sha256=ZKlP2spGySGHS7BIX-aV7ybUyGlao_X1BHuAyRp0624,486
-wikichangewatcher/wikichangewatcher.py,sha256=xur6W3qM7PDBqMtrU_hH6sHekfmGR_ZxQzOtOaCDYkI,10526
-wikichangewatcher-0.1.0.dist-info/LICENSE,sha256=TnXSlu6RXKQvvwOoFbWv--MAdwOfsuLVHilmQGOJLE0,10761
-wikichangewatcher-0.1.0.dist-info/METADATA,sha256=67GlKfZnjLOWv7t-WwPoIjKrTFA147-UnPmspVQMYqM,16417
-wikichangewatcher-0.1.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-wikichangewatcher-0.1.0.dist-info/top_level.txt,sha256=Vz7JWMMoLHhpqlNkP7tnrdtY_R2RebM4aodqN1p8rmo,18
-wikichangewatcher-0.1.0.dist-info/RECORD,,
+wikichangewatcher/__init__.py,sha256=IWa0TMb7Ymppgs-Is-3MBaUS-nI6w0hqIBHLwzggqLk,498
+wikichangewatcher/wikichangewatcher.py,sha256=MrZrOg6aQSSFQSsUW8EikZfDAp1PWK_K0b547HCBEnU,12743
+wikichangewatcher-0.2.0.dist-info/LICENSE,sha256=TnXSlu6RXKQvvwOoFbWv--MAdwOfsuLVHilmQGOJLE0,10761
+wikichangewatcher-0.2.0.dist-info/METADATA,sha256=8ZALwBodfY3_LtmFfFon-hjriJFuydKR6pl9RvUIg1I,16752
+wikichangewatcher-0.2.0.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+wikichangewatcher-0.2.0.dist-info/top_level.txt,sha256=Vz7JWMMoLHhpqlNkP7tnrdtY_R2RebM4aodqN1p8rmo,18
+wikichangewatcher-0.2.0.dist-info/RECORD,,
```

