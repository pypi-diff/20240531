# Comparing `tmp/confection-0.1.5.tar.gz` & `tmp/confection-0.1.5a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "confection-0.1.5.tar", last modified: Fri May 31 16:06:37 2024, max compression
+gzip compressed data, was "confection-0.1.5a0.tar", last modified: Sun Dec 31 15:48:01 2023, max compression
```

## Comparing `confection-0.1.5.tar` & `confection-0.1.5a0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-31 16:06:37.484152 confection-0.1.5/
--rw-r--r--   0 vsts      (1001) docker     (127)     1073 2024-05-31 16:06:32.000000 confection-0.1.5/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)       44 2024-05-31 16:06:32.000000 confection-0.1.5/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)    19593 2024-05-31 16:06:37.484152 confection-0.1.5/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)    18299 2024-05-31 16:06:32.000000 confection-0.1.5/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-31 16:06:37.484152 confection-0.1.5/confection/
--rw-r--r--   0 vsts      (1001) docker     (127)    47656 2024-05-31 16:06:32.000000 confection-0.1.5/confection/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-31 16:06:32.000000 confection-0.1.5/confection/py.typed
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-31 16:06:37.484152 confection-0.1.5/confection/tests/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-31 16:06:32.000000 confection-0.1.5/confection/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      489 2024-05-31 16:06:32.000000 confection-0.1.5/confection/tests/conftest.py
--rw-r--r--   0 vsts      (1001) docker     (127)    54505 2024-05-31 16:06:32.000000 confection-0.1.5/confection/tests/test_config.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1713 2024-05-31 16:06:32.000000 confection-0.1.5/confection/tests/test_frozen_structures.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3686 2024-05-31 16:06:32.000000 confection-0.1.5/confection/tests/util.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4300 2024-05-31 16:06:32.000000 confection-0.1.5/confection/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-31 16:06:37.484152 confection-0.1.5/confection.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)    19593 2024-05-31 16:06:37.000000 confection-0.1.5/confection.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)      481 2024-05-31 16:06:37.000000 confection-0.1.5/confection.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-31 16:06:37.000000 confection-0.1.5/confection.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      118 2024-05-31 16:06:37.000000 confection-0.1.5/confection.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       11 2024-05-31 16:06:37.000000 confection-0.1.5/confection.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-31 16:06:37.000000 confection-0.1.5/confection.egg-info/zip-safe
--rw-r--r--   0 vsts      (1001) docker     (127)      118 2024-05-31 16:06:32.000000 confection-0.1.5/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (127)     1413 2024-05-31 16:06:37.484152 confection-0.1.5/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)      154 2024-05-31 16:06:32.000000 confection-0.1.5/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-12-31 15:48:01.712195 confection-0.1.5a0/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1073 2023-12-31 15:47:46.000000 confection-0.1.5a0/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)       44 2023-12-31 15:47:46.000000 confection-0.1.5a0/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)    19544 2023-12-31 15:48:01.712195 confection-0.1.5a0/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)    18299 2023-12-31 15:47:46.000000 confection-0.1.5a0/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-12-31 15:48:01.708195 confection-0.1.5a0/confection/
+-rw-r--r--   0 vsts      (1001) docker     (127)    47656 2023-12-31 15:47:46.000000 confection-0.1.5a0/confection/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-12-31 15:47:46.000000 confection-0.1.5a0/confection/py.typed
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-12-31 15:48:01.712195 confection-0.1.5a0/confection/tests/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-12-31 15:47:46.000000 confection-0.1.5a0/confection/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      489 2023-12-31 15:47:46.000000 confection-0.1.5a0/confection/tests/conftest.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    54505 2023-12-31 15:47:46.000000 confection-0.1.5a0/confection/tests/test_config.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1713 2023-12-31 15:47:46.000000 confection-0.1.5a0/confection/tests/test_frozen_structures.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3686 2023-12-31 15:47:46.000000 confection-0.1.5a0/confection/tests/util.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4300 2023-12-31 15:47:46.000000 confection-0.1.5a0/confection/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-12-31 15:48:01.712195 confection-0.1.5a0/confection.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)    19544 2023-12-31 15:48:01.000000 confection-0.1.5a0/confection.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      481 2023-12-31 15:48:01.000000 confection-0.1.5a0/confection.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2023-12-31 15:48:01.000000 confection-0.1.5a0/confection.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      118 2023-12-31 15:48:01.000000 confection-0.1.5a0/confection.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       11 2023-12-31 15:48:01.000000 confection-0.1.5a0/confection.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2023-12-31 15:48:01.000000 confection-0.1.5a0/confection.egg-info/zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)      118 2023-12-31 15:47:46.000000 confection-0.1.5a0/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)     1375 2023-12-31 15:48:01.712195 confection-0.1.5a0/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)      154 2023-12-31 15:47:46.000000 confection-0.1.5a0/setup.py
```

### Comparing `confection-0.1.5/LICENSE` & `confection-0.1.5a0/LICENSE`

 * *Files identical despite different names*

### Comparing `confection-0.1.5/PKG-INFO` & `confection-0.1.5a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: confection
-Version: 0.1.5
+Version: 0.1.5a0
 Summary: The sweetest config system for Python
 Home-page: https://github.com/explosion/confection
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -17,21 +17,20 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic!=1.8,!=1.8.1,<3.0.0,>=1.7.4
-Requires-Dist: typing_extensions<5.0.0,>=3.7.4.1; python_version < "3.8"
+Requires-Dist: typing_extensions<4.5.0,>=3.7.4.1; python_version < "3.8"
 Requires-Dist: srsly<3.0.0,>=2.4.0
 
 <a href="https://explosion.ai"><img src="https://explosion.ai/assets/img/logo.svg" width="125" height="125" align="right" /></a>
 
 # Confection: The sweetest config system for Python
 
 `confection` :candy: is a lightweight library that offers a **configuration
```

### Comparing `confection-0.1.5/README.md` & `confection-0.1.5a0/README.md`

 * *Files identical despite different names*

### Comparing `confection-0.1.5/confection/__init__.py` & `confection-0.1.5a0/confection/__init__.py`

 * *Files identical despite different names*

### Comparing `confection-0.1.5/confection/tests/test_config.py` & `confection-0.1.5a0/confection/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `confection-0.1.5/confection/tests/test_frozen_structures.py` & `confection-0.1.5a0/confection/tests/test_frozen_structures.py`

 * *Files identical despite different names*

### Comparing `confection-0.1.5/confection/tests/util.py` & `confection-0.1.5a0/confection/tests/util.py`

 * *Files identical despite different names*

### Comparing `confection-0.1.5/confection/util.py` & `confection-0.1.5a0/confection/util.py`

 * *Files identical despite different names*

### Comparing `confection-0.1.5/confection.egg-info/PKG-INFO` & `confection-0.1.5a0/confection.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: confection
-Version: 0.1.5
+Version: 0.1.5a0
 Summary: The sweetest config system for Python
 Home-page: https://github.com/explosion/confection
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -17,21 +17,20 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic!=1.8,!=1.8.1,<3.0.0,>=1.7.4
-Requires-Dist: typing_extensions<5.0.0,>=3.7.4.1; python_version < "3.8"
+Requires-Dist: typing_extensions<4.5.0,>=3.7.4.1; python_version < "3.8"
 Requires-Dist: srsly<3.0.0,>=2.4.0
 
 <a href="https://explosion.ai"><img src="https://explosion.ai/assets/img/logo.svg" width="125" height="125" align="right" /></a>
 
 # Confection: The sweetest config system for Python
 
 `confection` :candy: is a lightweight library that offers a **configuration
```

### Comparing `confection-0.1.5/setup.cfg` & `confection-0.1.5a0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 0.1.5
+version = 0.1.5a0
 description = The sweetest config system for Python
 url = https://github.com/explosion/confection
 author = Explosion
 author_email = contact@explosion.ai
 license = MIT
 long_description = file: README.md
 long_description_content_type = text/markdown
@@ -19,24 +19,23 @@
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
-	Programming Language :: Python :: 3.12
 	Topic :: Scientific/Engineering
 
 [options]
 zip_safe = true
 include_package_data = true
 python_requires = >=3.6
 install_requires = 
 	pydantic>=1.7.4,!=1.8,!=1.8.1,<3.0.0
-	typing_extensions>=3.7.4.1,<5.0.0; python_version < "3.8"
+	typing_extensions>=3.7.4.1,<4.5.0; python_version < "3.8"
 	srsly>=2.4.0,<3.0.0
 
 [sdist]
 formats = gztar
 
 [flake8]
 ignore = E203, E266, E501, E731, W503
```

