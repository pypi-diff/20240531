# Comparing `tmp/swagware-0.0.2.tar.gz` & `tmp/swagware-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swagware-0.0.2.tar", last modified: Fri May 31 19:17:57 2024, max compression
+gzip compressed data, was "swagware-0.0.3.tar", last modified: Fri May 31 19:27:01 2024, max compression
```

## Comparing `swagware-0.0.2.tar` & `swagware-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 19:17:57.577470 swagware-0.0.2/
--rw-rw-rw-   0        0        0     1092 2024-05-31 18:34:53.000000 swagware-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      801 2024-05-31 19:17:57.426533 swagware-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       44 2024-05-31 18:35:29.000000 swagware-0.0.2/README.md
--rw-rw-rw-   0        0        0      953 2024-05-31 19:14:38.000000 swagware-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0        7 2024-05-31 18:36:22.000000 swagware-0.0.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-31 19:17:57.577470 swagware-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-31 19:17:56.417848 swagware-0.0.2/swagware/
--rw-rw-rw-   0        0        0       50 2024-05-31 18:58:46.000000 swagware-0.0.2/swagware/__init__.py
--rw-rw-rw-   0        0        0      292 2024-05-31 18:54:51.000000 swagware-0.0.2/swagware/terminal.py
-drwxrwxrwx   0        0        0        0 2024-05-31 19:17:57.417859 swagware-0.0.2/swagware.egg-info/
--rw-rw-rw-   0        0        0      801 2024-05-31 19:17:55.000000 swagware-0.0.2/swagware.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2024-05-31 19:17:55.000000 swagware-0.0.2/swagware.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 19:17:55.000000 swagware-0.0.2/swagware.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-31 19:17:55.000000 swagware-0.0.2/swagware.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-31 19:17:55.000000 swagware-0.0.2/swagware.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-31 19:27:01.126081 swagware-0.0.3/
+-rw-rw-rw-   0        0        0     1092 2024-05-31 18:34:53.000000 swagware-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      825 2024-05-31 19:27:01.108754 swagware-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       44 2024-05-31 18:35:29.000000 swagware-0.0.3/README.md
+-rw-rw-rw-   0        0        0      953 2024-05-31 19:14:38.000000 swagware-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       16 2024-05-31 19:24:35.000000 swagware-0.0.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-31 19:27:01.127082 swagware-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-31 19:27:00.438329 swagware-0.0.3/swagware/
+-rw-rw-rw-   0        0        0       58 2024-05-31 19:26:22.000000 swagware-0.0.3/swagware/__init__.py
+-rw-rw-rw-   0        0        0      438 2024-05-31 19:25:52.000000 swagware-0.0.3/swagware/terminal.py
+drwxrwxrwx   0        0        0        0 2024-05-31 19:27:01.008283 swagware-0.0.3/swagware.egg-info/
+-rw-rw-rw-   0        0        0      825 2024-05-31 19:26:59.000000 swagware-0.0.3/swagware.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2024-05-31 19:26:59.000000 swagware-0.0.3/swagware.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 19:26:59.000000 swagware-0.0.3/swagware.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-31 19:26:59.000000 swagware-0.0.3/swagware.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-31 19:26:59.000000 swagware-0.0.3/swagware.egg-info/top_level.txt
```

### Comparing `swagware-0.0.2/LICENSE` & `swagware-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `swagware-0.0.2/PKG-INFO` & `swagware-0.0.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swagware
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python Library for cool swaggers (with rizz)
 Author: codestantin
 License: MIT
 Project-URL: GitHub, https://github.com/codestantindev/swagware
 Keywords: swag,swaggy,nobitches
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -14,13 +14,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp
+Requires-Dist: pystyle
 
 # Swagware
 
 ```
 pip install swagware
 ```
```

### Comparing `swagware-0.0.2/pyproject.toml` & `swagware-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `swagware-0.0.2/swagware.egg-info/PKG-INFO` & `swagware-0.0.3/swagware.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swagware
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python Library for cool swaggers (with rizz)
 Author: codestantin
 License: MIT
 Project-URL: GitHub, https://github.com/codestantindev/swagware
 Keywords: swag,swaggy,nobitches
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -14,13 +14,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp
+Requires-Dist: pystyle
 
 # Swagware
 
 ```
 pip install swagware
 ```
```

