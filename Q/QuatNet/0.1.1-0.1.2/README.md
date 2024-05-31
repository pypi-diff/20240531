# Comparing `tmp/QuatNet-0.1.1.tar.gz` & `tmp/quatnet-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QuatNet-0.1.1.tar", last modified: Tue May 21 14:45:39 2024, max compression
+gzip compressed data, was "quatnet-0.1.2.tar", last modified: Fri May 31 15:44:16 2024, max compression
```

## Comparing `QuatNet-0.1.1.tar` & `quatnet-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxrwxr-x   0 hiddenleaf  (1001) hiddenleaf  (1001)        0 2024-05-21 14:45:39.074418 QuatNet-0.1.1/
--rw-rw-r--   0 hiddenleaf  (1001) hiddenleaf  (1001)        0 2024-05-21 13:16:19.000000 QuatNet-0.1.1/LICENSE
--rw-r--r--   0 hiddenleaf  (1001) hiddenleaf  (1001)      563 2024-05-21 14:45:39.074418 QuatNet-0.1.1/PKG-INFO
-drwxrwxr-x   0 hiddenleaf  (1001) hiddenleaf  (1001)        0 2024-05-21 14:45:39.074418 QuatNet-0.1.1/QuatNet/
--rw-rw-r--   0 hiddenleaf  (1001) hiddenleaf  (1001)        0 2024-05-21 13:16:19.000000 QuatNet-0.1.1/QuatNet/__init__.py
--rw-rw-r--   0 hiddenleaf  (1001) hiddenleaf  (1001)    75739 2024-05-21 14:42:28.000000 QuatNet-0.1.1/QuatNet/quaternion_layers.py
--rw-rw-r--   0 hiddenleaf  (1001) hiddenleaf  (1001)    38998 2024-05-21 14:41:58.000000 QuatNet-0.1.1/QuatNet/quaternion_ops.py
-drwxrwxr-x   0 hiddenleaf  (1001) hiddenleaf  (1001)        0 2024-05-21 14:45:39.074418 QuatNet-0.1.1/QuatNet.egg-info/
--rw-r--r--   0 hiddenleaf  (1001) hiddenleaf  (1001)      563 2024-05-21 14:45:39.000000 QuatNet-0.1.1/QuatNet.egg-info/PKG-INFO
--rw-rw-r--   0 hiddenleaf  (1001) hiddenleaf  (1001)      273 2024-05-21 14:45:39.000000 QuatNet-0.1.1/QuatNet.egg-info/SOURCES.txt
--rw-rw-r--   0 hiddenleaf  (1001) hiddenleaf  (1001)        1 2024-05-21 14:45:39.000000 QuatNet-0.1.1/QuatNet.egg-info/dependency_links.txt
--rw-rw-r--   0 hiddenleaf  (1001) hiddenleaf  (1001)       19 2024-05-21 14:45:39.000000 QuatNet-0.1.1/QuatNet.egg-info/requires.txt
--rw-rw-r--   0 hiddenleaf  (1001) hiddenleaf  (1001)       14 2024-05-21 14:45:39.000000 QuatNet-0.1.1/QuatNet.egg-info/top_level.txt
--rw-rw-r--   0 hiddenleaf  (1001) hiddenleaf  (1001)       59 2024-05-21 13:15:22.000000 QuatNet-0.1.1/README.md
--rw-rw-r--   0 hiddenleaf  (1001) hiddenleaf  (1001)       38 2024-05-21 14:45:39.074418 QuatNet-0.1.1/setup.cfg
--rw-rw-r--   0 hiddenleaf  (1001) hiddenleaf  (1001)      695 2024-05-21 14:45:33.000000 QuatNet-0.1.1/setup.py
-drwxrwxr-x   0 hiddenleaf  (1001) hiddenleaf  (1001)        0 2024-05-21 14:45:39.074418 QuatNet-0.1.1/tests/
--rw-rw-r--   0 hiddenleaf  (1001) hiddenleaf  (1001)        0 2024-05-21 13:16:19.000000 QuatNet-0.1.1/tests/__init__.py
+drwxrwxr-x   0 hiddenleaf  (1001) hiddenleaf  (1001)        0 2024-05-31 15:44:16.121911 quatnet-0.1.2/
+-rw-rw-r--   0 hiddenleaf  (1001) hiddenleaf  (1001)        0 2024-05-21 13:16:19.000000 quatnet-0.1.2/LICENSE
+-rw-r--r--   0 hiddenleaf  (1001) hiddenleaf  (1001)      755 2024-05-31 15:44:16.121911 quatnet-0.1.2/PKG-INFO
+drwxrwxr-x   0 hiddenleaf  (1001) hiddenleaf  (1001)        0 2024-05-31 15:44:16.121911 quatnet-0.1.2/QuatNet/
+-rw-rw-r--   0 hiddenleaf  (1001) hiddenleaf  (1001)        0 2024-05-21 13:16:19.000000 quatnet-0.1.2/QuatNet/__init__.py
+-rw-rw-r--   0 hiddenleaf  (1001) hiddenleaf  (1001)    75803 2024-05-31 15:28:20.000000 quatnet-0.1.2/QuatNet/quaternion_layers.py
+-rw-rw-r--   0 hiddenleaf  (1001) hiddenleaf  (1001)    39056 2024-05-31 15:28:12.000000 quatnet-0.1.2/QuatNet/quaternion_ops.py
+drwxrwxr-x   0 hiddenleaf  (1001) hiddenleaf  (1001)        0 2024-05-31 15:44:16.121911 quatnet-0.1.2/QuatNet.egg-info/
+-rw-r--r--   0 hiddenleaf  (1001) hiddenleaf  (1001)      755 2024-05-31 15:44:16.000000 quatnet-0.1.2/QuatNet.egg-info/PKG-INFO
+-rw-rw-r--   0 hiddenleaf  (1001) hiddenleaf  (1001)      263 2024-05-31 15:44:16.000000 quatnet-0.1.2/QuatNet.egg-info/SOURCES.txt
+-rw-rw-r--   0 hiddenleaf  (1001) hiddenleaf  (1001)        1 2024-05-31 15:44:16.000000 quatnet-0.1.2/QuatNet.egg-info/dependency_links.txt
+-rw-rw-r--   0 hiddenleaf  (1001) hiddenleaf  (1001)       41 2024-05-31 15:44:16.000000 quatnet-0.1.2/QuatNet.egg-info/requires.txt
+-rw-rw-r--   0 hiddenleaf  (1001) hiddenleaf  (1001)       14 2024-05-31 15:44:16.000000 quatnet-0.1.2/QuatNet.egg-info/top_level.txt
+-rw-rw-r--   0 hiddenleaf  (1001) hiddenleaf  (1001)       38 2024-05-31 15:44:16.121911 quatnet-0.1.2/setup.cfg
+-rw-rw-r--   0 hiddenleaf  (1001) hiddenleaf  (1001)      741 2024-05-31 15:41:26.000000 quatnet-0.1.2/setup.py
+drwxrwxr-x   0 hiddenleaf  (1001) hiddenleaf  (1001)        0 2024-05-31 15:44:16.121911 quatnet-0.1.2/tests/
+-rw-rw-r--   0 hiddenleaf  (1001) hiddenleaf  (1001)        0 2024-05-21 13:16:19.000000 quatnet-0.1.2/tests/__init__.py
```

### Comparing `QuatNet-0.1.1/PKG-INFO` & `quatnet-0.1.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,25 @@
 Metadata-Version: 2.1
 Name: QuatNet
-Version: 0.1.1
+Version: 0.1.2
 Summary: A PyTorch-based library for quaternion neural networks
 Home-page: https://github.com/DataSenseiAryan/QuatNet
-Author: aryan
+Author: aryan chaudhary
 Author-email: datasenseiaryan@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: ==3.8.19
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: torch>=2.0.0
-Requires-Dist: numpy
+Requires-Dist: torch==2.3.0
+Requires-Dist: numpy==1.24.4
+Requires-Dist: scipy==1.10.1
 
-# QuatNet
-A PyTorch library for Quaternion Neural Networks
+# Quaternion Neural Network Library
+https://pypi.org/project/QuatNet/0.1.0/
+A PyTorch-based library for building neural networks using quaternion numbers.
+
+## Installation
+
+```bash
+pip install quatnet
```

### Comparing `QuatNet-0.1.1/QuatNet/quaternion_layers.py` & `quatnet-0.1.2/QuatNet/quaternion_layers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 ##########################################################
 # pytorch-qnn v1.0
 # Titouan Parcollet
 # LIA, Université d'Avignon et des Pays du Vaucluse
 # ORKIS, Aix-en-provence
 # October 2018
+
+#Aryan Chaudhary, IIIT Delhi, added more functionalities 2023 
 ##########################################################
 
 import numpy  as np
 from   numpy.random import RandomState
 import torch
 from torch.nn.functional import normalize
 from   torch.autograd import Variable
```

### Comparing `QuatNet-0.1.1/QuatNet/quaternion_ops.py` & `quatnet-0.1.2/QuatNet/quaternion_ops.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 ##########################################################
 # pytorch-qnn v1.0
 # Titouan Parcollet
 # LIA, Université d'Avignon et des Pays du Vaucluse
 # ORKIS, Aix-en-provence
 # October 2018
+
+#Aryan Chaudhary IIIT Delhi, added more functionalities, 2023
 ##########################################################
 
 import torch
 import torch.nn as nn
 from torch.autograd import Variable
 import torch.nn.functional as F
 import numpy as np
 from numpy.random import RandomState
 import sys
 # import pdb
-# from scipy.stats import chi
+from scipy.stats import chi
 # import torchaudio
 
 def q_normalize(input, channel=1):
 
     r = get_r(input)
     i = get_i(input)
     j = get_j(input)
@@ -881,15 +883,15 @@
                  + str(r_weight.size()) +' i:'
                  + str(i_weight.size()) +' j:'
                  + str(j_weight.size()) +' k:'
                  + str(k_weight.size()))
 
     elif 2 >= r_weight.dim():
         raise Exception('affect_conv_init accepts only tensors that have more than 2 dimensions. Found dimension = '
-                        + str(real_weight.dim()))
+                        + str(r_weight.dim()))
 
     r, i, j, k = init_func(
         r_weight.size(1),
         r_weight.size(0),
         rng=rng,
         kernel_size=kernel_size,
         criterion=init_criterion
```

### Comparing `QuatNet-0.1.1/QuatNet.egg-info/PKG-INFO` & `quatnet-0.1.2/QuatNet.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,25 @@
 Metadata-Version: 2.1
 Name: QuatNet
-Version: 0.1.1
+Version: 0.1.2
 Summary: A PyTorch-based library for quaternion neural networks
 Home-page: https://github.com/DataSenseiAryan/QuatNet
-Author: aryan
+Author: aryan chaudhary
 Author-email: datasenseiaryan@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: ==3.8.19
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: torch>=2.0.0
-Requires-Dist: numpy
+Requires-Dist: torch==2.3.0
+Requires-Dist: numpy==1.24.4
+Requires-Dist: scipy==1.10.1
 
-# QuatNet
-A PyTorch library for Quaternion Neural Networks
+# Quaternion Neural Network Library
+https://pypi.org/project/QuatNet/0.1.0/
+A PyTorch-based library for building neural networks using quaternion numbers.
+
+## Installation
+
+```bash
+pip install quatnet
```

### Comparing `QuatNet-0.1.1/setup.py` & `quatnet-0.1.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 # setup.py
 from setuptools import setup, find_packages
 
 setup(
     name='QuatNet',
-    version='0.1.1',
+    version='0.1.2',
     packages=find_packages(),
     install_requires=[
-        'torch>=2.0.0',
-        'numpy'
+        'torch==2.3.0',
+        'numpy==1.24.4',
+        'scipy==1.10.1'
     ],
-    author='aryan',
+    author='aryan chaudhary',
     author_email='datasenseiaryan@gmail.com',
     description='A PyTorch-based library for quaternion neural networks',
-    long_description=open('README.md').read(),
+    long_description=open('README.MD').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/DataSenseiAryan/QuatNet',
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
-    python_requires='>=3.6',
+    python_requires='==3.8.19',
 )
```

