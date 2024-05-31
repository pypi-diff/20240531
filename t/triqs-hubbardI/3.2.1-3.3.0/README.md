# Comparing `tmp/triqs_hubbardI-3.2.1.tar.gz` & `tmp/triqs_hubbardi-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "triqs_hubbardI-3.2.1.tar", last modified: Wed Mar 20 14:27:27 2024, max compression
+gzip compressed data, was "triqs_hubbardi-3.3.0.tar", last modified: Fri May 31 13:26:33 2024, max compression
```

## Comparing `triqs_hubbardI-3.2.1.tar` & `triqs_hubbardi-3.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 14:27:27.536936 triqs_hubbardI-3.2.1/
--rw-r--r--   0 root         (0) root         (0)    35147 2024-03-20 14:27:20.000000 triqs_hubbardI-3.2.1/COPYING.txt
--rw-r--r--   0 root         (0) root         (0)      793 2024-03-20 14:27:20.000000 triqs_hubbardI-3.2.1/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      227 2024-03-20 14:27:24.000000 triqs_hubbardI-3.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1372 2024-03-20 14:27:27.536936 triqs_hubbardI-3.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      684 2024-03-20 14:27:20.000000 triqs_hubbardI-3.2.1/README.md
--rw-r--r--   0 root         (0) root         (0)      903 2024-03-20 14:27:24.000000 triqs_hubbardI-3.2.1/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 14:27:27.532936 triqs_hubbardI-3.2.1/python/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 14:27:27.536936 triqs_hubbardI-3.2.1/python/triqs_hubbardI/
--rw-r--r--   0 root         (0) root         (0)     1008 2024-03-20 14:27:20.000000 triqs_hubbardI-3.2.1/python/triqs_hubbardI/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8767 2024-03-20 14:27:20.000000 triqs_hubbardI-3.2.1/python/triqs_hubbardI/solver.py
--rw-r--r--   0 root         (0) root         (0)     1338 2024-03-20 14:27:24.000000 triqs_hubbardI-3.2.1/python/triqs_hubbardI/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 14:27:27.536936 triqs_hubbardI-3.2.1/python/triqs_hubbardI.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1372 2024-03-20 14:27:27.000000 triqs_hubbardI-3.2.1/python/triqs_hubbardI.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      383 2024-03-20 14:27:27.000000 triqs_hubbardI-3.2.1/python/triqs_hubbardI.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-20 14:27:27.000000 triqs_hubbardI-3.2.1/python/triqs_hubbardI.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-03-20 14:27:27.000000 triqs_hubbardI-3.2.1/python/triqs_hubbardI.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-03-20 14:27:27.000000 triqs_hubbardI-3.2.1/python/triqs_hubbardI.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-20 14:27:27.536936 triqs_hubbardI-3.2.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:26:33.720414 triqs_hubbardi-3.3.0/
+-rw-r--r--   0 root         (0) root         (0)    35147 2024-05-31 13:26:28.000000 triqs_hubbardi-3.3.0/COPYING.txt
+-rw-r--r--   0 root         (0) root         (0)      793 2024-05-31 13:26:28.000000 triqs_hubbardi-3.3.0/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      227 2024-05-31 13:26:31.000000 triqs_hubbardi-3.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1406 2024-05-31 13:26:33.720414 triqs_hubbardi-3.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      718 2024-05-31 13:26:28.000000 triqs_hubbardi-3.3.0/README.md
+-rw-r--r--   0 root         (0) root         (0)      903 2024-05-31 13:26:31.000000 triqs_hubbardi-3.3.0/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:26:33.716414 triqs_hubbardi-3.3.0/python/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:26:33.716414 triqs_hubbardi-3.3.0/python/triqs_hubbardI/
+-rw-r--r--   0 root         (0) root         (0)     1008 2024-05-31 13:26:28.000000 triqs_hubbardi-3.3.0/python/triqs_hubbardI/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8767 2024-05-31 13:26:28.000000 triqs_hubbardi-3.3.0/python/triqs_hubbardI/solver.py
+-rw-r--r--   0 root         (0) root         (0)     1338 2024-05-31 13:26:31.000000 triqs_hubbardi-3.3.0/python/triqs_hubbardI/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:26:33.720414 triqs_hubbardi-3.3.0/python/triqs_hubbardI.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1406 2024-05-31 13:26:33.000000 triqs_hubbardi-3.3.0/python/triqs_hubbardI.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      383 2024-05-31 13:26:33.000000 triqs_hubbardi-3.3.0/python/triqs_hubbardI.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-31 13:26:33.000000 triqs_hubbardi-3.3.0/python/triqs_hubbardI.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-05-31 13:26:33.000000 triqs_hubbardi-3.3.0/python/triqs_hubbardI.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-05-31 13:26:33.000000 triqs_hubbardi-3.3.0/python/triqs_hubbardI.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-31 13:26:33.720414 triqs_hubbardi-3.3.0/setup.cfg
```

### Comparing `triqs_hubbardI-3.2.1/COPYING.txt` & `triqs_hubbardi-3.3.0/COPYING.txt`

 * *Files identical despite different names*

### Comparing `triqs_hubbardI-3.2.1/LICENSE.txt` & `triqs_hubbardi-3.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `triqs_hubbardI-3.2.1/PKG-INFO` & `triqs_hubbardi-3.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: triqs_hubbardI
-Version: 3.2.1
+Version: 3.3.0
 Summary: Hubbard-I impurity solver based on the TRIQS library (triqs.github.io)
 Author-email: TRIQS <triqs@flatironinstitute.org>
 Project-URL: Homepage, https://triqs.github.io/hubbardI
 Project-URL: Bug Tracker, https://github.com/triqs/hubbardI/issues
 Keywords: triqs,hubbard-I,impurity solver,dmft
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -18,11 +18,11 @@
 
 [![build](https://github.com/TRIQS/hubbardI/workflows/build/badge.svg)](https://github.com/TRIQS/hubbardI/actions?query=workflow%3Abuild)
 
 # hubbardI - A Hubbard-I solver based on triqs atom_diag
 
 This application implements the Hubbard-I solver in triqs using the lightweight diagonalization routine which come with triqs/atom_diag.
 
-Requires a working TRIQS instalation with a matching major version number.
+Requires a working [TRIQS](https://triqs.github.io/triqs) installation with a matching major version number.
 
 ### Usage ###
 The Solver comes with the same interface as, e.g., the [cthyb solver](https://triqs.github.io/cthyb/latest/index.html). More information on how to use the solver can be found in the [documentation](https://triqs.github.io/hubbardI/latest/documentation.html).
```

### Comparing `triqs_hubbardI-3.2.1/README.md` & `triqs_hubbardi-3.3.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [![build](https://github.com/TRIQS/hubbardI/workflows/build/badge.svg)](https://github.com/TRIQS/hubbardI/actions?query=workflow%3Abuild)
 
 # hubbardI - A Hubbard-I solver based on triqs atom_diag
 
 This application implements the Hubbard-I solver in triqs using the lightweight diagonalization routine which come with triqs/atom_diag.
 
-Requires a working TRIQS instalation with a matching major version number.
+Requires a working [TRIQS](https://triqs.github.io/triqs) installation with a matching major version number.
 
 ### Usage ###
 The Solver comes with the same interface as, e.g., the [cthyb solver](https://triqs.github.io/cthyb/latest/index.html). More information on how to use the solver can be found in the [documentation](https://triqs.github.io/hubbardI/latest/documentation.html).
```

### Comparing `triqs_hubbardI-3.2.1/pyproject.toml` & `triqs_hubbardi-3.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["python"]
 
 [project]
 name = "triqs_hubbardI"
-version = "3.2.1"
+version = "3.3.0"
 authors = [
   { name="TRIQS", email="triqs@flatironinstitute.org" }
 ]
 description = "Hubbard-I impurity solver based on the TRIQS library (triqs.github.io)"
 readme = "README.md"
 keywords = ["triqs", "hubbard-I", "impurity solver", "dmft"]
 requires-python = ">=3.7"
```

### Comparing `triqs_hubbardI-3.2.1/python/triqs_hubbardI/__init__.py` & `triqs_hubbardi-3.3.0/python/triqs_hubbardI/__init__.py`

 * *Files identical despite different names*

### Comparing `triqs_hubbardI-3.2.1/python/triqs_hubbardI/solver.py` & `triqs_hubbardi-3.3.0/python/triqs_hubbardI/solver.py`

 * *Files identical despite different names*

### Comparing `triqs_hubbardI-3.2.1/python/triqs_hubbardI/version.py` & `triqs_hubbardi-3.3.0/python/triqs_hubbardI/version.py`

 * *Files 17% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 # details.
 #
 # You should have received a copy of the GNU General Public License along with
 # TRIQS. If not, see <http://www.gnu.org/licenses/>.
 #
 ################################################################################
 
-version = "3.2.1"
-triqs_hash = "3144cecc10d3a1cd602b47326857ac64240adb22"
-triqs_hubbardI_hash = "8746a6d2be1b6f2e69cd3156e134ec64253c42ae"
+version = "3.3.0"
+triqs_hash = "d7868de5b996d2fc756f53ec924b2ce0c2a163db"
+triqs_hubbardI_hash = "f0053b8caff159bd018986c653f2c584650abafe"
 
 def show_version():
   print("\nYou are using triqs_hubbardI version %s\n"%version)
 
 def show_git_hash():
-  print("\nYou are using triqs_hubbardI git hash %s based on triqs git hash %s\n"%("8746a6d2be1b6f2e69cd3156e134ec64253c42ae", triqs_hash))
+  print("\nYou are using triqs_hubbardI git hash %s based on triqs git hash %s\n"%("f0053b8caff159bd018986c653f2c584650abafe", triqs_hash))
```

### Comparing `triqs_hubbardI-3.2.1/python/triqs_hubbardI.egg-info/PKG-INFO` & `triqs_hubbardi-3.3.0/python/triqs_hubbardI.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: triqs_hubbardI
-Version: 3.2.1
+Version: 3.3.0
 Summary: Hubbard-I impurity solver based on the TRIQS library (triqs.github.io)
 Author-email: TRIQS <triqs@flatironinstitute.org>
 Project-URL: Homepage, https://triqs.github.io/hubbardI
 Project-URL: Bug Tracker, https://github.com/triqs/hubbardI/issues
 Keywords: triqs,hubbard-I,impurity solver,dmft
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -18,11 +18,11 @@
 
 [![build](https://github.com/TRIQS/hubbardI/workflows/build/badge.svg)](https://github.com/TRIQS/hubbardI/actions?query=workflow%3Abuild)
 
 # hubbardI - A Hubbard-I solver based on triqs atom_diag
 
 This application implements the Hubbard-I solver in triqs using the lightweight diagonalization routine which come with triqs/atom_diag.
 
-Requires a working TRIQS instalation with a matching major version number.
+Requires a working [TRIQS](https://triqs.github.io/triqs) installation with a matching major version number.
 
 ### Usage ###
 The Solver comes with the same interface as, e.g., the [cthyb solver](https://triqs.github.io/cthyb/latest/index.html). More information on how to use the solver can be found in the [documentation](https://triqs.github.io/hubbardI/latest/documentation.html).
```

