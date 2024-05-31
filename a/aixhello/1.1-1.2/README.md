# Comparing `tmp/aixhello-1.1.tar.gz` & `tmp/aixhello-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aixhello-1.1.tar", last modified: Fri May 31 08:36:02 2024, max compression
+gzip compressed data, was "aixhello-1.2.tar", last modified: Fri May 31 09:07:41 2024, max compression
```

## Comparing `aixhello-1.1.tar` & `aixhello-1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 08:36:02.948440 aixhello-1.1/
--rw-rw-rw-   0        0        0     1080 2024-05-31 08:14:25.000000 aixhello-1.1/LICENSE
--rw-rw-rw-   0        0        0       53 2024-05-31 08:13:47.000000 aixhello-1.1/MANIFEST.in
--rw-rw-rw-   0        0        0      573 2024-05-31 08:36:02.947440 aixhello-1.1/PKG-INFO
--rw-rw-rw-   0        0        0      201 2024-05-31 08:12:32.000000 aixhello-1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-31 08:36:02.927442 aixhello-1.1/aixhello/
--rw-rw-rw-   0        0        0       26 2024-05-31 08:07:25.000000 aixhello-1.1/aixhello/__init__.py
--rw-rw-rw-   0        0        0       82 2024-05-31 08:07:18.000000 aixhello-1.1/aixhello/xyello.py
-drwxrwxrwx   0        0        0        0 2024-05-31 08:36:02.947440 aixhello-1.1/aixhello.egg-info/
--rw-rw-rw-   0        0        0      573 2024-05-31 08:36:02.000000 aixhello-1.1/aixhello.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      216 2024-05-31 08:36:02.000000 aixhello-1.1/aixhello.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 08:36:02.000000 aixhello-1.1/aixhello.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-31 08:36:02.000000 aixhello-1.1/aixhello.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-31 08:36:02.958548 aixhello-1.1/setup.cfg
--rw-rw-rw-   0        0        0      532 2024-05-31 08:17:00.000000 aixhello-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 09:07:41.212841 aixhello-1.2/
+-rw-rw-rw-   0        0        0     1080 2024-05-31 08:14:25.000000 aixhello-1.2/LICENSE
+-rw-rw-rw-   0        0        0       86 2024-05-31 08:50:40.000000 aixhello-1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      573 2024-05-31 09:07:41.212841 aixhello-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      201 2024-05-31 08:12:32.000000 aixhello-1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-31 09:07:41.195843 aixhello-1.2/aixhello/
+-rw-rw-rw-   0        0        0       26 2024-05-31 08:07:25.000000 aixhello-1.2/aixhello/__init__.py
+-rw-rw-rw-   0        0        0   259945 2024-05-31 08:57:18.000000 aixhello-1.2/aixhello/xyello.c
+drwxrwxrwx   0        0        0        0 2024-05-31 09:07:41.211850 aixhello-1.2/aixhello.egg-info/
+-rw-rw-rw-   0        0        0      573 2024-05-31 09:07:41.000000 aixhello-1.2/aixhello.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      215 2024-05-31 09:07:41.000000 aixhello-1.2/aixhello.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 09:07:41.000000 aixhello-1.2/aixhello.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-31 09:07:41.000000 aixhello-1.2/aixhello.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-31 09:07:41.218842 aixhello-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      648 2024-05-31 09:04:48.000000 aixhello-1.2/setup.py
```

### Comparing `aixhello-1.1/LICENSE` & `aixhello-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aixhello-1.1/PKG-INFO` & `aixhello-1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aixhello
-Version: 1.1
+Version: 1.2
 Summary: AI HRM Package
 Author: SecureAI
 Author-email: package@xerocai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `aixhello-1.1/aixhello.egg-info/PKG-INFO` & `aixhello-1.2/aixhello.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aixhello
-Version: 1.1
+Version: 1.2
 Summary: AI HRM Package
 Author: SecureAI
 Author-email: package@xerocai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

