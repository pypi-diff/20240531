# Comparing `tmp/pathologyfoundation-0.2.5.tar.gz` & `tmp/pathologyfoundation-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pathologyfoundation-0.2.5.tar", last modified: Thu May  9 18:27:06 2024, max compression
+gzip compressed data, was "pathologyfoundation-0.2.6.tar", last modified: Fri May 31 19:46:32 2024, max compression
```

## Comparing `pathologyfoundation-0.2.5.tar` & `pathologyfoundation-0.2.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 zhihuang   (501) staff       (20)        0 2024-05-09 18:27:06.300938 pathologyfoundation-0.2.5/
--rw-r--r--   0 zhihuang   (501) staff       (20)     1048 2024-04-26 21:38:18.000000 pathologyfoundation-0.2.5/LICENSE
--rw-r--r--   0 zhihuang   (501) staff       (20)      542 2024-05-09 18:27:06.300172 pathologyfoundation-0.2.5/PKG-INFO
--rw-r--r--   0 zhihuang   (501) staff       (20)     2730 2024-04-26 21:38:18.000000 pathologyfoundation-0.2.5/README.md
-drwxr-xr-x   0 zhihuang   (501) staff       (20)        0 2024-05-09 18:27:06.283444 pathologyfoundation-0.2.5/pathologyfoundation/
--rw-r--r--   0 zhihuang   (501) staff       (20)      112 2024-04-26 21:38:18.000000 pathologyfoundation-0.2.5/pathologyfoundation/__init__.py
-drwxr-xr-x   0 zhihuang   (501) staff       (20)        0 2024-05-09 18:27:06.297665 pathologyfoundation-0.2.5/pathologyfoundation/dataset/
--rw-r--r--   0 zhihuang   (501) staff       (20)       25 2024-04-26 21:38:18.000000 pathologyfoundation-0.2.5/pathologyfoundation/dataset/__init__.py
--rw-r--r--   0 zhihuang   (501) staff       (20)     2813 2024-04-26 21:38:18.000000 pathologyfoundation-0.2.5/pathologyfoundation/dataset/load_data.py
--rw-r--r--   0 zhihuang   (501) staff       (20)      461 2024-04-26 22:13:48.000000 pathologyfoundation-0.2.5/pathologyfoundation/model_zoo.py
-drwxr-xr-x   0 zhihuang   (501) staff       (20)        0 2024-05-09 18:27:06.299280 pathologyfoundation-0.2.5/pathologyfoundation/models/
--rw-r--r--   0 zhihuang   (501) staff       (20)       64 2024-04-26 21:38:18.000000 pathologyfoundation-0.2.5/pathologyfoundation/models/__init__.py
--rw-r--r--   0 zhihuang   (501) staff       (20)    11198 2024-05-09 18:26:37.000000 pathologyfoundation-0.2.5/pathologyfoundation/models/finetuner.py
--rw-r--r--   0 zhihuang   (501) staff       (20)     6619 2024-04-26 21:38:18.000000 pathologyfoundation-0.2.5/pathologyfoundation/models/plip_vit.py
--rw-r--r--   0 zhihuang   (501) staff       (20)      700 2024-04-26 21:38:18.000000 pathologyfoundation-0.2.5/pathologyfoundation/utils.py
-drwxr-xr-x   0 zhihuang   (501) staff       (20)        0 2024-05-09 18:27:06.292713 pathologyfoundation-0.2.5/pathologyfoundation.egg-info/
--rw-r--r--   0 zhihuang   (501) staff       (20)      542 2024-05-09 18:27:06.000000 pathologyfoundation-0.2.5/pathologyfoundation.egg-info/PKG-INFO
--rw-r--r--   0 zhihuang   (501) staff       (20)      533 2024-05-09 18:27:06.000000 pathologyfoundation-0.2.5/pathologyfoundation.egg-info/SOURCES.txt
--rw-r--r--   0 zhihuang   (501) staff       (20)        1 2024-05-09 18:27:06.000000 pathologyfoundation-0.2.5/pathologyfoundation.egg-info/dependency_links.txt
--rw-r--r--   0 zhihuang   (501) staff       (20)       92 2024-05-09 18:27:06.000000 pathologyfoundation-0.2.5/pathologyfoundation.egg-info/requires.txt
--rw-r--r--   0 zhihuang   (501) staff       (20)       20 2024-05-09 18:27:06.000000 pathologyfoundation-0.2.5/pathologyfoundation.egg-info/top_level.txt
--rw-r--r--   0 zhihuang   (501) staff       (20)       38 2024-05-09 18:27:06.301006 pathologyfoundation-0.2.5/setup.cfg
--rw-r--r--   0 zhihuang   (501) staff       (20)      981 2024-05-09 18:26:15.000000 pathologyfoundation-0.2.5/setup.py
+drwxr-xr-x   0 zhihuang   (501) staff       (20)        0 2024-05-31 19:46:32.807780 pathologyfoundation-0.2.6/
+-rw-r--r--   0 zhihuang   (501) staff       (20)     1048 2024-04-26 21:38:18.000000 pathologyfoundation-0.2.6/LICENSE
+-rw-r--r--   0 zhihuang   (501) staff       (20)      542 2024-05-31 19:46:32.807496 pathologyfoundation-0.2.6/PKG-INFO
+-rw-r--r--   0 zhihuang   (501) staff       (20)     2730 2024-04-26 21:38:18.000000 pathologyfoundation-0.2.6/README.md
+drwxr-xr-x   0 zhihuang   (501) staff       (20)        0 2024-05-31 19:46:32.785071 pathologyfoundation-0.2.6/pathologyfoundation/
+-rw-r--r--   0 zhihuang   (501) staff       (20)      112 2024-04-26 21:38:18.000000 pathologyfoundation-0.2.6/pathologyfoundation/__init__.py
+drwxr-xr-x   0 zhihuang   (501) staff       (20)        0 2024-05-31 19:46:32.801922 pathologyfoundation-0.2.6/pathologyfoundation/dataset/
+-rw-r--r--   0 zhihuang   (501) staff       (20)       25 2024-04-26 21:38:18.000000 pathologyfoundation-0.2.6/pathologyfoundation/dataset/__init__.py
+-rw-r--r--   0 zhihuang   (501) staff       (20)     2813 2024-04-26 21:38:18.000000 pathologyfoundation-0.2.6/pathologyfoundation/dataset/load_data.py
+-rw-r--r--   0 zhihuang   (501) staff       (20)      461 2024-04-26 22:13:48.000000 pathologyfoundation-0.2.6/pathologyfoundation/model_zoo.py
+drwxr-xr-x   0 zhihuang   (501) staff       (20)        0 2024-05-31 19:46:32.806848 pathologyfoundation-0.2.6/pathologyfoundation/models/
+-rw-r--r--   0 zhihuang   (501) staff       (20)       64 2024-04-26 21:38:18.000000 pathologyfoundation-0.2.6/pathologyfoundation/models/__init__.py
+-rw-r--r--   0 zhihuang   (501) staff       (20)    11322 2024-05-31 19:46:17.000000 pathologyfoundation-0.2.6/pathologyfoundation/models/finetuner.py
+-rw-r--r--   0 zhihuang   (501) staff       (20)     6619 2024-04-26 21:38:18.000000 pathologyfoundation-0.2.6/pathologyfoundation/models/plip_vit.py
+-rw-r--r--   0 zhihuang   (501) staff       (20)      700 2024-04-26 21:38:18.000000 pathologyfoundation-0.2.6/pathologyfoundation/utils.py
+drwxr-xr-x   0 zhihuang   (501) staff       (20)        0 2024-05-31 19:46:32.799862 pathologyfoundation-0.2.6/pathologyfoundation.egg-info/
+-rw-r--r--   0 zhihuang   (501) staff       (20)      542 2024-05-31 19:46:32.000000 pathologyfoundation-0.2.6/pathologyfoundation.egg-info/PKG-INFO
+-rw-r--r--   0 zhihuang   (501) staff       (20)      533 2024-05-31 19:46:32.000000 pathologyfoundation-0.2.6/pathologyfoundation.egg-info/SOURCES.txt
+-rw-r--r--   0 zhihuang   (501) staff       (20)        1 2024-05-31 19:46:32.000000 pathologyfoundation-0.2.6/pathologyfoundation.egg-info/dependency_links.txt
+-rw-r--r--   0 zhihuang   (501) staff       (20)       92 2024-05-31 19:46:32.000000 pathologyfoundation-0.2.6/pathologyfoundation.egg-info/requires.txt
+-rw-r--r--   0 zhihuang   (501) staff       (20)       20 2024-05-31 19:46:32.000000 pathologyfoundation-0.2.6/pathologyfoundation.egg-info/top_level.txt
+-rw-r--r--   0 zhihuang   (501) staff       (20)       38 2024-05-31 19:46:32.807854 pathologyfoundation-0.2.6/setup.cfg
+-rw-r--r--   0 zhihuang   (501) staff       (20)      981 2024-05-31 01:10:08.000000 pathologyfoundation-0.2.6/setup.py
```

### Comparing `pathologyfoundation-0.2.5/LICENSE` & `pathologyfoundation-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pathologyfoundation-0.2.5/PKG-INFO` & `pathologyfoundation-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pathologyfoundation
-Version: 0.2.5
+Version: 0.2.6
 Summary: A package of pathology foundation models.
 Home-page: https://github.com/PathologyFoundation/pathologyfoundation
 Author: Zhi Huang
 Author-email: hz9423@gmail.com
 Keywords: Pathology,Foundation model,PLIP,OpenPath
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pathologyfoundation-0.2.5/README.md` & `pathologyfoundation-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `pathologyfoundation-0.2.5/pathologyfoundation/dataset/load_data.py` & `pathologyfoundation-0.2.6/pathologyfoundation/dataset/load_data.py`

 * *Files identical despite different names*

### Comparing `pathologyfoundation-0.2.5/pathologyfoundation/models/finetuner.py` & `pathologyfoundation-0.2.6/pathologyfoundation/models/finetuner.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,14 +198,18 @@
             y_true = np.array([])
             y_pred = np.array([])
             loss_log = AverageMeter()
             loss = 0
             tqdm_loader = tqdm(train_loader)
             for x, y in tqdm_loader:
                 tqdm_loader.set_description(f"Last Batch -- loss: {loss:.2f}")
+                if isinstance(x, list):
+                    x = torch.cat(x)
+                else:
+                    pass
                 x = torch.cat(x)
                 x = x.to(self.device)
                 y = y.reshape(-1).to(self.device)
                 self.model.train()
                 prediction, _ = self.model(x)
                 loss = self.loss_func(prediction, y)     # must be (1. nn output, 2. target)
                 proba = F.softmax(prediction, dim=1)
```

### Comparing `pathologyfoundation-0.2.5/pathologyfoundation/models/plip_vit.py` & `pathologyfoundation-0.2.6/pathologyfoundation/models/plip_vit.py`

 * *Files identical despite different names*

### Comparing `pathologyfoundation-0.2.5/pathologyfoundation/utils.py` & `pathologyfoundation-0.2.6/pathologyfoundation/utils.py`

 * *Files identical despite different names*

### Comparing `pathologyfoundation-0.2.5/pathologyfoundation.egg-info/PKG-INFO` & `pathologyfoundation-0.2.6/pathologyfoundation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pathologyfoundation
-Version: 0.2.5
+Version: 0.2.6
 Summary: A package of pathology foundation models.
 Home-page: https://github.com/PathologyFoundation/pathologyfoundation
 Author: Zhi Huang
 Author-email: hz9423@gmail.com
 Keywords: Pathology,Foundation model,PLIP,OpenPath
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pathologyfoundation-0.2.5/pathologyfoundation.egg-info/SOURCES.txt` & `pathologyfoundation-0.2.6/pathologyfoundation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pathologyfoundation-0.2.5/setup.py` & `pathologyfoundation-0.2.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         "appdirs",
         "pandas",
         "numpy",
         "tqdm",
         "gdown",
         "scikit-learn",
     ],
-    version = '0.2.5',  # Ideally should be same as the GitHub release tag varsion
+    version = '0.2.6',  # Ideally should be same as the GitHub release tag varsion
     description="A package of pathology foundation models.",
     long_description="Please check our github page: https://github.com/PathologyFoundation/pathologyfoundation",
     author = 'Zhi Huang',
     author_email = 'hz9423@gmail.com',
     url = 'https://github.com/PathologyFoundation/pathologyfoundation',
     keywords = ['Pathology', 'Foundation model', "PLIP", "OpenPath"],
     classifiers=[
```

