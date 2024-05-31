# Comparing `tmp/libABCD-0.3.0.tar.gz` & `tmp/libabcd-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libABCD-0.3.0.tar", last modified: Thu Mar 16 13:00:18 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `libABCD-0.3.0.tar` & `libabcd-2.1.0.tar`

### file list

```diff
@@ -1,17 +1,9 @@
-drwxr-xr-x   0 bertou     (501) staff       (20)        0 2023-03-16 13:00:18.694548 libABCD-0.3.0/
--rw-r--r--   0 bertou     (501) staff       (20)      325 2023-03-16 12:36:41.000000 libABCD-0.3.0/.gitignore
--rw-r--r--   0 bertou     (501) staff       (20)     2011 2023-03-16 12:42:02.000000 libABCD-0.3.0/CHANGELOG.md
--rw-r--r--   0 bertou     (501) staff       (20)     1155 2020-06-03 18:26:48.000000 libABCD-0.3.0/LICENSE
--rw-r--r--   0 bertou     (501) staff       (20)     1105 2023-03-16 13:00:18.694354 libABCD-0.3.0/PKG-INFO
--rw-r--r--   0 bertou     (501) staff       (20)      575 2023-03-16 12:36:41.000000 libABCD-0.3.0/README.md
--rw-r--r--   0 bertou     (501) staff       (20)       68 2023-03-16 12:36:41.000000 libABCD-0.3.0/TODO.md
-drwxr-xr-x   0 bertou     (501) staff       (20)        0 2023-03-16 13:00:18.693334 libABCD-0.3.0/libABCD/
--rw-r--r--   0 bertou     (501) staff       (20)    13021 2023-03-16 12:36:41.000000 libABCD-0.3.0/libABCD/__init__.py
-drwxr-xr-x   0 bertou     (501) staff       (20)        0 2023-03-16 13:00:18.694169 libABCD-0.3.0/libABCD.egg-info/
--rw-r--r--   0 bertou     (501) staff       (20)     1105 2023-03-16 13:00:18.000000 libABCD-0.3.0/libABCD.egg-info/PKG-INFO
--rw-r--r--   0 bertou     (501) staff       (20)      232 2023-03-16 13:00:18.000000 libABCD-0.3.0/libABCD.egg-info/SOURCES.txt
--rw-r--r--   0 bertou     (501) staff       (20)        1 2023-03-16 13:00:18.000000 libABCD-0.3.0/libABCD.egg-info/dependency_links.txt
--rw-r--r--   0 bertou     (501) staff       (20)        1 2020-06-03 23:21:10.000000 libABCD-0.3.0/libABCD.egg-info/not-zip-safe
--rw-r--r--   0 bertou     (501) staff       (20)        8 2023-03-16 13:00:18.000000 libABCD-0.3.0/libABCD.egg-info/top_level.txt
--rw-r--r--   0 bertou     (501) staff       (20)       38 2023-03-16 13:00:18.694592 libABCD-0.3.0/setup.cfg
--rw-r--r--   0 bertou     (501) staff       (20)      617 2023-03-16 12:58:46.000000 libABCD-0.3.0/setup.py
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 libabcd-2.1.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 libabcd-2.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 libabcd-2.1.0/TODO.md
+-rw-r--r--   0        0        0    12469 2020-02-02 00:00:00.000000 libabcd-2.1.0/libABCD/__init__.py
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 libabcd-2.1.0/.gitignore
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 libabcd-2.1.0/LICENSE
+-rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 libabcd-2.1.0/README.md
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 libabcd-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 libabcd-2.1.0/PKG-INFO
```

### Comparing `libABCD-0.3.0/CHANGELOG.md` & `libabcd-2.1.0/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,42 @@
 # Changelog
 
 Released versions of libABCD
 
+## [2.1.0] - 2024-05-31
+
+### Added
+
+- gitlab CI/CD auto deploy to pypi
+
+### Changed
+
+- callbacks added with `libabcd.add_callback()` can now receive empty payloads
+
+## [2.0] - 2024-03-27
+
+### Added
+
+- New logging handler (ABCDHandler) added to a root logger
+
+### Removed
+
+- ABCDLogger
+
+
+## [1.0.0] - 2023-07-18
+
+### Added
+
+- installation instructions in README.md
+
+### Changed
+
+- "info" level of loggings now goes through MQTT
+
 
 ## [0.3.0] - 2023-03-16
 
 ### Added
 
 - naming for unique clients
 - logging handled by class ABCDlog
@@ -62,12 +93,15 @@
 - S.py example logger
 - run.py example run manager (with damicm.json config file)
 - exec-client.py cient accepting and executing python commands (highly unsecure!)
 - send.py simple message sender example
 - README, LICENSE, and pypi setup for pip(3)
 
 [unreleased]: https://gitlab.com/bertou/libabcd/-/compare/v0.1.2...master
+[2.1.0]: https://gitlab.com/bertou/libabcd/-/tags/v2.1.0
+[2.0]: https://gitlab.com/bertou/libabcd/-/tags/v2.0
+[1.0.0]: https://gitlab.com/bertou/libabcd/-/tags/v1.0.0
 [0.3.0]: https://gitlab.com/bertou/libabcd/-/tags/v0.3.0
 [0.2.0]: https://gitlab.com/bertou/libabcd/-/tags/v0.2.0
 [0.1.2]: https://gitlab.com/bertou/libabcd/-/tags/v0.1.2
 [0.1.1]: https://gitlab.com/bertou/libabcd/-/tags/v0.1.1
 [0.1]: https://gitlab.com/bertou/libabcd/-/tags/v0.1
```

### Comparing `libABCD-0.3.0/LICENSE` & `libabcd-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `libABCD-0.3.0/libABCD/__init__.py` & `libabcd-2.1.0/libABCD/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import paho.mqtt.client as mqtt
-import logging.config
 import logging
 from logging.handlers import TimedRotatingFileHandler
 import configparser, json, os, sys, time
 
 
 ### logging in UTC
 logging.Formatter.converter = time.gmtime
@@ -17,51 +16,56 @@
 bInitialized = False # whether `init` has been run
 bReportStatus = False # whether to publish the status when on and off
 bPingPong = False # whether to subscribe and answer to ping calls
 host = 'localhost'  # mqtt defaults
 port = 1883
 subscriptions = []
 mqttreconnections = 0
+logger = logging.getLogger(name)
 
 
-def _init_logger(loglevel, fileloglevel):
+def _init_logger(loglevel, fileloglevel, mqttp):
 
-    ### log configuration
-    global logger
-
-    # Initialize logger
-    _logger = logging.getLogger(name)
+    # configure the root logger
+    rlogger = logging.getLogger()    
 
     # global logging level
-    _logger.setLevel(logging.DEBUG)
+    rlogger.setLevel(logging.DEBUG)
 
     # create formatter
     formatter = logging.Formatter('%(asctime)s - %(name)-10s - %(levelname)-8s - %(message)s')
 
     # create console handler
     ch = logging.StreamHandler(sys.stdout)
     ch.setLevel(loglevel)
     ch.setFormatter(formatter)
-    _logger.addHandler(ch)
+    rlogger.addHandler(ch)
 
     # create file handler if requested
     if fileloglevel:
         # file log directory
         logdir = ("log")
         if not os.path.isdir(logdir):
             os.makedirs(logdir)
 
         # create file handler
         fh = TimedRotatingFileHandler(
             os.path.join(logdir, name+'.log'), when='midnight', utc=True, delay=True)
         fh.setLevel(fileloglevel)
         fh.setFormatter(formatter)
-        _logger.addHandler(fh)
+        rlogger.addHandler(fh)
     
-    logger = ABCDlog()
+    # add an ABCDHandler if publishing is on
+    if mqttp:
+        ph = ABCDHandler(level=logging.INFO)
+        ph.setFormatter(formatter)
+        rlogger.addHandler(ph)
+
+    global logger
+    logger = logging.getLogger(name)
 
 
 def _init_mqtt(publisher, listener, username, password):
 
     ### start mqtt client(s)
     global mqttp, mqttl
 
@@ -86,15 +90,15 @@
 
 ### mqtt generic callbacks
 def _on_connect(mqttc: mqtt.Client, userdata, flags, rc):
 
     id = mqttc._client_id.decode()
 
     if rc == 0:
-        logger.info(f"mqtt client {id} connected to server")
+        logger.debug(f"mqtt client {id} connected to server")
         logger.debug(f'FLAGS: {flags}')
 
         if bReportStatus:
             # report on
             msg = _format_msg('on')
             mqttc.publish(f'status/{id}', msg, retain=True)
 
@@ -112,23 +116,24 @@
     if mqttreconnections > 1:
         for sub in subscriptions:
             logger.debug(f'Subscribing to {sub} (on_connect)')
             mqttc.subscribe(sub, qos=2)
 
 
 def _on_publish(mqttc, userdata, mid):
-    logger.debug(f"published mid {mid}")
+    # logger.debug(f"published mid {mid}")
+    pass
 
 
 def _on_disconnect(mqttc: mqtt.Client, userdata, rc):
     
     id = mqttc._client_id.decode()
 
     if rc == 0:
-        logger.info(f"mqtt client {id} disconnected from server")
+        logger.debug(f"mqtt client {id} disconnected from server")
     else:
         logger.warning(f"mqtt client {id} unexpected disconnection, rc={rc}")
 
 
 def _on_message(mqttc: mqtt.Client, userdata, msg: mqtt.MQTTMessage):
 
     logger.debug(f'Unhandled message on topic {msg.topic}: {msg.payload}')
@@ -195,15 +200,15 @@
         name = name+'_'+str(pid)
 
     # report status flag
     global bReportStatus
     bReportStatus = report_status
 
     # start logging
-    _init_logger(loglevel, fileloglevel)
+    _init_logger(loglevel, fileloglevel, publisher)
 
     # ping-pong flag
     global bPingPong
     if pingpong and (not listener or not publisher):
         logger.warning('Both `publisher` and `listener` should be True for pingpong to work.')
     bPingPong = pingpong
 
@@ -241,16 +246,15 @@
     if connect:
         mqconnect()
 
 
 def _mqconnect(mqttc: mqtt.Client):
     if bReportStatus:
         # set will if client dies unexpectedly
-        msg = _format_msg('off')
-        mqttc.will_set(f'status/{mqttc._client_id.decode()}', msg, retain=True)
+        mqttc.will_set(f'status/{mqttc._client_id.decode()}', None, retain=True)
     mqttc.connect(host, port)
     mqttc.loop_start()
 
 
 def _mqdisconnect(mqttc: mqtt.Client):
     
     if bReportStatus:
@@ -309,14 +313,15 @@
         what to publish. 
     **kwargs:
         keyword arguments passed to mqttp.publish
     """
 
     if mqttp:
         msg = _format_msg(payload)
+        logger.debug(f'Publishing "{msg}" to topic "{topic}"')
         try:
             mqttp.publish(topic, msg, **kwargs)
             time.sleep(.001)
         except Exception as e:
             logger.error(f'Following exception raised trying to publish: {e}')
     else:
         logger.error('mqtt publisher was not initialized. Cannot publish.')
@@ -354,37 +359,42 @@
         logger.debug(f'Unsubscribing from {topic}')
         mqttl.unsubscribe(topic)
         
     else:
         logger.warning('Listener was not initialized. Cannot unsubscribe.')
 
 
-def add_callback(sub, func):
+def add_callback(sub, func, allow_empty_payload=False):
     """
     Add a callback `func` to message received in topic(s) `sub`. `func`
     must have the following signature: `func(msg, topic)` with `msg` 
     the payload of the received message and `topic` its topic.
     """
 
     def _msg_callback(mqttc: mqtt.Client, userdata, msg: mqtt.MQTTMessage):
 
         # decode and json-load msg
         dmsg = msg.payload.decode()
-        try:
-            jmsg = json.loads(dmsg)
-        except Exception as e:
-            logger.warning(f'Could not json-load following payload: {dmsg}. Exception: {e}.')
-            return
 
-        if 'from' not in jmsg or 'timestamp' not in jmsg or 'payload' not in jmsg:
-            logger.warning(f'Wrong format in following message: {jmsg}. Nothing will happen.')
-            return
+        if dmsg == '':
+            if not allow_empty_payload:
+                return      # ignore empty payloads
+            jmsg = None
+
         else:
-            elapsed = time.time() - jmsg['timestamp']
-            logger.debug(f'Received payload {jmsg["payload"]} sent from {jmsg["from"]} {elapsed:.1f} s ago.')
+            try:
+                jmsg = json.loads(dmsg)
+            except Exception as e:
+                logger.warning(f'Could not json-load following payload: {dmsg}. Exception: {e}.')
+                return
+
+            if 'from' not in jmsg or 'timestamp' not in jmsg \
+                                                    or 'payload' not in jmsg:
+                logger.warning(f'Wrong format in following message: {jmsg}. Nothing will happen.')
+                return
         
         try:
             func(jmsg, msg.topic)
         except Exception as e:
             logger.error(f'Exception raised when processing message {jmsg}: {e}.')
 
 
@@ -400,49 +410,20 @@
 
 
 def _pingpong(msg, topic):
 
     publish('pongs')
 
 
-class ABCDlog:
-
-    def __init__(self, suffix=None):
-
-        # try:
-        fullname = name
-        # except NameError:
-        #     raise RuntimeError('Cannot initialize ABCDlog before running `libABCD.init()`')
-
-        if suffix:
-            fullname += '.'+suffix
-        self._logger = logging.getLogger(fullname)
-    
-    def debug(self, msg, *args, **kwargs):
-        self._logger.debug(msg, *args, **kwargs)
-
-    def info(self, msg, *args, **kwargs):
-        self._logger.info(msg, *args, **kwargs)
-
-    def extra(self, msg, *args, **kwargs):
-        self._logger.info(msg, *args, **kwargs)
-        if mqttp:
-            publish(f"logs/{name}", {"level": "info", "msg": msg})
-
-    def warning(self, msg, *args, **kwargs):
-        self._logger.warning(msg, *args, **kwargs)
-        if mqttp: 
-            publish(f"logs/{name}", {"level": "warning", "msg": msg})
-
-    def error(self, msg, *args, **kwargs):
-        self._logger.error(msg, *args, **kwargs)
-        if mqttp:
-            publish(f"logs/{name}", {"level": "error", "msg": msg})
-
-    def critical(self, msg, *args, **kwargs):
-        self._logger.critical(msg, *args, **kwargs)
-        if mqttp:
-            publish(f"logs/{name}", {"level": "critical", "msg": msg})
+class ABCDHandler(logging.Handler):
 
+    def __init__(self, level: int or str = 0) -> None: # type: ignore
+        super().__init__(level)
+        self.name = name
 
-### pre-initialization logger
-logger = ABCDlog()
+    def emit(self, record: logging.LogRecord):
+        
+        try:
+            publish(f'logs/{record.name}', 
+                    {'level': record.levelname, 'msg': record.msg})
+        except Exception:
+            self.handleError(record)
```

