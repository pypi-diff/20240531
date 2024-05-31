# Comparing `tmp/signalstickers_client_fork_laggykiller-3.3.post1.tar.gz` & `tmp/signalstickers_client_fork_laggykiller-3.3.0.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "signalstickers_client_fork_laggykiller-3.3.post1.tar", last modified: Fri Apr 12 16:39:00 2024, max compression
+gzip compressed data, was "signalstickers_client_fork_laggykiller-3.3.0.post2.tar", last modified: Fri May 31 13:01:55 2024, max compression
```

## Comparing `signalstickers_client_fork_laggykiller-3.3.post1.tar` & `signalstickers_client_fork_laggykiller-3.3.0.post2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 mcchau    (1000) mcchau    (1000)        0 2024-04-12 16:39:00.053974 signalstickers_client_fork_laggykiller-3.3.post1/
--rw-r--r--   0 mcchau    (1000) mcchau    (1000)     7652 2024-03-21 02:46:17.000000 signalstickers_client_fork_laggykiller-3.3.post1/LICENSE
--rw-r--r--   0 mcchau    (1000) mcchau    (1000)     3549 2024-04-12 16:39:00.053974 signalstickers_client_fork_laggykiller-3.3.post1/PKG-INFO
--rw-r--r--   0 mcchau    (1000) mcchau    (1000)     2843 2024-04-12 14:52:09.000000 signalstickers_client_fork_laggykiller-3.3.post1/README.md
--rw-r--r--   0 mcchau    (1000) mcchau    (1000)       38 2024-04-12 16:39:00.053974 signalstickers_client_fork_laggykiller-3.3.post1/setup.cfg
--rw-r--r--   0 mcchau    (1000) mcchau    (1000)     1056 2024-04-12 16:35:19.000000 signalstickers_client_fork_laggykiller-3.3.post1/setup.py
-drwxr-xr-x   0 mcchau    (1000) mcchau    (1000)        0 2024-04-12 16:39:00.050641 signalstickers_client_fork_laggykiller-3.3.post1/src/
-drwxr-xr-x   0 mcchau    (1000) mcchau    (1000)        0 2024-04-12 16:39:00.050641 signalstickers_client_fork_laggykiller-3.3.post1/src/signalstickers_client/
--rw-r--r--   0 mcchau    (1000) mcchau    (1000)       81 2024-03-21 04:09:16.000000 signalstickers_client_fork_laggykiller-3.3.post1/src/signalstickers_client/__init__.py
-drwxr-xr-x   0 mcchau    (1000) mcchau    (1000)        0 2024-04-12 16:39:00.050641 signalstickers_client_fork_laggykiller-3.3.post1/src/signalstickers_client/classes/
--rw-r--r--   0 mcchau    (1000) mcchau    (1000)     1293 2024-03-21 04:13:49.000000 signalstickers_client_fork_laggykiller-3.3.post1/src/signalstickers_client/classes/Stickers_pb2.py
--rw-r--r--   0 mcchau    (1000) mcchau    (1000)      442 2024-03-21 04:09:16.000000 signalstickers_client_fork_laggykiller-3.3.post1/src/signalstickers_client/classes/Stickers_pb2.pyi
--rw-r--r--   0 mcchau    (1000) mcchau    (1000)        0 2024-03-21 02:46:17.000000 signalstickers_client_fork_laggykiller-3.3.post1/src/signalstickers_client/classes/__init__.py
--rw-r--r--   0 mcchau    (1000) mcchau    (1000)     3204 2024-03-21 04:12:24.000000 signalstickers_client_fork_laggykiller-3.3.post1/src/signalstickers_client/classes/downloader.py
--rw-r--r--   0 mcchau    (1000) mcchau    (1000)     2515 2024-03-21 04:09:16.000000 signalstickers_client_fork_laggykiller-3.3.post1/src/signalstickers_client/classes/signalcrypto.py
--rw-r--r--   0 mcchau    (1000) mcchau    (1000)     3762 2024-03-21 04:12:24.000000 signalstickers_client_fork_laggykiller-3.3.post1/src/signalstickers_client/classes/uploader.py
--rw-r--r--   0 mcchau    (1000) mcchau    (1000)      576 2024-03-21 04:12:24.000000 signalstickers_client_fork_laggykiller-3.3.post1/src/signalstickers_client/errors.py
-drwxr-xr-x   0 mcchau    (1000) mcchau    (1000)        0 2024-04-12 16:39:00.053974 signalstickers_client_fork_laggykiller-3.3.post1/src/signalstickers_client/models/
--rw-r--r--   0 mcchau    (1000) mcchau    (1000)      175 2024-03-21 04:12:24.000000 signalstickers_client_fork_laggykiller-3.3.post1/src/signalstickers_client/models/__init__.py
--rw-r--r--   0 mcchau    (1000) mcchau    (1000)     1819 2024-03-21 04:09:16.000000 signalstickers_client_fork_laggykiller-3.3.post1/src/signalstickers_client/models/local_sticker_pack.py
--rw-r--r--   0 mcchau    (1000) mcchau    (1000)      283 2024-03-21 04:09:16.000000 signalstickers_client_fork_laggykiller-3.3.post1/src/signalstickers_client/models/sticker.py
--rw-r--r--   0 mcchau    (1000) mcchau    (1000)      832 2024-03-21 04:09:16.000000 signalstickers_client_fork_laggykiller-3.3.post1/src/signalstickers_client/models/sticker_pack.py
--rw-r--r--   0 mcchau    (1000) mcchau    (1000)        0 2024-04-12 16:19:25.000000 signalstickers_client_fork_laggykiller-3.3.post1/src/signalstickers_client/py.typed
--rw-r--r--   0 mcchau    (1000) mcchau    (1000)     2964 2024-03-21 04:13:26.000000 signalstickers_client_fork_laggykiller-3.3.post1/src/signalstickers_client/stickersclient.py
--rw-r--r--   0 mcchau    (1000) mcchau    (1000)      348 2024-03-21 04:09:16.000000 signalstickers_client_fork_laggykiller-3.3.post1/src/signalstickers_client/urls.py
-drwxr-xr-x   0 mcchau    (1000) mcchau    (1000)        0 2024-04-12 16:39:00.053974 signalstickers_client_fork_laggykiller-3.3.post1/src/signalstickers_client/utils/
--rw-r--r--   0 mcchau    (1000) mcchau    (1000)        0 2024-03-21 02:46:17.000000 signalstickers_client_fork_laggykiller-3.3.post1/src/signalstickers_client/utils/__init__.py
-drwxr-xr-x   0 mcchau    (1000) mcchau    (1000)        0 2024-04-12 16:39:00.053974 signalstickers_client_fork_laggykiller-3.3.post1/src/signalstickers_client/utils/ca/
--rw-r--r--   0 mcchau    (1000) mcchau    (1000)       44 2024-03-21 04:09:16.000000 signalstickers_client_fork_laggykiller-3.3.post1/src/signalstickers_client/utils/ca/__init__.py
--rw-r--r--   0 mcchau    (1000) mcchau    (1000)      137 2024-03-21 02:46:17.000000 signalstickers_client_fork_laggykiller-3.3.post1/src/signalstickers_client/utils/ca/ca.py
--rw-r--r--   0 mcchau    (1000) mcchau    (1000)     2090 2024-03-21 02:46:17.000000 signalstickers_client_fork_laggykiller-3.3.post1/src/signalstickers_client/utils/ca/cacert.pem
-drwxr-xr-x   0 mcchau    (1000) mcchau    (1000)        0 2024-04-12 16:39:00.053974 signalstickers_client_fork_laggykiller-3.3.post1/src/signalstickers_client_fork_laggykiller.egg-info/
--rw-r--r--   0 mcchau    (1000) mcchau    (1000)     3549 2024-04-12 16:39:00.000000 signalstickers_client_fork_laggykiller-3.3.post1/src/signalstickers_client_fork_laggykiller.egg-info/PKG-INFO
--rw-r--r--   0 mcchau    (1000) mcchau    (1000)     1227 2024-04-12 16:39:00.000000 signalstickers_client_fork_laggykiller-3.3.post1/src/signalstickers_client_fork_laggykiller.egg-info/SOURCES.txt
--rw-r--r--   0 mcchau    (1000) mcchau    (1000)        1 2024-04-12 16:39:00.000000 signalstickers_client_fork_laggykiller-3.3.post1/src/signalstickers_client_fork_laggykiller.egg-info/dependency_links.txt
--rw-r--r--   0 mcchau    (1000) mcchau    (1000)       64 2024-04-12 16:39:00.000000 signalstickers_client_fork_laggykiller-3.3.post1/src/signalstickers_client_fork_laggykiller.egg-info/requires.txt
--rw-r--r--   0 mcchau    (1000) mcchau    (1000)       22 2024-04-12 16:39:00.000000 signalstickers_client_fork_laggykiller-3.3.post1/src/signalstickers_client_fork_laggykiller.egg-info/top_level.txt
-drwxr-xr-x   0 mcchau    (1000) mcchau    (1000)        0 2024-04-12 16:39:00.053974 signalstickers_client_fork_laggykiller-3.3.post1/tests/
--rw-r--r--   0 mcchau    (1000) mcchau    (1000)     2185 2024-03-21 04:09:16.000000 signalstickers_client_fork_laggykiller-3.3.post1/tests/test_download.py
+drwxr-xr-x   0 mcchau    (1000) mcchau    (1000)        0 2024-05-31 13:01:55.330630 signalstickers_client_fork_laggykiller-3.3.0.post2/
+-rw-r--r--   0 mcchau    (1000) mcchau    (1000)     7652 2024-03-21 02:46:17.000000 signalstickers_client_fork_laggykiller-3.3.0.post2/LICENSE
+-rw-r--r--   0 mcchau    (1000) mcchau    (1000)     3549 2024-05-31 13:01:55.330630 signalstickers_client_fork_laggykiller-3.3.0.post2/PKG-INFO
+-rw-r--r--   0 mcchau    (1000) mcchau    (1000)     2843 2024-04-12 14:52:09.000000 signalstickers_client_fork_laggykiller-3.3.0.post2/README.md
+-rw-r--r--   0 mcchau    (1000) mcchau    (1000)       38 2024-05-31 13:01:55.330630 signalstickers_client_fork_laggykiller-3.3.0.post2/setup.cfg
+-rw-r--r--   0 mcchau    (1000) mcchau    (1000)     1056 2024-05-31 13:01:07.000000 signalstickers_client_fork_laggykiller-3.3.0.post2/setup.py
+drwxr-xr-x   0 mcchau    (1000) mcchau    (1000)        0 2024-05-31 13:01:55.327297 signalstickers_client_fork_laggykiller-3.3.0.post2/src/
+drwxr-xr-x   0 mcchau    (1000) mcchau    (1000)        0 2024-05-31 13:01:55.327297 signalstickers_client_fork_laggykiller-3.3.0.post2/src/signalstickers_client/
+-rw-r--r--   0 mcchau    (1000) mcchau    (1000)       81 2024-03-21 04:09:16.000000 signalstickers_client_fork_laggykiller-3.3.0.post2/src/signalstickers_client/__init__.py
+drwxr-xr-x   0 mcchau    (1000) mcchau    (1000)        0 2024-05-31 13:01:55.330630 signalstickers_client_fork_laggykiller-3.3.0.post2/src/signalstickers_client/classes/
+-rw-r--r--   0 mcchau    (1000) mcchau    (1000)     1293 2024-03-21 04:13:49.000000 signalstickers_client_fork_laggykiller-3.3.0.post2/src/signalstickers_client/classes/Stickers_pb2.py
+-rw-r--r--   0 mcchau    (1000) mcchau    (1000)      442 2024-03-21 04:09:16.000000 signalstickers_client_fork_laggykiller-3.3.0.post2/src/signalstickers_client/classes/Stickers_pb2.pyi
+-rw-r--r--   0 mcchau    (1000) mcchau    (1000)        0 2024-03-21 02:46:17.000000 signalstickers_client_fork_laggykiller-3.3.0.post2/src/signalstickers_client/classes/__init__.py
+-rw-r--r--   0 mcchau    (1000) mcchau    (1000)     3204 2024-03-21 04:12:24.000000 signalstickers_client_fork_laggykiller-3.3.0.post2/src/signalstickers_client/classes/downloader.py
+-rw-r--r--   0 mcchau    (1000) mcchau    (1000)     2515 2024-03-21 04:09:16.000000 signalstickers_client_fork_laggykiller-3.3.0.post2/src/signalstickers_client/classes/signalcrypto.py
+-rw-r--r--   0 mcchau    (1000) mcchau    (1000)     3762 2024-03-21 04:12:24.000000 signalstickers_client_fork_laggykiller-3.3.0.post2/src/signalstickers_client/classes/uploader.py
+-rw-r--r--   0 mcchau    (1000) mcchau    (1000)      576 2024-03-21 04:12:24.000000 signalstickers_client_fork_laggykiller-3.3.0.post2/src/signalstickers_client/errors.py
+drwxr-xr-x   0 mcchau    (1000) mcchau    (1000)        0 2024-05-31 13:01:55.330630 signalstickers_client_fork_laggykiller-3.3.0.post2/src/signalstickers_client/models/
+-rw-r--r--   0 mcchau    (1000) mcchau    (1000)      175 2024-03-21 04:12:24.000000 signalstickers_client_fork_laggykiller-3.3.0.post2/src/signalstickers_client/models/__init__.py
+-rw-r--r--   0 mcchau    (1000) mcchau    (1000)     1819 2024-03-21 04:09:16.000000 signalstickers_client_fork_laggykiller-3.3.0.post2/src/signalstickers_client/models/local_sticker_pack.py
+-rw-r--r--   0 mcchau    (1000) mcchau    (1000)      283 2024-03-21 04:09:16.000000 signalstickers_client_fork_laggykiller-3.3.0.post2/src/signalstickers_client/models/sticker.py
+-rw-r--r--   0 mcchau    (1000) mcchau    (1000)      832 2024-03-21 04:09:16.000000 signalstickers_client_fork_laggykiller-3.3.0.post2/src/signalstickers_client/models/sticker_pack.py
+-rw-r--r--   0 mcchau    (1000) mcchau    (1000)        0 2024-04-12 16:19:25.000000 signalstickers_client_fork_laggykiller-3.3.0.post2/src/signalstickers_client/py.typed
+-rw-r--r--   0 mcchau    (1000) mcchau    (1000)     2986 2024-05-31 12:55:27.000000 signalstickers_client_fork_laggykiller-3.3.0.post2/src/signalstickers_client/stickersclient.py
+-rw-r--r--   0 mcchau    (1000) mcchau    (1000)      348 2024-03-21 04:09:16.000000 signalstickers_client_fork_laggykiller-3.3.0.post2/src/signalstickers_client/urls.py
+drwxr-xr-x   0 mcchau    (1000) mcchau    (1000)        0 2024-05-31 13:01:55.330630 signalstickers_client_fork_laggykiller-3.3.0.post2/src/signalstickers_client/utils/
+-rw-r--r--   0 mcchau    (1000) mcchau    (1000)        0 2024-03-21 02:46:17.000000 signalstickers_client_fork_laggykiller-3.3.0.post2/src/signalstickers_client/utils/__init__.py
+drwxr-xr-x   0 mcchau    (1000) mcchau    (1000)        0 2024-05-31 13:01:55.330630 signalstickers_client_fork_laggykiller-3.3.0.post2/src/signalstickers_client/utils/ca/
+-rw-r--r--   0 mcchau    (1000) mcchau    (1000)       44 2024-03-21 04:09:16.000000 signalstickers_client_fork_laggykiller-3.3.0.post2/src/signalstickers_client/utils/ca/__init__.py
+-rw-r--r--   0 mcchau    (1000) mcchau    (1000)      137 2024-03-21 02:46:17.000000 signalstickers_client_fork_laggykiller-3.3.0.post2/src/signalstickers_client/utils/ca/ca.py
+-rw-r--r--   0 mcchau    (1000) mcchau    (1000)     2090 2024-03-21 02:46:17.000000 signalstickers_client_fork_laggykiller-3.3.0.post2/src/signalstickers_client/utils/ca/cacert.pem
+drwxr-xr-x   0 mcchau    (1000) mcchau    (1000)        0 2024-05-31 13:01:55.330630 signalstickers_client_fork_laggykiller-3.3.0.post2/src/signalstickers_client_fork_laggykiller.egg-info/
+-rw-r--r--   0 mcchau    (1000) mcchau    (1000)     3549 2024-05-31 13:01:55.000000 signalstickers_client_fork_laggykiller-3.3.0.post2/src/signalstickers_client_fork_laggykiller.egg-info/PKG-INFO
+-rw-r--r--   0 mcchau    (1000) mcchau    (1000)     1227 2024-05-31 13:01:55.000000 signalstickers_client_fork_laggykiller-3.3.0.post2/src/signalstickers_client_fork_laggykiller.egg-info/SOURCES.txt
+-rw-r--r--   0 mcchau    (1000) mcchau    (1000)        1 2024-05-31 13:01:55.000000 signalstickers_client_fork_laggykiller-3.3.0.post2/src/signalstickers_client_fork_laggykiller.egg-info/dependency_links.txt
+-rw-r--r--   0 mcchau    (1000) mcchau    (1000)       64 2024-05-31 13:01:55.000000 signalstickers_client_fork_laggykiller-3.3.0.post2/src/signalstickers_client_fork_laggykiller.egg-info/requires.txt
+-rw-r--r--   0 mcchau    (1000) mcchau    (1000)       22 2024-05-31 13:01:55.000000 signalstickers_client_fork_laggykiller-3.3.0.post2/src/signalstickers_client_fork_laggykiller.egg-info/top_level.txt
+drwxr-xr-x   0 mcchau    (1000) mcchau    (1000)        0 2024-05-31 13:01:55.330630 signalstickers_client_fork_laggykiller-3.3.0.post2/tests/
+-rw-r--r--   0 mcchau    (1000) mcchau    (1000)     2185 2024-03-21 04:09:16.000000 signalstickers_client_fork_laggykiller-3.3.0.post2/tests/test_download.py
```

### Comparing `signalstickers_client_fork_laggykiller-3.3.post1/LICENSE` & `signalstickers_client_fork_laggykiller-3.3.0.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `signalstickers_client_fork_laggykiller-3.3.post1/PKG-INFO` & `signalstickers_client_fork_laggykiller-3.3.0.post2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: signalstickers-client-fork-laggykiller
-Version: 3.3.0.post1
+Version: 3.3.0.post2
 Summary: A client for the Signal stickers API
 Home-page: https://github.com/laggykiller/signalstickers-client
 Author: Romain Ricard
 Author-email: contact+stickerclient@romainricard.fr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `signalstickers_client_fork_laggykiller-3.3.post1/README.md` & `signalstickers_client_fork_laggykiller-3.3.0.post2/README.md`

 * *Files identical despite different names*

### Comparing `signalstickers_client_fork_laggykiller-3.3.post1/setup.py` & `signalstickers_client_fork_laggykiller-3.3.0.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="signalstickers-client-fork-laggykiller",
-    version="3.3.0.post1",
+    version="3.3.0.post2",
     author="Romain Ricard",
     author_email="contact+stickerclient@romainricard.fr",
     description="A client for the Signal stickers API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/laggykiller/signalstickers-client",
     packages=setuptools.find_packages(where="src"),
```

### Comparing `signalstickers_client_fork_laggykiller-3.3.post1/src/signalstickers_client/classes/Stickers_pb2.py` & `signalstickers_client_fork_laggykiller-3.3.0.post2/src/signalstickers_client/classes/Stickers_pb2.py`

 * *Files identical despite different names*

### Comparing `signalstickers_client_fork_laggykiller-3.3.post1/src/signalstickers_client/classes/downloader.py` & `signalstickers_client_fork_laggykiller-3.3.0.post2/src/signalstickers_client/classes/downloader.py`

 * *Files identical despite different names*

### Comparing `signalstickers_client_fork_laggykiller-3.3.post1/src/signalstickers_client/classes/signalcrypto.py` & `signalstickers_client_fork_laggykiller-3.3.0.post2/src/signalstickers_client/classes/signalcrypto.py`

 * *Files identical despite different names*

### Comparing `signalstickers_client_fork_laggykiller-3.3.post1/src/signalstickers_client/classes/uploader.py` & `signalstickers_client_fork_laggykiller-3.3.0.post2/src/signalstickers_client/classes/uploader.py`

 * *Files identical despite different names*

### Comparing `signalstickers_client_fork_laggykiller-3.3.post1/src/signalstickers_client/errors.py` & `signalstickers_client_fork_laggykiller-3.3.0.post2/src/signalstickers_client/errors.py`

 * *Files identical despite different names*

### Comparing `signalstickers_client_fork_laggykiller-3.3.post1/src/signalstickers_client/models/local_sticker_pack.py` & `signalstickers_client_fork_laggykiller-3.3.0.post2/src/signalstickers_client/models/local_sticker_pack.py`

 * *Files identical despite different names*

### Comparing `signalstickers_client_fork_laggykiller-3.3.post1/src/signalstickers_client/models/sticker_pack.py` & `signalstickers_client_fork_laggykiller-3.3.0.post2/src/signalstickers_client/models/sticker_pack.py`

 * *Files identical despite different names*

### Comparing `signalstickers_client_fork_laggykiller-3.3.post1/src/signalstickers_client/stickersclient.py` & `signalstickers_client_fork_laggykiller-3.3.0.post2/src/signalstickers_client/stickersclient.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
     Author: Romain RICARD <contact+stickerclient@romainricard.fr>
     License: LGPLv3
 """
 
 import httpx
 from types import TracebackType
+from typing import Optional
 
 from signalstickers_client.classes import downloader, uploader
 from signalstickers_client.models import LocalStickerPack
 from signalstickers_client.utils.ca import CACERT_PATH
 
 
 class StickersClient:
@@ -42,17 +43,17 @@
 
     async def __aenter__(self) -> "StickersClient":
         self.http = await httpx.AsyncClient(verify=CACERT_PATH).__aenter__()
         return self
 
     async def __aexit__(
         self,
-        exc_type: type[BaseException] | None = None,
-        exc_value: BaseException | None = None,
-        traceback: TracebackType | None = None,
+        exc_type: Optional[type] = None,
+        exc_value: Optional[BaseException] = None,
+        traceback: Optional[TracebackType] = None,
     ) -> None:
         return await self.http.__aexit__(exc_type, exc_value, traceback)
 
     async def get_pack(self, pack_id: str, pack_key: str):
         """
         Return a `StickerPack` from its id and key
         """
```

### Comparing `signalstickers_client_fork_laggykiller-3.3.post1/src/signalstickers_client/utils/ca/cacert.pem` & `signalstickers_client_fork_laggykiller-3.3.0.post2/src/signalstickers_client/utils/ca/cacert.pem`

 * *Files identical despite different names*

### Comparing `signalstickers_client_fork_laggykiller-3.3.post1/src/signalstickers_client_fork_laggykiller.egg-info/PKG-INFO` & `signalstickers_client_fork_laggykiller-3.3.0.post2/src/signalstickers_client_fork_laggykiller.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: signalstickers-client-fork-laggykiller
-Version: 3.3.0.post1
+Version: 3.3.0.post2
 Summary: A client for the Signal stickers API
 Home-page: https://github.com/laggykiller/signalstickers-client
 Author: Romain Ricard
 Author-email: contact+stickerclient@romainricard.fr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `signalstickers_client_fork_laggykiller-3.3.post1/src/signalstickers_client_fork_laggykiller.egg-info/SOURCES.txt` & `signalstickers_client_fork_laggykiller-3.3.0.post2/src/signalstickers_client_fork_laggykiller.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `signalstickers_client_fork_laggykiller-3.3.post1/tests/test_download.py` & `signalstickers_client_fork_laggykiller-3.3.0.post2/tests/test_download.py`

 * *Files identical despite different names*

