# Comparing `tmp/sc_file-3.4.0.tar.gz` & `tmp/sc_file-3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sc_file-3.4.0.tar", max compression
+gzip compressed data, was "sc_file-3.4.1.tar", max compression
```

## Comparing `sc_file-3.4.0.tar` & `sc_file-3.4.1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0     1083 2023-01-22 13:34:34.609366 sc_file-3.4.0/LICENSE
--rw-r--r--   0        0        0      761 2024-05-31 19:43:42.694589 sc_file-3.4.0/pyproject.toml
--rw-r--r--   0        0        0     5319 2024-05-31 19:37:39.692272 sc_file-3.4.0/README.md
--rw-r--r--   0        0        0      783 2024-05-28 23:10:58.160590 sc_file-3.4.0/scfile/__init__.py
--rw-r--r--   0        0        0       84 2024-05-17 09:56:37.842579 sc_file-3.4.0/scfile/__main__.py
--rw-r--r--   0        0        0        0 2024-05-28 23:10:58.160590 sc_file-3.4.0/scfile/cli/__init__.py
--rw-r--r--   0        0        0      235 2024-05-17 09:58:45.510767 sc_file-3.4.0/scfile/cli/consts.py
--rw-r--r--   0        0        0      584 2024-05-17 09:58:46.657772 sc_file-3.4.0/scfile/cli/convert.py
--rw-r--r--   0        0        0      912 2024-05-28 23:10:58.177580 sc_file-3.4.0/scfile/cli/default.py
--rw-r--r--   0        0        0     1219 2024-05-28 23:10:58.178580 sc_file-3.4.0/scfile/consts.py
--rw-r--r--   0        0        0     1087 2024-05-28 23:10:58.179579 sc_file-3.4.0/scfile/enums.py
--rw-r--r--   0        0        0      802 2024-05-28 23:10:58.180579 sc_file-3.4.0/scfile/exceptions/__init__.py
--rw-r--r--   0        0        0       84 2024-03-20 03:27:16.312140 sc_file-3.4.0/scfile/exceptions/base.py
--rw-r--r--   0        0        0     1414 2024-05-16 12:42:30.544943 sc_file-3.4.0/scfile/exceptions/basic.py
--rw-r--r--   0        0        0      647 2024-05-16 12:42:30.544943 sc_file-3.4.0/scfile/exceptions/decode.py
--rw-r--r--   0        0        0     1415 2024-05-16 12:42:30.545943 sc_file-3.4.0/scfile/exceptions/mcsa.py
--rw-r--r--   0        0        0      872 2024-05-16 12:42:30.545943 sc_file-3.4.0/scfile/exceptions/ol.py
--rw-r--r--   0        0        0      498 2024-05-28 23:10:58.181578 sc_file-3.4.0/scfile/file/__init__.py
--rw-r--r--   0        0        0      148 2024-05-28 23:10:58.182577 sc_file-3.4.0/scfile/file/base/__init__.py
--rw-r--r--   0        0        0     3190 2024-05-28 23:10:58.183577 sc_file-3.4.0/scfile/file/base/decoder.py
--rw-r--r--   0        0        0     1753 2024-05-28 23:10:58.184595 sc_file-3.4.0/scfile/file/base/encoder.py
--rw-r--r--   0        0        0      746 2024-05-28 23:10:58.185589 sc_file-3.4.0/scfile/file/base/file.py
--rw-r--r--   0        0        0      184 2024-05-28 23:10:58.226569 sc_file-3.4.0/scfile/file/data/__init__.py
--rw-r--r--   0        0        0       52 2024-05-28 23:10:58.249554 sc_file-3.4.0/scfile/file/data/base.py
--rw-r--r--   0        0        0      119 2024-05-28 23:10:58.249554 sc_file-3.4.0/scfile/file/data/image.py
--rw-r--r--   0        0        0      157 2024-05-28 23:10:58.256547 sc_file-3.4.0/scfile/file/data/model.py
--rw-r--r--   0        0        0      191 2024-05-31 19:37:39.736246 sc_file-3.4.0/scfile/file/data/texture.py
--rw-r--r--   0        0        0      458 2024-05-28 23:10:58.258534 sc_file-3.4.0/scfile/file/formats/__init__.py
--rw-r--r--   0        0        0       60 2024-05-28 23:10:58.259544 sc_file-3.4.0/scfile/file/formats/dae/__init__.py
--rw-r--r--   0        0        0     5656 2024-05-31 19:43:42.695589 sc_file-3.4.0/scfile/file/formats/dae/encoder.py
--rw-r--r--   0        0        0      289 2024-05-31 19:37:39.750235 sc_file-3.4.0/scfile/file/formats/dds/__init__.py
--rw-r--r--   0        0        0     2085 2024-05-31 19:37:39.768228 sc_file-3.4.0/scfile/file/formats/dds/encoder.py
--rw-r--r--   0        0        0     1070 2024-05-31 19:37:39.768228 sc_file-3.4.0/scfile/file/formats/dds/structure.py
--rw-r--r--   0        0        0      180 2024-05-28 23:10:58.297526 sc_file-3.4.0/scfile/file/formats/mcsa/__init__.py
--rw-r--r--   0        0        0     7904 2024-05-31 19:37:39.785218 sc_file-3.4.0/scfile/file/formats/mcsa/decoder.py
--rw-r--r--   0        0        0      654 2024-05-28 23:10:58.299534 sc_file-3.4.0/scfile/file/formats/mcsa/flags.py
--rw-r--r--   0        0        0      142 2024-05-31 19:37:39.794210 sc_file-3.4.0/scfile/file/formats/mcsa/versions.py
--rw-r--r--   0        0        0       60 2024-05-28 23:10:58.301524 sc_file-3.4.0/scfile/file/formats/mic/__init__.py
--rw-r--r--   0        0        0      577 2024-05-28 23:10:58.302530 sc_file-3.4.0/scfile/file/formats/mic/decoder.py
--rw-r--r--   0        0        0       68 2024-05-28 23:10:58.303510 sc_file-3.4.0/scfile/file/formats/ms3d/__init__.py
--rw-r--r--   0        0        0     5081 2024-05-28 23:10:58.304514 sc_file-3.4.0/scfile/file/formats/ms3d/encoder.py
--rw-r--r--   0        0        0       72 2024-05-28 23:10:58.305507 sc_file-3.4.0/scfile/file/formats/ms3d_ascii/__init__.py
--rw-r--r--   0        0        0     3897 2024-05-28 23:10:58.306506 sc_file-3.4.0/scfile/file/formats/ms3d_ascii/encoder.py
--rw-r--r--   0        0        0       60 2024-05-28 23:10:58.307509 sc_file-3.4.0/scfile/file/formats/obj/__init__.py
--rw-r--r--   0        0        0     1949 2024-05-28 23:10:58.319509 sc_file-3.4.0/scfile/file/formats/obj/encoder.py
--rw-r--r--   0        0        0      308 2024-05-31 19:37:39.794210 sc_file-3.4.0/scfile/file/formats/ol/__init__.py
--rw-r--r--   0        0        0      672 2024-05-31 19:37:39.795214 sc_file-3.4.0/scfile/file/formats/ol/converter/base.py
--rw-r--r--   0        0        0      182 2024-05-31 19:37:39.795214 sc_file-3.4.0/scfile/file/formats/ol/converter/bgra8.py
--rw-r--r--   0        0        0      233 2024-05-31 19:37:39.795214 sc_file-3.4.0/scfile/file/formats/ol/converter/rgba32f.py
--rw-r--r--   0        0        0     3729 2024-05-31 19:37:39.835190 sc_file-3.4.0/scfile/file/formats/ol/decoder.py
--rw-r--r--   0        0        0      135 2024-05-31 19:37:39.836172 sc_file-3.4.0/scfile/file/formats/ol/formats.py
--rw-r--r--   0        0        0       60 2024-05-28 23:10:58.365492 sc_file-3.4.0/scfile/file/formats/png/__init__.py
--rw-r--r--   0        0        0      280 2024-05-28 23:10:58.366472 sc_file-3.4.0/scfile/file/formats/png/encoder.py
--rw-r--r--   0        0        0      174 2024-05-28 23:10:58.402452 sc_file-3.4.0/scfile/io/__init__.py
--rw-r--r--   0        0        0     1578 2024-05-17 09:54:23.532231 sc_file-3.4.0/scfile/io/base.py
--rw-r--r--   0        0        0      254 2024-05-28 23:10:58.403469 sc_file-3.4.0/scfile/io/binary.py
--rw-r--r--   0        0        0     3709 2024-05-30 22:22:15.673031 sc_file-3.4.0/scfile/io/mcsa.py
--rw-r--r--   0        0        0      385 2024-05-31 19:37:39.836172 sc_file-3.4.0/scfile/io/ol.py
--rw-r--r--   0        0        0     4859 2024-05-31 19:37:39.850181 sc_file-3.4.0/scfile/utils/convert.py
--rw-r--r--   0        0        0      368 2024-05-28 23:10:58.445447 sc_file-3.4.0/scfile/utils/model/__init__.py
--rw-r--r--   0        0        0     1078 2024-05-28 23:10:58.446427 sc_file-3.4.0/scfile/utils/model/datatypes.py
--rw-r--r--   0        0        0     1288 2024-05-29 12:41:05.633019 sc_file-3.4.0/scfile/utils/model/mesh.py
--rw-r--r--   0        0        0     1624 2024-05-28 23:10:58.448427 sc_file-3.4.0/scfile/utils/model/model.py
--rw-r--r--   0        0        0     1707 2024-05-28 23:10:58.449426 sc_file-3.4.0/scfile/utils/model/skeleton.py
--rw-r--r--   0        0        0      122 2024-05-20 17:51:09.958151 sc_file-3.4.0/scfile/utils/types.py
--rw-r--r--   0        0        0     6870 1970-01-01 00:00:00.000000 sc_file-3.4.0/setup.py
--rw-r--r--   0        0        0     6056 1970-01-01 00:00:00.000000 sc_file-3.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-01-22 13:34:34.609366 sc_file-3.4.1/LICENSE
+-rw-r--r--   0        0        0      761 2024-05-31 19:45:14.459813 sc_file-3.4.1/pyproject.toml
+-rw-r--r--   0        0        0     5319 2024-05-31 19:37:39.692272 sc_file-3.4.1/README.md
+-rw-r--r--   0        0        0      783 2024-05-28 23:10:58.160590 sc_file-3.4.1/scfile/__init__.py
+-rw-r--r--   0        0        0       84 2024-05-17 09:56:37.842579 sc_file-3.4.1/scfile/__main__.py
+-rw-r--r--   0        0        0        0 2024-05-28 23:10:58.160590 sc_file-3.4.1/scfile/cli/__init__.py
+-rw-r--r--   0        0        0      235 2024-05-17 09:58:45.510767 sc_file-3.4.1/scfile/cli/consts.py
+-rw-r--r--   0        0        0      584 2024-05-17 09:58:46.657772 sc_file-3.4.1/scfile/cli/convert.py
+-rw-r--r--   0        0        0      912 2024-05-28 23:10:58.177580 sc_file-3.4.1/scfile/cli/default.py
+-rw-r--r--   0        0        0     1219 2024-05-28 23:10:58.178580 sc_file-3.4.1/scfile/consts.py
+-rw-r--r--   0        0        0     1087 2024-05-28 23:10:58.179579 sc_file-3.4.1/scfile/enums.py
+-rw-r--r--   0        0        0      802 2024-05-28 23:10:58.180579 sc_file-3.4.1/scfile/exceptions/__init__.py
+-rw-r--r--   0        0        0       84 2024-03-20 03:27:16.312140 sc_file-3.4.1/scfile/exceptions/base.py
+-rw-r--r--   0        0        0     1414 2024-05-16 12:42:30.544943 sc_file-3.4.1/scfile/exceptions/basic.py
+-rw-r--r--   0        0        0      647 2024-05-16 12:42:30.544943 sc_file-3.4.1/scfile/exceptions/decode.py
+-rw-r--r--   0        0        0     1415 2024-05-16 12:42:30.545943 sc_file-3.4.1/scfile/exceptions/mcsa.py
+-rw-r--r--   0        0        0      872 2024-05-16 12:42:30.545943 sc_file-3.4.1/scfile/exceptions/ol.py
+-rw-r--r--   0        0        0      498 2024-05-28 23:10:58.181578 sc_file-3.4.1/scfile/file/__init__.py
+-rw-r--r--   0        0        0      148 2024-05-28 23:10:58.182577 sc_file-3.4.1/scfile/file/base/__init__.py
+-rw-r--r--   0        0        0     3190 2024-05-28 23:10:58.183577 sc_file-3.4.1/scfile/file/base/decoder.py
+-rw-r--r--   0        0        0     1753 2024-05-28 23:10:58.184595 sc_file-3.4.1/scfile/file/base/encoder.py
+-rw-r--r--   0        0        0      746 2024-05-28 23:10:58.185589 sc_file-3.4.1/scfile/file/base/file.py
+-rw-r--r--   0        0        0      184 2024-05-28 23:10:58.226569 sc_file-3.4.1/scfile/file/data/__init__.py
+-rw-r--r--   0        0        0       52 2024-05-28 23:10:58.249554 sc_file-3.4.1/scfile/file/data/base.py
+-rw-r--r--   0        0        0      119 2024-05-28 23:10:58.249554 sc_file-3.4.1/scfile/file/data/image.py
+-rw-r--r--   0        0        0      157 2024-05-28 23:10:58.256547 sc_file-3.4.1/scfile/file/data/model.py
+-rw-r--r--   0        0        0      191 2024-05-31 19:37:39.736246 sc_file-3.4.1/scfile/file/data/texture.py
+-rw-r--r--   0        0        0      458 2024-05-28 23:10:58.258534 sc_file-3.4.1/scfile/file/formats/__init__.py
+-rw-r--r--   0        0        0       60 2024-05-28 23:10:58.259544 sc_file-3.4.1/scfile/file/formats/dae/__init__.py
+-rw-r--r--   0        0        0     4901 2024-05-31 19:45:09.918053 sc_file-3.4.1/scfile/file/formats/dae/encoder.py
+-rw-r--r--   0        0        0      289 2024-05-31 19:37:39.750235 sc_file-3.4.1/scfile/file/formats/dds/__init__.py
+-rw-r--r--   0        0        0     2085 2024-05-31 19:37:39.768228 sc_file-3.4.1/scfile/file/formats/dds/encoder.py
+-rw-r--r--   0        0        0     1070 2024-05-31 19:37:39.768228 sc_file-3.4.1/scfile/file/formats/dds/structure.py
+-rw-r--r--   0        0        0      180 2024-05-28 23:10:58.297526 sc_file-3.4.1/scfile/file/formats/mcsa/__init__.py
+-rw-r--r--   0        0        0     7904 2024-05-31 19:37:39.785218 sc_file-3.4.1/scfile/file/formats/mcsa/decoder.py
+-rw-r--r--   0        0        0      654 2024-05-28 23:10:58.299534 sc_file-3.4.1/scfile/file/formats/mcsa/flags.py
+-rw-r--r--   0        0        0      142 2024-05-31 19:37:39.794210 sc_file-3.4.1/scfile/file/formats/mcsa/versions.py
+-rw-r--r--   0        0        0       60 2024-05-28 23:10:58.301524 sc_file-3.4.1/scfile/file/formats/mic/__init__.py
+-rw-r--r--   0        0        0      577 2024-05-28 23:10:58.302530 sc_file-3.4.1/scfile/file/formats/mic/decoder.py
+-rw-r--r--   0        0        0       68 2024-05-28 23:10:58.303510 sc_file-3.4.1/scfile/file/formats/ms3d/__init__.py
+-rw-r--r--   0        0        0     5081 2024-05-28 23:10:58.304514 sc_file-3.4.1/scfile/file/formats/ms3d/encoder.py
+-rw-r--r--   0        0        0       72 2024-05-28 23:10:58.305507 sc_file-3.4.1/scfile/file/formats/ms3d_ascii/__init__.py
+-rw-r--r--   0        0        0     3897 2024-05-28 23:10:58.306506 sc_file-3.4.1/scfile/file/formats/ms3d_ascii/encoder.py
+-rw-r--r--   0        0        0       60 2024-05-28 23:10:58.307509 sc_file-3.4.1/scfile/file/formats/obj/__init__.py
+-rw-r--r--   0        0        0     1949 2024-05-28 23:10:58.319509 sc_file-3.4.1/scfile/file/formats/obj/encoder.py
+-rw-r--r--   0        0        0      308 2024-05-31 19:37:39.794210 sc_file-3.4.1/scfile/file/formats/ol/__init__.py
+-rw-r--r--   0        0        0      672 2024-05-31 19:37:39.795214 sc_file-3.4.1/scfile/file/formats/ol/converter/base.py
+-rw-r--r--   0        0        0      182 2024-05-31 19:37:39.795214 sc_file-3.4.1/scfile/file/formats/ol/converter/bgra8.py
+-rw-r--r--   0        0        0      233 2024-05-31 19:37:39.795214 sc_file-3.4.1/scfile/file/formats/ol/converter/rgba32f.py
+-rw-r--r--   0        0        0     3729 2024-05-31 19:37:39.835190 sc_file-3.4.1/scfile/file/formats/ol/decoder.py
+-rw-r--r--   0        0        0      135 2024-05-31 19:37:39.836172 sc_file-3.4.1/scfile/file/formats/ol/formats.py
+-rw-r--r--   0        0        0       60 2024-05-28 23:10:58.365492 sc_file-3.4.1/scfile/file/formats/png/__init__.py
+-rw-r--r--   0        0        0      280 2024-05-28 23:10:58.366472 sc_file-3.4.1/scfile/file/formats/png/encoder.py
+-rw-r--r--   0        0        0      174 2024-05-28 23:10:58.402452 sc_file-3.4.1/scfile/io/__init__.py
+-rw-r--r--   0        0        0     1578 2024-05-17 09:54:23.532231 sc_file-3.4.1/scfile/io/base.py
+-rw-r--r--   0        0        0      254 2024-05-28 23:10:58.403469 sc_file-3.4.1/scfile/io/binary.py
+-rw-r--r--   0        0        0     3709 2024-05-30 22:22:15.673031 sc_file-3.4.1/scfile/io/mcsa.py
+-rw-r--r--   0        0        0      385 2024-05-31 19:37:39.836172 sc_file-3.4.1/scfile/io/ol.py
+-rw-r--r--   0        0        0     4859 2024-05-31 19:37:39.850181 sc_file-3.4.1/scfile/utils/convert.py
+-rw-r--r--   0        0        0      368 2024-05-28 23:10:58.445447 sc_file-3.4.1/scfile/utils/model/__init__.py
+-rw-r--r--   0        0        0     1078 2024-05-28 23:10:58.446427 sc_file-3.4.1/scfile/utils/model/datatypes.py
+-rw-r--r--   0        0        0     1288 2024-05-29 12:41:05.633019 sc_file-3.4.1/scfile/utils/model/mesh.py
+-rw-r--r--   0        0        0     1624 2024-05-28 23:10:58.448427 sc_file-3.4.1/scfile/utils/model/model.py
+-rw-r--r--   0        0        0     1707 2024-05-28 23:10:58.449426 sc_file-3.4.1/scfile/utils/model/skeleton.py
+-rw-r--r--   0        0        0      122 2024-05-20 17:51:09.958151 sc_file-3.4.1/scfile/utils/types.py
+-rw-r--r--   0        0        0     6870 1970-01-01 00:00:00.000000 sc_file-3.4.1/setup.py
+-rw-r--r--   0        0        0     6056 1970-01-01 00:00:00.000000 sc_file-3.4.1/PKG-INFO
```

### Comparing `sc_file-3.4.0/LICENSE` & `sc_file-3.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sc_file-3.4.0/pyproject.toml` & `sc_file-3.4.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sc-file"
-version = "3.4.0"
+version = "3.4.1"
 description = "Utility & Library for decoding stalcraft assets"
 authors = ["onejeuu <mail@66rk.ru>"]
 
 license = "MIT"
 readme = "README.md"
 
 homepage = "https://github.com/onejeuu/sc-file"
```

### Comparing `sc_file-3.4.0/README.md` & `sc_file-3.4.1/README.md`

 * *Files identical despite different names*

### Comparing `sc_file-3.4.0/scfile/__init__.py` & `sc_file-3.4.1/scfile/__init__.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.4.0/scfile/cli/convert.py` & `sc_file-3.4.1/scfile/cli/convert.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.4.0/scfile/cli/default.py` & `sc_file-3.4.1/scfile/cli/default.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.4.0/scfile/consts.py` & `sc_file-3.4.1/scfile/consts.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.4.0/scfile/enums.py` & `sc_file-3.4.1/scfile/enums.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.4.0/scfile/exceptions/__init__.py` & `sc_file-3.4.1/scfile/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.4.0/scfile/exceptions/basic.py` & `sc_file-3.4.1/scfile/exceptions/basic.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.4.0/scfile/exceptions/decode.py` & `sc_file-3.4.1/scfile/exceptions/decode.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.4.0/scfile/exceptions/mcsa.py` & `sc_file-3.4.1/scfile/exceptions/mcsa.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.4.0/scfile/exceptions/ol.py` & `sc_file-3.4.1/scfile/exceptions/ol.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.4.0/scfile/file/base/decoder.py` & `sc_file-3.4.1/scfile/file/base/decoder.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.4.0/scfile/file/base/encoder.py` & `sc_file-3.4.1/scfile/file/base/encoder.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.4.0/scfile/file/base/file.py` & `sc_file-3.4.1/scfile/file/base/file.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.4.0/scfile/file/formats/dae/encoder.py` & `sc_file-3.4.1/scfile/file/formats/dae/encoder.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from typing import Any
 
 import numpy as np
 from numpy.typing import NDArray
 
 from scfile.file.base import FileEncoder
 from scfile.file.data import ModelData
-from scfile.utils.model.skeleton import Bone
 
 
 class DaeEncoder(FileEncoder[ModelData]):
     def serialize(self):
         self.model = self.data.model
         self.flags = self.data.model.flags
         self.skeleton = self.data.model.skeleton
@@ -134,31 +133,13 @@
 
         for mesh in self.model.meshes:
             node = etree.SubElement(
                 visual_scene, "node", id=f"{mesh.name}-node", name=mesh.name, type="NODE"
             )
             etree.SubElement(node, "instance_geometry", url=f"#{mesh.name}-mesh", name=mesh.name)
 
-        if self.flags.skeleton:
-            skeleton_node = etree.SubElement(
-                visual_scene, "node", id="skeleton-node", name="skeleton", type="NODE"
-            )
-
-            def add_bone(bone: Bone, parent_node: etree.Element):
-                node = etree.SubElement(
-                    parent_node, "node", id=f"{bone.name}-bone", name=bone.name, type="JOINT"
-                )
-                etree.SubElement(node, "translate").text = " ".join(map(str, bone.position))
-
-                for child in bone.children:
-                    add_bone(child, node)
-
-            root = self.skeleton.bones[0]
-            for child in root.children:
-                add_bone(child, skeleton_node)
-
         scene = etree.SubElement(self.root, "scene")
         etree.SubElement(scene, "instance_visual_scene", url="#scene")
 
     def _render_xml(self):
         etree.indent(self.root)
         self.buffer.write(etree.tostring(self.root))
```

### Comparing `sc_file-3.4.0/scfile/file/formats/dds/encoder.py` & `sc_file-3.4.1/scfile/file/formats/dds/encoder.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.4.0/scfile/file/formats/dds/structure.py` & `sc_file-3.4.1/scfile/file/formats/dds/structure.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.4.0/scfile/file/formats/mcsa/decoder.py` & `sc_file-3.4.1/scfile/file/formats/mcsa/decoder.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.4.0/scfile/file/formats/mcsa/flags.py` & `sc_file-3.4.1/scfile/file/formats/mcsa/flags.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.4.0/scfile/file/formats/mic/decoder.py` & `sc_file-3.4.1/scfile/file/formats/mic/decoder.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.4.0/scfile/file/formats/ms3d/encoder.py` & `sc_file-3.4.1/scfile/file/formats/ms3d/encoder.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.4.0/scfile/file/formats/ms3d_ascii/encoder.py` & `sc_file-3.4.1/scfile/file/formats/ms3d_ascii/encoder.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.4.0/scfile/file/formats/obj/encoder.py` & `sc_file-3.4.1/scfile/file/formats/obj/encoder.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.4.0/scfile/file/formats/ol/converter/base.py` & `sc_file-3.4.1/scfile/file/formats/ol/converter/base.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.4.0/scfile/file/formats/ol/decoder.py` & `sc_file-3.4.1/scfile/file/formats/ol/decoder.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.4.0/scfile/io/base.py` & `sc_file-3.4.1/scfile/io/base.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.4.0/scfile/io/mcsa.py` & `sc_file-3.4.1/scfile/io/mcsa.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.4.0/scfile/utils/convert.py` & `sc_file-3.4.1/scfile/utils/convert.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.4.0/scfile/utils/model/datatypes.py` & `sc_file-3.4.1/scfile/utils/model/datatypes.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.4.0/scfile/utils/model/mesh.py` & `sc_file-3.4.1/scfile/utils/model/mesh.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.4.0/scfile/utils/model/model.py` & `sc_file-3.4.1/scfile/utils/model/model.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.4.0/scfile/utils/model/skeleton.py` & `sc_file-3.4.1/scfile/utils/model/skeleton.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.4.0/setup.py` & `sc_file-3.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
  'quicktex>=0.2.0,<0.3.0']
 
 entry_points = \
 {'console_scripts': ['build = scripts.build:build']}
 
 setup_kwargs = {
     'name': 'sc-file',
-    'version': '3.4.0',
+    'version': '3.4.1',
     'description': 'Utility & Library for decoding stalcraft assets',
     'long_description': '# SC FILE\n\nUtility and Library for decoding and converting stalcraft assets files, such as models and textures into well-known formats.\n\nDesigned for artworks creation and the like.\n\n> [!NOTE]\n> There is not and will not be encoding back into game formats.\n\n> [!WARNING]\n> Do not use game assets directly. \\\n> Any changes in game client can be detected.\n\nYou can use executable program from [Releases](https://github.com/onejeuu/sc-file/releases) page.\n\n# 📁 Formats\n\n| Type    | Source        | Output                 |\n| ------- | ------------- | ---------------------- |\n| Model   | .mcsa / .mcvd | .obj, .dae, ms3d, .txt |\n| Texture | .ol           | .dds                   |\n| Image   | .mic          | .png                   |\n\nModel versions supported: 7.0, 8.0, 10.0\n\nModel animations `.mcvd` currently supports only meshes\n\nCollada model `.dae` skeleton currently unsupported\n\nTexture formats supported: DXT1, DXT3, DXT5, RGBA8, BGRA8, RGBA32F, DXN_XY\n\nTexture formats unsupported: Cubemaps (hdri, sky)\n\n# 💻 CLI Utility\n\n## Usage\n\nFrom bash:\n\n```bash\nscfile [FILES]... [OPTIONS]\n```\n\n> [!TIP]\n> You can just drag and drop one or multiple files onto `scfile.exe`.\n\n## Arguments\n\n- `FILES`: **List of file paths to be converted**. Multiple files should be separated by **spaces**. Accepts both full and relative paths. **Does not accept directory**.\n\n## Options\n\n- `-O`, `--output`: **One path to output file or directory**. Can be specified multiple times for different output files or directories. If not specified, file will be saved in same directory with a new suffix. You can specify multiple `FILES` and a single `--output` directory.\n\n## Examples\n\n1. Convert a single file:\n\n   ```bash\n   scfile file.mcsa\n   ```\n\n   _Will be saved in same directory with a new suffix._\n\n2. Convert a single file with a specified path or name:\n\n   ```bash\n   scfile file.mcsa --output path/to/file.obj\n   ```\n\n3. Convert multiple files to a specified directory:\n\n   ```bash\n   scfile file1.mcsa file2.mcsa --output path/to/dir\n   ```\n\n4. Convert multiple files with explicitly specified output files:\n\n   ```bash\n   scfile file1.mcsa file2.mcsa -O 1.obj -O 2.obj\n   ```\n\n   _If count of `FILES` and `--output` is different, as many files as possible will be converted._\n\n5. Convert all `.mcsa` files in current directory:\n\n   ```bash\n   scfile *.mcsa\n   ```\n\n   _In this case, `--output` accepts only a directory. Subdirectories are not included._\n\n6. Convert all `.mcsa` files with subdirectories to a specified directory:\n\n   ```bash\n   scfile **/*.mcsa -O path/to/dir\n   ```\n\n   _In this case, `--output` accepts only a directory. With `--output` specified, directory structure is not duplicated._\n\n# 📚 Library\n\n## Install\n\n### Pip\n\n```bash\npip install sc-file -U\n```\n\n### Manual\n\n```bash\ngit clone git@github.com:onejeuu/sc-file.git\n```\n\n```bash\ncd sc-file\n```\n\n```bash\npoetry install\n```\n\n## Usage\n\n### Simple\n\n```python\nfrom scfile import convert\n\n# Output path is optional.\n# Defaults to source path with new suffix.\nconvert.mcsa_to_obj("path/to/model.mcsa", "path/to/model.obj")\nconvert.ol_to_dds("path/to/texture.ol", "path/to/texture.dds")\nconvert.mic_to_png("path/to/image.mic", "path/to/image.png")\n\n# Skeleton support via MilkShape3D\nconvert.mcsa_to_ms3d("path/to/model.mcsa", "path/to/model.ms3d")\nconvert.mcsa_to_ms3d_ascii("path/to/model.mcsa", "path/to/model.txt")\n\n# Or determinate it automatically\nconvert.auto("path/to/model.mcsa")\n```\n\n### Advanced\n\n- Default\n\n```python\nfrom scfile.file.data import ModelData\nfrom scfile.file import McsaDecoder, ObjEncoder\n\nmcsa = McsaDecoder("model.mcsa")\ndata: ModelData = mcsa.decode()\nmcsa.close() # ? Necessary to close\n\nobj = ObjEncoder(data)\nobj.encode().save("model.obj") # ? Encoder closes after saving\n```\n\n- Use encoded content bytes\n\n```python\nobj = ObjEncoder(data)\nobj.encode()\n\nwith open("model.obj", "wb") as fp:\n    fp.write(obj.content)\n\nobj.close() # ? Necessary to close\n```\n\n- Use convert methods\n\n```python\nmcsa = McsaDecoder("model.mcsa")\nmcsa.convert_to(ObjEncoder).save("model.obj")\nmcsa.close() # ? Necessary to close\n```\n\n```python\nmcsa = McsaDecoder("model.mcsa")\nmcsa.to_obj().save("model.obj")\nmcsa.close() # ? Necessary to close\n```\n\n- Use context manager\n\n```python\nwith McsaDecoder("model.mcsa") as mcsa:\n    data: ModelData = mcsa.decode()\n\nwith ObjEncoder(data) as obj:\n    obj.encode().save("model.obj")\n```\n\n- Use context manager + convert methods\n\n```python\nwith McsaDecoder("model.mcsa") as mcsa:\n    obj = mcsa.convert_to(ObjEncoder)\n    obj.close()\n```\n\n```python\nwith McsaDecoder("model.mcsa") as mcsa:\n    mcsa.to_obj().save("model.obj")\n```\n\n> [!IMPORTANT]\n> When using `convert_to` buffer remains open. \\\n> `close()` or `save()` or another context (`with`) is necessary.\n\n- Save multiple copies\n\n```python\nwith McsaDecoder("model.mcsa") as mcsa:\n    with mcsa.to_obj() as obj:\n        obj.save_as("model_1.obj")\n        obj.save_as("model_2.obj")\n```\n\n# 🛠️ Build\n\n> [!IMPORTANT]\n> You will need [poetry](https://python-poetry.org) to do compilation.\n\n> [!TIP]\n> Recommended to create virtual environment.\n>\n> ```bash\n> poetry shell\n> ```\n\nThen install dependencies:\n\n```bash\npoetry install\n```\n\nAnd run script to compile:\n\n```bash\npoetry run build\n```\n\nExecutable file will be created in `/dist` directory.\n',
     'author': 'onejeuu',
     'author_email': 'mail@66rk.ru',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/onejeuu/sc-file',
```

### Comparing `sc_file-3.4.0/PKG-INFO` & `sc_file-3.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sc-file
-Version: 3.4.0
+Version: 3.4.1
 Summary: Utility & Library for decoding stalcraft assets
 Home-page: https://github.com/onejeuu/sc-file
 License: MIT
 Author: onejeuu
 Author-email: mail@66rk.ru
 Requires-Python: >=3.11,<3.13
 Classifier: License :: OSI Approved :: MIT License
```

