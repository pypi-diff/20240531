# Comparing `tmp/oianalytics-0.5.3.tar.gz` & `tmp/oianalytics-0.5.4b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oianalytics-0.5.3.tar", max compression
+gzip compressed data, was "oianalytics-0.5.4b1.tar", max compression
```

## Comparing `oianalytics-0.5.3.tar` & `oianalytics-0.5.4b1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0    13799 2023-03-15 14:01:49.113528 oianalytics-0.5.3/LICENSE
--rw-r--r--   0        0        0       92 2024-04-11 08:26:37.003147 oianalytics-0.5.3/oianalytics/__init__.py
--rw-r--r--   0        0        0      124 2024-02-12 10:28:03.022129 oianalytics-0.5.3/oianalytics/api/__init__.py
--rw-r--r--   0        0        0     2373 2023-03-15 14:01:49.113932 oianalytics-0.5.3/oianalytics/api/_credentials.py
--rw-r--r--   0        0        0     2442 2024-02-12 10:28:03.022426 oianalytics-0.5.3/oianalytics/api/_dataframes/__init__.py
--rw-r--r--   0        0        0    16024 2023-11-06 09:30:13.500439 oianalytics-0.5.3/oianalytics/api/_dataframes/assets.py
--rw-r--r--   0        0        0     3847 2023-11-06 09:30:13.500761 oianalytics-0.5.3/oianalytics/api/_dataframes/azure_blob_sources.py
--rw-r--r--   0        0        0    48788 2024-02-12 10:28:03.022749 oianalytics-0.5.3/oianalytics/api/_dataframes/batches.py
--rw-r--r--   0        0        0    41856 2023-10-30 14:56:38.145683 oianalytics-0.5.3/oianalytics/api/_dataframes/data.py
--rw-r--r--   0        0        0     9979 2023-03-15 14:01:49.114785 oianalytics-0.5.3/oianalytics/api/_dataframes/events.py
--rw-r--r--   0        0        0     4631 2023-03-15 14:01:49.114887 oianalytics-0.5.3/oianalytics/api/_dataframes/files.py
--rw-r--r--   0        0        0     7991 2023-11-06 09:30:13.501670 oianalytics-0.5.3/oianalytics/api/_dataframes/model_instances.py
--rw-r--r--   0        0        0     3933 2023-11-06 09:30:13.502064 oianalytics-0.5.3/oianalytics/api/_dataframes/profiles.py
--rw-r--r--   0        0        0     2416 2023-10-30 14:56:38.146077 oianalytics-0.5.3/oianalytics/api/_dataframes/quantities.py
--rw-r--r--   0        0        0     5581 2024-02-12 10:28:10.083841 oianalytics-0.5.3/oianalytics/api/_dataframes/tags.py
--rw-r--r--   0        0        0     5463 2023-11-06 09:30:13.502604 oianalytics-0.5.3/oianalytics/api/_dataframes/units.py
--rw-r--r--   0        0        0     4251 2023-11-06 09:30:13.502818 oianalytics-0.5.3/oianalytics/api/_dataframes/users.py
--rw-r--r--   0        0        0      705 2024-04-11 08:26:37.003541 oianalytics-0.5.3/oianalytics/api/endpoints/__init__.py
--rw-r--r--   0        0        0     5806 2024-02-12 10:28:03.023906 oianalytics-0.5.3/oianalytics/api/endpoints/assets.py
--rw-r--r--   0        0        0     1437 2023-11-06 09:30:13.503405 oianalytics-0.5.3/oianalytics/api/endpoints/azure_blob_sources.py
--rw-r--r--   0        0        0    11949 2024-02-12 10:28:03.024141 oianalytics-0.5.3/oianalytics/api/endpoints/batches.py
--rw-r--r--   0        0        0     2646 2024-04-11 08:26:37.003805 oianalytics-0.5.3/oianalytics/api/endpoints/computation_jobs.py
--rw-r--r--   0        0        0    13255 2023-11-06 09:30:13.503842 oianalytics-0.5.3/oianalytics/api/endpoints/data.py
--rw-r--r--   0        0        0     2635 2023-11-06 09:30:13.504076 oianalytics-0.5.3/oianalytics/api/endpoints/events.py
--rw-r--r--   0        0        0     3204 2023-11-06 09:30:13.504386 oianalytics-0.5.3/oianalytics/api/endpoints/files.py
--rw-r--r--   0        0        0     1387 2023-11-06 09:30:13.504678 oianalytics-0.5.3/oianalytics/api/endpoints/model_instances.py
--rw-r--r--   0        0        0     2779 2024-02-12 10:28:03.024389 oianalytics-0.5.3/oianalytics/api/endpoints/profiles.py
--rw-r--r--   0        0        0      772 2023-10-30 14:56:38.147329 oianalytics-0.5.3/oianalytics/api/endpoints/quantities.py
--rw-r--r--   0        0        0     4519 2024-02-12 10:28:10.090400 oianalytics-0.5.3/oianalytics/api/endpoints/tags.py
--rw-r--r--   0        0        0     1787 2023-11-06 09:30:13.505426 oianalytics-0.5.3/oianalytics/api/endpoints/units.py
--rw-r--r--   0        0        0     2170 2024-02-12 10:28:03.024745 oianalytics-0.5.3/oianalytics/api/endpoints/users.py
--rw-r--r--   0        0        0     5881 2023-04-18 12:32:43.955607 oianalytics-0.5.3/oianalytics/api/utils.py
--rw-r--r--   0        0        0      133 2023-03-15 14:01:49.115833 oianalytics-0.5.3/oianalytics/models/__init__.py
--rw-r--r--   0        0        0    40900 2024-04-11 08:26:37.004294 oianalytics-0.5.3/oianalytics/models/_dtos.py
--rw-r--r--   0        0        0      346 2023-04-18 12:32:43.955722 oianalytics-0.5.3/oianalytics/models/_queries/__init__.py
--rw-r--r--   0        0        0     1965 2023-11-06 09:30:13.505992 oianalytics-0.5.3/oianalytics/models/_queries/files.py
--rw-r--r--   0        0        0      727 2023-11-06 09:30:13.506204 oianalytics-0.5.3/oianalytics/models/_queries/instances.py
--rw-r--r--   0        0        0    13883 2023-10-30 14:56:38.148516 oianalytics-0.5.3/oianalytics/models/_queries/single_observation.py
--rw-r--r--   0        0        0        0 2023-03-15 14:01:49.116471 oianalytics-0.5.3/oianalytics/models/_template_resources/__init__.py
--rw-r--r--   0        0        0     2796 2023-04-18 12:32:43.955950 oianalytics-0.5.3/oianalytics/models/_template_resources/file_processing_template.py
--rw-r--r--   0        0        0     3841 2023-03-15 14:01:49.116690 oianalytics-0.5.3/oianalytics/models/_template_resources/free_from_api_template.py
--rw-r--r--   0        0        0     2078 2023-03-15 14:01:49.116764 oianalytics-0.5.3/oianalytics/models/_template_resources/single_observation_template.py
--rw-r--r--   0        0        0    68166 2024-04-11 08:26:37.004822 oianalytics-0.5.3/oianalytics/models/outputs.py
--rw-r--r--   0        0        0      993 2023-11-06 09:30:13.506909 oianalytics-0.5.3/oianalytics/models/templates.py
--rw-r--r--   0        0        0      117 2023-03-15 14:01:49.117158 oianalytics-0.5.3/oianalytics/models/testing/__init__.py
--rw-r--r--   0        0        0    32133 2023-11-06 09:30:13.507306 oianalytics-0.5.3/oianalytics/models/testing/_mocking.py
--rw-r--r--   0        0        0     1067 2023-03-15 14:01:49.117460 oianalytics-0.5.3/oianalytics/models/testing/_tests_setup.py
--rw-r--r--   0        0        0     2811 2023-11-06 09:30:13.507566 oianalytics-0.5.3/oianalytics/models/testing/file_processing.py
--rw-r--r--   0        0        0     2710 2024-04-11 08:26:37.005487 oianalytics-0.5.3/oianalytics/models/testing/free_from_api.py
--rw-r--r--   0        0        0     7242 2023-11-06 09:30:13.508110 oianalytics-0.5.3/oianalytics/models/testing/single_observation.py
--rw-r--r--   0        0        0      256 2023-03-15 14:01:49.117791 oianalytics-0.5.3/oianalytics/models/utils.py
--rw-r--r--   0        0        0      475 2024-04-11 08:31:53.204621 oianalytics-0.5.3/pyproject.toml
--rw-r--r--   0        0        0      602 1970-01-01 00:00:00.000000 oianalytics-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0    13799 2023-03-15 14:01:49.113528 oianalytics-0.5.4b1/LICENSE
+-rw-r--r--   0        0        0       94 2024-05-30 13:52:44.876930 oianalytics-0.5.4b1/oianalytics/__init__.py
+-rw-r--r--   0        0        0      124 2024-02-12 10:28:03.022129 oianalytics-0.5.4b1/oianalytics/api/__init__.py
+-rw-r--r--   0        0        0     2373 2023-03-15 14:01:49.113932 oianalytics-0.5.4b1/oianalytics/api/_credentials.py
+-rw-r--r--   0        0        0     2442 2024-02-12 10:28:03.022426 oianalytics-0.5.4b1/oianalytics/api/_dataframes/__init__.py
+-rw-r--r--   0        0        0    16024 2023-11-06 09:30:13.500439 oianalytics-0.5.4b1/oianalytics/api/_dataframes/assets.py
+-rw-r--r--   0        0        0     3847 2023-11-06 09:30:13.500761 oianalytics-0.5.4b1/oianalytics/api/_dataframes/azure_blob_sources.py
+-rw-r--r--   0        0        0    48788 2024-02-12 10:28:03.022749 oianalytics-0.5.4b1/oianalytics/api/_dataframes/batches.py
+-rw-r--r--   0        0        0    41856 2023-10-30 14:56:38.145683 oianalytics-0.5.4b1/oianalytics/api/_dataframes/data.py
+-rw-r--r--   0        0        0     9979 2023-03-15 14:01:49.114785 oianalytics-0.5.4b1/oianalytics/api/_dataframes/events.py
+-rw-r--r--   0        0        0     4631 2023-03-15 14:01:49.114887 oianalytics-0.5.4b1/oianalytics/api/_dataframes/files.py
+-rw-r--r--   0        0        0     7991 2023-11-06 09:30:13.501670 oianalytics-0.5.4b1/oianalytics/api/_dataframes/model_instances.py
+-rw-r--r--   0        0        0     3933 2023-11-06 09:30:13.502064 oianalytics-0.5.4b1/oianalytics/api/_dataframes/profiles.py
+-rw-r--r--   0        0        0     2416 2023-10-30 14:56:38.146077 oianalytics-0.5.4b1/oianalytics/api/_dataframes/quantities.py
+-rw-r--r--   0        0        0     5581 2024-02-12 10:28:10.083841 oianalytics-0.5.4b1/oianalytics/api/_dataframes/tags.py
+-rw-r--r--   0        0        0     5463 2023-11-06 09:30:13.502604 oianalytics-0.5.4b1/oianalytics/api/_dataframes/units.py
+-rw-r--r--   0        0        0     4251 2023-11-06 09:30:13.502818 oianalytics-0.5.4b1/oianalytics/api/_dataframes/users.py
+-rw-r--r--   0        0        0      705 2024-04-11 08:26:37.003541 oianalytics-0.5.4b1/oianalytics/api/endpoints/__init__.py
+-rw-r--r--   0        0        0     5806 2024-02-12 10:28:03.023906 oianalytics-0.5.4b1/oianalytics/api/endpoints/assets.py
+-rw-r--r--   0        0        0     1437 2023-11-06 09:30:13.503405 oianalytics-0.5.4b1/oianalytics/api/endpoints/azure_blob_sources.py
+-rw-r--r--   0        0        0    11949 2024-02-12 10:28:03.024141 oianalytics-0.5.4b1/oianalytics/api/endpoints/batches.py
+-rw-r--r--   0        0        0     2646 2024-04-11 08:26:37.003805 oianalytics-0.5.4b1/oianalytics/api/endpoints/computation_jobs.py
+-rw-r--r--   0        0        0    13255 2023-11-06 09:30:13.503842 oianalytics-0.5.4b1/oianalytics/api/endpoints/data.py
+-rw-r--r--   0        0        0     2635 2023-11-06 09:30:13.504076 oianalytics-0.5.4b1/oianalytics/api/endpoints/events.py
+-rw-r--r--   0        0        0     3204 2023-11-06 09:30:13.504386 oianalytics-0.5.4b1/oianalytics/api/endpoints/files.py
+-rw-r--r--   0        0        0     1387 2023-11-06 09:30:13.504678 oianalytics-0.5.4b1/oianalytics/api/endpoints/model_instances.py
+-rw-r--r--   0        0        0     2779 2024-02-12 10:28:03.024389 oianalytics-0.5.4b1/oianalytics/api/endpoints/profiles.py
+-rw-r--r--   0        0        0      772 2023-10-30 14:56:38.147329 oianalytics-0.5.4b1/oianalytics/api/endpoints/quantities.py
+-rw-r--r--   0        0        0     4519 2024-02-12 10:28:10.090400 oianalytics-0.5.4b1/oianalytics/api/endpoints/tags.py
+-rw-r--r--   0        0        0     1787 2023-11-06 09:30:13.505426 oianalytics-0.5.4b1/oianalytics/api/endpoints/units.py
+-rw-r--r--   0        0        0     2170 2024-02-12 10:28:03.024745 oianalytics-0.5.4b1/oianalytics/api/endpoints/users.py
+-rw-r--r--   0        0        0     5881 2023-04-18 12:32:43.955607 oianalytics-0.5.4b1/oianalytics/api/utils.py
+-rw-r--r--   0        0        0      133 2023-03-15 14:01:49.115833 oianalytics-0.5.4b1/oianalytics/models/__init__.py
+-rw-r--r--   0        0        0    40900 2024-04-11 08:26:37.004294 oianalytics-0.5.4b1/oianalytics/models/_dtos.py
+-rw-r--r--   0        0        0      346 2023-04-18 12:32:43.955722 oianalytics-0.5.4b1/oianalytics/models/_queries/__init__.py
+-rw-r--r--   0        0        0     1965 2023-11-06 09:30:13.505992 oianalytics-0.5.4b1/oianalytics/models/_queries/files.py
+-rw-r--r--   0        0        0      727 2023-11-06 09:30:13.506204 oianalytics-0.5.4b1/oianalytics/models/_queries/instances.py
+-rw-r--r--   0        0        0    13883 2023-10-30 14:56:38.148516 oianalytics-0.5.4b1/oianalytics/models/_queries/single_observation.py
+-rw-r--r--   0        0        0        0 2023-03-15 14:01:49.116471 oianalytics-0.5.4b1/oianalytics/models/_template_resources/__init__.py
+-rw-r--r--   0        0        0     2796 2023-04-18 12:32:43.955950 oianalytics-0.5.4b1/oianalytics/models/_template_resources/file_processing_template.py
+-rw-r--r--   0        0        0     3841 2023-03-15 14:01:49.116690 oianalytics-0.5.4b1/oianalytics/models/_template_resources/free_from_api_template.py
+-rw-r--r--   0        0        0     2078 2023-03-15 14:01:49.116764 oianalytics-0.5.4b1/oianalytics/models/_template_resources/single_observation_template.py
+-rw-r--r--   0        0        0    74727 2024-05-30 12:36:11.343033 oianalytics-0.5.4b1/oianalytics/models/outputs.py
+-rw-r--r--   0        0        0      993 2023-11-06 09:30:13.506909 oianalytics-0.5.4b1/oianalytics/models/templates.py
+-rw-r--r--   0        0        0      117 2023-03-15 14:01:49.117158 oianalytics-0.5.4b1/oianalytics/models/testing/__init__.py
+-rw-r--r--   0        0        0    32133 2023-11-06 09:30:13.507306 oianalytics-0.5.4b1/oianalytics/models/testing/_mocking.py
+-rw-r--r--   0        0        0     1067 2023-03-15 14:01:49.117460 oianalytics-0.5.4b1/oianalytics/models/testing/_tests_setup.py
+-rw-r--r--   0        0        0     2811 2023-11-06 09:30:13.507566 oianalytics-0.5.4b1/oianalytics/models/testing/file_processing.py
+-rw-r--r--   0        0        0     2710 2024-04-11 08:26:37.005487 oianalytics-0.5.4b1/oianalytics/models/testing/free_from_api.py
+-rw-r--r--   0        0        0     7242 2023-11-06 09:30:13.508110 oianalytics-0.5.4b1/oianalytics/models/testing/single_observation.py
+-rw-r--r--   0        0        0      256 2023-03-15 14:01:49.117791 oianalytics-0.5.4b1/oianalytics/models/utils.py
+-rw-r--r--   0        0        0      477 2024-05-30 13:52:44.873438 oianalytics-0.5.4b1/pyproject.toml
+-rw-r--r--   0        0        0      604 1970-01-01 00:00:00.000000 oianalytics-0.5.4b1/PKG-INFO
```

### Comparing `oianalytics-0.5.3/LICENSE` & `oianalytics-0.5.4b1/LICENSE`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.3/oianalytics/api/_credentials.py` & `oianalytics-0.5.4b1/oianalytics/api/_credentials.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.3/oianalytics/api/_dataframes/__init__.py` & `oianalytics-0.5.4b1/oianalytics/api/_dataframes/__init__.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.3/oianalytics/api/_dataframes/assets.py` & `oianalytics-0.5.4b1/oianalytics/api/_dataframes/assets.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.3/oianalytics/api/_dataframes/azure_blob_sources.py` & `oianalytics-0.5.4b1/oianalytics/api/_dataframes/azure_blob_sources.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.3/oianalytics/api/_dataframes/batches.py` & `oianalytics-0.5.4b1/oianalytics/api/_dataframes/batches.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.3/oianalytics/api/_dataframes/data.py` & `oianalytics-0.5.4b1/oianalytics/api/_dataframes/data.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.3/oianalytics/api/_dataframes/events.py` & `oianalytics-0.5.4b1/oianalytics/api/_dataframes/events.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.3/oianalytics/api/_dataframes/files.py` & `oianalytics-0.5.4b1/oianalytics/api/_dataframes/files.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.3/oianalytics/api/_dataframes/model_instances.py` & `oianalytics-0.5.4b1/oianalytics/api/_dataframes/model_instances.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.3/oianalytics/api/_dataframes/profiles.py` & `oianalytics-0.5.4b1/oianalytics/api/_dataframes/profiles.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.3/oianalytics/api/_dataframes/quantities.py` & `oianalytics-0.5.4b1/oianalytics/api/_dataframes/quantities.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.3/oianalytics/api/_dataframes/tags.py` & `oianalytics-0.5.4b1/oianalytics/api/_dataframes/tags.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.3/oianalytics/api/_dataframes/units.py` & `oianalytics-0.5.4b1/oianalytics/api/_dataframes/units.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.3/oianalytics/api/_dataframes/users.py` & `oianalytics-0.5.4b1/oianalytics/api/_dataframes/users.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.3/oianalytics/api/endpoints/__init__.py` & `oianalytics-0.5.4b1/oianalytics/api/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.3/oianalytics/api/endpoints/assets.py` & `oianalytics-0.5.4b1/oianalytics/api/endpoints/assets.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.3/oianalytics/api/endpoints/azure_blob_sources.py` & `oianalytics-0.5.4b1/oianalytics/api/endpoints/azure_blob_sources.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.3/oianalytics/api/endpoints/batches.py` & `oianalytics-0.5.4b1/oianalytics/api/endpoints/batches.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.3/oianalytics/api/endpoints/computation_jobs.py` & `oianalytics-0.5.4b1/oianalytics/api/endpoints/computation_jobs.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.3/oianalytics/api/endpoints/data.py` & `oianalytics-0.5.4b1/oianalytics/api/endpoints/data.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.3/oianalytics/api/endpoints/events.py` & `oianalytics-0.5.4b1/oianalytics/api/endpoints/events.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.3/oianalytics/api/endpoints/files.py` & `oianalytics-0.5.4b1/oianalytics/api/endpoints/files.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.3/oianalytics/api/endpoints/model_instances.py` & `oianalytics-0.5.4b1/oianalytics/api/endpoints/model_instances.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.3/oianalytics/api/endpoints/profiles.py` & `oianalytics-0.5.4b1/oianalytics/api/endpoints/profiles.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.3/oianalytics/api/endpoints/quantities.py` & `oianalytics-0.5.4b1/oianalytics/api/endpoints/quantities.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.3/oianalytics/api/endpoints/tags.py` & `oianalytics-0.5.4b1/oianalytics/api/endpoints/tags.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.3/oianalytics/api/endpoints/units.py` & `oianalytics-0.5.4b1/oianalytics/api/endpoints/units.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.3/oianalytics/api/endpoints/users.py` & `oianalytics-0.5.4b1/oianalytics/api/endpoints/users.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.3/oianalytics/api/utils.py` & `oianalytics-0.5.4b1/oianalytics/api/utils.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.3/oianalytics/models/_dtos.py` & `oianalytics-0.5.4b1/oianalytics/models/_dtos.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.3/oianalytics/models/_queries/files.py` & `oianalytics-0.5.4b1/oianalytics/models/_queries/files.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.3/oianalytics/models/_queries/instances.py` & `oianalytics-0.5.4b1/oianalytics/models/_queries/instances.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.3/oianalytics/models/_queries/single_observation.py` & `oianalytics-0.5.4b1/oianalytics/models/_queries/single_observation.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.3/oianalytics/models/_template_resources/file_processing_template.py` & `oianalytics-0.5.4b1/oianalytics/models/_template_resources/file_processing_template.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.3/oianalytics/models/_template_resources/free_from_api_template.py` & `oianalytics-0.5.4b1/oianalytics/models/_template_resources/free_from_api_template.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.3/oianalytics/models/_template_resources/single_observation_template.py` & `oianalytics-0.5.4b1/oianalytics/models/_template_resources/single_observation_template.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.3/oianalytics/models/outputs.py` & `oianalytics-0.5.4b1/oianalytics/models/outputs.py`

 * *Files 18% similar despite different names*

```diff
@@ -50,36 +50,46 @@
     from_pandas(self, data, file_name, file_type):
         Initialize an instance of FileOutput with content from pandas.Series or pandas.DataFrame.
 
     send_to_oianalytics(self, api_credentials, execution_report, print_exceptions, raise_exceptions):
         Upload file to Oi Analytics.
     """
 
-    def __init__(self, file_name: str, content: Union[io.StringIO, io.BytesIO]):
+    def __init__(
+        self,
+        file_name: str,
+        content: Union[io.StringIO, io.BytesIO],
+        raise_exceptions_on_send: bool = True,
+        log_exceptions_if_not_raised: bool = True,
+    ):
         """
         Initialize a new instance of FileOutput.
 
         Parameters
         ----------
         file_name : str
             Name of the output file.
         content : io.StringIO | io.BytesIO
             Content of the output file.
         """
         self.output_type = "file"
         self.file_name = file_name
         self.content = content
+        self.raise_exceptions_on_send = raise_exceptions_on_send
+        self.log_exceptions_if_not_raised = log_exceptions_if_not_raised
 
     @classmethod
     def from_pandas(
         cls,
         data: Union[pd.Series, pd.DataFrame],
         file_name: str,
         file_type: str = "csv",
         writing_kwargs: Optional[dict] = None,
+        raise_exceptions_on_send: bool = True,
+        log_exceptions_if_not_raised: bool = True,
     ):
         """
         Initialize an instance of FileOutput with data from pandas.Series or pandas.DataFrame.
 
         Parameters
         ----------
         data : pandas.Series | pandas.DataFrame
@@ -108,63 +118,75 @@
         elif file_type == "csv":
             data.to_csv(bio, **writing_kwargs)
         else:
             raise NotImplementedError(f"Unsupported file_type: {file_type}")
         bio.seek(0)
 
         # Create object
-        return cls(file_name=file_name, content=bio)
+        return cls(
+            file_name=file_name,
+            content=bio,
+            raise_exceptions_on_send=raise_exceptions_on_send,
+            log_exceptions_if_not_raised=log_exceptions_if_not_raised,
+        )
 
     def send_to_oianalytics(
         self,
         api_credentials: Optional[api.OIAnalyticsAPICredentials] = None,
         execution_report: Optional[ExecutionReport] = None,
-        print_exceptions: bool = True,
-        raise_exceptions: bool = False,
+        raise_exceptions: Optional[bool] = None,
+        log_exceptions_if_not_raised: Optional[bool] = None,
         **kwargs,
     ) -> None:
         """
         Upload file to Oi Analytics.
 
         Parameters
         ----------
         api_credentials : api.OIAnalyticsAPICredentials, optional
-            The credentials to use to query the API. If None, previously set default credentials are used.
+            The credentials to use to query the API. If None, previously set default credentials are used
         execution_report : ExecutionReport, optional
-            Execution report for external use.
-        print_exceptions : bool, default True
-            Whether to print exception.
+            Execution report for external use
         raise_exceptions : bool, default False
-            Whether to raise exception.
+            Whether to raise exception
+        log_exceptions_if_not_raised : bool, default True
+            Whether to print exception
 
         Returns
         -------
         None
 
         """
+
+        # Init optional args
+        if raise_exceptions is None:
+            raise_exceptions = self.raise_exceptions_on_send
+        if log_exceptions_if_not_raised is None:
+            log_exceptions_if_not_raised = self.log_exceptions_if_not_raised
+
         # get execution report
         if execution_report is None:
             execution_report = get_default_execution_report()
         # update execution report
         try:
             response = api.endpoints.files.upload_file(
                 file_content=self.content,
                 file_name=self.file_name,
                 api_credentials=api_credentials,
             )
             execution_report.update(files_uploaded=1)
             return response
         except Exception:
             execution_report.update(errors=1)
-            if print_exceptions is True:
+            if raise_exceptions is True:
+                raise
+            if log_exceptions_if_not_raised is True:
                 print(
                     f"Error when trying to send to OIAnalytics:\n{traceback.format_exc()}"
                 )
-            if raise_exceptions is True:
-                raise
 
 
 class InstanceResourceOutput:
     """
     This class contains the content to be sent as an instance resource to Oi Analytics.
 
     Attributes
@@ -191,14 +213,16 @@
 
     def __init__(
         self,
         file_content: Union[io.StringIO, io.BytesIO],
         file_name: str,
         resource_file_id: str,
         model_instance_id: Optional[str] = None,
+        raise_exceptions_on_send: bool = True,
+        log_exceptions_if_not_raised: bool = True,
     ):
         """
         Initialize a new instance of InstanceResourceOutput.
 
         Parameters
         ----------
         file_content : io.StringIO | io.BytesIO
@@ -211,24 +235,28 @@
             Unique identifier of model instance.
         """
         self.output_type = "instance_resource"
         self.file_content = file_content
         self.file_name = file_name
         self.resource_file_id = resource_file_id
         self.model_instance_id = model_instance_id
+        self.raise_exceptions_on_send = raise_exceptions_on_send
+        self.log_exceptions_if_not_raised = log_exceptions_if_not_raised
 
     @classmethod
     def from_pandas(
         cls,
         data: Union[pd.Series, pd.DataFrame],
         file_name: str,
         resource_file_id: str,
         model_instance_id: Optional[str] = None,
         file_type: str = "csv",
         writing_kwargs: Optional[dict] = None,
+        raise_exceptions_on_send: bool = True,
+        log_exceptions_if_not_raised: bool = True,
     ):
         """Create InstanceResourceOutput object from a pandas.Series or a pandas.DataFrame.
 
         Parameters
         ----------
         data : pandas.Series, pandas.DataFrame
             Data of instance resource output.
@@ -265,42 +293,51 @@
 
         # Create object
         return cls(
             file_content=bio,
             file_name=file_name,
             resource_file_id=resource_file_id,
             model_instance_id=model_instance_id,
+            raise_exceptions_on_send=raise_exceptions_on_send,
+            log_exceptions_if_not_raised=log_exceptions_if_not_raised,
         )
 
     def send_to_oianalytics(
         self,
         api_credentials: Optional[api.OIAnalyticsAPICredentials] = None,
         execution_report: Optional[ExecutionReport] = None,
-        print_exceptions: bool = True,
-        raise_exceptions: bool = False,
+        raise_exceptions: Optional[bool] = None,
+        log_exceptions_if_not_raised: Optional[bool] = None,
         **kwargs,
     ) -> None:
         """
         Upload instance resource to Oi Analytics.
 
         Parameters
         ----------
         api_credentials : api.OIAnalyticsAPICredentials | None
             The credentials to use to query the API. If None, previously set default credentials are used.
         execution_report : ExecutionReport, optional
             Execution report for external use.
-        print_exceptions : bool, default True
+        log_exceptions_if_not_raised : bool, default True
             Whether to print exception.
         raise_exceptions : bool, default False
             Whether to raise exception.
 
         Returns
         -------
 
         """
+
+        # Init optional args
+        if raise_exceptions is None:
+            raise_exceptions = self.raise_exceptions_on_send
+        if log_exceptions_if_not_raised is None:
+            log_exceptions_if_not_raised = self.log_exceptions_if_not_raised
+
         # get execution report
         if execution_report is None:
             execution_report = get_default_execution_report()
         # update execution report
         execution_report.update(files_uploaded=1)
 
         try:
@@ -309,20 +346,20 @@
                 file_name=self.file_name,
                 resource_file_id=self.resource_file_id,
                 model_instance_id=self.model_instance_id,
                 api_credentials=api_credentials,
             )
         except Exception:
             execution_report.update(errors=1)
-            if print_exceptions is True:
+            if raise_exceptions is True:
+                raise
+            if log_exceptions_if_not_raised is True:
                 print(
                     f"Error when trying to send to OIAnalytics:\n{traceback.format_exc()}"
                 )
-            if raise_exceptions is True:
-                raise
 
 
 class TimeValuesOutput:
     """
     This class contains time values to be sent to Oi Analytics.
 
     Attributes
@@ -353,14 +390,16 @@
         self,
         data: Union[pd.Series, pd.DataFrame],
         units: Optional[dict] = None,
         rename_data: bool = True,
         use_external_reference: bool = False,
         timestamp_index_name: str = "timestamp",
         create_upload_event: Optional[bool] = None,
+        raise_exceptions_on_send: bool = True,
+        log_exceptions_if_not_raised: bool = True,
     ):
         """
         Initialize a new instance of TimeValuesOutput.
 
         Parameters
         ----------
         data : pandas.Series | pandas.DataFrame
@@ -411,20 +450,23 @@
         else:
             self.units = units
 
         self.use_external_reference = use_external_reference
 
         self.timestamp_index_name = timestamp_index_name
 
+        self.raise_exceptions_on_send = raise_exceptions_on_send
+        self.log_exceptions_if_not_raised = log_exceptions_if_not_raised
+
     def send_to_oianalytics(
         self,
         api_credentials: Optional[api.OIAnalyticsAPICredentials] = None,
         execution_report: Optional[ExecutionReport] = None,
-        print_exceptions: bool = True,
-        raise_exceptions: bool = False,
+        raise_exceptions: Optional[bool] = None,
+        log_exceptions_if_not_raised: Optional[bool] = None,
         create_upload_event: Optional[bool] = None,
     ) -> None:
         """
         Upload time values to Oi Analytics.
 
         Parameters
         ----------
@@ -440,14 +482,21 @@
             Whether to create a file upload event when uploading to Oi Analytics.
 
         Returns
         -------
         None
 
         """
+
+        # Init optional args
+        if raise_exceptions is None:
+            raise_exceptions = self.raise_exceptions_on_send
+        if log_exceptions_if_not_raised is None:
+            log_exceptions_if_not_raised = self.log_exceptions_if_not_raised
+
         # get execution report
         if execution_report is None:
             execution_report = get_default_execution_report()
 
         if create_upload_event is None:
             if self.create_upload_event is None:
                 model_exec = get_default_model_execution()
@@ -478,20 +527,20 @@
                     "numberOfValuesSuccessfullyInserted", 0
                 ),
                 errors=len(response.get("errors", [])),
             )
             return response
         except Exception:
             execution_report.update(errors=1)
-            if print_exceptions is True:
+            if raise_exceptions is True:
+                raise
+            if log_exceptions_if_not_raised is True:
                 print(
                     f"Error when trying to send to OIAnalytics:\n{traceback.format_exc()}"
                 )
-            if raise_exceptions is True:
-                raise
 
 
 class VectorTimeValuesOutput:
     """
     This class contains vector time values to be sent to Oi Analytics.
 
     Attributes
@@ -528,14 +577,16 @@
         data_reference: List[str],
         rename_data: bool = True,
         values_units: Optional[dict[str, str]] = None,
         index_units: Optional[dict[str, str]] = None,
         use_external_reference: bool = False,
         timestamp_index_name: str = "timestamp",
         create_upload_event: Optional[bool] = None,
+        raise_exceptions_on_send: bool = True,
+        log_exceptions_if_not_raised: bool = True,
     ):
         """
 
         Parameters
         ----------
         data : list of pandas.DataFrame
             List of vector time values.
@@ -606,20 +657,23 @@
         else:
             self.index_units = index_units
 
         self.use_external_reference = use_external_reference
 
         self.timestamp_index_name = timestamp_index_name
 
+        self.raise_exceptions_on_send = raise_exceptions_on_send
+        self.log_exceptions_if_not_raised = log_exceptions_if_not_raised
+
     def send_to_oianalytics(
         self,
         api_credentials: Optional[api.OIAnalyticsAPICredentials] = None,
         execution_report: Optional[ExecutionReport] = None,
-        print_exceptions: bool = True,
-        raise_exceptions: bool = False,
+        raise_exceptions: Optional[bool] = None,
+        log_exceptions_if_not_raised: Optional[bool] = None,
         create_upload_event: Optional[bool] = None,
     ) -> None:
         """
         Upload vector time values to Oi Analytics.
 
         Parameters
         ----------
@@ -635,14 +689,21 @@
             Whether to create a file upload event when uploading to Oi Analytics.
 
         Returns
         -------
         None
 
         """
+
+        # Init optional args
+        if raise_exceptions is None:
+            raise_exceptions = self.raise_exceptions_on_send
+        if log_exceptions_if_not_raised is None:
+            log_exceptions_if_not_raised = self.log_exceptions_if_not_raised
+
         # get execution report
         if execution_report is None:
             execution_report = get_default_execution_report()
 
         if create_upload_event is None:
             if self.create_upload_event is None:
                 model_exec = get_default_model_execution()
@@ -676,20 +737,20 @@
                 time_vector_values_updated=response.get(
                     "numberOfValuesSuccessfullyInserted", 0
                 ),
             )
             return response
         except Exception:
             execution_report.update(errors=1)
-            if print_exceptions is True:
+            if raise_exceptions is True:
+                raise
+            if log_exceptions_if_not_raised is True:
                 print(
                     f"Error when trying to send to OIAnalytics:\n{traceback.format_exc()}"
                 )
-            if raise_exceptions is True:
-                raise
 
 
 class BatchValuesOutput:
     """
     This class contains batch values to be sent to Oi Analytics.
 
     Attributes
@@ -715,14 +776,16 @@
         self,
         batch_type_id: str,
         data: Union[pd.Series, pd.DataFrame],
         units: Optional[dict] = None,
         batch_id_index_name: str = "batch_id",
         rename_data: bool = True,
         create_upload_event: Optional[bool] = None,
+        raise_exceptions_on_send: bool = True,
+        log_exceptions_if_not_raised: bool = True,
     ):
         """
 
         Parameters
         ----------
         batch_type_id : str
             Unique identifier of the batch type.
@@ -771,20 +834,23 @@
             else:
                 self.units = None
         else:
             self.units = units
 
         self.batch_id_index_name = batch_id_index_name
 
+        self.raise_exceptions_on_send = raise_exceptions_on_send
+        self.log_exceptions_if_not_raised = log_exceptions_if_not_raised
+
     def send_to_oianalytics(
         self,
         api_credentials: Optional[api.OIAnalyticsAPICredentials] = None,
         execution_report: Optional[ExecutionReport] = None,
-        print_exceptions: bool = True,
-        raise_exceptions: bool = False,
+        raise_exceptions: Optional[bool] = None,
+        log_exceptions_if_not_raised: Optional[bool] = None,
         create_upload_event: Optional[bool] = None,
     ) -> None:
         """
         Upload batch values to Oi Analytics.
 
         Parameters
         ----------
@@ -800,14 +866,21 @@
             Whether to create a file upload event when uploading to Oi Analytics.
 
         Returns
         -------
         None
 
         """
+
+        # Init optional args
+        if raise_exceptions is None:
+            raise_exceptions = self.raise_exceptions_on_send
+        if log_exceptions_if_not_raised is None:
+            log_exceptions_if_not_raised = self.log_exceptions_if_not_raised
+
         # get execution report
         if execution_report is None:
             execution_report = get_default_execution_report()
 
         if create_upload_event is None:
             if self.create_upload_event is None:
                 model_exec = get_default_model_execution()
@@ -834,20 +907,20 @@
             )
 
             # update execution report
             execution_report.update(batch_values_updated=int(self.data.count().sum()))
             return response
         except Exception:
             execution_report.update(errors=1)
-            if print_exceptions is True:
+            if raise_exceptions is True:
+                raise
+            if log_exceptions_if_not_raised is True:
                 print(
                     f"Error when trying to send to OIAnalytics:\n{traceback.format_exc()}"
                 )
-            if raise_exceptions is True:
-                raise
 
 
 class VectorBatchValuesOutput:
     """
     This class contains vector batch values to be sent to Oi Analytics.
 
     Attributes
@@ -878,14 +951,16 @@
         data: List[pd.DataFrame],
         data_reference: List[str],
         values_units: Optional[dict[str, str]] = None,
         index_units: Optional[dict[str, str]] = None,
         batch_id_index_name: str = "batch_id",
         rename_data: bool = True,
         create_upload_event: Optional[bool] = None,
+        raise_exceptions_on_send: bool = True,
+        log_exceptions_if_not_raised: bool = True,
     ):
         """
 
         Parameters
         ----------
         data : list of data
             List of batch vector values.
@@ -948,20 +1023,23 @@
                     if output_data.reference in data_reference
                 }
         else:
             self.index_units = index_units
 
         self.batch_id_index_name = batch_id_index_name
 
+        self.raise_exceptions_on_send = raise_exceptions_on_send
+        self.log_exceptions_if_not_raised = log_exceptions_if_not_raised
+
     def send_to_oianalytics(
         self,
         api_credentials: Optional[api.OIAnalyticsAPICredentials] = None,
         execution_report: Optional[ExecutionReport] = None,
-        print_exceptions: bool = True,
-        raise_exceptions: bool = False,
+        raise_exceptions: Optional[bool] = None,
+        log_exceptions_if_not_raised: Optional[bool] = None,
         create_upload_event: Optional[bool] = None,
     ) -> None:
         """
         Upload vector batch values to Oi Analytics.
 
         Parameters
         ----------
@@ -977,14 +1055,21 @@
             Whether to create a file upload event when uploading to Oi Analytics.
 
         Returns
         -------
         None
 
         """
+
+        # Init optional args
+        if raise_exceptions is None:
+            raise_exceptions = self.raise_exceptions_on_send
+        if log_exceptions_if_not_raised is None:
+            log_exceptions_if_not_raised = self.log_exceptions_if_not_raised
+
         # get execution report
         if execution_report is None:
             execution_report = get_default_execution_report()
 
         if create_upload_event is None:
             if self.create_upload_event is None:
                 model_exec = get_default_model_execution()
@@ -1017,20 +1102,20 @@
                 batch_vector_values_updated=response.get(
                     "numberOfValuesSuccessfullyInserted", 0
                 ),
             )
             return response
         except Exception:
             execution_report.update(errors=1)
-            if print_exceptions is True:
+            if raise_exceptions is True:
+                raise
+            if log_exceptions_if_not_raised is True:
                 print(
                     f"Error when trying to send to OIAnalytics:\n{traceback.format_exc()}"
                 )
-            if raise_exceptions is True:
-                raise
 
 
 class BatchFeaturesOutput:
     """
     This class contains batch features to be sent to Oi Analytics.
 
     Attributes
@@ -1055,14 +1140,16 @@
     def __init__(
         self,
         batch_type_id: str,
         data: Union[pd.Series, pd.DataFrame],
         rename_features: bool = True,
         batch_id_index_name: str = "batch_id",
         create_upload_event: Optional[bool] = None,
+        raise_exceptions_on_send: bool = True,
+        log_exceptions_if_not_raised: bool = True,
     ):
         """
         Initialize a new instance of BatchFeaturesOutput.
 
         Parameters
         ----------
         batch_type_id : str
@@ -1093,20 +1180,23 @@
             )
             self.data = data_df.rename(columns=output_dict)
         else:
             self.data = data_df
 
         self.batch_id_index_name = batch_id_index_name
 
+        self.raise_exceptions_on_send = raise_exceptions_on_send
+        self.log_exceptions_if_not_raised = log_exceptions_if_not_raised
+
     def send_to_oianalytics(
         self,
         api_credentials: Optional[api.OIAnalyticsAPICredentials] = None,
         execution_report: Optional[ExecutionReport] = None,
-        print_exceptions: bool = True,
-        raise_exceptions: bool = False,
+        raise_exceptions: Optional[bool] = None,
+        log_exceptions_if_not_raised: Optional[bool] = None,
         create_upload_event: Optional[bool] = None,
     ) -> None:
         """
         Upload batch features to Oi Analytics.
 
         Parameters
         ----------
@@ -1121,14 +1211,21 @@
         create_upload_event : bool, default True
             Whether to create a file upload event when uploading to Oi Analytics.
 
         Returns
         -------
 
         """
+
+        # Init optional args
+        if raise_exceptions is None:
+            raise_exceptions = self.raise_exceptions_on_send
+        if log_exceptions_if_not_raised is None:
+            log_exceptions_if_not_raised = self.log_exceptions_if_not_raised
+
         # update execution report
         if execution_report is None:
             execution_report = get_default_execution_report()
 
         if create_upload_event is None:
             if self.create_upload_event is None:
                 model_exec = get_default_model_execution()
@@ -1155,20 +1252,20 @@
             )
 
             # update execution report
             execution_report.update(batch_tags_updated=int(self.data.count().sum()))
             return response
         except Exception:
             execution_report.update(errors=1)
-            if print_exceptions is True:
+            if raise_exceptions is True:
+                raise
+            if log_exceptions_if_not_raised is True:
                 print(
                     f"Error when trying to send to OIAnalytics:\n{traceback.format_exc()}"
                 )
-            if raise_exceptions is True:
-                raise
 
 
 class BatchesOutput:
     """
     This class contains batches to be sent to Oi Analytics.
 
     Attributes
@@ -1239,14 +1336,16 @@
         batch_name_index_name: str = "batch_name",
         step_id_index_name: str = "step_id",
         start_date_name: str = "start",
         end_date_name: str = "end",
         asset_localisation_column: Optional[str] = None,
         tag_localisation_columns: Optional[Union[str, List[str]]] = None,
         create_upload_event: Optional[bool] = None,
+        raise_exceptions_on_send: bool = True,
+        log_exceptions_if_not_raised: bool = True,
     ):
         """
         Initialize a new instance of BatchesOutput.
 
         Parameters
         ----------
         batch_type_id : str
@@ -1383,20 +1482,23 @@
             else:
                 self.vector_data_values_units = None
         else:
             self.vector_data_references = vector_data_references
             self.vector_data_index_units = None
             self.vector_data_values_units = None
 
+        self.raise_exceptions_on_send = raise_exceptions_on_send
+        self.log_exceptions_if_not_raised = log_exceptions_if_not_raised
+
     def send_to_oianalytics(
         self,
         api_credentials: Optional[api.OIAnalyticsAPICredentials] = None,
         execution_report: Optional[ExecutionReport] = None,
-        print_exceptions: bool = True,
-        raise_exceptions: bool = False,
+        raise_exceptions: Optional[bool] = None,
+        log_exceptions_if_not_raised: Optional[bool] = None,
         create_upload_event: Optional[bool] = None,
     ) -> None:
         """
         Upload batches to Oi Analytics.
 
         Parameters
         ----------
@@ -1417,14 +1519,21 @@
             Upload batches to OI Analytics.
 
         Returns
         -------
         None
 
         """
+
+        # Init optional args
+        if raise_exceptions is None:
+            raise_exceptions = self.raise_exceptions_on_send
+        if log_exceptions_if_not_raised is None:
+            log_exceptions_if_not_raised = self.log_exceptions_if_not_raised
+
         # update execution report
         if execution_report is None:
             execution_report = get_default_execution_report()
 
         if create_upload_event is None:
             if self.create_upload_event is None:
                 model_exec = get_default_model_execution()
@@ -1463,20 +1572,20 @@
             )
 
             # update execution report
             execution_report.update(batch_created_updated=len(response))
             return response
         except Exception:
             execution_report.update(errors=1)
-            if print_exceptions is True:
+            if raise_exceptions is True:
+                raise
+            if log_exceptions_if_not_raised is True:
                 print(
                     f"Error when trying to send to OIAnalytics:\n{traceback.format_exc()}"
                 )
-            if raise_exceptions is True:
-                raise
 
 
 class Delay:
     """
     This class contains time delays to be added to the execution of a Python model.
 
     Attributes
@@ -1504,16 +1613,16 @@
         self.output_type = "delay"
         self.duration = duration
 
     def send_to_oianalytics(
         self,
         api_credentials: Optional[api.OIAnalyticsAPICredentials] = None,
         execution_report: Optional[ExecutionReport] = None,
-        print_exceptions: bool = True,
-        raise_exceptions: bool = False,
+        raise_exceptions: Optional[bool] = None,
+        log_exceptions_if_not_raised: Optional[bool] = None,
         **kwargs,
     ):
         """
         Add time delays to Python model execution in OI Analytics.
 
         Parameters
         ----------
@@ -1550,31 +1659,38 @@
 
     Methods
     -------
     send_to_oianalytics(self, api_credentials, execution_report, print_exceptions, raise_exceptions):
         Add the customized text to the Python model execution report.
     """
 
-    def __init__(self, content: str):
+    def __init__(
+        self,
+        content: str,
+        raise_exceptions_on_send: bool = True,
+        log_exceptions_if_not_raised: bool = True,
+    ):
         """
         Initialize a new instance of CustomTextOutput.
 
         Parameters
         ----------
         content : str
         """
         self.type = "text"
         self.content = content
+        self.raise_exceptions_on_send = raise_exceptions_on_send
+        self.log_exceptions_if_not_raised = log_exceptions_if_not_raised
 
     def send_to_oianalytics(
         self,
         api_credentials: Optional[api.OIAnalyticsAPICredentials] = None,
         execution_report: Optional[ExecutionReport] = None,
-        print_exceptions: bool = True,
-        raise_exceptions: bool = False,
+        raise_exceptions: Optional[bool] = None,
+        log_exceptions_if_not_raised: Optional[bool] = None,
         **kwargs,
     ) -> None:
         """
         Add the customized text to the Python model execution report.
 
         Parameters
         ----------
@@ -1588,31 +1704,38 @@
             Whether to raise exception.
 
         Returns
         -------
         None
 
         """
+
+        # Init optional args
+        if raise_exceptions is None:
+            raise_exceptions = self.raise_exceptions_on_send
+        if log_exceptions_if_not_raised is None:
+            log_exceptions_if_not_raised = self.log_exceptions_if_not_raised
+
         # Get the default execution report if not provided
         if execution_report is None:
             execution_report = get_default_execution_report()
 
         # Update the execution report
         try:
             execution_report.customOutput = CustomModelOutput(
                 type=self.type, content=self.content
             )
         except Exception:
             execution_report.update(errors=1)
-            if print_exceptions is True:
+            if raise_exceptions is True:
+                raise
+            if log_exceptions_if_not_raised is True:
                 print(
                     f"Error when trying to send to OIAnalytics:\n{traceback.format_exc()}"
                 )
-            if raise_exceptions is True:
-                raise
 
 
 class CustomJsonOutput:
     """
     This class contains customized json output to be added to the model execution report.
 
     Attributes
@@ -1624,30 +1747,37 @@
 
     Methods
     -------
     send_to_oianalytics(self, api_credentials, execution_report, print_exceptions, raise_exceptions):
         Add customized content to model execution report.
     """
 
-    def __init__(self, content):
+    def __init__(
+        self,
+        content,
+        raise_exceptions_on_send: bool = True,
+        log_exceptions_if_not_raised: bool = True,
+    ):
         """
 
         Parameters
         ----------
         content : list | str | dict
         """
         self.type = "json"
         self.content = content
+        self.raise_exceptions_on_send = raise_exceptions_on_send
+        self.log_exceptions_if_not_raised = log_exceptions_if_not_raised
 
     def send_to_oianalytics(
         self,
         api_credentials: Optional[api.OIAnalyticsAPICredentials] = None,
         execution_report: Optional[ExecutionReport] = None,
-        print_exceptions: bool = True,
-        raise_exceptions: bool = False,
+        raise_exceptions: Optional[bool] = None,
+        log_exceptions_if_not_raised: Optional[bool] = None,
         **kwargs,
     ):
         """
 
         Parameters
         ----------
         api_credentials : api.OIAnalyticsAPICredentials, optional
@@ -1659,31 +1789,38 @@
         raise_exceptions : bool, default False
             Whether to raise exception.
 
         Returns
         -------
 
         """
+
+        # Init optional args
+        if raise_exceptions is None:
+            raise_exceptions = self.raise_exceptions_on_send
+        if log_exceptions_if_not_raised is None:
+            log_exceptions_if_not_raised = self.log_exceptions_if_not_raised
+
         # Get the default execution report if not provided
         if execution_report is None:
             execution_report = get_default_execution_report()
 
         # Update the execution report
         try:
             execution_report.customOutput = CustomModelOutput(
                 type=self.type, content=self.content
             )
         except Exception:
             execution_report.update(errors=1)
-            if print_exceptions is True:
+            if raise_exceptions is True:
+                raise
+            if log_exceptions_if_not_raised is True:
                 print(
                     f"Error when trying to send to OIAnalytics:\n{traceback.format_exc()}"
                 )
-            if raise_exceptions is True:
-                raise
 
 
 class BatchComputationJob:
     """
     This class contains a command to create a batch computation job in OIAnalytics.
 
     Attributes
@@ -1699,14 +1836,16 @@
     """
 
     def __init__(
         self,
         batch_type_id: str,
         data_ids: Optional[List[str]] = None,
         batch_ids: Optional[List[str]] = None,
+        raise_exceptions_on_send: bool = True,
+        log_exceptions_if_not_raised: bool = True,
     ):
         """
         Initialize a new instance of BatchComputationJob
 
         Attributes
         ----------
         output_type : {'batch_computation_job'}
@@ -1719,21 +1858,23 @@
             List of batch IDs to be computed. If None, all batches are computed
         """
 
         self.output_type = "batch_computation_job"
         self.batch_type_id = batch_type_id
         self.data_ids = data_ids
         self.batch_ids = batch_ids
+        self.raise_exceptions_on_send = raise_exceptions_on_send
+        self.log_exceptions_if_not_raised = log_exceptions_if_not_raised
 
     def send_to_oianalytics(
         self,
         api_credentials: Optional[api.OIAnalyticsAPICredentials] = None,
         execution_report: Optional[ExecutionReport] = None,
-        print_exceptions: bool = True,
-        raise_exceptions: bool = False,
+        raise_exceptions: Optional[bool] = None,
+        log_exceptions_if_not_raised: Optional[bool] = None,
         **kwargs,
     ) -> None:
         """
         Send the batch computation job creation command to OIAnalytics
 
         Parameters
         ----------
@@ -1748,14 +1889,20 @@
 
         Returns
         -------
         dict
             ID and computation job type, with the keys 'id' and 'type'
         """
 
+        # Init optional args
+        if raise_exceptions is None:
+            raise_exceptions = self.raise_exceptions_on_send
+        if log_exceptions_if_not_raised is None:
+            log_exceptions_if_not_raised = self.log_exceptions_if_not_raised
+
         # update execution report
         if execution_report is None:
             execution_report = get_default_execution_report()
 
         # send data
         try:
             response = api.endpoints.computation_jobs.create_batch_computation_jobs(
@@ -1767,20 +1914,20 @@
 
             execution_report.update(batch_created_updated=len(self.batch_ids))
 
             return response
 
         except Exception:
             execution_report.update(errors=1)
-            if print_exceptions is True:
+            if raise_exceptions is True:
+                raise
+            if log_exceptions_if_not_raised is True:
                 print(
                     f"Error when trying to send to OIAnalytics:\n{traceback.format_exc()}"
                 )
-            if raise_exceptions is True:
-                raise
 
 
 class OIModelOutputs:
     """
     This class contains all the outputs objects to be sent to Oi Analytics.
 
     Attributes
@@ -1826,16 +1973,16 @@
         """
         self.model_outputs.append(output_object)
 
     def send_to_oianalytics(
         self,
         api_credentials: Optional[api.OIAnalyticsAPICredentials] = None,
         execution_report: Optional[ExecutionReport] = None,
-        print_exceptions: bool = True,
-        raise_exceptions: bool = False,
+        raise_exceptions: Optional[bool] = None,
+        log_exceptions_if_not_raised: Optional[bool] = None,
         create_upload_event: Optional[bool] = None,
     ) -> None:
         """
         Upload all model outputs to Oi Analytics.
 
         Parameters
         ----------
@@ -1855,11 +2002,11 @@
         None
 
         """
         for model_output in self.model_outputs:
             model_output.send_to_oianalytics(
                 api_credentials=api_credentials,
                 execution_report=execution_report,
-                print_exceptions=print_exceptions,
                 raise_exceptions=raise_exceptions,
+                log_exceptions_if_not_raised=log_exceptions_if_not_raised,
                 create_upload_event=create_upload_event,
             )
```

### Comparing `oianalytics-0.5.3/oianalytics/models/templates.py` & `oianalytics-0.5.4b1/oianalytics/models/templates.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.3/oianalytics/models/testing/_mocking.py` & `oianalytics-0.5.4b1/oianalytics/models/testing/_mocking.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.3/oianalytics/models/testing/_tests_setup.py` & `oianalytics-0.5.4b1/oianalytics/models/testing/_tests_setup.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.3/oianalytics/models/testing/file_processing.py` & `oianalytics-0.5.4b1/oianalytics/models/testing/file_processing.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.3/oianalytics/models/testing/free_from_api.py` & `oianalytics-0.5.4b1/oianalytics/models/testing/free_from_api.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.3/oianalytics/models/testing/single_observation.py` & `oianalytics-0.5.4b1/oianalytics/models/testing/single_observation.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.3/PKG-INFO` & `oianalytics-0.5.4b1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oianalytics
-Version: 0.5.3
+Version: 0.5.4b1
 Summary: Python tools for working with OIAnalytics
 License: EUPL-1.2
 Author: Optimistik SAS
 Author-email: arthur.martel@optimistik.fr
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
 Classifier: Programming Language :: Python :: 3
```

