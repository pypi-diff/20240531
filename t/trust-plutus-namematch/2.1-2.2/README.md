# Comparing `tmp/trust_plutus_namematch-2.1.tar.gz` & `tmp/trust_plutus_namematch-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trust_plutus_namematch-2.1.tar", max compression
+gzip compressed data, was "trust_plutus_namematch-2.2.tar", max compression
```

## Comparing `trust_plutus_namematch-2.1.tar` & `trust_plutus_namematch-2.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    35821 2024-03-20 09:06:41.708383 trust_plutus_namematch-2.1/LICENSE
--rw-r--r--   0        0        0      491 2024-05-31 07:04:01.042649 trust_plutus_namematch-2.1/pyproject.toml
--rw-r--r--   0        0        0      435 2024-05-10 06:55:13.290252 trust_plutus_namematch-2.1/README.md
--rw-r--r--   0        0        0        0 2024-05-09 10:32:15.022349 trust_plutus_namematch-2.1/trust_plutus_namematch/__init__.py
--rw-r--r--   0        0        0     2437 2024-05-31 07:03:22.406509 trust_plutus_namematch-2.1/trust_plutus_namematch/match.py
--rw-r--r--   0        0        0        0 2024-02-12 07:49:10.008013 trust_plutus_namematch-2.1/trust_plutus_namematch/utils/__init__.py
--rw-r--r--   0        0        0      425 2024-05-09 10:37:36.797518 trust_plutus_namematch-2.1/trust_plutus_namematch/utils/logs.py
--rw-r--r--   0        0        0     1049 1970-01-01 00:00:00.000000 trust_plutus_namematch-2.1/PKG-INFO
+-rw-r--r--   0        0        0    35821 2024-03-20 09:06:41.708383 trust_plutus_namematch-2.2/LICENSE
+-rw-r--r--   0        0        0      491 2024-05-31 07:06:35.809304 trust_plutus_namematch-2.2/pyproject.toml
+-rw-r--r--   0        0        0      435 2024-05-10 06:55:13.290252 trust_plutus_namematch-2.2/README.md
+-rw-r--r--   0        0        0        0 2024-05-09 10:32:15.022349 trust_plutus_namematch-2.2/trust_plutus_namematch/__init__.py
+-rw-r--r--   0        0        0     2443 2024-05-31 07:06:23.558883 trust_plutus_namematch-2.2/trust_plutus_namematch/match.py
+-rw-r--r--   0        0        0        0 2024-02-12 07:49:10.008013 trust_plutus_namematch-2.2/trust_plutus_namematch/utils/__init__.py
+-rw-r--r--   0        0        0      425 2024-05-09 10:37:36.797518 trust_plutus_namematch-2.2/trust_plutus_namematch/utils/logs.py
+-rw-r--r--   0        0        0     1049 1970-01-01 00:00:00.000000 trust_plutus_namematch-2.2/PKG-INFO
```

### Comparing `trust_plutus_namematch-2.1/LICENSE` & `trust_plutus_namematch-2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `trust_plutus_namematch-2.1/trust_plutus_namematch/match.py` & `trust_plutus_namematch-2.2/trust_plutus_namematch/match.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
             if ("dir" in input_cg) or ("direct" in input_cg):
                 if ("dir" in string_cg) or ("direct" in string_cg):
                     return string
             elif ("dir" not in input_cg) or ("direct" not in input_cg):
                 if ("dir" not in string_cg) or ("direct" not in string_cg):
                     return string
                 
-    def string_proc(x):
+    def string_proc(self, x):
         temp_1 = x.lower().replace("-"," ")
         return temp_1
 
     def process_funds(self, i, milesSheet_list):
         temp_ = [self.miles_process(i, x) for x in milesSheet_list]
         milesList = [x for x in temp_ if x is not None]
         result = rf.process.extract(i, milesList, scorer=fuzz.ratio, limit=1, processor=self.string_proc)
```

### Comparing `trust_plutus_namematch-2.1/PKG-INFO` & `trust_plutus_namematch-2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trust-plutus-namematch
-Version: 2.1
+Version: 2.2
 Summary: Name match for fund names from ICRA and MILES
 License: OSI Approved :: GNU General Public License v3 (GPLv3)
 Author: Rolf Lobo
 Requires-Python: >=3.10,<3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

