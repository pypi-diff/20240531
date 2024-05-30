# Comparing `tmp/pyutmodelv2-2.1.5.tar.gz` & `tmp/pyutmodelv2-2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyutmodelv2-2.1.5.tar", last modified: Sat Feb  3 15:08:20 2024, max compression
+gzip compressed data, was "pyutmodelv2-2.1.6.tar", last modified: Thu May 30 23:04:32 2024, max compression
```

## Comparing `pyutmodelv2-2.1.5.tar` & `pyutmodelv2-2.1.6.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-02-03 15:08:20.311759 pyutmodelv2-2.1.5/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2022-07-23 19:00:15.000000 pyutmodelv2-2.1.5/LICENSE
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2404 2024-02-03 15:08:20.311564 pyutmodelv2-2.1.5/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1941 2023-12-17 20:07:31.000000 pyutmodelv2-2.1.5/README.md
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      775 2024-01-09 04:25:20.000000 pyutmodelv2-2.1.5/pyproject.toml
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2024-02-03 15:08:20.311805 pyutmodelv2-2.1.5/setup.cfg
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-02-03 15:08:20.303454 pyutmodelv2-2.1.5/src/
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-02-03 15:08:20.309000 pyutmodelv2-2.1.5/src/pyutmodelv2/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      535 2023-12-12 03:53:31.000000 pyutmodelv2-2.1.5/src/pyutmodelv2/PyutActor.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2901 2024-02-03 15:00:52.000000 pyutmodelv2-2.1.5/src/pyutmodelv2/PyutClass.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      916 2023-12-08 21:47:34.000000 pyutmodelv2-2.1.5/src/pyutmodelv2/PyutClassCommon.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      951 2023-12-13 16:57:08.000000 pyutmodelv2-2.1.5/src/pyutmodelv2/PyutField.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1400 2023-12-11 17:12:25.000000 pyutmodelv2-2.1.5/src/pyutmodelv2/PyutInterface.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3186 2023-12-12 04:05:20.000000 pyutmodelv2-2.1.5/src/pyutmodelv2/PyutLink.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1560 2023-12-12 03:34:40.000000 pyutmodelv2-2.1.5/src/pyutmodelv2/PyutLinkedObject.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3102 2023-12-13 16:47:14.000000 pyutmodelv2-2.1.5/src/pyutmodelv2/PyutMethod.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      150 2023-12-10 21:14:19.000000 pyutmodelv2-2.1.5/src/pyutmodelv2/PyutModelTypes.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      426 2023-12-06 03:33:34.000000 pyutmodelv2-2.1.5/src/pyutmodelv2/PyutModifier.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      533 2023-12-07 03:25:37.000000 pyutmodelv2-2.1.5/src/pyutmodelv2/PyutNote.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      438 2023-12-12 03:09:47.000000 pyutmodelv2-2.1.5/src/pyutmodelv2/PyutObject.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      720 2023-12-13 16:55:10.000000 pyutmodelv2-2.1.5/src/pyutmodelv2/PyutParameter.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      524 2023-12-09 19:52:57.000000 pyutmodelv2-2.1.5/src/pyutmodelv2/PyutSDInstance.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2682 2023-12-09 19:02:21.000000 pyutmodelv2-2.1.5/src/pyutmodelv2/PyutSDMessage.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      504 2023-12-06 02:26:17.000000 pyutmodelv2-2.1.5/src/pyutmodelv2/PyutText.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      209 2023-12-06 15:49:24.000000 pyutmodelv2-2.1.5/src/pyutmodelv2/PyutType.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      237 2023-12-09 17:26:22.000000 pyutmodelv2-2.1.5/src/pyutmodelv2/PyutUseCase.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       45 2023-12-05 19:04:19.000000 pyutmodelv2-2.1.5/src/pyutmodelv2/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       27 2024-01-17 18:45:49.000000 pyutmodelv2-2.1.5/src/pyutmodelv2/_version.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-02-03 15:08:20.311204 pyutmodelv2-2.1.5/src/pyutmodelv2/enumerations/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      262 2024-01-12 03:20:53.000000 pyutmodelv2-2.1.5/src/pyutmodelv2/enumerations/PyutDisplayMethods.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      211 2023-12-06 04:33:07.000000 pyutmodelv2-2.1.5/src/pyutmodelv2/enumerations/PyutDisplayParameters.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1413 2023-11-17 01:51:01.000000 pyutmodelv2-2.1.5/src/pyutmodelv2/enumerations/PyutLinkType.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2603 2024-02-03 02:02:43.000000 pyutmodelv2-2.1.5/src/pyutmodelv2/enumerations/PyutStereotype.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1464 2023-12-05 23:38:43.000000 pyutmodelv2-2.1.5/src/pyutmodelv2/enumerations/PyutVisibility.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-05 21:50:10.000000 pyutmodelv2-2.1.5/src/pyutmodelv2/enumerations/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-11-17 01:51:01.000000 pyutmodelv2-2.1.5/src/pyutmodelv2/enumerations/py.typed
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-11-17 01:51:01.000000 pyutmodelv2-2.1.5/src/pyutmodelv2/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-02-03 15:08:20.311354 pyutmodelv2-2.1.5/src/pyutmodelv2.egg-info/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2404 2024-02-03 15:08:20.000000 pyutmodelv2-2.1.5/src/pyutmodelv2.egg-info/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1152 2024-02-03 15:08:20.000000 pyutmodelv2-2.1.5/src/pyutmodelv2.egg-info/SOURCES.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2024-02-03 15:08:20.000000 pyutmodelv2-2.1.5/src/pyutmodelv2.egg-info/dependency_links.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       12 2024-02-03 15:08:20.000000 pyutmodelv2-2.1.5/src/pyutmodelv2.egg-info/top_level.txt
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-30 23:04:32.643168 pyutmodelv2-2.1.6/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2022-07-23 19:00:15.000000 pyutmodelv2-2.1.6/LICENSE
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2404 2024-05-30 23:04:32.642989 pyutmodelv2-2.1.6/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1941 2023-12-17 20:07:31.000000 pyutmodelv2-2.1.6/README.md
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      775 2024-01-09 04:25:20.000000 pyutmodelv2-2.1.6/pyproject.toml
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2024-05-30 23:04:32.643203 pyutmodelv2-2.1.6/setup.cfg
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-30 23:04:32.638346 pyutmodelv2-2.1.6/src/
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-30 23:04:32.641402 pyutmodelv2-2.1.6/src/pyutmodelv2/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      535 2023-12-12 03:53:31.000000 pyutmodelv2-2.1.6/src/pyutmodelv2/PyutActor.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2901 2024-02-03 15:00:52.000000 pyutmodelv2-2.1.6/src/pyutmodelv2/PyutClass.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      916 2023-12-08 21:47:34.000000 pyutmodelv2-2.1.6/src/pyutmodelv2/PyutClassCommon.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      951 2023-12-13 16:57:08.000000 pyutmodelv2-2.1.6/src/pyutmodelv2/PyutField.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1884 2024-05-30 20:25:50.000000 pyutmodelv2-2.1.6/src/pyutmodelv2/PyutInterface.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3186 2023-12-12 04:05:20.000000 pyutmodelv2-2.1.6/src/pyutmodelv2/PyutLink.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1560 2023-12-12 03:34:40.000000 pyutmodelv2-2.1.6/src/pyutmodelv2/PyutLinkedObject.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3102 2023-12-13 16:47:14.000000 pyutmodelv2-2.1.6/src/pyutmodelv2/PyutMethod.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      150 2023-12-10 21:14:19.000000 pyutmodelv2-2.1.6/src/pyutmodelv2/PyutModelTypes.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      426 2023-12-06 03:33:34.000000 pyutmodelv2-2.1.6/src/pyutmodelv2/PyutModifier.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      533 2023-12-07 03:25:37.000000 pyutmodelv2-2.1.6/src/pyutmodelv2/PyutNote.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      438 2023-12-12 03:09:47.000000 pyutmodelv2-2.1.6/src/pyutmodelv2/PyutObject.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      720 2023-12-13 16:55:10.000000 pyutmodelv2-2.1.6/src/pyutmodelv2/PyutParameter.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      524 2023-12-09 19:52:57.000000 pyutmodelv2-2.1.6/src/pyutmodelv2/PyutSDInstance.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2682 2023-12-09 19:02:21.000000 pyutmodelv2-2.1.6/src/pyutmodelv2/PyutSDMessage.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      504 2023-12-06 02:26:17.000000 pyutmodelv2-2.1.6/src/pyutmodelv2/PyutText.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      209 2023-12-06 15:49:24.000000 pyutmodelv2-2.1.6/src/pyutmodelv2/PyutType.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      237 2023-12-09 17:26:22.000000 pyutmodelv2-2.1.6/src/pyutmodelv2/PyutUseCase.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       45 2023-12-05 19:04:19.000000 pyutmodelv2-2.1.6/src/pyutmodelv2/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       27 2024-05-30 20:10:02.000000 pyutmodelv2-2.1.6/src/pyutmodelv2/_version.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-30 23:04:32.642708 pyutmodelv2-2.1.6/src/pyutmodelv2/enumerations/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      262 2024-01-12 03:20:53.000000 pyutmodelv2-2.1.6/src/pyutmodelv2/enumerations/PyutDisplayMethods.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      211 2023-12-06 04:33:07.000000 pyutmodelv2-2.1.6/src/pyutmodelv2/enumerations/PyutDisplayParameters.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1413 2023-11-17 01:51:01.000000 pyutmodelv2-2.1.6/src/pyutmodelv2/enumerations/PyutLinkType.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2603 2024-02-03 02:02:43.000000 pyutmodelv2-2.1.6/src/pyutmodelv2/enumerations/PyutStereotype.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1464 2023-12-05 23:38:43.000000 pyutmodelv2-2.1.6/src/pyutmodelv2/enumerations/PyutVisibility.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-05 21:50:10.000000 pyutmodelv2-2.1.6/src/pyutmodelv2/enumerations/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-11-17 01:51:01.000000 pyutmodelv2-2.1.6/src/pyutmodelv2/enumerations/py.typed
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-11-17 01:51:01.000000 pyutmodelv2-2.1.6/src/pyutmodelv2/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-30 23:04:32.642833 pyutmodelv2-2.1.6/src/pyutmodelv2.egg-info/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2404 2024-05-30 23:04:32.000000 pyutmodelv2-2.1.6/src/pyutmodelv2.egg-info/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1152 2024-05-30 23:04:32.000000 pyutmodelv2-2.1.6/src/pyutmodelv2.egg-info/SOURCES.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2024-05-30 23:04:32.000000 pyutmodelv2-2.1.6/src/pyutmodelv2.egg-info/dependency_links.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       12 2024-05-30 23:04:32.000000 pyutmodelv2-2.1.6/src/pyutmodelv2.egg-info/top_level.txt
```

### Comparing `pyutmodelv2-2.1.5/LICENSE` & `pyutmodelv2-2.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyutmodelv2-2.1.5/PKG-INFO` & `pyutmodelv2-2.1.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyutmodelv2
-Version: 2.1.5
+Version: 2.1.6
 Summary: Version 2 of the External Pyut Data Model
 Author-email: "Humberto A. Sanchez II" <Humbert.A.Sanchez.II@gmail.com>
 Maintainer-email: "Humberto A. Sanchez II" <Humbert.A.Sanchez.II@gmail.com>
 License: GNU AFFERO GENERAL PUBLIC LICENSE
 Project-URL: Repository, https://github.com/hasii2011/pyutmodelv2
 Keywords: pyut,external model,python
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyutmodelv2 Version: 2.1.5 Summary: Version 2 of
+Metadata-Version: 2.1 Name: pyutmodelv2 Version: 2.1.6 Summary: Version 2 of
 the External Pyut Data Model Author-email: "Humberto A. Sanchez II"
 gmail.com> Maintainer-email: "Humberto A. Sanchez II"
 gmail.com> License: GNU AFFERO GENERAL PUBLIC LICENSE Project-URL: Repository,
 https://github.com/hasii2011/pyutmodelv2 Keywords: pyut,external model,python
 Description-Content-Type: text/markdown License-File: LICENSE ![](https://
 github.com/hasii2011/code-ally-basic/blob/master/developer/agpl-license-web-
 badge-version-2-256x48.png "AGPL") [![Maintenance](https://img.shields.io/
```

### Comparing `pyutmodelv2-2.1.5/README.md` & `pyutmodelv2-2.1.6/README.md`

 * *Files identical despite different names*

### Comparing `pyutmodelv2-2.1.5/pyproject.toml` & `pyutmodelv2-2.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyutmodelv2-2.1.5/src/pyutmodelv2/PyutActor.py` & `pyutmodelv2-2.1.6/src/pyutmodelv2/PyutActor.py`

 * *Files identical despite different names*

### Comparing `pyutmodelv2-2.1.5/src/pyutmodelv2/PyutClass.py` & `pyutmodelv2-2.1.6/src/pyutmodelv2/PyutClass.py`

 * *Files identical despite different names*

### Comparing `pyutmodelv2-2.1.5/src/pyutmodelv2/PyutClassCommon.py` & `pyutmodelv2-2.1.6/src/pyutmodelv2/PyutClassCommon.py`

 * *Files identical despite different names*

### Comparing `pyutmodelv2-2.1.5/src/pyutmodelv2/PyutField.py` & `pyutmodelv2-2.1.6/src/pyutmodelv2/PyutField.py`

 * *Files identical despite different names*

### Comparing `pyutmodelv2-2.1.5/src/pyutmodelv2/PyutLink.py` & `pyutmodelv2-2.1.6/src/pyutmodelv2/PyutLink.py`

 * *Files identical despite different names*

### Comparing `pyutmodelv2-2.1.5/src/pyutmodelv2/PyutLinkedObject.py` & `pyutmodelv2-2.1.6/src/pyutmodelv2/PyutLinkedObject.py`

 * *Files identical despite different names*

### Comparing `pyutmodelv2-2.1.5/src/pyutmodelv2/PyutMethod.py` & `pyutmodelv2-2.1.6/src/pyutmodelv2/PyutMethod.py`

 * *Files identical despite different names*

### Comparing `pyutmodelv2-2.1.5/src/pyutmodelv2/PyutNote.py` & `pyutmodelv2-2.1.6/src/pyutmodelv2/PyutNote.py`

 * *Files identical despite different names*

### Comparing `pyutmodelv2-2.1.5/src/pyutmodelv2/PyutParameter.py` & `pyutmodelv2-2.1.6/src/pyutmodelv2/PyutParameter.py`

 * *Files identical despite different names*

### Comparing `pyutmodelv2-2.1.5/src/pyutmodelv2/PyutSDInstance.py` & `pyutmodelv2-2.1.6/src/pyutmodelv2/PyutSDInstance.py`

 * *Files identical despite different names*

### Comparing `pyutmodelv2-2.1.5/src/pyutmodelv2/PyutSDMessage.py` & `pyutmodelv2-2.1.6/src/pyutmodelv2/PyutSDMessage.py`

 * *Files identical despite different names*

### Comparing `pyutmodelv2-2.1.5/src/pyutmodelv2/enumerations/PyutLinkType.py` & `pyutmodelv2-2.1.6/src/pyutmodelv2/enumerations/PyutLinkType.py`

 * *Files identical despite different names*

### Comparing `pyutmodelv2-2.1.5/src/pyutmodelv2/enumerations/PyutStereotype.py` & `pyutmodelv2-2.1.6/src/pyutmodelv2/enumerations/PyutStereotype.py`

 * *Files identical despite different names*

### Comparing `pyutmodelv2-2.1.5/src/pyutmodelv2/enumerations/PyutVisibility.py` & `pyutmodelv2-2.1.6/src/pyutmodelv2/enumerations/PyutVisibility.py`

 * *Files identical despite different names*

### Comparing `pyutmodelv2-2.1.5/src/pyutmodelv2.egg-info/PKG-INFO` & `pyutmodelv2-2.1.6/src/pyutmodelv2.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyutmodelv2
-Version: 2.1.5
+Version: 2.1.6
 Summary: Version 2 of the External Pyut Data Model
 Author-email: "Humberto A. Sanchez II" <Humbert.A.Sanchez.II@gmail.com>
 Maintainer-email: "Humberto A. Sanchez II" <Humbert.A.Sanchez.II@gmail.com>
 License: GNU AFFERO GENERAL PUBLIC LICENSE
 Project-URL: Repository, https://github.com/hasii2011/pyutmodelv2
 Keywords: pyut,external model,python
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyutmodelv2 Version: 2.1.5 Summary: Version 2 of
+Metadata-Version: 2.1 Name: pyutmodelv2 Version: 2.1.6 Summary: Version 2 of
 the External Pyut Data Model Author-email: "Humberto A. Sanchez II"
 gmail.com> Maintainer-email: "Humberto A. Sanchez II"
 gmail.com> License: GNU AFFERO GENERAL PUBLIC LICENSE Project-URL: Repository,
 https://github.com/hasii2011/pyutmodelv2 Keywords: pyut,external model,python
 Description-Content-Type: text/markdown License-File: LICENSE ![](https://
 github.com/hasii2011/code-ally-basic/blob/master/developer/agpl-license-web-
 badge-version-2-256x48.png "AGPL") [![Maintenance](https://img.shields.io/
```

### Comparing `pyutmodelv2-2.1.5/src/pyutmodelv2.egg-info/SOURCES.txt` & `pyutmodelv2-2.1.6/src/pyutmodelv2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

