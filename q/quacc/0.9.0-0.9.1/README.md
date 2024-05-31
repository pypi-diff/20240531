# Comparing `tmp/quacc-0.9.0.tar.gz` & `tmp/quacc-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quacc-0.9.0.tar", last modified: Thu May 23 21:18:29 2024, max compression
+gzip compressed data, was "quacc-0.9.1.tar", last modified: Fri May 31 20:50:14 2024, max compression
```

## Comparing `quacc-0.9.0.tar` & `quacc-0.9.1.tar`

### file list

```diff
@@ -1,177 +1,177 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:18:29.440842 quacc-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-23 21:17:10.000000 quacc-0.9.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-23 21:17:10.000000 quacc-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6471 2024-05-23 21:18:29.440842 quacc-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-05-23 21:17:10.000000 quacc-0.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-05-23 21:17:10.000000 quacc-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 21:18:29.440842 quacc-0.9.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:18:29.404842 quacc-0.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:18:29.408842 quacc-0.9.0/src/quacc/
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:18:29.412842 quacc-0.9.0/src/quacc/_cli/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5337 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/_cli/quacc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:18:29.412842 quacc-0.9.0/src/quacc/atoms/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/atoms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7246 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/atoms/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     5421 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/atoms/defects.py
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/atoms/deformation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/atoms/phonons.py
--rw-r--r--   0 runner    (1001) docker     (127)    13791 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/atoms/slabs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:18:29.412842 quacc-0.9.0/src/quacc/calculators/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/calculators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:18:29.412842 quacc-0.9.0/src/quacc/calculators/espresso/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/calculators/espresso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17294 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/calculators/espresso/espresso.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:18:29.416842 quacc-0.9.0/src/quacc/calculators/espresso/presets/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/calculators/espresso/presets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/calculators/espresso/presets/esm_metal_slab_efficiency.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/calculators/espresso/presets/esm_metal_slab_precision.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/calculators/espresso/presets/esm_semiconductors_slab_efficiency.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/calculators/espresso/presets/esm_semiconductors_slab_precision.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/calculators/espresso/presets/metal_efficiency.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/calculators/espresso/presets/metal_precision.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/calculators/espresso/presets/molecule_efficiency.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/calculators/espresso/presets/semiconductors_efficiency.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/calculators/espresso/presets/semiconductors_precision.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    17071 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/calculators/espresso/presets/sssp_1.3.0_pbe_efficiency.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    17181 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/calculators/espresso/presets/sssp_1.3.0_pbe_precision.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/calculators/espresso/presets/tough_metal_clusters_efficiency.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    10467 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/calculators/espresso/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:18:29.416842 quacc-0.9.0/src/quacc/calculators/qchem/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/calculators/qchem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/calculators/qchem/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/calculators/qchem/params.py
--rw-r--r--   0 runner    (1001) docker     (127)    12373 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/calculators/qchem/qchem.py
--rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/calculators/qchem/qchem_custodian.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:18:29.416842 quacc-0.9.0/src/quacc/calculators/vasp/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/calculators/vasp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/calculators/vasp/io.py
--rw-r--r--   0 runner    (1001) docker     (127)    14869 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/calculators/vasp/params.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:18:29.420842 quacc-0.9.0/src/quacc/calculators/vasp/presets/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/calculators/vasp/presets/BulkSet.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/calculators/vasp/presets/QMOFSet.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/calculators/vasp/presets/SlabSet.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/calculators/vasp/presets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/calculators/vasp/presets/magmoms_base.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/calculators/vasp/presets/magmoms_qmof.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/calculators/vasp/presets/setups_pbe54.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/calculators/vasp/presets/setups_qmof.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    11305 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/calculators/vasp/vasp.py
--rw-r--r--   0 runner    (1001) docker     (127)     7751 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/calculators/vasp/vasp_custodian.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:18:29.420842 quacc-0.9.0/src/quacc/recipes/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:18:29.420842 quacc-0.9.0/src/quacc/recipes/common/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/common/defects.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/common/elastic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/common/phonons.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/common/slabs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:18:29.420842 quacc-0.9.0/src/quacc/recipes/dftb/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/dftb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/dftb/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/dftb/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:18:29.420842 quacc-0.9.0/src/quacc/recipes/emt/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/emt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/emt/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3410 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/emt/defects.py
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/emt/elastic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/emt/phonons.py
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/emt/slabs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:18:29.424842 quacc-0.9.0/src/quacc/recipes/espresso/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/espresso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8370 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/espresso/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    13161 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/espresso/bands.py
--rw-r--r--   0 runner    (1001) docker     (127)    15333 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/espresso/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    10208 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/espresso/dos.py
--rw-r--r--   0 runner    (1001) docker     (127)    24148 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/espresso/phonons.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:18:29.424842 quacc-0.9.0/src/quacc/recipes/gaussian/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/gaussian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/gaussian/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/gaussian/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:18:29.424842 quacc-0.9.0/src/quacc/recipes/gulp/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/gulp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/gulp/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/gulp/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:18:29.424842 quacc-0.9.0/src/quacc/recipes/lj/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/lj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/lj/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:18:29.424842 quacc-0.9.0/src/quacc/recipes/mlp/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/mlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/mlp/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/mlp/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/mlp/phonons.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:18:29.424842 quacc-0.9.0/src/quacc/recipes/newtonnet/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/newtonnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7243 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/newtonnet/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     9109 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/newtonnet/ts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:18:29.428842 quacc-0.9.0/src/quacc/recipes/onetep/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/onetep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/onetep/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/onetep/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:18:29.428842 quacc-0.9.0/src/quacc/recipes/orca/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/orca/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6275 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/orca/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    12465 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/orca/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:18:29.428842 quacc-0.9.0/src/quacc/recipes/psi4/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/psi4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/psi4/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/psi4/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:18:29.428842 quacc-0.9.0/src/quacc/recipes/qchem/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/qchem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4009 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/qchem/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5629 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/qchem/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/qchem/ts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:18:29.428842 quacc-0.9.0/src/quacc/recipes/tblite/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/tblite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4817 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/tblite/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/tblite/phonons.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:18:29.428842 quacc-0.9.0/src/quacc/recipes/vasp/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/vasp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/vasp/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9471 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/vasp/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    12469 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/vasp/mp.py
--rw-r--r--   0 runner    (1001) docker     (127)    10130 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/vasp/qmof.py
--rw-r--r--   0 runner    (1001) docker     (127)     6770 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/vasp/slabs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:18:29.432842 quacc-0.9.0/src/quacc/runners/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/runners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12522 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/runners/ase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/runners/phonons.py
--rw-r--r--   0 runner    (1001) docker     (127)     5514 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/runners/prep.py
--rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/runners/thermo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:18:29.432842 quacc-0.9.0/src/quacc/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:18:29.432842 quacc-0.9.0/src/quacc/schemas/_aliases/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/schemas/_aliases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/schemas/_aliases/ase.py
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/schemas/_aliases/atoms.py
--rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/schemas/_aliases/cclib.py
--rw-r--r--   0 runner    (1001) docker     (127)     7144 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/schemas/_aliases/emmet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/schemas/_aliases/phonons.py
--rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/schemas/_aliases/vasp.py
--rw-r--r--   0 runner    (1001) docker     (127)    13451 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/schemas/ase.py
--rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/schemas/atoms.py
--rw-r--r--   0 runner    (1001) docker     (127)    17451 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/schemas/cclib.py
--rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/schemas/phonons.py
--rw-r--r--   0 runner    (1001) docker     (127)     5485 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/schemas/prep.py
--rw-r--r--   0 runner    (1001) docker     (127)    12266 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/schemas/vasp.py
--rw-r--r--   0 runner    (1001) docker     (127)    16906 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:18:29.432842 quacc-0.9.0/src/quacc/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6494 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/utils/dicts.py
--rw-r--r--   0 runner    (1001) docker     (127)     9240 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/utils/kpts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/utils/lists.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:18:29.436842 quacc-0.9.0/src/quacc/wflow_tools/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/wflow_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/wflow_tools/customizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/wflow_tools/db.py
--rw-r--r--   0 runner    (1001) docker     (127)    13248 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/wflow_tools/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:18:29.436842 quacc-0.9.0/src/quacc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6471 2024-05-23 21:18:29.000000 quacc-0.9.0/src/quacc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5154 2024-05-23 21:18:29.000000 quacc-0.9.0/src/quacc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 21:18:29.000000 quacc-0.9.0/src/quacc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-23 21:18:29.000000 quacc-0.9.0/src/quacc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-23 21:18:29.000000 quacc-0.9.0/src/quacc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-23 21:18:29.000000 quacc-0.9.0/src/quacc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:50:14.026778 quacc-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-31 20:48:59.000000 quacc-0.9.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-31 20:48:59.000000 quacc-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6468 2024-05-31 20:50:14.026778 quacc-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-05-31 20:48:59.000000 quacc-0.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5990 2024-05-31 20:48:59.000000 quacc-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 20:50:14.026778 quacc-0.9.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:50:13.998778 quacc-0.9.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:50:14.002778 quacc-0.9.1/src/quacc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:50:14.002778 quacc-0.9.1/src/quacc/_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5337 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/_cli/quacc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:50:14.002778 quacc-0.9.1/src/quacc/atoms/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/atoms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7246 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/atoms/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5585 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/atoms/defects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/atoms/deformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/atoms/phonons.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13791 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/atoms/slabs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:50:14.006778 quacc-0.9.1/src/quacc/calculators/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/calculators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:50:14.006778 quacc-0.9.1/src/quacc/calculators/espresso/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/calculators/espresso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17017 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/calculators/espresso/espresso.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:50:14.006778 quacc-0.9.1/src/quacc/calculators/espresso/presets/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/calculators/espresso/presets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/calculators/espresso/presets/esm_metal_slab_efficiency.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/calculators/espresso/presets/esm_metal_slab_precision.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/calculators/espresso/presets/esm_semiconductors_slab_efficiency.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/calculators/espresso/presets/esm_semiconductors_slab_precision.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/calculators/espresso/presets/metal_efficiency.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/calculators/espresso/presets/metal_precision.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/calculators/espresso/presets/molecule_efficiency.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/calculators/espresso/presets/semiconductors_efficiency.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/calculators/espresso/presets/semiconductors_precision.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    17071 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/calculators/espresso/presets/sssp_1.3.0_pbe_efficiency.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    17181 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/calculators/espresso/presets/sssp_1.3.0_pbe_precision.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/calculators/espresso/presets/tough_metal_clusters_efficiency.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    10467 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/calculators/espresso/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:50:14.006778 quacc-0.9.1/src/quacc/calculators/qchem/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/calculators/qchem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/calculators/qchem/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/calculators/qchem/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12373 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/calculators/qchem/qchem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/calculators/qchem/qchem_custodian.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:50:14.010778 quacc-0.9.1/src/quacc/calculators/vasp/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/calculators/vasp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/calculators/vasp/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14881 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/calculators/vasp/params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:50:14.010778 quacc-0.9.1/src/quacc/calculators/vasp/presets/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/calculators/vasp/presets/BulkSet.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/calculators/vasp/presets/QMOFSet.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/calculators/vasp/presets/SlabSet.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/calculators/vasp/presets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/calculators/vasp/presets/magmoms_base.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/calculators/vasp/presets/magmoms_qmof.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/calculators/vasp/presets/setups_pbe54.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/calculators/vasp/presets/setups_qmof.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11305 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/calculators/vasp/vasp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7751 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/calculators/vasp/vasp_custodian.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:50:14.010778 quacc-0.9.1/src/quacc/recipes/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/recipes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:50:14.010778 quacc-0.9.1/src/quacc/recipes/common/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/recipes/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/recipes/common/defects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/recipes/common/elastic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/recipes/common/phonons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/recipes/common/slabs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:50:14.010778 quacc-0.9.1/src/quacc/recipes/dftb/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/recipes/dftb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/recipes/dftb/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/recipes/dftb/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:50:14.014778 quacc-0.9.1/src/quacc/recipes/emt/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/recipes/emt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/recipes/emt/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/recipes/emt/defects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/recipes/emt/elastic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/recipes/emt/phonons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/recipes/emt/slabs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:50:14.014778 quacc-0.9.1/src/quacc/recipes/espresso/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/recipes/espresso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7905 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/recipes/espresso/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12087 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/recipes/espresso/bands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14118 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/recipes/espresso/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9722 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/recipes/espresso/dos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22933 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/recipes/espresso/phonons.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:50:14.014778 quacc-0.9.1/src/quacc/recipes/gaussian/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/recipes/gaussian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/recipes/gaussian/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/recipes/gaussian/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:50:14.014778 quacc-0.9.1/src/quacc/recipes/gulp/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/recipes/gulp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/recipes/gulp/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/recipes/gulp/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:50:14.014778 quacc-0.9.1/src/quacc/recipes/lj/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/recipes/lj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/recipes/lj/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:50:14.014778 quacc-0.9.1/src/quacc/recipes/mlp/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/recipes/mlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/recipes/mlp/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/recipes/mlp/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/recipes/mlp/phonons.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:50:14.014778 quacc-0.9.1/src/quacc/recipes/newtonnet/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/recipes/newtonnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7249 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/recipes/newtonnet/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9139 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/recipes/newtonnet/ts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:50:14.018778 quacc-0.9.1/src/quacc/recipes/onetep/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/recipes/onetep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4308 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/recipes/onetep/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/recipes/onetep/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:50:14.018778 quacc-0.9.1/src/quacc/recipes/orca/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/recipes/orca/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6283 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/recipes/orca/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12465 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/recipes/orca/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:50:14.018778 quacc-0.9.1/src/quacc/recipes/psi4/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/recipes/psi4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/recipes/psi4/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/recipes/psi4/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:50:14.018778 quacc-0.9.1/src/quacc/recipes/qchem/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/recipes/qchem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4009 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/recipes/qchem/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5649 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/recipes/qchem/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9973 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/recipes/qchem/ts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:50:14.018778 quacc-0.9.1/src/quacc/recipes/tblite/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/recipes/tblite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4877 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/recipes/tblite/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3572 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/recipes/tblite/phonons.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:50:14.018778 quacc-0.9.1/src/quacc/recipes/vasp/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/recipes/vasp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/recipes/vasp/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9471 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/recipes/vasp/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12480 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/recipes/vasp/mp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10130 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/recipes/vasp/qmof.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6770 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/recipes/vasp/slabs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:50:14.018778 quacc-0.9.1/src/quacc/runners/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12554 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/runners/ase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/runners/phonons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5514 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/runners/prep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/runners/thermo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:50:14.022778 quacc-0.9.1/src/quacc/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:50:14.022778 quacc-0.9.1/src/quacc/schemas/_aliases/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/schemas/_aliases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/schemas/_aliases/ase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/schemas/_aliases/atoms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/schemas/_aliases/cclib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7144 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/schemas/_aliases/emmet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/schemas/_aliases/phonons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/schemas/_aliases/vasp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13367 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/schemas/ase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/schemas/atoms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17451 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/schemas/cclib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/schemas/phonons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5485 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/schemas/prep.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12266 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/schemas/vasp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17728 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:50:14.022778 quacc-0.9.1/src/quacc/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6494 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/utils/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9240 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/utils/kpts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/utils/lists.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:50:14.022778 quacc-0.9.1/src/quacc/wflow_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/wflow_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/wflow_tools/customizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/wflow_tools/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13248 2024-05-31 20:48:59.000000 quacc-0.9.1/src/quacc/wflow_tools/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:50:14.022778 quacc-0.9.1/src/quacc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6468 2024-05-31 20:50:13.000000 quacc-0.9.1/src/quacc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5154 2024-05-31 20:50:13.000000 quacc-0.9.1/src/quacc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 20:50:13.000000 quacc-0.9.1/src/quacc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-31 20:50:13.000000 quacc-0.9.1/src/quacc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-31 20:50:13.000000 quacc-0.9.1/src/quacc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-31 20:50:13.000000 quacc-0.9.1/src/quacc.egg-info/top_level.txt
```

### Comparing `quacc-0.9.0/LICENSE.md` & `quacc-0.9.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `quacc-0.9.0/PKG-INFO` & `quacc-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quacc
-Version: 0.9.0
+Version: 0.9.1
 Summary: A platform to enable high-throughput, database-driven quantum chemistry and computational materials science
 Author-email: "Andrew S. Rosen" <asrosen@princeton.edu>
 Maintainer-email: "Andrew S. Rosen" <asrosen@princeton.edu>
 License: BSD-3
 Project-URL: repository, https://github.com/Quantum-Accelerators/quacc
 Project-URL: documentation, https://quantum-accelerators.github.io/quacc/
 Project-URL: changelog, https://github.com/Quantum-Accelerators/quacc/blob/main/CHANGELOG.md
@@ -20,15 +20,15 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: ase>=3.23.0b1
+Requires-Dist: ase>=3.23.0
 Requires-Dist: cclib>=1.8
 Requires-Dist: custodian>=2024.3.12
 Requires-Dist: emmet-core>=0.80.0
 Requires-Dist: maggma>=0.64.0
 Requires-Dist: monty>=2024.5.15
 Requires-Dist: numpy>=1.25.0
 Requires-Dist: psutil
@@ -55,15 +55,15 @@
 Requires-Dist: mace-torch>=0.3.3; extra == "mlp"
 Requires-Dist: torch-dftd>=0.4.0; extra == "mlp"
 Provides-Extra: mp
 Requires-Dist: atomate2>=0.0.14; extra == "mp"
 Provides-Extra: newtonnet
 Requires-Dist: newtonnet>=1.1; extra == "newtonnet"
 Provides-Extra: parsl
-Requires-Dist: parsl[monitoring]>=2023.10.23; platform_system != "Windows" and extra == "parsl"
+Requires-Dist: parsl[monitoring]>=2024.5.27; platform_system != "Windows" and extra == "parsl"
 Provides-Extra: phonons
 Requires-Dist: phonopy>=2.20.0; extra == "phonons"
 Requires-Dist: seekpath>=2.1.0; extra == "phonons"
 Provides-Extra: prefect
 Requires-Dist: prefect[dask]>=2.19.0; extra == "prefect"
 Requires-Dist: dask-jobqueue>=0.8.2; extra == "prefect"
 Provides-Extra: redun
```

### Comparing `quacc-0.9.0/README.md` & `quacc-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `quacc-0.9.0/pyproject.toml` & `quacc-0.9.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "quacc"
 description="A platform to enable high-throughput, database-driven quantum chemistry and computational materials science"
-version = "0.9.0"
+version = "0.9.1"
 readme = "README.md"
 license = { text = "BSD-3" }
 authors = [{ name = "Andrew S. Rosen", email = "asrosen@princeton.edu" }]
 maintainers = [{ name = "Andrew S. Rosen", email = "asrosen@princeton.edu" }]
 keywords = ["high-throughput", "automated", "workflow", "dft"]
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -23,15 +23,15 @@
     "Topic :: Scientific/Engineering",
     "Operating System :: Microsoft :: Windows",
     "Operating System :: Unix",
     "Operating System :: MacOS",
 ]
 requires-python = ">=3.9"
 dependencies = [
-    "ase>=3.23.0b1", # for Atoms object and calculators
+    "ase>=3.23.0", # for Atoms object and calculators
     "cclib>=1.8", # for I/O parsing of molecular DFT codes
     "custodian>=2024.3.12", # for automated error corrections
     "emmet-core>=0.80.0", # for pre-made schemas
     "maggma>=0.64.0", # for database handling
     "monty>=2024.5.15", # miscellaneous Python utilities
     "numpy>=1.25.0", # for array handling
     "psutil", # for getting compute architecture details
@@ -46,15 +46,15 @@
 covalent = ["covalent>=0.234.1-rc.0; platform_system!='Windows'", "covalent-cloud>=0.39.0; platform_system!='Windows'"]
 dask = ["dask[distributed]>=2023.12.1", "dask-jobqueue>=0.8.2"]
 defects = ["pymatgen-analysis-defects>=2023.8.22", "shakenbreak>=3.2.0"]
 jobflow = ["jobflow[fireworks]>=0.1.14", "jobflow-remote>=0.1.0"]
 mlp = ["matgl>=1.0.0", "chgnet>=0.3.3", "mace-torch>=0.3.3", "torch-dftd>=0.4.0"]
 mp = ["atomate2>=0.0.14"]
 newtonnet = ["newtonnet>=1.1"]
-parsl = ["parsl[monitoring]>=2023.10.23; platform_system!='Windows'"]
+parsl = ["parsl[monitoring]>=2024.5.27; platform_system!='Windows'"]
 phonons = ["phonopy>=2.20.0", "seekpath>=2.1.0"]
 prefect = ["prefect[dask]>=2.19.0", "dask-jobqueue>=0.8.2"]
 redun = ["redun>=0.16.2"]
 sella = ["sella>=2.3.4"]
 tblite = ["tblite>=0.3.0; platform_system=='Linux'"]
 dev = ["pytest>=7.4.0", "pytest-cov>=3.0.0", "ruff>=0.0.285"]
 docs = [
```

### Comparing `quacc-0.9.0/src/quacc/__init__.py` & `quacc-0.9.1/src/quacc/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Init data for quacc."""
 
 from __future__ import annotations
 
 import logging
+import os
 from importlib.metadata import version
 
 from ase.atoms import Atoms
 from pymatgen.io.ase import MSONAtoms
 
 from quacc.settings import QuaccSettings, change_settings
 from quacc.utils.dicts import Remove
@@ -33,14 +34,17 @@
 # Make Atoms MSONable
 Atoms.as_dict = MSONAtoms.as_dict
 Atoms.from_dict = MSONAtoms.from_dict
 
 # Load the settings
 SETTINGS = QuaccSettings()
 
+# Ignore ASE config file
+os.environ["ASE_CONFIG_PATH"] = ""
+
 # Set logging info
 logging.basicConfig(level=logging.DEBUG if SETTINGS.DEBUG else logging.INFO)
 
 # Monkeypatching for Prefect
 if SETTINGS.WORKFLOW_ENGINE == "prefect":
     from prefect.futures import PrefectFuture
     from prefect.states import State
```

### Comparing `quacc-0.9.0/src/quacc/_cli/quacc.py` & `quacc-0.9.1/src/quacc/_cli/quacc.py`

 * *Files identical despite different names*

### Comparing `quacc-0.9.0/src/quacc/atoms/core.py` & `quacc-0.9.1/src/quacc/atoms/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.9.0/src/quacc/atoms/defects.py` & `quacc-0.9.1/src/quacc/atoms/defects.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,44 +6,44 @@
 from typing import TYPE_CHECKING
 
 from monty.dev import requires
 from pymatgen.core.periodic_table import DummySpecies
 from pymatgen.entries.computed_entries import ComputedStructureEntry
 from pymatgen.io.ase import AseAtomsAdaptor
 
-has_deps = (
-    find_spec("pymatgen.analysis.defects") is not None
-    and find_spec("shakenbreak") is not None
-)
-
-if has_deps:
+has_pmg_defects = bool(find_spec("pymatgen.analysis.defects"))
+has_shakenbreak = bool(find_spec("shakenbreak"))
+if has_pmg_defects:
     from pymatgen.analysis.defects.generators import VacancyGenerator
+    from pymatgen.analysis.defects.thermo import DefectEntry
+if has_shakenbreak:
     from shakenbreak.input import Distortions
 
 
 if TYPE_CHECKING:
     from ase.atoms import Atoms
     from numpy.typing import NDArray
     from pymatgen.core.structure import Structure
 
-    if has_deps:
+    if has_pmg_defects:
         from pymatgen.analysis.defects.core import Defect
         from pymatgen.analysis.defects.generators import (
             AntiSiteGenerator,
             ChargeInterstitialGenerator,
             InterstitialGenerator,
             SubstitutionGenerator,
             VoronoiInterstitialGenerator,
         )
-        from pymatgen.analysis.defects.thermo import DefectEntry
 
 
 @requires(
-    has_deps, "Missing defect dependencies. Please run pip install quacc[defects]"
+    has_pmg_defects,
+    "Missing pymatgen-analysis-defects. Please run pip install quacc[defects]",
 )
+@requires(has_shakenbreak, "Missing shakenbreak. Please run pip install quacc[defects]")
 def make_defects_from_bulk(
     atoms: Atoms,
     defect_gen: (
         AntiSiteGenerator
         | ChargeInterstitialGenerator
         | InterstitialGenerator
         | SubstitutionGenerator
@@ -135,14 +135,18 @@
                 "defect": defect,
             }
             final_defect.info["defect_stats"] = defect_stats
             final_defects.append(final_defect)
     return final_defects
 
 
+@requires(
+    has_pmg_defects,
+    "Missing pymatgen-analysis-defects. Please run pip install quacc[defects]",
+)
 def get_defect_entry_from_defect(
     defect: Defect, defect_supercell: Structure, defect_charge: int
 ) -> DefectEntry:
     """
     Function to generate DefectEntry object from Defect object.
 
     Parameters
@@ -155,16 +159,14 @@
         charge state of defect
 
     Returns
     -------
     DefectEntry
         defect entry
     """
-    from pymatgen.analysis.defects.thermo import DefectEntry  # skipcq: PYL-W0621
-
     # Find defect's fractional coordinates and remove it from supercell
     for site in defect_supercell:
         if site.species.elements[0].symbol == DummySpecies().symbol:
             dummy_site = site
             break
     defect_supercell.remove(dummy_site)
```

### Comparing `quacc-0.9.0/src/quacc/atoms/deformation.py` & `quacc-0.9.1/src/quacc/atoms/deformation.py`

 * *Files identical despite different names*

### Comparing `quacc-0.9.0/src/quacc/atoms/phonons.py` & `quacc-0.9.1/src/quacc/atoms/phonons.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import numpy as np
 from monty.dev import requires
 from pymatgen.io.ase import AseAtomsAdaptor
 from pymatgen.io.phonopy import get_phonopy_structure, get_pmg_structure
 from pymatgen.symmetry.analyzer import SpacegroupAnalyzer
 
-has_phonopy = find_spec("phonopy")
+has_phonopy = bool(find_spec("phonopy"))
 
 if has_phonopy:
     from phonopy import Phonopy
 
 if TYPE_CHECKING:
     from ase.atoms import Atoms
```

### Comparing `quacc-0.9.0/src/quacc/atoms/slabs.py` & `quacc-0.9.1/src/quacc/atoms/slabs.py`

 * *Files identical despite different names*

### Comparing `quacc-0.9.0/src/quacc/calculators/espresso/espresso.py` & `quacc-0.9.1/src/quacc/calculators/espresso/espresso.py`

 * *Files 2% similar despite different names*

```diff
@@ -359,15 +359,14 @@
     Templates are used to set the binary and input/output file names.
     """
 
     def __init__(
         self,
         input_atoms: Atoms | None = None,
         preset: str | None = None,
-        parallel_info: dict[str, Any] | None = None,
         template: EspressoTemplate | None = None,
         **kwargs,
     ) -> None:
         """
         Initialize the Espresso calculator.
 
         Parameters
@@ -376,18 +375,14 @@
             The input Atoms object to be used for the calculation.
         preset
             The name of a YAML file containing a list of parameters to use as
             a "preset" for the calculator. quacc will automatically look in the
             `ESPRESSO_PRESET_DIR` (default: quacc/calculators/espresso/presets),
             The .yaml extension is not necessary. Any user-supplied calculator
             **kwargs will override any corresponding preset values.
-        parallel_info
-            parallel_info is a dictionary passed to the ASE Espresso calculator
-            profile. It is used to specify prefixes for the command line arguments.
-            See the ASE documentation for more details.
         template
             ASE calculator templace which can be used to specify which espresso
             binary will be used in the calculation. This is taken care of by recipe
             in most cases.
         **kwargs
             Additional arguments to be passed to the Espresso calculator. Takes all valid
             ASE calculator arguments, such as `input_data` and `kpts`. Refer to
@@ -397,15 +392,14 @@
 
         Returns
         -------
         None
         """
         self.input_atoms = input_atoms or Atoms()
         self.preset = preset
-        self.parallel_info = parallel_info
         self.kwargs = kwargs
         self.user_calc_params = {}
 
         template = template or EspressoTemplate("pw")
 
         self._binary = template.binary
 
@@ -427,15 +421,16 @@
         self._pseudo_path = (
             self.user_calc_params.get("input_data", {})
             .get("control", {})
             .get("pseudo_dir", str(SETTINGS.ESPRESSO_PSEUDO))
         )
 
         profile = EspressoProfile(
-            self._bin_path, self._pseudo_path, parallel_info=parallel_info
+            f"{SETTINGS.ESPRESSO_PARALLEL_CMD[0]} {self._bin_path} {SETTINGS.ESPRESSO_PARALLEL_CMD[1]}",
+            self._pseudo_path,
         )
 
         super().__init__(
             template=template,
             profile=profile,
             directory=".",
             parameters=self.user_calc_params,
```

### Comparing `quacc-0.9.0/src/quacc/calculators/espresso/presets/sssp_1.3.0_pbe_efficiency.yaml` & `quacc-0.9.1/src/quacc/calculators/espresso/presets/sssp_1.3.0_pbe_efficiency.yaml`

 * *Files identical despite different names*

### Comparing `quacc-0.9.0/src/quacc/calculators/espresso/presets/sssp_1.3.0_pbe_precision.yaml` & `quacc-0.9.1/src/quacc/calculators/espresso/presets/sssp_1.3.0_pbe_precision.yaml`

 * *Files identical despite different names*

### Comparing `quacc-0.9.0/src/quacc/calculators/espresso/presets/tough_metal_clusters_efficiency.yaml` & `quacc-0.9.1/src/quacc/calculators/espresso/presets/tough_metal_clusters_efficiency.yaml`

 * *Files identical despite different names*

### Comparing `quacc-0.9.0/src/quacc/calculators/espresso/utils.py` & `quacc-0.9.1/src/quacc/calculators/espresso/utils.py`

 * *Files identical despite different names*

### Comparing `quacc-0.9.0/src/quacc/calculators/qchem/io.py` & `quacc-0.9.1/src/quacc/calculators/qchem/io.py`

 * *Files identical despite different names*

### Comparing `quacc-0.9.0/src/quacc/calculators/qchem/params.py` & `quacc-0.9.1/src/quacc/calculators/qchem/params.py`

 * *Files identical despite different names*

### Comparing `quacc-0.9.0/src/quacc/calculators/qchem/qchem.py` & `quacc-0.9.1/src/quacc/calculators/qchem/qchem.py`

 * *Files identical despite different names*

### Comparing `quacc-0.9.0/src/quacc/calculators/qchem/qchem_custodian.py` & `quacc-0.9.1/src/quacc/calculators/qchem/qchem_custodian.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from monty.dev import requires
 
 from quacc import SETTINGS
 
 if TYPE_CHECKING:
     from pathlib import Path
 
-has_ob = find_spec("openbabel")
+has_ob = bool(find_spec("openbabel"))
 
 _DEFAULT_SETTING = ()
 
 
 @requires(
     has_ob, "Openbabel must be installed. Try conda install -c conda-forge openbabel"
 )
```

### Comparing `quacc-0.9.0/src/quacc/calculators/vasp/io.py` & `quacc-0.9.1/src/quacc/calculators/vasp/io.py`

 * *Files identical despite different names*

### Comparing `quacc-0.9.0/src/quacc/calculators/vasp/params.py` & `quacc-0.9.1/src/quacc/calculators/vasp/params.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 """Parameter-related utilities for the Vasp calculator."""
 
 from __future__ import annotations
 
 import logging
-from importlib import util
+from importlib.util import find_spec
 from typing import TYPE_CHECKING
 
 import numpy as np
 from ase.calculators.vasp import Vasp as Vasp_
 from monty.dev import requires
 from pymatgen.io.ase import AseAtomsAdaptor
 
 from quacc.atoms.core import check_is_metal
 from quacc.utils.kpts import convert_pmg_kpts
 
-has_atomate2 = util.find_spec("atomate2")
+has_atomate2 = bool(find_spec("atomate2"))
+
 if TYPE_CHECKING:
     from typing import Any, Literal
 
     from ase.atoms import Atoms
     from pymatgen.io.vasp.sets import DictSet
 
     from quacc.utils.files import SourceDirectory
```

### Comparing `quacc-0.9.0/src/quacc/calculators/vasp/presets/magmoms_qmof.yaml` & `quacc-0.9.1/src/quacc/calculators/vasp/presets/magmoms_qmof.yaml`

 * *Files identical despite different names*

### Comparing `quacc-0.9.0/src/quacc/calculators/vasp/presets/setups_pbe54.yaml` & `quacc-0.9.1/src/quacc/calculators/vasp/presets/setups_pbe54.yaml`

 * *Files identical despite different names*

### Comparing `quacc-0.9.0/src/quacc/calculators/vasp/presets/setups_qmof.yaml` & `quacc-0.9.1/src/quacc/calculators/vasp/presets/setups_qmof.yaml`

 * *Files identical despite different names*

### Comparing `quacc-0.9.0/src/quacc/calculators/vasp/vasp.py` & `quacc-0.9.1/src/quacc/calculators/vasp/vasp.py`

 * *Files identical despite different names*

### Comparing `quacc-0.9.0/src/quacc/calculators/vasp/vasp_custodian.py` & `quacc-0.9.1/src/quacc/calculators/vasp/vasp_custodian.py`

 * *Files identical despite different names*

### Comparing `quacc-0.9.0/src/quacc/recipes/common/defects.py` & `quacc-0.9.1/src/quacc/recipes/common/defects.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,33 +6,32 @@
 from typing import TYPE_CHECKING
 
 from monty.dev import requires
 
 from quacc import subflow
 from quacc.atoms.defects import make_defects_from_bulk
 
-has_deps = (
-    find_spec("shakenbreak") is not None
-    and find_spec("pymatgen.analysis.defects") is not None
-)
+has_pmg_defects = bool(find_spec("pymatgen.analysis.defects"))
+has_shakenbreak = bool(find_spec("shakenbreak"))
 
 
 if TYPE_CHECKING:
     from typing import Any
 
     from ase.atoms import Atoms
 
     from quacc import Job
 
 
 @subflow
 @requires(
-    has_deps,
-    "shakenbreak and pymatgen-analysis-defects must be installed. Run `pip install quacc[defects]`",
+    has_pmg_defects,
+    "Missing pymatgen-analysis-defects. Please run pip install quacc[defects]",
 )
+@requires(has_shakenbreak, "Missing shakenbreak. Please run pip install quacc[defects]")
 def bulk_to_defects_subflow(
     atoms: Atoms,
     relax_job: Job,
     static_job: Job | None = None,
     make_defects_kwargs: dict[str, Any] | None = None,
 ) -> list[dict]:
     """
```

### Comparing `quacc-0.9.0/src/quacc/recipes/common/elastic.py` & `quacc-0.9.1/src/quacc/recipes/common/elastic.py`

 * *Files identical despite different names*

### Comparing `quacc-0.9.0/src/quacc/recipes/common/phonons.py` & `quacc-0.9.1/src/quacc/recipes/common/phonons.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,32 +8,32 @@
 from monty.dev import requires
 
 from quacc import job, subflow
 from quacc.atoms.phonons import get_phonopy, phonopy_atoms_to_ase_atoms
 from quacc.runners.phonons import run_phonopy
 from quacc.schemas.phonons import summarize_phonopy
 
-has_deps = find_spec("phonopy") is not None and find_spec("seekpath") is not None
+has_phonopy = bool(find_spec("phonopy"))
+has_seekpath = bool(find_spec("seekpath"))
 
 if TYPE_CHECKING:
     from typing import Any
 
     from ase.atoms import Atoms
 
     from quacc import Job
     from quacc.schemas._aliases.phonons import PhononSchema
 
-    if has_deps:
+    if has_phonopy:
         from phonopy import Phonopy
 
 
 @subflow
-@requires(
-    has_deps, "Phonopy and seekpath must be installed. Run `pip install quacc[phonons]`"
-)
+@requires(has_phonopy, "Phonopy must be installed. Run `pip install quacc[phonons]`")
+@requires(has_seekpath, "Seekpath must be installed. Run `pip install quacc[phonons]`")
 def phonon_subflow(
     atoms: Atoms,
     force_job: Job,
     symprec: float = 1e-4,
     min_lengths: float | tuple[float, float, float] | None = 20.0,
     supercell_matrix: (
         tuple[tuple[int, int, int], tuple[int, int, int], tuple[int, int, int]] | None
```

### Comparing `quacc-0.9.0/src/quacc/recipes/common/slabs.py` & `quacc-0.9.1/src/quacc/recipes/common/slabs.py`

 * *Files identical despite different names*

### Comparing `quacc-0.9.0/src/quacc/recipes/dftb/_base.py` & `quacc-0.9.1/src/quacc/recipes/dftb/_base.py`

 * *Files identical despite different names*

### Comparing `quacc-0.9.0/src/quacc/recipes/dftb/core.py` & `quacc-0.9.1/src/quacc/recipes/dftb/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.9.0/src/quacc/recipes/emt/core.py` & `quacc-0.9.1/src/quacc/recipes/emt/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.9.0/src/quacc/recipes/emt/defects.py` & `quacc-0.9.1/src/quacc/recipes/emt/defects.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,51 +1,52 @@
 """Defect recipes for EMT."""
 
 from __future__ import annotations
 
+from importlib.util import find_spec
 from typing import TYPE_CHECKING
 
 from monty.dev import requires
 
 from quacc import flow
 from quacc.recipes.common.defects import bulk_to_defects_subflow
 from quacc.recipes.emt.core import relax_job, static_job
 from quacc.utils.dicts import recursive_dict_merge
 from quacc.wflow_tools.customizers import customize_funcs
 
-try:
-    import shakenbreak  # noqa: F401
-    from pymatgen.analysis.defects.generators import VacancyGenerator
+has_pmg_defects = bool(find_spec("pymatgen.analysis.defects"))
+has_shakenbreak = bool(find_spec("shakenbreak"))
 
-    has_deps = True
-except ImportError:
-    has_deps = False
+if has_pmg_defects:
+    from pymatgen.analysis.defects.generators import VacancyGenerator
 
 
 if TYPE_CHECKING:
     from typing import Any, Callable
 
     from ase.atoms import Atoms
 
     from quacc.schemas._aliases.ase import OptSchema, RunSchema
 
-    if has_deps:
+    if has_pmg_defects:
         from pymatgen.analysis.defects.generators import (
             AntiSiteGenerator,
             ChargeInterstitialGenerator,
             InterstitialGenerator,
             SubstitutionGenerator,
             VoronoiInterstitialGenerator,
         )
 
 
 @flow
 @requires(
-    has_deps, "Missing defect dependencies. Please run pip install quacc[defects]"
+    has_pmg_defects,
+    "Missing pymatgen-analysis-defects. Please run pip install quacc[defects]",
 )
+@requires(has_shakenbreak, "Missing shakenbreak. Please run pip install quacc[defects]")
 def bulk_to_defects_flow(
     atoms: Atoms,
     defect_gen: (
         AntiSiteGenerator
         | ChargeInterstitialGenerator
         | InterstitialGenerator
         | SubstitutionGenerator
```

### Comparing `quacc-0.9.0/src/quacc/recipes/emt/elastic.py` & `quacc-0.9.1/src/quacc/recipes/emt/elastic.py`

 * *Files identical despite different names*

### Comparing `quacc-0.9.0/src/quacc/recipes/emt/phonons.py` & `quacc-0.9.1/src/quacc/recipes/emt/phonons.py`

 * *Files identical despite different names*

### Comparing `quacc-0.9.0/src/quacc/recipes/emt/slabs.py` & `quacc-0.9.1/src/quacc/recipes/emt/slabs.py`

 * *Files identical despite different names*

### Comparing `quacc-0.9.0/src/quacc/recipes/espresso/_base.py` & `quacc-0.9.1/src/quacc/recipes/espresso/_base.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 def run_and_summarize(
     atoms: Atoms | None = None,
     preset: str | None = None,
     template: EspressoTemplate | None = None,
     profile: EspressoProfile | None = None,
     calc_defaults: dict[str, Any] | None = None,
     calc_swaps: dict[str, Any] | None = None,
-    parallel_info: dict[str, Any] | None = None,
     additional_fields: dict[str, Any] | None = None,
     copy_files: (
         SourceDirectory
         | list[SourceDirectory]
         | dict[SourceDirectory, Filenames]
         | None
     ) = None,
@@ -61,16 +60,14 @@
         EspressoProfile to use
     calc_defaults
         The default calculator parameters.
     calc_swaps
         Custom kwargs for the espresso calculator. Set a value to
         `quacc.Remove` to remove a pre-existing key entirely. For a list of available
         keys, refer to the [ase.calculators.espresso.Espresso][] calculator.
-    parallel_info
-        Dictionary of parallelization information.
     additional_fields
         Any additional fields to supply to the summarizer.
     copy_files
         Files to copy (and decompress) from source to the runtime directory.
 
     Returns
     -------
@@ -80,15 +77,14 @@
     atoms = prepare_atoms(
         atoms=atoms,
         preset=preset,
         template=template,
         profile=profile,
         calc_defaults=calc_defaults,
         calc_swaps=calc_swaps,
-        parallel_info=parallel_info,
     )
 
     updated_copy_files = prepare_copy(
         copy_files=copy_files,
         calc_params=atoms.calc.user_calc_params,
         binary=atoms.calc.template.binary,
     )
@@ -107,15 +103,14 @@
     preset: str | None = None,
     template: EspressoTemplate | None = None,
     profile: EspressoProfile | None = None,
     calc_defaults: dict[str, Any] | None = None,
     calc_swaps: dict[str, Any] | None = None,
     opt_defaults: dict[str, Any] | None = None,
     opt_params: OptParams | None = None,
-    parallel_info: dict[str, Any] | None = None,
     additional_fields: dict[str, Any] | None = None,
     copy_files: (
         SourceDirectory
         | list[SourceDirectory]
         | dict[SourceDirectory, Filenames]
         | None
     ) = None,
@@ -141,16 +136,14 @@
         keys, refer to the [ase.calculators.espresso.Espresso][] calculator.
     opt_defaults
         The default optimization parameters.
     opt_params
         Dictionary of parameters to pass to the optimizer. pass "optimizer"
         to change the optimizer being used. "fmax" and "max_steps" are commonly
         used keywords. See the ASE documentation for more information.
-    parallel_info
-        Dictionary of parallelization information.
     additional_fields
         Any additional fields to supply to the summarizer.
     copy_files
         Files to copy (and decompress) from source to the runtime directory.
 
     Returns
     -------
@@ -160,15 +153,14 @@
     atoms = prepare_atoms(
         atoms=atoms,
         preset=preset,
         template=template,
         profile=profile,
         calc_defaults=calc_defaults,
         calc_swaps=calc_swaps,
-        parallel_info=parallel_info,
     )
 
     updated_copy_files = prepare_copy(
         copy_files=copy_files,
         calc_params=atoms.calc.user_calc_params,
         binary=atoms.calc.template.binary,
     )
@@ -185,15 +177,14 @@
 def prepare_atoms(
     atoms: Atoms | None = None,
     preset: str | None = None,
     template: EspressoTemplate | None = None,
     profile: EspressoProfile | None = None,
     calc_defaults: dict[str, Any] | None = None,
     calc_swaps: dict[str, Any] | None = None,
-    parallel_info: dict[str, Any] | None = None,
 ) -> Atoms:
     """
     Commonly used preparation function to merge parameters
     and attach an Espresso calculator accordingly.
 
     Parameters
     ----------
@@ -207,16 +198,14 @@
         EspressoProfile to use
     calc_defaults
         The default calculator parameters.
     calc_swaps
         Custom kwargs for the espresso calculator. Set a value to
         `quacc.Remove` to remove a pre-existing key entirely. For a list of available
         keys, refer to the [ase.calculators.espresso.Espresso][] calculator.
-    parallel_info
-        Dictionary of parallelization information.
 
     Returns
     -------
     Atoms
         Atoms object with attached Espresso calculator.
     """
     atoms = Atoms() if atoms is None else atoms
@@ -235,15 +224,14 @@
     calc_defaults = remove_conflicting_kpts_kspacing(calc_defaults, calc_swaps)
 
     calc_flags = recursive_dict_merge(calc_defaults, calc_swaps)
 
     atoms.calc = Espresso(
         input_atoms=atoms,
         preset=preset,
-        parallel_info=parallel_info,
         template=template,
         profile=profile,
         **calc_flags,
     )
 
     return atoms
```

### Comparing `quacc-0.9.0/src/quacc/recipes/espresso/bands.py` & `quacc-0.9.1/src/quacc/recipes/espresso/bands.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,15 +40,14 @@
         | dict[SourceDirectory, Filenames]
         | None
     ) = None,
     prev_outdir: SourceDirectory | None = None,
     make_bandpath: bool = True,
     line_density: float = 20,
     force_gamma: bool = True,
-    parallel_info: dict[str] | None = None,
     test_run: bool = False,
     **calc_kwargs,
 ) -> RunSchema:
     """
     Function to carry out a basic bands structure calculation with pw.x.
 
     First perform a normal SCF calculation [quacc.recipes.espresso.core.static_job][];
@@ -76,17 +75,14 @@
         [pymatgen.symmetry.bandstructure.HighSymmKpath][]
     line_density
         Density of kpoints along the band path if make_bandpath is True
         For more information [quacc.utils.kpts.convert_pmg_kpts][]
     force_gamma
         Forces gamma-centered k-points when using make_bandpath
         For more information [quacc.utils.kpts.convert_pmg_kpts][]
-    parallel_info
-        Dictionary containing information about the parallelization of the
-        calculation. See the ASE documentation for more information.
     test_run
         If True, a test run is performed to check that the calculation input_data is correct or
         to generate some files/info if needed.
     **calc_kwargs
         Additional keyword arguments to pass to the Espresso calculator. Set a value to
         `quacc.Remove` to remove a pre-existing key entirely. See the docstring of
         [quacc.calculators.espresso.espresso.Espresso][] for more information.
@@ -112,30 +108,28 @@
         )
 
     return run_and_summarize(
         atoms,
         template=EspressoTemplate("pw", test_run=test_run, outdir=prev_outdir),
         calc_defaults=calc_defaults,
         calc_swaps=calc_kwargs,
-        parallel_info=parallel_info,
         additional_fields={"name": "pw.x bands"},
         copy_files=copy_files,
     )
 
 
 @job
 def bands_pp_job(
     copy_files: (
         SourceDirectory
         | list[SourceDirectory]
         | dict[SourceDirectory, Filenames]
         | None
     ) = None,
     prev_outdir: SourceDirectory | None = None,
-    parallel_info: dict[str] | None = None,
     test_run: bool = False,
     **calc_kwargs,
 ) -> RunSchema:
     """
     Function to re-order bands and computes bands-related properties with bands.x.
     This allows to get the bands structure in a more readable way. This requires a
     previous [quacc.recipes.espresso.bands.bands_pw_job][] calculation.
@@ -148,17 +142,14 @@
         which files have to be copied over by looking at the binary and `input_data`.
         If a dict is provided, the mode is manual, keys are source directories and values
         are relative path to files or directories to copy. Glob patterns are supported.
     prev_outdir
         The output directory of a previous calculation. If provided, Quantum Espresso
         will directly read the necessary files from this directory, eliminating the need
         to manually copy files. The directory will be ungzipped if necessary.
-    parallel_info
-        Dictionary containing information about the parallelization of the
-        calculation. See the ASE documentation for more information.
     test_run
         If True, a test run is performed to check that the calculation input_data is correct or
         to generate some files/info if needed.
     **calc_kwargs
         Additional keyword arguments to pass to the Espresso calculator. Set a value to
         `quacc.Remove` to remove a pre-existing key entirely. See the docstring of
         [quacc.calculators.espresso.espresso.Espresso][] for more information.
@@ -169,30 +160,28 @@
         Dictionary of results from [quacc.schemas.ase.summarize_run][].
         See the type-hint for the data structure.
     """
     return run_and_summarize(
         template=EspressoTemplate("bands", test_run=test_run, outdir=prev_outdir),
         calc_defaults={},
         calc_swaps=calc_kwargs,
-        parallel_info=parallel_info,
         additional_fields={"name": "bands.x post-processing"},
         copy_files=copy_files,
     )
 
 
 @job
 def fermi_surface_job(
     copy_files: (
         SourceDirectory
         | list[SourceDirectory]
         | dict[SourceDirectory, Filenames]
         | None
     ) = None,
     prev_outdir: SourceDirectory | None = None,
-    parallel_info: dict[str] | None = None,
     test_run: bool = False,
     **calc_kwargs,
 ) -> RunSchema:
     """
     Function to retrieve the fermi surface with fs.x
     It requires a previous uniform unshifted k-point grid bands calculation.
 
@@ -204,17 +193,14 @@
         which files have to be copied over by looking at the binary and `input_data`.
         If a dict is provided, the mode is manual, keys are source directories and values
         are relative path to files or directories to copy. Glob patterns are supported.
     prev_outdir
         The output directory of a previous calculation. If provided, Quantum Espresso
         will directly read the necessary files from this directory, eliminating the need
         to manually copy files. The directory will be ungzipped if necessary.
-    parallel_info
-        Dictionary containing information about the parallelization of the
-        calculation. See the ASE documentation for more information.
     test_run
         If True, a test run is performed to check that the calculation input_data is correct or
         to generate some files/info if needed.
     **calc_kwargs
         Additional keyword arguments to pass to the Espresso calculator. Set a value to
         `quacc.Remove` to remove a pre-existing key entirely. See the docstring of
         [quacc.calculators.espresso.espresso.Espresso][] for more information.
@@ -225,15 +211,14 @@
         Dictionary of results from [quacc.schemas.ase.summarize_run][].
         See the type-hint for the data structure.
     """
     return run_and_summarize(
         template=EspressoTemplate("fs", test_run=test_run, outdir=prev_outdir),
         calc_defaults={},
         calc_swaps=calc_kwargs,
-        parallel_info=parallel_info,
         additional_fields={"name": "fs.x fermi_surface"},
         copy_files=copy_files,
     )
 
 
 @flow
 def bands_flow(
@@ -242,15 +227,14 @@
         SourceDirectory | list[SourceDirectory] | dict[SourceDirectory, Filenames]
     ),
     run_bands_pp: bool = True,
     run_fermi_surface: bool = False,
     make_bandpath: bool = True,
     line_density: float = 20,
     force_gamma: bool = True,
-    parallel_info: dict[str] | None = None,
     job_params: dict[str, Any] | None = None,
     job_decorators: dict[str, Callable | None] | None = None,
 ) -> BandsSchema:
     """
     Function to compute bands structure and fermi surface using pw.x, bands.x and fs.x.
 
     Consists of the following steps:
@@ -287,17 +271,14 @@
         [pymatgen.symmetry.bandstructure.HighSymmKpath][]
     line_density
         Density of kpoints along the band path if make_bandpath is True
         For more information [quacc.utils.kpts.convert_pmg_kpts][]
     force_gamma
         Forces gamma-centered k-points when using make_bandpath
         For more information [quacc.utils.kpts.convert_pmg_kpts][]
-    parallel_info
-        Dictionary containing information about the parallelization of the
-        calculation. See the ASE documentation for more information.
     job_params
         Custom parameters to pass to each Job in the Flow. This is a dictionary where
         the keys are the names of the jobs and the values are dictionaries of parameters.
     job_decorators
         Custom decorators to apply to each Job in the Flow. This is a dictionary where
         the keys are the names of the jobs and the values are decorators.
 
@@ -316,24 +297,19 @@
 
     bands_results = bands_pw_job_(
         atoms,
         copy_files,
         make_bandpath=make_bandpath,
         line_density=line_density,
         force_gamma=force_gamma,
-        parallel_info=parallel_info,
     )
     results = {"bands_pw": bands_results}
 
     if run_bands_pp:
-        bands_pp_results = bands_pp_job_(
-            prev_outdir=bands_results["dir_name"], parallel_info=parallel_info
-        )
+        bands_pp_results = bands_pp_job_(prev_outdir=bands_results["dir_name"])
         results["bands_pp"] = bands_pp_results
 
     if run_fermi_surface:
-        fermi_results = fermi_surface_job_(
-            prev_outdir=bands_results["dir_name"], parallel_info=parallel_info
-        )
+        fermi_results = fermi_surface_job_(prev_outdir=bands_results["dir_name"])
         results["fermi_surface"] = fermi_results
 
     return results
```

### Comparing `quacc-0.9.0/src/quacc/recipes/espresso/core.py` & `quacc-0.9.1/src/quacc/recipes/espresso/core.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,15 +35,14 @@
 }
 
 
 @job
 def static_job(
     atoms: Atoms,
     preset: str | None = "sssp_1.3.0_pbe_efficiency",
-    parallel_info: dict[str] | None = None,
     test_run: bool = False,
     copy_files: (
         SourceDirectory
         | list[SourceDirectory]
         | dict[SourceDirectory, Filenames]
         | None
     ) = None,
@@ -57,17 +56,14 @@
     ----------
     atoms
         The Atoms object.
     preset
         The name of a YAML file containing a list of parameters to use as
         a "preset" for the calculator. quacc will automatically look in the
         `ESPRESSO_PRESET_DIR` (default: quacc/calculators/espresso/presets).
-    parallel_info
-        Dictionary containing information about the parallelization of the
-        calculation. See the ASE documentation for more information.
     test_run
         If True, a test run is performed to check that the calculation input_data is correct or
         to generate some files/info if needed.
     copy_files
         Source directory or directories to copy files from. If a `SourceDirectory` or a
         list of `SourceDirectory` is provided, this interface will automatically guess
         which files have to be copied over by looking at the binary and `input_data`.
@@ -95,26 +91,24 @@
 
     return run_and_summarize(
         atoms,
         preset=preset,
         template=EspressoTemplate("pw", test_run=test_run, outdir=prev_outdir),
         calc_defaults=calc_defaults,
         calc_swaps=calc_kwargs,
-        parallel_info=parallel_info,
         additional_fields={"name": "pw.x Static"},
         copy_files=copy_files,
     )
 
 
 @job
 def relax_job(
     atoms: Atoms,
     preset: str | None = "sssp_1.3.0_pbe_efficiency",
     relax_cell: bool = False,
-    parallel_info: dict[str] | None = None,
     test_run: bool = False,
     copy_files: (
         SourceDirectory
         | list[SourceDirectory]
         | dict[SourceDirectory, Filenames]
         | None
     ) = None,
@@ -130,17 +124,14 @@
         The Atoms object.
     preset
         The name of a YAML file containing a list of parameters to use as
         a "preset" for the calculator. quacc will automatically look in the
         `ESPRESSO_PRESET_DIR` (default: quacc/calculators/espresso/presets).
     relax_cell
         Whether to relax the cell or not.
-    parallel_info
-        Dictionary containing information about the parallelization of the
-        calculation. See the ASE documentation for more information.
     test_run
         If True, a test run is performed to check that the calculation input_data is correct or
         to generate some files/info if needed.
     copy_files
         Source directory or directories to copy files from. If a `SourceDirectory` or a
         list of `SourceDirectory` is provided, this interface will automatically guess
         which files have to be copied over by looking at the binary and `input_data`.
@@ -170,27 +161,25 @@
 
     return run_and_summarize(
         atoms,
         preset=preset,
         template=EspressoTemplate("pw", test_run=test_run, outdir=prev_outdir),
         calc_defaults=calc_defaults,
         calc_swaps=calc_kwargs,
-        parallel_info=parallel_info,
         additional_fields={"name": "pw.x Relax"},
         copy_files=copy_files,
     )
 
 
 @job
 def ase_relax_job(
     atoms: Atoms,
     preset: str | None = "sssp_1.3.0_pbe_efficiency",
     autorestart: bool = True,
     relax_cell: bool = False,
-    parallel_info: dict[str] | None = None,
     opt_params: OptParams | None = None,
     copy_files: (
         SourceDirectory
         | list[SourceDirectory]
         | dict[SourceDirectory, Filenames]
         | None
     ) = None,
@@ -211,17 +200,14 @@
         `ESPRESSO_PRESET_DIR` (default: quacc/calculators/espresso/presets).
     autorestart
         Whether to automatically turn on the restart flag after the first
         calculation. This avoids recomputing everything from scratch at each
         step of the optimization.
     relax_cell
         Whether to relax the cell or not.
-    parallel_info
-        Dictionary containing information about the parallelization of the
-        calculation. See the ASE documentation for more information.
     opt_params
         Dictionary of custom kwargs for the optimization process. For a list
         of available keys, refer to [quacc.runners.ase.run_opt][].
     copy_files
         Source directory or directories to copy files from. If a `SourceDirectory` or a
         list of `SourceDirectory` is provided, this interface will automatically guess
         which files have to be copied over by looking at the binary and `input_data`.
@@ -257,30 +243,28 @@
         atoms,
         preset=preset,
         template=EspressoTemplate("pw", autorestart=autorestart, outdir=prev_outdir),
         calc_defaults=calc_defaults,
         calc_swaps=calc_kwargs,
         opt_defaults=opt_defaults,
         opt_params=opt_params,
-        parallel_info=parallel_info,
         additional_fields={"name": "pw.x ExternalRelax"},
         copy_files=copy_files,
     )
 
 
 @job
 def post_processing_job(
     copy_files: (
         SourceDirectory
         | list[SourceDirectory]
         | dict[SourceDirectory, Filenames]
         | None
     ) = None,
     prev_outdir: SourceDirectory | None = None,
-    parallel_info: dict[str] | None = None,
     test_run: bool = False,
     **calc_kwargs,
 ) -> RunSchema:
     """
     Function to carry out a basic pp.x calculation (post-processing).
     It is mainly used to extract the charge density from a previous pw.x calculation.
     and perform simple to complex post-processing on it. Fore more details please see
@@ -294,17 +278,14 @@
         which files have to be copied over by looking at the binary and `input_data`.
         If a dict is provided, the mode is manual, keys are source directories and values
         are relative path to files or directories to copy. Glob patterns are supported.
     prev_outdir
         The output directory of a previous calculation. If provided, Quantum Espresso
         will directly read the necessary files from this directory, eliminating the need
         to manually copy files. The directory will be ungzipped if necessary.
-    parallel_info
-        Dictionary containing information about the parallelization of the
-        calculation. See the ASE documentation for more information.
     **calc_kwargs
         Additional keyword arguments to pass to the Espresso calculator. Set a value to
         `quacc.Remove` to remove a pre-existing key entirely. See the docstring of
         [quacc.calculators.espresso.espresso.Espresso][] for more information.
 
     Returns
     -------
@@ -323,15 +304,14 @@
         }
     }
 
     return run_and_summarize(
         template=EspressoTemplate("pp", test_run=test_run, outdir=prev_outdir),
         calc_defaults=calc_defaults,
         calc_swaps=calc_kwargs,
-        parallel_info=parallel_info,
         additional_fields={"name": "pp.x post-processing"},
         copy_files=copy_files,
     )
 
 
 @job
 def non_scf_job(
@@ -340,15 +320,14 @@
         SourceDirectory
         | list[SourceDirectory]
         | dict[SourceDirectory, Filenames]
         | None
     ) = None,
     prev_outdir: SourceDirectory | None = None,
     preset: str | None = "sssp_1.3.0_pbe_efficiency",
-    parallel_info: dict[str] | None = None,
     test_run: bool = False,
     **calc_kwargs,
 ) -> RunSchema:
     """
     Function to carry out a basic NSCF calculation with pw.x.
 
     Parameters
@@ -365,17 +344,14 @@
         The output directory of a previous calculation. If provided, Quantum Espresso
         will directly read the necessary files from this directory, eliminating the need
         to manually copy files. The directory will be ungzipped if necessary.
     preset
         The name of a YAML file containing a list of parameters to use as
         a "preset" for the calculator. quacc will automatically look in the
         `ESPRESSO_PRESET_DIR` (default: quacc/calculators/espresso/presets).
-    parallel_info
-        Dictionary containing information about the parallelization of the
-        calculation. See the ASE documentation for more information.
     test_run
         If True, a test run is performed to check that the calculation input_data is correct or
         to generate some files/info if needed.
     **calc_kwargs
         Additional keyword arguments to pass to the Espresso calculator. Set a value to
         `quacc.Remove` to remove a pre-existing key entirely. See the docstring of
         [quacc.calculators.espresso.espresso.Espresso][] for more information.
@@ -390,11 +366,10 @@
 
     return run_and_summarize(
         atoms,
         preset=preset,
         template=EspressoTemplate("pw", test_run=test_run, outdir=prev_outdir),
         calc_defaults=calc_defaults,
         calc_swaps=calc_kwargs,
-        parallel_info=parallel_info,
         additional_fields={"name": "pw.x Non SCF"},
         copy_files=copy_files,
     )
```

### Comparing `quacc-0.9.0/src/quacc/recipes/espresso/dos.py` & `quacc-0.9.1/src/quacc/recipes/espresso/dos.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,15 +34,14 @@
     copy_files: (
         SourceDirectory
         | list[SourceDirectory]
         | dict[SourceDirectory, Filenames]
         | None
     ) = None,
     prev_outdir: SourceDirectory | None = None,
-    parallel_info: dict[str] | None = None,
     test_run: bool = False,
     **calc_kwargs,
 ) -> RunSchema:
     """
     Function to carry out a basic dos.x calculation (density of states).
     It is mainly used to extract the charge density and wavefunction from a previous pw.x calculation.
     It generates the total density of states. For more details, please see
@@ -56,17 +55,14 @@
         which files have to be copied over by looking at the binary and `input_data`.
         If a dict is provided, the mode is manual, keys are source directories and values
         are relative path to files or directories to copy. Glob patterns are supported.
     prev_outdir
         The output directory of a previous calculation. If provided, Quantum Espresso
         will directly read the necessary files from this directory, eliminating the need
         to manually copy files. The directory will be ungzipped if necessary.
-    parallel_info
-        Dictionary containing information about the parallelization of the
-        calculation. See the ASE documentation for more information.
     **calc_kwargs
         Additional keyword arguments to pass to the Espresso calculator. Set a value to
         `quacc.Remove` to remove a pre-existing key entirely. See the docstring of
         `ase.io.espresso.write_fortran_namelist` for more information.
 
     Returns
     -------
@@ -74,30 +70,28 @@
         Dictionary of results from [quacc.schemas.ase.summarize_run][].
         See the type-hint for the data structure.
     """
     return run_and_summarize(
         template=EspressoTemplate("dos", test_run=test_run, outdir=prev_outdir),
         calc_defaults=None,
         calc_swaps=calc_kwargs,
-        parallel_info=parallel_info,
         additional_fields={"name": "dos.x Density-of-States"},
         copy_files=copy_files,
     )
 
 
 @job
 def projwfc_job(
     copy_files: (
         SourceDirectory
         | list[SourceDirectory]
         | dict[SourceDirectory, Filenames]
         | None
     ) = None,
     prev_outdir: SourceDirectory | None = None,
-    parallel_info: dict[str] | None = None,
     test_run: bool = False,
     **calc_kwargs,
 ) -> RunSchema:
     """
     Function to carry out a basic projwfc.x calculation.
     It is mainly used to extract the charge density and wavefunction from a previous pw.x calculation.
     It can generate partial dos, local dos, spilling parameter and more. Fore more details please see
@@ -111,17 +105,14 @@
         which files have to be copied over by looking at the binary and `input_data`.
         If a dict is provided, the mode is manual, keys are source directories and values
         are relative path to files or directories to copy. Glob patterns are supported.
     prev_outdir
         The output directory of a previous calculation. If provided, Quantum Espresso
         will directly read the necessary files from this directory, eliminating the need
         to manually copy files. The directory will be ungzipped if necessary.
-    parallel_info
-        Dictionary containing information about the parallelization of the
-        calculation. See the ASE documentation for more information.
     **calc_kwargs
         Additional keyword arguments to pass to the Espresso calculator. Set a value to
         `quacc.Remove` to remove a pre-existing key entirely. See the docstring of
         `ase.io.espresso.write_fortran_namelist` for more information.
 
     Returns
     -------
@@ -129,15 +120,14 @@
         Dictionary of results from [quacc.schemas.ase.summarize_run][].
         See the type-hint for the data structure.
     """
     return run_and_summarize(
         template=EspressoTemplate("projwfc", test_run=test_run, outdir=prev_outdir),
         calc_defaults=None,
         calc_swaps=calc_kwargs,
-        parallel_info=parallel_info,
         additional_fields={"name": "projwfc.x Projects-wavefunctions"},
         copy_files=copy_files,
     )
 
 
 @flow
 def dos_flow(
```

### Comparing `quacc-0.9.0/src/quacc/recipes/espresso/phonons.py` & `quacc-0.9.1/src/quacc/recipes/espresso/phonons.py`

 * *Files 10% similar despite different names*

```diff
@@ -42,15 +42,14 @@
     copy_files: (
         SourceDirectory
         | list[SourceDirectory]
         | dict[SourceDirectory, Filenames]
         | None
     ) = None,
     prev_outdir: SourceDirectory | None = None,
-    parallel_info: dict[str] | None = None,
     test_run: bool = False,
     use_phcg: bool = False,
     **calc_kwargs,
 ) -> RunSchema:
     """
     Function to carry out a basic ph.x calculation. It should allow you to
     use all the features of the [ph.x binary](https://www.quantum-espresso.org/Doc/INPUT_PH.html)
@@ -67,17 +66,14 @@
         which files have to be copied over by looking at the binary and `input_data`.
         If a dict is provided, the mode is manual, keys are source directories and values
         are relative path to files or directories to copy. Glob patterns are supported.
     prev_outdir
         The output directory of a previous calculation. If provided, Quantum Espresso
         will directly read the necessary files from this directory, eliminating the need
         to manually copy files. The directory will be ungzipped if necessary.
-    parallel_info
-        Dictionary containing information about the parallelization of the
-        calculation. See the ASE documentation for more information.
     test_run
         If True, a test run is performed to check that the calculation input_data is correct or
         to generate some files/info if needed.
     use_phcg
         If True, the calculation is performed using the `phcg.x` code which uses a faster algorithm.
         It can be used only if you sample the Brillouin Zone at Gamma and you only need the phonon
         modes at Gamma (molecules typically). It cannot be used with spin-polarization, USPP and PAW.
@@ -101,29 +97,27 @@
 
     binary = "phcg" if use_phcg else "ph"
 
     return run_and_summarize(
         template=EspressoTemplate(binary, test_run=test_run, outdir=prev_outdir),
         calc_defaults=calc_defaults,
         calc_swaps=calc_kwargs,
-        parallel_info=parallel_info,
         additional_fields={"name": f"{binary}.x Phonon"},
         copy_files=copy_files,
     )
 
 
 @job
 def q2r_job(
     copy_files: (
         SourceDirectory
         | list[SourceDirectory]
         | dict[SourceDirectory, Filenames]
         | None
     ) = None,
-    parallel_info: dict[str] | None = None,
     **calc_kwargs,
 ) -> RunSchema:
     """
     Function to carry out a basic q2r.x calculation. It should allow you to
     use all the features of the [q2r.x binary](https://www.quantum-espresso.org/Doc/INPUT_Q2R.html#idm51)
 
     `q2r.x` reads force constant matrices C(q) produced by the `ph.x` code
@@ -134,17 +128,14 @@
     ----------
     copy_files
         Source directory or directories to copy files from. If a `SourceDirectory` or a
         list of `SourceDirectory` is provided, this interface will automatically guess
         which files have to be copied over by looking at the binary and `input_data`.
         If a dict is provided, the mode is manual, keys are source directories and values
         are relative path to files or directories to copy. Glob patterns are supported.
-    parallel_info
-        Dictionary containing information about the parallelization of the
-        calculation. See the ASE documentation for more information.
     **calc_kwargs
         Additional keyword arguments to pass to the Espresso calculator. Set a value to
         `quacc.Remove` to remove a pre-existing key entirely. See the docstring of
         [quacc.calculators.espresso.espresso.Espresso][] for more information.
 
     Returns
     -------
@@ -152,29 +143,27 @@
         Dictionary of results from [quacc.schemas.ase.summarize_run][].
         See the type-hint for the data structure.
     """
     return run_and_summarize(
         template=EspressoTemplate("q2r"),
         calc_defaults={},
         calc_swaps=calc_kwargs,
-        parallel_info=parallel_info,
         additional_fields={"name": "q2r.x Phonon"},
         copy_files=copy_files,
     )
 
 
 @job
 def matdyn_job(
     copy_files: (
         SourceDirectory
         | list[SourceDirectory]
         | dict[SourceDirectory, Filenames]
         | None
     ) = None,
-    parallel_info: dict[str] | None = None,
     **calc_kwargs,
 ) -> RunSchema:
     """
     Function to carry out a basic `matdyn.x` calculation. It should allow you to use
     all the features of the [matdyn.x binary](https://www.quantum-espresso.org/Doc/INPUT_MATDYN.html#idm138)
 
     This program calculates the phonon frequencies for a list of generic
@@ -186,17 +175,14 @@
     ----------
     copy_files
         Source directory or directories to copy files from. If a `SourceDirectory` or a
         list of `SourceDirectory` is provided, this interface will automatically guess
         which files have to be copied over by looking at the binary and `input_data`.
         If a dict is provided, the mode is manual, keys are source directories and values
         are relative path to files or directories to copy. Glob patterns are supported.
-    parallel_info
-        Dictionary containing information about the parallelization of the
-        calculation. See the ASE documentation for more information.
     **calc_kwargs
         Additional keyword arguments to pass to the Espresso calculator. Set a value to
         `quacc.Remove` to remove a pre-existing key entirely. See the docstring of
         [quacc.calculators.espresso.espresso.Espresso][] for more information.
 
     Returns
     -------
@@ -204,15 +190,14 @@
         Dictionary of results from [quacc.schemas.ase.summarize_run][].
         See the type-hint for the data structure.
     """
     return run_and_summarize(
         template=EspressoTemplate("matdyn"),
         calc_defaults={},
         calc_swaps=calc_kwargs,
-        parallel_info=parallel_info,
         additional_fields={"name": "matdyn Phonon"},
         copy_files=copy_files,
     )
 
 
 @flow
 def phonon_dos_flow(
@@ -482,15 +467,14 @@
     copy_files: (
         SourceDirectory
         | list[SourceDirectory]
         | dict[SourceDirectory, Filenames]
         | None
     ) = None,
     prev_outdir: SourceDirectory | None = None,
-    parallel_info: dict[str] | None = None,
     **calc_kwargs,
 ) -> RunSchema:
     """
     Function to carry out a basic dvscf_q2r calculation allowing phonon potential
     interpolation from coarse to fine q-point grids using Fourier interpolation.
     It should allow you to use all the features of the dvscf_q2r binary which does
     not have an official documentation.
@@ -528,17 +512,14 @@
         which files have to be copied over by looking at the binary and `input_data`.
         If a dict is provided, the mode is manual, keys are source directories and values
         are relative path to files or directories to copy. Glob patterns are supported.
     prev_outdir
         The output directory of a previous calculation. If provided, Quantum Espresso
         will directly read the necessary files from this directory, eliminating the need
         to manually copy files. The directory will be ungzipped if necessary.
-    parallel_info
-        Dictionary containing information about the parallelization of the
-        calculation. See the ASE documentation for more information.
     **calc_kwargs
         Additional keyword arguments to pass to the Espresso calculator. Set a value to
         `quacc.Remove` to remove a pre-existing key entirely. See the docstring of
         [quacc.calculators.espresso.espresso.Espresso][] for more information.
 
     Returns
     -------
@@ -546,30 +527,28 @@
         Dictionary of results from [quacc.schemas.ase.summarize_run][].
         See the type-hint for the data structure.
     """
     return run_and_summarize(
         template=EspressoTemplate("dvscf_q2r", outdir=prev_outdir),
         calc_defaults={},
         calc_swaps=calc_kwargs,
-        parallel_info=parallel_info,
         additional_fields={"name": "dvscf_q2r Phonon"},
         copy_files=copy_files,
     )
 
 
 @job
 def postahc_job(
     copy_files: (
         SourceDirectory
         | list[SourceDirectory]
         | dict[SourceDirectory, Filenames]
         | None
     ) = None,
     prev_outdir: SourceDirectory | None = None,
-    parallel_info: dict[str] | None = None,
     **calc_kwargs,
 ) -> RunSchema:
     """
     Function to carry out a basic postahc calculation. It should allow you to
     use all the features of the [postahc.x binary](https://www.quantum-espresso.org/Doc/INPUT_POSTAHC.html#idm11)
 
     Calculate the phonon-induced electron self-energy in the full matrix form
@@ -592,17 +571,14 @@
         which files have to be copied over by looking at the binary and `input_data`.
         If a dict is provided, the mode is manual, keys are source directories and values
         are relative path to files or directories to copy. Glob patterns are supported.
     prev_outdir
         The output directory of a previous calculation. If provided, Quantum Espresso
         will directly read the necessary files from this directory, eliminating the need
         to manually copy files. The directory will be ungzipped if necessary.
-    parallel_info
-        Dictionary containing information about the parallelization of the
-        calculation. See the ASE documentation for more information.
     **calc_kwargs
         Additional keyword arguments to pass to the Espresso calculator. Set a value to
         `quacc.Remove` to remove a pre-existing key entirely. See the docstring of
         [quacc.calculators.espresso.espresso.Espresso][] for more information.
 
     Returns
     -------
@@ -610,11 +586,10 @@
         Dictionary of results from [quacc.schemas.ase.summarize_run][].
         See the type-hint for the data structure.
     """
     return run_and_summarize(
         template=EspressoTemplate("postahc", outdir=prev_outdir),
         calc_defaults={},
         calc_swaps=calc_kwargs,
-        parallel_info=parallel_info,
         additional_fields={"name": "postahc Phonon"},
         copy_files=copy_files,
     )
```

### Comparing `quacc-0.9.0/src/quacc/recipes/gaussian/_base.py` & `quacc-0.9.1/src/quacc/recipes/gaussian/_base.py`

 * *Files identical despite different names*

### Comparing `quacc-0.9.0/src/quacc/recipes/gaussian/core.py` & `quacc-0.9.1/src/quacc/recipes/gaussian/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.9.0/src/quacc/recipes/gulp/_base.py` & `quacc-0.9.1/src/quacc/recipes/gulp/_base.py`

 * *Files identical despite different names*

### Comparing `quacc-0.9.0/src/quacc/recipes/gulp/core.py` & `quacc-0.9.1/src/quacc/recipes/gulp/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.9.0/src/quacc/recipes/lj/core.py` & `quacc-0.9.1/src/quacc/recipes/lj/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.9.0/src/quacc/recipes/mlp/_base.py` & `quacc-0.9.1/src/quacc/recipes/mlp/_base.py`

 * *Files identical despite different names*

### Comparing `quacc-0.9.0/src/quacc/recipes/mlp/core.py` & `quacc-0.9.1/src/quacc/recipes/mlp/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.9.0/src/quacc/recipes/mlp/phonons.py` & `quacc-0.9.1/src/quacc/recipes/mlp/phonons.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,28 +8,31 @@
 from monty.dev import requires
 
 from quacc import flow
 from quacc.recipes.common.phonons import phonon_subflow
 from quacc.recipes.mlp.core import relax_job, static_job
 from quacc.wflow_tools.customizers import customize_funcs
 
-has_deps = find_spec("phonopy") is not None and find_spec("seekpath") is not None
+has_phonopy = bool(find_spec("phonopy"))
+has_seekpath = bool(find_spec("seekpath"))
 
 if TYPE_CHECKING:
     from typing import Any, Callable, Literal
 
     from ase.atoms import Atoms
 
     from quacc.schemas._aliases.phonons import PhononSchema
 
 
 @flow
 @requires(
-    has_deps,
-    message="Phonopy and seekpath must be installed. Run `pip install quacc[phonons]`",
+    has_phonopy, message="Phonopy must be installed. Run `pip install quacc[phonons]`"
+)
+@requires(
+    has_seekpath, message="Seekpath must be installed. Run `pip install quacc[phonons]`"
 )
 def phonon_flow(
     atoms: Atoms,
     method: Literal["mace-mp-0", "m3gnet", "chgnet"],
     symprec: float = 1e-4,
     min_lengths: float | tuple[float, float, float] | None = 20.0,
     supercell_matrix: (
```

### Comparing `quacc-0.9.0/src/quacc/recipes/newtonnet/core.py` & `quacc-0.9.1/src/quacc/recipes/newtonnet/core.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 """Core recipes for the NewtonNet code."""
 
 from __future__ import annotations
 
+from importlib.util import find_spec
 from typing import TYPE_CHECKING
 
 from ase.vibrations.data import VibrationsData
 from monty.dev import requires
 
 from quacc import SETTINGS, job
 from quacc.runners.ase import run_calc, run_opt
 from quacc.runners.thermo import run_ideal_gas
 from quacc.schemas.ase import summarize_opt_run, summarize_run, summarize_vib_and_thermo
 from quacc.utils.dicts import recursive_dict_merge
 
-try:
-    from sella import Sella
-except ImportError:
-    Sella = None
+has_sella = bool(find_spec("sella"))
+has_newtonnet = bool(find_spec("newtonnet"))
 
-try:
+if has_sella:
+    from sella import Sella
+if has_newtonnet:
     from newtonnet.utils.ase_interface import MLAseCalculator as NewtonNet
-except ImportError:
-    NewtonNet = None
 
 if TYPE_CHECKING:
     from typing import Any
 
     from ase.atoms import Atoms
 
     from quacc.runners.ase import OptParams
     from quacc.schemas._aliases.ase import OptSchema, RunSchema, VibThermoSchema
     from quacc.utils.files import Filenames, SourceDirectory
 
 
 @job
-@requires(NewtonNet, "NewtonNet must be installed. Refer to the quacc documentation.")
+@requires(
+    has_newtonnet, "NewtonNet must be installed. Refer to the quacc documentation."
+)
 def static_job(
     atoms: Atoms,
     copy_files: SourceDirectory | dict[SourceDirectory, Filenames] | None = None,
     **calc_kwargs,
 ) -> RunSchema:
     """
     Carry out a single-point calculation.
@@ -71,15 +72,17 @@
 
     return summarize_run(
         final_atoms, atoms, additional_fields={"name": "NewtonNet Static"}
     )
 
 
 @job
-@requires(NewtonNet, "NewtonNet must be installed. Refer to the quacc documentation.")
+@requires(
+    has_newtonnet, "NewtonNet must be installed. Refer to the quacc documentation."
+)
 def relax_job(
     atoms: Atoms,
     opt_params: OptParams | None = None,
     copy_files: SourceDirectory | dict[SourceDirectory, Filenames] | None = None,
     **calc_kwargs,
 ) -> OptSchema:
     """
@@ -105,29 +108,31 @@
         Dictionary of results, specified in [quacc.schemas.ase.summarize_opt_run][].
         See the type-hint for the data structure.
     """
     calc_defaults = {
         "model_path": SETTINGS.NEWTONNET_MODEL_PATH,
         "settings_path": SETTINGS.NEWTONNET_CONFIG_PATH,
     }
-    opt_defaults = {"optimizer": Sella} if Sella else {}
+    opt_defaults = {"optimizer": Sella} if has_sella else {}
 
     calc_flags = recursive_dict_merge(calc_defaults, calc_kwargs)
     opt_flags = recursive_dict_merge(opt_defaults, opt_params)
 
     atoms.calc = NewtonNet(**calc_flags)
     dyn = run_opt(atoms, copy_files=copy_files, **opt_flags)
 
     return _add_stdev_and_hess(
         summarize_opt_run(dyn, additional_fields={"name": "NewtonNet Relax"})
     )
 
 
 @job
-@requires(NewtonNet, "NewtonNet must be installed. Refer to the quacc documentation.")
+@requires(
+    has_newtonnet, "NewtonNet must be installed. Refer to the quacc documentation."
+)
 def freq_job(
     atoms: Atoms,
     temperature: float = 298.15,
     pressure: float = 1.0,
     copy_files: SourceDirectory | dict[SourceDirectory, Filenames] | None = None,
     **calc_kwargs,
 ) -> VibThermoSchema:
@@ -157,27 +162,25 @@
     calc_defaults = {
         "model_path": SETTINGS.NEWTONNET_MODEL_PATH,
         "settings_path": SETTINGS.NEWTONNET_CONFIG_PATH,
         "hess_method": "autograd",
     }
     calc_flags = recursive_dict_merge(calc_defaults, calc_kwargs)
 
-    ml_calculator = NewtonNet(**calc_flags)
-    atoms.calc = ml_calculator
+    atoms.calc = NewtonNet(**calc_flags)
     final_atoms = run_calc(atoms, copy_files=copy_files)
 
     summary = summarize_run(
         final_atoms, atoms, additional_fields={"name": "NewtonNet Hessian"}
     )
-    energy = summary["results"]["energy"]
-    hessian = summary["results"]["hessian"]
 
-    vib = VibrationsData(final_atoms, hessian)
-
-    igt = run_ideal_gas(final_atoms, vib.get_frequencies(), energy=energy)
+    vib = VibrationsData(final_atoms, summary["results"]["hessian"])
+    igt = run_ideal_gas(
+        final_atoms, vib.get_frequencies(), energy=summary["results"]["energy"]
+    )
 
     return summarize_vib_and_thermo(
         vib,
         igt,
         temperature=temperature,
         pressure=pressure,
         additional_fields={"name": "ASE Vibrations and Thermo Analysis"},
@@ -197,24 +200,23 @@
     Parameters
     ----------
     summary
         A dictionary containing information about the molecular trajectory.
 
     Returns
     -------
-    Dict
+    dict[str, Any]
         The modified summary dictionary with added standard deviation and
         Hessian values.
     """
     for i, atoms in enumerate(summary["trajectory"]):
-        ml_calculator = NewtonNet(
+        atoms.calc = NewtonNet(
             model_path=SETTINGS.NEWTONNET_MODEL_PATH,
             settings_path=SETTINGS.NEWTONNET_CONFIG_PATH,
         )
-        atoms.calc = ml_calculator
         results = run_calc(atoms).calc.results
         summary["trajectory_results"][i]["hessian"] = results["hessian"]
         summary["trajectory_results"][i]["energy_std"] = results["energy_disagreement"]
         summary["trajectory_results"][i]["forces_std"] = results["forces_disagreement"]
         summary["trajectory_results"][i]["hessian_std"] = results[
             "hessian_disagreement"
         ]
```

### Comparing `quacc-0.9.0/src/quacc/recipes/newtonnet/ts.py` & `quacc-0.9.1/src/quacc/recipes/newtonnet/ts.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 """Transition state recipes for the NewtonNet code."""
 
 from __future__ import annotations
 
+from importlib.util import find_spec
 from typing import TYPE_CHECKING
 
 from monty.dev import requires
 
 from quacc import SETTINGS, change_settings, job, strip_decorator
 from quacc.recipes.newtonnet.core import _add_stdev_and_hess, freq_job, relax_job
 from quacc.runners.ase import run_opt
 from quacc.schemas.ase import summarize_opt_run
 from quacc.utils.dicts import recursive_dict_merge
 
-try:
-    from sella import IRC, Sella
-except ImportError:
-    Sella = None
+has_sella = bool(find_spec("sella"))
+has_newtonnet = bool(find_spec("newtonnet"))
 
-try:
+if has_sella:
+    from sella import IRC, Sella
+if has_newtonnet:
     from newtonnet.utils.ase_interface import MLAseCalculator as NewtonNet
-except ImportError:
-    NewtonNet = None
+
 
 if TYPE_CHECKING:
     from typing import Any, Literal
 
     from ase.atoms import Atoms
     from numpy.typing import NDArray
 
@@ -40,16 +40,18 @@
 
     class QuasiIRCSchema(OptSchema):
         irc_job: IRCSchema
         freq_job: FreqSchema | None
 
 
 @job
-@requires(NewtonNet, "NewtonNet must be installed. Refer to the quacc documentation.")
-@requires(Sella, "Sella must be installed. Refer to the quacc documentation.")
+@requires(
+    has_newtonnet, "NewtonNet must be installed. Refer to the quacc documentation."
+)
+@requires(has_sella, "Sella must be installed. Refer to the quacc documentation.")
 def ts_job(
     atoms: Atoms,
     use_custom_hessian: bool = False,
     run_freq: bool = True,
     freq_job_kwargs: dict[str, Any] | None = None,
     opt_params: OptParams | None = None,
     **calc_kwargs,
@@ -93,21 +95,18 @@
             {"diag_every_n": 0, "order": 1} if use_custom_hessian else {"order": 1}
         ),
     }
 
     calc_flags = recursive_dict_merge(calc_defaults, calc_kwargs)
     opt_flags = recursive_dict_merge(opt_defaults, opt_params)
 
-    atoms.calc = NewtonNet(**calc_flags)
-
     if use_custom_hessian:
         opt_flags["optimizer_kwargs"]["hessian_function"] = _get_hessian
 
-    ml_calculator = NewtonNet(**calc_flags)
-    atoms.calc = ml_calculator
+    atoms.calc = NewtonNet(**calc_flags)
 
     # Run the TS optimization
     dyn = run_opt(atoms, **opt_flags)
     opt_ts_summary = _add_stdev_and_hess(
         summarize_opt_run(dyn, additional_fields={"name": "NewtonNet TS"})
     )
 
@@ -119,16 +118,18 @@
     )
     opt_ts_summary["freq_job"] = freq_summary
 
     return opt_ts_summary
 
 
 @job
-@requires(NewtonNet, "NewtonNet must be installed. Refer to the quacc documentation.")
-@requires(Sella, "Sella must be installed. Refer to the quacc documentation.")
+@requires(
+    has_newtonnet, "NewtonNet must be installed. Refer to the quacc documentation."
+)
+@requires(has_sella, "Sella must be installed. Refer to the quacc documentation.")
 def irc_job(
     atoms: Atoms,
     direction: Literal["forward", "reverse"] = "forward",
     run_freq: bool = True,
     freq_job_kwargs: dict[str, Any] | None = None,
     opt_params: OptParams | None = None,
     **calc_kwargs,
@@ -195,16 +196,18 @@
     )
     opt_irc_summary["freq_job"] = freq_summary
 
     return opt_irc_summary
 
 
 @job
-@requires(NewtonNet, "NewtonNet must be installed. Refer to the quacc documentation.")
-@requires(Sella, "Sella must be installed. Refer to the quacc documentation.")
+@requires(
+    has_newtonnet, "NewtonNet must be installed. Refer to the quacc documentation."
+)
+@requires(has_sella, "Sella must be installed. Refer to the quacc documentation.")
 def quasi_irc_job(
     atoms: Atoms,
     direction: Literal["forward", "reverse"] = "forward",
     run_freq: bool = True,
     irc_job_kwargs: dict[str, Any] | None = None,
     relax_job_kwargs: dict[str, Any] | None = None,
     freq_job_kwargs: dict[str, Any] | None = None,
```

### Comparing `quacc-0.9.0/src/quacc/recipes/onetep/_base.py` & `quacc-0.9.1/src/quacc/recipes/onetep/_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -124,12 +124,11 @@
     -------
     Onetep
         The Onetep calculator.
     """
     calc_flags = recursive_dict_merge(calc_defaults, calc_swaps)
 
     return Onetep(
-        pseudo_path=str(SETTINGS.ONETEP_PP_PATH) if SETTINGS.ONETEP_PP_PATH else ".",
-        parallel_info=SETTINGS.ONETEP_PARALLEL_CMD,
-        profile=OnetepProfile(SETTINGS.ONETEP_CMD),
+        profile=OnetepProfile(command=f"{SETTINGS.ONETEP_CMD}"),
+        pseudo_path=str(SETTINGS.ONETEP_PP_PATH),
         **calc_flags,
     )
```

### Comparing `quacc-0.9.0/src/quacc/recipes/onetep/core.py` & `quacc-0.9.1/src/quacc/recipes/onetep/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.9.0/src/quacc/recipes/orca/_base.py` & `quacc-0.9.1/src/quacc/recipes/orca/_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,14 +192,14 @@
     blocks = merge_list_params(default_blocks, block_swaps)
     if "xyzfile" not in inputs:
         inputs.append("xyzfile")
     orcasimpleinput = " ".join(inputs)
     orcablocks = "\n".join(blocks)
 
     return ORCA(
-        profile=OrcaProfile(SETTINGS.ORCA_CMD),
+        profile=OrcaProfile(command=SETTINGS.ORCA_CMD),
         charge=charge,
         mult=spin_multiplicity,
         orcasimpleinput=orcasimpleinput,
         orcablocks=orcablocks,
         **calc_kwargs,
     )
```

### Comparing `quacc-0.9.0/src/quacc/recipes/orca/core.py` & `quacc-0.9.1/src/quacc/recipes/orca/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.9.0/src/quacc/recipes/psi4/_base.py` & `quacc-0.9.1/src/quacc/recipes/psi4/_base.py`

 * *Files identical despite different names*

### Comparing `quacc-0.9.0/src/quacc/recipes/psi4/core.py` & `quacc-0.9.1/src/quacc/recipes/psi4/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import TYPE_CHECKING
 
 from monty.dev import requires
 
 from quacc import job
 from quacc.recipes.psi4._base import run_and_summarize
 
-has_psi4 = find_spec("psi4") is not None
+has_psi4 = bool(find_spec("psi4"))
 
 if TYPE_CHECKING:
     from ase.atoms import Atoms
 
     from quacc.schemas._aliases.ase import RunSchema
     from quacc.utils.files import Filenames, SourceDirectory
```

### Comparing `quacc-0.9.0/src/quacc/recipes/qchem/_base.py` & `quacc-0.9.1/src/quacc/recipes/qchem/_base.py`

 * *Files identical despite different names*

### Comparing `quacc-0.9.0/src/quacc/recipes/qchem/core.py` & `quacc-0.9.1/src/quacc/recipes/qchem/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 """Core recipes for Q-Chem."""
 
 from __future__ import annotations
 
+from importlib.util import find_spec
 from typing import TYPE_CHECKING
 
 from quacc import job
 from quacc.recipes.qchem._base import run_and_summarize, run_and_summarize_opt
 from quacc.utils.dicts import recursive_dict_merge
 
-try:
-    from sella import Sella
+has_sella = bool(find_spec("sella"))
 
-    has_sella = True
-except ImportError:
-    has_sella = False
+if has_sella:
+    from sella import Sella
 
 if TYPE_CHECKING:
     from ase.atoms import Atoms
 
     from quacc.runners.ase import OptParams
     from quacc.schemas._aliases.ase import OptSchema, RunSchema
     from quacc.utils.files import Filenames, SourceDirectory
```

### Comparing `quacc-0.9.0/src/quacc/recipes/qchem/ts.py` & `quacc-0.9.1/src/quacc/recipes/qchem/ts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 """Transition state recipes for Q-Chem."""
 
 from __future__ import annotations
 
+from importlib.util import find_spec
 from typing import TYPE_CHECKING
 
 from monty.dev import requires
 
 from quacc import change_settings, job, strip_decorator
 from quacc.atoms.core import perturb
 from quacc.recipes.qchem._base import run_and_summarize_opt
 from quacc.recipes.qchem.core import _BASE_SET, relax_job
 from quacc.utils.dicts import recursive_dict_merge
 
-try:
+has_sella = bool(find_spec("sella"))
+if has_sella:
     from sella import IRC, Sella
 
-    has_sella = True
-
-except ImportError:
-    has_sella = False
-
 if TYPE_CHECKING:
     from typing import Any, Literal
 
     from ase.atoms import Atoms
     from numpy.typing import NDArray
 
     from quacc.runners.ase import OptParams
```

### Comparing `quacc-0.9.0/src/quacc/recipes/tblite/core.py` & `quacc-0.9.1/src/quacc/recipes/tblite/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 """Core recipes for the tblite code."""
 
 from __future__ import annotations
 
+from importlib.util import find_spec
 from typing import TYPE_CHECKING
 
 from monty.dev import requires
 
 from quacc import job
 from quacc.runners.ase import run_calc, run_opt, run_vib
 from quacc.runners.thermo import run_ideal_gas
 from quacc.schemas.ase import summarize_opt_run, summarize_run, summarize_vib_and_thermo
 from quacc.utils.dicts import recursive_dict_merge
 
-try:
+has_tblite = bool(find_spec("tblite"))
+if has_tblite:
     from tblite.ase import TBLite
-except ImportError:
-    TBLite = None
 
 if TYPE_CHECKING:
     from typing import Literal
 
     from ase.atoms import Atoms
 
     from quacc.runners.ase import OptParams, VibKwargs
     from quacc.schemas._aliases.ase import OptSchema, RunSchema, VibThermoSchema
 
 
 @job
-@requires(TBLite, "tblite must be installed. Refer to the quacc documentation.")
+@requires(has_tblite, "tblite must be installed. Refer to the quacc documentation.")
 def static_job(
     atoms: Atoms,
     method: Literal["GFN1-xTB", "GFN2-xTB", "IPEA1-xTB"] = "GFN2-xTB",
     **calc_kwargs,
 ) -> RunSchema:
     """
     Carry out a single-point calculation.
@@ -60,15 +60,15 @@
     final_atoms = run_calc(atoms)
     return summarize_run(
         final_atoms, atoms, additional_fields={"name": "TBLite Static"}
     )
 
 
 @job
-@requires(TBLite, "tblite must be installed. Refer to the quacc documentation.")
+@requires(has_tblite, "tblite must be installed. Refer to the quacc documentation.")
 def relax_job(
     atoms: Atoms,
     method: Literal["GFN1-xTB", "GFN2-xTB", "IPEA1-xTB"] = "GFN2-xTB",
     relax_cell: bool = False,
     opt_params: OptParams | None = None,
     **calc_kwargs,
 ) -> OptSchema:
@@ -103,15 +103,15 @@
     atoms.calc = TBLite(**calc_flags)
     dyn = run_opt(atoms, relax_cell=relax_cell, **opt_params)
 
     return summarize_opt_run(dyn, additional_fields={"name": "TBLite Relax"})
 
 
 @job
-@requires(TBLite, "tblite must be installed. Refer to the quacc documentation.")
+@requires(has_tblite, "tblite must be installed. Refer to the quacc documentation.")
 def freq_job(
     atoms: Atoms,
     method: Literal["GFN1-xTB", "GFN2-xTB", "IPEA1-xTB"] = "GFN2-xTB",
     energy: float = 0.0,
     temperature: float = 298.15,
     pressure: float = 1.0,
     vib_kwargs: VibKwargs | None = None,
```

### Comparing `quacc-0.9.0/src/quacc/recipes/tblite/phonons.py` & `quacc-0.9.1/src/quacc/recipes/tblite/phonons.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,34 +8,33 @@
 from monty.dev import requires
 
 from quacc import flow
 from quacc.recipes.common.phonons import phonon_subflow
 from quacc.recipes.tblite.core import relax_job, static_job
 from quacc.wflow_tools.customizers import customize_funcs
 
-has_deps_tblite = find_spec("tblite") is not None
-has_deps_phonons = (
-    find_spec("phonopy") is not None and find_spec("seekpath") is not None
-)
+has_tblite = bool(find_spec("tblite"))
+has_phonopy = bool(find_spec("phonopy"))
+has_seekpath = bool(find_spec("seekpath"))
 
 if TYPE_CHECKING:
     from typing import Any, Callable
 
     from ase.atoms import Atoms
 
     from quacc.schemas._aliases.phonons import PhononSchema
 
 
 @flow
+@requires(has_tblite, "tblite must be installed. Refer to the quacc documentation.")
 @requires(
-    has_deps_tblite, "tblite must be installed. Refer to the quacc documentation."
+    has_phonopy, message="Phonopy must be installed. Run `pip install quacc[phonons]`"
 )
 @requires(
-    has_deps_phonons,
-    message="Phonopy and seekpath must be installed. Run `pip install quacc[phonons]`",
+    has_seekpath, message="Seekpath must be installed. Run `pip install quacc[phonons]`"
 )
 def phonon_flow(
     atoms: Atoms,
     symprec: float = 1e-4,
     min_lengths: float | tuple[float, float, float] | None = 20.0,
     supercell_matrix: (
         tuple[tuple[int, int, int], tuple[int, int, int], tuple[int, int, int]] | None
```

### Comparing `quacc-0.9.0/src/quacc/recipes/vasp/_base.py` & `quacc-0.9.1/src/quacc/recipes/vasp/_base.py`

 * *Files identical despite different names*

### Comparing `quacc-0.9.0/src/quacc/recipes/vasp/core.py` & `quacc-0.9.1/src/quacc/recipes/vasp/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.9.0/src/quacc/recipes/vasp/mp.py` & `quacc-0.9.1/src/quacc/recipes/vasp/mp.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,25 +6,25 @@
     Make sure that you use the Materials Project-compatible pseudpotential
     versions. The GGA workflows use the old (no version) PAW PBE potentials.
     The meta-GGA workflows currently use the v.54 PAW PBE potentials.
 """
 
 from __future__ import annotations
 
-from importlib import util
+from importlib.util import find_spec
 from typing import TYPE_CHECKING
 
 from monty.dev import requires
 
 from quacc import change_settings, flow, job
 from quacc.calculators.vasp.params import MPtoASEConverter
 from quacc.recipes.vasp._base import run_and_summarize
 from quacc.wflow_tools.customizers import customize_funcs
 
-has_atomate2 = util.find_spec("atomate2")
+has_atomate2 = bool(find_spec("atomate2"))
 if has_atomate2:
     from atomate2.vasp.jobs.mp import (
         MPGGARelaxMaker,
         MPGGAStaticMaker,
         MPMetaGGARelaxMaker,
         MPMetaGGAStaticMaker,
         MPPreRelaxMaker,
```

### Comparing `quacc-0.9.0/src/quacc/recipes/vasp/qmof.py` & `quacc-0.9.1/src/quacc/recipes/vasp/qmof.py`

 * *Files identical despite different names*

### Comparing `quacc-0.9.0/src/quacc/recipes/vasp/slabs.py` & `quacc-0.9.1/src/quacc/recipes/vasp/slabs.py`

 * *Files identical despite different names*

### Comparing `quacc-0.9.0/src/quacc/runners/ase.py` & `quacc-0.9.1/src/quacc/runners/ase.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Utility functions for running ASE calculators with ASE-based methods."""
 
 from __future__ import annotations
 
 import sys
+from importlib.util import find_spec
 from shutil import copy, copytree
 from typing import TYPE_CHECKING, Callable
 
 import numpy as np
 from ase.filters import FrechetCellFilter
 from ase.io import Trajectory, read
 from ase.optimize import BFGS
@@ -15,19 +16,19 @@
 from monty.os.path import zpath
 
 from quacc import SETTINGS
 from quacc.atoms.core import copy_atoms, get_final_atoms_from_dynamics
 from quacc.runners.prep import calc_cleanup, calc_setup, terminate
 from quacc.utils.dicts import recursive_dict_merge
 
-try:
-    from sella import Sella
+has_sella = bool(find_spec("sella"))
+
+if has_sella:
+    pass
 
-except ImportError:
-    Sella = None
 
 if TYPE_CHECKING:
     from pathlib import Path
     from typing import Any, TypedDict
 
     from ase.atoms import Atoms
     from ase.optimize.optimize import Optimizer
@@ -317,15 +318,15 @@
 
     # Perform cleanup operations
     calc_cleanup(vib.atoms, tmpdir, job_results_dir)
 
     return vib
 
 
-@requires(Sella, "Sella must be installed. Refer to the quacc documentation.")
+@requires(has_sella, "Sella must be installed. Refer to the quacc documentation.")
 def _set_sella_kwargs(atoms: Atoms, optimizer_kwargs: dict[str, Any]) -> None:
     """
     Modifies the `optimizer_kwargs` in-place to address various Sella-related
     parameters. This function does the following for the specified key/value pairs in
     `optimizer_kwargs`:
 
     1. Sets `order = 0` if not specified (i.e. minimization rather than TS
```

### Comparing `quacc-0.9.0/src/quacc/runners/phonons.py` & `quacc-0.9.1/src/quacc/runners/phonons.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,25 +4,27 @@
 from pathlib import Path
 from typing import TYPE_CHECKING
 
 from monty.dev import requires
 
 from quacc.runners.prep import calc_cleanup, calc_setup
 
-has_deps = find_spec("phonopy") is not None and find_spec("seekpath") is not None
+has_phonopy = bool(find_spec("phonopy"))
+has_seekpath = bool(find_spec("seekpath"))
 
 
 if TYPE_CHECKING:
     from numpy.typing import NDArray
 
-    if has_deps:
+    if has_phonopy:
         from phonopy import Phonopy
 
 
-@requires(has_deps, "Phonopy or seekpath is not installed.")
+@requires(has_phonopy, "Phonopy is not installed.")
+@requires(has_seekpath, "Seekpath is not installed.")
 def run_phonopy(
     phonon: Phonopy,
     forces: NDArray,
     t_step: float = 10,
     t_min: float = 0,
     t_max: float = 1000,
 ) -> Phonopy:
```

### Comparing `quacc-0.9.0/src/quacc/runners/prep.py` & `quacc-0.9.1/src/quacc/runners/prep.py`

 * *Files identical despite different names*

### Comparing `quacc-0.9.0/src/quacc/runners/thermo.py` & `quacc-0.9.1/src/quacc/runners/thermo.py`

 * *Files identical despite different names*

### Comparing `quacc-0.9.0/src/quacc/schemas/_aliases/ase.py` & `quacc-0.9.1/src/quacc/schemas/_aliases/ase.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,17 +16,15 @@
 
 
 class Parameters(TypedDict):
     """Dictionary of parameters from atoms.calc.parameters"""
 
 
 class ParametersOpt(TypedDict):
-    """Dictionary of parameters from Optimizer.todict() and fmax"""
-
-    fmax: float | None
+    """Dictionary of parameters from Optimizer.todict()"""
 
 
 class RunSchema(AtomsSchema):
     """Schema for [quacc.schemas.ase.summarize_run][]"""
 
     input_atoms: AtomsSchema | None
     nid: str
```

### Comparing `quacc-0.9.0/src/quacc/schemas/_aliases/atoms.py` & `quacc-0.9.1/src/quacc/schemas/_aliases/atoms.py`

 * *Files identical despite different names*

### Comparing `quacc-0.9.0/src/quacc/schemas/_aliases/cclib.py` & `quacc-0.9.1/src/quacc/schemas/_aliases/cclib.py`

 * *Files identical despite different names*

### Comparing `quacc-0.9.0/src/quacc/schemas/_aliases/emmet.py` & `quacc-0.9.1/src/quacc/schemas/_aliases/emmet.py`

 * *Files identical despite different names*

### Comparing `quacc-0.9.0/src/quacc/schemas/_aliases/phonons.py` & `quacc-0.9.1/src/quacc/schemas/_aliases/phonons.py`

 * *Files identical despite different names*

### Comparing `quacc-0.9.0/src/quacc/schemas/_aliases/vasp.py` & `quacc-0.9.1/src/quacc/schemas/_aliases/vasp.py`

 * *Files identical despite different names*

### Comparing `quacc-0.9.0/src/quacc/schemas/ase.py` & `quacc-0.9.1/src/quacc/schemas/ase.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,22 +189,21 @@
         initial_atoms,
         charge_and_multiplicity=charge_and_multiplicity,
         move_magmoms=move_magmoms,
         store=None,
     )
 
     # Clean up the opt parameters
-    parameters_opt = dyn.todict() | {"fmax": getattr(dyn, "fmax", None)}
+    parameters_opt = dyn.todict()
     parameters_opt.pop("logfile", None)
     parameters_opt.pop("restart", None)
 
     opt_fields = {
         "parameters_opt": parameters_opt,
         "converged": is_converged,
-        "nsteps": dyn.get_number_of_steps(),
         "trajectory": trajectory,
         "trajectory_results": [atoms.calc.results for atoms in trajectory],
     }
 
     # Create a dictionary of the inputs/outputs
     unsorted_task_doc = base_task_doc | opt_fields | additional_fields
```

### Comparing `quacc-0.9.0/src/quacc/schemas/atoms.py` & `quacc-0.9.1/src/quacc/schemas/atoms.py`

 * *Files identical despite different names*

### Comparing `quacc-0.9.0/src/quacc/schemas/cclib.py` & `quacc-0.9.1/src/quacc/schemas/cclib.py`

 * *Files identical despite different names*

### Comparing `quacc-0.9.0/src/quacc/schemas/phonons.py` & `quacc-0.9.1/src/quacc/schemas/phonons.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from monty.dev import requires
 
 from quacc import SETTINGS, __version__
 from quacc.schemas.atoms import atoms_to_metadata
 from quacc.utils.dicts import finalize_dict
 from quacc.utils.files import get_uri
 
-has_phonopy = find_spec("phonopy") is not None
+has_phonopy = bool(find_spec("phonopy"))
 
 if TYPE_CHECKING:
     from pathlib import Path
     from typing import Any
 
     from ase.atoms import Atoms
     from maggma.core import Store
```

### Comparing `quacc-0.9.0/src/quacc/schemas/prep.py` & `quacc-0.9.1/src/quacc/schemas/prep.py`

 * *Files identical despite different names*

### Comparing `quacc-0.9.0/src/quacc/schemas/vasp.py` & `quacc-0.9.1/src/quacc/schemas/vasp.py`

 * *Files identical despite different names*

### Comparing `quacc-0.9.0/src/quacc/settings.py` & `quacc-0.9.1/src/quacc/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     ] = Field(None, description=("The workflow manager to use, if any."))
 
     # ---------------------------
     # General Settings
     # ---------------------------
 
     RESULTS_DIR: Path = Field(
-        Path(),
+        Path.cwd(),
         description=(
             """
             Directory to permanently store I/O-based calculation results in.
             Note that this behavior may be modified by the chosen workflow engine.
             """
         ),
     )
@@ -170,14 +170,31 @@
             "wannier90": "wannier90.x",
             "fs": "fs.x",
             "postahc": "postahc.x",
             "dvscf_q2r": "dvscf_q2r.x",
         },
         description="Name for each espresso binary.",
     )
+    ESPRESSO_PARALLEL_CMD: Union[str, tuple[str, str]] = Field(
+        "",
+        description=(
+            """
+            Parallelization flags to run Espresso. The 0th index of the tuple
+            contains any commands that come before the binary, and the 1st index
+            contains any commands that come after the binary.
+
+            For example: ["mpirun -np 4", "-nk 2"] would be the same as running
+            Espresso via `"mpirun -np 4 {binary} -nk 2"` where {binary} is the
+            binary that is automatically determined based on the job type,
+            `ESPRESSO_BIN_DIR` and `ESPRESSO_BINARIES`.
+
+            If only a `str` is provided, no post-binary commands will be used.
+            """
+        ),
+    )
     ESPRESSO_PSEUDO: Optional[Path] = Field(
         None, description=("Path to a pseudopotential library for espresso.")
     )
     ESPRESSO_PRESET_DIR: Path = Field(
         Path(__file__).parent / "calculators" / "espresso" / "presets",
         description="Path to the espresso preset directory",
     )
@@ -186,26 +203,19 @@
     # Gaussian Settings
     # ---------------------------
     GAUSSIAN_CMD: str = Field("g16", description=("Path to the Gaussian executable."))
 
     # ---------------------------
     # ONETEP Settings
     # ---------------------------
-    ONETEP_CMD: Optional[str] = Field(
-        "onetep.arch", description=("Path to the ONETEP executable.")
-    )
-    ONETEP_PARALLEL_CMD: Optional[dict] = Field(
-        None,
-        description=(
-            "Parallelization commands to run ONETEP that are prepended to the executable."
-        ),
-    )
-    ONETEP_PP_PATH: Optional[Path] = Field(
-        None, description=("Path to pseudopotentials.")
+    ONETEP_CMD: str = Field(
+        "onetep.arch",
+        description=("Full ONETEP command, including parallelization flags."),
     )
+    ONETEP_PP_PATH: Path = Field(Path(), description=("Path to pseudopotentials."))
 
     # ---------------------------
     # GULP Settings
     # ---------------------------
     GULP_CMD: str = Field("gulp", description=("Path to the GULP executable."))
     GULP_LIB: Optional[Path] = Field(
         None,
@@ -445,14 +455,22 @@
             store_name = next(iter(v.keys()))
             store = getattr(stores, store_name)
 
             return store(**v[store_name])
         else:
             return v
 
+    @field_validator("ESPRESSO_PARALLEL_CMD")
+    @classmethod
+    def validate_espresso_parallel_cmd(cls, v: Union[str, tuple[str, str]]) -> Store:
+        """Clean up Espresso parallel command."""
+        if isinstance(v, str):
+            v = (v, "")
+        return v
+
     @model_validator(mode="before")
     @classmethod
     def load_user_settings(cls, settings: dict[str, Any]) -> dict[str, Any]:
         """
         Loads settings from a root file if available and uses that as defaults in place
         of built in defaults. Will also convert common strings to their proper types.
```

### Comparing `quacc-0.9.0/src/quacc/utils/dicts.py` & `quacc-0.9.1/src/quacc/utils/dicts.py`

 * *Files identical despite different names*

### Comparing `quacc-0.9.0/src/quacc/utils/files.py` & `quacc-0.9.1/src/quacc/utils/files.py`

 * *Files identical despite different names*

### Comparing `quacc-0.9.0/src/quacc/utils/kpts.py` & `quacc-0.9.1/src/quacc/utils/kpts.py`

 * *Files identical despite different names*

### Comparing `quacc-0.9.0/src/quacc/utils/lists.py` & `quacc-0.9.1/src/quacc/utils/lists.py`

 * *Files identical despite different names*

### Comparing `quacc-0.9.0/src/quacc/wflow_tools/customizers.py` & `quacc-0.9.1/src/quacc/wflow_tools/customizers.py`

 * *Files identical despite different names*

### Comparing `quacc-0.9.0/src/quacc/wflow_tools/db.py` & `quacc-0.9.1/src/quacc/wflow_tools/db.py`

 * *Files identical despite different names*

### Comparing `quacc-0.9.0/src/quacc/wflow_tools/decorators.py` & `quacc-0.9.1/src/quacc/wflow_tools/decorators.py`

 * *Files identical despite different names*

### Comparing `quacc-0.9.0/src/quacc.egg-info/PKG-INFO` & `quacc-0.9.1/src/quacc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quacc
-Version: 0.9.0
+Version: 0.9.1
 Summary: A platform to enable high-throughput, database-driven quantum chemistry and computational materials science
 Author-email: "Andrew S. Rosen" <asrosen@princeton.edu>
 Maintainer-email: "Andrew S. Rosen" <asrosen@princeton.edu>
 License: BSD-3
 Project-URL: repository, https://github.com/Quantum-Accelerators/quacc
 Project-URL: documentation, https://quantum-accelerators.github.io/quacc/
 Project-URL: changelog, https://github.com/Quantum-Accelerators/quacc/blob/main/CHANGELOG.md
@@ -20,15 +20,15 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: ase>=3.23.0b1
+Requires-Dist: ase>=3.23.0
 Requires-Dist: cclib>=1.8
 Requires-Dist: custodian>=2024.3.12
 Requires-Dist: emmet-core>=0.80.0
 Requires-Dist: maggma>=0.64.0
 Requires-Dist: monty>=2024.5.15
 Requires-Dist: numpy>=1.25.0
 Requires-Dist: psutil
@@ -55,15 +55,15 @@
 Requires-Dist: mace-torch>=0.3.3; extra == "mlp"
 Requires-Dist: torch-dftd>=0.4.0; extra == "mlp"
 Provides-Extra: mp
 Requires-Dist: atomate2>=0.0.14; extra == "mp"
 Provides-Extra: newtonnet
 Requires-Dist: newtonnet>=1.1; extra == "newtonnet"
 Provides-Extra: parsl
-Requires-Dist: parsl[monitoring]>=2023.10.23; platform_system != "Windows" and extra == "parsl"
+Requires-Dist: parsl[monitoring]>=2024.5.27; platform_system != "Windows" and extra == "parsl"
 Provides-Extra: phonons
 Requires-Dist: phonopy>=2.20.0; extra == "phonons"
 Requires-Dist: seekpath>=2.1.0; extra == "phonons"
 Provides-Extra: prefect
 Requires-Dist: prefect[dask]>=2.19.0; extra == "prefect"
 Requires-Dist: dask-jobqueue>=0.8.2; extra == "prefect"
 Provides-Extra: redun
```

### Comparing `quacc-0.9.0/src/quacc.egg-info/SOURCES.txt` & `quacc-0.9.1/src/quacc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quacc-0.9.0/src/quacc.egg-info/requires.txt` & `quacc-0.9.1/src/quacc.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-ase>=3.23.0b1
+ase>=3.23.0
 cclib>=1.8
 custodian>=2024.3.12
 emmet-core>=0.80.0
 maggma>=0.64.0
 monty>=2024.5.15
 numpy>=1.25.0
 psutil
@@ -55,15 +55,15 @@
 
 [newtonnet]
 newtonnet>=1.1
 
 [parsl]
 
 [parsl:platform_system != "Windows"]
-parsl[monitoring]>=2023.10.23
+parsl[monitoring]>=2024.5.27
 
 [phonons]
 phonopy>=2.20.0
 seekpath>=2.1.0
 
 [prefect]
 prefect[dask]>=2.19.0
```

