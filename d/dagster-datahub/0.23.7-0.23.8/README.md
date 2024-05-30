# Comparing `tmp/dagster-datahub-0.23.7.tar.gz` & `tmp/dagster-datahub-0.23.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-datahub-0.23.7.tar", last modified: Thu May 23 21:42:56 2024, max compression
+gzip compressed data, was "dagster-datahub-0.23.8.tar", last modified: Thu May 30 23:21:52 2024, max compression
```

## Comparing `dagster-datahub-0.23.7.tar` & `dagster-datahub-0.23.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 21:42:56.293243 dagster-datahub-0.23.7/
--rw-r--r--   0 root         (0) root         (0)    11349 2024-05-23 21:36:17.000000 dagster-datahub-0.23.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)      214 2024-05-23 21:36:17.000000 dagster-datahub-0.23.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      740 2024-05-23 21:42:56.293243 dagster-datahub-0.23.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      131 2024-05-23 21:36:17.000000 dagster-datahub-0.23.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 21:42:56.293243 dagster-datahub-0.23.7/dagster_datahub/
--rw-r--r--   0 root         (0) root         (0)      492 2024-05-23 21:36:17.000000 dagster-datahub-0.23.7/dagster_datahub/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 21:36:17.000000 dagster-datahub-0.23.7/dagster_datahub/py.typed
--rw-r--r--   0 root         (0) root         (0)     4225 2024-05-23 21:36:17.000000 dagster-datahub-0.23.7/dagster_datahub/resources.py
--rw-r--r--   0 root         (0) root         (0)       23 2024-05-23 21:36:17.000000 dagster-datahub-0.23.7/dagster_datahub/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 21:42:56.293243 dagster-datahub-0.23.7/dagster_datahub.egg-info/
--rw-r--r--   0 root         (0) root         (0)      740 2024-05-23 21:42:56.000000 dagster-datahub-0.23.7/dagster_datahub.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      389 2024-05-23 21:42:56.000000 dagster-datahub-0.23.7/dagster_datahub.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 21:42:56.000000 dagster-datahub-0.23.7/dagster_datahub.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 21:42:56.000000 dagster-datahub-0.23.7/dagster_datahub.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      100 2024-05-23 21:42:56.000000 dagster-datahub-0.23.7/dagster_datahub.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2024-05-23 21:42:56.000000 dagster-datahub-0.23.7/dagster_datahub.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      162 2024-05-23 21:42:56.293243 dagster-datahub-0.23.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1543 2024-05-23 21:36:17.000000 dagster-datahub-0.23.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:21:52.702782 dagster-datahub-0.23.8/
+-rw-r--r--   0 root         (0) root         (0)    11349 2024-05-30 23:14:09.000000 dagster-datahub-0.23.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      214 2024-05-30 23:14:09.000000 dagster-datahub-0.23.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      740 2024-05-30 23:21:52.702782 dagster-datahub-0.23.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      131 2024-05-30 23:14:09.000000 dagster-datahub-0.23.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:21:52.702782 dagster-datahub-0.23.8/dagster_datahub/
+-rw-r--r--   0 root         (0) root         (0)      492 2024-05-30 23:14:09.000000 dagster-datahub-0.23.8/dagster_datahub/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-30 23:14:09.000000 dagster-datahub-0.23.8/dagster_datahub/py.typed
+-rw-r--r--   0 root         (0) root         (0)     4225 2024-05-30 23:14:09.000000 dagster-datahub-0.23.8/dagster_datahub/resources.py
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-30 23:14:09.000000 dagster-datahub-0.23.8/dagster_datahub/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:21:52.702782 dagster-datahub-0.23.8/dagster_datahub.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      740 2024-05-30 23:21:52.000000 dagster-datahub-0.23.8/dagster_datahub.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      389 2024-05-30 23:21:52.000000 dagster-datahub-0.23.8/dagster_datahub.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 23:21:52.000000 dagster-datahub-0.23.8/dagster_datahub.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 23:21:52.000000 dagster-datahub-0.23.8/dagster_datahub.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      100 2024-05-30 23:21:52.000000 dagster-datahub-0.23.8/dagster_datahub.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-05-30 23:21:52.000000 dagster-datahub-0.23.8/dagster_datahub.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      162 2024-05-30 23:21:52.702782 dagster-datahub-0.23.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1543 2024-05-30 23:14:09.000000 dagster-datahub-0.23.8/setup.py
```

### Comparing `dagster-datahub-0.23.7/LICENSE` & `dagster-datahub-0.23.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-datahub-0.23.7/PKG-INFO` & `dagster-datahub-0.23.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-datahub
-Version: 0.23.7
+Version: 0.23.8
 Summary: Package for Datahub-specific Dagster framework solid and resource components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-datahub
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-datahub-0.23.7/dagster_datahub/resources.py` & `dagster-datahub-0.23.8/dagster_datahub/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-datahub-0.23.7/dagster_datahub.egg-info/PKG-INFO` & `dagster-datahub-0.23.8/dagster_datahub.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-datahub
-Version: 0.23.7
+Version: 0.23.8
 Summary: Package for Datahub-specific Dagster framework solid and resource components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-datahub
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-datahub-0.23.7/setup.py` & `dagster-datahub-0.23.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_datahub_tests*"]),
     include_package_data=True,
     python_requires=">=3.8,<3.13",
     install_requires=[
         "acryl-datahub[datahub-rest, datahub-kafka]",
-        "dagster==1.7.7",
+        "dagster==1.7.8",
         "packaging",
         "requests",
         "pydantic>=1.10.0,<2.0.0",
     ],
     extras_require={},
     zip_safe=False,
 )
```

