# Comparing `tmp/lit_ecology_classifier-0.3.4-py3-none-any.whl.zip` & `tmp/lit_ecology_classifier-0.3.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,23 +1,23 @@
-Zip file size: 24856 bytes, number of entries: 21
+Zip file size: 24847 bytes, number of entries: 21
 -rw-r--r--  2.0 unx        0 b- defN 24-May-28 11:43 lit_ecology_classifier/__init__.py
 -rw-r--r--  2.0 unx     3469 b- defN 24-May-29 08:00 lit_ecology_classifier/main.py
 -rw-r--r--  2.0 unx     1789 b- defN 24-May-31 13:46 lit_ecology_classifier/predict.py
 -rw-r--r--  2.0 unx     2327 b- defN 24-May-30 14:25 lit_ecology_classifier/test.py
 -rw-r--r--  2.0 unx        0 b- defN 24-May-28 11:43 lit_ecology_classifier/data/__init__.py
--rw-r--r--  2.0 unx     8159 b- defN 24-May-31 13:49 lit_ecology_classifier/data/datamodule.py
+-rw-r--r--  2.0 unx     8156 b- defN 24-May-31 13:51 lit_ecology_classifier/data/datamodule.py
 -rw-r--r--  2.0 unx     7710 b- defN 24-May-31 08:50 lit_ecology_classifier/data/imagedataset.py
 -rw-r--r--  2.0 unx     8016 b- defN 24-May-31 08:33 lit_ecology_classifier/data/tardataset.py
 -rw-r--r--  2.0 unx        0 b- defN 24-May-28 11:43 lit_ecology_classifier/helpers/__init__.py
 -rw-r--r--  2.0 unx     2827 b- defN 24-May-31 13:43 lit_ecology_classifier/helpers/argparser.py
 -rw-r--r--  2.0 unx     1145 b- defN 24-May-28 11:43 lit_ecology_classifier/helpers/calc_class_weights.py
 -rw-r--r--  2.0 unx    11114 b- defN 24-May-31 13:43 lit_ecology_classifier/helpers/helpers.py
 -rw-r--r--  2.0 unx        0 b- defN 24-May-28 11:43 lit_ecology_classifier/models/__init__.py
 -rw-r--r--  2.0 unx    11575 b- defN 24-May-31 08:24 lit_ecology_classifier/models/model.py
 -rw-r--r--  2.0 unx     2665 b- defN 24-May-31 09:28 lit_ecology_classifier/models/setup_model.py
--rw-r--r--  2.0 unx     1068 b- defN 24-May-31 13:49 lit_ecology_classifier-0.3.4.dist-info/LICENSE
--rw-r--r--  2.0 unx     3706 b- defN 24-May-31 13:49 lit_ecology_classifier-0.3.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-31 13:49 lit_ecology_classifier-0.3.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       76 b- defN 24-May-31 13:49 lit_ecology_classifier-0.3.4.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       23 b- defN 24-May-31 13:49 lit_ecology_classifier-0.3.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     2008 b- defN 24-May-31 13:49 lit_ecology_classifier-0.3.4.dist-info/RECORD
-21 files, 67769 bytes uncompressed, 21476 bytes compressed:  68.3%
+-rw-r--r--  2.0 unx     1068 b- defN 24-May-31 13:51 lit_ecology_classifier-0.3.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3706 b- defN 24-May-31 13:51 lit_ecology_classifier-0.3.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-31 13:51 lit_ecology_classifier-0.3.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       76 b- defN 24-May-31 13:51 lit_ecology_classifier-0.3.5.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       23 b- defN 24-May-31 13:51 lit_ecology_classifier-0.3.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2008 b- defN 24-May-31 13:51 lit_ecology_classifier-0.3.5.dist-info/RECORD
+21 files, 67766 bytes uncompressed, 21467 bytes compressed:  68.3%
```

## zipnote {}

```diff
@@ -39,26 +39,26 @@
 
 Filename: lit_ecology_classifier/models/model.py
 Comment: 
 
 Filename: lit_ecology_classifier/models/setup_model.py
 Comment: 
 
-Filename: lit_ecology_classifier-0.3.4.dist-info/LICENSE
+Filename: lit_ecology_classifier-0.3.5.dist-info/LICENSE
 Comment: 
 
-Filename: lit_ecology_classifier-0.3.4.dist-info/METADATA
+Filename: lit_ecology_classifier-0.3.5.dist-info/METADATA
 Comment: 
 
-Filename: lit_ecology_classifier-0.3.4.dist-info/WHEEL
+Filename: lit_ecology_classifier-0.3.5.dist-info/WHEEL
 Comment: 
 
-Filename: lit_ecology_classifier-0.3.4.dist-info/entry_points.txt
+Filename: lit_ecology_classifier-0.3.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: lit_ecology_classifier-0.3.4.dist-info/top_level.txt
+Filename: lit_ecology_classifier-0.3.5.dist-info/top_level.txt
 Comment: 
 
-Filename: lit_ecology_classifier-0.3.4.dist-info/RECORD
+Filename: lit_ecology_classifier-0.3.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## lit_ecology_classifier/data/datamodule.py

```diff
@@ -165,15 +165,15 @@
         """
 
         if self.TTA:
             loader = DataLoader(
                 self.predict_dataset,
                 batch_size=self.batch_size,
                 shuffle=False,
-                sampler=sampler,
+                sampler=None,
                 num_workers= 4,
                 pin_memory=False,
                 drop_last=False,
                 collate_fn=TTA_collate_fn,
             )
         else:
             loader = DataLoader(
```

## Comparing `lit_ecology_classifier-0.3.4.dist-info/LICENSE` & `lit_ecology_classifier-0.3.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `lit_ecology_classifier-0.3.4.dist-info/METADATA` & `lit_ecology_classifier-0.3.5.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lit_ecology_classifier
-Version: 0.3.4
+Version: 0.3.5
 Summary: Image Classifier optimised for ecology use-cases
 Home-page: https://github.com/kaechb/lit_ecology_classifier
 Author: Benno Kaech
 Author-email: your.email@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `lit_ecology_classifier-0.3.4.dist-info/RECORD` & `lit_ecology_classifier-0.3.5.dist-info/RECORD`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 lit_ecology_classifier/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 lit_ecology_classifier/main.py,sha256=oye_MqYi8_Pnlq4E3Dy65VtXPW7JyBxecJW9cHEM6rw,3469
 lit_ecology_classifier/predict.py,sha256=SZJeR842g3JrOgiIrNdxcCcM75HJncSHMe4qYq2mGxc,1789
 lit_ecology_classifier/test.py,sha256=NCm4SGXD8Aa4ckt3bXqskH6XtDNSV2KPZ6BO938Oo0Q,2327
 lit_ecology_classifier/data/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-lit_ecology_classifier/data/datamodule.py,sha256=Iuy_zmnaEUmPlizOJMxccf_lwce1fCkZeC_21lndWaI,8159
+lit_ecology_classifier/data/datamodule.py,sha256=3VVC8TJGrT9IeZeK5rg0uIgHSBLOO2qSxpLN4O628fI,8156
 lit_ecology_classifier/data/imagedataset.py,sha256=YblIo-n5LaVBzYuMu07b11Xy_fod_oZTnwGqLoYL4hs,7710
 lit_ecology_classifier/data/tardataset.py,sha256=HDxnCiJHuKUtgLJJslulhjXsC2KGnp8s_FUiQXbtXNI,8016
 lit_ecology_classifier/helpers/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 lit_ecology_classifier/helpers/argparser.py,sha256=JjWiA1cdqjOXVdx-WNUzGSJ0W8FEAIUZq3wk4dMalqI,2827
 lit_ecology_classifier/helpers/calc_class_weights.py,sha256=fMzuX0jeRNXScX9IO8veOgKsxAnWI3VfjwDwAFOO6A4,1145
 lit_ecology_classifier/helpers/helpers.py,sha256=bLjmrBrAr1wu90_cOqn-a_4oCuu3LRiFUafyfzFbb1k,11114
 lit_ecology_classifier/models/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 lit_ecology_classifier/models/model.py,sha256=HX2sC5ZEZNK2yf-bQNPj-FZGCNZaoKfDz1WOxNf-Cj4,11575
 lit_ecology_classifier/models/setup_model.py,sha256=sVULgitlYHlaVPNu3-IIMb_V5ZbA1-Vt3YPZ390ZmTs,2665
-lit_ecology_classifier-0.3.4.dist-info/LICENSE,sha256=otRPec6AwxKerM0zN-WiG66AnplxnmpbPaDyJd_QxE0,1068
-lit_ecology_classifier-0.3.4.dist-info/METADATA,sha256=OTfeD4WlWyUcwBbtW-ebWxJsBrQ3HWaTNlhPJxOLof8,3706
-lit_ecology_classifier-0.3.4.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-lit_ecology_classifier-0.3.4.dist-info/entry_points.txt,sha256=v3ZJ9RRS0_MjXgy4y3gPb2R7ANPKKyPQrRlEO384ITQ,76
-lit_ecology_classifier-0.3.4.dist-info/top_level.txt,sha256=PKi3Fm6NgOu2ej8D7-MCov1FmFYRFdfaTOAxYhDYJnw,23
-lit_ecology_classifier-0.3.4.dist-info/RECORD,,
+lit_ecology_classifier-0.3.5.dist-info/LICENSE,sha256=otRPec6AwxKerM0zN-WiG66AnplxnmpbPaDyJd_QxE0,1068
+lit_ecology_classifier-0.3.5.dist-info/METADATA,sha256=5TKnvizl-sqUzHt4lWf7UuDq6j3bjF8Rah60BJaiGL4,3706
+lit_ecology_classifier-0.3.5.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+lit_ecology_classifier-0.3.5.dist-info/entry_points.txt,sha256=v3ZJ9RRS0_MjXgy4y3gPb2R7ANPKKyPQrRlEO384ITQ,76
+lit_ecology_classifier-0.3.5.dist-info/top_level.txt,sha256=PKi3Fm6NgOu2ej8D7-MCov1FmFYRFdfaTOAxYhDYJnw,23
+lit_ecology_classifier-0.3.5.dist-info/RECORD,,
```
