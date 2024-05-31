# Comparing `tmp/lusid_bundle-0.0.2.tar.gz` & `tmp/lusid_bundle-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lusid_bundle-0.0.2.tar", last modified: Fri May 31 17:00:57 2024, max compression
+gzip compressed data, was "lusid_bundle-0.0.3.tar", last modified: Fri May 31 19:11:54 2024, max compression
```

## Comparing `lusid_bundle-0.0.2.tar` & `lusid_bundle-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 17:00:57.623981 lusid_bundle-0.0.2/
--rw-rw-rw-   0 root         (0) root         (0)     1062 2024-05-31 17:00:53.000000 lusid_bundle-0.0.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-31 17:00:53.000000 lusid_bundle-0.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2751 2024-05-31 17:00:57.622981 lusid_bundle-0.0.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2091 2024-05-31 17:00:53.000000 lusid_bundle-0.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 17:00:57.622981 lusid_bundle-0.0.2/lusid_bundle.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2751 2024-05-31 17:00:57.000000 lusid_bundle-0.0.2/lusid_bundle.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      217 2024-05-31 17:00:57.000000 lusid_bundle-0.0.2/lusid_bundle.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-31 17:00:57.000000 lusid_bundle-0.0.2/lusid_bundle.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      479 2024-05-31 17:00:57.000000 lusid_bundle-0.0.2/lusid_bundle.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-31 17:00:57.000000 lusid_bundle-0.0.2/lusid_bundle.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-31 17:00:57.623981 lusid_bundle-0.0.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1375 2024-05-31 17:00:53.000000 lusid_bundle-0.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 19:11:54.759647 lusid_bundle-0.0.3/
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2024-05-31 19:11:50.000000 lusid_bundle-0.0.3/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-31 19:11:50.000000 lusid_bundle-0.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2747 2024-05-31 19:11:54.759647 lusid_bundle-0.0.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2087 2024-05-31 19:11:50.000000 lusid_bundle-0.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 19:11:54.759647 lusid_bundle-0.0.3/lusid_bundle.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2747 2024-05-31 19:11:54.000000 lusid_bundle-0.0.3/lusid_bundle.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      217 2024-05-31 19:11:54.000000 lusid_bundle-0.0.3/lusid_bundle.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-31 19:11:54.000000 lusid_bundle-0.0.3/lusid_bundle.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      479 2024-05-31 19:11:54.000000 lusid_bundle-0.0.3/lusid_bundle.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-31 19:11:54.000000 lusid_bundle-0.0.3/lusid_bundle.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-31 19:11:54.759647 lusid_bundle-0.0.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1375 2024-05-31 19:11:50.000000 lusid_bundle-0.0.3/setup.py
```

### Comparing `lusid_bundle-0.0.2/LICENSE` & `lusid_bundle-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lusid_bundle-0.0.2/PKG-INFO` & `lusid_bundle-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lusid_bundle
-Version: 0.0.2
+Version: 0.0.3
 Summary: lusid-bundle is a python package that makes it quick and easy to install all of the Lusid and Luminesce sdks and dependencies.
 Home-page: https://gitlab.com/orlando.calvo1/lusid-bundle
 Author: Orlando Calvo
 Author-email: orlando.calvo@finbourne.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -12,16 +12,16 @@
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
-[![pypi](https://img.shields.io/pypi/v/lusid-express)](https://pypi.org/project/lusid-express/)
-[![python](https://img.shields.io/pypi/pyversions/lusid-express.svg)](https://pypi.org/project/lusid-express/)
+[![pypi](https://img.shields.io/pypi/v/lusid-bundle)](https://pypi.org/project/lusid-bundle/)
+[![python](https://img.shields.io/pypi/pyversions/lusid-bundle.svg)](https://pypi.org/project/lusid-bundle/)
 
 # 1. lusid-bundle
 #####  *`lusid-bundle` is a python package that makes it quick and easy to get started using Lusid and Luminesce. It bundles all packages needed to get started.*
```

### Comparing `lusid_bundle-0.0.2/README.md` & `lusid_bundle-0.0.3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
-[![pypi](https://img.shields.io/pypi/v/lusid-express)](https://pypi.org/project/lusid-express/)
-[![python](https://img.shields.io/pypi/pyversions/lusid-express.svg)](https://pypi.org/project/lusid-express/)
+[![pypi](https://img.shields.io/pypi/v/lusid-bundle)](https://pypi.org/project/lusid-bundle/)
+[![python](https://img.shields.io/pypi/pyversions/lusid-bundle.svg)](https://pypi.org/project/lusid-bundle/)
 
 # 1. lusid-bundle
 #####  *`lusid-bundle` is a python package that makes it quick and easy to get started using Lusid and Luminesce. It bundles all packages needed to get started.*
```

### Comparing `lusid_bundle-0.0.2/lusid_bundle.egg-info/PKG-INFO` & `lusid_bundle-0.0.3/lusid_bundle.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lusid-bundle
-Version: 0.0.2
+Version: 0.0.3
 Summary: lusid-bundle is a python package that makes it quick and easy to install all of the Lusid and Luminesce sdks and dependencies.
 Home-page: https://gitlab.com/orlando.calvo1/lusid-bundle
 Author: Orlando Calvo
 Author-email: orlando.calvo@finbourne.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -12,16 +12,16 @@
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
-[![pypi](https://img.shields.io/pypi/v/lusid-express)](https://pypi.org/project/lusid-express/)
-[![python](https://img.shields.io/pypi/pyversions/lusid-express.svg)](https://pypi.org/project/lusid-express/)
+[![pypi](https://img.shields.io/pypi/v/lusid-bundle)](https://pypi.org/project/lusid-bundle/)
+[![python](https://img.shields.io/pypi/pyversions/lusid-bundle.svg)](https://pypi.org/project/lusid-bundle/)
 
 # 1. lusid-bundle
 #####  *`lusid-bundle` is a python package that makes it quick and easy to get started using Lusid and Luminesce. It bundles all packages needed to get started.*
```

### Comparing `lusid_bundle-0.0.2/setup.py` & `lusid_bundle-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 ]
 
 
 
 
 setup(
     name='lusid_bundle',
-    version='0.0.2',
+    version='0.0.3',
     install_requires=requirements,
     description='lusid-bundle is a python package that makes it quick and easy to install all of the Lusid and Luminesce sdks and dependencies.',
     long_description=open('README.md').read(),
     include_package_data=True,  
     long_description_content_type='text/markdown',
     author='Orlando Calvo',
     author_email='orlando.calvo@finbourne.com',
```

