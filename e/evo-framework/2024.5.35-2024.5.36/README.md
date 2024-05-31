# Comparing `tmp/evo_framework-2024.5.35.tar.gz` & `tmp/evo_framework-2024.5.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evo_framework-2024.5.35.tar", max compression
+gzip compressed data, was "evo_framework-2024.5.36.tar", max compression
```

## Comparing `evo_framework-2024.5.35.tar` & `evo_framework-2024.5.36.tar`

### file list

```diff
@@ -1,75 +1,75 @@
--rw-r--r--   0        0        0    13525 2024-05-28 16:27:09.302451 evo_framework-2024.5.35/LICENSE.txt
--rw-r--r--   0        0        0      406 2024-05-28 16:35:10.344754 evo_framework-2024.5.35/README.md
--rwxr-xr-x   0        0        0      770 2024-05-29 23:15:57.646008 evo_framework-2024.5.35/evo_framework/__init__.py
--rwxr-xr-x   0        0        0     4030 2024-04-14 21:01:20.000000 evo_framework-2024.5.35/evo_framework/control/CObject.py
--rwxr-xr-x   0        0        0       51 2024-05-29 23:15:57.849272 evo_framework-2024.5.35/evo_framework/control/__init__.py
--rw-r--r--   0        0        0      399 2024-05-28 10:42:13.864068 evo_framework-2024.5.35/evo_framework/core/__init__.py
--rwxr-xr-x   0        0        0      160 2024-05-29 23:15:57.645990 evo_framework-2024.5.35/evo_framework/core/evo_core_api/__init__.py
--rw-r--r--   0        0        0     2657 2024-05-30 15:49:25.644184 evo_framework-2024.5.35/evo_framework/core/evo_core_api/automation/entity.yaml
--rw-r--r--   0        0        0     6058 2024-05-29 23:52:16.739992 evo_framework-2024.5.35/evo_framework/core/evo_core_api/control/CApi.py
--rw-r--r--   0        0        0    25474 2024-05-30 16:43:34.565564 evo_framework-2024.5.35/evo_framework/core/evo_core_api/control/CApiFlow.py
--rw-r--r--   0        0        0      131 2024-05-29 23:15:57.840551 evo_framework-2024.5.35/evo_framework/core/evo_core_api/control/__init__.py
--rw-r--r--   0        0        0     1893 2024-05-29 23:27:02.246146 evo_framework-2024.5.35/evo_framework/core/evo_core_api/entity/EAction.py
--rw-r--r--   0        0        0     1306 2024-05-29 23:15:57.646050 evo_framework-2024.5.35/evo_framework/core/evo_core_api/entity/EActionTask.py
--rw-r--r--   0        0        0     1770 2024-05-29 23:38:23.561186 evo_framework-2024.5.35/evo_framework/core/evo_core_api/entity/EApi.py
--rw-r--r--   0        0        0     1781 2024-05-29 23:42:56.957602 evo_framework-2024.5.35/evo_framework/core/evo_core_api/entity/EApiAudio.py
--rw-r--r--   0        0        0     3060 2024-05-29 23:29:47.211002 evo_framework-2024.5.35/evo_framework/core/evo_core_api/entity/EApiConfig.py
--rw-r--r--   0        0        0     1778 2024-05-29 23:43:06.604309 evo_framework-2024.5.35/evo_framework/core/evo_core_api/entity/EApiFile.py
--rw-r--r--   0        0        0     1786 2024-05-29 23:43:12.828390 evo_framework-2024.5.35/evo_framework/core/evo_core_api/entity/EApiImage.py
--rw-r--r--   0        0        0     1770 2024-05-29 23:45:08.289661 evo_framework-2024.5.35/evo_framework/core/evo_core_api/entity/EApiVideo.py
--rwxr-xr-x   0        0        0     2497 2024-05-30 16:41:08.607585 evo_framework-2024.5.35/evo_framework/core/evo_core_api/entity/ERequest.py
--rwxr-xr-x   0        0        0     2210 2024-05-30 16:42:44.419615 evo_framework-2024.5.35/evo_framework/core/evo_core_api/entity/EResponse.py
--rw-r--r--   0        0        0      568 2024-05-29 23:04:53.300310 evo_framework-2024.5.35/evo_framework/core/evo_core_api/entity/EnumApiAction.py
--rw-r--r--   0        0        0      101 2024-03-22 09:24:36.000000 evo_framework-2024.5.35/evo_framework/core/evo_core_api/entity/EnumApiCompress.py
--rw-r--r--   0        0        0       97 2024-03-22 09:18:53.000000 evo_framework-2024.5.35/evo_framework/core/evo_core_api/entity/EnumApiCrypto.py
--rw-r--r--   0        0        0      274 2024-05-28 15:31:41.321728 evo_framework-2024.5.35/evo_framework/core/evo_core_api/entity/EnumApiType.py
--rw-r--r--   0        0        0      493 2024-05-29 23:04:53.308461 evo_framework-2024.5.35/evo_framework/core/evo_core_api/entity/EnumApiVisibility.py
--rw-r--r--   0        0        0        0 2024-05-27 12:52:18.397976 evo_framework-2024.5.35/evo_framework/core/evo_core_api/entity/EnumLanguage.py
--rwxr-xr-x   0        0        0     1502 2024-05-29 23:16:21.970731 evo_framework-2024.5.35/evo_framework/core/evo_core_api/entity/__init__.py
--rwxr-xr-x   0        0        0    11410 2024-05-29 23:15:57.840538 evo_framework-2024.5.35/evo_framework/core/evo_core_api/utility/IuApi.py
--rw-r--r--   0        0        0    14944 2024-05-29 23:15:57.840524 evo_framework-2024.5.35/evo_framework/core/evo_core_api/utility/IuApiPb.py
--rwxr-xr-x   0        0        0       64 2024-05-29 23:15:57.840493 evo_framework-2024.5.35/evo_framework/core/evo_core_api/utility/__init__.py
--rwxr-xr-x   0        0        0      215 2024-05-29 23:15:57.848203 evo_framework-2024.5.35/evo_framework/core/evo_core_binary/__init__.py
--rwxr-xr-x   0        0        0      120 2021-11-24 10:46:35.000000 evo_framework-2024.5.35/evo_framework/core/evo_core_binary/entity/IBinary.py
--rwxr-xr-x   0        0        0     9089 2024-05-29 23:15:57.849286 evo_framework-2024.5.35/evo_framework/core/evo_core_binary/utility/IuBinary.py
--rw-r--r--   0        0        0     6658 2024-05-29 23:15:57.848274 evo_framework-2024.5.35/evo_framework/core/evo_core_binary/utility/IuBinaryAsync.py
--rw-r--r--   0        0        0     7700 2024-05-29 23:15:57.848234 evo_framework-2024.5.35/evo_framework/core/evo_core_binary/utility/UBinary.py
--rw-r--r--   0        0        0     1324 2024-05-29 23:15:57.844638 evo_framework-2024.5.35/evo_framework/core/evo_core_boot/control/CBoot.py
--rw-r--r--   0        0        0      281 2024-04-15 19:43:35.988232 evo_framework-2024.5.35/evo_framework/core/evo_core_bridge/IBridge.py
--rw-r--r--   0        0        0       75 2024-05-29 23:15:57.848167 evo_framework-2024.5.35/evo_framework/core/evo_core_convert/__init__.py
--rw-r--r--   0        0        0     6213 2024-05-29 23:54:10.283288 evo_framework-2024.5.35/evo_framework/core/evo_core_convert/test_evo_core_binary.py
--rw-r--r--   0        0        0      841 2024-04-12 09:23:48.000000 evo_framework-2024.5.35/evo_framework/core/evo_core_convert/utility/IuConvert.py
--rw-r--r--   0        0        0        0 2021-11-12 08:43:14.000000 evo_framework-2024.5.35/evo_framework/core/evo_core_convert/utility/__init__.py
--rw-r--r--   0        0        0      236 2024-05-29 23:15:57.848112 evo_framework-2024.5.35/evo_framework/core/evo_core_crypto/__init__.py
--rw-r--r--   0        0        0     1470 2024-03-26 15:03:45.000000 evo_framework-2024.5.35/evo_framework/core/evo_core_crypto/utility/IuCryptChacha.py
--rwxr-xr-x   0        0        0     1467 2024-05-29 23:15:57.848244 evo_framework-2024.5.35/evo_framework/core/evo_core_crypto/utility/IuCryptEC.py
--rwxr-xr-x   0        0        0      743 2024-03-17 11:26:36.000000 evo_framework-2024.5.35/evo_framework/core/evo_core_crypto/utility/IuCryptHash.py
--rw-r--r--   0        0        0     1332 2024-05-29 23:15:57.848017 evo_framework-2024.5.35/evo_framework/core/evo_core_file/entity/EFileChunk.py
--rw-r--r--   0        0        0      699 2024-05-29 23:15:57.848149 evo_framework-2024.5.35/evo_framework/core/evo_core_foundation/IFoundation.py
--rw-r--r--   0        0        0       63 2024-05-29 23:15:57.849413 evo_framework-2024.5.35/evo_framework/core/evo_core_key/__init__.py
--rw-r--r--   0        0        0      893 2024-05-29 23:15:57.844661 evo_framework-2024.5.35/evo_framework/core/evo_core_key/utility/IuKey.py
--rw-r--r--   0        0        0       63 2024-05-29 23:15:57.848179 evo_framework-2024.5.35/evo_framework/core/evo_core_log/__init__.py
--rw-r--r--   0        0        0     2150 2024-05-29 23:15:57.848192 evo_framework-2024.5.35/evo_framework/core/evo_core_log/utility/IuLog.py
--rw-r--r--   0        0        0     2289 2024-03-22 09:09:45.000000 evo_framework-2024.5.35/evo_framework/core/evo_core_log/utility/ULogger.py
--rwxr-xr-x   0        0        0      146 2024-05-29 23:15:57.848259 evo_framework-2024.5.35/evo_framework/core/evo_core_setting/__init__.py
--rw-r--r--   0        0        0     2813 2024-05-29 23:15:57.849237 evo_framework-2024.5.35/evo_framework/core/evo_core_setting/control/CSetting.py
--rwxr-xr-x   0        0        0        0 2024-01-05 09:11:06.000000 evo_framework-2024.5.35/evo_framework/core/evo_core_setting/control/__init__.py
--rw-r--r--   0        0        0     1201 2024-05-29 23:15:57.849250 evo_framework-2024.5.35/evo_framework/core/evo_core_setting/entity/ESetting.py
--rw-r--r--   0        0        0        0 2024-01-05 20:57:13.000000 evo_framework-2024.5.35/evo_framework/core/evo_core_setting/entity/__init__.py
--rw-r--r--   0        0        0       72 2024-05-29 23:15:57.848222 evo_framework-2024.5.35/evo_framework/core/evo_core_system/__init__.py
--rw-r--r--   0        0        0        0 2024-01-04 13:13:56.000000 evo_framework-2024.5.35/evo_framework/core/evo_core_system/control/__init__.py
--rw-r--r--   0        0        0     6742 2024-02-12 00:08:10.000000 evo_framework-2024.5.35/evo_framework/core/evo_core_system/utility/IuSystem.py
--rw-r--r--   0        0        0        0 2024-01-04 13:14:10.000000 evo_framework-2024.5.35/evo_framework/core/evo_core_system/utility/__init__.py
--rw-r--r--   0        0        0        0 2021-11-12 08:43:14.000000 evo_framework-2024.5.35/evo_framework/core/evo_core_type/__init__.py
--rwxr-xr-x   0        0        0      953 2024-04-22 18:31:06.740795 evo_framework-2024.5.35/evo_framework/core/evo_core_type/entity/EvoMap.py
--rw-r--r--   0        0        0       66 2024-05-29 23:15:57.849211 evo_framework-2024.5.35/evo_framework/core/evo_core_yaml/__init__.py
--rw-r--r--   0        0        0      304 2024-03-02 18:03:59.000000 evo_framework-2024.5.35/evo_framework/core/evo_core_yaml/utility/IuYaml.py
--rwxr-xr-x   0        0        0     9395 2024-05-29 23:15:57.849264 evo_framework-2024.5.35/evo_framework/entity/EObject.py
--rw-r--r--   0        0        0        0 2021-11-23 22:03:14.000000 evo_framework-2024.5.35/evo_framework/entity/IEObject.py
--rw-r--r--   0        0        0        0 2021-11-23 22:02:39.000000 evo_framework-2024.5.35/evo_framework/entity/IEvo.py
--rwxr-xr-x   0        0        0       64 2021-11-23 22:11:09.000000 evo_framework-2024.5.35/evo_framework/entity/Id.py
--rwxr-xr-x   0        0        0       62 2021-11-23 22:13:51.000000 evo_framework-2024.5.35/evo_framework/entity/Time.py
--rwxr-xr-x   0        0        0      181 2024-05-29 23:15:57.849324 evo_framework-2024.5.35/evo_framework/entity/__init__.py
--rwxr-xr-x   0        0        0        0 2024-01-14 01:56:17.000000 evo_framework-2024.5.35/evo_framework/utility/__init__.py
--rw-r--r--   0        0        0      557 2024-05-30 16:44:08.341663 evo_framework-2024.5.35/pyproject.toml
--rw-r--r--   0        0        0     1225 1970-01-01 00:00:00.000000 evo_framework-2024.5.35/PKG-INFO
+-rw-r--r--   0        0        0    13525 2024-05-28 16:27:09.302451 evo_framework-2024.5.36/LICENSE.txt
+-rw-r--r--   0        0        0      406 2024-05-28 16:35:10.344754 evo_framework-2024.5.36/README.md
+-rwxr-xr-x   0        0        0      770 2024-05-29 23:15:57.646008 evo_framework-2024.5.36/evo_framework/__init__.py
+-rwxr-xr-x   0        0        0     4030 2024-04-14 21:01:20.000000 evo_framework-2024.5.36/evo_framework/control/CObject.py
+-rwxr-xr-x   0        0        0       51 2024-05-29 23:15:57.849272 evo_framework-2024.5.36/evo_framework/control/__init__.py
+-rw-r--r--   0        0        0      399 2024-05-28 10:42:13.864068 evo_framework-2024.5.36/evo_framework/core/__init__.py
+-rwxr-xr-x   0        0        0      160 2024-05-29 23:15:57.645990 evo_framework-2024.5.36/evo_framework/core/evo_core_api/__init__.py
+-rw-r--r--   0        0        0     2657 2024-05-30 15:49:25.644184 evo_framework-2024.5.36/evo_framework/core/evo_core_api/automation/entity.yaml
+-rw-r--r--   0        0        0     6058 2024-05-29 23:52:16.739992 evo_framework-2024.5.36/evo_framework/core/evo_core_api/control/CApi.py
+-rw-r--r--   0        0        0    25474 2024-05-30 16:43:34.565564 evo_framework-2024.5.36/evo_framework/core/evo_core_api/control/CApiFlow.py
+-rw-r--r--   0        0        0      131 2024-05-29 23:15:57.840551 evo_framework-2024.5.36/evo_framework/core/evo_core_api/control/__init__.py
+-rw-r--r--   0        0        0     1893 2024-05-29 23:27:02.246146 evo_framework-2024.5.36/evo_framework/core/evo_core_api/entity/EAction.py
+-rw-r--r--   0        0        0     1306 2024-05-29 23:15:57.646050 evo_framework-2024.5.36/evo_framework/core/evo_core_api/entity/EActionTask.py
+-rw-r--r--   0        0        0     1770 2024-05-29 23:38:23.561186 evo_framework-2024.5.36/evo_framework/core/evo_core_api/entity/EApi.py
+-rw-r--r--   0        0        0     1781 2024-05-29 23:42:56.957602 evo_framework-2024.5.36/evo_framework/core/evo_core_api/entity/EApiAudio.py
+-rw-r--r--   0        0        0     3060 2024-05-29 23:29:47.211002 evo_framework-2024.5.36/evo_framework/core/evo_core_api/entity/EApiConfig.py
+-rw-r--r--   0        0        0     1775 2024-05-30 17:17:17.203521 evo_framework-2024.5.36/evo_framework/core/evo_core_api/entity/EApiFile.py
+-rw-r--r--   0        0        0     1786 2024-05-29 23:43:12.828390 evo_framework-2024.5.36/evo_framework/core/evo_core_api/entity/EApiImage.py
+-rw-r--r--   0        0        0     1770 2024-05-29 23:45:08.289661 evo_framework-2024.5.36/evo_framework/core/evo_core_api/entity/EApiVideo.py
+-rwxr-xr-x   0        0        0     2474 2024-05-30 17:16:56.438389 evo_framework-2024.5.36/evo_framework/core/evo_core_api/entity/ERequest.py
+-rwxr-xr-x   0        0        0     2189 2024-05-30 17:16:17.766668 evo_framework-2024.5.36/evo_framework/core/evo_core_api/entity/EResponse.py
+-rw-r--r--   0        0        0      568 2024-05-29 23:04:53.300310 evo_framework-2024.5.36/evo_framework/core/evo_core_api/entity/EnumApiAction.py
+-rw-r--r--   0        0        0      101 2024-03-22 09:24:36.000000 evo_framework-2024.5.36/evo_framework/core/evo_core_api/entity/EnumApiCompress.py
+-rw-r--r--   0        0        0       97 2024-03-22 09:18:53.000000 evo_framework-2024.5.36/evo_framework/core/evo_core_api/entity/EnumApiCrypto.py
+-rw-r--r--   0        0        0      274 2024-05-28 15:31:41.321728 evo_framework-2024.5.36/evo_framework/core/evo_core_api/entity/EnumApiType.py
+-rw-r--r--   0        0        0      493 2024-05-29 23:04:53.308461 evo_framework-2024.5.36/evo_framework/core/evo_core_api/entity/EnumApiVisibility.py
+-rw-r--r--   0        0        0        0 2024-05-27 12:52:18.397976 evo_framework-2024.5.36/evo_framework/core/evo_core_api/entity/EnumLanguage.py
+-rwxr-xr-x   0        0        0     1502 2024-05-29 23:16:21.970731 evo_framework-2024.5.36/evo_framework/core/evo_core_api/entity/__init__.py
+-rwxr-xr-x   0        0        0    11410 2024-05-29 23:15:57.840538 evo_framework-2024.5.36/evo_framework/core/evo_core_api/utility/IuApi.py
+-rw-r--r--   0        0        0    14944 2024-05-29 23:15:57.840524 evo_framework-2024.5.36/evo_framework/core/evo_core_api/utility/IuApiPb.py
+-rwxr-xr-x   0        0        0       64 2024-05-29 23:15:57.840493 evo_framework-2024.5.36/evo_framework/core/evo_core_api/utility/__init__.py
+-rwxr-xr-x   0        0        0      215 2024-05-29 23:15:57.848203 evo_framework-2024.5.36/evo_framework/core/evo_core_binary/__init__.py
+-rwxr-xr-x   0        0        0      120 2021-11-24 10:46:35.000000 evo_framework-2024.5.36/evo_framework/core/evo_core_binary/entity/IBinary.py
+-rwxr-xr-x   0        0        0     9089 2024-05-29 23:15:57.849286 evo_framework-2024.5.36/evo_framework/core/evo_core_binary/utility/IuBinary.py
+-rw-r--r--   0        0        0     6658 2024-05-29 23:15:57.848274 evo_framework-2024.5.36/evo_framework/core/evo_core_binary/utility/IuBinaryAsync.py
+-rw-r--r--   0        0        0     7700 2024-05-29 23:15:57.848234 evo_framework-2024.5.36/evo_framework/core/evo_core_binary/utility/UBinary.py
+-rw-r--r--   0        0        0     1324 2024-05-29 23:15:57.844638 evo_framework-2024.5.36/evo_framework/core/evo_core_boot/control/CBoot.py
+-rw-r--r--   0        0        0      281 2024-04-15 19:43:35.988232 evo_framework-2024.5.36/evo_framework/core/evo_core_bridge/IBridge.py
+-rw-r--r--   0        0        0       75 2024-05-29 23:15:57.848167 evo_framework-2024.5.36/evo_framework/core/evo_core_convert/__init__.py
+-rw-r--r--   0        0        0     6213 2024-05-29 23:54:10.283288 evo_framework-2024.5.36/evo_framework/core/evo_core_convert/test_evo_core_binary.py
+-rw-r--r--   0        0        0      841 2024-04-12 09:23:48.000000 evo_framework-2024.5.36/evo_framework/core/evo_core_convert/utility/IuConvert.py
+-rw-r--r--   0        0        0        0 2021-11-12 08:43:14.000000 evo_framework-2024.5.36/evo_framework/core/evo_core_convert/utility/__init__.py
+-rw-r--r--   0        0        0      236 2024-05-29 23:15:57.848112 evo_framework-2024.5.36/evo_framework/core/evo_core_crypto/__init__.py
+-rw-r--r--   0        0        0     1470 2024-03-26 15:03:45.000000 evo_framework-2024.5.36/evo_framework/core/evo_core_crypto/utility/IuCryptChacha.py
+-rwxr-xr-x   0        0        0     1467 2024-05-29 23:15:57.848244 evo_framework-2024.5.36/evo_framework/core/evo_core_crypto/utility/IuCryptEC.py
+-rwxr-xr-x   0        0        0      743 2024-03-17 11:26:36.000000 evo_framework-2024.5.36/evo_framework/core/evo_core_crypto/utility/IuCryptHash.py
+-rw-r--r--   0        0        0     1332 2024-05-29 23:15:57.848017 evo_framework-2024.5.36/evo_framework/core/evo_core_file/entity/EFileChunk.py
+-rw-r--r--   0        0        0      699 2024-05-29 23:15:57.848149 evo_framework-2024.5.36/evo_framework/core/evo_core_foundation/IFoundation.py
+-rw-r--r--   0        0        0       63 2024-05-29 23:15:57.849413 evo_framework-2024.5.36/evo_framework/core/evo_core_key/__init__.py
+-rw-r--r--   0        0        0      893 2024-05-29 23:15:57.844661 evo_framework-2024.5.36/evo_framework/core/evo_core_key/utility/IuKey.py
+-rw-r--r--   0        0        0       63 2024-05-29 23:15:57.848179 evo_framework-2024.5.36/evo_framework/core/evo_core_log/__init__.py
+-rw-r--r--   0        0        0     2150 2024-05-29 23:15:57.848192 evo_framework-2024.5.36/evo_framework/core/evo_core_log/utility/IuLog.py
+-rw-r--r--   0        0        0     2289 2024-03-22 09:09:45.000000 evo_framework-2024.5.36/evo_framework/core/evo_core_log/utility/ULogger.py
+-rwxr-xr-x   0        0        0      146 2024-05-29 23:15:57.848259 evo_framework-2024.5.36/evo_framework/core/evo_core_setting/__init__.py
+-rw-r--r--   0        0        0     2813 2024-05-29 23:15:57.849237 evo_framework-2024.5.36/evo_framework/core/evo_core_setting/control/CSetting.py
+-rwxr-xr-x   0        0        0        0 2024-01-05 09:11:06.000000 evo_framework-2024.5.36/evo_framework/core/evo_core_setting/control/__init__.py
+-rw-r--r--   0        0        0     1201 2024-05-29 23:15:57.849250 evo_framework-2024.5.36/evo_framework/core/evo_core_setting/entity/ESetting.py
+-rw-r--r--   0        0        0        0 2024-01-05 20:57:13.000000 evo_framework-2024.5.36/evo_framework/core/evo_core_setting/entity/__init__.py
+-rw-r--r--   0        0        0       72 2024-05-29 23:15:57.848222 evo_framework-2024.5.36/evo_framework/core/evo_core_system/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-04 13:13:56.000000 evo_framework-2024.5.36/evo_framework/core/evo_core_system/control/__init__.py
+-rw-r--r--   0        0        0     6742 2024-02-12 00:08:10.000000 evo_framework-2024.5.36/evo_framework/core/evo_core_system/utility/IuSystem.py
+-rw-r--r--   0        0        0        0 2024-01-04 13:14:10.000000 evo_framework-2024.5.36/evo_framework/core/evo_core_system/utility/__init__.py
+-rw-r--r--   0        0        0        0 2021-11-12 08:43:14.000000 evo_framework-2024.5.36/evo_framework/core/evo_core_type/__init__.py
+-rwxr-xr-x   0        0        0      953 2024-04-22 18:31:06.740795 evo_framework-2024.5.36/evo_framework/core/evo_core_type/entity/EvoMap.py
+-rw-r--r--   0        0        0       66 2024-05-29 23:15:57.849211 evo_framework-2024.5.36/evo_framework/core/evo_core_yaml/__init__.py
+-rw-r--r--   0        0        0      304 2024-03-02 18:03:59.000000 evo_framework-2024.5.36/evo_framework/core/evo_core_yaml/utility/IuYaml.py
+-rwxr-xr-x   0        0        0     9395 2024-05-29 23:15:57.849264 evo_framework-2024.5.36/evo_framework/entity/EObject.py
+-rw-r--r--   0        0        0        0 2021-11-23 22:03:14.000000 evo_framework-2024.5.36/evo_framework/entity/IEObject.py
+-rw-r--r--   0        0        0        0 2021-11-23 22:02:39.000000 evo_framework-2024.5.36/evo_framework/entity/IEvo.py
+-rwxr-xr-x   0        0        0       64 2021-11-23 22:11:09.000000 evo_framework-2024.5.36/evo_framework/entity/Id.py
+-rwxr-xr-x   0        0        0       62 2021-11-23 22:13:51.000000 evo_framework-2024.5.36/evo_framework/entity/Time.py
+-rwxr-xr-x   0        0        0      181 2024-05-29 23:15:57.849324 evo_framework-2024.5.36/evo_framework/entity/__init__.py
+-rwxr-xr-x   0        0        0        0 2024-01-14 01:56:17.000000 evo_framework-2024.5.36/evo_framework/utility/__init__.py
+-rw-r--r--   0        0        0      557 2024-05-30 17:24:14.122364 evo_framework-2024.5.36/pyproject.toml
+-rw-r--r--   0        0        0     1225 1970-01-01 00:00:00.000000 evo_framework-2024.5.36/PKG-INFO
```

### Comparing `evo_framework-2024.5.35/LICENSE.txt` & `evo_framework-2024.5.36/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.35/evo_framework/__init__.py` & `evo_framework-2024.5.36/evo_framework/__init__.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.35/evo_framework/control/CObject.py` & `evo_framework-2024.5.36/evo_framework/control/CObject.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.35/evo_framework/core/evo_core_api/automation/entity.yaml` & `evo_framework-2024.5.36/evo_framework/core/evo_core_api/automation/entity.yaml`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.35/evo_framework/core/evo_core_api/control/CApi.py` & `evo_framework-2024.5.36/evo_framework/core/evo_core_api/control/CApi.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.35/evo_framework/core/evo_core_api/control/CApiFlow.py` & `evo_framework-2024.5.36/evo_framework/core/evo_core_api/control/CApiFlow.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.35/evo_framework/core/evo_core_api/entity/EAction.py` & `evo_framework-2024.5.36/evo_framework/core/evo_core_api/entity/EAction.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.35/evo_framework/core/evo_core_api/entity/EActionTask.py` & `evo_framework-2024.5.36/evo_framework/core/evo_core_api/entity/EActionTask.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.35/evo_framework/core/evo_core_api/entity/EApi.py` & `evo_framework-2024.5.36/evo_framework/core/evo_core_api/entity/EApi.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.35/evo_framework/core/evo_core_api/entity/EApiAudio.py` & `evo_framework-2024.5.36/evo_framework/core/evo_core_api/entity/EApiAudio.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.35/evo_framework/core/evo_core_api/entity/EApiConfig.py` & `evo_framework-2024.5.36/evo_framework/core/evo_core_api/entity/EApiConfig.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.35/evo_framework/core/evo_core_api/entity/EApiFile.py` & `evo_framework-2024.5.36/evo_framework/core/evo_core_api/entity/EApiFile.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 		self.length = self._doReadInt(stream)
 		self.data = self._doReadBytes(stream)
 	
 	def __str__(self) -> str:
 		strReturn = "\n".join([
 				super().__str__(),
 							
-				f"\tisUrl:{ self.isUrl  }",
+				f"\tisUrl:{self.isUrl}",
 				f"\tname:{ self.name  }",
 				f"\text:{ self.ext  }",
 				f"\tlength:{ self.length  }",
 				#f"\tdata:{ self.data  }",
 							]) 
 		return strReturn
```

### Comparing `evo_framework-2024.5.35/evo_framework/core/evo_core_api/entity/EApiImage.py` & `evo_framework-2024.5.36/evo_framework/core/evo_core_api/entity/EApiImage.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.35/evo_framework/core/evo_core_api/entity/EApiVideo.py` & `evo_framework-2024.5.36/evo_framework/core/evo_core_api/entity/EApiVideo.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.35/evo_framework/core/evo_core_api/entity/ERequest.py` & `evo_framework-2024.5.36/evo_framework/core/evo_core_api/entity/ERequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -55,19 +55,19 @@
 		self.length = self._doReadInt(stream)
 		self.data = self._doReadBytes(stream)
 	
 	def __str__(self) -> str:
 		strReturn = "\n".join([
 				super().__str__(),
 							
-				f"\tenumApiCrypto:{ self.enumApiCrypto  }",
-				f"\tpk:{ self.pk!r }",
-				f"\tcipher:{ self.cipher!r  }",
-				f"\tsign:{ self.sign!r  }",
-				f"\thash:{ self.hash!r  }",
-				f"\tchunk:{ self.chunk  }",
-				f"\tchunkTotal:{ self.chunkTotal  }",
-				f"\tlength:{ self.length  }",
+				f"\tenumApiCrypto:{self.enumApiCrypto}",
+				f"\tpk:{self.pk!r}",
+				f"\tcipher:{self.cipher!r}",
+				f"\tsign:{self.sign!r}",
+				f"\thash:{self.hash!r}",
+				f"\tchunk:{self.chunk}",
+				f"\tchunkTotal:{self.chunkTotal}",
+				f"\tlength:{self.length}",
 				#f"\tdata:{ self.data  }",
 							]) 
 		return strReturn
```

### Comparing `evo_framework-2024.5.35/evo_framework/core/evo_core_api/entity/EResponse.py` & `evo_framework-2024.5.36/evo_framework/core/evo_core_api/entity/EResponse.py`

 * *Files 18% similar despite different names*

```diff
@@ -51,18 +51,18 @@
 		self.isError = self._doReadBool(stream)
 		self.error = self._doReadStr(stream)
 	
 	def __str__(self) -> str:
 		strReturn = "\n".join([
 				super().__str__(),
 							
-				f"\tsign:{ self.sign!r  }",
-				f"\thash:{ self.hash!r  }",
-				f"\tchunk:{ self.chunk  }",
-				f"\tchunkTotal:{ self.chunkTotal  }",
-				f"\tlength:{ self.length  }",
+				f"\tsign:{self.sign!r}",
+				f"\thash:{self.hash!r}",
+				f"\tchunk:{self.chunk}",
+				f"\tchunkTotal:{self.chunkTotal}",
+				f"\tlength:{self.length}",
 				#f"\tdata:{ self.data  }",
-				f"\tisError:{ self.isError  }",
-				f"\terror:{ self.error  }",
+				f"\tisError:{self.isError}",
+				f"\terror:{self.error}",
 							]) 
 		return strReturn
```

### Comparing `evo_framework-2024.5.35/evo_framework/core/evo_core_api/entity/EnumApiAction.py` & `evo_framework-2024.5.36/evo_framework/core/evo_core_api/entity/EnumApiAction.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.35/evo_framework/core/evo_core_api/entity/__init__.py` & `evo_framework-2024.5.36/evo_framework/core/evo_core_api/entity/__init__.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.35/evo_framework/core/evo_core_api/utility/IuApi.py` & `evo_framework-2024.5.36/evo_framework/core/evo_core_api/utility/IuApi.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.35/evo_framework/core/evo_core_api/utility/IuApiPb.py` & `evo_framework-2024.5.36/evo_framework/core/evo_core_api/utility/IuApiPb.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.35/evo_framework/core/evo_core_binary/utility/IuBinary.py` & `evo_framework-2024.5.36/evo_framework/core/evo_core_binary/utility/IuBinary.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.35/evo_framework/core/evo_core_binary/utility/IuBinaryAsync.py` & `evo_framework-2024.5.36/evo_framework/core/evo_core_binary/utility/IuBinaryAsync.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.35/evo_framework/core/evo_core_binary/utility/UBinary.py` & `evo_framework-2024.5.36/evo_framework/core/evo_core_binary/utility/UBinary.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.35/evo_framework/core/evo_core_boot/control/CBoot.py` & `evo_framework-2024.5.36/evo_framework/core/evo_core_boot/control/CBoot.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.35/evo_framework/core/evo_core_convert/test_evo_core_binary.py` & `evo_framework-2024.5.36/evo_framework/core/evo_core_convert/test_evo_core_binary.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.35/evo_framework/core/evo_core_convert/utility/IuConvert.py` & `evo_framework-2024.5.36/evo_framework/core/evo_core_convert/utility/IuConvert.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.35/evo_framework/core/evo_core_crypto/utility/IuCryptChacha.py` & `evo_framework-2024.5.36/evo_framework/core/evo_core_crypto/utility/IuCryptChacha.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.35/evo_framework/core/evo_core_crypto/utility/IuCryptEC.py` & `evo_framework-2024.5.36/evo_framework/core/evo_core_crypto/utility/IuCryptEC.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.35/evo_framework/core/evo_core_crypto/utility/IuCryptHash.py` & `evo_framework-2024.5.36/evo_framework/core/evo_core_crypto/utility/IuCryptHash.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.35/evo_framework/core/evo_core_file/entity/EFileChunk.py` & `evo_framework-2024.5.36/evo_framework/core/evo_core_file/entity/EFileChunk.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.35/evo_framework/core/evo_core_foundation/IFoundation.py` & `evo_framework-2024.5.36/evo_framework/core/evo_core_foundation/IFoundation.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.35/evo_framework/core/evo_core_key/utility/IuKey.py` & `evo_framework-2024.5.36/evo_framework/core/evo_core_key/utility/IuKey.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.35/evo_framework/core/evo_core_log/utility/IuLog.py` & `evo_framework-2024.5.36/evo_framework/core/evo_core_log/utility/IuLog.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.35/evo_framework/core/evo_core_log/utility/ULogger.py` & `evo_framework-2024.5.36/evo_framework/core/evo_core_log/utility/ULogger.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.35/evo_framework/core/evo_core_setting/control/CSetting.py` & `evo_framework-2024.5.36/evo_framework/core/evo_core_setting/control/CSetting.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.35/evo_framework/core/evo_core_setting/entity/ESetting.py` & `evo_framework-2024.5.36/evo_framework/core/evo_core_setting/entity/ESetting.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.35/evo_framework/core/evo_core_system/utility/IuSystem.py` & `evo_framework-2024.5.36/evo_framework/core/evo_core_system/utility/IuSystem.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.35/evo_framework/core/evo_core_type/entity/EvoMap.py` & `evo_framework-2024.5.36/evo_framework/core/evo_core_type/entity/EvoMap.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.35/evo_framework/entity/EObject.py` & `evo_framework-2024.5.36/evo_framework/entity/EObject.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.35/pyproject.toml` & `evo_framework-2024.5.36/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "evo-framework"
-version = "2024.5.35"
+version = "2024.5.36"
 description = "evo framework python"
 authors = ["cyborg-ai-git <129898917+cyborg-ai-git@users.noreply.github.com>"]
 readme = "README.md"
 #packages = [{include = "evo"}]
 license = "CC BY-NC-ND 4.0"
 include = ["LICENSE.txt"]
```

### Comparing `evo_framework-2024.5.35/PKG-INFO` & `evo_framework-2024.5.36/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evo-framework
-Version: 2024.5.35
+Version: 2024.5.36
 Summary: evo framework python
 License: CC BY-NC-ND 4.0
 Author: cyborg-ai-git
 Author-email: 129898917+cyborg-ai-git@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

