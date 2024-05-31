# Comparing `tmp/geocif-0.1.32.tar.gz` & `tmp/geocif-0.1.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geocif-0.1.32.tar", last modified: Tue May 28 01:06:33 2024, max compression
+gzip compressed data, was "geocif-0.1.33.tar", last modified: Fri May 31 02:06:30 2024, max compression
```

## Comparing `geocif-0.1.32.tar` & `geocif-0.1.33.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 01:06:33.417803 geocif-0.1.32/
--rw-rw-rw-   0        0        0     1096 2023-07-27 15:12:03.000000 geocif-0.1.32/LICENSE
--rw-rw-rw-   0        0        0      129 2023-07-27 15:12:03.000000 geocif-0.1.32/MANIFEST.in
--rw-rw-rw-   0        0        0     1586 2024-05-28 01:06:33.417803 geocif-0.1.32/PKG-INFO
--rw-rw-rw-   0        0        0      897 2024-05-12 14:58:37.000000 geocif-0.1.32/README.md
-drwxrwxrwx   0        0        0        0 2024-05-28 01:06:33.151611 geocif-0.1.32/geocif/
--rw-rw-rw-   0        0        0      155 2024-05-10 16:27:36.000000 geocif-0.1.32/geocif/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-28 01:06:33.209937 geocif-0.1.32/geocif/agmet/
--rw-rw-rw-   0        0        0        0 2024-05-09 16:19:42.000000 geocif-0.1.32/geocif/agmet/__init__.py
--rw-rw-rw-   0        0        0     6201 2024-05-09 16:20:58.000000 geocif-0.1.32/geocif/agmet/geoagmet.py
--rw-rw-rw-   0        0        0    27060 2024-05-09 16:20:58.000000 geocif-0.1.32/geocif/agmet/plot.py
--rw-rw-rw-   0        0        0     6907 2023-07-27 16:56:06.000000 geocif-0.1.32/geocif/agmet/utils.py
--rw-rw-rw-   0        0        0    42024 2024-05-27 22:17:35.000000 geocif-0.1.32/geocif/analysis.py
-drwxrwxrwx   0        0        0        0 2024-05-28 01:06:33.251512 geocif-0.1.32/geocif/backup/
--rw-rw-rw-   0        0        0        0 2024-05-09 16:19:12.000000 geocif-0.1.32/geocif/backup/__init__.py
--rw-rw-rw-   0        0        0       11 2023-07-27 15:12:03.000000 geocif-0.1.32/geocif/backup/constants.py
--rw-rw-rw-   0        0        0    10198 2024-05-10 00:43:58.000000 geocif-0.1.32/geocif/backup/features.py
--rw-rw-rw-   0        0        0     9919 2023-10-24 19:21:13.000000 geocif-0.1.32/geocif/backup/geo.py
--rw-rw-rw-   0        0        0    17693 2024-05-09 16:20:58.000000 geocif-0.1.32/geocif/backup/geocif.py
--rw-rw-rw-   0        0        0     1284 2023-10-24 19:33:45.000000 geocif-0.1.32/geocif/backup/metadata.py
--rw-rw-rw-   0        0        0       65 2023-07-27 16:50:11.000000 geocif-0.1.32/geocif/backup/models.py
-drwxrwxrwx   0        0        0        0 2024-05-28 01:06:33.283771 geocif-0.1.32/geocif/cei/
--rw-rw-rw-   0        0        0       83 2024-05-09 17:30:03.000000 geocif-0.1.32/geocif/cei/__init__.py
--rw-rw-rw-   0        0        0     5125 2024-05-09 18:11:43.000000 geocif-0.1.32/geocif/cei/definitions.py
--rw-rw-rw-   0        0        0    27358 2024-05-09 19:45:29.000000 geocif-0.1.32/geocif/cei/indices.py
--rw-rw-rw-   0        0        0    43725 2024-05-28 00:51:28.000000 geocif-0.1.32/geocif/geocif.py
--rw-rw-rw-   0        0        0     6647 2024-05-27 16:06:30.000000 geocif-0.1.32/geocif/indices_runner.py
--rw-rw-rw-   0        0        0     2274 2024-05-10 01:57:37.000000 geocif-0.1.32/geocif/logger.py
-drwxrwxrwx   0        0        0        0 2024-05-28 01:06:33.394899 geocif-0.1.32/geocif/ml/
--rw-rw-rw-   0        0        0       83 2024-05-10 16:27:36.000000 geocif-0.1.32/geocif/ml/__init__.py
--rw-rw-rw-   0        0        0    12623 2024-05-25 18:55:01.000000 geocif-0.1.32/geocif/ml/correlations.py
--rw-rw-rw-   0        0        0     5098 2024-05-25 18:55:01.000000 geocif-0.1.32/geocif/ml/embedding.py
--rw-rw-rw-   0        0        0    13882 2024-05-25 18:55:01.000000 geocif-0.1.32/geocif/ml/feature_engineering.py
--rw-rw-rw-   0        0        0     9120 2024-05-25 18:55:01.000000 geocif-0.1.32/geocif/ml/feature_selection.py
--rw-rw-rw-   0        0        0    10035 2024-05-25 18:55:01.000000 geocif-0.1.32/geocif/ml/outliers.py
--rw-rw-rw-   0        0        0      526 2024-03-31 02:56:14.000000 geocif-0.1.32/geocif/ml/outlook.py
--rw-rw-rw-   0        0        0     3671 2024-05-10 17:25:05.000000 geocif-0.1.32/geocif/ml/output.py
--rw-rw-rw-   0        0        0     5772 2024-05-28 01:02:23.000000 geocif-0.1.32/geocif/ml/spatial_autocorrelation.py
--rw-rw-rw-   0        0        0     8348 2024-05-25 18:55:01.000000 geocif-0.1.32/geocif/ml/stages.py
--rw-rw-rw-   0        0        0     9038 2024-05-25 18:55:01.000000 geocif-0.1.32/geocif/ml/stats.py
--rw-rw-rw-   0        0        0     9515 2024-05-25 18:55:01.000000 geocif-0.1.32/geocif/ml/trainers.py
--rw-rw-rw-   0        0        0     3171 2024-05-25 18:55:01.000000 geocif-0.1.32/geocif/ml/trend.py
--rw-rw-rw-   0        0        0     2831 2024-05-09 19:24:05.000000 geocif-0.1.32/geocif/ml/xai.py
-drwxrwxrwx   0        0        0        0 2024-05-28 01:06:33.408905 geocif-0.1.32/geocif/playground/
--rw-rw-rw-   0        0        0        0 2024-05-10 19:03:20.000000 geocif-0.1.32/geocif/playground/__init__.py
--rw-rw-rw-   0        0        0        0 2024-05-10 18:55:55.000000 geocif-0.1.32/geocif/playground/automl.py
--rw-rw-rw-   0        0        0    13665 2024-05-11 01:04:25.000000 geocif-0.1.32/geocif/playground/misc.py
--rw-rw-rw-   0        0        0    18744 2024-05-12 14:57:40.000000 geocif-0.1.32/geocif/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-28 01:06:33.413634 geocif-0.1.32/geocif/viz/
--rw-rw-rw-   0        0        0       83 2024-05-10 16:27:36.000000 geocif-0.1.32/geocif/viz/__init__.py
--rw-rw-rw-   0        0        0    15823 2024-05-27 18:53:10.000000 geocif-0.1.32/geocif/viz/plot.py
-drwxrwxrwx   0        0        0        0 2024-05-28 01:06:33.202823 geocif-0.1.32/geocif.egg-info/
--rw-rw-rw-   0        0        0     1586 2024-05-28 01:06:32.000000 geocif-0.1.32/geocif.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1144 2024-05-28 01:06:32.000000 geocif-0.1.32/geocif.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 01:06:32.000000 geocif-0.1.32/geocif.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-10-22 16:27:17.000000 geocif-0.1.32/geocif.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2024-05-28 01:06:32.000000 geocif-0.1.32/geocif.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2024-05-10 01:05:13.000000 geocif-0.1.32/requirements.txt
--rw-rw-rw-   0        0        0      415 2024-05-28 01:06:33.426329 geocif-0.1.32/setup.cfg
--rw-rw-rw-   0        0        0     1617 2024-05-28 01:06:27.000000 geocif-0.1.32/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-28 01:06:33.416800 geocif-0.1.32/tests/
--rw-rw-rw-   0        0        0      355 2024-05-09 16:20:58.000000 geocif-0.1.32/tests/test_geocif.py
+drwxrwxrwx   0        0        0        0 2024-05-31 02:06:30.424039 geocif-0.1.33/
+-rw-rw-rw-   0        0        0     1096 2023-07-27 15:12:03.000000 geocif-0.1.33/LICENSE
+-rw-rw-rw-   0        0        0      129 2023-07-27 15:12:03.000000 geocif-0.1.33/MANIFEST.in
+-rw-rw-rw-   0        0        0     1586 2024-05-31 02:06:30.423058 geocif-0.1.33/PKG-INFO
+-rw-rw-rw-   0        0        0      897 2024-05-12 14:58:37.000000 geocif-0.1.33/README.md
+drwxrwxrwx   0        0        0        0 2024-05-31 02:06:30.006187 geocif-0.1.33/geocif/
+-rw-rw-rw-   0        0        0      155 2024-05-10 16:27:36.000000 geocif-0.1.33/geocif/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 02:06:30.102784 geocif-0.1.33/geocif/agmet/
+-rw-rw-rw-   0        0        0        0 2024-05-09 16:19:42.000000 geocif-0.1.33/geocif/agmet/__init__.py
+-rw-rw-rw-   0        0        0     6201 2024-05-09 16:20:58.000000 geocif-0.1.33/geocif/agmet/geoagmet.py
+-rw-rw-rw-   0        0        0    27060 2024-05-09 16:20:58.000000 geocif-0.1.33/geocif/agmet/plot.py
+-rw-rw-rw-   0        0        0     6907 2023-07-27 16:56:06.000000 geocif-0.1.33/geocif/agmet/utils.py
+-rw-rw-rw-   0        0        0    42024 2024-05-27 22:17:35.000000 geocif-0.1.33/geocif/analysis.py
+drwxrwxrwx   0        0        0        0 2024-05-31 02:06:30.180630 geocif-0.1.33/geocif/backup/
+-rw-rw-rw-   0        0        0        0 2024-05-09 16:19:12.000000 geocif-0.1.33/geocif/backup/__init__.py
+-rw-rw-rw-   0        0        0       11 2023-07-27 15:12:03.000000 geocif-0.1.33/geocif/backup/constants.py
+-rw-rw-rw-   0        0        0    10198 2024-05-10 00:43:58.000000 geocif-0.1.33/geocif/backup/features.py
+-rw-rw-rw-   0        0        0     9919 2023-10-24 19:21:13.000000 geocif-0.1.33/geocif/backup/geo.py
+-rw-rw-rw-   0        0        0    17693 2024-05-09 16:20:58.000000 geocif-0.1.33/geocif/backup/geocif.py
+-rw-rw-rw-   0        0        0     1284 2023-10-24 19:33:45.000000 geocif-0.1.33/geocif/backup/metadata.py
+-rw-rw-rw-   0        0        0       65 2023-07-27 16:50:11.000000 geocif-0.1.33/geocif/backup/models.py
+drwxrwxrwx   0        0        0        0 2024-05-31 02:06:30.225075 geocif-0.1.33/geocif/cei/
+-rw-rw-rw-   0        0        0       83 2024-05-09 17:30:03.000000 geocif-0.1.33/geocif/cei/__init__.py
+-rw-rw-rw-   0        0        0     5125 2024-05-09 18:11:43.000000 geocif-0.1.33/geocif/cei/definitions.py
+-rw-rw-rw-   0        0        0    27358 2024-05-09 19:45:29.000000 geocif-0.1.33/geocif/cei/indices.py
+-rw-rw-rw-   0        0        0    45457 2024-05-30 03:25:48.000000 geocif-0.1.33/geocif/geocif.py
+-rw-rw-rw-   0        0        0     6647 2024-05-27 16:06:30.000000 geocif-0.1.33/geocif/indices_runner.py
+-rw-rw-rw-   0        0        0     2274 2024-05-10 01:57:37.000000 geocif-0.1.33/geocif/logger.py
+drwxrwxrwx   0        0        0        0 2024-05-31 02:06:30.358987 geocif-0.1.33/geocif/ml/
+-rw-rw-rw-   0        0        0       83 2024-05-10 16:27:36.000000 geocif-0.1.33/geocif/ml/__init__.py
+-rw-rw-rw-   0        0        0    12623 2024-05-25 18:55:01.000000 geocif-0.1.33/geocif/ml/correlations.py
+-rw-rw-rw-   0        0        0     5098 2024-05-25 18:55:01.000000 geocif-0.1.33/geocif/ml/embedding.py
+-rw-rw-rw-   0        0        0    13882 2024-05-25 18:55:01.000000 geocif-0.1.33/geocif/ml/feature_engineering.py
+-rw-rw-rw-   0        0        0     9120 2024-05-25 18:55:01.000000 geocif-0.1.33/geocif/ml/feature_selection.py
+-rw-rw-rw-   0        0        0    10035 2024-05-25 18:55:01.000000 geocif-0.1.33/geocif/ml/outliers.py
+-rw-rw-rw-   0        0        0      526 2024-03-31 02:56:14.000000 geocif-0.1.33/geocif/ml/outlook.py
+-rw-rw-rw-   0        0        0     3671 2024-05-10 17:25:05.000000 geocif-0.1.33/geocif/ml/output.py
+-rw-rw-rw-   0        0        0     5786 2024-05-28 02:25:52.000000 geocif-0.1.33/geocif/ml/spatial_autocorrelation.py
+-rw-rw-rw-   0        0        0     8348 2024-05-25 18:55:01.000000 geocif-0.1.33/geocif/ml/stages.py
+-rw-rw-rw-   0        0        0     9038 2024-05-25 18:55:01.000000 geocif-0.1.33/geocif/ml/stats.py
+-rw-rw-rw-   0        0        0    11008 2024-05-30 03:26:04.000000 geocif-0.1.33/geocif/ml/trainers.py
+-rw-rw-rw-   0        0        0     3171 2024-05-25 18:55:01.000000 geocif-0.1.33/geocif/ml/trend.py
+-rw-rw-rw-   0        0        0     2831 2024-05-09 19:24:05.000000 geocif-0.1.33/geocif/ml/xai.py
+drwxrwxrwx   0        0        0        0 2024-05-31 02:06:30.377988 geocif-0.1.33/geocif/playground/
+-rw-rw-rw-   0        0        0        0 2024-05-10 19:03:20.000000 geocif-0.1.33/geocif/playground/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-05-10 18:55:55.000000 geocif-0.1.33/geocif/playground/automl.py
+-rw-rw-rw-   0        0        0    13665 2024-05-11 01:04:25.000000 geocif-0.1.33/geocif/playground/misc.py
+-rw-rw-rw-   0        0        0    18744 2024-05-12 14:57:40.000000 geocif-0.1.33/geocif/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-31 02:06:30.401269 geocif-0.1.33/geocif/viz/
+-rw-rw-rw-   0        0        0       83 2024-05-10 16:27:36.000000 geocif-0.1.33/geocif/viz/__init__.py
+-rw-rw-rw-   0        0        0    15823 2024-05-27 18:53:10.000000 geocif-0.1.33/geocif/viz/plot.py
+drwxrwxrwx   0        0        0        0 2024-05-31 02:06:30.063470 geocif-0.1.33/geocif.egg-info/
+-rw-rw-rw-   0        0        0     1586 2024-05-31 02:06:28.000000 geocif-0.1.33/geocif.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1144 2024-05-31 02:06:29.000000 geocif-0.1.33/geocif.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 02:06:28.000000 geocif-0.1.33/geocif.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-10-22 16:27:17.000000 geocif-0.1.33/geocif.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        7 2024-05-31 02:06:28.000000 geocif-0.1.33/geocif.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2024-05-10 01:05:13.000000 geocif-0.1.33/requirements.txt
+-rw-rw-rw-   0        0        0      415 2024-05-31 02:06:30.433668 geocif-0.1.33/setup.cfg
+-rw-rw-rw-   0        0        0     1617 2024-05-31 02:03:32.000000 geocif-0.1.33/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 02:06:30.419412 geocif-0.1.33/tests/
+-rw-rw-rw-   0        0        0      355 2024-05-09 16:20:58.000000 geocif-0.1.33/tests/test_geocif.py
```

### Comparing `geocif-0.1.32/LICENSE` & `geocif-0.1.33/LICENSE`

 * *Files identical despite different names*

### Comparing `geocif-0.1.32/PKG-INFO` & `geocif-0.1.33/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geocif
-Version: 0.1.32
+Version: 0.1.33
 Summary: Models to visualize and forecast crop conditions and yields
 Home-page: https://ritviksahajpal.github.io/yield_forecasting/
 Author: Ritvik Sahajpal
 Author-email: ritvik@umd.edu
 License: MIT license
 Keywords: geocif
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `geocif-0.1.32/README.md` & `geocif-0.1.33/README.md`

 * *Files identical despite different names*

### Comparing `geocif-0.1.32/geocif/agmet/geoagmet.py` & `geocif-0.1.33/geocif/agmet/geoagmet.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.32/geocif/agmet/plot.py` & `geocif-0.1.33/geocif/agmet/plot.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.32/geocif/agmet/utils.py` & `geocif-0.1.33/geocif/agmet/utils.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.32/geocif/analysis.py` & `geocif-0.1.33/geocif/analysis.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.32/geocif/backup/features.py` & `geocif-0.1.33/geocif/backup/features.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.32/geocif/backup/geo.py` & `geocif-0.1.33/geocif/backup/geo.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.32/geocif/backup/geocif.py` & `geocif-0.1.33/geocif/backup/geocif.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.32/geocif/backup/metadata.py` & `geocif-0.1.33/geocif/backup/metadata.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.32/geocif/cei/definitions.py` & `geocif-0.1.33/geocif/cei/definitions.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.32/geocif/cei/indices.py` & `geocif-0.1.33/geocif/cei/indices.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.32/geocif/geocif.py` & `geocif-0.1.33/geocif/geocif.py`

 * *Files 3% similar despite different names*

```diff
@@ -218,14 +218,18 @@
             self.logger.info(f"Selecting features for {self.country} {self.crop}")
             selector, _, self.selected_features = fs.select_features(
                 X_train, y_train, method=self.feature_selection
             )
             self.logger.info(f"Selected features: {self.selected_features}")
 
             """ Update model to include conformal estimates """
+            if "lat" not in self.selected_features:
+                self.selected_features.append("lat")
+            if "lon" not in self.selected_features:
+                self.selected_features.append("lon")
             X_train = df_region[self.selected_features + self.cat_features]
             dir_output = (
                 self.dir_analysis
                 / self.country
                 / self.crop
                 / self.model_name
                 / str(self.forecast_season)
@@ -271,14 +275,20 @@
                     self.model.fit(
                         X_train,
                         y_train,
                         cat_features=self.cat_features,
                         verbose=False,
                         # callbacks=[TQDMCallback(self.best_hyperparams["iterations"])],
                     )
+                elif self.model_name == "geospaNN":
+                    self.model.fit(
+                        X_train,
+                        y_train,
+                        # callbacks=[TQDMCallback(self.best_hyperparams["iterations"])],
+                    )
                 elif self.model_name == "merf":
                     Z_train = np.ones((len(X_train), 1))
                     clusters_train = df_region["Region"]
                     clusters_train.reset_index(drop=True, inplace=True)
 
                     self.model.fit(
                         X_train,
@@ -337,14 +347,33 @@
                 clusters_test = df_region["Region"]
                 clusters_test.reset_index(drop=True, inplace=True)
 
                 y_pred = self.model.predict(
                     X_test, Z_test, clusters_test.astype("object")
                 )
                 best_hyperparameters = self.model.fe_model.get_params().copy()
+            elif self.model_name == "geospaNN":
+                import torch
+                import geospaNN
+
+                # Remove any categorical features
+                X_test = X_test.drop(columns=self.cat_features)
+                X = torch.from_numpy(X_test.to_numpy()).float()
+                coord = torch.from_numpy(self.df_test[['lon', 'lat']].to_numpy()).float()
+
+                p = X.shape[1]
+                n = X.shape[0]
+                nn = 5
+
+                data = geospaNN.make_graph(X, Y, coord, nn)
+
+                # remove categorical features from df_train
+                data_train = df_region[self.selected_features + self.cat_features + [self.target]]
+                w_train = data_train.y - self.estimate(data_train.x)
+
             else:
                 y_pred = self.model.predict(X_test)
                 best_hyperparameters = self.model.get_params().copy()
 
         if self.check_yield_trend:
             # Get information for retrending
             for idx, region in enumerate(df_region["Region"].unique()):
@@ -523,14 +552,18 @@
         if self.analogous_year_yield_as_feature:
             self.feature_names.append("Analogous Year")
             self.feature_names.append("Analogous Year Yield")
 
         if self.use_outlook_as_feature:
             self.feature_names.append("FCST")
 
+        # Add lat and lon to feature names
+        self.feature_names.append("lat")
+        self.feature_names.append("lon")
+
         self.selected_features = []
 
     def loop_ml(self, stages, dict_selected_features, dict_best_cei):
         """
 
         Args:
             stages:
@@ -778,14 +811,21 @@
         # Only use geometry column from self.dg
         self.dg_country = self.dg_country[["Country Region", "geometry"]].merge(
             df[["Country Region", self.correlation_plot_groupby]],
             on="Country Region",
             how="outer",
         )
 
+        # Add a lat and lon column to self.dg_country
+        self.dg_country["lat"] = self.dg_country.centroid.y
+        self.dg_country["lon"] = self.dg_country.centroid.x
+
+        # Add lat and lon columns to df by merging on Country Region column
+        df = df.merge(self.dg_country[["Country Region", "lat", "lon"]].drop_duplicates(), on="Country Region", how="left")
+
         dict_kwargs = {}
         dict_kwargs["all_stages"] = self.all_stages
         dict_kwargs["target_col"] = self.target
         dict_kwargs["country"] = self.country
         dict_kwargs["crop"] = self.crop
         dict_kwargs["dir_output"] = (
             self.dir_analysis
```

### Comparing `geocif-0.1.32/geocif/indices_runner.py` & `geocif-0.1.33/geocif/indices_runner.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.32/geocif/logger.py` & `geocif-0.1.33/geocif/logger.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.32/geocif/ml/correlations.py` & `geocif-0.1.33/geocif/ml/correlations.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.32/geocif/ml/embedding.py` & `geocif-0.1.33/geocif/ml/embedding.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.32/geocif/ml/feature_engineering.py` & `geocif-0.1.33/geocif/ml/feature_engineering.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.32/geocif/ml/feature_selection.py` & `geocif-0.1.33/geocif/ml/feature_selection.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.32/geocif/ml/outliers.py` & `geocif-0.1.33/geocif/ml/outliers.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.32/geocif/ml/outlook.py` & `geocif-0.1.33/geocif/ml/outlook.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.32/geocif/ml/output.py` & `geocif-0.1.33/geocif/ml/output.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.32/geocif/ml/spatial_autocorrelation.py` & `geocif-0.1.33/geocif/ml/spatial_autocorrelation.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     if no_neighbors:
         dg = dg.drop(index=no_neighbors[0]).reset_index(drop=True)
         w_base = weights.Queen.from_dataframe(dg[["Country Region", "geometry"]])
 
     return w_base, dg
 
 
-def create_weights_for_year(dg_country, regions_with_data):
+def create_weights_for_year(dg_country, regions_with_data, year):
     """
 
     Args:
         dg_country:
         regions_with_data:
 
     Returns:
@@ -93,18 +93,16 @@
     wt = weights.Queen.from_dataframe(dg)
 
     no_neighbors = [
         index for index, neighbors in wt.neighbors.items() if len(neighbors) == 0
     ]
     if no_neighbors:
         dg = dg.drop(index=no_neighbors[0]).reset_index(drop=True)
-        try:
-            wt = weights.Queen.from_dataframe(dg[["Country Region", "geometry"]])
-        except:
-            breakpoint()
+        wt = weights.Queen.from_dataframe(dg[["Country Region", "geometry"]])
+
     return wt, dg
 
 
 def compute_morans_i(merged_df):
     """
 
     Args:
@@ -121,24 +119,25 @@
 
     years = merged_df["Harvest Year"].unique()
     results = {"Harvest Year": [], "Moran's I": [], "p-value": [], "Significant": []}
 
     for year in tqdm(years, desc="Compute Moran's I"):
         year_data = merged_df[merged_df["Harvest Year"] == year]
         regions_with_data = year_data["Country Region"].unique()
+        if len(regions_with_data) < 3:
+            continue
         year_data = year_data[year_data["Country Region"].isin(regions_with_data)]
 
         y = year_data[
             ["Country Region", "Region", "Yield (tn per ha)"]
         ].drop_duplicates()
         dg_country = year_data[["Country Region", "geometry"]].drop_duplicates()
 
-        w, x = create_weights_for_year(dg_country, regions_with_data)
+        w, x = create_weights_for_year(dg_country, regions_with_data, year)
         y = y[y["Country Region"].isin(x["Country Region"])]
-
         if len(y) > 1:
             try:
                 mi = esda.Moran(y["Yield (tn per ha)"].values, w, permutations=999)
             except:
                 breakpoint()
             results["Harvest Year"].append(year)
             try:
```

### Comparing `geocif-0.1.32/geocif/ml/stages.py` & `geocif-0.1.33/geocif/ml/stages.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.32/geocif/ml/stats.py` & `geocif-0.1.33/geocif/ml/stats.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.32/geocif/ml/trainers.py` & `geocif-0.1.33/geocif/ml/trainers.py`

 * *Files 17% similar despite different names*

```diff
@@ -285,14 +285,48 @@
             model = LassoCV(cv=5, random_state=42)
         elif model_name == "gam":
             from pygam import LinearGAM
 
             model = LinearGAM(n_splines=25, spline_order=3).gridsearch(
                 X_train.values, y_train.values, lam=np.logspace(-3, 3, 11)
             )
+        elif model_name == "geospaNN":
+            import torch
+            import geospaNN
+
+            # Remove any categorical features
+            X_train = X_train.drop(columns=cat_features)
+            X = torch.from_numpy(X_train.to_numpy()).float()
+            Y = torch.from_numpy(y_train.to_numpy().reshape(-1)).float()
+
+            coord = torch.from_numpy(df_train[['lon', 'lat']].to_numpy()).float()
+
+            p = X.shape[1]
+            n = X.shape[0]
+            nn = 5
+
+            data = geospaNN.make_graph(X, Y, coord, nn)
+
+            mlp = torch.nn.Sequential(
+                torch.nn.Linear(p, 50),
+                torch.nn.ReLU(),
+                torch.nn.Linear(50, 20),
+                torch.nn.ReLU(),
+                torch.nn.Linear(20, 10),
+                torch.nn.ReLU(),
+                torch.nn.Linear(10, 1),
+            )
+
+            # Split data
+            data_train, data_val, data_test = geospaNN.split_data(X, Y, coord, neighbor_size=nn, test_proportion=0.1)
+            theta0 = geospaNN.theta_update(torch.tensor([1, 1.5, 0.01]), mlp(data_train.x).squeeze() - data_train.y, data_train.pos, neighbor_size=5)
+            model = geospaNN.nngls(p=p, neighbor_size=nn, coord_dimensions=2, mlp=mlp, theta=torch.tensor(theta0))
+            nngls_model = geospaNN.nngls_train(model, lr=0.01, min_delta=0.001)
+            # Log training process
+            training_log = nngls_model.train(data_train, data_val, data_test, Update_init=10, Update_step=10)
         elif model_name == "xgboost":
             raise NotImplementedError
         else:
             raise ValueError(f"Unknown model name: {model_name}")
 
     return hyperparams, model
```

### Comparing `geocif-0.1.32/geocif/ml/trend.py` & `geocif-0.1.33/geocif/ml/trend.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.32/geocif/ml/xai.py` & `geocif-0.1.33/geocif/ml/xai.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.32/geocif/playground/misc.py` & `geocif-0.1.33/geocif/playground/misc.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.32/geocif/utils.py` & `geocif-0.1.33/geocif/utils.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.32/geocif/viz/plot.py` & `geocif-0.1.33/geocif/viz/plot.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.32/geocif.egg-info/PKG-INFO` & `geocif-0.1.33/geocif.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geocif
-Version: 0.1.32
+Version: 0.1.33
 Summary: Models to visualize and forecast crop conditions and yields
 Home-page: https://ritviksahajpal.github.io/yield_forecasting/
 Author: Ritvik Sahajpal
 Author-email: ritvik@umd.edu
 License: MIT license
 Keywords: geocif
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `geocif-0.1.32/geocif.egg-info/SOURCES.txt` & `geocif-0.1.33/geocif.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geocif-0.1.32/setup.py` & `geocif-0.1.33/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,10 +46,10 @@
     keywords="geocif",
     name="geocif",
     packages=find_packages(include=["geocif", "geocif.*"]),
     setup_requires=setup_requirements,
     test_suite="tests",
     tests_require=test_requirements,
     url="https://ritviksahajpal.github.io/yield_forecasting/",
-    version="0.1.32",
+    version="0.1.33",
     zip_safe=False,
 )
```

