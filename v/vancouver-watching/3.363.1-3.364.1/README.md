# Comparing `tmp/vancouver_watching-3.363.1.tar.gz` & `tmp/vancouver_watching-3.364.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vancouver_watching-3.363.1.tar", last modified: Fri May 31 02:51:36 2024, max compression
+gzip compressed data, was "vancouver_watching-3.364.1.tar", last modified: Fri May 31 02:52:26 2024, max compression
```

## Comparing `vancouver_watching-3.363.1.tar` & `vancouver_watching-3.364.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-31 02:51:36.837306 vancouver_watching-3.363.1/
--rw-r--r--   0 kamangir   (502) staff       (20)     7048 2024-05-26 04:17:22.000000 vancouver_watching-3.363.1/LICENSE
--rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-26 04:17:22.000000 vancouver_watching-3.363.1/MANIFEST.in
--rw-r--r--   0 kamangir   (502) staff       (20)     4633 2024-05-31 02:51:36.836735 vancouver_watching-3.363.1/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)     3611 2024-05-26 04:17:22.000000 vancouver_watching-3.363.1/README.md
--rw-r--r--   0 kamangir   (502) staff       (20)       81 2024-05-26 04:17:22.000000 vancouver_watching-3.363.1/pyproject.toml
--rw-r--r--   0 kamangir   (502) staff       (20)      156 2024-05-26 04:17:22.000000 vancouver_watching-3.363.1/requirements.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-31 02:51:36.837396 vancouver_watching-3.363.1/setup.cfg
--rw-r--r--   0 kamangir   (502) staff       (20)      385 2024-05-26 20:40:48.000000 vancouver_watching-3.363.1/setup.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-31 02:51:36.819268 vancouver_watching-3.363.1/vancouver_watching/
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-31 02:51:36.830857 vancouver_watching-3.363.1/vancouver_watching/.abcli/
--rw-r--r--   0 kamangir   (502) staff       (20)      166 2024-05-26 17:36:39.000000 vancouver_watching-3.363.1/vancouver_watching/.abcli/actions.sh
--rw-r--r--   0 kamangir   (502) staff       (20)       74 2024-05-26 17:36:39.000000 vancouver_watching-3.363.1/vancouver_watching/.abcli/aka.sh
--rw-r--r--   0 kamangir   (502) staff       (20)       65 2024-05-26 17:36:39.000000 vancouver_watching-3.363.1/vancouver_watching/.abcli/alias.sh
--rw-r--r--   0 kamangir   (502) staff       (20)     1109 2024-05-26 17:36:39.000000 vancouver_watching-3.363.1/vancouver_watching/.abcli/discover.sh
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-31 02:51:36.831950 vancouver_watching-3.363.1/vancouver_watching/.abcli/discovery/
--rw-r--r--   0 kamangir   (502) staff       (20)      225 2024-05-26 17:36:39.000000 vancouver_watching-3.363.1/vancouver_watching/.abcli/discovery/iran.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      458 2024-05-26 17:36:39.000000 vancouver_watching-3.363.1/vancouver_watching/.abcli/discovery/vancouver.sh
--rw-r--r--   0 kamangir   (502) staff       (20)     2258 2024-05-26 17:36:39.000000 vancouver_watching-3.363.1/vancouver_watching/.abcli/ingest.sh
--rw-r--r--   0 kamangir   (502) staff       (20)     1041 2024-05-26 17:36:39.000000 vancouver_watching-3.363.1/vancouver_watching/.abcli/list.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      982 2024-05-26 17:36:39.000000 vancouver_watching-3.363.1/vancouver_watching/.abcli/openai_vision.sh
--rw-r--r--   0 kamangir   (502) staff       (20)     1763 2024-05-26 17:36:39.000000 vancouver_watching-3.363.1/vancouver_watching/.abcli/process.sh
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-31 02:51:36.834915 vancouver_watching-3.363.1/vancouver_watching/.abcli/tests/
--rw-r--r--   0 kamangir   (502) staff       (20)      549 2024-05-26 17:36:39.000000 vancouver_watching-3.363.1/vancouver_watching/.abcli/tests/ingest.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      341 2024-05-26 17:36:39.000000 vancouver_watching-3.363.1/vancouver_watching/.abcli/tests/list.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      403 2024-05-26 17:36:39.000000 vancouver_watching-3.363.1/vancouver_watching/.abcli/tests/process.sh
--rw-r--r--   0 kamangir   (502) staff       (20)     2618 2024-05-26 17:36:39.000000 vancouver_watching-3.363.1/vancouver_watching/.abcli/update.sh
--rwxr-xr-x   0 kamangir   (502) staff       (20)      745 2024-05-26 17:36:39.000000 vancouver_watching-3.363.1/vancouver_watching/.abcli/vancouver_watching.sh
--rw-r--r--   0 kamangir   (502) staff       (20)     4758 2024-05-26 04:17:22.000000 vancouver_watching-3.363.1/vancouver_watching/QGIS.py
--rw-r--r--   0 kamangir   (502) staff       (20)      151 2024-05-31 02:51:30.000000 vancouver_watching-3.363.1/vancouver_watching/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     1302 2024-05-28 01:10:45.000000 vancouver_watching-3.363.1/vancouver_watching/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     6783 2024-05-26 04:17:22.000000 vancouver_watching-3.363.1/vancouver_watching/area.py
--rw-r--r--   0 kamangir   (502) staff       (20)      127 2024-05-26 04:17:22.000000 vancouver_watching-3.363.1/vancouver_watching/config.env
--rw-r--r--   0 kamangir   (502) staff       (20)      284 2024-05-26 04:17:22.000000 vancouver_watching-3.363.1/vancouver_watching/env.py
--rw-r--r--   0 kamangir   (502) staff       (20)       99 2024-05-26 04:17:22.000000 vancouver_watching-3.363.1/vancouver_watching/logger.py
--rw-r--r--   0 kamangir   (502) staff       (20)      355 2024-05-26 04:17:22.000000 vancouver_watching-3.363.1/vancouver_watching/notebook.py
--rw-r--r--   0 kamangir   (502) staff       (20)       17 2024-05-26 04:17:22.000000 vancouver_watching-3.363.1/vancouver_watching/urls.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-31 02:51:36.835774 vancouver_watching-3.363.1/vancouver_watching.egg-info/
--rw-r--r--   0 kamangir   (502) staff       (20)     4633 2024-05-31 02:51:36.000000 vancouver_watching-3.363.1/vancouver_watching.egg-info/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)     1133 2024-05-31 02:51:36.000000 vancouver_watching-3.363.1/vancouver_watching.egg-info/SOURCES.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-31 02:51:36.000000 vancouver_watching-3.363.1/vancouver_watching.egg-info/dependency_links.txt
--rw-r--r--   0 kamangir   (502) staff       (20)      156 2024-05-31 02:51:36.000000 vancouver_watching-3.363.1/vancouver_watching.egg-info/requires.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       19 2024-05-31 02:51:36.000000 vancouver_watching-3.363.1/vancouver_watching.egg-info/top_level.txt
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-31 02:52:26.804058 vancouver_watching-3.364.1/
+-rw-r--r--   0 kamangir   (502) staff       (20)     7048 2024-05-26 04:17:22.000000 vancouver_watching-3.364.1/LICENSE
+-rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-26 04:17:22.000000 vancouver_watching-3.364.1/MANIFEST.in
+-rw-r--r--   0 kamangir   (502) staff       (20)     4633 2024-05-31 02:52:26.803389 vancouver_watching-3.364.1/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)     3611 2024-05-26 04:17:22.000000 vancouver_watching-3.364.1/README.md
+-rw-r--r--   0 kamangir   (502) staff       (20)       81 2024-05-26 04:17:22.000000 vancouver_watching-3.364.1/pyproject.toml
+-rw-r--r--   0 kamangir   (502) staff       (20)      156 2024-05-26 04:17:22.000000 vancouver_watching-3.364.1/requirements.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-31 02:52:26.804282 vancouver_watching-3.364.1/setup.cfg
+-rw-r--r--   0 kamangir   (502) staff       (20)      385 2024-05-26 20:40:48.000000 vancouver_watching-3.364.1/setup.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-31 02:52:26.794736 vancouver_watching-3.364.1/vancouver_watching/
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-31 02:52:26.800224 vancouver_watching-3.364.1/vancouver_watching/.abcli/
+-rw-r--r--   0 kamangir   (502) staff       (20)      166 2024-05-26 17:36:39.000000 vancouver_watching-3.364.1/vancouver_watching/.abcli/actions.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)       74 2024-05-26 17:36:39.000000 vancouver_watching-3.364.1/vancouver_watching/.abcli/aka.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)       65 2024-05-26 17:36:39.000000 vancouver_watching-3.364.1/vancouver_watching/.abcli/alias.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     1109 2024-05-26 17:36:39.000000 vancouver_watching-3.364.1/vancouver_watching/.abcli/discover.sh
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-31 02:52:26.801228 vancouver_watching-3.364.1/vancouver_watching/.abcli/discovery/
+-rw-r--r--   0 kamangir   (502) staff       (20)      225 2024-05-26 17:36:39.000000 vancouver_watching-3.364.1/vancouver_watching/.abcli/discovery/iran.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      458 2024-05-26 17:36:39.000000 vancouver_watching-3.364.1/vancouver_watching/.abcli/discovery/vancouver.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     2258 2024-05-26 17:36:39.000000 vancouver_watching-3.364.1/vancouver_watching/.abcli/ingest.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     1041 2024-05-26 17:36:39.000000 vancouver_watching-3.364.1/vancouver_watching/.abcli/list.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      982 2024-05-26 17:36:39.000000 vancouver_watching-3.364.1/vancouver_watching/.abcli/openai_vision.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     1763 2024-05-26 17:36:39.000000 vancouver_watching-3.364.1/vancouver_watching/.abcli/process.sh
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-31 02:52:26.802105 vancouver_watching-3.364.1/vancouver_watching/.abcli/tests/
+-rw-r--r--   0 kamangir   (502) staff       (20)      549 2024-05-26 17:36:39.000000 vancouver_watching-3.364.1/vancouver_watching/.abcli/tests/ingest.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      341 2024-05-26 17:36:39.000000 vancouver_watching-3.364.1/vancouver_watching/.abcli/tests/list.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      403 2024-05-26 17:36:39.000000 vancouver_watching-3.364.1/vancouver_watching/.abcli/tests/process.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     2618 2024-05-26 17:36:39.000000 vancouver_watching-3.364.1/vancouver_watching/.abcli/update.sh
+-rwxr-xr-x   0 kamangir   (502) staff       (20)      745 2024-05-26 17:36:39.000000 vancouver_watching-3.364.1/vancouver_watching/.abcli/vancouver_watching.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     4758 2024-05-26 04:17:22.000000 vancouver_watching-3.364.1/vancouver_watching/QGIS.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      151 2024-05-31 02:52:20.000000 vancouver_watching-3.364.1/vancouver_watching/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     1302 2024-05-28 01:10:45.000000 vancouver_watching-3.364.1/vancouver_watching/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     6783 2024-05-26 04:17:22.000000 vancouver_watching-3.364.1/vancouver_watching/area.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      127 2024-05-26 04:17:22.000000 vancouver_watching-3.364.1/vancouver_watching/config.env
+-rw-r--r--   0 kamangir   (502) staff       (20)      284 2024-05-26 04:17:22.000000 vancouver_watching-3.364.1/vancouver_watching/env.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       99 2024-05-26 04:17:22.000000 vancouver_watching-3.364.1/vancouver_watching/logger.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      355 2024-05-26 04:17:22.000000 vancouver_watching-3.364.1/vancouver_watching/notebook.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       17 2024-05-26 04:17:22.000000 vancouver_watching-3.364.1/vancouver_watching/urls.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-31 02:52:26.802513 vancouver_watching-3.364.1/vancouver_watching.egg-info/
+-rw-r--r--   0 kamangir   (502) staff       (20)     4633 2024-05-31 02:52:26.000000 vancouver_watching-3.364.1/vancouver_watching.egg-info/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)     1133 2024-05-31 02:52:26.000000 vancouver_watching-3.364.1/vancouver_watching.egg-info/SOURCES.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-31 02:52:26.000000 vancouver_watching-3.364.1/vancouver_watching.egg-info/dependency_links.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)      156 2024-05-31 02:52:26.000000 vancouver_watching-3.364.1/vancouver_watching.egg-info/requires.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       19 2024-05-31 02:52:26.000000 vancouver_watching-3.364.1/vancouver_watching.egg-info/top_level.txt
```

### Comparing `vancouver_watching-3.363.1/LICENSE` & `vancouver_watching-3.364.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vancouver_watching-3.363.1/PKG-INFO` & `vancouver_watching-3.364.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vancouver_watching
-Version: 3.363.1
+Version: 3.364.1
 Summary: 🌈 Vancouver Watching with AI.
 Home-page: https://github.com/kamangir/vancouver-watching
 Author: Arash Abadpour (Kamangir)
 Author-email: arash@kamangir.net
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Unix Shell
```

### Comparing `vancouver_watching-3.363.1/README.md` & `vancouver_watching-3.364.1/README.md`

 * *Files identical despite different names*

### Comparing `vancouver_watching-3.363.1/vancouver_watching/.abcli/discover.sh` & `vancouver_watching-3.364.1/vancouver_watching/.abcli/discover.sh`

 * *Files identical despite different names*

### Comparing `vancouver_watching-3.363.1/vancouver_watching/.abcli/ingest.sh` & `vancouver_watching-3.364.1/vancouver_watching/.abcli/ingest.sh`

 * *Files identical despite different names*

### Comparing `vancouver_watching-3.363.1/vancouver_watching/.abcli/list.sh` & `vancouver_watching-3.364.1/vancouver_watching/.abcli/list.sh`

 * *Files identical despite different names*

### Comparing `vancouver_watching-3.363.1/vancouver_watching/.abcli/openai_vision.sh` & `vancouver_watching-3.364.1/vancouver_watching/.abcli/openai_vision.sh`

 * *Files identical despite different names*

### Comparing `vancouver_watching-3.363.1/vancouver_watching/.abcli/process.sh` & `vancouver_watching-3.364.1/vancouver_watching/.abcli/process.sh`

 * *Files identical despite different names*

### Comparing `vancouver_watching-3.363.1/vancouver_watching/.abcli/tests/ingest.sh` & `vancouver_watching-3.364.1/vancouver_watching/.abcli/tests/ingest.sh`

 * *Files identical despite different names*

### Comparing `vancouver_watching-3.363.1/vancouver_watching/.abcli/update.sh` & `vancouver_watching-3.364.1/vancouver_watching/.abcli/update.sh`

 * *Files identical despite different names*

### Comparing `vancouver_watching-3.363.1/vancouver_watching/.abcli/vancouver_watching.sh` & `vancouver_watching-3.364.1/vancouver_watching/.abcli/vancouver_watching.sh`

 * *Files identical despite different names*

### Comparing `vancouver_watching-3.363.1/vancouver_watching/QGIS.py` & `vancouver_watching-3.364.1/vancouver_watching/QGIS.py`

 * *Files identical despite different names*

### Comparing `vancouver_watching-3.363.1/vancouver_watching/__main__.py` & `vancouver_watching-3.364.1/vancouver_watching/__main__.py`

 * *Files identical despite different names*

### Comparing `vancouver_watching-3.363.1/vancouver_watching/area.py` & `vancouver_watching-3.364.1/vancouver_watching/area.py`

 * *Files identical despite different names*

### Comparing `vancouver_watching-3.363.1/vancouver_watching.egg-info/PKG-INFO` & `vancouver_watching-3.364.1/vancouver_watching.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vancouver_watching
-Version: 3.363.1
+Version: 3.364.1
 Summary: 🌈 Vancouver Watching with AI.
 Home-page: https://github.com/kamangir/vancouver-watching
 Author: Arash Abadpour (Kamangir)
 Author-email: arash@kamangir.net
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Unix Shell
```

### Comparing `vancouver_watching-3.363.1/vancouver_watching.egg-info/SOURCES.txt` & `vancouver_watching-3.364.1/vancouver_watching.egg-info/SOURCES.txt`

 * *Files identical despite different names*

