# Comparing `tmp/dask_expr-1.1.1.tar.gz` & `tmp/dask_expr-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dask_expr-1.1.1.tar", last modified: Fri May 17 20:08:08 2024, max compression
+gzip compressed data, was "dask_expr-1.1.2.tar", last modified: Fri May 31 21:11:46 2024, max compression
```

## Comparing `dask_expr-1.1.1.tar` & `dask_expr-1.1.2.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-05-17 20:08:08.032506 dask_expr-1.1.1/
--rw-r--r--   0 james      (501) staff       (20)     1516 2024-04-01 19:20:57.000000 dask_expr-1.1.1/LICENSE.txt
--rw-r--r--   0 james      (501) staff       (20)     2415 2024-05-17 20:08:08.032416 dask_expr-1.1.1/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)     1347 2024-05-03 20:30:23.000000 dask_expr-1.1.1/README.md
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-05-17 20:08:08.032913 dask_expr-1.1.1/dask_expr/
--rw-r--r--   0 james      (501) staff       (20)      714 2024-04-01 19:20:57.000000 dask_expr-1.1.1/dask_expr/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     3495 2024-04-01 19:20:57.000000 dask_expr-1.1.1/dask_expr/_accessor.py
--rw-r--r--   0 james      (501) staff       (20)     3089 2024-04-01 19:20:57.000000 dask_expr-1.1.1/dask_expr/_backends.py
--rw-r--r--   0 james      (501) staff       (20)     5913 2024-04-01 19:20:57.000000 dask_expr-1.1.1/dask_expr/_categorical.py
--rw-r--r--   0 james      (501) staff       (20)   231004 2024-05-17 19:52:39.000000 dask_expr-1.1.1/dask_expr/_collection.py
--rw-r--r--   0 james      (501) staff       (20)    12014 2024-04-01 19:20:57.000000 dask_expr-1.1.1/dask_expr/_concat.py
--rw-r--r--   0 james      (501) staff       (20)    23493 2024-05-17 19:52:39.000000 dask_expr-1.1.1/dask_expr/_core.py
--rw-r--r--   0 james      (501) staff       (20)     3402 2024-04-01 19:20:57.000000 dask_expr-1.1.1/dask_expr/_cumulative.py
--rw-r--r--   0 james      (501) staff       (20)     1423 2024-04-01 19:20:57.000000 dask_expr-1.1.1/dask_expr/_datetime.py
--rw-r--r--   0 james      (501) staff       (20)     3125 2024-04-01 19:20:57.000000 dask_expr-1.1.1/dask_expr/_describe.py
--rw-r--r--   0 james      (501) staff       (20)      123 2024-04-01 19:20:57.000000 dask_expr-1.1.1/dask_expr/_dispatch.py
--rw-r--r--   0 james      (501) staff       (20)     5641 2024-05-03 20:30:23.000000 dask_expr-1.1.1/dask_expr/_dummies.py
--rw-r--r--   0 james      (501) staff       (20)   125381 2024-05-17 19:52:39.000000 dask_expr-1.1.1/dask_expr/_expr.py
--rw-r--r--   0 james      (501) staff       (20)    68056 2024-05-03 20:30:23.000000 dask_expr-1.1.1/dask_expr/_groupby.py
--rw-r--r--   0 james      (501) staff       (20)    12215 2024-05-03 20:30:23.000000 dask_expr-1.1.1/dask_expr/_indexing.py
--rw-r--r--   0 james      (501) staff       (20)    32183 2024-04-19 21:01:12.000000 dask_expr-1.1.1/dask_expr/_merge.py
--rw-r--r--   0 james      (501) staff       (20)    11712 2024-04-01 19:20:57.000000 dask_expr-1.1.1/dask_expr/_merge_asof.py
--rw-r--r--   0 james      (501) staff       (20)     3903 2024-04-01 19:20:57.000000 dask_expr-1.1.1/dask_expr/_quantile.py
--rw-r--r--   0 james      (501) staff       (20)     2491 2024-04-01 19:20:57.000000 dask_expr-1.1.1/dask_expr/_quantiles.py
--rw-r--r--   0 james      (501) staff       (20)    44935 2024-05-03 20:30:23.000000 dask_expr-1.1.1/dask_expr/_reductions.py
--rw-r--r--   0 james      (501) staff       (20)    17307 2024-04-19 21:01:12.000000 dask_expr-1.1.1/dask_expr/_repartition.py
--rw-r--r--   0 james      (501) staff       (20)     7020 2024-04-01 19:20:57.000000 dask_expr-1.1.1/dask_expr/_resample.py
--rw-r--r--   0 james      (501) staff       (20)     8765 2024-04-01 19:20:57.000000 dask_expr-1.1.1/dask_expr/_rolling.py
--rw-r--r--   0 james      (501) staff       (20)    43922 2024-05-17 19:52:39.000000 dask_expr-1.1.1/dask_expr/_shuffle.py
--rw-r--r--   0 james      (501) staff       (20)     5022 2024-04-01 19:20:57.000000 dask_expr-1.1.1/dask_expr/_str_accessor.py
--rw-r--r--   0 james      (501) staff       (20)     7029 2024-05-17 19:52:39.000000 dask_expr-1.1.1/dask_expr/_util.py
--rw-r--r--   0 james      (501) staff       (20)      497 2024-05-17 20:08:08.032953 dask_expr-1.1.1/dask_expr/_version.py
--rw-r--r--   0 james      (501) staff       (20)     6636 2024-04-01 19:20:57.000000 dask_expr-1.1.1/dask_expr/datasets.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-05-17 20:08:08.028967 dask_expr-1.1.1/dask_expr/diagnostics/
--rw-r--r--   0 james      (501) staff       (20)      136 2024-04-01 19:20:57.000000 dask_expr-1.1.1/dask_expr/diagnostics/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     5099 2024-04-19 21:01:12.000000 dask_expr-1.1.1/dask_expr/diagnostics/_analyze.py
--rw-r--r--   0 james      (501) staff       (20)     3943 2024-04-01 19:20:57.000000 dask_expr-1.1.1/dask_expr/diagnostics/_analyze_plugin.py
--rw-r--r--   0 james      (501) staff       (20)     2793 2024-04-19 21:01:12.000000 dask_expr-1.1.1/dask_expr/diagnostics/_explain.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-05-17 20:08:08.031832 dask_expr-1.1.1/dask_expr/io/
--rw-r--r--   0 james      (501) staff       (20)       96 2024-04-01 19:20:51.000000 dask_expr-1.1.1/dask_expr/io/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     3955 2024-05-03 20:30:23.000000 dask_expr-1.1.1/dask_expr/io/_delayed.py
--rw-r--r--   0 james      (501) staff       (20)      171 2024-04-01 19:20:57.000000 dask_expr-1.1.1/dask_expr/io/bag.py
--rw-r--r--   0 james      (501) staff       (20)     8975 2024-05-17 19:52:39.000000 dask_expr-1.1.1/dask_expr/io/csv.py
--rw-r--r--   0 james      (501) staff       (20)     4366 2024-05-03 20:30:23.000000 dask_expr-1.1.1/dask_expr/io/hdf.py
--rw-r--r--   0 james      (501) staff       (20)    19469 2024-05-17 19:52:39.000000 dask_expr-1.1.1/dask_expr/io/io.py
--rw-r--r--   0 james      (501) staff       (20)     6474 2024-05-03 20:30:23.000000 dask_expr-1.1.1/dask_expr/io/json.py
--rw-r--r--   0 james      (501) staff       (20)     2410 2024-04-19 21:01:12.000000 dask_expr-1.1.1/dask_expr/io/orc.py
--rw-r--r--   0 james      (501) staff       (20)    69913 2024-05-17 19:52:39.000000 dask_expr-1.1.1/dask_expr/io/parquet.py
--rw-r--r--   0 james      (501) staff       (20)      482 2024-05-03 20:30:23.000000 dask_expr-1.1.1/dask_expr/io/records.py
--rw-r--r--   0 james      (501) staff       (20)    13147 2024-05-03 20:30:23.000000 dask_expr-1.1.1/dask_expr/io/sql.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-05-17 20:08:08.032151 dask_expr-1.1.1/dask_expr.egg-info/
--rw-r--r--   0 james      (501) staff       (20)     2415 2024-05-17 20:08:08.000000 dask_expr-1.1.1/dask_expr.egg-info/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)     1239 2024-05-17 20:08:08.000000 dask_expr-1.1.1/dask_expr.egg-info/SOURCES.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2024-05-17 20:08:08.000000 dask_expr-1.1.1/dask_expr.egg-info/dependency_links.txt
--rw-r--r--   0 james      (501) staff       (20)       40 2024-05-17 20:08:08.000000 dask_expr-1.1.1/dask_expr.egg-info/requires.txt
--rw-r--r--   0 james      (501) staff       (20)       10 2024-05-17 20:08:08.000000 dask_expr-1.1.1/dask_expr.egg-info/top_level.txt
--rw-r--r--   0 james      (501) staff       (20)     2195 2024-05-17 19:56:34.000000 dask_expr-1.1.1/pyproject.toml
--rw-r--r--   0 james      (501) staff       (20)      230 2024-05-17 20:08:08.032781 dask_expr-1.1.1/setup.cfg
--rwxr-xr-x   0 james      (501) staff       (20)      194 2024-04-01 19:20:57.000000 dask_expr-1.1.1/setup.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-05-31 21:11:46.917201 dask_expr-1.1.2/
+-rw-r--r--   0 james      (501) staff       (20)     1516 2024-04-01 19:20:57.000000 dask_expr-1.1.2/LICENSE.txt
+-rw-r--r--   0 james      (501) staff       (20)     2415 2024-05-31 21:11:46.917100 dask_expr-1.1.2/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)     1347 2024-05-03 20:30:23.000000 dask_expr-1.1.2/README.md
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-05-31 21:11:46.917852 dask_expr-1.1.2/dask_expr/
+-rw-r--r--   0 james      (501) staff       (20)      714 2024-04-01 19:20:57.000000 dask_expr-1.1.2/dask_expr/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     3813 2024-05-31 20:51:25.000000 dask_expr-1.1.2/dask_expr/_accessor.py
+-rw-r--r--   0 james      (501) staff       (20)     3089 2024-04-01 19:20:57.000000 dask_expr-1.1.2/dask_expr/_backends.py
+-rw-r--r--   0 james      (501) staff       (20)     5913 2024-04-01 19:20:57.000000 dask_expr-1.1.2/dask_expr/_categorical.py
+-rw-r--r--   0 james      (501) staff       (20)   231004 2024-05-31 20:51:22.000000 dask_expr-1.1.2/dask_expr/_collection.py
+-rw-r--r--   0 james      (501) staff       (20)    12014 2024-04-01 19:20:57.000000 dask_expr-1.1.2/dask_expr/_concat.py
+-rw-r--r--   0 james      (501) staff       (20)    23493 2024-05-17 19:52:39.000000 dask_expr-1.1.2/dask_expr/_core.py
+-rw-r--r--   0 james      (501) staff       (20)     3402 2024-04-01 19:20:57.000000 dask_expr-1.1.2/dask_expr/_cumulative.py
+-rw-r--r--   0 james      (501) staff       (20)     1423 2024-04-01 19:20:57.000000 dask_expr-1.1.2/dask_expr/_datetime.py
+-rw-r--r--   0 james      (501) staff       (20)     3125 2024-04-01 19:20:57.000000 dask_expr-1.1.2/dask_expr/_describe.py
+-rw-r--r--   0 james      (501) staff       (20)      123 2024-04-01 19:20:57.000000 dask_expr-1.1.2/dask_expr/_dispatch.py
+-rw-r--r--   0 james      (501) staff       (20)     5641 2024-05-03 20:30:23.000000 dask_expr-1.1.2/dask_expr/_dummies.py
+-rw-r--r--   0 james      (501) staff       (20)   125395 2024-05-31 20:51:25.000000 dask_expr-1.1.2/dask_expr/_expr.py
+-rw-r--r--   0 james      (501) staff       (20)    68056 2024-05-03 20:30:23.000000 dask_expr-1.1.2/dask_expr/_groupby.py
+-rw-r--r--   0 james      (501) staff       (20)    12215 2024-05-03 20:30:23.000000 dask_expr-1.1.2/dask_expr/_indexing.py
+-rw-r--r--   0 james      (501) staff       (20)    32183 2024-04-19 21:01:12.000000 dask_expr-1.1.2/dask_expr/_merge.py
+-rw-r--r--   0 james      (501) staff       (20)    11712 2024-04-01 19:20:57.000000 dask_expr-1.1.2/dask_expr/_merge_asof.py
+-rw-r--r--   0 james      (501) staff       (20)     3903 2024-04-01 19:20:57.000000 dask_expr-1.1.2/dask_expr/_quantile.py
+-rw-r--r--   0 james      (501) staff       (20)     2491 2024-04-01 19:20:57.000000 dask_expr-1.1.2/dask_expr/_quantiles.py
+-rw-r--r--   0 james      (501) staff       (20)    44935 2024-05-03 20:30:23.000000 dask_expr-1.1.2/dask_expr/_reductions.py
+-rw-r--r--   0 james      (501) staff       (20)    17307 2024-04-19 21:01:12.000000 dask_expr-1.1.2/dask_expr/_repartition.py
+-rw-r--r--   0 james      (501) staff       (20)     7020 2024-04-01 19:20:57.000000 dask_expr-1.1.2/dask_expr/_resample.py
+-rw-r--r--   0 james      (501) staff       (20)     8765 2024-04-01 19:20:57.000000 dask_expr-1.1.2/dask_expr/_rolling.py
+-rw-r--r--   0 james      (501) staff       (20)    43968 2024-05-23 18:26:23.000000 dask_expr-1.1.2/dask_expr/_shuffle.py
+-rw-r--r--   0 james      (501) staff       (20)     5022 2024-04-01 19:20:57.000000 dask_expr-1.1.2/dask_expr/_str_accessor.py
+-rw-r--r--   0 james      (501) staff       (20)     7029 2024-05-17 19:52:39.000000 dask_expr-1.1.2/dask_expr/_util.py
+-rw-r--r--   0 james      (501) staff       (20)      497 2024-05-31 21:11:46.917931 dask_expr-1.1.2/dask_expr/_version.py
+-rw-r--r--   0 james      (501) staff       (20)     6636 2024-04-01 19:20:57.000000 dask_expr-1.1.2/dask_expr/datasets.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-05-31 21:11:46.913351 dask_expr-1.1.2/dask_expr/diagnostics/
+-rw-r--r--   0 james      (501) staff       (20)      136 2024-04-01 19:20:57.000000 dask_expr-1.1.2/dask_expr/diagnostics/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     5099 2024-04-19 21:01:12.000000 dask_expr-1.1.2/dask_expr/diagnostics/_analyze.py
+-rw-r--r--   0 james      (501) staff       (20)     3943 2024-04-01 19:20:57.000000 dask_expr-1.1.2/dask_expr/diagnostics/_analyze_plugin.py
+-rw-r--r--   0 james      (501) staff       (20)     2793 2024-04-19 21:01:12.000000 dask_expr-1.1.2/dask_expr/diagnostics/_explain.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-05-31 21:11:46.916394 dask_expr-1.1.2/dask_expr/io/
+-rw-r--r--   0 james      (501) staff       (20)       96 2024-04-01 19:20:51.000000 dask_expr-1.1.2/dask_expr/io/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     3955 2024-05-03 20:30:23.000000 dask_expr-1.1.2/dask_expr/io/_delayed.py
+-rw-r--r--   0 james      (501) staff       (20)      171 2024-04-01 19:20:57.000000 dask_expr-1.1.2/dask_expr/io/bag.py
+-rw-r--r--   0 james      (501) staff       (20)     8975 2024-05-17 19:52:39.000000 dask_expr-1.1.2/dask_expr/io/csv.py
+-rw-r--r--   0 james      (501) staff       (20)     4366 2024-05-03 20:30:23.000000 dask_expr-1.1.2/dask_expr/io/hdf.py
+-rw-r--r--   0 james      (501) staff       (20)    19469 2024-05-17 19:52:39.000000 dask_expr-1.1.2/dask_expr/io/io.py
+-rw-r--r--   0 james      (501) staff       (20)     6474 2024-05-03 20:30:23.000000 dask_expr-1.1.2/dask_expr/io/json.py
+-rw-r--r--   0 james      (501) staff       (20)     2410 2024-04-19 21:01:12.000000 dask_expr-1.1.2/dask_expr/io/orc.py
+-rw-r--r--   0 james      (501) staff       (20)    69913 2024-05-17 19:52:39.000000 dask_expr-1.1.2/dask_expr/io/parquet.py
+-rw-r--r--   0 james      (501) staff       (20)      482 2024-05-03 20:30:23.000000 dask_expr-1.1.2/dask_expr/io/records.py
+-rw-r--r--   0 james      (501) staff       (20)    13147 2024-05-03 20:30:23.000000 dask_expr-1.1.2/dask_expr/io/sql.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-05-31 21:11:46.916766 dask_expr-1.1.2/dask_expr.egg-info/
+-rw-r--r--   0 james      (501) staff       (20)     2415 2024-05-31 21:11:46.000000 dask_expr-1.1.2/dask_expr.egg-info/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)     1239 2024-05-31 21:11:46.000000 dask_expr-1.1.2/dask_expr.egg-info/SOURCES.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2024-05-31 21:11:46.000000 dask_expr-1.1.2/dask_expr.egg-info/dependency_links.txt
+-rw-r--r--   0 james      (501) staff       (20)       40 2024-05-31 21:11:46.000000 dask_expr-1.1.2/dask_expr.egg-info/requires.txt
+-rw-r--r--   0 james      (501) staff       (20)       10 2024-05-31 21:11:46.000000 dask_expr-1.1.2/dask_expr.egg-info/top_level.txt
+-rw-r--r--   0 james      (501) staff       (20)     2195 2024-05-31 20:58:53.000000 dask_expr-1.1.2/pyproject.toml
+-rw-r--r--   0 james      (501) staff       (20)      230 2024-05-31 21:11:46.917629 dask_expr-1.1.2/setup.cfg
+-rwxr-xr-x   0 james      (501) staff       (20)      194 2024-04-01 19:20:57.000000 dask_expr-1.1.2/setup.py
```

### Comparing `dask_expr-1.1.1/LICENSE.txt` & `dask_expr-1.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dask_expr-1.1.1/PKG-INFO` & `dask_expr-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-expr
-Version: 1.1.1
+Version: 1.1.2
 Summary: High Level Expressions for Dask 
 Maintainer-email: Matthew Rocklin <mrocklin@gmail.com>
 License: BSD
 Project-URL: Source code, https://github.com/dask-contrib/dask-expr/
 Keywords: dask pandas
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: System :: Distributed Computing
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: dask==2024.5.1
+Requires-Dist: dask==2024.5.2
 Requires-Dist: pyarrow>=7.0.0
 Requires-Dist: pandas>=2
 
 Dask Expressions
 ================
 
 Dask DataFrames with query optimization.
```

### Comparing `dask_expr-1.1.1/README.md` & `dask_expr-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `dask_expr-1.1.1/dask_expr/__init__.py` & `dask_expr-1.1.2/dask_expr/__init__.py`

 * *Files identical despite different names*

### Comparing `dask_expr-1.1.1/dask_expr/_accessor.py` & `dask_expr-1.1.2/dask_expr/_accessor.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,13 @@
+import functools
+
 from dask.dataframe.accessor import _bind_method, _bind_property, maybe_wrap_pandas
+from dask.dataframe.dispatch import make_meta, meta_nonempty
 
-from dask_expr._expr import Elemwise
+from dask_expr._expr import Elemwise, Expr
 
 
 class Accessor:
     """
     Base class for pandas Accessor objects cat, dt, and str.
 
     Notes
@@ -93,14 +96,21 @@
         # TODO: We can do better here
         return (None,) * (self.frame.npartitions + 1)
 
 
 class FunctionMap(Elemwise):
     _parameters = ["frame", "accessor", "attr", "args", "kwargs"]
 
+    @functools.cached_property
+    def _meta(self):
+        args = [
+            meta_nonempty(op._meta) if isinstance(op, Expr) else op for op in self._args
+        ]
+        return make_meta(self.operation(*args, **self._kwargs))
+
     @staticmethod
     def operation(obj, accessor, attr, args, kwargs):
         out = getattr(getattr(obj, accessor, obj), attr)(*args, **kwargs)
         return maybe_wrap_pandas(obj, out)
 
 
 class FunctionMapIndex(FunctionMap):
```

### Comparing `dask_expr-1.1.1/dask_expr/_backends.py` & `dask_expr-1.1.2/dask_expr/_backends.py`

 * *Files identical despite different names*

### Comparing `dask_expr-1.1.1/dask_expr/_categorical.py` & `dask_expr-1.1.2/dask_expr/_categorical.py`

 * *Files identical despite different names*

### Comparing `dask_expr-1.1.1/dask_expr/_collection.py` & `dask_expr-1.1.2/dask_expr/_collection.py`

 * *Files identical despite different names*

### Comparing `dask_expr-1.1.1/dask_expr/_concat.py` & `dask_expr-1.1.2/dask_expr/_concat.py`

 * *Files identical despite different names*

### Comparing `dask_expr-1.1.1/dask_expr/_core.py` & `dask_expr-1.1.2/dask_expr/_core.py`

 * *Files identical despite different names*

### Comparing `dask_expr-1.1.1/dask_expr/_cumulative.py` & `dask_expr-1.1.2/dask_expr/_cumulative.py`

 * *Files identical despite different names*

### Comparing `dask_expr-1.1.1/dask_expr/_datetime.py` & `dask_expr-1.1.2/dask_expr/_datetime.py`

 * *Files identical despite different names*

### Comparing `dask_expr-1.1.1/dask_expr/_describe.py` & `dask_expr-1.1.2/dask_expr/_describe.py`

 * *Files identical despite different names*

### Comparing `dask_expr-1.1.1/dask_expr/_dummies.py` & `dask_expr-1.1.2/dask_expr/_dummies.py`

 * *Files identical despite different names*

### Comparing `dask_expr-1.1.1/dask_expr/_expr.py` & `dask_expr-1.1.2/dask_expr/_expr.py`

 * *Files 0% similar despite different names*

```diff
@@ -3036,15 +3036,15 @@
     """
     This Series is broadcastable against another dataframe in the sequence
     """
 
     def compare(s, df):
         try:
             return s.divisions == (min(df.columns), max(df.columns))
-        except TypeError:
+        except (TypeError, ValueError):
             return False
 
     return (
         s.ndim == 1
         and s.npartitions == 1
         and s.known_divisions
         and any(compare(s, df) for df in dfs if df.ndim == 2)
```

### Comparing `dask_expr-1.1.1/dask_expr/_groupby.py` & `dask_expr-1.1.2/dask_expr/_groupby.py`

 * *Files identical despite different names*

### Comparing `dask_expr-1.1.1/dask_expr/_indexing.py` & `dask_expr-1.1.2/dask_expr/_indexing.py`

 * *Files identical despite different names*

### Comparing `dask_expr-1.1.1/dask_expr/_merge.py` & `dask_expr-1.1.2/dask_expr/_merge.py`

 * *Files identical despite different names*

### Comparing `dask_expr-1.1.1/dask_expr/_merge_asof.py` & `dask_expr-1.1.2/dask_expr/_merge_asof.py`

 * *Files identical despite different names*

### Comparing `dask_expr-1.1.1/dask_expr/_quantile.py` & `dask_expr-1.1.2/dask_expr/_quantile.py`

 * *Files identical despite different names*

### Comparing `dask_expr-1.1.1/dask_expr/_quantiles.py` & `dask_expr-1.1.2/dask_expr/_quantiles.py`

 * *Files identical despite different names*

### Comparing `dask_expr-1.1.1/dask_expr/_reductions.py` & `dask_expr-1.1.2/dask_expr/_reductions.py`

 * *Files identical despite different names*

### Comparing `dask_expr-1.1.1/dask_expr/_repartition.py` & `dask_expr-1.1.2/dask_expr/_repartition.py`

 * *Files identical despite different names*

### Comparing `dask_expr-1.1.1/dask_expr/_resample.py` & `dask_expr-1.1.2/dask_expr/_resample.py`

 * *Files identical despite different names*

### Comparing `dask_expr-1.1.1/dask_expr/_rolling.py` & `dask_expr-1.1.2/dask_expr/_rolling.py`

 * *Files identical despite different names*

### Comparing `dask_expr-1.1.1/dask_expr/_shuffle.py` & `dask_expr-1.1.2/dask_expr/_shuffle.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import uuid
 
 import numpy as np
 import pandas as pd
 import tlz as toolz
 from dask import compute
 from dask.dataframe.core import _concat, make_meta
+from dask.dataframe.dispatch import is_categorical_dtype
 from dask.dataframe.shuffle import (
     barrier,
     collect,
     ensure_cleanup_on_exception,
     maybe_buffered_partd,
     partitioning_index,
     set_partitions_pre,
@@ -1301,15 +1302,15 @@
     upsample: float = 1.0,
 ):
     from dask_expr import RepartitionQuantiles, new_collection
 
     if is_index_like(other._meta):
         other = ToSeriesIndex(other)
 
-    if isinstance(other._meta.dtype, pd.CategoricalDtype):
+    if is_categorical_dtype(other._meta.dtype):
         other = new_collection(other).cat.as_ordered()._expr
 
     try:
         divisions, mins, maxes = compute(
             new_collection(RepartitionQuantiles(other, npartitions, upsample=upsample)),
             new_collection(other).map_partitions(M.min),
             new_collection(other).map_partitions(M.max),
```

### Comparing `dask_expr-1.1.1/dask_expr/_str_accessor.py` & `dask_expr-1.1.2/dask_expr/_str_accessor.py`

 * *Files identical despite different names*

### Comparing `dask_expr-1.1.1/dask_expr/_util.py` & `dask_expr-1.1.2/dask_expr/_util.py`

 * *Files identical despite different names*

### Comparing `dask_expr-1.1.1/dask_expr/datasets.py` & `dask_expr-1.1.2/dask_expr/datasets.py`

 * *Files identical despite different names*

### Comparing `dask_expr-1.1.1/dask_expr/diagnostics/_analyze.py` & `dask_expr-1.1.2/dask_expr/diagnostics/_analyze.py`

 * *Files identical despite different names*

### Comparing `dask_expr-1.1.1/dask_expr/diagnostics/_analyze_plugin.py` & `dask_expr-1.1.2/dask_expr/diagnostics/_analyze_plugin.py`

 * *Files identical despite different names*

### Comparing `dask_expr-1.1.1/dask_expr/diagnostics/_explain.py` & `dask_expr-1.1.2/dask_expr/diagnostics/_explain.py`

 * *Files identical despite different names*

### Comparing `dask_expr-1.1.1/dask_expr/io/_delayed.py` & `dask_expr-1.1.2/dask_expr/io/_delayed.py`

 * *Files identical despite different names*

### Comparing `dask_expr-1.1.1/dask_expr/io/csv.py` & `dask_expr-1.1.2/dask_expr/io/csv.py`

 * *Files identical despite different names*

### Comparing `dask_expr-1.1.1/dask_expr/io/hdf.py` & `dask_expr-1.1.2/dask_expr/io/hdf.py`

 * *Files identical despite different names*

### Comparing `dask_expr-1.1.1/dask_expr/io/io.py` & `dask_expr-1.1.2/dask_expr/io/io.py`

 * *Files identical despite different names*

### Comparing `dask_expr-1.1.1/dask_expr/io/json.py` & `dask_expr-1.1.2/dask_expr/io/json.py`

 * *Files identical despite different names*

### Comparing `dask_expr-1.1.1/dask_expr/io/orc.py` & `dask_expr-1.1.2/dask_expr/io/orc.py`

 * *Files identical despite different names*

### Comparing `dask_expr-1.1.1/dask_expr/io/parquet.py` & `dask_expr-1.1.2/dask_expr/io/parquet.py`

 * *Files identical despite different names*

### Comparing `dask_expr-1.1.1/dask_expr/io/sql.py` & `dask_expr-1.1.2/dask_expr/io/sql.py`

 * *Files identical despite different names*

### Comparing `dask_expr-1.1.1/dask_expr.egg-info/PKG-INFO` & `dask_expr-1.1.2/dask_expr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-expr
-Version: 1.1.1
+Version: 1.1.2
 Summary: High Level Expressions for Dask 
 Maintainer-email: Matthew Rocklin <mrocklin@gmail.com>
 License: BSD
 Project-URL: Source code, https://github.com/dask-contrib/dask-expr/
 Keywords: dask pandas
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: System :: Distributed Computing
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: dask==2024.5.1
+Requires-Dist: dask==2024.5.2
 Requires-Dist: pyarrow>=7.0.0
 Requires-Dist: pandas>=2
 
 Dask Expressions
 ================
 
 Dask DataFrames with query optimization.
```

### Comparing `dask_expr-1.1.1/dask_expr.egg-info/SOURCES.txt` & `dask_expr-1.1.2/dask_expr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dask_expr-1.1.1/pyproject.toml` & `dask_expr-1.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     "Programming Language :: Python :: 3.12",
     "Topic :: Scientific/Engineering",
     "Topic :: System :: Distributed Computing",
 ]
 readme = "README.md"
 requires-python = ">=3.9"
 dependencies = [
-    "dask == 2024.5.1",
+    "dask == 2024.5.2",
     "pyarrow>=7.0.0",
     "pandas >= 2",
 ]
 
 dynamic = ["version"]
 
 [project.urls]
```

