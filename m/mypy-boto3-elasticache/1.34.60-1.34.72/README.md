# Comparing `tmp/mypy-boto3-elasticache-1.34.60.tar.gz` & `tmp/mypy-boto3-elasticache-1.34.72.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-elasticache-1.34.60.tar", last modified: Mon Mar 11 19:47:09 2024, max compression
+gzip compressed data, was "mypy-boto3-elasticache-1.34.72.tar", last modified: Wed Mar 27 19:47:06 2024, max compression
```

## Comparing `mypy-boto3-elasticache-1.34.60.tar` & `mypy-boto3-elasticache-1.34.72.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 19:47:09.838888 mypy-boto3-elasticache-1.34.60/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-11 19:46:55.000000 mypy-boto3-elasticache-1.34.60/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    17118 2024-03-11 19:47:09.838888 mypy-boto3-elasticache-1.34.60/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15547 2024-03-11 19:46:55.000000 mypy-boto3-elasticache-1.34.60/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 19:47:09.838888 mypy-boto3-elasticache-1.34.60/mypy_boto3_elasticache/
--rw-r--r--   0 runner    (1001) docker     (127)     6183 2024-03-11 19:46:55.000000 mypy-boto3-elasticache-1.34.60/mypy_boto3_elasticache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6183 2024-03-11 19:46:55.000000 mypy-boto3-elasticache-1.34.60/mypy_boto3_elasticache/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-03-11 19:46:55.000000 mypy-boto3-elasticache-1.34.60/mypy_boto3_elasticache/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    77164 2024-03-11 19:46:55.000000 mypy-boto3-elasticache-1.34.60/mypy_boto3_elasticache/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    77161 2024-03-11 19:46:55.000000 mypy-boto3-elasticache-1.34.60/mypy_boto3_elasticache/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    15324 2024-03-11 19:46:56.000000 mypy-boto3-elasticache-1.34.60/mypy_boto3_elasticache/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    15324 2024-03-11 19:46:56.000000 mypy-boto3-elasticache-1.34.60/mypy_boto3_elasticache/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    25234 2024-03-11 19:46:56.000000 mypy-boto3-elasticache-1.34.60/mypy_boto3_elasticache/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    25214 2024-03-11 19:46:56.000000 mypy-boto3-elasticache-1.34.60/mypy_boto3_elasticache/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 19:46:55.000000 mypy-boto3-elasticache-1.34.60/mypy_boto3_elasticache/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    91657 2024-03-11 19:46:58.000000 mypy-boto3-elasticache-1.34.60/mypy_boto3_elasticache/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    91657 2024-03-11 19:46:57.000000 mypy-boto3-elasticache-1.34.60/mypy_boto3_elasticache/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-11 19:46:55.000000 mypy-boto3-elasticache-1.34.60/mypy_boto3_elasticache/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-03-11 19:46:56.000000 mypy-boto3-elasticache-1.34.60/mypy_boto3_elasticache/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5139 2024-03-11 19:46:56.000000 mypy-boto3-elasticache-1.34.60/mypy_boto3_elasticache/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 19:47:09.838888 mypy-boto3-elasticache-1.34.60/mypy_boto3_elasticache.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17118 2024-03-11 19:47:09.000000 mypy-boto3-elasticache-1.34.60/mypy_boto3_elasticache.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-03-11 19:47:09.000000 mypy-boto3-elasticache-1.34.60/mypy_boto3_elasticache.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 19:47:09.000000 mypy-boto3-elasticache-1.34.60/mypy_boto3_elasticache.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 19:47:09.000000 mypy-boto3-elasticache-1.34.60/mypy_boto3_elasticache.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-11 19:47:09.000000 mypy-boto3-elasticache-1.34.60/mypy_boto3_elasticache.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-11 19:47:09.000000 mypy-boto3-elasticache-1.34.60/mypy_boto3_elasticache.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-11 19:47:09.838888 mypy-boto3-elasticache-1.34.60/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-03-11 19:46:55.000000 mypy-boto3-elasticache-1.34.60/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:47:06.034896 mypy-boto3-elasticache-1.34.72/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-27 19:46:50.000000 mypy-boto3-elasticache-1.34.72/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    17118 2024-03-27 19:47:06.034896 mypy-boto3-elasticache-1.34.72/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15547 2024-03-27 19:46:50.000000 mypy-boto3-elasticache-1.34.72/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:47:06.030896 mypy-boto3-elasticache-1.34.72/mypy_boto3_elasticache/
+-rw-r--r--   0 runner    (1001) docker     (127)     6183 2024-03-27 19:46:50.000000 mypy-boto3-elasticache-1.34.72/mypy_boto3_elasticache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6183 2024-03-27 19:46:50.000000 mypy-boto3-elasticache-1.34.72/mypy_boto3_elasticache/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-03-27 19:46:50.000000 mypy-boto3-elasticache-1.34.72/mypy_boto3_elasticache/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77164 2024-03-27 19:46:51.000000 mypy-boto3-elasticache-1.34.72/mypy_boto3_elasticache/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77161 2024-03-27 19:46:51.000000 mypy-boto3-elasticache-1.34.72/mypy_boto3_elasticache/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    15329 2024-03-27 19:46:51.000000 mypy-boto3-elasticache-1.34.72/mypy_boto3_elasticache/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15329 2024-03-27 19:46:51.000000 mypy-boto3-elasticache-1.34.72/mypy_boto3_elasticache/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    25234 2024-03-27 19:46:51.000000 mypy-boto3-elasticache-1.34.72/mypy_boto3_elasticache/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25214 2024-03-27 19:46:51.000000 mypy-boto3-elasticache-1.34.72/mypy_boto3_elasticache/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 19:46:50.000000 mypy-boto3-elasticache-1.34.72/mypy_boto3_elasticache/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    91757 2024-03-27 19:46:53.000000 mypy-boto3-elasticache-1.34.72/mypy_boto3_elasticache/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91757 2024-03-27 19:46:52.000000 mypy-boto3-elasticache-1.34.72/mypy_boto3_elasticache/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-27 19:46:50.000000 mypy-boto3-elasticache-1.34.72/mypy_boto3_elasticache/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-03-27 19:46:51.000000 mypy-boto3-elasticache-1.34.72/mypy_boto3_elasticache/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5139 2024-03-27 19:46:51.000000 mypy-boto3-elasticache-1.34.72/mypy_boto3_elasticache/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:47:06.030896 mypy-boto3-elasticache-1.34.72/mypy_boto3_elasticache.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17118 2024-03-27 19:47:05.000000 mypy-boto3-elasticache-1.34.72/mypy_boto3_elasticache.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-03-27 19:47:06.000000 mypy-boto3-elasticache-1.34.72/mypy_boto3_elasticache.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 19:47:05.000000 mypy-boto3-elasticache-1.34.72/mypy_boto3_elasticache.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 19:47:05.000000 mypy-boto3-elasticache-1.34.72/mypy_boto3_elasticache.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-27 19:47:05.000000 mypy-boto3-elasticache-1.34.72/mypy_boto3_elasticache.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-27 19:47:05.000000 mypy-boto3-elasticache-1.34.72/mypy_boto3_elasticache.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 19:47:06.034896 mypy-boto3-elasticache-1.34.72/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-03-27 19:46:50.000000 mypy-boto3-elasticache-1.34.72/setup.py
```

### Comparing `mypy-boto3-elasticache-1.34.60/LICENSE` & `mypy-boto3-elasticache-1.34.72/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticache-1.34.60/PKG-INFO` & `mypy-boto3-elasticache-1.34.72/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-elasticache
-Version: 1.34.60
-Summary: Type annotations for boto3.ElastiCache 1.34.60 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.72
+Summary: Type annotations for boto3.ElastiCache 1.34.72 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-elasticache.svg?color=blue)](https://pypi.org/project/mypy-boto3-elasticache)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-elasticache)](https://pepy.tech/project/mypy-boto3-elasticache)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElastiCache 1.34.60](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache)
+[boto3.ElastiCache 1.34.72](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-elasticache-1.34.60/README.md` & `mypy-boto3-elasticache-1.34.72/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-elasticache.svg?color=blue)](https://pypi.org/project/mypy-boto3-elasticache)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-elasticache)](https://pepy.tech/project/mypy-boto3-elasticache)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElastiCache 1.34.60](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache)
+[boto3.ElastiCache 1.34.72](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-elasticache-1.34.60/mypy_boto3_elasticache/__init__.py` & `mypy-boto3-elasticache-1.34.72/mypy_boto3_elasticache/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticache-1.34.60/mypy_boto3_elasticache/__init__.pyi` & `mypy-boto3-elasticache-1.34.72/mypy_boto3_elasticache/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticache-1.34.60/mypy_boto3_elasticache/__main__.py` & `mypy-boto3-elasticache-1.34.72/mypy_boto3_elasticache/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ElastiCache 1.34.60\n"
-        "Version:         1.34.60\n"
+        "Type annotations for boto3.ElastiCache 1.34.72\n"
+        "Version:         1.34.72\n"
         "Builder version: 7.23.2\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.60")
+    print("1.34.72")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-elasticache-1.34.60/mypy_boto3_elasticache/client.py` & `mypy-boto3-elasticache-1.34.72/mypy_boto3_elasticache/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticache-1.34.60/mypy_boto3_elasticache/client.pyi` & `mypy-boto3-elasticache-1.34.72/mypy_boto3_elasticache/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticache-1.34.60/mypy_boto3_elasticache/literals.py` & `mypy-boto3-elasticache-1.34.72/mypy_boto3_elasticache/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -322,15 +322,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -510,14 +509,15 @@
     "sts",
     "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy-boto3-elasticache-1.34.60/mypy_boto3_elasticache/literals.pyi` & `mypy-boto3-elasticache-1.34.72/mypy_boto3_elasticache/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -322,15 +322,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -510,14 +509,15 @@
     "sts",
     "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy-boto3-elasticache-1.34.60/mypy_boto3_elasticache/paginator.py` & `mypy-boto3-elasticache-1.34.72/mypy_boto3_elasticache/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticache-1.34.60/mypy_boto3_elasticache/paginator.pyi` & `mypy-boto3-elasticache-1.34.72/mypy_boto3_elasticache/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticache-1.34.60/mypy_boto3_elasticache/type_defs.py` & `mypy-boto3-elasticache-1.34.72/mypy_boto3_elasticache/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -456,22 +456,24 @@
         "EC2SecurityGroupName": NotRequired[str],
         "EC2SecurityGroupOwnerId": NotRequired[str],
     },
 )
 DataStorageTypeDef = TypedDict(
     "DataStorageTypeDef",
     {
-        "Maximum": int,
         "Unit": Literal["GB"],
+        "Maximum": NotRequired[int],
+        "Minimum": NotRequired[int],
     },
 )
 ECPUPerSecondTypeDef = TypedDict(
     "ECPUPerSecondTypeDef",
     {
-        "Maximum": int,
+        "Maximum": NotRequired[int],
+        "Minimum": NotRequired[int],
     },
 )
 CloudWatchLogsDestinationDetailsTypeDef = TypedDict(
     "CloudWatchLogsDestinationDetailsTypeDef",
     {
         "LogGroup": NotRequired[str],
     },
```

### Comparing `mypy-boto3-elasticache-1.34.60/mypy_boto3_elasticache/type_defs.pyi` & `mypy-boto3-elasticache-1.34.72/mypy_boto3_elasticache/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -456,22 +456,24 @@
         "EC2SecurityGroupName": NotRequired[str],
         "EC2SecurityGroupOwnerId": NotRequired[str],
     },
 )
 DataStorageTypeDef = TypedDict(
     "DataStorageTypeDef",
     {
-        "Maximum": int,
         "Unit": Literal["GB"],
+        "Maximum": NotRequired[int],
+        "Minimum": NotRequired[int],
     },
 )
 ECPUPerSecondTypeDef = TypedDict(
     "ECPUPerSecondTypeDef",
     {
-        "Maximum": int,
+        "Maximum": NotRequired[int],
+        "Minimum": NotRequired[int],
     },
 )
 CloudWatchLogsDestinationDetailsTypeDef = TypedDict(
     "CloudWatchLogsDestinationDetailsTypeDef",
     {
         "LogGroup": NotRequired[str],
     },
```

### Comparing `mypy-boto3-elasticache-1.34.60/mypy_boto3_elasticache/waiter.py` & `mypy-boto3-elasticache-1.34.72/mypy_boto3_elasticache/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticache-1.34.60/mypy_boto3_elasticache/waiter.pyi` & `mypy-boto3-elasticache-1.34.72/mypy_boto3_elasticache/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticache-1.34.60/mypy_boto3_elasticache.egg-info/PKG-INFO` & `mypy-boto3-elasticache-1.34.72/mypy_boto3_elasticache.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-elasticache
-Version: 1.34.60
-Summary: Type annotations for boto3.ElastiCache 1.34.60 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.72
+Summary: Type annotations for boto3.ElastiCache 1.34.72 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-elasticache.svg?color=blue)](https://pypi.org/project/mypy-boto3-elasticache)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-elasticache)](https://pepy.tech/project/mypy-boto3-elasticache)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElastiCache 1.34.60](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache)
+[boto3.ElastiCache 1.34.72](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-elasticache-1.34.60/mypy_boto3_elasticache.egg-info/SOURCES.txt` & `mypy-boto3-elasticache-1.34.72/mypy_boto3_elasticache.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticache-1.34.60/setup.py` & `mypy-boto3-elasticache-1.34.72/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-elasticache",
-    version="1.34.60",
+    version="1.34.72",
     packages=["mypy_boto3_elasticache"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.ElastiCache 1.34.60 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for boto3.ElastiCache 1.34.72 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

