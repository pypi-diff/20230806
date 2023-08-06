# Comparing `tmp/turbESN-0.0.1.9.4.0.tar.gz` & `tmp/turbESN-0.0.1.9.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turbESN-0.0.1.9.4.0.tar", last modified: Wed Mar  1 14:04:11 2023, max compression
+gzip compressed data, was "turbESN-0.0.1.9.5.0.tar", last modified: Sun Aug  6 07:41:44 2023, max compression
```

## Comparing `turbESN-0.0.1.9.4.0.tar` & `turbESN-0.0.1.9.5.0.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxr-xr-x   0 flhe      (1000) flhe      (1000)        0 2023-03-01 14:04:11.657563 turbESN-0.0.1.9.4.0/
--rw-r--r--   0 flhe      (1000) flhe      (1000)     1075 2022-07-17 17:27:10.000000 turbESN-0.0.1.9.4.0/LICENSE
--rw-r--r--   0 flhe      (1000) flhe      (1000)      810 2023-03-01 14:04:11.654230 turbESN-0.0.1.9.4.0/PKG-INFO
--rw-r--r--   0 flhe      (1000) flhe      (1000)     2746 2022-11-14 14:33:47.000000 turbESN-0.0.1.9.4.0/README.md
--rw-r--r--   0 flhe      (1000) flhe      (1000)       38 2023-03-01 14:04:11.657563 turbESN-0.0.1.9.4.0/setup.cfg
--rw-r--r--   0 flhe      (1000) flhe      (1000)     1417 2023-01-07 14:36:31.000000 turbESN-0.0.1.9.4.0/setup.py
-drwxr-xr-x   0 flhe      (1000) flhe      (1000)        0 2023-03-01 14:04:11.654230 turbESN-0.0.1.9.4.0/turbESN/
--rw-r--r--   0 flhe      (1000) flhe      (1000)      129 2023-01-17 15:26:20.000000 turbESN-0.0.1.9.4.0/turbESN/__init__.py
--rw-r--r--   0 flhe      (1000) flhe      (1000)      757 2023-03-01 12:28:19.000000 turbESN-0.0.1.9.4.0/turbESN/_modes.py
--rw-r--r--   0 flhe      (1000) flhe      (1000)       73 2023-03-01 14:04:08.000000 turbESN-0.0.1.9.4.0/turbESN/_version.py
--rw-r--r--   0 flhe      (1000) flhe      (1000)    61074 2023-03-01 14:00:55.000000 turbESN-0.0.1.9.4.0/turbESN/core.py
--rw-r--r--   0 flhe      (1000) flhe      (1000)     7557 2023-03-01 14:01:57.000000 turbESN-0.0.1.9.4.0/turbESN/cross_validation.py
--rw-r--r--   0 flhe      (1000) flhe      (1000)    18406 2023-03-01 14:00:35.000000 turbESN-0.0.1.9.4.0/turbESN/study.py
--rw-r--r--   0 flhe      (1000) flhe      (1000)    58062 2023-03-01 09:52:53.000000 turbESN-0.0.1.9.4.0/turbESN/util (conflicted copy 2023-03-01 105253).py
--rw-r--r--   0 flhe      (1000) flhe      (1000)    60797 2023-03-01 14:00:53.000000 turbESN-0.0.1.9.4.0/turbESN/util.py
-drwxr-xr-x   0 flhe      (1000) flhe      (1000)        0 2023-03-01 14:04:11.654230 turbESN-0.0.1.9.4.0/turbESN.egg-info/
--rw-r--r--   0 flhe      (1000) flhe      (1000)      810 2023-03-01 14:04:11.000000 turbESN-0.0.1.9.4.0/turbESN.egg-info/PKG-INFO
--rw-r--r--   0 flhe      (1000) flhe      (1000)      367 2023-03-01 14:04:11.000000 turbESN-0.0.1.9.4.0/turbESN.egg-info/SOURCES.txt
--rw-r--r--   0 flhe      (1000) flhe      (1000)        1 2023-03-01 14:04:11.000000 turbESN-0.0.1.9.4.0/turbESN.egg-info/dependency_links.txt
--rw-r--r--   0 flhe      (1000) flhe      (1000)       30 2023-03-01 14:04:11.000000 turbESN-0.0.1.9.4.0/turbESN.egg-info/requires.txt
--rw-r--r--   0 flhe      (1000) flhe      (1000)        8 2023-03-01 14:04:11.000000 turbESN-0.0.1.9.4.0/turbESN.egg-info/top_level.txt
+drwxr-xr-x   0 flhe      (1000) flhe      (1000)        0 2023-08-06 07:41:44.055768 turbESN-0.0.1.9.5.0/
+-rw-r--r--   0 flhe      (1000) flhe      (1000)     1075 2022-07-17 17:27:10.000000 turbESN-0.0.1.9.5.0/LICENSE
+-rw-r--r--   0 flhe      (1000) flhe      (1000)      810 2023-08-06 07:41:44.055768 turbESN-0.0.1.9.5.0/PKG-INFO
+-rw-r--r--   0 flhe      (1000) flhe      (1000)     3336 2023-03-04 14:55:59.000000 turbESN-0.0.1.9.5.0/README.md
+-rw-r--r--   0 flhe      (1000) flhe      (1000)       38 2023-08-06 07:41:44.055768 turbESN-0.0.1.9.5.0/setup.cfg
+-rw-r--r--   0 flhe      (1000) flhe      (1000)     1417 2023-01-07 14:36:31.000000 turbESN-0.0.1.9.5.0/setup.py
+drwxr-xr-x   0 flhe      (1000) flhe      (1000)        0 2023-08-06 07:41:44.055768 turbESN-0.0.1.9.5.0/turbESN/
+-rw-r--r--   0 flhe      (1000) flhe      (1000)      129 2023-08-06 07:39:21.000000 turbESN-0.0.1.9.5.0/turbESN/__init__.py
+-rw-r--r--   0 flhe      (1000) flhe      (1000)      757 2023-08-06 07:22:29.000000 turbESN-0.0.1.9.5.0/turbESN/_modes.py
+-rw-r--r--   0 flhe      (1000) flhe      (1000)       73 2023-08-06 07:40:18.000000 turbESN-0.0.1.9.5.0/turbESN/_version.py
+-rw-r--r--   0 flhe      (1000) flhe      (1000)    65165 2023-08-06 07:38:42.000000 turbESN-0.0.1.9.5.0/turbESN/core.py
+-rw-r--r--   0 flhe      (1000) flhe      (1000)     7638 2023-08-06 07:38:55.000000 turbESN-0.0.1.9.5.0/turbESN/cross_validation.py
+-rw-r--r--   0 flhe      (1000) flhe      (1000)    18414 2023-08-06 07:39:18.000000 turbESN-0.0.1.9.5.0/turbESN/study.py
+-rw-r--r--   0 flhe      (1000) flhe      (1000)    61562 2023-08-06 07:38:18.000000 turbESN-0.0.1.9.5.0/turbESN/util.py
+drwxr-xr-x   0 flhe      (1000) flhe      (1000)        0 2023-08-06 07:41:44.055768 turbESN-0.0.1.9.5.0/turbESN.egg-info/
+-rw-r--r--   0 flhe      (1000) flhe      (1000)      810 2023-08-06 07:41:43.000000 turbESN-0.0.1.9.5.0/turbESN.egg-info/PKG-INFO
+-rw-r--r--   0 flhe      (1000) flhe      (1000)      315 2023-08-06 07:41:43.000000 turbESN-0.0.1.9.5.0/turbESN.egg-info/SOURCES.txt
+-rw-r--r--   0 flhe      (1000) flhe      (1000)        1 2023-08-06 07:41:43.000000 turbESN-0.0.1.9.5.0/turbESN.egg-info/dependency_links.txt
+-rw-r--r--   0 flhe      (1000) flhe      (1000)       30 2023-08-06 07:41:43.000000 turbESN-0.0.1.9.5.0/turbESN.egg-info/requires.txt
+-rw-r--r--   0 flhe      (1000) flhe      (1000)        8 2023-08-06 07:41:43.000000 turbESN-0.0.1.9.5.0/turbESN.egg-info/top_level.txt
```

### Comparing `turbESN-0.0.1.9.4.0/LICENSE` & `turbESN-0.0.1.9.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `turbESN-0.0.1.9.4.0/PKG-INFO` & `turbESN-0.0.1.9.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turbESN
-Version: 0.0.1.9.4.0
+Version: 0.0.1.9.5.0
 Summary: An echo state network implementation.
 Home-page: UNKNOWN
 Author: flohey (Florian Heyder)
 Author-email: <florian.heyder@protonmail.com>
 License: UNKNOWN
 Keywords: python,ESN,reservoir computing,echo state network,recurrent neural network
 Platform: UNKNOWN
```

### Comparing `turbESN-0.0.1.9.4.0/README.md` & `turbESN-0.0.1.9.5.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -8,30 +8,43 @@
 
 ## Requirements
 Stable for
 - `python `>=  3.6.0
 - `torch`  >= 1.10.0
 - `numpy`  >= 1.20.1
 - `h5py`   >= 2.10.0 
+- `pyYAML` >= 6.0
 
 ## Manual
 A first basic introduction can be found in the notbeook`basic_tour.ipynb`.  This example uses data from the Lorenz '63 system (https://en.wikipedia.org/wiki/Lorenz_system).
 
 ## About Echo State Networks/ Reservoir Computing
 Classical Reservoir Computing  (RC) makes use of a nonlinear dynamical expansion of the information to be processed. This information is lifted to a high-dimensional reservoir state. A linear readout after each reservoir update yields the reservoir output. The training scheme of RC is concerned with finding the right hyperplane of within the reservoir space, s.t. the reservoir output matches the expected output.Therefore only the linear readout is trained, usually to minimize the mean square error between output and target. Therefore the readout can be computed by a simple linear regression (often with Tikhonov regularization/ L2 penalty). This, always converging learning procedure, makes RC an extremely computationally efficient method.
 RC is more then just a method, it stands for new computing paradigm (in contrast to the Turing-von Neumann architecture).
 
 The Echo State Network (ESN) is a certain implementation of RC. Its architecture follows a Recurrent Neural Network (RNN) structure, where only the output weights are trained by linear regression. This is also a simple way of circumventing the known exploding/ vanishing gradient problem which RNN suffer from.
 
-## Applications:
+## Our applications:
 - F. Heyder and J. Schumacher - Phys. Rev. E **103**, 053107 (2021):
   "Echo state network for two-dimensional turbulent moist Rayleigh-Bénard convection"
 
 - P. Pfeffer, F. Heyder and J. Schumacher - Phys Rev. Res. **4**, 033176 (2022): 
   "Hybrid quantum-classical reservoir computing of thermal convection flow"
 
 - F. Heyder and J. P. Mellado and J. Schumacher - Phys. Rev. E **106**, 055303 (2022): 
   "Generalizability of reservoir computing for flux-driven two-dimensional convection"
 
 - M. S. Ghazijahani, F. Heyder, J. Schumacher and C. Cierpka, Meas. Sci. Technol. **34** (2023) 014002 
   "On the benefits and limitations of Echo State Networks for turbulent flow prediction"
 
+
+## References: ESN good practices
+
+### Getting started
+- M. Lukoševičius - Tricks of the Trade. Lecture Notes in Computer Science, Vol. 7700 (2012): "A Practical Guide to Applying Echo State Networks".
+
+### Cross-Validation
+- M. Lukoševičius and A. Uselis - Cogn. Comput. (2021): "Efficient Implementations of Echo State Network Cross-Validation"
+
+### Random Searches
+- X. Hinaut and N. Trouvain - (2021) Artificial Neural Networks and Machine Learning – ICANN 2021: "Which Hype for My New Task? Hints and Random Search for Echo State Networks Hyperparameter"
+
```

### Comparing `turbESN-0.0.1.9.4.0/setup.py` & `turbESN-0.0.1.9.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `turbESN-0.0.1.9.4.0/turbESN/_modes.py` & `turbESN-0.0.1.9.5.0/turbESN/_modes.py`

 * *Files identical despite different names*

### Comparing `turbESN-0.0.1.9.4.0/turbESN/core.py` & `turbESN-0.0.1.9.5.0/turbESN/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,14 +124,16 @@
 
 
         # Init to None
         self.y_train = None           
         self.u_train = None
         self.y_test  = None
         self.u_test  = None
+        self.u_pre_test = None
+        self.y_pre_test = None
         self.y_val   = None
         self.u_val   = None
         self.u_pre_val = None
         self.y_pre_val = None
 
         self.test_init_input = None
         self.val_init_input  = None
@@ -147,22 +149,22 @@
 
         self.loss_func = None
 #--------------------------------------------------------------------------     
 #--------------------------------------------------------------------------
 #  ESN IMPLEMENTATION
 #--------------------------------------------------------------------------
 #--------------------------------------------------------------------------
-    def createInputMatrix(self):
+    def create_input_matrix(self):
         '''
         Random initialization of the input weights. The weights are drawn from U[-0.5,0.5] or N[0,1] and subsequently scaled by inputScaling.
         '''
         
         logger.debug('Building input matrix')
 
-        if self.weightGeneration == 'normal':
+        if self.weightGeneration == _WEIGTH_GENERATION[1]:
             self.Win = torch.randn(self.n_reservoir, 1 + self.n_input, device = self.device, dtype = _DTYPE)
         else:
             self.Win = torch.rand(self.n_reservoir, 1 + self.n_input, device = self.device, dtype = _DTYPE) - 0.5
 
 
         if self.inputDensity >= 1e-6:
             _mask = torch.rand(self.n_reservoir, 1 + self.n_input, dtype = _DTYPE, device = self.device) > self.inputDensity
@@ -185,23 +187,23 @@
             _inputScaling = self.inputScaling
 
         _inputScaling = torch.vstack((torch.tensor(1, device = self.device, dtype = _DTYPE), _inputScaling.reshape(-1,1))).flatten()
 
         self.Win *= _inputScaling.reshape(1,1+self.n_input)
         
 #--------------------------------------------------------------------------
-    def createReservoirMatrix(self):
+    def create_reservoir_matrix(self):
         '''
-        Random initialization of reservoir weights. The weights are drawn from U[-0.5,0.5]. The reservoir density is set.
+        Random initialization of reservoir weights. The weights are drawn from U[-0.5,0.5] or N[0,1] . The reservoir density is set.
         Finally, the largest absolute eigenvalue is computed, by which Wres is normalized. Then Wres is scaled by the spectral radius.
         '''
             
         logger.debug('Building reservoir matrix')
 
-        if self.weightGeneration == 'normal':
+        if self.weightGeneration == _WEIGTH_GENERATION[1]:
             self.Wres = torch.as_tensor(torch.randn(self.n_reservoir, self.n_reservoir, dtype = _DTYPE, device = self.device) , dtype = _DTYPE, device = self.device)
         else:
             self.Wres = torch.as_tensor(torch.rand(self.n_reservoir, self.n_reservoir, dtype = _DTYPE, device = self.device) - 0.5, dtype = _DTYPE, device = self.device)
  
         #prevent all-zero eigenvals 
         if self.reservoirDensity >= 1e-6 and self.spectralRadius != 0.0:
 
@@ -210,21 +212,21 @@
             self.Wres[_mask] = 0.0
             _eig_norm = torch.abs(torch.linalg.eigvals(self.Wres))
             self.Wres *= self.spectralRadius / torch.max(_eig_norm)
         else:
             self.Wres = torch.zeros((self.n_reservoir, self.n_reservoir), dtype = _DTYPE, device = self.device)
 
 #--------------------------------------------------------------------------
-    def createFeebackMatrix(self):
+    def create_feeback_matrix(self):
         '''
         Random initialization of feedback weights. The weights are drawn from U[-0.5,0.5] or N[0,1] and subsequently scaled by feedbackScaling.
         '''
         logger.debug('Building feedback matrix')
 
-        if self.weightGeneration == 'normal':
+        if self.weightGeneration == _WEIGTH_GENERATION[1]:
             self.Wfb = torch.randn(self.n_reservoir, self.n_output, device = self.device, dtype = _DTYPE)
         else:
             self.Wfb = torch.rand(self.n_reservoir, self.n_output, device = self.device, dtype = _DTYPE) - 0.5
 
 
         # Feedback Scaling
         #------------------
@@ -243,31 +245,31 @@
         self.Wfb *= _feedbackScaling.reshape(1,self.n_output)
         
 #--------------------------------------------------------------------------
     def createWeightMatrices(self):
         '''
         Reservoir initialization. The (fixed) weight matrices Win and Wres are created.
         '''
-        self.createInputMatrix()
-        self.createReservoirMatrix()
+        self.create_input_matrix()
+        self.create_reservoir_matrix()
 
         if self.use_feedback:
-            self.createFeebackMatrix()
+            self.create_feeback_matrix()
 
 #--------------------------------------------------------------------------
     def calculate_activation_argument(self, u: torch.Tensor, x: torch.Tensor, y: torch.Tensor) -> torch.Tensor:
         ''' 
-        Computes input and state contributions to the activation function.
+        Computes input, state and feedback contributions to the activation function argument:  Win@u + Wres@x + Wfb@y
         
         INPUT:
             u - current reservoir input
             x - last reservoir state
             y - last reservoir output
-        RETURN: Win@u + Wres@x + Wfb@y
-            
+        RETURN: 
+            Win@u + Wres@x + Wfb@y
         '''
         
         uu = u.reshape(self.n_input, 1)
         feedback = 0
 
         if self.use_feedback:
             yy = y.reshape(self.n_output, 1)
@@ -418,19 +420,21 @@
                     
         
         logger.warn('Reservoir states did not converge.')
         return torch.inf
 #--------------------------------------------------------------------------
     def fit(self, X: torch.Tensor, y: torch.Tensor):
         '''
-        Reservoir output weights Wout is computed by L2 penalized linear regression.
+        Compute output weights Wout. Depending on fit_method, Wout is compute by:
+        - L2 penalized linear regression
+        - pseudo inverse 
 
         INPUT:
-            X - reservoir state matrix
-            y - target training output
+            X - reservoir state matrix (training phase)
+            y - target training outputs
         '''
 
         logger.debug('Fitting output matrix')
         assert X.shape[1] == y.shape[0], "Time dimension of X ({0}) does not match time dimension of y ({1}).\nDid you forget to exclude the transientTime of y? ".format(X.shape[1], y.shape[0])
         
         if self.fit_method == "tikhonov":
             I = torch.eye(self.xrows, device = self.device)
@@ -617,38 +621,61 @@
             pred_input = pred_output
 
 
         return y_pred.T, x_pred
 
 
 #--------------------------------------------------------------------------     
-#--------------------------------------------------------------------------
 #  HYPERPARAMETER SETTERS
 #--------------------------------------------------------------------------
-#--------------------------------------------------------------------------
-    
-    #FH 01/02/2021: Added SetTrainingData & SetTestingData
+ 
     #--------------------------------------------------------------------------
-    def SetTrainingData(self, u_train: torch.Tensor, y_train: torch.Tensor):
+    def set_training_data(self, u_train: torch.Tensor, y_train: torch.Tensor):
+        '''
+        INPUT:
+            u_train - training input  data, shape (trainingLength, n_input)
+            y_train - training output/target data, shape (trainingLength, n_output)
+        '''
         
         assert u_train.shape[0] == y_train.shape[0],'Training input dimension ({0}) does not match training output time dimension ({1}).\n'.format(u_train.shape[0], y_train.shape[0])
         assert u_train.shape[1] == self.n_input,'Training input dimension ({0}) does not match ESN n_input ({1}).\n'.format(u_train.shape[1], self.n_input)
         assert y_train.shape[1] == self.n_output, 'Training output dimension ({0}) does not match ESN n_output ({1}).\n'.format(y_train.shape[1], self.n_output)
         
         self.u_train = u_train
         self.y_train = y_train
     
     #--------------------------------------------------------------------------
-    def SetTestingData(self, y_test: torch.Tensor, test_init_input: torch.Tensor = None, u_test: torch.Tensor = None):       
-        
+    def set_testing_data(self, 
+                         y_test: torch.Tensor,
+                         u_test: torch.Tensor = None,
+                         test_init_input: torch.Tensor = None, 
+                         u_pre_test: torch.Tensor=None,
+                         y_pre_test: torch.Tensor=None):       
+        '''
+        INPUT:
+            y_test          - ground truth output, shape (testingLenght, n_output)
+            u_test          - ground truth input, shape (testingLenght, n_input)
+            test_init_input - initial input in testing phase (optional), shape (1, n_input)
+            u_pre_test      - user-defined input used for building up reservoir state before testing phase (optinonal), shape (length, n_input)
+            y_pre_test      - user-defined output used for building up reservoir state before testing phase (optional & only required if self.use_feedback is True), shape (length, n_output)
+        '''
+
         assert y_test.shape[1] == self.n_output,'Testing output dimension ({0}) does not match ESN n_output ({1}).\n'.format(y_test.shape[1], self.n_output)
     
         self.y_test = y_test
         self.u_test = u_test
 
+        # Check pre-testing reservoir state build up
+        if u_pre_test is not None:
+            self.u_pre_test = u_pre_test
+
+            if self.use_feedback:
+                assert y_pre_test is not None, 'When using feedback & pre testing state propagation (u_pre_test) a target output has to be provided!'
+                self.y_pre_test = y_pre_test
+
         if self.mode == _ESN_MODES[0]:
 
             if self.y_train is None:
                 assert test_init_input is not None, 'Initial testing input and self.y_train not specified.\n'
 
             if self.y_train is not None and test_init_input is None:
                 #Initial input is last training input. Then first prediction aligns with the first entry of y_test
@@ -665,21 +692,28 @@
 
             if test_init_input is not None:
                 self.test_init_input = test_init_input
 
                 #TO DO: test_init_input has len n_input. The teacher part of it is not used (see self.semiteacherforce).
 
     #--------------------------------------------------------------------------
-    # FH 30.03.2022: Added Validation Datset (auto mode!)
-    def SetValidationData(self, 
+    def set_validation_data(self, 
                           y_val: torch.Tensor, 
                           u_val: torch.Tensor=None, 
                           val_init_input: torch.Tensor=None, 
                           u_pre_val: torch.Tensor=None,
                           y_pre_val: torch.Tensor=None):   
+        '''
+        INPUT:
+            y_val          - ground truth output, shape (validationLength, n_output)
+            u_val          - ground truth input, shape (validationLength, n_input)
+            val_init_input - initial input in validaiton phase (optional), shape (1, n_input)
+            u_pre_val      - user-defined input used for building up reservoir state before testing phase (optinonal), shape (length, n_input)
+            y_pre_val      - user-defined output used for building up reservoir state before validation phase (optional & only required if self.use_feedback is True), shape (length, n_output)
+        '''
 
         assert y_val.shape[1] == self.n_output,'Validation output dimension ({0}) does not match ESN n_output ({1}).\n'.format(y_val.shape[1], self.n_output)
         
         if self.mode == _ESN_MODES[1]:
             assert u_val is not None, 'Teacher mode requires non empty u_val!\n'
 
         if u_pre_val is not None:
@@ -699,15 +733,14 @@
         if self.mode == _ESN_MODES[0]:
             if val_init_input is None:
                 #Initial input is last testing input. Then first prediction aligns with the first entry of y_val
                 logger.debug('Initial validation input not specified. Using last target test output.')
                 self.val_init_input = self.y_test[-1:,:]    #initial input the trained ESN receives for the beginning of the validation phase
             else:
                 self.val_init_input = val_init_input
-
     
     #--------------------------------------------------------------------------
     def SetID(self, esn_id):
     
         logger.debug(f'Setting reservoir ID to {esn_id}')
         self.id = esn_id
 
@@ -729,15 +762,15 @@
         
         study_dict['n_input'] = n_input
      #--------------------------------------------------------------------------
     def SetNReservoir(self,n_reservoir: int, study_dict: dict = {}):
 
         logger.debug(f'Setting n_reservoir {n_reservoir}')
         
-        self.n_reservoir = n_reservoir
+        self.n_reservoir = int(n_reservoir)
 
         #adjust xrows as according to changed n_reservoir
         if self.extendedStateStyle == _EXTENDED_STATE_STYLES[0]:
             self.xrows = int(1+self.n_reservoir+self.n_input)           
         else:
             self.xrows = int(1+2*self.n_reservoir)
 
@@ -919,20 +952,18 @@
                 self.SetTransientTime(config_istudy[iparam], study_dict)
 
             else:
                 logger.critical('Specified parameter {0} unknown.'.format(parameter))
                 raise KeyError
                 
         return study_dict
-
-#--------------------------------------------------------------------------     
+ 
 #--------------------------------------------------------------------------
 #  MISC. IMPLEMENTATIONS
 #--------------------------------------------------------------------------
-#--------------------------------------------------------------------------
     def to_torch(self):
         '''
         Moves the ESN object to python or torch types. Torch tensors are automatically shifted to device.
         This will stop numpy vs. torch clashes from happening.
         '''
         
         logger.debug('Moving class arrays to {0} with dtype {1}'.format(self.device, _DTYPE))
@@ -962,23 +993,31 @@
                 else:
                     new_value = value
                     
                 setattr(self, member, new_value)       
             
 #--------------------------------------------------------------------------
     def set_device(self, device: str):
-        ''' Set globael ESN device (cpu or cuda)'''
+        ''' Set globael ESN device (cpu or cuda) & move all members to it.'''
         
         logger.debug('Setting device: {0}'.format(device))
         self.device = device
-        
+
+        allmembers = [m for m in dir(self) if m[:2] != '__' and m[-2:] != '__']
+        ifaddmember = [not callable(getattr(self, name)) for name in allmembers ]        
+        for ii,member in enumerate(allmembers):
+            if ifaddmember[ii]:
+                value = getattr(self,member)
+                if isinstance(value, torch.Tensor):
+                    setattr(self, member, value.to(self.device))  
+
 #---------------------------------------------------------------------------
     def get_size(self):
         """
-        Returns estimated size of ESN object in MB.
+        Returns estimated size of ESN object in MB. 
 
         RETURN:
             obj_size - estimated size of all torch.Tensors, np.ndarrays in MB
         """
 
         obj_size = 0
         
@@ -1194,18 +1233,19 @@
         
         return esn
 
  #--------------------------------------------------------------------------
     @classmethod
     def read_yaml(cls, filepath:str):
         '''
-        Creates an ESN object from a yaml config file.
+        Creates an ESN object from a yaml config file. 
+        Note that training, testing, validation data must be computed and set separately.
 
         INPUT:
-            filepath - path to the saved ESN 
+            filepath - path to the YAML config file
 
         RETURN:
             esn - ESN object
         '''
 
         logger.warn('Reading ESN parameters from YAML file {0}'.format(filepath))
 
@@ -1242,14 +1282,17 @@
             print(f"{key} - " +val["INFO"])
 
  #--------------------------------------------------------------------------
     @classmethod
     def get_HP_dict(cls):
         '''
             Returns hyperparameter dict.
+
+            RETURN:
+                HP_dict - hyperparameter dict
         '''
         return HP_dict
 
 #--------------------------------------------------------------------------     
 #--------------------------------------------------------------------------
 #  Standard ESNs
 #--------------------------------------------------------------------------
@@ -1372,7 +1415,39 @@
 
         bins = [bins_input,bins_input,bins_res,bins_fb]
         hist = [hist_total, hist_input, hist_res, hist_fb]
         
         return hist,bins
 
 #--------------------------------------------------------------------------
+
+
+
+#--------------------------------------------------------------------------     
+#  DEPRECATED (will be removed in newer versions)
+#--------------------------------------------------------------------------
+    def SetTrainingData(self, u_train: torch.Tensor, y_train: torch.Tensor):
+        '''DEPRECATED, will be removed in newer versions'''
+        self.set_training_data(u_train=u_train, y_train=y_train)
+
+    #--------------------------------------------------------------------------
+    def SetTestingData(self, 
+                       y_test: torch.Tensor,
+                       u_test: torch.Tensor = None,
+                       test_init_input: torch.Tensor = None, 
+                       u_pre_test: torch.Tensor=None,
+                       y_pre_test: torch.Tensor=None):  
+        '''DEPRECATED, will be removed in newer versions'''
+        self.set_testing_data(y_test=y_test, u_test=u_test, test_init_input=test_init_input, u_pre_test=u_pre_test, y_pre_test=y_pre_test)
+
+    #--------------------------------------------------------------------------
+    def SetValidationData(self, 
+                          y_val: torch.Tensor, 
+                          u_val: torch.Tensor=None, 
+                          val_init_input: torch.Tensor=None, 
+                          u_pre_val: torch.Tensor=None,
+                          y_pre_val: torch.Tensor=None): 
+        '''DEPRECATED, will be removed in newer versions'''
+        self.set_validation_data(y_val=y_val,u_val=u_val,val_init_input=val_init_input, u_pre_val=u_pre_val, y_pre_val=y_pre_val)
+
+    #--------------------------------------------------------------------------
+
```

### Comparing `turbESN-0.0.1.9.4.0/turbESN/cross_validation.py` & `turbESN-0.0.1.9.5.0/turbESN/cross_validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,18 @@
     def prepare_k_fold_walk_forward_validation_auto_data(self, 
                                                         data: Union[np.ndarray, torch.Tensor], 
                                                         esn_start: int,
                                                         esn_end: int,
                                                         n_folds: int, 
                                                         fold_length: int = None):
         '''Prepares the data for k fold walk forward validation, see Lukosevicius et al. (2021). Divides the data into n_folds w. length fold_length.
-        The cross validation will use the folds to create three parts: training (incl. transient), validation, testing
+        The cross validation will use the folds to create three parts: 
+        1. training (incl. transient)
+        2. validation (labeled testing here)
+        3. testing (labeled validaiton here)
         For this method n_output = n_input must be valid. 
 
         INPUT:
             data           - data to use for ESN. Shape: (datatimesteps, n_input/n_output)
             esn_start      - Index of the original data, at which the training will begin. 
             esn_end        - Index of the original data, at which the testing will end.
             n_folds        - no. folds into which data will be divided into
@@ -80,15 +83,15 @@
 
         n_input = data.shape[1]
         data_esn = data[esn_start-1:esn_end,:]
 
         if fold_length is None:
             fold_length = (esn_end - esn_start)//n_folds     # choose fold_length according to data length
 
-        assert esn_end - esn_start  >= n_folds*fold_length, f"Error: Chosen n_folds {n_folds} and fold_length {fold_length} do not fit in specified interval {esn_end - esn_start} steps"
+        assert esn_end - esn_start  >= n_folds*fold_length, f"Error: Chosen n_folds {n_folds} and fold_length {fold_length} do not fit in specified interval of {esn_end - esn_start} steps"
 
         data_folded_u = data_esn[0:int(n_folds*fold_length),:].reshape(n_folds,fold_length,n_input)
         data_folded_y = data_esn[1:int(n_folds*fold_length)+1,:].reshape(n_folds,fold_length,n_input)
         
         return torch.as_tensor(data_folded_u,dtype=_DTYPE), torch.as_tensor(data_folded_y,dtype=_DTYPE)
 
 
@@ -120,17 +123,14 @@
         G_data.create_dataset('data_folded_u',   data = self.data_folded_u, compression = 'gzip', compression_opts = 9)
         G_data.create_dataset('data_folded_y',   data = self.data_folded_y, compression = 'gzip', compression_opts = 9)
 
         
         if toClose:
             f.close()
 
-
-
-
 #--------------------------------------------------------------------------     
 #--------------------------------------------------------------------------
 #  CLASS METHODS
 #--------------------------------------------------------------------------
 #--------------------------------------------------------------------------
     @classmethod
     def read(cls, filepath: str, esn: ESN):
```

### Comparing `turbESN-0.0.1.9.4.0/turbESN/study.py` & `turbESN-0.0.1.9.5.0/turbESN/study.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,16 +28,16 @@
 
 #Data structure
 import h5py
 import json
 
 # Read hyperparameter.json
 import importlib.resources as pkg_resources
-hp_dict_path = '/home/flhe/nextcloud/Promotion/python/esn/github/turbESN/turbESN/hyperparameters.json'
-logging_config_path = '/home/flhe/nextcloud/Promotion/python/esn/github/turbESN/turbESN/logging_config.json'
+#hp_dict_path = '/home/flhe/nextcloud/Promotion/python/esn/github/turbESN/turbESN/hyperparameters.json'
+#logging_config_path = '/home/flhe/nextcloud/Promotion/python/esn/github/turbESN/turbESN/logging_config.json'
 
 with pkg_resources.path(__package__,'hyperparameters.json') as hp_dict_path:
     with open(hp_dict_path,'r') as f:
         HP_dict = json.load(f)   
 with pkg_resources.path(__package__,'logging_config.json') as logging_config_path:
     with open(logging_config_path,'r') as f:
         LOGGING_CONFIG = json.load(f)
@@ -122,19 +122,19 @@
             recompute_Win = True
         if HP_dict[param]["CHANGES_Wres"]:
             recompute_Wres = True
         if HP_dict[param]["CHANGES_Wfb"]:
             recompute_Wfb = True
         
     if not recompute_Win:
-        esn.createInputMatrix()
+        esn.create_input_matrix()
     if not recompute_Wres:
-        esn.createReservoirMatrix()
+        esn.create_reservoir_matrix()
     if not recompute_Wfb:
-        esn.createFeebackMatrix()
+        esn.create_feeback_matrix()
 
     #----------------------------------
     #Launch ThreadPool
     #----------------------------------
     executor = futures.ThreadPoolExecutor(MAX_THREADS)
 
     with executor as ex:
```

### Comparing `turbESN-0.0.1.9.4.0/turbESN/util (conflicted copy 2023-03-01 105253).py` & `turbESN-0.0.1.9.5.0/turbESN/util.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,58 +7,62 @@
 #backends
 import numpy as np
 import torch
 
 #save data structure
 import h5py 
 import json
+import yaml
 
 #misc
 import sys
 import os
 from copy import deepcopy
 import logging
 import logging.config
 
 from typing import Union, Tuple, List
 
 from scipy.stats import wasserstein_distance
 from scipy.stats import loguniform, uniform
 
-
 # Read hyperparameter.json
+#hp_dict_path = '/home/flhe/nextcloud/Promotion/python/esn/github/turbESN/turbESN/hyperparameters.json'
+#logging_config_path = '/home/flhe/nextcloud/Promotion/python/esn/github/turbESN/turbESN/logging_config.json'
+
 import importlib.resources as pkg_resources
 with pkg_resources.path(__package__,'hyperparameters.json') as hp_dict_path:
     with open(hp_dict_path,'r') as f:
         HP_dict = json.load(f)  
 with pkg_resources.path(__package__,'logging_config.json') as logging_config_path:
     with open(logging_config_path,'r') as f:
         LOGGING_CONFIG = json.load(f)
 
 logging.config.dictConfig(LOGGING_CONFIG)
 logger = logging.getLogger('turbESNlogger')
 
 
 ###########################################################################################################
 
-#                             PRE-PROCESSING/ IMPORTING
+#                             Pre-Processing & Importing
 
 ###########################################################################################################
 #--------------------------------------------------------------------------
 def prepare_auto_data(data: Union[np.ndarray, torch.Tensor],
                          n_input: int, 
                          trainingLength: int, 
                          testingLength: int, 
                          esn_start: int, 
                          esn_end: int,
                          validationLength: int=None) -> Union[Tuple[torch.Tensor,torch.Tensor,torch.Tensor,torch.Tensor],Tuple[torch.Tensor,torch.Tensor,torch.Tensor,torch.Tensor,torch.Tensor,torch.Tensor]]:
-    ''' Prepares the input and output training and testing/validation data set for the autonomous predictor ESN case, i.e. where in the
-        testing pase, the output data is fed back into the reservoir input layer.
-        The data set u_test is therefore not needed, as there is only one initial input in the testing phase.
-        Note that n_output = n_input. 
+    ''' 
+    Prepares the input and output training and testing/validation data set for the autonomous predictor ESN case, i.e. where in the
+    testing pase, the output data is fed back into the reservoir input layer.
+    The data set u_test is therefore not needed, as there is only one initial input in the testing phase.
+    Note that n_output = n_input. 
 
     INPUT:
         data           - data array which is supposed to be used for the ESN. The shape must be (data_timesteps, nmodes)
         n_input        - input dimensions/ no. input modes
         trainingLength - no. time steps for the training data set
         testingLength  - no. time steps for the testing/validation data set
         esn_start      - Index of the original data, at which the training output y_train will begin. 
@@ -95,20 +99,21 @@
                         n_input: int, 
                         n_output: int, 
                         trainingLength: int, 
                         testingLength: int, 
                         esn_start: int, 
                         esn_end: int,
                         validationLength: int = None) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor, torch.Tensor]:
-    ''' Prepares the input and output training and testing/validation data set for the teacher forced ESN case, i.e. where the
-        reservoir input is a teacher signal. 
+    ''' 
+    Prepares the input and output training and testing/validation data set for the teacher forced ESN case, i.e. where the
+    reservoir input is a teacher signal. 
 
     INPUT:
-        data_in        - data array to be used for the ESN. The shape must be (data_timesteps, n_input)
-        data_out       - data array to be used for the ESN. The shape must be (data_timesteps, n_output)
+        data_in        - data array to be used for the ESN. Shape must be (data_timesteps, n_input)
+        data_out       - data array to be used for the ESN. Shape must be (data_timesteps, n_output)
         n_input        - input dimensions/ no. input modes
         n_output       - output dimensions/ no. output modes
         trainingLength - no. time steps for the training data set
         testingLength  - no. time steps for the testing/validation data set
         validationLength -  no. time steps for the validation data set
         esn_start      - Index of the original data, at which the training output y_train will begin. 
         esn_end        - Index of the original data, at which the testing/validation output y_test will end.
@@ -144,29 +149,31 @@
 
     return u_train.to(_DTYPE), y_train.to(_DTYPE), u_test.to(_DTYPE), y_test.to(_DTYPE), u_val.to(_DTYPE), y_val.to(_DTYPE)
     #return torch.as_tensor(u_train, dtype = _DTYPE), torch.as_tensor(y_train, dtype = _DTYPE),torch.as_tensor(u_test, dtype = _DTYPE),torch.as_tensor(y_test, dtype = _DTYPE), torch.as_tensor(u_val, dtype = _DTYPE),torch.as_tensor(y_val, dtype = _DTYPE)
 
 
 #--------------------------------------------------------------------------
 def init_study_order(nsetting: int, study_parameters: list) -> list:
-    ''' Initializes the study parameter settings into an array.
+    ''' 
+    Initializes the study parameter settings into an array.
 
     INPUT:
         nsetting         - number of different reservoir settings that were studied. If nsetting = None, the number is deduced from the file.
         study_parameters - list specifying the values of the parameters that are studied
 
     RETURN: 
         config - list indicating the parameter setting for given study
     ''' 
     
     assert len(study_parameters) != 0,'study_parameters are empty. Did you forget to specify the range of the studied HP?'
     assert nsetting > 0, 'nsetting ({0}) must be > 0'.format(nsetting)
 
     def recursion(iparam: int, iterators: np.ndarray, study_tuple: tuple):
-        ''' Iterates the iterators which are used to change the hyperparmeters. 
+        ''' 
+        Iterates the iterators which are used to change the hyperparmeters. 
             Makes sure that all combinations of the parameters in study_tuple are used.
 
             INPUT:
                 iparam           - index which defines the hyperparameter that is changed
                 iterators        - iterator that defines the no. ESNs that have been run with changing one hyperparameter (study_tuple[iparam]) 
                 study_tuple      - tuple specifying the range of the parameters that are studies
 
@@ -203,15 +210,16 @@
 
         config.append(temp)
 
     return config
 
 #--------------------------------------------------------------------------
 def init_random_search(nsetting: int, study_tuple: tuple, limits: list = []) -> list:
-    ''' Initializes the hyperparameter study parameter settings for a random search. 
+    ''' 
+    Initializes the hyperparameter study parameter settings for a random search. 
         Each of the nsetting settings is given by an entry of the returned list config.
 
     INPUT:
         nsetting         - number of different reservoir setting that should be studied
         study_tuple      - tuple specifying the parameters that are studied
         limits           - user specified range values of hyperparameters in study_tuple: [val_min, val_max, nval, use_log]  
     RETURN: 
@@ -250,15 +258,15 @@
 #--------------------------------------------------------------------------
 def init_grid_search(study_tuple, limits, lists):
     ''' Initializes the hyperparameter study parameter settings for a grid search. 
 
     INPUT:
         study_tuple      - tuple specifying the parameters that are studied
         limits           - user specified range values of hyperparameters in study_tuple: [val_min, val_max, nval, use_log]  
-        limits           - user specified values of the hyperparameters in study_tuple:   [val1, val2, val3,...] 
+        lists            - user specified values of the hyperparameters in study_tuple:   [val1, val2, val3,...] 
         
     RETURN: 
         config   - array indicating the parameter setting for given study
         nsetting - number of different reservoir setting that should be studied
     '''
 
     study_parameters = []
@@ -270,15 +278,16 @@
 
         # HP grid is computed from user specified ranges
         else:
             assert len(limit) == 4, "Error: limits must be of style [value_min, value_max, nvals, use_log]!"
             xmin, xmax, nx, use_log = limit
 
             if use_log:
-                param_val = np.logspace(xmin,xmax,nx)
+                assert xmin > 0 and xmax > 0, 'Error: min./max. GS value must be > 0 in log-scale'
+                param_val = np.logspace(np.log10(xmin),np.log10(xmax),nx)
             else:
                 param_val = np.linspace(xmin,xmax,nx)
 
         study_parameters.append(param_val)   
 
     assert len(study_parameters) == len(study_tuple),f"Error: Length of study_tuple ({len(study_tuple)})  does not match no. study parameters ({len(study_parameters)})!\n"
     nsetting = np.prod([len(param_arr) for param_arr in study_parameters])
@@ -336,34 +345,40 @@
 
     RETURN:
         x_unscaled - data in original range(x_min,x_max)
     '''
 
     return 0.5*(x/dataScaling+1)*(x_max-x_min)+x_min
 
-#--------------------------------------------------------------------------
+###########################################################################################################
+
+#                            Running an ESN
+
+###########################################################################################################
 #FH 30.03.2022: added check_user_input (prev. in run_turbESN)
 def check_user_input(esn, u_train: Union[np.ndarray, torch.Tensor]=None, 
                     y_train:Union[np.ndarray, torch.Tensor]=None, 
                     y_test:Union[np.ndarray, torch.Tensor]=None, 
                     test_init_input:Union[np.ndarray, torch.Tensor]=None, 
                     u_test:Union[np.ndarray, torch.Tensor]=None, 
                     u_val:Union[np.ndarray, torch.Tensor]=None, 
                     y_val:Union[np.ndarray, torch.Tensor]=None,
                     val_init_input: Union[np.ndarray, torch.Tensor]=None, 
                     u_pre_val:Union[np.ndarray, torch.Tensor]=None,
+                    u_pre_test:Union[np.ndarray, torch.Tensor]=None,
                     loss_func:dict=None):
 
-    '''Checks data provided by user. The ESN object might get modified by this method.'''
+    '''
+    Checks data provided by user. The ESN object might get modified by this method.
+    '''
 
     #---------------------------------------
     # Check whether user data is compatiable 
     # (data from esn object is assumed to be correct)
     #---------------------------------------
-
     assert None not in [u_train, y_train, y_test] or None not in [esn.u_train, esn.y_train, esn.y_test], "Error: u_train, y_train or y_test not specified."
 
     if None not in [u_train, y_train, y_test]:
         for data in [u_train, y_train]:
             if esn.trainingLength != data.shape[0]:
                 logger.error('Training input/output time dimension ({0}) does not match ESN trainingLength ({1}).'.format(data.shape[0],esn.trainingLength))
 
@@ -383,169 +398,174 @@
     if test_init_input is not None:
         if test_init_input.dtype is not _DTYPE:
             test_init_input = torch.as_tensor(test_init_input, dtype = _DTYPE)
         if test_init_input.device is not esn.device:
             test_init_input.to(esn.device)
 
     if None not in [u_train, y_train, y_test]:
-        esn.SetTrainingData(u_train=u_train, y_train=y_train)
-        esn.SetTestingData(y_test=y_test, test_init_input=test_init_input, u_test=u_test)
+        esn.set_training_data(u_train=u_train, y_train=y_train)
+        esn.set_testing_data(y_test=y_test, test_init_input=test_init_input, u_test=u_test, u_pre_test=u_pre_test)
 
     if None not in [u_val, y_val]:
-        esn.SetValidationData(y_val=y_val, u_val=u_val, val_init_input=val_init_input,u_pre_val=u_pre_val)
+        esn.set_validation_data(y_val=y_val, u_val=u_val, val_init_input=val_init_input, u_pre_val=u_pre_val)
 
     if loss_func is not None:
         esn.loss_func = loss_func
     else:
         if esn.loss_func is None:
             esn.loss_func = dict(mse=compute_mse)
 
     esn.to_torch()
-###########################################################################################################
-
-#                            RUNNING AN ESN
-
-###########################################################################################################
 
+#--------------------------------------------------------------------------
 def run_turbESN(esn, 
                 u_train: Union[np.ndarray, torch.Tensor]=None, 
                 y_train: Union[np.ndarray, torch.Tensor]=None, 
                 y_test: Union[np.ndarray, torch.Tensor]=None, 
                 test_init_input: Union[np.ndarray, torch.Tensor]=None, 
                 u_test: Union[np.ndarray, torch.Tensor]=None, 
                 u_val: Union[np.ndarray, torch.Tensor]=None,
                 y_val: Union[np.ndarray, torch.Tensor]=None,
                 val_init_input:Union[np.ndarray, torch.Tensor]=None, 
                 u_pre_val:Union[np.ndarray,torch.Tensor]=None,
+                u_pre_test:Union[np.ndarray,torch.Tensor]=None,
                 index_list_auto: list = [], index_list_teacher: list = [],
                 recompute_Win:bool=True,
                 recompute_Wres:bool=True,
                 recompute_Wfb:bool=True,
                 loss_func:dict=None) -> Tuple[dict,torch.Tensor,torch.Tensor]:
 
-    ''' Runs the turbulent Echo State Network (turbESN) with the specified parameters. 
-        The training and testing data must be specfied in the argument or in the esn object.
+    ''' Runs the Echo State Network with the specified parameters. The training and testing data must be specfied in the argument or in the esn object.
         Optional: validation data (third dataset for cross validation, note naming convention (commonly: training/validation/testing, here: training/testing/validation))
-    
+        If an error occurs during training, the method returns zero predictions and losses with a defualt value _LOSS_DEFAULT .
+
         INPUT: 
             esn                - ESN class object. Contains the reservoir parameters. May contain training, testing and validation data sets.
-            u_train            - training input (optional if esn.u_train not None)
-            y_train            - training output (optional if esn.y_train not None)
-            u_test             - testing input (optional if esn.u_test not None)
-            y_test             - testing output (optional if esn.y_test not None)
-            test_init_input    - initial input in testing phase from which prediction start
+            u_train            - training input  (optional if esn.u_train is not None)
+            y_train            - training output (optional if esn.y_train is not None)
+            u_test             - testing input   (optional if esn.u_test is not None)
+            y_test             - testing output  (optional if esn.y_test is not None)
+            test_init_input    - initial input in testing phase from which prediction starts
             u_val              - validation input (optional)
             y_val              - validation output (optional)
-            val_init_input     - initial input in validation phase from which prediction starts (only if esn.mode = _ESN_MODES[1])
-            u_pre_val          - data used to build up reservoir state for start of validation phase (if None, last instance of self.x_test will be used)
-            index_list_auto    - indices of the modes which are passed back as new input (only if esn.mode = _ESN_MODES[2])
-            index_list_teacher - indices of the modes which are supplied by a teacher signal (only if esn.mode = _ESN_MODES[2])
-            recompute_Win      - whether input matrix must be initialized
-            recompute_Wres     - whether reservoir matrix must be initialized
-            recompute_Wfb      - whether feedback matrix must be initialized
+            val_init_input     - initial input in validation phase from which prediction starts (optional, only used if esn.mode == 'auto')
+            u_pre_val          - data used to build up initial reservoir state of validation phase (if None, last instance of esn.x_test will be used)
+            u_pre_test         - data used to build up initial reservoir state of testing phase (if None, last instance of esn.x_train will be used)
+            index_list_auto    - list of indices of the modes which are passed back as new input     (only if esn.mode == 'semi-teacher')
+            index_list_teacher - list of indices of the modes which are supplied by a teacher signal (only if esn.mode == 'semi-teacher')
+            recompute_Win      - bool whether input matrix must be initialized
+            recompute_Wres     - bool whether reservoir matrix must be initialized
+            recompute_Wfb      - bool whether feedback matrix must be initialized
             loss_func          - dict containing the loss function used for prediction evalutation
             
         RETURN:
-            loss_dic    - dictionary containing the losses specified in loss_func
+            loss_dict   - dictionary containing the losses specified in loss_func
             y_pred_test - reseroir outputs of testing phase
             y_pred_val  - reseroir outputs of validation phase
             
     '''
     torch.manual_seed(esn.randomSeed)  
 
     check_user_input(esn=esn,
-                    u_train=u_train,
-                    y_train=y_train,
-                    u_test=u_test,
-                    y_test=y_test,
-                    test_init_input=test_init_input,
-                    u_val=u_val,
-                    y_val=y_val,
-                    val_init_input=val_init_input,
-                    u_pre_val=u_pre_val,
-                    loss_func=loss_func)
+                     u_train=u_train,
+                     y_train=y_train,
+                     u_test=u_test,
+                     y_test=y_test,
+                     test_init_input=test_init_input,
+                     u_val=u_val,
+                     y_val=y_val,
+                     val_init_input=val_init_input,
+                     u_pre_val=u_pre_val,
+                     u_pre_test=u_pre_test,
+                     loss_func=loss_func)
 
     loss_dict = {}
     ##############################################
     # Run ESN
     ##############################################
     
     #----------------------------------------------------------
     #1. Create Random Matrices
     #----------------------------------------------------------
     if recompute_Win:
-        esn.createInputMatrix()
+        esn.create_input_matrix()
     if recompute_Wres:
-        esn.createReservoirMatrix()
+        esn.create_reservoir_matrix()
     if esn.use_feedback and recompute_Wfb:
-        esn.createFeebackMatrix()
+        esn.create_feeback_matrix()
 
     #----------------------------------------------------------
     #2. Training Phase
     #----------------------------------------------------------
     logger.debug('Training ESN')
-    esn.x_train=esn.propagate(u = esn.u_train, transientTime = esn.transientTime,y=esn.y_train)
+    esn.x_train=esn.propagate(u=esn.u_train, transientTime=esn.transientTime, y=esn.y_train)
     esn.fit(X=esn.x_train, y=esn.y_train[esn.transientTime:])
     loss_dict['mse_train']  = compute_mse(y_true=esn.y_train[esn.transientTime:], y_pred=(esn.Wout@esn.x_train).T)
     
     # Check for errors in training
-    #-----------------------------
-    if np.isnan(esn.Wout).any() or loss_dict['mse_train']  is None:
+    #-------------------------------
+    if torch.isnan(esn.Wout).any() or loss_dict['mse_train'] is None:
         logger.error("Reservoir {0}: while fitting the model, an error occured. Assuming default values.".format(esn.id))
         loss_dict['mse_train']  = torch.tensor([_LOSS_DEFAULT for _ in range(int(esn.trainingLength-esn.transientTime))],device = esn.device,dtype = _DTYPE)
         default_test = torch.tensor([_LOSS_DEFAULT for _ in range(esn.testingLength)],device = esn.device,dtype = _DTYPE)       
         default_val = torch.tensor([_LOSS_DEFAULT for _ in range(esn.validationLength)],device = esn.device,dtype = _DTYPE)
     
         loss_test, loss_val = [], []
         if esn.loss_func is not None:
             for loss_label in esn.loss_func.keys():
                 loss_dict[loss_label+'_test'] = default_test
                 
                 if None not in [esn.u_val, esn.y_val]:
                     loss_dict[loss_label+'_val']  = default_val
                 
         y_pred_test = torch.zeros([esn.testingLength, esn.n_output], device = esn.device, dtype = _DTYPE)
-        y_pred_val = torch.zeros([esn.validationLength, esn.n_output], device = esn.device, dtype = _DTYPE)
+        y_pred_val  = torch.zeros([esn.validationLength, esn.n_output], device = esn.device, dtype = _DTYPE)
 
         return loss_dict, y_pred_test, y_pred_val
 
     #----------------------------------------------------------
-    #3. Prediction/Testing Phase (Default:'auto')
+    # 3. Testing Phase
     #----------------------------------------------------------
     logger.debug('Testing ESN')
+
+    # Initialize reservoir state by user-defined GT data
+    if esn.u_pre_test is not None:
+        X_pre_test = esn.propagate(u=esn.u_pre_test, transientTime = esn.u_pre_test.shape[0]-1,y=esn.y_pre_test)
+    else:
+        X_pre_test = esn.x_train
+
+    # Run ESN
     if esn.mode == _ESN_MODES[0]:
-        y_pred_test, esn.x_test = esn.predict(X = esn.x_train, testingLength = esn.testingLength)
+        y_pred_test, esn.x_test = esn.predict(X=X_pre_test, testingLength=esn.testingLength)
 
     elif esn.mode == _ESN_MODES[1]:
-        y_pred_test, esn.x_test = esn.teacherforce(X = esn.x_train, testingLength = esn.testingLength)
+        y_pred_test, esn.x_test = esn.teacherforce(X=X_pre_test, testingLength=esn.testingLength)
   
     elif esn.mode == _ESN_MODES[2]:
         #TO DO: for now semi-teacher is only possible for n_input = n_output
         assert len(index_list_auto) + len(index_list_teacher) == esn.n_input,'index_list_auto and index_list_teacher do not add up to n_input.'
-        y_pred_test, esn.x_test = esn.semiteacherforce(X = esn.x_train, testingLength = esn.testingLength, 
+        y_pred_test, esn.x_test = esn.semiteacherforce(X=X_pre_test, testingLength = esn.testingLength, 
                                                   index_list_auto = index_list_auto, index_list_teacher = index_list_teacher, 
                                                   u_test = esn.u_test)
     else:
         raise NotImplementedError('Error: unkown mode {0}. Choices {1}'.format(mode, _ESN_MODES))                                
  
     #-------------------------------------------------------------------------
-    #4. (optional) Validation Phase (for now only in auto & teacherforce mode)
+    # 4. (optional) Validation Phase (for now only in auto & teacher mode)
     #-------------------------------------------------------------------------
-    logger.debug('Validating ESN')
-    y_pred_val = None
     
+    y_pred_val = None
     if None not in [esn.u_val, esn.y_val]:
-        
+        logger.debug('Validating ESN')
+
         validationLength = esn.y_val.shape[0]
 
-        # initial state is build up from GT data (similar to testing phase)
+        # Initialize reservoir state by GT data
         if esn.u_pre_val is not None:
             X_pre_val = esn.propagate(u = esn.u_pre_val, transientTime = esn.u_pre_val.shape[0]-1,y=esn.y_pre_val)
-
-        # initial state taken from testing phase (no state initialization by GT data)
         else:
             X_pre_val = esn.x_test
 
             if esn.val_init_input is None:
                 if esn.mode == _ESN_MODES[0]:
                     esn.val_init_input = esn.y_test[-1,:].reshape(1,esn.n_input)
 
@@ -558,27 +578,26 @@
             raise NotImplementedError('Error: mode {0} not supported for validation. Choices {1}'.format(mode, _ESN_MODES[:2]))
 
     #-------------------------------------------------------------------------
     #5. Compute test & validation losses 
     #-------------------------------------------------------------------------
     if esn.loss_func is not None:
         for loss_label,loss_func in esn.loss_func.items():
-            loss_dict[loss_label+'_test'] = loss_func(y_true=esn.y_test,y_pred=y_pred_test)
+            loss_dict[loss_label+'_train'] = loss_func(y_true=esn.y_train[esn.transientTime:], y_pred=(esn.Wout@esn.x_train).T)
+            loss_dict[loss_label+'_test']  = loss_func(y_true=esn.y_test,y_pred=y_pred_test)
 
             if None not in [esn.u_val, esn.y_val]:
                 loss_dict[loss_label+'_val'] = loss_func(y_true=esn.y_val,y_pred=y_pred_val)
 
     return loss_dict, y_pred_test, y_pred_val
 
 #--------------------------------------------------------------------------
 #FH 30.03.2022: added forward_validate_auto_ESN 
 def forward_validate_auto_ESN(esn: ESN, cv: CrossValidation):
     ''' Runs ESN with k-fold forward walk validation scheme described in Lukosevicius et al. (2021)
-
-    
     
     INPUT:
         esn    - ESN class object. Contains the reservoir parameters. May contain training, testing and validation data sets.
         cv     - CrossValidation class object  containing cross validation parameters and data
         
     RETURN:
         loss_dict      - dictionary containing the losses specified in esn.loss_func
@@ -656,15 +675,15 @@
         y_pred_test_cv[ifold] = y_pred_test
         y_pred_val_cv[ifold]  = y_pred_val
         
     return loss_dict, y_pred_test_cv, y_pred_val_cv
 
 ###########################################################################################################
 
-#                            ERROR METRICS
+#                            Collection of error metrics
 
 ###########################################################################################################
 
 def compute_mse(y_true: torch.Tensor, 
                 y_pred: torch.Tensor, 
                 axis: Union[int,tuple] = 1) -> torch.Tensor:
     '''
@@ -739,74 +758,76 @@
         y_pred = torch.as_tensor(y_pred, dtype = _DTYPE)
             
     res = torch.sum((y_true - y_pred)**2,dim (0,1))
     mean = torch.mean(y_true, dim = 0)
     return 1 - res / torch.sum((y_pred - mean)**2, dim = (0,1))
 
 #--------------------------------------------------------------------------
-def compute_wasserstein_distance(y_true: torch.Tensor, y_pred: torch.Tensor,bins=40) -> torch.Tensor:
+def compute_wasserstein_distance(y_true: torch.Tensor, y_pred: torch.Tensor, bins:int = 40) -> torch.Tensor:
     '''
     Computes the Wasserstein distance between target data y_true and prediction data y_pred.
 
     INPUT:
         y_true - validation/testing/ true output
         y_pred - reseroir outputs
+        bins   - no. bins that PDF should have
 
     OUTPUT:
         Wasserstein distance w.r.t. both timestep- & mode-axis.
     '''
 
+
     logger.debug('Computing Wasserstein Distance')
 
-    hist_true, bins = torch.histogram(y_true.flatten(), bins=bins)
+    hist_true, bins = torch.histogram(y_true, bins=bins)
     hist_true /= hist_true.sum()
-    hist_pred,_ = torch.histogram(y_pred.flatten(), bins=bins, range=(float(bins[0]),float(bins[-1])))
-    hist_pred /= hist_pred.sum()
 
-    return wasserstein_distance(hist_pred, hist_true)
+    hist_pred, _ = torch.histogram(y_pred, bins=bins)
+    hist_pred /= hist_pred.sum()
+    
+    return wasserstein_distance(hist_pred+1e-8, hist_true+1e-8)
 
 #--------------------------------------------------------------------------
-def compute_kld(y_true: torch.Tensor, y_pred: torch.Tensor,bins=40) -> torch.Tensor:
+def compute_kld(y_true: torch.Tensor, y_pred: torch.Tensor, bins: int = 40) -> torch.Tensor:
     '''
-    Computes the Kullback-Leibler divergence between target data y_true and prediction data y_pred.
+    Computes the Kullback-Leibler divergence  between target data y_true and prediction data y_pred.
 
     INPUT:
         y_true - validation/testing/ true output
         y_pred - reseroir outputs
+        bins   - no. bins that PDF should have
 
     OUTPUT:
         KLD w.r.t. both timestep- & mode-axis.
     '''
 
-
     logger.debug('Computing Kullback-Leibler Divergence')
 
-    hist_true, bins = torch.histogram(y_true.flatten(), bins=bins)
+    hist_true, bins = torch.histogram(y_true, bins=bins)
     hist_true /= hist_true.sum()
-    hist_pred,_ = torch.histogram(y_pred.flatten(), bins=bins, range=(float(bins[0]),float(bins[-1])))
-    hist_pred /= hist_pred.sum()
-
-    return torch.mean(hist_true*(torch.log10((hist_true+1e-8)/(hist_pred+1e-8))))
 
+    hist_pred, _ = torch.histogram(y_pred, bins=bins)
+    hist_pred /= hist_pred.sum()
+    
+    return torch.mean(hist_true*torch.log((hist_true + 1e-8)/(hist_pred + 1e-8)))
 
 #--------------------------------------------------------------------------
-# FH 28.08.2022: added normalized prediction error according to Tanaka et al. Phys. Rev. Res. 4 (2022)
 def compute_normalized_prediction_error(y_true:torch.Tensor, 
                                         y_pred:torch.Tensor, 
                                         modal_mean:bool=True) -> torch.Tensor:
-    """
+    '''
     Computes the normalized prediction error (or its mean):
                   ||y_true-y_pred|| / <y_true**2>_t^(1/2)
     INPUT: 
         y_true     - validation/ testing/ true output
         y_pred     - reseroir outputs
         modal_mean - return modal mean of normalized prediction errror
     RETURN:
         normalized_prediction_error - modal mean of normalized prediction error
-    """
+    '''
     
 
     logger.debug('Computing NPE')
 
     testingLength,n_output = y_true.shape
     
     norm = (torch.mean(y_true**2+1e-6,dim=(0,)).reshape(1,n_output))**(1/2)
@@ -815,27 +836,99 @@
     if modal_mean:
         normalized_prediction_error = normalized_prediction_error.mean(dim=1)
     
     return normalized_prediction_error
     
 ###########################################################################################################
 
-#                            SAVING ESN STUDY
+#                            Saving an ESN study
 
 ###########################################################################################################
 
-def create_hdf5_groups(filepath: str, seeds: Union[int,list,range], nsetting: int):
+def get_file_name(yaml_filepath=None)->str:
+    '''
+    Returns suggested filename for grid/random search hdf5 file.
+
+    INPUT:
+        yaml_filepath - path to the yaml config file
+
+    RETURN:
+        filename - suggested filename for study
+    '''
+
+    try:
+        with open(yaml_filepath,'r') as f:
+            yaml_config = yaml.safe_load(f)
+    except FileNotFoundError:
+        logger.debug('Error: file {0} not found.'.format(yaml_filepath))
+        return None
+    
+    # read yaml file
+    data_str         = yaml_config.get('data_str','')
+    study_tuple      = yaml_config['study_tuple']
+    n_reservoir      = yaml_config['n_reservoir']
+    reservoirDensity = yaml_config['reservoirDensity']
+    regressionParameter = yaml_config['regressionParameter']
+    spectralRadius = yaml_config['spectralRadius']
+    leakingRate    = yaml_config['leakingRate']
+    dataScaling    = yaml_config['dataScaling']
+    esn_start      = yaml_config['esn_start']
+    trainingLength = yaml_config['trainingLength']
+    
+    # prepare strings
+    N_str = ''
+    D_str = ''
+    regParam_str = ''
+    SR_str = ''
+    LR_str = ''
+    
+    study_str = ''
+    for ii,param_str in enumerate(study_tuple):
+        study_str += param_str 
+        if ii < len(study_tuple)-1:
+            study_str += "_"
+
+    if 'n_reservoir' not in study_tuple:
+        N_str = f'N{n_reservoir}'
+    if 'reservoirDensity' not in study_tuple:
+        D_str = 'D{0:.1f}'.format(reservoirDensity).replace('.','')
+    if 'regressionParameter' not in study_tuple:
+        regParam_str = "regParam{0:.1e}".format(regressionParameter).replace('-','').replace('+','').replace('.','').replace('0','')
+    if 'spectralRadius' not in study_tuple:
+        SR_str = "SR{0:.2f}".format(spectralRadius).replace('.','')
+    if 'leakingRate' not in study_tuple:
+        LR_str = "LR{0:.2f}".format(leakingRate).replace('.','')
+
+    DS_str = f'DS{dataScaling}'
+    esn_start_str = f'esn_start{esn_start}'
+    TL_str = 'TL{0:.1e}'.format(trainingLength).replace('-','').replace('+','').replace('.','').replace('0','')
+
+    info = [data_str, study_str,N_str,D_str,SR_str,LR_str,regParam_str,DS_str,esn_start_str,TL_str]
+        
+    # construct filename
+    filename = ''
+    for s,string in enumerate(info):
+        if string == '':
+            continue
+
+        filename += string
+        
+        if s < len(info)-1:
+            filename += '_'
+
+    return filename + '.hdf5'
+
+#--------------------------------------------------------------------------
+def init_esn_file(filepath: str, seeds: Union[int,list,range], nsetting: int):
     '''Initializes the ESN study hdf5 file structure (shown below).  
 
     INPUT:
        filepath   - path to which the hdf5 file of the ESN study will be saved to
        nseed      - no. RNG seeds used in grid search
        nsetting   - no. ESN settings used in grid search
-       
-    FH added 15.03.2021
     '''
     #hdf5-Structure:
     #- seed1
     #   - setting1
     #       - study_dict
     #       - y_pred
     #       - mse
@@ -910,15 +1003,15 @@
         #   - ...
         #- ...
         
     to_close = False
     logger.info('Saving study to {0}'.format(filepath))
 
     if f is None:
-        assert os.path.isfile(filepath), "Error: The file {0} does not exist. Did you initialize the file with util.create_hdf5_groups ?".format(filepath)
+        assert os.path.isfile(filepath), "Error: The file {0} does not exist. Did you initialize the file with util.init_esn_file ?".format(filepath)
         f = h5py.File(filepath, 'a')
         to_close = True
 
     if 'Study' in f:
         G_study = f['Study']
     else:
         G_study = f.create_group('Study')
@@ -956,22 +1049,25 @@
     
     G_setting.create_dataset('y_pred_val', data = y_pred_val, compression = 'gzip', compression_opts = 9)
 
     for loss_label,loss_value in loss_dict.items():
         if loss_label in G_setting:
             del G_setting[loss_label]
         
-        G_setting.create_dataset(loss_label, data=loss_value, compression = 'gzip', compression_opts = 9)
+        if loss_value.flatten().shape[0] > 1:
+            G_setting.create_dataset(loss_label, data=loss_value, compression = 'gzip', compression_opts = 9)
+        else:
+            G_setting.create_dataset(loss_label, data=loss_value)
 
     if to_close:
         f.close()
 
 ###########################################################################################################
 
-#                            READING AN ESN STUDY
+#                            Reading an ESN study
 
 ###########################################################################################################
 #--------------------------------------------------------------------------
 # FH added 28.02.2021
 #--------------------------------------------------------------------------
 def create_study_config_list(study_tuple: Union[list,tuple], study_dicts: dict) -> np.ndarray:
     ''' Computes an array, which gives the parameter configuration/setting for the corresponding study.
@@ -1233,19 +1329,18 @@
     #----------------------------------  
     config = create_study_config_list(study_tuple, study_dicts)
 
     return np.array(y_pred_test), np.array(y_pred_val), config
     
 ###########################################################################################################
 
-#                            EXPERIMENTAL
+#                            Experimental methods
 
 ###########################################################################################################
 import matplotlib.pyplot as plt
-
 prop_cycle = plt.rcParams['axes.prop_cycle']
 clrs = prop_cycle.by_key()['color']
 
 def plot_activation_arg_distribution(esn,
                                     style_dict,
                                     bins_input: Union[int,torch.Tensor] = 40, 
                                     bins_res: Union[int,torch.Tensor] = 40, 
@@ -1328,52 +1423,35 @@
 #--------------------------------------------------------------------------
 def plot_esn_predictions(esn,y_pred,style_dict,modes=None,phase='test'):
     """
     Plots ESN prediction from specified phase. 
     INPUT:
         esn        - ESN object
         y_pred     - ESN prediction  
-        style_dict - dict specifying plot parameters
+        style_dict - dict specifying plot parameters (base_size1,base_size2 are mandatory)
         modes      - list specifying which modes of y_pred will be plotted
         phase      - str indicating for which phase the distributions should be computed: 'train', 'test', 'validation'
     
     RETURN:
         fig - figure 
         axs - axes
     """
     
     # Read Style 
     #-----------------
     base_size1,base_size2 = style_dict["base_size1"], style_dict["base_size2"]
-    ylim = style_dict["ylim"]
-
-    try:
-        fs_label = style_dict["fs_label"]
-    except KeyError:
-        fs_label = 15
-
-    try:
-        fs_tick = style_dict["fs_tick"]
-    except KeyError:
-        fs_tick = 12
-
-    try:
-        lw = style_dict["lw"]
-    except KeyError:
-        lw = 12
-
-    try:
-        ylabels = style_dict["ylabels"]
-    except KeyError:
-        ylabels = [r'$a_{'+f'{ii+1}'+ r'}$'for ii in modes]
+    ylim = style_dict.get("ylim",(-1,1))
 
+    fs_label = style_dict.get("fs_label",15)
+    fs_tick = style_dict.get("fs_tick",12)
+    lw = style_dict.get('linewidth',2)
+    ylabels = style_dict.get('ylabels',[r'$a_{'+f'{ii+1}'+ r'}$'for ii in modes])
     if modes is None:
         modes = range(esn.n_output)
         
-    
     if phase == 'train':
         y_gt = esn.y_train[self.transientTime:]
     elif phase == 'test':
         y_gt = esn.y_test
     elif phase == 'validation':
         y_gt = esn.y_val
```

### Comparing `turbESN-0.0.1.9.4.0/turbESN.egg-info/PKG-INFO` & `turbESN-0.0.1.9.5.0/turbESN.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turbESN
-Version: 0.0.1.9.4.0
+Version: 0.0.1.9.5.0
 Summary: An echo state network implementation.
 Home-page: UNKNOWN
 Author: flohey (Florian Heyder)
 Author-email: <florian.heyder@protonmail.com>
 License: UNKNOWN
 Keywords: python,ESN,reservoir computing,echo state network,recurrent neural network
 Platform: UNKNOWN
```

