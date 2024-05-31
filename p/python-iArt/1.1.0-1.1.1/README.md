# Comparing `tmp/python-iArt-1.1.0.tar.gz` & `tmp/python-iArt-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-iArt-1.1.0.tar", last modified: Tue Apr 30 04:56:14 2024, max compression
+gzip compressed data, was "python-iArt-1.1.1.tar", last modified: Fri May 31 02:45:24 2024, max compression
```

## Comparing `python-iArt-1.1.0.tar` & `python-iArt-1.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jiaweizhang   (501) staff       (20)        0 2024-04-30 04:56:14.582780 python-iArt-1.1.0/
--rw-r--r--   0 jiaweizhang   (501) staff       (20)     5230 2024-04-30 04:56:14.582526 python-iArt-1.1.0/PKG-INFO
--rw-r--r--   0 jiaweizhang   (501) staff       (20)     3930 2024-04-09 03:41:46.000000 python-iArt-1.1.0/README.md
-drwxr-xr-x   0 jiaweizhang   (501) staff       (20)        0 2024-04-30 04:56:14.580594 python-iArt-1.1.0/iArt/
--rw-r--r--   0 jiaweizhang   (501) staff       (20)       48 2024-04-09 03:34:10.000000 python-iArt-1.1.0/iArt/__init__.py
--rw-r--r--   0 jiaweizhang   (501) staff       (20)    18075 2024-04-30 04:55:09.000000 python-iArt-1.1.0/iArt/iArt.py
-drwxr-xr-x   0 jiaweizhang   (501) staff       (20)        0 2024-04-30 04:56:14.582113 python-iArt-1.1.0/python_iArt.egg-info/
--rw-r--r--   0 jiaweizhang   (501) staff       (20)     5230 2024-04-30 04:56:14.000000 python-iArt-1.1.0/python_iArt.egg-info/PKG-INFO
--rw-r--r--   0 jiaweizhang   (501) staff       (20)      222 2024-04-30 04:56:14.000000 python-iArt-1.1.0/python_iArt.egg-info/SOURCES.txt
--rw-r--r--   0 jiaweizhang   (501) staff       (20)        1 2024-04-30 04:56:14.000000 python-iArt-1.1.0/python_iArt.egg-info/dependency_links.txt
--rw-r--r--   0 jiaweizhang   (501) staff       (20)       66 2024-04-30 04:56:14.000000 python-iArt-1.1.0/python_iArt.egg-info/requires.txt
--rw-r--r--   0 jiaweizhang   (501) staff       (20)        5 2024-04-30 04:56:14.000000 python-iArt-1.1.0/python_iArt.egg-info/top_level.txt
--rw-r--r--   0 jiaweizhang   (501) staff       (20)       38 2024-04-30 04:56:14.582896 python-iArt-1.1.0/setup.cfg
--rw-r--r--   0 jiaweizhang   (501) staff       (20)     1059 2024-04-30 04:55:27.000000 python-iArt-1.1.0/setup.py
+drwxr-xr-x   0 jiaweizhang   (501) staff       (20)        0 2024-05-31 02:45:24.513364 python-iArt-1.1.1/
+-rw-r--r--   0 jiaweizhang   (501) staff       (20)     5230 2024-05-31 02:45:24.513010 python-iArt-1.1.1/PKG-INFO
+-rw-r--r--   0 jiaweizhang   (501) staff       (20)     3930 2024-04-09 03:41:46.000000 python-iArt-1.1.1/README.md
+drwxr-xr-x   0 jiaweizhang   (501) staff       (20)        0 2024-05-31 02:45:24.509439 python-iArt-1.1.1/iArt/
+-rw-r--r--   0 jiaweizhang   (501) staff       (20)       48 2024-05-31 02:44:49.000000 python-iArt-1.1.1/iArt/__init__.py
+-rw-r--r--   0 jiaweizhang   (501) staff       (20)    17146 2024-05-31 02:33:31.000000 python-iArt-1.1.1/iArt/iArt.py
+drwxr-xr-x   0 jiaweizhang   (501) staff       (20)        0 2024-05-31 02:45:24.512251 python-iArt-1.1.1/python_iArt.egg-info/
+-rw-r--r--   0 jiaweizhang   (501) staff       (20)     5230 2024-05-31 02:45:24.000000 python-iArt-1.1.1/python_iArt.egg-info/PKG-INFO
+-rw-r--r--   0 jiaweizhang   (501) staff       (20)      222 2024-05-31 02:45:24.000000 python-iArt-1.1.1/python_iArt.egg-info/SOURCES.txt
+-rw-r--r--   0 jiaweizhang   (501) staff       (20)        1 2024-05-31 02:45:24.000000 python-iArt-1.1.1/python_iArt.egg-info/dependency_links.txt
+-rw-r--r--   0 jiaweizhang   (501) staff       (20)       66 2024-05-31 02:45:24.000000 python-iArt-1.1.1/python_iArt.egg-info/requires.txt
+-rw-r--r--   0 jiaweizhang   (501) staff       (20)        5 2024-05-31 02:45:24.000000 python-iArt-1.1.1/python_iArt.egg-info/top_level.txt
+-rw-r--r--   0 jiaweizhang   (501) staff       (20)       38 2024-05-31 02:45:24.513518 python-iArt-1.1.1/setup.cfg
+-rw-r--r--   0 jiaweizhang   (501) staff       (20)     1059 2024-05-31 02:45:08.000000 python-iArt-1.1.1/setup.py
```

### Comparing `python-iArt-1.1.0/PKG-INFO` & `python-iArt-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-iArt
-Version: 1.1.0
+Version: 1.1.1
 Summary: iArt: A Generalized Framework for Imputation-Assisted Randomization Tests
 Home-page: https://github.com/Imputation-Assisted-Randomization-Tests/iArt-py
 Author: Siyu Heng, Jiawei Zhang, and Yang Feng
 Author-email: siyuheng@nyu.edu,jz4721@nyu.edu,yang.feng@nyu.edu
 License: UNKNOWN
 Description: # iArt: Imputation-Assisted Randomization Tests
```

### Comparing `python-iArt-1.1.0/README.md` & `python-iArt-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `python-iArt-1.1.0/iArt/iArt.py` & `python-iArt-1.1.1/iArt/iArt.py`

 * *Files 8% similar despite different names*

```diff
@@ -111,47 +111,22 @@
         my_list.append((z[i],y[i]))
     sorted_list = sorted(my_list, key=lambda x: x[1])
     for i in range(n):
         t += sorted_list[i][0] * (i + 1)
 
     return t
 
-def split(y, z, M):
-    """
-    Split the data into missing and non-missing parts
-    """
-    
-    missing_indices = M[:].astype(bool)
-    non_missing_indices = ~missing_indices
-
-    y_missing = y[missing_indices].reshape(-1,)
-    y_non_missing = y[non_missing_indices].reshape(-1,)
-
-    z_missing = z[missing_indices].reshape(-1,)
-    z_non_missing = z[non_missing_indices].reshape(-1,)
-
-    return y_missing, y_non_missing, z_missing, z_non_missing
-
 def getT(y, z, lenY, M):
     """
-    Separately calculate T for missing and non-missing parts of each outcome using Wilcoxon rank sum test
-    Return the sum of T values for all outcomes
+    Calculate the Wilcoxon rank sum test statistics for each outcome
     """
 
     t = []
     for i in range(lenY):
-        # Split the data into missing and non-missing parts using the split function
-        y_missing, y_non_missing, z_missing, z_non_missing = split(y[:,i], z, M[:,i])
-        
-        # Calculate T for missing and non-missing parts
-        t_missing = T(z_missing, y_missing.reshape(-1,))
-        t_non_missing = T(z_non_missing, y_non_missing.reshape(-1,))
-
-        # Sum the T values for both parts
-        t_combined = t_missing + t_non_missing
+        t_combined = T(z.reshape(-1,), y[:,i].reshape(-1,))
         t.append(t_combined)
 
     return np.array(t)
 
 def getZsimTemplates(Z_sorted, S):
     """
     Create a Z_sim template for each unique value in S
```

### Comparing `python-iArt-1.1.0/python_iArt.egg-info/PKG-INFO` & `python-iArt-1.1.1/python_iArt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-iArt
-Version: 1.1.0
+Version: 1.1.1
 Summary: iArt: A Generalized Framework for Imputation-Assisted Randomization Tests
 Home-page: https://github.com/Imputation-Assisted-Randomization-Tests/iArt-py
 Author: Siyu Heng, Jiawei Zhang, and Yang Feng
 Author-email: siyuheng@nyu.edu,jz4721@nyu.edu,yang.feng@nyu.edu
 License: UNKNOWN
 Description: # iArt: Imputation-Assisted Randomization Tests
```

### Comparing `python-iArt-1.1.0/setup.py` & `python-iArt-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="python-iArt",
-    version="1.1.0",
+    version="1.1.1",
     author="Siyu Heng, Jiawei Zhang, and Yang Feng",
     author_email="siyuheng@nyu.edu,jz4721@nyu.edu,yang.feng@nyu.edu",
     description="iArt: A Generalized Framework for Imputation-Assisted Randomization Tests",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Imputation-Assisted-Randomization-Tests/iArt-py",
     packages=find_packages(),
```

