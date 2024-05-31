# Comparing `tmp/dlqhandler-0.2.5.tar.gz` & `tmp/dlqhandler-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dlqhandler-0.2.5.tar", last modified: Fri May 31 05:23:00 2024, max compression
+gzip compressed data, was "dlqhandler-0.2.6.tar", last modified: Fri May 31 05:45:08 2024, max compression
```

## Comparing `dlqhandler-0.2.5.tar` & `dlqhandler-0.2.6.tar`

### file list

```diff
@@ -1,26 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 05:23:00.719813 dlqhandler-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-31 05:22:37.000000 dlqhandler-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-31 05:23:00.719813 dlqhandler-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-31 05:22:37.000000 dlqhandler-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 05:23:00.715813 dlqhandler-0.2.5/dlqhandler/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-31 05:22:37.000000 dlqhandler-0.2.5/dlqhandler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 05:23:00.719813 dlqhandler-0.2.5/dlqhandler/dataprovider/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 05:22:37.000000 dlqhandler-0.2.5/dlqhandler/dataprovider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-31 05:22:37.000000 dlqhandler-0.2.5/dlqhandler/dataprovider/send_to_aws_sqs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-31 05:22:37.000000 dlqhandler-0.2.5/dlqhandler/dataprovider/sqs_queue.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 05:23:00.719813 dlqhandler-0.2.5/dlqhandler/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 05:22:37.000000 dlqhandler-0.2.5/dlqhandler/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-05-31 05:22:37.000000 dlqhandler-0.2.5/dlqhandler/services/cloudwatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-05-31 05:22:37.000000 dlqhandler-0.2.5/dlqhandler/services/process.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 05:23:00.719813 dlqhandler-0.2.5/dlqhandler/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 05:22:37.000000 dlqhandler-0.2.5/dlqhandler/tests/__ini__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-05-31 05:22:37.000000 dlqhandler-0.2.5/dlqhandler/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-05-31 05:22:37.000000 dlqhandler-0.2.5/dlqhandler/tests/test_process.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 05:23:00.715813 dlqhandler-0.2.5/dlqhandler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-31 05:23:00.000000 dlqhandler-0.2.5/dlqhandler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-31 05:23:00.000000 dlqhandler-0.2.5/dlqhandler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 05:23:00.000000 dlqhandler-0.2.5/dlqhandler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-31 05:23:00.000000 dlqhandler-0.2.5/dlqhandler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-31 05:23:00.000000 dlqhandler-0.2.5/dlqhandler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 05:23:00.719813 dlqhandler-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-31 05:22:37.000000 dlqhandler-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 05:45:08.553003 dlqhandler-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-31 05:44:45.000000 dlqhandler-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-31 05:45:08.553003 dlqhandler-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-31 05:44:45.000000 dlqhandler-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 05:45:08.549003 dlqhandler-0.2.6/dlqhandler/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-31 05:44:45.000000 dlqhandler-0.2.6/dlqhandler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 05:45:08.549003 dlqhandler-0.2.6/dlqhandler/dataprovider/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 05:44:45.000000 dlqhandler-0.2.6/dlqhandler/dataprovider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-31 05:44:45.000000 dlqhandler-0.2.6/dlqhandler/dataprovider/send_to_aws_sqs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-31 05:44:45.000000 dlqhandler-0.2.6/dlqhandler/dataprovider/sqs_queue.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 05:45:08.549003 dlqhandler-0.2.6/dlqhandler/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 05:44:45.000000 dlqhandler-0.2.6/dlqhandler/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-05-31 05:44:45.000000 dlqhandler-0.2.6/dlqhandler/services/cloudwatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-05-31 05:44:45.000000 dlqhandler-0.2.6/dlqhandler/services/process.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 05:45:08.549003 dlqhandler-0.2.6/dlqhandler/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 05:44:45.000000 dlqhandler-0.2.6/dlqhandler/tests/__ini__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-31 05:44:45.000000 dlqhandler-0.2.6/dlqhandler/tests/test_process.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 05:45:08.549003 dlqhandler-0.2.6/dlqhandler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-31 05:45:08.000000 dlqhandler-0.2.6/dlqhandler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-31 05:45:08.000000 dlqhandler-0.2.6/dlqhandler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 05:45:08.000000 dlqhandler-0.2.6/dlqhandler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-31 05:45:08.000000 dlqhandler-0.2.6/dlqhandler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-31 05:45:08.000000 dlqhandler-0.2.6/dlqhandler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 05:45:08.553003 dlqhandler-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-31 05:44:45.000000 dlqhandler-0.2.6/setup.py
```

### Comparing `dlqhandler-0.2.5/LICENSE` & `dlqhandler-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dlqhandler-0.2.5/PKG-INFO` & `dlqhandler-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlqhandler
-Version: 0.2.5
+Version: 0.2.6
 Summary: A library for handling DLQ messages in AWS SQS
 Home-page: https://github.com/seuusuario/dlq_handler_lib
 Author: Marcelo Ferreira
 Author-email: jaytilangus@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dlqhandler-0.2.5/README.md` & `dlqhandler-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `dlqhandler-0.2.5/dlqhandler/dataprovider/send_to_aws_sqs.py` & `dlqhandler-0.2.6/dlqhandler/dataprovider/send_to_aws_sqs.py`

 * *Files identical despite different names*

### Comparing `dlqhandler-0.2.5/dlqhandler/dataprovider/sqs_queue.py` & `dlqhandler-0.2.6/dlqhandler/dataprovider/sqs_queue.py`

 * *Files identical despite different names*

### Comparing `dlqhandler-0.2.5/dlqhandler/services/cloudwatch.py` & `dlqhandler-0.2.6/dlqhandler/services/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `dlqhandler-0.2.5/dlqhandler/services/process.py` & `dlqhandler-0.2.6/dlqhandler/services/process.py`

 * *Files identical despite different names*

### Comparing `dlqhandler-0.2.5/dlqhandler/tests/test_app.py` & `dlqhandler-0.2.6/dlqhandler/tests/test_process.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import unittest
 import json
 from unittest.mock import patch, MagicMock
-from dlqhandler import ProcessMessage, SQSQueue, SendToAwsSqs
+from dlqhandler.services.process import ProcessMessage
 
 class TestProcessMessage(unittest.TestCase):
 
     @patch('dlqhandler.services.cloudwatch.CloudWatch')
     @patch('dlqhandler.dataprovider.sqs_queue.SQSQueue')
     @patch('dlqhandler.dataprovider.send_to_aws_sqs.SendToAwsSqs')
     @patch('boto3.client')
@@ -53,11 +53,11 @@
 
         result = self.handler.execute()
 
         #self.mock_sqs_queue.receive_messages_dlq.assert_called_once()
 
         self.assertEqual(result, {'message': 'No messages to process'})
 
-        #self.assertEqual(result, {'message': 'Mensagem reenviada para fila', 'sq': mock_message_body})
+        #self.assertEqual(result, {'message': 'Mensagem reenviada para fila', 'sq': mock_message_body}) 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `dlqhandler-0.2.5/dlqhandler.egg-info/PKG-INFO` & `dlqhandler-0.2.6/dlqhandler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlqhandler
-Version: 0.2.5
+Version: 0.2.6
 Summary: A library for handling DLQ messages in AWS SQS
 Home-page: https://github.com/seuusuario/dlq_handler_lib
 Author: Marcelo Ferreira
 Author-email: jaytilangus@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dlqhandler-0.2.5/setup.py` & `dlqhandler-0.2.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='dlqhandler',
-    version="0.2.5",
+    version="0.2.6",
     packages=['dlqhandler', 'dlqhandler.services', 'dlqhandler.dataprovider', 'dlqhandler.tests'],
     install_requires=[
         'boto3',
         'mock'
     ],
     author="Marcelo Ferreira",
     author_email="jaytilangus@gmail.com",
```

