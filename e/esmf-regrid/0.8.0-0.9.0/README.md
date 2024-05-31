# Comparing `tmp/esmf_regrid-0.8.0.tar.gz` & `tmp/esmf_regrid-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esmf_regrid-0.8.0.tar", last modified: Tue Aug 22 13:15:04 2023, max compression
+gzip compressed data, was "esmf_regrid-0.9.0.tar", last modified: Fri Nov  3 11:44:03 2023, max compression
```

## Comparing `esmf_regrid-0.8.0.tar` & `esmf_regrid-0.9.0.tar`

### file list

```diff
@@ -1,89 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-22 13:15:04.833371 esmf_regrid-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     7972 2023-08-22 13:14:55.000000 esmf_regrid-0.8.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-08-22 13:14:55.000000 esmf_regrid-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-08-22 13:14:55.000000 esmf_regrid-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-08-22 13:15:04.833371 esmf_regrid-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-08-22 13:14:55.000000 esmf_regrid-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-22 13:15:04.825370 esmf_regrid-0.8.0/esmf_regrid/
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-08-22 13:14:55.000000 esmf_regrid-0.8.0/esmf_regrid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19216 2023-08-22 13:14:55.000000 esmf_regrid-0.8.0/esmf_regrid/_esmf_sdo.py
--rw-r--r--   0 runner    (1001) docker     (123)     8894 2023-08-22 13:14:55.000000 esmf_regrid-0.8.0/esmf_regrid/esmf_regridder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-22 13:15:04.825370 esmf_regrid-0.8.0/esmf_regrid/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-22 13:14:55.000000 esmf_regrid-0.8.0/esmf_regrid/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8886 2023-08-22 13:14:55.000000 esmf_regrid-0.8.0/esmf_regrid/experimental/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-08-22 13:14:55.000000 esmf_regrid-0.8.0/esmf_regrid/experimental/unstructured_regrid.py
--rw-r--r--   0 runner    (1001) docker     (123)    16644 2023-08-22 13:14:55.000000 esmf_regrid-0.8.0/esmf_regrid/experimental/unstructured_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)    58402 2023-08-22 13:14:55.000000 esmf_regrid-0.8.0/esmf_regrid/schemes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-22 13:15:04.825370 esmf_regrid-0.8.0/esmf_regrid/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-08-22 13:14:55.000000 esmf_regrid-0.8.0/esmf_regrid/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-22 13:15:04.825370 esmf_regrid-0.8.0/esmf_regrid/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-22 13:14:55.000000 esmf_regrid-0.8.0/esmf_regrid/tests/integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-22 13:15:04.829371 esmf_regrid-0.8.0/esmf_regrid/tests/integration/esmf_regridder/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-08-22 13:14:55.000000 esmf_regrid-0.8.0/esmf_regrid/tests/integration/esmf_regridder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-08-22 13:14:55.000000 esmf_regrid-0.8.0/esmf_regrid/tests/integration/esmf_regridder/test_Regridder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-22 13:15:04.829371 esmf_regrid-0.8.0/esmf_regrid/tests/integration/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-22 13:14:55.000000 esmf_regrid-0.8.0/esmf_regrid/tests/integration/experimental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-22 13:15:04.829371 esmf_regrid-0.8.0/esmf_regrid/tests/integration/experimental/unstructured_scheme/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-08-22 13:14:55.000000 esmf_regrid-0.8.0/esmf_regrid/tests/integration/experimental/unstructured_scheme/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-08-22 13:14:55.000000 esmf_regrid-0.8.0/esmf_regrid/tests/integration/experimental/unstructured_scheme/test_regrid_unstructured_to_rectilinear.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-22 13:15:04.821370 esmf_regrid-0.8.0/esmf_regrid/tests/results/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-22 13:15:04.821370 esmf_regrid-0.8.0/esmf_regrid/tests/results/unit/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-22 13:15:04.821370 esmf_regrid-0.8.0/esmf_regrid/tests/results/unit/_esmf_sdo/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-22 13:15:04.829371 esmf_regrid-0.8.0/esmf_regrid/tests/results/unit/_esmf_sdo/test_GridInfo/
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-08-22 13:14:55.000000 esmf_regrid-0.8.0/esmf_regrid/tests/results/unit/_esmf_sdo/test_GridInfo/small_grid.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-22 13:15:04.825370 esmf_regrid-0.8.0/esmf_regrid/tests/results/unit/experimental/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-22 13:15:04.825370 esmf_regrid-0.8.0/esmf_regrid/tests/results/unit/experimental/unstructured_regrid/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-22 13:15:04.829371 esmf_regrid-0.8.0/esmf_regrid/tests/results/unit/experimental/unstructured_regrid/test_MeshInfo/
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-08-22 13:14:55.000000 esmf_regrid-0.8.0/esmf_regrid/tests/results/unit/experimental/unstructured_regrid/test_MeshInfo/small_mesh.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-22 13:15:04.829371 esmf_regrid-0.8.0/esmf_regrid/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-22 13:14:55.000000 esmf_regrid-0.8.0/esmf_regrid/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-22 13:15:04.829371 esmf_regrid-0.8.0/esmf_regrid/tests/unit/_esmf_sdo/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-22 13:14:55.000000 esmf_regrid-0.8.0/esmf_regrid/tests/unit/_esmf_sdo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-08-22 13:14:55.000000 esmf_regrid-0.8.0/esmf_regrid/tests/unit/_esmf_sdo/test_GridInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-08-22 13:14:55.000000 esmf_regrid-0.8.0/esmf_regrid/tests/unit/_esmf_sdo/test_RefinedGridInfo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-22 13:15:04.829371 esmf_regrid-0.8.0/esmf_regrid/tests/unit/esmf_regridder/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-22 13:14:55.000000 esmf_regrid-0.8.0/esmf_regrid/tests/unit/esmf_regridder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8023 2023-08-22 13:14:55.000000 esmf_regrid-0.8.0/esmf_regrid/tests/unit/esmf_regridder/test_Regridder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-22 13:15:04.829371 esmf_regrid-0.8.0/esmf_regrid/tests/unit/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-22 13:14:55.000000 esmf_regrid-0.8.0/esmf_regrid/tests/unit/experimental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-22 13:15:04.829371 esmf_regrid-0.8.0/esmf_regrid/tests/unit/experimental/io/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-08-22 13:14:55.000000 esmf_regrid-0.8.0/esmf_regrid/tests/unit/experimental/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11658 2023-08-22 13:14:55.000000 esmf_regrid-0.8.0/esmf_regrid/tests/unit/experimental/io/test_round_tripping.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-08-22 13:14:55.000000 esmf_regrid-0.8.0/esmf_regrid/tests/unit/experimental/io/test_save_regridder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-22 13:15:04.829371 esmf_regrid-0.8.0/esmf_regrid/tests/unit/experimental/unstructured_regrid/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-08-22 13:14:55.000000 esmf_regrid-0.8.0/esmf_regrid/tests/unit/experimental/unstructured_regrid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6521 2023-08-22 13:14:55.000000 esmf_regrid-0.8.0/esmf_regrid/tests/unit/experimental/unstructured_regrid/test_MeshInfo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-22 13:15:04.829371 esmf_regrid-0.8.0/esmf_regrid/tests/unit/experimental/unstructured_scheme/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-08-22 13:14:55.000000 esmf_regrid-0.8.0/esmf_regrid/tests/unit/experimental/unstructured_scheme/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17732 2023-08-22 13:14:55.000000 esmf_regrid-0.8.0/esmf_regrid/tests/unit/experimental/unstructured_scheme/test_GridToMeshESMFRegridder.py
--rw-r--r--   0 runner    (1001) docker     (123)    16171 2023-08-22 13:14:55.000000 esmf_regrid-0.8.0/esmf_regrid/tests/unit/experimental/unstructured_scheme/test_MeshToGridESMFRegridder.py
--rw-r--r--   0 runner    (1001) docker     (123)    10026 2023-08-22 13:14:55.000000 esmf_regrid-0.8.0/esmf_regrid/tests/unit/experimental/unstructured_scheme/test_regrid_rectilinear_to_unstructured.py
--rw-r--r--   0 runner    (1001) docker     (123)     7777 2023-08-22 13:14:55.000000 esmf_regrid-0.8.0/esmf_regrid/tests/unit/experimental/unstructured_scheme/test_regrid_unstructured_to_rectilinear.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-22 13:15:04.833371 esmf_regrid-0.8.0/esmf_regrid/tests/unit/schemes/
--rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-08-22 13:14:55.000000 esmf_regrid-0.8.0/esmf_regrid/tests/unit/schemes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-08-22 13:14:55.000000 esmf_regrid-0.8.0/esmf_regrid/tests/unit/schemes/test_ESMFAreaWeighted.py
--rw-r--r--   0 runner    (1001) docker     (123)    10844 2023-08-22 13:14:55.000000 esmf_regrid-0.8.0/esmf_regrid/tests/unit/schemes/test_ESMFAreaWeightedRegridder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-08-22 13:14:55.000000 esmf_regrid-0.8.0/esmf_regrid/tests/unit/schemes/test_ESMFBilinear.py
--rw-r--r--   0 runner    (1001) docker     (123)    11626 2023-08-22 13:14:55.000000 esmf_regrid-0.8.0/esmf_regrid/tests/unit/schemes/test_ESMFBilinearRegridder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-08-22 13:14:55.000000 esmf_regrid-0.8.0/esmf_regrid/tests/unit/schemes/test_ESMFNearest.py
--rw-r--r--   0 runner    (1001) docker     (123)    12112 2023-08-22 13:14:55.000000 esmf_regrid-0.8.0/esmf_regrid/tests/unit/schemes/test_ESMFNearestRegridder.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-08-22 13:14:55.000000 esmf_regrid-0.8.0/esmf_regrid/tests/unit/schemes/test__ESMFRegridder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-08-22 13:14:55.000000 esmf_regrid-0.8.0/esmf_regrid/tests/unit/schemes/test__create_cube.py
--rw-r--r--   0 runner    (1001) docker     (123)     8573 2023-08-22 13:14:55.000000 esmf_regrid-0.8.0/esmf_regrid/tests/unit/schemes/test__cube_to_GridInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)    10012 2023-08-22 13:14:55.000000 esmf_regrid-0.8.0/esmf_regrid/tests/unit/schemes/test__mesh_to_MeshInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-08-22 13:14:55.000000 esmf_regrid-0.8.0/esmf_regrid/tests/unit/schemes/test__regrid_unstructured_to_rectilinear__prepare.py
--rw-r--r--   0 runner    (1001) docker     (123)    15808 2023-08-22 13:14:55.000000 esmf_regrid-0.8.0/esmf_regrid/tests/unit/schemes/test_regrid_rectilinear_to_rectilinear.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-22 13:15:04.825370 esmf_regrid-0.8.0/esmf_regrid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-08-22 13:15:04.000000 esmf_regrid-0.8.0/esmf_regrid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-08-22 13:15:04.000000 esmf_regrid-0.8.0/esmf_regrid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-22 13:15:04.000000 esmf_regrid-0.8.0/esmf_regrid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-22 13:15:04.000000 esmf_regrid-0.8.0/esmf_regrid.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-08-22 13:15:04.000000 esmf_regrid-0.8.0/esmf_regrid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-22 13:15:04.000000 esmf_regrid-0.8.0/esmf_regrid.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-08-22 13:14:55.000000 esmf_regrid-0.8.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-22 13:15:04.833371 esmf_regrid-0.8.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-22 13:14:55.000000 esmf_regrid-0.8.0/requirements/core.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-22 13:14:55.000000 esmf_regrid-0.8.0/requirements/optional-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-22 13:14:55.000000 esmf_regrid-0.8.0/requirements/optional-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-22 13:15:04.833371 esmf_regrid-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-08-22 13:14:55.000000 esmf_regrid-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 11:44:03.358350 esmf_regrid-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     8654 2023-11-03 11:43:52.000000 esmf_regrid-0.9.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2023-11-03 11:43:52.000000 esmf_regrid-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2023-11-03 11:43:52.000000 esmf_regrid-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2023-11-03 11:44:03.358350 esmf_regrid-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2023-11-03 11:43:52.000000 esmf_regrid-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 11:44:03.350350 esmf_regrid-0.9.0/esmf_regrid/
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2023-11-03 11:43:52.000000 esmf_regrid-0.9.0/esmf_regrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19216 2023-11-03 11:43:52.000000 esmf_regrid-0.9.0/esmf_regrid/_esmf_sdo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8894 2023-11-03 11:43:52.000000 esmf_regrid-0.9.0/esmf_regrid/esmf_regridder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 11:44:03.350350 esmf_regrid-0.9.0/esmf_regrid/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2023-11-03 11:43:52.000000 esmf_regrid-0.9.0/esmf_regrid/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8886 2023-11-03 11:43:52.000000 esmf_regrid-0.9.0/esmf_regrid/experimental/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5886 2023-11-03 11:43:52.000000 esmf_regrid-0.9.0/esmf_regrid/experimental/unstructured_regrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20018 2023-11-03 11:43:52.000000 esmf_regrid-0.9.0/esmf_regrid/experimental/unstructured_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60865 2023-11-03 11:43:52.000000 esmf_regrid-0.9.0/esmf_regrid/schemes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 11:44:03.350350 esmf_regrid-0.9.0/esmf_regrid/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2023-11-03 11:43:52.000000 esmf_regrid-0.9.0/esmf_regrid/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 11:44:03.350350 esmf_regrid-0.9.0/esmf_regrid/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2023-11-03 11:43:52.000000 esmf_regrid-0.9.0/esmf_regrid/tests/integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 11:44:03.350350 esmf_regrid-0.9.0/esmf_regrid/tests/integration/esmf_regridder/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2023-11-03 11:43:52.000000 esmf_regrid-0.9.0/esmf_regrid/tests/integration/esmf_regridder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2023-11-03 11:43:52.000000 esmf_regrid-0.9.0/esmf_regrid/tests/integration/esmf_regridder/test_Regridder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 11:44:03.350350 esmf_regrid-0.9.0/esmf_regrid/tests/integration/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2023-11-03 11:43:52.000000 esmf_regrid-0.9.0/esmf_regrid/tests/integration/experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 11:44:03.350350 esmf_regrid-0.9.0/esmf_regrid/tests/integration/experimental/unstructured_scheme/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2023-11-03 11:43:52.000000 esmf_regrid-0.9.0/esmf_regrid/tests/integration/experimental/unstructured_scheme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2023-11-03 11:43:52.000000 esmf_regrid-0.9.0/esmf_regrid/tests/integration/experimental/unstructured_scheme/test_regrid_unstructured_to_rectilinear.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 11:44:03.346349 esmf_regrid-0.9.0/esmf_regrid/tests/results/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 11:44:03.346349 esmf_regrid-0.9.0/esmf_regrid/tests/results/unit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 11:44:03.346349 esmf_regrid-0.9.0/esmf_regrid/tests/results/unit/_esmf_sdo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 11:44:03.350350 esmf_regrid-0.9.0/esmf_regrid/tests/results/unit/_esmf_sdo/test_GridInfo/
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2023-11-03 11:43:52.000000 esmf_regrid-0.9.0/esmf_regrid/tests/results/unit/_esmf_sdo/test_GridInfo/small_grid.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 11:44:03.346349 esmf_regrid-0.9.0/esmf_regrid/tests/results/unit/experimental/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 11:44:03.346349 esmf_regrid-0.9.0/esmf_regrid/tests/results/unit/experimental/unstructured_regrid/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 11:44:03.354350 esmf_regrid-0.9.0/esmf_regrid/tests/results/unit/experimental/unstructured_regrid/test_MeshInfo/
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2023-11-03 11:43:52.000000 esmf_regrid-0.9.0/esmf_regrid/tests/results/unit/experimental/unstructured_regrid/test_MeshInfo/small_mesh.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 11:44:03.354350 esmf_regrid-0.9.0/esmf_regrid/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2023-11-03 11:43:52.000000 esmf_regrid-0.9.0/esmf_regrid/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 11:44:03.354350 esmf_regrid-0.9.0/esmf_regrid/tests/unit/_esmf_sdo/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2023-11-03 11:43:52.000000 esmf_regrid-0.9.0/esmf_regrid/tests/unit/_esmf_sdo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2023-11-03 11:43:52.000000 esmf_regrid-0.9.0/esmf_regrid/tests/unit/_esmf_sdo/test_GridInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4028 2023-11-03 11:43:52.000000 esmf_regrid-0.9.0/esmf_regrid/tests/unit/_esmf_sdo/test_RefinedGridInfo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 11:44:03.354350 esmf_regrid-0.9.0/esmf_regrid/tests/unit/esmf_regridder/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2023-11-03 11:43:52.000000 esmf_regrid-0.9.0/esmf_regrid/tests/unit/esmf_regridder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8023 2023-11-03 11:43:52.000000 esmf_regrid-0.9.0/esmf_regrid/tests/unit/esmf_regridder/test_Regridder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 11:44:03.354350 esmf_regrid-0.9.0/esmf_regrid/tests/unit/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2023-11-03 11:43:52.000000 esmf_regrid-0.9.0/esmf_regrid/tests/unit/experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 11:44:03.354350 esmf_regrid-0.9.0/esmf_regrid/tests/unit/experimental/io/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2023-11-03 11:43:52.000000 esmf_regrid-0.9.0/esmf_regrid/tests/unit/experimental/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11658 2023-11-03 11:43:52.000000 esmf_regrid-0.9.0/esmf_regrid/tests/unit/experimental/io/test_round_tripping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2023-11-03 11:43:52.000000 esmf_regrid-0.9.0/esmf_regrid/tests/unit/experimental/io/test_save_regridder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 11:44:03.354350 esmf_regrid-0.9.0/esmf_regrid/tests/unit/experimental/unstructured_regrid/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2023-11-03 11:43:52.000000 esmf_regrid-0.9.0/esmf_regrid/tests/unit/experimental/unstructured_regrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6521 2023-11-03 11:43:52.000000 esmf_regrid-0.9.0/esmf_regrid/tests/unit/experimental/unstructured_regrid/test_MeshInfo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 11:44:03.354350 esmf_regrid-0.9.0/esmf_regrid/tests/unit/experimental/unstructured_scheme/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2023-11-03 11:43:52.000000 esmf_regrid-0.9.0/esmf_regrid/tests/unit/experimental/unstructured_scheme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17795 2023-11-03 11:43:52.000000 esmf_regrid-0.9.0/esmf_regrid/tests/unit/experimental/unstructured_scheme/test_GridToMeshESMFRegridder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16234 2023-11-03 11:43:52.000000 esmf_regrid-0.9.0/esmf_regrid/tests/unit/experimental/unstructured_scheme/test_MeshToGridESMFRegridder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10026 2023-11-03 11:43:52.000000 esmf_regrid-0.9.0/esmf_regrid/tests/unit/experimental/unstructured_scheme/test_regrid_rectilinear_to_unstructured.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7777 2023-11-03 11:43:52.000000 esmf_regrid-0.9.0/esmf_regrid/tests/unit/experimental/unstructured_scheme/test_regrid_unstructured_to_rectilinear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6067 2023-11-03 11:43:52.000000 esmf_regrid-0.9.0/esmf_regrid/tests/unit/experimental/unstructured_scheme/test_regrid_unstructured_to_unstructured.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 11:44:03.358350 esmf_regrid-0.9.0/esmf_regrid/tests/unit/schemes/
+-rw-r--r--   0 runner    (1001) docker     (127)     7465 2023-11-03 11:43:52.000000 esmf_regrid-0.9.0/esmf_regrid/tests/unit/schemes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2188 2023-11-03 11:43:52.000000 esmf_regrid-0.9.0/esmf_regrid/tests/unit/schemes/test_ESMFAreaWeighted.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10844 2023-11-03 11:43:52.000000 esmf_regrid-0.9.0/esmf_regrid/tests/unit/schemes/test_ESMFAreaWeightedRegridder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2023-11-03 11:43:52.000000 esmf_regrid-0.9.0/esmf_regrid/tests/unit/schemes/test_ESMFBilinear.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11626 2023-11-03 11:43:52.000000 esmf_regrid-0.9.0/esmf_regrid/tests/unit/schemes/test_ESMFBilinearRegridder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2023-11-03 11:43:52.000000 esmf_regrid-0.9.0/esmf_regrid/tests/unit/schemes/test_ESMFNearest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12112 2023-11-03 11:43:52.000000 esmf_regrid-0.9.0/esmf_regrid/tests/unit/schemes/test_ESMFNearestRegridder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2023-11-03 11:43:52.000000 esmf_regrid-0.9.0/esmf_regrid/tests/unit/schemes/test__ESMFRegridder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3012 2023-11-03 11:43:52.000000 esmf_regrid-0.9.0/esmf_regrid/tests/unit/schemes/test__create_cube.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8645 2023-11-03 11:43:52.000000 esmf_regrid-0.9.0/esmf_regrid/tests/unit/schemes/test__cube_to_GridInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10043 2023-11-03 11:43:52.000000 esmf_regrid-0.9.0/esmf_regrid/tests/unit/schemes/test__mesh_to_MeshInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2023-11-03 11:43:52.000000 esmf_regrid-0.9.0/esmf_regrid/tests/unit/schemes/test__regrid_unstructured_to_rectilinear__prepare.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15808 2023-11-03 11:43:52.000000 esmf_regrid-0.9.0/esmf_regrid/tests/unit/schemes/test_regrid_rectilinear_to_rectilinear.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 11:44:03.350350 esmf_regrid-0.9.0/esmf_regrid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2023-11-03 11:44:03.000000 esmf_regrid-0.9.0/esmf_regrid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3178 2023-11-03 11:44:03.000000 esmf_regrid-0.9.0/esmf_regrid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-03 11:44:03.000000 esmf_regrid-0.9.0/esmf_regrid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-03 11:44:03.000000 esmf_regrid-0.9.0/esmf_regrid.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2023-11-03 11:44:03.000000 esmf_regrid-0.9.0/esmf_regrid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2023-11-03 11:44:03.000000 esmf_regrid-0.9.0/esmf_regrid.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2023-11-03 11:43:52.000000 esmf_regrid-0.9.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 11:44:03.358350 esmf_regrid-0.9.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2023-11-03 11:43:52.000000 esmf_regrid-0.9.0/requirements/core.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2023-11-03 11:43:52.000000 esmf_regrid-0.9.0/requirements/optional-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2023-11-03 11:43:52.000000 esmf_regrid-0.9.0/requirements/optional-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-03 11:44:03.358350 esmf_regrid-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2023-11-03 11:43:52.000000 esmf_regrid-0.9.0/setup.py
```

### Comparing `esmf_regrid-0.8.0/CHANGELOG.md` & `esmf_regrid-0.9.0/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,33 @@
 
 # Change Log
 All notable changes to this project will be documented in this file.
  
 The format is based on [Keep a Changelog](http://keepachangelog.com/)
 and this project adheres to [Semantic Versioning](http://semver.org/).
 
+## [0.9] - 2023-11-03
+
+### Added
+
+- [PR#178](https://github.com/SciTools-incubator/iris-esmf-regrid/pull/178)
+  Added support for coordinate systems with non-degree type units.
+  [@stephenworsley](https://github.com/stephenworsley)
+
+- [PR#311](https://github.com/SciTools-incubator/iris-esmf-regrid/pull/311)
+  Added support for Mesh to Mesh regridding.
+  [@HGWright](https://github.com/HGWright)
+
+### Fixed
+
+- [PR#301](https://github.com/SciTools-incubator/iris-esmf-regrid/pull/301)
+  Fixed a bug which caused errors when regridding with the node locations
+  of a mesh whose face_node_connectivity had non-zero start_index.
+  [@stephenworsley](https://github.com/stephenworsley)
+
 ## [0.8] - 2023-08-22
 
 ### Added
 
 - [PR#289](https://github.com/SciTools-incubator/iris-esmf-regrid/pull/289)
   Added the ability to regrid onto a Mesh as a target instead of a Cube.
   [@stephenworsley](https://github.com/stephenworsley)
```

### Comparing `esmf_regrid-0.8.0/LICENSE` & `esmf_regrid-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `esmf_regrid-0.8.0/PKG-INFO` & `esmf_regrid-0.9.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esmf_regrid
-Version: 0.8.0
+Version: 0.9.0
 Summary: Iris regridding scheme using ESMF
 Author-email: ESMF Regrid Contributors <scitools.pub@gmail.com>
 License: BSD-3-Clause
 Project-URL: Code, https://github.com/SciTools-incubator/iris-esmf-regrid
 Project-URL: Docs, https://iris-esmf-regrid.readthedocs.io/en/stable
 Project-URL: Issues, https://github.com/SciTools-incubator/iris-esmf-regrid/issues
 Keywords: esmf,regrid
@@ -16,17 +16,32 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: cartopy
+Requires-Dist: cf-units
+Requires-Dist: numpy>=1.19
+Requires-Dist: scipy
+Requires-Dist: scitools-iris
 Provides-Extra: dev
+Requires-Dist: asv; extra == "dev"
+Requires-Dist: codecov; extra == "dev"
+Requires-Dist: nox; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
 Provides-Extra: docs
-License-File: LICENSE
+Requires-Dist: pydata-sphinx-theme; extra == "docs"
+Requires-Dist: sphinx; extra == "docs"
+Requires-Dist: sphinx-copybutton; extra == "docs"
+Requires-Dist: sphinxcontrib-apidoc; extra == "docs"
 
 # iris-esmf-regrid
 
 [![Build Status](https://api.cirrus-ci.com/github/SciTools-incubator/iris-esmf-regrid.svg)](https://cirrus-ci.com/github/SciTools-incubator/iris-esmf-regrid)
 [![Documentation Status](https://readthedocs.org/projects/iris-esmf-regrid/badge/?version=latest)](https://iris-esmf-regrid.readthedocs.io/en/latest/?badge=latest)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/SciTools-incubator/iris-esmf-regrid/main.svg)](https://results.pre-commit.ci/latest/github/SciTools-incubator/iris-esmf-regrid/master)
 [![codecov](https://codecov.io/gh/SciTools-incubator/iris-esmf-regrid/branch/main/graph/badge.svg?token=PKBXEHOZFT)](https://codecov.io/gh/SciTools-incubator/iris-esmf-regrid)
```

### Comparing `esmf_regrid-0.8.0/README.md` & `esmf_regrid-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `esmf_regrid-0.8.0/esmf_regrid/_esmf_sdo.py` & `esmf_regrid-0.9.0/esmf_regrid/_esmf_sdo.py`

 * *Files identical despite different names*

### Comparing `esmf_regrid-0.8.0/esmf_regrid/esmf_regridder.py` & `esmf_regrid-0.9.0/esmf_regrid/esmf_regridder.py`

 * *Files identical despite different names*

### Comparing `esmf_regrid-0.8.0/esmf_regrid/experimental/io.py` & `esmf_regrid-0.9.0/esmf_regrid/experimental/io.py`

 * *Files identical despite different names*

### Comparing `esmf_regrid-0.8.0/esmf_regrid/experimental/unstructured_regrid.py` & `esmf_regrid-0.9.0/esmf_regrid/experimental/unstructured_regrid.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,25 +71,27 @@
         self.nsi = node_start_index
         self.esi = elem_start_index
         self.areas = areas
         self.elem_coords = elem_coords
         if location == "face":
             field_kwargs = {"meshloc": esmpy.MeshLoc.ELEMENT}
             shape = (len(face_node_connectivity),)
+            index_offset = self.esi
         elif location == "node":
             field_kwargs = {"meshloc": esmpy.MeshLoc.NODE}
             shape = (len(node_coords),)
+            index_offset = self.nsi
         else:
             raise ValueError(
                 f"The mesh location '{location}' is not supported, only "
                 f"'face' and 'node' are supported."
             )
         super().__init__(
             shape=shape,
-            index_offset=self.esi,
+            index_offset=index_offset,
             field_kwargs=field_kwargs,
             mask=mask,
         )
 
     def _as_esmf_info(self):
         # ESMF uses a slightly different format to UGRID,
         # the data must be translated into a form ESMF understands
```

### Comparing `esmf_regrid-0.8.0/esmf_regrid/experimental/unstructured_scheme.py` & `esmf_regrid-0.9.0/esmf_regrid/experimental/unstructured_scheme.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 from esmf_regrid.schemes import (
     _ESMFRegridder,
     _get_mask,
     _regrid_rectilinear_to_unstructured__perform,
     _regrid_rectilinear_to_unstructured__prepare,
     _regrid_unstructured_to_rectilinear__perform,
     _regrid_unstructured_to_rectilinear__prepare,
+    _regrid_unstructured_to_unstructured__perform,
+    _regrid_unstructured_to_unstructured__prepare,
 )
 
 
 def regrid_unstructured_to_rectilinear(
     src_cube,
     grid_cube,
     mdtol=0,
@@ -349,7 +351,81 @@
             use_src_mask=use_src_mask,
             use_tgt_mask=use_tgt_mask,
             tgt_location=tgt_location,
         )
         self.resolution = src_resolution
         self.mesh, self.location = self._tgt
         self.grid_x, self.grid_y = self._src
+
+
+def regrid_unstructured_to_unstructured(
+    src_mesh_cube,
+    tgt_mesh_cube,
+    mdtol=0,
+    method="conservative",
+    use_src_mask=False,
+    use_tgt_mask=False,
+):
+    r"""
+    Regrid rectilinear :class:`~iris.cube.Cube` onto unstructured mesh.
+
+    Return a new :class:`~iris.cube.Cube` with :attr:`~iris.cube.Cube.data`
+    values calculated using weights generated by :mod:`esmpy` to give the weighted
+    mean of :attr:`~iris.cube.Cube.data` values from ``src_mesh_cube`` regridded onto the
+    horizontal mesh of ``tgt_mesh_cube``. The resulting cube will have the same
+    ``mesh_dim`` as ``src_mesh_cube``.
+
+    Parameters
+    ----------
+    src_mesh_cube : :class:`iris.cube.Cube`
+        A unstructured instance of :class:`~iris.cube.Cube` that supplies the data,
+        metadata and coordinates.
+    tgt_mesh_cube : :class:`iris.cube.Cube`
+        An unstructured instance of :class:`~iris.cube.Cube` that supplies the desired
+        horizontal mesh definition.
+    mdtol : float, default=0
+        Tolerance of missing data. The value returned in each element of the
+        returned :class:`~iris.cube.Cube`\\ 's :attr:`~iris.cube.Cube.data` array
+        will be masked if the fraction of masked
+        data in the overlapping cells of the source cube exceeds ``mdtol``. This
+        fraction is calculated based on the area of masked cells within each
+        target cell. ``mdtol=0`` means no missing data is tolerated while ``mdtol=1``
+        will mean the resulting element will be masked if and only if all the
+        overlapping cells of the ``src_cube`` are masked.
+    method : str, default="conservative"
+        Either "conservative", "bilinear" or "nearest". Corresponds to the :mod:`esmpy` methods
+        :attr:`~esmpy.api.constants.RegridMethod.CONSERVE` or
+        :attr:`~esmpy.api.constants.RegridMethod.BILINEAR` or
+        :attr:`~esmpy.api.constants.RegridMethod.NEAREST` used to calculate weights.
+    use_src_mask : :obj:`~numpy.typing.ArrayLike` or bool, default=False
+        Either an array representing the cells in the source to ignore, or else
+        a boolean value. If True, this array is taken from the mask on the data
+        in ``src_cube``. If False, no mask will be taken and all points will
+        be used in weights calculation.
+    use_tgt_mask : :obj:`~numpy.typing.ArrayLike` or bool, default=False
+        Either an array representing the cells in the target to ignore, or else
+        a boolean value. If True, this array is taken from the mask on the data
+        in ``grid_cube``. If False, no mask will be taken and all points
+        will be used in weights calculation.
+
+    Returns
+    -------
+    :class:`iris.cube.Cube`
+        A new :class:`~iris.cube.Cube` instance.
+
+    """
+    if tgt_mesh_cube.mesh is None:
+        raise ValueError("mesh_cube has no mesh.")
+    src_mask = _get_mask(src_mesh_cube, use_src_mask)
+    tgt_mask = _get_mask(tgt_mesh_cube, use_tgt_mask)
+
+    regrid_info = _regrid_unstructured_to_unstructured__prepare(
+        src_mesh_cube,
+        tgt_mesh_cube,
+        method=method,
+        src_mask=src_mask,
+        tgt_mask=tgt_mask,
+    )
+    result = _regrid_unstructured_to_unstructured__perform(
+        src_mesh_cube, regrid_info, mdtol
+    )
+    return result
```

### Comparing `esmf_regrid-0.8.0/esmf_regrid/schemes.py` & `esmf_regrid-0.9.0/esmf_regrid/schemes.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,18 +187,21 @@
             lon_bound_array = lon.contiguous_bounds()
             lat_bound_array = lat.contiguous_bounds()
         else:
             lon_bound_array = _contiguous_masked(lon.bounds, mask)
             lat_bound_array = _contiguous_masked(lat.bounds, mask)
         # 2D coords must be AuxCoords, which do not have a circular attribute.
         circular = False
-    lon_bound_array = lon.units.convert(lon_bound_array, Unit("degrees"))
-    lat_bound_array = lat.units.convert(lat_bound_array, Unit("degrees"))
-    lon_points = lon.units.convert(lon.points, Unit("degrees"))
-    lat_points = lon.units.convert(lat.points, Unit("degrees"))
+    lon_points = lon.points
+    lat_points = lat.points
+    if crs is None:
+        lon_bound_array = lon.units.convert(lon_bound_array, Unit("degrees"))
+        lat_bound_array = lat.units.convert(lat_bound_array, Unit("degrees"))
+        lon_points = lon.units.convert(lon_points, Unit("degrees"))
+        lat_points = lon.units.convert(lat_points, Unit("degrees"))
     if resolution is None:
         grid_info = GridInfo(
             lon_points,
             lat_points,
             lon_bound_array,
             lat_bound_array,
             crs=crs,
@@ -509,14 +512,21 @@
     method,
     precomputed_weights=None,
     src_resolution=None,
     tgt_resolution=None,
     src_mask=None,
     tgt_mask=None,
 ):
+    """
+    First (setup) part of 'regrid_rectilinear_to_rectilinear'.
+
+    Check inputs and calculate the sparse regrid matrix and related info.
+    The 'regrid info' returned can be re-used over many 2d slices.
+
+    """
     tgt_x = _get_coord(tgt_grid_cube, "x")
     tgt_y = _get_coord(tgt_grid_cube, "y")
     src_x = _get_coord(src_grid_cube, "x")
     src_y = _get_coord(src_grid_cube, "y")
 
     if len(src_x.shape) == 1:
         grid_x_dim = src_grid_cube.coord_dims(src_x)[0]
@@ -537,14 +547,20 @@
         regridder=regridder,
     )
 
     return regrid_info
 
 
 def _regrid_rectilinear_to_rectilinear__perform(src_cube, regrid_info, mdtol):
+    """
+    Second (regrid) part of 'regrid_rectilinear_to_rectilinear'.
+
+    Perform the prepared regrid calculation on a single cube.
+
+    """
     grid_x_dim, grid_y_dim = regrid_info.dims
     grid_x, grid_y = regrid_info.target
     regridder = regrid_info.regridder
 
     # Set up a function which can accept just chunk of data as an argument.
     regrid = functools.partial(
         _regrid_along_dims,
@@ -762,25 +778,104 @@
         mesh.to_MeshCoords(location),
         1,
     )
     return new_cube
 
 
 def _regrid_unstructured_to_unstructured__prepare(
-    src_grid_cube,
-    target_mesh_cube,
+    src_mesh_cube,
+    tgt_cube_or_mesh,
     method,
     precomputed_weights=None,
+    src_mask=None,
+    tgt_mask=None,
+    src_location=None,
     tgt_location=None,
 ):
-    raise NotImplementedError
+    """
+    First (setup) part of 'regrid_unstructured_to_unstructured'.
+
+    Check inputs and calculate the sparse regrid matrix and related info.
+    The 'regrid info' returned can be re-used over many 2d slices.
+
+    """
+    if isinstance(tgt_cube_or_mesh, Mesh):
+        mesh = tgt_cube_or_mesh
+        location = tgt_location
+    else:
+        mesh = tgt_cube_or_mesh.mesh
+        location = tgt_cube_or_mesh.location
+
+    mesh_dim = src_mesh_cube.mesh_dim()
+
+    src_meshinfo = _make_meshinfo(
+        src_mesh_cube, method, src_mask, "source", location=src_location
+    )
+    tgt_meshinfo = _make_meshinfo(
+        tgt_cube_or_mesh, method, tgt_mask, "target", location=tgt_location
+    )
+
+    regridder = Regridder(
+        src_meshinfo,
+        tgt_meshinfo,
+        method=method,
+        precomputed_weights=precomputed_weights,
+    )
+
+    regrid_info = RegridInfo(
+        dims=[mesh_dim],
+        target=MeshRecord(mesh, location),
+        regridder=regridder,
+    )
+
+    return regrid_info
 
 
 def _regrid_unstructured_to_unstructured__perform(src_cube, regrid_info, mdtol):
-    raise NotImplementedError
+    """
+    Second (regrid) part of 'regrid_unstructured_to_unstructured'.
+
+    Perform the prepared regrid calculation on a single cube.
+
+    """
+    (mesh_dim,) = regrid_info.dims
+    mesh, location = regrid_info.target
+    regridder = regrid_info.regridder
+
+    regrid = functools.partial(
+        _regrid_along_dims,
+        regridder,
+        dims=[mesh_dim],
+        num_out_dims=1,
+        mdtol=mdtol,
+    )
+    if location == "face":
+        face_node = mesh.face_node_connectivity
+        chunk_shape = (face_node.shape[face_node.location_axis],)
+    elif location == "node":
+        chunk_shape = mesh.node_coords[0].shape
+    else:
+        raise NotImplementedError(f"Unrecognised location {location}.")
+
+    new_data = _map_complete_blocks(
+        src_cube,
+        regrid,
+        (mesh_dim,),
+        chunk_shape,
+    )
+
+    new_cube = _create_cube(
+        new_data,
+        src_cube,
+        (mesh_dim,),
+        mesh.to_MeshCoords(location),
+        1,
+    )
+
+    return new_cube
 
 
 def regrid_rectilinear_to_rectilinear(
     src_cube,
     grid_cube,
     mdtol=0,
     method="conservative",
```

### Comparing `esmf_regrid-0.8.0/esmf_regrid/tests/__init__.py` & `esmf_regrid-0.9.0/esmf_regrid/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `esmf_regrid-0.8.0/esmf_regrid/tests/integration/esmf_regridder/test_Regridder.py` & `esmf_regrid-0.9.0/esmf_regrid/tests/integration/esmf_regridder/test_Regridder.py`

 * *Files identical despite different names*

### Comparing `esmf_regrid-0.8.0/esmf_regrid/tests/integration/experimental/unstructured_scheme/test_regrid_unstructured_to_rectilinear.py` & `esmf_regrid-0.9.0/esmf_regrid/tests/integration/experimental/unstructured_scheme/test_regrid_unstructured_to_rectilinear.py`

 * *Files identical despite different names*

### Comparing `esmf_regrid-0.8.0/esmf_regrid/tests/results/unit/_esmf_sdo/test_GridInfo/small_grid.txt` & `esmf_regrid-0.9.0/esmf_regrid/tests/results/unit/_esmf_sdo/test_GridInfo/small_grid.txt`

 * *Files identical despite different names*

### Comparing `esmf_regrid-0.8.0/esmf_regrid/tests/unit/_esmf_sdo/test_GridInfo.py` & `esmf_regrid-0.9.0/esmf_regrid/tests/unit/_esmf_sdo/test_GridInfo.py`

 * *Files identical despite different names*

### Comparing `esmf_regrid-0.8.0/esmf_regrid/tests/unit/_esmf_sdo/test_RefinedGridInfo.py` & `esmf_regrid-0.9.0/esmf_regrid/tests/unit/_esmf_sdo/test_RefinedGridInfo.py`

 * *Files identical despite different names*

### Comparing `esmf_regrid-0.8.0/esmf_regrid/tests/unit/esmf_regridder/test_Regridder.py` & `esmf_regrid-0.9.0/esmf_regrid/tests/unit/esmf_regridder/test_Regridder.py`

 * *Files identical despite different names*

### Comparing `esmf_regrid-0.8.0/esmf_regrid/tests/unit/experimental/io/test_round_tripping.py` & `esmf_regrid-0.9.0/esmf_regrid/tests/unit/experimental/io/test_round_tripping.py`

 * *Files identical despite different names*

### Comparing `esmf_regrid-0.8.0/esmf_regrid/tests/unit/experimental/unstructured_regrid/test_MeshInfo.py` & `esmf_regrid-0.9.0/esmf_regrid/tests/unit/experimental/unstructured_regrid/test_MeshInfo.py`

 * *Files identical despite different names*

### Comparing `esmf_regrid-0.8.0/esmf_regrid/tests/unit/experimental/unstructured_scheme/test_GridToMeshESMFRegridder.py` & `esmf_regrid-0.9.0/esmf_regrid/tests/unit/experimental/unstructured_scheme/test_GridToMeshESMFRegridder.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,28 +70,29 @@
     # Check metadata and scalar coords.
     expected_cube.data = result.data
     assert expected_cube == result
     expected_cube.data = result_transposed.data
     assert expected_cube == result_transposed
 
 
+@pytest.mark.parametrize("nsi", [0, 1])
 @pytest.mark.parametrize("method", ["bilinear", "nearest"])
-def test_node_friendly_methods(method):
+def test_node_friendly_methods(method, nsi):
     """
     Basic test for :class:`esmf_regrid.experimental.unstructured_scheme.GridToMeshESMFRegridder`.
 
     Tests with method="bilinear" and method="nearest".
     """
     n_lons = 6
     n_lats = 5
     lon_bounds = (-180, 180)
     lat_bounds = (-90, 90)
     src = _grid_cube(n_lons, n_lats, lon_bounds, lat_bounds, circular=True)
-    face_tgt = _gridlike_mesh_cube(n_lons, n_lats, location="face")
-    node_tgt = _gridlike_mesh_cube(n_lons, n_lats, location="node")
+    face_tgt = _gridlike_mesh_cube(n_lons, n_lats, location="face", nsi=nsi)
+    node_tgt = _gridlike_mesh_cube(n_lons, n_lats, location="node", nsi=nsi)
 
     src = _add_metadata(src)
     src.data[:] = 1  # Ensure all data in the source is one.
     face_regridder = GridToMeshESMFRegridder(src, face_tgt, method=method)
     node_regridder = GridToMeshESMFRegridder(src, node_tgt, method=method)
 
     assert face_regridder.regridder.method == method
```

### Comparing `esmf_regrid-0.8.0/esmf_regrid/tests/unit/experimental/unstructured_scheme/test_MeshToGridESMFRegridder.py` & `esmf_regrid-0.9.0/esmf_regrid/tests/unit/experimental/unstructured_scheme/test_MeshToGridESMFRegridder.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,28 +64,29 @@
     assert np.allclose(expected_data, result.data)
 
     # Check metadata and scalar coords.
     expected_cube.data = result.data
     assert expected_cube == result
 
 
+@pytest.mark.parametrize("nsi", [0, 1])
 @pytest.mark.parametrize("method", ["bilinear", "nearest"])
-def test_node_friendly_methods(method):
+def test_node_friendly_methods(method, nsi):
     """
     Basic test for :class:`esmf_regrid.experimental.unstructured_scheme.MeshToGridESMFRegridder`.
 
     Tests with method="bilinear" and method="nearest".
     """
     n_lons = 6
     n_lats = 5
     lon_bounds = (-180, 180)
     lat_bounds = (-90, 90)
     tgt = _grid_cube(n_lons, n_lats, lon_bounds, lat_bounds, circular=True)
-    face_src = _gridlike_mesh_cube(n_lons, n_lats, location="face")
-    node_src = _gridlike_mesh_cube(n_lons, n_lats, location="node")
+    face_src = _gridlike_mesh_cube(n_lons, n_lats, location="face", nsi=nsi)
+    node_src = _gridlike_mesh_cube(n_lons, n_lats, location="node", nsi=nsi)
 
     face_src = _add_metadata(face_src)
     node_src = _add_metadata(node_src)
     # Ensure all data in the source is one.
     face_src.data[:] = 1
     node_src.data[:] = 1
     face_regridder = MeshToGridESMFRegridder(face_src, tgt, method=method)
```

### Comparing `esmf_regrid-0.8.0/esmf_regrid/tests/unit/experimental/unstructured_scheme/test_regrid_rectilinear_to_unstructured.py` & `esmf_regrid-0.9.0/esmf_regrid/tests/unit/experimental/unstructured_scheme/test_regrid_rectilinear_to_unstructured.py`

 * *Files identical despite different names*

### Comparing `esmf_regrid-0.8.0/esmf_regrid/tests/unit/experimental/unstructured_scheme/test_regrid_unstructured_to_rectilinear.py` & `esmf_regrid-0.9.0/esmf_regrid/tests/unit/experimental/unstructured_scheme/test_regrid_unstructured_to_rectilinear.py`

 * *Files identical despite different names*

### Comparing `esmf_regrid-0.8.0/esmf_regrid/tests/unit/schemes/__init__.py` & `esmf_regrid-0.9.0/esmf_regrid/tests/unit/schemes/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """Unit tests for `esmf_regrid.schemes`."""
 
+from iris.coord_systems import OSGB
 import numpy as np
 from numpy import ma
 import pytest
 
+from esmf_regrid.schemes import ESMFAreaWeighted, ESMFBilinear, ESMFNearest
 from esmf_regrid.tests.unit.schemes.test__cube_to_GridInfo import _grid_cube
 from esmf_regrid.tests.unit.schemes.test__mesh_to_MeshInfo import (
     _gridlike_mesh,
     _gridlike_mesh_cube,
 )
 
 
@@ -162,7 +164,54 @@
     regridder_attr = mask_keyword[4:]
 
     # Check that the mask stored on the regridder is correct.
     np.testing.assert_allclose(getattr(rg_from_cube, regridder_attr), mask)
     np.testing.assert_allclose(
         getattr(rg_from_different, regridder_attr), mask_different
     )
+
+
+def _test_non_degree_crs(scheme):
+    """Test regridding scheme is compatible with coordinates with non-degree units."""
+    coord_system = OSGB()
+
+    # This definition comes from a small section of real user data.
+    n_lons_src = 2
+    n_lats_src = 3
+    lon_bounds = (-197500, -192500)
+    lat_bounds = (1247500, 1237500)
+    tm_cube = _grid_cube(
+        n_lons_src,
+        n_lats_src,
+        lon_bounds,
+        lat_bounds,
+        circular=False,
+        coord_system=coord_system,
+        standard_names=["projection_x_coordinate", "projection_y_coordinate"],
+        units="m",
+    )
+    data = np.arange(n_lats_src * n_lons_src).reshape([n_lats_src, n_lons_src])
+    tm_cube.data = data
+
+    n_lons_tgt = 12
+    n_lats_tgt = 14
+    lon_bounds_tgt = (-13, -12.8)
+    lat_bounds_tgt = (60.5, 60.7)
+    cube_tgt = _grid_cube(
+        n_lons_tgt, n_lats_tgt, lon_bounds_tgt, lat_bounds_tgt, circular=True
+    )
+
+    result = tm_cube.regrid(cube_tgt, scheme())
+
+    # Set expected results, this varies depending on the scheme.
+    if scheme is ESMFAreaWeighted:
+        expected_sum, expected_unmasked = 50.86147272655136, 21
+    elif scheme is ESMFBilinear:
+        expected_sum, expected_unmasked = 35.90837983047451, 13
+    elif scheme is ESMFNearest:
+        expected_sum, expected_unmasked = 490, 168
+
+    # Check that the data is as expected.
+    assert np.isclose(result.data.sum(), expected_sum)
+
+    # Check that the number of masked points is as expected.
+    assert (1 - result.data.mask).sum() == expected_unmasked
```

### Comparing `esmf_regrid-0.8.0/esmf_regrid/tests/unit/schemes/test_ESMFAreaWeighted.py` & `esmf_regrid-0.9.0/esmf_regrid/tests/unit/schemes/test_ESMFAreaWeighted.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,20 +4,27 @@
 
 from esmf_regrid.schemes import ESMFAreaWeighted
 from esmf_regrid.tests.unit.schemes.__init__ import (
     _test_cube_regrid,
     _test_invalid_mdtol,
     _test_mask_from_init,
     _test_mask_from_regridder,
+    _test_non_degree_crs,
 )
 
 
 @pytest.mark.parametrize(
     "src_type,tgt_type",
-    [("grid", "grid"), ("grid", "mesh"), ("grid", "just_mesh"), ("mesh", "grid")],
+    [
+        ("grid", "grid"),
+        ("grid", "mesh"),
+        ("grid", "just_mesh"),
+        ("mesh", "grid"),
+        ("mesh", "mesh"),
+    ],
 )
 def test_cube_regrid(src_type, tgt_type):
     """
     Test that ESMFAreaWeighted can be passed to a cubes regrid method.
 
     Checks that regridding occurs and that mdtol is used correctly.
     """
@@ -58,7 +65,12 @@
     Test initialisation of :class:`esmf_regrid.schemes.ESMFAreaWeighted`.
 
     Checks that initialisation fails when tgt_location is not "face".
     """
     match = "For area weighted regridding, target location must be 'face'."
     with pytest.raises(ValueError, match=match):
         _ = ESMFAreaWeighted(tgt_location="node")
+
+
+def test_non_degree_crs():
+    """Test for coordinates with non-degree units."""
+    _test_non_degree_crs(ESMFAreaWeighted)
```

### Comparing `esmf_regrid-0.8.0/esmf_regrid/tests/unit/schemes/test_ESMFAreaWeightedRegridder.py` & `esmf_regrid-0.9.0/esmf_regrid/tests/unit/schemes/test_ESMFAreaWeightedRegridder.py`

 * *Files identical despite different names*

### Comparing `esmf_regrid-0.8.0/esmf_regrid/tests/unit/schemes/test_ESMFBilinear.py` & `esmf_regrid-0.9.0/esmf_regrid/tests/unit/schemes/test_ESMFBilinear.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,20 +4,27 @@
 
 from esmf_regrid.schemes import ESMFBilinear
 from esmf_regrid.tests.unit.schemes.__init__ import (
     _test_cube_regrid,
     _test_invalid_mdtol,
     _test_mask_from_init,
     _test_mask_from_regridder,
+    _test_non_degree_crs,
 )
 
 
 @pytest.mark.parametrize(
     "src_type,tgt_type",
-    [("grid", "grid"), ("grid", "mesh"), ("grid", "just_mesh"), ("mesh", "grid")],
+    [
+        ("grid", "grid"),
+        ("grid", "mesh"),
+        ("grid", "just_mesh"),
+        ("mesh", "grid"),
+        ("mesh", "mesh"),
+    ],
 )
 def test_cube_regrid(src_type, tgt_type):
     """
     Test that ESMFBilinear can be passed to a cubes regrid method.
 
     Checks that regridding occurs and that mdtol is used correctly.
     """
@@ -47,7 +54,12 @@
 def test_mask_from_regridder(mask_keyword):
     """
     Test regridder method of :class:`esmf_regrid.schemes.ESMFBilinear`.
 
     Checks that use_src_mask and use_tgt_mask are passed down correctly.
     """
     _test_mask_from_regridder(ESMFBilinear, mask_keyword)
+
+
+def test_non_degree_crs():
+    """Test for coordinates with non-degree units."""
+    _test_non_degree_crs(ESMFBilinear)
```

### Comparing `esmf_regrid-0.8.0/esmf_regrid/tests/unit/schemes/test_ESMFBilinearRegridder.py` & `esmf_regrid-0.9.0/esmf_regrid/tests/unit/schemes/test_ESMFBilinearRegridder.py`

 * *Files identical despite different names*

### Comparing `esmf_regrid-0.8.0/esmf_regrid/tests/unit/schemes/test_ESMFNearest.py` & `esmf_regrid-0.9.0/esmf_regrid/tests/unit/schemes/test_ESMFNearest.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,25 +4,32 @@
 from numpy import ma
 import pytest
 
 from esmf_regrid.schemes import ESMFNearest
 from esmf_regrid.tests.unit.schemes.__init__ import (
     _test_mask_from_init,
     _test_mask_from_regridder,
+    _test_non_degree_crs,
 )
 from esmf_regrid.tests.unit.schemes.test__cube_to_GridInfo import _grid_cube
 from esmf_regrid.tests.unit.schemes.test__mesh_to_MeshInfo import (
     _gridlike_mesh,
     _gridlike_mesh_cube,
 )
 
 
 @pytest.mark.parametrize(
     "src_type,tgt_type",
-    [("grid", "grid"), ("grid", "mesh"), ("grid", "just_mesh"), ("mesh", "grid")],
+    [
+        ("grid", "grid"),
+        ("grid", "mesh"),
+        ("grid", "just_mesh"),
+        ("mesh", "grid"),
+        ("mesh", "mesh"),
+    ],
 )
 def test_cube_regrid(src_type, tgt_type):
     """
     Test that ESMFNearest can be passed to a cubes regrid method.
 
     Checks that regridding occurs.
     """
@@ -90,7 +97,12 @@
 def test_mask_from_regridder(mask_keyword):
     """
     Test regridder method of :class:`esmf_regrid.schemes.ESMFNearest`.
 
     Checks that use_src_mask and use_tgt_mask are passed down correctly.
     """
     _test_mask_from_regridder(ESMFNearest, mask_keyword)
+
+
+def test_non_degree_crs():
+    """Test for coordinates with non-degree units."""
+    _test_non_degree_crs(ESMFNearest)
```

### Comparing `esmf_regrid-0.8.0/esmf_regrid/tests/unit/schemes/test_ESMFNearestRegridder.py` & `esmf_regrid-0.9.0/esmf_regrid/tests/unit/schemes/test_ESMFNearestRegridder.py`

 * *Files identical despite different names*

### Comparing `esmf_regrid-0.8.0/esmf_regrid/tests/unit/schemes/test__ESMFRegridder.py` & `esmf_regrid-0.9.0/esmf_regrid/tests/unit/schemes/test__ESMFRegridder.py`

 * *Files identical despite different names*

### Comparing `esmf_regrid-0.8.0/esmf_regrid/tests/unit/schemes/test__create_cube.py` & `esmf_regrid-0.9.0/esmf_regrid/tests/unit/schemes/test__create_cube.py`

 * *Files identical despite different names*

### Comparing `esmf_regrid-0.8.0/esmf_regrid/tests/unit/schemes/test__cube_to_GridInfo.py` & `esmf_regrid-0.9.0/esmf_regrid/tests/unit/schemes/test__cube_to_GridInfo.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,29 +63,31 @@
 def _grid_cube(
     n_lons,
     n_lats,
     lon_outer_bounds,
     lat_outer_bounds,
     circular=False,
     coord_system=None,
+    standard_names=["longitude", "latitude"],
+    units="degrees",
 ):
     lon_points, lon_bounds = _generate_points_and_bounds(n_lons, lon_outer_bounds)
     lon = DimCoord(
         lon_points,
-        "longitude",
-        units="degrees",
+        standard_names[0],
+        units=units,
         bounds=lon_bounds,
         circular=circular,
         coord_system=coord_system,
     )
     lat_points, lat_bounds = _generate_points_and_bounds(n_lats, lat_outer_bounds)
     lat = DimCoord(
         lat_points,
-        "latitude",
-        units="degrees",
+        standard_names[1],
+        units=units,
         bounds=lat_bounds,
         coord_system=coord_system,
     )
 
     data = np.zeros([n_lats, n_lons])
     cube = Cube(data)
     cube.add_dim_coord(lon, 1)
```

### Comparing `esmf_regrid-0.8.0/esmf_regrid/tests/unit/schemes/test__mesh_to_MeshInfo.py` & `esmf_regrid-0.9.0/esmf_regrid/tests/unit/schemes/test__mesh_to_MeshInfo.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     lat_values = [60, -60, -60, 60, 10, 0]
     lons = AuxCoord(lon_values, standard_name="longitude")
     lats = AuxCoord(lat_values, standard_name="latitude")
     mesh = Mesh(2, ((lons, "x"), (lats, "y")), fnc)
     return mesh
 
 
-def _gridlike_mesh(n_lons, n_lats):
+def _gridlike_mesh(n_lons, n_lats, nsi=0):
     """
     Generate a global mesh with geometry similar to a rectilinear grid.
 
     The resulting mesh will have n_lons cells spanning its longitudes and
     n_lats cells spanning its latitudes for a total of (n_lons * n_lats) cells.
     Note that the cells neighbouring the poles will actually be triangular while
     the rest of the cells will be rectangular.
@@ -155,17 +155,17 @@
     lat_centers = np.linspace(-90, 90, (2 * n_lats) + 1)[1::2]
     lon_center_array, lat_center_array = np.meshgrid(lon_centers, lat_centers)
     face_lons = lon_center_array.flatten()
     face_lats = lat_center_array.flatten()
 
     # Translate the mesh information into iris objects.
     fnc = Connectivity(
-        fnc_ma,
+        fnc_ma + nsi,
         cf_role="face_node_connectivity",
-        start_index=0,
+        start_index=nsi,
     )
     enc = Connectivity(
         enc_array,
         cf_role="edge_node_connectivity",
         start_index=0,
     )
     lons = AuxCoord(node_lons, standard_name="longitude")
@@ -187,16 +187,16 @@
         edge_x=edge_lon_coord,
         edge_y=edge_lat_coord,
     )
     mesh.long_name = "example mesh"
     return mesh
 
 
-def _gridlike_mesh_cube(n_lons, n_lats, location="face"):
-    mesh = _gridlike_mesh(n_lons, n_lats)
+def _gridlike_mesh_cube(n_lons, n_lats, location="face", nsi=0):
+    mesh = _gridlike_mesh(n_lons, n_lats, nsi=nsi)
     mesh_coord_x, mesh_coord_y = mesh.to_MeshCoords(location)
     data = np.zeros_like(mesh_coord_x.points)
     cube = Cube(data)
     cube.add_aux_coord(mesh_coord_x, 0)
     cube.add_aux_coord(mesh_coord_y, 0)
     return cube
```

### Comparing `esmf_regrid-0.8.0/esmf_regrid/tests/unit/schemes/test__regrid_unstructured_to_rectilinear__prepare.py` & `esmf_regrid-0.9.0/esmf_regrid/tests/unit/schemes/test__regrid_unstructured_to_rectilinear__prepare.py`

 * *Files identical despite different names*

### Comparing `esmf_regrid-0.8.0/esmf_regrid/tests/unit/schemes/test_regrid_rectilinear_to_rectilinear.py` & `esmf_regrid-0.9.0/esmf_regrid/tests/unit/schemes/test_regrid_rectilinear_to_rectilinear.py`

 * *Files identical despite different names*

### Comparing `esmf_regrid-0.8.0/esmf_regrid.egg-info/PKG-INFO` & `esmf_regrid-0.9.0/esmf_regrid.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esmf-regrid
-Version: 0.8.0
+Version: 0.9.0
 Summary: Iris regridding scheme using ESMF
 Author-email: ESMF Regrid Contributors <scitools.pub@gmail.com>
 License: BSD-3-Clause
 Project-URL: Code, https://github.com/SciTools-incubator/iris-esmf-regrid
 Project-URL: Docs, https://iris-esmf-regrid.readthedocs.io/en/stable
 Project-URL: Issues, https://github.com/SciTools-incubator/iris-esmf-regrid/issues
 Keywords: esmf,regrid
@@ -16,17 +16,32 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: cartopy
+Requires-Dist: cf-units
+Requires-Dist: numpy>=1.19
+Requires-Dist: scipy
+Requires-Dist: scitools-iris
 Provides-Extra: dev
+Requires-Dist: asv; extra == "dev"
+Requires-Dist: codecov; extra == "dev"
+Requires-Dist: nox; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
 Provides-Extra: docs
-License-File: LICENSE
+Requires-Dist: pydata-sphinx-theme; extra == "docs"
+Requires-Dist: sphinx; extra == "docs"
+Requires-Dist: sphinx-copybutton; extra == "docs"
+Requires-Dist: sphinxcontrib-apidoc; extra == "docs"
 
 # iris-esmf-regrid
 
 [![Build Status](https://api.cirrus-ci.com/github/SciTools-incubator/iris-esmf-regrid.svg)](https://cirrus-ci.com/github/SciTools-incubator/iris-esmf-regrid)
 [![Documentation Status](https://readthedocs.org/projects/iris-esmf-regrid/badge/?version=latest)](https://iris-esmf-regrid.readthedocs.io/en/latest/?badge=latest)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/SciTools-incubator/iris-esmf-regrid/main.svg)](https://results.pre-commit.ci/latest/github/SciTools-incubator/iris-esmf-regrid/master)
 [![codecov](https://codecov.io/gh/SciTools-incubator/iris-esmf-regrid/branch/main/graph/badge.svg?token=PKBXEHOZFT)](https://codecov.io/gh/SciTools-incubator/iris-esmf-regrid)
```

### Comparing `esmf_regrid-0.8.0/esmf_regrid.egg-info/SOURCES.txt` & `esmf_regrid-0.9.0/esmf_regrid.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 esmf_regrid/tests/unit/experimental/unstructured_regrid/__init__.py
 esmf_regrid/tests/unit/experimental/unstructured_regrid/test_MeshInfo.py
 esmf_regrid/tests/unit/experimental/unstructured_scheme/__init__.py
 esmf_regrid/tests/unit/experimental/unstructured_scheme/test_GridToMeshESMFRegridder.py
 esmf_regrid/tests/unit/experimental/unstructured_scheme/test_MeshToGridESMFRegridder.py
 esmf_regrid/tests/unit/experimental/unstructured_scheme/test_regrid_rectilinear_to_unstructured.py
 esmf_regrid/tests/unit/experimental/unstructured_scheme/test_regrid_unstructured_to_rectilinear.py
+esmf_regrid/tests/unit/experimental/unstructured_scheme/test_regrid_unstructured_to_unstructured.py
 esmf_regrid/tests/unit/schemes/__init__.py
 esmf_regrid/tests/unit/schemes/test_ESMFAreaWeighted.py
 esmf_regrid/tests/unit/schemes/test_ESMFAreaWeightedRegridder.py
 esmf_regrid/tests/unit/schemes/test_ESMFBilinear.py
 esmf_regrid/tests/unit/schemes/test_ESMFBilinearRegridder.py
 esmf_regrid/tests/unit/schemes/test_ESMFNearest.py
 esmf_regrid/tests/unit/schemes/test_ESMFNearestRegridder.py
```

### Comparing `esmf_regrid-0.8.0/pyproject.toml` & `esmf_regrid-0.9.0/pyproject.toml`

 * *Files identical despite different names*

