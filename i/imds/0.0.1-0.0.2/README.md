# Comparing `tmp/imds-0.0.1.tar.gz` & `tmp/imds-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imds-0.0.1.tar", last modified: Sun Apr 21 14:18:02 2024, max compression
+gzip compressed data, was "imds-0.0.2.tar", last modified: Fri May 31 01:37:33 2024, max compression
```

## Comparing `imds-0.0.1.tar` & `imds-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 z          (501) staff       (20)        0 2024-04-21 14:18:02.736902 imds-0.0.1/
--rw-r--r--   0 z          (501) staff       (20)      552 2024-04-21 14:18:02.736709 imds-0.0.1/PKG-INFO
--rw-r--r--   0 z          (501) staff       (20)      164 2024-04-21 14:17:54.000000 imds-0.0.1/README.md
-drwxr-xr-x   0 z          (501) staff       (20)        0 2024-04-21 14:18:02.735757 imds-0.0.1/imds/
--rw-r--r--   0 z          (501) staff       (20)       58 2024-04-21 14:13:37.000000 imds-0.0.1/imds/__init__.py
--rw-r--r--   0 z          (501) staff       (20)     1068 2024-04-21 14:15:39.000000 imds-0.0.1/imds/datasets.py
-drwxr-xr-x   0 z          (501) staff       (20)        0 2024-04-21 14:18:02.736537 imds-0.0.1/imds.egg-info/
--rw-r--r--   0 z          (501) staff       (20)      552 2024-04-21 14:18:02.000000 imds-0.0.1/imds.egg-info/PKG-INFO
--rw-r--r--   0 z          (501) staff       (20)      170 2024-04-21 14:18:02.000000 imds-0.0.1/imds.egg-info/SOURCES.txt
--rw-r--r--   0 z          (501) staff       (20)        1 2024-04-21 14:18:02.000000 imds-0.0.1/imds.egg-info/dependency_links.txt
--rw-r--r--   0 z          (501) staff       (20)        5 2024-04-21 14:18:02.000000 imds-0.0.1/imds.egg-info/top_level.txt
--rw-r--r--   0 z          (501) staff       (20)      488 2024-04-21 14:14:22.000000 imds-0.0.1/pyproject.toml
--rw-r--r--   0 z          (501) staff       (20)       38 2024-04-21 14:18:02.736946 imds-0.0.1/setup.cfg
+drwxr-xr-x   0 ttt        (501) staff       (20)        0 2024-05-31 01:37:33.814425 imds-0.0.2/
+-rw-r--r--   0 ttt        (501) staff       (20)      618 2024-05-31 01:37:33.813996 imds-0.0.2/PKG-INFO
+-rw-r--r--   0 ttt        (501) staff       (20)      231 2024-05-31 01:37:10.000000 imds-0.0.2/README.md
+drwxr-xr-x   0 ttt        (501) staff       (20)        0 2024-05-31 01:37:33.810932 imds-0.0.2/imds/
+-rw-r--r--   0 ttt        (501) staff       (20)      110 2024-05-31 01:35:50.000000 imds-0.0.2/imds/__init__.py
+-rw-r--r--   0 ttt        (501) staff       (20)     1068 2024-05-31 01:34:45.000000 imds-0.0.2/imds/datasets.py
+drwxr-xr-x   0 ttt        (501) staff       (20)        0 2024-05-31 01:37:33.813543 imds-0.0.2/imds.egg-info/
+-rw-r--r--   0 ttt        (501) staff       (20)      618 2024-05-31 01:37:33.000000 imds-0.0.2/imds.egg-info/PKG-INFO
+-rw-r--r--   0 ttt        (501) staff       (20)      170 2024-05-31 01:37:33.000000 imds-0.0.2/imds.egg-info/SOURCES.txt
+-rw-r--r--   0 ttt        (501) staff       (20)        1 2024-05-31 01:37:33.000000 imds-0.0.2/imds.egg-info/dependency_links.txt
+-rw-r--r--   0 ttt        (501) staff       (20)        5 2024-05-31 01:37:33.000000 imds-0.0.2/imds.egg-info/top_level.txt
+-rw-r--r--   0 ttt        (501) staff       (20)      488 2024-05-31 01:36:05.000000 imds-0.0.2/pyproject.toml
+-rw-r--r--   0 ttt        (501) staff       (20)       38 2024-05-31 01:37:33.814516 imds-0.0.2/setup.cfg
```

### Comparing `imds-0.0.1/imds/datasets.py` & `imds-0.0.2/imds/datasets.py`

 * *Files identical despite different names*

