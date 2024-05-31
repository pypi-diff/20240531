# Comparing `tmp/idbt-0.0.4.tar.gz` & `tmp/idbt-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idbt-0.0.4.tar", last modified: Fri May 31 09:22:45 2024, max compression
+gzip compressed data, was "idbt-0.0.5.tar", last modified: Fri May 31 09:24:41 2024, max compression
```

## Comparing `idbt-0.0.4.tar` & `idbt-0.0.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 09:22:45.009253 idbt-0.0.4/
--rw-r--r--   0 root         (0) root         (0)      876 2024-05-31 09:22:44.999253 idbt-0.0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-21 08:25:20.000000 idbt-0.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 09:22:44.999253 idbt-0.0.4/idbt/
--rw-r--r--   0 root         (0) root         (0)      340 2024-03-21 08:42:30.000000 idbt-0.0.4/idbt/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 09:22:44.999253 idbt-0.0.4/idbt/compiler/
--rw-r--r--   0 root         (0) root         (0)     1217 2024-03-23 09:26:53.000000 idbt-0.0.4/idbt/compiler/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 09:22:44.999253 idbt-0.0.4/idbt/context/
--rw-r--r--   0 root         (0) root         (0)      467 2024-03-26 08:12:43.000000 idbt-0.0.4/idbt/context/i_unit_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 09:22:44.999253 idbt-0.0.4/idbt/events/
--rw-r--r--   0 root         (0) root         (0)     1353 2024-03-28 02:46:30.000000 idbt-0.0.4/idbt/events/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 09:22:44.999253 idbt-0.0.4/idbt/exception/
--rw-r--r--   0 root         (0) root         (0)      235 2024-04-05 04:11:28.000000 idbt-0.0.4/idbt/exception/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 09:22:44.999253 idbt-0.0.4/idbt/graph/
--rw-r--r--   0 root         (0) root         (0)     1310 2024-03-25 08:02:44.000000 idbt-0.0.4/idbt/graph/selector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 09:22:44.999253 idbt-0.0.4/idbt/loader/
--rw-r--r--   0 root         (0) root         (0)     1464 2024-03-27 02:22:53.000000 idbt-0.0.4/idbt/loader/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1398 2024-05-29 07:44:21.000000 idbt-0.0.4/idbt/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 09:22:44.999253 idbt-0.0.4/idbt/manifest/
--rw-r--r--   0 root         (0) root         (0)      838 2024-03-27 02:28:06.000000 idbt-0.0.4/idbt/manifest/__init__.py
--rw-r--r--   0 root         (0) root         (0)       75 2024-03-22 04:44:29.000000 idbt-0.0.4/idbt/manifest/base.py
--rw-r--r--   0 root         (0) root         (0)     1441 2024-04-05 04:11:42.000000 idbt-0.0.4/idbt/manifest/i_unit_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 09:22:44.999253 idbt-0.0.4/idbt/parser/
--rw-r--r--   0 root         (0) root         (0)      282 2024-03-22 03:44:12.000000 idbt-0.0.4/idbt/parser/base.py
--rw-r--r--   0 root         (0) root         (0)     1656 2024-04-05 04:10:15.000000 idbt-0.0.4/idbt/parser/yaml_parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 09:22:44.999253 idbt-0.0.4/idbt/task/
--rw-r--r--   0 root         (0) root         (0)    15204 2024-03-28 03:06:12.000000 idbt-0.0.4/idbt/task/i_unit_test.py
--rw-r--r--   0 root         (0) root         (0)     2296 2024-03-26 10:28:26.000000 idbt-0.0.4/idbt/task/seed.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 09:22:44.999253 idbt-0.0.4/idbt/unittest_func_hook/
--rw-r--r--   0 root         (0) root         (0)     2187 2024-03-21 08:11:56.000000 idbt-0.0.4/idbt/unittest_func_hook/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 09:22:44.999253 idbt-0.0.4/idbt.egg-info/
--rw-r--r--   0 root         (0) root         (0)      876 2024-05-31 09:22:44.000000 idbt-0.0.4/idbt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      597 2024-05-31 09:22:44.000000 idbt-0.0.4/idbt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-31 09:22:44.000000 idbt-0.0.4/idbt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2024-05-31 09:22:44.000000 idbt-0.0.4/idbt.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-27 03:45:04.000000 idbt-0.0.4/idbt.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       17 2024-05-31 09:22:44.000000 idbt-0.0.4/idbt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-05-31 09:22:44.000000 idbt-0.0.4/idbt.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-31 09:22:45.009253 idbt-0.0.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2341 2024-05-24 03:17:08.000000 idbt-0.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 09:24:41.319257 idbt-0.0.5/
+-rw-r--r--   0 root         (0) root         (0)      876 2024-05-31 09:24:41.319257 idbt-0.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-21 08:25:20.000000 idbt-0.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 09:24:41.319257 idbt-0.0.5/idbt/
+-rw-r--r--   0 root         (0) root         (0)      340 2024-03-21 08:42:30.000000 idbt-0.0.5/idbt/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 09:24:41.319257 idbt-0.0.5/idbt/compiler/
+-rw-r--r--   0 root         (0) root         (0)     1217 2024-03-23 09:26:53.000000 idbt-0.0.5/idbt/compiler/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 09:24:41.319257 idbt-0.0.5/idbt/context/
+-rw-r--r--   0 root         (0) root         (0)      467 2024-03-26 08:12:43.000000 idbt-0.0.5/idbt/context/i_unit_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 09:24:41.319257 idbt-0.0.5/idbt/events/
+-rw-r--r--   0 root         (0) root         (0)     1353 2024-03-28 02:46:30.000000 idbt-0.0.5/idbt/events/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 09:24:41.319257 idbt-0.0.5/idbt/exception/
+-rw-r--r--   0 root         (0) root         (0)      235 2024-04-05 04:11:28.000000 idbt-0.0.5/idbt/exception/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 09:24:41.319257 idbt-0.0.5/idbt/graph/
+-rw-r--r--   0 root         (0) root         (0)     1310 2024-03-25 08:02:44.000000 idbt-0.0.5/idbt/graph/selector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 09:24:41.319257 idbt-0.0.5/idbt/loader/
+-rw-r--r--   0 root         (0) root         (0)     1464 2024-03-27 02:22:53.000000 idbt-0.0.5/idbt/loader/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1415 2024-05-31 09:24:18.000000 idbt-0.0.5/idbt/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 09:24:41.319257 idbt-0.0.5/idbt/manifest/
+-rw-r--r--   0 root         (0) root         (0)      838 2024-03-27 02:28:06.000000 idbt-0.0.5/idbt/manifest/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       75 2024-03-22 04:44:29.000000 idbt-0.0.5/idbt/manifest/base.py
+-rw-r--r--   0 root         (0) root         (0)     1441 2024-04-05 04:11:42.000000 idbt-0.0.5/idbt/manifest/i_unit_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 09:24:41.319257 idbt-0.0.5/idbt/parser/
+-rw-r--r--   0 root         (0) root         (0)      282 2024-03-22 03:44:12.000000 idbt-0.0.5/idbt/parser/base.py
+-rw-r--r--   0 root         (0) root         (0)     1656 2024-04-05 04:10:15.000000 idbt-0.0.5/idbt/parser/yaml_parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 09:24:41.319257 idbt-0.0.5/idbt/task/
+-rw-r--r--   0 root         (0) root         (0)    15204 2024-03-28 03:06:12.000000 idbt-0.0.5/idbt/task/i_unit_test.py
+-rw-r--r--   0 root         (0) root         (0)     2296 2024-03-26 10:28:26.000000 idbt-0.0.5/idbt/task/seed.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 09:24:41.319257 idbt-0.0.5/idbt/unittest_func_hook/
+-rw-r--r--   0 root         (0) root         (0)     2187 2024-03-21 08:11:56.000000 idbt-0.0.5/idbt/unittest_func_hook/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 09:24:41.319257 idbt-0.0.5/idbt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      876 2024-05-31 09:24:41.000000 idbt-0.0.5/idbt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      597 2024-05-31 09:24:41.000000 idbt-0.0.5/idbt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-31 09:24:41.000000 idbt-0.0.5/idbt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2024-05-31 09:24:41.000000 idbt-0.0.5/idbt.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-03-27 03:45:04.000000 idbt-0.0.5/idbt.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       17 2024-05-31 09:24:41.000000 idbt-0.0.5/idbt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-05-31 09:24:41.000000 idbt-0.0.5/idbt.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-31 09:24:41.319257 idbt-0.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2341 2024-05-24 03:17:08.000000 idbt-0.0.5/setup.py
```

### Comparing `idbt-0.0.4/PKG-INFO` & `idbt-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idbt
-Version: 0.0.4
+Version: 0.0.5
 Summary: This is inter-k internal tool to help data practice becomes more testable
 Home-page: https://gitlab.inter-k.com/inter-k/internal-software/rnd/idbt
 Author: Bảo Phan
 Author-email: bao.phan1441@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `idbt-0.0.4/idbt/compiler/__init__.py` & `idbt-0.0.5/idbt/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `idbt-0.0.4/idbt/events/types.py` & `idbt-0.0.5/idbt/events/types.py`

 * *Files identical despite different names*

### Comparing `idbt-0.0.4/idbt/graph/selector.py` & `idbt-0.0.5/idbt/graph/selector.py`

 * *Files identical despite different names*

### Comparing `idbt-0.0.4/idbt/loader/__init__.py` & `idbt-0.0.5/idbt/loader/__init__.py`

 * *Files identical despite different names*

### Comparing `idbt-0.0.4/idbt/main.py` & `idbt-0.0.5/idbt/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 @requires.profile
 @requires.project
 @requires.runtime_config
 @requires.manifest
 def unittest(ctx, **kwargs):
     """Inter-k dbt unittest"""
 
-    uuid_str = str(uuid.uuid4())
+    uuid_str = str(uuid.uuid4()).replace("-","_")
     source_schema = f"source_unittest_{uuid_str}"
     i_unit_test_context = IUnitTestContext(
         uuid_str,
         source_schema,
         flags=copy.deepcopy(ctx.obj["flags"]),
         config=copy.deepcopy(ctx.obj["runtime_config"]),
         manifest=copy.deepcopy(ctx.obj["manifest"]),
```

### Comparing `idbt-0.0.4/idbt/manifest/__init__.py` & `idbt-0.0.5/idbt/manifest/__init__.py`

 * *Files identical despite different names*

### Comparing `idbt-0.0.4/idbt/manifest/i_unit_test.py` & `idbt-0.0.5/idbt/manifest/i_unit_test.py`

 * *Files identical despite different names*

### Comparing `idbt-0.0.4/idbt/parser/yaml_parser.py` & `idbt-0.0.5/idbt/parser/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `idbt-0.0.4/idbt/task/i_unit_test.py` & `idbt-0.0.5/idbt/task/i_unit_test.py`

 * *Files identical despite different names*

### Comparing `idbt-0.0.4/idbt/task/seed.py` & `idbt-0.0.5/idbt/task/seed.py`

 * *Files identical despite different names*

### Comparing `idbt-0.0.4/idbt/unittest_func_hook/__init__.py` & `idbt-0.0.5/idbt/unittest_func_hook/__init__.py`

 * *Files identical despite different names*

### Comparing `idbt-0.0.4/idbt.egg-info/PKG-INFO` & `idbt-0.0.5/idbt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idbt
-Version: 0.0.4
+Version: 0.0.5
 Summary: This is inter-k internal tool to help data practice becomes more testable
 Home-page: https://gitlab.inter-k.com/inter-k/internal-software/rnd/idbt
 Author: Bảo Phan
 Author-email: bao.phan1441@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `idbt-0.0.4/idbt.egg-info/SOURCES.txt` & `idbt-0.0.5/idbt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idbt-0.0.4/setup.py` & `idbt-0.0.5/setup.py`

 * *Files identical despite different names*

