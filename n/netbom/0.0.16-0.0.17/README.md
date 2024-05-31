# Comparing `tmp/netbom-0.0.16.tar.gz` & `tmp/netbom-0.0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbom-0.0.16.tar", last modified: Sat May 25 19:42:03 2024, max compression
+gzip compressed data, was "netbom-0.0.17.tar", last modified: Fri May 31 18:20:43 2024, max compression
```

## Comparing `netbom-0.0.16.tar` & `netbom-0.0.17.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:42:03.316257 netbom-0.0.16/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:42:03.304257 netbom-0.0.16/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:42:03.308257 netbom-0.0.16/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-25 19:41:57.000000 netbom-0.0.16/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-25 19:41:57.000000 netbom-0.0.16/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-25 19:41:57.000000 netbom-0.0.16/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-25 19:41:57.000000 netbom-0.0.16/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-25 19:41:57.000000 netbom-0.0.16/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-25 19:41:57.000000 netbom-0.0.16/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-05-25 19:42:03.316257 netbom-0.0.16/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-05-25 19:41:57.000000 netbom-0.0.16/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-25 19:41:57.000000 netbom-0.0.16/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:42:03.308257 netbom-0.0.16/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-25 19:41:57.000000 netbom-0.0.16/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:42:03.308257 netbom-0.0.16/docs/figures/
--rw-r--r--   0 runner    (1001) docker     (127)    26815 2024-05-25 19:41:57.000000 netbom-0.0.16/docs/figures/Altium_LED-Resistor.svg
--rw-r--r--   0 runner    (1001) docker     (127)    25818 2024-05-25 19:41:57.000000 netbom-0.0.16/docs/figures/Altium_LED-Resistor_netlist.svg
--rw-r--r--   0 runner    (1001) docker     (127)    35851 2024-05-25 19:41:57.000000 netbom-0.0.16/docs/figures/KiCad_LED-Resistor.svg
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-25 19:41:57.000000 netbom-0.0.16/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-05-25 19:41:57.000000 netbom-0.0.16/docs/netlist.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-05-25 19:41:57.000000 netbom-0.0.16/docs/netlist_readers.rst
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-25 19:41:57.000000 netbom-0.0.16/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-25 19:41:57.000000 netbom-0.0.16/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-25 19:41:57.000000 netbom-0.0.16/requirements-tests.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-25 19:42:03.316257 netbom-0.0.16/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:42:03.304257 netbom-0.0.16/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:42:03.308257 netbom-0.0.16/src/netbom/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 19:41:57.000000 netbom-0.0.16/src/netbom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-05-25 19:41:57.000000 netbom-0.0.16/src/netbom/bom.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:42:03.312257 netbom-0.0.16/src/netbom/bom_readers/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-25 19:41:57.000000 netbom-0.0.16/src/netbom/bom_readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-25 19:41:57.000000 netbom-0.0.16/src/netbom/bom_readers/altium_bom_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    13652 2024-05-25 19:41:57.000000 netbom-0.0.16/src/netbom/netlist.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:42:03.312257 netbom-0.0.16/src/netbom/netlist_readers/
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-25 19:41:57.000000 netbom-0.0.16/src/netbom/netlist_readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6544 2024-05-25 19:41:57.000000 netbom-0.0.16/src/netbom/netlist_readers/rinf_netlist_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:42:03.316257 netbom-0.0.16/src/netbom.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-05-25 19:42:03.000000 netbom-0.0.16/src/netbom.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-25 19:42:03.000000 netbom-0.0.16/src/netbom.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 19:42:03.000000 netbom-0.0.16/src/netbom.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-25 19:42:03.000000 netbom-0.0.16/src/netbom.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-25 19:42:03.000000 netbom-0.0.16/src/netbom.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-25 19:42:03.000000 netbom-0.0.16/src/netbom.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:42:03.312257 netbom-0.0.16/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:42:03.304257 netbom-0.0.16/tests/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:42:03.312257 netbom-0.0.16/tests/examples/bom/
--rw-r--r--   0 runner    (1001) docker     (127)    18265 2024-05-25 19:41:57.000000 netbom-0.0.16/tests/examples/bom/Altium_LED-Resistor.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)    32133 2024-05-25 19:41:57.000000 netbom-0.0.16/tests/examples/bom/Altium_LT3580-Module.xlsx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:42:03.312257 netbom-0.0.16/tests/examples/netlist/
--rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-05-25 19:41:57.000000 netbom-0.0.16/tests/examples/netlist/Altium_LED-Resistor.FRP
--rw-r--r--   0 runner    (1001) docker     (127)    24611 2024-05-25 19:41:57.000000 netbom-0.0.16/tests/examples/netlist/Altium_LT3580-Module.FRP
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-25 19:41:57.000000 netbom-0.0.16/tests/examples/netlist/KiCad_LED-Resistor.frp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:42:03.304257 netbom-0.0.16/tests/examples/projects/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:42:03.316257 netbom-0.0.16/tests/examples/projects/Altium_LED-Resistor/
--rw-r--r--   0 runner    (1001) docker     (127)    34887 2024-05-25 19:41:57.000000 netbom-0.0.16/tests/examples/projects/Altium_LED-Resistor/Altium_LED-Resistor.PrjPcb
--rw-r--r--   0 runner    (1001) docker     (127)    35840 2024-05-25 19:41:57.000000 netbom-0.0.16/tests/examples/projects/Altium_LED-Resistor/Altium_LED-Resistor.SchDoc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:42:03.316257 netbom-0.0.16/tests/examples/projects/KiCad_LED-Resistor/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-25 19:41:57.000000 netbom-0.0.16/tests/examples/projects/KiCad_LED-Resistor/KiCad_LED-Resistor.kicad_pcb
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-25 19:41:57.000000 netbom-0.0.16/tests/examples/projects/KiCad_LED-Resistor/KiCad_LED-Resistor.kicad_prl
--rw-r--r--   0 runner    (1001) docker     (127)     7449 2024-05-25 19:41:57.000000 netbom-0.0.16/tests/examples/projects/KiCad_LED-Resistor/KiCad_LED-Resistor.kicad_pro
--rw-r--r--   0 runner    (1001) docker     (127)    19135 2024-05-25 19:41:57.000000 netbom-0.0.16/tests/examples/projects/KiCad_LED-Resistor/KiCad_LED-Resistor.kicad_sch
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-25 19:41:57.000000 netbom-0.0.16/tests/run_all.py
--rw-r--r--   0 runner    (1001) docker     (127)     5203 2024-05-25 19:41:57.000000 netbom-0.0.16/tests/test_bom.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-25 19:41:57.000000 netbom-0.0.16/tests/test_bom_readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4995 2024-05-25 19:41:57.000000 netbom-0.0.16/tests/test_netlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-05-25 19:41:57.000000 netbom-0.0.16/tests/test_netlist_readers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:20:43.940712 netbom-0.0.17/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:20:43.928712 netbom-0.0.17/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:20:43.932712 netbom-0.0.17/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-31 18:20:35.000000 netbom-0.0.17/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-31 18:20:35.000000 netbom-0.0.17/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-31 18:20:35.000000 netbom-0.0.17/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-31 18:20:35.000000 netbom-0.0.17/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-31 18:20:35.000000 netbom-0.0.17/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-31 18:20:35.000000 netbom-0.0.17/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-05-31 18:20:43.940712 netbom-0.0.17/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-05-31 18:20:35.000000 netbom-0.0.17/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-31 18:20:35.000000 netbom-0.0.17/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:20:43.932712 netbom-0.0.17/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-31 18:20:35.000000 netbom-0.0.17/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:20:43.932712 netbom-0.0.17/docs/figures/
+-rw-r--r--   0 runner    (1001) docker     (127)    26815 2024-05-31 18:20:35.000000 netbom-0.0.17/docs/figures/Altium_LED-Resistor.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    25818 2024-05-31 18:20:35.000000 netbom-0.0.17/docs/figures/Altium_LED-Resistor_netlist.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    35851 2024-05-31 18:20:35.000000 netbom-0.0.17/docs/figures/KiCad_LED-Resistor.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-31 18:20:35.000000 netbom-0.0.17/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-05-31 18:20:35.000000 netbom-0.0.17/docs/netlist.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-05-31 18:20:35.000000 netbom-0.0.17/docs/netlist_readers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-31 18:20:35.000000 netbom-0.0.17/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-31 18:20:35.000000 netbom-0.0.17/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-31 18:20:35.000000 netbom-0.0.17/requirements-tests.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-31 18:20:43.940712 netbom-0.0.17/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:20:43.928712 netbom-0.0.17/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:20:43.932712 netbom-0.0.17/src/netbom/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:20:35.000000 netbom-0.0.17/src/netbom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-05-31 18:20:35.000000 netbom-0.0.17/src/netbom/bom.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:20:43.936712 netbom-0.0.17/src/netbom/bom_readers/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-31 18:20:35.000000 netbom-0.0.17/src/netbom/bom_readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-31 18:20:35.000000 netbom-0.0.17/src/netbom/bom_readers/altium_bom_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13830 2024-05-31 18:20:35.000000 netbom-0.0.17/src/netbom/netlist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:20:43.936712 netbom-0.0.17/src/netbom/netlist_readers/
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-31 18:20:35.000000 netbom-0.0.17/src/netbom/netlist_readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6544 2024-05-31 18:20:35.000000 netbom-0.0.17/src/netbom/netlist_readers/rinf_netlist_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:20:43.940712 netbom-0.0.17/src/netbom.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-05-31 18:20:43.000000 netbom-0.0.17/src/netbom.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-31 18:20:43.000000 netbom-0.0.17/src/netbom.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 18:20:43.000000 netbom-0.0.17/src/netbom.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-31 18:20:43.000000 netbom-0.0.17/src/netbom.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-31 18:20:43.000000 netbom-0.0.17/src/netbom.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-31 18:20:43.000000 netbom-0.0.17/src/netbom.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:20:43.936712 netbom-0.0.17/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:20:43.928712 netbom-0.0.17/tests/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:20:43.936712 netbom-0.0.17/tests/examples/bom/
+-rw-r--r--   0 runner    (1001) docker     (127)    18265 2024-05-31 18:20:35.000000 netbom-0.0.17/tests/examples/bom/Altium_LED-Resistor.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)    32133 2024-05-31 18:20:35.000000 netbom-0.0.17/tests/examples/bom/Altium_LT3580-Module.xlsx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:20:43.936712 netbom-0.0.17/tests/examples/netlist/
+-rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-05-31 18:20:35.000000 netbom-0.0.17/tests/examples/netlist/Altium_LED-Resistor.FRP
+-rw-r--r--   0 runner    (1001) docker     (127)    24611 2024-05-31 18:20:35.000000 netbom-0.0.17/tests/examples/netlist/Altium_LT3580-Module.FRP
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-31 18:20:35.000000 netbom-0.0.17/tests/examples/netlist/KiCad_LED-Resistor.frp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:20:43.928712 netbom-0.0.17/tests/examples/projects/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:20:43.936712 netbom-0.0.17/tests/examples/projects/Altium_LED-Resistor/
+-rw-r--r--   0 runner    (1001) docker     (127)    34887 2024-05-31 18:20:35.000000 netbom-0.0.17/tests/examples/projects/Altium_LED-Resistor/Altium_LED-Resistor.PrjPcb
+-rw-r--r--   0 runner    (1001) docker     (127)    35840 2024-05-31 18:20:35.000000 netbom-0.0.17/tests/examples/projects/Altium_LED-Resistor/Altium_LED-Resistor.SchDoc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:20:43.940712 netbom-0.0.17/tests/examples/projects/KiCad_LED-Resistor/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-31 18:20:35.000000 netbom-0.0.17/tests/examples/projects/KiCad_LED-Resistor/KiCad_LED-Resistor.kicad_pcb
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-31 18:20:35.000000 netbom-0.0.17/tests/examples/projects/KiCad_LED-Resistor/KiCad_LED-Resistor.kicad_prl
+-rw-r--r--   0 runner    (1001) docker     (127)     7449 2024-05-31 18:20:35.000000 netbom-0.0.17/tests/examples/projects/KiCad_LED-Resistor/KiCad_LED-Resistor.kicad_pro
+-rw-r--r--   0 runner    (1001) docker     (127)    19135 2024-05-31 18:20:35.000000 netbom-0.0.17/tests/examples/projects/KiCad_LED-Resistor/KiCad_LED-Resistor.kicad_sch
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-31 18:20:35.000000 netbom-0.0.17/tests/run_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5203 2024-05-31 18:20:35.000000 netbom-0.0.17/tests/test_bom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-31 18:20:35.000000 netbom-0.0.17/tests/test_bom_readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-05-31 18:20:35.000000 netbom-0.0.17/tests/test_netlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-05-31 18:20:35.000000 netbom-0.0.17/tests/test_netlist_readers.py
```

### Comparing `netbom-0.0.16/.github/workflows/publish.yml` & `netbom-0.0.17/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `netbom-0.0.16/.github/workflows/tests.yml` & `netbom-0.0.17/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `netbom-0.0.16/.gitignore` & `netbom-0.0.17/.gitignore`

 * *Files identical despite different names*

### Comparing `netbom-0.0.16/LICENSE` & `netbom-0.0.17/LICENSE`

 * *Files identical despite different names*

### Comparing `netbom-0.0.16/Makefile` & `netbom-0.0.17/Makefile`

 * *Files identical despite different names*

### Comparing `netbom-0.0.16/PKG-INFO` & `netbom-0.0.17/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbom
-Version: 0.0.16
+Version: 0.0.17
 Summary: Library to read, convert and process electrical netlists and bill of materials generated in Altium Designer and KiCad.
 Home-page: https://github.com/partmanager/netbom
 Author: Piotr Kuligowski
 Project-URL: Bug Tracker, https://github.com/partmanager/netbom/issues
 Project-URL: Changelog, https://github.com/partmanager/netbom/releases
 Project-URL: Source Code, https://github.com/partmanager/netbom
 Project-URL: Documentation, https://partmanager.github.io/netbom
```

### Comparing `netbom-0.0.16/README.rst` & `netbom-0.0.17/README.rst`

 * *Files identical despite different names*

### Comparing `netbom-0.0.16/docs/conf.py` & `netbom-0.0.17/docs/conf.py`

 * *Files identical despite different names*

### Comparing `netbom-0.0.16/docs/figures/Altium_LED-Resistor.svg` & `netbom-0.0.17/docs/figures/Altium_LED-Resistor.svg`

 * *Files identical despite different names*

### Comparing `netbom-0.0.16/docs/figures/Altium_LED-Resistor_netlist.svg` & `netbom-0.0.17/docs/figures/Altium_LED-Resistor_netlist.svg`

 * *Files identical despite different names*

### Comparing `netbom-0.0.16/docs/figures/KiCad_LED-Resistor.svg` & `netbom-0.0.17/docs/figures/KiCad_LED-Resistor.svg`

 * *Files identical despite different names*

### Comparing `netbom-0.0.16/docs/netlist.rst` & `netbom-0.0.17/docs/netlist.rst`

 * *Files identical despite different names*

### Comparing `netbom-0.0.16/docs/netlist_readers.rst` & `netbom-0.0.17/docs/netlist_readers.rst`

 * *Files identical despite different names*

### Comparing `netbom-0.0.16/requirements-dev.txt` & `netbom-0.0.17/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `netbom-0.0.16/setup.cfg` & `netbom-0.0.17/setup.cfg`

 * *Files identical despite different names*

### Comparing `netbom-0.0.16/src/netbom/bom.py` & `netbom-0.0.17/src/netbom/bom.py`

 * *Files identical despite different names*

### Comparing `netbom-0.0.16/src/netbom/bom_readers/altium_bom_reader.py` & `netbom-0.0.17/src/netbom/bom_readers/altium_bom_reader.py`

 * *Files identical despite different names*

### Comparing `netbom-0.0.16/src/netbom/netlist.py` & `netbom-0.0.17/src/netbom/netlist.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,30 +15,29 @@
 """
 
 import json
 import re
 
 
 def natsort(string):
-
+    # Source: https://www.reddit.com/r/learnpython/comments/vp3nnv/simple_way_to_do_alphanumeric_sorting_in_python/
+    # [TODO] to implement better natural sorting algorithm
     start_digits     = (re.search(r'(?x)^\d+    ', string) or re.search('inf', 'inf')).group()
     start_non_digits = (re.search(r'(?x)^\D+    ', string) or re.search(   '',    '')).group()
     end_non_digits   = (re.search(r'(?x)\D+$    ', string) or re.search(   '',    '')).group()
     start_lower      = (re.search(r'(?x)^[a-z]+ ', string) or re.search(   '',    '')).group()
     start_upper      = (re.search(r'(?x)^[A-Z]+ ', string) or re.search(   '',    '')).group()
-    all_digits       = [ float(n) for n in re.findall('\d+', string) or ['inf'] ]
+    all_digits       = [float(n) for n in re.findall('\d+', string) or ['inf']]
 
-    return (
-        float(start_digits),
-        start_non_digits.casefold(),
-        start_upper,
-        start_lower,
-        end_non_digits,
-        all_digits
-    )
+    return (float(start_digits),
+            start_non_digits.casefold(),
+            start_upper,
+            start_lower,
+            end_non_digits,
+            all_digits)
 
 
 class NetlistPins:
     """NetlistPins class used to store pins. It also provides basic converters and operators.
     """
 
     def __init__(self, pins: list = None) -> None:
```

### Comparing `netbom-0.0.16/src/netbom/netlist_readers/rinf_netlist_reader.py` & `netbom-0.0.17/src/netbom/netlist_readers/rinf_netlist_reader.py`

 * *Files identical despite different names*

### Comparing `netbom-0.0.16/src/netbom.egg-info/PKG-INFO` & `netbom-0.0.17/src/netbom.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbom
-Version: 0.0.16
+Version: 0.0.17
 Summary: Library to read, convert and process electrical netlists and bill of materials generated in Altium Designer and KiCad.
 Home-page: https://github.com/partmanager/netbom
 Author: Piotr Kuligowski
 Project-URL: Bug Tracker, https://github.com/partmanager/netbom/issues
 Project-URL: Changelog, https://github.com/partmanager/netbom/releases
 Project-URL: Source Code, https://github.com/partmanager/netbom
 Project-URL: Documentation, https://partmanager.github.io/netbom
```

### Comparing `netbom-0.0.16/src/netbom.egg-info/SOURCES.txt` & `netbom-0.0.17/src/netbom.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netbom-0.0.16/tests/examples/bom/Altium_LED-Resistor.xlsx` & `netbom-0.0.17/tests/examples/bom/Altium_LED-Resistor.xlsx`

 * *Files identical despite different names*

### Comparing `netbom-0.0.16/tests/examples/bom/Altium_LT3580-Module.xlsx` & `netbom-0.0.17/tests/examples/bom/Altium_LT3580-Module.xlsx`

 * *Files identical despite different names*

### Comparing `netbom-0.0.16/tests/examples/netlist/Altium_LED-Resistor.FRP` & `netbom-0.0.17/tests/examples/netlist/Altium_LED-Resistor.FRP`

 * *Files identical despite different names*

### Comparing `netbom-0.0.16/tests/examples/netlist/Altium_LT3580-Module.FRP` & `netbom-0.0.17/tests/examples/netlist/Altium_LT3580-Module.FRP`

 * *Files identical despite different names*

### Comparing `netbom-0.0.16/tests/examples/projects/Altium_LED-Resistor/Altium_LED-Resistor.PrjPcb` & `netbom-0.0.17/tests/examples/projects/Altium_LED-Resistor/Altium_LED-Resistor.PrjPcb`

 * *Files identical despite different names*

### Comparing `netbom-0.0.16/tests/examples/projects/Altium_LED-Resistor/Altium_LED-Resistor.SchDoc` & `netbom-0.0.17/tests/examples/projects/Altium_LED-Resistor/Altium_LED-Resistor.SchDoc`

 * *Files identical despite different names*

### Comparing `netbom-0.0.16/tests/examples/projects/KiCad_LED-Resistor/KiCad_LED-Resistor.kicad_prl` & `netbom-0.0.17/tests/examples/projects/KiCad_LED-Resistor/KiCad_LED-Resistor.kicad_prl`

 * *Files identical despite different names*

### Comparing `netbom-0.0.16/tests/examples/projects/KiCad_LED-Resistor/KiCad_LED-Resistor.kicad_pro` & `netbom-0.0.17/tests/examples/projects/KiCad_LED-Resistor/KiCad_LED-Resistor.kicad_pro`

 * *Files identical despite different names*

### Comparing `netbom-0.0.16/tests/examples/projects/KiCad_LED-Resistor/KiCad_LED-Resistor.kicad_sch` & `netbom-0.0.17/tests/examples/projects/KiCad_LED-Resistor/KiCad_LED-Resistor.kicad_sch`

 * *Files identical despite different names*

### Comparing `netbom-0.0.16/tests/test_bom.py` & `netbom-0.0.17/tests/test_bom.py`

 * *Files identical despite different names*

### Comparing `netbom-0.0.16/tests/test_bom_readers.py` & `netbom-0.0.17/tests/test_bom_readers.py`

 * *Files identical despite different names*

### Comparing `netbom-0.0.16/tests/test_netlist.py` & `netbom-0.0.17/tests/test_netlist.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,45 +30,44 @@
         self.assertEqual(connections.to_dict(), {'D1': ['1', '2'],
                                                  'D2': ['3', '4'],
                                                  'D3': ['5', '6', '7', '8']})
         self.assertEqual(len(connections), 3)
 
 
 class TestNetlist(unittest.TestCase):
-    def _template_netlist(self):
+    def test_netlist_duplicated_net_designator_and_pins(self):
         netlist = Netlist()
         netlist.append_pins('NetR1_1', 'R1', ['1', '2'])
-        self.assertEqual(len(netlist), 1)
-        return netlist
-
-    def test_netlist_duplicated_net_designator_and_pins(self):
-        netlist = self._template_netlist()
         netlist.append_pins('NetR1_1', 'R1', ['1', '2'])
         self.assertEqual(netlist.to_dict(), {'NetR1_1': {'R1': ['1', '2']}})
 
     def test_netlist_duplicated_designator_and_pins(self):
-        netlist = self._template_netlist()
+        netlist = Netlist()
+        netlist.append_pins('NetR1_1', 'R1', ['1', '2'])
         netlist.append_pins('NetR2_2', 'R1', ['1', '2'])
         # [TODO] method: detecting designators and pins connected to the same net
         self.assertEqual(netlist.to_dict(), {'NetR1_1': {'R1': ['1', '2']},
                                              'NetR2_2': {'R1': ['1', '2']}})
         self.assertEqual(len(netlist), 2)
 
     def test_netlist_duplicated_net_and_designator(self):
-        netlist = self._template_netlist()
+        netlist = Netlist()
+        netlist.append_pins('NetR1_1', 'R1', ['1', '2'])
         netlist.append_pins('NetR1_1', 'R1', ['3', '4'])
         self.assertEqual(netlist.to_dict(), {'NetR1_1': {'R1': ['1', '2', '3', '4']}})
 
     def test_netlist_numeric_pins_sorting(self):
-        netlist = self._template_netlist()
+        netlist = Netlist()
+        netlist.append_pins('NetR1_1', 'R1', ['1', '2'])
         netlist.append_pins('NetR1_1', 'R1', ['4', '7'])
         self.assertEqual(netlist.to_dict(), {'NetR1_1': {'R1': ['1', '2', '4', '7']}})
 
     def test_netlist_alphanumeric_pins_sorting(self):
-        netlist = self._template_netlist()
+        netlist = Netlist()
+        netlist.append_pins('NetR1_1', 'R1', ['1', '2'])
         netlist.append_pins('NetR1_1', 'R1', ['A44', 'A4'])
         self.assertEqual(netlist.to_dict(), {'NetR1_1': {'R1': ['1', '2', 'A4', 'A44']}})
 
     def test_netlist_alphanumeric_pins_natural_sorting(self):
         netlist = Netlist()
         netlist.append_pins('NetR1_1', 'R1', ['3', '4', '6', '5', '7', '8', '1', '2',
                                               '9', '10', '12', '11', 'A100', 'A10', 'A2'])
```

### Comparing `netbom-0.0.16/tests/test_netlist_readers.py` & `netbom-0.0.17/tests/test_netlist_readers.py`

 * *Files identical despite different names*

