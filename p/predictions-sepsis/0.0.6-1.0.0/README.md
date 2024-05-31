# Comparing `tmp/predictions_sepsis-0.0.6.tar.gz` & `tmp/predictions_sepsis-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/predictions_sepsis-0.0.6.tar", last modified: Thu May 30 17:47:43 2024, max compression
+gzip compressed data, was "dist/predictions_sepsis-1.0.0.tar", last modified: Fri May 31 16:10:50 2024, max compression
```

## Comparing `predictions_sepsis-0.0.6.tar` & `predictions_sepsis-1.0.0.tar`

### file list

```diff
@@ -1,14 +1,24 @@
-drwxr-xr-x   0 artemij    (501) staff       (20)        0 2024-05-30 17:47:43.000000 predictions_sepsis-0.0.6/
--rw-r--r--   0 artemij    (501) staff       (20)      529 2024-05-30 17:47:43.000000 predictions_sepsis-0.0.6/PKG-INFO
-drwxr-xr-x   0 artemij    (501) staff       (20)        0 2024-05-30 17:47:43.000000 predictions_sepsis-0.0.6/predictions_sepsis.egg-info/
--rw-r--r--   0 artemij    (501) staff       (20)      529 2024-05-30 17:47:43.000000 predictions_sepsis-0.0.6/predictions_sepsis.egg-info/PKG-INFO
--rw-r--r--   0 artemij    (501) staff       (20)      304 2024-05-30 17:47:43.000000 predictions_sepsis-0.0.6/predictions_sepsis.egg-info/SOURCES.txt
--rw-r--r--   0 artemij    (501) staff       (20)       31 2024-05-30 17:47:43.000000 predictions_sepsis-0.0.6/predictions_sepsis.egg-info/requires.txt
--rw-r--r--   0 artemij    (501) staff       (20)       19 2024-05-30 17:47:43.000000 predictions_sepsis-0.0.6/predictions_sepsis.egg-info/top_level.txt
--rw-r--r--   0 artemij    (501) staff       (20)        1 2024-05-30 17:47:43.000000 predictions_sepsis-0.0.6/predictions_sepsis.egg-info/dependency_links.txt
--rw-r--r--   0 artemij    (501) staff       (20)        0 2024-05-30 15:10:11.000000 predictions_sepsis-0.0.6/README.md
--rw-r--r--   0 artemij    (501) staff       (20)      803 2024-05-30 17:47:41.000000 predictions_sepsis-0.0.6/setup.py
--rw-r--r--   0 artemij    (501) staff       (20)       38 2024-05-30 17:47:43.000000 predictions_sepsis-0.0.6/setup.cfg
-drwxr-xr-x   0 artemij    (501) staff       (20)        0 2024-05-30 17:47:43.000000 predictions_sepsis-0.0.6/predictions_sepsis/
--rw-r--r--   0 artemij    (501) staff       (20)     1725 2024-05-30 17:47:12.000000 predictions_sepsis-0.0.6/predictions_sepsis/get_diagnoses.py
--rw-r--r--   0 artemij    (501) staff       (20)      129 2024-05-30 17:47:12.000000 predictions_sepsis-0.0.6/predictions_sepsis/__init__.py
+drwxr-xr-x   0 artemij    (501) staff       (20)        0 2024-05-31 16:10:50.000000 predictions_sepsis-1.0.0/
+-rw-r--r--   0 artemij    (501) staff       (20)     5375 2024-05-31 16:10:50.000000 predictions_sepsis-1.0.0/PKG-INFO
+drwxr-xr-x   0 artemij    (501) staff       (20)        0 2024-05-31 16:10:50.000000 predictions_sepsis-1.0.0/predictions_sepsis.egg-info/
+-rw-r--r--   0 artemij    (501) staff       (20)     5375 2024-05-31 16:10:50.000000 predictions_sepsis-1.0.0/predictions_sepsis.egg-info/PKG-INFO
+-rw-r--r--   0 artemij    (501) staff       (20)      686 2024-05-31 16:10:50.000000 predictions_sepsis-1.0.0/predictions_sepsis.egg-info/SOURCES.txt
+-rw-r--r--   0 artemij    (501) staff       (20)       64 2024-05-31 16:10:50.000000 predictions_sepsis-1.0.0/predictions_sepsis.egg-info/requires.txt
+-rw-r--r--   0 artemij    (501) staff       (20)       19 2024-05-31 16:10:50.000000 predictions_sepsis-1.0.0/predictions_sepsis.egg-info/top_level.txt
+-rw-r--r--   0 artemij    (501) staff       (20)        1 2024-05-31 16:10:50.000000 predictions_sepsis-1.0.0/predictions_sepsis.egg-info/dependency_links.txt
+-rw-r--r--   0 artemij    (501) staff       (20)     3877 2024-05-31 16:03:00.000000 predictions_sepsis-1.0.0/README.md
+-rw-r--r--   0 artemij    (501) staff       (20)      858 2024-05-31 16:10:26.000000 predictions_sepsis-1.0.0/setup.py
+-rw-r--r--   0 artemij    (501) staff       (20)       38 2024-05-31 16:10:50.000000 predictions_sepsis-1.0.0/setup.cfg
+drwxr-xr-x   0 artemij    (501) staff       (20)        0 2024-05-31 16:10:50.000000 predictions_sepsis-1.0.0/predictions_sepsis/
+-rw-r--r--   0 artemij    (501) staff       (20)     1774 2024-05-31 14:27:13.000000 predictions_sepsis-1.0.0/predictions_sepsis/choose.py
+-rw-r--r--   0 artemij    (501) staff       (20)     7265 2024-05-31 12:49:20.000000 predictions_sepsis-1.0.0/predictions_sepsis/merge_diagnoses_and_ssir_with_blood.py
+-rw-r--r--   0 artemij    (501) staff       (20)     3694 2024-05-31 13:59:27.000000 predictions_sepsis-1.0.0/predictions_sepsis/balance_on_patients.py
+-rw-r--r--   0 artemij    (501) staff       (20)     4197 2024-05-31 15:34:40.000000 predictions_sepsis-1.0.0/predictions_sepsis/train_model.py
+-rw-r--r--   0 artemij    (501) staff       (20)     4617 2024-05-31 12:49:20.000000 predictions_sepsis-1.0.0/predictions_sepsis/combine_diagnoses_and_ssir.py
+-rw-r--r--   0 artemij    (501) staff       (20)     8414 2024-05-31 12:51:29.000000 predictions_sepsis-1.0.0/predictions_sepsis/transformers.py
+-rw-r--r--   0 artemij    (501) staff       (20)     2822 2024-05-31 13:27:53.000000 predictions_sepsis-1.0.0/predictions_sepsis/get_ssir.py
+-rw-r--r--   0 artemij    (501) staff       (20)     1464 2024-05-31 15:05:36.000000 predictions_sepsis-1.0.0/predictions_sepsis/fill_values.py
+-rw-r--r--   0 artemij    (501) staff       (20)     1870 2024-05-31 12:49:20.000000 predictions_sepsis-1.0.0/predictions_sepsis/get_disease_info.py
+-rw-r--r--   0 artemij    (501) staff       (20)     1690 2024-05-31 12:54:42.000000 predictions_sepsis-1.0.0/predictions_sepsis/get_diagnoses.py
+-rw-r--r--   0 artemij    (501) staff       (20)      129 2024-05-30 17:47:12.000000 predictions_sepsis-1.0.0/predictions_sepsis/__init__.py
+-rw-r--r--   0 artemij    (501) staff       (20)     1026 2024-05-31 14:16:45.000000 predictions_sepsis-1.0.0/predictions_sepsis/compress.py
```

### Comparing `predictions_sepsis-0.0.6/setup.py` & `predictions_sepsis-1.0.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,25 +2,27 @@
 
 def readme():
     with open('README.md', 'r') as f:
         return f.read()
 
 setup(
     name='predictions_sepsis',
-    version='0.0.6',
+    version='1.0.0',
     author='@Margo78, @akp1n',
     author_email='timtimk30@yandex.ru',
     description='Module for sepsis predictions',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://github.com/sslavian812/sepsis-predictions.git',
     packages=find_packages(),
     install_requires=[
         'requests>=2.25.1',
-        'pandas>=1.0.0'
+        'pandas>=1.0.0',
+        'numpy>=1.0.0',
+        'scikit-learn>=1.0.0'
     ],
     classifiers=[
         'Programming Language :: Python :: 3.11',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent'
     ],
     keywords='sepsis, predictions, python',
```

### Comparing `predictions_sepsis-0.0.6/predictions_sepsis/get_diagnoses.py` & `predictions_sepsis-1.0.0/predictions_sepsis/get_diagnoses.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,13 +17,12 @@
         None: Writes the aggregated diagnosis file to output_file_csv.
     """
     df_d_diagnos = pd.read_csv(all_diagnoses_csv)
     df_diagnos = pd.read_csv(patient_diagnoses_csv)
     diagnos_results = df_diagnos[df_diagnos[diagnoses_code_column].isin(df_d_diagnos[diagnoses_code_column])]
     diagnos_results = diagnos_results.merge(df_d_diagnos[[diagnoses_code_column, title_column]],
                                             on=diagnoses_code_column)
-    print(diagnos_results.columns)
     diagnos_results = diagnos_results[[subject_id_column, title_column]]
     diagnos_results.to_csv(output_file_csv, index=False)
 
 
 get_diagnoses()
```

