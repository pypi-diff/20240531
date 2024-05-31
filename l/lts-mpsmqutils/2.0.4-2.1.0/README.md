# Comparing `tmp/lts-mpsmqutils-2.0.4.tar.gz` & `tmp/lts_mpsmqutils-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lts-mpsmqutils-2.0.4.tar", last modified: Fri Aug 18 20:25:10 2023, max compression
+gzip compressed data, was "lts_mpsmqutils-2.1.0.tar", last modified: Fri May 31 19:03:38 2024, max compression
```

## Comparing `lts-mpsmqutils-2.0.4.tar` & `lts_mpsmqutils-2.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2023-08-18 20:25:10.937687 lts-mpsmqutils-2.0.4/
--rw-r--r--   0 dougsimon   (502) staff       (20)     6649 2023-08-18 20:25:10.937413 lts-mpsmqutils-2.0.4/PKG-INFO
--rw-r--r--   0 dougsimon   (502) staff       (20)     5103 2021-10-29 20:43:09.000000 lts-mpsmqutils-2.0.4/README.md
-drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2023-08-18 20:25:10.933208 lts-mpsmqutils-2.0.4/lts_mpsmqutils.egg-info/
--rw-r--r--   0 dougsimon   (502) staff       (20)     6649 2023-08-18 20:25:10.000000 lts-mpsmqutils-2.0.4/lts_mpsmqutils.egg-info/PKG-INFO
--rw-r--r--   0 dougsimon   (502) staff       (20)      369 2023-08-18 20:25:10.000000 lts-mpsmqutils-2.0.4/lts_mpsmqutils.egg-info/SOURCES.txt
--rw-r--r--   0 dougsimon   (502) staff       (20)        1 2023-08-18 20:25:10.000000 lts-mpsmqutils-2.0.4/lts_mpsmqutils.egg-info/dependency_links.txt
--rw-r--r--   0 dougsimon   (502) staff       (20)       62 2023-08-18 20:25:10.000000 lts-mpsmqutils-2.0.4/lts_mpsmqutils.egg-info/requires.txt
--rw-r--r--   0 dougsimon   (502) staff       (20)       11 2023-08-18 20:25:10.000000 lts-mpsmqutils-2.0.4/lts_mpsmqutils.egg-info/top_level.txt
-drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2023-08-18 20:25:10.935732 lts-mpsmqutils-2.0.4/mpsmqutils/
--rw-r--r--   0 dougsimon   (502) staff       (20)        0 2021-10-29 20:43:09.000000 lts-mpsmqutils-2.0.4/mpsmqutils/__init__.py
--rw-r--r--   0 dougsimon   (502) staff       (20)     1095 2023-08-18 20:23:12.000000 lts-mpsmqutils-2.0.4/mpsmqutils/log_wrapper.py
--rw-r--r--   0 dougsimon   (502) staff       (20)    26508 2023-08-18 20:23:12.000000 lts-mpsmqutils-2.0.4/mpsmqutils/messagehandler.py
--rw-r--r--   0 dougsimon   (502) staff       (20)     7491 2023-08-18 20:23:12.000000 lts-mpsmqutils-2.0.4/mpsmqutils/mqutils.py
-drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2023-08-18 20:25:10.936672 lts-mpsmqutils-2.0.4/mpsmqutils/tests/
--rw-r--r--   0 dougsimon   (502) staff       (20)        0 2021-10-29 20:43:09.000000 lts-mpsmqutils-2.0.4/mpsmqutils/tests/__init__.py
--rw-r--r--   0 dougsimon   (502) staff       (20)     4783 2021-10-29 20:43:09.000000 lts-mpsmqutils-2.0.4/mpsmqutils/tests/test_mqutils.py
--rw-r--r--   0 dougsimon   (502) staff       (20)       38 2023-08-18 20:25:10.937762 lts-mpsmqutils-2.0.4/setup.cfg
--rw-r--r--   0 dougsimon   (502) staff       (20)      896 2023-08-18 20:24:47.000000 lts-mpsmqutils-2.0.4/setup.py
+drwxr-xr-x   0 davemayo   (503) staff       (20)        0 2024-05-31 19:03:38.150712 lts_mpsmqutils-2.1.0/
+-rw-r--r--   0 davemayo   (503) staff       (20)     5635 2024-05-31 19:03:38.150473 lts_mpsmqutils-2.1.0/PKG-INFO
+-rw-r--r--   0 davemayo   (503) staff       (20)     5103 2024-05-31 18:13:15.000000 lts_mpsmqutils-2.1.0/README.md
+drwxr-xr-x   0 davemayo   (503) staff       (20)        0 2024-05-31 19:03:38.150151 lts_mpsmqutils-2.1.0/lts_mpsmqutils.egg-info/
+-rw-r--r--   0 davemayo   (503) staff       (20)     5635 2024-05-31 19:03:38.000000 lts_mpsmqutils-2.1.0/lts_mpsmqutils.egg-info/PKG-INFO
+-rw-r--r--   0 davemayo   (503) staff       (20)      369 2024-05-31 19:03:38.000000 lts_mpsmqutils-2.1.0/lts_mpsmqutils.egg-info/SOURCES.txt
+-rw-r--r--   0 davemayo   (503) staff       (20)        1 2024-05-31 19:03:38.000000 lts_mpsmqutils-2.1.0/lts_mpsmqutils.egg-info/dependency_links.txt
+-rw-r--r--   0 davemayo   (503) staff       (20)       62 2024-05-31 19:03:38.000000 lts_mpsmqutils-2.1.0/lts_mpsmqutils.egg-info/requires.txt
+-rw-r--r--   0 davemayo   (503) staff       (20)       11 2024-05-31 19:03:38.000000 lts_mpsmqutils-2.1.0/lts_mpsmqutils.egg-info/top_level.txt
+drwxr-xr-x   0 davemayo   (503) staff       (20)        0 2024-05-31 19:03:38.149307 lts_mpsmqutils-2.1.0/mpsmqutils/
+-rw-r--r--   0 davemayo   (503) staff       (20)        0 2024-05-31 18:13:15.000000 lts_mpsmqutils-2.1.0/mpsmqutils/__init__.py
+-rw-r--r--   0 davemayo   (503) staff       (20)     1095 2024-05-31 18:13:15.000000 lts_mpsmqutils-2.1.0/mpsmqutils/log_wrapper.py
+-rw-r--r--   0 davemayo   (503) staff       (20)    26607 2024-05-31 18:58:12.000000 lts_mpsmqutils-2.1.0/mpsmqutils/messagehandler.py
+-rw-r--r--   0 davemayo   (503) staff       (20)     7491 2024-05-31 18:13:15.000000 lts_mpsmqutils-2.1.0/mpsmqutils/mqutils.py
+drwxr-xr-x   0 davemayo   (503) staff       (20)        0 2024-05-31 19:03:38.149676 lts_mpsmqutils-2.1.0/mpsmqutils/tests/
+-rw-r--r--   0 davemayo   (503) staff       (20)        0 2024-05-31 18:13:15.000000 lts_mpsmqutils-2.1.0/mpsmqutils/tests/__init__.py
+-rw-r--r--   0 davemayo   (503) staff       (20)     4783 2024-05-31 18:13:15.000000 lts_mpsmqutils-2.1.0/mpsmqutils/tests/test_mqutils.py
+-rw-r--r--   0 davemayo   (503) staff       (20)       38 2024-05-31 19:03:38.150763 lts_mpsmqutils-2.1.0/setup.cfg
+-rw-r--r--   0 davemayo   (503) staff       (20)      896 2024-05-31 19:00:53.000000 lts_mpsmqutils-2.1.0/setup.py
```

### Comparing `lts-mpsmqutils-2.0.4/README.md` & `lts_mpsmqutils-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `lts-mpsmqutils-2.0.4/mpsmqutils/log_wrapper.py` & `lts_mpsmqutils-2.1.0/mpsmqutils/log_wrapper.py`

 * *Files identical despite different names*

### Comparing `lts-mpsmqutils-2.0.4/mpsmqutils/messagehandler.py` & `lts_mpsmqutils-2.1.0/mpsmqutils/messagehandler.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 http_client.mount("http://", adapter)
 
 _hostname_prefix = os.getenv('HOSTNAME') + ": "
 
 # Notify config for use in the notify application
 NOTIFY_QUEUE = os.getenv('MQ_NOTIFY_QUEUE', '/queue/iiif_notify')
 DLQ_QUEUE = os.getenv('MQ_DLQ_QUEUE', '/queue/ActiveMQ.DLQ')
+QUEUE_PREFIX = os.getenv("MQ_QUEUE_NAME_PREFIX", '')
 
 # Email SMTP host for use in notify
 NOTIFY_MAIL_RELAY=os.getenv('MQ_NOTIFY_MAIL_RELAY', None)
 NOTIFY_DEFAULT_EMAIL=os.getenv('MQ_NOTIFY_DEFAULT_EMAIL', None)
 
 def call_worker_do_task(task_name, job_ticket_id = None, parent_job_ticket_id = None, worker_url_endpoint = 'do_task', worker_url = os.getenv('WORKER_API_URL'), add_params=None):
     logger.debug("************************ MQUTILS MQLISTENER - CALL WORKER DO TASK *******************************", end='')
@@ -321,15 +322,15 @@
                 except ValueError as e:
                     logger.error(e, end='')
                     job_tracker.append_error(job_ticket_id, 'Unable to get parse the next queue message',  traceback.format_exc(), False)
                     raise e
 
                 # Set the queue name to match the worker type
                 worker_type = json_message["event"]
-                queue = worker_type
+                queue = f'{QUEUE_PREFIX}{worker_type}'
                 logger.debug('worker_type {}'.format(worker_type), end='')
                 tracker_doc = job_tracker.get_tracker_document(job_ticket_id)
                 # Update the number of tries in the tracker file
                 tracker_doc["job_management"]["numberOfTries"] = 0
                 tracker_doc["job_management"]["current_step"] = json_message["current_step"]
                 tracker_doc["job_management"]["job_status"] = "queued"
                 tracker_doc["job_management"]["previous_step_status"] = json_message["previous_step_status"]
@@ -446,24 +447,24 @@
     def __generic_message_handler(self, message_data, worker_endpoint):
         logger.debug("************************ MQUTILS MQLISTENER - GENERIC_MESSAGE_HANDLER *******************************", end='')
         task_success = False
 
         # Call task
         try:
             worker_response = call_generic_worker_api(message_data, worker_endpoint)
-            next_queue = os.getenv('NEXT_QUEUE')
+            next_queue = f"{QUEUE_PREFIX}{os.getenv('NEXT_QUEUE')}"
             task_success = True if worker_response.get('success') else False
             logger.debug("SUCCESS IN WORKER RESPONSE TRY BLOCK", end='')
         except Exception as e:
             logger.error(e, end='')
             task_success = False
 
         if (task_success):
             # Update timestamp file after task is complete
-            if next_queue is None:
+            if next_queue == QUEUE_PREFIX:
                 #There are no more items to queue so the job is actually finished.
                 logger.debug('******** LAST TASK COMPLETED ********', end='')
             else:
                 logger.debug('******** TASK COMPLETED - GOING TO NEXT QUEUE ********', end='')
                 celeryapp.execute.send_task("tasks.tasks.do_task", args=[self.message], kwargs={}, queue=next_queue)
         logger.debug('task_success for __generic_message_handler', end='')
         logger.debug(task_success, end='')
```

### Comparing `lts-mpsmqutils-2.0.4/mpsmqutils/mqutils.py` & `lts_mpsmqutils-2.1.0/mpsmqutils/mqutils.py`

 * *Files identical despite different names*

### Comparing `lts-mpsmqutils-2.0.4/mpsmqutils/tests/test_mqutils.py` & `lts_mpsmqutils-2.1.0/mpsmqutils/tests/test_mqutils.py`

 * *Files identical despite different names*

### Comparing `lts-mpsmqutils-2.0.4/setup.py` & `lts_mpsmqutils-2.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lts-mpsmqutils",
-    version="2.0.4",
+    version="2.1.0",
     description="A set of utilities for communicating with a message queue",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.huit.harvard.edu/LTS/mps-mqutils",
     packages=setuptools.find_packages(),
     install_requires=[
         'lts-mpsjobtracker-mongo',
```

