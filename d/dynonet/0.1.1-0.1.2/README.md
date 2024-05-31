# Comparing `tmp/dynonet-0.1.1.tar.gz` & `tmp/dynonet-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynonet-0.1.1.tar", last modified: Fri Jul 16 13:53:45 2021, max compression
+gzip compressed data, was "dynonet-0.1.2.tar", last modified: Fri May 31 20:53:34 2024, max compression
```

## Comparing `dynonet-0.1.1.tar` & `dynonet-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2021-07-16 13:53:45.563007 dynonet-0.1.1/
--rw-rw-r--   0 marco     (1000) marco     (1000)     1071 2020-05-30 12:14:57.000000 dynonet-0.1.1/LICENSE
--rw-rw-r--   0 marco     (1000) marco     (1000)     4465 2021-07-16 13:53:45.563007 dynonet-0.1.1/PKG-INFO
--rw-rw-r--   0 marco     (1000) marco     (1000)     3637 2021-07-16 13:49:22.000000 dynonet-0.1.1/README.md
--rw-rw-r--   0 marco     (1000) marco     (1000)     1053 2021-07-16 13:53:45.563007 dynonet-0.1.1/setup.cfg
--rw-rw-r--   0 marco     (1000) marco     (1000)       38 2021-06-14 08:06:50.000000 dynonet-0.1.1/setup.py
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2021-07-16 13:53:45.559007 dynonet-0.1.1/src/
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2021-07-16 13:53:45.563007 dynonet-0.1.1/src/dynonet/
--rw-rw-r--   0 marco     (1000) marco     (1000)        0 2021-06-14 08:06:50.000000 dynonet-0.1.1/src/dynonet/__init__.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     5474 2021-06-14 08:06:50.000000 dynonet-0.1.1/src/dynonet/filtering.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     7822 2021-06-14 08:06:50.000000 dynonet-0.1.1/src/dynonet/functional.py
--rw-rw-r--   0 marco     (1000) marco     (1000)    14750 2021-06-14 08:06:50.000000 dynonet-0.1.1/src/dynonet/lti.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     4028 2021-06-14 08:06:50.000000 dynonet-0.1.1/src/dynonet/metrics.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     4051 2021-06-14 08:06:50.000000 dynonet-0.1.1/src/dynonet/static.py
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2021-07-16 13:53:45.563007 dynonet-0.1.1/src/dynonet.egg-info/
--rw-rw-r--   0 marco     (1000) marco     (1000)     4465 2021-07-16 13:53:45.000000 dynonet-0.1.1/src/dynonet.egg-info/PKG-INFO
--rw-rw-r--   0 marco     (1000) marco     (1000)      383 2021-07-16 13:53:45.000000 dynonet-0.1.1/src/dynonet.egg-info/SOURCES.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)        1 2021-07-16 13:53:45.000000 dynonet-0.1.1/src/dynonet.egg-info/dependency_links.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)        1 2021-07-16 13:53:45.000000 dynonet-0.1.1/src/dynonet.egg-info/not-zip-safe
--rw-rw-r--   0 marco     (1000) marco     (1000)       70 2021-07-16 13:53:45.000000 dynonet-0.1.1/src/dynonet.egg-info/requires.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)        8 2021-07-16 13:53:45.000000 dynonet-0.1.1/src/dynonet.egg-info/top_level.txt
+drwxr-xr-x   0 marco.forgione   (502) staff       (20)        0 2024-05-31 20:53:34.251262 dynonet-0.1.2/
+-rw-r--r--   0 marco.forgione   (502) staff       (20)     1071 2024-05-31 20:44:55.000000 dynonet-0.1.2/LICENSE
+-rw-r--r--   0 marco.forgione   (502) staff       (20)     4590 2024-05-31 20:53:34.250805 dynonet-0.1.2/PKG-INFO
+-rw-r--r--   0 marco.forgione   (502) staff       (20)     3637 2024-05-31 20:44:55.000000 dynonet-0.1.2/README.md
+-rw-r--r--   0 marco.forgione   (502) staff       (20)     1053 2024-05-31 20:53:34.252426 dynonet-0.1.2/setup.cfg
+-rw-r--r--   0 marco.forgione   (502) staff       (20)       38 2024-05-31 20:44:55.000000 dynonet-0.1.2/setup.py
+drwxr-xr-x   0 marco.forgione   (502) staff       (20)        0 2024-05-31 20:53:34.233853 dynonet-0.1.2/src/
+drwxr-xr-x   0 marco.forgione   (502) staff       (20)        0 2024-05-31 20:53:34.240936 dynonet-0.1.2/src/dynonet/
+-rw-r--r--   0 marco.forgione   (502) staff       (20)        0 2024-05-31 20:44:55.000000 dynonet-0.1.2/src/dynonet/__init__.py
+-rw-r--r--   0 marco.forgione   (502) staff       (20)     5474 2024-05-31 20:44:55.000000 dynonet-0.1.2/src/dynonet/filtering.py
+-rw-r--r--   0 marco.forgione   (502) staff       (20)     7822 2024-05-31 20:44:55.000000 dynonet-0.1.2/src/dynonet/functional.py
+-rw-r--r--   0 marco.forgione   (502) staff       (20)    17084 2024-05-31 20:50:20.000000 dynonet-0.1.2/src/dynonet/lti.py
+-rw-r--r--   0 marco.forgione   (502) staff       (20)     4028 2024-05-31 20:44:55.000000 dynonet-0.1.2/src/dynonet/metrics.py
+-rw-r--r--   0 marco.forgione   (502) staff       (20)     4051 2024-05-31 20:44:55.000000 dynonet-0.1.2/src/dynonet/static.py
+drwxr-xr-x   0 marco.forgione   (502) staff       (20)        0 2024-05-31 20:53:34.250283 dynonet-0.1.2/src/dynonet.egg-info/
+-rw-r--r--   0 marco.forgione   (502) staff       (20)     4590 2024-05-31 20:53:34.000000 dynonet-0.1.2/src/dynonet.egg-info/PKG-INFO
+-rw-r--r--   0 marco.forgione   (502) staff       (20)      383 2024-05-31 20:53:34.000000 dynonet-0.1.2/src/dynonet.egg-info/SOURCES.txt
+-rw-r--r--   0 marco.forgione   (502) staff       (20)        1 2024-05-31 20:53:34.000000 dynonet-0.1.2/src/dynonet.egg-info/dependency_links.txt
+-rw-r--r--   0 marco.forgione   (502) staff       (20)        1 2024-05-31 20:53:34.000000 dynonet-0.1.2/src/dynonet.egg-info/not-zip-safe
+-rw-r--r--   0 marco.forgione   (502) staff       (20)       70 2024-05-31 20:53:34.000000 dynonet-0.1.2/src/dynonet.egg-info/requires.txt
+-rw-r--r--   0 marco.forgione   (502) staff       (20)        8 2024-05-31 20:53:34.000000 dynonet-0.1.2/src/dynonet.egg-info/top_level.txt
```

### Comparing `dynonet-0.1.1/LICENSE` & `dynonet-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dynonet-0.1.1/PKG-INFO` & `dynonet-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 Metadata-Version: 2.1
 Name: dynonet
-Version: 0.1.1
+Version: 0.1.2
 Summary: dynoNet: A neural network architecture for learning dynamical systems
 Home-page: https://github.com/forgi86/dynonet
 Author: Marco Forgione and Dario Piga
 Author-email: marco.forgione1986@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/forgi86/dynonet/issues
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy>=1.19.4
+Requires-Dist: scipy>=1.5.4
+Requires-Dist: matplotlib>=3.3.3
+Requires-Dist: pandas>=1.1.4
+Requires-Dist: torch>=1.4
 
 # dynoNet: A neural network architecture for learning dynamical systems 
 
 This repository contains the Python code to reproduce the results of the paper [dynoNet: A neural network architecture for learning dynamical systems](https://arxiv.org/pdf/2006.02250.pdf) by Marco Forgione and Dario Piga.
 
 In this work, we introduce the linear dynamical operator as a differentiable layer compatible with back-propagation-based training. 
 The operator is parametrized as a rational transfer function and thus can represent an infinite impulse response (IIR)
@@ -105,9 +109,7 @@
   volume={35},
   number={4},
   pages={612--626},
   year={2021},
   publisher={Wiley}
 }
 ```
-
-
```

### Comparing `dynonet-0.1.1/README.md` & `dynonet-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `dynonet-0.1.1/setup.cfg` & `dynonet-0.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [wheel]
 universal = 1
 
 [metadata]
 name = dynonet
-version = 0.1.1
+version = 0.1.2
 author = Marco Forgione and Dario Piga
 author_email = marco.forgione1986@gmail.com
 description = dynoNet: A neural network architecture for learning dynamical systems
 long_description = file: README.md
 long_description_content_type = text/markdown
 license_file = LICENSE
 license = MIT
```

### Comparing `dynonet-0.1.1/src/dynonet/filtering.py` & `dynonet-0.1.2/src/dynonet/filtering.py`

 * *Files identical despite different names*

### Comparing `dynonet-0.1.1/src/dynonet/functional.py` & `dynonet-0.1.2/src/dynonet/functional.py`

 * *Files identical despite different names*

### Comparing `dynonet-0.1.1/src/dynonet/lti.py` & `dynonet-0.1.2/src/dynonet/lti.py`

 * *Files 4% similar despite different names*

```diff
@@ -322,34 +322,90 @@
         >>> u_in = torch.ones((batch_size, seq_len, in_channels))
         >>> y_out = G(u_in, y_0, u_0) # shape: (batch_size, seq_len, 1)
 
     """
 
     def __init__(self, in_channels, out_channels):
         super(StableSecondOrderMimoLinearDynamicalOperator, self).__init__()
-        self.b_coeff = Parameter(torch.zeros(out_channels, in_channels, 2))
+        self.b_coeff = Parameter(torch.zeros(out_channels, in_channels, 3))
         self.rho = Parameter(torch.zeros(out_channels, in_channels, 1))
         self.psi = Parameter(torch.zeros((out_channels, in_channels, 1)))
+        self.out_channels = out_channels
+        self.in_channels = in_channels
+        self.n_b = 3
+        self.n_a = 2
+        self.n_k = 0
         with torch.no_grad():
             self.rho[:] = torch.randn(self.rho.shape) * 0.1
             self.psi[:] = torch.randn(self.rho.shape) * 0.1
             self.b_coeff[:] = torch.randn(self.b_coeff.shape) * 0.01
 
     def forward(self, u_in, y_0=None, u_0=None):
         r = torch.sigmoid(self.rho)
         beta = np.pi * torch.sigmoid(self.psi)
         a_1 = -2 * r * torch.cos(beta)
         a_2 = r ** 2
         a_coeff = torch.cat((a_1, a_2), dim=-1)
+        # print (r)
         return MimoLinearDynamicalOperatorFun.apply(self.b_coeff, a_coeff, u_in, y_0, u_0)
 
 
 class StableSecondOrderSisoLinearDynamicalOperator(StableSecondOrderMimoLinearDynamicalOperator):
     r"""Applies a stable second-order linear single-input-single-output filtering operation.
     The denominator of the transfer function is parametrized in terms of two complex conjugate poles with magnitude
     :math:: `r, 0 < r < 1` and phase :math:: `\beta, < 0 \beta < \pi`. In turn, :math:: `r` and :math:: `\beta` are
     parametrized in terms of unconstrained variables :math:: `\rho` and :math:: `\psi`
 
     """
 
     def __init__(self):
         super(StableSecondOrderSisoLinearDynamicalOperator, self).__init__(1, 1)  # in_channels, out_channels, n_b, n_a
+
+#########################################################
+
+class StableSecondOrderMimoLinearDynamicalOperatorX(torch.nn.Module):
+    r"""Like StableSecondOrderSisoLinearDynamicalOperator, using equation (32), which allows 2 distinct real poles.
+    The denominator of the transfer function is parametrized in terms of two poles (distinct reals or complex
+    conjugates) defined by unconstrained variables :math:: `\alpha_1` and :math:: `\alpha_2`
+
+    Args:
+        in_channels (int): Number of input channels
+        out_channels (int): Number of output channels
+
+    Shape:
+        - Input: (batch_size, seq_len, 1)
+        - Output: (batch_size, seq_len, 1)
+
+    Attributes:
+        alpha1 (Tensor): the learnable :math:: `\alpha_1` coefficients of the transfer function denominator
+        alpha2 (Tensor): the learnable :math:: `\alpha_2` coefficients of the transfer function denominator
+        b_coeff (Tensor): the learnable numerator coefficients
+
+    Examples::
+
+        >>> G = StableSecondOrderMimoLinearDynamicalOperator(in_channels=2, out_channels=4)
+    """
+
+    def __init__(self, in_channels, out_channels):
+        super(StableSecondOrderMimoLinearDynamicalOperatorX, self).__init__()
+        self.b_coeff = Parameter(torch.zeros(out_channels, in_channels, 3))
+        self.alpha1 = Parameter(torch.zeros(out_channels, in_channels, 1))
+        self.alpha2 = Parameter(torch.zeros((out_channels, in_channels, 1)))
+        self.out_channels = out_channels
+        self.in_channels = in_channels
+        self.n_b = 3
+        self.n_a = 2
+        self.n_k = 0
+        with torch.no_grad():
+            self.alpha1[:] = torch.randn(self.alpha1.shape) * 0.1
+            self.alpha2[:] = torch.randn(self.alpha2.shape) * 0.1
+            self.b_coeff[:] = torch.randn(self.b_coeff.shape) * 0.01
+
+    def forward(self, u_in, y_0=None, u_0=None):
+        a_1 = 2.0 * torch.tanh(self.alpha1)
+        a_1_abs = torch.abs(a_1)
+        a_2 = a_1_abs + (2.0 - a_1_abs) * torch.sigmoid(self.alpha2) - 1.0
+        a_coeff = torch.cat((a_1, a_2), dim=-1)
+        # print (r)
+        return MimoLinearDynamicalOperatorFun.apply(self.b_coeff, a_coeff, u_in, y_0, u_0)
+
+
```

### Comparing `dynonet-0.1.1/src/dynonet/metrics.py` & `dynonet-0.1.2/src/dynonet/metrics.py`

 * *Files identical despite different names*

### Comparing `dynonet-0.1.1/src/dynonet/static.py` & `dynonet-0.1.2/src/dynonet/static.py`

 * *Files identical despite different names*

### Comparing `dynonet-0.1.1/src/dynonet.egg-info/PKG-INFO` & `dynonet-0.1.2/src/dynonet.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 Metadata-Version: 2.1
 Name: dynonet
-Version: 0.1.1
+Version: 0.1.2
 Summary: dynoNet: A neural network architecture for learning dynamical systems
 Home-page: https://github.com/forgi86/dynonet
 Author: Marco Forgione and Dario Piga
 Author-email: marco.forgione1986@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/forgi86/dynonet/issues
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy>=1.19.4
+Requires-Dist: scipy>=1.5.4
+Requires-Dist: matplotlib>=3.3.3
+Requires-Dist: pandas>=1.1.4
+Requires-Dist: torch>=1.4
 
 # dynoNet: A neural network architecture for learning dynamical systems 
 
 This repository contains the Python code to reproduce the results of the paper [dynoNet: A neural network architecture for learning dynamical systems](https://arxiv.org/pdf/2006.02250.pdf) by Marco Forgione and Dario Piga.
 
 In this work, we introduce the linear dynamical operator as a differentiable layer compatible with back-propagation-based training. 
 The operator is parametrized as a rational transfer function and thus can represent an infinite impulse response (IIR)
@@ -105,9 +109,7 @@
   volume={35},
   number={4},
   pages={612--626},
   year={2021},
   publisher={Wiley}
 }
 ```
-
-
```

