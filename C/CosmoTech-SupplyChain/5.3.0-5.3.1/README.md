# Comparing `tmp/CosmoTech-SupplyChain-5.3.0.tar.gz` & `tmp/cosmotech_supplychain-5.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CosmoTech-SupplyChain-5.3.0.tar", last modified: Wed Apr 10 10:18:34 2024, max compression
+gzip compressed data, was "cosmotech_supplychain-5.3.1.tar", last modified: Fri May 31 10:11:52 2024, max compression
```

## Comparing `CosmoTech-SupplyChain-5.3.0.tar` & `cosmotech_supplychain-5.3.1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:18:34.923935 CosmoTech-SupplyChain-5.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:18:34.923935 CosmoTech-SupplyChain-5.3.0/CosmoTech_SupplyChain.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-10 10:18:34.000000 CosmoTech-SupplyChain-5.3.0/CosmoTech_SupplyChain.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-04-10 10:18:34.000000 CosmoTech-SupplyChain-5.3.0/CosmoTech_SupplyChain.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 10:18:34.000000 CosmoTech-SupplyChain-5.3.0/CosmoTech_SupplyChain.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-10 10:18:34.000000 CosmoTech-SupplyChain-5.3.0/CosmoTech_SupplyChain.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-10 10:18:34.000000 CosmoTech-SupplyChain-5.3.0/CosmoTech_SupplyChain.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-10 10:18:34.923935 CosmoTech-SupplyChain-5.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:18:34.911934 CosmoTech-SupplyChain-5.3.0/Supplychain/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:18:34.915934 CosmoTech-SupplyChain-5.3.0/Supplychain/Generic/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Generic/adt_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Generic/adx_and_file_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6617 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Generic/adx_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Generic/cosmo_api_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Generic/csv_folder_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Generic/csv_folder_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Generic/duration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Generic/excel_folder_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Generic/excel_folder_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Generic/folder_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Generic/json_folder_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Generic/json_folder_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Generic/memory_folder_io.py
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Generic/simulator_io.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Generic/storage_queue_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Generic/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:18:34.915934 CosmoTech-SupplyChain-5.3.0/Supplychain/Protocol/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Protocol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Protocol/cmaes_optimization_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (127)     8275 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Protocol/default_transformation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Protocol/multiprocessing_optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Protocol/objective_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Protocol/protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:18:34.919934 CosmoTech-SupplyChain-5.3.0/Supplychain/Run/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5535 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Run/cmaes_optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Run/consumers.py
--rw-r--r--   0 runner    (1001) docker     (127)    31559 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Run/local_sensitivity_analysis_comets.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Run/simulation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Run/simulation_comets.py
--rw-r--r--   0 runner    (1001) docker     (127)    20725 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Run/stochastic_optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)     7709 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Run/uncertainty_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    24482 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Run/uncertainty_analysis_comets.py
--rw-r--r--   0 runner    (1001) docker     (127)    19531 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Run/uncertainty_analysis_helper_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:18:34.919934 CosmoTech-SupplyChain-5.3.0/Supplychain/Schema/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6726 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Schema/adt_column_description.py
--rw-r--r--   0 runner    (1001) docker     (127)     5878 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Schema/default_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Schema/simulator_files_description.py
--rw-r--r--   0 runner    (1001) docker     (127)    24493 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Schema/validation_schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:18:34.919934 CosmoTech-SupplyChain-5.3.0/Supplychain/Transform/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7699 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Transform/complete_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)    41114 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Transform/from_dict_to_simulator.py
--rw-r--r--   0 runner    (1001) docker     (127)    14265 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Transform/from_dict_to_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     8326 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Transform/from_table_to_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)    52415 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Transform/from_table_to_dict_old.py
--rw-r--r--   0 runner    (1001) docker     (127)    15664 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Transform/patch_dict_with_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Transform/production_route.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:18:34.919934 CosmoTech-SupplyChain-5.3.0/Supplychain/Validate/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Validate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23908 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Validate/validate_dict.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:18:34.923935 CosmoTech-SupplyChain-5.3.0/Supplychain/Wrappers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Wrappers/environment_variables.py
--rw-r--r--   0 runner    (1001) docker     (127)    19839 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Wrappers/simulator.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 10:18:34.923935 CosmoTech-SupplyChain-5.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:11:52.773136 cosmotech_supplychain-5.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:11:52.773136 cosmotech_supplychain-5.3.1/CosmoTech_SupplyChain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-31 10:11:52.000000 cosmotech_supplychain-5.3.1/CosmoTech_SupplyChain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-05-31 10:11:52.000000 cosmotech_supplychain-5.3.1/CosmoTech_SupplyChain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 10:11:52.000000 cosmotech_supplychain-5.3.1/CosmoTech_SupplyChain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-31 10:11:52.000000 cosmotech_supplychain-5.3.1/CosmoTech_SupplyChain.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-31 10:11:52.000000 cosmotech_supplychain-5.3.1/CosmoTech_SupplyChain.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-31 10:11:46.000000 cosmotech_supplychain-5.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-31 10:11:52.773136 cosmotech_supplychain-5.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-05-31 10:11:46.000000 cosmotech_supplychain-5.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:11:52.765137 cosmotech_supplychain-5.3.1/Supplychain/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:11:52.765137 cosmotech_supplychain-5.3.1/Supplychain/Generic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 10:11:46.000000 cosmotech_supplychain-5.3.1/Supplychain/Generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-05-31 10:11:46.000000 cosmotech_supplychain-5.3.1/Supplychain/Generic/adt_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-31 10:11:46.000000 cosmotech_supplychain-5.3.1/Supplychain/Generic/adx_and_file_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6617 2024-05-31 10:11:46.000000 cosmotech_supplychain-5.3.1/Supplychain/Generic/adx_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-05-31 10:11:46.000000 cosmotech_supplychain-5.3.1/Supplychain/Generic/cosmo_api_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-05-31 10:11:46.000000 cosmotech_supplychain-5.3.1/Supplychain/Generic/csv_folder_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-31 10:11:46.000000 cosmotech_supplychain-5.3.1/Supplychain/Generic/csv_folder_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-31 10:11:46.000000 cosmotech_supplychain-5.3.1/Supplychain/Generic/duration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-31 10:11:46.000000 cosmotech_supplychain-5.3.1/Supplychain/Generic/excel_folder_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-05-31 10:11:46.000000 cosmotech_supplychain-5.3.1/Supplychain/Generic/excel_folder_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-31 10:11:46.000000 cosmotech_supplychain-5.3.1/Supplychain/Generic/folder_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-31 10:11:46.000000 cosmotech_supplychain-5.3.1/Supplychain/Generic/json_folder_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-31 10:11:46.000000 cosmotech_supplychain-5.3.1/Supplychain/Generic/json_folder_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-31 10:11:46.000000 cosmotech_supplychain-5.3.1/Supplychain/Generic/memory_folder_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-31 10:11:46.000000 cosmotech_supplychain-5.3.1/Supplychain/Generic/simulator_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-31 10:11:46.000000 cosmotech_supplychain-5.3.1/Supplychain/Generic/storage_queue_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-05-31 10:11:46.000000 cosmotech_supplychain-5.3.1/Supplychain/Generic/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:11:52.769137 cosmotech_supplychain-5.3.1/Supplychain/Protocol/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 10:11:46.000000 cosmotech_supplychain-5.3.1/Supplychain/Protocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-31 10:11:46.000000 cosmotech_supplychain-5.3.1/Supplychain/Protocol/cmaes_optimization_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8275 2024-05-31 10:11:46.000000 cosmotech_supplychain-5.3.1/Supplychain/Protocol/default_transformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-05-31 10:11:46.000000 cosmotech_supplychain-5.3.1/Supplychain/Protocol/multiprocessing_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-31 10:11:46.000000 cosmotech_supplychain-5.3.1/Supplychain/Protocol/objective_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-05-31 10:11:46.000000 cosmotech_supplychain-5.3.1/Supplychain/Protocol/protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:11:52.769137 cosmotech_supplychain-5.3.1/Supplychain/Run/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 10:11:46.000000 cosmotech_supplychain-5.3.1/Supplychain/Run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5535 2024-05-31 10:11:46.000000 cosmotech_supplychain-5.3.1/Supplychain/Run/cmaes_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-05-31 10:11:46.000000 cosmotech_supplychain-5.3.1/Supplychain/Run/consumers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31559 2024-05-31 10:11:46.000000 cosmotech_supplychain-5.3.1/Supplychain/Run/local_sensitivity_analysis_comets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-31 10:11:46.000000 cosmotech_supplychain-5.3.1/Supplychain/Run/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-31 10:11:46.000000 cosmotech_supplychain-5.3.1/Supplychain/Run/simulation_comets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20725 2024-05-31 10:11:46.000000 cosmotech_supplychain-5.3.1/Supplychain/Run/stochastic_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7709 2024-05-31 10:11:46.000000 cosmotech_supplychain-5.3.1/Supplychain/Run/uncertainty_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24482 2024-05-31 10:11:46.000000 cosmotech_supplychain-5.3.1/Supplychain/Run/uncertainty_analysis_comets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19531 2024-05-31 10:11:46.000000 cosmotech_supplychain-5.3.1/Supplychain/Run/uncertainty_analysis_helper_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:11:52.769137 cosmotech_supplychain-5.3.1/Supplychain/Schema/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 10:11:46.000000 cosmotech_supplychain-5.3.1/Supplychain/Schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6726 2024-05-31 10:11:46.000000 cosmotech_supplychain-5.3.1/Supplychain/Schema/adt_column_description.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5878 2024-05-31 10:11:46.000000 cosmotech_supplychain-5.3.1/Supplychain/Schema/default_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-05-31 10:11:46.000000 cosmotech_supplychain-5.3.1/Supplychain/Schema/simulator_files_description.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24493 2024-05-31 10:11:46.000000 cosmotech_supplychain-5.3.1/Supplychain/Schema/validation_schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:11:52.773136 cosmotech_supplychain-5.3.1/Supplychain/Transform/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 10:11:46.000000 cosmotech_supplychain-5.3.1/Supplychain/Transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7699 2024-05-31 10:11:46.000000 cosmotech_supplychain-5.3.1/Supplychain/Transform/complete_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41114 2024-05-31 10:11:46.000000 cosmotech_supplychain-5.3.1/Supplychain/Transform/from_dict_to_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14265 2024-05-31 10:11:46.000000 cosmotech_supplychain-5.3.1/Supplychain/Transform/from_dict_to_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8326 2024-05-31 10:11:46.000000 cosmotech_supplychain-5.3.1/Supplychain/Transform/from_table_to_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52415 2024-05-31 10:11:46.000000 cosmotech_supplychain-5.3.1/Supplychain/Transform/from_table_to_dict_old.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15664 2024-05-31 10:11:46.000000 cosmotech_supplychain-5.3.1/Supplychain/Transform/patch_dict_with_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-05-31 10:11:46.000000 cosmotech_supplychain-5.3.1/Supplychain/Transform/production_route.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:11:52.773136 cosmotech_supplychain-5.3.1/Supplychain/Validate/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 10:11:46.000000 cosmotech_supplychain-5.3.1/Supplychain/Validate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23908 2024-05-31 10:11:46.000000 cosmotech_supplychain-5.3.1/Supplychain/Validate/validate_dict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:11:52.773136 cosmotech_supplychain-5.3.1/Supplychain/Wrappers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 10:11:46.000000 cosmotech_supplychain-5.3.1/Supplychain/Wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-05-31 10:11:46.000000 cosmotech_supplychain-5.3.1/Supplychain/Wrappers/environment_variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19839 2024-05-31 10:11:46.000000 cosmotech_supplychain-5.3.1/Supplychain/Wrappers/simulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 10:11:46.000000 cosmotech_supplychain-5.3.1/Supplychain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 10:11:52.773136 cosmotech_supplychain-5.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-31 10:11:46.000000 cosmotech_supplychain-5.3.1/setup.py
```

### Comparing `CosmoTech-SupplyChain-5.3.0/CosmoTech_SupplyChain.egg-info/PKG-INFO` & `cosmotech_supplychain-5.3.1/CosmoTech_SupplyChain.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CosmoTech-SupplyChain
-Version: 5.3.0
+Version: 5.3.1
 Summary: A support package for SupplyChain
 Home-page: https://github.com/Cosmo-Tech/supplychain-python-library<
 Author: Alexis Fossart
 Author-email: alexis.fossart@cosmotech.com
 License: MIT
 License-File: LICENSE
 Requires-Dist: azure-core
```

### Comparing `CosmoTech-SupplyChain-5.3.0/CosmoTech_SupplyChain.egg-info/SOURCES.txt` & `cosmotech_supplychain-5.3.1/CosmoTech_SupplyChain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.3.0/LICENSE` & `cosmotech_supplychain-5.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.3.0/PKG-INFO` & `cosmotech_supplychain-5.3.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CosmoTech-SupplyChain
-Version: 5.3.0
+Version: 5.3.1
 Summary: A support package for SupplyChain
 Home-page: https://github.com/Cosmo-Tech/supplychain-python-library<
 Author: Alexis Fossart
 Author-email: alexis.fossart@cosmotech.com
 License: MIT
 License-File: LICENSE
 Requires-Dist: azure-core
```

### Comparing `CosmoTech-SupplyChain-5.3.0/README.md` & `cosmotech_supplychain-5.3.1/README.md`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.3.0/Supplychain/Generic/adt_writer.py` & `cosmotech_supplychain-5.3.1/Supplychain/Generic/adt_writer.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.3.0/Supplychain/Generic/adx_and_file_writer.py` & `cosmotech_supplychain-5.3.1/Supplychain/Generic/adx_and_file_writer.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.3.0/Supplychain/Generic/adx_wrapper.py` & `cosmotech_supplychain-5.3.1/Supplychain/Generic/adx_wrapper.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.3.0/Supplychain/Generic/cosmo_api_parameters.py` & `cosmotech_supplychain-5.3.1/Supplychain/Generic/cosmo_api_parameters.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.3.0/Supplychain/Generic/csv_folder_reader.py` & `cosmotech_supplychain-5.3.1/Supplychain/Generic/csv_folder_reader.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.3.0/Supplychain/Generic/csv_folder_writer.py` & `cosmotech_supplychain-5.3.1/Supplychain/Generic/csv_folder_writer.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.3.0/Supplychain/Generic/duration.py` & `cosmotech_supplychain-5.3.1/Supplychain/Generic/duration.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.3.0/Supplychain/Generic/excel_folder_reader.py` & `cosmotech_supplychain-5.3.1/Supplychain/Generic/excel_folder_reader.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.3.0/Supplychain/Generic/excel_folder_writer.py` & `cosmotech_supplychain-5.3.1/Supplychain/Generic/excel_folder_writer.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.3.0/Supplychain/Generic/folder_io.py` & `cosmotech_supplychain-5.3.1/Supplychain/Generic/folder_io.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.3.0/Supplychain/Generic/json_folder_reader.py` & `cosmotech_supplychain-5.3.1/Supplychain/Generic/json_folder_reader.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.3.0/Supplychain/Generic/json_folder_writer.py` & `cosmotech_supplychain-5.3.1/Supplychain/Generic/json_folder_writer.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.3.0/Supplychain/Generic/memory_folder_io.py` & `cosmotech_supplychain-5.3.1/Supplychain/Generic/memory_folder_io.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.3.0/Supplychain/Generic/simulator_io.py` & `cosmotech_supplychain-5.3.1/Supplychain/Generic/simulator_io.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.3.0/Supplychain/Generic/storage_queue_writer.py` & `cosmotech_supplychain-5.3.1/Supplychain/Generic/storage_queue_writer.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.3.0/Supplychain/Generic/timer.py` & `cosmotech_supplychain-5.3.1/Supplychain/Generic/timer.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.3.0/Supplychain/Protocol/cmaes_optimization_algorithm.py` & `cosmotech_supplychain-5.3.1/Supplychain/Protocol/cmaes_optimization_algorithm.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.3.0/Supplychain/Protocol/default_transformation.py` & `cosmotech_supplychain-5.3.1/Supplychain/Protocol/default_transformation.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.3.0/Supplychain/Protocol/multiprocessing_optimization.py` & `cosmotech_supplychain-5.3.1/Supplychain/Protocol/multiprocessing_optimization.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.3.0/Supplychain/Protocol/objective_functions.py` & `cosmotech_supplychain-5.3.1/Supplychain/Protocol/objective_functions.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.3.0/Supplychain/Protocol/protocol.py` & `cosmotech_supplychain-5.3.1/Supplychain/Protocol/protocol.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.3.0/Supplychain/Run/cmaes_optimization.py` & `cosmotech_supplychain-5.3.1/Supplychain/Run/cmaes_optimization.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.3.0/Supplychain/Run/consumers.py` & `cosmotech_supplychain-5.3.1/Supplychain/Run/consumers.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.3.0/Supplychain/Run/local_sensitivity_analysis_comets.py` & `cosmotech_supplychain-5.3.1/Supplychain/Run/local_sensitivity_analysis_comets.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.3.0/Supplychain/Run/simulation.py` & `cosmotech_supplychain-5.3.1/Supplychain/Run/simulation.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.3.0/Supplychain/Run/simulation_comets.py` & `cosmotech_supplychain-5.3.1/Supplychain/Run/simulation_comets.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.3.0/Supplychain/Run/stochastic_optimization.py` & `cosmotech_supplychain-5.3.1/Supplychain/Run/stochastic_optimization.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.3.0/Supplychain/Run/uncertainty_analysis.py` & `cosmotech_supplychain-5.3.1/Supplychain/Run/uncertainty_analysis.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.3.0/Supplychain/Run/uncertainty_analysis_comets.py` & `cosmotech_supplychain-5.3.1/Supplychain/Run/uncertainty_analysis_comets.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.3.0/Supplychain/Run/uncertainty_analysis_helper_functions.py` & `cosmotech_supplychain-5.3.1/Supplychain/Run/uncertainty_analysis_helper_functions.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.3.0/Supplychain/Schema/adt_column_description.py` & `cosmotech_supplychain-5.3.1/Supplychain/Schema/adt_column_description.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.3.0/Supplychain/Schema/default_values.py` & `cosmotech_supplychain-5.3.1/Supplychain/Schema/default_values.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.3.0/Supplychain/Schema/simulator_files_description.py` & `cosmotech_supplychain-5.3.1/Supplychain/Schema/simulator_files_description.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.3.0/Supplychain/Schema/validation_schemas.py` & `cosmotech_supplychain-5.3.1/Supplychain/Schema/validation_schemas.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.3.0/Supplychain/Transform/complete_dict.py` & `cosmotech_supplychain-5.3.1/Supplychain/Transform/complete_dict.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.3.0/Supplychain/Transform/from_dict_to_simulator.py` & `cosmotech_supplychain-5.3.1/Supplychain/Transform/from_dict_to_simulator.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.3.0/Supplychain/Transform/from_dict_to_table.py` & `cosmotech_supplychain-5.3.1/Supplychain/Transform/from_dict_to_table.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.3.0/Supplychain/Transform/from_table_to_dict.py` & `cosmotech_supplychain-5.3.1/Supplychain/Transform/from_table_to_dict.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.3.0/Supplychain/Transform/from_table_to_dict_old.py` & `cosmotech_supplychain-5.3.1/Supplychain/Transform/from_table_to_dict_old.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.3.0/Supplychain/Transform/patch_dict_with_parameters.py` & `cosmotech_supplychain-5.3.1/Supplychain/Transform/patch_dict_with_parameters.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.3.0/Supplychain/Transform/production_route.py` & `cosmotech_supplychain-5.3.1/Supplychain/Transform/production_route.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.3.0/Supplychain/Validate/validate_dict.py` & `cosmotech_supplychain-5.3.1/Supplychain/Validate/validate_dict.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.3.0/Supplychain/Wrappers/environment_variables.py` & `cosmotech_supplychain-5.3.1/Supplychain/Wrappers/environment_variables.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.3.0/Supplychain/Wrappers/simulator.py` & `cosmotech_supplychain-5.3.1/Supplychain/Wrappers/simulator.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.3.0/setup.py` & `cosmotech_supplychain-5.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 
 
-VERSION = "5.3.0"
+VERSION = "5.3.1"
 
 setuptools.setup(
     name='CosmoTech-SupplyChain',
     version=VERSION,
     author='Alexis Fossart',
     author_email='alexis.fossart@cosmotech.com',
     url='https://github.com/Cosmo-Tech/supplychain-python-library<',
```

