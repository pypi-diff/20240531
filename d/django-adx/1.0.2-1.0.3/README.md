# Comparing `tmp/django_adx-1.0.2.tar.gz` & `tmp/django_adx-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_adx-1.0.2.tar", last modified: Mon May 27 07:54:21 2024, max compression
+gzip compressed data, was "django_adx-1.0.3.tar", last modified: Fri May 31 14:38:24 2024, max compression
```

## Comparing `django_adx-1.0.2.tar` & `django_adx-1.0.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.582677 django_adx-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-27 07:54:13.000000 django_adx-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-05-27 07:54:13.000000 django_adx-1.0.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     6977 2024-05-27 07:54:21.582677 django_adx-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6002 2024-05-27 07:54:13.000000 django_adx-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.578677 django_adx-1.0.2/django_adx/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 07:54:13.000000 django_adx-1.0.2/django_adx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.582677 django_adx-1.0.2/django_adx/builders/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-27 07:54:13.000000 django_adx-1.0.2/django_adx/builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12941 2024-05-27 07:54:13.000000 django_adx-1.0.2/django_adx/builders/adx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.582677 django_adx-1.0.2/django_adx/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:13.000000 django_adx-1.0.2/django_adx/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.582677 django_adx-1.0.2/django_adx/models/adx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:13.000000 django_adx-1.0.2/django_adx/models/adx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-27 07:54:13.000000 django_adx-1.0.2/django_adx/models/adx/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-27 07:54:13.000000 django_adx-1.0.2/django_adx/models/adx/definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-05-27 07:54:13.000000 django_adx-1.0.2/django_adx/models/adx/time_period.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.582677 django_adx-1.0.2/django_adx/models/dhis2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:13.000000 django_adx-1.0.2/django_adx/models/dhis2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-27 07:54:13.000000 django_adx-1.0.2/django_adx/models/dhis2/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     5882 2024-05-27 07:54:13.000000 django_adx-1.0.2/django_adx/models/dhis2/enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     5425 2024-05-27 07:54:13.000000 django_adx-1.0.2/django_adx/models/dhis2/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-27 07:54:13.000000 django_adx-1.0.2/django_adx/models/dhis2/program.py
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-27 07:54:13.000000 django_adx-1.0.2/django_adx/models/dhis2/type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.582677 django_adx-1.0.2/django_adx/serializers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:13.000000 django_adx-1.0.2/django_adx/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-05-27 07:54:13.000000 django_adx-1.0.2/django_adx/serializers/adx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.582677 django_adx-1.0.2/django_adx/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:13.000000 django_adx-1.0.2/django_adx/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7077 2024-05-27 07:54:13.000000 django_adx-1.0.2/django_adx/services/adx_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-05-27 07:54:13.000000 django_adx-1.0.2/django_adx/services/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-05-27 07:54:13.000000 django_adx-1.0.2/django_adx/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.582677 django_adx-1.0.2/django_adx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6977 2024-05-27 07:54:21.000000 django_adx-1.0.2/django_adx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-27 07:54:21.000000 django_adx-1.0.2/django_adx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 07:54:21.000000 django_adx-1.0.2/django_adx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-27 07:54:21.000000 django_adx-1.0.2/django_adx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-27 07:54:21.000000 django_adx-1.0.2/django_adx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 07:54:21.582677 django_adx-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-27 07:54:21.000000 django_adx-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:38:24.771833 django_adx-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-31 14:38:17.000000 django_adx-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-05-31 14:38:17.000000 django_adx-1.0.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7002 2024-05-31 14:38:24.771833 django_adx-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6002 2024-05-31 14:38:17.000000 django_adx-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:38:24.767833 django_adx-1.0.3/django_adx/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 14:38:17.000000 django_adx-1.0.3/django_adx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:38:24.767833 django_adx-1.0.3/django_adx/builders/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-31 14:38:17.000000 django_adx-1.0.3/django_adx/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12941 2024-05-31 14:38:17.000000 django_adx-1.0.3/django_adx/builders/adx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:38:24.767833 django_adx-1.0.3/django_adx/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 14:38:17.000000 django_adx-1.0.3/django_adx/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:38:24.767833 django_adx-1.0.3/django_adx/models/adx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 14:38:17.000000 django_adx-1.0.3/django_adx/models/adx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-31 14:38:17.000000 django_adx-1.0.3/django_adx/models/adx/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-31 14:38:17.000000 django_adx-1.0.3/django_adx/models/adx/definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-05-31 14:38:17.000000 django_adx-1.0.3/django_adx/models/adx/time_period.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:38:24.767833 django_adx-1.0.3/django_adx/models/dhis2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 14:38:17.000000 django_adx-1.0.3/django_adx/models/dhis2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-31 14:38:17.000000 django_adx-1.0.3/django_adx/models/dhis2/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5882 2024-05-31 14:38:17.000000 django_adx-1.0.3/django_adx/models/dhis2/enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5425 2024-05-31 14:38:17.000000 django_adx-1.0.3/django_adx/models/dhis2/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-31 14:38:17.000000 django_adx-1.0.3/django_adx/models/dhis2/program.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-31 14:38:17.000000 django_adx-1.0.3/django_adx/models/dhis2/type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:38:24.767833 django_adx-1.0.3/django_adx/serializers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 14:38:17.000000 django_adx-1.0.3/django_adx/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-05-31 14:38:17.000000 django_adx-1.0.3/django_adx/serializers/adx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:38:24.771833 django_adx-1.0.3/django_adx/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 14:38:17.000000 django_adx-1.0.3/django_adx/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7077 2024-05-31 14:38:17.000000 django_adx-1.0.3/django_adx/services/adx_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-05-31 14:38:17.000000 django_adx-1.0.3/django_adx/services/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-05-31 14:38:17.000000 django_adx-1.0.3/django_adx/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:38:24.771833 django_adx-1.0.3/django_adx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7002 2024-05-31 14:38:24.000000 django_adx-1.0.3/django_adx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-31 14:38:24.000000 django_adx-1.0.3/django_adx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 14:38:24.000000 django_adx-1.0.3/django_adx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-31 14:38:24.000000 django_adx-1.0.3/django_adx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-31 14:38:24.000000 django_adx-1.0.3/django_adx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 14:38:24.771833 django_adx-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-31 14:38:24.000000 django_adx-1.0.3/setup.py
```

### Comparing `django_adx-1.0.2/LICENSE` & `django_adx-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django_adx-1.0.2/LICENSE.md` & `django_adx-1.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django_adx-1.0.2/PKG-INFO` & `django_adx-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-adx
-Version: 1.0.2
+Version: 1.0.3
 Home-page: https://github.com/delcroip/django-adx
 Author: Patrick Delcroix
 Author-email: patrick.delcroix@swisstph.ch
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.1
@@ -22,14 +22,15 @@
 Requires-Dist: django
 Requires-Dist: dhis2.py
 Requires-Dist: pydantic
 Requires-Dist: dict2obj
 Requires-Dist: isodate
 Requires-Dist: python-dateutil
 Requires-Dist: numpy
+Requires-Dist: packaging
 
 # django-adx
 
 
 This module enable creating aggregated data on multiple dimensions (CUBE)
 
 It was initially build as part of openimis-be-dhis2_etl_py made by Damian Borowiecki @dborowiecki (models) and Kamil Malinowski @Malinowskikam (dev) and Patrick Delcroix (desing)
```

### Comparing `django_adx-1.0.2/README.md` & `django_adx-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `django_adx-1.0.2/django_adx/builders/adx.py` & `django_adx-1.0.3/django_adx/builders/adx.py`

 * *Files identical despite different names*

### Comparing `django_adx-1.0.2/django_adx/models/adx/data.py` & `django_adx-1.0.3/django_adx/models/adx/data.py`

 * *Files identical despite different names*

### Comparing `django_adx-1.0.2/django_adx/models/adx/definition.py` & `django_adx-1.0.3/django_adx/models/adx/definition.py`

 * *Files identical despite different names*

### Comparing `django_adx-1.0.2/django_adx/models/adx/time_period.py` & `django_adx-1.0.3/django_adx/models/adx/time_period.py`

 * *Files identical despite different names*

### Comparing `django_adx-1.0.2/django_adx/models/dhis2/dataset.py` & `django_adx-1.0.3/django_adx/models/dhis2/dataset.py`

 * *Files identical despite different names*

### Comparing `django_adx-1.0.2/django_adx/models/dhis2/enum.py` & `django_adx-1.0.3/django_adx/models/dhis2/enum.py`

 * *Files identical despite different names*

### Comparing `django_adx-1.0.2/django_adx/models/dhis2/metadata.py` & `django_adx-1.0.3/django_adx/models/dhis2/metadata.py`

 * *Files identical despite different names*

### Comparing `django_adx-1.0.2/django_adx/models/dhis2/program.py` & `django_adx-1.0.3/django_adx/models/dhis2/program.py`

 * *Files identical despite different names*

### Comparing `django_adx-1.0.2/django_adx/models/dhis2/type.py` & `django_adx-1.0.3/django_adx/models/dhis2/type.py`

 * *Files identical despite different names*

### Comparing `django_adx-1.0.2/django_adx/serializers/adx.py` & `django_adx-1.0.3/django_adx/serializers/adx.py`

 * *Files identical despite different names*

### Comparing `django_adx-1.0.2/django_adx/services/adx_metadata.py` & `django_adx-1.0.3/django_adx/services/adx_metadata.py`

 * *Files identical despite different names*

### Comparing `django_adx-1.0.2/django_adx/services/utils.py` & `django_adx-1.0.3/django_adx/services/utils.py`

 * *Files identical despite different names*

### Comparing `django_adx-1.0.2/django_adx/utils.py` & `django_adx-1.0.3/django_adx/utils.py`

 * *Files identical despite different names*

### Comparing `django_adx-1.0.2/django_adx.egg-info/PKG-INFO` & `django_adx-1.0.3/django_adx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-adx
-Version: 1.0.2
+Version: 1.0.3
 Home-page: https://github.com/delcroip/django-adx
 Author: Patrick Delcroix
 Author-email: patrick.delcroix@swisstph.ch
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.1
@@ -22,14 +22,15 @@
 Requires-Dist: django
 Requires-Dist: dhis2.py
 Requires-Dist: pydantic
 Requires-Dist: dict2obj
 Requires-Dist: isodate
 Requires-Dist: python-dateutil
 Requires-Dist: numpy
+Requires-Dist: packaging
 
 # django-adx
 
 
 This module enable creating aggregated data on multiple dimensions (CUBE)
 
 It was initially build as part of openimis-be-dhis2_etl_py made by Damian Borowiecki @dborowiecki (models) and Kamil Malinowski @Malinowskikam (dev) and Patrick Delcroix (desing)
```

### Comparing `django_adx-1.0.2/django_adx.egg-info/SOURCES.txt` & `django_adx-1.0.3/django_adx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_adx-1.0.2/setup.py` & `django_adx-1.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='django-adx',
-    version='v1.0.2',
+    version='v1.0.3',
     packages=find_packages(),
     include_package_data=True,
     license='GNU AGPL v3',
     # other arguments omitted
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://github.com/delcroip/django-adx',
@@ -22,15 +22,16 @@
     install_requires=[
         'django',
         'dhis2.py',
         'pydantic',
         'dict2obj',
         'isodate',
         'python-dateutil',
-        'numpy'
+        'numpy',
+        'packaging'
     ],   
     classifiers=[
         'Environment :: Web Environment',
         'Framework :: Django',
         'Framework :: Django :: 3.1',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: GNU Affero General Public License v3',
```

