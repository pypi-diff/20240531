# Comparing `tmp/crispr_millipede_helper-0.1.5.tar.gz` & `tmp/crispr_millipede_helper-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crispr_millipede_helper-0.1.5.tar", max compression
+gzip compressed data, was "crispr_millipede_helper-0.1.6.tar", max compression
```

## Comparing `crispr_millipede_helper-0.1.5.tar` & `crispr_millipede_helper-0.1.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       44 2024-01-30 18:58:55.790231 crispr_millipede_helper-0.1.5/crispr_millipede_helper/__init__.py
--rw-r--r--   0        0        0       30 2024-01-30 19:04:17.430762 crispr_millipede_helper-0.1.5/crispr_millipede_helper/models/__init__.py
--rw-r--r--   0        0        0     1369 2024-01-30 15:53:10.605794 crispr_millipede_helper-0.1.5/crispr_millipede_helper/models/pipeline_models.py
--rw-r--r--   0        0        0       26 2024-01-30 19:04:26.497177 crispr_millipede_helper-0.1.5/crispr_millipede_helper/pipeline/__init__.py
--rw-r--r--   0        0        0    10256 2024-01-30 15:56:45.168155 crispr_millipede_helper-0.1.5/crispr_millipede_helper/pipeline/InitialFile.py
--rw-r--r--   0        0        0      502 2024-01-30 19:04:37.875031 crispr_millipede_helper-0.1.5/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-30 15:38:23.041146 crispr_millipede_helper-0.1.5/README.md
--rw-r--r--   0        0        0      734 1970-01-01 00:00:00.000000 crispr_millipede_helper-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       44 2024-01-30 18:58:55.790231 crispr_millipede_helper-0.1.6/crispr_millipede_helper/__init__.py
+-rw-r--r--   0        0        0       30 2024-01-30 19:04:17.430762 crispr_millipede_helper-0.1.6/crispr_millipede_helper/models/__init__.py
+-rw-r--r--   0        0        0     1360 2024-05-31 20:09:15.481891 crispr_millipede_helper-0.1.6/crispr_millipede_helper/models/pipeline_models.py
+-rw-r--r--   0        0        0       26 2024-01-30 19:04:26.497177 crispr_millipede_helper-0.1.6/crispr_millipede_helper/pipeline/__init__.py
+-rw-r--r--   0        0        0    10206 2024-05-31 20:13:05.254177 crispr_millipede_helper-0.1.6/crispr_millipede_helper/pipeline/InitialFile.py
+-rw-r--r--   0        0        0      502 2024-05-31 20:13:31.284691 crispr_millipede_helper-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-01-30 15:38:23.041146 crispr_millipede_helper-0.1.6/README.md
+-rw-r--r--   0        0        0      734 1970-01-01 00:00:00.000000 crispr_millipede_helper-0.1.6/PKG-INFO
```

### Comparing `crispr_millipede_helper-0.1.5/crispr_millipede_helper/models/pipeline_models.py` & `crispr_millipede_helper-0.1.6/crispr_millipede_helper/models/pipeline_models.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from dataclasses import dataclass
 from typing import Optional, List
 import pandas as pd
 
 @dataclass
 class IndexPairPipelineBean:
-    barcode_index: str
-    i5_index: str
+    index2: str
+    index1: str
     read1_fn: str
     read2_fn: Optional[str]
         
 @dataclass
 class CountResultOutputPipelineBean:
     screen_id: str
     count_result_fn: str
```

### Comparing `crispr_millipede_helper-0.1.5/crispr_millipede_helper/pipeline/InitialFile.py` & `crispr_millipede_helper-0.1.6/crispr_millipede_helper/pipeline/InitialFile.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,22 +47,22 @@
     output_screen_supplementaryFiles_map_processed = process_pipeline_element(output_screen_supplementaryFiles_map)
     
     total_count_result: int = len(output_screen_countResults_map_processed[screen_id])
     
     sample_result_model_list: List[SampleResultModel] = []
     for index in range(0, total_count_result):
         index_pair_pipeline_bean = IndexPairPipelineBean(
-                barcode_index =  output_screen_countResults_map_processed[screen_id][index][0][0]["barcodeIndex"],
-                i5_index =  output_screen_countResults_map_processed[screen_id][index][0][0]["i5Index"],
+                index1 =  output_screen_countResults_map_processed[screen_id][index][0][0]["index1"],
+                index2 =  output_screen_countResults_map_processed[screen_id][index][0][0]["index2"],
                 read1_fn =  output_screen_countResults_map_processed[screen_id][index][0][0]["read1"],
                 read2_fn =  output_screen_countResults_map_processed[screen_id][index][0][0]["read2"]
             )
         
         sample_annotation_pipeline_bean = SampleAnnotationPipelineBean(
-            sample_annotations_series = pd.Series(input_i5ToBarcodeToSampleInfoVarsMap_processed[index_pair_pipeline_bean.i5_index][index_pair_pipeline_bean.barcode_index], index=input_sampleInfoVarnames_processed)
+            sample_annotations_series = pd.Series(input_i5ToBarcodeToSampleInfoVarsMap_processed[index_pair_pipeline_bean.index1][index_pair_pipeline_bean.index2], index=input_sampleInfoVarnames_processed)
         )
         
         count_result_output_pipeline_bean = None
         if (output_screen_countResults_map is not None) and (output_screen_editingEfficiencies_map is not None) and (output_screen_supplementaryFiles_map is not None):
             count_result_output_pipeline_bean = CountResultOutputPipelineBean(
                 count_result_fn =  output_screen_countResults_map_processed[screen_id][index][1],
                 screen_id = output_screen_countResults_map_processed[screen_id][index][0][0]["screenId"],
@@ -107,22 +107,22 @@
     output_screenIdToSampleMap_processed = process_pipeline_element(output_screenIdToSampleMap)
     
     total_count_result: int = len(output_screenIdToSampleMap_processed[screen_id])
     
     sample_result_model_list: List[SampleResultModel] = []
     for index in range(0, total_count_result):
         index_pair_pipeline_bean = IndexPairPipelineBean(
-                barcode_index =  output_screenIdToSampleMap_processed[screen_id][index][0]["barcodeIndex"],
-                i5_index =  output_screenIdToSampleMap_processed[screen_id][index][0]["i5Index"],
+                index1 =  output_screenIdToSampleMap_processed[screen_id][index][0]["index1"],
+                index2 =  output_screenIdToSampleMap_processed[screen_id][index][0]["index2"],
                 read1_fn =  output_screenIdToSampleMap_processed[screen_id][index][0]["read1"],
                 read2_fn =  output_screenIdToSampleMap_processed[screen_id][index][0]["read2"]
             )
         
         sample_annotation_pipeline_bean = SampleAnnotationPipelineBean(
-            sample_annotations_series = pd.Series(input_i5ToBarcodeToSampleInfoVarsMap_processed[index_pair_pipeline_bean.i5_index][index_pair_pipeline_bean.barcode_index], index=input_sampleInfoVarnames_processed)
+            sample_annotations_series = pd.Series(input_i5ToBarcodeToSampleInfoVarsMap_processed[index_pair_pipeline_bean.index1][index_pair_pipeline_bean.index2], index=input_sampleInfoVarnames_processed)
         )
         
         sample_result_model = SampleResultModel(
             index_pair_pipeline_bean = index_pair_pipeline_bean,
             sample_annotation_pipeline_bean = sample_annotation_pipeline_bean
         )
```

### Comparing `crispr_millipede_helper-0.1.5/PKG-INFO` & `crispr_millipede_helper-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crispr-millipede-helper
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 Author: Basheer Becerra
 Author-email: bbecerr@outlook.com
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

