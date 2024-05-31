# Comparing `tmp/wp_enhanced-0.9.0.tar.gz` & `tmp/wp_enhanced-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wp_enhanced-0.9.0.tar", max compression
+gzip compressed data, was "wp_enhanced-0.9.1.tar", max compression
```

## Comparing `wp_enhanced-0.9.0.tar` & `wp_enhanced-0.9.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0      629 2024-05-29 10:23:14.223279 wp_enhanced-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     1975 2024-03-05 10:44:56.655179 wp_enhanced-0.9.0/README.md
--rw-r--r--   0        0        0     5471 2024-05-29 08:37:52.344092 wp_enhanced-0.9.0/src/wpe/cli.py
--rw-r--r--   0        0        0     3414 2024-05-20 06:36:07.243649 wp_enhanced-0.9.0/src/wpe/constants.py
--rw-r--r--   0        0        0     9201 2024-05-29 09:55:00.869477 wp_enhanced-0.9.0/src/wpe/core.py
--rw-r--r--   0        0        0     1778 2024-03-19 10:33:46.953081 wp_enhanced-0.9.0/src/wpe/hook_processor.py
--rw-r--r--   0        0        0    22804 2024-05-24 09:25:52.692469 wp_enhanced-0.9.0/src/wpe/parameter.py
--rw-r--r--   0        0        0     2557 2024-05-29 09:54:49.747133 wp_enhanced-0.9.0/src/wpe/pathman.py
--rw-r--r--   0        0        0     4372 2024-05-20 08:48:15.544654 wp_enhanced-0.9.0/src/wpe/project_config.py
--rw-r--r--   0        0        0     2536 2024-05-29 10:22:40.904327 wp_enhanced-0.9.0/src/wpe/renamer.py
--rw-r--r--   0        0        0      529 2024-03-20 09:54:37.946663 wp_enhanced-0.9.0/src/wpe/templates/.wpe/hooks/post_build.py
--rw-r--r--   0        0        0      570 2024-05-15 07:41:57.248430 wp_enhanced-0.9.0/src/wpe/templates/.wpe/hooks/pre_premake.py
--rw-r--r--   0        0        0     2313 2024-05-24 09:16:35.575895 wp_enhanced-0.9.0/src/wpe/templates/.wpe/wpe_project.toml
--rw-r--r--   0        0        0     3564 2024-05-15 10:45:20.195972 wp_enhanced-0.9.0/src/wpe/templates/SoundEnginePlugin/ProjectNameFXParams.cpp
--rw-r--r--   0        0        0     3637 2024-05-15 10:45:01.387675 wp_enhanced-0.9.0/src/wpe/templates/SoundEnginePlugin/ProjectNameFXParams.h
--rw-r--r--   0        0        0        7 2024-03-28 07:45:27.251336 wp_enhanced-0.9.0/src/wpe/templates/test/.gitignore
--rw-r--r--   0        0        0      690 2024-03-28 10:50:17.608326 wp_enhanced-0.9.0/src/wpe/templates/test/CMakeLists.txt
--rw-r--r--   0        0        0     1088 2024-03-28 10:27:22.354678 wp_enhanced-0.9.0/src/wpe/templates/test/main.cpp
--rw-r--r--   0        0        0     3720 2024-03-28 10:20:00.582064 wp_enhanced-0.9.0/src/wpe/templates/test/util/test_mem_alloc.hpp
--rw-r--r--   0        0        0      546 2024-03-28 10:23:24.722404 wp_enhanced-0.9.0/src/wpe/templates/test/util/test_util.hpp
--rw-r--r--   0        0        0     2319 2024-05-21 07:17:38.787997 wp_enhanced-0.9.0/src/wpe/templates/WwisePlugin/ProjectName.rc
--rw-r--r--   0        0        0     2591 2023-11-09 12:01:43.217512 wp_enhanced-0.9.0/src/wpe/templates/WwisePlugin/ProjectName.xml
--rw-r--r--   0        0        0     2619 2023-11-09 12:01:43.210512 wp_enhanced-0.9.0/src/wpe/templates/WwisePlugin/ProjectNamePlugin.cpp
--rw-r--r--   0        0        0     2212 2023-11-09 12:01:43.213515 wp_enhanced-0.9.0/src/wpe/templates/WwisePlugin/ProjectNamePlugin.h
--rw-r--r--   0        0        0      502 2024-05-21 07:17:53.334293 wp_enhanced-0.9.0/src/wpe/templates/WwisePlugin/resource.h
--rw-r--r--   0        0        0     1649 2024-05-21 07:38:14.439284 wp_enhanced-0.9.0/src/wpe/templates/WwisePlugin/Win32/ProjectNamePluginGUI.cpp
--rw-r--r--   0        0        0      865 2024-05-21 06:24:33.977130 wp_enhanced-0.9.0/src/wpe/templates/WwisePlugin/Win32/ProjectNamePluginGUI.h
--rw-r--r--   0        0        0     4743 2024-03-28 10:59:21.634177 wp_enhanced-0.9.0/src/wpe/test_runner.py
--rw-r--r--   0        0        0     3440 2024-05-29 10:11:26.069297 wp_enhanced-0.9.0/src/wpe/util.py
--rw-r--r--   0        0        0     5618 2024-03-19 10:51:33.313938 wp_enhanced-0.9.0/src/wpe/wp_patch/build.py
--rw-r--r--   0        0        0     2847 2024-03-19 03:42:12.795265 wp_enhanced-0.9.0/src/wpe/wp_patch/common/command/android.py
--rw-r--r--   0        0        0     1409 2024-03-19 03:38:23.562202 wp_enhanced-0.9.0/src/wpe/wp_patch/common/platform/android.py
--rw-r--r--   0        0        0    11092 2024-04-28 06:59:44.257676 wp_enhanced-0.9.0/src/wpe/wp_patch/package.py
--rw-r--r--   0        0        0     2560 2024-03-14 08:02:19.221827 wp_enhanced-0.9.0/src/wpe/wp_patch/premake.py
--rw-r--r--   0        0        0    12962 2024-03-20 09:54:02.989529 wp_enhanced-0.9.0/src/wpe/wp_patch/premakePlugins.lua
--rw-r--r--   0        0        0     3846 2024-03-19 10:51:33.314938 wp_enhanced-0.9.0/src/wpe/wp_wrapper.py
--rw-r--r--   0        0        0     2760 1970-01-01 00:00:00.000000 wp_enhanced-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0      629 2024-05-31 07:46:41.672168 wp_enhanced-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     1975 2024-03-05 10:44:56.655179 wp_enhanced-0.9.1/README.md
+-rw-r--r--   0        0        0     5471 2024-05-29 08:37:52.344092 wp_enhanced-0.9.1/src/wpe/cli.py
+-rw-r--r--   0        0        0     3414 2024-05-20 06:36:07.243649 wp_enhanced-0.9.1/src/wpe/constants.py
+-rw-r--r--   0        0        0     9201 2024-05-29 09:55:00.869477 wp_enhanced-0.9.1/src/wpe/core.py
+-rw-r--r--   0        0        0     1778 2024-03-19 10:33:46.953081 wp_enhanced-0.9.1/src/wpe/hook_processor.py
+-rw-r--r--   0        0        0    22804 2024-05-24 09:25:52.692469 wp_enhanced-0.9.1/src/wpe/parameter.py
+-rw-r--r--   0        0        0     2557 2024-05-29 09:54:49.747133 wp_enhanced-0.9.1/src/wpe/pathman.py
+-rw-r--r--   0        0        0     4372 2024-05-20 08:48:15.544654 wp_enhanced-0.9.1/src/wpe/project_config.py
+-rw-r--r--   0        0        0     2536 2024-05-29 10:22:40.904327 wp_enhanced-0.9.1/src/wpe/renamer.py
+-rw-r--r--   0        0        0      529 2024-03-20 09:54:37.946663 wp_enhanced-0.9.1/src/wpe/templates/.wpe/hooks/post_build.py
+-rw-r--r--   0        0        0      570 2024-05-15 07:41:57.248430 wp_enhanced-0.9.1/src/wpe/templates/.wpe/hooks/pre_premake.py
+-rw-r--r--   0        0        0     2313 2024-05-24 09:16:35.575895 wp_enhanced-0.9.1/src/wpe/templates/.wpe/wpe_project.toml
+-rw-r--r--   0        0        0     3564 2024-05-15 10:45:20.195972 wp_enhanced-0.9.1/src/wpe/templates/SoundEnginePlugin/ProjectNameFXParams.cpp
+-rw-r--r--   0        0        0     3637 2024-05-15 10:45:01.387675 wp_enhanced-0.9.1/src/wpe/templates/SoundEnginePlugin/ProjectNameFXParams.h
+-rw-r--r--   0        0        0        7 2024-03-28 07:45:27.251336 wp_enhanced-0.9.1/src/wpe/templates/test/.gitignore
+-rw-r--r--   0        0        0      690 2024-03-28 10:50:17.608326 wp_enhanced-0.9.1/src/wpe/templates/test/CMakeLists.txt
+-rw-r--r--   0        0        0     1088 2024-03-28 10:27:22.354678 wp_enhanced-0.9.1/src/wpe/templates/test/main.cpp
+-rw-r--r--   0        0        0     3720 2024-03-28 10:20:00.582064 wp_enhanced-0.9.1/src/wpe/templates/test/util/test_mem_alloc.hpp
+-rw-r--r--   0        0        0      546 2024-03-28 10:23:24.722404 wp_enhanced-0.9.1/src/wpe/templates/test/util/test_util.hpp
+-rw-r--r--   0        0        0     2319 2024-05-21 07:17:38.787997 wp_enhanced-0.9.1/src/wpe/templates/WwisePlugin/ProjectName.rc
+-rw-r--r--   0        0        0     2591 2023-11-09 12:01:43.217512 wp_enhanced-0.9.1/src/wpe/templates/WwisePlugin/ProjectName.xml
+-rw-r--r--   0        0        0     2619 2023-11-09 12:01:43.210512 wp_enhanced-0.9.1/src/wpe/templates/WwisePlugin/ProjectNamePlugin.cpp
+-rw-r--r--   0        0        0     2212 2023-11-09 12:01:43.213515 wp_enhanced-0.9.1/src/wpe/templates/WwisePlugin/ProjectNamePlugin.h
+-rw-r--r--   0        0        0      502 2024-05-21 07:17:53.334293 wp_enhanced-0.9.1/src/wpe/templates/WwisePlugin/resource.h
+-rw-r--r--   0        0        0     1649 2024-05-21 07:38:14.439284 wp_enhanced-0.9.1/src/wpe/templates/WwisePlugin/Win32/ProjectNamePluginGUI.cpp
+-rw-r--r--   0        0        0      865 2024-05-21 06:24:33.977130 wp_enhanced-0.9.1/src/wpe/templates/WwisePlugin/Win32/ProjectNamePluginGUI.h
+-rw-r--r--   0        0        0     4743 2024-03-28 10:59:21.634177 wp_enhanced-0.9.1/src/wpe/test_runner.py
+-rw-r--r--   0        0        0     3441 2024-05-31 07:46:13.602498 wp_enhanced-0.9.1/src/wpe/util.py
+-rw-r--r--   0        0        0     5618 2024-03-19 10:51:33.313938 wp_enhanced-0.9.1/src/wpe/wp_patch/build.py
+-rw-r--r--   0        0        0     2847 2024-03-19 03:42:12.795265 wp_enhanced-0.9.1/src/wpe/wp_patch/common/command/android.py
+-rw-r--r--   0        0        0     1409 2024-03-19 03:38:23.562202 wp_enhanced-0.9.1/src/wpe/wp_patch/common/platform/android.py
+-rw-r--r--   0        0        0    11092 2024-04-28 06:59:44.257676 wp_enhanced-0.9.1/src/wpe/wp_patch/package.py
+-rw-r--r--   0        0        0     2560 2024-03-14 08:02:19.221827 wp_enhanced-0.9.1/src/wpe/wp_patch/premake.py
+-rw-r--r--   0        0        0    12962 2024-03-20 09:54:02.989529 wp_enhanced-0.9.1/src/wpe/wp_patch/premakePlugins.lua
+-rw-r--r--   0        0        0     3846 2024-03-19 10:51:33.314938 wp_enhanced-0.9.1/src/wpe/wp_wrapper.py
+-rw-r--r--   0        0        0     2760 1970-01-01 00:00:00.000000 wp_enhanced-0.9.1/PKG-INFO
```

### Comparing `wp_enhanced-0.9.0/pyproject.toml` & `wp_enhanced-0.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wp-enhanced"
-version = "0.9.0"
+version = "0.9.1"
 description = "Wrapper of `wp.py`. Easy to premake, build, and deploy wwise plugins."
 authors = ["tgalpha <tanalpha.zhy@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "wpe", from = "src" }
 ]
```

### Comparing `wp_enhanced-0.9.0/README.md` & `wp_enhanced-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `wp_enhanced-0.9.0/src/wpe/cli.py` & `wp_enhanced-0.9.1/src/wpe/cli.py`

 * *Files identical despite different names*

### Comparing `wp_enhanced-0.9.0/src/wpe/constants.py` & `wp_enhanced-0.9.1/src/wpe/constants.py`

 * *Files identical despite different names*

### Comparing `wp_enhanced-0.9.0/src/wpe/core.py` & `wp_enhanced-0.9.1/src/wpe/core.py`

 * *Files identical despite different names*

### Comparing `wp_enhanced-0.9.0/src/wpe/hook_processor.py` & `wp_enhanced-0.9.1/src/wpe/hook_processor.py`

 * *Files identical despite different names*

### Comparing `wp_enhanced-0.9.0/src/wpe/parameter.py` & `wp_enhanced-0.9.1/src/wpe/parameter.py`

 * *Files identical despite different names*

### Comparing `wp_enhanced-0.9.0/src/wpe/pathman.py` & `wp_enhanced-0.9.1/src/wpe/pathman.py`

 * *Files identical despite different names*

### Comparing `wp_enhanced-0.9.0/src/wpe/project_config.py` & `wp_enhanced-0.9.1/src/wpe/project_config.py`

 * *Files identical despite different names*

### Comparing `wp_enhanced-0.9.0/src/wpe/renamer.py` & `wp_enhanced-0.9.1/src/wpe/renamer.py`

 * *Files identical despite different names*

### Comparing `wp_enhanced-0.9.0/src/wpe/templates/.wpe/hooks/post_build.py` & `wp_enhanced-0.9.1/src/wpe/templates/.wpe/hooks/post_build.py`

 * *Files identical despite different names*

### Comparing `wp_enhanced-0.9.0/src/wpe/templates/.wpe/hooks/pre_premake.py` & `wp_enhanced-0.9.1/src/wpe/templates/.wpe/hooks/pre_premake.py`

 * *Files identical despite different names*

### Comparing `wp_enhanced-0.9.0/src/wpe/templates/.wpe/wpe_project.toml` & `wp_enhanced-0.9.1/src/wpe/templates/.wpe/wpe_project.toml`

 * *Files identical despite different names*

### Comparing `wp_enhanced-0.9.0/src/wpe/templates/SoundEnginePlugin/ProjectNameFXParams.cpp` & `wp_enhanced-0.9.1/src/wpe/templates/SoundEnginePlugin/ProjectNameFXParams.cpp`

 * *Files identical despite different names*

### Comparing `wp_enhanced-0.9.0/src/wpe/templates/SoundEnginePlugin/ProjectNameFXParams.h` & `wp_enhanced-0.9.1/src/wpe/templates/SoundEnginePlugin/ProjectNameFXParams.h`

 * *Files identical despite different names*

### Comparing `wp_enhanced-0.9.0/src/wpe/templates/test/CMakeLists.txt` & `wp_enhanced-0.9.1/src/wpe/templates/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `wp_enhanced-0.9.0/src/wpe/templates/test/main.cpp` & `wp_enhanced-0.9.1/src/wpe/templates/test/main.cpp`

 * *Files identical despite different names*

### Comparing `wp_enhanced-0.9.0/src/wpe/templates/test/util/test_mem_alloc.hpp` & `wp_enhanced-0.9.1/src/wpe/templates/test/util/test_mem_alloc.hpp`

 * *Files identical despite different names*

### Comparing `wp_enhanced-0.9.0/src/wpe/templates/test/util/test_util.hpp` & `wp_enhanced-0.9.1/src/wpe/templates/test/util/test_util.hpp`

 * *Files identical despite different names*

### Comparing `wp_enhanced-0.9.0/src/wpe/templates/WwisePlugin/ProjectName.rc` & `wp_enhanced-0.9.1/src/wpe/templates/WwisePlugin/ProjectName.rc`

 * *Files identical despite different names*

### Comparing `wp_enhanced-0.9.0/src/wpe/templates/WwisePlugin/ProjectName.xml` & `wp_enhanced-0.9.1/src/wpe/templates/WwisePlugin/ProjectName.xml`

 * *Files identical despite different names*

### Comparing `wp_enhanced-0.9.0/src/wpe/templates/WwisePlugin/ProjectNamePlugin.cpp` & `wp_enhanced-0.9.1/src/wpe/templates/WwisePlugin/ProjectNamePlugin.cpp`

 * *Files identical despite different names*

### Comparing `wp_enhanced-0.9.0/src/wpe/templates/WwisePlugin/ProjectNamePlugin.h` & `wp_enhanced-0.9.1/src/wpe/templates/WwisePlugin/ProjectNamePlugin.h`

 * *Files identical despite different names*

### Comparing `wp_enhanced-0.9.0/src/wpe/templates/WwisePlugin/Win32/ProjectNamePluginGUI.cpp` & `wp_enhanced-0.9.1/src/wpe/templates/WwisePlugin/Win32/ProjectNamePluginGUI.cpp`

 * *Files identical despite different names*

### Comparing `wp_enhanced-0.9.0/src/wpe/templates/WwisePlugin/Win32/ProjectNamePluginGUI.h` & `wp_enhanced-0.9.1/src/wpe/templates/WwisePlugin/Win32/ProjectNamePluginGUI.h`

 * *Files identical despite different names*

### Comparing `wp_enhanced-0.9.0/src/wpe/test_runner.py` & `wp_enhanced-0.9.1/src/wpe/test_runner.py`

 * *Files identical despite different names*

### Comparing `wp_enhanced-0.9.0/src/wpe/util.py` & `wp_enhanced-0.9.1/src/wpe/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         # git ignored files will raise error, fallback to os.rename
         os.rename(src, dst)
     except Exception as e:
         logging.error(f'Error moving {src} to {dst} with `git mv`: {e}')
         raise e
 
 
-def replace_in_basename(path: str, old: str, new: str, count=0):
+def replace_in_basename(path: str, old: str, new: str, count=-1):
     return osp.join(osp.dirname(path), osp.basename(path).replace(old, new, count))
 
 
 def remove_path(path, ignore_errors=True):
     if osp.isfile(path):
         os.remove(path)
     if osp.isdir(path):
```

### Comparing `wp_enhanced-0.9.0/src/wpe/wp_patch/build.py` & `wp_enhanced-0.9.1/src/wpe/wp_patch/build.py`

 * *Files identical despite different names*

### Comparing `wp_enhanced-0.9.0/src/wpe/wp_patch/common/command/android.py` & `wp_enhanced-0.9.1/src/wpe/wp_patch/common/command/android.py`

 * *Files identical despite different names*

### Comparing `wp_enhanced-0.9.0/src/wpe/wp_patch/common/platform/android.py` & `wp_enhanced-0.9.1/src/wpe/wp_patch/common/platform/android.py`

 * *Files identical despite different names*

### Comparing `wp_enhanced-0.9.0/src/wpe/wp_patch/package.py` & `wp_enhanced-0.9.1/src/wpe/wp_patch/package.py`

 * *Files identical despite different names*

### Comparing `wp_enhanced-0.9.0/src/wpe/wp_patch/premake.py` & `wp_enhanced-0.9.1/src/wpe/wp_patch/premake.py`

 * *Files identical despite different names*

### Comparing `wp_enhanced-0.9.0/src/wpe/wp_patch/premakePlugins.lua` & `wp_enhanced-0.9.1/src/wpe/wp_patch/premakePlugins.lua`

 * *Files identical despite different names*

### Comparing `wp_enhanced-0.9.0/src/wpe/wp_wrapper.py` & `wp_enhanced-0.9.1/src/wpe/wp_wrapper.py`

 * *Files identical despite different names*

### Comparing `wp_enhanced-0.9.0/PKG-INFO` & `wp_enhanced-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wp-enhanced
-Version: 0.9.0
+Version: 0.9.1
 Summary: Wrapper of `wp.py`. Easy to premake, build, and deploy wwise plugins.
 Home-page: https://github.com/tgalpha/wp-enhanced
 License: MIT
 Author: tgalpha
 Author-email: tanalpha.zhy@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

