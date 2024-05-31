# Comparing `tmp/checks-superstaq-0.5.8.tar.gz` & `tmp/checks-superstaq-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "checks-superstaq-0.5.8.tar", last modified: Tue Jan 30 18:46:51 2024, max compression
+gzip compressed data, was "checks-superstaq-0.5.9.tar", last modified: Fri Feb  9 16:12:54 2024, max compression
```

## Comparing `checks-superstaq-0.5.8.tar` & `checks-superstaq-0.5.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 18:46:51.914783 checks-superstaq-0.5.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-01-30 18:46:51.910783 checks-superstaq-0.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-01-30 18:46:39.000000 checks-superstaq-0.5.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 18:46:51.910783 checks-superstaq-0.5.8/checks_superstaq/
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-01-30 18:46:39.000000 checks-superstaq-0.5.8/checks_superstaq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-30 18:46:39.000000 checks-superstaq-0.5.8/checks_superstaq/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-01-30 18:46:39.000000 checks-superstaq-0.5.8/checks_superstaq/all_.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1371 2024-01-30 18:46:39.000000 checks-superstaq-0.5.8/checks_superstaq/build_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)    14850 2024-01-30 18:46:39.000000 checks-superstaq-0.5.8/checks_superstaq/check_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-01-30 18:46:39.000000 checks-superstaq-0.5.8/checks_superstaq/checks-pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-01-30 18:46:39.000000 checks-superstaq-0.5.8/checks_superstaq/configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-01-30 18:46:39.000000 checks-superstaq-0.5.8/checks_superstaq/coverage_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-01-30 18:46:39.000000 checks-superstaq-0.5.8/checks_superstaq/flake8_.py
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-01-30 18:46:39.000000 checks-superstaq-0.5.8/checks_superstaq/format_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-01-30 18:46:39.000000 checks-superstaq-0.5.8/checks_superstaq/mypy_.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 18:46:39.000000 checks-superstaq-0.5.8/checks_superstaq/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-01-30 18:46:39.000000 checks-superstaq-0.5.8/checks_superstaq/pylint_.py
--rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-01-30 18:46:39.000000 checks-superstaq-0.5.8/checks_superstaq/pytest_.py
--rw-r--r--   0 runner    (1001) docker     (127)    10155 2024-01-30 18:46:39.000000 checks-superstaq-0.5.8/checks_superstaq/requirements.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 18:46:51.910783 checks-superstaq-0.5.8/checks_superstaq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-01-30 18:46:51.000000 checks-superstaq-0.5.8/checks_superstaq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-01-30 18:46:51.000000 checks-superstaq-0.5.8/checks_superstaq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-30 18:46:51.000000 checks-superstaq-0.5.8/checks_superstaq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-01-30 18:46:51.000000 checks-superstaq-0.5.8/checks_superstaq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-01-30 18:46:51.000000 checks-superstaq-0.5.8/checks_superstaq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-01-30 18:46:39.000000 checks-superstaq-0.5.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-01-30 18:46:39.000000 checks-superstaq-0.5.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-30 18:46:51.914783 checks-superstaq-0.5.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:12:54.916901 checks-superstaq-0.5.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-02-09 16:12:54.916901 checks-superstaq-0.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-02-09 16:12:41.000000 checks-superstaq-0.5.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:12:54.916901 checks-superstaq-0.5.9/checks_superstaq/
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-02-09 16:12:41.000000 checks-superstaq-0.5.9/checks_superstaq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-09 16:12:41.000000 checks-superstaq-0.5.9/checks_superstaq/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-02-09 16:12:41.000000 checks-superstaq-0.5.9/checks_superstaq/all_.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1371 2024-02-09 16:12:41.000000 checks-superstaq-0.5.9/checks_superstaq/build_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14850 2024-02-09 16:12:41.000000 checks-superstaq-0.5.9/checks_superstaq/check_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-02-09 16:12:41.000000 checks-superstaq-0.5.9/checks_superstaq/checks-pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-02-09 16:12:41.000000 checks-superstaq-0.5.9/checks_superstaq/configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-02-09 16:12:41.000000 checks-superstaq-0.5.9/checks_superstaq/coverage_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-02-09 16:12:41.000000 checks-superstaq-0.5.9/checks_superstaq/flake8_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-02-09 16:12:41.000000 checks-superstaq-0.5.9/checks_superstaq/format_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-02-09 16:12:41.000000 checks-superstaq-0.5.9/checks_superstaq/mypy_.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-09 16:12:41.000000 checks-superstaq-0.5.9/checks_superstaq/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-02-09 16:12:41.000000 checks-superstaq-0.5.9/checks_superstaq/pylint_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-02-09 16:12:41.000000 checks-superstaq-0.5.9/checks_superstaq/pytest_.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10155 2024-02-09 16:12:41.000000 checks-superstaq-0.5.9/checks_superstaq/requirements.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:12:54.916901 checks-superstaq-0.5.9/checks_superstaq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-02-09 16:12:54.000000 checks-superstaq-0.5.9/checks_superstaq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-02-09 16:12:54.000000 checks-superstaq-0.5.9/checks_superstaq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-09 16:12:54.000000 checks-superstaq-0.5.9/checks_superstaq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-02-09 16:12:54.000000 checks-superstaq-0.5.9/checks_superstaq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-09 16:12:54.000000 checks-superstaq-0.5.9/checks_superstaq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-02-09 16:12:41.000000 checks-superstaq-0.5.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-02-09 16:12:41.000000 checks-superstaq-0.5.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-09 16:12:54.916901 checks-superstaq-0.5.9/setup.cfg
```

### Comparing `checks-superstaq-0.5.8/PKG-INFO` & `checks-superstaq-0.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: checks-superstaq
-Version: 0.5.8
+Version: 0.5.9
 Summary: Check script tools for Superstaq.
 Author-email: Superstaq development team <superstaq@infleqtion.com>
 License: Apache-2.0
 Project-URL: homepage, https://github.com/Infleqtion/client-superstaq
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Requires-Dist: black[colorama,jupyter]>=24.1.0
```

### Comparing `checks-superstaq-0.5.8/checks_superstaq/all_.py` & `checks-superstaq-0.5.9/checks_superstaq/all_.py`

 * *Files identical despite different names*

### Comparing `checks-superstaq-0.5.8/checks_superstaq/build_docs.py` & `checks-superstaq-0.5.9/checks_superstaq/build_docs.py`

 * *Files identical despite different names*

### Comparing `checks-superstaq-0.5.8/checks_superstaq/check_utils.py` & `checks-superstaq-0.5.9/checks_superstaq/check_utils.py`

 * *Files identical despite different names*

### Comparing `checks-superstaq-0.5.8/checks_superstaq/checks-pyproject.toml` & `checks-superstaq-0.5.9/checks_superstaq/checks-pyproject.toml`

 * *Files identical despite different names*

### Comparing `checks-superstaq-0.5.8/checks_superstaq/configs.py` & `checks-superstaq-0.5.9/checks_superstaq/configs.py`

 * *Files identical despite different names*

### Comparing `checks-superstaq-0.5.8/checks_superstaq/coverage_.py` & `checks-superstaq-0.5.9/checks_superstaq/coverage_.py`

 * *Files identical despite different names*

### Comparing `checks-superstaq-0.5.8/checks_superstaq/flake8_.py` & `checks-superstaq-0.5.9/checks_superstaq/flake8_.py`

 * *Files identical despite different names*

### Comparing `checks-superstaq-0.5.8/checks_superstaq/format_.py` & `checks-superstaq-0.5.9/checks_superstaq/format_.py`

 * *Files identical despite different names*

### Comparing `checks-superstaq-0.5.8/checks_superstaq/mypy_.py` & `checks-superstaq-0.5.9/checks_superstaq/mypy_.py`

 * *Files identical despite different names*

### Comparing `checks-superstaq-0.5.8/checks_superstaq/pylint_.py` & `checks-superstaq-0.5.9/checks_superstaq/pylint_.py`

 * *Files identical despite different names*

### Comparing `checks-superstaq-0.5.8/checks_superstaq/pytest_.py` & `checks-superstaq-0.5.9/checks_superstaq/pytest_.py`

 * *Files identical despite different names*

### Comparing `checks-superstaq-0.5.8/checks_superstaq/requirements.py` & `checks-superstaq-0.5.9/checks_superstaq/requirements.py`

 * *Files identical despite different names*

### Comparing `checks-superstaq-0.5.8/checks_superstaq.egg-info/PKG-INFO` & `checks-superstaq-0.5.9/checks_superstaq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: checks-superstaq
-Version: 0.5.8
+Version: 0.5.9
 Summary: Check script tools for Superstaq.
 Author-email: Superstaq development team <superstaq@infleqtion.com>
 License: Apache-2.0
 Project-URL: homepage, https://github.com/Infleqtion/client-superstaq
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Requires-Dist: black[colorama,jupyter]>=24.1.0
```

### Comparing `checks-superstaq-0.5.8/checks_superstaq.egg-info/SOURCES.txt` & `checks-superstaq-0.5.9/checks_superstaq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `checks-superstaq-0.5.8/pyproject.toml` & `checks-superstaq-0.5.9/pyproject.toml`

 * *Files identical despite different names*

