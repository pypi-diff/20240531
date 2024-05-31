# Comparing `tmp/pyerualjetwork-1.3.6.tar.gz` & `tmp/pyerualjetwork-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyerualjetwork-1.3.6.tar", last modified: Thu May 30 02:18:14 2024, max compression
+gzip compressed data, was "pyerualjetwork-1.3.7.tar", last modified: Thu May 30 23:25:29 2024, max compression
```

## Comparing `pyerualjetwork-1.3.6.tar` & `pyerualjetwork-1.3.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 02:18:14.918068 pyerualjetwork-1.3.6/
--rw-rw-rw-   0        0        0      502 2024-05-30 02:18:14.910553 pyerualjetwork-1.3.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-30 02:18:14.879936 pyerualjetwork-1.3.6/plan/
--rw-rw-rw-   0        0        0      375 2024-05-29 18:09:13.000000 pyerualjetwork-1.3.6/plan/__init__.py
--rw-rw-rw-   0        0        0    44211 2024-05-30 02:10:10.000000 pyerualjetwork-1.3.6/plan/plan.py
-drwxrwxrwx   0        0        0        0 2024-05-30 02:18:14.910553 pyerualjetwork-1.3.6/pyerualjetwork.egg-info/
--rw-rw-rw-   0        0        0      502 2024-05-30 02:18:14.000000 pyerualjetwork-1.3.6/pyerualjetwork.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2024-05-30 02:18:14.000000 pyerualjetwork-1.3.6/pyerualjetwork.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 02:18:14.000000 pyerualjetwork-1.3.6/pyerualjetwork.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-30 02:18:14.000000 pyerualjetwork-1.3.6/pyerualjetwork.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-30 02:18:14.918068 pyerualjetwork-1.3.6/setup.cfg
--rw-rw-rw-   0        0        0      681 2024-05-30 02:10:15.000000 pyerualjetwork-1.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 23:25:29.161381 pyerualjetwork-1.3.7/
+-rw-rw-rw-   0        0        0      391 2024-05-30 23:25:29.160379 pyerualjetwork-1.3.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-30 23:25:29.110507 pyerualjetwork-1.3.7/plan/
+-rw-rw-rw-   0        0        0      375 2024-05-29 18:09:13.000000 pyerualjetwork-1.3.7/plan/__init__.py
+-rw-rw-rw-   0        0        0    44862 2024-05-30 23:23:36.000000 pyerualjetwork-1.3.7/plan/plan.py
+drwxrwxrwx   0        0        0        0 2024-05-30 23:25:29.157448 pyerualjetwork-1.3.7/pyerualjetwork.egg-info/
+-rw-rw-rw-   0        0        0      391 2024-05-30 23:25:28.000000 pyerualjetwork-1.3.7/pyerualjetwork.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2024-05-30 23:25:28.000000 pyerualjetwork-1.3.7/pyerualjetwork.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 23:25:28.000000 pyerualjetwork-1.3.7/pyerualjetwork.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-30 23:25:28.000000 pyerualjetwork-1.3.7/pyerualjetwork.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-30 23:25:29.162379 pyerualjetwork-1.3.7/setup.cfg
+-rw-rw-rw-   0        0        0      570 2024-05-30 23:24:45.000000 pyerualjetwork-1.3.7/setup.py
```

### Comparing `pyerualjetwork-1.3.6/plan/plan.py` & `pyerualjetwork-1.3.7/plan/plan.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+"""
+Created on Thu May 30 22:12:49 2024
+
+@author: hasan can beydili
+"""
 import numpy as np
 import time
 from colorama import Fore,Style
 from typing import List, Union
 import math
 from scipy.special import expit, softmax
 import matplotlib.pyplot as plt
@@ -144,15 +149,15 @@
         return 'e'
     
     x_train[0] = np.array(x_train[0])
     x_train[0] = x_train[0].ravel()
     x_train_size = len(x_train[0])
     
     W = WeightIdentification(len(layers) - 1,class_count,neurons,x_train_size)
-    Divides = SynapticDividing(class_count,W)
+    Divides, Piece = SynapticDividing(class_count,W)
     trained_W = [1] * len(W)
     print(Fore.GREEN + "Train Started with 0 ERROR" + Style.RESET_ALL,)
     train_predictions = [None] * len(y_train)
     true = 0
     start_time = time.time()
     for index, inp in enumerate(x_train):
         uni_start_time = time.time()
@@ -167,17 +172,19 @@
         for Ulindex, Ul in enumerate(Uniquey_train):
             
             if Ul == y_train[index]:
                 for Windex, w in enumerate(W):
                     for i, ul in enumerate(Ul):
                         if ul == 1.0:
                             k = i
+
                     cs = Divides[int(k)][Windex][0]
+
        
-                    W[Windex] = SynapticPruning(w, cs, 'row', int(k),class_count)
+                    W[Windex] = SynapticPruning(w, cs, 'row', int(k),class_count,Piece[Windex],1)
 
         neural_layer = inp
         
         for Lindex, Layer in enumerate(layers):
             
             if normalizations[Lindex] == 'y':
                 neural_layer = Normalization(neural_layer)
@@ -186,17 +193,17 @@
                 neural_layer = Relu(neural_layer)
             elif activations[Lindex] == 'sigmoid':
                 neural_layer = Sigmoid(neural_layer)
             elif activations[Lindex] == 'softmax':
                 neural_layer = Softmax(neural_layer)
                 
             if Layer == 'fex':
-                neural_layer,W[Lindex] = Fex(neural_layer, W[Lindex], membran_thresholds[Lindex], membran_potentials[Lindex])
+                neural_layer,W[Lindex] = Fex(neural_layer, W[Lindex], membran_thresholds[Lindex], membran_potentials[Lindex], Piece[Windex],1)
             elif Layer == 'cat':
-                neural_layer,W[Lindex] = Cat(neural_layer, W[Lindex], membran_thresholds[Lindex], membran_potentials[Lindex],1)
+                neural_layer,W[Lindex] = Cat(neural_layer, W[Lindex], membran_thresholds[Lindex], membran_potentials[Lindex],1, Piece[Windex])
                 
         RealOutput = np.argmax(y_train[index])
         PredictedOutput = np.argmax(neural_layer)
         if RealOutput == PredictedOutput:
             true += 1
         acc = true / len(y_train)
         train_predictions[index] = PredictedOutput
@@ -308,15 +315,17 @@
     return W
 
 def SynapticPruning(
     w,            # list[list[num]]: Weight matrix of the neural network.
     cs,           # list[list[num]]: Synaptic connections between neurons.
     key,          # int: key for identifying synaptic connections.
     Class,        # int: Class label for the current training instance.
-    class_count   # int: Total number of classes in the dataset.
+    class_count, # int: Total number of classes in the dataset.
+    piece, # ???
+    is_training # int: 1 or 0
     
 ) -> str:
     infoPruning = """
     Performs synaptic pruning in a neural network model.
 
     Args:
         w (list[list[num]]): Weight matrix of the neural network.
@@ -324,26 +333,39 @@
         key (str): key for identifying synaptic row or col connections.
         Class (int): Class label for the current training instance.
         class_count (int): Total number of classes in the dataset.
 
     Returns:
         numpy array: Weight matrix.
     """
-
+    
     
     Class += 1 # because index start 0
     
-    if Class != class_count and Class != 1:
-            
-            ce = cs / Class
+    if  Class != 1:
+        
      
-            w[int(ce)-1::-1,:] = 0
-          
-            w[cs:,:] = 0
-    
+               
+        ce = cs / Class
+        
+        if is_training == 1:
+        
+            p = piece
+                
+            for i in range(Class - 3):
+                    
+                piece+=p
+                    
+            if Class!= 2:
+                 ce += piece
+            
+        w[int(ce)-1::-1,:] = 0
+        
+            
+        w[cs:,:] = 0
 
     else:
         
         if Class == 1:
             if key == 'row':
     
                 w[cs:,:] = 0
@@ -390,40 +412,44 @@
     
     Piece = [1] * len(W)
     #print('Piece:' + Piece)
     #input()
     # Boş bir üç boyutlu liste oluşturma
     Divides = [[[0] for _ in range(len(W))] for _ in range(class_count)]
     
+    
     for i in range(len(W)):
             
 
             Piece[i] = int(math.floor(W[i].shape[0] / class_count))
 
-    cs = 0
+    cs = 0 
     # j = Classes, i = Weights, [0] = CutStart.
 
     for i in range(len(W)):
         for j in range(class_count):
             cs = cs + Piece[i]
             Divides[j][i][0] = cs
+        #pruning_param[i] = cs
             #print('Divides: ' + j + i + ' = ' + Divides[j][i][0])
             #input()
-        
+            
         j = 0
         cs = 0
         
-    return Divides
+    return Divides, Piece
         
 
 def Fex(
     Input,               # list[num]: Input data.
     w,                   # list[list[num]]: Weight matrix of the neural network.
     membran_threshold,      # str: Sign for threshold comparison ('<', '>', '==', '!=').
-    membran_potential       # num: Threshold value for comparison.
+    membran_potential, # num: Threshold value for comparison.
+    piece, # ???
+    is_training # num: 1 or 0
 ) -> tuple:
     """
     Applies feature extraction process to the input data using synaptic pruning.
 
     Args:
         Input (list[num]): Input data.
         w (list[list[num]]): Weight matrix of the neural network.
@@ -439,25 +465,26 @@
     elif membran_threshold == '>': 
         PruneIndex = np.where(Input > membran_potential)
     elif membran_threshold == '==':
         PruneIndex = np.where(Input == membran_potential)
     elif membran_threshold == '!=':
         PruneIndex = np.where(Input != membran_potential)
 
-    w = SynapticPruning(w, PruneIndex, 'col', 0, 0)
+    w = SynapticPruning(w, PruneIndex, 'col', 0, 0, piece, is_training)
 
     neural_layer = np.dot(w, Input)
     return neural_layer,w
 
 def Cat(
     Input,               # list[num]: Input data.
     w,                   # list[list[num]]: Weight matrix of the neural network.
     membran_threshold,      # str: Sign for threshold comparison ('<', '>', '==', '!=').
     membran_potential,      # num: Threshold value for comparison.
-    isTrain              # int: Flag indicating if the function is called during training (1 for training, 0 otherwise).
+    isTrain,
+    piece              # int: Flag indicating if the function is called during training (1 for training, 0 otherwise).
 ) -> tuple:
     """
     Applies categorization process to the input data using synaptic pruning if specified.
 
     Args:
         Input (list[num]): Input data.
         w (list[list[num]]): Weight matrix of the neural network.
@@ -475,15 +502,15 @@
         PruneIndex = np.where(Input > membran_potential)
     elif membran_threshold == '==':
         PruneIndex = np.where(Input == membran_potential)
     elif membran_threshold == '!=':     
         PruneIndex = np.where(Input != membran_potential)
     if isTrain == 1 and membran_threshold != 'none':
      
-            w = SynapticPruning(w, PruneIndex, 'col', 0, 0)
+            w = SynapticPruning(w, PruneIndex, 'col', 0, 0, piece, isTrain)
      
     
     neural_layer = np.dot(w, Input)
     return neural_layer,w
 
 
 def Normalization(
@@ -553,14 +580,16 @@
         list[num]: Transformed data after applying ReLU function.
     """
 
     
     return np.maximum(0, x)
 
 
+
+
 def TestPLAN(
     x_test,         # list[list[num]]: Test input data.
     y_test,         # list[num]: Test labels.
     layers,             # list[str]: List of layer names.
     membran_thresholds,     # list[str]: List of MEMBRAN THRESHOLDS for each layer.
     membran_potentials,    # list[num]: List of MEMBRAN POTENTIALS for each layer.
     normalizations,    # str: Whether normalization will be performed ("y" or "n").
@@ -609,17 +638,17 @@
                         neural_layer = Relu(neural_layer)
                 elif activations[index] == 'sigmoid':
                         neural_layer = Sigmoid(neural_layer)
                 elif activations[index] == 'softmax':
                         neural_layer = Softmax(neural_layer)
                         
                 if layers[index] == 'fex':
-                    neural_layer,useless = Fex(neural_layer, W[index], membran_thresholds[index], membran_potentials[index])
+                    neural_layer,useless = Fex(neural_layer, W[index], membran_thresholds[index], membran_potentials[index],0,0)
                 if layers[index] == 'cat':
-                    neural_layer,useless = Cat(neural_layer, W[index], membran_thresholds[index], membran_potentials[index],0)
+                    neural_layer,useless = Cat(neural_layer, W[index], membran_thresholds[index], membran_potentials[index],0,0)
             for i, w in enumerate(Wc):
                 W[i] = np.copy(w)
             RealOutput = np.argmax(y_test[inpIndex])
             PredictedOutput = np.argmax(neural_layer)
             if RealOutput == PredictedOutput:
                 true += 1
             acc = true / len(y_test)
@@ -968,20 +997,20 @@
                 neural_layer = Sigmoid(neural_layer)
             elif activations[index] == 'softmax':
                 neural_layer = Softmax(neural_layer)
                                 
             if layers[index] == 'fex':
                 neural_layer,useless = Fex(neural_layer, W[index],
                                           membran_thresholds[index],
-                                          membran_potentials[index])
+                                          membran_potentials[index],0,0)
             if layers[index] == 'cat':
                 neural_layer,useless = Cat(neural_layer, W[index],
                                           membran_thresholds[index],
                                           membran_potentials[index],
-                                          0)
+                                          0,0)
     except:
        print(Fore.RED + "ERROR: The input was probably entered incorrectly. from: PredictFromDiscPLAN"  + infoPredictFromDİscPLAN + Style.RESET_ALL)
        return 'e'
     for i, w in enumerate(Wc):
         W[i] = np.copy(w)
     return neural_layer
 
@@ -1020,19 +1049,20 @@
                 neural_layer = Sigmoid(neural_layer)
             elif activations[index] == 'softmax':
                 neural_layer = Softmax(neural_layer)
                                 
             if layers[index] == 'fex':
                 neural_layer,useless = Fex(neural_layer, W[index],
                                           membran_thresholds[index],
-                                          membran_potentials[index])
+                                          membran_potentials[index],0,0)
             if layers[index] == 'cat':
                 neural_layer,useless = Cat(neural_layer, W[index],
                                           membran_thresholds[index],
-                                          membran_potentials[index],0)
+                                          membran_potentials[index],
+                                          0,0)
     except:
         print(Fore.RED + "ERROR: Unexpected input or wrong model parameters from: PredictFromRamPLAN."  + infoPredictFromRamPLAN + Style.RESET_ALL)
         return 'e'
     for i, w in enumerate(Wc):
         W[i] = np.copy(w)
     return neural_layer
```

### Comparing `pyerualjetwork-1.3.6/setup.py` & `pyerualjetwork-1.3.7/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 # Setting Up
 
 setup(
       
       name = "pyerualjetwork",
-      version = "1.3.6",
+      version = "1.3.7",
       author = "Hasan Can Beydili",
       author_email = "tchasancan@gmail.com",
-      description= "Advanced python deep learning library. New Features: 'SyntheticAugmentation' function added for unbalanced datasets. Changes for variable names to snake_case (Function names are still PascalCase). (Documentation in desc. Examples in GİTHUB: https://github.com/HCB06/PyerualJetwork)",
+      description= "Advanced python deep learning library. MASSIVE Technic Update, unlocked class limits. (Documentation in desc. Examples in GİTHUB: https://github.com/HCB06/PyerualJetwork)",
       packages = find_packages(),
       keywords = ["model evaluation", "classifcation", 'pruning learning artficial neural networks'],
 
       
       )
```

