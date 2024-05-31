# Comparing `tmp/alibabacloud_rocketmq20220801-1.4.2.tar.gz` & `tmp/alibabacloud_rocketmq20220801-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_rocketmq20220801-1.4.2.tar", last modified: Tue May 28 17:17:03 2024, max compression
+gzip compressed data, was "dist/alibabacloud_rocketmq20220801-1.4.3.tar", last modified: Fri May 31 17:07:05 2024, max compression
```

## Comparing `alibabacloud_rocketmq20220801-1.4.2.tar` & `alibabacloud_rocketmq20220801-1.4.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 17:17:03.000000 alibabacloud_rocketmq20220801-1.4.2/
--rw-r--r--   0 root         (0) root         (0)     1318 2024-05-28 17:17:03.000000 alibabacloud_rocketmq20220801-1.4.2/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-05-28 17:17:03.000000 alibabacloud_rocketmq20220801-1.4.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-05-28 17:17:03.000000 alibabacloud_rocketmq20220801-1.4.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2436 2024-05-28 17:17:03.000000 alibabacloud_rocketmq20220801-1.4.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1115 2024-05-28 17:17:03.000000 alibabacloud_rocketmq20220801-1.4.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1200 2024-05-28 17:17:03.000000 alibabacloud_rocketmq20220801-1.4.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 17:17:03.000000 alibabacloud_rocketmq20220801-1.4.2/alibabacloud_rocketmq20220801/
--rw-r--r--   0 root         (0) root         (0)       21 2024-05-28 17:17:03.000000 alibabacloud_rocketmq20220801-1.4.2/alibabacloud_rocketmq20220801/__init__.py
--rw-r--r--   0 root         (0) root         (0)   105632 2024-05-28 17:17:03.000000 alibabacloud_rocketmq20220801-1.4.2/alibabacloud_rocketmq20220801/client.py
--rw-r--r--   0 root         (0) root         (0)   223043 2024-05-28 17:17:03.000000 alibabacloud_rocketmq20220801-1.4.2/alibabacloud_rocketmq20220801/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 17:17:03.000000 alibabacloud_rocketmq20220801-1.4.2/alibabacloud_rocketmq20220801.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2436 2024-05-28 17:17:03.000000 alibabacloud_rocketmq20220801-1.4.2/alibabacloud_rocketmq20220801.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      460 2024-05-28 17:17:03.000000 alibabacloud_rocketmq20220801-1.4.2/alibabacloud_rocketmq20220801.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 17:17:03.000000 alibabacloud_rocketmq20220801-1.4.2/alibabacloud_rocketmq20220801.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-05-28 17:17:03.000000 alibabacloud_rocketmq20220801-1.4.2/alibabacloud_rocketmq20220801.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2024-05-28 17:17:03.000000 alibabacloud_rocketmq20220801-1.4.2/alibabacloud_rocketmq20220801.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-05-28 17:17:03.000000 alibabacloud_rocketmq20220801-1.4.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2636 2024-05-28 17:17:03.000000 alibabacloud_rocketmq20220801-1.4.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 17:07:05.000000 alibabacloud_rocketmq20220801-1.4.3/
+-rw-r--r--   0 root         (0) root         (0)     1523 2024-05-31 17:07:04.000000 alibabacloud_rocketmq20220801-1.4.3/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-31 17:07:04.000000 alibabacloud_rocketmq20220801-1.4.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-31 17:07:04.000000 alibabacloud_rocketmq20220801-1.4.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2436 2024-05-31 17:07:05.000000 alibabacloud_rocketmq20220801-1.4.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1115 2024-05-31 17:07:04.000000 alibabacloud_rocketmq20220801-1.4.3/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1200 2024-05-31 17:07:04.000000 alibabacloud_rocketmq20220801-1.4.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 17:07:05.000000 alibabacloud_rocketmq20220801-1.4.3/alibabacloud_rocketmq20220801/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-31 17:07:04.000000 alibabacloud_rocketmq20220801-1.4.3/alibabacloud_rocketmq20220801/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   105632 2024-05-31 17:07:04.000000 alibabacloud_rocketmq20220801-1.4.3/alibabacloud_rocketmq20220801/client.py
+-rw-r--r--   0 root         (0) root         (0)   222945 2024-05-31 17:07:04.000000 alibabacloud_rocketmq20220801-1.4.3/alibabacloud_rocketmq20220801/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 17:07:05.000000 alibabacloud_rocketmq20220801-1.4.3/alibabacloud_rocketmq20220801.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2436 2024-05-31 17:07:04.000000 alibabacloud_rocketmq20220801-1.4.3/alibabacloud_rocketmq20220801.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      460 2024-05-31 17:07:04.000000 alibabacloud_rocketmq20220801-1.4.3/alibabacloud_rocketmq20220801.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-31 17:07:04.000000 alibabacloud_rocketmq20220801-1.4.3/alibabacloud_rocketmq20220801.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-05-31 17:07:04.000000 alibabacloud_rocketmq20220801-1.4.3/alibabacloud_rocketmq20220801.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2024-05-31 17:07:04.000000 alibabacloud_rocketmq20220801-1.4.3/alibabacloud_rocketmq20220801.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-31 17:07:05.000000 alibabacloud_rocketmq20220801-1.4.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2636 2024-05-31 17:07:04.000000 alibabacloud_rocketmq20220801-1.4.3/setup.py
```

### Comparing `alibabacloud_rocketmq20220801-1.4.2/ChangeLog.md` & `alibabacloud_rocketmq20220801-1.4.3/ChangeLog.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+2024-05-28 Version: 1.4.2
+- Update API GetInstance: update response param.
+- Update API ListConsumerGroupSubscriptions: update response param.
+- Update API ListTopicSubscriptions: update response param.
+
+
 2024-03-29 Version: 1.4.1
 - Update API GetInstance: update response param.
 - Update API UpdateInstance: update param body.
 
 
 2024-03-28 Version: 1.4.0
 - Support API ListAvailableZones.
```

### Comparing `alibabacloud_rocketmq20220801-1.4.2/LICENSE` & `alibabacloud_rocketmq20220801-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_rocketmq20220801-1.4.2/PKG-INFO` & `alibabacloud_rocketmq20220801-1.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_rocketmq20220801
-Version: 1.4.2
+Version: 1.4.3
 Summary: Alibaba Cloud RocketMQ (20220801) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_rocketmq20220801-1.4.2/README-CN.md` & `alibabacloud_rocketmq20220801-1.4.3/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_rocketmq20220801-1.4.2/README.md` & `alibabacloud_rocketmq20220801-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_rocketmq20220801-1.4.2/alibabacloud_rocketmq20220801/client.py` & `alibabacloud_rocketmq20220801-1.4.3/alibabacloud_rocketmq20220801/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_rocketmq20220801-1.4.2/alibabacloud_rocketmq20220801/models.py` & `alibabacloud_rocketmq20220801-1.4.3/alibabacloud_rocketmq20220801/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -4044,24 +4044,20 @@
         # The filter condition that is used to query instances. If you do not configure this parameter, all instances are queried.
         self.filter = filter
         # The number of the page to return.
         # 
         # Valid values: 1 to 100000000.
         # 
         # If the value that you specify for this parameter is less than 1, the system uses 1 as the value. If the value that you specify for this parameter is greater than 100000000, the system uses 100000000 as the value.
-        # 
-        # This parameter is required.
         self.page_number = page_number
         # The number of entries returned on each page.
         # 
         # Valid values: 10 to 200.
         # 
         # If the value that you specify for this parameter is less than 10, the system uses 10 as the value. If the value that you specify for this parameter is greater than 200, the system uses 200 as the value.
-        # 
-        # This parameter is required.
         self.page_size = page_size
         # The ID of the resource group to which the instance belongs.
         self.resource_group_id = resource_group_id
         # The tags that are used to filter instances.
         self.tags = tags
 
     def validate(self):
```

### Comparing `alibabacloud_rocketmq20220801-1.4.2/alibabacloud_rocketmq20220801.egg-info/PKG-INFO` & `alibabacloud_rocketmq20220801-1.4.3/alibabacloud_rocketmq20220801.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-rocketmq20220801
-Version: 1.4.2
+Version: 1.4.3
 Summary: Alibaba Cloud RocketMQ (20220801) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_rocketmq20220801-1.4.2/setup.py` & `alibabacloud_rocketmq20220801-1.4.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_rocketmq20220801.
 
-Created on 28/05/2024
+Created on 31/05/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_rocketmq20220801"
 NAME = "alibabacloud_rocketmq20220801" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud RocketMQ (20220801) SDK Library for Python"
```

