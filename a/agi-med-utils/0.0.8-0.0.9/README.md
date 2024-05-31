# Comparing `tmp/agi_med_utils-0.0.8.tar.gz` & `tmp/agi_med_utils-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agi_med_utils-0.0.8.tar", last modified: Wed May 22 09:44:12 2024, max compression
+gzip compressed data, was "agi_med_utils-0.0.9.tar", last modified: Fri May 31 12:46:42 2024, max compression
```

## Comparing `agi_med_utils-0.0.8.tar` & `agi_med_utils-0.0.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-22 09:44:12.924600 agi_med_utils-0.0.8/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       25 2024-05-13 08:33:25.000000 agi_med_utils-0.0.8/MANIFEST.in
--rw-r--r--   0 ivan      (1000) ivan      (1000)      624 2024-05-22 09:44:12.924600 agi_med_utils-0.0.8/PKG-INFO
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      379 2024-05-21 11:23:57.000000 agi_med_utils-0.0.8/README.md
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-22 09:44:12.920600 agi_med_utils-0.0.8/agi_med_utils/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-05-22 09:43:00.000000 agi_med_utils-0.0.8/agi_med_utils/__init__.py
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-22 09:44:12.920600 agi_med_utils-0.0.8/agi_med_utils/config/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)        0 2024-05-13 08:25:13.000000 agi_med_utils-0.0.8/agi_med_utils/config/__init__.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      523 2024-05-13 09:00:12.000000 agi_med_utils-0.0.8/agi_med_utils/config/config.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      232 2024-05-13 09:00:59.000000 agi_med_utils-0.0.8/agi_med_utils/config/singleton.py
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-22 09:44:12.920600 agi_med_utils-0.0.8/agi_med_utils/dig_ass/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)        0 2024-05-22 09:23:32.000000 agi_med_utils-0.0.8/agi_med_utils/dig_ass/__init__.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      104 2024-05-22 09:23:32.000000 agi_med_utils-0.0.8/agi_med_utils/dig_ass/db.py
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-22 09:44:12.920600 agi_med_utils-0.0.8/agi_med_utils/llm/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)        0 2024-05-13 08:25:13.000000 agi_med_utils-0.0.8/agi_med_utils/llm/__init__.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     2004 2024-05-21 08:24:29.000000 agi_med_utils-0.0.8/agi_med_utils/llm/giga_access.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     2538 2024-05-21 08:24:29.000000 agi_med_utils-0.0.8/agi_med_utils/llm/yandex_access.py
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-22 09:44:12.920600 agi_med_utils-0.0.8/agi_med_utils/logger/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)        0 2024-05-22 09:26:17.000000 agi_med_utils-0.0.8/agi_med_utils/logger/__init__.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     1597 2024-05-22 09:40:47.000000 agi_med_utils-0.0.8/agi_med_utils/logger/logger.py
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-22 09:44:12.924600 agi_med_utils-0.0.8/agi_med_utils.egg-info/
--rw-r--r--   0 ivan      (1000) ivan      (1000)      624 2024-05-22 09:44:12.000000 agi_med_utils-0.0.8/agi_med_utils.egg-info/PKG-INFO
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      652 2024-05-22 09:44:12.000000 agi_med_utils-0.0.8/agi_med_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)        1 2024-05-22 09:44:12.000000 agi_med_utils-0.0.8/agi_med_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       74 2024-05-22 09:44:12.000000 agi_med_utils-0.0.8/agi_med_utils.egg-info/requires.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       19 2024-05-22 09:44:12.000000 agi_med_utils-0.0.8/agi_med_utils.egg-info/top_level.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       73 2024-05-22 09:25:32.000000 agi_med_utils-0.0.8/requirements.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       38 2024-05-22 09:44:12.924600 agi_med_utils-0.0.8/setup.cfg
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      778 2024-05-13 08:36:40.000000 agi_med_utils-0.0.8/setup.py
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-22 09:44:12.924600 agi_med_utils-0.0.8/test/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)        0 2024-05-20 10:22:34.000000 agi_med_utils-0.0.8/test/__init__.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       61 2024-05-21 08:24:29.000000 agi_med_utils-0.0.8/test/test_base.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      163 2024-05-22 09:23:32.000000 agi_med_utils-0.0.8/test/test_dig_ass.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      843 2024-05-21 08:24:29.000000 agi_med_utils-0.0.8/test/test_llm.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-31 12:46:42.911489 agi_med_utils-0.0.9/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       25 2024-05-13 08:33:25.000000 agi_med_utils-0.0.9/MANIFEST.in
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      624 2024-05-31 12:46:42.911489 agi_med_utils-0.0.9/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      379 2024-05-21 11:23:57.000000 agi_med_utils-0.0.9/README.md
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-31 12:46:42.907489 agi_med_utils-0.0.9/agi_med_utils/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-05-31 12:46:04.000000 agi_med_utils-0.0.9/agi_med_utils/__init__.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-31 12:46:42.911489 agi_med_utils-0.0.9/agi_med_utils/config/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)        0 2024-05-13 08:25:13.000000 agi_med_utils-0.0.9/agi_med_utils/config/__init__.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      523 2024-05-13 09:00:12.000000 agi_med_utils-0.0.9/agi_med_utils/config/config.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      232 2024-05-13 09:00:59.000000 agi_med_utils-0.0.9/agi_med_utils/config/singleton.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-31 12:46:42.911489 agi_med_utils-0.0.9/agi_med_utils/dig_ass/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)        0 2024-05-22 09:23:32.000000 agi_med_utils-0.0.9/agi_med_utils/dig_ass/__init__.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      104 2024-05-22 09:23:32.000000 agi_med_utils-0.0.9/agi_med_utils/dig_ass/db.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-31 12:46:42.911489 agi_med_utils-0.0.9/agi_med_utils/llm/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)        0 2024-05-13 08:25:13.000000 agi_med_utils-0.0.9/agi_med_utils/llm/__init__.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     2004 2024-05-21 08:24:29.000000 agi_med_utils-0.0.9/agi_med_utils/llm/giga_access.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     2538 2024-05-21 08:24:29.000000 agi_med_utils-0.0.9/agi_med_utils/llm/yandex_access.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-31 12:46:42.911489 agi_med_utils-0.0.9/agi_med_utils/logger/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)        0 2024-05-22 09:26:17.000000 agi_med_utils-0.0.9/agi_med_utils/logger/__init__.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     1304 2024-05-31 12:45:29.000000 agi_med_utils-0.0.9/agi_med_utils/logger/logger.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-31 12:46:42.911489 agi_med_utils-0.0.9/agi_med_utils.egg-info/
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      624 2024-05-31 12:46:42.000000 agi_med_utils-0.0.9/agi_med_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      652 2024-05-31 12:46:42.000000 agi_med_utils-0.0.9/agi_med_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)        1 2024-05-31 12:46:42.000000 agi_med_utils-0.0.9/agi_med_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       74 2024-05-31 12:46:42.000000 agi_med_utils-0.0.9/agi_med_utils.egg-info/requires.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       19 2024-05-31 12:46:42.000000 agi_med_utils-0.0.9/agi_med_utils.egg-info/top_level.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       73 2024-05-22 09:25:32.000000 agi_med_utils-0.0.9/requirements.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       38 2024-05-31 12:46:42.911489 agi_med_utils-0.0.9/setup.cfg
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      778 2024-05-13 08:36:40.000000 agi_med_utils-0.0.9/setup.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-31 12:46:42.911489 agi_med_utils-0.0.9/test/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)        0 2024-05-20 10:22:34.000000 agi_med_utils-0.0.9/test/__init__.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       61 2024-05-21 08:24:29.000000 agi_med_utils-0.0.9/test/test_base.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      163 2024-05-22 09:23:32.000000 agi_med_utils-0.0.9/test/test_dig_ass.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      843 2024-05-21 08:24:29.000000 agi_med_utils-0.0.9/test/test_llm.py
```

### Comparing `agi_med_utils-0.0.8/PKG-INFO` & `agi_med_utils-0.0.9/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agi_med_utils
-Version: 0.0.8
+Version: 0.0.9
 Summary: Utils for agi-med team
 Author: AGI-MED-TEAM
 Requires-Dist: pyyaml==6.0.1
 Requires-Dist: gigachat==0.1.17
 Requires-Dist: requests==2.31.0
 Requires-Dist: python-json-logger==2.0.7
```

### Comparing `agi_med_utils-0.0.8/agi_med_utils/config/config.py` & `agi_med_utils-0.0.9/agi_med_utils/config/config.py`

 * *Files identical despite different names*

### Comparing `agi_med_utils-0.0.8/agi_med_utils/llm/giga_access.py` & `agi_med_utils-0.0.9/agi_med_utils/llm/giga_access.py`

 * *Files identical despite different names*

### Comparing `agi_med_utils-0.0.8/agi_med_utils/llm/yandex_access.py` & `agi_med_utils-0.0.9/agi_med_utils/llm/yandex_access.py`

 * *Files identical despite different names*

### Comparing `agi_med_utils-0.0.8/agi_med_utils/logger/logger.py` & `agi_med_utils-0.0.9/agi_med_utils/logger/logger.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,22 +8,18 @@
 
 class JsonFormatter(jsonlogger.JsonFormatter):
     pass
     ####
     # additional json formatting possible
     ####
 
-    # def add_fields(self, log_record, record, message_dict):
-    #     super(JsonFormatter, self).add_fields(log_record, record, message_dict)
-    #     if not log_record.get('timestamp'):
-    #         log_record['timestamp'] = record.created
-    #     if log_record.get('level'):
-    #         log_record['level'] = log_record['level'].upper()
-    #     else:
-    #         log_record['level'] = record.levelname
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+        self.json_ensure_ascii = False
 
 
 @singleton
 class LoggerSingleton:
     def __init__(self, loggerConfig) -> None:
         self.logger = logging.getLogger(name=loggerConfig['name'])
         self.logger.setLevel(loggerConfig['level_common'])
```

### Comparing `agi_med_utils-0.0.8/agi_med_utils.egg-info/PKG-INFO` & `agi_med_utils-0.0.9/agi_med_utils.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agi_med_utils
-Version: 0.0.8
+Version: 0.0.9
 Summary: Utils for agi-med team
 Author: AGI-MED-TEAM
 Requires-Dist: pyyaml==6.0.1
 Requires-Dist: gigachat==0.1.17
 Requires-Dist: requests==2.31.0
 Requires-Dist: python-json-logger==2.0.7
```

### Comparing `agi_med_utils-0.0.8/agi_med_utils.egg-info/SOURCES.txt` & `agi_med_utils-0.0.9/agi_med_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `agi_med_utils-0.0.8/setup.py` & `agi_med_utils-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `agi_med_utils-0.0.8/test/test_llm.py` & `agi_med_utils-0.0.9/test/test_llm.py`

 * *Files identical despite different names*

