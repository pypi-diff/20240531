# Comparing `tmp/resages-0.2.tar.gz` & `tmp/resages-0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resages-0.2.tar", last modified: Fri May 31 10:16:34 2024, max compression
+gzip compressed data, was "resages-0.21.tar", last modified: Fri May 31 12:32:29 2024, max compression
```

## Comparing `resages-0.2.tar` & `resages-0.21.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 10:16:34.720601 resages-0.2/
--rw-rw-rw-   0        0        0      261 2024-05-31 10:16:34.714578 resages-0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-31 10:16:34.535993 resages-0.2/resages/
--rw-rw-rw-   0        0        0        0 2024-05-31 08:12:38.000000 resages-0.2/resages/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-31 10:16:34.651615 resages-0.2/resages/colyear/
--rw-rw-rw-   0        0        0        0 2024-05-31 08:12:38.000000 resages-0.2/resages/colyear/__init__.py
--rw-rw-rw-   0        0        0     1932 2024-05-31 08:12:38.000000 resages-0.2/resages/colyear/abs.py
--rw-rw-rw-   0        0        0     5483 2024-05-31 08:12:38.000000 resages-0.2/resages/colyear/colyear.py
-drwxrwxrwx   0        0        0        0 2024-05-31 10:16:34.680619 resages-0.2/resages/rad2/
--rw-rw-rw-   0        0        0    11599 2024-05-31 08:12:38.000000 resages-0.2/resages/rad2/Rad2.py
--rw-rw-rw-   0        0        0        0 2024-05-31 08:12:38.000000 resages-0.2/resages/rad2/__init__.py
--rw-rw-rw-   0        0        0     1932 2024-05-31 08:12:38.000000 resages-0.2/resages/rad2/abs.py
-drwxrwxrwx   0        0        0        0 2024-05-31 10:16:34.713605 resages-0.2/resages/radical/
--rw-rw-rw-   0        0        0        0 2024-05-26 13:53:18.000000 resages-0.2/resages/radical/__init__.py
--rw-rw-rw-   0        0        0     1932 2024-05-28 05:16:31.000000 resages-0.2/resages/radical/abs.py
--rw-rw-rw-   0        0        0    36636 2024-05-31 08:12:38.000000 resages-0.2/resages/radical/radical.py
-drwxrwxrwx   0        0        0        0 2024-05-31 10:16:34.607995 resages-0.2/resages.egg-info/
--rw-rw-rw-   0        0        0      261 2024-05-31 10:16:34.000000 resages-0.2/resages.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      404 2024-05-31 10:16:34.000000 resages-0.2/resages.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 10:16:34.000000 resages-0.2/resages.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-05-31 10:16:34.000000 resages-0.2/resages.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-31 10:16:34.000000 resages-0.2/resages.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-31 10:16:34.720601 resages-0.2/setup.cfg
--rw-rw-rw-   0        0        0      652 2024-05-31 10:09:10.000000 resages-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 12:32:29.653539 resages-0.21/
+-rw-rw-rw-   0        0        0     1089 2024-05-31 12:27:15.000000 resages-0.21/LICENSE
+-rw-rw-rw-   0        0        0     4986 2024-05-31 12:32:29.653539 resages-0.21/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-31 12:32:29.637118 resages-0.21/resages/
+-rw-rw-rw-   0        0        0        0 2024-05-31 08:12:38.000000 resages-0.21/resages/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 12:32:29.653539 resages-0.21/resages/colyear/
+-rw-rw-rw-   0        0        0        0 2024-05-31 08:12:38.000000 resages-0.21/resages/colyear/__init__.py
+-rw-rw-rw-   0        0        0     1932 2024-05-31 08:12:38.000000 resages-0.21/resages/colyear/abs.py
+-rw-rw-rw-   0        0        0     5483 2024-05-31 08:12:38.000000 resages-0.21/resages/colyear/colyear.py
+drwxrwxrwx   0        0        0        0 2024-05-31 12:32:29.653539 resages-0.21/resages/rad2/
+-rw-rw-rw-   0        0        0    11599 2024-05-31 08:12:38.000000 resages-0.21/resages/rad2/Rad2.py
+-rw-rw-rw-   0        0        0        0 2024-05-31 08:12:38.000000 resages-0.21/resages/rad2/__init__.py
+-rw-rw-rw-   0        0        0     1932 2024-05-31 08:12:38.000000 resages-0.21/resages/rad2/abs.py
+drwxrwxrwx   0        0        0        0 2024-05-31 12:32:29.653539 resages-0.21/resages/radical/
+-rw-rw-rw-   0        0        0        0 2024-05-26 13:53:18.000000 resages-0.21/resages/radical/__init__.py
+-rw-rw-rw-   0        0        0     1932 2024-05-28 05:16:31.000000 resages-0.21/resages/radical/abs.py
+-rw-rw-rw-   0        0        0    36636 2024-05-31 08:12:38.000000 resages-0.21/resages/radical/radical.py
+drwxrwxrwx   0        0        0        0 2024-05-31 12:32:29.653539 resages-0.21/resages.egg-info/
+-rw-rw-rw-   0        0        0     4986 2024-05-31 12:32:29.000000 resages-0.21/resages.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      412 2024-05-31 12:32:29.000000 resages-0.21/resages.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 12:32:29.000000 resages-0.21/resages.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-05-31 12:32:29.000000 resages-0.21/resages.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-31 12:32:29.000000 resages-0.21/resages.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-31 12:32:29.653539 resages-0.21/setup.cfg
+-rw-rw-rw-   0        0        0      998 2024-05-31 12:32:15.000000 resages-0.21/setup.py
```

### Comparing `resages-0.2/resages/colyear/abs.py` & `resages-0.21/resages/colyear/abs.py`

 * *Files identical despite different names*

### Comparing `resages-0.2/resages/colyear/colyear.py` & `resages-0.21/resages/colyear/colyear.py`

 * *Files identical despite different names*

### Comparing `resages-0.2/resages/rad2/Rad2.py` & `resages-0.21/resages/rad2/Rad2.py`

 * *Files identical despite different names*

### Comparing `resages-0.2/resages/rad2/abs.py` & `resages-0.21/resages/rad2/abs.py`

 * *Files identical despite different names*

### Comparing `resages-0.2/resages/radical/abs.py` & `resages-0.21/resages/radical/abs.py`

 * *Files identical despite different names*

### Comparing `resages-0.2/resages/radical/radical.py` & `resages-0.21/resages/radical/radical.py`

 * *Files identical despite different names*

