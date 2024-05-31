# Comparing `tmp/lindi-0.3.8.tar.gz` & `tmp/lindi-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lindi-0.3.8.tar", max compression
+gzip compressed data, was "lindi-0.3.9.tar", max compression
```

## Comparing `lindi-0.3.8.tar` & `lindi-0.3.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1512 2024-03-15 13:05:25.255694 lindi-0.3.8/LICENSE
--rw-r--r--   0        0        0     5609 2024-05-13 21:58:43.566094 lindi-0.3.8/README.md
--rw-r--r--   0        0        0     1314 2024-05-13 21:58:43.568424 lindi-0.3.8/lindi/File/File.py
--rw-r--r--   0        0        0        0 2024-05-13 21:58:43.568519 lindi-0.3.8/lindi/File/__init__.py
--rw-r--r--   0        0        0    32505 2024-05-22 06:14:26.999857 lindi-0.3.8/lindi/LindiH5ZarrStore/LindiH5ZarrStore.py
--rw-r--r--   0        0        0      613 2024-05-18 21:55:23.472567 lindi-0.3.8/lindi/LindiH5ZarrStore/LindiH5ZarrStoreOpts.py
--rw-r--r--   0        0        0      169 2024-05-13 21:58:43.569750 lindi-0.3.8/lindi/LindiH5ZarrStore/__init__.py
--rw-r--r--   0        0        0     5310 2024-05-18 21:55:23.473554 lindi-0.3.8/lindi/LindiH5ZarrStore/_util.py
--rw-r--r--   0        0        0     2242 2024-04-20 02:25:06.810707 lindi-0.3.8/lindi/LindiH5pyFile/LindiH5pyAttributes.py
--rw-r--r--   0        0        0    11982 2024-05-27 23:07:58.518932 lindi-0.3.8/lindi/LindiH5pyFile/LindiH5pyDataset.py
--rw-r--r--   0        0        0    26328 2024-05-18 21:55:23.473895 lindi-0.3.8/lindi/LindiH5pyFile/LindiH5pyFile.py
--rw-r--r--   0        0        0     6051 2024-05-20 04:06:13.795499 lindi-0.3.8/lindi/LindiH5pyFile/LindiH5pyGroup.py
--rw-r--r--   0        0        0      255 2024-03-27 05:24:30.816048 lindi-0.3.8/lindi/LindiH5pyFile/LindiH5pyLink.py
--rw-r--r--   0        0        0      478 2024-04-18 05:06:23.250257 lindi-0.3.8/lindi/LindiH5pyFile/LindiH5pyReference.py
--rw-r--r--   0        0        0    11675 2024-05-28 15:47:40.201989 lindi-0.3.8/lindi/LindiH5pyFile/LindiReferenceFileSystemStore.py
--rw-r--r--   0        0        0      327 2024-03-27 05:24:30.816756 lindi-0.3.8/lindi/LindiH5pyFile/__init__.py
--rw-r--r--   0        0        0      528 2024-04-20 02:25:06.814407 lindi-0.3.8/lindi/LindiH5pyFile/writers/LindiH5pyAttributesWriter.py
--rw-r--r--   0        0        0     1941 2024-04-20 02:25:06.814919 lindi-0.3.8/lindi/LindiH5pyFile/writers/LindiH5pyDatasetWriter.py
--rw-r--r--   0        0        0     6651 2024-05-13 21:58:39.793666 lindi-0.3.8/lindi/LindiH5pyFile/writers/LindiH5pyGroupWriter.py
--rw-r--r--   0        0        0        0 2024-04-18 05:06:23.251611 lindi-0.3.8/lindi/LindiH5pyFile/writers/__init__.py
--rw-r--r--   0        0        0    16448 2024-05-27 14:43:57.139282 lindi-0.3.8/lindi/LindiRemfile/LindiRemfile.py
--rw-r--r--   0        0        0        0 2024-05-13 21:58:43.572320 lindi-0.3.8/lindi/LindiRemfile/__init__.py
--rw-r--r--   0        0        0     8772 2024-05-13 21:58:43.572941 lindi-0.3.8/lindi/LindiStagingStore/LindiStagingStore.py
--rw-r--r--   0        0        0     3506 2024-05-13 21:58:43.573425 lindi-0.3.8/lindi/LindiStagingStore/StagingArea.py
--rw-r--r--   0        0        0       76 2024-04-20 02:25:06.816263 lindi-0.3.8/lindi/LindiStagingStore/__init__.py
--rw-r--r--   0        0        0     2688 2024-05-22 06:14:27.002296 lindi-0.3.8/lindi/LocalCache/LocalCache.py
--rw-r--r--   0        0        0        0 2024-05-13 21:58:43.573886 lindi-0.3.8/lindi/LocalCache/__init__.py
--rw-r--r--   0        0        0      408 2024-05-22 06:14:27.002942 lindi-0.3.8/lindi/__init__.py
--rw-r--r--   0        0        0        0 2024-04-18 05:06:23.251715 lindi-0.3.8/lindi/conversion/__init__.py
--rw-r--r--   0        0        0      167 2024-04-18 05:06:23.251940 lindi-0.3.8/lindi/conversion/_util.py
--rw-r--r--   0        0        0     5907 2024-04-18 05:06:23.252121 lindi-0.3.8/lindi/conversion/attr_conversion.py
--rw-r--r--   0        0        0    10819 2024-04-20 02:25:06.817742 lindi-0.3.8/lindi/conversion/create_zarr_dataset_from_h5_data.py
--rw-r--r--   0        0        0     1079 2024-04-18 05:06:23.252489 lindi-0.3.8/lindi/conversion/decode_references.py
--rw-r--r--   0        0        0     2887 2024-05-13 21:58:39.794516 lindi-0.3.8/lindi/conversion/h5_filters_to_codecs.py
--rw-r--r--   0        0        0     2041 2024-04-18 05:06:23.253039 lindi-0.3.8/lindi/conversion/h5_ref_to_zarr_attr.py
--rw-r--r--   0        0        0      936 2024-04-18 05:06:23.253228 lindi-0.3.8/lindi/conversion/nan_inf_ninf.py
--rw-r--r--   0        0        0      503 2024-04-18 05:06:23.253445 lindi-0.3.8/lindi/conversion/reformat_json.py
--rw-r--r--   0        0        0      746 2024-05-28 15:50:35.125765 lindi-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     6307 1970-01-01 00:00:00.000000 lindi-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1512 2024-03-15 13:05:25.255694 lindi-0.3.9/LICENSE
+-rw-r--r--   0        0        0     5609 2024-05-13 21:58:43.566094 lindi-0.3.9/README.md
+-rw-r--r--   0        0        0     1314 2024-05-13 21:58:43.568424 lindi-0.3.9/lindi/File/File.py
+-rw-r--r--   0        0        0        0 2024-05-13 21:58:43.568519 lindi-0.3.9/lindi/File/__init__.py
+-rw-r--r--   0        0        0    33051 2024-05-29 15:54:31.483661 lindi-0.3.9/lindi/LindiH5ZarrStore/LindiH5ZarrStore.py
+-rw-r--r--   0        0        0      613 2024-05-18 21:55:23.472567 lindi-0.3.9/lindi/LindiH5ZarrStore/LindiH5ZarrStoreOpts.py
+-rw-r--r--   0        0        0      169 2024-05-13 21:58:43.569750 lindi-0.3.9/lindi/LindiH5ZarrStore/__init__.py
+-rw-r--r--   0        0        0     5310 2024-05-18 21:55:23.473554 lindi-0.3.9/lindi/LindiH5ZarrStore/_util.py
+-rw-r--r--   0        0        0     2242 2024-04-20 02:25:06.810707 lindi-0.3.9/lindi/LindiH5pyFile/LindiH5pyAttributes.py
+-rw-r--r--   0        0        0    11982 2024-05-29 13:54:37.928166 lindi-0.3.9/lindi/LindiH5pyFile/LindiH5pyDataset.py
+-rw-r--r--   0        0        0    26328 2024-05-29 13:55:16.270177 lindi-0.3.9/lindi/LindiH5pyFile/LindiH5pyFile.py
+-rw-r--r--   0        0        0     6051 2024-05-29 13:54:49.102973 lindi-0.3.9/lindi/LindiH5pyFile/LindiH5pyGroup.py
+-rw-r--r--   0        0        0      255 2024-03-27 05:24:30.816048 lindi-0.3.9/lindi/LindiH5pyFile/LindiH5pyLink.py
+-rw-r--r--   0        0        0      478 2024-04-18 05:06:23.250257 lindi-0.3.9/lindi/LindiH5pyFile/LindiH5pyReference.py
+-rw-r--r--   0        0        0    11740 2024-05-29 15:54:31.484284 lindi-0.3.9/lindi/LindiH5pyFile/LindiReferenceFileSystemStore.py
+-rw-r--r--   0        0        0      327 2024-03-27 05:24:30.816756 lindi-0.3.9/lindi/LindiH5pyFile/__init__.py
+-rw-r--r--   0        0        0      528 2024-04-20 02:25:06.814407 lindi-0.3.9/lindi/LindiH5pyFile/writers/LindiH5pyAttributesWriter.py
+-rw-r--r--   0        0        0     1941 2024-04-20 02:25:06.814919 lindi-0.3.9/lindi/LindiH5pyFile/writers/LindiH5pyDatasetWriter.py
+-rw-r--r--   0        0        0     6651 2024-05-29 13:55:03.181729 lindi-0.3.9/lindi/LindiH5pyFile/writers/LindiH5pyGroupWriter.py
+-rw-r--r--   0        0        0        0 2024-04-18 05:06:23.251611 lindi-0.3.9/lindi/LindiH5pyFile/writers/__init__.py
+-rw-r--r--   0        0        0    16448 2024-05-27 14:43:57.139282 lindi-0.3.9/lindi/LindiRemfile/LindiRemfile.py
+-rw-r--r--   0        0        0        0 2024-05-13 21:58:43.572320 lindi-0.3.9/lindi/LindiRemfile/__init__.py
+-rw-r--r--   0        0        0     8772 2024-05-13 21:58:43.572941 lindi-0.3.9/lindi/LindiStagingStore/LindiStagingStore.py
+-rw-r--r--   0        0        0     3506 2024-05-13 21:58:43.573425 lindi-0.3.9/lindi/LindiStagingStore/StagingArea.py
+-rw-r--r--   0        0        0       76 2024-04-20 02:25:06.816263 lindi-0.3.9/lindi/LindiStagingStore/__init__.py
+-rw-r--r--   0        0        0     2688 2024-05-22 06:14:27.002296 lindi-0.3.9/lindi/LocalCache/LocalCache.py
+-rw-r--r--   0        0        0        0 2024-05-13 21:58:43.573886 lindi-0.3.9/lindi/LocalCache/__init__.py
+-rw-r--r--   0        0        0      408 2024-05-22 06:14:27.002942 lindi-0.3.9/lindi/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-18 05:06:23.251715 lindi-0.3.9/lindi/conversion/__init__.py
+-rw-r--r--   0        0        0      167 2024-04-18 05:06:23.251940 lindi-0.3.9/lindi/conversion/_util.py
+-rw-r--r--   0        0        0     5907 2024-04-18 05:06:23.252121 lindi-0.3.9/lindi/conversion/attr_conversion.py
+-rw-r--r--   0        0        0    10819 2024-05-29 13:54:33.143538 lindi-0.3.9/lindi/conversion/create_zarr_dataset_from_h5_data.py
+-rw-r--r--   0        0        0     1079 2024-04-18 05:06:23.252489 lindi-0.3.9/lindi/conversion/decode_references.py
+-rw-r--r--   0        0        0     2887 2024-05-13 21:58:39.794516 lindi-0.3.9/lindi/conversion/h5_filters_to_codecs.py
+-rw-r--r--   0        0        0     2041 2024-04-18 05:06:23.253039 lindi-0.3.9/lindi/conversion/h5_ref_to_zarr_attr.py
+-rw-r--r--   0        0        0      936 2024-04-18 05:06:23.253228 lindi-0.3.9/lindi/conversion/nan_inf_ninf.py
+-rw-r--r--   0        0        0      503 2024-04-18 05:06:23.253445 lindi-0.3.9/lindi/conversion/reformat_json.py
+-rw-r--r--   0        0        0      746 2024-05-29 15:55:25.744477 lindi-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     6307 1970-01-01 00:00:00.000000 lindi-0.3.9/PKG-INFO
```

### Comparing `lindi-0.3.8/LICENSE` & `lindi-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lindi-0.3.8/README.md` & `lindi-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `lindi-0.3.8/lindi/File/File.py` & `lindi-0.3.9/lindi/File/File.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.8/lindi/LindiH5ZarrStore/LindiH5ZarrStore.py` & `lindi-0.3.9/lindi/LindiH5ZarrStore/LindiH5ZarrStore.py`

 * *Files 2% similar despite different names*

```diff
@@ -299,24 +299,30 @@
 
         filters = h5_filters_to_codecs(h5_item)
 
         # We create a dummy zarr dataset with the appropriate shape, chunks,
         # dtype, and filters and then copy the .zarray JSON text from it
         memory_store = MemoryStore()
         dummy_group = zarr.group(store=memory_store)
+        chunks = h5_item.chunks
+        if chunks is None:
+            # It's important to not have chunks be None here because that would
+            # let zarr choose an optimal chunking, whereas we need this to reflect
+            # the actual chunking in the HDF5 file.
+            chunks = h5_item.shape
+            if np.prod(chunks) == 0:
+                # A chunking of (0,) or (0, 0) or (0, 0, 0), etc. is not allowed in Zarr
+                chunks = [1] * len(chunks)
         # Importantly, I'm pretty sure this doesn't actually create the
         # chunks in the memory store. That's important because we just need
         # to get the .zarray JSON text from the dummy group.
         dummy_group.create_dataset(
             name="dummy_array",
             shape=h5_item.shape,
-            # It's important to not have chunks be None here because that would
-            # let zarr choose an optimal chunking, whereas we need this to reflect
-            # the actual chunking in the HDF5 file.
-            chunks=h5_item.chunks if h5_item.chunks is not None else h5_item.shape,
+            chunks=chunks,
             dtype=h5_item.dtype,
             compressor=None,
             order="C",
             fill_value=h5_item.fillvalue,
             filters=filters
         )
         zarray_text = reformat_json(memory_store.get("dummy_array/.zarray"))
@@ -430,14 +436,18 @@
 
     def _add_chunk_info_to_refs(self, key_parent: str, add_ref: Callable, add_ref_chunk: Callable):
         if self._h5f is None:
             raise Exception("Store is closed")
         h5_item = self._h5f.get('/' + key_parent, None)
         assert isinstance(h5_item, h5py.Dataset)
 
+        # If the shape is (0,), (0, 0), (0, 0, 0), etc., then do not add any chunk references
+        if np.prod(h5_item.shape) == 0:
+            return
+
         # For the case of a scalar dataset, we need to check a few things
         if h5_item.ndim == 0:
             if h5_item.chunks is not None:
                 raise Exception(
                     f"Unable to handle case where chunks is not None but ndim is 0 for dataset {key_parent}"
                 )
 
@@ -585,16 +595,18 @@
                     # If the content is not valid ASCII, then we base64 encode it. The
                     # reference file system reader will know what to do with it.
                     ret["refs"][key] = (b"base64:" + base64.b64encode(content)).decode(
                         "ascii"
                     )
 
         def _add_ref_chunk(key: str, data: Tuple[str, int, int]):
-            assert data[1] is not None
-            assert data[2] is not None
+            assert data[1] is not None, \
+                f"{key} chunk data is invalid. Element at index 1 cannot be None: {data}"
+            assert data[2] is not None, \
+                f"{key} chunk data is invalid. Element at index 2 cannot be None: {data}"
             ret["refs"][key] = list(data)  # downstream expects a list like on read from a JSON file
 
         def _process_group(key, item: h5py.Group):
             if isinstance(item, h5py.Group):
                 # Add the .zattrs and .zgroup files for the group
                 zattrs_bytes = self.get(_join(key, ".zattrs"))
                 if zattrs_bytes != b"{}":  # don't include empty zattrs
```

### Comparing `lindi-0.3.8/lindi/LindiH5ZarrStore/LindiH5ZarrStoreOpts.py` & `lindi-0.3.9/lindi/LindiH5ZarrStore/LindiH5ZarrStoreOpts.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.8/lindi/LindiH5ZarrStore/_util.py` & `lindi-0.3.9/lindi/LindiH5ZarrStore/_util.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.8/lindi/LindiH5pyFile/LindiH5pyAttributes.py` & `lindi-0.3.9/lindi/LindiH5pyFile/LindiH5pyAttributes.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.8/lindi/LindiH5pyFile/LindiH5pyDataset.py` & `lindi-0.3.9/lindi/LindiH5pyFile/LindiH5pyDataset.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.8/lindi/LindiH5pyFile/LindiH5pyFile.py` & `lindi-0.3.9/lindi/LindiH5pyFile/LindiH5pyFile.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.8/lindi/LindiH5pyFile/LindiH5pyGroup.py` & `lindi-0.3.9/lindi/LindiH5pyFile/LindiH5pyGroup.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.8/lindi/LindiH5pyFile/LindiReferenceFileSystemStore.py` & `lindi-0.3.9/lindi/LindiH5pyFile/LindiReferenceFileSystemStore.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,15 +111,17 @@
                     raise Exception(f"Problem with templates: value for {k} must be a string")
 
         self.rfs = rfs
         self.mode = mode
         self.local_cache = local_cache
 
     # These methods are overridden from MutableMapping
-    def __contains__(self, key: str):
+    def __contains__(self, key: object):
+        if not isinstance(key, str):
+            return False
         return key in self.rfs["refs"]
 
     def __getitem__(self, key: str):
         if key not in self.rfs["refs"]:
             raise KeyError(key)
         x = self.rfs["refs"][key]
         if isinstance(x, str):
```

### Comparing `lindi-0.3.8/lindi/LindiH5pyFile/writers/LindiH5pyAttributesWriter.py` & `lindi-0.3.9/lindi/LindiH5pyFile/writers/LindiH5pyAttributesWriter.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.8/lindi/LindiH5pyFile/writers/LindiH5pyDatasetWriter.py` & `lindi-0.3.9/lindi/LindiH5pyFile/writers/LindiH5pyDatasetWriter.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.8/lindi/LindiH5pyFile/writers/LindiH5pyGroupWriter.py` & `lindi-0.3.9/lindi/LindiH5pyFile/writers/LindiH5pyGroupWriter.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.8/lindi/LindiRemfile/LindiRemfile.py` & `lindi-0.3.9/lindi/LindiRemfile/LindiRemfile.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.8/lindi/LindiStagingStore/LindiStagingStore.py` & `lindi-0.3.9/lindi/LindiStagingStore/LindiStagingStore.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.8/lindi/LindiStagingStore/StagingArea.py` & `lindi-0.3.9/lindi/LindiStagingStore/StagingArea.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.8/lindi/LocalCache/LocalCache.py` & `lindi-0.3.9/lindi/LocalCache/LocalCache.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.8/lindi/conversion/attr_conversion.py` & `lindi-0.3.9/lindi/conversion/attr_conversion.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.8/lindi/conversion/create_zarr_dataset_from_h5_data.py` & `lindi-0.3.9/lindi/conversion/create_zarr_dataset_from_h5_data.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.8/lindi/conversion/decode_references.py` & `lindi-0.3.9/lindi/conversion/decode_references.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.8/lindi/conversion/h5_filters_to_codecs.py` & `lindi-0.3.9/lindi/conversion/h5_filters_to_codecs.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.8/lindi/conversion/h5_ref_to_zarr_attr.py` & `lindi-0.3.9/lindi/conversion/h5_ref_to_zarr_attr.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.8/lindi/conversion/nan_inf_ninf.py` & `lindi-0.3.9/lindi/conversion/nan_inf_ninf.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.8/pyproject.toml` & `lindi-0.3.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lindi"
-version = "0.3.8"
+version = "0.3.9"
 description = ""
 authors = [
     "Jeremy Magland <jmagland@flatironinstitute.org>",
     "Ryan Ly <rly@lbl.gov>",
     "Oliver Ruebel <oruebel@lbl.gov>"
 ]
 readme = "README.md"
```

### Comparing `lindi-0.3.8/PKG-INFO` & `lindi-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lindi
-Version: 0.3.8
+Version: 0.3.9
 Summary: 
 Author: Jeremy Magland
 Author-email: jmagland@flatironinstitute.org
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

