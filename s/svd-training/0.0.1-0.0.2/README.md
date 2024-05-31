# Comparing `tmp/svd_training-0.0.1-py3-none-any.whl.zip` & `tmp/svd_training-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 8447 bytes, number of entries: 14
+Zip file size: 8492 bytes, number of entries: 14
 -rw-r--r--  2.0 unx        2 b- defN 24-May-19 12:11 svd_training/__init__.py
 -rw-r--r--  2.0 unx      442 b- defN 24-May-19 12:18 svd_training/model_keys.py
 -rw-r--r--  2.0 unx     1667 b- defN 24-Apr-26 09:08 svd_training/svd_linear.py
 -rw-r--r--  2.0 unx     1752 b- defN 24-May-03 08:01 svd_training/svd_llama3_model.py
 -rw-r--r--  2.0 unx     3498 b- defN 24-Apr-26 09:50 svd_training/svd_mistral-v0.1_model.py
 -rw-r--r--  2.0 unx     3498 b- defN 24-Apr-26 09:50 svd_training/svd_mistralv01_model.py
--rw-r--r--  2.0 unx     1817 b- defN 24-May-19 12:45 svd_training/svd_model.py
+-rw-r--r--  2.0 unx     1970 b- defN 24-May-31 10:44 svd_training/svd_model.py
 -rw-r--r--  2.0 unx     3501 b- defN 24-Apr-26 09:53 svd_training/svd_phi3-mini_model.py
 -rw-r--r--  2.0 unx     3480 b- defN 24-Apr-26 17:20 svd_training/svd_phi3mini_model.py
--rw-r--r--  2.0 unx       76 b- defN 24-Apr-05 08:23 svd_training/variables.py
--rw-r--r--  2.0 unx     1079 b- defN 24-May-19 12:52 svd_training-0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-19 12:52 svd_training-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 24-May-19 12:52 svd_training-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1183 b- defN 24-May-19 12:52 svd_training-0.0.1.dist-info/RECORD
-14 files, 22100 bytes uncompressed, 6463 bytes compressed:  70.8%
+-rw-r--r--  2.0 unx       76 b- defN 24-May-31 10:45 svd_training/variables.py
+-rw-r--r--  2.0 unx     1079 b- defN 24-May-31 11:12 svd_training-0.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-31 11:12 svd_training-0.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 24-May-31 11:12 svd_training-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1183 b- defN 24-May-31 11:12 svd_training-0.0.2.dist-info/RECORD
+14 files, 22253 bytes uncompressed, 6508 bytes compressed:  70.8%
```

## zipnote {}

```diff
@@ -24,20 +24,20 @@
 
 Filename: svd_training/svd_phi3mini_model.py
 Comment: 
 
 Filename: svd_training/variables.py
 Comment: 
 
-Filename: svd_training-0.0.1.dist-info/METADATA
+Filename: svd_training-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: svd_training-0.0.1.dist-info/WHEEL
+Filename: svd_training-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: svd_training-0.0.1.dist-info/top_level.txt
+Filename: svd_training-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: svd_training-0.0.1.dist-info/RECORD
+Filename: svd_training-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## svd_training/svd_model.py

```diff
@@ -7,33 +7,37 @@
 _logger = logging.getLogger(__name__)
 logging.basicConfig(level=logging.INFO)
 
 
 class SVDForCausalLM(PreTrainedModel):
     def merge(self):
         for layer_index in range(len(self.model.layers)):
-            for mlp_name in get_mlp_names():
+            for mlp_name in self._target_modules:
                 try:
                     exec(
                         f"self.model.layers[layer_index].{mlp_name} = self.model.layers[layer_index].{mlp_name}.get_merged_linear()"
                     )
                 except AttributeError:
                     continue
 
         self.lm_head = self.lm_head.get_merged_linear()
 
     @staticmethod
-    def create_from_model(model, rank_fraction):
+    def create_from_model(model, rank_fraction, target_modules=None):
+        if target_modules is None:
+            target_modules = get_mlp_names()
+        model._target_modules = target_modules
+
         _logger.info(f"Building SVD model with rank_fraction={rank_fraction}")
         _logger.info(f"lm_head is substituted with rank_fraction={rank_fraction}")
         model.lm_head = SVDLinear.create_from_weight(
             model.lm_head.weight, rank_fraction
         )
         for layer_index in range(len(model.base_model.layers)):
-            for mlp_name in get_mlp_names():
+            for mlp_name in target_modules:
                 try:
                     exec(f"weight = model.model.layers[layer_index].{mlp_name}.weight")
                     exec(
                         f"model.model.layers[layer_index].{mlp_name} = SVDLinear.create_from_weight(weight, rank_fraction)"
                     )
                 except AttributeError:
                     continue
```

## svd_training/variables.py

```diff
@@ -1,4 +1,4 @@
 def get_variables() -> dict:
     return {
-        "version": "0.0.1",
+        "version": "0.0.2",
     }
```

## Comparing `svd_training-0.0.1.dist-info/METADATA` & `svd_training-0.0.2.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: svd-training
-Version: 0.0.1
+Version: 0.0.2
 Summary: A training helper for LLM.
 Home-page: http://github.com/fractalego/svd-training
 Author: Alberto Cetoli
 Author-email: alberto@fractalego.io
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 Requires-Dist: transformers (==4.41.0)
```

## Comparing `svd_training-0.0.1.dist-info/RECORD` & `svd_training-0.0.2.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 svd_training/__init__.py,sha256=daEdpEyAJIa8b2VkCqSKcw8PaExcB6Qro80XNes_sHA,2
 svd_training/model_keys.py,sha256=lsMNqafqY6IEixaMuJWanw6XGZEQ8q1OORr_q31JSBs,442
 svd_training/svd_linear.py,sha256=D-WIOxEdg32PvnaknaxLkyrlNO5hLeoBSj74PP3GKpQ,1667
 svd_training/svd_llama3_model.py,sha256=9NHHMI2y89f5298dK3ZXlY73AaTSfpPAVgZkwmR5Te0,1752
 svd_training/svd_mistral-v0.1_model.py,sha256=s0x5iWLV7FgJeyhNf3tTQuCQv4yhbXBROw29BcudKKg,3498
 svd_training/svd_mistralv01_model.py,sha256=s0x5iWLV7FgJeyhNf3tTQuCQv4yhbXBROw29BcudKKg,3498
-svd_training/svd_model.py,sha256=WXRPf5-Z4y3dOoZLv9EsROiRVdBAvSKmZmDS4oPzGhs,1817
+svd_training/svd_model.py,sha256=zSIY10J5ejzOby6fYzdP4hWveK7ks7rpxtqaeo0_De0,1970
 svd_training/svd_phi3-mini_model.py,sha256=fO6tV_cdyt47f95jVumLrjMCPFLKUPuM9wYEVwhV8C4,3501
 svd_training/svd_phi3mini_model.py,sha256=GH5rHU5dSzM9TaLQkKwuiR073KW5vGR1-JENgAG_ErE,3480
-svd_training/variables.py,sha256=S8gVsbBNKgOG7B--6ooLVdyhX5zpiQq0Z_H-uOHA5cM,76
-svd_training-0.0.1.dist-info/METADATA,sha256=RYGTLno-J98sc0RnGoCeMgDxIdqK0dZzUY0dOgqlR-E,1079
-svd_training-0.0.1.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
-svd_training-0.0.1.dist-info/top_level.txt,sha256=QSEf2CY_soVadOl29kZcA3tEF-wxRo7ZlJxha1zU3C8,13
-svd_training-0.0.1.dist-info/RECORD,,
+svd_training/variables.py,sha256=L651AUgVym3M7JE3ymrvSt_eV0j8C9qbMIP4WHlUqcI,76
+svd_training-0.0.2.dist-info/METADATA,sha256=qEtacZg-5G9NlzZYAGrt-j18Yj4Zw3SkjDJqR6qqON0,1079
+svd_training-0.0.2.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+svd_training-0.0.2.dist-info/top_level.txt,sha256=QSEf2CY_soVadOl29kZcA3tEF-wxRo7ZlJxha1zU3C8,13
+svd_training-0.0.2.dist-info/RECORD,,
```

