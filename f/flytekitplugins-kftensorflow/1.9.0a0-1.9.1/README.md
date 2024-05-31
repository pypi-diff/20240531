# Comparing `tmp/flytekitplugins-kftensorflow-1.9.0a0.tar.gz` & `tmp/flytekitplugins-kftensorflow-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-kftensorflow-1.9.0a0.tar", last modified: Thu Jul 20 18:58:21 2023, max compression
+gzip compressed data, was "flytekitplugins-kftensorflow-1.9.1.tar", last modified: Mon Aug 28 16:43:09 2023, max compression
```

## Comparing `flytekitplugins-kftensorflow-1.9.0a0.tar` & `flytekitplugins-kftensorflow-1.9.1.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:21.632701 flytekitplugins-kftensorflow-1.9.0a0/
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-20 18:58:21.632701 flytekitplugins-kftensorflow-1.9.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-20 18:57:54.000000 flytekitplugins-kftensorflow-1.9.0a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:21.628701 flytekitplugins-kftensorflow-1.9.0a0/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:21.632701 flytekitplugins-kftensorflow-1.9.0a0/flytekitplugins/kftensorflow/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-20 18:57:54.000000 flytekitplugins-kftensorflow-1.9.0a0/flytekitplugins/kftensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-07-20 18:57:54.000000 flytekitplugins-kftensorflow-1.9.0a0/flytekitplugins/kftensorflow/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-07-20 18:57:54.000000 flytekitplugins-kftensorflow-1.9.0a0/flytekitplugins/kftensorflow/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:21.632701 flytekitplugins-kftensorflow-1.9.0a0/flytekitplugins_kftensorflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-20 18:58:21.000000 flytekitplugins-kftensorflow-1.9.0a0/flytekitplugins_kftensorflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-20 18:58:21.000000 flytekitplugins-kftensorflow-1.9.0a0/flytekitplugins_kftensorflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 18:58:21.000000 flytekitplugins-kftensorflow-1.9.0a0/flytekitplugins_kftensorflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 18:58:21.000000 flytekitplugins-kftensorflow-1.9.0a0/flytekitplugins_kftensorflow.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-20 18:58:21.000000 flytekitplugins-kftensorflow-1.9.0a0/flytekitplugins_kftensorflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 18:58:21.000000 flytekitplugins-kftensorflow-1.9.0a0/flytekitplugins_kftensorflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 18:58:21.632701 flytekitplugins-kftensorflow-1.9.0a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-20 18:58:12.000000 flytekitplugins-kftensorflow-1.9.0a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:43:09.126125 flytekitplugins-kftensorflow-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (999)      802 2023-08-28 16:43:09.126125 flytekitplugins-kftensorflow-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)     1763 2023-08-28 16:42:38.000000 flytekitplugins-kftensorflow-1.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:43:09.126125 flytekitplugins-kftensorflow-1.9.1/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:43:09.126125 flytekitplugins-kftensorflow-1.9.1/flytekitplugins/kftensorflow/
+-rw-r--r--   0 runner    (1001) docker     (999)      290 2023-08-28 16:42:38.000000 flytekitplugins-kftensorflow-1.9.1/flytekitplugins/kftensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     8342 2023-08-28 16:42:38.000000 flytekitplugins-kftensorflow-1.9.1/flytekitplugins/kftensorflow/task.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:43:09.126125 flytekitplugins-kftensorflow-1.9.1/flytekitplugins_kftensorflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (999)      802 2023-08-28 16:43:09.000000 flytekitplugins-kftensorflow-1.9.1/flytekitplugins_kftensorflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)      416 2023-08-28 16:43:09.000000 flytekitplugins-kftensorflow-1.9.1/flytekitplugins_kftensorflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-28 16:43:09.000000 flytekitplugins-kftensorflow-1.9.1/flytekitplugins_kftensorflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       16 2023-08-28 16:43:09.000000 flytekitplugins-kftensorflow-1.9.1/flytekitplugins_kftensorflow.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       16 2023-08-28 16:43:09.000000 flytekitplugins-kftensorflow-1.9.1/flytekitplugins_kftensorflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       16 2023-08-28 16:43:09.000000 flytekitplugins-kftensorflow-1.9.1/flytekitplugins_kftensorflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       38 2023-08-28 16:43:09.126125 flytekitplugins-kftensorflow-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (999)     1139 2023-08-28 16:43:00.000000 flytekitplugins-kftensorflow-1.9.1/setup.py
```

### Comparing `flytekitplugins-kftensorflow-1.9.0a0/PKG-INFO` & `flytekitplugins-kftensorflow-1.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-kftensorflow
-Version: 1.9.0a0
+Version: 1.9.1
 Summary: K8s based Tensorflow plugin for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-kftensorflow-1.9.0a0/flytekitplugins_kftensorflow.egg-info/PKG-INFO` & `flytekitplugins-kftensorflow-1.9.1/flytekitplugins_kftensorflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-kftensorflow
-Version: 1.9.0a0
+Version: 1.9.1
 Summary: K8s based Tensorflow plugin for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-kftensorflow-1.9.0a0/setup.py` & `flytekitplugins-kftensorflow-1.9.1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from setuptools import setup
 
 PLUGIN_NAME = "kftensorflow"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
-# TODO: Requirements are missing, add them back in later.
-plugin_requires = ["flytekit>=1.3.0b2,<2.0.0"]
+plugin_requires = ["flytekit>=1.6.1"]
 
-__version__ = "1.9.0a0"
+__version__ = "1.9.1"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="K8s based Tensorflow plugin for flytekit",
```

