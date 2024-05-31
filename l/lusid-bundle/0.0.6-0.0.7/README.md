# Comparing `tmp/lusid_bundle-0.0.6.tar.gz` & `tmp/lusid_bundle-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lusid_bundle-0.0.6.tar", last modified: Fri May 31 19:17:12 2024, max compression
+gzip compressed data, was "lusid_bundle-0.0.7.tar", last modified: Fri May 31 19:19:15 2024, max compression
```

## Comparing `lusid_bundle-0.0.6.tar` & `lusid_bundle-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 19:17:12.420631 lusid_bundle-0.0.6/
--rw-rw-rw-   0 root         (0) root         (0)     1062 2024-05-31 19:17:08.000000 lusid_bundle-0.0.6/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-31 19:17:08.000000 lusid_bundle-0.0.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2747 2024-05-31 19:17:12.419630 lusid_bundle-0.0.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2087 2024-05-31 19:17:08.000000 lusid_bundle-0.0.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 19:17:12.419630 lusid_bundle-0.0.6/lusid_bundle.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2747 2024-05-31 19:17:12.000000 lusid_bundle-0.0.6/lusid_bundle.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      217 2024-05-31 19:17:12.000000 lusid_bundle-0.0.6/lusid_bundle.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-31 19:17:12.000000 lusid_bundle-0.0.6/lusid_bundle.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      479 2024-05-31 19:17:12.000000 lusid_bundle-0.0.6/lusid_bundle.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-31 19:17:12.000000 lusid_bundle-0.0.6/lusid_bundle.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-31 19:17:12.420631 lusid_bundle-0.0.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1375 2024-05-31 19:17:08.000000 lusid_bundle-0.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 19:19:15.784268 lusid_bundle-0.0.7/
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2024-05-31 19:19:12.000000 lusid_bundle-0.0.7/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-31 19:19:12.000000 lusid_bundle-0.0.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2747 2024-05-31 19:19:15.784268 lusid_bundle-0.0.7/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2087 2024-05-31 19:19:12.000000 lusid_bundle-0.0.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 19:19:15.783269 lusid_bundle-0.0.7/lusid_bundle.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2747 2024-05-31 19:19:15.000000 lusid_bundle-0.0.7/lusid_bundle.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      217 2024-05-31 19:19:15.000000 lusid_bundle-0.0.7/lusid_bundle.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-31 19:19:15.000000 lusid_bundle-0.0.7/lusid_bundle.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      479 2024-05-31 19:19:15.000000 lusid_bundle-0.0.7/lusid_bundle.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-31 19:19:15.000000 lusid_bundle-0.0.7/lusid_bundle.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-31 19:19:15.784268 lusid_bundle-0.0.7/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1535 2024-05-31 19:19:12.000000 lusid_bundle-0.0.7/setup.py
```

### Comparing `lusid_bundle-0.0.6/LICENSE` & `lusid_bundle-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `lusid_bundle-0.0.6/PKG-INFO` & `lusid_bundle-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lusid_bundle
-Version: 0.0.6
+Version: 0.0.7
 Summary: lusid-bundle is a python package that makes it quick and easy to install all of the Lusid and Luminesce sdks and dependencies.
 Home-page: https://gitlab.com/orlando.calvo1/lusid-bundle
 Author: Orlando Calvo
 Author-email: orlando.calvo@finbourne.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `lusid_bundle-0.0.6/README.md` & `lusid_bundle-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `lusid_bundle-0.0.6/lusid_bundle.egg-info/PKG-INFO` & `lusid_bundle-0.0.7/lusid_bundle.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lusid-bundle
-Version: 0.0.6
+Version: 0.0.7
 Summary: lusid-bundle is a python package that makes it quick and easy to install all of the Lusid and Luminesce sdks and dependencies.
 Home-page: https://gitlab.com/orlando.calvo1/lusid-bundle
 Author: Orlando Calvo
 Author-email: orlando.calvo@finbourne.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `lusid_bundle-0.0.6/setup.py` & `lusid_bundle-0.0.7/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 from setuptools import setup
 
 
 # List of requirements
 requirements = [
-    'pyyaml',
-'luminesce-sdk-preview==1.14.758',
-'lusid-jam==0.1.2',
-'lusid-sdk-preview==1.1.120',
-'fbnlab-preview==0.1.108',
-'finbourne-access-sdk==0.0.3751',
-'finbourne-identity-sdk==0.0.2834',
-'finbourne-insights-sdk-preview==0.0.763',
-'finbourne-sdk-utilities==0.0.10',
-'lusid-configuration-sdk-preview==0.1.514',
-'lusid-drive-sdk-preview==0.1.617',
-'lusid-notifications-sdk-preview==0.1.923',
-'lusid-scheduler-sdk-preview==0.0.829',
-'lusid-workflow-sdk-preview==0.1.810',
-'lusidtools==1.0.14',
-'dve-lumipy-preview==0.1.1075',
+    'pyyaml', # no-bump
+'luminesce-sdk-preview==1.14.758', # no-bump
+'lusid-jam==0.1.2', # no-bump
+'lusid-sdk-preview==1.1.120', # no-bump
+'fbnlab-preview==0.1.108', # no-bump
+'finbourne-access-sdk==0.0.3751', # no-bump
+'finbourne-identity-sdk==0.0.2834', # no-bump
+'finbourne-insights-sdk-preview==0.0.763', # no-bump
+'finbourne-sdk-utilities==0.0.10', # no-bump
+'lusid-configuration-sdk-preview==0.1.514', # no-bump
+'lusid-drive-sdk-preview==0.1.617', # no-bump
+'lusid-notifications-sdk-preview==0.1.923', # no-bump
+'lusid-scheduler-sdk-preview==0.0.829', # no-bump
+'lusid-workflow-sdk-preview==0.1.810', # no-bump
+'lusidtools==1.0.14', # no-bump
+'dve-lumipy-preview==0.1.1075', # no-bump
 
 ]
 
 
 
 
 setup(
     name='lusid_bundle',
-    version='0.0.6',
+    version='0.0.7',
     install_requires=requirements,
     description='lusid-bundle is a python package that makes it quick and easy to install all of the Lusid and Luminesce sdks and dependencies.',
     long_description=open('README.md').read(),
     include_package_data=True,  
     long_description_content_type='text/markdown',
     author='Orlando Calvo',
     author_email='orlando.calvo@finbourne.com',
```

