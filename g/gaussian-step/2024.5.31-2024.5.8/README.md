# Comparing `tmp/gaussian_step-2024.5.31.tar.gz` & `tmp/gaussian_step-2024.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaussian_step-2024.5.31.tar", last modified: Fri May 31 20:16:46 2024, max compression
+gzip compressed data, was "gaussian_step-2024.5.8.tar", last modified: Thu May  9 10:32:05 2024, max compression
```

## Comparing `gaussian_step-2024.5.31.tar` & `gaussian_step-2024.5.8.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:16:46.704220 gaussian_step-2024.5.31/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-31 20:16:38.000000 gaussian_step-2024.5.31/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-05-31 20:16:38.000000 gaussian_step-2024.5.31/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-05-31 20:16:38.000000 gaussian_step-2024.5.31/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-31 20:16:38.000000 gaussian_step-2024.5.31/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-31 20:16:38.000000 gaussian_step-2024.5.31/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6075 2024-05-31 20:16:46.704220 gaussian_step-2024.5.31/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-05-31 20:16:38.000000 gaussian_step-2024.5.31/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:16:46.696220 gaussian_step-2024.5.31/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     6790 2024-05-31 20:16:38.000000 gaussian_step-2024.5.31/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:16:46.696220 gaussian_step-2024.5.31/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    20790 2024-05-31 20:16:38.000000 gaussian_step-2024.5.31/docs/_static/SEAMM inverted.png
--rw-r--r--   0 runner    (1001) docker     (127)    17802 2024-05-31 20:16:38.000000 gaussian_step-2024.5.31/docs/_static/SEAMM logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    79373 2024-05-31 20:16:38.000000 gaussian_step-2024.5.31/docs/_static/molssi_main_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    68255 2024-05-31 20:16:38.000000 gaussian_step-2024.5.31/docs/_static/molssi_main_logo_inverted_white.png
--rw-r--r--   0 runner    (1001) docker     (127)    63967 2024-05-31 20:16:38.000000 gaussian_step-2024.5.31/docs/_static/molssi_square.png
--rw-r--r--   0 runner    (1001) docker     (127)    32355 2024-05-31 20:16:38.000000 gaussian_step-2024.5.31/docs/_static/nsf.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:16:46.696220 gaussian_step-2024.5.31/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-31 20:16:38.000000 gaussian_step-2024.5.31/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-31 20:16:38.000000 gaussian_step-2024.5.31/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)     9564 2024-05-31 20:16:38.000000 gaussian_step-2024.5.31/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:16:46.700220 gaussian_step-2024.5.31/docs/developer_guide/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-31 20:16:38.000000 gaussian_step-2024.5.31/docs/developer_guide/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-31 20:16:38.000000 gaussian_step-2024.5.31/docs/developer_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-31 20:16:38.000000 gaussian_step-2024.5.31/docs/developer_guide/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-31 20:16:38.000000 gaussian_step-2024.5.31/docs/developer_guide/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:16:46.700220 gaussian_step-2024.5.31/docs/getting_started/
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-31 20:16:38.000000 gaussian_step-2024.5.31/docs/getting_started/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-31 20:16:38.000000 gaussian_step-2024.5.31/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-31 20:16:38.000000 gaussian_step-2024.5.31/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6715 2024-05-31 20:16:38.000000 gaussian_step-2024.5.31/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:16:46.700220 gaussian_step-2024.5.31/docs/user_guide/
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-31 20:16:38.000000 gaussian_step-2024.5.31/docs/user_guide/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:16:46.704220 gaussian_step-2024.5.31/gaussian_step/
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-31 20:16:38.000000 gaussian_step-2024.5.31/gaussian_step/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-31 20:16:46.704220 gaussian_step-2024.5.31/gaussian_step/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:16:46.704220 gaussian_step-2024.5.31/gaussian_step/data/
--rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-05-31 20:16:38.000000 gaussian_step-2024.5.31/gaussian_step/data/gaussian.ini
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-31 20:16:38.000000 gaussian_step-2024.5.31/gaussian_step/data/properties.csv
--rw-r--r--   0 runner    (1001) docker     (127)     4827 2024-05-31 20:16:38.000000 gaussian_step-2024.5.31/gaussian_step/data/references.bib
--rw-r--r--   0 runner    (1001) docker     (127)    23273 2024-05-31 20:16:38.000000 gaussian_step-2024.5.31/gaussian_step/energy.py
--rw-r--r--   0 runner    (1001) docker     (127)    10863 2024-05-31 20:16:38.000000 gaussian_step-2024.5.31/gaussian_step/energy_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-31 20:16:38.000000 gaussian_step-2024.5.31/gaussian_step/energy_step.py
--rw-r--r--   0 runner    (1001) docker     (127)    11018 2024-05-31 20:16:38.000000 gaussian_step-2024.5.31/gaussian_step/gaussian.py
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-31 20:16:38.000000 gaussian_step-2024.5.31/gaussian_step/gaussian_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-31 20:16:38.000000 gaussian_step-2024.5.31/gaussian_step/gaussian_step.py
--rw-r--r--   0 runner    (1001) docker     (127)    38084 2024-05-31 20:16:38.000000 gaussian_step-2024.5.31/gaussian_step/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     9169 2024-05-31 20:16:38.000000 gaussian_step-2024.5.31/gaussian_step/optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3970 2024-05-31 20:16:38.000000 gaussian_step-2024.5.31/gaussian_step/optimization_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-31 20:16:38.000000 gaussian_step-2024.5.31/gaussian_step/optimization_step.py
--rw-r--r--   0 runner    (1001) docker     (127)    41086 2024-05-31 20:16:38.000000 gaussian_step-2024.5.31/gaussian_step/substep.py
--rw-r--r--   0 runner    (1001) docker     (127)    11977 2024-05-31 20:16:38.000000 gaussian_step-2024.5.31/gaussian_step/tk_energy.py
--rw-r--r--   0 runner    (1001) docker     (127)     6724 2024-05-31 20:16:38.000000 gaussian_step-2024.5.31/gaussian_step/tk_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (127)     4676 2024-05-31 20:16:38.000000 gaussian_step-2024.5.31/gaussian_step/tk_optimization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:16:46.704220 gaussian_step-2024.5.31/gaussian_step.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6075 2024-05-31 20:16:46.000000 gaussian_step-2024.5.31/gaussian_step.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-05-31 20:16:46.000000 gaussian_step-2024.5.31/gaussian_step.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 20:16:46.000000 gaussian_step-2024.5.31/gaussian_step.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-31 20:16:46.000000 gaussian_step-2024.5.31/gaussian_step.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-31 20:16:46.000000 gaussian_step-2024.5.31/gaussian_step.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-31 20:16:46.000000 gaussian_step-2024.5.31/gaussian_step.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 20:16:41.000000 gaussian_step-2024.5.31/gaussian_step.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-31 20:16:38.000000 gaussian_step-2024.5.31/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-31 20:16:38.000000 gaussian_step-2024.5.31/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-31 20:16:38.000000 gaussian_step-2024.5.31/requirements_install.txt
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-31 20:16:46.704220 gaussian_step-2024.5.31/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-05-31 20:16:38.000000 gaussian_step-2024.5.31/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:16:46.704220 gaussian_step-2024.5.31/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-31 20:16:38.000000 gaussian_step-2024.5.31/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-31 20:16:38.000000 gaussian_step-2024.5.31/tests/test_gaussian_step.py
--rw-r--r--   0 runner    (1001) docker     (127)    68610 2024-05-31 20:16:38.000000 gaussian_step-2024.5.31/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:32:05.537320 gaussian_step-2024.5.8/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5447 2024-05-09 10:32:05.537320 gaussian_step-2024.5.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:32:05.529320 gaussian_step-2024.5.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6790 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:32:05.533320 gaussian_step-2024.5.8/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    20790 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/docs/_static/SEAMM inverted.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17802 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/docs/_static/SEAMM logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    79373 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/docs/_static/molssi_main_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    68255 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/docs/_static/molssi_main_logo_inverted_white.png
+-rw-r--r--   0 runner    (1001) docker     (127)    63967 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/docs/_static/molssi_square.png
+-rw-r--r--   0 runner    (1001) docker     (127)    32355 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/docs/_static/nsf.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:32:05.533320 gaussian_step-2024.5.8/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9564 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:32:05.533320 gaussian_step-2024.5.8/docs/developer_guide/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/docs/developer_guide/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/docs/developer_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/docs/developer_guide/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/docs/developer_guide/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:32:05.533320 gaussian_step-2024.5.8/docs/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/docs/getting_started/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6715 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:32:05.533320 gaussian_step-2024.5.8/docs/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/docs/user_guide/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:32:05.541319 gaussian_step-2024.5.8/gaussian_step/
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/gaussian_step/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-09 10:32:05.541319 gaussian_step-2024.5.8/gaussian_step/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:32:05.537320 gaussian_step-2024.5.8/gaussian_step/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/gaussian_step/data/gaussian.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/gaussian_step/data/properties.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4827 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/gaussian_step/data/references.bib
+-rw-r--r--   0 runner    (1001) docker     (127)    21579 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/gaussian_step/energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10863 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/gaussian_step/energy_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/gaussian_step/energy_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10849 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/gaussian_step/gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/gaussian_step/gaussian_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/gaussian_step/gaussian_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36943 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/gaussian_step/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7389 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/gaussian_step/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/gaussian_step/optimization_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/gaussian_step/optimization_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39787 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/gaussian_step/substep.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11977 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/gaussian_step/tk_energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6724 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/gaussian_step/tk_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4468 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/gaussian_step/tk_optimization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:32:05.537320 gaussian_step-2024.5.8/gaussian_step.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5447 2024-05-09 10:32:05.000000 gaussian_step-2024.5.8/gaussian_step.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-05-09 10:32:05.000000 gaussian_step-2024.5.8/gaussian_step.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 10:32:05.000000 gaussian_step-2024.5.8/gaussian_step.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-09 10:32:05.000000 gaussian_step-2024.5.8/gaussian_step.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-09 10:32:05.000000 gaussian_step-2024.5.8/gaussian_step.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-09 10:32:05.000000 gaussian_step-2024.5.8/gaussian_step.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 10:31:52.000000 gaussian_step-2024.5.8/gaussian_step.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/requirements_install.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-09 10:32:05.541319 gaussian_step-2024.5.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:32:05.537320 gaussian_step-2024.5.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/tests/test_gaussian_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68610 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/versioneer.py
```

### Comparing `gaussian_step-2024.5.31/CONTRIBUTING.rst` & `gaussian_step-2024.5.8/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.5.31/HISTORY.rst` & `gaussian_step-2024.5.8/HISTORY.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,10 @@
 =======
 History
 =======
-2024.5.31: Added optimization of transition states, and...
-    * Corrected implementation of composite methods (Gn, CBS-x) to handle optimization.
-    * Added target of the optimization to allow transition states and saddle points.
-    * Corrected a bug in handling the maximum number of optimization steps.
-    * Corrected bug determining if optimization completed properly.
-    * Corrected bug handling the composite method results.
-      
-2024.5.27: Added number of optimization steps to results
-    * Added the number of steps for the optimizations to the results that can be output
-      to tables, variables, etc.
-      
 2024.5.8 General enhancements
     * Updated to new calculation handling, with ~/SEAMM/gaussian.ini controlling access
       to the installed version of Gaussian on the machine.
     * Added energy and gradients to results to support general use in e.g. energy scans.
 
 2024.1.19: Switched to new way to run Gaussian, added option to just write input file
     * Switched to using the new way to run executables, which supports containers.
```

### Comparing `gaussian_step-2024.5.31/LICENSE` & `gaussian_step-2024.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.5.31/PKG-INFO` & `gaussian_step-2024.5.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaussian_step
-Version: 2024.5.31
+Version: 2024.5.8
 Summary: A SEAMM plugin for A SEAMM plug-in for Gaussian
 Home-page: https://github.com/molssi-seamm/gaussian_step
 Author: Paul Saxe
 Author-email: psaxe@vt.edu
 License: BSD-3-Clause
 Keywords: SEAMM,SEAMMplugin,flowchart
 Platform: Linux
@@ -86,25 +86,14 @@
 .. _MolSSI: https://molssi.org
 .. _`National Science Foundation`: https://www.nsf.gov
 
 
 =======
 History
 =======
-2024.5.31: Added optimization of transition states, and...
-    * Corrected implementation of composite methods (Gn, CBS-x) to handle optimization.
-    * Added target of the optimization to allow transition states and saddle points.
-    * Corrected a bug in handling the maximum number of optimization steps.
-    * Corrected bug determining if optimization completed properly.
-    * Corrected bug handling the composite method results.
-      
-2024.5.27: Added number of optimization steps to results
-    * Added the number of steps for the optimizations to the results that can be output
-      to tables, variables, etc.
-      
 2024.5.8 General enhancements
     * Updated to new calculation handling, with ~/SEAMM/gaussian.ini controlling access
       to the installed version of Gaussian on the machine.
     * Added energy and gradients to results to support general use in e.g. energy scans.
 
 2024.1.19: Switched to new way to run Gaussian, added option to just write input file
     * Switched to using the new way to run executables, which supports containers.
```

### Comparing `gaussian_step-2024.5.31/README.rst` & `gaussian_step-2024.5.8/README.rst`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.5.31/docs/Makefile` & `gaussian_step-2024.5.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.5.31/docs/_static/SEAMM inverted.png` & `gaussian_step-2024.5.8/docs/_static/SEAMM inverted.png`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.5.31/docs/_static/SEAMM logo.png` & `gaussian_step-2024.5.8/docs/_static/SEAMM logo.png`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.5.31/docs/_static/molssi_main_logo.png` & `gaussian_step-2024.5.8/docs/_static/molssi_main_logo.png`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.5.31/docs/_static/molssi_main_logo_inverted_white.png` & `gaussian_step-2024.5.8/docs/_static/molssi_main_logo_inverted_white.png`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.5.31/docs/_static/molssi_square.png` & `gaussian_step-2024.5.8/docs/_static/molssi_square.png`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.5.31/docs/_static/nsf.png` & `gaussian_step-2024.5.8/docs/_static/nsf.png`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.5.31/docs/conf.py` & `gaussian_step-2024.5.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.5.31/docs/developer_guide/installation.rst` & `gaussian_step-2024.5.8/docs/developer_guide/installation.rst`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.5.31/docs/getting_started/index.rst` & `gaussian_step-2024.5.8/docs/getting_started/index.rst`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.5.31/docs/index.rst` & `gaussian_step-2024.5.8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.5.31/docs/make.bat` & `gaussian_step-2024.5.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.5.31/gaussian_step/__init__.py` & `gaussian_step-2024.5.8/gaussian_step/__init__.py`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.5.31/gaussian_step/data/gaussian.ini` & `gaussian_step-2024.5.8/gaussian_step/data/gaussian.ini`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.5.31/gaussian_step/data/references.bib` & `gaussian_step-2024.5.8/gaussian_step/data/references.bib`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.5.31/gaussian_step/energy.py` & `gaussian_step-2024.5.8/gaussian_step/energy.py`

 * *Files 11% similar despite different names*

```diff
@@ -244,92 +244,44 @@
             if restricted:
                 if multiplicity == 1:
                     keywords.add(f"RHF/{basis}")
                 else:
                     keywords.add(f"ROHF/{basis}")
             else:
                 keywords.add(f"UHF/{basis}")
-            # keywords.add("Guess=Mix")
         elif method[0:2] == "MP":
-            if restricted:
-                if multiplicity == 1:
-                    keywords.add(f"R{method}/{basis}")
-                else:
-                    keywords.add(f"RO{method}/{basis}")
+            if restricted and multiplicity != 1 and isinstance(self, Energy):
+                keywords.add(f"RO{method}/{basis}")
             else:
-                keywords.add(f"U{method}/{basis}")
+                keywords.add(f"{method}/{basis}")
         elif method in ("CCSD", "CCSD(T)"):
-            if restricted:
-                if multiplicity == 1:
-                    keywords.add(f"R{method}/{basis}")
-                else:
-                    keywords.add(f"RO{method}/{basis}")
+            if restricted and multiplicity != 1 and isinstance(self, Energy):
+                keywords.add(f"RO{method}/{basis}")
             else:
-                keywords.add(f"U{method}/{basis}")
+                keywords.add(f"{method}/{basis}")
         elif method in ("CBS-4M", "CBS-QB3"):
-            if self.gversion == "g09":
-                if self.__class__ == Energy:
-                    raise RuntimeError(
-                        "G09 does not appear to be able to run the CBS methods without "
-                        "optimizing the structure during the calculation."
-                    )
-                else:
-                    if restricted and multiplicity != 1:
-                        keywords.add(f"RO{method}")
-                    else:
-                        keywords.add(f"{method}")
-            else:
-                if self.__class__ == Energy:
-                    if restricted and multiplicity != 1:
-                        keywords.add(f"RO{method}=NoOpt")
-                    else:
-                        keywords.add(f"{method}=(NoOpt)")
-                else:
-                    if restricted and multiplicity != 1:
-                        keywords.add(f"RO{method}")
-                    else:
-                        keywords.add(f"{method}")
-        elif method == "CBS-APNO":
-            if self.gversion == "g09":
-                if self.__class__ == Energy:
-                    raise RuntimeError(
-                        "G09 does not appear to be able to run the CBS methods without "
-                        "optimizing the structure during the calculation."
-                    )
+            if isinstance(self, Energy):
+                if restricted and multiplicity != 1:
+                    keywords.add(f"RO{method}")
                 else:
                     keywords.add(f"{method}")
             else:
-                if self.__class__ == Energy:
-                    keywords.add(f"{method}=NoOpt")
-                else:
-                    keywords.add(f"{method}")
-        elif method in (
-            "G1",
-            "G2",
-            "G3",
-            "G4",
-            "G2MP2",
-            "G3B3",
-            "G3MP2",
-            "G3MP2B3",
-            "G4MP2",
-        ):
-            if self.gversion == "g09":
-                if self.__class__ == Energy:
-                    raise RuntimeError(
-                        "G09 does not appear to be able to run the CBS methods without "
-                        "optimizing the structure during the calculation."
-                    )
-                else:
-                    keywords.add(f"{method}")
+                raise ValueError("CBS methods are only for single-point calculations.")
+        elif method == "CBS-APNO":
+            if isinstance(self, Energy):
+                keywords.add(f"{method}")
             else:
-                if self.__class__ == Energy:
-                    keywords.add(f"{method}=(NoOpt)")
-                else:
-                    keywords.add(f"{method}")
+                raise ValueError("CBS methods are only for single-point calculations.")
+        elif method in ("G1", "G2", "G3", "G4"):
+            if isinstance(self, Energy):
+                keywords.add(f"{method}")
+            else:
+                raise ValueError(
+                    "Gaussian composite methods are only for single-point calculations."
+                )
         else:
             keywords.add(f"{method}/{basis}")
 
         if P["use symmetry"] == "loose":
             keywords.add("Symmetry=Loose")
         elif P["use symmetry"] == "identify only":
             keywords.add("NoSymmetry")
@@ -364,20 +316,20 @@
             table = {
                 "Property": [],
                 "Value": [],
                 "Units": [],
             }
 
         metadata = gaussian_step.metadata["results"]
-        if "energy" not in data:
+        if "Total Energy" not in data:
             text += "Gaussian did not produce the energy. Something is wrong!"
             printer.normal(__(text, indent=self.indent + 4 * " "))
 
         for key in (
-            "energy",
+            "Total Energy",
             "Virial Ratio",
             "RMS Density",
             "Cluster Energy with triples",
             "Cluster Energy",
             "MP5 Energy",
             "MP4 Energy",
             "MP4SDQ Energy",
```

### Comparing `gaussian_step-2024.5.31/gaussian_step/energy_parameters.py` & `gaussian_step-2024.5.8/gaussian_step/energy_parameters.py`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.5.31/gaussian_step/energy_step.py` & `gaussian_step-2024.5.8/gaussian_step/energy_step.py`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.5.31/gaussian_step/gaussian.py` & `gaussian_step-2024.5.8/gaussian_step/gaussian.py`

 * *Files 3% similar despite different names*

```diff
@@ -156,36 +156,26 @@
             title="Gaussian",
             extension=extension,
             module=__name__,
             logger=logger,
         )
 
         self.parameters = gaussian_step.GaussianParameters()
-        self._gversion = "g09"
         self._data = {}
 
     @property
     def version(self):
         """The semantic version of this module."""
         return gaussian_step.__version__
 
     @property
     def git_revision(self):
         """The git version of this module."""
         return gaussian_step.__git_revision__
 
-    @property
-    def gversion(self):
-        """The Gaussian version to target."""
-        return self._gversion
-
-    @gversion.setter
-    def gversion(self, version):
-        self._gversion = version
-
     def set_id(self, node_id):
         """Set the id for node to a given tuple"""
         self._id = node_id
 
         # and set our subnodes
         self.subflowchart.set_ids(self._id)
 
@@ -347,14 +337,17 @@
         "printer".
 
         Parameters
         ----------
         indent: str
             An extra indentation for the output
         """
+        self.parse_fchk(fchk)
+        self.parse_output(output)
+
         # Get the first real node
         node = self.subflowchart.get_node("1").next()
 
         # Loop over the subnodes, asking them to do their analysis
         while node is not None:
             for value in node.description:
                 printer.important(value)
```

### Comparing `gaussian_step-2024.5.31/gaussian_step/gaussian_parameters.py` & `gaussian_step-2024.5.8/gaussian_step/gaussian_parameters.py`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.5.31/gaussian_step/gaussian_step.py` & `gaussian_step-2024.5.8/gaussian_step/gaussian_step.py`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.5.31/gaussian_step/metadata.py` & `gaussian_step-2024.5.8/gaussian_step/metadata.py`

 * *Files 7% similar despite different names*

```diff
@@ -70,92 +70,57 @@
         "calculation": ["energy", "gradients"],
         "level": "normal",
         "gradients": "numeric",
         "freeze core?": True,
     },
     "CBS-4M: Complete Basis Set method of Petersson, et al.": {
         "method": "CBS-4M",
-        "calculation": ["energy", "gradients"],
+        "calculation": ["energy"],
         "level": "advanced",
         "gradients": "none",
         "nobasis": True,
     },
     "CBS-QB3: Complete Basis Set method of Petersson, et al.": {
         "method": "CBS-QB3",
-        "calculation": ["energy", "gradients"],
+        "calculation": ["energy"],
         "level": "normal",
         "gradients": "none",
         "nobasis": True,
     },
     "CBS-APNO: Complete Basis Set method of Petersson, et al.": {
         "method": "CBS-APNO",
-        "calculation": ["energy", "gradients"],
+        "calculation": ["energy"],
         "level": "advanced",
         "gradients": "none",
         "nobasis": True,
     },
     "G1: Gaussian-1 composite method": {
         "method": "G1",
-        "calculation": ["energy", "gradients"],
+        "calculation": ["energy"],
         "level": "advanced",
         "gradients": "none",
         "nobasis": True,
     },
     "G2: Gaussian-2 composite method": {
         "method": "G2",
-        "calculation": ["energy", "gradients"],
-        "level": "advanced",
-        "gradients": "none",
-        "nobasis": True,
-    },
-    "G2MP2: Gaussian-2 MP2 composite method": {
-        "method": "G2MP2",
-        "calculation": ["energy", "gradients"],
+        "calculation": ["energy"],
         "level": "advanced",
         "gradients": "none",
         "nobasis": True,
     },
     "G3: Gaussian-3 composite method": {
         "method": "G3",
-        "calculation": ["energy", "gradients"],
-        "level": "advanced",
-        "gradients": "none",
-        "nobasis": True,
-    },
-    "G3MP2: Gaussian-3 MP2 composite method": {
-        "method": "G3MP2",
-        "calculation": ["energy", "gradients"],
-        "level": "advanced",
-        "gradients": "none",
-        "nobasis": True,
-    },
-    "G3B3: Gaussian-3 B3LYP composite method": {
-        "method": "G3B3",
-        "calculation": ["energy", "gradients"],
-        "level": "advanced",
-        "gradients": "none",
-        "nobasis": True,
-    },
-    "G3MP2B3: Gaussian-3 MP2 B3LYP composite method": {
-        "method": "G3MP2B3",
-        "calculation": ["energy", "gradients"],
+        "calculation": ["energy"],
         "level": "advanced",
         "gradients": "none",
         "nobasis": True,
     },
     "G4: Gaussian-4 composite method": {
         "method": "G4",
-        "calculation": ["energy", "gradients"],
-        "level": "advanced",
-        "gradients": "none",
-        "nobasis": True,
-    },
-    "G4MP2: Gaussian-4 MP2 composite method": {
-        "method": "G4MP2",
-        "calculation": ["energy", "gradients"],
+        "calculation": ["energy"],
         "level": "advanced",
         "gradients": "none",
         "nobasis": True,
     },
 }
 
 dft_functionals = {
@@ -251,50 +216,31 @@
 
 type : str
     The type of the data: string, integer, or float.
 
 units : str
     Optional units for the result. If present, the value should be in these units.
 """
-composite = (
-    "CBS-4M",
-    "CBS-QB3",
-    "CBS-APNO",
-    "G1",
-    "G2",
-    "G3",
-    "G4",
-    "G2MP2",
-    "G3B3",
-    "G3MP2",
-    "G3MP2B3",
-    "G4MP2",
-)
 metadata["results"] = {
     "energy": {
+        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
         "description": "energy",
         "dimensionality": "scalar",
         "type": "float",
         "units": "E_h",
         "format": ".6f",
     },
     "gradients": {
         "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
         "description": "gradients",
         "dimensionality": [3, "natoms"],
         "type": "float",
         "units": "E_h/a0",
         "format": ".6f",
     },
-    "nsteps": {
-        "calculation": ["optimization"],
-        "description": "optimization nsteps",
-        "dimensionality": "scalar",
-        "type": "integer",
-    },
     "model": {
         "description": "The model string",
         "dimensionality": "scalar",
         "type": "string",
     },
     "Virial Ratio": {
         "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
@@ -977,186 +923,187 @@
         "dimensionality": "scalar",
         "methods": ["CCSD(T)"],
         "type": "float",
         "units": "E_h",
         "format": ".6f",
     },
     "Composite/Temperature": {
-        "calculation": ["energy", "optimization"],
+        "calculation": ["energy"],
         "description": "the temperature for the CBS/Gn extrapolation",
         "dimensionality": "scalar",
-        "methods": composite,
+        "methods": ["CBS-4M", "CBS-QB3", "CBS-APNO", "G1", "G2", "G3", "G4"],
         "type": "float",
         "units": "K",
         "format": ".2f",
     },
     "Composite/Pressure": {
-        "calculation": ["energy", "optimization"],
+        "calculation": ["energy"],
         "description": "the pressure for the CBS/Gn extrapolation",
         "dimensionality": "scalar",
-        "methods": composite,
+        "methods": ["CBS-4M", "CBS-QB3", "CBS-APNO", "G1", "G2", "G3", "G4"],
         "type": "float",
         "units": "atm",
         "format": ".2f",
     },
     "Composite/E(ZPE)": {
-        "calculation": ["energy", "optimization"],
+        "calculation": ["energy"],
         "description": "the ZPE from the CBS/Gn extrapolation",
         "dimensionality": "scalar",
-        "methods": composite,
+        "methods": ["CBS-4M", "CBS-QB3", "CBS-APNO", "G1", "G2", "G3", "G4"],
         "type": "float",
         "units": "E_h",
         "format": ".6f",
     },
     "Composite/E(Thermal)": {
-        "calculation": ["energy", "optimization"],
+        "calculation": ["energy"],
         "description": "the thermal energy from the CBS/Gn extrapolation",
         "dimensionality": "scalar",
-        "methods": composite,
+        "methods": ["CBS-4M", "CBS-QB3", "CBS-APNO", "G1", "G2", "G3", "G4"],
         "type": "float",
         "units": "E_h",
         "format": ".6f",
     },
     "Composite/E(SCF)": {
-        "calculation": ["energy", "optimization"],
+        "calculation": ["energy"],
         "description": "the SCF energy from the CBS/Gn extrapolation",
         "dimensionality": "scalar",
-        "methods": composite,
+        "methods": ["CBS-4M", "CBS-QB3", "CBS-APNO"],
         "type": "float",
         "units": "E_h",
         "format": ".6f",
     },
     "Composite/DE(MP2)": {
-        "calculation": ["energy", "optimization"],
+        "calculation": ["energy"],
         "description": "dE from MP2 from the CBS/Gn extrapolation",
         "dimensionality": "scalar",
-        "methods": composite,
+        "methods": ["CBS-4M", "CBS-QB3", "CBS-APNO"],
         "type": "float",
         "units": "E_h",
         "format": ".6f",
     },
     "Composite/DE(CBS)": {
-        "calculation": ["energy", "optimization"],
+        "calculation": ["energy"],
         "description": "dE from the basis extrapolation from the CBS/Gn extrapolation",
         "dimensionality": "scalar",
-        "methods": composite,
+        "methods": ["CBS-4M", "CBS-QB3", "CBS-APNO"],
         "type": "float",
         "units": "E_h",
         "format": ".6f",
     },
     "Composite/DE(MP34)": {
-        "calculation": ["energy", "optimization"],
+        "calculation": ["energy"],
         "description": "dE of MP3-4 from the CBS/Gn extrapolation",
         "dimensionality": "scalar",
-        "methods": composite,
+        "methods": ["CBS-4M", "CBS-QB3", "CBS-APNO"],
         "type": "float",
         "units": "E_h",
         "format": ".6f",
     },
     "Composite/DE(CCSD)": {
-        "calculation": ["energy", "optimization"],
+        "calculation": ["energy"],
         "description": "dE of CCSD from the CBS/Gn extrapolation",
         "dimensionality": "scalar",
         "methods": ["CBS-4M", "CBS-QB3", "CBS-APNO"],
         "type": "float",
         "units": "E_h",
         "format": ".6f",
     },
     "Composite/DE(int)": {
-        "calculation": ["energy", "optimization"],
+        "calculation": ["energy"],
         "description": "dE from internals from the CBS/Gn extrapolation",
         "dimensionality": "scalar",
-        "methods": composite,
+        "methods": ["CBS-4M", "CBS-QB3", "CBS-APNO"],
         "type": "float",
         "units": "E_h",
         "format": ".6f",
     },
     "Composite/DE(empirical)": {
-        "calculation": ["energy", "optimization"],
+        "calculation": ["energy"],
         "description": "Empirical correction to the CBS/Gn extrapolation",
         "dimensionality": "scalar",
-        "methods": composite,
+        "methods": ["CBS-4M", "CBS-QB3", "CBS-APNO", "G1", "G2", "G3", "G4"],
         "type": "float",
         "units": "E_h",
         "format": ".6f",
     },
     "Composite/E(CCSD(T))": {
-        "calculation": ["energy", "optimization"],
+        "calculation": ["energy"],
         "description": "CCSD(T) term for the Gn extrapolation",
         "dimensionality": "scalar",
         "methods": ["G1", "G2", "G3", "G4"],
         "type": "float",
         "units": "E_h",
         "format": ".6f",
     },
     "Composite/DE(Plus)": {
-        "calculation": ["energy", "optimization"],
+        "calculation": ["energy"],
         "description": "Plus term for the Gn extrapolation",
         "dimensionality": "scalar",
         "methods": ["G1", "G2", "G3", "G4"],
         "type": "float",
         "units": "E_h",
         "format": ".6f",
     },
     "Composite/DE(2DF)": {
-        "calculation": ["energy", "optimization"],
+        "calculation": ["energy"],
         "description": "The delta energy for 2D's and F term for the Gn extrapolation",
         "dimensionality": "scalar",
         "methods": ["G1", "G2", "G3", "G4"],
         "type": "float",
         "units": "E_h",
         "format": ".6f",
     },
     "Composite/E(Delta-G3XP)": {
-        "calculation": ["energy", "optimization"],
+        "calculation": ["energy"],
         "description": "Delta G3XP term for the Gn extrapolation",
         "dimensionality": "scalar",
         "methods": ["G1", "G2", "G3", "G4"],
         "type": "float",
         "units": "E_h",
         "format": ".6f",
     },
     "Composite/DE(HF)": {
-        "calculation": ["energy", "optimization"],
+        "calculation": ["energy"],
         "description": "delta E(HF) term for the Gn extrapolation",
         "dimensionality": "scalar",
         "methods": ["G1", "G2", "G3", "G4"],
         "type": "float",
         "units": "E_h",
         "format": ".6f",
     },
-    "Composite/E(0 K)": {
+    "Composite/(0 K)": {
+        "calculation": ["energy"],
         "description": "the 0 K energy from the CBS/Gn extrapolation",
         "dimensionality": "scalar",
-        "methods": composite,
+        "methods": ["CBS-4M", "CBS-QB3", "CBS-APNO", "G1", "G2", "G3", "G4"],
         "type": "float",
         "units": "E_h",
         "format": ".6f",
     },
     "Composite/Energy": {
-        "calculation": ["energy", "optimization"],
+        "calculation": ["energy"],
         "description": "the energy from the CBS/Gn extrapolation",
         "dimensionality": "scalar",
-        "methods": composite,
+        "methods": ["CBS-4M", "CBS-QB3", "CBS-APNO", "G1", "G2", "G3", "G4"],
         "type": "float",
         "units": "E_h",
         "format": ".6f",
     },
     "Composite/Enthalpy": {
-        "calculation": ["energy", "optimization"],
+        "calculation": ["energy"],
         "description": "the enthalpy from the CBS/Gn extrapolation",
         "dimensionality": "scalar",
-        "methods": composite,
+        "methods": ["CBS-4M", "CBS-QB3", "CBS-APNO", "G1", "G2", "G3", "G4"],
         "type": "float",
         "units": "E_h",
         "format": ".6f",
     },
     "Composite/Free Energy": {
-        "calculation": ["energy", "optimization"],
+        "calculation": ["energy"],
         "description": "the free energy from the CBS/Gn extrapolation",
         "dimensionality": "scalar",
-        "methods": composite,
+        "methods": ["CBS-4M", "CBS-QB3", "CBS-APNO", "G1", "G2", "G3", "G4"],
         "type": "float",
         "units": "E_h",
         "format": ".6f",
     },
 }
```

### Comparing `gaussian_step-2024.5.31/gaussian_step/optimization.py` & `gaussian_step-2024.5.8/gaussian_step/optimization.py`

 * *Files 16% similar despite different names*

```diff
@@ -51,52 +51,28 @@
 
         if not P:
             P = self.parameters.values_to_dict()
 
         text = super().description_text(P=P, calculation=calculation)
 
         coordinates = P["coordinates"]
-        added = "\nThe geometry optimization is targeting "
-
-        target = P["target"].lower()
-        if self.is_expr(target):
-            added += "a minimum or saddle point, depending on {target},"
-        elif "min" in target:
-            added += "the minimum"
-        elif "trans" in target or target == "ts":
-            added += "a transition state"
-        elif "saddle" in target:
-            added += "a saddle point with {saddle order} downhill directions"
-        added += f" using {coordinates} coordinates,"
+        added = f"\nThe geometry optimization will use {coordinates} coordinates,"
         added += " a {geometry convergence} convergence criterion, "
         if P["max geometry steps"] == "default":
             added += (
                 "and the default maximum number of steps, which is based on the "
                 "system size."
             )
         else:
             added += "and no more than {max geometry steps} steps."
 
-        if P["recalc hessian"] == "never":
-            pass
-        elif self.is_expr(P["recalc hessian"]):
-            added += " Whether and how to calculate the Hessian will be determined by "
-            added += "{recalc hessian}."
-        elif "every" in P["recalc hessian"]:
-            added += " The Hessian will be recalculated every step."
-        elif P["recalc hessian"] == "at beginning":
-            added += " The Hessian will be calculated once at the beginning."
-        elif P["recalc hessian"] == "HF at beginning":
-            added += (
-                " The Hartree-Fock Hessian will be calculated once at the beginning."
-            )
-        else:
-            added += " The Hessian will be recalculated every {recalc hessian} steps."
         if P["recalc hessian"] != "never":
-            added += " Note that calculating the second derivatives is quite expensive!"
+            added += " The Hessian will be recalculated every {recalc hessian}"
+            added += " steps. Note that calculating the second derivatives is "
+            added += "quite expensive!"
 
         if (
             isinstance(P["input only"], bool)
             and P["input only"]
             or P["input only"] == "yes"
         ):
             if type(self) is Optimization:
@@ -126,29 +102,15 @@
             if "nAtoms" in max_steps:
                 n_atoms = configuration.n_atoms
                 max_steps = max_steps.replace("nAtoms", str(n_atoms))
                 max_steps = eval(max_steps)
             else:
                 max_steps = int(max_steps)
             subkeywords.append(f"MaxCycles={max_steps}")
-            # Also need to use an IOP to set the max. Odd.
-            # https://mattermodeling.stackexchange.com/questions/5087/ (continued)
-            #       why-does-gaussian-ignore-the-opt-maxcycles-keyword-for-optimizations
-            keywords.add(f"iop(1/152={max_steps})")
-
-        # Handle the target for the optimization
-        target = P["target"].lower()
-        if "min" in target:
-            pass
-        elif "trans" in target or target == "ts":
-            subkeywords.append("TS")
-        elif "saddle" in target:
-            subkeywords.append(f"Saddle={P['saddle order']}")
 
-        # Handle options for the calculation of the Hessian
         if P["recalc hessian"] == "every step":
             subkeywords.append("CalcAll")
         elif P["recalc hessian"] == "at beginning":
             subkeywords.append("CalcFC")
         elif P["recalc hessian"] == "HF at beginning":
             subkeywords.append("CalcHFFC")
         elif P["recalc hessian"] == "never":
@@ -187,26 +149,25 @@
             table = {
                 "Property": [],
                 "Value": [],
                 "Units": [],
             }
 
         # metadata = gaussian_step.metadata["results"]
-        if "energy" not in data:
+        if "Total Energy" not in data:
             text += "Gaussian did not produce the energy. Something is wrong!"
 
         # Get the system & configuration
         _, configuration = self.get_system_configuration(None)
 
         if configuration.n_atoms == 1:
             text += "System is an atom, so nothing to optimize."
         else:
             # Information about the optimization
             n_steps = data["Optimization Number of geometries"][0]
-            data["nsteps"] = n_steps
             if data["Geometry Optimization Converged"]:
                 text += f"The geometry optimization converged in {n_steps} steps."
             else:
                 text += (
                     f"Warning: The geometry optimization did not converge in {n_steps} "
                     "steps."
                 )
```

### Comparing `gaussian_step-2024.5.31/gaussian_step/optimization_parameters.py` & `gaussian_step-2024.5.8/gaussian_step/optimization_parameters.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,34 +11,14 @@
 logger = logging.getLogger("Gaussian")
 
 
 class OptimizationParameters(gaussian_step.EnergyParameters):
     """The control parameters for the energy."""
 
     parameters = {
-        "target": {
-            "default": "minimum",
-            "kind": "string",
-            "default_units": "",
-            "enumeration": ("minimum", "transition state", "saddle point"),
-            "format_string": "",
-            "description": "Optimization target:",
-            "help_text": (
-                "The type of structure that is the target for the optimization."
-            ),
-        },
-        "saddle order": {
-            "default": 2,
-            "kind": "integer",
-            "default_units": "",
-            "enumeration": tuple(),
-            "format_string": "",
-            "description": "Order of saddle point:",
-            "help_text": "Number of directions down from the saddle point.",
-        },
         "max geometry steps": {
             "default": "default",
             "kind": "string",
             "default_units": "",
             "enumeration": ("default", "6*nAtoms", "9*nAtoms"),
             "format_string": "",
             "description": "Maximum steps:",
```

### Comparing `gaussian_step-2024.5.31/gaussian_step/optimization_step.py` & `gaussian_step-2024.5.8/gaussian_step/optimization_step.py`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.5.31/gaussian_step/substep.py` & `gaussian_step-2024.5.8/gaussian_step/substep.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,18 +112,14 @@
         return gaussian_step.__git_revision__
 
     @property
     def global_options(self):
         return self.parent.global_options
 
     @property
-    def gversion(self):
-        return self.parent.gversion
-
-    @property
     def input_only(self):
         """Whether to write the input only, not run MOPAC."""
         return self._input_only
 
     @input_only.setter
     def input_only(self, value):
         self._input_only = value
@@ -481,26 +477,21 @@
                                 _, month, year = date.split("-")
                                 revision = revision.split("Rev")[1]
                                 data["G revision"] = revision
                                 data["G version"] = f"G{version.strip(':')}"
                                 data["G month"] = month
                                 data["G year"] = year
                             except Exception as e:
-                                self.logger.warning(
+                                logger.warning(
                                     f"Could not find the Gaussian citation: {e}"
                                 )
                             break
                 break
 
         # And the optimization steps, if any.
-        #
-        # Need to be careful about end of the first (and presumably only?) optimization.
-        # The FORCE calculation prints out the same information about convergence, but
-        # may indicate no convergence. This can confuse this code unless we look for the
-        # end of the optimization step and quit then
         it = iter(lines)
         n_steps = 0
         max_force = []
         rms_force = []
         max_displacement = []
         rms_displacement = []
         converged = None
@@ -532,24 +523,14 @@
 
                 tmp1, tmp2, value, threshold, criterion = next(it).split()
                 if tmp1 == "RMS" and tmp2 == "Displacement":
                     rms_displacement.append(float(value))
                     data["RMS Displacement Threshold"] = float(threshold)
                     if criterion != "YES":
                         converged = False
-            elif line == " Optimization completed.":
-                line = next(it)
-                if line == "    -- Stationary point found.":
-                    converged = True
-                else:
-                    self.logger.warning(f"Optimization completed: {line}")
-                break
-            elif line == "    -- Stationary point found.":
-                converged = True
-                break
 
         if converged is not None:
             data["Geometry Optimization Converged"] = converged
             data["Maximum Force"] = max_force[-1]
             data["RMS Force"] = rms_force[-1]
             data["Maximum Displacement"] = max_displacement[-1]
             data["RMS Displacement"] = rms_displacement[-1]
@@ -613,22 +594,16 @@
                         part = [line]
                     for p in part:
                         if "=" not in p:
                             continue
                         key, value = p.split("=", 1)
                         key = key.strip()
                         value = float(value.strip())
-                        if "(0 K)" in key:
-                            key = "E(0 K)"
-                        elif "Free Energy" in key:
-                            key = "Free Energy"
-                        elif "Energy" in key:
-                            key = "Energy"
-                        elif "Enthalpy" in key:
-                            key = "Enthalpy"
+                        if method in key:
+                            key = key.split(" ", 1)[1]
                         data[f"Composite/{key}"] = value
                 data["Composite/model"] = method
                 data["Composite/summary"] = "\n".join(text)
                 data["Total Energy"] = data["Composite/Free Energy"]
 
         # Gn calculations. No header!!!!!
 
@@ -636,25 +611,15 @@
         # E(ZPE)=                     0.050251 E(Thermal)=                    0.053306
         # E(CCSD(T))=               -78.321715 E(Empiric)=                   -0.041682
         # DE(Plus)=                  -0.005930 DE(2DF)=                      -0.076980
         # E(Delta-G3XP)=             -0.117567 DE(HF)=                       -0.008255
         # G4(0 K)=                  -78.521880 G4 Energy=                   -78.518825
         # G4 Enthalpy=              -78.517880 G4 Free Energy=              -78.542752
 
-        if P["method"] in (
-            "G1",
-            "G2",
-            "G3",
-            "G4",
-            "G2MP2",
-            "G3B3",
-            "G3MP2",
-            "G3MP2B3",
-            "G4MP2",
-        ):
+        if P["method"][0:2] in ("G1", "G2", "G3", "G4"):
             # Need last section
             method = P["method"][0:2]
             match = f"{method} Enthalpy="
             text = []
             found = False
             for line in reversed(lines):
                 if found:
@@ -690,15 +655,15 @@
                 data["Composite/summary"] = tmp + "\n".join(text)
                 data["Total Energy"] = data["Composite/Free Energy"]
 
         return data
 
     def process_data(self, data):
         """Massage the cclib data to a more easily used form."""
-        self.logger.debug(pprint.pformat(data))
+        logger.debug(pprint.pformat(data))
         # Convert numpy arrays to Python lists
         new = {}
         for key, value in data.items():
             if isinstance(value, np.ndarray):
                 new[key] = value.tolist()
             elif isinstance(value, list):
                 if len(value) > 0 and isinstance(value[0], np.ndarray):
@@ -888,15 +853,15 @@
             XYZs = configuration.atoms.coordinates
             for symbol, xyz in zip(symbols, XYZs):
                 x, y, z = xyz
                 lines.append(f"{symbol:2}   {x:10.6f} {y:10.6f} {z:10.6f}")
             lines.append(" ")
 
             files = {"input.dat": "\n".join(lines)}
-            self.logger.info("input.dat:\n" + files["input.dat"])
+            logger.info("input.dat:\n" + files["input.dat"])
 
             printer.important(
                 self.indent + f"    Gaussian will use {n_threads} OpenMP threads and "
                 f"up to {memory} of memory.\n"
             )
             if self.input_only:
                 # Just write the input files and stop
@@ -1022,48 +987,48 @@
             # And parse a bit more out of the output
             if path.exists():
                 data = self.parse_output(path, data)
 
             # Debug output
             if self.logger.isEnabledFor(logging.INFO):
                 keys = "\n".join(data.keys())
-                self.logger.info(f"Data keys:\n{keys}")
+                logger.info(f"Data keys:\n{keys}")
             if self.logger.isEnabledFor(logging.DEBUG):
                 keys = "\n".join(data.keys())
-                self.logger.info(f"Data keys:\n{keys}")
-                self.logger.debug(f"Data:\n{pprint.pformat(data)}")
+                logger.info(f"Data keys:\n{keys}")
+                logger.debug(f"Data:\n{pprint.pformat(data)}")
 
             # Explicitly pull out the energy and gradients to standard name
             if "Total Energy" in data:
                 data["energy"] = data["Total Energy"]
                 del data["Total Energy"]
             if "Cartesian Gradient" in data:
                 tmp = np.array(data["Cartesian Gradient"])
                 data["gradients"] = tmp.reshape(-1, 3).tolist()
                 del data["Cartesian Gradient"]
 
             # Debug output
             if self.logger.isEnabledFor(logging.INFO):
                 keys = "\n".join(data.keys())
-                self.logger.info(f"Data keys:\n{keys}")
+                logger.info(f"Data keys:\n{keys}")
             if self.logger.isEnabledFor(logging.DEBUG):
                 keys = "\n".join(data.keys())
-                self.logger.info(f"Data keys:\n{keys}")
-                self.logger.debug(f"Data:\n{pprint.pformat(data)}")
+                logger.info(f"Data keys:\n{keys}")
+                logger.debug(f"Data:\n{pprint.pformat(data)}")
 
             # The model chemistry
             # self.model = f"{data['metadata/functional']}/{data['metadata/basis_set']}"
             if "Composite/model" in data:
                 self.model = data["Composite/model"]
             else:
                 self.model = (
                     f"{data['metadata/methods'][-1]}/{data['method']}/"
                     f"{data['metadata/basis_set']}"
                 )
-            self.logger.info(f"model = {self.model}")
+            logger.info(f"model = {self.model}")
 
             data["model"] = "Gaussian/" + self.model
 
             # If ran successfully, put out the success file
             if data["success"]:
                 success.write_text("success")
```

### Comparing `gaussian_step-2024.5.31/gaussian_step/tk_energy.py` & `gaussian_step-2024.5.8/gaussian_step/tk_energy.py`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.5.31/gaussian_step/tk_gaussian.py` & `gaussian_step-2024.5.8/gaussian_step/tk_gaussian.py`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.5.31/gaussian_step/tk_optimization.py` & `gaussian_step-2024.5.8/gaussian_step/tk_optimization.py`

 * *Files 18% similar despite different names*

```diff
@@ -90,20 +90,14 @@
             labelanchor="n",
             padding=10,
         )
 
         for key in gaussian_step.OptimizationParameters.parameters:
             self[key] = P[key].widget(opt_frame)
 
-        # bindings...
-        for key in ("target",):
-            self[key].bind("<<ComboboxSelected>>", self.reset_optimization)
-            self[key].bind("<Return>", self.reset_optimization)
-            self[key].bind("<FocusOut>", self.reset_optimization)
-
         # Top level needs to call reset_dialog
         if self.node.calculation == "optimization":
             self.reset_dialog()
 
     def reset_dialog(self, widget=None):
         """Layout the widgets, letting our parents go first."""
         frame = self["frame"]
@@ -129,35 +123,34 @@
         return row
 
     def reset_optimization(self, widget=None):
         frame = self["optimization"]
         for slave in frame.grid_slaves():
             slave.grid_forget()
 
-        target = self["target"].get()
-
         widgets = []
-        widgets2 = []
+        # widgets2 = []
         row = 0
 
-        self["target"].grid(row=row, column=0, columnspan=2, sticky=tk.EW)
-        widgets.append(self["target"])
+        self["geometry convergence"].grid(row=row, column=0, columnspan=2, sticky=tk.EW)
+        widgets.append(self["geometry convergence"])
+        row += 1
+
+        self["coordinates"].grid(row=row, column=0, columnspan=2, sticky=tk.EW)
+        widgets.append(self["coordinates"])
+        row += 1
+
+        self["max geometry steps"].grid(row=row, column=0, columnspan=2, sticky=tk.EW)
+        widgets.append(self["max geometry steps"])
+        row += 1
+
+        self["recalc hessian"].grid(row=row, column=0, columnspan=2, sticky=tk.EW)
+        widgets.append(self["recalc hessian"])
         row += 1
 
-        if target not in ("minimum", "transition state"):
-            self["saddle order"].grid(row=row, column=1, sticky=tk.EW)
-            widgets2.append(self["saddle order"])
-            row += 1
-
-        for key in (
-            "geometry convergence",
-            "coordinates",
-            "max geometry steps",
-            "recalc hessian",
-            "ignore unconverged optimization",
-        ):
-            self[key].grid(row=row, column=0, columnspan=2, sticky=tk.EW)
-            widgets.append(self[key])
-            row += 1
+        self["ignore unconverged optimization"].grid(
+            row=row, column=0, columnspan=2, sticky=tk.EW
+        )
+        widgets.append(self["ignore unconverged optimization"])
+        row += 1
 
         sw.align_labels(widgets, sticky=tk.E)
-        sw.align_labels(widgets2, sticky=tk.E)
```

### Comparing `gaussian_step-2024.5.31/gaussian_step.egg-info/PKG-INFO` & `gaussian_step-2024.5.8/gaussian_step.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaussian_step
-Version: 2024.5.31
+Version: 2024.5.8
 Summary: A SEAMM plugin for A SEAMM plug-in for Gaussian
 Home-page: https://github.com/molssi-seamm/gaussian_step
 Author: Paul Saxe
 Author-email: psaxe@vt.edu
 License: BSD-3-Clause
 Keywords: SEAMM,SEAMMplugin,flowchart
 Platform: Linux
@@ -86,25 +86,14 @@
 .. _MolSSI: https://molssi.org
 .. _`National Science Foundation`: https://www.nsf.gov
 
 
 =======
 History
 =======
-2024.5.31: Added optimization of transition states, and...
-    * Corrected implementation of composite methods (Gn, CBS-x) to handle optimization.
-    * Added target of the optimization to allow transition states and saddle points.
-    * Corrected a bug in handling the maximum number of optimization steps.
-    * Corrected bug determining if optimization completed properly.
-    * Corrected bug handling the composite method results.
-      
-2024.5.27: Added number of optimization steps to results
-    * Added the number of steps for the optimizations to the results that can be output
-      to tables, variables, etc.
-      
 2024.5.8 General enhancements
     * Updated to new calculation handling, with ~/SEAMM/gaussian.ini controlling access
       to the installed version of Gaussian on the machine.
     * Added energy and gradients to results to support general use in e.g. energy scans.
 
 2024.1.19: Switched to new way to run Gaussian, added option to just write input file
     * Switched to using the new way to run executables, which supports containers.
```

### Comparing `gaussian_step-2024.5.31/gaussian_step.egg-info/SOURCES.txt` & `gaussian_step-2024.5.8/gaussian_step.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.5.31/setup.py` & `gaussian_step-2024.5.8/setup.py`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.5.31/versioneer.py` & `gaussian_step-2024.5.8/versioneer.py`

 * *Files identical despite different names*

