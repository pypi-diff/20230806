# Comparing `tmp/voicebox-pytorch-0.0.5.tar.gz` & `tmp/voicebox-pytorch-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voicebox-pytorch-0.0.5.tar", last modified: Sat Aug  5 20:19:34 2023, max compression
+gzip compressed data, was "voicebox-pytorch-0.0.6.tar", last modified: Sun Aug  6 00:56:47 2023, max compression
```

## Comparing `voicebox-pytorch-0.0.5.tar` & `voicebox-pytorch-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 20:19:34.324803 voicebox-pytorch-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-05 20:19:25.000000 voicebox-pytorch-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-08-05 20:19:34.324803 voicebox-pytorch-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-08-05 20:19:25.000000 voicebox-pytorch-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 20:19:34.324803 voicebox-pytorch-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-08-05 20:19:25.000000 voicebox-pytorch-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 20:19:34.324803 voicebox-pytorch-0.0.5/voicebox_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-08-05 20:19:25.000000 voicebox-pytorch-0.0.5/voicebox_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-08-05 20:19:25.000000 voicebox-pytorch-0.0.5/voicebox_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)    16197 2023-08-05 20:19:25.000000 voicebox-pytorch-0.0.5/voicebox_pytorch/voicebox_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 20:19:34.324803 voicebox-pytorch-0.0.5/voicebox_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-08-05 20:19:34.000000 voicebox-pytorch-0.0.5/voicebox_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-08-05 20:19:34.000000 voicebox-pytorch-0.0.5/voicebox_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 20:19:34.000000 voicebox-pytorch-0.0.5/voicebox_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-05 20:19:34.000000 voicebox-pytorch-0.0.5/voicebox_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-05 20:19:34.000000 voicebox-pytorch-0.0.5/voicebox_pytorch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 00:56:47.811332 voicebox-pytorch-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-06 00:56:36.000000 voicebox-pytorch-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-08-06 00:56:47.811332 voicebox-pytorch-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-08-06 00:56:36.000000 voicebox-pytorch-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 00:56:47.811332 voicebox-pytorch-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-08-06 00:56:36.000000 voicebox-pytorch-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 00:56:47.811332 voicebox-pytorch-0.0.6/voicebox_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-08-06 00:56:36.000000 voicebox-pytorch-0.0.6/voicebox_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-08-06 00:56:36.000000 voicebox-pytorch-0.0.6/voicebox_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16368 2023-08-06 00:56:36.000000 voicebox-pytorch-0.0.6/voicebox_pytorch/voicebox_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 00:56:47.811332 voicebox-pytorch-0.0.6/voicebox_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-08-06 00:56:47.000000 voicebox-pytorch-0.0.6/voicebox_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-08-06 00:56:47.000000 voicebox-pytorch-0.0.6/voicebox_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 00:56:47.000000 voicebox-pytorch-0.0.6/voicebox_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-06 00:56:47.000000 voicebox-pytorch-0.0.6/voicebox_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-06 00:56:47.000000 voicebox-pytorch-0.0.6/voicebox_pytorch.egg-info/top_level.txt
```

### Comparing `voicebox-pytorch-0.0.5/LICENSE` & `voicebox-pytorch-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `voicebox-pytorch-0.0.5/PKG-INFO` & `voicebox-pytorch-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voicebox-pytorch
-Version: 0.0.5
+Version: 0.0.6
 Summary: Voicebox - Pytorch
 Home-page: https://github.com/lucidrains/voicebox-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,text to speech
 Classifier: Development Status :: 4 - Beta
```

### Comparing `voicebox-pytorch-0.0.5/README.md` & `voicebox-pytorch-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `voicebox-pytorch-0.0.5/setup.py` & `voicebox-pytorch-0.0.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'voicebox-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.0.5',
+  version = '0.0.6',
   license='MIT',
   description = 'Voicebox - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/voicebox-pytorch',
   keywords = [
```

### Comparing `voicebox-pytorch-0.0.5/voicebox_pytorch/attend.py` & `voicebox-pytorch-0.0.6/voicebox_pytorch/attend.py`

 * *Files identical despite different names*

### Comparing `voicebox-pytorch-0.0.5/voicebox_pytorch/voicebox_pytorch.py` & `voicebox-pytorch-0.0.6/voicebox_pytorch/voicebox_pytorch.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,14 +220,16 @@
 
             self.layers.append(nn.ModuleList([
                 nn.Linear(dim * 2, dim) if has_skip else None,
                 Attention(dim = dim, dim_head = dim_head, heads = heads, flash = attn_flash),
                 FeedForward(dim = dim, mult = ff_mult)
             ]))
 
+        self.final_norm = RMSNorm(dim)
+
     def forward(self, x):
         skip_connects = []
 
         rotary_emb = self.rotary_emb(x.shape[-2])
 
         for skip_combiner, attn, ff in self.layers:
 
@@ -239,15 +241,15 @@
             else:
                 x = torch.cat((x, skip_connects.pop()), dim = -1)
                 x = skip_combiner(x)
 
             x = attn(x, rotary_emb = rotary_emb) + x
             x = ff(x) + x
 
-        return x
+        return self.final_norm(x)
 
 # both duration and main denoising model are transformers
 
 class DurationPredictor(Module):
     def __init__(
         self,
         *,
@@ -282,14 +284,19 @@
             depth = depth,
             dim_head = dim_head,
             heads = heads,
             ff_mult = ff_mult,
             attn_flash = attn_flash
         )
 
+        self.to_pred = nn.Sequential(
+            nn.Linear(dim, 1),
+            Rearrange('... 1 -> ...')
+        )
+
     @torch.inference_mode()
     def forward_with_cond_scale(
         self,
         *args,
         cond_scale = 1.,
         **kwargs
     ):
@@ -340,16 +347,14 @@
         x = self.conv_embed(x) + x
         x = self.transformer(x)
 
         if not exists(mask):
             return F.l1_loss(x, target)
 
         loss = F.l1_loss(x, target, reduction = 'none')
-
-        loss = reduce(loss, 'b n d -> b n', 'mean')
         loss = loss.masked_fill(mask, 0.)
 
         # masked mean
 
         num = reduce(loss, 'b n -> b', 'sum')
         den = mask.sum(dim = -1).clamp(min = 1e-5)
         loss = num / den
@@ -393,14 +398,16 @@
             depth = depth,
             dim_head = dim_head,
             heads = heads,
             ff_mult = ff_mult,
             attn_flash = attn_flash
         )
 
+        self.to_pred = nn.Linear(dim, dim, bias = False)
+
     @torch.inference_mode()
     def forward_with_cond_scale(
         self,
         *args,
         cond_scale = 1.,
         **kwargs
     ):
@@ -461,14 +468,16 @@
         time_emb = self.sinu_pos_emb(times)
         x, ps = pack((time_emb, x), 'b * d')
 
         # attend
 
         x = self.transformer(x)
 
+        x = self.to_pred(x)
+
         # split out time embedding
 
         _, x = unpack(x, ps, 'b * d')
 
         # if no target passed in, just return logits
 
         if not exists(target):
@@ -594,17 +603,15 @@
         # random times
 
         times = torch.rand((batch,), dtype = dtype)
         t = rearrange(times, 'b -> b 1 1')
 
         # sample xt (w in the paper)
 
-        mu_t = t * x1
-        σt = (1 - (1 - σ) * t) * x0
-        w = mu_t + σt
+        w = (1 - (1 - σ) * t) * x0 + t * x1
 
         flow = x1 - (1 - σ) * x0
 
         # construct mask if not given
 
         if (
             not exists(mask) and
```

### Comparing `voicebox-pytorch-0.0.5/voicebox_pytorch.egg-info/PKG-INFO` & `voicebox-pytorch-0.0.6/voicebox_pytorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voicebox-pytorch
-Version: 0.0.5
+Version: 0.0.6
 Summary: Voicebox - Pytorch
 Home-page: https://github.com/lucidrains/voicebox-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,text to speech
 Classifier: Development Status :: 4 - Beta
```

