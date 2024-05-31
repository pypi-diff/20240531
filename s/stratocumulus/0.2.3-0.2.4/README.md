# Comparing `tmp/stratocumulus-0.2.3.tar.gz` & `tmp/stratocumulus-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stratocumulus-0.2.3.tar", last modified: Tue May  7 22:45:05 2024, max compression
+gzip compressed data, was "stratocumulus-0.2.4.tar", last modified: Fri May 31 20:40:59 2024, max compression
```

## Comparing `stratocumulus-0.2.3.tar` & `stratocumulus-0.2.4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2024-05-07 22:45:05.691191 stratocumulus-0.2.3/
-drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2024-05-07 22:45:05.674279 stratocumulus-0.2.3/.github/
-drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2024-05-07 22:45:05.677077 stratocumulus-0.2.3/.github/workflows/
--rw-r--r--   0 yangy197   (501) staff       (20)      703 2022-09-28 20:06:45.000000 stratocumulus-0.2.3/.github/workflows/test.yml
--rw-r--r--   0 yangy197   (501) staff       (20)     1532 2021-08-19 16:43:59.000000 stratocumulus-0.2.3/LICENSE
--rw-r--r--   0 yangy197   (501) staff       (20)       62 2021-08-19 16:43:59.000000 stratocumulus-0.2.3/MANIFEST.in
--rw-r--r--   0 yangy197   (501) staff       (20)     7259 2024-05-07 22:45:05.690561 stratocumulus-0.2.3/PKG-INFO
--rw-r--r--   0 yangy197   (501) staff       (20)     4433 2022-09-28 20:06:45.000000 stratocumulus-0.2.3/README.rst
--rw-r--r--   0 yangy197   (501) staff       (20)     1974 2023-03-21 21:30:56.000000 stratocumulus-0.2.3/pyproject.toml
--rw-r--r--   0 yangy197   (501) staff       (20)       38 2024-05-07 22:45:05.691321 stratocumulus-0.2.3/setup.cfg
-drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2024-05-07 22:45:05.678561 stratocumulus-0.2.3/strato/
--rw-r--r--   0 yangy197   (501) staff       (20)        0 2021-11-10 17:34:26.000000 stratocumulus-0.2.3/strato/__init__.py
--rw-r--r--   0 yangy197   (501) staff       (20)     1020 2022-09-28 20:06:45.000000 stratocumulus-0.2.3/strato/__main__.py
-drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2024-05-07 22:45:05.681115 stratocumulus-0.2.3/strato/backends/
--rw-r--r--   0 yangy197   (501) staff       (20)      133 2022-09-28 20:06:45.000000 stratocumulus-0.2.3/strato/backends/__init__.py
--rw-r--r--   0 yangy197   (501) staff       (20)     4524 2023-03-21 21:26:55.000000 stratocumulus-0.2.3/strato/backends/_aws.py
--rw-r--r--   0 yangy197   (501) staff       (20)     2531 2022-09-28 20:06:45.000000 stratocumulus-0.2.3/strato/backends/_gcp.py
--rw-r--r--   0 yangy197   (501) staff       (20)     2640 2024-05-07 22:42:03.000000 stratocumulus-0.2.3/strato/backends/_local.py
-drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2024-05-07 22:45:05.683725 stratocumulus-0.2.3/strato/commands/
--rw-r--r--   0 yangy197   (501) staff       (20)        0 2021-11-10 17:34:26.000000 stratocumulus-0.2.3/strato/commands/__init__.py
--rw-r--r--   0 yangy197   (501) staff       (20)     2719 2023-03-20 20:53:11.000000 stratocumulus-0.2.3/strato/commands/cp.py
--rw-r--r--   0 yangy197   (501) staff       (20)     1360 2022-09-28 20:06:45.000000 stratocumulus-0.2.3/strato/commands/exists.py
--rw-r--r--   0 yangy197   (501) staff       (20)     2312 2022-09-28 20:06:45.000000 stratocumulus-0.2.3/strato/commands/rm.py
--rw-r--r--   0 yangy197   (501) staff       (20)     2457 2022-09-28 20:06:45.000000 stratocumulus-0.2.3/strato/commands/sync.py
--rw-r--r--   0 yangy197   (501) staff       (20)     1135 2022-09-28 20:06:45.000000 stratocumulus-0.2.3/strato/commands/util.py
-drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2024-05-07 22:45:05.686337 stratocumulus-0.2.3/strato/tests/
--rw-r--r--   0 yangy197   (501) staff       (20)       72 2022-09-28 20:06:45.000000 stratocumulus-0.2.3/strato/tests/helpers.py
--rw-r--r--   0 yangy197   (501) staff       (20)      444 2022-09-28 20:06:45.000000 stratocumulus-0.2.3/strato/tests/test_backend.py
--rw-r--r--   0 yangy197   (501) staff       (20)     1271 2024-05-06 23:02:54.000000 stratocumulus-0.2.3/strato/tests/test_cp.py
--rw-r--r--   0 yangy197   (501) staff       (20)     1071 2022-09-28 20:06:45.000000 stratocumulus-0.2.3/strato/tests/test_rm.py
--rw-r--r--   0 yangy197   (501) staff       (20)      592 2022-09-28 20:06:45.000000 stratocumulus-0.2.3/strato/tests/test_sync.py
--rw-r--r--   0 yangy197   (501) staff       (20)      411 2024-05-07 22:45:05.000000 stratocumulus-0.2.3/strato/version.py
-drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2024-05-07 22:45:05.689358 stratocumulus-0.2.3/stratocumulus.egg-info/
--rw-r--r--   0 yangy197   (501) staff       (20)     7259 2024-05-07 22:45:05.000000 stratocumulus-0.2.3/stratocumulus.egg-info/PKG-INFO
--rw-r--r--   0 yangy197   (501) staff       (20)      727 2024-05-07 22:45:05.000000 stratocumulus-0.2.3/stratocumulus.egg-info/SOURCES.txt
--rw-r--r--   0 yangy197   (501) staff       (20)        1 2024-05-07 22:45:05.000000 stratocumulus-0.2.3/stratocumulus.egg-info/dependency_links.txt
--rw-r--r--   0 yangy197   (501) staff       (20)       48 2024-05-07 22:45:05.000000 stratocumulus-0.2.3/stratocumulus.egg-info/entry_points.txt
--rw-r--r--   0 yangy197   (501) staff       (20)       71 2024-05-07 22:45:05.000000 stratocumulus-0.2.3/stratocumulus.egg-info/requires.txt
--rw-r--r--   0 yangy197   (501) staff       (20)        7 2024-05-07 22:45:05.000000 stratocumulus-0.2.3/stratocumulus.egg-info/top_level.txt
+drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2024-05-31 20:40:59.434743 stratocumulus-0.2.4/
+drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2024-05-31 20:40:59.407508 stratocumulus-0.2.4/.github/
+drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2024-05-31 20:40:59.410784 stratocumulus-0.2.4/.github/workflows/
+-rw-r--r--   0 yangy197   (501) staff       (20)      703 2022-09-28 20:06:45.000000 stratocumulus-0.2.4/.github/workflows/test.yml
+-rw-r--r--   0 yangy197   (501) staff       (20)     1532 2021-08-19 16:43:59.000000 stratocumulus-0.2.4/LICENSE
+-rw-r--r--   0 yangy197   (501) staff       (20)       62 2021-08-19 16:43:59.000000 stratocumulus-0.2.4/MANIFEST.in
+-rw-r--r--   0 yangy197   (501) staff       (20)     7259 2024-05-31 20:40:59.433859 stratocumulus-0.2.4/PKG-INFO
+-rw-r--r--   0 yangy197   (501) staff       (20)     4433 2022-09-28 20:06:45.000000 stratocumulus-0.2.4/README.rst
+-rw-r--r--   0 yangy197   (501) staff       (20)     1974 2023-03-21 21:30:56.000000 stratocumulus-0.2.4/pyproject.toml
+-rw-r--r--   0 yangy197   (501) staff       (20)       38 2024-05-31 20:40:59.435011 stratocumulus-0.2.4/setup.cfg
+drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2024-05-31 20:40:59.412633 stratocumulus-0.2.4/strato/
+-rw-r--r--   0 yangy197   (501) staff       (20)        0 2021-11-10 17:34:26.000000 stratocumulus-0.2.4/strato/__init__.py
+-rw-r--r--   0 yangy197   (501) staff       (20)     1020 2022-09-28 20:06:45.000000 stratocumulus-0.2.4/strato/__main__.py
+drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2024-05-31 20:40:59.416019 stratocumulus-0.2.4/strato/backends/
+-rw-r--r--   0 yangy197   (501) staff       (20)      133 2022-09-28 20:06:45.000000 stratocumulus-0.2.4/strato/backends/__init__.py
+-rw-r--r--   0 yangy197   (501) staff       (20)     4524 2023-03-21 21:26:55.000000 stratocumulus-0.2.4/strato/backends/_aws.py
+-rw-r--r--   0 yangy197   (501) staff       (20)     2531 2022-09-28 20:06:45.000000 stratocumulus-0.2.4/strato/backends/_gcp.py
+-rw-r--r--   0 yangy197   (501) staff       (20)     2811 2024-05-29 17:48:54.000000 stratocumulus-0.2.4/strato/backends/_local.py
+drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2024-05-31 20:40:59.422615 stratocumulus-0.2.4/strato/commands/
+-rw-r--r--   0 yangy197   (501) staff       (20)        0 2021-11-10 17:34:26.000000 stratocumulus-0.2.4/strato/commands/__init__.py
+-rw-r--r--   0 yangy197   (501) staff       (20)     2719 2024-05-08 20:15:44.000000 stratocumulus-0.2.4/strato/commands/cp.py
+-rw-r--r--   0 yangy197   (501) staff       (20)     1360 2022-09-28 20:06:45.000000 stratocumulus-0.2.4/strato/commands/exists.py
+-rw-r--r--   0 yangy197   (501) staff       (20)     2312 2022-09-28 20:06:45.000000 stratocumulus-0.2.4/strato/commands/rm.py
+-rw-r--r--   0 yangy197   (501) staff       (20)     2457 2022-09-28 20:06:45.000000 stratocumulus-0.2.4/strato/commands/sync.py
+-rw-r--r--   0 yangy197   (501) staff       (20)     1135 2022-09-28 20:06:45.000000 stratocumulus-0.2.4/strato/commands/util.py
+drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2024-05-31 20:40:59.426831 stratocumulus-0.2.4/strato/tests/
+-rw-r--r--   0 yangy197   (501) staff       (20)       72 2022-09-28 20:06:45.000000 stratocumulus-0.2.4/strato/tests/helpers.py
+-rw-r--r--   0 yangy197   (501) staff       (20)      444 2022-09-28 20:06:45.000000 stratocumulus-0.2.4/strato/tests/test_backend.py
+-rw-r--r--   0 yangy197   (501) staff       (20)     1271 2024-05-06 23:02:54.000000 stratocumulus-0.2.4/strato/tests/test_cp.py
+-rw-r--r--   0 yangy197   (501) staff       (20)     1071 2022-09-28 20:06:45.000000 stratocumulus-0.2.4/strato/tests/test_rm.py
+-rw-r--r--   0 yangy197   (501) staff       (20)      592 2022-09-28 20:06:45.000000 stratocumulus-0.2.4/strato/tests/test_sync.py
+-rw-r--r--   0 yangy197   (501) staff       (20)      411 2024-05-31 20:40:59.000000 stratocumulus-0.2.4/strato/version.py
+drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2024-05-31 20:40:59.432296 stratocumulus-0.2.4/stratocumulus.egg-info/
+-rw-r--r--   0 yangy197   (501) staff       (20)     7259 2024-05-31 20:40:59.000000 stratocumulus-0.2.4/stratocumulus.egg-info/PKG-INFO
+-rw-r--r--   0 yangy197   (501) staff       (20)      727 2024-05-31 20:40:59.000000 stratocumulus-0.2.4/stratocumulus.egg-info/SOURCES.txt
+-rw-r--r--   0 yangy197   (501) staff       (20)        1 2024-05-31 20:40:59.000000 stratocumulus-0.2.4/stratocumulus.egg-info/dependency_links.txt
+-rw-r--r--   0 yangy197   (501) staff       (20)       48 2024-05-31 20:40:59.000000 stratocumulus-0.2.4/stratocumulus.egg-info/entry_points.txt
+-rw-r--r--   0 yangy197   (501) staff       (20)       71 2024-05-31 20:40:59.000000 stratocumulus-0.2.4/stratocumulus.egg-info/requires.txt
+-rw-r--r--   0 yangy197   (501) staff       (20)        7 2024-05-31 20:40:59.000000 stratocumulus-0.2.4/stratocumulus.egg-info/top_level.txt
```

### Comparing `stratocumulus-0.2.3/.github/workflows/test.yml` & `stratocumulus-0.2.4/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `stratocumulus-0.2.3/LICENSE` & `stratocumulus-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `stratocumulus-0.2.3/PKG-INFO` & `stratocumulus-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stratocumulus
-Version: 0.2.3
+Version: 0.2.4
 Summary: File backend component of Cumulus
 Author-email: "Yiming Yang, Joshua Gould, Rimte Rocher, Bo Li" <cumulus-support@googlegroups.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2021, klarman-cell-observatory
         All rights reserved.
```

### Comparing `stratocumulus-0.2.3/README.rst` & `stratocumulus-0.2.4/README.rst`

 * *Files identical despite different names*

### Comparing `stratocumulus-0.2.3/pyproject.toml` & `stratocumulus-0.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `stratocumulus-0.2.3/strato/__main__.py` & `stratocumulus-0.2.4/strato/__main__.py`

 * *Files identical despite different names*

### Comparing `stratocumulus-0.2.3/strato/backends/_aws.py` & `stratocumulus-0.2.4/strato/backends/_aws.py`

 * *Files identical despite different names*

### Comparing `stratocumulus-0.2.3/strato/backends/_gcp.py` & `stratocumulus-0.2.4/strato/backends/_gcp.py`

 * *Files identical despite different names*

### Comparing `stratocumulus-0.2.3/strato/backends/_local.py` & `stratocumulus-0.2.4/strato/backends/_local.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,20 +52,25 @@
             print(" ".join(call_args))
         if not dryrun:
             check_call(call_args)
 
     def sync(self, ionice, source, target, quiet, dryrun):
         if shutil.which("rsync") is None:
             raise Exception("rsync is not installed!")
-        target = os.path.dirname(target)
+        # target = os.path.dirname(target)
+        os.makedirs(target, exist_ok=True)
         call_args = (
             ["ionice", "-c", "2", "-n", "7"]
             if ionice and (shutil.which("ionice")) is not None
             else []
         )
+        if not source.endswith("/"):
+            source += "/"
+        if not target.endswith("/"):
+            target += "/"
         call_args += ["rsync", "-r", "--delete", source, target]
         if not quiet or dryrun:
             print(" ".join(call_args))
         if not dryrun:
             check_call(call_args)
 
     def delete(self, recursive, filenames, quiet, dryrun):
```

### Comparing `stratocumulus-0.2.3/strato/commands/cp.py` & `stratocumulus-0.2.4/strato/commands/cp.py`

 * *Files identical despite different names*

### Comparing `stratocumulus-0.2.3/strato/commands/exists.py` & `stratocumulus-0.2.4/strato/commands/exists.py`

 * *Files identical despite different names*

### Comparing `stratocumulus-0.2.3/strato/commands/rm.py` & `stratocumulus-0.2.4/strato/commands/rm.py`

 * *Files identical despite different names*

### Comparing `stratocumulus-0.2.3/strato/commands/sync.py` & `stratocumulus-0.2.4/strato/commands/sync.py`

 * *Files identical despite different names*

### Comparing `stratocumulus-0.2.3/strato/commands/util.py` & `stratocumulus-0.2.4/strato/commands/util.py`

 * *Files identical despite different names*

### Comparing `stratocumulus-0.2.3/strato/tests/test_cp.py` & `stratocumulus-0.2.4/strato/tests/test_cp.py`

 * *Files identical despite different names*

### Comparing `stratocumulus-0.2.3/strato/tests/test_rm.py` & `stratocumulus-0.2.4/strato/tests/test_rm.py`

 * *Files identical despite different names*

### Comparing `stratocumulus-0.2.3/strato/tests/test_sync.py` & `stratocumulus-0.2.4/strato/tests/test_sync.py`

 * *Files identical despite different names*

### Comparing `stratocumulus-0.2.3/stratocumulus.egg-info/PKG-INFO` & `stratocumulus-0.2.4/stratocumulus.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stratocumulus
-Version: 0.2.3
+Version: 0.2.4
 Summary: File backend component of Cumulus
 Author-email: "Yiming Yang, Joshua Gould, Rimte Rocher, Bo Li" <cumulus-support@googlegroups.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2021, klarman-cell-observatory
         All rights reserved.
```

### Comparing `stratocumulus-0.2.3/stratocumulus.egg-info/SOURCES.txt` & `stratocumulus-0.2.4/stratocumulus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

