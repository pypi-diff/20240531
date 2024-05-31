# Comparing `tmp/prefect_dbt-0.5.0.tar.gz` & `tmp/prefect_dbt-0.6.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefect_dbt-0.5.0.tar", last modified: Thu May 16 20:58:35 2024, max compression
+gzip compressed data, was "prefect_dbt-0.6.0rc1.tar", last modified: Fri May 31 21:10:15 2024, max compression
```

## Comparing `prefect_dbt-0.5.0.tar` & `prefect_dbt-0.6.0rc1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:35.844794 prefect_dbt-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-16 20:58:23.000000 prefect_dbt-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-16 20:58:23.000000 prefect_dbt-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12678 2024-05-16 20:58:35.840794 prefect_dbt-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9853 2024-05-16 20:58:23.000000 prefect_dbt-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:35.832794 prefect_dbt-0.5.0/prefect_dbt/
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-16 20:58:23.000000 prefect_dbt-0.5.0/prefect_dbt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-16 20:58:35.000000 prefect_dbt-0.5.0/prefect_dbt/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:35.832794 prefect_dbt-0.5.0/prefect_dbt/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-16 20:58:23.000000 prefect_dbt-0.5.0/prefect_dbt/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35737 2024-05-16 20:58:23.000000 prefect_dbt-0.5.0/prefect_dbt/cli/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:35.832794 prefect_dbt-0.5.0/prefect_dbt/cli/configs/
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-16 20:58:23.000000 prefect_dbt-0.5.0/prefect_dbt/cli/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10508 2024-05-16 20:58:23.000000 prefect_dbt-0.5.0/prefect_dbt/cli/configs/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5768 2024-05-16 20:58:23.000000 prefect_dbt-0.5.0/prefect_dbt/cli/configs/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-05-16 20:58:23.000000 prefect_dbt-0.5.0/prefect_dbt/cli/configs/postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-05-16 20:58:23.000000 prefect_dbt-0.5.0/prefect_dbt/cli/configs/snowflake.py
--rw-r--r--   0 runner    (1001) docker     (127)     5568 2024-05-16 20:58:23.000000 prefect_dbt-0.5.0/prefect_dbt/cli/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:35.836794 prefect_dbt-0.5.0/prefect_dbt/cloud/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-16 20:58:23.000000 prefect_dbt-0.5.0/prefect_dbt/cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8538 2024-05-16 20:58:23.000000 prefect_dbt-0.5.0/prefect_dbt/cloud/clients.py
--rw-r--r--   0 runner    (1001) docker     (127)     6519 2024-05-16 20:58:23.000000 prefect_dbt-0.5.0/prefect_dbt/cloud/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-16 20:58:23.000000 prefect_dbt-0.5.0/prefect_dbt/cloud/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    43316 2024-05-16 20:58:23.000000 prefect_dbt-0.5.0/prefect_dbt/cloud/jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-16 20:58:23.000000 prefect_dbt-0.5.0/prefect_dbt/cloud/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     9943 2024-05-16 20:58:23.000000 prefect_dbt-0.5.0/prefect_dbt/cloud/runs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5098 2024-05-16 20:58:23.000000 prefect_dbt-0.5.0/prefect_dbt/cloud/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:35.836794 prefect_dbt-0.5.0/prefect_dbt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12678 2024-05-16 20:58:35.000000 prefect_dbt-0.5.0/prefect_dbt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-16 20:58:35.000000 prefect_dbt-0.5.0/prefect_dbt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 20:58:35.000000 prefect_dbt-0.5.0/prefect_dbt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-16 20:58:35.000000 prefect_dbt-0.5.0/prefect_dbt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-16 20:58:35.000000 prefect_dbt-0.5.0/prefect_dbt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-16 20:58:35.000000 prefect_dbt-0.5.0/prefect_dbt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-05-16 20:58:23.000000 prefect_dbt-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 20:58:35.844794 prefect_dbt-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:35.836794 prefect_dbt-0.5.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:35.836794 prefect_dbt-0.5.0/tests/cli/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:35.836794 prefect_dbt-0.5.0/tests/cli/configs/
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-16 20:58:23.000000 prefect_dbt-0.5.0/tests/cli/configs/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5314 2024-05-16 20:58:23.000000 prefect_dbt-0.5.0/tests/cli/configs/test_bigquery.py
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-05-16 20:58:23.000000 prefect_dbt-0.5.0/tests/cli/configs/test_postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-05-16 20:58:23.000000 prefect_dbt-0.5.0/tests/cli/configs/test_snowflake.py
--rw-r--r--   0 runner    (1001) docker     (127)    17727 2024-05-16 20:58:23.000000 prefect_dbt-0.5.0/tests/cli/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-05-16 20:58:23.000000 prefect_dbt-0.5.0/tests/cli/test_credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:35.836794 prefect_dbt-0.5.0/tests/cloud/
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-16 20:58:23.000000 prefect_dbt-0.5.0/tests/cloud/test_clients.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-16 20:58:23.000000 prefect_dbt-0.5.0/tests/cloud/test_cloud_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    31500 2024-05-16 20:58:23.000000 prefect_dbt-0.5.0/tests/cloud/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6602 2024-05-16 20:58:23.000000 prefect_dbt-0.5.0/tests/cloud/test_runs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-05-16 20:58:23.000000 prefect_dbt-0.5.0/tests/cloud/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5840 2024-05-16 20:58:23.000000 prefect_dbt-0.5.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-16 20:58:23.000000 prefect_dbt-0.5.0/tests/test_block_standards.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-16 20:58:23.000000 prefect_dbt-0.5.0/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:10:15.235337 prefect_dbt-0.6.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-31 21:10:04.000000 prefect_dbt-0.6.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-31 21:10:04.000000 prefect_dbt-0.6.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12596 2024-05-31 21:10:15.235337 prefect_dbt-0.6.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9853 2024-05-31 21:10:04.000000 prefect_dbt-0.6.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:10:15.227337 prefect_dbt-0.6.0rc1/prefect_dbt/
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-31 21:10:04.000000 prefect_dbt-0.6.0rc1/prefect_dbt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-31 21:10:14.000000 prefect_dbt-0.6.0rc1/prefect_dbt/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:10:15.227337 prefect_dbt-0.6.0rc1/prefect_dbt/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-31 21:10:04.000000 prefect_dbt-0.6.0rc1/prefect_dbt/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35180 2024-05-31 21:10:04.000000 prefect_dbt-0.6.0rc1/prefect_dbt/cli/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:10:15.227337 prefect_dbt-0.6.0rc1/prefect_dbt/cli/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-31 21:10:04.000000 prefect_dbt-0.6.0rc1/prefect_dbt/cli/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10263 2024-05-31 21:10:04.000000 prefect_dbt-0.6.0rc1/prefect_dbt/cli/configs/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5640 2024-05-31 21:10:04.000000 prefect_dbt-0.6.0rc1/prefect_dbt/cli/configs/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-05-31 21:10:04.000000 prefect_dbt-0.6.0rc1/prefect_dbt/cli/configs/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-05-31 21:10:04.000000 prefect_dbt-0.6.0rc1/prefect_dbt/cli/configs/snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5435 2024-05-31 21:10:04.000000 prefect_dbt-0.6.0rc1/prefect_dbt/cli/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:10:15.231337 prefect_dbt-0.6.0rc1/prefect_dbt/cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-31 21:10:04.000000 prefect_dbt-0.6.0rc1/prefect_dbt/cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8545 2024-05-31 21:10:04.000000 prefect_dbt-0.6.0rc1/prefect_dbt/cloud/clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6375 2024-05-31 21:10:04.000000 prefect_dbt-0.6.0rc1/prefect_dbt/cloud/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-31 21:10:04.000000 prefect_dbt-0.6.0rc1/prefect_dbt/cloud/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43066 2024-05-31 21:10:04.000000 prefect_dbt-0.6.0rc1/prefect_dbt/cloud/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-05-31 21:10:04.000000 prefect_dbt-0.6.0rc1/prefect_dbt/cloud/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9922 2024-05-31 21:10:04.000000 prefect_dbt-0.6.0rc1/prefect_dbt/cloud/runs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-05-31 21:10:04.000000 prefect_dbt-0.6.0rc1/prefect_dbt/cloud/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:10:15.231337 prefect_dbt-0.6.0rc1/prefect_dbt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12596 2024-05-31 21:10:14.000000 prefect_dbt-0.6.0rc1/prefect_dbt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-31 21:10:15.000000 prefect_dbt-0.6.0rc1/prefect_dbt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 21:10:14.000000 prefect_dbt-0.6.0rc1/prefect_dbt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-31 21:10:14.000000 prefect_dbt-0.6.0rc1/prefect_dbt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-31 21:10:14.000000 prefect_dbt-0.6.0rc1/prefect_dbt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-31 21:10:14.000000 prefect_dbt-0.6.0rc1/prefect_dbt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-05-31 21:10:04.000000 prefect_dbt-0.6.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 21:10:15.235337 prefect_dbt-0.6.0rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:10:15.231337 prefect_dbt-0.6.0rc1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:10:15.231337 prefect_dbt-0.6.0rc1/tests/cli/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:10:15.231337 prefect_dbt-0.6.0rc1/tests/cli/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-31 21:10:04.000000 prefect_dbt-0.6.0rc1/tests/cli/configs/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5314 2024-05-31 21:10:04.000000 prefect_dbt-0.6.0rc1/tests/cli/configs/test_bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-31 21:10:04.000000 prefect_dbt-0.6.0rc1/tests/cli/configs/test_postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3341 2024-05-31 21:10:04.000000 prefect_dbt-0.6.0rc1/tests/cli/configs/test_snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17855 2024-05-31 21:10:04.000000 prefect_dbt-0.6.0rc1/tests/cli/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-05-31 21:10:04.000000 prefect_dbt-0.6.0rc1/tests/cli/test_credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:10:15.231337 prefect_dbt-0.6.0rc1/tests/cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-31 21:10:04.000000 prefect_dbt-0.6.0rc1/tests/cloud/test_clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-31 21:10:04.000000 prefect_dbt-0.6.0rc1/tests/cloud/test_cloud_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31500 2024-05-31 21:10:04.000000 prefect_dbt-0.6.0rc1/tests/cloud/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6602 2024-05-31 21:10:04.000000 prefect_dbt-0.6.0rc1/tests/cloud/test_runs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-05-31 21:10:04.000000 prefect_dbt-0.6.0rc1/tests/cloud/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5840 2024-05-31 21:10:04.000000 prefect_dbt-0.6.0rc1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-31 21:10:04.000000 prefect_dbt-0.6.0rc1/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-31 21:10:04.000000 prefect_dbt-0.6.0rc1/tests/test_version.py
```

### Comparing `prefect_dbt-0.5.0/LICENSE` & `prefect_dbt-0.6.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `prefect_dbt-0.5.0/PKG-INFO` & `prefect_dbt-0.6.0rc1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,66 +1,64 @@
 Metadata-Version: 2.1
 Name: prefect-dbt
-Version: 0.5.0
+Version: 0.6.0rc1
 Summary: Prefect integrations for working with dbt
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-dbt
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
 License-File: LICENSE
-Requires-Dist: prefect<3.0.0,>=2.16.6
+Requires-Dist: prefect>=3.0.0rc1
 Requires-Dist: dbt-core>=1.7.0
-Requires-Dist: prefect_shell>=0.1.4
+Requires-Dist: prefect_shell>=0.3.0rc1
 Requires-Dist: sgqlc>=16.0.0
 Provides-Extra: snowflake
-Requires-Dist: prefect-snowflake>=0.2.4; extra == "snowflake"
+Requires-Dist: prefect-snowflake>=0.28.0rc1; extra == "snowflake"
 Requires-Dist: dbt-snowflake; extra == "snowflake"
 Provides-Extra: bigquery
-Requires-Dist: prefect-gcp[bigquery]>=0.1.8; extra == "bigquery"
+Requires-Dist: prefect-gcp[bigquery]>=0.6.0rc1; extra == "bigquery"
 Requires-Dist: dbt-bigquery; extra == "bigquery"
 Provides-Extra: postgres
-Requires-Dist: prefect-sqlalchemy>=0.2.1; extra == "postgres"
+Requires-Dist: prefect-sqlalchemy>=0.5.0rc1; extra == "postgres"
 Requires-Dist: dbt-postgres; extra == "postgres"
 Provides-Extra: all-extras
 Requires-Dist: dbt-bigquery; extra == "all-extras"
 Requires-Dist: dbt-postgres; extra == "all-extras"
 Requires-Dist: dbt-snowflake; extra == "all-extras"
-Requires-Dist: prefect-gcp[bigquery]>=0.1.8; extra == "all-extras"
-Requires-Dist: prefect-snowflake>=0.2.4; extra == "all-extras"
-Requires-Dist: prefect-sqlalchemy>=0.2.1; extra == "all-extras"
+Requires-Dist: prefect-gcp[bigquery]>=0.6.0rc1; extra == "all-extras"
+Requires-Dist: prefect-snowflake>=0.28.0rc1; extra == "all-extras"
+Requires-Dist: prefect-sqlalchemy>=0.5.0rc1; extra == "all-extras"
 Provides-Extra: dev
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: dbt-bigquery; extra == "dev"
 Requires-Dist: dbt-postgres; extra == "dev"
 Requires-Dist: dbt-snowflake; extra == "dev"
 Requires-Dist: interrogate; extra == "dev"
 Requires-Dist: mkdocs-gen-files; extra == "dev"
 Requires-Dist: mkdocs-material; extra == "dev"
 Requires-Dist: mkdocs; extra == "dev"
 Requires-Dist: mkdocstrings[python]; extra == "dev"
-Requires-Dist: mock; python_version < "3.8" and extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pillow; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
-Requires-Dist: prefect-gcp[bigquery]>=0.1.8; extra == "dev"
-Requires-Dist: prefect-snowflake>=0.2.4; extra == "dev"
-Requires-Dist: prefect-sqlalchemy>=0.2.1; extra == "dev"
+Requires-Dist: prefect-gcp[bigquery]>=0.6.0rc1; extra == "dev"
+Requires-Dist: prefect-snowflake>=0.28.0rc1; extra == "dev"
+Requires-Dist: prefect-sqlalchemy>=0.5.0rc1; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: pytest-xdist; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: respx; extra == "dev"
 
 # prefect-dbt
 
@@ -206,15 +204,15 @@
 
     ```bash
     pip install dbt-databricks
     ```
 
     Check out the [desired profile setup page](https://docs.getdbt.com/reference/profiles.yml) on the sidebar for others.
 
-Requires an installation of Python 3.8+.
+Requires an installation of Python 3.9+.
 
 We recommend using a Python virtual environment manager such as pipenv, conda or virtualenv.
 
 These tasks are designed to work with Prefect 2. For more information about how to use Prefect, please refer to the [Prefect documentation](https://docs.prefect.io/).
 
 ### Saving credentials to block
```

### Comparing `prefect_dbt-0.5.0/README.md` & `prefect_dbt-0.6.0rc1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,15 @@
 
     ```bash
     pip install dbt-databricks
     ```
 
     Check out the [desired profile setup page](https://docs.getdbt.com/reference/profiles.yml) on the sidebar for others.
 
-Requires an installation of Python 3.8+.
+Requires an installation of Python 3.9+.
 
 We recommend using a Python virtual environment manager such as pipenv, conda or virtualenv.
 
 These tasks are designed to work with Prefect 2. For more information about how to use Prefect, please refer to the [Prefect documentation](https://docs.prefect.io/).
 
 ### Saving credentials to block
```

### Comparing `prefect_dbt-0.5.0/prefect_dbt/__init__.py` & `prefect_dbt-0.6.0rc1/prefect_dbt/__init__.py`

 * *Files identical despite different names*

### Comparing `prefect_dbt-0.5.0/prefect_dbt/cli/__init__.py` & `prefect_dbt-0.6.0rc1/prefect_dbt/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `prefect_dbt-0.5.0/prefect_dbt/cli/commands.py` & `prefect_dbt-0.6.0rc1/prefect_dbt/cli/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,30 +4,26 @@
 from pathlib import Path, PosixPath
 from typing import Any, Dict, List, Optional, Union
 
 import yaml
 from dbt.cli.main import dbtRunner, dbtRunnerResult
 from dbt.contracts.results import NodeStatus, RunExecutionResult
 from prefect_shell.commands import ShellOperation
-from pydantic import VERSION as PYDANTIC_VERSION
+from pydantic import Field
 
 from prefect import get_run_logger, task
 from prefect.artifacts import create_markdown_artifact
 from prefect.states import Failed
+from prefect.utilities.asyncutils import sync_compatible
 from prefect.utilities.filesystem import relative_path_to_current_platform
-
-if PYDANTIC_VERSION.startswith("2."):
-    from pydantic.v1 import Field, validator
-else:
-    from pydantic import Field, validator
-
 from prefect_dbt.cli.credentials import DbtCliProfile
 
 
 @task
+@sync_compatible
 async def trigger_dbt_cli_command(
     command: str,
     profiles_dir: Optional[Union[Path, str]] = None,
     project_dir: Optional[Union[Path, str]] = None,
     overwrite_profiles: bool = False,
     dbt_cli_profile: Optional[DbtCliProfile] = None,
     create_summary_artifact: bool = False,
@@ -198,15 +194,15 @@
                      due to create_artifact=False or the dbt command did not \
                      return any RunExecutionResults. \
                      See https://docs.getdbt.com/reference/programmatic-invocations \
                      for more details on dbtRunnerResult."
         )
     if isinstance(result.result, RunExecutionResult) and not result.success:
         return Failed(
-            message=f"dbt task result unsuccessful with exception: {result.exception}"
+            message=f"dbt task result success: {result.success} with exception: {result.exception}"
         )
     return result
 
 
 class DbtCoreOperation(ShellOperation):
     """
     A block representing a dbt operation, containing multiple dbt and shell commands.
@@ -312,27 +308,14 @@
         description=(
             "Profiles class containing the profile written to profiles.yml. "
             "Note! This is optional and will raise an error if profiles.yml already "
             "exists under profile_dir and overwrite_profiles is set to False."
         ),
     )
 
-    @validator("commands", always=True)
-    def _has_a_dbt_command(cls, commands):
-        """
-        Check that the commands contain a dbt command.
-        """
-        if not any("dbt " in command for command in commands):
-            raise ValueError(
-                "None of the commands are a valid dbt sub-command; see dbt --help, "
-                "or use prefect_shell.ShellOperation for non-dbt related "
-                "commands instead"
-            )
-        return commands
-
     def _find_valid_profiles_dir(self) -> PosixPath:
         """
         Ensure that there is a profiles.yml available for use.
         """
         profiles_dir = self.profiles_dir
         if profiles_dir is None:
             if self.env.get("DBT_PROFILES_DIR") is not None:
```

### Comparing `prefect_dbt-0.5.0/prefect_dbt/cli/configs/base.py` & `prefect_dbt-0.6.0rc1/prefect_dbt/cli/configs/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,17 @@
 """Module containing models for base configs"""
 
 import abc
 from pathlib import Path
 from typing import Any, Dict, Optional
 
-from pydantic import VERSION as PYDANTIC_VERSION
+from pydantic import BaseModel, Field
 
 from prefect.blocks.core import Block
 
-if PYDANTIC_VERSION.startswith("2."):
-    from pydantic.v1 import BaseModel, Field, SecretField
-else:
-    from pydantic import BaseModel, Field, SecretField
-
 
 class DbtConfigs(Block, abc.ABC):
     """
     Abstract class for other dbt Configs.
 
     Attributes:
         extras: Extra target configs' keywords, not yet exposed
@@ -52,45 +47,43 @@
         """
         # if allow_field_overrides is True keys from TargetConfigs take precedence
         override_configs_json = {}
 
         for field_name, field in fields.items():
             if model is not None:
                 # get actual value from model
-                try:
-                    field_value = getattr(model, field_name)
-                except AttributeError:
-                    field_value = getattr(model, field.alias)
+                field_value = getattr(model, field_name, None)
                 # override the name with alias so dbt parser can recognize the keyword;
                 # e.g. schema_ -> schema, returns the original name if no alias is set
-                field_name = field.alias
+                if field.alias:
+                    field_name = field.alias
             else:
                 field_value = field
 
             if field_value is None or field_name == "allow_field_overrides":
                 # do not add to configs json if no value or default is set
                 continue
 
             if isinstance(field_value, BaseModel):
                 configs_json = self._populate_configs_json(
-                    configs_json, field_value.__fields__, model=field_value
+                    configs_json, field_value.model_fields, model=field_value
                 )
             elif field_name == "extras":
                 configs_json = self._populate_configs_json(
                     configs_json,
                     field_value,
                 )
                 override_configs_json.update(configs_json)
             else:
                 if field_name in configs_json.keys() and not self.allow_field_overrides:
                     raise ValueError(
                         f"The keyword, {field_name}, has already been provided in "
                         f"TargetConfigs; remove duplicated keywords to continue"
                     )
-                if isinstance(field_value, SecretField):
+                if hasattr(field_value, "get_secret_value"):
                     field_value = field_value.get_secret_value()
                 elif isinstance(field_value, Path):
                     field_value = str(field_value)
                 configs_json[field_name] = field_value
 
                 if self.allow_field_overrides and model is self or model is None:
                     override_configs_json[field_name] = field_value
@@ -101,15 +94,15 @@
     def get_configs(self) -> Dict[str, Any]:
         """
         Returns the dbt configs, likely used eventually for writing to profiles.yml.
 
         Returns:
             A configs JSON.
         """
-        return self._populate_configs_json({}, self.__fields__, model=self)
+        return self._populate_configs_json({}, self.model_fields, model=self)
 
 
 class BaseTargetConfigs(DbtConfigs, abc.ABC):
     type: str = Field(default=..., description="The name of the database warehouse.")
     schema_: str = Field(
         alias="schema",
         description=(
```

### Comparing `prefect_dbt-0.5.0/prefect_dbt/cli/configs/bigquery.py` & `prefect_dbt-0.6.0rc1/prefect_dbt/cli/configs/bigquery.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 """Module containing models for BigQuery configs"""
+
 from typing import Any, Dict, Optional
 
 from google.auth.transport.requests import Request
 
 try:
     from typing import Literal
 except ImportError:
     from typing_extensions import Literal
 
-from pydantic import VERSION as PYDANTIC_VERSION
 
-if PYDANTIC_VERSION.startswith("2."):
-    from pydantic.v1 import Field
-else:
-    from pydantic import Field
+from pydantic import Field
 
 from prefect_dbt.cli.configs.base import BaseTargetConfigs, MissingExtrasRequireError
 
 try:
     from prefect_gcp.credentials import GcpCredentials
 except ModuleNotFoundError as e:
     raise MissingExtrasRequireError("BigQuery") from e
@@ -79,15 +76,15 @@
             A configs JSON.
         """
         # since GcpCredentials will always define a project
         self_copy = self.copy()
         if self_copy.project is not None:
             self_copy.credentials.project = None
         all_configs_json = self._populate_configs_json(
-            {}, self_copy.__fields__, model=self_copy
+            {}, self_copy.model_fields, model=self_copy
         )
 
         # decouple prefect-gcp from prefect-dbt
         # by mapping all the keys dbt gcp accepts
         # https://docs.getdbt.com/reference/warehouse-setups/bigquery-setup
         rename_keys = {
             # dbt
```

### Comparing `prefect_dbt-0.5.0/prefect_dbt/cli/configs/postgres.py` & `prefect_dbt-0.6.0rc1/prefect_dbt/cli/configs/postgres.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,18 @@
 """Module containing models for Postgres configs"""
-import warnings
-from typing import Any, Dict, Union
 
-from pydantic import VERSION as PYDANTIC_VERSION
-
-if PYDANTIC_VERSION.startswith("2."):
-    from pydantic.v1 import Field
-else:
-    from pydantic import Field
+from typing import Any, Dict
 
+from pydantic import Field
 from typing_extensions import Literal
 
 from prefect_dbt.cli.configs.base import BaseTargetConfigs, MissingExtrasRequireError
 
 try:
-    from prefect_sqlalchemy import DatabaseCredentials, SqlAlchemyConnector
+    from prefect_sqlalchemy import SqlAlchemyConnector
 except ModuleNotFoundError as e:
     raise MissingExtrasRequireError("Postgres") from e
 
 
 class PostgresTargetConfigs(BaseTargetConfigs):
     """
     Target configs contain credentials and
@@ -28,48 +22,26 @@
     page.
 
     Attributes:
         credentials: The credentials to use to authenticate; if there are
             duplicate keys between credentials and TargetConfigs,
             e.g. schema, an error will be raised.
 
-    Examples:
-        Load stored PostgresTargetConfigs:
-        ```python
-        from prefect_dbt.cli.configs import PostgresTargetConfigs
-
-        postgres_target_configs = PostgresTargetConfigs.load("BLOCK_NAME")
-        ```
-
-        Instantiate PostgresTargetConfigs with DatabaseCredentials.
-        ```python
-        from prefect_dbt.cli.configs import PostgresTargetConfigs
-        from prefect_sqlalchemy import DatabaseCredentials, SyncDriver
-
-        credentials = DatabaseCredentials(
-            driver=SyncDriver.POSTGRESQL_PSYCOPG2,
-            username="prefect",
-            password="prefect_password",
-            database="postgres",
-            host="host",
-            port=8080
-        )
-        target_configs = PostgresTargetConfigs(credentials=credentials, schema="schema")
         ```
     """
 
     _block_type_name = "dbt CLI Postgres Target Configs"
     _logo_url = "https://images.ctfassets.net/gm98wzqotmnx/5zE9lxfzBHjw3tnEup4wWL/9a001902ed43a84c6c96d23b24622e19/dbt-bit_tm.png?h=250"  # noqa
     _description = "dbt CLI target configs containing credentials and settings specific to Postgres."  # noqa
     _documentation_url = "https://prefecthq.github.io/prefect-dbt/cli/configs/postgres/#prefect_dbt.cli.configs.postgres.PostgresTargetConfigs"  # noqa
 
     type: Literal["postgres"] = Field(
         default="postgres", description="The type of the target."
     )
-    credentials: Union[SqlAlchemyConnector, DatabaseCredentials] = Field(
+    credentials: SqlAlchemyConnector = Field(
         default=...,
         description=(
             "The credentials to use to authenticate; if there are duplicate keys "
             "between credentials and TargetConfigs, e.g. schema, "
             "an error will be raised."
         ),
     )  # noqa
@@ -77,20 +49,14 @@
     def get_configs(self) -> Dict[str, Any]:
         """
         Returns the dbt configs specific to Postgres profile.
 
         Returns:
             A configs JSON.
         """
-        if isinstance(self.credentials, DatabaseCredentials):
-            warnings.warn(
-                "Using DatabaseCredentials is deprecated and will be removed "
-                "on May 7th, 2023, use SqlAlchemyConnector instead.",
-                DeprecationWarning,
-            )
         all_configs_json = super().get_configs()
 
         rename_keys = {
             # dbt
             "type": "type",
             "schema": "schema",
             "threads": "threads",
```

### Comparing `prefect_dbt-0.5.0/prefect_dbt/cli/configs/snowflake.py` & `prefect_dbt-0.6.0rc1/prefect_dbt/cli/configs/snowflake.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 """Module containing models for Snowflake configs"""
+
 from typing import Any, Dict, Optional
 
 try:
     from typing import Literal
 except ImportError:
     from typing_extensions import Literal
 
-from pydantic import VERSION as PYDANTIC_VERSION
 
-if PYDANTIC_VERSION.startswith("2."):
-    from pydantic.v1 import Field
-else:
-    from pydantic import Field
+from pydantic import Field
 
 from prefect_dbt.cli.configs.base import BaseTargetConfigs, MissingExtrasRequireError
 
 try:
     from prefect_snowflake.database import SnowflakeConnector
 except ModuleNotFoundError as e:
     raise MissingExtrasRequireError("Snowflake") from e
```

### Comparing `prefect_dbt-0.5.0/prefect_dbt/cli/credentials.py` & `prefect_dbt-0.6.0rc1/prefect_dbt/cli/credentials.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,14 @@
 """Module containing credentials for interacting with dbt CLI"""
 
 from typing import Any, Dict, Optional, Union
 
-from pydantic import VERSION as PYDANTIC_VERSION
+from pydantic import Field
 
 from prefect.blocks.core import Block
-
-if PYDANTIC_VERSION.startswith("2."):
-    from pydantic.v1 import Field
-else:
-    from pydantic import Field
-
 from prefect_dbt.cli.configs import GlobalConfigs, TargetConfigs
 
 try:
     from prefect_dbt.cli.configs.bigquery import BigQueryTargetConfigs
 except ImportError:
     BigQueryTargetConfigs = None
```

### Comparing `prefect_dbt-0.5.0/prefect_dbt/cloud/clients.py` & `prefect_dbt-0.6.0rc1/prefect_dbt/cloud/clients.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module containing clients for interacting with the dbt Cloud API"""
+
 from typing import Any, Dict, List, Optional
 
 from httpx import AsyncClient, Response
 from sgqlc.endpoint.http import HTTPEndpoint
 from typing_extensions import Literal
 
 import prefect
@@ -96,15 +97,15 @@
         """  # noqa
         if options is None:
             options = TriggerJobRunOptions()
 
         return await self.call_endpoint(
             path=f"/jobs/{job_id}/run/",
             http_method="POST",
-            json=options.dict(exclude_none=True),
+            json=options.model_dump(exclude_none=True),
         )
 
     async def get_run(
         self,
         run_id: int,
         include_related: Optional[
             List[Literal["trigger", "job", "debug_logs", "run_steps"]]
```

### Comparing `prefect_dbt-0.5.0/prefect_dbt/cloud/credentials.py` & `prefect_dbt-0.6.0rc1/prefect_dbt/cloud/credentials.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,15 @@
 """Module containing credentials for interacting with dbt Cloud"""
-from typing import Union
-
-from pydantic import VERSION as PYDANTIC_VERSION
-
-from prefect.blocks.abstract import CredentialsBlock
 
-if PYDANTIC_VERSION.startswith("2."):
-    from pydantic.v1 import Field, SecretStr
-else:
-    from pydantic import Field, SecretStr
+from typing import Union
 
+from pydantic import Field, SecretStr
 from typing_extensions import Literal
 
+from prefect.blocks.abstract import CredentialsBlock
 from prefect_dbt.cloud.clients import (
     DbtCloudAdministrativeClient,
     DbtCloudMetadataClient,
 )
 
 
 class DbtCloudCredentials(CredentialsBlock):
```

### Comparing `prefect_dbt-0.5.0/prefect_dbt/cloud/exceptions.py` & `prefect_dbt-0.6.0rc1/prefect_dbt/cloud/exceptions.py`

 * *Files identical despite different names*

### Comparing `prefect_dbt-0.5.0/prefect_dbt/cloud/jobs.py` & `prefect_dbt-0.6.0rc1/prefect_dbt/cloud/jobs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 """Module containing tasks and flows for interacting with dbt Cloud jobs"""
+
 import asyncio
 import shlex
 import time
 from json import JSONDecodeError
 from typing import Any, Awaitable, Callable, Dict, List, Optional, Union
 
 from httpx import HTTPStatusError
-from pydantic import VERSION as PYDANTIC_VERSION
+from pydantic import Field
+from typing_extensions import Literal
 
 from prefect import flow, get_run_logger, task
 from prefect.blocks.abstract import JobBlock, JobRun
 from prefect.context import FlowRunContext
 from prefect.utilities.asyncutils import sync_compatible
-
-if PYDANTIC_VERSION.startswith("2."):
-    from pydantic.v1 import Field
-else:
-    from pydantic import Field
-
-from typing_extensions import Literal
-
 from prefect_dbt.cloud.credentials import DbtCloudCredentials
 from prefect_dbt.cloud.exceptions import (
     DbtCloudGetJobFailed,
     DbtCloudGetRunArtifactFailed,
     DbtCloudGetRunFailed,
     DbtCloudJobRunCancelled,
     DbtCloudJobRunFailed,
@@ -230,15 +224,15 @@
                 )
 
             triggered_run_data = trigger_dbt_cloud_job_run(
                 dbt_cloud_credentials=dbt_cloud_credentials,
                 job_id=job_id,
                 options=trigger_job_run_options,
             )
-            run_id = get_run_id.submit(triggered_run_data)
+            run_id = get_run_id(triggered_run_data)
             return run_id
 
         trigger_run_and_get_id()
         ```
     """
     id = obj.get("id")
     if id is None:
@@ -349,37 +343,37 @@
                 ),
             )
         )
         ```
     """  # noqa
     logger = get_run_logger()
 
-    triggered_run_data_future = await trigger_dbt_cloud_job_run.submit(
+    triggered_run_data_future = await trigger_dbt_cloud_job_run(
         dbt_cloud_credentials=dbt_cloud_credentials,
         job_id=job_id,
         options=trigger_job_run_options,
     )
-    run_id = (await triggered_run_data_future.result()).get("id")
+    run_id = (triggered_run_data_future).get("id")
     if run_id is None:
         raise RuntimeError("Unable to determine run ID for triggered job.")
 
     final_run_status, run_data = await wait_for_dbt_cloud_job_run(
         run_id=run_id,
         dbt_cloud_credentials=dbt_cloud_credentials,
         max_wait_seconds=max_wait_seconds,
         poll_frequency_seconds=poll_frequency_seconds,
     )
 
     if final_run_status == DbtCloudJobRunStatus.SUCCESS:
         try:
-            list_run_artifacts_future = await list_dbt_cloud_run_artifacts.submit(
+            list_run_artifacts_future = await list_dbt_cloud_run_artifacts(
                 dbt_cloud_credentials=dbt_cloud_credentials,
                 run_id=run_id,
             )
-            run_data["artifact_paths"] = await list_run_artifacts_future.result()
+            run_data["artifact_paths"] = list_run_artifacts_future
         except DbtCloudListRunArtifactsFailed as ex:
             logger.warning(
                 "Unable to retrieve artifacts for job run with ID %s. Reason: %s",
                 run_id,
                 ex,
             )
         logger.info(
@@ -474,21 +468,21 @@
             steps_override.append(command)
         else:
             # errors and failures are when we need to inspect to figure
             # out the point of failure
             try:
                 run_artifact_future = await get_dbt_cloud_run_artifact.with_options(
                     retries=0, retry_delay_seconds=0
-                ).submit(
+                )(
                     dbt_cloud_credentials=dbt_cloud_credentials,
                     run_id=run_id,
                     path="run_results.json",
                     step=run_step["index"],
                 )
-                run_artifact = await run_artifact_future.result()
+                run_artifact = run_artifact_future
             except JSONDecodeError:
                 # get the run results scoped to the step which had an error
                 # an error here indicates that either:
                 # 1) the fail-fast flag was set, in which case
                 #    the run_results.json file was never created; or
                 # 2) there was a problem on dbt Cloud's side saving
                 #    this artifact
@@ -596,27 +590,27 @@
     """  # noqa
     if trigger_job_run_options and trigger_job_run_options.steps_override is not None:
         raise ValueError(
             "Do not set `steps_override` in `trigger_job_run_options` "
             "because this flow will automatically set it"
         )
 
-    run_info_future = await get_dbt_cloud_run_info.submit(
+    run_info_future = await get_dbt_cloud_run_info(
         dbt_cloud_credentials=dbt_cloud_credentials,
         run_id=run_id,
         include_related=["run_steps"],
     )
-    run_info = await run_info_future.result()
+    run_info = run_info_future
 
     job_id = run_info["job_id"]
-    job_info_future = await get_dbt_cloud_job_info.submit(
+    job_info_future = await get_dbt_cloud_job_info(
         dbt_cloud_credentials=dbt_cloud_credentials,
         job_id=job_id,
     )
-    job_info = await job_info_future.result()
+    job_info = job_info_future
 
     trigger_job_run_options_override = await _build_trigger_job_run_options(
         dbt_cloud_credentials=dbt_cloud_credentials,
         trigger_job_run_options=trigger_job_run_options,
         run_id=run_id,
         run_info=run_info,
         job_info=job_info,
```

### Comparing `prefect_dbt-0.5.0/prefect_dbt/cloud/models.py` & `prefect_dbt-0.6.0rc1/prefect_dbt/cloud/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 """Module containing models used for passing data to dbt Cloud"""
+
 from typing import List, Optional
 
-from pydantic import VERSION as PYDANTIC_VERSION
+from pydantic import BaseModel, Field
 
 from prefect.context import FlowRunContext, TaskRunContext, get_run_context
 
-if PYDANTIC_VERSION.startswith("2."):
-    from pydantic.v1 import BaseModel, Field
-else:
-    from pydantic import BaseModel, Field
-
 
 def default_cause_factory():
     """
     Factory function to populate the default cause for a job run to include information
     from the Prefect run context.
     """
     cause = "Triggered via Prefect"
```

### Comparing `prefect_dbt-0.5.0/prefect_dbt/cloud/runs.py` & `prefect_dbt-0.6.0rc1/prefect_dbt/cloud/runs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module containing tasks and flows for interacting with dbt Cloud job runs"""
+
 import asyncio
 from enum import Enum
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from httpx import HTTPStatusError
 from typing_extensions import Literal
 
@@ -270,20 +271,20 @@
 
 
     """
     logger = get_run_logger()
     seconds_waited_for_run_completion = 0
     wait_for = []
     while seconds_waited_for_run_completion <= max_wait_seconds:
-        run_data_future = await get_dbt_cloud_run_info.submit(
+        run_data_future = await get_dbt_cloud_run_info(
             dbt_cloud_credentials=dbt_cloud_credentials,
             run_id=run_id,
             wait_for=wait_for,
         )
-        run_data = await run_data_future.result()
+        run_data = run_data_future
         run_status_code = run_data.get("status")
 
         if DbtCloudJobRunStatus.is_terminal_status_code(run_status_code):
             return DbtCloudJobRunStatus(run_status_code), run_data
 
         wait_for = [run_data_future]
         logger.debug(
```

### Comparing `prefect_dbt-0.5.0/prefect_dbt/cloud/utils.py` & `prefect_dbt-0.6.0rc1/prefect_dbt/cloud/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Utilities for common interactions with the dbt Cloud API"""
+
 from json import JSONDecodeError
 from typing import Any, Dict, Optional
 
 from httpx import HTTPStatusError
 
 from prefect import task
 from prefect_dbt.cloud.credentials import DbtCloudCredentials
```

### Comparing `prefect_dbt-0.5.0/prefect_dbt.egg-info/PKG-INFO` & `prefect_dbt-0.6.0rc1/prefect_dbt.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,66 +1,64 @@
 Metadata-Version: 2.1
 Name: prefect-dbt
-Version: 0.5.0
+Version: 0.6.0rc1
 Summary: Prefect integrations for working with dbt
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-dbt
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
 License-File: LICENSE
-Requires-Dist: prefect<3.0.0,>=2.16.6
+Requires-Dist: prefect>=3.0.0rc1
 Requires-Dist: dbt-core>=1.7.0
-Requires-Dist: prefect_shell>=0.1.4
+Requires-Dist: prefect_shell>=0.3.0rc1
 Requires-Dist: sgqlc>=16.0.0
 Provides-Extra: snowflake
-Requires-Dist: prefect-snowflake>=0.2.4; extra == "snowflake"
+Requires-Dist: prefect-snowflake>=0.28.0rc1; extra == "snowflake"
 Requires-Dist: dbt-snowflake; extra == "snowflake"
 Provides-Extra: bigquery
-Requires-Dist: prefect-gcp[bigquery]>=0.1.8; extra == "bigquery"
+Requires-Dist: prefect-gcp[bigquery]>=0.6.0rc1; extra == "bigquery"
 Requires-Dist: dbt-bigquery; extra == "bigquery"
 Provides-Extra: postgres
-Requires-Dist: prefect-sqlalchemy>=0.2.1; extra == "postgres"
+Requires-Dist: prefect-sqlalchemy>=0.5.0rc1; extra == "postgres"
 Requires-Dist: dbt-postgres; extra == "postgres"
 Provides-Extra: all-extras
 Requires-Dist: dbt-bigquery; extra == "all-extras"
 Requires-Dist: dbt-postgres; extra == "all-extras"
 Requires-Dist: dbt-snowflake; extra == "all-extras"
-Requires-Dist: prefect-gcp[bigquery]>=0.1.8; extra == "all-extras"
-Requires-Dist: prefect-snowflake>=0.2.4; extra == "all-extras"
-Requires-Dist: prefect-sqlalchemy>=0.2.1; extra == "all-extras"
+Requires-Dist: prefect-gcp[bigquery]>=0.6.0rc1; extra == "all-extras"
+Requires-Dist: prefect-snowflake>=0.28.0rc1; extra == "all-extras"
+Requires-Dist: prefect-sqlalchemy>=0.5.0rc1; extra == "all-extras"
 Provides-Extra: dev
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: dbt-bigquery; extra == "dev"
 Requires-Dist: dbt-postgres; extra == "dev"
 Requires-Dist: dbt-snowflake; extra == "dev"
 Requires-Dist: interrogate; extra == "dev"
 Requires-Dist: mkdocs-gen-files; extra == "dev"
 Requires-Dist: mkdocs-material; extra == "dev"
 Requires-Dist: mkdocs; extra == "dev"
 Requires-Dist: mkdocstrings[python]; extra == "dev"
-Requires-Dist: mock; python_version < "3.8" and extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pillow; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
-Requires-Dist: prefect-gcp[bigquery]>=0.1.8; extra == "dev"
-Requires-Dist: prefect-snowflake>=0.2.4; extra == "dev"
-Requires-Dist: prefect-sqlalchemy>=0.2.1; extra == "dev"
+Requires-Dist: prefect-gcp[bigquery]>=0.6.0rc1; extra == "dev"
+Requires-Dist: prefect-snowflake>=0.28.0rc1; extra == "dev"
+Requires-Dist: prefect-sqlalchemy>=0.5.0rc1; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: pytest-xdist; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: respx; extra == "dev"
 
 # prefect-dbt
 
@@ -206,15 +204,15 @@
 
     ```bash
     pip install dbt-databricks
     ```
 
     Check out the [desired profile setup page](https://docs.getdbt.com/reference/profiles.yml) on the sidebar for others.
 
-Requires an installation of Python 3.8+.
+Requires an installation of Python 3.9+.
 
 We recommend using a Python virtual environment manager such as pipenv, conda or virtualenv.
 
 These tasks are designed to work with Prefect 2. For more information about how to use Prefect, please refer to the [Prefect documentation](https://docs.prefect.io/).
 
 ### Saving credentials to block
```

### Comparing `prefect_dbt-0.5.0/prefect_dbt.egg-info/SOURCES.txt` & `prefect_dbt-0.6.0rc1/prefect_dbt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prefect_dbt-0.5.0/prefect_dbt.egg-info/requires.txt` & `prefect_dbt-0.6.0rc1/prefect_dbt.egg-info/requires.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-prefect<3.0.0,>=2.16.6
+prefect>=3.0.0rc1
 dbt-core>=1.7.0
-prefect_shell>=0.1.4
+prefect_shell>=0.3.0rc1
 sgqlc>=16.0.0
 
 [all_extras]
 dbt-bigquery
 dbt-postgres
 dbt-snowflake
-prefect-gcp[bigquery]>=0.1.8
-prefect-snowflake>=0.2.4
-prefect-sqlalchemy>=0.2.1
+prefect-gcp[bigquery]>=0.6.0rc1
+prefect-snowflake>=0.28.0rc1
+prefect-sqlalchemy>=0.5.0rc1
 
 [bigquery]
-prefect-gcp[bigquery]>=0.1.8
+prefect-gcp[bigquery]>=0.6.0rc1
 dbt-bigquery
 
 [dev]
 coverage
 dbt-bigquery
 dbt-postgres
 dbt-snowflake
@@ -24,25 +24,22 @@
 mkdocs-gen-files
 mkdocs-material
 mkdocs
 mkdocstrings[python]
 mypy
 pillow
 pre-commit
-prefect-gcp[bigquery]>=0.1.8
-prefect-snowflake>=0.2.4
-prefect-sqlalchemy>=0.2.1
+prefect-gcp[bigquery]>=0.6.0rc1
+prefect-snowflake>=0.28.0rc1
+prefect-sqlalchemy>=0.5.0rc1
 pytest-asyncio
 pytest-xdist
 pytest
 respx
 
-[dev:python_version < "3.8"]
-mock
-
 [postgres]
-prefect-sqlalchemy>=0.2.1
+prefect-sqlalchemy>=0.5.0rc1
 dbt-postgres
 
 [snowflake]
-prefect-snowflake>=0.2.4
+prefect-snowflake>=0.28.0rc1
 dbt-snowflake
```

### Comparing `prefect_dbt-0.5.0/pyproject.toml` & `prefect_dbt-0.6.0rc1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,68 +2,66 @@
 requires = ["setuptools>=45", "wheel", "setuptools_scm>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "prefect-dbt"
 description = "Prefect integrations for working with dbt"
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
-  "prefect>=2.16.6, < 3.0.0",
+  "prefect>=3.0.0rc1",
   "dbt-core>=1.7.0",
-  "prefect_shell>=0.1.4",
+  "prefect_shell>=0.3.0rc1",
   "sgqlc>=16.0.0",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
-snowflake = ["prefect-snowflake>=0.2.4", "dbt-snowflake"]
-bigquery = ["prefect-gcp[bigquery]>=0.1.8", "dbt-bigquery"]
-postgres = ["prefect-sqlalchemy>=0.2.1", "dbt-postgres"]
+snowflake = ["prefect-snowflake>=0.28.0rc1", "dbt-snowflake"]
+bigquery = ["prefect-gcp[bigquery]>=0.6.0rc1", "dbt-bigquery"]
+postgres = ["prefect-sqlalchemy>=0.5.0rc1", "dbt-postgres"]
 all_extras = [
   "dbt-bigquery",
   "dbt-postgres",
   "dbt-snowflake",
-  "prefect-gcp[bigquery]>=0.1.8",
-  "prefect-snowflake>=0.2.4",
-  "prefect-sqlalchemy>=0.2.1",
+  "prefect-gcp[bigquery]>=0.6.0rc1",
+  "prefect-snowflake>=0.28.0rc1",
+  "prefect-sqlalchemy>=0.5.0rc1",
 ]
 dev = [
   "coverage",
   "dbt-bigquery",
   "dbt-postgres",
   "dbt-snowflake",
   "interrogate",
   "mkdocs-gen-files",
   "mkdocs-material",
   "mkdocs",
   "mkdocstrings[python]",
-  "mock; python_version < '3.8'",
   "mypy",
   "pillow",
   "pre-commit",
-  "prefect-gcp[bigquery]>=0.1.8",
-  "prefect-snowflake>=0.2.4",
-  "prefect-sqlalchemy>=0.2.1",
+  "prefect-gcp[bigquery]>=0.6.0rc1",
+  "prefect-snowflake>=0.28.0rc1",
+  "prefect-sqlalchemy>=0.5.0rc1",
   "pytest-asyncio",
   "pytest-xdist",
   "pytest",
   "respx",
 ]
 
 [project.urls]
@@ -71,15 +69,15 @@
 
 [project.entry-points."prefect.collections"]
 prefect_dbt = "prefect_dbt"
 
 [tool.setuptools_scm]
 version_file = "prefect_dbt/_version.py"
 root = "../../.."
-tag_regex = "^prefect-dbt-(?P<version>\\d+\\.\\d+\\.\\d+)$"
+tag_regex = "^prefect-dbt-(?P<version>\\d+\\.\\d+\\.\\d+(?:[a-zA-Z0-9]+(?:\\.[a-zA-Z0-9]+)*)?)$"
 fallback_version = "0.0.0"
 git_describe_command = 'git describe --dirty --tags --long --match "prefect-dbt-*[0-9]*"'
 
 [tool.interrogate]
 ignore-init-module = true
 ignore_init_method = true
 exclude = ["prefect_dbt/_version.py", "tests"]
```

### Comparing `prefect_dbt-0.5.0/tests/cli/configs/test_base.py` & `prefect_dbt-0.6.0rc1/tests/cli/configs/test_base.py`

 * *Files identical despite different names*

### Comparing `prefect_dbt-0.5.0/tests/cli/configs/test_bigquery.py` & `prefect_dbt-0.6.0rc1/tests/cli/configs/test_bigquery.py`

 * *Files identical despite different names*

### Comparing `prefect_dbt-0.5.0/tests/cli/configs/test_postgres.py` & `prefect_dbt-0.6.0rc1/tests/cli/configs/test_postgres.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,48 +1,13 @@
+from prefect_dbt.cli.configs import PostgresTargetConfigs
 from prefect_sqlalchemy import (
     ConnectionComponents,
-    DatabaseCredentials,
     SqlAlchemyConnector,
-    SyncDriver,
 )
-from pydantic import VERSION as PYDANTIC_VERSION
-
-if PYDANTIC_VERSION.startswith("2."):
-    from pydantic.v1 import SecretStr
-else:
-    from pydantic import SecretStr
-
-from prefect_dbt.cli.configs import PostgresTargetConfigs
-
-
-def test_postgres_target_configs_get_configs():
-    credentials = DatabaseCredentials(
-        driver=SyncDriver.POSTGRESQL_PSYCOPG2,
-        username="prefect",
-        password="prefect_password",
-        database="postgres",
-        host="host",
-        port=8080,
-    )
-    configs = PostgresTargetConfigs(schema="schema", credentials=credentials)
-    actual = configs.get_configs()
-    expected = {
-        "type": "postgres",
-        "schema": "schema",
-        "threads": 4,
-        "dbname": "postgres",
-        "user": "prefect",
-        "password": "prefect_password",
-        "host": "host",
-        "port": 8080,
-    }
-    for k, v in actual.items():
-        actual_v = v.get_secret_value() if isinstance(v, SecretStr) else v
-        expected_v = expected[k]
-        assert actual_v == expected_v
+from pydantic import SecretStr
 
 
 def test_postgres_target_configs_get_configs_for_sqlalchemy_connector():
     configs = PostgresTargetConfigs(
         credentials=SqlAlchemyConnector(
             connection_info=ConnectionComponents(
                 driver="postgresql+psycopg2",
```

### Comparing `prefect_dbt-0.5.0/tests/cli/configs/test_snowflake.py` & `prefect_dbt-0.6.0rc1/tests/cli/configs/test_snowflake.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,13 @@
 from pathlib import Path
 
+from prefect_dbt.cli.configs import SnowflakeTargetConfigs
 from prefect_snowflake.credentials import SnowflakeCredentials
 from prefect_snowflake.database import SnowflakeConnector
-from pydantic import VERSION as PYDANTIC_VERSION
-
-if PYDANTIC_VERSION.startswith("2."):
-    from pydantic.v1 import SecretBytes, SecretStr
-else:
-    from pydantic import SecretBytes, SecretStr
-
-from prefect_dbt.cli.configs import SnowflakeTargetConfigs
+from pydantic import SecretBytes, SecretStr
 
 
 def test_snowflake_target_configs_get_configs():
     credentials = SnowflakeCredentials(
         account="account",
         user="user",
         password="password",
```

### Comparing `prefect_dbt-0.5.0/tests/cli/test_commands.py` & `prefect_dbt-0.6.0rc1/tests/cli/test_commands.py`

 * *Files 16% similar despite different names*

```diff
@@ -389,83 +389,83 @@
         assert (
             mock_write.call_args_list[0][0][0]
             == f"dbt debug --profiles-dir {tmp_path} --project-dir {tmp_path}".encode()
         )
 
 
 @pytest.mark.usefixtures("dbt_runner_model_result")
-def test_run_dbt_build_creates_artifact(profiles_dir, dbt_cli_profile_bare):
+async def test_run_dbt_build_creates_artifact(profiles_dir, dbt_cli_profile_bare):
     @flow
-    def test_flow():
-        return run_dbt_build(
+    async def test_flow():
+        return await run_dbt_build(
             profiles_dir=profiles_dir,
             dbt_cli_profile=dbt_cli_profile_bare,
             summary_artifact_key="foo",
             create_summary_artifact=True,
         )
 
-    test_flow()
-    assert (a := Artifact.get(key="foo"))
+    await test_flow()
+    assert (a := await Artifact.get(key="foo"))
     assert a.type == "markdown"
     assert a.data.startswith("# dbt build Task Summary")
     assert "my_first_dbt_model" in a.data
     assert "Successful Nodes" in a.data
 
 
 @pytest.mark.usefixtures("dbt_runner_model_result")
-def test_run_dbt_test_creates_artifact(profiles_dir, dbt_cli_profile_bare):
+async def test_run_dbt_test_creates_artifact(profiles_dir, dbt_cli_profile_bare):
     @flow
-    def test_flow():
+    async def test_flow():
         return run_dbt_test(
             profiles_dir=profiles_dir,
             dbt_cli_profile=dbt_cli_profile_bare,
             summary_artifact_key="foo",
             create_summary_artifact=True,
         )
 
-    test_flow()
-    assert (a := Artifact.get(key="foo"))
+    await test_flow()
+    assert (a := await Artifact.get(key="foo"))
     assert a.type == "markdown"
     assert a.data.startswith("# dbt test Task Summary")
     assert "my_first_dbt_model" in a.data
     assert "Successful Nodes" in a.data
 
 
 @pytest.mark.usefixtures("dbt_runner_model_result")
-def test_run_dbt_snapshot_creates_artifact(profiles_dir, dbt_cli_profile_bare):
+async def test_run_dbt_snapshot_creates_artifact(profiles_dir, dbt_cli_profile_bare):
     @flow
-    def test_flow():
-        return run_dbt_snapshot(
+    async def test_flow():
+        return await run_dbt_snapshot(
             profiles_dir=profiles_dir,
             dbt_cli_profile=dbt_cli_profile_bare,
             summary_artifact_key="foo",
             create_summary_artifact=True,
         )
 
-    test_flow()
-    assert (a := Artifact.get(key="foo"))
+    await test_flow()
+    assert (a := await Artifact.get(key="foo"))
     assert a.type == "markdown"
     assert a.data.startswith("# dbt snapshot Task Summary")
     assert "my_first_dbt_model" in a.data
     assert "Successful Nodes" in a.data
 
 
 @pytest.mark.usefixtures("dbt_runner_model_result")
-def test_run_dbt_seed_creates_artifact(profiles_dir, dbt_cli_profile_bare):
+async def test_run_dbt_seed_creates_artifact(profiles_dir, dbt_cli_profile_bare):
     @flow
-    def test_flow():
-        return run_dbt_seed(
+    async def test_flow():
+        return await run_dbt_seed(
             profiles_dir=profiles_dir,
             dbt_cli_profile=dbt_cli_profile_bare,
             summary_artifact_key="foo",
             create_summary_artifact=True,
         )
 
-    test_flow()
-    assert (a := Artifact.get(key="foo"))
+    await test_flow()
+    assert (a := await Artifact.get(key="foo"))
     assert a.type == "markdown"
     assert a.data.startswith("# dbt seed Task Summary")
     assert "my_first_dbt_model" in a.data
     assert "Successful Nodes" in a.data
 
 
 @pytest.mark.usefixtures("dbt_runner_model_result")
@@ -476,15 +476,15 @@
             profiles_dir=profiles_dir,
             dbt_cli_profile=dbt_cli_profile_bare,
             summary_artifact_key="foo",
             create_summary_artifact=True,
         )
 
     test_flow()
-    assert (a := Artifact.get(key="foo"))
+    assert (a := await Artifact.get(key="foo"))
     assert a.type == "markdown"
     assert a.data.startswith("# dbt run Task Summary")
     assert "my_first_dbt_model" in a.data
     assert "Successful Nodes" in a.data
 
 
 @pytest.fixture
@@ -503,18 +503,18 @@
             profiles_dir=profiles_dir,
             dbt_cli_profile=dbt_cli_profile_bare,
             summary_artifact_key="foo",
             create_summary_artifact=True,
         )
 
     with pytest.raises(
-        Exception, match="dbt task result unsuccessful with exception: None"
+        Exception, match="dbt task result success: False with exception: None"
     ):
         test_flow()
-    assert (a := Artifact.get(key="foo"))
+    assert (a := await Artifact.get(key="foo"))
     assert a.type == "markdown"
     assert a.data.startswith("# dbt run Task Summary")
     assert "my_first_dbt_model" in a.data
     assert "Unsuccessful Nodes" in a.data
 
 
 @pytest.mark.usefixtures("dbt_runner_failed_result")
```

### Comparing `prefect_dbt-0.5.0/tests/cli/test_credentials.py` & `prefect_dbt-0.6.0rc1/tests/cli/test_credentials.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,34 @@
 import pytest
-from pydantic import VERSION as PYDANTIC_VERSION
-
-if PYDANTIC_VERSION.startswith("2."):
-    from pydantic.v1.error_wrappers import ValidationError
-else:
-    from pydantic.error_wrappers import ValidationError
-
 from prefect_dbt.cli.credentials import DbtCliProfile, GlobalConfigs, TargetConfigs
+from pydantic import ValidationError
 
 
 @pytest.mark.parametrize("configs_type", ["dict", "model"])
 def test_dbt_cli_profile_init(configs_type):
     target_configs = dict(type="snowflake", schema="schema")
     global_configs = dict(use_colors=False)
     if configs_type == "model":
-        target_configs = TargetConfigs.parse_obj(target_configs)
-        global_configs = GlobalConfigs.parse_obj(global_configs)
+        target_configs = TargetConfigs.model_validate(target_configs)
+        global_configs = GlobalConfigs.model_validate(global_configs)
 
     dbt_cli_profile = DbtCliProfile(
         name="test_name",
         target="dev",
         target_configs=target_configs,
         global_configs=global_configs,
     )
     assert isinstance(dbt_cli_profile.target_configs, TargetConfigs)
     assert dbt_cli_profile.name == "test_name"
     assert dbt_cli_profile.target == "dev"
 
 
 def test_dbt_cli_profile_init_validation_failed():
     # 6 instead of 2 now because it tries to validate each of the Union types
-    with pytest.raises(ValidationError, match="6 validation errors for DbtCliProfile"):
+    with pytest.raises(ValidationError):
         DbtCliProfile(
             name="test_name", target="dev", target_configs={"extras": {"field": "abc"}}
         )
 
 
 def test_dbt_cli_profile_get_profile():
     target_configs = dict(type="snowflake", schema="analysis")
@@ -62,18 +56,18 @@
     "target_configs_request",
     [
         "snowflake_target_configs",
         "dict_target_configs",
         "class_target_configs",
     ],
 )
-def test_dbt_cli_profile_save_load_roundtrip(target_configs_request, request):
+async def test_dbt_cli_profile_save_load_roundtrip(target_configs_request, request):
     target_configs = request.getfixturevalue(target_configs_request)
     dbt_cli_profile = DbtCliProfile(
         name="my_name",
         target="dev",
         target_configs=target_configs,
     )
     block_name = target_configs_request.replace("_", "-")
-    dbt_cli_profile.save(block_name)
-    dbt_cli_profile_loaded = DbtCliProfile.load(block_name)
+    await dbt_cli_profile.save(block_name)
+    dbt_cli_profile_loaded = await DbtCliProfile.load(block_name)
     assert dbt_cli_profile_loaded.get_profile()
```

### Comparing `prefect_dbt-0.5.0/tests/cloud/test_clients.py` & `prefect_dbt-0.6.0rc1/tests/cloud/test_clients.py`

 * *Files identical despite different names*

### Comparing `prefect_dbt-0.5.0/tests/cloud/test_cloud_credentials.py` & `prefect_dbt-0.6.0rc1/tests/cloud/test_cloud_credentials.py`

 * *Files identical despite different names*

### Comparing `prefect_dbt-0.5.0/tests/cloud/test_jobs.py` & `prefect_dbt-0.6.0rc1/tests/cloud/test_jobs.py`

 * *Files identical despite different names*

### Comparing `prefect_dbt-0.5.0/tests/cloud/test_runs.py` & `prefect_dbt-0.6.0rc1/tests/cloud/test_runs.py`

 * *Files identical despite different names*

### Comparing `prefect_dbt-0.5.0/tests/cloud/test_utils.py` & `prefect_dbt-0.6.0rc1/tests/cloud/test_utils.py`

 * *Files identical despite different names*

### Comparing `prefect_dbt-0.5.0/tests/conftest.py` & `prefect_dbt-0.6.0rc1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `prefect_dbt-0.5.0/tests/test_block_standards.py` & `prefect_dbt-0.6.0rc1/tests/test_block_standards.py`

 * *Files identical despite different names*

