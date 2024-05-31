# Comparing `tmp/predictions_sepsis-1.0.2.tar.gz` & `tmp/predictions_sepsis-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/predictions_sepsis-1.0.2.tar", last modified: Fri May 31 16:29:45 2024, max compression
+gzip compressed data, was "dist/predictions_sepsis-1.0.3.tar", last modified: Fri May 31 16:33:49 2024, max compression
```

## Comparing `predictions_sepsis-1.0.2.tar` & `predictions_sepsis-1.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 artemij    (501) staff       (20)        0 2024-05-31 16:29:45.000000 predictions_sepsis-1.0.2/
--rw-r--r--   0 artemij    (501) staff       (20)     5375 2024-05-31 16:29:45.000000 predictions_sepsis-1.0.2/PKG-INFO
-drwxr-xr-x   0 artemij    (501) staff       (20)        0 2024-05-31 16:29:45.000000 predictions_sepsis-1.0.2/predictions_sepsis.egg-info/
--rw-r--r--   0 artemij    (501) staff       (20)     5375 2024-05-31 16:29:45.000000 predictions_sepsis-1.0.2/predictions_sepsis.egg-info/PKG-INFO
--rw-r--r--   0 artemij    (501) staff       (20)      686 2024-05-31 16:29:45.000000 predictions_sepsis-1.0.2/predictions_sepsis.egg-info/SOURCES.txt
--rw-r--r--   0 artemij    (501) staff       (20)      138 2024-05-31 16:29:45.000000 predictions_sepsis-1.0.2/predictions_sepsis.egg-info/requires.txt
--rw-r--r--   0 artemij    (501) staff       (20)       19 2024-05-31 16:29:45.000000 predictions_sepsis-1.0.2/predictions_sepsis.egg-info/top_level.txt
--rw-r--r--   0 artemij    (501) staff       (20)        1 2024-05-31 16:29:45.000000 predictions_sepsis-1.0.2/predictions_sepsis.egg-info/dependency_links.txt
--rw-r--r--   0 artemij    (501) staff       (20)     3877 2024-05-31 16:03:00.000000 predictions_sepsis-1.0.2/README.md
--rw-r--r--   0 artemij    (501) staff       (20)      976 2024-05-31 16:29:37.000000 predictions_sepsis-1.0.2/setup.py
--rw-r--r--   0 artemij    (501) staff       (20)       38 2024-05-31 16:29:45.000000 predictions_sepsis-1.0.2/setup.cfg
-drwxr-xr-x   0 artemij    (501) staff       (20)        0 2024-05-31 16:29:45.000000 predictions_sepsis-1.0.2/predictions_sepsis/
--rw-r--r--   0 artemij    (501) staff       (20)     1774 2024-05-31 14:27:13.000000 predictions_sepsis-1.0.2/predictions_sepsis/choose.py
--rw-r--r--   0 artemij    (501) staff       (20)     7265 2024-05-31 12:49:20.000000 predictions_sepsis-1.0.2/predictions_sepsis/merge_diagnoses_and_ssir_with_blood.py
--rw-r--r--   0 artemij    (501) staff       (20)     3694 2024-05-31 13:59:27.000000 predictions_sepsis-1.0.2/predictions_sepsis/balance_on_patients.py
--rw-r--r--   0 artemij    (501) staff       (20)     4197 2024-05-31 15:34:40.000000 predictions_sepsis-1.0.2/predictions_sepsis/train_model.py
--rw-r--r--   0 artemij    (501) staff       (20)     4617 2024-05-31 12:49:20.000000 predictions_sepsis-1.0.2/predictions_sepsis/combine_diagnoses_and_ssir.py
--rw-r--r--   0 artemij    (501) staff       (20)     8414 2024-05-31 12:51:29.000000 predictions_sepsis-1.0.2/predictions_sepsis/transformers.py
--rw-r--r--   0 artemij    (501) staff       (20)     2822 2024-05-31 13:27:53.000000 predictions_sepsis-1.0.2/predictions_sepsis/get_ssir.py
--rw-r--r--   0 artemij    (501) staff       (20)     1464 2024-05-31 15:05:36.000000 predictions_sepsis-1.0.2/predictions_sepsis/fill_values.py
--rw-r--r--   0 artemij    (501) staff       (20)     1870 2024-05-31 12:49:20.000000 predictions_sepsis-1.0.2/predictions_sepsis/get_disease_info.py
--rw-r--r--   0 artemij    (501) staff       (20)     1690 2024-05-31 12:54:42.000000 predictions_sepsis-1.0.2/predictions_sepsis/get_diagnoses.py
--rw-r--r--   0 artemij    (501) staff       (20)      853 2024-05-31 16:27:17.000000 predictions_sepsis-1.0.2/predictions_sepsis/__init__.py
--rw-r--r--   0 artemij    (501) staff       (20)     1026 2024-05-31 14:16:45.000000 predictions_sepsis-1.0.2/predictions_sepsis/compress.py
+drwxr-xr-x   0 artemij    (501) staff       (20)        0 2024-05-31 16:33:49.000000 predictions_sepsis-1.0.3/
+-rw-r--r--   0 artemij    (501) staff       (20)     5375 2024-05-31 16:33:49.000000 predictions_sepsis-1.0.3/PKG-INFO
+drwxr-xr-x   0 artemij    (501) staff       (20)        0 2024-05-31 16:33:49.000000 predictions_sepsis-1.0.3/predictions_sepsis.egg-info/
+-rw-r--r--   0 artemij    (501) staff       (20)     5375 2024-05-31 16:33:49.000000 predictions_sepsis-1.0.3/predictions_sepsis.egg-info/PKG-INFO
+-rw-r--r--   0 artemij    (501) staff       (20)      686 2024-05-31 16:33:49.000000 predictions_sepsis-1.0.3/predictions_sepsis.egg-info/SOURCES.txt
+-rw-r--r--   0 artemij    (501) staff       (20)      138 2024-05-31 16:33:49.000000 predictions_sepsis-1.0.3/predictions_sepsis.egg-info/requires.txt
+-rw-r--r--   0 artemij    (501) staff       (20)       19 2024-05-31 16:33:49.000000 predictions_sepsis-1.0.3/predictions_sepsis.egg-info/top_level.txt
+-rw-r--r--   0 artemij    (501) staff       (20)        1 2024-05-31 16:33:49.000000 predictions_sepsis-1.0.3/predictions_sepsis.egg-info/dependency_links.txt
+-rw-r--r--   0 artemij    (501) staff       (20)     3877 2024-05-31 16:03:00.000000 predictions_sepsis-1.0.3/README.md
+-rw-r--r--   0 artemij    (501) staff       (20)      976 2024-05-31 16:33:34.000000 predictions_sepsis-1.0.3/setup.py
+-rw-r--r--   0 artemij    (501) staff       (20)       38 2024-05-31 16:33:49.000000 predictions_sepsis-1.0.3/setup.cfg
+drwxr-xr-x   0 artemij    (501) staff       (20)        0 2024-05-31 16:33:49.000000 predictions_sepsis-1.0.3/predictions_sepsis/
+-rw-r--r--   0 artemij    (501) staff       (20)     1774 2024-05-31 14:27:13.000000 predictions_sepsis-1.0.3/predictions_sepsis/choose.py
+-rw-r--r--   0 artemij    (501) staff       (20)     7265 2024-05-31 12:49:20.000000 predictions_sepsis-1.0.3/predictions_sepsis/merge_diagnoses_and_ssir_with_blood.py
+-rw-r--r--   0 artemij    (501) staff       (20)     3694 2024-05-31 13:59:27.000000 predictions_sepsis-1.0.3/predictions_sepsis/balance_on_patients.py
+-rw-r--r--   0 artemij    (501) staff       (20)     4197 2024-05-31 15:34:40.000000 predictions_sepsis-1.0.3/predictions_sepsis/train_model.py
+-rw-r--r--   0 artemij    (501) staff       (20)     4617 2024-05-31 12:49:20.000000 predictions_sepsis-1.0.3/predictions_sepsis/combine_diagnoses_and_ssir.py
+-rw-r--r--   0 artemij    (501) staff       (20)     8414 2024-05-31 12:51:29.000000 predictions_sepsis-1.0.3/predictions_sepsis/transformers.py
+-rw-r--r--   0 artemij    (501) staff       (20)     2822 2024-05-31 13:27:53.000000 predictions_sepsis-1.0.3/predictions_sepsis/get_ssir.py
+-rw-r--r--   0 artemij    (501) staff       (20)     1464 2024-05-31 15:05:36.000000 predictions_sepsis-1.0.3/predictions_sepsis/fill_values.py
+-rw-r--r--   0 artemij    (501) staff       (20)     1870 2024-05-31 12:49:20.000000 predictions_sepsis-1.0.3/predictions_sepsis/get_disease_info.py
+-rw-r--r--   0 artemij    (501) staff       (20)     1690 2024-05-31 12:54:42.000000 predictions_sepsis-1.0.3/predictions_sepsis/get_diagnoses.py
+-rw-r--r--   0 artemij    (501) staff       (20)      863 2024-05-31 16:33:34.000000 predictions_sepsis-1.0.3/predictions_sepsis/__init__.py
+-rw-r--r--   0 artemij    (501) staff       (20)     1026 2024-05-31 14:16:45.000000 predictions_sepsis-1.0.3/predictions_sepsis/compress.py
```

### Comparing `predictions_sepsis-1.0.2/PKG-INFO` & `predictions_sepsis-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: predictions_sepsis
-Version: 1.0.2
+Version: 1.0.3
 Summary: Module for sepsis predictions
 Home-page: https://github.com/sslavian812/sepsis-predictions.git
 Author: @Margo78, @akp1n
 Author-email: timtimk30@yandex.ru
 License: UNKNOWN
 Description: # Predictions sepsis
```

### Comparing `predictions_sepsis-1.0.2/predictions_sepsis.egg-info/PKG-INFO` & `predictions_sepsis-1.0.3/predictions_sepsis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: predictions-sepsis
-Version: 1.0.2
+Version: 1.0.3
 Summary: Module for sepsis predictions
 Home-page: https://github.com/sslavian812/sepsis-predictions.git
 Author: @Margo78, @akp1n
 Author-email: timtimk30@yandex.ru
 License: UNKNOWN
 Description: # Predictions sepsis
```

### Comparing `predictions_sepsis-1.0.2/predictions_sepsis.egg-info/SOURCES.txt` & `predictions_sepsis-1.0.3/predictions_sepsis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `predictions_sepsis-1.0.2/README.md` & `predictions_sepsis-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `predictions_sepsis-1.0.2/setup.py` & `predictions_sepsis-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 def readme():
     with open('README.md', 'r') as f:
         return f.read()
 
 setup(
     name='predictions_sepsis',
-    version='1.0.2',
+    version='1.0.3',
     author='@Margo78, @akp1n',
     author_email='timtimk30@yandex.ru',
     description='Module for sepsis predictions',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://github.com/sslavian812/sepsis-predictions.git',
     packages=find_packages(),
```

### Comparing `predictions_sepsis-1.0.2/predictions_sepsis/choose.py` & `predictions_sepsis-1.0.3/predictions_sepsis/choose.py`

 * *Files identical despite different names*

### Comparing `predictions_sepsis-1.0.2/predictions_sepsis/merge_diagnoses_and_ssir_with_blood.py` & `predictions_sepsis-1.0.3/predictions_sepsis/merge_diagnoses_and_ssir_with_blood.py`

 * *Files identical despite different names*

### Comparing `predictions_sepsis-1.0.2/predictions_sepsis/balance_on_patients.py` & `predictions_sepsis-1.0.3/predictions_sepsis/balance_on_patients.py`

 * *Files identical despite different names*

### Comparing `predictions_sepsis-1.0.2/predictions_sepsis/train_model.py` & `predictions_sepsis-1.0.3/predictions_sepsis/train_model.py`

 * *Files identical despite different names*

### Comparing `predictions_sepsis-1.0.2/predictions_sepsis/combine_diagnoses_and_ssir.py` & `predictions_sepsis-1.0.3/predictions_sepsis/combine_diagnoses_and_ssir.py`

 * *Files identical despite different names*

### Comparing `predictions_sepsis-1.0.2/predictions_sepsis/transformers.py` & `predictions_sepsis-1.0.3/predictions_sepsis/transformers.py`

 * *Files identical despite different names*

### Comparing `predictions_sepsis-1.0.2/predictions_sepsis/get_ssir.py` & `predictions_sepsis-1.0.3/predictions_sepsis/get_ssir.py`

 * *Files identical despite different names*

### Comparing `predictions_sepsis-1.0.2/predictions_sepsis/fill_values.py` & `predictions_sepsis-1.0.3/predictions_sepsis/fill_values.py`

 * *Files identical despite different names*

### Comparing `predictions_sepsis-1.0.2/predictions_sepsis/get_disease_info.py` & `predictions_sepsis-1.0.3/predictions_sepsis/get_disease_info.py`

 * *Files identical despite different names*

### Comparing `predictions_sepsis-1.0.2/predictions_sepsis/get_diagnoses.py` & `predictions_sepsis-1.0.3/predictions_sepsis/get_diagnoses.py`

 * *Files identical despite different names*

### Comparing `predictions_sepsis-1.0.2/predictions_sepsis/__init__.py` & `predictions_sepsis-1.0.3/predictions_sepsis/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 from .get_diagnoses import get_diagnoses
 from .get_ssir import get_ssir
 from .get_disease_info import get_diseas_info
 from .balance_on_patients import balance_on_patients
 from .choose import choose
 from .combine_diagnoses_and_ssir import combine_diagnoses_and_ssir
 from .compress import compress
-from fill_values import fill_values
-from merge_diagnoses_and_ssir_with_blood import merge_diagnoses_and_ssir_with_blood
-from train_model import train_model
-from transformers import process_chartevents
-from transformers import add_diagnosis_column
-from transformers import impute_data
-from transformers import prepare_and_save_data
-from transformers import resample_test_val_data
-from transformers import train_tabnet_model
-from transformers import evaluate_tabnet_model
+from .fill_values import fill_values
+from .merge_diagnoses_and_ssir_with_blood import merge_diagnoses_and_ssir_with_blood
+from .train_model import train_model
+from .transformers import process_chartevents
+from .transformers import add_diagnosis_column
+from .transformers import impute_data
+from .transformers import prepare_and_save_data
+from .transformers import resample_test_val_data
+from .transformers import train_tabnet_model
+from .transformers import evaluate_tabnet_model
 def hello_world():
     print("Hello, world! Version 2")
 
 print("")
```

### Comparing `predictions_sepsis-1.0.2/predictions_sepsis/compress.py` & `predictions_sepsis-1.0.3/predictions_sepsis/compress.py`

 * *Files identical despite different names*

