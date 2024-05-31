# Comparing `tmp/forecastout-0.0.4.tar.gz` & `tmp/forecastout-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forecastout-0.0.4.tar", max compression
+gzip compressed data, was "forecastout-0.0.5.tar", max compression
```

## Comparing `forecastout-0.0.4.tar` & `forecastout-0.0.5.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1065 2024-05-21 07:38:27.498190 forecastout-0.0.4/LICENSE
--rw-r--r--   0        0        0     3279 2024-05-21 07:38:27.498190 forecastout-0.0.4/README.md
--rw-r--r--   0        0        0       68 2024-05-21 07:38:27.498190 forecastout-0.0.4/forecastout/__init__.py
--rw-r--r--   0        0        0     1064 2024-05-21 07:38:27.498190 forecastout-0.0.4/forecastout/config.yaml
--rw-r--r--   0        0        0     7655 2024-05-21 07:38:27.498190 forecastout-0.0.4/forecastout/core.py
--rw-r--r--   0        0        0      128 2024-05-21 07:38:27.498190 forecastout-0.0.4/forecastout/data_engine/__init__.py
--rw-r--r--   0        0        0     5041 2024-05-21 07:38:27.498190 forecastout-0.0.4/forecastout/data_engine/data_handler.py
--rw-r--r--   0        0        0     1358 2024-05-21 07:38:27.498190 forecastout-0.0.4/forecastout/data_engine/train_test_split.py
--rw-r--r--   0        0        0      576 2024-05-21 07:38:27.498190 forecastout-0.0.4/forecastout/disaggregation_engine/__init__.py
--rw-r--r--   0        0        0     1154 2024-05-21 07:38:27.498190 forecastout-0.0.4/forecastout/disaggregation_engine/disaggregate_monthly_to_daily_forecast.py
--rw-r--r--   0        0        0      557 2024-05-21 07:38:27.498190 forecastout-0.0.4/forecastout/disaggregation_engine/disaggregation_model_factory.py
--rw-r--r--   0        0        0     1678 2024-05-21 07:38:27.498190 forecastout-0.0.4/forecastout/disaggregation_engine/disaggregation_model_predictor.py
--rw-r--r--   0        0        0      943 2024-05-21 07:38:27.498190 forecastout-0.0.4/forecastout/disaggregation_engine/disaggregation_model_trainer.py
--rw-r--r--   0        0        0     1035 2024-05-21 07:38:27.498190 forecastout-0.0.4/forecastout/disaggregation_engine/get_daily_shares.py
--rw-r--r--   0        0        0     1537 2024-05-21 07:38:27.498190 forecastout-0.0.4/forecastout/disaggregation_engine/remake_monthly_forecast_current_month.py
--rw-r--r--   0        0        0        0 2024-05-21 07:38:27.498190 forecastout-0.0.4/forecastout/disaggregation_features/__init__.py
--rw-r--r--   0        0        0     1330 2024-05-21 07:38:27.498190 forecastout-0.0.4/forecastout/disaggregation_features/add_features.py
--rw-r--r--   0        0        0     3092 2024-05-21 07:38:27.498190 forecastout-0.0.4/forecastout/disaggregation_features/feature_creator.py
--rw-r--r--   0        0        0      641 2024-05-21 07:38:27.498190 forecastout-0.0.4/forecastout/disaggregation_features/feature_encoding.py
--rw-r--r--   0        0        0      594 2024-05-21 07:38:27.498190 forecastout-0.0.4/forecastout/disaggregation_features/feature_normalizer.py
--rw-r--r--   0        0        0        0 2024-05-21 07:38:27.498190 forecastout-0.0.4/forecastout/disaggregation_models/__init__.py
--rw-r--r--   0        0        0      567 2024-05-21 07:38:27.498190 forecastout-0.0.4/forecastout/disaggregation_models/abstract_model.py
--rw-r--r--   0        0        0     2413 2024-05-21 07:38:27.498190 forecastout-0.0.4/forecastout/disaggregation_models/random_forest_model.py
--rw-r--r--   0        0        0      433 2024-05-21 07:38:27.498190 forecastout-0.0.4/forecastout/forecast_engine/__init__.py
--rw-r--r--   0        0        0     2836 2024-05-21 07:38:27.498190 forecastout-0.0.4/forecastout/forecast_engine/anomaly_detector.py
--rw-r--r--   0        0        0     2447 2024-05-21 07:38:27.498190 forecastout-0.0.4/forecastout/forecast_engine/anomaly_fixer.py
--rw-r--r--   0        0        0     2794 2024-05-21 07:38:27.498190 forecastout-0.0.4/forecastout/forecast_engine/backtester.py
--rw-r--r--   0        0        0      776 2024-05-21 07:38:27.498190 forecastout-0.0.4/forecastout/forecast_engine/decompose_time_series.py
--rw-r--r--   0        0        0      778 2024-05-21 07:38:27.498190 forecastout-0.0.4/forecastout/forecast_engine/ensemble_models.py
--rw-r--r--   0        0        0     2207 2024-05-21 07:38:27.498190 forecastout-0.0.4/forecastout/forecast_engine/ensembler.py
--rw-r--r--   0        0        0     1390 2024-05-21 07:38:27.498190 forecastout-0.0.4/forecastout/forecast_engine/forecast_model_factory.py
--rw-r--r--   0        0        0      906 2024-05-21 07:38:27.498190 forecastout-0.0.4/forecastout/forecast_engine/model_predictor.py
--rw-r--r--   0        0        0     1155 2024-05-21 07:38:27.498190 forecastout-0.0.4/forecastout/forecast_engine/model_trainer.py
--rw-r--r--   0        0        0        0 2024-05-21 07:38:27.498190 forecastout-0.0.4/forecastout/forecast_models/__init__.py
--rw-r--r--   0        0        0      442 2024-05-21 07:38:27.498190 forecastout-0.0.4/forecastout/forecast_models/abstract_model.py
--rw-r--r--   0        0        0     1497 2024-05-21 07:38:27.498190 forecastout-0.0.4/forecastout/forecast_models/autoarima_model.py
--rw-r--r--   0        0        0     3741 2024-05-21 07:38:27.498190 forecastout-0.0.4/forecastout/forecast_models/holtwinters_model.py
--rw-r--r--   0        0        0     2294 2024-05-21 07:38:27.498190 forecastout-0.0.4/forecastout/forecast_models/naive_seasonal.py
--rw-r--r--   0        0        0     1721 2024-05-21 07:38:27.498190 forecastout-0.0.4/forecastout/forecast_models/prophet_model.py
--rw-r--r--   0        0        0      114 2024-05-21 07:38:27.498190 forecastout-0.0.4/forecastout/utils/__init__.py
--rw-r--r--   0        0        0     5520 2024-05-21 07:38:27.498190 forecastout-0.0.4/forecastout/utils/input_checker.py
--rw-r--r--   0        0        0      850 2024-05-21 07:38:27.498190 forecastout-0.0.4/forecastout/utils/update_config.py
--rw-r--r--   0        0        0      992 2024-05-21 07:38:34.158192 forecastout-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     3974 1970-01-01 00:00:00.000000 forecastout-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-05-31 10:52:24.179920 forecastout-0.0.5/LICENSE
+-rw-r--r--   0        0        0     3279 2024-05-31 10:52:24.179920 forecastout-0.0.5/README.md
+-rw-r--r--   0        0        0       68 2024-05-31 10:52:24.179920 forecastout-0.0.5/forecastout/__init__.py
+-rw-r--r--   0        0        0     1062 2024-05-31 10:52:24.179920 forecastout-0.0.5/forecastout/config.yaml
+-rw-r--r--   0        0        0     7704 2024-05-31 10:52:24.179920 forecastout-0.0.5/forecastout/core.py
+-rw-r--r--   0        0        0      128 2024-05-31 10:52:24.179920 forecastout-0.0.5/forecastout/data_engine/__init__.py
+-rw-r--r--   0        0        0     5041 2024-05-31 10:52:24.179920 forecastout-0.0.5/forecastout/data_engine/data_handler.py
+-rw-r--r--   0        0        0     1358 2024-05-31 10:52:24.179920 forecastout-0.0.5/forecastout/data_engine/train_test_split.py
+-rw-r--r--   0        0        0      576 2024-05-31 10:52:24.179920 forecastout-0.0.5/forecastout/disaggregation_engine/__init__.py
+-rw-r--r--   0        0        0     1154 2024-05-31 10:52:24.179920 forecastout-0.0.5/forecastout/disaggregation_engine/disaggregate_monthly_to_daily_forecast.py
+-rw-r--r--   0        0        0      557 2024-05-31 10:52:24.179920 forecastout-0.0.5/forecastout/disaggregation_engine/disaggregation_model_factory.py
+-rw-r--r--   0        0        0     1678 2024-05-31 10:52:24.179920 forecastout-0.0.5/forecastout/disaggregation_engine/disaggregation_model_predictor.py
+-rw-r--r--   0        0        0      943 2024-05-31 10:52:24.179920 forecastout-0.0.5/forecastout/disaggregation_engine/disaggregation_model_trainer.py
+-rw-r--r--   0        0        0     1035 2024-05-31 10:52:24.179920 forecastout-0.0.5/forecastout/disaggregation_engine/get_daily_shares.py
+-rw-r--r--   0        0        0     1852 2024-05-31 10:52:24.179920 forecastout-0.0.5/forecastout/disaggregation_engine/remake_monthly_forecast_current_month.py
+-rw-r--r--   0        0        0        0 2024-05-31 10:52:24.179920 forecastout-0.0.5/forecastout/disaggregation_features/__init__.py
+-rw-r--r--   0        0        0     1330 2024-05-31 10:52:24.179920 forecastout-0.0.5/forecastout/disaggregation_features/add_features.py
+-rw-r--r--   0        0        0     3092 2024-05-31 10:52:24.179920 forecastout-0.0.5/forecastout/disaggregation_features/feature_creator.py
+-rw-r--r--   0        0        0      641 2024-05-31 10:52:24.179920 forecastout-0.0.5/forecastout/disaggregation_features/feature_encoding.py
+-rw-r--r--   0        0        0      594 2024-05-31 10:52:24.179920 forecastout-0.0.5/forecastout/disaggregation_features/feature_normalizer.py
+-rw-r--r--   0        0        0        0 2024-05-31 10:52:24.179920 forecastout-0.0.5/forecastout/disaggregation_models/__init__.py
+-rw-r--r--   0        0        0      567 2024-05-31 10:52:24.179920 forecastout-0.0.5/forecastout/disaggregation_models/abstract_model.py
+-rw-r--r--   0        0        0     2413 2024-05-31 10:52:24.179920 forecastout-0.0.5/forecastout/disaggregation_models/random_forest_model.py
+-rw-r--r--   0        0        0      433 2024-05-31 10:52:24.179920 forecastout-0.0.5/forecastout/forecast_engine/__init__.py
+-rw-r--r--   0        0        0     2836 2024-05-31 10:52:24.179920 forecastout-0.0.5/forecastout/forecast_engine/anomaly_detector.py
+-rw-r--r--   0        0        0     2447 2024-05-31 10:52:24.179920 forecastout-0.0.5/forecastout/forecast_engine/anomaly_fixer.py
+-rw-r--r--   0        0        0     2794 2024-05-31 10:52:24.179920 forecastout-0.0.5/forecastout/forecast_engine/backtester.py
+-rw-r--r--   0        0        0      776 2024-05-31 10:52:24.179920 forecastout-0.0.5/forecastout/forecast_engine/decompose_time_series.py
+-rw-r--r--   0        0        0      778 2024-05-31 10:52:24.179920 forecastout-0.0.5/forecastout/forecast_engine/ensemble_models.py
+-rw-r--r--   0        0        0     2207 2024-05-31 10:52:24.179920 forecastout-0.0.5/forecastout/forecast_engine/ensembler.py
+-rw-r--r--   0        0        0     1445 2024-05-31 10:52:24.179920 forecastout-0.0.5/forecastout/forecast_engine/forecast_model_factory.py
+-rw-r--r--   0        0        0      906 2024-05-31 10:52:24.179920 forecastout-0.0.5/forecastout/forecast_engine/model_predictor.py
+-rw-r--r--   0        0        0     1155 2024-05-31 10:52:24.179920 forecastout-0.0.5/forecastout/forecast_engine/model_trainer.py
+-rw-r--r--   0        0        0        0 2024-05-31 10:52:24.179920 forecastout-0.0.5/forecastout/forecast_models/__init__.py
+-rw-r--r--   0        0        0      541 2024-05-31 10:52:24.179920 forecastout-0.0.5/forecastout/forecast_models/abstract_model.py
+-rw-r--r--   0        0        0     2110 2024-05-31 10:52:24.179920 forecastout-0.0.5/forecastout/forecast_models/autoarima_model.py
+-rw-r--r--   0        0        0     3698 2024-05-31 10:52:24.179920 forecastout-0.0.5/forecastout/forecast_models/holtwinters_model.py
+-rw-r--r--   0        0        0     2251 2024-05-31 10:52:24.179920 forecastout-0.0.5/forecastout/forecast_models/naive_seasonal.py
+-rw-r--r--   0        0        0     1678 2024-05-31 10:52:24.179920 forecastout-0.0.5/forecastout/forecast_models/prophet_model.py
+-rw-r--r--   0        0        0      114 2024-05-31 10:52:24.179920 forecastout-0.0.5/forecastout/utils/__init__.py
+-rw-r--r--   0        0        0     5520 2024-05-31 10:52:24.179920 forecastout-0.0.5/forecastout/utils/input_checker.py
+-rw-r--r--   0        0        0      850 2024-05-31 10:52:24.179920 forecastout-0.0.5/forecastout/utils/update_config.py
+-rw-r--r--   0        0        0      992 2024-05-31 10:52:31.199919 forecastout-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3974 1970-01-01 00:00:00.000000 forecastout-0.0.5/PKG-INFO
```

### Comparing `forecastout-0.0.4/LICENSE` & `forecastout-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `forecastout-0.0.4/README.md` & `forecastout-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `forecastout-0.0.4/forecastout/config.yaml` & `forecastout-0.0.5/forecastout/config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 months_to_backtest: 3
 models_to_use: ['autoarima', 'holtwinters', 'prophet'] # "seasonalnaive"
 models_to_fix: ['seasonalnaive']
 models:
   autoarima:
     "seasonality": "True"
     "freq": 12
-    "alpha_intervals": 0.05
+    "alpha_intervals": 95
   prophet:
   holtwinters:
     "freq": 12
     "alpha_intervals": 95
   seasonalnaive:
     "freq": 12
     "alpha_intervals": 95
```

### Comparing `forecastout-0.0.4/forecastout/core.py` & `forecastout-0.0.5/forecastout/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,16 +146,16 @@
         self.log.info(">> 3.1. Feature Creation")
         df = add_features(df=self.df_daily)
         self.log.info(">> 3.2. Train/Test Split")
         df_train_test = TrainTestSplit.split_by_current_closed_month(
             df=df.copy(),
             current_month=(
                 self.df_monthly.loc[
-                    ~self.df_monthly['value'].isna(), 'date'
-                ].max()
+                    self.df_monthly['value'].isna(), 'date'
+                ].min()
             ),
             granularity_month=False
         )
         self.log.info(">> 3.3. Train disaggregation models")
         disaggregation_model_trainer = DisaggregationModelTrainer(
             df_train=(
                 df_train_test.loc[df_train_test['test'] == 0].dropna().copy()
@@ -188,9 +188,10 @@
                 df_daily_forecast["date"] > self.df["date"].max()
                 ].copy()
         )
 
     def __remake_monthly_forecast(self):
         self.df_monthly_forecast = remake_monthly_forecast_current_month(
             df_daily_forecast=self.df_daily_forecast.copy(),
-            df_actuals=self.df.copy()
+            df_actuals=self.df.copy(),
+            sum_aggregation=self.sum_aggregation
         )
```

### Comparing `forecastout-0.0.4/forecastout/data_engine/data_handler.py` & `forecastout-0.0.5/forecastout/data_engine/data_handler.py`

 * *Files identical despite different names*

### Comparing `forecastout-0.0.4/forecastout/data_engine/train_test_split.py` & `forecastout-0.0.5/forecastout/data_engine/train_test_split.py`

 * *Files identical despite different names*

### Comparing `forecastout-0.0.4/forecastout/disaggregation_engine/__init__.py` & `forecastout-0.0.5/forecastout/disaggregation_engine/__init__.py`

 * *Files identical despite different names*

### Comparing `forecastout-0.0.4/forecastout/disaggregation_engine/disaggregate_monthly_to_daily_forecast.py` & `forecastout-0.0.5/forecastout/disaggregation_engine/disaggregate_monthly_to_daily_forecast.py`

 * *Files identical despite different names*

### Comparing `forecastout-0.0.4/forecastout/disaggregation_engine/disaggregation_model_factory.py` & `forecastout-0.0.5/forecastout/disaggregation_engine/disaggregation_model_factory.py`

 * *Files identical despite different names*

### Comparing `forecastout-0.0.4/forecastout/disaggregation_engine/disaggregation_model_predictor.py` & `forecastout-0.0.5/forecastout/disaggregation_engine/disaggregation_model_predictor.py`

 * *Files identical despite different names*

### Comparing `forecastout-0.0.4/forecastout/disaggregation_engine/disaggregation_model_trainer.py` & `forecastout-0.0.5/forecastout/disaggregation_engine/disaggregation_model_trainer.py`

 * *Files identical despite different names*

### Comparing `forecastout-0.0.4/forecastout/disaggregation_engine/get_daily_shares.py` & `forecastout-0.0.5/forecastout/disaggregation_engine/get_daily_shares.py`

 * *Files identical despite different names*

### Comparing `forecastout-0.0.4/forecastout/disaggregation_engine/remake_monthly_forecast_current_month.py` & `forecastout-0.0.5/forecastout/disaggregation_engine/remake_monthly_forecast_current_month.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import pandas as pd
 
 
 def remake_monthly_forecast_current_month(
         df_daily_forecast: pd.DataFrame,
-        df_actuals: pd.DataFrame
+        df_actuals: pd.DataFrame,
+        sum_aggregation: bool
 ) -> pd.DataFrame:
     # -- Get actuals of unfinished month
     first_forecast_day = df_daily_forecast['date'].min()
     first_actuals_day = pd.to_datetime(
         str(first_forecast_day)[0:7] + '-01'
     )
     df_actuals = df_actuals.loc[
@@ -22,21 +23,30 @@
     # -- Recompute monthly forecast
     df_daily_forecast = pd.concat(
         [df_actuals, df_daily_forecast], axis=0
     )
     df_daily_forecast["date"] = (
         df_daily_forecast["date"].astype(str).str[0:7]
     )
-    df_monthly_forecast = (
-        df_daily_forecast
-        .groupby(["date", "model"])
-        [["forecast", "forecast_lower", "forecast_upper"]]
-        .sum()
-        .reset_index()
-    )
+    if sum_aggregation:
+        df_monthly_forecast = (
+            df_daily_forecast
+            .groupby(["date", "model"])
+            [["forecast", "forecast_lower", "forecast_upper"]]
+            .sum()
+            .reset_index()
+        )
+    else:
+        df_monthly_forecast = (
+            df_daily_forecast
+            .groupby(["date", "model"])
+            [["forecast", "forecast_lower", "forecast_upper"]]
+            .mean()
+            .reset_index()
+        )
     df_monthly_forecast['date'] = pd.to_datetime(
         df_monthly_forecast['date'] + '-01'
     )
     column_order = [
         "forecast",
         "forecast_lower",
         "forecast_upper",
```

### Comparing `forecastout-0.0.4/forecastout/disaggregation_features/add_features.py` & `forecastout-0.0.5/forecastout/disaggregation_features/add_features.py`

 * *Files identical despite different names*

### Comparing `forecastout-0.0.4/forecastout/disaggregation_features/feature_creator.py` & `forecastout-0.0.5/forecastout/disaggregation_features/feature_creator.py`

 * *Files identical despite different names*

### Comparing `forecastout-0.0.4/forecastout/disaggregation_features/feature_encoding.py` & `forecastout-0.0.5/forecastout/disaggregation_features/feature_encoding.py`

 * *Files identical despite different names*

### Comparing `forecastout-0.0.4/forecastout/disaggregation_features/feature_normalizer.py` & `forecastout-0.0.5/forecastout/disaggregation_features/feature_normalizer.py`

 * *Files identical despite different names*

### Comparing `forecastout-0.0.4/forecastout/disaggregation_models/abstract_model.py` & `forecastout-0.0.5/forecastout/disaggregation_models/abstract_model.py`

 * *Files identical despite different names*

### Comparing `forecastout-0.0.4/forecastout/disaggregation_models/random_forest_model.py` & `forecastout-0.0.5/forecastout/disaggregation_models/random_forest_model.py`

 * *Files identical despite different names*

### Comparing `forecastout-0.0.4/forecastout/forecast_engine/anomaly_detector.py` & `forecastout-0.0.5/forecastout/forecast_engine/anomaly_detector.py`

 * *Files identical despite different names*

### Comparing `forecastout-0.0.4/forecastout/forecast_engine/anomaly_fixer.py` & `forecastout-0.0.5/forecastout/forecast_engine/anomaly_fixer.py`

 * *Files identical despite different names*

### Comparing `forecastout-0.0.4/forecastout/forecast_engine/backtester.py` & `forecastout-0.0.5/forecastout/forecast_engine/backtester.py`

 * *Files identical despite different names*

### Comparing `forecastout-0.0.4/forecastout/forecast_engine/decompose_time_series.py` & `forecastout-0.0.5/forecastout/forecast_engine/decompose_time_series.py`

 * *Files identical despite different names*

### Comparing `forecastout-0.0.4/forecastout/forecast_engine/ensemble_models.py` & `forecastout-0.0.5/forecastout/forecast_engine/ensemble_models.py`

 * *Files identical despite different names*

### Comparing `forecastout-0.0.4/forecastout/forecast_engine/ensembler.py` & `forecastout-0.0.5/forecastout/forecast_engine/ensembler.py`

 * *Files identical despite different names*

### Comparing `forecastout-0.0.4/forecastout/forecast_engine/forecast_model_factory.py` & `forecastout-0.0.5/forecastout/forecast_engine/forecast_model_factory.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,15 +15,16 @@
             df_train_y: pd.DataFrame,
             dict_config: dict,
             series_train_dates: pd.Series
     ):
         if model == "autoarima":
             return AutoArimaModel(
                 df_train_y=df_train_y,
-                dict_config=dict_config
+                dict_config=dict_config,
+                series_train_dates=series_train_dates
             )
         if model == "prophet":
             return ProphetModel(
                 df_train_y=df_train_y,
                 dict_config=dict_config,
                 series_train_dates=series_train_dates
             )
```

### Comparing `forecastout-0.0.4/forecastout/forecast_engine/model_predictor.py` & `forecastout-0.0.5/forecastout/forecast_engine/model_predictor.py`

 * *Files identical despite different names*

### Comparing `forecastout-0.0.4/forecastout/forecast_engine/model_trainer.py` & `forecastout-0.0.5/forecastout/forecast_engine/model_trainer.py`

 * *Files identical despite different names*

### Comparing `forecastout-0.0.4/forecastout/forecast_models/holtwinters_model.py` & `forecastout-0.0.5/forecastout/forecast_models/holtwinters_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from statsforecast import StatsForecast
 import pandas as pd
 import numpy as np
 
 
 class HoltWintersModel(ForecastModel):
     def __init__(self,
-                 series_train_dates: pd.Series,
                  *args,
                  **kwargs
                  ):
         """
         This implementation returns the corresponding `ETS` model with additive
         (A) or multiplicative (M) errors (so either 'AAA' or 'MAM').
         """
@@ -29,15 +28,15 @@
                 error_type='M',
                 alias='HW_M')],
             freq='MS',
             n_jobs=-1
         )
         # -- Transform data
         df_train_y_holtwinters = pd.concat(
-            [series_train_dates, self.df_train_y],
+            [self.series_train_dates, self.df_train_y],
             axis=1
         )
         df_train_y_holtwinters.columns = ['ds', 'y']
         df_train_y_holtwinters['ds'] = (
             pd.to_datetime(df_train_y_holtwinters['ds'])
         )
         df_train_y_holtwinters['ds'] = (
```

### Comparing `forecastout-0.0.4/forecastout/forecast_models/naive_seasonal.py` & `forecastout-0.0.5/forecastout/forecast_models/naive_seasonal.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from statsforecast.models import SeasonalNaive
 from statsforecast import StatsForecast
 import pandas as pd
 
 
 class NaiveSeasonalModel(ForecastModel):
     def __init__(self,
-                 series_train_dates: pd.Series,
                  *args,
                  **kwargs
                  ):
         """
         This implementation a naive seasonal forecast
         """
         super(NaiveSeasonalModel, self).__init__(*args, **kwargs)
@@ -20,15 +19,15 @@
         self.seasonalnaive_model = StatsForecast(models=[
             SeasonalNaive(season_length=self.dict_config['freq'])],
             freq='MS',
             n_jobs=-1
         )
         # -- Transform data
         df_train_y_seasonalnaive = (
-            pd.concat([series_train_dates, self.df_train_y], axis=1)
+            pd.concat([self.series_train_dates, self.df_train_y], axis=1)
         )
         df_train_y_seasonalnaive.columns = ['ds', 'y']
         df_train_y_seasonalnaive['ds'] = (
             pd.to_datetime(df_train_y_seasonalnaive['ds'])
         )
         df_train_y_seasonalnaive['ds'] = (
             df_train_y_seasonalnaive['ds'].dt.tz_localize(None)
```

### Comparing `forecastout-0.0.4/forecastout/forecast_models/prophet_model.py` & `forecastout-0.0.5/forecastout/forecast_models/prophet_model.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 from forecastout.forecast_models.abstract_model import ForecastModel
 from prophet import Prophet
 import pandas as pd
 
 
 class ProphetModel(ForecastModel):
     def __init__(self,
-                 series_train_dates: pd.Series,
                  *args,
                  **kwargs
                  ):
         """
         This implementation a prophet model
         """
         super(ProphetModel, self).__init__(*args, **kwargs)
         # -- Prophet
         # -- Constructor
         df_train_y_prophet = pd.concat(
-            [series_train_dates, self.df_train_y],
+            [self.series_train_dates, self.df_train_y],
             axis=1)
         df_train_y_prophet.columns = ['ds', 'y']
         df_train_y_prophet['ds'] = pd.to_datetime(df_train_y_prophet['ds'])
         df_train_y_prophet['ds'] = (
             df_train_y_prophet['ds']
             .dt
             .tz_localize(None)
```

### Comparing `forecastout-0.0.4/forecastout/utils/input_checker.py` & `forecastout-0.0.5/forecastout/utils/input_checker.py`

 * *Files identical despite different names*

### Comparing `forecastout-0.0.4/forecastout/utils/update_config.py` & `forecastout-0.0.5/forecastout/utils/update_config.py`

 * *Files identical despite different names*

### Comparing `forecastout-0.0.4/pyproject.toml` & `forecastout-0.0.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "forecastout"
-version = "0.0.4"
+version = "0.0.5"
 description = ""
 authors = ["alexis-vazquez <alexis.vazquez@adevinta.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pandas = "^2.2.1"
```

### Comparing `forecastout-0.0.4/PKG-INFO` & `forecastout-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forecastout
-Version: 0.0.4
+Version: 0.0.5
 Summary: 
 Author: alexis-vazquez
 Author-email: alexis.vazquez@adevinta.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

