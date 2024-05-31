# Comparing `tmp/UnityPredict-0.1.8.tar.gz` & `tmp/UnityPredict-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UnityPredict-0.1.8.tar", last modified: Fri May 31 07:30:33 2024, max compression
+gzip compressed data, was "UnityPredict-0.1.9.tar", last modified: Fri May 31 07:31:02 2024, max compression
```

## Comparing `UnityPredict-0.1.8.tar` & `UnityPredict-0.1.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 07:30:33.211995 UnityPredict-0.1.8/
--rw-rw-rw-   0        0        0     6878 2024-05-31 07:30:33.210957 UnityPredict-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     6774 2024-05-31 07:26:06.000000 UnityPredict-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-31 07:30:33.183605 UnityPredict-0.1.8/UnityPredict/
--rw-rw-rw-   0        0        0      445 2024-05-31 07:20:00.000000 UnityPredict-0.1.8/UnityPredict/AppEngineConfig.py
--rw-rw-rw-   0        0        0     3088 2024-05-31 07:28:44.000000 UnityPredict-0.1.8/UnityPredict/Models.py
--rw-rw-rw-   0        0        0     3052 2024-05-31 07:28:53.000000 UnityPredict-0.1.8/UnityPredict/Platform.py
--rw-rw-rw-   0        0        0    18367 2024-05-31 07:29:28.000000 UnityPredict-0.1.8/UnityPredict/UnityPredictLocalHost.py
--rw-rw-rw-   0        0        0       53 2024-05-31 07:26:06.000000 UnityPredict-0.1.8/UnityPredict/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-31 07:30:33.210957 UnityPredict-0.1.8/UnityPredict.egg-info/
--rw-rw-rw-   0        0        0     6878 2024-05-31 07:30:33.000000 UnityPredict-0.1.8/UnityPredict.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2024-05-31 07:30:33.000000 UnityPredict-0.1.8/UnityPredict.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 07:30:33.000000 UnityPredict-0.1.8/UnityPredict.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-05-31 07:30:33.000000 UnityPredict-0.1.8/UnityPredict.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-31 07:30:33.211995 UnityPredict-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      441 2024-05-31 07:30:32.000000 UnityPredict-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 07:31:02.945121 UnityPredict-0.1.9/
+-rw-rw-rw-   0        0        0     6878 2024-05-31 07:31:02.945121 UnityPredict-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     6774 2024-05-31 07:26:06.000000 UnityPredict-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-31 07:31:02.918110 UnityPredict-0.1.9/UnityPredict/
+-rw-rw-rw-   0        0        0      445 2024-05-31 07:20:00.000000 UnityPredict-0.1.9/UnityPredict/AppEngineConfig.py
+-rw-rw-rw-   0        0        0     3088 2024-05-31 07:28:44.000000 UnityPredict-0.1.9/UnityPredict/Models.py
+-rw-rw-rw-   0        0        0     3052 2024-05-31 07:28:53.000000 UnityPredict-0.1.9/UnityPredict/Platform.py
+-rw-rw-rw-   0        0        0    18367 2024-05-31 07:29:28.000000 UnityPredict-0.1.9/UnityPredict/UnityPredictLocalHost.py
+-rw-rw-rw-   0        0        0       53 2024-05-31 07:26:06.000000 UnityPredict-0.1.9/UnityPredict/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 07:31:02.944121 UnityPredict-0.1.9/UnityPredict.egg-info/
+-rw-rw-rw-   0        0        0     6878 2024-05-31 07:31:02.000000 UnityPredict-0.1.9/UnityPredict.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      305 2024-05-31 07:31:02.000000 UnityPredict-0.1.9/UnityPredict.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 07:31:02.000000 UnityPredict-0.1.9/UnityPredict.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-05-31 07:31:02.000000 UnityPredict-0.1.9/UnityPredict.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-31 07:31:02.945121 UnityPredict-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      441 2024-05-31 07:31:02.000000 UnityPredict-0.1.9/setup.py
```

### Comparing `UnityPredict-0.1.8/PKG-INFO` & `UnityPredict-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UnityPredict
-Version: 0.1.8
+Version: 0.1.9
 Description-Content-Type: text/markdown
 
 # UnityPredict Local App Engine Creator
 
 ## Introduction
 
 This library allows you to create App Engines in your local system and finetune the engines before updating it to the [ModelCentral](https://modelcentral.ai) repositories.
```

### Comparing `UnityPredict-0.1.8/README.md` & `UnityPredict-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `UnityPredict-0.1.8/UnityPredict/Models.py` & `UnityPredict-0.1.9/UnityPredict/Models.py`

 * *Files identical despite different names*

### Comparing `UnityPredict-0.1.8/UnityPredict/Platform.py` & `UnityPredict-0.1.9/UnityPredict/Platform.py`

 * *Files identical despite different names*

### Comparing `UnityPredict-0.1.8/UnityPredict/UnityPredictLocalHost.py` & `UnityPredict-0.1.9/UnityPredict/UnityPredictLocalHost.py`

 * *Files identical despite different names*

### Comparing `UnityPredict-0.1.8/UnityPredict.egg-info/PKG-INFO` & `UnityPredict-0.1.9/UnityPredict.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UnityPredict
-Version: 0.1.8
+Version: 0.1.9
 Description-Content-Type: text/markdown
 
 # UnityPredict Local App Engine Creator
 
 ## Introduction
 
 This library allows you to create App Engines in your local system and finetune the engines before updating it to the [ModelCentral](https://modelcentral.ai) repositories.
```

