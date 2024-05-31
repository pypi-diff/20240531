# Comparing `tmp/lusid_bundle-0.0.1.tar.gz` & `tmp/lusid_bundle-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lusid_bundle-0.0.1.tar", last modified: Fri May 31 15:09:36 2024, max compression
+gzip compressed data, was "lusid_bundle-0.0.2.tar", last modified: Fri May 31 17:00:57 2024, max compression
```

## Comparing `lusid_bundle-0.0.1.tar` & `lusid_bundle-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 15:09:36.148419 lusid_bundle-0.0.1/
--rw-rw-rw-   0 root         (0) root         (0)     1062 2024-05-31 15:09:33.000000 lusid_bundle-0.0.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-31 15:09:33.000000 lusid_bundle-0.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2751 2024-05-31 15:09:36.148419 lusid_bundle-0.0.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2091 2024-05-31 15:09:33.000000 lusid_bundle-0.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 15:09:36.147419 lusid_bundle-0.0.1/lusid_bundle.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2751 2024-05-31 15:09:36.000000 lusid_bundle-0.0.1/lusid_bundle.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      217 2024-05-31 15:09:36.000000 lusid_bundle-0.0.1/lusid_bundle.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-31 15:09:36.000000 lusid_bundle-0.0.1/lusid_bundle.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      479 2024-05-31 15:09:36.000000 lusid_bundle-0.0.1/lusid_bundle.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-31 15:09:36.000000 lusid_bundle-0.0.1/lusid_bundle.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-31 15:09:36.148419 lusid_bundle-0.0.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1375 2024-05-31 15:09:33.000000 lusid_bundle-0.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 17:00:57.623981 lusid_bundle-0.0.2/
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2024-05-31 17:00:53.000000 lusid_bundle-0.0.2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-31 17:00:53.000000 lusid_bundle-0.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2751 2024-05-31 17:00:57.622981 lusid_bundle-0.0.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2091 2024-05-31 17:00:53.000000 lusid_bundle-0.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 17:00:57.622981 lusid_bundle-0.0.2/lusid_bundle.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2751 2024-05-31 17:00:57.000000 lusid_bundle-0.0.2/lusid_bundle.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      217 2024-05-31 17:00:57.000000 lusid_bundle-0.0.2/lusid_bundle.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-31 17:00:57.000000 lusid_bundle-0.0.2/lusid_bundle.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      479 2024-05-31 17:00:57.000000 lusid_bundle-0.0.2/lusid_bundle.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-31 17:00:57.000000 lusid_bundle-0.0.2/lusid_bundle.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-31 17:00:57.623981 lusid_bundle-0.0.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1375 2024-05-31 17:00:53.000000 lusid_bundle-0.0.2/setup.py
```

### Comparing `lusid_bundle-0.0.1/LICENSE` & `lusid_bundle-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lusid_bundle-0.0.1/PKG-INFO` & `lusid_bundle-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lusid_bundle
-Version: 0.0.1
+Version: 0.0.2
 Summary: lusid-bundle is a python package that makes it quick and easy to install all of the Lusid and Luminesce sdks and dependencies.
 Home-page: https://gitlab.com/orlando.calvo1/lusid-bundle
 Author: Orlando Calvo
 Author-email: orlando.calvo@finbourne.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `lusid_bundle-0.0.1/README.md` & `lusid_bundle-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `lusid_bundle-0.0.1/lusid_bundle.egg-info/PKG-INFO` & `lusid_bundle-0.0.2/lusid_bundle.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lusid-bundle
-Version: 0.0.1
+Version: 0.0.2
 Summary: lusid-bundle is a python package that makes it quick and easy to install all of the Lusid and Luminesce sdks and dependencies.
 Home-page: https://gitlab.com/orlando.calvo1/lusid-bundle
 Author: Orlando Calvo
 Author-email: orlando.calvo@finbourne.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `lusid_bundle-0.0.1/setup.py` & `lusid_bundle-0.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 ]
 
 
 
 
 setup(
     name='lusid_bundle',
-    version='0.0.1',
+    version='0.0.2',
     install_requires=requirements,
     description='lusid-bundle is a python package that makes it quick and easy to install all of the Lusid and Luminesce sdks and dependencies.',
     long_description=open('README.md').read(),
     include_package_data=True,  
     long_description_content_type='text/markdown',
     author='Orlando Calvo',
     author_email='orlando.calvo@finbourne.com',
```

