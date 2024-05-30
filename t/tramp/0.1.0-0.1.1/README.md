# Comparing `tmp/tramp-0.1.0.tar.gz` & `tmp/tramp-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tramp-0.1.0.tar", max compression
+gzip compressed data, was "tramp-0.1.1.tar", max compression
```

## Comparing `tramp-0.1.0.tar` & `tramp-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,7 @@
--rw-r--r--   0        0        0       34 2024-01-06 15:36:49.179444 tramp-0.1.0/README.md
--rw-r--r--   0        0        0      311 2024-01-06 15:36:07.837481 tramp-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1664 2024-01-06 15:28:44.492177 tramp-0.1.0/tramp/results.py
--rw-r--r--   0        0        0      560 1970-01-01 00:00:00.000000 tramp-0.1.0/setup.py
--rw-r--r--   0        0        0      463 1970-01-01 00:00:00.000000 tramp-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       35 2024-05-30 23:33:01.796806 tramp-0.1.1/README.md
+-rw-r--r--   0        0        0      311 2024-05-30 23:32:44.295223 tramp-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      371 2024-05-30 23:23:56.025236 tramp-0.1.1/tramp/containers.py
+-rw-r--r--   0        0        0     1717 2024-05-30 23:12:32.270826 tramp-0.1.1/tramp/optionals.py
+-rw-r--r--   0        0        0     2641 2024-05-30 23:50:30.714838 tramp-0.1.1/tramp/results.py
+-rw-r--r--   0        0        0      561 1970-01-01 00:00:00.000000 tramp-0.1.1/setup.py
+-rw-r--r--   0        0        0      464 1970-01-01 00:00:00.000000 tramp-0.1.1/PKG-INFO
```

### Comparing `tramp-0.1.0/setup.py` & `tramp-0.1.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 ['tramp']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'tramp',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'No idea but we have a result type!',
-    'long_description': 'No idea but we have a result type\n',
+    'long_description': 'No idea but we have a result type!\n',
     'author': 'Zech Zimmerman',
     'author_email': 'hi@zech.codes',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

