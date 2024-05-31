# Comparing `tmp/urbantrips-0.2.4.tar.gz` & `tmp/urbantrips-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "urbantrips-0.2.4.tar", last modified: Tue Oct 17 17:08:12 2023, max compression
+gzip compressed data, was "urbantrips-0.2.5.tar", last modified: Fri May 31 21:31:42 2024, max compression
```

## Comparing `urbantrips-0.2.4.tar` & `urbantrips-0.2.5.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 17:08:12.273875 urbantrips-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11834 2023-10-17 17:08:03.000000 urbantrips-0.2.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     3584 2023-10-17 17:08:12.273875 urbantrips-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2023-10-17 17:08:03.000000 urbantrips-0.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       70 2023-10-17 17:08:03.000000 urbantrips-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-17 17:08:12.273875 urbantrips-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2023-10-17 17:08:03.000000 urbantrips-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 17:08:12.269875 urbantrips-0.2.4/urbantrips/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-17 17:08:03.000000 urbantrips-0.2.4/urbantrips/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 17:08:12.269875 urbantrips-0.2.4/urbantrips/carto/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-17 17:08:03.000000 urbantrips-0.2.4/urbantrips/carto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20160 2023-10-17 17:08:03.000000 urbantrips-0.2.4/urbantrips/carto/carto.py
--rw-r--r--   0 runner    (1001) docker     (127)    14220 2023-10-17 17:08:03.000000 urbantrips-0.2.4/urbantrips/carto/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     8291 2023-10-17 17:08:03.000000 urbantrips-0.2.4/urbantrips/carto/stops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 17:08:12.269875 urbantrips-0.2.4/urbantrips/cluster/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-17 17:08:03.000000 urbantrips-0.2.4/urbantrips/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22133 2023-10-17 17:08:03.000000 urbantrips-0.2.4/urbantrips/cluster/dbscan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2023-10-17 17:08:03.000000 urbantrips-0.2.4/urbantrips/compute_clusters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2023-10-17 17:08:03.000000 urbantrips-0.2.4/urbantrips/create_viz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 17:08:12.269875 urbantrips-0.2.4/urbantrips/datamodel/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-17 17:08:03.000000 urbantrips-0.2.4/urbantrips/datamodel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16139 2023-10-17 17:08:03.000000 urbantrips-0.2.4/urbantrips/datamodel/legs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8123 2023-10-17 17:08:03.000000 urbantrips-0.2.4/urbantrips/datamodel/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    19082 2023-10-17 17:08:03.000000 urbantrips-0.2.4/urbantrips/datamodel/services.py
--rw-r--r--   0 runner    (1001) docker     (127)    26165 2023-10-17 17:08:03.000000 urbantrips-0.2.4/urbantrips/datamodel/transactions.py
--rw-r--r--   0 runner    (1001) docker     (127)    14090 2023-10-17 17:08:03.000000 urbantrips-0.2.4/urbantrips/datamodel/trips.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 17:08:12.269875 urbantrips-0.2.4/urbantrips/destinations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-17 17:08:03.000000 urbantrips-0.2.4/urbantrips/destinations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10665 2023-10-17 17:08:03.000000 urbantrips-0.2.4/urbantrips/destinations/destinations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 17:08:12.269875 urbantrips-0.2.4/urbantrips/geo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-17 17:08:03.000000 urbantrips-0.2.4/urbantrips/geo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10450 2023-10-17 17:08:03.000000 urbantrips-0.2.4/urbantrips/geo/geo.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2023-10-17 17:08:03.000000 urbantrips-0.2.4/urbantrips/initialize_environment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 17:08:12.269875 urbantrips-0.2.4/urbantrips/kpi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-17 17:08:03.000000 urbantrips-0.2.4/urbantrips/kpi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    48551 2023-10-17 17:08:03.000000 urbantrips-0.2.4/urbantrips/kpi/kpi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2023-10-17 17:08:03.000000 urbantrips-0.2.4/urbantrips/process_transactions.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2023-10-17 17:08:03.000000 urbantrips-0.2.4/urbantrips/run_all_urbantrips.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2023-10-17 17:08:03.000000 urbantrips-0.2.4/urbantrips/run_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2023-10-17 17:08:03.000000 urbantrips-0.2.4/urbantrips/run_postprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 17:08:12.273875 urbantrips-0.2.4/urbantrips/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-17 17:08:03.000000 urbantrips-0.2.4/urbantrips/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2023-10-17 17:08:03.000000 urbantrips-0.2.4/urbantrips/tests/test_routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3604 2023-10-17 17:08:03.000000 urbantrips-0.2.4/urbantrips/tests/test_services.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2023-10-17 17:08:03.000000 urbantrips-0.2.4/urbantrips/tests/test_stops.py
--rw-r--r--   0 runner    (1001) docker     (127)    26747 2023-10-17 17:08:03.000000 urbantrips-0.2.4/urbantrips/tests/test_unit_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 17:08:12.273875 urbantrips-0.2.4/urbantrips/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-17 17:08:03.000000 urbantrips-0.2.4/urbantrips/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29121 2023-10-17 17:08:03.000000 urbantrips-0.2.4/urbantrips/utils/check_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)    25618 2023-10-17 17:08:03.000000 urbantrips-0.2.4/urbantrips/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 17:08:12.273875 urbantrips-0.2.4/urbantrips/viz/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-17 17:08:03.000000 urbantrips-0.2.4/urbantrips/viz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   100198 2023-10-17 17:08:03.000000 urbantrips-0.2.4/urbantrips/viz/viz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 17:08:12.273875 urbantrips-0.2.4/urbantrips/viz_ppt_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-17 17:08:03.000000 urbantrips-0.2.4/urbantrips/viz_ppt_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30645 2023-10-17 17:08:03.000000 urbantrips-0.2.4/urbantrips/viz_ppt_utils/viz_ppt_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 17:08:12.269875 urbantrips-0.2.4/urbantrips.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3584 2023-10-17 17:08:12.000000 urbantrips-0.2.4/urbantrips.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2023-10-17 17:08:12.000000 urbantrips-0.2.4/urbantrips.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-17 17:08:12.000000 urbantrips-0.2.4/urbantrips.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      452 2023-10-17 17:08:12.000000 urbantrips-0.2.4/urbantrips.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-10-17 17:08:12.000000 urbantrips-0.2.4/urbantrips.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:31:42.380489 urbantrips-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11834 2024-05-31 21:31:38.000000 urbantrips-0.2.5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-05-31 21:31:42.380489 urbantrips-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-31 21:31:38.000000 urbantrips-0.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-31 21:31:38.000000 urbantrips-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 21:31:42.380489 urbantrips-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-31 21:31:38.000000 urbantrips-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:31:42.372489 urbantrips-0.2.5/urbantrips/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 21:31:38.000000 urbantrips-0.2.5/urbantrips/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:31:42.372489 urbantrips-0.2.5/urbantrips/carto/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 21:31:38.000000 urbantrips-0.2.5/urbantrips/carto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20160 2024-05-31 21:31:38.000000 urbantrips-0.2.5/urbantrips/carto/carto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14220 2024-05-31 21:31:38.000000 urbantrips-0.2.5/urbantrips/carto/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8291 2024-05-31 21:31:38.000000 urbantrips-0.2.5/urbantrips/carto/stops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:31:42.372489 urbantrips-0.2.5/urbantrips/cluster/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 21:31:38.000000 urbantrips-0.2.5/urbantrips/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22133 2024-05-31 21:31:38.000000 urbantrips-0.2.5/urbantrips/cluster/dbscan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-31 21:31:38.000000 urbantrips-0.2.5/urbantrips/compute_clusters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-31 21:31:38.000000 urbantrips-0.2.5/urbantrips/create_viz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:31:42.376489 urbantrips-0.2.5/urbantrips/datamodel/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 21:31:38.000000 urbantrips-0.2.5/urbantrips/datamodel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16139 2024-05-31 21:31:38.000000 urbantrips-0.2.5/urbantrips/datamodel/legs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8123 2024-05-31 21:31:38.000000 urbantrips-0.2.5/urbantrips/datamodel/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19082 2024-05-31 21:31:38.000000 urbantrips-0.2.5/urbantrips/datamodel/services.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26165 2024-05-31 21:31:38.000000 urbantrips-0.2.5/urbantrips/datamodel/transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14090 2024-05-31 21:31:38.000000 urbantrips-0.2.5/urbantrips/datamodel/trips.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:31:42.376489 urbantrips-0.2.5/urbantrips/destinations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 21:31:38.000000 urbantrips-0.2.5/urbantrips/destinations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10665 2024-05-31 21:31:38.000000 urbantrips-0.2.5/urbantrips/destinations/destinations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:31:42.376489 urbantrips-0.2.5/urbantrips/geo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 21:31:38.000000 urbantrips-0.2.5/urbantrips/geo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10450 2024-05-31 21:31:38.000000 urbantrips-0.2.5/urbantrips/geo/geo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-31 21:31:38.000000 urbantrips-0.2.5/urbantrips/initialize_environment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:31:42.376489 urbantrips-0.2.5/urbantrips/kpi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 21:31:38.000000 urbantrips-0.2.5/urbantrips/kpi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48551 2024-05-31 21:31:38.000000 urbantrips-0.2.5/urbantrips/kpi/kpi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-05-31 21:31:38.000000 urbantrips-0.2.5/urbantrips/process_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-31 21:31:38.000000 urbantrips-0.2.5/urbantrips/run_all_urbantrips.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-31 21:31:38.000000 urbantrips-0.2.5/urbantrips/run_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-31 21:31:38.000000 urbantrips-0.2.5/urbantrips/run_postprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:31:42.376489 urbantrips-0.2.5/urbantrips/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 21:31:38.000000 urbantrips-0.2.5/urbantrips/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-31 21:31:38.000000 urbantrips-0.2.5/urbantrips/tests/test_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-05-31 21:31:38.000000 urbantrips-0.2.5/urbantrips/tests/test_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-31 21:31:38.000000 urbantrips-0.2.5/urbantrips/tests/test_stops.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26747 2024-05-31 21:31:38.000000 urbantrips-0.2.5/urbantrips/tests/test_unit_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:31:42.376489 urbantrips-0.2.5/urbantrips/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 21:31:38.000000 urbantrips-0.2.5/urbantrips/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29121 2024-05-31 21:31:38.000000 urbantrips-0.2.5/urbantrips/utils/check_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25618 2024-05-31 21:31:38.000000 urbantrips-0.2.5/urbantrips/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:31:42.376489 urbantrips-0.2.5/urbantrips/viz/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 21:31:38.000000 urbantrips-0.2.5/urbantrips/viz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   100329 2024-05-31 21:31:38.000000 urbantrips-0.2.5/urbantrips/viz/viz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:31:42.376489 urbantrips-0.2.5/urbantrips/viz_ppt_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 21:31:38.000000 urbantrips-0.2.5/urbantrips/viz_ppt_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30645 2024-05-31 21:31:38.000000 urbantrips-0.2.5/urbantrips/viz_ppt_utils/viz_ppt_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:31:42.376489 urbantrips-0.2.5/urbantrips.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-05-31 21:31:42.000000 urbantrips-0.2.5/urbantrips.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-31 21:31:42.000000 urbantrips-0.2.5/urbantrips.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 21:31:42.000000 urbantrips-0.2.5/urbantrips.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-31 21:31:42.000000 urbantrips-0.2.5/urbantrips.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-31 21:31:42.000000 urbantrips-0.2.5/urbantrips.egg-info/top_level.txt
```

### Comparing `urbantrips-0.2.4/LICENSE.md` & `urbantrips-0.2.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `urbantrips-0.2.4/PKG-INFO` & `urbantrips-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: urbantrips
-Version: 0.2.4
+Version: 0.2.5
 Summary: A library to process public transit smart card data.
 Home-page: https://github.com/EL-BID/UrbanTrips
 Author: Felipe Gonzalez & Sebastian Anapolsky
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
@@ -15,15 +15,14 @@
 Requires-Dist: geopandas==0.14.0
 Requires-Dist: h3==3.7.6
 Requires-Dist: ipython==8.16.1
 Requires-Dist: jupyterlab==4.0.6
 Requires-Dist: libpysal==4.8.0
 Requires-Dist: mapclassify==2.6.1
 Requires-Dist: matplotlib-scalebar==0.8.1
-Requires-Dist: mycolorpy==1.5.1
 Requires-Dist: notebook==7.0.4
 Requires-Dist: numba==0.58.0
 Requires-Dist: numpy==1.25.2
 Requires-Dist: openpyxl==3.1.2
 Requires-Dist: osmnx==1.6.0
 Requires-Dist: pandas==2.1.1
 Requires-Dist: patsy==0.5.3
```

### Comparing `urbantrips-0.2.4/README.md` & `urbantrips-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `urbantrips-0.2.4/setup.py` & `urbantrips-0.2.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open('requirements.txt', 'r') as f:
     install_requires = f.read().split('\n')[:-1]
 
 setuptools.setup(
     name='urbantrips',
-    version='0.2.4',
+    version='0.2.5',
     author="Felipe Gonzalez & Sebastian Anapolsky",
     author_email="",
     description="A library to process public transit smart card data.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/EL-BID/UrbanTrips",
     packages=setuptools.find_packages(),
@@ -27,15 +27,14 @@
         'geopandas==0.14.0',
         'h3==3.7.6',
         'ipython==8.16.1',
         'jupyterlab==4.0.6',
         'libpysal==4.8.0',
         'mapclassify==2.6.1',
         'matplotlib-scalebar==0.8.1',
-        'mycolorpy==1.5.1',
         'notebook==7.0.4',
         'numba==0.58.0',
         'numpy==1.25.2',
         'openpyxl==3.1.2',
         'osmnx==1.6.0',
         'pandas==2.1.1',
         'patsy==0.5.3',
```

### Comparing `urbantrips-0.2.4/urbantrips/carto/carto.py` & `urbantrips-0.2.5/urbantrips/carto/carto.py`

 * *Files identical despite different names*

### Comparing `urbantrips-0.2.4/urbantrips/carto/routes.py` & `urbantrips-0.2.5/urbantrips/carto/routes.py`

 * *Files identical despite different names*

### Comparing `urbantrips-0.2.4/urbantrips/carto/stops.py` & `urbantrips-0.2.5/urbantrips/carto/stops.py`

 * *Files identical despite different names*

### Comparing `urbantrips-0.2.4/urbantrips/cluster/dbscan.py` & `urbantrips-0.2.5/urbantrips/cluster/dbscan.py`

 * *Files identical despite different names*

### Comparing `urbantrips-0.2.4/urbantrips/compute_clusters.py` & `urbantrips-0.2.5/urbantrips/compute_clusters.py`

 * *Files identical despite different names*

### Comparing `urbantrips-0.2.4/urbantrips/create_viz.py` & `urbantrips-0.2.5/urbantrips/create_viz.py`

 * *Files identical despite different names*

### Comparing `urbantrips-0.2.4/urbantrips/datamodel/legs.py` & `urbantrips-0.2.5/urbantrips/datamodel/legs.py`

 * *Files identical despite different names*

### Comparing `urbantrips-0.2.4/urbantrips/datamodel/misc.py` & `urbantrips-0.2.5/urbantrips/datamodel/misc.py`

 * *Files identical despite different names*

### Comparing `urbantrips-0.2.4/urbantrips/datamodel/services.py` & `urbantrips-0.2.5/urbantrips/datamodel/services.py`

 * *Files identical despite different names*

### Comparing `urbantrips-0.2.4/urbantrips/datamodel/transactions.py` & `urbantrips-0.2.5/urbantrips/datamodel/transactions.py`

 * *Files identical despite different names*

### Comparing `urbantrips-0.2.4/urbantrips/datamodel/trips.py` & `urbantrips-0.2.5/urbantrips/datamodel/trips.py`

 * *Files identical despite different names*

### Comparing `urbantrips-0.2.4/urbantrips/destinations/destinations.py` & `urbantrips-0.2.5/urbantrips/destinations/destinations.py`

 * *Files identical despite different names*

### Comparing `urbantrips-0.2.4/urbantrips/geo/geo.py` & `urbantrips-0.2.5/urbantrips/geo/geo.py`

 * *Files identical despite different names*

### Comparing `urbantrips-0.2.4/urbantrips/initialize_environment.py` & `urbantrips-0.2.5/urbantrips/initialize_environment.py`

 * *Files identical despite different names*

### Comparing `urbantrips-0.2.4/urbantrips/kpi/kpi.py` & `urbantrips-0.2.5/urbantrips/kpi/kpi.py`

 * *Files identical despite different names*

### Comparing `urbantrips-0.2.4/urbantrips/process_transactions.py` & `urbantrips-0.2.5/urbantrips/process_transactions.py`

 * *Files identical despite different names*

### Comparing `urbantrips-0.2.4/urbantrips/run_dashboard.py` & `urbantrips-0.2.5/urbantrips/run_dashboard.py`

 * *Files identical despite different names*

### Comparing `urbantrips-0.2.4/urbantrips/run_postprocessing.py` & `urbantrips-0.2.5/urbantrips/run_postprocessing.py`

 * *Files identical despite different names*

### Comparing `urbantrips-0.2.4/urbantrips/tests/test_routes.py` & `urbantrips-0.2.5/urbantrips/tests/test_routes.py`

 * *Files identical despite different names*

### Comparing `urbantrips-0.2.4/urbantrips/tests/test_services.py` & `urbantrips-0.2.5/urbantrips/tests/test_services.py`

 * *Files identical despite different names*

### Comparing `urbantrips-0.2.4/urbantrips/tests/test_stops.py` & `urbantrips-0.2.5/urbantrips/tests/test_stops.py`

 * *Files identical despite different names*

### Comparing `urbantrips-0.2.4/urbantrips/tests/test_unit_tests.py` & `urbantrips-0.2.5/urbantrips/tests/test_unit_tests.py`

 * *Files identical despite different names*

### Comparing `urbantrips-0.2.4/urbantrips/utils/check_configs.py` & `urbantrips-0.2.5/urbantrips/utils/check_configs.py`

 * *Files identical despite different names*

### Comparing `urbantrips-0.2.4/urbantrips/utils/utils.py` & `urbantrips-0.2.5/urbantrips/utils/utils.py`

 * *Files identical despite different names*

### Comparing `urbantrips-0.2.4/urbantrips/viz/viz.py` & `urbantrips-0.2.5/urbantrips/viz/viz.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 import contextily as ctx
 from IPython.display import display
 from matplotlib_scalebar.scalebar import ScaleBar
 from matplotlib.collections import QuadMesh
 from pathlib import Path
 from matplotlib import colors as mcolors
 from matplotlib.text import Text
-from mycolorpy import colorlist as mcp
 from requests.exceptions import ConnectionError as r_ConnectionError
 from pandas.io.sql import DatabaseError
 
 from urbantrips.kpi import kpi
 from urbantrips.carto import carto
 from urbantrips.geo import geo
 from urbantrips.geo.geo import (
@@ -540,22 +539,21 @@
     ax4.annotate('Sentido', xy=flecha_vuelta_xy, xytext=flecha_vuelta_text_xy,
                  size=16, va="center", ha="center",
                  xycoords='axes fraction',
                  arrowprops=dict(facecolor='Orange',
                                  shrink=0.05, edgecolor='Orange'),
                  )
 
-    prov = cx.providers.Stamen.TonerLite
+    prov = cx.providers.CartoDB.Positron
     try:
         cx.add_basemap(ax1, crs=gdf_d0.crs.to_string(), source=prov)
         cx.add_basemap(ax2, crs=gdf_d1.crs.to_string(), source=prov)
     except (UnidentifiedImageError, ValueError):
-        prov = cx.providers.CartoDB.Positron
-        cx.add_basemap(ax1, crs=gdf_d0.crs.to_string(), source=prov)
-        cx.add_basemap(ax2, crs=gdf_d1.crs.to_string(), source=prov)
+        cx.add_basemap(ax1, crs=gdf_d0.crs.to_string())
+        cx.add_basemap(ax2, crs=gdf_d1.crs.to_string())
     except (r_ConnectionError):
         pass
 
     alias = leer_alias()
 
     for frm in ['png', 'pdf']:
         archivo = f"{alias}_{day}_segmentos_id_linea_"
@@ -2215,15 +2213,15 @@
     title_html = """
     <h3 align="center" style="font-size:20px"><b>Your map title</b></h3>
     """
     m.get_root().html.add_child(folium.Element(title_html))
 
     line_w = 0.5
 
-    colors = mcp.gen_color(cmap=cmap, n=k_jenks)
+    colors = extract_hex_colors_from_cmap(cmap=cmap, n=k_jenks)
 
     n = 0
     for i in bins_labels:
 
         df_agg[df_agg.cuts == i].explore(
             m=m,
             color=colors[n],
@@ -2515,17 +2513,15 @@
                      color='Purple', label='Oferta')
         sns.lineplot(data=kpi_stats_line_plot, x="hora", y="pax", ax=ax,
                      color='Orange', label='Demanda')
 
         ax.set_xlabel("Hora")
         ax.set_ylabel(ylabel_str)
 
-        f.suptitle(f"Indicadores de oferta y demanda estadarizados",
-                   fontdict={'size': 18,
-                             'weight': 'bold'})
+        f.suptitle(f"Indicadores de oferta y demanda estadarizados")
 
         ax.set_title(f"{id_linea_str} id linea: {line_id} - Dia: {day_str}",
                      fontdict={"fontsize": 11})
         # Add a footnote below and to the right side of the chart
 
         ax_note = ax.annotate(note,
                               xy=(0, -.18),
@@ -2892,7 +2888,20 @@
     indicadores_dash()
 
     # plor dispatched services
     plot_dispatched_services_wrapper()
 
     # plot basic kpi if exists
     plot_basic_kpi_wrapper()
+
+
+def extract_hex_colors_from_cmap(cmap, n=5):
+    # Choose a colormap
+    cmap = plt.get_cmap(cmap)
+
+    # Extract colors from the colormap
+    colors = cmap(np.linspace(0, 1, n))
+
+    # Convert the colors to hex format
+    hex_colors = [mcolors.rgb2hex(color) for color in colors]
+
+    return hex_colors
```

### Comparing `urbantrips-0.2.4/urbantrips/viz_ppt_utils/viz_ppt_utils.py` & `urbantrips-0.2.5/urbantrips/viz_ppt_utils/viz_ppt_utils.py`

 * *Files identical despite different names*

### Comparing `urbantrips-0.2.4/urbantrips.egg-info/PKG-INFO` & `urbantrips-0.2.5/urbantrips.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: urbantrips
-Version: 0.2.4
+Version: 0.2.5
 Summary: A library to process public transit smart card data.
 Home-page: https://github.com/EL-BID/UrbanTrips
 Author: Felipe Gonzalez & Sebastian Anapolsky
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
@@ -15,15 +15,14 @@
 Requires-Dist: geopandas==0.14.0
 Requires-Dist: h3==3.7.6
 Requires-Dist: ipython==8.16.1
 Requires-Dist: jupyterlab==4.0.6
 Requires-Dist: libpysal==4.8.0
 Requires-Dist: mapclassify==2.6.1
 Requires-Dist: matplotlib-scalebar==0.8.1
-Requires-Dist: mycolorpy==1.5.1
 Requires-Dist: notebook==7.0.4
 Requires-Dist: numba==0.58.0
 Requires-Dist: numpy==1.25.2
 Requires-Dist: openpyxl==3.1.2
 Requires-Dist: osmnx==1.6.0
 Requires-Dist: pandas==2.1.1
 Requires-Dist: patsy==0.5.3
```

### Comparing `urbantrips-0.2.4/urbantrips.egg-info/SOURCES.txt` & `urbantrips-0.2.5/urbantrips.egg-info/SOURCES.txt`

 * *Files identical despite different names*

