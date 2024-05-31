# Comparing `tmp/roboto_ingestion_utils-0.0.8.tar.gz` & `tmp/roboto_ingestion_utils-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roboto_ingestion_utils-0.0.8.tar", last modified: Tue May 28 13:49:38 2024, max compression
+gzip compressed data, was "roboto_ingestion_utils-0.0.9.tar", last modified: Fri May 31 10:37:53 2024, max compression
```

## Comparing `roboto_ingestion_utils-0.0.8.tar` & `roboto_ingestion_utils-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 yves      (1000) yves      (1000)        0 2024-05-28 13:49:38.627130 roboto_ingestion_utils-0.0.8/
--rw-rw-r--   0 yves      (1000) yves      (1000)     3078 2024-05-28 08:13:50.000000 roboto_ingestion_utils-0.0.8/.gitignore
--rw-rw-r--   0 yves      (1000) yves      (1000)    11357 2024-05-28 08:13:50.000000 roboto_ingestion_utils-0.0.8/LICENSE
--rw-rw-r--   0 yves      (1000) yves      (1000)      521 2024-05-28 13:49:38.627130 roboto_ingestion_utils-0.0.8/PKG-INFO
--rw-rw-r--   0 yves      (1000) yves      (1000)       50 2024-05-28 08:13:50.000000 roboto_ingestion_utils-0.0.8/README.md
--rwxrwxrwx   0 yves      (1000) yves      (1000)      112 2024-05-28 13:42:40.000000 roboto_ingestion_utils-0.0.8/build.sh
--rw-rw-r--   0 yves      (1000) yves      (1000)       90 2024-05-28 08:45:43.000000 roboto_ingestion_utils-0.0.8/pyproject.toml
-drwxrwxr-x   0 yves      (1000) yves      (1000)        0 2024-05-28 13:49:38.623130 roboto_ingestion_utils-0.0.8/roboto_ingestion_utils/
--rw-rw-r--   0 yves      (1000) yves      (1000)        0 2024-05-28 09:14:14.000000 roboto_ingestion_utils-0.0.8/roboto_ingestion_utils/__init__.py
--rw-rw-r--   0 yves      (1000) yves      (1000)     6225 2024-05-28 10:39:32.000000 roboto_ingestion_utils-0.0.8/roboto_ingestion_utils/ingestion_utils.py
--rw-rw-r--   0 yves      (1000) yves      (1000)      985 2024-05-28 10:39:21.000000 roboto_ingestion_utils-0.0.8/roboto_ingestion_utils/timed.py
-drwxrwxr-x   0 yves      (1000) yves      (1000)        0 2024-05-28 13:49:38.627130 roboto_ingestion_utils-0.0.8/roboto_ingestion_utils.egg-info/
--rw-r--r--   0 yves      (1000) yves      (1000)      521 2024-05-28 13:49:38.000000 roboto_ingestion_utils-0.0.8/roboto_ingestion_utils.egg-info/PKG-INFO
--rw-rw-r--   0 yves      (1000) yves      (1000)      374 2024-05-28 13:49:38.000000 roboto_ingestion_utils-0.0.8/roboto_ingestion_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 yves      (1000) yves      (1000)        1 2024-05-28 13:49:38.000000 roboto_ingestion_utils-0.0.8/roboto_ingestion_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 yves      (1000) yves      (1000)       23 2024-05-28 13:49:38.000000 roboto_ingestion_utils-0.0.8/roboto_ingestion_utils.egg-info/top_level.txt
--rw-rw-r--   0 yves      (1000) yves      (1000)       38 2024-05-28 13:49:38.627130 roboto_ingestion_utils-0.0.8/setup.cfg
--rw-rw-r--   0 yves      (1000) yves      (1000)      698 2024-05-28 13:41:20.000000 roboto_ingestion_utils-0.0.8/setup.py
-drwxrwxr-x   0 yves      (1000) yves      (1000)        0 2024-05-28 13:49:38.627130 roboto_ingestion_utils-0.0.8/tests/
--rw-rw-r--   0 yves      (1000) yves      (1000)      358 2024-05-28 10:04:51.000000 roboto_ingestion_utils-0.0.8/tests/test_utils.py
+drwxrwxr-x   0 yves      (1000) yves      (1000)        0 2024-05-31 10:37:53.042541 roboto_ingestion_utils-0.0.9/
+-rw-rw-r--   0 yves      (1000) yves      (1000)     3078 2024-05-28 08:13:50.000000 roboto_ingestion_utils-0.0.9/.gitignore
+-rw-rw-r--   0 yves      (1000) yves      (1000)    11357 2024-05-28 08:13:50.000000 roboto_ingestion_utils-0.0.9/LICENSE
+-rw-rw-r--   0 yves      (1000) yves      (1000)      521 2024-05-31 10:37:53.038541 roboto_ingestion_utils-0.0.9/PKG-INFO
+-rw-rw-r--   0 yves      (1000) yves      (1000)       50 2024-05-28 08:13:50.000000 roboto_ingestion_utils-0.0.9/README.md
+-rwxrwxrwx   0 yves      (1000) yves      (1000)      112 2024-05-28 13:42:40.000000 roboto_ingestion_utils-0.0.9/build.sh
+-rw-rw-r--   0 yves      (1000) yves      (1000)       90 2024-05-28 08:45:43.000000 roboto_ingestion_utils-0.0.9/pyproject.toml
+drwxrwxr-x   0 yves      (1000) yves      (1000)        0 2024-05-31 10:37:53.038541 roboto_ingestion_utils-0.0.9/roboto_ingestion_utils/
+-rw-rw-r--   0 yves      (1000) yves      (1000)        0 2024-05-28 09:14:14.000000 roboto_ingestion_utils-0.0.9/roboto_ingestion_utils/__init__.py
+-rw-rw-r--   0 yves      (1000) yves      (1000)     6531 2024-05-31 10:37:01.000000 roboto_ingestion_utils-0.0.9/roboto_ingestion_utils/ingestion_utils.py
+-rw-rw-r--   0 yves      (1000) yves      (1000)      985 2024-05-28 10:39:21.000000 roboto_ingestion_utils-0.0.9/roboto_ingestion_utils/timed.py
+drwxrwxr-x   0 yves      (1000) yves      (1000)        0 2024-05-31 10:37:53.038541 roboto_ingestion_utils-0.0.9/roboto_ingestion_utils.egg-info/
+-rw-r--r--   0 yves      (1000) yves      (1000)      521 2024-05-31 10:37:52.000000 roboto_ingestion_utils-0.0.9/roboto_ingestion_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 yves      (1000) yves      (1000)      374 2024-05-31 10:37:53.000000 roboto_ingestion_utils-0.0.9/roboto_ingestion_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 yves      (1000) yves      (1000)        1 2024-05-31 10:37:52.000000 roboto_ingestion_utils-0.0.9/roboto_ingestion_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 yves      (1000) yves      (1000)       23 2024-05-31 10:37:52.000000 roboto_ingestion_utils-0.0.9/roboto_ingestion_utils.egg-info/top_level.txt
+-rw-rw-r--   0 yves      (1000) yves      (1000)       38 2024-05-31 10:37:53.042541 roboto_ingestion_utils-0.0.9/setup.cfg
+-rw-rw-r--   0 yves      (1000) yves      (1000)      698 2024-05-31 10:37:45.000000 roboto_ingestion_utils-0.0.9/setup.py
+drwxrwxr-x   0 yves      (1000) yves      (1000)        0 2024-05-31 10:37:53.038541 roboto_ingestion_utils-0.0.9/tests/
+-rw-rw-r--   0 yves      (1000) yves      (1000)      358 2024-05-28 10:04:51.000000 roboto_ingestion_utils-0.0.9/tests/test_utils.py
```

### Comparing `roboto_ingestion_utils-0.0.8/.gitignore` & `roboto_ingestion_utils-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `roboto_ingestion_utils-0.0.8/LICENSE` & `roboto_ingestion_utils-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `roboto_ingestion_utils-0.0.8/PKG-INFO` & `roboto_ingestion_utils-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roboto_ingestion_utils
-Version: 0.0.8
+Version: 0.0.9
 Summary: Utility functions for roboto data ingestion
 Home-page: https://github.com/roboto-ai/roboto-ingestion-utils
 Author: Roboto Technologies
 Author-email: yves@roboto.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `roboto_ingestion_utils-0.0.8/roboto_ingestion_utils/ingestion_utils.py` & `roboto_ingestion_utils-0.0.9/roboto_ingestion_utils/ingestion_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -191,27 +191,34 @@
     """
     Set up the logger for the action.
 
     Returns:
     - None
     """
     log_file = (
-            pathlib.Path(default_env.output_dir)
-            / ".metrics"
-            / f"process_timing_{default_env.invocation_id}.csv"
+        pathlib.Path(default_env.output_dir)
+        / ".metrics"
+        / f"process_timing_{default_env.invocation_id}.csv"
     )
     log_file.parent.mkdir(parents=True, exist_ok=True)
 
     logger = logging.getLogger(logger_name)
     logger.setLevel(logging.DEBUG)
 
     # Remove any existing handlers
     logger.handlers = []
 
+    # File handler
     file_handler = logging.FileHandler(str(log_file))
     file_handler.setLevel(logging.DEBUG)
+    file_formatter = logging.Formatter('%(message)s')
+    file_handler.setFormatter(file_formatter)
+    logger.addHandler(file_handler)
 
-    # Create a logging format
-    formatter = logging.Formatter('%(message)s')
-    file_handler.setFormatter(formatter)
+    # Console handler
+    console_handler = logging.StreamHandler()
+    console_handler.setLevel(logging.DEBUG)
+    console_formatter = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
+    console_handler.setFormatter(console_formatter)
+    logger.addHandler(console_handler)
 
-    logger.addHandler(file_handler)
+    return logger
```

### Comparing `roboto_ingestion_utils-0.0.8/roboto_ingestion_utils/timed.py` & `roboto_ingestion_utils-0.0.9/roboto_ingestion_utils/timed.py`

 * *Files identical despite different names*

### Comparing `roboto_ingestion_utils-0.0.8/roboto_ingestion_utils.egg-info/PKG-INFO` & `roboto_ingestion_utils-0.0.9/roboto_ingestion_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roboto-ingestion-utils
-Version: 0.0.8
+Version: 0.0.9
 Summary: Utility functions for roboto data ingestion
 Home-page: https://github.com/roboto-ai/roboto-ingestion-utils
 Author: Roboto Technologies
 Author-email: yves@roboto.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `roboto_ingestion_utils-0.0.8/setup.py` & `roboto_ingestion_utils-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='roboto_ingestion_utils',
-    version='0.0.8',
+    version='0.0.9',
     author='Roboto Technologies',
     author_email='yves@roboto.ai',
     description='Utility functions for roboto data ingestion',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/roboto-ai/roboto-ingestion-utils',
     packages=find_packages(),
```

