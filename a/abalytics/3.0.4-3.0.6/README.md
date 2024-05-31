# Comparing `tmp/abalytics-3.0.4.tar.gz` & `tmp/abalytics-3.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abalytics-3.0.4.tar", last modified: Mon Feb 26 15:34:51 2024, max compression
+gzip compressed data, was "abalytics-3.0.6.tar", last modified: Fri May 31 08:37:46 2024, max compression
```

## Comparing `abalytics-3.0.4.tar` & `abalytics-3.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 15:34:51.240108 abalytics-3.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-26 15:34:43.000000 abalytics-3.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6673 2024-02-26 15:34:51.240108 abalytics-3.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6185 2024-02-26 15:34:43.000000 abalytics-3.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 15:34:51.240108 abalytics-3.0.4/abalytics/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-02-26 15:34:43.000000 abalytics-3.0.4/abalytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11458 2024-02-26 15:34:43.000000 abalytics-3.0.4/abalytics/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    24462 2024-02-26 15:34:43.000000 abalytics-3.0.4/abalytics/significance_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-02-26 15:34:43.000000 abalytics-3.0.4/abalytics/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 15:34:51.240108 abalytics-3.0.4/abalytics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6673 2024-02-26 15:34:51.000000 abalytics-3.0.4/abalytics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-02-26 15:34:51.000000 abalytics-3.0.4/abalytics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-26 15:34:51.000000 abalytics-3.0.4/abalytics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-02-26 15:34:51.000000 abalytics-3.0.4/abalytics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-26 15:34:51.000000 abalytics-3.0.4/abalytics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-26 15:34:51.240108 abalytics-3.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-02-26 15:34:43.000000 abalytics-3.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:37:46.272598 abalytics-3.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-31 08:37:37.000000 abalytics-3.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6673 2024-05-31 08:37:46.272598 abalytics-3.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6185 2024-05-31 08:37:37.000000 abalytics-3.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:37:46.272598 abalytics-3.0.6/abalytics/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-31 08:37:37.000000 abalytics-3.0.6/abalytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11458 2024-05-31 08:37:37.000000 abalytics-3.0.6/abalytics/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24462 2024-05-31 08:37:37.000000 abalytics-3.0.6/abalytics/significance_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-05-31 08:37:37.000000 abalytics-3.0.6/abalytics/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:37:46.272598 abalytics-3.0.6/abalytics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6673 2024-05-31 08:37:46.000000 abalytics-3.0.6/abalytics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-31 08:37:46.000000 abalytics-3.0.6/abalytics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 08:37:46.000000 abalytics-3.0.6/abalytics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-31 08:37:46.000000 abalytics-3.0.6/abalytics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-31 08:37:46.000000 abalytics-3.0.6/abalytics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 08:37:46.272598 abalytics-3.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-31 08:37:37.000000 abalytics-3.0.6/setup.py
```

### Comparing `abalytics-3.0.4/LICENSE` & `abalytics-3.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `abalytics-3.0.4/PKG-INFO` & `abalytics-3.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abalytics
-Version: 3.0.4
+Version: 3.0.6
 Summary: Advanced A/B Testing Statistical Analytics
 Author: Janis Berneker
 License: LICENSE
 Project-URL: Repository, https://github.com/BigBerny/abalytics
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `abalytics-3.0.4/README.md` & `abalytics-3.0.6/README.md`

 * *Files identical despite different names*

### Comparing `abalytics-3.0.4/abalytics/analysis.py` & `abalytics-3.0.6/abalytics/analysis.py`

 * *Files identical despite different names*

### Comparing `abalytics-3.0.4/abalytics/significance_tests.py` & `abalytics-3.0.6/abalytics/significance_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -238,15 +238,15 @@
                     "mean": group_b_stats["mean"],
                     "median": group_b_stats["median"],
                 },
             ],
             key=lambda x: x["mean"],
             reverse=True,
         )
-        result_pretty_text = f"{groups_info[0]['name']} ({groups_info[0]['mean']:.2f}) > {groups_info[1]['name']} ({groups_info[1]['mean']:.2f})"
+        result_pretty_text = f"{groups_info[0]['name']} ({groups_info[0]['mean']:.3f}) > {groups_info[1]['name']} ({groups_info[1]['mean']:.3f})"
         posthoc_results.add_result(
             "Games-Howell", result_pretty_text, row["pval"], groups_info
         )
 
     return posthoc_results
 
 
@@ -334,15 +334,15 @@
                     "mean": group_b_stats["mean"],
                     "median": group_b_stats["median"],
                 },
             ],
             key=lambda x: x["mean"],
             reverse=True,
         )
-        result_pretty_text = f"{groups_info[0]['name']} ({groups_info[0]['mean']:.2f}) > {groups_info[1]['name']} ({groups_info[1]['mean']:.2f})"
+        result_pretty_text = f"{groups_info[0]['name']} ({groups_info[0]['mean']:.3f}) > {groups_info[1]['name']} ({groups_info[1]['mean']:.3f})"
         posthoc_results.add_result(
             "Tukey HSD", result_pretty_text, row["p-adj"], groups_info
         )
 
     return posthoc_results
 
 
@@ -394,15 +394,15 @@
                             "median": group_b_stats["median"],
                         },
                     ],
                     key=lambda x: x["mean"],
                     reverse=True,
                 )
 
-                result_pretty_text = f"{groups_info[0]['name']} ({groups_info[0]['mean']:.2f}) > {groups_info[1]['name']} ({groups_info[1]['mean']:.2f})"
+                result_pretty_text = f"{groups_info[0]['name']} ({groups_info[0]['mean']:.3f}) > {groups_info[1]['name']} ({groups_info[1]['mean']:.3f})"
                 posthoc_results.add_result(
                     "Dunn", result_pretty_text, p_value, groups_info
                 )
 
     return posthoc_results
 
 
@@ -441,15 +441,15 @@
                     "median": df[variable].median(),
                 }
                 for variable in [var1, var2]
             ]
             # Sort groups by mean for consistent presentation
             groups_info.sort(key=lambda x: x["mean"], reverse=True)
             # Format the result text
-            result_pretty_text = f"{groups_info[0]['name']} ({groups_info[0]['mean']:.2f}) > {groups_info[1]['name']} ({groups_info[1]['mean']:.2f})"
+            result_pretty_text = f"{groups_info[0]['name']} ({groups_info[0]['mean']:.3f}) > {groups_info[1]['name']} ({groups_info[1]['mean']:.3f})"
             # Add the result to posthoc results
             posthoc_results.add_result(
                 "McNemar", result_pretty_text, p_value, groups_info
             )
 
     return posthoc_results
 
@@ -524,15 +524,15 @@
                     "mean": df[var].mean(),
                     "median": df[var].median(),
                 }
                 for var in [var1, var2]
             ]
             # Sort groups by mean for consistent presentation
             groups_info.sort(key=lambda x: x["mean"], reverse=True)
-            result_pretty_text = f"{groups_info[0]['name']} ({groups_info[0]['mean']:.2f}) > {groups_info[1]['name']} ({groups_info[1]['mean']:.2f})"
+            result_pretty_text = f"{groups_info[0]['name']} ({groups_info[0]['mean']:.3f}) > {groups_info[1]['name']} ({groups_info[1]['mean']:.3f})"
             posthoc_results.add_result(
                 "Repeated Measures ANOVA",
                 result_pretty_text,
                 p_val_corrected,
                 groups_info,
             )
 
@@ -572,15 +572,15 @@
             "mean": df[var].mean(),
             "median": df[var].median(),
         }
         for var in variables_to_compare
     ]
     groups_info.sort(key=lambda x: x["mean"], reverse=True)
 
-    result_pretty_text = f"{groups_info[0]['name']} ({groups_info[0]['mean']:.2f}) > {groups_info[1]['name']} ({groups_info[1]['mean']:.2f})"
+    result_pretty_text = f"{groups_info[0]['name']} ({groups_info[0]['mean']:.3f}) > {groups_info[1]['name']} ({groups_info[1]['mean']:.3f})"
     posthoc_results.add_result("Wilcoxon", result_pretty_text, p_value, groups_info)
 
     return p_value, posthoc_results
 
 
 def get_friedman_significance(
     df: pd.DataFrame, variables_to_compare: List[str]
@@ -629,13 +629,13 @@
                     "mean": df[var].mean(),
                     "median": df[var].median(),
                 }
                 for var in [var1, var2]
             ]
             groups_info.sort(key=lambda x: x["mean"], reverse=True)
 
-            result_pretty_text = f"{groups_info[0]['name']} ({groups_info[0]['mean']:.2f}) > {groups_info[1]['name']} ({groups_info[1]['mean']:.2f})"
+            result_pretty_text = f"{groups_info[0]['name']} ({groups_info[0]['mean']:.3f}) > {groups_info[1]['name']} ({groups_info[1]['mean']:.3f})"
             posthoc_results.add_result(
                 "Nemenyi", result_pretty_text, posthoc_p_value, groups_info
             )
 
     return posthoc_results
```

### Comparing `abalytics-3.0.4/abalytics/utils.py` & `abalytics-3.0.6/abalytics/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         if show_only_significant_results and len(significant_results) == 0:
             continue
         if len(significant_results) > 0:
             for result in significant_results:
                 row = identifiers_list[idx].copy()
                 row["n"] = sample_size
                 row["Result"] = result.result_pretty_text
-                row["p-value"] = result.p_value  # round(result.p_value,3)
+                row["p-value"] = result.p_value
                 if show_details:
                     row["Analysis method"] = result.analysis_method
                     if info:
                         row["info"] = info
                     row["Gaussian"] = gaussian_flag
                     row["Levene"] = levene_flag
                     row["A priori test"] = a_priori_test
```

### Comparing `abalytics-3.0.4/abalytics.egg-info/PKG-INFO` & `abalytics-3.0.6/abalytics.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abalytics
-Version: 3.0.4
+Version: 3.0.6
 Summary: Advanced A/B Testing Statistical Analytics
 Author: Janis Berneker
 License: LICENSE
 Project-URL: Repository, https://github.com/BigBerny/abalytics
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `abalytics-3.0.4/setup.py` & `abalytics-3.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='abalytics',
-    version='3.0.4',
+    version='3.0.6',
     author='Janis Berneker',
     packages=find_packages(),
     license='LICENSE',
     description='Advanced A/B Testing Statistical Analytics',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     install_requires=[
```

