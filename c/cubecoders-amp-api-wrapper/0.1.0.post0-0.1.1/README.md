# Comparing `tmp/cubecoders_amp_api_wrapper-0.1.0.post0.tar.gz` & `tmp/cubecoders_amp_api_wrapper-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubecoders_amp_api_wrapper-0.1.0.post0.tar", last modified: Fri May 31 06:10:08 2024, max compression
+gzip compressed data, was "cubecoders_amp_api_wrapper-0.1.1.tar", last modified: Fri May 31 06:23:59 2024, max compression
```

## Comparing `cubecoders_amp_api_wrapper-0.1.0.post0.tar` & `cubecoders_amp_api_wrapper-0.1.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)        0 2024-05-31 06:10:06.172690 cubecoders_amp_api_wrapper-0.1.0.post0/
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    10304 2024-05-31 06:10:03.000000 cubecoders_amp_api_wrapper-0.1.0.post0/CHANGELOG.md
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    35149 2024-04-28 19:14:36.000000 cubecoders_amp_api_wrapper-0.1.0.post0/LICENSE
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)       76 2024-04-28 19:14:36.000000 cubecoders_amp_api_wrapper-0.1.0.post0/MANIFEST.in
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     4793 2024-05-31 06:10:06.166507 cubecoders_amp_api_wrapper-0.1.0.post0/PKG-INFO
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     3481 2024-05-08 15:52:03.000000 cubecoders_amp_api_wrapper-0.1.0.post0/README.md
-drwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)        0 2024-05-31 06:10:05.570693 cubecoders_amp_api_wrapper-0.1.0.post0/ampapi/
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     1576 2024-05-31 06:08:28.000000 cubecoders_amp_api_wrapper-0.1.0.post0/ampapi/__init__.py
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     3219 2024-05-10 01:40:17.000000 cubecoders_amp_api_wrapper-0.1.0.post0/ampapi/ads.py
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    76650 2024-05-31 01:56:27.000000 cubecoders_amp_api_wrapper-0.1.0.post0/ampapi/adsmodule.py
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    15128 2024-05-10 01:30:45.000000 cubecoders_amp_api_wrapper-0.1.0.post0/ampapi/base.py
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     1719 2024-05-08 21:38:55.000000 cubecoders_amp_api_wrapper-0.1.0.post0/ampapi/bridge.py
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    75481 2024-05-31 05:32:55.000000 cubecoders_amp_api_wrapper-0.1.0.post0/ampapi/core.py
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)      258 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.1.0.post0/ampapi/emailsender.py
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     8024 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.1.0.post0/ampapi/filebackup.py
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    22707 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.1.0.post0/ampapi/filemanager.py
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     2836 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.1.0.post0/ampapi/instance.py
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    19680 2024-05-08 16:26:18.000000 cubecoders_amp_api_wrapper-0.1.0.post0/ampapi/minecraft.py
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    35216 2024-05-31 05:42:23.000000 cubecoders_amp_api_wrapper-0.1.0.post0/ampapi/types.py
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     4845 2024-05-31 05:40:47.000000 cubecoders_amp_api_wrapper-0.1.0.post0/ampapi/util.py
-drwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)        0 2024-05-31 06:10:06.134691 cubecoders_amp_api_wrapper-0.1.0.post0/cubecoders_amp_api_wrapper.egg-info/
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     4793 2024-05-31 06:10:04.000000 cubecoders_amp_api_wrapper-0.1.0.post0/cubecoders_amp_api_wrapper.egg-info/PKG-INFO
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)      696 2024-05-31 06:10:04.000000 cubecoders_amp_api_wrapper-0.1.0.post0/cubecoders_amp_api_wrapper.egg-info/SOURCES.txt
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)        1 2024-05-31 06:10:04.000000 cubecoders_amp_api_wrapper-0.1.0.post0/cubecoders_amp_api_wrapper.egg-info/dependency_links.txt
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)       59 2024-05-31 06:10:04.000000 cubecoders_amp_api_wrapper-0.1.0.post0/cubecoders_amp_api_wrapper.egg-info/requires.txt
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)        7 2024-05-31 06:10:04.000000 cubecoders_amp_api_wrapper-0.1.0.post0/cubecoders_amp_api_wrapper.egg-info/top_level.txt
-drwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)        0 2024-05-31 06:10:06.094691 cubecoders_amp_api_wrapper-0.1.0.post0/docs/
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    43567 2024-05-31 05:40:12.000000 cubecoders_amp_api_wrapper-0.1.0.post0/docs/ADS_api_spec.md
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    29384 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.1.0.post0/docs/Minecraft_api_spec.md
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    10444 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.1.0.post0/docs/permission_nodes.md
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    10444 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.1.0.post0/docs/permission_nodes.txt
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     4691 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.1.0.post0/docs/setting_nodes.md
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     4649 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.1.0.post0/docs/setting_nodes.txt
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)       59 2024-05-08 21:36:33.000000 cubecoders_amp_api_wrapper-0.1.0.post0/requirements.txt
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)       38 2024-05-31 06:10:06.208382 cubecoders_amp_api_wrapper-0.1.0.post0/setup.cfg
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     2180 2024-05-31 06:02:58.000000 cubecoders_amp_api_wrapper-0.1.0.post0/setup.py
+drwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)        0 2024-05-31 06:23:57.609982 cubecoders_amp_api_wrapper-0.1.1/
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    10569 2024-05-31 06:23:24.000000 cubecoders_amp_api_wrapper-0.1.1/CHANGELOG.md
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    35149 2024-04-28 19:14:36.000000 cubecoders_amp_api_wrapper-0.1.1/LICENSE
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)       76 2024-04-28 19:14:36.000000 cubecoders_amp_api_wrapper-0.1.1/MANIFEST.in
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     4787 2024-05-31 06:23:57.606794 cubecoders_amp_api_wrapper-0.1.1/PKG-INFO
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     3481 2024-05-08 15:52:03.000000 cubecoders_amp_api_wrapper-0.1.1/README.md
+drwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)        0 2024-05-31 06:23:57.076985 cubecoders_amp_api_wrapper-0.1.1/ampapi/
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     1604 2024-05-31 06:19:46.000000 cubecoders_amp_api_wrapper-0.1.1/ampapi/__init__.py
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     3219 2024-05-10 01:40:17.000000 cubecoders_amp_api_wrapper-0.1.1/ampapi/ads.py
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    76650 2024-05-31 01:56:27.000000 cubecoders_amp_api_wrapper-0.1.1/ampapi/adsmodule.py
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    15128 2024-05-10 01:30:45.000000 cubecoders_amp_api_wrapper-0.1.1/ampapi/base.py
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     1719 2024-05-08 21:38:55.000000 cubecoders_amp_api_wrapper-0.1.1/ampapi/bridge.py
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    75481 2024-05-31 05:32:55.000000 cubecoders_amp_api_wrapper-0.1.1/ampapi/core.py
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)      258 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.1.1/ampapi/emailsender.py
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     8024 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.1.1/ampapi/filebackup.py
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    22707 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.1.1/ampapi/filemanager.py
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     2836 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.1.1/ampapi/instance.py
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    19680 2024-05-08 16:26:18.000000 cubecoders_amp_api_wrapper-0.1.1/ampapi/minecraft.py
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    35216 2024-05-31 05:42:23.000000 cubecoders_amp_api_wrapper-0.1.1/ampapi/types.py
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     4845 2024-05-31 05:40:47.000000 cubecoders_amp_api_wrapper-0.1.1/ampapi/util.py
+drwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)        0 2024-05-31 06:23:57.567982 cubecoders_amp_api_wrapper-0.1.1/cubecoders_amp_api_wrapper.egg-info/
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     4787 2024-05-31 06:23:56.000000 cubecoders_amp_api_wrapper-0.1.1/cubecoders_amp_api_wrapper.egg-info/PKG-INFO
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)      696 2024-05-31 06:23:56.000000 cubecoders_amp_api_wrapper-0.1.1/cubecoders_amp_api_wrapper.egg-info/SOURCES.txt
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)        1 2024-05-31 06:23:56.000000 cubecoders_amp_api_wrapper-0.1.1/cubecoders_amp_api_wrapper.egg-info/dependency_links.txt
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)       59 2024-05-31 06:23:56.000000 cubecoders_amp_api_wrapper-0.1.1/cubecoders_amp_api_wrapper.egg-info/requires.txt
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)        7 2024-05-31 06:23:56.000000 cubecoders_amp_api_wrapper-0.1.1/cubecoders_amp_api_wrapper.egg-info/top_level.txt
+drwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)        0 2024-05-31 06:23:57.528982 cubecoders_amp_api_wrapper-0.1.1/docs/
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    43567 2024-05-31 05:40:12.000000 cubecoders_amp_api_wrapper-0.1.1/docs/ADS_api_spec.md
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    29384 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.1.1/docs/Minecraft_api_spec.md
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    10444 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.1.1/docs/permission_nodes.md
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    10444 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.1.1/docs/permission_nodes.txt
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     4691 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.1.1/docs/setting_nodes.md
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     4649 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.1.1/docs/setting_nodes.txt
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)       59 2024-05-08 21:36:33.000000 cubecoders_amp_api_wrapper-0.1.1/requirements.txt
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)       38 2024-05-31 06:23:57.643108 cubecoders_amp_api_wrapper-0.1.1/setup.cfg
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     2180 2024-05-31 06:02:58.000000 cubecoders_amp_api_wrapper-0.1.1/setup.py
```

### Comparing `cubecoders_amp_api_wrapper-0.1.0.post0/CHANGELOG.md` & `cubecoders_amp_api_wrapper-0.1.1/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+## Version - 0.1.1 - [0cf953e](https://github.com/k8thekat/AMPAPI_Python/commit/0cf953e)
+#### __init__.py
+- Version bump `0.1.1`
+- Changed formatting of releaseLevel and `__version__` to match *PEP440*
+
+#### changelog.md
+- Version info from `0.0.42b` and `0.1.0r`
+
 ## Version - 0.1.0r - [ac16314](https://github.com/k8thekat/AMPAPI_Python/commit/ac16314)
 #### __init__.py
 - Version bump to `0.1.0r`
 - Changed `releaseLevel` to "release"
 - Version bump `0.1.0r`
 
 #### setup.py
```

### Comparing `cubecoders_amp_api_wrapper-0.1.0.post0/LICENSE` & `cubecoders_amp_api_wrapper-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cubecoders_amp_api_wrapper-0.1.0.post0/PKG-INFO` & `cubecoders_amp_api_wrapper-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cubecoders_amp_api_wrapper
-Version: 0.1.0.post0
+Version: 0.1.1
 Summary: A python wrapper for the AMP API by CubeCoders
 Home-page: https://github.com/k8thekat/AMPAPI_Python
 Author: Katelynn Cadwallader
 Author-email: Cadwalladerkatelynn+AMPAPI@gmail.com
 License: GNU
 Project-URL: GitHub, https://github.com/k8thekat/AMPAPI_Python
 Project-URL: Changelog, https://github.com/k8thekat/AMPAPI_Python/blob/master/CHANGELOG.md
```

### Comparing `cubecoders_amp_api_wrapper-0.1.0.post0/README.md` & `cubecoders_amp_api_wrapper-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `cubecoders_amp_api_wrapper-0.1.0.post0/ampapi/__init__.py` & `cubecoders_amp_api_wrapper-0.1.1/ampapi/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,15 +19,15 @@
    02110-1301, USA. 
 '''
 from __future__ import annotations
 
 __title__ = "CubeCoders AMP API"
 __author__ = "k8thekat"
 __license__ = "GNU"
-__version__ = "0.1.0r"
+__version__ = "0.1.1"
 __credits__ = "AMP by CubeCoders and associates."
 
 from typing import Literal, NamedTuple
 
 from .ads import *
 from .adsmodule import *
 from .bridge import *
@@ -41,13 +41,13 @@
 from .util import *
 
 
 class VersionInfo(NamedTuple):
     Major: int
     Minor: int
     Revision: int
-    releaseLevel: Literal["alpha", "beta", "release"]
+    releaseLevel: Literal["alpha", "beta", "pre-release", "release", "development"]
 
 
-version_info: VersionInfo = VersionInfo(Major=0, Minor=1, Revision=00, releaseLevel="release")
+version_info: VersionInfo = VersionInfo(Major=0, Minor=1, Revision=1, releaseLevel="release")
 
 del NamedTuple, Literal, VersionInfo
```

### Comparing `cubecoders_amp_api_wrapper-0.1.0.post0/ampapi/ads.py` & `cubecoders_amp_api_wrapper-0.1.1/ampapi/ads.py`

 * *Files identical despite different names*

### Comparing `cubecoders_amp_api_wrapper-0.1.0.post0/ampapi/adsmodule.py` & `cubecoders_amp_api_wrapper-0.1.1/ampapi/adsmodule.py`

 * *Files identical despite different names*

### Comparing `cubecoders_amp_api_wrapper-0.1.0.post0/ampapi/base.py` & `cubecoders_amp_api_wrapper-0.1.1/ampapi/base.py`

 * *Files identical despite different names*

### Comparing `cubecoders_amp_api_wrapper-0.1.0.post0/ampapi/bridge.py` & `cubecoders_amp_api_wrapper-0.1.1/ampapi/bridge.py`

 * *Files identical despite different names*

### Comparing `cubecoders_amp_api_wrapper-0.1.0.post0/ampapi/core.py` & `cubecoders_amp_api_wrapper-0.1.1/ampapi/core.py`

 * *Files identical despite different names*

### Comparing `cubecoders_amp_api_wrapper-0.1.0.post0/ampapi/filebackup.py` & `cubecoders_amp_api_wrapper-0.1.1/ampapi/filebackup.py`

 * *Files identical despite different names*

### Comparing `cubecoders_amp_api_wrapper-0.1.0.post0/ampapi/filemanager.py` & `cubecoders_amp_api_wrapper-0.1.1/ampapi/filemanager.py`

 * *Files identical despite different names*

### Comparing `cubecoders_amp_api_wrapper-0.1.0.post0/ampapi/instance.py` & `cubecoders_amp_api_wrapper-0.1.1/ampapi/instance.py`

 * *Files identical despite different names*

### Comparing `cubecoders_amp_api_wrapper-0.1.0.post0/ampapi/minecraft.py` & `cubecoders_amp_api_wrapper-0.1.1/ampapi/minecraft.py`

 * *Files identical despite different names*

### Comparing `cubecoders_amp_api_wrapper-0.1.0.post0/ampapi/types.py` & `cubecoders_amp_api_wrapper-0.1.1/ampapi/types.py`

 * *Files identical despite different names*

### Comparing `cubecoders_amp_api_wrapper-0.1.0.post0/ampapi/util.py` & `cubecoders_amp_api_wrapper-0.1.1/ampapi/util.py`

 * *Files identical despite different names*

### Comparing `cubecoders_amp_api_wrapper-0.1.0.post0/cubecoders_amp_api_wrapper.egg-info/PKG-INFO` & `cubecoders_amp_api_wrapper-0.1.1/cubecoders_amp_api_wrapper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cubecoders_amp_api_wrapper
-Version: 0.1.0.post0
+Version: 0.1.1
 Summary: A python wrapper for the AMP API by CubeCoders
 Home-page: https://github.com/k8thekat/AMPAPI_Python
 Author: Katelynn Cadwallader
 Author-email: Cadwalladerkatelynn+AMPAPI@gmail.com
 License: GNU
 Project-URL: GitHub, https://github.com/k8thekat/AMPAPI_Python
 Project-URL: Changelog, https://github.com/k8thekat/AMPAPI_Python/blob/master/CHANGELOG.md
```

### Comparing `cubecoders_amp_api_wrapper-0.1.0.post0/cubecoders_amp_api_wrapper.egg-info/SOURCES.txt` & `cubecoders_amp_api_wrapper-0.1.1/cubecoders_amp_api_wrapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cubecoders_amp_api_wrapper-0.1.0.post0/docs/ADS_api_spec.md` & `cubecoders_amp_api_wrapper-0.1.1/docs/ADS_api_spec.md`

 * *Files identical despite different names*

### Comparing `cubecoders_amp_api_wrapper-0.1.0.post0/docs/Minecraft_api_spec.md` & `cubecoders_amp_api_wrapper-0.1.1/docs/Minecraft_api_spec.md`

 * *Files identical despite different names*

### Comparing `cubecoders_amp_api_wrapper-0.1.0.post0/docs/permission_nodes.md` & `cubecoders_amp_api_wrapper-0.1.1/docs/permission_nodes.md`

 * *Files identical despite different names*

### Comparing `cubecoders_amp_api_wrapper-0.1.0.post0/docs/permission_nodes.txt` & `cubecoders_amp_api_wrapper-0.1.1/docs/permission_nodes.txt`

 * *Files identical despite different names*

### Comparing `cubecoders_amp_api_wrapper-0.1.0.post0/docs/setting_nodes.md` & `cubecoders_amp_api_wrapper-0.1.1/docs/setting_nodes.md`

 * *Files identical despite different names*

### Comparing `cubecoders_amp_api_wrapper-0.1.0.post0/docs/setting_nodes.txt` & `cubecoders_amp_api_wrapper-0.1.1/docs/setting_nodes.txt`

 * *Files identical despite different names*

### Comparing `cubecoders_amp_api_wrapper-0.1.0.post0/setup.py` & `cubecoders_amp_api_wrapper-0.1.1/setup.py`

 * *Files identical despite different names*

