# Comparing `tmp/lit_ecology_classifier-0.3-py3-none-any.whl.zip` & `tmp/lit_ecology_classifier-0.3.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,23 +1,23 @@
-Zip file size: 24871 bytes, number of entries: 21
+Zip file size: 24963 bytes, number of entries: 21
 -rw-r--r--  2.0 unx        0 b- defN 24-May-28 11:43 lit_ecology_classifier/__init__.py
 -rw-r--r--  2.0 unx     3469 b- defN 24-May-29 08:00 lit_ecology_classifier/main.py
--rw-r--r--  2.0 unx     1865 b- defN 24-May-31 13:26 lit_ecology_classifier/predict.py
+-rw-r--r--  2.0 unx     2016 b- defN 24-May-31 13:38 lit_ecology_classifier/predict.py
 -rw-r--r--  2.0 unx     2327 b- defN 24-May-30 14:25 lit_ecology_classifier/test.py
 -rw-r--r--  2.0 unx        0 b- defN 24-May-28 11:43 lit_ecology_classifier/data/__init__.py
 -rw-r--r--  2.0 unx     8697 b- defN 24-May-31 08:46 lit_ecology_classifier/data/datamodule.py
 -rw-r--r--  2.0 unx     7710 b- defN 24-May-31 08:50 lit_ecology_classifier/data/imagedataset.py
 -rw-r--r--  2.0 unx     8016 b- defN 24-May-31 08:33 lit_ecology_classifier/data/tardataset.py
 -rw-r--r--  2.0 unx        0 b- defN 24-May-28 11:43 lit_ecology_classifier/helpers/__init__.py
 -rw-r--r--  2.0 unx     2735 b- defN 24-May-31 13:30 lit_ecology_classifier/helpers/argparser.py
 -rw-r--r--  2.0 unx     1145 b- defN 24-May-28 11:43 lit_ecology_classifier/helpers/calc_class_weights.py
--rw-r--r--  2.0 unx    11113 b- defN 24-May-31 08:52 lit_ecology_classifier/helpers/helpers.py
+-rw-r--r--  2.0 unx    11113 b- defN 24-May-31 13:35 lit_ecology_classifier/helpers/helpers.py
 -rw-r--r--  2.0 unx        0 b- defN 24-May-28 11:43 lit_ecology_classifier/models/__init__.py
 -rw-r--r--  2.0 unx    11575 b- defN 24-May-31 08:24 lit_ecology_classifier/models/model.py
 -rw-r--r--  2.0 unx     2665 b- defN 24-May-31 09:28 lit_ecology_classifier/models/setup_model.py
--rw-r--r--  2.0 unx     1068 b- defN 24-May-31 13:30 lit_ecology_classifier-0.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     3704 b- defN 24-May-31 13:30 lit_ecology_classifier-0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-31 13:30 lit_ecology_classifier-0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       76 b- defN 24-May-31 13:30 lit_ecology_classifier-0.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       23 b- defN 24-May-31 13:30 lit_ecology_classifier-0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1996 b- defN 24-May-31 13:30 lit_ecology_classifier-0.3.dist-info/RECORD
-21 files, 68276 bytes uncompressed, 21515 bytes compressed:  68.5%
+-rw-r--r--  2.0 unx     1068 b- defN 24-May-31 13:38 lit_ecology_classifier-0.3.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3706 b- defN 24-May-31 13:38 lit_ecology_classifier-0.3.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-31 13:38 lit_ecology_classifier-0.3.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       76 b- defN 24-May-31 13:38 lit_ecology_classifier-0.3.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       23 b- defN 24-May-31 13:38 lit_ecology_classifier-0.3.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2008 b- defN 24-May-31 13:38 lit_ecology_classifier-0.3.1.dist-info/RECORD
+21 files, 68441 bytes uncompressed, 21583 bytes compressed:  68.5%
```

## zipnote {}

```diff
@@ -39,26 +39,26 @@
 
 Filename: lit_ecology_classifier/models/model.py
 Comment: 
 
 Filename: lit_ecology_classifier/models/setup_model.py
 Comment: 
 
-Filename: lit_ecology_classifier-0.3.dist-info/LICENSE
+Filename: lit_ecology_classifier-0.3.1.dist-info/LICENSE
 Comment: 
 
-Filename: lit_ecology_classifier-0.3.dist-info/METADATA
+Filename: lit_ecology_classifier-0.3.1.dist-info/METADATA
 Comment: 
 
-Filename: lit_ecology_classifier-0.3.dist-info/WHEEL
+Filename: lit_ecology_classifier-0.3.1.dist-info/WHEEL
 Comment: 
 
-Filename: lit_ecology_classifier-0.3.dist-info/entry_points.txt
+Filename: lit_ecology_classifier-0.3.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: lit_ecology_classifier-0.3.dist-info/top_level.txt
+Filename: lit_ecology_classifier-0.3.1.dist-info/top_level.txt
 Comment: 
 
-Filename: lit_ecology_classifier-0.3.dist-info/RECORD
+Filename: lit_ecology_classifier-0.3.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## lit_ecology_classifier/predict.py

```diff
@@ -30,15 +30,20 @@
 
     # Parse Arguments for prediction
     parser = inference_argparser()
     args = parser.parse_args()
 
     # Create Output Directory if it doesn't exist
     pathlib.Path(args.outpath).mkdir(parents=True, exist_ok=True)
+    try:
 
+        os.remove(os.join(args.outpath,"predictions_lit_ecology_classifier.txt"))
+    except:
+        print("outfile not found")
+        pass
     # Initialize the Model
     model = LitClassifier.load_from_checkpoint(args.model_path)
 
     # Initialize the Data Module
     hparams = model.hparams # copy the hyperparameters from the model
     model.hparams.batch_size = args.batch_size
     model.hparams.TTA = not args.no_TTA # set the TTA flag based on the argument
```

## lit_ecology_classifier/helpers/helpers.py

```diff
@@ -21,15 +21,15 @@
         labels (list): List of predicted labels.
     """
 
     labels = labels.tolist()
     base_filename = f"{outpath}/predictions_lit_ecology_classifier"
     file_path = f"{base_filename}.txt"
     lines = [f"\n{img}------------------ {label}/{score}" for img, label,score in zip(im_names, labels,scores)]
-    with open(file_path, "w") as f:
+    with open(file_path, "a") as f:
         f.writelines(lines)
 
 
 def gmean(input_x, dim):
     """
     Compute the geometric mean of the input tensor along the specified dimension.
```

## Comparing `lit_ecology_classifier-0.3.dist-info/LICENSE` & `lit_ecology_classifier-0.3.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `lit_ecology_classifier-0.3.dist-info/METADATA` & `lit_ecology_classifier-0.3.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lit_ecology_classifier
-Version: 0.3
+Version: 0.3.1
 Summary: Image Classifier optimised for ecology use-cases
 Home-page: https://github.com/kaechb/lit_ecology_classifier
 Author: Benno Kaech
 Author-email: your.email@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

