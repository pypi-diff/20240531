# Comparing `tmp/cldfgeojson-0.2.0.tar.gz` & `tmp/cldfgeojson-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cldfgeojson-0.2.0.tar", last modified: Fri Apr 26 09:07:19 2024, max compression
+gzip compressed data, was "cldfgeojson-0.2.1.tar", last modified: Fri May 17 09:22:55 2024, max compression
```

## Comparing `cldfgeojson-0.2.0.tar` & `cldfgeojson-0.2.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2024-04-26 09:07:19.738656 cldfgeojson-0.2.0/
--rw-rw-r--   0 robert    (1000) robert    (1000)    11357 2024-04-25 05:54:39.000000 cldfgeojson-0.2.0/LICENSE
--rw-rw-r--   0 robert    (1000) robert    (1000)       50 2024-04-25 05:55:32.000000 cldfgeojson-0.2.0/MANIFEST.in
--rw-rw-r--   0 robert    (1000) robert    (1000)     1946 2024-04-26 09:07:19.738656 cldfgeojson-0.2.0/PKG-INFO
--rw-rw-r--   0 robert    (1000) robert    (1000)      723 2024-04-26 06:13:24.000000 cldfgeojson-0.2.0/README.md
--rw-rw-r--   0 robert    (1000) robert    (1000)       81 2024-04-25 05:55:40.000000 cldfgeojson-0.2.0/pyproject.toml
--rw-rw-r--   0 robert    (1000) robert    (1000)     1892 2024-04-26 09:07:19.738656 cldfgeojson-0.2.0/setup.cfg
--rwxrwxr-x   0 robert    (1000) robert    (1000)       39 2024-04-25 05:56:22.000000 cldfgeojson-0.2.0/setup.py
-drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2024-04-26 09:07:19.738656 cldfgeojson-0.2.0/src/
-drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2024-04-26 09:07:19.738656 cldfgeojson-0.2.0/src/cldfgeojson/
--rw-rw-r--   0 robert    (1000) robert    (1000)      106 2024-04-26 09:06:29.000000 cldfgeojson-0.2.0/src/cldfgeojson/__init__.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     6542 2024-04-26 08:46:30.000000 cldfgeojson-0.2.0/src/cldfgeojson/create.py
--rw-rw-r--   0 robert    (1000) robert    (1000)      928 2024-04-26 06:42:20.000000 cldfgeojson-0.2.0/src/cldfgeojson/geojson.py
-drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2024-04-26 09:07:19.738656 cldfgeojson-0.2.0/src/cldfgeojson.egg-info/
--rw-r--r--   0 robert    (1000) robert    (1000)     1946 2024-04-26 09:07:19.000000 cldfgeojson-0.2.0/src/cldfgeojson.egg-info/PKG-INFO
--rw-rw-r--   0 robert    (1000) robert    (1000)      397 2024-04-26 09:07:19.000000 cldfgeojson-0.2.0/src/cldfgeojson.egg-info/SOURCES.txt
--rw-rw-r--   0 robert    (1000) robert    (1000)        1 2024-04-26 09:07:19.000000 cldfgeojson-0.2.0/src/cldfgeojson.egg-info/dependency_links.txt
--rw-rw-r--   0 robert    (1000) robert    (1000)        1 2024-04-25 09:27:55.000000 cldfgeojson-0.2.0/src/cldfgeojson.egg-info/not-zip-safe
--rw-rw-r--   0 robert    (1000) robert    (1000)      120 2024-04-26 09:07:19.000000 cldfgeojson-0.2.0/src/cldfgeojson.egg-info/requires.txt
--rw-rw-r--   0 robert    (1000) robert    (1000)       12 2024-04-26 09:07:19.000000 cldfgeojson-0.2.0/src/cldfgeojson.egg-info/top_level.txt
-drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2024-04-26 09:07:19.738656 cldfgeojson-0.2.0/tests/
--rw-rw-r--   0 robert    (1000) robert    (1000)     3981 2024-04-26 05:56:16.000000 cldfgeojson-0.2.0/tests/test_create.py
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2024-05-17 09:22:55.568064 cldfgeojson-0.2.1/
+-rw-rw-r--   0 robert    (1000) robert    (1000)    11357 2024-04-25 05:54:39.000000 cldfgeojson-0.2.1/LICENSE
+-rw-rw-r--   0 robert    (1000) robert    (1000)       50 2024-04-25 05:55:32.000000 cldfgeojson-0.2.1/MANIFEST.in
+-rw-rw-r--   0 robert    (1000) robert    (1000)     1946 2024-05-17 09:22:55.568064 cldfgeojson-0.2.1/PKG-INFO
+-rw-rw-r--   0 robert    (1000) robert    (1000)      723 2024-04-26 06:13:24.000000 cldfgeojson-0.2.1/README.md
+-rw-rw-r--   0 robert    (1000) robert    (1000)       81 2024-04-25 05:55:40.000000 cldfgeojson-0.2.1/pyproject.toml
+-rw-rw-r--   0 robert    (1000) robert    (1000)     1892 2024-05-17 09:22:55.568064 cldfgeojson-0.2.1/setup.cfg
+-rwxrwxr-x   0 robert    (1000) robert    (1000)       39 2024-04-25 05:56:22.000000 cldfgeojson-0.2.1/setup.py
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2024-05-17 09:22:55.568064 cldfgeojson-0.2.1/src/
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2024-05-17 09:22:55.568064 cldfgeojson-0.2.1/src/cldfgeojson/
+-rw-rw-r--   0 robert    (1000) robert    (1000)      106 2024-05-17 09:21:55.000000 cldfgeojson-0.2.1/src/cldfgeojson/__init__.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     6679 2024-05-16 15:28:13.000000 cldfgeojson-0.2.1/src/cldfgeojson/create.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)      928 2024-04-26 06:42:20.000000 cldfgeojson-0.2.1/src/cldfgeojson/geojson.py
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2024-05-17 09:22:55.568064 cldfgeojson-0.2.1/src/cldfgeojson.egg-info/
+-rw-r--r--   0 robert    (1000) robert    (1000)     1946 2024-05-17 09:22:55.000000 cldfgeojson-0.2.1/src/cldfgeojson.egg-info/PKG-INFO
+-rw-rw-r--   0 robert    (1000) robert    (1000)      397 2024-05-17 09:22:55.000000 cldfgeojson-0.2.1/src/cldfgeojson.egg-info/SOURCES.txt
+-rw-rw-r--   0 robert    (1000) robert    (1000)        1 2024-05-17 09:22:55.000000 cldfgeojson-0.2.1/src/cldfgeojson.egg-info/dependency_links.txt
+-rw-rw-r--   0 robert    (1000) robert    (1000)        1 2024-04-25 09:27:55.000000 cldfgeojson-0.2.1/src/cldfgeojson.egg-info/not-zip-safe
+-rw-rw-r--   0 robert    (1000) robert    (1000)      120 2024-05-17 09:22:55.000000 cldfgeojson-0.2.1/src/cldfgeojson.egg-info/requires.txt
+-rw-rw-r--   0 robert    (1000) robert    (1000)       12 2024-05-17 09:22:55.000000 cldfgeojson-0.2.1/src/cldfgeojson.egg-info/top_level.txt
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2024-05-17 09:22:55.568064 cldfgeojson-0.2.1/tests/
+-rw-rw-r--   0 robert    (1000) robert    (1000)     3981 2024-04-26 05:56:16.000000 cldfgeojson-0.2.1/tests/test_create.py
```

### Comparing `cldfgeojson-0.2.0/LICENSE` & `cldfgeojson-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cldfgeojson-0.2.0/PKG-INFO` & `cldfgeojson-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cldfgeojson
-Version: 0.2.0
+Version: 0.2.1
 Summary: Functionality to access and curate GeoJSON in CLDF datasets
 Home-page: https://github.com/cldf/cldfgeojson
 Author: Robert Forkel
 Author-email: dlce.rdm@eva.mpg.de
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/cldf/cldfgeojson/issues
 Keywords: linguistics
```

### Comparing `cldfgeojson-0.2.0/README.md` & `cldfgeojson-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `cldfgeojson-0.2.0/setup.cfg` & `cldfgeojson-0.2.1/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cldfgeojson
-version = 0.2.0
+version = 0.2.1
 author = Robert Forkel
 author_email = dlce.rdm@eva.mpg.de
 description = Functionality to access and curate GeoJSON in CLDF datasets
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = linguistics
 license = Apache 2.0
```

### Comparing `cldfgeojson-0.2.0/src/cldfgeojson/create.py` & `cldfgeojson-0.2.1/src/cldfgeojson/create.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,29 +71,34 @@
                     buffer: typing.Union[float, None] = 0.001,
                     ) -> geojson.Geometry:
     """
     Merge the geographic structures supplied as GeoJSON Features or Geometries.
 
     :param features: An iterable of geographic structures.
     :param buffer: A buffer to be added to the shapes in order to make them overlap, thereby \
-    removing internal boundaries when merging. Specify `None` to add no buffer.
+    removing internal boundaries when merging. Will be subtracted from the merged geometry. \
+    Specify `None` to add no buffer.
     :return: The resulting Geometry object representing the merged shapes.
     """
     def get_shape(f):
         s = shape(f.get('geometry', f))
         if buffer:
             s = s.buffer(buffer)
         return s
-    return union_all([get_shape(f) for f in features])
+    res = union_all([get_shape(f) for f in features])
+    if buffer:
+        res = res.buffer(-buffer)
+    return res.__geo_interface__
 
 
 def aggregate(shapes: typing.Iterable[typing.Tuple[str, geojson.Feature, str]],
               glottolog: typing.Union[Glottolog, Dataset],
               level: str = 'language',
               buffer: typing.Union[float, None] = 0.001,
+              opacity: float = 0.8,
               ) -> typing.Tuple[
         typing.List[geojson.Feature],
         typing.List[typing.Tuple[Languoid, list, str]]]:
     """
     :param shapes: Iterable of (feature ID, GeoJSON feature, Glottocode) triples.
     :param glottolog: Glottolog data can be supplied either as `pyglottolog.Glottolog` API object \
     or as glottolog-cldf `pycldf.Dataset`.
@@ -150,11 +155,10 @@
         features.append(dict(
             type="Feature",
             properties={
                 'title': glangs[gc].name,
                 'fill': colors[lang2fam[gc]],
                 'family': glangs[lang2fam[gc]].name if lang2fam[gc] != gc else None,
                 'cldf:languageReference': gc,
-                'fill-opacity': 0.8},
-            geometry=merged_geometry(
-                [p[1] for p in polys_by_code[gc]], buffer=buffer).__geo_interface__))
+                'fill-opacity': opacity},
+            geometry=merged_geometry([p[1] for p in polys_by_code[gc]], buffer=buffer)))
     return features, languoids
```

### Comparing `cldfgeojson-0.2.0/src/cldfgeojson/geojson.py` & `cldfgeojson-0.2.1/src/cldfgeojson/geojson.py`

 * *Files identical despite different names*

### Comparing `cldfgeojson-0.2.0/src/cldfgeojson.egg-info/PKG-INFO` & `cldfgeojson-0.2.1/src/cldfgeojson.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cldfgeojson
-Version: 0.2.0
+Version: 0.2.1
 Summary: Functionality to access and curate GeoJSON in CLDF datasets
 Home-page: https://github.com/cldf/cldfgeojson
 Author: Robert Forkel
 Author-email: dlce.rdm@eva.mpg.de
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/cldf/cldfgeojson/issues
 Keywords: linguistics
```

### Comparing `cldfgeojson-0.2.0/tests/test_create.py` & `cldfgeojson-0.2.1/tests/test_create.py`

 * *Files identical despite different names*

