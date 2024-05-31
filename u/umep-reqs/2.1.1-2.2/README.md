# Comparing `tmp/umep-reqs-2.1.1.tar.gz` & `tmp/umep_reqs-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "umep-reqs-2.1.1.tar", last modified: Thu Jun  1 17:29:36 2023, max compression
+gzip compressed data, was "umep_reqs-2.2.tar", last modified: Fri May 31 12:59:11 2024, max compression
```

## Comparing `umep-reqs-2.1.1.tar` & `umep_reqs-2.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:29:36.625202 umep-reqs-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-01 17:29:36.625202 umep-reqs-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-01 17:29:28.000000 umep-reqs-2.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 17:29:36.625202 umep-reqs-2.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:29:36.625202 umep-reqs-2.1.1/umep-reqs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 17:29:28.000000 umep-reqs-2.1.1/umep-reqs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-01 17:29:28.000000 umep-reqs-2.1.1/umep-reqs/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:29:36.625202 umep-reqs-2.1.1/umep_reqs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-01 17:29:36.000000 umep-reqs-2.1.1/umep_reqs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-01 17:29:36.000000 umep-reqs-2.1.1/umep_reqs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 17:29:36.000000 umep-reqs-2.1.1/umep_reqs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-01 17:29:36.000000 umep-reqs-2.1.1/umep_reqs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-01 17:29:36.000000 umep-reqs-2.1.1/umep_reqs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:59:11.405678 umep_reqs-2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-31 12:59:11.405678 umep_reqs-2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-31 12:59:01.000000 umep_reqs-2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 12:59:11.405678 umep_reqs-2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:59:11.405678 umep_reqs-2.2/umep-reqs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 12:59:01.000000 umep_reqs-2.2/umep-reqs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-31 12:59:01.000000 umep_reqs-2.2/umep-reqs/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:59:11.405678 umep_reqs-2.2/umep_reqs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-31 12:59:11.000000 umep_reqs-2.2/umep_reqs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-31 12:59:11.000000 umep_reqs-2.2/umep_reqs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 12:59:11.000000 umep_reqs-2.2/umep_reqs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-31 12:59:11.000000 umep_reqs-2.2/umep_reqs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-31 12:59:11.000000 umep_reqs-2.2/umep_reqs.egg-info/top_level.txt
```

### Comparing `umep-reqs-2.1.1/umep-reqs/setup.py` & `umep_reqs-2.2/umep-reqs/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,16 +23,16 @@
     long_description = f.read()
 
 setup(
     name="umep-reqs",
     version=get_version(),  # Use setuptools_scm to get version from git tags.
     packages=find_packages(),
     install_requires=[
-        "supy==2023.5.26.dev0",  # Replace with actual dependency and version number.
-        "numba",
+        "supy==2024.5.24.dev",  # Replace with actual dependency and version number.
+        "numba==0.59.0",
         "jaydebeapi==1.2.3",
         "netCDF4", #   "dependency2==y.y.y" 
     ],
     author="UMEP dev team",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

