# Comparing `tmp/jyhelper-1.2.6.tar.gz` & `tmp/jyhelper-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jyhelper-1.2.6.tar", last modified: Wed May 29 10:30:17 2024, max compression
+gzip compressed data, was "jyhelper-1.2.7.tar", last modified: Fri May 31 05:50:35 2024, max compression
```

## Comparing `jyhelper-1.2.6.tar` & `jyhelper-1.2.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 10:30:17.451034 jyhelper-1.2.6/
--rw-rw-rw-   0        0        0     1130 2024-05-29 10:30:17.451034 jyhelper-1.2.6/PKG-INFO
--rw-rw-rw-   0        0        0      820 2023-11-17 09:46:48.000000 jyhelper-1.2.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-29 10:30:17.429526 jyhelper-1.2.6/jyhelper/
--rw-rw-rw-   0        0        0      385 2023-11-17 06:00:40.000000 jyhelper-1.2.6/jyhelper/__init__.py
--rw-rw-rw-   0        0        0     4455 2024-01-30 07:23:11.000000 jyhelper-1.2.6/jyhelper/common.py
--rw-rw-rw-   0        0        0    15771 2024-05-23 02:43:07.000000 jyhelper-1.2.6/jyhelper/db.py
--rw-rw-rw-   0        0        0     5284 2024-01-05 03:38:54.000000 jyhelper-1.2.6/jyhelper/feishuRobot.py
--rw-rw-rw-   0        0        0     3480 2024-05-29 10:25:03.000000 jyhelper-1.2.6/jyhelper/file.py
--rw-rw-rw-   0        0        0     4752 2024-05-29 09:37:08.000000 jyhelper-1.2.6/jyhelper/timeHelper.py
-drwxrwxrwx   0        0        0        0 2024-05-29 10:30:17.448606 jyhelper-1.2.6/jyhelper.egg-info/
--rw-rw-rw-   0        0        0     1130 2024-05-29 10:30:17.000000 jyhelper-1.2.6/jyhelper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      296 2024-05-29 10:30:17.000000 jyhelper-1.2.6/jyhelper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 10:30:17.000000 jyhelper-1.2.6/jyhelper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-29 10:30:17.000000 jyhelper-1.2.6/jyhelper.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-29 10:30:17.000000 jyhelper-1.2.6/jyhelper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-29 10:30:17.451034 jyhelper-1.2.6/setup.cfg
--rw-rw-rw-   0        0        0      718 2024-05-29 09:44:36.000000 jyhelper-1.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:50:35.229159 jyhelper-1.2.7/
+-rw-rw-rw-   0        0        0     1130 2024-05-31 05:50:35.229159 jyhelper-1.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0      820 2023-11-17 09:46:48.000000 jyhelper-1.2.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-31 05:50:35.201324 jyhelper-1.2.7/jyhelper/
+-rw-rw-rw-   0        0        0      385 2023-11-17 06:00:40.000000 jyhelper-1.2.7/jyhelper/__init__.py
+-rw-rw-rw-   0        0        0     8305 2024-05-31 03:42:07.000000 jyhelper-1.2.7/jyhelper/common.py
+-rw-rw-rw-   0        0        0    15771 2024-05-23 02:43:07.000000 jyhelper-1.2.7/jyhelper/db.py
+-rw-rw-rw-   0        0        0     5284 2024-01-05 03:38:54.000000 jyhelper-1.2.7/jyhelper/feishuRobot.py
+-rw-rw-rw-   0        0        0     3480 2024-05-29 10:25:03.000000 jyhelper-1.2.7/jyhelper/file.py
+-rw-rw-rw-   0        0        0     4752 2024-05-29 09:37:08.000000 jyhelper-1.2.7/jyhelper/timeHelper.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:50:35.225219 jyhelper-1.2.7/jyhelper.egg-info/
+-rw-rw-rw-   0        0        0     1130 2024-05-31 05:50:34.000000 jyhelper-1.2.7/jyhelper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      296 2024-05-31 05:50:34.000000 jyhelper-1.2.7/jyhelper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 05:50:34.000000 jyhelper-1.2.7/jyhelper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-31 05:50:34.000000 jyhelper-1.2.7/jyhelper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-31 05:50:34.000000 jyhelper-1.2.7/jyhelper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-31 05:50:35.230156 jyhelper-1.2.7/setup.cfg
+-rw-rw-rw-   0        0        0      718 2024-05-31 05:40:37.000000 jyhelper-1.2.7/setup.py
```

### Comparing `jyhelper-1.2.6/PKG-INFO` & `jyhelper-1.2.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jyhelper
-Version: 1.2.6
+Version: 1.2.7
 Summary: 各种实用、常用的小函数、类
 Home-page: https://pypi.org/project/jyhelper/
 Author: JY
 Author-email: your-email@example.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.0
```

### Comparing `jyhelper-1.2.6/README.md` & `jyhelper-1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `jyhelper-1.2.6/jyhelper/db.py` & `jyhelper-1.2.7/jyhelper/db.py`

 * *Files identical despite different names*

### Comparing `jyhelper-1.2.6/jyhelper/feishuRobot.py` & `jyhelper-1.2.7/jyhelper/feishuRobot.py`

 * *Files identical despite different names*

### Comparing `jyhelper-1.2.6/jyhelper/file.py` & `jyhelper-1.2.7/jyhelper/file.py`

 * *Files identical despite different names*

### Comparing `jyhelper-1.2.6/jyhelper/timeHelper.py` & `jyhelper-1.2.7/jyhelper/timeHelper.py`

 * *Files identical despite different names*

### Comparing `jyhelper-1.2.6/jyhelper.egg-info/PKG-INFO` & `jyhelper-1.2.7/jyhelper.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jyhelper
-Version: 1.2.6
+Version: 1.2.7
 Summary: 各种实用、常用的小函数、类
 Home-page: https://pypi.org/project/jyhelper/
 Author: JY
 Author-email: your-email@example.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.0
```

### Comparing `jyhelper-1.2.6/setup.py` & `jyhelper-1.2.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # @Time : 2023/11/08 18:38 
 # @Author : JY
 
 from setuptools import setup
 
 setup(
     name='jyhelper',
-    version='1.2.6',
+    version='1.2.7',
     packages=['jyhelper'],
     install_requires=[
         'pymysql',
         'requests'
     ],
     description='各种实用、常用的小函数、类',
     long_description=open('README.md',encoding='utf-8').read(),  # 详细描述，通常从 README.md 中读取
```

