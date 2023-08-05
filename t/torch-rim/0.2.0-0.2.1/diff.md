# Comparing `tmp/torch_rim-0.2.0.tar.gz` & `tmp/torch_rim-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_rim-0.2.0.tar", last modified: Sat Aug  5 22:34:20 2023, max compression
+gzip compressed data, was "torch_rim-0.2.1.tar", last modified: Sat Aug  5 22:48:34 2023, max compression
```

## Comparing `torch_rim-0.2.0.tar` & `torch_rim-0.2.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-08-05 22:34:20.679979 torch_rim-0.2.0/
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      450 2023-08-05 22:34:20.679979 torch_rim-0.2.0/PKG-INFO
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     9431 2023-08-05 22:24:19.000000 torch_rim-0.2.0/README.md
-drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-08-05 22:34:20.679979 torch_rim-0.2.0/rim/
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       72 2023-07-30 05:03:49.000000 torch_rim-0.2.0/rim/__init__.py
-drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-08-05 22:34:20.679979 torch_rim-0.2.0/rim/architectures/
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       33 2023-07-30 04:16:22.000000 torch_rim-0.2.0/rim/architectures/__init__.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      364 2023-07-30 04:46:56.000000 torch_rim-0.2.0/rim/architectures/base.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     5896 2023-08-05 22:21:03.000000 torch_rim-0.2.0/rim/architectures/hourglass.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)        7 2023-07-30 05:34:37.000000 torch_rim-0.2.0/rim/architectures/unet.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      108 2023-07-29 23:08:17.000000 torch_rim-0.2.0/rim/definitions.py
-drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-08-05 22:34:20.679979 torch_rim-0.2.0/rim/layers/
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      358 2023-07-31 23:40:45.000000 torch_rim-0.2.0/rim/layers/__init__.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2269 2023-08-01 00:03:41.000000 torch_rim-0.2.0/rim/layers/gru.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1921 2023-07-30 00:22:46.000000 torch_rim-0.2.0/rim/layers/gru_component.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)    23054 2023-08-05 15:09:24.000000 torch_rim-0.2.0/rim/rim.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2926 2023-07-31 19:31:56.000000 torch_rim-0.2.0/rim/utils.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       38 2023-08-05 22:34:20.679979 torch_rim-0.2.0/setup.cfg
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      813 2023-08-05 22:34:09.000000 torch_rim-0.2.0/setup.py
-drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-08-05 22:34:20.679979 torch_rim-0.2.0/tests/
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2137 2023-08-01 00:00:12.000000 torch_rim-0.2.0/tests/test_architectures.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2693 2023-08-01 00:04:18.000000 torch_rim-0.2.0/tests/test_layers.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2956 2023-07-31 12:37:16.000000 torch_rim-0.2.0/tests/test_rim.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3938 2023-08-05 21:32:32.000000 torch_rim-0.2.0/tests/test_training.py
-drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-08-05 22:34:20.679979 torch_rim-0.2.0/torch_rim.egg-info/
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      450 2023-08-05 22:34:20.000000 torch_rim-0.2.0/torch_rim.egg-info/PKG-INFO
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      513 2023-08-05 22:34:20.000000 torch_rim-0.2.0/torch_rim.egg-info/SOURCES.txt
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)        1 2023-08-05 22:34:20.000000 torch_rim-0.2.0/torch_rim.egg-info/dependency_links.txt
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       38 2023-08-05 22:34:20.000000 torch_rim-0.2.0/torch_rim.egg-info/requires.txt
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)        4 2023-08-05 22:34:20.000000 torch_rim-0.2.0/torch_rim.egg-info/top_level.txt
+drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-08-05 22:48:33.999976 torch_rim-0.2.1/
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      450 2023-08-05 22:48:33.999976 torch_rim-0.2.1/PKG-INFO
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     9468 2023-08-05 22:47:23.000000 torch_rim-0.2.1/README.md
+drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-08-05 22:48:33.995976 torch_rim-0.2.1/rim/
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       72 2023-07-30 05:03:49.000000 torch_rim-0.2.1/rim/__init__.py
+drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-08-05 22:48:33.995976 torch_rim-0.2.1/rim/architectures/
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       33 2023-07-30 04:16:22.000000 torch_rim-0.2.1/rim/architectures/__init__.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      364 2023-07-30 04:46:56.000000 torch_rim-0.2.1/rim/architectures/base.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     5896 2023-08-05 22:21:03.000000 torch_rim-0.2.1/rim/architectures/hourglass.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)        7 2023-07-30 05:34:37.000000 torch_rim-0.2.1/rim/architectures/unet.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      108 2023-07-29 23:08:17.000000 torch_rim-0.2.1/rim/definitions.py
+drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-08-05 22:48:33.995976 torch_rim-0.2.1/rim/layers/
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      358 2023-07-31 23:40:45.000000 torch_rim-0.2.1/rim/layers/__init__.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2269 2023-08-01 00:03:41.000000 torch_rim-0.2.1/rim/layers/gru.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1921 2023-07-30 00:22:46.000000 torch_rim-0.2.1/rim/layers/gru_component.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)    23054 2023-08-05 15:09:24.000000 torch_rim-0.2.1/rim/rim.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2926 2023-07-31 19:31:56.000000 torch_rim-0.2.1/rim/utils.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       38 2023-08-05 22:48:33.999976 torch_rim-0.2.1/setup.cfg
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      844 2023-08-05 22:48:10.000000 torch_rim-0.2.1/setup.py
+drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-08-05 22:48:33.995976 torch_rim-0.2.1/tests/
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2137 2023-08-01 00:00:12.000000 torch_rim-0.2.1/tests/test_architectures.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2693 2023-08-01 00:04:18.000000 torch_rim-0.2.1/tests/test_layers.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2956 2023-07-31 12:37:16.000000 torch_rim-0.2.1/tests/test_rim.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3938 2023-08-05 21:32:32.000000 torch_rim-0.2.1/tests/test_training.py
+drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-08-05 22:48:33.999976 torch_rim-0.2.1/torch_rim.egg-info/
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      450 2023-08-05 22:48:33.000000 torch_rim-0.2.1/torch_rim.egg-info/PKG-INFO
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      513 2023-08-05 22:48:33.000000 torch_rim-0.2.1/torch_rim.egg-info/SOURCES.txt
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)        1 2023-08-05 22:48:33.000000 torch_rim-0.2.1/torch_rim.egg-info/dependency_links.txt
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       58 2023-08-05 22:48:33.000000 torch_rim-0.2.1/torch_rim.egg-info/requires.txt
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)        4 2023-08-05 22:48:33.000000 torch_rim-0.2.1/torch_rim.egg-info/top_level.txt
```

### Comparing `torch_rim-0.2.0/README.md` & `torch_rim-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 This is an implementation of a Recurrent Inference Machine (see [Putzky & Welling (2017)](https://arxiv.org/abs/1706.04008)) 
 alongside some standard neural network architectures for the type of problem RIM can solve.
 
 # Installation
 To install the package, you can use pip:
 ```bash
-pip install torch_rim
+pip install torch-rim
 ```
 
 # Usage
 ```python
 from torch_rim import RIM, Hourglass, Unet
 from torch.func import vmap
 
@@ -36,54 +36,55 @@
 net = Hourglass(C, dimensions=len(dimensions))
 rim = RIM(dimensions, net, score_fn=score_fn)
 
 # ... or with the energy function
 rim = RIM(dimensions, net, energy_fn=energy_fn)
 
 # Train the rim, and save its weight in checkpoints_directory
-model.fit(dataset=your_dataset, epochs=100, learning_rate=1e-4, checkpoints_directory=checkpoints_directory)
+rim.fit(dataset, epochs=100, learning_rate=1e-4, checkpoints_directory=checkpoints_directory)
 
 # Make a prediction on an observation y
 x_hat = rim.predict(y, A, Sigma) # of with the signature (y, F, Sigma) with the energy_fn
 
 ```
 
 # Background
 
 A RIM is a gradient-based meta-learning algorithm. It is trained not as a feed-forward neural network, but rather as an optimisation 
 algorithm. More specifically, the RIM is given a *problem instance* specified by a likelihood score $\nabla_\mathbf{x} \log p(y \mid x)$, 
-or more generally a posterior scoe function $\nabla_{\mathbf{x}} \log p(x \mid y)$, and an observation $y$ to condition said posterior. 
+or more generally a posterior scoe function $\nabla_{\mathbf{x} \mid \mathbf{y}} \equiv \nabla_{\mathbf{x}} \log p(x \mid y)$, and an observation $y$ to condition said posterior. 
 
 The RIM uses this information to perform a learned gradient ascent algorithm on the posterior. 
 This procedure will produce a MAP estimate of the parameters of interests $\mathbf{x}$ when the RIM is trained
 ```math
 \begin{align}
-\hat{\mathbf{x}}_{t+1} &= \hat{\mathbf{x}}_t + \mathbf{g}_\theta (\hat{\mathbf{x}}_t, y, \nabla_{\hat{\mathbf{x}}_t} \log p(\hat{\mathbf{x}}_t, \mathbf{y}), \mathbf{h}_t) \hspace{0.5cm} t \in [0, T]\\
-\mathbf{h}_{t+1} &= g_\theta(\hat{\mathbf{x}}_t, \mathbf{y}, \nabla_{\hat{\mathbf{x}}_t} \log p(\hat{\mathbf{x}}_t, \mathbf{y}), \mathbf{h}_t)
+\hat{\mathbf{x}}_{t+1} &= \hat{\mathbf{x}}_t + \mathbf{g}_\theta (\hat{\mathbf{x}}_t,\, \mathbf{y},\, \nabla_{\hat{\mathbf{x}}_t \mid \mathbf{y}},\, \mathbf{h}_t)\\
+\mathbf{h}_{t+1} &= \mathbf{g}_\theta(\hat{\mathbf{x}}_t,\, \mathbf{y},\, \nabla_{\hat{\mathbf{x}}_t \mid \mathbf{y}},\, \mathbf{h}_t)
 \end{align}
 ```
-In the last equation, $g_\theta$ is a neural network that act as the *gradient* in the gradient ascent algorithm. The second equation represent an hidden state 
+for $t \in [0, T]$. 
+In the last equation, $\mathbf{g}_\theta$ is a neural network that act as the *gradient* in the gradient ascent algorithm. The second equation represent an hidden state 
 much like modern optimisation algorithm like ADAM ([Kingma & Ba (2014)](https://arxiv.org/abs/1412.6980)) or RMSProp 
 ([Hinton (2011)](https://www.cs.toronto.edu/~tijmen/csc321/slides/lecture_slides_lec6.pdf)) that uses hidden state to aggregate information 
 about the trajectory of the particle during optimisation. In this case, $\mathbf{h}$ is the hidden state of a Gated Recurrent Unit 
 ([Chung et al. (2014)](https://arxiv.org/abs/1412.3555)).
 
 
 The RIM is trained using an outer loop optimisation contructed with labels $\mathbf{x}$ (the parameters of interests) and a simulator $F$: 
 ```math
-$\mathbf{y} = F(\mathbf{x}) + \boldsymbol{\eta}$. 
+\mathbf{y} = F(\mathbf{x}) + \boldsymbol{\eta}\, . 
 ```
 Equipped with a dataset of problem instances and their solutions $\mathbf{x}$
 ```math
-\mathcal{D} = \{(\mathbf{y}, \mathbf{x}, \nabla_\mathbf{x}\log p(\mathbf{x} \mid \mathbf{y})\}\, ,
+\mathcal{D} = \big\{\mathbf{y}^{(i)},\, \mathbf{x}^{(i)},\, \nabla_{\mathbf{x} \mid \mathbf{y}}^{(i)}\big\}_{i=1}^N\, ,
 ```
 we can train the RIM to make it's gradient ascent trajectories as efficient as possible by minimizing a weighted mean squared 
 loss
 ```math
-\mathcal{L}_\theta = \mathbb{E}_\mathcal{D} \left[ \sum_{t=1}^T\lvert \mathbf{w}_t(\hat{\mathbf{x}}_t - \mahtbf{x}\rVert^2_2 \right]\, .
+\mathcal{L}_\theta = \mathbb{E}_\mathcal{D} \left[ \sum_{t=1}^T\lVert \mathbf{w}_t(\hat{\mathbf{x}}_t - \mathbf{x})\rVert^2_2 \right]\, .
 ```
 $\mathbf{w}_t$ weighs each MSE on the parameter trajectory $\big\{\mathbf{x}_t\big\}_{t=0}^T$.
 
 
 # Citations
 If you find this work useful, please consider citing
 #### [Putzky & Welling (2017)](http://arxiv.org/abs/1706.04008)
```

### Comparing `torch_rim-0.2.0/rim/architectures/hourglass.py` & `torch_rim-0.2.1/rim/architectures/hourglass.py`

 * *Files identical despite different names*

### Comparing `torch_rim-0.2.0/rim/layers/gru.py` & `torch_rim-0.2.1/rim/layers/gru.py`

 * *Files identical despite different names*

### Comparing `torch_rim-0.2.0/rim/layers/gru_component.py` & `torch_rim-0.2.1/rim/layers/gru_component.py`

 * *Files identical despite different names*

### Comparing `torch_rim-0.2.0/rim/rim.py` & `torch_rim-0.2.1/rim/rim.py`

 * *Files identical despite different names*

### Comparing `torch_rim-0.2.0/rim/utils.py` & `torch_rim-0.2.1/rim/utils.py`

 * *Files identical despite different names*

### Comparing `torch_rim-0.2.0/setup.py` & `torch_rim-0.2.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 
 # Read the contents of the README file
 with open("long_description.rst", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='torch_rim',
-    version='0.2.0',
+    version='0.2.1',
     author='Alexandre Adam',
     author_email='alexande.adam@umontreal.ca',
     description='A torch implementation of the Recurrent Inference Machine',
     url="https://github.com/AlexandreAdam/torch_rim",
     packages=find_packages(),
     install_requires=[
         'torch>=2.0',
+        'score_models>=0.4.4',
         "torch_ema",
         'numpy',
         'tqdm',
         'scipy',
     ],
 	python_requires=">=3.8",
     classifiers=[
```

### Comparing `torch_rim-0.2.0/tests/test_architectures.py` & `torch_rim-0.2.1/tests/test_architectures.py`

 * *Files identical despite different names*

### Comparing `torch_rim-0.2.0/tests/test_layers.py` & `torch_rim-0.2.1/tests/test_layers.py`

 * *Files identical despite different names*

### Comparing `torch_rim-0.2.0/tests/test_rim.py` & `torch_rim-0.2.1/tests/test_rim.py`

 * *Files identical despite different names*

### Comparing `torch_rim-0.2.0/tests/test_training.py` & `torch_rim-0.2.1/tests/test_training.py`

 * *Files identical despite different names*

### Comparing `torch_rim-0.2.0/torch_rim.egg-info/SOURCES.txt` & `torch_rim-0.2.1/torch_rim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

