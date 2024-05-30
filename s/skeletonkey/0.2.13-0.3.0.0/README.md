# Comparing `tmp/skeletonkey-0.2.13.tar.gz` & `tmp/skeletonkey-0.3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skeletonkey-0.2.13.tar", last modified: Tue May 14 18:10:05 2024, max compression
+gzip compressed data, was "skeletonkey-0.3.0.0.tar", last modified: Thu May 30 22:03:22 2024, max compression
```

## Comparing `skeletonkey-0.2.13.tar` & `skeletonkey-0.3.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:10:05.774318 skeletonkey-0.2.13/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-14 18:10:03.000000 skeletonkey-0.2.13/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7642 2024-05-14 18:10:05.774318 skeletonkey-0.2.13/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7142 2024-05-14 18:10:03.000000 skeletonkey-0.2.13/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 18:10:05.774318 skeletonkey-0.2.13/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-14 18:10:05.000000 skeletonkey-0.2.13/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:10:05.774318 skeletonkey-0.2.13/skeletonkey/
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-14 18:10:03.000000 skeletonkey-0.2.13/skeletonkey/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16514 2024-05-14 18:10:03.000000 skeletonkey-0.2.13/skeletonkey/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-05-14 18:10:03.000000 skeletonkey-0.2.13/skeletonkey/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-05-14 18:10:03.000000 skeletonkey-0.2.13/skeletonkey/instantiate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:10:05.774318 skeletonkey-0.2.13/skeletonkey.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7642 2024-05-14 18:10:05.000000 skeletonkey-0.2.13/skeletonkey.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-14 18:10:05.000000 skeletonkey-0.2.13/skeletonkey.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 18:10:05.000000 skeletonkey-0.2.13/skeletonkey.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-14 18:10:05.000000 skeletonkey-0.2.13/skeletonkey.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 18:10:05.000000 skeletonkey-0.2.13/skeletonkey.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:03:22.741806 skeletonkey-0.3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-30 22:03:17.000000 skeletonkey-0.3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7643 2024-05-30 22:03:22.741806 skeletonkey-0.3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7142 2024-05-30 22:03:17.000000 skeletonkey-0.3.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 22:03:22.741806 skeletonkey-0.3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-30 22:03:22.000000 skeletonkey-0.3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:03:22.741806 skeletonkey-0.3.0.0/skeletonkey/
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-30 22:03:17.000000 skeletonkey-0.3.0.0/skeletonkey/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18849 2024-05-30 22:03:17.000000 skeletonkey-0.3.0.0/skeletonkey/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-05-30 22:03:17.000000 skeletonkey-0.3.0.0/skeletonkey/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-05-30 22:03:17.000000 skeletonkey-0.3.0.0/skeletonkey/instantiate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:03:22.741806 skeletonkey-0.3.0.0/skeletonkey.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7643 2024-05-30 22:03:22.000000 skeletonkey-0.3.0.0/skeletonkey.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-30 22:03:22.000000 skeletonkey-0.3.0.0/skeletonkey.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 22:03:22.000000 skeletonkey-0.3.0.0/skeletonkey.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-30 22:03:22.000000 skeletonkey-0.3.0.0/skeletonkey.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-30 22:03:22.000000 skeletonkey-0.3.0.0/skeletonkey.egg-info/top_level.txt
```

### Comparing `skeletonkey-0.2.13/LICENSE` & `skeletonkey-0.3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `skeletonkey-0.2.13/PKG-INFO` & `skeletonkey-0.3.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skeletonkey
-Version: 0.2.13
+Version: 0.3.0.0
 Summary: A bare-bones configuration managment tool.
 Home-page: https://github.com/sizemore0125/skeletonkey
 Author: Logan Sizemore
 Author-email: sizemore0125@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `skeletonkey-0.2.13/README.md` & `skeletonkey-0.3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `skeletonkey-0.2.13/setup.py` & `skeletonkey-0.3.0.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="skeletonkey",
-    version='v0.2.13',
+    version='v0.3.0.0',
     description="A bare-bones configuration managment tool.",
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/sizemore0125/skeletonkey",
     author="Logan Sizemore",
     author_email="sizemore0125@gmail.com",
```

### Comparing `skeletonkey-0.2.13/skeletonkey/__init__.py` & `skeletonkey-0.3.0.0/skeletonkey/__init__.py`

 * *Files identical despite different names*

### Comparing `skeletonkey-0.2.13/skeletonkey/config.py` & `skeletonkey-0.3.0.0/skeletonkey/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import yaml
 import argparse
 import os
 from typing import List, Tuple, Union
 
 from .instantiate import instantiate
 
-BASE_DEFAULT_KEYWORD: str = "defaults"
+BASE_PROFILES_KEYWORD: str = "profiles"
 BASE_COLLECTION_KEYWORD: str = "keyring"
 
 class Config():
     def __init__(self, *args, **kwargs):
         """
         Initializes the config from a dictionary or from kwargs.\n
 
@@ -87,15 +87,15 @@
         return self.__getattribute__(key)
 
     def __setitem__(self, key: str, value):
         self.__setattr__(key, value)
 
 
     def __delitem__(self, key: str):
-        self.__delattr__()
+        self.__delattr__(key)
 
     def __str__(self):
         return self._subconfig_str(self, 0)[1:]
 
     def __repr__(self):
         return f"Config({self._subconfig_str(self, 1)})"
     
@@ -220,54 +220,71 @@
     yaml_extention1 = ".yaml"
     yaml_extention2 = ".yml"
     if not path.endswith(yaml_extention1) and not path.endswith(yaml_extention2):
         path += yaml_extention1
     return path
 
 
-def get_default_yaml_paths_from_dict(default_yaml: dict) -> List[str]:
+def load_yaml_config(config_path: str,
+                     config_name: str,
+                     profile: str,
+                     profile_specifiers: List[str],
+                     profiles_keyword: str = BASE_PROFILES_KEYWORD,
+                     collection_keyword: str = BASE_COLLECTION_KEYWORD) -> dict:
     """
-    Process a nested dictionary of default YAML file paths, flattening the
-    dictionary, converting it to a list of paths, and ensuring each path has
-    a '.yaml' extension.
+    Load a YAML configuration file and update with profiles and collections.
 
     Args:
-        default_yaml (dict): A nested dictionary containing default YAML file paths.
+        config_path (str): The file path to the YAML configuration file.
+        config_name (str): The name of the YAML configuration file.
+        profiles_keyword (str): The keyword used to identify profiles in the YAML file. Defaults to "profiles".
 
     Returns:
-        List[str]: A list of processed and validated default YAML file paths.
+        dict: The updated configuration dictionary.
     """
-    default_yaml = dict_to_path(default_yaml)
-    default_yaml = [add_yaml_extension(filename) for filename in default_yaml]
-    return default_yaml
+    path = os.path.join(config_path, config_name)
+    config = open_yaml(path)
+
+    if profiles_keyword in config:
+        unpack_profiles(config, config_path, profile, profile_specifiers, profiles_keyword)
 
+    if collection_keyword in config:
+        unpack_collection(config, config_path, collection_keyword)
+
+    
+    return config
 
-def get_default_args_from_dict(config_path: str, default_yaml: dict) -> dict:
+def override_profile_with_specifier(profile_dict: dict, specifier: str, config: dict):
     """
-    Load a YAML default configuration files in dict format and returns a dictionary of args.
+    Will take the section of the config indicated by the specifier and place it in the profile.
+    If such a section does not exist in the profile, it will be created. If it does, it will be 
+    overwritten. If the specifier does not match a subprofile in the config, this will throw an
+    error.
 
     Args:
-        config_path (str): The file path to the YAML configuration file.
-        default_yml (dict): A dictionary data structure representing the paths to many
-            YAML configuration files.
+        profile_dict (dict): The dictionary holding the profile to be overwritten.
+        specifier (str): The dot-notation specifier referencing which subconfig to bring into
+            the profile
+        config (dict): The profiles config dictionary holding all of the profiles.
+    """
 
-    Returns:
-        dict: The updated configuration dictionary."""
-    yaml_paths = get_default_yaml_paths_from_dict(default_yaml)
-    default_configs = [
-        open_yaml(os.path.join(config_path, yaml_path)) for yaml_path in yaml_paths
-    ]
-    default_config = {
-        key: value
-        for config_dict in default_configs
-        if config_dict
-        for key, value in config_dict.items()
-    }
-    return default_config
 
+    alt_profile, *split_specifier, final_key = specifier.split(".")
+    config = config[alt_profile]
+
+    for key in split_specifier:
+        if key not in config:
+            raise ValueError(f"The given profile specifier ({specifier}) can't be matched to any profiles.")
+        elif key not in profile_dict.keys():
+            profile_dict[key] = {}
+
+        config  = config[key]
+        profile_dict = profile_dict[key]
+
+    profile_dict[final_key] = config[final_key]
 
 def get_default_args_from_path(config_path: str, default_yaml: str) -> dict:
     """
     Load a YAML default configuration files and returns a dictionary of args.
 
     Args:
         config_path (str): The file path to the YAML base configuration file.
@@ -277,69 +294,79 @@
         dict: The updated configuration dictionary.
     """
     default_yaml = add_yaml_extension(default_yaml)
     default_config_path = os.path.join(config_path, default_yaml)
     default_config = open_yaml(default_config_path)
     return default_config
 
+def unpack_profiles(config, config_path: str, profile: str, profile_specifiers: List[str], profiles_keyword: str):
+    default_paths = None
+    
+    if isinstance(config[profiles_keyword], dict):
+        # Get the default profile or the given profile
+        default_profile = []
+        for key, val  in list(config[profiles_keyword].items()):
+            if key[0] == "~":
+                default_profile.append(key[1:])
+
+                config[profiles_keyword][key[1:]] = val
+                del config[profiles_keyword][key]
+
+        if len(default_profile) > 1:
+            raise ValueError("Only one profile may be specified as default.")
+        elif len(default_profile) == 0 and profile is None:
+            raise ValueError("You must specify a profile or assign one to as default using the '~' prefix.")
+        elif profile is None:
+            profile = default_profile[0]
+
+        profile_dict = config[profiles_keyword][profile]
+        for specifier in profile_specifiers:
+            override_profile_with_specifier(profile_dict, specifier, config[profiles_keyword])
+
+
+        # Perform BFS on the profile to get all of the paths
+        default_paths = []
+        queue = [profile_dict]
+        while len(queue) != 0:
+            current_subdict = queue.pop(0)
+            for k, v in current_subdict.items():
+                if isinstance(v, dict):
+                    queue.append(v)
+                elif isinstance(v, str):
+                    default_paths.append(v)
+                elif isinstance(v, list):
+                    default_paths.extend(v)
+                else:
+                    ValueError(f"The type of {v} ({type(v)}) is not a valid path to a default config.")
+    
+    elif isinstance(config[profiles_keyword], list):
+        default_paths = config[profiles_keyword]
+    
+    elif isinstance(config[profiles_keyword], str):
+        default_paths = [config[profiles_keyword]]
 
-def load_yaml_config(
-    config_path: str, config_name: str, default_keyword: str = BASE_DEFAULT_KEYWORD, collection_keyword: str = BASE_COLLECTION_KEYWORD
-) -> dict:
-    """
-    Load a YAML configuration file and update it with default configurations.
-
-    Args:
-        config_path (str): The file path to the YAML configuration file.
-        config_name (str): The name of the YAML configuration file.
-        default_keyword (str): The keyword used to identify default configurations
-            in the YAML file. Defaults to "defaults".
-
-    Returns:
-        dict: The updated configuration dictionary.
-    """
-    path = os.path.join(config_path, config_name)
-    config = open_yaml(path)
-
-    if default_keyword in config:
-        default_path_dict = config[default_keyword]
-        if isinstance(default_path_dict, dict):
-            default_config = get_default_args_from_dict(config_path, default_path_dict)
-
-            if default_config:
-                config.update(
-                    (key, value)
-                    for key, value in default_config.items()
-                    if key not in config
-                )
-        else:
-            for default_yaml in default_path_dict:
-                if isinstance(default_yaml, dict):
-                    default_config = get_default_args_from_dict(
-                        config_path, default_yaml
-                    )
-
-                elif isinstance(default_yaml, str):
-                    default_config = get_default_args_from_path(
-                        config_path, default_yaml
-                    )
-
-                if default_config:
-                    config.update(
-                        (key, value)
-                        for key, value in default_config.items()
-                        if key not in config
-                    )
-        del config[default_keyword]
-
-    if collection_keyword in config:
-        unpack_collection(config, config_path, collection_keyword)
+    else:
+        ValueError(f" The value '{config[profiles_keyword]}' is not valid for profiles.")
 
+    # Apply all of the paths to the config
+    for default_path in default_paths:
+        default_config = get_default_args_from_path(
+            config_path, default_path)
+
+        if default_config:
+            config.update(
+                (key, value)
+                for key, value in default_config.items()
+                if key not in config
+            )
     
-    return config
+    del config[profiles_keyword]
+
+def unpack_single_profile():
+    pass
 
 def unpack_collection(config, config_path, collection_keyword):
         collections_dict = config[collection_keyword]
         
         for collection_key in collections_dict.keys():
             if collection_key in config:
                 return ValueError("You cannot have a collection with the same name as an argument.")
@@ -404,33 +431,51 @@
     return Config({
         key: yaml.safe_load(value) if isinstance(value, str) else value
         for key, value in vars(flat_config).items()
     })
         
 
 
-def get_command_line_config(arg_parser: argparse.ArgumentParser, config_argument_keyword: str="config") -> Tuple[str, List[str]]:
+def parse_initial_args(arg_parser: argparse.ArgumentParser,
+                            config_argument_keyword: str="config", 
+                            profiles_keyword: str = BASE_PROFILES_KEYWORD) -> Tuple[str, List[str]]:
     """
-    Check to see if the user specified an alternative config via the command line. If so,
-    return the path of that config, and the remaining arguments. Otherwise, return None
-    and the remaining arguments.
+    Check to see if the user specified a config or profile information via the command line. If so,
+    return the path of that config, any profiles information, and the used keywords. Otherwise, return None
 
     Args:
         arg_parser (argparse.ArgumentParser): The argparse object to add the config arg to.
         config_argument_keyword (str): Default keyword to accept new config path from the 
             command line.
+        profiles_keyword (str): Default keyword for profiles
     
     Returns:
         str: A string of the path to the alternate config.
-        List[str]: All remaining arguments.
+        str: The specified profile
+        List[str]: A list of the profile specifiers.
+        List[str]: The argument names used by the initial args that should be ignored at later steps
     """
-    arg_parser.add_argument(f"--{config_argument_keyword}", default=None, type=str)
-    known_args, unknown_args = arg_parser.parse_known_args()
-    config_path = vars(known_args)[config_argument_keyword]
-    return config_path, unknown_args
+
+    arg_parser.add_argument("_main_profile", metavar="profile", type=str, nargs="?", default=None)
+    arg_parser.add_argument(f"--{config_argument_keyword}", dest="_alt_config_name", default=None, type=str)
+    arg_parser.add_argument(f"--{profiles_keyword}", metavar="Profile Specifiers", dest="_profile_specifiers", type=str, nargs="*", default=[])
+
+    known_args, _ = arg_parser.parse_known_args()
+    
+    profile = known_args._main_profile
+    profile_specifiers = known_args._profile_specifiers
+    
+    if "." not in profile_specifiers[0]:
+        if profile is not None:
+            raise ValueError(f"Cannot specify profile in two places: {profile} vs. {profile_specifiers[0]}")
+        profile = profile_specifiers[0]
+        del profile_specifiers[0]
+
+    config_path = known_args._alt_config_name
+    return config_path, profile, profile_specifiers, ["_main_profile", "_alt_config_name", "_profile_specifiers"]
 
 
 def config_to_nested_config(config: Config) -> Config:
     """
     Convert an Config object with 'key1.keyn' formatted keys into a nested Config object.
 
     Args:
```

### Comparing `skeletonkey-0.2.13/skeletonkey/core.py` & `skeletonkey-0.3.0.0/skeletonkey/core.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import argparse
 import functools
 import os
 import sys
 from typing import Callable, Optional
 
 from .config import (
-    get_command_line_config,
+    parse_initial_args,
     load_yaml_config,
     add_args_from_dict,
     add_yaml_extension,
     update_flat_config_types,
     config_to_nested_config,
     Config
 )
@@ -42,55 +42,59 @@
             path_from_main = os.path.dirname(path_from_main)
 
         # Create absolute path.
         config_path = os.path.join(path_from_main, config_path)
     return config_path
 
 
-def unlock(config_name: Optional[str] = None, config_path: Optional[str] = None) -> Callable:
+def unlock(config_name: Optional[str] = None, config_dir: Optional[str] = None) -> Callable:
     """
     Create a decorator for parsing and injecting configuration arguments into a
     main function from a YAML file.
 
     Args:
         config_name (str): The name of the YAML configuration file.
         config_path (str): The path to the directory containing the configuration
                            file. Defaults to the current directory.
 
     Returns:
         Callable: A decorator function that, when applied to a main function, will
                   parse the configuration file and inject the arguments into the
                   main function.
     """
-    parser = argparse.ArgumentParser()
-    command_line_config_path, remaining_args = get_command_line_config(parser)
+    # Parse high-level arguments
+    parser = argparse.ArgumentParser()    
+    config_dir_command_line, profile, profile_specifiers, temp_args = parse_initial_args(parser)
     
-    if command_line_config_path:
-        config_name = os.path.abspath(command_line_config_path)
-        config_path = None
 
-    if config_name == None and command_line_config_path == None:
+    # Find final config name and directory
+    if config_dir_command_line is not None:
+        config_name = os.path.abspath(config_dir_command_line)
+        config_dir = None
+    elif config_name is not None:
+        config_dir = get_config_dir_path(os.path.dirname(config_name))
+    else: 
         raise ValueError("config path is neither specified in 'unlock' nor via the command line.")
-    
-    config_path = config_path if config_path else os.path.dirname(config_name)
-    
-    if not command_line_config_path:
-        config_path = get_config_dir_path(config_path)
-
-    config_name = add_yaml_extension(config_name)
-    config_name = os.path.basename(config_name)
-
-    config = load_yaml_config(config_path, config_name)
+    config_name = os.path.basename(add_yaml_extension(config_name))
 
+    # Create decorator
     def _parse_config(main: Callable):
         @functools.wraps(main)
         def _inner_function():
+            config = load_yaml_config(config_dir, config_name, profile, profile_specifiers)
+
             add_args_from_dict(parser, config)
-            args = parser.parse_args(remaining_args)
+
+            args = parser.parse_args()
             args = update_flat_config_types(args)
+
+            for temp_arg in temp_args:
+                del args[temp_arg]
+
             args = config_to_nested_config(args)
+
             return main(args)
 
         return _inner_function
 
     return _parse_config
```

### Comparing `skeletonkey-0.2.13/skeletonkey/instantiate.py` & `skeletonkey-0.3.0.0/skeletonkey/instantiate.py`

 * *Files identical despite different names*

### Comparing `skeletonkey-0.2.13/skeletonkey.egg-info/PKG-INFO` & `skeletonkey-0.3.0.0/skeletonkey.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skeletonkey
-Version: 0.2.13
+Version: 0.3.0.0
 Summary: A bare-bones configuration managment tool.
 Home-page: https://github.com/sizemore0125/skeletonkey
 Author: Logan Sizemore
 Author-email: sizemore0125@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

