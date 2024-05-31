# Comparing `tmp/flytekitplugins-polars-1.9.0a0.tar.gz` & `tmp/flytekitplugins-polars-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-polars-1.9.0a0.tar", last modified: Thu Jul 20 18:58:24 2023, max compression
+gzip compressed data, was "flytekitplugins-polars-1.9.1.tar", last modified: Mon Aug 28 16:43:12 2023, max compression
```

## Comparing `flytekitplugins-polars-1.9.0a0.tar` & `flytekitplugins-polars-1.9.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:24.940733 flytekitplugins-polars-1.9.0a0/
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-20 18:58:24.940733 flytekitplugins-polars-1.9.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-20 18:57:54.000000 flytekitplugins-polars-1.9.0a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:24.940733 flytekitplugins-polars-1.9.0a0/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:24.940733 flytekitplugins-polars-1.9.0a0/flytekitplugins/polars/
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-20 18:57:54.000000 flytekitplugins-polars-1.9.0a0/flytekitplugins/polars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-07-20 18:57:54.000000 flytekitplugins-polars-1.9.0a0/flytekitplugins/polars/sd_transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:24.940733 flytekitplugins-polars-1.9.0a0/flytekitplugins_polars.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-20 18:58:24.000000 flytekitplugins-polars-1.9.0a0/flytekitplugins_polars.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-20 18:58:24.000000 flytekitplugins-polars-1.9.0a0/flytekitplugins_polars.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 18:58:24.000000 flytekitplugins-polars-1.9.0a0/flytekitplugins_polars.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-20 18:58:24.000000 flytekitplugins-polars-1.9.0a0/flytekitplugins_polars.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 18:58:24.000000 flytekitplugins-polars-1.9.0a0/flytekitplugins_polars.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-20 18:58:24.000000 flytekitplugins-polars-1.9.0a0/flytekitplugins_polars.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 18:58:24.000000 flytekitplugins-polars-1.9.0a0/flytekitplugins_polars.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 18:58:24.940733 flytekitplugins-polars-1.9.0a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-20 18:58:12.000000 flytekitplugins-polars-1.9.0a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:43:12.502129 flytekitplugins-polars-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (999)      756 2023-08-28 16:43:12.502129 flytekitplugins-polars-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)      469 2023-08-28 16:42:38.000000 flytekitplugins-polars-1.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:43:12.502129 flytekitplugins-polars-1.9.1/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:43:12.502129 flytekitplugins-polars-1.9.1/flytekitplugins/polars/
+-rw-r--r--   0 runner    (1001) docker     (999)      400 2023-08-28 16:42:38.000000 flytekitplugins-polars-1.9.1/flytekitplugins/polars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2996 2023-08-28 16:42:38.000000 flytekitplugins-polars-1.9.1/flytekitplugins/polars/sd_transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:43:12.502129 flytekitplugins-polars-1.9.1/flytekitplugins_polars.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (999)      756 2023-08-28 16:43:12.000000 flytekitplugins-polars-1.9.1/flytekitplugins_polars.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)      428 2023-08-28 16:43:12.000000 flytekitplugins-polars-1.9.1/flytekitplugins_polars.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-28 16:43:12.000000 flytekitplugins-polars-1.9.1/flytekitplugins_polars.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       51 2023-08-28 16:43:12.000000 flytekitplugins-polars-1.9.1/flytekitplugins_polars.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       16 2023-08-28 16:43:12.000000 flytekitplugins-polars-1.9.1/flytekitplugins_polars.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       40 2023-08-28 16:43:12.000000 flytekitplugins-polars-1.9.1/flytekitplugins_polars.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       16 2023-08-28 16:43:12.000000 flytekitplugins-polars-1.9.1/flytekitplugins_polars.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       38 2023-08-28 16:43:12.502129 flytekitplugins-polars-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (999)     1252 2023-08-28 16:43:00.000000 flytekitplugins-polars-1.9.1/setup.py
```

### Comparing `flytekitplugins-polars-1.9.0a0/PKG-INFO` & `flytekitplugins-polars-1.9.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-polars
-Version: 1.9.0a0
+Version: 1.9.1
 Summary: Polars plugin for flytekit
 Author: Robin Kahlow
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `flytekitplugins-polars-1.9.0a0/flytekitplugins/polars/sd_transformers.py` & `flytekitplugins-polars-1.9.1/flytekitplugins/polars/sd_transformers.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-polars-1.9.0a0/flytekitplugins_polars.egg-info/PKG-INFO` & `flytekitplugins-polars-1.9.1/flytekitplugins_polars.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-polars
-Version: 1.9.0a0
+Version: 1.9.1
 Summary: Polars plugin for flytekit
 Author: Robin Kahlow
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `flytekitplugins-polars-1.9.0a0/setup.py` & `flytekitplugins-polars-1.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = [
     "flytekit>=1.3.0b2,<2.0.0",
     "polars>=0.8.27",
 ]
 
-__version__ = "1.9.0a0"
+__version__ = "1.9.1"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="Robin Kahlow",
     description="Polars plugin for flytekit",
     namespace_packages=["flytekitplugins"],
```

