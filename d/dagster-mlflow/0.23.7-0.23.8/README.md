# Comparing `tmp/dagster-mlflow-0.23.7.tar.gz` & `tmp/dagster-mlflow-0.23.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-mlflow-0.23.7.tar", last modified: Thu May 23 20:55:31 2024, max compression
+gzip compressed data, was "dagster-mlflow-0.23.8.tar", last modified: Thu May 30 22:27:23 2024, max compression
```

## Comparing `dagster-mlflow-0.23.7.tar` & `dagster-mlflow-0.23.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:55:31.373041 dagster-mlflow-0.23.7/
--rw-r--r--   0 root         (0) root         (0)    11349 2024-05-23 20:50:32.000000 dagster-mlflow-0.23.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)       66 2024-05-23 20:50:32.000000 dagster-mlflow-0.23.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      607 2024-05-23 20:55:31.373041 dagster-mlflow-0.23.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      128 2024-05-23 20:50:32.000000 dagster-mlflow-0.23.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:55:31.369041 dagster-mlflow-0.23.7/dagster_mlflow/
--rw-r--r--   0 root         (0) root         (0)      303 2024-05-23 20:50:32.000000 dagster-mlflow-0.23.7/dagster_mlflow/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1197 2024-05-23 20:50:32.000000 dagster-mlflow-0.23.7/dagster_mlflow/hooks.py
--rw-r--r--   0 root         (0) root         (0)        8 2024-05-23 20:50:32.000000 dagster-mlflow-0.23.7/dagster_mlflow/py.typed
--rw-r--r--   0 root         (0) root         (0)    10924 2024-05-23 20:50:32.000000 dagster-mlflow-0.23.7/dagster_mlflow/resources.py
--rw-r--r--   0 root         (0) root         (0)       23 2024-05-23 20:50:32.000000 dagster-mlflow-0.23.7/dagster_mlflow/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:55:31.369041 dagster-mlflow-0.23.7/dagster_mlflow.egg-info/
--rw-r--r--   0 root         (0) root         (0)      607 2024-05-23 20:55:31.000000 dagster-mlflow-0.23.7/dagster_mlflow.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      403 2024-05-23 20:55:31.000000 dagster-mlflow-0.23.7/dagster_mlflow.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 20:55:31.000000 dagster-mlflow-0.23.7/dagster_mlflow.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 20:55:31.000000 dagster-mlflow-0.23.7/dagster_mlflow.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       29 2024-05-23 20:55:31.000000 dagster-mlflow-0.23.7/dagster_mlflow.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-05-23 20:55:31.000000 dagster-mlflow-0.23.7/dagster_mlflow.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      161 2024-05-23 20:55:31.377040 dagster-mlflow-0.23.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1225 2024-05-23 20:50:32.000000 dagster-mlflow-0.23.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:27:23.162946 dagster-mlflow-0.23.8/
+-rw-r--r--   0 root         (0) root         (0)    11349 2024-05-30 22:22:14.000000 dagster-mlflow-0.23.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       66 2024-05-30 22:22:14.000000 dagster-mlflow-0.23.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      607 2024-05-30 22:27:23.162946 dagster-mlflow-0.23.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      128 2024-05-30 22:22:14.000000 dagster-mlflow-0.23.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:27:23.162946 dagster-mlflow-0.23.8/dagster_mlflow/
+-rw-r--r--   0 root         (0) root         (0)      303 2024-05-30 22:22:14.000000 dagster-mlflow-0.23.8/dagster_mlflow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1197 2024-05-30 22:22:14.000000 dagster-mlflow-0.23.8/dagster_mlflow/hooks.py
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-30 22:22:14.000000 dagster-mlflow-0.23.8/dagster_mlflow/py.typed
+-rw-r--r--   0 root         (0) root         (0)    10924 2024-05-30 22:22:14.000000 dagster-mlflow-0.23.8/dagster_mlflow/resources.py
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-30 22:22:14.000000 dagster-mlflow-0.23.8/dagster_mlflow/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:27:23.162946 dagster-mlflow-0.23.8/dagster_mlflow.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      607 2024-05-30 22:27:23.000000 dagster-mlflow-0.23.8/dagster_mlflow.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      403 2024-05-30 22:27:23.000000 dagster-mlflow-0.23.8/dagster_mlflow.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 22:27:23.000000 dagster-mlflow-0.23.8/dagster_mlflow.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 22:27:23.000000 dagster-mlflow-0.23.8/dagster_mlflow.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-30 22:27:23.000000 dagster-mlflow-0.23.8/dagster_mlflow.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-05-30 22:27:23.000000 dagster-mlflow-0.23.8/dagster_mlflow.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      161 2024-05-30 22:27:23.166947 dagster-mlflow-0.23.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1225 2024-05-30 22:22:14.000000 dagster-mlflow-0.23.8/setup.py
```

### Comparing `dagster-mlflow-0.23.7/LICENSE` & `dagster-mlflow-0.23.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-mlflow-0.23.7/PKG-INFO` & `dagster-mlflow-0.23.8/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-mlflow
-Version: 0.23.7
+Version: 0.23.8
 Summary: Package for mlflow Dagster framework components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-mlflow
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-mlflow-0.23.7/dagster_mlflow/hooks.py` & `dagster-mlflow-0.23.8/dagster_mlflow/hooks.py`

 * *Files identical despite different names*

### Comparing `dagster-mlflow-0.23.7/dagster_mlflow/resources.py` & `dagster-mlflow-0.23.8/dagster_mlflow/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-mlflow-0.23.7/dagster_mlflow.egg-info/PKG-INFO` & `dagster-mlflow-0.23.8/dagster_mlflow.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-mlflow
-Version: 0.23.7
+Version: 0.23.8
 Summary: Package for mlflow Dagster framework components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-mlflow
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-mlflow-0.23.7/setup.py` & `dagster-mlflow-0.23.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,10 +28,10 @@
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_mlflow_tests*"]),
     python_requires=">=3.8,<3.13",
-    install_requires=["dagster==1.7.7", "mlflow", "pandas"],
+    install_requires=["dagster==1.7.8", "mlflow", "pandas"],
     zip_safe=False,
 )
```

