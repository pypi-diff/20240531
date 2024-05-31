# Comparing `tmp/cdk8s-plus-28-2.3.4.tar.gz` & `tmp/cdk8s-plus-28-2.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk8s-plus-28-2.3.4.tar", last modified: Tue May 21 12:38:12 2024, max compression
+gzip compressed data, was "cdk8s-plus-28-2.3.5.tar", last modified: Fri May 31 12:14:35 2024, max compression
```

## Comparing `cdk8s-plus-28-2.3.4.tar` & `cdk8s-plus-28-2.3.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:38:12.009624 cdk8s-plus-28-2.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-21 12:38:02.000000 cdk8s-plus-28-2.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-21 12:38:02.000000 cdk8s-plus-28-2.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-21 12:38:02.000000 cdk8s-plus-28-2.3.4/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-05-21 12:38:12.009624 cdk8s-plus-28-2.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-05-21 12:38:02.000000 cdk8s-plus-28-2.3.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-21 12:38:02.000000 cdk8s-plus-28-2.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 12:38:12.009624 cdk8s-plus-28-2.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-21 12:38:02.000000 cdk8s-plus-28-2.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:38:11.997624 cdk8s-plus-28-2.3.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:38:12.001624 cdk8s-plus-28-2.3.4/src/cdk8s_plus_28/
--rw-r--r--   0 runner    (1001) docker     (127)  1180500 2024-05-21 12:38:02.000000 cdk8s-plus-28-2.3.4/src/cdk8s_plus_28/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:38:12.001624 cdk8s-plus-28-2.3.4/src/cdk8s_plus_28/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-21 12:38:02.000000 cdk8s-plus-28-2.3.4/src/cdk8s_plus_28/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  1351365 2024-05-21 12:38:02.000000 cdk8s-plus-28-2.3.4/src/cdk8s_plus_28/_jsii/cdk8s-plus-28@2.3.4.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:38:12.005624 cdk8s-plus-28-2.3.4/src/cdk8s_plus_28/k8s/
--rw-r--r--   0 runner    (1001) docker     (127)  3002746 2024-05-21 12:38:02.000000 cdk8s-plus-28-2.3.4/src/cdk8s_plus_28/k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 12:38:02.000000 cdk8s-plus-28-2.3.4/src/cdk8s_plus_28/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:38:12.001624 cdk8s-plus-28-2.3.4/src/cdk8s_plus_28.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-05-21 12:38:11.000000 cdk8s-plus-28-2.3.4/src/cdk8s_plus_28.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-21 12:38:11.000000 cdk8s-plus-28-2.3.4/src/cdk8s_plus_28.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 12:38:11.000000 cdk8s-plus-28-2.3.4/src/cdk8s_plus_28.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-21 12:38:11.000000 cdk8s-plus-28-2.3.4/src/cdk8s_plus_28.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-21 12:38:11.000000 cdk8s-plus-28-2.3.4/src/cdk8s_plus_28.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:14:35.956841 cdk8s-plus-28-2.3.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-31 12:14:25.000000 cdk8s-plus-28-2.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-31 12:14:25.000000 cdk8s-plus-28-2.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-31 12:14:25.000000 cdk8s-plus-28-2.3.5/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-05-31 12:14:35.956841 cdk8s-plus-28-2.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-05-31 12:14:25.000000 cdk8s-plus-28-2.3.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-31 12:14:25.000000 cdk8s-plus-28-2.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 12:14:35.956841 cdk8s-plus-28-2.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-31 12:14:25.000000 cdk8s-plus-28-2.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:14:35.948841 cdk8s-plus-28-2.3.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:14:35.948841 cdk8s-plus-28-2.3.5/src/cdk8s_plus_28/
+-rw-r--r--   0 runner    (1001) docker     (127)  1180500 2024-05-31 12:14:25.000000 cdk8s-plus-28-2.3.5/src/cdk8s_plus_28/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:14:35.952841 cdk8s-plus-28-2.3.5/src/cdk8s_plus_28/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-31 12:14:25.000000 cdk8s-plus-28-2.3.5/src/cdk8s_plus_28/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1351375 2024-05-31 12:14:25.000000 cdk8s-plus-28-2.3.5/src/cdk8s_plus_28/_jsii/cdk8s-plus-28@2.3.5.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:14:35.952841 cdk8s-plus-28-2.3.5/src/cdk8s_plus_28/k8s/
+-rw-r--r--   0 runner    (1001) docker     (127)  3002746 2024-05-31 12:14:25.000000 cdk8s-plus-28-2.3.5/src/cdk8s_plus_28/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 12:14:25.000000 cdk8s-plus-28-2.3.5/src/cdk8s_plus_28/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:14:35.952841 cdk8s-plus-28-2.3.5/src/cdk8s_plus_28.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-05-31 12:14:35.000000 cdk8s-plus-28-2.3.5/src/cdk8s_plus_28.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-31 12:14:35.000000 cdk8s-plus-28-2.3.5/src/cdk8s_plus_28.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 12:14:35.000000 cdk8s-plus-28-2.3.5/src/cdk8s_plus_28.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-31 12:14:35.000000 cdk8s-plus-28-2.3.5/src/cdk8s_plus_28.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-31 12:14:35.000000 cdk8s-plus-28-2.3.5/src/cdk8s_plus_28.egg-info/top_level.txt
```

### Comparing `cdk8s-plus-28-2.3.4/LICENSE` & `cdk8s-plus-28-2.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk8s-plus-28-2.3.4/PKG-INFO` & `cdk8s-plus-28-2.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk8s-plus-28
-Version: 2.3.4
+Version: 2.3.5
 Summary: cdk8s+ is a software development framework that provides high level abstractions for authoring Kubernetes applications. cdk8s-plus-28 synthesizes Kubernetes manifests for Kubernetes 1.28.0
 Home-page: https://github.com/cdk8s-team/cdk8s-plus.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdk8s-team/cdk8s-plus.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk8s-plus-28-2.3.4/README.md` & `cdk8s-plus-28-2.3.5/README.md`

 * *Files identical despite different names*

### Comparing `cdk8s-plus-28-2.3.4/setup.py` & `cdk8s-plus-28-2.3.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk8s-plus-28",
-    "version": "2.3.4",
+    "version": "2.3.5",
     "description": "cdk8s+ is a software development framework that provides high level abstractions for authoring Kubernetes applications. cdk8s-plus-28 synthesizes Kubernetes manifests for Kubernetes 1.28.0",
     "license": "Apache-2.0",
     "url": "https://github.com/cdk8s-team/cdk8s-plus.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -23,15 +23,15 @@
     "packages": [
         "cdk8s_plus_28",
         "cdk8s_plus_28._jsii",
         "cdk8s_plus_28.k8s"
     ],
     "package_data": {
         "cdk8s_plus_28._jsii": [
-            "cdk8s-plus-28@2.3.4.jsii.tgz"
+            "cdk8s-plus-28@2.3.5.jsii.tgz"
         ],
         "cdk8s_plus_28": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `cdk8s-plus-28-2.3.4/src/cdk8s_plus_28/__init__.py` & `cdk8s-plus-28-2.3.5/src/cdk8s_plus_28/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk8s-plus-28-2.3.4/src/cdk8s_plus_28/k8s/__init__.py` & `cdk8s-plus-28-2.3.5/src/cdk8s_plus_28/k8s/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk8s-plus-28-2.3.4/src/cdk8s_plus_28.egg-info/PKG-INFO` & `cdk8s-plus-28-2.3.5/src/cdk8s_plus_28.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk8s-plus-28
-Version: 2.3.4
+Version: 2.3.5
 Summary: cdk8s+ is a software development framework that provides high level abstractions for authoring Kubernetes applications. cdk8s-plus-28 synthesizes Kubernetes manifests for Kubernetes 1.28.0
 Home-page: https://github.com/cdk8s-team/cdk8s-plus.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdk8s-team/cdk8s-plus.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

