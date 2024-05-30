# Comparing `tmp/dagster-embedded-elt-0.23.7.tar.gz` & `tmp/dagster-embedded-elt-0.23.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-embedded-elt-0.23.7.tar", last modified: Thu May 23 20:56:30 2024, max compression
+gzip compressed data, was "dagster-embedded-elt-0.23.8.tar", last modified: Thu May 30 22:12:04 2024, max compression
```

## Comparing `dagster-embedded-elt-0.23.7.tar` & `dagster-embedded-elt-0.23.8.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:56:30.176526 dagster-embedded-elt-0.23.7/
--rw-r--r--   0 root         (0) root         (0)    11349 2024-05-23 20:50:32.000000 dagster-embedded-elt-0.23.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)       97 2024-05-23 20:50:32.000000 dagster-embedded-elt-0.23.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      744 2024-05-23 20:56:30.176526 dagster-embedded-elt-0.23.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      146 2024-05-23 20:50:32.000000 dagster-embedded-elt-0.23.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:56:30.176526 dagster-embedded-elt-0.23.7/dagster_embedded_elt/
--rw-r--r--   0 root         (0) root         (0)      163 2024-05-23 20:50:32.000000 dagster-embedded-elt-0.23.7/dagster_embedded_elt/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:56:30.176526 dagster-embedded-elt-0.23.7/dagster_embedded_elt/dlt/
--rw-r--r--   0 root         (0) root         (0)      270 2024-05-23 20:50:32.000000 dagster-embedded-elt-0.23.7/dagster_embedded_elt/dlt/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3947 2024-05-23 20:50:32.000000 dagster-embedded-elt-0.23.7/dagster_embedded_elt/dlt/asset_decorator.py
--rw-r--r--   0 root         (0) root         (0)      129 2024-05-23 20:50:32.000000 dagster-embedded-elt-0.23.7/dagster_embedded_elt/dlt/constants.py
--rw-r--r--   0 root         (0) root         (0)     7076 2024-05-23 20:50:32.000000 dagster-embedded-elt-0.23.7/dagster_embedded_elt/dlt/resource.py
--rw-r--r--   0 root         (0) root         (0)     1563 2024-05-23 20:50:32.000000 dagster-embedded-elt-0.23.7/dagster_embedded_elt/dlt/translator.py
--rw-r--r--   0 root         (0) root         (0)        8 2024-05-23 20:50:32.000000 dagster-embedded-elt-0.23.7/dagster_embedded_elt/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:56:30.176526 dagster-embedded-elt-0.23.7/dagster_embedded_elt/sling/
--rw-r--r--   0 root         (0) root         (0)      718 2024-05-23 20:50:32.000000 dagster-embedded-elt-0.23.7/dagster_embedded_elt/sling/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6011 2024-05-23 20:50:32.000000 dagster-embedded-elt-0.23.7/dagster_embedded_elt/sling/asset_decorator.py
--rw-r--r--   0 root         (0) root         (0)     4162 2024-05-23 20:50:32.000000 dagster-embedded-elt-0.23.7/dagster_embedded_elt/sling/asset_defs.py
--rw-r--r--   0 root         (0) root         (0)     8087 2024-05-23 20:50:32.000000 dagster-embedded-elt-0.23.7/dagster_embedded_elt/sling/dagster_sling_translator.py
--rw-r--r--   0 root         (0) root         (0)    20594 2024-05-23 20:50:32.000000 dagster-embedded-elt-0.23.7/dagster_embedded_elt/sling/resources.py
--rw-r--r--   0 root         (0) root         (0)     1106 2024-05-23 20:50:32.000000 dagster-embedded-elt-0.23.7/dagster_embedded_elt/sling/sling_replication.py
--rw-r--r--   0 root         (0) root         (0)       23 2024-05-23 20:50:32.000000 dagster-embedded-elt-0.23.7/dagster_embedded_elt/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:56:30.176526 dagster-embedded-elt-0.23.7/dagster_embedded_elt.egg-info/
--rw-r--r--   0 root         (0) root         (0)      744 2024-05-23 20:56:29.000000 dagster-embedded-elt-0.23.7/dagster_embedded_elt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      886 2024-05-23 20:56:29.000000 dagster-embedded-elt-0.23.7/dagster_embedded_elt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 20:56:29.000000 dagster-embedded-elt-0.23.7/dagster_embedded_elt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 20:56:29.000000 dagster-embedded-elt-0.23.7/dagster_embedded_elt.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       52 2024-05-23 20:56:29.000000 dagster-embedded-elt-0.23.7/dagster_embedded_elt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2024-05-23 20:56:29.000000 dagster-embedded-elt-0.23.7/dagster_embedded_elt.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      124 2024-05-23 20:50:32.000000 dagster-embedded-elt-0.23.7/integration.yaml
--rw-r--r--   0 root         (0) root         (0)      167 2024-05-23 20:56:30.180526 dagster-embedded-elt-0.23.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1427 2024-05-23 20:50:32.000000 dagster-embedded-elt-0.23.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:12:04.307031 dagster-embedded-elt-0.23.8/
+-rw-r--r--   0 root         (0) root         (0)    11349 2024-05-30 22:04:22.000000 dagster-embedded-elt-0.23.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       97 2024-05-30 22:04:22.000000 dagster-embedded-elt-0.23.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      744 2024-05-30 22:12:04.307031 dagster-embedded-elt-0.23.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      146 2024-05-30 22:04:22.000000 dagster-embedded-elt-0.23.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:12:04.299031 dagster-embedded-elt-0.23.8/dagster_embedded_elt/
+-rw-r--r--   0 root         (0) root         (0)      163 2024-05-30 22:04:22.000000 dagster-embedded-elt-0.23.8/dagster_embedded_elt/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:12:04.303031 dagster-embedded-elt-0.23.8/dagster_embedded_elt/dlt/
+-rw-r--r--   0 root         (0) root         (0)      270 2024-05-30 22:04:22.000000 dagster-embedded-elt-0.23.8/dagster_embedded_elt/dlt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4151 2024-05-30 22:04:22.000000 dagster-embedded-elt-0.23.8/dagster_embedded_elt/dlt/asset_decorator.py
+-rw-r--r--   0 root         (0) root         (0)      129 2024-05-30 22:04:22.000000 dagster-embedded-elt-0.23.8/dagster_embedded_elt/dlt/constants.py
+-rw-r--r--   0 root         (0) root         (0)     7502 2024-05-30 22:04:22.000000 dagster-embedded-elt-0.23.8/dagster_embedded_elt/dlt/resource.py
+-rw-r--r--   0 root         (0) root         (0)     1913 2024-05-30 22:04:22.000000 dagster-embedded-elt-0.23.8/dagster_embedded_elt/dlt/translator.py
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-30 22:04:22.000000 dagster-embedded-elt-0.23.8/dagster_embedded_elt/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:12:04.307031 dagster-embedded-elt-0.23.8/dagster_embedded_elt/sling/
+-rw-r--r--   0 root         (0) root         (0)      718 2024-05-30 22:04:22.000000 dagster-embedded-elt-0.23.8/dagster_embedded_elt/sling/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6011 2024-05-30 22:04:22.000000 dagster-embedded-elt-0.23.8/dagster_embedded_elt/sling/asset_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     4162 2024-05-30 22:04:22.000000 dagster-embedded-elt-0.23.8/dagster_embedded_elt/sling/asset_defs.py
+-rw-r--r--   0 root         (0) root         (0)     8087 2024-05-30 22:04:22.000000 dagster-embedded-elt-0.23.8/dagster_embedded_elt/sling/dagster_sling_translator.py
+-rw-r--r--   0 root         (0) root         (0)    20594 2024-05-30 22:04:22.000000 dagster-embedded-elt-0.23.8/dagster_embedded_elt/sling/resources.py
+-rw-r--r--   0 root         (0) root         (0)     1106 2024-05-30 22:04:22.000000 dagster-embedded-elt-0.23.8/dagster_embedded_elt/sling/sling_replication.py
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-30 22:04:22.000000 dagster-embedded-elt-0.23.8/dagster_embedded_elt/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 22:12:04.299031 dagster-embedded-elt-0.23.8/dagster_embedded_elt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      744 2024-05-30 22:12:04.000000 dagster-embedded-elt-0.23.8/dagster_embedded_elt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      886 2024-05-30 22:12:04.000000 dagster-embedded-elt-0.23.8/dagster_embedded_elt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 22:12:04.000000 dagster-embedded-elt-0.23.8/dagster_embedded_elt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 22:12:04.000000 dagster-embedded-elt-0.23.8/dagster_embedded_elt.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       52 2024-05-30 22:12:04.000000 dagster-embedded-elt-0.23.8/dagster_embedded_elt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-30 22:12:04.000000 dagster-embedded-elt-0.23.8/dagster_embedded_elt.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      124 2024-05-30 22:04:22.000000 dagster-embedded-elt-0.23.8/integration.yaml
+-rw-r--r--   0 root         (0) root         (0)      167 2024-05-30 22:12:04.307031 dagster-embedded-elt-0.23.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1427 2024-05-30 22:04:22.000000 dagster-embedded-elt-0.23.8/setup.py
```

### Comparing `dagster-embedded-elt-0.23.7/LICENSE` & `dagster-embedded-elt-0.23.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.7/PKG-INFO` & `dagster-embedded-elt-0.23.8/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-embedded-elt
-Version: 0.23.7
+Version: 0.23.8
 Summary: Package for performing ETL/ELT tasks with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-embedded-elt
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-embedded-elt-0.23.7/dagster_embedded_elt/dlt/asset_decorator.py` & `dagster-embedded-elt-0.23.8/dagster_embedded_elt/dlt/asset_decorator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Any, Callable, Optional
 
 from dagster import (
     AssetsDefinition,
     AssetSpec,
+    PartitionsDefinition,
     _check as check,
     multi_asset,
 )
 from dlt.extract.source import DltSource
 from dlt.pipeline.pipeline import Pipeline
 
 from .constants import META_KEY_PIPELINE, META_KEY_SOURCE, META_KEY_TRANSLATOR
@@ -16,14 +17,15 @@
 def dlt_assets(
     *,
     dlt_source: DltSource,
     dlt_pipeline: Pipeline,
     name: Optional[str] = None,
     group_name: Optional[str] = None,
     dlt_dagster_translator: Optional[DagsterDltTranslator] = None,
+    partitions_def: Optional[PartitionsDefinition] = None,
 ) -> Callable[[Callable[..., Any]], AssetsDefinition]:
     """Asset Factory for using data load tool (dlt).
 
     Args:
         dlt_source (DltSource): The DltSource to be ingested.
         dlt_pipeline (Pipeline): The dlt Pipeline defining the destination parameters.
         name (Optional[str], optional): The name of the op.
@@ -84,23 +86,25 @@
         or DagsterDltTranslator()
     )
     return multi_asset(
         name=name,
         group_name=group_name,
         compute_kind="dlt",
         can_subset=True,
+        partitions_def=partitions_def,
         specs=[
             AssetSpec(
                 key=dlt_dagster_translator.get_asset_key(dlt_source_resource),
                 deps=dlt_dagster_translator.get_deps_asset_keys(dlt_source_resource),
                 auto_materialize_policy=dlt_dagster_translator.get_auto_materialize_policy(
                     dlt_source_resource
                 ),
                 metadata={
                     META_KEY_SOURCE: dlt_source,
                     META_KEY_PIPELINE: dlt_pipeline,
                     META_KEY_TRANSLATOR: dlt_dagster_translator,
+                    **dlt_dagster_translator.get_metadata(dlt_source_resource),
                 },
             )
             for dlt_source_resource in dlt_source.selected_resources.values()
         ],
     )
```

### Comparing `dagster-embedded-elt-0.23.7/dagster_embedded_elt/dlt/resource.py` & `dagster-embedded-elt-0.23.8/dagster_embedded_elt/dlt/resource.py`

 * *Files 6% similar despite different names*

```diff
@@ -114,24 +114,30 @@
             **kwargs (dict[str, Any]): Keyword args passed to pipeline `run` method
 
         Returns:
             Iterator[Union[MaterializeResult, AssetMaterialization]]: An iterator of MaterializeResult or AssetMaterialization
 
         """
         # This resource can be used in both `asset` and `op` definitions. In the context of an asset
-        # execution, we retrieve the dlt source, pipeline, and translator from the asset metadata.
-        # This allows us to provide the parameter _only_ in the `dlt_assets` decorator.
+        # execution, we retrieve the dlt source, pipeline, and translator from the asset metadata
+        # as a fallback mechanism. We give preference to explicit parameters to make it easy to
+        # customize execution, e.g., when using partitions.
         if isinstance(context, AssetExecutionContext):
             metadata_by_key = context.assets_def.metadata_by_key
             first_asset_metadata = next(iter(metadata_by_key.values()))
 
-            dlt_source = check.inst(first_asset_metadata.get(META_KEY_SOURCE), DltSource)
-            dlt_pipeline = check.inst(first_asset_metadata.get(META_KEY_PIPELINE), Pipeline)
+            dlt_source = check.inst(
+                dlt_source or first_asset_metadata.get(META_KEY_SOURCE), DltSource
+            )
+            dlt_pipeline = check.inst(
+                dlt_pipeline or first_asset_metadata.get(META_KEY_PIPELINE), Pipeline
+            )
             dagster_dlt_translator = check.inst(
-                first_asset_metadata.get(META_KEY_TRANSLATOR), DagsterDltTranslator
+                dagster_dlt_translator or first_asset_metadata.get(META_KEY_TRANSLATOR),
+                DagsterDltTranslator,
             )
 
         dlt_source = check.not_none(
             dlt_source, "dlt_source is a required parameter in an op context"
         )
         dlt_pipeline = check.not_none(
             dlt_pipeline, "dlt_pipeline is a required parameter in an op context"
@@ -158,14 +164,18 @@
             dlt_source = dlt_source.with_resources(
                 *[
                     dlt_source_resource.name
                     for dlt_source_resource in asset_key_dlt_source_resource_mapping.values()
                     if dlt_source_resource
                 ]
             )
+        # https://github.com/dagster-io/dagster/issues/21022
+        if context.has_partition_key:
+            last_partition_key = context.partition_keys[-1]
+            dlt_pipeline.pipeline_name += f"_{last_partition_key}"
 
         load_info = dlt_pipeline.run(dlt_source, **kwargs)
 
         load_info.raise_on_failed_jobs()
 
         has_asset_def: bool = bool(context and context.has_assets_def)
```

### Comparing `dagster-embedded-elt-0.23.7/dagster_embedded_elt/dlt/translator.py` & `dagster-embedded-elt-0.23.8/dagster_embedded_elt/dlt/translator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dataclasses import dataclass
-from typing import Iterable, Optional
+from typing import Any, Iterable, Mapping, Optional
 
 from dagster import (
     AssetKey,
     AutoMaterializePolicy,
 )
 from dagster._annotations import public
 from dlt.extract.resource import DltResource
@@ -47,7 +47,19 @@
             resource (DltResource): dlt resource / transformer
 
         Returns:
             Optional[AutoMaterializePolicy]: The automaterialize policy for a resource
 
         """
         return None
+
+    @public
+    def get_metadata(self, resource: DltResource) -> Mapping[str, Any]:
+        """Defines resource specific metadata.
+
+        Args:
+            resource (DltResource): dlt resource / transformer
+
+        Returns:
+            Mapping[str, Any]: The custom metadata entries for this resource.
+        """
+        return {}
```

### Comparing `dagster-embedded-elt-0.23.7/dagster_embedded_elt/sling/__init__.py` & `dagster-embedded-elt-0.23.8/dagster_embedded_elt/sling/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.7/dagster_embedded_elt/sling/asset_decorator.py` & `dagster-embedded-elt-0.23.8/dagster_embedded_elt/sling/asset_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.7/dagster_embedded_elt/sling/asset_defs.py` & `dagster-embedded-elt-0.23.8/dagster_embedded_elt/sling/asset_defs.py`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.7/dagster_embedded_elt/sling/dagster_sling_translator.py` & `dagster-embedded-elt-0.23.8/dagster_embedded_elt/sling/dagster_sling_translator.py`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.7/dagster_embedded_elt/sling/resources.py` & `dagster-embedded-elt-0.23.8/dagster_embedded_elt/sling/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.7/dagster_embedded_elt/sling/sling_replication.py` & `dagster-embedded-elt-0.23.8/dagster_embedded_elt/sling/sling_replication.py`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.7/dagster_embedded_elt.egg-info/PKG-INFO` & `dagster-embedded-elt-0.23.8/dagster_embedded_elt.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-embedded-elt
-Version: 0.23.7
+Version: 0.23.8
 Summary: Package for performing ETL/ELT tasks with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-embedded-elt
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-embedded-elt-0.23.7/dagster_embedded_elt.egg-info/SOURCES.txt` & `dagster-embedded-elt-0.23.8/dagster_embedded_elt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.7/setup.py` & `dagster-embedded-elt-0.23.8/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_embedded_elt_tests*"]),
     python_requires=">=3.8,<3.13",
-    install_requires=["dagster==1.7.7", "sling>=1.1.5", "dlt>=0.4"],
+    install_requires=["dagster==1.7.8", "sling>=1.1.5", "dlt>=0.4"],
     zip_safe=False,
     extras_require={
         "test": [
             "duckdb",
         ]
     },
 )
```

