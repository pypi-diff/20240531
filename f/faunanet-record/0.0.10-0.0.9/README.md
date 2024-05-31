# Comparing `tmp/faunanet_record-0.0.10.tar.gz` & `tmp/faunanet_record-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faunanet_record-0.0.10.tar", last modified: Fri May 31 11:43:23 2024, max compression
+gzip compressed data, was "faunanet_record-0.0.9.tar", last modified: Fri May 31 11:24:45 2024, max compression
```

## Comparing `faunanet_record-0.0.10.tar` & `faunanet_record-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,21 @@
-drwxrwxr-x   0 hmack     (1004) hmack     (1005)        0 2024-05-31 11:43:23.005960 faunanet_record-0.0.10/
--rw-rw-r--   0 hmack     (1004) hmack     (1005)    11356 2024-05-24 13:41:43.000000 faunanet_record-0.0.10/LICENSE
--rw-rw-r--   0 hmack     (1004) hmack     (1005)       34 2024-05-31 11:42:54.000000 faunanet_record-0.0.10/MANIFEST.in
--rw-r--r--   0 hmack     (1004) hmack     (1005)    16464 2024-05-31 11:43:23.005960 faunanet_record-0.0.10/PKG-INFO
--rw-rw-r--   0 hmack     (1004) hmack     (1005)     2492 2024-05-31 11:42:31.000000 faunanet_record-0.0.10/README.md
--rw-rw-r--   0 hmack     (1004) hmack     (1005)     1759 2024-05-31 11:42:31.000000 faunanet_record-0.0.10/pyproject.toml
--rw-rw-r--   0 hmack     (1004) hmack     (1005)       38 2024-05-31 11:43:23.005960 faunanet_record-0.0.10/setup.cfg
-drwxrwxr-x   0 hmack     (1004) hmack     (1005)        0 2024-05-31 11:43:23.005960 faunanet_record-0.0.10/src/
-drwxrwxr-x   0 hmack     (1004) hmack     (1005)        0 2024-05-31 11:43:23.005960 faunanet_record-0.0.10/src/faunanet_record/
--rw-rw-r--   0 hmack     (1004) hmack     (1005)      138 2024-05-31 11:43:07.000000 faunanet_record-0.0.10/src/faunanet_record/__init__.py
--rw-rw-r--   0 hmack     (1004) hmack     (1005)    11178 2024-05-31 11:42:31.000000 faunanet_record-0.0.10/src/faunanet_record/audio_recording.py
--rw-rw-r--   0 hmack     (1004) hmack     (1005)     2819 2024-05-31 11:42:31.000000 faunanet_record-0.0.10/src/faunanet_record/cli.py
--rw-rw-r--   0 hmack     (1004) hmack     (1005)      301 2024-05-31 11:42:31.000000 faunanet_record-0.0.10/src/faunanet_record/default.yml
--rw-rw-r--   0 hmack     (1004) hmack     (1005)       76 2024-05-31 11:42:31.000000 faunanet_record-0.0.10/src/faunanet_record/install.yml
--rw-rw-r--   0 hmack     (1004) hmack     (1005)     6779 2024-05-31 11:42:31.000000 faunanet_record-0.0.10/src/faunanet_record/runner.py
--rw-rw-r--   0 hmack     (1004) hmack     (1005)     2630 2024-05-31 11:42:31.000000 faunanet_record-0.0.10/src/faunanet_record/set_up.py
--rw-rw-r--   0 hmack     (1004) hmack     (1005)     2205 2024-05-31 11:42:31.000000 faunanet_record-0.0.10/src/faunanet_record/utils.py
-drwxrwxr-x   0 hmack     (1004) hmack     (1005)        0 2024-05-31 11:43:23.005960 faunanet_record-0.0.10/src/faunanet_record.egg-info/
--rw-r--r--   0 hmack     (1004) hmack     (1005)    16464 2024-05-31 11:43:23.000000 faunanet_record-0.0.10/src/faunanet_record.egg-info/PKG-INFO
--rw-rw-r--   0 hmack     (1004) hmack     (1005)      555 2024-05-31 11:43:23.000000 faunanet_record-0.0.10/src/faunanet_record.egg-info/SOURCES.txt
--rw-rw-r--   0 hmack     (1004) hmack     (1005)        1 2024-05-31 11:43:23.000000 faunanet_record-0.0.10/src/faunanet_record.egg-info/dependency_links.txt
--rw-rw-r--   0 hmack     (1004) hmack     (1005)       60 2024-05-31 11:43:23.000000 faunanet_record-0.0.10/src/faunanet_record.egg-info/entry_points.txt
--rw-rw-r--   0 hmack     (1004) hmack     (1005)       98 2024-05-31 11:43:23.000000 faunanet_record-0.0.10/src/faunanet_record.egg-info/requires.txt
--rw-rw-r--   0 hmack     (1004) hmack     (1005)       16 2024-05-31 11:43:23.000000 faunanet_record-0.0.10/src/faunanet_record.egg-info/top_level.txt
+drwxrwxr-x   0 hmack     (1004) hmack     (1005)        0 2024-05-31 11:24:45.118135 faunanet_record-0.0.9/
+-rw-rw-r--   0 hmack     (1004) hmack     (1005)    11356 2024-05-24 13:41:43.000000 faunanet_record-0.0.9/LICENSE
+-rw-r--r--   0 hmack     (1004) hmack     (1005)    14611 2024-05-31 11:24:45.118135 faunanet_record-0.0.9/PKG-INFO
+-rw-rw-r--   0 hmack     (1004) hmack     (1005)      438 2024-05-31 11:08:25.000000 faunanet_record-0.0.9/README.md
+-rw-rw-r--   0 hmack     (1004) hmack     (1005)     1856 2024-05-31 11:08:25.000000 faunanet_record-0.0.9/pyproject.toml
+-rw-rw-r--   0 hmack     (1004) hmack     (1005)       38 2024-05-31 11:24:45.118135 faunanet_record-0.0.9/setup.cfg
+drwxrwxr-x   0 hmack     (1004) hmack     (1005)        0 2024-05-31 11:24:45.118135 faunanet_record-0.0.9/src/
+drwxrwxr-x   0 hmack     (1004) hmack     (1005)        0 2024-05-31 11:24:45.118135 faunanet_record-0.0.9/src/faunanet_record/
+-rw-rw-r--   0 hmack     (1004) hmack     (1005)      120 2024-05-31 11:08:25.000000 faunanet_record-0.0.9/src/faunanet_record/__init__.py
+-rw-rw-r--   0 hmack     (1004) hmack     (1005)    11178 2024-05-31 11:08:25.000000 faunanet_record-0.0.9/src/faunanet_record/audio_recording.py
+-rw-rw-r--   0 hmack     (1004) hmack     (1005)     2907 2024-05-31 11:17:53.000000 faunanet_record-0.0.9/src/faunanet_record/cli.py
+-rw-rw-r--   0 hmack     (1004) hmack     (1005)     6788 2024-05-31 11:08:25.000000 faunanet_record-0.0.9/src/faunanet_record/runner.py
+-rw-rw-r--   0 hmack     (1004) hmack     (1005)     2634 2024-05-31 11:08:25.000000 faunanet_record-0.0.9/src/faunanet_record/set_up.py
+-rw-rw-r--   0 hmack     (1004) hmack     (1005)     2205 2024-05-31 11:08:25.000000 faunanet_record-0.0.9/src/faunanet_record/utils.py
+drwxrwxr-x   0 hmack     (1004) hmack     (1005)        0 2024-05-31 11:24:45.118135 faunanet_record-0.0.9/src/faunanet_record.egg-info/
+-rw-r--r--   0 hmack     (1004) hmack     (1005)    14611 2024-05-31 11:24:45.000000 faunanet_record-0.0.9/src/faunanet_record.egg-info/PKG-INFO
+-rw-rw-r--   0 hmack     (1004) hmack     (1005)      479 2024-05-31 11:24:45.000000 faunanet_record-0.0.9/src/faunanet_record.egg-info/SOURCES.txt
+-rw-rw-r--   0 hmack     (1004) hmack     (1005)        1 2024-05-31 11:24:45.000000 faunanet_record-0.0.9/src/faunanet_record.egg-info/dependency_links.txt
+-rw-rw-r--   0 hmack     (1004) hmack     (1005)       60 2024-05-31 11:24:45.000000 faunanet_record-0.0.9/src/faunanet_record.egg-info/entry_points.txt
+-rw-rw-r--   0 hmack     (1004) hmack     (1005)      164 2024-05-31 11:24:45.000000 faunanet_record-0.0.9/src/faunanet_record.egg-info/requires.txt
+-rw-rw-r--   0 hmack     (1004) hmack     (1005)       16 2024-05-31 11:24:45.000000 faunanet_record-0.0.9/src/faunanet_record.egg-info/top_level.txt
```

### Comparing `faunanet_record-0.0.10/LICENSE` & `faunanet_record-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `faunanet_record-0.0.10/PKG-INFO` & `faunanet_record-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: faunanet-record
-Version: 0.0.10
-Summary: Audio Recording Facilities for the isparrow package
-Author-email: Harald Mack <harald.mack@iwr.uni-heidelberg.de>, Inga Ulusoy <inga.ulusoy@uni-heidelberg.de>
+Version: 0.0.9
+Summary: Audio recording facilities for the faunanet package
+Author-email: Inga Ulusoy <inga.ulusoy@uni-heidelberg.de>, Harald Mack <harald.mack@iwr.uni-heidelberg.de>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
            1. Definitions.
@@ -221,49 +221,26 @@
 Requires-Dist: click
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: librosa; extra == "dev"
+Provides-Extra: doc
+Requires-Dist: sphinx; extra == "doc"
+Requires-Dist: myst-parser; extra == "doc"
+Requires-Dist: sphinxcontrib-napoleon; extra == "doc"
+Requires-Dist: sphinx-rtd-theme; extra == "doc"
+
+[![tests](https://github.com/ssciwr/iSparrowRecord/actions/workflows/main.yml/badge.svg?event=push)](https://github.com/ssciwr/iSparrowRecord/actions/workflows/main.yml)
+[![codecov](https://codecov.io/gh/ssciwr/iSparrowRecord/graph/badge.svg?token=FwyE0PNiOk)](https://codecov.io/gh/ssciwr/iSparrowRecord)
+# faunanet_record - Audio Recording facilities for the faunanet package
 
-[![tests](https://github.com/ssciwr/faunanet-record/actions/workflows/main.yml/badge.svg?event=push)](https://github.com/ssciwr/faunanet-record/actions/workflows/main.yml)
-[![codecov](https://codecov.io/gh/ssciwr/faunanet-record/graph/badge.svg?token=FwyE0PNiOk)](https://codecov.io/gh/ssciwr/faunanet-record)
-[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=ssciwr_iSparrowRecord&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=ssciwr_iSparrowRecord)
-[![Supported OS: Linux](https://img.shields.io/badge/OS-Linux%20%7C%20macOS%20%7C%20Windows-green.svg)](https://www.linux.org/)
-[![License: Apache 2.0](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
-# faunanet-record - Audio Recording facilities for the faunanet package
-The `faunanet-record` project is a simple collection of audio recording facilities for the [faunanet](https://github.com/ssciwr/iSparrow) project. While it can be used standalone, it is designed to cooperate with `faunanet`. 
+## Summary 
+tbd
 
-## Installation
-faunanet-record officially only supports Linux-based operating systems and tests on Ubuntu. That being said, it has been successfully deployed on macOS, too. However, it has never been tried on Windows. Follow the following instruction to run it on Ubuntu: 
+## Features 
+tbd 
 
-- Install portaudio and python development libraries first. `faunanet-record` depends on pyaudio, which in turn depends on portaudio. Hence, these steps are essential. 
-```bash 
-sudo apt install python3.x-dev portaudio19-dev
-```
-Replace the `x` with the python version you want `faunanet-record` to run on, or leave it out and use `python3` only if you want your OS' default python version. `faunanet-record` has been tested on `python3.9` and `python3.12`.
+## Installation 
+tbd 
 
-- Then, to get the newest release, install `faunanet-record` via pip: 
-```bash 
-python3.x -m pip install faunanet-record
-```
-After this, you should be able to get the `faunanet-record` cli in a terminal window by typing `faunanet-record`. 
-
-For a development installation, install `faunanet-record` in editable mode: 
-
-- Clone this repository
-```bash
- git clone https://github.com/ssciwr/iSparrowRecord.git 
-```
-or, when you're using ssh: 
-```bash
-git@github.com:ssciwr/iSparrowRecord.git
-```
-
-- then, from the root directory of the repository: 
-```bash 
-python3 -m pip install -e . && python3 -m pip install -r requirements-dev.txt
-```
-
-## Usage
-`faunanet-record` comes with two configuration files -
```

### Comparing `faunanet_record-0.0.10/pyproject.toml` & `faunanet_record-0.0.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "faunanet-record"
 requires-python = ">= 3.9"
-authors=[{name = "Harald Mack", email = "harald.mack@iwr.uni-heidelberg.de"}, {name = "Inga Ulusoy", email = "inga.ulusoy@uni-heidelberg.de"}]
-description = "Audio Recording Facilities for the isparrow package"
+authors=[{name = "Inga Ulusoy", email = "inga.ulusoy@uni-heidelberg.de"}, {name = "Harald Mack", email = "harald.mack@iwr.uni-heidelberg.de"}]
+description = "Audio recording facilities for the faunanet package"
 readme ="README.md"
 license={file = "LICENSE"}
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: POSIX :: Linux",
     "License :: OSI Approved :: Apache Software License",
     "Topic :: Multimedia :: Sound/Audio :: Capture/Recording", 
@@ -34,14 +34,21 @@
     "pytest", 
     "pytest-cov",  
     "coverage", 
     "pre-commit",
     "librosa", 
 ]
 
+doc = [
+    "sphinx",
+    "myst-parser",
+    "sphinxcontrib-napoleon",
+    "sphinx-rtd-theme"
+]
+
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 # tools
 [tool.setuptools.dynamic]
 version = { attr = "faunanet_record.__version__" }
```

### Comparing `faunanet_record-0.0.10/src/faunanet_record/audio_recording.py` & `faunanet_record-0.0.9/src/faunanet_record/audio_recording.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 import pyaudio
 import wave
 
 
 class RecorderBase(ABC):
     """
-    RecorderBase Abstract base class for any audio recording functionality that shall be used with iSparrow.
+    RecorderBase Abstract base class for any audio recording functionality that shall be used with faunanet.
 
 
     Methods:
     --------
     start(stop_condition = lambda x: False):  Abstract method that needs to be implemented by derived class. Should make the caller start generate data. Runs until 'stop_condition(self)' returns True.
     stream_audio(): Abstract method that needs to be implemented by derived class. Should get a chunk of recorded data corresponding to 'length_in_s' seconds of recording.
     stop(): Abstract method that needs to be implemented by derived class. Should stop the recorder's data collecting process and release resources.
```

### Comparing `faunanet_record-0.0.10/src/faunanet_record/cli.py` & `faunanet_record-0.0.9/src/faunanet_record/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 from .utils import read_yaml, update_dict_recursive, dict_from_string
 from .runner import Runner
 from . import set_up as sus
 
+import faunanet_record
+from importlib.resources import files
 from pathlib import Path
 import warnings
 import click
 from platformdirs import user_config_dir
 
 
 @click.group()
 def cli():
     # empty because everything is done in subcommands
     pass
 
 
 @cli.command()
-@click.argument(
-    "cfg_dir",
-    type=str,
-)
+@click.option("--cfg_dir", type=str, default=str(files(faunanet_record)))
 def install(cfg_dir: str):
     "The directory given must contain 'default.yml' and 'install.yml'. Check out the defaults provided in the code repository under './config'."
     sus.set_up(cfg_dir)
 
 
 @cli.command()
 @click.option("--cfg", help="custom configuration file", default="")
 @click.option("--debug", help="Enable debug output", is_flag=True)
 @click.option(
     "--defaults",
     help="Path to where the install and default configs are",
-    default=str(user_config_dir("iSparrowRecord")),
+    default=str(user_config_dir("faunanet_record")),
 )
 @click.option(
     "--replace",
     help="Replace any entry in the config with a different value. Mostly useful for debugging or testing purposes.",
     default="{}",
 )
 def run(cfg: str, debug: bool, replace: str, defaults: str):
```

### Comparing `faunanet_record-0.0.10/src/faunanet_record/runner.py` & `faunanet_record-0.0.9/src/faunanet_record/runner.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,31 +13,31 @@
     """
     Class that runs data collection.
 
     Attributes:
     -----------
     config (dict): Configuration parameters for data collection
     end_time (int or datetime): Limit for how long or until when to collect data
-    recorder (iSparroRecord.Recorder): Recorder to collect data. See iSparrow.Recorder documentation
+    recorder (iSparroRecord.Recorder): Recorder to collect data. See faunanet.RecorderBase documentation
 
     Methods:
     --------
     output Get the output data folder
     run Run data collection
     """
 
     def _process_configs(
-        self, custom_cfg: dict, config_folder: str = user_config_dir("iSparrowRecord")
+        self, custom_cfg: dict, config_folder: str = user_config_dir("faunanet_record")
     ) -> dict:
         """
         _process_configs Make a complete config dictionary that contains all necessary parameters for the runner to work.
 
         Args:
             custom_cfg (dict): custom dictionary that overrides some of the parameters for the runner.
-            config_folder (optional, str): When given, the folder where iSparrowRecord has stored the default configuration files. Defaults to /path/to/standard/config/folder/iSparrowRecord, e.g., /home/username/.config/iSparrowRecord on linux.
+            config_folder (optional, str): When given, the folder where faunanet_record has stored the default configuration files. Defaults to /path/to/standard/config/folder/faunanet_record, e.g., /home/username/.config/faunanet_record on linux.
         Returns:
             dict:  Full configuration for the runner.
         """
 
         # get config files, then run. Their existence is guaranteed by the install
         default_filepath = Path(config_folder).expanduser() / "default.yml"
 
@@ -100,15 +100,15 @@
 
         else:
             return runtime
 
     def __init__(
         self,
         custom_config: dict = None,
-        config_folder: str = user_config_dir("iSparrowRecord"),
+        config_folder: str = user_config_dir("faunanet_record"),
     ):
         """
         __init__ Create a new 'Runner' instance. A custom configpath can be supplied to update the default config with.
                  Merges the updated config with the installation info and dumps everything to the same folder where
                  the data is recorded to.
         Args:
             custom_config (dict, optional): A custom configuration dictionary containing key-value pairs that correspond to arguments used by this class or by the Recorder. Defaults to {}.
```

### Comparing `faunanet_record-0.0.10/src/faunanet_record/set_up.py` & `faunanet_record-0.0.9/src/faunanet_record/set_up.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,32 +21,32 @@
         KeyError: A folder given in the config does not exist
 
     Returns:
         tuple: created folders: ( datafolder, configfolder)
     """
     print("...making directories")
     if "data" not in base_cfg_dirs:
-        raise KeyError("The data folder for iSparrow must be given in the base config")
+        raise KeyError("The data folder for faunaanet must be given in the base config")
 
     if "config" not in base_cfg_dirs:
-        base_cfg_dirs["config"] = "iSparrowRecord"
+        base_cfg_dirs["config"] = "faunanet_record"
 
     isd = Path(base_cfg_dirs["data"]).expanduser().resolve()
     isc = Path(user_config_dir(base_cfg_dirs["config"])).expanduser().resolve()
 
     for p in [isd, isc]:
         p.mkdir(parents=True, exist_ok=True)
 
     return isd, isc
 
 
 # add a fixture with session scope that emulates the result of a later to-be-implemented-install-routine
 def set_up(cfg_path: str = ""):
     """
-    set_up set up the faunanet-record system to be ready for running and recording data. Makes data and config folders and copies the default configs there.
+    set_up set up the faunanet_recorder system to be ready for running and recording data. Makes data and config folders and copies the default configs there.
 
     Args:
         cfg_path (str): Path to a folder containing "default.yml" (the default parameters) and "install.yml" (the install parameters).
         for_tests (bool, optional): Whether a special 'test' directory should be created for testing.
                                     Used in unit tests to not interfer with base installation mostly. Defaults to False.
     """
     print("Creating faunanet folders...")
```

### Comparing `faunanet_record-0.0.10/src/faunanet_record/utils.py` & `faunanet_record-0.0.9/src/faunanet_record/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,17 +30,17 @@
                 update_dict_recursive(vb, update)  # find entrypoint
     else:
         pass  # not found and no dictionaries - pass
 
 
 def read_yaml(path: str):
     """
-    read_yaml Read the yaml basic config file for iSparrow from path.
+    read_yaml Read the yaml basic config file for faunanet from path.
             It contains the install directory, data directory and other things used
-            by iSparrow internally.
+            by faunanet internally.
 
     Args:
         path (str): Path to the yaml base config.
 
     Returns:
         dict: read base config file.
     """
```

### Comparing `faunanet_record-0.0.10/src/faunanet_record.egg-info/PKG-INFO` & `faunanet_record-0.0.9/src/faunanet_record.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: faunanet-record
-Version: 0.0.10
-Summary: Audio Recording Facilities for the isparrow package
-Author-email: Harald Mack <harald.mack@iwr.uni-heidelberg.de>, Inga Ulusoy <inga.ulusoy@uni-heidelberg.de>
+Version: 0.0.9
+Summary: Audio recording facilities for the faunanet package
+Author-email: Inga Ulusoy <inga.ulusoy@uni-heidelberg.de>, Harald Mack <harald.mack@iwr.uni-heidelberg.de>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
            1. Definitions.
@@ -221,49 +221,26 @@
 Requires-Dist: click
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: librosa; extra == "dev"
+Provides-Extra: doc
+Requires-Dist: sphinx; extra == "doc"
+Requires-Dist: myst-parser; extra == "doc"
+Requires-Dist: sphinxcontrib-napoleon; extra == "doc"
+Requires-Dist: sphinx-rtd-theme; extra == "doc"
+
+[![tests](https://github.com/ssciwr/iSparrowRecord/actions/workflows/main.yml/badge.svg?event=push)](https://github.com/ssciwr/iSparrowRecord/actions/workflows/main.yml)
+[![codecov](https://codecov.io/gh/ssciwr/iSparrowRecord/graph/badge.svg?token=FwyE0PNiOk)](https://codecov.io/gh/ssciwr/iSparrowRecord)
+# faunanet_record - Audio Recording facilities for the faunanet package
 
-[![tests](https://github.com/ssciwr/faunanet-record/actions/workflows/main.yml/badge.svg?event=push)](https://github.com/ssciwr/faunanet-record/actions/workflows/main.yml)
-[![codecov](https://codecov.io/gh/ssciwr/faunanet-record/graph/badge.svg?token=FwyE0PNiOk)](https://codecov.io/gh/ssciwr/faunanet-record)
-[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=ssciwr_iSparrowRecord&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=ssciwr_iSparrowRecord)
-[![Supported OS: Linux](https://img.shields.io/badge/OS-Linux%20%7C%20macOS%20%7C%20Windows-green.svg)](https://www.linux.org/)
-[![License: Apache 2.0](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
-# faunanet-record - Audio Recording facilities for the faunanet package
-The `faunanet-record` project is a simple collection of audio recording facilities for the [faunanet](https://github.com/ssciwr/iSparrow) project. While it can be used standalone, it is designed to cooperate with `faunanet`. 
+## Summary 
+tbd
 
-## Installation
-faunanet-record officially only supports Linux-based operating systems and tests on Ubuntu. That being said, it has been successfully deployed on macOS, too. However, it has never been tried on Windows. Follow the following instruction to run it on Ubuntu: 
+## Features 
+tbd 
 
-- Install portaudio and python development libraries first. `faunanet-record` depends on pyaudio, which in turn depends on portaudio. Hence, these steps are essential. 
-```bash 
-sudo apt install python3.x-dev portaudio19-dev
-```
-Replace the `x` with the python version you want `faunanet-record` to run on, or leave it out and use `python3` only if you want your OS' default python version. `faunanet-record` has been tested on `python3.9` and `python3.12`.
+## Installation 
+tbd 
 
-- Then, to get the newest release, install `faunanet-record` via pip: 
-```bash 
-python3.x -m pip install faunanet-record
-```
-After this, you should be able to get the `faunanet-record` cli in a terminal window by typing `faunanet-record`. 
-
-For a development installation, install `faunanet-record` in editable mode: 
-
-- Clone this repository
-```bash
- git clone https://github.com/ssciwr/iSparrowRecord.git 
-```
-or, when you're using ssh: 
-```bash
-git@github.com:ssciwr/iSparrowRecord.git
-```
-
-- then, from the root directory of the repository: 
-```bash 
-python3 -m pip install -e . && python3 -m pip install -r requirements-dev.txt
-```
-
-## Usage
-`faunanet-record` comes with two configuration files -
```

