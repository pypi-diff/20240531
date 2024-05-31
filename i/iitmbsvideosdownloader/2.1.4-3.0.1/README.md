# Comparing `tmp/iitmbsvideosdownloader-2.1.4.tar.gz` & `tmp/iitmbsvideosdownloader-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iitmbsvideosdownloader-2.1.4.tar", last modified: Sat Sep 23 23:27:17 2023, max compression
+gzip compressed data, was "iitmbsvideosdownloader-3.0.1.tar", max compression
```

## Comparing `iitmbsvideosdownloader-2.1.4.tar` & `iitmbsvideosdownloader-3.0.1.tar`

### file list

```diff
@@ -1,20 +1,10 @@
-drwxrwxrwx   0 savi      (1000) savi      (1000)        0 2023-09-23 23:27:17.854971 iitmbsvideosdownloader-2.1.4/
--rwxrwxrwx   0 savi      (1000) savi      (1000)     1081 2023-02-09 17:48:29.000000 iitmbsvideosdownloader-2.1.4/LICENSE.txt
--rwxrwxrwx   0 savi      (1000) savi      (1000)      228 2023-09-23 23:27:17.854971 iitmbsvideosdownloader-2.1.4/PKG-INFO
--rwxrwxrwx   0 savi      (1000) savi      (1000)     2315 2023-02-11 12:05:04.000000 iitmbsvideosdownloader-2.1.4/README.md
-drwxrwxrwx   0 savi      (1000) savi      (1000)        0 2023-09-23 23:27:17.119352 iitmbsvideosdownloader-2.1.4/iitmbsvideosdownloader/
--rwxrwxrwx   0 savi      (1000) savi      (1000)      348 2023-09-23 21:43:15.000000 iitmbsvideosdownloader-2.1.4/iitmbsvideosdownloader/SITES.py
--rwxrwxrwx   0 savi      (1000) savi      (1000)     3814 2023-02-11 11:11:49.000000 iitmbsvideosdownloader-2.1.4/iitmbsvideosdownloader/SUBJECTS.py
--rwxrwxrwx   0 savi      (1000) savi      (1000)        0 2023-02-08 09:47:19.000000 iitmbsvideosdownloader-2.1.4/iitmbsvideosdownloader/__init__.py
--rwxrwxrwx   0 savi      (1000) savi      (1000)     8370 2023-09-23 23:18:02.000000 iitmbsvideosdownloader-2.1.4/iitmbsvideosdownloader/_downloader.py
--rwxrwxrwx   0 savi      (1000) savi      (1000)     7356 2023-07-29 05:09:28.000000 iitmbsvideosdownloader-2.1.4/iitmbsvideosdownloader/_functions.py
--rwxrwxrwx   0 savi      (1000) savi      (1000)     6109 2023-07-29 04:36:21.000000 iitmbsvideosdownloader-2.1.4/iitmbsvideosdownloader/_iitm.py
--rwxrwxrwx   0 savi      (1000) savi      (1000)     7281 2023-09-23 23:12:29.000000 iitmbsvideosdownloader-2.1.4/iitmbsvideosdownloader/iitmbsvideosdownloader.py
-drwxrwxrwx   0 savi      (1000) savi      (1000)        0 2023-09-23 23:27:17.713925 iitmbsvideosdownloader-2.1.4/iitmbsvideosdownloader.egg-info/
--rwxrwxrwx   0 savi      (1000) savi      (1000)      228 2023-09-23 23:27:10.000000 iitmbsvideosdownloader-2.1.4/iitmbsvideosdownloader.egg-info/PKG-INFO
--rwxrwxrwx   0 savi      (1000) savi      (1000)      527 2023-09-23 23:27:11.000000 iitmbsvideosdownloader-2.1.4/iitmbsvideosdownloader.egg-info/SOURCES.txt
--rwxrwxrwx   0 savi      (1000) savi      (1000)        1 2023-09-23 23:27:10.000000 iitmbsvideosdownloader-2.1.4/iitmbsvideosdownloader.egg-info/dependency_links.txt
--rwxrwxrwx   0 savi      (1000) savi      (1000)       72 2023-09-23 23:27:10.000000 iitmbsvideosdownloader-2.1.4/iitmbsvideosdownloader.egg-info/requires.txt
--rwxrwxrwx   0 savi      (1000) savi      (1000)       23 2023-09-23 23:27:10.000000 iitmbsvideosdownloader-2.1.4/iitmbsvideosdownloader.egg-info/top_level.txt
--rwxrwxrwx   0 savi      (1000) savi      (1000)      107 2023-09-23 23:27:17.886215 iitmbsvideosdownloader-2.1.4/setup.cfg
--rwxrwxrwx   0 savi      (1000) savi      (1000)      500 2023-09-23 23:20:59.000000 iitmbsvideosdownloader-2.1.4/setup.py
+-rwxr-xr-x   0        0        0     2315 2024-05-31 19:38:06.899649 iitmbsvideosdownloader-3.0.1/README.md
+-rwxr-xr-x   0        0        0      348 2024-05-31 19:37:11.188183 iitmbsvideosdownloader-3.0.1/iitmbsvideosdownloader/SITES.py
+-rwxr-xr-x   0        0        0     3893 2024-05-31 19:37:11.192898 iitmbsvideosdownloader-3.0.1/iitmbsvideosdownloader/SUBJECTS.py
+-rw-r--r--   0        0        0        0 2024-05-31 19:32:49.869345 iitmbsvideosdownloader-3.0.1/iitmbsvideosdownloader/__init__.py
+-rwxr-xr-x   0        0        0     8370 2024-05-31 19:37:11.171208 iitmbsvideosdownloader-3.0.1/iitmbsvideosdownloader/_downloader.py
+-rwxr-xr-x   0        0        0     7943 2024-05-31 19:37:11.179558 iitmbsvideosdownloader-3.0.1/iitmbsvideosdownloader/_functions.py
+-rwxr-xr-x   0        0        0     6109 2024-05-31 19:37:11.182448 iitmbsvideosdownloader-3.0.1/iitmbsvideosdownloader/_iitm.py
+-rwxr-xr-x   0        0        0     7281 2024-05-31 19:37:11.185141 iitmbsvideosdownloader-3.0.1/iitmbsvideosdownloader/iitmbsvideosdownloader.py
+-rw-r--r--   0        0        0      363 2024-05-31 19:53:16.650898 iitmbsvideosdownloader-3.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2790 1970-01-01 00:00:00.000000 iitmbsvideosdownloader-3.0.1/PKG-INFO
```

### Comparing `iitmbsvideosdownloader-2.1.4/README.md` & `iitmbsvideosdownloader-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `iitmbsvideosdownloader-2.1.4/iitmbsvideosdownloader/SUBJECTS.py` & `iitmbsvideosdownloader-3.0.1/iitmbsvideosdownloader/SUBJECTS.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,21 +34,27 @@
 ALGORITHMIC_THINKING_IN_BIOINFORMATICS = _Subject("Algorithmic Thinking in Bioinformatics", "bt4001")
 BIG_DATA_AND_BIOLOGICAL_NETWORKS = _Subject("Big Data and Biological Networks", "bt4002")
 SOFTWARE_ENGINEERING = _Subject("Software Engineering", "cs3001")
 SOFTWARE_TESTING = _Subject("Software Testing", "cs3002")
 AI_SEARCH_METHODS_FOR_PROBLEM_SOLVING = _Subject("AI - Search Methods for Problem Solving", "cs3003")
 DEEP_LEARNING = _Subject("Deep Learning", "cs3004")
 INTRODUCTION_TO_CRYPTOGRAPHY_AND_CYBER_SECURITY = _Subject("Introduction to Cryptography and Cyber Security", "cs3005")
-INTRODUCTION_TO_BIG_DATA = _Subject("Introduction to Big Data", "cs3006")
+
 PRIVACY_SECURITY_IN_ONLINE_SOCIAL_MEDIA = _Subject("Privacy and Security in Online Social Media", "cs3007")
 DATA_VISUALIZATION_DESIGN = _Subject("Data Visualization Design", "cs4001")
-SPECIAL_TOPICS_IN_MACHINE_LEARNING_REINFORCEMENT_LEARNING = _Subject(
-    "Special topics in Machine Learning (Reinforcement Learning)", "cs4002")
+
 THEMATIC_IDEAS_IN_DATA_SCIENCE = _Subject("Thematic Ideas in Data Science", "cs4003")
 SEQUENTIAL_DECISION_MAKING = _Subject("Sequential Decision Making", "cs4004")
 SPEECH_TECHNOLOGY = _Subject("Speech Technology", "ee4001")
 STRATEGIES_FOR_PROFESSIONAL_GROWTH = _Subject("Strategies for Professional Growth", "gn3001")
 FINANCIAL_FORENSICS = _Subject("Financial Forensics", "gn3002")
 LINEAR_STATISTICAL_MODELS = _Subject("Linear Statistical Models", "ma2001")
-DESIGN_THINKING_FOR_DATA_DRIVEN_APP_DEVELOPMENT = _Subject("Design Thinking for Data-Driven App Development", "ms3001")
+DESIGN_THINKING_FOR_DATA_DRIVEN_APP_DEVELOPMENT = _Subject("Design Thinking for Data-Driven App Development", "ms4002")
 MARKET_RESEARCH = _Subject("Market Research", "ms3002")
 INDUSTRY_4_0 = _Subject("Industry 4_0", "ms4001")
+
+MATHEMATICAL_THINKING = _Subject("Mathematical Thinking", "ma2001")
+INTRODUCTION_TO_BIG_DATA = _Subject("Introduction to Big Data", "cs4004")
+SPECIAL_TOPICS_IN_MACHINE_LEARNING_REINFORCEMENT_LEARNING = _Subject(
+    "Special topics in Machine Learning (Reinforcement Learning)", "cs4002")
+
+
```

### Comparing `iitmbsvideosdownloader-2.1.4/iitmbsvideosdownloader/_downloader.py` & `iitmbsvideosdownloader-3.0.1/iitmbsvideosdownloader/_downloader.py`

 * *Files identical despite different names*

### Comparing `iitmbsvideosdownloader-2.1.4/iitmbsvideosdownloader/_functions.py` & `iitmbsvideosdownloader-3.0.1/iitmbsvideosdownloader/_functions.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import re
 import time
+import platform
 
 from iitmbsvideosdownloader.SUBJECTS import _Subject
 from selenium.common.exceptions import TimeoutException
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.support.wait import WebDriverWait
 
@@ -103,14 +104,24 @@
             if self.VERBOSE >= verbose:
                 print(s)
 
     def check_file_exists(self, filename):
         return os.path.isfile(os.path.join(self.DOWNLOAD_DIRECTORY, filename))
 
     # gets the newest .mp4 or .webm file in path
+
+    def get_current_os(self):
+        system = platform.system()
+        if system == "Windows":
+            return "windows"
+        elif system == "Darwin":
+            return "mac"
+        else:
+            return "unknown"
+
     def newest(self, path):
         files = os.listdir(path)
         final_files = {}
 
         for f in files:
             if f.endswith(".mp4"):
                 final_files[f] = ".mp4"
@@ -119,16 +130,26 @@
 
         if len(list(final_files.keys())) == 0:
             return None
 
         paths = [os.path.join(path, basename) for basename in final_files.keys()]
 
         newest_file = max(paths, key=os.path.getctime)
-        file_name = newest_file.split("\\")[-1]
-        ext = final_files[file_name]
+
+        current_os = self.get_current_os()
+        if current_os == 'windows':
+            file_name = newest_file.split("\\")[-1]
+            ext = final_files[file_name]
+        elif current_os == 'mac':
+            file_name = newest_file.split("/")[-1]
+            ext = final_files[file_name]
+        else:
+            file_name = newest_file.split("/")[-1]
+            ext = final_files[file_name]
+
         return newest_file, ext
 
     # beautifies name of file, for ex: puts L in starting if it's not there and makes something like L1.2 -
     def beautify_file_name(self, filename):
         if "&amp;" in filename:
             filename = filename.replace("&amp;", "&")
         filename = filename.replace("  ", " ")
```

### Comparing `iitmbsvideosdownloader-2.1.4/iitmbsvideosdownloader/_iitm.py` & `iitmbsvideosdownloader-3.0.1/iitmbsvideosdownloader/_iitm.py`

 * *Files identical despite different names*

### Comparing `iitmbsvideosdownloader-2.1.4/iitmbsvideosdownloader/iitmbsvideosdownloader.py` & `iitmbsvideosdownloader-3.0.1/iitmbsvideosdownloader/iitmbsvideosdownloader.py`

 * *Files identical despite different names*

