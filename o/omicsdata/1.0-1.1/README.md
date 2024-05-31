# Comparing `tmp/omicsdata-1.0.tar.gz` & `tmp/omicsdata-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omicsdata-1.0.tar", last modified: Mon Jul 10 22:12:33 2023, max compression
+gzip compressed data, was "omicsdata-1.1.tar", last modified: Fri May 31 20:47:01 2024, max compression
```

## Comparing `omicsdata-1.0.tar` & `omicsdata-1.1.tar`

### file list

```diff
@@ -1,35 +1,47 @@
-drwxr-xr-x   0 ethank     (501) staff       (20)        0 2023-07-10 22:12:33.674869 omicsdata-1.0/
--rw-r--r--   0 ethank     (501) staff       (20)     1064 2023-06-28 14:55:04.000000 omicsdata-1.0/LICENSE
--rw-r--r--   0 ethank     (501) staff       (20)      548 2023-07-10 22:12:33.674758 omicsdata-1.0/PKG-INFO
--rw-r--r--   0 ethank     (501) staff       (20)       33 2023-07-04 21:25:16.000000 omicsdata-1.0/README.md
--rw-r--r--   0 ethank     (501) staff       (20)      581 2023-07-10 22:12:19.000000 omicsdata-1.0/pyproject.toml
--rw-r--r--   0 ethank     (501) staff       (20)       38 2023-07-10 22:12:33.674901 omicsdata-1.0/setup.cfg
-drwxr-xr-x   0 ethank     (501) staff       (20)        0 2023-07-10 22:12:33.668926 omicsdata-1.0/src/
-drwxr-xr-x   0 ethank     (501) staff       (20)        0 2023-07-10 22:12:33.669889 omicsdata-1.0/src/omicsdata/
--rw-r--r--   0 ethank     (501) staff       (20)        0 2023-06-28 14:55:04.000000 omicsdata-1.0/src/omicsdata/__init__.py
-drwxr-xr-x   0 ethank     (501) staff       (20)        0 2023-07-10 22:12:33.670443 omicsdata-1.0/src/omicsdata/npz/
--rw-r--r--   0 ethank     (501) staff       (20)        0 2023-07-04 21:32:15.000000 omicsdata-1.0/src/omicsdata/npz/__init__.py
--rw-r--r--   0 ethank     (501) staff       (20)     4952 2023-06-28 17:29:10.000000 omicsdata-1.0/src/omicsdata/npz/archive.py
-drwxr-xr-x   0 ethank     (501) staff       (20)        0 2023-07-10 22:12:33.672016 omicsdata-1.0/src/omicsdata/ssm/
--rw-r--r--   0 ethank     (501) staff       (20)        0 2023-06-28 14:55:04.000000 omicsdata-1.0/src/omicsdata/ssm/__init__.py
--rw-r--r--   0 ethank     (501) staff       (20)      918 2023-06-28 18:10:15.000000 omicsdata-1.0/src/omicsdata/ssm/columns.py
--rw-r--r--   0 ethank     (501) staff       (20)     1345 2023-06-28 18:10:10.000000 omicsdata-1.0/src/omicsdata/ssm/common.py
--rw-r--r--   0 ethank     (501) staff       (20)      628 2023-06-28 18:10:22.000000 omicsdata-1.0/src/omicsdata/ssm/constants.py
-drwxr-xr-x   0 ethank     (501) staff       (20)        0 2023-07-10 22:12:33.673675 omicsdata-1.0/src/omicsdata/ssm/convert/
--rw-r--r--   0 ethank     (501) staff       (20)     6953 2023-06-28 18:17:26.000000 omicsdata-1.0/src/omicsdata/ssm/convert/ssm_base_converter.py
--rw-r--r--   0 ethank     (501) staff       (20)     2659 2023-06-28 14:55:04.000000 omicsdata-1.0/src/omicsdata/ssm/convert/ssm_to_fastclone.py
--rw-r--r--   0 ethank     (501) staff       (20)     2931 2023-06-28 14:55:04.000000 omicsdata-1.0/src/omicsdata/ssm/convert/ssm_to_mobster_tsv.py
--rw-r--r--   0 ethank     (501) staff       (20)     2758 2023-06-28 14:55:04.000000 omicsdata-1.0/src/omicsdata/ssm/convert/ssm_to_pcvi_tsv.py
--rw-r--r--   0 ethank     (501) staff       (20)     3712 2023-06-28 16:21:44.000000 omicsdata-1.0/src/omicsdata/ssm/convert/ssm_to_scc_tsv.py
--rw-r--r--   0 ethank     (501) staff       (20)     2419 2023-06-28 16:21:28.000000 omicsdata-1.0/src/omicsdata/ssm/convert/ssm_to_viber.py
--rw-r--r--   0 ethank     (501) staff       (20)     6788 2023-06-28 18:32:54.000000 omicsdata-1.0/src/omicsdata/ssm/convert/vcf_to_ssm.py
--rw-r--r--   0 ethank     (501) staff       (20)     6549 2023-06-28 18:10:57.000000 omicsdata-1.0/src/omicsdata/ssm/parse.py
--rw-r--r--   0 ethank     (501) staff       (20)     7398 2023-07-04 21:35:27.000000 omicsdata-1.0/src/omicsdata/ssm/supervariants.py
-drwxr-xr-x   0 ethank     (501) staff       (20)        0 2023-07-10 22:12:33.674465 omicsdata-1.0/src/omicsdata/tree/
--rw-r--r--   0 ethank     (501) staff       (20)     1645 2023-07-05 16:15:15.000000 omicsdata-1.0/src/omicsdata/tree/adj.py
--rw-r--r--   0 ethank     (501) staff       (20)      583 2023-06-28 14:55:04.000000 omicsdata-1.0/src/omicsdata/tree/parents.py
-drwxr-xr-x   0 ethank     (501) staff       (20)        0 2023-07-10 22:12:33.670260 omicsdata-1.0/src/omicsdata.egg-info/
--rw-r--r--   0 ethank     (501) staff       (20)      548 2023-07-10 22:12:33.000000 omicsdata-1.0/src/omicsdata.egg-info/PKG-INFO
--rw-r--r--   0 ethank     (501) staff       (20)      814 2023-07-10 22:12:33.000000 omicsdata-1.0/src/omicsdata.egg-info/SOURCES.txt
--rw-r--r--   0 ethank     (501) staff       (20)        1 2023-07-10 22:12:33.000000 omicsdata-1.0/src/omicsdata.egg-info/dependency_links.txt
--rw-r--r--   0 ethank     (501) staff       (20)       10 2023-07-10 22:12:33.000000 omicsdata-1.0/src/omicsdata.egg-info/top_level.txt
+drwxr-xr-x   0 ethank     (501) staff       (20)        0 2024-05-31 20:47:01.551123 omicsdata-1.1/
+-rw-r--r--   0 ethank     (501) staff       (20)     1064 2023-06-28 14:55:04.000000 omicsdata-1.1/LICENSE
+-rw-r--r--   0 ethank     (501) staff       (20)     1100 2024-05-31 20:47:01.550951 omicsdata-1.1/PKG-INFO
+-rw-r--r--   0 ethank     (501) staff       (20)      584 2023-07-11 22:14:55.000000 omicsdata-1.1/README.md
+-rw-r--r--   0 ethank     (501) staff       (20)      583 2024-05-31 15:14:41.000000 omicsdata-1.1/pyproject.toml
+-rw-r--r--   0 ethank     (501) staff       (20)       38 2024-05-31 20:47:01.551167 omicsdata-1.1/setup.cfg
+drwxr-xr-x   0 ethank     (501) staff       (20)        0 2024-05-31 20:47:01.543040 omicsdata-1.1/src/
+drwxr-xr-x   0 ethank     (501) staff       (20)        0 2024-05-31 20:47:01.544279 omicsdata-1.1/src/omicsdata/
+-rw-r--r--   0 ethank     (501) staff       (20)        0 2023-06-28 14:55:04.000000 omicsdata-1.1/src/omicsdata/__init__.py
+drwxr-xr-x   0 ethank     (501) staff       (20)        0 2024-05-31 20:47:01.544825 omicsdata-1.1/src/omicsdata/cn/
+-rw-r--r--   0 ethank     (501) staff       (20)        0 2023-12-20 16:09:45.000000 omicsdata-1.1/src/omicsdata/cn/estimate.py
+drwxr-xr-x   0 ethank     (501) staff       (20)        0 2024-05-31 20:47:01.544907 omicsdata-1.1/src/omicsdata/csv/
+-rw-r--r--   0 ethank     (501) staff       (20)        0 2023-12-21 15:38:04.000000 omicsdata-1.1/src/omicsdata/csv/parse.py
+drwxr-xr-x   0 ethank     (501) staff       (20)        0 2024-05-31 20:47:01.545078 omicsdata-1.1/src/omicsdata/npz/
+-rw-r--r--   0 ethank     (501) staff       (20)        0 2023-07-04 21:32:15.000000 omicsdata-1.1/src/omicsdata/npz/__init__.py
+-rw-r--r--   0 ethank     (501) staff       (20)     4952 2023-06-28 17:29:10.000000 omicsdata-1.1/src/omicsdata/npz/archive.py
+drwxr-xr-x   0 ethank     (501) staff       (20)        0 2024-05-31 20:47:01.547180 omicsdata-1.1/src/omicsdata/ssm/
+-rw-r--r--   0 ethank     (501) staff       (20)        0 2023-06-28 14:55:04.000000 omicsdata-1.1/src/omicsdata/ssm/__init__.py
+drwxr-xr-x   0 ethank     (501) staff       (20)        0 2024-05-31 20:47:01.547669 omicsdata-1.1/src/omicsdata/ssm/_convert/
+-rw-r--r--   0 ethank     (501) staff       (20)        0 2024-05-31 15:29:09.000000 omicsdata-1.1/src/omicsdata/ssm/_convert/__init__.py
+drwxr-xr-x   0 ethank     (501) staff       (20)        0 2024-05-31 20:47:01.549553 omicsdata-1.1/src/omicsdata/ssm/_convert/convert_extra/
+-rw-r--r--   0 ethank     (501) staff       (20)     6953 2023-06-28 18:17:26.000000 omicsdata-1.1/src/omicsdata/ssm/_convert/convert_extra/ssm_base_converter.py
+-rw-r--r--   0 ethank     (501) staff       (20)     2659 2023-06-28 14:55:04.000000 omicsdata-1.1/src/omicsdata/ssm/_convert/convert_extra/ssm_to_fastclone.py
+-rw-r--r--   0 ethank     (501) staff       (20)     2931 2023-06-28 14:55:04.000000 omicsdata-1.1/src/omicsdata/ssm/_convert/convert_extra/ssm_to_mobster_tsv.py
+-rw-r--r--   0 ethank     (501) staff       (20)     2758 2024-03-15 14:30:29.000000 omicsdata-1.1/src/omicsdata/ssm/_convert/convert_extra/ssm_to_pcvi_tsv.py
+-rw-r--r--   0 ethank     (501) staff       (20)     3712 2023-06-28 16:21:44.000000 omicsdata-1.1/src/omicsdata/ssm/_convert/convert_extra/ssm_to_scc_tsv.py
+-rw-r--r--   0 ethank     (501) staff       (20)     2419 2024-05-31 14:45:42.000000 omicsdata-1.1/src/omicsdata/ssm/_convert/convert_extra/ssm_to_viber_tsv.py
+-rw-r--r--   0 ethank     (501) staff       (20)     6788 2023-06-28 18:32:54.000000 omicsdata-1.1/src/omicsdata/ssm/_convert/convert_extra/vcf_to_ssm.py
+-rw-r--r--   0 ethank     (501) staff       (20)     3420 2024-05-31 14:59:22.000000 omicsdata-1.1/src/omicsdata/ssm/_convert/ssm_to_pyclone.py
+-rw-r--r--   0 ethank     (501) staff       (20)     5364 2024-05-31 15:50:54.000000 omicsdata-1.1/src/omicsdata/ssm/_convert/ssm_to_viber.py
+-rw-r--r--   0 ethank     (501) staff       (20)      918 2023-06-28 18:10:15.000000 omicsdata-1.1/src/omicsdata/ssm/columns.py
+-rw-r--r--   0 ethank     (501) staff       (20)     1345 2023-06-28 18:10:10.000000 omicsdata-1.1/src/omicsdata/ssm/common.py
+-rw-r--r--   0 ethank     (501) staff       (20)      628 2023-06-28 18:10:22.000000 omicsdata-1.1/src/omicsdata/ssm/constants.py
+-rw-r--r--   0 ethank     (501) staff       (20)     5444 2024-05-31 19:28:45.000000 omicsdata-1.1/src/omicsdata/ssm/convert.py
+-rw-r--r--   0 ethank     (501) staff       (20)     7916 2024-05-31 14:35:35.000000 omicsdata-1.1/src/omicsdata/ssm/parse.py
+-rw-r--r--   0 ethank     (501) staff       (20)     3420 2024-05-31 14:59:22.000000 omicsdata-1.1/src/omicsdata/ssm/ssm_to_pyclone.py
+-rw-r--r--   0 ethank     (501) staff       (20)     8255 2024-02-06 20:46:12.000000 omicsdata-1.1/src/omicsdata/ssm/supervariants.py
+drwxr-xr-x   0 ethank     (501) staff       (20)        0 2024-05-31 20:47:01.550576 omicsdata-1.1/src/omicsdata/tree/
+-rw-r--r--   0 ethank     (501) staff       (20)        0 2023-07-11 20:46:56.000000 omicsdata-1.1/src/omicsdata/tree/__init__.py
+-rw-r--r--   0 ethank     (501) staff       (20)     1645 2023-07-05 16:15:15.000000 omicsdata-1.1/src/omicsdata/tree/adj.py
+-rw-r--r--   0 ethank     (501) staff       (20)     1711 2024-05-31 14:37:46.000000 omicsdata-1.1/src/omicsdata/tree/newick.py
+-rw-r--r--   0 ethank     (501) staff       (20)      583 2023-06-28 14:55:04.000000 omicsdata-1.1/src/omicsdata/tree/parents.py
+drwxr-xr-x   0 ethank     (501) staff       (20)        0 2024-05-31 20:47:01.550745 omicsdata-1.1/src/omicsdata.egg-info/
+-rw-r--r--   0 ethank     (501) staff       (20)     1100 2024-05-31 20:47:01.000000 omicsdata-1.1/src/omicsdata.egg-info/PKG-INFO
+-rw-r--r--   0 ethank     (501) staff       (20)     1231 2024-05-31 20:47:01.000000 omicsdata-1.1/src/omicsdata.egg-info/SOURCES.txt
+-rw-r--r--   0 ethank     (501) staff       (20)        1 2024-05-31 20:47:01.000000 omicsdata-1.1/src/omicsdata.egg-info/dependency_links.txt
+-rw-r--r--   0 ethank     (501) staff       (20)       10 2024-05-31 20:47:01.000000 omicsdata-1.1/src/omicsdata.egg-info/top_level.txt
```

### Comparing `omicsdata-1.0/LICENSE` & `omicsdata-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `omicsdata-1.0/pyproject.toml` & `omicsdata-1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "omicsdata"
-version = "1.0"
+version = "1.01"
 authors = [{name="ethanumn", email="kulma009@umn.edu"}]
 description = "A package for manipulating omics data file types"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
```

### Comparing `omicsdata-1.0/src/omicsdata/npz/archive.py` & `omicsdata-1.1/src/omicsdata/npz/archive.py`

 * *Files identical despite different names*

### Comparing `omicsdata-1.0/src/omicsdata/ssm/columns.py` & `omicsdata-1.1/src/omicsdata/ssm/columns.py`

 * *Files identical despite different names*

### Comparing `omicsdata-1.0/src/omicsdata/ssm/common.py` & `omicsdata-1.1/src/omicsdata/ssm/common.py`

 * *Files identical despite different names*

### Comparing `omicsdata-1.0/src/omicsdata/ssm/constants.py` & `omicsdata-1.1/src/omicsdata/ssm/constants.py`

 * *Files identical despite different names*

### Comparing `omicsdata-1.0/src/omicsdata/ssm/convert/ssm_base_converter.py` & `omicsdata-1.1/src/omicsdata/ssm/_convert/convert_extra/ssm_base_converter.py`

 * *Files identical despite different names*

### Comparing `omicsdata-1.0/src/omicsdata/ssm/convert/ssm_to_fastclone.py` & `omicsdata-1.1/src/omicsdata/ssm/_convert/convert_extra/ssm_to_fastclone.py`

 * *Files identical despite different names*

### Comparing `omicsdata-1.0/src/omicsdata/ssm/convert/ssm_to_mobster_tsv.py` & `omicsdata-1.1/src/omicsdata/ssm/_convert/convert_extra/ssm_to_mobster_tsv.py`

 * *Files identical despite different names*

### Comparing `omicsdata-1.0/src/omicsdata/ssm/convert/ssm_to_pcvi_tsv.py` & `omicsdata-1.1/src/omicsdata/ssm/_convert/convert_extra/ssm_to_pcvi_tsv.py`

 * *Files identical despite different names*

### Comparing `omicsdata-1.0/src/omicsdata/ssm/convert/ssm_to_scc_tsv.py` & `omicsdata-1.1/src/omicsdata/ssm/_convert/convert_extra/ssm_to_scc_tsv.py`

 * *Files identical despite different names*

### Comparing `omicsdata-1.0/src/omicsdata/ssm/convert/ssm_to_viber.py` & `omicsdata-1.1/src/omicsdata/ssm/_convert/convert_extra/ssm_to_viber_tsv.py`

 * *Files identical despite different names*

### Comparing `omicsdata-1.0/src/omicsdata/ssm/convert/vcf_to_ssm.py` & `omicsdata-1.1/src/omicsdata/ssm/_convert/convert_extra/vcf_to_ssm.py`

 * *Files identical despite different names*

### Comparing `omicsdata-1.0/src/omicsdata/ssm/parse.py` & `omicsdata-1.1/src/omicsdata/ssm/parse.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,28 +7,32 @@
 
 import csv
 import json
 import numpy as np
 import numpy.ma as ma
 from .constants import Variants_Keys
 from .columns import SSM_Columns, PARAMS_Columns
+from .common import extract_vids
 
 
 def extract_nums(S, dtype):
     """Extracts and converts values from a comma delimited string"""
     return np.array(S.split(','), dtype=dtype)
 
-def load_ssm(ssm_fn):
+def load_ssm(ssm_fn, rescale_depth=False):
     """Loads a ssm file and extracts the read count and copy number data for each variant
     
     Parameters
     ----------
     ssm_fn : str
         The simple somatic mutation file
 
+    rescale_depth : bool, optional
+        A flag for whether or not to rescale the read depth for each variant using the average across each sample.
+
     Returns
     -------
     dictionary
         A dictionary where the keys are unique variant 'id' values and the value is a dictionary for each variant
         containing the variant's 'id' (unique identifier), 'name' (string identifier), 
         'var_reads' (array of variants reads for each sample),  'total_reads' (array of total reads for each sample)
         'omega_v' (array of variant read probabilities for each sample)
@@ -58,14 +62,28 @@
             T = ma.masked_equal(variant[Variants_Keys.TOTAL_READS], 0)
             variant[Variants_Keys.VAF] = np.array(variant[Variants_Keys.VAR_READS] / T)
 
             assert variant[Variants_Keys.ID] not in variants, \
                     "Cannot have variants with the same ID, variant %s occurs more than once" % variant[Variants_Keys.ID]
             variants[variant[Variants_Keys.ID]] = variant
 
+    # rescale read depth using average across samples
+    if rescale_depth:
+        vids = extract_vids(variants)
+        V = np.array([variants[vid][Variants_Keys.VAR_READS] for vid in vids])
+        T = np.array([variants[vid][Variants_Keys.TOTAL_READS] for vid in vids])
+        
+        VAFs = np.divide(V, T, where=T>0)
+        T = np.maximum(0,np.rint(np.tile(T.mean(axis=0), (T.shape[0],1))).astype(np.int32))
+        V = np.maximum(0,np.rint(VAFs*T).astype(np.int32))
+
+        for idx,vid in enumerate(vids):
+            variants[vid][Variants_Keys.VAR_READS] = V[idx,:]
+            variants[vid][Variants_Keys.TOTAL_READS] = T[idx,:]
+
     S = len(next(iter(variants.values()))[Variants_Keys.VAR_READS])
     for vid, V in variants.items():
         for K in (Variants_Keys.VAR_READS, Variants_Keys.TOTAL_READS, Variants_Keys.OMEGA_V):
             assert len(V[K]) == S, '%s for %s is of length %s, but %s expected' % (K, vid, len(V[K]), S)
 
     return variants
 
@@ -97,41 +115,40 @@
 
 def load_params(params_fn):
     """Loads a params file into a dictionary
     
     Parameters
     ----------
     params_fn : str
-        The parameters file (.params.json) to load into memory
+        The parameters file 
 
     Returns
     -------
     dictionary
         A dictionary where each of the key, value pairs are the same as those listed in the params_fn file
     """
     if params_fn is None:
         return {}
     with open(params_fn) as P:
         return json.load(P)
 
-def load_ssms_and_params(ssm_fn, params_fn, remove_garb=True):
+def load_ssms_and_params(ssm_fn, params_fn, remove_garb=True, rescale_depth=False):
     """Loads ssm file and params file
     
     Parameters
     ----------
     ssm_fn : str
         The simple somatic mutation file
-
     params_fn : str
-        The parameters file (.params.json) to load into memory
+        The parameters file 
 
     remove_garb : bool, optional
         A flag to remove garbage from the 'variants' dictionary (default is True)
     """
-    variants = load_ssm(ssmfn)
+    variants = load_ssm(ssmfn, rescale_depth)
     params = load_params(paramsfn)
     if PARAMS_Columns.GARBAGE not in params:
         params[PARAMS_Columns.GARBAGE] = []
     if remove_garb:
         variants = remove_garbage(variants, params[PARAMS_Columns.GARBAGE])
     return (variants, params)
 
@@ -158,14 +175,34 @@
             SSM_Columns.ID, 
             SSM_Columns.NAME, 
             SSM_Columns.VAR_READS, 
             SSM_Columns.TOTAL_READS, 
             SSM_Columns.VAR_READ_PROB
     )
     with open(ssm_fn, 'w') as f:
+        print(*keys, sep='\t', file=f)
         for variant in variants.values():
-            print(*keys, sep='\t', file=f)
             variant = dict(variant)
             for k in (Variants_Keys.VAR_READS, Variants_Keys.TOTAL_READS, Variants_Keys.OMEGA_V):
-                variant[k] = ','.join([str(val) for val in variant[K]])
+                variant[k] = ','.join([str(val) for val in variant[k]])
             variant[SSM_Columns.VAR_READ_PROB] = variant[Variants_Keys.OMEGA_V]
             print(*[variant[k] for k in keys], sep='\t', file=f)
+
+def write_params(params, params_fn):
+    """Writes a set of variants along with their associated read 
+    count and copy number information to an ssm file
+    
+    Parameters
+    ----------
+    params : dictionary 
+        A dictionary that contains a set of key/value pairs to write to a file as a JSON string
+
+    params_fn : str
+        The parameters file (.params.json) to write the params to
+
+    Returns
+    -------
+    None
+    """
+    json_params = json.dumps(params)
+    with open(params_fn, "w") as outfile:
+        outfile.write(json_params)
```

### Comparing `omicsdata-1.0/src/omicsdata/ssm/supervariants.py` & `omicsdata-1.1/src/omicsdata/ssm/supervariants.py`

 * *Files 22% similar despite different names*

```diff
@@ -59,27 +59,31 @@
     list
         A list of namedtuples for each variant in the variants input. Each value in the list is a 'Variant'
         namedtuple with the following keys: 'id', 'var_reads', 'ref_reads', 'total_reads','vaf','omega_v'
 
     """
     return [convert_variant_dict_to_tuple(variants[V]) for V in list(variants.keys())]
 
-def make_supervar(name, variants):
+def make_supervar(name, variants, fill_chr_pos=False):
     """Makes a supervariant given a list of variants
     
     Parameters
     ----------
     name : str
         A name/id value to give the supervariant
 
     variants : list
         A list of 'variant' dictionaries. Each variant dictionary contains the following keys:'id' (unique identifier), 'name' (string identifier), 
         'var_reads' (array of variants reads for each sample),  'total_reads' (array of total reads for each sample)
         'omega_v' (array of variant read probabilities for each sample)
 
+    fill_chr_pos : bool
+        A flag to fill the chromosome and position fields for each supervariant. This will only work 
+        if all variant names match the pattern '{chromosome}_{position}'
+
     Returns
     -------
     dictionary
         A dictionary that has summarizes the information in the list of variants inputted. The supervariant
         has the following (used) keys: 'id' (unique id for supervariant), 'name' (string name of supervariant), 'var_reads' (array of variants reads for each sample),  'total_reads' (array of total reads for each sample)
         'omega_v' (array of variant read probabilities for each sample)
     """
@@ -90,57 +94,70 @@
 
     # converts all supervariants to have an omega_v of 0.5
     _, S = N.shape
     N_hat = 2*N*omega_v
     V_hat = np.minimum(V, N_hat)
     omega_v_hat = 0.5 * np.ones(S)
 
+    chrom = None 
+    pos = None
+
+    # fill chromosome and position if given flag and the name field matches pattern
+    if fill_chr_pos:
+        if all([len(var[Variants_Keys.NAME].split("_")) == 2 for var in variants]):
+            chrom = np.array([var[Variants_Keys.NAME].split("_")[0] for var in variants])
+            pos = np.array([var[Variants_Keys.NAME].split("_")[1] for var in variants])
+
     supervariant = {
         Variants_Keys.ID:          name,
         Variants_Keys.NAME:        name,
-        Variants_Keys.CHROM:       None,
-        Variants_Keys.POS:         None,
+        Variants_Keys.CHROM:       chrom,
+        Variants_Keys.POS:         pos,
         Variants_Keys.OMEGA_V:     omega_v_hat,
         Variants_Keys.VAR_READS:   np.round(np.sum(V_hat, axis=0)).astype(np.int32),
         Variants_Keys.TOTAL_READS: np.round(np.sum(N_hat, axis=0)).astype(np.int32),
     }
     supervariant[Variants_Keys.REF_READS] = \
         supervariant[Variants_Keys.TOTAL_READS] - supervariant[Variants_Keys.VAR_READS]
     T = ma.masked_equal(supervariant[Variants_Keys.TOTAL_READS], 0)
     supervariant[Variants_Keys.VAF] = np.array(supervariant[Variants_Keys.VAR_READS] / T)
 
     return supervariant
 
-def clusters_to_supervars(clusters, variants):
+def clusters_to_supervars(clusters, variants, fill_chr_pos=False):
     """Converts clusters into supervariants
     
     Parameters
     ----------
     clusters: list
         A list of lists, where each sublist contains the 'id' values for the variants that are in that cluster
 
     variants : dictionary
         A dictionary where the keys are unique variant 'id' values and the value is a dictionary for each variant
         containing the variant's 'id' (unique identifier), 'name' (string identifier), 
         'var_reads' (array of variants reads for each sample),  'total_reads' (array of total reads for each sample)
         'omega_v' (array of variant read probabilities for each sample)
 
+    fill_chr_pos : bool
+        A flag to fill the chromosome and position fields for each supervariant. This will only work 
+        if all variant names match the pattern '{chromosome}_{position}'
+
     Returns
     -------
     dictionary
         A dictionary of supervariants, where the keys are the supervariant 'id' values and the values are a 
         dictionary containing the data for the supervariant
     """
     supervars = {}
 
     for cluster in clusters:
         assert len(cluster) > 0, "Cannot make a supervariant from an empty list"
         cluster_variants = [variants[vid] for vid in cluster]
         name = 'S%s' % (len(supervars) + 1)
-        supervars[name] = make_supervar(name, cluster_variants)
+        supervars[name] = make_supervar(name, cluster_variants, fill_chr_pos)
 
     return supervars
 
 def make_superclusters(supervars):
     """Generates a clustering where each supervariant is in its own cluster
     
     Parameters
@@ -178,9 +195,10 @@
         An ndarray where each row i = 1,...,n is the variant read probability for all m samples for supervariant i, and each column s = 1,...,m is the
         variant read probability for supervariant i in sample s.
     """
     svids = extract_vids(supervars)
     V = np.array([supervars[S][Variants_Keys.VAR_READS] for S in svids])
     R = np.array([supervars[S][Variants_Keys.REF_READS] for S in svids])
     omega_v = np.array([supervars[S][Variants_Keys.OMEGA_V] for S in svids])
+
     assert np.all(omega_v == 0.5), "supervariant omega_v is incorrect"
     return V, R, omega_v
```

### Comparing `omicsdata-1.0/src/omicsdata/tree/adj.py` & `omicsdata-1.1/src/omicsdata/tree/adj.py`

 * *Files identical despite different names*

### Comparing `omicsdata-1.0/src/omicsdata/tree/parents.py` & `omicsdata-1.1/src/omicsdata/tree/parents.py`

 * *Files identical despite different names*

