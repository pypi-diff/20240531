# Comparing `tmp/predictions_sepsis-1.0.0.tar.gz` & `tmp/predictions_sepsis-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/predictions_sepsis-1.0.0.tar", last modified: Fri May 31 16:10:50 2024, max compression
+gzip compressed data, was "dist/predictions_sepsis-1.0.1.tar", last modified: Fri May 31 16:19:09 2024, max compression
```

## Comparing `predictions_sepsis-1.0.0.tar` & `predictions_sepsis-1.0.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 artemij    (501) staff       (20)        0 2024-05-31 16:10:50.000000 predictions_sepsis-1.0.0/
--rw-r--r--   0 artemij    (501) staff       (20)     5375 2024-05-31 16:10:50.000000 predictions_sepsis-1.0.0/PKG-INFO
-drwxr-xr-x   0 artemij    (501) staff       (20)        0 2024-05-31 16:10:50.000000 predictions_sepsis-1.0.0/predictions_sepsis.egg-info/
--rw-r--r--   0 artemij    (501) staff       (20)     5375 2024-05-31 16:10:50.000000 predictions_sepsis-1.0.0/predictions_sepsis.egg-info/PKG-INFO
--rw-r--r--   0 artemij    (501) staff       (20)      686 2024-05-31 16:10:50.000000 predictions_sepsis-1.0.0/predictions_sepsis.egg-info/SOURCES.txt
--rw-r--r--   0 artemij    (501) staff       (20)       64 2024-05-31 16:10:50.000000 predictions_sepsis-1.0.0/predictions_sepsis.egg-info/requires.txt
--rw-r--r--   0 artemij    (501) staff       (20)       19 2024-05-31 16:10:50.000000 predictions_sepsis-1.0.0/predictions_sepsis.egg-info/top_level.txt
--rw-r--r--   0 artemij    (501) staff       (20)        1 2024-05-31 16:10:50.000000 predictions_sepsis-1.0.0/predictions_sepsis.egg-info/dependency_links.txt
--rw-r--r--   0 artemij    (501) staff       (20)     3877 2024-05-31 16:03:00.000000 predictions_sepsis-1.0.0/README.md
--rw-r--r--   0 artemij    (501) staff       (20)      858 2024-05-31 16:10:26.000000 predictions_sepsis-1.0.0/setup.py
--rw-r--r--   0 artemij    (501) staff       (20)       38 2024-05-31 16:10:50.000000 predictions_sepsis-1.0.0/setup.cfg
-drwxr-xr-x   0 artemij    (501) staff       (20)        0 2024-05-31 16:10:50.000000 predictions_sepsis-1.0.0/predictions_sepsis/
--rw-r--r--   0 artemij    (501) staff       (20)     1774 2024-05-31 14:27:13.000000 predictions_sepsis-1.0.0/predictions_sepsis/choose.py
--rw-r--r--   0 artemij    (501) staff       (20)     7265 2024-05-31 12:49:20.000000 predictions_sepsis-1.0.0/predictions_sepsis/merge_diagnoses_and_ssir_with_blood.py
--rw-r--r--   0 artemij    (501) staff       (20)     3694 2024-05-31 13:59:27.000000 predictions_sepsis-1.0.0/predictions_sepsis/balance_on_patients.py
--rw-r--r--   0 artemij    (501) staff       (20)     4197 2024-05-31 15:34:40.000000 predictions_sepsis-1.0.0/predictions_sepsis/train_model.py
--rw-r--r--   0 artemij    (501) staff       (20)     4617 2024-05-31 12:49:20.000000 predictions_sepsis-1.0.0/predictions_sepsis/combine_diagnoses_and_ssir.py
--rw-r--r--   0 artemij    (501) staff       (20)     8414 2024-05-31 12:51:29.000000 predictions_sepsis-1.0.0/predictions_sepsis/transformers.py
--rw-r--r--   0 artemij    (501) staff       (20)     2822 2024-05-31 13:27:53.000000 predictions_sepsis-1.0.0/predictions_sepsis/get_ssir.py
--rw-r--r--   0 artemij    (501) staff       (20)     1464 2024-05-31 15:05:36.000000 predictions_sepsis-1.0.0/predictions_sepsis/fill_values.py
--rw-r--r--   0 artemij    (501) staff       (20)     1870 2024-05-31 12:49:20.000000 predictions_sepsis-1.0.0/predictions_sepsis/get_disease_info.py
--rw-r--r--   0 artemij    (501) staff       (20)     1690 2024-05-31 12:54:42.000000 predictions_sepsis-1.0.0/predictions_sepsis/get_diagnoses.py
--rw-r--r--   0 artemij    (501) staff       (20)      129 2024-05-30 17:47:12.000000 predictions_sepsis-1.0.0/predictions_sepsis/__init__.py
--rw-r--r--   0 artemij    (501) staff       (20)     1026 2024-05-31 14:16:45.000000 predictions_sepsis-1.0.0/predictions_sepsis/compress.py
+drwxr-xr-x   0 artemij    (501) staff       (20)        0 2024-05-31 16:19:09.000000 predictions_sepsis-1.0.1/
+-rw-r--r--   0 artemij    (501) staff       (20)     5375 2024-05-31 16:19:09.000000 predictions_sepsis-1.0.1/PKG-INFO
+drwxr-xr-x   0 artemij    (501) staff       (20)        0 2024-05-31 16:19:09.000000 predictions_sepsis-1.0.1/predictions_sepsis.egg-info/
+-rw-r--r--   0 artemij    (501) staff       (20)     5375 2024-05-31 16:19:09.000000 predictions_sepsis-1.0.1/predictions_sepsis.egg-info/PKG-INFO
+-rw-r--r--   0 artemij    (501) staff       (20)      686 2024-05-31 16:19:09.000000 predictions_sepsis-1.0.1/predictions_sepsis.egg-info/SOURCES.txt
+-rw-r--r--   0 artemij    (501) staff       (20)       64 2024-05-31 16:19:09.000000 predictions_sepsis-1.0.1/predictions_sepsis.egg-info/requires.txt
+-rw-r--r--   0 artemij    (501) staff       (20)       19 2024-05-31 16:19:09.000000 predictions_sepsis-1.0.1/predictions_sepsis.egg-info/top_level.txt
+-rw-r--r--   0 artemij    (501) staff       (20)        1 2024-05-31 16:19:09.000000 predictions_sepsis-1.0.1/predictions_sepsis.egg-info/dependency_links.txt
+-rw-r--r--   0 artemij    (501) staff       (20)     3877 2024-05-31 16:03:00.000000 predictions_sepsis-1.0.1/README.md
+-rw-r--r--   0 artemij    (501) staff       (20)      858 2024-05-31 16:19:00.000000 predictions_sepsis-1.0.1/setup.py
+-rw-r--r--   0 artemij    (501) staff       (20)       38 2024-05-31 16:19:09.000000 predictions_sepsis-1.0.1/setup.cfg
+drwxr-xr-x   0 artemij    (501) staff       (20)        0 2024-05-31 16:19:09.000000 predictions_sepsis-1.0.1/predictions_sepsis/
+-rw-r--r--   0 artemij    (501) staff       (20)     1774 2024-05-31 14:27:13.000000 predictions_sepsis-1.0.1/predictions_sepsis/choose.py
+-rw-r--r--   0 artemij    (501) staff       (20)     7265 2024-05-31 12:49:20.000000 predictions_sepsis-1.0.1/predictions_sepsis/merge_diagnoses_and_ssir_with_blood.py
+-rw-r--r--   0 artemij    (501) staff       (20)     3694 2024-05-31 13:59:27.000000 predictions_sepsis-1.0.1/predictions_sepsis/balance_on_patients.py
+-rw-r--r--   0 artemij    (501) staff       (20)     4197 2024-05-31 15:34:40.000000 predictions_sepsis-1.0.1/predictions_sepsis/train_model.py
+-rw-r--r--   0 artemij    (501) staff       (20)     4617 2024-05-31 12:49:20.000000 predictions_sepsis-1.0.1/predictions_sepsis/combine_diagnoses_and_ssir.py
+-rw-r--r--   0 artemij    (501) staff       (20)     8414 2024-05-31 12:51:29.000000 predictions_sepsis-1.0.1/predictions_sepsis/transformers.py
+-rw-r--r--   0 artemij    (501) staff       (20)     2822 2024-05-31 13:27:53.000000 predictions_sepsis-1.0.1/predictions_sepsis/get_ssir.py
+-rw-r--r--   0 artemij    (501) staff       (20)     1464 2024-05-31 15:05:36.000000 predictions_sepsis-1.0.1/predictions_sepsis/fill_values.py
+-rw-r--r--   0 artemij    (501) staff       (20)     1870 2024-05-31 12:49:20.000000 predictions_sepsis-1.0.1/predictions_sepsis/get_disease_info.py
+-rw-r--r--   0 artemij    (501) staff       (20)     1690 2024-05-31 12:54:42.000000 predictions_sepsis-1.0.1/predictions_sepsis/get_diagnoses.py
+-rw-r--r--   0 artemij    (501) staff       (20)      559 2024-05-31 16:17:57.000000 predictions_sepsis-1.0.1/predictions_sepsis/__init__.py
+-rw-r--r--   0 artemij    (501) staff       (20)     1026 2024-05-31 14:16:45.000000 predictions_sepsis-1.0.1/predictions_sepsis/compress.py
```

### Comparing `predictions_sepsis-1.0.0/PKG-INFO` & `predictions_sepsis-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: predictions_sepsis
-Version: 1.0.0
+Version: 1.0.1
 Summary: Module for sepsis predictions
 Home-page: https://github.com/sslavian812/sepsis-predictions.git
 Author: @Margo78, @akp1n
 Author-email: timtimk30@yandex.ru
 License: UNKNOWN
 Description: # Predictions sepsis
```

### Comparing `predictions_sepsis-1.0.0/predictions_sepsis.egg-info/PKG-INFO` & `predictions_sepsis-1.0.1/predictions_sepsis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: predictions-sepsis
-Version: 1.0.0
+Version: 1.0.1
 Summary: Module for sepsis predictions
 Home-page: https://github.com/sslavian812/sepsis-predictions.git
 Author: @Margo78, @akp1n
 Author-email: timtimk30@yandex.ru
 License: UNKNOWN
 Description: # Predictions sepsis
```

### Comparing `predictions_sepsis-1.0.0/predictions_sepsis.egg-info/SOURCES.txt` & `predictions_sepsis-1.0.1/predictions_sepsis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `predictions_sepsis-1.0.0/README.md` & `predictions_sepsis-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `predictions_sepsis-1.0.0/setup.py` & `predictions_sepsis-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 def readme():
     with open('README.md', 'r') as f:
         return f.read()
 
 setup(
     name='predictions_sepsis',
-    version='1.0.0',
+    version='1.0.1',
     author='@Margo78, @akp1n',
     author_email='timtimk30@yandex.ru',
     description='Module for sepsis predictions',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://github.com/sslavian812/sepsis-predictions.git',
     packages=find_packages(),
```

### Comparing `predictions_sepsis-1.0.0/predictions_sepsis/choose.py` & `predictions_sepsis-1.0.1/predictions_sepsis/choose.py`

 * *Files identical despite different names*

### Comparing `predictions_sepsis-1.0.0/predictions_sepsis/merge_diagnoses_and_ssir_with_blood.py` & `predictions_sepsis-1.0.1/predictions_sepsis/merge_diagnoses_and_ssir_with_blood.py`

 * *Files identical despite different names*

### Comparing `predictions_sepsis-1.0.0/predictions_sepsis/balance_on_patients.py` & `predictions_sepsis-1.0.1/predictions_sepsis/balance_on_patients.py`

 * *Files identical despite different names*

### Comparing `predictions_sepsis-1.0.0/predictions_sepsis/train_model.py` & `predictions_sepsis-1.0.1/predictions_sepsis/train_model.py`

 * *Files identical despite different names*

### Comparing `predictions_sepsis-1.0.0/predictions_sepsis/combine_diagnoses_and_ssir.py` & `predictions_sepsis-1.0.1/predictions_sepsis/combine_diagnoses_and_ssir.py`

 * *Files identical despite different names*

### Comparing `predictions_sepsis-1.0.0/predictions_sepsis/transformers.py` & `predictions_sepsis-1.0.1/predictions_sepsis/transformers.py`

 * *Files identical despite different names*

### Comparing `predictions_sepsis-1.0.0/predictions_sepsis/get_ssir.py` & `predictions_sepsis-1.0.1/predictions_sepsis/get_ssir.py`

 * *Files identical despite different names*

### Comparing `predictions_sepsis-1.0.0/predictions_sepsis/fill_values.py` & `predictions_sepsis-1.0.1/predictions_sepsis/fill_values.py`

 * *Files identical despite different names*

### Comparing `predictions_sepsis-1.0.0/predictions_sepsis/get_disease_info.py` & `predictions_sepsis-1.0.1/predictions_sepsis/get_disease_info.py`

 * *Files identical despite different names*

### Comparing `predictions_sepsis-1.0.0/predictions_sepsis/get_diagnoses.py` & `predictions_sepsis-1.0.1/predictions_sepsis/get_diagnoses.py`

 * *Files identical despite different names*

### Comparing `predictions_sepsis-1.0.0/predictions_sepsis/compress.py` & `predictions_sepsis-1.0.1/predictions_sepsis/compress.py`

 * *Files identical despite different names*

