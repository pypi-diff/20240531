# Comparing `tmp/dagster-fivetran-0.23.7.tar.gz` & `tmp/dagster-fivetran-0.23.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-fivetran-0.23.7.tar", last modified: Thu May 23 20:59:23 2024, max compression
+gzip compressed data, was "dagster-fivetran-0.23.8.tar", last modified: Thu May 30 22:28:06 2024, max compression
```

## Comparing `dagster-fivetran-0.23.7.tar` & `dagster-fivetran-0.23.8.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:59:23.795054 dagster-fivetran-0.23.7/
--rw-r--r--   0 root         (0) root         (0)    11349 2024-05-23 20:50:32.000000 dagster-fivetran-0.23.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)       68 2024-05-23 20:50:32.000000 dagster-fivetran-0.23.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      735 2024-05-23 20:59:23.795054 dagster-fivetran-0.23.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      134 2024-05-23 20:50:32.000000 dagster-fivetran-0.23.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:59:23.795054 dagster-fivetran-0.23.7/dagster_fivetran/
--rw-r--r--   0 root         (0) root         (0)      854 2024-05-23 20:50:32.000000 dagster-fivetran-0.23.7/dagster_fivetran/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22841 2024-05-23 20:50:32.000000 dagster-fivetran-0.23.7/dagster_fivetran/asset_defs.py
--rw-r--r--   0 root         (0) root         (0)      426 2024-05-23 20:50:32.000000 dagster-fivetran-0.23.7/dagster_fivetran/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:59:23.795054 dagster-fivetran-0.23.7/dagster_fivetran/managed/
--rw-r--r--   0 root         (0) root         (0)      212 2024-05-23 20:50:32.000000 dagster-fivetran-0.23.7/dagster_fivetran/managed/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14615 2024-05-23 20:50:32.000000 dagster-fivetran-0.23.7/dagster_fivetran/managed/reconciliation.py
--rw-r--r--   0 root         (0) root         (0)     3628 2024-05-23 20:50:32.000000 dagster-fivetran-0.23.7/dagster_fivetran/managed/types.py
--rw-r--r--   0 root         (0) root         (0)     7139 2024-05-23 20:50:32.000000 dagster-fivetran-0.23.7/dagster_fivetran/ops.py
--rw-r--r--   0 root         (0) root         (0)        8 2024-05-23 20:50:32.000000 dagster-fivetran-0.23.7/dagster_fivetran/py.typed
--rw-r--r--   0 root         (0) root         (0)    18339 2024-05-23 20:50:32.000000 dagster-fivetran-0.23.7/dagster_fivetran/resources.py
--rw-r--r--   0 root         (0) root         (0)      936 2024-05-23 20:50:32.000000 dagster-fivetran-0.23.7/dagster_fivetran/types.py
--rw-r--r--   0 root         (0) root         (0)     2996 2024-05-23 20:50:32.000000 dagster-fivetran-0.23.7/dagster_fivetran/utils.py
--rw-r--r--   0 root         (0) root         (0)       23 2024-05-23 20:50:32.000000 dagster-fivetran-0.23.7/dagster_fivetran/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:59:23.795054 dagster-fivetran-0.23.7/dagster_fivetran.egg-info/
--rw-r--r--   0 root         (0) root         (0)      735 2024-05-23 20:59:23.000000 dagster-fivetran-0.23.7/dagster_fivetran.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      687 2024-05-23 20:59:23.000000 dagster-fivetran-0.23.7/dagster_fivetran.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 20:59:23.000000 dagster-fivetran-0.23.7/dagster_fivetran.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2024-05-23 20:59:23.000000 dagster-fivetran-0.23.7/dagster_fivetran.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 20:59:23.000000 dagster-fivetran-0.23.7/dagster_fivetran.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       59 2024-05-23 20:59:23.000000 dagster-fivetran-0.23.7/dagster_fivetran.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-05-23 20:59:23.000000 dagster-fivetran-0.23.7/dagster_fivetran.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      163 2024-05-23 20:59:23.799054 dagster-fivetran-0.23.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1534 2024-05-23 20:50:32.000000 dagster-fivetran-0.23.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:28:06.250568 dagster-fivetran-0.23.8/
+-rw-r--r--   0 root         (0) root         (0)    11349 2024-05-30 22:22:14.000000 dagster-fivetran-0.23.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       68 2024-05-30 22:22:14.000000 dagster-fivetran-0.23.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      735 2024-05-30 22:28:06.250568 dagster-fivetran-0.23.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      134 2024-05-30 22:22:14.000000 dagster-fivetran-0.23.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:28:06.246568 dagster-fivetran-0.23.8/dagster_fivetran/
+-rw-r--r--   0 root         (0) root         (0)      854 2024-05-30 22:22:14.000000 dagster-fivetran-0.23.8/dagster_fivetran/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22841 2024-05-30 22:22:14.000000 dagster-fivetran-0.23.8/dagster_fivetran/asset_defs.py
+-rw-r--r--   0 root         (0) root         (0)      426 2024-05-30 22:22:14.000000 dagster-fivetran-0.23.8/dagster_fivetran/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:28:06.250568 dagster-fivetran-0.23.8/dagster_fivetran/managed/
+-rw-r--r--   0 root         (0) root         (0)      212 2024-05-30 22:22:14.000000 dagster-fivetran-0.23.8/dagster_fivetran/managed/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14615 2024-05-30 22:22:14.000000 dagster-fivetran-0.23.8/dagster_fivetran/managed/reconciliation.py
+-rw-r--r--   0 root         (0) root         (0)     3628 2024-05-30 22:22:14.000000 dagster-fivetran-0.23.8/dagster_fivetran/managed/types.py
+-rw-r--r--   0 root         (0) root         (0)     7139 2024-05-30 22:22:14.000000 dagster-fivetran-0.23.8/dagster_fivetran/ops.py
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-30 22:22:14.000000 dagster-fivetran-0.23.8/dagster_fivetran/py.typed
+-rw-r--r--   0 root         (0) root         (0)    18339 2024-05-30 22:22:14.000000 dagster-fivetran-0.23.8/dagster_fivetran/resources.py
+-rw-r--r--   0 root         (0) root         (0)      936 2024-05-30 22:22:14.000000 dagster-fivetran-0.23.8/dagster_fivetran/types.py
+-rw-r--r--   0 root         (0) root         (0)     2996 2024-05-30 22:22:14.000000 dagster-fivetran-0.23.8/dagster_fivetran/utils.py
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-30 22:22:14.000000 dagster-fivetran-0.23.8/dagster_fivetran/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:28:06.250568 dagster-fivetran-0.23.8/dagster_fivetran.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      735 2024-05-30 22:28:06.000000 dagster-fivetran-0.23.8/dagster_fivetran.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      687 2024-05-30 22:28:06.000000 dagster-fivetran-0.23.8/dagster_fivetran.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 22:28:06.000000 dagster-fivetran-0.23.8/dagster_fivetran.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2024-05-30 22:28:06.000000 dagster-fivetran-0.23.8/dagster_fivetran.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 22:28:06.000000 dagster-fivetran-0.23.8/dagster_fivetran.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       59 2024-05-30 22:28:06.000000 dagster-fivetran-0.23.8/dagster_fivetran.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-05-30 22:28:06.000000 dagster-fivetran-0.23.8/dagster_fivetran.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      163 2024-05-30 22:28:06.250568 dagster-fivetran-0.23.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1534 2024-05-30 22:22:14.000000 dagster-fivetran-0.23.8/setup.py
```

### Comparing `dagster-fivetran-0.23.7/LICENSE` & `dagster-fivetran-0.23.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-fivetran-0.23.7/PKG-INFO` & `dagster-fivetran-0.23.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-fivetran
-Version: 0.23.7
+Version: 0.23.8
 Summary: Package for integrating Fivetran with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-fivetran
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-fivetran-0.23.7/dagster_fivetran/__init__.py` & `dagster-fivetran-0.23.8/dagster_fivetran/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-fivetran-0.23.7/dagster_fivetran/asset_defs.py` & `dagster-fivetran-0.23.8/dagster_fivetran/asset_defs.py`

 * *Files identical despite different names*

### Comparing `dagster-fivetran-0.23.7/dagster_fivetran/managed/reconciliation.py` & `dagster-fivetran-0.23.8/dagster_fivetran/managed/reconciliation.py`

 * *Files identical despite different names*

### Comparing `dagster-fivetran-0.23.7/dagster_fivetran/managed/types.py` & `dagster-fivetran-0.23.8/dagster_fivetran/managed/types.py`

 * *Files identical despite different names*

### Comparing `dagster-fivetran-0.23.7/dagster_fivetran/ops.py` & `dagster-fivetran-0.23.8/dagster_fivetran/ops.py`

 * *Files identical despite different names*

### Comparing `dagster-fivetran-0.23.7/dagster_fivetran/resources.py` & `dagster-fivetran-0.23.8/dagster_fivetran/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-fivetran-0.23.7/dagster_fivetran/types.py` & `dagster-fivetran-0.23.8/dagster_fivetran/types.py`

 * *Files identical despite different names*

### Comparing `dagster-fivetran-0.23.7/dagster_fivetran/utils.py` & `dagster-fivetran-0.23.8/dagster_fivetran/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-fivetran-0.23.7/dagster_fivetran.egg-info/PKG-INFO` & `dagster-fivetran-0.23.8/dagster_fivetran.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-fivetran
-Version: 0.23.7
+Version: 0.23.8
 Summary: Package for integrating Fivetran with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-fivetran
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-fivetran-0.23.7/dagster_fivetran.egg-info/SOURCES.txt` & `dagster-fivetran-0.23.8/dagster_fivetran.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-fivetran-0.23.7/setup.py` & `dagster-fivetran-0.23.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,20 +30,20 @@
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_fivetran_tests*"]),
     python_requires=">=3.8,<3.13",
-    install_requires=["dagster==1.7.7"],
+    install_requires=["dagster==1.7.8"],
     zip_safe=False,
     entry_points={
         "console_scripts": [
             "dagster-fivetran = dagster_fivetran.cli:main",
         ]
     },
     extras_require={
         "managed": [
-            "dagster-managed-elements==0.23.7",
+            "dagster-managed-elements==0.23.8",
         ],
     },
 )
```

