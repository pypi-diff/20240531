# Comparing `tmp/django_template_lsp-0.2.0.tar.gz` & `tmp/django_template_lsp-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_template_lsp-0.2.0.tar", last modified: Wed May 29 14:46:25 2024, max compression
+gzip compressed data, was "django_template_lsp-0.2.1.tar", last modified: Fri May 31 10:00:18 2024, max compression
```

## Comparing `django_template_lsp-0.2.0.tar` & `django_template_lsp-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 maikel    (1000) maikel    (1000)        0 2024-05-29 14:46:25.049451 django_template_lsp-0.2.0/
--rw-r--r--   0 maikel    (1000) maikel    (1000)     1331 2024-05-29 14:46:25.049451 django_template_lsp-0.2.0/PKG-INFO
--rw-r--r--   0 maikel    (1000) maikel    (1000)      862 2024-05-29 14:45:50.000000 django_template_lsp-0.2.0/README.md
-drwxr-xr-x   0 maikel    (1000) maikel    (1000)        0 2024-05-29 14:46:25.049451 django_template_lsp-0.2.0/django_template_lsp.egg-info/
--rw-r--r--   0 maikel    (1000) maikel    (1000)     1331 2024-05-29 14:46:25.000000 django_template_lsp-0.2.0/django_template_lsp.egg-info/PKG-INFO
--rw-r--r--   0 maikel    (1000) maikel    (1000)      419 2024-05-29 14:46:25.000000 django_template_lsp-0.2.0/django_template_lsp.egg-info/SOURCES.txt
--rw-r--r--   0 maikel    (1000) maikel    (1000)        1 2024-05-29 14:46:25.000000 django_template_lsp-0.2.0/django_template_lsp.egg-info/dependency_links.txt
--rw-r--r--   0 maikel    (1000) maikel    (1000)       78 2024-05-29 14:46:25.000000 django_template_lsp-0.2.0/django_template_lsp.egg-info/entry_points.txt
--rw-r--r--   0 maikel    (1000) maikel    (1000)       67 2024-05-29 14:46:25.000000 django_template_lsp-0.2.0/django_template_lsp.egg-info/requires.txt
--rw-r--r--   0 maikel    (1000) maikel    (1000)        6 2024-05-29 14:46:25.000000 django_template_lsp-0.2.0/django_template_lsp.egg-info/top_level.txt
-drwxr-xr-x   0 maikel    (1000) maikel    (1000)        0 2024-05-29 14:46:25.049451 django_template_lsp-0.2.0/djlsp/
--rw-r--r--   0 maikel    (1000) maikel    (1000)       22 2024-05-29 14:46:03.000000 django_template_lsp-0.2.0/djlsp/__init__.py
--rw-r--r--   0 maikel    (1000) maikel    (1000)       35 2024-05-17 11:41:45.000000 django_template_lsp-0.2.0/djlsp/__main__.py
--rw-r--r--   0 maikel    (1000) maikel    (1000)      515 2024-05-29 14:45:50.000000 django_template_lsp-0.2.0/djlsp/cli.py
--rw-r--r--   0 maikel    (1000) maikel    (1000)     4103 2024-05-29 14:45:50.000000 django_template_lsp-0.2.0/djlsp/constants.py
--rw-r--r--   0 maikel    (1000) maikel    (1000)     4255 2024-05-29 14:45:50.000000 django_template_lsp-0.2.0/djlsp/parser.py
--rw-r--r--   0 maikel    (1000) maikel    (1000)     6881 2024-05-29 14:45:50.000000 django_template_lsp-0.2.0/djlsp/server.py
--rw-r--r--   0 maikel    (1000) maikel    (1000)      141 2024-05-29 14:46:25.049451 django_template_lsp-0.2.0/setup.cfg
--rw-r--r--   0 maikel    (1000) maikel    (1000)      841 2024-05-29 14:45:50.000000 django_template_lsp-0.2.0/setup.py
-drwxr-xr-x   0 maikel    (1000) maikel    (1000)        0 2024-05-29 14:46:25.049451 django_template_lsp-0.2.0/tests/
--rw-r--r--   0 maikel    (1000) maikel    (1000)     1036 2024-05-29 14:45:50.000000 django_template_lsp-0.2.0/tests/test_django_collector.py
+drwxr-xr-x   0 maikel    (1000) maikel    (1000)        0 2024-05-31 10:00:18.750810 django_template_lsp-0.2.1/
+-rw-r--r--   0 maikel    (1000) maikel    (1000)     1331 2024-05-31 10:00:18.750810 django_template_lsp-0.2.1/PKG-INFO
+-rw-r--r--   0 maikel    (1000) maikel    (1000)      862 2024-05-29 14:45:50.000000 django_template_lsp-0.2.1/README.md
+drwxr-xr-x   0 maikel    (1000) maikel    (1000)        0 2024-05-31 10:00:18.747476 django_template_lsp-0.2.1/django_template_lsp.egg-info/
+-rw-r--r--   0 maikel    (1000) maikel    (1000)     1331 2024-05-31 10:00:18.000000 django_template_lsp-0.2.1/django_template_lsp.egg-info/PKG-INFO
+-rw-r--r--   0 maikel    (1000) maikel    (1000)      453 2024-05-31 10:00:18.000000 django_template_lsp-0.2.1/django_template_lsp.egg-info/SOURCES.txt
+-rw-r--r--   0 maikel    (1000) maikel    (1000)        1 2024-05-31 10:00:18.000000 django_template_lsp-0.2.1/django_template_lsp.egg-info/dependency_links.txt
+-rw-r--r--   0 maikel    (1000) maikel    (1000)       78 2024-05-31 10:00:18.000000 django_template_lsp-0.2.1/django_template_lsp.egg-info/entry_points.txt
+-rw-r--r--   0 maikel    (1000) maikel    (1000)       67 2024-05-31 10:00:18.000000 django_template_lsp-0.2.1/django_template_lsp.egg-info/requires.txt
+-rw-r--r--   0 maikel    (1000) maikel    (1000)        6 2024-05-31 10:00:18.000000 django_template_lsp-0.2.1/django_template_lsp.egg-info/top_level.txt
+drwxr-xr-x   0 maikel    (1000) maikel    (1000)        0 2024-05-31 10:00:18.747476 django_template_lsp-0.2.1/djlsp/
+-rw-r--r--   0 maikel    (1000) maikel    (1000)       22 2024-05-31 10:00:01.000000 django_template_lsp-0.2.1/djlsp/__init__.py
+-rw-r--r--   0 maikel    (1000) maikel    (1000)       35 2024-05-17 11:41:45.000000 django_template_lsp-0.2.1/djlsp/__main__.py
+-rw-r--r--   0 maikel    (1000) maikel    (1000)      515 2024-05-29 14:45:50.000000 django_template_lsp-0.2.1/djlsp/cli.py
+-rw-r--r--   0 maikel    (1000) maikel    (1000)     4103 2024-05-29 14:45:50.000000 django_template_lsp-0.2.1/djlsp/constants.py
+-rw-r--r--   0 maikel    (1000) maikel    (1000)     4255 2024-05-29 14:45:50.000000 django_template_lsp-0.2.1/djlsp/parser.py
+drwxr-xr-x   0 maikel    (1000) maikel    (1000)        0 2024-05-31 10:00:18.747476 django_template_lsp-0.2.1/djlsp/scripts/
+-rw-r--r--   0 maikel    (1000) maikel    (1000)     6234 2024-05-29 14:45:50.000000 django_template_lsp-0.2.1/djlsp/scripts/django-collector.py
+-rw-r--r--   0 maikel    (1000) maikel    (1000)     6881 2024-05-29 14:45:50.000000 django_template_lsp-0.2.1/djlsp/server.py
+-rw-r--r--   0 maikel    (1000) maikel    (1000)      141 2024-05-31 10:00:18.750810 django_template_lsp-0.2.1/setup.cfg
+-rw-r--r--   0 maikel    (1000) maikel    (1000)      887 2024-05-31 09:59:09.000000 django_template_lsp-0.2.1/setup.py
+drwxr-xr-x   0 maikel    (1000) maikel    (1000)        0 2024-05-31 10:00:18.747476 django_template_lsp-0.2.1/tests/
+-rw-r--r--   0 maikel    (1000) maikel    (1000)     1036 2024-05-29 14:45:50.000000 django_template_lsp-0.2.1/tests/test_django_collector.py
```

### Comparing `django_template_lsp-0.2.0/PKG-INFO` & `django_template_lsp-0.2.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-template-lsp
-Version: 0.2.0
+Version: 0.2.1
 Summary: Django template LSP
 Requires-Python: >= 3.9
 Description-Content-Type: text/markdown
 Requires-Dist: pygls
 Provides-Extra: dev
 Requires-Dist: tox; extra == "dev"
 Requires-Dist: black; extra == "dev"
```

### Comparing `django_template_lsp-0.2.0/README.md` & `django_template_lsp-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `django_template_lsp-0.2.0/django_template_lsp.egg-info/PKG-INFO` & `django_template_lsp-0.2.1/django_template_lsp.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-template-lsp
-Version: 0.2.0
+Version: 0.2.1
 Summary: Django template LSP
 Requires-Python: >= 3.9
 Description-Content-Type: text/markdown
 Requires-Dist: pygls
 Provides-Extra: dev
 Requires-Dist: tox; extra == "dev"
 Requires-Dist: black; extra == "dev"
```

### Comparing `django_template_lsp-0.2.0/djlsp/cli.py` & `django_template_lsp-0.2.1/djlsp/cli.py`

 * *Files identical despite different names*

### Comparing `django_template_lsp-0.2.0/djlsp/constants.py` & `django_template_lsp-0.2.1/djlsp/constants.py`

 * *Files identical despite different names*

### Comparing `django_template_lsp-0.2.0/djlsp/parser.py` & `django_template_lsp-0.2.1/djlsp/parser.py`

 * *Files identical despite different names*

### Comparing `django_template_lsp-0.2.0/djlsp/server.py` & `django_template_lsp-0.2.1/djlsp/server.py`

 * *Files identical despite different names*

### Comparing `django_template_lsp-0.2.0/setup.py` & `django_template_lsp-0.2.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 setup(
     name="django-template-lsp",
     version=__version__,
     description="Django template LSP",
     long_description=readme(),
     long_description_content_type="text/markdown",
     packages=find_packages(include=["djlsp", "djlsp.*"]),
+    package_data={"djlsp": ["scripts/*.py"]},
     entry_points={
         "console_scripts": [
             "djlsp = djlsp.cli:main",
             "django-template-lsp = djlsp.cli:main",
         ]
     },
     python_requires=">= 3.9",
```

### Comparing `django_template_lsp-0.2.0/tests/test_django_collector.py` & `django_template_lsp-0.2.1/tests/test_django_collector.py`

 * *Files identical despite different names*

