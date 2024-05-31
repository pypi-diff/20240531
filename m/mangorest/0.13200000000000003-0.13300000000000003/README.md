# Comparing `tmp/mangorest-0.13200000000000003.tar.gz` & `tmp/mangorest-0.13300000000000003.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mangorest-0.13200000000000003.tar", last modified: Fri May 10 18:49:31 2024, max compression
+gzip compressed data, was "mangorest-0.13300000000000003.tar", last modified: Fri May 31 04:34:22 2024, max compression
```

## Comparing `mangorest-0.13200000000000003.tar` & `mangorest-0.13300000000000003.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 snarayan   (501) wheel        (0)        0 2024-05-10 18:49:31.037272 mangorest-0.13200000000000003/
--rw-r--r--   0 snarayan   (501) wheel        (0)    11357 2020-09-20 16:46:27.000000 mangorest-0.13200000000000003/LICENSE
--rw-r--r--   0 snarayan   (501) wheel        (0)      820 2024-05-10 18:49:31.036862 mangorest-0.13200000000000003/PKG-INFO
--rw-r--r--   0 snarayan   (501) wheel        (0)     2449 2022-07-26 01:13:10.000000 mangorest-0.13200000000000003/README.md
-drwxr-xr-x   0 snarayan   (501) wheel        (0)        0 2024-05-10 18:49:31.033138 mangorest-0.13200000000000003/mangorest/
--rw-r--r--   0 snarayan   (501) wheel        (0)        0 2020-09-20 16:51:18.000000 mangorest-0.13200000000000003/mangorest/__init__.py
--rw-r--r--   0 snarayan   (501) wheel        (0)     1310 2020-09-26 18:35:34.000000 mangorest-0.13200000000000003/mangorest/dirlist.py
--rwxr-xr-x   0 snarayan   (501) wheel        (0)    14814 2024-05-10 18:48:38.000000 mangorest-0.13200000000000003/mangorest/mango.py
--rw-r--r--   0 snarayan   (501) wheel        (0)       27 2024-05-10 18:49:30.000000 mangorest-0.13200000000000003/mangorest/version.txt
-drwxr-xr-x   0 snarayan   (501) wheel        (0)        0 2024-05-10 18:49:31.036316 mangorest-0.13200000000000003/mangorest.egg-info/
--rw-r--r--   0 snarayan   (501) wheel        (0)      820 2024-05-10 18:49:30.000000 mangorest-0.13200000000000003/mangorest.egg-info/PKG-INFO
--rw-r--r--   0 snarayan   (501) wheel        (0)      319 2024-05-10 18:49:30.000000 mangorest-0.13200000000000003/mangorest.egg-info/SOURCES.txt
--rw-r--r--   0 snarayan   (501) wheel        (0)        1 2024-05-10 18:49:30.000000 mangorest-0.13200000000000003/mangorest.egg-info/dependency_links.txt
--rw-r--r--   0 snarayan   (501) wheel        (0)        1 2020-09-26 14:25:00.000000 mangorest-0.13200000000000003/mangorest.egg-info/not-zip-safe
--rw-r--r--   0 snarayan   (501) wheel        (0)        7 2024-05-10 18:49:30.000000 mangorest-0.13200000000000003/mangorest.egg-info/requires.txt
--rw-r--r--   0 snarayan   (501) wheel        (0)       10 2024-05-10 18:49:30.000000 mangorest-0.13200000000000003/mangorest.egg-info/top_level.txt
--rw-r--r--   0 snarayan   (501) wheel        (0)       38 2024-05-10 18:49:31.037369 mangorest-0.13200000000000003/setup.cfg
--rw-r--r--   0 snarayan   (501) wheel        (0)     1698 2024-05-10 18:49:30.000000 mangorest-0.13200000000000003/setup.py
-drwxr-xr-x   0 snarayan   (501) wheel        (0)        0 2024-05-10 18:49:31.035379 mangorest-0.13200000000000003/test/
--rwxrwxr-x   0 snarayan   (501) wheel        (0)      653 2022-07-20 11:34:26.000000 mangorest-0.13200000000000003/test/test.py
+drwxr-xr-x   0 snarayan   (501) wheel        (0)        0 2024-05-31 04:34:22.784340 mangorest-0.13300000000000003/
+-rw-r--r--   0 snarayan   (501) wheel        (0)    11357 2020-09-20 16:46:27.000000 mangorest-0.13300000000000003/LICENSE
+-rw-r--r--   0 snarayan   (501) wheel        (0)      820 2024-05-31 04:34:22.783867 mangorest-0.13300000000000003/PKG-INFO
+-rw-r--r--   0 snarayan   (501) wheel        (0)     2449 2022-07-26 01:13:10.000000 mangorest-0.13300000000000003/README.md
+drwxr-xr-x   0 snarayan   (501) wheel        (0)        0 2024-05-31 04:34:22.779704 mangorest-0.13300000000000003/mangorest/
+-rw-r--r--   0 snarayan   (501) wheel        (0)        0 2020-09-20 16:51:18.000000 mangorest-0.13300000000000003/mangorest/__init__.py
+-rw-r--r--   0 snarayan   (501) wheel        (0)     1310 2020-09-26 18:35:34.000000 mangorest-0.13300000000000003/mangorest/dirlist.py
+-rwxr-xr-x   0 snarayan   (501) wheel        (0)    14870 2024-05-24 04:14:14.000000 mangorest-0.13300000000000003/mangorest/mango.py
+-rw-r--r--   0 snarayan   (501) wheel        (0)       27 2024-05-31 04:34:22.000000 mangorest-0.13300000000000003/mangorest/version.txt
+drwxr-xr-x   0 snarayan   (501) wheel        (0)        0 2024-05-31 04:34:22.783330 mangorest-0.13300000000000003/mangorest.egg-info/
+-rw-r--r--   0 snarayan   (501) wheel        (0)      820 2024-05-31 04:34:22.000000 mangorest-0.13300000000000003/mangorest.egg-info/PKG-INFO
+-rw-r--r--   0 snarayan   (501) wheel        (0)      319 2024-05-31 04:34:22.000000 mangorest-0.13300000000000003/mangorest.egg-info/SOURCES.txt
+-rw-r--r--   0 snarayan   (501) wheel        (0)        1 2024-05-31 04:34:22.000000 mangorest-0.13300000000000003/mangorest.egg-info/dependency_links.txt
+-rw-r--r--   0 snarayan   (501) wheel        (0)        1 2020-09-26 14:25:00.000000 mangorest-0.13300000000000003/mangorest.egg-info/not-zip-safe
+-rw-r--r--   0 snarayan   (501) wheel        (0)        7 2024-05-31 04:34:22.000000 mangorest-0.13300000000000003/mangorest.egg-info/requires.txt
+-rw-r--r--   0 snarayan   (501) wheel        (0)       10 2024-05-31 04:34:22.000000 mangorest-0.13300000000000003/mangorest.egg-info/top_level.txt
+-rw-r--r--   0 snarayan   (501) wheel        (0)       38 2024-05-31 04:34:22.784568 mangorest-0.13300000000000003/setup.cfg
+-rw-r--r--   0 snarayan   (501) wheel        (0)     1698 2024-05-31 04:34:22.000000 mangorest-0.13300000000000003/setup.py
+drwxr-xr-x   0 snarayan   (501) wheel        (0)        0 2024-05-31 04:34:22.782533 mangorest-0.13300000000000003/test/
+-rwxrwxr-x   0 snarayan   (501) wheel        (0)      653 2022-07-20 11:34:26.000000 mangorest-0.13300000000000003/test/test.py
```

### Comparing `mangorest-0.13200000000000003/LICENSE` & `mangorest-0.13300000000000003/LICENSE`

 * *Files identical despite different names*

### Comparing `mangorest-0.13200000000000003/PKG-INFO` & `mangorest-0.13300000000000003/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mangorest
-Version: 0.13200000000000003
+Version: 0.13300000000000003
 Summary: Very simple quick way to deploy Django Webservices
 Home-page: https://github.com/meyers007/mangorest.git
 Author: Wan Bae, Seattle University
 Author-email: baew@seattleu.edu
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `mangorest-0.13200000000000003/README.md` & `mangorest-0.13300000000000003/README.md`

 * *Files identical despite different names*

### Comparing `mangorest-0.13200000000000003/mangorest/dirlist.py` & `mangorest-0.13300000000000003/mangorest/dirlist.py`

 * *Files identical despite different names*

### Comparing `mangorest-0.13200000000000003/mangorest/mango.py` & `mangorest-0.13300000000000003/mangorest/mango.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,16 @@
            L    {getlist} </pre> '''
     return HttpResponse(ret);
 #--------------------------------------------------------------------------------
 class myEncoder(DjangoJSONEncoder):
     def default(self, obj):
         if isinstance(obj, np.int64):
             return int(obj)
-        elif isinstance(obj, pd._libs.tslibs.timestamps.Timestamp):
+        elif isinstance(obj, pd._libs.tslibs.timestamps.Timestamp) or \
+                isinstance(obj, datetime.datetime):
             return str(obj)
         else:
             return super(DjangoJSONEncoder, self).default(obj)
 #--------------------------------------------------------------------------------
 def getparms(request):
     par = dict(request.GET)
     par.update(request.POST)
```

### Comparing `mangorest-0.13200000000000003/mangorest.egg-info/PKG-INFO` & `mangorest-0.13300000000000003/mangorest.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mangorest
-Version: 0.13200000000000003
+Version: 0.13300000000000003
 Summary: Very simple quick way to deploy Django Webservices
 Home-page: https://github.com/meyers007/mangorest.git
 Author: Wan Bae, Seattle University
 Author-email: baew@seattleu.edu
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `mangorest-0.13200000000000003/setup.py` & `mangorest-0.13300000000000003/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version=0.13200000000000003
+version=0.13300000000000003
 
 setup(name='mangorest', 
       version=str(version), 
       description='Very simple quick way to deploy Django Webservices',
       url='https://github.com/meyers007/mangorest.git',
       author='Wan Bae, Seattle University',
       author_email='baew@seattleu.edu',
```

### Comparing `mangorest-0.13200000000000003/test/test.py` & `mangorest-0.13300000000000003/test/test.py`

 * *Files identical despite different names*

