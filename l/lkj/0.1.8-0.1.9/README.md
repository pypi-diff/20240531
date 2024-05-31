# Comparing `tmp/lkj-0.1.8.tar.gz` & `tmp/lkj-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lkj-0.1.8.tar", last modified: Fri Feb  9 12:49:07 2024, max compression
+gzip compressed data, was "lkj-0.1.9.tar", last modified: Fri Feb 23 13:46:53 2024, max compression
```

## Comparing `lkj-0.1.8.tar` & `lkj-0.1.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:49:07.344043 lkj-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-09 12:48:18.000000 lkj-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-02-09 12:49:07.344043 lkj-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-02-09 12:48:18.000000 lkj-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:49:07.340043 lkj-0.1.8/lkj/
--rw-r--r--   0 runner    (1001) docker     (127)     5816 2024-02-09 12:48:18.000000 lkj-0.1.8/lkj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6779 2024-02-09 12:49:03.000000 lkj-0.1.8/lkj/filesys.py
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-02-09 12:48:18.000000 lkj-0.1.8/lkj/strings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:49:07.344043 lkj-0.1.8/lkj.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-02-09 12:49:06.000000 lkj-0.1.8/lkj.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-02-09 12:49:07.000000 lkj-0.1.8/lkj.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-09 12:49:06.000000 lkj-0.1.8/lkj.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-09 12:49:06.000000 lkj-0.1.8/lkj.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-02-09 12:49:06.000000 lkj-0.1.8/lkj.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-02-09 12:49:07.344043 lkj-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-02-09 12:48:18.000000 lkj-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 13:46:53.968688 lkj-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-23 13:46:27.000000 lkj-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-02-23 13:46:53.968688 lkj-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-02-23 13:46:27.000000 lkj-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 13:46:53.968688 lkj-0.1.9/lkj/
+-rw-r--r--   0 runner    (1001) docker     (127)     7538 2024-02-23 13:46:27.000000 lkj-0.1.9/lkj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6779 2024-02-23 13:46:27.000000 lkj-0.1.9/lkj/filesys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-02-23 13:46:27.000000 lkj-0.1.9/lkj/strings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 13:46:53.968688 lkj-0.1.9/lkj.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-02-23 13:46:53.000000 lkj-0.1.9/lkj.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-02-23 13:46:53.000000 lkj-0.1.9/lkj.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-23 13:46:53.000000 lkj-0.1.9/lkj.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-23 13:46:53.000000 lkj-0.1.9/lkj.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-02-23 13:46:53.000000 lkj-0.1.9/lkj.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-02-23 13:46:53.968688 lkj-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-02-23 13:46:27.000000 lkj-0.1.9/setup.py
```

### Comparing `lkj-0.1.8/LICENSE` & `lkj-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lkj-0.1.8/PKG-INFO` & `lkj-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lkj
-Version: 0.1.8
+Version: 0.1.9
 Summary: A dump of homeless useful utils
 Home-page: https://github.com/thorwhalen/lkj
 Author: Thor Whalen
 License: apache-2.0
 Description: # lkj
         
         Lightweight Kit Jumpstart. A place for useful python utils built only with pure python.
```

### Comparing `lkj-0.1.8/lkj/filesys.py` & `lkj-0.1.9/lkj/filesys.py`

 * *Files identical despite different names*

### Comparing `lkj-0.1.8/lkj/strings.py` & `lkj-0.1.9/lkj/strings.py`

 * *Files identical despite different names*

### Comparing `lkj-0.1.8/lkj.egg-info/PKG-INFO` & `lkj-0.1.9/lkj.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lkj
-Version: 0.1.8
+Version: 0.1.9
 Summary: A dump of homeless useful utils
 Home-page: https://github.com/thorwhalen/lkj
 Author: Thor Whalen
 License: apache-2.0
 Description: # lkj
         
         Lightweight Kit Jumpstart. A place for useful python utils built only with pure python.
```

