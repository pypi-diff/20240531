# Comparing `tmp/dlqhandler-0.2.6.tar.gz` & `tmp/dlqhandler-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dlqhandler-0.2.6.tar", last modified: Fri May 31 05:45:08 2024, max compression
+gzip compressed data, was "dlqhandler-0.2.7.tar", last modified: Fri May 31 14:55:57 2024, max compression
```

## Comparing `dlqhandler-0.2.6.tar` & `dlqhandler-0.2.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 05:45:08.553003 dlqhandler-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-31 05:44:45.000000 dlqhandler-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-31 05:45:08.553003 dlqhandler-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-31 05:44:45.000000 dlqhandler-0.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 05:45:08.549003 dlqhandler-0.2.6/dlqhandler/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-31 05:44:45.000000 dlqhandler-0.2.6/dlqhandler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 05:45:08.549003 dlqhandler-0.2.6/dlqhandler/dataprovider/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 05:44:45.000000 dlqhandler-0.2.6/dlqhandler/dataprovider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-31 05:44:45.000000 dlqhandler-0.2.6/dlqhandler/dataprovider/send_to_aws_sqs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-31 05:44:45.000000 dlqhandler-0.2.6/dlqhandler/dataprovider/sqs_queue.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 05:45:08.549003 dlqhandler-0.2.6/dlqhandler/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 05:44:45.000000 dlqhandler-0.2.6/dlqhandler/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-05-31 05:44:45.000000 dlqhandler-0.2.6/dlqhandler/services/cloudwatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-05-31 05:44:45.000000 dlqhandler-0.2.6/dlqhandler/services/process.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 05:45:08.549003 dlqhandler-0.2.6/dlqhandler/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 05:44:45.000000 dlqhandler-0.2.6/dlqhandler/tests/__ini__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-31 05:44:45.000000 dlqhandler-0.2.6/dlqhandler/tests/test_process.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 05:45:08.549003 dlqhandler-0.2.6/dlqhandler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-31 05:45:08.000000 dlqhandler-0.2.6/dlqhandler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-31 05:45:08.000000 dlqhandler-0.2.6/dlqhandler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 05:45:08.000000 dlqhandler-0.2.6/dlqhandler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-31 05:45:08.000000 dlqhandler-0.2.6/dlqhandler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-31 05:45:08.000000 dlqhandler-0.2.6/dlqhandler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 05:45:08.553003 dlqhandler-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-31 05:44:45.000000 dlqhandler-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:55:57.831411 dlqhandler-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-31 14:55:40.000000 dlqhandler-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-31 14:55:57.831411 dlqhandler-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-31 14:55:40.000000 dlqhandler-0.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:55:57.827411 dlqhandler-0.2.7/dlqhandler/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-31 14:55:40.000000 dlqhandler-0.2.7/dlqhandler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:55:57.831411 dlqhandler-0.2.7/dlqhandler/dataprovider/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 14:55:40.000000 dlqhandler-0.2.7/dlqhandler/dataprovider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-31 14:55:40.000000 dlqhandler-0.2.7/dlqhandler/dataprovider/send_to_aws_sqs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-31 14:55:40.000000 dlqhandler-0.2.7/dlqhandler/dataprovider/sqs_queue.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:55:57.831411 dlqhandler-0.2.7/dlqhandler/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 14:55:40.000000 dlqhandler-0.2.7/dlqhandler/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-05-31 14:55:40.000000 dlqhandler-0.2.7/dlqhandler/services/cloudwatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-05-31 14:55:40.000000 dlqhandler-0.2.7/dlqhandler/services/process.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:55:57.831411 dlqhandler-0.2.7/dlqhandler/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 14:55:40.000000 dlqhandler-0.2.7/dlqhandler/tests/__ini__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-05-31 14:55:40.000000 dlqhandler-0.2.7/dlqhandler/tests/test_process.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:55:57.831411 dlqhandler-0.2.7/dlqhandler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-31 14:55:57.000000 dlqhandler-0.2.7/dlqhandler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-31 14:55:57.000000 dlqhandler-0.2.7/dlqhandler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 14:55:57.000000 dlqhandler-0.2.7/dlqhandler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-31 14:55:57.000000 dlqhandler-0.2.7/dlqhandler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-31 14:55:57.000000 dlqhandler-0.2.7/dlqhandler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 14:55:57.831411 dlqhandler-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-31 14:55:40.000000 dlqhandler-0.2.7/setup.py
```

### Comparing `dlqhandler-0.2.6/LICENSE` & `dlqhandler-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dlqhandler-0.2.6/PKG-INFO` & `dlqhandler-0.2.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlqhandler
-Version: 0.2.6
+Version: 0.2.7
 Summary: A library for handling DLQ messages in AWS SQS
 Home-page: https://github.com/seuusuario/dlq_handler_lib
 Author: Marcelo Ferreira
 Author-email: jaytilangus@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dlqhandler-0.2.6/README.md` & `dlqhandler-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `dlqhandler-0.2.6/dlqhandler/dataprovider/send_to_aws_sqs.py` & `dlqhandler-0.2.7/dlqhandler/dataprovider/send_to_aws_sqs.py`

 * *Files identical despite different names*

### Comparing `dlqhandler-0.2.6/dlqhandler/dataprovider/sqs_queue.py` & `dlqhandler-0.2.7/dlqhandler/dataprovider/sqs_queue.py`

 * *Files identical despite different names*

### Comparing `dlqhandler-0.2.6/dlqhandler/services/cloudwatch.py` & `dlqhandler-0.2.7/dlqhandler/services/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `dlqhandler-0.2.6/dlqhandler/services/process.py` & `dlqhandler-0.2.7/dlqhandler/services/process.py`

 * *Files identical despite different names*

### Comparing `dlqhandler-0.2.6/dlqhandler.egg-info/PKG-INFO` & `dlqhandler-0.2.7/dlqhandler.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlqhandler
-Version: 0.2.6
+Version: 0.2.7
 Summary: A library for handling DLQ messages in AWS SQS
 Home-page: https://github.com/seuusuario/dlq_handler_lib
 Author: Marcelo Ferreira
 Author-email: jaytilangus@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dlqhandler-0.2.6/setup.py` & `dlqhandler-0.2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='dlqhandler',
-    version="0.2.6",
+    version="0.2.7",
     packages=['dlqhandler', 'dlqhandler.services', 'dlqhandler.dataprovider', 'dlqhandler.tests'],
     install_requires=[
         'boto3',
         'mock'
     ],
     author="Marcelo Ferreira",
     author_email="jaytilangus@gmail.com",
```

