# Comparing `tmp/cubecoders_amp_api_wrapper-0.0.42b0.tar.gz` & `tmp/cubecoders_amp_api_wrapper-0.1.0.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubecoders_amp_api_wrapper-0.0.42b0.tar", last modified: Wed May  8 21:50:59 2024, max compression
+gzip compressed data, was "cubecoders_amp_api_wrapper-0.1.0.post0.tar", last modified: Fri May 31 06:10:08 2024, max compression
```

## Comparing `cubecoders_amp_api_wrapper-0.0.42b0.tar` & `cubecoders_amp_api_wrapper-0.1.0.post0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)        0 2024-05-08 21:50:59.077004 cubecoders_amp_api_wrapper-0.0.42b0/
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     8872 2024-05-08 21:50:56.000000 cubecoders_amp_api_wrapper-0.0.42b0/CHANGELOG.md
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    35149 2024-04-28 19:14:36.000000 cubecoders_amp_api_wrapper-0.0.42b0/LICENSE
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)       76 2024-04-28 19:14:36.000000 cubecoders_amp_api_wrapper-0.0.42b0/MANIFEST.in
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     4778 2024-05-08 21:50:59.072454 cubecoders_amp_api_wrapper-0.0.42b0/PKG-INFO
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     3481 2024-05-08 15:52:03.000000 cubecoders_amp_api_wrapper-0.0.42b0/README.md
-drwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)        0 2024-05-08 21:50:58.626006 cubecoders_amp_api_wrapper-0.0.42b0/ampapi/
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     1575 2024-05-08 21:48:22.000000 cubecoders_amp_api_wrapper-0.0.42b0/ampapi/__init__.py
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     2501 2024-05-08 21:39:59.000000 cubecoders_amp_api_wrapper-0.0.42b0/ampapi/ads.py
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    76652 2024-05-08 21:43:40.000000 cubecoders_amp_api_wrapper-0.0.42b0/ampapi/adsmodule.py
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    15110 2024-05-08 21:36:15.000000 cubecoders_amp_api_wrapper-0.0.42b0/ampapi/base.py
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     1719 2024-05-08 21:38:55.000000 cubecoders_amp_api_wrapper-0.0.42b0/ampapi/bridge.py
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    75470 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.0.42b0/ampapi/core.py
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)      258 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.0.42b0/ampapi/emailsender.py
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     8024 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.0.42b0/ampapi/filebackup.py
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    22707 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.0.42b0/ampapi/filemanager.py
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     2836 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.0.42b0/ampapi/instance.py
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    19680 2024-05-08 16:26:18.000000 cubecoders_amp_api_wrapper-0.0.42b0/ampapi/minecraft.py
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    34985 2024-05-08 16:35:09.000000 cubecoders_amp_api_wrapper-0.0.42b0/ampapi/types.py
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     3570 2024-05-08 16:26:31.000000 cubecoders_amp_api_wrapper-0.0.42b0/ampapi/util.py
-drwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)        0 2024-05-08 21:50:59.038004 cubecoders_amp_api_wrapper-0.0.42b0/cubecoders_amp_api_wrapper.egg-info/
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     4778 2024-05-08 21:50:57.000000 cubecoders_amp_api_wrapper-0.0.42b0/cubecoders_amp_api_wrapper.egg-info/PKG-INFO
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)      696 2024-05-08 21:50:57.000000 cubecoders_amp_api_wrapper-0.0.42b0/cubecoders_amp_api_wrapper.egg-info/SOURCES.txt
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)        1 2024-05-08 21:50:57.000000 cubecoders_amp_api_wrapper-0.0.42b0/cubecoders_amp_api_wrapper.egg-info/dependency_links.txt
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)       59 2024-05-08 21:50:57.000000 cubecoders_amp_api_wrapper-0.0.42b0/cubecoders_amp_api_wrapper.egg-info/requires.txt
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)        7 2024-05-08 21:50:57.000000 cubecoders_amp_api_wrapper-0.0.42b0/cubecoders_amp_api_wrapper.egg-info/top_level.txt
-drwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)        0 2024-05-08 21:50:59.010004 cubecoders_amp_api_wrapper-0.0.42b0/docs/
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    44032 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.0.42b0/docs/ADS_api_spec.md
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    29384 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.0.42b0/docs/Minecraft_api_spec.md
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    10444 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.0.42b0/docs/permission_nodes.md
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    10444 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.0.42b0/docs/permission_nodes.txt
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     4691 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.0.42b0/docs/setting_nodes.md
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     4649 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.0.42b0/docs/setting_nodes.txt
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)       59 2024-05-08 21:36:33.000000 cubecoders_amp_api_wrapper-0.0.42b0/requirements.txt
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)       38 2024-05-08 21:50:59.117169 cubecoders_amp_api_wrapper-0.0.42b0/setup.cfg
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     2134 2024-05-08 21:49:44.000000 cubecoders_amp_api_wrapper-0.0.42b0/setup.py
+drwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)        0 2024-05-31 06:10:06.172690 cubecoders_amp_api_wrapper-0.1.0.post0/
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    10304 2024-05-31 06:10:03.000000 cubecoders_amp_api_wrapper-0.1.0.post0/CHANGELOG.md
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    35149 2024-04-28 19:14:36.000000 cubecoders_amp_api_wrapper-0.1.0.post0/LICENSE
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)       76 2024-04-28 19:14:36.000000 cubecoders_amp_api_wrapper-0.1.0.post0/MANIFEST.in
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     4793 2024-05-31 06:10:06.166507 cubecoders_amp_api_wrapper-0.1.0.post0/PKG-INFO
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     3481 2024-05-08 15:52:03.000000 cubecoders_amp_api_wrapper-0.1.0.post0/README.md
+drwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)        0 2024-05-31 06:10:05.570693 cubecoders_amp_api_wrapper-0.1.0.post0/ampapi/
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     1576 2024-05-31 06:08:28.000000 cubecoders_amp_api_wrapper-0.1.0.post0/ampapi/__init__.py
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     3219 2024-05-10 01:40:17.000000 cubecoders_amp_api_wrapper-0.1.0.post0/ampapi/ads.py
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    76650 2024-05-31 01:56:27.000000 cubecoders_amp_api_wrapper-0.1.0.post0/ampapi/adsmodule.py
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    15128 2024-05-10 01:30:45.000000 cubecoders_amp_api_wrapper-0.1.0.post0/ampapi/base.py
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     1719 2024-05-08 21:38:55.000000 cubecoders_amp_api_wrapper-0.1.0.post0/ampapi/bridge.py
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    75481 2024-05-31 05:32:55.000000 cubecoders_amp_api_wrapper-0.1.0.post0/ampapi/core.py
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)      258 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.1.0.post0/ampapi/emailsender.py
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     8024 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.1.0.post0/ampapi/filebackup.py
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    22707 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.1.0.post0/ampapi/filemanager.py
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     2836 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.1.0.post0/ampapi/instance.py
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    19680 2024-05-08 16:26:18.000000 cubecoders_amp_api_wrapper-0.1.0.post0/ampapi/minecraft.py
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    35216 2024-05-31 05:42:23.000000 cubecoders_amp_api_wrapper-0.1.0.post0/ampapi/types.py
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     4845 2024-05-31 05:40:47.000000 cubecoders_amp_api_wrapper-0.1.0.post0/ampapi/util.py
+drwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)        0 2024-05-31 06:10:06.134691 cubecoders_amp_api_wrapper-0.1.0.post0/cubecoders_amp_api_wrapper.egg-info/
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     4793 2024-05-31 06:10:04.000000 cubecoders_amp_api_wrapper-0.1.0.post0/cubecoders_amp_api_wrapper.egg-info/PKG-INFO
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)      696 2024-05-31 06:10:04.000000 cubecoders_amp_api_wrapper-0.1.0.post0/cubecoders_amp_api_wrapper.egg-info/SOURCES.txt
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)        1 2024-05-31 06:10:04.000000 cubecoders_amp_api_wrapper-0.1.0.post0/cubecoders_amp_api_wrapper.egg-info/dependency_links.txt
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)       59 2024-05-31 06:10:04.000000 cubecoders_amp_api_wrapper-0.1.0.post0/cubecoders_amp_api_wrapper.egg-info/requires.txt
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)        7 2024-05-31 06:10:04.000000 cubecoders_amp_api_wrapper-0.1.0.post0/cubecoders_amp_api_wrapper.egg-info/top_level.txt
+drwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)        0 2024-05-31 06:10:06.094691 cubecoders_amp_api_wrapper-0.1.0.post0/docs/
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    43567 2024-05-31 05:40:12.000000 cubecoders_amp_api_wrapper-0.1.0.post0/docs/ADS_api_spec.md
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    29384 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.1.0.post0/docs/Minecraft_api_spec.md
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    10444 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.1.0.post0/docs/permission_nodes.md
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    10444 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.1.0.post0/docs/permission_nodes.txt
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     4691 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.1.0.post0/docs/setting_nodes.md
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     4649 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.1.0.post0/docs/setting_nodes.txt
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)       59 2024-05-08 21:36:33.000000 cubecoders_amp_api_wrapper-0.1.0.post0/requirements.txt
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)       38 2024-05-31 06:10:06.208382 cubecoders_amp_api_wrapper-0.1.0.post0/setup.cfg
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     2180 2024-05-31 06:02:58.000000 cubecoders_amp_api_wrapper-0.1.0.post0/setup.py
```

### Comparing `cubecoders_amp_api_wrapper-0.0.42b0/CHANGELOG.md` & `cubecoders_amp_api_wrapper-0.1.0.post0/CHANGELOG.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,42 @@
+## Version - 0.1.0r - [ac16314](https://github.com/k8thekat/AMPAPI_Python/commit/ac16314)
+#### __init__.py
+- Version bump to `0.1.0r`
+- Changed `releaseLevel` to "release"
+- Version bump `0.1.0r`
+
+#### setup.py
+- Changed classifiers from "Alpha" to "Production/Stable"
+
+#### ads.py
+- Added `_AvailableInstances` as an attribute to better handle population of `AvailableInstances` attribute.
+- Added `_Controller_exists` as an attribute to catch attribute errors for the Controller dataclass that ADSInstance inherits from when accessed prior to class creation/population.
+
+#### adsmodule.py
+- Updated `detatch_target` to `detach_target` to align with the `v2.5.0.12` AMP Update.
+- Updated the API endpoint for `detach_target` to align with the `v2.5.0.12` AMP Update.
+
+#### base.py
+- Added parameter declaration to the `fields()` method.
+
+#### core.py
+- Formatting change on one line.
+- Updated return type for `get_api_spec()`
+
+#### types.py
+- Added `to_str()` method to the `AMP_Version()` dataclass to be used for future plans.
+- Removed an un-needed `# type:ignore`
+
+#### util.py
+- Formatting changes on multiple lines.
+- Re-wrote logic for `parse_get_api_spec()`
+	- Added the `@classmethod` decorator for usage prior to `APIUtil` class generation.
+	- Added Instance Type, Version and Build strings to the output document to better compare API changes between versions.
+	-- Improved formatting of data output from API parsing.
+
 ## Version - 0.0.42b - [2bf7996](https://github.com/k8thekat/AMPAPI_Python/commit/2bf7996)
 #### Changelog.md
 - Version info from `0.0.41b`
 
 #### __init__.py
 - Version bump `0.0.42b`
```

### Comparing `cubecoders_amp_api_wrapper-0.0.42b0/LICENSE` & `cubecoders_amp_api_wrapper-0.1.0.post0/LICENSE`

 * *Files identical despite different names*

### Comparing `cubecoders_amp_api_wrapper-0.0.42b0/PKG-INFO` & `cubecoders_amp_api_wrapper-0.1.0.post0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: cubecoders_amp_api_wrapper
-Version: 0.0.42b0
+Version: 0.1.0.post0
 Summary: A python wrapper for the AMP API by CubeCoders
 Home-page: https://github.com/k8thekat/AMPAPI_Python
 Author: Katelynn Cadwallader
 Author-email: Cadwalladerkatelynn+AMPAPI@gmail.com
 License: GNU
 Project-URL: GitHub, https://github.com/k8thekat/AMPAPI_Python
 Project-URL: Changelog, https://github.com/k8thekat/AMPAPI_Python/blob/master/CHANGELOG.md
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `cubecoders_amp_api_wrapper-0.0.42b0/README.md` & `cubecoders_amp_api_wrapper-0.1.0.post0/README.md`

 * *Files identical despite different names*

### Comparing `cubecoders_amp_api_wrapper-0.0.42b0/ampapi/__init__.py` & `cubecoders_amp_api_wrapper-0.1.0.post0/ampapi/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,15 +19,15 @@
    02110-1301, USA. 
 '''
 from __future__ import annotations
 
 __title__ = "CubeCoders AMP API"
 __author__ = "k8thekat"
 __license__ = "GNU"
-__version__ = "0.0.42b"
+__version__ = "0.1.0r"
 __credits__ = "AMP by CubeCoders and associates."
 
 from typing import Literal, NamedTuple
 
 from .ads import *
 from .adsmodule import *
 from .bridge import *
@@ -44,10 +44,10 @@
 class VersionInfo(NamedTuple):
     Major: int
     Minor: int
     Revision: int
     releaseLevel: Literal["alpha", "beta", "release"]
 
 
-version_info: VersionInfo = VersionInfo(Major=0, Minor=0, Revision=33, releaseLevel="alpha")
+version_info: VersionInfo = VersionInfo(Major=0, Minor=1, Revision=00, releaseLevel="release")
 
 del NamedTuple, Literal, VersionInfo
```

### Comparing `cubecoders_amp_api_wrapper-0.0.42b0/ampapi/ads.py` & `cubecoders_amp_api_wrapper-0.1.0.post0/ampapi/ads.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from typing import TYPE_CHECKING, Self, Union
+from dataclasses import fields
+from typing import Any, Self, Union
 
 from .adsmodule import ADSModule
 from .core import Core
 from .emailsender import EmailSenderPlugin
 from .filebackup import LocalFileBackupPlugin
 from .filemanager import FileManagerPlugin
 from .instance import AMPInstance, AMPMinecraftInstance
@@ -14,22 +15,24 @@
 class ADSInstance(ADSModule, Core, EmailSenderPlugin, LocalFileBackupPlugin, FileManagerPlugin, Controller):
     """
     The ADS class is the top most level of Instances inside of AMP, may also be referred to as the "Controller".
 
     """
 
     Module: str = "ADS"
+    _AvailableInstances: list[AMPInstance | AMPMinecraftInstance] = []
+    _Controller_exists: bool = False
 
     @property
     def AvailableInstances(self) -> list[AMPInstance | AMPMinecraftInstance]:
         return self._AvailableInstances
 
     @AvailableInstances.setter
     def AvailableInstances(self, instances: list[Instance]) -> None:
-        self._AvailableInstances: list[AMPInstance] = []
+        self._AvailableInstances = []
         if isinstance(instances, list) and len(instances) > 0:
             for i in range(0, len(instances)):
                 if instances[i].Module == "ADS":
                     continue
 
                 elif instances[i].Module == "Minecraft":
                     self._AvailableInstances.append(AMPMinecraftInstance(data=instances[i]))
@@ -37,29 +40,36 @@
                 else:
                     self._AvailableInstances.append(AMPInstance(data=instances[i]))
 
     def __init__(self) -> None:
         self._logger.debug(msg=f"DEBUG {type(self).__name__} __init__")
         super().__init__()
 
+    def __getattr__(self, name: str) -> AttributeError | Any:
+        if name in [field.name for field in fields(class_or_instance=Controller)] and self._Controller_exists == False:
+            raise AttributeError(f"'{type(self).__name__}' object has no attribute '{name}' | You must call get_instances() with 'format_data=True' to update this object.")
+        return self.__getattribute__(name)
+
     async def get_instances(self, format_data: Union[bool, None] = None) -> list[Controller | Self]:
         """
-        Returns a list of all Instances on the AMP Panel and updates our self object.
+        Returns a list of all Controller Instances on the AMP Panel.\n
+        `format_data == True` -- Will update our current object calling this method with the Instances belonging to it, else any Controller attributes will raise an AttributeError.
+
         `**ADSInstance Only**`
 
         Args:
             format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
 
         Returns:
             list[Self] | str | bool | int | None: On success returns a list of Self dataclasses. 
 
         """
-
         ads_list: list[ADSInstance | Controller] = []
         result: list[Controller] = await super().get_instances(format_data=format_data)
         if isinstance(result, list) and isinstance(result[0], Controller):
+            self._Controller_exists = True
             self.parse_data(data=result[0])  # Need to update our self object.
             for i in range(1, len(result)):
                 ads_list.append(ADSInstance().parse_data(data=result[i]))
             return ads_list
         else:
             return result
```

### Comparing `cubecoders_amp_api_wrapper-0.0.42b0/ampapi/adsmodule.py` & `cubecoders_amp_api_wrapper-0.1.0.post0/ampapi/adsmodule.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 class ADSModule(Base):
     """
     Contains the base functions for any `/API/ADSModule/` AMP API endpoints.
 
     """
     # ADSModule.AddDatastore:({'Parameters': [{'Name': 'newDatastore', 'TypeName': 'InstanceDatastore', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
+
     async def add_datastore(self, new_datastore: InstanceDatastore, format_data: Union[bool, None] = None) -> ActionResult:
         """
         Add a new datastore.
         **Requires ADS**
 
         Args:
             new_datastore (InstanceDatastore): InstanceDatastore dataclass. See `types.py -> InstanceDatastore`
@@ -479,15 +480,14 @@
         # new_email (str | None, optional): If 'NewUsername' is specified and the user doesn't already exist, the email address that will be assigned to this user. `Defaults to None.`
         # required_tags (list[str] | None, optional): If specified, AMP will only deploy this template to targets that have every single 'tag' specified in their target configuration. You can adjust this via the controller by clicking 'Edit' on the target settings. `Defaults to None.`
         # tag (str | None, optional): Unrelated to RequiredTags. This is to uniquely identify this instance to your own systems. It may be something like an order ID or service ID so you can find the associated instance again at a later time. If 'UseTagAsInstanceName' is enabled, then this will also be used as the instance name for the created instance - but it must be unique. `Defaults to None.`
         # friendly_name (str | None, optional): A friendly name for this instance. If left blank, AMP will generate one for you. `Defaults to None.`
         # secret (str | None, optional): Must be a non-empty strong in order to get a callback on deployment state change. This secret will be passed back to you in the callback so you can verify the request. `Defaults to None.`
         # post_create: 0: Do nothing, 1: Start instance only, 2: Start instance and update application, 3: Full application startup, 16: Every time. `Default to 0.`
         # extra_provision_settings (dict[str, str] | None, optional): A dictionary of setting nodes and values to create the new instance with. Identical in function to the provisioning arguments in the template itself. `Defaults to None.`
-
         """
         Deploy a Instance template.
         **Requires ADS**
 
         Args:
             template (Template | None, optional): The Template to deploy. See `types.py -> Template`.
             format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
@@ -805,15 +805,15 @@
             "instanceId": instance_id
         }
         await self._connect()
         result = await self._call_api(api='ADSModule/AttachADS', parameters=parameters, format_data=format_data, format=ActionResult)
         return result
 
     # ADSModule.DetatchTarget:({'Parameters': [{'Name': 'Id', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
-    async def detatch_target(self, instance_id: str, format_data: Union[bool, None] = None) -> ActionResult:
+    async def detach_target(self, instance_id: str, format_data: Union[bool, None] = None) -> ActionResult:
         """
         De-tach an Instance from the ADS.
 
         Args:
             instance_id (str): Instance ID.
             format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
 
@@ -825,15 +825,15 @@
         if self.Module != "ADS":
             raise RuntimeError(self.ADS_ONLY)
 
         parameters = {
             "id": instance_id
         }
         await self._connect()
-        result = await self._call_api(api='ADSModule/DetatchTarget', parameters=parameters, format_data=format_data, format=ActionResult)
+        result = await self._call_api(api='ADSModule/DetachTarget', parameters=parameters, format_data=format_data, format=ActionResult)
         return result
 
     # ADSModule.UpdateTargetInfo:({'Parameters': [{'Name': 'Id', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'FriendlyName', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Url', 'TypeName': 'Uri', 'Description': '', 'Optional': False}, {'Name': 'Description', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Tags', 'TypeName': 'List<String>', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True})
     async def update_target_info(self, instance_id: str, friendly_name: str, url: str, description: str, tags: list[str], format_data: Union[bool, None] = None) -> ActionResult:
         """
         Update a target Instance information.
```

### Comparing `cubecoders_amp_api_wrapper-0.0.42b0/ampapi/base.py` & `cubecoders_amp_api_wrapper-0.1.0.post0/ampapi/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,15 +112,15 @@
 
         Args:
             data (Controller | Instance): The Controller or Instance dataclass.
 
         Returns:
             Self: Returns the class that called this function.
         """
-        for field in fields(data):
+        for field in fields(class_or_instance=data):
             # This is to deal with improperly cased InstanceId.
             if field.name == "InstanceId":
                 setattr(self, "InstanceID", getattr(data, field.name))
                 continue
             setattr(self, field.name, getattr(data, field.name))
         return self
```

### Comparing `cubecoders_amp_api_wrapper-0.0.42b0/ampapi/bridge.py` & `cubecoders_amp_api_wrapper-0.1.0.post0/ampapi/bridge.py`

 * *Files identical despite different names*

### Comparing `cubecoders_amp_api_wrapper-0.0.42b0/ampapi/core.py` & `cubecoders_amp_api_wrapper-0.1.0.post0/ampapi/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 
 class Core(Base):
     """
     Contains the base functions for any `/API/Core/` AMP API endpoints.
 
     """
+
     async def login(self, amp_user: str, amp_password: str, token: str = "", rememberME: bool = False, format_data: Union[bool, None] = None) -> LoginResults:
         """
         AMP API login function. \n
 
         Args:
             amp_user (str): The username for logging into the AMP Panel
             amp_password (str): The password for logging into the AMP Panel
@@ -43,15 +44,15 @@
         Returns:
             None
         """
         await self._connect()
         await self._call_api(api='Core/Logout')
         return
 
-    async def get_api_spec(self) -> dict:
+    async def get_api_spec(self) -> dict[Any, Any]:
         """
         Get's all the API specs for the ADS or Instance.
          - See `docs/api_spec.md`
 
         Returns:
             dict: A dictionary containing all of the API specs, their parameters and return types for the ADS or Instance.
         """
```

### Comparing `cubecoders_amp_api_wrapper-0.0.42b0/ampapi/filebackup.py` & `cubecoders_amp_api_wrapper-0.1.0.post0/ampapi/filebackup.py`

 * *Files identical despite different names*

### Comparing `cubecoders_amp_api_wrapper-0.0.42b0/ampapi/filemanager.py` & `cubecoders_amp_api_wrapper-0.1.0.post0/ampapi/filemanager.py`

 * *Files identical despite different names*

### Comparing `cubecoders_amp_api_wrapper-0.0.42b0/ampapi/instance.py` & `cubecoders_amp_api_wrapper-0.1.0.post0/ampapi/instance.py`

 * *Files identical despite different names*

### Comparing `cubecoders_amp_api_wrapper-0.0.42b0/ampapi/minecraft.py` & `cubecoders_amp_api_wrapper-0.1.0.post0/ampapi/minecraft.py`

 * *Files identical despite different names*

### Comparing `cubecoders_amp_api_wrapper-0.0.42b0/ampapi/types.py` & `cubecoders_amp_api_wrapper-0.1.0.post0/ampapi/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,26 +166,30 @@
 
     Major: int
     Minor: int
     Revision: int
     MinorRevision: int
     Build: Union[int, None] = None
 
+    def to_str(self) -> str:
+        "Returns a string representation of the AMP_Version dataclass as `Major.Minor.Revision.MinorRevision | Build`."
+        return f"{self.Major}.{self.Minor}.{self.Revision}.{self.MinorRevision} | {self.Build}"
+
 
 @dataclass()
 class UpdateInfo():
     """
     Represents AMP API call `Core/GetUpdateInfo`.
 
     """
 
     UpdateAvailable: bool
     ReleaseNotesURL: str
     Build: str
-    Version: str  # type:ignore
+    Version: str
     ToolsVersion: None | str = None
     PatchOnly: None | bool = None
 
 
 @dataclass()
 class Metrics_Data():
     """
```

### Comparing `cubecoders_amp_api_wrapper-0.0.42b0/ampapi/util.py` & `cubecoders_amp_api_wrapper-0.1.0.post0/ampapi/util.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 from __future__ import annotations
 
+from io import TextIOWrapper
 from pathlib import Path
-from typing import Any
+from typing import Any, Union
 
+from ampapi.types import UpdateInfo
+
+from .ads import ADSInstance
 from .core import Core
+from .instance import AMPInstance, AMPMinecraftInstance
 
 
 class APIUtil():
     """
     AMP API util functions to parse specific API calls for specific Data.
     """
 
     async def get_node_spec(self, amp: Core) -> str | dict[str, Any] | list | bool | int | None:
         """
         Creates a `setting_nodes.txt` in the script directory with nodes from api `Core/GetSettingSpec`
 
         Args:
             amp (Core): API_Core class object signed in.
 
-        See -> `amp/util/setting_nodes.txt` 
+        See -> `amp/util/setting_nodes.txt`
 
         """
         res = await amp.get_settings_spec()
         dir = Path(__file__).parent.joinpath("../docs/setting_nodes.md")
         mode = "x"
         if dir.exists():
             mode = "w"
@@ -41,15 +46,15 @@
     async def get_permission_nodes(self, amp: Core) -> str | dict[str, Any] | list | bool | int | None:
         """
         Creates a `permission_nodes.txt` in the script directory with nodes from api `Core/GetPermissionsSpec`
 
         Args:
             amp (Core): API_Core class object signed in.
 
-        See -> `amp/util/permission_nodes.txt`  
+        See -> `amp/util/permission_nodes.txt`
         """
         res = await amp.get_permissions_spec()
         if isinstance(res, list):
             self.node_scrape(text=res)
         else:
             raise ValueError(f"Error - invalid data type returned. {type(res)}")
 
@@ -75,34 +80,59 @@
         for index in text:
             if "Node" in index:
                 file.write(f'{index["Node"]} \n')
             if "Children" in index:
                 self.node_scrape(text=index["Children"], file=file)
         file.close()
 
-    async def parse_get_api_spec(self, instance_type: str, data: dict) -> None | str | dict[str, Any] | list | bool | int | None:
+    @classmethod
+    async def parse_get_api_spec(cls, instance: Union[Core, ADSInstance, AMPInstance, AMPMinecraftInstance]) -> None:
         """
         Creates a `api_spec.txt` in the script directory with nodes from api `Core/GetAPISpec`
         #TODO - Improve formatting of the Markdown file.
         Args:
-            amp (Core): API_Core class object signed in.
+            instance(str): The API Class 
 
-        See -> `../docs/api_spec.md` 
+        See -> `../docs/api_spec.md`
         """
-        # res = await amp.get_api_spec()
-        dir = Path(__file__).parent.joinpath(f"../docs/{instance_type}_api_spec.md")
+        data: dict[Any, Any] = await instance.get_api_spec()
+        platform_info: UpdateInfo = await instance.get_update_info()
+        if not isinstance(data, dict):
+            return None
+
+        if isinstance(instance, Core):
+            instance_type: str = "Core"
+
+        if isinstance(instance, (ADSInstance, AMPInstance, AMPMinecraftInstance)):
+            instance_type = instance.Module
+
+        dir: Path = Path(__file__).parent.joinpath(f"../docs/{instance_type}_api_spec.md")
+        parents: list = []
         mode = "x"
         if dir.exists():
             mode = "w"
-        file = open(dir, mode)
+        file: TextIOWrapper = open(file=dir, mode=mode)
 
-        if not isinstance(data, dict):
-            return None
-        else:
-            for parent, parent_value in data.items():
-                if isinstance(parent_value, dict):
-                    for child, child_value in parent_value.items():
-                        file.write(f"{parent}.{child}:({child_value}) \n")
-                else:
-                    file.write(f"{parent}({parent_value}) \n")
+        file.write(f"INSTANCE TYPE: {instance_type}\n")
+        file.write(f"VERSION: {platform_info.Version}\n")
+        file.write(f"BUILD: {platform_info.Build}\n\n")
+        for parent, parent_value in data.items():
+            if parent not in parents:
+                parents.append(parent)
+                file.write("____________________________________________________\n")
+                file.write(f"{parent}:\n")
+            if isinstance(parent_value, dict):
+                for child, child_value in parent_value.items():
+                    file.write(f"\t{child}:\n")
+                    if isinstance(child_value, dict):
+                        for key, value in child_value.items():
+                            if key == "Parameters":
+                                file.write(f"\t\t{key}:\n")
+                                for entry in value:
+                                    file.write(f"\t\t\t{entry}\n")
+                            else:
+                                file.write(f"\t\t{key}: {value}\n")
+
+                    else:
+                        file.write(f"\t\t({child_value})\n")
 
         file.close()
```

### Comparing `cubecoders_amp_api_wrapper-0.0.42b0/cubecoders_amp_api_wrapper.egg-info/PKG-INFO` & `cubecoders_amp_api_wrapper-0.1.0.post0/cubecoders_amp_api_wrapper.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: cubecoders_amp_api_wrapper
-Version: 0.0.42b0
+Version: 0.1.0.post0
 Summary: A python wrapper for the AMP API by CubeCoders
 Home-page: https://github.com/k8thekat/AMPAPI_Python
 Author: Katelynn Cadwallader
 Author-email: Cadwalladerkatelynn+AMPAPI@gmail.com
 License: GNU
 Project-URL: GitHub, https://github.com/k8thekat/AMPAPI_Python
 Project-URL: Changelog, https://github.com/k8thekat/AMPAPI_Python/blob/master/CHANGELOG.md
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `cubecoders_amp_api_wrapper-0.0.42b0/cubecoders_amp_api_wrapper.egg-info/SOURCES.txt` & `cubecoders_amp_api_wrapper-0.1.0.post0/cubecoders_amp_api_wrapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cubecoders_amp_api_wrapper-0.0.42b0/docs/ADS_api_spec.md` & `cubecoders_amp_api_wrapper-0.1.0.post0/docs/Minecraft_api_spec.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,67 +1,30 @@
-ADSModule.AddDatastore:({'Parameters': [{'Name': 'newDatastore', 'TypeName': 'InstanceDatastore', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-ADSModule.DeleteDatastore:({'Parameters': [{'Name': 'id', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-ADSModule.UpdateDatastore:({'Parameters': [{'Name': 'updatedDatastore', 'TypeName': 'InstanceDatastore', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-ADSModule.GetDatastores:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True}) 
-ADSModule.RequestDatastoreSizeCalculation:({'Parameters': [{'Name': 'datastoreId', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'RunningTask', 'IsComplexType': True}) 
-ADSModule.GetDatastore:({'Parameters': [{'Name': 'id', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'JObject', 'IsComplexType': True}) 
-ADSModule.RepairDatastore:({'Parameters': [{'Name': 'id', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'RunningTask', 'IsComplexType': True}) 
-ADSModule.GetDatastoreInstances:({'Parameters': [{'Name': 'datastoreId', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True}) 
-ADSModule.MoveInstanceDatastore:({'Parameters': [{'Name': 'instanceId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'datastoreId', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'RunningTask', 'IsComplexType': True}) 
-ADSModule.GetDeploymentTemplates:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True}) 
-ADSModule.CreateDeploymentTemplate:({'Parameters': [{'Name': 'Name', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-ADSModule.UpdateDeploymentTemplate:({'Parameters': [{'Name': 'templateToUpdate', 'TypeName': 'DeploymentTemplate', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-ADSModule.DeleteDeploymentTemplate:({'Parameters': [{'Name': 'Id', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-ADSModule.CloneTemplate:({'Parameters': [{'Name': 'Id', 'TypeName': 'Int32', 'Description': '', 'Optional': False}, {'Name': 'NewName', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-ADSModule.ApplyTemplate:({'Description': "Overlays an existing template on an existing instance. Used to perform package reconfigurations. Do not use this to 'transform' an existing application into another. The instance should be deleted and re-created in that situation.", 'Returns': '', 'Parameters': [{'Name': 'InstanceID', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'TemplateID', 'TypeName': 'Int32', 'Description': '', 'Optional': False}, {'Name': 'NewFriendlyName', 'TypeName': 'String', 'Description': '', 'Optional': True}, {'Name': 'Secret', 'TypeName': 'String', 'Description': '', 'Optional': True}, {'Name': 'RestartIfPreviouslyRunning', 'TypeName': 'Boolean', 'Description': '', 'Optional': True}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-ADSModule.DeployTemplate:({'Parameters': [{'Name': 'TemplateID', 'TypeName': 'Int32', 'Description': 'The ID of the template to be deployed, as per the Template Management UI in AMP itself.', 'Optional': False}, {'Name': 'NewUsername', 'TypeName': 'String', 'Description': 'If specified, AMP will create a new user with this name for this instance. Must be unique. If this user already exists, this will be ignored but the new instance will be assigned to this user.', 'Optional': True}, {'Name': 'NewPassword', 'TypeName': 'String', 'Description': "If 'NewUsername' is specified and the user doesn't already exist, the password that will be assigned to this user.", 'Optional': True}, {'Name': 'NewEmail', 'TypeName': 'String', 'Description': "If 'NewUsername' is specified and the user doesn't already exist, the email address that will be assigned to this user.", 'Optional': True}, {'Name': 'RequiredTags', 'TypeName': 'List<String>', 'Description': "If specified, AMP will only deploy this template to targets that have every single 'tag' specified in their target configuration. You can adjust this via the controller by clicking 'Edit' on the target settings.", 'Optional': True}, {'Name': 'Tag', 'TypeName': 'String', 'Description': "Unrelated to RequiredTags. This is to uniquely identify this instance to your own systems. It may be something like an order ID or service ID so you can find the associated instance again at a later time. If 'UseTagAsInstanceName' is enabled, then this will also be used as the instance name for the created instance - but it must be unique.", 'Optional': True}, {'Name': 'FriendlyName', 'TypeName': 'String', 'Description': 'A friendly name for this instance. If left blank, AMP will generate one for you.', 'Optional': True}, {'Name': 'Secret', 'TypeName': 'String', 'Description': 'Must be a non-empty strong in order to get a callback on deployment state change. This secret will be passed back to you in the callback so you can verify the request.', 'Optional': True}, {'Name': 'PostCreate', 'TypeName': 'PostCreateActions', 'Description': '0: Do nothing, 1: Start instance only, 2: Start instance and update application, 3: Full application startup.', 'Optional': True, 'ParamEnumValues': {'DoNothing': 0, 'StartInstance': 1, 'StartAndUpdate': 2, 'FullStartup': 3, 'EveryTime': 16}}, {'Name': 'ExtraProvisionSettings', 'TypeName': 'Dictionary<String, String>', 'Description': 'A dictionary of setting nodes and values to create the new instance with. Identical in function to the provisioning arguments in the template itself.', 'Optional': True}], 'ReturnTypeName': 'RunningTask', 'IsComplexType': True}) 
-ADSModule.GetTargetInfo:({'Parameters': [], 'ReturnTypeName': 'JObject', 'IsComplexType': True}) 
-ADSModule.GetSupportedApplications:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True}) 
-ADSModule.RefreshAppCache:({'Parameters': [], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
-ADSModule.RefreshRemoteConfigStores:({'Parameters': [{'Name': 'force', 'TypeName': 'Boolean', 'Description': '', 'Optional': True}], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
-ADSModule.GetApplicationEndpoints:({'Parameters': [{'Name': 'instanceId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True}) 
-ADSModule.ReactivateLocalInstances:({'Parameters': [], 'ReturnTypeName': 'RunningTask', 'IsComplexType': True}) 
-ADSModule.GetInstances:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True}) 
-ADSModule.GetInstance:({'Parameters': [{'Name': 'InstanceId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'JObject', 'IsComplexType': True}) 
-ADSModule.ModifyCustomFirewallRule:({'Parameters': [{'Name': 'instanceId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'PortNumber', 'TypeName': 'Int32', 'Description': '', 'Optional': False}, {'Name': 'Range', 'TypeName': 'Int32', 'Description': '', 'Optional': False}, {'Name': 'Protocol', 'TypeName': 'PortProtocol', 'Description': '', 'Optional': False, 'ParamEnumValues': {'TCP': 0, 'UDP': 1, 'Both': 2}}, {'Name': 'Description', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Open', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-ADSModule.ManageInstance:({'Parameters': [{'Name': 'InstanceId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult<String>', 'IsComplexType': True}) 
-ADSModule.GetGroup:({'Parameters': [{'Name': 'GroupId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'JObject', 'IsComplexType': True}) 
-ADSModule.RefreshGroup:({'Parameters': [{'Name': 'GroupId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-ADSModule.GetLocalInstances:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True}) 
-ADSModule.GetInstanceStatuses:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True}) 
-ADSModule.GetProvisionFitness:({'Parameters': [], 'ReturnTypeName': 'JObject', 'IsComplexType': True}) 
-ADSModule.AttachADS:({'Parameters': [{'Name': 'Friendly', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'IsHTTPS', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}, {'Name': 'Host', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Port', 'TypeName': 'Int32', 'Description': '', 'Optional': False}, {'Name': 'InstanceID', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-ADSModule.DetatchTarget:({'Parameters': [{'Name': 'Id', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-ADSModule.UpdateTargetInfo:({'Parameters': [{'Name': 'Id', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'FriendlyName', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Url', 'TypeName': 'Uri', 'Description': '', 'Optional': False}, {'Name': 'Description', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Tags', 'TypeName': 'List<String>', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-ADSModule.ConvertToManaged:({'Parameters': [{'Name': 'InstanceName', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-ADSModule.GetInstanceNetworkInfo:({'Parameters': [{'Name': 'InstanceName', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True}) 
-ADSModule.SetInstanceNetworkInfo:({'Parameters': [{'Name': 'InstanceId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'PortMappings', 'TypeName': 'Dictionary<String, Int32>', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-ADSModule.ApplyInstanceConfiguration:({'Parameters': [{'Name': 'InstanceID', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'Args', 'TypeName': 'Dictionary<String, String>', 'Description': '', 'Optional': False}, {'Name': 'RebuildConfiguration', 'TypeName': 'Boolean', 'Description': '', 'Optional': True}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-ADSModule.CreateLocalInstance:({'Parameters': [{'Name': 'Instance', 'TypeName': 'LocalAMPInstance', 'Description': '', 'Optional': False}, {'Name': 'PostCreate', 'TypeName': 'PostCreateActions', 'Description': '', 'Optional': True, 'ParamEnumValues': {'DoNothing': 0, 'StartInstance': 1, 'StartAndUpdate': 2, 'FullStartup': 3, 'EveryTime': 16}}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-ADSModule.CreateInstance:({'Parameters': [{'Name': 'TargetADSInstance', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'NewInstanceId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}, {'Name': 'Module', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'InstanceName', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'FriendlyName', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'IPBinding', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'PortNumber', 'TypeName': 'Int32', 'Description': '', 'Optional': False}, {'Name': 'AdminUsername', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'AdminPassword', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'ProvisionSettings', 'TypeName': 'Dictionary<String, String>', 'Description': '', 'Optional': False}, {'Name': 'AutoConfigure', 'TypeName': 'Boolean', 'Description': 'When enabled, all settings other than the Module, Target and FriendlyName are ignored and replaced with automatically generated values.', 'Optional': True}, {'Name': 'PostCreate', 'TypeName': 'PostCreateActions', 'Description': '', 'Optional': True, 'ParamEnumValues': {'DoNothing': 0, 'StartInstance': 1, 'StartAndUpdate': 2, 'FullStartup': 3, 'EveryTime': 16}}, {'Name': 'StartOnBoot', 'TypeName': 'Boolean', 'Description': '', 'Optional': True}, {'Name': 'DisplayImageSource', 'TypeName': 'String', 'Description': '', 'Optional': True}, {'Name': 'TargetDatastore', 'TypeName': 'Int32', 'Description': '', 'Optional': True}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-ADSModule.SetInstanceConfig:({'Parameters': [{'Name': 'InstanceName', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'SettingNode', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Value', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-ADSModule.RefreshInstanceConfig:({'Parameters': [{'Name': 'InstanceId', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-ADSModule.HandoutInstanceConfigs:({'Parameters': [{'Name': 'ForModule', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'SettingNode', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Values', 'TypeName': 'List<String>', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-ADSModule.GetProvisionArguments:({'Parameters': [{'Name': 'ModuleName', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'IEnumerable<ProvisionSettingInfo>', 'IsComplexType': True}) 
-ADSModule.TestADSLoginDetails:({'Parameters': [{'Name': 'url', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'username', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'password', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-ADSModule.RegisterTarget:({'Parameters': [{'Name': 'controllerUrl', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'myUrl', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'username', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'password', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'twoFactorToken', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'friendlyName', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-ADSModule.UpdateTarget:({'Parameters': [{'Name': 'TargetID', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
-ADSModule.UpdateInstanceInfo:({'Parameters': [{'Name': 'InstanceId', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'FriendlyName', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Description', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'StartOnBoot', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}, {'Name': 'Suspended', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}, {'Name': 'ExcludeFromFirewall', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}, {'Name': 'RunInContainer', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}, {'Name': 'ContainerMemory', 'TypeName': 'Int32', 'Description': '', 'Optional': False}, {'Name': 'MemoryPolicy', 'TypeName': 'ContainerMemoryPolicy', 'Description': '', 'Optional': False, 'ParamEnumValues': {'NotSpecified': 0, 'Reserve': 100, 'Restrict': 200}}, {'Name': 'ContainerMaxCPU', 'TypeName': 'Single', 'Description': '', 'Optional': False}, {'Name': 'ContainerImage', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-ADSModule.SetInstanceSuspended:({'Parameters': [{'Name': 'InstanceName', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Suspended', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-ADSModule.UpgradeInstance:({'Parameters': [{'Name': 'InstanceName', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-ADSModule.StartAllInstances:({'Parameters': [], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-ADSModule.StopAllInstances:({'Parameters': [], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-ADSModule.UpgradeAllInstances:({'Parameters': [{'Name': 'RestartRunning', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-ADSModule.StartInstance:({'Parameters': [{'Name': 'InstanceName', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-ADSModule.RestartInstance:({'Parameters': [{'Name': 'InstanceName', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-ADSModule.StopInstance:({'Parameters': [{'Name': 'InstanceName', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-ADSModule.DeleteInstanceUsers:({'Parameters': [{'Name': 'InstanceId', 'TypeName': 'Guid', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-ADSModule.DeleteInstance:({'Parameters': [{'Name': 'InstanceName', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'RunningTask', 'IsComplexType': True}) 
-ADSModule.ExtractEverywhere:({'Parameters': [{'Name': 'SourceArchive', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
-ADSModule.Servers:({'Parameters': [{'Name': 'id', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'REQ_RAWJSON', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'JSONRawResponse', 'IsComplexType': True}) 
+MinecraftModule.BukGetCategories:({'Parameters': [], 'ReturnTypeName': 'JSONRawResponse', 'IsComplexType': True}) 
+MinecraftModule.BukGetPopularPlugins:({'Parameters': [], 'ReturnTypeName': 'JSONRawResponse', 'IsComplexType': True}) 
+MinecraftModule.BukGetPluginsForCategory:({'Parameters': [{'Name': 'CategoryId', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'PageNumber', 'TypeName': 'Int32', 'Description': '', 'Optional': False}, {'Name': 'PageSize', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'JSONRawResponse', 'IsComplexType': True}) 
+MinecraftModule.BukGetPluginInfo:({'Parameters': [{'Name': 'PluginId', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'JSONRawResponse', 'IsComplexType': True}) 
+MinecraftModule.BukGetInstalledPlugins:({'Parameters': [], 'ReturnTypeName': 'JSONRawResponse', 'IsComplexType': True}) 
+MinecraftModule.BukGetRemovePlugin:({'Parameters': [{'Name': 'PluginId', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
+MinecraftModule.BukGetInstallUpdatePlugin:({'Parameters': [{'Name': 'pluginId', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'RunningTask', 'IsComplexType': True}) 
+MinecraftModule.BukGetSearch:({'Parameters': [{'Name': 'Query', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'PageNumber', 'TypeName': 'Int32', 'Description': '', 'Optional': False}, {'Name': 'PageSize', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'JSONRawResponse', 'IsComplexType': True}) 
+MinecraftModule.GetHeadByUUID:({'Description': 'Get a skin as a base64 string', 'Returns': '', 'Parameters': [{'Name': 'id', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'String', 'IsComplexType': False}) 
+MinecraftModule.GetFailureReason:({'Parameters': [], 'ReturnTypeName': 'String', 'IsComplexType': False}) 
+MinecraftModule.AcceptEULA:({'Parameters': [], 'ReturnTypeName': 'Boolean', 'IsComplexType': False}) 
+MinecraftModule.BanUserByID:({'Parameters': [{'Name': 'ID', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
+MinecraftModule.KickUserByID:({'Parameters': [{'Name': 'ID', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
+MinecraftModule.ClearInventoryByID:({'Parameters': [{'Name': 'ID', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
+MinecraftModule.KillByID:({'Parameters': [{'Name': 'ID', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
+MinecraftModule.SmiteByID:({'Description': 'Strike a player with lightning', 'Returns': '', 'Parameters': [{'Name': 'ID', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
+MinecraftModule.GetOPWhitelist:({'Parameters': [], 'ReturnTypeName': 'JObject', 'IsComplexType': True}) 
+MinecraftModule.GetWhitelist:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True}) 
+MinecraftModule.LoadOPList:({'Parameters': [], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True}) 
+MinecraftModule.AddOPEntry:({'Parameters': [{'Name': 'UserOrUUID', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+MinecraftModule.RemoveOPEntry:({'Parameters': [{'Name': 'UserOrUUID', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
+MinecraftModule.AddToWhitelist:({'Parameters': [{'Name': 'UserOrUUID', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
+MinecraftModule.RemoveWhitelistEntry:({'Parameters': [{'Name': 'UserOrUUID', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
 FileManagerPlugin.Dummy:({'Parameters': [], 'ReturnTypeName': 'Void', 'IsComplexType': False}) 
 FileManagerPlugin.CalculateFileMD5Sum:({'Parameters': [{'Name': 'FilePath', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult<String>', 'IsComplexType': True}) 
 FileManagerPlugin.ChangeExclusion:({'Parameters': [{'Name': 'ModifyPath', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'AsDirectory', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}, {'Name': 'Exclude', 'TypeName': 'Boolean', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
 FileManagerPlugin.CreateArchive:({'Parameters': [{'Name': 'PathToArchive', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
 FileManagerPlugin.ExtractArchive:({'Parameters': [{'Name': 'ArchivePath', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'DestinationPath', 'TypeName': 'String', 'Description': '', 'Optional': True}], 'ReturnTypeName': 'ActionResult', 'IsComplexType': True}) 
 FileManagerPlugin.GetDirectoryListing:({'Parameters': [{'Name': 'Dir', 'TypeName': 'String', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'IEnumerable<JObject>', 'IsComplexType': True}) 
 FileManagerPlugin.GetFileChunk:({'Parameters': [{'Name': 'Filename', 'TypeName': 'String', 'Description': '', 'Optional': False}, {'Name': 'Position', 'TypeName': 'Int64', 'Description': '', 'Optional': False}, {'Name': 'Length', 'TypeName': 'Int32', 'Description': '', 'Optional': False}], 'ReturnTypeName': 'JObject', 'IsComplexType': True})
```

### Comparing `cubecoders_amp_api_wrapper-0.0.42b0/docs/permission_nodes.md` & `cubecoders_amp_api_wrapper-0.1.0.post0/docs/permission_nodes.md`

 * *Files identical despite different names*

### Comparing `cubecoders_amp_api_wrapper-0.0.42b0/docs/permission_nodes.txt` & `cubecoders_amp_api_wrapper-0.1.0.post0/docs/permission_nodes.txt`

 * *Files identical despite different names*

### Comparing `cubecoders_amp_api_wrapper-0.0.42b0/docs/setting_nodes.md` & `cubecoders_amp_api_wrapper-0.1.0.post0/docs/setting_nodes.md`

 * *Files identical despite different names*

### Comparing `cubecoders_amp_api_wrapper-0.0.42b0/docs/setting_nodes.txt` & `cubecoders_amp_api_wrapper-0.1.0.post0/docs/setting_nodes.txt`

 * *Files identical despite different names*

### Comparing `cubecoders_amp_api_wrapper-0.0.42b0/setup.py` & `cubecoders_amp_api_wrapper-0.1.0.post0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,25 +29,25 @@
     license='GNU',
     project_urls={
         'GitHub': 'https://github.com/k8thekat/AMPAPI_Python',
         'Changelog': 'https://github.com/k8thekat/AMPAPI_Python/blob/master/CHANGELOG.md',
     },
     packages=packages,
     package_data={
-        "docs": ["docs/api_spec.md", "docs/permission_nodes.md", "docs/setting_nodes.md"],
+        "docs": ["docs/ADS_api_spec.md", "docs/Minecraft_api_spec.md", "docs/permission_nodes.md", "docs/setting_nodes.md"],
         "license": ["LICENSE"],
         "requirements": ["requirements.txt"],
         "readme": ["README.md"],
         "changelog": ["CHANGELOG.md"]},
     long_description=readme,
     long_description_content_type="text/markdown",
     install_requires=requirements,
     python_requires='>=3.9.0',
     classifiers=[
-        'Development Status :: 3 - Alpha',
+        'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.12',
```

