# Comparing `tmp/sage_lib-0.1.5.4.tar.gz` & `tmp/sage_lib-0.1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sage_lib-0.1.5.4.tar", last modified: Mon May 27 11:21:32 2024, max compression
+gzip compressed data, was "sage_lib-0.1.5.5.tar", last modified: Fri May 31 14:24:32 2024, max compression
```

## Comparing `sage_lib-0.1.5.4.tar` & `sage_lib-0.1.5.5.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-27 11:21:32.648360 sage_lib-0.1.5.4/
--rw-r--r--   0 dimitry    (501) staff       (20)      122 2024-05-27 11:21:32.648155 sage_lib-0.1.5.4/PKG-INFO
--rw-rw-r--   0 dimitry    (501) staff       (20)        7 2023-11-24 15:31:44.000000 sage_lib-0.1.5.4/README.md
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-27 11:21:32.626533 sage_lib-0.1.5.4/sage_lib/
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-27 11:21:32.630271 sage_lib-0.1.5.4/sage_lib/IO/
--rw-rw-r--   0 dimitry    (501) staff       (20)     5213 2023-11-26 10:15:10.000000 sage_lib-0.1.5.4/sage_lib/IO/BashScriptManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     4088 2023-11-26 10:15:54.000000 sage_lib-0.1.5.4/sage_lib/IO/BinaryDataHandler.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     3145 2023-11-26 10:15:38.000000 sage_lib-0.1.5.4/sage_lib/IO/ChargeFileManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     6402 2023-11-30 08:47:00.000000 sage_lib-0.1.5.4/sage_lib/IO/DOSManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     9400 2023-11-30 16:58:50.000000 sage_lib-0.1.5.4/sage_lib/IO/EigenvalueFileManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)      559 2023-11-26 11:22:04.000000 sage_lib-0.1.5.4/sage_lib/IO/ForceFieldManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     8862 2023-11-30 09:14:10.000000 sage_lib-0.1.5.4/sage_lib/IO/KPointsManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    17982 2024-05-14 11:48:21.000000 sage_lib-0.1.5.4/sage_lib/IO/OutFileManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     5292 2023-11-26 10:15:38.000000 sage_lib-0.1.5.4/sage_lib/IO/PROFileManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     8151 2023-11-26 10:16:36.000000 sage_lib-0.1.5.4/sage_lib/IO/PotentialManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     2756 2023-11-26 10:15:40.000000 sage_lib-0.1.5.4/sage_lib/IO/WaveFileManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.4/sage_lib/IO/__init__.py
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-27 11:21:32.631574 sage_lib-0.1.5.4/sage_lib/IO/input_handling_tools/
--rw-rw-r--   0 dimitry    (501) staff       (20)      609 2024-01-17 11:45:45.000000 sage_lib-0.1.5.4/sage_lib/IO/input_handling_tools/InputClassic.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    24368 2024-01-17 11:45:39.000000 sage_lib-0.1.5.4/sage_lib/IO/input_handling_tools/InputDFT.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     1168 2024-01-17 11:45:21.000000 sage_lib-0.1.5.4/sage_lib/IO/input_handling_tools/InputFile.py
--rw-rw-r--   0 dimitry    (501) staff       (20)      873 2023-11-26 10:17:02.000000 sage_lib-0.1.5.4/sage_lib/IO/input_handling_tools/InputFileManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.4/sage_lib/IO/input_handling_tools/__init__.py
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-27 11:21:32.634356 sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/
--rw-rw-r--   0 dimitry    (501) staff       (20)     2622 2024-01-17 11:44:29.000000 sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/AtomPosition.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     5789 2024-05-21 15:53:34.000000 sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/AtomPositionLoader.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     6242 2024-05-24 12:11:00.000000 sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/AtomPositionMaker.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    24117 2024-05-27 10:02:52.000000 sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/AtomPositionManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    47824 2024-05-27 11:11:25.000000 sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/AtomPositionOperator.py
--rw-rw-r--   0 dimitry    (501) staff       (20)      666 2024-01-30 15:22:44.000000 sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/NonPeriodicSystem.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    32829 2024-05-22 08:19:10.000000 sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/PeriodicSystem.py
--rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/__init__.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    10187 2024-01-25 08:34:17.000000 sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/plot.py
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-27 11:21:32.637608 sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/structural_file_readers/
--rw-rw-r--   0 dimitry    (501) staff       (20)     5733 2023-12-12 15:25:04.000000 sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/structural_file_readers/AIMS.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     4702 2023-12-18 08:26:38.000000 sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/structural_file_readers/ASE.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     3458 2023-11-28 08:43:18.000000 sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/structural_file_readers/CIF.py
--rw-r--r--   0 dimitry    (501) staff       (20)     8851 2024-05-21 15:56:27.000000 sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/structural_file_readers/DUMP.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     6036 2024-01-17 16:13:47.000000 sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/structural_file_readers/GEN.py
--rw-r--r--   0 dimitry    (501) staff       (20)    12682 2024-05-22 08:19:13.000000 sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/structural_file_readers/LAMMPS.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     7960 2024-04-03 12:15:20.000000 sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/structural_file_readers/PDB.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     5328 2024-05-16 15:26:28.000000 sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/structural_file_readers/POSCAR.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     2583 2023-11-28 07:46:02.000000 sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/structural_file_readers/SI.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    12012 2024-04-29 15:28:10.000000 sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/structural_file_readers/XYZ.py
--rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/structural_file_readers/__init__.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     5409 2024-01-17 14:07:15.000000 sage_lib-0.1.5.4/sage_lib/__init__.py
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-27 11:21:32.638464 sage_lib-0.1.5.4/sage_lib/descriptor/
--rw-rw-r--   0 dimitry    (501) staff       (20)    22605 2024-01-30 14:35:03.000000 sage_lib-0.1.5.4/sage_lib/descriptor/MBTR.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    12332 2024-01-26 13:40:44.000000 sage_lib-0.1.5.4/sage_lib/descriptor/MDTR_rev.py
--rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.4/sage_lib/descriptor/__init__.py
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-27 11:21:32.639216 sage_lib-0.1.5.4/sage_lib/ensemble/
--rw-rw-r--   0 dimitry    (501) staff       (20)      723 2023-11-30 08:05:18.000000 sage_lib-0.1.5.4/sage_lib/ensemble/DFTEnsemble.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     1943 2023-11-30 08:04:04.000000 sage_lib-0.1.5.4/sage_lib/ensemble/FFEnsembleManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.4/sage_lib/ensemble/__init__.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    63292 2024-05-24 08:50:37.000000 sage_lib-0.1.5.4/sage_lib/main.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    60371 2024-05-26 18:50:36.000000 sage_lib-0.1.5.4/sage_lib/main2.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    63292 2024-05-24 08:50:37.000000 sage_lib-0.1.5.4/sage_lib/main_rev.py
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-27 11:21:32.640139 sage_lib-0.1.5.4/sage_lib/master/
--rw-rw-r--   0 dimitry    (501) staff       (20)    56879 2024-05-16 12:31:55.000000 sage_lib-0.1.5.4/sage_lib/master/AtomicProperties.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    12849 2024-05-16 15:37:20.000000 sage_lib-0.1.5.4/sage_lib/master/FileManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.4/sage_lib/master/__init__.py
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-27 11:21:32.640993 sage_lib-0.1.5.4/sage_lib/miscellaneous/
--rw-rw-r--   0 dimitry    (501) staff       (20)     7176 2024-01-17 14:09:09.000000 sage_lib-0.1.5.4/sage_lib/miscellaneous/BandPathGenerator.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    24192 2024-03-27 14:48:16.000000 sage_lib-0.1.5.4/sage_lib/miscellaneous/MD_tools.py
--rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.4/sage_lib/miscellaneous/__init__.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    22279 2024-01-31 09:07:23.000000 sage_lib-0.1.5.4/sage_lib/miscellaneous/periodic_kdtree.py
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-27 11:21:32.641775 sage_lib-0.1.5.4/sage_lib/partition/
--rw-rw-r--   0 dimitry    (501) staff       (20)    18094 2024-05-22 09:47:50.000000 sage_lib-0.1.5.4/sage_lib/partition/Partition.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    28251 2024-05-27 11:12:35.000000 sage_lib-0.1.5.4/sage_lib/partition/PartitionManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.4/sage_lib/partition/__init__.py
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-27 11:21:32.646734 sage_lib-0.1.5.4/sage_lib/partition/partition_builder/
--rw-rw-r--   0 dimitry    (501) staff       (20)     7189 2024-02-23 12:29:06.000000 sage_lib-0.1.5.4/sage_lib/partition/partition_builder/AbInitioThermodynamics_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     2503 2023-11-26 11:03:08.000000 sage_lib-0.1.5.4/sage_lib/partition/partition_builder/BandStructure_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    24419 2024-04-30 06:33:56.000000 sage_lib-0.1.5.4/sage_lib/partition/partition_builder/Blender_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    11799 2024-04-15 15:59:15.000000 sage_lib-0.1.5.4/sage_lib/partition/partition_builder/Config_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    23321 2024-05-27 11:18:25.000000 sage_lib-0.1.5.4/sage_lib/partition/partition_builder/CrystalDefect_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)      614 2023-11-26 10:15:36.000000 sage_lib-0.1.5.4/sage_lib/partition/partition_builder/Crystal_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     2714 2024-02-28 10:50:31.000000 sage_lib-0.1.5.4/sage_lib/partition/partition_builder/Dataset_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    14023 2024-02-28 09:01:31.000000 sage_lib-0.1.5.4/sage_lib/partition/partition_builder/Filter_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    35233 2024-05-02 11:31:03.000000 sage_lib-0.1.5.4/sage_lib/partition/partition_builder/MolecularDynamic_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    15646 2024-05-24 14:03:21.000000 sage_lib-0.1.5.4/sage_lib/partition/partition_builder/MoleculeCluster_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     3669 2024-01-17 14:10:13.000000 sage_lib-0.1.5.4/sage_lib/partition/partition_builder/Molecule_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     4199 2024-04-02 14:56:25.000000 sage_lib-0.1.5.4/sage_lib/partition/partition_builder/PositionEditor_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    11331 2024-01-17 14:16:35.000000 sage_lib-0.1.5.4/sage_lib/partition/partition_builder/SupercellEmbedding_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     5375 2023-11-26 12:34:42.000000 sage_lib-0.1.5.4/sage_lib/partition/partition_builder/SurfaceStates_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     6358 2024-02-23 08:00:39.000000 sage_lib-0.1.5.4/sage_lib/partition/partition_builder/VacuumStates_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.4/sage_lib/partition/partition_builder/__init__.py
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-27 11:21:32.647808 sage_lib-0.1.5.4/sage_lib/single_run/
--rw-rw-r--   0 dimitry    (501) staff       (20)     6596 2023-11-24 15:31:44.000000 sage_lib-0.1.5.4/sage_lib/single_run/FF_Gap.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     1803 2024-01-17 15:01:44.000000 sage_lib-0.1.5.4/sage_lib/single_run/SingleRun.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    13356 2024-03-12 14:35:36.000000 sage_lib-0.1.5.4/sage_lib/single_run/SingleRunDFT.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     3098 2024-01-17 14:12:18.000000 sage_lib-0.1.5.4/sage_lib/single_run/SingleRunManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.4/sage_lib/single_run/__init__.py
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-27 11:21:32.647945 sage_lib-0.1.5.4/sage_lib.egg-info/
--rw-r--r--   0 dimitry    (501) staff       (20)      122 2024-05-27 11:21:32.000000 sage_lib-0.1.5.4/sage_lib.egg-info/PKG-INFO
--rw-rw-r--   0 dimitry    (501) staff       (20)     3836 2024-05-27 11:21:32.000000 sage_lib-0.1.5.4/sage_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 dimitry    (501) staff       (20)        1 2024-05-27 11:21:32.000000 sage_lib-0.1.5.4/sage_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 dimitry    (501) staff       (20)       44 2024-05-27 11:21:32.000000 sage_lib-0.1.5.4/sage_lib.egg-info/entry_points.txt
--rw-rw-r--   0 dimitry    (501) staff       (20)       23 2024-05-27 11:21:32.000000 sage_lib-0.1.5.4/sage_lib.egg-info/requires.txt
--rw-rw-r--   0 dimitry    (501) staff       (20)        9 2024-05-27 11:21:32.000000 sage_lib-0.1.5.4/sage_lib.egg-info/top_level.txt
--rw-r--r--   0 dimitry    (501) staff       (20)       38 2024-05-27 11:21:32.648406 sage_lib-0.1.5.4/setup.cfg
--rw-rw-r--   0 dimitry    (501) staff       (20)      394 2024-05-27 11:19:11.000000 sage_lib-0.1.5.4/setup.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-31 14:24:32.079643 sage_lib-0.1.5.5/
+-rw-r--r--   0 dimitry    (501) staff       (20)      122 2024-05-31 14:24:32.079441 sage_lib-0.1.5.5/PKG-INFO
+-rw-rw-r--   0 dimitry    (501) staff       (20)        7 2023-11-24 15:31:44.000000 sage_lib-0.1.5.5/README.md
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-31 14:24:32.056768 sage_lib-0.1.5.5/sage_lib/
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-31 14:24:32.060659 sage_lib-0.1.5.5/sage_lib/IO/
+-rw-rw-r--   0 dimitry    (501) staff       (20)     5213 2023-11-26 10:15:10.000000 sage_lib-0.1.5.5/sage_lib/IO/BashScriptManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     4088 2023-11-26 10:15:54.000000 sage_lib-0.1.5.5/sage_lib/IO/BinaryDataHandler.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     3145 2023-11-26 10:15:38.000000 sage_lib-0.1.5.5/sage_lib/IO/ChargeFileManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     6402 2023-11-30 08:47:00.000000 sage_lib-0.1.5.5/sage_lib/IO/DOSManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     9400 2023-11-30 16:58:50.000000 sage_lib-0.1.5.5/sage_lib/IO/EigenvalueFileManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)      559 2023-11-26 11:22:04.000000 sage_lib-0.1.5.5/sage_lib/IO/ForceFieldManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     8862 2023-11-30 09:14:10.000000 sage_lib-0.1.5.5/sage_lib/IO/KPointsManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    17984 2024-05-31 14:22:32.000000 sage_lib-0.1.5.5/sage_lib/IO/OutFileManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     5292 2023-11-26 10:15:38.000000 sage_lib-0.1.5.5/sage_lib/IO/PROFileManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     8151 2023-11-26 10:16:36.000000 sage_lib-0.1.5.5/sage_lib/IO/PotentialManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     2756 2023-11-26 10:15:40.000000 sage_lib-0.1.5.5/sage_lib/IO/WaveFileManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.5/sage_lib/IO/__init__.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-31 14:24:32.062124 sage_lib-0.1.5.5/sage_lib/IO/input_handling_tools/
+-rw-rw-r--   0 dimitry    (501) staff       (20)      609 2024-01-17 11:45:45.000000 sage_lib-0.1.5.5/sage_lib/IO/input_handling_tools/InputClassic.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    24368 2024-01-17 11:45:39.000000 sage_lib-0.1.5.5/sage_lib/IO/input_handling_tools/InputDFT.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     1168 2024-01-17 11:45:21.000000 sage_lib-0.1.5.5/sage_lib/IO/input_handling_tools/InputFile.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)      873 2023-11-26 10:17:02.000000 sage_lib-0.1.5.5/sage_lib/IO/input_handling_tools/InputFileManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.5/sage_lib/IO/input_handling_tools/__init__.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-31 14:24:32.065498 sage_lib-0.1.5.5/sage_lib/IO/structure_handling_tools/
+-rw-rw-r--   0 dimitry    (501) staff       (20)     2622 2024-01-17 11:44:29.000000 sage_lib-0.1.5.5/sage_lib/IO/structure_handling_tools/AtomPosition.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     5789 2024-05-21 15:53:34.000000 sage_lib-0.1.5.5/sage_lib/IO/structure_handling_tools/AtomPositionLoader.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     6242 2024-05-24 12:11:00.000000 sage_lib-0.1.5.5/sage_lib/IO/structure_handling_tools/AtomPositionMaker.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    24117 2024-05-27 10:02:52.000000 sage_lib-0.1.5.5/sage_lib/IO/structure_handling_tools/AtomPositionManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    47905 2024-05-29 15:35:27.000000 sage_lib-0.1.5.5/sage_lib/IO/structure_handling_tools/AtomPositionOperator.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)      666 2024-01-30 15:22:44.000000 sage_lib-0.1.5.5/sage_lib/IO/structure_handling_tools/NonPeriodicSystem.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    32829 2024-05-22 08:19:10.000000 sage_lib-0.1.5.5/sage_lib/IO/structure_handling_tools/PeriodicSystem.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.5/sage_lib/IO/structure_handling_tools/__init__.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    10187 2024-01-25 08:34:17.000000 sage_lib-0.1.5.5/sage_lib/IO/structure_handling_tools/plot.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-31 14:24:32.068784 sage_lib-0.1.5.5/sage_lib/IO/structure_handling_tools/structural_file_readers/
+-rw-rw-r--   0 dimitry    (501) staff       (20)     5733 2023-12-12 15:25:04.000000 sage_lib-0.1.5.5/sage_lib/IO/structure_handling_tools/structural_file_readers/AIMS.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     4702 2023-12-18 08:26:38.000000 sage_lib-0.1.5.5/sage_lib/IO/structure_handling_tools/structural_file_readers/ASE.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     3458 2023-11-28 08:43:18.000000 sage_lib-0.1.5.5/sage_lib/IO/structure_handling_tools/structural_file_readers/CIF.py
+-rw-r--r--   0 dimitry    (501) staff       (20)     8851 2024-05-21 15:56:27.000000 sage_lib-0.1.5.5/sage_lib/IO/structure_handling_tools/structural_file_readers/DUMP.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     6036 2024-01-17 16:13:47.000000 sage_lib-0.1.5.5/sage_lib/IO/structure_handling_tools/structural_file_readers/GEN.py
+-rw-r--r--   0 dimitry    (501) staff       (20)    12684 2024-05-29 12:51:56.000000 sage_lib-0.1.5.5/sage_lib/IO/structure_handling_tools/structural_file_readers/LAMMPS.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     7960 2024-04-03 12:15:20.000000 sage_lib-0.1.5.5/sage_lib/IO/structure_handling_tools/structural_file_readers/PDB.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     5328 2024-05-16 15:26:28.000000 sage_lib-0.1.5.5/sage_lib/IO/structure_handling_tools/structural_file_readers/POSCAR.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     2583 2023-11-28 07:46:02.000000 sage_lib-0.1.5.5/sage_lib/IO/structure_handling_tools/structural_file_readers/SI.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    12012 2024-05-31 14:04:06.000000 sage_lib-0.1.5.5/sage_lib/IO/structure_handling_tools/structural_file_readers/XYZ.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.5/sage_lib/IO/structure_handling_tools/structural_file_readers/__init__.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     5409 2024-01-17 14:07:15.000000 sage_lib-0.1.5.5/sage_lib/__init__.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-31 14:24:32.069639 sage_lib-0.1.5.5/sage_lib/descriptor/
+-rw-rw-r--   0 dimitry    (501) staff       (20)    22605 2024-01-30 14:35:03.000000 sage_lib-0.1.5.5/sage_lib/descriptor/MBTR.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    12332 2024-01-26 13:40:44.000000 sage_lib-0.1.5.5/sage_lib/descriptor/MDTR_rev.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.5/sage_lib/descriptor/__init__.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-31 14:24:32.070380 sage_lib-0.1.5.5/sage_lib/ensemble/
+-rw-rw-r--   0 dimitry    (501) staff       (20)      723 2023-11-30 08:05:18.000000 sage_lib-0.1.5.5/sage_lib/ensemble/DFTEnsemble.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     1943 2023-11-30 08:04:04.000000 sage_lib-0.1.5.5/sage_lib/ensemble/FFEnsembleManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.5/sage_lib/ensemble/__init__.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    63301 2024-05-29 15:27:20.000000 sage_lib-0.1.5.5/sage_lib/main.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    60371 2024-05-26 18:50:36.000000 sage_lib-0.1.5.5/sage_lib/main2.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    63292 2024-05-24 08:50:37.000000 sage_lib-0.1.5.5/sage_lib/main_rev.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-31 14:24:32.071334 sage_lib-0.1.5.5/sage_lib/master/
+-rw-rw-r--   0 dimitry    (501) staff       (20)    56879 2024-05-16 12:31:55.000000 sage_lib-0.1.5.5/sage_lib/master/AtomicProperties.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    12849 2024-05-16 15:37:20.000000 sage_lib-0.1.5.5/sage_lib/master/FileManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.5/sage_lib/master/__init__.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-31 14:24:32.072194 sage_lib-0.1.5.5/sage_lib/miscellaneous/
+-rw-rw-r--   0 dimitry    (501) staff       (20)     7176 2024-01-17 14:09:09.000000 sage_lib-0.1.5.5/sage_lib/miscellaneous/BandPathGenerator.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    24192 2024-03-27 14:48:16.000000 sage_lib-0.1.5.5/sage_lib/miscellaneous/MD_tools.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.5/sage_lib/miscellaneous/__init__.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    22279 2024-01-31 09:07:23.000000 sage_lib-0.1.5.5/sage_lib/miscellaneous/periodic_kdtree.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-31 14:24:32.073087 sage_lib-0.1.5.5/sage_lib/partition/
+-rw-rw-r--   0 dimitry    (501) staff       (20)    18094 2024-05-22 09:47:50.000000 sage_lib-0.1.5.5/sage_lib/partition/Partition.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    28251 2024-05-27 11:12:35.000000 sage_lib-0.1.5.5/sage_lib/partition/PartitionManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.5/sage_lib/partition/__init__.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-31 14:24:32.078072 sage_lib-0.1.5.5/sage_lib/partition/partition_builder/
+-rw-rw-r--   0 dimitry    (501) staff       (20)     7189 2024-02-23 12:29:06.000000 sage_lib-0.1.5.5/sage_lib/partition/partition_builder/AbInitioThermodynamics_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     2503 2023-11-26 11:03:08.000000 sage_lib-0.1.5.5/sage_lib/partition/partition_builder/BandStructure_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    24419 2024-04-30 06:33:56.000000 sage_lib-0.1.5.5/sage_lib/partition/partition_builder/Blender_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    14428 2024-05-29 15:37:37.000000 sage_lib-0.1.5.5/sage_lib/partition/partition_builder/Config_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    24171 2024-05-29 14:35:56.000000 sage_lib-0.1.5.5/sage_lib/partition/partition_builder/CrystalDefect_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)      614 2023-11-26 10:15:36.000000 sage_lib-0.1.5.5/sage_lib/partition/partition_builder/Crystal_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     2714 2024-02-28 10:50:31.000000 sage_lib-0.1.5.5/sage_lib/partition/partition_builder/Dataset_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    14023 2024-02-28 09:01:31.000000 sage_lib-0.1.5.5/sage_lib/partition/partition_builder/Filter_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    35233 2024-05-02 11:31:03.000000 sage_lib-0.1.5.5/sage_lib/partition/partition_builder/MolecularDynamic_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    15646 2024-05-24 14:03:21.000000 sage_lib-0.1.5.5/sage_lib/partition/partition_builder/MoleculeCluster_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     3669 2024-01-17 14:10:13.000000 sage_lib-0.1.5.5/sage_lib/partition/partition_builder/Molecule_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     4199 2024-04-02 14:56:25.000000 sage_lib-0.1.5.5/sage_lib/partition/partition_builder/PositionEditor_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    11331 2024-01-17 14:16:35.000000 sage_lib-0.1.5.5/sage_lib/partition/partition_builder/SupercellEmbedding_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     5375 2023-11-26 12:34:42.000000 sage_lib-0.1.5.5/sage_lib/partition/partition_builder/SurfaceStates_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     6358 2024-02-23 08:00:39.000000 sage_lib-0.1.5.5/sage_lib/partition/partition_builder/VacuumStates_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.5/sage_lib/partition/partition_builder/__init__.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-31 14:24:32.079066 sage_lib-0.1.5.5/sage_lib/single_run/
+-rw-rw-r--   0 dimitry    (501) staff       (20)     6596 2023-11-24 15:31:44.000000 sage_lib-0.1.5.5/sage_lib/single_run/FF_Gap.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     1803 2024-01-17 15:01:44.000000 sage_lib-0.1.5.5/sage_lib/single_run/SingleRun.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    13356 2024-03-12 14:35:36.000000 sage_lib-0.1.5.5/sage_lib/single_run/SingleRunDFT.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     3098 2024-01-17 14:12:18.000000 sage_lib-0.1.5.5/sage_lib/single_run/SingleRunManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.5/sage_lib/single_run/__init__.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-31 14:24:32.079214 sage_lib-0.1.5.5/sage_lib.egg-info/
+-rw-r--r--   0 dimitry    (501) staff       (20)      122 2024-05-31 14:24:32.000000 sage_lib-0.1.5.5/sage_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 dimitry    (501) staff       (20)     3836 2024-05-31 14:24:32.000000 sage_lib-0.1.5.5/sage_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 dimitry    (501) staff       (20)        1 2024-05-31 14:24:32.000000 sage_lib-0.1.5.5/sage_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 dimitry    (501) staff       (20)       44 2024-05-31 14:24:32.000000 sage_lib-0.1.5.5/sage_lib.egg-info/entry_points.txt
+-rw-rw-r--   0 dimitry    (501) staff       (20)       23 2024-05-31 14:24:32.000000 sage_lib-0.1.5.5/sage_lib.egg-info/requires.txt
+-rw-rw-r--   0 dimitry    (501) staff       (20)        9 2024-05-31 14:24:32.000000 sage_lib-0.1.5.5/sage_lib.egg-info/top_level.txt
+-rw-r--r--   0 dimitry    (501) staff       (20)       38 2024-05-31 14:24:32.079694 sage_lib-0.1.5.5/setup.cfg
+-rw-rw-r--   0 dimitry    (501) staff       (20)      394 2024-05-31 14:22:44.000000 sage_lib-0.1.5.5/setup.py
```

### Comparing `sage_lib-0.1.5.4/sage_lib/IO/BashScriptManager.py` & `sage_lib-0.1.5.5/sage_lib/IO/BashScriptManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.4/sage_lib/IO/BinaryDataHandler.py` & `sage_lib-0.1.5.5/sage_lib/IO/BinaryDataHandler.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.4/sage_lib/IO/ChargeFileManager.py` & `sage_lib-0.1.5.5/sage_lib/IO/ChargeFileManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.4/sage_lib/IO/DOSManager.py` & `sage_lib-0.1.5.5/sage_lib/IO/DOSManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.4/sage_lib/IO/EigenvalueFileManager.py` & `sage_lib-0.1.5.5/sage_lib/IO/EigenvalueFileManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.4/sage_lib/IO/ForceFieldManager.py` & `sage_lib-0.1.5.5/sage_lib/IO/ForceFieldManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.4/sage_lib/IO/KPointsManager.py` & `sage_lib-0.1.5.5/sage_lib/IO/KPointsManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.4/sage_lib/IO/OutFileManager.py` & `sage_lib-0.1.5.5/sage_lib/IO/OutFileManager.py`

 * *Files 0% similar despite different names*

```diff
@@ -313,15 +313,15 @@
 
                     if not hasattr(self, '_dynamical_eigenvector_diff') or not isinstance(self._dynamical_eigenvector_diff, list):
                         setattr(self, '_dynamical_eigenvector_diff', [_extract_parameter(None, 2, slice(3, None))] )
                     else:
                         self._dynamical_eigenvector_diff.append( _extract_parameter(None, 2, slice(3, None)) ) 
 
         # Append the final APM object if it exists and is not already in APM_holder
-        if isinstance(APM, AtomPosition) and not APM in APM_holder: 
+        if isinstance(APM, AtomPosition): #and not APM in APM_holder: 
             APM_holder.append(APM)
 
         # Updating the instance's AtomPositionManager with the extracted data
         self._AtomPositionManager = APM_holder
 
     def _update_parameters(self, var_name, value):
         """
```

### Comparing `sage_lib-0.1.5.4/sage_lib/IO/PROFileManager.py` & `sage_lib-0.1.5.5/sage_lib/IO/PROFileManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.4/sage_lib/IO/PotentialManager.py` & `sage_lib-0.1.5.5/sage_lib/IO/PotentialManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.4/sage_lib/IO/WaveFileManager.py` & `sage_lib-0.1.5.5/sage_lib/IO/WaveFileManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.4/sage_lib/IO/input_handling_tools/InputClassic.py` & `sage_lib-0.1.5.5/sage_lib/IO/input_handling_tools/InputClassic.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.4/sage_lib/IO/input_handling_tools/InputDFT.py` & `sage_lib-0.1.5.5/sage_lib/IO/input_handling_tools/InputDFT.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.4/sage_lib/IO/input_handling_tools/InputFile.py` & `sage_lib-0.1.5.5/sage_lib/IO/input_handling_tools/InputFile.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.4/sage_lib/IO/input_handling_tools/InputFileManager.py` & `sage_lib-0.1.5.5/sage_lib/IO/input_handling_tools/InputFileManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/AtomPosition.py` & `sage_lib-0.1.5.5/sage_lib/IO/structure_handling_tools/AtomPosition.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/AtomPositionLoader.py` & `sage_lib-0.1.5.5/sage_lib/IO/structure_handling_tools/AtomPositionLoader.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/AtomPositionMaker.py` & `sage_lib-0.1.5.5/sage_lib/IO/structure_handling_tools/AtomPositionMaker.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/AtomPositionManager.py` & `sage_lib-0.1.5.5/sage_lib/IO/structure_handling_tools/AtomPositionManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/AtomPositionOperator.py` & `sage_lib-0.1.5.5/sage_lib/IO/structure_handling_tools/AtomPositionOperator.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,14 +198,16 @@
             bool: True if the operation is successful, False otherwise.
 
         Note:
             Similar to change_ID, this method also resets attributes like the full atom label string,
             atom count by type, and unique atom labels, to maintain data integrity.
         """
         # Set the new ID for the atom at the specified index
+        self.atomLabelsList 
+        print(self.atomLabelsList, atom_index, ID) 
         self._atomLabelsList[atom_index] = ID
 
         # Reset related attributes to nullify any previous computations
         self._fullAtomLabelString= None
         self._atomCountByType = None
         self._uniqueAtomLabels = None
```

### Comparing `sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/NonPeriodicSystem.py` & `sage_lib-0.1.5.5/sage_lib/IO/structure_handling_tools/NonPeriodicSystem.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/PeriodicSystem.py` & `sage_lib-0.1.5.5/sage_lib/IO/structure_handling_tools/PeriodicSystem.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/plot.py` & `sage_lib-0.1.5.5/sage_lib/IO/structure_handling_tools/plot.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/structural_file_readers/AIMS.py` & `sage_lib-0.1.5.5/sage_lib/IO/structure_handling_tools/structural_file_readers/AIMS.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/structural_file_readers/ASE.py` & `sage_lib-0.1.5.5/sage_lib/IO/structure_handling_tools/structural_file_readers/ASE.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/structural_file_readers/CIF.py` & `sage_lib-0.1.5.5/sage_lib/IO/structure_handling_tools/structural_file_readers/CIF.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/structural_file_readers/DUMP.py` & `sage_lib-0.1.5.5/sage_lib/IO/structure_handling_tools/structural_file_readers/DUMP.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/structural_file_readers/GEN.py` & `sage_lib-0.1.5.5/sage_lib/IO/structure_handling_tools/structural_file_readers/GEN.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/structural_file_readers/LAMMPS.py` & `sage_lib-0.1.5.5/sage_lib/IO/structure_handling_tools/structural_file_readers/LAMMPS.py`

 * *Files 0% similar despite different names*

```diff
@@ -283,15 +283,15 @@
             file.write("\n")
             '''
 
             # Atoms
             label_dict = {unique_atom_label:i for i, unique_atom_label in enumerate(self.uniqueAtomLabels, start=1) }
             file.write("Atoms\n\n")
             for i, (atom_position, atom_label) in enumerate( zip(self.atomPositions, self.atomLabelsList) ):
-                file.write(f"{i} {label_dict[atom_label]} {atom_position[0]} {atom_position[1]} {atom_position[2]}\n")
+                file.write(f"{i+1} {label_dict[atom_label]} {atom_position[0]} {atom_position[1]} {atom_position[2]}\n")
             file.write("\n")
             '''
             # Velocities
             file.write("Velocities\n\n")
             for velocity in self.velocities:
                 file.write(f"{velocity['id']} {velocity['vx']} {velocity['vy']} {velocity['vz']}\n")
             file.write("\n")
```

### Comparing `sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/structural_file_readers/PDB.py` & `sage_lib-0.1.5.5/sage_lib/IO/structure_handling_tools/structural_file_readers/PDB.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/structural_file_readers/POSCAR.py` & `sage_lib-0.1.5.5/sage_lib/IO/structure_handling_tools/structural_file_readers/POSCAR.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/structural_file_readers/SI.py` & `sage_lib-0.1.5.5/sage_lib/IO/structure_handling_tools/structural_file_readers/SI.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/structural_file_readers/XYZ.py` & `sage_lib-0.1.5.5/sage_lib/IO/structure_handling_tools/structural_file_readers/XYZ.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,18 +62,18 @@
             f'{time_tag}={self.time}' if include_time else ''
         ]
         properties_str = ' '.join(filter(None, properties_list))
 
         # Preparing atom data lines
         atom_lines = [
             f"{self.atomLabelsList[i]} {' '.join(map('{:13.10f}'.format, self.atomPositions[i])) if include_position else ''} \
-            {' '.join(map('{:2d}'.format, np.array(self.atomicConstraints[i], dtype=np.int32) )) if include_fixed else ''} \
+            {' '.join(map('{:14.10f}'.format, self.total_force[i])) if include_forces else ''} \
             {' '.join(map('{:14.10f}'.format, self.charge[i] if np.ndim(self.charge) == 1 else [self.charge[i, -1]])) if include_charge else ''} \
             {' '.join(map('{:14.10f}'.format, self.magnetization[i] if np.ndim(self.magnetization) == 1 else [self.magnetization[i, -1]])) if include_magnetization else ''} \
-            {' '.join(map('{:14.10f}'.format, self.total_force[i])) if include_forces else ''} "
+            {' '.join(map('{:2d}'.format, np.array(self.atomicConstraints[i], dtype=np.int32) )) if include_fixed else ''} "
             for i in range(self.atomCount)
         ]
 
         # Combining header and atom data
         xyz_content = f"{self.atomCount}\n{properties_str}\n" + "\n".join(atom_lines)+ "\n"
 
         # Saving to file if required
```

### Comparing `sage_lib-0.1.5.4/sage_lib/__init__.py` & `sage_lib-0.1.5.5/sage_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.4/sage_lib/descriptor/MBTR.py` & `sage_lib-0.1.5.5/sage_lib/descriptor/MBTR.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.4/sage_lib/descriptor/MDTR_rev.py` & `sage_lib-0.1.5.5/sage_lib/descriptor/MDTR_rev.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.4/sage_lib/ensemble/DFTEnsemble.py` & `sage_lib-0.1.5.5/sage_lib/ensemble/DFTEnsemble.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.4/sage_lib/ensemble/FFEnsembleManager.py` & `sage_lib-0.1.5.5/sage_lib/ensemble/FFEnsembleManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.4/sage_lib/main.py` & `sage_lib-0.1.5.5/sage_lib/main_rev.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.4/sage_lib/main2.py` & `sage_lib-0.1.5.5/sage_lib/main2.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.4/sage_lib/main_rev.py` & `sage_lib-0.1.5.5/sage_lib/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -774,15 +774,15 @@
     parser_edit.add_argument('--degree', type=int, required=False, default=1, help='')
     parser_edit.add_argument('--first_neighbor', required=False, default=False, action='store_true', help='')
 
     # ========== Sub-command: edit_configuration ===========
     parser_edit_config = subparsers.add_parser('edit_configuration', help='Modify the configuration settings of your simulation or calculation process.')
     add_arguments(parser_edit_config)
     parser_edit_config.add_argument('--edit', type=str, choices=['atom_id', 'atom_index'], help='Specify the type of configuration modification.')
-    parser_edit_config.add_argument('--search', type=str, choices=['full', 'random'], required=False, help='')
+    parser_edit_config.add_argument('--search', type=str, choices=['full', 'random', 'exact'], required=False, help='')
     parser_edit_config.add_argument('--index', type=int, nargs='+', required=False, help='')
     parser_edit_config.add_argument('--ID', type=str, nargs='+', required=False, help='Identifier for the configuration element to modify.')
     parser_edit_config.add_argument('--new_ID', type=str, nargs='+', required=False, help='New identifier to assign to the configuration element.')
     parser_edit_config.add_argument('--weights', type=float, nargs='+', required=False, help='')
     parser_edit_config.add_argument('--N', default=1, type=int, required=False, help='.')
     parser_edit_config.add_argument('--seed', default=1, type=int, required=False, help='.')
```

### Comparing `sage_lib-0.1.5.4/sage_lib/master/AtomicProperties.py` & `sage_lib-0.1.5.5/sage_lib/master/AtomicProperties.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.4/sage_lib/master/FileManager.py` & `sage_lib-0.1.5.5/sage_lib/master/FileManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.4/sage_lib/miscellaneous/BandPathGenerator.py` & `sage_lib-0.1.5.5/sage_lib/miscellaneous/BandPathGenerator.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.4/sage_lib/miscellaneous/MD_tools.py` & `sage_lib-0.1.5.5/sage_lib/miscellaneous/MD_tools.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.4/sage_lib/miscellaneous/periodic_kdtree.py` & `sage_lib-0.1.5.5/sage_lib/miscellaneous/periodic_kdtree.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.4/sage_lib/partition/Partition.py` & `sage_lib-0.1.5.5/sage_lib/partition/Partition.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.4/sage_lib/partition/PartitionManager.py` & `sage_lib-0.1.5.5/sage_lib/partition/PartitionManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.4/sage_lib/partition/partition_builder/AbInitioThermodynamics_builder.py` & `sage_lib-0.1.5.5/sage_lib/partition/partition_builder/AbInitioThermodynamics_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.4/sage_lib/partition/partition_builder/BandStructure_builder.py` & `sage_lib-0.1.5.5/sage_lib/partition/partition_builder/BandStructure_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.4/sage_lib/partition/partition_builder/Blender_builder.py` & `sage_lib-0.1.5.5/sage_lib/partition/partition_builder/Blender_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.4/sage_lib/partition/partition_builder/Config_builder.py` & `sage_lib-0.1.5.5/sage_lib/partition/partition_builder/Config_builder.py`

 * *Files 22% similar despite different names*

```diff
@@ -159,15 +159,15 @@
 
                             selected_atomLabels_None = np.where(container_copy.AtomPositionManager.atomLabelsList =='X')[0]
                             container_copy.AtomPositionManager.remove_atom( atom_index=selected_atomLabels_None )
 
                             containers.append(container_copy)
 
                     if values[v]['search'].upper() == 'RANDOM':
-                        atom_index, new_atom_ID = np.array(values['atom_ID']), np.array(values['new_atom_ID'])
+                        atom_index, new_atom_ID = np.array(values[v]['atom_ID']), np.array(values[v]['new_atom_ID'])
                        
                         for n in range(values[v]['N']):
 
                             container_copy = self.copy_and_update_container(container, f'/Atom_ID_Change_random_', '')
                     
                             # Choose new atom IDs based on the specified weights
                             new_atomLabels = random.choices(new_atom_ID, values[v]['weights'], k=atom_index.shape[0] )
@@ -178,14 +178,58 @@
                             selected_atomLabels_None = np.where(container_copy.AtomPositionManager.atomLabelsList =='X')[0]
                             
                             container_copy.AtomPositionManager.remove_atom( atom_index=selected_atomLabels_None )
 
                             # Add the updated container to the list
                             containers.append(container_copy)
 
+                    if values[v]['search'].upper() == 'EXACT':
+                        atom_index, new_atom_ID = np.array([int(n) for n in values[v]['atom_ID']]), np.array(values[v]['new_atom_ID'])
+                        
+                        weights = values[v]['weights']
+                        total_atoms = atom_index.shape[0]
+
+                        replacement_quantities = {new_id: int(round(weight * total_atoms)) for new_id, weight in zip(new_atom_ID, weights)}
+                        
+                        # Adjust quantities to ensure they sum up to the total number of atoms
+                        diff = total_atoms - sum(replacement_quantities.values())
+                        while diff != 0:
+                            for key in replacement_quantities.keys():
+                                if diff == 0:
+                                    break
+                                if diff > 0:
+                                    replacement_quantities[key] += 1
+                                    diff -= 1
+                                elif diff < 0 and replacement_quantities[key] > 0:
+                                    replacement_quantities[key] -= 1
+                                    diff += 1
+
+                        for n in range(values[v]['N']):
+
+                            container_copy = self.copy_and_update_container(container, f'/Atom_ID_Change_random_', '')
+                    
+                            # Create a list of new atom IDs based on fixed quantities
+                            new_atomLabels = []
+                            for atom, quantity in replacement_quantities.items():
+                                new_atomLabels.extend([atom] * quantity)
+                            
+                            # Shuffle the new atom IDs to distribute them randomly
+                            random.shuffle(new_atomLabels)
+
+                            # Update the atom IDs in the container copy
+                            print(new_atomLabels, container_copy.AtomPositionManager._atomLabelsList)
+                            container_copy.AtomPositionManager.set_ID(atom_index=atom_index, ID=new_atomLabels)
+
+                            # Find and remove atoms with the label 'X'
+                            selected_atomLabels_None = np.where(container_copy.AtomPositionManager.atomLabelsList =='X')[0]
+                            container_copy.AtomPositionManager.remove_atom( atom_index=selected_atomLabels_None )
+
+                            # Add the updated container to the list
+                            containers.append(container_copy)
+
 
                 if v.upper() == 'ATOM_ID':
 
                     if values[v]['search'].upper() == 'FULL':
                         selected_atomLabels = np.isin(container.AtomPositionManager.atomLabelsList, values[v]['atom_ID'])
 
                         for new_atom_ID in self._product( values[v]['new_atom_ID'], repeat=np.sum(selected_atomLabels) ):
```

### Comparing `sage_lib-0.1.5.4/sage_lib/partition/partition_builder/CrystalDefect_builder.py` & `sage_lib-0.1.5.5/sage_lib/partition/partition_builder/CrystalDefect_builder.py`

 * *Files 4% similar despite different names*

```diff
@@ -151,15 +151,23 @@
         is_number = lambda s: s.replace('.', '', 1).isdigit() or s.replace('-', '', 1).replace('.', '', 1).isdigit()
 
         atom_ids = set()
         for item in selection_list:
             if isinstance(item, int) or is_number(item):
                 atom_ids.add( int(item) )
             elif isinstance(item, str):
-                if '-' in item:
+                if item.upper() in ['H2O', 'water']:
+                    for i, label in enumerate(AtomPositionManager.atomLabelsList):
+                        if label == 'O':
+                            pos = AtomPositionManager.atomPositions[i]
+                            closest_neighbors = AtomPositionManager.find_n_closest_neighbors(pos, 4)
+                            if AtomPositionManager.atomLabelsList[closest_neighbors[1][1]] == AtomPositionManager.atomLabelsList[closest_neighbors[1][2]] == 'H' and closest_neighbors[0][2] < 1.2 and closest_neighbors[0][3] > 1.2: 
+                                atom_ids.add( tuple(closest_neighbors[1][:3]) )
+
+                elif '-' in item:
                     a1, a2 = item.split('-')
                     for i, label in enumerate(AtomPositionManager.atomLabelsList):
                         if label == a1:
                             
                             pos = AtomPositionManager.atomPositions[i]
                             if AtomPositionManager.atomLabelsList[AtomPositionManager.find_n_closest_neighbors(pos, 2)[1][1]] == a2 or \
                                 AtomPositionManager.atomLabelsList[AtomPositionManager.find_n_closest_neighbors(pos, 3)[1][2]] == a2 :
@@ -224,31 +232,36 @@
                 
                 for ite in range(iterations):
                     if verbose: print(f' - iteration : {ite} ({100*float(ite)/iterations}%)')    
                     
                     atom_groups_ID = [self.get_atom_ids(container_copy.AtomPositionManager, group) for group in atom_groups]
                     if verbose: print(f' - Processing : {len(atom_groups_ID)} groups : { [len(agi) for agi in atom_groups_ID] } groups len ')    
 
-                    distances_dict = self.get_distances_dict(list(set(item for sublist in atom_groups_ID for item in sublist)), container_copy.AtomPositionManager) 
-                    if verbose: print(f' - Distance dict calculated (ok!) ')    
+                    if 'distance' in distribution:
+                        distances_dict = self.get_distances_dict(list(set(item for sublist in atom_groups_ID for item in sublist)), container_copy.AtomPositionManager) 
+                        if verbose: print(f' - Distance dict calculated (ok!) ')    
+                    else:
+                        distances_dict = {}
 
                     combinations = self.generate_combinations(atom_groups_ID, group_numbers)
                     if verbose: print(f' - Founded {len(combinations)} ')    
 
-                    probabilities = [self.get_probability(combination=c, distribution=distribution, AtomPositionManager=container_copy.AtomPositionManager, distances_dict=distances_dict, coefficient=coefficient) for c in combinations]
+                    probabilities = [self.get_probability(  combination=c, distribution=distribution, AtomPositionManager=container_copy.AtomPositionManager, 
+                                                            distances_dict=distances_dict, coefficient=coefficient) for c in combinations]
                     if verbose: print(f' - Probabilities calculated')    
 
                     probabilities_norm = np.array(probabilities) / np.sum(probabilities)
                     if verbose: print(f' - Probabilities normalized')
 
                     selected_index = np.random.choice(np.arange(len(combinations)), p=probabilities_norm)
-                    selected_combination = combinations[selected_index]
+                    selected_combination = np.array(combinations[selected_index]).flatten()
+                    print(selected_combination)
 
                     container_copy.AtomPositionManager.atomLabelsList = np.array(container_copy.AtomPositionManager.atomLabelsList)
-                    print( container_copy.AtomPositionManager.atomLabelsList[atom_groups_ID[2]] )
+
                     if fill:
                         translation = np.mean([container_copy.AtomPositionManager.atomPositions[n] for n in selected_combination], axis=0)
                         r = self.get_probability(combination=combinations[selected_index], distribution='distance', 
                                                 AtomPositionManager=container_copy.AtomPositionManager, distances_dict=distances_dict, coefficient=1) / np.sum(group_numbers)
                         # mean distance for N point in a r radius circle
                         if verbose: print(f' - Fill with water | sphere r={r} c={translation}')
 
@@ -263,15 +276,15 @@
                             'colition_tolerance': 2.0,
                             'translation': translation,
                             'distribution':'center',
                             'wrap': True,
                             'verbose':verbose
                         }
                         container_copy = self.handleCLUSTER(values= {'ADD_SOLVENT':values}, containers=[container_copy])[0]
-
+                        
                 containers_new.append(container_copy)
                 if verbose: print(f' - Configuration generated (ok!)')
             
 
         self.containers = containers_new
 
         return containers_new
```

### Comparing `sage_lib-0.1.5.4/sage_lib/partition/partition_builder/Crystal_builder.py` & `sage_lib-0.1.5.5/sage_lib/partition/partition_builder/Crystal_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.4/sage_lib/partition/partition_builder/Dataset_builder.py` & `sage_lib-0.1.5.5/sage_lib/partition/partition_builder/Dataset_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.4/sage_lib/partition/partition_builder/Filter_builder.py` & `sage_lib-0.1.5.5/sage_lib/partition/partition_builder/Filter_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.4/sage_lib/partition/partition_builder/MolecularDynamic_builder.py` & `sage_lib-0.1.5.5/sage_lib/partition/partition_builder/MolecularDynamic_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.4/sage_lib/partition/partition_builder/MoleculeCluster_builder.py` & `sage_lib-0.1.5.5/sage_lib/partition/partition_builder/MoleculeCluster_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.4/sage_lib/partition/partition_builder/Molecule_builder.py` & `sage_lib-0.1.5.5/sage_lib/partition/partition_builder/Molecule_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.4/sage_lib/partition/partition_builder/PositionEditor_builder.py` & `sage_lib-0.1.5.5/sage_lib/partition/partition_builder/PositionEditor_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.4/sage_lib/partition/partition_builder/SupercellEmbedding_builder.py` & `sage_lib-0.1.5.5/sage_lib/partition/partition_builder/SupercellEmbedding_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.4/sage_lib/partition/partition_builder/SurfaceStates_builder.py` & `sage_lib-0.1.5.5/sage_lib/partition/partition_builder/SurfaceStates_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.4/sage_lib/partition/partition_builder/VacuumStates_builder.py` & `sage_lib-0.1.5.5/sage_lib/partition/partition_builder/VacuumStates_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.4/sage_lib/single_run/FF_Gap.py` & `sage_lib-0.1.5.5/sage_lib/single_run/FF_Gap.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.4/sage_lib/single_run/SingleRun.py` & `sage_lib-0.1.5.5/sage_lib/single_run/SingleRun.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.4/sage_lib/single_run/SingleRunDFT.py` & `sage_lib-0.1.5.5/sage_lib/single_run/SingleRunDFT.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.4/sage_lib/single_run/SingleRunManager.py` & `sage_lib-0.1.5.5/sage_lib/single_run/SingleRunManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.4/sage_lib.egg-info/SOURCES.txt` & `sage_lib-0.1.5.5/sage_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

