# Comparing `tmp/sevenbridges-0.0.8.tar.gz` & `tmp/sevenbridges-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sevenbridges-0.0.8.tar", last modified: Thu Nov  9 13:28:53 2023, max compression
+gzip compressed data, was "sevenbridges-0.0.9.tar", last modified: Thu Nov  9 13:57:59 2023, max compression
```

## Comparing `sevenbridges-0.0.8.tar` & `sevenbridges-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-11-09 13:28:53.684373 sevenbridges-0.0.8/
--rw-rw-rw-   0        0        0     1094 2023-11-08 20:55:04.000000 sevenbridges-0.0.8/LICENSE
--rw-rw-rw-   0        0        0        0 2023-11-08 20:45:06.000000 sevenbridges-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0      250 2023-11-09 13:28:53.683373 sevenbridges-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       22 2023-11-08 20:19:39.000000 sevenbridges-0.0.8/README.md
--rw-rw-rw-   0        0        0        0 2023-11-08 20:44:52.000000 sevenbridges-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-11-09 13:28:53.685373 sevenbridges-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      498 2023-11-09 13:28:34.000000 sevenbridges-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-11-09 13:28:53.681375 sevenbridges-0.0.8/sevenbridges.egg-info/
--rw-rw-rw-   0        0        0      250 2023-11-09 13:28:53.000000 sevenbridges-0.0.8/sevenbridges.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      248 2023-11-09 13:28:53.000000 sevenbridges-0.0.8/sevenbridges.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-09 13:28:53.000000 sevenbridges-0.0.8/sevenbridges.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       74 2023-11-09 13:28:53.000000 sevenbridges-0.0.8/sevenbridges.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-11-09 13:28:53.000000 sevenbridges-0.0.8/sevenbridges.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-11-09 13:28:53.682373 sevenbridges-0.0.8/src/
--rw-rw-rw-   0        0        0    20038 2023-11-09 13:21:20.000000 sevenbridges-0.0.8/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-11-09 13:57:59.708040 sevenbridges-0.0.9/
+-rw-rw-rw-   0        0        0     1094 2023-11-08 20:55:04.000000 sevenbridges-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-11-08 20:45:06.000000 sevenbridges-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      250 2023-11-09 13:57:59.707045 sevenbridges-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       22 2023-11-08 20:19:39.000000 sevenbridges-0.0.9/README.md
+-rw-rw-rw-   0        0        0        0 2023-11-08 20:44:52.000000 sevenbridges-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-11-09 13:57:59.708040 sevenbridges-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      507 2023-11-09 13:57:30.000000 sevenbridges-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-11-09 13:57:59.689040 sevenbridges-0.0.9/sevenbridges/
+-rw-rw-rw-   0        0        0      147 2023-11-09 13:30:08.000000 sevenbridges-0.0.9/sevenbridges/__init__.py
+-rw-rw-rw-   0        0        0      151 2023-11-09 13:56:21.000000 sevenbridges-0.0.9/sevenbridges/new_joke.py
+drwxrwxrwx   0        0        0        0 2023-11-09 13:57:59.705042 sevenbridges-0.0.9/sevenbridges.egg-info/
+-rw-rw-rw-   0        0        0      250 2023-11-09 13:57:59.000000 sevenbridges-0.0.9/sevenbridges.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2023-11-09 13:57:59.000000 sevenbridges-0.0.9/sevenbridges.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-11-09 13:57:59.000000 sevenbridges-0.0.9/sevenbridges.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       74 2023-11-09 13:57:59.000000 sevenbridges-0.0.9/sevenbridges.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-11-09 13:57:59.000000 sevenbridges-0.0.9/sevenbridges.egg-info/top_level.txt
```

### Comparing `sevenbridges-0.0.8/LICENSE` & `sevenbridges-0.0.9/LICENSE`

 * *Files identical despite different names*

