# Comparing `tmp/torch_rim-0.2.4.tar.gz` & `tmp/torch_rim-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_rim-0.2.4.tar", last modified: Sat Aug  5 23:13:59 2023, max compression
+gzip compressed data, was "torch_rim-0.2.5.tar", last modified: Sat Aug  5 23:15:41 2023, max compression
```

## Comparing `torch_rim-0.2.4.tar` & `torch_rim-0.2.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-08-05 23:13:59.203970 torch_rim-0.2.4/
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1081 2023-08-05 23:02:16.000000 torch_rim-0.2.4/LICENSE.txt
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     4999 2023-08-05 23:13:59.203970 torch_rim-0.2.4/PKG-INFO
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     9482 2023-08-05 23:05:36.000000 torch_rim-0.2.4/README.md
-drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-08-05 23:13:59.203970 torch_rim-0.2.4/rim/
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       72 2023-07-30 05:03:49.000000 torch_rim-0.2.4/rim/__init__.py
-drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-08-05 23:13:59.203970 torch_rim-0.2.4/rim/architectures/
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       33 2023-07-30 04:16:22.000000 torch_rim-0.2.4/rim/architectures/__init__.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      364 2023-07-30 04:46:56.000000 torch_rim-0.2.4/rim/architectures/base.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     5896 2023-08-05 22:21:03.000000 torch_rim-0.2.4/rim/architectures/hourglass.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)        7 2023-07-30 05:34:37.000000 torch_rim-0.2.4/rim/architectures/unet.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      108 2023-07-29 23:08:17.000000 torch_rim-0.2.4/rim/definitions.py
-drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-08-05 23:13:59.203970 torch_rim-0.2.4/rim/layers/
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      358 2023-07-31 23:40:45.000000 torch_rim-0.2.4/rim/layers/__init__.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2269 2023-08-01 00:03:41.000000 torch_rim-0.2.4/rim/layers/gru.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1921 2023-07-30 00:22:46.000000 torch_rim-0.2.4/rim/layers/gru_component.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)    23054 2023-08-05 15:09:24.000000 torch_rim-0.2.4/rim/rim.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2926 2023-07-31 19:31:56.000000 torch_rim-0.2.4/rim/utils.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       38 2023-08-05 23:13:59.203970 torch_rim-0.2.4/setup.cfg
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      883 2023-08-05 23:13:56.000000 torch_rim-0.2.4/setup.py
-drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-08-05 23:13:59.203970 torch_rim-0.2.4/tests/
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2137 2023-08-01 00:00:12.000000 torch_rim-0.2.4/tests/test_architectures.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2693 2023-08-01 00:04:18.000000 torch_rim-0.2.4/tests/test_layers.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2956 2023-07-31 12:37:16.000000 torch_rim-0.2.4/tests/test_rim.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3938 2023-08-05 21:32:32.000000 torch_rim-0.2.4/tests/test_training.py
-drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-08-05 23:13:59.203970 torch_rim-0.2.4/torch_rim.egg-info/
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     4999 2023-08-05 23:13:59.000000 torch_rim-0.2.4/torch_rim.egg-info/PKG-INFO
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      525 2023-08-05 23:13:59.000000 torch_rim-0.2.4/torch_rim.egg-info/SOURCES.txt
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)        1 2023-08-05 23:13:59.000000 torch_rim-0.2.4/torch_rim.egg-info/dependency_links.txt
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       58 2023-08-05 23:13:59.000000 torch_rim-0.2.4/torch_rim.egg-info/requires.txt
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)        4 2023-08-05 23:13:59.000000 torch_rim-0.2.4/torch_rim.egg-info/top_level.txt
+drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-08-05 23:15:41.979970 torch_rim-0.2.5/
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1081 2023-08-05 23:02:16.000000 torch_rim-0.2.5/LICENSE.txt
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     4966 2023-08-05 23:15:41.979970 torch_rim-0.2.5/PKG-INFO
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     9482 2023-08-05 23:05:36.000000 torch_rim-0.2.5/README.md
+drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-08-05 23:15:41.979970 torch_rim-0.2.5/rim/
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       72 2023-07-30 05:03:49.000000 torch_rim-0.2.5/rim/__init__.py
+drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-08-05 23:15:41.979970 torch_rim-0.2.5/rim/architectures/
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       33 2023-07-30 04:16:22.000000 torch_rim-0.2.5/rim/architectures/__init__.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      364 2023-07-30 04:46:56.000000 torch_rim-0.2.5/rim/architectures/base.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     5896 2023-08-05 22:21:03.000000 torch_rim-0.2.5/rim/architectures/hourglass.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)        7 2023-07-30 05:34:37.000000 torch_rim-0.2.5/rim/architectures/unet.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      108 2023-07-29 23:08:17.000000 torch_rim-0.2.5/rim/definitions.py
+drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-08-05 23:15:41.979970 torch_rim-0.2.5/rim/layers/
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      358 2023-07-31 23:40:45.000000 torch_rim-0.2.5/rim/layers/__init__.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2269 2023-08-01 00:03:41.000000 torch_rim-0.2.5/rim/layers/gru.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1921 2023-07-30 00:22:46.000000 torch_rim-0.2.5/rim/layers/gru_component.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)    23054 2023-08-05 15:09:24.000000 torch_rim-0.2.5/rim/rim.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2926 2023-07-31 19:31:56.000000 torch_rim-0.2.5/rim/utils.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       38 2023-08-05 23:15:41.979970 torch_rim-0.2.5/setup.cfg
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      883 2023-08-05 23:15:16.000000 torch_rim-0.2.5/setup.py
+drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-08-05 23:15:41.979970 torch_rim-0.2.5/tests/
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2137 2023-08-01 00:00:12.000000 torch_rim-0.2.5/tests/test_architectures.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2693 2023-08-01 00:04:18.000000 torch_rim-0.2.5/tests/test_layers.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2956 2023-07-31 12:37:16.000000 torch_rim-0.2.5/tests/test_rim.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3938 2023-08-05 21:32:32.000000 torch_rim-0.2.5/tests/test_training.py
+drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-08-05 23:15:41.979970 torch_rim-0.2.5/torch_rim.egg-info/
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     4966 2023-08-05 23:15:41.000000 torch_rim-0.2.5/torch_rim.egg-info/PKG-INFO
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      525 2023-08-05 23:15:41.000000 torch_rim-0.2.5/torch_rim.egg-info/SOURCES.txt
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)        1 2023-08-05 23:15:41.000000 torch_rim-0.2.5/torch_rim.egg-info/dependency_links.txt
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       58 2023-08-05 23:15:41.000000 torch_rim-0.2.5/torch_rim.egg-info/requires.txt
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)        4 2023-08-05 23:15:41.000000 torch_rim-0.2.5/torch_rim.egg-info/top_level.txt
```

### Comparing `torch_rim-0.2.4/LICENSE.txt` & `torch_rim-0.2.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `torch_rim-0.2.4/PKG-INFO` & `torch_rim-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch_rim
-Version: 0.2.4
+Version: 0.2.5
 Summary: A torch implementation of the Recurrent Inference Machine
 Home-page: https://github.com/AlexandreAdam/torch_rim
 Author: Alexandre Adam
 Author-email: alexande.adam@umontreal.ca
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -78,18 +78,16 @@
 algorithm. More specifically, the RIM is given a *problem instance* specified by a likelihood score :math:`\nabla_\mathbf{x} \log p(y \mid x)`, 
 or more generally a posterior score function :math:`\nabla_{\mathbf{x} \mid \mathbf{y}} \equiv \nabla_{\mathbf{x}} \log p(x \mid y)`, and an observation :math:`y` to condition said posterior.
 
 The RIM uses this information to perform a learned gradient ascent algorithm on the posterior. This procedure will produce a MAP estimate of the parameters of interests :math:`\mathbf{x}` when the RIM is trained.
 
 .. math::
 
-   \begin{align}
    \hat{\mathbf{x}}_{t+1} &= \hat{\mathbf{x}}_t + \mathbf{g}_\theta (\hat{\mathbf{x}}_t,\, \mathbf{y},\, \nabla_{\hat{\mathbf{x}}_t \mid \mathbf{y}},\, \mathbf{h}_t)\\
    \mathbf{h}_{t+1} &= \mathbf{g}_\theta(\hat{\mathbf{x}}_t,\, \mathbf{y},\, \nabla_{\hat{\mathbf{x}}_t \mid \mathbf{y}},\, \mathbf{h}_t)
-   \end{align}
 
 for :math:`t \in [0, T]`. 
 
 In the last equation, :math:`\mathbf{g}_\theta` is a neural network that act as the *gradient* in the gradient ascent algorithm. The second equation represent an hidden state much like modern optimisation algorithm like ADAM (`Kingma & Ba (2014) <https://arxiv.org/abs/1412.6980>`_) or RMSProp (`Hinton (2011) <https://www.cs.toronto.edu/~tijmen/csc321/slides/lecture_slides_lec6.pdf>`_) that uses hidden state to aggregate information about the trajectory of the particle during optimisation. In this case, :math:`\mathbf{h}` is the hidden state of a Gated Recurrent Unit (`Chung et al. (2014) <https://arxiv.org/abs/1412.3555>`_).
 
 The RIM is trained using an outer loop optimisation contructed with labels :math:`\mathbf{x}` (the parameters of interests) and a simulator :math:`F`: 
 
@@ -107,8 +105,7 @@
 
 .. math::
 
    \mathcal{L}_\theta = \mathbb{E}_\mathcal{D} \left[ \sum_{t=1}^T\lVert \mathbf{w}_t(\hat{\mathbf{x}}_t - \mathbf{x})\rVert^2_2 \right]
 
 :math:`\mathbf{w}_t` weighs each MSE on the parameter trajectory.
 
-
```

### Comparing `torch_rim-0.2.4/README.md` & `torch_rim-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `torch_rim-0.2.4/rim/architectures/hourglass.py` & `torch_rim-0.2.5/rim/architectures/hourglass.py`

 * *Files identical despite different names*

### Comparing `torch_rim-0.2.4/rim/layers/gru.py` & `torch_rim-0.2.5/rim/layers/gru.py`

 * *Files identical despite different names*

### Comparing `torch_rim-0.2.4/rim/layers/gru_component.py` & `torch_rim-0.2.5/rim/layers/gru_component.py`

 * *Files identical despite different names*

### Comparing `torch_rim-0.2.4/rim/rim.py` & `torch_rim-0.2.5/rim/rim.py`

 * *Files identical despite different names*

### Comparing `torch_rim-0.2.4/rim/utils.py` & `torch_rim-0.2.5/rim/utils.py`

 * *Files identical despite different names*

### Comparing `torch_rim-0.2.4/setup.py` & `torch_rim-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of the README file
 with open("long_description.rst", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='torch_rim',
-    version='0.2.4',
+    version='0.2.5',
     author='Alexandre Adam',
     author_email='alexande.adam@umontreal.ca',
     description='A torch implementation of the Recurrent Inference Machine',
     long_description=long_description,
     url="https://github.com/AlexandreAdam/torch_rim",
     packages=find_packages(),
     install_requires=[
```

### Comparing `torch_rim-0.2.4/tests/test_architectures.py` & `torch_rim-0.2.5/tests/test_architectures.py`

 * *Files identical despite different names*

### Comparing `torch_rim-0.2.4/tests/test_layers.py` & `torch_rim-0.2.5/tests/test_layers.py`

 * *Files identical despite different names*

### Comparing `torch_rim-0.2.4/tests/test_rim.py` & `torch_rim-0.2.5/tests/test_rim.py`

 * *Files identical despite different names*

### Comparing `torch_rim-0.2.4/tests/test_training.py` & `torch_rim-0.2.5/tests/test_training.py`

 * *Files identical despite different names*

### Comparing `torch_rim-0.2.4/torch_rim.egg-info/PKG-INFO` & `torch_rim-0.2.5/torch_rim.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-rim
-Version: 0.2.4
+Version: 0.2.5
 Summary: A torch implementation of the Recurrent Inference Machine
 Home-page: https://github.com/AlexandreAdam/torch_rim
 Author: Alexandre Adam
 Author-email: alexande.adam@umontreal.ca
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -78,18 +78,16 @@
 algorithm. More specifically, the RIM is given a *problem instance* specified by a likelihood score :math:`\nabla_\mathbf{x} \log p(y \mid x)`, 
 or more generally a posterior score function :math:`\nabla_{\mathbf{x} \mid \mathbf{y}} \equiv \nabla_{\mathbf{x}} \log p(x \mid y)`, and an observation :math:`y` to condition said posterior.
 
 The RIM uses this information to perform a learned gradient ascent algorithm on the posterior. This procedure will produce a MAP estimate of the parameters of interests :math:`\mathbf{x}` when the RIM is trained.
 
 .. math::
 
-   \begin{align}
    \hat{\mathbf{x}}_{t+1} &= \hat{\mathbf{x}}_t + \mathbf{g}_\theta (\hat{\mathbf{x}}_t,\, \mathbf{y},\, \nabla_{\hat{\mathbf{x}}_t \mid \mathbf{y}},\, \mathbf{h}_t)\\
    \mathbf{h}_{t+1} &= \mathbf{g}_\theta(\hat{\mathbf{x}}_t,\, \mathbf{y},\, \nabla_{\hat{\mathbf{x}}_t \mid \mathbf{y}},\, \mathbf{h}_t)
-   \end{align}
 
 for :math:`t \in [0, T]`. 
 
 In the last equation, :math:`\mathbf{g}_\theta` is a neural network that act as the *gradient* in the gradient ascent algorithm. The second equation represent an hidden state much like modern optimisation algorithm like ADAM (`Kingma & Ba (2014) <https://arxiv.org/abs/1412.6980>`_) or RMSProp (`Hinton (2011) <https://www.cs.toronto.edu/~tijmen/csc321/slides/lecture_slides_lec6.pdf>`_) that uses hidden state to aggregate information about the trajectory of the particle during optimisation. In this case, :math:`\mathbf{h}` is the hidden state of a Gated Recurrent Unit (`Chung et al. (2014) <https://arxiv.org/abs/1412.3555>`_).
 
 The RIM is trained using an outer loop optimisation contructed with labels :math:`\mathbf{x}` (the parameters of interests) and a simulator :math:`F`: 
 
@@ -107,8 +105,7 @@
 
 .. math::
 
    \mathcal{L}_\theta = \mathbb{E}_\mathcal{D} \left[ \sum_{t=1}^T\lVert \mathbf{w}_t(\hat{\mathbf{x}}_t - \mathbf{x})\rVert^2_2 \right]
 
 :math:`\mathbf{w}_t` weighs each MSE on the parameter trajectory.
 
-
```

### Comparing `torch_rim-0.2.4/torch_rim.egg-info/SOURCES.txt` & `torch_rim-0.2.5/torch_rim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

