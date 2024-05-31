# Comparing `tmp/transmission_rpc-7.0.7a1.tar.gz` & `tmp/transmission_rpc-7.0.7a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transmission_rpc-7.0.7a1.tar", max compression
+gzip compressed data, was "transmission_rpc-7.0.7a2.tar", max compression
```

## Comparing `transmission_rpc-7.0.7a1.tar` & `transmission_rpc-7.0.7a2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1127 2024-05-30 17:46:00.296672 transmission_rpc-7.0.7a1/LICENSE
--rw-r--r--   0        0        0     2277 2024-05-30 17:46:00.296672 transmission_rpc-7.0.7a1/README.md
--rw-r--r--   0        0        0     3057 2024-05-30 17:46:00.300672 transmission_rpc-7.0.7a1/pyproject.toml
--rw-r--r--   0        0        0     2230 2024-05-30 17:46:00.300672 transmission_rpc-7.0.7a1/transmission_rpc/__init__.py
--rw-r--r--   0        0        0    45352 2024-05-30 17:46:00.300672 transmission_rpc-7.0.7a1/transmission_rpc/client.py
--rw-r--r--   0        0        0    10080 2024-05-30 17:46:00.300672 transmission_rpc-7.0.7a1/transmission_rpc/constants.py
--rw-r--r--   0        0        0     1673 2024-05-30 17:46:00.300672 transmission_rpc-7.0.7a1/transmission_rpc/error.py
--rw-r--r--   0        0        0        0 2024-05-30 17:46:00.300672 transmission_rpc-7.0.7a1/transmission_rpc/py.typed
--rw-r--r--   0        0        0    12488 2024-05-30 17:46:00.300672 transmission_rpc-7.0.7a1/transmission_rpc/session.py
--rw-r--r--   0        0        0    23901 2024-05-30 17:46:00.300672 transmission_rpc-7.0.7a1/transmission_rpc/torrent.py
--rw-r--r--   0        0        0     1900 2024-05-30 17:46:00.300672 transmission_rpc-7.0.7a1/transmission_rpc/types.py
--rw-r--r--   0        0        0     2643 2024-05-30 17:46:00.300672 transmission_rpc-7.0.7a1/transmission_rpc/utils.py
--rw-r--r--   0        0        0     3424 1970-01-01 00:00:00.000000 transmission_rpc-7.0.7a1/PKG-INFO
+-rw-r--r--   0        0        0     1127 2024-05-30 20:25:43.107619 transmission_rpc-7.0.7a2/LICENSE
+-rw-r--r--   0        0        0     2277 2024-05-30 20:25:43.107619 transmission_rpc-7.0.7a2/README.md
+-rw-r--r--   0        0        0     3057 2024-05-30 20:25:43.107619 transmission_rpc-7.0.7a2/pyproject.toml
+-rw-r--r--   0        0        0     2230 2024-05-30 20:25:43.107619 transmission_rpc-7.0.7a2/transmission_rpc/__init__.py
+-rw-r--r--   0        0        0    45352 2024-05-30 20:25:43.107619 transmission_rpc-7.0.7a2/transmission_rpc/client.py
+-rw-r--r--   0        0        0    10080 2024-05-30 20:25:43.107619 transmission_rpc-7.0.7a2/transmission_rpc/constants.py
+-rw-r--r--   0        0        0     1673 2024-05-30 20:25:43.107619 transmission_rpc-7.0.7a2/transmission_rpc/error.py
+-rw-r--r--   0        0        0        0 2024-05-30 20:25:43.107619 transmission_rpc-7.0.7a2/transmission_rpc/py.typed
+-rw-r--r--   0        0        0    12488 2024-05-30 20:25:43.107619 transmission_rpc-7.0.7a2/transmission_rpc/session.py
+-rw-r--r--   0        0        0    24178 2024-05-30 20:25:43.107619 transmission_rpc-7.0.7a2/transmission_rpc/torrent.py
+-rw-r--r--   0        0        0     1900 2024-05-30 20:25:43.107619 transmission_rpc-7.0.7a2/transmission_rpc/types.py
+-rw-r--r--   0        0        0     2643 2024-05-30 20:25:43.107619 transmission_rpc-7.0.7a2/transmission_rpc/utils.py
+-rw-r--r--   0        0        0     3424 1970-01-01 00:00:00.000000 transmission_rpc-7.0.7a2/PKG-INFO
```

### Comparing `transmission_rpc-7.0.7a1/LICENSE` & `transmission_rpc-7.0.7a2/LICENSE`

 * *Files identical despite different names*

### Comparing `transmission_rpc-7.0.7a1/README.md` & `transmission_rpc-7.0.7a2/README.md`

 * *Files identical despite different names*

### Comparing `transmission_rpc-7.0.7a1/pyproject.toml` & `transmission_rpc-7.0.7a2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "transmission-rpc"
-version = "7.0.7a1"
+version = "7.0.7a2"
 description = "Python module that implements the Transmission bittorent client JSON-RPC protocol"
 authors = ["Trim21 <i@trim21.me>"]
 readme = 'README.md'
 repository = 'https://github.com/Trim21/transmission-rpc'
 license = 'MIT'
 packages = [{ include = 'transmission_rpc' }]
 keywords = ['transmission', 'rpc']
```

### Comparing `transmission_rpc-7.0.7a1/transmission_rpc/__init__.py` & `transmission_rpc-7.0.7a2/transmission_rpc/__init__.py`

 * *Files identical despite different names*

### Comparing `transmission_rpc-7.0.7a1/transmission_rpc/client.py` & `transmission_rpc-7.0.7a2/transmission_rpc/client.py`

 * *Files identical despite different names*

### Comparing `transmission_rpc-7.0.7a1/transmission_rpc/constants.py` & `transmission_rpc-7.0.7a2/transmission_rpc/constants.py`

 * *Files identical despite different names*

### Comparing `transmission_rpc-7.0.7a1/transmission_rpc/error.py` & `transmission_rpc-7.0.7a2/transmission_rpc/error.py`

 * *Files identical despite different names*

### Comparing `transmission_rpc-7.0.7a1/transmission_rpc/session.py` & `transmission_rpc-7.0.7a2/transmission_rpc/session.py`

 * *Files identical despite different names*

### Comparing `transmission_rpc-7.0.7a1/transmission_rpc/torrent.py` & `transmission_rpc-7.0.7a2/transmission_rpc/torrent.py`

 * *Files 1% similar despite different names*

```diff
@@ -266,14 +266,24 @@
 
     @property
     def hashString(self) -> str:
         """Torrent info hash string, can also be used as Torrent ID"""
         return self.fields["hashString"]
 
     @property
+    def hash_string(self) -> str:
+        """Torrent info hash string, can also be used as Torrent ID"""
+        return self.fields["hashString"]
+
+    @property
+    def into_hash(self) -> str:
+        """alias of ``hashString``"""
+        return self.hashString
+
+    @property
     def available(self) -> float:
         """Availability in percent"""
         bytes_all = self.total_size
         bytes_done = sum(x["bytesCompleted"] for x in self.fields["fileStats"])
         bytes_avail = self.desired_available + bytes_done
         return (bytes_avail / bytes_all) * 100 if bytes_all else 0
```

### Comparing `transmission_rpc-7.0.7a1/transmission_rpc/types.py` & `transmission_rpc-7.0.7a2/transmission_rpc/types.py`

 * *Files identical despite different names*

### Comparing `transmission_rpc-7.0.7a1/transmission_rpc/utils.py` & `transmission_rpc-7.0.7a2/transmission_rpc/utils.py`

 * *Files identical despite different names*

### Comparing `transmission_rpc-7.0.7a1/PKG-INFO` & `transmission_rpc-7.0.7a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transmission-rpc
-Version: 7.0.7a1
+Version: 7.0.7a2
 Summary: Python module that implements the Transmission bittorent client JSON-RPC protocol
 Home-page: https://github.com/Trim21/transmission-rpc
 License: MIT
 Keywords: transmission,rpc
 Author: Trim21
 Author-email: i@trim21.me
 Requires-Python: >=3.8,<4.0
```

