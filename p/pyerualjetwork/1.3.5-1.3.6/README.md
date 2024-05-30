# Comparing `tmp/pyerualjetwork-1.3.5.tar.gz` & `tmp/pyerualjetwork-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyerualjetwork-1.3.5.tar", last modified: Thu May 30 02:07:32 2024, max compression
+gzip compressed data, was "pyerualjetwork-1.3.6.tar", last modified: Thu May 30 02:18:14 2024, max compression
```

## Comparing `pyerualjetwork-1.3.5.tar` & `pyerualjetwork-1.3.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 02:07:32.304244 pyerualjetwork-1.3.5/
--rw-rw-rw-   0        0        0      502 2024-05-30 02:07:32.304244 pyerualjetwork-1.3.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-30 02:07:32.266201 pyerualjetwork-1.3.5/plan/
--rw-rw-rw-   0        0        0      375 2024-05-29 18:09:13.000000 pyerualjetwork-1.3.5/plan/__init__.py
--rw-rw-rw-   0        0        0    44286 2024-05-30 02:06:18.000000 pyerualjetwork-1.3.5/plan/plan.py
-drwxrwxrwx   0        0        0        0 2024-05-30 02:07:32.304244 pyerualjetwork-1.3.5/pyerualjetwork.egg-info/
--rw-rw-rw-   0        0        0      502 2024-05-30 02:07:31.000000 pyerualjetwork-1.3.5/pyerualjetwork.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2024-05-30 02:07:32.000000 pyerualjetwork-1.3.5/pyerualjetwork.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 02:07:31.000000 pyerualjetwork-1.3.5/pyerualjetwork.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-30 02:07:31.000000 pyerualjetwork-1.3.5/pyerualjetwork.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-30 02:07:32.304244 pyerualjetwork-1.3.5/setup.cfg
--rw-rw-rw-   0        0        0      681 2024-05-30 02:07:11.000000 pyerualjetwork-1.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 02:18:14.918068 pyerualjetwork-1.3.6/
+-rw-rw-rw-   0        0        0      502 2024-05-30 02:18:14.910553 pyerualjetwork-1.3.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-30 02:18:14.879936 pyerualjetwork-1.3.6/plan/
+-rw-rw-rw-   0        0        0      375 2024-05-29 18:09:13.000000 pyerualjetwork-1.3.6/plan/__init__.py
+-rw-rw-rw-   0        0        0    44211 2024-05-30 02:10:10.000000 pyerualjetwork-1.3.6/plan/plan.py
+drwxrwxrwx   0        0        0        0 2024-05-30 02:18:14.910553 pyerualjetwork-1.3.6/pyerualjetwork.egg-info/
+-rw-rw-rw-   0        0        0      502 2024-05-30 02:18:14.000000 pyerualjetwork-1.3.6/pyerualjetwork.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2024-05-30 02:18:14.000000 pyerualjetwork-1.3.6/pyerualjetwork.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 02:18:14.000000 pyerualjetwork-1.3.6/pyerualjetwork.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-30 02:18:14.000000 pyerualjetwork-1.3.6/pyerualjetwork.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-30 02:18:14.918068 pyerualjetwork-1.3.6/setup.cfg
+-rw-rw-rw-   0        0        0      681 2024-05-30 02:10:15.000000 pyerualjetwork-1.3.6/setup.py
```

### Comparing `pyerualjetwork-1.3.5/plan/plan.py` & `pyerualjetwork-1.3.6/plan/plan.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,35 +1,28 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Thu May 30 05:00:38 2024
-
-@author: hasan
-"""
-
 import numpy as np
 import time
 from colorama import Fore,Style
 from typing import List, Union
 import math
 from scipy.special import expit, softmax
 import matplotlib.pyplot as plt
 import seaborn as sns
 
 # BUILD -----
 def TrainPLAN(
     x_train: List[Union[int, float]], 
     y_train: List[Union[int, float, str]], # At least two.. and one hot encoded
     class_count: int,
-    layers = ['fex','cat'],
-    neurons = [],
-    membran_thresholds  = ['<','=='],
-    membran_potentials = [0.01,0],
-    normalizations = ['y','y'],
-    activations = ['none','none'],
-    visualize = 'n'
+    layers: List[str],
+    neurons: List[Union[int, float]],
+    membran_thresholds: List[str],
+    membran_potentials: List[Union[int, float]],
+    normalizations: List[str],
+    activations: List[str],
+    visualize: str
 ) -> str:
         
     infoPLAN = """
     Creates and configures a PLAN model.
     
     Args:
         x_train (list[num]): List of input data.
```

### Comparing `pyerualjetwork-1.3.5/setup.py` & `pyerualjetwork-1.3.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 # Setting Up
 
 setup(
       
       name = "pyerualjetwork",
-      version = "1.3.5",
+      version = "1.3.6",
       author = "Hasan Can Beydili",
       author_email = "tchasancan@gmail.com",
       description= "Advanced python deep learning library. New Features: 'SyntheticAugmentation' function added for unbalanced datasets. Changes for variable names to snake_case (Function names are still PascalCase). (Documentation in desc. Examples in GİTHUB: https://github.com/HCB06/PyerualJetwork)",
       packages = find_packages(),
       keywords = ["model evaluation", "classifcation", 'pruning learning artficial neural networks'],
```

