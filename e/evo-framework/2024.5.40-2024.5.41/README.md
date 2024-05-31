# Comparing `tmp/evo_framework-2024.5.40.tar.gz` & `tmp/evo_framework-2024.5.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evo_framework-2024.5.40.tar", max compression
+gzip compressed data, was "evo_framework-2024.5.41.tar", max compression
```

## Comparing `evo_framework-2024.5.40.tar` & `evo_framework-2024.5.41.tar`

### file list

```diff
@@ -1,75 +1,73 @@
--rw-r--r--   0        0        0    13525 2024-05-28 16:27:09.302451 evo_framework-2024.5.40/LICENSE.txt
--rw-r--r--   0        0        0      406 2024-05-28 16:35:10.344754 evo_framework-2024.5.40/README.md
--rwxr-xr-x   0        0        0      770 2024-05-29 23:15:57.646008 evo_framework-2024.5.40/evo_framework/__init__.py
--rwxr-xr-x   0        0        0     4030 2024-04-14 21:01:20.000000 evo_framework-2024.5.40/evo_framework/control/CObject.py
--rwxr-xr-x   0        0        0       51 2024-05-29 23:15:57.849272 evo_framework-2024.5.40/evo_framework/control/__init__.py
--rw-r--r--   0        0        0      399 2024-05-28 10:42:13.864068 evo_framework-2024.5.40/evo_framework/core/__init__.py
--rwxr-xr-x   0        0        0      160 2024-05-29 23:15:57.645990 evo_framework-2024.5.40/evo_framework/core/evo_core_api/__init__.py
--rw-r--r--   0        0        0     2651 2024-05-31 13:29:39.297670 evo_framework-2024.5.40/evo_framework/core/evo_core_api/automation/entity.yaml
--rw-r--r--   0        0        0     6058 2024-05-29 23:52:16.739992 evo_framework-2024.5.40/evo_framework/core/evo_core_api/control/CApi.py
--rw-r--r--   0        0        0    25500 2024-05-31 14:22:31.688287 evo_framework-2024.5.40/evo_framework/core/evo_core_api/control/CApiFlow.py
--rw-r--r--   0        0        0      131 2024-05-29 23:15:57.840551 evo_framework-2024.5.40/evo_framework/core/evo_core_api/control/__init__.py
--rw-r--r--   0        0        0     3387 2024-05-31 19:10:00.435649 evo_framework-2024.5.40/evo_framework/core/evo_core_api/entity/EAction.py
--rw-r--r--   0        0        0     1306 2024-05-29 23:15:57.646050 evo_framework-2024.5.40/evo_framework/core/evo_core_api/entity/EActionTask.py
--rw-r--r--   0        0        0     1770 2024-05-29 23:38:23.561186 evo_framework-2024.5.40/evo_framework/core/evo_core_api/entity/EApi.py
--rw-r--r--   0        0        0     1781 2024-05-29 23:42:56.957602 evo_framework-2024.5.40/evo_framework/core/evo_core_api/entity/EApiAudio.py
--rw-r--r--   0        0        0     3060 2024-05-29 23:29:47.211002 evo_framework-2024.5.40/evo_framework/core/evo_core_api/entity/EApiConfig.py
--rw-r--r--   0        0        0     2669 2024-05-31 19:03:54.323051 evo_framework-2024.5.40/evo_framework/core/evo_core_api/entity/EApiFile.py
--rw-r--r--   0        0        0     1816 2024-05-31 19:04:06.221218 evo_framework-2024.5.40/evo_framework/core/evo_core_api/entity/EApiImage.py
--rw-r--r--   0        0        0     1800 2024-05-31 19:04:13.300985 evo_framework-2024.5.40/evo_framework/core/evo_core_api/entity/EApiVideo.py
--rwxr-xr-x   0        0        0     2474 2024-05-31 13:30:23.336888 evo_framework-2024.5.40/evo_framework/core/evo_core_api/entity/ERequest.py
--rwxr-xr-x   0        0        0     2189 2024-05-30 17:16:17.766668 evo_framework-2024.5.40/evo_framework/core/evo_core_api/entity/EResponse.py
--rw-r--r--   0        0        0      568 2024-05-29 23:04:53.300310 evo_framework-2024.5.40/evo_framework/core/evo_core_api/entity/EnumApiAction.py
--rw-r--r--   0        0        0      101 2024-03-22 09:24:36.000000 evo_framework-2024.5.40/evo_framework/core/evo_core_api/entity/EnumApiCompress.py
--rw-r--r--   0        0        0       97 2024-03-22 09:18:53.000000 evo_framework-2024.5.40/evo_framework/core/evo_core_api/entity/EnumApiCrypto.py
--rw-r--r--   0        0        0      274 2024-05-28 15:31:41.321728 evo_framework-2024.5.40/evo_framework/core/evo_core_api/entity/EnumApiType.py
--rw-r--r--   0        0        0      493 2024-05-29 23:04:53.308461 evo_framework-2024.5.40/evo_framework/core/evo_core_api/entity/EnumApiVisibility.py
--rw-r--r--   0        0        0        0 2024-05-27 12:52:18.397976 evo_framework-2024.5.40/evo_framework/core/evo_core_api/entity/EnumLanguage.py
--rwxr-xr-x   0        0        0     1502 2024-05-29 23:16:21.970731 evo_framework-2024.5.40/evo_framework/core/evo_core_api/entity/__init__.py
--rwxr-xr-x   0        0        0    11914 2024-05-31 17:42:52.571236 evo_framework-2024.5.40/evo_framework/core/evo_core_api/utility/IuApi.py
--rw-r--r--   0        0        0    14944 2024-05-29 23:15:57.840524 evo_framework-2024.5.40/evo_framework/core/evo_core_api/utility/IuApiPb.py
--rwxr-xr-x   0        0        0       64 2024-05-29 23:15:57.840493 evo_framework-2024.5.40/evo_framework/core/evo_core_api/utility/__init__.py
--rwxr-xr-x   0        0        0      215 2024-05-29 23:15:57.848203 evo_framework-2024.5.40/evo_framework/core/evo_core_binary/__init__.py
--rwxr-xr-x   0        0        0      120 2021-11-24 10:46:35.000000 evo_framework-2024.5.40/evo_framework/core/evo_core_binary/entity/IBinary.py
--rwxr-xr-x   0        0        0     9089 2024-05-29 23:15:57.849286 evo_framework-2024.5.40/evo_framework/core/evo_core_binary/utility/IuBinary.py
--rw-r--r--   0        0        0     6658 2024-05-29 23:15:57.848274 evo_framework-2024.5.40/evo_framework/core/evo_core_binary/utility/IuBinaryAsync.py
--rw-r--r--   0        0        0     7700 2024-05-30 20:17:43.461565 evo_framework-2024.5.40/evo_framework/core/evo_core_binary/utility/UBinary.py
--rw-r--r--   0        0        0     1324 2024-05-29 23:15:57.844638 evo_framework-2024.5.40/evo_framework/core/evo_core_boot/control/CBoot.py
--rw-r--r--   0        0        0      281 2024-04-15 19:43:35.988232 evo_framework-2024.5.40/evo_framework/core/evo_core_bridge/IBridge.py
--rw-r--r--   0        0        0       75 2024-05-29 23:15:57.848167 evo_framework-2024.5.40/evo_framework/core/evo_core_convert/__init__.py
--rw-r--r--   0        0        0     6213 2024-05-29 23:54:10.283288 evo_framework-2024.5.40/evo_framework/core/evo_core_convert/test_evo_core_binary.py
--rw-r--r--   0        0        0      841 2024-04-12 09:23:48.000000 evo_framework-2024.5.40/evo_framework/core/evo_core_convert/utility/IuConvert.py
--rw-r--r--   0        0        0        0 2021-11-12 08:43:14.000000 evo_framework-2024.5.40/evo_framework/core/evo_core_convert/utility/__init__.py
--rw-r--r--   0        0        0      236 2024-05-29 23:15:57.848112 evo_framework-2024.5.40/evo_framework/core/evo_core_crypto/__init__.py
--rw-r--r--   0        0        0     1470 2024-03-26 15:03:45.000000 evo_framework-2024.5.40/evo_framework/core/evo_core_crypto/utility/IuCryptChacha.py
--rwxr-xr-x   0        0        0     1467 2024-05-29 23:15:57.848244 evo_framework-2024.5.40/evo_framework/core/evo_core_crypto/utility/IuCryptEC.py
--rwxr-xr-x   0        0        0      743 2024-03-17 11:26:36.000000 evo_framework-2024.5.40/evo_framework/core/evo_core_crypto/utility/IuCryptHash.py
--rw-r--r--   0        0        0     1332 2024-05-29 23:15:57.848017 evo_framework-2024.5.40/evo_framework/core/evo_core_file/entity/EFileChunk.py
--rw-r--r--   0        0        0      699 2024-05-29 23:15:57.848149 evo_framework-2024.5.40/evo_framework/core/evo_core_foundation/IFoundation.py
--rw-r--r--   0        0        0       63 2024-05-29 23:15:57.849413 evo_framework-2024.5.40/evo_framework/core/evo_core_key/__init__.py
--rw-r--r--   0        0        0      893 2024-05-29 23:15:57.844661 evo_framework-2024.5.40/evo_framework/core/evo_core_key/utility/IuKey.py
--rw-r--r--   0        0        0       63 2024-05-29 23:15:57.848179 evo_framework-2024.5.40/evo_framework/core/evo_core_log/__init__.py
--rw-r--r--   0        0        0     2150 2024-05-29 23:15:57.848192 evo_framework-2024.5.40/evo_framework/core/evo_core_log/utility/IuLog.py
--rw-r--r--   0        0        0     2289 2024-03-22 09:09:45.000000 evo_framework-2024.5.40/evo_framework/core/evo_core_log/utility/ULogger.py
--rwxr-xr-x   0        0        0      146 2024-05-29 23:15:57.848259 evo_framework-2024.5.40/evo_framework/core/evo_core_setting/__init__.py
--rw-r--r--   0        0        0     2813 2024-05-29 23:15:57.849237 evo_framework-2024.5.40/evo_framework/core/evo_core_setting/control/CSetting.py
--rwxr-xr-x   0        0        0        0 2024-01-05 09:11:06.000000 evo_framework-2024.5.40/evo_framework/core/evo_core_setting/control/__init__.py
--rw-r--r--   0        0        0     1201 2024-05-29 23:15:57.849250 evo_framework-2024.5.40/evo_framework/core/evo_core_setting/entity/ESetting.py
--rw-r--r--   0        0        0        0 2024-01-05 20:57:13.000000 evo_framework-2024.5.40/evo_framework/core/evo_core_setting/entity/__init__.py
--rw-r--r--   0        0        0       72 2024-05-29 23:15:57.848222 evo_framework-2024.5.40/evo_framework/core/evo_core_system/__init__.py
--rw-r--r--   0        0        0        0 2024-01-04 13:13:56.000000 evo_framework-2024.5.40/evo_framework/core/evo_core_system/control/__init__.py
--rw-r--r--   0        0        0     6742 2024-02-12 00:08:10.000000 evo_framework-2024.5.40/evo_framework/core/evo_core_system/utility/IuSystem.py
--rw-r--r--   0        0        0        0 2024-01-04 13:14:10.000000 evo_framework-2024.5.40/evo_framework/core/evo_core_system/utility/__init__.py
--rw-r--r--   0        0        0        0 2021-11-12 08:43:14.000000 evo_framework-2024.5.40/evo_framework/core/evo_core_type/__init__.py
--rwxr-xr-x   0        0        0      953 2024-04-22 18:31:06.740795 evo_framework-2024.5.40/evo_framework/core/evo_core_type/entity/EvoMap.py
--rw-r--r--   0        0        0       66 2024-05-29 23:15:57.849211 evo_framework-2024.5.40/evo_framework/core/evo_core_yaml/__init__.py
--rw-r--r--   0        0        0      304 2024-03-02 18:03:59.000000 evo_framework-2024.5.40/evo_framework/core/evo_core_yaml/utility/IuYaml.py
--rwxr-xr-x   0        0        0     9395 2024-05-29 23:15:57.849264 evo_framework-2024.5.40/evo_framework/entity/EObject.py
--rw-r--r--   0        0        0        0 2021-11-23 22:03:14.000000 evo_framework-2024.5.40/evo_framework/entity/IEObject.py
--rw-r--r--   0        0        0        0 2021-11-23 22:02:39.000000 evo_framework-2024.5.40/evo_framework/entity/IEvo.py
--rwxr-xr-x   0        0        0       64 2021-11-23 22:11:09.000000 evo_framework-2024.5.40/evo_framework/entity/Id.py
--rwxr-xr-x   0        0        0       62 2021-11-23 22:13:51.000000 evo_framework-2024.5.40/evo_framework/entity/Time.py
--rwxr-xr-x   0        0        0      181 2024-05-29 23:15:57.849324 evo_framework-2024.5.40/evo_framework/entity/__init__.py
--rwxr-xr-x   0        0        0        0 2024-01-14 01:56:17.000000 evo_framework-2024.5.40/evo_framework/utility/__init__.py
--rw-r--r--   0        0        0      557 2024-05-31 19:10:09.701236 evo_framework-2024.5.40/pyproject.toml
--rw-r--r--   0        0        0     1225 1970-01-01 00:00:00.000000 evo_framework-2024.5.40/PKG-INFO
+-rw-r--r--   0        0        0    13525 2024-05-28 16:27:09.302451 evo_framework-2024.5.41/LICENSE.txt
+-rw-r--r--   0        0        0      406 2024-05-28 16:35:10.344754 evo_framework-2024.5.41/README.md
+-rwxr-xr-x   0        0        0      770 2024-05-29 23:15:57.646008 evo_framework-2024.5.41/evo_framework/__init__.py
+-rwxr-xr-x   0        0        0     4030 2024-04-14 21:01:20.000000 evo_framework-2024.5.41/evo_framework/control/CObject.py
+-rwxr-xr-x   0        0        0       51 2024-05-29 23:15:57.849272 evo_framework-2024.5.41/evo_framework/control/__init__.py
+-rw-r--r--   0        0        0      399 2024-05-28 10:42:13.864068 evo_framework-2024.5.41/evo_framework/core/__init__.py
+-rwxr-xr-x   0        0        0      160 2024-05-29 23:15:57.645990 evo_framework-2024.5.41/evo_framework/core/evo_core_api/__init__.py
+-rw-r--r--   0        0        0     2332 2024-05-31 20:33:51.808286 evo_framework-2024.5.41/evo_framework/core/evo_core_api/automation/entity.yaml
+-rw-r--r--   0        0        0     6058 2024-05-29 23:52:16.739992 evo_framework-2024.5.41/evo_framework/core/evo_core_api/control/CApi.py
+-rw-r--r--   0        0        0    25500 2024-05-31 14:22:31.688287 evo_framework-2024.5.41/evo_framework/core/evo_core_api/control/CApiFlow.py
+-rw-r--r--   0        0        0      131 2024-05-29 23:15:57.840551 evo_framework-2024.5.41/evo_framework/core/evo_core_api/control/__init__.py
+-rw-r--r--   0        0        0     3344 2024-05-31 21:01:27.585493 evo_framework-2024.5.41/evo_framework/core/evo_core_api/entity/EAction.py
+-rw-r--r--   0        0        0     1306 2024-05-29 23:15:57.646050 evo_framework-2024.5.41/evo_framework/core/evo_core_api/entity/EActionTask.py
+-rw-r--r--   0        0        0     1770 2024-05-29 23:38:23.561186 evo_framework-2024.5.41/evo_framework/core/evo_core_api/entity/EApi.py
+-rw-r--r--   0        0        0     3029 2024-05-31 21:11:15.610746 evo_framework-2024.5.41/evo_framework/core/evo_core_api/entity/EApiConfig.py
+-rw-r--r--   0        0        0     2681 2024-05-31 21:16:03.003273 evo_framework-2024.5.41/evo_framework/core/evo_core_api/entity/EApiFile.py
+-rw-r--r--   0        0        0     1525 2024-05-31 21:08:35.640177 evo_framework-2024.5.41/evo_framework/core/evo_core_api/entity/EApiText.py
+-rwxr-xr-x   0        0        0     2491 2024-05-31 21:04:55.955198 evo_framework-2024.5.41/evo_framework/core/evo_core_api/entity/ERequest.py
+-rwxr-xr-x   0        0        0     2155 2024-05-31 21:07:11.505845 evo_framework-2024.5.41/evo_framework/core/evo_core_api/entity/EResponse.py
+-rw-r--r--   0        0        0      568 2024-05-29 23:04:53.300310 evo_framework-2024.5.41/evo_framework/core/evo_core_api/entity/EnumApiAction.py
+-rw-r--r--   0        0        0      101 2024-03-22 09:24:36.000000 evo_framework-2024.5.41/evo_framework/core/evo_core_api/entity/EnumApiCompress.py
+-rw-r--r--   0        0        0       97 2024-03-22 09:18:53.000000 evo_framework-2024.5.41/evo_framework/core/evo_core_api/entity/EnumApiCrypto.py
+-rw-r--r--   0        0        0      274 2024-05-28 15:31:41.321728 evo_framework-2024.5.41/evo_framework/core/evo_core_api/entity/EnumApiType.py
+-rw-r--r--   0        0        0      493 2024-05-29 23:04:53.308461 evo_framework-2024.5.41/evo_framework/core/evo_core_api/entity/EnumApiVisibility.py
+-rw-r--r--   0        0        0        0 2024-05-27 12:52:18.397976 evo_framework-2024.5.41/evo_framework/core/evo_core_api/entity/EnumLanguage.py
+-rwxr-xr-x   0        0        0     1574 2024-05-31 21:03:43.170559 evo_framework-2024.5.41/evo_framework/core/evo_core_api/entity/__init__.py
+-rwxr-xr-x   0        0        0     7848 2024-05-31 21:16:51.768317 evo_framework-2024.5.41/evo_framework/core/evo_core_api/utility/IuApi.py
+-rw-r--r--   0        0        0    14944 2024-05-29 23:15:57.840524 evo_framework-2024.5.41/evo_framework/core/evo_core_api/utility/IuApiPb.py
+-rwxr-xr-x   0        0        0       64 2024-05-29 23:15:57.840493 evo_framework-2024.5.41/evo_framework/core/evo_core_api/utility/__init__.py
+-rwxr-xr-x   0        0        0      215 2024-05-29 23:15:57.848203 evo_framework-2024.5.41/evo_framework/core/evo_core_binary/__init__.py
+-rwxr-xr-x   0        0        0      120 2021-11-24 10:46:35.000000 evo_framework-2024.5.41/evo_framework/core/evo_core_binary/entity/IBinary.py
+-rwxr-xr-x   0        0        0     9089 2024-05-29 23:15:57.849286 evo_framework-2024.5.41/evo_framework/core/evo_core_binary/utility/IuBinary.py
+-rw-r--r--   0        0        0     6658 2024-05-29 23:15:57.848274 evo_framework-2024.5.41/evo_framework/core/evo_core_binary/utility/IuBinaryAsync.py
+-rw-r--r--   0        0        0     7700 2024-05-30 20:17:43.461565 evo_framework-2024.5.41/evo_framework/core/evo_core_binary/utility/UBinary.py
+-rw-r--r--   0        0        0     1324 2024-05-29 23:15:57.844638 evo_framework-2024.5.41/evo_framework/core/evo_core_boot/control/CBoot.py
+-rw-r--r--   0        0        0      281 2024-04-15 19:43:35.988232 evo_framework-2024.5.41/evo_framework/core/evo_core_bridge/IBridge.py
+-rw-r--r--   0        0        0       75 2024-05-29 23:15:57.848167 evo_framework-2024.5.41/evo_framework/core/evo_core_convert/__init__.py
+-rw-r--r--   0        0        0     6213 2024-05-29 23:54:10.283288 evo_framework-2024.5.41/evo_framework/core/evo_core_convert/test_evo_core_binary.py
+-rw-r--r--   0        0        0      841 2024-04-12 09:23:48.000000 evo_framework-2024.5.41/evo_framework/core/evo_core_convert/utility/IuConvert.py
+-rw-r--r--   0        0        0        0 2021-11-12 08:43:14.000000 evo_framework-2024.5.41/evo_framework/core/evo_core_convert/utility/__init__.py
+-rw-r--r--   0        0        0      236 2024-05-29 23:15:57.848112 evo_framework-2024.5.41/evo_framework/core/evo_core_crypto/__init__.py
+-rw-r--r--   0        0        0     1470 2024-03-26 15:03:45.000000 evo_framework-2024.5.41/evo_framework/core/evo_core_crypto/utility/IuCryptChacha.py
+-rwxr-xr-x   0        0        0     1467 2024-05-29 23:15:57.848244 evo_framework-2024.5.41/evo_framework/core/evo_core_crypto/utility/IuCryptEC.py
+-rwxr-xr-x   0        0        0      743 2024-03-17 11:26:36.000000 evo_framework-2024.5.41/evo_framework/core/evo_core_crypto/utility/IuCryptHash.py
+-rw-r--r--   0        0        0     1332 2024-05-29 23:15:57.848017 evo_framework-2024.5.41/evo_framework/core/evo_core_file/entity/EFileChunk.py
+-rw-r--r--   0        0        0      699 2024-05-29 23:15:57.848149 evo_framework-2024.5.41/evo_framework/core/evo_core_foundation/IFoundation.py
+-rw-r--r--   0        0        0       63 2024-05-29 23:15:57.849413 evo_framework-2024.5.41/evo_framework/core/evo_core_key/__init__.py
+-rw-r--r--   0        0        0      893 2024-05-29 23:15:57.844661 evo_framework-2024.5.41/evo_framework/core/evo_core_key/utility/IuKey.py
+-rw-r--r--   0        0        0       63 2024-05-29 23:15:57.848179 evo_framework-2024.5.41/evo_framework/core/evo_core_log/__init__.py
+-rw-r--r--   0        0        0     2150 2024-05-29 23:15:57.848192 evo_framework-2024.5.41/evo_framework/core/evo_core_log/utility/IuLog.py
+-rw-r--r--   0        0        0     2289 2024-03-22 09:09:45.000000 evo_framework-2024.5.41/evo_framework/core/evo_core_log/utility/ULogger.py
+-rwxr-xr-x   0        0        0      146 2024-05-29 23:15:57.848259 evo_framework-2024.5.41/evo_framework/core/evo_core_setting/__init__.py
+-rw-r--r--   0        0        0     2813 2024-05-29 23:15:57.849237 evo_framework-2024.5.41/evo_framework/core/evo_core_setting/control/CSetting.py
+-rwxr-xr-x   0        0        0        0 2024-01-05 09:11:06.000000 evo_framework-2024.5.41/evo_framework/core/evo_core_setting/control/__init__.py
+-rw-r--r--   0        0        0     1201 2024-05-29 23:15:57.849250 evo_framework-2024.5.41/evo_framework/core/evo_core_setting/entity/ESetting.py
+-rw-r--r--   0        0        0        0 2024-01-05 20:57:13.000000 evo_framework-2024.5.41/evo_framework/core/evo_core_setting/entity/__init__.py
+-rw-r--r--   0        0        0       72 2024-05-29 23:15:57.848222 evo_framework-2024.5.41/evo_framework/core/evo_core_system/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-04 13:13:56.000000 evo_framework-2024.5.41/evo_framework/core/evo_core_system/control/__init__.py
+-rw-r--r--   0        0        0     6742 2024-02-12 00:08:10.000000 evo_framework-2024.5.41/evo_framework/core/evo_core_system/utility/IuSystem.py
+-rw-r--r--   0        0        0        0 2024-01-04 13:14:10.000000 evo_framework-2024.5.41/evo_framework/core/evo_core_system/utility/__init__.py
+-rw-r--r--   0        0        0        0 2021-11-12 08:43:14.000000 evo_framework-2024.5.41/evo_framework/core/evo_core_type/__init__.py
+-rwxr-xr-x   0        0        0      953 2024-04-22 18:31:06.740795 evo_framework-2024.5.41/evo_framework/core/evo_core_type/entity/EvoMap.py
+-rw-r--r--   0        0        0       66 2024-05-29 23:15:57.849211 evo_framework-2024.5.41/evo_framework/core/evo_core_yaml/__init__.py
+-rw-r--r--   0        0        0      304 2024-03-02 18:03:59.000000 evo_framework-2024.5.41/evo_framework/core/evo_core_yaml/utility/IuYaml.py
+-rwxr-xr-x   0        0        0     9395 2024-05-29 23:15:57.849264 evo_framework-2024.5.41/evo_framework/entity/EObject.py
+-rw-r--r--   0        0        0        0 2021-11-23 22:03:14.000000 evo_framework-2024.5.41/evo_framework/entity/IEObject.py
+-rw-r--r--   0        0        0        0 2021-11-23 22:02:39.000000 evo_framework-2024.5.41/evo_framework/entity/IEvo.py
+-rwxr-xr-x   0        0        0       64 2021-11-23 22:11:09.000000 evo_framework-2024.5.41/evo_framework/entity/Id.py
+-rwxr-xr-x   0        0        0       62 2021-11-23 22:13:51.000000 evo_framework-2024.5.41/evo_framework/entity/Time.py
+-rwxr-xr-x   0        0        0      181 2024-05-29 23:15:57.849324 evo_framework-2024.5.41/evo_framework/entity/__init__.py
+-rwxr-xr-x   0        0        0        0 2024-01-14 01:56:17.000000 evo_framework-2024.5.41/evo_framework/utility/__init__.py
+-rw-r--r--   0        0        0      583 2024-05-31 21:17:28.143465 evo_framework-2024.5.41/pyproject.toml
+-rw-r--r--   0        0        0     1271 1970-01-01 00:00:00.000000 evo_framework-2024.5.41/PKG-INFO
```

### Comparing `evo_framework-2024.5.40/LICENSE.txt` & `evo_framework-2024.5.41/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.40/evo_framework/__init__.py` & `evo_framework-2024.5.41/evo_framework/__init__.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.40/evo_framework/control/CObject.py` & `evo_framework-2024.5.41/evo_framework/control/CObject.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.40/evo_framework/core/evo_core_api/automation/entity.yaml` & `evo_framework-2024.5.41/evo_framework/core/evo_core_api/automation/entity.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -28,108 +28,88 @@
     DOUBLE
     BYTE
     BYTES
     BOOL
     EOBJECT
     MAP
     ENUM
-    IMAGE
-    AUDIO
-    VIDEO
-    FILE
 
   EnumApiAction:
     NONE
     ERROR
     PROGRESS
     PROGRESS_UPLOAD
     PROGRESS_DOWNLOAD
     PARTIAL
     COMPLETE
 
   EnumApiVisibility:
     PUBLIC
     PRIVATE
+    LOCAL
 
   EnumApiCrypto:
+    NONE
     ECC
     PQ
 
 entity:
   ERequest:
+    _DESCRIPTION_: "ERequest DESCRIPTION"
     enumApiCrypto: ENUM EnumApiCrypto .ECC
     pk: BYTES
     cipher: BYTES
     sign: BYTES
     hash: BYTES
     chunk: INT
     chunkTotal: INT
-    length: INT
     data: BYTES
 
   EResponse:
+    _DESCRIPTION_: "EResponse DESCRIPTION"
     sign: BYTES
     hash: BYTES
     chunk: INT
     chunkTotal: INT
-    length: INT
     data: BYTES
     isError: BOOL
     error: STRING
 
   EApi: 
-    _DESCRIPTION_: "this is EAPI DESCRIPTION"
+    _DESCRIPTION_: "EApi DESCRIPTION"
     description: STRING
     isStream: BOOL     
     input: STRING
     output: STRING
 
   EAction:
-    _DESCRIPTION_: "this is EAction DESCRIPTION"
+    _DESCRIPTION_: "EAction DESCRIPTION"
     enumApiAction: ENUM EnumApiAction .NONE
     action: STRING     
     input: BYTES 
     output: BYTES
 
   EApiConfig:
-      _DESCRIPTION_: "this is EAction DESCRIPTION"
+      _DESCRIPTION_: "EApiConfig DESCRIPTION"
       enumApiVisibility: ENUM EnumApiVisibility .PRIVATE
       publicKey: BYTES
       label: STRING
       description: STRING
       urlLogo: STRING
       remoteUrl: STRING 
       remotePort: INT 443
       os: STRING
       mapEApi: MAP EApi
 
   EApiFile:
-    _DESCRIPTION_: "this is EApiFile DESCRIPTION"
-    isUrl: BOOL
-    name : STRING
-    ext: STRING
-    length : INT
-    data: BYTES
-
-  EApiImage:
-    _DESCRIPTION_: "this is EAPiImagection DESCRIPTION"
-    isUrl: BOOL
-    name : STRING
-    ext: STRING
-    length : INT
-    data: BYTES
-
-  EApiVideo:
-    _DESCRIPTION_: "this is EApiVideo DESCRIPTION"
+    _DESCRIPTION_: "EApiFile DESCRIPTION"
     isUrl: BOOL
     name : STRING
     ext: STRING
-    length : INT
+    hash: BYTES
     data: BYTES
-
-  EApiAudio:
-    _DESCRIPTION_: "this is EAPIAudio DESCRIPTION"
-    isUrl: BOOL
-    name : STRING
-    ext: STRING
-    length : INT
-    data: BYTES
+  
+  EApiText:
+    _DESCRIPTION_: "EApiFile DESCRIPTION"
+    language: LANGUAGE "en-US"
+    text : STRING
+    isComplete: BOOL
```

### Comparing `evo_framework-2024.5.40/evo_framework/core/evo_core_api/control/CApi.py` & `evo_framework-2024.5.41/evo_framework/core/evo_core_api/control/CApi.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.40/evo_framework/core/evo_core_api/control/CApiFlow.py` & `evo_framework-2024.5.41/evo_framework/core/evo_core_api/control/CApiFlow.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.40/evo_framework/core/evo_core_api/entity/EAction.py` & `evo_framework-2024.5.41/evo_framework/core/evo_core_api/entity/EAction.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 #========================================================================================================================================
 # CyborgAI CC BY-NC-ND 4.0 Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 Internation	https://github.com/cyborg-ai-git # 
 #========================================================================================================================================
 
 from evo_framework.entity.EObject import EObject
 from evo_framework.core.evo_core_type.entity.EvoMap import EvoMap
-from evo_framework.core.evo_core_api.entity.EnumApiAction import EnumApiAction
+
+from evo_core_api.entity.EnumApiAction import EnumApiAction
 #========================================================================================================================================
 """EAction
 
-	this is EAction DESCRIPTION
+	EAction DESCRIPTION
 	
 """
 class EAction(EObject):
 
-	VERSION:str="2fb34e332b25762d5c8b1a9c054b537e46aa53785799f595a4c1c0a0d5d769fb"
+	VERSION:str="6774ada8be5c1a37bcd9bfd6c0f19a34467e169d0f9d6397f4714f0245f35b58"
 
 	def __init__(self):
 		super().__init__()
 		self.enumApiAction:EnumApiAction = EnumApiAction.NONE
 		self.action:str = None
 		self.input:bytes = None
 		self.output:bytes = None
@@ -26,30 +27,29 @@
 		super().toStream(stream)
 		self._doWriteInt(self.enumApiAction.value, stream)
 		self._doWriteStr(self.action, stream)
 		self._doWriteBytes(self.input, stream)
 		self._doWriteBytes(self.output, stream)
 		
 	def fromStream(self, stream):
-		super().fromStream(stream)	
+		super().fromStream(stream)
 		self.enumApiAction = EnumApiAction(self._doReadInt(stream))
 		self.action = self._doReadStr(stream)
 		self.input = self._doReadBytes(stream)
 		self.output = self._doReadBytes(stream)
 	
 	def __str__(self) -> str:
 		strReturn = "\n".join([
 				super().__str__(),			
-				f"\tenumApiAction:{ self.enumApiAction  }",
-				f"\taction:{ self.action  }",
-				f"\tinput len: {len(self.input) if self.input else 'None'}",
-            	f"\toutput len: {len(self.output) if self.output else 'None'}"
+				f"\tenumApiAction:{self.enumApiAction}",
+				f"\taction:{self.action}",
+				f"input length:{len(self.input) if self.input else 'None'}",
+				f"output length:{len(self.output) if self.output else 'None'}",
 							]) 
 		return strReturn
-	
 #----------------------------------------------------------------------------------------------------------------------------------------
 #EXTENSION
 #----------------------------------------------------------------------------------------------------------------------------------------
 	async def doSetInput(self, eObject:EObject):
 		from evo_framework.core.evo_core_api.utility.IuApi import IuApi
 		self.input = eObject.toBytes()
 #----------------------------------------------------------------------------------------------------------------------------------------
```

### Comparing `evo_framework-2024.5.40/evo_framework/core/evo_core_api/entity/EActionTask.py` & `evo_framework-2024.5.41/evo_framework/core/evo_core_api/entity/EActionTask.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.40/evo_framework/core/evo_core_api/entity/EApi.py` & `evo_framework-2024.5.41/evo_framework/core/evo_core_api/entity/EApi.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.40/evo_framework/core/evo_core_api/entity/EApiAudio.py` & `evo_framework-2024.5.41/evo_framework/core/evo_core_api/entity/EResponse.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,55 +2,58 @@
 # CyborgAI CC BY-NC-ND 4.0 Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 Internation	https://github.com/cyborg-ai-git # 
 #========================================================================================================================================
 
 from evo_framework.entity.EObject import EObject
 from evo_framework.core.evo_core_type.entity.EvoMap import EvoMap
 
 #========================================================================================================================================
-"""EApiAudio
+"""EResponse
 
-	this is EAPIAudio DESCRIPTION
+	EResponse DESCRIPTION
 	
 """
-class EApiAudio(EObject):
+class EResponse(EObject):
 
-	VERSION:str="3c37d0d7315664187980d10bc9abe5541b93f38ef107473e66bc336fac026f55"
+	VERSION:str="3dd3040068f3ba355af96cf55e3aa7024246c88036eb50ca2d5dad4b91ab6c2a"
 
 	def __init__(self):
 		super().__init__()
-		
-		self.isUrl:bool = None
-		self.name:str = None
-		self.ext:str = None
-		self.length:int = None
+		self.sign:bytes = None
+		self.hash:bytes = None
+		self.chunk:int = None
+		self.chunkTotal:int = None
 		self.data:bytes = None
+		self.isError:bool = None
+		self.error:str = None
   
 	def toStream(self, stream):
 		super().toStream(stream)
-		
-		self._doWriteBool(self.isUrl, stream)
-		self._doWriteStr(self.name, stream)
-		self._doWriteStr(self.ext, stream)
-		self._doWriteInt(self.length, stream)
+		self._doWriteBytes(self.sign, stream)
+		self._doWriteBytes(self.hash, stream)
+		self._doWriteInt(self.chunk, stream)
+		self._doWriteInt(self.chunkTotal, stream)
 		self._doWriteBytes(self.data, stream)
+		self._doWriteBool(self.isError, stream)
+		self._doWriteStr(self.error, stream)
 		
 	def fromStream(self, stream):
 		super().fromStream(stream)
-		
-		self.isUrl = self._doReadBool(stream)
-		self.name = self._doReadStr(stream)
-		self.ext = self._doReadStr(stream)
-		self.length = self._doReadInt(stream)
+		self.sign = self._doReadBytes(stream)
+		self.hash = self._doReadBytes(stream)
+		self.chunk = self._doReadInt(stream)
+		self.chunkTotal = self._doReadInt(stream)
 		self.data = self._doReadBytes(stream)
+		self.isError = self._doReadBool(stream)
+		self.error = self._doReadStr(stream)
 	
 	def __str__(self) -> str:
 		strReturn = "\n".join([
-				super().__str__(),
-							
-				f"\tisUrl:{ self.isUrl  }",
-				f"\tname:{ self.name  }",
-				f"\text:{ self.ext  }",
-				f"\tlength:{ self.length  }",
-				#f"\tdata:{ self.data  }",
+				super().__str__(),			
+				f"sign length:{len(self.sign) if self.sign else 'None'}",
+				f"hash length:{len(self.hash) if self.hash else 'None'}",
+				f"\tchunk:{self.chunk}",
+				f"\tchunkTotal:{self.chunkTotal}",
+				f"data length:{len(self.data) if self.data else 'None'}",
+				f"\tisError:{self.isError}",
+				f"\terror:{self.error}",
 							]) 
-		return strReturn
-	
+		return strReturn
```

### Comparing `evo_framework-2024.5.40/evo_framework/core/evo_core_api/entity/EApiConfig.py` & `evo_framework-2024.5.41/evo_framework/core/evo_core_api/entity/EApiConfig.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 """
 class EApiConfig(EObject):
 
 	VERSION:str="522375abdb36150eb2abfdc838fe48145d8442932f2034b2cba34f38d20e014f"
 
 	def __init__(self):
 		super().__init__()
-		
 		self.enumApiVisibility:EnumApiVisibility = EnumApiVisibility.PRIVATE
 		self.publicKey:bytes = None
 		self.label:str = None
 		self.description:str = None
 		self.urlLogo:str = None
 		self.remoteUrl:str = None
 		self.remotePort:int = 443
@@ -43,48 +42,44 @@
 		self.secretKey:bytes = None
 		self.isFirstStart:bool = True
 		self.localAddress:str = "0.0.0.0"
 		self.localPort:int = 8001
 		self.enumApiTunnel:EnumApiTunnel = EnumApiTunnel.LOCAL
   
 	def toStream(self, stream):
-		super().toStream(stream)
-		
+		super().toStream(stream)	
 		self._doWriteInt(self.enumApiVisibility.value, stream)
 		self._doWriteBytes(self.publicKey, stream)
 		self._doWriteStr(self.label, stream)
 		self._doWriteStr(self.description, stream)
 		self._doWriteStr(self.urlLogo, stream)
 		self._doWriteStr(self.remoteUrl, stream)
 		self._doWriteInt(self.remotePort, stream)
 		self._doWriteStr(self.os, stream)
 		self._doWriteMap(self.mapEApi, stream)
 		
 	def fromStream(self, stream):
 		super().fromStream(stream)
-		
 		self.enumApiVisibility = EnumApiVisibility(self._doReadInt(stream))
 		self.publicKey = self._doReadBytes(stream)
 		self.label = self._doReadStr(stream)
 		self.description = self._doReadStr(stream)
 		self.urlLogo = self._doReadStr(stream)
 		self.remoteUrl = self._doReadStr(stream)
 		self.remotePort = self._doReadInt(stream)
 		self.os = self._doReadStr(stream)
 		self.mapEApi = self._doReadMap(EApi, stream)
 	
 	def __str__(self) -> str:
 		strReturn = "\n".join([
-				super().__str__(),
-							
+				super().__str__(),					
 				f"\tenumApiVisibility:{ self.enumApiVisibility  }",
 				f"\tpublicKey:{ self.publicKey!r}",
-				f"\tlabel:{ self.label  }",
-				f"\tdescription:{ self.description  }",
-				f"\turlLogo:{ self.urlLogo  }",
-				f"\tremoteUrl:{ self.remoteUrl  }",
-				f"\tremotePort:{ self.remotePort  }",
-				f"\tos:{ self.os  }",
-				f"\tmapEApi:{ self.mapEApi  }",
-							]) 
-		return strReturn
-	
+				f"\tlabel:{self.label}",
+				f"\tdescription:{self.description}",
+				f"\turlLogo:{self.urlLogo}",
+				f"\tremoteUrl:{self.remoteUrl}",
+				f"\tremotePort:{self.remotePort}",
+				f"\tos:{self.os}",
+				f"\tmapEApi:{self.mapEApi}",					
+    	]) 
+		return strReturn
```

### Comparing `evo_framework-2024.5.40/evo_framework/core/evo_core_api/entity/EApiFile.py` & `evo_framework-2024.5.41/evo_framework/core/evo_core_api/entity/EApiFile.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,66 +1,63 @@
 #========================================================================================================================================
 # CyborgAI CC BY-NC-ND 4.0 Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 Internation	https://github.com/cyborg-ai-git # 
 #========================================================================================================================================
 
 from evo_framework.entity.EObject import EObject
 from evo_framework.core.evo_core_type.entity.EvoMap import EvoMap
+
 #========================================================================================================================================
 """EApiFile
 
-	this is EApiFile DESCRIPTION
+	EApiFile DESCRIPTION
 	
 """
 class EApiFile(EObject):
 
-	VERSION:str="3c37d0d7315664187980d10bc9abe5541b93f38ef107473e66bc336fac026f55"
+	VERSION:str="c1cfb486a24b16fcdb499ce8c187f5f16c09b2178a6e42450e3da68a933e7b3f"
 
 	def __init__(self):
 		super().__init__()
-		
 		self.isUrl:bool = None
 		self.name:str = None
 		self.ext:str = None
-		self.length:int = None
+		self.hash:bytes = None
 		self.data:bytes = None
   
 	def toStream(self, stream):
 		super().toStream(stream)
-		
 		self._doWriteBool(self.isUrl, stream)
 		self._doWriteStr(self.name, stream)
 		self._doWriteStr(self.ext, stream)
-		self._doWriteInt(self.length, stream)
+		self._doWriteBytes(self.hash, stream)
 		self._doWriteBytes(self.data, stream)
 		
 	def fromStream(self, stream):
 		super().fromStream(stream)
-		
 		self.isUrl = self._doReadBool(stream)
 		self.name = self._doReadStr(stream)
 		self.ext = self._doReadStr(stream)
-		self.length = self._doReadInt(stream)
+		self.hash = self._doReadBytes(stream)
 		self.data = self._doReadBytes(stream)
 	
 	def __str__(self) -> str:
 		strReturn = "\n".join([
-				super().__str__(),
-							
+				super().__str__(),			
 				f"\tisUrl:{self.isUrl}",
-				f"\tname:{ self.name  }",
-				f"\text:{ self.ext  }",
-				f"\tlength:{ self.length  }",
-				f"\tdata len: {len(self.data) if self.data else 'None'}"
+				f"\tname:{self.name}",
+				f"\text:{self.ext}",
+				f"hash length:{len(self.hash) if self.hash else 'None'}",
+				f"data length:{len(self.data) if self.data else 'None'}",
 							]) 
 		return strReturn
 
 #----------------------------------------------------------------------------------------------------------------------------------------
 #EXTENSION
 #----------------------------------------------------------------------------------------------------------------------------------------
 	async def toFile(self) -> str:
 		from evo_framework.core.evo_core_api.utility.IuApi import IuApi
 		return await IuApi.toFile(self.data, self.ext)	 
 #----------------------------------------------------------------------------------------------------------------------------------------
 	async def fromFile(self, pathFile:str):
 		from evo_framework.core.evo_core_api.utility.IuApi import IuApi
-		self.data = await IuApi.fromFile(pathFile)	 
+		self.data, self.ext = await IuApi.fromFile(pathFile)	 
 #----------------------------------------------------------------------------------------------------------------------------------------
```

### Comparing `evo_framework-2024.5.40/evo_framework/core/evo_core_api/entity/EApiImage.py` & `evo_framework-2024.5.41/evo_framework/core/evo_core_api/entity/EApiText.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,55 +2,43 @@
 # CyborgAI CC BY-NC-ND 4.0 Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 Internation	https://github.com/cyborg-ai-git # 
 #========================================================================================================================================
 
 from evo_framework.entity.EObject import EObject
 from evo_framework.core.evo_core_type.entity.EvoMap import EvoMap
 
 #========================================================================================================================================
-"""EApiImage
+"""EApiText
 
-	this is EAPiImagection DESCRIPTION
+	EApiFile DESCRIPTION
 	
 """
-class EApiImage(EObject):
+class EApiText(EObject):
 
-	VERSION:str="3c37d0d7315664187980d10bc9abe5541b93f38ef107473e66bc336fac026f55"
+	VERSION:str="4672b9fb466a618ab6adfeb34e328702670ec6af44d6d64619bb99b3d132fcfe"
 
 	def __init__(self):
 		super().__init__()
-		
-		self.isUrl:bool = None
-		self.name:str = None
-		self.ext:str = None
-		self.length:int = None
-		self.data:bytes = None
+		self.language:str = "en-US"
+		self.text:str = None
+		self.isComplete:bool = None
   
 	def toStream(self, stream):
 		super().toStream(stream)
-		
-		self._doWriteBool(self.isUrl, stream)
-		self._doWriteStr(self.name, stream)
-		self._doWriteStr(self.ext, stream)
-		self._doWriteInt(self.length, stream)
-		self._doWriteBytes(self.data, stream)
+		self._doWriteStr(self.language, stream)
+		self._doWriteStr(self.text, stream)
+		self._doWriteBool(self.isComplete, stream)
 		
 	def fromStream(self, stream):
 		super().fromStream(stream)
-		
-		self.isUrl = self._doReadBool(stream)
-		self.name = self._doReadStr(stream)
-		self.ext = self._doReadStr(stream)
-		self.length = self._doReadInt(stream)
-		self.data = self._doReadBytes(stream)
+		self.language = self._doReadStr(stream)
+		self.text = self._doReadStr(stream)
+		self.isComplete = self._doReadBool(stream)
 	
 	def __str__(self) -> str:
 		strReturn = "\n".join([
-				super().__str__(),
-							
-				f"\tisUrl:{ self.isUrl  }",
-				f"\tname:{ self.name  }",
-				f"\text:{ self.ext  }",
-				f"\tlength:{ self.length  }",
-				f"\tdata len: {len(self.data) if self.data else 'None'}"
+				super().__str__(),			
+				f"\tlanguage:{self.language}",
+				f"\ttext:{self.text}",
+				f"\tisComplete:{self.isComplete}",
 							]) 
 		return strReturn
```

### Comparing `evo_framework-2024.5.40/evo_framework/core/evo_core_api/entity/EApiVideo.py` & `evo_framework-2024.5.41/evo_framework/core/evo_core_api/entity/ERequest.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,52 +1,65 @@
 #========================================================================================================================================
 # CyborgAI CC BY-NC-ND 4.0 Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 Internation	https://github.com/cyborg-ai-git # 
 #========================================================================================================================================
 
 from evo_framework.entity.EObject import EObject
 from evo_framework.core.evo_core_type.entity.EvoMap import EvoMap
 
+from evo_core_api.entity.EnumApiCrypto import EnumApiCrypto
 #========================================================================================================================================
-"""EApiVideo
+"""ERequest
 
-	this is EApiVideo DESCRIPTION
+	ERequest DESCRIPTION
 	
 """
-class EApiVideo(EObject):
+class ERequest(EObject):
 
-	VERSION:str="3c37d0d7315664187980d10bc9abe5541b93f38ef107473e66bc336fac026f55"
+	VERSION:str="2aafac6a76b23b255eed9371f540c0d5b0f1fc5bf47cbd6c4fcba659dee2f7b6"
 
 	def __init__(self):
 		super().__init__()
-		self.isUrl:bool = None
-		self.name:str = None
-		self.ext:str = None
-		self.length:int = None
+		self.enumApiCrypto:EnumApiCrypto = EnumApiCrypto.ECC
+		self.pk:bytes = None
+		self.cipher:bytes = None
+		self.sign:bytes = None
+		self.hash:bytes = None
+		self.chunk:int = None
+		self.chunkTotal:int = None
 		self.data:bytes = None
   
 	def toStream(self, stream):
 		super().toStream(stream)
-		self._doWriteBool(self.isUrl, stream)
-		self._doWriteStr(self.name, stream)
-		self._doWriteStr(self.ext, stream)
-		self._doWriteInt(self.length, stream)
+		self._doWriteInt(self.enumApiCrypto.value, stream)
+		self._doWriteBytes(self.pk, stream)
+		self._doWriteBytes(self.cipher, stream)
+		self._doWriteBytes(self.sign, stream)
+		self._doWriteBytes(self.hash, stream)
+		self._doWriteInt(self.chunk, stream)
+		self._doWriteInt(self.chunkTotal, stream)
 		self._doWriteBytes(self.data, stream)
 		
 	def fromStream(self, stream):
-		super().fromStream(stream)
-		self.isUrl = self._doReadBool(stream)
-		self.name = self._doReadStr(stream)
-		self.ext = self._doReadStr(stream)
-		self.length = self._doReadInt(stream)
+		super().fromStream(stream)	
+		self.enumApiCrypto = EnumApiCrypto(self._doReadInt(stream))
+		self.pk = self._doReadBytes(stream)
+		self.cipher = self._doReadBytes(stream)
+		self.sign = self._doReadBytes(stream)
+		self.hash = self._doReadBytes(stream)
+		self.chunk = self._doReadInt(stream)
+		self.chunkTotal = self._doReadInt(stream)
 		self.data = self._doReadBytes(stream)
 	
 	def __str__(self) -> str:
 		strReturn = "\n".join([
-				super().__str__(),
-							
-				f"\tisUrl:{ self.isUrl  }",
-				f"\tname:{ self.name  }",
-				f"\text:{ self.ext  }",
-				f"\tlength:{ self.length  }",
-				f"\tdata len: {len(self.data) if self.data else 'None'}"
+				super().__str__(),					
+				f"\tenumApiCrypto:{self.enumApiCrypto}",
+				f"pk length:{len(self.pk) if self.pk else 'None'}",
+				f"cipher length:{len(self.cipher) if self.cipher else 'None'}",
+				f"sign length:{len(self.sign) if self.sign else 'None'}",
+				f"hash length:{len(self.hash) if self.hash else 'None'}",
+				f"\tchunk:{self.chunk}",
+				f"\tchunkTotal:{self.chunkTotal}",
+				f"data length:{len(self.data) if self.data else 'None'}",
 							]) 
-		return strReturn
+		return strReturn
+
```

### Comparing `evo_framework-2024.5.40/evo_framework/core/evo_core_api/entity/EnumApiAction.py` & `evo_framework-2024.5.41/evo_framework/core/evo_core_api/entity/EnumApiAction.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.40/evo_framework/core/evo_core_api/entity/__init__.py` & `evo_framework-2024.5.41/evo_framework/core/evo_core_api/entity/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,10 +17,11 @@
 from evo_framework.core.evo_core_api.entity.EActionTask import EActionTask
 
 from evo_framework.core.evo_core_api.entity.EAction import EAction
 
 from evo_framework.core.evo_core_api.entity.EApi import EApi
 
 from evo_framework.core.evo_core_api.entity.EApiFile import EApiFile
-from evo_framework.core.evo_core_api.entity.EApiImage import EApiImage
-from evo_framework.core.evo_core_api.entity.EApiVideo import EApiVideo
-from evo_framework.core.evo_core_api.entity.EApiAudio import EApiAudio
+from evo_framework.core.evo_core_api.entity.EApiText import EApiText
+#from evo_framework.core.evo_core_api.entity.EApiImage import EApiImage
+#from evo_framework.core.evo_core_api.entity.EApiVideo import EApiVideo
+#from evo_framework.core.evo_core_api.entity.EApiAudio import EApiAudio
```

### Comparing `evo_framework-2024.5.40/evo_framework/core/evo_core_api/utility/IuApiPb.py` & `evo_framework-2024.5.41/evo_framework/core/evo_core_api/utility/IuApiPb.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.40/evo_framework/core/evo_core_binary/utility/IuBinary.py` & `evo_framework-2024.5.41/evo_framework/core/evo_core_binary/utility/IuBinary.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.40/evo_framework/core/evo_core_binary/utility/IuBinaryAsync.py` & `evo_framework-2024.5.41/evo_framework/core/evo_core_binary/utility/IuBinaryAsync.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.40/evo_framework/core/evo_core_binary/utility/UBinary.py` & `evo_framework-2024.5.41/evo_framework/core/evo_core_binary/utility/UBinary.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.40/evo_framework/core/evo_core_boot/control/CBoot.py` & `evo_framework-2024.5.41/evo_framework/core/evo_core_boot/control/CBoot.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.40/evo_framework/core/evo_core_convert/test_evo_core_binary.py` & `evo_framework-2024.5.41/evo_framework/core/evo_core_convert/test_evo_core_binary.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.40/evo_framework/core/evo_core_convert/utility/IuConvert.py` & `evo_framework-2024.5.41/evo_framework/core/evo_core_convert/utility/IuConvert.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.40/evo_framework/core/evo_core_crypto/utility/IuCryptChacha.py` & `evo_framework-2024.5.41/evo_framework/core/evo_core_crypto/utility/IuCryptChacha.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.40/evo_framework/core/evo_core_crypto/utility/IuCryptEC.py` & `evo_framework-2024.5.41/evo_framework/core/evo_core_crypto/utility/IuCryptEC.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.40/evo_framework/core/evo_core_crypto/utility/IuCryptHash.py` & `evo_framework-2024.5.41/evo_framework/core/evo_core_crypto/utility/IuCryptHash.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.40/evo_framework/core/evo_core_file/entity/EFileChunk.py` & `evo_framework-2024.5.41/evo_framework/core/evo_core_file/entity/EFileChunk.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.40/evo_framework/core/evo_core_foundation/IFoundation.py` & `evo_framework-2024.5.41/evo_framework/core/evo_core_foundation/IFoundation.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.40/evo_framework/core/evo_core_key/utility/IuKey.py` & `evo_framework-2024.5.41/evo_framework/core/evo_core_key/utility/IuKey.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.40/evo_framework/core/evo_core_log/utility/IuLog.py` & `evo_framework-2024.5.41/evo_framework/core/evo_core_log/utility/IuLog.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.40/evo_framework/core/evo_core_log/utility/ULogger.py` & `evo_framework-2024.5.41/evo_framework/core/evo_core_log/utility/ULogger.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.40/evo_framework/core/evo_core_setting/control/CSetting.py` & `evo_framework-2024.5.41/evo_framework/core/evo_core_setting/control/CSetting.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.40/evo_framework/core/evo_core_setting/entity/ESetting.py` & `evo_framework-2024.5.41/evo_framework/core/evo_core_setting/entity/ESetting.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.40/evo_framework/core/evo_core_system/utility/IuSystem.py` & `evo_framework-2024.5.41/evo_framework/core/evo_core_system/utility/IuSystem.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.40/evo_framework/core/evo_core_type/entity/EvoMap.py` & `evo_framework-2024.5.41/evo_framework/core/evo_core_type/entity/EvoMap.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.40/evo_framework/entity/EObject.py` & `evo_framework-2024.5.41/evo_framework/entity/EObject.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.40/pyproject.toml` & `evo_framework-2024.5.41/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "evo-framework"
-version = "2024.5.40"
+version = "2024.5.41"
 description = "evo framework python"
 authors = ["cyborg-ai-git <129898917+cyborg-ai-git@users.noreply.github.com>"]
 readme = "README.md"
 #packages = [{include = "evo"}]
 license = "CC BY-NC-ND 4.0"
 include = ["LICENSE.txt"]
 
@@ -13,11 +13,12 @@
 PyYAML = "^6.0.1"
 lz4 = "^4.3.2"
 ecdsa = "^0.18.0"
 cryptography = "^41.0.7"
 aiofiles= "^23.2.1"
 typing-extensions = "^4.12.0"
 Pillow = "^10.3.0"
+python-magic  = "^0.4.27"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `evo_framework-2024.5.40/PKG-INFO` & `evo_framework-2024.5.41/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evo-framework
-Version: 2024.5.40
+Version: 2024.5.41
 Summary: evo framework python
 License: CC BY-NC-ND 4.0
 Author: cyborg-ai-git
 Author-email: 129898917+cyborg-ai-git@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: Pillow (>=10.3.0,<11.0.0)
 Requires-Dist: PyYAML (>=6.0.1,<7.0.0)
 Requires-Dist: aiofiles (>=23.2.1,<24.0.0)
 Requires-Dist: cryptography (>=41.0.7,<42.0.0)
 Requires-Dist: ecdsa (>=0.18.0,<0.19.0)
 Requires-Dist: lz4 (>=4.3.2,<5.0.0)
+Requires-Dist: python-magic (>=0.4.27,<0.5.0)
 Requires-Dist: typing-extensions (>=4.12.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 #========================================================================================================================================
 CC BY-NC-ND 4.0 Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International       https://github.com/cyborg-ai-git
 #========================================================================================================================================
```

