# Comparing `tmp/swagware-0.0.1.tar.gz` & `tmp/swagware-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swagware-0.0.1.tar", last modified: Fri May 31 18:42:19 2024, max compression
+gzip compressed data, was "swagware-0.0.2.tar", last modified: Fri May 31 19:17:57 2024, max compression
```

## Comparing `swagware-0.0.1.tar` & `swagware-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 18:42:19.636149 swagware-0.0.1/
--rw-rw-rw-   0        0        0     1092 2024-05-31 18:34:53.000000 swagware-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      789 2024-05-31 18:42:19.623139 swagware-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       44 2024-05-31 18:35:29.000000 swagware-0.0.1/README.md
--rw-rw-rw-   0        0        0      941 2024-05-31 18:42:03.000000 swagware-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0        7 2024-05-31 18:36:22.000000 swagware-0.0.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-31 18:42:19.637531 swagware-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-31 18:42:19.259141 swagware-0.0.1/swagware/
--rw-rw-rw-   0        0        0       50 2024-05-31 18:37:45.000000 swagware-0.0.1/swagware/__init__.py
--rw-rw-rw-   0        0        0      359 2024-05-31 18:37:42.000000 swagware-0.0.1/swagware/terminal.py
-drwxrwxrwx   0        0        0        0 2024-05-31 18:42:19.611144 swagware-0.0.1/swagware.egg-info/
--rw-rw-rw-   0        0        0      789 2024-05-31 18:42:18.000000 swagware-0.0.1/swagware.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2024-05-31 18:42:18.000000 swagware-0.0.1/swagware.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 18:42:18.000000 swagware-0.0.1/swagware.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-31 18:42:18.000000 swagware-0.0.1/swagware.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-31 18:42:18.000000 swagware-0.0.1/swagware.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-31 19:17:57.577470 swagware-0.0.2/
+-rw-rw-rw-   0        0        0     1092 2024-05-31 18:34:53.000000 swagware-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      801 2024-05-31 19:17:57.426533 swagware-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       44 2024-05-31 18:35:29.000000 swagware-0.0.2/README.md
+-rw-rw-rw-   0        0        0      953 2024-05-31 19:14:38.000000 swagware-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0        7 2024-05-31 18:36:22.000000 swagware-0.0.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-31 19:17:57.577470 swagware-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-31 19:17:56.417848 swagware-0.0.2/swagware/
+-rw-rw-rw-   0        0        0       50 2024-05-31 18:58:46.000000 swagware-0.0.2/swagware/__init__.py
+-rw-rw-rw-   0        0        0      292 2024-05-31 18:54:51.000000 swagware-0.0.2/swagware/terminal.py
+drwxrwxrwx   0        0        0        0 2024-05-31 19:17:57.417859 swagware-0.0.2/swagware.egg-info/
+-rw-rw-rw-   0        0        0      801 2024-05-31 19:17:55.000000 swagware-0.0.2/swagware.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2024-05-31 19:17:55.000000 swagware-0.0.2/swagware.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 19:17:55.000000 swagware-0.0.2/swagware.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-31 19:17:55.000000 swagware-0.0.2/swagware.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-31 19:17:55.000000 swagware-0.0.2/swagware.egg-info/top_level.txt
```

### Comparing `swagware-0.0.1/LICENSE` & `swagware-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `swagware-0.0.1/PKG-INFO` & `swagware-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: swagware
-Version: 0.0.1
-Summary: A Python Library for cool swaggers
+Version: 0.0.2
+Summary: A Python Library for cool swaggers (with rizz)
 Author: codestantin
 License: MIT
 Project-URL: GitHub, https://github.com/codestantindev/swagware
 Keywords: swag,swaggy,nobitches
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `swagware-0.0.1/pyproject.toml` & `swagware-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "swagware"
-description = "A Python Library for cool swaggers"
+description = "A Python Library for cool swaggers (with rizz)"
 requires-python = ">=3.9"
 license = {text = "MIT"}
 readme = "README.md"
 keywords = ["swag", "swaggy", "nobitches"]
 authors = [
     { name = "codestantin" }
 ]
```

### Comparing `swagware-0.0.1/swagware.egg-info/PKG-INFO` & `swagware-0.0.2/swagware.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: swagware
-Version: 0.0.1
-Summary: A Python Library for cool swaggers
+Version: 0.0.2
+Summary: A Python Library for cool swaggers (with rizz)
 Author: codestantin
 License: MIT
 Project-URL: GitHub, https://github.com/codestantindev/swagware
 Keywords: swag,swaggy,nobitches
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

