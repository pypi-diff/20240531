# Comparing `tmp/peptdeep-1.2.0.tar.gz` & `tmp/peptdeep-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peptdeep-1.2.0.tar", last modified: Wed May 29 20:21:27 2024, max compression
+gzip compressed data, was "peptdeep-1.2.1.tar", last modified: Fri May 31 01:26:54 2024, max compression
```

## Comparing `peptdeep-1.2.0.tar` & `peptdeep-1.2.1.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:21:27.427364 peptdeep-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11338 2024-05-29 20:20:55.000000 peptdeep-1.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-29 20:20:55.000000 peptdeep-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    40162 2024-05-29 20:21:27.427364 peptdeep-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    32229 2024-05-29 20:20:55.000000 peptdeep-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:21:27.403364 peptdeep-1.2.0/peptdeep/
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:21:27.407364 peptdeep-1.2.0/peptdeep/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-29 20:21:27.000000 peptdeep-1.2.0/peptdeep/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/_modidx.py
--rw-r--r--   0 runner    (1001) docker     (127)     5634 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/cli_argparse.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:21:27.407364 peptdeep-1.2.0/peptdeep/constants/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/constants/_const.py
--rw-r--r--   0 runner    (1001) docker     (127)     6838 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/constants/default_settings.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/constants/model_const.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/gui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:21:27.407364 peptdeep-1.2.0/peptdeep/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:21:27.407364 peptdeep-1.2.0/peptdeep/legacy/thermo_raw/
--rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/legacy/thermo_raw/THERMO_LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)   366080 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/legacy/thermo_raw/ThermoFisher.CommonCore.Data.dll
--rw-r--r--   0 runner    (1001) docker     (127)   620032 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/legacy/thermo_raw/ThermoFisher.CommonCore.RawFileReader.dll
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/legacy/thermo_raw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26311 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/legacy/thermo_raw/pyrawfilereader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:21:27.411364 peptdeep-1.2.0/peptdeep/mass_spec/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/mass_spec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/mass_spec/mass_calibration.py
--rw-r--r--   0 runner    (1001) docker     (127)    14257 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/mass_spec/match.py
--rw-r--r--   0 runner    (1001) docker     (127)    14590 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/mass_spec/ms_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:21:27.411364 peptdeep-1.2.0/peptdeep/model/
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/model/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    31537 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/model/building_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     4540 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/model/ccs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6362 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/model/charge.py
--rw-r--r--   0 runner    (1001) docker     (127)     4583 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/model/featurize.py
--rw-r--r--   0 runner    (1001) docker     (127)    15390 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/model/generic_property_prediction.py
--rw-r--r--   0 runner    (1001) docker     (127)    36564 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/model/model_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/model/model_shop.py
--rw-r--r--   0 runner    (1001) docker     (127)    26671 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/model/ms2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5421 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/model/rt.py
--rw-r--r--   0 runner    (1001) docker     (127)    18706 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/pipeline_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    40941 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/pretrained_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:21:27.411364 peptdeep-1.2.0/peptdeep/protein/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/protein/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7745 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/protein/fasta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:21:27.411364 peptdeep-1.2.0/peptdeep/psm_frag_reader/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/psm_frag_reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/psm_frag_reader/maxquant_frag_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/psm_frag_reader/psm_frag_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     6049 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/psm_frag_reader/psmlabel_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:21:27.415364 peptdeep-1.2.0/peptdeep/rescore/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/rescore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4139 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/rescore/fdr.py
--rw-r--r--   0 runner    (1001) docker     (127)    39596 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/rescore/feature_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)    16548 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/rescore/percolator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:21:27.415364 peptdeep-1.2.0/peptdeep/spec_lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/spec_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11995 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/spec_lib/library_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     7729 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/spec_lib/predict_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/spec_lib/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:21:27.415364 peptdeep-1.2.0/peptdeep/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/utils/_pyinstaller_hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/utils/device_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6403 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/utils/regression.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:21:27.415364 peptdeep-1.2.0/peptdeep/webui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/webui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16127 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/webui/library_ui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:21:27.415364 peptdeep-1.2.0/peptdeep/webui/logos/
--rw-r--r--   0 runner    (1001) docker     (127)   118381 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/webui/logos/peptdeep.ico
--rw-r--r--   0 runner    (1001) docker     (127)    20283 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/webui/logos/peptdeep.png
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/webui/main_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/webui/model_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/webui/rescore_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/webui/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/webui/server_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     5905 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/webui/settings_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/webui/startpage.py
--rw-r--r--   0 runner    (1001) docker     (127)    11148 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/webui/transfer_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     8451 2024-05-29 20:20:55.000000 peptdeep-1.2.0/peptdeep/webui/ui_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:21:27.419364 peptdeep-1.2.0/peptdeep.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    40162 2024-05-29 20:21:27.000000 peptdeep-1.2.0/peptdeep.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-05-29 20:21:27.000000 peptdeep-1.2.0/peptdeep.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 20:21:27.000000 peptdeep-1.2.0/peptdeep.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-29 20:21:27.000000 peptdeep-1.2.0/peptdeep.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-29 20:21:27.000000 peptdeep-1.2.0/peptdeep.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-29 20:21:27.000000 peptdeep-1.2.0/peptdeep.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-29 20:20:55.000000 peptdeep-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 20:21:27.427364 peptdeep-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-05-29 20:20:55.000000 peptdeep-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:21:27.419364 peptdeep-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-29 20:20:55.000000 peptdeep-1.2.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-29 20:20:55.000000 peptdeep-1.2.0/tests/test_gui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:26:54.597790 peptdeep-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11338 2024-05-31 01:26:29.000000 peptdeep-1.2.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-31 01:26:29.000000 peptdeep-1.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    40162 2024-05-31 01:26:54.593790 peptdeep-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    32229 2024-05-31 01:26:29.000000 peptdeep-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:26:54.573790 peptdeep-1.2.1/peptdeep/
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-31 01:26:29.000000 peptdeep-1.2.1/peptdeep/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:26:54.573790 peptdeep-1.2.1/peptdeep/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-31 01:26:54.000000 peptdeep-1.2.1/peptdeep/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 01:26:29.000000 peptdeep-1.2.1/peptdeep/_modidx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5634 2024-05-31 01:26:29.000000 peptdeep-1.2.1/peptdeep/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-05-31 01:26:29.000000 peptdeep-1.2.1/peptdeep/cli_argparse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:26:54.573790 peptdeep-1.2.1/peptdeep/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 01:26:29.000000 peptdeep-1.2.1/peptdeep/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-31 01:26:29.000000 peptdeep-1.2.1/peptdeep/constants/_const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6834 2024-05-31 01:26:29.000000 peptdeep-1.2.1/peptdeep/constants/default_settings.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-31 01:26:29.000000 peptdeep-1.2.1/peptdeep/constants/model_const.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-31 01:26:29.000000 peptdeep-1.2.1/peptdeep/gui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:26:54.573790 peptdeep-1.2.1/peptdeep/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-31 01:26:29.000000 peptdeep-1.2.1/peptdeep/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:26:54.577790 peptdeep-1.2.1/peptdeep/legacy/thermo_raw/
+-rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-05-31 01:26:29.000000 peptdeep-1.2.1/peptdeep/legacy/thermo_raw/THERMO_LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   366080 2024-05-31 01:26:29.000000 peptdeep-1.2.1/peptdeep/legacy/thermo_raw/ThermoFisher.CommonCore.Data.dll
+-rw-r--r--   0 runner    (1001) docker     (127)   620032 2024-05-31 01:26:29.000000 peptdeep-1.2.1/peptdeep/legacy/thermo_raw/ThermoFisher.CommonCore.RawFileReader.dll
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 01:26:29.000000 peptdeep-1.2.1/peptdeep/legacy/thermo_raw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26311 2024-05-31 01:26:29.000000 peptdeep-1.2.1/peptdeep/legacy/thermo_raw/pyrawfilereader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:26:54.577790 peptdeep-1.2.1/peptdeep/mass_spec/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-31 01:26:29.000000 peptdeep-1.2.1/peptdeep/mass_spec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-05-31 01:26:29.000000 peptdeep-1.2.1/peptdeep/mass_spec/mass_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14257 2024-05-31 01:26:29.000000 peptdeep-1.2.1/peptdeep/mass_spec/match.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14590 2024-05-31 01:26:29.000000 peptdeep-1.2.1/peptdeep/mass_spec/ms_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:26:54.581790 peptdeep-1.2.1/peptdeep/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-31 01:26:29.000000 peptdeep-1.2.1/peptdeep/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-31 01:26:29.000000 peptdeep-1.2.1/peptdeep/model/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31537 2024-05-31 01:26:29.000000 peptdeep-1.2.1/peptdeep/model/building_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4540 2024-05-31 01:26:29.000000 peptdeep-1.2.1/peptdeep/model/ccs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6362 2024-05-31 01:26:29.000000 peptdeep-1.2.1/peptdeep/model/charge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4583 2024-05-31 01:26:29.000000 peptdeep-1.2.1/peptdeep/model/featurize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15390 2024-05-31 01:26:29.000000 peptdeep-1.2.1/peptdeep/model/generic_property_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36564 2024-05-31 01:26:29.000000 peptdeep-1.2.1/peptdeep/model/model_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-31 01:26:29.000000 peptdeep-1.2.1/peptdeep/model/model_shop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26671 2024-05-31 01:26:29.000000 peptdeep-1.2.1/peptdeep/model/ms2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5421 2024-05-31 01:26:29.000000 peptdeep-1.2.1/peptdeep/model/rt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18706 2024-05-31 01:26:29.000000 peptdeep-1.2.1/peptdeep/pipeline_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40941 2024-05-31 01:26:29.000000 peptdeep-1.2.1/peptdeep/pretrained_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:26:54.581790 peptdeep-1.2.1/peptdeep/protein/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-31 01:26:29.000000 peptdeep-1.2.1/peptdeep/protein/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7745 2024-05-31 01:26:29.000000 peptdeep-1.2.1/peptdeep/protein/fasta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:26:54.581790 peptdeep-1.2.1/peptdeep/psm_frag_reader/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-31 01:26:29.000000 peptdeep-1.2.1/peptdeep/psm_frag_reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-05-31 01:26:29.000000 peptdeep-1.2.1/peptdeep/psm_frag_reader/maxquant_frag_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-31 01:26:29.000000 peptdeep-1.2.1/peptdeep/psm_frag_reader/psm_frag_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6049 2024-05-31 01:26:29.000000 peptdeep-1.2.1/peptdeep/psm_frag_reader/psmlabel_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:26:54.581790 peptdeep-1.2.1/peptdeep/rescore/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-31 01:26:29.000000 peptdeep-1.2.1/peptdeep/rescore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4139 2024-05-31 01:26:29.000000 peptdeep-1.2.1/peptdeep/rescore/fdr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39596 2024-05-31 01:26:29.000000 peptdeep-1.2.1/peptdeep/rescore/feature_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16548 2024-05-31 01:26:29.000000 peptdeep-1.2.1/peptdeep/rescore/percolator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-05-31 01:26:29.000000 peptdeep-1.2.1/peptdeep/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:26:54.581790 peptdeep-1.2.1/peptdeep/spec_lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 01:26:29.000000 peptdeep-1.2.1/peptdeep/spec_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11995 2024-05-31 01:26:29.000000 peptdeep-1.2.1/peptdeep/spec_lib/library_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7729 2024-05-31 01:26:29.000000 peptdeep-1.2.1/peptdeep/spec_lib/predict_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-31 01:26:29.000000 peptdeep-1.2.1/peptdeep/spec_lib/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:26:54.581790 peptdeep-1.2.1/peptdeep/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-05-31 01:26:29.000000 peptdeep-1.2.1/peptdeep/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-31 01:26:29.000000 peptdeep-1.2.1/peptdeep/utils/_pyinstaller_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-31 01:26:29.000000 peptdeep-1.2.1/peptdeep/utils/device_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6403 2024-05-31 01:26:29.000000 peptdeep-1.2.1/peptdeep/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-05-31 01:26:29.000000 peptdeep-1.2.1/peptdeep/utils/regression.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:26:54.585790 peptdeep-1.2.1/peptdeep/webui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 01:26:29.000000 peptdeep-1.2.1/peptdeep/webui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16127 2024-05-31 01:26:29.000000 peptdeep-1.2.1/peptdeep/webui/library_ui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:26:54.585790 peptdeep-1.2.1/peptdeep/webui/logos/
+-rw-r--r--   0 runner    (1001) docker     (127)   118381 2024-05-31 01:26:29.000000 peptdeep-1.2.1/peptdeep/webui/logos/peptdeep.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    20283 2024-05-31 01:26:29.000000 peptdeep-1.2.1/peptdeep/webui/logos/peptdeep.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-31 01:26:29.000000 peptdeep-1.2.1/peptdeep/webui/main_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-05-31 01:26:29.000000 peptdeep-1.2.1/peptdeep/webui/model_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-31 01:26:29.000000 peptdeep-1.2.1/peptdeep/webui/rescore_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-05-31 01:26:29.000000 peptdeep-1.2.1/peptdeep/webui/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-05-31 01:26:29.000000 peptdeep-1.2.1/peptdeep/webui/server_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5905 2024-05-31 01:26:29.000000 peptdeep-1.2.1/peptdeep/webui/settings_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-05-31 01:26:29.000000 peptdeep-1.2.1/peptdeep/webui/startpage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11148 2024-05-31 01:26:29.000000 peptdeep-1.2.1/peptdeep/webui/transfer_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8451 2024-05-31 01:26:29.000000 peptdeep-1.2.1/peptdeep/webui/ui_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:26:54.585790 peptdeep-1.2.1/peptdeep.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    40162 2024-05-31 01:26:54.000000 peptdeep-1.2.1/peptdeep.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-05-31 01:26:54.000000 peptdeep-1.2.1/peptdeep.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 01:26:54.000000 peptdeep-1.2.1/peptdeep.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-31 01:26:54.000000 peptdeep-1.2.1/peptdeep.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-31 01:26:54.000000 peptdeep-1.2.1/peptdeep.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-31 01:26:54.000000 peptdeep-1.2.1/peptdeep.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-31 01:26:29.000000 peptdeep-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 01:26:54.597790 peptdeep-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-05-31 01:26:29.000000 peptdeep-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:26:54.585790 peptdeep-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-31 01:26:29.000000 peptdeep-1.2.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-31 01:26:29.000000 peptdeep-1.2.1/tests/test_gui.py
```

### Comparing `peptdeep-1.2.0/LICENSE.txt` & `peptdeep-1.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `peptdeep-1.2.0/PKG-INFO` & `peptdeep-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peptdeep
-Version: 1.2.0
+Version: 1.2.1
 Summary: The AlphaX deep learning framework for Proteomics
 Home-page: https://github.com/MannLabs/peptdeep
 Author: Mann Labs
 Author-email: jalew.zwf@qq.com
 License: Apache 2.0
 Project-URL: Mann Labs at MPIB, https://www.biochem.mpg.de/mann
 Project-URL: Mann Labs at CPR, https://www.cpr.ku.dk/research/proteomics/mann/
```

### Comparing `peptdeep-1.2.0/README.md` & `peptdeep-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `peptdeep-1.2.0/peptdeep/__init__.py` & `peptdeep-1.2.1/peptdeep/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 #     from . import protein # rely on spec_lib, import after
 # except (ImportError,RuntimeError, OSError):
 #     # happends when installation
 #     pass
 
 __project__ = "peptdeep"
-__version__ = "1.2.0"
+__version__ = "1.2.1"
 __license__ = "Apache 2.0"
 __description__ = "The AlphaX deep learning framework for Proteomics"
 __author__ = "Mann Labs"
 __author_email__ = "jalew.zwf@qq.com"
 __github__ = "https://github.com/MannLabs/peptdeep"
 __doc__ = "https://alphapeptdeep.readthedocs.io/en/latest/"
 __pypi__ = "https://pypi.org/project/peptdeep/"
```

### Comparing `peptdeep-1.2.0/peptdeep/__pycache__/__init__.cpython-39.pyc` & `peptdeep-1.2.1/peptdeep/__pycache__/__init__.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed May 29 20:20:55 2024 UTC, .py size: 1673 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-00000000: 610d 0d0a 0000 0000 278e 5766 8906 0000  a.......'.Wf....
+00000000: 610d 0d0a 0000 0000 4527 5966 8906 0000  a.......E'Yf....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 5c00 0000 6400  .....@...s\...d.
 00000030: 5a00 6401 5a01 6402 5a02 6403 5a03 6404  Z.d.Z.d.Z.d.Z.d.
 00000040: 5a04 6405 5a05 6406 5a06 6407 5a07 6408  Z.d.Z.d.Z.d.Z.d.
 00000050: 5a08 6700 6409 a201 5a09 640a 5a0a 6700  Z.g.d...Z.d.Z.g.
 00000060: 640b a201 5a0b 640c 6701 5a0c 640d 640e  d...Z.d.g.Z.d.d.
 00000070: 6506 6507 6508 640f 9c05 5a0d 6410 6411  e.e.e.d...Z.d.d.
 00000080: 6412 9c02 5a0e 6413 5300 2914 da08 7065  d...Z.d.S.)...pe
-00000090: 7074 6465 6570 7a05 312e 322e 307a 0a41  ptdeepz.1.2.0z.A
+00000090: 7074 6465 6570 7a05 312e 322e 317a 0a41  ptdeepz.1.2.1z.A
 000000a0: 7061 6368 6520 322e 307a 3154 6865 2041  pache 2.0z1The A
 000000b0: 6c70 6861 5820 6465 6570 206c 6561 726e  lphaX deep learn
 000000c0: 696e 6720 6672 616d 6577 6f72 6b20 666f  ing framework fo
 000000d0: 7220 5072 6f74 656f 6d69 6373 7a09 4d61  r Proteomicsz.Ma
 000000e0: 6e6e 204c 6162 737a 106a 616c 6577 2e7a  nn Labsz.jalew.z
 000000f0: 7766 4071 712e 636f 6d7a 2468 7474 7073  wf@qq.comz$https
 00000100: 3a2f 2f67 6974 6875 622e 636f 6d2f 4d61  ://github.com/Ma
```

### Comparing `peptdeep-1.2.0/peptdeep/cli.py` & `peptdeep-1.2.1/peptdeep/cli.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.2.0/peptdeep/cli_argparse.py` & `peptdeep-1.2.1/peptdeep/cli_argparse.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.2.0/peptdeep/constants/default_settings.yaml` & `peptdeep-1.2.1/peptdeep/constants/default_settings.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
   - seq
   - modseq
   charge_model_file: ''
   charge_prob_cutoff: 0.3
   use_predicted_charge_in_speclib: True # if True, it ignores min/max_precursor_charge in `library`
   instrument_group:
     ThermoTOF: ThermoTOF
-    Astral: ThermoTOF
+    Astral: Lumos
     Lumos: Lumos
     QE: QE
     timsTOF: timsTOF
     SciexTOF: SciexTOF
     Fusion: Lumos
     Eclipse: Lumos
     Velos: Lumos # not important
```

### Comparing `peptdeep-1.2.0/peptdeep/constants/model_const.yaml` & `peptdeep-1.2.1/peptdeep/constants/model_const.yaml`

 * *Files identical despite different names*

### Comparing `peptdeep-1.2.0/peptdeep/gui.py` & `peptdeep-1.2.1/peptdeep/gui.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.2.0/peptdeep/legacy/thermo_raw/THERMO_LICENSE.txt` & `peptdeep-1.2.1/peptdeep/legacy/thermo_raw/THERMO_LICENSE.txt`

 * *Files identical despite different names*

### Comparing `peptdeep-1.2.0/peptdeep/legacy/thermo_raw/ThermoFisher.CommonCore.Data.dll` & `peptdeep-1.2.1/peptdeep/legacy/thermo_raw/ThermoFisher.CommonCore.Data.dll`

 * *Files identical despite different names*

### Comparing `peptdeep-1.2.0/peptdeep/legacy/thermo_raw/ThermoFisher.CommonCore.RawFileReader.dll` & `peptdeep-1.2.1/peptdeep/legacy/thermo_raw/ThermoFisher.CommonCore.RawFileReader.dll`

 * *Files identical despite different names*

### Comparing `peptdeep-1.2.0/peptdeep/legacy/thermo_raw/pyrawfilereader.py` & `peptdeep-1.2.1/peptdeep/legacy/thermo_raw/pyrawfilereader.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.2.0/peptdeep/mass_spec/mass_calibration.py` & `peptdeep-1.2.1/peptdeep/mass_spec/mass_calibration.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.2.0/peptdeep/mass_spec/match.py` & `peptdeep-1.2.1/peptdeep/mass_spec/match.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.2.0/peptdeep/mass_spec/ms_reader.py` & `peptdeep-1.2.1/peptdeep/mass_spec/ms_reader.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.2.0/peptdeep/model/building_block.py` & `peptdeep-1.2.1/peptdeep/model/building_block.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.2.0/peptdeep/model/ccs.py` & `peptdeep-1.2.1/peptdeep/model/ccs.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.2.0/peptdeep/model/charge.py` & `peptdeep-1.2.1/peptdeep/model/charge.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.2.0/peptdeep/model/featurize.py` & `peptdeep-1.2.1/peptdeep/model/featurize.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.2.0/peptdeep/model/generic_property_prediction.py` & `peptdeep-1.2.1/peptdeep/model/generic_property_prediction.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.2.0/peptdeep/model/model_interface.py` & `peptdeep-1.2.1/peptdeep/model/model_interface.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.2.0/peptdeep/model/ms2.py` & `peptdeep-1.2.1/peptdeep/model/ms2.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.2.0/peptdeep/model/rt.py` & `peptdeep-1.2.1/peptdeep/model/rt.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.2.0/peptdeep/pipeline_api.py` & `peptdeep-1.2.1/peptdeep/pipeline_api.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.2.0/peptdeep/pretrained_models.py` & `peptdeep-1.2.1/peptdeep/pretrained_models.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.2.0/peptdeep/protein/fasta.py` & `peptdeep-1.2.1/peptdeep/protein/fasta.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.2.0/peptdeep/psm_frag_reader/maxquant_frag_reader.py` & `peptdeep-1.2.1/peptdeep/psm_frag_reader/maxquant_frag_reader.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.2.0/peptdeep/psm_frag_reader/psm_frag_reader.py` & `peptdeep-1.2.1/peptdeep/psm_frag_reader/psm_frag_reader.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.2.0/peptdeep/psm_frag_reader/psmlabel_reader.py` & `peptdeep-1.2.1/peptdeep/psm_frag_reader/psmlabel_reader.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.2.0/peptdeep/rescore/fdr.py` & `peptdeep-1.2.1/peptdeep/rescore/fdr.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.2.0/peptdeep/rescore/feature_extractor.py` & `peptdeep-1.2.1/peptdeep/rescore/feature_extractor.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.2.0/peptdeep/rescore/percolator.py` & `peptdeep-1.2.1/peptdeep/rescore/percolator.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.2.0/peptdeep/settings.py` & `peptdeep-1.2.1/peptdeep/settings.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.2.0/peptdeep/spec_lib/library_factory.py` & `peptdeep-1.2.1/peptdeep/spec_lib/library_factory.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.2.0/peptdeep/spec_lib/predict_lib.py` & `peptdeep-1.2.1/peptdeep/spec_lib/predict_lib.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.2.0/peptdeep/utils/__init__.py` & `peptdeep-1.2.1/peptdeep/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.2.0/peptdeep/utils/_pyinstaller_hooks.py` & `peptdeep-1.2.1/peptdeep/utils/_pyinstaller_hooks.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.2.0/peptdeep/utils/device_utils.py` & `peptdeep-1.2.1/peptdeep/utils/device_utils.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.2.0/peptdeep/utils/logger.py` & `peptdeep-1.2.1/peptdeep/utils/logger.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.2.0/peptdeep/utils/regression.py` & `peptdeep-1.2.1/peptdeep/utils/regression.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.2.0/peptdeep/webui/library_ui.py` & `peptdeep-1.2.1/peptdeep/webui/library_ui.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.2.0/peptdeep/webui/logos/peptdeep.ico` & `peptdeep-1.2.1/peptdeep/webui/logos/peptdeep.ico`

 * *Files identical despite different names*

### Comparing `peptdeep-1.2.0/peptdeep/webui/logos/peptdeep.png` & `peptdeep-1.2.1/peptdeep/webui/logos/peptdeep.png`

 * *Files identical despite different names*

### Comparing `peptdeep-1.2.0/peptdeep/webui/main_ui.py` & `peptdeep-1.2.1/peptdeep/webui/main_ui.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.2.0/peptdeep/webui/model_ui.py` & `peptdeep-1.2.1/peptdeep/webui/model_ui.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.2.0/peptdeep/webui/rescore_ui.py` & `peptdeep-1.2.1/peptdeep/webui/rescore_ui.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.2.0/peptdeep/webui/server.py` & `peptdeep-1.2.1/peptdeep/webui/server.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.2.0/peptdeep/webui/server_ui.py` & `peptdeep-1.2.1/peptdeep/webui/server_ui.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.2.0/peptdeep/webui/settings_ui.py` & `peptdeep-1.2.1/peptdeep/webui/settings_ui.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.2.0/peptdeep/webui/startpage.py` & `peptdeep-1.2.1/peptdeep/webui/startpage.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.2.0/peptdeep/webui/transfer_ui.py` & `peptdeep-1.2.1/peptdeep/webui/transfer_ui.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.2.0/peptdeep/webui/ui_utils.py` & `peptdeep-1.2.1/peptdeep/webui/ui_utils.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.2.0/peptdeep.egg-info/PKG-INFO` & `peptdeep-1.2.1/peptdeep.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peptdeep
-Version: 1.2.0
+Version: 1.2.1
 Summary: The AlphaX deep learning framework for Proteomics
 Home-page: https://github.com/MannLabs/peptdeep
 Author: Mann Labs
 Author-email: jalew.zwf@qq.com
 License: Apache 2.0
 Project-URL: Mann Labs at MPIB, https://www.biochem.mpg.de/mann
 Project-URL: Mann Labs at CPR, https://www.cpr.ku.dk/research/proteomics/mann/
```

### Comparing `peptdeep-1.2.0/peptdeep.egg-info/SOURCES.txt` & `peptdeep-1.2.1/peptdeep.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `peptdeep-1.2.0/peptdeep.egg-info/requires.txt` & `peptdeep-1.2.1/peptdeep.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `peptdeep-1.2.0/setup.py` & `peptdeep-1.2.1/setup.py`

 * *Files identical despite different names*

