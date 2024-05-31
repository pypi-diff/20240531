# Comparing `tmp/liblta-3.1.0.tar.gz` & `tmp/liblta-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liblta-3.1.0.tar", last modified: Thu May 30 20:20:21 2024, max compression
+gzip compressed data, was "liblta-3.1.1.tar", last modified: Fri May 31 16:46:48 2024, max compression
```

## Comparing `liblta-3.1.0.tar` & `liblta-3.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 20:20:21.017353 liblta-3.1.0/
--rw-rw-rw-   0 root         (0) root         (0)     1072 2024-05-30 20:20:14.000000 liblta-3.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2467 2024-05-30 20:20:21.017353 liblta-3.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1913 2024-05-30 20:20:14.000000 liblta-3.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 20:20:21.015353 liblta-3.1.0/liblta/
--rw-rw-rw-   0 root         (0) root         (0)      104 2024-05-30 20:20:14.000000 liblta-3.1.0/liblta/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2115 2024-05-30 20:20:14.000000 liblta-3.1.0/liblta/_auxiliary.py
--rw-rw-rw-   0 root         (0) root         (0)    15491 2024-05-30 20:20:14.000000 liblta-3.1.0/liblta/_ethernet.py
--rw-rw-rw-   0 root         (0) root         (0)    16030 2024-05-30 20:20:14.000000 liblta-3.1.0/liblta/_sseq_handler.py
--rw-rw-rw-   0 root         (0) root         (0)    10999 2024-05-30 20:20:14.000000 liblta-3.1.0/liblta/legacy_lta.py
--rw-rw-rw-   0 root         (0) root         (0)    10760 2024-05-30 20:20:14.000000 liblta-3.1.0/liblta/lta_decoder.py
--rw-rw-rw-   0 root         (0) root         (0)    33669 2024-05-30 20:20:14.000000 liblta-3.1.0/liblta/pylta.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 20:20:21.017353 liblta-3.1.0/liblta.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2467 2024-05-30 20:20:21.000000 liblta-3.1.0/liblta.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      324 2024-05-30 20:20:21.000000 liblta-3.1.0/liblta.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 20:20:21.000000 liblta-3.1.0/liblta.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       21 2024-05-30 20:20:21.000000 liblta-3.1.0/liblta.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-05-30 20:20:21.000000 liblta-3.1.0/liblta.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      626 2024-05-30 20:20:14.000000 liblta-3.1.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-30 20:20:21.017353 liblta-3.1.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 16:46:48.164310 liblta-3.1.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1072 2024-05-31 16:46:42.000000 liblta-3.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2467 2024-05-31 16:46:48.164310 liblta-3.1.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1913 2024-05-31 16:46:42.000000 liblta-3.1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 16:46:48.162310 liblta-3.1.1/liblta/
+-rw-rw-rw-   0 root         (0) root         (0)      104 2024-05-31 16:46:42.000000 liblta-3.1.1/liblta/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2115 2024-05-31 16:46:42.000000 liblta-3.1.1/liblta/_auxiliary.py
+-rw-rw-rw-   0 root         (0) root         (0)    15491 2024-05-31 16:46:42.000000 liblta-3.1.1/liblta/_ethernet.py
+-rw-rw-rw-   0 root         (0) root         (0)    16030 2024-05-31 16:46:42.000000 liblta-3.1.1/liblta/_sseq_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)    10999 2024-05-31 16:46:42.000000 liblta-3.1.1/liblta/legacy_lta.py
+-rw-rw-rw-   0 root         (0) root         (0)    10760 2024-05-31 16:46:42.000000 liblta-3.1.1/liblta/lta_decoder.py
+-rw-rw-rw-   0 root         (0) root         (0)    33667 2024-05-31 16:46:42.000000 liblta-3.1.1/liblta/pylta.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 16:46:48.164310 liblta-3.1.1/liblta.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2467 2024-05-31 16:46:48.000000 liblta-3.1.1/liblta.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      324 2024-05-31 16:46:48.000000 liblta-3.1.1/liblta.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-31 16:46:48.000000 liblta-3.1.1/liblta.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-31 16:46:48.000000 liblta-3.1.1/liblta.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-05-31 16:46:48.000000 liblta-3.1.1/liblta.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      626 2024-05-31 16:46:42.000000 liblta-3.1.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-31 16:46:48.165310 liblta-3.1.1/setup.cfg
```

### Comparing `liblta-3.1.0/LICENSE` & `liblta-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `liblta-3.1.0/PKG-INFO` & `liblta-3.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liblta
-Version: 3.1.0
+Version: 3.1.1
 Summary: A python API to send commands to the LTA (Low-Threshold Acquisition) board.
 Author-email: Nicolás Avalos <nicolaseavalos@gmail.com>
 Project-URL: Repository, https://gitlab.com/nicolaseavalos/liblta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.7
```

### Comparing `liblta-3.1.0/README.md` & `liblta-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `liblta-3.1.0/liblta/_auxiliary.py` & `liblta-3.1.1/liblta/_auxiliary.py`

 * *Files identical despite different names*

### Comparing `liblta-3.1.0/liblta/_ethernet.py` & `liblta-3.1.1/liblta/_ethernet.py`

 * *Files identical despite different names*

### Comparing `liblta-3.1.0/liblta/_sseq_handler.py` & `liblta-3.1.1/liblta/_sseq_handler.py`

 * *Files identical despite different names*

### Comparing `liblta-3.1.0/liblta/legacy_lta.py` & `liblta-3.1.1/liblta/legacy_lta.py`

 * *Files identical despite different names*

### Comparing `liblta-3.1.0/liblta/lta_decoder.py` & `liblta-3.1.1/liblta/lta_decoder.py`

 * *Files identical despite different names*

### Comparing `liblta-3.1.0/liblta/pylta.py` & `liblta-3.1.1/liblta/pylta.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,15 +124,15 @@
 
 
     def disconnect(self):
         '''Close the connection to the LTA. If not connected, nothing will
         happen.
         '''
 
-        if not self._connected(): return
+        if not self._connected: return
 
         self._eth._stop_idle_thread()
         self._control_socket.close()
         self._data_socket.close()
 
         self._connected = False
```

### Comparing `liblta-3.1.0/liblta.egg-info/PKG-INFO` & `liblta-3.1.1/liblta.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liblta
-Version: 3.1.0
+Version: 3.1.1
 Summary: A python API to send commands to the LTA (Low-Threshold Acquisition) board.
 Author-email: Nicolás Avalos <nicolaseavalos@gmail.com>
 Project-URL: Repository, https://gitlab.com/nicolaseavalos/liblta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.7
```

### Comparing `liblta-3.1.0/pyproject.toml` & `liblta-3.1.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "liblta"
-version = "3.1.0"
+version = "3.1.1"
 authors = [
     {name = "Nicolás Avalos", email = "nicolaseavalos@gmail.com"},
 ]
 description = "A python API to send commands to the LTA (Low-Threshold Acquisition) board."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

