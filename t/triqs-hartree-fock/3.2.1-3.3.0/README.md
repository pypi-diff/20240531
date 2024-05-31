# Comparing `tmp/triqs_hartree_fock-3.2.1.tar.gz` & `tmp/triqs_hartree_fock-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "triqs_hartree_fock-3.2.1.tar", last modified: Wed Mar 20 14:35:09 2024, max compression
+gzip compressed data, was "triqs_hartree_fock-3.3.0.tar", last modified: Fri May 31 16:00:57 2024, max compression
```

## Comparing `triqs_hartree_fock-3.2.1.tar` & `triqs_hartree_fock-3.3.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 14:35:09.341392 triqs_hartree_fock-3.2.1/
--rw-r--r--   0 root         (0) root         (0)    35147 2024-03-20 14:35:00.000000 triqs_hartree_fock-3.2.1/COPYING.txt
--rw-r--r--   0 root         (0) root         (0)      894 2024-03-20 14:35:00.000000 triqs_hartree_fock-3.2.1/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      227 2024-03-20 14:35:06.000000 triqs_hartree_fock-3.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1026 2024-03-20 14:35:09.337392 triqs_hartree_fock-3.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      307 2024-03-20 14:35:00.000000 triqs_hartree_fock-3.2.1/README.md
--rw-r--r--   0 root         (0) root         (0)      934 2024-03-20 14:35:06.000000 triqs_hartree_fock-3.2.1/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 14:35:09.333392 triqs_hartree_fock-3.2.1/python/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 14:35:09.337392 triqs_hartree_fock-3.2.1/python/triqs_hartree_fock/
--rw-r--r--   0 root         (0) root         (0)     1147 2024-03-20 14:35:00.000000 triqs_hartree_fock-3.2.1/python/triqs_hartree_fock/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16309 2024-03-20 14:35:00.000000 triqs_hartree_fock-3.2.1/python/triqs_hartree_fock/impurity.py
--rw-r--r--   0 root         (0) root         (0)    10239 2024-03-20 14:35:00.000000 triqs_hartree_fock-3.2.1/python/triqs_hartree_fock/lattice.py
--rw-r--r--   0 root         (0) root         (0)     6039 2024-03-20 14:35:00.000000 triqs_hartree_fock-3.2.1/python/triqs_hartree_fock/utils.py
--rw-r--r--   0 root         (0) root         (0)     1119 2024-03-20 14:35:06.000000 triqs_hartree_fock-3.2.1/python/triqs_hartree_fock/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 14:35:09.337392 triqs_hartree_fock-3.2.1/python/triqs_hartree_fock.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1026 2024-03-20 14:35:09.000000 triqs_hartree_fock-3.2.1/python/triqs_hartree_fock.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      489 2024-03-20 14:35:09.000000 triqs_hartree_fock-3.2.1/python/triqs_hartree_fock.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-20 14:35:09.000000 triqs_hartree_fock-3.2.1/python/triqs_hartree_fock.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-03-20 14:35:09.000000 triqs_hartree_fock-3.2.1/python/triqs_hartree_fock.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2024-03-20 14:35:09.000000 triqs_hartree_fock-3.2.1/python/triqs_hartree_fock.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-20 14:35:09.341392 triqs_hartree_fock-3.2.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 16:00:57.180509 triqs_hartree_fock-3.3.0/
+-rw-r--r--   0 root         (0) root         (0)    35147 2024-05-31 16:00:52.000000 triqs_hartree_fock-3.3.0/COPYING.txt
+-rw-r--r--   0 root         (0) root         (0)      894 2024-05-31 16:00:52.000000 triqs_hartree_fock-3.3.0/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      227 2024-05-31 16:00:55.000000 triqs_hartree_fock-3.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1054 2024-05-31 16:00:57.180509 triqs_hartree_fock-3.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      335 2024-05-31 16:00:52.000000 triqs_hartree_fock-3.3.0/README.md
+-rw-r--r--   0 root         (0) root         (0)      934 2024-05-31 16:00:55.000000 triqs_hartree_fock-3.3.0/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 16:00:57.176509 triqs_hartree_fock-3.3.0/python/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 16:00:57.180509 triqs_hartree_fock-3.3.0/python/triqs_hartree_fock/
+-rw-r--r--   0 root         (0) root         (0)     1147 2024-05-31 16:00:52.000000 triqs_hartree_fock-3.3.0/python/triqs_hartree_fock/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16309 2024-05-31 16:00:52.000000 triqs_hartree_fock-3.3.0/python/triqs_hartree_fock/impurity.py
+-rw-r--r--   0 root         (0) root         (0)    10239 2024-05-31 16:00:52.000000 triqs_hartree_fock-3.3.0/python/triqs_hartree_fock/lattice.py
+-rw-r--r--   0 root         (0) root         (0)     6039 2024-05-31 16:00:52.000000 triqs_hartree_fock-3.3.0/python/triqs_hartree_fock/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1119 2024-05-31 16:00:55.000000 triqs_hartree_fock-3.3.0/python/triqs_hartree_fock/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 16:00:57.180509 triqs_hartree_fock-3.3.0/python/triqs_hartree_fock.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1054 2024-05-31 16:00:57.000000 triqs_hartree_fock-3.3.0/python/triqs_hartree_fock.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      489 2024-05-31 16:00:57.000000 triqs_hartree_fock-3.3.0/python/triqs_hartree_fock.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-31 16:00:57.000000 triqs_hartree_fock-3.3.0/python/triqs_hartree_fock.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-05-31 16:00:57.000000 triqs_hartree_fock-3.3.0/python/triqs_hartree_fock.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2024-05-31 16:00:57.000000 triqs_hartree_fock-3.3.0/python/triqs_hartree_fock.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-31 16:00:57.180509 triqs_hartree_fock-3.3.0/setup.cfg
```

### Comparing `triqs_hartree_fock-3.2.1/COPYING.txt` & `triqs_hartree_fock-3.3.0/COPYING.txt`

 * *Files identical despite different names*

### Comparing `triqs_hartree_fock-3.2.1/LICENSE.txt` & `triqs_hartree_fock-3.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `triqs_hartree_fock-3.2.1/PKG-INFO` & `triqs_hartree_fock-3.3.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: triqs_hartree_fock
-Version: 3.2.1
+Version: 3.3.0
 Summary: Hartree-Fock lattice and impurity solvers based on the TRIQS library (triqs.github.io)
 Author-email: TRIQS <triqs@flatironinstitute.org>
 Project-URL: Homepage, https://triqs.github.io/hartree_fock
 Project-URL: Bug Tracker, https://github.com/triqs/hartree_fock/issues
 Keywords: triqs,hartree_fock,dmft,impurity solver
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -15,10 +15,10 @@
 License-File: COPYING.txt
 Requires-Dist: numpy
 Requires-Dist: scipy
 
 # TRIQS hartree_fock
 An application based on TRIQS for using the Hartree-Fock method to solve lattice and impurity problems.
 
-Requires a working TRIQS instalation with a matching major version number.
+Requires a working [TRIQS](https://triqs.github.io) installation with a matching major version number.
 
 The documentation can be found at [triqs.github.io/hartree_fock](https://triqs.github.io/hartree_fock/).
```

### Comparing `triqs_hartree_fock-3.2.1/pyproject.toml` & `triqs_hartree_fock-3.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["python"]
 
 [project]
 name = "triqs_hartree_fock"
-version = "3.2.1"
+version = "3.3.0"
 authors = [
   { name="TRIQS", email="triqs@flatironinstitute.org" }
 ]
 description = "Hartree-Fock lattice and impurity solvers based on the TRIQS library (triqs.github.io)"
 readme = "README.md"
 keywords = ["triqs", "hartree_fock", "dmft", "impurity solver"]
 requires-python = ">=3.7"
```

### Comparing `triqs_hartree_fock-3.2.1/python/triqs_hartree_fock/__init__.py` & `triqs_hartree_fock-3.3.0/python/triqs_hartree_fock/__init__.py`

 * *Files identical despite different names*

### Comparing `triqs_hartree_fock-3.2.1/python/triqs_hartree_fock/impurity.py` & `triqs_hartree_fock-3.3.0/python/triqs_hartree_fock/impurity.py`

 * *Files identical despite different names*

### Comparing `triqs_hartree_fock-3.2.1/python/triqs_hartree_fock/lattice.py` & `triqs_hartree_fock-3.3.0/python/triqs_hartree_fock/lattice.py`

 * *Files identical despite different names*

### Comparing `triqs_hartree_fock-3.2.1/python/triqs_hartree_fock/utils.py` & `triqs_hartree_fock-3.3.0/python/triqs_hartree_fock/utils.py`

 * *Files identical despite different names*

### Comparing `triqs_hartree_fock-3.2.1/python/triqs_hartree_fock/version.py` & `triqs_hartree_fock-3.3.0/python/triqs_hartree_fock/version.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 # GNU General Public License for more details.
 #
 # You may obtain a copy of the License at
 #     https:#www.gnu.org/licenses/gpl-3.0.txt
 #
 # Authors: Jonathan Karp, Alexander Hampel, Nils Wentzell, Hugo U. R. Strand, Olivier Parcollet
 
-version = "3.2.1"
-triqs_hash = "40768343b393dbacaf535adc72e140d6dc316b65"
-triqs_hartree_fock_hash = "459b62a765c2d4218d1f91153f363d044d3c495a"
+version = "3.3.0"
+triqs_hash = "d7868de5b996d2fc756f53ec924b2ce0c2a163db"
+triqs_hartree_fock_hash = "6e6ea1330bb3712528ea1415e3df61591d7eb021"
 
 def show_version():
   print("\nYou are using triqs_hartree_fock version %s\n"%version)
 
 def show_git_hash():
-  print("\nYou are using triqs_hartree_fock git hash %s based on triqs git hash %s\n"%("459b62a765c2d4218d1f91153f363d044d3c495a", triqs_hash))
+  print("\nYou are using triqs_hartree_fock git hash %s based on triqs git hash %s\n"%("6e6ea1330bb3712528ea1415e3df61591d7eb021", triqs_hash))
```

### Comparing `triqs_hartree_fock-3.2.1/python/triqs_hartree_fock.egg-info/PKG-INFO` & `triqs_hartree_fock-3.3.0/python/triqs_hartree_fock.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: triqs_hartree_fock
-Version: 3.2.1
+Version: 3.3.0
 Summary: Hartree-Fock lattice and impurity solvers based on the TRIQS library (triqs.github.io)
 Author-email: TRIQS <triqs@flatironinstitute.org>
 Project-URL: Homepage, https://triqs.github.io/hartree_fock
 Project-URL: Bug Tracker, https://github.com/triqs/hartree_fock/issues
 Keywords: triqs,hartree_fock,dmft,impurity solver
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -15,10 +15,10 @@
 License-File: COPYING.txt
 Requires-Dist: numpy
 Requires-Dist: scipy
 
 # TRIQS hartree_fock
 An application based on TRIQS for using the Hartree-Fock method to solve lattice and impurity problems.
 
-Requires a working TRIQS instalation with a matching major version number.
+Requires a working [TRIQS](https://triqs.github.io) installation with a matching major version number.
 
 The documentation can be found at [triqs.github.io/hartree_fock](https://triqs.github.io/hartree_fock/).
```

