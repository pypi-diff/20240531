# Comparing `tmp/pythonanywhere-0.9.8.tar.gz` & `tmp/pythonanywhere-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pythonanywhere-0.9.8.tar", last modified: Sat May  8 08:00:28 2021, max compression
+gzip compressed data, was "dist/pythonanywhere-0.9.9.tar", last modified: Thu Jun 17 12:03:17 2021, max compression
```

## Comparing `pythonanywhere-0.9.8.tar` & `pythonanywhere-0.9.9.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 fjl       (1000) users      (985)        0 2021-05-08 08:00:28.000000 pythonanywhere-0.9.8/
-drwxr-xr-x   0 fjl       (1000) users      (985)        0 2021-05-08 08:00:28.000000 pythonanywhere-0.9.8/pythonanywhere.egg-info/
--rw-r--r--   0 fjl       (1000) users      (985)        1 2021-05-08 08:00:27.000000 pythonanywhere-0.9.8/pythonanywhere.egg-info/dependency_links.txt
--rw-r--r--   0 fjl       (1000) users      (985)     4460 2021-05-08 08:00:27.000000 pythonanywhere-0.9.8/pythonanywhere.egg-info/PKG-INFO
--rw-r--r--   0 fjl       (1000) users      (985)     1192 2021-05-08 08:00:27.000000 pythonanywhere-0.9.8/pythonanywhere.egg-info/SOURCES.txt
--rw-r--r--   0 fjl       (1000) users      (985)       64 2021-05-08 08:00:27.000000 pythonanywhere-0.9.8/pythonanywhere.egg-info/requires.txt
--rw-r--r--   0 fjl       (1000) users      (985)       19 2021-05-08 08:00:27.000000 pythonanywhere-0.9.8/pythonanywhere.egg-info/top_level.txt
-drwxr-xr-x   0 fjl       (1000) users      (985)        0 2021-05-08 08:00:28.000000 pythonanywhere-0.9.8/cli/
--rw-r--r--   0 fjl       (1000) users      (985)     4978 2021-02-19 15:42:42.000000 pythonanywhere-0.9.8/cli/webapp.py
--rwxr-xr-x   0 fjl       (1000) users      (985)      557 2021-05-07 09:45:22.000000 pythonanywhere-0.9.8/cli/pa
--rw-r--r--   0 fjl       (1000) users      (985)    10800 2021-02-19 15:42:42.000000 pythonanywhere-0.9.8/cli/schedule.py
--rw-r--r--   0 fjl       (1000) users      (985)        0 2021-02-19 15:42:42.000000 pythonanywhere-0.9.8/cli/__init__.py
--rw-r--r--   0 fjl       (1000) users      (985)     3035 2021-02-19 15:42:42.000000 pythonanywhere-0.9.8/cli/django.py
--rw-r--r--   0 fjl       (1000) users      (985)     4460 2021-05-08 08:00:28.000000 pythonanywhere-0.9.8/PKG-INFO
--rw-r--r--   0 fjl       (1000) users      (985)       38 2021-05-08 08:00:28.000000 pythonanywhere-0.9.8/setup.cfg
-drwxr-xr-x   0 fjl       (1000) users      (985)        0 2021-05-08 08:00:28.000000 pythonanywhere-0.9.8/scripts/
--rwxr-xr-x   0 fjl       (1000) users      (985)     3983 2020-05-22 17:21:57.000000 pythonanywhere-0.9.8/scripts/pa_update_scheduled_task.py
--rwxr-xr-x   0 fjl       (1000) users      (985)     1896 2021-02-19 19:07:25.000000 pythonanywhere-0.9.8/scripts/pa_autoconfigure_django.py
--rwxr-xr-x   0 fjl       (1000) users      (985)     1638 2020-05-22 17:21:57.000000 pythonanywhere-0.9.8/scripts/pa_get_scheduled_tasks_list.py
--rwxr-xr-x   0 fjl       (1000) users      (985)     1733 2020-05-22 17:21:57.000000 pythonanywhere-0.9.8/scripts/pa_create_webapp_with_virtualenv.py
--rwxr-xr-x   0 fjl       (1000) users      (985)     1467 2020-05-22 17:21:57.000000 pythonanywhere-0.9.8/scripts/pa_delete_webapp_logs.py
--rwxr-xr-x   0 fjl       (1000) users      (985)     2945 2020-05-25 18:57:12.000000 pythonanywhere-0.9.8/scripts/pa_install_webapp_letsencrypt_ssl.py
--rwxr-xr-x   0 fjl       (1000) users      (985)     2315 2020-05-25 18:57:12.000000 pythonanywhere-0.9.8/scripts/pa_install_webapp_ssl.py
--rwxr-xr-x   0 fjl       (1000) users      (985)     4007 2020-05-25 18:57:12.000000 pythonanywhere-0.9.8/scripts/pa_get_scheduled_task_specs.py
--rwxr-xr-x   0 fjl       (1000) users      (985)      516 2020-05-25 18:57:12.000000 pythonanywhere-0.9.8/scripts/pa_reload_webapp.py
--rwxr-xr-x   0 fjl       (1000) users      (985)     1588 2020-05-25 18:57:12.000000 pythonanywhere-0.9.8/scripts/pa_start_django_webapp_with_virtualenv.py
--rwxr-xr-x   0 fjl       (1000) users      (985)     2018 2020-05-22 17:21:57.000000 pythonanywhere-0.9.8/scripts/pa_create_scheduled_task.py
--rwxr-xr-x   0 fjl       (1000) users      (985)     1389 2020-11-20 11:18:00.000000 pythonanywhere-0.9.8/scripts/pa_delete_scheduled_task.py
--rw-r--r--   0 fjl       (1000) users      (985)     3244 2020-05-25 18:57:12.000000 pythonanywhere-0.9.8/README.md
--rw-r--r--   0 fjl       (1000) users      (985)       18 2020-02-02 20:51:03.000000 pythonanywhere-0.9.8/MANIFEST.in
--rw-r--r--   0 fjl       (1000) users      (985)     2012 2021-05-07 10:31:15.000000 pythonanywhere-0.9.8/setup.py
-drwxr-xr-x   0 fjl       (1000) users      (985)        0 2021-05-08 08:00:28.000000 pythonanywhere-0.9.8/pythonanywhere/
--rw-r--r--   0 fjl       (1000) users      (985)       43 2020-02-02 20:51:03.000000 pythonanywhere-0.9.8/pythonanywhere/exceptions.py
--rw-r--r--   0 fjl       (1000) users      (985)      539 2020-02-02 20:51:03.000000 pythonanywhere-0.9.8/pythonanywhere/wsgi_file_template.py
--rw-r--r--   0 fjl       (1000) users      (985)     1354 2020-11-20 09:49:13.000000 pythonanywhere-0.9.8/pythonanywhere/virtualenvs.py
--rw-r--r--   0 fjl       (1000) users      (985)     7940 2020-05-25 18:57:12.000000 pythonanywhere-0.9.8/pythonanywhere/task.py
--rw-r--r--   0 fjl       (1000) users      (985)      307 2020-05-25 18:57:12.000000 pythonanywhere-0.9.8/pythonanywhere/utils.py
--rw-r--r--   0 fjl       (1000) users      (985)       22 2020-05-25 18:57:12.000000 pythonanywhere-0.9.8/pythonanywhere/__init__.py
--rw-r--r--   0 fjl       (1000) users      (985)     4382 2020-05-25 18:57:12.000000 pythonanywhere-0.9.8/pythonanywhere/scripts_commons.py
--rw-r--r--   0 fjl       (1000) users      (985)     1960 2020-05-25 18:57:12.000000 pythonanywhere-0.9.8/pythonanywhere/project.py
--rw-r--r--   0 fjl       (1000) users      (985)     1659 2020-05-25 18:57:12.000000 pythonanywhere-0.9.8/pythonanywhere/launch_bash_in_virtualenv.py
--rwxr-xr-x   0 fjl       (1000) users      (985)      873 2020-05-25 18:57:12.000000 pythonanywhere-0.9.8/pythonanywhere/snakesay.py
-drwxr-xr-x   0 fjl       (1000) users      (985)        0 2021-05-08 08:00:28.000000 pythonanywhere-0.9.8/pythonanywhere/api/
--rw-r--r--   0 fjl       (1000) users      (985)     7865 2020-05-25 18:57:12.000000 pythonanywhere-0.9.8/pythonanywhere/api/webapp.py
--rw-r--r--   0 fjl       (1000) users      (985)     3712 2020-05-25 18:57:12.000000 pythonanywhere-0.9.8/pythonanywhere/api/schedule.py
--rw-r--r--   0 fjl       (1000) users      (985)      558 2020-05-22 17:21:57.000000 pythonanywhere-0.9.8/pythonanywhere/api/__init__.py
--rw-r--r--   0 fjl       (1000) users      (985)     1404 2021-05-06 14:20:55.000000 pythonanywhere-0.9.8/pythonanywhere/api/base.py
--rw-r--r--   0 fjl       (1000) users      (985)     5033 2021-02-22 15:09:36.000000 pythonanywhere-0.9.8/pythonanywhere/django_project.py
+drwxr-xr-x   0 fjl       (1000) users      (985)        0 2021-06-17 12:03:17.000000 pythonanywhere-0.9.9/
+drwxr-xr-x   0 fjl       (1000) users      (985)        0 2021-06-17 12:03:17.000000 pythonanywhere-0.9.9/pythonanywhere.egg-info/
+-rw-r--r--   0 fjl       (1000) users      (985)        1 2021-06-17 12:03:17.000000 pythonanywhere-0.9.9/pythonanywhere.egg-info/dependency_links.txt
+-rw-r--r--   0 fjl       (1000) users      (985)     4510 2021-06-17 12:03:17.000000 pythonanywhere-0.9.9/pythonanywhere.egg-info/PKG-INFO
+-rw-r--r--   0 fjl       (1000) users      (985)     1192 2021-06-17 12:03:17.000000 pythonanywhere-0.9.9/pythonanywhere.egg-info/SOURCES.txt
+-rw-r--r--   0 fjl       (1000) users      (985)       64 2021-06-17 12:03:17.000000 pythonanywhere-0.9.9/pythonanywhere.egg-info/requires.txt
+-rw-r--r--   0 fjl       (1000) users      (985)       19 2021-06-17 12:03:17.000000 pythonanywhere-0.9.9/pythonanywhere.egg-info/top_level.txt
+drwxr-xr-x   0 fjl       (1000) users      (985)        0 2021-06-17 12:03:17.000000 pythonanywhere-0.9.9/cli/
+-rw-r--r--   0 fjl       (1000) users      (985)     4978 2021-05-21 10:47:17.000000 pythonanywhere-0.9.9/cli/webapp.py
+-rwxr-xr-x   0 fjl       (1000) users      (985)      557 2021-05-21 12:34:36.000000 pythonanywhere-0.9.9/cli/pa
+-rw-r--r--   0 fjl       (1000) users      (985)    10800 2021-05-21 11:14:17.000000 pythonanywhere-0.9.9/cli/schedule.py
+-rw-r--r--   0 fjl       (1000) users      (985)        0 2021-05-21 10:14:55.000000 pythonanywhere-0.9.9/cli/__init__.py
+-rw-r--r--   0 fjl       (1000) users      (985)     3035 2021-05-21 10:47:01.000000 pythonanywhere-0.9.9/cli/django.py
+-rw-r--r--   0 fjl       (1000) users      (985)     4510 2021-06-17 12:03:17.000000 pythonanywhere-0.9.9/PKG-INFO
+-rw-r--r--   0 fjl       (1000) users      (985)       38 2021-06-17 12:03:17.000000 pythonanywhere-0.9.9/setup.cfg
+drwxr-xr-x   0 fjl       (1000) users      (985)        0 2021-06-17 12:03:17.000000 pythonanywhere-0.9.9/scripts/
+-rwxr-xr-x   0 fjl       (1000) users      (985)     3983 2020-05-22 17:21:57.000000 pythonanywhere-0.9.9/scripts/pa_update_scheduled_task.py
+-rwxr-xr-x   0 fjl       (1000) users      (985)     1896 2021-05-21 10:14:55.000000 pythonanywhere-0.9.9/scripts/pa_autoconfigure_django.py
+-rwxr-xr-x   0 fjl       (1000) users      (985)     1638 2020-05-22 17:21:57.000000 pythonanywhere-0.9.9/scripts/pa_get_scheduled_tasks_list.py
+-rwxr-xr-x   0 fjl       (1000) users      (985)     1733 2020-05-22 17:21:57.000000 pythonanywhere-0.9.9/scripts/pa_create_webapp_with_virtualenv.py
+-rwxr-xr-x   0 fjl       (1000) users      (985)     1467 2020-05-22 17:21:57.000000 pythonanywhere-0.9.9/scripts/pa_delete_webapp_logs.py
+-rwxr-xr-x   0 fjl       (1000) users      (985)     2945 2020-05-25 18:57:12.000000 pythonanywhere-0.9.9/scripts/pa_install_webapp_letsencrypt_ssl.py
+-rwxr-xr-x   0 fjl       (1000) users      (985)     2315 2020-05-25 18:57:12.000000 pythonanywhere-0.9.9/scripts/pa_install_webapp_ssl.py
+-rwxr-xr-x   0 fjl       (1000) users      (985)     4007 2020-05-25 18:57:12.000000 pythonanywhere-0.9.9/scripts/pa_get_scheduled_task_specs.py
+-rwxr-xr-x   0 fjl       (1000) users      (985)      516 2020-05-25 18:57:12.000000 pythonanywhere-0.9.9/scripts/pa_reload_webapp.py
+-rwxr-xr-x   0 fjl       (1000) users      (985)     1588 2020-05-25 18:57:12.000000 pythonanywhere-0.9.9/scripts/pa_start_django_webapp_with_virtualenv.py
+-rwxr-xr-x   0 fjl       (1000) users      (985)     2018 2020-05-22 17:21:57.000000 pythonanywhere-0.9.9/scripts/pa_create_scheduled_task.py
+-rwxr-xr-x   0 fjl       (1000) users      (985)     1389 2020-11-20 11:18:00.000000 pythonanywhere-0.9.9/scripts/pa_delete_scheduled_task.py
+-rw-r--r--   0 fjl       (1000) users      (985)     3244 2020-05-25 18:57:12.000000 pythonanywhere-0.9.9/README.md
+-rw-r--r--   0 fjl       (1000) users      (985)       18 2020-02-02 20:51:03.000000 pythonanywhere-0.9.9/MANIFEST.in
+-rw-r--r--   0 fjl       (1000) users      (985)     2061 2021-06-17 12:01:32.000000 pythonanywhere-0.9.9/setup.py
+drwxr-xr-x   0 fjl       (1000) users      (985)        0 2021-06-17 12:03:17.000000 pythonanywhere-0.9.9/pythonanywhere/
+-rw-r--r--   0 fjl       (1000) users      (985)       43 2020-02-02 20:51:03.000000 pythonanywhere-0.9.9/pythonanywhere/exceptions.py
+-rw-r--r--   0 fjl       (1000) users      (985)      539 2020-02-02 20:51:03.000000 pythonanywhere-0.9.9/pythonanywhere/wsgi_file_template.py
+-rw-r--r--   0 fjl       (1000) users      (985)     1354 2020-11-20 09:49:13.000000 pythonanywhere-0.9.9/pythonanywhere/virtualenvs.py
+-rw-r--r--   0 fjl       (1000) users      (985)     7940 2020-05-25 18:57:12.000000 pythonanywhere-0.9.9/pythonanywhere/task.py
+-rw-r--r--   0 fjl       (1000) users      (985)      307 2020-05-25 18:57:12.000000 pythonanywhere-0.9.9/pythonanywhere/utils.py
+-rw-r--r--   0 fjl       (1000) users      (985)       22 2020-05-25 18:57:12.000000 pythonanywhere-0.9.9/pythonanywhere/__init__.py
+-rw-r--r--   0 fjl       (1000) users      (985)     4382 2020-05-25 18:57:12.000000 pythonanywhere-0.9.9/pythonanywhere/scripts_commons.py
+-rw-r--r--   0 fjl       (1000) users      (985)     1960 2020-05-25 18:57:12.000000 pythonanywhere-0.9.9/pythonanywhere/project.py
+-rw-r--r--   0 fjl       (1000) users      (985)     1659 2020-05-25 18:57:12.000000 pythonanywhere-0.9.9/pythonanywhere/launch_bash_in_virtualenv.py
+-rwxr-xr-x   0 fjl       (1000) users      (985)      873 2020-05-25 18:57:12.000000 pythonanywhere-0.9.9/pythonanywhere/snakesay.py
+drwxr-xr-x   0 fjl       (1000) users      (985)        0 2021-06-17 12:03:17.000000 pythonanywhere-0.9.9/pythonanywhere/api/
+-rw-r--r--   0 fjl       (1000) users      (985)     7865 2020-05-25 18:57:12.000000 pythonanywhere-0.9.9/pythonanywhere/api/webapp.py
+-rw-r--r--   0 fjl       (1000) users      (985)     3712 2020-05-25 18:57:12.000000 pythonanywhere-0.9.9/pythonanywhere/api/schedule.py
+-rw-r--r--   0 fjl       (1000) users      (985)      558 2020-05-22 17:21:57.000000 pythonanywhere-0.9.9/pythonanywhere/api/__init__.py
+-rw-r--r--   0 fjl       (1000) users      (985)     1423 2021-06-17 12:00:52.000000 pythonanywhere-0.9.9/pythonanywhere/api/base.py
+-rw-r--r--   0 fjl       (1000) users      (985)     5033 2021-05-21 10:14:55.000000 pythonanywhere-0.9.9/pythonanywhere/django_project.py
```

### Comparing `pythonanywhere-0.9.8/pythonanywhere.egg-info/PKG-INFO` & `pythonanywhere-0.9.9/pythonanywhere.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythonanywhere
-Version: 0.9.8
+Version: 0.9.9
 Summary: PythonAnywhere helper tools for users
 Home-page: https://github.com/pythonanywhere/helper_scripts/
 Author: PythonAnywhere LLP
 Author-email: developers@pythonanywhere.com
 License: MIT
 Description: [![Build Status](https://travis-ci.org/pythonanywhere/helper_scripts.svg?branch=master)](https://travis-ci.org/pythonanywhere/helper_scripts)
         [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
@@ -69,12 +69,13 @@
         
 Keywords: pythonanywhere api cloud web hosting
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `pythonanywhere-0.9.8/pythonanywhere.egg-info/SOURCES.txt` & `pythonanywhere-0.9.9/pythonanywhere.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pythonanywhere-0.9.8/cli/webapp.py` & `pythonanywhere-0.9.9/cli/webapp.py`

 * *Files identical despite different names*

### Comparing `pythonanywhere-0.9.8/cli/pa` & `pythonanywhere-0.9.9/cli/pa`

 * *Files identical despite different names*

### Comparing `pythonanywhere-0.9.8/cli/schedule.py` & `pythonanywhere-0.9.9/cli/schedule.py`

 * *Files identical despite different names*

### Comparing `pythonanywhere-0.9.8/cli/django.py` & `pythonanywhere-0.9.9/cli/django.py`

 * *Files identical despite different names*

### Comparing `pythonanywhere-0.9.8/PKG-INFO` & `pythonanywhere-0.9.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythonanywhere
-Version: 0.9.8
+Version: 0.9.9
 Summary: PythonAnywhere helper tools for users
 Home-page: https://github.com/pythonanywhere/helper_scripts/
 Author: PythonAnywhere LLP
 Author-email: developers@pythonanywhere.com
 License: MIT
 Description: [![Build Status](https://travis-ci.org/pythonanywhere/helper_scripts.svg?branch=master)](https://travis-ci.org/pythonanywhere/helper_scripts)
         [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
@@ -69,12 +69,13 @@
         
 Keywords: pythonanywhere api cloud web hosting
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `pythonanywhere-0.9.8/scripts/pa_update_scheduled_task.py` & `pythonanywhere-0.9.9/scripts/pa_update_scheduled_task.py`

 * *Files identical despite different names*

### Comparing `pythonanywhere-0.9.8/scripts/pa_autoconfigure_django.py` & `pythonanywhere-0.9.9/scripts/pa_autoconfigure_django.py`

 * *Files identical despite different names*

### Comparing `pythonanywhere-0.9.8/scripts/pa_get_scheduled_tasks_list.py` & `pythonanywhere-0.9.9/scripts/pa_get_scheduled_tasks_list.py`

 * *Files identical despite different names*

### Comparing `pythonanywhere-0.9.8/scripts/pa_create_webapp_with_virtualenv.py` & `pythonanywhere-0.9.9/scripts/pa_create_webapp_with_virtualenv.py`

 * *Files identical despite different names*

### Comparing `pythonanywhere-0.9.8/scripts/pa_delete_webapp_logs.py` & `pythonanywhere-0.9.9/scripts/pa_delete_webapp_logs.py`

 * *Files identical despite different names*

### Comparing `pythonanywhere-0.9.8/scripts/pa_install_webapp_letsencrypt_ssl.py` & `pythonanywhere-0.9.9/scripts/pa_install_webapp_letsencrypt_ssl.py`

 * *Files identical despite different names*

### Comparing `pythonanywhere-0.9.8/scripts/pa_install_webapp_ssl.py` & `pythonanywhere-0.9.9/scripts/pa_install_webapp_ssl.py`

 * *Files identical despite different names*

### Comparing `pythonanywhere-0.9.8/scripts/pa_get_scheduled_task_specs.py` & `pythonanywhere-0.9.9/scripts/pa_get_scheduled_task_specs.py`

 * *Files identical despite different names*

### Comparing `pythonanywhere-0.9.8/scripts/pa_reload_webapp.py` & `pythonanywhere-0.9.9/scripts/pa_reload_webapp.py`

 * *Files identical despite different names*

### Comparing `pythonanywhere-0.9.8/scripts/pa_start_django_webapp_with_virtualenv.py` & `pythonanywhere-0.9.9/scripts/pa_start_django_webapp_with_virtualenv.py`

 * *Files identical despite different names*

### Comparing `pythonanywhere-0.9.8/scripts/pa_create_scheduled_task.py` & `pythonanywhere-0.9.9/scripts/pa_create_scheduled_task.py`

 * *Files identical despite different names*

### Comparing `pythonanywhere-0.9.8/scripts/pa_delete_scheduled_task.py` & `pythonanywhere-0.9.9/scripts/pa_delete_scheduled_task.py`

 * *Files identical despite different names*

### Comparing `pythonanywhere-0.9.8/README.md` & `pythonanywhere-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `pythonanywhere-0.9.8/setup.py` & `pythonanywhere-0.9.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,27 +5,28 @@
 
 # Get the long description from the README file
 with (here / "README.md").open(encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="pythonanywhere",
-    version="0.9.8",
+    version="0.9.9",
     description="PythonAnywhere helper tools for users",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pythonanywhere/helper_scripts/",
     author="PythonAnywhere LLP",
     author_email="developers@pythonanywhere.com",
     license="MIT",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries",
         "License :: OSI Approved :: MIT License",
+        "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.6",
     ],
     keywords="pythonanywhere api cloud web hosting",
     packages=["cli", "pythonanywhere", "pythonanywhere.api"],
     install_requires=[
```

### Comparing `pythonanywhere-0.9.8/pythonanywhere/wsgi_file_template.py` & `pythonanywhere-0.9.9/pythonanywhere/wsgi_file_template.py`

 * *Files identical despite different names*

### Comparing `pythonanywhere-0.9.8/pythonanywhere/virtualenvs.py` & `pythonanywhere-0.9.9/pythonanywhere/virtualenvs.py`

 * *Files identical despite different names*

### Comparing `pythonanywhere-0.9.8/pythonanywhere/task.py` & `pythonanywhere-0.9.9/pythonanywhere/task.py`

 * *Files identical despite different names*

### Comparing `pythonanywhere-0.9.8/pythonanywhere/scripts_commons.py` & `pythonanywhere-0.9.9/pythonanywhere/scripts_commons.py`

 * *Files identical despite different names*

### Comparing `pythonanywhere-0.9.8/pythonanywhere/project.py` & `pythonanywhere-0.9.9/pythonanywhere/project.py`

 * *Files identical despite different names*

### Comparing `pythonanywhere-0.9.8/pythonanywhere/launch_bash_in_virtualenv.py` & `pythonanywhere-0.9.9/pythonanywhere/launch_bash_in_virtualenv.py`

 * *Files identical despite different names*

### Comparing `pythonanywhere-0.9.8/pythonanywhere/snakesay.py` & `pythonanywhere-0.9.9/pythonanywhere/snakesay.py`

 * *Files identical despite different names*

### Comparing `pythonanywhere-0.9.8/pythonanywhere/api/webapp.py` & `pythonanywhere-0.9.9/pythonanywhere/api/webapp.py`

 * *Files identical despite different names*

### Comparing `pythonanywhere-0.9.8/pythonanywhere/api/schedule.py` & `pythonanywhere-0.9.9/pythonanywhere/api/schedule.py`

 * *Files identical despite different names*

### Comparing `pythonanywhere-0.9.8/pythonanywhere/api/__init__.py` & `pythonanywhere-0.9.9/pythonanywhere/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonanywhere-0.9.8/pythonanywhere/api/base.py` & `pythonanywhere-0.9.9/pythonanywhere/api/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 
 import requests
 
 PYTHON_VERSIONS = {
-    "3.6": "python36", "3.7": "python37", "3.8": "python38",
+    "3.6": "python36", "3.7": "python37", "3.8": "python38", "3.9": "python39",
 }
 
 
 class AuthenticationError(Exception):
     pass
```

### Comparing `pythonanywhere-0.9.8/pythonanywhere/django_project.py` & `pythonanywhere-0.9.9/pythonanywhere/django_project.py`

 * *Files identical despite different names*

