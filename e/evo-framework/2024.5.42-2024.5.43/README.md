# Comparing `tmp/evo_framework-2024.5.42.tar.gz` & `tmp/evo_framework-2024.5.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evo_framework-2024.5.42.tar", max compression
+gzip compressed data, was "evo_framework-2024.5.43.tar", max compression
```

## Comparing `evo_framework-2024.5.42.tar` & `evo_framework-2024.5.43.tar`

### file list

```diff
@@ -1,73 +1,73 @@
--rw-r--r--   0        0        0    13525 2024-05-28 16:27:09.302451 evo_framework-2024.5.42/LICENSE.txt
--rw-r--r--   0        0        0      406 2024-05-28 16:35:10.344754 evo_framework-2024.5.42/README.md
--rwxr-xr-x   0        0        0      770 2024-05-29 23:15:57.646008 evo_framework-2024.5.42/evo_framework/__init__.py
--rwxr-xr-x   0        0        0     4030 2024-04-14 21:01:20.000000 evo_framework-2024.5.42/evo_framework/control/CObject.py
--rwxr-xr-x   0        0        0       51 2024-05-29 23:15:57.849272 evo_framework-2024.5.42/evo_framework/control/__init__.py
--rw-r--r--   0        0        0      399 2024-05-28 10:42:13.864068 evo_framework-2024.5.42/evo_framework/core/__init__.py
--rwxr-xr-x   0        0        0      160 2024-05-29 23:15:57.645990 evo_framework-2024.5.42/evo_framework/core/evo_core_api/__init__.py
--rw-r--r--   0        0        0     2332 2024-05-31 20:33:51.808286 evo_framework-2024.5.42/evo_framework/core/evo_core_api/automation/entity.yaml
--rw-r--r--   0        0        0     6058 2024-05-29 23:52:16.739992 evo_framework-2024.5.42/evo_framework/core/evo_core_api/control/CApi.py
--rw-r--r--   0        0        0    25500 2024-05-31 14:22:31.688287 evo_framework-2024.5.42/evo_framework/core/evo_core_api/control/CApiFlow.py
--rw-r--r--   0        0        0      131 2024-05-29 23:15:57.840551 evo_framework-2024.5.42/evo_framework/core/evo_core_api/control/__init__.py
--rw-r--r--   0        0        0     3344 2024-05-31 21:01:27.585493 evo_framework-2024.5.42/evo_framework/core/evo_core_api/entity/EAction.py
--rw-r--r--   0        0        0     1306 2024-05-29 23:15:57.646050 evo_framework-2024.5.42/evo_framework/core/evo_core_api/entity/EActionTask.py
--rw-r--r--   0        0        0     1770 2024-05-29 23:38:23.561186 evo_framework-2024.5.42/evo_framework/core/evo_core_api/entity/EApi.py
--rw-r--r--   0        0        0     3029 2024-05-31 21:11:15.610746 evo_framework-2024.5.42/evo_framework/core/evo_core_api/entity/EApiConfig.py
--rw-r--r--   0        0        0     2681 2024-05-31 21:16:03.003273 evo_framework-2024.5.42/evo_framework/core/evo_core_api/entity/EApiFile.py
--rw-r--r--   0        0        0     1525 2024-05-31 21:08:35.640177 evo_framework-2024.5.42/evo_framework/core/evo_core_api/entity/EApiText.py
--rwxr-xr-x   0        0        0     2510 2024-05-31 21:21:54.441023 evo_framework-2024.5.42/evo_framework/core/evo_core_api/entity/ERequest.py
--rwxr-xr-x   0        0        0     2155 2024-05-31 21:07:11.505845 evo_framework-2024.5.42/evo_framework/core/evo_core_api/entity/EResponse.py
--rw-r--r--   0        0        0      568 2024-05-29 23:04:53.300310 evo_framework-2024.5.42/evo_framework/core/evo_core_api/entity/EnumApiAction.py
--rw-r--r--   0        0        0      101 2024-03-22 09:24:36.000000 evo_framework-2024.5.42/evo_framework/core/evo_core_api/entity/EnumApiCompress.py
--rw-r--r--   0        0        0       97 2024-03-22 09:18:53.000000 evo_framework-2024.5.42/evo_framework/core/evo_core_api/entity/EnumApiCrypto.py
--rw-r--r--   0        0        0      274 2024-05-28 15:31:41.321728 evo_framework-2024.5.42/evo_framework/core/evo_core_api/entity/EnumApiType.py
--rw-r--r--   0        0        0      493 2024-05-29 23:04:53.308461 evo_framework-2024.5.42/evo_framework/core/evo_core_api/entity/EnumApiVisibility.py
--rw-r--r--   0        0        0        0 2024-05-27 12:52:18.397976 evo_framework-2024.5.42/evo_framework/core/evo_core_api/entity/EnumLanguage.py
--rwxr-xr-x   0        0        0     1574 2024-05-31 21:03:43.170559 evo_framework-2024.5.42/evo_framework/core/evo_core_api/entity/__init__.py
--rwxr-xr-x   0        0        0     7848 2024-05-31 21:16:51.768317 evo_framework-2024.5.42/evo_framework/core/evo_core_api/utility/IuApi.py
--rw-r--r--   0        0        0    14944 2024-05-29 23:15:57.840524 evo_framework-2024.5.42/evo_framework/core/evo_core_api/utility/IuApiPb.py
--rwxr-xr-x   0        0        0       64 2024-05-29 23:15:57.840493 evo_framework-2024.5.42/evo_framework/core/evo_core_api/utility/__init__.py
--rwxr-xr-x   0        0        0      215 2024-05-29 23:15:57.848203 evo_framework-2024.5.42/evo_framework/core/evo_core_binary/__init__.py
--rwxr-xr-x   0        0        0      120 2021-11-24 10:46:35.000000 evo_framework-2024.5.42/evo_framework/core/evo_core_binary/entity/IBinary.py
--rwxr-xr-x   0        0        0     9089 2024-05-29 23:15:57.849286 evo_framework-2024.5.42/evo_framework/core/evo_core_binary/utility/IuBinary.py
--rw-r--r--   0        0        0     6658 2024-05-29 23:15:57.848274 evo_framework-2024.5.42/evo_framework/core/evo_core_binary/utility/IuBinaryAsync.py
--rw-r--r--   0        0        0     7700 2024-05-30 20:17:43.461565 evo_framework-2024.5.42/evo_framework/core/evo_core_binary/utility/UBinary.py
--rw-r--r--   0        0        0     1324 2024-05-29 23:15:57.844638 evo_framework-2024.5.42/evo_framework/core/evo_core_boot/control/CBoot.py
--rw-r--r--   0        0        0      281 2024-04-15 19:43:35.988232 evo_framework-2024.5.42/evo_framework/core/evo_core_bridge/IBridge.py
--rw-r--r--   0        0        0       75 2024-05-29 23:15:57.848167 evo_framework-2024.5.42/evo_framework/core/evo_core_convert/__init__.py
--rw-r--r--   0        0        0     6213 2024-05-29 23:54:10.283288 evo_framework-2024.5.42/evo_framework/core/evo_core_convert/test_evo_core_binary.py
--rw-r--r--   0        0        0      841 2024-04-12 09:23:48.000000 evo_framework-2024.5.42/evo_framework/core/evo_core_convert/utility/IuConvert.py
--rw-r--r--   0        0        0        0 2021-11-12 08:43:14.000000 evo_framework-2024.5.42/evo_framework/core/evo_core_convert/utility/__init__.py
--rw-r--r--   0        0        0      236 2024-05-29 23:15:57.848112 evo_framework-2024.5.42/evo_framework/core/evo_core_crypto/__init__.py
--rw-r--r--   0        0        0     1470 2024-03-26 15:03:45.000000 evo_framework-2024.5.42/evo_framework/core/evo_core_crypto/utility/IuCryptChacha.py
--rwxr-xr-x   0        0        0     1467 2024-05-29 23:15:57.848244 evo_framework-2024.5.42/evo_framework/core/evo_core_crypto/utility/IuCryptEC.py
--rwxr-xr-x   0        0        0      743 2024-03-17 11:26:36.000000 evo_framework-2024.5.42/evo_framework/core/evo_core_crypto/utility/IuCryptHash.py
--rw-r--r--   0        0        0     1332 2024-05-29 23:15:57.848017 evo_framework-2024.5.42/evo_framework/core/evo_core_file/entity/EFileChunk.py
--rw-r--r--   0        0        0      699 2024-05-29 23:15:57.848149 evo_framework-2024.5.42/evo_framework/core/evo_core_foundation/IFoundation.py
--rw-r--r--   0        0        0       63 2024-05-29 23:15:57.849413 evo_framework-2024.5.42/evo_framework/core/evo_core_key/__init__.py
--rw-r--r--   0        0        0      893 2024-05-29 23:15:57.844661 evo_framework-2024.5.42/evo_framework/core/evo_core_key/utility/IuKey.py
--rw-r--r--   0        0        0       63 2024-05-29 23:15:57.848179 evo_framework-2024.5.42/evo_framework/core/evo_core_log/__init__.py
--rw-r--r--   0        0        0     2150 2024-05-29 23:15:57.848192 evo_framework-2024.5.42/evo_framework/core/evo_core_log/utility/IuLog.py
--rw-r--r--   0        0        0     2289 2024-03-22 09:09:45.000000 evo_framework-2024.5.42/evo_framework/core/evo_core_log/utility/ULogger.py
--rwxr-xr-x   0        0        0      146 2024-05-29 23:15:57.848259 evo_framework-2024.5.42/evo_framework/core/evo_core_setting/__init__.py
--rw-r--r--   0        0        0     2813 2024-05-29 23:15:57.849237 evo_framework-2024.5.42/evo_framework/core/evo_core_setting/control/CSetting.py
--rwxr-xr-x   0        0        0        0 2024-01-05 09:11:06.000000 evo_framework-2024.5.42/evo_framework/core/evo_core_setting/control/__init__.py
--rw-r--r--   0        0        0     1201 2024-05-29 23:15:57.849250 evo_framework-2024.5.42/evo_framework/core/evo_core_setting/entity/ESetting.py
--rw-r--r--   0        0        0        0 2024-01-05 20:57:13.000000 evo_framework-2024.5.42/evo_framework/core/evo_core_setting/entity/__init__.py
--rw-r--r--   0        0        0       72 2024-05-29 23:15:57.848222 evo_framework-2024.5.42/evo_framework/core/evo_core_system/__init__.py
--rw-r--r--   0        0        0        0 2024-01-04 13:13:56.000000 evo_framework-2024.5.42/evo_framework/core/evo_core_system/control/__init__.py
--rw-r--r--   0        0        0     6742 2024-02-12 00:08:10.000000 evo_framework-2024.5.42/evo_framework/core/evo_core_system/utility/IuSystem.py
--rw-r--r--   0        0        0        0 2024-01-04 13:14:10.000000 evo_framework-2024.5.42/evo_framework/core/evo_core_system/utility/__init__.py
--rw-r--r--   0        0        0        0 2021-11-12 08:43:14.000000 evo_framework-2024.5.42/evo_framework/core/evo_core_type/__init__.py
--rwxr-xr-x   0        0        0      953 2024-04-22 18:31:06.740795 evo_framework-2024.5.42/evo_framework/core/evo_core_type/entity/EvoMap.py
--rw-r--r--   0        0        0       66 2024-05-29 23:15:57.849211 evo_framework-2024.5.42/evo_framework/core/evo_core_yaml/__init__.py
--rw-r--r--   0        0        0      304 2024-03-02 18:03:59.000000 evo_framework-2024.5.42/evo_framework/core/evo_core_yaml/utility/IuYaml.py
--rwxr-xr-x   0        0        0     9395 2024-05-29 23:15:57.849264 evo_framework-2024.5.42/evo_framework/entity/EObject.py
--rw-r--r--   0        0        0        0 2021-11-23 22:03:14.000000 evo_framework-2024.5.42/evo_framework/entity/IEObject.py
--rw-r--r--   0        0        0        0 2021-11-23 22:02:39.000000 evo_framework-2024.5.42/evo_framework/entity/IEvo.py
--rwxr-xr-x   0        0        0       64 2021-11-23 22:11:09.000000 evo_framework-2024.5.42/evo_framework/entity/Id.py
--rwxr-xr-x   0        0        0       62 2021-11-23 22:13:51.000000 evo_framework-2024.5.42/evo_framework/entity/Time.py
--rwxr-xr-x   0        0        0      181 2024-05-29 23:15:57.849324 evo_framework-2024.5.42/evo_framework/entity/__init__.py
--rwxr-xr-x   0        0        0        0 2024-01-14 01:56:17.000000 evo_framework-2024.5.42/evo_framework/utility/__init__.py
--rw-r--r--   0        0        0      583 2024-05-31 21:20:56.933884 evo_framework-2024.5.42/pyproject.toml
--rw-r--r--   0        0        0     1271 1970-01-01 00:00:00.000000 evo_framework-2024.5.42/PKG-INFO
+-rw-r--r--   0        0        0    13525 2024-05-28 16:27:09.302451 evo_framework-2024.5.43/LICENSE.txt
+-rw-r--r--   0        0        0      406 2024-05-28 16:35:10.344754 evo_framework-2024.5.43/README.md
+-rwxr-xr-x   0        0        0      770 2024-05-29 23:15:57.646008 evo_framework-2024.5.43/evo_framework/__init__.py
+-rwxr-xr-x   0        0        0     4030 2024-04-14 21:01:20.000000 evo_framework-2024.5.43/evo_framework/control/CObject.py
+-rwxr-xr-x   0        0        0       51 2024-05-29 23:15:57.849272 evo_framework-2024.5.43/evo_framework/control/__init__.py
+-rw-r--r--   0        0        0      399 2024-05-28 10:42:13.864068 evo_framework-2024.5.43/evo_framework/core/__init__.py
+-rwxr-xr-x   0        0        0      160 2024-05-29 23:15:57.645990 evo_framework-2024.5.43/evo_framework/core/evo_core_api/__init__.py
+-rw-r--r--   0        0        0     2365 2024-05-31 21:24:54.044751 evo_framework-2024.5.43/evo_framework/core/evo_core_api/automation/entity.yaml
+-rw-r--r--   0        0        0     6058 2024-05-29 23:52:16.739992 evo_framework-2024.5.43/evo_framework/core/evo_core_api/control/CApi.py
+-rw-r--r--   0        0        0    25500 2024-05-31 14:22:31.688287 evo_framework-2024.5.43/evo_framework/core/evo_core_api/control/CApiFlow.py
+-rw-r--r--   0        0        0      131 2024-05-29 23:15:57.840551 evo_framework-2024.5.43/evo_framework/core/evo_core_api/control/__init__.py
+-rw-r--r--   0        0        0     3314 2024-05-31 21:23:45.784186 evo_framework-2024.5.43/evo_framework/core/evo_core_api/entity/EAction.py
+-rw-r--r--   0        0        0     1306 2024-05-29 23:15:57.646050 evo_framework-2024.5.43/evo_framework/core/evo_core_api/entity/EActionTask.py
+-rw-r--r--   0        0        0     1770 2024-05-29 23:38:23.561186 evo_framework-2024.5.43/evo_framework/core/evo_core_api/entity/EApi.py
+-rw-r--r--   0        0        0     3029 2024-05-31 21:11:15.610746 evo_framework-2024.5.43/evo_framework/core/evo_core_api/entity/EApiConfig.py
+-rw-r--r--   0        0        0     2681 2024-05-31 21:16:03.003273 evo_framework-2024.5.43/evo_framework/core/evo_core_api/entity/EApiFile.py
+-rw-r--r--   0        0        0     1525 2024-05-31 21:08:35.640177 evo_framework-2024.5.43/evo_framework/core/evo_core_api/entity/EApiText.py
+-rwxr-xr-x   0        0        0     2510 2024-05-31 21:21:54.441023 evo_framework-2024.5.43/evo_framework/core/evo_core_api/entity/ERequest.py
+-rwxr-xr-x   0        0        0     2155 2024-05-31 21:07:11.505845 evo_framework-2024.5.43/evo_framework/core/evo_core_api/entity/EResponse.py
+-rw-r--r--   0        0        0      568 2024-05-29 23:04:53.300310 evo_framework-2024.5.43/evo_framework/core/evo_core_api/entity/EnumApiAction.py
+-rw-r--r--   0        0        0      101 2024-03-22 09:24:36.000000 evo_framework-2024.5.43/evo_framework/core/evo_core_api/entity/EnumApiCompress.py
+-rw-r--r--   0        0        0       97 2024-03-22 09:18:53.000000 evo_framework-2024.5.43/evo_framework/core/evo_core_api/entity/EnumApiCrypto.py
+-rw-r--r--   0        0        0      274 2024-05-28 15:31:41.321728 evo_framework-2024.5.43/evo_framework/core/evo_core_api/entity/EnumApiType.py
+-rw-r--r--   0        0        0      493 2024-05-29 23:04:53.308461 evo_framework-2024.5.43/evo_framework/core/evo_core_api/entity/EnumApiVisibility.py
+-rw-r--r--   0        0        0        0 2024-05-27 12:52:18.397976 evo_framework-2024.5.43/evo_framework/core/evo_core_api/entity/EnumLanguage.py
+-rwxr-xr-x   0        0        0     1574 2024-05-31 21:03:43.170559 evo_framework-2024.5.43/evo_framework/core/evo_core_api/entity/__init__.py
+-rwxr-xr-x   0        0        0     7848 2024-05-31 21:16:51.768317 evo_framework-2024.5.43/evo_framework/core/evo_core_api/utility/IuApi.py
+-rw-r--r--   0        0        0    14944 2024-05-29 23:15:57.840524 evo_framework-2024.5.43/evo_framework/core/evo_core_api/utility/IuApiPb.py
+-rwxr-xr-x   0        0        0       64 2024-05-29 23:15:57.840493 evo_framework-2024.5.43/evo_framework/core/evo_core_api/utility/__init__.py
+-rwxr-xr-x   0        0        0      215 2024-05-29 23:15:57.848203 evo_framework-2024.5.43/evo_framework/core/evo_core_binary/__init__.py
+-rwxr-xr-x   0        0        0      120 2021-11-24 10:46:35.000000 evo_framework-2024.5.43/evo_framework/core/evo_core_binary/entity/IBinary.py
+-rwxr-xr-x   0        0        0     9089 2024-05-29 23:15:57.849286 evo_framework-2024.5.43/evo_framework/core/evo_core_binary/utility/IuBinary.py
+-rw-r--r--   0        0        0     6658 2024-05-29 23:15:57.848274 evo_framework-2024.5.43/evo_framework/core/evo_core_binary/utility/IuBinaryAsync.py
+-rw-r--r--   0        0        0     7700 2024-05-30 20:17:43.461565 evo_framework-2024.5.43/evo_framework/core/evo_core_binary/utility/UBinary.py
+-rw-r--r--   0        0        0     1324 2024-05-29 23:15:57.844638 evo_framework-2024.5.43/evo_framework/core/evo_core_boot/control/CBoot.py
+-rw-r--r--   0        0        0      281 2024-04-15 19:43:35.988232 evo_framework-2024.5.43/evo_framework/core/evo_core_bridge/IBridge.py
+-rw-r--r--   0        0        0       75 2024-05-29 23:15:57.848167 evo_framework-2024.5.43/evo_framework/core/evo_core_convert/__init__.py
+-rw-r--r--   0        0        0     6213 2024-05-29 23:54:10.283288 evo_framework-2024.5.43/evo_framework/core/evo_core_convert/test_evo_core_binary.py
+-rw-r--r--   0        0        0      841 2024-04-12 09:23:48.000000 evo_framework-2024.5.43/evo_framework/core/evo_core_convert/utility/IuConvert.py
+-rw-r--r--   0        0        0        0 2021-11-12 08:43:14.000000 evo_framework-2024.5.43/evo_framework/core/evo_core_convert/utility/__init__.py
+-rw-r--r--   0        0        0      236 2024-05-29 23:15:57.848112 evo_framework-2024.5.43/evo_framework/core/evo_core_crypto/__init__.py
+-rw-r--r--   0        0        0     1470 2024-03-26 15:03:45.000000 evo_framework-2024.5.43/evo_framework/core/evo_core_crypto/utility/IuCryptChacha.py
+-rwxr-xr-x   0        0        0     1467 2024-05-29 23:15:57.848244 evo_framework-2024.5.43/evo_framework/core/evo_core_crypto/utility/IuCryptEC.py
+-rwxr-xr-x   0        0        0      743 2024-03-17 11:26:36.000000 evo_framework-2024.5.43/evo_framework/core/evo_core_crypto/utility/IuCryptHash.py
+-rw-r--r--   0        0        0     1332 2024-05-29 23:15:57.848017 evo_framework-2024.5.43/evo_framework/core/evo_core_file/entity/EFileChunk.py
+-rw-r--r--   0        0        0      699 2024-05-29 23:15:57.848149 evo_framework-2024.5.43/evo_framework/core/evo_core_foundation/IFoundation.py
+-rw-r--r--   0        0        0       63 2024-05-29 23:15:57.849413 evo_framework-2024.5.43/evo_framework/core/evo_core_key/__init__.py
+-rw-r--r--   0        0        0      893 2024-05-29 23:15:57.844661 evo_framework-2024.5.43/evo_framework/core/evo_core_key/utility/IuKey.py
+-rw-r--r--   0        0        0       63 2024-05-29 23:15:57.848179 evo_framework-2024.5.43/evo_framework/core/evo_core_log/__init__.py
+-rw-r--r--   0        0        0     2150 2024-05-29 23:15:57.848192 evo_framework-2024.5.43/evo_framework/core/evo_core_log/utility/IuLog.py
+-rw-r--r--   0        0        0     2289 2024-03-22 09:09:45.000000 evo_framework-2024.5.43/evo_framework/core/evo_core_log/utility/ULogger.py
+-rwxr-xr-x   0        0        0      146 2024-05-29 23:15:57.848259 evo_framework-2024.5.43/evo_framework/core/evo_core_setting/__init__.py
+-rw-r--r--   0        0        0     2813 2024-05-29 23:15:57.849237 evo_framework-2024.5.43/evo_framework/core/evo_core_setting/control/CSetting.py
+-rwxr-xr-x   0        0        0        0 2024-01-05 09:11:06.000000 evo_framework-2024.5.43/evo_framework/core/evo_core_setting/control/__init__.py
+-rw-r--r--   0        0        0     1201 2024-05-29 23:15:57.849250 evo_framework-2024.5.43/evo_framework/core/evo_core_setting/entity/ESetting.py
+-rw-r--r--   0        0        0        0 2024-01-05 20:57:13.000000 evo_framework-2024.5.43/evo_framework/core/evo_core_setting/entity/__init__.py
+-rw-r--r--   0        0        0       72 2024-05-29 23:15:57.848222 evo_framework-2024.5.43/evo_framework/core/evo_core_system/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-04 13:13:56.000000 evo_framework-2024.5.43/evo_framework/core/evo_core_system/control/__init__.py
+-rw-r--r--   0        0        0     6742 2024-02-12 00:08:10.000000 evo_framework-2024.5.43/evo_framework/core/evo_core_system/utility/IuSystem.py
+-rw-r--r--   0        0        0        0 2024-01-04 13:14:10.000000 evo_framework-2024.5.43/evo_framework/core/evo_core_system/utility/__init__.py
+-rw-r--r--   0        0        0        0 2021-11-12 08:43:14.000000 evo_framework-2024.5.43/evo_framework/core/evo_core_type/__init__.py
+-rwxr-xr-x   0        0        0      953 2024-04-22 18:31:06.740795 evo_framework-2024.5.43/evo_framework/core/evo_core_type/entity/EvoMap.py
+-rw-r--r--   0        0        0       66 2024-05-29 23:15:57.849211 evo_framework-2024.5.43/evo_framework/core/evo_core_yaml/__init__.py
+-rw-r--r--   0        0        0      304 2024-03-02 18:03:59.000000 evo_framework-2024.5.43/evo_framework/core/evo_core_yaml/utility/IuYaml.py
+-rwxr-xr-x   0        0        0     9395 2024-05-29 23:15:57.849264 evo_framework-2024.5.43/evo_framework/entity/EObject.py
+-rw-r--r--   0        0        0        0 2021-11-23 22:03:14.000000 evo_framework-2024.5.43/evo_framework/entity/IEObject.py
+-rw-r--r--   0        0        0        0 2021-11-23 22:02:39.000000 evo_framework-2024.5.43/evo_framework/entity/IEvo.py
+-rwxr-xr-x   0        0        0       64 2021-11-23 22:11:09.000000 evo_framework-2024.5.43/evo_framework/entity/Id.py
+-rwxr-xr-x   0        0        0       62 2021-11-23 22:13:51.000000 evo_framework-2024.5.43/evo_framework/entity/Time.py
+-rwxr-xr-x   0        0        0      181 2024-05-29 23:15:57.849324 evo_framework-2024.5.43/evo_framework/entity/__init__.py
+-rwxr-xr-x   0        0        0        0 2024-01-14 01:56:17.000000 evo_framework-2024.5.43/evo_framework/utility/__init__.py
+-rw-r--r--   0        0        0      583 2024-05-31 21:25:57.688997 evo_framework-2024.5.43/pyproject.toml
+-rw-r--r--   0        0        0     1271 1970-01-01 00:00:00.000000 evo_framework-2024.5.43/PKG-INFO
```

### Comparing `evo_framework-2024.5.42/LICENSE.txt` & `evo_framework-2024.5.43/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.42/evo_framework/__init__.py` & `evo_framework-2024.5.43/evo_framework/__init__.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.42/evo_framework/control/CObject.py` & `evo_framework-2024.5.43/evo_framework/control/CObject.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.42/evo_framework/core/evo_core_api/automation/entity.yaml` & `evo_framework-2024.5.43/evo_framework/core/evo_core_api/automation/entity.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #   BYTE
 #   BYTES
 #   BOOL [DEFAULT_VALUE]
 #   EOBJECT EOBJECT_CLASS
 #   MAP EOBJECT_CLASS
 #   ENUM ENUM_DEFAULT
 
-package: evo_core_api
+package: evo_framework.evo_framework.core.evo_core_api
 
 enum:
   EnumApiType:
     STRING
     LANGUAGE
     INT
     LONG
```

### Comparing `evo_framework-2024.5.42/evo_framework/core/evo_core_api/control/CApi.py` & `evo_framework-2024.5.43/evo_framework/core/evo_core_api/control/CApi.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.42/evo_framework/core/evo_core_api/control/CApiFlow.py` & `evo_framework-2024.5.43/evo_framework/core/evo_core_api/control/CApiFlow.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.42/evo_framework/core/evo_core_api/entity/EAction.py` & `evo_framework-2024.5.43/evo_framework/core/evo_core_api/entity/EAction.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #========================================================================================================================================
 # CyborgAI CC BY-NC-ND 4.0 Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 Internation	https://github.com/cyborg-ai-git # 
 #========================================================================================================================================
 
 from evo_framework.entity.EObject import EObject
 from evo_framework.core.evo_core_type.entity.EvoMap import EvoMap
 
-from evo_core_api.entity.EnumApiAction import EnumApiAction
+from evo import EnumApiAction
 #========================================================================================================================================
 """EAction
 
 	EAction DESCRIPTION
 	
 """
 class EAction(EObject):
```

### Comparing `evo_framework-2024.5.42/evo_framework/core/evo_core_api/entity/EActionTask.py` & `evo_framework-2024.5.43/evo_framework/core/evo_core_api/entity/EActionTask.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.42/evo_framework/core/evo_core_api/entity/EApi.py` & `evo_framework-2024.5.43/evo_framework/core/evo_core_api/entity/EApi.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.42/evo_framework/core/evo_core_api/entity/EApiConfig.py` & `evo_framework-2024.5.43/evo_framework/core/evo_core_api/entity/EApiConfig.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.42/evo_framework/core/evo_core_api/entity/EApiFile.py` & `evo_framework-2024.5.43/evo_framework/core/evo_core_api/entity/EApiFile.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.42/evo_framework/core/evo_core_api/entity/EApiText.py` & `evo_framework-2024.5.43/evo_framework/core/evo_core_api/entity/EApiText.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.42/evo_framework/core/evo_core_api/entity/ERequest.py` & `evo_framework-2024.5.43/evo_framework/core/evo_core_api/entity/ERequest.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.42/evo_framework/core/evo_core_api/entity/EResponse.py` & `evo_framework-2024.5.43/evo_framework/core/evo_core_api/entity/EResponse.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.42/evo_framework/core/evo_core_api/entity/EnumApiAction.py` & `evo_framework-2024.5.43/evo_framework/core/evo_core_api/entity/EnumApiAction.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.42/evo_framework/core/evo_core_api/entity/__init__.py` & `evo_framework-2024.5.43/evo_framework/core/evo_core_api/entity/__init__.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.42/evo_framework/core/evo_core_api/utility/IuApi.py` & `evo_framework-2024.5.43/evo_framework/core/evo_core_api/utility/IuApi.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.42/evo_framework/core/evo_core_api/utility/IuApiPb.py` & `evo_framework-2024.5.43/evo_framework/core/evo_core_api/utility/IuApiPb.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.42/evo_framework/core/evo_core_binary/utility/IuBinary.py` & `evo_framework-2024.5.43/evo_framework/core/evo_core_binary/utility/IuBinary.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.42/evo_framework/core/evo_core_binary/utility/IuBinaryAsync.py` & `evo_framework-2024.5.43/evo_framework/core/evo_core_binary/utility/IuBinaryAsync.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.42/evo_framework/core/evo_core_binary/utility/UBinary.py` & `evo_framework-2024.5.43/evo_framework/core/evo_core_binary/utility/UBinary.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.42/evo_framework/core/evo_core_boot/control/CBoot.py` & `evo_framework-2024.5.43/evo_framework/core/evo_core_boot/control/CBoot.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.42/evo_framework/core/evo_core_convert/test_evo_core_binary.py` & `evo_framework-2024.5.43/evo_framework/core/evo_core_convert/test_evo_core_binary.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.42/evo_framework/core/evo_core_convert/utility/IuConvert.py` & `evo_framework-2024.5.43/evo_framework/core/evo_core_convert/utility/IuConvert.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.42/evo_framework/core/evo_core_crypto/utility/IuCryptChacha.py` & `evo_framework-2024.5.43/evo_framework/core/evo_core_crypto/utility/IuCryptChacha.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.42/evo_framework/core/evo_core_crypto/utility/IuCryptEC.py` & `evo_framework-2024.5.43/evo_framework/core/evo_core_crypto/utility/IuCryptEC.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.42/evo_framework/core/evo_core_crypto/utility/IuCryptHash.py` & `evo_framework-2024.5.43/evo_framework/core/evo_core_crypto/utility/IuCryptHash.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.42/evo_framework/core/evo_core_file/entity/EFileChunk.py` & `evo_framework-2024.5.43/evo_framework/core/evo_core_file/entity/EFileChunk.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.42/evo_framework/core/evo_core_foundation/IFoundation.py` & `evo_framework-2024.5.43/evo_framework/core/evo_core_foundation/IFoundation.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.42/evo_framework/core/evo_core_key/utility/IuKey.py` & `evo_framework-2024.5.43/evo_framework/core/evo_core_key/utility/IuKey.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.42/evo_framework/core/evo_core_log/utility/IuLog.py` & `evo_framework-2024.5.43/evo_framework/core/evo_core_log/utility/IuLog.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.42/evo_framework/core/evo_core_log/utility/ULogger.py` & `evo_framework-2024.5.43/evo_framework/core/evo_core_log/utility/ULogger.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.42/evo_framework/core/evo_core_setting/control/CSetting.py` & `evo_framework-2024.5.43/evo_framework/core/evo_core_setting/control/CSetting.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.42/evo_framework/core/evo_core_setting/entity/ESetting.py` & `evo_framework-2024.5.43/evo_framework/core/evo_core_setting/entity/ESetting.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.42/evo_framework/core/evo_core_system/utility/IuSystem.py` & `evo_framework-2024.5.43/evo_framework/core/evo_core_system/utility/IuSystem.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.42/evo_framework/core/evo_core_type/entity/EvoMap.py` & `evo_framework-2024.5.43/evo_framework/core/evo_core_type/entity/EvoMap.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.42/evo_framework/entity/EObject.py` & `evo_framework-2024.5.43/evo_framework/entity/EObject.py`

 * *Files identical despite different names*

### Comparing `evo_framework-2024.5.42/pyproject.toml` & `evo_framework-2024.5.43/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "evo-framework"
-version = "2024.5.42"
+version = "2024.5.43"
 description = "evo framework python"
 authors = ["cyborg-ai-git <129898917+cyborg-ai-git@users.noreply.github.com>"]
 readme = "README.md"
 #packages = [{include = "evo"}]
 license = "CC BY-NC-ND 4.0"
 include = ["LICENSE.txt"]
```

### Comparing `evo_framework-2024.5.42/PKG-INFO` & `evo_framework-2024.5.43/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evo-framework
-Version: 2024.5.42
+Version: 2024.5.43
 Summary: evo framework python
 License: CC BY-NC-ND 4.0
 Author: cyborg-ai-git
 Author-email: 129898917+cyborg-ai-git@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

