# Comparing `tmp/libcache-1.0.tar.gz` & `tmp/libcache-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libcache-1.0.tar", last modified: Thu May 30 19:13:24 2024, max compression
+gzip compressed data, was "libcache-1.1.tar", last modified: Thu May 30 20:18:21 2024, max compression
```

## Comparing `libcache-1.0.tar` & `libcache-1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 19:13:24.694874 libcache-1.0/
--rw-r--r--   0 root         (0) root         (0)      542 2024-05-30 19:13:24.690874 libcache-1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      101 2024-05-30 19:12:21.000000 libcache-1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 19:13:24.686874 libcache-1.0/libcache/
--rw-rw-rw-   0 root         (0) root         (0)     2005 2024-05-30 19:12:21.000000 libcache-1.0/libcache/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 19:13:24.690874 libcache-1.0/libcache.egg-info/
--rw-r--r--   0 root         (0) root         (0)      542 2024-05-30 19:13:24.000000 libcache-1.0/libcache.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      187 2024-05-30 19:13:24.000000 libcache-1.0/libcache.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 19:13:24.000000 libcache-1.0/libcache.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-30 19:13:24.000000 libcache-1.0/libcache.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-30 19:13:24.694874 libcache-1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      796 2024-05-30 19:12:21.000000 libcache-1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 19:13:24.690874 libcache-1.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)      439 2024-05-30 19:12:21.000000 libcache-1.0/tests/test_cache.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 20:18:21.113734 libcache-1.1/
+-rw-r--r--   0 root         (0) root         (0)      542 2024-05-30 20:18:21.109733 libcache-1.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      101 2024-05-30 19:12:21.000000 libcache-1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 20:18:21.105733 libcache-1.1/libcache/
+-rw-rw-rw-   0 root         (0) root         (0)     2027 2024-05-30 20:17:29.000000 libcache-1.1/libcache/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 20:18:21.109733 libcache-1.1/libcache.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      542 2024-05-30 20:18:21.000000 libcache-1.1/libcache.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      187 2024-05-30 20:18:21.000000 libcache-1.1/libcache.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 20:18:21.000000 libcache-1.1/libcache.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-30 20:18:21.000000 libcache-1.1/libcache.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-30 20:18:21.113734 libcache-1.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      796 2024-05-30 20:17:29.000000 libcache-1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 20:18:21.109733 libcache-1.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      439 2024-05-30 19:12:21.000000 libcache-1.1/tests/test_cache.py
```

### Comparing `libcache-1.0/PKG-INFO` & `libcache-1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libcache
-Version: 1.0
+Version: 1.1
 Summary: Simple cache with TTL
 Home-page: https://flerken.zapto.org:1115/kuba/libcache
 Author: kuba201
 Project-URL: Source, https://flerken.zapto.org:1115/kuba/libcache
 Keywords: cache,temp,ttl
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `libcache-1.0/libcache/__init__.py` & `libcache-1.1/libcache/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+__version__ = 1.1
 import time
 from dataclasses import dataclass
 @dataclass
 class CacheEntry:
     key: str
     value: str
     ttl: int
@@ -19,17 +20,17 @@
             if (time.time()-entry.saved) > entry.ttl:
                 self.cache.remove(entry)
                 continue
             if entry.key == key:
                 return entry.value
         if aggressive: raise NotInCache
         else: return None
-    def saveElement(self, key: str, value, ttl=(5*60)):
-        try: assert self.doesElementExist(key) == False
-        except AssertionError: raise AlreadyInCache
+    def saveElement(self, key: str, value, ttl=(5*60), aggressive:bool=False):
+        if self.doesElementExist(key) and aggressive:
+            raise AlreadyInCache()
         self.cache.insert(0, CacheEntry(key, value, ttl, time.time()))
         return value
     def doesElementExist(self, key:str):
         found = False
         for entry in self.cache:
             if (time.time()-entry.saved) > entry.ttl:
                 self.cache.remove(entry)
```

### Comparing `libcache-1.0/libcache.egg-info/PKG-INFO` & `libcache-1.1/libcache.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libcache
-Version: 1.0
+Version: 1.1
 Summary: Simple cache with TTL
 Home-page: https://flerken.zapto.org:1115/kuba/libcache
 Author: kuba201
 Project-URL: Source, https://flerken.zapto.org:1115/kuba/libcache
 Keywords: cache,temp,ttl
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `libcache-1.0/setup.py` & `libcache-1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', encoding='utf-8') as f:
     readme = f.read()
 
 setup(
         name="libcache", 
-        version="1.0",
+        version="1.1",
         author="kuba201",
         description='Simple cache with TTL',
         long_description=readme,
         long_description_content_type='text/markdown',
         packages=find_packages(),
         url="https://flerken.zapto.org:1115/kuba/libcache",
         install_requires=[],
```

