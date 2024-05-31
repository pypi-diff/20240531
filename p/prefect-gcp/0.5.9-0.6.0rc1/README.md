# Comparing `tmp/prefect_gcp-0.5.9.tar.gz` & `tmp/prefect_gcp-0.6.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefect_gcp-0.5.9.tar", last modified: Thu Apr 25 19:20:03 2024, max compression
+gzip compressed data, was "prefect_gcp-0.6.0rc1.tar", last modified: Fri May 31 20:49:41 2024, max compression
```

## Comparing `prefect_gcp-0.5.9.tar` & `prefect_gcp-0.6.0rc1.tar`

### file list

```diff
@@ -1,50 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:03.083167 prefect_gcp-0.5.9/
--rw-r--r--   0 runner    (1001) docker     (127)     3888 2024-04-25 19:20:03.083167 prefect_gcp-0.5.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-25 19:19:50.000000 prefect_gcp-0.5.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:03.075167 prefect_gcp-0.5.9/prefect_gcp/
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-25 19:19:50.000000 prefect_gcp-0.5.9/prefect_gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-25 19:20:02.000000 prefect_gcp-0.5.9/prefect_gcp/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    21574 2024-04-25 19:19:50.000000 prefect_gcp-0.5.9/prefect_gcp/aiplatform.py
--rw-r--r--   0 runner    (1001) docker     (127)    34350 2024-04-25 19:19:50.000000 prefect_gcp-0.5.9/prefect_gcp/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (127)    32157 2024-04-25 19:19:50.000000 prefect_gcp-0.5.9/prefect_gcp/cloud_run.py
--rw-r--r--   0 runner    (1001) docker     (127)    46401 2024-04-25 19:19:50.000000 prefect_gcp-0.5.9/prefect_gcp/cloud_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    17066 2024-04-25 19:19:50.000000 prefect_gcp-0.5.9/prefect_gcp/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:03.075167 prefect_gcp-0.5.9/prefect_gcp/deployments/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:19:50.000000 prefect_gcp-0.5.9/prefect_gcp/deployments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8914 2024-04-25 19:19:50.000000 prefect_gcp-0.5.9/prefect_gcp/deployments/steps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:03.075167 prefect_gcp-0.5.9/prefect_gcp/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:19:50.000000 prefect_gcp-0.5.9/prefect_gcp/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11694 2024-04-25 19:19:50.000000 prefect_gcp-0.5.9/prefect_gcp/models/cloud_run_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    13578 2024-04-25 19:19:50.000000 prefect_gcp-0.5.9/prefect_gcp/secret_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-25 19:19:50.000000 prefect_gcp-0.5.9/prefect_gcp/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:03.079167 prefect_gcp-0.5.9/prefect_gcp/workers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:19:50.000000 prefect_gcp-0.5.9/prefect_gcp/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31977 2024-04-25 19:19:50.000000 prefect_gcp-0.5.9/prefect_gcp/workers/cloud_run.py
--rw-r--r--   0 runner    (1001) docker     (127)    28870 2024-04-25 19:19:50.000000 prefect_gcp-0.5.9/prefect_gcp/workers/cloud_run_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    24134 2024-04-25 19:19:50.000000 prefect_gcp-0.5.9/prefect_gcp/workers/vertex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:03.079167 prefect_gcp-0.5.9/prefect_gcp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3888 2024-04-25 19:20:02.000000 prefect_gcp-0.5.9/prefect_gcp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-25 19:20:03.000000 prefect_gcp-0.5.9/prefect_gcp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 19:20:02.000000 prefect_gcp-0.5.9/prefect_gcp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-25 19:20:02.000000 prefect_gcp-0.5.9/prefect_gcp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-25 19:20:02.000000 prefect_gcp-0.5.9/prefect_gcp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-25 19:20:02.000000 prefect_gcp-0.5.9/prefect_gcp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-04-25 19:19:50.000000 prefect_gcp-0.5.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 19:20:03.083167 prefect_gcp-0.5.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:03.079167 prefect_gcp-0.5.9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-04-25 19:19:50.000000 prefect_gcp-0.5.9/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:03.079167 prefect_gcp-0.5.9/tests/projects/
--rw-r--r--   0 runner    (1001) docker     (127)     7646 2024-04-25 19:19:50.000000 prefect_gcp-0.5.9/tests/projects/test_steps.py
--rw-r--r--   0 runner    (1001) docker     (127)    12090 2024-04-25 19:19:50.000000 prefect_gcp-0.5.9/tests/test_aiplatform.py
--rw-r--r--   0 runner    (1001) docker     (127)     9871 2024-04-25 19:19:50.000000 prefect_gcp-0.5.9/tests/test_bigquery.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-25 19:19:50.000000 prefect_gcp-0.5.9/tests/test_block_standards.py
--rw-r--r--   0 runner    (1001) docker     (127)    34051 2024-04-25 19:19:50.000000 prefect_gcp-0.5.9/tests/test_cloud_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     5273 2024-04-25 19:19:50.000000 prefect_gcp-0.5.9/tests/test_cloud_run_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    26236 2024-04-25 19:19:50.000000 prefect_gcp-0.5.9/tests/test_cloud_run_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     6508 2024-04-25 19:19:50.000000 prefect_gcp-0.5.9/tests/test_cloud_run_worker_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    20315 2024-04-25 19:19:50.000000 prefect_gcp-0.5.9/tests/test_cloud_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     8319 2024-04-25 19:19:50.000000 prefect_gcp-0.5.9/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-25 19:19:50.000000 prefect_gcp-0.5.9/tests/test_deprecation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-04-25 19:19:50.000000 prefect_gcp-0.5.9/tests/test_secret_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-25 19:19:50.000000 prefect_gcp-0.5.9/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    10710 2024-04-25 19:19:50.000000 prefect_gcp-0.5.9/tests/test_vertex_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:41.317391 prefect_gcp-0.6.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-31 20:49:29.000000 prefect_gcp-0.6.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-31 20:49:29.000000 prefect_gcp-0.6.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-05-31 20:49:41.317391 prefect_gcp-0.6.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-31 20:49:29.000000 prefect_gcp-0.6.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:41.309392 prefect_gcp-0.6.0rc1/prefect_gcp/
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-31 20:49:29.000000 prefect_gcp-0.6.0rc1/prefect_gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-31 20:49:40.000000 prefect_gcp-0.6.0rc1/prefect_gcp/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34303 2024-05-31 20:49:29.000000 prefect_gcp-0.6.0rc1/prefect_gcp/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46646 2024-05-31 20:49:29.000000 prefect_gcp-0.6.0rc1/prefect_gcp/cloud_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20055 2024-05-31 20:49:29.000000 prefect_gcp-0.6.0rc1/prefect_gcp/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:41.309392 prefect_gcp-0.6.0rc1/prefect_gcp/deployments/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:29.000000 prefect_gcp-0.6.0rc1/prefect_gcp/deployments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8914 2024-05-31 20:49:29.000000 prefect_gcp-0.6.0rc1/prefect_gcp/deployments/steps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:41.309392 prefect_gcp-0.6.0rc1/prefect_gcp/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:29.000000 prefect_gcp-0.6.0rc1/prefect_gcp/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11843 2024-05-31 20:49:29.000000 prefect_gcp-0.6.0rc1/prefect_gcp/models/cloud_run_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13530 2024-05-31 20:49:29.000000 prefect_gcp-0.6.0rc1/prefect_gcp/secret_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6572 2024-05-31 20:49:29.000000 prefect_gcp-0.6.0rc1/prefect_gcp/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:41.313392 prefect_gcp-0.6.0rc1/prefect_gcp/workers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:29.000000 prefect_gcp-0.6.0rc1/prefect_gcp/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31997 2024-05-31 20:49:29.000000 prefect_gcp-0.6.0rc1/prefect_gcp/workers/cloud_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28795 2024-05-31 20:49:29.000000 prefect_gcp-0.6.0rc1/prefect_gcp/workers/cloud_run_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24505 2024-05-31 20:49:29.000000 prefect_gcp-0.6.0rc1/prefect_gcp/workers/vertex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:41.313392 prefect_gcp-0.6.0rc1/prefect_gcp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-05-31 20:49:40.000000 prefect_gcp-0.6.0rc1/prefect_gcp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-31 20:49:41.000000 prefect_gcp-0.6.0rc1/prefect_gcp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 20:49:40.000000 prefect_gcp-0.6.0rc1/prefect_gcp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-31 20:49:40.000000 prefect_gcp-0.6.0rc1/prefect_gcp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-31 20:49:40.000000 prefect_gcp-0.6.0rc1/prefect_gcp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-31 20:49:40.000000 prefect_gcp-0.6.0rc1/prefect_gcp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-05-31 20:49:29.000000 prefect_gcp-0.6.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 20:49:41.317391 prefect_gcp-0.6.0rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:41.313392 prefect_gcp-0.6.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-31 20:49:29.000000 prefect_gcp-0.6.0rc1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:41.313392 prefect_gcp-0.6.0rc1/tests/projects/
+-rw-r--r--   0 runner    (1001) docker     (127)     7646 2024-05-31 20:49:29.000000 prefect_gcp-0.6.0rc1/tests/projects/test_steps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9871 2024-05-31 20:49:29.000000 prefect_gcp-0.6.0rc1/tests/test_bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-31 20:49:29.000000 prefect_gcp-0.6.0rc1/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4554 2024-05-31 20:49:29.000000 prefect_gcp-0.6.0rc1/tests/test_cloud_run_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25738 2024-05-31 20:49:29.000000 prefect_gcp-0.6.0rc1/tests/test_cloud_run_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6508 2024-05-31 20:49:29.000000 prefect_gcp-0.6.0rc1/tests/test_cloud_run_worker_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19950 2024-05-31 20:49:29.000000 prefect_gcp-0.6.0rc1/tests/test_cloud_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10531 2024-05-31 20:49:29.000000 prefect_gcp-0.6.0rc1/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-05-31 20:49:29.000000 prefect_gcp-0.6.0rc1/tests/test_secret_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7019 2024-05-31 20:49:29.000000 prefect_gcp-0.6.0rc1/tests/test_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-31 20:49:29.000000 prefect_gcp-0.6.0rc1/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10567 2024-05-31 20:49:29.000000 prefect_gcp-0.6.0rc1/tests/test_vertex_worker.py
```

### Comparing `prefect_gcp-0.5.9/PKG-INFO` & `prefect_gcp-0.6.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 Metadata-Version: 2.1
 Name: prefect-gcp
-Version: 0.5.9
+Version: 0.6.0rc1
 Summary: Prefect integrations for interacting with Google Cloud Platform.
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-gcp
 Keywords: prefect
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: prefect>=2.16.4
+License-File: LICENSE
+Requires-Dist: prefect>=3.0.0rc1
 Requires-Dist: google-api-python-client>=2.20.0
 Requires-Dist: google-cloud-storage>=2.0.0
 Requires-Dist: tenacity>=8.0.0
 Requires-Dist: python-slugify>=8.0.0
+Requires-Dist: google-cloud-secret-manager
 Provides-Extra: cloud-storage
 Requires-Dist: google-cloud-storage; extra == "cloud-storage"
 Provides-Extra: bigquery
 Requires-Dist: google-cloud-bigquery; extra == "bigquery"
 Requires-Dist: google-cloud-bigquery-storage; extra == "bigquery"
 Provides-Extra: secret-manager
 Requires-Dist: google-cloud-secret-manager; extra == "secret-manager"
@@ -47,15 +48,14 @@
 Requires-Dist: google-cloud-secret-manager; extra == "dev"
 Requires-Dist: google-cloud-storage; extra == "dev"
 Requires-Dist: interrogate; extra == "dev"
 Requires-Dist: mkdocs-gen-files; extra == "dev"
 Requires-Dist: mkdocs-material; extra == "dev"
 Requires-Dist: mkdocs; extra == "dev"
 Requires-Dist: mkdocstrings[python]; extra == "dev"
-Requires-Dist: mock; python_version < "3.8" and extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pandas; extra == "dev"
 Requires-Dist: pillow; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pyarrow; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: pytest-xdist; extra == "dev"
```

#### html2text {}

```diff
@@ -1,46 +1,46 @@
-Metadata-Version: 2.1 Name: prefect-gcp Version: 0.5.9 Summary: Prefect
+Metadata-Version: 2.1 Name: prefect-gcp Version: 0.6.0rc1 Summary: Prefect
 integrations for interacting with Google Cloud Platform. Author-email: "Prefect
 Technologies, Inc."
 prefect.io> License: Apache License 2.0 Project-URL: Homepage, https://
 github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-gcp Keywords:
 prefect Classifier: Natural Language :: English Classifier: Intended Audience
 :: Developers Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
-Topic :: Software Development :: Libraries Requires-Python: >=3.8 Description-
-Content-Type: text/markdown Requires-Dist: prefect>=2.16.4 Requires-Dist:
-google-api-python-client>=2.20.0 Requires-Dist: google-cloud-storage>=2.0.0
-Requires-Dist: tenacity>=8.0.0 Requires-Dist: python-slugify>=8.0.0 Provides-
-Extra: cloud-storage Requires-Dist: google-cloud-storage; extra == "cloud-
-storage" Provides-Extra: bigquery Requires-Dist: google-cloud-bigquery; extra
-== "bigquery" Requires-Dist: google-cloud-bigquery-storage; extra == "bigquery"
-Provides-Extra: secret-manager Requires-Dist: google-cloud-secret-manager;
-extra == "secret-manager" Provides-Extra: aiplatform Requires-Dist: google-
-cloud-aiplatform; extra == "aiplatform" Provides-Extra: all-extras Requires-
-Dist: google-cloud-storage; extra == "all-extras" Requires-Dist: google-cloud-
-bigquery; extra == "all-extras" Requires-Dist: google-cloud-bigquery-storage;
-extra == "all-extras" Requires-Dist: google-cloud-secret-manager; extra ==
-"all-extras" Requires-Dist: google-cloud-aiplatform; extra == "all-extras"
-Provides-Extra: dev Requires-Dist: coverage; extra == "dev" Requires-Dist:
-google-cloud-aiplatform; extra == "dev" Requires-Dist: google-cloud-bigquery-
-storage; extra == "dev" Requires-Dist: google-cloud-bigquery; extra == "dev"
-Requires-Dist: google-cloud-secret-manager; extra == "dev" Requires-Dist:
-google-cloud-storage; extra == "dev" Requires-Dist: interrogate; extra == "dev"
-Requires-Dist: mkdocs-gen-files; extra == "dev" Requires-Dist: mkdocs-material;
-extra == "dev" Requires-Dist: mkdocs; extra == "dev" Requires-Dist:
-mkdocstrings[python]; extra == "dev" Requires-Dist: mock; python_version <
-"3.8" and extra == "dev" Requires-Dist: mypy; extra == "dev" Requires-Dist:
-pandas; extra == "dev" Requires-Dist: pillow; extra == "dev" Requires-Dist:
-pre-commit; extra == "dev" Requires-Dist: pyarrow; extra == "dev" Requires-
-Dist: pytest-asyncio; extra == "dev" Requires-Dist: pytest-xdist; extra ==
-"dev" Requires-Dist: pytest; extra == "dev" # `prefect-gcp`
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3.12 Classifier: Topic :: Software Development :: Libraries Requires-
+Python: >=3.9 Description-Content-Type: text/markdown License-File: LICENSE
+Requires-Dist: prefect>=3.0.0rc1 Requires-Dist: google-api-python-
+client>=2.20.0 Requires-Dist: google-cloud-storage>=2.0.0 Requires-Dist:
+tenacity>=8.0.0 Requires-Dist: python-slugify>=8.0.0 Requires-Dist: google-
+cloud-secret-manager Provides-Extra: cloud-storage Requires-Dist: google-cloud-
+storage; extra == "cloud-storage" Provides-Extra: bigquery Requires-Dist:
+google-cloud-bigquery; extra == "bigquery" Requires-Dist: google-cloud-
+bigquery-storage; extra == "bigquery" Provides-Extra: secret-manager Requires-
+Dist: google-cloud-secret-manager; extra == "secret-manager" Provides-Extra:
+aiplatform Requires-Dist: google-cloud-aiplatform; extra == "aiplatform"
+Provides-Extra: all-extras Requires-Dist: google-cloud-storage; extra == "all-
+extras" Requires-Dist: google-cloud-bigquery; extra == "all-extras" Requires-
+Dist: google-cloud-bigquery-storage; extra == "all-extras" Requires-Dist:
+google-cloud-secret-manager; extra == "all-extras" Requires-Dist: google-cloud-
+aiplatform; extra == "all-extras" Provides-Extra: dev Requires-Dist: coverage;
+extra == "dev" Requires-Dist: google-cloud-aiplatform; extra == "dev" Requires-
+Dist: google-cloud-bigquery-storage; extra == "dev" Requires-Dist: google-
+cloud-bigquery; extra == "dev" Requires-Dist: google-cloud-secret-manager;
+extra == "dev" Requires-Dist: google-cloud-storage; extra == "dev" Requires-
+Dist: interrogate; extra == "dev" Requires-Dist: mkdocs-gen-files; extra ==
+"dev" Requires-Dist: mkdocs-material; extra == "dev" Requires-Dist: mkdocs;
+extra == "dev" Requires-Dist: mkdocstrings[python]; extra == "dev" Requires-
+Dist: mypy; extra == "dev" Requires-Dist: pandas; extra == "dev" Requires-Dist:
+pillow; extra == "dev" Requires-Dist: pre-commit; extra == "dev" Requires-Dist:
+pyarrow; extra == "dev" Requires-Dist: pytest-asyncio; extra == "dev" Requires-
+Dist: pytest-xdist; extra == "dev" Requires-Dist: pytest; extra == "dev" #
+`prefect-gcp`
                 _[_P_y_P_I_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_d_m_/_p_r_e_f_e_c_t_-
                       _g_c_p_?_c_o_l_o_r_=_0_0_5_2_F_F_&_l_a_b_e_l_C_o_l_o_r_=_0_9_0_4_2_2_]
 `prefect-gcp` makes it easy to leverage the capabilities of Google Cloud
 Platform (GCP) in your flows, featuring support for Vertex AI, Cloud Run,
 BigQuery, Cloud Storage, and Secret Manager. Visit the full docs [here](https:/
 /PrefectHQ.github.io/prefect-gcp). ### Installation To start using `prefect-
 gcp`: ```bash pip install prefect-gcp ``` To install extras, see [here](https:/
```

### Comparing `prefect_gcp-0.5.9/README.md` & `prefect_gcp-0.6.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `prefect_gcp-0.5.9/prefect_gcp/__init__.py` & `prefect_gcp-0.6.0rc1/prefect_gcp/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 from prefect._internal.compatibility.deprecated import (
     register_renamed_module,
 )
 
 from . import _version
-from .aiplatform import VertexAICustomTrainingJob  # noqa
 from .bigquery import BigQueryWarehouse  # noqa
-from .cloud_run import CloudRunJob  # noqa
 from .cloud_storage import GcsBucket  # noqa
 from .credentials import GcpCredentials  # noqa
 from .secret_manager import GcpSecret  # noqa
 from .workers.vertex import VertexAIWorker  # noqa
 from .workers.cloud_run import CloudRunWorker  # noqa
 from .workers.cloud_run_v2 import CloudRunWorkerV2  # noqa
```

### Comparing `prefect_gcp-0.5.9/prefect_gcp/aiplatform.py` & `prefect_gcp-0.6.0rc1/prefect_gcp/workers/vertex.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,576 +1,657 @@
-"""
-DEPRECATION WARNING:
+"""<!-- # noqa -->
+
+Module containing the custom worker used for executing flow runs as Vertex AI Custom Jobs.
+
+Get started by creating a Cloud Run work pool:
 
-This module is deprecated as of March 2024 and will not be available after September 2024.
-It has been replaced by the Vertex AI worker, which offers enhanced functionality and better performance.
+```bash
+prefect work-pool create 'my-vertex-pool' --type vertex-ai
+```
 
-For upgrade instructions, see https://docs.prefect.io/latest/guides/upgrade-guide-agents-to-workers/.
+Then start a Cloud Run worker with the following command:
 
-Integrations with Google AI Platform.
+```bash
+prefect worker start --pool 'my-vertex-pool'
+```
 
-Examples:
-
-    Run a job using Vertex AI Custom Training:
-    ```python
-    from prefect_gcp.credentials import GcpCredentials
-    from prefect_gcp.aiplatform import VertexAICustomTrainingJob
-
-    gcp_credentials = GcpCredentials.load("BLOCK_NAME")
-    job = VertexAICustomTrainingJob(
-        region="us-east1",
-        image="us-docker.pkg.dev/cloudrun/container/job:latest",
-        gcp_credentials=gcp_credentials,
-    )
-    job.run()
-    ```
-
-    Run a job that runs the command `echo hello world` using Google Cloud Run Jobs:
-    ```python
-    from prefect_gcp.credentials import GcpCredentials
-    from prefect_gcp.aiplatform import VertexAICustomTrainingJob
-
-    gcp_credentials = GcpCredentials.load("BLOCK_NAME")
-    job = VertexAICustomTrainingJob(
-        command=["echo", "hello world"],
-        region="us-east1",
-        image="us-docker.pkg.dev/cloudrun/container/job:latest",
-        gcp_credentials=gcp_credentials,
-    )
-    job.run()
-    ```
-
-    Preview job specs:
-    ```python
-    from prefect_gcp.credentials import GcpCredentials
-    from prefect_gcp.aiplatform import VertexAICustomTrainingJob
-
-    gcp_credentials = GcpCredentials.load("BLOCK_NAME")
-    job = VertexAICustomTrainingJob(
-        command=["echo", "hello world"],
-        region="us-east1",
-        image="us-docker.pkg.dev/cloudrun/container/job:latest",
-        gcp_credentials=gcp_credentials,
-    )
-    job.preview()
-    ```
-"""  # noqa
+## Configuration
+Read more about configuring work pools
+[here](https://docs.prefect.io/latest/concepts/work-pools/#work-pool-overview).
+"""
 
+import asyncio
 import datetime
 import re
 import shlex
 import time
-from typing import Dict, List, Optional, Tuple
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple
 from uuid import uuid4
 
-from anyio.abc import TaskStatus
-from pydantic import VERSION as PYDANTIC_VERSION
+import anyio
+from pydantic import Field, field_validator
+from slugify import slugify
 
-from prefect._internal.compatibility.deprecated import deprecated_class
 from prefect.exceptions import InfrastructureNotFound
-from prefect.infrastructure import Infrastructure, InfrastructureResult
-from prefect.utilities.asyncutils import run_sync_in_worker_thread, sync_compatible
-
-if PYDANTIC_VERSION.startswith("2."):
-    from pydantic.v1 import Field
-else:
-    from pydantic import Field
-
-from slugify import slugify
-from typing_extensions import Literal
+from prefect.logging.loggers import PrefectLogAdapter
+from prefect.utilities.pydantic import JsonPatch
+from prefect.workers.base import (
+    BaseJobConfiguration,
+    BaseVariables,
+    BaseWorker,
+    BaseWorkerResult,
+)
+from prefect_gcp.credentials import GcpCredentials
 
 # to prevent "Failed to load collection" from surfacing
 # if google-cloud-aiplatform is not installed
 try:
     from google.api_core.client_options import ClientOptions
-    from google.cloud.aiplatform.gapic import JobServiceClient
+    from google.cloud.aiplatform.gapic import JobServiceAsyncClient
     from google.cloud.aiplatform_v1.types.custom_job import (
         ContainerSpec,
         CustomJob,
         CustomJobSpec,
         Scheduling,
         WorkerPoolSpec,
     )
     from google.cloud.aiplatform_v1.types.job_service import CancelCustomJobRequest
     from google.cloud.aiplatform_v1.types.job_state import JobState
     from google.cloud.aiplatform_v1.types.machine_resources import DiskSpec, MachineSpec
     from google.protobuf.duration_pb2 import Duration
-    from tenacity import retry, stop_after_attempt, wait_fixed, wait_random
+    from tenacity import AsyncRetrying, stop_after_attempt, wait_fixed, wait_random
 except ModuleNotFoundError:
     pass
 
-from prefect.blocks.core import BlockNotSavedError
-from prefect.workers.utilities import (
-    get_default_base_job_template_for_infrastructure_type,
-)
-from prefect_gcp.credentials import GcpCredentials
-
 _DISALLOWED_GCP_LABEL_CHARACTERS = re.compile(r"[^-a-zA-Z0-9_]+")
 
-
-class VertexAICustomTrainingJobResult(InfrastructureResult):
-    """Result from a Vertex AI custom training job."""
+if TYPE_CHECKING:
+    from prefect.client.schemas import FlowRun
+    from prefect.server.schemas.core import Flow
+    from prefect.server.schemas.responses import DeploymentResponse
 
 
-@deprecated_class(
-    start_date="Mar 2024",
-    help=(
-        "Use the Vertex AI worker instead."
-        " Refer to the upgrade guide for more information:"
-        " https://docs.prefect.io/latest/guides/upgrade-guide-agents-to-workers/."
-    ),
-)
-class VertexAICustomTrainingJob(Infrastructure):
+class VertexAIWorkerVariables(BaseVariables):
     """
-    Infrastructure block used to run Vertex AI custom training jobs.
-    """
-
-    _block_type_name = "Vertex AI Custom Training Job"
-    _block_type_slug = "vertex-ai-custom-training-job"
-    _logo_url = "https://cdn.sanity.io/images/3ugk85nk/production/10424e311932e31c477ac2b9ef3d53cefbaad708-250x250.png"  # noqa
-    _documentation_url = "https://prefecthq.github.io/prefect-gcp/aiplatform/#prefect_gcp.aiplatform.VertexAICustomTrainingJob"  # noqa: E501
+    Default variables for the Vertex AI worker.
 
-    type: Literal["vertex-ai-custom-training-job"] = Field(
-        "vertex-ai-custom-training-job", description="The slug for this task type."
-    )
+    The schema for this class is used to populate the `variables` section of the default
+    base job template.
+    """
 
-    gcp_credentials: GcpCredentials = Field(
-        default_factory=GcpCredentials,
-        description=(
-            "GCP credentials to use when running the configured Vertex AI custom "
-            "training job. If not provided, credentials will be inferred from the "
-            "environment. See `GcpCredentials` for details."
-        ),
-    )
     region: str = Field(
-        default=...,
-        description="The region where the Vertex AI custom training job resides.",
+        description="The region where the Vertex AI Job resides.",
+        examples=["us-central1"],
     )
     image: str = Field(
-        default=...,
         title="Image Name",
         description=(
-            "The image to use for a new Vertex AI custom training job. This value must "
-            "refer to an image within either Google Container Registry "
-            "or Google Artifact Registry, like `gcr.io/<project_name>/<repo>/`."
+            "The URI of a container image in the Container or Artifact Registry, "
+            "used to run your Vertex AI Job. Note that Vertex AI will need access"
+            "to the project and region where the container image is stored. See "
+            "https://cloud.google.com/vertex-ai/docs/training/create-custom-container"
         ),
+        examples=["gcr.io/your-project/your-repo:latest"],
     )
-    env: Dict[str, str] = Field(
-        default_factory=dict,
-        title="Environment Variables",
-        description="Environment variables to be passed to your Cloud Run Job.",
+    credentials: Optional[GcpCredentials] = Field(
+        title="GCP Credentials",
+        default_factory=GcpCredentials,
+        description="The GCP Credentials used to initiate the "
+        "Vertex AI Job. If not provided credentials will be "
+        "inferred from the local environment.",
     )
     machine_type: str = Field(
+        title="Machine Type",
+        description=(
+            "The machine type to use for the run, which controls "
+            "the available CPU and memory. "
+            "See https://cloud.google.com/vertex-ai/docs/reference/rest/v1/MachineSpec"
+        ),
         default="n1-standard-4",
-        description="The machine type to use for the run, which controls the available "
-        "CPU and memory.",
     )
     accelerator_type: Optional[str] = Field(
-        default=None, description="The type of accelerator to attach to the machine."
+        title="Accelerator Type",
+        description=(
+            "The type of accelerator to attach to the machine. "
+            "See https://cloud.google.com/vertex-ai/docs/reference/rest/v1/MachineSpec"
+        ),
+        examples=["NVIDIA_TESLA_K80"],
+        default=None,
     )
     accelerator_count: Optional[int] = Field(
-        default=None, description="The number of accelerators to attach to the machine."
+        title="Accelerator Count",
+        description=(
+            "The number of accelerators to attach to the machine. "
+            "See https://cloud.google.com/vertex-ai/docs/reference/rest/v1/MachineSpec"
+        ),
+        examples=[1],
+        default=None,
     )
     boot_disk_type: str = Field(
-        default="pd-ssd",
         title="Boot Disk Type",
         description="The type of boot disk to attach to the machine.",
+        default="pd-ssd",
     )
     boot_disk_size_gb: int = Field(
-        default=100,
-        title="Boot Disk Size",
+        title="Boot Disk Size (GB)",
         description="The size of the boot disk to attach to the machine, in gigabytes.",
+        default=100,
     )
-    maximum_run_time: datetime.timedelta = Field(
-        default=datetime.timedelta(days=7), description="The maximum job running time."
+    maximum_run_time_hours: int = Field(
+        default=1,
+        title="Maximum Run Time (Hours)",
+        description="The maximum job running time, in hours",
     )
     network: Optional[str] = Field(
         default=None,
+        title="Network",
         description="The full name of the Compute Engine network"
         "to which the Job should be peered. Private services access must "
         "already be configured for the network. If left unspecified, the job "
-        "is not peered with any network.",
+        "is not peered with any network. "
+        "For example: projects/12345/global/networks/myVPC",
     )
     reserved_ip_ranges: Optional[List[str]] = Field(
         default=None,
+        title="Reserved IP Ranges",
         description="A list of names for the reserved ip ranges under the VPC "
         "network that can be used for this job. If set, we will deploy the job "
         "within the provided ip ranges. Otherwise, the job will be deployed to "
         "any ip ranges under the provided VPC network.",
     )
-    service_account: Optional[str] = Field(
+    service_account_name: Optional[str] = Field(
         default=None,
+        title="Service Account Name",
         description=(
             "Specifies the service account to use "
-            "as the run-as account in Vertex AI. The agent submitting jobs must have "
+            "as the run-as account in Vertex AI. The worker submitting jobs must have "
             "act-as permission on this run-as account. If unspecified, the AI "
             "Platform Custom Code Service Agent for the CustomJob's project is "
-            "used. Takes precedence over the service account found in gcp_credentials, "
-            "and required if a service account cannot be detected in gcp_credentials."
+            "used. Takes precedence over the service account found in GCP credentials, "
+            "and required if a service account cannot be detected in GCP credentials."
         ),
     )
     job_watch_poll_interval: float = Field(
         default=5.0,
+        title="Poll Interval (Seconds)",
         description=(
             "The amount of time to wait between GCP API calls while monitoring the "
             "state of a Vertex AI Job."
         ),
     )
 
+
+def _get_base_job_spec() -> Dict[str, Any]:
+    """Returns a base job body to use for job spec validation.
+    Note that the values are stubbed and are not used for the actual job."""
+    return {
+        "maximum_run_time_hours": "1",
+        "worker_pool_specs": [
+            {
+                "replica_count": 1,
+                "container_spec": {
+                    "image_uri": "gcr.io/your-project/your-repo:latest",
+                },
+                "machine_spec": {
+                    "machine_type": "n1-standard-4",
+                },
+                "disk_spec": {
+                    "boot_disk_type": "pd-ssd",
+                    "boot_disk_size_gb": "100",
+                },
+            }
+        ],
+    }
+
+
+class VertexAIWorkerJobConfiguration(BaseJobConfiguration):
+    """
+    Configuration class used by the Vertex AI Worker to create a Job.
+
+    An instance of this class is passed to the Vertex AI Worker's `run` method
+    for each flow run. It contains all information necessary to execute
+    the flow run as a Vertex AI Job.
+
+    Attributes:
+        region: The region where the Vertex AI Job resides.
+        credentials: The GCP Credentials used to connect to Vertex AI.
+        job_spec: The Vertex AI Job spec used to create the Job.
+        job_watch_poll_interval: The interval between GCP API calls to check Job state.
+    """
+
+    region: str = Field(
+        description="The region where the Vertex AI Job resides.",
+        examples=["us-central1"],
+    )
+    credentials: Optional[GcpCredentials] = Field(
+        title="GCP Credentials",
+        default_factory=GcpCredentials,
+        description="The GCP Credentials used to initiate the "
+        "Vertex AI Job. If not provided credentials will be "
+        "inferred from the local environment.",
+    )
+
+    job_spec: Dict[str, Any] = Field(
+        json_schema_extra=dict(
+            template={
+                "service_account_name": "{{ service_account_name }}",
+                "network": "{{ network }}",
+                "reserved_ip_ranges": "{{ reserved_ip_ranges }}",
+                "maximum_run_time_hours": "{{ maximum_run_time_hours }}",
+                "worker_pool_specs": [
+                    {
+                        "replica_count": 1,
+                        "container_spec": {
+                            "image_uri": "{{ image }}",
+                            "command": "{{ command }}",
+                            "args": [],
+                        },
+                        "machine_spec": {
+                            "machine_type": "{{ machine_type }}",
+                            "accelerator_type": "{{ accelerator_type }}",
+                            "accelerator_count": "{{ accelerator_count }}",
+                        },
+                        "disk_spec": {
+                            "boot_disk_type": "{{ boot_disk_type }}",
+                            "boot_disk_size_gb": "{{ boot_disk_size_gb }}",
+                        },
+                    }
+                ],
+            }
+        ),
+    )
+    job_watch_poll_interval: float = Field(
+        default=5.0,
+        title="Poll Interval (Seconds)",
+        description=(
+            "The amount of time to wait between GCP API calls while monitoring the "
+            "state of a Vertex AI Job."
+        ),
+    )
+
+    @property
+    def project(self) -> str:
+        """property for accessing the project from the credentials."""
+        return self.credentials.project
+
     @property
-    def job_name(self):
+    def job_name(self) -> str:
         """
         The name can be up to 128 characters long and can be consist of any UTF-8 characters. Reference:
         https://cloud.google.com/python/docs/reference/aiplatform/latest/google.cloud.aiplatform.CustomJob#google_cloud_aiplatform_CustomJob_display_name
         """  # noqa
-        try:
-            base_name = self.name or self.image.split("/")[2]
-            return f"{base_name}-{uuid4().hex}"
-        except IndexError:
+        unique_suffix = uuid4().hex
+        job_name = f"{self.name}-{unique_suffix}"
+        return job_name
+
+    def prepare_for_flow_run(
+        self,
+        flow_run: "FlowRun",
+        deployment: Optional["DeploymentResponse"] = None,
+        flow: Optional["Flow"] = None,
+    ):
+        super().prepare_for_flow_run(flow_run, deployment, flow)
+
+        self._inject_formatted_env_vars()
+        self._inject_formatted_command()
+        self._ensure_existence_of_service_account()
+
+    def _inject_formatted_env_vars(self):
+        """Inject environment variables in the Vertex job_spec configuration,
+        in the correct format, which is sourced from the BaseJobConfiguration.
+        This method is invoked by `prepare_for_flow_run()`."""
+        worker_pool_specs = self.job_spec["worker_pool_specs"]
+        formatted_env_vars = [
+            {"name": key, "value": value} for key, value in self.env.items()
+        ]
+        worker_pool_specs[0]["container_spec"]["env"] = formatted_env_vars
+
+    def _inject_formatted_command(self):
+        """Inject shell commands in the Vertex job_spec configuration,
+        in the correct format, which is sourced from the BaseJobConfiguration.
+        Here, we'll ensure that the default string format
+        is converted to a list of strings."""
+        worker_pool_specs = self.job_spec["worker_pool_specs"]
+
+        existing_command = worker_pool_specs[0]["container_spec"].get("command")
+        if existing_command is None:
+            worker_pool_specs[0]["container_spec"]["command"] = shlex.split(
+                self._base_flow_run_command()
+            )
+        elif isinstance(existing_command, str):
+            worker_pool_specs[0]["container_spec"]["command"] = shlex.split(
+                existing_command
+            )
+
+    def _ensure_existence_of_service_account(self):
+        """Verify that a service account was provided, either in the credentials
+        or as a standalone service account name override."""
+
+        provided_service_account_name = self.job_spec.get("service_account_name")
+        credential_service_account = self.credentials._service_account_email
+
+        service_account_to_use = (
+            provided_service_account_name or credential_service_account
+        )
+
+        if service_account_to_use is None:
             raise ValueError(
-                "The provided image must be from either Google Container Registry "
-                "or Google Artifact Registry"
+                "A service account is required for the Vertex job. "
+                "A service account could not be detected in the attached credentials "
+                "or in the service_account_name input. "
+                "Please pass in valid GCP credentials or a valid service_account_name"
             )
 
-    def _get_compatible_labels(self) -> Dict[str, str]:
-        """
-        Ensures labels are compatible with GCP label requirements.
-        https://cloud.google.com/resource-manager/docs/creating-managing-labels
+        self.job_spec["service_account_name"] = service_account_to_use
 
-        Ex: the Prefect provided key of prefect.io/flow-name -> prefect-io_flow-name
+    @field_validator("job_spec")
+    @classmethod
+    def _ensure_job_spec_includes_required_attributes(cls, value: Dict[str, Any]):
         """
-        compatible_labels = {}
-        for key, val in self.labels.items():
-            new_key = slugify(
-                key,
-                lowercase=True,
-                replacements=[("/", "_"), (".", "-")],
-                max_length=63,
-                regex_pattern=_DISALLOWED_GCP_LABEL_CHARACTERS,
-            )
-            compatible_labels[new_key] = slugify(
-                val,
-                lowercase=True,
-                replacements=[("/", "_"), (".", "-")],
-                max_length=63,
-                regex_pattern=_DISALLOWED_GCP_LABEL_CHARACTERS,
+        Ensures that the job spec includes all required components.
+        """
+        patch = JsonPatch.from_diff(value, _get_base_job_spec())
+        missing_paths = sorted([op["path"] for op in patch if op["op"] == "add"])
+        if missing_paths:
+            raise ValueError(
+                "Job is missing required attributes at the following paths: "
+                f"{', '.join(missing_paths)}"
             )
-        return compatible_labels
+        return value
 
-    def preview(self) -> str:
-        """Generate a preview of the job definition that will be sent to GCP."""
-        job_spec = self._build_job_spec()
-        custom_job = CustomJob(
-            display_name=self.job_name,
-            job_spec=job_spec,
-            labels=self._get_compatible_labels(),
-        )
-        return str(custom_job)  # outputs a json string
 
-    def get_corresponding_worker_type(self) -> str:
-        """Return the corresponding worker type for this infrastructure block."""
-        return "vertex-ai"
+class VertexAIWorkerResult(BaseWorkerResult):
+    """Contains information about the final state of a completed process"""
+
+
+class VertexAIWorker(BaseWorker):
+    """Prefect worker that executes flow runs within Vertex AI Jobs."""
+
+    type = "vertex-ai"
+    job_configuration = VertexAIWorkerJobConfiguration
+    job_configuration_variables = VertexAIWorkerVariables
+    _description = (
+        "Execute flow runs within containers on Google Vertex AI. Requires "
+        "a Google Cloud Platform account."
+    )
+    _display_name = "Google Vertex AI"
+    _documentation_url = "https://prefecthq.github.io/prefect-gcp/vertex_worker/"
+    _logo_url = "https://cdn.sanity.io/images/3ugk85nk/production/10424e311932e31c477ac2b9ef3d53cefbaad708-250x250.png"  # noqa
 
-    async def generate_work_pool_base_job_template(self) -> dict:
+    async def run(
+        self,
+        flow_run: "FlowRun",
+        configuration: VertexAIWorkerJobConfiguration,
+        task_status: Optional[anyio.abc.TaskStatus] = None,
+    ) -> VertexAIWorkerResult:
         """
-        Generate a base job template for a `Vertex AI` work pool with the same
-        configuration as this block.
+        Executes a flow run within a Vertex AI Job and waits for the flow run
+        to complete.
+
+        Args:
+            flow_run: The flow run to execute
+            configuration: The configuration to use when executing the flow run.
+            task_status: The task status object for the current flow run. If provided,
+                the task will be marked as started.
+
         Returns:
-            - dict: a base job template for a `Vertex AI` work pool
+            VertexAIWorkerResult: A result object containing information about the
+                final state of the flow run
         """
-        base_job_template = await get_default_base_job_template_for_infrastructure_type(
-            self.get_corresponding_worker_type(),
+        logger = self.get_flow_run_logger(flow_run)
+
+        client_options = ClientOptions(
+            api_endpoint=f"{configuration.region}-aiplatform.googleapis.com"
         )
-        assert (
-            base_job_template is not None
-        ), "Failed to generate default base job template for Cloud Run worker."
-        for key, value in self.dict(exclude_unset=True, exclude_defaults=True).items():
-            if key == "command":
-                base_job_template["variables"]["properties"]["command"][
-                    "default"
-                ] = shlex.join(value)
-            elif key in [
-                "type",
-                "block_type_slug",
-                "_block_document_id",
-                "_block_document_name",
-                "_is_anonymous",
-            ]:
-                continue
-            elif key == "gcp_credentials":
-                if not self.gcp_credentials._block_document_id:
-                    raise BlockNotSavedError(
-                        "It looks like you are trying to use a block that"
-                        " has not been saved. Please call `.save` on your block"
-                        " before publishing it as a work pool."
-                    )
-                base_job_template["variables"]["properties"]["credentials"][
-                    "default"
-                ] = {
-                    "$ref": {
-                        "block_document_id": str(
-                            self.gcp_credentials._block_document_id
-                        )
-                    }
-                }
-            elif key == "maximum_run_time":
-                base_job_template["variables"]["properties"]["maximum_run_time_hours"][
-                    "default"
-                ] = round(value.total_seconds() / 3600)
-            elif key == "service_account":
-                base_job_template["variables"]["properties"]["service_account_name"][
-                    "default"
-                ] = value
-            elif key in base_job_template["variables"]["properties"]:
-                base_job_template["variables"]["properties"][key]["default"] = value
-            else:
-                self.logger.warning(
-                    f"Variable {key!r} is not supported by `Vertex AI` work pools."
-                    " Skipping."
-                )
 
-        return base_job_template
+        job_name = configuration.job_name
 
-    def _build_job_spec(self) -> "CustomJobSpec":
-        """
-        Builds a job spec by gathering details.
-        """
-        # gather worker pool spec
-        env_list = [
-            {"name": name, "value": value}
-            for name, value in {
-                **self._base_environment(),
-                **self.env,
-            }.items()
-        ]
-        container_spec = ContainerSpec(
-            image_uri=self.image, command=self.command, args=[], env=env_list
+        job_spec = self._build_job_spec(configuration)
+        job_service_async_client = (
+            configuration.credentials.get_job_service_async_client(
+                client_options=client_options
+            )
         )
-        machine_spec = MachineSpec(
-            machine_type=self.machine_type,
-            accelerator_type=self.accelerator_type,
-            accelerator_count=self.accelerator_count,
-        )
-        worker_pool_spec = WorkerPoolSpec(
-            container_spec=container_spec,
-            machine_spec=machine_spec,
-            replica_count=1,
-            disk_spec=DiskSpec(
-                boot_disk_type=self.boot_disk_type,
-                boot_disk_size_gb=self.boot_disk_size_gb,
+
+        job_run = await self._create_and_begin_job(
+            job_name,
+            job_spec,
+            job_service_async_client,
+            configuration,
+            logger,
+        )
+
+        if task_status:
+            task_status.started(job_run.name)
+
+        final_job_run = await self._watch_job_run(
+            job_name=job_name,
+            full_job_name=job_run.name,
+            job_service_async_client=job_service_async_client,
+            current_state=job_run.state,
+            until_states=(
+                JobState.JOB_STATE_SUCCEEDED,
+                JobState.JOB_STATE_FAILED,
+                JobState.JOB_STATE_CANCELLED,
+                JobState.JOB_STATE_EXPIRED,
+            ),
+            configuration=configuration,
+            logger=logger,
+            timeout=int(
+                datetime.timedelta(
+                    hours=configuration.job_spec["maximum_run_time_hours"]
+                ).total_seconds()
             ),
         )
-        # look for service account
-        service_account = (
-            self.service_account or self.gcp_credentials._service_account_email
+
+        error_msg = final_job_run.error.message
+
+        # Vertex will include an error message upon valid
+        # flow cancellations, so we'll avoid raising an error in that case
+        if error_msg and "CANCELED" not in error_msg:
+            raise RuntimeError(error_msg)
+
+        status_code = 0 if final_job_run.state == JobState.JOB_STATE_SUCCEEDED else 1
+
+        return VertexAIWorkerResult(
+            identifier=final_job_run.display_name, status_code=status_code
         )
-        if service_account is None:
-            raise ValueError(
-                "A service account is required for the Vertex job. "
-                "A service account could not be detected in the attached credentials; "
-                "please set a service account explicitly, e.g. "
-                '`VertexAICustomTrainingJob(service_acount="...")`'
+
+    def _build_job_spec(
+        self, configuration: VertexAIWorkerJobConfiguration
+    ) -> "CustomJobSpec":
+        """
+        Builds a job spec by gathering details.
+        """
+        # here, we extract the `worker_pool_specs` out of the job_spec
+        worker_pool_specs = [
+            WorkerPoolSpec(
+                container_spec=ContainerSpec(**spec["container_spec"]),
+                machine_spec=MachineSpec(**spec["machine_spec"]),
+                replica_count=spec["replica_count"],
+                disk_spec=DiskSpec(**spec["disk_spec"]),
             )
+            for spec in configuration.job_spec.pop("worker_pool_specs", [])
+        ]
 
-        # build custom job specs
-        timeout = Duration().FromTimedelta(td=self.maximum_run_time)
+        timeout = Duration().FromTimedelta(
+            td=datetime.timedelta(
+                hours=configuration.job_spec["maximum_run_time_hours"]
+            )
+        )
         scheduling = Scheduling(timeout=timeout)
+
+        # construct the final job spec that we will provide to Vertex AI
         job_spec = CustomJobSpec(
-            worker_pool_specs=[worker_pool_spec],
-            service_account=service_account,
+            worker_pool_specs=worker_pool_specs,
             scheduling=scheduling,
-            network=self.network,
-            reserved_ip_ranges=self.reserved_ip_ranges,
+            ignore_unknown_fields=True,
+            **configuration.job_spec,
         )
         return job_spec
 
     async def _create_and_begin_job(
-        self, job_spec: "CustomJobSpec", job_service_client: "JobServiceClient"
+        self,
+        job_name: str,
+        job_spec: "CustomJobSpec",
+        job_service_async_client: "JobServiceAsyncClient",
+        configuration: VertexAIWorkerJobConfiguration,
+        logger: PrefectLogAdapter,
     ) -> "CustomJob":
         """
         Builds a custom job and begins running it.
         """
         # create custom job
         custom_job = CustomJob(
-            display_name=self.job_name,
+            display_name=job_name,
             job_spec=job_spec,
-            labels=self._get_compatible_labels(),
+            labels=self._get_compatible_labels(configuration=configuration),
         )
 
         # run job
-        self.logger.info(
-            f"{self._log_prefix}: Job {self.job_name!r} starting to run "
-            f"the command {' '.join(self.command)!r} in region "
-            f"{self.region!r} using image {self.image!r}"
-        )
+        logger.info(f"Creating job {job_name!r}")
 
-        project = self.gcp_credentials.project
-        resource_name = f"projects/{project}/locations/{self.region}"
+        project = configuration.project
+        resource_name = f"projects/{project}/locations/{configuration.region}"
 
-        retry_policy = retry(
+        async for attempt in AsyncRetrying(
             stop=stop_after_attempt(3), wait=wait_fixed(1) + wait_random(0, 3)
-        )
-
-        custom_job_run = await run_sync_in_worker_thread(
-            retry_policy(job_service_client.create_custom_job),
-            parent=resource_name,
-            custom_job=custom_job,
-        )
+        ):
+            with attempt:
+                custom_job_run = await job_service_async_client.create_custom_job(
+                    parent=resource_name,
+                    custom_job=custom_job,
+                )
 
-        self.logger.info(
-            f"{self._log_prefix}: Job {self.job_name!r} has successfully started; "
-            f"the full job name is {custom_job_run.name!r}"
+        logger.info(
+            f"Job {job_name!r} created. "
+            f"The full job name is {custom_job_run.name!r}"
         )
 
         return custom_job_run
 
     async def _watch_job_run(
         self,
-        full_job_name: str,  # different from self.job_name
-        job_service_client: "JobServiceClient",
+        job_name: str,
+        full_job_name: str,  # different from job_name
+        job_service_async_client: "JobServiceAsyncClient",
         current_state: "JobState",
         until_states: Tuple["JobState"],
+        configuration: VertexAIWorkerJobConfiguration,
+        logger: PrefectLogAdapter,
         timeout: int = None,
     ) -> "CustomJob":
         """
         Polls job run to see if status changed.
+
+        State changes reported by the Vertex AI API may sometimes be inaccurate
+        immediately upon startup, but should eventually report a correct running
+        and then terminal state. The minimum training duration for a custom job is
+        30 seconds, so short-lived jobs may be marked as successful some time
+        after a flow run has completed.
         """
         state = JobState.JOB_STATE_UNSPECIFIED
         last_state = current_state
         t0 = time.time()
 
         while state not in until_states:
-            job_run = await run_sync_in_worker_thread(
-                job_service_client.get_custom_job,
+            job_run = await job_service_async_client.get_custom_job(
                 name=full_job_name,
             )
             state = job_run.state
             if state != last_state:
                 state_label = (
                     state.name.replace("_", " ")
                     .lower()
                     .replace("state", "state is now:")
                 )
                 # results in "New job state is now: succeeded"
-                self.logger.info(
-                    f"{self._log_prefix}: {self.job_name} has new {state_label}"
-                )
+                logger.debug(f"{job_name} has new {state_label}")
                 last_state = state
             else:
                 # Intermittently, the job will not be described. We want to respect the
                 # watch timeout though.
-                self.logger.debug(f"{self._log_prefix}: Job not found.")
+                logger.debug(f"Job {job_name} not found.")
 
             elapsed_time = time.time() - t0
             if timeout is not None and elapsed_time > timeout:
                 raise RuntimeError(
                     f"Timed out after {elapsed_time}s while watching job for states "
                     "{until_states!r}"
                 )
-            time.sleep(self.job_watch_poll_interval)
+            await asyncio.sleep(configuration.job_watch_poll_interval)
 
         return job_run
 
-    @sync_compatible
-    async def run(
-        self, task_status: Optional["TaskStatus"] = None
-    ) -> VertexAICustomTrainingJobResult:
+    def _get_compatible_labels(
+        self, configuration: VertexAIWorkerJobConfiguration
+    ) -> Dict[str, str]:
         """
-        Run the configured task on VertexAI.
-
-        Args:
-            task_status: An optional `TaskStatus` to update when the container starts.
+        Ensures labels are compatible with GCP label requirements.
+        https://cloud.google.com/resource-manager/docs/creating-managing-labels
 
-        Returns:
-            The `VertexAICustomTrainingJobResult`.
+        Ex: the Prefect provided key of prefect.io/flow-name -> prefect-io_flow-name
         """
-        client_options = ClientOptions(
-            api_endpoint=f"{self.region}-aiplatform.googleapis.com"
-        )
-
-        job_spec = self._build_job_spec()
-        with self.gcp_credentials.get_job_service_client(
-            client_options=client_options
-        ) as job_service_client:
-            job_run = await self._create_and_begin_job(job_spec, job_service_client)
-
-            if task_status:
-                task_status.started(self.job_name)
-
-            final_job_run = await self._watch_job_run(
-                full_job_name=job_run.name,
-                job_service_client=job_service_client,
-                current_state=job_run.state,
-                until_states=(
-                    JobState.JOB_STATE_SUCCEEDED,
-                    JobState.JOB_STATE_FAILED,
-                    JobState.JOB_STATE_CANCELLED,
-                    JobState.JOB_STATE_EXPIRED,
-                ),
-                timeout=self.maximum_run_time.total_seconds(),
+        compatible_labels = {}
+        for key, val in configuration.labels.items():
+            new_key = slugify(
+                key,
+                lowercase=True,
+                replacements=[("/", "_"), (".", "-")],
+                max_length=63,
+                regex_pattern=_DISALLOWED_GCP_LABEL_CHARACTERS,
             )
+            compatible_labels[new_key] = slugify(
+                val,
+                lowercase=True,
+                replacements=[("/", "_"), (".", "-")],
+                max_length=63,
+                regex_pattern=_DISALLOWED_GCP_LABEL_CHARACTERS,
+            )
+        return compatible_labels
 
-        error_msg = final_job_run.error.message
-        if error_msg:
-            raise RuntimeError(f"{self._log_prefix}: {error_msg}")
-
-        status_code = 0 if final_job_run.state == JobState.JOB_STATE_SUCCEEDED else 1
+    async def kill_infrastructure(
+        self,
+        infrastructure_pid: str,
+        configuration: VertexAIWorkerJobConfiguration,
+        grace_seconds: int = 30,
+    ):
+        """
+        Stops a job running in Vertex AI upon flow cancellation,
+        based on the provided infrastructure PID + run configuration.
+        """
+        if grace_seconds != 30:
+            self._logger.warning(
+                f"Kill grace period of {grace_seconds}s requested, but GCP does not "
+                "support dynamic grace period configuration. See here for more info: "
+                "https://cloud.google.com/vertex-ai/docs/reference/rest/v1/projects.locations.customJobs/cancel"  # noqa
+            )
 
-        return VertexAICustomTrainingJobResult(
-            identifier=final_job_run.display_name, status_code=status_code
+        client_options = ClientOptions(
+            api_endpoint=f"{configuration.region}-aiplatform.googleapis.com"
+        )
+        job_service_async_client = (
+            configuration.credentials.get_job_service_async_client(
+                client_options=client_options
+            )
+        )
+        await self._stop_job(
+            client=job_service_async_client,
+            vertex_job_name=infrastructure_pid,
         )
 
-    @sync_compatible
-    async def kill(self, identifier: str, grace_seconds: int = 30) -> None:
-        """
-        Kill a job running Cloud Run.
-
-        Args:
-            identifier: The Vertex AI full job name, formatted like
-                "projects/{project}/locations/{location}/customJobs/{custom_job}".
-
-        Returns:
-            The `VertexAICustomTrainingJobResult`.
+    async def _stop_job(self, client: "JobServiceAsyncClient", vertex_job_name: str):
         """
-        client_options = ClientOptions(
-            api_endpoint=f"{self.region}-aiplatform.googleapis.com"
-        )
-        with self.gcp_credentials.get_job_service_client(
-            client_options=client_options
-        ) as job_service_client:
-            await run_sync_in_worker_thread(
-                self._kill_job,
-                job_service_client=job_service_client,
-                full_job_name=identifier,
-            )
-            self.logger.info(f"Requested to cancel {identifier}...")
-
-    def _kill_job(
-        self, job_service_client: "JobServiceClient", full_job_name: str
-    ) -> None:
-        """
-        Thin wrapper around Job.delete, wrapping a try/except since
-        Job is an independent class that doesn't have knowledge of
-        CloudRunJob and its associated logic.
+        Calls the `cancel_custom_job` method on the Vertex AI Job Service Client.
         """
-        cancel_custom_job_request = CancelCustomJobRequest(name=full_job_name)
+        cancel_custom_job_request = CancelCustomJobRequest(name=vertex_job_name)
         try:
-            job_service_client.cancel_custom_job(
+            await client.cancel_custom_job(
                 request=cancel_custom_job_request,
             )
         except Exception as exc:
             if "does not exist" in str(exc):
                 raise InfrastructureNotFound(
-                    f"Cannot stop Vertex AI job; the job name {full_job_name!r} "
+                    f"Cannot stop Vertex AI job; the job name {vertex_job_name!r} "
                     "could not be found."
                 ) from exc
             raise
-
-    @property
-    def _log_prefix(self) -> str:
-        """
-        Internal property for generating a prefix for logs where `name` may be null
-        """
-        if self.name is not None:
-            return f"VertexAICustomTrainingJob {self.name!r}"
-        else:
-            return "VertexAICustomTrainingJob"
```

### Comparing `prefect_gcp-0.5.9/prefect_gcp/bigquery.py` & `prefect_gcp-0.6.0rc1/prefect_gcp/bigquery.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,26 +2,20 @@
 
 import os
 from functools import partial
 from pathlib import Path
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
 from anyio import to_thread
-from pydantic import VERSION as PYDANTIC_VERSION
+from pydantic import Field
 
 from prefect import get_run_logger, task
 from prefect.blocks.abstract import DatabaseBlock
 from prefect.utilities.asyncutils import run_sync_in_worker_thread, sync_compatible
 from prefect.utilities.hashing import hash_objects
-
-if PYDANTIC_VERSION.startswith("2."):
-    from pydantic.v1 import Field
-else:
-    from pydantic import Field
-
 from prefect_gcp.credentials import GcpCredentials
 
 try:
     from google.cloud.bigquery import (
         ExternalConfig,
         LoadJob,
         LoadJobConfig,
@@ -44,14 +38,15 @@
     Helper function to ensure result is run on a single thread.
     """
     result = func(*args, **kwargs).result()
     return result
 
 
 @task
+@sync_compatible
 async def bigquery_query(
     query: str,
     gcp_credentials: GcpCredentials,
     query_params: Optional[List[tuple]] = None,  # 3-tuples
     dry_run_max_bytes: Optional[int] = None,
     dataset: Optional[str] = None,
     table: Optional[str] = None,
@@ -171,14 +166,15 @@
         if result_transformer:
             return result_transformer(result)
         else:
             return list(result)
 
 
 @task
+@sync_compatible
 async def bigquery_create_table(
     dataset: str,
     table: str,
     gcp_credentials: GcpCredentials,
     schema: Optional[List["SchemaField"]] = None,
     clustering_fields: List[str] = None,
     time_partitioning: "TimePartitioning" = None,
@@ -204,14 +200,15 @@
         Table name.
     Example:
         ```python
         from prefect import flow
         from prefect_gcp import GcpCredentials
         from prefect_gcp.bigquery import bigquery_create_table
         from google.cloud.bigquery import SchemaField
+
         @flow
         def example_bigquery_create_table_flow():
             gcp_credentials = GcpCredentials(project="project")
             schema = [
                 SchemaField("number", field_type="INTEGER", mode="REQUIRED"),
                 SchemaField("text", field_type="STRING", mode="REQUIRED"),
                 SchemaField("bool", field_type="BOOLEAN")
@@ -265,14 +262,15 @@
         partial_create_table = partial(client.create_table, table_obj)
         await to_thread.run_sync(partial_create_table)
 
     return table
 
 
 @task
+@sync_compatible
 async def bigquery_insert_stream(
     dataset: str,
     table: str,
     records: List[dict],
     gcp_credentials: GcpCredentials,
     project: Optional[str] = None,
     location: str = "US",
@@ -340,14 +338,15 @@
     if errors:
         raise ValueError(errors)
 
     return output
 
 
 @task
+@sync_compatible
 async def bigquery_load_cloud_storage(
     dataset: str,
     table: str,
     uri: str,
     gcp_credentials: GcpCredentials,
     schema: Optional[List["SchemaField"]] = None,
     job_config: Optional[dict] = None,
@@ -428,14 +427,15 @@
         result._client = None
         result._completion_lock = None
 
     return result
 
 
 @task
+@sync_compatible
 async def bigquery_load_file(
     dataset: str,
     table: str,
     path: Union[str, Path],
     gcp_credentials: GcpCredentials,
     schema: Optional[List["SchemaField"]] = None,
     job_config: Optional[dict] = None,
```

### Comparing `prefect_gcp-0.5.9/prefect_gcp/cloud_run.py` & `prefect_gcp-0.6.0rc1/prefect_gcp/workers/cloud_run.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,732 +1,773 @@
-"""
-DEPRECATION WARNING:
-
-This module is deprecated as of March 2024 and will not be available after September 2024.
-It has been replaced by the Cloud Run and Cloud Run V2 workers, which offer enhanced functionality and better performance.
+"""<!-- # noqa -->
 
-For upgrade instructions, see https://docs.prefect.io/latest/guides/upgrade-guide-agents-to-workers/.
+Module containing the Cloud Run worker used for executing flow runs as Cloud Run jobs.
 
-Integrations with Google Cloud Run Job.
+Get started by creating a Cloud Run work pool:
 
-Examples:
-
-    Run a job using Google Cloud Run Jobs:
-    ```python
-    CloudRunJob(
-        image="gcr.io/my-project/my-image",
-        region="us-east1",
-        credentials=my_gcp_credentials
-    ).run()
+```bash
+prefect work-pool create 'my-cloud-run-pool' --type cloud-run
+```
+
+Then start a Cloud Run worker with the following command:
+
+```bash
+prefect worker start --pool 'my-cloud-run-pool'
+```
+
+## Configuration
+Read more about configuring work pools
+[here](https://docs.prefect.io/latest/concepts/work-pools/#work-pool-overview).
+
+## Advanced Configuration
+!!! example "Using a custom Cloud Run job template"
+    Below is the default job body template used by the Cloud Run Worker:
+    ```json
+    {
+        "apiVersion": "run.googleapis.com/v1",
+        "kind": "Job",
+        "metadata":
+            {
+                "name": "{{ name }}",
+                "annotations":
+                {
+                    "run.googleapis.com/launch-stage": "BETA",
+                }
+            },
+            "spec":
+            {
+                "template":
+                {
+                    "spec":
+                    {
+                        "template":
+                        {
+                            "spec":
+                            {
+                                "containers":
+                                [
+                                    {
+                                        "image": "{{ image }}",
+                                        "args": "{{ args }}",
+                                        "resources":
+                                        {
+                                            "limits":
+                                            {
+                                                "cpu": "{{ cpu }}",
+                                                "memory": "{{ memory }}"
+                                            },
+                                            "requests":
+                                            {
+                                                "cpu": "{{ cpu }}",
+                                                "memory": "{{ memory }}"
+                                            }
+                                        }
+                                    }
+                                ],
+                                "timeoutSeconds": "{{ timeout }}",
+                                "serviceAccountName": "{{ service_account_name }}"
+                            }
+                        }
+                    }
+                    }
+                },
+                "metadata":
+                {
+                    "annotations":
+                    {
+                        "run.googleapis.com/vpc-access-connector": "{{ vpc_connector_name }}"
+                    }
+                }
+            },
+        },
+        "timeout": "{{ timeout }}",
+        "keep_job": "{{ keep_job }}"
+    }
     ```
-
-    Run a job that runs the command `echo hello world` using Google Cloud Run Jobs:
-    ```python
-    CloudRunJob(
-        image="gcr.io/my-project/my-image",
-        region="us-east1",
-        credentials=my_gcp_credentials
-        command=["echo", "hello world"]
-    ).run()
+    Each values enclosed in `{{ }}` is a placeholder that will be replaced with
+    a value at runtime on a per-deployment basis. The values that can be used a
+    placeholders are defined by the `variables` schema defined in the base job template.
+
+    The default job body template and available variables can be customized on a work pool
+    by work pool basis. By editing the default job body template you can:
+
+    - Add additional placeholders to the default job template
+    - Remove placeholders from the default job template
+    - Pass values to Cloud Run that are not defined in the `variables` schema
+
+    ### Adding additional placeholders
+    For example, to allow for extra customization of a new annotation not described in
+    the default job template, you can add the following:
+    ```json
+    {
+        "apiVersion": "run.googleapis.com/v1",
+        "kind": "Job",
+        "metadata":
+        {
+            "name": "{{ name }}",
+            "annotations":
+            {
+                "run.googleapis.com/my-custom-annotation": "{{ my_custom_annotation }}",
+                "run.googleapis.com/launch-stage": "BETA",
+            },
+          ...
+        },
+      ...
+    }
     ```
+    `my_custom_annotation` can now be used as a placeholder in the job template and set
+    on a per-deployment basis.
 
-"""  # noqa
+    ```yaml
+    # prefect.yaml
+    deployments:
+    ...
+      - name: my-deployment
+      ...
+      work_pool: my-cloud-run-pool
+        job_variables: {"my_custom_annotation": "my-custom-value"}
+    ```
 
-from __future__ import annotations
+    Additionally, fields can be set to prevent configuration at the deployment
+    level. For example to configure the `vpc_connector_name` field, the placeholder can
+    be removed and replaced with an actual value. Now all deployments that point to this
+    work pool will use the same `vpc_connector_name` value.
+
+    ```json
+    {
+        "apiVersion": "run.googleapis.com/v1",
+        "kind": "Job",
+        "spec":
+        {
+            "template":
+            {
+                "metadata":
+                {
+                    "annotations":
+                    {
+                        "run.googleapis.com/vpc-access-connector": "my-vpc-connector"
+                    }
+                },
+                ...
+            },
+            ...
+        }
+    }
+    ```
+"""
 
-import json
 import re
 import shlex
 import time
-from typing import Any, Dict, List, Optional
+from typing import TYPE_CHECKING, Any, Dict, Optional
 from uuid import uuid4
 
+import anyio
 import googleapiclient
-from anyio.abc import TaskStatus
+from anyio.abc import TaskStatus  # noqa
 from google.api_core.client_options import ClientOptions
 from googleapiclient import discovery
 from googleapiclient.discovery import Resource
-from pydantic import VERSION as PYDANTIC_VERSION
+from pydantic import Field, field_validator
 
-from prefect._internal.compatibility.deprecated import deprecated_class
 from prefect.exceptions import InfrastructureNotFound
-from prefect.infrastructure.base import Infrastructure, InfrastructureResult
-from prefect.utilities.asyncutils import run_sync_in_worker_thread, sync_compatible
-
-if PYDANTIC_VERSION.startswith("2."):
-    from pydantic.v1 import BaseModel, Field, root_validator, validator
-else:
-    from pydantic import BaseModel, Field, root_validator, validator
-
-from typing_extensions import Literal
-
-from prefect.blocks.core import BlockNotSavedError
-from prefect.workers.utilities import (
-    get_default_base_job_template_for_infrastructure_type,
+from prefect.logging.loggers import PrefectLogAdapter
+from prefect.utilities.asyncutils import run_sync_in_worker_thread
+from prefect.utilities.dockerutils import get_prefect_image_name
+from prefect.utilities.pydantic import JsonPatch
+from prefect.workers.base import (
+    BaseJobConfiguration,
+    BaseVariables,
+    BaseWorker,
+    BaseWorkerResult,
 )
 from prefect_gcp.credentials import GcpCredentials
+from prefect_gcp.utilities import Execution, Job, slugify_name
+
+if TYPE_CHECKING:
+    from prefect.client.schemas import FlowRun
+    from prefect.server.schemas.core import Flow
+    from prefect.server.schemas.responses import DeploymentResponse
+
+
+def _get_default_job_body_template() -> Dict[str, Any]:
+    """Returns the default job body template used by the Cloud Run Job."""
+    return {
+        "apiVersion": "run.googleapis.com/v1",
+        "kind": "Job",
+        "metadata": {
+            "name": "{{ name }}",
+            "annotations": {
+                # See: https://cloud.google.com/run/docs/troubleshooting#launch-stage-validation  # noqa
+                "run.googleapis.com/launch-stage": "BETA",
+            },
+        },
+        "spec": {  # JobSpec
+            "template": {  # ExecutionTemplateSpec
+                "spec": {  # ExecutionSpec
+                    "template": {  # TaskTemplateSpec
+                        "spec": {  # TaskSpec
+                            "containers": [
+                                {
+                                    "image": "{{ image }}",
+                                    "command": "{{ command }}",
+                                    "resources": {
+                                        "limits": {
+                                            "cpu": "{{ cpu }}",
+                                            "memory": "{{ memory }}",
+                                        },
+                                        "requests": {
+                                            "cpu": "{{ cpu }}",
+                                            "memory": "{{ memory }}",
+                                        },
+                                    },
+                                }
+                            ],
+                            "timeoutSeconds": "{{ timeout }}",
+                            "serviceAccountName": "{{ service_account_name }}",
+                        }
+                    },
+                },
+                "metadata": {
+                    "annotations": {
+                        "run.googleapis.com/vpc-access-connector": "{{ vpc_connector_name }}"  # noqa
+                    }
+                },
+            },
+        },
+    }
 
 
-class Job(BaseModel):
+def _get_base_job_body() -> Dict[str, Any]:
+    """Returns a base job body to use for job body validation."""
+    return {
+        "apiVersion": "run.googleapis.com/v1",
+        "kind": "Job",
+        "metadata": {
+            "annotations": {
+                # See: https://cloud.google.com/run/docs/troubleshooting#launch-stage-validation  # noqa
+                "run.googleapis.com/launch-stage": "BETA",
+            },
+        },
+        "spec": {  # JobSpec
+            "template": {  # ExecutionTemplateSpec
+                "spec": {  # ExecutionSpec
+                    "template": {  # TaskTemplateSpec
+                        "spec": {"containers": [{}]},  # TaskSpec
+                    },
+                },
+            },
+        },
+    }
+
+
+class CloudRunWorkerJobConfiguration(BaseJobConfiguration):
     """
-    Utility class to call GCP `jobs` API and
-    interact with the returned objects.
+    Configuration class used by the Cloud Run Worker to create a Cloud Run Job.
+
+    An instance of this class is passed to the Cloud Run worker's `run` method
+    for each flow run. It contains all information necessary to execute
+    the flow run as a Cloud Run Job.
+
+    Attributes:
+        region: The region where the Cloud Run Job resides.
+        credentials: The GCP Credentials used to connect to Cloud Run.
+        job_body: The job body used to create the Cloud Run Job.
+        timeout: The length of time that Prefect will wait for a Cloud Run Job.
+        keep_job: Whether to delete the Cloud Run Job after it completes.
     """
 
-    metadata: dict
-    spec: dict
-    status: dict
-    name: str
-    ready_condition: dict
-    execution_status: dict
-
-    def _is_missing_container(self):
-        """
-        Check if Job status is not ready because
-        the specified container cannot be found.
-        """
-        if (
-            self.ready_condition.get("status") == "False"
-            and self.ready_condition.get("reason") == "ContainerMissing"
-        ):
-            return True
-        return False
-
-    def is_ready(self) -> bool:
-        """Whether a job is finished registering and ready to be executed"""
-        if self._is_missing_container():
-            raise Exception(f"{self.ready_condition['message']}")
-        return self.ready_condition.get("status") == "True"
-
-    def has_execution_in_progress(self) -> bool:
-        """See if job has a run in progress."""
-        return (
-            self.execution_status == {}
-            or self.execution_status.get("completionTimestamp") is None
-        )
+    region: str = Field(
+        default="us-central1", description="The region where the Cloud Run Job resides."
+    )
+    credentials: Optional[GcpCredentials] = Field(
+        title="GCP Credentials",
+        default_factory=GcpCredentials,
+        description="The GCP Credentials used to connect to Cloud Run. "
+        "If not provided credentials will be inferred from "
+        "the local environment.",
+    )
+    job_body: Dict[str, Any] = Field(
+        json_schema_extra=dict(template=_get_default_job_body_template())
+    )
+    timeout: Optional[int] = Field(
+        default=600,
+        gt=0,
+        le=3600,
+        title="Job Timeout",
+        description=(
+            "The length of time that Prefect will wait for a Cloud Run Job to complete "
+            "before raising an exception."
+        ),
+    )
+    keep_job: Optional[bool] = Field(
+        default=False,
+        title="Keep Job After Completion",
+        description="Keep the completed Cloud Run Job on Google Cloud Platform.",
+    )
 
-    @staticmethod
-    def _get_ready_condition(job: dict) -> dict:
-        """Utility to access JSON field containing ready condition."""
-        if job["status"].get("conditions"):
-            for condition in job["status"]["conditions"]:
-                if condition["type"] == "Ready":
-                    return condition
-
-        return {}
-
-    @staticmethod
-    def _get_execution_status(job: dict):
-        """Utility to access JSON field containing execution status."""
-        if job["status"].get("latestCreatedExecution"):
-            return job["status"]["latestCreatedExecution"]
+    @property
+    def project(self) -> str:
+        """property for accessing the project from the credentials."""
+        return self.credentials.project
 
-        return {}
+    @property
+    def job_name(self) -> str:
+        """property for accessing the name from the job metadata."""
+        return self.job_body["metadata"]["name"]
+
+    def prepare_for_flow_run(
+        self,
+        flow_run: "FlowRun",
+        deployment: Optional["DeploymentResponse"] = None,
+        flow: Optional["Flow"] = None,
+    ):
+        """
+        Prepares the job configuration for a flow run.
 
-    @classmethod
-    def get(cls, client: Resource, namespace: str, job_name: str):
-        """Make a get request to the GCP jobs API and return a Job instance."""
-        request = client.jobs().get(name=f"namespaces/{namespace}/jobs/{job_name}")
-        response = request.execute()
-
-        return cls(
-            metadata=response["metadata"],
-            spec=response["spec"],
-            status=response["status"],
-            name=response["metadata"]["name"],
-            ready_condition=cls._get_ready_condition(response),
-            execution_status=cls._get_execution_status(response),
-        )
+        Ensures that necessary values are present in the job body and that the
+        job body is valid.
 
-    @staticmethod
-    def create(client: Resource, namespace: str, body: dict):
-        """Make a create request to the GCP jobs API."""
-        request = client.jobs().create(parent=f"namespaces/{namespace}", body=body)
-        response = request.execute()
-        return response
-
-    @staticmethod
-    def delete(client: Resource, namespace: str, job_name: str):
-        """Make a delete request to the GCP jobs API."""
-        request = client.jobs().delete(name=f"namespaces/{namespace}/jobs/{job_name}")
-        response = request.execute()
-        return response
-
-    @staticmethod
-    def run(client: Resource, namespace: str, job_name: str):
-        """Make a run request to the GCP jobs API."""
-        request = client.jobs().run(name=f"namespaces/{namespace}/jobs/{job_name}")
-        response = request.execute()
-        return response
+        Args:
+            flow_run: The flow run to prepare the job configuration for
+            deployment: The deployment associated with the flow run used for
+                preparation.
+            flow: The flow associated with the flow run used for preparation.
+        """
+        super().prepare_for_flow_run(flow_run, deployment, flow)
+
+        self._populate_envs()
+        self._populate_or_format_command()
+        self._format_args_if_present()
+        self._populate_image_if_not_present()
+        self._populate_name_if_not_present()
+
+    def _populate_envs(self):
+        """Populate environment variables. BaseWorker.prepare_for_flow_run handles
+        putting the environment variables in the `env` attribute. This method
+        moves them into the jobs body"""
+        envs = [{"name": k, "value": v} for k, v in self.env.items()]
+        self.job_body["spec"]["template"]["spec"]["template"]["spec"]["containers"][0][
+            "env"
+        ] = envs
 
+    def _populate_name_if_not_present(self):
+        """Adds the flow run name to the job if one is not already provided."""
+        try:
+            if "name" not in self.job_body["metadata"]:
+                base_job_name = slugify_name(self.name)
+                job_name = f"{base_job_name}-{uuid4().hex}"
+                self.job_body["metadata"]["name"] = job_name
+        except KeyError:
+            raise ValueError("Unable to verify name due to invalid job body template.")
 
-class Execution(BaseModel):
-    """
-    Utility class to call GCP `executions` API and
-    interact with the returned objects.
-    """
+    def _populate_image_if_not_present(self):
+        """Adds the latest prefect image to the job if one is not already provided."""
+        try:
+            if (
+                "image"
+                not in self.job_body["spec"]["template"]["spec"]["template"]["spec"][
+                    "containers"
+                ][0]
+            ):
+                self.job_body["spec"]["template"]["spec"]["template"]["spec"][
+                    "containers"
+                ][0]["image"] = f"docker.io/{get_prefect_image_name()}"
+        except KeyError:
+            raise ValueError("Unable to verify image due to invalid job body template.")
 
-    name: str
-    namespace: str
-    metadata: dict
-    spec: dict
-    status: dict
-    log_uri: str
-
-    def is_running(self) -> bool:
-        """Returns True if Execution is not completed."""
-        return self.status.get("completionTime") is None
-
-    def condition_after_completion(self):
-        """Returns Execution condition if Execution has completed."""
-        for condition in self.status["conditions"]:
-            if condition["type"] == "Completed":
-                return condition
-
-    def succeeded(self):
-        """Whether or not the Execution completed is a successful state."""
-        completed_condition = self.condition_after_completion()
-        if completed_condition and completed_condition["status"] == "True":
-            return True
+    def _populate_or_format_command(self):
+        """
+        Ensures that the command is present in the job manifest. Populates the command
+        with the `prefect -m prefect.engine` if a command is not present.
+        """
+        try:
+            command = self.job_body["spec"]["template"]["spec"]["template"]["spec"][
+                "containers"
+            ][0].get("command")
+            if command is None:
+                self.job_body["spec"]["template"]["spec"]["template"]["spec"][
+                    "containers"
+                ][0]["command"] = shlex.split(self._base_flow_run_command())
+            elif isinstance(command, str):
+                self.job_body["spec"]["template"]["spec"]["template"]["spec"][
+                    "containers"
+                ][0]["command"] = shlex.split(command)
+        except KeyError:
+            raise ValueError(
+                "Unable to verify command due to invalid job body template."
+            )
 
-        return False
+    def _format_args_if_present(self):
+        try:
+            args = self.job_body["spec"]["template"]["spec"]["template"]["spec"][
+                "containers"
+            ][0].get("args")
+            if args is not None and isinstance(args, str):
+                self.job_body["spec"]["template"]["spec"]["template"]["spec"][
+                    "containers"
+                ][0]["args"] = shlex.split(args)
+        except KeyError:
+            raise ValueError("Unable to verify args due to invalid job body template.")
 
+    @field_validator("job_body")
     @classmethod
-    def get(cls, client: Resource, namespace: str, execution_name: str):
+    def _ensure_job_includes_all_required_components(cls, value: Dict[str, Any]):
         """
-        Make a get request to the GCP executions API
-        and return an Execution instance.
+        Ensures that the job body includes all required components.
         """
-        request = client.executions().get(
-            name=f"namespaces/{namespace}/executions/{execution_name}"
-        )
-        response = request.execute()
+        patch = JsonPatch.from_diff(value, _get_base_job_body())
+        missing_paths = sorted([op["path"] for op in patch if op["op"] == "add"])
+        if missing_paths:
+            raise ValueError(
+                "Job is missing required attributes at the following paths: "
+                f"{', '.join(missing_paths)}"
+            )
+        return value
 
-        return cls(
-            name=response["metadata"]["name"],
-            namespace=response["metadata"]["namespace"],
-            metadata=response["metadata"],
-            spec=response["spec"],
-            status=response["status"],
-            log_uri=response["status"]["logUri"],
+    @field_validator("job_body")
+    @classmethod
+    def _ensure_job_has_compatible_values(cls, value: Dict[str, Any]):
+        """Ensure that the job body has compatible values."""
+        patch = JsonPatch.from_diff(value, _get_base_job_body())
+        incompatible = sorted(
+            [
+                f"{op['path']} must have value {op['value']!r}"
+                for op in patch
+                if op["op"] == "replace"
+            ]
         )
+        if incompatible:
+            raise ValueError(
+                "Job has incompatible values for the following attributes: "
+                f"{', '.join(incompatible)}"
+            )
+        return value
 
 
-class CloudRunJobResult(InfrastructureResult):
-    """Result from a Cloud Run Job."""
-
-
-@deprecated_class(
-    start_date="Mar 2024",
-    help=(
-        "Use the Cloud Run or Cloud Run v2 worker instead."
-        " Refer to the upgrade guide for more information:"
-        " https://docs.prefect.io/latest/guides/upgrade-guide-agents-to-workers/."
-    ),
-)
-class CloudRunJob(Infrastructure):
+class CloudRunWorkerVariables(BaseVariables):
     """
-    <span class="badge-api experimental"/>
-
-    Infrastructure block used to run GCP Cloud Run Jobs.
+    Default variables for the Cloud Run worker.
 
-    Project name information is provided by the Credentials object, and should always
-    be correct as long as the Credentials object is for the correct project.
-
-    Note this block is experimental. The interface may change without notice.
+    The schema for this class is used to populate the `variables` section of the default
+    base job template.
     """
 
-    _block_type_slug = "cloud-run-job"
-    _block_type_name = "GCP Cloud Run Job"
-    _description = "Infrastructure block used to run GCP Cloud Run Jobs. Note this block is experimental. The interface may change without notice."  # noqa
-    _logo_url = "https://cdn.sanity.io/images/3ugk85nk/production/10424e311932e31c477ac2b9ef3d53cefbaad708-250x250.png"  # noqa
-    _documentation_url = "https://prefecthq.github.io/prefect-gcp/cloud_run/#prefect_gcp.cloud_run.CloudRunJob"  # noqa: E501
-
-    type: Literal["cloud-run-job"] = Field(
-        "cloud-run-job", description="The slug for this task type."
+    region: str = Field(
+        default="us-central1",
+        description="The region where the Cloud Run Job resides.",
+        examples=["us-central1"],
+    )
+    credentials: Optional[GcpCredentials] = Field(
+        title="GCP Credentials",
+        default_factory=GcpCredentials,
+        description="The GCP Credentials used to initiate the "
+        "Cloud Run Job. If not provided credentials will be "
+        "inferred from the local environment.",
     )
-    image: str = Field(
-        ...,
+    image: Optional[str] = Field(
+        default=None,
         title="Image Name",
         description=(
-            "The image to use for a new Cloud Run Job. This value must "
-            "refer to an image within either Google Container Registry "
-            "or Google Artifact Registry, like `gcr.io/<project_name>/<repo>/`."
+            "The image to use for a new Cloud Run Job. "
+            "If not set, the latest Prefect image will be used. "
+            "See https://cloud.google.com/run/docs/deploying#images."
         ),
+        examples=["docker.io/prefecthq/prefect:3-latest"],
     )
-    region: str = Field(..., description="The region where the Cloud Run Job resides.")
-    credentials: GcpCredentials  # cannot be Field; else it shows as Json
-
-    # Job settings
-    cpu: Optional[int] = Field(
+    cpu: Optional[str] = Field(
         default=None,
         title="CPU",
         description=(
             "The amount of compute allocated to the Cloud Run Job. "
-            "The int must be valid based on the rules specified at "
-            "https://cloud.google.com/run/docs/configuring/cpu#setting-jobs ."
+            "(1000m = 1 CPU). See "
+            "https://cloud.google.com/run/docs/configuring/cpu#setting-jobs."
         ),
+        examples=["1000m"],
+        pattern=r"^(\d*000)m$",
     )
-    memory: Optional[int] = Field(
+    memory: Optional[str] = Field(
         default=None,
         title="Memory",
-        description="The amount of memory allocated to the Cloud Run Job.",
-    )
-    memory_unit: Optional[Literal["G", "Gi", "M", "Mi"]] = Field(
-        default=None,
-        title="Memory Units",
         description=(
-            "The unit of memory. See "
-            "https://cloud.google.com/run/docs/configuring/memory-limits#setting "
-            "for additional details."
+            "The amount of memory allocated to the Cloud Run Job. "
+            "Must be specified in units of 'G', 'Gi', 'M', or 'Mi'. "
+            "See https://cloud.google.com/run/docs/configuring/memory-limits#setting."
         ),
+        examples=["512Mi"],
+        pattern=r"^\d+(?:G|Gi|M|Mi)$",
     )
     vpc_connector_name: Optional[str] = Field(
         default=None,
         title="VPC Connector Name",
         description="The name of the VPC connector to use for the Cloud Run Job.",
     )
-    args: Optional[List[str]] = Field(
+    service_account_name: Optional[str] = Field(
         default=None,
-        description=(
-            "Arguments to be passed to your Cloud Run Job's entrypoint command."
-        ),
-    )
-    env: Dict[str, str] = Field(
-        default_factory=dict,
-        description="Environment variables to be passed to your Cloud Run Job.",
+        title="Service Account Name",
+        description="The name of the service account to use for the task execution "
+        "of Cloud Run Job. By default Cloud Run jobs run as the default "
+        "Compute Engine Service Account. ",
+        examples=["service-account@example.iam.gserviceaccount.com"],
     )
-
-    # Cleanup behavior
     keep_job: Optional[bool] = Field(
         default=False,
         title="Keep Job After Completion",
-        description="Keep the completed Cloud Run Job on Google Cloud Platform.",
+        description="Keep the completed Cloud Run Job after it has run.",
     )
     timeout: Optional[int] = Field(
+        title="Job Timeout",
         default=600,
         gt=0,
         le=3600,
-        title="Job Timeout",
-        description=(
-            "The length of time that Prefect will wait for a Cloud Run Job to complete "
-            "before raising an exception."
-        ),
-    )
-    max_retries: Optional[int] = Field(
-        default=3,
-        ge=0,
-        le=10,
-        title="Max Retries",
         description=(
-            "The maximum retries setting specifies the number of times a task is "
-            "allowed to restart in case of failure before being failed permanently."
+            "The length of time that Prefect will wait for Cloud Run Job state changes."
         ),
     )
-    # For private use
-    _job_name: str = None
-    _execution: Optional[Execution] = None
-
-    @property
-    def job_name(self):
-        """Create a unique and valid job name."""
-
-        if self._job_name is None:
-            # get `repo` from `gcr.io/<project_name>/repo/other`
-            components = self.image.split("/")
-            image_name = components[2]
-            # only alphanumeric and '-' allowed for a job name
-            modified_image_name = image_name.replace(":", "-").replace(".", "-")
-            # make 50 char limit for final job name, which will be '<name>-<uuid>'
-            if len(modified_image_name) > 17:
-                modified_image_name = modified_image_name[:17]
-            name = f"{modified_image_name}-{uuid4().hex}"
-            self._job_name = name
-
-        return self._job_name
 
-    @property
-    def memory_string(self):
-        """Returns the string expected for memory resources argument."""
-        if self.memory and self.memory_unit:
-            return str(self.memory) + self.memory_unit
-        return None
-
-    @validator("image")
-    def _remove_image_spaces(cls, value):
-        """Deal with spaces in image names."""
-        if value is not None:
-            return value.strip()
-
-    @root_validator
-    def _check_valid_memory(cls, values):
-        """Make sure memory conforms to expected values for API.
-        See: https://cloud.google.com/run/docs/configuring/memory-limits#setting
-        """  # noqa
-        if (values.get("memory") is not None and values.get("memory_unit") is None) or (
-            values.get("memory_unit") is not None and values.get("memory") is None
-        ):
-            raise ValueError(
-                "A memory value and unit must both be supplied to specify a memory"
-                " value other than the default memory value."
-            )
-        return values
 
-    def get_corresponding_worker_type(self) -> str:
-        """Return the corresponding worker type for this infrastructure block."""
-        return "cloud-run"
+class CloudRunWorkerResult(BaseWorkerResult):
+    """Contains information about the final state of a completed process"""
 
-    async def generate_work_pool_base_job_template(self) -> dict:
-        """
-        Generate a base job template for a cloud-run work pool with the same
-        configuration as this block.
 
-        Returns:
-            - dict: a base job template for a cloud-run work pool
-        """
-        base_job_template = await get_default_base_job_template_for_infrastructure_type(
-            self.get_corresponding_worker_type(),
-        )
-        assert (
-            base_job_template is not None
-        ), "Failed to generate default base job template for Cloud Run worker."
-        for key, value in self.dict(exclude_unset=True, exclude_defaults=True).items():
-            if key == "command":
-                base_job_template["variables"]["properties"]["command"][
-                    "default"
-                ] = shlex.join(value)
-            elif key in [
-                "type",
-                "block_type_slug",
-                "_block_document_id",
-                "_block_document_name",
-                "_is_anonymous",
-                "memory_unit",
-            ]:
-                continue
-            elif key == "credentials":
-                if not self.credentials._block_document_id:
-                    raise BlockNotSavedError(
-                        "It looks like you are trying to use a block that"
-                        " has not been saved. Please call `.save` on your block"
-                        " before publishing it as a work pool."
-                    )
-                base_job_template["variables"]["properties"]["credentials"][
-                    "default"
-                ] = {
-                    "$ref": {
-                        "block_document_id": str(self.credentials._block_document_id)
-                    }
-                }
-            elif key == "memory" and self.memory_string:
-                base_job_template["variables"]["properties"]["memory"][
-                    "default"
-                ] = self.memory_string
-            elif key == "cpu" and self.cpu is not None:
-                base_job_template["variables"]["properties"]["cpu"][
-                    "default"
-                ] = f"{self.cpu * 1000}m"
-            elif key == "args":
-                # Not a default variable, but we can add it to the template
-                base_job_template["variables"]["properties"]["args"] = {
-                    "title": "Arguments",
-                    "type": "string",
-                    "description": "Arguments to be passed to your Cloud Run Job's entrypoint command.",  # noqa
-                    "default": value,
-                }
-                base_job_template["job_configuration"]["job_body"]["spec"]["template"][
-                    "spec"
-                ]["template"]["spec"]["containers"][0]["args"] = "{{ args }}"
-            elif key in base_job_template["variables"]["properties"]:
-                base_job_template["variables"]["properties"][key]["default"] = value
-            else:
-                self.logger.warning(
-                    f"Variable {key!r} is not supported by Cloud Run work pools."
-                    " Skipping."
-                )
+class CloudRunWorker(BaseWorker):
+    """Prefect worker that executes flow runs within Cloud Run Jobs."""
 
-        return base_job_template
+    type = "cloud-run"
+    job_configuration = CloudRunWorkerJobConfiguration
+    job_configuration_variables = CloudRunWorkerVariables
+    _description = (
+        "Execute flow runs within containers on Google Cloud Run. Requires "
+        "a Google Cloud Platform account."
+    )
+    _display_name = "Google Cloud Run"
+    _documentation_url = "https://prefecthq.github.io/prefect-gcp/cloud_run_worker/"
+    _logo_url = "https://cdn.sanity.io/images/3ugk85nk/production/10424e311932e31c477ac2b9ef3d53cefbaad708-250x250.png"  # noqa
 
-    def _create_job_error(self, exc):
+    def _create_job_error(self, exc, configuration):
         """Provides a nicer error for 404s when trying to create a Cloud Run Job."""
         # TODO consider lookup table instead of the if/else,
         # also check for documented errors
         if exc.status_code == 404:
             raise RuntimeError(
                 f"Failed to find resources at {exc.uri}. Confirm that region"
                 f" '{self.region}' is the correct region for your Cloud Run Job and"
-                f" that {self.credentials.project} is the correct GCP project. If"
+                f" that {configuration.project} is the correct GCP project. If"
                 f" your project ID is not correct, you are using a Credentials block"
                 f" with permissions for the wrong project."
             ) from exc
         raise exc
 
-    def _job_run_submission_error(self, exc):
+    def _job_run_submission_error(self, exc, configuration):
         """Provides a nicer error for 404s when submitting job runs."""
         if exc.status_code == 404:
             pat1 = r"The requested URL [^ ]+ was not found on this server"
             # pat2 = (
             #     r"Resource '[^ ]+' of kind 'JOB' in region '[\w\-0-9]+' "
             #     r"in project '[\w\-0-9]+' does not exist"
             # )
             if re.findall(pat1, str(exc)):
                 raise RuntimeError(
                     f"Failed to find resources at {exc.uri}. "
                     f"Confirm that region '{self.region}' is "
                     f"the correct region for your Cloud Run Job "
-                    f"and that '{self.credentials.project}' is the "
+                    f"and that '{configuration.project}' is the "
                     f"correct GCP project. If your project ID is not "
                     f"correct, you are using a Credentials "
                     f"block with permissions for the wrong project."
                 ) from exc
             else:
                 raise exc
 
         raise exc
 
-    def _cpu_as_k8s_quantity(self) -> str:
-        """Return the CPU integer in the format expected by GCP Cloud Run Jobs API.
-        See: https://kubernetes.io/docs/concepts/configuration/manage-resources-containers/
-        See also: https://cloud.google.com/run/docs/configuring/cpu#setting-jobs
-        """  # noqa
-        return str(self.cpu * 1000) + "m"
-
-    @sync_compatible
-    async def run(self, task_status: Optional[TaskStatus] = None):
-        """Run the configured job on a Google Cloud Run Job."""
-        with self._get_client() as client:
+    async def run(
+        self,
+        flow_run: "FlowRun",
+        configuration: CloudRunWorkerJobConfiguration,
+        task_status: Optional[anyio.abc.TaskStatus] = None,
+    ) -> CloudRunWorkerResult:
+        """
+        Executes a flow run within a Cloud Run Job and waits for the flow run
+        to complete.
+
+        Args:
+            flow_run: The flow run to execute
+            configuration: The configuration to use when executing the flow run.
+            task_status: The task status object for the current flow run. If provided,
+                the task will be marked as started.
+
+        Returns:
+            CloudRunWorkerResult: A result object containing information about the
+                final state of the flow run
+        """
+
+        logger = self.get_flow_run_logger(flow_run)
+
+        with self._get_client(configuration) as client:
             await run_sync_in_worker_thread(
-                self._create_job_and_wait_for_registration, client
+                self._create_job_and_wait_for_registration,
+                configuration,
+                client,
+                logger,
             )
             job_execution = await run_sync_in_worker_thread(
-                self._begin_job_execution, client
+                self._begin_job_execution, configuration, client, logger
             )
 
             if task_status:
-                task_status.started(self.job_name)
+                task_status.started(configuration.job_name)
 
             result = await run_sync_in_worker_thread(
                 self._watch_job_execution_and_get_result,
+                configuration,
                 client,
                 job_execution,
-                5,
+                logger,
             )
             return result
 
-    @sync_compatible
-    async def kill(self, identifier: str, grace_seconds: int = 30) -> None:
-        """
-        Kill a task running Cloud Run.
-
-        Args:
-            identifier: The Cloud Run Job name. This should match a
-                value yielded by CloudRunJob.run.
-        """
-        if grace_seconds != 30:
-            self.logger.warning(
-                f"Kill grace period of {grace_seconds}s requested, but GCP does not "
-                "support dynamic grace period configuration. See here for more info: "
-                "https://cloud.google.com/run/docs/reference/rest/v1/namespaces.jobs/delete"  # noqa
-            )
-
-        with self._get_client() as client:
-            await run_sync_in_worker_thread(
-                self._kill_job,
-                client=client,
-                namespace=self.credentials.project,
-                job_name=identifier,
-            )
+    def _get_client(self, configuration: CloudRunWorkerJobConfiguration) -> Resource:
+        """Get the base client needed for interacting with GCP APIs."""
+        # region needed for 'v1' API
+        api_endpoint = f"https://{configuration.region}-run.googleapis.com"
+        gcp_creds = configuration.credentials.get_credentials_from_service_account()
+        options = ClientOptions(api_endpoint=api_endpoint)
 
-    def _kill_job(self, client: Resource, namespace: str, job_name: str) -> None:
-        """
-        Thin wrapper around Job.delete, wrapping a try/except since
-        Job is an independent class that doesn't have knowledge of
-        CloudRunJob and its associated logic.
-        """
-        try:
-            Job.delete(client=client, namespace=namespace, job_name=job_name)
-        except Exception as exc:
-            if "does not exist" in str(exc):
-                raise InfrastructureNotFound(
-                    f"Cannot stop Cloud Run Job; the job name {job_name!r} "
-                    "could not be found."
-                ) from exc
-            raise
+        return discovery.build(
+            "run", "v1", client_options=options, credentials=gcp_creds
+        ).namespaces()
 
-    def _create_job_and_wait_for_registration(self, client: Resource) -> None:
+    def _create_job_and_wait_for_registration(
+        self,
+        configuration: CloudRunWorkerJobConfiguration,
+        client: Resource,
+        logger: PrefectLogAdapter,
+    ) -> None:
         """Create a new job wait for it to finish registering."""
         try:
-            self.logger.info(f"Creating Cloud Run Job {self.job_name}")
+            logger.info(f"Creating Cloud Run Job {configuration.job_name}")
+
             Job.create(
                 client=client,
-                namespace=self.credentials.project,
-                body=self._jobs_body(),
+                namespace=configuration.credentials.project,
+                body=configuration.job_body,
             )
         except googleapiclient.errors.HttpError as exc:
-            self._create_job_error(exc)
+            self._create_job_error(exc, configuration)
 
         try:
-            self._wait_for_job_creation(client=client, timeout=self.timeout)
+            self._wait_for_job_creation(
+                client=client, configuration=configuration, logger=logger
+            )
         except Exception:
-            self.logger.exception(
+            logger.exception(
                 "Encountered an exception while waiting for job run creation"
             )
-            if not self.keep_job:
-                self.logger.info(
-                    f"Deleting Cloud Run Job {self.job_name} from Google Cloud Run."
+            if not configuration.keep_job:
+                logger.info(
+                    f"Deleting Cloud Run Job {configuration.job_name} from "
+                    "Google Cloud Run."
                 )
                 try:
                     Job.delete(
                         client=client,
-                        namespace=self.credentials.project,
-                        job_name=self.job_name,
+                        namespace=configuration.credentials.project,
+                        job_name=configuration.job_name,
                     )
                 except Exception:
-                    self.logger.exception(
+                    logger.exception(
                         "Received an unexpected exception while attempting to delete"
-                        f" Cloud Run Job {self.job_name!r}"
+                        f" Cloud Run Job {configuration.job_name!r}"
                     )
             raise
 
-    def _begin_job_execution(self, client: Resource) -> Execution:
+    def _begin_job_execution(
+        self,
+        configuration: CloudRunWorkerJobConfiguration,
+        client: Resource,
+        logger: PrefectLogAdapter,
+    ) -> Execution:
         """Submit a job run for execution and return the execution object."""
         try:
-            self.logger.info(
-                f"Submitting Cloud Run Job {self.job_name!r} for execution."
+            logger.info(
+                f"Submitting Cloud Run Job {configuration.job_name!r} for execution."
             )
             submission = Job.run(
                 client=client,
-                namespace=self.credentials.project,
-                job_name=self.job_name,
+                namespace=configuration.project,
+                job_name=configuration.job_name,
             )
 
             job_execution = Execution.get(
                 client=client,
                 namespace=submission["metadata"]["namespace"],
                 execution_name=submission["metadata"]["name"],
             )
-
-            command = (
-                " ".join(self.command) if self.command else "default container command"
-            )
-
-            self.logger.info(
-                f"Cloud Run Job {self.job_name!r}: Running command {command!r}"
-            )
         except Exception as exc:
-            self._job_run_submission_error(exc)
+            self._job_run_submission_error(exc, configuration)
 
         return job_execution
 
     def _watch_job_execution_and_get_result(
-        self, client: Resource, execution: Execution, poll_interval: int
-    ) -> CloudRunJobResult:
+        self,
+        configuration: CloudRunWorkerJobConfiguration,
+        client: Resource,
+        execution: Execution,
+        logger: PrefectLogAdapter,
+        poll_interval: int = 5,
+    ) -> CloudRunWorkerResult:
         """Wait for execution to complete and then return result."""
         try:
             job_execution = self._watch_job_execution(
                 client=client,
                 job_execution=execution,
-                timeout=self.timeout,
+                timeout=configuration.timeout,
                 poll_interval=poll_interval,
             )
         except Exception:
-            self.logger.exception(
+            logger.exception(
                 "Received an unexpected exception while monitoring Cloud Run Job "
-                f"{self.job_name!r}"
+                f"{configuration.job_name!r}"
             )
             raise
 
         if job_execution.succeeded():
             status_code = 0
-            self.logger.info(f"Job Run {self.job_name} completed successfully")
+            logger.info(f"Job Run {configuration.job_name} completed successfully")
         else:
             status_code = 1
             error_msg = job_execution.condition_after_completion()["message"]
-            self.logger.error(
-                f"Job Run {self.job_name} did not complete successfully. {error_msg}"
+            logger.error(
+                "Job Run {configuration.job_name} did not complete successfully. "
+                f"{error_msg}"
             )
 
-        self.logger.info(
-            f"Job Run logs can be found on GCP at: {job_execution.log_uri}"
-        )
+        logger.info(f"Job Run logs can be found on GCP at: {job_execution.log_uri}")
 
-        if not self.keep_job:
-            self.logger.info(
-                f"Deleting completed Cloud Run Job {self.job_name!r} from Google Cloud"
-                " Run..."
+        if not configuration.keep_job:
+            logger.info(
+                f"Deleting completed Cloud Run Job {configuration.job_name!r} "
+                "from Google Cloud Run..."
             )
             try:
                 Job.delete(
                     client=client,
-                    namespace=self.credentials.project,
-                    job_name=self.job_name,
+                    namespace=configuration.project,
+                    job_name=configuration.job_name,
                 )
             except Exception:
-                self.logger.exception(
+                logger.exception(
                     "Received an unexpected exception while attempting to delete Cloud"
-                    f" Run Job {self.job_name}"
+                    f" Run Job {configuration.job_name}"
                 )
 
-        return CloudRunJobResult(identifier=self.job_name, status_code=status_code)
-
-    def _jobs_body(self) -> dict:
-        """Create properly formatted body used for a Job CREATE request.
-        See: https://cloud.google.com/run/docs/reference/rest/v1/namespaces.jobs
-        """
-        jobs_metadata = {"name": self.job_name}
-
-        annotations = {
-            # See: https://cloud.google.com/run/docs/troubleshooting#launch-stage-validation  # noqa
-            "run.googleapis.com/launch-stage": "BETA",
-        }
-        # add vpc connector if specified
-        if self.vpc_connector_name:
-            annotations[
-                "run.googleapis.com/vpc-access-connector"
-            ] = self.vpc_connector_name
-
-        # env and command here
-        containers = [self._add_container_settings({"image": self.image})]
-
-        # apply this timeout to each task
-        timeout_seconds = str(self.timeout)
-
-        body = {
-            "apiVersion": "run.googleapis.com/v1",
-            "kind": "Job",
-            "metadata": jobs_metadata,
-            "spec": {  # JobSpec
-                "template": {  # ExecutionTemplateSpec
-                    "metadata": {"annotations": annotations},
-                    "spec": {  # ExecutionSpec
-                        "template": {  # TaskTemplateSpec
-                            "spec": {
-                                "containers": containers,
-                                "timeoutSeconds": timeout_seconds,
-                                "maxRetries": self.max_retries,
-                            }  # TaskSpec
-                        }
-                    },
-                }
-            },
-        }
-        return body
-
-    def preview(self) -> str:
-        """Generate a preview of the job definition that will be sent to GCP."""
-        body = self._jobs_body()
-        container_settings = body["spec"]["template"]["spec"]["template"]["spec"][
-            "containers"
-        ][0]["env"]
-        body["spec"]["template"]["spec"]["template"]["spec"]["containers"][0]["env"] = [
-            container_setting
-            for container_setting in container_settings
-            if container_setting["name"] != "PREFECT_API_KEY"
-        ]
-        return json.dumps(body, indent=2)
+        return CloudRunWorkerResult(
+            identifier=configuration.job_name, status_code=status_code
+        )
 
     def _watch_job_execution(
         self, client, job_execution: Execution, timeout: int, poll_interval: int = 5
     ):
         """
         Update job_execution status until it is no longer running or timeout is reached.
         """
@@ -746,107 +787,81 @@
                 )
 
             time.sleep(poll_interval)
 
         return job_execution
 
     def _wait_for_job_creation(
-        self, client: Resource, timeout: int, poll_interval: int = 5
+        self,
+        client: Resource,
+        configuration: CloudRunWorkerJobConfiguration,
+        logger: PrefectLogAdapter,
+        poll_interval: int = 5,
     ):
         """Give created job time to register."""
         job = Job.get(
-            client=client, namespace=self.credentials.project, job_name=self.job_name
+            client=client,
+            namespace=configuration.project,
+            job_name=configuration.job_name,
         )
 
         t0 = time.time()
         while not job.is_ready():
             ready_condition = (
                 job.ready_condition
                 if job.ready_condition
                 else "waiting for condition update"
             )
-            self.logger.info(
-                f"Job is not yet ready... Current condition: {ready_condition}"
-            )
+            logger.info(f"Job is not yet ready... Current condition: {ready_condition}")
             job = Job.get(
                 client=client,
-                namespace=self.credentials.project,
-                job_name=self.job_name,
+                namespace=configuration.project,
+                job_name=configuration.job_name,
             )
 
             elapsed_time = time.time() - t0
-            if timeout is not None and elapsed_time > timeout:
+            if (
+                configuration.timeout is not None
+                and elapsed_time > configuration.timeout
+            ):
                 raise RuntimeError(
                     f"Timed out after {elapsed_time}s while waiting for Cloud Run Job "
                     "execution to complete. Your job may still be running on GCP."
                 )
 
             time.sleep(poll_interval)
 
-    def _get_client(self) -> Resource:
-        """Get the base client needed for interacting with GCP APIs."""
-        # region needed for 'v1' API
-        api_endpoint = f"https://{self.region}-run.googleapis.com"
-        gcp_creds = self.credentials.get_credentials_from_service_account()
-        options = ClientOptions(api_endpoint=api_endpoint)
+    async def kill_infrastructure(
+        self,
+        infrastructure_pid: str,
+        configuration: CloudRunWorkerJobConfiguration,
+        grace_seconds: int = 30,
+    ):
+        """
+        Stops a job for a cancelled flow run based on the provided infrastructure PID
+        and run configuration.
+        """
+        if grace_seconds != 30:
+            self._logger.warning(
+                f"Kill grace period of {grace_seconds}s requested, but GCP does not "
+                "support dynamic grace period configuration. See here for more info: "
+                "https://cloud.google.com/run/docs/reference/rest/v1/namespaces.jobs/delete"  # noqa
+            )
 
-        return discovery.build(
-            "run", "v1", client_options=options, credentials=gcp_creds
-        ).namespaces()
+        with self._get_client(configuration) as client:
+            await run_sync_in_worker_thread(
+                self._stop_job,
+                client=client,
+                namespace=configuration.project,
+                job_name=infrastructure_pid,
+            )
 
-    # CONTAINER SETTINGS
-    def _add_container_settings(self, base_settings: Dict[str, Any]) -> Dict[str, Any]:
-        """
-        Add settings related to containers for Cloud Run Jobs to a dictionary.
-        Includes environment variables, entrypoint command, entrypoint arguments,
-        and cpu and memory limits.
-        See: https://cloud.google.com/run/docs/reference/rest/v1/Container
-        and https://cloud.google.com/run/docs/reference/rest/v1/Container#ResourceRequirements
-        """  # noqa
-        container_settings = base_settings.copy()
-        container_settings.update(self._add_env())
-        container_settings.update(self._add_resources())
-        container_settings.update(self._add_command())
-        container_settings.update(self._add_args())
-        return container_settings
-
-    def _add_args(self) -> dict:
-        """Set the arguments that will be passed to the entrypoint for a Cloud Run Job.
-        See: https://cloud.google.com/run/docs/reference/rest/v1/Container
-        """  # noqa
-        return {"args": self.args} if self.args else {}
-
-    def _add_command(self) -> dict:
-        """Set the command that a container will run for a Cloud Run Job.
-        See: https://cloud.google.com/run/docs/reference/rest/v1/Container
-        """  # noqa
-        return {"command": self.command}
-
-    def _add_resources(self) -> dict:
-        """Set specified resources limits for a Cloud Run Job.
-        See: https://cloud.google.com/run/docs/reference/rest/v1/Container#ResourceRequirements
-        See also: https://kubernetes.io/docs/concepts/configuration/manage-resources-containers/
-        """  # noqa
-        resources = {"limits": {}, "requests": {}}
-
-        if self.cpu is not None:
-            cpu = self._cpu_as_k8s_quantity()
-            resources["limits"]["cpu"] = cpu
-            resources["requests"]["cpu"] = cpu
-        if self.memory_string is not None:
-            resources["limits"]["memory"] = self.memory_string
-            resources["requests"]["memory"] = self.memory_string
-
-        return {"resources": resources} if resources["requests"] else {}
-
-    def _add_env(self) -> dict:
-        """Add environment variables for a Cloud Run Job.
-
-        Method `self._base_environment()` gets necessary Prefect environment variables
-        from the config.
-
-        See: https://cloud.google.com/run/docs/reference/rest/v1/Container#envvar for
-        how environment variables are specified for Cloud Run Jobs.
-        """  # noqa
-        env = {**self._base_environment(), **self.env}
-        cloud_run_env = [{"name": k, "value": v} for k, v in env.items()]
-        return {"env": cloud_run_env}
+    def _stop_job(self, client: Resource, namespace: str, job_name: str):
+        try:
+            Job.delete(client=client, namespace=namespace, job_name=job_name)
+        except Exception as exc:
+            if "does not exist" in str(exc):
+                raise InfrastructureNotFound(
+                    f"Cannot stop Cloud Run Job; the job name {job_name!r} "
+                    "could not be found."
+                ) from exc
+            raise
```

### Comparing `prefect_gcp-0.5.9/prefect_gcp/cloud_storage.py` & `prefect_gcp-0.6.0rc1/prefect_gcp/cloud_storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,28 +3,23 @@
 import asyncio
 import os
 from enum import Enum
 from io import BytesIO
 from pathlib import Path, PurePosixPath
 from typing import Any, BinaryIO, Dict, List, Optional, Tuple, Union
 
-from pydantic import VERSION as PYDANTIC_VERSION
+from pydantic import Field, field_validator
 
 from prefect import get_run_logger, task
 from prefect.blocks.abstract import ObjectStorageBlock
 from prefect.filesystems import WritableDeploymentStorage, WritableFileSystem
 from prefect.logging import disable_run_logger
 from prefect.utilities.asyncutils import run_sync_in_worker_thread, sync_compatible
 from prefect.utilities.filesystem import filter_files
 
-if PYDANTIC_VERSION.startswith("2."):
-    from pydantic.v1 import Field, validator
-else:
-    from pydantic import Field, validator
-
 # cannot be type_checking only or else `fields = cls.schema()` raises
 # TypeError: issubclass() arg 1 must be a class
 from prefect_gcp.credentials import GcpCredentials
 
 try:
     from pandas import DataFrame
 except ModuleNotFoundError:
@@ -34,14 +29,15 @@
     from google.cloud.storage import Bucket
     from google.cloud.storage.blob import Blob
 except ModuleNotFoundError:
     pass
 
 
 @task
+@sync_compatible
 async def cloud_storage_create_bucket(
     bucket: str,
     gcp_credentials: GcpCredentials,
     project: Optional[str] = None,
     location: Optional[str] = None,
     **create_kwargs: Dict[str, Any],
 ) -> str:
@@ -81,28 +77,42 @@
     client = gcp_credentials.get_cloud_storage_client(project=project)
     await run_sync_in_worker_thread(
         client.create_bucket, bucket, location=location, **create_kwargs
     )
     return bucket
 
 
-async def _get_bucket(
+async def _get_bucket_async(
     bucket: str,
     gcp_credentials: GcpCredentials,
     project: Optional[str] = None,
 ) -> "Bucket":
     """
     Helper function to retrieve a bucket.
     """
     client = gcp_credentials.get_cloud_storage_client(project=project)
     bucket_obj = await run_sync_in_worker_thread(client.get_bucket, bucket)
     return bucket_obj
 
 
+def _get_bucket(
+    bucket: str,
+    gcp_credentials: GcpCredentials,
+    project: Optional[str] = None,
+) -> "Bucket":
+    """
+    Helper function to retrieve a bucket.
+    """
+    client = gcp_credentials.get_cloud_storage_client(project=project)
+    bucket_obj = client.get_bucket(bucket)
+    return bucket_obj
+
+
 @task
+@sync_compatible
 async def cloud_storage_download_blob_as_bytes(
     bucket: str,
     blob: str,
     gcp_credentials: GcpCredentials,
     chunk_size: Optional[int] = None,
     encryption_key: Optional[str] = None,
     timeout: Union[float, Tuple[float, float]] = 60,
@@ -148,26 +158,27 @@
 
         example_cloud_storage_download_blob_flow()
         ```
     """
     logger = get_run_logger()
     logger.info("Downloading blob named %s from the %s bucket", blob, bucket)
 
-    bucket_obj = await _get_bucket(bucket, gcp_credentials, project=project)
+    bucket_obj = await _get_bucket_async(bucket, gcp_credentials, project=project)
     blob_obj = bucket_obj.blob(
         blob, chunk_size=chunk_size, encryption_key=encryption_key
     )
 
     contents = await run_sync_in_worker_thread(
         blob_obj.download_as_bytes, timeout=timeout, **download_kwargs
     )
     return contents
 
 
 @task
+@sync_compatible
 async def cloud_storage_download_blob_to_file(
     bucket: str,
     blob: str,
     path: Union[str, Path],
     gcp_credentials: GcpCredentials,
     chunk_size: Optional[int] = None,
     encryption_key: Optional[str] = None,
@@ -218,15 +229,15 @@
         ```
     """
     logger = get_run_logger()
     logger.info(
         "Downloading blob named %s from the %s bucket to %s", blob, bucket, path
     )
 
-    bucket_obj = await _get_bucket(bucket, gcp_credentials, project=project)
+    bucket_obj = await _get_bucket_async(bucket, gcp_credentials, project=project)
     blob_obj = bucket_obj.blob(
         blob, chunk_size=chunk_size, encryption_key=encryption_key
     )
 
     if os.path.isdir(path):
         if isinstance(path, Path):
             path = path.joinpath(blob)  # keep as Path if Path is passed
@@ -236,14 +247,15 @@
     await run_sync_in_worker_thread(
         blob_obj.download_to_filename, path, timeout=timeout, **download_kwargs
     )
     return path
 
 
 @task
+@sync_compatible
 async def cloud_storage_upload_blob_from_string(
     data: Union[str, bytes],
     bucket: str,
     blob: str,
     gcp_credentials: GcpCredentials,
     content_type: Optional[str] = None,
     chunk_size: Optional[int] = None,
@@ -293,15 +305,15 @@
 
         example_cloud_storage_upload_blob_from_string_flow()
         ```
     """
     logger = get_run_logger()
     logger.info("Uploading blob named %s to the %s bucket", blob, bucket)
 
-    bucket_obj = await _get_bucket(bucket, gcp_credentials, project=project)
+    bucket_obj = await _get_bucket_async(bucket, gcp_credentials, project=project)
     blob_obj = bucket_obj.blob(
         blob, chunk_size=chunk_size, encryption_key=encryption_key
     )
 
     await run_sync_in_worker_thread(
         blob_obj.upload_from_string,
         data,
@@ -309,14 +321,15 @@
         timeout=timeout,
         **upload_kwargs,
     )
     return blob
 
 
 @task
+@sync_compatible
 async def cloud_storage_upload_blob_from_file(
     file: Union[str, Path, BytesIO],
     bucket: str,
     blob: str,
     gcp_credentials: GcpCredentials,
     content_type: Optional[str] = None,
     chunk_size: Optional[int] = None,
@@ -368,15 +381,15 @@
 
         example_cloud_storage_upload_blob_from_file_flow()
         ```
     """
     logger = get_run_logger()
     logger.info("Uploading blob named %s to the %s bucket", blob, bucket)
 
-    bucket_obj = await _get_bucket(bucket, gcp_credentials, project=project)
+    bucket_obj = await _get_bucket_async(bucket, gcp_credentials, project=project)
     blob_obj = bucket_obj.blob(
         blob, chunk_size=chunk_size, encryption_key=encryption_key
     )
 
     if isinstance(file, BytesIO):
         await run_sync_in_worker_thread(
             blob_obj.upload_from_file,
@@ -393,15 +406,15 @@
             timeout=timeout,
             **upload_kwargs,
         )
     return blob
 
 
 @task
-async def cloud_storage_copy_blob(
+def cloud_storage_copy_blob(
     source_bucket: str,
     dest_bucket: str,
     source_blob: str,
     gcp_credentials: GcpCredentials,
     dest_blob: Optional[str] = None,
     timeout: Union[float, Tuple[float, float]] = 60,
     project: Optional[str] = None,
@@ -454,32 +467,28 @@
     logger.info(
         "Copying blob named %s from the %s bucket to the %s bucket",
         source_blob,
         source_bucket,
         dest_bucket,
     )
 
-    source_bucket_obj = await _get_bucket(
-        source_bucket, gcp_credentials, project=project
-    )
+    source_bucket_obj = _get_bucket(source_bucket, gcp_credentials, project=project)
 
-    dest_bucket_obj = await _get_bucket(dest_bucket, gcp_credentials, project=project)
+    dest_bucket_obj = _get_bucket(dest_bucket, gcp_credentials, project=project)
     if dest_blob is None:
         dest_blob = source_blob
 
     source_blob_obj = source_bucket_obj.blob(source_blob)
-    await run_sync_in_worker_thread(
-        source_bucket_obj.copy_blob,
+    source_bucket_obj.copy_blob(
         blob=source_blob_obj,
         destination_bucket=dest_bucket_obj,
         new_name=dest_blob,
         timeout=timeout,
         **copy_kwargs,
     )
-
     return dest_blob
 
 
 class DataFrameSerializationFormat(Enum):
     """
     An enumeration class to represent different file formats,
     compression options for upload_from_dataframe
@@ -592,15 +601,16 @@
         """
         Read-only property that mirrors the bucket folder.
 
         Used for deployment.
         """
         return self.bucket_folder
 
-    @validator("bucket_folder", pre=True, always=True)
+    @field_validator("bucket_folder")
+    @classmethod
     def _bucket_folder_suffix(cls, value):
         """
         Ensures that the bucket folder is suffixed with a forward slash.
         """
         if value != "" and not value.endswith("/"):
             value = f"{value}/"
         return value
@@ -717,15 +727,15 @@
                 ignore_patterns = f.readlines()
             included_files = filter_files(local_path, ignore_patterns)
 
         uploaded_file_count = 0
         for local_file_path in Path(local_path).rglob("*"):
             if (
                 included_files is not None
-                and local_file_path.name not in included_files
+                and str(local_file_path.relative_to(local_path)) not in included_files
             ):
                 continue
             elif not local_file_path.is_dir():
                 remote_file_path = str(
                     PurePosixPath(to_path, local_file_path.relative_to(local_path))
                 )
                 local_file_content = local_file_path.read_bytes()
```

### Comparing `prefect_gcp-0.5.9/prefect_gcp/credentials.py` & `prefect_gcp-0.6.0rc1/prefect_gcp/credentials.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,23 @@
 """Module handling GCP credentials."""
 
 import functools
 import json
 from enum import Enum
 from pathlib import Path
+from threading import Lock
 from typing import Any, Dict, Optional, Union
 
 import google.auth
 import google.auth.transport.requests
 from google.oauth2.service_account import Credentials
-from pydantic import VERSION as PYDANTIC_VERSION
+from pydantic import Field, field_validator, model_validator
 
 from prefect.blocks.abstract import CredentialsBlock
-from prefect.blocks.fields import SecretDict
-from prefect.utilities.asyncutils import run_sync_in_worker_thread, sync_compatible
-
-if PYDANTIC_VERSION.startswith("2."):
-    from pydantic.v1 import Field, root_validator, validator
-else:
-    from pydantic import Field, root_validator, validator
+from prefect.types import SecretDict
 
 try:
     from google.cloud.bigquery import Client as BigQueryClient
 except ModuleNotFoundError:
     pass  # will be raised in get_client
 
 try:
@@ -32,18 +27,25 @@
 
 try:
     from google.cloud.storage import Client as StorageClient
 except ModuleNotFoundError:
     pass
 
 try:
-    from google.cloud.aiplatform.gapic import JobServiceClient
+    from google.cloud.aiplatform.gapic import JobServiceAsyncClient, JobServiceClient
+except ModuleNotFoundError:
+    pass
+
+try:
+    from google.api_core.client_options import ClientOptions, from_dict
 except ModuleNotFoundError:
     pass
 
+_LOCK = Lock()
+
 
 def _raise_help_msg(key: str):
     """
     Raises a helpful error message.
 
     Args:
         key: the key to access HELP_URLS
@@ -75,14 +77,33 @@
 class ClientType(Enum):
     CLOUD_STORAGE = "cloud_storage"
     BIGQUERY = "bigquery"
     SECRET_MANAGER = "secret_manager"
     AIPLATFORM = "job_service"  # vertex ai
 
 
+@functools.lru_cache(maxsize=8, typed=True)
+def _get_job_service_async_client_cached(
+    ctx, client_options: tuple
+) -> "JobServiceAsyncClient":
+    """
+    Gets an authenticated Job Service async client for Vertex AI.
+
+    Returns:
+        An authenticated Job Service async client.
+    """
+    with _LOCK:
+        client_options = dict(client_options)
+        credentials = ctx.get_credentials_from_service_account()
+        job_service_client = JobServiceAsyncClient(
+            credentials=credentials, client_options=client_options
+        )
+    return job_service_client
+
+
 class GcpCredentials(CredentialsBlock):
     """
     Block used to manage authentication with GCP. Google authentication is
     handled via the `google.oauth2` module or through the CLI.
     Specify either one of service `account_file` or `service_account_info`; if both
     are not specified, the client will try to detect the credentials following Google's
     [Application Default Credentials](https://cloud.google.com/docs/authentication/application-default-credentials).
@@ -113,42 +134,52 @@
     )
     project: Optional[str] = Field(
         default=None, description="The GCP project to use for the client."
     )
 
     _service_account_email: Optional[str] = None
 
-    @root_validator
-    def _provide_one_service_account_source(cls, values):
+    def __hash__(self):
+        return hash(
+            (
+                hash(self.service_account_file),
+                hash(frozenset(self.service_account_info.get_secret_value().items()))
+                if self.service_account_info
+                else None,
+                hash(self.project),
+                hash(self._service_account_email),
+            )
+        )
+
+    @model_validator(mode="after")
+    def _provide_one_service_account_source(self):
         """
         Ensure that only a service account file or service account info ias provided.
         """
-        both_service_account = (
-            values.get("service_account_info") is not None
-            and values.get("service_account_file") is not None
-        )
-        if both_service_account:
+        if self.service_account_info and self.service_account_file:
             raise ValueError(
                 "Only one of service_account_info or service_account_file "
                 "can be specified at once"
             )
-        return values
+        return self
 
-    @validator("service_account_file")
+    @field_validator("service_account_file")
+    @classmethod
     def _check_service_account_file(cls, file):
         """Get full path of provided file and make sure that it exists."""
         if not file:
             return file
 
         service_account_file = Path(file).expanduser()
         if not service_account_file.exists():
             raise ValueError("The provided path to the service account is invalid")
         return service_account_file
 
-    @validator("service_account_info", pre=True)
+    @field_validator("service_account_info", mode="before")
+    @classmethod
     def _convert_json_string_json_service_account_info(cls, value):
         """
         Converts service account info provided as a json formatted string
         to a dictionary
         """
         if isinstance(value, str):
             try:
@@ -190,23 +221,22 @@
                 self.service_account_file,
                 scopes=["https://www.googleapis.com/auth/cloud-platform"],
             )
         else:
             credentials, _ = google.auth.default()
         return credentials
 
-    @sync_compatible
-    async def get_access_token(self):
+    def get_access_token(self):
         """
         See: https://stackoverflow.com/a/69107745
         Also: https://www.jhanley.com/google-cloud-creating-oauth-access-tokens-for-rest-api-calls/
         """  # noqa
         request = google.auth.transport.requests.Request()
         credentials = self.get_credentials_from_service_account()
-        await run_sync_in_worker_thread(credentials.refresh, request)
+        credentials.refresh(request)
         return credentials.token
 
     def get_client(
         self,
         client_type: Union[str, ClientType],
         **get_client_kwargs: Dict[str, Any],
     ) -> Any:
@@ -408,15 +438,15 @@
 
         # doesn't accept project; must pass in project in tasks
         secret_manager_client = SecretManagerServiceClient(credentials=credentials)
         return secret_manager_client
 
     @_raise_help_msg("aiplatform")
     def get_job_service_client(
-        self, client_options: Dict[str, Any] = None
+        self, client_options: Union[Dict[str, Any], ClientOptions] = None
     ) -> "JobServiceClient":
         """
         Gets an authenticated Job Service client for Vertex AI.
 
         Returns:
             An authenticated Job Service client.
 
@@ -458,12 +488,71 @@
                 client = GcpCredentials(
                     service_account_info=service_account_info
                 ).get_job_service_client()
 
             example_get_client_flow()
             ```
         """
+        if isinstance(client_options, dict):
+            client_options = from_dict(client_options)
+
         credentials = self.get_credentials_from_service_account()
-        job_service_client = JobServiceClient(
-            credentials=credentials, client_options=client_options
+        return JobServiceClient(credentials=credentials, client_options=client_options)
+
+    @_raise_help_msg("aiplatform")
+    def get_job_service_async_client(
+        self, client_options: Union[Dict[str, Any], ClientOptions] = None
+    ) -> "JobServiceAsyncClient":
+        """
+        Gets an authenticated Job Service async client for Vertex AI.
+
+        Returns:
+            An authenticated Job Service async client.
+
+        Examples:
+            Gets a GCP Job Service client from a path.
+            ```python
+            from prefect import flow
+            from prefect_gcp.credentials import GcpCredentials
+
+            @flow()
+            def example_get_client_flow():
+                service_account_file = "~/.secrets/prefect-service-account.json"
+                client = GcpCredentials(
+                    service_account_file=service_account_file
+                ).get_job_service_async_client()
+
+            example_get_client_flow()
+            ```
+
+            Gets a GCP Cloud Storage client from a dictionary.
+            ```python
+            from prefect import flow
+            from prefect_gcp.credentials import GcpCredentials
+
+            @flow()
+            def example_get_client_flow():
+                service_account_info = {
+                    "type": "service_account",
+                    "project_id": "project_id",
+                    "private_key_id": "private_key_id",
+                    "private_key": "private_key",
+                    "client_email": "client_email",
+                    "client_id": "client_id",
+                    "auth_uri": "auth_uri",
+                    "token_uri": "token_uri",
+                    "auth_provider_x509_cert_url": "auth_provider_x509_cert_url",
+                    "client_x509_cert_url": "client_x509_cert_url"
+                }
+                client = GcpCredentials(
+                    service_account_info=service_account_info
+                ).get_job_service_async_client()
+
+            example_get_client_flow()
+            ```
+        """
+        if isinstance(client_options, dict):
+            client_options = from_dict(client_options)
+
+        return _get_job_service_async_client_cached(
+            self, tuple(client_options.__dict__.items())
         )
-        return job_service_client
```

### Comparing `prefect_gcp-0.5.9/prefect_gcp/deployments/steps.py` & `prefect_gcp-0.6.0rc1/prefect_gcp/deployments/steps.py`

 * *Files identical despite different names*

### Comparing `prefect_gcp-0.5.9/prefect_gcp/models/cloud_run_v2.py` & `prefect_gcp-0.6.0rc1/prefect_gcp/models/cloud_run_v2.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,60 +1,53 @@
 import time
 from typing import Dict, List, Literal, Optional
 
 # noinspection PyProtectedMember
 from googleapiclient.discovery import Resource
-from pydantic import VERSION as PYDANTIC_VERSION
-
-from prefect.infrastructure.base import InfrastructureResult
-
-if PYDANTIC_VERSION.startswith("2."):
-    from pydantic.v1 import BaseModel
-else:
-    from pydantic import BaseModel
+from pydantic import BaseModel, Field
 
 
 class JobV2(BaseModel):
     """
     JobV2 is a data model for a job that will be run on Cloud Run with the V2 API.
     """
 
     name: str
     uid: str
     generation: str
-    labels: Dict[str, str]
-    annotations: Dict[str, str]
+    labels: Dict[str, str] = Field(default_factory=dict)
+    annotations: Dict[str, str] = Field(default_factory=dict)
     createTime: str
     updateTime: str
-    deleteTime: Optional[str]
-    expireTime: Optional[str]
-    creator: Optional[str]
-    lastModifier: Optional[str]
-    client: Optional[str]
-    clientVersion: Optional[str]
+    deleteTime: Optional[str] = Field(None)
+    expireTime: Optional[str] = Field(None)
+    creator: Optional[str] = Field(None)
+    lastModifier: Optional[str] = Field(None)
+    client: Optional[str] = Field(None)
+    clientVersion: Optional[str] = Field(None)
     launchStage: Literal[
         "ALPHA",
         "BETA",
         "GA",
         "DEPRECATED",
         "EARLY_ACCESS",
         "PRELAUNCH",
         "UNIMPLEMENTED",
         "LAUNCH_TAG_UNSPECIFIED",
     ]
-    binaryAuthorization: Dict
-    template: Dict
-    observedGeneration: Optional[str]
-    terminalCondition: Dict
-    conditions: List[Dict]
+    binaryAuthorization: Dict = Field(default_factory=dict)
+    template: Dict = Field(default_factory=dict)
+    observedGeneration: Optional[str] = Field(None)
+    terminalCondition: Dict = Field(default_factory=dict)
+    conditions: List[Dict] = Field(default_factory=list)
     executionCount: int
-    latestCreatedExecution: Dict
-    reconciling: bool
-    satisfiesPzs: bool
-    etag: str
+    latestCreatedExecution: Dict = Field(default_factory=dict)
+    reconciling: bool = Field(False)
+    satisfiesPzs: bool = Field(False)
+    etag: Optional[str] = Field(None)
 
     def is_ready(self) -> bool:
         """
         Check if the job is ready to run.
 
         Returns:
             Whether the job is ready to run.
@@ -386,9 +379,9 @@
             retriedCount=response.get("retriedCount"),
             logUri=response["logUri"],
             satisfiesPzs=response.get("satisfiesPzs", False),
             etag=response["etag"],
         )
 
 
-class CloudRunJobV2Result(InfrastructureResult):
+class CloudRunJobV2Result:
     """Result from a Cloud Run Job."""
```

### Comparing `prefect_gcp-0.5.9/prefect_gcp/secret_manager.py` & `prefect_gcp-0.6.0rc1/prefect_gcp/secret_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,17 @@
 from functools import partial
 from typing import Optional, Union
 
 from anyio import to_thread
 from google.api_core.exceptions import NotFound
-from pydantic import VERSION as PYDANTIC_VERSION
+from pydantic import Field
 
 from prefect import get_run_logger, task
 from prefect.blocks.abstract import SecretBlock
 from prefect.utilities.asyncutils import run_sync_in_worker_thread, sync_compatible
-
-if PYDANTIC_VERSION.startswith("2."):
-    from pydantic.v1 import Field
-else:
-    from pydantic import Field
-
 from prefect_gcp.credentials import GcpCredentials
 
 try:
     from google.cloud.secretmanager_v1.types.resources import (
         Replication,
         Secret,
         SecretPayload,
@@ -29,14 +23,15 @@
         DeleteSecretRequest,
     )
 except ModuleNotFoundError:
     pass
 
 
 @task
+@sync_compatible
 async def create_secret(
     secret_name: str,
     gcp_credentials: "GcpCredentials",
     timeout: float = 60,
     project: Optional[str] = None,
 ) -> str:
     """
@@ -85,14 +80,15 @@
         timeout=timeout,
     )
     response = await to_thread.run_sync(partial_create)
     return response.name
 
 
 @task
+@sync_compatible
 async def update_secret(
     secret_name: str,
     secret_value: Union[str, bytes],
     gcp_credentials: "GcpCredentials",
     timeout: float = 60,
     project: Optional[str] = None,
 ) -> str:
@@ -142,14 +138,15 @@
         timeout=timeout,
     )
     response = await to_thread.run_sync(partial_add)
     return response.name
 
 
 @task
+@sync_compatible
 async def read_secret(
     secret_name: str,
     gcp_credentials: "GcpCredentials",
     version_id: Union[str, int] = "latest",
     timeout: float = 60,
     project: Optional[str] = None,
 ) -> str:
@@ -192,14 +189,15 @@
     partial_access = partial(client.access_secret_version, name=name, timeout=timeout)
     response = await to_thread.run_sync(partial_access)
     secret = response.payload.data.decode("UTF-8")
     return secret
 
 
 @task
+@sync_compatible
 async def delete_secret(
     secret_name: str,
     gcp_credentials: "GcpCredentials",
     timeout: float = 60,
     project: Optional[str] = None,
 ) -> str:
     """
@@ -240,14 +238,15 @@
     name = f"projects/{project}/secrets/{secret_name}/"
     partial_delete = partial(client.delete_secret, name=name, timeout=timeout)
     await to_thread.run_sync(partial_delete)
     return name
 
 
 @task
+@sync_compatible
 async def delete_secret_version(
     secret_name: str,
     version_id: int,
     gcp_credentials: "GcpCredentials",
     timeout: float = 60,
     project: Optional[str] = None,
 ) -> str:
```

### Comparing `prefect_gcp-0.5.9/prefect_gcp/workers/cloud_run.py` & `prefect_gcp-0.6.0rc1/prefect_gcp/workers/cloud_run_v2.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,324 +1,158 @@
-""" <!-- # noqa -->
-
-Module containing the Cloud Run worker used for executing flow runs as Cloud Run jobs.
-
-Get started by creating a Cloud Run work pool:
-
-```bash
-prefect work-pool create 'my-cloud-run-pool' --type cloud-run
-```
-
-Then start a Cloud Run worker with the following command:
-
-```bash
-prefect worker start --pool 'my-cloud-run-pool'
-```
-
-## Configuration
-Read more about configuring work pools
-[here](https://docs.prefect.io/latest/concepts/work-pools/#work-pool-overview).
-
-## Advanced Configuration
-!!! example "Using a custom Cloud Run job template"
-    Below is the default job body template used by the Cloud Run Worker:
-    ```json
-    {
-        "apiVersion": "run.googleapis.com/v1",
-        "kind": "Job",
-        "metadata":
-            {
-                "name": "{{ name }}",
-                "annotations":
-                {
-                    "run.googleapis.com/launch-stage": "BETA",
-                }
-            },
-            "spec":
-            {
-                "template":
-                {
-                    "spec":
-                    {
-                        "template":
-                        {
-                            "spec":
-                            {
-                                "containers":
-                                [
-                                    {
-                                        "image": "{{ image }}",
-                                        "args": "{{ args }}",
-                                        "resources":
-                                        {
-                                            "limits":
-                                            {
-                                                "cpu": "{{ cpu }}",
-                                                "memory": "{{ memory }}"
-                                            },
-                                            "requests":
-                                            {
-                                                "cpu": "{{ cpu }}",
-                                                "memory": "{{ memory }}"
-                                            }
-                                        }
-                                    }
-                                ],
-                                "timeoutSeconds": "{{ timeout }}",
-                                "serviceAccountName": "{{ service_account_name }}"
-                            }
-                        }
-                    }
-                    }
-                },
-                "metadata":
-                {
-                    "annotations":
-                    {
-                        "run.googleapis.com/vpc-access-connector": "{{ vpc_connector_name }}"
-                    }
-                }
-            },
-        },
-        "timeout": "{{ timeout }}",
-        "keep_job": "{{ keep_job }}"
-    }
-    ```
-    Each values enclosed in `{{ }}` is a placeholder that will be replaced with
-    a value at runtime on a per-deployment basis. The values that can be used a
-    placeholders are defined by the `variables` schema defined in the base job template.
-
-    The default job body template and available variables can be customized on a work pool
-    by work pool basis. By editing the default job body template you can:
-
-    - Add additional placeholders to the default job template
-    - Remove placeholders from the default job template
-    - Pass values to Cloud Run that are not defined in the `variables` schema
-
-    ### Adding additional placeholders
-    For example, to allow for extra customization of a new annotation not described in
-    the default job template, you can add the following:
-    ```json
-    {
-        "apiVersion": "run.googleapis.com/v1",
-        "kind": "Job",
-        "metadata":
-        {
-            "name": "{{ name }}",
-            "annotations":
-            {
-                "run.googleapis.com/my-custom-annotation": "{{ my_custom_annotation }}",
-                "run.googleapis.com/launch-stage": "BETA",
-            },
-          ...
-        },
-      ...
-    }
-    ```
-    `my_custom_annotation` can now be used as a placeholder in the job template and set
-    on a per-deployment basis.
-
-    ```yaml
-    # deployment.yaml
-    ...
-    infra_overrides: {"my_custom_annotation": "my-custom-value"}
-    ```
-
-    Additionally, fields can be set to prevent configuration at the deployment
-    level. For example to configure the `vpc_connector_name` field, the placeholder can
-    be removed and replaced with an actual value. Now all deployments that point to this
-    work pool will use the same `vpc_connector_name` value.
-
-    ```json
-    {
-        "apiVersion": "run.googleapis.com/v1",
-        "kind": "Job",
-        "spec":
-        {
-            "template":
-            {
-                "metadata":
-                {
-                    "annotations":
-                    {
-                        "run.googleapis.com/vpc-access-connector": "my-vpc-connector"
-                    }
-                },
-                ...
-            },
-            ...
-        }
-    }
-    ```
-"""
-
 import re
 import shlex
 import time
-from typing import TYPE_CHECKING, Any, Dict, Optional
+from typing import TYPE_CHECKING, Any, Dict, List, Literal, Optional
 from uuid import uuid4
 
-import anyio
-import googleapiclient
-from anyio.abc import TaskStatus  # noqa
+from anyio.abc import TaskStatus
 from google.api_core.client_options import ClientOptions
 from googleapiclient import discovery
+
+# noinspection PyProtectedMember
 from googleapiclient.discovery import Resource
-from pydantic import VERSION as PYDANTIC_VERSION
+from googleapiclient.errors import HttpError
+from pydantic import Field, PrivateAttr, field_validator
 
 from prefect.exceptions import InfrastructureNotFound
 from prefect.logging.loggers import PrefectLogAdapter
 from prefect.utilities.asyncutils import run_sync_in_worker_thread
 from prefect.utilities.dockerutils import get_prefect_image_name
 from prefect.utilities.pydantic import JsonPatch
 from prefect.workers.base import (
     BaseJobConfiguration,
     BaseVariables,
     BaseWorker,
     BaseWorkerResult,
 )
-
-if PYDANTIC_VERSION.startswith("2."):
-    from pydantic.v1 import Field, validator
-else:
-    from pydantic import Field, validator
-
-from prefect_gcp.cloud_run import Execution, Job
 from prefect_gcp.credentials import GcpCredentials
+from prefect_gcp.models.cloud_run_v2 import CloudRunJobV2Result, ExecutionV2, JobV2
 from prefect_gcp.utilities import slugify_name
 
 if TYPE_CHECKING:
     from prefect.client.schemas import FlowRun
     from prefect.server.schemas.core import Flow
     from prefect.server.schemas.responses import DeploymentResponse
 
 
 def _get_default_job_body_template() -> Dict[str, Any]:
-    """Returns the default job body template used by the Cloud Run Job."""
+    """
+    Returns the default job body template for the Cloud Run worker.
+
+    Returns:
+        The default job body template.
+    """
     return {
-        "apiVersion": "run.googleapis.com/v1",
-        "kind": "Job",
-        "metadata": {
-            "name": "{{ name }}",
-            "annotations": {
-                # See: https://cloud.google.com/run/docs/troubleshooting#launch-stage-validation  # noqa
-                "run.googleapis.com/launch-stage": "BETA",
-            },
-        },
-        "spec": {  # JobSpec
-            "template": {  # ExecutionTemplateSpec
-                "spec": {  # ExecutionSpec
-                    "template": {  # TaskTemplateSpec
-                        "spec": {  # TaskSpec
-                            "containers": [
-                                {
-                                    "image": "{{ image }}",
-                                    "command": "{{ command }}",
-                                    "resources": {
-                                        "limits": {
-                                            "cpu": "{{ cpu }}",
-                                            "memory": "{{ memory }}",
-                                        },
-                                        "requests": {
-                                            "cpu": "{{ cpu }}",
-                                            "memory": "{{ memory }}",
-                                        },
-                                    },
-                                }
-                            ],
-                            "timeoutSeconds": "{{ timeout }}",
-                            "serviceAccountName": "{{ service_account_name }}",
-                        }
+        "client": "prefect",
+        "launchStage": "{{ launch_stage }}",
+        "template": {
+            "template": {
+                "serviceAccount": "{{ service_account_name }}",
+                "maxRetries": "{{ max_retries }}",
+                "timeout": "{{ timeout }}",
+                "vpcAccess": {"connector": "{{ vpc_connector_name }}"},
+                "containers": [
+                    {
+                        "env": [],
+                        "image": "{{ image }}",
+                        "command": "{{ command }}",
+                        "args": "{{ args }}",
+                        "resources": {
+                            "limits": {
+                                "cpu": "{{ cpu }}",
+                                "memory": "{{ memory }}",
+                            },
+                        },
                     },
-                },
-                "metadata": {
-                    "annotations": {
-                        "run.googleapis.com/vpc-access-connector": "{{ vpc_connector_name }}"  # noqa
-                    }
-                },
-            },
+                ],
+            }
         },
     }
 
 
 def _get_base_job_body() -> Dict[str, Any]:
-    """Returns a base job body to use for job body validation."""
+    """
+    Returns the base job body for the Cloud Run worker's job body validation.
+
+    Returns:
+        The base job body.
+    """
     return {
-        "apiVersion": "run.googleapis.com/v1",
-        "kind": "Job",
-        "metadata": {
-            "annotations": {
-                # See: https://cloud.google.com/run/docs/troubleshooting#launch-stage-validation  # noqa
-                "run.googleapis.com/launch-stage": "BETA",
-            },
-        },
-        "spec": {  # JobSpec
-            "template": {  # ExecutionTemplateSpec
-                "spec": {  # ExecutionSpec
-                    "template": {  # TaskTemplateSpec
-                        "spec": {"containers": [{}]},  # TaskSpec
-                    },
-                },
+        "template": {
+            "template": {
+                "containers": [],
             },
         },
     }
 
 
-class CloudRunWorkerJobConfiguration(BaseJobConfiguration):
+class CloudRunWorkerJobV2Configuration(BaseJobConfiguration):
     """
-    Configuration class used by the Cloud Run Worker to create a Cloud Run Job.
+    The configuration for the Cloud Run worker V2.
 
-    An instance of this class is passed to the Cloud Run worker's `run` method
-    for each flow run. It contains all information necessary to execute
-    the flow run as a Cloud Run Job.
-
-    Attributes:
-        region: The region where the Cloud Run Job resides.
-        credentials: The GCP Credentials used to connect to Cloud Run.
-        job_body: The job body used to create the Cloud Run Job.
-        timeout: The length of time that Prefect will wait for a Cloud Run Job.
-        keep_job: Whether to delete the Cloud Run Job after it completes.
+    The schema for this class is used to populate the `job_body` section of the
+    default base job template.
     """
 
-    region: str = Field(
-        default="us-central1", description="The region where the Cloud Run Job resides."
-    )
-    credentials: Optional[GcpCredentials] = Field(
+    credentials: GcpCredentials = Field(
         title="GCP Credentials",
         default_factory=GcpCredentials,
-        description="The GCP Credentials used to connect to Cloud Run. "
-        "If not provided credentials will be inferred from "
-        "the local environment.",
-    )
-    job_body: Dict[str, Any] = Field(template=_get_default_job_body_template())
-    timeout: Optional[int] = Field(
-        default=600,
-        gt=0,
-        le=3600,
-        title="Job Timeout",
         description=(
-            "The length of time that Prefect will wait for a Cloud Run Job to complete "
-            "before raising an exception."
+            "The GCP Credentials used to connect to Cloud Run. "
+            "If not provided credentials will be inferred from "
+            "the local environment."
         ),
     )
-    keep_job: Optional[bool] = Field(
+    job_body: Dict[str, Any] = Field(
+        json_schema_extra=dict(template=_get_default_job_body_template()),
+    )
+    keep_job: bool = Field(
         default=False,
         title="Keep Job After Completion",
-        description="Keep the completed Cloud Run Job on Google Cloud Platform.",
+        description="Keep the completed Cloud run job on Google Cloud Platform.",
+    )
+    region: str = Field(
+        default="us-central1",
+        description="The region in which to run the Cloud Run job",
+    )
+    timeout: int = Field(
+        default=600,
+        gt=0,
+        le=86400,
+        description=(
+            "The length of time that Prefect will wait for a Cloud Run Job to "
+            "complete before raising an exception."
+        ),
     )
+    _job_name: str = PrivateAttr(default=None)
 
     @property
     def project(self) -> str:
-        """property for accessing the project from the credentials."""
+        """
+        Returns the GCP project associated with the credentials.
+
+        Returns:
+            str: The GCP project associated with the credentials.
+        """
         return self.credentials.project
 
     @property
     def job_name(self) -> str:
-        """property for accessing the name from the job metadata."""
-        return self.job_body["metadata"]["name"]
+        """
+        Returns the name of the job.
+
+        Returns:
+            str: The name of the job.
+        """
+        if self._job_name is None:
+            base_job_name = slugify_name(self.name)
+            job_name = f"{base_job_name}-{uuid4().hex}"
+            self._job_name = job_name
+
+        return self._job_name
 
     def prepare_for_flow_run(
         self,
         flow_run: "FlowRun",
         deployment: Optional["DeploymentResponse"] = None,
         flow: Optional["Flow"] = None,
     ):
@@ -330,105 +164,121 @@
 
         Args:
             flow_run: The flow run to prepare the job configuration for
             deployment: The deployment associated with the flow run used for
                 preparation.
             flow: The flow associated with the flow run used for preparation.
         """
-        super().prepare_for_flow_run(flow_run, deployment, flow)
+        super().prepare_for_flow_run(
+            flow_run=flow_run,
+            deployment=deployment,
+            flow=flow,
+        )
 
-        self._populate_envs()
+        self._populate_env()
         self._populate_or_format_command()
         self._format_args_if_present()
         self._populate_image_if_not_present()
-        self._populate_name_if_not_present()
+        self._populate_timeout()
+        self._remove_vpc_access_if_unset()
 
-    def _populate_envs(self):
-        """Populate environment variables. BaseWorker.prepare_for_flow_run handles
-        putting the environment variables in the `env` attribute. This method
-        moves them into the jobs body"""
+    def _populate_timeout(self):
+        """
+        Populates the job body with the timeout.
+        """
+        self.job_body["template"]["template"]["timeout"] = f"{self.timeout}s"
+
+    def _populate_env(self):
+        """
+        Populates the job body with environment variables.
+        """
         envs = [{"name": k, "value": v} for k, v in self.env.items()]
-        self.job_body["spec"]["template"]["spec"]["template"]["spec"]["containers"][0][
-            "env"
-        ] = envs
 
-    def _populate_name_if_not_present(self):
-        """Adds the flow run name to the job if one is not already provided."""
-        try:
-            if "name" not in self.job_body["metadata"]:
-                base_job_name = slugify_name(self.name)
-                job_name = f"{base_job_name}-{uuid4().hex}"
-                self.job_body["metadata"]["name"] = job_name
-        except KeyError:
-            raise ValueError("Unable to verify name due to invalid job body template.")
+        self.job_body["template"]["template"]["containers"][0]["env"] = envs
 
     def _populate_image_if_not_present(self):
-        """Adds the latest prefect image to the job if one is not already provided."""
-        try:
-            if (
+        """
+        Populates the job body with the image if not present.
+        """
+        if "image" not in self.job_body["template"]["template"]["containers"][0]:
+            self.job_body["template"]["template"]["containers"][0][
                 "image"
-                not in self.job_body["spec"]["template"]["spec"]["template"]["spec"][
-                    "containers"
-                ][0]
-            ):
-                self.job_body["spec"]["template"]["spec"]["template"]["spec"][
-                    "containers"
-                ][0]["image"] = f"docker.io/{get_prefect_image_name()}"
-        except KeyError:
-            raise ValueError("Unable to verify image due to invalid job body template.")
+            ] = f"docker.io/{get_prefect_image_name()}"
 
     def _populate_or_format_command(self):
         """
-        Ensures that the command is present in the job manifest. Populates the command
-        with the `prefect -m prefect.engine` if a command is not present.
+        Populates the job body with the command if not present.
         """
-        try:
-            command = self.job_body["spec"]["template"]["spec"]["template"]["spec"][
-                "containers"
-            ][0].get("command")
-            if command is None:
-                self.job_body["spec"]["template"]["spec"]["template"]["spec"][
-                    "containers"
-                ][0]["command"] = shlex.split(self._base_flow_run_command())
-            elif isinstance(command, str):
-                self.job_body["spec"]["template"]["spec"]["template"]["spec"][
-                    "containers"
-                ][0]["command"] = shlex.split(command)
-        except KeyError:
-            raise ValueError(
-                "Unable to verify command due to invalid job body template."
-            )
+        command = self.job_body["template"]["template"]["containers"][0].get("command")
+
+        if command is None:
+            self.job_body["template"]["template"]["containers"][0][
+                "command"
+            ] = shlex.split(self._base_flow_run_command())
+        elif isinstance(command, str):
+            self.job_body["template"]["template"]["containers"][0][
+                "command"
+            ] = shlex.split(command)
 
     def _format_args_if_present(self):
-        try:
-            args = self.job_body["spec"]["template"]["spec"]["template"]["spec"][
-                "containers"
-            ][0].get("args")
-            if args is not None and isinstance(args, str):
-                self.job_body["spec"]["template"]["spec"]["template"]["spec"][
-                    "containers"
-                ][0]["args"] = shlex.split(args)
-        except KeyError:
-            raise ValueError("Unable to verify args due to invalid job body template.")
+        """
+        Formats the job body args if present.
+        """
+        args = self.job_body["template"]["template"]["containers"][0].get("args")
+
+        if args is not None and isinstance(args, str):
+            self.job_body["template"]["template"]["containers"][0][
+                "args"
+            ] = shlex.split(args)
 
-    @validator("job_body")
+    def _remove_vpc_access_if_unset(self):
+        """
+        Removes vpcAccess if unset.
+        """
+
+        if "vpcAccess" not in self.job_body["template"]["template"]:
+            return
+
+        vpc_access = self.job_body["template"]["template"]["vpcAccess"]
+
+        # if vpcAccess is unset or connector is unset, remove the entire vpcAccess block
+        # otherwise leave the user provided value.
+        if not vpc_access or (
+            len(vpc_access) == 1
+            and "connector" in vpc_access
+            and vpc_access["connector"] is None
+        ):
+            self.job_body["template"]["template"].pop("vpcAccess")
+
+    # noinspection PyMethodParameters
+    @field_validator("job_body")
+    @classmethod
     def _ensure_job_includes_all_required_components(cls, value: Dict[str, Any]):
         """
         Ensures that the job body includes all required components.
+
+        Args:
+            value: The job body to validate.
+        Returns:
+            The validated job body.
         """
         patch = JsonPatch.from_diff(value, _get_base_job_body())
+
         missing_paths = sorted([op["path"] for op in patch if op["op"] == "add"])
+
         if missing_paths:
             raise ValueError(
-                "Job is missing required attributes at the following paths: "
-                f"{', '.join(missing_paths)}"
+                f"Job body is missing required components: {', '.join(missing_paths)}"
             )
+
         return value
 
-    @validator("job_body")
+    # noinspection PyMethodParameters
+    @field_validator("job_body")
+    @classmethod
     def _ensure_job_has_compatible_values(cls, value: Dict[str, Any]):
         """Ensure that the job body has compatible values."""
         patch = JsonPatch.from_diff(value, _get_base_job_body())
         incompatible = sorted(
             [
                 f"{op['path']} must have value {op['value']!r}"
                 for op in patch
@@ -439,428 +289,588 @@
             raise ValueError(
                 "Job has incompatible values for the following attributes: "
                 f"{', '.join(incompatible)}"
             )
         return value
 
 
-class CloudRunWorkerVariables(BaseVariables):
+class CloudRunWorkerV2Variables(BaseVariables):
     """
-    Default variables for the Cloud Run worker.
+    Default variables for the v2 Cloud Run worker.
 
-    The schema for this class is used to populate the `variables` section of the default
-    base job template.
+    The schema for this class is used to populate the `variables` section of the
+    default base job template.
     """
 
-    region: str = Field(
-        default="us-central1",
-        description="The region where the Cloud Run Job resides.",
-        example="us-central1",
-    )
-    credentials: Optional[GcpCredentials] = Field(
+    credentials: GcpCredentials = Field(
         title="GCP Credentials",
         default_factory=GcpCredentials,
-        description="The GCP Credentials used to initiate the "
-        "Cloud Run Job. If not provided credentials will be "
-        "inferred from the local environment.",
+        description=(
+            "The GCP Credentials used to connect to Cloud Run. "
+            "If not provided credentials will be inferred from "
+            "the local environment."
+        ),
+    )
+    region: str = Field(
+        default="us-central1",
+        description="The region in which to run the Cloud Run job",
     )
     image: Optional[str] = Field(
-        default=None,
+        default="prefecthq/prefect:3-latest",
         title="Image Name",
         description=(
-            "The image to use for a new Cloud Run Job. "
-            "If not set, the latest Prefect image will be used. "
-            "See https://cloud.google.com/run/docs/deploying#images."
+            "The image to use for the Cloud Run job. "
+            "If not provided the default Prefect image will be used."
         ),
-        example="docker.io/prefecthq/prefect:2-latest",
     )
-    cpu: Optional[str] = Field(
-        default=None,
-        title="CPU",
+    args: List[str] = Field(
+        default_factory=list,
         description=(
-            "The amount of compute allocated to the Cloud Run Job. "
-            "(1000m = 1 CPU). See "
-            "https://cloud.google.com/run/docs/configuring/cpu#setting-jobs."
+            "The arguments to pass to the Cloud Run Job V2's entrypoint command."
         ),
-        example="1000m",
-        regex=r"^(\d*000)m$",
     )
-    memory: Optional[str] = Field(
-        default=None,
+    keep_job: bool = Field(
+        default=False,
+        title="Keep Job After Completion",
+        description="Keep the completed Cloud run job on Google Cloud Platform.",
+    )
+    launch_stage: Literal[
+        "ALPHA",
+        "BETA",
+        "GA",
+        "DEPRECATED",
+        "EARLY_ACCESS",
+        "PRELAUNCH",
+        "UNIMPLEMENTED",
+        "LAUNCH_TAG_UNSPECIFIED",
+    ] = Field(
+        "BETA",
+        description=(
+            "The launch stage of the Cloud Run Job V2. "
+            "See https://cloud.google.com/run/docs/about-features-categories "
+            "for additional details."
+        ),
+    )
+    max_retries: int = Field(
+        default=0,
+        title="Max Retries",
+        description="The number of times to retry the Cloud Run job.",
+    )
+    cpu: str = Field(
+        default="1000m",
+        title="CPU",
+        description="The CPU to allocate to the Cloud Run job.",
+    )
+    memory: str = Field(
+        default="512Mi",
         title="Memory",
         description=(
-            "The amount of memory allocated to the Cloud Run Job. "
-            "Must be specified in units of 'G', 'Gi', 'M', or 'Mi'. "
-            "See https://cloud.google.com/run/docs/configuring/memory-limits#setting."
+            "The memory to allocate to the Cloud Run job along with the units, which"
+            "could be: G, Gi, M, Mi."
+        ),
+        examples=["512Mi"],
+        pattern=r"^\d+(?:G|Gi|M|Mi)$",
+    )
+    timeout: int = Field(
+        default=600,
+        gt=0,
+        le=86400,
+        title="Job Timeout",
+        description=(
+            "The length of time that Prefect will wait for a Cloud Run Job to "
+            "complete before raising an exception (maximum of 86400 seconds, 1 day)."
         ),
-        example="512Mi",
-        regex=r"^\d+(?:G|Gi|M|Mi)$",
     )
     vpc_connector_name: Optional[str] = Field(
         default=None,
         title="VPC Connector Name",
-        description="The name of the VPC connector to use for the Cloud Run Job.",
+        description="The name of the VPC connector to use for the Cloud Run job.",
     )
     service_account_name: Optional[str] = Field(
         default=None,
         title="Service Account Name",
-        description="The name of the service account to use for the task execution "
-        "of Cloud Run Job. By default Cloud Run jobs run as the default "
-        "Compute Engine Service Account. ",
-        example="service-account@example.iam.gserviceaccount.com",
-    )
-    keep_job: Optional[bool] = Field(
-        default=False,
-        title="Keep Job After Completion",
-        description="Keep the completed Cloud Run Job after it has run.",
-    )
-    timeout: Optional[int] = Field(
-        default=600,
-        gt=0,
-        le=3600,
-        title="Job Timeout",
         description=(
-            "The length of time that Prefect will wait for Cloud Run Job state changes."
+            "The name of the service account to use for the task execution "
+            "of Cloud Run Job. By default Cloud Run jobs run as the default "
+            "Compute Engine Service Account."
         ),
+        examples=["service-account@example.iam.gserviceaccount.com"],
     )
 
 
-class CloudRunWorkerResult(BaseWorkerResult):
-    """Contains information about the final state of a completed process"""
-
+class CloudRunWorkerV2Result(BaseWorkerResult):
+    """
+    The result of a Cloud Run worker V2 job.
+    """
 
-class CloudRunWorker(BaseWorker):
-    """Prefect worker that executes flow runs within Cloud Run Jobs."""
 
-    type = "cloud-run"
-    job_configuration = CloudRunWorkerJobConfiguration
-    job_configuration_variables = CloudRunWorkerVariables
-    _description = (
-        "Execute flow runs within containers on Google Cloud Run. Requires "
-        "a Google Cloud Platform account."
-    )
-    _display_name = "Google Cloud Run"
-    _documentation_url = "https://prefecthq.github.io/prefect-gcp/cloud_run_worker/"
-    _logo_url = "https://cdn.sanity.io/images/3ugk85nk/production/10424e311932e31c477ac2b9ef3d53cefbaad708-250x250.png"  # noqa
-
-    def _create_job_error(self, exc, configuration):
-        """Provides a nicer error for 404s when trying to create a Cloud Run Job."""
-        # TODO consider lookup table instead of the if/else,
-        # also check for documented errors
-        if exc.status_code == 404:
-            raise RuntimeError(
-                f"Failed to find resources at {exc.uri}. Confirm that region"
-                f" '{self.region}' is the correct region for your Cloud Run Job and"
-                f" that {configuration.project} is the correct GCP project. If"
-                f" your project ID is not correct, you are using a Credentials block"
-                f" with permissions for the wrong project."
-            ) from exc
-        raise exc
-
-    def _job_run_submission_error(self, exc, configuration):
-        """Provides a nicer error for 404s when submitting job runs."""
-        if exc.status_code == 404:
-            pat1 = r"The requested URL [^ ]+ was not found on this server"
-            # pat2 = (
-            #     r"Resource '[^ ]+' of kind 'JOB' in region '[\w\-0-9]+' "
-            #     r"in project '[\w\-0-9]+' does not exist"
-            # )
-            if re.findall(pat1, str(exc)):
-                raise RuntimeError(
-                    f"Failed to find resources at {exc.uri}. "
-                    f"Confirm that region '{self.region}' is "
-                    f"the correct region for your Cloud Run Job "
-                    f"and that '{configuration.project}' is the "
-                    f"correct GCP project. If your project ID is not "
-                    f"correct, you are using a Credentials "
-                    f"block with permissions for the wrong project."
-                ) from exc
-            else:
-                raise exc
+class CloudRunWorkerV2(BaseWorker):
+    """
+    The Cloud Run worker V2.
+    """
 
-        raise exc
+    type = "cloud-run-v2"
+    job_configuration = CloudRunWorkerJobV2Configuration
+    job_configuration_variables = CloudRunWorkerV2Variables
+    _description = "Execute flow runs within containers on Google Cloud Run (V2 API). Requires a Google Cloud Platform account."  # noqa
+    _display_name = "Google Cloud Run V2"
+    _documentation_url = "https://prefecthq.github.io/prefect-gcp/worker_v2/"
+    _logo_url = "https://images.ctfassets.net/gm98wzqotmnx/4SpnOBvMYkHp6z939MDKP6/549a91bc1ce9afd4fb12c68db7b68106/social-icon-google-cloud-1200-630.png?h=250"  # noqa
 
     async def run(
         self,
         flow_run: "FlowRun",
-        configuration: CloudRunWorkerJobConfiguration,
-        task_status: Optional[anyio.abc.TaskStatus] = None,
-    ) -> CloudRunWorkerResult:
-        """
-        Executes a flow run within a Cloud Run Job and waits for the flow run
-        to complete.
+        configuration: CloudRunWorkerJobV2Configuration,
+        task_status: Optional[TaskStatus] = None,
+    ) -> CloudRunJobV2Result:
+        """
+        Runs the flow run on Cloud Run and waits for it to complete.
 
         Args:
-            flow_run: The flow run to execute
-            configuration: The configuration to use when executing the flow run.
-            task_status: The task status object for the current flow run. If provided,
-                the task will be marked as started.
+            flow_run: The flow run to run.
+            configuration: The configuration for the job.
+            task_status: The task status to update.
 
         Returns:
-            CloudRunWorkerResult: A result object containing information about the
-                final state of the flow run
+            The result of the job.
         """
-
         logger = self.get_flow_run_logger(flow_run)
 
-        with self._get_client(configuration) as client:
+        with self._get_client(configuration=configuration) as cr_client:
             await run_sync_in_worker_thread(
                 self._create_job_and_wait_for_registration,
-                configuration,
-                client,
-                logger,
+                configuration=configuration,
+                cr_client=cr_client,
+                logger=logger,
             )
-            job_execution = await run_sync_in_worker_thread(
-                self._begin_job_execution, configuration, client, logger
+
+            execution = await run_sync_in_worker_thread(
+                self._begin_job_execution,
+                configuration=configuration,
+                cr_client=cr_client,
+                logger=logger,
             )
 
             if task_status:
                 task_status.started(configuration.job_name)
 
             result = await run_sync_in_worker_thread(
                 self._watch_job_execution_and_get_result,
-                configuration,
-                client,
-                job_execution,
-                logger,
+                configuration=configuration,
+                cr_client=cr_client,
+                execution=execution,
+                logger=logger,
             )
+
             return result
 
-    def _get_client(self, configuration: CloudRunWorkerJobConfiguration) -> Resource:
-        """Get the base client needed for interacting with GCP APIs."""
-        # region needed for 'v1' API
-        api_endpoint = f"https://{configuration.region}-run.googleapis.com"
+    async def kill_infrastructure(
+        self,
+        infrastructure_pid: str,
+        configuration: CloudRunWorkerJobV2Configuration,
+        grace_seconds: int = 30,
+    ):
+        """
+        Stops the Cloud Run job.
+
+        Args:
+            infrastructure_pid: The ID of the infrastructure to stop.
+            configuration: The configuration for the job.
+            grace_seconds: The number of seconds to wait before stopping the job.
+        """
+        if grace_seconds != 30:
+            self._logger.warning(
+                f"Kill grace period of {grace_seconds}s requested, but GCP does not "
+                "support dynamic grace period configuration. See here for more info: "
+                "https://cloud.google.com/run/docs/reference/rest/v1/namespaces.jobs/delete"  # noqa
+            )
+
+        with self._get_client(configuration=configuration) as cr_client:
+            await run_sync_in_worker_thread(
+                self._stop_job,
+                cr_client=cr_client,
+                configuration=configuration,
+                job_name=infrastructure_pid,
+            )
+
+    @staticmethod
+    def _get_client(
+        configuration: CloudRunWorkerJobV2Configuration,
+    ) -> ResourceWarning:
+        """
+        Get the base client needed for interacting with GCP Cloud Run V2 API.
+
+        Returns:
+            Resource: The base client needed for interacting with GCP Cloud Run V2 API.
+        """
+        api_endpoint = "https://run.googleapis.com"
         gcp_creds = configuration.credentials.get_credentials_from_service_account()
+
         options = ClientOptions(api_endpoint=api_endpoint)
 
-        return discovery.build(
-            "run", "v1", client_options=options, credentials=gcp_creds
-        ).namespaces()
+        return (
+            discovery.build(
+                "run",
+                "v2",
+                client_options=options,
+                credentials=gcp_creds,
+                num_retries=3,  # Set to 3 in case of intermittent/connection issues
+            )
+            .projects()
+            .locations()
+        )
 
     def _create_job_and_wait_for_registration(
         self,
-        configuration: CloudRunWorkerJobConfiguration,
-        client: Resource,
+        configuration: CloudRunWorkerJobV2Configuration,
+        cr_client: Resource,
         logger: PrefectLogAdapter,
-    ) -> None:
-        """Create a new job wait for it to finish registering."""
+    ):
+        """
+        Creates the Cloud Run job and waits for it to register.
+
+        Args:
+            configuration: The configuration for the job.
+            cr_client: The Cloud Run client.
+            logger: The logger to use.
+        """
         try:
-            logger.info(f"Creating Cloud Run Job {configuration.job_name}")
+            logger.info(f"Creating Cloud Run JobV2 {configuration.job_name}")
 
-            Job.create(
-                client=client,
-                namespace=configuration.credentials.project,
+            JobV2.create(
+                cr_client=cr_client,
+                project=configuration.project,
+                location=configuration.region,
+                job_id=configuration.job_name,
                 body=configuration.job_body,
             )
-        except googleapiclient.errors.HttpError as exc:
-            self._create_job_error(exc, configuration)
+        except HttpError as exc:
+            self._create_job_error(
+                exc=exc,
+                configuration=configuration,
+            )
 
         try:
             self._wait_for_job_creation(
-                client=client, configuration=configuration, logger=logger
+                cr_client=cr_client,
+                configuration=configuration,
+                logger=logger,
             )
-        except Exception:
-            logger.exception(
-                "Encountered an exception while waiting for job run creation"
+        except Exception as exc:
+            logger.critical(
+                f"Failed to create Cloud Run JobV2 {configuration.job_name}.\n{exc}"
             )
+
             if not configuration.keep_job:
-                logger.info(
-                    f"Deleting Cloud Run Job {configuration.job_name} from "
-                    "Google Cloud Run."
-                )
                 try:
-                    Job.delete(
-                        client=client,
-                        namespace=configuration.credentials.project,
+                    JobV2.delete(
+                        cr_client=cr_client,
+                        project=configuration.project,
+                        location=configuration.region,
                         job_name=configuration.job_name,
                     )
-                except Exception:
-                    logger.exception(
-                        "Received an unexpected exception while attempting to delete"
-                        f" Cloud Run Job {configuration.job_name!r}"
+                except Exception as exc2:
+                    logger.critical(
+                        f"Failed to delete Cloud Run JobV2 {configuration.job_name}."
+                        f"\n{exc2}"
                     )
+
             raise
 
+    @staticmethod
+    def _wait_for_job_creation(
+        cr_client: Resource,
+        configuration: CloudRunWorkerJobV2Configuration,
+        logger: PrefectLogAdapter,
+        poll_interval: int = 5,
+    ):
+        """
+        Waits for the Cloud Run job to be created.
+
+        Args:
+            cr_client: The Cloud Run client.
+            configuration: The configuration for the job.
+            logger: The logger to use.
+            poll_interval: The interval to poll the Cloud Run job, defaults to 5
+                seconds.
+        """
+        job = JobV2.get(
+            cr_client=cr_client,
+            project=configuration.project,
+            location=configuration.region,
+            job_name=configuration.job_name,
+        )
+
+        t0 = time.time()
+
+        while not job.is_ready():
+            if not (ready_condition := job.get_ready_condition()):
+                ready_condition = "waiting for condition update"
+
+            logger.info(f"Current Job Condition: {ready_condition}")
+
+            job = JobV2.get(
+                cr_client=cr_client,
+                project=configuration.project,
+                location=configuration.region,
+                job_name=configuration.job_name,
+            )
+
+            elapsed_time = time.time() - t0
+
+            if elapsed_time > configuration.timeout:
+                raise RuntimeError(
+                    f"Timeout of {configuration.timeout} seconds reached while "
+                    f"waiting for Cloud Run Job V2 {configuration.job_name} to be "
+                    "created."
+                )
+
+            time.sleep(poll_interval)
+
+    @staticmethod
+    def _create_job_error(
+        exc: HttpError,
+        configuration: CloudRunWorkerJobV2Configuration,
+    ):
+        """
+        Creates a formatted error message for the Cloud Run V2 API errors
+        """
+        # noinspection PyUnresolvedReferences
+        if exc.status_code == 404:
+            raise RuntimeError(
+                f"Failed to find resources at {exc.uri}. Confirm that region"
+                f" '{configuration.region}' is the correct region for your Cloud"
+                f" Run Job and that {configuration.project} is the correct GCP "
+                f" project. If your project ID is not correct, you are using a "
+                f"Credentials block with permissions for the wrong project."
+            ) from exc
+
+        raise exc
+
     def _begin_job_execution(
         self,
-        configuration: CloudRunWorkerJobConfiguration,
-        client: Resource,
+        cr_client: Resource,
+        configuration: CloudRunWorkerJobV2Configuration,
         logger: PrefectLogAdapter,
-    ) -> Execution:
-        """Submit a job run for execution and return the execution object."""
+    ) -> ExecutionV2:
+        """
+        Begins the Cloud Run job execution.
+
+        Args:
+            cr_client: The Cloud Run client.
+            configuration: The configuration for the job.
+            logger: The logger to use.
+
+        Returns:
+            The Cloud Run job execution.
+        """
         try:
             logger.info(
-                f"Submitting Cloud Run Job {configuration.job_name!r} for execution."
+                f"Submitting Cloud Run Job V2 {configuration.job_name} for execution..."
             )
-            submission = Job.run(
-                client=client,
-                namespace=configuration.project,
+
+            submission = JobV2.run(
+                cr_client=cr_client,
+                project=configuration.project,
+                location=configuration.region,
                 job_name=configuration.job_name,
             )
 
-            job_execution = Execution.get(
-                client=client,
-                namespace=submission["metadata"]["namespace"],
-                execution_name=submission["metadata"]["name"],
+            job_execution = ExecutionV2.get(
+                cr_client=cr_client,
+                execution_id=submission["metadata"]["name"],
+            )
+
+            command = (
+                " ".join(configuration.command)
+                if configuration.command
+                else "default container command"
             )
-        except Exception as exc:
-            self._job_run_submission_error(exc, configuration)
 
-        return job_execution
+            logger.info(
+                f"Cloud Run Job V2 {configuration.job_name} submitted for execution "
+                f"with command: {command}"
+            )
+
+            return job_execution
+        except Exception as exc:
+            self._job_run_submission_error(
+                exc=exc,
+                configuration=configuration,
+            )
+            raise
 
     def _watch_job_execution_and_get_result(
         self,
-        configuration: CloudRunWorkerJobConfiguration,
-        client: Resource,
-        execution: Execution,
+        cr_client: Resource,
+        configuration: CloudRunWorkerJobV2Configuration,
+        execution: ExecutionV2,
         logger: PrefectLogAdapter,
         poll_interval: int = 5,
-    ) -> CloudRunWorkerResult:
-        """Wait for execution to complete and then return result."""
+    ) -> CloudRunJobV2Result:
+        """
+        Watch the job execution and get the result.
+
+        Args:
+            cr_client (Resource): The base client needed for interacting with GCP
+                Cloud Run V2 API.
+            configuration (CloudRunWorkerJobV2Configuration): The configuration for
+                the job.
+            execution (ExecutionV2): The execution to watch.
+            logger (PrefectLogAdapter): The logger to use.
+            poll_interval (int): The number of seconds to wait between polls.
+                Defaults to 5 seconds.
+
+        Returns:
+            The result of the job.
+        """
         try:
-            job_execution = self._watch_job_execution(
-                client=client,
-                job_execution=execution,
-                timeout=configuration.timeout,
+            execution = self._watch_job_execution(
+                cr_client=cr_client,
+                configuration=configuration,
+                execution=execution,
                 poll_interval=poll_interval,
             )
-        except Exception:
-            logger.exception(
-                "Received an unexpected exception while monitoring Cloud Run Job "
-                f"{configuration.job_name!r}"
+        except Exception as exc:
+            logger.critical(
+                f"Encountered an exception while waiting for job run completion - "
+                f"{exc}"
             )
             raise
 
-        if job_execution.succeeded():
+        if execution.succeeded():
             status_code = 0
-            logger.info(f"Job Run {configuration.job_name} completed successfully")
+            logger.info(f"Cloud Run Job V2 {configuration.job_name} succeeded")
         else:
             status_code = 1
-            error_msg = job_execution.condition_after_completion()["message"]
+            error_mg = execution.condition_after_completion().get("message")
             logger.error(
-                "Job Run {configuration.job_name} did not complete successfully. "
-                f"{error_msg}"
+                f"Cloud Run Job V2 {configuration.job_name} failed - {error_mg}"
             )
 
-        logger.info(f"Job Run logs can be found on GCP at: {job_execution.log_uri}")
+        logger.info(f"Job run logs can be found on GCP at: {execution.logUri}")
 
         if not configuration.keep_job:
             logger.info(
-                f"Deleting completed Cloud Run Job {configuration.job_name!r} "
-                "from Google Cloud Run..."
+                f"Deleting completed Cloud Run Job {configuration.job_name!r} from "
+                "Google Cloud Run..."
             )
+
             try:
-                Job.delete(
-                    client=client,
-                    namespace=configuration.project,
+                JobV2.delete(
+                    cr_client=cr_client,
+                    project=configuration.project,
+                    location=configuration.region,
                     job_name=configuration.job_name,
                 )
-            except Exception:
-                logger.exception(
-                    "Received an unexpected exception while attempting to delete Cloud"
-                    f" Run Job {configuration.job_name}"
+            except Exception as exc:
+                logger.critical(
+                    "Received an exception while deleting the Cloud Run Job V2 "
+                    f"- {configuration.job_name} - {exc}"
                 )
 
-        return CloudRunWorkerResult(
-            identifier=configuration.job_name, status_code=status_code
+        return CloudRunJobV2Result(
+            identifier=configuration.job_name,
+            status_code=status_code,
         )
 
+    # noinspection DuplicatedCode
+    @staticmethod
     def _watch_job_execution(
-        self, client, job_execution: Execution, timeout: int, poll_interval: int = 5
-    ):
+        cr_client: Resource,
+        configuration: CloudRunWorkerJobV2Configuration,
+        execution: ExecutionV2,
+        poll_interval: int,
+    ) -> ExecutionV2:
         """
-        Update job_execution status until it is no longer running or timeout is reached.
+        Update execution status until it is no longer running or timeout is reached.
+
+        Args:
+            cr_client (Resource): The base client needed for interacting with GCP
+                Cloud Run V2 API.
+            configuration (CloudRunWorkerJobV2Configuration): The configuration for
+                the job.
+            execution (ExecutionV2): The execution to watch.
+            poll_interval (int): The number of seconds to wait between polls.
+
+        Returns:
+            The execution.
         """
         t0 = time.time()
-        while job_execution.is_running():
-            job_execution = Execution.get(
-                client=client,
-                namespace=job_execution.namespace,
-                execution_name=job_execution.name,
+
+        while execution.is_running():
+            execution = ExecutionV2.get(
+                cr_client=cr_client,
+                execution_id=execution.name,
             )
 
             elapsed_time = time.time() - t0
-            if timeout is not None and elapsed_time > timeout:
+
+            if elapsed_time > configuration.timeout:
                 raise RuntimeError(
-                    f"Timed out after {elapsed_time}s while waiting for Cloud Run Job "
-                    "execution to complete. Your job may still be running on GCP."
+                    f"Timeout of {configuration.timeout} seconds reached while "
+                    f"waiting for Cloud Run Job V2 {configuration.job_name} to "
+                    "complete."
                 )
 
             time.sleep(poll_interval)
 
-        return job_execution
+        return execution
 
-    def _wait_for_job_creation(
-        self,
-        client: Resource,
-        configuration: CloudRunWorkerJobConfiguration,
-        logger: PrefectLogAdapter,
-        poll_interval: int = 5,
+    @staticmethod
+    def _job_run_submission_error(
+        exc: Exception,
+        configuration: CloudRunWorkerJobV2Configuration,
     ):
-        """Give created job time to register."""
-        job = Job.get(
-            client=client,
-            namespace=configuration.project,
-            job_name=configuration.job_name,
-        )
+        """
+        Creates a formatted error message for the Cloud Run V2 API errors
 
-        t0 = time.time()
-        while not job.is_ready():
-            ready_condition = (
-                job.ready_condition
-                if job.ready_condition
-                else "waiting for condition update"
-            )
-            logger.info(f"Job is not yet ready... Current condition: {ready_condition}")
-            job = Job.get(
-                client=client,
-                namespace=configuration.project,
-                job_name=configuration.job_name,
-            )
+        Args:
+            exc: The exception to format.
+            configuration: The configuration for the job.
+        """
+        # noinspection PyUnresolvedReferences
+        if exc.status_code == 404:
+            pat1 = r"The requested URL [^ ]+ was not found on this server"
 
-            elapsed_time = time.time() - t0
-            if (
-                configuration.timeout is not None
-                and elapsed_time > configuration.timeout
-            ):
+            if re.findall(pat1, str(exc)):
+                # noinspection PyUnresolvedReferences
                 raise RuntimeError(
-                    f"Timed out after {elapsed_time}s while waiting for Cloud Run Job "
-                    "execution to complete. Your job may still be running on GCP."
-                )
-
-            time.sleep(poll_interval)
+                    f"Failed to find resources at {exc.uri}. "
+                    f"Confirm that region '{configuration.region}' is "
+                    f"the correct region for your Cloud Run Job "
+                    f"and that '{configuration.project}' is the "
+                    f"correct GCP project. If your project ID is not "
+                    f"correct, you are using a Credentials "
+                    f"block with permissions for the wrong project."
+                ) from exc
+            else:
+                raise exc
 
-    async def kill_infrastructure(
-        self,
-        infrastructure_pid: str,
-        configuration: CloudRunWorkerJobConfiguration,
-        grace_seconds: int = 30,
+    @staticmethod
+    def _stop_job(
+        cr_client: Resource,
+        configuration: CloudRunWorkerJobV2Configuration,
+        job_name: str,
     ):
         """
-        Stops a job for a cancelled flow run based on the provided infrastructure PID
-        and run configuration.
-        """
-        if grace_seconds != 30:
-            self._logger.warning(
-                f"Kill grace period of {grace_seconds}s requested, but GCP does not "
-                "support dynamic grace period configuration. See here for more info: "
-                "https://cloud.google.com/run/docs/reference/rest/v1/namespaces.jobs/delete"  # noqa
-            )
+        Stops/deletes the Cloud Run job.
 
-        with self._get_client(configuration) as client:
-            await run_sync_in_worker_thread(
-                self._stop_job,
-                client=client,
-                namespace=configuration.project,
-                job_name=infrastructure_pid,
-            )
-
-    def _stop_job(self, client: Resource, namespace: str, job_name: str):
+        Args:
+            cr_client: The Cloud Run client.
+            configuration: The configuration for the job.
+            job_name: The name of the job to stop.
+        """
         try:
-            Job.delete(client=client, namespace=namespace, job_name=job_name)
+            JobV2.delete(
+                cr_client=cr_client,
+                project=configuration.project,
+                location=configuration.region,
+                job_name=job_name,
+            )
         except Exception as exc:
             if "does not exist" in str(exc):
                 raise InfrastructureNotFound(
                     f"Cannot stop Cloud Run Job; the job name {job_name!r} "
                     "could not be found."
                 ) from exc
             raise
```

### Comparing `prefect_gcp-0.5.9/prefect_gcp/workers/cloud_run_v2.py` & `prefect_gcp-0.6.0rc1/tests/test_cloud_run_worker.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,880 +1,708 @@
-import re
-import shlex
-import time
-from typing import TYPE_CHECKING, Any, Dict, List, Literal, Optional
-from uuid import uuid4
-
-from anyio.abc import TaskStatus
-from google.api_core.client_options import ClientOptions
-from googleapiclient import discovery
+import uuid
+from unittest.mock import Mock
 
-# noinspection PyProtectedMember
-from googleapiclient.discovery import Resource
+import anyio
+import pydantic
+import pytest
 from googleapiclient.errors import HttpError
-from pydantic import VERSION as PYDANTIC_VERSION
+from prefect_gcp.credentials import GcpCredentials
+from prefect_gcp.utilities import slugify_name
+from prefect_gcp.workers.cloud_run import (
+    CloudRunWorker,
+    CloudRunWorkerJobConfiguration,
+    CloudRunWorkerResult,
+)
 
+from prefect.client.schemas.objects import FlowRun
 from prefect.exceptions import InfrastructureNotFound
-from prefect.logging.loggers import PrefectLogAdapter
-from prefect.utilities.asyncutils import run_sync_in_worker_thread
+from prefect.server.schemas.actions import DeploymentCreate
 from prefect.utilities.dockerutils import get_prefect_image_name
-from prefect.utilities.pydantic import JsonPatch
-from prefect.workers.base import (
-    BaseJobConfiguration,
-    BaseVariables,
-    BaseWorker,
-    BaseWorkerResult,
+from prefect.utilities.schema_tools.validation import (
+    ValidationError as PrefectValidationError,
 )
 
-if PYDANTIC_VERSION.startswith("2."):
-    from pydantic.v1 import Field, PrivateAttr, validator
-else:
-    from pydantic import Field, PrivateAttr, validator
-
-from prefect_gcp.credentials import GcpCredentials
-from prefect_gcp.models.cloud_run_v2 import CloudRunJobV2Result, ExecutionV2, JobV2
-from prefect_gcp.utilities import slugify_name
 
-if TYPE_CHECKING:
-    from prefect.client.schemas import FlowRun
-    from prefect.server.schemas.core import Flow
-    from prefect.server.schemas.responses import DeploymentResponse
+@pytest.fixture(autouse=True)
+def mock_credentials(gcp_credentials):
+    yield
 
 
-def _get_default_job_body_template() -> Dict[str, Any]:
-    """
-    Returns the default job body template for the Cloud Run worker.
-
-    Returns:
-        The default job body template.
-    """
+@pytest.fixture
+def jobs_body():
     return {
-        "client": "prefect",
-        "launchStage": "{{ launch_stage }}",
-        "template": {
-            "template": {
-                "serviceAccount": "{{ service_account_name }}",
-                "maxRetries": "{{ max_retries }}",
-                "timeout": "{{ timeout }}",
-                "vpcAccess": {"connector": "{{ vpc_connector_name }}"},
-                "containers": [
-                    {
-                        "env": [],
-                        "image": "{{ image }}",
-                        "command": "{{ command }}",
-                        "args": "{{ args }}",
-                        "resources": {
-                            "limits": {
-                                "cpu": "{{ cpu }}",
-                                "memory": "{{ memory }}",
-                            },
-                        },
+        "apiVersion": "run.googleapis.com/v1",
+        "kind": "Job",
+        "metadata": {
+            "annotations": {
+                # See: https://cloud.google.com/run/docs/troubleshooting#launch-stage-validation  # noqa
+                "run.googleapis.com/launch-stage": "BETA",
+            },
+        },
+        "spec": {  # JobSpec
+            "template": {  # ExecutionTemplateSpec
+                "spec": {  # ExecutionSpec
+                    "template": {  # TaskTemplateSpec
+                        "spec": {"containers": [{}]},  # TaskSpec
                     },
-                ],
-            }
+                },
+            },
         },
     }
 
 
-def _get_base_job_body() -> Dict[str, Any]:
-    """
-    Returns the base job body for the Cloud Run worker's job body validation.
-
-    Returns:
-        The base job body.
-    """
-    return {
-        "template": {
-            "template": {
-                "containers": [],
-            },
-        },
-    }
+@pytest.fixture
+def flow_run():
+    return FlowRun(flow_id=uuid.uuid4(), name="my-flow-run-name")
 
 
-class CloudRunWorkerJobV2Configuration(BaseJobConfiguration):
-    """
-    The configuration for the Cloud Run worker V2.
-
-    The schema for this class is used to populate the `job_body` section of the
-    default base job template.
-    """
-
-    credentials: GcpCredentials = Field(
-        title="GCP Credentials",
-        default_factory=GcpCredentials,
-        description=(
-            "The GCP Credentials used to connect to Cloud Run. "
-            "If not provided credentials will be inferred from "
-            "the local environment."
-        ),
-    )
-    job_body: Dict[str, Any] = Field(
-        template=_get_default_job_body_template(),
-    )
-    keep_job: bool = Field(
-        default=False,
-        title="Keep Job After Completion",
-        description="Keep the completed Cloud run job on Google Cloud Platform.",
+@pytest.fixture
+def cloud_run_worker_job_config(service_account_info, jobs_body):
+    return CloudRunWorkerJobConfiguration(
+        name="my-job-name",
+        region="middle-earth2",
+        job_body=jobs_body,
+        credentials=GcpCredentials(service_account_info=service_account_info),
     )
-    region: str = Field(
-        default="us-central1",
-        description="The region in which to run the Cloud Run job",
-    )
-    timeout: int = Field(
-        default=600,
-        gt=0,
-        le=86400,
-        description=(
-            "The length of time that Prefect will wait for a Cloud Run Job to "
-            "complete before raising an exception."
-        ),
-    )
-    _job_name: str = PrivateAttr(default=None)
 
-    @property
-    def project(self) -> str:
-        """
-        Returns the GCP project associated with the credentials.
 
-        Returns:
-            str: The GCP project associated with the credentials.
-        """
-        return self.credentials.project
+@pytest.fixture
+def cloud_run_worker_job_config_noncompliant_name(service_account_info, jobs_body):
+    return CloudRunWorkerJobConfiguration(
+        name="MY_JOB_NAME",
+        region="middle-earth2",
+        job_body=jobs_body,
+        credentials=GcpCredentials(service_account_info=service_account_info),
+    )
 
-    @property
-    def job_name(self) -> str:
-        """
-        Returns the name of the job.
 
-        Returns:
-            str: The name of the job.
-        """
-        if self._job_name is None:
-            base_job_name = slugify_name(self.name)
-            job_name = f"{base_job_name}-{uuid4().hex}"
-            self._job_name = job_name
+class TestCloudRunWorkerJobConfiguration:
+    def test_job_name(self, cloud_run_worker_job_config):
+        cloud_run_worker_job_config.job_body["metadata"]["name"] = "my-job-name"
+        assert cloud_run_worker_job_config.job_name == "my-job-name"
 
-        return self._job_name
+    def test_job_name_is_slug(self, cloud_run_worker_job_config_noncompliant_name):
+        cloud_run_worker_job_config_noncompliant_name._populate_name_if_not_present()
+        assert cloud_run_worker_job_config_noncompliant_name.job_name[
+            :-33
+        ] == slugify_name("MY_JOB_NAME")
 
-    def prepare_for_flow_run(
+    def test_populate_envs(
         self,
-        flow_run: "FlowRun",
-        deployment: Optional["DeploymentResponse"] = None,
-        flow: Optional["Flow"] = None,
+        cloud_run_worker_job_config,
     ):
-        """
-        Prepares the job configuration for a flow run.
-
-        Ensures that necessary values are present in the job body and that the
-        job body is valid.
-
-        Args:
-            flow_run: The flow run to prepare the job configuration for
-            deployment: The deployment associated with the flow run used for
-                preparation.
-            flow: The flow associated with the flow run used for preparation.
-        """
-        super().prepare_for_flow_run(
-            flow_run=flow_run,
-            deployment=deployment,
-            flow=flow,
+        container = cloud_run_worker_job_config.job_body["spec"]["template"]["spec"][
+            "template"
+        ]["spec"]["containers"][0]
+
+        assert "env" not in container
+        assert cloud_run_worker_job_config.env == {}
+        cloud_run_worker_job_config.env = {"a": "b"}
+
+        cloud_run_worker_job_config._populate_envs()
+
+        assert "env" in container
+        assert len(container["env"]) == 1
+        assert container["env"][0]["name"] == "a"
+        assert container["env"][0]["value"] == "b"
+
+    def test_populate_image_if_not_present(self, cloud_run_worker_job_config):
+        cloud_run_worker_job_config._populate_image_if_not_present()
+
+        assert (
+            cloud_run_worker_job_config.job_body["spec"]["template"]["spec"][
+                "template"
+            ]["spec"]["containers"][0]["image"]
+            == f"docker.io/{get_prefect_image_name()}"
         )
 
-        self._populate_env()
-        self._populate_or_format_command()
-        self._format_args_if_present()
-        self._populate_image_if_not_present()
-        self._populate_timeout()
-        self._remove_vpc_access_if_unset()
+    def test_populate_image_doesnt_overwrite(self, cloud_run_worker_job_config):
+        image = "my-first-image"
+        container = cloud_run_worker_job_config.job_body["spec"]["template"]["spec"][
+            "template"
+        ]["spec"]["containers"][0]
+        container["image"] = image
 
-    def _populate_timeout(self):
-        """
-        Populates the job body with the timeout.
-        """
-        self.job_body["template"]["template"]["timeout"] = f"{self.timeout}s"
-
-    def _populate_env(self):
-        """
-        Populates the job body with environment variables.
-        """
-        envs = [{"name": k, "value": v} for k, v in self.env.items()]
+        cloud_run_worker_job_config._populate_image_if_not_present()
 
-        self.job_body["template"]["template"]["containers"][0]["env"] = envs
+        assert container["image"] == image
 
-    def _populate_image_if_not_present(self):
-        """
-        Populates the job body with the image if not present.
-        """
-        if "image" not in self.job_body["template"]["template"]["containers"][0]:
-            self.job_body["template"]["template"]["containers"][0][
-                "image"
-            ] = f"docker.io/{get_prefect_image_name()}"
+    def test_populate_name_if_not_present(self, cloud_run_worker_job_config):
+        metadata = cloud_run_worker_job_config.job_body["metadata"]
 
-    def _populate_or_format_command(self):
-        """
-        Populates the job body with the command if not present.
-        """
-        command = self.job_body["template"]["template"]["containers"][0].get("command")
+        assert "name" not in metadata
 
-        if command is None:
-            self.job_body["template"]["template"]["containers"][0][
-                "command"
-            ] = shlex.split(self._base_flow_run_command())
-        elif isinstance(command, str):
-            self.job_body["template"]["template"]["containers"][0][
-                "command"
-            ] = shlex.split(command)
+        cloud_run_worker_job_config._populate_name_if_not_present()
 
-    def _format_args_if_present(self):
-        """
-        Formats the job body args if present.
-        """
-        args = self.job_body["template"]["template"]["containers"][0].get("args")
+        assert "name" in metadata
+        assert metadata["name"][:-33] == cloud_run_worker_job_config.name
 
-        if args is not None and isinstance(args, str):
-            self.job_body["template"]["template"]["containers"][0][
-                "args"
-            ] = shlex.split(args)
+    def test_job_name_different_after_retry(self, cloud_run_worker_job_config):
+        metadata = cloud_run_worker_job_config.job_body["metadata"]
 
-    def _remove_vpc_access_if_unset(self):
-        """
-        Removes vpcAccess if unset.
-        """
+        assert "name" not in metadata
 
-        if "vpcAccess" not in self.job_body["template"]["template"]:
-            return
+        cloud_run_worker_job_config._populate_name_if_not_present()
+        job_name_1 = metadata.pop("name")
 
-        vpc_access = self.job_body["template"]["template"]["vpcAccess"]
+        cloud_run_worker_job_config._populate_name_if_not_present()
+        job_name_2 = metadata.pop("name")
 
-        # if vpcAccess is unset or connector is unset, remove the entire vpcAccess block
-        # otherwise leave the user provided value.
-        if not vpc_access or (
-            len(vpc_access) == 1
-            and "connector" in vpc_access
-            and vpc_access["connector"] is None
-        ):
-            self.job_body["template"]["template"].pop("vpcAccess")
-
-    # noinspection PyMethodParameters
-    @validator("job_body")
-    def _ensure_job_includes_all_required_components(cls, value: Dict[str, Any]):
-        """
-        Ensures that the job body includes all required components.
+        assert job_name_1[:-33] == job_name_2[:-33]
+        assert job_name_1 != job_name_2
 
-        Args:
-            value: The job body to validate.
-        Returns:
-            The validated job body.
-        """
-        patch = JsonPatch.from_diff(value, _get_base_job_body())
+    def test_populate_or_format_command_doesnt_exist(self, cloud_run_worker_job_config):
+        container = cloud_run_worker_job_config.job_body["spec"]["template"]["spec"][
+            "template"
+        ]["spec"]["containers"][0]
 
-        missing_paths = sorted([op["path"] for op in patch if op["op"] == "add"])
+        assert "command" not in container
 
-        if missing_paths:
-            raise ValueError(
-                f"Job body is missing required components: {', '.join(missing_paths)}"
-            )
+        cloud_run_worker_job_config._populate_or_format_command()
 
-        return value
+        assert "command" in container
+        assert container["command"] == ["prefect", "flow-run", "execute"]
 
-    # noinspection PyMethodParameters
-    @validator("job_body")
-    def _ensure_job_has_compatible_values(cls, value: Dict[str, Any]):
-        """Ensure that the job body has compatible values."""
-        patch = JsonPatch.from_diff(value, _get_base_job_body())
-        incompatible = sorted(
-            [
-                f"{op['path']} must have value {op['value']!r}"
-                for op in patch
-                if op["op"] == "replace"
-            ]
-        )
-        if incompatible:
-            raise ValueError(
-                "Job has incompatible values for the following attributes: "
-                f"{', '.join(incompatible)}"
-            )
-        return value
-
-
-class CloudRunWorkerV2Variables(BaseVariables):
-    """
-    Default variables for the Cloud Run worker V2.
-
-    The schema for this class is used to populate the `variables` section of the
-    default base job template.
-    """
-
-    credentials: GcpCredentials = Field(
-        title="GCP Credentials",
-        default_factory=GcpCredentials,
-        description=(
-            "The GCP Credentials used to connect to Cloud Run. "
-            "If not provided credentials will be inferred from "
-            "the local environment."
-        ),
-    )
-    region: str = Field(
-        default="us-central1",
-        description="The region in which to run the Cloud Run job",
-    )
-    image: Optional[str] = Field(
-        default="prefecthq/prefect:2-latest",
-        title="Image Name",
-        description=(
-            "The image to use for the Cloud Run job. "
-            "If not provided the default Prefect image will be used."
-        ),
-    )
-    args: List[str] = Field(
-        default_factory=list,
-        description=(
-            "The arguments to pass to the Cloud Run Job V2's entrypoint command."
-        ),
-    )
-    keep_job: bool = Field(
-        default=False,
-        title="Keep Job After Completion",
-        description="Keep the completed Cloud run job on Google Cloud Platform.",
-    )
-    launch_stage: Literal[
-        "ALPHA",
-        "BETA",
-        "GA",
-        "DEPRECATED",
-        "EARLY_ACCESS",
-        "PRELAUNCH",
-        "UNIMPLEMENTED",
-        "LAUNCH_TAG_UNSPECIFIED",
-    ] = Field(
-        "BETA",
-        description=(
-            "The launch stage of the Cloud Run Job V2. "
-            "See https://cloud.google.com/run/docs/about-features-categories "
-            "for additional details."
-        ),
-    )
-    max_retries: int = Field(
-        default=0,
-        title="Max Retries",
-        description="The number of times to retry the Cloud Run job.",
-    )
-    cpu: str = Field(
-        default="1000m",
-        title="CPU",
-        description="The CPU to allocate to the Cloud Run job.",
-    )
-    memory: str = Field(
-        default="512Mi",
-        title="Memory",
-        description=(
-            "The memory to allocate to the Cloud Run job along with the units, which"
-            "could be: G, Gi, M, Mi."
-        ),
-        example="512Mi",
-        pattern=r"^\d+(?:G|Gi|M|Mi)$",
-    )
-    timeout: int = Field(
-        default=600,
-        gt=0,
-        le=86400,
-        title="Job Timeout",
-        description=(
-            "The length of time that Prefect will wait for a Cloud Run Job to "
-            "complete before raising an exception (maximum of 86400 seconds, 1 day)."
-        ),
-    )
-    vpc_connector_name: Optional[str] = Field(
-        default=None,
-        title="VPC Connector Name",
-        description="The name of the VPC connector to use for the Cloud Run job.",
-    )
-    service_account_name: Optional[str] = Field(
-        default=None,
-        title="Service Account Name",
-        description=(
-            "The name of the service account to use for the task execution "
-            "of Cloud Run Job. By default Cloud Run jobs run as the default "
-            "Compute Engine Service Account."
-        ),
-        example="service-account@example.iam.gserviceaccount.com",
-    )
+    def test_populate_or_format_command_already_exists(
+        self, cloud_run_worker_job_config
+    ):
+        command = "my command and args"
+        container = cloud_run_worker_job_config.job_body["spec"]["template"]["spec"][
+            "template"
+        ]["spec"]["containers"][0]
+        container["command"] = command
 
+        cloud_run_worker_job_config._populate_or_format_command()
 
-class CloudRunWorkerV2Result(BaseWorkerResult):
-    """
-    The result of a Cloud Run worker V2 job.
-    """
-
-
-class CloudRunWorkerV2(BaseWorker):
-    """
-    The Cloud Run worker V2.
-    """
-
-    type = "cloud-run-v2"
-    job_configuration = CloudRunWorkerJobV2Configuration
-    job_configuration_variables = CloudRunWorkerV2Variables
-    _description = "Execute flow runs within containers on Google Cloud Run (V2 API). Requires a Google Cloud Platform account."  # noqa
-    _display_name = "Google Cloud Run V2"
-    _documentation_url = "https://prefecthq.github.io/prefect-gcp/worker_v2/"
-    _logo_url = "https://images.ctfassets.net/gm98wzqotmnx/4SpnOBvMYkHp6z939MDKP6/549a91bc1ce9afd4fb12c68db7b68106/social-icon-google-cloud-1200-630.png?h=250"  # noqa
+        assert "command" in container
+        assert container["command"] == command.split()
 
-    async def run(
-        self,
-        flow_run: "FlowRun",
-        configuration: CloudRunWorkerJobV2Configuration,
-        task_status: Optional[TaskStatus] = None,
-    ) -> CloudRunJobV2Result:
-        """
-        Runs the flow run on Cloud Run and waits for it to complete.
+    def test_format_args_if_present(self, cloud_run_worker_job_config):
+        args = "my args"
+        container = cloud_run_worker_job_config.job_body["spec"]["template"]["spec"][
+            "template"
+        ]["spec"]["containers"][0]
+        container["args"] = args
 
-        Args:
-            flow_run: The flow run to run.
-            configuration: The configuration for the job.
-            task_status: The task status to update.
+        cloud_run_worker_job_config._format_args_if_present()
 
-        Returns:
-            The result of the job.
-        """
-        logger = self.get_flow_run_logger(flow_run)
+        assert "args" in container
+        assert container["args"] == args.split()
 
-        with self._get_client(configuration=configuration) as cr_client:
-            await run_sync_in_worker_thread(
-                self._create_job_and_wait_for_registration,
-                configuration=configuration,
-                cr_client=cr_client,
-                logger=logger,
-            )
+    def test_format_args_if_present_no_args(self, cloud_run_worker_job_config):
+        container = cloud_run_worker_job_config.job_body["spec"]["template"]["spec"][
+            "template"
+        ]["spec"]["containers"][0]
+        assert "args" not in container
 
-            execution = await run_sync_in_worker_thread(
-                self._begin_job_execution,
-                configuration=configuration,
-                cr_client=cr_client,
-                logger=logger,
-            )
+        cloud_run_worker_job_config._format_args_if_present()
 
-            if task_status:
-                task_status.started(configuration.job_name)
+        assert "args" not in container
 
-            result = await run_sync_in_worker_thread(
-                self._watch_job_execution_and_get_result,
-                configuration=configuration,
-                cr_client=cr_client,
-                execution=execution,
-                logger=logger,
-            )
-
-            return result
-
-    async def kill_infrastructure(
-        self,
-        infrastructure_pid: str,
-        configuration: CloudRunWorkerJobV2Configuration,
-        grace_seconds: int = 30,
+    def test_populate_name_doesnt_overwrite(
+        self, cloud_run_worker_job_config, flow_run
     ):
-        """
-        Stops the Cloud Run job.
-
-        Args:
-            infrastructure_pid: The ID of the infrastructure to stop.
-            configuration: The configuration for the job.
-            grace_seconds: The number of seconds to wait before stopping the job.
-        """
-        if grace_seconds != 30:
-            self._logger.warning(
-                f"Kill grace period of {grace_seconds}s requested, but GCP does not "
-                "support dynamic grace period configuration. See here for more info: "
-                "https://cloud.google.com/run/docs/reference/rest/v1/namespaces.jobs/delete"  # noqa
-            )
-
-        with self._get_client(configuration=configuration) as cr_client:
-            await run_sync_in_worker_thread(
-                self._stop_job,
-                cr_client=cr_client,
-                configuration=configuration,
-                job_name=infrastructure_pid,
-            )
-
-    @staticmethod
-    def _get_client(
-        configuration: CloudRunWorkerJobV2Configuration,
-    ) -> ResourceWarning:
-        """
-        Get the base client needed for interacting with GCP Cloud Run V2 API.
+        name = "my-name"
+        metadata = cloud_run_worker_job_config.job_body["metadata"]
+        metadata["name"] = name
+
+        cloud_run_worker_job_config._populate_name_if_not_present()
+
+        assert "name" in metadata
+        assert metadata["name"] != flow_run.name
+        assert metadata["name"] == name
+
+    async def test_validates_against_an_empty_job_body(self):
+        template = CloudRunWorker.get_default_base_job_template()
+        template["job_configuration"]["job_body"] = {}
+        template["job_configuration"]["region"] = "test-region1"
+
+        with pytest.raises(pydantic.ValidationError) as excinfo:
+            await CloudRunWorkerJobConfiguration.from_template_and_values(template, {})
+
+        assert len(err := excinfo.value.errors()) == 1
+        assert err[0]["loc"] == ("job_body",)
+        assert "Value error, Job is missing required attributes" in err[0]["msg"]
+        assert all(
+            key in err[0]["msg"]
+            for key in ["/apiVersion", "/kind", "/metadata", "/spec"]
+        )
 
-        Returns:
-            Resource: The base client needed for interacting with GCP Cloud Run V2 API.
-        """
-        api_endpoint = "https://run.googleapis.com"
-        gcp_creds = configuration.credentials.get_credentials_from_service_account()
+    async def test_validates_for_a_job_body_missing_deeper_attributes(self):
+        template = CloudRunWorker.get_default_base_job_template()
+        template["job_configuration"]["job_body"] = {
+            "apiVersion": "run.googleapis.com/v1",
+            "kind": "Job",
+            "metadata": {},
+            "spec": {"template": {"spec": {"template": {"spec": {}}}}},
+        }
+        template["job_configuration"]["region"] = "test-region1"
+
+        with pytest.raises(pydantic.ValidationError) as excinfo:
+            await CloudRunWorkerJobConfiguration.from_template_and_values(template, {})
+
+        assert len(err := excinfo.value.errors()) == 1
+        assert err[0]["loc"] == ("job_body",)
+        assert "Job is missing required attributes" in err[0]["msg"]
+        assert "/metadata/annotations" in err[0]["msg"]
+        assert "/spec/template/spec/template/spec/containers" in err[0]["msg"]
+
+    async def test_validates_for_a_job_with_incompatible_values(self):
+        """We should give a human-friendly error when the user provides a custom Job
+        manifest that is attempting to change required values."""
+        template = CloudRunWorker.get_default_base_job_template()
+        template["job_configuration"]["region"] = "test-region1"
+        template["job_configuration"]["job_body"] = {
+            "apiVersion": "v1",
+            "kind": "NOTAJOB",
+            "metadata": {
+                "annotations": {
+                    "run.googleapis.com/launch-stage": "NOTABETA",
+                },
+            },
+            "spec": {  # JobSpec
+                "template": {  # ExecutionTemplateSpec
+                    "spec": {  # ExecutionSpec
+                        "template": {  # TaskTemplateSpec
+                            "spec": {"containers": [{}]},  # TaskSpec
+                        },
+                    },
+                },
+            },
+        }
 
-        options = ClientOptions(api_endpoint=api_endpoint)
+        with pytest.raises(pydantic.ValidationError) as excinfo:
+            await CloudRunWorkerJobConfiguration.from_template_and_values(template, {})
 
-        return (
-            discovery.build(
-                "run",
-                "v2",
-                client_options=options,
-                credentials=gcp_creds,
-                num_retries=3,  # Set to 3 in case of intermittent/connection issues
-            )
-            .projects()
-            .locations()
+        assert len(err := excinfo.value.errors()) == 1
+        assert err[0]["loc"] == ("job_body",)
+        assert "/apiVersion must have value 'run.googleapis.com/v1'" in err[0]["msg"]
+        assert "/kind must have value 'Job'" in err[0]["msg"]
+        assert (
+            "/metadata/annotations/run.googleapis.com~1launch-stage must have value 'BETA'"
+            in err[0]["msg"]
         )
 
-    def _create_job_and_wait_for_registration(
-        self,
-        configuration: CloudRunWorkerJobV2Configuration,
-        cr_client: Resource,
-        logger: PrefectLogAdapter,
-    ):
-        """
-        Creates the Cloud Run job and waits for it to register.
-
-        Args:
-            configuration: The configuration for the job.
-            cr_client: The Cloud Run client.
-            logger: The logger to use.
-        """
-        try:
-            logger.info(f"Creating Cloud Run JobV2 {configuration.job_name}")
-
-            JobV2.create(
-                cr_client=cr_client,
-                project=configuration.project,
-                location=configuration.region,
-                job_id=configuration.job_name,
-                body=configuration.job_body,
-            )
-        except HttpError as exc:
-            self._create_job_error(
-                exc=exc,
-                configuration=configuration,
-            )
 
-        try:
-            self._wait_for_job_creation(
-                cr_client=cr_client,
-                configuration=configuration,
-                logger=logger,
-            )
-        except Exception as exc:
-            logger.critical(
-                f"Failed to create Cloud Run JobV2 {configuration.job_name}.\n{exc}"
+class TestCloudRunWorkerValidConfiguration:
+    @pytest.mark.parametrize("cpu", ["1", "100", "100m", "1500m"])
+    def test_invalid_cpu_string(self, cpu):
+        deployment = DeploymentCreate(
+            name="my-deployment",
+            flow_id=uuid.uuid4(),
+            job_variables={"region": "test-region1", "cpu": cpu},
+        )
+        with pytest.raises(PrefectValidationError) as exc:
+            deployment.check_valid_configuration(
+                CloudRunWorker.get_default_base_job_template()
             )
 
-            if not configuration.keep_job:
-                try:
-                    JobV2.delete(
-                        cr_client=cr_client,
-                        project=configuration.project,
-                        location=configuration.region,
-                        job_name=configuration.job_name,
-                    )
-                except Exception as exc2:
-                    logger.critical(
-                        f"Failed to delete Cloud Run JobV2 {configuration.job_name}."
-                        f"\n{exc2}"
-                    )
-
-            raise
-
-    @staticmethod
-    def _wait_for_job_creation(
-        cr_client: Resource,
-        configuration: CloudRunWorkerJobV2Configuration,
-        logger: PrefectLogAdapter,
-        poll_interval: int = 5,
-    ):
-        """
-        Waits for the Cloud Run job to be created.
+        assert f"'{cpu}' does not match '^(\\\\d*000)m$'" in str(exc.value)
+
+    @pytest.mark.parametrize("cpu", ["1000m", "2000m", "3000m"])
+    def test_valid_cpu_string(self, cpu):
+        deployment = DeploymentCreate(
+            name="my-deployment",
+            flow_id=uuid.uuid4(),
+            job_variables={"region": "test-region1", "cpu": cpu},
+        )
+        deployment.check_valid_configuration(
+            CloudRunWorker.get_default_base_job_template()
+        )
 
-        Args:
-            cr_client: The Cloud Run client.
-            configuration: The configuration for the job.
-            logger: The logger to use.
-            poll_interval: The interval to poll the Cloud Run job, defaults to 5
-                seconds.
-        """
-        job = JobV2.get(
-            cr_client=cr_client,
-            project=configuration.project,
-            location=configuration.region,
-            job_name=configuration.job_name,
+    @pytest.mark.parametrize("memory", ["1", "100", "100Gigs"])
+    def test_invalid_memory_string(self, memory):
+        deployment = DeploymentCreate(
+            name="my-deployment",
+            flow_id=uuid.uuid4(),
+            job_variables={"region": "test-region1", "memory": memory},
+        )
+        with pytest.raises(PrefectValidationError) as exc:
+            deployment.check_valid_configuration(
+                CloudRunWorker.get_default_base_job_template()
+            )
+        assert f"'{memory}' does not match '^\\\\d+(?:G|Gi|M|Mi)$'" in str(exc.value)
+
+    @pytest.mark.parametrize("memory", ["512G", "512Gi", "512M", "512Mi"])
+    def test_valid_memory_string(self, memory):
+        deployment = DeploymentCreate(
+            name="my-deployment",
+            flow_id=uuid.uuid4(),
+            job_variables={"region": "test-region1", "memory": memory},
+        )
+        deployment.check_valid_configuration(
+            CloudRunWorker.get_default_base_job_template()
         )
 
-        t0 = time.time()
 
-        while not job.is_ready():
-            if not (ready_condition := job.get_ready_condition()):
-                ready_condition = "waiting for condition update"
-
-            logger.info(f"Current Job Condition: {ready_condition}")
-
-            job = JobV2.get(
-                cr_client=cr_client,
-                project=configuration.project,
-                location=configuration.region,
-                job_name=configuration.job_name,
-            )
+executions_return_value = {
+    "metadata": {"name": "test-name", "namespace": "test-namespace"},
+    "spec": {"MySpec": "spec"},
+    "status": {"logUri": "test-log-uri"},
+}
 
-            elapsed_time = time.time() - t0
+jobs_return_value = {
+    "metadata": {"name": "Test", "namespace": "test-namespace"},
+    "spec": {"MySpec": "spec"},
+    "status": {
+        "conditions": [{"type": "Ready", "dog": "cat"}],
+        "latestCreatedExecution": {"puppy": "kitty"},
+    },
+}
 
-            if elapsed_time > configuration.timeout:
-                raise RuntimeError(
-                    f"Timeout of {configuration.timeout} seconds reached while "
-                    f"waiting for Cloud Run Job V2 {configuration.job_name} to be "
-                    "created."
-                )
 
-            time.sleep(poll_interval)
+@pytest.fixture
+def mock_client(monkeypatch, mock_credentials):
+    m = Mock(name="MockClient")
 
-    @staticmethod
-    def _create_job_error(
-        exc: HttpError,
-        configuration: CloudRunWorkerJobV2Configuration,
-    ):
-        """
-        Creates a formatted error message for the Cloud Run V2 API errors
-        """
-        # noinspection PyUnresolvedReferences
-        if exc.status_code == 404:
-            raise RuntimeError(
-                f"Failed to find resources at {exc.uri}. Confirm that region"
-                f" '{configuration.region}' is the correct region for your Cloud"
-                f" Run Job and that {configuration.project} is the correct GCP "
-                f" project. If your project ID is not correct, you are using a "
-                f"Credentials block with permissions for the wrong project."
-            ) from exc
+    def mock_enter(m, *args, **kwargs):
+        return m
 
-        raise exc
+    def mock_exit(m, *args, **kwargs):
+        pass
 
-    def _begin_job_execution(
-        self,
-        cr_client: Resource,
-        configuration: CloudRunWorkerJobV2Configuration,
-        logger: PrefectLogAdapter,
-    ) -> ExecutionV2:
-        """
-        Begins the Cloud Run job execution.
+    m.__enter__ = mock_enter
+    m.__exit__ = mock_exit
 
-        Args:
-            cr_client: The Cloud Run client.
-            configuration: The configuration for the job.
-            logger: The logger to use.
+    def get_mock_client(*args, **kwargs):
+        return m
 
-        Returns:
-            The Cloud Run job execution.
-        """
-        try:
-            logger.info(
-                f"Submitting Cloud Run Job V2 {configuration.job_name} for execution..."
-            )
+    monkeypatch.setattr(
+        "prefect_gcp.workers.cloud_run.CloudRunWorker._get_client",
+        get_mock_client,
+    )
 
-            submission = JobV2.run(
-                cr_client=cr_client,
-                project=configuration.project,
-                location=configuration.region,
-                job_name=configuration.job_name,
-            )
+    return m
 
-            job_execution = ExecutionV2.get(
-                cr_client=cr_client,
-                execution_id=submission["metadata"]["name"],
-            )
 
-            command = (
-                " ".join(configuration.command)
-                if configuration.command
-                else "default container command"
-            )
+class MockExecution(Mock):
+    call_count = 0
 
-            logger.info(
-                f"Cloud Run Job V2 {configuration.job_name} submitted for execution "
-                f"with command: {command}"
-            )
+    def __init__(self, succeeded=False, *args, **kwargs):
+        super().__init__()
+        self.log_uri = "test_uri"
+        self._succeeded = succeeded
 
-            return job_execution
-        except Exception as exc:
-            self._job_run_submission_error(
-                exc=exc,
-                configuration=configuration,
-            )
-            raise
+    def is_running(self):
+        MockExecution.call_count += 1
 
-    def _watch_job_execution_and_get_result(
-        self,
-        cr_client: Resource,
-        configuration: CloudRunWorkerJobV2Configuration,
-        execution: ExecutionV2,
-        logger: PrefectLogAdapter,
-        poll_interval: int = 5,
-    ) -> CloudRunJobV2Result:
-        """
-        Watch the job execution and get the result.
+        if self.call_count > 2:
+            return False
+        return True
 
-        Args:
-            cr_client (Resource): The base client needed for interacting with GCP
-                Cloud Run V2 API.
-            configuration (CloudRunWorkerJobV2Configuration): The configuration for
-                the job.
-            execution (ExecutionV2): The execution to watch.
-            logger (PrefectLogAdapter): The logger to use.
-            poll_interval (int): The number of seconds to wait between polls.
-                Defaults to 5 seconds.
+    def condition_after_completion(self):
+        return {"message": "test"}
 
-        Returns:
-            The result of the job.
-        """
-        try:
-            execution = self._watch_job_execution(
-                cr_client=cr_client,
-                configuration=configuration,
-                execution=execution,
-                poll_interval=poll_interval,
-            )
-        except Exception as exc:
-            logger.critical(
-                f"Encountered an exception while waiting for job run completion - "
-                f"{exc}"
-            )
-            raise
+    def succeeded(self):
+        return self._succeeded
 
-        if execution.succeeded():
-            status_code = 0
-            logger.info(f"Cloud Run Job V2 {configuration.job_name} succeeded")
-        else:
-            status_code = 1
-            error_mg = execution.condition_after_completion().get("message")
-            logger.error(
-                f"Cloud Run Job V2 {configuration.job_name} failed - {error_mg}"
-            )
+    @classmethod
+    def get(cls, *args, **kwargs):
+        return cls()
 
-        logger.info(f"Job run logs can be found on GCP at: {execution.logUri}")
 
-        if not configuration.keep_job:
-            logger.info(
-                f"Deleting completed Cloud Run Job {configuration.job_name!r} from "
-                "Google Cloud Run..."
-            )
+def list_mock_calls(mock_client, assigned_calls=0):
+    calls = []
+    for call in mock_client.mock_calls:
+        # mock `call.jobs().get()` results in two calls: `call.jobs()` and
+        # `call.jobs().get()`, so we want to remove the first, smaller
+        # call.
+        if len(str(call).split(".")) > 2:
+            calls.append(str(call))
+    # assigning a return value to a call results in initial
+    # mock calls which are not actually made
+    actual_calls = calls[assigned_calls:]
 
-            try:
-                JobV2.delete(
-                    cr_client=cr_client,
-                    project=configuration.project,
-                    location=configuration.region,
-                    job_name=configuration.job_name,
-                )
-            except Exception as exc:
-                logger.critical(
-                    "Received an exception while deleting the Cloud Run Job V2 "
-                    f"- {configuration.job_name} - {exc}"
-                )
+    return actual_calls
 
-        return CloudRunJobV2Result(
-            identifier=configuration.job_name,
-            status_code=status_code,
-        )
 
-    # noinspection DuplicatedCode
-    @staticmethod
-    def _watch_job_execution(
-        cr_client: Resource,
-        configuration: CloudRunWorkerJobV2Configuration,
-        execution: ExecutionV2,
-        poll_interval: int,
-    ) -> ExecutionV2:
-        """
-        Update execution status until it is no longer running or timeout is reached.
-
-        Args:
-            cr_client (Resource): The base client needed for interacting with GCP
-                Cloud Run V2 API.
-            configuration (CloudRunWorkerJobV2Configuration): The configuration for
-                the job.
-            execution (ExecutionV2): The execution to watch.
-            poll_interval (int): The number of seconds to wait between polls.
-
-        Returns:
-            The execution.
-        """
-        t0 = time.time()
+class TestCloudRunWorker:
+    job_ready = {
+        "metadata": {"name": "Test", "namespace": "test-namespace"},
+        "spec": {"MySpec": "spec"},
+        "status": {
+            "conditions": [{"type": "Ready", "status": "True"}],
+            "latestCreatedExecution": {"puppy": "kitty"},
+        },
+    }
+    execution_ready = {
+        "metadata": {"name": "test-name", "namespace": "test-namespace"},
+        "spec": {"MySpec": "spec"},
+        "status": {"logUri": "test-log-uri"},
+    }
+    execution_complete_and_succeeded = {
+        "metadata": {"name": "test-name", "namespace": "test-namespace"},
+        "spec": {"MySpec": "spec"},
+        "status": {
+            "logUri": "test-log-uri",
+            "completionTime": "Done!",
+            "conditions": [{"type": "Completed", "status": "True"}],
+        },
+    }
+    execution_not_found = {
+        "metadata": {"name": "test-name", "namespace": "test-namespace"},
+        "spec": {"MySpec": "spec"},
+        "status": {
+            "logUri": "test-log-uri",
+            "completionTime": "Done!",
+            "conditions": [
+                {"type": "Completed", "status": "False", "message": "Not found"}
+            ],
+        },
+    }
+    execution_complete_and_failed = {
+        "metadata": {"name": "test-name", "namespace": "test-namespace"},
+        "spec": {"MySpec": "spec"},
+        "status": {
+            "logUri": "test-log-uri",
+            "completionTime": "Done!",
+            "conditions": [
+                {"type": "Completed", "status": "False", "message": "test failure"}
+            ],
+        },
+    }
 
-        while execution.is_running():
-            execution = ExecutionV2.get(
-                cr_client=cr_client,
-                execution_id=execution.name,
+    @pytest.mark.parametrize(
+        "keep_job,expected_calls",
+        [
+            (
+                True,
+                [
+                    "call.jobs().create",
+                    "call.jobs().create().execute()",
+                ],
+            ),
+            (
+                False,
+                [
+                    "call.jobs().create",
+                    "call.jobs().create().execute()",
+                    "call.jobs().get",
+                    "call.jobs().get().execute()",
+                    "call.jobs().run",
+                    "call.jobs().run().execute()",
+                ],
+            ),
+        ],
+    )
+    async def test_happy_path_api_calls_made_correctly(
+        self,
+        mock_client,
+        cloud_run_worker_job_config,
+        keep_job,
+        flow_run,
+        expected_calls,
+    ):
+        """Expected behavior:
+        Happy path:
+        - A call to Job.create and execute
+        - A call to Job.get and execute (check status)
+        - A call to Job.run and execute (start the job when status is ready)
+        - A call to Executions.get and execute (see the status of the Execution)
+        - A call to Job.delete and execute if `keep_job` False, otherwise no call
+        """
+        async with CloudRunWorker("my-work-pool") as cloud_run_worker:
+            cloud_run_worker_job_config.keep_job = keep_job
+            cloud_run_worker_job_config.prepare_for_flow_run(flow_run, None, None)
+            mock_client.jobs().get().execute.return_value = self.job_ready
+            mock_client.jobs().run().execute.return_value = self.job_ready
+            mock_client.executions().get().execute.return_value = (
+                self.execution_complete_and_succeeded
             )
+            await cloud_run_worker.run(flow_run, cloud_run_worker_job_config)
+            calls = list_mock_calls(mock_client, 3)
 
-            elapsed_time = time.time() - t0
+            for call, expected_call in zip(calls, expected_calls):
+                assert call.startswith(expected_call)
 
-            if elapsed_time > configuration.timeout:
-                raise RuntimeError(
-                    f"Timeout of {configuration.timeout} seconds reached while "
-                    f"waiting for Cloud Run Job V2 {configuration.job_name} to "
-                    "complete."
-                )
+    async def test_happy_path_result(
+        self, mock_client, cloud_run_worker_job_config, flow_run
+    ):
+        """Expected behavior: returns a CloudrunJobResult with status_code 0"""
+        async with CloudRunWorker("my-work-pool") as cloud_run_worker:
+            cloud_run_worker_job_config.keep_job = True
+            cloud_run_worker_job_config.prepare_for_flow_run(flow_run, None, None)
+            mock_client.jobs().get().execute.return_value = self.job_ready
+            mock_client.jobs().run().execute.return_value = self.job_ready
+            mock_client.executions().get().execute.return_value = (
+                self.execution_complete_and_succeeded
+            )
+            res = await cloud_run_worker.run(flow_run, cloud_run_worker_job_config)
+            assert isinstance(res, CloudRunWorkerResult)
+            assert res.status_code == 0
+
+    @pytest.mark.parametrize(
+        "keep_job,expected_calls",
+        [
+            (
+                True,
+                [
+                    "call.jobs().create",
+                    "call.jobs().create().execute()",
+                ],
+            ),
+            (
+                False,
+                [
+                    "call.jobs().create",
+                    "call.jobs().create().execute()",
+                    "call.jobs().delete",
+                    "call.jobs().delete().execute()",
+                ],
+            ),
+        ],
+    )
+    async def test_behavior_called_when_job_get_fails(
+        self,
+        monkeypatch,
+        mock_client,
+        cloud_run_worker_job_config,
+        flow_run,
+        keep_job,
+        expected_calls,
+    ):
+        """Expected behavior:
+        When job create is called, but there is a subsequent exception on a get,
+        there should be a delete call for that job if `keep_job` is False
+        """
+        async with CloudRunWorker("my-work-pool") as cloud_run_worker:
+            cloud_run_worker_job_config.keep_job = keep_job
+
+            # Getting job will raise error
+            def raise_exception(*args, **kwargs):
+                raise Exception("This is an intentional exception")
+
+            monkeypatch.setattr("prefect_gcp.utilities.Job.get", raise_exception)
+
+            with pytest.raises(Exception):
+                await cloud_run_worker.run(flow_run, cloud_run_worker_job_config)
+            calls = list_mock_calls(mock_client, 0)
+
+            for call, expected_call in zip(calls, expected_calls):
+                assert call.startswith(expected_call)
+
+    # Test that RuntimeError raised if something happens with execution
+    @pytest.mark.parametrize(
+        "keep_job,expected_calls",
+        [
+            (
+                True,
+                [
+                    "call.jobs().create",
+                    "call.jobs().create().execute()",
+                    "call.jobs().get",
+                    "call.jobs().get().execute()",
+                    "call.jobs().run",
+                    "call.jobs().run().execute()",
+                ],
+            ),
+            (
+                False,
+                [
+                    "call.jobs().create",
+                    "call.jobs().create().execute()",
+                    "call.jobs().get",
+                    "call.jobs().get().execute()",
+                    "call.jobs().run",
+                    "call.jobs().run().execute()",
+                    "call.jobs().delete",
+                    "call.jobs().delete().execute()",
+                ],
+            ),
+        ],
+    )
+    async def test_behavior_called_when_execution_get_fails(
+        self,
+        monkeypatch,
+        mock_client,
+        cloud_run_worker_job_config,
+        flow_run,
+        keep_job,
+        expected_calls,
+    ):
+        """Expected behavior:
+        Job creation is called successfully, the job is found when `get` is called,
+        job `run` is called, but the execution fails, there should be a delete
+        call for that job if `keep_job` is False, and an exception should be raised.
+        """
+        async with CloudRunWorker("my-work-pool") as cloud_run_worker:
+            cloud_run_worker_job_config.keep_job = keep_job
+            mock_client.jobs().get().execute.return_value = self.job_ready
+            mock_client.jobs().run().execute.return_value = self.job_ready
+
+            # Getting execution will raise error
+            def raise_exception(*args, **kwargs):
+                raise Exception("This is an intentional exception")
+
+            monkeypatch.setattr("prefect_gcp.utilities.Execution.get", raise_exception)
+
+            with pytest.raises(Exception):
+                await cloud_run_worker.run(flow_run, cloud_run_worker_job_config)
+            calls = list_mock_calls(mock_client, 2)
+            for call, expected_call in zip(calls, expected_calls):
+                assert call.startswith(expected_call)
+
+    async def test_kill(self, mock_client, cloud_run_worker_job_config, flow_run):
+        async with CloudRunWorker("my-work-pool") as cloud_run_worker:
+            cloud_run_worker_job_config.prepare_for_flow_run(flow_run, None, None)
+
+            mock_client.jobs().get().execute.return_value = self.job_ready
+            mock_client.jobs().run().execute.return_value = self.job_ready
+            mock_client.executions().get().execute.return_value = (
+                self.execution_not_found
+            )  # noqa
+
+            with anyio.fail_after(5):
+                async with anyio.create_task_group() as tg:
+                    identifier = await tg.start(
+                        cloud_run_worker.run, flow_run, cloud_run_worker_job_config
+                    )
+                    await cloud_run_worker.kill_infrastructure(
+                        identifier, cloud_run_worker_job_config
+                    )
 
-            time.sleep(poll_interval)
+            actual_calls = list_mock_calls(mock_client=mock_client)
+            assert "call.jobs().delete().execute()" in actual_calls
 
-        return execution
+    def failed_to_get(self):
+        raise HttpError(Mock(reason="does not exist"), content=b"")
 
-    @staticmethod
-    def _job_run_submission_error(
-        exc: Exception,
-        configuration: CloudRunWorkerJobV2Configuration,
+    async def test_kill_not_found(
+        self, mock_client, cloud_run_worker_job_config, flow_run
     ):
-        """
-        Creates a formatted error message for the Cloud Run V2 API errors
+        async with CloudRunWorker("my-work-pool") as cloud_run_worker:
+            cloud_run_worker_job_config.prepare_for_flow_run(flow_run, None, None)
 
-        Args:
-            exc: The exception to format.
-            configuration: The configuration for the job.
-        """
-        # noinspection PyUnresolvedReferences
-        if exc.status_code == 404:
-            pat1 = r"The requested URL [^ ]+ was not found on this server"
-
-            if re.findall(pat1, str(exc)):
-                # noinspection PyUnresolvedReferences
-                raise RuntimeError(
-                    f"Failed to find resources at {exc.uri}. "
-                    f"Confirm that region '{configuration.region}' is "
-                    f"the correct region for your Cloud Run Job "
-                    f"and that '{configuration.project}' is the "
-                    f"correct GCP project. If your project ID is not "
-                    f"correct, you are using a Credentials "
-                    f"block with permissions for the wrong project."
-                ) from exc
-            else:
-                raise exc
+            mock_client.jobs().delete().execute.side_effect = self.failed_to_get
+            with pytest.raises(
+                InfrastructureNotFound, match="Cannot stop Cloud Run Job; the job name"
+            ):
+                await cloud_run_worker.kill_infrastructure(
+                    "non-existent", cloud_run_worker_job_config
+                )
 
-    @staticmethod
-    def _stop_job(
-        cr_client: Resource,
-        configuration: CloudRunWorkerJobV2Configuration,
-        job_name: str,
+    async def test_kill_grace_seconds(
+        self, mock_client, cloud_run_worker_job_config, flow_run, caplog
     ):
-        """
-        Stops/deletes the Cloud Run job.
+        async with CloudRunWorker("my-work-pool") as cloud_run_worker:
+            cloud_run_worker_job_config.prepare_for_flow_run(flow_run, None, None)
 
-        Args:
-            cr_client: The Cloud Run client.
-            configuration: The configuration for the job.
-            job_name: The name of the job to stop.
-        """
-        try:
-            JobV2.delete(
-                cr_client=cr_client,
-                project=configuration.project,
-                location=configuration.region,
-                job_name=job_name,
+            mock_client.jobs().get().execute.return_value = self.job_ready
+            mock_client.jobs().run().execute.return_value = self.job_ready
+            mock_client.executions().get().execute.return_value = (
+                self.execution_not_found
             )
-        except Exception as exc:
-            if "does not exist" in str(exc):
-                raise InfrastructureNotFound(
-                    f"Cannot stop Cloud Run Job; the job name {job_name!r} "
-                    "could not be found."
-                ) from exc
-            raise
+
+            with anyio.fail_after(5):
+                async with anyio.create_task_group() as tg:
+                    identifier = await tg.start(
+                        cloud_run_worker.run, flow_run, cloud_run_worker_job_config
+                    )
+                    await cloud_run_worker.kill_infrastructure(
+                        identifier, cloud_run_worker_job_config, grace_seconds=42
+                    )
+
+            for record in caplog.records:
+                if "Kill grace period of 42s requested, but GCP does not" in record.msg:
+                    break
+            else:
+                raise AssertionError("Expected message not found.")
```

### Comparing `prefect_gcp-0.5.9/prefect_gcp.egg-info/PKG-INFO` & `prefect_gcp-0.6.0rc1/prefect_gcp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 Metadata-Version: 2.1
 Name: prefect-gcp
-Version: 0.5.9
+Version: 0.6.0rc1
 Summary: Prefect integrations for interacting with Google Cloud Platform.
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-gcp
 Keywords: prefect
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: prefect>=2.16.4
+License-File: LICENSE
+Requires-Dist: prefect>=3.0.0rc1
 Requires-Dist: google-api-python-client>=2.20.0
 Requires-Dist: google-cloud-storage>=2.0.0
 Requires-Dist: tenacity>=8.0.0
 Requires-Dist: python-slugify>=8.0.0
+Requires-Dist: google-cloud-secret-manager
 Provides-Extra: cloud-storage
 Requires-Dist: google-cloud-storage; extra == "cloud-storage"
 Provides-Extra: bigquery
 Requires-Dist: google-cloud-bigquery; extra == "bigquery"
 Requires-Dist: google-cloud-bigquery-storage; extra == "bigquery"
 Provides-Extra: secret-manager
 Requires-Dist: google-cloud-secret-manager; extra == "secret-manager"
@@ -47,15 +48,14 @@
 Requires-Dist: google-cloud-secret-manager; extra == "dev"
 Requires-Dist: google-cloud-storage; extra == "dev"
 Requires-Dist: interrogate; extra == "dev"
 Requires-Dist: mkdocs-gen-files; extra == "dev"
 Requires-Dist: mkdocs-material; extra == "dev"
 Requires-Dist: mkdocs; extra == "dev"
 Requires-Dist: mkdocstrings[python]; extra == "dev"
-Requires-Dist: mock; python_version < "3.8" and extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pandas; extra == "dev"
 Requires-Dist: pillow; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pyarrow; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: pytest-xdist; extra == "dev"
```

#### html2text {}

```diff
@@ -1,46 +1,46 @@
-Metadata-Version: 2.1 Name: prefect-gcp Version: 0.5.9 Summary: Prefect
+Metadata-Version: 2.1 Name: prefect-gcp Version: 0.6.0rc1 Summary: Prefect
 integrations for interacting with Google Cloud Platform. Author-email: "Prefect
 Technologies, Inc."
 prefect.io> License: Apache License 2.0 Project-URL: Homepage, https://
 github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-gcp Keywords:
 prefect Classifier: Natural Language :: English Classifier: Intended Audience
 :: Developers Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
-Topic :: Software Development :: Libraries Requires-Python: >=3.8 Description-
-Content-Type: text/markdown Requires-Dist: prefect>=2.16.4 Requires-Dist:
-google-api-python-client>=2.20.0 Requires-Dist: google-cloud-storage>=2.0.0
-Requires-Dist: tenacity>=8.0.0 Requires-Dist: python-slugify>=8.0.0 Provides-
-Extra: cloud-storage Requires-Dist: google-cloud-storage; extra == "cloud-
-storage" Provides-Extra: bigquery Requires-Dist: google-cloud-bigquery; extra
-== "bigquery" Requires-Dist: google-cloud-bigquery-storage; extra == "bigquery"
-Provides-Extra: secret-manager Requires-Dist: google-cloud-secret-manager;
-extra == "secret-manager" Provides-Extra: aiplatform Requires-Dist: google-
-cloud-aiplatform; extra == "aiplatform" Provides-Extra: all-extras Requires-
-Dist: google-cloud-storage; extra == "all-extras" Requires-Dist: google-cloud-
-bigquery; extra == "all-extras" Requires-Dist: google-cloud-bigquery-storage;
-extra == "all-extras" Requires-Dist: google-cloud-secret-manager; extra ==
-"all-extras" Requires-Dist: google-cloud-aiplatform; extra == "all-extras"
-Provides-Extra: dev Requires-Dist: coverage; extra == "dev" Requires-Dist:
-google-cloud-aiplatform; extra == "dev" Requires-Dist: google-cloud-bigquery-
-storage; extra == "dev" Requires-Dist: google-cloud-bigquery; extra == "dev"
-Requires-Dist: google-cloud-secret-manager; extra == "dev" Requires-Dist:
-google-cloud-storage; extra == "dev" Requires-Dist: interrogate; extra == "dev"
-Requires-Dist: mkdocs-gen-files; extra == "dev" Requires-Dist: mkdocs-material;
-extra == "dev" Requires-Dist: mkdocs; extra == "dev" Requires-Dist:
-mkdocstrings[python]; extra == "dev" Requires-Dist: mock; python_version <
-"3.8" and extra == "dev" Requires-Dist: mypy; extra == "dev" Requires-Dist:
-pandas; extra == "dev" Requires-Dist: pillow; extra == "dev" Requires-Dist:
-pre-commit; extra == "dev" Requires-Dist: pyarrow; extra == "dev" Requires-
-Dist: pytest-asyncio; extra == "dev" Requires-Dist: pytest-xdist; extra ==
-"dev" Requires-Dist: pytest; extra == "dev" # `prefect-gcp`
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3.12 Classifier: Topic :: Software Development :: Libraries Requires-
+Python: >=3.9 Description-Content-Type: text/markdown License-File: LICENSE
+Requires-Dist: prefect>=3.0.0rc1 Requires-Dist: google-api-python-
+client>=2.20.0 Requires-Dist: google-cloud-storage>=2.0.0 Requires-Dist:
+tenacity>=8.0.0 Requires-Dist: python-slugify>=8.0.0 Requires-Dist: google-
+cloud-secret-manager Provides-Extra: cloud-storage Requires-Dist: google-cloud-
+storage; extra == "cloud-storage" Provides-Extra: bigquery Requires-Dist:
+google-cloud-bigquery; extra == "bigquery" Requires-Dist: google-cloud-
+bigquery-storage; extra == "bigquery" Provides-Extra: secret-manager Requires-
+Dist: google-cloud-secret-manager; extra == "secret-manager" Provides-Extra:
+aiplatform Requires-Dist: google-cloud-aiplatform; extra == "aiplatform"
+Provides-Extra: all-extras Requires-Dist: google-cloud-storage; extra == "all-
+extras" Requires-Dist: google-cloud-bigquery; extra == "all-extras" Requires-
+Dist: google-cloud-bigquery-storage; extra == "all-extras" Requires-Dist:
+google-cloud-secret-manager; extra == "all-extras" Requires-Dist: google-cloud-
+aiplatform; extra == "all-extras" Provides-Extra: dev Requires-Dist: coverage;
+extra == "dev" Requires-Dist: google-cloud-aiplatform; extra == "dev" Requires-
+Dist: google-cloud-bigquery-storage; extra == "dev" Requires-Dist: google-
+cloud-bigquery; extra == "dev" Requires-Dist: google-cloud-secret-manager;
+extra == "dev" Requires-Dist: google-cloud-storage; extra == "dev" Requires-
+Dist: interrogate; extra == "dev" Requires-Dist: mkdocs-gen-files; extra ==
+"dev" Requires-Dist: mkdocs-material; extra == "dev" Requires-Dist: mkdocs;
+extra == "dev" Requires-Dist: mkdocstrings[python]; extra == "dev" Requires-
+Dist: mypy; extra == "dev" Requires-Dist: pandas; extra == "dev" Requires-Dist:
+pillow; extra == "dev" Requires-Dist: pre-commit; extra == "dev" Requires-Dist:
+pyarrow; extra == "dev" Requires-Dist: pytest-asyncio; extra == "dev" Requires-
+Dist: pytest-xdist; extra == "dev" Requires-Dist: pytest; extra == "dev" #
+`prefect-gcp`
                 _[_P_y_P_I_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_d_m_/_p_r_e_f_e_c_t_-
                       _g_c_p_?_c_o_l_o_r_=_0_0_5_2_F_F_&_l_a_b_e_l_C_o_l_o_r_=_0_9_0_4_2_2_]
 `prefect-gcp` makes it easy to leverage the capabilities of Google Cloud
 Platform (GCP) in your flows, featuring support for Vertex AI, Cloud Run,
 BigQuery, Cloud Storage, and Secret Manager. Visit the full docs [here](https:/
 /PrefectHQ.github.io/prefect-gcp). ### Installation To start using `prefect-
 gcp`: ```bash pip install prefect-gcp ``` To install extras, see [here](https:/
```

### Comparing `prefect_gcp-0.5.9/prefect_gcp.egg-info/SOURCES.txt` & `prefect_gcp-0.6.0rc1/prefect_gcp.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
+LICENSE
+MANIFEST.in
 README.md
 pyproject.toml
 prefect_gcp/__init__.py
 prefect_gcp/_version.py
-prefect_gcp/aiplatform.py
 prefect_gcp/bigquery.py
-prefect_gcp/cloud_run.py
 prefect_gcp/cloud_storage.py
 prefect_gcp/credentials.py
 prefect_gcp/secret_manager.py
 prefect_gcp/utilities.py
 prefect_gcp.egg-info/PKG-INFO
 prefect_gcp.egg-info/SOURCES.txt
 prefect_gcp.egg-info/dependency_links.txt
@@ -20,21 +20,19 @@
 prefect_gcp/models/__init__.py
 prefect_gcp/models/cloud_run_v2.py
 prefect_gcp/workers/__init__.py
 prefect_gcp/workers/cloud_run.py
 prefect_gcp/workers/cloud_run_v2.py
 prefect_gcp/workers/vertex.py
 tests/conftest.py
-tests/test_aiplatform.py
 tests/test_bigquery.py
 tests/test_block_standards.py
-tests/test_cloud_run.py
 tests/test_cloud_run_v2.py
 tests/test_cloud_run_worker.py
 tests/test_cloud_run_worker_v2.py
 tests/test_cloud_storage.py
 tests/test_credentials.py
-tests/test_deprecation.py
 tests/test_secret_manager.py
+tests/test_utilities.py
 tests/test_version.py
 tests/test_vertex_worker.py
 tests/projects/test_steps.py
```

### Comparing `prefect_gcp-0.5.9/prefect_gcp.egg-info/requires.txt` & `prefect_gcp-0.6.0rc1/prefect_gcp.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-prefect>=2.16.4
+prefect>=3.0.0rc1
 google-api-python-client>=2.20.0
 google-cloud-storage>=2.0.0
 tenacity>=8.0.0
 python-slugify>=8.0.0
+google-cloud-secret-manager
 
 [aiplatform]
 google-cloud-aiplatform
 
 [all_extras]
 google-cloud-storage
 google-cloud-bigquery
@@ -38,12 +39,9 @@
 pillow
 pre-commit
 pyarrow
 pytest-asyncio
 pytest-xdist
 pytest
 
-[dev:python_version < "3.8"]
-mock
-
 [secret_manager]
 google-cloud-secret-manager
```

### Comparing `prefect_gcp-0.5.9/pyproject.toml` & `prefect_gcp-0.6.0rc1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,37 +2,37 @@
 requires = ["setuptools>=45", "wheel", "setuptools_scm>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "prefect-gcp"
 description = "Prefect integrations for interacting with Google Cloud Platform."
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 license = { text = "Apache License 2.0" }
 keywords = ["prefect"]
 authors = [{ name = "Prefect Technologies, Inc.", email = "help@prefect.io" }]
 classifiers = [
   "Natural Language :: English",
   "Intended Audience :: Developers",
   "Intended Audience :: System Administrators",
   "License :: OSI Approved :: Apache Software License",
   "Programming Language :: Python :: 3 :: Only",
-  "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Topic :: Software Development :: Libraries",
 ]
 dependencies = [
-  "prefect>=2.16.4",
+  "prefect>=3.0.0rc1",
   "google-api-python-client>=2.20.0",
   "google-cloud-storage>=2.0.0",
   "tenacity>=8.0.0",
   "python-slugify>=8.0.0",
+  "google-cloud-secret-manager",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 cloud_storage = ["google-cloud-storage"]
 bigquery = ["google-cloud-bigquery", "google-cloud-bigquery-storage"]
 secret_manager = ["google-cloud-secret-manager"]
@@ -52,15 +52,14 @@
   "google-cloud-secret-manager",
   "google-cloud-storage",
   "interrogate",
   "mkdocs-gen-files",
   "mkdocs-material",
   "mkdocs",
   "mkdocstrings[python]",
-  "mock; python_version < '3.8'",
   "mypy",
   "pandas",
   "pillow",
   "pre-commit",
   "pyarrow",
   "pytest-asyncio",
   "pytest-xdist",
@@ -72,15 +71,15 @@
 
 [project.entry-points."prefect.collections"]
 prefect_gcp = "prefect_gcp"
 
 [tool.setuptools_scm]
 version_file = "prefect_gcp/_version.py"
 root = "../../.."
-tag_regex = "^prefect-gcp-(?P<version>\\d+\\.\\d+\\.\\d+)$"
+tag_regex = "^prefect-gcp-(?P<version>\\d+\\.\\d+\\.\\d+(?:[a-zA-Z0-9]+(?:\\.[a-zA-Z0-9]+)*)?)$"
 fallback_version = "0.0.0"
 git_describe_command = 'git describe --dirty --tags --long --match "prefect-gcp-*[0-9]*"'
 
 [tool.interrogate]
 ignore-init-module = true
 ignore_init_method = true
 exclude = ["prefect_gcp/_version.py", "tests"]
@@ -92,7 +91,11 @@
 
 [tool.coverage.report]
 fail_under = 80
 show_missing = true
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
+
+filterwarnings = [
+  "ignore:Type google._upb._message.* uses PyType_Spec with a metaclass that has custom tp_new. This is deprecated and will no longer be allowed in Python 3.14:DeprecationWarning",
+]
```

### Comparing `prefect_gcp-0.5.9/tests/conftest.py` & `prefect_gcp-0.6.0rc1/tests/conftest.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 from pathlib import Path
-from unittest.mock import MagicMock
+from unittest.mock import AsyncMock, MagicMock
 
 import pytest
 from google.api_core.exceptions import NotFound as ApiCoreNotFound
 from google.cloud.aiplatform_v1.types.job_state import JobState
 from google.cloud.exceptions import NotFound
 from prefect_gcp.credentials import GcpCredentials
 
@@ -234,26 +234,28 @@
         return name
 
 
 @pytest.fixture
 def mock_credentials(monkeypatch):
     mock_credentials = MagicMock(name="MockGoogleCredentials")
     mock_authenticated_credentials = MagicMock(token="my-token")
-    mock_credentials.from_service_account_info = mock_authenticated_credentials
-    mock_credentials.from_service_account_file = mock_authenticated_credentials
     monkeypatch.setattr(
         "prefect_gcp.credentials.Credentials",  # noqa
         mock_credentials,
     )
     mock_auth = MagicMock()
     mock_auth.default.return_value = (mock_authenticated_credentials, "project")
     monkeypatch.setattr(
         "prefect_gcp.credentials.google.auth",  # noqa
         mock_auth,
     )
+    monkeypatch.setattr(
+        "prefect_gcp.credentials.Credentials.from_service_account_info.universe_domain",  # noqa
+        "fake_universe_domain",
+    )
     return mock_credentials
 
 
 @pytest.fixture
 def job_service_client():
     job_service_client_mock = MagicMock()
     custom_run = MagicMock(name="mock_name")
@@ -267,34 +269,31 @@
         display_name="mock_display_name",
     )
     job_service_client_mock.get_custom_job.return_value = custom_run_final
     return job_service_client_mock
 
 
 @pytest.fixture
-def gcp_credentials(monkeypatch, google_auth, mock_credentials, job_service_client):
-    gcp_credentials_mock = GcpCredentials(project="gcp_credentials_project")
-    gcp_credentials_mock._service_account_email = "my_service_account_email"
-
-    gcp_credentials_mock.cloud_storage_client = CloudStorageClient()
-    gcp_credentials_mock.secret_manager_client = SecretManagerClient()
-    gcp_credentials_mock.job_service_client = job_service_client
-    gcp_credentials_mock.job_service_client.__enter__.return_value = job_service_client
+def job_service_async_client():
+    job_service_client_async_mock = MagicMock()
+    custom_run = MagicMock(name="mock_name")
+    job_service_client_async_mock.create_custom_job = AsyncMock(return_value=custom_run)
 
-    gcp_credentials_mock.get_cloud_storage_client = (
-        lambda *args, **kwargs: gcp_credentials_mock.cloud_storage_client
-    )
-    gcp_credentials_mock.get_bigquery_client = lambda *args, **kwargs: BigQueryClient()
-    gcp_credentials_mock.get_secret_manager_client = (
-        lambda *args, **kwargs: gcp_credentials_mock.secret_manager_client
+    error = MagicMock(message="")
+    custom_run_final = MagicMock(
+        name="mock_name",
+        state=JobState.JOB_STATE_SUCCEEDED,
+        error=error,
+        display_name="mock_display_name",
     )
-    gcp_credentials_mock.get_job_service_client = (
-        lambda *args, **kwargs: gcp_credentials_mock.job_service_client
+    job_service_client_async_mock.get_custom_job = AsyncMock(
+        return_value=custom_run_final
     )
-    return gcp_credentials_mock
+    job_service_client_async_mock.cancel_custom_job = AsyncMock()
+    return job_service_client_async_mock
 
 
 @pytest.fixture()
 def service_account_info(monkeypatch):
     monkeypatch.setattr(
         "google.auth.crypt._cryptography_rsa.serialization.load_pem_private_key",
         lambda *args, **kwargs: args[0],
@@ -319,7 +318,43 @@
             "project_id": "my_project",
             "token_uri": "my-token-uri",
             "client_email": "my-client-email",
             "private_key": "my-private-key",
         }
     )
     return _service_account_info
+
+
+@pytest.fixture
+def gcp_credentials(
+    monkeypatch,
+    google_auth,
+    mock_credentials,
+    job_service_client,
+    job_service_async_client,
+):
+    gcp_credentials_mock = MagicMock(spec=GcpCredentials)
+    gcp_credentials_mock.service_account_info = None
+    gcp_credentials_mock.service_account_info_file = None
+    gcp_credentials_mock.project = "gcp_credentials_project"
+
+    gcp_credentials_mock.get_cloud_storage_client.return_value = CloudStorageClient()
+    gcp_credentials_mock.get_credentials_from_service_account.return_value = (
+        mock_credentials
+    )
+    gcp_credentials_mock._service_account_email = "my_service_account_email"
+
+    gcp_credentials_mock.job_service_client = job_service_client
+    gcp_credentials_mock.job_service_client.__enter__.return_value = job_service_client
+    gcp_credentials_mock.job_service_async_client = job_service_async_client
+    gcp_credentials_mock.job_service_client.__enter__.return_value = (
+        job_service_async_client
+    )
+    gcp_credentials_mock.get_bigquery_client.return_value = BigQueryClient()
+    gcp_credentials_mock.get_secret_manager_client.return_value = SecretManagerClient()
+    gcp_credentials_mock.get_job_service_client.return_value = (
+        gcp_credentials_mock.job_service_client
+    )
+    gcp_credentials_mock.get_job_service_async_client.return_value = (
+        gcp_credentials_mock.job_service_async_client
+    )
+    return gcp_credentials_mock
```

### Comparing `prefect_gcp-0.5.9/tests/projects/test_steps.py` & `prefect_gcp-0.6.0rc1/tests/projects/test_steps.py`

 * *Files identical despite different names*

### Comparing `prefect_gcp-0.5.9/tests/test_bigquery.py` & `prefect_gcp-0.6.0rc1/tests/test_bigquery.py`

 * *Files identical despite different names*

### Comparing `prefect_gcp-0.5.9/tests/test_block_standards.py` & `prefect_gcp-0.6.0rc1/tests/test_block_standards.py`

 * *Files identical despite different names*

### Comparing `prefect_gcp-0.5.9/tests/test_cloud_run_v2.py` & `prefect_gcp-0.6.0rc1/tests/test_cloud_run_v2.py`

 * *Files 13% similar despite different names*

```diff
@@ -34,55 +34,44 @@
         [("CONDITION_SUCCEEDED", True), ("CONDITION_FAILED", False)],
     )
     def test_is_ready(self, state, expected):
         job = JobV2(
             name="test-job",
             uid="12345",
             generation="2",
-            labels={},
-            annotations={},
             createTime="2021-08-31T18:00:00Z",
             updateTime="2021-08-31T18:00:00Z",
             launchStage="BETA",
-            binaryAuthorization={},
-            template={},
             terminalCondition={
                 "type": "Ready",
                 "state": state,
             },
             conditions=[],
             executionCount=1,
-            latestCreatedExecution={},
             reconciling=False,
             satisfiesPzs=False,
             etag="etag-12345",
         )
 
         assert job.is_ready() == expected
 
     def test_is_ready_raises_exception(self):
         job = JobV2(
             name="test-job",
             uid="12345",
             generation="2",
-            labels={},
-            annotations={},
             createTime="2021-08-31T18:00:00Z",
             updateTime="2021-08-31T18:00:00Z",
             launchStage="BETA",
-            binaryAuthorization={},
-            template={},
             terminalCondition={
                 "type": "Ready",
                 "state": "CONTAINER_FAILED",
                 "reason": "ContainerMissing",
             },
-            conditions=[],
             executionCount=1,
-            latestCreatedExecution={},
             reconciling=False,
             satisfiesPzs=False,
             etag="etag-12345",
         )
 
         with pytest.raises(Exception):
             job.is_ready()
@@ -110,25 +99,19 @@
         ],
     )
     def test_get_ready_condition(self, terminal_condition, expected):
         job = JobV2(
             name="test-job",
             uid="12345",
             generation="2",
-            labels={},
-            annotations={},
             createTime="2021-08-31T18:00:00Z",
             updateTime="2021-08-31T18:00:00Z",
             launchStage="BETA",
-            binaryAuthorization={},
-            template={},
             terminalCondition=terminal_condition,
-            conditions=[],
             executionCount=1,
-            latestCreatedExecution={},
             reconciling=False,
             satisfiesPzs=False,
             etag="etag-12345",
         )
 
         assert job.get_ready_condition() == expected
 
@@ -151,25 +134,18 @@
         ],
     )
     def test_is_missing_container(self, ready_condition, expected):
         job = JobV2(
             name="test-job",
             uid="12345",
             generation="2",
-            labels={},
-            annotations={},
             createTime="2021-08-31T18:00:00Z",
             updateTime="2021-08-31T18:00:00Z",
             launchStage="BETA",
-            binaryAuthorization={},
-            template={},
-            terminalCondition={},
-            conditions=[],
             executionCount=1,
-            latestCreatedExecution={},
             reconciling=False,
             satisfiesPzs=False,
             etag="etag-12345",
         )
 
         assert job._is_missing_container(ready_condition=ready_condition) == expected
```

### Comparing `prefect_gcp-0.5.9/tests/test_cloud_run_worker_v2.py` & `prefect_gcp-0.6.0rc1/tests/test_cloud_run_worker_v2.py`

 * *Files identical despite different names*

### Comparing `prefect_gcp-0.5.9/tests/test_cloud_storage.py` & `prefect_gcp-0.6.0rc1/tests/test_cloud_storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,14 @@
     cloud_storage_download_blob_as_bytes,
     cloud_storage_download_blob_to_file,
     cloud_storage_upload_blob_from_file,
     cloud_storage_upload_blob_from_string,
 )
 
 from prefect import flow
-from prefect.deployments import Deployment
 
 
 def test_cloud_storage_create_bucket(gcp_credentials):
     bucket = "expected"
     location = "US"
 
     @flow
@@ -183,20 +182,22 @@
     def test_put_directory(self, gcs_bucket, tmp_path, to_path, ignore):
         local_path = tmp_path / "a_directory"
         local_path.mkdir()
 
         (local_path / "abc.html").write_text("<div>abc</div>")
         (local_path / "cab.txt").write_text("cab")
         (local_path / "some_dir").mkdir()
+        (local_path / "some_dir" / "nested_abc.html").write_text("<div>abc</div>")
+        (local_path / "some_dir" / "nested_cab.txt").write_text("cab")
 
-        expected = 2
+        expected = 4
         if ignore:
             ignore_file = tmp_path / "ignore.txt"
             ignore_file.write_text("*.html")
-            expected -= 1
+            expected -= 2
         else:
             ignore_file = None
 
         actual = gcs_bucket.put_directory(
             local_path=local_path, to_path=to_path, ignore_file=ignore_file
         )
         assert actual == expected
@@ -545,20 +546,7 @@
         self, gcs_bucket_with_bucket_folder, pandas_dataframe
     ):
         with pytest.raises(KeyError):
             to_path = "to_path"
             gcs_bucket_with_bucket_folder.upload_from_dataframe(
                 df=pandas_dataframe, to_path=to_path, serialization_format="pickle"
             )
-
-    def test_basepath(self, gcs_bucket_with_bucket_folder, monkeypatch):
-        monkeypatch.setattr(
-            "prefect_gcp.GcpCredentials.get_cloud_storage_client", lambda x: x
-        )
-        assert gcs_bucket_with_bucket_folder.basepath == "base_folder/"
-
-        deployment = Deployment(
-            flow_name="test-flow-name",
-            name="test-deployment",
-            storage=gcs_bucket_with_bucket_folder,
-        )
-        assert deployment.location == ""
```

### Comparing `prefect_gcp-0.5.9/tests/test_credentials.py` & `prefect_gcp-0.6.0rc1/tests/test_credentials.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import json
 import os
 from pathlib import Path
 
 import pytest
-from google.cloud.aiplatform.gapic import JobServiceClient
+from google.cloud.aiplatform.gapic import JobServiceAsyncClient, JobServiceClient
 from prefect_gcp import GcpCredentials
-from prefect_gcp.credentials import ClientType
+from prefect_gcp.credentials import ClientType, _get_job_service_async_client_cached
 
 from prefect import flow, task
 from prefect.blocks.core import Block
+from prefect.types import SecretDict
 
 
 def _get_first_file_in_root():
     for path in os.listdir(os.path.expanduser("~")):
         if os.path.isfile(os.path.join(os.path.expanduser("~"), path)):
             return os.path.join("~", path)
 
@@ -153,25 +154,93 @@
         )
         client = credentials.get_job_service_client(client_options={})
         assert isinstance(client, JobServiceClient)
 
     test_flow()
 
 
+async def test_get_job_service_async_client(service_account_info, oauth2_credentials):
+    @flow
+    def test_flow():
+        project = "test_project"
+        credentials = GcpCredentials(
+            service_account_info=service_account_info,
+            project=project,
+        )
+        client = credentials.get_job_service_async_client(client_options={})
+        assert isinstance(client, JobServiceAsyncClient)
+
+    test_flow()
+
+
+async def test_get_job_service_async_client_cached(
+    service_account_info, oauth2_credentials
+):
+    """
+    Test to ensure that _get_job_service_async_client_cached function returns the same instance
+    for multiple calls with the same parameters and properly utilizes lru_cache.
+    """
+    _get_job_service_async_client_cached.cache_clear()
+
+    project = "test_project"
+    credentials = GcpCredentials(
+        service_account_info=service_account_info,
+        project=project,
+    )
+
+    assert (
+        _get_job_service_async_client_cached.cache_info().hits == 0
+    ), "Initial call count should be 0"
+
+    credentials.get_job_service_async_client(client_options={})
+    credentials.get_job_service_async_client(client_options={})
+    credentials.get_job_service_async_client(client_options={})
+
+    assert _get_job_service_async_client_cached.cache_info().misses == 1
+    assert _get_job_service_async_client_cached.cache_info().hits == 2
+
+
+async def test_get_job_service_async_client_cached_from_file(
+    service_account_info, oauth2_credentials
+):
+    """
+    Test to ensure that _get_job_service_async_client_cached function returns the same instance
+    for multiple calls with the same parameters and properly utilizes lru_cache.
+    """
+    _get_job_service_async_client_cached.cache_clear()
+
+    project = "test_project"
+    credentials = GcpCredentials(
+        service_account_file=SERVICE_ACCOUNT_FILES[0],
+        project=project,
+    )
+
+    assert (
+        _get_job_service_async_client_cached.cache_info().hits == 0
+    ), "Initial call count should be 0"
+
+    credentials.get_job_service_async_client(client_options={})
+    credentials.get_job_service_async_client(client_options={})
+    credentials.get_job_service_async_client(client_options={})
+
+    assert _get_job_service_async_client_cached.cache_info().misses == 1
+    assert _get_job_service_async_client_cached.cache_info().hits == 2
+
+
 class MockTargetConfigs(Block):
     credentials: GcpCredentials
 
     def get_configs(self):
         """
         Returns the dbt configs, likely used eventually for writing to profiles.yml.
         Returns:
             A configs JSON.
         """
-        configs = self.credentials.dict()
-        for key in Block().dict():
+        configs = self.credentials.model_dump()
+        for key in Block().model_dump():
             configs.pop(key, None)
         for key in configs.copy():
             if key.startswith("_"):
                 configs.pop(key)
             elif hasattr(configs[key], "get_secret_value"):
                 configs[key] = configs[key].get_secret_value()
         return configs
@@ -219,25 +288,14 @@
                 }
             }
         }
     }
     assert test_flow() == expected
 
 
-async def test_get_access_token_async(gcp_credentials):
-    print(gcp_credentials.get_credentials_from_service_account().token)
-    token = await gcp_credentials.get_access_token()
-    assert token == "my-token"
-
-
-def test_get_access_token_sync_compatible(gcp_credentials):
-    token = gcp_credentials.get_access_token()
-    assert token == "my-token"
-
-
 @pytest.mark.parametrize("input_type", [None, str])
 @pytest.mark.parametrize(
     "client_type",
     [
         ClientType.BIGQUERY,
         ClientType.CLOUD_STORAGE,
         ClientType.AIPLATFORM,
@@ -246,10 +304,12 @@
 )
 def test_get_client(gcp_credentials, input_type, client_type):
     if input_type is not None:
         client_type = input_type(client_type.value)
     assert gcp_credentials.get_client(client_type=client_type)
 
 
-def test_get_client_error(gcp_credentials):
+def test_get_client_error(service_account_info):
     with pytest.raises(ValueError, match="'cool' is not a valid ClientType"):
-        assert gcp_credentials.get_client(client_type="cool")
+        assert GcpCredentials(
+            service_account_info=SecretDict(secret_value=service_account_info)
+        ).get_client(client_type="cool")
```

### Comparing `prefect_gcp-0.5.9/tests/test_secret_manager.py` & `prefect_gcp-0.6.0rc1/tests/test_secret_manager.py`

 * *Files identical despite different names*

### Comparing `prefect_gcp-0.5.9/tests/test_vertex_worker.py` & `prefect_gcp-0.6.0rc1/tests/test_vertex_worker.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,13 @@
 import uuid
 from types import SimpleNamespace
 from unittest.mock import MagicMock
 
 import anyio
-from pydantic import VERSION as PYDANTIC_VERSION
-
-if PYDANTIC_VERSION.startswith("2."):
-    import pydantic.v1 as pydantic
-else:
-    import pydantic
-
+import pydantic
 import pytest
 from google.cloud.aiplatform_v1.types.job_service import CancelCustomJobRequest
 from google.cloud.aiplatform_v1.types.job_state import JobState
 from prefect_gcp.workers.vertex import (
     VertexAIWorker,
     VertexAIWorkerJobConfiguration,
     VertexAIWorkerResult,
@@ -65,24 +59,20 @@
         base_job_template["job_configuration"]["region"] = "us-central1"
 
         with pytest.raises(pydantic.ValidationError) as excinfo:
             await VertexAIWorkerJobConfiguration.from_template_and_values(
                 base_job_template, {"credentials": gcp_credentials}
             )
 
-        assert excinfo.value.errors() == [
-            {
-                "loc": ("job_spec",),
-                "msg": (
-                    "Job is missing required attributes at the following paths: "
-                    "/maximum_run_time_hours, /worker_pool_specs"
-                ),
-                "type": "value_error",
-            }
-        ]
+        assert len(errs := excinfo.value.errors()) == 1
+        loc, msg, type_ = [errs[0].get(k) for k in ("loc", "msg", "type")]
+        assert "job_spec" in str(loc)
+        assert type_ == "value_error"
+        assert "/maximum_run_time_hours" in msg
+        assert "/worker_pool_specs" in msg
 
     async def test_validate_incomplete_worker_pool_spec(self, gcp_credentials):
         base_job_template = VertexAIWorker.get_default_base_job_template()
         base_job_template["job_configuration"]["job_spec"] = {
             "maximum_run_time_hours": 1,
             "worker_pool_specs": [
                 {
@@ -97,26 +87,21 @@
         base_job_template["job_configuration"]["region"] = "us-central1"
 
         with pytest.raises(pydantic.ValidationError) as excinfo:
             await VertexAIWorkerJobConfiguration.from_template_and_values(
                 base_job_template, {"credentials": gcp_credentials}
             )
 
-        assert excinfo.value.errors() == [
-            {
-                "loc": ("job_spec",),
-                "msg": (
-                    "Job is missing required attributes at the following paths: "
-                    "/worker_pool_specs/0/container_spec/image_uri, "
-                    "/worker_pool_specs/0/disk_spec, "
-                    "/worker_pool_specs/0/machine_spec/machine_type"
-                ),
-                "type": "value_error",
-            }
-        ]
+        assert len(errs := excinfo.value.errors()) == 1
+        loc, msg, type_ = [errs[0].get(k) for k in ("loc", "msg", "type")]
+        assert "job_spec" in str(loc)
+        assert type_ == "value_error"
+        assert "/worker_pool_specs/0/container_spec/image_uri" in msg
+        assert "/worker_pool_specs/0/disk_spec" in msg
+        assert "/worker_pool_specs/0/machine_spec/machine_type" in msg
 
     def test_gcp_project(self, job_config: VertexAIWorkerJobConfiguration):
         assert job_config.project == "gcp_credentials_project"
 
     def test_job_name(self, flow_run, job_config: VertexAIWorkerJobConfiguration):
         job_config.prepare_for_flow_run(flow_run, None, None)
         assert job_config.job_name.startswith("my-custom-ai-job")
@@ -153,94 +138,97 @@
 
 class TestVertexAIWorker:
     async def test_successful_worker_run(self, flow_run, job_config):
         async with VertexAIWorker("test-pool") as worker:
             job_config.prepare_for_flow_run(flow_run, None, None)
             result = await worker.run(flow_run=flow_run, configuration=job_config)
             assert (
-                job_config.credentials.job_service_client.create_custom_job.call_count
+                job_config.credentials.job_service_async_client.create_custom_job.call_count
                 == 1
             )
             assert (
-                job_config.credentials.job_service_client.get_custom_job.call_count == 1
+                job_config.credentials.job_service_async_client.get_custom_job.call_count
+                == 1
             )
             assert result == VertexAIWorkerResult(
                 status_code=0, identifier="mock_display_name"
             )
 
     async def test_failed_worker_run(self, flow_run, job_config):
         job_config.prepare_for_flow_run(flow_run, None, None)
         error_msg = "something went kablooey"
         error_job_display_name = "catastrophization"
-        job_config.credentials.job_service_client.get_custom_job.return_value = (
+        job_config.credentials.job_service_async_client.get_custom_job.return_value = (
             MagicMock(
                 name="error_mock_name",
                 state=JobState.JOB_STATE_FAILED,
                 error=MagicMock(message=error_msg),
                 display_name=error_job_display_name,
             )
         )
         async with VertexAIWorker("test-pool") as worker:
             with pytest.raises(RuntimeError, match=error_msg):
                 await worker.run(flow_run=flow_run, configuration=job_config)
 
             assert (
-                job_config.credentials.job_service_client.create_custom_job.call_count
+                job_config.credentials.job_service_async_client.create_custom_job.call_count
                 == 1
             )
             assert (
-                job_config.credentials.job_service_client.get_custom_job.call_count == 1
+                job_config.credentials.job_service_async_client.get_custom_job.call_count
+                == 1
             )
 
     async def test_cancelled_worker_run(self, flow_run, job_config):
         job_config.prepare_for_flow_run(flow_run, None, None)
         job_display_name = "a-job-well-done"
-        job_config.credentials.job_service_client.get_custom_job.return_value = (
+        job_config.credentials.job_service_async_client.get_custom_job.return_value = (
             MagicMock(
                 name="cancelled_mock_name",
                 state=JobState.JOB_STATE_CANCELLED,
                 error=MagicMock(message=""),
                 display_name=job_display_name,
             )
         )
         async with VertexAIWorker("test-pool") as worker:
             result = await worker.run(flow_run=flow_run, configuration=job_config)
             assert (
-                job_config.credentials.job_service_client.create_custom_job.call_count
+                job_config.credentials.job_service_async_client.create_custom_job.call_count
                 == 1
             )
             assert (
-                job_config.credentials.job_service_client.get_custom_job.call_count == 1
+                job_config.credentials.job_service_async_client.get_custom_job.call_count
+                == 1
             )
             assert result == VertexAIWorkerResult(
                 status_code=1, identifier=job_display_name
             )
 
     async def test_kill_infrastructure(self, flow_run, job_config):
-        mock = job_config.credentials.job_service_client.create_custom_job
+        mock = job_config.credentials.job_service_async_client.create_custom_job
         # the CancelCustomJobRequest class seems to reject a MagicMock value
         # so here, we'll use a SimpleNamespace as the mocked return values
         mock.return_value = SimpleNamespace(
             name="foobar", state=JobState.JOB_STATE_PENDING
         )
 
         async with VertexAIWorker("test-pool") as worker:
             with anyio.fail_after(10):
                 async with anyio.create_task_group() as tg:
                     result = await tg.start(worker.run, flow_run, job_config)
                 await worker.kill_infrastructure(result, job_config)
 
-            mock = job_config.credentials.job_service_client.cancel_custom_job
+            mock = job_config.credentials.job_service_async_client.cancel_custom_job
             assert mock.call_count == 1
             mock.assert_called_with(request=CancelCustomJobRequest(name="foobar"))
 
     async def test_kill_infrastructure_no_grace_seconds(
         self, flow_run, job_config, caplog
     ):
-        mock = job_config.credentials.job_service_client.create_custom_job
+        mock = job_config.credentials.job_service_async_client.create_custom_job
         mock.return_value = SimpleNamespace(
             name="bazzbar", state=JobState.JOB_STATE_PENDING
         )
         async with VertexAIWorker("test-pool") as worker:
             input_grace_period = 32
 
             with anyio.fail_after(10):
@@ -256,14 +244,14 @@
                 ) in record.msg:
                     break
             else:
                 raise AssertionError("Expected message not found.")
 
     async def test_kill_infrastructure_not_found(self, job_config):
         async with VertexAIWorker("test-pool") as worker:
-            job_config.credentials.job_service_client.cancel_custom_job.side_effect = (
-                Exception("does not exist")
+            job_config.credentials.job_service_async_client.cancel_custom_job.side_effect = Exception(
+                "does not exist"
             )
             with pytest.raises(
                 InfrastructureNotFound, match="Cannot stop Vertex AI job"
             ):
                 await worker.kill_infrastructure("foobarbazz", job_config)
```

