# Comparing `tmp/agent-bdi-2.4.5.tar.gz` & `tmp/agent-bdi-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agent-bdi-2.4.5.tar", last modified: Thu May 23 20:29:30 2024, max compression
+gzip compressed data, was "agent-bdi-2.5.0.tar", last modified: Fri May 31 19:15:49 2024, max compression
```

## Comparing `agent-bdi-2.4.5.tar` & `agent-bdi-2.5.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 20:29:30.649205 agent-bdi-2.4.5/
--rw-rw-rw-   0        0        0        0 2023-04-25 11:32:48.000000 agent-bdi-2.4.5/LICENSE.md
--rw-rw-rw-   0        0        0        0 2023-04-25 11:32:48.000000 agent-bdi-2.4.5/MANIFEST.in
--rw-rw-rw-   0        0        0     3202 2024-05-23 20:29:30.648091 agent-bdi-2.4.5/PKG-INFO
--rw-rw-rw-   0        0        0     2650 2023-04-25 11:32:48.000000 agent-bdi-2.4.5/README.md
--rw-rw-rw-   0        0        0       42 2024-05-23 20:29:30.649205 agent-bdi-2.4.5/setup.cfg
--rw-rw-rw-   0        0        0      885 2024-05-23 20:29:05.000000 agent-bdi-2.4.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-23 20:29:30.584122 agent-bdi-2.4.5/src/
--rw-rw-rw-   0        0        0        0 2024-01-04 04:28:19.000000 agent-bdi-2.4.5/src/__init__.py
--rw-rw-rw-   0        0        0      657 2024-01-04 04:28:19.000000 agent-bdi-2.4.5/src/abdi_config.py
-drwxrwxrwx   0        0        0        0 2024-05-23 20:29:30.605547 agent-bdi-2.4.5/src/agent_bdi.egg-info/
--rw-rw-rw-   0        0        0     3202 2024-05-23 20:29:30.000000 agent-bdi-2.4.5/src/agent_bdi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1084 2024-05-23 20:29:30.000000 agent-bdi-2.4.5/src/agent_bdi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 20:29:30.000000 agent-bdi-2.4.5/src/agent_bdi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2024-05-23 20:29:30.000000 agent-bdi-2.4.5/src/agent_bdi.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-23 20:29:30.618125 agent-bdi-2.4.5/src/broker/
--rw-rw-rw-   0        0        0      134 2023-12-25 14:17:27.000000 agent-bdi-2.4.5/src/broker/__init__.py
--rw-rw-rw-   0        0        0      964 2023-12-25 14:17:27.000000 agent-bdi-2.4.5/src/broker/broker_maker.py
--rw-rw-rw-   0        0        0      943 2024-01-04 04:28:19.000000 agent-bdi-2.4.5/src/broker/empty_broker.py
--rw-rw-rw-   0        0        0      645 2023-12-25 14:17:27.000000 agent-bdi-2.4.5/src/broker/message_broker.py
--rw-rw-rw-   0        0        0     2186 2024-03-13 16:08:10.000000 agent-bdi-2.4.5/src/broker/mqtt_broker.py
--rw-rw-rw-   0        0        0      383 2023-12-25 14:17:27.000000 agent-bdi-2.4.5/src/broker/notifier.py
--rw-rw-rw-   0        0        0      903 2024-01-04 04:28:19.000000 agent-bdi-2.4.5/src/broker/redis_broker.py
--rw-rw-rw-   0        0        0      897 2024-01-04 04:28:19.000000 agent-bdi-2.4.5/src/broker/ros_broker.py
--rw-rw-rw-   0        0        0     2651 2024-01-04 04:28:19.000000 agent-bdi-2.4.5/src/broker/ros_noetic_broker.py
-drwxrwxrwx   0        0        0        0 2024-05-23 20:29:30.624774 agent-bdi-2.4.5/src/core/
--rw-rw-rw-   0        0        0      316 2023-05-22 15:55:38.000000 agent-bdi-2.4.5/src/core/Agent.py
--rw-rw-rw-   0        0        0       58 2023-04-25 11:32:48.000000 agent-bdi-2.4.5/src/core/Belief.py
--rw-rw-rw-   0        0        0       52 2023-04-25 11:32:48.000000 agent-bdi-2.4.5/src/core/Desire.py
--rw-rw-rw-   0        0        0       55 2023-04-25 11:32:48.000000 agent-bdi-2.4.5/src/core/Intention.py
--rw-rw-rw-   0        0        0        0 2023-04-25 11:32:48.000000 agent-bdi-2.4.5/src/core/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 20:29:30.632223 agent-bdi-2.4.5/src/holon/
--rw-rw-rw-   0        0        0      116 2023-04-25 11:32:48.000000 agent-bdi-2.4.5/src/holon/Blackboard.py
--rw-rw-rw-   0        0        0      452 2023-05-28 19:59:05.000000 agent-bdi-2.4.5/src/holon/Heart.py
--rw-rw-rw-   0        0        0    10481 2024-05-23 19:22:38.000000 agent-bdi-2.4.5/src/holon/HolonicAgent.py
--rw-rw-rw-   0        0        0       72 2023-04-25 11:32:48.000000 agent-bdi-2.4.5/src/holon/HolonicDesire.py
--rw-rw-rw-   0        0        0       84 2023-04-25 11:32:48.000000 agent-bdi-2.4.5/src/holon/HolonicIntention.py
--rw-rw-rw-   0        0        0        0 2023-12-25 14:17:27.000000 agent-bdi-2.4.5/src/holon/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 20:29:30.641089 agent-bdi-2.4.5/src/holon/logistics/
--rw-rw-rw-   0        0        0        0 2024-02-13 16:04:18.000000 agent-bdi-2.4.5/src/holon/logistics/__init__.py
--rw-rw-rw-   0        0        0      722 2024-04-27 17:02:10.000000 agent-bdi-2.4.5/src/holon/logistics/base_logistic.py
--rw-rw-rw-   0        0        0      356 2024-02-07 10:01:09.000000 agent-bdi-2.4.5/src/holon/logistics/broker_logistic.py
--rw-rw-rw-   0        0        0     5283 2024-05-11 08:16:35.000000 agent-bdi-2.4.5/src/holon/logistics/loading_coordinator.py
--rw-rw-rw-   0        0        0     6780 2024-05-07 17:25:25.000000 agent-bdi-2.4.5/src/holon/logistics/payload_wrapper.py
--rw-rw-rw-   0        0        0     3335 2024-05-18 14:28:14.000000 agent-bdi-2.4.5/src/holon/logistics/request_logistic.py
--rw-rw-rw-   0        0        0     5112 2024-05-18 14:31:46.000000 agent-bdi-2.4.5/src/holon/logistics/response_logistic.py
--rw-rw-rw-   0        0        0       80 2024-01-05 16:48:07.000000 agent-bdi-2.4.5/src/holon/payload.py
-drwxrwxrwx   0        0        0        0 2024-05-23 20:29:30.645865 agent-bdi-2.4.5/tests/
--rw-rw-rw-   0        0        0      404 2024-04-27 15:27:38.000000 agent-bdi-2.4.5/tests/test01.py
--rw-rw-rw-   0        0        0     1837 2024-02-15 11:41:34.000000 agent-bdi-2.4.5/tests/test_loadingbal.py
--rw-rw-rw-   0        0        0     2318 2024-01-06 16:12:29.000000 agent-bdi-2.4.5/tests/test_request.py
--rw-rw-rw-   0        0        0     2754 2024-01-06 16:34:09.000000 agent-bdi-2.4.5/tests/test_send.py
+drwxrwxrwx   0        0        0        0 2024-05-31 19:15:49.935335 agent-bdi-2.5.0/
+-rw-rw-rw-   0        0        0        0 2023-04-25 11:32:48.000000 agent-bdi-2.5.0/LICENSE.md
+-rw-rw-rw-   0        0        0        0 2023-04-25 11:32:48.000000 agent-bdi-2.5.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     3202 2024-05-31 19:15:49.934293 agent-bdi-2.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2650 2023-04-25 11:32:48.000000 agent-bdi-2.5.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-31 19:15:49.935867 agent-bdi-2.5.0/setup.cfg
+-rw-rw-rw-   0        0        0      885 2024-05-31 19:14:13.000000 agent-bdi-2.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 19:15:49.867445 agent-bdi-2.5.0/src/
+-rw-rw-rw-   0        0        0        0 2024-01-04 04:28:19.000000 agent-bdi-2.5.0/src/__init__.py
+-rw-rw-rw-   0        0        0      657 2024-01-04 04:28:19.000000 agent-bdi-2.5.0/src/abdi_config.py
+drwxrwxrwx   0        0        0        0 2024-05-31 19:15:49.889207 agent-bdi-2.5.0/src/agent_bdi.egg-info/
+-rw-rw-rw-   0        0        0     3202 2024-05-31 19:15:49.000000 agent-bdi-2.5.0/src/agent_bdi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1084 2024-05-31 19:15:49.000000 agent-bdi-2.5.0/src/agent_bdi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 19:15:49.000000 agent-bdi-2.5.0/src/agent_bdi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2024-05-31 19:15:49.000000 agent-bdi-2.5.0/src/agent_bdi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-31 19:15:49.901259 agent-bdi-2.5.0/src/broker/
+-rw-rw-rw-   0        0        0      134 2023-12-25 14:17:27.000000 agent-bdi-2.5.0/src/broker/__init__.py
+-rw-rw-rw-   0        0        0      964 2023-12-25 14:17:27.000000 agent-bdi-2.5.0/src/broker/broker_maker.py
+-rw-rw-rw-   0        0        0      943 2024-01-04 04:28:19.000000 agent-bdi-2.5.0/src/broker/empty_broker.py
+-rw-rw-rw-   0        0        0      645 2023-12-25 14:17:27.000000 agent-bdi-2.5.0/src/broker/message_broker.py
+-rw-rw-rw-   0        0        0     2186 2024-03-13 16:08:10.000000 agent-bdi-2.5.0/src/broker/mqtt_broker.py
+-rw-rw-rw-   0        0        0      383 2023-12-25 14:17:27.000000 agent-bdi-2.5.0/src/broker/notifier.py
+-rw-rw-rw-   0        0        0      903 2024-01-04 04:28:19.000000 agent-bdi-2.5.0/src/broker/redis_broker.py
+-rw-rw-rw-   0        0        0      897 2024-01-04 04:28:19.000000 agent-bdi-2.5.0/src/broker/ros_broker.py
+-rw-rw-rw-   0        0        0     2651 2024-01-04 04:28:19.000000 agent-bdi-2.5.0/src/broker/ros_noetic_broker.py
+drwxrwxrwx   0        0        0        0 2024-05-31 19:15:49.907483 agent-bdi-2.5.0/src/core/
+-rw-rw-rw-   0        0        0      316 2023-05-22 15:55:38.000000 agent-bdi-2.5.0/src/core/Agent.py
+-rw-rw-rw-   0        0        0       58 2023-04-25 11:32:48.000000 agent-bdi-2.5.0/src/core/Belief.py
+-rw-rw-rw-   0        0        0       52 2023-04-25 11:32:48.000000 agent-bdi-2.5.0/src/core/Desire.py
+-rw-rw-rw-   0        0        0       55 2023-04-25 11:32:48.000000 agent-bdi-2.5.0/src/core/Intention.py
+-rw-rw-rw-   0        0        0        0 2023-04-25 11:32:48.000000 agent-bdi-2.5.0/src/core/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 19:15:49.916861 agent-bdi-2.5.0/src/holon/
+-rw-rw-rw-   0        0        0      116 2023-04-25 11:32:48.000000 agent-bdi-2.5.0/src/holon/Blackboard.py
+-rw-rw-rw-   0        0        0      452 2023-05-28 19:59:05.000000 agent-bdi-2.5.0/src/holon/Heart.py
+-rw-rw-rw-   0        0        0    12244 2024-05-31 18:51:55.000000 agent-bdi-2.5.0/src/holon/HolonicAgent.py
+-rw-rw-rw-   0        0        0       72 2023-04-25 11:32:48.000000 agent-bdi-2.5.0/src/holon/HolonicDesire.py
+-rw-rw-rw-   0        0        0       84 2023-04-25 11:32:48.000000 agent-bdi-2.5.0/src/holon/HolonicIntention.py
+-rw-rw-rw-   0        0        0        0 2023-12-25 14:17:27.000000 agent-bdi-2.5.0/src/holon/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 19:15:49.926897 agent-bdi-2.5.0/src/holon/logistics/
+-rw-rw-rw-   0        0        0        0 2024-02-13 16:04:18.000000 agent-bdi-2.5.0/src/holon/logistics/__init__.py
+-rw-rw-rw-   0        0        0      722 2024-04-27 17:02:10.000000 agent-bdi-2.5.0/src/holon/logistics/base_logistic.py
+-rw-rw-rw-   0        0        0      356 2024-02-07 10:01:09.000000 agent-bdi-2.5.0/src/holon/logistics/broker_logistic.py
+-rw-rw-rw-   0        0        0     5283 2024-05-11 08:16:35.000000 agent-bdi-2.5.0/src/holon/logistics/loading_coordinator.py
+-rw-rw-rw-   0        0        0     6851 2024-05-29 19:10:38.000000 agent-bdi-2.5.0/src/holon/logistics/payload_wrapper.py
+-rw-rw-rw-   0        0        0     3347 2024-05-31 18:08:28.000000 agent-bdi-2.5.0/src/holon/logistics/request_logistic.py
+-rw-rw-rw-   0        0        0     5193 2024-05-31 18:09:01.000000 agent-bdi-2.5.0/src/holon/logistics/response_logistic.py
+-rw-rw-rw-   0        0        0       80 2024-01-05 16:48:07.000000 agent-bdi-2.5.0/src/holon/payload.py
+drwxrwxrwx   0        0        0        0 2024-05-31 19:15:49.932174 agent-bdi-2.5.0/tests/
+-rw-rw-rw-   0        0        0      404 2024-04-27 15:27:38.000000 agent-bdi-2.5.0/tests/test01.py
+-rw-rw-rw-   0        0        0     1837 2024-02-15 11:41:34.000000 agent-bdi-2.5.0/tests/test_loadingbal.py
+-rw-rw-rw-   0        0        0     2318 2024-01-06 16:12:29.000000 agent-bdi-2.5.0/tests/test_request.py
+-rw-rw-rw-   0        0        0     2754 2024-01-06 16:34:09.000000 agent-bdi-2.5.0/tests/test_send.py
```

### Comparing `agent-bdi-2.4.5/PKG-INFO` & `agent-bdi-2.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agent-bdi
-Version: 2.4.5
+Version: 2.5.0
 Summary: Agent BDI framework
 Home-page: https://github.com/mfshiu/abdi.git
 Author: Ming Fang Shiu
 Author-email: avatar.xu@gmail.com
 Project-URL: Bug Tracker, https://bugtracker.zoho.com/portal/avatardotxugmaildotcom#allprojects/1982079000000043717/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `agent-bdi-2.4.5/README.md` & `agent-bdi-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.4.5/setup.py` & `agent-bdi-2.5.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "agent-bdi",
-    version = "2.4.5",
+    version = "2.5.0",
     author = "Ming Fang Shiu",
     author_email='avatar.xu@gmail.com',
     description='Agent BDI framework',
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/mfshiu/abdi.git",
     project_urls = {
```

### Comparing `agent-bdi-2.4.5/src/abdi_config.py` & `agent-bdi-2.5.0/src/abdi_config.py`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.4.5/src/agent_bdi.egg-info/PKG-INFO` & `agent-bdi-2.5.0/src/agent_bdi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agent-bdi
-Version: 2.4.5
+Version: 2.5.0
 Summary: Agent BDI framework
 Home-page: https://github.com/mfshiu/abdi.git
 Author: Ming Fang Shiu
 Author-email: avatar.xu@gmail.com
 Project-URL: Bug Tracker, https://bugtracker.zoho.com/portal/avatardotxugmaildotcom#allprojects/1982079000000043717/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `agent-bdi-2.4.5/src/agent_bdi.egg-info/SOURCES.txt` & `agent-bdi-2.5.0/src/agent_bdi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.4.5/src/broker/broker_maker.py` & `agent-bdi-2.5.0/src/broker/broker_maker.py`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.4.5/src/broker/empty_broker.py` & `agent-bdi-2.5.0/src/broker/empty_broker.py`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.4.5/src/broker/message_broker.py` & `agent-bdi-2.5.0/src/broker/message_broker.py`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.4.5/src/broker/mqtt_broker.py` & `agent-bdi-2.5.0/src/broker/mqtt_broker.py`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.4.5/src/broker/redis_broker.py` & `agent-bdi-2.5.0/src/broker/redis_broker.py`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.4.5/src/broker/ros_broker.py` & `agent-bdi-2.5.0/src/broker/ros_broker.py`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.4.5/src/broker/ros_noetic_broker.py` & `agent-bdi-2.5.0/src/broker/ros_noetic_broker.py`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.4.5/src/holon/HolonicAgent.py` & `agent-bdi-2.5.0/src/holon/HolonicAgent.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import inspect
+import json
 import logging
 from multiprocessing import Process
 import os
 import signal
 import sys
 import threading
 import time 
@@ -43,15 +44,24 @@
         self.__run_interval_seconds = 1
         
         self.name = f'<{self.__class__.__name__}>'
         self._agent_proc = None        
         self._agent_thread = None        
         self._broker = None
         self._topic_handlers = {}
-        # self._logistics = None
+        self._echo_handlers = {}
+        self.subscribed_topics = set()
+        self.logistics = {}
+        
+        
+    @final
+    def register_logistic(self, logistic:BaseLogistic):
+        if not logistic.job_topic:
+            raise Exception("Logistic must define the job topic.")
+        self.logistics[logistic.job_topic] = logistic
 
 
     @final
     def get_data(self, key:str):
         return self.__repository.get(key)
 
 
@@ -204,24 +214,26 @@
         pass
 
 
     def on_terminated(self):
         pass
     
     
-    def get_logistic(self, topic:str):
-        if topic.startswith("@request."):
-            return RequestLogistic(self)
-        else:
-            return BrokerLogistic(self)
+    # def get_logistic(self, topic:str):
+    #     if topic.startswith("@request."):
+    #         return RequestLogistic(self)
+    #     else:
+    #         return BrokerLogistic(self)
 
 
     @final
     def publish(self, topic, payload=None):
         # logger.debug(f"topic: {topic}, payload: {payload}")
+        if topic in self.logistics:
+            self.logistics[topic].publish(topic, payload)
         return self._broker.publish(topic, payload)
 
 
     @final
     def _publish(self, topic, payload=None):
         return self._broker.publish(topic, payload)
         
@@ -258,50 +270,85 @@
             response_payload = self._request_logistic.pack_for_response(response_payload, request_payload)
             # logger.debug(f"response_payload: {response_payload}, managed_payload: {managed_payload}")
             self.publish(response_topic, response_payload)
         
 
     @final
     def subscribe(self, topic, data_type="str", topic_handler=None):
-        if topic_handler:
-            self.set_topic_handler(topic, topic_handler)
-        return self._broker.subscribe(topic, data_type)
+        logger.debug(f"topic: {topic}, topic_handler: {topic_handler}")
+        self.subscribed_topics.add(topic)
+        
+        if topic in self.logistics:
+            return self.logistics[topic].subscribe(topic, topic_handler, data_type)
+        else:
+            if topic_handler:
+                self.set_topic_handler(topic, topic_handler)
+            return self._broker.subscribe(topic, data_type)
     
     
     def set_topic_handler(self, topic, handler):
         logger.debug(f"{self.short_id}> Set topic handler: {topic}")
         self._topic_handlers[topic] = handler
         
 
     @final
     def terminate(self):
         logger.warn(f"{self.short_id}> {self.name}.")
 
         for a in self.head_agents:
             name = a.__class__.__name__
-            self.publish(topic='terminate', payload=name)
+            # self.publish(topic='terminate', payload=name)
 
         for a in self.body_agents:
             name = a.__class__.__name__
-            self.publish(topic='terminate', payload=name)
+            # self.publish(topic='terminate', payload=name)
 
         self._terminate_lock.set()
 
 
 
 # ==================================
 #  Implementation of BrokerNotifier 
 # ==================================
 
+
+    # For overriding
+    # def on_echo_response(self, resp):
+    #     pass
+    
+    
+    def echo(self, topic, echo_handler):
+        # logger.debug(f"topic: {topic}")
+        self._echo_handlers[topic] = echo_handler
+        self.publish(topic='system.echo', payload=topic)
+
+
+    def _handle_echo(self, topic:str, payload):
+        echo_topic = payload.decode('utf-8')
+        # logger.debug(f"topic: {topic}, echo_topic: {echo_topic}")
+        if echo_topic in self.subscribed_topics:
+            resp = {
+                'topic': echo_topic,
+                'agent_id': self.agent_id,
+            }
+            self.publish('system.echo_response', json.dumps(resp))
+        
+
+    def _handle_echo_response(self, topic:str, payload):
+        resp = json.loads(payload.decode('utf-8'))
+        if echo_handler := self._echo_handlers.get(resp['topic']):
+            echo_handler(resp)
+
     
     def _on_connect(self):
         logger.info(f"{self.short_id}> {self.name} Broker is connected.")
         
-        self.subscribe("echo")
-        self.subscribe("terminate")
+        self.subscribe("system.echo", topic_handler=self._handle_echo)
+        self.subscribe("system.echo_response", topic_handler=self._handle_echo_response)
+        # self.subscribe("terminate")
         self.on_connected()
             
             
     def on_connected(self):
         pass
```

### Comparing `agent-bdi-2.4.5/src/holon/logistics/base_logistic.py` & `agent-bdi-2.5.0/src/holon/logistics/base_logistic.py`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.4.5/src/holon/logistics/loading_coordinator.py` & `agent-bdi-2.5.0/src/holon/logistics/loading_coordinator.py`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.4.5/src/holon/logistics/payload_wrapper.py` & `agent-bdi-2.5.0/src/holon/logistics/payload_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,16 @@
     def __init__(self, agent_id:str):
         self.binary_wrapper = BinaryWrapper(self)
         self.text_wrapper = TextWrapper(self)
         self.agent_id = agent_id
         
         
     def create_response_json(self, response_payload, request_payload):
+        if request_payload is None:
+            request_payload = {}
         response_json = copy.deepcopy(request_payload)
         # response_json = {
         #     "version": VERSION,
         #     "request_id": request_payload["request_id"],
         #     "receiver": request_payload["sender"],
         #     "request_token": request_payload["request_token"]
         # }
```

### Comparing `agent-bdi-2.4.5/src/holon/logistics/request_logistic.py` & `agent-bdi-2.5.0/src/holon/logistics/request_logistic.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 SUBSCRIBE_HEADER = "@response"
 
 
 class RequestLogistic(BaseLogistic):
     __handlers = {}
     
     
-    def __init__(self, agent:HolonicAgent, request_id="", job_topic=None):
+    def __init__(self, agent:HolonicAgent=None, request_id="", job_topic=None):
         self.agent = agent
         self.job_topic = job_topic
         self.request_id = request_id
         self.response_topic_header = f"{SUBSCRIBE_HEADER}.{self.agent.agent_id}.{self.request_id}"
         logger.debug(f"self, agent_id: {self.agent.agent_id}, short_id: {self.agent.short_id}, request_id: {self.request_id}")
         self._payload_wrapper = PayloadWrapper(self.agent.agent_id)
         
@@ -57,16 +57,16 @@
         if not topic:
             if self.job_topic:
                 topic = self.job_topic
             else:
                 raise Exception("The job topic has not been set yet.")
         response_topic = f"{self.response_topic_header}.{topic}"
         logger.debug(f"response_topic: {response_topic}")
-        self.agent.subscribe(response_topic, datatype, self.handle_response)
         RequestLogistic.__handlers[self.response_topic_header] = topic_handler
+        return self.agent.subscribe(response_topic, datatype, self.handle_response)
 
 
     def handle_response(self, topic:str, payload):
         responsed_topic = topic[len(self.response_topic_header)+1:]
         unpacked = self._payload_wrapper.unpack(payload)
         logger.debug(f"topic: {topic}, unpacked: {str(unpacked)[:300]}..")
```

### Comparing `agent-bdi-2.4.5/src/holon/logistics/response_logistic.py` & `agent-bdi-2.5.0/src/holon/logistics/response_logistic.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,39 +30,41 @@
             if self.job_topic:
                 topic = self.job_topic
             else:
                 raise Exception("The job topic has not been set yet.")
 
         request_topic = f"{SUBSCRIBE_HEADER}.{topic}"
         logger.debug(f"request_topic: {request_topic}")
-        self.agent.subscribe(request_topic, datatype, self.handle_request)
 
         if topic_handler:
             self.agent.set_topic_handler(topic, topic_handler)
             
+        return self.agent.subscribe(request_topic, datatype, self.handle_request)
+            
             
     def get_original_topic(self, source_payload):
         topic = ResponseLogistic._deep_find_deepest('request_topic', source_payload)
         return topic[0] if topic else None
 
     
     def _deep_find_deepest(key, dictionary, depth=0):
         deepest_value = None
         max_depth = -1
 
-        if key in dictionary:
-            deepest_value = dictionary[key]
-            max_depth = depth
-
-        for subkey, subvalue in dictionary.items():
-            if isinstance(subvalue, dict):  # Only search in sub-dictionaries
-                found_value, found_depth = ResponseLogistic._deep_find_deepest(key, subvalue, depth + 1)
-                if found_depth > max_depth:
-                    deepest_value = found_value
-                    max_depth = found_depth
+        if dictionary:
+            if key in dictionary:
+                deepest_value = dictionary[key]
+                max_depth = depth
+
+            for subkey, subvalue in dictionary.items():
+                if isinstance(subvalue, dict):  # Only search in sub-dictionaries
+                    found_value, found_depth = ResponseLogistic._deep_find_deepest(key, subvalue, depth + 1)
+                    if found_depth > max_depth:
+                        deepest_value = found_value
+                        max_depth = found_depth
 
         return deepest_value, max_depth
 
 
     def publish(self, topic=None, result=None, source_payload=None):
         if not topic:
             if self.job_topic:
```

### Comparing `agent-bdi-2.4.5/tests/test_loadingbal.py` & `agent-bdi-2.5.0/tests/test_loadingbal.py`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.4.5/tests/test_request.py` & `agent-bdi-2.5.0/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.4.5/tests/test_send.py` & `agent-bdi-2.5.0/tests/test_send.py`

 * *Files identical despite different names*

