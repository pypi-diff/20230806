# Comparing `tmp/voicebox-pytorch-0.0.6.tar.gz` & `tmp/voicebox-pytorch-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voicebox-pytorch-0.0.6.tar", last modified: Sun Aug  6 00:56:47 2023, max compression
+gzip compressed data, was "voicebox-pytorch-0.0.7.tar", last modified: Sun Aug  6 03:46:48 2023, max compression
```

## Comparing `voicebox-pytorch-0.0.6.tar` & `voicebox-pytorch-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 00:56:47.811332 voicebox-pytorch-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-06 00:56:36.000000 voicebox-pytorch-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-08-06 00:56:47.811332 voicebox-pytorch-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-08-06 00:56:36.000000 voicebox-pytorch-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 00:56:47.811332 voicebox-pytorch-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-08-06 00:56:36.000000 voicebox-pytorch-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 00:56:47.811332 voicebox-pytorch-0.0.6/voicebox_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-08-06 00:56:36.000000 voicebox-pytorch-0.0.6/voicebox_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-08-06 00:56:36.000000 voicebox-pytorch-0.0.6/voicebox_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)    16368 2023-08-06 00:56:36.000000 voicebox-pytorch-0.0.6/voicebox_pytorch/voicebox_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 00:56:47.811332 voicebox-pytorch-0.0.6/voicebox_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-08-06 00:56:47.000000 voicebox-pytorch-0.0.6/voicebox_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-08-06 00:56:47.000000 voicebox-pytorch-0.0.6/voicebox_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 00:56:47.000000 voicebox-pytorch-0.0.6/voicebox_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-06 00:56:47.000000 voicebox-pytorch-0.0.6/voicebox_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-06 00:56:47.000000 voicebox-pytorch-0.0.6/voicebox_pytorch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 03:46:48.170486 voicebox-pytorch-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-06 03:46:38.000000 voicebox-pytorch-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-08-06 03:46:48.170486 voicebox-pytorch-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-08-06 03:46:38.000000 voicebox-pytorch-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 03:46:48.170486 voicebox-pytorch-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-08-06 03:46:38.000000 voicebox-pytorch-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 03:46:48.170486 voicebox-pytorch-0.0.7/voicebox_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-08-06 03:46:38.000000 voicebox-pytorch-0.0.7/voicebox_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-08-06 03:46:38.000000 voicebox-pytorch-0.0.7/voicebox_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15934 2023-08-06 03:46:38.000000 voicebox-pytorch-0.0.7/voicebox_pytorch/voicebox_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 03:46:48.170486 voicebox-pytorch-0.0.7/voicebox_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-08-06 03:46:48.000000 voicebox-pytorch-0.0.7/voicebox_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-08-06 03:46:48.000000 voicebox-pytorch-0.0.7/voicebox_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 03:46:48.000000 voicebox-pytorch-0.0.7/voicebox_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-06 03:46:48.000000 voicebox-pytorch-0.0.7/voicebox_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-06 03:46:48.000000 voicebox-pytorch-0.0.7/voicebox_pytorch.egg-info/top_level.txt
```

### Comparing `voicebox-pytorch-0.0.6/LICENSE` & `voicebox-pytorch-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `voicebox-pytorch-0.0.6/PKG-INFO` & `voicebox-pytorch-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voicebox-pytorch
-Version: 0.0.6
+Version: 0.0.7
 Summary: Voicebox - Pytorch
 Home-page: https://github.com/lucidrains/voicebox-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,text to speech
 Classifier: Development Status :: 4 - Beta
```

### Comparing `voicebox-pytorch-0.0.6/README.md` & `voicebox-pytorch-0.0.7/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -18,15 +18,16 @@
 $ pip install voicebox-pytorch
 ```
 
 ## Usage
 
 ```python
 import torch
-from voicebox_pytorch.voicebox_pytorch import (
+
+from voicebox_pytorch import (
     VoiceBox,
     ConditionalFlowMatcherWrapper
 )
 
 model = VoiceBox(
     dim = 512,
     num_phoneme_tokens = 256,
@@ -35,17 +36,17 @@
     heads = 16
 )
 
 cfm_wrapper = ConditionalFlowMatcherWrapper(
     voicebox = model
 )
 
-x = torch.randn(1, 1024, 512)
-phonemes = torch.randint(0, 256, (1, 1024))
-mask = torch.randint(0, 2, (1, 1024))
+x = torch.randn(2, 1024, 512)
+phonemes = torch.randint(0, 256, (2, 1024))
+mask = torch.randint(0, 2, (2, 1024)).bool()
 
 loss = cfm_wrapper(
     x,
     phoneme_ids = phonemes,
     cond = x,
     mask = mask
 )
@@ -54,28 +55,29 @@
 
 # after much training above...
 
 sampled = cfm_wrapper.sample(
     phoneme_ids = phonemes,
     cond = x,
     mask = mask
-)
+) # (2, 1024, 512) <- same as cond
+
 ```
 
 ## Todo
 
 - [x] read and internalize original flow matching paper
     - [x] basic loss
     - [x] get neural ode working with torchdyn
 - [x] get basic mask generation logic with the p_drop of 0.2-0.3 for ICL
+- [x] just use torchdiffeq, nothing else is mature. torchode looks promising but cannot support ndim > 2
 
 - [ ] consider switching to adaptive rmsnorm for time conditioning
 - [ ] integrate with either hifi-gan and soundstream / encodec
 - [ ] basic trainer
-- [ ] look at alternatives to torchsde (torchode, torchdiffeq etc), since the space seems to be immature. perhaps offer way to use different packages and see which ones researcher gets best results with
 
 ## Citations
 
 ```bibtex
 @article{Le2023VoiceboxTM,
     title   = {Voicebox: Text-Guided Multilingual Universal Speech Generation at Scale},
     author  = {Matt Le and Apoorv Vyas and Bowen Shi and Brian Karrer and Leda Sari and Rashel Moritz and Mary Williamson and Vimal Manohar and Yossi Adi and Jay Mahadeokar and Wei-Ning Hsu},
```

#### html2text {}

```diff
@@ -3,33 +3,31 @@
 we will use rotary embeddings. The authors seem unaware that ALiBi cannot be
 straightforwardly used for bidirectional models. ## Appreciation - StabilityAI
 for the generous sponsorship, as well as my other sponsors, for affording me
 the independence to open source artificial intelligence. - Bryan_Chiang for the
 ongoing code review, sharing his expertise on TTS, and pointing me to an_open
 sourced_implementation of conditional flow matching ## Install ```bash $ pip
 install voicebox-pytorch ``` ## Usage ```python import torch from
-voicebox_pytorch.voicebox_pytorch import ( VoiceBox,
-ConditionalFlowMatcherWrapper ) model = VoiceBox( dim = 512, num_phoneme_tokens
-= 256, depth = 2, dim_head = 64, heads = 16 ) cfm_wrapper =
-ConditionalFlowMatcherWrapper( voicebox = model ) x = torch.randn(1, 1024, 512)
-phonemes = torch.randint(0, 256, (1, 1024)) mask = torch.randint(0, 2, (1,
-1024)) loss = cfm_wrapper( x, phoneme_ids = phonemes, cond = x, mask = mask )
-loss.backward() # after much training above... sampled = cfm_wrapper.sample
-( phoneme_ids = phonemes, cond = x, mask = mask ) ``` ## Todo - [x] read and
-internalize original flow matching paper - [x] basic loss - [x] get neural ode
-working with torchdyn - [x] get basic mask generation logic with the p_drop of
-0.2-0.3 for ICL - [ ] consider switching to adaptive rmsnorm for time
-conditioning - [ ] integrate with either hifi-gan and soundstream / encodec -
-[ ] basic trainer - [ ] look at alternatives to torchsde (torchode, torchdiffeq
-etc), since the space seems to be immature. perhaps offer way to use different
-packages and see which ones researcher gets best results with ## Citations
-```bibtex @article{Le2023VoiceboxTM, title = {Voicebox: Text-Guided
-Multilingual Universal Speech Generation at Scale}, author = {Matt Le and
-Apoorv Vyas and Bowen Shi and Brian Karrer and Leda Sari and Rashel Moritz and
-Mary Williamson and Vimal Manohar and Yossi Adi and Jay Mahadeokar and Wei-Ning
-Hsu}, journal = {ArXiv}, year = {2023}, volume = {abs/2306.15687}, url =
-{https://api.semanticscholar.org/CorpusID:259275061} } ``` ```bibtex
-@inproceedings{dao2022flashattention, title = {Flash{A}ttention: Fast and
-Memory-Efficient Exact Attention with {IO}-Awareness}, author = {Dao, Tri and
-Fu, Daniel Y. and Ermon, Stefano and Rudra, Atri and R{\'e}, Christopher},
-booktitle = {Advances in Neural Information Processing Systems}, year = {2022}
-} ```
+voicebox_pytorch import ( VoiceBox, ConditionalFlowMatcherWrapper ) model =
+VoiceBox( dim = 512, num_phoneme_tokens = 256, depth = 2, dim_head = 64, heads
+= 16 ) cfm_wrapper = ConditionalFlowMatcherWrapper( voicebox = model ) x =
+torch.randn(2, 1024, 512) phonemes = torch.randint(0, 256, (2, 1024)) mask =
+torch.randint(0, 2, (2, 1024)).bool() loss = cfm_wrapper( x, phoneme_ids =
+phonemes, cond = x, mask = mask ) loss.backward() # after much training
+above... sampled = cfm_wrapper.sample( phoneme_ids = phonemes, cond = x, mask =
+mask ) # (2, 1024, 512) <- same as cond ``` ## Todo - [x] read and internalize
+original flow matching paper - [x] basic loss - [x] get neural ode working with
+torchdyn - [x] get basic mask generation logic with the p_drop of 0.2-0.3 for
+ICL - [x] just use torchdiffeq, nothing else is mature. torchode looks
+promising but cannot support ndim > 2 - [ ] consider switching to adaptive
+rmsnorm for time conditioning - [ ] integrate with either hifi-gan and
+soundstream / encodec - [ ] basic trainer ## Citations ```bibtex @article
+{Le2023VoiceboxTM, title = {Voicebox: Text-Guided Multilingual Universal Speech
+Generation at Scale}, author = {Matt Le and Apoorv Vyas and Bowen Shi and Brian
+Karrer and Leda Sari and Rashel Moritz and Mary Williamson and Vimal Manohar
+and Yossi Adi and Jay Mahadeokar and Wei-Ning Hsu}, journal = {ArXiv}, year =
+{2023}, volume = {abs/2306.15687}, url = {https://api.semanticscholar.org/
+CorpusID:259275061} } ``` ```bibtex @inproceedings{dao2022flashattention, title
+= {Flash{A}ttention: Fast and Memory-Efficient Exact Attention with {IO}-
+Awareness}, author = {Dao, Tri and Fu, Daniel Y. and Ermon, Stefano and Rudra,
+Atri and R{\'e}, Christopher}, booktitle = {Advances in Neural Information
+Processing Systems}, year = {2022} } ```
```

### Comparing `voicebox-pytorch-0.0.6/setup.py` & `voicebox-pytorch-0.0.7/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'voicebox-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.0.6',
+  version = '0.0.7',
   license='MIT',
   description = 'Voicebox - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/voicebox-pytorch',
   keywords = [
@@ -15,17 +15,15 @@
     'deep learning',
     'text to speech'
   ],
   install_requires=[
     'beartype',
     'einops>=0.6.1',
     'torch>=2.0',
-    'torchdiffeq',
-    'torchdyn==1.0.3',
-    'torchode'
+    'torchdiffeq'
   ],
   classifiers=[
     'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
     'Topic :: Scientific/Engineering :: Artificial Intelligence',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3.6',
```

### Comparing `voicebox-pytorch-0.0.6/voicebox_pytorch/attend.py` & `voicebox-pytorch-0.0.7/voicebox_pytorch/attend.py`

 * *Files identical despite different names*

### Comparing `voicebox-pytorch-0.0.6/voicebox_pytorch/voicebox_pytorch.py` & `voicebox-pytorch-0.0.7/voicebox_pytorch/voicebox_pytorch.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import math
 import torch
 from torch import nn, Tensor, einsum
 from torch.nn import Module
 import torch.nn.functional as F
 
+from torchdiffeq import odeint_adjoint as odeint
+
 from beartype import beartype
 
 from einops import rearrange, repeat, reduce, pack, unpack
 
 from voicebox_pytorch.attend import Attend
 
 from torchdyn.core import NeuralODE
@@ -428,15 +430,15 @@
         times,
         cond_drop_prob = 0.1,
         target = None,
         mask = None,
     ):
         assert cond.shape[-1] == x.shape[-1]
 
-        # auto manage shape of times, for node.traj
+        # auto manage shape of times, for odeint times
 
         if times.ndim == 0:
             times = repeat(times, '-> b', b = cond.shape[0])
 
         if times.ndim == 1 and times.shape[0] == 1:
             times = repeat(times, '1 -> b', b = cond.shape[0])
 
@@ -495,57 +497,38 @@
 
         num = reduce(loss, 'b n -> b', 'sum')
         den = mask.sum(dim = -1).clamp(min = 1e-5)
         loss = num / den
 
         return loss.mean()
 
-# neural ode voicebox wrapper
-
-class NeuralODEVoiceboxWrapper(Module):
-    @beartype
-    def __init__(
-        self,
-        voicebox: VoiceBox
-    ):
-        super().__init__()
-        self.voicebox = voicebox
-        self.forward_kwargs = dict()
-
-    def forward(self, t, x):
-        return self.voicebox.forward_with_cond_scale(x, times = t, **self.forward_kwargs)
-
 # wrapper for the CNF
 
 class ConditionalFlowMatcherWrapper(Module):
     @beartype
     def __init__(
         self,
         voicebox: VoiceBox,
         sigma = 0.,
-        node_solver = 'dopri5',
-        node_sensitivity = 'adjoint',
-        node_atol = 1e-5,
-        node_rtol = 1e-5,
+        ode_atol = 1e-5,
+        ode_rtol = 1e-5,
+        ode_method = 'dopri5',
         cond_drop_prob = 0.,
         prob_seq_drop = 0.3  # not entirely sure
     ):
         super().__init__()
         self.sigma = sigma
 
         self.voicebox = voicebox
         self.cond_drop_prob = cond_drop_prob
 
-        self.prob_seq_drop = prob_seq_drop
-
-        self.node_kwargs = dict(
-            solver = node_solver,
-            sensitivity = node_sensitivity,
-            atol = node_atol,
-            rtol = node_rtol
+        self.odeint_kwargs = dict(
+            atol = ode_atol,
+            rtol = ode_rtol,
+            method= ode_method
         )
 
     @property
     def device(self):
         return next(self.parameters()).device
 
     @torch.inference_mode()
@@ -556,36 +539,32 @@
         cond,
         mask = None,
         steps = 2,
         cond_scale = 1.
     ):
         self.voicebox.eval()
 
-        wrapped_voicebox = NeuralODEVoiceboxWrapper(self.voicebox)
-
-        wrapped_voicebox.forward_kwargs = dict(
-            phoneme_ids = phoneme_ids,
-            cond = cond,
-            mask = mask,
-            cond_scale = cond_scale
-        )
+        def fn(t, x):
+            return self.voicebox.forward_with_cond_scale(
+                x,
+                times = t,
+                phoneme_ids = phoneme_ids,
+                cond = cond,
+                cond_scale = cond_scale
+            )
 
-        node = NeuralODE(
-            wrapped_voicebox,
-            **self.node_kwargs
-        )
+        batch = cond.shape[0]
 
-        print('sampling...')
+        y0 = torch.randn_like(cond)
+        t = torch.linspace(0, 1, steps, device = self.device)
 
-        traj = node.trajectory(
-            torch.randn_like(cond),
-            t_span = torch.linspace(0, 1, steps, device = self.device)
-        )
+        trajectory = odeint(fn, y0, t, adjoint_params=(), **self.odeint_kwargs)
 
-        return traj
+        sampled = trajectory[-1] # last in trajectory
+        return sampled
 
     def forward(
         self,
         x1,
         *,
         phoneme_ids,
         cond,
@@ -598,15 +577,15 @@
 
         batch, seq_len, dtype, σ = *x1.shape[:2], x1.dtype, self.sigma
 
         x0 = torch.randn_like(x1)
 
         # random times
 
-        times = torch.rand((batch,), dtype = dtype)
+        times = torch.rand((batch,), dtype = dtype, device = self.device)
         t = rearrange(times, 'b -> b 1 1')
 
         # sample xt (w in the paper)
 
         w = (1 - (1 - σ) * t) * x0 + t * x1
 
         flow = x1 - (1 - σ) * x0
```

### Comparing `voicebox-pytorch-0.0.6/voicebox_pytorch.egg-info/PKG-INFO` & `voicebox-pytorch-0.0.7/voicebox_pytorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voicebox-pytorch
-Version: 0.0.6
+Version: 0.0.7
 Summary: Voicebox - Pytorch
 Home-page: https://github.com/lucidrains/voicebox-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,text to speech
 Classifier: Development Status :: 4 - Beta
```

