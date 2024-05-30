# Comparing `tmp/beforerr-0.0.0.tar.gz` & `tmp/beforerr-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beforerr-0.0.0.tar", last modified: Thu May 30 22:38:37 2024, max compression
+gzip compressed data, was "beforerr-0.1.0.tar", last modified: Thu May 30 20:15:38 2024, max compression
```

## Comparing `beforerr-0.0.0.tar` & `beforerr-0.1.0.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0    11337 2023-04-27 10:12:58.000000 beforerr-0.0.0/LICENSE
--rw-r--r--   0        0        0      185 2024-05-30 20:42:04.877118 beforerr-0.0.0/README.md
--rw-r--r--   0        0        0       25 2024-05-30 22:14:38.279086 beforerr-0.0.0/beforerr/__init__.py
--rw-r--r--   0        0        0     2609 2024-05-30 21:25:24.448237 beforerr-0.0.0/beforerr/_modidx.py
--rw-r--r--   0        0        0      338 2024-05-30 21:25:23.994230 beforerr-0.0.0/beforerr/basics.py
--rw-r--r--   0        0        0      214 2024-05-30 21:25:23.993466 beforerr-0.0.0/beforerr/core.py
--rw-r--r--   0        0        0      965 2024-05-30 21:25:23.996239 beforerr-0.0.0/beforerr/matplotlib.py
--rw-r--r--   0        0        0     2394 2024-05-30 21:25:23.998261 beforerr-0.0.0/beforerr/polars.py
--rw-r--r--   0        0        0     5200 2024-05-30 21:25:24.001286 beforerr-0.0.0/beforerr/project.py
--rw-r--r--   0        0        0      811 2024-05-30 21:25:23.995358 beforerr-0.0.0/beforerr/r.py
--rw-r--r--   0        0        0      886 2024-05-30 22:38:37.779371 beforerr-0.0.0/pyproject.toml
--rw-r--r--   0        0        0      654 1970-01-01 00:00:00.000000 beforerr-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11337 2023-04-27 10:12:58.000000 beforerr-0.1.0/LICENSE
+-rw-r--r--   0        0        0       22 2024-02-18 16:43:58.046819 beforerr-0.1.0/beforerr/__init__.py
+-rw-r--r--   0        0        0     2609 2024-05-30 19:55:52.023915 beforerr-0.1.0/beforerr/_modidx.py
+-rw-r--r--   0        0        0      338 2024-05-26 19:40:30.375661 beforerr-0.1.0/beforerr/basics.py
+-rw-r--r--   0        0        0      214 2024-05-26 19:40:30.375751 beforerr-0.1.0/beforerr/core.py
+-rw-r--r--   0        0        0      965 2024-05-26 19:40:30.375814 beforerr-0.1.0/beforerr/matplotlib.py
+-rw-r--r--   0        0        0     2394 2024-02-18 16:43:58.046191 beforerr-0.1.0/beforerr/polars.py
+-rw-r--r--   0        0        0     5200 2024-05-30 19:55:52.024827 beforerr-0.1.0/beforerr/project.py
+-rw-r--r--   0        0        0      811 2024-02-18 16:43:58.043275 beforerr-0.1.0/beforerr/r.py
+-rw-r--r--   0        0        0      774 2024-05-30 20:15:38.628699 beforerr-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      296 1970-01-01 00:00:00.000000 beforerr-0.1.0/PKG-INFO
```

### Comparing `beforerr-0.0.0/LICENSE` & `beforerr-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `beforerr-0.0.0/beforerr/_modidx.py` & `beforerr-0.1.0/beforerr/_modidx.py`

 * *Files identical despite different names*

### Comparing `beforerr-0.0.0/beforerr/matplotlib.py` & `beforerr-0.1.0/beforerr/matplotlib.py`

 * *Files identical despite different names*

### Comparing `beforerr-0.0.0/beforerr/polars.py` & `beforerr-0.1.0/beforerr/polars.py`

 * *Files identical despite different names*

### Comparing `beforerr-0.0.0/beforerr/project.py` & `beforerr-0.1.0/beforerr/project.py`

 * *Files identical despite different names*

### Comparing `beforerr-0.0.0/beforerr/r.py` & `beforerr-0.1.0/beforerr/r.py`

 * *Files identical despite different names*

