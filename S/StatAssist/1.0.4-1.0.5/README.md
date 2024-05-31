# Comparing `tmp/StatAssist-1.0.4.tar.gz` & `tmp/StatAssist-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "StatAssist-1.0.4.tar", last modified: Thu May 23 01:45:58 2024, max compression
+gzip compressed data, was "StatAssist-1.0.5.tar", last modified: Fri May 31 16:15:34 2024, max compression
```

## Comparing `StatAssist-1.0.4.tar` & `StatAssist-1.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 01:45:58.891928 StatAssist-1.0.4/
--rw-rw-rw-   0        0        0     2253 2024-05-23 01:45:58.891928 StatAssist-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1745 2024-05-20 00:10:03.000000 StatAssist-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 01:45:58.876268 StatAssist-1.0.4/StatAssist/
--rw-rw-rw-   0        0        0      285 2024-05-23 01:43:37.000000 StatAssist-1.0.4/StatAssist/__init__.py
--rw-rw-rw-   0        0        0     2358 2024-05-19 19:35:48.000000 StatAssist-1.0.4/StatAssist/algebra.py
--rw-rw-rw-   0        0        0    15935 2024-05-20 05:11:46.000000 StatAssist-1.0.4/StatAssist/stats.py
--rw-rw-rw-   0        0        0    10009 2024-05-23 01:43:25.000000 StatAssist-1.0.4/StatAssist/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-23 01:45:58.891928 StatAssist-1.0.4/StatAssist.egg-info/
--rw-rw-rw-   0        0        0     2253 2024-05-23 01:45:58.000000 StatAssist-1.0.4/StatAssist.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2024-05-23 01:45:58.000000 StatAssist-1.0.4/StatAssist.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 01:45:58.000000 StatAssist-1.0.4/StatAssist.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2024-05-23 01:45:58.000000 StatAssist-1.0.4/StatAssist.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-23 01:45:58.000000 StatAssist-1.0.4/StatAssist.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 01:45:58.891928 StatAssist-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      816 2024-05-23 01:43:48.000000 StatAssist-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 16:15:34.352756 StatAssist-1.0.5/
+-rw-rw-rw-   0        0        0     2253 2024-05-31 16:15:34.349404 StatAssist-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1745 2024-05-23 02:37:53.000000 StatAssist-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-31 16:15:34.326665 StatAssist-1.0.5/StatAssist/
+-rw-rw-rw-   0        0        0      285 2024-05-23 02:37:53.000000 StatAssist-1.0.5/StatAssist/__init__.py
+-rw-rw-rw-   0        0        0     2358 2024-05-19 19:35:48.000000 StatAssist-1.0.5/StatAssist/algebra.py
+-rw-rw-rw-   0        0        0    15935 2024-05-27 20:53:16.000000 StatAssist-1.0.5/StatAssist/stats.py
+-rw-rw-rw-   0        0        0    11435 2024-05-31 15:58:29.000000 StatAssist-1.0.5/StatAssist/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-31 16:15:34.345958 StatAssist-1.0.5/StatAssist.egg-info/
+-rw-rw-rw-   0        0        0     2253 2024-05-31 16:15:34.000000 StatAssist-1.0.5/StatAssist.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2024-05-31 16:15:34.000000 StatAssist-1.0.5/StatAssist.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 16:15:34.000000 StatAssist-1.0.5/StatAssist.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-05-31 16:15:34.000000 StatAssist-1.0.5/StatAssist.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-31 16:15:34.000000 StatAssist-1.0.5/StatAssist.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-31 16:15:34.352756 StatAssist-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      816 2024-05-31 16:15:13.000000 StatAssist-1.0.5/setup.py
```

### Comparing `StatAssist-1.0.4/PKG-INFO` & `StatAssist-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: StatAssist
-Version: 1.0.4
+Version: 1.0.5
 Summary: Math tools for private or personal use.
 Author: Damion J. Quintanilla
 Author-email: djq314159@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -19,15 +19,15 @@
 StatAssist is a python library that provides statistical and mathematical functions as well as built-in algorithms such
 as integration and linear regression.
 
 ## Installation
 
 You can install StatAssist using pip:
 
-pip install StatAssist==1.0.3
+pip install StatAssist==1.0.5
 
 ## Usage
 
 Example 1:
 
 ```python
 from StatAssist import statistics_ as stats
```

### Comparing `StatAssist-1.0.4/README.md` & `StatAssist-1.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 StatAssist is a python library that provides statistical and mathematical functions as well as built-in algorithms such
 as integration and linear regression.
 
 ## Installation
 
 You can install StatAssist using pip:
 
-pip install StatAssist==1.0.3
+pip install StatAssist==1.0.5
 
 ## Usage
 
 Example 1:
 
 ```python
 from StatAssist import statistics_ as stats
```

### Comparing `StatAssist-1.0.4/StatAssist/algebra.py` & `StatAssist-1.0.5/StatAssist/algebra.py`

 * *Files identical despite different names*

### Comparing `StatAssist-1.0.4/StatAssist/stats.py` & `StatAssist-1.0.5/StatAssist/stats.py`

 * *Files identical despite different names*

### Comparing `StatAssist-1.0.4/StatAssist/utils.py` & `StatAssist-1.0.5/StatAssist/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -147,14 +147,58 @@
                     matrix[i][j] += cov/pow(variances[0]*variances[1], 0.5)
 
                 if i == j:
                     matrix[i][j] = 0
 
         return matrix
 
+    def multiple_linear_regression(self, data: list, depth: int) -> list:
+        pred = []
+        for d in range(depth):
+            # averages for data
+            averages = []
+            for dataset in data:
+                temp = 0
+                n = len(dataset)
+                for datapoint in dataset:
+                    temp += datapoint / n
+
+                averages.append(temp)
+            cols = len(data)
+
+            # variances for data
+            variances = []
+
+            if len(data) == len(averages):
+                for i in range(len(averages)):
+                    n = len(data[i])
+                    temp = 0
+
+                    for j in range(n):
+                        temp += pow(data[i][j] - averages[i], 2) / n
+
+                    variances.append(temp)
+
+            corr_coeff_matrix = self.correlation_coefficient_matrix(data)
+            A = [0 for i in range(cols)]
+            p_matrix = [A for i in range(cols)]
+
+            # p_matrix -> slope matrix
+            S = [0 for c in range(cols)]
+            for i in range(cols):
+                for j in range(cols):
+                    if corr_coeff_matrix[i][j] > 0.7 and i != j:
+                        p_matrix[i][j] += corr_coeff_matrix[i][j]*math.sqrt(variances[i]/variances[j])
+
+                    if i != j:
+                        S[i] += p_matrix[i][j]
+
+
+        return pred
+
     @staticmethod
     def integral(func, func_args: list, interval: list) -> float:
         """
         Returns the area under a defined continuous function on an interval.
         :param func: callable function with x as first param.
         :param func_args: list, arguments for callable function that returns float.
         :param interval: interval on which the geometric area is to be calculated.
```

### Comparing `StatAssist-1.0.4/StatAssist.egg-info/PKG-INFO` & `StatAssist-1.0.5/StatAssist.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: StatAssist
-Version: 1.0.4
+Version: 1.0.5
 Summary: Math tools for private or personal use.
 Author: Damion J. Quintanilla
 Author-email: djq314159@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -19,15 +19,15 @@
 StatAssist is a python library that provides statistical and mathematical functions as well as built-in algorithms such
 as integration and linear regression.
 
 ## Installation
 
 You can install StatAssist using pip:
 
-pip install StatAssist==1.0.3
+pip install StatAssist==1.0.5
 
 ## Usage
 
 Example 1:
 
 ```python
 from StatAssist import statistics_ as stats
```

### Comparing `StatAssist-1.0.4/setup.py` & `StatAssist-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="StatAssist",
-    version="1.0.4",
+    version="1.0.5",
     license='MIT',
     author="Damion J. Quintanilla",
     author_email="djq314159@gmail.com",
     description="Math tools for private or personal use.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
```

