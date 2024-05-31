# Comparing `tmp/leap_data_management_utils-0.0.8.tar.gz` & `tmp/leap_data_management_utils-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leap_data_management_utils-0.0.8.tar", last modified: Mon May  6 21:29:17 2024, max compression
+gzip compressed data, was "leap_data_management_utils-0.0.9.tar", last modified: Wed May  8 00:47:31 2024, max compression
```

## Comparing `leap_data_management_utils-0.0.8.tar` & `leap_data_management_utils-0.0.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:29:17.335491 leap_data_management_utils-0.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:29:17.327491 leap_data_management_utils-0.0.8/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-06 21:29:04.000000 leap_data_management_utils-0.0.8/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:29:17.327491 leap_data_management_utils-0.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-06 21:29:04.000000 leap_data_management_utils-0.0.8/.github/workflows/catalog-ci.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-06 21:29:04.000000 leap_data_management_utils-0.0.8/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-06 21:29:04.000000 leap_data_management_utils-0.0.8/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-05-06 21:29:04.000000 leap_data_management_utils-0.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-06 21:29:04.000000 leap_data_management_utils-0.0.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-06 21:29:04.000000 leap_data_management_utils-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-05-06 21:29:17.335491 leap_data_management_utils-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-06 21:29:04.000000 leap_data_management_utils-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:29:17.331491 leap_data_management_utils-0.0.8/ci/
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-06 21:29:04.000000 leap_data_management_utils-0.0.8/ci/environment.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:29:17.331491 leap_data_management_utils-0.0.8/leap_data_management_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-06 21:29:04.000000 leap_data_management_utils-0.0.8/leap_data_management_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-06 21:29:17.000000 leap_data_management_utils-0.0.8/leap_data_management_utils/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-06 21:29:04.000000 leap_data_management_utils-0.0.8/leap_data_management_utils/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-05-06 21:29:04.000000 leap_data_management_utils-0.0.8/leap_data_management_utils/cmip_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-05-06 21:29:04.000000 leap_data_management_utils-0.0.8/leap_data_management_utils/cmip_testing.py
--rw-r--r--   0 runner    (1001) docker     (127)     9115 2024-05-06 21:29:04.000000 leap_data_management_utils-0.0.8/leap_data_management_utils/cmip_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     9450 2024-05-06 21:29:04.000000 leap_data_management_utils-0.0.8/leap_data_management_utils/data_management_transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:29:17.331491 leap_data_management_utils-0.0.8/leap_data_management_utils/testing_notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)    25238 2024-05-06 21:29:04.000000 leap_data_management_utils-0.0.8/leap_data_management_utils/testing_notebooks/testing_cmip_bigquery.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:29:17.331491 leap_data_management_utils-0.0.8/leap_data_management_utils/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-06 21:29:04.000000 leap_data_management_utils-0.0.8/leap_data_management_utils/tests/test_cmip_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-06 21:29:04.000000 leap_data_management_utils-0.0.8/leap_data_management_utils/tests/test_data_management_transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:29:17.331491 leap_data_management_utils-0.0.8/leap_data_management_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-05-06 21:29:17.000000 leap_data_management_utils-0.0.8/leap_data_management_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-06 21:29:17.000000 leap_data_management_utils-0.0.8/leap_data_management_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 21:29:17.000000 leap_data_management_utils-0.0.8/leap_data_management_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-06 21:29:17.000000 leap_data_management_utils-0.0.8/leap_data_management_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-06 21:29:17.000000 leap_data_management_utils-0.0.8/leap_data_management_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-06 21:29:17.000000 leap_data_management_utils-0.0.8/leap_data_management_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-05-06 21:29:04.000000 leap_data_management_utils-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 21:29:17.335491 leap_data_management_utils-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:47:31.378398 leap_data_management_utils-0.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:47:31.374398 leap_data_management_utils-0.0.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-08 00:47:18.000000 leap_data_management_utils-0.0.9/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:47:31.374398 leap_data_management_utils-0.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-08 00:47:18.000000 leap_data_management_utils-0.0.9/.github/workflows/catalog-ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-08 00:47:18.000000 leap_data_management_utils-0.0.9/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-08 00:47:18.000000 leap_data_management_utils-0.0.9/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-05-08 00:47:18.000000 leap_data_management_utils-0.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-08 00:47:18.000000 leap_data_management_utils-0.0.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-08 00:47:18.000000 leap_data_management_utils-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-05-08 00:47:31.378398 leap_data_management_utils-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-08 00:47:18.000000 leap_data_management_utils-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:47:31.374398 leap_data_management_utils-0.0.9/ci/
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-08 00:47:18.000000 leap_data_management_utils-0.0.9/ci/environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:47:31.374398 leap_data_management_utils-0.0.9/leap_data_management_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-08 00:47:18.000000 leap_data_management_utils-0.0.9/leap_data_management_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-08 00:47:31.000000 leap_data_management_utils-0.0.9/leap_data_management_utils/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-08 00:47:18.000000 leap_data_management_utils-0.0.9/leap_data_management_utils/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-05-08 00:47:18.000000 leap_data_management_utils-0.0.9/leap_data_management_utils/cmip_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-05-08 00:47:18.000000 leap_data_management_utils-0.0.9/leap_data_management_utils/cmip_testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9475 2024-05-08 00:47:18.000000 leap_data_management_utils-0.0.9/leap_data_management_utils/cmip_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9450 2024-05-08 00:47:18.000000 leap_data_management_utils-0.0.9/leap_data_management_utils/data_management_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:47:31.374398 leap_data_management_utils-0.0.9/leap_data_management_utils/testing_notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)    25238 2024-05-08 00:47:18.000000 leap_data_management_utils-0.0.9/leap_data_management_utils/testing_notebooks/testing_cmip_bigquery.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:47:31.374398 leap_data_management_utils-0.0.9/leap_data_management_utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-08 00:47:18.000000 leap_data_management_utils-0.0.9/leap_data_management_utils/tests/test_cmip_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-08 00:47:18.000000 leap_data_management_utils-0.0.9/leap_data_management_utils/tests/test_data_management_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:47:31.374398 leap_data_management_utils-0.0.9/leap_data_management_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-05-08 00:47:31.000000 leap_data_management_utils-0.0.9/leap_data_management_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-08 00:47:31.000000 leap_data_management_utils-0.0.9/leap_data_management_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 00:47:31.000000 leap_data_management_utils-0.0.9/leap_data_management_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-08 00:47:31.000000 leap_data_management_utils-0.0.9/leap_data_management_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-08 00:47:31.000000 leap_data_management_utils-0.0.9/leap_data_management_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-08 00:47:31.000000 leap_data_management_utils-0.0.9/leap_data_management_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-05-08 00:47:18.000000 leap_data_management_utils-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 00:47:31.378398 leap_data_management_utils-0.0.9/setup.cfg
```

### Comparing `leap_data_management_utils-0.0.8/.github/workflows/catalog-ci.yaml` & `leap_data_management_utils-0.0.9/.github/workflows/catalog-ci.yaml`

 * *Files identical despite different names*

### Comparing `leap_data_management_utils-0.0.8/.github/workflows/ci.yaml` & `leap_data_management_utils-0.0.9/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `leap_data_management_utils-0.0.8/.github/workflows/release.yaml` & `leap_data_management_utils-0.0.9/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `leap_data_management_utils-0.0.8/.gitignore` & `leap_data_management_utils-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `leap_data_management_utils-0.0.8/.pre-commit-config.yaml` & `leap_data_management_utils-0.0.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `leap_data_management_utils-0.0.8/LICENSE` & `leap_data_management_utils-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `leap_data_management_utils-0.0.8/PKG-INFO` & `leap_data_management_utils-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leap-data-management-utils
-Version: 0.0.8
+Version: 0.0.9
 Summary: LEAP / pangeo-forge-recipes extension library for logging data in Google Big Query
 Author-email: LEAP <leap@columbia.edu>
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
@@ -17,14 +17,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cftime
 Requires-Dist: ruamel.yaml
 Requires-Dist: xarray
 Requires-Dist: zarr
 Provides-Extra: pangeo-forge
+Requires-Dist: tqdm; extra == "pangeo-forge"
 Requires-Dist: db_dtypes; extra == "pangeo-forge"
 Requires-Dist: google-api-core; extra == "pangeo-forge"
 Requires-Dist: google-cloud-bigquery; extra == "pangeo-forge"
 Requires-Dist: pandas; extra == "pangeo-forge"
 Requires-Dist: pangeo-forge-esgf; extra == "pangeo-forge"
 Requires-Dist: pangeo-forge-recipes; extra == "pangeo-forge"
 Requires-Dist: apache-beam; extra == "pangeo-forge"
```

### Comparing `leap_data_management_utils-0.0.8/leap_data_management_utils/catalog.py` & `leap_data_management_utils-0.0.9/leap_data_management_utils/catalog.py`

 * *Files identical despite different names*

### Comparing `leap_data_management_utils-0.0.8/leap_data_management_utils/cmip_catalog.py` & `leap_data_management_utils-0.0.9/leap_data_management_utils/cmip_catalog.py`

 * *Files identical despite different names*

### Comparing `leap_data_management_utils-0.0.8/leap_data_management_utils/cmip_testing.py` & `leap_data_management_utils-0.0.9/leap_data_management_utils/cmip_testing.py`

 * *Files identical despite different names*

### Comparing `leap_data_management_utils-0.0.8/leap_data_management_utils/cmip_transforms.py` & `leap_data_management_utils-0.0.9/leap_data_management_utils/cmip_transforms.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import datetime
 from dataclasses import dataclass
 
 import apache_beam as beam
 import zarr
 from google.cloud import bigquery
 from pangeo_forge_recipes.transforms import Indexed, T
+from tqdm.auto import tqdm
 
 from leap_data_management_utils.cmip_testing import test_all
 from leap_data_management_utils.data_management_transforms import BQInterface
 
 
 @dataclass
 class IIDEntry:
@@ -132,42 +133,48 @@
         ).result()  # TODO: `.result()` is waiting for the query. Should I do this here?
         return IIDResult(results, iid)
 
     def iid_exists(self, iid: str) -> bool:
         """Check if iid exists in the table"""
         return self._get_iid_results(iid).exists
 
-    def iid_list_exists(self, iids: list[str]) -> list[str]:
+    def _iid_list_exists_batch(self, iids: list[str]) -> list[str]:
         """More efficient way to check if a list of iids exists in the table
         Passes the entire list to a single SQL query.
         Returns a list of iids that exist in the table
-        Only supports list up to 10k elements. If you want to check more, you should
-        work in batches:
-        ```
-        iids = df['instance_id'].tolist()
-        iids_in_bq = []
-        batchsize = 10000
-        iid_batches = [iids[i : i + batchsize] for i in range(0, len(iids), batchsize)]
-        for iids_batch in tqdm(iid_batches):
-            iids_in_bq_batch = bq.iid_list_exists(iids_batch)
-            iids_in_bq.extend(iids_in_bq_batch)
         ```
         """
-        assert len(iids) <= 10000
+        if len(iids) > 10000:
+            raise ValueError('List of iids is too long. Please work in batches.')
 
         # source: https://stackoverflow.com/questions/26441928/how-do-i-check-if-multiple-values-exists-in-database
         query = f"""
         SELECT instance_id, store
         FROM {self.table_id}
         WHERE instance_id IN ({",".join([f"'{iid}'" for iid in iids])})
         """
         results = self._get_query_job(query).result()
         # this is a full row iterator, for now just return the iids
         return list(set([r['instance_id'] for r in results]))
 
+    def iid_list_exists(self, iids: list[str]) -> list[str]:
+        """More efficient way to check if a list of iids exists in the table
+        Passes the entire list in batches into SQL querys for maximum efficiency.
+        Returns a list of iids that exist in the table
+        """
+
+        # make batches of the input, since bq cannot handle more than 10k elements here
+        iids_in_bq = []
+        batchsize = 10000
+        iid_batches = [iids[i : i + batchsize] for i in range(0, len(iids), batchsize)]
+        for iids_batch in tqdm(iid_batches):
+            iids_in_bq_batch = self._iid_list_exists_batch(iids_batch)
+            iids_in_bq.extend(iids_in_bq_batch)
+        return iids_in_bq
+
 
 # ----------------------------------------------------------------------------------------------
 # apache Beam stages
 # ----------------------------------------------------------------------------------------------
 
 
 @dataclass
```

### Comparing `leap_data_management_utils-0.0.8/leap_data_management_utils/data_management_transforms.py` & `leap_data_management_utils-0.0.9/leap_data_management_utils/data_management_transforms.py`

 * *Files identical despite different names*

### Comparing `leap_data_management_utils-0.0.8/leap_data_management_utils/testing_notebooks/testing_cmip_bigquery.ipynb` & `leap_data_management_utils-0.0.9/leap_data_management_utils/testing_notebooks/testing_cmip_bigquery.ipynb`

 * *Files identical despite different names*

### Comparing `leap_data_management_utils-0.0.8/leap_data_management_utils/tests/test_cmip_transforms.py` & `leap_data_management_utils-0.0.9/leap_data_management_utils/tests/test_cmip_transforms.py`

 * *Files identical despite different names*

### Comparing `leap_data_management_utils-0.0.8/leap_data_management_utils/tests/test_data_management_transforms.py` & `leap_data_management_utils-0.0.9/leap_data_management_utils/tests/test_data_management_transforms.py`

 * *Files identical despite different names*

### Comparing `leap_data_management_utils-0.0.8/leap_data_management_utils.egg-info/PKG-INFO` & `leap_data_management_utils-0.0.9/leap_data_management_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leap-data-management-utils
-Version: 0.0.8
+Version: 0.0.9
 Summary: LEAP / pangeo-forge-recipes extension library for logging data in Google Big Query
 Author-email: LEAP <leap@columbia.edu>
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
@@ -17,14 +17,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cftime
 Requires-Dist: ruamel.yaml
 Requires-Dist: xarray
 Requires-Dist: zarr
 Provides-Extra: pangeo-forge
+Requires-Dist: tqdm; extra == "pangeo-forge"
 Requires-Dist: db_dtypes; extra == "pangeo-forge"
 Requires-Dist: google-api-core; extra == "pangeo-forge"
 Requires-Dist: google-cloud-bigquery; extra == "pangeo-forge"
 Requires-Dist: pandas; extra == "pangeo-forge"
 Requires-Dist: pangeo-forge-esgf; extra == "pangeo-forge"
 Requires-Dist: pangeo-forge-recipes; extra == "pangeo-forge"
 Requires-Dist: apache-beam; extra == "pangeo-forge"
```

### Comparing `leap_data_management_utils-0.0.8/leap_data_management_utils.egg-info/SOURCES.txt` & `leap_data_management_utils-0.0.9/leap_data_management_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `leap_data_management_utils-0.0.8/pyproject.toml` & `leap_data_management_utils-0.0.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     "xarray",
     "zarr",
 ]
 
 [project.optional-dependencies]
 
 pangeo-forge=[
+    "tqdm",
     "db_dtypes",
     "google-api-core",
     "google-cloud-bigquery",
     "pandas",
     "pangeo-forge-esgf",
     "pangeo-forge-recipes",
     "apache-beam",
```

