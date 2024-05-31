# Comparing `tmp/tb-mqtt-client-1.9.1.tar.gz` & `tmp/tb-mqtt-client-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tb-mqtt-client-1.9.1.tar", last modified: Tue May  7 07:54:12 2024, max compression
+gzip compressed data, was "tb-mqtt-client-1.9.2.tar", last modified: Fri May 31 11:49:24 2024, max compression
```

## Comparing `tb-mqtt-client-1.9.1.tar` & `tb-mqtt-client-1.9.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-05-07 07:54:12.585042 tb-mqtt-client-1.9.1/
--rw-r--r--   0 imbeacon   (501) staff       (20)      549 2024-02-06 08:47:51.000000 tb-mqtt-client-1.9.1/LICENSE
--rw-r--r--   0 imbeacon   (501) staff       (20)    11764 2024-05-07 07:54:12.584793 tb-mqtt-client-1.9.1/PKG-INFO
--rw-r--r--   0 imbeacon   (501) staff       (20)    11196 2024-02-06 08:44:17.000000 tb-mqtt-client-1.9.1/README.md
--rw-r--r--   0 imbeacon   (501) staff       (20)      608 2024-02-06 08:47:51.000000 tb-mqtt-client-1.9.1/__init__.py
--rw-r--r--   0 imbeacon   (501) staff       (20)     3458 2024-02-06 08:47:51.000000 tb-mqtt-client-1.9.1/sdk_utils.py
--rw-r--r--   0 imbeacon   (501) staff       (20)       38 2024-05-07 07:54:12.585088 tb-mqtt-client-1.9.1/setup.cfg
--rw-r--r--   0 imbeacon   (501) staff       (20)     1438 2024-05-07 07:52:58.000000 tb-mqtt-client-1.9.1/setup.py
--rw-r--r--   0 imbeacon   (501) staff       (20)    18630 2024-02-06 08:47:51.000000 tb-mqtt-client-1.9.1/tb_device_http.py
--rw-r--r--   0 imbeacon   (501) staff       (20)    42006 2024-05-07 07:52:40.000000 tb-mqtt-client-1.9.1/tb_device_mqtt.py
--rw-r--r--   0 imbeacon   (501) staff       (20)    11614 2024-03-21 07:53:27.000000 tb-mqtt-client-1.9.1/tb_gateway_mqtt.py
-drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-05-07 07:54:12.584570 tb-mqtt-client-1.9.1/tb_mqtt_client.egg-info/
--rw-r--r--   0 imbeacon   (501) staff       (20)    11764 2024-05-07 07:54:12.000000 tb-mqtt-client-1.9.1/tb_mqtt_client.egg-info/PKG-INFO
--rw-r--r--   0 imbeacon   (501) staff       (20)      304 2024-05-07 07:54:12.000000 tb-mqtt-client-1.9.1/tb_mqtt_client.egg-info/SOURCES.txt
--rw-r--r--   0 imbeacon   (501) staff       (20)        1 2024-05-07 07:54:12.000000 tb-mqtt-client-1.9.1/tb_mqtt_client.egg-info/dependency_links.txt
--rw-r--r--   0 imbeacon   (501) staff       (20)       55 2024-05-07 07:54:12.000000 tb-mqtt-client-1.9.1/tb_mqtt_client.egg-info/requires.txt
--rw-r--r--   0 imbeacon   (501) staff       (20)        1 2024-05-07 07:54:12.000000 tb-mqtt-client-1.9.1/tb_mqtt_client.egg-info/top_level.txt
--rw-r--r--   0 imbeacon   (501) staff       (20)     1704 2024-02-06 08:47:51.000000 tb-mqtt-client-1.9.1/utils.py
+drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-05-31 11:49:24.263305 tb-mqtt-client-1.9.2/
+-rw-r--r--   0 imbeacon   (501) staff       (20)      549 2024-02-06 08:47:51.000000 tb-mqtt-client-1.9.2/LICENSE
+-rw-r--r--   0 imbeacon   (501) staff       (20)    11764 2024-05-31 11:49:24.263019 tb-mqtt-client-1.9.2/PKG-INFO
+-rw-r--r--   0 imbeacon   (501) staff       (20)    11196 2024-02-06 08:44:17.000000 tb-mqtt-client-1.9.2/README.md
+-rw-r--r--   0 imbeacon   (501) staff       (20)      608 2024-02-06 08:47:51.000000 tb-mqtt-client-1.9.2/__init__.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)     3458 2024-02-06 08:47:51.000000 tb-mqtt-client-1.9.2/sdk_utils.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)       38 2024-05-31 11:49:24.263350 tb-mqtt-client-1.9.2/setup.cfg
+-rw-r--r--   0 imbeacon   (501) staff       (20)     1438 2024-05-31 11:44:20.000000 tb-mqtt-client-1.9.2/setup.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)    18630 2024-02-06 08:47:51.000000 tb-mqtt-client-1.9.2/tb_device_http.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)    41884 2024-05-29 06:04:21.000000 tb-mqtt-client-1.9.2/tb_device_mqtt.py
+-rw-r--r--   0 imbeacon   (501) staff       (20)    11625 2024-05-27 12:26:00.000000 tb-mqtt-client-1.9.2/tb_gateway_mqtt.py
+drwxr-xr-x   0 imbeacon   (501) staff       (20)        0 2024-05-31 11:49:24.262759 tb-mqtt-client-1.9.2/tb_mqtt_client.egg-info/
+-rw-r--r--   0 imbeacon   (501) staff       (20)    11764 2024-05-31 11:49:24.000000 tb-mqtt-client-1.9.2/tb_mqtt_client.egg-info/PKG-INFO
+-rw-r--r--   0 imbeacon   (501) staff       (20)      304 2024-05-31 11:49:24.000000 tb-mqtt-client-1.9.2/tb_mqtt_client.egg-info/SOURCES.txt
+-rw-r--r--   0 imbeacon   (501) staff       (20)        1 2024-05-31 11:49:24.000000 tb-mqtt-client-1.9.2/tb_mqtt_client.egg-info/dependency_links.txt
+-rw-r--r--   0 imbeacon   (501) staff       (20)       55 2024-05-31 11:49:24.000000 tb-mqtt-client-1.9.2/tb_mqtt_client.egg-info/requires.txt
+-rw-r--r--   0 imbeacon   (501) staff       (20)        1 2024-05-31 11:49:24.000000 tb-mqtt-client-1.9.2/tb_mqtt_client.egg-info/top_level.txt
+-rw-r--r--   0 imbeacon   (501) staff       (20)     1704 2024-02-06 08:47:51.000000 tb-mqtt-client-1.9.2/utils.py
```

### Comparing `tb-mqtt-client-1.9.1/LICENSE` & `tb-mqtt-client-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tb-mqtt-client-1.9.1/PKG-INFO` & `tb-mqtt-client-1.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tb-mqtt-client
-Version: 1.9.1
+Version: 1.9.2
 Summary: ThingsBoard python client SDK
 Home-page: https://github.com/thingsboard/thingsboard-python-client-sdk
-Download-URL: https://github.com/thingsboard/thingsboard-python-client-sdk/archive/1.9.1.tar.gz
+Download-URL: https://github.com/thingsboard/thingsboard-python-client-sdk/archive/1.9.2.tar.gz
 Author: ThingsBoard
 Author-email: info@thingsboard.io
 License: Apache Software License (Apache Software License 2.0)
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: tb-paho-mqtt-client>=1.6.3
```

### Comparing `tb-mqtt-client-1.9.1/README.md` & `tb-mqtt-client-1.9.2/README.md`

 * *Files identical despite different names*

### Comparing `tb-mqtt-client-1.9.1/__init__.py` & `tb-mqtt-client-1.9.2/__init__.py`

 * *Files identical despite different names*

### Comparing `tb-mqtt-client-1.9.1/sdk_utils.py` & `tb-mqtt-client-1.9.2/sdk_utils.py`

 * *Files identical despite different names*

### Comparing `tb-mqtt-client-1.9.1/setup.py` & `tb-mqtt-client-1.9.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from setuptools import setup
 
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md')) as f:
     long_description = f.read()
 
-VERSION = "1.9.1"
+VERSION = "1.9.2"
 
 setup(
     version=VERSION,
     name="tb-mqtt-client",
     author="ThingsBoard",
     author_email="info@thingsboard.io",
     license="Apache Software License (Apache Software License 2.0)",
```

### Comparing `tb-mqtt-client-1.9.1/tb_device_http.py` & `tb-mqtt-client-1.9.2/tb_device_http.py`

 * *Files identical despite different names*

### Comparing `tb-mqtt-client-1.9.1/tb_device_mqtt.py` & `tb-mqtt-client-1.9.2/tb_device_mqtt.py`

 * *Files 0% similar despite different names*

```diff
@@ -450,19 +450,20 @@
         self.reconnect_delay_set(min_reconnect_delay, timeout)
         self._client.connect(self.__host, self.__port, keepalive=keepalive)
         self._client.loop_start()
         self.__connect_callback = callback
 
     def disconnect(self):
         """Disconnect from ThingsBoard."""
-        self._client.disconnect()
+        result = self._client.disconnect()
         log.debug(self._client)
         log.debug("Disconnecting from ThingsBoard")
         self.__is_connected = False
         self._client.loop_stop()
+        return result
 
     def stop(self):
         self.stopped = True
 
     def _on_message(self, client, userdata, message):
         update_response_pattern = "v2/fw/response/" + str(self.__firmware_request_id) + "/chunk/"
         if message.topic.startswith(update_response_pattern):
@@ -661,17 +662,15 @@
 
     def __sending_thread_main(self):
         while not self.stopped:
             try:
                 if not self.is_connected():
                     sleep(.1)
                     continue
-                if (not self.__rate_limit.check_limit_reached()
-                        and (self.__rate_limit.get_minimal_limit() == 0
-                             or self.__rate_limit.get_minimal_limit() > len(self._client._out_packet))):
+                if not self.__rate_limit.check_limit_reached():
                     if not self.__sending_queue.empty():
                         item = self.__sending_queue.get(False)
                         if item is not None:
                             if item["method"] == TBSendMethod.PUBLISH:
                                 info = self._client.publish(item["topic"], item["data"], qos=item["qos"])
                                 if TBPublishInfo.TB_ERR_QUEUE_SIZE == info.rc:
                                     self.__sending_queue.put_left(item, True)
@@ -679,17 +678,17 @@
                                 self.__responses[item['id']] = {"info": info, "timeout_ts": int(time()) + DEFAULT_TIMEOUT}
                                 self.__rate_limit.add_counter()
                             elif item["method"] == TBSendMethod.SUBSCRIBE:
                                 result = self._client.subscribe(item["topic"], qos=item["qos"])
                                 self.__responses[item['id']] = {"info": result, "timeout_ts": int(time()) + DEFAULT_TIMEOUT}
                                 self.__rate_limit.add_counter()
                     else:
-                        sleep(.1)
+                        sleep(.01)
                 else:
-                    sleep(0.1)
+                    sleep(0.001)
             except Exception as e:
                 log.exception("Error during data sending:", exc_info=e)
                 sleep(1)
 
     def __housekeeping_thread_main(self):
         while not self.stopped:
             if not self.__responses:
@@ -705,15 +704,15 @@
                                 self.__responses.pop(req_id)
                         except (KeyError, AttributeError):
                             pass
                         except (Exception, RuntimeError, ValueError) as e:
                             pass
                             # log.debug("Error during housekeeping sent messages:", exc_info=e)
                         # log.debug("Timeout occurred while waiting for a reply from ThingsBoard!")
-                sleep(0.1)
+                sleep(0.01)
 
     def _subscribe_to_topic(self, topic, callback=None, qos=None, wait_for_result=False, timeout=DEFAULT_TIMEOUT):
         if qos is None:
             qos = self.quality_of_service
         req_id = uuid.uuid4()
         self.__sending_queue.put_left({"topic": topic, "qos": qos, "callback": callback, "id": req_id,
                                        "method": TBSendMethod.SUBSCRIBE}, True)
@@ -726,23 +725,23 @@
         waiting_for_connection_message_time = 0
         while not self.is_connected():
             if self.stopped:
                 return -1, 128
             if time() - waiting_for_connection_message_time > 10.0:
                 log.warning("Waiting for connection to be established before subscribing for data on ThingsBoard!")
                 waiting_for_connection_message_time = time()
-            sleep(0.1)
+            sleep(0.01)
 
         start_time = int(time())
         if wait_for_result:
             while req_id not in list(self.__responses.keys()):
-                if 0 < timeout < int(time()) - start_time:
+                if 0 < timeout < int(time()) - start_time or self.stopped:
                     log.error("Timeout while waiting for a subscribe to ThingsBoard!")
                     return -1, 128
-                sleep(0.1)
+                sleep(0.01)
 
             return self.__responses.pop(req_id)["info"]
 
     def _publish_data(self, data, topic, qos, wait_for_publish=True, high_priority=False, timeout=DEFAULT_TIMEOUT):
         data = dumps(data)
         if qos is None:
             qos = self.quality_of_service
@@ -765,23 +764,23 @@
         waiting_for_connection_message_time = 0
         while not self.is_connected():
             if self.stopped:
                 return TBPublishInfo(paho.MQTTMessageInfo(None))
             if time() - waiting_for_connection_message_time > 10.0:
                 log.warning("Waiting for connection to be established before sending data to ThingsBoard!")
                 waiting_for_connection_message_time = time()
-            sleep(0.1)
+            sleep(0.01)
 
         start_time = int(time())
         if wait_for_publish:
             while req_id not in list(self.__responses.keys()):
                 if 0 < timeout < int(time()) - start_time:
                     log.error("Timeout while waiting for a publish to ThingsBoard!")
                     return TBPublishInfo(paho.MQTTMessageInfo(None))
-                sleep(0.1)
+                sleep(0.01)
 
             return TBPublishInfo(self.__responses.pop(req_id)["info"])
 
     def send_telemetry(self, telemetry, quality_of_service=None, wait_for_publish=True, high_priority=False):
         """Send telemetry to ThingsBoard. The telemetry can be a single dictionary or a list of dictionaries."""
         quality_of_service = quality_of_service if quality_of_service is not None else self.quality_of_service
         if not isinstance(telemetry, list) and not (isinstance(telemetry, dict) and telemetry.get("ts") is not None):
```

### Comparing `tb-mqtt-client-1.9.1/tb_gateway_mqtt.py` & `tb-mqtt-client-1.9.2/tb_gateway_mqtt.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 class TBGatewayAPI:
     pass
 
 
 class TBGatewayMqttClient(TBDeviceMqttClient):
     def __init__(self, host, port=1883, username=None, password=None, gateway=None, quality_of_service=1, client_id="",
                  rate_limit="DEFAULT_RATE_LIMIT"):
-        super().__init__(host, port, username, password, quality_of_service, client_id, rate_limit)
+        super().__init__(host, port, username, password, quality_of_service, client_id, rate_limit=rate_limit)
         self.quality_of_service = quality_of_service
         self.__max_sub_id = 0
         self.__sub_dict = {}
         self.__connected_devices = set("*")
         self.devices_server_side_rpc_request_handler = None
         self._client.on_connect = self._on_connect
         self._client.on_message = self._on_message
```

### Comparing `tb-mqtt-client-1.9.1/tb_mqtt_client.egg-info/PKG-INFO` & `tb-mqtt-client-1.9.2/tb_mqtt_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tb-mqtt-client
-Version: 1.9.1
+Version: 1.9.2
 Summary: ThingsBoard python client SDK
 Home-page: https://github.com/thingsboard/thingsboard-python-client-sdk
-Download-URL: https://github.com/thingsboard/thingsboard-python-client-sdk/archive/1.9.1.tar.gz
+Download-URL: https://github.com/thingsboard/thingsboard-python-client-sdk/archive/1.9.2.tar.gz
 Author: ThingsBoard
 Author-email: info@thingsboard.io
 License: Apache Software License (Apache Software License 2.0)
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: tb-paho-mqtt-client>=1.6.3
```

### Comparing `tb-mqtt-client-1.9.1/utils.py` & `tb-mqtt-client-1.9.2/utils.py`

 * *Files identical despite different names*

