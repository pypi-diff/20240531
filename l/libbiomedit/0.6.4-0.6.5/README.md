# Comparing `tmp/libbiomedit-0.6.4.tar.gz` & `tmp/libbiomedit-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libbiomedit-0.6.4.tar", last modified: Wed May 29 07:08:11 2024, max compression
+gzip compressed data, was "libbiomedit-0.6.5.tar", last modified: Fri May 31 14:08:18 2024, max compression
```

## Comparing `libbiomedit-0.6.4.tar` & `libbiomedit-0.6.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 07:08:11.696083 libbiomedit-0.6.4/
--rw-rw-rw-   0 root         (0) root         (0)     7652 2024-05-29 07:07:58.000000 libbiomedit-0.6.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2093 2024-05-29 07:08:11.696083 libbiomedit-0.6.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      770 2024-05-29 07:07:58.000000 libbiomedit-0.6.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 07:08:11.691083 libbiomedit-0.6.4/libbiomedit/
--rw-rw-rw-   0 root         (0) root         (0)      236 2024-05-29 07:07:58.000000 libbiomedit-0.6.4/libbiomedit/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2916 2024-05-29 07:07:58.000000 libbiomedit-0.6.4/libbiomedit/archive.py
--rw-rw-rw-   0 root         (0) root         (0)    13317 2024-05-29 07:07:58.000000 libbiomedit-0.6.4/libbiomedit/crypt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 07:08:11.693083 libbiomedit-0.6.4/libbiomedit/lib/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-29 07:07:59.000000 libbiomedit-0.6.4/libbiomedit/lib/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2536 2024-05-29 07:07:58.000000 libbiomedit-0.6.4/libbiomedit/lib/classify.py
--rw-rw-rw-   0 root         (0) root         (0)    11817 2024-05-29 07:07:58.000000 libbiomedit-0.6.4/libbiomedit/lib/deserialize.py
--rw-rw-rw-   0 root         (0) root         (0)      638 2024-05-29 07:07:58.000000 libbiomedit-0.6.4/libbiomedit/lib/secret.py
--rw-rw-rw-   0 root         (0) root         (0)     3982 2024-05-29 07:07:58.000000 libbiomedit-0.6.4/libbiomedit/metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    10401 2024-05-29 07:07:58.000000 libbiomedit-0.6.4/libbiomedit/portal.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-29 07:07:59.000000 libbiomedit-0.6.4/libbiomedit/py.typed
--rw-rw-rw-   0 root         (0) root         (0)       22 2024-05-29 07:07:58.000000 libbiomedit-0.6.4/libbiomedit/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 07:08:11.694083 libbiomedit-0.6.4/libbiomedit.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2093 2024-05-29 07:08:11.000000 libbiomedit-0.6.4/libbiomedit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      650 2024-05-29 07:08:11.000000 libbiomedit-0.6.4/libbiomedit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 07:08:11.000000 libbiomedit-0.6.4/libbiomedit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 07:08:10.000000 libbiomedit-0.6.4/libbiomedit.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       96 2024-05-29 07:08:11.000000 libbiomedit-0.6.4/libbiomedit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-05-29 07:08:11.000000 libbiomedit-0.6.4/libbiomedit.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      864 2024-05-29 07:07:58.000000 libbiomedit-0.6.4/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1326 2024-05-29 07:08:11.696083 libbiomedit-0.6.4/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 07:08:11.694083 libbiomedit-0.6.4/test/
--rw-rw-rw-   0 root         (0) root         (0)     3311 2024-05-29 07:07:58.000000 libbiomedit-0.6.4/test/test_archive.py
--rw-rw-rw-   0 root         (0) root         (0)      669 2024-05-29 07:07:58.000000 libbiomedit-0.6.4/test/test_classify.py
--rw-rw-rw-   0 root         (0) root         (0)    22832 2024-05-29 07:07:58.000000 libbiomedit-0.6.4/test/test_crypt.py
--rw-rw-rw-   0 root         (0) root         (0)     6790 2024-05-29 07:07:58.000000 libbiomedit-0.6.4/test/test_deserialize.py
--rw-rw-rw-   0 root         (0) root         (0)     5239 2024-05-29 07:07:58.000000 libbiomedit-0.6.4/test/test_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    13310 2024-05-29 07:07:58.000000 libbiomedit-0.6.4/test/test_portal.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 14:08:18.159185 libbiomedit-0.6.5/
+-rw-rw-rw-   0 root         (0) root         (0)     7652 2024-05-31 14:08:04.000000 libbiomedit-0.6.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2093 2024-05-31 14:08:18.159185 libbiomedit-0.6.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      770 2024-05-31 14:08:04.000000 libbiomedit-0.6.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 14:08:18.154185 libbiomedit-0.6.5/libbiomedit/
+-rw-rw-rw-   0 root         (0) root         (0)      236 2024-05-31 14:08:04.000000 libbiomedit-0.6.5/libbiomedit/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2916 2024-05-31 14:08:04.000000 libbiomedit-0.6.5/libbiomedit/archive.py
+-rw-rw-rw-   0 root         (0) root         (0)    13317 2024-05-31 14:08:04.000000 libbiomedit-0.6.5/libbiomedit/crypt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 14:08:18.156185 libbiomedit-0.6.5/libbiomedit/lib/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-31 14:08:05.000000 libbiomedit-0.6.5/libbiomedit/lib/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2536 2024-05-31 14:08:04.000000 libbiomedit-0.6.5/libbiomedit/lib/classify.py
+-rw-rw-rw-   0 root         (0) root         (0)    11817 2024-05-31 14:08:04.000000 libbiomedit-0.6.5/libbiomedit/lib/deserialize.py
+-rw-rw-rw-   0 root         (0) root         (0)      638 2024-05-31 14:08:04.000000 libbiomedit-0.6.5/libbiomedit/lib/secret.py
+-rw-rw-rw-   0 root         (0) root         (0)     4155 2024-05-31 14:08:04.000000 libbiomedit-0.6.5/libbiomedit/metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    10401 2024-05-31 14:08:04.000000 libbiomedit-0.6.5/libbiomedit/portal.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-31 14:08:05.000000 libbiomedit-0.6.5/libbiomedit/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)       22 2024-05-31 14:08:04.000000 libbiomedit-0.6.5/libbiomedit/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 14:08:18.157185 libbiomedit-0.6.5/libbiomedit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2093 2024-05-31 14:08:18.000000 libbiomedit-0.6.5/libbiomedit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      650 2024-05-31 14:08:18.000000 libbiomedit-0.6.5/libbiomedit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-31 14:08:18.000000 libbiomedit-0.6.5/libbiomedit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-31 14:08:17.000000 libbiomedit-0.6.5/libbiomedit.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       96 2024-05-31 14:08:18.000000 libbiomedit-0.6.5/libbiomedit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-05-31 14:08:18.000000 libbiomedit-0.6.5/libbiomedit.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      864 2024-05-31 14:08:04.000000 libbiomedit-0.6.5/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1326 2024-05-31 14:08:18.160185 libbiomedit-0.6.5/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 14:08:18.157185 libbiomedit-0.6.5/test/
+-rw-rw-rw-   0 root         (0) root         (0)     3311 2024-05-31 14:08:04.000000 libbiomedit-0.6.5/test/test_archive.py
+-rw-rw-rw-   0 root         (0) root         (0)      669 2024-05-31 14:08:04.000000 libbiomedit-0.6.5/test/test_classify.py
+-rw-rw-rw-   0 root         (0) root         (0)    22832 2024-05-31 14:08:04.000000 libbiomedit-0.6.5/test/test_crypt.py
+-rw-rw-rw-   0 root         (0) root         (0)     6790 2024-05-31 14:08:04.000000 libbiomedit-0.6.5/test/test_deserialize.py
+-rw-rw-rw-   0 root         (0) root         (0)     5242 2024-05-31 14:08:04.000000 libbiomedit-0.6.5/test/test_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    13310 2024-05-31 14:08:04.000000 libbiomedit-0.6.5/test/test_portal.py
```

### Comparing `libbiomedit-0.6.4/LICENSE` & `libbiomedit-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `libbiomedit-0.6.4/PKG-INFO` & `libbiomedit-0.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libbiomedit
-Version: 0.6.4
+Version: 0.6.5
 Summary: Shared library for arround biomedit data transfer
 Home-page: https://gitlab.com/biomedit/libbiomedit
 Author: Robin Engler, Jarosław Surkont, Riccardo Muri, Gerhard Bräunlich, Christian Ribeaud, François Martin
 Author-email: Robin.Engler@sib.swiss, riccardo.murri@id.ethz.ch, jaroslaw.surkont@unibas.ch, gerhard.braeunlich@id.ethz.ch, christian.ribeaud@karakun.com, francois.martin@karakun.com
 License: LGPL3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `libbiomedit-0.6.4/README.md` & `libbiomedit-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `libbiomedit-0.6.4/libbiomedit/archive.py` & `libbiomedit-0.6.5/libbiomedit/archive.py`

 * *Files identical despite different names*

### Comparing `libbiomedit-0.6.4/libbiomedit/crypt.py` & `libbiomedit-0.6.5/libbiomedit/crypt.py`

 * *Files identical despite different names*

### Comparing `libbiomedit-0.6.4/libbiomedit/lib/classify.py` & `libbiomedit-0.6.5/libbiomedit/lib/classify.py`

 * *Files identical despite different names*

### Comparing `libbiomedit-0.6.4/libbiomedit/lib/deserialize.py` & `libbiomedit-0.6.5/libbiomedit/lib/deserialize.py`

 * *Files identical despite different names*

### Comparing `libbiomedit-0.6.4/libbiomedit/lib/secret.py` & `libbiomedit-0.6.5/libbiomedit/lib/secret.py`

 * *Files identical despite different names*

### Comparing `libbiomedit-0.6.4/libbiomedit/metadata.py` & `libbiomedit-0.6.5/libbiomedit/metadata.py`

 * *Files 3% similar despite different names*

```diff
@@ -85,20 +85,24 @@
 
 DATE_FMT = "%Y-%m-%dT%H:%M:%S%z"
 
 
 # TODO: use `datetime.fromisoformat` when support for Python <= 3.10 is dropped
 def _datetime_from_isoformat(s: str) -> datetime:
     try:
-        # try to parse the date with the default format (without milliseconds)
+        # try to parse the date with the default format (without microseconds)
         return datetime.strptime(s, DATE_FMT)
     except ValueError:
-        # as a fallback, try using the default format extended with milliseconds
+        # as a fallback, try using the default format extended with microseconds
         # (note the `.%f` part)
-        return datetime.strptime(s, "%Y-%m-%dT%H:%M:%S.%f%z")
+        # Note: If the precision of the timestamp is greater than microseconds the
+        # extra digits are ignored.
+        return datetime.strptime(
+            re.sub(r"(\.\d{6})\d*", r"\1", s), "%Y-%m-%dT%H:%M:%S.%f%z"
+        )
 
 
 class Purpose(Enum):
     PRODUCTION = "PRODUCTION"
     TEST = "TEST"
```

### Comparing `libbiomedit-0.6.4/libbiomedit/portal.py` & `libbiomedit-0.6.5/libbiomedit/portal.py`

 * *Files identical despite different names*

### Comparing `libbiomedit-0.6.4/libbiomedit.egg-info/PKG-INFO` & `libbiomedit-0.6.5/libbiomedit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libbiomedit
-Version: 0.6.4
+Version: 0.6.5
 Summary: Shared library for arround biomedit data transfer
 Home-page: https://gitlab.com/biomedit/libbiomedit
 Author: Robin Engler, Jarosław Surkont, Riccardo Muri, Gerhard Bräunlich, Christian Ribeaud, François Martin
 Author-email: Robin.Engler@sib.swiss, riccardo.murri@id.ethz.ch, jaroslaw.surkont@unibas.ch, gerhard.braeunlich@id.ethz.ch, christian.ribeaud@karakun.com, francois.martin@karakun.com
 License: LGPL3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `libbiomedit-0.6.4/libbiomedit.egg-info/SOURCES.txt` & `libbiomedit-0.6.5/libbiomedit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libbiomedit-0.6.4/pyproject.toml` & `libbiomedit-0.6.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `libbiomedit-0.6.4/setup.cfg` & `libbiomedit-0.6.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `libbiomedit-0.6.4/test/test_archive.py` & `libbiomedit-0.6.5/test/test_archive.py`

 * *Files identical despite different names*

### Comparing `libbiomedit-0.6.4/test/test_classify.py` & `libbiomedit-0.6.5/test/test_classify.py`

 * *Files identical despite different names*

### Comparing `libbiomedit-0.6.4/test/test_crypt.py` & `libbiomedit-0.6.5/test/test_crypt.py`

 * *Files identical despite different names*

### Comparing `libbiomedit-0.6.4/test/test_deserialize.py` & `libbiomedit-0.6.5/test/test_deserialize.py`

 * *Files identical despite different names*

### Comparing `libbiomedit-0.6.4/test/test_metadata.py` & `libbiomedit-0.6.5/test/test_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
             "sender": "14948C167662768AD33C8D2C7DE1E0794C1C000B",
             "recipients": [
                 "14948C167662768AD33C8D2C7DE1E0794C1C000B",
                 "14948C167662768AD33C8D2C7DE1E0794C1C000A",
             ],
             "checksum": "d7c3094d6ba7d8f31a8950c83f61078ca2"
             "c1b3b7cad6c188e9257a52a1e27411",
-            "timestamp": "2024-04-22T12:34:31.172511Z",
+            "timestamp": "2024-04-22T12:34:31.208872700Z",
             "version": "0.7.1",
             "checksum_algorithm": "SHA256",
             "compression_algorithm": "zstandard",
             "transfer_id": None,
             "purpose": None,
         }
         sett_v5_metadata = MetaData(
@@ -68,15 +68,15 @@
             recipients=[
                 HexStr1024("14948C167662768AD33C8D2C7DE1E0794C1C000B"),
                 HexStr1024("14948C167662768AD33C8D2C7DE1E0794C1C000A"),
             ],
             checksum=HexStr256(
                 "d7c3094d6ba7d8f31a8950c83f61078ca2c1b3b7cad6c188e9257a52a1e27411"
             ),
-            timestamp=datetime(2024, 4, 22, 12, 34, 31, 172511, timezone.utc),
+            timestamp=datetime(2024, 4, 22, 12, 34, 31, 208872, timezone.utc),
             version="0.7.1",
             checksum_algorithm="SHA256",
             compression_algorithm="zstandard",
             transfer_id=None,
             purpose=None,
         )
         self.assertEqual(MetaData.from_dict(sett_v5_dict), sett_v5_metadata)
```

### Comparing `libbiomedit-0.6.4/test/test_portal.py` & `libbiomedit-0.6.5/test/test_portal.py`

 * *Files identical despite different names*

