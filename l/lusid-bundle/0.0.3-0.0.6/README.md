# Comparing `tmp/lusid_bundle-0.0.3.tar.gz` & `tmp/lusid_bundle-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lusid_bundle-0.0.3.tar", last modified: Fri May 31 19:11:54 2024, max compression
+gzip compressed data, was "lusid_bundle-0.0.6.tar", last modified: Fri May 31 19:17:12 2024, max compression
```

## Comparing `lusid_bundle-0.0.3.tar` & `lusid_bundle-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 19:11:54.759647 lusid_bundle-0.0.3/
--rw-rw-rw-   0 root         (0) root         (0)     1062 2024-05-31 19:11:50.000000 lusid_bundle-0.0.3/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-31 19:11:50.000000 lusid_bundle-0.0.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2747 2024-05-31 19:11:54.759647 lusid_bundle-0.0.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2087 2024-05-31 19:11:50.000000 lusid_bundle-0.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 19:11:54.759647 lusid_bundle-0.0.3/lusid_bundle.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2747 2024-05-31 19:11:54.000000 lusid_bundle-0.0.3/lusid_bundle.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      217 2024-05-31 19:11:54.000000 lusid_bundle-0.0.3/lusid_bundle.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-31 19:11:54.000000 lusid_bundle-0.0.3/lusid_bundle.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      479 2024-05-31 19:11:54.000000 lusid_bundle-0.0.3/lusid_bundle.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-31 19:11:54.000000 lusid_bundle-0.0.3/lusid_bundle.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-31 19:11:54.759647 lusid_bundle-0.0.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1375 2024-05-31 19:11:50.000000 lusid_bundle-0.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 19:17:12.420631 lusid_bundle-0.0.6/
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2024-05-31 19:17:08.000000 lusid_bundle-0.0.6/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-31 19:17:08.000000 lusid_bundle-0.0.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2747 2024-05-31 19:17:12.419630 lusid_bundle-0.0.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2087 2024-05-31 19:17:08.000000 lusid_bundle-0.0.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 19:17:12.419630 lusid_bundle-0.0.6/lusid_bundle.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2747 2024-05-31 19:17:12.000000 lusid_bundle-0.0.6/lusid_bundle.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      217 2024-05-31 19:17:12.000000 lusid_bundle-0.0.6/lusid_bundle.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-31 19:17:12.000000 lusid_bundle-0.0.6/lusid_bundle.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      479 2024-05-31 19:17:12.000000 lusid_bundle-0.0.6/lusid_bundle.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-31 19:17:12.000000 lusid_bundle-0.0.6/lusid_bundle.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-31 19:17:12.420631 lusid_bundle-0.0.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1375 2024-05-31 19:17:08.000000 lusid_bundle-0.0.6/setup.py
```

### Comparing `lusid_bundle-0.0.3/LICENSE` & `lusid_bundle-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lusid_bundle-0.0.3/PKG-INFO` & `lusid_bundle-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lusid_bundle
-Version: 0.0.3
+Version: 0.0.6
 Summary: lusid-bundle is a python package that makes it quick and easy to install all of the Lusid and Luminesce sdks and dependencies.
 Home-page: https://gitlab.com/orlando.calvo1/lusid-bundle
 Author: Orlando Calvo
 Author-email: orlando.calvo@finbourne.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `lusid_bundle-0.0.3/README.md` & `lusid_bundle-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `lusid_bundle-0.0.3/lusid_bundle.egg-info/PKG-INFO` & `lusid_bundle-0.0.6/lusid_bundle.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lusid-bundle
-Version: 0.0.3
+Version: 0.0.6
 Summary: lusid-bundle is a python package that makes it quick and easy to install all of the Lusid and Luminesce sdks and dependencies.
 Home-page: https://gitlab.com/orlando.calvo1/lusid-bundle
 Author: Orlando Calvo
 Author-email: orlando.calvo@finbourne.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `lusid_bundle-0.0.3/setup.py` & `lusid_bundle-0.0.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 ]
 
 
 
 
 setup(
     name='lusid_bundle',
-    version='0.0.3',
+    version='0.0.6',
     install_requires=requirements,
     description='lusid-bundle is a python package that makes it quick and easy to install all of the Lusid and Luminesce sdks and dependencies.',
     long_description=open('README.md').read(),
     include_package_data=True,  
     long_description_content_type='text/markdown',
     author='Orlando Calvo',
     author_email='orlando.calvo@finbourne.com',
```

