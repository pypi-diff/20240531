# Comparing `tmp/py-ard-1.2.0.tar.gz` & `tmp/py-ard-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-ard-1.2.0.tar", last modified: Wed May 29 18:03:21 2024, max compression
+gzip compressed data, was "py-ard-1.2.1.tar", last modified: Fri May 31 16:46:32 2024, max compression
```

## Comparing `py-ard-1.2.0.tar` & `py-ard-1.2.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:03:21.204545 py-ard-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-05-29 18:03:07.000000 py-ard-1.2.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-29 18:03:07.000000 py-ard-1.2.0/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-29 18:03:07.000000 py-ard-1.2.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-29 18:03:07.000000 py-ard-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-29 18:03:07.000000 py-ard-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    21193 2024-05-29 18:03:21.204545 py-ard-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16266 2024-05-29 18:03:07.000000 py-ard-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:03:21.200545 py-ard-1.2.0/py_ard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    21193 2024-05-29 18:03:20.000000 py-ard-1.2.0/py_ard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-29 18:03:21.000000 py-ard-1.2.0/py_ard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 18:03:20.000000 py-ard-1.2.0/py_ard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 18:03:20.000000 py-ard-1.2.0/py_ard.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 18:03:20.000000 py-ard-1.2.0/py_ard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-29 18:03:20.000000 py-ard-1.2.0/py_ard.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:03:21.204545 py-ard-1.2.0/pyard/
--rw-r--r--   0 runner    (1001) docker     (127)    12706 2024-05-29 18:03:07.000000 py-ard-1.2.0/pyard/CWD2.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-29 18:03:07.000000 py-ard-1.2.0/pyard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    39521 2024-05-29 18:03:07.000000 py-ard-1.2.0/pyard/ard.py
--rw-r--r--   0 runner    (1001) docker     (127)     7628 2024-05-29 18:03:07.000000 py-ard-1.2.0/pyard/blender.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-29 18:03:07.000000 py-ard-1.2.0/pyard/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    17513 2024-05-29 18:03:07.000000 py-ard-1.2.0/pyard/data_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    22303 2024-05-29 18:03:07.000000 py-ard-1.2.0/pyard/db.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-29 18:03:07.000000 py-ard-1.2.0/pyard/dna_relshp.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-05-29 18:03:07.000000 py-ard-1.2.0/pyard/drbx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-29 18:03:07.000000 py-ard-1.2.0/pyard/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10163 2024-05-29 18:03:07.000000 py-ard-1.2.0/pyard/load.py
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-29 18:03:07.000000 py-ard-1.2.0/pyard/mappings.py
--rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-05-29 18:03:07.000000 py-ard-1.2.0/pyard/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7912 2024-05-29 18:03:07.000000 py-ard-1.2.0/pyard/serology.py
--rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-05-29 18:03:07.000000 py-ard-1.2.0/pyard/smart_sort.py
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-29 18:03:07.000000 py-ard-1.2.0/requirements-tests.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 18:03:07.000000 py-ard-1.2.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:03:21.204545 py-ard-1.2.0/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)     6024 2024-05-29 18:03:07.000000 py-ard-1.2.0/scripts/pyard
--rwxr-xr-x   0 runner    (1001) docker     (127)     5195 2024-05-29 18:03:07.000000 py-ard-1.2.0/scripts/pyard-import
--rwxr-xr-x   0 runner    (1001) docker     (127)    15974 2024-05-29 18:03:07.000000 py-ard-1.2.0/scripts/pyard-reduce-csv
--rwxr-xr-x   0 runner    (1001) docker     (127)     4183 2024-05-29 18:03:07.000000 py-ard-1.2.0/scripts/pyard-status
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-29 18:03:21.204545 py-ard-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-05-29 18:03:07.000000 py-ard-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:46:32.520650 py-ard-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-05-31 16:46:23.000000 py-ard-1.2.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-31 16:46:23.000000 py-ard-1.2.1/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-31 16:46:23.000000 py-ard-1.2.1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-31 16:46:23.000000 py-ard-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-31 16:46:23.000000 py-ard-1.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    21193 2024-05-31 16:46:32.520650 py-ard-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16266 2024-05-31 16:46:23.000000 py-ard-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:46:32.516650 py-ard-1.2.1/py_ard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21193 2024-05-31 16:46:32.000000 py-ard-1.2.1/py_ard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-31 16:46:32.000000 py-ard-1.2.1/py_ard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 16:46:32.000000 py-ard-1.2.1/py_ard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 16:46:32.000000 py-ard-1.2.1/py_ard.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-31 16:46:32.000000 py-ard-1.2.1/py_ard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-31 16:46:32.000000 py-ard-1.2.1/py_ard.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:46:32.520650 py-ard-1.2.1/pyard/
+-rw-r--r--   0 runner    (1001) docker     (127)    12706 2024-05-31 16:46:23.000000 py-ard-1.2.1/pyard/CWD2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-31 16:46:23.000000 py-ard-1.2.1/pyard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39851 2024-05-31 16:46:23.000000 py-ard-1.2.1/pyard/ard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7628 2024-05-31 16:46:23.000000 py-ard-1.2.1/pyard/blender.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-31 16:46:23.000000 py-ard-1.2.1/pyard/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17513 2024-05-31 16:46:23.000000 py-ard-1.2.1/pyard/data_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22303 2024-05-31 16:46:23.000000 py-ard-1.2.1/pyard/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-31 16:46:23.000000 py-ard-1.2.1/pyard/dna_relshp.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-05-31 16:46:23.000000 py-ard-1.2.1/pyard/drbx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-31 16:46:23.000000 py-ard-1.2.1/pyard/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10163 2024-05-31 16:46:23.000000 py-ard-1.2.1/pyard/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-31 16:46:23.000000 py-ard-1.2.1/pyard/mappings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-05-31 16:46:23.000000 py-ard-1.2.1/pyard/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7912 2024-05-31 16:46:23.000000 py-ard-1.2.1/pyard/serology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-05-31 16:46:23.000000 py-ard-1.2.1/pyard/smart_sort.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-31 16:46:23.000000 py-ard-1.2.1/requirements-tests.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-31 16:46:23.000000 py-ard-1.2.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:46:32.520650 py-ard-1.2.1/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6024 2024-05-31 16:46:23.000000 py-ard-1.2.1/scripts/pyard
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5195 2024-05-31 16:46:23.000000 py-ard-1.2.1/scripts/pyard-import
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15974 2024-05-31 16:46:23.000000 py-ard-1.2.1/scripts/pyard-reduce-csv
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4183 2024-05-31 16:46:23.000000 py-ard-1.2.1/scripts/pyard-status
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-31 16:46:32.520650 py-ard-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-05-31 16:46:23.000000 py-ard-1.2.1/setup.py
```

### Comparing `py-ard-1.2.0/CONTRIBUTING.rst` & `py-ard-1.2.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `py-ard-1.2.0/COPYING` & `py-ard-1.2.1/COPYING`

 * *Files identical despite different names*

### Comparing `py-ard-1.2.0/LICENSE` & `py-ard-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py-ard-1.2.0/PKG-INFO` & `py-ard-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-ard
-Version: 1.2.0
+Version: 1.2.1
 Summary: ARD reduction for HLA with Python
 Home-page: https://github.com/nmdp-bioinformatics/py-ard
 Author: CIBMTR
 Author-email: cibmtr-pypi@nmdp.org
 License: LGPL 3.0
 Description: # py-ard
```

### Comparing `py-ard-1.2.0/README.md` & `py-ard-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `py-ard-1.2.0/py_ard.egg-info/PKG-INFO` & `py-ard-1.2.1/py_ard.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-ard
-Version: 1.2.0
+Version: 1.2.1
 Summary: ARD reduction for HLA with Python
 Home-page: https://github.com/nmdp-bioinformatics/py-ard
 Author: CIBMTR
 Author-email: cibmtr-pypi@nmdp.org
 License: LGPL 3.0
 Description: # py-ard
```

### Comparing `py-ard-1.2.0/py_ard.egg-info/SOURCES.txt` & `py-ard-1.2.1/py_ard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-ard-1.2.0/pyard/CWD2.csv` & `py-ard-1.2.1/pyard/CWD2.csv`

 * *Files identical despite different names*

### Comparing `py-ard-1.2.0/pyard/__init__.py` & `py-ard-1.2.1/pyard/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 #    > http://www.opensource.org/licenses/lgpl-license.php
 #
 from .blender import blender as dr_blender
 from .constants import DEFAULT_CACHE_SIZE
 from .misc import get_imgt_db_versions as db_versions
 
 __author__ = """NMDP Bioinformatics"""
-__version__ = "1.2.0"
+__version__ = "1.2.1"
 
 
 def init(
     imgt_version: str = "Latest",
     data_dir: str = None,
     load_mac: bool = True,
     cache_size: int = DEFAULT_CACHE_SIZE,
```

### Comparing `py-ard-1.2.0/pyard/ard.py` & `py-ard-1.2.1/pyard/ard.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,22 +221,26 @@
                         no_suffix_allele = redux_allele[:-1]
                     elif redux_allele.endswith("ARS"):
                         no_suffix_allele = redux_allele[:-3]
                     else:
                         no_suffix_allele = redux_allele
                     if (
                         no_suffix_allele == allele
+                        or "/" in no_suffix_allele
                         or no_suffix_allele in self.ars_mappings.p_not_g.values()
                     ):
                         return redux_allele
-                    redux_allele = self._redux_allele(
-                        no_suffix_allele, redux_type, True
+
+                    twice_redux_allele = self._redux_allele(
+                        no_suffix_allele, redux_type, False
                     )
-                    if self._is_valid_allele(redux_allele):
-                        return redux_allele
+                    if "/" in twice_redux_allele:
+                        return twice_redux_allele
+                    if self._is_valid_allele(twice_redux_allele):
+                        return twice_redux_allele
 
         if redux_type == "G" and allele in self.ars_mappings.g_group:
             if allele in self.ars_mappings.dup_g:
                 return self.ars_mappings.dup_g[allele]
             else:
                 return self.ars_mappings.g_group[allele]
         elif redux_type == "P" and allele in self.ars_mappings.p_group:
@@ -334,14 +338,18 @@
 
             if self._is_allele_in_db(allele):
                 return allele
             else:
                 raise InvalidAlleleError(f"{allele} is an invalid allele.")
 
     def _add_lg_suffix(self, redux_allele):
+        if "/" in redux_allele:
+            return "/".join(
+                [self._add_lg_suffix(allele) for allele in redux_allele.split("/")]
+            )
         # ARS suffix maybe used instead of g
         if self._config["ARS_as_lg"]:
             return redux_allele + "ARS"
         # lg mode has g appended with lgx reduction
         return redux_allele + "g"
 
     def _get_non_strict_allele(self, allele):
```

### Comparing `py-ard-1.2.0/pyard/blender.py` & `py-ard-1.2.1/pyard/blender.py`

 * *Files identical despite different names*

### Comparing `py-ard-1.2.0/pyard/constants.py` & `py-ard-1.2.1/pyard/constants.py`

 * *Files identical despite different names*

### Comparing `py-ard-1.2.0/pyard/data_repository.py` & `py-ard-1.2.1/pyard/data_repository.py`

 * *Files identical despite different names*

### Comparing `py-ard-1.2.0/pyard/db.py` & `py-ard-1.2.1/pyard/db.py`

 * *Files identical despite different names*

### Comparing `py-ard-1.2.0/pyard/drbx.py` & `py-ard-1.2.1/pyard/drbx.py`

 * *Files identical despite different names*

### Comparing `py-ard-1.2.0/pyard/exceptions.py` & `py-ard-1.2.1/pyard/exceptions.py`

 * *Files identical despite different names*

### Comparing `py-ard-1.2.0/pyard/load.py` & `py-ard-1.2.1/pyard/load.py`

 * *Files identical despite different names*

### Comparing `py-ard-1.2.0/pyard/mappings.py` & `py-ard-1.2.1/pyard/mappings.py`

 * *Files identical despite different names*

### Comparing `py-ard-1.2.0/pyard/misc.py` & `py-ard-1.2.1/pyard/misc.py`

 * *Files identical despite different names*

### Comparing `py-ard-1.2.0/pyard/serology.py` & `py-ard-1.2.1/pyard/serology.py`

 * *Files identical despite different names*

### Comparing `py-ard-1.2.0/pyard/smart_sort.py` & `py-ard-1.2.1/pyard/smart_sort.py`

 * *Files identical despite different names*

### Comparing `py-ard-1.2.0/scripts/pyard` & `py-ard-1.2.1/scripts/pyard`

 * *Files identical despite different names*

### Comparing `py-ard-1.2.0/scripts/pyard-import` & `py-ard-1.2.1/scripts/pyard-import`

 * *Files identical despite different names*

### Comparing `py-ard-1.2.0/scripts/pyard-reduce-csv` & `py-ard-1.2.1/scripts/pyard-reduce-csv`

 * *Files identical despite different names*

### Comparing `py-ard-1.2.0/scripts/pyard-status` & `py-ard-1.2.1/scripts/pyard-status`

 * *Files identical despite different names*

### Comparing `py-ard-1.2.0/setup.cfg` & `py-ard-1.2.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.2.0
+current_version = 1.2.1
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version="{current_version}"
 replace = version="{new_version}"
```

### Comparing `py-ard-1.2.0/setup.py` & `py-ard-1.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     requirements = requirements_file.read().split("\n")
 
 with open("requirements-tests.txt") as requirements_file:
     test_requirements = requirements_file.read().split("\n")
 
 setup(
     name="py-ard",
-    version="1.2.0",
+    version="1.2.1",
     description="ARD reduction for HLA with Python",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="CIBMTR",
     author_email="cibmtr-pypi@nmdp.org",
     url="https://github.com/nmdp-bioinformatics/py-ard",
     packages=[
```

