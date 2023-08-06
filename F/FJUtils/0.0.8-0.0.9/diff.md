# Comparing `tmp/FJUtils-0.0.8.tar.gz` & `tmp/FJUtils-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FJUtils-0.0.8.tar", last modified: Tue Aug  1 09:19:41 2023, max compression
+gzip compressed data, was "FJUtils-0.0.9.tar", last modified: Tue Aug  1 13:39:30 2023, max compression
```

## Comparing `FJUtils-0.0.8.tar` & `FJUtils-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-08-01 09:19:41.482348 FJUtils-0.0.8/
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-08-01 09:19:41.478348 FJUtils-0.0.8/FJUtils.egg-info/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     3670 2023-08-01 09:19:41.000000 FJUtils-0.0.8/FJUtils.egg-info/PKG-INFO
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      362 2023-08-01 09:19:41.000000 FJUtils-0.0.8/FJUtils.egg-info/SOURCES.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)        1 2023-08-01 09:19:41.000000 FJUtils-0.0.8/FJUtils.egg-info/dependency_links.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      116 2023-08-01 09:19:41.000000 FJUtils-0.0.8/FJUtils.egg-info/requires.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)        8 2023-08-01 09:19:41.000000 FJUtils-0.0.8/FJUtils.egg-info/top_level.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    11357 2023-06-06 11:02:09.000000 FJUtils-0.0.8/LICENSE
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     3670 2023-08-01 09:19:41.482348 FJUtils-0.0.8/PKG-INFO
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     2911 2023-06-06 11:02:09.000000 FJUtils-0.0.8/README.md
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-08-01 09:19:41.482348 FJUtils-0.0.8/fjutils/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      885 2023-07-31 09:42:46.000000 FJUtils-0.0.8/fjutils/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     8332 2023-06-17 08:26:17.000000 FJUtils-0.0.8/fjutils/checkpointing.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     9956 2023-07-22 12:20:22.000000 FJUtils-0.0.8/fjutils/easylm.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    25511 2023-07-31 09:40:02.000000 FJUtils-0.0.8/fjutils/flash_attention.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1800 2023-06-06 11:02:09.000000 FJUtils-0.0.8/fjutils/load.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1931 2023-07-26 09:37:29.000000 FJUtils-0.0.8/fjutils/loss_funcs.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    15184 2023-08-01 09:19:08.000000 FJUtils-0.0.8/fjutils/optimizers.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     7278 2023-07-22 12:19:47.000000 FJUtils-0.0.8/fjutils/utils.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      533 2023-06-06 11:02:09.000000 FJUtils-0.0.8/pyproject.toml
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       38 2023-08-01 09:19:41.482348 FJUtils-0.0.8/setup.cfg
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1209 2023-08-01 09:19:08.000000 FJUtils-0.0.8/setup.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-08-01 13:39:30.491582 FJUtils-0.0.9/
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-08-01 13:39:30.491582 FJUtils-0.0.9/FJUtils.egg-info/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     3670 2023-08-01 13:39:30.000000 FJUtils-0.0.9/FJUtils.egg-info/PKG-INFO
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      362 2023-08-01 13:39:30.000000 FJUtils-0.0.9/FJUtils.egg-info/SOURCES.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)        1 2023-08-01 13:39:30.000000 FJUtils-0.0.9/FJUtils.egg-info/dependency_links.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      109 2023-08-01 13:39:30.000000 FJUtils-0.0.9/FJUtils.egg-info/requires.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)        8 2023-08-01 13:39:30.000000 FJUtils-0.0.9/FJUtils.egg-info/top_level.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    11357 2023-06-06 11:02:09.000000 FJUtils-0.0.9/LICENSE
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     3670 2023-08-01 13:39:30.491582 FJUtils-0.0.9/PKG-INFO
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     2911 2023-06-06 11:02:09.000000 FJUtils-0.0.9/README.md
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-08-01 13:39:30.491582 FJUtils-0.0.9/fjutils/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      885 2023-07-31 09:42:46.000000 FJUtils-0.0.9/fjutils/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     8332 2023-06-17 08:26:17.000000 FJUtils-0.0.9/fjutils/checkpointing.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     9956 2023-07-22 12:20:22.000000 FJUtils-0.0.9/fjutils/easylm.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    25511 2023-07-31 09:40:02.000000 FJUtils-0.0.9/fjutils/flash_attention.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1800 2023-06-06 11:02:09.000000 FJUtils-0.0.9/fjutils/load.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1931 2023-07-26 09:37:29.000000 FJUtils-0.0.9/fjutils/loss_funcs.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    15652 2023-08-01 13:37:59.000000 FJUtils-0.0.9/fjutils/optimizers.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     7278 2023-07-22 12:19:47.000000 FJUtils-0.0.9/fjutils/utils.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      533 2023-06-06 11:02:09.000000 FJUtils-0.0.9/pyproject.toml
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       38 2023-08-01 13:39:30.491582 FJUtils-0.0.9/setup.cfg
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1202 2023-08-01 13:38:18.000000 FJUtils-0.0.9/setup.py
```

### Comparing `FJUtils-0.0.8/FJUtils.egg-info/PKG-INFO` & `FJUtils-0.0.9/FJUtils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FJUtils
-Version: 0.0.8
+Version: 0.0.9
 Summary: UNKNOWN
 Home-page: https://github.com/erfanzar/
 Author: Erfan Zare Chavoshi
 Author-email: erfanzare82@yahoo.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `FJUtils-0.0.8/LICENSE` & `FJUtils-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `FJUtils-0.0.8/PKG-INFO` & `FJUtils-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FJUtils
-Version: 0.0.8
+Version: 0.0.9
 Summary: UNKNOWN
 Home-page: https://github.com/erfanzar/
 Author: Erfan Zare Chavoshi
 Author-email: erfanzare82@yahoo.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `FJUtils-0.0.8/README.md` & `FJUtils-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `FJUtils-0.0.8/fjutils/__init__.py` & `FJUtils-0.0.9/fjutils/__init__.py`

 * *Files identical despite different names*

### Comparing `FJUtils-0.0.8/fjutils/checkpointing.py` & `FJUtils-0.0.9/fjutils/checkpointing.py`

 * *Files identical despite different names*

### Comparing `FJUtils-0.0.8/fjutils/easylm.py` & `FJUtils-0.0.9/fjutils/easylm.py`

 * *Files identical despite different names*

### Comparing `FJUtils-0.0.8/fjutils/flash_attention.py` & `FJUtils-0.0.9/fjutils/flash_attention.py`

 * *Files identical despite different names*

### Comparing `FJUtils-0.0.8/fjutils/load.py` & `FJUtils-0.0.9/fjutils/load.py`

 * *Files identical despite different names*

### Comparing `FJUtils-0.0.8/fjutils/loss_funcs.py` & `FJUtils-0.0.9/fjutils/loss_funcs.py`

 * *Files identical despite different names*

### Comparing `FJUtils-0.0.8/fjutils/optimizers.py` & `FJUtils-0.0.9/fjutils/optimizers.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,17 +77,18 @@
         ),
         optax.add_decayed_weights(
             weight_decay=weight_decay
         ),
         optax.scale_by_schedule(scheduler),
         optax.scale(-1)
     )
-    tx = optax.MultiSteps(
-        tx, gradient_accumulation_steps
-    )
+    if gradient_accumulation_steps > 1:
+        tx = optax.MultiSteps(
+            tx, gradient_accumulation_steps
+        )
     return tx, scheduler
 
 
 def get_adamw_with_linear_scheduler(
         steps: int,
         learning_rate_start: float = 5e-5,
         learning_rate_end: float = 1e-5,
@@ -129,17 +130,18 @@
         ),
         optax.add_decayed_weights(
             weight_decay=weight_decay
         ),
         optax.scale_by_schedule(scheduler),
         optax.scale(-1)
     )
-    tx = optax.MultiSteps(
-        tx, gradient_accumulation_steps
-    )
+    if gradient_accumulation_steps > 1:
+        tx = optax.MultiSteps(
+            tx, gradient_accumulation_steps
+        )
     return tx, scheduler
 
 
 def get_adafactor_with_linear_scheduler(
         steps: int,
         learning_rate_start: float = 5e-5,
         learning_rate_end: float = 1e-5,
@@ -199,17 +201,18 @@
             factored=factored
         ),
         optax_add_scheduled_weight_decay(
             lambda step: -scheduler(step) * weight_decay,
             weight_decay_mask
         )
     )
-    tx = optax.MultiSteps(
-        tx, gradient_accumulation_steps
-    )
+    if gradient_accumulation_steps > 1:
+        tx = optax.MultiSteps(
+            tx, gradient_accumulation_steps
+        )
     return tx, scheduler
 
 
 def get_adafactor_with_cosine_scheduler(
         steps: int,
         learning_rate=5e-5,
         weight_decay=1e-1,
@@ -265,17 +268,18 @@
             factored=factored
         ),
         optax_add_scheduled_weight_decay(
             lambda step: -scheduler(step) * weight_decay,
             weight_decay_mask
         )
     )
-    tx = optax.MultiSteps(
-        tx, gradient_accumulation_steps
-    )
+    if gradient_accumulation_steps > 1:
+        tx = optax.MultiSteps(
+            tx, gradient_accumulation_steps
+        )
     return tx, scheduler
 
 
 def get_lion_with_cosine_scheduler(
         steps: int,
         learning_rate=5e-5,
         alpha: float = 0.0,
@@ -324,17 +328,18 @@
             b1=b1,
             b2=b2,
             mu_dtype=mu_dtype
         ),
         optax.scale_by_schedule(scheduler),
         optax.scale(-1)
     )
-    tx = optax.MultiSteps(
-        tx, gradient_accumulation_steps
-    )
+    if gradient_accumulation_steps > 1:
+        tx = optax.MultiSteps(
+            tx, gradient_accumulation_steps
+        )
     return tx, scheduler
 
 
 def get_lion_with_linear_scheduler(
         steps: int,
         learning_rate_start: float = 5e-5,
         learning_rate_end: float = 1e-5,
@@ -366,17 +371,18 @@
             b1=b1,
             b2=b2,
             mu_dtype=mu_dtype
         ),
         optax.scale_by_schedule(scheduler),
         optax.scale(-1)
     )
-    tx = optax.MultiSteps(
-        tx, gradient_accumulation_steps
-    )
+    if gradient_accumulation_steps > 1:
+        tx = optax.MultiSteps(
+            tx, gradient_accumulation_steps
+        )
     return tx, scheduler
 
 
 def get_adamw_with_warm_up_cosine_scheduler(
         steps: int,
         learning_rate: float = 5e-5,
         b1: float = 0.9,
@@ -420,17 +426,18 @@
         ),
         optax.add_decayed_weights(
             weight_decay=weight_decay
         ),
         optax.scale_by_schedule(scheduler),
         optax.scale(-1)
     )
-    tx = optax.MultiSteps(
-        tx, gradient_accumulation_steps
-    )
+    if gradient_accumulation_steps > 1:
+        tx = optax.MultiSteps(
+            tx, gradient_accumulation_steps
+        )
     return tx, scheduler
 
 
 def get_adafactor_with_warm_up_cosine_scheduler(
         steps: int,
         learning_rate=5e-5,
         weight_decay=1e-1,
@@ -491,17 +498,18 @@
             factored=factored
         ),
         optax_add_scheduled_weight_decay(
             lambda step: -scheduler(step) * weight_decay,
             weight_decay_mask
         )
     )
-    tx = optax.MultiSteps(
-        tx, gradient_accumulation_steps
-    )
+    if gradient_accumulation_steps > 1:
+        tx = optax.MultiSteps(
+            tx, gradient_accumulation_steps
+        )
     return tx, scheduler
 
 
 def get_lion_with_warm_up_cosine_scheduler(
         steps: int,
         learning_rate=5e-5,
         exponent: float = 1.0,
@@ -534,11 +542,12 @@
             b1=b1,
             b2=b2,
             mu_dtype=mu_dtype
         ),
         optax.scale_by_schedule(scheduler),
         optax.scale(-1)
     )
-    tx = optax.MultiSteps(
-        tx, gradient_accumulation_steps
-    )
+    if gradient_accumulation_steps > 1:
+        tx = optax.MultiSteps(
+            tx, gradient_accumulation_steps
+        )
     return tx, scheduler
```

### Comparing `FJUtils-0.0.8/fjutils/utils.py` & `FJUtils-0.0.9/fjutils/utils.py`

 * *Files identical despite different names*

### Comparing `FJUtils-0.0.8/pyproject.toml` & `FJUtils-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `FJUtils-0.0.8/setup.py` & `FJUtils-0.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="FJUtils",
-    version='0.0.8',
+    version='0.0.9',
     author="Erfan Zare Chavoshi",
     author_email="erfanzare82@yahoo.com",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/erfanzar/",
     packages=setuptools.find_packages(),
     install_requires=[
         'jax',
-        'transformers~=4.30.2',
+        'transformers~=4.31.0',
         'typing~=3.7.4.3',
         'numpy~=1.24.3',
-        'flax~=0.6.4',
+        'flax',
         'msgpack~=1.0.5',
         'setuptools~=59.6.0',
         'ml_collections'
     ],
     python_requires=">=3.7, <3.11",
     license='Apache License 2.0',
     classifiers=[
```

