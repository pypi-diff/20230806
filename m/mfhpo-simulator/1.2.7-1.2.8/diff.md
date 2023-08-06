# Comparing `tmp/mfhpo_simulator-1.2.7-py3-none-any.whl.zip` & `tmp/mfhpo_simulator-1.2.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 37256 bytes, number of entries: 19
--rw-rw-r--  2.0 unx      560 b- defN 23-Aug-01 14:25 benchmark_simulator/__init__.py
--rw-rw-r--  2.0 unx     8275 b- defN 23-Aug-01 13:19 benchmark_simulator/_constants.py
+Zip file size: 37346 bytes, number of entries: 19
+-rw-rw-r--  2.0 unx      560 b- defN 23-Aug-06 08:23 benchmark_simulator/__init__.py
+-rw-rw-r--  2.0 unx     8516 b- defN 23-Aug-06 08:23 benchmark_simulator/_constants.py
 -rw-rw-r--  2.0 unx    16238 b- defN 23-Aug-01 13:41 benchmark_simulator/_secure_proc.py
 -rw-rw-r--  2.0 unx     5116 b- defN 23-Jul-06 23:36 benchmark_simulator/_utils.py
 -rw-rw-r--  2.0 unx    30591 b- defN 23-Aug-01 13:19 benchmark_simulator/simulator.py
 -rw-rw-r--  2.0 unx     2582 b- defN 23-Jul-06 18:41 benchmark_simulator/_simulator/_base_wrapper.py
 -rw-rw-r--  2.0 unx     3362 b- defN 23-Aug-01 13:19 benchmark_simulator/_simulator/_utils.py
 -rw-rw-r--  2.0 unx    15295 b- defN 23-Aug-01 13:36 benchmark_simulator/_simulator/_worker.py
 -rw-rw-r--  2.0 unx     3767 b- defN 23-Jul-18 21:06 benchmark_simulator/_simulator/_worker_manager.py
 -rw-rw-r--  2.0 unx    10175 b- defN 23-Aug-01 13:19 benchmark_simulator/_simulator/_worker_manager_for_ask_and_tell.py
 -rw-rw-r--  2.0 unx     2181 b- defN 23-Jul-06 18:55 benchmark_simulator/_trackers/_config_tracker.py
 -rw-rw-r--  2.0 unx     5012 b- defN 23-Jul-06 23:14 benchmark_simulator/_trackers/_state_tracker.py
 -rw-rw-r--  2.0 unx      284 b- defN 23-Jul-10 08:56 benchmark_simulator/utils/__init__.py
 -rw-rw-r--  2.0 unx     9963 b- defN 23-Jul-25 19:56 benchmark_simulator/utils/_performance_over_time.py
--rw-rw-r--  2.0 unx    10760 b- defN 23-Aug-01 14:26 mfhpo_simulator-1.2.7.dist-info/LICENSE
--rw-rw-r--  2.0 unx      307 b- defN 23-Aug-01 14:26 mfhpo_simulator-1.2.7.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Aug-01 14:26 mfhpo_simulator-1.2.7.dist-info/WHEEL
--rw-rw-r--  2.0 unx      107 b- defN 23-Aug-01 14:26 mfhpo_simulator-1.2.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1813 b- defN 23-Aug-01 14:26 mfhpo_simulator-1.2.7.dist-info/RECORD
-19 files, 126480 bytes uncompressed, 34220 bytes compressed:  72.9%
+-rw-rw-r--  2.0 unx    10760 b- defN 23-Aug-06 08:25 mfhpo_simulator-1.2.8.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      307 b- defN 23-Aug-06 08:25 mfhpo_simulator-1.2.8.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Aug-06 08:25 mfhpo_simulator-1.2.8.dist-info/WHEEL
+-rw-rw-r--  2.0 unx      107 b- defN 23-Aug-06 08:25 mfhpo_simulator-1.2.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1813 b- defN 23-Aug-06 08:25 mfhpo_simulator-1.2.8.dist-info/RECORD
+19 files, 126721 bytes uncompressed, 34310 bytes compressed:  72.9%
```

## zipnote {}

```diff
@@ -36,23 +36,23 @@
 
 Filename: benchmark_simulator/utils/__init__.py
 Comment: 
 
 Filename: benchmark_simulator/utils/_performance_over_time.py
 Comment: 
 
-Filename: mfhpo_simulator-1.2.7.dist-info/LICENSE
+Filename: mfhpo_simulator-1.2.8.dist-info/LICENSE
 Comment: 
 
-Filename: mfhpo_simulator-1.2.7.dist-info/METADATA
+Filename: mfhpo_simulator-1.2.8.dist-info/METADATA
 Comment: 
 
-Filename: mfhpo_simulator-1.2.7.dist-info/WHEEL
+Filename: mfhpo_simulator-1.2.8.dist-info/WHEEL
 Comment: 
 
-Filename: mfhpo_simulator-1.2.7.dist-info/top_level.txt
+Filename: mfhpo_simulator-1.2.8.dist-info/top_level.txt
 Comment: 
 
-Filename: mfhpo_simulator-1.2.7.dist-info/RECORD
+Filename: mfhpo_simulator-1.2.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## benchmark_simulator/__init__.py

```diff
@@ -1,12 +1,12 @@
 from benchmark_simulator._constants import AbstractAskTellOptimizer, ObjectiveFuncType
 from benchmark_simulator.simulator import ObjectiveFuncWrapper, get_multiple_wrappers
 
 
-__version__ = "1.2.7"
+__version__ = "1.2.8"
 __copyright__ = "Copyright (C) 2023 Shuhei Watanabe"
 __licence__ = "Apache-2.0 License"
 __author__ = "Shuhei Watanabe"
 __author_email__ = "shuhei.watanabe.utokyo@gmail.com"
 __url__ = "https://github.com/nabenabe0928/mfhpo-simulator"
```

## benchmark_simulator/_constants.py

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import os
+import warnings
 from abc import ABCMeta, abstractmethod
 from dataclasses import dataclass
 from enum import Enum
 from typing import Any, Final, Protocol
 
 import numpy as np
 
@@ -104,14 +105,18 @@
             )
         if self.allow_parallel_sampling and self.expensive_sampler:
             raise ValueError(
                 "expensive_sampler and allow_parallel_sampling cannot be True simultaneously.\n"
                 "Note that allow_parallel_sampling=True correctly handles expensive samplers"
                 " if sampling happens in parallel."
             )
+        if self.n_workers > os.cpu_count():
+            msg = f"n_workers larger than the number of CPU cores (={os.cpu_count()}) "
+            msg += "may cause hang or significant slow down."
+            warnings.warn(msg)
 
 
 @dataclass(frozen=True)
 class _WorkerVars:
     continual_eval: bool
     worker_id: str
     worker_index: int
```

## Comparing `mfhpo_simulator-1.2.7.dist-info/LICENSE` & `mfhpo_simulator-1.2.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mfhpo_simulator-1.2.7.dist-info/RECORD` & `mfhpo_simulator-1.2.8.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-benchmark_simulator/__init__.py,sha256=WotbIOje4UKe4lyspQVwoDTSIi11Z-Lb-RzSHs_BCLs,560
-benchmark_simulator/_constants.py,sha256=3FIaZuUjJjc36Lb6wCnVbMAadhO3vFlkpqg_Au_MK9Q,8275
+benchmark_simulator/__init__.py,sha256=0MyKags7oV9Nub_S2MTmF3uqkOJ-n21tOZDyLcogJhQ,560
+benchmark_simulator/_constants.py,sha256=GU2inn7LpvNNaQ14unK1asnmwKTkUKsDh_oJkq4VLww,8516
 benchmark_simulator/_secure_proc.py,sha256=4stXKjvQqaGCr8JTqq8g8SFx6vpssibRpm-xzgMjm5c,16238
 benchmark_simulator/_utils.py,sha256=ZA8l51dZMxpjhMZCUExO-Mg8r5ilJWdvR2P3RFipzk4,5116
 benchmark_simulator/simulator.py,sha256=1DU1tvisQH_gqGwWbT5tF2rxEdHsiyoJG67CD3-CfZw,30591
 benchmark_simulator/_simulator/_base_wrapper.py,sha256=HvK4Iq1vjCuD1HEcphY-hl4Wo_vo1d-N_FA9PFkYukA,2582
 benchmark_simulator/_simulator/_utils.py,sha256=_E65XZddiFb6sMpZkZCzfOyoZVpADwtDUd_2TQ0Dudg,3362
 benchmark_simulator/_simulator/_worker.py,sha256=kPuVUkyUxJWrU3JszC5h_fiQ9J3tcavKNFpfQw0yOgc,15295
 benchmark_simulator/_simulator/_worker_manager.py,sha256=wwdsMDeuVLjdFKqbZ3sJ7C5Ep8G2fFDT0jyYw-RkGGc,3767
 benchmark_simulator/_simulator/_worker_manager_for_ask_and_tell.py,sha256=WWgP7qV_XOKSGgaKBNFeAtM2oPTW__z1qY5x7er88VM,10175
 benchmark_simulator/_trackers/_config_tracker.py,sha256=-tKF_13VtOnAmCm0uzENpUg_ePyd7o_PvG9mkxzXjzQ,2181
 benchmark_simulator/_trackers/_state_tracker.py,sha256=EyeOuoFPf7c8yUgmhrDe54d0wc0Jowxo-6Vs7aUBZ5I,5012
 benchmark_simulator/utils/__init__.py,sha256=PWSU9sL4fLNRLkwm3mElZ7D_wLCWDdyCZa39RqcTYoQ,284
 benchmark_simulator/utils/_performance_over_time.py,sha256=FrSdxUuD5R2lBkqxfqlvBySY5tE8WUVPuxmm7kbMLkY,9963
-mfhpo_simulator-1.2.7.dist-info/LICENSE,sha256=auQsw_aAlfeXmKRQ_tmNBjUD2-wJojtRJPslgGyGqK4,10760
-mfhpo_simulator-1.2.7.dist-info/METADATA,sha256=m-jFK3_jwYfCdECCUXF40h-TUaZ8Gk2U6aufLvCMhoQ,307
-mfhpo_simulator-1.2.7.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-mfhpo_simulator-1.2.7.dist-info/top_level.txt,sha256=uJovuRlKQlk3_JQI_pIvLjq9bJ7D1LdHBYxgRvtIzFk,107
-mfhpo_simulator-1.2.7.dist-info/RECORD,,
+mfhpo_simulator-1.2.8.dist-info/LICENSE,sha256=auQsw_aAlfeXmKRQ_tmNBjUD2-wJojtRJPslgGyGqK4,10760
+mfhpo_simulator-1.2.8.dist-info/METADATA,sha256=qKqrrmHfCeF-fZSUZ89t7EB3FLfHntFbgBnZ3OSZ4xA,307
+mfhpo_simulator-1.2.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+mfhpo_simulator-1.2.8.dist-info/top_level.txt,sha256=uJovuRlKQlk3_JQI_pIvLjq9bJ7D1LdHBYxgRvtIzFk,107
+mfhpo_simulator-1.2.8.dist-info/RECORD,,
```

