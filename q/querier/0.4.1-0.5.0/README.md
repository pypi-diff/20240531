# Comparing `tmp/querier-0.4.1.tar.gz` & `tmp/querier-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/querier-0.4.1.tar", last modified: Sun Aug 21 11:52:15 2022, max compression
+gzip compressed data, was "querier-0.5.0.tar", last modified: Thu May 30 22:06:37 2024, max compression
```

## Comparing `querier-0.4.1.tar` & `querier-0.5.0.tar`

### file list

```diff
@@ -1,47 +1,51 @@
-drwxr-xr-x   0 t          (501) staff       (20)        0 2022-08-21 11:52:15.316001 querier-0.4.1/
--rw-r--r--   0 t          (501) staff       (20)     1690 2021-11-21 12:24:47.000000 querier-0.4.1/LICENSE
--rw-r--r--   0 t          (501) staff       (20)       42 2021-11-21 12:24:47.000000 querier-0.4.1/MANIFEST.in
--rw-r--r--   0 t          (501) staff       (20)      473 2022-08-21 11:52:15.316232 querier-0.4.1/PKG-INFO
--rw-r--r--   0 t          (501) staff       (20)     3522 2021-11-21 12:24:47.000000 querier-0.4.1/README.md
-drwxr-xr-x   0 t          (501) staff       (20)        0 2022-08-21 11:52:15.279623 querier-0.4.1/querier/
--rw-r--r--   0 t          (501) staff       (20)      481 2021-11-21 12:24:47.000000 querier-0.4.1/querier/__init__.py
-drwxr-xr-x   0 t          (501) staff       (20)        0 2022-08-21 11:52:15.297663 querier-0.4.1/querier/queries/
--rw-r--r--   0 t          (501) staff       (20)      404 2021-11-21 12:24:47.000000 querier-0.4.1/querier/queries/__init__.py
--rw-r--r--   0 t          (501) staff       (20)     1573 2021-11-21 12:24:47.000000 querier-0.4.1/querier/queries/concat.py
--rw-r--r--   0 t          (501) staff       (20)      807 2021-11-21 12:24:47.000000 querier-0.4.1/querier/queries/delete.py
--rw-r--r--   0 t          (501) staff       (20)      586 2021-11-21 12:24:47.000000 querier-0.4.1/querier/queries/drop.py
--rw-r--r--   0 t          (501) staff       (20)     2395 2021-11-21 12:24:47.000000 querier-0.4.1/querier/queries/filtr.py
--rw-r--r--   0 t          (501) staff       (20)     1221 2021-11-21 12:24:47.000000 querier-0.4.1/querier/queries/join.py
--rw-r--r--   0 t          (501) staff       (20)     2192 2021-11-21 12:24:47.000000 querier-0.4.1/querier/queries/request.py
--rw-r--r--   0 t          (501) staff       (20)     3900 2021-11-21 12:24:47.000000 querier-0.4.1/querier/queries/select.py
--rw-r--r--   0 t          (501) staff       (20)      996 2021-11-21 12:24:47.000000 querier-0.4.1/querier/queries/set.py
--rw-r--r--   0 t          (501) staff       (20)     1055 2021-11-21 12:24:47.000000 querier-0.4.1/querier/queries/summarize.py
--rw-r--r--   0 t          (501) staff       (20)      743 2021-11-21 12:24:47.000000 querier-0.4.1/querier/queries/update.py
-drwxr-xr-x   0 t          (501) staff       (20)        0 2022-08-21 11:52:15.309047 querier-0.4.1/querier/tests/
--rw-r--r--   0 t          (501) staff       (20)        0 2021-11-21 12:24:47.000000 querier-0.4.1/querier/tests/__init__.py
--rw-r--r--   0 t          (501) staff       (20)      887 2021-11-21 12:24:47.000000 querier-0.4.1/querier/tests/tests_concat.py
--rw-r--r--   0 t          (501) staff       (20)     1214 2021-11-21 12:24:47.000000 querier-0.4.1/querier/tests/tests_delete.py
--rw-r--r--   0 t          (501) staff       (20)     1056 2021-11-21 12:24:47.000000 querier-0.4.1/querier/tests/tests_drop.py
--rw-r--r--   0 t          (501) staff       (20)      760 2021-11-21 12:24:47.000000 querier-0.4.1/querier/tests/tests_filtr.py
--rw-r--r--   0 t          (501) staff       (20)     1054 2021-11-21 12:24:47.000000 querier-0.4.1/querier/tests/tests_join.py
--rw-r--r--   0 t          (501) staff       (20)     1403 2021-11-21 12:24:47.000000 querier-0.4.1/querier/tests/tests_request.py
--rw-r--r--   0 t          (501) staff       (20)      773 2021-11-21 12:24:47.000000 querier-0.4.1/querier/tests/tests_select.py
--rw-r--r--   0 t          (501) staff       (20)     1100 2021-11-21 12:24:47.000000 querier-0.4.1/querier/tests/tests_summarize.py
--rw-r--r--   0 t          (501) staff       (20)     1258 2021-11-21 12:24:47.000000 querier-0.4.1/querier/tests/tests_update.py
-drwxr-xr-x   0 t          (501) staff       (20)        0 2022-08-21 11:52:15.313629 querier-0.4.1/querier/utils/
--rw-r--r--   0 t          (501) staff       (20)      272 2021-11-21 12:24:47.000000 querier-0.4.1/querier/utils/__init__.py
--rw-r--r--   0 t          (501) staff       (20)      702 2021-11-21 12:24:47.000000 querier-0.4.1/querier/utils/deepcopy.py
--rw-r--r--   0 t          (501) staff       (20)      481 2021-11-21 12:24:47.000000 querier-0.4.1/querier/utils/memoize.py
--rw-r--r--   0 t          (501) staff       (20)     6308 2021-11-21 12:24:47.000000 querier-0.4.1/querier/utils/parse_request.py
-drwxr-xr-x   0 t          (501) staff       (20)        0 2022-08-21 11:52:15.314981 querier-0.4.1/querier/wrapper/
--rw-r--r--   0 t          (501) staff       (20)       51 2021-11-21 12:24:47.000000 querier-0.4.1/querier/wrapper/__init__.py
--rw-r--r--   0 t          (501) staff       (20)    12210 2021-11-21 12:24:47.000000 querier-0.4.1/querier/wrapper/wrapper.py
-drwxr-xr-x   0 t          (501) staff       (20)        0 2022-08-21 11:52:15.284975 querier-0.4.1/querier.egg-info/
--rw-r--r--   0 t          (501) staff       (20)      473 2022-08-21 11:52:15.000000 querier-0.4.1/querier.egg-info/PKG-INFO
--rw-r--r--   0 t          (501) staff       (20)      981 2022-08-21 11:52:15.000000 querier-0.4.1/querier.egg-info/SOURCES.txt
--rw-r--r--   0 t          (501) staff       (20)        1 2022-08-21 11:52:15.000000 querier-0.4.1/querier.egg-info/dependency_links.txt
--rw-r--r--   0 t          (501) staff       (20)      196 2022-08-21 11:52:15.000000 querier-0.4.1/querier.egg-info/requires.txt
--rw-r--r--   0 t          (501) staff       (20)        8 2022-08-21 11:52:15.000000 querier-0.4.1/querier.egg-info/top_level.txt
--rw-r--r--   0 t          (501) staff       (20)      196 2022-08-21 11:34:37.000000 querier-0.4.1/requirements.txt
--rw-r--r--   0 t          (501) staff       (20)      147 2022-08-21 11:52:15.317218 querier-0.4.1/setup.cfg
--rw-r--r--   0 t          (501) staff       (20)     1116 2022-08-21 11:39:44.000000 querier-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:06:37.036076 querier-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-05-30 22:06:28.000000 querier-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-30 22:06:28.000000 querier-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-30 22:06:37.036076 querier-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-05-30 22:06:28.000000 querier-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:06:37.028076 querier-0.5.0/querier/
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-30 22:06:28.000000 querier-0.5.0/querier/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:06:37.028076 querier-0.5.0/querier/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-30 22:06:28.000000 querier-0.5.0/querier/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-30 22:06:28.000000 querier-0.5.0/querier/datasets/download.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:06:37.032076 querier-0.5.0/querier/queries/
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-30 22:06:28.000000 querier-0.5.0/querier/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-30 22:06:28.000000 querier-0.5.0/querier/queries/concat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-30 22:06:28.000000 querier-0.5.0/querier/queries/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-30 22:06:28.000000 querier-0.5.0/querier/queries/drop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-05-30 22:06:28.000000 querier-0.5.0/querier/queries/filtr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-30 22:06:28.000000 querier-0.5.0/querier/queries/join.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-05-30 22:06:28.000000 querier-0.5.0/querier/queries/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5015 2024-05-30 22:06:28.000000 querier-0.5.0/querier/queries/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-30 22:06:28.000000 querier-0.5.0/querier/queries/set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-30 22:06:28.000000 querier-0.5.0/querier/queries/summarize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-30 22:06:28.000000 querier-0.5.0/querier/queries/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:06:37.032076 querier-0.5.0/querier/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 22:06:28.000000 querier-0.5.0/querier/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-30 22:06:28.000000 querier-0.5.0/querier/tests/tests_concat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-30 22:06:28.000000 querier-0.5.0/querier/tests/tests_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-30 22:06:28.000000 querier-0.5.0/querier/tests/tests_drop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-30 22:06:28.000000 querier-0.5.0/querier/tests/tests_filtr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-30 22:06:28.000000 querier-0.5.0/querier/tests/tests_join.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-30 22:06:28.000000 querier-0.5.0/querier/tests/tests_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-30 22:06:28.000000 querier-0.5.0/querier/tests/tests_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-30 22:06:28.000000 querier-0.5.0/querier/tests/tests_summarize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-30 22:06:28.000000 querier-0.5.0/querier/tests/tests_update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:06:37.032076 querier-0.5.0/querier/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-30 22:06:28.000000 querier-0.5.0/querier/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-30 22:06:28.000000 querier-0.5.0/querier/utils/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-30 22:06:28.000000 querier-0.5.0/querier/utils/deepcopy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-30 22:06:28.000000 querier-0.5.0/querier/utils/memoize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6308 2024-05-30 22:06:28.000000 querier-0.5.0/querier/utils/parse_request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:06:37.032076 querier-0.5.0/querier/wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-30 22:06:28.000000 querier-0.5.0/querier/wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-30 22:06:28.000000 querier-0.5.0/querier/wrapper/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:06:37.036076 querier-0.5.0/querier.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-30 22:06:36.000000 querier-0.5.0/querier.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-30 22:06:37.000000 querier-0.5.0/querier.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 22:06:36.000000 querier-0.5.0/querier.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-30 22:06:36.000000 querier-0.5.0/querier.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-30 22:06:36.000000 querier-0.5.0/querier.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-30 22:06:28.000000 querier-0.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-30 22:06:37.036076 querier-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-30 22:06:28.000000 querier-0.5.0/setup.py
```

### Comparing `querier-0.4.1/LICENSE` & `querier-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `querier-0.4.1/README.md` & `querier-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `querier-0.4.1/querier/queries/concat.py` & `querier-0.5.0/querier/queries/concat.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # Authors: Thierry Moudiki
 #
 # License: BSD 3
 
 
 import pandas as pd
+import polars as pl
 import numpy as np
-from ..utils import memoize
+from ..utils import polars_to_pandas, pandas_to_polars
+
 
 
 # df1 = pd.DataFrame({'key': ['A', 'B', 'C', 'D'],
 #                     'value': np.random.randn(4)})
 # df2 = pd.DataFrame({'key': ['B', 'D', 'D', 'E'],
 #                    'value': np.random.randn(4)})
 # print(concat(df1, df2, axis="h"))
-@memoize
+
 def concat(df1, df2, axis="h", **kwargs):
     """Concatenate data frames.
        
     Args:           
         
         df1: a data frame
             a data frame
@@ -32,32 +34,42 @@
            
         https://github.com/thierrymoudiki/querier/tree/master/querier/demo
        
     """
 
     assert axis in ("h", "v"), "must have axis in ('h', 'v')"
 
+    if isinstance(df1, pl.DataFrame):
+        df1 = polars_to_pandas(df1)
+    
+    if isinstance(df2, pl.DataFrame):
+        df2 = polars_to_pandas(df2)
+
     if axis == "h":
 
         assert (
             len(
                 np.intersect1d(df1.columns.values, np.array(["key2", "value2"]))
             )
             == 0
         ), "df1 and df2 must have different column names (try function join instead)"
 
         df = pd.DataFrame(np.hstack((df1, df2)))
 
         df.columns = np.append(df1.columns.values, df2.columns.values)
 
+        if isinstance(df1, pl.DataFrame):
+            return polars_to_pandas(df)
         return df
 
     # if axis == "v":
     assert (
         df1.columns.values == df2.columns.values
     ).all(), "must have: df1.columns == df2.columns"
 
     df = pd.DataFrame(np.vstack((df1, df2)))
 
     df.columns = df1.columns.values
 
+    if isinstance(df1, pl.DataFrame):
+        return polars_to_pandas(df)
     return df.drop_duplicates()
```

### Comparing `querier-0.4.1/querier/queries/delete.py` & `querier-0.5.0/querier/queries/delete.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # Authors: Thierry Moudiki
 #
 # License: BSD 3
 
 
 import numpy as np
+import polars as pl
 from ..utils import parse_request
-from ..utils import memoize
+from ..utils import polars_to_pandas, pandas_to_polars
 
 
 # delete(df, 'tip > 1.5')
 # delete(df, '(size == 2) | (size == 3)')
-@memoize
-def delete(df, req=None):
+
+def delete(df, req):
     """Delete rows from a data frame.
        
     Args:           
         
         df: a data frame 
             a data frame
                
@@ -24,17 +25,23 @@
                                  
     Examples:    
            
         https://github.com/thierrymoudiki/querier/tree/master/querier/demo
        
     """
 
-    if req is None:  # useless tho...
-
-        return df
+    if isinstance(df, pl.DataFrame):
+            
+        df = polars_to_pandas(df)
 
     # if request is not None:
     n, p = df.shape
 
     str_conds = parse_request(req)
 
-    return df[np.logical_not(eval(str_conds).values)]
+    result = df[np.logical_not(eval(str_conds).values)]
+
+    if isinstance(df, pl.DataFrame):
+
+        return pandas_to_polars(result)
+
+    return result
```

### Comparing `querier-0.4.1/querier/queries/drop.py` & `querier-0.5.0/querier/queries/drop.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # Authors: Thierry Moudiki
 #
 # License: BSD 3
 
-
-from ..utils import memoize
+import pandas as pd
+import polars as pl
+from ..utils import polars_to_pandas, pandas_to_polars
 
 # creates a copy
-@memoize
+
 def drop(df, req=None):
     """ Drop columns.
        
     Args: 
        
         req: str
             comma-separated list of columns to be dropped
@@ -18,12 +19,20 @@
     Examples:     
        
         https://github.com/thierrymoudiki/querier/tree/master/querier/demo
        
     """
 
     try:
-        return df.drop(req.replace(" ", "").split(","), axis=1)
+        if isinstance(df, pl.DataFrame):
+            df = polars_to_pandas(df)
+
+        result = df.drop(req.replace(" ", "").split(","), axis=1)
+
+        if isinstance(df, pl.DataFrame):
+            return pandas_to_polars(result)
+
+        return result
     except:
         raise ValueError(
             "request must contain df" "s column names (comma-separated)"
         )
```

### Comparing `querier-0.4.1/querier/queries/join.py` & `querier-0.5.0/querier/queries/join.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # Authors: Thierry Moudiki
 #
 # License: BSD 3
 
 
 import pandas as pd
-from ..utils import memoize
-
+import polars as pl
+from ..utils import polars_to_pandas, pandas_to_polars
 
 # just for 'completeness' of the interface
 # already straightforward in pd
 
 # df1 = pd.DataFrame({'key': ['A', 'B', 'C', 'D'],
 #                     'value': np.random.randn(4)})
 # df2 = pd.DataFrame({'key': ['B', 'D', 'D', 'E'],
 #                    'value': np.random.randn(4)})
 # join(df1, df2, on='key')
 # join(df1, df2, 'key', "left")
 # join(df1, df2, 'key', "right")
 # join(df1, df2, 'key', "outer")
-@memoize
+
 def join(df1, df2, on=None, type_join="inner", **kwargs):
     """ Join data frames.
    
     Args:
     
         df1: a data frame           
            a data frame
@@ -41,8 +41,17 @@
        
         https://github.com/thierrymoudiki/querier/tree/master/querier/demo
    
    """
     if on is not None:
         on_ = on.replace(" ", "").split(",")
 
-    return pd.merge(df1, df2, on=on_, how=type_join, **kwargs)
+    if isinstance(df1, pl.DataFrame):
+         df1 = polars_to_pandas(df1)
+         df2 = polars_to_pandas(df2)
+
+    result = pd.merge(df1, df2, on=on_, how=type_join, **kwargs)
+
+    if isinstance(df1, pl.DataFrame):
+        return pandas_to_polars(result)
+    
+    return result
```

### Comparing `querier-0.4.1/querier/queries/request.py` & `querier-0.5.0/querier/queries/request.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 # Authors: Thierry Moudiki
 #
 # License: BSD 3
 
 
 import pandas as pd
-from sqlalchemy import create_engine
+import polars as pl
+from sqlalchemy import create_engine, text 
 from ..utils import parse_cols_request
-from ..utils import memoize
+from ..utils import polars_to_pandas, pandas_to_polars
+
 
 # request(df, "SELECT tip, smoker, day FROM df WHERE tip > 25")
 # request(df, "SELECT tip, smoker, day, size FROM df WHERE (tip > 2) and (size > 4)")
 # request(df, "SELECT tip, smoker, day, size FROM df WHERE (tip > 2) and (size > 4) and (day like 'Thur')")
 # request(df, "SELECT tip, smoker, day, size FROM df WHERE (tip > 2) and (size > 4) and (day not like 'Thur')")
 # request(df, "SELECT SUM(tip), smoker FROM df WHERE tip > 20 GROUP BY smoker")
 # request(df, "SELECT AVG(tip), size, smoker FROM df WHERE tip > 20 GROUP BY size")
 # request(df, "SELECT AVG(tip) as avg_tip, size, smoker FROM df WHERE tip > 20 GROUP BY size")
 # request(df, "SELECT avg(tip) as avg_tip, AVG(size) as   avg_size, smoker FROM df WHERE tip > 20 GROUP BY size, tip")
 # request(df, "SELECT SUM(tip), smoker FROM df GROUP BY smoker having tip > 1.5")
-@memoize
-def request(df, req=None, **kwargs):
+
+def request(df, req, **kwargs):
     """ SQL request on a data frame.
        
     Args:           
     
         df: a data frame
             a data frame
            
@@ -32,18 +34,14 @@
            
     Examples:           
            
         https://github.com/thierrymoudiki/querier/tree/master/querier/demo
        
     """
 
-    if req is None:  # useless tho...
-
-        return df
-
     # if req is not None:
     assert (
         "UPDATE".lower() not in req.lower()
     ), "'UPDATE' is forbidden here, try querier.update"
 
     assert (
         "DELETE".lower() not in req.lower()
@@ -53,16 +51,18 @@
         "DROP".lower() not in req.lower()
     ), "'DROP' is forbidden here, try querier.drop"
 
     try:
 
         engine = create_engine("sqlite://", echo=False)
         df.to_sql("df", con=engine, **kwargs)
-        req_res = engine.execute(req.upper()).fetchall()
+        with engine.connect() as conn:
+            req_res = conn.execute(text(req.upper())).fetchall()
         col_names = parse_cols_request(req)
-        df_res = pd.DataFrame(req_res, columns=col_names)
-
-        return df_res
+        result = pd.DataFrame(req_res, columns=col_names)
+        if isinstance(df, pl.DataFrame):
+            return(pandas_to_polars(result))
+        return result
 
     except:
 
         raise ValueError("invalid request: check SQL syntax")
```

### Comparing `querier-0.4.1/querier/queries/set.py` & `querier-0.5.0/querier/queries/set.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 #
 # License: BSD 3 Clause Clear
 
 
 import numpy as np
 import pickle
 import warnings
+import pandas as pd
+import polars as pl
+from ..utils import polars_to_pandas, pandas_to_polars
 
 warnings.filterwarnings("ignore")
 
 def setwhere(df, col, val, replace, copy=False):
     """ Set value.
    
     Args:
@@ -30,16 +33,26 @@
            If True, a new data frame is created else input data frame is modified (default False)
        
     Examples: 
        
         https://github.com/thierrymoudiki/querier/tree/master/querier/demo
    
     """
+
+    is_polars = False
     
+    if isinstance(df, pl.DataFrame):
+        is_polars = True
+        df = polars_to_pandas(df)
+
     if copy is True:        
-        df_ = pickle.loads(pickle.dumps(df, -1))
-        df_[col][np.where(df[col] == val)[0]] = replace       
-        return df_
+      df_ = pickle.loads(pickle.dumps(df, -1))
+      df_[col][np.where(df[col] == val)[0]] = replace       
+      if is_polars:
+         return pandas_to_polars(df_)
+      return df_
     
     # copy == False:    
-    df[col][np.where(df[col] == val)[0]] = replace       
+    df[col][np.where(df[col] == val)[0]] = replace
+    if is_polars:
+        return pandas_to_polars(df)       
     return df
```

### Comparing `querier-0.4.1/querier/queries/update.py` & `querier-0.5.0/querier/queries/update.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # Authors: Thierry Moudiki
 #
 # License: BSD 3
 
-
+import pandas as pd
+import polars as pl
 from ..utils import parse_update_request
+from ..utils import polars_to_pandas, pandas_to_polars
 
 # modifies input df (!)
 # update(df, 'tip = 2*tip')
 # update(df, "toto = 3*tip")
 # update(df, 'tip = np.mean(tip)')
 # update(df, 'toto = np.mean(tip)')
-def update(df, req=None):
+def update(df, req):
     """ Update the data frame.
    
     Args:           
 
         df: a data frame
             a data frame
        
@@ -22,16 +24,20 @@
             specifying the transformation, e.g `new_size = 3*size`
                  
     Examples: 
    
         https://github.com/thierrymoudiki/querier/tree/master/querier/demo
    
     """
+    
+    is_polars = False
 
-    if req is None:  # useless tho...
-
-        return df
+    if isinstance(df, pl.DataFrame):
+        is_polars = True
+        df = polars_to_pandas(df)
 
     # if request is not None:
     exec(parse_update_request(req), {"df": df})
 
+    if is_polars:
+        return pandas_to_polars(df)
     return df
```

### Comparing `querier-0.4.1/querier/tests/tests_concat.py` & `querier-0.5.0/querier/tests/tests_concat.py`

 * *Files identical despite different names*

### Comparing `querier-0.4.1/querier/tests/tests_delete.py` & `querier-0.5.0/querier/tests/tests_delete.py`

 * *Files identical despite different names*

### Comparing `querier-0.4.1/querier/tests/tests_drop.py` & `querier-0.5.0/querier/tests/tests_drop.py`

 * *Files identical despite different names*

### Comparing `querier-0.4.1/querier/tests/tests_filtr.py` & `querier-0.5.0/querier/tests/tests_filtr.py`

 * *Files identical despite different names*

### Comparing `querier-0.4.1/querier/tests/tests_join.py` & `querier-0.5.0/querier/tests/tests_join.py`

 * *Files identical despite different names*

### Comparing `querier-0.4.1/querier/tests/tests_request.py` & `querier-0.5.0/querier/tests/tests_request.py`

 * *Files identical despite different names*

### Comparing `querier-0.4.1/querier/tests/tests_select.py` & `querier-0.5.0/querier/tests/tests_select.py`

 * *Files identical despite different names*

### Comparing `querier-0.4.1/querier/tests/tests_summarize.py` & `querier-0.5.0/querier/tests/tests_summarize.py`

 * *Files identical despite different names*

### Comparing `querier-0.4.1/querier/tests/tests_update.py` & `querier-0.5.0/querier/tests/tests_update.py`

 * *Files identical despite different names*

### Comparing `querier-0.4.1/querier/utils/deepcopy.py` & `querier-0.5.0/querier/utils/deepcopy.py`

 * *Files identical despite different names*

### Comparing `querier-0.4.1/querier/utils/parse_request.py` & `querier-0.5.0/querier/utils/parse_request.py`

 * *Files identical despite different names*

### Comparing `querier-0.4.1/querier/wrapper/wrapper.py` & `querier-0.5.0/querier/wrapper/wrapper.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,33 +2,33 @@
 
 # Authors: Thierry Moudiki
 #
 # License: BSD 3
 
 
 import pandas as pd
-from sklearn.base import BaseEstimator
+import polars as pl
 import sqlite3
 from pymongo import MongoClient
-
+from ..utils import polars_to_pandas, pandas_to_polars
 from ..queries import (
     select as select_,
     update as update_,
     delete as delete_,
     concat as concat_,
     filtr as filtr_,
     join as join_,
     summarize as summarize_,
     drop as drop_,
     request as request_,
     setwhere as setwhere_,
 )
 
 
-class Querier(BaseEstimator):
+class Querier(object):
     """ A wrapper for chaining the querier's atomic operations, which are currently:
        `concat`, `delete`, `drop`, `filtr`, `join`, `select`, `summarize`,
        `update`, `request`
        
     Attributes: 
        
         df: a data frame
@@ -47,15 +47,15 @@
        
         https://github.com/thierrymoudiki/querier/tree/master/querier/demo
        
     """
 
     def __init__(self, df=None, source=None, db=None, table=None, **kwargs):
 
-        if (df is not None) & isinstance(df, pd.DataFrame):
+        if (df is not None):
 
             assert (source is None) & (
                 table is None
             ), "No `source` required when `df` is provided"
 
             self.df = df
 
@@ -249,15 +249,15 @@
        
        """
 
         assert isinstance(df2, pd.DataFrame), "'df2' must be a data frame"
         self.df = concat_(self.df, df2, axis, **kwargs)
         return self
 
-    def filtr(self, req=None, limit=None, random=False, seed=123):
+    def filtr(self, req, limit=None, random=False, seed=123):
         """ Filter rows, based on given criteria.
        
         Args:           
         
             req: str
                criteria for filtering the rows
 
@@ -296,20 +296,18 @@
            
            
         Examples:        
            
             https://github.com/thierrymoudiki/querier/tree/master/querier/demo
        
        """
-
-        assert isinstance(df2, pd.DataFrame), "'df2' must be a data frame"
         self.df = join_(self.df, df2, on, type_join, **kwargs)
         return self
 
-    def summarize(self, req=None, group_by=None, having=None, **kwargs):
+    def summarize(self, req, group_by=None, having=None, **kwargs):
         """ Data summaries on rows.
        
         Args:           
             
             req: str
                specifying the aggregating operations on columns
            
@@ -324,15 +322,15 @@
             https://github.com/thierrymoudiki/querier/tree/master/querier/demo
        
        """
 
         self.df = summarize_(self.df, req, group_by, having, **kwargs)
         return self
 
-    def drop(self, req=None):
+    def drop(self, req):
         """ Drop columns.
        
         Args:           
         
             req: str
                comma-separated list of columns to be dropped                      
            
@@ -341,15 +339,15 @@
             https://github.com/thierrymoudiki/querier/tree/master/querier/demo
        
        """
 
         self.df = drop_(self.df, req)
         return self
 
-    def request(self, req=None, **kwargs):
+    def request(self, req, **kwargs):
         """ SQL request on the data frame.
        
         Args:           
         
             req: str
                 specifying the SQL request
```

### Comparing `querier-0.4.1/querier.egg-info/SOURCES.txt` & `querier-0.5.0/querier.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 setup.py
 querier/__init__.py
 querier.egg-info/PKG-INFO
 querier.egg-info/SOURCES.txt
 querier.egg-info/dependency_links.txt
 querier.egg-info/requires.txt
 querier.egg-info/top_level.txt
+querier/datasets/__init__.py
+querier/datasets/download.py
 querier/queries/__init__.py
 querier/queries/concat.py
 querier/queries/delete.py
 querier/queries/drop.py
 querier/queries/filtr.py
 querier/queries/join.py
 querier/queries/request.py
@@ -28,12 +30,13 @@
 querier/tests/tests_filtr.py
 querier/tests/tests_join.py
 querier/tests/tests_request.py
 querier/tests/tests_select.py
 querier/tests/tests_summarize.py
 querier/tests/tests_update.py
 querier/utils/__init__.py
+querier/utils/convert.py
 querier/utils/deepcopy.py
 querier/utils/memoize.py
 querier/utils/parse_request.py
 querier/wrapper/__init__.py
 querier/wrapper/wrapper.py
```

### Comparing `querier-0.4.1/setup.py` & `querier-0.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 from codecs import open
 from os import path
 
-__version__ = '0.4.1'
+__version__ = '0.5.0'
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 # get the dependencies and installs
 here = path.abspath(path.dirname(__file__))
 with open(path.join(here, 'requirements.txt'), encoding='utf-8') as f:
```

