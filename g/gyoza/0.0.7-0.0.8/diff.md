# Comparing `tmp/gyoza-0.0.7.tar.gz` & `tmp/gyoza-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gyoza-0.0.7.tar", last modified: Thu Jul 27 14:52:30 2023, max compression
+gzip compressed data, was "gyoza-0.0.8.tar", last modified: Sun Aug  6 07:45:46 2023, max compression
```

## Comparing `gyoza-0.0.7.tar` & `gyoza-0.0.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 timdick    (501) staff       (20)        0 2023-07-27 14:52:30.326175 gyoza-0.0.7/
--rwxrwxrwx   0 timdick    (501) staff       (20)     1091 2023-06-02 09:45:10.000000 gyoza-0.0.7/LICENSE
--rw-r--r--   0 timdick    (501) staff       (20)     2995 2023-07-27 14:52:30.325736 gyoza-0.0.7/PKG-INFO
--rwxr-xr-x   0 timdick    (501) staff       (20)     2608 2023-07-27 14:35:24.000000 gyoza-0.0.7/README.md
--rwxr-xr-x   0 timdick    (501) staff       (20)      797 2023-07-27 14:50:16.000000 gyoza-0.0.7/pyproject.toml
--rw-r--r--   0 timdick    (501) staff       (20)       38 2023-07-27 14:52:30.326308 gyoza-0.0.7/setup.cfg
--rwxrwxrwx   0 timdick    (501) staff       (20)      173 2023-06-15 09:02:13.000000 gyoza-0.0.7/setup.py
-drwxr-xr-x   0 timdick    (501) staff       (20)        0 2023-07-27 14:52:30.314569 gyoza-0.0.7/src/
-drwxr-xr-x   0 timdick    (501) staff       (20)        0 2023-07-27 14:52:30.316404 gyoza-0.0.7/src/gyoza/
--rw-r--r--   0 timdick    (501) staff       (20)        0 2023-06-07 09:58:20.000000 gyoza-0.0.7/src/gyoza/__init__.py
-drwxr-xr-x   0 timdick    (501) staff       (20)        0 2023-07-27 14:52:30.322547 gyoza-0.0.7/src/gyoza/modelling/
--rwxrwxrwx   0 timdick    (501) staff       (20)        0 2023-06-02 11:33:16.000000 gyoza-0.0.7/src/gyoza/modelling/__init__.py
--rw-r--r--   0 timdick    (501) staff       (20)    13578 2023-07-27 14:11:22.000000 gyoza-0.0.7/src/gyoza/modelling/data_iterators.py
--rwxr-xr-x   0 timdick    (501) staff       (20)    42532 2023-07-27 14:11:22.000000 gyoza-0.0.7/src/gyoza/modelling/flow_layers.py
--rw-r--r--   0 timdick    (501) staff       (20)    12575 2023-07-27 14:11:22.000000 gyoza-0.0.7/src/gyoza/modelling/losses.py
--rw-r--r--   0 timdick    (501) staff       (20)     9161 2023-07-27 14:11:22.000000 gyoza-0.0.7/src/gyoza/modelling/masks.py
--rw-r--r--   0 timdick    (501) staff       (20)     3173 2023-07-27 14:11:22.000000 gyoza-0.0.7/src/gyoza/modelling/standard_layers.py
-drwxr-xr-x   0 timdick    (501) staff       (20)        0 2023-07-27 14:52:30.324920 gyoza-0.0.7/src/gyoza/utilities/
--rwxrwxrwx   0 timdick    (501) staff       (20)        0 2023-06-02 12:24:09.000000 gyoza-0.0.7/src/gyoza/utilities/__init__.py
--rwxr-xr-x   0 timdick    (501) staff       (20)    11781 2023-07-27 14:11:22.000000 gyoza-0.0.7/src/gyoza/utilities/math.py
--rw-r--r--   0 timdick    (501) staff       (20)     3987 2023-07-27 14:11:22.000000 gyoza-0.0.7/src/gyoza/utilities/tensors.py
-drwxr-xr-x   0 timdick    (501) staff       (20)        0 2023-07-27 14:52:30.317880 gyoza-0.0.7/src/gyoza.egg-info/
--rwxrwxrwx   0 timdick    (501) staff       (20)     2995 2023-07-27 14:52:30.000000 gyoza-0.0.7/src/gyoza.egg-info/PKG-INFO
--rwxrwxrwx   0 timdick    (501) staff       (20)      521 2023-07-27 14:52:30.000000 gyoza-0.0.7/src/gyoza.egg-info/SOURCES.txt
--rwxrwxrwx   0 timdick    (501) staff       (20)        1 2023-07-27 14:52:30.000000 gyoza-0.0.7/src/gyoza.egg-info/dependency_links.txt
--rwxrwxrwx   0 timdick    (501) staff       (20)       98 2023-07-27 14:52:30.000000 gyoza-0.0.7/src/gyoza.egg-info/requires.txt
--rwxrwxrwx   0 timdick    (501) staff       (20)        6 2023-07-27 14:52:30.000000 gyoza-0.0.7/src/gyoza.egg-info/top_level.txt
+drwxr-xr-x   0 timdick    (501) staff       (20)        0 2023-08-06 07:45:46.162406 gyoza-0.0.8/
+-rwxrwxrwx   0 timdick    (501) staff       (20)     1091 2023-06-02 09:45:10.000000 gyoza-0.0.8/LICENSE
+-rw-r--r--   0 timdick    (501) staff       (20)      936 2023-08-06 07:45:46.162003 gyoza-0.0.8/PKG-INFO
+-rwxr-xr-x   0 timdick    (501) staff       (20)      493 2023-08-06 07:39:58.000000 gyoza-0.0.8/README.md
+-rwxr-xr-x   0 timdick    (501) staff       (20)      797 2023-08-06 07:39:58.000000 gyoza-0.0.8/pyproject.toml
+-rw-r--r--   0 timdick    (501) staff       (20)       38 2023-08-06 07:45:46.162545 gyoza-0.0.8/setup.cfg
+-rwxrwxrwx   0 timdick    (501) staff       (20)      173 2023-06-15 09:02:13.000000 gyoza-0.0.8/setup.py
+drwxr-xr-x   0 timdick    (501) staff       (20)        0 2023-08-06 07:45:46.150811 gyoza-0.0.8/src/
+drwxr-xr-x   0 timdick    (501) staff       (20)        0 2023-08-06 07:45:46.152877 gyoza-0.0.8/src/gyoza/
+-rw-r--r--   0 timdick    (501) staff       (20)        0 2023-06-07 09:58:20.000000 gyoza-0.0.8/src/gyoza/__init__.py
+drwxr-xr-x   0 timdick    (501) staff       (20)        0 2023-08-06 07:45:46.158985 gyoza-0.0.8/src/gyoza/modelling/
+-rwxrwxrwx   0 timdick    (501) staff       (20)        0 2023-06-02 11:33:16.000000 gyoza-0.0.8/src/gyoza/modelling/__init__.py
+-rw-r--r--   0 timdick    (501) staff       (20)    13578 2023-07-27 14:11:22.000000 gyoza-0.0.8/src/gyoza/modelling/data_iterators.py
+-rwxr-xr-x   0 timdick    (501) staff       (20)    46625 2023-08-06 07:39:58.000000 gyoza-0.0.8/src/gyoza/modelling/flow_layers.py
+-rw-r--r--   0 timdick    (501) staff       (20)    12575 2023-07-27 14:11:22.000000 gyoza-0.0.8/src/gyoza/modelling/losses.py
+-rw-r--r--   0 timdick    (501) staff       (20)     9166 2023-08-06 07:39:58.000000 gyoza-0.0.8/src/gyoza/modelling/masks.py
+-rw-r--r--   0 timdick    (501) staff       (20)     3173 2023-07-27 14:11:22.000000 gyoza-0.0.8/src/gyoza/modelling/standard_layers.py
+drwxr-xr-x   0 timdick    (501) staff       (20)        0 2023-08-06 07:45:46.161195 gyoza-0.0.8/src/gyoza/utilities/
+-rwxrwxrwx   0 timdick    (501) staff       (20)        0 2023-06-02 12:24:09.000000 gyoza-0.0.8/src/gyoza/utilities/__init__.py
+-rwxr-xr-x   0 timdick    (501) staff       (20)    11781 2023-07-27 14:11:22.000000 gyoza-0.0.8/src/gyoza/utilities/math.py
+-rw-r--r--   0 timdick    (501) staff       (20)     3987 2023-07-27 14:11:22.000000 gyoza-0.0.8/src/gyoza/utilities/tensors.py
+drwxr-xr-x   0 timdick    (501) staff       (20)        0 2023-08-06 07:45:46.155062 gyoza-0.0.8/src/gyoza.egg-info/
+-rwxrwxrwx   0 timdick    (501) staff       (20)      936 2023-08-06 07:45:46.000000 gyoza-0.0.8/src/gyoza.egg-info/PKG-INFO
+-rwxrwxrwx   0 timdick    (501) staff       (20)      521 2023-08-06 07:45:46.000000 gyoza-0.0.8/src/gyoza.egg-info/SOURCES.txt
+-rwxrwxrwx   0 timdick    (501) staff       (20)        1 2023-08-06 07:45:46.000000 gyoza-0.0.8/src/gyoza.egg-info/dependency_links.txt
+-rwxrwxrwx   0 timdick    (501) staff       (20)       98 2023-08-06 07:45:46.000000 gyoza-0.0.8/src/gyoza.egg-info/requires.txt
+-rwxrwxrwx   0 timdick    (501) staff       (20)        6 2023-08-06 07:45:46.000000 gyoza-0.0.8/src/gyoza.egg-info/top_level.txt
```

### Comparing `gyoza-0.0.7/LICENSE` & `gyoza-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `gyoza-0.0.7/pyproject.toml` & `gyoza-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [project]
 name = "gyoza"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Tim Dick", email="timdi@icloud.com" },
 ]
 description = ""
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `gyoza-0.0.7/src/gyoza/modelling/data_iterators.py` & `gyoza-0.0.8/src/gyoza/modelling/data_iterators.py`

 * *Files identical despite different names*

### Comparing `gyoza-0.0.7/src/gyoza/modelling/flow_layers.py` & `gyoza-0.0.8/src/gyoza/modelling/flow_layers.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,43 +48,104 @@
         # Attributes
         self.__shape__ = cp.copy(shape)
         """(:class:`List[int]`) - The shape of the input that shall be transformed by this layer. For detail, see constructor of :class:`FlowLayer`"""
 
         self.__axes__ = cp.copy(axes)
         """(:class:`List[int]`) - The axes of transformation. For detail, see constructor of :class:`FlowLayer`"""
 
-    def fit(self, iterator: tf.keras.utils.Sequence, epoch_count: int, batch_count) -> tf.Tensor:
-        """Fits self to data. Assumes that the model is compiled with loss and an optimizer and has a train_step implementation.
+    def fit(self, epoch_count: int, batch_count:int, X:tf.Tensor=None, Y: tf.Tensor=None, batch_size: int=None, iterator: tf.keras.utils.Sequence=None) -> tf.Tensor:
+        """Fits self to data. Assumes that the model is compiled with loss and an optimizer. Unless overwritten by the subclass, this fit
+        method relies on a train_step method that passes an X batch through the model, flattens its output and after flattening the
+        Y batch, computes the loss to apply gradient descent. If ``X``, ``Y``, ``batch_size`` are specified, then no iterator is needed. 
+        Instead an iterator is created that samples ``batch_size`` instances from X and Y uniformly at random. Alternatively, ``X``, 
+        ``Y`` and ``batch_size`` can be omitted if an iterator is provided. 
 
-        :param iterator: An iterator that produces X, Y pairs of shape [batch_size, ...]. 
-        :type iterator: :class:`tf.keras.utils.Sequential`
         :param epoch_count: The number of times self shall be calibrated on `iterator`. 
         :type epoch_count: int
-        :param batch_count: The number of times a new batch shall be drawn from the `iterator`. 
+        :param batch_count: The number of times a new batch shall be drawn from the `iterator` per epoch. 
         :type batch_count: int
+        :param X: Input data to be fed through the network. Shape is assumed to be [instance count, ...], where ... needs to be 
+            compatible with the network.
+        :type X: :class:`tensorflow.Tensor`, optional
+        :param Y: Expected output data to be obtained after feeding ``X`` through the network. Shape is assumed to be [instance count, 
+            ...], where ... needs to be compatible with the network and indexing is assumed to be synchronous with ``X``.
+        :type Y: :class:`tensorflow.Tensor`, optional
+        :param batch_size: The number of instance that shall be sampled per batch.
+        :param iterator: An iterator that produces X, Y pairs of shape [batch_size, ...], where ... needs to be compatible with the 
+            network. 
+        :type iterator: :class:`tf.keras.utils.Sequential`
         :return: 
             - epoch_loss_means (:class:`tensorflow.Tensor`) - The mean loss per epoch. Length == [``epoch_count``].
-            - epoch_loss_standard_deviations (:class:`tensorflow.Tensor`) - The standard_deviation of loss per epoch. Length == [``epoch_count``].
+            - epoch_loss_standard_deviations (:class:`tensorflow.Tensor`) - The standard_deviation of loss per epoch. Length == 
+                [``epoch_count``].
         """
         
+        # Input validity
+        if type(X) != type(None) or type(Y) != type(None) or type(batch_size) != type(None):
+            assert type(X) != type(None) and type(Y) != type(None) and type(batch_size) != type(None) and type(iterator) == type(None), f"If X, Y or batch size are provided, then all need to be provided while iterator shall be none. "
+        else:
+            assert type(iterator) != type(None), f"If neither X, Y, nor batch_size are specified, then an iterator must be provided."
+
+        # Initialization
         epoch_loss_means = [None] * epoch_count
         epoch_loss_standard_deviations = [None] * epoch_count
         batch_losses = [None] * batch_count
+        if type(iterator) == type(None):
+            def iterate(X,Y, batch_size):
+                instance_count = X.shape[0]
+                while True:
+                    indices = np.random.randint(0,instance_count,size=[batch_size])
+                    yield X[indices], Y[indices]
+            iterator = iterate(X=X, Y=Y, batch_size=batch_size)
         
         # Iterate epochs
         for e in range(epoch_count):
             
             # Iterate batches
             for b in range(batch_count): batch_losses[b] = self.train_step(data=next(iterator)).numpy()
             epoch_loss_means[e] = np.mean(batch_losses)
             epoch_loss_standard_deviations[e] = np.std(batch_losses)
 
         # Outputs
         return epoch_loss_means, epoch_loss_standard_deviations
 
+    def train_step(self, data):
+        """Performs one step of gradient descent. Assumes self.optimzer and self.loss are initialized.
+
+        :param data: A tuple containg the batch of X and Y, respectively. X is assumed to be a tensorflow.Tensor of shape [batch size,
+            ...] where ... is the shape of one input instance that has to fit through :py:attr:`self.sequence`. The tensorflow.Tensor
+            Y shall be of same shape of X.
+        :type data: Tuple(tensorflow.Tensor, tensorflow.Tensor)
+        :return: loss: A scalar for the loss observed before applying the train step.
+        """
+        
+        # Unpack inputs
+        X, Y = data
+        
+        with tf.GradientTape() as tape:
+            # Predict
+            Y_hat = self(X, training=True)  # Forward pass
+            
+            # Flatten to apply loss (most keras losses expect flat inputs)
+            Y_flat = tf.reshape(Y, shape=[-1])
+            Y_hat_flat = tf.reshape(Y_hat, shape=[-1])
+            
+            # Compute loss
+            loss = self.loss(y_true=Y_flat, y_pred=Y_hat_flat)
+
+        # Compute gradients
+        trainable_vars = self.trainable_variables
+        gradients = tape.gradient(loss, trainable_vars)
+
+        # Update weights
+        self.optimizer.apply_gradients(zip(gradients, trainable_vars))
+
+        # Outputs
+        return loss
+
     @abc.abstractmethod
     def call(self, x: tf.Tensor) -> tf.Tensor:
         """Executes the operation of this layer in the forward direction.
 
         :param x: The data to be tranformed. Assumed to be of shape [batch size, ...].
         :type x: :class:`tensorflow.Tensor`
         :return: y_hat (:class:`tensorflow.Tensor`) - The output of the transformation of shape [batch size, ...]."""        
@@ -814,16 +875,15 @@
     def __init__(self, sequence: List[FlowLayer], **kwargs):
         
         # Super
         super(SequentialFlowNetwork, self).__init__(shape=[], axes=[], **kwargs) # Shape and axes are set to empty lists here because the individual layers may have different shapes and axes of
         
         # Attributes
         self.sequence = sequence
-        self.loss_tracker = tf.keras.metrics.Mean(name="loss")
-        self.mae_metric = tf.keras.metrics.MeanAbsoluteError(name="mae")
+        """(List[:class:`FlowLayer`]) - Stores the sequence of flow layers through which the data shall be passed."""
 
     def call(self, x: tf.Tensor) -> tf.Tensor:
         
         # Transform
         for layer in self.sequence: x = layer(x=x)
         y_hat = x
 
@@ -847,44 +907,49 @@
             logarithmic_determinant += layer.compute_jacobian_determinant(x=x) 
             x = layer(x=x)
             
         # Outputs
         return logarithmic_determinant
 
 class SupervisedFactorNetwork(SequentialFlowNetwork):
-
+    """This network is a :class:`SequentialFlowNetwork` that can be used to disentangle factors, e.g. to understand representations
+    in latent spaces of regular neural networks. It automatically uses the :class:`losses.SupervisedFactorLoss` to compute its losses.
+    It also overrides the :class:`FlowLayer`'s implementation for train_step to accomodate for the fact that calibration does not
+    simply use single instances but pairs of instances and their similarity.
+    """
+    
     def __init__(self, sequence: List[FlowLayer], dimensions_per_factor: List[int], **kwargs):
         super().__init__(sequence=sequence, **kwargs)
-        self.__loss__ = mls.SupervisedFactorLoss(dimensions_per_factor=dimensions_per_factor)
+        self.loss = mls.SupervisedFactorLoss(dimensions_per_factor=dimensions_per_factor)
 
     def train_step(self, data):
-        """_summary_
+        """Performs one step of gradient descent. Assumes self.optimzer and self.loss are initialized.
 
-        :param data: A tuple containg the batch of X and y, respectively. X is assumed to be a tensorflow.Tensor of shape [batch size,
+        :param data: A tuple containg the batch of X and Y, respectively. X is assumed to be a tensorflow.Tensor of shape [batch size,
             2, ...] where 2 indicates the pair x_a, x_b of same factor and ... is the shape of one input instance that has to fit 
-            through :py:attr:`self.sequence`. The tensorflow.Tensor y shall contain the factor indices of shape [batch size].
+            through :py:attr:`self.sequence`. The tensorflow.Tensor Y shall contain the factor indices of shape [batch size].
         :type data: Tuple(tensorflow.Tensor, tensorflow.Tensor)
-        :return: metrics (Dict[str:tensroflow.keras.metrics.Metric]) - A dictionary of training metrics.
+        :return: loss: A scalar for the loss observed before applying the train step.
         """
         
         # Unpack inputs
-        X, y = data
+        X, Y = data
         z_a = X[:,0,:]; z_b = X[:,1,:]
         
         with tf.GradientTape() as tape:
             # First instance
             z_tilde_a = self(z_a, training=True)  # Forward pass
             j_a = self.compute_jacobian_determinant(x=z_a)
             
             # Second instance
             z_tilde_b = self(z_b, training=True)
             j_b = self.compute_jacobian_determinant(x=z_b)
             
             # Compute loss
-            loss = self.__loss__.compute(y_true=y, y_pred=(z_tilde_a, z_tilde_b, j_a, j_b))
+            loss = self.loss.compute(y_true=Y, y_pred=(z_tilde_a, z_tilde_b, j_a, j_b))
 
         # Compute gradients
         trainable_vars = self.trainable_variables
         gradients = tape.gradient(loss, trainable_vars)
 
         # Update weights
         self.optimizer.apply_gradients(zip(gradients, trainable_vars))
```

### Comparing `gyoza-0.0.7/src/gyoza/modelling/losses.py` & `gyoza-0.0.8/src/gyoza/modelling/losses.py`

 * *Files identical despite different names*

### Comparing `gyoza-0.0.7/src/gyoza/modelling/masks.py` & `gyoza-0.0.8/src/gyoza/modelling/masks.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,15 +157,15 @@
     """
 
     def __init__(self, axes: int, shape: int):
         
         # Set up mask
         mask = np.ones(shape=shape)
         mask = np.reshape(mask, [-1]) # Flattening
-        mask[:shape[0] // 2] = 0
+        mask[:mask.shape[0] // 2] = 0
         mask = tf.constant(mask) 
 
         # Super
         super(Heaviside, self).__init__(axes=axes, shape=shape, mask=mask)
 
 class CheckerBoard(Mask):
     """Applies a `checkerboard <https://en.wikipedia.org/wiki/Check_(pattern)>`_ pattern to its input. Observe that it is equivalent
```

### Comparing `gyoza-0.0.7/src/gyoza/modelling/standard_layers.py` & `gyoza-0.0.8/src/gyoza/modelling/standard_layers.py`

 * *Files identical despite different names*

### Comparing `gyoza-0.0.7/src/gyoza/utilities/math.py` & `gyoza-0.0.8/src/gyoza/utilities/math.py`

 * *Files identical despite different names*

### Comparing `gyoza-0.0.7/src/gyoza/utilities/tensors.py` & `gyoza-0.0.8/src/gyoza/utilities/tensors.py`

 * *Files identical despite different names*

### Comparing `gyoza-0.0.7/src/gyoza.egg-info/SOURCES.txt` & `gyoza-0.0.8/src/gyoza.egg-info/SOURCES.txt`

 * *Files identical despite different names*

