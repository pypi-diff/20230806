# Comparing `tmp/voicebox-pytorch-0.0.4.tar.gz` & `tmp/voicebox-pytorch-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voicebox-pytorch-0.0.4.tar", last modified: Sat Aug  5 16:48:05 2023, max compression
+gzip compressed data, was "voicebox-pytorch-0.0.5.tar", last modified: Sat Aug  5 20:19:34 2023, max compression
```

## Comparing `voicebox-pytorch-0.0.4.tar` & `voicebox-pytorch-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 16:48:05.487434 voicebox-pytorch-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-05 16:47:49.000000 voicebox-pytorch-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-08-05 16:48:05.487434 voicebox-pytorch-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-08-05 16:47:49.000000 voicebox-pytorch-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 16:48:05.487434 voicebox-pytorch-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-08-05 16:47:49.000000 voicebox-pytorch-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 16:48:05.487434 voicebox-pytorch-0.0.4/voicebox_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-08-05 16:47:49.000000 voicebox-pytorch-0.0.4/voicebox_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-08-05 16:47:49.000000 voicebox-pytorch-0.0.4/voicebox_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)    16225 2023-08-05 16:47:49.000000 voicebox-pytorch-0.0.4/voicebox_pytorch/voicebox_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 16:48:05.487434 voicebox-pytorch-0.0.4/voicebox_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-08-05 16:48:05.000000 voicebox-pytorch-0.0.4/voicebox_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-08-05 16:48:05.000000 voicebox-pytorch-0.0.4/voicebox_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 16:48:05.000000 voicebox-pytorch-0.0.4/voicebox_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-05 16:48:05.000000 voicebox-pytorch-0.0.4/voicebox_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-05 16:48:05.000000 voicebox-pytorch-0.0.4/voicebox_pytorch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 20:19:34.324803 voicebox-pytorch-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-05 20:19:25.000000 voicebox-pytorch-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-08-05 20:19:34.324803 voicebox-pytorch-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-08-05 20:19:25.000000 voicebox-pytorch-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 20:19:34.324803 voicebox-pytorch-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-08-05 20:19:25.000000 voicebox-pytorch-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 20:19:34.324803 voicebox-pytorch-0.0.5/voicebox_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-08-05 20:19:25.000000 voicebox-pytorch-0.0.5/voicebox_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-08-05 20:19:25.000000 voicebox-pytorch-0.0.5/voicebox_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16197 2023-08-05 20:19:25.000000 voicebox-pytorch-0.0.5/voicebox_pytorch/voicebox_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 20:19:34.324803 voicebox-pytorch-0.0.5/voicebox_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-08-05 20:19:34.000000 voicebox-pytorch-0.0.5/voicebox_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-08-05 20:19:34.000000 voicebox-pytorch-0.0.5/voicebox_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 20:19:34.000000 voicebox-pytorch-0.0.5/voicebox_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-05 20:19:34.000000 voicebox-pytorch-0.0.5/voicebox_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-05 20:19:34.000000 voicebox-pytorch-0.0.5/voicebox_pytorch.egg-info/top_level.txt
```

### Comparing `voicebox-pytorch-0.0.4/LICENSE` & `voicebox-pytorch-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `voicebox-pytorch-0.0.4/PKG-INFO` & `voicebox-pytorch-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voicebox-pytorch
-Version: 0.0.4
+Version: 0.0.5
 Summary: Voicebox - Pytorch
 Home-page: https://github.com/lucidrains/voicebox-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,text to speech
 Classifier: Development Status :: 4 - Beta
```

### Comparing `voicebox-pytorch-0.0.4/README.md` & `voicebox-pytorch-0.0.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -61,19 +61,21 @@
 )
 ```
 
 ## Todo
 
 - [x] read and internalize original flow matching paper
     - [x] basic loss
-    - [ ] get neural ode working with torchdyn
+    - [x] get neural ode working with torchdyn
+- [x] get basic mask generation logic with the p_drop of 0.2-0.3 for ICL
+
 - [ ] consider switching to adaptive rmsnorm for time conditioning
-- [ ] integrate with either hifi-gan or soundstream / encodec
+- [ ] integrate with either hifi-gan and soundstream / encodec
 - [ ] basic trainer
-- [ ] get basic mask generation logic with the p_drop of 0.2-0.3 for ICL
+- [ ] look at alternatives to torchsde (torchode, torchdiffeq etc), since the space seems to be immature. perhaps offer way to use different packages and see which ones researcher gets best results with
 
 ## Citations
 
 ```bibtex
 @article{Le2023VoiceboxTM,
     title   = {Voicebox: Text-Guided Multilingual Universal Speech Generation at Scale},
     author  = {Matt Le and Apoorv Vyas and Bowen Shi and Brian Karrer and Leda Sari and Rashel Moritz and Mary Williamson and Vimal Manohar and Yossi Adi and Jay Mahadeokar and Wei-Ning Hsu},
```

#### html2text {}

```diff
@@ -11,22 +11,25 @@
 ConditionalFlowMatcherWrapper ) model = VoiceBox( dim = 512, num_phoneme_tokens
 = 256, depth = 2, dim_head = 64, heads = 16 ) cfm_wrapper =
 ConditionalFlowMatcherWrapper( voicebox = model ) x = torch.randn(1, 1024, 512)
 phonemes = torch.randint(0, 256, (1, 1024)) mask = torch.randint(0, 2, (1,
 1024)) loss = cfm_wrapper( x, phoneme_ids = phonemes, cond = x, mask = mask )
 loss.backward() # after much training above... sampled = cfm_wrapper.sample
 ( phoneme_ids = phonemes, cond = x, mask = mask ) ``` ## Todo - [x] read and
-internalize original flow matching paper - [x] basic loss - [ ] get neural ode
-working with torchdyn - [ ] consider switching to adaptive rmsnorm for time
-conditioning - [ ] integrate with either hifi-gan or soundstream / encodec -
-[ ] basic trainer - [ ] get basic mask generation logic with the p_drop of 0.2-
-0.3 for ICL ## Citations ```bibtex @article{Le2023VoiceboxTM, title =
-{Voicebox: Text-Guided Multilingual Universal Speech Generation at Scale},
-author = {Matt Le and Apoorv Vyas and Bowen Shi and Brian Karrer and Leda Sari
-and Rashel Moritz and Mary Williamson and Vimal Manohar and Yossi Adi and Jay
-Mahadeokar and Wei-Ning Hsu}, journal = {ArXiv}, year = {2023}, volume = {abs/
-2306.15687}, url = {https://api.semanticscholar.org/CorpusID:259275061} } ```
-```bibtex @inproceedings{dao2022flashattention, title = {Flash{A}ttention: Fast
-and Memory-Efficient Exact Attention with {IO}-Awareness}, author = {Dao, Tri
-and Fu, Daniel Y. and Ermon, Stefano and Rudra, Atri and R{\'e}, Christopher},
+internalize original flow matching paper - [x] basic loss - [x] get neural ode
+working with torchdyn - [x] get basic mask generation logic with the p_drop of
+0.2-0.3 for ICL - [ ] consider switching to adaptive rmsnorm for time
+conditioning - [ ] integrate with either hifi-gan and soundstream / encodec -
+[ ] basic trainer - [ ] look at alternatives to torchsde (torchode, torchdiffeq
+etc), since the space seems to be immature. perhaps offer way to use different
+packages and see which ones researcher gets best results with ## Citations
+```bibtex @article{Le2023VoiceboxTM, title = {Voicebox: Text-Guided
+Multilingual Universal Speech Generation at Scale}, author = {Matt Le and
+Apoorv Vyas and Bowen Shi and Brian Karrer and Leda Sari and Rashel Moritz and
+Mary Williamson and Vimal Manohar and Yossi Adi and Jay Mahadeokar and Wei-Ning
+Hsu}, journal = {ArXiv}, year = {2023}, volume = {abs/2306.15687}, url =
+{https://api.semanticscholar.org/CorpusID:259275061} } ``` ```bibtex
+@inproceedings{dao2022flashattention, title = {Flash{A}ttention: Fast and
+Memory-Efficient Exact Attention with {IO}-Awareness}, author = {Dao, Tri and
+Fu, Daniel Y. and Ermon, Stefano and Rudra, Atri and R{\'e}, Christopher},
 booktitle = {Advances in Neural Information Processing Systems}, year = {2022}
 } ```
```

### Comparing `voicebox-pytorch-0.0.4/setup.py` & `voicebox-pytorch-0.0.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'voicebox-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.0.4',
+  version = '0.0.5',
   license='MIT',
   description = 'Voicebox - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/voicebox-pytorch',
   keywords = [
@@ -15,14 +15,15 @@
     'deep learning',
     'text to speech'
   ],
   install_requires=[
     'beartype',
     'einops>=0.6.1',
     'torch>=2.0',
+    'torchdiffeq',
     'torchdyn==1.0.3',
     'torchode'
   ],
   classifiers=[
     'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
     'Topic :: Scientific/Engineering :: Artificial Intelligence',
```

### Comparing `voicebox-pytorch-0.0.4/voicebox_pytorch/attend.py` & `voicebox-pytorch-0.0.5/voicebox_pytorch/attend.py`

 * *Files identical despite different names*

### Comparing `voicebox-pytorch-0.0.4/voicebox_pytorch/voicebox_pytorch.py` & `voicebox-pytorch-0.0.5/voicebox_pytorch/voicebox_pytorch.py`

 * *Files 2% similar despite different names*

```diff
@@ -579,35 +579,34 @@
         x1,
         *,
         phoneme_ids,
         cond,
         mask = None,
     ):
         """
-        following the example put forth
-        https://github.com/atong01/conditional-flow-matching/blob/main/torchcfm/conditional_flow_matching.py#L248
+        following eq (5) (6) in https://arxiv.org/pdf/2306.15687.pdf
+        using https://github.com/atong01/conditional-flow-matching/blob/main/torchcfm/conditional_flow_matching.py as reference
         """
-        batch, seq_len, dtype = *x1.shape[:2], x1.dtype
+
+        batch, seq_len, dtype, σ = *x1.shape[:2], x1.dtype, self.sigma
 
         x0 = torch.randn_like(x1)
 
         # random times
 
         times = torch.rand((batch,), dtype = dtype)
-        padded_times = rearrange(times, 'b -> b 1 1')
-
-        # sample xt
+        t = rearrange(times, 'b -> b 1 1')
 
-        mu_t = padded_times * x1
-        sigma_t = 1 - (1 - self.sigma) * padded_times
+        # sample xt (w in the paper)
 
-        eps = torch.rand_like(x1)
-        xt = mu_t + sigma_t * eps
+        mu_t = t * x1
+        σt = (1 - (1 - σ) * t) * x0
+        w = mu_t + σt
 
-        flow = (x1 - (1 - self.sigma) * xt) / sigma_t
+        flow = x1 - (1 - σ) * x0
 
         # construct mask if not given
 
         if (
             not exists(mask) and
             exists(self.prob_seq_drop) and
             self.prob_seq_drop > 0.
@@ -616,15 +615,15 @@
             mask = mask_from_frac_lengths(seq_len, frac_lengths)
 
         # predict
 
         self.voicebox.train()
 
         loss = self.voicebox(
-            xt,
+            w,
             phoneme_ids = phoneme_ids,
             cond = cond,
             mask = mask,
             times = times,
             target = flow,
             cond_drop_prob = self.cond_drop_prob
         )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `voicebox-pytorch-0.0.4/voicebox_pytorch.egg-info/PKG-INFO` & `voicebox-pytorch-0.0.5/voicebox_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voicebox-pytorch
-Version: 0.0.4
+Version: 0.0.5
 Summary: Voicebox - Pytorch
 Home-page: https://github.com/lucidrains/voicebox-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,text to speech
 Classifier: Development Status :: 4 - Beta
```

