# Comparing `tmp/aperturedb-0.4.8.tar.gz` & `tmp/aperturedb-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aperturedb-0.4.8.tar", last modified: Fri Aug 11 13:17:27 2023, max compression
+gzip compressed data, was "aperturedb-0.4.9.tar", last modified: Wed Sep  6 13:46:54 2023, max compression
```

## Comparing `aperturedb-0.4.8.tar` & `aperturedb-0.4.9.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-11 13:17:27.770107 aperturedb-0.4.8/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-08-10 20:49:03.000000 aperturedb-0.4.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2065 2023-08-11 13:17:27.770107 aperturedb-0.4.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1550 2023-08-10 20:49:03.000000 aperturedb-0.4.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-11 13:17:27.770107 aperturedb-0.4.8/aperturedb/
--rw-r--r--   0 root         (0) root         (0)     4443 2023-08-10 20:49:03.000000 aperturedb-0.4.8/aperturedb/BBoxDataCSV.py
--rw-r--r--   0 root         (0) root         (0)     2846 2023-08-10 20:49:03.000000 aperturedb-0.4.8/aperturedb/BlobDataCSV.py
--rw-r--r--   0 root         (0) root         (0)    12177 2023-08-10 20:49:03.000000 aperturedb-0.4.8/aperturedb/BlobNewestDataCSV.py
--rw-r--r--   0 root         (0) root         (0)      126 2023-08-10 20:49:03.000000 aperturedb-0.4.8/aperturedb/Blobs.py
--rw-r--r--   0 root         (0) root         (0)      141 2023-08-10 20:49:03.000000 aperturedb-0.4.8/aperturedb/BoundingBoxes.py
--rw-r--r--   0 root         (0) root         (0)     6037 2023-08-10 20:49:03.000000 aperturedb-0.4.8/aperturedb/CSVParser.py
--rw-r--r--   0 root         (0) root         (0)      392 2023-08-10 20:49:03.000000 aperturedb-0.4.8/aperturedb/Configuration.py
--rw-r--r--   0 root         (0) root         (0)     5052 2023-08-10 20:49:03.000000 aperturedb-0.4.8/aperturedb/ConnectionDataCSV.py
--rw-r--r--   0 root         (0) root         (0)    14669 2023-08-10 20:49:03.000000 aperturedb-0.4.8/aperturedb/Connector.py
--rw-r--r--   0 root         (0) root         (0)     6243 2023-08-10 20:49:03.000000 aperturedb-0.4.8/aperturedb/ConnectorRest.py
--rw-r--r--   0 root         (0) root         (0)     2212 2023-08-10 20:49:03.000000 aperturedb-0.4.8/aperturedb/Constraints.py
--rw-r--r--   0 root         (0) root         (0)     3561 2023-08-10 20:49:03.000000 aperturedb-0.4.8/aperturedb/DaskManager.py
--rw-r--r--   0 root         (0) root         (0)     5334 2023-08-10 20:49:03.000000 aperturedb-0.4.8/aperturedb/DescriptorDataCSV.py
--rw-r--r--   0 root         (0) root         (0)     3255 2023-08-10 20:49:03.000000 aperturedb-0.4.8/aperturedb/DescriptorSetDataCSV.py
--rw-r--r--   0 root         (0) root         (0)     9263 2023-08-10 20:49:03.000000 aperturedb-0.4.8/aperturedb/Entities.py
--rw-r--r--   0 root         (0) root         (0)     4074 2023-08-10 20:49:03.000000 aperturedb-0.4.8/aperturedb/EntityDataCSV.py
--rw-r--r--   0 root         (0) root         (0)     5831 2023-08-10 20:49:03.000000 aperturedb-0.4.8/aperturedb/EntityUpdateDataCSV.py
--rw-r--r--   0 root         (0) root         (0)    15910 2023-08-10 20:49:03.000000 aperturedb-0.4.8/aperturedb/ImageDataCSV.py
--rw-r--r--   0 root         (0) root         (0)     4846 2023-08-10 20:49:03.000000 aperturedb-0.4.8/aperturedb/ImageDownloader.py
--rw-r--r--   0 root         (0) root         (0)    21437 2023-08-10 20:49:03.000000 aperturedb-0.4.8/aperturedb/Images.py
--rw-r--r--   0 root         (0) root         (0)     6494 2023-08-10 20:49:03.000000 aperturedb-0.4.8/aperturedb/KaggleData.py
--rw-r--r--   0 root         (0) root         (0)     4859 2023-08-10 20:49:03.000000 aperturedb-0.4.8/aperturedb/NotebookHelpers.py
--rw-r--r--   0 root         (0) root         (0)      546 2023-08-10 20:49:03.000000 aperturedb-0.4.8/aperturedb/Operations.py
--rw-r--r--   0 root         (0) root         (0)     4263 2023-08-10 20:49:03.000000 aperturedb-0.4.8/aperturedb/ParallelLoader.py
--rw-r--r--   0 root         (0) root         (0)    13570 2023-08-10 20:49:03.000000 aperturedb-0.4.8/aperturedb/ParallelQuery.py
--rw-r--r--   0 root         (0) root         (0)    19370 2023-08-10 20:49:03.000000 aperturedb-0.4.8/aperturedb/ParallelQuerySet.py
--rw-r--r--   0 root         (0) root         (0)     2261 2023-08-10 20:49:03.000000 aperturedb-0.4.8/aperturedb/Parallelizer.py
--rw-r--r--   0 root         (0) root         (0)     4014 2023-08-10 20:49:03.000000 aperturedb-0.4.8/aperturedb/PolygonDataCSV.py
--rw-r--r--   0 root         (0) root         (0)     1995 2023-08-10 20:49:03.000000 aperturedb-0.4.8/aperturedb/Polygons.py
--rw-r--r--   0 root         (0) root         (0)     3138 2023-08-10 20:49:03.000000 aperturedb-0.4.8/aperturedb/ProgressBar.py
--rw-r--r--   0 root         (0) root         (0)     4961 2023-08-10 20:49:03.000000 aperturedb-0.4.8/aperturedb/PyTorchDataset.py
--rw-r--r--   0 root         (0) root         (0)      917 2023-08-10 20:49:03.000000 aperturedb-0.4.8/aperturedb/PytorchData.py
--rw-r--r--   0 root         (0) root         (0)     9952 2023-08-10 20:49:03.000000 aperturedb-0.4.8/aperturedb/Query.py
--rw-r--r--   0 root         (0) root         (0)      246 2023-08-10 20:49:03.000000 aperturedb-0.4.8/aperturedb/QueryGenerator.py
--rw-r--r--   0 root         (0) root         (0)     1086 2023-08-10 20:49:03.000000 aperturedb-0.4.8/aperturedb/QueryTypes.py
--rw-r--r--   0 root         (0) root         (0)      263 2023-08-10 20:49:03.000000 aperturedb-0.4.8/aperturedb/Sort.py
--rw-r--r--   0 root         (0) root         (0)     2622 2023-08-10 20:49:03.000000 aperturedb-0.4.8/aperturedb/SparseAddingDataCSV.py
--rw-r--r--   0 root         (0) root         (0)      432 2023-08-10 20:49:03.000000 aperturedb-0.4.8/aperturedb/Stats.py
--rw-r--r--   0 root         (0) root         (0)     2054 2023-08-10 20:49:03.000000 aperturedb-0.4.8/aperturedb/Subscriptable.py
--rw-r--r--   0 root         (0) root         (0)    19835 2023-08-10 20:49:03.000000 aperturedb-0.4.8/aperturedb/Utils.py
--rw-r--r--   0 root         (0) root         (0)     2898 2023-08-10 20:49:03.000000 aperturedb-0.4.8/aperturedb/VideoDataCSV.py
--rw-r--r--   0 root         (0) root         (0)     3887 2023-08-10 20:49:03.000000 aperturedb-0.4.8/aperturedb/VideoDownloader.py
--rw-r--r--   0 root         (0) root         (0)     1126 2023-08-10 20:49:03.000000 aperturedb-0.4.8/aperturedb/Videos.py
--rw-r--r--   0 root         (0) root         (0)     1411 2023-08-11 12:42:52.000000 aperturedb-0.4.8/aperturedb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-11 13:17:27.770107 aperturedb-0.4.8/aperturedb/cli/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-10 20:49:03.000000 aperturedb-0.4.8/aperturedb/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)      709 2023-08-10 20:49:03.000000 aperturedb-0.4.8/aperturedb/cli/adb.py
--rw-r--r--   0 root         (0) root         (0)     6668 2023-08-10 20:49:03.000000 aperturedb-0.4.8/aperturedb/cli/configure.py
--rw-r--r--   0 root         (0) root         (0)       54 2023-08-10 20:49:03.000000 aperturedb-0.4.8/aperturedb/cli/console.py
--rw-r--r--   0 root         (0) root         (0)     2528 2023-08-10 20:49:03.000000 aperturedb-0.4.8/aperturedb/cli/ingest.py
--rw-r--r--   0 root         (0) root         (0)      534 2023-08-10 20:49:03.000000 aperturedb-0.4.8/aperturedb/cli/transact.py
--rw-r--r--   0 root         (0) root         (0)      860 2023-08-10 20:49:03.000000 aperturedb-0.4.8/aperturedb/cli/utilities.py
--rw-r--r--   0 root         (0) root         (0)     2942 2023-08-10 20:49:03.000000 aperturedb-0.4.8/aperturedb/queryMessage_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-11 13:17:27.770107 aperturedb-0.4.8/aperturedb.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2065 2023-08-11 13:17:27.000000 aperturedb-0.4.8/aperturedb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1996 2023-08-11 13:17:27.000000 aperturedb-0.4.8/aperturedb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-11 13:17:27.000000 aperturedb-0.4.8/aperturedb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       48 2023-08-11 13:17:27.000000 aperturedb-0.4.8/aperturedb.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      212 2023-08-11 13:17:27.000000 aperturedb-0.4.8/aperturedb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-08-11 13:17:27.000000 aperturedb-0.4.8/aperturedb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-11 13:17:27.770107 aperturedb-0.4.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1635 2023-08-11 12:42:52.000000 aperturedb-0.4.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-11 13:17:27.770107 aperturedb-0.4.8/test/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-10 20:49:03.000000 aperturedb-0.4.8/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9432 2023-08-10 20:49:03.000000 aperturedb-0.4.8/test/conftest.py
--rw-r--r--   0 root         (0) root         (0)      195 2023-08-10 20:49:03.000000 aperturedb-0.4.8/test/dbinfo.py
--rw-r--r--   0 root         (0) root         (0)      641 2023-08-10 20:49:03.000000 aperturedb-0.4.8/test/download_images.py
--rw-r--r--   0 root         (0) root         (0)     5929 2023-08-10 20:49:03.000000 aperturedb-0.4.8/test/generateImages.py
--rw-r--r--   0 root         (0) root         (0)    25438 2023-08-10 20:49:03.000000 aperturedb-0.4.8/test/generateInput.py
--rw-r--r--   0 root         (0) root         (0)     1129 2023-08-10 20:49:03.000000 aperturedb-0.4.8/test/mark_checker.py
--rw-r--r--   0 root         (0) root         (0)    14799 2023-08-10 20:49:03.000000 aperturedb-0.4.8/test/test_CLI.py
--rw-r--r--   0 root         (0) root         (0)    15375 2023-08-10 20:49:03.000000 aperturedb-0.4.8/test/test_Data.py
--rw-r--r--   0 root         (0) root         (0)     6363 2023-08-10 20:49:03.000000 aperturedb-0.4.8/test/test_Datawizard.py
--rw-r--r--   0 root         (0) root         (0)     5358 2023-08-10 20:49:03.000000 aperturedb-0.4.8/test/test_ResponseHandler.py
--rw-r--r--   0 root         (0) root         (0)      944 2023-08-10 20:49:03.000000 aperturedb-0.4.8/test/test_Server.py
--rw-r--r--   0 root         (0) root         (0)     1261 2023-08-10 20:49:03.000000 aperturedb-0.4.8/test/test_Session.py
--rw-r--r--   0 root         (0) root         (0)     1837 2023-08-10 20:49:03.000000 aperturedb-0.4.8/test/test_Stats.py
--rw-r--r--   0 root         (0) root         (0)     1963 2023-08-10 20:49:03.000000 aperturedb-0.4.8/test/test_Success.py
--rw-r--r--   0 root         (0) root         (0)      264 2023-08-10 20:49:03.000000 aperturedb-0.4.8/test/test_Utils.py
--rw-r--r--   0 root         (0) root         (0)     4909 2023-08-10 20:49:03.000000 aperturedb-0.4.8/test/test_kaggle.py
--rw-r--r--   0 root         (0) root         (0)     4292 2023-08-10 20:49:03.000000 aperturedb-0.4.8/test/test_torch_connector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-06 13:46:54.034733 aperturedb-0.4.9/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-08-18 20:28:12.000000 aperturedb-0.4.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2065 2023-09-06 13:46:54.034733 aperturedb-0.4.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1550 2023-08-18 20:28:12.000000 aperturedb-0.4.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-06 13:46:54.034733 aperturedb-0.4.9/aperturedb/
+-rw-r--r--   0 root         (0) root         (0)     4443 2023-08-18 20:28:12.000000 aperturedb-0.4.9/aperturedb/BBoxDataCSV.py
+-rw-r--r--   0 root         (0) root         (0)     2846 2023-08-18 20:28:12.000000 aperturedb-0.4.9/aperturedb/BlobDataCSV.py
+-rw-r--r--   0 root         (0) root         (0)    12177 2023-08-18 20:28:12.000000 aperturedb-0.4.9/aperturedb/BlobNewestDataCSV.py
+-rw-r--r--   0 root         (0) root         (0)      126 2023-08-18 20:28:12.000000 aperturedb-0.4.9/aperturedb/Blobs.py
+-rw-r--r--   0 root         (0) root         (0)      141 2023-08-18 20:28:12.000000 aperturedb-0.4.9/aperturedb/BoundingBoxes.py
+-rw-r--r--   0 root         (0) root         (0)     6037 2023-08-18 20:28:12.000000 aperturedb-0.4.9/aperturedb/CSVParser.py
+-rw-r--r--   0 root         (0) root         (0)      392 2023-08-18 20:28:12.000000 aperturedb-0.4.9/aperturedb/Configuration.py
+-rw-r--r--   0 root         (0) root         (0)     5052 2023-08-18 20:28:12.000000 aperturedb-0.4.9/aperturedb/ConnectionDataCSV.py
+-rw-r--r--   0 root         (0) root         (0)    15051 2023-08-28 20:18:12.000000 aperturedb-0.4.9/aperturedb/Connector.py
+-rw-r--r--   0 root         (0) root         (0)     6260 2023-08-28 20:18:12.000000 aperturedb-0.4.9/aperturedb/ConnectorRest.py
+-rw-r--r--   0 root         (0) root         (0)     2212 2023-08-18 20:28:12.000000 aperturedb-0.4.9/aperturedb/Constraints.py
+-rw-r--r--   0 root         (0) root         (0)     3561 2023-08-18 20:28:12.000000 aperturedb-0.4.9/aperturedb/DaskManager.py
+-rw-r--r--   0 root         (0) root         (0)     5334 2023-08-18 20:28:12.000000 aperturedb-0.4.9/aperturedb/DescriptorDataCSV.py
+-rw-r--r--   0 root         (0) root         (0)     3255 2023-08-18 20:28:12.000000 aperturedb-0.4.9/aperturedb/DescriptorSetDataCSV.py
+-rw-r--r--   0 root         (0) root         (0)     9263 2023-08-18 20:28:12.000000 aperturedb-0.4.9/aperturedb/Entities.py
+-rw-r--r--   0 root         (0) root         (0)     4074 2023-08-18 20:28:12.000000 aperturedb-0.4.9/aperturedb/EntityDataCSV.py
+-rw-r--r--   0 root         (0) root         (0)     5831 2023-08-18 20:28:12.000000 aperturedb-0.4.9/aperturedb/EntityUpdateDataCSV.py
+-rw-r--r--   0 root         (0) root         (0)    15910 2023-08-18 20:28:12.000000 aperturedb-0.4.9/aperturedb/ImageDataCSV.py
+-rw-r--r--   0 root         (0) root         (0)     4846 2023-08-18 20:28:12.000000 aperturedb-0.4.9/aperturedb/ImageDownloader.py
+-rw-r--r--   0 root         (0) root         (0)    21437 2023-08-18 20:28:12.000000 aperturedb-0.4.9/aperturedb/Images.py
+-rw-r--r--   0 root         (0) root         (0)     6498 2023-08-29 17:45:21.000000 aperturedb-0.4.9/aperturedb/KaggleData.py
+-rw-r--r--   0 root         (0) root         (0)     4859 2023-08-18 20:28:12.000000 aperturedb-0.4.9/aperturedb/NotebookHelpers.py
+-rw-r--r--   0 root         (0) root         (0)      546 2023-08-18 20:28:12.000000 aperturedb-0.4.9/aperturedb/Operations.py
+-rw-r--r--   0 root         (0) root         (0)     4263 2023-08-18 20:28:12.000000 aperturedb-0.4.9/aperturedb/ParallelLoader.py
+-rw-r--r--   0 root         (0) root         (0)    13570 2023-08-18 20:28:12.000000 aperturedb-0.4.9/aperturedb/ParallelQuery.py
+-rw-r--r--   0 root         (0) root         (0)    19370 2023-08-18 20:28:12.000000 aperturedb-0.4.9/aperturedb/ParallelQuerySet.py
+-rw-r--r--   0 root         (0) root         (0)     2261 2023-08-18 20:28:12.000000 aperturedb-0.4.9/aperturedb/Parallelizer.py
+-rw-r--r--   0 root         (0) root         (0)     4045 2023-08-29 17:45:21.000000 aperturedb-0.4.9/aperturedb/PolygonDataCSV.py
+-rw-r--r--   0 root         (0) root         (0)     1995 2023-08-18 20:28:12.000000 aperturedb-0.4.9/aperturedb/Polygons.py
+-rw-r--r--   0 root         (0) root         (0)     3138 2023-08-18 20:28:12.000000 aperturedb-0.4.9/aperturedb/ProgressBar.py
+-rw-r--r--   0 root         (0) root         (0)     4961 2023-08-18 20:28:12.000000 aperturedb-0.4.9/aperturedb/PyTorchDataset.py
+-rw-r--r--   0 root         (0) root         (0)      917 2023-08-18 20:28:12.000000 aperturedb-0.4.9/aperturedb/PytorchData.py
+-rw-r--r--   0 root         (0) root         (0)     9964 2023-08-30 13:35:40.000000 aperturedb-0.4.9/aperturedb/Query.py
+-rw-r--r--   0 root         (0) root         (0)      246 2023-08-18 20:28:12.000000 aperturedb-0.4.9/aperturedb/QueryGenerator.py
+-rw-r--r--   0 root         (0) root         (0)     1086 2023-08-18 20:28:12.000000 aperturedb-0.4.9/aperturedb/QueryTypes.py
+-rw-r--r--   0 root         (0) root         (0)      263 2023-08-18 20:28:12.000000 aperturedb-0.4.9/aperturedb/Sort.py
+-rw-r--r--   0 root         (0) root         (0)     2622 2023-08-18 20:28:12.000000 aperturedb-0.4.9/aperturedb/SparseAddingDataCSV.py
+-rw-r--r--   0 root         (0) root         (0)      432 2023-08-18 20:28:12.000000 aperturedb-0.4.9/aperturedb/Stats.py
+-rw-r--r--   0 root         (0) root         (0)     2054 2023-08-18 20:28:12.000000 aperturedb-0.4.9/aperturedb/Subscriptable.py
+-rw-r--r--   0 root         (0) root         (0)    19835 2023-09-05 21:08:58.000000 aperturedb-0.4.9/aperturedb/Utils.py
+-rw-r--r--   0 root         (0) root         (0)     2898 2023-08-18 20:28:12.000000 aperturedb-0.4.9/aperturedb/VideoDataCSV.py
+-rw-r--r--   0 root         (0) root         (0)     3887 2023-08-18 20:28:12.000000 aperturedb-0.4.9/aperturedb/VideoDownloader.py
+-rw-r--r--   0 root         (0) root         (0)     1126 2023-08-18 20:28:12.000000 aperturedb-0.4.9/aperturedb/Videos.py
+-rw-r--r--   0 root         (0) root         (0)     1411 2023-09-05 21:08:58.000000 aperturedb-0.4.9/aperturedb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-06 13:46:54.034733 aperturedb-0.4.9/aperturedb/cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-18 20:28:12.000000 aperturedb-0.4.9/aperturedb/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      709 2023-08-18 20:28:12.000000 aperturedb-0.4.9/aperturedb/cli/adb.py
+-rw-r--r--   0 root         (0) root         (0)     6668 2023-08-18 20:28:12.000000 aperturedb-0.4.9/aperturedb/cli/configure.py
+-rw-r--r--   0 root         (0) root         (0)       54 2023-08-18 20:28:12.000000 aperturedb-0.4.9/aperturedb/cli/console.py
+-rw-r--r--   0 root         (0) root         (0)     2528 2023-08-18 20:28:12.000000 aperturedb-0.4.9/aperturedb/cli/ingest.py
+-rw-r--r--   0 root         (0) root         (0)      534 2023-08-18 20:28:12.000000 aperturedb-0.4.9/aperturedb/cli/transact.py
+-rw-r--r--   0 root         (0) root         (0)      860 2023-08-18 20:28:12.000000 aperturedb-0.4.9/aperturedb/cli/utilities.py
+-rw-r--r--   0 root         (0) root         (0)     2942 2023-08-18 20:28:12.000000 aperturedb-0.4.9/aperturedb/queryMessage_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-06 13:46:54.034733 aperturedb-0.4.9/aperturedb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2065 2023-09-06 13:46:54.000000 aperturedb-0.4.9/aperturedb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1996 2023-09-06 13:46:54.000000 aperturedb-0.4.9/aperturedb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-09-06 13:46:54.000000 aperturedb-0.4.9/aperturedb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2023-09-06 13:46:54.000000 aperturedb-0.4.9/aperturedb.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      212 2023-09-06 13:46:54.000000 aperturedb-0.4.9/aperturedb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-09-06 13:46:54.000000 aperturedb-0.4.9/aperturedb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-09-06 13:46:54.034733 aperturedb-0.4.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1635 2023-09-05 21:08:58.000000 aperturedb-0.4.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-06 13:46:54.034733 aperturedb-0.4.9/test/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-18 20:28:12.000000 aperturedb-0.4.9/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9695 2023-08-28 20:18:12.000000 aperturedb-0.4.9/test/conftest.py
+-rw-r--r--   0 root         (0) root         (0)      195 2023-08-18 20:28:12.000000 aperturedb-0.4.9/test/dbinfo.py
+-rw-r--r--   0 root         (0) root         (0)      641 2023-08-18 20:28:12.000000 aperturedb-0.4.9/test/download_images.py
+-rw-r--r--   0 root         (0) root         (0)     5929 2023-08-18 20:28:12.000000 aperturedb-0.4.9/test/generateImages.py
+-rw-r--r--   0 root         (0) root         (0)    25438 2023-08-18 20:28:12.000000 aperturedb-0.4.9/test/generateInput.py
+-rw-r--r--   0 root         (0) root         (0)     1129 2023-08-18 20:28:12.000000 aperturedb-0.4.9/test/mark_checker.py
+-rw-r--r--   0 root         (0) root         (0)    14799 2023-08-18 20:28:12.000000 aperturedb-0.4.9/test/test_CLI.py
+-rw-r--r--   0 root         (0) root         (0)    15375 2023-08-18 20:28:12.000000 aperturedb-0.4.9/test/test_Data.py
+-rw-r--r--   0 root         (0) root         (0)     6363 2023-08-18 20:28:12.000000 aperturedb-0.4.9/test/test_Datawizard.py
+-rw-r--r--   0 root         (0) root         (0)     5358 2023-08-18 20:28:12.000000 aperturedb-0.4.9/test/test_ResponseHandler.py
+-rw-r--r--   0 root         (0) root         (0)      944 2023-08-18 20:28:12.000000 aperturedb-0.4.9/test/test_Server.py
+-rw-r--r--   0 root         (0) root         (0)     2457 2023-08-28 20:18:12.000000 aperturedb-0.4.9/test/test_Session.py
+-rw-r--r--   0 root         (0) root         (0)     1837 2023-08-18 20:28:12.000000 aperturedb-0.4.9/test/test_Stats.py
+-rw-r--r--   0 root         (0) root         (0)     1963 2023-08-18 20:28:12.000000 aperturedb-0.4.9/test/test_Success.py
+-rw-r--r--   0 root         (0) root         (0)      265 2023-09-05 21:11:29.000000 aperturedb-0.4.9/test/test_Utils.py
+-rw-r--r--   0 root         (0) root         (0)     4909 2023-08-18 20:28:12.000000 aperturedb-0.4.9/test/test_kaggle.py
+-rw-r--r--   0 root         (0) root         (0)     4292 2023-08-18 20:28:12.000000 aperturedb-0.4.9/test/test_torch_connector.py
```

### Comparing `aperturedb-0.4.8/LICENSE` & `aperturedb-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.8/PKG-INFO` & `aperturedb-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aperturedb
-Version: 0.4.8
+Version: 0.4.9
 Summary: ApertureDB Client Module
 Home-page: https://github.com/aperture-data/aperturedb-python
 Author: Luis Remis
 Author-email: luis@aperturedata.io
 License: Apache
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aperturedb-0.4.8/README.md` & `aperturedb-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.8/aperturedb/BBoxDataCSV.py` & `aperturedb-0.4.9/aperturedb/BBoxDataCSV.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.8/aperturedb/BlobDataCSV.py` & `aperturedb-0.4.9/aperturedb/BlobDataCSV.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.8/aperturedb/BlobNewestDataCSV.py` & `aperturedb-0.4.9/aperturedb/BlobNewestDataCSV.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.8/aperturedb/CSVParser.py` & `aperturedb-0.4.9/aperturedb/CSVParser.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.8/aperturedb/ConnectionDataCSV.py` & `aperturedb-0.4.9/aperturedb/ConnectionDataCSV.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.8/aperturedb/Connector.py` & `aperturedb-0.4.9/aperturedb/Connector.py`

 * *Files 4% similar despite different names*

```diff
@@ -203,15 +203,15 @@
     def _refresh_token(self):
         query = [{
             "RefreshToken": {
                 "refresh_token": self.shared_data.session.refresh_token
             }
         }]
 
-        response, _ = self._query(query, [])
+        response, _ = self._query(query, [], try_resume=False)
 
         logger.info(f"Refresh token response: \r\n{response}")
         if isinstance(response, list):
             session_info = response[0]["RefreshToken"]
             if session_info["status"] != 0:
                 raise UnauthorizedException(response)
 
@@ -277,15 +277,15 @@
             self.conn.close()
             self.connected = False
             raise ConnectionError(
                 f"Failed to connect to ApertureDB {self.config}")
 
         self.connected = True
 
-    def _query(self, query, blob_array = []):
+    def _query(self, query, blob_array = [], try_resume=True):
         response_blob_array = []
         # Check the query type
         if not isinstance(query, str):  # assumes json
             query_str = json.dumps(query)
         else:
             query_str = query
 
@@ -324,15 +324,20 @@
                 logger.warning(f"Socket error on process {os.getpid()}")
             tries += 1
             logger.warning(
                 f"Connection broken. Reconnectng attempt [{tries}/3] .. PID = {os.getpid()}")
             time.sleep(1)
             self.conn.close()
             self._connect()
-            self._renew_session()
+            # Try to resume the session, in cases where the connection is severed.
+            # For example aperturedb server is restarted, or network is lost.
+            # While this is useful bit of code, when executed in a refresh token
+            # path, this can cause a deadlock. Hence the try_resume flag.
+            if try_resume:
+                self._renew_session()
         if tries == 3:
             raise Exception(
                 f"Could not query apertureDB using TCP.")
         return (self.last_response, response_blob_array)
 
     def query(self, q, blobs=[]):
         """
```

### Comparing `aperturedb-0.4.8/aperturedb/ConnectorRest.py` & `aperturedb-0.4.9/aperturedb/ConnectorRest.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,15 +132,15 @@
         else:
             self.shared_data = shared_data
 
     def __del__(self):
         logger.info("Done with connector")
         self.http_session.close()
 
-    def _query(self, query, blob_array = []):
+    def _query(self, query, blob_array = [], try_resume=True):
         response_blob_array = []
         # Check the query type
         if not isinstance(query, str):  # assumes json
             query_str = json.dumps(query)
         else:
             query_str = query
```

### Comparing `aperturedb-0.4.8/aperturedb/Constraints.py` & `aperturedb-0.4.9/aperturedb/Constraints.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.8/aperturedb/DaskManager.py` & `aperturedb-0.4.9/aperturedb/DaskManager.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.8/aperturedb/DescriptorDataCSV.py` & `aperturedb-0.4.9/aperturedb/DescriptorDataCSV.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.8/aperturedb/DescriptorSetDataCSV.py` & `aperturedb-0.4.9/aperturedb/DescriptorSetDataCSV.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.8/aperturedb/Entities.py` & `aperturedb-0.4.9/aperturedb/Entities.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.8/aperturedb/EntityDataCSV.py` & `aperturedb-0.4.9/aperturedb/EntityDataCSV.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.8/aperturedb/EntityUpdateDataCSV.py` & `aperturedb-0.4.9/aperturedb/EntityUpdateDataCSV.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.8/aperturedb/ImageDataCSV.py` & `aperturedb-0.4.9/aperturedb/ImageDataCSV.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.8/aperturedb/ImageDownloader.py` & `aperturedb-0.4.9/aperturedb/ImageDownloader.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.8/aperturedb/Images.py` & `aperturedb-0.4.9/aperturedb/Images.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.8/aperturedb/KaggleData.py` & `aperturedb-0.4.9/aperturedb/KaggleData.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 from aperturedb.Subscriptable import Subscriptable
 
 
 class KaggleData(Subscriptable):
     """
     **Class to wrap around a Dataset retrieved from kaggle**
 
-    A DataSet downloaded from kaggle does not implement a standard mechanism to iterate over it's values
-    This class intends to provide an abstracion like that of a pytorch dataset.
-    Where the iteration over Dataset elements yields an atomic record.
+    A DataSet downloaded from kaggle does not implement a standard mechanism to iterate over its values
+    This class intends to provide an abstracion like that of a pytorch dataset
+    where the iteration over Dataset elements yields an atomic record.
 
     .. note::
-        This class should be subclassed with specefic implementations of generate_index and generate_query.
+        This class should be subclassed with specific implementations of generate_index and generate_query.
 
     Example subclass:
 
     ``` python
 
         class CelebADataKaggle(KaggleData):
            def __init__(self, **kwargs) -> None:
@@ -90,15 +90,15 @@
                blob = open(image_file_name, "rb").read()
                embedding = self.embedding_generator(Image.open(image_file_name))
                serialized = embedding.cpu().detach().numpy().tobytes()
                return q, [blob, serialized]
     ```
 
         Args:
-            dataset_ref (str): URL of kaggle dataset, for example 'https://www.kaggle.com/datasets/crawford/cat-dataset'
+            dataset_ref (str): URL of kaggle dataset, for example https://www.kaggle.com/datasets/jessicali9530/celeba-dataset
             records_count (int): number of records to provide to generate.
 
     """
 
     def __init__(
             self,
             dataset_ref: str,
```

### Comparing `aperturedb-0.4.8/aperturedb/NotebookHelpers.py` & `aperturedb-0.4.9/aperturedb/NotebookHelpers.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.8/aperturedb/Operations.py` & `aperturedb-0.4.9/aperturedb/Operations.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.8/aperturedb/ParallelLoader.py` & `aperturedb-0.4.9/aperturedb/ParallelLoader.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.8/aperturedb/ParallelQuery.py` & `aperturedb-0.4.9/aperturedb/ParallelQuery.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.8/aperturedb/ParallelQuerySet.py` & `aperturedb-0.4.9/aperturedb/ParallelQuerySet.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.8/aperturedb/Parallelizer.py` & `aperturedb-0.4.9/aperturedb/Parallelizer.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.8/aperturedb/PolygonDataCSV.py` & `aperturedb-0.4.9/aperturedb/PolygonDataCSV.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
     **POLYGON_PROPERTY_I**: declares the name of a property that will be assigned to all polygon objects. Any number of properties can be declared in this way.
 
     **constraint_POLYGON_PROPERTY_I**: declares that POLYGON_PROPERTY_I should be unique, and that a new polygon will not be added if there already exists one with the same value for this property. For each row, the value in this column should match the value in column POLYGON_PROPERTY_I.
 
     **_label**: optionally applies a label to the polygon objects.
 
-    **polygons**: a JSON array of polygon regions. Each polygon region is itself an array of [x,y] vertices that describe the boundary of a single contiguous polygon. See also https://docs.aperturedata.io/parameters/polygons.html.
+    **polygons**: a JSON array of polygon regions. Each polygon region is itself an array of [x,y] vertices that describe the boundary of a single contiguous polygon. See also [Polygon API parameter](query_language/Reference/shared_command_parameters/polygons).
 
     Example csv file::
 
         image_id,polygon_id,constraint_polygon_id,category_id,_label,polygons
         397133,82445,82445,44,bottle,"[[[224.24, 297.18], [228.29, 297.18], ...]]"
         397133,119568,119568,67,dining table,"[[[292.37, 425.1], [340.6, 373.86], ...]]"
         ...
```

### Comparing `aperturedb-0.4.8/aperturedb/Polygons.py` & `aperturedb-0.4.9/aperturedb/Polygons.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.8/aperturedb/ProgressBar.py` & `aperturedb-0.4.9/aperturedb/ProgressBar.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.8/aperturedb/PyTorchDataset.py` & `aperturedb-0.4.9/aperturedb/PyTorchDataset.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.8/aperturedb/PytorchData.py` & `aperturedb-0.4.9/aperturedb/PytorchData.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.8/aperturedb/Query.py` & `aperturedb-0.4.9/aperturedb/Query.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from aperturedb.Constraints import Constraints
 from aperturedb.Sort import Sort
 from pydantic import BaseModel
 
 
 class ObjectType(Enum):
     """
-    Based on : https://docs.aperturedata.io/API-Description.html
+    Based on : [API description](/query_language/Overview/API%20Description)
 
     """
     BLOB = "_Blob"
     BOUNDING_BOX = "_BoundingBox"
     CONNECTION = "_Connection"
     DESCRIPTOR = "_Descriptor"
     DESCRIPTORSET = "_DescriptorSet"
```

### Comparing `aperturedb-0.4.8/aperturedb/QueryTypes.py` & `aperturedb-0.4.9/aperturedb/QueryTypes.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.8/aperturedb/SparseAddingDataCSV.py` & `aperturedb-0.4.9/aperturedb/SparseAddingDataCSV.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.8/aperturedb/Subscriptable.py` & `aperturedb-0.4.9/aperturedb/Subscriptable.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.8/aperturedb/Utils.py` & `aperturedb-0.4.9/aperturedb/Utils.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.8/aperturedb/VideoDataCSV.py` & `aperturedb-0.4.9/aperturedb/VideoDataCSV.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.8/aperturedb/VideoDownloader.py` & `aperturedb-0.4.9/aperturedb/VideoDownloader.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.8/aperturedb/Videos.py` & `aperturedb-0.4.9/aperturedb/Videos.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.8/aperturedb/__init__.py` & `aperturedb-0.4.9/aperturedb/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import datetime
 import os
 import json
 import requests
 
 logger = logging.getLogger(__name__)
 
-__version__ = "0.4.8"
+__version__ = "0.4.9"
 
 # set log level
 logger.setLevel(logging.DEBUG)
 formatter    = logging.Formatter(
     "%(asctime)s : %(levelname)s : %(name)s : %(thread)d : %(lineno)d : %(message)s")
 
 log_file_level = logging.getLevelName(os.getenv("LOG_FILE_LEVEL", "WARN"))
```

### Comparing `aperturedb-0.4.8/aperturedb/cli/adb.py` & `aperturedb-0.4.9/aperturedb/cli/adb.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.8/aperturedb/cli/configure.py` & `aperturedb-0.4.9/aperturedb/cli/configure.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.8/aperturedb/cli/ingest.py` & `aperturedb-0.4.9/aperturedb/cli/ingest.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.8/aperturedb/cli/transact.py` & `aperturedb-0.4.9/aperturedb/cli/transact.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.8/aperturedb/cli/utilities.py` & `aperturedb-0.4.9/aperturedb/cli/utilities.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.8/aperturedb/queryMessage_pb2.py` & `aperturedb-0.4.9/aperturedb/queryMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.8/aperturedb.egg-info/PKG-INFO` & `aperturedb-0.4.9/aperturedb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aperturedb
-Version: 0.4.8
+Version: 0.4.9
 Summary: ApertureDB Client Module
 Home-page: https://github.com/aperture-data/aperturedb-python
 Author: Luis Remis
 Author-email: luis@aperturedata.io
 License: Apache
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aperturedb-0.4.8/aperturedb.egg-info/SOURCES.txt` & `aperturedb-0.4.9/aperturedb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.8/setup.py` & `aperturedb-0.4.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
                     'ipywidgets==8.0.4'
                     ]
 if OPENCV_VERSION is None:
     install_requires.append('opencv-python')
 
 setuptools.setup(
     name="aperturedb",
-    version="0.4.8",
+    version="0.4.9",
     description="ApertureDB Client Module",
     install_requires=install_requires,
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/aperture-data/aperturedb-python",
     license="Apache",
     packages=setuptools.find_packages(),
```

### Comparing `aperturedb-0.4.8/test/conftest.py` & `aperturedb-0.4.9/test/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,17 +27,23 @@
     if "db" in metafunc.fixturenames:
         metafunc.parametrize("db", [
             {"db": Connector(
                 host = dbinfo.DB_TCP_HOST,
                 port = dbinfo.DB_TCP_PORT,
                 user = dbinfo.DB_USER,
                 password = dbinfo.DB_PASSWORD,
-                use_ssl = True)}
-
-        ], indirect=True, ids=["TCP"])
+                use_ssl = True)},
+            {"db": ConnectorRest(
+                host = dbinfo.DB_REST_HOST,
+                port = dbinfo.DB_REST_PORT,
+                user = dbinfo.DB_USER,
+                password = dbinfo.DB_PASSWORD,
+                use_ssl = False
+            )}
+        ], indirect=True, ids=["TCP", "HTTP"])
     if all(func in metafunc.fixturenames for func in ["insert_data_from_csv", "modify_data_from_csv"]) and \
             metafunc.module.__name__ in ["test.test_Data"]:
         metafunc.parametrize("insert_data_from_csv,modify_data_from_csv", [
                              [True, True], [False, False]], indirect=True, ids=["with_dask", "without_dask"])
     elif "insert_data_from_csv" in metafunc.fixturenames and metafunc.module.__name__ in \
             ["test.test_Data"]:
         metafunc.parametrize("insert_data_from_csv", [
```

### Comparing `aperturedb-0.4.8/test/download_images.py` & `aperturedb-0.4.9/test/download_images.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.8/test/generateImages.py` & `aperturedb-0.4.9/test/generateImages.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.8/test/generateInput.py` & `aperturedb-0.4.9/test/generateInput.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.8/test/mark_checker.py` & `aperturedb-0.4.9/test/mark_checker.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.8/test/test_CLI.py` & `aperturedb-0.4.9/test/test_CLI.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.8/test/test_Data.py` & `aperturedb-0.4.9/test/test_Data.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.8/test/test_Datawizard.py` & `aperturedb-0.4.9/test/test_Datawizard.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.8/test/test_ResponseHandler.py` & `aperturedb-0.4.9/test/test_ResponseHandler.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.8/test/test_Server.py` & `aperturedb-0.4.9/test/test_Server.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.8/test/test_Stats.py` & `aperturedb-0.4.9/test/test_Stats.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.8/test/test_Success.py` & `aperturedb-0.4.9/test/test_Success.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.8/test/test_kaggle.py` & `aperturedb-0.4.9/test/test_kaggle.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.8/test/test_torch_connector.py` & `aperturedb-0.4.9/test/test_torch_connector.py`

 * *Files identical despite different names*

