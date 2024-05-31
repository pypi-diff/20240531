# Comparing `tmp/tsv2py-0.6.2.tar.gz` & `tmp/tsv2py-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsv2py-0.6.2.tar", last modified: Fri Mar 29 08:46:47 2024, max compression
+gzip compressed data, was "tsv2py-0.6.3.tar", last modified: Fri May 31 07:02:01 2024, max compression
```

## Comparing `tsv2py-0.6.2.tar` & `tsv2py-0.6.3.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2024-03-29 08:46:47.615173 tsv2py-0.6.2/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1077 2024-02-01 18:54:17.000000 tsv2py-0.6.2/LICENSE
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     7118 2024-03-29 08:46:47.614939 tsv2py-0.6.2/PKG-INFO
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     6006 2023-11-20 13:06:33.000000 tsv2py-0.6.2/README.md
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2024-03-29 08:46:47.604646 tsv2py-0.6.2/lib/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)    43547 2024-03-29 08:41:21.000000 tsv2py-0.6.2/lib/tsv_parser.c
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      140 2024-02-01 18:38:25.000000 tsv2py-0.6.2/pyproject.toml
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1176 2024-03-29 08:46:47.616310 tsv2py-0.6.2/setup.cfg
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1810 2024-03-25 20:23:21.000000 tsv2py-0.6.2/setup.py
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2024-03-29 08:46:47.606866 tsv2py-0.6.2/tests/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1930 2023-11-22 23:25:39.000000 tsv2py-0.6.2/tests/test_fuzz.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)    11235 2024-03-19 08:08:34.000000 tsv2py-0.6.2/tests/test_perf.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)    11690 2024-03-29 08:45:51.000000 tsv2py-0.6.2/tests/test_tsv.py
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2024-03-29 08:46:47.609567 tsv2py-0.6.2/tsv/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      506 2024-03-29 08:28:18.000000 tsv2py-0.6.2/tsv/__init__.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     7008 2023-11-22 23:48:38.000000 tsv2py-0.6.2/tsv/helper.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1951 2023-11-17 19:16:00.000000 tsv2py-0.6.2/tsv/parser.pyi
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-06-28 23:16:45.000000 tsv2py-0.6.2/tsv/py.typed
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2024-03-29 08:46:47.613874 tsv2py-0.6.2/tsv2py.egg-info/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     7118 2024-03-29 08:46:47.000000 tsv2py-0.6.2/tsv2py.egg-info/PKG-INFO
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      327 2024-03-29 08:46:47.000000 tsv2py-0.6.2/tsv2py.egg-info/SOURCES.txt
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        1 2024-03-29 08:46:47.000000 tsv2py-0.6.2/tsv2py.egg-info/dependency_links.txt
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        4 2024-03-29 08:46:47.000000 tsv2py-0.6.2/tsv2py.egg-info/top_level.txt
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        1 2024-03-29 08:46:47.000000 tsv2py-0.6.2/tsv2py.egg-info/zip-safe
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2024-05-31 07:02:01.597119 tsv2py-0.6.3/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1077 2024-02-01 18:54:17.000000 tsv2py-0.6.3/LICENSE
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)       52 2024-05-31 06:52:21.000000 tsv2py-0.6.3/MANIFEST.in
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     7118 2024-05-31 07:02:01.596865 tsv2py-0.6.3/PKG-INFO
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     6006 2023-11-20 13:06:33.000000 tsv2py-0.6.3/README.md
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2024-05-31 07:02:01.588013 tsv2py-0.6.3/lib/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    43547 2024-03-29 08:41:21.000000 tsv2py-0.6.3/lib/tsv_parser.c
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      140 2024-02-01 18:38:25.000000 tsv2py-0.6.3/pyproject.toml
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1176 2024-05-31 07:02:01.598108 tsv2py-0.6.3/setup.cfg
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1971 2024-05-30 13:07:59.000000 tsv2py-0.6.3/setup.py
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2024-05-31 07:02:01.589891 tsv2py-0.6.3/tests/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1930 2023-11-22 23:25:39.000000 tsv2py-0.6.3/tests/test_fuzz.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    11235 2024-03-19 08:08:34.000000 tsv2py-0.6.3/tests/test_perf.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    11690 2024-03-29 08:45:51.000000 tsv2py-0.6.3/tests/test_tsv.py
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2024-05-31 07:02:01.592776 tsv2py-0.6.3/tsv/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      506 2024-05-30 13:13:42.000000 tsv2py-0.6.3/tsv/__init__.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     7027 2024-04-09 08:42:55.000000 tsv2py-0.6.3/tsv/helper.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1951 2023-11-17 19:16:00.000000 tsv2py-0.6.3/tsv/parser.pyi
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-06-28 23:16:45.000000 tsv2py-0.6.3/tsv/py.typed
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2024-05-31 07:02:01.596190 tsv2py-0.6.3/tsv2py.egg-info/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     7118 2024-05-31 07:02:01.000000 tsv2py-0.6.3/tsv2py.egg-info/PKG-INFO
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      339 2024-05-31 07:02:01.000000 tsv2py-0.6.3/tsv2py.egg-info/SOURCES.txt
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        1 2024-05-31 07:02:01.000000 tsv2py-0.6.3/tsv2py.egg-info/dependency_links.txt
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        4 2024-05-31 07:02:01.000000 tsv2py-0.6.3/tsv2py.egg-info/top_level.txt
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        1 2024-05-31 07:00:00.000000 tsv2py-0.6.3/tsv2py.egg-info/zip-safe
```

### Comparing `tsv2py-0.6.2/LICENSE` & `tsv2py-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tsv2py-0.6.2/PKG-INFO` & `tsv2py-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsv2py
-Version: 0.6.2
+Version: 0.6.3
 Summary: High-performance parser and generator for PostgreSQL-compatible tab-separated values (TSV)
 Home-page: https://github.com/hunyadi/tsv2py
 Author: Levente Hunyadi
 Author-email: hunyadi@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `tsv2py-0.6.2/README.md` & `tsv2py-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `tsv2py-0.6.2/lib/tsv_parser.c` & `tsv2py-0.6.3/lib/tsv_parser.c`

 * *Files identical despite different names*

### Comparing `tsv2py-0.6.2/setup.cfg` & `tsv2py-0.6.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `tsv2py-0.6.2/setup.py` & `tsv2py-0.6.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,20 +21,24 @@
 
 
 if sys.platform.startswith("win"):
     compile_args = []
 else:
     compile_args = ["-fvisibility=hidden"]
 
+avx2_enabled = False
 if os.getenv("TSV_AVX2", "1") == "1":
-    print("compiling with AVX2")
     if sys.platform.startswith("win"):
+        avx2_enabled = True
         compile_args.append("/arch:AVX2")
-    else:
+    elif "x86_64" in os.uname().machine and "ARM" not in os.uname().version:
+        avx2_enabled = True
         compile_args.append("-mavx2")
+if avx2_enabled:
+    print("compiling with AVX2")
 else:
     print("compiling without AVX2")
 
 define_macros: List[Tuple[str, Optional[str]]] = []
 if sys.platform.startswith("win"):
     define_macros.append(("_WIN32_WINNT", "0x0603"))
 if os.getenv("TSV_LIMITED_API", "1") == "1":
```

### Comparing `tsv2py-0.6.2/tests/test_fuzz.py` & `tsv2py-0.6.3/tests/test_fuzz.py`

 * *Files identical despite different names*

### Comparing `tsv2py-0.6.2/tests/test_perf.py` & `tsv2py-0.6.3/tests/test_perf.py`

 * *Files identical despite different names*

### Comparing `tsv2py-0.6.2/tests/test_tsv.py` & `tsv2py-0.6.3/tests/test_tsv.py`

 * *Files identical despite different names*

### Comparing `tsv2py-0.6.2/tsv/helper.py` & `tsv2py-0.6.3/tsv/helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import enum
 import ipaddress
 import json
 import sys
 import types
 import typing
 import uuid
-from typing import Any, BinaryIO, Dict, Iterable, List, Tuple, Union
+from typing import Any, BinaryIO, Dict, Iterable, List, Set, Tuple, Union
 
 from . import parser
 
 
 def escape(s: bytes) -> bytes:
     "Replaces special characters in a string with their escape sequences."
 
@@ -80,15 +80,15 @@
         return "."
     elif typ is uuid.UUID:
         return "u"
     elif typ is ipaddress.IPv4Address:
         return "4"
     elif typ is ipaddress.IPv6Address:
         return "6"
-    elif typ is list or typ is dict:  # serialized JSON
+    elif typ is list or typ is set or typ is dict:  # serialized JSON
         return "j"
     elif typ is type(None):
         return "_"
 
     if is_union_like(typ):
         args = typing.get_args(typ)
         if (
```

### Comparing `tsv2py-0.6.2/tsv/parser.pyi` & `tsv2py-0.6.3/tsv/parser.pyi`

 * *Files identical despite different names*

### Comparing `tsv2py-0.6.2/tsv2py.egg-info/PKG-INFO` & `tsv2py-0.6.3/tsv2py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsv2py
-Version: 0.6.2
+Version: 0.6.3
 Summary: High-performance parser and generator for PostgreSQL-compatible tab-separated values (TSV)
 Home-page: https://github.com/hunyadi/tsv2py
 Author: Levente Hunyadi
 Author-email: hunyadi@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

