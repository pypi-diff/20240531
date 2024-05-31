# Comparing `tmp/cdk8s-cdktf-resolver-0.0.82.tar.gz` & `tmp/cdk8s-cdktf-resolver-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk8s-cdktf-resolver-0.0.82.tar", last modified: Fri May 31 12:15:43 2024, max compression
+gzip compressed data, was "cdk8s-cdktf-resolver-0.0.9.tar", last modified: Sat Oct 14 06:17:33 2023, max compression
```

## Comparing `cdk8s-cdktf-resolver-0.0.82.tar` & `cdk8s-cdktf-resolver-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:15:43.788710 cdk8s-cdktf-resolver-0.0.82/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-31 12:15:30.000000 cdk8s-cdktf-resolver-0.0.82/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-31 12:15:30.000000 cdk8s-cdktf-resolver-0.0.82/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6993 2024-05-31 12:15:43.788710 cdk8s-cdktf-resolver-0.0.82/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6105 2024-05-31 12:15:30.000000 cdk8s-cdktf-resolver-0.0.82/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-31 12:15:30.000000 cdk8s-cdktf-resolver-0.0.82/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 12:15:43.788710 cdk8s-cdktf-resolver-0.0.82/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-05-31 12:15:30.000000 cdk8s-cdktf-resolver-0.0.82/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:15:43.784710 cdk8s-cdktf-resolver-0.0.82/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:15:43.784710 cdk8s-cdktf-resolver-0.0.82/src/cdk8s_cdktf_resolver/
--rw-r--r--   0 runner    (1001) docker     (127)     9310 2024-05-31 12:15:30.000000 cdk8s-cdktf-resolver-0.0.82/src/cdk8s_cdktf_resolver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:15:43.788710 cdk8s-cdktf-resolver-0.0.82/src/cdk8s_cdktf_resolver/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-31 12:15:30.000000 cdk8s-cdktf-resolver-0.0.82/src/cdk8s_cdktf_resolver/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21020 2024-05-31 12:15:30.000000 cdk8s-cdktf-resolver-0.0.82/src/cdk8s_cdktf_resolver/_jsii/cdktf-resolver@0.0.82.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 12:15:30.000000 cdk8s-cdktf-resolver-0.0.82/src/cdk8s_cdktf_resolver/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:15:43.788710 cdk8s-cdktf-resolver-0.0.82/src/cdk8s_cdktf_resolver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6993 2024-05-31 12:15:43.000000 cdk8s-cdktf-resolver-0.0.82/src/cdk8s_cdktf_resolver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-31 12:15:43.000000 cdk8s-cdktf-resolver-0.0.82/src/cdk8s_cdktf_resolver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 12:15:43.000000 cdk8s-cdktf-resolver-0.0.82/src/cdk8s_cdktf_resolver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-31 12:15:43.000000 cdk8s-cdktf-resolver-0.0.82/src/cdk8s_cdktf_resolver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-31 12:15:43.000000 cdk8s-cdktf-resolver-0.0.82/src/cdk8s_cdktf_resolver.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 06:17:33.350856 cdk8s-cdktf-resolver-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2023-10-14 06:17:19.000000 cdk8s-cdktf-resolver-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2023-10-14 06:17:19.000000 cdk8s-cdktf-resolver-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7042 2023-10-14 06:17:33.350856 cdk8s-cdktf-resolver-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6105 2023-10-14 06:17:19.000000 cdk8s-cdktf-resolver-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2023-10-14 06:17:19.000000 cdk8s-cdktf-resolver-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-14 06:17:33.350856 cdk8s-cdktf-resolver-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2023-10-14 06:17:19.000000 cdk8s-cdktf-resolver-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 06:17:33.346856 cdk8s-cdktf-resolver-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 06:17:33.350856 cdk8s-cdktf-resolver-0.0.9/src/cdk8s_cdktf_resolver/
+-rw-r--r--   0 runner    (1001) docker     (127)     9234 2023-10-14 06:17:19.000000 cdk8s-cdktf-resolver-0.0.9/src/cdk8s_cdktf_resolver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 06:17:33.350856 cdk8s-cdktf-resolver-0.0.9/src/cdk8s_cdktf_resolver/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2023-10-14 06:17:19.000000 cdk8s-cdktf-resolver-0.0.9/src/cdk8s_cdktf_resolver/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22291 2023-10-14 06:17:19.000000 cdk8s-cdktf-resolver-0.0.9/src/cdk8s_cdktf_resolver/_jsii/cdktf-resolver@0.0.9.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-14 06:17:19.000000 cdk8s-cdktf-resolver-0.0.9/src/cdk8s_cdktf_resolver/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 06:17:33.350856 cdk8s-cdktf-resolver-0.0.9/src/cdk8s_cdktf_resolver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7042 2023-10-14 06:17:33.000000 cdk8s-cdktf-resolver-0.0.9/src/cdk8s_cdktf_resolver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2023-10-14 06:17:33.000000 cdk8s-cdktf-resolver-0.0.9/src/cdk8s_cdktf_resolver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-14 06:17:33.000000 cdk8s-cdktf-resolver-0.0.9/src/cdk8s_cdktf_resolver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2023-10-14 06:17:33.000000 cdk8s-cdktf-resolver-0.0.9/src/cdk8s_cdktf_resolver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2023-10-14 06:17:33.000000 cdk8s-cdktf-resolver-0.0.9/src/cdk8s_cdktf_resolver.egg-info/top_level.txt
```

### Comparing `cdk8s-cdktf-resolver-0.0.82/LICENSE` & `cdk8s-cdktf-resolver-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk8s-cdktf-resolver-0.0.82/PKG-INFO` & `cdk8s-cdktf-resolver-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: cdk8s-cdktf-resolver
-Version: 0.0.82
+Version: 0.0.9
 Summary: @cdk8s/cdktf-resolver
 Home-page: https://github.com/cdk8s-team/cdk8s-cdktf-resolver.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdk8s-team/cdk8s-cdktf-resolver.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
-Requires-Python: ~=3.8
+Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CDK For Terraform Resolver
 
 The `CdkTfResolver` is able to resolve any [`TerraformOutput`](https://developer.hashicorp.com/terraform/cdktf/concepts/variables-and-outputs#output-values)
 defined by your CDKTF application. In this example, we create an S3 `Bucket` with the CDKTF, and pass its (deploy time generated)
```

### Comparing `cdk8s-cdktf-resolver-0.0.82/README.md` & `cdk8s-cdktf-resolver-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `cdk8s-cdktf-resolver-0.0.82/setup.py` & `cdk8s-cdktf-resolver-0.0.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk8s-cdktf-resolver",
-    "version": "0.0.82",
+    "version": "0.0.9",
     "description": "@cdk8s/cdktf-resolver",
     "license": "Apache-2.0",
     "url": "https://github.com/cdk8s-team/cdk8s-cdktf-resolver.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,34 +22,35 @@
     },
     "packages": [
         "cdk8s_cdktf_resolver",
         "cdk8s_cdktf_resolver._jsii"
     ],
     "package_data": {
         "cdk8s_cdktf_resolver._jsii": [
-            "cdktf-resolver@0.0.82.jsii.tgz"
+            "cdktf-resolver@0.0.9.jsii.tgz"
         ],
         "cdk8s_cdktf_resolver": [
             "py.typed"
         ]
     },
-    "python_requires": "~=3.8",
+    "python_requires": "~=3.7",
     "install_requires": [
-        "cdk8s>=2.68.11, <3.0.0",
-        "cdktf>=0.19.1, <0.20.0",
+        "cdk8s>=2.66.10, <3.0.0",
+        "cdktf>=0.18.2, <0.19.0",
         "constructs>=10.3.0, <11.0.0",
-        "jsii>=1.98.0, <2.0.0",
+        "jsii>=1.90.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
         "Programming Language :: Python :: 3 :: Only",
+        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Typing :: Typed",
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved"
```

### Comparing `cdk8s-cdktf-resolver-0.0.82/src/cdk8s_cdktf_resolver/__init__.py` & `cdk8s-cdktf-resolver-0.0.9/src/cdk8s_cdktf_resolver/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,17 +157,14 @@
     }
  }]
 });
 
 k8sApp.synth();
 ```
 '''
-from pkgutil import extend_path
-__path__ = extend_path(__path__, __name__)
-
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
```

### Comparing `cdk8s-cdktf-resolver-0.0.82/src/cdk8s_cdktf_resolver.egg-info/PKG-INFO` & `cdk8s-cdktf-resolver-0.0.9/src/cdk8s_cdktf_resolver.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: cdk8s-cdktf-resolver
-Version: 0.0.82
+Version: 0.0.9
 Summary: @cdk8s/cdktf-resolver
 Home-page: https://github.com/cdk8s-team/cdk8s-cdktf-resolver.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdk8s-team/cdk8s-cdktf-resolver.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
-Requires-Python: ~=3.8
+Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CDK For Terraform Resolver
 
 The `CdkTfResolver` is able to resolve any [`TerraformOutput`](https://developer.hashicorp.com/terraform/cdktf/concepts/variables-and-outputs#output-values)
 defined by your CDKTF application. In this example, we create an S3 `Bucket` with the CDKTF, and pass its (deploy time generated)
```

