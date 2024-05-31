# Comparing `tmp/flytekitplugins_airflow-1.12.1b4.tar.gz` & `tmp/flytekitplugins_airflow-1.12.1rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins_airflow-1.12.1b4.tar", last modified: Tue May 28 15:50:21 2024, max compression
+gzip compressed data, was "flytekitplugins_airflow-1.12.1rc0.tar", last modified: Fri May 31 21:49:28 2024, max compression
```

## Comparing `flytekitplugins_airflow-1.12.1b4.tar` & `flytekitplugins_airflow-1.12.1rc0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:50:21.059359 flytekitplugins_airflow-1.12.1b4/
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-28 15:50:21.059359 flytekitplugins_airflow-1.12.1b4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-28 15:49:57.000000 flytekitplugins_airflow-1.12.1b4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:50:21.059359 flytekitplugins_airflow-1.12.1b4/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:50:21.059359 flytekitplugins_airflow-1.12.1b4/flytekitplugins/airflow/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-28 15:49:57.000000 flytekitplugins_airflow-1.12.1b4/flytekitplugins/airflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7959 2024-05-28 15:49:57.000000 flytekitplugins_airflow-1.12.1b4/flytekitplugins/airflow/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     9131 2024-05-28 15:49:57.000000 flytekitplugins_airflow-1.12.1b4/flytekitplugins/airflow/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:50:21.059359 flytekitplugins_airflow-1.12.1b4/flytekitplugins_airflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-28 15:50:21.000000 flytekitplugins_airflow-1.12.1b4/flytekitplugins_airflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-28 15:50:21.000000 flytekitplugins_airflow-1.12.1b4/flytekitplugins_airflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 15:50:21.000000 flytekitplugins_airflow-1.12.1b4/flytekitplugins_airflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-28 15:50:21.000000 flytekitplugins_airflow-1.12.1b4/flytekitplugins_airflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-28 15:50:21.000000 flytekitplugins_airflow-1.12.1b4/flytekitplugins_airflow.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-28 15:50:21.000000 flytekitplugins_airflow-1.12.1b4/flytekitplugins_airflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-28 15:50:21.000000 flytekitplugins_airflow-1.12.1b4/flytekitplugins_airflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 15:50:21.059359 flytekitplugins_airflow-1.12.1b4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-28 15:50:20.000000 flytekitplugins_airflow-1.12.1b4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:50:21.059359 flytekitplugins_airflow-1.12.1b4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-05-28 15:49:57.000000 flytekitplugins_airflow-1.12.1b4/tests/test_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     4770 2024-05-28 15:49:57.000000 flytekitplugins_airflow-1.12.1b4/tests/test_task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:49:28.284996 flytekitplugins_airflow-1.12.1rc0/
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-31 21:49:28.284996 flytekitplugins_airflow-1.12.1rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-31 21:49:04.000000 flytekitplugins_airflow-1.12.1rc0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:49:28.284996 flytekitplugins_airflow-1.12.1rc0/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:49:28.284996 flytekitplugins_airflow-1.12.1rc0/flytekitplugins/airflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-31 21:49:04.000000 flytekitplugins_airflow-1.12.1rc0/flytekitplugins/airflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7959 2024-05-31 21:49:04.000000 flytekitplugins_airflow-1.12.1rc0/flytekitplugins/airflow/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9131 2024-05-31 21:49:04.000000 flytekitplugins_airflow-1.12.1rc0/flytekitplugins/airflow/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:49:28.284996 flytekitplugins_airflow-1.12.1rc0/flytekitplugins_airflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-31 21:49:28.000000 flytekitplugins_airflow-1.12.1rc0/flytekitplugins_airflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-31 21:49:28.000000 flytekitplugins_airflow-1.12.1rc0/flytekitplugins_airflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 21:49:28.000000 flytekitplugins_airflow-1.12.1rc0/flytekitplugins_airflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-31 21:49:28.000000 flytekitplugins_airflow-1.12.1rc0/flytekitplugins_airflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-31 21:49:28.000000 flytekitplugins_airflow-1.12.1rc0/flytekitplugins_airflow.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-31 21:49:28.000000 flytekitplugins_airflow-1.12.1rc0/flytekitplugins_airflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-31 21:49:28.000000 flytekitplugins_airflow-1.12.1rc0/flytekitplugins_airflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 21:49:28.284996 flytekitplugins_airflow-1.12.1rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-05-31 21:49:27.000000 flytekitplugins_airflow-1.12.1rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:49:28.284996 flytekitplugins_airflow-1.12.1rc0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-05-31 21:49:04.000000 flytekitplugins_airflow-1.12.1rc0/tests/test_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4770 2024-05-31 21:49:04.000000 flytekitplugins_airflow-1.12.1rc0/tests/test_task.py
```

### Comparing `flytekitplugins_airflow-1.12.1b4/PKG-INFO` & `flytekitplugins_airflow-1.12.1rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-airflow
-Version: 1.12.1b4
+Version: 1.12.1rc0
 Summary: This package holds the Airflow plugins for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins_airflow-1.12.1b4/README.md` & `flytekitplugins_airflow-1.12.1rc0/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins_airflow-1.12.1b4/flytekitplugins/airflow/agent.py` & `flytekitplugins_airflow-1.12.1rc0/flytekitplugins/airflow/agent.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins_airflow-1.12.1b4/flytekitplugins/airflow/task.py` & `flytekitplugins_airflow-1.12.1rc0/flytekitplugins/airflow/task.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins_airflow-1.12.1b4/flytekitplugins_airflow.egg-info/PKG-INFO` & `flytekitplugins_airflow-1.12.1rc0/flytekitplugins_airflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-airflow
-Version: 1.12.1b4
+Version: 1.12.1rc0
 Summary: This package holds the Airflow plugins for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins_airflow-1.12.1b4/setup.py` & `flytekitplugins_airflow-1.12.1rc0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 plugin_requires = [
     "apache-airflow",
     "flytekit>1.10.7",
     "flyteidl>1.10.7",
 ]
 
-__version__ = "1.12.1b4"
+__version__ = "1.12.1-rc0"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="This package holds the Airflow plugins for flytekit",
```

### Comparing `flytekitplugins_airflow-1.12.1b4/tests/test_agent.py` & `flytekitplugins_airflow-1.12.1rc0/tests/test_agent.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins_airflow-1.12.1b4/tests/test_task.py` & `flytekitplugins_airflow-1.12.1rc0/tests/test_task.py`

 * *Files identical despite different names*

