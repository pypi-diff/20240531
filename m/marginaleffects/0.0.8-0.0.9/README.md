# Comparing `tmp/marginaleffects-0.0.8.tar.gz` & `tmp/marginaleffects-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marginaleffects-0.0.8.tar", max compression
+gzip compressed data, was "marginaleffects-0.0.9.tar", max compression
```

## Comparing `marginaleffects-0.0.8.tar` & `marginaleffects-0.0.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    35149 2023-12-24 02:49:26.417082 marginaleffects-0.0.8/LICENSE
--rw-r--r--   0        0        0     4058 2023-12-26 16:04:55.996631 marginaleffects-0.0.8/README.md
--rw-r--r--   0        0        0      344 2023-12-27 16:46:13.174919 marginaleffects-0.0.8/marginaleffects/__init__.py
--rw-r--r--   0        0        0     1027 2023-12-27 17:38:03.854178 marginaleffects-0.0.8/marginaleffects/by.py
--rw-r--r--   0        0        0     2432 2024-01-23 12:25:27.384552 marginaleffects-0.0.8/marginaleffects/classes.py
--rw-r--r--   0        0        0    14163 2024-01-23 12:25:27.384552 marginaleffects-0.0.8/marginaleffects/comparisons.py
--rw-r--r--   0        0        0     6580 2024-01-23 12:17:35.414694 marginaleffects-0.0.8/marginaleffects/datagrid.py
--rw-r--r--   0        0        0     1636 2023-12-27 18:20:39.193549 marginaleffects-0.0.8/marginaleffects/equivalence.py
--rw-r--r--   0        0        0     3157 2023-12-24 02:49:26.417082 marginaleffects-0.0.8/marginaleffects/estimands.py
--rw-r--r--   0        0        0     4145 2024-01-23 12:25:22.944553 marginaleffects-0.0.8/marginaleffects/hypotheses.py
--rw-r--r--   0        0        0     7367 2023-12-27 17:24:25.964361 marginaleffects-0.0.8/marginaleffects/hypothesis.py
--rw-r--r--   0        0        0     1828 2024-01-23 12:17:35.414694 marginaleffects-0.0.8/marginaleffects/model_abstract.py
--rw-r--r--   0        0        0     3391 2024-01-23 12:17:35.414694 marginaleffects-0.0.8/marginaleffects/model_pyfixest.py
--rw-r--r--   0        0        0     3762 2023-12-27 17:25:34.714358 marginaleffects-0.0.8/marginaleffects/model_statsmodels.py
--rw-r--r--   0        0        0     1659 2024-01-23 12:17:35.414694 marginaleffects-0.0.8/marginaleffects/p9.py
--rw-r--r--   0        0        0     3928 2024-01-23 12:17:35.414694 marginaleffects-0.0.8/marginaleffects/plot_common.py
--rw-r--r--   0        0        0     5001 2024-01-23 12:17:35.424694 marginaleffects-0.0.8/marginaleffects/plot_comparisons.py
--rw-r--r--   0        0        0     4275 2024-01-23 12:17:35.424694 marginaleffects-0.0.8/marginaleffects/plot_predictions.py
--rw-r--r--   0        0        0     4967 2024-01-23 12:17:35.424694 marginaleffects-0.0.8/marginaleffects/plot_slopes.py
--rw-r--r--   0        0        0     7867 2024-01-23 12:25:27.384552 marginaleffects-0.0.8/marginaleffects/predictions.py
--rw-r--r--   0        0        0      749 2023-12-27 04:16:38.195890 marginaleffects-0.0.8/marginaleffects/sanitize_model.py
--rw-r--r--   0        0        0    13953 2024-01-23 12:17:35.424694 marginaleffects-0.0.8/marginaleffects/sanity.py
--rw-r--r--   0        0        0     1573 2023-12-27 22:09:48.990070 marginaleffects-0.0.8/marginaleffects/slopes.py
--rw-r--r--   0        0        0      393 2023-12-27 18:20:10.203555 marginaleffects-0.0.8/marginaleffects/transform.py
--rw-r--r--   0        0        0     2622 2023-12-27 17:39:54.654151 marginaleffects-0.0.8/marginaleffects/uncertainty.py
--rw-r--r--   0        0        0     3050 2024-01-23 12:17:35.424694 marginaleffects-0.0.8/marginaleffects/utils.py
--rw-r--r--   0        0        0      884 2024-01-23 12:27:41.054578 marginaleffects-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     4741 1970-01-01 00:00:00.000000 marginaleffects-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-23 12:35:22.380022 marginaleffects-0.0.9/LICENSE
+-rw-r--r--   0        0        0     4058 2023-12-31 20:13:18.164193 marginaleffects-0.0.9/README.md
+-rw-r--r--   0        0        0      344 2024-02-16 15:54:04.256033 marginaleffects-0.0.9/marginaleffects/__init__.py
+-rw-r--r--   0        0        0     1027 2024-02-16 15:54:04.256033 marginaleffects-0.0.9/marginaleffects/by.py
+-rw-r--r--   0        0        0     2432 2024-02-16 15:54:04.256033 marginaleffects-0.0.9/marginaleffects/classes.py
+-rw-r--r--   0        0        0    14163 2024-02-16 15:54:04.256033 marginaleffects-0.0.9/marginaleffects/comparisons.py
+-rw-r--r--   0        0        0     6580 2024-02-16 15:54:04.256033 marginaleffects-0.0.9/marginaleffects/datagrid.py
+-rw-r--r--   0        0        0     1636 2024-02-16 15:54:04.256033 marginaleffects-0.0.9/marginaleffects/equivalence.py
+-rw-r--r--   0        0        0     3157 2024-02-16 15:54:04.256033 marginaleffects-0.0.9/marginaleffects/estimands.py
+-rw-r--r--   0        0        0     4145 2024-02-16 15:54:04.256033 marginaleffects-0.0.9/marginaleffects/hypotheses.py
+-rw-r--r--   0        0        0     7367 2024-02-16 15:56:23.115979 marginaleffects-0.0.9/marginaleffects/hypothesis.py
+-rw-r--r--   0        0        0     1828 2024-02-16 15:54:04.256033 marginaleffects-0.0.9/marginaleffects/model_abstract.py
+-rw-r--r--   0        0        0     3391 2024-02-16 15:54:04.256033 marginaleffects-0.0.9/marginaleffects/model_pyfixest.py
+-rw-r--r--   0        0        0     3804 2024-03-03 17:10:22.442984 marginaleffects-0.0.9/marginaleffects/model_statsmodels.py
+-rw-r--r--   0        0        0     1659 2024-02-16 15:54:04.256033 marginaleffects-0.0.9/marginaleffects/p9.py
+-rw-r--r--   0        0        0     3928 2024-02-16 15:56:23.115979 marginaleffects-0.0.9/marginaleffects/plot_common.py
+-rw-r--r--   0        0        0     5001 2024-02-16 15:54:04.256033 marginaleffects-0.0.9/marginaleffects/plot_comparisons.py
+-rw-r--r--   0        0        0     4275 2024-02-16 15:54:04.256033 marginaleffects-0.0.9/marginaleffects/plot_predictions.py
+-rw-r--r--   0        0        0     4967 2024-02-16 15:54:04.256033 marginaleffects-0.0.9/marginaleffects/plot_slopes.py
+-rw-r--r--   0        0        0     7867 2024-03-03 17:04:43.873010 marginaleffects-0.0.9/marginaleffects/predictions.py
+-rw-r--r--   0        0        0      749 2024-02-16 15:54:04.256033 marginaleffects-0.0.9/marginaleffects/sanitize_model.py
+-rw-r--r--   0        0        0    14697 2024-03-03 17:04:43.873010 marginaleffects-0.0.9/marginaleffects/sanity.py
+-rw-r--r--   0        0        0     1573 2024-02-16 15:54:04.256033 marginaleffects-0.0.9/marginaleffects/slopes.py
+-rw-r--r--   0        0        0      393 2024-02-16 15:54:04.256033 marginaleffects-0.0.9/marginaleffects/transform.py
+-rw-r--r--   0        0        0     2622 2024-02-16 15:54:04.256033 marginaleffects-0.0.9/marginaleffects/uncertainty.py
+-rw-r--r--   0        0        0     3050 2024-02-16 15:54:04.256033 marginaleffects-0.0.9/marginaleffects/utils.py
+-rw-r--r--   0        0        0      884 2024-03-03 17:10:49.352982 marginaleffects-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     4690 1970-01-01 00:00:00.000000 marginaleffects-0.0.9/PKG-INFO
```

### Comparing `marginaleffects-0.0.8/LICENSE` & `marginaleffects-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `marginaleffects-0.0.8/README.md` & `marginaleffects-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `marginaleffects-0.0.8/marginaleffects/by.py` & `marginaleffects-0.0.9/marginaleffects/by.py`

 * *Files identical despite different names*

### Comparing `marginaleffects-0.0.8/marginaleffects/classes.py` & `marginaleffects-0.0.9/marginaleffects/classes.py`

 * *Files identical despite different names*

### Comparing `marginaleffects-0.0.8/marginaleffects/comparisons.py` & `marginaleffects-0.0.9/marginaleffects/comparisons.py`

 * *Files identical despite different names*

### Comparing `marginaleffects-0.0.8/marginaleffects/datagrid.py` & `marginaleffects-0.0.9/marginaleffects/datagrid.py`

 * *Files identical despite different names*

### Comparing `marginaleffects-0.0.8/marginaleffects/equivalence.py` & `marginaleffects-0.0.9/marginaleffects/equivalence.py`

 * *Files identical despite different names*

### Comparing `marginaleffects-0.0.8/marginaleffects/estimands.py` & `marginaleffects-0.0.9/marginaleffects/estimands.py`

 * *Files identical despite different names*

### Comparing `marginaleffects-0.0.8/marginaleffects/hypotheses.py` & `marginaleffects-0.0.9/marginaleffects/hypotheses.py`

 * *Files identical despite different names*

### Comparing `marginaleffects-0.0.8/marginaleffects/hypothesis.py` & `marginaleffects-0.0.9/marginaleffects/hypothesis.py`

 * *Files identical despite different names*

### Comparing `marginaleffects-0.0.8/marginaleffects/model_abstract.py` & `marginaleffects-0.0.9/marginaleffects/model_abstract.py`

 * *Files identical despite different names*

### Comparing `marginaleffects-0.0.8/marginaleffects/model_pyfixest.py` & `marginaleffects-0.0.9/marginaleffects/model_pyfixest.py`

 * *Files identical despite different names*

### Comparing `marginaleffects-0.0.8/marginaleffects/model_statsmodels.py` & `marginaleffects-0.0.9/marginaleffects/model_statsmodels.py`

 * *Files 24% similar despite different names*

```diff
@@ -46,18 +46,23 @@
                     "vcov must be a square numpy array with dimensions equal to the length of self.coef"
                 )
 
         return V
 
     def get_variables_names(self, variables=None, newdata=None):
         if variables is None:
-            variables = self.model.model.exog_names
-            variables = [re.sub("\[.*\]", "", x) for x in variables]
-            variables = [x for x in variables if x in self.modeldata.columns]
-            variables = pl.Series(variables).unique().to_list()
+            formula = self.formula
+            columns = self.modeldata.columns
+            variables = list(
+                {
+                    var
+                    for var in columns
+                    if re.search(rf"\b{re.escape(var)}\b", formula.split("~")[1])
+                }
+            )
 
         if isinstance(variables, (str, dict)):
             variables = [variables] if isinstance(variables, str) else variables
         elif isinstance(variables, list) and all(
             isinstance(var, str) for var in variables
         ):
             pass
```

### Comparing `marginaleffects-0.0.8/marginaleffects/p9.py` & `marginaleffects-0.0.9/marginaleffects/p9.py`

 * *Files identical despite different names*

### Comparing `marginaleffects-0.0.8/marginaleffects/plot_common.py` & `marginaleffects-0.0.9/marginaleffects/plot_common.py`

 * *Files identical despite different names*

### Comparing `marginaleffects-0.0.8/marginaleffects/plot_comparisons.py` & `marginaleffects-0.0.9/marginaleffects/plot_comparisons.py`

 * *Files identical despite different names*

### Comparing `marginaleffects-0.0.8/marginaleffects/plot_predictions.py` & `marginaleffects-0.0.9/marginaleffects/plot_predictions.py`

 * *Files identical despite different names*

### Comparing `marginaleffects-0.0.8/marginaleffects/plot_slopes.py` & `marginaleffects-0.0.9/marginaleffects/plot_slopes.py`

 * *Files identical despite different names*

### Comparing `marginaleffects-0.0.8/marginaleffects/predictions.py` & `marginaleffects-0.0.9/marginaleffects/predictions.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     -------
     DataFrame
         A DataFrame with one row per observation and several columns:
         - rowid: row number of the `newdata` data frame
         - type: prediction type, as defined by the `type` argument
         - group: (optional) value of the grouped outcome (e.g., categorical outcome models)
         - estimate: predicted outcome
-        - std.error: standard errors computed using the delta method.
+        - std_error: standard errors computed using the delta method.
         - p_value: p value associated with the `estimate` column.
         - s_value: Shannon information transforms of p values.
         - conf_low: lower bound of the confidence interval (or equal-tailed interval for Bayesian models)
         - conf_high: upper bound of the confidence interval (or equal-tailed interval for Bayesian models)
     """
 
     if callable(newdata):
```

### Comparing `marginaleffects-0.0.8/marginaleffects/sanitize_model.py` & `marginaleffects-0.0.9/marginaleffects/sanitize_model.py`

 * *Files identical despite different names*

### Comparing `marginaleffects-0.0.8/marginaleffects/sanity.py` & `marginaleffects-0.0.9/marginaleffects/sanity.py`

 * *Files 13% similar despite different names*

```diff
@@ -50,14 +50,32 @@
             if isinstance(newdata, pd.DataFrame):
                 out = pl.from_pandas(newdata)
             else:
                 out = newdata
         except ImportError:
             out = newdata
 
+    reserved_names = {
+        "rowid",
+        "type",
+        "group",
+        "estimate",
+        "std_error",
+        "p_value",
+        "s_value",
+        "conf_low",
+        "conf_high",
+        "term",
+        "contrast",
+        "statistic",
+    }
+    assert not (
+        set(out.columns) & reserved_names
+    ), f"Input data contain reserved column name(s) : {set(out.columns).intersection(reserved_names)}"
+
     datagrid_explicit = None
     if isinstance(out, pl.DataFrame) and hasattr(out, "datagrid_explicit"):
         datagrid_explicit = out.datagrid_explicit
 
     if isinstance(by, list) and len(by) > 0:
         by = [x for x in by if x in out.columns]
         if len(by) > 0:
@@ -258,14 +276,23 @@
 
         elif isinstance(value, (int, float)):
             if comparison not in elasticities:
                 lab = f"+{value}"
             hi = newdata[variable] + value / 2
             lo = newdata[variable] - value / 2
 
+        elif callable(value):
+            tmp = value(newdata[variable])
+            assert (
+                tmp.shape[1] == 2
+            ), f"The function passed to `variables` must return a DataFrame with two columns. Got {tmp.shape[1]}."
+            lo = tmp[:, 0]
+            hi = tmp[:, 1]
+            lab = "custom"
+
         else:
             raise ValueError(msg)
 
         out = [
             HiLo(
                 variable=variable,
                 lo=lo,
```

### Comparing `marginaleffects-0.0.8/marginaleffects/slopes.py` & `marginaleffects-0.0.9/marginaleffects/slopes.py`

 * *Files identical despite different names*

### Comparing `marginaleffects-0.0.8/marginaleffects/uncertainty.py` & `marginaleffects-0.0.9/marginaleffects/uncertainty.py`

 * *Files identical despite different names*

### Comparing `marginaleffects-0.0.8/marginaleffects/utils.py` & `marginaleffects-0.0.9/marginaleffects/utils.py`

 * *Files identical despite different names*

### Comparing `marginaleffects-0.0.8/pyproject.toml` & `marginaleffects-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "marginaleffects"
-version = "0.0.8"
+version = "0.0.9"
 description = ""
 authors = ["Vincent Arel-Bundock <vincent.arel-bundock@umontreal.ca>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 numpy = "^1.25.0"
```

### Comparing `marginaleffects-0.0.8/PKG-INFO` & `marginaleffects-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: marginaleffects
-Version: 0.0.8
+Version: 0.0.9
 Summary: 
 Author: Vincent Arel-Bundock
 Author-email: vincent.arel-bundock@umontreal.ca
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: numpy (>=1.25.0,<2.0.0)
 Requires-Dist: patsy (>0.5.0)
 Requires-Dist: plotnine (>0.12.3)
 Requires-Dist: polars (>0.20.1)
 Requires-Dist: pyarrow (>=14.0.1,<15.0.0)
 Requires-Dist: scipy (>=1.10.0,<2.0.0)
 Description-Content-Type: text/markdown
```

