# Comparing `tmp/crip-1.7.9.tar.gz` & `tmp/crip-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crip-1.7.9.tar", last modified: Sun Mar  3 06:40:01 2024, max compression
+gzip compressed data, was "crip-1.8.0.tar", last modified: Fri May 31 16:10:15 2024, max compression
```

## Comparing `crip-1.7.9.tar` & `crip-1.8.0.tar`

### file list

```diff
@@ -1,75 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 06:40:01.289824 crip-1.7.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-03-03 06:39:57.000000 crip-1.7.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-03-03 06:40:01.289824 crip-1.7.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-03-03 06:39:57.000000 crip-1.7.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 06:40:01.273825 crip-1.7.9/crip/
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-03-03 06:39:57.000000 crip-1.7.9/crip/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 06:40:01.273825 crip-1.7.9/crip/_asset/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 06:40:01.277824 crip-1.7.9/crip/_asset/atten/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-03 06:39:57.000000 crip-1.7.9/crip/_asset/atten/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-03 06:39:57.000000 crip-1.7.9/crip/_asset/atten/commonDensity.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 06:40:01.281824 crip-1.7.9/crip/_asset/atten/data/
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-03-03 06:39:57.000000 crip-1.7.9/crip/_asset/atten/data/Adipose.txt
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-03-03 06:39:57.000000 crip-1.7.9/crip/_asset/atten/data/Air.txt
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-03-03 06:39:57.000000 crip-1.7.9/crip/_asset/atten/data/Al.txt
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-03-03 06:39:57.000000 crip-1.7.9/crip/_asset/atten/data/Au.txt
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-03-03 06:39:57.000000 crip-1.7.9/crip/_asset/atten/data/Blood.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-03-03 06:39:57.000000 crip-1.7.9/crip/_asset/atten/data/Bone.txt
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-03-03 06:39:57.000000 crip-1.7.9/crip/_asset/atten/data/Breast.txt
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-03-03 06:39:57.000000 crip-1.7.9/crip/_asset/atten/data/C.txt
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-03-03 06:39:57.000000 crip-1.7.9/crip/_asset/atten/data/Ca.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-03-03 06:39:57.000000 crip-1.7.9/crip/_asset/atten/data/CaCl2.txt
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-03-03 06:39:57.000000 crip-1.7.9/crip/_asset/atten/data/CaF2.txt
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-03-03 06:39:57.000000 crip-1.7.9/crip/_asset/atten/data/CdTe.txt
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-03-03 06:39:57.000000 crip-1.7.9/crip/_asset/atten/data/Cl.txt
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-03-03 06:39:57.000000 crip-1.7.9/crip/_asset/atten/data/Cu.txt
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-03-03 06:39:57.000000 crip-1.7.9/crip/_asset/atten/data/F.txt
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-03-03 06:39:57.000000 crip-1.7.9/crip/_asset/atten/data/Fe.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-03-03 06:39:57.000000 crip-1.7.9/crip/_asset/atten/data/Gd.txt
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-03-03 06:39:57.000000 crip-1.7.9/crip/_asset/atten/data/H.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-03-03 06:39:57.000000 crip-1.7.9/crip/_asset/atten/data/I.txt
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-03-03 06:39:57.000000 crip-1.7.9/crip/_asset/atten/data/Muscle.txt
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-03-03 06:39:57.000000 crip-1.7.9/crip/_asset/atten/data/N.txt
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-03-03 06:39:57.000000 crip-1.7.9/crip/_asset/atten/data/Na.txt
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-03-03 06:39:57.000000 crip-1.7.9/crip/_asset/atten/data/Ni.txt
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-03-03 06:39:57.000000 crip-1.7.9/crip/_asset/atten/data/O.txt
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-03-03 06:39:57.000000 crip-1.7.9/crip/_asset/atten/data/P.txt
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-03-03 06:39:57.000000 crip-1.7.9/crip/_asset/atten/data/PE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-03-03 06:39:57.000000 crip-1.7.9/crip/_asset/atten/data/PET.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-03-03 06:39:57.000000 crip-1.7.9/crip/_asset/atten/data/PMMA.txt
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-03-03 06:39:57.000000 crip-1.7.9/crip/_asset/atten/data/Pyrex.txt
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-03-03 06:39:57.000000 crip-1.7.9/crip/_asset/atten/data/S.txt
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-03-03 06:39:57.000000 crip-1.7.9/crip/_asset/atten/data/Si.txt
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-03-03 06:39:57.000000 crip-1.7.9/crip/_asset/atten/data/Sn.txt
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-03-03 06:39:57.000000 crip-1.7.9/crip/_asset/atten/data/SoftTissue.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-03-03 06:39:57.000000 crip-1.7.9/crip/_asset/atten/data/Teflon.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-03-03 06:39:57.000000 crip-1.7.9/crip/_asset/atten/data/Water.txt
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-03-03 06:39:57.000000 crip-1.7.9/crip/_asset/atten/data/WhiteMatter.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 06:40:01.289824 crip-1.7.9/crip/_asset/shepplogan/
--rw-r--r--   0 runner    (1001) docker     (127)  4194576 2024-03-03 06:39:57.000000 crip-1.7.9/crip/_asset/shepplogan/1024.tif
--rw-r--r--   0 runner    (1001) docker     (127)   262416 2024-03-03 06:39:57.000000 crip-1.7.9/crip/_asset/shepplogan/256.tif
--rw-r--r--   0 runner    (1001) docker     (127)  1048848 2024-03-03 06:39:57.000000 crip-1.7.9/crip/_asset/shepplogan/512.tif
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-03-03 06:39:57.000000 crip-1.7.9/crip/_rc.py
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-03-03 06:39:57.000000 crip-1.7.9/crip/_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     8372 2024-03-03 06:39:57.000000 crip-1.7.9/crip/de.py
--rw-r--r--   0 runner    (1001) docker     (127)    10222 2024-03-03 06:39:57.000000 crip-1.7.9/crip/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-03-03 06:39:57.000000 crip-1.7.9/crip/lowdose.py
--rw-r--r--   0 runner    (1001) docker     (127)    10683 2024-03-03 06:39:57.000000 crip-1.7.9/crip/mangoct.py
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-03-03 06:39:57.000000 crip-1.7.9/crip/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)    15095 2024-03-03 06:39:57.000000 crip-1.7.9/crip/physics.py
--rw-r--r--   0 runner    (1001) docker     (127)     7492 2024-03-03 06:39:57.000000 crip-1.7.9/crip/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-03-03 06:39:57.000000 crip-1.7.9/crip/postprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     9406 2024-03-03 06:39:57.000000 crip-1.7.9/crip/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     9198 2024-03-03 06:39:57.000000 crip-1.7.9/crip/shared.py
--rw-r--r--   0 runner    (1001) docker     (127)     5690 2024-03-03 06:39:57.000000 crip-1.7.9/crip/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-03-03 06:39:57.000000 crip-1.7.9/crip/zoo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 06:40:01.277824 crip-1.7.9/crip.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-03-03 06:40:01.000000 crip-1.7.9/crip.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-03-03 06:40:01.000000 crip-1.7.9/crip.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-03 06:40:01.000000 crip-1.7.9/crip.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-03 06:40:01.000000 crip-1.7.9/crip.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-03 06:40:01.000000 crip-1.7.9/crip.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-03-03 06:40:01.289824 crip-1.7.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-03-03 06:39:57.000000 crip-1.7.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 06:40:01.289824 crip-1.7.9/test/
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-03-03 06:39:57.000000 crip-1.7.9/test/test_it_just_imports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:10:15.153117 crip-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-31 16:10:08.000000 crip-1.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-31 16:10:15.153117 crip-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-31 16:10:08.000000 crip-1.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:10:15.141116 crip-1.8.0/crip/
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-31 16:10:08.000000 crip-1.8.0/crip/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:10:15.137116 crip-1.8.0/crip/_asset/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:10:15.141116 crip-1.8.0/crip/_asset/atten/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:10:15.145116 crip-1.8.0/crip/_asset/atten/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-31 16:10:08.000000 crip-1.8.0/crip/_asset/atten/data/Adipose.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-31 16:10:08.000000 crip-1.8.0/crip/_asset/atten/data/Air.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-31 16:10:08.000000 crip-1.8.0/crip/_asset/atten/data/Al.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-31 16:10:08.000000 crip-1.8.0/crip/_asset/atten/data/Au.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-31 16:10:08.000000 crip-1.8.0/crip/_asset/atten/data/Blood.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-31 16:10:08.000000 crip-1.8.0/crip/_asset/atten/data/Bone.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-31 16:10:08.000000 crip-1.8.0/crip/_asset/atten/data/Breast.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-31 16:10:08.000000 crip-1.8.0/crip/_asset/atten/data/C.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-31 16:10:08.000000 crip-1.8.0/crip/_asset/atten/data/Ca.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-31 16:10:08.000000 crip-1.8.0/crip/_asset/atten/data/CaCl2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-31 16:10:08.000000 crip-1.8.0/crip/_asset/atten/data/CaF2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-31 16:10:08.000000 crip-1.8.0/crip/_asset/atten/data/CdTe.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-31 16:10:08.000000 crip-1.8.0/crip/_asset/atten/data/Cl.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-31 16:10:08.000000 crip-1.8.0/crip/_asset/atten/data/Cu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-31 16:10:08.000000 crip-1.8.0/crip/_asset/atten/data/F.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-31 16:10:08.000000 crip-1.8.0/crip/_asset/atten/data/Fe.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-31 16:10:08.000000 crip-1.8.0/crip/_asset/atten/data/Gd.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-31 16:10:08.000000 crip-1.8.0/crip/_asset/atten/data/H.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-31 16:10:08.000000 crip-1.8.0/crip/_asset/atten/data/I.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-31 16:10:08.000000 crip-1.8.0/crip/_asset/atten/data/Muscle.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-31 16:10:08.000000 crip-1.8.0/crip/_asset/atten/data/N.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-31 16:10:08.000000 crip-1.8.0/crip/_asset/atten/data/Na.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-31 16:10:08.000000 crip-1.8.0/crip/_asset/atten/data/Ni.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-31 16:10:08.000000 crip-1.8.0/crip/_asset/atten/data/O.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-31 16:10:08.000000 crip-1.8.0/crip/_asset/atten/data/P.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-31 16:10:08.000000 crip-1.8.0/crip/_asset/atten/data/PE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-31 16:10:08.000000 crip-1.8.0/crip/_asset/atten/data/PET.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-31 16:10:08.000000 crip-1.8.0/crip/_asset/atten/data/PMMA.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-31 16:10:08.000000 crip-1.8.0/crip/_asset/atten/data/Pyrex.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-31 16:10:08.000000 crip-1.8.0/crip/_asset/atten/data/S.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-31 16:10:08.000000 crip-1.8.0/crip/_asset/atten/data/Si.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-31 16:10:08.000000 crip-1.8.0/crip/_asset/atten/data/Sn.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-31 16:10:08.000000 crip-1.8.0/crip/_asset/atten/data/SoftTissue.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-31 16:10:08.000000 crip-1.8.0/crip/_asset/atten/data/Teflon.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-31 16:10:08.000000 crip-1.8.0/crip/_asset/atten/data/Water.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-31 16:10:08.000000 crip-1.8.0/crip/_asset/atten/data/WhiteMatter.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-31 16:10:08.000000 crip-1.8.0/crip/_asset/atten/density.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:10:15.153117 crip-1.8.0/crip/_asset/shepplogan/
+-rw-r--r--   0 runner    (1001) docker     (127)  4194576 2024-05-31 16:10:08.000000 crip-1.8.0/crip/_asset/shepplogan/1024.tif
+-rw-r--r--   0 runner    (1001) docker     (127)   262416 2024-05-31 16:10:08.000000 crip-1.8.0/crip/_asset/shepplogan/256.tif
+-rw-r--r--   0 runner    (1001) docker     (127)  1048848 2024-05-31 16:10:08.000000 crip-1.8.0/crip/_asset/shepplogan/512.tif
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-31 16:10:08.000000 crip-1.8.0/crip/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9722 2024-05-31 16:10:08.000000 crip-1.8.0/crip/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6334 2024-05-31 16:10:08.000000 crip-1.8.0/crip/lowdose.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11000 2024-05-31 16:10:08.000000 crip-1.8.0/crip/mangoct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-05-31 16:10:08.000000 crip-1.8.0/crip/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16392 2024-05-31 16:10:08.000000 crip-1.8.0/crip/physics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7884 2024-05-31 16:10:08.000000 crip-1.8.0/crip/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-05-31 16:10:08.000000 crip-1.8.0/crip/postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8559 2024-05-31 16:10:08.000000 crip-1.8.0/crip/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9635 2024-05-31 16:10:08.000000 crip-1.8.0/crip/shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-05-31 16:10:08.000000 crip-1.8.0/crip/spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6579 2024-05-31 16:10:08.000000 crip-1.8.0/crip/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:10:15.141116 crip-1.8.0/crip.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-31 16:10:15.000000 crip-1.8.0/crip.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-31 16:10:15.000000 crip-1.8.0/crip.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 16:10:15.000000 crip-1.8.0/crip.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-31 16:10:15.000000 crip-1.8.0/crip.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-31 16:10:15.000000 crip-1.8.0/crip.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-31 16:10:15.153117 crip-1.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-31 16:10:08.000000 crip-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:10:15.153117 crip-1.8.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-31 16:10:08.000000 crip-1.8.0/test/test_lowdose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-31 16:10:08.000000 crip-1.8.0/test/test_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-05-31 16:10:08.000000 crip-1.8.0/test/test_physics.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-31 16:10:08.000000 crip-1.8.0/test/test_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-31 16:10:08.000000 crip-1.8.0/test/test_postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-31 16:10:08.000000 crip-1.8.0/test/test_preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5139 2024-05-31 16:10:08.000000 crip-1.8.0/test/test_shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-31 16:10:08.000000 crip-1.8.0/test/test_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-31 16:10:08.000000 crip-1.8.0/test/test_utils.py
```

### Comparing `crip-1.7.9/LICENSE` & `crip-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `crip-1.7.9/crip/__init__.py` & `crip-1.8.0/crip/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,19 +3,18 @@
 __license__ = 'MIT License'
 __doc__ = '''
 CT Recon in Python: An all-in-one tool for Data IO, Pre/Post-process, Physics, Dual Energy, Low Dose and everything.
 https://github.com/SEU-CT-Recon/crip
 '''
 
 __all__ = [
-    'de', 'io', 'lowdose', 'physics', 'postprocess', 'preprocess', 'shared', 'utils', 'mangoct', 'plot', 'metric', '_rc'
+    'spec', 'io', 'lowdose', 'physics', 'postprocess', 'preprocess', 'shared', 'utils', 'mangoct', 'plot', 'metric'
 ]
 
-from . import _rc
-from . import de
+from . import spec
 from . import io
 from . import lowdose
 from . import physics
 from . import postprocess
 from . import preprocess
 from . import shared
 from . import utils
```

### Comparing `crip-1.7.9/crip/_asset/atten/commonDensity.json` & `crip-1.8.0/crip/_asset/atten/density.json`

 * *Files identical despite different names*

### Comparing `crip-1.7.9/crip/_asset/atten/data/Adipose.txt` & `crip-1.8.0/crip/_asset/atten/data/Adipose.txt`

 * *Files identical despite different names*

### Comparing `crip-1.7.9/crip/_asset/atten/data/Air.txt` & `crip-1.8.0/crip/_asset/atten/data/Air.txt`

 * *Files identical despite different names*

### Comparing `crip-1.7.9/crip/_asset/atten/data/Al.txt` & `crip-1.8.0/crip/_asset/atten/data/Al.txt`

 * *Files identical despite different names*

### Comparing `crip-1.7.9/crip/_asset/atten/data/Au.txt` & `crip-1.8.0/crip/_asset/atten/data/Au.txt`

 * *Files identical despite different names*

### Comparing `crip-1.7.9/crip/_asset/atten/data/Bone.txt` & `crip-1.8.0/crip/_asset/atten/data/Bone.txt`

 * *Files identical despite different names*

### Comparing `crip-1.7.9/crip/_asset/atten/data/Breast.txt` & `crip-1.8.0/crip/_asset/atten/data/Breast.txt`

 * *Files identical despite different names*

### Comparing `crip-1.7.9/crip/_asset/atten/data/C.txt` & `crip-1.8.0/crip/_asset/atten/data/C.txt`

 * *Files identical despite different names*

### Comparing `crip-1.7.9/crip/_asset/atten/data/Ca.txt` & `crip-1.8.0/crip/_asset/atten/data/Ca.txt`

 * *Files identical despite different names*

### Comparing `crip-1.7.9/crip/_asset/atten/data/CaCl2.txt` & `crip-1.8.0/crip/_asset/atten/data/CaCl2.txt`

 * *Files identical despite different names*

### Comparing `crip-1.7.9/crip/_asset/atten/data/CaF2.txt` & `crip-1.8.0/crip/_asset/atten/data/CaF2.txt`

 * *Files identical despite different names*

### Comparing `crip-1.7.9/crip/_asset/atten/data/CdTe.txt` & `crip-1.8.0/crip/_asset/atten/data/CdTe.txt`

 * *Files identical despite different names*

### Comparing `crip-1.7.9/crip/_asset/atten/data/Cl.txt` & `crip-1.8.0/crip/_asset/atten/data/Cl.txt`

 * *Files identical despite different names*

### Comparing `crip-1.7.9/crip/_asset/atten/data/Cu.txt` & `crip-1.8.0/crip/_asset/atten/data/Cu.txt`

 * *Files identical despite different names*

### Comparing `crip-1.7.9/crip/_asset/atten/data/F.txt` & `crip-1.8.0/crip/_asset/atten/data/F.txt`

 * *Files identical despite different names*

### Comparing `crip-1.7.9/crip/_asset/atten/data/Fe.txt` & `crip-1.8.0/crip/_asset/atten/data/Fe.txt`

 * *Files identical despite different names*

### Comparing `crip-1.7.9/crip/_asset/atten/data/Gd.txt` & `crip-1.8.0/crip/_asset/atten/data/Gd.txt`

 * *Files identical despite different names*

### Comparing `crip-1.7.9/crip/_asset/atten/data/H.txt` & `crip-1.8.0/crip/_asset/atten/data/H.txt`

 * *Files identical despite different names*

### Comparing `crip-1.7.9/crip/_asset/atten/data/I.txt` & `crip-1.8.0/crip/_asset/atten/data/I.txt`

 * *Files identical despite different names*

### Comparing `crip-1.7.9/crip/_asset/atten/data/Muscle.txt` & `crip-1.8.0/crip/_asset/atten/data/Muscle.txt`

 * *Files identical despite different names*

### Comparing `crip-1.7.9/crip/_asset/atten/data/N.txt` & `crip-1.8.0/crip/_asset/atten/data/N.txt`

 * *Files identical despite different names*

### Comparing `crip-1.7.9/crip/_asset/atten/data/Na.txt` & `crip-1.8.0/crip/_asset/atten/data/Na.txt`

 * *Files identical despite different names*

### Comparing `crip-1.7.9/crip/_asset/atten/data/Ni.txt` & `crip-1.8.0/crip/_asset/atten/data/Ni.txt`

 * *Files identical despite different names*

### Comparing `crip-1.7.9/crip/_asset/atten/data/O.txt` & `crip-1.8.0/crip/_asset/atten/data/O.txt`

 * *Files identical despite different names*

### Comparing `crip-1.7.9/crip/_asset/atten/data/P.txt` & `crip-1.8.0/crip/_asset/atten/data/P.txt`

 * *Files identical despite different names*

### Comparing `crip-1.7.9/crip/_asset/atten/data/PE.txt` & `crip-1.8.0/crip/_asset/atten/data/PE.txt`

 * *Files identical despite different names*

### Comparing `crip-1.7.9/crip/_asset/atten/data/PET.txt` & `crip-1.8.0/crip/_asset/atten/data/PET.txt`

 * *Files identical despite different names*

### Comparing `crip-1.7.9/crip/_asset/atten/data/PMMA.txt` & `crip-1.8.0/crip/_asset/atten/data/PMMA.txt`

 * *Files identical despite different names*

### Comparing `crip-1.7.9/crip/_asset/atten/data/S.txt` & `crip-1.8.0/crip/_asset/atten/data/S.txt`

 * *Files identical despite different names*

### Comparing `crip-1.7.9/crip/_asset/atten/data/Si.txt` & `crip-1.8.0/crip/_asset/atten/data/Si.txt`

 * *Files identical despite different names*

### Comparing `crip-1.7.9/crip/_asset/atten/data/SoftTissue.txt` & `crip-1.8.0/crip/_asset/atten/data/SoftTissue.txt`

 * *Files identical despite different names*

### Comparing `crip-1.7.9/crip/_asset/atten/data/Teflon.txt` & `crip-1.8.0/crip/_asset/atten/data/Teflon.txt`

 * *Files identical despite different names*

### Comparing `crip-1.7.9/crip/_asset/atten/data/Water.txt` & `crip-1.8.0/crip/_asset/atten/data/Water.txt`

 * *Files identical despite different names*

### Comparing `crip-1.7.9/crip/_asset/shepplogan/1024.tif` & `crip-1.8.0/crip/_asset/shepplogan/1024.tif`

 * *Files identical despite different names*

### Comparing `crip-1.7.9/crip/_asset/shepplogan/256.tif` & `crip-1.8.0/crip/_asset/shepplogan/256.tif`

 * *Files identical despite different names*

### Comparing `crip-1.7.9/crip/_asset/shepplogan/512.tif` & `crip-1.8.0/crip/_asset/shepplogan/512.tif`

 * *Files identical despite different names*

### Comparing `crip-1.7.9/crip/io.py` & `crip-1.8.0/crip/io.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,13 @@
 '''
     I/O module of crip.
 
     https://github.com/SEU-CT-Recon/crip
 '''
 
-__all__ = [
-    'listDirectory', 'imreadDicom', 'readDicom', 'imreadRaw', 'imwriteRaw', 'imreadTiff', 'imwriteTiff', 'CTPARAMS',
-    'fetchCTParam', 'readEVI', 'imreadEVI'
-]
-
 import os
 import re
 import numpy as np
 import tifffile
 import pydicom
 import natsort
 
@@ -21,20 +16,20 @@
 
 
 def listDirectory(folder: str,
                   style='filename',
                   match: Or[re.Pattern, str, None] = None,
                   sort='nat',
                   reverse=False) -> Or[List[str], Iterable[Tuple[str, str]]]:
-    '''
-        List files under `folder` and sort in `nat`(ural) or `dict`(ionary) order. 
+    ''' List files under `folder` and `sort` in `nat`(ural) or `dict`(ionary) order.
         Return `style` can be `filename`, `fullpath` or `both` (path, name) tuple.
+        Results can be filtered by `match` and reversed by `reverse`.
     '''
-    cripAssert(sort in ['nat', 'dict'], 'Invalid sort.')
-    cripAssert(style in ['filename', 'fullpath', 'both'], 'Invalid style.')
+    cripAssert(sort in ['nat', 'dict'], f'Invalid `sort`: {sort}.')
+    cripAssert(style in ['filename', 'fullpath', 'both'], f'Invalid `style`: {style}.')
 
     files = os.listdir(folder)
 
     if match is not None:
         if isinstance(match, str):
             match = re.compile(match)
         files = list(filter(lambda x: match.search(x), files))
@@ -46,171 +41,164 @@
         return files
     elif style == 'fullpath':
         return [os.path.join(folder, file) for file in files]
     elif style == 'both':
         return zip([os.path.join(folder, file) for file in files], files)
 
 
-def imreadDicom(path: str, dtype=None, attrs: Or[None, Dict[str, Any]] = None) -> np.ndarray:
-    '''
-        Read DICOM file. Return numpy array. Use `attrs` to supplement DICOM tags for non-standard images.
-        You should be very careful about the whether Rescale Slope is cancelled for CT images.
-    
-        Convert dtype with `dtype != None`.
+def imreadDicom(path: str, dtype=None, attrs: Or[None, Dict[str, Any]] = None) -> NDArray:
+    ''' Read DICOM file, return numpy array. Use `attrs` to supplement DICOM tags for non-standard images.
+        You should be very careful whether the Rescale is cancelled for CT images.
+        Convert dtype when `dtype` is not `None`.
     '''
     dcm = pydicom.dcmread(path)
 
     if attrs is not None:
         for key in attrs:
             dcm.__setattr__(key, attrs[key])
 
     if dtype is not None:
         return np.array(dcm.pixel_array).astype(dtype)
     else:
         return np.array(dcm.pixel_array)
 
 
-def imreadDicoms(dir_: str, dtype=None, attrs: Or[None, Dict[str, Any]] = None) -> np.ndarray:
-    '''
-        Read series of DICOM files in directory.
+def imreadDicoms(dir_: str, **kwargs) -> NDArray:
+    ''' Read series of DICOM files in a directory. `kwargs` is forwarded to `imreadDicom`.
     '''
-    imgs = [imreadDicom(x, dtype, attrs) for x in listDirectory(dir_, style='fullpath')]
+    imgs = [imreadDicom(x, **kwargs) for x in listDirectory(dir_, style='fullpath')]
 
     return np.array(imgs)
 
 
 def readDicom(path: str) -> pydicom.Dataset:
-    '''
-        Read DICOM file as pydicom object.
+    ''' Read DICOM file as pydicom Dataset object.
     '''
     return pydicom.read_file(path)
 
 
 def imreadRaw(path: str,
               h: int,
               w: int,
               dtype=DefaultFloatDType,
               nSlice: int = 1,
               offset: int = 0,
               gap: int = 0,
-              order='CHW') -> np.ndarray:
-    '''
-        Read binary raw file. Return numpy array with shape `(nSlice, h, w)`. `offset` from head in bytes.
-        `gap` between images in bytes.
-    '''
-    cripAssert(order in ['CHW', 'HWC'], 'Invalid order.')
+              swapEndian=False) -> NDArray:
+    ''' Read binary raw file stored in `dtype`.
+        Return numpy array with shape `(min(nSlice, actualNSlice), h, w)`.
+        Input `nSlice` can be unequal to the actual number of slices.
+        Allow setting `offset` from head and `gap` between images in bytes.
+        Allow change the endian-ness to the contrary of your machine by `swapEndian`.
+        This function acts like ImageJ's `Import Raw`.
+    '''
+    simpleValidate([
+        offset >= 0,
+        h > 0 and w > 0 and nSlice > 0,
+    ])
+
+    slices = []
+    sliceBytes = h * w * np.dtype(dtype).itemsize  # bytes per slice
+    fileBytes = os.path.getsize(path)  # actual bytes of the file
+
+    fp = open(path, 'rb')
+    fp.seek(offset)
+    for _ in range(nSlice):
+        slices.append(np.frombuffer(fp.read(sliceBytes), dtype=dtype).reshape((h, w)).squeeze())
+        fp.seek(gap, os.SEEK_CUR)
+        if fp.tell() >= fileBytes:
+            break
+    fp.close()
+
+    slices = np.array(slices).astype(dtype)
 
-    with open(path, 'rb') as fp:
-        fp.seek(offset)
-        if gap == 0:
-            arr = np.frombuffer(fp.read(), dtype=dtype).reshape((nSlice, h, w)).squeeze()
-        else:
-            cripAssert(order == 'CHW', 'gap is only availble in CHW order.')
-            imageBytes = h * w * np.dtype(dtype).itemsize
-            arr = np.zeros((nSlice, h, w), dtype=dtype)
-            for i in range(nSlice):
-                arr[i, ...] = np.frombuffer(fp.read(imageBytes), dtype=dtype).reshape((h, w)).squeeze()
-                fp.seek(gap, os.SEEK_CUR)
-
-    if order == 'HWC':
-        arr = np.transpose(arr, (2, 0, 1))
-
-    return arr
+    return slices if not swapEndian else slices.byteswap(inplace=True)
 
 
-def imreadRaws(dir_: str,
-               h: int,
-               w: int,
-               dtype=DefaultFloatDType,
-               nSlice: int = 1,
-               offset: int = 0,
-               gap: int = 0,
-               order='CHW'):
+def imreadRaws(dir_: str, **kwargs: Any) -> NDArray:
+    ''' Read series of raw images in directory. `kwargs` will be forwarded to `imreadRaw`.
     '''
-        Read series of raw images in directory.
-    '''
-    imgs = [imreadRaw(x, h, w, dtype, nSlice, offset, gap, order) for x in listDirectory(dir_, style='fullpath')]
+    imgs = [imreadRaw(x, **kwargs) for x in listDirectory(dir_, style='fullpath')]
 
     return np.array(imgs)
 
 
 @ConvertListNDArray
-def imwriteRaw(img: TwoOrThreeD, path: str, dtype=None, order='CHW'):
-    '''
-        Write raw file. Convert dtype with `dtype != None`.
+def imwriteRaw(img: TwoOrThreeD, path: str, dtype=None, order='CHW', swapEndian=False, fortranOrder=False):
+    ''' Write `img` to raw file `path`. Convert dtype when `dtype` is not `None`.
+        `order` can be [CHW or HWC].
+        Allow change the endian-ness to the contrary of your machine by `swapEndian`.
+        Allow using Fortran order (Column-major) by setting `fortranOrder`.
     '''
-    cripAssert(order in ['CHW', 'HWC'], 'Invalid order.')
+    cripAssert(order in ['CHW', 'HWC'], f'Invalid order: {order}.')
 
     if dtype is not None:
         img = img.astype(dtype)
+    if order == 'HWC':
+        img = chw2hwc(img)
+    if swapEndian:
+        img = img.byteswap(inplace=False)
 
     with open(path, 'wb') as fp:
-        if order == 'HWC':
-            img = np.transpose(img, (1, 2, 0))
-        fp.write(img.flatten().tobytes())
+        fp.write(img.tobytes('F' if fortranOrder else 'C'))
 
 
-def imreadTiff(path: str, dtype=None):
-    '''
-        Read TIFF file. Return numpy array. Convert dtype with `dtype != None`.
+def imreadTiff(path: str, dtype=None) -> NDArray:
+    ''' Read TIFF file, return numpy array. Convert dtype when `dtype` is not `None`.
     '''
     if dtype is not None:
         return np.array(tifffile.imread(path)).astype(dtype)
     else:
         return np.array(tifffile.imread(path))
 
 
-def imreadTiffs(dir_: str, dtype=None):
-    '''
-        Read series of tiff images in directory. Will add one dim.
+def imreadTiffs(dir_: str, **kwargs) -> NDArray:
+    ''' Read series of tiff images in directory. `kwargs` will be forwarded to `imreadTiff`.
     '''
-    imgs = [imreadTiff(x, dtype) for x in listDirectory(dir_, style='fullpath')]
+    imgs = [imreadTiff(x, **kwargs) for x in listDirectory(dir_, style='fullpath')]
 
     return np.array(imgs)
 
 
 @ConvertListNDArray
 def imwriteTiff(img: TwoOrThreeD, path: str, dtype=None):
-    '''
-        Write TIFF file. Convert dtype with `dtype != None`.
-        
-        Note that any floating dtype will be converted to float32.
+    ''' Write TIFF file. Convert dtype if `dtype` is not `None`.
+        All floating dtype will be converted to float32.
     '''
     if dtype is not None:
         img = img.astype(dtype)
     if isFloatDtype(img.dtype):
-        img = img.astype(np.float32)  # always use float32 for floating image.
+        img = img.astype(np.float32)
 
     tifffile.imwrite(path, img)
 
 
-def readEVI(path: str):
-    '''
-        Read EVI file saved by XCounter Hydra PCD detector. Return the images and metadata.
+def readEVI(path: str) -> Tuple[NDArray, Dict[str, Any]]:
+    ''' Read EVI file saved by XCounter Hydra PCD detector. Return the images and metadata.
     '''
     metadata = {
         'ImageType': None,
         'Width': None,
         'Height': None,
         'NumberOfImages': None,
         'OffsetToFirstImage': None,
         'GapBetweenImages': None,
         'FrameRate': None,
         'LowThreshold': None,
         'HighThreshold': None,
     }
 
+    # mapping between EVI file prelude and metadata to fill in
     mapping = {
         'Image_Type': 'ImageType',
         'Width': 'Width',
         'Height': 'Height',
         'Nr_of_images': 'NumberOfImages',
         'Offset_To_First_Image': 'OffsetToFirstImage',
-        # interesting
-        'Gap_between_iamges_in_bytes': 'GapBetweenImages',
+        'Gap_between_iamges_in_bytes': 'GapBetweenImages',  # for compatibility
         'Gap_between_images_in_bytes': 'GapBetweenImages',
         'Frame_Rate_HZ': 'FrameRate',
         'Low_Thresholds_KV': 'LowThreshold',
         'High_Thresholds_KV': 'HighThreshold',
     }
 
     take = lambda str, idx: str.split(' ')[idx]
@@ -226,93 +214,76 @@
                 metadata[mapping[key]] = int(val) if str.isdigit(val) else val
 
             line = fp.readline().strip()
 
     nones = list(filter(lambda x: x[1] is None, metadata.items()))
     cripAssert(len(nones) == 0, f'Failed to find metadata for {list(map(lambda x: x[0], nones))}')
     cripAssert(metadata['ImageType'] in ['Single', 'Double'], f'Unsupported ImageType: {metadata["ImageType"]}')
-    dtype = {'Single': np.float32, 'Double': np.float64}
 
+    dtype = {'Single': np.float32, 'Double': np.float64}
     img = imreadRaw(path, metadata['Height'], metadata['Width'], dtype[metadata['ImageType']],
                     metadata['NumberOfImages'], metadata['OffsetToFirstImage'], metadata['GapBetweenImages'])
 
     return img, metadata
 
 
-def imreadEVI(path: str):
-    '''
-        Read EVI file saved by XCounter Hydra PCD detector. Return the images only.
+def imreadEVI(path: str) -> NDArray:
+    ''' Read EVI file saved by XCounter Hydra PCD detector. Return the images only.
     '''
     return readEVI(path)[0]
 
 
-def _CTPARAM(loc, type_):
-    return {'loc': loc, 'type': type_}
-
-
-# These CT parameters will be retrieved.
+# These CT parameters can be retrieved.
 CTPARAMS = {
-    # For WC sometimes two values will be fetched. Usually they are the same.
-    # If not, it means that the view is recommended to be displayed using to windows.
-    # So as WD.
-    'Window Center': _CTPARAM([0x0028, 0x1050], str),
-    'Window Width': _CTPARAM([0x0028, 0x1051], str),
-
     # Manufacturer
-    'Manufacturer': _CTPARAM([0x0008, 0x0070], str),
-    'Manufacturer Model Name': _CTPARAM([0x0008, 0x1090], str),
+    'Manufacturer': ([0x0008, 0x0070], str),
+    'Manufacturer Model Name': ([0x0008, 0x1090], str),
 
     # Study
-    'Series Instance UID': _CTPARAM([0x0020, 0x000E], str),
+    'Series Instance UID': ([0x0020, 0x000E], str),
 
     # Patient status
-    'Body Part Examined': _CTPARAM([0x0018, 0x0015], str),
-    'Patient Position': _CTPARAM([0x0018, 0x5100], str),  # (H/F)F(S/P)
+    'Body Part Examined': ([0x0018, 0x0015], str),
+    'Patient Position': ([0x0018, 0x5100], str),  # (H/F)F(S/P)
 
     # X-Ray exposure
-    'KVP': _CTPARAM([0x0018, 0x0060], float),  # kVpeak
-    'X Ray Tube Current': _CTPARAM([0x0018, 0x1151], float),  # mA
-    'Exposure Time': _CTPARAM([0x0018, 0x1150], float),
-    'Exposure': _CTPARAM([0x0018, 0x1152], float),
+    'KVP': ([0x0018, 0x0060], float),
+    'X Ray Tube Current': ([0x0018, 0x1151], float),  # mA
+    'Exposure Time': ([0x0018, 0x1150], float),
+    'Exposure': ([0x0018, 0x1152], float),
 
     # CT Reconstruction
-    'Slice Thickness': _CTPARAM([0x0018, 0x0050], float),
-    'Data Collection Diameter': _CTPARAM([0x0018, 0x0090], float),
-    'Reconstruction Diameter': _CTPARAM([0x0018, 0x1100], float),
-    'Rows': _CTPARAM([0x0028, 0x0010], int),
-    'Columns': _CTPARAM([0x0028, 0x0011], int),
-    'Pixel Spacing': _CTPARAM([0x0028, 0x0030], str),  # u/v, mm
-    'Distance Source To Detector': _CTPARAM([0x0018, 0x1110], float),  # SDD (S-Image-D), mm
-    'Distance Source To Patient': _CTPARAM([0x0018, 0x1111], float),  # SOD (S-Isocenter-D), mm
-    'Rotation Direction': _CTPARAM([0x0018, 0x1140], str),  # CW/CCW
-    'Bits Allocated': _CTPARAM([0x0028, 0x0100], int),
+    'Slice Thickness': ([0x0018, 0x0050], float),
+    'Data Collection Diameter': ([0x0018, 0x0090], float),
+    'Reconstruction Diameter': ([0x0018, 0x1100], float),
+    'Rows': ([0x0028, 0x0010], int),
+    'Columns': ([0x0028, 0x0011], int),
+    'Pixel Spacing': ([0x0028, 0x0030], str),  # u/v, mm
+    'Distance Source To Detector': ([0x0018, 0x1110], float),  # mm
+    'Distance Source To Patient': ([0x0018, 0x1111], float),  # mm
+    'Rotation Direction': ([0x0018, 0x1140], str),  # CW/CCW
+    'Bits Allocated': ([0x0028, 0x0100], int),
 
     # Table
-    'Table Height': _CTPARAM([0x0018, 0x1130], float),
-    'Table Speed': _CTPARAM([0x0018, 0x9309], float),
-    'Table Feed Per Rotation': _CTPARAM([0x0018, 0x9310], float),
-
-    # CT Value rescaling
-    # e.g.  HU = 1X-1024
-    'Rescale Intercept': _CTPARAM([0x0028, 0x1052], float),  # b
-    'Rescale Slope': _CTPARAM([0x0028, 0x1053], float),  # k
-    'Rescale Type': _CTPARAM([0x0028, 0x1054], str),
+    'Table Height': ([0x0018, 0x1130], float),
+    'Table Speed': ([0x0018, 0x9309], float),
+    'Table Feed Per Rotation': ([0x0018, 0x9310], float),
+
+    # CT value rescaling
+    'Rescale Intercept': ([0x0028, 0x1052], float),
+    'Rescale Slope': ([0x0028, 0x1053], float),
+    'Rescale Type': ([0x0028, 0x1054], str),
 
-    # For helical CT
-    'Spiral Pitch Factor': _CTPARAM([0x0018, 0x9311], float)
+    # Helical CT
+    'Spiral Pitch Factor': ([0x0018, 0x9311], float)
 }
 
 
-def fetchCTParam(dicom: pydicom.Dataset, key: str):
+def fetchCTParam(dicom: pydicom.Dataset, key: str) -> Any:
+    ''' Fetch CT metadata from DICOM Dataset read by `readDicom`
+        Refer to `CTPARAMS` for available keys.
     '''
-        Fetch CT related parameter from DICOM file. Use `readDicom` to get DICOM Dataset.
+    cripAssert(key in CTPARAMS.keys(), f'Invalid key: {key}.')
 
-        @see CTPARAMS in the source code for available keys.
-    '''
-    metaParam = CTPARAMS[key]
-    if metaParam is None:
-        return None
-    try:
-        value = metaParam['type'](dicom[metaParam['loc'][0], metaParam['loc'][1]].value)
-    except:
-        return None
-    return value
+    addr, cast = CTPARAMS[key]
+
+    return cast(dicom[addr[0], addr[1]].value)
```

### Comparing `crip-1.7.9/crip/mangoct.py` & `crip-1.8.0/crip/mangoct.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,53 +1,59 @@
 '''
-    MangoCT integration interface. See https://github.com/SEU-CT-Recon/mandoct
+    MangoCT integration interface.
 
     https://github.com/SEU-CT-Recon/crip
 '''
 
-__all__ = ['Mgfbp', 'Mgfpj', 'MgfbpConfig', 'MgfpjConfig']
-
 import os
 import json
 import tempfile
 import subprocess
 
-from .utils import cripAssert, isType
+from .utils import cripAssert, getAttrKeysOfObject, isType
 from ._typing import *
 
 
-class _MgConfig(object):
+class _MgCliConfig(object):
+    ''' The base class for configuration of CLI version of mangoct.
+    '''
 
     def __init__(self):
         pass
 
     def dumpJSON(self):
-        attrs = [
-            a for a in (set(dir(self)) - set(dir(object)))
-            if not a.startswith('__') and not callable(getattr(self, a)) and getattr(self, a) is not None
-        ]
-        dict_ = dict([(k, getattr(self, k)) for k in attrs])
+        ''' Dump the configuration to JSON string.
+        '''
+        dict_ = dict([(k, getattr(self, k)) for k in getAttrKeysOfObject(self)])
 
         return json.dumps(dict_, indent=2)
 
     def dumpJSONFile(self, path: str):
+        ''' Dump the configuration to JSON file.
+        '''
         with open(path, 'w') as fp:
             fp.write(self.dumpJSON())
 
     def fromJSON(self, json_: str):
+        ''' Load the configuration from JSON string.
+        '''
         obj = json.loads(json_)
         for key in obj:
-            self[key] = obj
+            self[key] = obj[key]
 
     def fromJSONFile(self, path: str):
+        ''' Load the configuration from JSON file.
+        '''
         with open(path, 'r') as fp:
             self.fromJSON(fp.read())
 
 
-class MgfbpConfig(_MgConfig):
+class MgfbpCliConfig(_MgCliConfig):
+    ''' Configuration class for CLI version `mgfbp`.
+    '''
 
     def __init__(self):
         super().__init__()
         self.setIO(None, None, None, None, [])
         self.setGeometry(None, None, None, None, None, None, None, None)
         self.setSgmConeBeam(None, None, None, None, None, None, None)
         self.setRecConeBeam(None, None, None, None, 'HammingFilter', 1, None, None, None, None, None)
@@ -147,15 +153,17 @@
         self.setRecFanBeam(ImageDimension, PixelSize, _Filter, _FilterParam, ImageRotation, ImageCenter, WaterMu,
                            SaveFilteredSinogram)
         self.ImageSliceCount = ImageSliceCount
         self.ImageSliceThickness = ImageSliceThickness
         self.ImageCenterZ = ImageCenterZ
 
 
-class MgfpjConfig(_MgConfig):
+class MgfpjCliConfig(_MgCliConfig):
+    ''' Configuration class for CLI version `mgfpj`.
+    '''
 
     def __init__(self):
         super().__init__()
         self.setIO(None, None, None, None, [])
         self.setGeometry(None, None, None, None)
         self.setRecConeBeam(None, None, None, None)
         self.setSgmConeBeam(None, None, None, None, None, None, None, None)
@@ -215,57 +223,57 @@
                        OversampleSize: int = 2):
         self.setSgmFanBeam(Views, DetectorElementCount, DetectorElementSize, DetectorOffcenter, OversampleSize)
         self.DetectorZElementCount = DetectorZElementCount
         self.DetectorElementHeight = DetectorElementHeight
         self.DetectorZOffcenter = DetectorZOffcenter
 
 
-class _Mgbin(object):
+class _MgCliBin(object):
+    ''' The base class for execution of CLI version of mangoct.
+    '''
 
     def __init__(self, exe: str, name: str, cudaDevice: int = 0, tempDir: str = None):
         self.exe = exe
         self.name = name
         self.cudaDevice = cudaDevice
         self.tempDir = tempDir
-        self.cmd = []
-        self.cmd.append([f'{self.exe}', '<1>'])
+        self.cmd = [f'{self.exe}', '<1>']
 
-    def exec(self, conf: Or[str, _MgConfig], verbose=True):
-        if isType(conf, _MgConfig):
+    def exec(self, conf: Or[str, _MgCliConfig], verbose=True):
+        if isType(conf, _MgCliConfig):
             tmp = tempfile.NamedTemporaryFile('w',
                                               prefix='crip_mangoct_',
                                               suffix=f'.{self.name}.jsonc',
                                               dir=self.tempDir,
                                               delete=False)
             tmp.write(conf.dumpJSON())
             conf = tmp.name
             tmp.close()
 
         os.environ['CUDA_VISIBLE_DEVICES'] = str(self.cudaDevice)
         stdout = stderr = None if verbose else subprocess.DEVNULL
-
         for cmd in self.cmd:
             if len(cmd) == 2:  # include args
                 cmd[1] = cmd[1].replace('<1>', conf)
                 subprocess.run(cmd, stdout=stdout, stderr=stderr)
             else:
                 os.system(cmd[0])
 
 
-class Mgfbp(_Mgbin):
+class MgCliFbp(_MgCliBin):
 
-    def __init__(self, exe: str = 'mgfbp', cudaDevice: int = 0, tempDir: str = None):
-        '''
-            Initialize a handler object to use the FBP tool in mangoct.
+    def __init__(self, exe='mgfbp', cudaDevice=0, tempDir: Or[str, None] = None):
+        ''' Initialize a handler object to use the CLI version FBP tool in mangoct.
             `exe` is the path to the executable.
         '''
         super().__init__(exe, 'mgfbp', cudaDevice, tempDir)
 
 
-class Mgfpj(_Mgbin):
+class MgCliFpj(_MgCliBin):
 
-    def __init__(self, exe: str = 'mgfpj', cudaDevice=0, tempDir: str = None) -> None:
-        '''
-            Initialize a handler object to use the FPJ tool in mangoct.
+    def __init__(self, exe='mgfpj', cudaDevice=0, tempDir: Or[str, None] = None):
+        ''' Initialize a handler object to use the CLI version FPJ tool in mangoct.
             `exe` is the path to the executable.
         '''
         super().__init__(exe, 'mgfpj', cudaDevice, tempDir)
+
+# TODO Add supports for Taichi version mangoct.
```

### Comparing `crip-1.7.9/crip/physics.py` & `crip-1.8.0/crip/physics.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,406 +1,421 @@
-'''
-    Physics module of crip.
-
-    https://github.com/SEU-CT-Recon/crip
-'''
-
-__all__ = [
-    'Spectrum', 'Atten', 'Material', 'calcMu', 'DiagEnergyLow', 'DiagEnergyHigh', 'DiagEnergyRange', 'DiagEnergyLen',
-    'forwardProjectWithSpectrum', 'brewPowderSolution', 'calcContrastHU', 'getCommonDensity', 'EnergyConversion',
-    'calcPathLength'
-]
-
-import json
-import re
-import numpy as np
-from os import path
-import enum
-
-from ._typing import *
-from .utils import cvtEnergyUnit, cvtMuUnit, inArray, cripAssert, getAsset, inRange, isOfSameShape, isType, readFileText, cvtConcentrationUnit
-from .io import listDirectory
-from .postprocess import muToHU
-
-## Constants ##
-
-DiagEnergyLow = 0  # keV
-DiagEnergyHigh = 150  # keV
-DiagEnergyRange = range(DiagEnergyLow, DiagEnergyHigh + 1)  # Diagonstic energy range, [low, high)
-DiagEnergyLen = DiagEnergyHigh - DiagEnergyLow + 1
-AttenAliases = {
-    'Gold': 'Au',
-    'Carbon': 'C',
-    'Copper': 'Cu',
-    'Iodine': 'I',
-    'H2O': 'Water',
-    'Gadolinium': 'Gd',
-}
-
-
-# recommended
-class EnergyConversion(enum.Enum):
-    EID = 'EID'  # Energy-Integrating Detector
-    PCD = 'PCD'  # Photon-Counting Detector
-
-
-def getCommonDensity(materialName: str):
-    '''
-        Get the common value of density of a specified material (g/cm^3) from built-in dataset.
-    '''
-    rhoObject = json.loads(readFileText(path.join(getAsset('atten'), 'commonDensity.json')))
-
-    if materialName in AttenAliases:
-        materialName = AttenAliases[materialName]
-    cripAssert(materialName in rhoObject, f'Material not found in density dataset: {materialName}')
-
-    return rhoObject[materialName]
-
-
-class Spectrum:
-    '''
-        Construct Spectrum object with omega array of every energy.
-
-        Get \\omega of certain energy (keV):
-        ```py
-            omega = spec.omega[E]
-        ```
-    '''
-
-    def __init__(self, omega: np.ndarray, unit='keV'):
-        cripAssert(
-            len(omega) == DiagEnergyLen,
-            f'omega array should have same length as DiagEnergyLen: got {len(omega)} expect {DiagEnergyLen}.')
-        cripAssert(inArray(unit, ['MeV', 'keV', 'eV']), f'Invalid unit: {unit}')
-
-        self.unit = unit
-        self.omega = np.array(omega, dtype=np.float32)
-        self.sumOmega = np.sum(self.omega)
-
-    def isMonochromatic(self):
-        at = -1
-        for i in DiagEnergyRange:
-            if self.omega[i] > 0:
-                if at != -1:
-                    return False, None
-                at = i
-
-        return True, at
-
-    @staticmethod
-    def fromText(specText: str, unit='keV'):
-        '''
-            Parse spectrum text as `Spectrum` class object.
-            
-            Refer to the document for spectrum text format. @see https://github.com/SEU-CT-Recon/crip      
-        '''
-        cripAssert(inArray(unit, ['MeV', 'keV', 'eV']), f'Invalid unit: {unit}')
-        omega = np.zeros(DiagEnergyLen, dtype=DefaultFloatDType)
-
-        # split content into list, and ignore all lines starting with non-digit
-        content = list(
-            filter(lambda y: len(y) > 0 and str.isdigit(y[0]),
-                   list(map(lambda x: x.strip(),
-                            specText.replace('\r\n', '\n').split('\n')))))
-
-        def procSpecLine(line: str):
-            tup = tuple(map(float, re.split(r'\s+', line)))
-            cripAssert(len(tup) == 2, f'Invalid line in spectrum: \n{line}\n')
-            return tup  # (energy, omega)
-
-        # parse the spectrum text
-        content = np.array(list(map(procSpecLine, content)), dtype=DefaultFloatDType)
-        specEnergy, specOmega = content.T
-        specOmega[specOmega < 0] = 0
-
-        # to keV
-        specEnergy = cvtEnergyUnit(specEnergy, unit, DefaultEnergyUnit)
-
-        startEnergy, cutOffEnergy = int(specEnergy[0]), int(specEnergy[-1])
-        cripAssert(inRange(startEnergy, DiagEnergyRange),
-                   f'startEnergy is out of DiagEnergyRange: {DiagEnergyRange} keV')
-        cripAssert(inRange(cutOffEnergy, DiagEnergyRange),
-                   f'cutOffEnergy is out of DiagEnergyRange: {DiagEnergyRange} keV')
-        cripAssert(cutOffEnergy + 1 - startEnergy == len(specOmega),
-                   'The spectrum is not continous by 1 keV from start to cutoff.')
-
-        omega[startEnergy:cutOffEnergy + 1] = specOmega[:]
-
-        return Spectrum(omega, unit)
-
-    @staticmethod
-    def fromFile(path: str, unit='keV'):
-        '''
-            Construct a Spectrum object from spectrum file (first column is energy while second is omega).
-        '''
-        spec = readFileText(path)
-
-        return Spectrum.fromText(spec, unit)
-
-    @staticmethod
-    def monochromatic(at: int, unit='keV', omega=10**5):
-        '''
-            Construct a monochromatic spectrum.
-        '''
-        text = '{} {}\n{} -1'.format(str(at), str(omega), str(at + 1))
-
-        return Spectrum.fromText(text, unit)
-
-
-class Atten:
-    '''
-        Parse atten text as `Atten` class object. Interpolation is performed to fill `DiagEnergyRange`.
-        Refer to the document for atten text format (NIST ASCII). The density is in g/cm^3.
-
-        Get \\mu (mm-1) of certain energy (keV):
-        ```py
-            mu = atten.mu[E]
-        ```
-    '''
-
-    def __init__(self, muArray: NDArray, density: Or[None, float] = None) -> None:
-        cripAssert(len(muArray) == DiagEnergyLen, f'muArray should have length of {DiagEnergyLen} energy bins')
-        self.mu = muArray
-        self.rho = density
-        self.attenText = ''
-        self.energyUnit = 'keV'
-
-    @staticmethod
-    def builtInAttenList() -> List:
-        '''
-            Get all built-in materials.
-        '''
-        attenListPath = path.join(getAsset('atten'), 'data')
-        attenList = list(map(lambda x: x.replace('.txt', ''), listDirectory(attenListPath, style='filename')))
-        attenList.extend(AttenAliases.keys())
-
-        return attenList
-
-    @staticmethod
-    def _builtInAttenText(materialName: str):
-        '''
-            Get the built-in atten file content of `materialName` from NIST data source.
-        '''
-        if materialName in AttenAliases:
-            materialName = AttenAliases[materialName]
-
-        attenFilePath = path.join(getAsset('atten'), f'data/{materialName}.txt')
-        cripAssert(path.exists(attenFilePath), f'Atten file for {materialName} does not exist.')
-        content = readFileText(attenFilePath)
-
-        return content
-
-    @staticmethod
-    def fromBuiltIn(materialName: str, density: Or[float, None] = None):
-        '''
-            Get the built-in atten object.
-            Call `builtInAttenList` to get available materials.
-            The density is in g/cm^3.
-        '''
-        if materialName in AttenAliases:
-            materialName = AttenAliases[materialName]
-
-        if density is None:
-            density = getCommonDensity(materialName)
-
-        return Atten.fromText(Atten._builtInAttenText(materialName), density, BuiltInAttenEnergyUnit)
-
-    @staticmethod
-    def fromText(attenText: str, density: float, energyUnit='MeV'):
-        cripAssert(density > 0, '`density` should > 0.')
-        rho = density
-
-        # split attenText into list, and ignore all lines starting with non-digit
-        content = list(
-            filter(lambda y: len(y) > 0 and str.isdigit(y[0]),
-                   list(map(lambda x: x.strip(),
-                            attenText.replace('\r\n', '\n').split('\n')))))
-
-        def procAttenLine(line: str):
-            tup = tuple(map(float, re.split(r'\s+', line)))
-            cripAssert(inArray(len(tup), [2, 3]), f'Invalid line in attenText: {line}')
-            energy, muDivRho = tuple(map(float, re.split(r'\s+', line)))[0:2]
-            return energy, muDivRho
-
-        content = np.array(list(map(procAttenLine, content)), dtype=DefaultFloatDType)
-
-        energy, muDivRho = content.T
-        energy = cvtEnergyUnit(energy, energyUnit, DefaultEnergyUnit)  # keV
-
-        # perform log-domain interpolation to fill in `DiagEnergyRange`
-        interpEnergy = np.log(DiagEnergyRange[1:])  # avoid log(0)
-        interpMuDivRho = np.interp(interpEnergy, np.log(energy), np.log(muDivRho))
-
-        # now we have mu for every energy in `DiagEnergyRange`.
-        mu = np.exp(interpMuDivRho) * rho  # cm-1
-        mu = cvtMuUnit(mu, 'cm-1', DefaultMuUnit)  # mm-1
-        mu = np.insert(mu, 0, 0, axis=0)  # prepend energy = 0
-
-        return Atten(mu, rho)
-
-    @staticmethod
-    def fromMuArray(muArray: NDArray, rho: Or[float, None] = None):
-        return Atten(muArray, rho)
-
-    @staticmethod
-    def fromFile(path: str, rho: float, energyUnit='MeV'):
-        '''
-            Construct a new material from file where first column is energy while second
-            is \\mu / \\rho.
-        '''
-        atten = readFileText(path)
-
-        return Atten.fromText(atten, rho, energyUnit)
-
-
-Material = Atten
-WaterAtten = Atten.fromBuiltIn('Water')
-
-
-def calcMu(atten: Atten, spec: Spectrum, energyConversion: str) -> float:
-    '''
-        Calculate the LAC \mu value (mm-1) of certain atten under a specific spectrum.
-        energyConversion determines the energy conversion efficiency of the detector,
-        can be "PCD" (Photon Counting), "EID" (Energy Integrating)
-    '''
-    cripAssert(inArray(energyConversion, ['PCD', 'EID']), f'Invalid energyConversion: {energyConversion}')
-
-    mus = atten.mu
-    eff = {'PCD': 1, 'EID': np.array(DiagEnergyRange)}[energyConversion]
-
-    return np.sum(spec.omega * eff * mus) / np.sum(spec.omega * eff)
-
-
-def calcAttenedSpec(spec: Spectrum, attens: Or[Atten, List[Atten]], Ls: Or[float, List[float]]) -> Spectrum:
-    '''
-        Calculate the attenuated spectrum using polychromatic Beer-Lambert law. Supports multiple materials.
-
-        I.e., `\\Omega(E) \\exp (- \\mu(E) L) through all E`. L in mm.
-    '''
-    if isType(attens, Atten):
-        attens = [attens]
-    if isType(Ls, float):
-        Ls = [Ls]
-    cripAssert(len(attens) == len(Ls), 'atten should have same length as L.')
-
-    N = len(attens)
-    omega = np.array(spec.omega, copy=True)
-    for i in range(N):  # materials
-        atten = attens[i]
-        L = Ls[i]
-        for E in DiagEnergyRange:  # energies
-            omega[E] *= np.exp(-atten.mu[E] * L)
-
-    return Spectrum(omega, spec.unit)
-
-
-def calcPostLog(spec: Spectrum, atten: Or[Atten, List[Atten]], L: Or[float, List[float]]) -> float:
-    '''
-        Calculate post-log value after attenuation of `L` length `atten`. L in mm.
-    '''
-    attenSpec = calcAttenedSpec(spec, atten, L)
-
-    return -np.log(attenSpec.sumOmega / spec.sumOmega)
-
-
-def forwardProjectWithSpectrum(lengths: List[TwoD], materials: List[Atten], spec: Spectrum, energyConversion: str):
-    '''
-        Perform forward projection using `spec`. `lengths` is a list of corresponding length [mm] images 
-        (projection or sinogram) of `materials`. 
-        This function would simulate attenuation and Beam Hardening but no scatter.
-        
-        Set `lengths` and `materials` to empty lists to compute the flat field.
-
-        It's highly recommended to use a monochronmatic spectrum to accelerate if you simulate a lot.
-    '''
-    cripAssert(len(lengths) == len(materials), 'Lengths and materials should correspond.')
-    cripAssert(all([isOfSameShape(lengths[0], x) for x in lengths]), 'Lengths map should have same shape.')
-    cripAssert(energyConversion in ['PCD', 'EID'], 'Invalid energyConversion.')
-
-    efficiency = 1 if energyConversion == 'PCD' else np.array(DiagEnergyRange)
-
-    if len(lengths) == 0:
-        # compute the flat field
-        ones = np.ones_like(lengths[0], dtype=DefaultFloatDType) if len(lengths) > 0 else 1
-        effectiveOmega = spec.omega * efficiency
-
-        return np.sum(effectiveOmega) * ones
-
-    resultShape = lengths[0].shape
-
-    # speed up when it's monochromatic
-    isMono, monoAt = spec.isMonochromatic()
-    if isMono:
-        attenuations = 0.0
-        for length, material in zip(lengths, materials):
-            attenuations += length * material.mu[monoAt]
-
-        attened = spec.omega[monoAt] * np.exp(-attenuations) * (1 if energyConversion == 'PCD' else monoAt
-                                                               )  # the attenuated image
-
-        return attened
-    else:
-        # a[h, w] = [vector of attenuation in that energy bin]
-        attenuations = np.zeros((*resultShape, DiagEnergyLen), dtype=DefaultFloatDType)
-        for length, material in zip(lengths, materials):
-            attenuations += np.outer(length, material.mu).reshape((*resultShape, DiagEnergyLen))
-
-        attened = spec.omega * np.exp(-attenuations) * efficiency  # the attenuated image
-
-    return np.sum(attened, axis=-1)
-
-
-def brewPowderSolution(solute: Atten,
-                       solvent: Atten,
-                       concentration: float,
-                       concentrationUnit='mg/mL',
-                       rhoSolution: Or[float, None] = None) -> Atten:
-    '''
-        Generate the Atten of powder solution with certain concentration (mg/mL by default).
-    '''
-    cripAssert(inArray(concentrationUnit, ['mg/mL', 'g/mL']), f'Invalid concentration unit: {concentrationUnit}')
-
-    concentration = cvtConcentrationUnit(concentration, concentrationUnit, 'g/mL')
-    mu = solvent.mu + (solute.mu / solute.rho) * concentration
-    atten = Atten.fromMuArray(mu, rhoSolution)
-
-    return atten
-
-
-def calcContrastHU(contrast: Atten, spec: Spectrum, energyConversion: str, base: Atten = WaterAtten):
-    '''
-        Calculate HU difference resulted by contrast.
-    '''
-    cripAssert(energyConversion in ['EID', 'PCD'], 'Invalid energyConversion.')
-
-    _calcMu = lambda atten: calcMu(atten, spec, energyConversion)
-
-    muWater = _calcMu(WaterAtten)
-    if base is not WaterAtten:
-        muBase = _calcMu(base)
-    else:
-        muBase = muWater
-    muContrast = _calcMu(contrast)
-
-    contrastHU = muToHU(muContrast, muWater) - muToHU(muBase, muWater)
-
-    return contrastHU
-
-
-def calcPathLength(thickness: float, SID: float, detH: int, detW: int, detElementSize: float):
-    '''
-        Calculate the X-ray peneration pathlength of an cuboid object based on geometry.
-        SID is source-isocenter distance. Currently no offset can be assumed.
-    '''
-    detCenter = (detW / 2, detH / 2)
-    r, c = np.meshgrid(np.arange(detH), np.arange(detW))
-    coords = np.array((r.flatten(), c.flatten()), dtype=np.float32).T
-
-    offcenter = coords - np.array(detCenter)
-    offcenter = np.abs(offcenter) * detElementSize
-    offcenterDist = np.sqrt(np.sum(offcenter**2, axis=1))
-
-    theta = np.arctan(offcenterDist / SID)
-    rayIntersect = thickness / np.cos(theta)
-    rayIntersect = rayIntersect.reshape((detW, detH)).T
-
-    return rayIntersect
+'''
+    Physics module of crip.
+
+    https://github.com/SEU-CT-Recon/crip
+'''
+
+import json
+import re
+import numpy as np
+from os import path
+import periodictable as pt
+import enum
+
+from ._typing import *
+from .utils import *
+from .io import listDirectory
+from .postprocess import muToHU
+
+## Constants ##
+
+DiagEnergyLow = 0  # [keV] Lowest energy of diagnostic X-ray
+DiagEnergyHigh = 150  # [keV] Highest energy of diagnostic X-ray
+DiagEnergyRange = range(DiagEnergyLow, DiagEnergyHigh + 1)  # Diagonstic energy range, [0, 150] keV
+DiagEnergyLen = DiagEnergyHigh - DiagEnergyLow + 1
+NA = 6.02214076e23  # Avogadro's number
+
+# Alias for built-in materials
+AttenAliases = {
+    'Gold': 'Au',
+    'Carbon': 'C',
+    'Copper': 'Cu',
+    'Iodine': 'I',
+    'H2O': 'Water',
+    'Gadolinium': 'Gd',
+}
+
+
+class EnergyConversion(enum.Enum):
+    ''' Energy conversion efficiency marker of the detector.
+    '''
+    EID = 'EID'  # Energy-Integrating Detector
+    PCD = 'PCD'  # Photon-Counting Detector
+
+
+def getCommonDensity(materialName: str):
+    ''' Get the common density of a material [g/cm^3] from built-in dataset.
+    '''
+    db = json.loads(readFileText(path.join(getAsset('atten'), 'density.json')))
+
+    if materialName in AttenAliases:
+        materialName = AttenAliases[materialName]
+    cripAssert(materialName in db, f'Material not found in density dataset: {materialName}')
+
+    return db[materialName]
+
+
+class Spectrum:
+
+    def __init__(self, omega: NDArray, unit='keV'):
+        ''' Construct a Spectrum object with omega array describing every energy bin in DiagEnergyRange.
+            To access omega of certain energy E [keV], use `spec.omega[E]`.
+        '''
+        cripAssert(
+            len(omega) == DiagEnergyLen,
+            f'omega array should length of DiagEnergyLen ({DiagEnergyLen}), but got {len(omega)}.')
+        cripAssert(unit in EnergyUnits, f'Invalid unit: {unit}.')
+
+        self.unit = unit
+        self.omega = np.array(omega, dtype=DefaultFloatDType)
+        self.sumOmega = np.sum(self.omega)
+
+    def isMonochromatic(self):
+        ''' Test if the spectrum is monochromatic. If so, return True and the energy.
+        '''
+        at = -1
+        for i in DiagEnergyRange:
+            if self.omega[i] > 0:
+                if at != -1:
+                    return False, None
+                at = i
+
+        return True, at
+
+    @staticmethod
+    def fromText(specText: str, unit='keV'):
+        ''' Parse spectrum text into `Spectrum` object.
+            The text should be in the format of `<energy> <omega>`, one pair per line.
+            Leading lines starting with non-digit will be ignored.
+            All `<energy>` should be in ascending order and continous by 1 keV and inside `DiagEnergyRange`.
+            Recommend you to end the last line with `omega=-1` to indicate the end of spectrum.
+        '''
+        cripAssert(unit in EnergyUnits, f'Invalid unit: {unit}.')
+        omega = np.zeros(DiagEnergyLen, dtype=DefaultFloatDType)
+
+        # split content into list, and ignore all lines starting with non-digit
+        content = list(
+            filter(lambda y: len(y) > 0 and str.isdigit(y[0]),
+                   list(map(lambda x: x.strip(),
+                            specText.replace('\r\n', '\n').split('\n')))))
+
+        # process each line
+        def proc1(line: str):
+            tup = tuple(map(float, re.split(r'\s+', line)))
+            cripAssert(len(tup) == 2, f'Invalid line in spectrum: {line}.')
+
+            return tup  # (energy, omega)
+
+        # parse the spectrum text to get provided omega array
+        content = np.array(list(map(proc1, content)), dtype=DefaultFloatDType)
+        specEnergy, specOmega = content.T
+        specEnergy = convertEnergyUnit(specEnergy, unit, DefaultEnergyUnit)
+        cripAssert(np.all(np.diff(specEnergy) == 1), 'Energy should be in ascending order and continous by 1 keV.')
+        specOmega[specOmega < 0] = 0
+        startEnergy, cutOffEnergy = int(specEnergy[0]), int(specEnergy[-1])
+        cripAssert(startEnergy in DiagEnergyRange, f'startEnergy is out of DiagEnergyRange: {startEnergy} keV')
+        cripAssert(cutOffEnergy in DiagEnergyRange, f'cutOffEnergy is out of DiagEnergyRange: {cutOffEnergy} keV')
+
+        # fill omega array
+        omega[startEnergy:cutOffEnergy + 1] = specOmega[:]
+
+        return Spectrum(omega, unit)
+
+    @staticmethod
+    def fromFile(path: str, unit='keV'):
+        ''' Construct a Spectrum object from spectrum file whose format follows `fromText`.
+        '''
+        return Spectrum.fromText(readFileText(path), unit)
+
+    @staticmethod
+    def monochromatic(at: int, unit='keV', omega=10**5):
+        ''' Construct a monochromatic spectrum at `at`.
+        '''
+        text = '{} {}\n{} -1'.format(str(at), str(omega), str(at + 1))
+
+        return Spectrum.fromText(text, unit)
+
+
+class Atten:
+
+    def __init__(self, muArray: NDArray, density: Or[None, float] = None) -> None:
+        ''' Construct an Atten object with mu array describing every LAC for energy bins in DiagEnergyRange.
+            The density is in [g/cm^3]. To access mu [mm-1] of certain energy E [keV], use `atten.mu[E]`.
+        '''
+        cripAssert(len(muArray) == DiagEnergyLen, f'muArray should have length of {DiagEnergyLen} energy bins.')
+        if density is not None:
+            cripAssert(density > 0, 'Density should be positive.')
+
+        self.mu = muArray
+        self.rho = density
+        self.attenText = ''
+        self.energyUnit = 'keV'
+
+    @staticmethod
+    def builtInAttenList() -> List[str]:
+        ''' Get all built-in material names and aliases.
+        '''
+        attenListPath = path.join(getAsset('atten'), 'data')
+        attenList = list(map(lambda x: x.replace('.txt', ''), listDirectory(attenListPath, style='filename')))
+        attenList.extend(AttenAliases.keys())
+
+        return attenList
+
+    @staticmethod
+    def builtInAttenText(material: str):
+        ''' Get built-in atten file content of `material` from NIST data source.
+        '''
+        if material in AttenAliases:
+            material = AttenAliases[material]
+
+        attenFilePath = path.join(getAsset('atten'), f'data/{material}.txt')
+        cripAssert(path.exists(attenFilePath), f'Atten file for {material} does not exist.')
+
+        return readFileText(attenFilePath)
+
+    @staticmethod
+    def fromBuiltIn(material: str, density: Or[float, None] = None):
+        ''' Get a built-in atten object for `material`.
+            Call `builtInAttenList` to inspect all available materials.
+            The density is in [g/cm^3], and will be automatically filled with common value if not provided.
+        '''
+        if material in AttenAliases:
+            material = AttenAliases[material]
+
+        if density is None:
+            density = getCommonDensity(material)
+
+        return Atten.fromText(Atten.builtInAttenText(material), density, BuiltInAttenEnergyUnit)
+
+    @staticmethod
+    def fromText(attenText: str, density: float, energyUnit='MeV'):
+        ''' Parse atten text into `Atten` object. Interpolation will be performed to fill `DiagEnergyRange`.
+            The text should be in the format of `<energy> <mu/density>` one pair per line,
+            or `<energy> <mu/density> <mu_en/density>` where the second column will be used.
+            Leading lines starting with non-digit will be ignored.
+        '''
+        rho = density
+
+        # split attenText into list, and ignore all lines starting with non-digit
+        content = list(
+            filter(lambda y: len(y) > 0 and str.isdigit(y[0]),
+                   list(map(lambda x: x.strip(),
+                            attenText.replace('\r\n', '\n').split('\n')))))
+
+        # process each line
+        def proc1(line: str):
+            tup = tuple(map(float, re.split(r'\s+', line)))
+            cripAssert(len(tup) in [2, 3], f'Invalid line in attenText: {line}.')
+            energy, muDivRho = tuple(map(float, re.split(r'\s+', line)))[0:2]
+
+            return energy, muDivRho
+
+        # parse the atten text to get provided mu array
+        content = np.array(list(map(proc1, content)), dtype=DefaultFloatDType)
+        energy, muDivRho = content.T
+        energy = convertEnergyUnit(energy, energyUnit, DefaultEnergyUnit)  # keV
+
+        # perform log-domain interpolation to fill in `DiagEnergyRange`
+        interpEnergy = np.log(DiagEnergyRange[1:])  # avoid log(0)
+        interpMuDivRho = np.interp(interpEnergy, np.log(energy), np.log(muDivRho))
+
+        # now we have mu for every energy in `DiagEnergyRange`.
+        mu = np.exp(interpMuDivRho) * rho  # cm-1
+        mu = convertMuUnit(mu, 'cm-1', DefaultMuUnit)  # mm-1
+        mu = np.insert(mu, 0, 0, axis=0)  # prepend for E=0
+
+        return Atten.fromMuArray(mu, rho)
+
+    @staticmethod
+    def fromMuArray(muArray: NDArray, density: Or[float, None] = None):
+        ''' Construct a new material from mu array for every energy in `DiagEnergyRange`.
+            The density is in [g/cm^3].
+        '''
+        return Atten(muArray, density)
+
+    @staticmethod
+    def fromFile(path: str, density: float, energyUnit='MeV'):
+        ''' Construct a new material from file where the format follows `fromText`.
+        '''
+        return Atten.fromText(readFileText(path), density, energyUnit)
+
+
+WaterAtten = Atten.fromBuiltIn('Water')
+
+
+def computeMu(atten: Atten, spec: Spectrum, energyConversion: EnergyConversion) -> float:
+    ''' Calculate the LAC (mu) [mm-1] for certain Atten under a Spectrum.
+        `energyConversion` determines the energy conversion efficiency of the detector.
+    '''
+    mus = atten.mu
+    eff = {
+        EnergyConversion.PCD: 1,
+        EnergyConversion.EID: np.array(DiagEnergyRange),
+    }[energyConversion]
+
+    return np.sum(spec.omega * eff * mus) / np.sum(spec.omega * eff)
+
+
+def computeAttenedSpectrum(spec: Spectrum, attens: Or[Atten, List[Atten]], Ls: Or[float, List[float]]) -> Spectrum:
+    ''' Calculate the spectrum after attenuation through `attens` with thickness `Ls` [mm]
+        using Beer-Lambert law.
+    '''
+    if isType(attens, Atten):
+        attens = [attens]
+    if isType(Ls, float):
+        Ls = [Ls]
+    cripAssert(len(attens) == len(Ls), '`attens` should be paired with `Ls`.')
+
+    N = len(attens)
+    omega = np.array(spec.omega, copy=True)
+    for i in range(N):
+        atten, L = attens[i], Ls[i]
+        for E in DiagEnergyRange:  # energies
+            omega[E] *= np.exp(-atten.mu[E] * L)
+
+    return Spectrum(omega, spec.unit)
+
+
+def forwardProjectWithSpectrum(lengths: List[TwoD], materials: List[Atten], spec: Spectrum, energyConversion: str):
+    ''' Perform forward projection using `spec`. `lengths` is a list of corresponding length [mm] images 
+        (projection or sinogram) of `materials`. 
+        This function would simulate attenuation and Beam Hardening but no scatter.
+        
+        Set `lengths` and `materials` to empty lists to compute the flat field.
+
+        It's highly recommended to use a monochronmatic spectrum to accelerate if you simulate a lot.
+    '''
+    cripAssert(len(lengths) == len(materials), 'Lengths and materials should correspond.')
+    cripAssert(all([isOfSameShape(lengths[0], x) for x in lengths]), 'Lengths map should have same shape.')
+    cripAssert(energyConversion in ['PCD', 'EID'], 'Invalid energyConversion.')
+
+    efficiency = 1 if energyConversion == 'PCD' else np.array(DiagEnergyRange)
+
+    if len(lengths) == 0:
+        # compute the flat field
+        ones = np.ones_like(lengths[0], dtype=DefaultFloatDType) if len(lengths) > 0 else 1
+        effectiveOmega = spec.omega * efficiency
+
+        return np.sum(effectiveOmega) * ones
+
+    resultShape = lengths[0].shape
+
+    # speed up when it's monochromatic
+    isMono, monoAt = spec.isMonochromatic()
+    if isMono:
+        attenuations = 0.0
+        for length, material in zip(lengths, materials):
+            attenuations += length * material.mu[monoAt]
+
+        attened = spec.omega[monoAt] * np.exp(-attenuations) * (1 if energyConversion == 'PCD' else monoAt
+                                                               )  # the attenuated image
+
+        return attened
+    else:
+        # a[h, w] = [vector of attenuation in that energy bin]
+        attenuations = np.zeros((*resultShape, DiagEnergyLen), dtype=DefaultFloatDType)
+        for length, material in zip(lengths, materials):
+            attenuations += np.outer(length, material.mu).reshape((*resultShape, DiagEnergyLen))
+
+        attened = spec.omega * np.exp(-attenuations) * efficiency  # the attenuated image
+
+    return np.sum(attened, axis=-1)
+
+
+def brewPowderSolution(solute: Atten,
+                       solvent: Atten,
+                       concentration: float,
+                       concentrationUnit='mg/mL',
+                       rhoSolution: Or[float, None] = None) -> Atten:
+    ''' Generate the `Atten` of ideal powder solution with certain concentration.
+    '''
+    cripAssert(concentrationUnit in ConcentrationUnits, f'Invalid concentration unit: {concentrationUnit}.')
+
+    concentration = convertConcentrationUnit(concentration, concentrationUnit, 'g/mL')
+    mu = solvent.mu + (solute.mu / solute.rho) * concentration
+    atten = Atten.fromMuArray(mu, rhoSolution)
+
+    return atten
+
+
+def computeContrastHU(contrast: Atten,
+                      spec: Spectrum,
+                      energyConversion: EnergyConversion,
+                      base: Atten = WaterAtten) -> float:
+    ''' Compute the HU difference caused by contrast.
+    '''
+    _calcMu = lambda atten: computeMu(atten, spec, energyConversion)
+
+    muWater = _calcMu(WaterAtten)
+    muContrast = _calcMu(contrast)
+    if base is not WaterAtten:
+        muBase = _calcMu(base)
+    else:
+        muBase = muWater
+
+    return muToHU(muContrast, muWater) - muToHU(muBase, muWater)
+
+
+def computePathLength(thickness: float, sod: float, detH: int, detW: int, detElementSize: float) -> NDArray:
+    ''' Compute the ray peneration pathlength for each detector element using a cuboid object with `thickness`.
+        `sod` is the Source-Object Distance. `(detH, detW)` is the detector size [pixel].
+        `detElementSize` is the element size of detector.
+        All length units are recommended to be [mm]. Currently no object offset can be assumed.
+    '''
+    detCenter = (detW / 2, detH / 2)
+    r, c = np.meshgrid(np.arange(detH), np.arange(detW))
+    coords = np.array((r.flatten(), c.flatten()), dtype=np.float32).T
+
+    offcenter = coords - np.array(detCenter)
+    offcenter = np.abs(offcenter) * detElementSize
+    offcenterDist = np.sqrt(np.sum(offcenter**2, axis=1))
+
+    theta = np.arctan(offcenterDist / sod)
+    rayIntersect = thickness / np.cos(theta)
+    rayIntersect = rayIntersect.reshape((detW, detH)).T
+
+    return rayIntersect
+
+
+def atomsFromMolecule(molecule: str) -> Dict[str, int]:
+    ''' Parse the molecule string to get the atoms and their counts.
+        e.g. `'H2 O1' -> {'H': 2, 'O': 1}`
+    '''
+    atoms = {}
+    for part in molecule.split(' '):
+        count = ''.join(filter(str.isdigit, part))
+        element = ''.join(filter(str.isalpha, part))
+        atoms[element] = int(count)
+
+    return atoms
+
+
+def zeffTheoretical(molecule: str, m=2.94) -> float:
+    ''' Compute the eheoretical effective atomic number (Zeff) of a molecule using the power law with parameter `m`.
+        `molecule` is parsed by `atomsFromMolecule`.
+    '''
+    atoms = atomsFromMolecule(molecule)
+    totalElectrons = 0
+    for atom in atoms:
+        totalElectrons += atoms[atom] * pt.elements.symbol(atom).number
+
+    sumUnderSqrt = 0
+    for atom in atoms:
+        Z = pt.elements.symbol(atom).number  # atomic number
+        f = atoms[atom] * Z / totalElectrons  # fraction
+        sumUnderSqrt += f * (Z**m)
+
+    return sumUnderSqrt**(1 / m)
+
+
+def zeffExperimental(a1: float, a2: float, rhoe1: float, rhoe2: float, zeff1: float, zeff2: float, m=2.94):
+    ''' Compute the experimental effective atomic number (Zeff) from Dual-Energy Two-Material decomposition
+        using the power law with parameter `m`. `(a1, a2)` are material decomposition coefficients.
+        `(rhoe1, rhoe2)` are electron densities of material bases.
+        `(zeff1, zeff2)` are effective atomic numbers of material bases.
+    '''
+    n1 = a1 * rhoe1 * zeff1**m
+    n2 = a2 * rhoe2 * zeff2**m
+    d1 = a1 * rhoe1
+    d2 = a2 * rhoe2
+
+    return ((n1 + n2) / (d1 + d2))**(1 / m)
```

### Comparing `crip-1.7.9/crip/plot.py` & `crip-1.8.0/crip/plot.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,223 +1,237 @@
-'''
-    Figure artist module of crip.
-
-    https://github.com/z0gSh1u/crip
-'''
-
-import cv2
-import numpy as np
-from matplotlib import font_manager
-import matplotlib.pyplot as plt
-import matplotlib.figure
-import matplotlib.patches
-import matplotlib.axes
-from mpl_toolkits.axes_grid1 import ImageGrid
-from ._typing import *
-from .utils import cripAssert, is1D, isInt, cripWarning
-from .physics import Spectrum, DiagEnergyRange, Atten
-from .shared import resize
-
-__all__ = ['smooth', 'window', 'average', 'addFont', 'fontdict', 'zoomIn', 'plotSpectrum', 'makeImageGrid', 'windowFullRange']
-
-
-def smooth(data: NDArray, winSize: int = 5):
-    '''
-        Smooth an 1D array by moving averaging window. This name follows MATLAB.
-
-        The implementation is from https://stackoverflow.com/questions/40443020
-    '''
-    cripAssert(is1D(data), '`data` should be 1D array.')
-    cripAssert(isInt(winSize) and winSize % 2 == 1, '`winSize` should be odd integer.')
-
-    out0 = np.convolve(data, np.ones(winSize, dtype=int), 'valid') / winSize
-    r = np.arange(1, winSize - 1, 2)
-    start = np.cumsum(data[:winSize - 1])[::2] / r
-    stop = (np.cumsum(data[:-winSize:-1])[::2] / r)[::-1]
-    return np.concatenate((start, out0, stop))
-
-
-def window(img: TwoOrThreeD, win: Or[Tuple[int], Tuple[float]], style: str = 'lr', normalize: Or[str, None] = None):
-    '''
-        Window `img` using `win` (ww, wl) with style 'wwwl' or (left, right) with style 'lr'.
-        Set `normalize` to '0255' to convert to 8-bit image, or '01' to [0, 1] float image.
-    '''
-    cripAssert(len(win) == 2, '`win` should have length of 2.')
-    cripAssert(style in ['wwwl', 'lr'], "`style` should be 'wwwl' or 'lr'")
-
-    if style == 'wwwl':
-        ww, wl = win
-        l = wl - ww / 2
-        r = l + ww
-    elif style == 'lr':
-        l, r = win
-
-    res = img.copy()
-    res[res > r] = r
-    res[res < l] = l
-
-    if normalize == '0255':
-        res = cv2.normalize(res, None, 0, 255, cv2.NORM_MINMAX).astype(np.uint8)
-    elif normalize == '01':
-        res = (res - l) / (r - l)
-
-    return res
-
-
-def windowFullRange(img: TwoOrThreeD, normalize='01'):
-    '''Window `img` using full dynamic range of pixel values.
-    '''
-    return window(img, (np.max(img), np.min(img)), 'lr', normalize)
-
-
-def addFont(dir_: str):
-    '''
-        Add font files under `dir` to matplotlib.
-    '''
-    for file in font_manager.findSystemFonts(fontpaths=[dir_]):
-        font_manager.fontManager.addfont(file)
-
-
-def average(imgs: ThreeD, i: int, r: int):
-    '''
-        Average along `channel` dimension [i - r, i + r].
-        Use for example, show CT slices smoother.
-    '''
-    return np.mean(imgs[i - r:i + r], axis=0)
-
-
-def zoomIn(img, row, col, h, w):
-    '''
-        Crop a patch. (row, col) determines the left-top point. (h, w) gives height and width.
-    '''
-    return img[row:row + h, col:col + w]
-
-
-def stddev(img, row, col, h, w):
-    '''
-        Compute the standard deviation of a image crop.
-        (row, col) determines the left-top point. (h, w) gives height and width.
-    '''
-    return np.std(zoomIn(img, row, col, h, w))
-
-
-def fontdict(family, weight, size):
-    return {'family': family, 'weight': weight, 'size': size}
-
-
-def makeImageGrid(subimages: List[TwoD],
-                  colTitles: List[str],
-                  rowTitles: List[str],
-                  preproc=None,
-                  fontdict=None,
-                  crops=None,
-                  cropLoc='bottom right',
-                  cropSize=96 * 2,
-                  arrows=None,
-                  arrowLen=24):
-    # determine the number of rows and columns
-    ncols = len(colTitles)
-    nrows = len(rowTitles)
-    cripAssert(len(subimages) == ncols * nrows, 'Number of subimages should be equal to ncols * nrows.')
-    cripAssert(crops is None or len(crops) == nrows, 'Number of crops should be equal to nrows.')
-    cripAssert(arrows is None or len(arrows) == nrows, 'Number of arrows should be equal to nrows.')
-
-    # create the figure
-    fig = plt.figure(figsize=(ncols * 2, nrows * 2))
-    grid = ImageGrid(fig, 111, nrows_ncols=(nrows, ncols), axes_pad=0)
-
-    # apply the preprocessor
-    if preproc:
-        subimages = list(map(lambda ix: preproc(*ix), list(enumerate(subimages))))
-
-    def overlayPatch(img, patch, loc):
-        if loc == 'bottom left':
-            img[-patch.shape[0]:, :patch.shape[1]] = patch
-            box = matplotlib.patches.Rectangle((0, img.shape[0] - patch.shape[0]),
-                                               patch.shape[1],
-                                               patch.shape[0],
-                                               linewidth=1,
-                                               edgecolor='yellow',
-                                               facecolor='none')
-            return box
-        else:
-            raise 'Invalid cropLoc, not in `bottom left`.'
-
-    # display the subimages
-    cur = 0
-    for ax, img in zip(grid, subimages):
-        # remove the ticks and spines
-        ax.get_xaxis().set_ticks([])
-        ax.get_yaxis().set_ticks([])
-        list(map(lambda x: x.set_visible(False), ax.spines.values()))
-
-        # prepare the image crop
-        box = None
-        if crops is not None and crops[cur // ncols]:
-            r, c, hw = crops[cur // ncols]
-            patch = resize(zoomIn(img, r, c, hw, hw), (cropSize, cropSize))
-            box = overlayPatch(img, patch, cropLoc)
-
-        # display the image
-        ax.imshow(img, cmap='gray', vmin=0, vmax=1)
-
-        # display the crop box
-        box and ax.add_patch(box)
-        if box and cur % ncols == 0:
-            r, c, hw = crops[cur // ncols]
-            box = matplotlib.patches.Rectangle((c, r), hw, hw, linewidth=0.8, edgecolor='yellow', facecolor='none')
-            ax.add_patch(box)
-
-        # display the arrow
-        if arrows is not None and arrows[cur // ncols]:
-            r, c = arrows[cur // ncols]
-            ax.arrow(c + arrowLen, r - arrowLen, -arrowLen, +arrowLen, color='yellow', head_width=10)
-
-        # display the column titles
-        if cur < len(colTitles):
-            ax.set_title(colTitles[cur], loc='center', fontdict=fontdict)
-        cur += 1
-
-    # display the row titles
-    for i in range(nrows):
-        grid[ncols * i].set_ylabel(rowTitles[i], fontdict=fontdict)
-
-    return fig
-
-
-def plotSpectrum(ax: matplotlib.axes.Axes, spec: Spectrum):
-    '''
-        Plot the spectrum in `ax`. Example
-        ```
-        fig = plt.figure()
-        ax = fig.add_subplot(111)
-        plotSpectrum(ax, spec)
-    '''
-    energies = DiagEnergyRange
-    omega = spec.omega
-
-    ax.plot(energies, omega, 'k')
-    ax.set_xlabel('Energy (keV)')
-    ax.set_ylabel('Omega')
-
-
-def plotMu(ax: matplotlib.axes.Axes, atten: Atten, startEnergy: int = 1, logScale=True):
-    '''
-        Plot the LACs of `atten` from `startEnergy` keV in ax in `logScale` if true.
-    '''
-    x = list(DiagEnergyRange)[startEnergy:]
-    ax.plot(x, atten.mu[startEnergy:])
-
-    if logScale:
-        ax.set_yscale('log')
-
-    ax.xlabel('Energy (keV)')
-    ax.ylabel('LAC (1/mm)')
-
-
-def savefigTight(fig, path, dpi=200, pad=0.05):
-    fig.tight_layout()
-    fig.savefig(path, dpi=dpi, bbox_inches='tight', pad_inches=pad)
-
-
-def meanstd(x):
-    return np.mean(x), np.std(x)
+'''
+    Figure artist module of crip.
+
+    https://github.com/z0gSh1u/crip
+'''
+
+import cv2
+import numpy as np
+import matplotlib.pyplot as plt
+import matplotlib.figure
+import matplotlib.patches
+import matplotlib.axes
+from mpl_toolkits.axes_grid1 import ImageGrid as MplImageGrid
+
+from ._typing import *
+from .utils import *
+from .physics import Spectrum, DiagEnergyRange, Atten
+from .shared import resizeTo
+
+
+def smooth1D(data: NDArray, winSize: int = 5) -> NDArray:
+    ''' Smooth an 1D array using moving average window.
+        The implementation is from https://stackoverflow.com/questions/40443020
+    '''
+    cripAssert(is1D(data), '`data` should be 1D array.')
+    cripAssert(isInt(winSize) and winSize % 2 == 1, '`winSize` should be odd positive integer.')
+
+    out0 = np.convolve(data, np.ones(winSize, dtype=int), 'valid') / winSize
+    r = np.arange(1, winSize - 1, 2)
+    start = np.cumsum(data[:winSize - 1])[::2] / r
+    stop = (np.cumsum(data[:-winSize:-1])[::2] / r)[::-1]
+
+    return np.concatenate((start, out0, stop))
+
+
+# def zsmooth(imgs: ThreeD, r: int):
+#     ''' Average along `C` dimension [i - r, i + r].
+#     '''
+#     return np.mean(imgs[i - r:i + r], axis=0)
+
+
+def window(img: TwoOrThreeD,
+           win: Tuple[float, float],
+           style: str = 'lr',
+           normalize: Or[str, None] = None) -> TwoOrThreeD:
+    ''' Window `img` using `win` (WW, WL) with style `wwwl` or (left, right) with style `lr`.
+        Set `normalize` to `0255` to convert to 8-bit image, or `01` to [0, 1] float image.
+    '''
+    cripAssert(len(win) == 2, '`win` should have length of 2.')
+    cripAssert(style in ['wwwl', 'lr'], "`style` should be 'wwwl' or 'lr'")
+
+    if style == 'wwwl':
+        ww, wl = win
+        l = wl - ww / 2
+        r = l + ww
+    elif style == 'lr':
+        l, r = win
+
+    res = asFloat(img.copy())
+    res[res > r] = r
+    res[res < l] = l
+
+    if normalize == '0255':
+        res = cv2.normalize(res, None, 0, 255, cv2.NORM_MINMAX).astype(np.uint8)
+    elif normalize == '01':
+        res = (res - l) / (r - l)
+
+    return res
+
+
+def windowFullRange(img: TwoOrThreeD, normalize='01') -> TwoOrThreeD:
+    ''' Window `img` using its full dynamic range of pixel values.
+    '''
+    return window(img, (np.max(img), np.min(img)), 'lr', normalize)
+
+
+def zoomIn(img: TwoD, row: int, col: int, h: int, w: int) -> TwoD:
+    ''' Crop a patch. `(row, col)` determines the left-top point. `(h, w)` gives height and width.
+    '''
+    return img[row:row + h, col:col + w]
+
+
+def stddev(img: TwoD) -> float:
+    ''' Compute the standard deviation of a image crop.
+        `(row, col)` determines the left-top point. (h, w) gives height and width.
+    '''
+    return np.std(img)
+
+
+def meanstd(x: Any) -> Tuple[float, float]:
+    ''' Compute the mean and standard deviation of `x`.
+    '''
+    return np.mean(x), np.std(x)
+
+
+def fontdict(family, weight, size):
+    return {'family': family, 'weight': weight, 'size': size}
+
+
+class ImageGrid:
+    subimgs: List[TwoD]
+    nrow: int
+    ncol: int
+    fig: matplotlib.figure.Figure
+    grid: MplImageGrid
+
+    # titles
+    rowTitles: List[str] = None
+    colTitles: List[str] = None
+    # preprocessor
+    preprocessor: Callable = None
+    # fontdict
+    fontdict: Dict = None
+    # crops
+    crops: List[Tuple[int, int, int]] = None
+    cropLoc: str = 'bottom left'
+    cropSize: int = 96 * 2
+
+    def __init__(self, subimgs: List[TwoD], nrow: int, ncol: int) -> None:
+        ''' Initialize the ImageGrid with `subimgs` in `nrow` * `ncol` layout.
+        '''
+        self.subimgs = subimgs
+        self.nrow = nrow
+        self.ncol = ncol
+        cripAssert(len(subimgs) == nrow * ncol, 'Number of subimages should be equal to `nrow * ncol`.')
+
+    def setTitles(self, rowTitles: List[str], colTitles: List[str]):
+        ''' Set the row and column titles.
+        '''
+        self.rowTitles = rowTitles
+        self.colTitles = colTitles
+
+    def setPreprocessor(self, fn: Callable):
+        ''' Set the preprocessor for the subimages.
+            A preprocessor is a function that takes the index of a subimage and the subimage and returns a new one.
+        '''
+        self.preprocessor = fn
+
+    def setFontdict(self, fontdict: Dict):
+        ''' Set the fontdict for the texts in the figure.
+        '''
+        self.fontdict = fontdict
+
+    def setCrops(self, crops, cropLoc='bottom left', cropSize=96 * 2):
+        self.crops = crops
+        self.cropLoc = cropLoc
+        self.cropSize = cropSize
+
+    def _overlayPatch(self, img, patch, loc):
+        if loc == 'bottom left':
+            img[-patch.shape[0]:, :patch.shape[1]] = patch
+            box = matplotlib.patches.Rectangle((0, img.shape[0] - patch.shape[0]),
+                                               patch.shape[1],
+                                               patch.shape[0],
+                                               linewidth=1,
+                                               edgecolor='yellow',
+                                               facecolor='none')
+            return box
+        else:
+            cripAssert(False, 'Currently only loc at `bottom left` is supported.')
+
+    def fig(self):
+        ''' Execute the plot and return the figure.
+        '''
+        # preprocess the subimages
+        if self.preprocessor is not None:
+            self.subimages = list(map(lambda ix: self.preprocessor(*ix), list(enumerate(self.subimages))))
+
+        # create the figure
+        self.fig = plt.figure(figsize=(self.ncol * 2, self.nrow * 2))
+        self.grid = MplImageGrid(self.fig, 111, nrows_ncols=(self.nrow, self.ncol), axes_pad=0)
+
+        # display the subimages
+        cur = 0
+        for ax, img in zip(self.grid, self.subimages):
+            # remove the ticks and spines
+            ax.get_xaxis().set_ticks([])
+            ax.get_yaxis().set_ticks([])
+            list(map(lambda x: x.set_visible(False), ax.spines.values()))
+
+            # prepare the image crop
+            box = None
+            if self.crops is not None and self.crops[cur // self.ncol]:
+                r, c, hw = self.crops[cur // self.ncol]
+                patch = resizeTo(zoomIn(img, r, c, hw, hw), (self.cropSize, self.cropSize))
+                box = self._overlayPatch(img, patch, self.cropLoc)
+
+            # display the image
+            ax.imshow(img, cmap='gray', vmin=0, vmax=1)
+
+            # display the crop box
+            box and ax.add_patch(box)
+            if box and cur % self.ncol == 0:
+                r, c, hw = self.crops[cur // self.ncol]
+                box = matplotlib.patches.Rectangle((c, r), hw, hw, linewidth=0.8, edgecolor='yellow', facecolor='none')
+                ax.add_patch(box)
+
+            # display the column titles
+            if self.colTitles and cur < len(self.colTitles):
+                ax.set_title(self.colTitles[cur], loc='center', fontdict=fontdict)
+            cur += 1
+
+        # display the row titles
+        if self.rowTitles:
+            for i in range(self.nrows):
+                self.grid[self.ncols * i].set_ylabel(self.rowTitles[i], fontdict=fontdict)
+
+        return self.fig
+
+
+def plotSpectrum(ax: matplotlib.axes.Axes, spec: Spectrum):
+    ''' Plot the spectrum using handler `ax`.
+    '''
+    energies = DiagEnergyRange
+    omega = spec.omega
+
+    ax.plot(energies, omega, 'k')
+    ax.set_xlabel('Energy (keV)')
+    ax.set_ylabel('Omega (a.u.)')
+
+
+def plotMu(ax: matplotlib.axes.Axes, atten: Atten, startEnergy: int = 1, logScale=True):
+    ''' Plot the LACs of `atten` from `startEnergy` keV in ax in `logScale` if true.
+    '''
+    x = list(DiagEnergyRange)[startEnergy:]
+    ax.plot(x, atten.mu[startEnergy:])
+
+    if logScale:
+        ax.set_yscale('log')
+
+    ax.xlabel('Energy (keV)')
+    ax.ylabel('LAC (1/mm)')
+
+
+def savefigTight(fig, path, dpi=200, pad=0.05):
+    fig.tight_layout()
+    fig.savefig(path, dpi=dpi, bbox_inches='tight', pad_inches=pad)
```

### Comparing `crip-1.7.9/crip/preprocess.py` & `crip-1.8.0/crip/preprocess.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,110 +1,97 @@
 '''
     Preprocess module of crip.
 
     https://github.com/SEU-CT-Recon/crip
 '''
 
-__all__ = [
-    'averageProjections', 'flatDarkFieldCorrection', 'projectionsToSinograms', 'sinogramsToProjections', 'padImage',
-    'padSinogram', 'correctBeamHardeningPolynomial', 'injectGaussianNoise', 'injectPoissonNoise', 'binning',
-    'fanToPara', 'correctRingArtifactInProj', 'correctFlatDarkField'
-]
-
 import numpy as np
 import warnings
-
-warnings.simplefilter("ignore", DeprecationWarning)
-
 from scipy.interpolate import interpn
 import cv2
+
 from .shared import *
 from ._typing import *
 from .utils import *
-from .lowdose import injectGaussianNoise, injectPoissonNoise
+
+warnings.simplefilter("ignore", DeprecationWarning)
 
 
 @ConvertListNDArray
-def averageProjections(projections: TwoOrThreeD) -> TwoD:
+def averageProjections(projections: ThreeD) -> TwoD:
+    ''' Average projections along the first axis (views) to get a single projection.
     '''
-        Average projections. For example, to calculate the flat field.
-        Projections can be either `(views, H, W)` shaped numpy array, or
-        `views * (H, W)` Python List.
-    '''
-    cripAssert(is3D(projections), '`projections` should be 3D array.')
-    projections = asFloat(projections)
+    cripAssert(is3D(projections), f'`projections` should be 3D, but got {len(projections.shape)}-D.')
 
+    projections = asFloat(projections)
     res = projections.sum(axis=0) / projections.shape[0]
 
     return res
 
 
 @ConvertListNDArray
-def flatDarkFieldCorrection(projections: TwoOrThreeD,
-                            flat: Or[TwoD, ThreeD, float, None] = None,
-                            dark: Or[TwoD, ThreeD, float] = 0) -> TwoOrThreeD:
-    '''
-        Perform flat field (air) and dark field correction to get post-log value.
-        If `flat` is 3D and `projections` is also 3D, the correction will be performed view by view.
-        I.e., `- log [(X - D) / (F - D)]`. Multi projections accepted.
-        If flat is None, air is estimated using the brightest pixel by default.
+def correctFlatDarkField(projections: TwoOrThreeD,
+                         flat: Or[TwoD, ThreeD, float, None] = None,
+                         dark: Or[TwoD, ThreeD, float] = 0,
+                         fillNaN: Or[float, None] = 0,
+                         fillInf: Or[float, None] = 0) -> TwoOrThreeD:
+    ''' Perform flat field (air) and dark field correction to get post-log projections.
+        I.e., `- log [(X - D) / (F - D)]`.
+        Usually `flat` and `dark` are 2D.
+        If `flat` and `projections` are both 3D, perform view by view.
+        If `flat` is None, estimate it by brightest pixel each view.
     '''
+    if flat is None:
+        cripWarning(False, '`flat` is None. Use the maximum value of each view instead.')
+        flat = np.max(projections, axis=0) * np.ones_like(projections)
+
     sampleProjection = projections if is2D(projections) else projections[0]
 
-    if is2D(flat):
-        cripAssert(isOfSameShape(sampleProjection, flat), '`projection` and `flat` should have same shape.')
-    if is3D(flat):
-        cripAssert(isOfSameShape(projections, flat), '`projection` and `flat` should have same shape.')
-    if is2D(dark):
-        cripAssert(isOfSameShape(sampleProjection, dark), '`projection` and `dark` should have same shape.')
-    if is3D(dark):
-        cripAssert(isOfSameShape(projections, dark), '`projection` and `dark` should have same shape.')
-    if flat is None:
-        cripWarning(False, '`flat` is None. Use the maximum value instead.')
-        flat = np.max(projections)
+    def checkShape(haystack, needle, needleName):
+        cripAssert(
+            isOfSameShape(haystack, needle),
+            f'`projections` and `{needleName}` should have same shape, but got {haystack.shape} and {needle.shape}.')
+
+    checkShape(sampleProjection if is2D(flat) else projections, flat, 'flat')
+    checkShape(sampleProjection if is2D(dark) else projections, dark, 'dark')
 
     numerator = projections - dark
     denominator = flat - dark
-    cripAssert(np.min(numerator > 0), 'Some projections values are not greater than zero.')
-    cripAssert(np.min(denominator > 0), 'Some flat field values are not greater than zero.')
+    cripAssert(np.min(numerator > 0), 'Some `projections` values are not greater than zero after canceling `dark`.')
+    cripAssert(np.min(denominator > 0), 'Some `flat` values are not greater than zero after canceling `dark`.')
 
     res = -np.log(numerator / denominator)
-    res[res == np.inf] = 0
-    res[res == np.nan] = 0
-
-    return res
 
+    if fillInf is not None:
+        res[res == np.inf] = fillInf
+    if fillNaN is not None:
+        res[res == np.nan] = fillNaN
 
-# a recommended alias
-correctFlatDarkField = flatDarkFieldCorrection
+    return res
 
 
 @ConvertListNDArray
 def projectionsToSinograms(projections: ThreeD):
-    '''
-        Permute projections to sinograms by axes swapping `(views, h, w) -> (h, views, w)`.
-
-        Note that the width direction is along detector channels of a row.
+    ''' Permute projections to sinograms by axes swapping `(views, h, w) -> (h, views, w)`.
+        The width direction is along detector channels of a row.
     '''
     cripAssert(is3D(projections), 'projections should be 3D.')
 
     (views, h, w) = projections.shape
     sinograms = np.zeros((h, views, w), dtype=projections.dtype)
     for i in range(views):
         sinograms[:, i, :] = projections[i, :, :]
 
     return sinograms
 
 
 @ConvertListNDArray
 def sinogramsToProjections(sinograms: ThreeD):
-    '''
-        Permute sinograms back to projections by axes swapping `(h, views, w) -> (views, h, w)`.
-
-        Note that the width direction is along detector channels of a row.
+    ''' Permute sinograms back to projections by axes swapping `(h, views, w) -> (views, h, w)`.
+        The width direction is along detector channels of a row.
     '''
     cripAssert(is3D(sinograms), 'projections should be 3D.')
 
     (h, views, w) = sinograms.shape
     projections = np.zeros((views, h, w), dtype=sinograms.dtype)
     for i in range(views):
         projections[i, :, :] = sinograms[:, i, :]
@@ -129,15 +116,15 @@
         'cosine':
             lambda ascend, dot: np.cos(np.linspace(-np.pi / 2, 0, dot) if ascend else np.linspace(0, np.pi / 2, dot)),
         'smoothCosine':
             lambda ascend, dot: 0.5 * np.cos(np.linspace(-np.pi, 0, dot)) + 0.5
             if ascend else 0.5 * np.cos(np.linspace(0, np.pi, dot)) + 0.5
     }
 
-    h, w = getHW(img)
+    h, w = getHnW(img)
     nPadU, nPadR, nPadD, nPadL = padding
     padH = h + nPadU + nPadD
     padW = w + nPadL + nPadR
 
     def decayLR(xPad, w, nPadL, nPadR, decay):
         xPad[:, 0:nPadL] *= decay(True, nPadL)[:]
         xPad[:, w - nPadR:w] *= decay(False, nPadR)[:]
@@ -171,23 +158,14 @@
 
     l, r = padding
 
     return padImage(sgms, (0, r, 0, l), mode, decay)
 
 
 @ConvertListNDArray
-def correctBeamHardeningPolynomial(postlog: TwoOrThreeD, coeffs: Or[Tuple, np.poly1d], bias=True):
-    '''
-        Apply the polynomial (\\mu L vs. PostLog fit) on postlog to perform basic beam hardening correction.
-        `coeffs` can be either `tuple` or `np.poly1d`. Set `bias=True` if your coeffs includes the bias (order 0) term.
-    '''
-    cripAssert(False, 'The implementation of this function is being re-investigating now.')
-
-
-@ConvertListNDArray
 def correctRingArtifactInProj(sgm: TwoOrThreeD, sigma: float, ksize: Or[int, None] = None):
     '''
         Apply the ring artifact correction method in projection domain (input postlog sinogram),
         using gaussian filter in sinogram detector direction [1].
         [1] 李俊江,胡少兴,李保磊等.CT图像环状伪影校正方法[J].北京航空航天大学学报,2007,(11):1378-1382.DOI:10.13700/j.bh.1001-5965.2007.11.020
         https://kns.cnki.net/kcms2/article/abstract?v=xBNwvqFr00JMj5WzBbZMcj9N-kBm9Pi08enuNi8ymtGWVZuwGHdLWwttkgzSivkJSBVk0CVQZxo7DgBmujqhLCaVvvBMoig5RV0B4fDLUnjGQcCPo3O4KfAo4iX4vCwZ&uniplatform=NZKPT&flag=copy
     '''
@@ -207,20 +185,20 @@
 
     return res
 
 
 def fanToPara(sgm: TwoD, gammas: NDArray, betas: NDArray, sid: float, oThetas: Tuple[float],
               oLines: Tuple[float]) -> TwoD:
     '''
-        Re-order Fan-Beam sinogram to Parallel-Beam's.
-        `gammas`: fan angles from min to max [rad], e.g., `arctan(elementOffcenter / SDD)`
-        `betas`: system rotation angles from min to max [rad]
-        `sid`: Source-Isocenter-Distance [mm]
-        `oThetas`: output rotation angle range (min, delta, max) tuple [rad]
-        `oLines`: output detector element physical locations range (min, delta, max) tuple [mm], e.g., `elementOffcenter` array
+        Re-order a Fan-Beam sinogram to Parallel-Beam's.
+        `gammas` is fan angles from min to max [RAD], computed by `arctan(elementOffcenter / SDD)` for each element.
+        `betas` is system rotation angles from min to max [RAD].
+        `sid` is Source-Isocenter-Distance [mm].
+        `oThetas` is output rotation angle range (min, delta, max) tuple [RAD]
+        `oLines` is output detector element physical locations range (min, delta, max) tuple [mm], e.g., `elementOffcenter` array
         ```
                /| <- gamma for detector element X
               / | <- SID
              /  |
         ====X============ <- detector
             ^<--^ <- offcenter
     '''
```

### Comparing `crip-1.7.9/crip/shared.py` & `crip-1.8.0/crip/shared.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,297 +1,290 @@
-'''
-    Shared module of crip.
-
-    https://github.com/SEU-CT-Recon/crip
-'''
-
-__all__ = [
-    'rotate', 'verticalFlip', 'horizontalFlip', 'stackFlip', 'resize', 'gaussianSmooth', 'stackImages', 'splitImages',
-    'binning', 'transpose', 'permute', 'shepplogan', 'fitPolyV1D2', 'fitPolyV2D2', 'applyPolyV1D2', 'applyPolyV2D2'
-]
-
-import numpy as np
-import cv2
-
-from .utils import ConvertListNDArray, cripAssert, getAsset, inArray, is2D, is2or3D, is3D, isInt, isType
-from ._typing import *
-from .io import imreadTiff
-from os import path
-
-
-@ConvertListNDArray
-def rotate(img: TwoOrThreeD, deg: int) -> TwoOrThreeD:
-    '''
-        Rotate the image or each image in a volume by deg [DEG] (multiple of 90) clockwise.
-    '''
-    deg = int(deg % 360)
-    cripAssert(deg % 90 == 0, 'deg should be multiple of 90.')
-
-    k = deg // 90
-    axes = (1, 2) if is3D(img) else (0, 1)
-
-    return np.rot90(img, -k, axes)
-
-
-@ConvertListNDArray
-def verticalFlip(img: TwoOrThreeD, copy=False) -> TwoOrThreeD:
-    '''
-        Vertical flip one image, or each image in a volume.
-
-        Set `copy = True` to get a copy of array, otherwise a view only.
-    '''
-    cripAssert(is2or3D(img), 'img should be 2D or 3D.')
-
-    if copy:
-        return np.array(img[..., ::-1, :], copy=True)
-    else:
-        return img[..., ::-1, :]
-
-
-@ConvertListNDArray
-def horizontalFlip(img: TwoOrThreeD, copy=False) -> TwoOrThreeD:
-    '''
-        Horizontal flip one image, or each image in a volume.
-        
-        Set `copy = True` to get a copy of array, otherwise a view only.
-    '''
-    cripAssert(is2or3D(img), 'img should be 2D or 3D.')
-
-    if copy:
-        return np.array(img[..., ::-1], copy=True)
-    else:
-        return img[..., ::-1]
-
-
-@ConvertListNDArray
-def stackFlip(img: ThreeD, copy=False) -> ThreeD:
-    '''
-        Flip a stack w.r.t. z-axis, i.e., reverse slices.
-
-        Set `copy = True` to get a copy of array, otherwise a view only.
-    '''
-    cripAssert(is3D(img), 'img should be 3D.')
-
-    if copy:
-        return np.array(np.flip(img, axis=0), copy=True)
-    else:
-        return np.flip(img, axis=0)
-
-
-@ConvertListNDArray
-def resize(img: TwoOrThreeD,
-           dsize: Tuple[int] = None,
-           scale: Tuple[Or[float, int]] = None,
-           interp: str = 'bicubic') -> TwoOrThreeD:
-    '''
-        Resize the image or each image in a volume to `dsize = (H, W)` (if dsize is not None) or scale 
-        by `scale = (facH, facW)` using `interp` (bicubic, linear, nearest available).
-    '''
-    cripAssert(inArray(interp, ['bicubic', 'linear', 'nearest']), 'Invalid interp method.')
-
-    if dsize is None:
-        cripAssert(scale is not None, 'dsize and scale cannot be None at the same time.')
-        cripAssert(len(scale) == 2, 'scale should have length 2.')
-        fH, fW = scale
-    else:
-        cripAssert(scale is None, 'scale should not be set when dsize is set.')
-        # OpenCV dsize is in (W, H) form, so we reverse it.
-        dsize = dsize[::-1]
-        fH = fW = None
-
-    interp_ = {'bicubic': cv2.INTER_CUBIC, 'linear': cv2.INTER_LINEAR, 'nearest': cv2.INTER_NEAREST}
-
-    if is3D(img):
-        c, _, _ = img.shape
-        res = [cv2.resize(img[i, ...], dsize, None, fW, fH, interpolation=interp_[interp]) for i in range(c)]
-        return np.array(res)
-    else:
-        return cv2.resize(img, dsize, None, fW, fH, interpolation=interp_[interp])
-
-
-@ConvertListNDArray
-def gaussianSmooth(img: TwoOrThreeD, sigma: Or[float, int, Tuple[Or[float, int]]], ksize: int = None):
-    '''
-        Perform Gaussian smooth with kernel size = ksize and Gaussian \sigma = sigma (int or tuple (x, y)).
-        
-        Leave `ksize = None` to auto determine to include the majority of Gaussian energy.
-    '''
-    if ksize is not None:
-        cripAssert(isInt(ksize), 'ksize should be int.')
-
-    if not isType(sigma, Tuple):
-        sigma = (sigma, sigma)
-
-    if is3D(img):
-        c, _, _ = img.shape
-        res = [cv2.GaussianBlur(img[i, ...], ksize, sigmaX=sigma[0], sigmaY=sigma[1]) for i in range(c)]
-        return np.array(res)
-    else:
-        return cv2.GaussianBlur(img, ksize, sigmaX=sigma[0], sigmaY=sigma[1])
-
-
-@ConvertListNDArray
-def stackImages(imgList: ListNDArray, dtype=None) -> NDArray:
-    '''
-        Stack seperate image into one numpy array. I.e., views * (h, w) -> (views, h, w).
-
-        Convert dtype with `dtype != None`.
-    '''
-    if dtype is not None:
-        imgList = imgList.astype(dtype)
-
-    return imgList
-
-
-def splitImages(imgs: ThreeD, dtype=None) -> List[NDArray]:
-    '''
-        Split stacked image into seperate numpy arrays. I.e., (views, h, w) -> views * (h, w).
-
-        Convert dtype with `dtype != None`.
-    '''
-    cripAssert(is3D(imgs), 'imgs should be 3D.')
-
-    if dtype is not None:
-        imgs = imgs.astype(dtype)
-
-    return list(imgs)
-
-
-@ConvertListNDArray
-def binning(img: TwoOrThreeD, rates: Tuple[int]) -> TwoOrThreeD:
-    '''
-        Perform binning with `rates = (c, h, w) / (h, w)`.
-    '''
-    for rate in rates:
-        cripAssert(isInt(rate) and rate > 0, 'rates should be positive int.')
-    if is2D(img):
-        cripAssert(len(rates) == 2, 'img is 2D, while rates is 3D.')
-    if is3D(img):
-        cripAssert(len(rates) == 3, 'img is 3D, while rates is 2D.')
-
-    if rates[-1] != 1:
-        img = img[..., ::rates[-1]]
-    if rates[-2] != 1:
-        img = img[..., ::rates[-2], :]
-    if len(rates) == 3 and rates[0] != 1:
-        img = img[::rates[0], ...]
-
-    return img
-
-
-@ConvertListNDArray
-def transpose(vol: TwoOrThreeD, order: Tuple[int]) -> TwoOrThreeD:
-    '''
-        Transpose vol with axes swapping `order`.
-    '''
-    if is2D(vol):
-        cripAssert(len(order) == 2, 'order should have length 2 for 2D input.')
-    if is3D(vol):
-        cripAssert(len(order) == 3, 'order should have length 3 for 3D input.')
-
-    return vol.transpose(order)
-
-
-@ConvertListNDArray
-def permute(vol: ThreeD, from_: str, to: str) -> ThreeD:
-    '''
-        Permute axes (transpose) from `from_` to `to`, reslicing the reconstructed volume.
-
-        Valid directions are: 'sagittal', 'coronal', 'transverse'.
-    '''
-    dirs = ['sagittal', 'coronal', 'transverse']
-
-    cripAssert(from_ in dirs, f'Invalid direction string: {from_}')
-    cripAssert(to in dirs, f'Invalid direction string: {to}')
-
-    if from_ == to:
-        return vol
-
-    dirFrom = dirs.index(from_)
-    dirTo = dirs.index(to)
-
-    # TODO check this matrix
-    orders = [
-        # to sag       cor         tra      # from
-        [(0, 1, 2), (1, 2, 0), (2, 1, 0)],  # sag
-        [(1, 2, 0), (0, 1, 2), (1, 0, 2)],  # cor
-        [(2, 1, 0), (1, 0, 2), (0, 1, 2)],  # tra
-    ]
-    order = orders[dirFrom][dirTo]
-
-    return transpose(vol, order)
-
-
-def shepplogan(size: int = 512):
-    '''
-        Generate the Shepp-Logan phantom.
-    '''
-    cripAssert(size in [256, 512, 1024], 'Shepp-Logan can only have size in 256 / 512 / 1024.')
-
-    phantomPath = path.join(getAsset('shepplogan'), f'{size}.tif')
-
-    return imreadTiff(phantomPath)
-
-
-def fitPolyV2D2(x1: NDArray, x2: NDArray, y: NDArray, bias: bool = True):
-    '''
-        Fit a degree-2 polynomial using pseudo-inverse to a pair of variables `x1, x2`.
-        Output 6 coefficients. If `bias` is False, the last coefficient will be 0.
-
-        `c[0] * x1**2 + c[1] * x2**2 + c[2] * x1 * x2 + c[3] * x1 + c[4] * x2 + c[5]`
-    '''
-    x1sq = x1.T**2
-    x2sq = x2.T**2
-    x1x2 = (x1 * x2).T
-    x1 = x1.T
-    x2 = x2.T
-    const = (np.ones if bias else np.zeros)((x1.T.shape[0]))
-    A = np.array([x1sq, x2sq, x1x2, x1, x2, const]).T
-
-    return np.linalg.pinv(A) @ y
-
-
-def applyPolyV2D2(coeff: NDArray, x1: NDArray, x2: NDArray):
-    '''
-        Apply a degree-2 polynomial to a pair of variables `x1, x2`.
-        
-        `c[0] * x1**2 + c[1] * x2**2 + c[2] * x1 * x2 + c[3] * x1 + c[4] * x2 + c[5]`
-    '''
-    cripAssert(len(coeff) in [5, 6], 'coeff should have length 5 or 6.')
-
-    if len(coeff) == 5:
-        bias = 0
-    else:
-        bias = coeff[5]
-
-    return coeff[0] * x1**2 + coeff[1] * x2**2 + coeff[2] * x1 * x2 + coeff[3] * x1 + coeff[4] * x2 + bias
-
-
-def fitPolyV1D2(x1: NDArray, y: NDArray, bias: bool = True):
-    '''
-        Fit a degree-2 polynomial using pseudo-inverse to a variable `x1`.
-        Output 3 coefficients. If `bias` is False, the last coefficient will be 0.
-
-        `c[0] * x1**2 + c[1] * x1 + c[2]`
-    '''
-    x1sq = x1.T**2
-    x1 = x1.T
-    const = (np.ones if bias else np.zeros)((x1.T.shape[0]))
-    A = np.array([x1sq, x1, const]).T
-
-    return np.linalg.pinv(A) @ y
-
-
-def applyPolyV1D2(coeff: NDArray, x1: NDArray):
-    '''
-        Apply a degree-2 polynomial to a variable `x1`.
-        
-        `c[0] * x1**2 + c[1] * x1 + c[2]`
-    '''
-    cripAssert(len(coeff) in [2, 3], 'coeff should have length 2 or 3.')
-
-    if len(coeff) == 5:
-        bias = 0
-    else:
-        bias = coeff[2]
-
-    return coeff[0] * x1**2 + coeff[1] * x1 + bias
+'''
+    Shared module of crip.
+
+    https://github.com/SEU-CT-Recon/crip
+'''
+
+import numpy as np
+from os import path
+import cv2
+import scipy.ndimage
+
+from .utils import *
+from ._typing import *
+from .io import imreadTiff
+
+
+@ConvertListNDArray
+def rotate(img: TwoOrThreeD, deg: int) -> TwoOrThreeD:
+    ''' Rotate each image by deg [DEG] (multiple of 90) clockwise.
+    '''
+    cripAssert(deg % 90 == 0, f'`deg` should be multiple of 90, but got {deg}.')
+
+    k = int(deg % 360) // 90
+    axes = (1, 2) if is3D(img) else (0, 1)
+
+    return np.rot90(img, -k, axes)
+
+
+@ConvertListNDArray
+def verticalFlip(img: TwoOrThreeD, copy=False) -> TwoOrThreeD:
+    ''' Vertical flip each image.
+    '''
+    cripAssert(is2or3D(img), f'img should be 2D or 3D, but got {img.ndim}-D.')
+
+    if copy:
+        return np.array(img[..., ::-1, :])
+    else:
+        return img[..., ::-1, :]
+
+
+@ConvertListNDArray
+def horizontalFlip(img: TwoOrThreeD, copy=False) -> TwoOrThreeD:
+    ''' Horizontal flip each image.
+    '''
+    cripAssert(is2or3D(img), f'img should be 2D or 3D, but got {img.ndim}-D.')
+
+    if copy:
+        return np.array(img[..., ::-1])
+    else:
+        return img[..., ::-1]
+
+
+@ConvertListNDArray
+def stackFlip(img: ThreeD, copy=False) -> ThreeD:
+    ''' Flip a stack w.r.t. z-axis, i.e., reverse slices.
+    '''
+    cripAssert(is3D(img), 'img should be 3D.')
+
+    if copy:
+        return np.array(np.flip(img, axis=0))
+    else:
+        return np.flip(img, axis=0)
+
+
+@ConvertListNDArray
+def resizeTo(img: TwoOrThreeD, dsize: Tuple[int], interp='bicubic') -> TwoOrThreeD:
+    ''' Resize each image to `dsize=(H, W)` using `interp` [bicubic, linear, nearest].
+    '''
+    cripAssert(interp in ['bicubic', 'linear', 'nearest'], f'Invalid interp method: {interp}.')
+    cripAssert(len(dsize) == 2, '`dsize` should be 2D.')
+
+    dsize = dsize[::-1]  # OpenCV dsize is in (W, H) form, so we reverse it.
+    interp_ = {'bicubic': cv2.INTER_CUBIC, 'linear': cv2.INTER_LINEAR, 'nearest': cv2.INTER_NEAREST}
+
+    if is3D(img):
+        res = [cv2.resize(img[i, ...], dsize, None, interpolation=interp_[interp]) for i in range(img.shape[0])]
+        return np.array(res)
+    else:
+        return cv2.resize(img, dsize, None, interpolation=interp_[interp])
+
+
+@ConvertListNDArray
+def resizeBy(img: TwoOrThreeD, factor: Or[Tuple[float], float], interp='bicubic') -> TwoOrThreeD:
+    ''' Resize each slice in img by `factor=(fH, fW)` or `(f, f)` float using `interp` [bicubic, linear, nearest].
+    '''
+    cripAssert(interp in ['bicubic', 'linear', 'nearest'], f'Invalid interp method: {interp}.')
+    if not isType(factor, Tuple):
+        factor = (factor, factor)
+    cripAssert(len(factor) == 2, '`factor` should be 2D.')
+
+    interp_ = {'bicubic': cv2.INTER_CUBIC, 'linear': cv2.INTER_LINEAR, 'nearest': cv2.INTER_NEAREST}
+    fH, fW = factor
+
+    if is3D(img):
+        res = [cv2.resize(img[i, ...], None, None, fW, fH, interpolation=interp_[interp]) for i in range(img.shape[0])]
+        return np.array(res)
+    else:
+        print(img, fW, fH, interp_[interp])
+        return cv2.resize(img, None, None, fW, fH, interpolation=interp_[interp])
+
+
+@ConvertListNDArray
+def resize3D(img: ThreeD, factor: Tuple[int], order=3) -> ThreeD:
+    ''' Resize 3D `img` by `factor=(fSlice, fH, fW)` using `order`-spline interpolation.
+    '''
+    cripAssert(len(factor) == 3, '`factor` should be 3D.')
+
+    return scipy.ndimage.zoom(img, factor, None, order, mode='mirror')
+
+
+@ConvertListNDArray
+def gaussianSmooth(img: TwoOrThreeD,
+                   sigma: Or[float, int, Tuple[Or[float, int]]],
+                   ksize: Or[Tuple[int], int, None] = None) -> TwoOrThreeD:
+    ''' Perform Gaussian smooth with kernel size `ksize` and Gaussian sigma = `sigma` [int or tuple (row, col)].
+        Leave `ksize=None` to auto determine it to include the majority of kernel energy.
+    '''
+    if ksize is not None:
+        if not isType(ksize, Sequence):
+            cripAssert(isInt(ksize), 'ksize should be int or sequence of int.')
+            ksize = (ksize, ksize)
+        else:
+            cripAssert(len(ksize) == 2, 'ksize should have length 2.')
+            cripAssert(isInt(ksize[0]) and isInt(ksize[1]), 'ksize should be int or sequence of int.')
+
+    if not isType(sigma, Sequence):
+        sigma = (sigma, sigma)
+
+    if is3D(img):
+        res = [cv2.GaussianBlur(img[i, ...], ksize, sigmaX=sigma[1], sigmaY=sigma[0]) for i in range(img.shape[0])]
+        return np.array(res)
+    else:
+        return cv2.GaussianBlur(img, ksize, sigmaX=sigma[1], sigmaY=sigma[0])
+
+
+@ConvertListNDArray
+def stackImages(imgList: ListNDArray, dtype=None) -> NDArray:
+    ''' Stack seperate image into one numpy array. I.e., views * (h, w) -> (views, h, w).
+        Convert dtype when `dtype` is not `None`.
+    '''
+    if dtype is not None:
+        imgList = imgList.astype(dtype)
+
+    return imgList
+
+
+def splitImages(imgs: ThreeD, dtype=None) -> ListNDArray:
+    ''' Split stacked image into seperate numpy arrays. I.e., (views, h, w) -> views * (h, w).
+        Convert dtype when `dtype` is not `None`.
+    '''
+    cripAssert(is3D(imgs), 'imgs should be 3D.')
+
+    if dtype is not None:
+        imgs = imgs.astype(dtype)
+
+    return list(imgs)
+
+
+@ConvertListNDArray
+def binning(img: TwoOrThreeD, rates: Tuple[int]) -> TwoOrThreeD:
+    ''' Perform binning with `rates = (c, h, w) / (h, w)`.
+    '''
+    for rate in rates:
+        cripAssert(isInt(rate) and rate > 0, 'rates should be positive int.')
+    if is2D(img):
+        cripAssert(len(rates) == 2, 'img is 2D, while rates is 3D.')
+    if is3D(img):
+        cripAssert(len(rates) == 3, 'img is 3D, while rates is 2D.')
+
+    if rates[-1] != 1:
+        img = img[..., ::rates[-1]]
+    if rates[-2] != 1:
+        img = img[..., ::rates[-2], :]
+    if len(rates) == 3 and rates[0] != 1:
+        img = img[::rates[0], ...]
+
+    return img
+
+
+@ConvertListNDArray
+def transpose(vol: TwoOrThreeD, order: Tuple[int]) -> TwoOrThreeD:
+    ''' Transpose vol with axes swapping `order`.
+    '''
+    if is2D(vol):
+        cripAssert(len(order) == 2, 'order should have length 2 for 2D input.')
+    if is3D(vol):
+        cripAssert(len(order) == 3, 'order should have length 3 for 3D input.')
+
+    return vol.transpose(order)
+
+
+@ConvertListNDArray
+def permute(vol: ThreeD, from_: str, to: str) -> ThreeD:
+    ''' Permute axes (transpose) from `from_` to `to`, reslicing the reconstructed volume.
+
+        Valid directions are: 'sagittal', 'coronal', 'transverse'.
+    '''
+    dirs = ['sagittal', 'coronal', 'transverse']
+
+    cripAssert(from_ in dirs, f'Invalid direction string: {from_}')
+    cripAssert(to in dirs, f'Invalid direction string: {to}')
+
+    if from_ == to:
+        return vol
+
+    dirFrom = dirs.index(from_)
+    dirTo = dirs.index(to)
+
+    # TODO check this matrix
+    orders = [
+        # to sag       cor         tra      # from
+        [(0, 1, 2), (1, 2, 0), (2, 1, 0)],  # sag
+        [(1, 2, 0), (0, 1, 2), (1, 0, 2)],  # cor
+        [(2, 1, 0), (1, 0, 2), (0, 1, 2)],  # tra
+    ]
+    order = orders[dirFrom][dirTo]
+
+    return transpose(vol, order)
+
+
+def shepplogan(size: int = 512) -> TwoD:
+    ''' Generate a `size x size` Shepp-Logan phantom.
+    '''
+    cripAssert(size in [256, 512, 1024], 'Shepp-Logan size should be in [256, 512, 1024]')
+
+    return imreadTiff(path.join(getAsset('shepplogan'), f'{size}.tif'))
+
+
+def fitPolyV2D2(x1: NDArray, x2: NDArray, y: NDArray, bias: bool = True) -> NDArray:
+    ''' Fit a degree-2 polynomial using pseudo-inverse to a pair of variables `x1, x2`.
+        Output 6 coefficients `c[0~5]`, minimizing the error of `y` and
+        `c[0] * x1**2 + c[1] * x2**2 + c[2] * x1 * x2 + c[3] * x1 + c[4] * x2 + c[5]`.
+        If `bias` is False, `c[5]` will be 0.
+    '''
+    cripAssert(is1D(x1) and is1D(x2) and is1D(y), 'Inputs should be 1D sequence.')
+    cripAssert(isOfSameShape(x1, x2) and isOfSameShape(x1, y), '`x1`, `x2` and `y` should have same shape.')
+
+    x1sq = x1.T**2
+    x2sq = x2.T**2
+    x1x2 = (x1 * x2).T
+    x1 = x1.T
+    x2 = x2.T
+    const = (np.ones if bias else np.zeros)((x1.T.shape[0]))
+    A = np.array([x1sq, x2sq, x1x2, x1, x2, const]).T
+
+    return np.linalg.pinv(A) @ y
+
+
+def applyPolyV2D2(coeff: NDArray, x1: NDArray, x2: NDArray) -> NDArray:
+    ''' Apply a degree-2 polynomial to a pair of variables `x1, x2`.
+        `coeff` has 5 or 6 elements, expands to 
+        `c[0] * x1**2 + c[1] * x2**2 + c[2] * x1 * x2 + c[3] * x1 + c[4] * x2 + (c[5] or 0)`.
+    '''
+    cripAssert(len(coeff) in [5, 6], '`coeff` should have length of 5 or 6.')
+
+    if len(coeff) == 5:
+        bias = 0
+    else:
+        bias = coeff[5]
+
+    return coeff[0] * x1**2 + coeff[1] * x2**2 + coeff[2] * x1 * x2 + coeff[3] * x1 + coeff[4] * x2 + bias
+
+
+def fitPolyV1D2(x1: NDArray, y: NDArray, bias: bool = True) -> NDArray:
+    ''' Fit a degree-2 polynomial using pseudo-inverse to a variable `x1`.
+        Output 3 coefficients `c[0~2]`, minimizing the error of `y` and
+        `c[0] * x1**2 + c[1] * x1 + c[2]`.
+        If `bias` is False, `c[2]` will be 0.
+    '''
+    x1sq = x1.T**2
+    x1 = x1.T
+    const = (np.ones if bias else np.zeros)((x1.T.shape[0]))
+    A = np.array([x1sq, x1, const]).T
+
+    return np.linalg.pinv(A) @ y
+
+
+def applyPolyV1D2(coeff: NDArray, x1: NDArray) -> NDArray:
+    ''' Apply a degree-2 polynomial to a variable `x1`.
+        `coeff` has 2 or 3 elements, expands to 
+        `c[0] * x1**2 + c[1] * x1 + (c[2] or 0)`.
+    '''
+    cripAssert(len(coeff) in [2, 3], 'coeff should have length 2 or 3.')
+
+    if len(coeff) == 2:
+        bias = 0
+    else:
+        bias = coeff[2]
+
+    return coeff[0] * x1**2 + coeff[1] * x1 + bias
```

