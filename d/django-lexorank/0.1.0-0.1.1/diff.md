# Comparing `tmp/django_lexorank-0.1.0.tar.gz` & `tmp/django_lexorank-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_lexorank-0.1.0.tar", max compression
+gzip compressed data, was "django_lexorank-0.1.1.tar", max compression
```

## Comparing `django_lexorank-0.1.0.tar` & `django_lexorank-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     1065 2023-08-03 18:04:39.896261 django_lexorank-0.1.0/LICENSE
--rw-r--r--   0        0        0      103 2023-08-03 18:04:39.896350 django_lexorank-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-08-03 18:23:10.714000 django_lexorank-0.1.0/django_lexorank/__init__.py
--rw-r--r--   0        0        0      489 2023-08-06 10:52:45.401064 django_lexorank-0.1.0/django_lexorank/admin.py
--rw-r--r--   0        0        0      104 2023-08-06 10:54:04.667471 django_lexorank-0.1.0/django_lexorank/apps.py
--rw-r--r--   0        0        0     1218 2023-08-06 10:58:40.504664 django_lexorank-0.1.0/django_lexorank/fields.py
--rw-r--r--   0        0        0     5191 2023-08-06 10:58:40.548778 django_lexorank-0.1.0/django_lexorank/lexorank.py
--rw-r--r--   0        0        0        0 2023-08-06 10:56:59.851770 django_lexorank-0.1.0/django_lexorank/migrations/__init__.py
--rw-r--r--   0        0        0     5715 2023-08-06 11:01:53.747413 django_lexorank-0.1.0/django_lexorank/models.py
--rw-r--r--   0        0        0      908 2023-08-06 11:06:27.850630 django_lexorank-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      790 1970-01-01 00:00:00.000000 django_lexorank-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-08-06 16:03:57.877756 django_lexorank-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3456 2023-08-06 21:18:08.061475 django_lexorank-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-08-03 18:23:10.714000 django_lexorank-0.1.1/django_lexorank/__init__.py
+-rw-r--r--   0        0        0      489 2023-08-06 10:52:45.401000 django_lexorank-0.1.1/django_lexorank/admin.py
+-rw-r--r--   0        0        0      104 2023-08-06 10:54:04.667000 django_lexorank-0.1.1/django_lexorank/apps.py
+-rw-r--r--   0        0        0     1817 2023-08-06 15:13:30.915126 django_lexorank-0.1.1/django_lexorank/fields.py
+-rw-r--r--   0        0        0     5017 2023-08-06 15:13:34.774411 django_lexorank-0.1.1/django_lexorank/lexorank.py
+-rw-r--r--   0        0        0     1739 2023-08-06 19:33:03.324562 django_lexorank-0.1.1/django_lexorank/managers.py
+-rw-r--r--   0        0        0        0 2023-08-06 10:56:59.851000 django_lexorank-0.1.1/django_lexorank/migrations/__init__.py
+-rw-r--r--   0        0        0     8201 2023-08-06 21:06:49.593696 django_lexorank-0.1.1/django_lexorank/models.py
+-rw-r--r--   0        0        0     1403 2023-08-06 21:19:14.635008 django_lexorank-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4288 1970-01-01 00:00:00.000000 django_lexorank-0.1.1/PKG-INFO
```

### Comparing `django_lexorank-0.1.0/LICENSE` & `django_lexorank-0.1.1/LICENSE`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 rozumdev
+Copyright (c) 2023 Aleksandr Rozum
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `django_lexorank-0.1.0/django_lexorank/lexorank.py` & `django_lexorank-0.1.1/django_lexorank/lexorank.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import math
 import string
-from typing import Optional
+from typing import List, Optional, Tuple
 
 
 class LexoRank:
+    default_rank_length = 6
+    rebalancing_length = 128
     max_rank_length = 200
     base_symbols = string.ascii_lowercase
     first_symbol = base_symbols[0]
     last_symbol = base_symbols[-1]
     base = len(base_symbols)
 
     @classmethod
@@ -15,130 +17,125 @@
         return ord(char) - ord(cls.first_symbol)
 
     @classmethod
     def int_to_char(cls, num: int) -> str:
         return chr(num + ord(cls.first_symbol))
 
     @classmethod
-    def parse_rank(cls, rank: str) -> list[int]:
+    def parse_rank(cls, rank: str) -> List[int]:
         return [cls.char_to_int(char) for char in rank]
 
     @classmethod
-    def format_rank(cls, rank: list[int]) -> str:
+    def format_rank(cls, rank: List[int]) -> str:
         return "".join(map(cls.int_to_char, rank))
 
     @classmethod
-    def align_ranks(cls, previous_rank: str, next_rank: str) -> tuple[str, str]:
+    def align_ranks(cls, previous_rank: str, next_rank: str) -> Tuple[str, str]:
         max_len = max(len(previous_rank), len(next_rank))
 
         if max_len > cls.max_rank_length:
             raise ValueError("Rebalancing Required")
 
         previous_rank = previous_rank.ljust(max_len, cls.first_symbol)
-        next_rank = next_rank.ljust(max_len, cls.first_symbol)
+        next_rank = next_rank.ljust(max_len, cls.last_symbol)
 
         return previous_rank, next_rank
 
     @classmethod
     def get_lexorank_in_between(
         cls,
         previous_rank: Optional[str],
         next_rank: Optional[str],
         objects_count: int,
-        default_rank_length: int,
         force_reorder: bool = False,
     ) -> str:
         if not previous_rank:
-            previous_rank = cls.get_min_rank(
-                objects_count=objects_count, default_rank_length=default_rank_length
-            )
+            previous_rank = cls.get_min_rank(objects_count=objects_count)
 
         if not next_rank:
-            next_rank = cls.get_max_rank(
-                objects_count=objects_count, default_rank_length=default_rank_length
-            )
+            next_rank = cls.get_max_rank(objects_count=objects_count)
+
+        previous_rank, next_rank = cls.align_ranks(previous_rank, next_rank)
 
         if force_reorder:
             previous_rank, next_rank = sorted([previous_rank, next_rank])
         else:
             if not previous_rank < next_rank:
                 raise ValueError("Previous rank must go before than next rank.")
 
-        previous_rank, next_rank = cls.align_ranks(previous_rank, next_rank)
-
         previous_rank_parts = cls.parse_rank(previous_rank)
         next_rank_parts = cls.parse_rank(next_rank)
 
         total_diff = 0
         for i, previous_rank_part in enumerate(reversed(previous_rank_parts)):
             next_rank_part = next_rank_parts[len(next_rank_parts) - (i + 1)]
             if next_rank_part < previous_rank_part:
                 next_rank_part += cls.base
                 next_rank_parts[len(next_rank_parts) - (i + 1)] = next_rank_part
                 next_rank_parts[len(next_rank_parts) - (i + 2)] -= 1
 
             diff = next_rank_part - previous_rank_part
             total_diff += diff * (cls.base**i)
 
-        middle_rank_parts = []
+        middle_rank_parts = []  # type: ignore[var-annotated]
 
+        offset = 0
         for i, previous_rank_part in enumerate(reversed(previous_rank_parts)):
-            to_add = (
-                total_diff
-                / 2
-                / cls.base ** (len(previous_rank_parts) - (i + 1))
-                % cls.base
-            )
-            middle_rank_part = previous_rank_part + to_add
-            middle_rank_parts.append(math.floor(middle_rank_part))
+            to_add = total_diff / 2 / cls.base**i % cls.base
+            middle_rank_part = previous_rank_part + to_add + offset
+            offset = 0
+
+            if middle_rank_part > cls.base:
+                offset = 1
+                middle_rank_part -= cls.base
+
+            middle_rank_parts.insert(0, math.floor(middle_rank_part))
+
+        if offset:
+            middle_rank_parts.insert(0, cls.char_to_int(cls.first_symbol))
 
         if middle_rank_parts == previous_rank_parts:
             middle_rank_parts.append(
-                (ord(cls.last_symbol) - ord(cls.first_symbol)) // 2
+                (cls.char_to_int(cls.last_symbol) - cls.char_to_int(cls.first_symbol))
+                // 2
             )
 
         return cls.format_rank(middle_rank_parts)
 
     @classmethod
-    def get_min_rank(cls, objects_count: int, default_rank_length: int) -> str:
-        rank_length = cls.get_rank_length(objects_count, default_rank_length)
+    def get_min_rank(cls, objects_count: int) -> str:
+        rank_length = cls.get_rank_length(objects_count)
         return cls.format_rank([0] * rank_length)
 
     @classmethod
-    def get_max_rank(cls, objects_count: int, default_rank_length: int) -> str:
-        rank_length = cls.get_rank_length(objects_count, default_rank_length)
-        return cls.format_rank([cls.base - 1] * rank_length)
+    def get_max_rank(cls, objects_count: int) -> str:
+        rank_length = cls.get_rank_length(objects_count)
+        return cls.format_rank([cls.char_to_int(cls.last_symbol)] * rank_length)
 
     @classmethod
-    def get_rank_step(cls, objects_count: int, default_rank_length: int) -> int:
-        rank_length = cls.get_rank_length(
-            objects_count=objects_count, default_rank_length=default_rank_length
-        )
+    def get_rank_step(cls, objects_count: int) -> int:
+        rank_length = cls.get_rank_length(objects_count=objects_count)
         return int(cls.base**rank_length / objects_count - 0.5)
 
     @classmethod
-    def get_rank_length(cls, objects_count: int, default_rank_length: int) -> int:
+    def get_rank_length(cls, objects_count: int) -> int:
         if objects_count == 0:
             length_required_to_place_all_objects = 1
         else:
             length_required_to_place_all_objects = math.ceil(
                 math.log(objects_count, cls.base)
             )
         return min(
             cls.max_rank_length,
-            max(length_required_to_place_all_objects * 2, default_rank_length),
+            max(length_required_to_place_all_objects * 2, cls.default_rank_length),
         )
 
     @classmethod
-    def increment_rank(
-        cls, rank: str, objects_count: int, default_rank_length: int
-    ) -> str:
-        step = cls.get_rank_step(
-            objects_count=objects_count, default_rank_length=default_rank_length
-        )
+    def increment_rank(cls, rank: str, objects_count: int) -> str:
+        step = cls.get_rank_step(objects_count=objects_count)
         rank_parts = LexoRank.parse_rank(rank)
 
         for i in range(len(rank_parts) - 1, -1, -1):
             if step == 0:
                 break
 
             total = rank_parts[i] + step
```

