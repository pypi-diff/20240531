# Comparing `tmp/lit_ecology_classifier-0.2.9-py3-none-any.whl.zip` & `tmp/lit_ecology_classifier-0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,23 +1,23 @@
-Zip file size: 24899 bytes, number of entries: 21
+Zip file size: 24871 bytes, number of entries: 21
 -rw-r--r--  2.0 unx        0 b- defN 24-May-28 11:43 lit_ecology_classifier/__init__.py
 -rw-r--r--  2.0 unx     3469 b- defN 24-May-29 08:00 lit_ecology_classifier/main.py
 -rw-r--r--  2.0 unx     1865 b- defN 24-May-31 13:26 lit_ecology_classifier/predict.py
 -rw-r--r--  2.0 unx     2327 b- defN 24-May-30 14:25 lit_ecology_classifier/test.py
 -rw-r--r--  2.0 unx        0 b- defN 24-May-28 11:43 lit_ecology_classifier/data/__init__.py
 -rw-r--r--  2.0 unx     8697 b- defN 24-May-31 08:46 lit_ecology_classifier/data/datamodule.py
 -rw-r--r--  2.0 unx     7710 b- defN 24-May-31 08:50 lit_ecology_classifier/data/imagedataset.py
 -rw-r--r--  2.0 unx     8016 b- defN 24-May-31 08:33 lit_ecology_classifier/data/tardataset.py
 -rw-r--r--  2.0 unx        0 b- defN 24-May-28 11:43 lit_ecology_classifier/helpers/__init__.py
--rw-r--r--  2.0 unx     2726 b- defN 24-May-31 13:26 lit_ecology_classifier/helpers/argparser.py
+-rw-r--r--  2.0 unx     2735 b- defN 24-May-31 13:30 lit_ecology_classifier/helpers/argparser.py
 -rw-r--r--  2.0 unx     1145 b- defN 24-May-28 11:43 lit_ecology_classifier/helpers/calc_class_weights.py
 -rw-r--r--  2.0 unx    11113 b- defN 24-May-31 08:52 lit_ecology_classifier/helpers/helpers.py
 -rw-r--r--  2.0 unx        0 b- defN 24-May-28 11:43 lit_ecology_classifier/models/__init__.py
 -rw-r--r--  2.0 unx    11575 b- defN 24-May-31 08:24 lit_ecology_classifier/models/model.py
 -rw-r--r--  2.0 unx     2665 b- defN 24-May-31 09:28 lit_ecology_classifier/models/setup_model.py
--rw-r--r--  2.0 unx     1068 b- defN 24-May-31 13:27 lit_ecology_classifier-0.2.9.dist-info/LICENSE
--rw-r--r--  2.0 unx     3706 b- defN 24-May-31 13:27 lit_ecology_classifier-0.2.9.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-31 13:27 lit_ecology_classifier-0.2.9.dist-info/WHEEL
--rw-r--r--  2.0 unx       76 b- defN 24-May-31 13:27 lit_ecology_classifier-0.2.9.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       23 b- defN 24-May-31 13:27 lit_ecology_classifier-0.2.9.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     2008 b- defN 24-May-31 13:27 lit_ecology_classifier-0.2.9.dist-info/RECORD
-21 files, 68281 bytes uncompressed, 21519 bytes compressed:  68.5%
+-rw-r--r--  2.0 unx     1068 b- defN 24-May-31 13:30 lit_ecology_classifier-0.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3704 b- defN 24-May-31 13:30 lit_ecology_classifier-0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-31 13:30 lit_ecology_classifier-0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       76 b- defN 24-May-31 13:30 lit_ecology_classifier-0.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       23 b- defN 24-May-31 13:30 lit_ecology_classifier-0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1996 b- defN 24-May-31 13:30 lit_ecology_classifier-0.3.dist-info/RECORD
+21 files, 68276 bytes uncompressed, 21515 bytes compressed:  68.5%
```

## zipnote {}

```diff
@@ -39,26 +39,26 @@
 
 Filename: lit_ecology_classifier/models/model.py
 Comment: 
 
 Filename: lit_ecology_classifier/models/setup_model.py
 Comment: 
 
-Filename: lit_ecology_classifier-0.2.9.dist-info/LICENSE
+Filename: lit_ecology_classifier-0.3.dist-info/LICENSE
 Comment: 
 
-Filename: lit_ecology_classifier-0.2.9.dist-info/METADATA
+Filename: lit_ecology_classifier-0.3.dist-info/METADATA
 Comment: 
 
-Filename: lit_ecology_classifier-0.2.9.dist-info/WHEEL
+Filename: lit_ecology_classifier-0.3.dist-info/WHEEL
 Comment: 
 
-Filename: lit_ecology_classifier-0.2.9.dist-info/entry_points.txt
+Filename: lit_ecology_classifier-0.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: lit_ecology_classifier-0.2.9.dist-info/top_level.txt
+Filename: lit_ecology_classifier-0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: lit_ecology_classifier-0.2.9.dist-info/RECORD
+Filename: lit_ecology_classifier-0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## lit_ecology_classifier/helpers/argparser.py

```diff
@@ -23,15 +23,15 @@
 
     # Augmentation and training/testing specifics
     parser.add_argument("--testing", action="store_true", help="Set this to True if in testing mode, False for training")
     return parser
 
 def inference_argparser():
     parser = argparse.ArgumentParser(description="Use Classifier on unlabelled data.")
-    parser.add_argument("--batch_size", default=32, help="Batch  Size")
+    parser.add_argument("--batch_size", type=int, default=32, help="Batch Size")
     parser.add_argument("--outpath", default="./preds/", help="Directory where you want to save the predictions")
     parser.add_argument("--model_path", default="./checkpoints/model.ckpt", help="Path to the model file")
     parser.add_argument("--datapath",  default="/store/empa/em09/aquascope/phyto.tar", help="Path to the folder containing the data to classify as Tar file")
     parser.add_argument("--no_gpu", action="store_true", help="Use no GPU for training, default is False")
     parser.add_argument("--no_TTA", action="store_true", help="Disable test-time augmentation")
 
     return parser
```

## Comparing `lit_ecology_classifier-0.2.9.dist-info/LICENSE` & `lit_ecology_classifier-0.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `lit_ecology_classifier-0.2.9.dist-info/METADATA` & `lit_ecology_classifier-0.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lit_ecology_classifier
-Version: 0.2.9
+Version: 0.3
 Summary: Image Classifier optimised for ecology use-cases
 Home-page: https://github.com/kaechb/lit_ecology_classifier
 Author: Benno Kaech
 Author-email: your.email@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `lit_ecology_classifier-0.2.9.dist-info/RECORD` & `lit_ecology_classifier-0.3.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 lit_ecology_classifier/predict.py,sha256=RaRJMJjo3Sdm8bZ-Dma1rfFi9fFlnG0J2PA8x6OPClA,1865
 lit_ecology_classifier/test.py,sha256=NCm4SGXD8Aa4ckt3bXqskH6XtDNSV2KPZ6BO938Oo0Q,2327
 lit_ecology_classifier/data/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 lit_ecology_classifier/data/datamodule.py,sha256=JG60qcQkT2BBh2EzpwMKz-7i7rQA5jAGBQg_IME-HuE,8697
 lit_ecology_classifier/data/imagedataset.py,sha256=YblIo-n5LaVBzYuMu07b11Xy_fod_oZTnwGqLoYL4hs,7710
 lit_ecology_classifier/data/tardataset.py,sha256=HDxnCiJHuKUtgLJJslulhjXsC2KGnp8s_FUiQXbtXNI,8016
 lit_ecology_classifier/helpers/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-lit_ecology_classifier/helpers/argparser.py,sha256=mte6H_3bK1J7tH8VROmUc3foMHLkpmWCxu0GwZ0YhTY,2726
+lit_ecology_classifier/helpers/argparser.py,sha256=iU1sC3djKn4zwr19oPA8XIl9t2VUL6i1ILM7If2ZtG0,2735
 lit_ecology_classifier/helpers/calc_class_weights.py,sha256=fMzuX0jeRNXScX9IO8veOgKsxAnWI3VfjwDwAFOO6A4,1145
 lit_ecology_classifier/helpers/helpers.py,sha256=NM1c7rYsY0BGcyghoJvGOWfnrpt7OrkNEtlJfjuA310,11113
 lit_ecology_classifier/models/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 lit_ecology_classifier/models/model.py,sha256=HX2sC5ZEZNK2yf-bQNPj-FZGCNZaoKfDz1WOxNf-Cj4,11575
 lit_ecology_classifier/models/setup_model.py,sha256=sVULgitlYHlaVPNu3-IIMb_V5ZbA1-Vt3YPZ390ZmTs,2665
-lit_ecology_classifier-0.2.9.dist-info/LICENSE,sha256=otRPec6AwxKerM0zN-WiG66AnplxnmpbPaDyJd_QxE0,1068
-lit_ecology_classifier-0.2.9.dist-info/METADATA,sha256=tJBaQpTKdpdAHi0PNOzkIKkVupcpD7JLqAsOhyrCDwQ,3706
-lit_ecology_classifier-0.2.9.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-lit_ecology_classifier-0.2.9.dist-info/entry_points.txt,sha256=v3ZJ9RRS0_MjXgy4y3gPb2R7ANPKKyPQrRlEO384ITQ,76
-lit_ecology_classifier-0.2.9.dist-info/top_level.txt,sha256=PKi3Fm6NgOu2ej8D7-MCov1FmFYRFdfaTOAxYhDYJnw,23
-lit_ecology_classifier-0.2.9.dist-info/RECORD,,
+lit_ecology_classifier-0.3.dist-info/LICENSE,sha256=otRPec6AwxKerM0zN-WiG66AnplxnmpbPaDyJd_QxE0,1068
+lit_ecology_classifier-0.3.dist-info/METADATA,sha256=rC8t34oMkDNqrZXU4__vVPTwH4OQkSMpLkGGolskuco,3704
+lit_ecology_classifier-0.3.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+lit_ecology_classifier-0.3.dist-info/entry_points.txt,sha256=v3ZJ9RRS0_MjXgy4y3gPb2R7ANPKKyPQrRlEO384ITQ,76
+lit_ecology_classifier-0.3.dist-info/top_level.txt,sha256=PKi3Fm6NgOu2ej8D7-MCov1FmFYRFdfaTOAxYhDYJnw,23
+lit_ecology_classifier-0.3.dist-info/RECORD,,
```
